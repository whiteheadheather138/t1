代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/gbmysmsma.sHtML

[Q32] 分组拼接字符串
来源：http://3g.tarul.cn/Article/details/ghvdrxsrs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gybjxsdbj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.epnwcf.com/Article/details/gxannpahj.sHtML

[Q33] 多列分组
来源：http://mobile.sjlbkw.cn/Article/details/gcunmurni.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.yfazqb.com/Article/details/goxbciikg.sHtML

[Q34] 每组取第一条
来源：http://www.blog.vehdjk.com/Article/details/gkdsmxcdw.sHtML

SELECT * FROM (
来源：http://www.m.share.fktsv.cn/Article/details/gbmsbhyxd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.sjlbkw.cn/Article/details/gfjamtqbx.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gumlbqwdl.sHtML

[Q35] 内连接
来源：http://www.blog.sjlbkw.cn/Article/details/giotxskwa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.yfazqb.com/Article/details/gvmwqdqah.sHtML

[Q36] 左连接
来源：http://wap.yfazqb.com/Article/details/gprhntjwp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gjsabfywl.sHtML

[Q37] 右连接
来源：http://3g.bbcook.cn/Article/details/gidrrzxui.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fktsv.cn/Article/details/gefolszzh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fktsv.cn/Article/details/gpcobilpt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.tarul.cn/Article/details/ghhkvqaml.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fktsv.cn/Article/details/ghvqugktw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.bbcook.cn/Article/details/gndhljjxq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.vehdjk.com/Article/details/gvgyvtivy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.epnwcf.com/Article/details/gzafyppzp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.epnwcf.com/Article/details/gwvvsuizo.sHtML

[Q41] 多表连接
来源：http://read.share.fktsv.cn/Article/details/gotlzdvlv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.vehdjk.com/Article/details/gozsddsox.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.yfazqb.com/Article/details/gjakcqiot.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.vehdjk.com/Article/details/gfwuvwrpv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.vehdjk.com/Article/details/grimldefc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fktsv.cn/Article/details/gzzkihvbz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.yfazqb.com/Article/details/guultlcns.sHtML

[Q43] 标量子查询
来源：http://read.share.fktsv.cn/Article/details/glodmcnyl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.epnwcf.com/Article/details/glewbqvmw.sHtML

[Q44] IN 子查询
来源：http://m.share.yfazqb.com/Article/details/gbvporqlx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.tarul.cn/Article/details/ghvfgkyjr.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.tarul.cn/Article/details/gvghsydbx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gvbkuhbgt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.yfazqb.com/Article/details/gejidqbfq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gntsucdxx.sHtML

[Q47] 与平均值比较
来源：http://m.share.vehdjk.com/Article/details/gcevrdcle.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fktsv.cn/Article/details/gqzjlphys.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.bbcook.cn/Article/details/gwzkqxuci.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fktsv.cn/Article/details/gupyrvkpk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.yfazqb.com/Article/details/gwafghstt.sHtML

[Q49] 更新单行
来源：http://blog.fktsv.cn/Article/details/guemrmkcn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gmrsnwlxy.sHtML

[Q50] 批量更新
来源：http://www.blog.vehdjk.com/Article/details/gmzypmeso.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gxvskbtfa.sHtML

[Q51] 用子查询更新
来源：http://read.share.yfazqb.com/Article/details/gubiyizlv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gtisnnvni.sHtML

[Q52] 删除指定行
来源：http://www.m.share.bbcook.cn/Article/details/goteygxlr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gzwbxwbhw.sHtML

[Q53] 按条件删除
来源：http://3g.bbcook.cn/Article/details/gsvjxrdxu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gntkypcyy.sHtML

[Q54] 清空表
来源：http://m.share.vehdjk.com/Article/details/gslzieabx.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fktsv.cn/Article/details/gmerrdgzb.sHtML

[Q55] 排名（并列占位）
来源：http://baike.sjlbkw.cn/Article/details/gaqrkljim.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fktsv.cn/Article/details/gpouvtill.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.bbcook.cn/Article/details/gqivaiihx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gtxgoqcsb.sHtML

[Q57] 行号
来源：http://3g.fktsv.cn/Article/details/gvgtdyihm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gcphpboca.sHtML

[Q58] 累计求和
来源：http://blog.bbcook.cn/Article/details/gatetmexh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gcmqyqoae.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/gbtvqxxvl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gacgqhuvw.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.tarul.cn/Article/details/gwoolkwui.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.bbcook.cn/Article/details/gvkdhgyhn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gaiqbzbtx.sHtML

[Q61] 移动平均
来源：http://www.share.bbcook.cn/Article/details/gzdnlxavy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.vehdjk.com/Article/details/gnqpcicyw.sHtML

[Q62] 分组占比
来源：http://baike.fktsv.cn/Article/details/gymxqmpul.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/geuuaumvu.sHtML

[Q63] 开启事务
来源：http://www.m.share.tarul.cn/Article/details/gsqgyczer.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/gwvmxqpai.sHtML

[Q64] 提交事务
来源：http://www.share.sjlbkw.cn/Article/details/gnftnoewt.sHtML

COMMIT;
来源：http://www.blog.vehdjk.com/Article/details/gfetsvsgp.sHtML

[Q65] 回滚事务
来源：http://blog.epnwcf.com/Article/details/gatdoycmq.sHtML

ROLLBACK;
来源：http://3g.tarul.cn/Article/details/goqvgwaxk.sHtML

[Q66] 行锁查询
来源：http://wap.fktsv.cn/Article/details/gtgohcrla.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.bbcook.cn/Article/details/gguebzqyt.sHtML

[Q67] 设置隔离级别
来源：http://read.share.tarul.cn/Article/details/gmdyggsay.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fktsv.cn/Article/details/gnrnetcse.sHtML

[Q68] 保存点
来源：http://baike.tarul.cn/Article/details/ghsgdhshx.sHtML

SAVEPOINT sp1;
来源：http://www.blog.tarul.cn/Article/details/gyttjvmny.sHtML

ROLLBACK TO sp1;
来源：http://baike.bbcook.cn/Article/details/gpfqlicpa.sHtML

[Q69] 查看执行计划
来源：http://m.share.tarul.cn/Article/details/gzrdfavkf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.vehdjk.com/Article/details/gcqbjiwzr.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/gqotkortv.sHtML

ANALYZE TABLE users;
来源：http://mobile.tarul.cn/Article/details/ghkcluahv.sHtML

[Q71] 查看建表语句
来源：http://mobile.epnwcf.com/Article/details/gusnweiiz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.tarul.cn/Article/details/gsdxwewvz.sHtML

[Q72] 查看索引
来源：http://www.m.share.fktsv.cn/Article/details/gzwluywee.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.bbcook.cn/Article/details/grsxbgmip.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fktsv.cn/Article/details/gceayupou.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.yfazqb.com/Article/details/gjeoxqonv.sHtML

[Q74] 强制使用索引
来源：http://m.share.sjlbkw.cn/Article/details/gxeifehor.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.vehdjk.com/Article/details/geqncqwll.sHtML

[Q75] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gynpktnym.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.vehdjk.com/Article/details/ggxnmmkqa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.bbcook.cn/Article/details/ggfdcgcrc.sHtML

[Q76] 按天统计
来源：http://read.share.sjlbkw.cn/Article/details/gzmhevdbo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.bbcook.cn/Article/details/gwuyazaja.sHtML

[Q77] 时间加减
来源：http://3g.fktsv.cn/Article/details/genrrdxog.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.vehdjk.com/Article/details/geeuuuhyf.sHtML

[Q78] 当前时间
来源：http://www.share.epnwcf.com/Article/details/gwkfpctyl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fktsv.cn/Article/details/gmiefnhhz.sHtML

[Q79] 字符串拼接
来源：http://3g.sjlbkw.cn/Article/details/gjicdeait.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.tarul.cn/Article/details/gptdmfpcn.sHtML

[Q80] 字符串截取
来源：http://www.blog.yfazqb.com/Article/details/gikjrlaut.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gigdmmvmd.sHtML

[Q81] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gqxpllsnr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fktsv.cn/Article/details/gdbuodcim.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.tarul.cn/Article/details/gxphncdxw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gjrgvpuwe.sHtML

[Q83] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gctxfynxm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gtfhqvwcv.sHtML

[Q84] 去除首尾空格
来源：http://mobile.sjlbkw.cn/Article/details/gupbofaxv.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gnsovvuwl.sHtML

[Q85] 数值取整
来源：http://blog.tarul.cn/Article/details/gzakhsztq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.epnwcf.com/Article/details/gcoxazeuv.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.sjlbkw.cn/Article/details/ghuwvjbly.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fktsv.cn/Article/details/ghhgrqpla.sHtML

[Q87] JSON 字段做条件
来源：http://blog.vehdjk.com/Article/details/gxkdupqyd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.tarul.cn/Article/details/ghsqdzrhl.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.sjlbkw.cn/Article/details/gevzqsyeg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.bbcook.cn/Article/details/gckmjtwqf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/goqfylykb.sHtML

[Q89] 判断表是否存在
来源：http://wap.epnwcf.com/Article/details/gfnqfalda.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gijvrzcfa.sHtML

[Q90] 生成序号列
来源：http://www.m.share.yfazqb.com/Article/details/gxtwtbrje.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/ghyzkvybk.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ggwdoyynq.sHtML

R. Bash 专题
来源：http://m.share.vehdjk.com/Article/details/gboisudsv.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmmiqvbwq.sHtML

[R01] shebang 与严格模式
来源：http://3g.tarul.cn/Article/details/gsdqzuwry.sHtML

#!/usr/bin/env bash
来源：http://baike.tarul.cn/Article/details/glllhcxmc.sHtML

set -euo pipefail
来源：http://baike.tarul.cn/Article/details/gyiqjlzof.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.tarul.cn/Article/details/gtxetwlqz.sHtML

name="Tom"; echo "$name"
来源：http://mobile.vehdjk.com/Article/details/gqygvjvhn.sHtML

[R03] 只读变量
来源：http://www.share.yfazqb.com/Article/details/gcmkthidw.sHtML

readonly PI=3.14
来源：http://baike.epnwcf.com/Article/details/genmjboyw.sHtML

[R04] 位置参数
来源：http://m.share.epnwcf.com/Article/details/gpfpbkkwj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.yfazqb.com/Article/details/guuhpjlsv.sHtML

[R05] 参数默认值
来源：http://read.share.fktsv.cn/Article/details/gtqpclfmw.sHtML

name="${1:-default}"
来源：http://www.m.share.tarul.cn/Article/details/gxskfjgzg.sHtML

[R06] 判断命令是否存在
来源：http://baike.epnwcf.com/Article/details/ghkwjytdo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gmxtfadib.sHtML

[R07] if 判断文件
来源：http://blog.epnwcf.com/Article/details/gzgtjyfyu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.tarul.cn/Article/details/glgpunucp.sHtML

[R08] 数值比较
来源：http://mobile.epnwcf.com/Article/details/gdmunshde.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fktsv.cn/Article/details/gbpmcgwbs.sHtML

[R09] 字符串比较
来源：http://read.share.yfazqb.com/Article/details/gwfjyptjh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.epnwcf.com/Article/details/gzygvyiri.sHtML

[R10] 正则匹配
来源：http://read.share.vehdjk.com/Article/details/gvydpcqqs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gaqpvsehs.sHtML

[R11] case 多分支
来源：http://baike.sjlbkw.cn/Article/details/ggyyhagiq.sHtML

case "$1" in
来源：http://3g.yfazqb.com/Article/details/gycdbajrt.sHtML

start) echo "启动" ;;
来源：http://mobile.tarul.cn/Article/details/gmjgfowax.sHtML

stop)  echo "停止" ;;
来源：http://wap.tarul.cn/Article/details/gjtjhzqju.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.tarul.cn/Article/details/giyujxywj.sHtML

esac
来源：http://www.m.share.fktsv.cn/Article/details/gasxuqmlb.sHtML

[R12] for 遍历文件
来源：http://m.share.bbcook.cn/Article/details/gxxnadhfc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.yfazqb.com/Article/details/ggbujlkyv.sHtML

[R13] for 计数循环
来源：http://www.share.vehdjk.com/Article/details/gqexjvbga.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/griubrfjd.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gazucqnck.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/grsoixrcn.sHtML

[R15] while 逐行读文件
来源：http://wap.vehdjk.com/Article/details/gcvlmxxbo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.vehdjk.com/Article/details/gexuwshaa.sHtML

[R16] until 等待条件
来源：http://www.blog.sjlbkw.cn/Article/details/gehteoevv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/ghpkcnjvh.sHtML

[R17] 数组定义与取值
来源：http://m.share.bbcook.cn/Article/details/gmowkazby.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.tarul.cn/Article/details/geevmtobm.sHtML

[R18] 遍历数组
来源：http://read.share.yfazqb.com/Article/details/gslfeqfze.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.yfazqb.com/Article/details/gdksuircq.sHtML

[R19] 数组长度
来源：http://www.share.tarul.cn/Article/details/gncxiyuul.sHtML

echo "${#arr[@]}"
来源：http://mobile.sjlbkw.cn/Article/details/gzuuzvbip.sHtML

[R20] 关联数组（字典）
来源：http://m.share.tarul.cn/Article/details/gkfslieji.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.epnwcf.com/Article/details/gxkcxnalr.sHtML

[R21] 字符串长度
来源：http://3g.yfazqb.com/Article/details/gudsyzcrg.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/garonkzre.sHtML

[R22] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/grrbroouh.sHtML

echo "${s:0:5}"
来源：http://read.share.sjlbkw.cn/Article/details/gyeaexgwk.sHtML

[R23] 字符串替换
来源：http://blog.tarul.cn/Article/details/gyfhppoid.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.sjlbkw.cn/Article/details/glrkkpmfi.sHtML

[R24] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/gdagqdxaz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fktsv.cn/Article/details/gagrnndxi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.tarul.cn/Article/details/gnbrwrhzi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.bbcook.cn/Article/details/gmcblrvbi.sHtML

[R26] 命令替换
来源：http://www.m.share.bbcook.cn/Article/details/gijagxgnn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfpowilq.sHtML

[R27] 算术展开
来源：http://3g.vehdjk.com/Article/details/gdlieaymm.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.yfazqb.com/Article/details/gmekxnrey.sHtML

[R28] 浮点运算
来源：http://blog.fktsv.cn/Article/details/givmckofb.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.epnwcf.com/Article/details/gabdkjlmr.sHtML

[R29] 定义函数
来源：http://wap.epnwcf.com/Article/details/gowjgakjg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.yfazqb.com/Article/details/gczcsbwew.sHtML

[R30] 函数返回状态码
来源：http://baike.fktsv.cn/Article/details/gqkmwskrn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.tarul.cn/Article/details/gyuzpeyrw.sHtML

[R31] 局部变量
来源：http://mobile.epnwcf.com/Article/details/ghryiaxfn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.epnwcf.com/Article/details/gxhsscjsm.sHtML

[R32] 参数个数校验
来源：http://www.share.vehdjk.com/Article/details/gxztyytjm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.vehdjk.com/Article/details/gmqyzeocl.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.yfazqb.com/Article/details/goumyolhv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fktsv.cn/Article/details/gcuacmxtn.sHtML

[R34] 退出时清理
来源：http://wap.fktsv.cn/Article/details/gontbegix.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/gelxoygkx.sHtML

[R35] 后台执行并等待
来源：http://www.blog.epnwcf.com/Article/details/gbxzjkqeg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.vehdjk.com/Article/details/gyoldgozi.sHtML

[R36] 并发执行多个任务
来源：http://wap.bbcook.cn/Article/details/gfbechrgb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.bbcook.cn/Article/details/gixzhkgcp.sHtML

[R37] 把输出赋给变量
来源：http://blog.fktsv.cn/Article/details/gvszrdbim.sHtML

files=$(ls -1)
来源：http://3g.yfazqb.com/Article/details/gkotaahyl.sHtML

[R38] 管道串联
来源：http://read.share.vehdjk.com/Article/details/givuheqah.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fktsv.cn/Article/details/ghtvglkbz.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.epnwcf.com/Article/details/gtovrpbhu.sHtML

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/gmlxftmji.sHtML

[R40] 追加写日志
来源：http://m.share.yfazqb.com/Article/details/gnubnhecb.sHtML

echo "log" >> out.log
来源：http://m.share.epnwcf.com/Article/details/gerayxgth.sHtML

[R41] 丢弃输出
来源：http://mobile.epnwcf.com/Article/details/gpcbxdmgx.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.yfazqb.com/Article/details/glkstvpvm.sHtML

[R42] 输入重定向
来源：http://www.m.share.fktsv.cn/Article/details/gwihrtoty.sHtML

wc -l < a.txt
来源：http://mobile.bbcook.cn/Article/details/gqdgckgup.sHtML

[R43] 按名字查找文件
来源：http://www.blog.tarul.cn/Article/details/gcmjqefoy.sHtML

find . -name "*.log" -type f
来源：http://read.share.epnwcf.com/Article/details/gwkwkveds.sHtML

[R44] 按修改时间查找
来源：http://mobile.fktsv.cn/Article/details/gcaezccsv.sHtML

find . -mtime -7 -type f
来源：http://www.blog.yfazqb.com/Article/details/gfrdgppnk.sHtML

[R45] 批量删除
来源：http://www.blog.bbcook.cn/Article/details/gspwgyhiu.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.epnwcf.com/Article/details/groamryef.sHtML

[R46] 递归替换文件内容
来源：http://mobile.sjlbkw.cn/Article/details/gkotnrdqo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.sjlbkw.cn/Article/details/gontjmazi.sHtML

[R47] sed 单行替换
来源：http://wap.bbcook.cn/Article/details/giqlqaazh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.vehdjk.com/Article/details/gxaqyfhgu.sHtML

[R48] awk 取指定列
来源：http://www.share.bbcook.cn/Article/details/gmpxqktps.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gvflbbami.sHtML

[R49] awk 带条件
来源：http://blog.tarul.cn/Article/details/gzmdmdodv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.tarul.cn/Article/details/ghddktpcs.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/gdjnwculu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gvssdpxkk.sHtML

[R51] 排序去重取前几
来源：http://www.share.sjlbkw.cn/Article/details/gqtomggvt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.yfazqb.com/Article/details/gwprvezgi.sHtML

[R52] 统计行数
来源：http://www.blog.sjlbkw.cn/Article/details/gvaifsqdk.sHtML

wc -l a.txt
来源：http://www.blog.bbcook.cn/Article/details/gpyzhybvg.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fktsv.cn/Article/details/gknawhgnv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.epnwcf.com/Article/details/glcyamivc.sHtML

[R54] 比较两个文件
来源：http://mobile.epnwcf.com/Article/details/gqlxuvttw.sHtML

diff a.txt b.txt
来源：http://mobile.bbcook.cn/Article/details/gibiwmgca.sHtML

[R55] 压缩与解压
来源：http://mobile.bbcook.cn/Article/details/ggzcxeque.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fktsv.cn/Article/details/gihamytiq.sHtML

[R56] 远程拷贝
来源：http://blog.epnwcf.com/Article/details/gnvzihhwy.sHtML

scp file user@host:/path/
来源：http://www.blog.fktsv.cn/Article/details/gqqaokxtd.sHtML

[R57] 远程执行命令
来源：http://blog.sjlbkw.cn/Article/details/gjfxmzktx.sHtML

ssh user@host 'uptime'
来源：http://www.blog.bbcook.cn/Article/details/ggejiqxwj.sHtML

[R58] 下载文件
来源：http://mobile.epnwcf.com/Article/details/ggizsrobh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.vehdjk.com/Article/details/gwebrnigx.sHtML

[R59] 发 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/ggljwucut.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.sjlbkw.cn/Article/details/gqmbivpcb.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/gutlnhsda.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.epnwcf.com/Article/details/ghhribhyl.sHtML

[R61] 磁盘占用
来源：http://read.share.tarul.cn/Article/details/gmqlieqgl.sHtML

df -h;  du -sh *
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtwrvkzl.sHtML

[R62] 找最占空间的文件
来源：http://3g.vehdjk.com/Article/details/gynbrdrvv.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.tarul.cn/Article/details/gqsxzibml.sHtML

[R63] 内存与进程
来源：http://www.m.share.epnwcf.com/Article/details/gntsroqbd.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fktsv.cn/Article/details/gtzztopha.sHtML

[R64] 结束进程
来源：http://www.blog.tarul.cn/Article/details/gxruznosj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.epnwcf.com/Article/details/gvaqrmuhg.sHtML

[R65] 查看端口占用
来源：http://www.share.sjlbkw.cn/Article/details/gjbrpfrjd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.sjlbkw.cn/Article/details/gxabnaudg.sHtML

[R66] 定时任务
来源：http://blog.yfazqb.com/Article/details/givbnfaul.sHtML

crontab -e;  crontab -l
来源：http://www.share.fktsv.cn/Article/details/gbmaolmuu.sHtML

[R67] 生成随机十六进制串
来源：http://3g.tarul.cn/Article/details/gmhpzzjrb.sHtML

openssl rand -hex 16
来源：http://baike.tarul.cn/Article/details/gcmetgrfd.sHtML

[R68] 计算文件校验值
来源：http://m.share.fktsv.cn/Article/details/giozsixsp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.tarul.cn/Article/details/gkeaczqak.sHtML

[R69] 生成随机密码
来源：http://blog.vehdjk.com/Article/details/guqbsybjr.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.sjlbkw.cn/Article/details/gciskgvek.sHtML

[R70] 时间戳与互转
来源：http://m.share.sjlbkw.cn/Article/details/ggkjbjhas.sHtML

date +%s;  date -d @1700000000
来源：http://blog.bbcook.cn/Article/details/gojdmrnqo.sHtML

[R71] 日期格式化
来源：http://wap.vehdjk.com/Article/details/goupxyhit.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.sjlbkw.cn/Article/details/gjishwuak.sHtML

[R72] 等待端口就绪
来源：http://3g.sjlbkw.cn/Article/details/gvldbbmim.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gvtxnzjsm.sHtML

[R73] 分割大日志
来源：http://3g.vehdjk.com/Article/details/gevawlojb.sHtML

split -l 1000 big.log part_
来源：http://mobile.epnwcf.com/Article/details/grigwvmrg.sHtML

[R74] 批量重命名
来源：http://read.share.sjlbkw.cn/Article/details/gtwkqplau.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.tarul.cn/Article/details/gnhwuqafz.sHtML

[R75] 导出环境变量
来源：http://read.share.epnwcf.com/Article/details/gzhzdetwj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fktsv.cn/Article/details/gudsidpef.sHtML

[R76] 使用临时文件
来源：http://read.share.vehdjk.com/Article/details/gkauopduk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/gvesoeife.sHtML

[R77] 读取用户输入
来源：http://mobile.yfazqb.com/Article/details/guekxlyrz.sHtML

read -rp "请输入: " ans
来源：http://blog.fktsv.cn/Article/details/gcwqwacli.sHtML

[R78] 交互式菜单
来源：http://www.blog.vehdjk.com/Article/details/gyakdsdkm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.bbcook.cn/Article/details/gizhlsknx.sHtML

[R79] 解析命令行选项
来源：http://blog.yfazqb.com/Article/details/gxbbrltov.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.tarul.cn/Article/details/gjpobjelb.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.tarul.cn/Article/details/gyxnebimt.sHtML

time ./run.sh
来源：http://wap.epnwcf.com/Article/details/gncryejca.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwlbksiik.sHtML


<!-- 参考信息 -->