build/web/${SOC}: $(shell find . -name '*.dart')
	mkdir -p build/${SOC}
	flutter config --build-dir=build/${SOC}
	flutter build web --web-renderer html --dart-define=SOC=${SOC}

.PHONY: all seva-web clean
all: seva-web
seva-web: build/web/${SOC}
clean:
	flutter config --build-dir=build/
	flutter clean
