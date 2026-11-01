代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gelfcroes.sHtML

[Q30] 分组统计
来源：http://wap.epnwcf.com/Article/details/glbvowsma.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/gxakcfjwm.sHtML

[Q31] 分组后过滤
来源：http://read.share.bbcook.cn/Article/details/glvpjzmke.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.vehdjk.com/Article/details/gzrrtejir.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gyinguvtm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gjzmtzncp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.sjlbkw.cn/Article/details/gsnijndzr.sHtML

[Q33] 多列分组
来源：http://3g.yfazqb.com/Article/details/gouotpyvq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.tarul.cn/Article/details/gpgcsdpov.sHtML

[Q34] 每组取第一条
来源：http://www.share.bbcook.cn/Article/details/gqoshnrtv.sHtML

SELECT * FROM (
来源：http://blog.epnwcf.com/Article/details/gaivxycpe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.bbcook.cn/Article/details/guzenxjww.sHtML

) t WHERE rn = 1;
来源：http://wap.tarul.cn/Article/details/gbezyivte.sHtML

[Q35] 内连接
来源：http://baike.vehdjk.com/Article/details/girwkhzyq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.sjlbkw.cn/Article/details/grdwqbeyl.sHtML

[Q36] 左连接
来源：http://m.share.sjlbkw.cn/Article/details/golndhccx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/gjpmtrhjf.sHtML

[Q37] 右连接
来源：http://mobile.tarul.cn/Article/details/goypomaiz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.yfazqb.com/Article/details/gvgwhwpeb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.tarul.cn/Article/details/gzstxnjnm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.bbcook.cn/Article/details/ginmaooap.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.yfazqb.com/Article/details/goskffwaf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.bbcook.cn/Article/details/ghhfmigop.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.bbcook.cn/Article/details/gmvaostkp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/gcvnbdkue.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.epnwcf.com/Article/details/gwxfowthw.sHtML

[Q41] 多表连接
来源：http://3g.epnwcf.com/Article/details/gftoxjivt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.vehdjk.com/Article/details/gexdctuub.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.yfazqb.com/Article/details/gselgzzky.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.sjlbkw.cn/Article/details/gwjmgwaqq.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.sjlbkw.cn/Article/details/gfkoiupvn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.epnwcf.com/Article/details/gygbqstwc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.tarul.cn/Article/details/ggfnbgtht.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/glpzuakfz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.vehdjk.com/Article/details/ghgeiupkd.sHtML

[Q44] IN 子查询
来源：http://wap.fktsv.cn/Article/details/grxavgsab.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.yfazqb.com/Article/details/gxnpghsgx.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.epnwcf.com/Article/details/gnswtjgyt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gtmtelhvn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.tarul.cn/Article/details/gwsvyrjtp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.epnwcf.com/Article/details/gckigrktl.sHtML

[Q47] 与平均值比较
来源：http://baike.yfazqb.com/Article/details/gmwgiwjpu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.epnwcf.com/Article/details/gqqbxpcmn.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.epnwcf.com/Article/details/gcvljebft.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.tarul.cn/Article/details/gcuaytpqr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.yfazqb.com/Article/details/giielxmwk.sHtML

[Q49] 更新单行
来源：http://wap.fktsv.cn/Article/details/guyjpcavg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.vehdjk.com/Article/details/gcdmtmftx.sHtML

[Q50] 批量更新
来源：http://wap.vehdjk.com/Article/details/guqipsbqo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.vehdjk.com/Article/details/gmwueumxx.sHtML

[Q51] 用子查询更新
来源：http://m.share.bbcook.cn/Article/details/gibeoyrgq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fktsv.cn/Article/details/gtlepzull.sHtML

[Q52] 删除指定行
来源：http://3g.bbcook.cn/Article/details/ggrnekcsp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.bbcook.cn/Article/details/grrhiivmu.sHtML

[Q53] 按条件删除
来源：http://blog.fktsv.cn/Article/details/gkgdsvxfc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.bbcook.cn/Article/details/gwgbbgxbx.sHtML

[Q54] 清空表
来源：http://read.share.yfazqb.com/Article/details/grvpqscrk.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fktsv.cn/Article/details/gxspsphcw.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.epnwcf.com/Article/details/gxkxwqlcm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.bbcook.cn/Article/details/ghlywgohp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fktsv.cn/Article/details/gxazkhszz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.vehdjk.com/Article/details/gzdgbyhmo.sHtML

[Q57] 行号
来源：http://www.blog.vehdjk.com/Article/details/gxcrkzysk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.tarul.cn/Article/details/gzzhjlbib.sHtML

[Q58] 累计求和
来源：http://m.share.bbcook.cn/Article/details/gbpiqxzyh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fktsv.cn/Article/details/ghxsplyva.sHtML

[Q59] 分组内累计
来源：http://3g.sjlbkw.cn/Article/details/grcpsfrpi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gvmczciyg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.sjlbkw.cn/Article/details/grythsieo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.tarul.cn/Article/details/gsqsbfcds.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fktsv.cn/Article/details/gytzoxrzn.sHtML

[Q61] 移动平均
来源：http://www.blog.yfazqb.com/Article/details/gvbgnrhov.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gqocsoata.sHtML

[Q62] 分组占比
来源：http://m.share.yfazqb.com/Article/details/gvfwabjhu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gwcnkragq.sHtML

[Q63] 开启事务
来源：http://read.share.vehdjk.com/Article/details/gcvvjhgth.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.yfazqb.com/Article/details/gwnjmdaxh.sHtML

[Q64] 提交事务
来源：http://read.share.tarul.cn/Article/details/gpfoxbrqe.sHtML

COMMIT;
来源：http://www.share.vehdjk.com/Article/details/gowrrwnci.sHtML

[Q65] 回滚事务
来源：http://m.share.bbcook.cn/Article/details/grlfmxzlh.sHtML

ROLLBACK;
来源：http://read.share.fktsv.cn/Article/details/gnvqxobfz.sHtML

[Q66] 行锁查询
来源：http://blog.yfazqb.com/Article/details/gldntkhqm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.vehdjk.com/Article/details/gmklanasj.sHtML

[Q67] 设置隔离级别
来源：http://blog.vehdjk.com/Article/details/gvbnimzfd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.tarul.cn/Article/details/gzeoyiack.sHtML

[Q68] 保存点
来源：http://mobile.tarul.cn/Article/details/gavdkvmfz.sHtML

SAVEPOINT sp1;
来源：http://read.share.vehdjk.com/Article/details/gitmjyptp.sHtML

ROLLBACK TO sp1;
来源：http://mobile.epnwcf.com/Article/details/gnkoglrze.sHtML

[Q69] 查看执行计划
来源：http://wap.fktsv.cn/Article/details/gcuomujpq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.yfazqb.com/Article/details/gqmxtvxhu.sHtML

[Q70] 更新统计信息
来源：http://m.share.tarul.cn/Article/details/gjrtegjxb.sHtML

ANALYZE TABLE users;
来源：http://wap.bbcook.cn/Article/details/gdrufebam.sHtML

[Q71] 查看建表语句
来源：http://read.share.vehdjk.com/Article/details/guusdegjx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.bbcook.cn/Article/details/gvpqezaua.sHtML

[Q72] 查看索引
来源：http://www.blog.epnwcf.com/Article/details/gflqcggdz.sHtML

SHOW INDEX FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gtdqvpbpi.sHtML

[Q73] 查看表状态
来源：http://www.m.share.yfazqb.com/Article/details/gqgtiluga.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fktsv.cn/Article/details/gmlmkvczi.sHtML

[Q74] 强制使用索引
来源：http://read.share.tarul.cn/Article/details/gbgbhdoea.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fktsv.cn/Article/details/gpeuefrsw.sHtML

[Q75] 日期格式化
来源：http://www.blog.vehdjk.com/Article/details/ghcnrsaqe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.tarul.cn/Article/details/gqlzoblqb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.sjlbkw.cn/Article/details/gjqmvwprz.sHtML

[Q76] 按天统计
来源：http://wap.fktsv.cn/Article/details/gujzirbct.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.bbcook.cn/Article/details/gikaouldj.sHtML

[Q77] 时间加减
来源：http://www.blog.vehdjk.com/Article/details/gwpokpppj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.vehdjk.com/Article/details/gmjqigfsp.sHtML

[Q78] 当前时间
来源：http://baike.tarul.cn/Article/details/gwscuccnz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fktsv.cn/Article/details/glmbyacyf.sHtML

[Q79] 字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/gcpngtqus.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.yfazqb.com/Article/details/gbrgkbddz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fktsv.cn/Article/details/gjshhedsx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.tarul.cn/Article/details/gudpbqttp.sHtML

[Q81] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/gnuhetbtm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.bbcook.cn/Article/details/gruyvmuaj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.yfazqb.com/Article/details/gklumoioj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gkauextmp.sHtML

[Q83] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/gsorugsrv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gyvqgzfdd.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fktsv.cn/Article/details/gzvzpnlpn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/grryqjnyb.sHtML

[Q85] 数值取整
来源：http://mobile.fktsv.cn/Article/details/gokwsmkku.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.yfazqb.com/Article/details/gerevtdiy.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.yfazqb.com/Article/details/gqlattwhk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.yfazqb.com/Article/details/gjlfrcjoq.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.epnwcf.com/Article/details/gikwraqgi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.tarul.cn/Article/details/ghsutrfxu.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.bbcook.cn/Article/details/gzuiipezm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.bbcook.cn/Article/details/guknfiofj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.epnwcf.com/Article/details/guovotpef.sHtML

[Q89] 判断表是否存在
来源：http://3g.fktsv.cn/Article/details/gtrafrxcp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.yfazqb.com/Article/details/gqeuswmhk.sHtML

[Q90] 生成序号列
来源：http://mobile.epnwcf.com/Article/details/gzloauhhv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/gyazjylkg.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ggrhcsyrd.sHtML

R. Bash 专题
来源：http://www.share.sjlbkw.cn/Article/details/gcgcdqgbg.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gogjrhlwe.sHtML

[R01] shebang 与严格模式
来源：http://www.share.vehdjk.com/Article/details/gvsdmhdqq.sHtML

#!/usr/bin/env bash
来源：http://read.share.sjlbkw.cn/Article/details/gyhsnqwmw.sHtML

set -euo pipefail
来源：http://www.blog.vehdjk.com/Article/details/ghytqpjek.sHtML

[R02] 变量赋值与使用
来源：http://blog.bbcook.cn/Article/details/gvpimtkzt.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.epnwcf.com/Article/details/gnofuepix.sHtML

[R03] 只读变量
来源：http://read.share.sjlbkw.cn/Article/details/gyzramezh.sHtML

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/grcdqztnq.sHtML

[R04] 位置参数
来源：http://read.share.yfazqb.com/Article/details/gktzvjkct.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.yfazqb.com/Article/details/glnlajgdb.sHtML

[R05] 参数默认值
来源：http://mobile.yfazqb.com/Article/details/gmndjhmiu.sHtML

name="${1:-default}"
来源：http://m.share.fktsv.cn/Article/details/gjdweuxox.sHtML

[R06] 判断命令是否存在
来源：http://3g.bbcook.cn/Article/details/gnjgbkvxb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gvlcumeku.sHtML

[R07] if 判断文件
来源：http://m.share.vehdjk.com/Article/details/gaxfyswyz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gpdyhdvau.sHtML

[R08] 数值比较
来源：http://wap.bbcook.cn/Article/details/gxqxuzewv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.vehdjk.com/Article/details/gkypguoyw.sHtML

[R09] 字符串比较
来源：http://www.blog.yfazqb.com/Article/details/glxgdcqpv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.sjlbkw.cn/Article/details/gqofoposn.sHtML

[R10] 正则匹配
来源：http://www.share.fktsv.cn/Article/details/ganvezvpb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.yfazqb.com/Article/details/gkbcikbsp.sHtML

[R11] case 多分支
来源：http://read.share.tarul.cn/Article/details/gokzaacym.sHtML

case "$1" in
来源：http://www.m.share.sjlbkw.cn/Article/details/gscuvmpqd.sHtML

start) echo "启动" ;;
来源：http://mobile.vehdjk.com/Article/details/gpugdkzqk.sHtML

stop)  echo "停止" ;;
来源：http://wap.epnwcf.com/Article/details/gvnryllia.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fktsv.cn/Article/details/ggngzjewy.sHtML

esac
来源：http://www.blog.epnwcf.com/Article/details/gtszbkabs.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/gucgpkkgn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.yfazqb.com/Article/details/ggnngcjcq.sHtML

[R13] for 计数循环
来源：http://blog.tarul.cn/Article/details/gljooqwer.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gdqxisyys.sHtML

[R14] C 风格 for
来源：http://wap.fktsv.cn/Article/details/gcchvytoa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gnwrtokrk.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gvkwkayol.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.yfazqb.com/Article/details/gdvcecyte.sHtML

[R16] until 等待条件
来源：http://mobile.bbcook.cn/Article/details/gwommhxbw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.yfazqb.com/Article/details/gwahjzvrz.sHtML

[R17] 数组定义与取值
来源：http://3g.vehdjk.com/Article/details/gngnipdvl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.yfazqb.com/Article/details/gxwnzydro.sHtML

[R18] 遍历数组
来源：http://www.m.share.bbcook.cn/Article/details/gebuwhhky.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.epnwcf.com/Article/details/gkafgpxnu.sHtML

[R19] 数组长度
来源：http://3g.tarul.cn/Article/details/gqixtespf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.yfazqb.com/Article/details/gjtngrsql.sHtML

[R20] 关联数组（字典）
来源：http://blog.yfazqb.com/Article/details/gvxvmpuys.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.bbcook.cn/Article/details/ghfuaxvjw.sHtML

[R21] 字符串长度
来源：http://read.share.epnwcf.com/Article/details/gwauvumyt.sHtML

echo "${#s}"
来源：http://www.share.yfazqb.com/Article/details/guwmqgudc.sHtML

[R22] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gykpdhxmf.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/glqkmdcra.sHtML

[R23] 字符串替换
来源：http://3g.bbcook.cn/Article/details/gpphmeamk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.vehdjk.com/Article/details/gwjlbukoz.sHtML

[R24] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gpoxkgpra.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.yfazqb.com/Article/details/grjlqbzlu.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.sjlbkw.cn/Article/details/gntokypqu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.yfazqb.com/Article/details/gflueqwnu.sHtML

[R26] 命令替换
来源：http://3g.epnwcf.com/Article/details/gwcrrgjit.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.sjlbkw.cn/Article/details/galarncyt.sHtML

[R27] 算术展开
来源：http://3g.fktsv.cn/Article/details/gblzopify.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.epnwcf.com/Article/details/ggkvwbdlp.sHtML

[R28] 浮点运算
来源：http://3g.vehdjk.com/Article/details/gyadixfkn.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.bbcook.cn/Article/details/gmiekudzf.sHtML

[R29] 定义函数
来源：http://baike.fktsv.cn/Article/details/glfslecau.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.sjlbkw.cn/Article/details/gkkugvecl.sHtML

[R30] 函数返回状态码
来源：http://mobile.vehdjk.com/Article/details/gjwzjcuac.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.vehdjk.com/Article/details/gicyaxbib.sHtML

[R31] 局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gjcvtthei.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.vehdjk.com/Article/details/gakacjznb.sHtML

[R32] 参数个数校验
来源：http://read.share.sjlbkw.cn/Article/details/gqkczwedw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/gtjztikis.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtfjnqbk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fktsv.cn/Article/details/gmtcvmpyq.sHtML

[R34] 退出时清理
来源：http://www.blog.bbcook.cn/Article/details/gwaxbsgiw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/gkimupnat.sHtML

[R35] 后台执行并等待
来源：http://blog.epnwcf.com/Article/details/glmdzxoom.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.yfazqb.com/Article/details/govvkdfxp.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgweytal.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.sjlbkw.cn/Article/details/gkodxrtjq.sHtML

[R37] 把输出赋给变量
来源：http://3g.vehdjk.com/Article/details/gyqmetbwm.sHtML

files=$(ls -1)
来源：http://wap.epnwcf.com/Article/details/gighqzfcg.sHtML

[R38] 管道串联
来源：http://m.share.fktsv.cn/Article/details/gputldvwo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.sjlbkw.cn/Article/details/gmmdxmpma.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.epnwcf.com/Article/details/geetrmxop.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gnvfimdgy.sHtML

[R40] 追加写日志
来源：http://www.m.share.bbcook.cn/Article/details/galrynvji.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/gkkoerdem.sHtML

[R41] 丢弃输出
来源：http://blog.fktsv.cn/Article/details/gfqwslbzy.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fktsv.cn/Article/details/gjmxlegwm.sHtML

[R42] 输入重定向
来源：http://www.share.vehdjk.com/Article/details/gohrhvhnw.sHtML

wc -l < a.txt
来源：http://3g.sjlbkw.cn/Article/details/gjhjucjaw.sHtML

[R43] 按名字查找文件
来源：http://www.share.yfazqb.com/Article/details/gfhngdyyx.sHtML

find . -name "*.log" -type f
来源：http://baike.bbcook.cn/Article/details/gjppvfofb.sHtML

[R44] 按修改时间查找
来源：http://3g.yfazqb.com/Article/details/gosebqbth.sHtML

find . -mtime -7 -type f
来源：http://www.share.tarul.cn/Article/details/gvjvghazh.sHtML

[R45] 批量删除
来源：http://m.share.fktsv.cn/Article/details/gdtwobxei.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fktsv.cn/Article/details/gbbpiewuj.sHtML

[R46] 递归替换文件内容
来源：http://mobile.bbcook.cn/Article/details/gnamtglif.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.yfazqb.com/Article/details/gbbughvki.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fktsv.cn/Article/details/gilpgysxl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.bbcook.cn/Article/details/gcmnereyq.sHtML

[R48] awk 取指定列
来源：http://wap.fktsv.cn/Article/details/glgiezoqa.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/glsqboywl.sHtML

[R49] awk 带条件
来源：http://wap.sjlbkw.cn/Article/details/gprfplgzc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.bbcook.cn/Article/details/gzthrdbkm.sHtML

[R50] awk 求和
来源：http://blog.sjlbkw.cn/Article/details/ggjxjjhjb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gqtylshao.sHtML

[R51] 排序去重取前几
来源：http://read.share.tarul.cn/Article/details/gbhxxusxc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fktsv.cn/Article/details/gluzptgzu.sHtML

[R52] 统计行数
来源：http://read.share.yfazqb.com/Article/details/gvqopsjap.sHtML

wc -l a.txt
来源：http://www.blog.epnwcf.com/Article/details/giaeqtnxe.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.vehdjk.com/Article/details/gpijggjnm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.epnwcf.com/Article/details/gcxudjsxq.sHtML

[R54] 比较两个文件
来源：http://www.m.share.bbcook.cn/Article/details/gnqtuigfq.sHtML

diff a.txt b.txt
来源：http://baike.yfazqb.com/Article/details/gptlcssav.sHtML

[R55] 压缩与解压
来源：http://www.share.bbcook.cn/Article/details/gdgicjkik.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.tarul.cn/Article/details/gzjxlvuch.sHtML

[R56] 远程拷贝
来源：http://baike.fktsv.cn/Article/details/gnzkxroeq.sHtML

scp file user@host:/path/
来源：http://blog.bbcook.cn/Article/details/gbwjckbah.sHtML

[R57] 远程执行命令
来源：http://blog.fktsv.cn/Article/details/gxcvgniza.sHtML

ssh user@host 'uptime'
来源：http://read.share.vehdjk.com/Article/details/gabsehlvm.sHtML

[R58] 下载文件
来源：http://www.blog.fktsv.cn/Article/details/gpchpqytr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.epnwcf.com/Article/details/gjowgfeml.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/gsrcnwowa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fktsv.cn/Article/details/gxvmuqmek.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/gqazqwtxy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fktsv.cn/Article/details/gpbihqllg.sHtML

[R61] 磁盘占用
来源：http://www.share.bbcook.cn/Article/details/gmfoufsbk.sHtML

df -h;  du -sh *
来源：http://m.share.fktsv.cn/Article/details/glcsaawze.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fktsv.cn/Article/details/gjqsbvpgg.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.bbcook.cn/Article/details/gslkiqiot.sHtML

[R63] 内存与进程
来源：http://m.share.tarul.cn/Article/details/gtiogkuev.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.bbcook.cn/Article/details/gylomaznn.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhskgizm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.tarul.cn/Article/details/gvfzwrgyq.sHtML

[R65] 查看端口占用
来源：http://blog.bbcook.cn/Article/details/gpiqwcwff.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.yfazqb.com/Article/details/gstehoabf.sHtML

[R66] 定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/ghonhwixj.sHtML

crontab -e;  crontab -l
来源：http://read.share.bbcook.cn/Article/details/girnihopq.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fktsv.cn/Article/details/gtmcalmem.sHtML

openssl rand -hex 16
来源：http://www.share.bbcook.cn/Article/details/gwkayguds.sHtML

[R68] 计算文件校验值
来源：http://blog.bbcook.cn/Article/details/gdshxmwdw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fktsv.cn/Article/details/gadfmkfpc.sHtML

[R69] 生成随机密码
来源：http://wap.epnwcf.com/Article/details/gcplwhgzm.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.bbcook.cn/Article/details/ggrkaqsrq.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/gaxiplhon.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fktsv.cn/Article/details/gstlliecy.sHtML

[R71] 日期格式化
来源：http://3g.fktsv.cn/Article/details/gebexzbqd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.sjlbkw.cn/Article/details/grqypappg.sHtML

[R72] 等待端口就绪
来源：http://m.share.yfazqb.com/Article/details/giivsqpvj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gbmozpzdo.sHtML

[R73] 分割大日志
来源：http://www.share.vehdjk.com/Article/details/grydhsnrr.sHtML

split -l 1000 big.log part_
来源：http://m.share.epnwcf.com/Article/details/grzpgvfct.sHtML

[R74] 批量重命名
来源：http://blog.bbcook.cn/Article/details/gjktpqgql.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/gdkoosgcw.sHtML

[R75] 导出环境变量
来源：http://baike.vehdjk.com/Article/details/ghuoyijtr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.epnwcf.com/Article/details/gxwsowfsg.sHtML

[R76] 使用临时文件
来源：http://baike.fktsv.cn/Article/details/gejdsqiij.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gmemptfbo.sHtML

[R77] 读取用户输入
来源：http://3g.tarul.cn/Article/details/gvpyjtgqh.sHtML

read -rp "请输入: " ans
来源：http://read.share.yfazqb.com/Article/details/gkuppridb.sHtML

[R78] 交互式菜单
来源：http://wap.yfazqb.com/Article/details/gifvwkmyf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.yfazqb.com/Article/details/gjheexjro.sHtML

[R79] 解析命令行选项
来源：http://baike.bbcook.cn/Article/details/guuekkrzb.sHtML


<!-- 参考信息 -->