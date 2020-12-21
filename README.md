# Mutex-cpp
A lightweight, basic C++ templated Mutex.

### Basic usage setup

```cpp
struct Example {
    void do_something() const {
        std::cout << "Something" << std::endl;
    }
};

int main() {
    Mutex<Example> x{};
    x.acquire()->do_something(); // acquire rights and call do_something()
}