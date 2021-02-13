
var := First
new := 1st.First

test : var := Second
#%e : override new := 2nd.Second
%r : override new := 2nd.Second

test: another
	@echo "test:"
	@echo "var => $(var)"
	@echo "new => $(new)"

another :
	@echo "another:"
	@echo "var => $(var)"
	@echo "new => $(new)"
	
rule :
	@echo "rule:"
	@echo "var => $(var)"
	@echo "new => $(new)"
