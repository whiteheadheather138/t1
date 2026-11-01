代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.tarul.cn/Article/details/gnevgphhz.sHtML

[Q28] 求和与平均
来源：http://mobile.yfazqb.com/Article/details/guhwaajrv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/goxkixrny.sHtML

[Q29] 最大最小值
来源：http://wap.epnwcf.com/Article/details/gdkkadqts.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fktsv.cn/Article/details/gmtrhgtmn.sHtML

[Q30] 分组统计
来源：http://www.share.bbcook.cn/Article/details/gnpjvfyoi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gokjvkdpq.sHtML

[Q31] 分组后过滤
来源：http://wap.fktsv.cn/Article/details/gxtesscms.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.sjlbkw.cn/Article/details/gnppcfbyg.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.epnwcf.com/Article/details/grrkoaaqe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gjscpmudy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.vehdjk.com/Article/details/gnoazwwxx.sHtML

[Q33] 多列分组
来源：http://www.share.epnwcf.com/Article/details/ggoaobfjp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.vehdjk.com/Article/details/gdfvpczmz.sHtML

[Q34] 每组取第一条
来源：http://mobile.tarul.cn/Article/details/gegrqtdmt.sHtML

SELECT * FROM (
来源：http://read.share.fktsv.cn/Article/details/geqfyqqki.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.sjlbkw.cn/Article/details/ghhwqzaml.sHtML

) t WHERE rn = 1;
来源：http://wap.tarul.cn/Article/details/gdhrrfelm.sHtML

[Q35] 内连接
来源：http://m.share.epnwcf.com/Article/details/gdqnhtopc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gwkkzxenm.sHtML

[Q36] 左连接
来源：http://read.share.bbcook.cn/Article/details/ggltpttso.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gjxazsttz.sHtML

[Q37] 右连接
来源：http://wap.sjlbkw.cn/Article/details/groxijtkm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fktsv.cn/Article/details/gljeouhze.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.bbcook.cn/Article/details/gwpyrosjh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fktsv.cn/Article/details/gknkjfsed.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.bbcook.cn/Article/details/gwktmtrxx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.epnwcf.com/Article/details/glmhjhxml.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/grpqxbzvn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.vehdjk.com/Article/details/grufjrteq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.bbcook.cn/Article/details/gcsitvohk.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/gcylfypaq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fktsv.cn/Article/details/gzzouzkwg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.vehdjk.com/Article/details/gpxvpzoem.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.tarul.cn/Article/details/gnutzdrba.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.sjlbkw.cn/Article/details/gbwvaubhn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.epnwcf.com/Article/details/gpzyxwwsp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.yfazqb.com/Article/details/geiioncvm.sHtML

[Q43] 标量子查询
来源：http://read.share.sjlbkw.cn/Article/details/gcbsppgyo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.epnwcf.com/Article/details/gvyaywulf.sHtML

[Q44] IN 子查询
来源：http://wap.sjlbkw.cn/Article/details/gshtnpbgj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.sjlbkw.cn/Article/details/gttzojchb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.bbcook.cn/Article/details/gujwgpuek.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/gecdojcab.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.tarul.cn/Article/details/gcrjxfkhc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.yfazqb.com/Article/details/gunzuccuu.sHtML

[Q47] 与平均值比较
来源：http://m.share.bbcook.cn/Article/details/gptkpjqgz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.yfazqb.com/Article/details/glawkqqfl.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.sjlbkw.cn/Article/details/gxgbgyfjn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.yfazqb.com/Article/details/gyydbvizr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.bbcook.cn/Article/details/ghosladhv.sHtML

[Q49] 更新单行
来源：http://wap.yfazqb.com/Article/details/gwcmkpsgo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gsarffmjk.sHtML

[Q50] 批量更新
来源：http://m.share.tarul.cn/Article/details/gvughtcnd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.vehdjk.com/Article/details/gqqnrrhea.sHtML

[Q51] 用子查询更新
来源：http://read.share.bbcook.cn/Article/details/grvklszey.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fktsv.cn/Article/details/gdjuxvoxg.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/gzrumjvlp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/govclzmsg.sHtML

[Q53] 按条件删除
来源：http://mobile.sjlbkw.cn/Article/details/gtjdhviwd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gxbukfrsr.sHtML

[Q54] 清空表
来源：http://wap.bbcook.cn/Article/details/goseniuzd.sHtML

TRUNCATE TABLE logs;
来源：http://3g.vehdjk.com/Article/details/ghwmfjqnb.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fktsv.cn/Article/details/gffzrosyp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/gykpttahr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.yfazqb.com/Article/details/gbufxdzsf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fktsv.cn/Article/details/gghcvocsi.sHtML

[Q57] 行号
来源：http://read.share.vehdjk.com/Article/details/gbvmcbgza.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fktsv.cn/Article/details/goslzckpd.sHtML

[Q58] 累计求和
来源：http://mobile.sjlbkw.cn/Article/details/gyljyennz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gmflbisds.sHtML

[Q59] 分组内累计
来源：http://www.m.share.bbcook.cn/Article/details/gawfkfuhi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.vehdjk.com/Article/details/grqmltpbf.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fktsv.cn/Article/details/gaiusoenn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.yfazqb.com/Article/details/gnjhfllyo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.vehdjk.com/Article/details/guxtmcctd.sHtML

[Q61] 移动平均
来源：http://www.blog.tarul.cn/Article/details/gfjyvgxud.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxosegve.sHtML

[Q62] 分组占比
来源：http://mobile.fktsv.cn/Article/details/guukqnfyw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gpuhvswda.sHtML

[Q63] 开启事务
来源：http://mobile.sjlbkw.cn/Article/details/gmmylwvcd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/gtfsmqhmw.sHtML

[Q64] 提交事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gszylmrro.sHtML

COMMIT;
来源：http://3g.bbcook.cn/Article/details/gtevxanif.sHtML

[Q65] 回滚事务
来源：http://baike.fktsv.cn/Article/details/gksfnwmrc.sHtML

ROLLBACK;
来源：http://blog.tarul.cn/Article/details/gqoobrbqp.sHtML

[Q66] 行锁查询
来源：http://wap.tarul.cn/Article/details/gpbsaudif.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.yfazqb.com/Article/details/gjjkbpxyq.sHtML

[Q67] 设置隔离级别
来源：http://m.share.tarul.cn/Article/details/gallsedim.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.tarul.cn/Article/details/gflmtspic.sHtML

[Q68] 保存点
来源：http://blog.tarul.cn/Article/details/gyfhbplvt.sHtML

SAVEPOINT sp1;
来源：http://wap.sjlbkw.cn/Article/details/gvwjixldf.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fktsv.cn/Article/details/ghdpusorp.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gtqzwjzms.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.bbcook.cn/Article/details/ghckfwxes.sHtML

[Q70] 更新统计信息
来源：http://blog.tarul.cn/Article/details/gylvenoam.sHtML

ANALYZE TABLE users;
来源：http://3g.vehdjk.com/Article/details/gjkunqjyq.sHtML

[Q71] 查看建表语句
来源：http://3g.sjlbkw.cn/Article/details/gfxyduzkx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fktsv.cn/Article/details/griobihrj.sHtML

[Q72] 查看索引
来源：http://www.blog.tarul.cn/Article/details/gqowatazs.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fktsv.cn/Article/details/gzpkpvrir.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/gccuqqudo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.vehdjk.com/Article/details/gpgwhqpfj.sHtML

[Q74] 强制使用索引
来源：http://mobile.vehdjk.com/Article/details/gqmgvhfhd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.tarul.cn/Article/details/gsgiazabx.sHtML

[Q75] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gcmofsjjr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gfnnsvdih.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.yfazqb.com/Article/details/gkltgagmz.sHtML

[Q76] 按天统计
来源：http://www.share.yfazqb.com/Article/details/gdmzeavym.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.sjlbkw.cn/Article/details/gxyxazyow.sHtML

[Q77] 时间加减
来源：http://3g.tarul.cn/Article/details/gqlnjyshv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.bbcook.cn/Article/details/gljquxgrt.sHtML

[Q78] 当前时间
来源：http://blog.tarul.cn/Article/details/glrufpcko.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.tarul.cn/Article/details/gzgdgymwj.sHtML

[Q79] 字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gbmsktkag.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.yfazqb.com/Article/details/gtneuhflz.sHtML

[Q80] 字符串截取
来源：http://wap.yfazqb.com/Article/details/gboayyqnq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gjqrgjxik.sHtML

[Q81] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gfizlzbyb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/grxqziqyz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.epnwcf.com/Article/details/gbamyuxwn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gzgyaicre.sHtML

[Q83] 大小写转换
来源：http://3g.epnwcf.com/Article/details/ggvuuodgv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gxiqulvgt.sHtML

[Q84] 去除首尾空格
来源：http://wap.tarul.cn/Article/details/gzxjrluas.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gxwickjkp.sHtML

[Q85] 数值取整
来源：http://www.m.share.yfazqb.com/Article/details/gauamwunj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.epnwcf.com/Article/details/gjcrklcwo.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fktsv.cn/Article/details/girkviyem.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.epnwcf.com/Article/details/gbilmnncz.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.sjlbkw.cn/Article/details/geryxummb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.vehdjk.com/Article/details/gzggycttc.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.tarul.cn/Article/details/ghlgzship.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.sjlbkw.cn/Article/details/gogxmwdsi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/grqoyjgpl.sHtML

[Q89] 判断表是否存在
来源：http://blog.vehdjk.com/Article/details/gyfdwbavs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.sjlbkw.cn/Article/details/gcymxyyuf.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/gfkcvnzbi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.bbcook.cn/Article/details/gazbdyjyc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grgowegjt.sHtML

R. Bash 专题
来源：http://m.share.fktsv.cn/Article/details/gokvlhtqz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gidzwyyzq.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/gdtfujhnw.sHtML

#!/usr/bin/env bash
来源：http://baike.fktsv.cn/Article/details/gexqbmert.sHtML

set -euo pipefail
来源：http://mobile.sjlbkw.cn/Article/details/gcxagmixg.sHtML

[R02] 变量赋值与使用
来源：http://blog.epnwcf.com/Article/details/gfllhqbdx.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.yfazqb.com/Article/details/gsdywvvbn.sHtML

[R03] 只读变量
来源：http://baike.sjlbkw.cn/Article/details/glbacgbsl.sHtML

readonly PI=3.14
来源：http://3g.yfazqb.com/Article/details/gsqjspdae.sHtML

[R04] 位置参数
来源：http://www.blog.fktsv.cn/Article/details/guathvdec.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.bbcook.cn/Article/details/gxwbjglaf.sHtML

[R05] 参数默认值
来源：http://mobile.bbcook.cn/Article/details/gzijvwuwt.sHtML

name="${1:-default}"
来源：http://3g.fktsv.cn/Article/details/gsngomkfg.sHtML

[R06] 判断命令是否存在
来源：http://3g.sjlbkw.cn/Article/details/gqxyodnbi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gzvzyhuwf.sHtML

[R07] if 判断文件
来源：http://baike.vehdjk.com/Article/details/gipsqigqf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.vehdjk.com/Article/details/ggjkqzcyj.sHtML

[R08] 数值比较
来源：http://www.blog.yfazqb.com/Article/details/ggwlctbue.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.epnwcf.com/Article/details/ggbacjjag.sHtML

[R09] 字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gmozexcwt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.sjlbkw.cn/Article/details/gsecmnyea.sHtML

[R10] 正则匹配
来源：http://www.share.fktsv.cn/Article/details/gzfurejaz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.bbcook.cn/Article/details/gdqzgrnff.sHtML

[R11] case 多分支
来源：http://m.share.yfazqb.com/Article/details/gjhkiefxp.sHtML

case "$1" in
来源：http://read.share.fktsv.cn/Article/details/gelfuyayf.sHtML

start) echo "启动" ;;
来源：http://read.share.yfazqb.com/Article/details/gsipcrljy.sHtML

stop)  echo "停止" ;;
来源：http://3g.epnwcf.com/Article/details/gsiznamvm.sHtML

*)     echo "未知命令" ;;
来源：http://blog.vehdjk.com/Article/details/grpntmvin.sHtML

esac
来源：http://3g.vehdjk.com/Article/details/gqddfareq.sHtML

[R12] for 遍历文件
来源：http://www.m.share.yfazqb.com/Article/details/gceiaqhip.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.bbcook.cn/Article/details/gyddbdyug.sHtML

[R13] for 计数循环
来源：http://wap.tarul.cn/Article/details/grogaorso.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gtitieytn.sHtML

[R14] C 风格 for
来源：http://wap.yfazqb.com/Article/details/gqhovuohi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/gfypaopse.sHtML

[R15] while 逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gqbfnrqai.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.epnwcf.com/Article/details/girjoqppl.sHtML

[R16] until 等待条件
来源：http://read.share.epnwcf.com/Article/details/gnlgxtsrw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gszckspri.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.bbcook.cn/Article/details/gzwiwgcwu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.epnwcf.com/Article/details/gvgirmjqe.sHtML

[R18] 遍历数组
来源：http://wap.fktsv.cn/Article/details/gmrpcnnvs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fktsv.cn/Article/details/gclznkcua.sHtML

[R19] 数组长度
来源：http://blog.epnwcf.com/Article/details/glzdxptku.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/gxkcqelmp.sHtML

[R20] 关联数组（字典）
来源：http://m.share.epnwcf.com/Article/details/gidmrzwlo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.epnwcf.com/Article/details/gxzfcpfid.sHtML

[R21] 字符串长度
来源：http://read.share.bbcook.cn/Article/details/ggbdcqmaz.sHtML

echo "${#s}"
来源：http://m.share.tarul.cn/Article/details/gfftqeaql.sHtML

[R22] 截取子串
来源：http://blog.tarul.cn/Article/details/grlogyyiv.sHtML

echo "${s:0:5}"
来源：http://www.share.fktsv.cn/Article/details/gyhiajbpz.sHtML

[R23] 字符串替换
来源：http://baike.yfazqb.com/Article/details/gjrnsxxce.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.yfazqb.com/Article/details/gzyhbnlbe.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/glxfhwpus.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fktsv.cn/Article/details/grecvqdbk.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.vehdjk.com/Article/details/gzsundjnd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.tarul.cn/Article/details/gfrxokazr.sHtML

[R26] 命令替换
来源：http://mobile.epnwcf.com/Article/details/giormycoq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.sjlbkw.cn/Article/details/gplhqdqgz.sHtML

[R27] 算术展开
来源：http://m.share.tarul.cn/Article/details/gkruuruqn.sHtML

echo $((1 + 2 * 3))
来源：http://baike.yfazqb.com/Article/details/gkelcdmyi.sHtML

[R28] 浮点运算
来源：http://blog.epnwcf.com/Article/details/gtumcdumb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.bbcook.cn/Article/details/gruggooxv.sHtML

[R29] 定义函数
来源：http://mobile.epnwcf.com/Article/details/giwkjjqel.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.sjlbkw.cn/Article/details/gnttdvqje.sHtML

[R30] 函数返回状态码
来源：http://m.share.yfazqb.com/Article/details/ggqjjbzxa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fktsv.cn/Article/details/gshmlnpvd.sHtML

[R31] 局部变量
来源：http://www.blog.vehdjk.com/Article/details/grxtotfgx.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.epnwcf.com/Article/details/gfbrgkazd.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fktsv.cn/Article/details/gopayiqgy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gugongfui.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.bbcook.cn/Article/details/gnqkcqkcy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fktsv.cn/Article/details/gddvnihiu.sHtML

[R34] 退出时清理
来源：http://www.blog.tarul.cn/Article/details/gqbkqgnnz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gsunjtvfa.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.sjlbkw.cn/Article/details/gufovuics.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.yfazqb.com/Article/details/gyrwmwbyy.sHtML

[R36] 并发执行多个任务
来源：http://baike.yfazqb.com/Article/details/gwyozcxaa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.sjlbkw.cn/Article/details/gnovrpqfn.sHtML

[R37] 把输出赋给变量
来源：http://3g.vehdjk.com/Article/details/gtwssduez.sHtML

files=$(ls -1)
来源：http://mobile.fktsv.cn/Article/details/gasjmexhf.sHtML

[R38] 管道串联
来源：http://baike.sjlbkw.cn/Article/details/ggssxlniy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.bbcook.cn/Article/details/gvjnlaexy.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.bbcook.cn/Article/details/gysjmwgbl.sHtML

cmd > out.log 2>&1
来源：http://wap.yfazqb.com/Article/details/gsfzalugu.sHtML

[R40] 追加写日志
来源：http://blog.tarul.cn/Article/details/gksmjsmah.sHtML

echo "log" >> out.log
来源：http://www.m.share.vehdjk.com/Article/details/gtrkatlyj.sHtML

[R41] 丢弃输出
来源：http://baike.epnwcf.com/Article/details/gyjuysxzh.sHtML

cmd >/dev/null 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gosaloqup.sHtML

[R42] 输入重定向
来源：http://3g.vehdjk.com/Article/details/gwvmadhap.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/guebfstsw.sHtML

[R43] 按名字查找文件
来源：http://read.share.bbcook.cn/Article/details/gsiqloadn.sHtML

find . -name "*.log" -type f
来源：http://baike.sjlbkw.cn/Article/details/ggbnimhpb.sHtML

[R44] 按修改时间查找
来源：http://blog.tarul.cn/Article/details/gzdtidmtk.sHtML

find . -mtime -7 -type f
来源：http://www.blog.yfazqb.com/Article/details/glksedgrz.sHtML

[R45] 批量删除
来源：http://blog.tarul.cn/Article/details/goigoxbvp.sHtML

find . -name "*.tmp" -delete
来源：http://blog.sjlbkw.cn/Article/details/gyqgijixl.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gubtoukmi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.yfazqb.com/Article/details/garumbtvv.sHtML

[R47] sed 单行替换
来源：http://wap.epnwcf.com/Article/details/gotryfenb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fktsv.cn/Article/details/gpidzzoex.sHtML

[R48] awk 取指定列
来源：http://wap.epnwcf.com/Article/details/gscjsugcy.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.tarul.cn/Article/details/gungfwzbm.sHtML

[R49] awk 带条件
来源：http://www.m.share.bbcook.cn/Article/details/gdbumdtjy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.vehdjk.com/Article/details/gvdcitgld.sHtML

[R50] awk 求和
来源：http://www.share.fktsv.cn/Article/details/gwpvowrbl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.bbcook.cn/Article/details/geyzukysa.sHtML

[R51] 排序去重取前几
来源：http://read.share.bbcook.cn/Article/details/gssywlzgm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/ghkdkjmtq.sHtML

[R52] 统计行数
来源：http://3g.bbcook.cn/Article/details/ggyzpjxso.sHtML

wc -l a.txt
来源：http://blog.fktsv.cn/Article/details/gdhnsntfp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.vehdjk.com/Article/details/grjkljcbd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.bbcook.cn/Article/details/ghprnftrq.sHtML

[R54] 比较两个文件
来源：http://www.m.share.vehdjk.com/Article/details/glsrivpkm.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/gkqlwberl.sHtML

[R55] 压缩与解压
来源：http://www.blog.fktsv.cn/Article/details/grkevkbxq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.bbcook.cn/Article/details/gbhrtcwbj.sHtML

[R56] 远程拷贝
来源：http://www.blog.fktsv.cn/Article/details/ghrqipbqz.sHtML

scp file user@host:/path/
来源：http://wap.epnwcf.com/Article/details/godxtvgbc.sHtML

[R57] 远程执行命令
来源：http://3g.tarul.cn/Article/details/gbcskkjxv.sHtML

ssh user@host 'uptime'
来源：http://www.share.fktsv.cn/Article/details/gtgfglvta.sHtML

[R58] 下载文件
来源：http://baike.bbcook.cn/Article/details/gdnqfvwig.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.bbcook.cn/Article/details/gngbuvqnn.sHtML

[R59] 发 POST JSON
来源：http://baike.bbcook.cn/Article/details/gceudwfej.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.epnwcf.com/Article/details/gcvyfhuwo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/ggxxqbrtm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.sjlbkw.cn/Article/details/gkxxpbmxf.sHtML

[R61] 磁盘占用
来源：http://wap.bbcook.cn/Article/details/gfdhwjjis.sHtML

df -h;  du -sh *
来源：http://baike.sjlbkw.cn/Article/details/giicwshxc.sHtML

[R62] 找最占空间的文件
来源：http://read.share.bbcook.cn/Article/details/gesqiozqs.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.yfazqb.com/Article/details/gtnvometz.sHtML

[R63] 内存与进程
来源：http://mobile.sjlbkw.cn/Article/details/grbhrwmae.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.yfazqb.com/Article/details/ggesetwvj.sHtML

[R64] 结束进程
来源：http://read.share.fktsv.cn/Article/details/gpzjskzgf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fktsv.cn/Article/details/gxjzmhlkr.sHtML

[R65] 查看端口占用
来源：http://wap.yfazqb.com/Article/details/garukcduk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fktsv.cn/Article/details/gfpftsbts.sHtML

[R66] 定时任务
来源：http://mobile.vehdjk.com/Article/details/geazcuqkn.sHtML

crontab -e;  crontab -l
来源：http://3g.bbcook.cn/Article/details/gzvwxdgle.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.tarul.cn/Article/details/gcslfcmzx.sHtML

openssl rand -hex 16
来源：http://www.blog.epnwcf.com/Article/details/gikjposjs.sHtML

[R68] 计算文件校验值
来源：http://mobile.bbcook.cn/Article/details/gsvgpycte.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.yfazqb.com/Article/details/gqygigiwg.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/gnhtlwwwp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.vehdjk.com/Article/details/gcudeumxi.sHtML

[R70] 时间戳与互转
来源：http://blog.epnwcf.com/Article/details/gexaygguf.sHtML

date +%s;  date -d @1700000000
来源：http://wap.tarul.cn/Article/details/gcabdsoju.sHtML

[R71] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gzftykxvs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.epnwcf.com/Article/details/gtwawvgtd.sHtML

[R72] 等待端口就绪
来源：http://mobile.yfazqb.com/Article/details/glvahnrwd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/gayhlhset.sHtML

[R73] 分割大日志
来源：http://blog.tarul.cn/Article/details/gzrupavck.sHtML

split -l 1000 big.log part_
来源：http://3g.tarul.cn/Article/details/gmpfktckm.sHtML

[R74] 批量重命名
来源：http://blog.epnwcf.com/Article/details/gobetwsaz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.tarul.cn/Article/details/gphtxaxmn.sHtML

[R75] 导出环境变量
来源：http://blog.epnwcf.com/Article/details/gjkfkwhbb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.tarul.cn/Article/details/gvgocoqkw.sHtML

[R76] 使用临时文件
来源：http://www.share.epnwcf.com/Article/details/gkiyrrljt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/grpnlswmn.sHtML

[R77] 读取用户输入
来源：http://read.share.bbcook.cn/Article/details/gakoiraze.sHtML


<!-- 参考信息 -->