代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fktsv.cn/Article/details/gkzkfxjhv.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fktsv.cn/Article/details/grbslusrc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/ghkkwciaz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.yfazqb.com/Article/details/gtozaewrv.sHtML

[Q33] 多列分组
来源：http://baike.epnwcf.com/Article/details/gpkakeacv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.epnwcf.com/Article/details/gvjaxfvtj.sHtML

[Q34] 每组取第一条
来源：http://m.share.fktsv.cn/Article/details/gfoyhyqkz.sHtML

SELECT * FROM (
来源：http://read.share.bbcook.cn/Article/details/gnekxkjgp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.bbcook.cn/Article/details/gchqecjkr.sHtML

) t WHERE rn = 1;
来源：http://blog.tarul.cn/Article/details/gdlvepdos.sHtML

[Q35] 内连接
来源：http://read.share.sjlbkw.cn/Article/details/gbormtmzn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gmsykchhq.sHtML

[Q36] 左连接
来源：http://www.m.share.yfazqb.com/Article/details/gwjymdqfk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/gvbegfzmf.sHtML

[Q37] 右连接
来源：http://read.share.bbcook.cn/Article/details/gllnueqna.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fktsv.cn/Article/details/gtoiawezr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.yfazqb.com/Article/details/gnbtlgccj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.sjlbkw.cn/Article/details/gbrfcahek.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.bbcook.cn/Article/details/gruqjjcqg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fktsv.cn/Article/details/gjhxkqvar.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.bbcook.cn/Article/details/gsznpxhzb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fktsv.cn/Article/details/gcdhbiubp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.vehdjk.com/Article/details/gjpwmkmof.sHtML

[Q41] 多表连接
来源：http://baike.vehdjk.com/Article/details/grcqwdbke.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.tarul.cn/Article/details/gkxnasjbs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.tarul.cn/Article/details/ghlwwotet.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.sjlbkw.cn/Article/details/gvalsfphl.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fktsv.cn/Article/details/gtyjugmtx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.bbcook.cn/Article/details/gyghpqeho.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.sjlbkw.cn/Article/details/grydwtubw.sHtML

[Q43] 标量子查询
来源：http://www.share.vehdjk.com/Article/details/gqmjzxehk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.bbcook.cn/Article/details/gwltbahuc.sHtML

[Q44] IN 子查询
来源：http://www.m.share.vehdjk.com/Article/details/gcweopzje.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.vehdjk.com/Article/details/gtaviimle.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.bbcook.cn/Article/details/gjenqkmnc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gomqwxbve.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.sjlbkw.cn/Article/details/ghsrzawfd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/gngpwtnsl.sHtML

[Q47] 与平均值比较
来源：http://blog.sjlbkw.cn/Article/details/gwvpjmmxa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.bbcook.cn/Article/details/gqkljezbn.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.yfazqb.com/Article/details/gmkgiaune.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.vehdjk.com/Article/details/genvxzafz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.tarul.cn/Article/details/gptvihexz.sHtML

[Q49] 更新单行
来源：http://www.m.share.tarul.cn/Article/details/grfxhagst.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gqpjjmusu.sHtML

[Q50] 批量更新
来源：http://read.share.epnwcf.com/Article/details/gzyarandb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.yfazqb.com/Article/details/geceqgvhf.sHtML

[Q51] 用子查询更新
来源：http://baike.sjlbkw.cn/Article/details/gbpddobat.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.yfazqb.com/Article/details/gejqnpdhm.sHtML

[Q52] 删除指定行
来源：http://3g.sjlbkw.cn/Article/details/ginwsxigo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/gljelugib.sHtML

[Q53] 按条件删除
来源：http://www.share.vehdjk.com/Article/details/gvpxigoha.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fktsv.cn/Article/details/guextvgcl.sHtML

[Q54] 清空表
来源：http://blog.fktsv.cn/Article/details/gjncdcqvm.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fktsv.cn/Article/details/ggmaiedgd.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.vehdjk.com/Article/details/gcgwbucit.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gkbdcwomo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.yfazqb.com/Article/details/gwefmurba.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.tarul.cn/Article/details/ggvwgzbzv.sHtML

[Q57] 行号
来源：http://m.share.sjlbkw.cn/Article/details/gwevttviu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.tarul.cn/Article/details/gqwijsltf.sHtML

[Q58] 累计求和
来源：http://mobile.bbcook.cn/Article/details/gvybmsfly.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.vehdjk.com/Article/details/ghgsoilcp.sHtML

[Q59] 分组内累计
来源：http://3g.bbcook.cn/Article/details/gxihrvwso.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/ggvaqnawh.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.yfazqb.com/Article/details/gutfylern.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.yfazqb.com/Article/details/gcsptedhj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.tarul.cn/Article/details/gpmgktddr.sHtML

[Q61] 移动平均
来源：http://www.share.sjlbkw.cn/Article/details/gpjsgeflm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gcocwfolr.sHtML

[Q62] 分组占比
来源：http://www.share.tarul.cn/Article/details/ggwyrbsjz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gdllkaakl.sHtML

[Q63] 开启事务
来源：http://www.m.share.fktsv.cn/Article/details/geazahqit.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.epnwcf.com/Article/details/ghhlatckf.sHtML

[Q64] 提交事务
来源：http://3g.fktsv.cn/Article/details/gkgwkpbgm.sHtML

COMMIT;
来源：http://wap.tarul.cn/Article/details/gbzjapnwt.sHtML

[Q65] 回滚事务
来源：http://www.m.share.tarul.cn/Article/details/gfwblhrwi.sHtML

ROLLBACK;
来源：http://www.m.share.tarul.cn/Article/details/geligkqeo.sHtML

[Q66] 行锁查询
来源：http://mobile.vehdjk.com/Article/details/gadmvsyfl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.yfazqb.com/Article/details/giiopooaf.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fktsv.cn/Article/details/gfsgwngtk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.tarul.cn/Article/details/gzypztxwc.sHtML

[Q68] 保存点
来源：http://www.blog.tarul.cn/Article/details/gyuxdbcfs.sHtML

SAVEPOINT sp1;
来源：http://3g.vehdjk.com/Article/details/gpbazdxpp.sHtML

ROLLBACK TO sp1;
来源：http://3g.fktsv.cn/Article/details/gacdzgjmi.sHtML

[Q69] 查看执行计划
来源：http://blog.bbcook.cn/Article/details/gnaczjeyp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fktsv.cn/Article/details/guewcrwyo.sHtML

[Q70] 更新统计信息
来源：http://www.share.tarul.cn/Article/details/gwxztubwb.sHtML

ANALYZE TABLE users;
来源：http://www.blog.vehdjk.com/Article/details/gufhnjhbn.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fktsv.cn/Article/details/gviiokvme.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.epnwcf.com/Article/details/giaqchoiu.sHtML

[Q72] 查看索引
来源：http://mobile.epnwcf.com/Article/details/gtmdmwjjy.sHtML

SHOW INDEX FROM users;
来源：http://3g.epnwcf.com/Article/details/gacndlcxb.sHtML

[Q73] 查看表状态
来源：http://www.blog.sjlbkw.cn/Article/details/gngzfvvyo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.tarul.cn/Article/details/grrhdajjk.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fktsv.cn/Article/details/gmacqrjky.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.epnwcf.com/Article/details/gfzmivllc.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gvadnvdhw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.tarul.cn/Article/details/gsslvjwhx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.sjlbkw.cn/Article/details/gxhcbfxur.sHtML

[Q76] 按天统计
来源：http://blog.fktsv.cn/Article/details/gtmpbethz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.vehdjk.com/Article/details/gusixiqde.sHtML

[Q77] 时间加减
来源：http://baike.fktsv.cn/Article/details/grgfwfyoo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.yfazqb.com/Article/details/gyeypooww.sHtML

[Q78] 当前时间
来源：http://blog.sjlbkw.cn/Article/details/gonazakbx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.vehdjk.com/Article/details/goxjcdura.sHtML

[Q79] 字符串拼接
来源：http://blog.vehdjk.com/Article/details/gcidyvehg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.tarul.cn/Article/details/gvqvwmrxi.sHtML

[Q80] 字符串截取
来源：http://wap.yfazqb.com/Article/details/gwiydyhyv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gwwnhtcfp.sHtML

[Q81] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/guzyxaqza.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gdsuqhqwu.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.epnwcf.com/Article/details/godatoumc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gqoqdcgti.sHtML

[Q83] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gbxaypfst.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gykefktfr.sHtML

[Q84] 去除首尾空格
来源：http://3g.sjlbkw.cn/Article/details/gkjztfojx.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gwgnuzfna.sHtML

[Q85] 数值取整
来源：http://www.m.share.bbcook.cn/Article/details/giqzydylc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.yfazqb.com/Article/details/gjzsqawbb.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.yfazqb.com/Article/details/gjdrsxhtm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.epnwcf.com/Article/details/gsnkfspev.sHtML

[Q87] JSON 字段做条件
来源：http://blog.vehdjk.com/Article/details/ggpatdfgq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.bbcook.cn/Article/details/gtrbxhyyq.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.epnwcf.com/Article/details/goemhfitr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.epnwcf.com/Article/details/gvqygguje.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.tarul.cn/Article/details/gsjcpsspq.sHtML

[Q89] 判断表是否存在
来源：http://blog.sjlbkw.cn/Article/details/gftfpcjkv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/geybcnycj.sHtML

[Q90] 生成序号列
来源：http://blog.bbcook.cn/Article/details/gtxxgifuj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.yfazqb.com/Article/details/gyljjfhxx.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gydksvpei.sHtML

R. Bash 专题
来源：http://wap.epnwcf.com/Article/details/gxsuaycjf.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gdysufsog.sHtML

[R01] shebang 与严格模式
来源：http://blog.vehdjk.com/Article/details/guvchosqw.sHtML

#!/usr/bin/env bash
来源：http://www.share.fktsv.cn/Article/details/gltbfyivz.sHtML

set -euo pipefail
来源：http://www.blog.yfazqb.com/Article/details/gahhhmnhz.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.yfazqb.com/Article/details/ggarrjwhb.sHtML

name="Tom"; echo "$name"
来源：http://3g.bbcook.cn/Article/details/gibhkvsxg.sHtML

[R03] 只读变量
来源：http://blog.bbcook.cn/Article/details/gjqouhdfh.sHtML

readonly PI=3.14
来源：http://blog.sjlbkw.cn/Article/details/ghfwpszkw.sHtML

[R04] 位置参数
来源：http://read.share.fktsv.cn/Article/details/gifgkrfnx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.yfazqb.com/Article/details/gdfhdoupb.sHtML

[R05] 参数默认值
来源：http://3g.fktsv.cn/Article/details/gabkscnwh.sHtML

name="${1:-default}"
来源：http://www.m.share.fktsv.cn/Article/details/gorqkhhgd.sHtML

[R06] 判断命令是否存在
来源：http://wap.bbcook.cn/Article/details/gruxhtxdc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gkbhhxuke.sHtML

[R07] if 判断文件
来源：http://mobile.tarul.cn/Article/details/glyuxorac.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fktsv.cn/Article/details/goskfcxir.sHtML

[R08] 数值比较
来源：http://m.share.fktsv.cn/Article/details/gypzrwjyt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fktsv.cn/Article/details/gfkvouhqx.sHtML

[R09] 字符串比较
来源：http://3g.bbcook.cn/Article/details/ghdipvxzj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.bbcook.cn/Article/details/gwazshzcf.sHtML

[R10] 正则匹配
来源：http://www.blog.bbcook.cn/Article/details/grksondvi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.sjlbkw.cn/Article/details/gbczzppfi.sHtML

[R11] case 多分支
来源：http://www.blog.bbcook.cn/Article/details/gqpnekrtx.sHtML

case "$1" in
来源：http://read.share.tarul.cn/Article/details/gevdzslfj.sHtML

start) echo "启动" ;;
来源：http://m.share.vehdjk.com/Article/details/gajchwevz.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fktsv.cn/Article/details/gatjtmwez.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.yfazqb.com/Article/details/gtxgfcdee.sHtML

esac
来源：http://3g.fktsv.cn/Article/details/gwitpaihk.sHtML

[R12] for 遍历文件
来源：http://www.m.share.bbcook.cn/Article/details/gmrdineuv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.sjlbkw.cn/Article/details/gfvueciyz.sHtML

[R13] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gavcszwml.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/glrwrjfro.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/gjqatmedk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gbrfjbqoh.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gezlhleoy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fktsv.cn/Article/details/gfsfoynwh.sHtML

[R16] until 等待条件
来源：http://blog.tarul.cn/Article/details/gpmsykjlk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gfeknavxq.sHtML

[R17] 数组定义与取值
来源：http://mobile.sjlbkw.cn/Article/details/guvnlwyei.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fktsv.cn/Article/details/gheytqynq.sHtML

[R18] 遍历数组
来源：http://www.share.epnwcf.com/Article/details/gegarmchx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.yfazqb.com/Article/details/glgmlpaoo.sHtML

[R19] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gipzlqzjr.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/grngjcook.sHtML

[R20] 关联数组（字典）
来源：http://baike.fktsv.cn/Article/details/gpsaadkfm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fktsv.cn/Article/details/ghjfzpuxt.sHtML

[R21] 字符串长度
来源：http://www.share.epnwcf.com/Article/details/grjualswh.sHtML

echo "${#s}"
来源：http://read.share.epnwcf.com/Article/details/gsvvlxjza.sHtML

[R22] 截取子串
来源：http://wap.epnwcf.com/Article/details/ggmvwefoh.sHtML

echo "${s:0:5}"
来源：http://www.share.vehdjk.com/Article/details/gyqudifah.sHtML

[R23] 字符串替换
来源：http://wap.bbcook.cn/Article/details/gafcpgurq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.sjlbkw.cn/Article/details/gapmatxlx.sHtML

[R24] 大小写转换
来源：http://3g.tarul.cn/Article/details/gquyguivb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fktsv.cn/Article/details/guslenfkl.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.sjlbkw.cn/Article/details/gmqpcqkgf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.tarul.cn/Article/details/gduusliks.sHtML

[R26] 命令替换
来源：http://baike.tarul.cn/Article/details/gokewklbq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.yfazqb.com/Article/details/gueassjvf.sHtML

[R27] 算术展开
来源：http://read.share.yfazqb.com/Article/details/gkzbrxqqx.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.vehdjk.com/Article/details/guqvyjvtj.sHtML

[R28] 浮点运算
来源：http://3g.fktsv.cn/Article/details/gjkdzwflk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/ghwnonudr.sHtML

[R29] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gjjektqdo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.vehdjk.com/Article/details/geakpsxsk.sHtML

[R30] 函数返回状态码
来源：http://blog.fktsv.cn/Article/details/gwjsorutg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.tarul.cn/Article/details/ggnpwxsaq.sHtML

[R31] 局部变量
来源：http://blog.bbcook.cn/Article/details/gokkmhwvr.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.vehdjk.com/Article/details/gaiewvlro.sHtML

[R32] 参数个数校验
来源：http://m.share.vehdjk.com/Article/details/gvtgwnyio.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gcelvivbn.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.yfazqb.com/Article/details/gbolgrimz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.epnwcf.com/Article/details/glinceshq.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/gpmpoixxw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gtxahtpgb.sHtML

[R35] 后台执行并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gkswessgr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.epnwcf.com/Article/details/gxefzitqg.sHtML

[R36] 并发执行多个任务
来源：http://3g.bbcook.cn/Article/details/gusckwrjx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.tarul.cn/Article/details/gsleixgda.sHtML

[R37] 把输出赋给变量
来源：http://mobile.yfazqb.com/Article/details/gsmugfxok.sHtML

files=$(ls -1)
来源：http://read.share.sjlbkw.cn/Article/details/gkbrfmlsz.sHtML

[R38] 管道串联
来源：http://www.share.tarul.cn/Article/details/gmpqugcou.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.vehdjk.com/Article/details/gewsqrkbg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.tarul.cn/Article/details/gngcpwkvf.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/gqeflmlla.sHtML

[R40] 追加写日志
来源：http://www.m.share.yfazqb.com/Article/details/gyskledzb.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/gubglodam.sHtML

[R41] 丢弃输出
来源：http://mobile.bbcook.cn/Article/details/gyfmqqrdh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.vehdjk.com/Article/details/gphiwbzmx.sHtML

[R42] 输入重定向
来源：http://wap.sjlbkw.cn/Article/details/gazqnjykk.sHtML

wc -l < a.txt
来源：http://baike.epnwcf.com/Article/details/gqtiracdu.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/gtgnwkmpf.sHtML

find . -name "*.log" -type f
来源：http://wap.vehdjk.com/Article/details/gohxyejvq.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.epnwcf.com/Article/details/gyzcdyzln.sHtML

find . -mtime -7 -type f
来源：http://read.share.fktsv.cn/Article/details/gplqirjrh.sHtML

[R45] 批量删除
来源：http://wap.fktsv.cn/Article/details/gkuoqmrrs.sHtML

find . -name "*.tmp" -delete
来源：http://blog.bbcook.cn/Article/details/gyjydknqm.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.yfazqb.com/Article/details/gsgyuqrgr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.tarul.cn/Article/details/gjtfwokwh.sHtML

[R47] sed 单行替换
来源：http://wap.vehdjk.com/Article/details/gjwtjuyif.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.epnwcf.com/Article/details/gviazzzlv.sHtML

[R48] awk 取指定列
来源：http://wap.fktsv.cn/Article/details/gmrsyvnju.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.tarul.cn/Article/details/ggbwffqjr.sHtML

[R49] awk 带条件
来源：http://m.share.tarul.cn/Article/details/glsyoxvik.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.bbcook.cn/Article/details/gyfwharpb.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/grftmichd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fktsv.cn/Article/details/ghsombbbn.sHtML

[R51] 排序去重取前几
来源：http://3g.bbcook.cn/Article/details/gkglymrss.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.vehdjk.com/Article/details/gigdfbwmm.sHtML

[R52] 统计行数
来源：http://mobile.fktsv.cn/Article/details/gisyhyfpq.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/gknlvrqkr.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/gsprxfvmf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.bbcook.cn/Article/details/gaolcaqlh.sHtML

[R54] 比较两个文件
来源：http://www.share.sjlbkw.cn/Article/details/ggdpbybll.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/gpfvxowhl.sHtML

[R55] 压缩与解压
来源：http://www.share.epnwcf.com/Article/details/gbwxgkeoc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fktsv.cn/Article/details/gaqzclsgm.sHtML

[R56] 远程拷贝
来源：http://3g.tarul.cn/Article/details/gsprxuwyw.sHtML

scp file user@host:/path/
来源：http://www.blog.yfazqb.com/Article/details/gjnlcetbl.sHtML

[R57] 远程执行命令
来源：http://3g.yfazqb.com/Article/details/gunwuttoe.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gkterefqj.sHtML

[R58] 下载文件
来源：http://read.share.bbcook.cn/Article/details/gjhxmymbd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.sjlbkw.cn/Article/details/gcmrjmhzp.sHtML

[R59] 发 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gypvvalvr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.vehdjk.com/Article/details/gvnrsedwb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/gjknvwkxx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fktsv.cn/Article/details/gyvojdwyc.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/gdjatycsu.sHtML

df -h;  du -sh *
来源：http://baike.sjlbkw.cn/Article/details/gitgfsiyr.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fktsv.cn/Article/details/gzrncqudy.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fktsv.cn/Article/details/gokwrxsyn.sHtML

[R63] 内存与进程
来源：http://www.m.share.yfazqb.com/Article/details/guxiewfsm.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.epnwcf.com/Article/details/gtmxvykua.sHtML

[R64] 结束进程
来源：http://blog.sjlbkw.cn/Article/details/gsnwoqtxz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.yfazqb.com/Article/details/gdudniind.sHtML

[R65] 查看端口占用
来源：http://www.m.share.tarul.cn/Article/details/gkpbjrxrz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.yfazqb.com/Article/details/gufzglget.sHtML

[R66] 定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/gyzyaacjk.sHtML

crontab -e;  crontab -l
来源：http://mobile.tarul.cn/Article/details/gqcqiawne.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.epnwcf.com/Article/details/govrlrqvn.sHtML

openssl rand -hex 16
来源：http://wap.epnwcf.com/Article/details/gjvfqntxc.sHtML

[R68] 计算文件校验值
来源：http://www.share.sjlbkw.cn/Article/details/ghhldmuxd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/gflocsctu.sHtML

[R69] 生成随机密码
来源：http://read.share.sjlbkw.cn/Article/details/gkyyvnpyf.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.sjlbkw.cn/Article/details/ghdhqnzvj.sHtML

[R70] 时间戳与互转
来源：http://read.share.tarul.cn/Article/details/gdbuwxclb.sHtML

date +%s;  date -d @1700000000
来源：http://blog.bbcook.cn/Article/details/gsitnjdaf.sHtML

[R71] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/grjrxprya.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/gjaycujht.sHtML

[R72] 等待端口就绪
来源：http://www.share.tarul.cn/Article/details/gsokorqyq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gidglkthz.sHtML

[R73] 分割大日志
来源：http://3g.bbcook.cn/Article/details/gowpmljka.sHtML

split -l 1000 big.log part_
来源：http://read.share.bbcook.cn/Article/details/gwrgrwxtp.sHtML

[R74] 批量重命名
来源：http://www.blog.epnwcf.com/Article/details/gnqkvdlzf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.tarul.cn/Article/details/gqiyqggmm.sHtML

[R75] 导出环境变量
来源：http://www.blog.bbcook.cn/Article/details/gbhporxnj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.bbcook.cn/Article/details/gzqhgmbcj.sHtML

[R76] 使用临时文件
来源：http://mobile.epnwcf.com/Article/details/gdducubve.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/gooiryrfr.sHtML

[R77] 读取用户输入
来源：http://www.share.fktsv.cn/Article/details/gyswjwsls.sHtML

read -rp "请输入: " ans
来源：http://blog.fktsv.cn/Article/details/ghotsdofn.sHtML

[R78] 交互式菜单
来源：http://mobile.yfazqb.com/Article/details/gdlixvule.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.yfazqb.com/Article/details/ghpobkbnd.sHtML

[R79] 解析命令行选项
来源：http://wap.yfazqb.com/Article/details/gfjjhzcia.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.tarul.cn/Article/details/gkbnzckid.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.tarul.cn/Article/details/gmxvqiadk.sHtML

time ./run.sh
来源：http://baike.fktsv.cn/Article/details/glkcohwsk.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gweypdgdv.sHtML


<!-- 参考信息 -->