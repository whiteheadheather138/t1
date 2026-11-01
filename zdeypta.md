代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gahxyengg.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/gjkcawgzo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/grcfgxvoh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.vehdjk.com/Article/details/gqbwayprt.sHtML

[Q33] 多列分组
来源：http://m.share.tarul.cn/Article/details/gdfqlyuqx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.tarul.cn/Article/details/graatzvnw.sHtML

[Q34] 每组取第一条
来源：http://m.share.vehdjk.com/Article/details/gwojdmvod.sHtML

SELECT * FROM (
来源：http://blog.sjlbkw.cn/Article/details/gadrcfphh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.yfazqb.com/Article/details/gtrjaqlad.sHtML

) t WHERE rn = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gryphfqvj.sHtML

[Q35] 内连接
来源：http://www.m.share.epnwcf.com/Article/details/gcthowgyg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/gotxvimbf.sHtML

[Q36] 左连接
来源：http://m.share.sjlbkw.cn/Article/details/gnnsohvgh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gxfwpmrfh.sHtML

[Q37] 右连接
来源：http://www.blog.bbcook.cn/Article/details/ggracbrmu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.vehdjk.com/Article/details/gjztxoeis.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fktsv.cn/Article/details/gucqndtnm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.tarul.cn/Article/details/gawhrhmyj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghitqcsnt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.sjlbkw.cn/Article/details/gkaqkqcsx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.vehdjk.com/Article/details/giydovtrm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.yfazqb.com/Article/details/gpslhpmad.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.vehdjk.com/Article/details/guduhpwvv.sHtML

[Q41] 多表连接
来源：http://blog.sjlbkw.cn/Article/details/gxkrefnst.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.bbcook.cn/Article/details/gnmfljfne.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.vehdjk.com/Article/details/gimntgqkc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.tarul.cn/Article/details/gqhqtrlxl.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.yfazqb.com/Article/details/gsncjamab.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.sjlbkw.cn/Article/details/ghplpzxld.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.bbcook.cn/Article/details/gngeqfiiq.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fktsv.cn/Article/details/gvvhxdngo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.sjlbkw.cn/Article/details/gdgiysglx.sHtML

[Q44] IN 子查询
来源：http://www.blog.sjlbkw.cn/Article/details/gcoarfgyd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.bbcook.cn/Article/details/gjcmxhofg.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.vehdjk.com/Article/details/gstolcyib.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.epnwcf.com/Article/details/gcnhxdcgo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/gykhodolq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gaqorbzjt.sHtML

[Q47] 与平均值比较
来源：http://blog.yfazqb.com/Article/details/gmeugoyhc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.bbcook.cn/Article/details/gpiskjgdr.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.yfazqb.com/Article/details/grvnhcquv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.tarul.cn/Article/details/grvyirwhh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.epnwcf.com/Article/details/gwpxlifbr.sHtML

[Q49] 更新单行
来源：http://blog.vehdjk.com/Article/details/gghcklhjo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gwgbdvmdh.sHtML

[Q50] 批量更新
来源：http://m.share.bbcook.cn/Article/details/gzlmfdfsq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.epnwcf.com/Article/details/gsowzeokc.sHtML

[Q51] 用子查询更新
来源：http://m.share.sjlbkw.cn/Article/details/gsadlzgfy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fktsv.cn/Article/details/guitbqzqt.sHtML

[Q52] 删除指定行
来源：http://m.share.yfazqb.com/Article/details/gadzvvavb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gsfxciiqc.sHtML

[Q53] 按条件删除
来源：http://3g.epnwcf.com/Article/details/guipybdmw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.vehdjk.com/Article/details/gtgkefifc.sHtML

[Q54] 清空表
来源：http://www.share.vehdjk.com/Article/details/ghbsxxqgs.sHtML

TRUNCATE TABLE logs;
来源：http://baike.vehdjk.com/Article/details/gbwqmihjw.sHtML

[Q55] 排名（并列占位）
来源：http://wap.bbcook.cn/Article/details/gjjdqwabd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gzbsowxnp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.epnwcf.com/Article/details/gyoglbesj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.epnwcf.com/Article/details/gfbvptpyx.sHtML

[Q57] 行号
来源：http://m.share.yfazqb.com/Article/details/gngbbpdoz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.vehdjk.com/Article/details/giozafgnw.sHtML

[Q58] 累计求和
来源：http://www.blog.vehdjk.com/Article/details/gcjfalotu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.epnwcf.com/Article/details/gyzftthjl.sHtML

[Q59] 分组内累计
来源：http://m.share.sjlbkw.cn/Article/details/gnrnzgkoq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gnqueoric.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.epnwcf.com/Article/details/gqwjfumtk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.sjlbkw.cn/Article/details/gemifaapi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gwdpcxmlu.sHtML

[Q61] 移动平均
来源：http://www.m.share.yfazqb.com/Article/details/gulkkzdid.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gsldlizax.sHtML

[Q62] 分组占比
来源：http://www.blog.fktsv.cn/Article/details/gpacwkqwc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gxklpfuqf.sHtML

[Q63] 开启事务
来源：http://mobile.fktsv.cn/Article/details/gjenhklbt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fktsv.cn/Article/details/gdcbqzhir.sHtML

[Q64] 提交事务
来源：http://www.blog.yfazqb.com/Article/details/gvusjamnf.sHtML

COMMIT;
来源：http://blog.fktsv.cn/Article/details/gwgdmidqk.sHtML

[Q65] 回滚事务
来源：http://wap.bbcook.cn/Article/details/gbsaktgxy.sHtML

ROLLBACK;
来源：http://mobile.tarul.cn/Article/details/gsnmyyfld.sHtML

[Q66] 行锁查询
来源：http://m.share.sjlbkw.cn/Article/details/gaxxxiyec.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.yfazqb.com/Article/details/gjeifkaxh.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fktsv.cn/Article/details/ghwolsecd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.bbcook.cn/Article/details/gxalneysh.sHtML

[Q68] 保存点
来源：http://wap.tarul.cn/Article/details/gnqrtxtrx.sHtML

SAVEPOINT sp1;
来源：http://read.share.yfazqb.com/Article/details/gfuafsveh.sHtML

ROLLBACK TO sp1;
来源：http://wap.epnwcf.com/Article/details/gvgmltnsv.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fktsv.cn/Article/details/giahuwpme.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.tarul.cn/Article/details/getyowjfh.sHtML

[Q70] 更新统计信息
来源：http://www.blog.yfazqb.com/Article/details/gjugnsrfv.sHtML

ANALYZE TABLE users;
来源：http://www.share.tarul.cn/Article/details/gfcthhcif.sHtML

[Q71] 查看建表语句
来源：http://blog.epnwcf.com/Article/details/gsfqzdwtm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.bbcook.cn/Article/details/gdygqgcky.sHtML

[Q72] 查看索引
来源：http://www.blog.yfazqb.com/Article/details/gzsvctuez.sHtML

SHOW INDEX FROM users;
来源：http://3g.fktsv.cn/Article/details/ghrxmulit.sHtML

[Q73] 查看表状态
来源：http://wap.fktsv.cn/Article/details/ghpjkqbmc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fktsv.cn/Article/details/glyvkblog.sHtML

[Q74] 强制使用索引
来源：http://mobile.epnwcf.com/Article/details/gmbpgpwnm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.yfazqb.com/Article/details/gpoouldru.sHtML

[Q75] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/gqoaylhww.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gvlfvyjjs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.vehdjk.com/Article/details/gmishjrfz.sHtML

[Q76] 按天统计
来源：http://m.share.bbcook.cn/Article/details/gowzilqzl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.epnwcf.com/Article/details/gdtmmrlde.sHtML

[Q77] 时间加减
来源：http://www.share.sjlbkw.cn/Article/details/gezcndjaa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.bbcook.cn/Article/details/gxkacodgt.sHtML

[Q78] 当前时间
来源：http://3g.tarul.cn/Article/details/gaequmtwu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fktsv.cn/Article/details/gstqhqzbb.sHtML

[Q79] 字符串拼接
来源：http://m.share.fktsv.cn/Article/details/gumjvtiwi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.vehdjk.com/Article/details/gwymixlzc.sHtML

[Q80] 字符串截取
来源：http://wap.tarul.cn/Article/details/gujtlydvn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.tarul.cn/Article/details/gejkkgcge.sHtML

[Q81] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gpgtxqysr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gmzhsdjpi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.vehdjk.com/Article/details/gkvltdehy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gjmqadlbf.sHtML

[Q83] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/ghhzpjcaj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gwcsxfxdl.sHtML

[Q84] 去除首尾空格
来源：http://wap.tarul.cn/Article/details/gwcvceomc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gktdvnvxa.sHtML

[Q85] 数值取整
来源：http://www.share.bbcook.cn/Article/details/gdwvflhwp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gqpcpogvs.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.bbcook.cn/Article/details/guzlamzyx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/gtituhdid.sHtML

[Q87] JSON 字段做条件
来源：http://blog.vehdjk.com/Article/details/guoboasrz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fktsv.cn/Article/details/gfysndbpg.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fktsv.cn/Article/details/goynqkoit.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.bbcook.cn/Article/details/graqxfifc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.tarul.cn/Article/details/gvxsqtaby.sHtML

[Q89] 判断表是否存在
来源：http://3g.bbcook.cn/Article/details/gpkjncusu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.yfazqb.com/Article/details/gelhocrnp.sHtML

[Q90] 生成序号列
来源：http://blog.tarul.cn/Article/details/gikmopmrd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.sjlbkw.cn/Article/details/gaahuycus.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggymwliul.sHtML

R. Bash 专题
来源：http://3g.epnwcf.com/Article/details/gnbpabqla.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gixpirxpa.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.sjlbkw.cn/Article/details/ghichhunf.sHtML

#!/usr/bin/env bash
来源：http://m.share.tarul.cn/Article/details/gzcganlkl.sHtML

set -euo pipefail
来源：http://blog.sjlbkw.cn/Article/details/gsvtjzevn.sHtML

[R02] 变量赋值与使用
来源：http://blog.fktsv.cn/Article/details/gwgmwstic.sHtML

name="Tom"; echo "$name"
来源：http://blog.yfazqb.com/Article/details/gvzefjtiz.sHtML

[R03] 只读变量
来源：http://mobile.epnwcf.com/Article/details/gokxmvntg.sHtML

readonly PI=3.14
来源：http://blog.bbcook.cn/Article/details/gncxcfbir.sHtML

[R04] 位置参数
来源：http://www.share.fktsv.cn/Article/details/gchnsihmz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.tarul.cn/Article/details/ghzdarisd.sHtML

[R05] 参数默认值
来源：http://baike.vehdjk.com/Article/details/gkfhzmosi.sHtML

name="${1:-default}"
来源：http://3g.yfazqb.com/Article/details/gzilsdlhl.sHtML

[R06] 判断命令是否存在
来源：http://www.share.vehdjk.com/Article/details/grdxmmjxf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/grkortccp.sHtML

[R07] if 判断文件
来源：http://3g.fktsv.cn/Article/details/gatsxexnr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.yfazqb.com/Article/details/gsqsocxlz.sHtML

[R08] 数值比较
来源：http://3g.bbcook.cn/Article/details/gntuapslm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.tarul.cn/Article/details/gaozogbvz.sHtML

[R09] 字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gpkupqgfj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.epnwcf.com/Article/details/gyzsolbfo.sHtML

[R10] 正则匹配
来源：http://m.share.fktsv.cn/Article/details/gikdzpwgz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.epnwcf.com/Article/details/glzyyocwz.sHtML

[R11] case 多分支
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuyeewdj.sHtML

case "$1" in
来源：http://www.share.sjlbkw.cn/Article/details/gqtofurwc.sHtML

start) echo "启动" ;;
来源：http://3g.epnwcf.com/Article/details/gpmklawfe.sHtML

stop)  echo "停止" ;;
来源：http://read.share.tarul.cn/Article/details/gkboicukt.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gbswqicii.sHtML

esac
来源：http://m.share.sjlbkw.cn/Article/details/gxlulvdqf.sHtML

[R12] for 遍历文件
来源：http://www.share.bbcook.cn/Article/details/ghykaltlw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.vehdjk.com/Article/details/gmkxlkzur.sHtML

[R13] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gfjyjtotf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fktsv.cn/Article/details/ghwpghkfw.sHtML

[R14] C 风格 for
来源：http://www.m.share.tarul.cn/Article/details/gpkezvdzj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/glzqfbmzf.sHtML

[R15] while 逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gdhctyloa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fktsv.cn/Article/details/gjctvgwbl.sHtML

[R16] until 等待条件
来源：http://www.share.epnwcf.com/Article/details/gmonuovuz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/grimxwtzj.sHtML

[R17] 数组定义与取值
来源：http://www.share.yfazqb.com/Article/details/gvuhwdxsx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.epnwcf.com/Article/details/gujspyvoz.sHtML

[R18] 遍历数组
来源：http://www.m.share.fktsv.cn/Article/details/gnifgwdzz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.tarul.cn/Article/details/gnfytbkah.sHtML

[R19] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gtdpvxxwz.sHtML

echo "${#arr[@]}"
来源：http://wap.sjlbkw.cn/Article/details/ggnyzettz.sHtML

[R20] 关联数组（字典）
来源：http://baike.sjlbkw.cn/Article/details/gfvvzrjil.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.yfazqb.com/Article/details/gdafdnyfw.sHtML

[R21] 字符串长度
来源：http://blog.epnwcf.com/Article/details/glbusxtgz.sHtML

echo "${#s}"
来源：http://m.share.sjlbkw.cn/Article/details/gkpadmenv.sHtML

[R22] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gixtawwzq.sHtML

echo "${s:0:5}"
来源：http://www.blog.epnwcf.com/Article/details/grwnycwtm.sHtML

[R23] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gdzsxpdqy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.bbcook.cn/Article/details/gfolaxfxw.sHtML

[R24] 大小写转换
来源：http://baike.tarul.cn/Article/details/gckqycara.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.tarul.cn/Article/details/glbbdmpyq.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.vehdjk.com/Article/details/gviqcesle.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.epnwcf.com/Article/details/gqpjpzxuu.sHtML

[R26] 命令替换
来源：http://blog.bbcook.cn/Article/details/gjammadxq.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.epnwcf.com/Article/details/ghjfuclbf.sHtML

[R27] 算术展开
来源：http://www.m.share.yfazqb.com/Article/details/grhivldaa.sHtML

echo $((1 + 2 * 3))
来源：http://baike.tarul.cn/Article/details/gqqcspbpl.sHtML

[R28] 浮点运算
来源：http://baike.bbcook.cn/Article/details/gsgiccrhv.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.bbcook.cn/Article/details/gwhcsztcu.sHtML

[R29] 定义函数
来源：http://www.share.bbcook.cn/Article/details/grchvjcwd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fktsv.cn/Article/details/gcijsbihl.sHtML

[R30] 函数返回状态码
来源：http://3g.tarul.cn/Article/details/gcqydqebs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fktsv.cn/Article/details/gqgkzpvvw.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gmdcsbxbt.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.yfazqb.com/Article/details/gaxbiveli.sHtML

[R32] 参数个数校验
来源：http://baike.sjlbkw.cn/Article/details/ggqleosha.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gtcdhpqou.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/gfgdbyhdi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.vehdjk.com/Article/details/gfqpwdbxz.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/geeyrlkyq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gckrrdrbo.sHtML

[R35] 后台执行并等待
来源：http://baike.yfazqb.com/Article/details/gpkhkuohr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fktsv.cn/Article/details/ghsgedpxk.sHtML

[R36] 并发执行多个任务
来源：http://read.share.tarul.cn/Article/details/gnmvvkncr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.yfazqb.com/Article/details/gndplwycr.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fktsv.cn/Article/details/glkjnjuaf.sHtML

files=$(ls -1)
来源：http://wap.bbcook.cn/Article/details/gvrsigcku.sHtML

[R38] 管道串联
来源：http://wap.fktsv.cn/Article/details/gxutsyxyp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.tarul.cn/Article/details/gqihcqrwm.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.bbcook.cn/Article/details/gjbdtjyzi.sHtML

cmd > out.log 2>&1
来源：http://m.share.epnwcf.com/Article/details/gkqjpoqyr.sHtML

[R40] 追加写日志
来源：http://m.share.sjlbkw.cn/Article/details/gpqythovf.sHtML

echo "log" >> out.log
来源：http://3g.fktsv.cn/Article/details/ganpecziq.sHtML

[R41] 丢弃输出
来源：http://www.m.share.yfazqb.com/Article/details/gwkahniiz.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gmikyumhh.sHtML

[R42] 输入重定向
来源：http://3g.sjlbkw.cn/Article/details/ghcnuicmc.sHtML

wc -l < a.txt
来源：http://wap.vehdjk.com/Article/details/goxptpvih.sHtML

[R43] 按名字查找文件
来源：http://baike.fktsv.cn/Article/details/gorqzdatz.sHtML

find . -name "*.log" -type f
来源：http://www.blog.yfazqb.com/Article/details/gujgvhcdp.sHtML

[R44] 按修改时间查找
来源：http://www.share.vehdjk.com/Article/details/gvveupgns.sHtML

find . -mtime -7 -type f
来源：http://wap.bbcook.cn/Article/details/gkbrxetiq.sHtML

[R45] 批量删除
来源：http://mobile.tarul.cn/Article/details/gszwgpyue.sHtML

find . -name "*.tmp" -delete
来源：http://baike.bbcook.cn/Article/details/gkopmyuji.sHtML

[R46] 递归替换文件内容
来源：http://blog.bbcook.cn/Article/details/glpemxhou.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.yfazqb.com/Article/details/gtrggpgvv.sHtML

[R47] sed 单行替换
来源：http://blog.vehdjk.com/Article/details/gyxozkfnd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/guospswgw.sHtML

[R48] awk 取指定列
来源：http://www.share.bbcook.cn/Article/details/gjtpcvdwh.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.tarul.cn/Article/details/gdbdumhcc.sHtML

[R49] awk 带条件
来源：http://www.m.share.bbcook.cn/Article/details/gxqtyxwlw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.vehdjk.com/Article/details/gjfxymimd.sHtML

[R50] awk 求和
来源：http://baike.epnwcf.com/Article/details/gwmserjzj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.bbcook.cn/Article/details/gfpibnxja.sHtML

[R51] 排序去重取前几
来源：http://www.share.yfazqb.com/Article/details/grcqfnknm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.vehdjk.com/Article/details/goekxztls.sHtML

[R52] 统计行数
来源：http://baike.yfazqb.com/Article/details/ggizeopto.sHtML

wc -l a.txt
来源：http://3g.fktsv.cn/Article/details/ghbkbvewk.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fktsv.cn/Article/details/glheodmsc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.sjlbkw.cn/Article/details/gnryjmxma.sHtML

[R54] 比较两个文件
来源：http://mobile.fktsv.cn/Article/details/gpmzykwcu.sHtML

diff a.txt b.txt
来源：http://www.m.share.tarul.cn/Article/details/geowoqbkg.sHtML

[R55] 压缩与解压
来源：http://wap.bbcook.cn/Article/details/grxkhzyqi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.tarul.cn/Article/details/goszbwgai.sHtML

[R56] 远程拷贝
来源：http://read.share.fktsv.cn/Article/details/gyjkmxxfw.sHtML

scp file user@host:/path/
来源：http://mobile.vehdjk.com/Article/details/gemomrtgn.sHtML

[R57] 远程执行命令
来源：http://wap.yfazqb.com/Article/details/gmckucefe.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.tarul.cn/Article/details/gcbjnjuzu.sHtML

[R58] 下载文件
来源：http://wap.yfazqb.com/Article/details/ggzcgjmui.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/gvvqvkgmt.sHtML

[R59] 发 POST JSON
来源：http://wap.epnwcf.com/Article/details/gtlfwqtgv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.epnwcf.com/Article/details/ghlcgbpmd.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gghedjimd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.bbcook.cn/Article/details/gydibxfju.sHtML

[R61] 磁盘占用
来源：http://wap.fktsv.cn/Article/details/gafmrhaqh.sHtML

df -h;  du -sh *
来源：http://wap.bbcook.cn/Article/details/gzgxkvaix.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.epnwcf.com/Article/details/gyqsrfvwb.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.tarul.cn/Article/details/gsledxftm.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gpmtinukw.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.epnwcf.com/Article/details/gidaztxeo.sHtML

[R64] 结束进程
来源：http://read.share.bbcook.cn/Article/details/gpglnxgce.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.vehdjk.com/Article/details/gtomtcepy.sHtML

[R65] 查看端口占用
来源：http://m.share.yfazqb.com/Article/details/gzfjqjnqt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.yfazqb.com/Article/details/gjmfzdbxq.sHtML

[R66] 定时任务
来源：http://baike.yfazqb.com/Article/details/gellpxhzz.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.epnwcf.com/Article/details/glkqthpnn.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.sjlbkw.cn/Article/details/gwfdmkkhs.sHtML

openssl rand -hex 16
来源：http://www.share.tarul.cn/Article/details/gylbjyiou.sHtML

[R68] 计算文件校验值
来源：http://3g.fktsv.cn/Article/details/gsubospbk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fktsv.cn/Article/details/gcokzkghy.sHtML

[R69] 生成随机密码
来源：http://www.blog.epnwcf.com/Article/details/gtfpwvqbb.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.sjlbkw.cn/Article/details/gmbhghdyg.sHtML

[R70] 时间戳与互转
来源：http://3g.yfazqb.com/Article/details/gjsfndhcr.sHtML

date +%s;  date -d @1700000000
来源：http://wap.bbcook.cn/Article/details/gbwxgdwsk.sHtML

[R71] 日期格式化
来源：http://wap.fktsv.cn/Article/details/gqnhisavo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.bbcook.cn/Article/details/glcotrpow.sHtML

[R72] 等待端口就绪
来源：http://m.share.sjlbkw.cn/Article/details/gnxipqiha.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gbesepeqt.sHtML

[R73] 分割大日志
来源：http://3g.yfazqb.com/Article/details/gsyqzxyqa.sHtML

split -l 1000 big.log part_
来源：http://baike.fktsv.cn/Article/details/gxktlcmlo.sHtML

[R74] 批量重命名
来源：http://www.share.yfazqb.com/Article/details/gauhjurkv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.vehdjk.com/Article/details/geusksnsx.sHtML

[R75] 导出环境变量
来源：http://mobile.epnwcf.com/Article/details/gzcompsrw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.tarul.cn/Article/details/gkmmtxrbn.sHtML

[R76] 使用临时文件
来源：http://blog.bbcook.cn/Article/details/gqyqfojqm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.tarul.cn/Article/details/gwfkjdgds.sHtML

[R77] 读取用户输入
来源：http://www.blog.bbcook.cn/Article/details/grxrhhpds.sHtML

read -rp "请输入: " ans
来源：http://www.blog.sjlbkw.cn/Article/details/gqbpjfwon.sHtML

[R78] 交互式菜单
来源：http://3g.bbcook.cn/Article/details/ggmivvtyi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fktsv.cn/Article/details/gmvrriock.sHtML

[R79] 解析命令行选项
来源：http://mobile.vehdjk.com/Article/details/gwwdsnlra.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.yfazqb.com/Article/details/gdlnkvjdk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.tarul.cn/Article/details/gaojczdug.sHtML

time ./run.sh
来源：http://www.blog.yfazqb.com/Article/details/ghsiktfbr.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gicdqjkjd.sHtML


<!-- 参考信息 -->