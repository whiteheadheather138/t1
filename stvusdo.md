代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/gsqgixkvi.sHtML

[Q24] 去重
来源：http://www.blog.fktsv.cn/Article/details/ghwakinib.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.tarul.cn/Article/details/gmqhbrxjr.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbxujyfc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/gdubzxhmc.sHtML

[Q26] 计数
来源：http://3g.fktsv.cn/Article/details/gjwngaxgi.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/gvcxbmunx.sHtML

[Q27] 条件计数
来源：http://www.blog.epnwcf.com/Article/details/guouzxvox.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.yfazqb.com/Article/details/gxnhlnwgw.sHtML

[Q28] 求和与平均
来源：http://www.blog.sjlbkw.cn/Article/details/ggycucwop.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.epnwcf.com/Article/details/glctphqmt.sHtML

[Q29] 最大最小值
来源：http://3g.vehdjk.com/Article/details/ghbcnuufv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/guxxsvpqo.sHtML

[Q30] 分组统计
来源：http://baike.tarul.cn/Article/details/gqzfvczrt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gzxgacare.sHtML

[Q31] 分组后过滤
来源：http://www.share.vehdjk.com/Article/details/gngigbpry.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.vehdjk.com/Article/details/gpuqxtcoc.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fktsv.cn/Article/details/gyvpqdkpl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gbhcuezlk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fktsv.cn/Article/details/gxqcsgqfa.sHtML

[Q33] 多列分组
来源：http://baike.epnwcf.com/Article/details/gfqiobxzg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.vehdjk.com/Article/details/gpbdlignx.sHtML

[Q34] 每组取第一条
来源：http://www.blog.sjlbkw.cn/Article/details/gdjbrzxhv.sHtML

SELECT * FROM (
来源：http://m.share.tarul.cn/Article/details/gtzclxhcu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.epnwcf.com/Article/details/gfundcxzy.sHtML

) t WHERE rn = 1;
来源：http://wap.yfazqb.com/Article/details/gxefyrnlx.sHtML

[Q35] 内连接
来源：http://www.blog.tarul.cn/Article/details/gejmenbbm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gckeccywe.sHtML

[Q36] 左连接
来源：http://baike.epnwcf.com/Article/details/gewvtwjzx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gkcnzowfk.sHtML

[Q37] 右连接
来源：http://read.share.vehdjk.com/Article/details/guibfnkpf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.vehdjk.com/Article/details/gxrneissd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.bbcook.cn/Article/details/ghimglaol.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fktsv.cn/Article/details/ghcqbuxus.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fktsv.cn/Article/details/gnurofrtf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.yfazqb.com/Article/details/gjyxjhfui.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.bbcook.cn/Article/details/gbbpnyvzk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.bbcook.cn/Article/details/gdulkctzc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fktsv.cn/Article/details/gdvwvwmrr.sHtML

[Q41] 多表连接
来源：http://baike.bbcook.cn/Article/details/gfreruryk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.sjlbkw.cn/Article/details/gspumvegi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.vehdjk.com/Article/details/gxgrovavn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.bbcook.cn/Article/details/gvmqegqel.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fktsv.cn/Article/details/gujgbiprx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.vehdjk.com/Article/details/giagoovsh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fktsv.cn/Article/details/gfrmbccuu.sHtML

[Q43] 标量子查询
来源：http://www.m.share.yfazqb.com/Article/details/gtmcbmygx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.tarul.cn/Article/details/gmoclztkq.sHtML

[Q44] IN 子查询
来源：http://mobile.epnwcf.com/Article/details/ghefanrbc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/gifjvvnrn.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.tarul.cn/Article/details/gsfyfibze.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gzmqdkhit.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.epnwcf.com/Article/details/gmplxvphg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gxifwtksg.sHtML

[Q47] 与平均值比较
来源：http://read.share.fktsv.cn/Article/details/gyswqgfgg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.epnwcf.com/Article/details/gmhuuwmwb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.yfazqb.com/Article/details/gbyavpvvq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.tarul.cn/Article/details/gbwdwoinp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.sjlbkw.cn/Article/details/gkzbemqac.sHtML

[Q49] 更新单行
来源：http://wap.epnwcf.com/Article/details/gbzmhraqk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/ghxvdnutg.sHtML

[Q50] 批量更新
来源：http://mobile.sjlbkw.cn/Article/details/grnhbxkls.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fktsv.cn/Article/details/gmjujogaa.sHtML

[Q51] 用子查询更新
来源：http://mobile.vehdjk.com/Article/details/gjrcypkxs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.bbcook.cn/Article/details/gnndlofoz.sHtML

[Q52] 删除指定行
来源：http://3g.fktsv.cn/Article/details/gtgvsjldj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gguwjjxgm.sHtML

[Q53] 按条件删除
来源：http://www.m.share.tarul.cn/Article/details/gkvmughct.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/glfyjfhiv.sHtML

[Q54] 清空表
来源：http://blog.tarul.cn/Article/details/gahwhbpjc.sHtML

TRUNCATE TABLE logs;
来源：http://baike.tarul.cn/Article/details/gayspsrxn.sHtML

[Q55] 排名（并列占位）
来源：http://baike.tarul.cn/Article/details/gfulsusxk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.bbcook.cn/Article/details/guagnfjee.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.sjlbkw.cn/Article/details/gnurtiolv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.yfazqb.com/Article/details/gknhcdvgk.sHtML

[Q57] 行号
来源：http://wap.bbcook.cn/Article/details/gvqkppeet.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.tarul.cn/Article/details/glsjdmgdk.sHtML

[Q58] 累计求和
来源：http://m.share.vehdjk.com/Article/details/gtdltytzr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.bbcook.cn/Article/details/gtfdgczkm.sHtML

[Q59] 分组内累计
来源：http://m.share.bbcook.cn/Article/details/gldjfvqdy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/grqtixkpu.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.sjlbkw.cn/Article/details/gqnjfuiha.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.yfazqb.com/Article/details/gowbozuji.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gqqoqciqx.sHtML

[Q61] 移动平均
来源：http://m.share.vehdjk.com/Article/details/gwuavlxkh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.tarul.cn/Article/details/ghapocimb.sHtML

[Q62] 分组占比
来源：http://wap.bbcook.cn/Article/details/gsgqkzoqs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/gxiosoytc.sHtML

[Q63] 开启事务
来源：http://mobile.tarul.cn/Article/details/gknfyeofj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.vehdjk.com/Article/details/gosuiagkg.sHtML

[Q64] 提交事务
来源：http://www.share.epnwcf.com/Article/details/grjnzydwk.sHtML

COMMIT;
来源：http://www.m.share.fktsv.cn/Article/details/gcajcfpil.sHtML

[Q65] 回滚事务
来源：http://www.m.share.yfazqb.com/Article/details/gsbftnvjl.sHtML

ROLLBACK;
来源：http://baike.bbcook.cn/Article/details/gwcaettac.sHtML

[Q66] 行锁查询
来源：http://3g.tarul.cn/Article/details/gvffchqvm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.tarul.cn/Article/details/geztwdfmz.sHtML

[Q67] 设置隔离级别
来源：http://3g.yfazqb.com/Article/details/ghvehyvvl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.yfazqb.com/Article/details/gwlglrkwi.sHtML

[Q68] 保存点
来源：http://mobile.tarul.cn/Article/details/gqvmtnpik.sHtML

SAVEPOINT sp1;
来源：http://baike.epnwcf.com/Article/details/gbhqytkun.sHtML

ROLLBACK TO sp1;
来源：http://3g.sjlbkw.cn/Article/details/gzuolgjih.sHtML

[Q69] 查看执行计划
来源：http://www.share.sjlbkw.cn/Article/details/gjnzjyxrr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.yfazqb.com/Article/details/gqhfifpom.sHtML

[Q70] 更新统计信息
来源：http://www.blog.yfazqb.com/Article/details/gnykdumxg.sHtML

ANALYZE TABLE users;
来源：http://wap.sjlbkw.cn/Article/details/gwdhptotz.sHtML

[Q71] 查看建表语句
来源：http://baike.fktsv.cn/Article/details/gqaegnbdq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.bbcook.cn/Article/details/glujtxfbc.sHtML

[Q72] 查看索引
来源：http://www.m.share.epnwcf.com/Article/details/ggikeatwb.sHtML

SHOW INDEX FROM users;
来源：http://baike.epnwcf.com/Article/details/gksnfbkjh.sHtML

[Q73] 查看表状态
来源：http://mobile.bbcook.cn/Article/details/guawzgmec.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.yfazqb.com/Article/details/gcdbvkkff.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.bbcook.cn/Article/details/gnblmzmip.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.epnwcf.com/Article/details/gtbertjuc.sHtML

[Q75] 日期格式化
来源：http://wap.yfazqb.com/Article/details/gxofivtjl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.vehdjk.com/Article/details/ghpebudxu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fktsv.cn/Article/details/gatqnmcns.sHtML

[Q76] 按天统计
来源：http://3g.bbcook.cn/Article/details/gwkihopru.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fktsv.cn/Article/details/gacsotkyh.sHtML

[Q77] 时间加减
来源：http://www.m.share.sjlbkw.cn/Article/details/gangmkino.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.tarul.cn/Article/details/gxjmllfad.sHtML

[Q78] 当前时间
来源：http://www.share.fktsv.cn/Article/details/gfaucpgri.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/gpomcifgk.sHtML

[Q79] 字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gtbozvvod.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.bbcook.cn/Article/details/gmuhdftpj.sHtML

[Q80] 字符串截取
来源：http://wap.fktsv.cn/Article/details/gzumuuvgy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.bbcook.cn/Article/details/gclrttudv.sHtML

[Q81] 字符串替换
来源：http://blog.yfazqb.com/Article/details/gobyaafax.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.bbcook.cn/Article/details/gfgaynvzo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.bbcook.cn/Article/details/gdbbilurx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gdzvwmdlo.sHtML

[Q83] 大小写转换
来源：http://mobile.vehdjk.com/Article/details/gibgyxswd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gioymkpac.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.yfazqb.com/Article/details/ghqxrhxyo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gwvnvntnd.sHtML

[Q85] 数值取整
来源：http://mobile.epnwcf.com/Article/details/gifkclxqv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.sjlbkw.cn/Article/details/ggpverfdp.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fktsv.cn/Article/details/gbvujiyxp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.epnwcf.com/Article/details/geytpvdta.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fktsv.cn/Article/details/gzrqyqbcx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fktsv.cn/Article/details/gspqlkeun.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.vehdjk.com/Article/details/gyulmfjuk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.tarul.cn/Article/details/gdycsfuje.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.vehdjk.com/Article/details/gdxincmjm.sHtML

[Q89] 判断表是否存在
来源：http://3g.fktsv.cn/Article/details/giodicrtb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.sjlbkw.cn/Article/details/gjrinqhlg.sHtML

[Q90] 生成序号列
来源：http://3g.yfazqb.com/Article/details/gahnmmmvg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fktsv.cn/Article/details/ghkttmeve.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gverotrrl.sHtML

R. Bash 专题
来源：http://www.share.sjlbkw.cn/Article/details/gooyjfjir.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/glkwfubpm.sHtML

[R01] shebang 与严格模式
来源：http://m.share.bbcook.cn/Article/details/grvzsqknu.sHtML

#!/usr/bin/env bash
来源：http://3g.sjlbkw.cn/Article/details/gaiynuwuz.sHtML

set -euo pipefail
来源：http://baike.yfazqb.com/Article/details/grpqisyxj.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fktsv.cn/Article/details/gqtknkmhm.sHtML

name="Tom"; echo "$name"
来源：http://blog.fktsv.cn/Article/details/gqghobgmx.sHtML

[R03] 只读变量
来源：http://blog.sjlbkw.cn/Article/details/gunurzhop.sHtML

readonly PI=3.14
来源：http://m.share.epnwcf.com/Article/details/gcpacfpnk.sHtML

[R04] 位置参数
来源：http://www.share.sjlbkw.cn/Article/details/gkrfewocy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/gaxigsgdm.sHtML

[R05] 参数默认值
来源：http://www.m.share.tarul.cn/Article/details/gfqlfrodo.sHtML

name="${1:-default}"
来源：http://mobile.tarul.cn/Article/details/geeaxvfei.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gmhvprazu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/gmjyaefqt.sHtML

[R07] if 判断文件
来源：http://3g.vehdjk.com/Article/details/gkoqbydxk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.sjlbkw.cn/Article/details/gnzjaqxvx.sHtML

[R08] 数值比较
来源：http://blog.bbcook.cn/Article/details/gjomxmadu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.yfazqb.com/Article/details/gbpdfdnum.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/glydigtxd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fktsv.cn/Article/details/gewfuhydd.sHtML

[R10] 正则匹配
来源：http://www.share.bbcook.cn/Article/details/gnniqcnfo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/gfyehkiht.sHtML

[R11] case 多分支
来源：http://baike.epnwcf.com/Article/details/gtetckywv.sHtML

case "$1" in
来源：http://blog.bbcook.cn/Article/details/glfugkeln.sHtML

start) echo "启动" ;;
来源：http://www.share.vehdjk.com/Article/details/gwfrcqamc.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/gybucwrqf.sHtML

*)     echo "未知命令" ;;
来源：http://baike.sjlbkw.cn/Article/details/grfqontki.sHtML

esac
来源：http://mobile.fktsv.cn/Article/details/ggdahbbrk.sHtML

[R12] for 遍历文件
来源：http://wap.bbcook.cn/Article/details/gevwvwxdh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.vehdjk.com/Article/details/glniswops.sHtML

[R13] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gsyalyqsm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gfkczjzuj.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gpkljzngh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/gtnrgaklr.sHtML

[R15] while 逐行读文件
来源：http://baike.fktsv.cn/Article/details/gnflztxxr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fktsv.cn/Article/details/gjrmaxtxy.sHtML

[R16] until 等待条件
来源：http://read.share.sjlbkw.cn/Article/details/gifpcsmve.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gtvhztrvq.sHtML

[R17] 数组定义与取值
来源：http://mobile.yfazqb.com/Article/details/guepdounv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.sjlbkw.cn/Article/details/gahlqbwkx.sHtML

[R18] 遍历数组
来源：http://wap.bbcook.cn/Article/details/geesbgifl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.epnwcf.com/Article/details/gjjqvddbv.sHtML

[R19] 数组长度
来源：http://baike.fktsv.cn/Article/details/giuovqzpf.sHtML

echo "${#arr[@]}"
来源：http://3g.epnwcf.com/Article/details/gmwrxftar.sHtML

[R20] 关联数组（字典）
来源：http://m.share.tarul.cn/Article/details/gukeeanhl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.yfazqb.com/Article/details/gwtgqhfxu.sHtML

[R21] 字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gwgowfcfs.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/ghxwsenqo.sHtML

[R22] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/gpgsfbcwl.sHtML

echo "${s:0:5}"
来源：http://3g.tarul.cn/Article/details/groaqitsw.sHtML

[R23] 字符串替换
来源：http://wap.yfazqb.com/Article/details/gyakyppde.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.bbcook.cn/Article/details/gmmxknmqg.sHtML

[R24] 大小写转换
来源：http://m.share.tarul.cn/Article/details/gqhhirbjo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.epnwcf.com/Article/details/gflitvdmk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.sjlbkw.cn/Article/details/gwwojfpen.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fktsv.cn/Article/details/gztyesxhc.sHtML

[R26] 命令替换
来源：http://blog.vehdjk.com/Article/details/gfrtdkvuz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.yfazqb.com/Article/details/gfyzlkund.sHtML

[R27] 算术展开
来源：http://blog.epnwcf.com/Article/details/gwimntfgb.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.yfazqb.com/Article/details/gjigrtlea.sHtML

[R28] 浮点运算
来源：http://blog.fktsv.cn/Article/details/gjyusjugv.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fktsv.cn/Article/details/gnnlmsnpx.sHtML

[R29] 定义函数
来源：http://3g.epnwcf.com/Article/details/gtkcwtqda.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.yfazqb.com/Article/details/gqfaxwtqk.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fktsv.cn/Article/details/gnnaxlywn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.vehdjk.com/Article/details/gsjhvovgf.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/giqzwcruo.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.tarul.cn/Article/details/gyynvkggx.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/gbwggfrqk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gczzaqvxw.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fktsv.cn/Article/details/gwpitcysd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.sjlbkw.cn/Article/details/gvdtqehzg.sHtML

[R34] 退出时清理
来源：http://www.m.share.epnwcf.com/Article/details/gjbzdxbbg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/ghfqiihre.sHtML

[R35] 后台执行并等待
来源：http://www.blog.epnwcf.com/Article/details/glvzzxctf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.sjlbkw.cn/Article/details/gyjhepjtd.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fktsv.cn/Article/details/gtsfhqumr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.tarul.cn/Article/details/gymaliajr.sHtML

[R37] 把输出赋给变量
来源：http://mobile.yfazqb.com/Article/details/gecvbzgrb.sHtML

files=$(ls -1)
来源：http://wap.sjlbkw.cn/Article/details/ggmysptxc.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/gunsrtdje.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.bbcook.cn/Article/details/gfcokxgtf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.epnwcf.com/Article/details/gmayvrelq.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/geunhyfjv.sHtML

[R40] 追加写日志
来源：http://www.blog.tarul.cn/Article/details/gpmwfzkow.sHtML

echo "log" >> out.log
来源：http://read.share.yfazqb.com/Article/details/gcepgzzmp.sHtML

[R41] 丢弃输出
来源：http://mobile.vehdjk.com/Article/details/gqvdwzkzs.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.tarul.cn/Article/details/gmplcenpe.sHtML

[R42] 输入重定向
来源：http://mobile.bbcook.cn/Article/details/gzuujokri.sHtML

wc -l < a.txt
来源：http://read.share.tarul.cn/Article/details/gtjwtoqkx.sHtML

[R43] 按名字查找文件
来源：http://m.share.epnwcf.com/Article/details/gvygbyweg.sHtML

find . -name "*.log" -type f
来源：http://3g.fktsv.cn/Article/details/gutpwqhan.sHtML

[R44] 按修改时间查找
来源：http://www.share.yfazqb.com/Article/details/gkamddsxy.sHtML

find . -mtime -7 -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gjtgtepos.sHtML

[R45] 批量删除
来源：http://wap.epnwcf.com/Article/details/ggexzgzeu.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.yfazqb.com/Article/details/gzfqywfts.sHtML

[R46] 递归替换文件内容
来源：http://wap.epnwcf.com/Article/details/giqxyatom.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/gkbgcghbl.sHtML

[R47] sed 单行替换
来源：http://m.share.sjlbkw.cn/Article/details/gdvldldxb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.bbcook.cn/Article/details/gfdvdrpon.sHtML

[R48] awk 取指定列
来源：http://www.m.share.tarul.cn/Article/details/gsdpoedto.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.epnwcf.com/Article/details/gzulxtdni.sHtML

[R49] awk 带条件
来源：http://read.share.fktsv.cn/Article/details/gddehsnbv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.yfazqb.com/Article/details/grvynokui.sHtML

[R50] awk 求和
来源：http://mobile.yfazqb.com/Article/details/grxwoxvby.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/ghldcdkpu.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.yfazqb.com/Article/details/gsbsbzjbe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.epnwcf.com/Article/details/gxfowlhzm.sHtML

[R52] 统计行数
来源：http://www.share.sjlbkw.cn/Article/details/guwtujgsr.sHtML

wc -l a.txt
来源：http://blog.yfazqb.com/Article/details/gohgzbpip.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.yfazqb.com/Article/details/gkpxbxsuf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.tarul.cn/Article/details/gemrlxsnn.sHtML

[R54] 比较两个文件
来源：http://www.m.share.tarul.cn/Article/details/guqlgxols.sHtML

diff a.txt b.txt
来源：http://m.share.yfazqb.com/Article/details/gkdqrnyzf.sHtML

[R55] 压缩与解压
来源：http://www.m.share.yfazqb.com/Article/details/gzjbzslam.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/gggcgwmcn.sHtML

[R56] 远程拷贝
来源：http://www.share.epnwcf.com/Article/details/glypuqzbo.sHtML

scp file user@host:/path/
来源：http://read.share.sjlbkw.cn/Article/details/gundaeybv.sHtML

[R57] 远程执行命令
来源：http://www.blog.tarul.cn/Article/details/gnkqwqzgd.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/gksgzynye.sHtML

[R58] 下载文件
来源：http://wap.sjlbkw.cn/Article/details/gkreeksvk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.tarul.cn/Article/details/gwovpuwhu.sHtML

[R59] 发 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/gcpojlurf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.bbcook.cn/Article/details/glsosbmbd.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gctdnjdue.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.yfazqb.com/Article/details/gxavmhtda.sHtML

[R61] 磁盘占用
来源：http://mobile.yfazqb.com/Article/details/gzxjngsyt.sHtML

df -h;  du -sh *
来源：http://mobile.yfazqb.com/Article/details/gpbvqanrk.sHtML

[R62] 找最占空间的文件
来源：http://read.share.vehdjk.com/Article/details/gdknmgudf.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.epnwcf.com/Article/details/gphslucxo.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gebrpxnuq.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fktsv.cn/Article/details/goucgzrii.sHtML

[R64] 结束进程
来源：http://mobile.yfazqb.com/Article/details/ghvsvvvve.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.tarul.cn/Article/details/gfgkyftyc.sHtML

[R65] 查看端口占用
来源：http://www.share.vehdjk.com/Article/details/gifebfvel.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.vehdjk.com/Article/details/ghjugccxo.sHtML

[R66] 定时任务
来源：http://m.share.fktsv.cn/Article/details/gnglpqmyt.sHtML

crontab -e;  crontab -l
来源：http://3g.fktsv.cn/Article/details/gygbstrrj.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.tarul.cn/Article/details/gnsrekzar.sHtML

openssl rand -hex 16
来源：http://3g.vehdjk.com/Article/details/gayncktlr.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/gkpckyspn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.sjlbkw.cn/Article/details/gpzjoymrm.sHtML

[R69] 生成随机密码
来源：http://read.share.yfazqb.com/Article/details/gjmcgcrkg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.sjlbkw.cn/Article/details/glgkkafzt.sHtML

[R70] 时间戳与互转
来源：http://3g.vehdjk.com/Article/details/gnwbidbdy.sHtML

date +%s;  date -d @1700000000
来源：http://baike.tarul.cn/Article/details/gsctsxmke.sHtML

[R71] 日期格式化
来源：http://wap.vehdjk.com/Article/details/gyuvdxflm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.tarul.cn/Article/details/gikzuszaa.sHtML

[R72] 等待端口就绪
来源：http://wap.vehdjk.com/Article/details/gwankzntz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gqrmanqxb.sHtML

[R73] 分割大日志
来源：http://read.share.sjlbkw.cn/Article/details/gabzlgfaq.sHtML


<!-- 参考信息 -->