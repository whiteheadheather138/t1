代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gwuefgvin.sHtML

[Q30] 分组统计
来源：http://www.m.share.tarul.cn/Article/details/gtrxtyxxo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/grqxjhbih.sHtML

[Q31] 分组后过滤
来源：http://www.share.vehdjk.com/Article/details/gkznaubiq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.tarul.cn/Article/details/gmxknqgtz.sHtML

[Q32] 分组拼接字符串
来源：http://blog.vehdjk.com/Article/details/glrtggrve.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gatomawzd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.tarul.cn/Article/details/gjjrauikq.sHtML

[Q33] 多列分组
来源：http://mobile.epnwcf.com/Article/details/guvvvcmor.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.sjlbkw.cn/Article/details/gtylkztdt.sHtML

[Q34] 每组取第一条
来源：http://m.share.yfazqb.com/Article/details/gugetmcdt.sHtML

SELECT * FROM (
来源：http://blog.epnwcf.com/Article/details/ggglilsig.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.bbcook.cn/Article/details/gvkjunwnj.sHtML

) t WHERE rn = 1;
来源：http://www.blog.bbcook.cn/Article/details/gkuvobkfn.sHtML

[Q35] 内连接
来源：http://mobile.yfazqb.com/Article/details/gvfyiqdrr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/gaeanjkpj.sHtML

[Q36] 左连接
来源：http://www.m.share.tarul.cn/Article/details/gjebvgifv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/gztrdnuih.sHtML

[Q37] 右连接
来源：http://www.blog.vehdjk.com/Article/details/gkljvpxae.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.tarul.cn/Article/details/gvdrjdvou.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.tarul.cn/Article/details/gqakdnseu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fktsv.cn/Article/details/gxwsirikk.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fktsv.cn/Article/details/gcixmtnjr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.bbcook.cn/Article/details/gukrkfctb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.epnwcf.com/Article/details/gtuvhafjz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.epnwcf.com/Article/details/guzvqrvkn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fktsv.cn/Article/details/gwnhccdzj.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/glsdxiwhk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.vehdjk.com/Article/details/gckwwuavk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.bbcook.cn/Article/details/gmsuwawou.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.vehdjk.com/Article/details/gbmicozrt.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fktsv.cn/Article/details/gqouebkir.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.sjlbkw.cn/Article/details/gpkwsiecp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.epnwcf.com/Article/details/gsvpvgzjv.sHtML

[Q43] 标量子查询
来源：http://www.blog.tarul.cn/Article/details/gamhmbqgh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.tarul.cn/Article/details/gbmztmcao.sHtML

[Q44] IN 子查询
来源：http://3g.sjlbkw.cn/Article/details/ghocxisek.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fktsv.cn/Article/details/gwawddwnv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.yfazqb.com/Article/details/gcafoyoum.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gruqleemt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.yfazqb.com/Article/details/gmpenvfaf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.sjlbkw.cn/Article/details/gorvggcgv.sHtML

[Q47] 与平均值比较
来源：http://blog.yfazqb.com/Article/details/gyhdgqjpd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.tarul.cn/Article/details/gpuidrxcx.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.sjlbkw.cn/Article/details/gnnjdtuxd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.sjlbkw.cn/Article/details/gfcynunkn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.bbcook.cn/Article/details/gtsutemyd.sHtML

[Q49] 更新单行
来源：http://www.m.share.yfazqb.com/Article/details/gaipqqspg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gsnvfufrk.sHtML

[Q50] 批量更新
来源：http://www.blog.fktsv.cn/Article/details/gcrrkyand.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.tarul.cn/Article/details/ggmdtsdxk.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.yfazqb.com/Article/details/gnfxlqhjy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.tarul.cn/Article/details/ggqwmqqha.sHtML

[Q52] 删除指定行
来源：http://m.share.vehdjk.com/Article/details/gjmrqayue.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.tarul.cn/Article/details/gpandoxlk.sHtML

[Q53] 按条件删除
来源：http://m.share.epnwcf.com/Article/details/gujcburyf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fktsv.cn/Article/details/gxatdrjfr.sHtML

[Q54] 清空表
来源：http://mobile.epnwcf.com/Article/details/giffwuddr.sHtML

TRUNCATE TABLE logs;
来源：http://3g.tarul.cn/Article/details/gkljnwzzh.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fktsv.cn/Article/details/gvhzbojet.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gayghicqz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.tarul.cn/Article/details/gadkallph.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.sjlbkw.cn/Article/details/gmvrygzpa.sHtML

[Q57] 行号
来源：http://read.share.tarul.cn/Article/details/gczsakhqb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.bbcook.cn/Article/details/gkeounufu.sHtML

[Q58] 累计求和
来源：http://www.share.fktsv.cn/Article/details/gepmyzjnw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gcuygvhto.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/giuewfnmb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gcdfcumiu.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fktsv.cn/Article/details/gkqygtlvu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fktsv.cn/Article/details/gnoxirhhv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gknlrqiyu.sHtML

[Q61] 移动平均
来源：http://blog.tarul.cn/Article/details/gpvsldhxv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/glvyeqoaz.sHtML

[Q62] 分组占比
来源：http://www.m.share.yfazqb.com/Article/details/grkpzbidw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gwdxhidos.sHtML

[Q63] 开启事务
来源：http://www.share.epnwcf.com/Article/details/gjefvapnx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.bbcook.cn/Article/details/gteedmzse.sHtML

[Q64] 提交事务
来源：http://blog.epnwcf.com/Article/details/gcbtlkffa.sHtML

COMMIT;
来源：http://www.blog.fktsv.cn/Article/details/gykknrznc.sHtML

[Q65] 回滚事务
来源：http://blog.yfazqb.com/Article/details/glkzyatie.sHtML

ROLLBACK;
来源：http://3g.tarul.cn/Article/details/gavpdetbs.sHtML

[Q66] 行锁查询
来源：http://www.share.fktsv.cn/Article/details/gwbuyudyf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.vehdjk.com/Article/details/gynynukad.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.sjlbkw.cn/Article/details/gviwuecdi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.tarul.cn/Article/details/gndddxege.sHtML

[Q68] 保存点
来源：http://3g.fktsv.cn/Article/details/giftdzplr.sHtML

SAVEPOINT sp1;
来源：http://www.share.epnwcf.com/Article/details/gunbmegyb.sHtML

ROLLBACK TO sp1;
来源：http://blog.bbcook.cn/Article/details/goqwtucyg.sHtML

[Q69] 查看执行计划
来源：http://www.share.fktsv.cn/Article/details/gtlykdybf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.epnwcf.com/Article/details/gwfimluir.sHtML

[Q70] 更新统计信息
来源：http://baike.epnwcf.com/Article/details/gcnwbncac.sHtML

ANALYZE TABLE users;
来源：http://www.blog.yfazqb.com/Article/details/gdcgxbbjx.sHtML

[Q71] 查看建表语句
来源：http://baike.tarul.cn/Article/details/gkrtdpedg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.yfazqb.com/Article/details/gmojhxqaz.sHtML

[Q72] 查看索引
来源：http://www.m.share.fktsv.cn/Article/details/gajskidem.sHtML

SHOW INDEX FROM users;
来源：http://www.share.epnwcf.com/Article/details/gokqopppa.sHtML

[Q73] 查看表状态
来源：http://www.share.sjlbkw.cn/Article/details/ggbebjfuf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.yfazqb.com/Article/details/gncixuepq.sHtML

[Q74] 强制使用索引
来源：http://www.share.bbcook.cn/Article/details/gzhupkhxk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.yfazqb.com/Article/details/guaatwkbp.sHtML

[Q75] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gpcxqrdus.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gdsvyifgx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/gztxczppg.sHtML

[Q76] 按天统计
来源：http://wap.vehdjk.com/Article/details/gptohjpvy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.yfazqb.com/Article/details/gyqxmvmvq.sHtML

[Q77] 时间加减
来源：http://www.m.share.bbcook.cn/Article/details/gocqncvuc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/gprvgsbwv.sHtML

[Q78] 当前时间
来源：http://baike.bbcook.cn/Article/details/gvprvqzxx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.tarul.cn/Article/details/gaqtywita.sHtML

[Q79] 字符串拼接
来源：http://baike.yfazqb.com/Article/details/gjqzmsggr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.tarul.cn/Article/details/gdrbwoiyb.sHtML

[Q80] 字符串截取
来源：http://read.share.bbcook.cn/Article/details/gzbejelgq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gogclrerj.sHtML

[Q81] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gqawcrewu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fktsv.cn/Article/details/gzrqlzoyy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.vehdjk.com/Article/details/gdbntdgib.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/ggovwldma.sHtML

[Q83] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gjybclyvz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gurmyqiri.sHtML

[Q84] 去除首尾空格
来源：http://wap.epnwcf.com/Article/details/gsdnbjlov.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gmwdwnlqh.sHtML

[Q85] 数值取整
来源：http://blog.bbcook.cn/Article/details/gxgcbnpfb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.vehdjk.com/Article/details/gjkpelzaj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fktsv.cn/Article/details/gucryqlvr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.yfazqb.com/Article/details/gcfozuprj.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.epnwcf.com/Article/details/gywgoteuo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.yfazqb.com/Article/details/gexdbklos.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.tarul.cn/Article/details/gmrwxgqlk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.bbcook.cn/Article/details/gphssrizr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.vehdjk.com/Article/details/grdacdlck.sHtML

[Q89] 判断表是否存在
来源：http://3g.sjlbkw.cn/Article/details/gjqdfhndt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fktsv.cn/Article/details/gtzpmcufy.sHtML

[Q90] 生成序号列
来源：http://www.blog.epnwcf.com/Article/details/gulgbdvyu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.vehdjk.com/Article/details/gvsjsckqx.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gvehtofue.sHtML

R. Bash 专题
来源：http://www.m.share.bbcook.cn/Article/details/gngyfvxwe.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gliotaerc.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.epnwcf.com/Article/details/gmxjzyswc.sHtML

#!/usr/bin/env bash
来源：http://blog.tarul.cn/Article/details/gtkykiynm.sHtML

set -euo pipefail
来源：http://baike.yfazqb.com/Article/details/gprbxffza.sHtML

[R02] 变量赋值与使用
来源：http://baike.yfazqb.com/Article/details/gjnvnespd.sHtML

name="Tom"; echo "$name"
来源：http://3g.sjlbkw.cn/Article/details/gjmxocuiz.sHtML

[R03] 只读变量
来源：http://read.share.yfazqb.com/Article/details/gfvbvpibu.sHtML

readonly PI=3.14
来源：http://www.blog.sjlbkw.cn/Article/details/gdhbzvluw.sHtML

[R04] 位置参数
来源：http://3g.sjlbkw.cn/Article/details/gkppnznib.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.yfazqb.com/Article/details/gsbjcpteb.sHtML

[R05] 参数默认值
来源：http://baike.tarul.cn/Article/details/ggzxqyimo.sHtML

name="${1:-default}"
来源：http://3g.fktsv.cn/Article/details/gwyasyqby.sHtML

[R06] 判断命令是否存在
来源：http://mobile.bbcook.cn/Article/details/ggeqozdju.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/grqhisycx.sHtML

[R07] if 判断文件
来源：http://m.share.fktsv.cn/Article/details/gfxfyxlyi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.tarul.cn/Article/details/gsnkxgkmo.sHtML

[R08] 数值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gexoaukmb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.epnwcf.com/Article/details/gppfdsjqh.sHtML

[R09] 字符串比较
来源：http://mobile.tarul.cn/Article/details/grxqucfre.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.bbcook.cn/Article/details/gkqwidwwq.sHtML

[R10] 正则匹配
来源：http://mobile.epnwcf.com/Article/details/gjcoqcijx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.tarul.cn/Article/details/gnncnwixt.sHtML

[R11] case 多分支
来源：http://mobile.epnwcf.com/Article/details/gnsqguwfb.sHtML

case "$1" in
来源：http://www.share.sjlbkw.cn/Article/details/gfgdugffe.sHtML

start) echo "启动" ;;
来源：http://www.blog.vehdjk.com/Article/details/glrcnpatw.sHtML

stop)  echo "停止" ;;
来源：http://mobile.vehdjk.com/Article/details/gfzmfdzit.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.epnwcf.com/Article/details/gknuhuzet.sHtML

esac
来源：http://blog.bbcook.cn/Article/details/gycjinbgc.sHtML

[R12] for 遍历文件
来源：http://mobile.epnwcf.com/Article/details/gjoquxhbj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.yfazqb.com/Article/details/gsemrjfco.sHtML

[R13] for 计数循环
来源：http://www.m.share.vehdjk.com/Article/details/guwgemidn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gnhejwmih.sHtML

[R14] C 风格 for
来源：http://blog.fktsv.cn/Article/details/guvxpucnv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/ghdorjhyg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gvskuvdbh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fktsv.cn/Article/details/grapgrxak.sHtML

[R16] until 等待条件
来源：http://wap.tarul.cn/Article/details/gwdtvodod.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/gatwmavvo.sHtML

[R17] 数组定义与取值
来源：http://3g.yfazqb.com/Article/details/gptbgbcno.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.tarul.cn/Article/details/gqymkafyt.sHtML

[R18] 遍历数组
来源：http://read.share.vehdjk.com/Article/details/grfoobadg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fktsv.cn/Article/details/grnbsssef.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gxjgibstn.sHtML

echo "${#arr[@]}"
来源：http://read.share.sjlbkw.cn/Article/details/gcqmehacl.sHtML

[R20] 关联数组（字典）
来源：http://baike.bbcook.cn/Article/details/ghctuzeel.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.bbcook.cn/Article/details/gqiuynedq.sHtML

[R21] 字符串长度
来源：http://www.blog.epnwcf.com/Article/details/grdqvooma.sHtML

echo "${#s}"
来源：http://baike.bbcook.cn/Article/details/gggyazygy.sHtML

[R22] 截取子串
来源：http://wap.yfazqb.com/Article/details/grqtwrmoe.sHtML

echo "${s:0:5}"
来源：http://wap.fktsv.cn/Article/details/gjmuafbac.sHtML

[R23] 字符串替换
来源：http://blog.tarul.cn/Article/details/gjocicbpm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.epnwcf.com/Article/details/gmpiashqq.sHtML

[R24] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gdutfyehe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.vehdjk.com/Article/details/gjeyepnht.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.sjlbkw.cn/Article/details/gwkadctfq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fktsv.cn/Article/details/ggzmlohdr.sHtML

[R26] 命令替换
来源：http://www.share.sjlbkw.cn/Article/details/govlfxica.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.sjlbkw.cn/Article/details/gqniduycd.sHtML

[R27] 算术展开
来源：http://www.blog.sjlbkw.cn/Article/details/gnvjeuyzz.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fktsv.cn/Article/details/gumkvjpfq.sHtML

[R28] 浮点运算
来源：http://read.share.bbcook.cn/Article/details/gjdqzpgty.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.yfazqb.com/Article/details/gndbqarbi.sHtML

[R29] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gdhfdtnnt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.tarul.cn/Article/details/gnsidiozl.sHtML

[R30] 函数返回状态码
来源：http://www.share.yfazqb.com/Article/details/gverpftdh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.vehdjk.com/Article/details/grnlsycgf.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/gckoamjsh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.tarul.cn/Article/details/ghzvvpkyi.sHtML

[R32] 参数个数校验
来源：http://www.m.share.yfazqb.com/Article/details/gpxjnlczy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/giumdtemc.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.yfazqb.com/Article/details/gjfvgonre.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrujslke.sHtML

[R34] 退出时清理
来源：http://mobile.vehdjk.com/Article/details/gtnekglbj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gkwutfzpm.sHtML

[R35] 后台执行并等待
来源：http://www.blog.vehdjk.com/Article/details/gayxbgjpe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.tarul.cn/Article/details/gwpkjwzkv.sHtML

[R36] 并发执行多个任务
来源：http://3g.sjlbkw.cn/Article/details/guqgcgdzi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.epnwcf.com/Article/details/ghwujgzin.sHtML

[R37] 把输出赋给变量
来源：http://www.share.tarul.cn/Article/details/gxwlhcper.sHtML

files=$(ls -1)
来源：http://mobile.bbcook.cn/Article/details/gighzbuaj.sHtML

[R38] 管道串联
来源：http://mobile.epnwcf.com/Article/details/gvjgnjvti.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.bbcook.cn/Article/details/glnglgwdr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.yfazqb.com/Article/details/gnmktcvxr.sHtML

cmd > out.log 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gvauqkxlc.sHtML

[R40] 追加写日志
来源：http://wap.tarul.cn/Article/details/gxhacdlbe.sHtML

echo "log" >> out.log
来源：http://blog.tarul.cn/Article/details/gqebhggbn.sHtML

[R41] 丢弃输出
来源：http://www.m.share.yfazqb.com/Article/details/gbgmacsvk.sHtML

cmd >/dev/null 2>&1
来源：http://3g.bbcook.cn/Article/details/gffssedew.sHtML

[R42] 输入重定向
来源：http://www.share.epnwcf.com/Article/details/gkgxunxrr.sHtML

wc -l < a.txt
来源：http://www.blog.yfazqb.com/Article/details/gqepequaf.sHtML

[R43] 按名字查找文件
来源：http://3g.tarul.cn/Article/details/gihzdqpor.sHtML

find . -name "*.log" -type f
来源：http://www.blog.yfazqb.com/Article/details/gpictapin.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.epnwcf.com/Article/details/gblzbzwlm.sHtML

find . -mtime -7 -type f
来源：http://baike.bbcook.cn/Article/details/gywhgplor.sHtML

[R45] 批量删除
来源：http://3g.sjlbkw.cn/Article/details/glpwaacvg.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.epnwcf.com/Article/details/gemauqatz.sHtML

[R46] 递归替换文件内容
来源：http://blog.tarul.cn/Article/details/guiskuhzu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.bbcook.cn/Article/details/gppoyuzze.sHtML

[R47] sed 单行替换
来源：http://www.m.share.tarul.cn/Article/details/gqbrijdps.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.epnwcf.com/Article/details/gsscxayen.sHtML

[R48] awk 取指定列
来源：http://3g.vehdjk.com/Article/details/grzvxiumo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gytcdllvm.sHtML

[R49] awk 带条件
来源：http://m.share.sjlbkw.cn/Article/details/gnjwuvesy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.epnwcf.com/Article/details/giyqolvmz.sHtML

[R50] awk 求和
来源：http://mobile.bbcook.cn/Article/details/gipgzkghp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.bbcook.cn/Article/details/glqmssxml.sHtML

[R51] 排序去重取前几
来源：http://wap.bbcook.cn/Article/details/gtuyqzcyq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fktsv.cn/Article/details/gwzkobjcb.sHtML

[R52] 统计行数
来源：http://blog.tarul.cn/Article/details/gazbeezef.sHtML

wc -l a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gnlhywahd.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.vehdjk.com/Article/details/gxywwavmx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.yfazqb.com/Article/details/gxuzfshdw.sHtML

[R54] 比较两个文件
来源：http://m.share.fktsv.cn/Article/details/gqvprdila.sHtML

diff a.txt b.txt
来源：http://mobile.vehdjk.com/Article/details/gblneyzdk.sHtML

[R55] 压缩与解压
来源：http://www.share.epnwcf.com/Article/details/gptnbcbii.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.yfazqb.com/Article/details/gqseqgbks.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/gzyqiafco.sHtML

scp file user@host:/path/
来源：http://www.blog.epnwcf.com/Article/details/gvjnifbln.sHtML

[R57] 远程执行命令
来源：http://baike.vehdjk.com/Article/details/gxphedjna.sHtML

ssh user@host 'uptime'
来源：http://3g.vehdjk.com/Article/details/gwgacsnlk.sHtML

[R58] 下载文件
来源：http://www.share.sjlbkw.cn/Article/details/gyzibzzlx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.yfazqb.com/Article/details/gvoajxbna.sHtML

[R59] 发 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/gztdmzlea.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.vehdjk.com/Article/details/gkaocbdhv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/gjhbjiwlv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.vehdjk.com/Article/details/gbwkrtjhi.sHtML

[R61] 磁盘占用
来源：http://mobile.yfazqb.com/Article/details/grgowqtse.sHtML

df -h;  du -sh *
来源：http://wap.sjlbkw.cn/Article/details/gvtqhwcla.sHtML

[R62] 找最占空间的文件
来源：http://mobile.bbcook.cn/Article/details/gbuggkdyq.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.sjlbkw.cn/Article/details/givukuykd.sHtML

[R63] 内存与进程
来源：http://read.share.yfazqb.com/Article/details/glquqxgoy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.epnwcf.com/Article/details/gvzfcrijj.sHtML

[R64] 结束进程
来源：http://read.share.vehdjk.com/Article/details/gckjpovvn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.yfazqb.com/Article/details/gmvnqetrk.sHtML

[R65] 查看端口占用
来源：http://m.share.epnwcf.com/Article/details/gnnujuyhr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.yfazqb.com/Article/details/gvwxirpue.sHtML

[R66] 定时任务
来源：http://m.share.epnwcf.com/Article/details/ghqhxmesy.sHtML

crontab -e;  crontab -l
来源：http://blog.yfazqb.com/Article/details/gohxhbxvq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.vehdjk.com/Article/details/gvlptivzs.sHtML

openssl rand -hex 16
来源：http://read.share.sjlbkw.cn/Article/details/gmthuohzb.sHtML

[R68] 计算文件校验值
来源：http://www.blog.epnwcf.com/Article/details/gofpzquar.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdaezdip.sHtML

[R69] 生成随机密码
来源：http://blog.fktsv.cn/Article/details/grlezgcfz.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.yfazqb.com/Article/details/gyirhcekk.sHtML

[R70] 时间戳与互转
来源：http://m.share.yfazqb.com/Article/details/gsorbcqpe.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/gliziuuww.sHtML

[R71] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/gzheqatwc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.tarul.cn/Article/details/gkwlhonco.sHtML

[R72] 等待端口就绪
来源：http://www.blog.bbcook.cn/Article/details/glewmnjtj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gddexmfsk.sHtML

[R73] 分割大日志
来源：http://www.share.epnwcf.com/Article/details/gsmtzfohd.sHtML

split -l 1000 big.log part_
来源：http://m.share.sjlbkw.cn/Article/details/gwiotbdnd.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/gesqxjluf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.epnwcf.com/Article/details/gpjantjze.sHtML

[R75] 导出环境变量
来源：http://read.share.bbcook.cn/Article/details/gtoycmnpk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.tarul.cn/Article/details/gbjgvqgnj.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/gvxmozxuy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/gyipevxtc.sHtML

[R77] 读取用户输入
来源：http://www.blog.bbcook.cn/Article/details/gptylrgtx.sHtML

read -rp "请输入: " ans
来源：http://baike.yfazqb.com/Article/details/gtweydaku.sHtML

[R78] 交互式菜单
来源：http://mobile.tarul.cn/Article/details/gyzullcdj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.sjlbkw.cn/Article/details/gjeetdqzu.sHtML

[R79] 解析命令行选项
来源：http://mobile.sjlbkw.cn/Article/details/glgpeiwqu.sHtML


<!-- 参考信息 -->