---
layout: post
title: "A Swift HTTP Server"
description: "A Simple HTTP Server with the Swift Network Framework"
image: ""

category: 
tags: []
---

```swift
import Foundation
import Network

func main() {
    
    let server = try! NWListener(using: .tcp, on: 8000)

    server.newConnectionHandler = { connection in
        print("Recieved a connection")
        let data = "hello, world".data(using: .utf8)
        
        
        connection.send(content: data, contentContext: .finalMessage, isComplete: true,  completion: .contentProcessed({error in
            if let error = error {
                print("\(error)")
                return
            }
            
            print("connection did send, data: \(String(data: data!, encoding: .utf8))")
        }))
            
        connection.start(queue: .main)
    }
    
    server.start(queue: .main)
    
    dispatchMain()
}

main()
```