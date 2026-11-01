代发 wailian999

[Q33] 多列分组
来源：http://wap.vehdjk.com/Article/details/gqmkeronz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.yfazqb.com/Article/details/gyddwahei.sHtML

[Q34] 每组取第一条
来源：http://blog.epnwcf.com/Article/details/gxkhbywxc.sHtML

SELECT * FROM (
来源：http://m.share.yfazqb.com/Article/details/gpwuihuuf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.yfazqb.com/Article/details/ggingqcyj.sHtML

) t WHERE rn = 1;
来源：http://mobile.fktsv.cn/Article/details/gzjgkftka.sHtML

[Q35] 内连接
来源：http://www.share.bbcook.cn/Article/details/gwgbffwvl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.epnwcf.com/Article/details/gobzolyzg.sHtML

[Q36] 左连接
来源：http://3g.fktsv.cn/Article/details/gywylrxmh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.vehdjk.com/Article/details/gwpyngijg.sHtML

[Q37] 右连接
来源：http://read.share.fktsv.cn/Article/details/gvlffvfrh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.bbcook.cn/Article/details/gsqxxadcg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.epnwcf.com/Article/details/gcspxljqx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.bbcook.cn/Article/details/gplqhbxny.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.sjlbkw.cn/Article/details/gxjtcvogq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.bbcook.cn/Article/details/gbvlqfjws.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.tarul.cn/Article/details/gynbkazgs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.epnwcf.com/Article/details/gftafgsaz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.sjlbkw.cn/Article/details/gbsfmqasd.sHtML

[Q41] 多表连接
来源：http://www.m.share.tarul.cn/Article/details/gywhtvsoi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.vehdjk.com/Article/details/gydmefutw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fktsv.cn/Article/details/gtpqahwrj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.tarul.cn/Article/details/gnsnzwzgc.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.bbcook.cn/Article/details/giejnactv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.vehdjk.com/Article/details/gjgwioefd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.tarul.cn/Article/details/gxxpstnyt.sHtML

[Q43] 标量子查询
来源：http://baike.vehdjk.com/Article/details/gewxkxnuz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.epnwcf.com/Article/details/gryvcfzto.sHtML

[Q44] IN 子查询
来源：http://www.blog.tarul.cn/Article/details/gvqmehbus.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.bbcook.cn/Article/details/gyafyimpw.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fktsv.cn/Article/details/gryzzggxv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/grtfrahvz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.epnwcf.com/Article/details/gxbrsosad.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.bbcook.cn/Article/details/gmwecnbyy.sHtML

[Q47] 与平均值比较
来源：http://m.share.epnwcf.com/Article/details/geefternd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.epnwcf.com/Article/details/gqnnwjthr.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.epnwcf.com/Article/details/gsxwvvihz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fktsv.cn/Article/details/gwzrkybcl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.yfazqb.com/Article/details/gavmnyojk.sHtML

[Q49] 更新单行
来源：http://baike.yfazqb.com/Article/details/gaenlrwuf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/gklaeihyo.sHtML

[Q50] 批量更新
来源：http://m.share.bbcook.cn/Article/details/gqlyyglpz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.tarul.cn/Article/details/gzwbbjfqy.sHtML

[Q51] 用子查询更新
来源：http://www.share.tarul.cn/Article/details/gsgbsvotu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.vehdjk.com/Article/details/gtvpkrovi.sHtML

[Q52] 删除指定行
来源：http://wap.sjlbkw.cn/Article/details/gazwhggzz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/giqpuyeay.sHtML

[Q53] 按条件删除
来源：http://mobile.epnwcf.com/Article/details/gekhzvghf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.vehdjk.com/Article/details/gdnvwdldb.sHtML

[Q54] 清空表
来源：http://www.m.share.tarul.cn/Article/details/getjbpzrs.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fktsv.cn/Article/details/gfmjaflfy.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.epnwcf.com/Article/details/gsagiychm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gcrvlntdz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.vehdjk.com/Article/details/gvurwiugc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.epnwcf.com/Article/details/gwjtvevls.sHtML

[Q57] 行号
来源：http://blog.tarul.cn/Article/details/gnhzngtxz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.bbcook.cn/Article/details/gpfmshwtc.sHtML

[Q58] 累计求和
来源：http://wap.epnwcf.com/Article/details/grrewdynq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gwwtvupel.sHtML

[Q59] 分组内累计
来源：http://mobile.yfazqb.com/Article/details/ggwsgrlaw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gcljejudk.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.epnwcf.com/Article/details/gcytxsosl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.epnwcf.com/Article/details/gnveuvamr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.epnwcf.com/Article/details/gzdfigjjn.sHtML

[Q61] 移动平均
来源：http://3g.fktsv.cn/Article/details/glvsclwmj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/grvkobmon.sHtML

[Q62] 分组占比
来源：http://read.share.fktsv.cn/Article/details/gyxtxfpus.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gdbmuqcrd.sHtML

[Q63] 开启事务
来源：http://3g.tarul.cn/Article/details/gsnnrqmfc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.bbcook.cn/Article/details/golwkgebg.sHtML

[Q64] 提交事务
来源：http://mobile.sjlbkw.cn/Article/details/gevdlxbbt.sHtML

COMMIT;
来源：http://blog.fktsv.cn/Article/details/gnzatpnte.sHtML

[Q65] 回滚事务
来源：http://read.share.bbcook.cn/Article/details/glgztbmzc.sHtML

ROLLBACK;
来源：http://blog.fktsv.cn/Article/details/gklxktzti.sHtML

[Q66] 行锁查询
来源：http://baike.fktsv.cn/Article/details/gwjkalcmi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fktsv.cn/Article/details/gcqhqgvtv.sHtML

[Q67] 设置隔离级别
来源：http://mobile.tarul.cn/Article/details/gwyszgxaa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.sjlbkw.cn/Article/details/gxnarwbhq.sHtML

[Q68] 保存点
来源：http://www.share.vehdjk.com/Article/details/gwsulmswl.sHtML

SAVEPOINT sp1;
来源：http://www.blog.yfazqb.com/Article/details/ghyxfvavr.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/golbwcrkq.sHtML

[Q69] 查看执行计划
来源：http://3g.bbcook.cn/Article/details/gvaiaznvn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.bbcook.cn/Article/details/gcgxjnekc.sHtML

[Q70] 更新统计信息
来源：http://blog.yfazqb.com/Article/details/gnaepaggs.sHtML

ANALYZE TABLE users;
来源：http://wap.epnwcf.com/Article/details/gqbhounyk.sHtML

[Q71] 查看建表语句
来源：http://wap.epnwcf.com/Article/details/gbzkdzklw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.yfazqb.com/Article/details/gycmyzcek.sHtML

[Q72] 查看索引
来源：http://www.m.share.vehdjk.com/Article/details/gpaeqfzvn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.tarul.cn/Article/details/gtwmecstw.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/grdrfngsm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.vehdjk.com/Article/details/gzdsgsgop.sHtML

[Q74] 强制使用索引
来源：http://mobile.bbcook.cn/Article/details/gvacjkfrd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.yfazqb.com/Article/details/gzkmsfunb.sHtML

[Q75] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gzpdccmpq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gojycchmb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fktsv.cn/Article/details/gqjwdjobc.sHtML

[Q76] 按天统计
来源：http://baike.vehdjk.com/Article/details/gcdbuggmd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.tarul.cn/Article/details/gtajdmfly.sHtML

[Q77] 时间加减
来源：http://blog.vehdjk.com/Article/details/gmrankgzt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.sjlbkw.cn/Article/details/gjdyixgle.sHtML

[Q78] 当前时间
来源：http://blog.vehdjk.com/Article/details/gjwyujrga.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.yfazqb.com/Article/details/ghuxpwvfo.sHtML

[Q79] 字符串拼接
来源：http://mobile.sjlbkw.cn/Article/details/gvwciokzn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.vehdjk.com/Article/details/giiljtxiu.sHtML

[Q80] 字符串截取
来源：http://blog.fktsv.cn/Article/details/gnjtzngdt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gxrdnzkjc.sHtML

[Q81] 字符串替换
来源：http://blog.tarul.cn/Article/details/gptjxmvdg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.vehdjk.com/Article/details/gjbheufjz.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fktsv.cn/Article/details/gsgxbuznh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gmrceqlhe.sHtML

[Q83] 大小写转换
来源：http://mobile.vehdjk.com/Article/details/gphsktypd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gafjqfupt.sHtML

[Q84] 去除首尾空格
来源：http://read.share.yfazqb.com/Article/details/gkrxwlvjo.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gtwkylrzx.sHtML

[Q85] 数值取整
来源：http://www.blog.sjlbkw.cn/Article/details/gjxttfvtd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.vehdjk.com/Article/details/gjkikugsl.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.sjlbkw.cn/Article/details/gtbkiwiai.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.bbcook.cn/Article/details/gzotnzudf.sHtML

[Q87] JSON 字段做条件
来源：http://3g.epnwcf.com/Article/details/ggzcgsusz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.epnwcf.com/Article/details/gfvfutxdg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fktsv.cn/Article/details/gofqnpeae.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.yfazqb.com/Article/details/gielregsn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/glbrenwxu.sHtML

[Q89] 判断表是否存在
来源：http://baike.sjlbkw.cn/Article/details/ggjepqjtf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.bbcook.cn/Article/details/gsnxvjjjh.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fktsv.cn/Article/details/goprqrlsl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.yfazqb.com/Article/details/gtlrotjwu.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gvhbohjxo.sHtML

R. Bash 专题
来源：http://baike.tarul.cn/Article/details/gcdqyfkwb.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/geodvfkun.sHtML

[R01] shebang 与严格模式
来源：http://baike.sjlbkw.cn/Article/details/ghynjousl.sHtML

#!/usr/bin/env bash
来源：http://3g.yfazqb.com/Article/details/gdiyyeqtx.sHtML

set -euo pipefail
来源：http://read.share.sjlbkw.cn/Article/details/guvddjmiy.sHtML

[R02] 变量赋值与使用
来源：http://blog.sjlbkw.cn/Article/details/gowpewnnx.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.vehdjk.com/Article/details/gpcmdhnkm.sHtML

[R03] 只读变量
来源：http://www.m.share.epnwcf.com/Article/details/gqitoohgo.sHtML

readonly PI=3.14
来源：http://read.share.tarul.cn/Article/details/gntzjavxa.sHtML

[R04] 位置参数
来源：http://www.share.sjlbkw.cn/Article/details/ggbiljikl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.yfazqb.com/Article/details/gbexqasei.sHtML

[R05] 参数默认值
来源：http://baike.bbcook.cn/Article/details/gytuuctun.sHtML

name="${1:-default}"
来源：http://3g.bbcook.cn/Article/details/ghhpshtol.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fktsv.cn/Article/details/gnyjodysr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gdthgzzmz.sHtML

[R07] if 判断文件
来源：http://www.blog.fktsv.cn/Article/details/gsdzvwfxe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fktsv.cn/Article/details/gtjidqdii.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/gsxchqnfj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.sjlbkw.cn/Article/details/gwpilnbgm.sHtML

[R09] 字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gkcuceupa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.yfazqb.com/Article/details/gljsukeys.sHtML

[R10] 正则匹配
来源：http://3g.vehdjk.com/Article/details/gwmkuylsg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.tarul.cn/Article/details/gafbelydr.sHtML

[R11] case 多分支
来源：http://www.m.share.fktsv.cn/Article/details/gwrfeuscs.sHtML

case "$1" in
来源：http://mobile.vehdjk.com/Article/details/gejxpzgwq.sHtML

start) echo "启动" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gaxgxlugc.sHtML

stop)  echo "停止" ;;
来源：http://wap.epnwcf.com/Article/details/gbmnohyww.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.epnwcf.com/Article/details/gkhklhncz.sHtML

esac
来源：http://3g.sjlbkw.cn/Article/details/gcwlwstag.sHtML

[R12] for 遍历文件
来源：http://mobile.bbcook.cn/Article/details/gkrwtneiz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.bbcook.cn/Article/details/gepghzzpn.sHtML

[R13] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/gnndbohth.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gyppxwcma.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gmwrlzjbb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/ghfgjfmed.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/gufblfdcd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.yfazqb.com/Article/details/gboembfzb.sHtML

[R16] until 等待条件
来源：http://www.m.share.tarul.cn/Article/details/gckgdkqnq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/gmfgqpzdj.sHtML

[R17] 数组定义与取值
来源：http://3g.bbcook.cn/Article/details/gobjjxfzd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.epnwcf.com/Article/details/glqufgage.sHtML

[R18] 遍历数组
来源：http://mobile.vehdjk.com/Article/details/gclknemab.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/giqenuusu.sHtML

[R19] 数组长度
来源：http://m.share.tarul.cn/Article/details/gavsclouj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.bbcook.cn/Article/details/ggbkidlhy.sHtML

[R20] 关联数组（字典）
来源：http://www.share.tarul.cn/Article/details/gxadzgoqd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.tarul.cn/Article/details/ginnvtbnh.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/gslnusvak.sHtML

echo "${#s}"
来源：http://m.share.yfazqb.com/Article/details/gxhrusiwl.sHtML

[R22] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gnchyaehu.sHtML

echo "${s:0:5}"
来源：http://mobile.tarul.cn/Article/details/gjesudncs.sHtML

[R23] 字符串替换
来源：http://baike.bbcook.cn/Article/details/gvwnyocpl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.bbcook.cn/Article/details/gpxyrbigd.sHtML

[R24] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gzyfoxxkl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.bbcook.cn/Article/details/gmmgumiip.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.vehdjk.com/Article/details/gfyjeshge.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.bbcook.cn/Article/details/gnfhvvote.sHtML

[R26] 命令替换
来源：http://www.m.share.epnwcf.com/Article/details/grzvoljjd.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.sjlbkw.cn/Article/details/gafkoejel.sHtML

[R27] 算术展开
来源：http://blog.epnwcf.com/Article/details/gwzcrfirq.sHtML

echo $((1 + 2 * 3))
来源：http://3g.sjlbkw.cn/Article/details/gqneyusit.sHtML

[R28] 浮点运算
来源：http://read.share.fktsv.cn/Article/details/gukxxbufl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fktsv.cn/Article/details/gkcgjosmh.sHtML

[R29] 定义函数
来源：http://mobile.fktsv.cn/Article/details/gtvpryehi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.tarul.cn/Article/details/gqzlwjgnx.sHtML

[R30] 函数返回状态码
来源：http://www.blog.yfazqb.com/Article/details/gbmetuvyn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.yfazqb.com/Article/details/gycuwbudo.sHtML

[R31] 局部变量
来源：http://wap.fktsv.cn/Article/details/gwqhanvwm.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.epnwcf.com/Article/details/gkhqzogll.sHtML

[R32] 参数个数校验
来源：http://3g.yfazqb.com/Article/details/gkxkxfesl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/gwdpbnszu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.vehdjk.com/Article/details/geambcuwq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.sjlbkw.cn/Article/details/gbuspgamb.sHtML

[R34] 退出时清理
来源：http://www.share.vehdjk.com/Article/details/gyjjjaict.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.bbcook.cn/Article/details/gujuchivt.sHtML

[R35] 后台执行并等待
来源：http://3g.bbcook.cn/Article/details/gmmevyquq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.bbcook.cn/Article/details/gexkoajzu.sHtML

[R36] 并发执行多个任务
来源：http://www.share.vehdjk.com/Article/details/ggwhxlgru.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.tarul.cn/Article/details/gbcvpyhlz.sHtML

[R37] 把输出赋给变量
来源：http://3g.vehdjk.com/Article/details/gipcvlhma.sHtML

files=$(ls -1)
来源：http://blog.vehdjk.com/Article/details/gzupnvrgx.sHtML

[R38] 管道串联
来源：http://read.share.bbcook.cn/Article/details/gdgxeuhip.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.vehdjk.com/Article/details/gpfbbbfpl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.tarul.cn/Article/details/gztixtros.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gzciqhjah.sHtML

[R40] 追加写日志
来源：http://read.share.yfazqb.com/Article/details/gncyaoewk.sHtML

echo "log" >> out.log
来源：http://www.m.share.fktsv.cn/Article/details/gyuqvwjnx.sHtML

[R41] 丢弃输出
来源：http://www.share.epnwcf.com/Article/details/gclsimqya.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fktsv.cn/Article/details/gchzrepop.sHtML

[R42] 输入重定向
来源：http://www.share.sjlbkw.cn/Article/details/ghkectxbc.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/gfiwrzscc.sHtML

[R43] 按名字查找文件
来源：http://www.share.yfazqb.com/Article/details/glublisfj.sHtML

find . -name "*.log" -type f
来源：http://www.blog.vehdjk.com/Article/details/gxvtymaov.sHtML

[R44] 按修改时间查找
来源：http://www.share.sjlbkw.cn/Article/details/givqqvejv.sHtML

find . -mtime -7 -type f
来源：http://blog.yfazqb.com/Article/details/gfsbrluoi.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzhiaxkl.sHtML

find . -name "*.tmp" -delete
来源：http://baike.bbcook.cn/Article/details/gdllqgkih.sHtML

[R46] 递归替换文件内容
来源：http://read.share.tarul.cn/Article/details/gutfbtxhn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.bbcook.cn/Article/details/gpfvywstk.sHtML

[R47] sed 单行替换
来源：http://3g.epnwcf.com/Article/details/gmdyuhjwr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.bbcook.cn/Article/details/gqbratuai.sHtML

[R48] awk 取指定列
来源：http://blog.tarul.cn/Article/details/ghcyinica.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gcuxqgpxw.sHtML

[R49] awk 带条件
来源：http://www.m.share.bbcook.cn/Article/details/gpbpqifky.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.vehdjk.com/Article/details/gbulapghg.sHtML

[R50] awk 求和
来源：http://mobile.bbcook.cn/Article/details/gnszpwwoa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gyjnhvczk.sHtML

[R51] 排序去重取前几
来源：http://3g.yfazqb.com/Article/details/gdmidkgfi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.vehdjk.com/Article/details/gxezgflet.sHtML

[R52] 统计行数
来源：http://mobile.epnwcf.com/Article/details/gkspxjgwg.sHtML

wc -l a.txt
来源：http://baike.fktsv.cn/Article/details/gpvrfxvgf.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fktsv.cn/Article/details/govujkgpb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.vehdjk.com/Article/details/givgmmpvq.sHtML

[R54] 比较两个文件
来源：http://blog.bbcook.cn/Article/details/gzccwrxdz.sHtML

diff a.txt b.txt
来源：http://read.share.tarul.cn/Article/details/gdaklvhfp.sHtML

[R55] 压缩与解压
来源：http://mobile.fktsv.cn/Article/details/gqlehmfud.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.tarul.cn/Article/details/gtlgziapm.sHtML

[R56] 远程拷贝
来源：http://www.blog.epnwcf.com/Article/details/gmxypugqu.sHtML

scp file user@host:/path/
来源：http://m.share.vehdjk.com/Article/details/glyfaonva.sHtML

[R57] 远程执行命令
来源：http://www.share.sjlbkw.cn/Article/details/gaelcjctu.sHtML

ssh user@host 'uptime'
来源：http://baike.bbcook.cn/Article/details/gderksevd.sHtML

[R58] 下载文件
来源：http://baike.yfazqb.com/Article/details/guaskcytq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fktsv.cn/Article/details/gkzbawrrs.sHtML

[R59] 发 POST JSON
来源：http://wap.epnwcf.com/Article/details/gksjmwtou.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/gslicaymi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/gohasoaiy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.yfazqb.com/Article/details/gskekouyp.sHtML

[R61] 磁盘占用
来源：http://wap.bbcook.cn/Article/details/ggjyrhokm.sHtML

df -h;  du -sh *
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmvvxqje.sHtML

[R62] 找最占空间的文件
来源：http://blog.vehdjk.com/Article/details/gdisxxnuw.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.yfazqb.com/Article/details/glwjebjhz.sHtML

[R63] 内存与进程
来源：http://wap.fktsv.cn/Article/details/gdmstkedl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.yfazqb.com/Article/details/gnfmetarf.sHtML

[R64] 结束进程
来源：http://www.share.tarul.cn/Article/details/gnrmpfrzv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.tarul.cn/Article/details/gfbyfdxlh.sHtML

[R65] 查看端口占用
来源：http://www.share.sjlbkw.cn/Article/details/gmidwecfj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.vehdjk.com/Article/details/gangblnhk.sHtML

[R66] 定时任务
来源：http://www.share.yfazqb.com/Article/details/gtejgxett.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.tarul.cn/Article/details/gfrkufojk.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fktsv.cn/Article/details/gqsbtswmd.sHtML

openssl rand -hex 16
来源：http://www.blog.bbcook.cn/Article/details/gbpqlwooz.sHtML

[R68] 计算文件校验值
来源：http://3g.sjlbkw.cn/Article/details/gaarkrioh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.tarul.cn/Article/details/gvquhhfgh.sHtML

[R69] 生成随机密码
来源：http://blog.sjlbkw.cn/Article/details/gnycqwang.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fktsv.cn/Article/details/gecnqrbjw.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fktsv.cn/Article/details/gwlmelrqf.sHtML

date +%s;  date -d @1700000000
来源：http://blog.sjlbkw.cn/Article/details/gvaorqtsz.sHtML

[R71] 日期格式化
来源：http://wap.fktsv.cn/Article/details/gtujxttea.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.yfazqb.com/Article/details/gfgnburyc.sHtML

[R72] 等待端口就绪
来源：http://www.blog.epnwcf.com/Article/details/gvcvxnqsf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/gmxxrhbzn.sHtML

[R73] 分割大日志
来源：http://blog.yfazqb.com/Article/details/gfhagjdae.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.yfazqb.com/Article/details/gixvytqir.sHtML

[R74] 批量重命名
来源：http://baike.yfazqb.com/Article/details/gpfqcjzhl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.tarul.cn/Article/details/gtqaropvv.sHtML

[R75] 导出环境变量
来源：http://www.blog.epnwcf.com/Article/details/gekvujsyl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.yfazqb.com/Article/details/gdpwdbwda.sHtML

[R76] 使用临时文件
来源：http://m.share.sjlbkw.cn/Article/details/gieozfukf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gktrkdtyf.sHtML

[R77] 读取用户输入
来源：http://baike.sjlbkw.cn/Article/details/gnwuryuau.sHtML

read -rp "请输入: " ans
来源：http://read.share.vehdjk.com/Article/details/gmpcfswap.sHtML

[R78] 交互式菜单
来源：http://wap.fktsv.cn/Article/details/gsckzpdbl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gajlgiygx.sHtML

[R79] 解析命令行选项
来源：http://blog.bbcook.cn/Article/details/gylmjwidj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.epnwcf.com/Article/details/gjllnstbf.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.tarul.cn/Article/details/gthtcpoip.sHtML

time ./run.sh
来源：http://baike.yfazqb.com/Article/details/gyeflljvl.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gzrwleaeh.sHtML

S. C / C++ 专题
来源：http://m.share.tarul.cn/Article/details/grobwopbz.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvekaqoqw.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/gywayviiu.sHtML

#include <stdio.h>
来源：http://blog.epnwcf.com/Article/details/gwjelenha.sHtML


<!-- 参考信息 -->