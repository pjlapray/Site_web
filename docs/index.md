# Test de rendu final
Voici une équation centrée (LaTeX) :

$$
t_{pd} = \sum_{i=1}^{n} t_{logic\_i}
$$

Voici un exemple de compteur :

```vhdl
library IEEE;
use IEEE.STD_LOGIC_1164.ALL;

entity counter is
port ( 
	clk9 : in std_logic;
	reset : in std_logic
);
end counter;
architecture rtl of counter is
begin
process(clk)
begin
	if rising_edge(clk) then
	-- La coloration syntaxique doit apparaître ici
	end if;
						end process;
end rtl; 
```

<iframe src="https://edaplayground.com/x/ejkp" width="100%" height="500px" frameborder="0"></iframe>
