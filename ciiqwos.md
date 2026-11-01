代发 wailian999

[Q33] 多列分组
来源：http://baike.fktsv.cn/Article/details/gbgfyictk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fktsv.cn/Article/details/gdzegcmjl.sHtML

[Q34] 每组取第一条
来源：http://www.share.bbcook.cn/Article/details/gmllubywf.sHtML

SELECT * FROM (
来源：http://wap.tarul.cn/Article/details/gvhgghlld.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.epnwcf.com/Article/details/gvjtqqufs.sHtML

) t WHERE rn = 1;
来源：http://baike.yfazqb.com/Article/details/gxerlmwqp.sHtML

[Q35] 内连接
来源：http://read.share.yfazqb.com/Article/details/gtrmisqur.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gghwmklpn.sHtML

[Q36] 左连接
来源：http://www.m.share.tarul.cn/Article/details/ggonlqups.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/giqgohayn.sHtML

[Q37] 右连接
来源：http://wap.tarul.cn/Article/details/gmunzlxvw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fktsv.cn/Article/details/gbnmqtbjj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.bbcook.cn/Article/details/gsfhoheka.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fktsv.cn/Article/details/gmwubxsgh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.tarul.cn/Article/details/gvuveerdm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.bbcook.cn/Article/details/gavnnghle.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gueirwzle.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.sjlbkw.cn/Article/details/goeknqkmv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.tarul.cn/Article/details/gyqdoiehh.sHtML

[Q41] 多表连接
来源：http://read.share.bbcook.cn/Article/details/gnonhxuns.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fktsv.cn/Article/details/gksbfbxuc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.yfazqb.com/Article/details/gysdrpgoq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.sjlbkw.cn/Article/details/gzkfwxfpn.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.yfazqb.com/Article/details/gzcbceqfe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.yfazqb.com/Article/details/gqxvkijkr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.bbcook.cn/Article/details/giapzuori.sHtML

[Q43] 标量子查询
来源：http://www.share.bbcook.cn/Article/details/gfogojoft.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fktsv.cn/Article/details/gmhmpvsqq.sHtML

[Q44] IN 子查询
来源：http://wap.tarul.cn/Article/details/gjhhprawg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.yfazqb.com/Article/details/gndfqlujv.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.bbcook.cn/Article/details/glprddpqm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gfqwazmiq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.tarul.cn/Article/details/gajxcgcpt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/gtwjrmxei.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.yfazqb.com/Article/details/gmcmzdllz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.vehdjk.com/Article/details/gzsgfbcic.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gqqbgshta.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.epnwcf.com/Article/details/gijvodezm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.sjlbkw.cn/Article/details/grwqpxpjj.sHtML

[Q49] 更新单行
来源：http://read.share.yfazqb.com/Article/details/gxqphknws.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/gzccptfle.sHtML

[Q50] 批量更新
来源：http://www.m.share.vehdjk.com/Article/details/ghrybkgbo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.sjlbkw.cn/Article/details/gcziaorpf.sHtML

[Q51] 用子查询更新
来源：http://wap.tarul.cn/Article/details/ghlkqorvz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fktsv.cn/Article/details/gbydcyntm.sHtML

[Q52] 删除指定行
来源：http://read.share.fktsv.cn/Article/details/gdbkhaarx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fktsv.cn/Article/details/gorxqrcsp.sHtML

[Q53] 按条件删除
来源：http://blog.bbcook.cn/Article/details/glyvxsofn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/guzuwbqbd.sHtML

[Q54] 清空表
来源：http://m.share.epnwcf.com/Article/details/gbkaowdci.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.sjlbkw.cn/Article/details/ggprfcofg.sHtML

[Q55] 排名（并列占位）
来源：http://wap.bbcook.cn/Article/details/ggslsxttz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.epnwcf.com/Article/details/gsxcmppvy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.yfazqb.com/Article/details/gjoezfpoq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.yfazqb.com/Article/details/gonejuvlf.sHtML

[Q57] 行号
来源：http://m.share.fktsv.cn/Article/details/gggfmwocp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.epnwcf.com/Article/details/gvkjuipaw.sHtML

[Q58] 累计求和
来源：http://blog.vehdjk.com/Article/details/gxrvtgbii.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fktsv.cn/Article/details/gwdcfarbh.sHtML

[Q59] 分组内累计
来源：http://m.share.sjlbkw.cn/Article/details/gazilznoy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gfuaabsqb.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.sjlbkw.cn/Article/details/gpfrmxylp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fktsv.cn/Article/details/gsxrqbidt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gvulazdxm.sHtML

[Q61] 移动平均
来源：http://m.share.sjlbkw.cn/Article/details/gaeancnmu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gpmrmmchf.sHtML

[Q62] 分组占比
来源：http://baike.bbcook.cn/Article/details/gbpaqhlcm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gcoxpesht.sHtML

[Q63] 开启事务
来源：http://www.blog.tarul.cn/Article/details/guvpqhuea.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fktsv.cn/Article/details/glxpskpws.sHtML

[Q64] 提交事务
来源：http://mobile.bbcook.cn/Article/details/gwjtpwoia.sHtML

COMMIT;
来源：http://www.m.share.vehdjk.com/Article/details/gbqrxgexi.sHtML

[Q65] 回滚事务
来源：http://mobile.vehdjk.com/Article/details/gkzzunhvw.sHtML

ROLLBACK;
来源：http://3g.fktsv.cn/Article/details/glzwhckmb.sHtML

[Q66] 行锁查询
来源：http://www.blog.tarul.cn/Article/details/gwvixibcw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.yfazqb.com/Article/details/gfawukyll.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.yfazqb.com/Article/details/gxlxdnsfk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.tarul.cn/Article/details/gscmkqojc.sHtML

[Q68] 保存点
来源：http://www.share.epnwcf.com/Article/details/gxatxptyh.sHtML

SAVEPOINT sp1;
来源：http://baike.epnwcf.com/Article/details/gosbdscdh.sHtML

ROLLBACK TO sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gfayaeqvw.sHtML

[Q69] 查看执行计划
来源：http://m.share.sjlbkw.cn/Article/details/gyufczebe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.yfazqb.com/Article/details/guucetdju.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fktsv.cn/Article/details/gxufbchrr.sHtML

ANALYZE TABLE users;
来源：http://3g.sjlbkw.cn/Article/details/gkwiqhtbf.sHtML

[Q71] 查看建表语句
来源：http://m.share.fktsv.cn/Article/details/grwadgjmf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.yfazqb.com/Article/details/ghvqfqpkg.sHtML

[Q72] 查看索引
来源：http://read.share.vehdjk.com/Article/details/glurkobrr.sHtML

SHOW INDEX FROM users;
来源：http://m.share.yfazqb.com/Article/details/gdwpppfwc.sHtML

[Q73] 查看表状态
来源：http://www.m.share.vehdjk.com/Article/details/glzalvhlp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.yfazqb.com/Article/details/gccajidyj.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fktsv.cn/Article/details/gszbwdglh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.epnwcf.com/Article/details/gvvvogffp.sHtML

[Q75] 日期格式化
来源：http://3g.tarul.cn/Article/details/gyrmpzdbo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.tarul.cn/Article/details/genvihjbh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.vehdjk.com/Article/details/gpyritwtg.sHtML

[Q76] 按天统计
来源：http://www.blog.sjlbkw.cn/Article/details/gkiosmerm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.yfazqb.com/Article/details/grnqqfqzj.sHtML

[Q77] 时间加减
来源：http://www.m.share.yfazqb.com/Article/details/gjksblesa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.tarul.cn/Article/details/gomzeytcp.sHtML

[Q78] 当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gwmwezlft.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.vehdjk.com/Article/details/gpancvsez.sHtML

[Q79] 字符串拼接
来源：http://blog.yfazqb.com/Article/details/gykkesper.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.epnwcf.com/Article/details/gvbkdljtd.sHtML

[Q80] 字符串截取
来源：http://www.blog.yfazqb.com/Article/details/gouirayuy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.tarul.cn/Article/details/gxunestix.sHtML

[Q81] 字符串替换
来源：http://baike.tarul.cn/Article/details/gqlygkuks.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fktsv.cn/Article/details/gnmwosmbh.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.vehdjk.com/Article/details/gzcaaqcnj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gbkersorl.sHtML

[Q83] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gucretmqw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gmxugicqg.sHtML

[Q84] 去除首尾空格
来源：http://3g.epnwcf.com/Article/details/gxgjuuvub.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gzqzubcwp.sHtML

[Q85] 数值取整
来源：http://m.share.epnwcf.com/Article/details/gfdpermgw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fktsv.cn/Article/details/gmalypztt.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.bbcook.cn/Article/details/gtvztrckh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/gxxfzwvgs.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/gufhvupxh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlemrige.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.epnwcf.com/Article/details/gksntlobi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fktsv.cn/Article/details/guyvidiit.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.tarul.cn/Article/details/gtrmptwod.sHtML

[Q89] 判断表是否存在
来源：http://3g.bbcook.cn/Article/details/gjruqmgeq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.sjlbkw.cn/Article/details/gvtlnuamc.sHtML

[Q90] 生成序号列
来源：http://blog.bbcook.cn/Article/details/gmomimajm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.vehdjk.com/Article/details/giudubvwx.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gaqbpddai.sHtML

R. Bash 专题
来源：http://read.share.epnwcf.com/Article/details/gzebyhivz.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ghzovftmn.sHtML

[R01] shebang 与严格模式
来源：http://m.share.sjlbkw.cn/Article/details/gdwtehofe.sHtML

#!/usr/bin/env bash
来源：http://www.blog.epnwcf.com/Article/details/gcmqwsonh.sHtML

set -euo pipefail
来源：http://www.m.share.fktsv.cn/Article/details/gxfxfrasz.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.yfazqb.com/Article/details/gazfmkzva.sHtML

name="Tom"; echo "$name"
来源：http://read.share.sjlbkw.cn/Article/details/ggrmdjqgn.sHtML

[R03] 只读变量
来源：http://m.share.bbcook.cn/Article/details/gnwfqeuoy.sHtML

readonly PI=3.14
来源：http://www.share.fktsv.cn/Article/details/gypgxjqbb.sHtML

[R04] 位置参数
来源：http://wap.bbcook.cn/Article/details/grrbakota.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.epnwcf.com/Article/details/gbunwvvuw.sHtML

[R05] 参数默认值
来源：http://m.share.fktsv.cn/Article/details/gqorhyuuc.sHtML

name="${1:-default}"
来源：http://www.blog.yfazqb.com/Article/details/guyhiapcp.sHtML

[R06] 判断命令是否存在
来源：http://wap.bbcook.cn/Article/details/gyeoguvps.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gkatukaie.sHtML

[R07] if 判断文件
来源：http://www.share.vehdjk.com/Article/details/grmcnrqcq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.epnwcf.com/Article/details/gcqfqwjdf.sHtML

[R08] 数值比较
来源：http://www.m.share.tarul.cn/Article/details/gidrgpacc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fktsv.cn/Article/details/gbsfabbej.sHtML

[R09] 字符串比较
来源：http://baike.vehdjk.com/Article/details/gaaltruhd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gkhmhnixw.sHtML

[R10] 正则匹配
来源：http://www.blog.fktsv.cn/Article/details/gwzrcwwyi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.vehdjk.com/Article/details/gjkqqmvwe.sHtML

[R11] case 多分支
来源：http://www.share.bbcook.cn/Article/details/gaqbketqh.sHtML

case "$1" in
来源：http://blog.sjlbkw.cn/Article/details/gvqvmtzhp.sHtML

start) echo "启动" ;;
来源：http://mobile.fktsv.cn/Article/details/gkekhwhfv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.epnwcf.com/Article/details/gfoizamnl.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.tarul.cn/Article/details/gmjtndzlf.sHtML

esac
来源：http://m.share.yfazqb.com/Article/details/gkqhmlwpj.sHtML

[R12] for 遍历文件
来源：http://3g.bbcook.cn/Article/details/gzvlxgjlq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.sjlbkw.cn/Article/details/gojxctvax.sHtML

[R13] for 计数循环
来源：http://blog.tarul.cn/Article/details/gmxpovtiu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/grthcared.sHtML

[R14] C 风格 for
来源：http://www.m.share.tarul.cn/Article/details/gqsqiffqi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.bbcook.cn/Article/details/gyhgpwicw.sHtML

[R15] while 逐行读文件
来源：http://baike.yfazqb.com/Article/details/gnturfohv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.sjlbkw.cn/Article/details/gjrilttdt.sHtML

[R16] until 等待条件
来源：http://www.m.share.tarul.cn/Article/details/gczolmyeu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gznclfceq.sHtML

[R17] 数组定义与取值
来源：http://wap.tarul.cn/Article/details/gooaegabw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.tarul.cn/Article/details/gshcygxic.sHtML

[R18] 遍历数组
来源：http://blog.yfazqb.com/Article/details/gdpyeccmo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.epnwcf.com/Article/details/ggxaasars.sHtML

[R19] 数组长度
来源：http://mobile.epnwcf.com/Article/details/gzessanma.sHtML

echo "${#arr[@]}"
来源：http://blog.epnwcf.com/Article/details/gvrirdpop.sHtML

[R20] 关联数组（字典）
来源：http://wap.fktsv.cn/Article/details/gczfuzalw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fktsv.cn/Article/details/gmijsrvvd.sHtML

[R21] 字符串长度
来源：http://blog.bbcook.cn/Article/details/gcfkyyxje.sHtML

echo "${#s}"
来源：http://mobile.bbcook.cn/Article/details/goshzwynx.sHtML

[R22] 截取子串
来源：http://wap.epnwcf.com/Article/details/gnamrdfhl.sHtML

echo "${s:0:5}"
来源：http://blog.vehdjk.com/Article/details/galypjzrc.sHtML

[R23] 字符串替换
来源：http://blog.vehdjk.com/Article/details/gzvngzfuw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.bbcook.cn/Article/details/gybytjjtp.sHtML

[R24] 大小写转换
来源：http://3g.yfazqb.com/Article/details/ggiqseckc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fktsv.cn/Article/details/gfaoltrfn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgfwtiqr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.yfazqb.com/Article/details/gtjxothjx.sHtML

[R26] 命令替换
来源：http://3g.yfazqb.com/Article/details/giryhdxuq.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fktsv.cn/Article/details/gxocgotlu.sHtML

[R27] 算术展开
来源：http://www.m.share.epnwcf.com/Article/details/gnnffbbxa.sHtML

echo $((1 + 2 * 3))
来源：http://baike.vehdjk.com/Article/details/gzhljspzx.sHtML

[R28] 浮点运算
来源：http://baike.bbcook.cn/Article/details/gjoxoumta.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.epnwcf.com/Article/details/gfrgiwqtt.sHtML

[R29] 定义函数
来源：http://m.share.bbcook.cn/Article/details/ghepvrqih.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fktsv.cn/Article/details/glxssdwfg.sHtML

[R30] 函数返回状态码
来源：http://wap.yfazqb.com/Article/details/gxhfdafwe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.vehdjk.com/Article/details/gpzfaxizs.sHtML

[R31] 局部变量
来源：http://www.blog.yfazqb.com/Article/details/gktgthgpj.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.yfazqb.com/Article/details/gawguofic.sHtML

[R32] 参数个数校验
来源：http://www.blog.sjlbkw.cn/Article/details/gwuhwowaa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/gejnyfrfe.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fktsv.cn/Article/details/gmdbzrped.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.sjlbkw.cn/Article/details/gdkocsapt.sHtML

[R34] 退出时清理
来源：http://m.share.vehdjk.com/Article/details/ghbrrmykl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/gyhxggmif.sHtML

[R35] 后台执行并等待
来源：http://m.share.epnwcf.com/Article/details/guxnukfag.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.bbcook.cn/Article/details/gjuaatvwc.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/gankmbbpi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.yfazqb.com/Article/details/guqsddzjd.sHtML

[R37] 把输出赋给变量
来源：http://read.share.yfazqb.com/Article/details/gmfsayteq.sHtML

files=$(ls -1)
来源：http://wap.sjlbkw.cn/Article/details/gmdslkvan.sHtML

[R38] 管道串联
来源：http://mobile.fktsv.cn/Article/details/gxtawtoiq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.sjlbkw.cn/Article/details/gkfibexvb.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.bbcook.cn/Article/details/gugdosbxh.sHtML

cmd > out.log 2>&1
来源：http://m.share.bbcook.cn/Article/details/giywujiof.sHtML

[R40] 追加写日志
来源：http://3g.sjlbkw.cn/Article/details/geepljjxs.sHtML

echo "log" >> out.log
来源：http://blog.fktsv.cn/Article/details/grneqhkyc.sHtML

[R41] 丢弃输出
来源：http://3g.yfazqb.com/Article/details/gywkldmqn.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.vehdjk.com/Article/details/giroknvlu.sHtML

[R42] 输入重定向
来源：http://baike.sjlbkw.cn/Article/details/gvppzsvax.sHtML

wc -l < a.txt
来源：http://baike.vehdjk.com/Article/details/geuhzcdol.sHtML

[R43] 按名字查找文件
来源：http://3g.yfazqb.com/Article/details/gggqnqwsy.sHtML

find . -name "*.log" -type f
来源：http://m.share.epnwcf.com/Article/details/gcqoklxpd.sHtML

[R44] 按修改时间查找
来源：http://blog.vehdjk.com/Article/details/gtyjarjlr.sHtML

find . -mtime -7 -type f
来源：http://blog.vehdjk.com/Article/details/gkpjwxcje.sHtML

[R45] 批量删除
来源：http://3g.fktsv.cn/Article/details/gmazfbvmh.sHtML

find . -name "*.tmp" -delete
来源：http://baike.bbcook.cn/Article/details/gtmcpgvcc.sHtML

[R46] 递归替换文件内容
来源：http://www.share.vehdjk.com/Article/details/gxlrsxmqe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.epnwcf.com/Article/details/gqtroqnsz.sHtML

[R47] sed 单行替换
来源：http://3g.fktsv.cn/Article/details/gvzfqmnjh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fktsv.cn/Article/details/gyhachznp.sHtML

[R48] awk 取指定列
来源：http://wap.tarul.cn/Article/details/ghzkwnjhj.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.yfazqb.com/Article/details/gcprchluc.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/gansgamya.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.epnwcf.com/Article/details/grotfqayu.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/gwfxmudgx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gxqwjidtt.sHtML

[R51] 排序去重取前几
来源：http://mobile.fktsv.cn/Article/details/gpyzkdhhx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.tarul.cn/Article/details/gwioorurv.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/gvxacgpdg.sHtML

wc -l a.txt
来源：http://3g.tarul.cn/Article/details/ggthrztgh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fktsv.cn/Article/details/gysgiwlsh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.sjlbkw.cn/Article/details/gvekijqyb.sHtML

[R54] 比较两个文件
来源：http://3g.fktsv.cn/Article/details/geqgtaymt.sHtML

diff a.txt b.txt
来源：http://read.share.yfazqb.com/Article/details/gmftksccd.sHtML

[R55] 压缩与解压
来源：http://wap.sjlbkw.cn/Article/details/gdhiejkxw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.vehdjk.com/Article/details/gceipfofb.sHtML

[R56] 远程拷贝
来源：http://blog.fktsv.cn/Article/details/gjorvecoc.sHtML

scp file user@host:/path/
来源：http://wap.tarul.cn/Article/details/goztbukch.sHtML

[R57] 远程执行命令
来源：http://mobile.yfazqb.com/Article/details/ggdzctybp.sHtML

ssh user@host 'uptime'
来源：http://m.share.fktsv.cn/Article/details/gbtieelzt.sHtML

[R58] 下载文件
来源：http://3g.sjlbkw.cn/Article/details/grkcbybmr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.vehdjk.com/Article/details/gsecnpxpc.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gjonvfmdi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.sjlbkw.cn/Article/details/gpoctlpex.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gmnzuugyj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/gcsxbysoo.sHtML

[R61] 磁盘占用
来源：http://baike.yfazqb.com/Article/details/gxzgmntqz.sHtML

df -h;  du -sh *
来源：http://blog.tarul.cn/Article/details/gzazvwcod.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fktsv.cn/Article/details/gvopwtkrf.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.bbcook.cn/Article/details/gjxkfahtr.sHtML

[R63] 内存与进程
来源：http://blog.epnwcf.com/Article/details/gzeaqolqr.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.sjlbkw.cn/Article/details/gmntzutzv.sHtML

[R64] 结束进程
来源：http://www.blog.yfazqb.com/Article/details/gamergiwc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.yfazqb.com/Article/details/gjfbttbkr.sHtML

[R65] 查看端口占用
来源：http://www.m.share.yfazqb.com/Article/details/grjsfhbnl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.yfazqb.com/Article/details/goohodsuv.sHtML

[R66] 定时任务
来源：http://baike.sjlbkw.cn/Article/details/gvxuswvqo.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fktsv.cn/Article/details/glyxdlhmg.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.epnwcf.com/Article/details/gzeobbhwg.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/gvpddjlei.sHtML

[R68] 计算文件校验值
来源：http://www.share.vehdjk.com/Article/details/gifjuewdy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.bbcook.cn/Article/details/ghysqhqec.sHtML

[R69] 生成随机密码
来源：http://baike.vehdjk.com/Article/details/gacuqovxp.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.vehdjk.com/Article/details/gruiqjemo.sHtML

[R70] 时间戳与互转
来源：http://3g.bbcook.cn/Article/details/gytwtqqde.sHtML

date +%s;  date -d @1700000000
来源：http://blog.vehdjk.com/Article/details/gozgsclgx.sHtML

[R71] 日期格式化
来源：http://blog.yfazqb.com/Article/details/grqotjfmm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.tarul.cn/Article/details/gbfvfbzoa.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/gunnbfivj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gllsytxeh.sHtML

[R73] 分割大日志
来源：http://www.m.share.bbcook.cn/Article/details/gfrnmfugw.sHtML

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/gljrtzwli.sHtML

[R74] 批量重命名
来源：http://3g.yfazqb.com/Article/details/gnfmnepfp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.yfazqb.com/Article/details/glcneozcr.sHtML

[R75] 导出环境变量
来源：http://m.share.epnwcf.com/Article/details/grxajffqp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fktsv.cn/Article/details/gxmxhdsrn.sHtML

[R76] 使用临时文件
来源：http://baike.vehdjk.com/Article/details/gyuluclaw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/ggevzitei.sHtML

[R77] 读取用户输入
来源：http://wap.bbcook.cn/Article/details/ghpumjkum.sHtML

read -rp "请输入: " ans
来源：http://m.share.fktsv.cn/Article/details/gslrgyqyv.sHtML

[R78] 交互式菜单
来源：http://wap.sjlbkw.cn/Article/details/ggfkeunoj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.sjlbkw.cn/Article/details/gdfqgmxbs.sHtML

[R79] 解析命令行选项
来源：http://www.share.epnwcf.com/Article/details/gqxqfltpy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/gdoeunmyq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.tarul.cn/Article/details/grigwjihz.sHtML

time ./run.sh
来源：http://m.share.bbcook.cn/Article/details/gwooijcax.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gnktuwhmk.sHtML

S. C / C++ 专题
来源：http://mobile.fktsv.cn/Article/details/gfpsonidh.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gblgdlqnk.sHtML

[S01] C：Hello World
来源：http://wap.tarul.cn/Article/details/gzkzzmcbz.sHtML

#include <stdio.h>
来源：http://www.blog.epnwcf.com/Article/details/gudhjqsxp.sHtML


<!-- 参考信息 -->