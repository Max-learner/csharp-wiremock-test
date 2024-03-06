# Комментарии к заданию:
- не реализовал DI и не применил пару паттернов - пометил TODO места для применения паттернов
- почему-то билды собираются нестабильно(надеюсь, дебаг этого за рамками тестового:-)), это сильно увеличило время выполнения
- к сожалению, не до конца реализован мок на GET одной записи, не парсится todoId и не получается его вернуть в ответе. В других моках он работает
- хотелось бы в моках проверять валидность входящих запросов с помощью Matchers, пока не разобрался, как это заставить работать

# DI_in_Tests_Demo

## Dependencies
- [dotnet 6 SDK] (https://dotnet.microsoft.com/en-us/download/dotnet/6.0)
- [Wiremock.NET nuget packages](https://github.com/WireMock-Net/WireMock.Net)

## How to run
1. Clone this git repository
2. Build DIDemoTestProject.sln
3. Run RunWireMockServer.cmd
4. Run all tests in solution (All will be passed)

## How to learn
1. Clone this git repository
2. Checkout branch "feature/withoutDI" (or "withoutDI" tag in 'main' branch)
3. Watch my speech at the conference
  - 3.1 [Hesenbug 2023](https://heisenbug.ru/talks/8548145422db42068b64f30649349a82/)
  - 3.2 [Youtube](https://youtu.be/fofhl0ZyhNU?si=yaWM9eSh7tkZ6s7F)
  - 3.3 [HabrHabr](https://habr.com/ru/companies/kaspersky/articles/757980/)
4. Repeat the steps to embed the DI Container in the test solution
