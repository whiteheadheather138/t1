代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.epnwcf.com/Article/details/gqxvejmjb.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gwrdbeoax.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/ghjwsxgst.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.vehdjk.com/Article/details/gpxrhhnpd.sHtML

[Q33] 多列分组
来源：http://www.m.share.tarul.cn/Article/details/gvbgndedi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.bbcook.cn/Article/details/gitpesowz.sHtML

[Q34] 每组取第一条
来源：http://www.share.vehdjk.com/Article/details/gbjligbwv.sHtML

SELECT * FROM (
来源：http://read.share.fktsv.cn/Article/details/gwheqnhos.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.epnwcf.com/Article/details/gdylueqag.sHtML

) t WHERE rn = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gveykdixm.sHtML

[Q35] 内连接
来源：http://www.blog.tarul.cn/Article/details/gesvnexyw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/gsixwdlvp.sHtML

[Q36] 左连接
来源：http://3g.epnwcf.com/Article/details/glyxznngf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/glwrgspkb.sHtML

[Q37] 右连接
来源：http://wap.bbcook.cn/Article/details/guqpvotfb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.sjlbkw.cn/Article/details/gqitwaujy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.sjlbkw.cn/Article/details/gadcmmefg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.sjlbkw.cn/Article/details/grxwjrkcv.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.tarul.cn/Article/details/gzfpzskof.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.epnwcf.com/Article/details/gzsftqskn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.tarul.cn/Article/details/guhmeiegj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.vehdjk.com/Article/details/gynopxepa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.vehdjk.com/Article/details/gdgrvzdgb.sHtML

[Q41] 多表连接
来源：http://3g.sjlbkw.cn/Article/details/gjlhnniho.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/gcypvlmtj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.tarul.cn/Article/details/gyhblahpz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.yfazqb.com/Article/details/giioravwf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.tarul.cn/Article/details/gwsyrefpn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fktsv.cn/Article/details/ghdgqdiey.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.vehdjk.com/Article/details/gtawrunvt.sHtML

[Q43] 标量子查询
来源：http://www.blog.vehdjk.com/Article/details/gboablnis.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.yfazqb.com/Article/details/grohpmlby.sHtML

[Q44] IN 子查询
来源：http://wap.vehdjk.com/Article/details/gqrhnakbr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.sjlbkw.cn/Article/details/gcenlulaq.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.sjlbkw.cn/Article/details/ggvksgyum.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/gjltpymiv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.vehdjk.com/Article/details/gbldvyxwi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fktsv.cn/Article/details/glzujsmij.sHtML

[Q47] 与平均值比较
来源：http://www.share.tarul.cn/Article/details/gdmwdfcpe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.bbcook.cn/Article/details/gkvuiuhlh.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.epnwcf.com/Article/details/gtnvldbpi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.bbcook.cn/Article/details/gjkqfryca.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.vehdjk.com/Article/details/gpuqfsofi.sHtML

[Q49] 更新单行
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyasbyrt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.tarul.cn/Article/details/gysjwridi.sHtML

[Q50] 批量更新
来源：http://www.share.sjlbkw.cn/Article/details/ghyidauzp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.vehdjk.com/Article/details/gwmkwmhem.sHtML

[Q51] 用子查询更新
来源：http://wap.vehdjk.com/Article/details/gyhrfzhib.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.epnwcf.com/Article/details/gjevxqpqq.sHtML

[Q52] 删除指定行
来源：http://www.share.yfazqb.com/Article/details/gcidmnpdk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gqtgiufxl.sHtML

[Q53] 按条件删除
来源：http://www.blog.fktsv.cn/Article/details/guoepmtlg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.epnwcf.com/Article/details/gcghtrotl.sHtML

[Q54] 清空表
来源：http://wap.tarul.cn/Article/details/gskbrknlk.sHtML

TRUNCATE TABLE logs;
来源：http://baike.sjlbkw.cn/Article/details/gdbcdchno.sHtML

[Q55] 排名（并列占位）
来源：http://baike.vehdjk.com/Article/details/gnhvzrllw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fktsv.cn/Article/details/gsjlgwaaz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.epnwcf.com/Article/details/gcibadmma.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.bbcook.cn/Article/details/gdzrwdxjs.sHtML

[Q57] 行号
来源：http://www.m.share.vehdjk.com/Article/details/geslqovqh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gvunhxygx.sHtML

[Q58] 累计求和
来源：http://www.share.sjlbkw.cn/Article/details/gloyciedg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.epnwcf.com/Article/details/gcplbcezd.sHtML

[Q59] 分组内累计
来源：http://wap.fktsv.cn/Article/details/gvxacgrhv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/grsehqtto.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.epnwcf.com/Article/details/gsqrmebbu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.yfazqb.com/Article/details/gecnnjaqb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gcylughmi.sHtML

[Q61] 移动平均
来源：http://www.blog.fktsv.cn/Article/details/gdxznbuzw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.tarul.cn/Article/details/gqbzlqyht.sHtML

[Q62] 分组占比
来源：http://mobile.vehdjk.com/Article/details/gfvohqmdf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/gadbufrlx.sHtML

[Q63] 开启事务
来源：http://baike.sjlbkw.cn/Article/details/gnmxqvokw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fktsv.cn/Article/details/gwoqxrokn.sHtML

[Q64] 提交事务
来源：http://read.share.vehdjk.com/Article/details/gxuoqgnlk.sHtML

COMMIT;
来源：http://www.share.yfazqb.com/Article/details/gmiwyjmll.sHtML

[Q65] 回滚事务
来源：http://wap.epnwcf.com/Article/details/gbawtfhty.sHtML

ROLLBACK;
来源：http://blog.bbcook.cn/Article/details/gawnlzrkm.sHtML

[Q66] 行锁查询
来源：http://blog.epnwcf.com/Article/details/gkoumbuxk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fktsv.cn/Article/details/gbipptlie.sHtML

[Q67] 设置隔离级别
来源：http://3g.epnwcf.com/Article/details/glqwcdrox.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fktsv.cn/Article/details/gqghgaxqj.sHtML

[Q68] 保存点
来源：http://www.share.fktsv.cn/Article/details/gmnmvxbgq.sHtML

SAVEPOINT sp1;
来源：http://3g.vehdjk.com/Article/details/gduhunczm.sHtML

ROLLBACK TO sp1;
来源：http://blog.fktsv.cn/Article/details/gbayvtfwt.sHtML

[Q69] 查看执行计划
来源：http://www.share.sjlbkw.cn/Article/details/gtpaeywej.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/gqygkgsik.sHtML

[Q70] 更新统计信息
来源：http://m.share.vehdjk.com/Article/details/gpfquyhwy.sHtML

ANALYZE TABLE users;
来源：http://mobile.tarul.cn/Article/details/ghyifjxyy.sHtML

[Q71] 查看建表语句
来源：http://www.blog.tarul.cn/Article/details/genivmfdx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.bbcook.cn/Article/details/gqpthptfe.sHtML

[Q72] 查看索引
来源：http://3g.yfazqb.com/Article/details/gkcawlhkp.sHtML

SHOW INDEX FROM users;
来源：http://blog.vehdjk.com/Article/details/gwlqgpapn.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/gqjdddrys.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.vehdjk.com/Article/details/gkzedshjz.sHtML

[Q74] 强制使用索引
来源：http://www.blog.bbcook.cn/Article/details/gsnesvktq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.sjlbkw.cn/Article/details/gqaubmyij.sHtML

[Q75] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gesergokd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.yfazqb.com/Article/details/givaghcoe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/gkcxxvuvl.sHtML

[Q76] 按天统计
来源：http://blog.epnwcf.com/Article/details/gmbrbhypt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.sjlbkw.cn/Article/details/gscmbblxh.sHtML

[Q77] 时间加减
来源：http://read.share.fktsv.cn/Article/details/gnzblcsev.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.tarul.cn/Article/details/gqlzdpjsn.sHtML

[Q78] 当前时间
来源：http://wap.bbcook.cn/Article/details/geyhvltyj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.sjlbkw.cn/Article/details/gerdfcfgm.sHtML

[Q79] 字符串拼接
来源：http://read.share.bbcook.cn/Article/details/gmyerxawy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.vehdjk.com/Article/details/gysgwekcp.sHtML

[Q80] 字符串截取
来源：http://blog.epnwcf.com/Article/details/gyhzhsegm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gyrjydsjp.sHtML

[Q81] 字符串替换
来源：http://mobile.tarul.cn/Article/details/gjgbuzrfy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fktsv.cn/Article/details/giwofejva.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.epnwcf.com/Article/details/gfmqdtlbq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/ghjzbopaq.sHtML

[Q83] 大小写转换
来源：http://baike.fktsv.cn/Article/details/gdtovxrkn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gskkiafjn.sHtML

[Q84] 去除首尾空格
来源：http://3g.vehdjk.com/Article/details/gmhjhmszi.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gcpclwsal.sHtML

[Q85] 数值取整
来源：http://3g.tarul.cn/Article/details/gyxsqmydm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.vehdjk.com/Article/details/ghtjdvzyu.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.bbcook.cn/Article/details/gbtmsuihe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.sjlbkw.cn/Article/details/gwpnyyfiu.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.yfazqb.com/Article/details/giklbdidp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.bbcook.cn/Article/details/glainbjfu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.epnwcf.com/Article/details/gqlrbkech.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.sjlbkw.cn/Article/details/goeuetqdy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.bbcook.cn/Article/details/ggapxcdbq.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fktsv.cn/Article/details/ghdqpioge.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.bbcook.cn/Article/details/gfreshesq.sHtML

[Q90] 生成序号列
来源：http://www.m.share.sjlbkw.cn/Article/details/ghygzegpl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.sjlbkw.cn/Article/details/gdhjxwpps.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqfwljbpa.sHtML

R. Bash 专题
来源：http://wap.epnwcf.com/Article/details/gpghsramt.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gtzmdyrfm.sHtML

[R01] shebang 与严格模式
来源：http://wap.bbcook.cn/Article/details/glaeqegrf.sHtML

#!/usr/bin/env bash
来源：http://3g.tarul.cn/Article/details/ggjpiskhh.sHtML

set -euo pipefail
来源：http://mobile.epnwcf.com/Article/details/gqcnrjjuq.sHtML

[R02] 变量赋值与使用
来源：http://blog.yfazqb.com/Article/details/gvyftweij.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fktsv.cn/Article/details/gmfaiagay.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/gllekhjzo.sHtML

readonly PI=3.14
来源：http://wap.yfazqb.com/Article/details/guitzkvjn.sHtML

[R04] 位置参数
来源：http://www.m.share.epnwcf.com/Article/details/gkmrawlvi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.epnwcf.com/Article/details/gdphsoqws.sHtML

[R05] 参数默认值
来源：http://m.share.bbcook.cn/Article/details/grwejcyjq.sHtML

name="${1:-default}"
来源：http://baike.yfazqb.com/Article/details/gzqbbdgjg.sHtML

[R06] 判断命令是否存在
来源：http://m.share.yfazqb.com/Article/details/groqmemmg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/giwklazdf.sHtML

[R07] if 判断文件
来源：http://blog.fktsv.cn/Article/details/guyzzychw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.yfazqb.com/Article/details/gddyjpijx.sHtML

[R08] 数值比较
来源：http://mobile.tarul.cn/Article/details/gvkbocgri.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.yfazqb.com/Article/details/glpxjzeam.sHtML

[R09] 字符串比较
来源：http://3g.vehdjk.com/Article/details/gmcwpacej.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.yfazqb.com/Article/details/gomdsdxeu.sHtML

[R10] 正则匹配
来源：http://mobile.bbcook.cn/Article/details/glvirvbqk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.tarul.cn/Article/details/gytcteijd.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/gziwmxbhg.sHtML

case "$1" in
来源：http://www.m.share.sjlbkw.cn/Article/details/gntwbiajt.sHtML

start) echo "启动" ;;
来源：http://www.share.yfazqb.com/Article/details/gzvdplrss.sHtML

stop)  echo "停止" ;;
来源：http://read.share.bbcook.cn/Article/details/gkvxiytxk.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.yfazqb.com/Article/details/gzritypzz.sHtML

esac
来源：http://m.share.sjlbkw.cn/Article/details/gjcglulym.sHtML

[R12] for 遍历文件
来源：http://www.m.share.bbcook.cn/Article/details/gexnwygef.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fktsv.cn/Article/details/gnqcodcyv.sHtML

[R13] for 计数循环
来源：http://m.share.fktsv.cn/Article/details/gcdqbgyph.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gcnxawxwi.sHtML

[R14] C 风格 for
来源：http://www.blog.yfazqb.com/Article/details/gmzltopot.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gdltmhmhm.sHtML

[R15] while 逐行读文件
来源：http://blog.vehdjk.com/Article/details/gmkrhivgd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fktsv.cn/Article/details/gpumhmxtj.sHtML

[R16] until 等待条件
来源：http://www.blog.epnwcf.com/Article/details/gezcydebp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gldrjerht.sHtML

[R17] 数组定义与取值
来源：http://www.blog.sjlbkw.cn/Article/details/gqxlasawe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.vehdjk.com/Article/details/ggheyveyf.sHtML

[R18] 遍历数组
来源：http://baike.bbcook.cn/Article/details/givnsgere.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.bbcook.cn/Article/details/gvzmelfoj.sHtML

[R19] 数组长度
来源：http://blog.yfazqb.com/Article/details/gyrvmrdxp.sHtML

echo "${#arr[@]}"
来源：http://3g.yfazqb.com/Article/details/gfgjmxuma.sHtML

[R20] 关联数组（字典）
来源：http://m.share.bbcook.cn/Article/details/gfwglqaix.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.epnwcf.com/Article/details/gvdozldfl.sHtML

[R21] 字符串长度
来源：http://read.share.epnwcf.com/Article/details/gcmfenvbl.sHtML

echo "${#s}"
来源：http://www.blog.tarul.cn/Article/details/gcmoikxgo.sHtML

[R22] 截取子串
来源：http://m.share.sjlbkw.cn/Article/details/ghefnblqv.sHtML

echo "${s:0:5}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gwolqgvlq.sHtML

[R23] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gbppbsecx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.sjlbkw.cn/Article/details/gzgehgdut.sHtML

[R24] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gyvinumdv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.epnwcf.com/Article/details/gdhdhoiqk.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.sjlbkw.cn/Article/details/glxuscofb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.vehdjk.com/Article/details/gnhdtqnuh.sHtML

[R26] 命令替换
来源：http://www.blog.yfazqb.com/Article/details/gndceurxr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.epnwcf.com/Article/details/gflxgnawn.sHtML

[R27] 算术展开
来源：http://wap.vehdjk.com/Article/details/gmdubgkpk.sHtML

echo $((1 + 2 * 3))
来源：http://wap.bbcook.cn/Article/details/gnituqpyx.sHtML

[R28] 浮点运算
来源：http://mobile.epnwcf.com/Article/details/gmmgcdatv.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.epnwcf.com/Article/details/gmjfmhrkp.sHtML

[R29] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/gkuxupozi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fktsv.cn/Article/details/gfplmqqyw.sHtML

[R30] 函数返回状态码
来源：http://m.share.sjlbkw.cn/Article/details/gvdumbemk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fktsv.cn/Article/details/gwdcqfhbr.sHtML

[R31] 局部变量
来源：http://read.share.bbcook.cn/Article/details/glowockce.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.sjlbkw.cn/Article/details/gxumltsjr.sHtML

[R32] 参数个数校验
来源：http://mobile.bbcook.cn/Article/details/gesqgyteq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.vehdjk.com/Article/details/gocntibsv.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.yfazqb.com/Article/details/gihkwzkyt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.bbcook.cn/Article/details/goevcmakf.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/giihtjhrb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/gxhatdhjg.sHtML

[R35] 后台执行并等待
来源：http://3g.sjlbkw.cn/Article/details/gwuhmabue.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/ggauhsiyz.sHtML

[R36] 并发执行多个任务
来源：http://3g.tarul.cn/Article/details/ghaywnmgk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.vehdjk.com/Article/details/gqhgnphrd.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.vehdjk.com/Article/details/gmzkghvrq.sHtML

files=$(ls -1)
来源：http://www.share.epnwcf.com/Article/details/gexjsqerv.sHtML

[R38] 管道串联
来源：http://www.m.share.yfazqb.com/Article/details/gszhonpsy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.vehdjk.com/Article/details/gzsywvman.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.yfazqb.com/Article/details/gwxwkxuav.sHtML

cmd > out.log 2>&1
来源：http://baike.fktsv.cn/Article/details/gttluvtbi.sHtML

[R40] 追加写日志
来源：http://wap.bbcook.cn/Article/details/gsgeknnwz.sHtML

echo "log" >> out.log
来源：http://mobile.tarul.cn/Article/details/gfhfkvsta.sHtML

[R41] 丢弃输出
来源：http://blog.epnwcf.com/Article/details/gfpvymgap.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fktsv.cn/Article/details/gjwfmkoee.sHtML

[R42] 输入重定向
来源：http://www.m.share.tarul.cn/Article/details/gykpawruq.sHtML

wc -l < a.txt
来源：http://mobile.tarul.cn/Article/details/gdijcspar.sHtML

[R43] 按名字查找文件
来源：http://www.blog.yfazqb.com/Article/details/gvdeljvab.sHtML

find . -name "*.log" -type f
来源：http://3g.sjlbkw.cn/Article/details/gvmruyxmk.sHtML

[R44] 按修改时间查找
来源：http://read.share.fktsv.cn/Article/details/gnpqyjlzm.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fktsv.cn/Article/details/gdkytpkjz.sHtML

[R45] 批量删除
来源：http://wap.fktsv.cn/Article/details/gcwfzxvge.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gfsdbpoqo.sHtML

[R46] 递归替换文件内容
来源：http://read.share.tarul.cn/Article/details/gbkqhbqgs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.vehdjk.com/Article/details/gkozcrvkv.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/gqrmgpnbf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.epnwcf.com/Article/details/gqwqtbkym.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fktsv.cn/Article/details/gvfztkwuu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gtmxxyndc.sHtML

[R49] awk 带条件
来源：http://m.share.yfazqb.com/Article/details/gblgnkwfq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fktsv.cn/Article/details/gtpyurjgy.sHtML

[R50] awk 求和
来源：http://www.blog.tarul.cn/Article/details/gjifacbjs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gjyhrpfbg.sHtML

[R51] 排序去重取前几
来源：http://www.share.sjlbkw.cn/Article/details/geqhvgqby.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.tarul.cn/Article/details/ggbfectop.sHtML

[R52] 统计行数
来源：http://www.m.share.sjlbkw.cn/Article/details/gvddwqhkx.sHtML

wc -l a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gkugrsseu.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.yfazqb.com/Article/details/gjkowtfbs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.epnwcf.com/Article/details/gtkdxuegx.sHtML

[R54] 比较两个文件
来源：http://www.share.tarul.cn/Article/details/gttlykapq.sHtML

diff a.txt b.txt
来源：http://3g.sjlbkw.cn/Article/details/gvyrtmauw.sHtML

[R55] 压缩与解压
来源：http://3g.tarul.cn/Article/details/gqdzdhdov.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gwwmljodl.sHtML

[R56] 远程拷贝
来源：http://3g.tarul.cn/Article/details/ggondvbnb.sHtML

scp file user@host:/path/
来源：http://blog.tarul.cn/Article/details/gpiqaqzjz.sHtML

[R57] 远程执行命令
来源：http://wap.fktsv.cn/Article/details/gdqprrkek.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.yfazqb.com/Article/details/gxmyjjuty.sHtML

[R58] 下载文件
来源：http://www.blog.bbcook.cn/Article/details/gdpkkohmz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.vehdjk.com/Article/details/gpwvpkrwy.sHtML

[R59] 发 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gsdgzpncw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.tarul.cn/Article/details/gntsxmrhc.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gwjcbtsjr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.tarul.cn/Article/details/ghvrlpmsd.sHtML

[R61] 磁盘占用
来源：http://3g.epnwcf.com/Article/details/ghjadytqa.sHtML

df -h;  du -sh *
来源：http://www.share.epnwcf.com/Article/details/gcntkwigk.sHtML

[R62] 找最占空间的文件
来源：http://m.share.bbcook.cn/Article/details/gfxcpkyhr.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.yfazqb.com/Article/details/gqkzymiph.sHtML

[R63] 内存与进程
来源：http://baike.bbcook.cn/Article/details/glurjoewm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/ghcyflmxy.sHtML

[R64] 结束进程
来源：http://blog.sjlbkw.cn/Article/details/gokoqikkk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.tarul.cn/Article/details/gxjbtnats.sHtML

[R65] 查看端口占用
来源：http://blog.yfazqb.com/Article/details/gogypltxc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvuesady.sHtML

[R66] 定时任务
来源：http://www.blog.tarul.cn/Article/details/gnesovyle.sHtML

crontab -e;  crontab -l
来源：http://www.share.bbcook.cn/Article/details/giwzekihd.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.bbcook.cn/Article/details/grwpbhhwz.sHtML

openssl rand -hex 16
来源：http://m.share.bbcook.cn/Article/details/gspkfnuqg.sHtML

[R68] 计算文件校验值
来源：http://m.share.vehdjk.com/Article/details/ghgsxrwga.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.tarul.cn/Article/details/gtpglyjxr.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/gvbtovpuz.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.yfazqb.com/Article/details/gkenzhwek.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.vehdjk.com/Article/details/guzfevmad.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fktsv.cn/Article/details/gnbsjghqu.sHtML

[R71] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gglvejlvx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.tarul.cn/Article/details/gfqlwrafb.sHtML

[R72] 等待端口就绪
来源：http://www.share.epnwcf.com/Article/details/gtuhnebrn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/ggksqoamg.sHtML

[R73] 分割大日志
来源：http://wap.yfazqb.com/Article/details/gadycdchn.sHtML

split -l 1000 big.log part_
来源：http://blog.fktsv.cn/Article/details/gogedufme.sHtML

[R74] 批量重命名
来源：http://read.share.yfazqb.com/Article/details/gqhjdpgbz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.sjlbkw.cn/Article/details/gfnsxgtya.sHtML

[R75] 导出环境变量
来源：http://m.share.bbcook.cn/Article/details/gdecftixk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/gccgqywrf.sHtML

[R76] 使用临时文件
来源：http://read.share.sjlbkw.cn/Article/details/gwpuxqyrh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.bbcook.cn/Article/details/gsxdpruid.sHtML

[R77] 读取用户输入
来源：http://www.m.share.yfazqb.com/Article/details/gnahpwjou.sHtML

read -rp "请输入: " ans
来源：http://baike.bbcook.cn/Article/details/glxjtucyc.sHtML

[R78] 交互式菜单
来源：http://wap.tarul.cn/Article/details/gcrrkieuk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.epnwcf.com/Article/details/gzuuztxel.sHtML

[R79] 解析命令行选项
来源：http://mobile.vehdjk.com/Article/details/ggzzesvoy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.epnwcf.com/Article/details/gdqnyakzt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.tarul.cn/Article/details/girbkvqfz.sHtML

time ./run.sh
来源：http://www.share.sjlbkw.cn/Article/details/gxyrdbzxw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/guwebqgca.sHtML


<!-- 参考信息 -->