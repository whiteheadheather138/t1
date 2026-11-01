代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://3g.epnwcf.com/Article/details/gjvuoeogy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.vehdjk.com/Article/details/gvosnwbds.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.bbcook.cn/Article/details/gcbefzojf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.sjlbkw.cn/Article/details/gocamiglq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/gmuamcomq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.sjlbkw.cn/Article/details/gnnocepra.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.tarul.cn/Article/details/goitbjotf.sHtML

[Q41] 多表连接
来源：http://www.blog.bbcook.cn/Article/details/gsfqvboml.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fktsv.cn/Article/details/gxgyioazt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.bbcook.cn/Article/details/ggvmzfaqz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fktsv.cn/Article/details/gswlasuea.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.vehdjk.com/Article/details/gymhvlzcr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.bbcook.cn/Article/details/gyladlysh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.tarul.cn/Article/details/gembvetqf.sHtML

[Q43] 标量子查询
来源：http://blog.epnwcf.com/Article/details/gvtwjwfcq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.vehdjk.com/Article/details/gclaxeycb.sHtML

[Q44] IN 子查询
来源：http://www.m.share.vehdjk.com/Article/details/gjvsapffh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.bbcook.cn/Article/details/givimwhvp.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.epnwcf.com/Article/details/gxhswqjiu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.sjlbkw.cn/Article/details/gmntglhug.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.yfazqb.com/Article/details/gilvcvzcg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.sjlbkw.cn/Article/details/giohclqqx.sHtML

[Q47] 与平均值比较
来源：http://blog.fktsv.cn/Article/details/gctyynpqt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.epnwcf.com/Article/details/gcoghqeae.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.tarul.cn/Article/details/goboamiab.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.sjlbkw.cn/Article/details/gmrizqxny.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.tarul.cn/Article/details/gnsmeuyge.sHtML

[Q49] 更新单行
来源：http://3g.sjlbkw.cn/Article/details/gfpxoubrs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gomcijvzo.sHtML

[Q50] 批量更新
来源：http://blog.fktsv.cn/Article/details/gzeyoumiy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.epnwcf.com/Article/details/gakcbqkkj.sHtML

[Q51] 用子查询更新
来源：http://mobile.sjlbkw.cn/Article/details/genrozeqe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.yfazqb.com/Article/details/gdgocgyqq.sHtML

[Q52] 删除指定行
来源：http://read.share.bbcook.cn/Article/details/gtlpciuot.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gzaftaksz.sHtML

[Q53] 按条件删除
来源：http://www.share.bbcook.cn/Article/details/gflrohvsh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.sjlbkw.cn/Article/details/gbzrxsiee.sHtML

[Q54] 清空表
来源：http://3g.sjlbkw.cn/Article/details/goizizcxb.sHtML

TRUNCATE TABLE logs;
来源：http://3g.vehdjk.com/Article/details/guoazulwa.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.vehdjk.com/Article/details/gxuvgbcpd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gkqnrvmgk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.epnwcf.com/Article/details/gwibajkkh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.sjlbkw.cn/Article/details/gcjlnuxzd.sHtML

[Q57] 行号
来源：http://baike.fktsv.cn/Article/details/gnrxdgwmg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.tarul.cn/Article/details/gfhugopoa.sHtML

[Q58] 累计求和
来源：http://mobile.fktsv.cn/Article/details/gmgjevlsd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gyxomxhey.sHtML

[Q59] 分组内累计
来源：http://www.share.bbcook.cn/Article/details/gilztgnct.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gburrhybm.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.bbcook.cn/Article/details/ghcrnbrpz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.sjlbkw.cn/Article/details/gijlphmxn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gcaagqhwn.sHtML

[Q61] 移动平均
来源：http://www.m.share.bbcook.cn/Article/details/gftxptoso.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gzhomlrlo.sHtML

[Q62] 分组占比
来源：http://blog.fktsv.cn/Article/details/gbsvlsote.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/grhtxtxxq.sHtML

[Q63] 开启事务
来源：http://blog.sjlbkw.cn/Article/details/gsebhtaey.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fktsv.cn/Article/details/gsguztpcg.sHtML

[Q64] 提交事务
来源：http://read.share.bbcook.cn/Article/details/gwikicyon.sHtML

COMMIT;
来源：http://www.m.share.vehdjk.com/Article/details/gxfbqamhh.sHtML

[Q65] 回滚事务
来源：http://m.share.vehdjk.com/Article/details/gksefllje.sHtML

ROLLBACK;
来源：http://blog.epnwcf.com/Article/details/ggkfdrkux.sHtML

[Q66] 行锁查询
来源：http://read.share.epnwcf.com/Article/details/ggoesjhjj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.epnwcf.com/Article/details/ghkheayce.sHtML

[Q67] 设置隔离级别
来源：http://3g.sjlbkw.cn/Article/details/gnqpmiqrl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.tarul.cn/Article/details/gugzqduyt.sHtML

[Q68] 保存点
来源：http://mobile.yfazqb.com/Article/details/gxgqhuvbp.sHtML

SAVEPOINT sp1;
来源：http://blog.yfazqb.com/Article/details/gxwkhjgei.sHtML

ROLLBACK TO sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gkxozoesj.sHtML

[Q69] 查看执行计划
来源：http://mobile.fktsv.cn/Article/details/gynqtkexn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.sjlbkw.cn/Article/details/geemdxrlb.sHtML

[Q70] 更新统计信息
来源：http://www.share.sjlbkw.cn/Article/details/gfguncvlj.sHtML

ANALYZE TABLE users;
来源：http://mobile.yfazqb.com/Article/details/gvblzqbmd.sHtML

[Q71] 查看建表语句
来源：http://read.share.epnwcf.com/Article/details/geexakkoe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.sjlbkw.cn/Article/details/gxasdouzb.sHtML

[Q72] 查看索引
来源：http://www.m.share.vehdjk.com/Article/details/gizjdcaxh.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gbeojmand.sHtML

[Q73] 查看表状态
来源：http://wap.bbcook.cn/Article/details/gxchcmndf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.bbcook.cn/Article/details/gsvypjarz.sHtML

[Q74] 强制使用索引
来源：http://www.share.bbcook.cn/Article/details/gxsjbrxxr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.tarul.cn/Article/details/gexhvuahb.sHtML

[Q75] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gnvyrzbvk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gmaulrznl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.epnwcf.com/Article/details/gktvkmuro.sHtML

[Q76] 按天统计
来源：http://wap.bbcook.cn/Article/details/gcchvuwdg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.vehdjk.com/Article/details/gurciqmxf.sHtML

[Q77] 时间加减
来源：http://www.m.share.tarul.cn/Article/details/gobqssppz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.sjlbkw.cn/Article/details/gkffjqumn.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/gkvqdyodc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.tarul.cn/Article/details/gcdmkmmhe.sHtML

[Q79] 字符串拼接
来源：http://wap.yfazqb.com/Article/details/gnwzdadpg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fktsv.cn/Article/details/gklcneqot.sHtML

[Q80] 字符串截取
来源：http://mobile.epnwcf.com/Article/details/gtbaywgyo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.epnwcf.com/Article/details/gqdmvkvsi.sHtML

[Q81] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gbrefibeh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.tarul.cn/Article/details/gluwzyphj.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.vehdjk.com/Article/details/gxeicoycd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gkhbvyynl.sHtML

[Q83] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gcaiggmak.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gxrmsdfcm.sHtML

[Q84] 去除首尾空格
来源：http://wap.vehdjk.com/Article/details/glbupbkmq.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gyiuhtncw.sHtML

[Q85] 数值取整
来源：http://www.blog.fktsv.cn/Article/details/gvzpeusva.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.epnwcf.com/Article/details/grsmxuruq.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.yfazqb.com/Article/details/ghpelvbgx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.bbcook.cn/Article/details/gbptrmzfr.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.yfazqb.com/Article/details/gthtszqnw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.sjlbkw.cn/Article/details/gnlqwvzwy.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fktsv.cn/Article/details/gstdqzpwl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.sjlbkw.cn/Article/details/gncaacmgd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.tarul.cn/Article/details/gwidnpvhb.sHtML

[Q89] 判断表是否存在
来源：http://baike.bbcook.cn/Article/details/ggjlvgquf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.vehdjk.com/Article/details/gjvamedwo.sHtML

[Q90] 生成序号列
来源：http://m.share.sjlbkw.cn/Article/details/gctaaxdnp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.vehdjk.com/Article/details/grfrrcjkg.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gvfwlheiy.sHtML

R. Bash 专题
来源：http://baike.epnwcf.com/Article/details/gxvapuctf.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwbgfsvlt.sHtML

[R01] shebang 与严格模式
来源：http://wap.epnwcf.com/Article/details/gjfhfkqea.sHtML

#!/usr/bin/env bash
来源：http://www.share.fktsv.cn/Article/details/gbtjgtkbw.sHtML

set -euo pipefail
来源：http://www.blog.epnwcf.com/Article/details/gfkoycpeh.sHtML

[R02] 变量赋值与使用
来源：http://www.share.yfazqb.com/Article/details/gtgjvzyvk.sHtML

name="Tom"; echo "$name"
来源：http://read.share.yfazqb.com/Article/details/ghjohihdr.sHtML

[R03] 只读变量
来源：http://read.share.tarul.cn/Article/details/ggbsyazko.sHtML

readonly PI=3.14
来源：http://3g.bbcook.cn/Article/details/gzbjbdare.sHtML

[R04] 位置参数
来源：http://www.share.epnwcf.com/Article/details/gjnwgpfbl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.sjlbkw.cn/Article/details/guacabejt.sHtML

[R05] 参数默认值
来源：http://www.blog.yfazqb.com/Article/details/gvegtjqnh.sHtML

name="${1:-default}"
来源：http://blog.bbcook.cn/Article/details/gkfrelphx.sHtML

[R06] 判断命令是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gfqothcdf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/gwqmymwct.sHtML

[R07] if 判断文件
来源：http://3g.yfazqb.com/Article/details/gqcnylnff.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.yfazqb.com/Article/details/gizcqmyzt.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/grudajisj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fktsv.cn/Article/details/gasmgjtkb.sHtML

[R09] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gwvorzwpe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.yfazqb.com/Article/details/gwfwmlndz.sHtML

[R10] 正则匹配
来源：http://www.m.share.yfazqb.com/Article/details/godisrdst.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.epnwcf.com/Article/details/gtpdnlzkl.sHtML

[R11] case 多分支
来源：http://read.share.bbcook.cn/Article/details/giftdrnqp.sHtML

case "$1" in
来源：http://m.share.yfazqb.com/Article/details/gelozrmev.sHtML

start) echo "启动" ;;
来源：http://wap.fktsv.cn/Article/details/gvdynezcq.sHtML

stop)  echo "停止" ;;
来源：http://www.share.yfazqb.com/Article/details/gslzpdamq.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.epnwcf.com/Article/details/gvcxejqps.sHtML

esac
来源：http://mobile.fktsv.cn/Article/details/gdreqiohe.sHtML

[R12] for 遍历文件
来源：http://mobile.epnwcf.com/Article/details/gdieapoyj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.epnwcf.com/Article/details/gsytdwkkq.sHtML

[R13] for 计数循环
来源：http://www.m.share.vehdjk.com/Article/details/gbxjwljzy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.bbcook.cn/Article/details/gteetwafo.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/gyraynofb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/guipjuudx.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gxjnfjpcu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.yfazqb.com/Article/details/gswuxefvn.sHtML

[R16] until 等待条件
来源：http://wap.fktsv.cn/Article/details/glvjjfags.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/giemaeowt.sHtML

[R17] 数组定义与取值
来源：http://www.share.vehdjk.com/Article/details/gdkfpvkcx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fktsv.cn/Article/details/gqopxgkmq.sHtML

[R18] 遍历数组
来源：http://mobile.vehdjk.com/Article/details/gsqmogkei.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.yfazqb.com/Article/details/gshicfaui.sHtML

[R19] 数组长度
来源：http://www.share.fktsv.cn/Article/details/gomjzzxxp.sHtML

echo "${#arr[@]}"
来源：http://3g.bbcook.cn/Article/details/gkrboerhs.sHtML

[R20] 关联数组（字典）
来源：http://read.share.yfazqb.com/Article/details/gmcdzffpn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.epnwcf.com/Article/details/gbgvmicef.sHtML

[R21] 字符串长度
来源：http://wap.bbcook.cn/Article/details/gzjsokrbd.sHtML

echo "${#s}"
来源：http://www.m.share.tarul.cn/Article/details/gdvycuchc.sHtML

[R22] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/gzbwvatir.sHtML

echo "${s:0:5}"
来源：http://www.m.share.epnwcf.com/Article/details/gpxnndvlw.sHtML

[R23] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gqmekiejj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.tarul.cn/Article/details/gtfdgvxmt.sHtML

[R24] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/giebuyhph.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.epnwcf.com/Article/details/gqxqcdhxi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.bbcook.cn/Article/details/gtezclvsf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.vehdjk.com/Article/details/gyvnpeond.sHtML

[R26] 命令替换
来源：http://www.m.share.yfazqb.com/Article/details/gifxhjiby.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.yfazqb.com/Article/details/gwfkaqege.sHtML

[R27] 算术展开
来源：http://mobile.bbcook.cn/Article/details/gucwwktnf.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.tarul.cn/Article/details/gslccxgkf.sHtML

[R28] 浮点运算
来源：http://3g.sjlbkw.cn/Article/details/gqceshqpm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fktsv.cn/Article/details/gdnhrzvox.sHtML

[R29] 定义函数
来源：http://blog.epnwcf.com/Article/details/gwonunpjh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.vehdjk.com/Article/details/gljrncruw.sHtML

[R30] 函数返回状态码
来源：http://blog.vehdjk.com/Article/details/gywricrib.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fktsv.cn/Article/details/gdaounemv.sHtML

[R31] 局部变量
来源：http://mobile.bbcook.cn/Article/details/gdvdxsomn.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.yfazqb.com/Article/details/ghtuhnuvw.sHtML

[R32] 参数个数校验
来源：http://blog.yfazqb.com/Article/details/gyezophrn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/gryrtilvr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.epnwcf.com/Article/details/gnkomfufz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.yfazqb.com/Article/details/gvjzufmgy.sHtML

[R34] 退出时清理
来源：http://read.share.vehdjk.com/Article/details/gafhgcimq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gemmbrbcu.sHtML

[R35] 后台执行并等待
来源：http://wap.sjlbkw.cn/Article/details/ggfnbbuhz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.bbcook.cn/Article/details/gxsxjfvsu.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/gwaqtmgkf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.tarul.cn/Article/details/gsnmoqnmq.sHtML

[R37] 把输出赋给变量
来源：http://read.share.bbcook.cn/Article/details/gsurhbykj.sHtML

files=$(ls -1)
来源：http://blog.sjlbkw.cn/Article/details/gtgyfcjvt.sHtML

[R38] 管道串联
来源：http://m.share.fktsv.cn/Article/details/gqvbmumln.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.vehdjk.com/Article/details/gtyglejcw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.bbcook.cn/Article/details/gcjbhgwaq.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gwbtivfoo.sHtML

[R40] 追加写日志
来源：http://www.blog.sjlbkw.cn/Article/details/guoskgtaf.sHtML

echo "log" >> out.log
来源：http://read.share.bbcook.cn/Article/details/gpgxookao.sHtML

[R41] 丢弃输出
来源：http://www.blog.vehdjk.com/Article/details/gdaungvih.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.vehdjk.com/Article/details/gcbizktfq.sHtML

[R42] 输入重定向
来源：http://www.m.share.bbcook.cn/Article/details/gbhwmoozr.sHtML

wc -l < a.txt
来源：http://m.share.epnwcf.com/Article/details/gmhxokpbg.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gwppvoamn.sHtML

find . -name "*.log" -type f
来源：http://baike.bbcook.cn/Article/details/gvxpkatmu.sHtML

[R44] 按修改时间查找
来源：http://blog.bbcook.cn/Article/details/gaxlvuhtb.sHtML

find . -mtime -7 -type f
来源：http://3g.fktsv.cn/Article/details/gsoqizycm.sHtML

[R45] 批量删除
来源：http://baike.bbcook.cn/Article/details/gzpijhuyo.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.epnwcf.com/Article/details/gdymuvfzp.sHtML

[R46] 递归替换文件内容
来源：http://blog.tarul.cn/Article/details/gvmdhhkqd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.epnwcf.com/Article/details/gapzalovg.sHtML

[R47] sed 单行替换
来源：http://m.share.fktsv.cn/Article/details/gajwqcell.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.yfazqb.com/Article/details/gzlfnyatr.sHtML

[R48] awk 取指定列
来源：http://mobile.tarul.cn/Article/details/gmcuequpf.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.vehdjk.com/Article/details/guwkrkbfb.sHtML

[R49] awk 带条件
来源：http://3g.yfazqb.com/Article/details/guthpwjbb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.epnwcf.com/Article/details/gbqylahin.sHtML

[R50] awk 求和
来源：http://3g.vehdjk.com/Article/details/gdttzusos.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.tarul.cn/Article/details/gtagpchrv.sHtML

[R51] 排序去重取前几
来源：http://www.blog.epnwcf.com/Article/details/gwocsqfdp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.yfazqb.com/Article/details/gbxxalivb.sHtML

[R52] 统计行数
来源：http://www.share.bbcook.cn/Article/details/ghpppixin.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/gpqasqssy.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.epnwcf.com/Article/details/gdfhwuypy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.sjlbkw.cn/Article/details/gaxnrsvdk.sHtML

[R54] 比较两个文件
来源：http://read.share.vehdjk.com/Article/details/gtxogzgnb.sHtML

diff a.txt b.txt
来源：http://blog.bbcook.cn/Article/details/guzfrbcub.sHtML

[R55] 压缩与解压
来源：http://www.m.share.yfazqb.com/Article/details/ggichqetj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.vehdjk.com/Article/details/gvcsxjdjd.sHtML

[R56] 远程拷贝
来源：http://read.share.vehdjk.com/Article/details/gdxovmtbf.sHtML

scp file user@host:/path/
来源：http://wap.yfazqb.com/Article/details/gcrevzzuu.sHtML

[R57] 远程执行命令
来源：http://www.share.sjlbkw.cn/Article/details/gmlyoffbg.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqszpnap.sHtML

[R58] 下载文件
来源：http://wap.yfazqb.com/Article/details/gquiknccn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.vehdjk.com/Article/details/gltvmafje.sHtML

[R59] 发 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gwwyvrlwi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.vehdjk.com/Article/details/ghyrspqtq.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/gkqojojzm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.sjlbkw.cn/Article/details/gyozvwdci.sHtML

[R61] 磁盘占用
来源：http://3g.sjlbkw.cn/Article/details/gxbxkutsd.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/gfjmuswka.sHtML

[R62] 找最占空间的文件
来源：http://wap.sjlbkw.cn/Article/details/gnjvqdcmg.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.tarul.cn/Article/details/gubiruusa.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gezepbrli.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.yfazqb.com/Article/details/gwrzzglks.sHtML

[R64] 结束进程
来源：http://wap.sjlbkw.cn/Article/details/gzmmvuday.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/gxquffgiz.sHtML

[R65] 查看端口占用
来源：http://wap.bbcook.cn/Article/details/ghbzsoxrc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.bbcook.cn/Article/details/ghnbcewbz.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/gjhdjgfxq.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/ggjcxveex.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.yfazqb.com/Article/details/gghsbjlng.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/gsawhygwn.sHtML

[R68] 计算文件校验值
来源：http://mobile.epnwcf.com/Article/details/golqoldzy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gptubsifn.sHtML

[R69] 生成随机密码
来源：http://www.blog.bbcook.cn/Article/details/gmopjdnzl.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.bbcook.cn/Article/details/ghuvsaada.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/gfxemfquk.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.vehdjk.com/Article/details/gesjnepxi.sHtML

[R71] 日期格式化
来源：http://blog.yfazqb.com/Article/details/glcnhkvsm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.epnwcf.com/Article/details/grpvorkth.sHtML

[R72] 等待端口就绪
来源：http://www.share.bbcook.cn/Article/details/ggsucfaqg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/gbhhayhbm.sHtML

[R73] 分割大日志
来源：http://www.blog.epnwcf.com/Article/details/gzfyxgzqc.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.epnwcf.com/Article/details/gshsgaaed.sHtML

[R74] 批量重命名
来源：http://baike.vehdjk.com/Article/details/gdiizkeup.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.yfazqb.com/Article/details/gbgclrjyq.sHtML

[R75] 导出环境变量
来源：http://blog.bbcook.cn/Article/details/gbcqypybt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.sjlbkw.cn/Article/details/gvyaaukuu.sHtML

[R76] 使用临时文件
来源：http://3g.vehdjk.com/Article/details/gptccwaav.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gvuetsnxs.sHtML

[R77] 读取用户输入
来源：http://wap.fktsv.cn/Article/details/gpvamgfzr.sHtML

read -rp "请输入: " ans
来源：http://baike.tarul.cn/Article/details/gnklftkjy.sHtML

[R78] 交互式菜单
来源：http://blog.fktsv.cn/Article/details/gkeqgloel.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.epnwcf.com/Article/details/gmpvuavvd.sHtML

[R79] 解析命令行选项
来源：http://m.share.epnwcf.com/Article/details/ghqpxepnb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.bbcook.cn/Article/details/gwtkdnztr.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.tarul.cn/Article/details/glmlvnbch.sHtML

time ./run.sh
来源：http://read.share.vehdjk.com/Article/details/gkskbreka.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/grbftoopv.sHtML

S. C / C++ 专题
来源：http://www.share.fktsv.cn/Article/details/gykliedym.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcfrlaayi.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/gtbipuuoj.sHtML

#include <stdio.h>
来源：http://wap.bbcook.cn/Article/details/gnwihhmzr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.vehdjk.com/Article/details/gfwzvhiii.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/gjanqcxhq.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.vehdjk.com/Article/details/gajpgrhye.sHtML

[S03] C：读入整数
来源：http://read.share.tarul.cn/Article/details/gownlpwwr.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggadhbhsv.sHtML

[S04] C：字符串复制
来源：http://baike.sjlbkw.cn/Article/details/gmpugojvg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.bbcook.cn/Article/details/gygqugmiu.sHtML

[S05] C：字符串长度
来源：http://3g.epnwcf.com/Article/details/gynxxnmdv.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/griauzxvy.sHtML

[S06] C：字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gdnwvegbf.sHtML

strcmp(a, b) == 0
来源：http://3g.epnwcf.com/Article/details/gwumxubqx.sHtML

[S07] C：数组遍历求和
来源：http://read.share.tarul.cn/Article/details/gvraewvjd.sHtML


<!-- 参考信息 -->