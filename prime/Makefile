all:	clean
	gcc -O3 -ffast-math -o prime main.c
test:	all
	./prime input.txt >output.txt
	diff output.txt expected.txt
get-assets:
	wget https://github.com/soallpeach/onboarding/raw/master/challenges/prime/input.txt
	wget https://github.com/soallpeach/onboarding/raw/master/challenges/prime/expected.txt
clean:
	rm -f prime
	rm -f output.txt
clean-all:	clean
	rm -f input.txt
	rm -f expected.txt
