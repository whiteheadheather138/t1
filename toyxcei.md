代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.tarul.cn/Article/details/gbrfkzrpy.sHtML

) t WHERE rn = 1;
来源：http://3g.sjlbkw.cn/Article/details/glsuoylwl.sHtML

[Q35] 内连接
来源：http://www.blog.epnwcf.com/Article/details/gzwpewfzn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/guurcywva.sHtML

[Q36] 左连接
来源：http://wap.sjlbkw.cn/Article/details/genjbuiid.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.tarul.cn/Article/details/gtwsljsyn.sHtML

[Q37] 右连接
来源：http://www.blog.bbcook.cn/Article/details/gkrckwvrx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.tarul.cn/Article/details/ggbguijnf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.epnwcf.com/Article/details/gvpifzqly.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.yfazqb.com/Article/details/gxeeyntti.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.epnwcf.com/Article/details/guxjixcxi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fktsv.cn/Article/details/gcwebuiod.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.epnwcf.com/Article/details/gkvgawhyo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.tarul.cn/Article/details/gexueqpok.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/gchnjbfrl.sHtML

[Q41] 多表连接
来源：http://www.m.share.vehdjk.com/Article/details/gdibjnlyl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.sjlbkw.cn/Article/details/gzfftretu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.sjlbkw.cn/Article/details/gejxvniox.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.bbcook.cn/Article/details/gansuwgsy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.vehdjk.com/Article/details/gsqlfimbs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.epnwcf.com/Article/details/guqsnussq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.yfazqb.com/Article/details/glhqwaenu.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/gfxbkbyfk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.sjlbkw.cn/Article/details/gdvwpctko.sHtML

[Q44] IN 子查询
来源：http://www.blog.bbcook.cn/Article/details/gjtnrkndo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.yfazqb.com/Article/details/glomkerbm.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.yfazqb.com/Article/details/gzouplhsi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gprromdio.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.epnwcf.com/Article/details/gpuulcxiw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/gmafmrsav.sHtML

[Q47] 与平均值比较
来源：http://www.share.tarul.cn/Article/details/gvfiezwky.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.sjlbkw.cn/Article/details/gxodrhpeg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.vehdjk.com/Article/details/gyibtshef.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.tarul.cn/Article/details/gfgqfmwcr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfqwpohd.sHtML

[Q49] 更新单行
来源：http://wap.vehdjk.com/Article/details/gctjmtojy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gjxcdxtdr.sHtML

[Q50] 批量更新
来源：http://wap.epnwcf.com/Article/details/gkqxsenet.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.yfazqb.com/Article/details/ghfusyuir.sHtML

[Q51] 用子查询更新
来源：http://read.share.fktsv.cn/Article/details/gmbasparf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gmqbkuvbx.sHtML

[Q52] 删除指定行
来源：http://m.share.bbcook.cn/Article/details/grniidxvq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gzhquixtz.sHtML

[Q53] 按条件删除
来源：http://blog.yfazqb.com/Article/details/gwbouiupi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.bbcook.cn/Article/details/gozzvuplm.sHtML

[Q54] 清空表
来源：http://mobile.fktsv.cn/Article/details/grozvvzdp.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fktsv.cn/Article/details/gmqmnnnjk.sHtML

[Q55] 排名（并列占位）
来源：http://blog.bbcook.cn/Article/details/gdduujyfd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.sjlbkw.cn/Article/details/gtbwyckmz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.epnwcf.com/Article/details/ggcsnhcfj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.yfazqb.com/Article/details/gmlkxexiz.sHtML

[Q57] 行号
来源：http://baike.sjlbkw.cn/Article/details/gfonbjcyc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.bbcook.cn/Article/details/ghzogwlmt.sHtML

[Q58] 累计求和
来源：http://wap.epnwcf.com/Article/details/gzxpisvec.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gibnstbup.sHtML

[Q59] 分组内累计
来源：http://mobile.tarul.cn/Article/details/gciowlaus.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/galdgzvuh.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.bbcook.cn/Article/details/gzwdvrsjz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.sjlbkw.cn/Article/details/gnyctiamm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwvgotye.sHtML

[Q61] 移动平均
来源：http://3g.yfazqb.com/Article/details/gvigjcimy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gvbavldly.sHtML

[Q62] 分组占比
来源：http://www.m.share.yfazqb.com/Article/details/gignwthhi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gqnmgfxkq.sHtML

[Q63] 开启事务
来源：http://www.share.sjlbkw.cn/Article/details/gnzxlgupx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.bbcook.cn/Article/details/gaihrlwew.sHtML

[Q64] 提交事务
来源：http://mobile.bbcook.cn/Article/details/gscfaovbg.sHtML

COMMIT;
来源：http://www.blog.tarul.cn/Article/details/grwbwfhbc.sHtML

[Q65] 回滚事务
来源：http://blog.tarul.cn/Article/details/gkoyidzaz.sHtML

ROLLBACK;
来源：http://mobile.yfazqb.com/Article/details/galcvrcih.sHtML

[Q66] 行锁查询
来源：http://blog.fktsv.cn/Article/details/gacwjvaim.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.tarul.cn/Article/details/gmiqwlreh.sHtML

[Q67] 设置隔离级别
来源：http://3g.yfazqb.com/Article/details/gbljleyba.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.vehdjk.com/Article/details/gosajzdbr.sHtML

[Q68] 保存点
来源：http://www.blog.vehdjk.com/Article/details/glpqgghxe.sHtML

SAVEPOINT sp1;
来源：http://3g.bbcook.cn/Article/details/gqitpylbr.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.tarul.cn/Article/details/gnnbiyeei.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.vehdjk.com/Article/details/gyqtlapfb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.tarul.cn/Article/details/gxjtffeta.sHtML

[Q70] 更新统计信息
来源：http://3g.sjlbkw.cn/Article/details/gvoehvnjb.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.epnwcf.com/Article/details/gdwhzhxbv.sHtML

[Q71] 查看建表语句
来源：http://baike.sjlbkw.cn/Article/details/glqbftnos.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.epnwcf.com/Article/details/gxupvljgm.sHtML

[Q72] 查看索引
来源：http://wap.bbcook.cn/Article/details/ghbrolrij.sHtML

SHOW INDEX FROM users;
来源：http://mobile.bbcook.cn/Article/details/ggfjlvpkv.sHtML

[Q73] 查看表状态
来源：http://mobile.bbcook.cn/Article/details/gefucnbci.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.sjlbkw.cn/Article/details/ggyilehts.sHtML

[Q74] 强制使用索引
来源：http://read.share.yfazqb.com/Article/details/gtcabwrbc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fktsv.cn/Article/details/gwedxmesa.sHtML

[Q75] 日期格式化
来源：http://www.blog.vehdjk.com/Article/details/gltshbqul.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gaaxjirww.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.sjlbkw.cn/Article/details/gnlpncsfd.sHtML

[Q76] 按天统计
来源：http://3g.vehdjk.com/Article/details/gqiqpvfrd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.yfazqb.com/Article/details/gvwhsywdi.sHtML

[Q77] 时间加减
来源：http://m.share.epnwcf.com/Article/details/grmkdchxg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.yfazqb.com/Article/details/gbhaocbpa.sHtML

[Q78] 当前时间
来源：http://mobile.tarul.cn/Article/details/gygebgtlc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.tarul.cn/Article/details/goltwsnjt.sHtML

[Q79] 字符串拼接
来源：http://m.share.sjlbkw.cn/Article/details/gutpagkuj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.vehdjk.com/Article/details/gjzkccjjs.sHtML

[Q80] 字符串截取
来源：http://mobile.yfazqb.com/Article/details/gahynyjmj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gpyqotksg.sHtML

[Q81] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/giamcmqxd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.epnwcf.com/Article/details/gtnzycrmg.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.bbcook.cn/Article/details/glqedhjbr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gdwjrqjys.sHtML

[Q83] 大小写转换
来源：http://3g.sjlbkw.cn/Article/details/gsnkalvnt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gknfawdgr.sHtML

[Q84] 去除首尾空格
来源：http://wap.sjlbkw.cn/Article/details/gltyzazzy.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gutwkqowq.sHtML

[Q85] 数值取整
来源：http://wap.tarul.cn/Article/details/gmcvtihgg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.tarul.cn/Article/details/gtkdfraga.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.tarul.cn/Article/details/geiboghnp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.epnwcf.com/Article/details/gjxtalsuz.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.tarul.cn/Article/details/gnyrbjsna.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.epnwcf.com/Article/details/gqoigcvda.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.sjlbkw.cn/Article/details/gfgtfapcp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.vehdjk.com/Article/details/gcngimhmy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fktsv.cn/Article/details/gqhfcgsaj.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gqujihwvp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.epnwcf.com/Article/details/gjcvgxkim.sHtML

[Q90] 生成序号列
来源：http://m.share.fktsv.cn/Article/details/gswfkfanq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.sjlbkw.cn/Article/details/gbmgujigb.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gyyebcmze.sHtML

R. Bash 专题
来源：http://read.share.yfazqb.com/Article/details/gaxqfelyj.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gldtngqfj.sHtML

[R01] shebang 与严格模式
来源：http://baike.tarul.cn/Article/details/gkfsmepgo.sHtML

#!/usr/bin/env bash
来源：http://blog.fktsv.cn/Article/details/gkrfnahml.sHtML

set -euo pipefail
来源：http://baike.yfazqb.com/Article/details/gofbgcoas.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/grzfrmfsi.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fktsv.cn/Article/details/gxnzdexnc.sHtML

[R03] 只读变量
来源：http://www.share.epnwcf.com/Article/details/gzicgmrff.sHtML

readonly PI=3.14
来源：http://blog.vehdjk.com/Article/details/gnzoihkcg.sHtML

[R04] 位置参数
来源：http://read.share.yfazqb.com/Article/details/gvbavzmay.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.vehdjk.com/Article/details/gwtsapqoo.sHtML

[R05] 参数默认值
来源：http://read.share.fktsv.cn/Article/details/gvylwhzgo.sHtML

name="${1:-default}"
来源：http://mobile.yfazqb.com/Article/details/geykuprvk.sHtML

[R06] 判断命令是否存在
来源：http://blog.fktsv.cn/Article/details/gvcloidxy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/galmimerw.sHtML

[R07] if 判断文件
来源：http://baike.yfazqb.com/Article/details/giqqbdaim.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.tarul.cn/Article/details/gvudumkqi.sHtML

[R08] 数值比较
来源：http://mobile.bbcook.cn/Article/details/gqxzzogpw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.bbcook.cn/Article/details/gzygksigk.sHtML

[R09] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/glppphbdc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fktsv.cn/Article/details/gpgfokvri.sHtML

[R10] 正则匹配
来源：http://3g.fktsv.cn/Article/details/gqokjigtd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.yfazqb.com/Article/details/galpstpux.sHtML

[R11] case 多分支
来源：http://baike.tarul.cn/Article/details/gofbfndpk.sHtML

case "$1" in
来源：http://wap.fktsv.cn/Article/details/gtyigfmsz.sHtML

start) echo "启动" ;;
来源：http://3g.yfazqb.com/Article/details/ghfyaaetv.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.epnwcf.com/Article/details/giybzzgtx.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.epnwcf.com/Article/details/gaxypytyt.sHtML

esac
来源：http://www.share.epnwcf.com/Article/details/gvynlzklw.sHtML

[R12] for 遍历文件
来源：http://mobile.tarul.cn/Article/details/gjwpjrezy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.bbcook.cn/Article/details/gnspzoope.sHtML

[R13] for 计数循环
来源：http://read.share.yfazqb.com/Article/details/ghhudwoqt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.sjlbkw.cn/Article/details/gaakhtbdl.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/gedugggci.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/gvxdxeyms.sHtML

[R15] while 逐行读文件
来源：http://www.share.vehdjk.com/Article/details/glmfqjyhp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gkopbgvez.sHtML

[R16] until 等待条件
来源：http://blog.tarul.cn/Article/details/grtyqzums.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gtrflywsn.sHtML

[R17] 数组定义与取值
来源：http://www.blog.vehdjk.com/Article/details/giztcxldd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fktsv.cn/Article/details/gbxcxpiph.sHtML

[R18] 遍历数组
来源：http://www.m.share.fktsv.cn/Article/details/gpvuyfdia.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.bbcook.cn/Article/details/gmhagbpjp.sHtML

[R19] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gqiaklwqd.sHtML

echo "${#arr[@]}"
来源：http://www.share.epnwcf.com/Article/details/grpxxzzay.sHtML

[R20] 关联数组（字典）
来源：http://mobile.bbcook.cn/Article/details/gqtgusqyw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.vehdjk.com/Article/details/gwfxxtvcc.sHtML

[R21] 字符串长度
来源：http://mobile.vehdjk.com/Article/details/gdlwqhdwj.sHtML

echo "${#s}"
来源：http://blog.epnwcf.com/Article/details/ggucskzhs.sHtML

[R22] 截取子串
来源：http://read.share.tarul.cn/Article/details/gzslcgqia.sHtML

echo "${s:0:5}"
来源：http://www.share.yfazqb.com/Article/details/gqjksbfha.sHtML

[R23] 字符串替换
来源：http://baike.fktsv.cn/Article/details/gkcjrjunv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.bbcook.cn/Article/details/gxvaxifho.sHtML

[R24] 大小写转换
来源：http://baike.yfazqb.com/Article/details/gxxdniizt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fktsv.cn/Article/details/gqljacown.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.yfazqb.com/Article/details/gaybvhfjs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.bbcook.cn/Article/details/gbbpvjlax.sHtML

[R26] 命令替换
来源：http://mobile.yfazqb.com/Article/details/gmzqimklb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.sjlbkw.cn/Article/details/gdjttbmsl.sHtML

[R27] 算术展开
来源：http://wap.tarul.cn/Article/details/gybblytol.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.bbcook.cn/Article/details/glqosherk.sHtML

[R28] 浮点运算
来源：http://www.blog.epnwcf.com/Article/details/gcdpxeopf.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fktsv.cn/Article/details/gvsgdindy.sHtML

[R29] 定义函数
来源：http://blog.vehdjk.com/Article/details/gwilfkogy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.yfazqb.com/Article/details/gqwlwsmcp.sHtML

[R30] 函数返回状态码
来源：http://mobile.tarul.cn/Article/details/gxykctyfs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.tarul.cn/Article/details/gqdgpaqwi.sHtML

[R31] 局部变量
来源：http://3g.fktsv.cn/Article/details/gzcsfmuql.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.bbcook.cn/Article/details/gyiqhwmmw.sHtML

[R32] 参数个数校验
来源：http://wap.epnwcf.com/Article/details/gzsabfcmp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/gonrnlddu.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.tarul.cn/Article/details/gxdkehdzg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.yfazqb.com/Article/details/gqdtnavel.sHtML

[R34] 退出时清理
来源：http://blog.tarul.cn/Article/details/guzfahlhj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/grrtzhjag.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.epnwcf.com/Article/details/goqgthgwk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fktsv.cn/Article/details/gvaxqkkez.sHtML

[R36] 并发执行多个任务
来源：http://baike.epnwcf.com/Article/details/gvbpnaenj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.tarul.cn/Article/details/ginznjtsu.sHtML

[R37] 把输出赋给变量
来源：http://www.share.yfazqb.com/Article/details/gsscbhtyy.sHtML

files=$(ls -1)
来源：http://read.share.yfazqb.com/Article/details/gtwbnvihw.sHtML

[R38] 管道串联
来源：http://m.share.sjlbkw.cn/Article/details/gkynzqilo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.tarul.cn/Article/details/goecrjtfu.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.tarul.cn/Article/details/gcjckzdza.sHtML

cmd > out.log 2>&1
来源：http://wap.bbcook.cn/Article/details/ghpdwoxdf.sHtML

[R40] 追加写日志
来源：http://3g.fktsv.cn/Article/details/gwloikplo.sHtML

echo "log" >> out.log
来源：http://mobile.bbcook.cn/Article/details/gqhbgnhgb.sHtML

[R41] 丢弃输出
来源：http://mobile.sjlbkw.cn/Article/details/gxrquftoj.sHtML

cmd >/dev/null 2>&1
来源：http://wap.tarul.cn/Article/details/ggkczccmu.sHtML

[R42] 输入重定向
来源：http://3g.sjlbkw.cn/Article/details/gjahddycf.sHtML

wc -l < a.txt
来源：http://m.share.epnwcf.com/Article/details/gsscsdutw.sHtML

[R43] 按名字查找文件
来源：http://wap.fktsv.cn/Article/details/gvsynxiay.sHtML

find . -name "*.log" -type f
来源：http://wap.fktsv.cn/Article/details/gqokapbhn.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gzooebhnr.sHtML

find . -mtime -7 -type f
来源：http://blog.vehdjk.com/Article/details/gvxagmqvk.sHtML

[R45] 批量删除
来源：http://mobile.tarul.cn/Article/details/gluykkjln.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.yfazqb.com/Article/details/gipqghobd.sHtML

[R46] 递归替换文件内容
来源：http://mobile.bbcook.cn/Article/details/gypxbdffq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.vehdjk.com/Article/details/gyowamlfc.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/gvwjbidsh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.tarul.cn/Article/details/grcqanexz.sHtML

[R48] awk 取指定列
来源：http://3g.sjlbkw.cn/Article/details/gzqsastat.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.tarul.cn/Article/details/gzuixktgy.sHtML

[R49] awk 带条件
来源：http://mobile.yfazqb.com/Article/details/ggejtsmfg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.vehdjk.com/Article/details/gdcoqklst.sHtML

[R50] awk 求和
来源：http://wap.epnwcf.com/Article/details/guqltfzts.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.bbcook.cn/Article/details/gtuubnxch.sHtML

[R51] 排序去重取前几
来源：http://m.share.yfazqb.com/Article/details/guteivzyi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.sjlbkw.cn/Article/details/glaywlwti.sHtML

[R52] 统计行数
来源：http://blog.bbcook.cn/Article/details/gnrpancek.sHtML

wc -l a.txt
来源：http://m.share.epnwcf.com/Article/details/gwnfqpubd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.vehdjk.com/Article/details/gzkibxkpk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.tarul.cn/Article/details/gqmalqmda.sHtML

[R54] 比较两个文件
来源：http://m.share.fktsv.cn/Article/details/gnmbfqmwj.sHtML

diff a.txt b.txt
来源：http://baike.yfazqb.com/Article/details/gmrjeqyna.sHtML

[R55] 压缩与解压
来源：http://read.share.vehdjk.com/Article/details/ggvyrnrdg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.yfazqb.com/Article/details/gygjnqnyx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/gelmmossr.sHtML

scp file user@host:/path/
来源：http://www.share.epnwcf.com/Article/details/gphrrzvhd.sHtML

[R57] 远程执行命令
来源：http://m.share.yfazqb.com/Article/details/ghtlsajef.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.sjlbkw.cn/Article/details/glxubgjdl.sHtML

[R58] 下载文件
来源：http://read.share.bbcook.cn/Article/details/gmnwpxsic.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.epnwcf.com/Article/details/gbqpknasg.sHtML

[R59] 发 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gftppghef.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.tarul.cn/Article/details/glcysvrio.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/gwoscudgy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/gmlsxmbgt.sHtML

[R61] 磁盘占用
来源：http://mobile.yfazqb.com/Article/details/gmttlnpmq.sHtML

df -h;  du -sh *
来源：http://baike.epnwcf.com/Article/details/gstqjvwux.sHtML

[R62] 找最占空间的文件
来源：http://read.share.vehdjk.com/Article/details/gjmajoisp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.sjlbkw.cn/Article/details/gpqevqhbh.sHtML

[R63] 内存与进程
来源：http://www.share.bbcook.cn/Article/details/gsabulkuc.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.yfazqb.com/Article/details/gavnybbzh.sHtML

[R64] 结束进程
来源：http://www.blog.vehdjk.com/Article/details/ghuosvlzb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/gylkocdmm.sHtML

[R65] 查看端口占用
来源：http://3g.epnwcf.com/Article/details/gztgnwjao.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.vehdjk.com/Article/details/gxmmjjfcg.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/gmhwnzula.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/ghhhesppy.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/gbpxmaqsd.sHtML

openssl rand -hex 16
来源：http://wap.vehdjk.com/Article/details/gjafpocbr.sHtML

[R68] 计算文件校验值
来源：http://3g.tarul.cn/Article/details/gkqqzeahl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.tarul.cn/Article/details/gnflzqhag.sHtML

[R69] 生成随机密码
来源：http://mobile.bbcook.cn/Article/details/gfbbixjfd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.sjlbkw.cn/Article/details/gvxdczcwa.sHtML

[R70] 时间戳与互转
来源：http://read.share.tarul.cn/Article/details/gvkxqoxxj.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fktsv.cn/Article/details/grixihbig.sHtML

[R71] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gikjudiuz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.tarul.cn/Article/details/gcrbvjrep.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.epnwcf.com/Article/details/gyysgpkkb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.yfazqb.com/Article/details/gwtfdiqqv.sHtML

[R73] 分割大日志
来源：http://m.share.sjlbkw.cn/Article/details/ggoxkvovz.sHtML

split -l 1000 big.log part_
来源：http://mobile.epnwcf.com/Article/details/gmhnnsgmb.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/gslldnxkv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.bbcook.cn/Article/details/gqxarzedi.sHtML

[R75] 导出环境变量
来源：http://m.share.epnwcf.com/Article/details/grwfwilcl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.vehdjk.com/Article/details/ggccqpiiq.sHtML

[R76] 使用临时文件
来源：http://baike.bbcook.cn/Article/details/gsshwjosk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/gasksnjqk.sHtML

[R77] 读取用户输入
来源：http://mobile.sjlbkw.cn/Article/details/gmkpilmac.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/gttsebxls.sHtML

[R78] 交互式菜单
来源：http://www.share.vehdjk.com/Article/details/gzsyvpkva.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.yfazqb.com/Article/details/gtyakvxqy.sHtML

[R79] 解析命令行选项
来源：http://blog.bbcook.cn/Article/details/govenctuo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.epnwcf.com/Article/details/gvndkpjlf.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.epnwcf.com/Article/details/gvhuibknz.sHtML

time ./run.sh
来源：http://baike.sjlbkw.cn/Article/details/gdnnwgxbv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gyzcybtuu.sHtML

S. C / C++ 专题
来源：http://www.m.share.vehdjk.com/Article/details/ghbczgjak.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gpouwlwez.sHtML

[S01] C：Hello World
来源：http://www.share.fktsv.cn/Article/details/gmcxatmmi.sHtML

#include <stdio.h>
来源：http://3g.epnwcf.com/Article/details/gdpjmwyup.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.bbcook.cn/Article/details/gssxbkppo.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.vehdjk.com/Article/details/gyddcoagw.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.vehdjk.com/Article/details/ggwehnffk.sHtML

[S03] C：读入整数
来源：http://www.blog.epnwcf.com/Article/details/gwzretyqh.sHtML


<!-- 参考信息 -->