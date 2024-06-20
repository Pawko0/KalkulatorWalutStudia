cmake_minimum_required(VERSION 3.27)
project(Kalkulator)

set(CMAKE_CXX_STANDARD 17)

configure_file(CurrencyExchangeRates.txt ${CMAKE_CURRENT_BINARY_DIR}/CurrencyExchangeRates.txt COPYONLY)

add_executable(Kalkulator main.cpp
        Currency.cpp
        Currency.h
        BankAccount.cpp
        BankAccount.h
        SpecialBankAccount.cpp
        SpecialBankAccount.h
        Service.cpp
        Service.h
)
