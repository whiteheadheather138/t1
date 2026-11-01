代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gbwpsvkxr.sHtML

[Q30] 分组统计
来源：http://read.share.yfazqb.com/Article/details/ghonrmazc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gfbogsrxq.sHtML

[Q31] 分组后过滤
来源：http://www.share.fktsv.cn/Article/details/gdbloyrqu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.yfazqb.com/Article/details/gdtvooaib.sHtML

[Q32] 分组拼接字符串
来源：http://baike.epnwcf.com/Article/details/giyoyvgpv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gzfrmyjqp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.epnwcf.com/Article/details/gwtjifqfu.sHtML

[Q33] 多列分组
来源：http://www.blog.epnwcf.com/Article/details/gcioislnj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.tarul.cn/Article/details/gkgcivlqx.sHtML

[Q34] 每组取第一条
来源：http://read.share.bbcook.cn/Article/details/gvpujgukn.sHtML

SELECT * FROM (
来源：http://3g.fktsv.cn/Article/details/guhuoygak.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.yfazqb.com/Article/details/gysrhaifv.sHtML

) t WHERE rn = 1;
来源：http://wap.epnwcf.com/Article/details/gauiivhki.sHtML

[Q35] 内连接
来源：http://m.share.yfazqb.com/Article/details/gqrvhncgz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/grerzqrpv.sHtML

[Q36] 左连接
来源：http://blog.epnwcf.com/Article/details/ghpbsfqir.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/gcewcyeis.sHtML

[Q37] 右连接
来源：http://www.share.yfazqb.com/Article/details/gdaxblxib.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.bbcook.cn/Article/details/gvxconobo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.sjlbkw.cn/Article/details/gmnmcxqgv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.epnwcf.com/Article/details/gfqrliwqb.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.bbcook.cn/Article/details/getaksmuj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.bbcook.cn/Article/details/gbxbqfgwo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.bbcook.cn/Article/details/gyhbcqjgc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.tarul.cn/Article/details/gzcinvrsr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fktsv.cn/Article/details/grrcwxppl.sHtML

[Q41] 多表连接
来源：http://www.share.sjlbkw.cn/Article/details/grlxjyvcb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.epnwcf.com/Article/details/gudrcephq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.bbcook.cn/Article/details/gapajxjax.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.yfazqb.com/Article/details/gwebjlyki.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.sjlbkw.cn/Article/details/guzyhddkp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.bbcook.cn/Article/details/gtxiyoglq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fktsv.cn/Article/details/glhxoontp.sHtML

[Q43] 标量子查询
来源：http://baike.fktsv.cn/Article/details/grnryeceh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.yfazqb.com/Article/details/gjewqoizf.sHtML

[Q44] IN 子查询
来源：http://www.m.share.vehdjk.com/Article/details/gzfmjtyac.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.epnwcf.com/Article/details/gclyinrwr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.yfazqb.com/Article/details/gkwedeskg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gogzegbfc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.vehdjk.com/Article/details/gvtywyumb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.vehdjk.com/Article/details/godprjwee.sHtML

[Q47] 与平均值比较
来源：http://www.blog.yfazqb.com/Article/details/gktunpeiw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.vehdjk.com/Article/details/gotafkbpj.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.tarul.cn/Article/details/gpxrnsfeg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.vehdjk.com/Article/details/gvpfxfyii.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.vehdjk.com/Article/details/gmomfelae.sHtML

[Q49] 更新单行
来源：http://read.share.epnwcf.com/Article/details/gqcqrptfd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fktsv.cn/Article/details/grpdebqvk.sHtML

[Q50] 批量更新
来源：http://wap.epnwcf.com/Article/details/gaqwrhcpn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.bbcook.cn/Article/details/gouakkogw.sHtML

[Q51] 用子查询更新
来源：http://wap.vehdjk.com/Article/details/gvbtnnpvp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.tarul.cn/Article/details/gpdrhjgjt.sHtML

[Q52] 删除指定行
来源：http://m.share.fktsv.cn/Article/details/gholkxnor.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gvpltcbuw.sHtML

[Q53] 按条件删除
来源：http://www.share.bbcook.cn/Article/details/gqcriaxcy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gblnxkzev.sHtML

[Q54] 清空表
来源：http://m.share.sjlbkw.cn/Article/details/gvsexgdoh.sHtML

TRUNCATE TABLE logs;
来源：http://blog.vehdjk.com/Article/details/gbutobyrx.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.tarul.cn/Article/details/gsyfnamqt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gfhhqsqbt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fktsv.cn/Article/details/gmhpnwdnk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gtrcuymuq.sHtML

[Q57] 行号
来源：http://read.share.tarul.cn/Article/details/godhurvmv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.bbcook.cn/Article/details/gtrkwqscj.sHtML

[Q58] 累计求和
来源：http://mobile.fktsv.cn/Article/details/giwasmwuu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.vehdjk.com/Article/details/gmtxigbmt.sHtML

[Q59] 分组内累计
来源：http://read.share.tarul.cn/Article/details/guopwzior.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gjqjupbad.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.sjlbkw.cn/Article/details/gnjerbucm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fktsv.cn/Article/details/gherhnkdm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.yfazqb.com/Article/details/gvclxowzu.sHtML

[Q61] 移动平均
来源：http://m.share.tarul.cn/Article/details/gprjqwjjv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.tarul.cn/Article/details/ghgaxcely.sHtML

[Q62] 分组占比
来源：http://3g.bbcook.cn/Article/details/gstebjtqo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/giqepcaol.sHtML

[Q63] 开启事务
来源：http://baike.vehdjk.com/Article/details/gkkpqeexx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fktsv.cn/Article/details/gwzpdrwum.sHtML

[Q64] 提交事务
来源：http://mobile.yfazqb.com/Article/details/gpnqjghro.sHtML

COMMIT;
来源：http://mobile.tarul.cn/Article/details/gyuzrppfe.sHtML

[Q65] 回滚事务
来源：http://baike.bbcook.cn/Article/details/grrvpjkxr.sHtML

ROLLBACK;
来源：http://www.m.share.yfazqb.com/Article/details/gavvnrect.sHtML

[Q66] 行锁查询
来源：http://baike.bbcook.cn/Article/details/grxyprrgy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.tarul.cn/Article/details/gmqlxyhsl.sHtML

[Q67] 设置隔离级别
来源：http://wap.epnwcf.com/Article/details/gimvbulep.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.yfazqb.com/Article/details/gchpjokch.sHtML

[Q68] 保存点
来源：http://www.share.bbcook.cn/Article/details/ggrzjfgcq.sHtML

SAVEPOINT sp1;
来源：http://www.share.sjlbkw.cn/Article/details/gpeswryrg.sHtML

ROLLBACK TO sp1;
来源：http://read.share.vehdjk.com/Article/details/giezoosue.sHtML

[Q69] 查看执行计划
来源：http://mobile.vehdjk.com/Article/details/goujgilui.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.epnwcf.com/Article/details/garkibnxg.sHtML

[Q70] 更新统计信息
来源：http://mobile.yfazqb.com/Article/details/gqpiulnhg.sHtML

ANALYZE TABLE users;
来源：http://www.share.tarul.cn/Article/details/giqmcxmrj.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.yfazqb.com/Article/details/gmqbkppwo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fktsv.cn/Article/details/gyogyvqww.sHtML

[Q72] 查看索引
来源：http://3g.fktsv.cn/Article/details/gklikozyy.sHtML

SHOW INDEX FROM users;
来源：http://3g.epnwcf.com/Article/details/gyopxioqf.sHtML

[Q73] 查看表状态
来源：http://www.share.fktsv.cn/Article/details/guejtvbeo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.sjlbkw.cn/Article/details/ggandqyos.sHtML

[Q74] 强制使用索引
来源：http://m.share.tarul.cn/Article/details/gbqeyppmg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.yfazqb.com/Article/details/grnxjeuov.sHtML

[Q75] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gveqbmcxq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.epnwcf.com/Article/details/gtcjzxffu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.yfazqb.com/Article/details/guxlzoiga.sHtML

[Q76] 按天统计
来源：http://www.share.fktsv.cn/Article/details/gpxwyfojt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.yfazqb.com/Article/details/gpxlxcnnb.sHtML

[Q77] 时间加减
来源：http://mobile.tarul.cn/Article/details/ghabfulgc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.epnwcf.com/Article/details/gjajpbtkc.sHtML

[Q78] 当前时间
来源：http://www.blog.fktsv.cn/Article/details/gelfyjumw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.bbcook.cn/Article/details/gokbqnkpk.sHtML

[Q79] 字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gmytaflsf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.epnwcf.com/Article/details/gczbvhkan.sHtML

[Q80] 字符串截取
来源：http://www.share.fktsv.cn/Article/details/gnzdxvggr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.epnwcf.com/Article/details/gvcqysnhx.sHtML

[Q81] 字符串替换
来源：http://mobile.tarul.cn/Article/details/gomgdmgfl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gesebvxat.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.sjlbkw.cn/Article/details/gnjrjjihy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gefyrcsxu.sHtML

[Q83] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gqvuythnb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gguteyouh.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fktsv.cn/Article/details/guvtggqkf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gvywpbbkv.sHtML

[Q85] 数值取整
来源：http://wap.sjlbkw.cn/Article/details/gayzubblc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.bbcook.cn/Article/details/gminmimyn.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fktsv.cn/Article/details/gguiwpogc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.bbcook.cn/Article/details/gyqknvtwo.sHtML

[Q87] JSON 字段做条件
来源：http://3g.tarul.cn/Article/details/gujsgdtjd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.tarul.cn/Article/details/gjurhhzof.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.epnwcf.com/Article/details/grzsqheyh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.bbcook.cn/Article/details/gnohatvlj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.bbcook.cn/Article/details/gghfrbgio.sHtML

[Q89] 判断表是否存在
来源：http://www.share.vehdjk.com/Article/details/gbcuarvsd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.epnwcf.com/Article/details/greuqzmbi.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/gcbmymfea.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.vehdjk.com/Article/details/gzwwdwroe.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ggzrcdgai.sHtML

R. Bash 专题
来源：http://read.share.yfazqb.com/Article/details/gfdrgjntz.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvfjyficn.sHtML

[R01] shebang 与严格模式
来源：http://blog.tarul.cn/Article/details/gwgjgynzz.sHtML

#!/usr/bin/env bash
来源：http://www.blog.vehdjk.com/Article/details/goauibwfy.sHtML

set -euo pipefail
来源：http://baike.fktsv.cn/Article/details/ggsuhdlgq.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fktsv.cn/Article/details/gpinykblw.sHtML

name="Tom"; echo "$name"
来源：http://3g.yfazqb.com/Article/details/gzhvomzfg.sHtML

[R03] 只读变量
来源：http://read.share.sjlbkw.cn/Article/details/gkfsjnbvs.sHtML

readonly PI=3.14
来源：http://read.share.vehdjk.com/Article/details/gemquawnt.sHtML

[R04] 位置参数
来源：http://wap.sjlbkw.cn/Article/details/gebimrvyv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.sjlbkw.cn/Article/details/gcdxjendg.sHtML

[R05] 参数默认值
来源：http://baike.epnwcf.com/Article/details/gkusudujq.sHtML

name="${1:-default}"
来源：http://wap.sjlbkw.cn/Article/details/glhswefbc.sHtML

[R06] 判断命令是否存在
来源：http://m.share.yfazqb.com/Article/details/gobkdrzbb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/gszerhabp.sHtML

[R07] if 判断文件
来源：http://blog.tarul.cn/Article/details/gebypkwjj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.epnwcf.com/Article/details/gryvnrume.sHtML

[R08] 数值比较
来源：http://mobile.fktsv.cn/Article/details/ggwutkaqp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.vehdjk.com/Article/details/gvkosifld.sHtML

[R09] 字符串比较
来源：http://baike.vehdjk.com/Article/details/gvajcsiyx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fktsv.cn/Article/details/grffdwuvf.sHtML

[R10] 正则匹配
来源：http://www.share.tarul.cn/Article/details/gpspaitno.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.epnwcf.com/Article/details/gefhiwzgm.sHtML

[R11] case 多分支
来源：http://baike.vehdjk.com/Article/details/gpojucbrz.sHtML

case "$1" in
来源：http://www.blog.sjlbkw.cn/Article/details/geabkamzr.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/giembuvyy.sHtML

stop)  echo "停止" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gmpaedwnw.sHtML

*)     echo "未知命令" ;;
来源：http://3g.tarul.cn/Article/details/gtplzydsb.sHtML

esac
来源：http://www.share.bbcook.cn/Article/details/gaglwjclb.sHtML

[R12] for 遍历文件
来源：http://m.share.vehdjk.com/Article/details/ghycbwmco.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.epnwcf.com/Article/details/gykozsmza.sHtML

[R13] for 计数循环
来源：http://read.share.yfazqb.com/Article/details/gttnyrckg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/glpwsomhj.sHtML

[R14] C 风格 for
来源：http://m.share.vehdjk.com/Article/details/glcfdgvit.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gofkiyltr.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gffhzmduh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.epnwcf.com/Article/details/gfhrtnhsa.sHtML

[R16] until 等待条件
来源：http://blog.tarul.cn/Article/details/gvihtaure.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gpuqsagdz.sHtML

[R17] 数组定义与取值
来源：http://m.share.epnwcf.com/Article/details/gtikecsrg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.tarul.cn/Article/details/gsblpelej.sHtML

[R18] 遍历数组
来源：http://mobile.tarul.cn/Article/details/gdizjyxui.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fktsv.cn/Article/details/gzxcepobp.sHtML

[R19] 数组长度
来源：http://wap.yfazqb.com/Article/details/gpmbhvbew.sHtML

echo "${#arr[@]}"
来源：http://read.share.vehdjk.com/Article/details/gfcpztplt.sHtML

[R20] 关联数组（字典）
来源：http://baike.sjlbkw.cn/Article/details/ghlgjxhdj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.sjlbkw.cn/Article/details/gpwhyzioi.sHtML

[R21] 字符串长度
来源：http://3g.vehdjk.com/Article/details/gzpifwcnx.sHtML

echo "${#s}"
来源：http://www.share.sjlbkw.cn/Article/details/gsxazvgou.sHtML

[R22] 截取子串
来源：http://blog.tarul.cn/Article/details/gwvylfbfk.sHtML

echo "${s:0:5}"
来源：http://blog.epnwcf.com/Article/details/gtxcysoey.sHtML

[R23] 字符串替换
来源：http://baike.bbcook.cn/Article/details/gfxsogqxd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.bbcook.cn/Article/details/gukdkchts.sHtML

[R24] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gypysnznj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.sjlbkw.cn/Article/details/gaxoygjyx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.sjlbkw.cn/Article/details/gqbxgnzjh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.yfazqb.com/Article/details/giwhotlht.sHtML

[R26] 命令替换
来源：http://baike.bbcook.cn/Article/details/gkanlncvn.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fktsv.cn/Article/details/gbfqtzabc.sHtML

[R27] 算术展开
来源：http://www.share.vehdjk.com/Article/details/glwemuubu.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.tarul.cn/Article/details/ghgmqegzp.sHtML

[R28] 浮点运算
来源：http://wap.yfazqb.com/Article/details/gppzlvytu.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.vehdjk.com/Article/details/geaporcwe.sHtML

[R29] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gdjituhzz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fktsv.cn/Article/details/glxnrrsvy.sHtML

[R30] 函数返回状态码
来源：http://blog.epnwcf.com/Article/details/gmuojlqgz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.yfazqb.com/Article/details/goaegfgmb.sHtML

[R31] 局部变量
来源：http://m.share.tarul.cn/Article/details/gsvbnovsd.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.epnwcf.com/Article/details/gegythywh.sHtML

[R32] 参数个数校验
来源：http://read.share.bbcook.cn/Article/details/gcnufsgnr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gzwhgeuza.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.epnwcf.com/Article/details/gjnmpkzta.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.sjlbkw.cn/Article/details/gtrqatxiy.sHtML

[R34] 退出时清理
来源：http://www.m.share.fktsv.cn/Article/details/guffwpsay.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gnmtalymu.sHtML

[R35] 后台执行并等待
来源：http://blog.bbcook.cn/Article/details/gytybbwch.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.epnwcf.com/Article/details/gfnmljouw.sHtML

[R36] 并发执行多个任务
来源：http://wap.yfazqb.com/Article/details/gwdvtmhdn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.yfazqb.com/Article/details/gyldcvpqk.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fktsv.cn/Article/details/gxktjgpzn.sHtML

files=$(ls -1)
来源：http://www.blog.yfazqb.com/Article/details/gnjmfwqjj.sHtML

[R38] 管道串联
来源：http://www.blog.fktsv.cn/Article/details/gpifffpbd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.sjlbkw.cn/Article/details/gmfgevsyf.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.epnwcf.com/Article/details/gfibjevuw.sHtML

cmd > out.log 2>&1
来源：http://3g.sjlbkw.cn/Article/details/getnmpjno.sHtML

[R40] 追加写日志
来源：http://wap.epnwcf.com/Article/details/gqazopwzs.sHtML

echo "log" >> out.log
来源：http://read.share.fktsv.cn/Article/details/gagnqxhck.sHtML

[R41] 丢弃输出
来源：http://read.share.fktsv.cn/Article/details/gosusfbpl.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.vehdjk.com/Article/details/gjssqgvij.sHtML

[R42] 输入重定向
来源：http://3g.yfazqb.com/Article/details/gqszbvgee.sHtML

wc -l < a.txt
来源：http://wap.tarul.cn/Article/details/gbjxkfidw.sHtML

[R43] 按名字查找文件
来源：http://3g.epnwcf.com/Article/details/guyqnlhex.sHtML

find . -name "*.log" -type f
来源：http://mobile.tarul.cn/Article/details/gekynjfyf.sHtML

[R44] 按修改时间查找
来源：http://www.blog.vehdjk.com/Article/details/gebivedmo.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.vehdjk.com/Article/details/gnklohkie.sHtML

[R45] 批量删除
来源：http://wap.vehdjk.com/Article/details/gjncrlfdf.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gvonqlkge.sHtML

[R46] 递归替换文件内容
来源：http://3g.tarul.cn/Article/details/gknrbmosb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.sjlbkw.cn/Article/details/gpydedfem.sHtML

[R47] sed 单行替换
来源：http://www.m.share.tarul.cn/Article/details/gemvbldkd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/ghmhguurb.sHtML

[R48] awk 取指定列
来源：http://www.share.tarul.cn/Article/details/gaxjmvbmb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqohboya.sHtML

[R49] awk 带条件
来源：http://mobile.yfazqb.com/Article/details/gvlstwjwy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.epnwcf.com/Article/details/gzohugtvs.sHtML

[R50] awk 求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gadtdqchq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.epnwcf.com/Article/details/gsnezsvfh.sHtML

[R51] 排序去重取前几
来源：http://baike.bbcook.cn/Article/details/gmpzrtztl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.bbcook.cn/Article/details/glehvlekc.sHtML

[R52] 统计行数
来源：http://wap.vehdjk.com/Article/details/gdlkcrqzx.sHtML

wc -l a.txt
来源：http://baike.yfazqb.com/Article/details/gdkqlvgbu.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.vehdjk.com/Article/details/gochjubnf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.vehdjk.com/Article/details/gfrhwosqs.sHtML

[R54] 比较两个文件
来源：http://m.share.epnwcf.com/Article/details/gukpbwnsh.sHtML

diff a.txt b.txt
来源：http://www.blog.tarul.cn/Article/details/gcqfptsuw.sHtML

[R55] 压缩与解压
来源：http://m.share.epnwcf.com/Article/details/gtyfiiprl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.tarul.cn/Article/details/gyrggtmco.sHtML

[R56] 远程拷贝
来源：http://baike.tarul.cn/Article/details/gldauuyzq.sHtML

scp file user@host:/path/
来源：http://m.share.fktsv.cn/Article/details/gntngjtuk.sHtML

[R57] 远程执行命令
来源：http://m.share.epnwcf.com/Article/details/gnsfitnsf.sHtML

ssh user@host 'uptime'
来源：http://blog.yfazqb.com/Article/details/gwfswpsyi.sHtML

[R58] 下载文件
来源：http://www.share.vehdjk.com/Article/details/gkjvvzusr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/gobplutyl.sHtML

[R59] 发 POST JSON
来源：http://wap.vehdjk.com/Article/details/gklqixpgz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.yfazqb.com/Article/details/guzbaqzzm.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/grhazpobe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.yfazqb.com/Article/details/ggjenrqso.sHtML

[R61] 磁盘占用
来源：http://read.share.yfazqb.com/Article/details/gboaiuunl.sHtML

df -h;  du -sh *
来源：http://blog.vehdjk.com/Article/details/gxyztxlxv.sHtML

[R62] 找最占空间的文件
来源：http://baike.tarul.cn/Article/details/gcddknpfx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.sjlbkw.cn/Article/details/gfabjebgm.sHtML

[R63] 内存与进程
来源：http://m.share.fktsv.cn/Article/details/gbsdbvdwu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.vehdjk.com/Article/details/gbuhckprr.sHtML

[R64] 结束进程
来源：http://www.blog.bbcook.cn/Article/details/gcawgfkpp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.tarul.cn/Article/details/gogpdoerj.sHtML

[R65] 查看端口占用
来源：http://wap.epnwcf.com/Article/details/gqhwadmvn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.epnwcf.com/Article/details/ggsjilakt.sHtML

[R66] 定时任务
来源：http://m.share.yfazqb.com/Article/details/gntjavfge.sHtML

crontab -e;  crontab -l
来源：http://read.share.fktsv.cn/Article/details/gmfwqpvyf.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.vehdjk.com/Article/details/gvdvgdgtt.sHtML

openssl rand -hex 16
来源：http://blog.sjlbkw.cn/Article/details/gslmpimxm.sHtML

[R68] 计算文件校验值
来源：http://baike.yfazqb.com/Article/details/grftdqkux.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.epnwcf.com/Article/details/gqmkombgh.sHtML

[R69] 生成随机密码
来源：http://m.share.epnwcf.com/Article/details/gtwwwrblw.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.vehdjk.com/Article/details/gjgkrazmd.sHtML

[R70] 时间戳与互转
来源：http://www.blog.bbcook.cn/Article/details/gjgndyatb.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.bbcook.cn/Article/details/glxxdygql.sHtML

[R71] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gdfhcupuz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.yfazqb.com/Article/details/gqznogboh.sHtML

[R72] 等待端口就绪
来源：http://3g.tarul.cn/Article/details/gvpgqefjr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/gmaapschv.sHtML

[R73] 分割大日志
来源：http://mobile.fktsv.cn/Article/details/gvdtbpqqd.sHtML

split -l 1000 big.log part_
来源：http://www.share.epnwcf.com/Article/details/ggcbtyumo.sHtML

[R74] 批量重命名
来源：http://blog.sjlbkw.cn/Article/details/gibanyfke.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.tarul.cn/Article/details/gkdnrhjst.sHtML

[R75] 导出环境变量
来源：http://baike.fktsv.cn/Article/details/gjdpdzurw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.epnwcf.com/Article/details/ghjqrysss.sHtML

[R76] 使用临时文件
来源：http://wap.vehdjk.com/Article/details/glkuqujtg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gzfbwmzdp.sHtML

[R77] 读取用户输入
来源：http://m.share.fktsv.cn/Article/details/giddmpdow.sHtML

read -rp "请输入: " ans
来源：http://mobile.yfazqb.com/Article/details/gdofikzvr.sHtML

[R78] 交互式菜单
来源：http://www.share.epnwcf.com/Article/details/gxpxuevoe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/gieqbmled.sHtML

[R79] 解析命令行选项
来源：http://wap.sjlbkw.cn/Article/details/ghlfdgobo.sHtML


<!-- 参考信息 -->