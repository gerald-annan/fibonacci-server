# FibonacciServer

**TODO: Add description**

Let’s round out this chapter with an example program. Its task is to calculate
fib(n) for a list of n, where fib(n) is the nth Fibonacci number. (The Fibonacci
sequence starts 0, 1. Each subsequent number is the sum of the preceding
two numbers in the sequence.)2 I chose this not because it is something we
all do every day, but because the naive calculation of Fibonacci numbers 10
through 37 takes a measurable number of seconds on typical computers.
The twist is that we’ll write our program to calculate different Fibonacci
numbers in parallel. To do this, we’ll write a trivial server process that does
the calculation, and a scheduler that assigns work to a calculation process
when it becomes free.

## Installation

If [available in Hex](https://hex.pm/docs/publish), the package can be installed
by adding `fibonacci_server` to your list of dependencies in `mix.exs`:

```elixir
def deps do
  [
    {:fibonacci_server, "~> 0.1.0"}
  ]
end
```

Documentation can be generated with [ExDoc](https://github.com/elixir-lang/ex_doc)
and published on [HexDocs](https://hexdocs.pm). Once published, the docs can
be found at [https://hexdocs.pm/fibonacci_server](https://hexdocs.pm/fibonacci_server).
