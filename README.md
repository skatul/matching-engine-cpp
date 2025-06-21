Match Engine in C++
A high-performance trade matching engine written in C++, designed for real-time financial markets. This project aims to deliver a fast and efficient core for executing and matching orders in an order-driven exchange.

🚀 Key Features
Limit order book with O(1) access for top-of-book operations

Support for limit and market orders, IOC/FOK order types

Price-time priority matching logic

Real-time order insertion, cancellation, and execution

Multithreaded event processing for optimal latency

Logging and performance metrics collection

⚙️ Tech Stack
Language: C++17

Build System: CMake

Testing Framework: Google Test

Multithreading: std::thread, condition_variable

Optional: Boost.Asio or ZeroMQ for future gateway messaging

📁 Project Structure
/src
  Order.hpp / OrderBook.hpp / MatchingEngine.hpp  
/tests
  Unit tests for order and matching logic  
/scripts
  Startup scripts and performance test drivers  
README.md
CMakeLists.txt
📈 Performance Goals
Target latency: sub-100µs for order matching Target throughput: 100K+ orders per second

🧭 Future Enhancements
Add FIX/FAST protocol support for external connectivity

Introduce persistent storage with RocksDB for audit trails

Web dashboard for real-time book visualization

🛠️ Getting Started
To build the project:

bash
mkdir build && cd build  
cmake ..  
make  
Run unit tests:

bash
./run_tests
