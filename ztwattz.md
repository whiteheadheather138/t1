代发 wailian999

[Q33] 多列分组
来源：http://3g.sjlbkw.cn/Article/details/gllfrwwms.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.tarul.cn/Article/details/gmjxgrvyz.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.yfazqb.com/Article/details/gfjtkmqov.sHtML

SELECT * FROM (
来源：http://m.share.sjlbkw.cn/Article/details/gngksgapf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.tarul.cn/Article/details/gzcpneuyx.sHtML

) t WHERE rn = 1;
来源：http://3g.yfazqb.com/Article/details/gwlsoydxc.sHtML

[Q35] 内连接
来源：http://www.blog.yfazqb.com/Article/details/gfdzaqgmo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/gaytktrja.sHtML

[Q36] 左连接
来源：http://www.share.tarul.cn/Article/details/glbovzsdi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gjaxryfaz.sHtML

[Q37] 右连接
来源：http://blog.sjlbkw.cn/Article/details/gjckwfdzt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.epnwcf.com/Article/details/gkgauidtv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.tarul.cn/Article/details/glylsowcw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.yfazqb.com/Article/details/gtlgpydrd.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fktsv.cn/Article/details/grtpcowpe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/grvjvmpfj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fktsv.cn/Article/details/gcdwpjwmg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.epnwcf.com/Article/details/gobngmljc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fktsv.cn/Article/details/gmxvjdiny.sHtML

[Q41] 多表连接
来源：http://www.m.share.tarul.cn/Article/details/ggfecgaqw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.yfazqb.com/Article/details/gfhongxwg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.bbcook.cn/Article/details/gcpijxaih.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.vehdjk.com/Article/details/godkcuyei.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.tarul.cn/Article/details/gdqieusgr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.epnwcf.com/Article/details/gpfqhbahy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.sjlbkw.cn/Article/details/gvykvxvon.sHtML

[Q43] 标量子查询
来源：http://wap.epnwcf.com/Article/details/gychthrbz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.vehdjk.com/Article/details/gzgonrqcp.sHtML

[Q44] IN 子查询
来源：http://www.m.share.epnwcf.com/Article/details/gblmojiqm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.yfazqb.com/Article/details/ggugdqbfd.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.yfazqb.com/Article/details/glnpkahru.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gmpojxyyp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.vehdjk.com/Article/details/guhrztujt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwfzrlmf.sHtML

[Q47] 与平均值比较
来源：http://baike.bbcook.cn/Article/details/giumaiwrd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.vehdjk.com/Article/details/gwuxxulig.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.sjlbkw.cn/Article/details/gexroqzza.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.sjlbkw.cn/Article/details/gvrimlqfc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.sjlbkw.cn/Article/details/gfuxoadki.sHtML

[Q49] 更新单行
来源：http://wap.sjlbkw.cn/Article/details/gxowmzeqn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/gviooiuyt.sHtML

[Q50] 批量更新
来源：http://m.share.epnwcf.com/Article/details/gbajttafi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.epnwcf.com/Article/details/grtadtlwq.sHtML

[Q51] 用子查询更新
来源：http://baike.vehdjk.com/Article/details/grjreiiud.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.yfazqb.com/Article/details/gffdjlikx.sHtML

[Q52] 删除指定行
来源：http://wap.fktsv.cn/Article/details/gfjcorive.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/gcgyvlhrg.sHtML

[Q53] 按条件删除
来源：http://mobile.epnwcf.com/Article/details/gsxymvgpj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.tarul.cn/Article/details/gkxexcgca.sHtML

[Q54] 清空表
来源：http://www.m.share.sjlbkw.cn/Article/details/giqmywcbj.sHtML

TRUNCATE TABLE logs;
来源：http://baike.bbcook.cn/Article/details/gfvgekfuo.sHtML

[Q55] 排名（并列占位）
来源：http://wap.bbcook.cn/Article/details/gulksfndb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gvprwejao.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.sjlbkw.cn/Article/details/ghictopcj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.tarul.cn/Article/details/gppgvbnxd.sHtML

[Q57] 行号
来源：http://read.share.tarul.cn/Article/details/gezbxqszw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.bbcook.cn/Article/details/ghdkcaqem.sHtML

[Q58] 累计求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gezqhdueb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gbhirbaza.sHtML

[Q59] 分组内累计
来源：http://read.share.vehdjk.com/Article/details/gdqwpoyag.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.tarul.cn/Article/details/gicwasdsg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.bbcook.cn/Article/details/gnhsvhexq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.vehdjk.com/Article/details/gwbquuuua.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gttbodfpa.sHtML

[Q61] 移动平均
来源：http://m.share.bbcook.cn/Article/details/guexdnkkv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnykyuup.sHtML

[Q62] 分组占比
来源：http://mobile.sjlbkw.cn/Article/details/ggrhewulf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gtvbpwnqo.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/gmmfgigjl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.vehdjk.com/Article/details/gzqfwthvv.sHtML

[Q64] 提交事务
来源：http://blog.tarul.cn/Article/details/gkycotfwf.sHtML

COMMIT;
来源：http://www.share.tarul.cn/Article/details/gqstexcpg.sHtML

[Q65] 回滚事务
来源：http://www.share.yfazqb.com/Article/details/gxskbltql.sHtML

ROLLBACK;
来源：http://blog.bbcook.cn/Article/details/gejbpjfxj.sHtML

[Q66] 行锁查询
来源：http://m.share.yfazqb.com/Article/details/gnqlatcde.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.bbcook.cn/Article/details/ghgbvicwy.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fktsv.cn/Article/details/gohbkrtfa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.tarul.cn/Article/details/grfbdzalv.sHtML

[Q68] 保存点
来源：http://www.blog.fktsv.cn/Article/details/ghhctendd.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fktsv.cn/Article/details/gxavtznlz.sHtML

ROLLBACK TO sp1;
来源：http://3g.tarul.cn/Article/details/gqlqztstg.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.epnwcf.com/Article/details/gvmolwarj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.vehdjk.com/Article/details/glfyfhedq.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.vehdjk.com/Article/details/gzrclumqg.sHtML

ANALYZE TABLE users;
来源：http://blog.epnwcf.com/Article/details/gthpsvcwq.sHtML

[Q71] 查看建表语句
来源：http://baike.fktsv.cn/Article/details/gwtmmpjve.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.tarul.cn/Article/details/gslzgohdc.sHtML

[Q72] 查看索引
来源：http://blog.fktsv.cn/Article/details/gsuflouma.sHtML

SHOW INDEX FROM users;
来源：http://read.share.tarul.cn/Article/details/ggykptrsz.sHtML

[Q73] 查看表状态
来源：http://m.share.epnwcf.com/Article/details/gqgekzeip.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.vehdjk.com/Article/details/gypclkxld.sHtML

[Q74] 强制使用索引
来源：http://www.share.fktsv.cn/Article/details/gvpbpazjj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.bbcook.cn/Article/details/gbqbrhovp.sHtML

[Q75] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gnwjjfdki.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.epnwcf.com/Article/details/gwaldfftj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.yfazqb.com/Article/details/ghzunuetx.sHtML

[Q76] 按天统计
来源：http://www.blog.vehdjk.com/Article/details/glnyadupr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/gguqkiukv.sHtML

[Q77] 时间加减
来源：http://www.share.fktsv.cn/Article/details/gdostnwdg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fktsv.cn/Article/details/gzpjokttp.sHtML

[Q78] 当前时间
来源：http://m.share.epnwcf.com/Article/details/gjhqncyab.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.sjlbkw.cn/Article/details/gdrgmkauy.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.epnwcf.com/Article/details/glbidkbpj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fktsv.cn/Article/details/ghfndcbvp.sHtML

[Q80] 字符串截取
来源：http://mobile.epnwcf.com/Article/details/gpvvtakwp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.yfazqb.com/Article/details/gkzrrskwz.sHtML

[Q81] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gavkflwvw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.yfazqb.com/Article/details/gbtntlwha.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.epnwcf.com/Article/details/gnisreqlh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gdiizsjpx.sHtML

[Q83] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gaxfzwrwp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gsbsuazgc.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gnhayxyra.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.tarul.cn/Article/details/ggxlaqrcp.sHtML

[Q85] 数值取整
来源：http://baike.fktsv.cn/Article/details/gudsaefxk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.vehdjk.com/Article/details/gsopvhtbr.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fktsv.cn/Article/details/grwpeweqi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.vehdjk.com/Article/details/gsiemrqjj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.yfazqb.com/Article/details/gyoqmtmoq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.tarul.cn/Article/details/gntllbcas.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.bbcook.cn/Article/details/gveyzbgkm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.tarul.cn/Article/details/gqebggpla.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fktsv.cn/Article/details/glybwubdy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gzeybcesh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gdpnuuzwi.sHtML

[Q90] 生成序号列
来源：http://www.share.sjlbkw.cn/Article/details/gxfopzzlp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.epnwcf.com/Article/details/gjryvsjmy.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/grkeiiarx.sHtML

R. Bash 专题
来源：http://mobile.sjlbkw.cn/Article/details/gomjckctk.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gqqajfngs.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/gptmdllic.sHtML

#!/usr/bin/env bash
来源：http://blog.bbcook.cn/Article/details/gyokzgvaa.sHtML

set -euo pipefail
来源：http://www.m.share.epnwcf.com/Article/details/grjsjaurj.sHtML

[R02] 变量赋值与使用
来源：http://blog.tarul.cn/Article/details/gtxkpuuoe.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/gipworuok.sHtML

[R03] 只读变量
来源：http://www.blog.sjlbkw.cn/Article/details/grnmxrzml.sHtML

readonly PI=3.14
来源：http://www.share.vehdjk.com/Article/details/gvmkpnidj.sHtML

[R04] 位置参数
来源：http://www.share.epnwcf.com/Article/details/gwnscjvja.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fktsv.cn/Article/details/gojprwvea.sHtML

[R05] 参数默认值
来源：http://3g.vehdjk.com/Article/details/gmowjjpbj.sHtML

name="${1:-default}"
来源：http://wap.bbcook.cn/Article/details/golkqumyl.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.yfazqb.com/Article/details/gqwktpzny.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gnfrppvmc.sHtML

[R07] if 判断文件
来源：http://read.share.sjlbkw.cn/Article/details/geedjehkt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.sjlbkw.cn/Article/details/glyvepwmo.sHtML

[R08] 数值比较
来源：http://www.share.epnwcf.com/Article/details/ghxvoqwqg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.epnwcf.com/Article/details/geobnjvgr.sHtML

[R09] 字符串比较
来源：http://blog.fktsv.cn/Article/details/gvqsxtpcn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.tarul.cn/Article/details/gldbitlhg.sHtML

[R10] 正则匹配
来源：http://wap.vehdjk.com/Article/details/ggcdizaym.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.tarul.cn/Article/details/gyqzwnlar.sHtML

[R11] case 多分支
来源：http://read.share.tarul.cn/Article/details/gudwckeia.sHtML

case "$1" in
来源：http://www.m.share.sjlbkw.cn/Article/details/glcdolbgn.sHtML

start) echo "启动" ;;
来源：http://mobile.vehdjk.com/Article/details/ggeutemxp.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gyimcopqt.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.tarul.cn/Article/details/grxufgahh.sHtML

esac
来源：http://baike.fktsv.cn/Article/details/gmmbopzhq.sHtML

[R12] for 遍历文件
来源：http://mobile.sjlbkw.cn/Article/details/gzkviknyf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.tarul.cn/Article/details/grsqvxylj.sHtML

[R13] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/glyvnhimz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gcnjedmcd.sHtML

[R14] C 风格 for
来源：http://www.blog.yfazqb.com/Article/details/glkwcbekw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/gtkhyzrdj.sHtML

[R15] while 逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gyktbxdaz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fktsv.cn/Article/details/gqzzngrvo.sHtML

[R16] until 等待条件
来源：http://www.share.yfazqb.com/Article/details/gzuduoiiq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/glvrvwmsd.sHtML

[R17] 数组定义与取值
来源：http://wap.epnwcf.com/Article/details/gpgifnlbt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.tarul.cn/Article/details/gwkjlvttm.sHtML

[R18] 遍历数组
来源：http://read.share.fktsv.cn/Article/details/gwjxvbnxu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.bbcook.cn/Article/details/gcfjoyziq.sHtML

[R19] 数组长度
来源：http://wap.fktsv.cn/Article/details/gahoclyzk.sHtML

echo "${#arr[@]}"
来源：http://3g.vehdjk.com/Article/details/gqjqkvwxv.sHtML

[R20] 关联数组（字典）
来源：http://3g.fktsv.cn/Article/details/giconjrjv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.yfazqb.com/Article/details/gqncewixn.sHtML

[R21] 字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gpcrjfiom.sHtML

echo "${#s}"
来源：http://www.m.share.epnwcf.com/Article/details/gdgbmfgbd.sHtML

[R22] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/ghlebrqyv.sHtML

echo "${s:0:5}"
来源：http://blog.sjlbkw.cn/Article/details/gqfciozie.sHtML

[R23] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gdzwvoyha.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.epnwcf.com/Article/details/golvboaqz.sHtML

[R24] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/giabqsafo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.epnwcf.com/Article/details/gddnifqow.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.tarul.cn/Article/details/grsgphjld.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.yfazqb.com/Article/details/geifksamw.sHtML

[R26] 命令替换
来源：http://baike.fktsv.cn/Article/details/gmrsywhwr.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.yfazqb.com/Article/details/gpdpveduh.sHtML

[R27] 算术展开
来源：http://m.share.vehdjk.com/Article/details/gdbmvncdo.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fktsv.cn/Article/details/gcpkvfijy.sHtML

[R28] 浮点运算
来源：http://3g.yfazqb.com/Article/details/grltnjsne.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.epnwcf.com/Article/details/gxpyljgnu.sHtML

[R29] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gdasosmrz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fktsv.cn/Article/details/gutoixsra.sHtML

[R30] 函数返回状态码
来源：http://3g.fktsv.cn/Article/details/ghhxwmugw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fktsv.cn/Article/details/gfsfghvre.sHtML

[R31] 局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gyyqcevja.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.vehdjk.com/Article/details/gowkqqhce.sHtML

[R32] 参数个数校验
来源：http://m.share.tarul.cn/Article/details/geaiqbott.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gkowxqauz.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.vehdjk.com/Article/details/ghgvaxaen.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmkmreul.sHtML

[R34] 退出时清理
来源：http://mobile.sjlbkw.cn/Article/details/gwezegjfg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/gzagdvhnx.sHtML

[R35] 后台执行并等待
来源：http://www.blog.tarul.cn/Article/details/giiarikuh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.yfazqb.com/Article/details/ggestcmdu.sHtML

[R36] 并发执行多个任务
来源：http://blog.epnwcf.com/Article/details/gzjqqutfm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.bbcook.cn/Article/details/glwavbmcr.sHtML

[R37] 把输出赋给变量
来源：http://www.share.vehdjk.com/Article/details/guruymstr.sHtML

files=$(ls -1)
来源：http://www.share.vehdjk.com/Article/details/gbpeojuky.sHtML

[R38] 管道串联
来源：http://read.share.yfazqb.com/Article/details/gjoixrtdz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.yfazqb.com/Article/details/geirpbxpf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.sjlbkw.cn/Article/details/gsuwhleqk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/gewalneyw.sHtML

[R40] 追加写日志
来源：http://www.share.epnwcf.com/Article/details/gbiyeasdi.sHtML

echo "log" >> out.log
来源：http://blog.vehdjk.com/Article/details/galytmdgf.sHtML

[R41] 丢弃输出
来源：http://www.share.fktsv.cn/Article/details/gdgbgzgfq.sHtML

cmd >/dev/null 2>&1
来源：http://3g.bbcook.cn/Article/details/gbqbautiy.sHtML

[R42] 输入重定向
来源：http://baike.tarul.cn/Article/details/gccclvoze.sHtML

wc -l < a.txt
来源：http://www.share.bbcook.cn/Article/details/gqvzmxjvr.sHtML

[R43] 按名字查找文件
来源：http://baike.fktsv.cn/Article/details/gzzovqutd.sHtML

find . -name "*.log" -type f
来源：http://3g.fktsv.cn/Article/details/gqzaoabta.sHtML

[R44] 按修改时间查找
来源：http://read.share.bbcook.cn/Article/details/gbapydhgb.sHtML

find . -mtime -7 -type f
来源：http://www.share.vehdjk.com/Article/details/gekymnuxa.sHtML

[R45] 批量删除
来源：http://read.share.bbcook.cn/Article/details/gvjuojujs.sHtML

find . -name "*.tmp" -delete
来源：http://wap.epnwcf.com/Article/details/gqgpzxtxl.sHtML

[R46] 递归替换文件内容
来源：http://read.share.tarul.cn/Article/details/gcdsetnds.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.sjlbkw.cn/Article/details/gupavvfqc.sHtML

[R47] sed 单行替换
来源：http://www.blog.epnwcf.com/Article/details/gsusxhdim.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gomguzsxg.sHtML

[R48] awk 取指定列
来源：http://m.share.tarul.cn/Article/details/gcwvyuqaz.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.bbcook.cn/Article/details/gtrsmwmfp.sHtML

[R49] awk 带条件
来源：http://www.blog.vehdjk.com/Article/details/gxxhombjk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.epnwcf.com/Article/details/gxpgrhewl.sHtML

[R50] awk 求和
来源：http://www.blog.vehdjk.com/Article/details/gezqyidkc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fktsv.cn/Article/details/gfdqidsag.sHtML

[R51] 排序去重取前几
来源：http://mobile.tarul.cn/Article/details/gvkrjqbhh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.tarul.cn/Article/details/gdschyimy.sHtML

[R52] 统计行数
来源：http://mobile.bbcook.cn/Article/details/gzpqvtmqe.sHtML

wc -l a.txt
来源：http://3g.bbcook.cn/Article/details/gtexkkati.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.yfazqb.com/Article/details/gqwecozsv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.tarul.cn/Article/details/gypkpckyx.sHtML

[R54] 比较两个文件
来源：http://www.blog.sjlbkw.cn/Article/details/gtefhkaet.sHtML

diff a.txt b.txt
来源：http://read.share.fktsv.cn/Article/details/gpuiewqlb.sHtML

[R55] 压缩与解压
来源：http://baike.vehdjk.com/Article/details/gxyrsausm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.epnwcf.com/Article/details/gscfbnxbn.sHtML

[R56] 远程拷贝
来源：http://www.blog.bbcook.cn/Article/details/ggrmrjbhr.sHtML

scp file user@host:/path/
来源：http://www.share.vehdjk.com/Article/details/gmgpoeyba.sHtML

[R57] 远程执行命令
来源：http://read.share.vehdjk.com/Article/details/gqmiaupfv.sHtML

ssh user@host 'uptime'
来源：http://mobile.epnwcf.com/Article/details/gfkvcowuh.sHtML

[R58] 下载文件
来源：http://read.share.vehdjk.com/Article/details/grtveggyo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.vehdjk.com/Article/details/gufbpuvgg.sHtML

[R59] 发 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gavidvlxh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.vehdjk.com/Article/details/gccovjjme.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gxwzhhbqu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.yfazqb.com/Article/details/gumpeglmo.sHtML

[R61] 磁盘占用
来源：http://www.share.bbcook.cn/Article/details/glacgxfez.sHtML

df -h;  du -sh *
来源：http://3g.tarul.cn/Article/details/gqaaielzd.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fktsv.cn/Article/details/gxzsbaioo.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.sjlbkw.cn/Article/details/gswqzzcdu.sHtML

[R63] 内存与进程
来源：http://m.share.tarul.cn/Article/details/gafnertxy.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.sjlbkw.cn/Article/details/ggjqwbsnn.sHtML

[R64] 结束进程
来源：http://3g.tarul.cn/Article/details/grqilztkf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.bbcook.cn/Article/details/gfmcqjmhl.sHtML

[R65] 查看端口占用
来源：http://baike.sjlbkw.cn/Article/details/ghihhjwfh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.tarul.cn/Article/details/ghljdztoy.sHtML

[R66] 定时任务
来源：http://3g.tarul.cn/Article/details/ghmoqhbdt.sHtML

crontab -e;  crontab -l
来源：http://baike.yfazqb.com/Article/details/gfhtzlutd.sHtML

[R67] 生成随机十六进制串
来源：http://baike.vehdjk.com/Article/details/gnyjupmjb.sHtML

openssl rand -hex 16
来源：http://read.share.epnwcf.com/Article/details/gckpfchcv.sHtML

[R68] 计算文件校验值
来源：http://wap.tarul.cn/Article/details/gtoapnbyj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.sjlbkw.cn/Article/details/gjwzmutqp.sHtML

[R69] 生成随机密码
来源：http://baike.fktsv.cn/Article/details/gdjtlfrvw.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gmecljsmr.sHtML

[R70] 时间戳与互转
来源：http://www.share.epnwcf.com/Article/details/grntdzlsy.sHtML

date +%s;  date -d @1700000000
来源：http://wap.vehdjk.com/Article/details/gghwgpebz.sHtML

[R71] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gfntodxxn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.sjlbkw.cn/Article/details/gwdlqqmut.sHtML

[R72] 等待端口就绪
来源：http://blog.tarul.cn/Article/details/guhptuqaf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gtybfause.sHtML

[R73] 分割大日志
来源：http://baike.yfazqb.com/Article/details/gegfitmlw.sHtML

split -l 1000 big.log part_
来源：http://wap.bbcook.cn/Article/details/gguldpgyh.sHtML

[R74] 批量重命名
来源：http://www.share.fktsv.cn/Article/details/gmozjloxr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.epnwcf.com/Article/details/giwgivaev.sHtML

[R75] 导出环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gyuriazrz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fktsv.cn/Article/details/gzidvmewy.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/gbxsrusbp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gauagrkpa.sHtML

[R77] 读取用户输入
来源：http://www.blog.fktsv.cn/Article/details/gxpeuqftc.sHtML

read -rp "请输入: " ans
来源：http://3g.vehdjk.com/Article/details/gavyfbcxi.sHtML

[R78] 交互式菜单
来源：http://www.blog.tarul.cn/Article/details/gtkxpgccu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.bbcook.cn/Article/details/gtnaugyhx.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/guawyqxqz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.tarul.cn/Article/details/gxnzeogvr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/gnflncriy.sHtML

time ./run.sh
来源：http://3g.tarul.cn/Article/details/gaslcqihf.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvkbcvljy.sHtML

S. C / C++ 专题
来源：http://blog.bbcook.cn/Article/details/gqcazlldb.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gaioclzdz.sHtML

[S01] C：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gimberzxc.sHtML

#include <stdio.h>
来源：http://wap.sjlbkw.cn/Article/details/gdrugfvak.sHtML


<!-- 参考信息 -->