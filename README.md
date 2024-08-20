# testcontainers-go-demo

Testcontainers is an open source framework for provisioning throwaway, on-demand containers for development and testing
use cases.
Testcontainers make it easy to work with databases, message brokers, web browsers, or just about anything that can run
in a Docker container.

### Things todo list

1. Clone this repository: `git clone https://github.com/hendisantika/testcontainers-go-demo.git`
2. Navigate to the folder: `cd testcontainers-go-demo`
3. Run the test: `go test -v ./...`
4. Check the console log

Run command:

```shell
hendisantika@Hendis-MacBook-Pro testcontainers-go-demo % go test -v ./...
?       testcontainers-go-demo  [no test files]
?       testcontainers-go-demo/testhelpers      [no test files]
=== RUN   TestCustomerRepoTestSuite
2024/08/20 15:38:51 github.com/testcontainers/testcontainers-go - Connected to docker: 
  Server Version: 27.1.1 (via Testcontainers Desktop 1.15.1)
  API Version: 1.46
  Operating System: Docker Desktop
  Total Memory: 7837 MB
  Testcontainers for Go Version: v0.32.0
  Resolved Docker Host: tcp://127.0.0.1:49690
  Resolved Docker Socket Path: /var/run/docker.sock
  Test SessionID: ccbf734e92809f02d4b5c73c544414936a05e13239498660321001c4ca445f46
  Test ProcessID: 607e2f77-eb68-4d86-b3b8-2a832a1dad6f
2024/08/20 15:38:59 🐳 Creating container for image testcontainers/ryuk:0.7.0
2024/08/20 15:38:59 ✅ Container created: bf4b3d1c6729
2024/08/20 15:38:59 🐳 Starting container: bf4b3d1c6729
2024/08/20 15:38:59 ✅ Container started: bf4b3d1c6729
2024/08/20 15:38:59 ⏳ Waiting for container id bf4b3d1c6729 image: testcontainers/ryuk:0.7.0. Waiting for: &{Port:8080/tcp timeout:<nil> PollInterval:100ms}
2024/08/20 15:39:00 🔔 Container is ready: bf4b3d1c6729
2024/08/20 15:39:00 🐳 Creating container for image postgres:17beta3-alpine3.20
2024/08/20 15:39:00 ✅ Container created: a9c78f358447
2024/08/20 15:39:00 🐳 Starting container: a9c78f358447
2024/08/20 15:39:00 ✅ Container started: a9c78f358447
2024/08/20 15:39:00 ⏳ Waiting for container id a9c78f358447 image: postgres:17beta3-alpine3.20. Waiting for: &{timeout:<nil> deadline:0x140006084b0 Strategies:[0x1400026e0c0]}
2024/08/20 15:39:00 🔔 Container is ready: a9c78f358447
=== RUN   TestCustomerRepoTestSuite/TestCreateCustomer
=== RUN   TestCustomerRepoTestSuite/TestGetCustomerByEmail
2024/08/20 15:39:00 🐳 Terminating container: a9c78f358447
2024/08/20 15:39:01 🚫 Container terminated: a9c78f358447
--- PASS: TestCustomerRepoTestSuite (9.08s)
    --- PASS: TestCustomerRepoTestSuite/TestCreateCustomer (0.00s)
    --- PASS: TestCustomerRepoTestSuite/TestGetCustomerByEmail (0.00s)
=== RUN   TestCustomerRepository
2024/08/20 15:39:01 🐳 Creating container for image postgres:17beta3-alpine3.20
2024/08/20 15:39:01 ✅ Container created: b01ee7ead810
2024/08/20 15:39:01 🐳 Starting container: b01ee7ead810
2024/08/20 15:39:01 ✅ Container started: b01ee7ead810
2024/08/20 15:39:01 ⏳ Waiting for container id b01ee7ead810 image: postgres:17beta3-alpine3.20. Waiting for: &{timeout:<nil> deadline:0x140004b11d0 Strategies:[0x14000322360]}
2024/08/20 15:39:01 🔔 Container is ready: b01ee7ead810
2024/08/20 15:39:01 🐳 Terminating container: b01ee7ead810
2024/08/20 15:39:01 🚫 Container terminated: b01ee7ead810
--- PASS: TestCustomerRepository (0.90s)
PASS
ok      testcontainers-go-demo/customer 10.392s

```