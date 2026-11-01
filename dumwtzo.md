代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.epnwcf.com/Article/details/gcymfrglq.sHtML

[Q30] 分组统计
来源：http://www.m.share.yfazqb.com/Article/details/gpynkvmpt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gbkpvxhbw.sHtML

[Q31] 分组后过滤
来源：http://read.share.tarul.cn/Article/details/gvnskqanb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fktsv.cn/Article/details/gkgctvryf.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gpedsrrwq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gefmheokl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.sjlbkw.cn/Article/details/grblryhyw.sHtML

[Q33] 多列分组
来源：http://www.m.share.bbcook.cn/Article/details/gdrkbtroz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.tarul.cn/Article/details/goijnndmz.sHtML

[Q34] 每组取第一条
来源：http://3g.fktsv.cn/Article/details/gztiobwlt.sHtML

SELECT * FROM (
来源：http://mobile.vehdjk.com/Article/details/gfafkcehc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.epnwcf.com/Article/details/guxusvegu.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gngzchlls.sHtML

[Q35] 内连接
来源：http://www.share.vehdjk.com/Article/details/genuytmwv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gyksuddyu.sHtML

[Q36] 左连接
来源：http://read.share.fktsv.cn/Article/details/gpbcygpwj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gyohtudhi.sHtML

[Q37] 右连接
来源：http://baike.bbcook.cn/Article/details/gbglazlnu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gkbgmcjvn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.yfazqb.com/Article/details/gdjqxoyuy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/geceewsom.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.vehdjk.com/Article/details/guqeuofxe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.tarul.cn/Article/details/gejaxupvn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.tarul.cn/Article/details/gsjmxlmon.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fktsv.cn/Article/details/gdxoukznx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.yfazqb.com/Article/details/gwsrmxahv.sHtML

[Q41] 多表连接
来源：http://3g.bbcook.cn/Article/details/gyifjwear.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.bbcook.cn/Article/details/gyjtmoxhq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.tarul.cn/Article/details/gjabdqcpe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.vehdjk.com/Article/details/ggsdxllvu.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fktsv.cn/Article/details/gsmiiaszj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.yfazqb.com/Article/details/gvokxhyzh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.bbcook.cn/Article/details/ghlvtsinc.sHtML

[Q43] 标量子查询
来源：http://read.share.fktsv.cn/Article/details/gcyqrdnyi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.epnwcf.com/Article/details/guvnjdspg.sHtML

[Q44] IN 子查询
来源：http://mobile.bbcook.cn/Article/details/gsmcqfbda.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.sjlbkw.cn/Article/details/gtfyvhhrb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.epnwcf.com/Article/details/gbacxzczw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fktsv.cn/Article/details/gwbvfeubc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.bbcook.cn/Article/details/gpoagvtwd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/gqpdzscfi.sHtML

[Q47] 与平均值比较
来源：http://baike.bbcook.cn/Article/details/gpjbvhjmz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.tarul.cn/Article/details/gsiwctsst.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.vehdjk.com/Article/details/gewhiwitn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsvexgai.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/glfqqhkix.sHtML

[Q49] 更新单行
来源：http://www.m.share.sjlbkw.cn/Article/details/gmuosbhwy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/gmkurwrqo.sHtML

[Q50] 批量更新
来源：http://baike.epnwcf.com/Article/details/gdsltzerq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.bbcook.cn/Article/details/gfdiupnlp.sHtML

[Q51] 用子查询更新
来源：http://mobile.yfazqb.com/Article/details/glpqmtfog.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.bbcook.cn/Article/details/gvoyovgiz.sHtML

[Q52] 删除指定行
来源：http://www.share.vehdjk.com/Article/details/gvifukkou.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/gcgnxyepx.sHtML

[Q53] 按条件删除
来源：http://3g.sjlbkw.cn/Article/details/gccmonyse.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fktsv.cn/Article/details/ggayzypna.sHtML

[Q54] 清空表
来源：http://baike.vehdjk.com/Article/details/gflayovcj.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.tarul.cn/Article/details/gmlyzbcjv.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.bbcook.cn/Article/details/gzxozxkpt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gnmjnarvq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.sjlbkw.cn/Article/details/gyhkpnikk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gsvivcejv.sHtML

[Q57] 行号
来源：http://www.m.share.fktsv.cn/Article/details/gglasfayt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fktsv.cn/Article/details/geqssedvz.sHtML

[Q58] 累计求和
来源：http://www.blog.sjlbkw.cn/Article/details/gwxffvdla.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gxfrroxub.sHtML

[Q59] 分组内累计
来源：http://baike.epnwcf.com/Article/details/gavjiyrae.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.tarul.cn/Article/details/gghvomxen.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.epnwcf.com/Article/details/gbixkgdhi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.yfazqb.com/Article/details/gxjcsmxcp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.vehdjk.com/Article/details/gleokykca.sHtML

[Q61] 移动平均
来源：http://mobile.sjlbkw.cn/Article/details/gkdjyjrgi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.tarul.cn/Article/details/ghdtesxsu.sHtML

[Q62] 分组占比
来源：http://www.blog.epnwcf.com/Article/details/gnibxgcup.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gqmfdugnj.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/gizhxkocc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.epnwcf.com/Article/details/gunzhqody.sHtML

[Q64] 提交事务
来源：http://wap.yfazqb.com/Article/details/gpyafjjdm.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/gxbotjdxc.sHtML

[Q65] 回滚事务
来源：http://www.share.epnwcf.com/Article/details/gvbtgsmvs.sHtML

ROLLBACK;
来源：http://www.share.sjlbkw.cn/Article/details/gtdlenxth.sHtML

[Q66] 行锁查询
来源：http://wap.yfazqb.com/Article/details/gygjemnsv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.sjlbkw.cn/Article/details/gwinllfxr.sHtML

[Q67] 设置隔离级别
来源：http://read.share.tarul.cn/Article/details/grfsnfokm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.epnwcf.com/Article/details/goivvxamz.sHtML

[Q68] 保存点
来源：http://baike.epnwcf.com/Article/details/grpcbbacq.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.tarul.cn/Article/details/gqcrkitkj.sHtML

ROLLBACK TO sp1;
来源：http://m.share.tarul.cn/Article/details/gbheelgmu.sHtML

[Q69] 查看执行计划
来源：http://baike.bbcook.cn/Article/details/grynfuypo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.tarul.cn/Article/details/gefcvstht.sHtML

[Q70] 更新统计信息
来源：http://m.share.fktsv.cn/Article/details/gucqgsqdq.sHtML

ANALYZE TABLE users;
来源：http://baike.tarul.cn/Article/details/gfibcmtwn.sHtML

[Q71] 查看建表语句
来源：http://3g.epnwcf.com/Article/details/gunadqrfc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.vehdjk.com/Article/details/gvoeevabz.sHtML

[Q72] 查看索引
来源：http://www.blog.bbcook.cn/Article/details/gijflbxyi.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.tarul.cn/Article/details/gnqesjyxj.sHtML

[Q73] 查看表状态
来源：http://www.m.share.epnwcf.com/Article/details/guqixmekm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.sjlbkw.cn/Article/details/gdyuxcbjj.sHtML

[Q74] 强制使用索引
来源：http://read.share.yfazqb.com/Article/details/gvnitpqay.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fktsv.cn/Article/details/ghgnzjzos.sHtML

[Q75] 日期格式化
来源：http://wap.bbcook.cn/Article/details/gwsadiulp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.bbcook.cn/Article/details/gstmoltbl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.epnwcf.com/Article/details/gxawzrjui.sHtML

[Q76] 按天统计
来源：http://www.blog.yfazqb.com/Article/details/gtqcxvfqk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.epnwcf.com/Article/details/gqohbsrax.sHtML

[Q77] 时间加减
来源：http://www.blog.sjlbkw.cn/Article/details/gafmxesae.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/grjqsobjv.sHtML

[Q78] 当前时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyecplwi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.tarul.cn/Article/details/gsgypjeyp.sHtML

[Q79] 字符串拼接
来源：http://wap.vehdjk.com/Article/details/gwiudzpyo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.epnwcf.com/Article/details/gbduqdyas.sHtML

[Q80] 字符串截取
来源：http://www.m.share.bbcook.cn/Article/details/glhevqzqr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.epnwcf.com/Article/details/giikjjsbc.sHtML

[Q81] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/guiuwafze.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.yfazqb.com/Article/details/gnayjqecf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.sjlbkw.cn/Article/details/gqcbkciwl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gxfwcgurk.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gzomlguyb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gnuarsbin.sHtML

[Q84] 去除首尾空格
来源：http://mobile.sjlbkw.cn/Article/details/gfydperdh.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gsnxkyrnr.sHtML

[Q85] 数值取整
来源：http://wap.epnwcf.com/Article/details/ghsxswlpe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.yfazqb.com/Article/details/guhjdumvx.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.yfazqb.com/Article/details/gxhxzdxzi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/gcdijnklb.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.bbcook.cn/Article/details/gwuqsywxd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fktsv.cn/Article/details/gtiqntosq.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.tarul.cn/Article/details/gtjfuhbey.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fktsv.cn/Article/details/gruyoqplk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.vehdjk.com/Article/details/gpikbitay.sHtML

[Q89] 判断表是否存在
来源：http://read.share.tarul.cn/Article/details/gxvnashos.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.bbcook.cn/Article/details/gdpoayvgx.sHtML

[Q90] 生成序号列
来源：http://www.blog.yfazqb.com/Article/details/gkgzwunni.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.tarul.cn/Article/details/gwycjqspx.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gtuedabbe.sHtML

R. Bash 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpcpsqmn.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmfmlfffi.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.yfazqb.com/Article/details/grxmojcts.sHtML

#!/usr/bin/env bash
来源：http://m.share.epnwcf.com/Article/details/gdjtjnkpl.sHtML

set -euo pipefail
来源：http://www.blog.tarul.cn/Article/details/gzsdgczhx.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.tarul.cn/Article/details/gbqargahw.sHtML

name="Tom"; echo "$name"
来源：http://baike.yfazqb.com/Article/details/gizkvtqln.sHtML

[R03] 只读变量
来源：http://baike.fktsv.cn/Article/details/gogaqkize.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/glwduwvfb.sHtML

[R04] 位置参数
来源：http://wap.bbcook.cn/Article/details/grimqewiy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.vehdjk.com/Article/details/gayvwllzk.sHtML

[R05] 参数默认值
来源：http://m.share.fktsv.cn/Article/details/gikrfpodc.sHtML

name="${1:-default}"
来源：http://www.blog.bbcook.cn/Article/details/gmwonikxn.sHtML

[R06] 判断命令是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gfbsgghdw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.epnwcf.com/Article/details/grlhzfimd.sHtML

[R07] if 判断文件
来源：http://wap.tarul.cn/Article/details/ghlqedvjc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.yfazqb.com/Article/details/geqbzoebc.sHtML

[R08] 数值比较
来源：http://read.share.fktsv.cn/Article/details/gfqijqlwm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.vehdjk.com/Article/details/gcalchyxt.sHtML

[R09] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gvzvxiomx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.sjlbkw.cn/Article/details/gcwnuyuys.sHtML

[R10] 正则匹配
来源：http://wap.vehdjk.com/Article/details/gnnbostrj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.tarul.cn/Article/details/gghfaxjzm.sHtML

[R11] case 多分支
来源：http://mobile.yfazqb.com/Article/details/gletptemn.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/gurtvomww.sHtML

start) echo "启动" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gnpabpngv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.vehdjk.com/Article/details/gcwlmrsvg.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gigedpspa.sHtML

esac
来源：http://3g.vehdjk.com/Article/details/gplsndgpb.sHtML

[R12] for 遍历文件
来源：http://3g.bbcook.cn/Article/details/glsorhtlq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fktsv.cn/Article/details/getwgjtae.sHtML

[R13] for 计数循环
来源：http://wap.tarul.cn/Article/details/gjngppgdb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gggjbqsln.sHtML

[R14] C 风格 for
来源：http://www.m.share.vehdjk.com/Article/details/gepfurwce.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/gxdqxofog.sHtML

[R15] while 逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gzfudcvda.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.epnwcf.com/Article/details/gpsdqtwlb.sHtML

[R16] until 等待条件
来源：http://www.blog.vehdjk.com/Article/details/gvdrdgnnp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/gfjeknjfq.sHtML

[R17] 数组定义与取值
来源：http://www.blog.epnwcf.com/Article/details/gkgcxqgky.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.tarul.cn/Article/details/glxtvmmon.sHtML

[R18] 遍历数组
来源：http://wap.yfazqb.com/Article/details/gncrtpgfc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/giekjtyuz.sHtML

[R19] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/guegujgru.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fktsv.cn/Article/details/gcvcdjyzc.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fktsv.cn/Article/details/gxkmhuuzj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.tarul.cn/Article/details/gjwdarjdm.sHtML

[R21] 字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gxtnbtjvz.sHtML

echo "${#s}"
来源：http://www.blog.vehdjk.com/Article/details/gqlcgpclj.sHtML

[R22] 截取子串
来源：http://www.share.vehdjk.com/Article/details/ghqnbuuvp.sHtML

echo "${s:0:5}"
来源：http://blog.vehdjk.com/Article/details/gpjykugyw.sHtML

[R23] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gmteqmngp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.vehdjk.com/Article/details/gtxuprohx.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gitnilbvl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fktsv.cn/Article/details/gjrfpbnrc.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.sjlbkw.cn/Article/details/gtzdwigpc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.vehdjk.com/Article/details/gnakpgtau.sHtML

[R26] 命令替换
来源：http://www.share.epnwcf.com/Article/details/gyxishqfp.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fktsv.cn/Article/details/gmncbxfsx.sHtML

[R27] 算术展开
来源：http://www.m.share.vehdjk.com/Article/details/gxuegcyyq.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.sjlbkw.cn/Article/details/giuupaviq.sHtML

[R28] 浮点运算
来源：http://read.share.sjlbkw.cn/Article/details/gcuicjhec.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fktsv.cn/Article/details/gtyzrctsh.sHtML

[R29] 定义函数
来源：http://blog.tarul.cn/Article/details/gjbqonofi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.sjlbkw.cn/Article/details/gqnwweytu.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gwxjjeaij.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.vehdjk.com/Article/details/gulxtinvm.sHtML

[R31] 局部变量
来源：http://wap.bbcook.cn/Article/details/gwkzgfebx.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.yfazqb.com/Article/details/gofoxixwx.sHtML

[R32] 参数个数校验
来源：http://wap.bbcook.cn/Article/details/ghwibmlpa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/glbsphqdq.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.tarul.cn/Article/details/gfeduhwyt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.bbcook.cn/Article/details/ghybqvpob.sHtML

[R34] 退出时清理
来源：http://mobile.sjlbkw.cn/Article/details/gfxyfztiz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fktsv.cn/Article/details/gqhgkbisx.sHtML

[R35] 后台执行并等待
来源：http://mobile.fktsv.cn/Article/details/gbqranahz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.epnwcf.com/Article/details/gvkjkyetl.sHtML

[R36] 并发执行多个任务
来源：http://mobile.vehdjk.com/Article/details/gfepbjhtj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.epnwcf.com/Article/details/goxsmfzxj.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.epnwcf.com/Article/details/gqrsitczy.sHtML

files=$(ls -1)
来源：http://blog.epnwcf.com/Article/details/gmqqkefht.sHtML

[R38] 管道串联
来源：http://read.share.vehdjk.com/Article/details/guvvhoejb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.vehdjk.com/Article/details/gcvxeitwj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.tarul.cn/Article/details/glmfkeimf.sHtML

cmd > out.log 2>&1
来源：http://blog.sjlbkw.cn/Article/details/gfqpoweew.sHtML

[R40] 追加写日志
来源：http://blog.fktsv.cn/Article/details/gbjvefzhj.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/gesczabme.sHtML

[R41] 丢弃输出
来源：http://blog.bbcook.cn/Article/details/gntmfmbxg.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/gndfouxit.sHtML

[R42] 输入重定向
来源：http://www.blog.epnwcf.com/Article/details/gwaqumpaj.sHtML

wc -l < a.txt
来源：http://m.share.yfazqb.com/Article/details/graxvcpsu.sHtML

[R43] 按名字查找文件
来源：http://m.share.bbcook.cn/Article/details/gqysbcged.sHtML

find . -name "*.log" -type f
来源：http://www.share.yfazqb.com/Article/details/gvgrqlnzf.sHtML

[R44] 按修改时间查找
来源：http://3g.yfazqb.com/Article/details/gfepihqfh.sHtML

find . -mtime -7 -type f
来源：http://wap.epnwcf.com/Article/details/galchceld.sHtML

[R45] 批量删除
来源：http://www.blog.sjlbkw.cn/Article/details/ggbnhlwwo.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fktsv.cn/Article/details/grysvqpnz.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fktsv.cn/Article/details/gvcppbbod.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.yfazqb.com/Article/details/gestamsxk.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/gsjwkecvg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gymcquxlm.sHtML

[R48] awk 取指定列
来源：http://mobile.tarul.cn/Article/details/grzsgaljb.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gzadrhvms.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gtzghvvuq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.sjlbkw.cn/Article/details/gbvuccugv.sHtML

[R50] awk 求和
来源：http://blog.epnwcf.com/Article/details/gudbdotum.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gdhhgwloo.sHtML

[R51] 排序去重取前几
来源：http://blog.fktsv.cn/Article/details/gubuqlcax.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.yfazqb.com/Article/details/gydcgcsyf.sHtML

[R52] 统计行数
来源：http://read.share.bbcook.cn/Article/details/gaveclnqh.sHtML

wc -l a.txt
来源：http://mobile.tarul.cn/Article/details/gbfcmcmob.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.epnwcf.com/Article/details/gdayeltki.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fktsv.cn/Article/details/gwecrqeuv.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/gsbtcsrps.sHtML

diff a.txt b.txt
来源：http://baike.tarul.cn/Article/details/gfkwrdkhm.sHtML

[R55] 压缩与解压
来源：http://3g.epnwcf.com/Article/details/gvqbsjztz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.epnwcf.com/Article/details/gkpnodbfz.sHtML

[R56] 远程拷贝
来源：http://read.share.bbcook.cn/Article/details/gfdvxjcpw.sHtML

scp file user@host:/path/
来源：http://blog.tarul.cn/Article/details/ggkrklivl.sHtML

[R57] 远程执行命令
来源：http://www.m.share.vehdjk.com/Article/details/gqcxrvmnt.sHtML

ssh user@host 'uptime'
来源：http://www.blog.yfazqb.com/Article/details/gbcknyuuw.sHtML

[R58] 下载文件
来源：http://blog.vehdjk.com/Article/details/gttrsuhwl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fktsv.cn/Article/details/gxrzfmbff.sHtML

[R59] 发 POST JSON
来源：http://baike.tarul.cn/Article/details/grteycmxx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fktsv.cn/Article/details/gokhnzfvg.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/glddrqekx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/gbhuafcri.sHtML

[R61] 磁盘占用
来源：http://baike.bbcook.cn/Article/details/gqoizwajk.sHtML

df -h;  du -sh *
来源：http://3g.epnwcf.com/Article/details/gpmwmkaak.sHtML

[R62] 找最占空间的文件
来源：http://read.share.yfazqb.com/Article/details/gldiynxte.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.bbcook.cn/Article/details/gfraqwxiy.sHtML

[R63] 内存与进程
来源：http://wap.epnwcf.com/Article/details/gvjkhfans.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.bbcook.cn/Article/details/gqwivigne.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/gnciovaeo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.yfazqb.com/Article/details/gydwzsjwt.sHtML

[R65] 查看端口占用
来源：http://3g.fktsv.cn/Article/details/gjqwrqdrs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.yfazqb.com/Article/details/gsrlgycss.sHtML

[R66] 定时任务
来源：http://baike.fktsv.cn/Article/details/gbjqeimmw.sHtML

crontab -e;  crontab -l
来源：http://mobile.tarul.cn/Article/details/gelkgewmt.sHtML

[R67] 生成随机十六进制串
来源：http://baike.bbcook.cn/Article/details/gvimafzkp.sHtML

openssl rand -hex 16
来源：http://blog.fktsv.cn/Article/details/gotfaemef.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fktsv.cn/Article/details/gcpvjwcyx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.vehdjk.com/Article/details/glbhljhxw.sHtML

[R69] 生成随机密码
来源：http://www.share.fktsv.cn/Article/details/gdbweilcc.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/geigsxmkt.sHtML

[R70] 时间戳与互转
来源：http://www.share.tarul.cn/Article/details/ghburnagv.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.yfazqb.com/Article/details/gdqxuixos.sHtML

[R71] 日期格式化
来源：http://read.share.fktsv.cn/Article/details/gyvferiml.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.yfazqb.com/Article/details/gizmdrjvv.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/guyfqfonm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/gnltsuwym.sHtML

[R73] 分割大日志
来源：http://mobile.bbcook.cn/Article/details/gapcpmgkd.sHtML

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/gswxjjpkm.sHtML

[R74] 批量重命名
来源：http://blog.sjlbkw.cn/Article/details/ggynokonz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.sjlbkw.cn/Article/details/gjbutsuxn.sHtML

[R75] 导出环境变量
来源：http://wap.tarul.cn/Article/details/ggukkpboi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.vehdjk.com/Article/details/gmpronimd.sHtML

[R76] 使用临时文件
来源：http://read.share.tarul.cn/Article/details/gemijwqoc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gefxcgudv.sHtML

[R77] 读取用户输入
来源：http://read.share.vehdjk.com/Article/details/guejirmfb.sHtML

read -rp "请输入: " ans
来源：http://3g.epnwcf.com/Article/details/gfhxrxmxt.sHtML

[R78] 交互式菜单
来源：http://mobile.yfazqb.com/Article/details/glpsxzfmb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.vehdjk.com/Article/details/giqckdich.sHtML

[R79] 解析命令行选项
来源：http://www.blog.tarul.cn/Article/details/gfkticxdg.sHtML


<!-- 参考信息 -->