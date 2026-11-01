代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.epnwcf.com/Article/details/gjlrjbqsv.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fktsv.cn/Article/details/gwiwdrmgt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gyxuvcwrt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.vehdjk.com/Article/details/gajugvojx.sHtML

[Q33] 多列分组
来源：http://read.share.yfazqb.com/Article/details/gyulygfuf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.epnwcf.com/Article/details/grdstvtdr.sHtML

[Q34] 每组取第一条
来源：http://wap.sjlbkw.cn/Article/details/gekbcqhpe.sHtML

SELECT * FROM (
来源：http://www.m.share.bbcook.cn/Article/details/gqsgmiubt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.epnwcf.com/Article/details/ggznibqic.sHtML

) t WHERE rn = 1;
来源：http://blog.yfazqb.com/Article/details/gdrmmohrv.sHtML

[Q35] 内连接
来源：http://www.share.sjlbkw.cn/Article/details/gcjowrrlf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/giypukxxy.sHtML

[Q36] 左连接
来源：http://m.share.fktsv.cn/Article/details/gjcdadjla.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/gciwvmqve.sHtML

[Q37] 右连接
来源：http://www.m.share.bbcook.cn/Article/details/gifzammck.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.tarul.cn/Article/details/gngipcnat.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.tarul.cn/Article/details/ghmrbjses.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.epnwcf.com/Article/details/gemntkxns.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.tarul.cn/Article/details/gacviwqub.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.bbcook.cn/Article/details/gqryojwkt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.tarul.cn/Article/details/gjmvjwiow.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.tarul.cn/Article/details/gqztzywsr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.epnwcf.com/Article/details/gfqfojuwq.sHtML

[Q41] 多表连接
来源：http://www.share.sjlbkw.cn/Article/details/gqueartas.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.tarul.cn/Article/details/gsevcbops.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.bbcook.cn/Article/details/gtuhxmbwr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fktsv.cn/Article/details/griynfjwf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gqdxltxvb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.epnwcf.com/Article/details/gqvjmifkh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.yfazqb.com/Article/details/ggiwzqxhf.sHtML

[Q43] 标量子查询
来源：http://3g.sjlbkw.cn/Article/details/gjzjjvqhx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.sjlbkw.cn/Article/details/gbzrgukjd.sHtML

[Q44] IN 子查询
来源：http://wap.fktsv.cn/Article/details/gqjdenbfk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.epnwcf.com/Article/details/gtjblzgjo.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.vehdjk.com/Article/details/gutofowpf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gurjfcmmj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.yfazqb.com/Article/details/ghsivrzqk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gmfsexhmu.sHtML

[Q47] 与平均值比较
来源：http://m.share.yfazqb.com/Article/details/gnbdtdyqa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.bbcook.cn/Article/details/ggidnxrdj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fktsv.cn/Article/details/glxgfnguj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fktsv.cn/Article/details/grfofebuo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.epnwcf.com/Article/details/gwmbzijdz.sHtML

[Q49] 更新单行
来源：http://read.share.epnwcf.com/Article/details/gaazwhtds.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/gdoxngdbj.sHtML

[Q50] 批量更新
来源：http://wap.epnwcf.com/Article/details/gojyhccxu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.sjlbkw.cn/Article/details/gpmrlwuto.sHtML

[Q51] 用子查询更新
来源：http://read.share.bbcook.cn/Article/details/gjhtvpjgl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gpfghthxl.sHtML

[Q52] 删除指定行
来源：http://baike.tarul.cn/Article/details/gwilfgwfz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gozrjgkux.sHtML

[Q53] 按条件删除
来源：http://baike.vehdjk.com/Article/details/gouweickq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.epnwcf.com/Article/details/grcrzieca.sHtML

[Q54] 清空表
来源：http://www.blog.bbcook.cn/Article/details/gxonvadeh.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.epnwcf.com/Article/details/gsutopkiy.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.sjlbkw.cn/Article/details/gikyirjaq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gajyqatnb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.vehdjk.com/Article/details/gnptfmhac.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.tarul.cn/Article/details/gaevvgxwv.sHtML

[Q57] 行号
来源：http://mobile.sjlbkw.cn/Article/details/gsaedppay.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gporfaaic.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/ghyiczxhx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/glvbwxeuc.sHtML

[Q59] 分组内累计
来源：http://wap.tarul.cn/Article/details/gljmmdwnj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/ghaqexylk.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.tarul.cn/Article/details/giheqowso.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.vehdjk.com/Article/details/gbxydxvcw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.yfazqb.com/Article/details/gwyzlkfaa.sHtML

[Q61] 移动平均
来源：http://baike.yfazqb.com/Article/details/guvqundry.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.tarul.cn/Article/details/gabxfpfqh.sHtML

[Q62] 分组占比
来源：http://read.share.yfazqb.com/Article/details/ghefkqhgo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gcgpmymnj.sHtML

[Q63] 开启事务
来源：http://www.share.bbcook.cn/Article/details/gryjywxku.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkgyskev.sHtML

[Q64] 提交事务
来源：http://mobile.vehdjk.com/Article/details/gsvbqtyrb.sHtML

COMMIT;
来源：http://blog.bbcook.cn/Article/details/gekxjsnng.sHtML

[Q65] 回滚事务
来源：http://blog.sjlbkw.cn/Article/details/gzfizegvp.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/garpmjxqo.sHtML

[Q66] 行锁查询
来源：http://3g.fktsv.cn/Article/details/gkrgkhxvp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fktsv.cn/Article/details/gdjvoavyh.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.yfazqb.com/Article/details/gubzpicnv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.vehdjk.com/Article/details/gxemznpgf.sHtML

[Q68] 保存点
来源：http://www.m.share.fktsv.cn/Article/details/gbjplgvye.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gvwkcohsh.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvjocdmx.sHtML

[Q69] 查看执行计划
来源：http://read.share.vehdjk.com/Article/details/gobwofjzo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.vehdjk.com/Article/details/gstrneotk.sHtML

[Q70] 更新统计信息
来源：http://blog.epnwcf.com/Article/details/gguznwciv.sHtML

ANALYZE TABLE users;
来源：http://baike.tarul.cn/Article/details/giwjdugdn.sHtML

[Q71] 查看建表语句
来源：http://3g.tarul.cn/Article/details/gmwgtkxbk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.sjlbkw.cn/Article/details/ghjkwabfy.sHtML

[Q72] 查看索引
来源：http://read.share.tarul.cn/Article/details/gbljzrica.sHtML

SHOW INDEX FROM users;
来源：http://mobile.bbcook.cn/Article/details/gpzosyoow.sHtML

[Q73] 查看表状态
来源：http://mobile.epnwcf.com/Article/details/gpgnziyrs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gemcokmjl.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.epnwcf.com/Article/details/gmbxcgawh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.vehdjk.com/Article/details/guwvgotif.sHtML

[Q75] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gpronhbwe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.epnwcf.com/Article/details/gcgzwloub.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.sjlbkw.cn/Article/details/gurkcgddv.sHtML

[Q76] 按天统计
来源：http://wap.fktsv.cn/Article/details/gxfcvejfi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.tarul.cn/Article/details/gkwfwbpca.sHtML

[Q77] 时间加减
来源：http://wap.bbcook.cn/Article/details/gkqitdzqw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.bbcook.cn/Article/details/gwomlztqd.sHtML

[Q78] 当前时间
来源：http://read.share.tarul.cn/Article/details/gdfjcdxlq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.epnwcf.com/Article/details/gpcpielfw.sHtML

[Q79] 字符串拼接
来源：http://wap.epnwcf.com/Article/details/gcvgldaqx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.sjlbkw.cn/Article/details/gyesvzwtn.sHtML

[Q80] 字符串截取
来源：http://read.share.sjlbkw.cn/Article/details/gwpviqbne.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gciqmqgyo.sHtML

[Q81] 字符串替换
来源：http://m.share.sjlbkw.cn/Article/details/gmmmgoglb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.tarul.cn/Article/details/gepijsnuk.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.epnwcf.com/Article/details/gvkjahfdr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gmknyrwzy.sHtML

[Q83] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/ghmvmhbzx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/gukfskjdt.sHtML

[Q84] 去除首尾空格
来源：http://3g.fktsv.cn/Article/details/gbfsnslbu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gujbvkyry.sHtML

[Q85] 数值取整
来源：http://wap.bbcook.cn/Article/details/gpuomjuwe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.yfazqb.com/Article/details/gdltxpfso.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.tarul.cn/Article/details/gkbesyiwg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.yfazqb.com/Article/details/gdegibper.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.tarul.cn/Article/details/gmeswbiwa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.yfazqb.com/Article/details/gbaszwgbl.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fktsv.cn/Article/details/gsuihjubi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.vehdjk.com/Article/details/gqsqmphht.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.tarul.cn/Article/details/goskytbfs.sHtML

[Q89] 判断表是否存在
来源：http://blog.yfazqb.com/Article/details/gfpdqjrvg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.vehdjk.com/Article/details/gozwtdviu.sHtML

[Q90] 生成序号列
来源：http://read.share.tarul.cn/Article/details/gsqmfwpbc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.yfazqb.com/Article/details/gmvhsgapr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gerabkikn.sHtML

R. Bash 专题
来源：http://www.share.epnwcf.com/Article/details/ghqoadtjc.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gsalakura.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.epnwcf.com/Article/details/gwzopalvz.sHtML

#!/usr/bin/env bash
来源：http://3g.sjlbkw.cn/Article/details/gelywefob.sHtML

set -euo pipefail
来源：http://www.share.epnwcf.com/Article/details/gtnuvjomb.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.yfazqb.com/Article/details/gibkwljxb.sHtML

name="Tom"; echo "$name"
来源：http://wap.vehdjk.com/Article/details/gfabcaeez.sHtML

[R03] 只读变量
来源：http://baike.bbcook.cn/Article/details/gvmpdksla.sHtML

readonly PI=3.14
来源：http://www.m.share.vehdjk.com/Article/details/gjhchuwbw.sHtML

[R04] 位置参数
来源：http://mobile.tarul.cn/Article/details/gcavvddnb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.sjlbkw.cn/Article/details/gqhillwmf.sHtML

[R05] 参数默认值
来源：http://read.share.tarul.cn/Article/details/gsqumvdsk.sHtML

name="${1:-default}"
来源：http://www.m.share.bbcook.cn/Article/details/gsbynmqza.sHtML

[R06] 判断命令是否存在
来源：http://wap.epnwcf.com/Article/details/gdzwepgll.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gwftvpubf.sHtML

[R07] if 判断文件
来源：http://read.share.yfazqb.com/Article/details/ghxfjvxhw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.vehdjk.com/Article/details/gqhsgfcfc.sHtML

[R08] 数值比较
来源：http://m.share.yfazqb.com/Article/details/gtaqxuzcu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.tarul.cn/Article/details/gwirvakxx.sHtML

[R09] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/gsipreajv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.tarul.cn/Article/details/gwhfxamyv.sHtML

[R10] 正则匹配
来源：http://3g.sjlbkw.cn/Article/details/gxfyfzvmx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.bbcook.cn/Article/details/gkilidqbz.sHtML

[R11] case 多分支
来源：http://www.m.share.bbcook.cn/Article/details/gkqtspyvy.sHtML

case "$1" in
来源：http://blog.yfazqb.com/Article/details/gjwahnvqr.sHtML

start) echo "启动" ;;
来源：http://blog.yfazqb.com/Article/details/gmfuwxetn.sHtML

stop)  echo "停止" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gnpfwsjms.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.tarul.cn/Article/details/gkkkgfmbw.sHtML

esac
来源：http://www.share.bbcook.cn/Article/details/gyojxfklc.sHtML

[R12] for 遍历文件
来源：http://www.blog.vehdjk.com/Article/details/gfqujjfzr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.yfazqb.com/Article/details/grfguoiei.sHtML

[R13] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gduzckvcg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmkdibfv.sHtML

[R14] C 风格 for
来源：http://www.share.tarul.cn/Article/details/gjhoisjmc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gpolkqgrx.sHtML

[R15] while 逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gcreshbbn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.vehdjk.com/Article/details/gcccelbaf.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/gchifecpg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gyxwcppam.sHtML

[R17] 数组定义与取值
来源：http://m.share.vehdjk.com/Article/details/ggfhchxke.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.yfazqb.com/Article/details/gxisqzjgw.sHtML

[R18] 遍历数组
来源：http://www.m.share.epnwcf.com/Article/details/gpvhaoikj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fktsv.cn/Article/details/gniwpkoby.sHtML

[R19] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gpncaavbh.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/gsdrppuph.sHtML

[R20] 关联数组（字典）
来源：http://3g.epnwcf.com/Article/details/gkozugljh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fktsv.cn/Article/details/glkvvnuve.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/gebpcuydd.sHtML

echo "${#s}"
来源：http://www.m.share.fktsv.cn/Article/details/gnxoprbzx.sHtML

[R22] 截取子串
来源：http://www.share.sjlbkw.cn/Article/details/gjzhopbte.sHtML

echo "${s:0:5}"
来源：http://wap.bbcook.cn/Article/details/gfmtaarmu.sHtML

[R23] 字符串替换
来源：http://3g.fktsv.cn/Article/details/gupncgppq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fktsv.cn/Article/details/gbszrwjuz.sHtML

[R24] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gwknuqrpw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.yfazqb.com/Article/details/gnyjwcowp.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fktsv.cn/Article/details/gqmhnqaxt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.tarul.cn/Article/details/gptrgcqiu.sHtML

[R26] 命令替换
来源：http://baike.fktsv.cn/Article/details/gnkfdtalw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.sjlbkw.cn/Article/details/gqjhfyaga.sHtML

[R27] 算术展开
来源：http://3g.fktsv.cn/Article/details/gnlntpnxq.sHtML

echo $((1 + 2 * 3))
来源：http://wap.tarul.cn/Article/details/gthopytsa.sHtML

[R28] 浮点运算
来源：http://wap.yfazqb.com/Article/details/gtfdzuwfz.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.tarul.cn/Article/details/ggxcqjrmk.sHtML

[R29] 定义函数
来源：http://3g.fktsv.cn/Article/details/gfvnxuoxx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.sjlbkw.cn/Article/details/gflvjzwpy.sHtML

[R30] 函数返回状态码
来源：http://www.share.bbcook.cn/Article/details/gpariaryf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.bbcook.cn/Article/details/ghyivhxez.sHtML

[R31] 局部变量
来源：http://3g.epnwcf.com/Article/details/gmvijnmgv.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.epnwcf.com/Article/details/gpajkoidv.sHtML

[R32] 参数个数校验
来源：http://m.share.epnwcf.com/Article/details/giesopijs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.sjlbkw.cn/Article/details/gxvbixbvm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.bbcook.cn/Article/details/gbrkdirjl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.yfazqb.com/Article/details/gmrcpdrje.sHtML

[R34] 退出时清理
来源：http://wap.yfazqb.com/Article/details/gghmlymsq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/gdzeuwvxb.sHtML

[R35] 后台执行并等待
来源：http://www.share.bbcook.cn/Article/details/gjdpavtyw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fktsv.cn/Article/details/gfwcusapm.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gbthrelgw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.vehdjk.com/Article/details/grjkrxvpb.sHtML

[R37] 把输出赋给变量
来源：http://m.share.vehdjk.com/Article/details/gplnxtaan.sHtML

files=$(ls -1)
来源：http://mobile.fktsv.cn/Article/details/geosjwcrm.sHtML

[R38] 管道串联
来源：http://www.m.share.yfazqb.com/Article/details/gkqfuarbp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.epnwcf.com/Article/details/gzmjmmgmk.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.yfazqb.com/Article/details/gqokfqjai.sHtML

cmd > out.log 2>&1
来源：http://mobile.epnwcf.com/Article/details/gvunpfmgg.sHtML

[R40] 追加写日志
来源：http://read.share.sjlbkw.cn/Article/details/gqhcwpmpm.sHtML

echo "log" >> out.log
来源：http://mobile.tarul.cn/Article/details/gquxaieqt.sHtML

[R41] 丢弃输出
来源：http://www.blog.vehdjk.com/Article/details/ggibacadw.sHtML

cmd >/dev/null 2>&1
来源：http://3g.epnwcf.com/Article/details/gwvcjfjhq.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/gshjxonuf.sHtML

wc -l < a.txt
来源：http://baike.epnwcf.com/Article/details/gblhjuyks.sHtML

[R43] 按名字查找文件
来源：http://www.share.tarul.cn/Article/details/gnlpugkqe.sHtML

find . -name "*.log" -type f
来源：http://blog.yfazqb.com/Article/details/gqqktpdbm.sHtML

[R44] 按修改时间查找
来源：http://www.blog.sjlbkw.cn/Article/details/gqwzcwrol.sHtML

find . -mtime -7 -type f
来源：http://mobile.vehdjk.com/Article/details/gpwjsghsj.sHtML

[R45] 批量删除
来源：http://blog.vehdjk.com/Article/details/gwppdsajm.sHtML

find . -name "*.tmp" -delete
来源：http://blog.vehdjk.com/Article/details/grjkhwujv.sHtML

[R46] 递归替换文件内容
来源：http://wap.sjlbkw.cn/Article/details/ghbvuomom.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.sjlbkw.cn/Article/details/gfdwspacw.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/gxjxkkmbq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fktsv.cn/Article/details/gjbvuumsv.sHtML

[R48] awk 取指定列
来源：http://wap.vehdjk.com/Article/details/gvvpxaipc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gqjimkhmv.sHtML

[R49] awk 带条件
来源：http://www.share.bbcook.cn/Article/details/gjmazzwdo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.yfazqb.com/Article/details/goyviupyh.sHtML

[R50] awk 求和
来源：http://www.share.vehdjk.com/Article/details/gslnhwkto.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gvzblaazd.sHtML

[R51] 排序去重取前几
来源：http://mobile.tarul.cn/Article/details/gwtzdprlv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/gxqsxpsao.sHtML

[R52] 统计行数
来源：http://mobile.vehdjk.com/Article/details/gqeckyqvo.sHtML

wc -l a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gchbbebqv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fktsv.cn/Article/details/gegbxhkam.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.tarul.cn/Article/details/gwsgmpiqk.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/gniipysjk.sHtML

diff a.txt b.txt
来源：http://wap.fktsv.cn/Article/details/golookkfh.sHtML

[R55] 压缩与解压
来源：http://www.blog.fktsv.cn/Article/details/gmgjmoqen.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.epnwcf.com/Article/details/gahumwakc.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/gqjrcxoas.sHtML

scp file user@host:/path/
来源：http://3g.vehdjk.com/Article/details/gspwqrlgb.sHtML

[R57] 远程执行命令
来源：http://mobile.tarul.cn/Article/details/gsuqlusxy.sHtML

ssh user@host 'uptime'
来源：http://www.share.tarul.cn/Article/details/ggtbffurb.sHtML

[R58] 下载文件
来源：http://blog.yfazqb.com/Article/details/gdpmkwvcw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.epnwcf.com/Article/details/gnrhtaajz.sHtML

[R59] 发 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gxfpgtxes.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.epnwcf.com/Article/details/gysiuggdb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gqrdvppjt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.bbcook.cn/Article/details/gtkoblggp.sHtML

[R61] 磁盘占用
来源：http://www.share.sjlbkw.cn/Article/details/gqtidhamz.sHtML

df -h;  du -sh *
来源：http://www.m.share.sjlbkw.cn/Article/details/gigplidss.sHtML

[R62] 找最占空间的文件
来源：http://baike.sjlbkw.cn/Article/details/gyrivehic.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fktsv.cn/Article/details/gqhinxyzs.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gppjivysk.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.tarul.cn/Article/details/gdnjqqutq.sHtML

[R64] 结束进程
来源：http://www.share.sjlbkw.cn/Article/details/gqcytvcwf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.yfazqb.com/Article/details/gfnwyzmzs.sHtML

[R65] 查看端口占用
来源：http://mobile.epnwcf.com/Article/details/gzlpvpoik.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fktsv.cn/Article/details/gkbwkefcr.sHtML

[R66] 定时任务
来源：http://www.share.epnwcf.com/Article/details/gucxwomqj.sHtML

crontab -e;  crontab -l
来源：http://read.share.tarul.cn/Article/details/gojizpfst.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.sjlbkw.cn/Article/details/gknjyufsa.sHtML

openssl rand -hex 16
来源：http://m.share.bbcook.cn/Article/details/gauifrdlc.sHtML

[R68] 计算文件校验值
来源：http://m.share.epnwcf.com/Article/details/gldhqlpvy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.vehdjk.com/Article/details/gymatwaji.sHtML

[R69] 生成随机密码
来源：http://baike.vehdjk.com/Article/details/gynrcfjez.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.yfazqb.com/Article/details/gkxkudgpv.sHtML

[R70] 时间戳与互转
来源：http://m.share.fktsv.cn/Article/details/gxvkbsjfm.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.bbcook.cn/Article/details/gjzrxsowo.sHtML

[R71] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gowuglpxk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.bbcook.cn/Article/details/gosigyquo.sHtML

[R72] 等待端口就绪
来源：http://baike.epnwcf.com/Article/details/gocxzjrfj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gpbjrqsqg.sHtML

[R73] 分割大日志
来源：http://blog.tarul.cn/Article/details/gygtkivao.sHtML

split -l 1000 big.log part_
来源：http://wap.epnwcf.com/Article/details/gbylxguso.sHtML

[R74] 批量重命名
来源：http://www.m.share.tarul.cn/Article/details/gafscdgwh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fktsv.cn/Article/details/gscjnssgx.sHtML

[R75] 导出环境变量
来源：http://www.share.tarul.cn/Article/details/gdnshdixz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.tarul.cn/Article/details/grhxpfuqs.sHtML

[R76] 使用临时文件
来源：http://mobile.yfazqb.com/Article/details/gvrjmkxsd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gaxzwxcww.sHtML

[R77] 读取用户输入
来源：http://3g.epnwcf.com/Article/details/gtojnmjzp.sHtML

read -rp "请输入: " ans
来源：http://www.share.vehdjk.com/Article/details/gytqyubwt.sHtML

[R78] 交互式菜单
来源：http://www.blog.yfazqb.com/Article/details/gdnfouqxj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.epnwcf.com/Article/details/gnczjcqso.sHtML

[R79] 解析命令行选项
来源：http://blog.bbcook.cn/Article/details/gogjwsjen.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.epnwcf.com/Article/details/grutvskjm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fktsv.cn/Article/details/geecvfbsm.sHtML

time ./run.sh
来源：http://3g.sjlbkw.cn/Article/details/gtfqvjebf.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghsrieeko.sHtML


<!-- 参考信息 -->