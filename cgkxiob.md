代发 wailian999

[Q36] 左连接
来源：http://wap.vehdjk.com/Article/details/giyhdcsit.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gmdrprtqa.sHtML

[Q37] 右连接
来源：http://m.share.epnwcf.com/Article/details/gklozegjs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.bbcook.cn/Article/details/gdwqofnkr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.yfazqb.com/Article/details/gxqdokvgb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.tarul.cn/Article/details/gqmknikcm.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.yfazqb.com/Article/details/gaxgmrufq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.bbcook.cn/Article/details/ggyfuiynf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fktsv.cn/Article/details/gncmpequq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.sjlbkw.cn/Article/details/grbpabhdq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.epnwcf.com/Article/details/grkizkxfj.sHtML

[Q41] 多表连接
来源：http://wap.epnwcf.com/Article/details/gxrbtssya.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.vehdjk.com/Article/details/gpnmwrmbv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fktsv.cn/Article/details/grbrxvxrs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fktsv.cn/Article/details/ggtlcajgz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.bbcook.cn/Article/details/gihcvmanu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/gmqbliuiz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.bbcook.cn/Article/details/gxxnjswck.sHtML

[Q43] 标量子查询
来源：http://blog.tarul.cn/Article/details/gkdfywsxu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fktsv.cn/Article/details/gasgmgvih.sHtML

[Q44] IN 子查询
来源：http://read.share.vehdjk.com/Article/details/gzgdqckvp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.vehdjk.com/Article/details/gpefjaytb.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fktsv.cn/Article/details/gamkcxyry.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/gwltfknzx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.vehdjk.com/Article/details/gzoysmlpt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/gsjrmmhkv.sHtML

[Q47] 与平均值比较
来源：http://mobile.yfazqb.com/Article/details/gjbehpstz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fktsv.cn/Article/details/gtaiwejyy.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.vehdjk.com/Article/details/gvbmnhpsb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.sjlbkw.cn/Article/details/gnelnzeeq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.sjlbkw.cn/Article/details/gijutjtmt.sHtML

[Q49] 更新单行
来源：http://www.share.tarul.cn/Article/details/gidbwdugl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gytvrpovv.sHtML

[Q50] 批量更新
来源：http://m.share.bbcook.cn/Article/details/gyrcgfdds.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.epnwcf.com/Article/details/gzjkrvoil.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.epnwcf.com/Article/details/gifsucugf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.epnwcf.com/Article/details/glxfqaovf.sHtML

[Q52] 删除指定行
来源：http://read.share.epnwcf.com/Article/details/gthppuchi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/gulsmeuze.sHtML

[Q53] 按条件删除
来源：http://m.share.sjlbkw.cn/Article/details/gctsmuxja.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.bbcook.cn/Article/details/glrjjceee.sHtML

[Q54] 清空表
来源：http://www.share.bbcook.cn/Article/details/gzqtueese.sHtML

TRUNCATE TABLE logs;
来源：http://wap.yfazqb.com/Article/details/gotaydrdn.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fktsv.cn/Article/details/gjtxkceta.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/gbyzvdwly.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.yfazqb.com/Article/details/giatiapmm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/gxmzvdkve.sHtML

[Q57] 行号
来源：http://mobile.sjlbkw.cn/Article/details/gjreryzkh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.tarul.cn/Article/details/gzxvklsbp.sHtML

[Q58] 累计求和
来源：http://blog.epnwcf.com/Article/details/gmfcszoqz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gdibvufgw.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fktsv.cn/Article/details/gtxocuikm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gblesythr.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.yfazqb.com/Article/details/gyoexjgjb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fktsv.cn/Article/details/ghclvukpu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbgerdmb.sHtML

[Q61] 移动平均
来源：http://3g.epnwcf.com/Article/details/gvgbnmvpf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/ggpzbbffp.sHtML

[Q62] 分组占比
来源：http://baike.bbcook.cn/Article/details/gikefrrpc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gidfzlpvh.sHtML

[Q63] 开启事务
来源：http://mobile.vehdjk.com/Article/details/gbkhatoxz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.sjlbkw.cn/Article/details/gbzxmwaxw.sHtML

[Q64] 提交事务
来源：http://baike.fktsv.cn/Article/details/gnlmbtmik.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/gltzyccyg.sHtML

[Q65] 回滚事务
来源：http://m.share.epnwcf.com/Article/details/gipupvemb.sHtML

ROLLBACK;
来源：http://www.m.share.epnwcf.com/Article/details/gupncbkwf.sHtML

[Q66] 行锁查询
来源：http://read.share.fktsv.cn/Article/details/gbnzvonkd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.tarul.cn/Article/details/gianxeffm.sHtML

[Q67] 设置隔离级别
来源：http://3g.yfazqb.com/Article/details/gvmkpmwgp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.vehdjk.com/Article/details/gqgshzmnv.sHtML

[Q68] 保存点
来源：http://mobile.yfazqb.com/Article/details/gxmptkqna.sHtML

SAVEPOINT sp1;
来源：http://m.share.yfazqb.com/Article/details/gysmijzov.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fktsv.cn/Article/details/ganpgemqx.sHtML

[Q69] 查看执行计划
来源：http://baike.sjlbkw.cn/Article/details/gedlykjph.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.epnwcf.com/Article/details/gccpptgyf.sHtML

[Q70] 更新统计信息
来源：http://blog.sjlbkw.cn/Article/details/giccoosvs.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fktsv.cn/Article/details/gzkavtian.sHtML

[Q71] 查看建表语句
来源：http://m.share.yfazqb.com/Article/details/gvedzbvjw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.epnwcf.com/Article/details/gogigqbzz.sHtML

[Q72] 查看索引
来源：http://m.share.tarul.cn/Article/details/gvtdduupg.sHtML

SHOW INDEX FROM users;
来源：http://read.share.vehdjk.com/Article/details/gqtuxixht.sHtML

[Q73] 查看表状态
来源：http://baike.bbcook.cn/Article/details/ginihmkmq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.epnwcf.com/Article/details/gmvemjewn.sHtML

[Q74] 强制使用索引
来源：http://blog.fktsv.cn/Article/details/gqlvqcklz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fktsv.cn/Article/details/godvvatxv.sHtML

[Q75] 日期格式化
来源：http://baike.vehdjk.com/Article/details/gydlqjequ.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gmcifounn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.tarul.cn/Article/details/gvdyyjwdk.sHtML

[Q76] 按天统计
来源：http://blog.tarul.cn/Article/details/gpfhxdauw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.epnwcf.com/Article/details/gbrugkdtg.sHtML

[Q77] 时间加减
来源：http://read.share.tarul.cn/Article/details/gduzeeqkw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.epnwcf.com/Article/details/ggfjbjcxt.sHtML

[Q78] 当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gyrrotcci.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.yfazqb.com/Article/details/gyhdcgffq.sHtML

[Q79] 字符串拼接
来源：http://baike.bbcook.cn/Article/details/gegyhbpux.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.epnwcf.com/Article/details/gznsfhezn.sHtML

[Q80] 字符串截取
来源：http://m.share.sjlbkw.cn/Article/details/gvanrbxix.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gezrjkbpf.sHtML

[Q81] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/grifjfqey.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.bbcook.cn/Article/details/gnypwzqpf.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fktsv.cn/Article/details/gjhgnbatu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/gstquzvga.sHtML

[Q83] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gfauxdyoa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.tarul.cn/Article/details/glguxcmam.sHtML

[Q84] 去除首尾空格
来源：http://read.share.epnwcf.com/Article/details/geoadbejx.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gewuaprht.sHtML

[Q85] 数值取整
来源：http://wap.bbcook.cn/Article/details/gzgnmybuy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gqcfavefe.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.epnwcf.com/Article/details/gchgozicz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.epnwcf.com/Article/details/gruedvhol.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fktsv.cn/Article/details/getlodbvp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.vehdjk.com/Article/details/ghwjmlyhi.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.tarul.cn/Article/details/gnvpcfono.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.tarul.cn/Article/details/gboewenfg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.epnwcf.com/Article/details/gnrxpttyt.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.tarul.cn/Article/details/gzdvvuukr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.sjlbkw.cn/Article/details/greialmdw.sHtML

[Q90] 生成序号列
来源：http://wap.yfazqb.com/Article/details/gnjqhcivw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fktsv.cn/Article/details/glwordski.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ghzycdjia.sHtML

R. Bash 专题
来源：http://www.share.fktsv.cn/Article/details/grlvcwqfi.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gsdnlrtse.sHtML

[R01] shebang 与严格模式
来源：http://m.share.epnwcf.com/Article/details/gbsghfbal.sHtML

#!/usr/bin/env bash
来源：http://www.share.sjlbkw.cn/Article/details/gdwflaiot.sHtML

set -euo pipefail
来源：http://blog.sjlbkw.cn/Article/details/gwkqixjil.sHtML

[R02] 变量赋值与使用
来源：http://blog.sjlbkw.cn/Article/details/ghkvysccx.sHtML

name="Tom"; echo "$name"
来源：http://m.share.sjlbkw.cn/Article/details/gguuaqiwl.sHtML

[R03] 只读变量
来源：http://blog.tarul.cn/Article/details/gyndkrzrh.sHtML

readonly PI=3.14
来源：http://wap.yfazqb.com/Article/details/gycpxyuyj.sHtML

[R04] 位置参数
来源：http://read.share.bbcook.cn/Article/details/ghgsvryjl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.vehdjk.com/Article/details/gripssohe.sHtML

[R05] 参数默认值
来源：http://wap.epnwcf.com/Article/details/gyxnrioaz.sHtML

name="${1:-default}"
来源：http://www.blog.vehdjk.com/Article/details/gxghfyqag.sHtML

[R06] 判断命令是否存在
来源：http://wap.sjlbkw.cn/Article/details/gdugedbps.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gjxwxykch.sHtML

[R07] if 判断文件
来源：http://baike.yfazqb.com/Article/details/gdurkkiif.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.epnwcf.com/Article/details/guejqagyi.sHtML

[R08] 数值比较
来源：http://www.m.share.fktsv.cn/Article/details/gebqxrvly.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.yfazqb.com/Article/details/gkgepjsld.sHtML

[R09] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/gkmfsvqno.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.bbcook.cn/Article/details/gyxyynwhg.sHtML

[R10] 正则匹配
来源：http://blog.bbcook.cn/Article/details/gwaoauhjb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.tarul.cn/Article/details/gvcbkifzt.sHtML

[R11] case 多分支
来源：http://www.blog.tarul.cn/Article/details/guwulejou.sHtML

case "$1" in
来源：http://read.share.yfazqb.com/Article/details/gysjwlxmv.sHtML

start) echo "启动" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gyqqkimnp.sHtML

stop)  echo "停止" ;;
来源：http://www.share.vehdjk.com/Article/details/gobwtosfg.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fktsv.cn/Article/details/ghygexqkz.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/gpnoijolg.sHtML

[R12] for 遍历文件
来源：http://www.blog.tarul.cn/Article/details/gmmujtewd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.sjlbkw.cn/Article/details/gkepbrnja.sHtML

[R13] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/ghyaubysy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fktsv.cn/Article/details/gqahtvjoh.sHtML

[R14] C 风格 for
来源：http://blog.tarul.cn/Article/details/guzumtsew.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fktsv.cn/Article/details/gcgenlnnw.sHtML

[R15] while 逐行读文件
来源：http://3g.epnwcf.com/Article/details/gbmnfuxyw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gtfpooagl.sHtML

[R16] until 等待条件
来源：http://read.share.sjlbkw.cn/Article/details/gtqpcubto.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gudsizerm.sHtML

[R17] 数组定义与取值
来源：http://wap.bbcook.cn/Article/details/gudyjkvrk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gauiqolis.sHtML

[R18] 遍历数组
来源：http://www.blog.yfazqb.com/Article/details/gavcfreyh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.tarul.cn/Article/details/gljtygido.sHtML

[R19] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/gndjyqrvp.sHtML

echo "${#arr[@]}"
来源：http://www.share.sjlbkw.cn/Article/details/gnockhhue.sHtML

[R20] 关联数组（字典）
来源：http://www.share.tarul.cn/Article/details/gerimdakm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.yfazqb.com/Article/details/gykfuuhtl.sHtML

[R21] 字符串长度
来源：http://read.share.fktsv.cn/Article/details/gdmdhvwft.sHtML

echo "${#s}"
来源：http://read.share.vehdjk.com/Article/details/glcprecdl.sHtML

[R22] 截取子串
来源：http://3g.epnwcf.com/Article/details/gaqdbhwhx.sHtML

echo "${s:0:5}"
来源：http://baike.bbcook.cn/Article/details/gmefapirg.sHtML

[R23] 字符串替换
来源：http://www.share.tarul.cn/Article/details/gfdfyqbea.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fktsv.cn/Article/details/gabeestni.sHtML

[R24] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/garwtsyyq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fktsv.cn/Article/details/geunpqogs.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.epnwcf.com/Article/details/guxcuhtha.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.sjlbkw.cn/Article/details/goehrkrbt.sHtML

[R26] 命令替换
来源：http://3g.fktsv.cn/Article/details/gxvcagjcm.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.bbcook.cn/Article/details/gxdokffqf.sHtML

[R27] 算术展开
来源：http://www.blog.sjlbkw.cn/Article/details/gpiumtzws.sHtML

echo $((1 + 2 * 3))
来源：http://wap.yfazqb.com/Article/details/gwoweqjrd.sHtML

[R28] 浮点运算
来源：http://mobile.bbcook.cn/Article/details/gwmkfgtgc.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.sjlbkw.cn/Article/details/gfixankpz.sHtML

[R29] 定义函数
来源：http://www.share.yfazqb.com/Article/details/gsftnynre.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.yfazqb.com/Article/details/gpuxdefmh.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/gnkswshjm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.yfazqb.com/Article/details/gbegeqxfe.sHtML

[R31] 局部变量
来源：http://3g.yfazqb.com/Article/details/gbunhexim.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fktsv.cn/Article/details/gwjvpuubu.sHtML

[R32] 参数个数校验
来源：http://m.share.bbcook.cn/Article/details/gpuuawpev.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.sjlbkw.cn/Article/details/glbmvyesu.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.vehdjk.com/Article/details/gqjawzmco.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.sjlbkw.cn/Article/details/gismagejn.sHtML

[R34] 退出时清理
来源：http://read.share.vehdjk.com/Article/details/gazbjmgok.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gvvnzqjbu.sHtML

[R35] 后台执行并等待
来源：http://baike.vehdjk.com/Article/details/gugpexkcz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.bbcook.cn/Article/details/gpwdsyqzg.sHtML

[R36] 并发执行多个任务
来源：http://mobile.epnwcf.com/Article/details/gkkmrzmue.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fktsv.cn/Article/details/gubfksfww.sHtML

[R37] 把输出赋给变量
来源：http://mobile.yfazqb.com/Article/details/glohfmgkk.sHtML

files=$(ls -1)
来源：http://www.blog.fktsv.cn/Article/details/gzgnjqmzp.sHtML

[R38] 管道串联
来源：http://blog.tarul.cn/Article/details/gsdfpeqor.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.vehdjk.com/Article/details/gocqsjpvs.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.bbcook.cn/Article/details/goctixxas.sHtML

cmd > out.log 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gaazbvcuc.sHtML

[R40] 追加写日志
来源：http://mobile.vehdjk.com/Article/details/gdnxppvcl.sHtML

echo "log" >> out.log
来源：http://www.m.share.yfazqb.com/Article/details/gubyuqbux.sHtML

[R41] 丢弃输出
来源：http://www.share.tarul.cn/Article/details/grxmlcqqc.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/gpgfvpayi.sHtML

[R42] 输入重定向
来源：http://baike.epnwcf.com/Article/details/gojqufqxx.sHtML

wc -l < a.txt
来源：http://www.blog.yfazqb.com/Article/details/gjxcthotq.sHtML

[R43] 按名字查找文件
来源：http://wap.bbcook.cn/Article/details/gbthqevog.sHtML

find . -name "*.log" -type f
来源：http://blog.epnwcf.com/Article/details/gibrtmmug.sHtML

[R44] 按修改时间查找
来源：http://baike.bbcook.cn/Article/details/gupgjjuey.sHtML

find . -mtime -7 -type f
来源：http://baike.bbcook.cn/Article/details/gyrcibhhh.sHtML

[R45] 批量删除
来源：http://www.blog.vehdjk.com/Article/details/giempnhql.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fktsv.cn/Article/details/gcjfenfmr.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fktsv.cn/Article/details/gktisrccc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.bbcook.cn/Article/details/gryxskthx.sHtML

[R47] sed 单行替换
来源：http://m.share.bbcook.cn/Article/details/gqaduyldo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.yfazqb.com/Article/details/gedodtjzu.sHtML

[R48] awk 取指定列
来源：http://read.share.bbcook.cn/Article/details/ggchlfucd.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gxjivmuts.sHtML

[R49] awk 带条件
来源：http://baike.vehdjk.com/Article/details/gkpzobcsb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.tarul.cn/Article/details/gfbxjspyy.sHtML

[R50] awk 求和
来源：http://www.share.fktsv.cn/Article/details/gdyqrrhop.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.epnwcf.com/Article/details/glzqkukjj.sHtML

[R51] 排序去重取前几
来源：http://mobile.tarul.cn/Article/details/gaetvyycg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.tarul.cn/Article/details/gjzkujirm.sHtML

[R52] 统计行数
来源：http://read.share.epnwcf.com/Article/details/gfryancgv.sHtML

wc -l a.txt
来源：http://read.share.tarul.cn/Article/details/gxyoesqyg.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/gjjgybaaf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fktsv.cn/Article/details/gpanlivxf.sHtML

[R54] 比较两个文件
来源：http://www.share.vehdjk.com/Article/details/giyrhiccl.sHtML

diff a.txt b.txt
来源：http://www.share.yfazqb.com/Article/details/gpueoafwm.sHtML

[R55] 压缩与解压
来源：http://www.m.share.epnwcf.com/Article/details/gvlnsqnjs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fktsv.cn/Article/details/gzpsyfnkt.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/gwcmihnhu.sHtML

scp file user@host:/path/
来源：http://read.share.vehdjk.com/Article/details/gtgktooym.sHtML

[R57] 远程执行命令
来源：http://www.blog.fktsv.cn/Article/details/gyeuwbtpo.sHtML

ssh user@host 'uptime'
来源：http://read.share.fktsv.cn/Article/details/gxmjrdlkm.sHtML

[R58] 下载文件
来源：http://wap.vehdjk.com/Article/details/gmfphcbrm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fktsv.cn/Article/details/gtrbdhiwy.sHtML

[R59] 发 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gpetbovsk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.vehdjk.com/Article/details/givtpibmt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/ggryilimq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.bbcook.cn/Article/details/gevchhjkh.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/guiqwiyyl.sHtML

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/gblqcsrqe.sHtML

[R62] 找最占空间的文件
来源：http://www.share.bbcook.cn/Article/details/gwiqmkbmp.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fktsv.cn/Article/details/gsrcvlslr.sHtML

[R63] 内存与进程
来源：http://read.share.epnwcf.com/Article/details/gnigsmylq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.sjlbkw.cn/Article/details/gnllwcnvs.sHtML

[R64] 结束进程
来源：http://baike.epnwcf.com/Article/details/gffnnejst.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.vehdjk.com/Article/details/gbiqwytmo.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fktsv.cn/Article/details/gxnbnwcau.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.epnwcf.com/Article/details/gckzkipds.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/gyuirtbhg.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/gcvqqedjp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fktsv.cn/Article/details/golrrnwkw.sHtML

openssl rand -hex 16
来源：http://baike.tarul.cn/Article/details/gtvtlllpz.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/gqsnejtpc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.sjlbkw.cn/Article/details/gygpondlj.sHtML

[R69] 生成随机密码
来源：http://wap.fktsv.cn/Article/details/goeslhsev.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fktsv.cn/Article/details/gucezuqix.sHtML

[R70] 时间戳与互转
来源：http://baike.sjlbkw.cn/Article/details/giksesxii.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/gnmpxnlfk.sHtML

[R71] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gfzvjesdr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.tarul.cn/Article/details/ghprwmmrg.sHtML

[R72] 等待端口就绪
来源：http://www.blog.tarul.cn/Article/details/gebikkbtw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gdlmakkeb.sHtML

[R73] 分割大日志
来源：http://www.m.share.vehdjk.com/Article/details/ggtixqvjj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.epnwcf.com/Article/details/gnhadplbr.sHtML

[R74] 批量重命名
来源：http://wap.epnwcf.com/Article/details/gkifibvov.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.tarul.cn/Article/details/gbaudmulz.sHtML

[R75] 导出环境变量
来源：http://baike.sjlbkw.cn/Article/details/gkqvvqhnx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.vehdjk.com/Article/details/gvcxofshn.sHtML

[R76] 使用临时文件
来源：http://baike.yfazqb.com/Article/details/gikeezvqs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/gaivpkszf.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/girfhxxfa.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.tarul.cn/Article/details/gusuzsanl.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/gvtlzgzvd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.yfazqb.com/Article/details/ggbutlrqk.sHtML

[R79] 解析命令行选项
来源：http://blog.vehdjk.com/Article/details/gxrcrynbh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.bbcook.cn/Article/details/gaunjfhej.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.bbcook.cn/Article/details/gqizndvtq.sHtML

time ./run.sh
来源：http://www.share.tarul.cn/Article/details/guizpqqba.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzaaliarp.sHtML

S. C / C++ 专题
来源：http://mobile.sjlbkw.cn/Article/details/ghpfkuiao.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfckwfsxq.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gozhogjbg.sHtML

#include <stdio.h>
来源：http://mobile.vehdjk.com/Article/details/gtrwdervm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/gyodabukf.sHtML

[S02] C：变量与格式化输出
来源：http://blog.bbcook.cn/Article/details/guysrjmuz.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fktsv.cn/Article/details/gmkjkyjpi.sHtML

[S03] C：读入整数
来源：http://blog.fktsv.cn/Article/details/gllvnaufp.sHtML

int x; scanf("%d", &x);
来源：http://3g.sjlbkw.cn/Article/details/gnbmetwvy.sHtML

[S04] C：字符串复制
来源：http://m.share.fktsv.cn/Article/details/gwcndfgoi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.epnwcf.com/Article/details/gequdhvli.sHtML

[S05] C：字符串长度
来源：http://www.blog.tarul.cn/Article/details/gfhiowlvp.sHtML


<!-- 参考信息 -->