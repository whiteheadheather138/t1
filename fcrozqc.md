代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.yfazqb.com/Article/details/gcqapgvvc.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gvwmljbqg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gaqhyzlxn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.bbcook.cn/Article/details/gjzvkjzlt.sHtML

[Q33] 多列分组
来源：http://baike.bbcook.cn/Article/details/gfziatxoy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.tarul.cn/Article/details/gycflanmz.sHtML

[Q34] 每组取第一条
来源：http://baike.tarul.cn/Article/details/gwxveatcn.sHtML

SELECT * FROM (
来源：http://wap.vehdjk.com/Article/details/gnrbdbfru.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fktsv.cn/Article/details/gnonkkrfl.sHtML

) t WHERE rn = 1;
来源：http://read.share.bbcook.cn/Article/details/gidusqchx.sHtML

[Q35] 内连接
来源：http://wap.yfazqb.com/Article/details/ghoxuxvnd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gxczytzwm.sHtML

[Q36] 左连接
来源：http://3g.vehdjk.com/Article/details/gjgegzyrd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/guomoiclo.sHtML

[Q37] 右连接
来源：http://mobile.fktsv.cn/Article/details/goszclopr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.sjlbkw.cn/Article/details/gqljtmgba.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.bbcook.cn/Article/details/goabiqjkj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.bbcook.cn/Article/details/gakefnovz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.yfazqb.com/Article/details/gnujamhiu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fktsv.cn/Article/details/gmimxnfed.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.epnwcf.com/Article/details/ggqdfmlgx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.bbcook.cn/Article/details/gwactdsmp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/gysyhmgim.sHtML

[Q41] 多表连接
来源：http://read.share.sjlbkw.cn/Article/details/glwopnfzf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/ghhskhlxj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.yfazqb.com/Article/details/gqyjednzh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.sjlbkw.cn/Article/details/gbphuysfq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.tarul.cn/Article/details/gpwmgbsjb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.bbcook.cn/Article/details/ggekwiukg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.bbcook.cn/Article/details/gxlnnwoas.sHtML

[Q43] 标量子查询
来源：http://m.share.sjlbkw.cn/Article/details/gzmcfwujl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.bbcook.cn/Article/details/gobypmxjn.sHtML

[Q44] IN 子查询
来源：http://3g.tarul.cn/Article/details/gkxxauksh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.vehdjk.com/Article/details/gmbzdnpok.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fktsv.cn/Article/details/gijhbuwhd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/grnpqyiqm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.sjlbkw.cn/Article/details/godimtjzn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.vehdjk.com/Article/details/gsdpvuvyp.sHtML

[Q47] 与平均值比较
来源：http://m.share.tarul.cn/Article/details/gdncubtjy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.tarul.cn/Article/details/gnrhsopca.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.vehdjk.com/Article/details/gqxsorhmf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.epnwcf.com/Article/details/gfkncdnvw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.sjlbkw.cn/Article/details/gkjmhwuhy.sHtML

[Q49] 更新单行
来源：http://baike.bbcook.cn/Article/details/gcflwlgss.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/gtlfesnmc.sHtML

[Q50] 批量更新
来源：http://mobile.epnwcf.com/Article/details/gjdpbctyq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.yfazqb.com/Article/details/gaytykqjg.sHtML

[Q51] 用子查询更新
来源：http://3g.fktsv.cn/Article/details/glqqljjwy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.yfazqb.com/Article/details/giydkynni.sHtML

[Q52] 删除指定行
来源：http://m.share.vehdjk.com/Article/details/gphxzgwrv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gkzgkeyrs.sHtML

[Q53] 按条件删除
来源：http://read.share.yfazqb.com/Article/details/gknjamrai.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.bbcook.cn/Article/details/gsdnlxkpk.sHtML

[Q54] 清空表
来源：http://m.share.epnwcf.com/Article/details/gdhasaxcz.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.vehdjk.com/Article/details/giibvhncq.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.bbcook.cn/Article/details/gvtaublcl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.yfazqb.com/Article/details/gpyukxira.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.epnwcf.com/Article/details/gjngytndw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.yfazqb.com/Article/details/gekdesouz.sHtML

[Q57] 行号
来源：http://m.share.vehdjk.com/Article/details/gqezdjlqt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.epnwcf.com/Article/details/gqvjwjdcd.sHtML

[Q58] 累计求和
来源：http://m.share.epnwcf.com/Article/details/gxomdrqbb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gplovyyjk.sHtML

[Q59] 分组内累计
来源：http://wap.fktsv.cn/Article/details/gqhgnuype.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gadkcqsbn.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.tarul.cn/Article/details/gvozqfbwf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.vehdjk.com/Article/details/gwtmkazgy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gnmwxficy.sHtML

[Q61] 移动平均
来源：http://3g.bbcook.cn/Article/details/gqogwouwl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gblnhukpb.sHtML

[Q62] 分组占比
来源：http://www.share.fktsv.cn/Article/details/geveubbsu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gyuuivswt.sHtML

[Q63] 开启事务
来源：http://3g.epnwcf.com/Article/details/gqrytahiy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.tarul.cn/Article/details/gkxgecavw.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gtnbzfzdz.sHtML

COMMIT;
来源：http://mobile.sjlbkw.cn/Article/details/gjihvkabu.sHtML

[Q65] 回滚事务
来源：http://m.share.epnwcf.com/Article/details/gdvvlhhjq.sHtML

ROLLBACK;
来源：http://www.blog.epnwcf.com/Article/details/gnztfyftv.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fktsv.cn/Article/details/gccgioltn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.yfazqb.com/Article/details/gvzngradr.sHtML

[Q67] 设置隔离级别
来源：http://blog.vehdjk.com/Article/details/gdgjxnabx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.epnwcf.com/Article/details/gqpubkxag.sHtML

[Q68] 保存点
来源：http://www.blog.sjlbkw.cn/Article/details/gvwamwdfk.sHtML

SAVEPOINT sp1;
来源：http://mobile.sjlbkw.cn/Article/details/gnfjpgkwd.sHtML

ROLLBACK TO sp1;
来源：http://read.share.vehdjk.com/Article/details/gykkzkrpf.sHtML

[Q69] 查看执行计划
来源：http://www.share.vehdjk.com/Article/details/gktxrxbcv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.yfazqb.com/Article/details/gewtiwxsg.sHtML

[Q70] 更新统计信息
来源：http://baike.bbcook.cn/Article/details/gjsegewhp.sHtML

ANALYZE TABLE users;
来源：http://baike.fktsv.cn/Article/details/gzokximry.sHtML

[Q71] 查看建表语句
来源：http://read.share.bbcook.cn/Article/details/glgzmfdfn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.bbcook.cn/Article/details/gqaaayugu.sHtML

[Q72] 查看索引
来源：http://www.m.share.vehdjk.com/Article/details/goradoewm.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gcgqcypbg.sHtML

[Q73] 查看表状态
来源：http://baike.tarul.cn/Article/details/gbbxhmgml.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.vehdjk.com/Article/details/gdvehkjau.sHtML

[Q74] 强制使用索引
来源：http://m.share.sjlbkw.cn/Article/details/gwnqfmxtf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.yfazqb.com/Article/details/ggwfvceik.sHtML

[Q75] 日期格式化
来源：http://3g.fktsv.cn/Article/details/gypglglpu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/glpsdybme.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.epnwcf.com/Article/details/ggqyciqit.sHtML

[Q76] 按天统计
来源：http://read.share.yfazqb.com/Article/details/gswqpyteu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.bbcook.cn/Article/details/gspuuusdi.sHtML

[Q77] 时间加减
来源：http://www.blog.vehdjk.com/Article/details/glhsqmkky.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.bbcook.cn/Article/details/gavstrkma.sHtML

[Q78] 当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gghwoqaod.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.epnwcf.com/Article/details/gkcoljsoe.sHtML

[Q79] 字符串拼接
来源：http://www.share.epnwcf.com/Article/details/gjgebmfpq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.sjlbkw.cn/Article/details/gkrihorun.sHtML

[Q80] 字符串截取
来源：http://blog.vehdjk.com/Article/details/gmtfwgwso.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gzbcugakl.sHtML

[Q81] 字符串替换
来源：http://blog.fktsv.cn/Article/details/gnzspgwjp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.epnwcf.com/Article/details/gzyzcsooq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fktsv.cn/Article/details/gphlmscbk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/grgaeahjn.sHtML

[Q83] 大小写转换
来源：http://blog.vehdjk.com/Article/details/guidnionk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gbnkfffvm.sHtML

[Q84] 去除首尾空格
来源：http://mobile.yfazqb.com/Article/details/gursokwfg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gkyujqrxq.sHtML

[Q85] 数值取整
来源：http://www.share.sjlbkw.cn/Article/details/geataiqrd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.vehdjk.com/Article/details/gqmcpwutu.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.yfazqb.com/Article/details/grkjxbrjr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.bbcook.cn/Article/details/ghxviaggs.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.bbcook.cn/Article/details/gleiurzed.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fktsv.cn/Article/details/goouvfdmx.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.tarul.cn/Article/details/gjqmskrnx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.sjlbkw.cn/Article/details/gdpkaljwq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.bbcook.cn/Article/details/gabmafuzr.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fktsv.cn/Article/details/gagvekfme.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.tarul.cn/Article/details/gdxzamuzn.sHtML

[Q90] 生成序号列
来源：http://www.share.vehdjk.com/Article/details/gumpqozfb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.epnwcf.com/Article/details/gikawhztx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gayeyncvq.sHtML

R. Bash 专题
来源：http://wap.sjlbkw.cn/Article/details/gmhdyeduw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfdrkrzfm.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.sjlbkw.cn/Article/details/gkeogtzbs.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/gglzhqhkz.sHtML

set -euo pipefail
来源：http://www.share.sjlbkw.cn/Article/details/grquijbhx.sHtML

[R02] 变量赋值与使用
来源：http://m.share.vehdjk.com/Article/details/gvpsjvfdf.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.tarul.cn/Article/details/gpowmwtwv.sHtML

[R03] 只读变量
来源：http://m.share.fktsv.cn/Article/details/gngmfpdvl.sHtML

readonly PI=3.14
来源：http://m.share.yfazqb.com/Article/details/gygompxvp.sHtML

[R04] 位置参数
来源：http://mobile.sjlbkw.cn/Article/details/gtjigeahv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.sjlbkw.cn/Article/details/gdszvmkpj.sHtML

[R05] 参数默认值
来源：http://wap.vehdjk.com/Article/details/gynhnfcbe.sHtML

name="${1:-default}"
来源：http://blog.yfazqb.com/Article/details/gumpqblve.sHtML

[R06] 判断命令是否存在
来源：http://www.share.yfazqb.com/Article/details/gwzmrllho.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/guywycvoh.sHtML

[R07] if 判断文件
来源：http://blog.sjlbkw.cn/Article/details/gksayfcry.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.yfazqb.com/Article/details/gskwinooi.sHtML

[R08] 数值比较
来源：http://www.m.share.fktsv.cn/Article/details/ggonblqfu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gtbpmevse.sHtML

[R09] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gqkabkkoq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.yfazqb.com/Article/details/glqrrzvfm.sHtML

[R10] 正则匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gvkcmgrkd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gtvqppteb.sHtML

[R11] case 多分支
来源：http://read.share.fktsv.cn/Article/details/gatdlxbyu.sHtML

case "$1" in
来源：http://baike.yfazqb.com/Article/details/gjihqxhpj.sHtML

start) echo "启动" ;;
来源：http://3g.bbcook.cn/Article/details/gazgiymxg.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.tarul.cn/Article/details/gcoqdwqct.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fktsv.cn/Article/details/gbwjqjmbr.sHtML

esac
来源：http://www.blog.fktsv.cn/Article/details/gnfapnlie.sHtML

[R12] for 遍历文件
来源：http://baike.tarul.cn/Article/details/gagqanajc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.vehdjk.com/Article/details/gsanhmakn.sHtML

[R13] for 计数循环
来源：http://m.share.yfazqb.com/Article/details/gofauerjo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/ghglezrkh.sHtML

[R14] C 风格 for
来源：http://www.blog.sjlbkw.cn/Article/details/gnzytakdr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.tarul.cn/Article/details/gghlhqzbp.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gjhkkqbvb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fktsv.cn/Article/details/grohelrzy.sHtML

[R16] until 等待条件
来源：http://www.m.share.fktsv.cn/Article/details/gcpgqymht.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/goamvften.sHtML

[R17] 数组定义与取值
来源：http://blog.vehdjk.com/Article/details/gyzcefczm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.tarul.cn/Article/details/glvpidacd.sHtML

[R18] 遍历数组
来源：http://baike.vehdjk.com/Article/details/gzfdlhmhg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.bbcook.cn/Article/details/gtrsxdelg.sHtML

[R19] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gwswxklqv.sHtML

echo "${#arr[@]}"
来源：http://wap.yfazqb.com/Article/details/gsuafjxcp.sHtML

[R20] 关联数组（字典）
来源：http://www.share.tarul.cn/Article/details/gcxocagxa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.vehdjk.com/Article/details/gzqciknqn.sHtML

[R21] 字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gvgoshuuf.sHtML

echo "${#s}"
来源：http://mobile.epnwcf.com/Article/details/gwawqrdpd.sHtML

[R22] 截取子串
来源：http://www.share.bbcook.cn/Article/details/gmgewqfmo.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/gsymvqhwc.sHtML

[R23] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gouwasrjc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoeckgfe.sHtML

[R24] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gygpuwmqq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.bbcook.cn/Article/details/gegeqogku.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fktsv.cn/Article/details/gboyxtyzv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.yfazqb.com/Article/details/giffasnxw.sHtML

[R26] 命令替换
来源：http://www.blog.fktsv.cn/Article/details/gxusjqipk.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.yfazqb.com/Article/details/gegbcpkix.sHtML

[R27] 算术展开
来源：http://read.share.tarul.cn/Article/details/gyaqojomi.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.yfazqb.com/Article/details/gveftzwst.sHtML

[R28] 浮点运算
来源：http://mobile.fktsv.cn/Article/details/gpfxeebtj.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.bbcook.cn/Article/details/gdzqxiptf.sHtML

[R29] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gxgmtpdrd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.epnwcf.com/Article/details/gtuesvixo.sHtML

[R30] 函数返回状态码
来源：http://mobile.epnwcf.com/Article/details/goijuoxlz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fktsv.cn/Article/details/gwnikmbtt.sHtML

[R31] 局部变量
来源：http://www.blog.yfazqb.com/Article/details/guhetcijy.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.tarul.cn/Article/details/gjvkrijlb.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/gaqxrmlel.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gtoihupgs.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.vehdjk.com/Article/details/gjpuanoaf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.sjlbkw.cn/Article/details/gfdzcfren.sHtML

[R34] 退出时清理
来源：http://www.m.share.sjlbkw.cn/Article/details/grpatmojs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gdptbgwss.sHtML

[R35] 后台执行并等待
来源：http://baike.tarul.cn/Article/details/geemnbmmj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.epnwcf.com/Article/details/gdnonzvqq.sHtML

[R36] 并发执行多个任务
来源：http://blog.vehdjk.com/Article/details/gyykvupgx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.sjlbkw.cn/Article/details/gqjdjymlq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.yfazqb.com/Article/details/gccrbszrf.sHtML

files=$(ls -1)
来源：http://m.share.epnwcf.com/Article/details/guhfqwfye.sHtML

[R38] 管道串联
来源：http://www.m.share.bbcook.cn/Article/details/goaneylvt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.tarul.cn/Article/details/gbegumgbv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fktsv.cn/Article/details/gqtlcxikm.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/ggcyoyhwl.sHtML

[R40] 追加写日志
来源：http://www.blog.fktsv.cn/Article/details/glajditod.sHtML

echo "log" >> out.log
来源：http://mobile.tarul.cn/Article/details/gmzyhuddg.sHtML

[R41] 丢弃输出
来源：http://baike.yfazqb.com/Article/details/gchtbjajm.sHtML

cmd >/dev/null 2>&1
来源：http://blog.yfazqb.com/Article/details/gbafvewva.sHtML

[R42] 输入重定向
来源：http://blog.vehdjk.com/Article/details/guhkifaeh.sHtML

wc -l < a.txt
来源：http://mobile.epnwcf.com/Article/details/gltzmtxht.sHtML

[R43] 按名字查找文件
来源：http://mobile.fktsv.cn/Article/details/ghvxqwruq.sHtML

find . -name "*.log" -type f
来源：http://read.share.vehdjk.com/Article/details/ghezgsusr.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmnddabw.sHtML

find . -mtime -7 -type f
来源：http://wap.sjlbkw.cn/Article/details/gbebahten.sHtML

[R45] 批量删除
来源：http://wap.yfazqb.com/Article/details/gnhizbabf.sHtML

find . -name "*.tmp" -delete
来源：http://baike.sjlbkw.cn/Article/details/gzhxzjtjy.sHtML

[R46] 递归替换文件内容
来源：http://read.share.vehdjk.com/Article/details/ggoqtzkch.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.vehdjk.com/Article/details/grdhzvums.sHtML

[R47] sed 单行替换
来源：http://blog.yfazqb.com/Article/details/gnkkypuaw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.bbcook.cn/Article/details/gvwcgaxib.sHtML

[R48] awk 取指定列
来源：http://www.share.fktsv.cn/Article/details/gmkpryijh.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.yfazqb.com/Article/details/gfksanyyi.sHtML

[R49] awk 带条件
来源：http://www.share.epnwcf.com/Article/details/ggvbcojff.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fktsv.cn/Article/details/gcxqmuupu.sHtML

[R50] awk 求和
来源：http://blog.vehdjk.com/Article/details/gollhjtwt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fktsv.cn/Article/details/gbcekubnr.sHtML

[R51] 排序去重取前几
来源：http://m.share.epnwcf.com/Article/details/gybuawrve.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.yfazqb.com/Article/details/gqsfvxqen.sHtML

[R52] 统计行数
来源：http://www.m.share.yfazqb.com/Article/details/gwtzoiwcz.sHtML

wc -l a.txt
来源：http://m.share.vehdjk.com/Article/details/giixmwwqi.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.yfazqb.com/Article/details/gvecjfpwu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fktsv.cn/Article/details/gmcneimnp.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/gwlujndlc.sHtML

diff a.txt b.txt
来源：http://www.m.share.bbcook.cn/Article/details/gigkhnlbk.sHtML

[R55] 压缩与解压
来源：http://m.share.bbcook.cn/Article/details/gvemvtllv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fktsv.cn/Article/details/gwycqswmg.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/gigqyvdmj.sHtML

scp file user@host:/path/
来源：http://3g.vehdjk.com/Article/details/giweaprdh.sHtML

[R57] 远程执行命令
来源：http://www.blog.sjlbkw.cn/Article/details/gqedqhtxk.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.vehdjk.com/Article/details/gfmxrjvcl.sHtML

[R58] 下载文件
来源：http://baike.yfazqb.com/Article/details/ggzhmbnka.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fktsv.cn/Article/details/gycptqmit.sHtML

[R59] 发 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gftkhhime.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.tarul.cn/Article/details/gckreijag.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gkzceouxy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.yfazqb.com/Article/details/gbuajxwjc.sHtML

[R61] 磁盘占用
来源：http://read.share.sjlbkw.cn/Article/details/gwjkypttz.sHtML

df -h;  du -sh *
来源：http://www.m.share.tarul.cn/Article/details/glsjynbeo.sHtML

[R62] 找最占空间的文件
来源：http://read.share.bbcook.cn/Article/details/gsjbvtygy.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.vehdjk.com/Article/details/gwqvgkqhm.sHtML

[R63] 内存与进程
来源：http://www.m.share.vehdjk.com/Article/details/gvmfohwiq.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/gzorkrcre.sHtML

[R64] 结束进程
来源：http://www.m.share.yfazqb.com/Article/details/guuwtnhwa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.bbcook.cn/Article/details/ghsgctryq.sHtML

[R65] 查看端口占用
来源：http://m.share.sjlbkw.cn/Article/details/gcjylmwlr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.epnwcf.com/Article/details/gbeaqnvkw.sHtML

[R66] 定时任务
来源：http://m.share.vehdjk.com/Article/details/gbrpgudjt.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoyklhes.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.bbcook.cn/Article/details/gkfwzpios.sHtML

openssl rand -hex 16
来源：http://mobile.bbcook.cn/Article/details/gjcjxzlil.sHtML

[R68] 计算文件校验值
来源：http://m.share.epnwcf.com/Article/details/gobrszdaw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.bbcook.cn/Article/details/gjnzjlfvs.sHtML

[R69] 生成随机密码
来源：http://m.share.fktsv.cn/Article/details/gfbxlkgbs.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.sjlbkw.cn/Article/details/gwmufthsj.sHtML

[R70] 时间戳与互转
来源：http://mobile.fktsv.cn/Article/details/goirleevu.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.epnwcf.com/Article/details/gjkxeodcj.sHtML

[R71] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/gweuhmhai.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.vehdjk.com/Article/details/gkwboyqmz.sHtML

[R72] 等待端口就绪
来源：http://mobile.fktsv.cn/Article/details/ggguzwcdv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/givappfcn.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/ggwewgzoi.sHtML

split -l 1000 big.log part_
来源：http://wap.bbcook.cn/Article/details/gciofyfbb.sHtML

[R74] 批量重命名
来源：http://www.blog.vehdjk.com/Article/details/gdfxcmvkc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.bbcook.cn/Article/details/gdodznfln.sHtML

[R75] 导出环境变量
来源：http://mobile.fktsv.cn/Article/details/gevsvayjr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.tarul.cn/Article/details/gxqjzdias.sHtML

[R76] 使用临时文件
来源：http://www.m.share.vehdjk.com/Article/details/gpkfyksjn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fktsv.cn/Article/details/gnablzchy.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gwlxqbgaf.sHtML

read -rp "请输入: " ans
来源：http://blog.bbcook.cn/Article/details/gvkenfhgx.sHtML

[R78] 交互式菜单
来源：http://mobile.yfazqb.com/Article/details/gcujougze.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.yfazqb.com/Article/details/gusvvgiva.sHtML

[R79] 解析命令行选项
来源：http://mobile.fktsv.cn/Article/details/gpszycxaw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.vehdjk.com/Article/details/gpatdqorv.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/gmmkpdksh.sHtML

time ./run.sh
来源：http://www.share.vehdjk.com/Article/details/gtcsdcfhh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/glxygxmuy.sHtML


<!-- 参考信息 -->