.PHONY: run setup clean fresh__env

# @ to supresses echoing
run:
	python arbitrary_calculations.py $(var1) $(var2)

# Only executes when install.sh when install.sh has changed 
setup: install.sh
	#minillm
	@./install.sh

clean:
	@rm -rf __pycache__
	pip3 cache purge
	conda clean -a

fresh_env: fresh_env.sh
	#New env and cleanup
	@./fresh_env.sh
