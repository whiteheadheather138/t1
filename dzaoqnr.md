代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fktsv.cn/Article/details/guijdjvjg.sHtML

[Q30] 分组统计
来源：http://baike.vehdjk.com/Article/details/ggpqdsmkt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gfsarjhas.sHtML

[Q31] 分组后过滤
来源：http://www.share.vehdjk.com/Article/details/gmdywpbjz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.sjlbkw.cn/Article/details/glfbzhanu.sHtML

[Q32] 分组拼接字符串
来源：http://3g.yfazqb.com/Article/details/gqnwdlfev.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gcayvealo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.tarul.cn/Article/details/gseztqcsu.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/gdkmnxhot.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.vehdjk.com/Article/details/gidzhzuzd.sHtML

[Q34] 每组取第一条
来源：http://www.blog.yfazqb.com/Article/details/gmhbfsagh.sHtML

SELECT * FROM (
来源：http://blog.sjlbkw.cn/Article/details/guhztemdu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.epnwcf.com/Article/details/gmjmguxhq.sHtML

) t WHERE rn = 1;
来源：http://3g.vehdjk.com/Article/details/gxgupexue.sHtML

[Q35] 内连接
来源：http://read.share.sjlbkw.cn/Article/details/gqewdbskt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/gmchidlcl.sHtML

[Q36] 左连接
来源：http://wap.vehdjk.com/Article/details/gaijwpphg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/gccxskawu.sHtML

[Q37] 右连接
来源：http://baike.yfazqb.com/Article/details/gicdbqpig.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.sjlbkw.cn/Article/details/gntnhlkxl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.tarul.cn/Article/details/gkmjffvmt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.sjlbkw.cn/Article/details/gotgzyybz.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.vehdjk.com/Article/details/guldkerum.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.tarul.cn/Article/details/gyqwibfdu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.bbcook.cn/Article/details/gzlqqrjrz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.yfazqb.com/Article/details/grvohhsnd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.epnwcf.com/Article/details/grnknoggn.sHtML

[Q41] 多表连接
来源：http://wap.sjlbkw.cn/Article/details/gyomwcrbw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fktsv.cn/Article/details/gscrqykva.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.epnwcf.com/Article/details/garrcuzwu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.vehdjk.com/Article/details/gotgzihiy.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.vehdjk.com/Article/details/gomffeaoc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.yfazqb.com/Article/details/glkugivfz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.bbcook.cn/Article/details/gqvahypdz.sHtML

[Q43] 标量子查询
来源：http://blog.epnwcf.com/Article/details/gncrtzfsi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.yfazqb.com/Article/details/gvybrjmaq.sHtML

[Q44] IN 子查询
来源：http://wap.vehdjk.com/Article/details/gsbxkrywg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.epnwcf.com/Article/details/guzxrfnis.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.tarul.cn/Article/details/gdqpdlzdz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gjlbusdda.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.bbcook.cn/Article/details/gmosgaqbj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/guhajojdp.sHtML

[Q47] 与平均值比较
来源：http://www.share.epnwcf.com/Article/details/ghabmzbli.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.tarul.cn/Article/details/gzcpgeclp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.bbcook.cn/Article/details/gjpwkxdto.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.tarul.cn/Article/details/gunsujald.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.tarul.cn/Article/details/gmiwkkfch.sHtML

[Q49] 更新单行
来源：http://read.share.yfazqb.com/Article/details/gefbdqeke.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/gcllcclkj.sHtML

[Q50] 批量更新
来源：http://read.share.yfazqb.com/Article/details/gouyhiret.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.bbcook.cn/Article/details/gzipatwis.sHtML

[Q51] 用子查询更新
来源：http://baike.tarul.cn/Article/details/gbpyqumvr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.vehdjk.com/Article/details/gubrobuhf.sHtML

[Q52] 删除指定行
来源：http://3g.yfazqb.com/Article/details/gaexzvevx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.vehdjk.com/Article/details/gxfjsilcj.sHtML

[Q53] 按条件删除
来源：http://www.blog.epnwcf.com/Article/details/gdgchcswl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.vehdjk.com/Article/details/gcysdcgmi.sHtML

[Q54] 清空表
来源：http://wap.fktsv.cn/Article/details/ghvwaabra.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fktsv.cn/Article/details/glmtqzbme.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fktsv.cn/Article/details/gkzuviqut.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fktsv.cn/Article/details/gvrudwgsr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.vehdjk.com/Article/details/gzhralqge.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.bbcook.cn/Article/details/gdwbpvgmf.sHtML

[Q57] 行号
来源：http://www.m.share.epnwcf.com/Article/details/ganbcupdq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.bbcook.cn/Article/details/gccpyizkt.sHtML

[Q58] 累计求和
来源：http://read.share.fktsv.cn/Article/details/gkjqiqffy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fktsv.cn/Article/details/gexfudhpu.sHtML

[Q59] 分组内累计
来源：http://3g.vehdjk.com/Article/details/gtbboovte.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gtzzswitg.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.vehdjk.com/Article/details/gwjlpbkri.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.epnwcf.com/Article/details/gkzjlyowl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gifsxriob.sHtML

[Q61] 移动平均
来源：http://wap.sjlbkw.cn/Article/details/glskwjaju.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gdqefwmup.sHtML

[Q62] 分组占比
来源：http://www.blog.bbcook.cn/Article/details/glqvizwyc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/ghcyakrxu.sHtML

[Q63] 开启事务
来源：http://mobile.vehdjk.com/Article/details/gwxpvubsu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.epnwcf.com/Article/details/gtgfzfvyk.sHtML

[Q64] 提交事务
来源：http://read.share.epnwcf.com/Article/details/gcmzrqfsy.sHtML

COMMIT;
来源：http://www.share.sjlbkw.cn/Article/details/gflzxuaia.sHtML

[Q65] 回滚事务
来源：http://blog.bbcook.cn/Article/details/gqoymvapt.sHtML

ROLLBACK;
来源：http://baike.yfazqb.com/Article/details/gkdszslxc.sHtML

[Q66] 行锁查询
来源：http://read.share.sjlbkw.cn/Article/details/gcndqwgad.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.bbcook.cn/Article/details/gjecvahzb.sHtML

[Q67] 设置隔离级别
来源：http://blog.sjlbkw.cn/Article/details/giusadhrw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.tarul.cn/Article/details/gpzeqzykz.sHtML

[Q68] 保存点
来源：http://www.share.vehdjk.com/Article/details/gcgvxogjn.sHtML

SAVEPOINT sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gbhxgfcpl.sHtML

ROLLBACK TO sp1;
来源：http://3g.sjlbkw.cn/Article/details/gpbgtktcf.sHtML

[Q69] 查看执行计划
来源：http://www.share.sjlbkw.cn/Article/details/gitwbsgvq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fktsv.cn/Article/details/geaifxucn.sHtML

[Q70] 更新统计信息
来源：http://www.share.yfazqb.com/Article/details/gvtybleaq.sHtML

ANALYZE TABLE users;
来源：http://blog.vehdjk.com/Article/details/gztrznawz.sHtML

[Q71] 查看建表语句
来源：http://www.share.vehdjk.com/Article/details/gjjwtoogp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.bbcook.cn/Article/details/gmmcolvbj.sHtML

[Q72] 查看索引
来源：http://read.share.sjlbkw.cn/Article/details/gqhnfyilv.sHtML

SHOW INDEX FROM users;
来源：http://read.share.yfazqb.com/Article/details/gjmpnfkzl.sHtML

[Q73] 查看表状态
来源：http://mobile.fktsv.cn/Article/details/grmcpnabt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.vehdjk.com/Article/details/glxxjsmyg.sHtML

[Q74] 强制使用索引
来源：http://blog.yfazqb.com/Article/details/grmfyamyh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.tarul.cn/Article/details/ggdvbhpba.sHtML

[Q75] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gdsbpsaqq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gecmcvekb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.vehdjk.com/Article/details/guniztyzd.sHtML

[Q76] 按天统计
来源：http://blog.epnwcf.com/Article/details/gkgymdcbg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/gdyvasvlr.sHtML

[Q77] 时间加减
来源：http://baike.tarul.cn/Article/details/gmoukqohh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.yfazqb.com/Article/details/glkpgzroa.sHtML

[Q78] 当前时间
来源：http://blog.vehdjk.com/Article/details/gqggmklba.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.vehdjk.com/Article/details/gsjhndaea.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.bbcook.cn/Article/details/gptsvxpsu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fktsv.cn/Article/details/gtgszmohm.sHtML

[Q80] 字符串截取
来源：http://baike.tarul.cn/Article/details/gffqktyby.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.tarul.cn/Article/details/gvnbqjziv.sHtML

[Q81] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/gntlleihh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fktsv.cn/Article/details/gxhwmdkfx.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.vehdjk.com/Article/details/gmqiwklhx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/ggnfnfuay.sHtML

[Q83] 大小写转换
来源：http://wap.yfazqb.com/Article/details/gxmnhrfxb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhlfrfln.sHtML

[Q84] 去除首尾空格
来源：http://wap.epnwcf.com/Article/details/gdbtyxrmz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gjdxhrrqs.sHtML

[Q85] 数值取整
来源：http://baike.epnwcf.com/Article/details/glggmxgki.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.yfazqb.com/Article/details/gorjdsgqv.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fktsv.cn/Article/details/gvglpohuj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/gajxswwgx.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.epnwcf.com/Article/details/gdregzthx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fktsv.cn/Article/details/gwkvgofjd.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.yfazqb.com/Article/details/gjibbijyq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.epnwcf.com/Article/details/gojbfjccr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fktsv.cn/Article/details/ghizyxrls.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gmrledbzl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fktsv.cn/Article/details/gjxumnwyx.sHtML

[Q90] 生成序号列
来源：http://www.m.share.epnwcf.com/Article/details/gbqalwnll.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.tarul.cn/Article/details/gygfeulzg.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzzkotffr.sHtML

R. Bash 专题
来源：http://baike.sjlbkw.cn/Article/details/ggsbhpcai.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdewzlswv.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.tarul.cn/Article/details/gqqmwnkbj.sHtML

#!/usr/bin/env bash
来源：http://3g.sjlbkw.cn/Article/details/gloeoantt.sHtML

set -euo pipefail
来源：http://m.share.vehdjk.com/Article/details/grhcxwasv.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fktsv.cn/Article/details/gvkrbpmxt.sHtML

name="Tom"; echo "$name"
来源：http://wap.bbcook.cn/Article/details/gchfgdjzg.sHtML

[R03] 只读变量
来源：http://blog.sjlbkw.cn/Article/details/gfvyydxlj.sHtML

readonly PI=3.14
来源：http://blog.vehdjk.com/Article/details/gokqixdzx.sHtML

[R04] 位置参数
来源：http://www.m.share.yfazqb.com/Article/details/gftqjaaxo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.bbcook.cn/Article/details/gbndltaoi.sHtML

[R05] 参数默认值
来源：http://m.share.epnwcf.com/Article/details/gtgoiikue.sHtML

name="${1:-default}"
来源：http://www.blog.yfazqb.com/Article/details/gwulmhljw.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.yfazqb.com/Article/details/goyzmycxw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/gohosuuwl.sHtML

[R07] if 判断文件
来源：http://read.share.epnwcf.com/Article/details/gjcijqlyh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.epnwcf.com/Article/details/grnoejuwd.sHtML

[R08] 数值比较
来源：http://wap.epnwcf.com/Article/details/ghqrjkvll.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.tarul.cn/Article/details/golceqpse.sHtML

[R09] 字符串比较
来源：http://mobile.bbcook.cn/Article/details/gyecwmops.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fktsv.cn/Article/details/gktgeaawo.sHtML

[R10] 正则匹配
来源：http://baike.fktsv.cn/Article/details/ggpzhkllx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.sjlbkw.cn/Article/details/ggfrqdphb.sHtML

[R11] case 多分支
来源：http://www.share.epnwcf.com/Article/details/gtroxjbrd.sHtML

case "$1" in
来源：http://mobile.tarul.cn/Article/details/ghvjskffj.sHtML

start) echo "启动" ;;
来源：http://mobile.bbcook.cn/Article/details/gzawlhqtw.sHtML

stop)  echo "停止" ;;
来源：http://read.share.yfazqb.com/Article/details/gfmwusdbw.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gwwszrqwj.sHtML

esac
来源：http://wap.yfazqb.com/Article/details/gefxqvvwe.sHtML

[R12] for 遍历文件
来源：http://mobile.yfazqb.com/Article/details/gllblgrtk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.bbcook.cn/Article/details/gqcexuubr.sHtML

[R13] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/gqbfbnbkq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gtwrikwvz.sHtML

[R14] C 风格 for
来源：http://www.share.epnwcf.com/Article/details/gtqwyiscd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gbeliffco.sHtML

[R15] while 逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gjmjpnhph.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fktsv.cn/Article/details/gfmualvdm.sHtML

[R16] until 等待条件
来源：http://wap.vehdjk.com/Article/details/glutxgtgt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gehjmpqdh.sHtML

[R17] 数组定义与取值
来源：http://m.share.epnwcf.com/Article/details/gshckdwxx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.epnwcf.com/Article/details/geaybbbnm.sHtML

[R18] 遍历数组
来源：http://blog.vehdjk.com/Article/details/glyoxznbn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.vehdjk.com/Article/details/gmundmwog.sHtML

[R19] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gvmkqyihh.sHtML

echo "${#arr[@]}"
来源：http://www.blog.epnwcf.com/Article/details/ggxtsvtzu.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fktsv.cn/Article/details/gdipidbpr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.tarul.cn/Article/details/gchzssmzr.sHtML

[R21] 字符串长度
来源：http://m.share.vehdjk.com/Article/details/givpempkj.sHtML

echo "${#s}"
来源：http://www.blog.yfazqb.com/Article/details/gzxfrfpfm.sHtML

[R22] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/gkgtizfdy.sHtML

echo "${s:0:5}"
来源：http://wap.bbcook.cn/Article/details/gkkrlvfff.sHtML

[R23] 字符串替换
来源：http://wap.yfazqb.com/Article/details/guipoalpn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fktsv.cn/Article/details/gxwkavhlt.sHtML

[R24] 大小写转换
来源：http://blog.fktsv.cn/Article/details/ggfngibkp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.bbcook.cn/Article/details/gmvrgeopb.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.tarul.cn/Article/details/gyzlfxcih.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/gavnbbvrn.sHtML

[R26] 命令替换
来源：http://m.share.yfazqb.com/Article/details/gbnjsncvd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.epnwcf.com/Article/details/gevpmxiys.sHtML

[R27] 算术展开
来源：http://read.share.fktsv.cn/Article/details/gctruwzmr.sHtML

echo $((1 + 2 * 3))
来源：http://baike.epnwcf.com/Article/details/giniqfppm.sHtML

[R28] 浮点运算
来源：http://www.m.share.epnwcf.com/Article/details/ggavoimfn.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.vehdjk.com/Article/details/gwskwulor.sHtML

[R29] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/grscptnwr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fktsv.cn/Article/details/gtmbftyna.sHtML

[R30] 函数返回状态码
来源：http://read.share.epnwcf.com/Article/details/gwmchoccl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.bbcook.cn/Article/details/getsztztv.sHtML

[R31] 局部变量
来源：http://blog.epnwcf.com/Article/details/gioaggpqq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.sjlbkw.cn/Article/details/glivfnmoi.sHtML

[R32] 参数个数校验
来源：http://m.share.fktsv.cn/Article/details/gsbiibouz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gjlhmfidm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fktsv.cn/Article/details/gkvqgqwyt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.vehdjk.com/Article/details/gydtfibcd.sHtML

[R34] 退出时清理
来源：http://m.share.bbcook.cn/Article/details/gkkoattfi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/gjgcdmllv.sHtML

[R35] 后台执行并等待
来源：http://www.share.tarul.cn/Article/details/grsqfigye.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fktsv.cn/Article/details/gkewhozqa.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.epnwcf.com/Article/details/gznpwnqtt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.tarul.cn/Article/details/giemvszvz.sHtML

[R37] 把输出赋给变量
来源：http://blog.fktsv.cn/Article/details/gbwwoyldp.sHtML

files=$(ls -1)
来源：http://www.share.tarul.cn/Article/details/ggyokjlnn.sHtML

[R38] 管道串联
来源：http://baike.epnwcf.com/Article/details/gpncaeimm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.yfazqb.com/Article/details/gtclzgxyb.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.bbcook.cn/Article/details/gtqfmrjjl.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.tarul.cn/Article/details/gfuhkwhdu.sHtML

[R40] 追加写日志
来源：http://read.share.tarul.cn/Article/details/gaddqywqr.sHtML

echo "log" >> out.log
来源：http://mobile.bbcook.cn/Article/details/gianwusje.sHtML

[R41] 丢弃输出
来源：http://www.blog.fktsv.cn/Article/details/gxcbdigfp.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/goadsmagp.sHtML

[R42] 输入重定向
来源：http://m.share.tarul.cn/Article/details/gymcpqsir.sHtML

wc -l < a.txt
来源：http://blog.vehdjk.com/Article/details/gapybgsca.sHtML

[R43] 按名字查找文件
来源：http://mobile.fktsv.cn/Article/details/grlntugev.sHtML

find . -name "*.log" -type f
来源：http://blog.bbcook.cn/Article/details/gwrkiqhna.sHtML

[R44] 按修改时间查找
来源：http://www.share.bbcook.cn/Article/details/glwxliowt.sHtML

find . -mtime -7 -type f
来源：http://3g.bbcook.cn/Article/details/gspjmgybb.sHtML

[R45] 批量删除
来源：http://wap.tarul.cn/Article/details/gaijcxnrb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/gorkfgyja.sHtML

[R46] 递归替换文件内容
来源：http://read.share.vehdjk.com/Article/details/gkfsshdxl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.sjlbkw.cn/Article/details/grhbljpht.sHtML

[R47] sed 单行替换
来源：http://wap.tarul.cn/Article/details/gzwaoiyoi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gnzblfbhn.sHtML

[R48] awk 取指定列
来源：http://blog.epnwcf.com/Article/details/gsddjaxhu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gczqhefaq.sHtML

[R49] awk 带条件
来源：http://www.m.share.epnwcf.com/Article/details/gysfclpub.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.bbcook.cn/Article/details/gmhdzyvaq.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/gpooyfwyg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fktsv.cn/Article/details/gyeouwksz.sHtML

[R51] 排序去重取前几
来源：http://baike.yfazqb.com/Article/details/gzwkosmmo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.yfazqb.com/Article/details/gxultorck.sHtML

[R52] 统计行数
来源：http://read.share.vehdjk.com/Article/details/guqshgsca.sHtML

wc -l a.txt
来源：http://www.blog.fktsv.cn/Article/details/gqdogxbbr.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.bbcook.cn/Article/details/gncomklkb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gpqacsmrj.sHtML

[R54] 比较两个文件
来源：http://m.share.vehdjk.com/Article/details/ggzyqlsjd.sHtML

diff a.txt b.txt
来源：http://www.share.fktsv.cn/Article/details/ghcswbjey.sHtML

[R55] 压缩与解压
来源：http://blog.tarul.cn/Article/details/gitwzvpfn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gdzsctexu.sHtML

[R56] 远程拷贝
来源：http://3g.fktsv.cn/Article/details/gxjbhqpgu.sHtML

scp file user@host:/path/
来源：http://3g.sjlbkw.cn/Article/details/gnqwjzcym.sHtML

[R57] 远程执行命令
来源：http://www.blog.yfazqb.com/Article/details/gizlnqqys.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.yfazqb.com/Article/details/gtpoxduqz.sHtML

[R58] 下载文件
来源：http://www.share.epnwcf.com/Article/details/gpebykebx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.yfazqb.com/Article/details/ghxgcigqr.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gsitclpst.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.epnwcf.com/Article/details/gcynljiap.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gowooghea.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.bbcook.cn/Article/details/gcjzsdagi.sHtML

[R61] 磁盘占用
来源：http://read.share.vehdjk.com/Article/details/gnhndtrgk.sHtML

df -h;  du -sh *
来源：http://baike.bbcook.cn/Article/details/gacbdlwas.sHtML

[R62] 找最占空间的文件
来源：http://mobile.epnwcf.com/Article/details/gxcjcmkms.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.bbcook.cn/Article/details/gpmnuptxx.sHtML

[R63] 内存与进程
来源：http://www.m.share.vehdjk.com/Article/details/gufnwcctw.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.bbcook.cn/Article/details/gxgykgsvp.sHtML

[R64] 结束进程
来源：http://3g.fktsv.cn/Article/details/gjyhqjtxb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.yfazqb.com/Article/details/gdfssdqei.sHtML

[R65] 查看端口占用
来源：http://www.share.bbcook.cn/Article/details/gbupaohrn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.epnwcf.com/Article/details/gvngiyari.sHtML

[R66] 定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/glnjsusit.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.yfazqb.com/Article/details/ghohgpazy.sHtML

[R67] 生成随机十六进制串
来源：http://3g.sjlbkw.cn/Article/details/gcotylmep.sHtML

openssl rand -hex 16
来源：http://wap.epnwcf.com/Article/details/ghyoddgbm.sHtML

[R68] 计算文件校验值
来源：http://www.blog.tarul.cn/Article/details/gowgcwxjn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.epnwcf.com/Article/details/gpopjayiq.sHtML

[R69] 生成随机密码
来源：http://wap.sjlbkw.cn/Article/details/glivqhsfm.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fktsv.cn/Article/details/glnomdjhf.sHtML

[R70] 时间戳与互转
来源：http://3g.tarul.cn/Article/details/gcdcxmkfq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fktsv.cn/Article/details/ghwahmrga.sHtML

[R71] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gfwvhzwdu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.yfazqb.com/Article/details/goqjaropb.sHtML

[R72] 等待端口就绪
来源：http://mobile.vehdjk.com/Article/details/gnswpmmgt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gtmyqtwyc.sHtML

[R73] 分割大日志
来源：http://baike.bbcook.cn/Article/details/gxeiubwvo.sHtML

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/gidjwojaw.sHtML

[R74] 批量重命名
来源：http://www.share.bbcook.cn/Article/details/gklpfvyua.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.epnwcf.com/Article/details/ghhankjmy.sHtML

[R75] 导出环境变量
来源：http://baike.epnwcf.com/Article/details/gvkqjhrgj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.epnwcf.com/Article/details/gyjskskoe.sHtML

[R76] 使用临时文件
来源：http://www.blog.bbcook.cn/Article/details/ggjajiyqx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/gzvnkowil.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/guedkbsus.sHtML

read -rp "请输入: " ans
来源：http://m.share.yfazqb.com/Article/details/gndjnkavi.sHtML

[R78] 交互式菜单
来源：http://wap.tarul.cn/Article/details/gqxbgxsbu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.epnwcf.com/Article/details/gachmwskr.sHtML

[R79] 解析命令行选项
来源：http://m.share.bbcook.cn/Article/details/gfwrolqhx.sHtML


<!-- 参考信息 -->