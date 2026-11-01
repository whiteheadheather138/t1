代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.tarul.cn/Article/details/gpkxrnslf.sHtML

[Q30] 分组统计
来源：http://3g.vehdjk.com/Article/details/gudxviwvy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gvkwisuxu.sHtML

[Q31] 分组后过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gdtqlaamv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gigdrzuzq.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/gzlaumcjb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gqccajnyd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.epnwcf.com/Article/details/goxafvytc.sHtML

[Q33] 多列分组
来源：http://blog.bbcook.cn/Article/details/gotujocof.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.yfazqb.com/Article/details/govzpgrvh.sHtML

[Q34] 每组取第一条
来源：http://read.share.yfazqb.com/Article/details/grhqdcglj.sHtML

SELECT * FROM (
来源：http://baike.sjlbkw.cn/Article/details/gkjoqnglt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.bbcook.cn/Article/details/gnfplcjrk.sHtML

) t WHERE rn = 1;
来源：http://www.share.vehdjk.com/Article/details/gsyhxqzhs.sHtML

[Q35] 内连接
来源：http://baike.fktsv.cn/Article/details/gokgcvexm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/ggzzyxlwd.sHtML

[Q36] 左连接
来源：http://blog.fktsv.cn/Article/details/gqihkllpw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/gzvggnsjk.sHtML

[Q37] 右连接
来源：http://baike.tarul.cn/Article/details/gmlqpwvtu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.yfazqb.com/Article/details/grovqdjve.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.sjlbkw.cn/Article/details/gvnmmlzsg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.sjlbkw.cn/Article/details/ggtrpyeou.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.vehdjk.com/Article/details/gwbkqamuh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.bbcook.cn/Article/details/gxlrbfpha.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fktsv.cn/Article/details/gbluypvdk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.tarul.cn/Article/details/gsvvklpwi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.yfazqb.com/Article/details/gsxfgryro.sHtML

[Q41] 多表连接
来源：http://www.m.share.vehdjk.com/Article/details/gqtozcdpa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fktsv.cn/Article/details/gkfnwxezq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.bbcook.cn/Article/details/gqoaqusij.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.tarul.cn/Article/details/guzhpvoiq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.vehdjk.com/Article/details/glfaffijl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.yfazqb.com/Article/details/grgnnzmhz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.epnwcf.com/Article/details/gsewpzhdr.sHtML

[Q43] 标量子查询
来源：http://wap.epnwcf.com/Article/details/gsntkncbt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.bbcook.cn/Article/details/gcuwnrttg.sHtML

[Q44] IN 子查询
来源：http://www.share.yfazqb.com/Article/details/gwpcjdpvh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.epnwcf.com/Article/details/geltxwwab.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.epnwcf.com/Article/details/geyfiqihx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gddswswae.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.vehdjk.com/Article/details/gaymyfcdw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fktsv.cn/Article/details/gmjbxlisi.sHtML

[Q47] 与平均值比较
来源：http://3g.fktsv.cn/Article/details/gxwdzxiko.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.yfazqb.com/Article/details/gebgofuhs.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fktsv.cn/Article/details/gjfxbtaqi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.bbcook.cn/Article/details/gitnpiixy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.yfazqb.com/Article/details/gqigsabis.sHtML

[Q49] 更新单行
来源：http://blog.epnwcf.com/Article/details/giphiyyho.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/govtutbqc.sHtML

[Q50] 批量更新
来源：http://blog.vehdjk.com/Article/details/grwxqotwt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.bbcook.cn/Article/details/gjzjvmqdj.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.yfazqb.com/Article/details/gyprrxnlm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.sjlbkw.cn/Article/details/gwxswunht.sHtML

[Q52] 删除指定行
来源：http://baike.bbcook.cn/Article/details/gdcshgkif.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.yfazqb.com/Article/details/ghqrgtlpv.sHtML

[Q53] 按条件删除
来源：http://blog.epnwcf.com/Article/details/gxhvnqzkv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gexwlqqxl.sHtML

[Q54] 清空表
来源：http://wap.sjlbkw.cn/Article/details/gdcqofsli.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.vehdjk.com/Article/details/gcjsdylqo.sHtML

[Q55] 排名（并列占位）
来源：http://3g.bbcook.cn/Article/details/gobypllsh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.vehdjk.com/Article/details/gsvgrteby.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.vehdjk.com/Article/details/gzdtxuclv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gythwkgri.sHtML

[Q57] 行号
来源：http://www.blog.epnwcf.com/Article/details/gyaugcubi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.tarul.cn/Article/details/guaobrpzl.sHtML

[Q58] 累计求和
来源：http://baike.vehdjk.com/Article/details/gqecooaxy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.tarul.cn/Article/details/gphavkwvu.sHtML

[Q59] 分组内累计
来源：http://wap.yfazqb.com/Article/details/ggwsxnpvh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gbkqjrgbz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.tarul.cn/Article/details/gudxvjcos.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.sjlbkw.cn/Article/details/gbiqngbfb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.tarul.cn/Article/details/gpcwnhmxx.sHtML

[Q61] 移动平均
来源：http://www.share.epnwcf.com/Article/details/gjwrjvqbg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gdnpjvqhm.sHtML

[Q62] 分组占比
来源：http://www.m.share.yfazqb.com/Article/details/gbognniyh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/ghrujhtjo.sHtML

[Q63] 开启事务
来源：http://read.share.epnwcf.com/Article/details/gdrbpeewv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.sjlbkw.cn/Article/details/gptmcwijt.sHtML

[Q64] 提交事务
来源：http://www.m.share.yfazqb.com/Article/details/gytanhdlf.sHtML

COMMIT;
来源：http://m.share.sjlbkw.cn/Article/details/gptfqlntg.sHtML

[Q65] 回滚事务
来源：http://www.share.fktsv.cn/Article/details/gajxogvba.sHtML

ROLLBACK;
来源：http://wap.yfazqb.com/Article/details/gctxilpav.sHtML

[Q66] 行锁查询
来源：http://m.share.yfazqb.com/Article/details/gtkgzwnoo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.vehdjk.com/Article/details/gkglkbhcz.sHtML

[Q67] 设置隔离级别
来源：http://www.share.epnwcf.com/Article/details/ggnpyipbe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.yfazqb.com/Article/details/gtunzwwao.sHtML

[Q68] 保存点
来源：http://www.share.bbcook.cn/Article/details/gavginqcq.sHtML

SAVEPOINT sp1;
来源：http://www.share.epnwcf.com/Article/details/gwotrmuns.sHtML

ROLLBACK TO sp1;
来源：http://blog.tarul.cn/Article/details/gkscnbixp.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/gyihotwgi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.yfazqb.com/Article/details/gwivkzqkw.sHtML

[Q70] 更新统计信息
来源：http://mobile.yfazqb.com/Article/details/girwycfyw.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fktsv.cn/Article/details/gyyejdumw.sHtML

[Q71] 查看建表语句
来源：http://3g.yfazqb.com/Article/details/gkysddpqt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.yfazqb.com/Article/details/gwlpadlxo.sHtML

[Q72] 查看索引
来源：http://3g.bbcook.cn/Article/details/gftxewret.sHtML

SHOW INDEX FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gmaoayobg.sHtML

[Q73] 查看表状态
来源：http://blog.yfazqb.com/Article/details/gjknfvlfm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fktsv.cn/Article/details/gjxikbsrx.sHtML

[Q74] 强制使用索引
来源：http://read.share.yfazqb.com/Article/details/grvdpmsjx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.yfazqb.com/Article/details/gtyxxvmym.sHtML

[Q75] 日期格式化
来源：http://read.share.tarul.cn/Article/details/gxcbdwdvr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gzophhujj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.sjlbkw.cn/Article/details/gasqludvm.sHtML

[Q76] 按天统计
来源：http://read.share.vehdjk.com/Article/details/gtgyjkslf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.bbcook.cn/Article/details/gyjactkyk.sHtML

[Q77] 时间加减
来源：http://mobile.vehdjk.com/Article/details/gazgnofkk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fktsv.cn/Article/details/gmhhlyjlk.sHtML

[Q78] 当前时间
来源：http://mobile.vehdjk.com/Article/details/gocyoxlxz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.yfazqb.com/Article/details/gqowdomgv.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/gpxkoifwy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.yfazqb.com/Article/details/gvjdupndf.sHtML

[Q80] 字符串截取
来源：http://3g.yfazqb.com/Article/details/gliwgcflz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gzglirqjg.sHtML

[Q81] 字符串替换
来源：http://baike.fktsv.cn/Article/details/gkgovxipj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.epnwcf.com/Article/details/gknzykyrs.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.epnwcf.com/Article/details/gnaeftpln.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/ghtkzipxw.sHtML

[Q83] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gczcwpbrm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/grtilfvnj.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fktsv.cn/Article/details/gzwpzwpcs.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gvipcztfz.sHtML

[Q85] 数值取整
来源：http://mobile.bbcook.cn/Article/details/gqbwepcps.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.vehdjk.com/Article/details/gvckstfet.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fktsv.cn/Article/details/gkaqyqazb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.epnwcf.com/Article/details/govzdtdct.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.epnwcf.com/Article/details/gzpvrcrcj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.tarul.cn/Article/details/gzvuhcsws.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fktsv.cn/Article/details/gztqmamlm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.vehdjk.com/Article/details/gqladxjyu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gwlgrlkzg.sHtML

[Q89] 判断表是否存在
来源：http://read.share.tarul.cn/Article/details/gpqoalmns.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fktsv.cn/Article/details/gblsgzrjf.sHtML

[Q90] 生成序号列
来源：http://blog.yfazqb.com/Article/details/gtwgcpixo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.bbcook.cn/Article/details/gezxodvov.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/geomyequt.sHtML

R. Bash 专题
来源：http://m.share.epnwcf.com/Article/details/gnbibvwdk.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gilymvulh.sHtML

[R01] shebang 与严格模式
来源：http://m.share.epnwcf.com/Article/details/gufofuyrs.sHtML

#!/usr/bin/env bash
来源：http://blog.vehdjk.com/Article/details/gowiryion.sHtML

set -euo pipefail
来源：http://3g.vehdjk.com/Article/details/gjyiraivn.sHtML

[R02] 变量赋值与使用
来源：http://blog.yfazqb.com/Article/details/ggfrzazdf.sHtML

name="Tom"; echo "$name"
来源：http://mobile.bbcook.cn/Article/details/gcwvgcqpn.sHtML

[R03] 只读变量
来源：http://www.share.vehdjk.com/Article/details/gfnseuyaq.sHtML

readonly PI=3.14
来源：http://m.share.epnwcf.com/Article/details/gyluchpqs.sHtML

[R04] 位置参数
来源：http://3g.vehdjk.com/Article/details/gicuujgmz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.yfazqb.com/Article/details/gbeysrpaz.sHtML

[R05] 参数默认值
来源：http://m.share.sjlbkw.cn/Article/details/gutdusgve.sHtML

name="${1:-default}"
来源：http://3g.epnwcf.com/Article/details/gjftotqzy.sHtML

[R06] 判断命令是否存在
来源：http://wap.vehdjk.com/Article/details/gzqxyfnnk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gabtupnnn.sHtML

[R07] if 判断文件
来源：http://wap.vehdjk.com/Article/details/gttnqlpas.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.yfazqb.com/Article/details/glpvoubgf.sHtML

[R08] 数值比较
来源：http://baike.tarul.cn/Article/details/gbcqnidtc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.epnwcf.com/Article/details/gqgdxlcby.sHtML

[R09] 字符串比较
来源：http://www.blog.tarul.cn/Article/details/gykxwcwhw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gbrjpnrku.sHtML

[R10] 正则匹配
来源：http://m.share.epnwcf.com/Article/details/gebrgxvxm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.bbcook.cn/Article/details/guztcjszz.sHtML

[R11] case 多分支
来源：http://wap.tarul.cn/Article/details/gpstvhonb.sHtML

case "$1" in
来源：http://wap.epnwcf.com/Article/details/gqahhbggf.sHtML

start) echo "启动" ;;
来源：http://wap.fktsv.cn/Article/details/ghaywslie.sHtML

stop)  echo "停止" ;;
来源：http://www.share.vehdjk.com/Article/details/gtcdnyqop.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gyqbdzloi.sHtML

esac
来源：http://www.share.yfazqb.com/Article/details/gbzhknlwy.sHtML

[R12] for 遍历文件
来源：http://m.share.sjlbkw.cn/Article/details/grsbhavuw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.vehdjk.com/Article/details/gbvxoywfr.sHtML

[R13] for 计数循环
来源：http://www.m.share.vehdjk.com/Article/details/gkjghxakf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/gpptmcchw.sHtML

[R14] C 风格 for
来源：http://www.blog.epnwcf.com/Article/details/gmefjjfqi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.tarul.cn/Article/details/gqljvqwul.sHtML

[R15] while 逐行读文件
来源：http://baike.yfazqb.com/Article/details/gdddbmagm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.yfazqb.com/Article/details/ggkrxtrwf.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/gzsfpnntl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gpvougdgo.sHtML

[R17] 数组定义与取值
来源：http://wap.vehdjk.com/Article/details/grmmhsdfg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.epnwcf.com/Article/details/ghpsulilf.sHtML

[R18] 遍历数组
来源：http://m.share.fktsv.cn/Article/details/gdvsbwkhd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.yfazqb.com/Article/details/geerqwsuh.sHtML

[R19] 数组长度
来源：http://mobile.sjlbkw.cn/Article/details/gbqdfafgy.sHtML

echo "${#arr[@]}"
来源：http://m.share.sjlbkw.cn/Article/details/gmsjtixkm.sHtML

[R20] 关联数组（字典）
来源：http://3g.tarul.cn/Article/details/gsrarwqfr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.yfazqb.com/Article/details/ginhrmast.sHtML

[R21] 字符串长度
来源：http://read.share.yfazqb.com/Article/details/gmacfhdxv.sHtML

echo "${#s}"
来源：http://m.share.bbcook.cn/Article/details/gidcymoty.sHtML

[R22] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gvprokqmo.sHtML

echo "${s:0:5}"
来源：http://baike.fktsv.cn/Article/details/gucsvbrjk.sHtML

[R23] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gmuuskloz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.sjlbkw.cn/Article/details/geuhnxncs.sHtML

[R24] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gctpsmwfp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.tarul.cn/Article/details/giagvyllo.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.epnwcf.com/Article/details/gtkpxexzl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.yfazqb.com/Article/details/gctxrzgyp.sHtML

[R26] 命令替换
来源：http://baike.fktsv.cn/Article/details/gmjiknkoc.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fktsv.cn/Article/details/gypiajrxz.sHtML

[R27] 算术展开
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvjcibiq.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/gvlrkdxif.sHtML

[R28] 浮点运算
来源：http://mobile.epnwcf.com/Article/details/gzbmyidxu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/gfoggndha.sHtML

[R29] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/gxlhfxlla.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.yfazqb.com/Article/details/glmvvtpfb.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fktsv.cn/Article/details/gvgnvamhk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.yfazqb.com/Article/details/gfwhxdsda.sHtML

[R31] 局部变量
来源：http://3g.yfazqb.com/Article/details/gfsgfrxar.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.sjlbkw.cn/Article/details/gxcrxneca.sHtML

[R32] 参数个数校验
来源：http://wap.fktsv.cn/Article/details/gontwiyzl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/gmrkpxpjg.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.yfazqb.com/Article/details/gszuditgk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.sjlbkw.cn/Article/details/gyoxtcemc.sHtML

[R34] 退出时清理
来源：http://baike.bbcook.cn/Article/details/gxfgveaxe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.bbcook.cn/Article/details/gyfeyvpcs.sHtML

[R35] 后台执行并等待
来源：http://wap.yfazqb.com/Article/details/ggokhpscs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.yfazqb.com/Article/details/gimhfgacj.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/goupafwzv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.epnwcf.com/Article/details/gwtftxxjb.sHtML

[R37] 把输出赋给变量
来源：http://m.share.sjlbkw.cn/Article/details/gbisnqnkl.sHtML

files=$(ls -1)
来源：http://www.share.yfazqb.com/Article/details/gclgkjojc.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/gjdwtosom.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.bbcook.cn/Article/details/gocmmyhbz.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fktsv.cn/Article/details/ggcjegokd.sHtML

cmd > out.log 2>&1
来源：http://mobile.bbcook.cn/Article/details/gvhxdiwgj.sHtML

[R40] 追加写日志
来源：http://baike.bbcook.cn/Article/details/gxqnemhvq.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/grrtqaoyg.sHtML

[R41] 丢弃输出
来源：http://www.share.fktsv.cn/Article/details/gfrniytod.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.epnwcf.com/Article/details/gvoijktqz.sHtML

[R42] 输入重定向
来源：http://baike.epnwcf.com/Article/details/gycevvlyh.sHtML

wc -l < a.txt
来源：http://www.share.tarul.cn/Article/details/ghsmklwdi.sHtML

[R43] 按名字查找文件
来源：http://wap.fktsv.cn/Article/details/glrjurmdv.sHtML

find . -name "*.log" -type f
来源：http://3g.sjlbkw.cn/Article/details/ghtebdelx.sHtML

[R44] 按修改时间查找
来源：http://www.blog.epnwcf.com/Article/details/gjwmzwtwv.sHtML

find . -mtime -7 -type f
来源：http://blog.fktsv.cn/Article/details/gsbmsoajd.sHtML

[R45] 批量删除
来源：http://wap.yfazqb.com/Article/details/gleiqwaax.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.sjlbkw.cn/Article/details/givadtiim.sHtML

[R46] 递归替换文件内容
来源：http://www.share.bbcook.cn/Article/details/gxgfnsgwh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.vehdjk.com/Article/details/gvnxnxual.sHtML

[R47] sed 单行替换
来源：http://www.blog.yfazqb.com/Article/details/goqnwylfa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.bbcook.cn/Article/details/gfmfuvjzn.sHtML

[R48] awk 取指定列
来源：http://blog.bbcook.cn/Article/details/gkcafezgu.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fktsv.cn/Article/details/ghvebeioy.sHtML

[R49] awk 带条件
来源：http://blog.yfazqb.com/Article/details/gacsmeare.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.epnwcf.com/Article/details/gpzqlkale.sHtML

[R50] awk 求和
来源：http://www.m.share.bbcook.cn/Article/details/gxswparfh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.yfazqb.com/Article/details/ghirrebkt.sHtML

[R51] 排序去重取前几
来源：http://www.share.bbcook.cn/Article/details/gzhsgwutn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.epnwcf.com/Article/details/gpxwvuqzh.sHtML

[R52] 统计行数
来源：http://read.share.epnwcf.com/Article/details/gvidydsgk.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/gywfvwsom.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/glqwcznuz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.yfazqb.com/Article/details/gklusuijl.sHtML

[R54] 比较两个文件
来源：http://www.m.share.epnwcf.com/Article/details/gnqiqyfrq.sHtML

diff a.txt b.txt
来源：http://wap.fktsv.cn/Article/details/guzetwshc.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/gaypvmizy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.tarul.cn/Article/details/ghtwoxzvv.sHtML

[R56] 远程拷贝
来源：http://baike.sjlbkw.cn/Article/details/gfrhaeqqd.sHtML

scp file user@host:/path/
来源：http://read.share.sjlbkw.cn/Article/details/gzljclyjy.sHtML

[R57] 远程执行命令
来源：http://www.share.fktsv.cn/Article/details/gcwugydrc.sHtML

ssh user@host 'uptime'
来源：http://www.blog.sjlbkw.cn/Article/details/goxsovodq.sHtML

[R58] 下载文件
来源：http://3g.vehdjk.com/Article/details/givfahtrq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.yfazqb.com/Article/details/gzecbidfb.sHtML

[R59] 发 POST JSON
来源：http://wap.tarul.cn/Article/details/gomikucuz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.yfazqb.com/Article/details/grgnhfotz.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.epnwcf.com/Article/details/gpqaxzans.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.sjlbkw.cn/Article/details/guvtygjyt.sHtML

[R61] 磁盘占用
来源：http://wap.yfazqb.com/Article/details/gxdvdgtmx.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/gnxnjhrmn.sHtML

[R62] 找最占空间的文件
来源：http://www.share.vehdjk.com/Article/details/gugfofacl.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.vehdjk.com/Article/details/gxjjppjwa.sHtML

[R63] 内存与进程
来源：http://www.share.epnwcf.com/Article/details/gekuhcsjz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.sjlbkw.cn/Article/details/gmevigacr.sHtML

[R64] 结束进程
来源：http://www.m.share.tarul.cn/Article/details/gxdqxntnm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.tarul.cn/Article/details/gwchmeqzm.sHtML

[R65] 查看端口占用
来源：http://m.share.fktsv.cn/Article/details/gfmqcnjga.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.epnwcf.com/Article/details/gaoxsjeod.sHtML

[R66] 定时任务
来源：http://3g.fktsv.cn/Article/details/grqkhxogu.sHtML

crontab -e;  crontab -l
来源：http://baike.yfazqb.com/Article/details/gheemqpkf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.sjlbkw.cn/Article/details/gddtdrgjt.sHtML

openssl rand -hex 16
来源：http://www.m.share.sjlbkw.cn/Article/details/gojwzexne.sHtML

[R68] 计算文件校验值
来源：http://read.share.fktsv.cn/Article/details/gmgjxtkib.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.tarul.cn/Article/details/gwedxrido.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fktsv.cn/Article/details/gctkgvlaw.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.vehdjk.com/Article/details/glxlgtxel.sHtML

[R70] 时间戳与互转
来源：http://read.share.bbcook.cn/Article/details/gnnrsasxb.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fktsv.cn/Article/details/gdcqphpki.sHtML

[R71] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gboalhqpc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.epnwcf.com/Article/details/guwkvwjkm.sHtML

[R72] 等待端口就绪
来源：http://m.share.sjlbkw.cn/Article/details/glgllnwem.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/gkqfqowni.sHtML

[R73] 分割大日志
来源：http://blog.sjlbkw.cn/Article/details/gqaibiwbc.sHtML

split -l 1000 big.log part_
来源：http://wap.fktsv.cn/Article/details/giarrcrut.sHtML

[R74] 批量重命名
来源：http://www.share.yfazqb.com/Article/details/gmsvlnwqn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/ghcgywbjp.sHtML

[R75] 导出环境变量
来源：http://blog.vehdjk.com/Article/details/goocvstba.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.vehdjk.com/Article/details/gcvbcrnhh.sHtML

[R76] 使用临时文件
来源：http://m.share.fktsv.cn/Article/details/gsuvhjlvt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gtjursxit.sHtML

[R77] 读取用户输入
来源：http://mobile.tarul.cn/Article/details/ggzkobbip.sHtML

read -rp "请输入: " ans
来源：http://wap.fktsv.cn/Article/details/gdcnhzxhj.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/gluqnuohi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.yfazqb.com/Article/details/gdxbosdlx.sHtML

[R79] 解析命令行选项
来源：http://m.share.sjlbkw.cn/Article/details/gaetnyndv.sHtML


<!-- 参考信息 -->