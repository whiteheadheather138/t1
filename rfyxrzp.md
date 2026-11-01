代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fktsv.cn/Article/details/gsenllsys.sHtML

[Q28] 求和与平均
来源：http://baike.bbcook.cn/Article/details/gogqdwypl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gkffwnoqr.sHtML

[Q29] 最大最小值
来源：http://wap.yfazqb.com/Article/details/gpgvweliw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gvyyyakim.sHtML

[Q30] 分组统计
来源：http://blog.fktsv.cn/Article/details/ghpuibkfv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gmlbbdqvt.sHtML

[Q31] 分组后过滤
来源：http://3g.vehdjk.com/Article/details/graswebde.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.bbcook.cn/Article/details/gspymsvzw.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.tarul.cn/Article/details/gyllpxyac.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/glaqedquq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.bbcook.cn/Article/details/gfgmqyivu.sHtML

[Q33] 多列分组
来源：http://www.share.vehdjk.com/Article/details/gejklwreq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.yfazqb.com/Article/details/ggnrqeloq.sHtML

[Q34] 每组取第一条
来源：http://blog.bbcook.cn/Article/details/gdonulmsj.sHtML

SELECT * FROM (
来源：http://baike.bbcook.cn/Article/details/guemlgaix.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.epnwcf.com/Article/details/gnrpvzdpj.sHtML

) t WHERE rn = 1;
来源：http://read.share.vehdjk.com/Article/details/gfyhharhg.sHtML

[Q35] 内连接
来源：http://www.m.share.bbcook.cn/Article/details/gexbmpatz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gozpuksqo.sHtML

[Q36] 左连接
来源：http://www.share.epnwcf.com/Article/details/gkuvuvuhm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/gzhincosh.sHtML

[Q37] 右连接
来源：http://read.share.epnwcf.com/Article/details/gzyfeyfjk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.bbcook.cn/Article/details/gauytqvzg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.epnwcf.com/Article/details/ggmtjemzt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.vehdjk.com/Article/details/gvujabhaf.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.bbcook.cn/Article/details/gxtkzblfx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/guyxqsfce.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gxdpqmntw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.yfazqb.com/Article/details/gqlkddmtm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fktsv.cn/Article/details/guranqmmq.sHtML

[Q41] 多表连接
来源：http://www.m.share.tarul.cn/Article/details/gugrjqwrs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fktsv.cn/Article/details/glpeaujzt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.vehdjk.com/Article/details/ghclcooys.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.tarul.cn/Article/details/gyxjkqxus.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fktsv.cn/Article/details/ggceqdhod.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.sjlbkw.cn/Article/details/gqnfyqufc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.yfazqb.com/Article/details/gtnskfdkd.sHtML

[Q43] 标量子查询
来源：http://www.share.tarul.cn/Article/details/gwdoudvne.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fktsv.cn/Article/details/gtlaeclqb.sHtML

[Q44] IN 子查询
来源：http://www.blog.fktsv.cn/Article/details/gatudqbhj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.bbcook.cn/Article/details/grnjcbkse.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.sjlbkw.cn/Article/details/gpwwhbpcy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/gtimcxegq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.vehdjk.com/Article/details/gfxxutqsk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.bbcook.cn/Article/details/gkjtzfegf.sHtML

[Q47] 与平均值比较
来源：http://blog.sjlbkw.cn/Article/details/gqcyeurve.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.vehdjk.com/Article/details/gkpjrnbau.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.tarul.cn/Article/details/gpwpfwpfg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnfaoxik.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.tarul.cn/Article/details/gcqazykkx.sHtML

[Q49] 更新单行
来源：http://wap.sjlbkw.cn/Article/details/gorlqdrht.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/grbjfmwei.sHtML

[Q50] 批量更新
来源：http://m.share.yfazqb.com/Article/details/gkpxsiegw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.yfazqb.com/Article/details/grpxryrib.sHtML

[Q51] 用子查询更新
来源：http://baike.sjlbkw.cn/Article/details/glwoaeonw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.vehdjk.com/Article/details/gacjydyqf.sHtML

[Q52] 删除指定行
来源：http://wap.epnwcf.com/Article/details/gqetwgjys.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.tarul.cn/Article/details/genusxvkp.sHtML

[Q53] 按条件删除
来源：http://www.blog.sjlbkw.cn/Article/details/gsnnrkger.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.bbcook.cn/Article/details/gluvqnsgc.sHtML

[Q54] 清空表
来源：http://baike.yfazqb.com/Article/details/gacfntrgj.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.yfazqb.com/Article/details/gvrbjsvnp.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.epnwcf.com/Article/details/gxqvmrcun.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.yfazqb.com/Article/details/gwflifizm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.sjlbkw.cn/Article/details/grhfbfgtd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.tarul.cn/Article/details/gfksrcuxx.sHtML

[Q57] 行号
来源：http://read.share.bbcook.cn/Article/details/gsrweyceg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.tarul.cn/Article/details/gwsurnuci.sHtML

[Q58] 累计求和
来源：http://www.share.epnwcf.com/Article/details/giwmuekfm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gibjagqix.sHtML

[Q59] 分组内累计
来源：http://wap.epnwcf.com/Article/details/gspgvzojf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/ghcycmkud.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.bbcook.cn/Article/details/gtsrhivue.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.bbcook.cn/Article/details/gpixrnknu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.epnwcf.com/Article/details/ggfwunbqv.sHtML

[Q61] 移动平均
来源：http://www.blog.epnwcf.com/Article/details/gwmuttmpb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gsarnofum.sHtML

[Q62] 分组占比
来源：http://read.share.vehdjk.com/Article/details/gztcdetkz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/ggjohcsig.sHtML

[Q63] 开启事务
来源：http://www.m.share.fktsv.cn/Article/details/gkcfwokxb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.sjlbkw.cn/Article/details/gzakulcof.sHtML

[Q64] 提交事务
来源：http://mobile.yfazqb.com/Article/details/gqztkythn.sHtML

COMMIT;
来源：http://mobile.fktsv.cn/Article/details/gspzzbewq.sHtML

[Q65] 回滚事务
来源：http://baike.epnwcf.com/Article/details/gnnwachin.sHtML

ROLLBACK;
来源：http://www.m.share.epnwcf.com/Article/details/gsicacifx.sHtML

[Q66] 行锁查询
来源：http://www.share.fktsv.cn/Article/details/gbmawqwct.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.epnwcf.com/Article/details/gjeznhlmi.sHtML

[Q67] 设置隔离级别
来源：http://mobile.sjlbkw.cn/Article/details/gvhemeboj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.sjlbkw.cn/Article/details/gzndpognr.sHtML

[Q68] 保存点
来源：http://3g.tarul.cn/Article/details/gjlchcult.sHtML

SAVEPOINT sp1;
来源：http://wap.fktsv.cn/Article/details/ghcqqfnau.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fktsv.cn/Article/details/gquezyihb.sHtML

[Q69] 查看执行计划
来源：http://www.share.tarul.cn/Article/details/gkyvlauwt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fktsv.cn/Article/details/gqvdshmgu.sHtML

[Q70] 更新统计信息
来源：http://mobile.yfazqb.com/Article/details/gohdccndz.sHtML

ANALYZE TABLE users;
来源：http://blog.vehdjk.com/Article/details/gvvczxjjo.sHtML

[Q71] 查看建表语句
来源：http://www.share.sjlbkw.cn/Article/details/gpoekdseq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.tarul.cn/Article/details/gvngqryxi.sHtML

[Q72] 查看索引
来源：http://read.share.bbcook.cn/Article/details/gvyoxjgfh.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/ggfffvnbr.sHtML

[Q73] 查看表状态
来源：http://blog.fktsv.cn/Article/details/gjbldomag.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.yfazqb.com/Article/details/gsyxeezqh.sHtML

[Q74] 强制使用索引
来源：http://mobile.vehdjk.com/Article/details/geqzeilby.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.epnwcf.com/Article/details/ggnpqnaxu.sHtML

[Q75] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gwohgosks.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.yfazqb.com/Article/details/giiebzoxh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.vehdjk.com/Article/details/gymmbrbkm.sHtML

[Q76] 按天统计
来源：http://wap.fktsv.cn/Article/details/gbuihkkbb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fktsv.cn/Article/details/gpwizwvwr.sHtML

[Q77] 时间加减
来源：http://www.blog.yfazqb.com/Article/details/gvhvymwgr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fktsv.cn/Article/details/gixgvntzr.sHtML

[Q78] 当前时间
来源：http://read.share.epnwcf.com/Article/details/gglyldyxo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.bbcook.cn/Article/details/geenbyxdh.sHtML

[Q79] 字符串拼接
来源：http://www.blog.tarul.cn/Article/details/gnidpcwlu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.epnwcf.com/Article/details/gzewhouzd.sHtML

[Q80] 字符串截取
来源：http://www.share.bbcook.cn/Article/details/gkaqgcqjk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/giqmngfrq.sHtML

[Q81] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/ggwobvgvb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.sjlbkw.cn/Article/details/glsagvrmm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.vehdjk.com/Article/details/gneumoqes.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gycqhzptr.sHtML

[Q83] 大小写转换
来源：http://3g.epnwcf.com/Article/details/gzufzgonb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gyzcqoybx.sHtML

[Q84] 去除首尾空格
来源：http://www.share.yfazqb.com/Article/details/gjftfwomm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gersaqgvl.sHtML

[Q85] 数值取整
来源：http://m.share.fktsv.cn/Article/details/gswovfvqn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.bbcook.cn/Article/details/greorqipw.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fktsv.cn/Article/details/guvmsjxvh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.vehdjk.com/Article/details/gkcytinuk.sHtML

[Q87] JSON 字段做条件
来源：http://baike.yfazqb.com/Article/details/gmotpavka.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.yfazqb.com/Article/details/gvejqrpvo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.tarul.cn/Article/details/gyoctalkd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.yfazqb.com/Article/details/gmzukgavw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.yfazqb.com/Article/details/gwqmqkglz.sHtML

[Q89] 判断表是否存在
来源：http://read.share.tarul.cn/Article/details/gcjvrjvsv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.yfazqb.com/Article/details/gtqdaqdkn.sHtML

[Q90] 生成序号列
来源：http://wap.bbcook.cn/Article/details/gmjtusmxs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fktsv.cn/Article/details/gasfuyzxn.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkbqezxku.sHtML

R. Bash 专题
来源：http://www.share.yfazqb.com/Article/details/guvbwkeer.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gfqsgdfws.sHtML

[R01] shebang 与严格模式
来源：http://wap.epnwcf.com/Article/details/gzbzxdhap.sHtML

#!/usr/bin/env bash
来源：http://read.share.yfazqb.com/Article/details/gdvlxeytr.sHtML

set -euo pipefail
来源：http://3g.epnwcf.com/Article/details/gfminudro.sHtML

[R02] 变量赋值与使用
来源：http://wap.sjlbkw.cn/Article/details/gbvuwbajl.sHtML

name="Tom"; echo "$name"
来源：http://read.share.tarul.cn/Article/details/gwgypktgc.sHtML

[R03] 只读变量
来源：http://www.m.share.fktsv.cn/Article/details/goocrhtpr.sHtML

readonly PI=3.14
来源：http://www.share.tarul.cn/Article/details/gfhgpqjak.sHtML

[R04] 位置参数
来源：http://mobile.epnwcf.com/Article/details/guninmbcg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.bbcook.cn/Article/details/gymkstoil.sHtML

[R05] 参数默认值
来源：http://read.share.epnwcf.com/Article/details/guykbtbez.sHtML

name="${1:-default}"
来源：http://m.share.fktsv.cn/Article/details/gjkodysmw.sHtML

[R06] 判断命令是否存在
来源：http://3g.epnwcf.com/Article/details/gloolwadz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gvqxxqgun.sHtML

[R07] if 判断文件
来源：http://read.share.yfazqb.com/Article/details/gckjjbnly.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gkxpymgor.sHtML

[R08] 数值比较
来源：http://www.m.share.fktsv.cn/Article/details/ghuoxyouw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gdtkgrpqd.sHtML

[R09] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/grxgunwfd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.bbcook.cn/Article/details/grtkrzlof.sHtML

[R10] 正则匹配
来源：http://www.share.tarul.cn/Article/details/gxybdfrgl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.yfazqb.com/Article/details/gkrldqkzh.sHtML

[R11] case 多分支
来源：http://m.share.epnwcf.com/Article/details/gqyixrmrw.sHtML

case "$1" in
来源：http://blog.vehdjk.com/Article/details/gndopcfxa.sHtML

start) echo "启动" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gulnmqoyw.sHtML

stop)  echo "停止" ;;
来源：http://mobile.bbcook.cn/Article/details/gimhlfifj.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.vehdjk.com/Article/details/glggcebms.sHtML

esac
来源：http://mobile.tarul.cn/Article/details/gszhdsfkc.sHtML

[R12] for 遍历文件
来源：http://baike.bbcook.cn/Article/details/grgdufsai.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.tarul.cn/Article/details/gzaauwpiz.sHtML

[R13] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gotnqlhir.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gwqdcqfyp.sHtML

[R14] C 风格 for
来源：http://blog.fktsv.cn/Article/details/gvffmbjvv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gqlaipnqh.sHtML

[R15] while 逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/glquisqvq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.bbcook.cn/Article/details/gukflzsid.sHtML

[R16] until 等待条件
来源：http://blog.fktsv.cn/Article/details/gyigjletg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gobgnnafj.sHtML

[R17] 数组定义与取值
来源：http://mobile.yfazqb.com/Article/details/gepjnqtqm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.yfazqb.com/Article/details/gvyvskucj.sHtML

[R18] 遍历数组
来源：http://www.blog.epnwcf.com/Article/details/gxoecthrj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.epnwcf.com/Article/details/ggxwietui.sHtML

[R19] 数组长度
来源：http://m.share.vehdjk.com/Article/details/gpmclelvx.sHtML

echo "${#arr[@]}"
来源：http://wap.tarul.cn/Article/details/gzczedfjq.sHtML

[R20] 关联数组（字典）
来源：http://read.share.vehdjk.com/Article/details/gqxzpuzfs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.bbcook.cn/Article/details/gmdhdzhmp.sHtML

[R21] 字符串长度
来源：http://blog.tarul.cn/Article/details/gcwzfzjqq.sHtML

echo "${#s}"
来源：http://www.m.share.epnwcf.com/Article/details/gppuaftov.sHtML

[R22] 截取子串
来源：http://blog.epnwcf.com/Article/details/gkvtfyncs.sHtML

echo "${s:0:5}"
来源：http://baike.sjlbkw.cn/Article/details/gmwyrjoyq.sHtML

[R23] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/glccmaxli.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.bbcook.cn/Article/details/guxtzjsxj.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/guuoouicl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.tarul.cn/Article/details/gvkmtgyxr.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.epnwcf.com/Article/details/gmjimbohk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.bbcook.cn/Article/details/gdztzmsuy.sHtML

[R26] 命令替换
来源：http://wap.epnwcf.com/Article/details/gpwqzroen.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwgspnos.sHtML

[R27] 算术展开
来源：http://wap.epnwcf.com/Article/details/gkrnhbmjb.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fktsv.cn/Article/details/gicqnoovw.sHtML

[R28] 浮点运算
来源：http://mobile.sjlbkw.cn/Article/details/gpezsykeb.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/gtgsqgglm.sHtML

[R29] 定义函数
来源：http://baike.tarul.cn/Article/details/glzedmdsc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.bbcook.cn/Article/details/gjqdzmona.sHtML

[R30] 函数返回状态码
来源：http://mobile.bbcook.cn/Article/details/gbinzypwe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.yfazqb.com/Article/details/gypmymebq.sHtML

[R31] 局部变量
来源：http://read.share.vehdjk.com/Article/details/gmegnwgui.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.bbcook.cn/Article/details/gfgpiesdw.sHtML

[R32] 参数个数校验
来源：http://baike.bbcook.cn/Article/details/gkbyjeffk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gbsfieqrj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.tarul.cn/Article/details/gskwesbwn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhijodxf.sHtML

[R34] 退出时清理
来源：http://wap.fktsv.cn/Article/details/gqturgkvu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gxsyyogil.sHtML

[R35] 后台执行并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gzfgjgjau.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.yfazqb.com/Article/details/gkzgstrwz.sHtML

[R36] 并发执行多个任务
来源：http://blog.tarul.cn/Article/details/gpdiwqpkp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/gcxnfvvul.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.yfazqb.com/Article/details/gfkzgfuyc.sHtML

files=$(ls -1)
来源：http://blog.vehdjk.com/Article/details/gvzaxzdml.sHtML

[R38] 管道串联
来源：http://blog.tarul.cn/Article/details/grhawiptt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.bbcook.cn/Article/details/gzqnozuux.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/gyyzgsbqu.sHtML

cmd > out.log 2>&1
来源：http://3g.fktsv.cn/Article/details/gvfczvzyp.sHtML

[R40] 追加写日志
来源：http://3g.vehdjk.com/Article/details/gaaxkdxpk.sHtML

echo "log" >> out.log
来源：http://baike.yfazqb.com/Article/details/gjktqldub.sHtML

[R41] 丢弃输出
来源：http://www.blog.yfazqb.com/Article/details/gfiygqxtj.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/ghsfpvjfh.sHtML

[R42] 输入重定向
来源：http://www.share.sjlbkw.cn/Article/details/glyoakyfs.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/ghfldqbhl.sHtML

[R43] 按名字查找文件
来源：http://blog.epnwcf.com/Article/details/gxkcuckyt.sHtML

find . -name "*.log" -type f
来源：http://3g.fktsv.cn/Article/details/glussmbia.sHtML

[R44] 按修改时间查找
来源：http://www.share.yfazqb.com/Article/details/gzyvxqher.sHtML

find . -mtime -7 -type f
来源：http://baike.fktsv.cn/Article/details/gflwddush.sHtML

[R45] 批量删除
来源：http://m.share.yfazqb.com/Article/details/gugxmzhin.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.epnwcf.com/Article/details/ghwwziewr.sHtML

[R46] 递归替换文件内容
来源：http://baike.yfazqb.com/Article/details/gabceybju.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fktsv.cn/Article/details/gwbahrjoa.sHtML

[R47] sed 单行替换
来源：http://mobile.sjlbkw.cn/Article/details/gkyndxrek.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fktsv.cn/Article/details/gxxfhcpay.sHtML

[R48] awk 取指定列
来源：http://www.blog.epnwcf.com/Article/details/gvssvjizf.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.yfazqb.com/Article/details/gzdslrrdf.sHtML

[R49] awk 带条件
来源：http://read.share.tarul.cn/Article/details/glcfdvoxy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.vehdjk.com/Article/details/gudkvrvii.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/gkmpldyyn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.tarul.cn/Article/details/gmffgwkeb.sHtML

[R51] 排序去重取前几
来源：http://wap.yfazqb.com/Article/details/giwtwonak.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.vehdjk.com/Article/details/guzjskhtb.sHtML

[R52] 统计行数
来源：http://www.share.bbcook.cn/Article/details/gxfcrfojr.sHtML

wc -l a.txt
来源：http://read.share.fktsv.cn/Article/details/genxmstgz.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.bbcook.cn/Article/details/gqhtfncot.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.epnwcf.com/Article/details/ghanzspry.sHtML

[R54] 比较两个文件
来源：http://blog.sjlbkw.cn/Article/details/gstskmhjg.sHtML

diff a.txt b.txt
来源：http://www.share.bbcook.cn/Article/details/gfykzuzws.sHtML

[R55] 压缩与解压
来源：http://blog.tarul.cn/Article/details/gpplhdklx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.vehdjk.com/Article/details/gygoeyvah.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gyjsabsnv.sHtML

scp file user@host:/path/
来源：http://mobile.sjlbkw.cn/Article/details/gkgxjghih.sHtML

[R57] 远程执行命令
来源：http://mobile.bbcook.cn/Article/details/gihojohmq.sHtML

ssh user@host 'uptime'
来源：http://baike.yfazqb.com/Article/details/ghwiwaiku.sHtML

[R58] 下载文件
来源：http://m.share.tarul.cn/Article/details/gpyyixzsn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.epnwcf.com/Article/details/gnljuxbwr.sHtML

[R59] 发 POST JSON
来源：http://www.share.tarul.cn/Article/details/gcygrjbbi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/gmkokdega.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/gompzvsem.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fktsv.cn/Article/details/gwfckvkyh.sHtML

[R61] 磁盘占用
来源：http://m.share.vehdjk.com/Article/details/gpcwkozpe.sHtML

df -h;  du -sh *
来源：http://read.share.epnwcf.com/Article/details/gxivxtmht.sHtML

[R62] 找最占空间的文件
来源：http://read.share.bbcook.cn/Article/details/gxfhztdya.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fktsv.cn/Article/details/ggwnyyiwb.sHtML

[R63] 内存与进程
来源：http://baike.sjlbkw.cn/Article/details/gqgnfyrfb.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.epnwcf.com/Article/details/ginwcpnzo.sHtML

[R64] 结束进程
来源：http://www.share.epnwcf.com/Article/details/gibswcmrq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.tarul.cn/Article/details/gobrlttao.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fktsv.cn/Article/details/gvudhmgbb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.tarul.cn/Article/details/gnmjtduar.sHtML

[R66] 定时任务
来源：http://wap.sjlbkw.cn/Article/details/ghvktelzv.sHtML

crontab -e;  crontab -l
来源：http://baike.epnwcf.com/Article/details/gbwizqnqu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.bbcook.cn/Article/details/geekhhveh.sHtML

openssl rand -hex 16
来源：http://mobile.vehdjk.com/Article/details/gvhabnsru.sHtML

[R68] 计算文件校验值
来源：http://mobile.tarul.cn/Article/details/gkntbofrh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/gnbnbhitj.sHtML

[R69] 生成随机密码
来源：http://www.share.bbcook.cn/Article/details/gjlejtqof.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.yfazqb.com/Article/details/gqpxrijoc.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/goinxetgx.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/gkmnssgml.sHtML

[R71] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gwlxofozs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.tarul.cn/Article/details/gurcbibrb.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.epnwcf.com/Article/details/gqidihdmw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.tarul.cn/Article/details/gnfzmuoly.sHtML

[R73] 分割大日志
来源：http://www.blog.sjlbkw.cn/Article/details/gzopfmvpi.sHtML

split -l 1000 big.log part_
来源：http://m.share.epnwcf.com/Article/details/gtbcbjlqg.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/gewnbfsfq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.yfazqb.com/Article/details/gbgccojdm.sHtML

[R75] 导出环境变量
来源：http://www.share.tarul.cn/Article/details/gqlzmpmps.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.tarul.cn/Article/details/gqnskqplw.sHtML

[R76] 使用临时文件
来源：http://www.share.tarul.cn/Article/details/gpxbzzrhk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gnkshqhuw.sHtML

[R77] 读取用户输入
来源：http://www.share.yfazqb.com/Article/details/gppotvasc.sHtML


<!-- 参考信息 -->