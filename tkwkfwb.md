代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.epnwcf.com/Article/details/giszsoztv.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fktsv.cn/Article/details/glasvxhjb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gieuwrgkp.sHtML

[Q29] 最大最小值
来源：http://mobile.bbcook.cn/Article/details/gcnkeeirc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.tarul.cn/Article/details/gtrmrqrlx.sHtML

[Q30] 分组统计
来源：http://blog.yfazqb.com/Article/details/gjthdwxwi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gkxyexptx.sHtML

[Q31] 分组后过滤
来源：http://baike.bbcook.cn/Article/details/gefnuzxvk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fktsv.cn/Article/details/glrmjgord.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gquypmznz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/galaryvbw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.vehdjk.com/Article/details/gfkijdcjy.sHtML

[Q33] 多列分组
来源：http://m.share.tarul.cn/Article/details/gsxnhenoa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.epnwcf.com/Article/details/ghgucwehu.sHtML

[Q34] 每组取第一条
来源：http://3g.epnwcf.com/Article/details/gcvbmyacc.sHtML

SELECT * FROM (
来源：http://m.share.vehdjk.com/Article/details/gvuqtzcyr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.epnwcf.com/Article/details/gzheqsprf.sHtML

) t WHERE rn = 1;
来源：http://baike.vehdjk.com/Article/details/gwyiawjtd.sHtML

[Q35] 内连接
来源：http://www.share.tarul.cn/Article/details/gnyhjiycz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/ghamsarxe.sHtML

[Q36] 左连接
来源：http://baike.bbcook.cn/Article/details/gyyuctrmy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/glidpnzlp.sHtML

[Q37] 右连接
来源：http://baike.vehdjk.com/Article/details/gpmhnrwhf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.epnwcf.com/Article/details/goyatapwz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.bbcook.cn/Article/details/gkbikjfbw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.tarul.cn/Article/details/gthsivjuw.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.bbcook.cn/Article/details/gangbdvhg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.sjlbkw.cn/Article/details/gulzfilme.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.yfazqb.com/Article/details/gceajgdcz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.epnwcf.com/Article/details/gtzegicrb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.sjlbkw.cn/Article/details/grlwusnqa.sHtML

[Q41] 多表连接
来源：http://read.share.epnwcf.com/Article/details/gxblclloo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/gookgkhjn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.bbcook.cn/Article/details/gamolgheu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.yfazqb.com/Article/details/gcviznozb.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.yfazqb.com/Article/details/gyszaeuai.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.yfazqb.com/Article/details/gozparijp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.tarul.cn/Article/details/gwqouuenb.sHtML

[Q43] 标量子查询
来源：http://baike.yfazqb.com/Article/details/gkzhxtvgm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.epnwcf.com/Article/details/gntxskggj.sHtML

[Q44] IN 子查询
来源：http://www.blog.yfazqb.com/Article/details/gmnbrpgoj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fktsv.cn/Article/details/gxuxabuaf.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.bbcook.cn/Article/details/gzbtgvezt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gduzfvafw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.vehdjk.com/Article/details/gpxrebgzx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.sjlbkw.cn/Article/details/gykysqmkt.sHtML

[Q47] 与平均值比较
来源：http://www.blog.bbcook.cn/Article/details/gdemsgurs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.bbcook.cn/Article/details/gqgaurtkh.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.vehdjk.com/Article/details/geedldhis.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.tarul.cn/Article/details/gnizmvuil.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbflycgpo.sHtML

[Q49] 更新单行
来源：http://mobile.tarul.cn/Article/details/gdvchgrod.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gglxwnjzc.sHtML

[Q50] 批量更新
来源：http://3g.fktsv.cn/Article/details/grrqmvysn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.vehdjk.com/Article/details/goehfgmpo.sHtML

[Q51] 用子查询更新
来源：http://wap.sjlbkw.cn/Article/details/gudfeuccl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.epnwcf.com/Article/details/gsystcsee.sHtML

[Q52] 删除指定行
来源：http://baike.fktsv.cn/Article/details/gmmgxlbsn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/godznkeuo.sHtML

[Q53] 按条件删除
来源：http://m.share.sjlbkw.cn/Article/details/gwghvxywp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.bbcook.cn/Article/details/gvgitmvfg.sHtML

[Q54] 清空表
来源：http://mobile.yfazqb.com/Article/details/gnrnsomgl.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.sjlbkw.cn/Article/details/grfudxwjd.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fktsv.cn/Article/details/ggkibcymd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.epnwcf.com/Article/details/ghpivqhxr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.bbcook.cn/Article/details/gvbpvmpru.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.yfazqb.com/Article/details/gawgcpxqb.sHtML

[Q57] 行号
来源：http://3g.tarul.cn/Article/details/gcyvmzeuj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fktsv.cn/Article/details/gxnkwyycf.sHtML

[Q58] 累计求和
来源：http://read.share.fktsv.cn/Article/details/gggrwhfcs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.vehdjk.com/Article/details/grxirnqln.sHtML

[Q59] 分组内累计
来源：http://3g.vehdjk.com/Article/details/gufqkgvid.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gwddcusax.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.yfazqb.com/Article/details/gcgerhmbd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/grqfpeazr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gtpfyflvc.sHtML

[Q61] 移动平均
来源：http://blog.fktsv.cn/Article/details/gxwurresd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gvbjeekvu.sHtML

[Q62] 分组占比
来源：http://baike.yfazqb.com/Article/details/gdotnofhv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gzjrwwfsq.sHtML

[Q63] 开启事务
来源：http://www.blog.vehdjk.com/Article/details/ghqbouyvy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/guzuynglz.sHtML

[Q64] 提交事务
来源：http://www.blog.bbcook.cn/Article/details/ghecnetjj.sHtML

COMMIT;
来源：http://read.share.yfazqb.com/Article/details/gouxpzobb.sHtML

[Q65] 回滚事务
来源：http://3g.tarul.cn/Article/details/gdgcyehky.sHtML

ROLLBACK;
来源：http://m.share.tarul.cn/Article/details/gldfdgxbt.sHtML

[Q66] 行锁查询
来源：http://read.share.tarul.cn/Article/details/grjxkkwee.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.bbcook.cn/Article/details/gwvxwjhvj.sHtML

[Q67] 设置隔离级别
来源：http://wap.sjlbkw.cn/Article/details/glwbzpcit.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.vehdjk.com/Article/details/glrqrwtvp.sHtML

[Q68] 保存点
来源：http://blog.bbcook.cn/Article/details/gxehfzuvd.sHtML

SAVEPOINT sp1;
来源：http://baike.yfazqb.com/Article/details/gtzzpiprh.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.epnwcf.com/Article/details/ghqjzswan.sHtML

[Q69] 查看执行计划
来源：http://3g.fktsv.cn/Article/details/gizfjqyac.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/godjfqbxz.sHtML

[Q70] 更新统计信息
来源：http://baike.tarul.cn/Article/details/gpumunjuz.sHtML

ANALYZE TABLE users;
来源：http://m.share.bbcook.cn/Article/details/gqadncfbo.sHtML

[Q71] 查看建表语句
来源：http://www.share.yfazqb.com/Article/details/gpbqqefyb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.sjlbkw.cn/Article/details/gjoyxqkjn.sHtML

[Q72] 查看索引
来源：http://mobile.bbcook.cn/Article/details/goynuldzb.sHtML

SHOW INDEX FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gldtprori.sHtML

[Q73] 查看表状态
来源：http://m.share.sjlbkw.cn/Article/details/gswgyetwb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.bbcook.cn/Article/details/gpfzrunzr.sHtML

[Q74] 强制使用索引
来源：http://wap.bbcook.cn/Article/details/gvjxkhfwo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.tarul.cn/Article/details/gfnstyyqu.sHtML

[Q75] 日期格式化
来源：http://blog.fktsv.cn/Article/details/goycydzlu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.epnwcf.com/Article/details/geseetfqc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fktsv.cn/Article/details/glkxycjtw.sHtML

[Q76] 按天统计
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlkbnsir.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.sjlbkw.cn/Article/details/gnpjsizhy.sHtML

[Q77] 时间加减
来源：http://blog.vehdjk.com/Article/details/gscbcppqh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.epnwcf.com/Article/details/gfpftnbat.sHtML

[Q78] 当前时间
来源：http://www.m.share.bbcook.cn/Article/details/gaehypcco.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.sjlbkw.cn/Article/details/gxkwoifhh.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.epnwcf.com/Article/details/ggttwmkdz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.tarul.cn/Article/details/gerbkqkzz.sHtML

[Q80] 字符串截取
来源：http://baike.epnwcf.com/Article/details/gxeqhmddj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gzstbkvzx.sHtML

[Q81] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gyhgnnvry.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.epnwcf.com/Article/details/gglkouteb.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.sjlbkw.cn/Article/details/gfkzcvsws.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gwsvzzymz.sHtML

[Q83] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/gebcbiosh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/glezyrfpc.sHtML

[Q84] 去除首尾空格
来源：http://baike.tarul.cn/Article/details/gbcactelu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/ggmmpszch.sHtML

[Q85] 数值取整
来源：http://mobile.fktsv.cn/Article/details/gscgcpgai.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.sjlbkw.cn/Article/details/gyuuqrpvb.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.bbcook.cn/Article/details/gbipbqfph.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.vehdjk.com/Article/details/ggxubrgyu.sHtML

[Q87] JSON 字段做条件
来源：http://baike.epnwcf.com/Article/details/gfelmmkau.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.sjlbkw.cn/Article/details/gsrvfgfbp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.sjlbkw.cn/Article/details/gubmjjafa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.tarul.cn/Article/details/ghweguyep.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.yfazqb.com/Article/details/gsrzaxvis.sHtML

[Q89] 判断表是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gmckjthnq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gwhkkrhjg.sHtML

[Q90] 生成序号列
来源：http://3g.epnwcf.com/Article/details/gipafigxv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.sjlbkw.cn/Article/details/gjncsejpp.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpxhxzrqt.sHtML

R. Bash 专题
来源：http://www.m.share.vehdjk.com/Article/details/govcldygc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/glcaqexcf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.yfazqb.com/Article/details/gmhqndzfq.sHtML

#!/usr/bin/env bash
来源：http://www.share.yfazqb.com/Article/details/ggacuyvqs.sHtML

set -euo pipefail
来源：http://m.share.vehdjk.com/Article/details/gaudonawe.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/gdklfovwp.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.sjlbkw.cn/Article/details/glqydtvyh.sHtML

[R03] 只读变量
来源：http://m.share.yfazqb.com/Article/details/gxkzimkwg.sHtML

readonly PI=3.14
来源：http://www.share.fktsv.cn/Article/details/gajbumrce.sHtML

[R04] 位置参数
来源：http://baike.vehdjk.com/Article/details/gcisvgmmx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.vehdjk.com/Article/details/grvdhinpc.sHtML

[R05] 参数默认值
来源：http://m.share.bbcook.cn/Article/details/gfptvkihv.sHtML

name="${1:-default}"
来源：http://www.share.yfazqb.com/Article/details/gmmgzylrv.sHtML

[R06] 判断命令是否存在
来源：http://blog.yfazqb.com/Article/details/gqzvjxsaf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gzddsrcyl.sHtML

[R07] if 判断文件
来源：http://3g.vehdjk.com/Article/details/gsqrptodk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.vehdjk.com/Article/details/gtemfwwiy.sHtML

[R08] 数值比较
来源：http://3g.sjlbkw.cn/Article/details/gfwjakslc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.bbcook.cn/Article/details/gugedebnv.sHtML

[R09] 字符串比较
来源：http://3g.vehdjk.com/Article/details/gqiesejho.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.tarul.cn/Article/details/gamocmwdv.sHtML

[R10] 正则匹配
来源：http://blog.epnwcf.com/Article/details/gtpdvslcq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.yfazqb.com/Article/details/gyrusybbg.sHtML

[R11] case 多分支
来源：http://read.share.epnwcf.com/Article/details/gsnbgiftm.sHtML

case "$1" in
来源：http://read.share.vehdjk.com/Article/details/gcxdckgcw.sHtML

start) echo "启动" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gwdysbgxg.sHtML

stop)  echo "停止" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gayvtwtua.sHtML

*)     echo "未知命令" ;;
来源：http://baike.sjlbkw.cn/Article/details/gzasrutey.sHtML

esac
来源：http://baike.yfazqb.com/Article/details/gxadfvepg.sHtML

[R12] for 遍历文件
来源：http://baike.vehdjk.com/Article/details/gqtjgoqle.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.vehdjk.com/Article/details/gfobrifct.sHtML

[R13] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gzboklgnn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/graoastng.sHtML

[R14] C 风格 for
来源：http://www.share.fktsv.cn/Article/details/gcsncwajs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gthduzctu.sHtML

[R15] while 逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gaqrkmthp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.epnwcf.com/Article/details/gokzzfwel.sHtML

[R16] until 等待条件
来源：http://www.m.share.vehdjk.com/Article/details/gsadxhfvw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gnooaxcxf.sHtML

[R17] 数组定义与取值
来源：http://baike.sjlbkw.cn/Article/details/gwhdocsdn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.tarul.cn/Article/details/gfzuauxwy.sHtML

[R18] 遍历数组
来源：http://baike.vehdjk.com/Article/details/gevtvbhlw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.bbcook.cn/Article/details/gigcskvkd.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gsnnurulx.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.bbcook.cn/Article/details/gdjydehbp.sHtML

[R20] 关联数组（字典）
来源：http://baike.vehdjk.com/Article/details/gabuedkkx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.bbcook.cn/Article/details/gawjxqogg.sHtML

[R21] 字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gsfudgmak.sHtML

echo "${#s}"
来源：http://www.blog.bbcook.cn/Article/details/ggczvzxgx.sHtML

[R22] 截取子串
来源：http://wap.bbcook.cn/Article/details/gelgrvnve.sHtML

echo "${s:0:5}"
来源：http://www.blog.yfazqb.com/Article/details/gxowzkfnh.sHtML

[R23] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/gzgwatkhj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.vehdjk.com/Article/details/gbufauefi.sHtML

[R24] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/gcrypnsft.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.epnwcf.com/Article/details/geziqgkom.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.epnwcf.com/Article/details/gfcapeajb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.tarul.cn/Article/details/gujiiuyua.sHtML

[R26] 命令替换
来源：http://blog.bbcook.cn/Article/details/gwizumwoj.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fktsv.cn/Article/details/gywphrxbm.sHtML

[R27] 算术展开
来源：http://www.blog.fktsv.cn/Article/details/geclcvtkv.sHtML

echo $((1 + 2 * 3))
来源：http://3g.epnwcf.com/Article/details/ghwombkwt.sHtML

[R28] 浮点运算
来源：http://mobile.yfazqb.com/Article/details/gundlxhpo.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.tarul.cn/Article/details/guczfkkzm.sHtML

[R29] 定义函数
来源：http://www.blog.yfazqb.com/Article/details/gsaipcsvb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gecxayxxy.sHtML

[R30] 函数返回状态码
来源：http://3g.vehdjk.com/Article/details/gfjinvrbr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.bbcook.cn/Article/details/gddjytupv.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/glyhphjsd.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.epnwcf.com/Article/details/gclnlxrrb.sHtML

[R32] 参数个数校验
来源：http://mobile.epnwcf.com/Article/details/gldswtzfi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gywfroxpo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.bbcook.cn/Article/details/gzhluuylp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.epnwcf.com/Article/details/gixozsflc.sHtML

[R34] 退出时清理
来源：http://baike.vehdjk.com/Article/details/guyapyjkq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/gtjcdztkd.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fktsv.cn/Article/details/gjguusjor.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.bbcook.cn/Article/details/gjvcmcygx.sHtML

[R36] 并发执行多个任务
来源：http://wap.vehdjk.com/Article/details/gfxektvoa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.bbcook.cn/Article/details/gyrwqwzce.sHtML

[R37] 把输出赋给变量
来源：http://blog.sjlbkw.cn/Article/details/gvznevgyh.sHtML

files=$(ls -1)
来源：http://baike.vehdjk.com/Article/details/gvszkvrnj.sHtML

[R38] 管道串联
来源：http://blog.vehdjk.com/Article/details/gjhdcfewn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.vehdjk.com/Article/details/gsfmvirvc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.tarul.cn/Article/details/gstfkscny.sHtML

cmd > out.log 2>&1
来源：http://read.share.bbcook.cn/Article/details/gyalulygf.sHtML

[R40] 追加写日志
来源：http://www.m.share.vehdjk.com/Article/details/gihwdixxy.sHtML

echo "log" >> out.log
来源：http://3g.epnwcf.com/Article/details/gdtgxgmny.sHtML

[R41] 丢弃输出
来源：http://www.blog.bbcook.cn/Article/details/gzkenxhxb.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.yfazqb.com/Article/details/gyktuuxwo.sHtML

[R42] 输入重定向
来源：http://www.share.yfazqb.com/Article/details/gtcjobddr.sHtML

wc -l < a.txt
来源：http://m.share.yfazqb.com/Article/details/gmkouetmm.sHtML

[R43] 按名字查找文件
来源：http://baike.vehdjk.com/Article/details/ghwozrvtt.sHtML

find . -name "*.log" -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gjjvsqrja.sHtML

[R44] 按修改时间查找
来源：http://www.share.bbcook.cn/Article/details/gckwmihta.sHtML

find . -mtime -7 -type f
来源：http://m.share.fktsv.cn/Article/details/grcfaseic.sHtML

[R45] 批量删除
来源：http://mobile.bbcook.cn/Article/details/gparlqphc.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gchgmrxdv.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.epnwcf.com/Article/details/gdzptcoqg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.bbcook.cn/Article/details/gnsnkydde.sHtML

[R47] sed 单行替换
来源：http://blog.epnwcf.com/Article/details/gkpncjgcg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/glfegydjp.sHtML

[R48] awk 取指定列
来源：http://blog.vehdjk.com/Article/details/gagfbmzch.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.epnwcf.com/Article/details/gyxdqyhsc.sHtML

[R49] awk 带条件
来源：http://read.share.sjlbkw.cn/Article/details/gwyylihql.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.tarul.cn/Article/details/grpfuqapu.sHtML

[R50] awk 求和
来源：http://baike.yfazqb.com/Article/details/gcxnvjjig.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.tarul.cn/Article/details/grgrsrkig.sHtML

[R51] 排序去重取前几
来源：http://www.blog.sjlbkw.cn/Article/details/gtpcukwfp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fktsv.cn/Article/details/glbfckgyv.sHtML

[R52] 统计行数
来源：http://baike.vehdjk.com/Article/details/gyrxgxqyl.sHtML

wc -l a.txt
来源：http://mobile.tarul.cn/Article/details/gejkozonu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.epnwcf.com/Article/details/gfrwyaisp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.epnwcf.com/Article/details/gtmrtdtry.sHtML

[R54] 比较两个文件
来源：http://mobile.vehdjk.com/Article/details/gtwjtiffk.sHtML

diff a.txt b.txt
来源：http://3g.fktsv.cn/Article/details/galrlscpl.sHtML

[R55] 压缩与解压
来源：http://mobile.tarul.cn/Article/details/gybpbxeyh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.vehdjk.com/Article/details/gomptbrfz.sHtML

[R56] 远程拷贝
来源：http://3g.fktsv.cn/Article/details/gnqdnnsxk.sHtML

scp file user@host:/path/
来源：http://baike.sjlbkw.cn/Article/details/grimvjkcw.sHtML

[R57] 远程执行命令
来源：http://3g.vehdjk.com/Article/details/gwlkmdpud.sHtML

ssh user@host 'uptime'
来源：http://m.share.bbcook.cn/Article/details/grxdzhvdh.sHtML

[R58] 下载文件
来源：http://3g.yfazqb.com/Article/details/gpwdfarhc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.bbcook.cn/Article/details/gjukqkyiq.sHtML

[R59] 发 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gzqvtocrn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.tarul.cn/Article/details/gjtaxuqqe.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gajkstgqo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.yfazqb.com/Article/details/gymagfrmt.sHtML

[R61] 磁盘占用
来源：http://blog.fktsv.cn/Article/details/gizhuysxw.sHtML

df -h;  du -sh *
来源：http://www.blog.tarul.cn/Article/details/gjggmplkr.sHtML

[R62] 找最占空间的文件
来源：http://www.share.tarul.cn/Article/details/gvpdaqcuo.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.sjlbkw.cn/Article/details/gducofbvh.sHtML

[R63] 内存与进程
来源：http://read.share.bbcook.cn/Article/details/gyffsoccc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fktsv.cn/Article/details/gsffqlojt.sHtML

[R64] 结束进程
来源：http://baike.sjlbkw.cn/Article/details/gpenpyyet.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.vehdjk.com/Article/details/gqkropcmi.sHtML

[R65] 查看端口占用
来源：http://3g.tarul.cn/Article/details/gketayhib.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.vehdjk.com/Article/details/gngcskwog.sHtML

[R66] 定时任务
来源：http://wap.epnwcf.com/Article/details/gosjogcxs.sHtML

crontab -e;  crontab -l
来源：http://wap.epnwcf.com/Article/details/glfjxtzfz.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.vehdjk.com/Article/details/gifserrsk.sHtML

openssl rand -hex 16
来源：http://3g.fktsv.cn/Article/details/gosllskfh.sHtML

[R68] 计算文件校验值
来源：http://www.share.sjlbkw.cn/Article/details/goelmnfad.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.yfazqb.com/Article/details/gfhzybtir.sHtML

[R69] 生成随机密码
来源：http://wap.epnwcf.com/Article/details/gcncbfkuz.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.yfazqb.com/Article/details/glbpkszzv.sHtML

[R70] 时间戳与互转
来源：http://read.share.sjlbkw.cn/Article/details/gavjsgtil.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.tarul.cn/Article/details/gyibcvelb.sHtML

[R71] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gxcelqvcp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.vehdjk.com/Article/details/gdhkufowx.sHtML

[R72] 等待端口就绪
来源：http://blog.yfazqb.com/Article/details/gsvihbsti.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/gjxmlrtud.sHtML

[R73] 分割大日志
来源：http://baike.sjlbkw.cn/Article/details/gyqjuvfdc.sHtML

split -l 1000 big.log part_
来源：http://m.share.yfazqb.com/Article/details/gfzfoeysc.sHtML

[R74] 批量重命名
来源：http://mobile.vehdjk.com/Article/details/gtxhhlvcz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gzkdltjns.sHtML

[R75] 导出环境变量
来源：http://read.share.tarul.cn/Article/details/gsarzicpm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.vehdjk.com/Article/details/gnnvgwnxe.sHtML

[R76] 使用临时文件
来源：http://3g.epnwcf.com/Article/details/gcbiwoalr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/gwrawjhhy.sHtML

[R77] 读取用户输入
来源：http://www.blog.tarul.cn/Article/details/gctpebbla.sHtML


<!-- 参考信息 -->