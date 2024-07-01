# E-o-Oscar-vai-para... 🏆 🕴 🎬 🎥-
And the Oscar goes to... 🏆 🕴 🎬 🎥

1 Quantas vezes Natalie Portman foi indicada ao Oscar?
SELECT * FROM indicados_ao_oscar WHERE nome_do_indicado = 'nathalie portman' 
return: 3
 
ou
 
SELECT COUNT(*) AS indicados_ao_oscar
FROM indicados_ao_oscar
WHERE nome_do_indicado = 'Natalie Portman';
 
-- 2 Quantos Oscars Natalie Portman ganhou?
apenas 1
 
-- 3 Amy Adams já ganhou algum Oscar?
SELECT *
FROM indicados_ao_oscar
WHERE ano_cerimonia = 2024 AND vencedor = 'Sim';
 
-- 4 A série de filmes Toy Story ganhou um Oscar em quais anos?
UPDATE indicados_ao_oscar
SET vencedor = 'Sim'
WHERE ano_filmagem = %2024% AND categoria = nome_do_indicado = 'Toy Story';
 
-- 5 
DELETE FROM indicados_ao_oscar
WHERE Actress = % ;
 
-- 6 
SELECT nome_do_indicado, MIN(ano_filmagem)
FROM indicados_ao_oscar
WHERE categoria = 'Melhor Atriz' AND vencedor = 'Sim';
 
-- 7 UPDATE indicados_ao_oscar
SET vencedor = CASE 
    WHEN vencedor = 'Sim' THEN 1
    WHEN vencedor = 'Não' THEN 0
    ELSE vencedor
END;
 
-- 8 SELECT DISTINCT cerimonia
FROM indicados_ao_oscar
WHERE nome_do_filme LIKE '%Crash%';
 
-- 9 INSERT INTO indicados_ao_oscar (ano_filmagem, ano_cerimonia, cerimonia, categoria, nome_do_indicado, nome_do_filme, vencedor)
VALUES (2023, 2024, 96, '%', 'Great Film', 'The Great Movie', 'Sim');
 
-- 10 SELECT *
FROM indicados_ao_oscar
WHERE nome_do_filme LIKE '%Central do Brasil%';
 
-- 11 SELECT DISTINCT cerimonia
FROM indicados_ao_oscar
WHERE nome_do_filme LIKE '%Crash%';
 
-- 12 UPDATE indicados_ao_oscar
SET nome_do_filme = 'The Matrix 8', ano_filmagem = 2040
WHERE categoria = 'Melhor Filme' AND nome_do_indicado = 'Great Film' AND ano_filmagem = 2025;
 
-- 13 SELECT *
FROM indicados_ao_oscar
WHERE nome_do_filme LIKE '%Central do Brasil%';
 
-- 14 INSERT INTO indicados_ao_oscar (ano_filmagem,  nome_do_filme, vencedor)
VALUES 
(1987, 'The Wolf of Wall Street', 'Não'),
(2002, 'Cidade de Deus', 'Não'),
(1998, 'Central do Brasil', 'Não');
 
-- 15 SELECT nome_do_indicado, nome_do_filme, cerimonia
 
-- dar update p atualizar o database
FROM indicados_ao_oscar
 
WHERE categoria IN ('Uma Mente Brilhante', 'Jennifer Connelly', 'David Lean') AND ano_filmagem = 2002 AND vencedor = 'Sim';
tem menu de contexto
