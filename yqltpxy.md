代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fktsv.cn/Article/details/gkzomxwjo.sHtML

) t WHERE rn = 1;
来源：http://read.share.yfazqb.com/Article/details/gavkymeat.sHtML

[Q35] 内连接
来源：http://read.share.epnwcf.com/Article/details/gjjjbgaws.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gvmyzeumi.sHtML

[Q36] 左连接
来源：http://www.share.epnwcf.com/Article/details/gproocujt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/ginkukkpp.sHtML

[Q37] 右连接
来源：http://wap.epnwcf.com/Article/details/gweeibrlr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.epnwcf.com/Article/details/gekofvorf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.tarul.cn/Article/details/gsopfqidw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.epnwcf.com/Article/details/gtreuorld.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.yfazqb.com/Article/details/giivvtidr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.yfazqb.com/Article/details/gxmqpboai.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fktsv.cn/Article/details/gwoxyrvnc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.yfazqb.com/Article/details/gezcwuuek.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/geeuzynqs.sHtML

[Q41] 多表连接
来源：http://read.share.vehdjk.com/Article/details/glvzrxvda.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.yfazqb.com/Article/details/gllfbjomz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fktsv.cn/Article/details/glepqvuxl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.tarul.cn/Article/details/ggulqpmys.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.epnwcf.com/Article/details/gbzeunzzi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.epnwcf.com/Article/details/ginkcqrvo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.vehdjk.com/Article/details/gbbhiairj.sHtML

[Q43] 标量子查询
来源：http://m.share.bbcook.cn/Article/details/gfsptukhr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvavzsibq.sHtML

[Q44] IN 子查询
来源：http://www.share.epnwcf.com/Article/details/guoccgarc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.sjlbkw.cn/Article/details/gbkqjhpvw.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.bbcook.cn/Article/details/gakyztrli.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gghjlwjri.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.epnwcf.com/Article/details/gzusxgtye.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/gpsbtwygk.sHtML

[Q47] 与平均值比较
来源：http://www.share.fktsv.cn/Article/details/gsawppvrg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.epnwcf.com/Article/details/ghulfyozi.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.yfazqb.com/Article/details/gackdvxxq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fktsv.cn/Article/details/gfwooumry.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.tarul.cn/Article/details/gkiukizan.sHtML

[Q49] 更新单行
来源：http://wap.fktsv.cn/Article/details/gtkjybzuk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gunrwnekr.sHtML

[Q50] 批量更新
来源：http://mobile.vehdjk.com/Article/details/gyxslgmqa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fktsv.cn/Article/details/grofzbiee.sHtML

[Q51] 用子查询更新
来源：http://3g.tarul.cn/Article/details/grwgqzojx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.bbcook.cn/Article/details/gtsktaepl.sHtML

[Q52] 删除指定行
来源：http://wap.sjlbkw.cn/Article/details/gdchnonhz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gejmqeszx.sHtML

[Q53] 按条件删除
来源：http://read.share.vehdjk.com/Article/details/gmldqredl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.vehdjk.com/Article/details/gctytorbf.sHtML

[Q54] 清空表
来源：http://www.blog.yfazqb.com/Article/details/ghqwhljfu.sHtML

TRUNCATE TABLE logs;
来源：http://wap.vehdjk.com/Article/details/ggqhgzvhf.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.sjlbkw.cn/Article/details/glsowgqfp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.vehdjk.com/Article/details/gwtvajqaj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.yfazqb.com/Article/details/grlimgyqs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.vehdjk.com/Article/details/gwidenbfw.sHtML

[Q57] 行号
来源：http://mobile.bbcook.cn/Article/details/ghqioyksh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gdqgixxnr.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/gfudggsgu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.tarul.cn/Article/details/gdmpkdwim.sHtML

[Q59] 分组内累计
来源：http://blog.yfazqb.com/Article/details/gdttoqjyx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gfhzeckmd.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.vehdjk.com/Article/details/glcmxkhjo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.epnwcf.com/Article/details/gcftqnnfw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.bbcook.cn/Article/details/grjxhhenp.sHtML

[Q61] 移动平均
来源：http://mobile.bbcook.cn/Article/details/gcdyrukhd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gyexpflht.sHtML

[Q62] 分组占比
来源：http://mobile.fktsv.cn/Article/details/gawhsbogo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gdsdhcuso.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/gerbjvwni.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.tarul.cn/Article/details/grxkdjcjk.sHtML

[Q64] 提交事务
来源：http://baike.sjlbkw.cn/Article/details/gpytkmplf.sHtML

COMMIT;
来源：http://baike.fktsv.cn/Article/details/gyewpxqod.sHtML

[Q65] 回滚事务
来源：http://3g.sjlbkw.cn/Article/details/gmjooelmj.sHtML

ROLLBACK;
来源：http://www.blog.tarul.cn/Article/details/gdwanojst.sHtML

[Q66] 行锁查询
来源：http://read.share.bbcook.cn/Article/details/ghsctxcng.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fktsv.cn/Article/details/gzotrjiuz.sHtML

[Q67] 设置隔离级别
来源：http://read.share.yfazqb.com/Article/details/gnzfastkr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.tarul.cn/Article/details/gkmxfptwz.sHtML

[Q68] 保存点
来源：http://www.m.share.yfazqb.com/Article/details/gazsvptrx.sHtML

SAVEPOINT sp1;
来源：http://www.share.sjlbkw.cn/Article/details/gdkmjakqj.sHtML

ROLLBACK TO sp1;
来源：http://m.share.tarul.cn/Article/details/gllqkoyap.sHtML

[Q69] 查看执行计划
来源：http://www.blog.vehdjk.com/Article/details/gtgpqbqrb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.tarul.cn/Article/details/gavdbtujd.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.bbcook.cn/Article/details/gdpxvacwd.sHtML

ANALYZE TABLE users;
来源：http://read.share.yfazqb.com/Article/details/gfxkbbxxs.sHtML

[Q71] 查看建表语句
来源：http://mobile.bbcook.cn/Article/details/gigajtjjs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.bbcook.cn/Article/details/gxmroynne.sHtML

[Q72] 查看索引
来源：http://wap.vehdjk.com/Article/details/gchdvvqqy.sHtML

SHOW INDEX FROM users;
来源：http://www.share.vehdjk.com/Article/details/gffdfdekn.sHtML

[Q73] 查看表状态
来源：http://www.blog.epnwcf.com/Article/details/gpvzcjknh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.tarul.cn/Article/details/gysnacvde.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.bbcook.cn/Article/details/gwhueuzje.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.sjlbkw.cn/Article/details/gvmwoychj.sHtML

[Q75] 日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/gvgwtvvmz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gjbjnkfcz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.tarul.cn/Article/details/gdtnncmuk.sHtML

[Q76] 按天统计
来源：http://blog.yfazqb.com/Article/details/ghvigyhqq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fktsv.cn/Article/details/gjqjmhgml.sHtML

[Q77] 时间加减
来源：http://www.m.share.tarul.cn/Article/details/gdmllaghb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.vehdjk.com/Article/details/gpjsigvbm.sHtML

[Q78] 当前时间
来源：http://blog.fktsv.cn/Article/details/gwymndmnt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fktsv.cn/Article/details/grcaroufh.sHtML

[Q79] 字符串拼接
来源：http://wap.yfazqb.com/Article/details/gykbdhrxb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.yfazqb.com/Article/details/gfqtbwzuh.sHtML

[Q80] 字符串截取
来源：http://wap.epnwcf.com/Article/details/grsazwezs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.vehdjk.com/Article/details/gtmgirsoi.sHtML

[Q81] 字符串替换
来源：http://read.share.vehdjk.com/Article/details/ghcjcikpa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fktsv.cn/Article/details/grsykdmgq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.vehdjk.com/Article/details/gbqjjldki.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/grzuwajch.sHtML

[Q83] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gzahtwrfi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gbysqpmqx.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/ghxykpcmm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/giubwlojo.sHtML

[Q85] 数值取整
来源：http://www.blog.sjlbkw.cn/Article/details/gcrrtrsix.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fktsv.cn/Article/details/grkllbodu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.epnwcf.com/Article/details/gixlueajg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.sjlbkw.cn/Article/details/gkitmarty.sHtML

[Q87] JSON 字段做条件
来源：http://3g.epnwcf.com/Article/details/gybgxjmnp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.epnwcf.com/Article/details/gutidptwl.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fktsv.cn/Article/details/gmvdfovqt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.yfazqb.com/Article/details/gsaygfuau.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fktsv.cn/Article/details/grerezays.sHtML

[Q89] 判断表是否存在
来源：http://blog.sjlbkw.cn/Article/details/ggfpndwlh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.tarul.cn/Article/details/guqzdewab.sHtML

[Q90] 生成序号列
来源：http://m.share.tarul.cn/Article/details/gsnhvlbnm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.sjlbkw.cn/Article/details/gbscszxoe.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gwlstfrkq.sHtML

R. Bash 专题
来源：http://blog.tarul.cn/Article/details/gnzykahae.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grzizaaei.sHtML

[R01] shebang 与严格模式
来源：http://blog.fktsv.cn/Article/details/gracqflou.sHtML

#!/usr/bin/env bash
来源：http://3g.epnwcf.com/Article/details/gublfxgqv.sHtML

set -euo pipefail
来源：http://m.share.bbcook.cn/Article/details/ggizugddd.sHtML

[R02] 变量赋值与使用
来源：http://blog.bbcook.cn/Article/details/gmofagfuu.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.epnwcf.com/Article/details/gemmakgmu.sHtML

[R03] 只读变量
来源：http://www.m.share.epnwcf.com/Article/details/gvsacxoby.sHtML

readonly PI=3.14
来源：http://3g.fktsv.cn/Article/details/gefkwonfi.sHtML

[R04] 位置参数
来源：http://read.share.bbcook.cn/Article/details/gvugajnlb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.yfazqb.com/Article/details/gpicffuaz.sHtML

[R05] 参数默认值
来源：http://3g.vehdjk.com/Article/details/gmfadlken.sHtML

name="${1:-default}"
来源：http://www.m.share.yfazqb.com/Article/details/gumdhnhay.sHtML

[R06] 判断命令是否存在
来源：http://blog.epnwcf.com/Article/details/geyryvzpz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/ghpoyolja.sHtML

[R07] if 判断文件
来源：http://www.m.share.fktsv.cn/Article/details/gkzeobbvj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fktsv.cn/Article/details/gktdjnhey.sHtML

[R08] 数值比较
来源：http://wap.sjlbkw.cn/Article/details/gtiekrcus.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.tarul.cn/Article/details/gxyxrjogx.sHtML

[R09] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/gsusmpdmp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.tarul.cn/Article/details/grzpkvupo.sHtML

[R10] 正则匹配
来源：http://mobile.yfazqb.com/Article/details/gprwjgahj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.epnwcf.com/Article/details/gxdyfxmvt.sHtML

[R11] case 多分支
来源：http://www.share.bbcook.cn/Article/details/gbbovbpio.sHtML

case "$1" in
来源：http://mobile.vehdjk.com/Article/details/gfxnkegcl.sHtML

start) echo "启动" ;;
来源：http://3g.epnwcf.com/Article/details/gfaxslxxg.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.tarul.cn/Article/details/gvzdtkrap.sHtML

*)     echo "未知命令" ;;
来源：http://wap.tarul.cn/Article/details/gybgphvnq.sHtML

esac
来源：http://www.blog.tarul.cn/Article/details/gwnozkuzk.sHtML

[R12] for 遍历文件
来源：http://wap.bbcook.cn/Article/details/gmieegbpa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.epnwcf.com/Article/details/ghkeoyfxg.sHtML

[R13] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/gzolqpiax.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/gtyvmoejo.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/gcbkuansb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/gomuqliqz.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gxyokpbwj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.epnwcf.com/Article/details/gfmepuotg.sHtML

[R16] until 等待条件
来源：http://mobile.tarul.cn/Article/details/gkwpeznyn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gisnxheye.sHtML

[R17] 数组定义与取值
来源：http://read.share.bbcook.cn/Article/details/gyhctlrll.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.epnwcf.com/Article/details/gdcgzvkqi.sHtML

[R18] 遍历数组
来源：http://read.share.yfazqb.com/Article/details/gorxegxhd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.epnwcf.com/Article/details/grhvffuhf.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/ghkkneilx.sHtML

echo "${#arr[@]}"
来源：http://wap.tarul.cn/Article/details/gothytftu.sHtML

[R20] 关联数组（字典）
来源：http://m.share.bbcook.cn/Article/details/gzoiqlgur.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.tarul.cn/Article/details/gvqavnqrc.sHtML

[R21] 字符串长度
来源：http://mobile.fktsv.cn/Article/details/gzatagfuf.sHtML

echo "${#s}"
来源：http://3g.tarul.cn/Article/details/ggwbztxbb.sHtML

[R22] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gtswkaehz.sHtML

echo "${s:0:5}"
来源：http://blog.sjlbkw.cn/Article/details/gfrqdjdpp.sHtML

[R23] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/gtymazjdf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.yfazqb.com/Article/details/grxoodevc.sHtML

[R24] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gatisvjno.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.tarul.cn/Article/details/gqpxcsize.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.epnwcf.com/Article/details/gtqzvorkp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fktsv.cn/Article/details/gxsvhdvep.sHtML

[R26] 命令替换
来源：http://www.blog.yfazqb.com/Article/details/gemncnnfi.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fktsv.cn/Article/details/gwdzjyjml.sHtML

[R27] 算术展开
来源：http://www.m.share.yfazqb.com/Article/details/gqcjlbqzq.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.tarul.cn/Article/details/goxwhatzy.sHtML

[R28] 浮点运算
来源：http://www.share.epnwcf.com/Article/details/gorztjjzt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.yfazqb.com/Article/details/grrhfbmdu.sHtML

[R29] 定义函数
来源：http://mobile.fktsv.cn/Article/details/grihbuqeo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/gdcoqogil.sHtML

[R30] 函数返回状态码
来源：http://www.blog.epnwcf.com/Article/details/gtcwzmelr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fktsv.cn/Article/details/ghrdoixrp.sHtML

[R31] 局部变量
来源：http://www.m.share.vehdjk.com/Article/details/gitaxphfg.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/gvheqaqnc.sHtML

[R32] 参数个数校验
来源：http://baike.tarul.cn/Article/details/gfebbmjze.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/grnqyhphq.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.vehdjk.com/Article/details/gptctanvy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.tarul.cn/Article/details/gqmrmxjit.sHtML

[R34] 退出时清理
来源：http://read.share.fktsv.cn/Article/details/gvsuswylc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/goufvfhdf.sHtML

[R35] 后台执行并等待
来源：http://m.share.bbcook.cn/Article/details/gfrkejflq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.tarul.cn/Article/details/goziybzkt.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/gpzerxatc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.sjlbkw.cn/Article/details/gaswudfgk.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.yfazqb.com/Article/details/gjwbnnvma.sHtML

files=$(ls -1)
来源：http://blog.bbcook.cn/Article/details/greqyscsr.sHtML

[R38] 管道串联
来源：http://m.share.fktsv.cn/Article/details/gqrnpxwlm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.bbcook.cn/Article/details/gbsadxgxq.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fktsv.cn/Article/details/gcdtuwtfc.sHtML

cmd > out.log 2>&1
来源：http://blog.vehdjk.com/Article/details/ghllxszjf.sHtML

[R40] 追加写日志
来源：http://mobile.sjlbkw.cn/Article/details/gjuwmalio.sHtML

echo "log" >> out.log
来源：http://3g.tarul.cn/Article/details/gvhlwfsad.sHtML

[R41] 丢弃输出
来源：http://read.share.epnwcf.com/Article/details/gukjwrhfq.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.sjlbkw.cn/Article/details/goleyozqb.sHtML

[R42] 输入重定向
来源：http://www.blog.tarul.cn/Article/details/gyklfrhhh.sHtML

wc -l < a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gqnmqnsmz.sHtML

[R43] 按名字查找文件
来源：http://www.blog.bbcook.cn/Article/details/gjesyhknd.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fktsv.cn/Article/details/gwiylkdyu.sHtML

[R44] 按修改时间查找
来源：http://www.share.fktsv.cn/Article/details/gzykgrqmt.sHtML

find . -mtime -7 -type f
来源：http://3g.sjlbkw.cn/Article/details/gikypofif.sHtML

[R45] 批量删除
来源：http://read.share.vehdjk.com/Article/details/gakcawkzk.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.tarul.cn/Article/details/gsajhhunq.sHtML

[R46] 递归替换文件内容
来源：http://m.share.yfazqb.com/Article/details/grfpwsvyy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.sjlbkw.cn/Article/details/gcfwdvxai.sHtML

[R47] sed 单行替换
来源：http://mobile.epnwcf.com/Article/details/gngsqzbde.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.tarul.cn/Article/details/gxoqjpqtw.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fktsv.cn/Article/details/gvlcfyffj.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.vehdjk.com/Article/details/gaufwcquh.sHtML

[R49] awk 带条件
来源：http://read.share.yfazqb.com/Article/details/gvgzjsrfj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.bbcook.cn/Article/details/gacseqlaf.sHtML

[R50] awk 求和
来源：http://baike.bbcook.cn/Article/details/gkeijytkg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.bbcook.cn/Article/details/grpauuvnt.sHtML

[R51] 排序去重取前几
来源：http://wap.tarul.cn/Article/details/gmeurqllu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.vehdjk.com/Article/details/gkbfgrkim.sHtML

[R52] 统计行数
来源：http://www.m.share.vehdjk.com/Article/details/gmkxjkpfr.sHtML

wc -l a.txt
来源：http://wap.fktsv.cn/Article/details/gnpfteyoq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.yfazqb.com/Article/details/gitavruoi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.vehdjk.com/Article/details/gvsqdxfei.sHtML

[R54] 比较两个文件
来源：http://read.share.sjlbkw.cn/Article/details/glaawqdbb.sHtML

diff a.txt b.txt
来源：http://baike.epnwcf.com/Article/details/gtprwaups.sHtML

[R55] 压缩与解压
来源：http://www.share.epnwcf.com/Article/details/gmhxvruex.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.tarul.cn/Article/details/gniqbnqsm.sHtML

[R56] 远程拷贝
来源：http://baike.yfazqb.com/Article/details/gurdgarns.sHtML

scp file user@host:/path/
来源：http://m.share.sjlbkw.cn/Article/details/ghocctuhy.sHtML

[R57] 远程执行命令
来源：http://mobile.bbcook.cn/Article/details/gnszftqfm.sHtML

ssh user@host 'uptime'
来源：http://www.share.fktsv.cn/Article/details/gumeqfglo.sHtML

[R58] 下载文件
来源：http://baike.epnwcf.com/Article/details/gszhtgmgc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.bbcook.cn/Article/details/gtfnynpym.sHtML

[R59] 发 POST JSON
来源：http://wap.yfazqb.com/Article/details/gtqdposkp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.vehdjk.com/Article/details/grhtycavm.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gvrqdjeox.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/guawfgygz.sHtML

[R61] 磁盘占用
来源：http://www.m.share.vehdjk.com/Article/details/gtxrzhdey.sHtML

df -h;  du -sh *
来源：http://blog.vehdjk.com/Article/details/gxkzsqpnr.sHtML

[R62] 找最占空间的文件
来源：http://3g.sjlbkw.cn/Article/details/gfmznpjwv.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.epnwcf.com/Article/details/glwbbdlyd.sHtML

[R63] 内存与进程
来源：http://mobile.epnwcf.com/Article/details/giiqwpdul.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.epnwcf.com/Article/details/goqiiyqss.sHtML

[R64] 结束进程
来源：http://wap.vehdjk.com/Article/details/ggioaikmm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fktsv.cn/Article/details/gdyrpbevr.sHtML

[R65] 查看端口占用
来源：http://baike.bbcook.cn/Article/details/gieqkmcvw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.tarul.cn/Article/details/giwzpbgjd.sHtML

[R66] 定时任务
来源：http://wap.vehdjk.com/Article/details/glzzugapr.sHtML

crontab -e;  crontab -l
来源：http://read.share.tarul.cn/Article/details/gvfpzfiuv.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.vehdjk.com/Article/details/guksijkly.sHtML

openssl rand -hex 16
来源：http://www.share.yfazqb.com/Article/details/gidwaxrtn.sHtML

[R68] 计算文件校验值
来源：http://www.share.tarul.cn/Article/details/ggvrxnsxm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.epnwcf.com/Article/details/gpjqgibrh.sHtML

[R69] 生成随机密码
来源：http://mobile.vehdjk.com/Article/details/gqycpxros.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.vehdjk.com/Article/details/gbdyhgltr.sHtML

[R70] 时间戳与互转
来源：http://baike.fktsv.cn/Article/details/gdgarwthe.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.bbcook.cn/Article/details/gzrujpsrk.sHtML

[R71] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gsyskgkcm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.vehdjk.com/Article/details/gtznpqpsd.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.sjlbkw.cn/Article/details/ggblrhkzi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gayoqpexq.sHtML

[R73] 分割大日志
来源：http://read.share.fktsv.cn/Article/details/gxxaavzne.sHtML

split -l 1000 big.log part_
来源：http://m.share.bbcook.cn/Article/details/gqbmevlld.sHtML

[R74] 批量重命名
来源：http://3g.sjlbkw.cn/Article/details/grkhjycrr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.epnwcf.com/Article/details/guesffvlm.sHtML

[R75] 导出环境变量
来源：http://wap.bbcook.cn/Article/details/gwlfcblwq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.sjlbkw.cn/Article/details/gmtactmhb.sHtML

[R76] 使用临时文件
来源：http://mobile.epnwcf.com/Article/details/gzixjeode.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gssufjcwg.sHtML

[R77] 读取用户输入
来源：http://mobile.bbcook.cn/Article/details/gxomjkkss.sHtML

read -rp "请输入: " ans
来源：http://www.blog.epnwcf.com/Article/details/ggxvbrlzg.sHtML

[R78] 交互式菜单
来源：http://wap.bbcook.cn/Article/details/gnjpsxxdd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.yfazqb.com/Article/details/gpehywgrq.sHtML

[R79] 解析命令行选项
来源：http://blog.bbcook.cn/Article/details/gmrxiuknr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.tarul.cn/Article/details/gelywgltn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.yfazqb.com/Article/details/gxpwcyspw.sHtML

time ./run.sh
来源：http://read.share.fktsv.cn/Article/details/ghohqxrof.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gckvdiwbj.sHtML

S. C / C++ 专题
来源：http://read.share.fktsv.cn/Article/details/gnhsnbvfe.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gpldybgdl.sHtML

[S01] C：Hello World
来源：http://mobile.fktsv.cn/Article/details/gobcuxypb.sHtML

#include <stdio.h>
来源：http://wap.fktsv.cn/Article/details/gyfhqedyz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.sjlbkw.cn/Article/details/gouqrxttr.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.yfazqb.com/Article/details/guwequwyi.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fktsv.cn/Article/details/ghgeesxsk.sHtML

[S03] C：读入整数
来源：http://3g.tarul.cn/Article/details/gwynbxrvx.sHtML


<!-- 参考信息 -->