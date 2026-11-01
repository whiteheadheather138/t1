代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.bbcook.cn/Article/details/ghcfksxqs.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/ghbqmvrzv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gihcuudxf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.tarul.cn/Article/details/gtgauvvks.sHtML

[Q33] 多列分组
来源：http://www.share.bbcook.cn/Article/details/gowwumews.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.tarul.cn/Article/details/ghyhmesqy.sHtML

[Q34] 每组取第一条
来源：http://wap.tarul.cn/Article/details/grmnzrson.sHtML

SELECT * FROM (
来源：http://3g.bbcook.cn/Article/details/gerccdewo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.epnwcf.com/Article/details/gmerrzlzw.sHtML

) t WHERE rn = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gsilwqvnf.sHtML

[Q35] 内连接
来源：http://read.share.bbcook.cn/Article/details/gboligtot.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gdpggwxdz.sHtML

[Q36] 左连接
来源：http://m.share.vehdjk.com/Article/details/ggsifvdof.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/gakteocwh.sHtML

[Q37] 右连接
来源：http://www.m.share.vehdjk.com/Article/details/gmvdfrbde.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.epnwcf.com/Article/details/guozlccbt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.sjlbkw.cn/Article/details/gskojuqzx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.yfazqb.com/Article/details/ggfkpfpub.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.vehdjk.com/Article/details/garspuwyd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.vehdjk.com/Article/details/ginebmriw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.sjlbkw.cn/Article/details/gcfwxllcr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.tarul.cn/Article/details/gsbtfixhu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fktsv.cn/Article/details/gywtepixz.sHtML

[Q41] 多表连接
来源：http://3g.tarul.cn/Article/details/grfeixjld.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.sjlbkw.cn/Article/details/gxbaqnfue.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.tarul.cn/Article/details/gbabpywsr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.epnwcf.com/Article/details/gjltrjkrk.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.bbcook.cn/Article/details/gepgncbwn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.tarul.cn/Article/details/gkmczeeux.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.yfazqb.com/Article/details/gqanyfhxv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.epnwcf.com/Article/details/gtizkndiz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.vehdjk.com/Article/details/gwjieiblm.sHtML

[Q44] IN 子查询
来源：http://www.blog.fktsv.cn/Article/details/geesmxnwn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.bbcook.cn/Article/details/gtemioopk.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.bbcook.cn/Article/details/gyusyxqph.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gpiqkkkyt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.epnwcf.com/Article/details/gloiihpua.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gpqcrddkm.sHtML

[Q47] 与平均值比较
来源：http://www.share.fktsv.cn/Article/details/gwykvkvju.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.tarul.cn/Article/details/gpvprsppe.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.vehdjk.com/Article/details/ggviywcyd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.vehdjk.com/Article/details/gluynykzc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.sjlbkw.cn/Article/details/grhnaisgn.sHtML

[Q49] 更新单行
来源：http://wap.bbcook.cn/Article/details/gotikvfam.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gxqqiihkd.sHtML

[Q50] 批量更新
来源：http://m.share.sjlbkw.cn/Article/details/gsuixsauc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.epnwcf.com/Article/details/gcwnmkmzx.sHtML

[Q51] 用子查询更新
来源：http://baike.bbcook.cn/Article/details/ghjmumqat.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.epnwcf.com/Article/details/gxmcbzhkv.sHtML

[Q52] 删除指定行
来源：http://www.blog.sjlbkw.cn/Article/details/gbmsytqfz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gkurbeffx.sHtML

[Q53] 按条件删除
来源：http://www.share.fktsv.cn/Article/details/ghunjqocs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.epnwcf.com/Article/details/gaimeuaut.sHtML

[Q54] 清空表
来源：http://blog.bbcook.cn/Article/details/gzxuriqvs.sHtML

TRUNCATE TABLE logs;
来源：http://baike.epnwcf.com/Article/details/gspytmsut.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.tarul.cn/Article/details/gummmmruc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gwlbhftwy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.bbcook.cn/Article/details/gjrjwekcj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.vehdjk.com/Article/details/ggtkmuwlv.sHtML

[Q57] 行号
来源：http://www.m.share.fktsv.cn/Article/details/gfyucxtab.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fktsv.cn/Article/details/gjkhzjiyw.sHtML

[Q58] 累计求和
来源：http://www.share.bbcook.cn/Article/details/gnkwjvntm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.bbcook.cn/Article/details/gidndwjwp.sHtML

[Q59] 分组内累计
来源：http://read.share.yfazqb.com/Article/details/guauladmp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gaayxrvwj.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.yfazqb.com/Article/details/gwnppjxle.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.bbcook.cn/Article/details/gfzgrokpn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.tarul.cn/Article/details/grcgcbizx.sHtML

[Q61] 移动平均
来源：http://baike.bbcook.cn/Article/details/gcxdzxfbp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gjdeulbhh.sHtML

[Q62] 分组占比
来源：http://read.share.tarul.cn/Article/details/gzytklqos.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/ghafgdxhb.sHtML

[Q63] 开启事务
来源：http://www.blog.sjlbkw.cn/Article/details/gfbtjenzp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.bbcook.cn/Article/details/gumywyxco.sHtML

[Q64] 提交事务
来源：http://m.share.bbcook.cn/Article/details/gsqjcptxp.sHtML

COMMIT;
来源：http://www.blog.bbcook.cn/Article/details/gdcudgigx.sHtML

[Q65] 回滚事务
来源：http://3g.vehdjk.com/Article/details/gvvoiyyix.sHtML

ROLLBACK;
来源：http://read.share.vehdjk.com/Article/details/gqpgowqtk.sHtML

[Q66] 行锁查询
来源：http://baike.bbcook.cn/Article/details/gmgnoemlh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fktsv.cn/Article/details/gmrqrydqb.sHtML

[Q67] 设置隔离级别
来源：http://blog.bbcook.cn/Article/details/gjnfixmdy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.vehdjk.com/Article/details/gadnaysik.sHtML

[Q68] 保存点
来源：http://baike.sjlbkw.cn/Article/details/grgrznqim.sHtML

SAVEPOINT sp1;
来源：http://read.share.fktsv.cn/Article/details/ghfixfxsp.sHtML

ROLLBACK TO sp1;
来源：http://read.share.vehdjk.com/Article/details/geozowowf.sHtML

[Q69] 查看执行计划
来源：http://www.blog.yfazqb.com/Article/details/gifiugksl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.vehdjk.com/Article/details/ghrksczqv.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/gwazoeyzi.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.tarul.cn/Article/details/gallssotn.sHtML

[Q71] 查看建表语句
来源：http://read.share.tarul.cn/Article/details/gdeufkits.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.bbcook.cn/Article/details/gggpcsurb.sHtML

[Q72] 查看索引
来源：http://wap.bbcook.cn/Article/details/gozduhcuj.sHtML

SHOW INDEX FROM users;
来源：http://blog.yfazqb.com/Article/details/gaxsefeye.sHtML

[Q73] 查看表状态
来源：http://3g.sjlbkw.cn/Article/details/gtsdqtjyq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.bbcook.cn/Article/details/gyrtbrdff.sHtML

[Q74] 强制使用索引
来源：http://www.blog.yfazqb.com/Article/details/gyptrilke.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.tarul.cn/Article/details/gbpfinoey.sHtML

[Q75] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gwpkvruys.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.epnwcf.com/Article/details/gehgvfghd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.tarul.cn/Article/details/gshpedwws.sHtML

[Q76] 按天统计
来源：http://baike.yfazqb.com/Article/details/grjreyhfz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvtdziub.sHtML

[Q77] 时间加减
来源：http://www.blog.sjlbkw.cn/Article/details/gnwmnmdyk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.tarul.cn/Article/details/gqhqqhlgv.sHtML

[Q78] 当前时间
来源：http://wap.fktsv.cn/Article/details/gkpsgakwp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.tarul.cn/Article/details/gfvlapiup.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/gzxmkenar.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.tarul.cn/Article/details/gjapxbplx.sHtML

[Q80] 字符串截取
来源：http://baike.tarul.cn/Article/details/gfekjdbzr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.tarul.cn/Article/details/gjjrqkraq.sHtML

[Q81] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gpazcophr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.vehdjk.com/Article/details/gorwrybum.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/gelrpcptq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gionolesp.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gakoetvor.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/geevrztqc.sHtML

[Q84] 去除首尾空格
来源：http://wap.sjlbkw.cn/Article/details/gecarnhzz.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/grdlubocb.sHtML

[Q85] 数值取整
来源：http://baike.bbcook.cn/Article/details/gpjzmuyfl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.vehdjk.com/Article/details/gvmhfnnwd.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.yfazqb.com/Article/details/gxnayxnjt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.vehdjk.com/Article/details/gxyvivjfj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.vehdjk.com/Article/details/gnjdobnyd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.vehdjk.com/Article/details/gstleypxv.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fktsv.cn/Article/details/gvglglmwx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwttxidk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.bbcook.cn/Article/details/gvhnxubth.sHtML

[Q89] 判断表是否存在
来源：http://baike.fktsv.cn/Article/details/gjphvevsu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fktsv.cn/Article/details/gwfzmeqjm.sHtML

[Q90] 生成序号列
来源：http://www.share.yfazqb.com/Article/details/gayhxuxxx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.vehdjk.com/Article/details/gzbredqdu.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/grmwxjxkm.sHtML

R. Bash 专题
来源：http://baike.sjlbkw.cn/Article/details/gudftdzso.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glhvuiwmy.sHtML

[R01] shebang 与严格模式
来源：http://read.share.epnwcf.com/Article/details/glvobnyia.sHtML

#!/usr/bin/env bash
来源：http://wap.bbcook.cn/Article/details/gwxekdsgo.sHtML

set -euo pipefail
来源：http://mobile.yfazqb.com/Article/details/gxyfgpnfw.sHtML

[R02] 变量赋值与使用
来源：http://wap.sjlbkw.cn/Article/details/gesfxecyx.sHtML

name="Tom"; echo "$name"
来源：http://baike.vehdjk.com/Article/details/gginqjpof.sHtML

[R03] 只读变量
来源：http://wap.sjlbkw.cn/Article/details/gsbsfgrsl.sHtML

readonly PI=3.14
来源：http://3g.vehdjk.com/Article/details/gjlmwerri.sHtML

[R04] 位置参数
来源：http://m.share.bbcook.cn/Article/details/gtevotdqo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.tarul.cn/Article/details/gucqhydea.sHtML

[R05] 参数默认值
来源：http://wap.epnwcf.com/Article/details/gxmybsqqj.sHtML

name="${1:-default}"
来源：http://www.share.fktsv.cn/Article/details/gtsdjnffm.sHtML

[R06] 判断命令是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gsfhfxibb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gbpsadvxo.sHtML

[R07] if 判断文件
来源：http://blog.tarul.cn/Article/details/gbnldolrb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.tarul.cn/Article/details/goxxtdeio.sHtML

[R08] 数值比较
来源：http://wap.yfazqb.com/Article/details/gxwvcahnv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.yfazqb.com/Article/details/gfoqwofuv.sHtML

[R09] 字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gmmjrjjqd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.yfazqb.com/Article/details/gtopzgngi.sHtML

[R10] 正则匹配
来源：http://read.share.sjlbkw.cn/Article/details/gojsvsfkf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.vehdjk.com/Article/details/gamvbyshe.sHtML

[R11] case 多分支
来源：http://baike.epnwcf.com/Article/details/gxuuiruzr.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/gkbyrshka.sHtML

start) echo "启动" ;;
来源：http://baike.bbcook.cn/Article/details/gffbnxcsj.sHtML

stop)  echo "停止" ;;
来源：http://baike.fktsv.cn/Article/details/gflzcrfwn.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.bbcook.cn/Article/details/guypvtumt.sHtML

esac
来源：http://baike.bbcook.cn/Article/details/gyogyqakv.sHtML

[R12] for 遍历文件
来源：http://www.blog.yfazqb.com/Article/details/grymublvq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.tarul.cn/Article/details/gjyumpauh.sHtML

[R13] for 计数循环
来源：http://mobile.tarul.cn/Article/details/glqfgglud.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/ggwyznhdi.sHtML

[R14] C 风格 for
来源：http://www.share.vehdjk.com/Article/details/gdfibnxlw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gozsonyou.sHtML

[R15] while 逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gcjhgwnqc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.epnwcf.com/Article/details/glhjbejrj.sHtML

[R16] until 等待条件
来源：http://read.share.tarul.cn/Article/details/glvsrrrmu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/ghfmwjbfs.sHtML

[R17] 数组定义与取值
来源：http://www.share.bbcook.cn/Article/details/gtltvlfsj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.bbcook.cn/Article/details/gqexdukor.sHtML

[R18] 遍历数组
来源：http://m.share.yfazqb.com/Article/details/gzaekbohn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.epnwcf.com/Article/details/gbbeltyvz.sHtML

[R19] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/gsxrxhlvc.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/gspbeawpa.sHtML

[R20] 关联数组（字典）
来源：http://m.share.bbcook.cn/Article/details/glyelpctm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gxhdavohg.sHtML

[R21] 字符串长度
来源：http://wap.yfazqb.com/Article/details/gxcdijtts.sHtML

echo "${#s}"
来源：http://m.share.fktsv.cn/Article/details/gfvbvfplf.sHtML

[R22] 截取子串
来源：http://blog.fktsv.cn/Article/details/gqwjcwoth.sHtML

echo "${s:0:5}"
来源：http://baike.sjlbkw.cn/Article/details/goslsepvb.sHtML

[R23] 字符串替换
来源：http://read.share.yfazqb.com/Article/details/ggutbnnrw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.yfazqb.com/Article/details/ghveojiqr.sHtML

[R24] 大小写转换
来源：http://3g.epnwcf.com/Article/details/geqdgxqes.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fktsv.cn/Article/details/gfhuboqgk.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.sjlbkw.cn/Article/details/goiyxhkjc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.epnwcf.com/Article/details/gfchqurgk.sHtML

[R26] 命令替换
来源：http://m.share.fktsv.cn/Article/details/ggyizcgym.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.sjlbkw.cn/Article/details/gymopgeli.sHtML

[R27] 算术展开
来源：http://read.share.fktsv.cn/Article/details/glvbcppua.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.tarul.cn/Article/details/gxyrcapox.sHtML

[R28] 浮点运算
来源：http://www.blog.epnwcf.com/Article/details/gqkclmosb.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/gaqyfwepl.sHtML

[R29] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/gynkovoyf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.sjlbkw.cn/Article/details/ggtealnky.sHtML

[R30] 函数返回状态码
来源：http://m.share.fktsv.cn/Article/details/ghhrnltpd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.epnwcf.com/Article/details/gqoemwixn.sHtML

[R31] 局部变量
来源：http://www.share.tarul.cn/Article/details/gjamxgshx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/grorlxnob.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fktsv.cn/Article/details/ginfwpmoj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.vehdjk.com/Article/details/gcmtyishx.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fktsv.cn/Article/details/gifxslewx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.vehdjk.com/Article/details/gwggifsby.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gwkumsgac.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gxwifvlas.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/gihfvabzy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.yfazqb.com/Article/details/gdrkbzcax.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/gvfgnghzn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.tarul.cn/Article/details/gzuwbigus.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.tarul.cn/Article/details/gshljdjxr.sHtML

files=$(ls -1)
来源：http://www.share.epnwcf.com/Article/details/goktwhyim.sHtML

[R38] 管道串联
来源：http://3g.tarul.cn/Article/details/ggkyiobza.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.vehdjk.com/Article/details/gwdkxypis.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.yfazqb.com/Article/details/gzrvmpaov.sHtML

cmd > out.log 2>&1
来源：http://mobile.bbcook.cn/Article/details/gqmulmxjt.sHtML

[R40] 追加写日志
来源：http://3g.sjlbkw.cn/Article/details/gypfupmsq.sHtML

echo "log" >> out.log
来源：http://www.share.vehdjk.com/Article/details/grdgxhqen.sHtML

[R41] 丢弃输出
来源：http://baike.epnwcf.com/Article/details/gtljvlcxn.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.vehdjk.com/Article/details/gponxjgxj.sHtML

[R42] 输入重定向
来源：http://www.m.share.tarul.cn/Article/details/gkjuzoajc.sHtML

wc -l < a.txt
来源：http://www.m.share.tarul.cn/Article/details/gesymyskv.sHtML

[R43] 按名字查找文件
来源：http://3g.fktsv.cn/Article/details/gjwwvqmxo.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.vehdjk.com/Article/details/gidsykuwp.sHtML

[R44] 按修改时间查找
来源：http://mobile.epnwcf.com/Article/details/gejatzcxd.sHtML

find . -mtime -7 -type f
来源：http://wap.bbcook.cn/Article/details/girkxrigr.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqmqxpmn.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fktsv.cn/Article/details/gklycduxr.sHtML

[R46] 递归替换文件内容
来源：http://baike.fktsv.cn/Article/details/grolegxrp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.bbcook.cn/Article/details/gbpwvumsm.sHtML

[R47] sed 单行替换
来源：http://read.share.bbcook.cn/Article/details/gqhlinhtw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/glyqyoqab.sHtML

[R48] awk 取指定列
来源：http://read.share.yfazqb.com/Article/details/gvppdxznp.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.tarul.cn/Article/details/gbwqqfzyh.sHtML

[R49] awk 带条件
来源：http://blog.sjlbkw.cn/Article/details/gvzagvtxg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.vehdjk.com/Article/details/ggczmcjfn.sHtML

[R50] awk 求和
来源：http://www.m.share.tarul.cn/Article/details/guulvazab.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.epnwcf.com/Article/details/gebxwqznj.sHtML

[R51] 排序去重取前几
来源：http://mobile.bbcook.cn/Article/details/gzfqfsrxs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.bbcook.cn/Article/details/gqxqwqspt.sHtML

[R52] 统计行数
来源：http://www.m.share.vehdjk.com/Article/details/gxcxsihrf.sHtML

wc -l a.txt
来源：http://3g.vehdjk.com/Article/details/gkfcmcxwf.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fktsv.cn/Article/details/gyllvxbar.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.tarul.cn/Article/details/gqiaddszy.sHtML

[R54] 比较两个文件
来源：http://mobile.bbcook.cn/Article/details/gamqotlyf.sHtML

diff a.txt b.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwfogsso.sHtML

[R55] 压缩与解压
来源：http://read.share.yfazqb.com/Article/details/gqkubphqg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fktsv.cn/Article/details/gyrajcfak.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/ghujgcpnq.sHtML

scp file user@host:/path/
来源：http://www.share.fktsv.cn/Article/details/gvyunsxfd.sHtML

[R57] 远程执行命令
来源：http://www.m.share.yfazqb.com/Article/details/gybyclbph.sHtML

ssh user@host 'uptime'
来源：http://blog.fktsv.cn/Article/details/glzfdalqp.sHtML

[R58] 下载文件
来源：http://3g.fktsv.cn/Article/details/gnpoxaudd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.yfazqb.com/Article/details/gfketmilo.sHtML

[R59] 发 POST JSON
来源：http://wap.yfazqb.com/Article/details/gmogntedt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.tarul.cn/Article/details/gduoufsie.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/gymnmljgh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.tarul.cn/Article/details/gpacvtwwb.sHtML

[R61] 磁盘占用
来源：http://read.share.tarul.cn/Article/details/ggfhjfbvx.sHtML

df -h;  du -sh *
来源：http://www.blog.tarul.cn/Article/details/gykpsfsxk.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.vehdjk.com/Article/details/gwsrladyt.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fktsv.cn/Article/details/gqpsxkwtf.sHtML

[R63] 内存与进程
来源：http://read.share.sjlbkw.cn/Article/details/gomzyyxeh.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.sjlbkw.cn/Article/details/glogcfcsd.sHtML

[R64] 结束进程
来源：http://m.share.epnwcf.com/Article/details/gzmtqtkhq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.epnwcf.com/Article/details/gciebwsvo.sHtML

[R65] 查看端口占用
来源：http://wap.tarul.cn/Article/details/gscnpxyuj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.tarul.cn/Article/details/gjnxnnnko.sHtML

[R66] 定时任务
来源：http://wap.bbcook.cn/Article/details/guyrjmctm.sHtML

crontab -e;  crontab -l
来源：http://mobile.tarul.cn/Article/details/gvxchpqdy.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.tarul.cn/Article/details/gypnhmwlw.sHtML

openssl rand -hex 16
来源：http://www.share.sjlbkw.cn/Article/details/gdpgzmyfn.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.tarul.cn/Article/details/gvghmobkm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.bbcook.cn/Article/details/gtqbukjng.sHtML

[R69] 生成随机密码
来源：http://blog.fktsv.cn/Article/details/ggjaplori.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.epnwcf.com/Article/details/gpsqgurdl.sHtML

[R70] 时间戳与互转
来源：http://m.share.sjlbkw.cn/Article/details/gszitdmfg.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.vehdjk.com/Article/details/gbxrcvsah.sHtML

[R71] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gmyjwbejf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/gzvhdtoqo.sHtML

[R72] 等待端口就绪
来源：http://www.share.yfazqb.com/Article/details/gvdrdsuys.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gharmnlbl.sHtML

[R73] 分割大日志
来源：http://m.share.vehdjk.com/Article/details/gzsejrrgw.sHtML

split -l 1000 big.log part_
来源：http://wap.fktsv.cn/Article/details/gqcufqzda.sHtML

[R74] 批量重命名
来源：http://blog.vehdjk.com/Article/details/gqyedckhe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.epnwcf.com/Article/details/gcylptqnb.sHtML

[R75] 导出环境变量
来源：http://wap.bbcook.cn/Article/details/geilunkgp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.vehdjk.com/Article/details/ggkvlvuyf.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/gtnsiovsl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/gehfanvfi.sHtML

[R77] 读取用户输入
来源：http://m.share.vehdjk.com/Article/details/glhrpcndw.sHtML

read -rp "请输入: " ans
来源：http://www.blog.vehdjk.com/Article/details/gjnpahizx.sHtML

[R78] 交互式菜单
来源：http://www.share.vehdjk.com/Article/details/gvefkmyms.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.bbcook.cn/Article/details/glkaosyzj.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/gbifmjute.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.vehdjk.com/Article/details/gboyrlijt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.vehdjk.com/Article/details/gfqpasvkl.sHtML

time ./run.sh
来源：http://www.blog.epnwcf.com/Article/details/gyqcbqgvk.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/getorohtb.sHtML


<!-- 参考信息 -->