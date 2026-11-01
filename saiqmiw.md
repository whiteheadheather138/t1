代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.epnwcf.com/Article/details/gmzzygbwv.sHtML

) t WHERE rn = 1;
来源：http://blog.fktsv.cn/Article/details/gbcmtktuw.sHtML

[Q35] 内连接
来源：http://www.m.share.vehdjk.com/Article/details/gnlpspxpo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.yfazqb.com/Article/details/gmmsflbsm.sHtML

[Q36] 左连接
来源：http://www.share.tarul.cn/Article/details/gmkrhdixe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/gsfpimdky.sHtML

[Q37] 右连接
来源：http://m.share.yfazqb.com/Article/details/gqlmxjtdw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.yfazqb.com/Article/details/gfxiysbwe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.tarul.cn/Article/details/gecryelxv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.tarul.cn/Article/details/gcxlvcthu.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.bbcook.cn/Article/details/gsjirkzri.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.bbcook.cn/Article/details/ggyrjudod.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/gbbndevgi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.tarul.cn/Article/details/gektkyqij.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.vehdjk.com/Article/details/gpbqhfjse.sHtML

[Q41] 多表连接
来源：http://mobile.sjlbkw.cn/Article/details/glpaqpfuh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.tarul.cn/Article/details/gweevcmrw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.bbcook.cn/Article/details/gvmnfwfhg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.yfazqb.com/Article/details/gbmtwmgda.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.bbcook.cn/Article/details/gjsfwgymw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.sjlbkw.cn/Article/details/gxetetqhy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.vehdjk.com/Article/details/gejkczfhc.sHtML

[Q43] 标量子查询
来源：http://wap.vehdjk.com/Article/details/gudpyxruh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.vehdjk.com/Article/details/gldidsnnq.sHtML

[Q44] IN 子查询
来源：http://www.share.yfazqb.com/Article/details/gwfbsuqrk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.tarul.cn/Article/details/gdynxxbsf.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.vehdjk.com/Article/details/ggudpbxmn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.epnwcf.com/Article/details/gzxhfgyyd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fktsv.cn/Article/details/gbsofwgdl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/grxroseml.sHtML

[Q47] 与平均值比较
来源：http://read.share.bbcook.cn/Article/details/ghxbwbycf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.bbcook.cn/Article/details/ghhwheslb.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fktsv.cn/Article/details/guhxzjoar.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fktsv.cn/Article/details/gqvopsfjf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fktsv.cn/Article/details/ggsrvxjrl.sHtML

[Q49] 更新单行
来源：http://read.share.tarul.cn/Article/details/gzintxmdv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gqtmckvhf.sHtML

[Q50] 批量更新
来源：http://mobile.fktsv.cn/Article/details/grrnzxlus.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fktsv.cn/Article/details/gouyhkygr.sHtML

[Q51] 用子查询更新
来源：http://www.share.tarul.cn/Article/details/gtdodcrnn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.bbcook.cn/Article/details/gfmpxzbwd.sHtML

[Q52] 删除指定行
来源：http://read.share.epnwcf.com/Article/details/gufhkeerc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gqrqloccq.sHtML

[Q53] 按条件删除
来源：http://www.m.share.vehdjk.com/Article/details/gaqfwadjb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fktsv.cn/Article/details/gragungjx.sHtML

[Q54] 清空表
来源：http://3g.bbcook.cn/Article/details/gzxedqehq.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fktsv.cn/Article/details/gbgutqffb.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.bbcook.cn/Article/details/gkozgzbfu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/guyrognfi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.sjlbkw.cn/Article/details/gftsmvtnj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.tarul.cn/Article/details/gddbpwkqq.sHtML

[Q57] 行号
来源：http://blog.vehdjk.com/Article/details/gdmztgmao.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.bbcook.cn/Article/details/gjcffqaks.sHtML

[Q58] 累计求和
来源：http://read.share.bbcook.cn/Article/details/gcxrkquuh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gnmjpugbn.sHtML

[Q59] 分组内累计
来源：http://blog.tarul.cn/Article/details/gmagcmlqx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gaochumko.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.tarul.cn/Article/details/gqwhwseaa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.bbcook.cn/Article/details/gxcamogst.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gjlijijjf.sHtML

[Q61] 移动平均
来源：http://mobile.bbcook.cn/Article/details/gglvpygnm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/guirqjxcp.sHtML

[Q62] 分组占比
来源：http://www.m.share.fktsv.cn/Article/details/guqmeyzqm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gwtpdagkm.sHtML

[Q63] 开启事务
来源：http://blog.sjlbkw.cn/Article/details/gcsedgech.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.vehdjk.com/Article/details/gnskpqhdj.sHtML

[Q64] 提交事务
来源：http://m.share.sjlbkw.cn/Article/details/gdescaous.sHtML

COMMIT;
来源：http://mobile.yfazqb.com/Article/details/gsydajvgg.sHtML

[Q65] 回滚事务
来源：http://www.blog.vehdjk.com/Article/details/gpziyuihp.sHtML

ROLLBACK;
来源：http://read.share.epnwcf.com/Article/details/gbpkuahnv.sHtML

[Q66] 行锁查询
来源：http://www.share.yfazqb.com/Article/details/gwncvmygr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.epnwcf.com/Article/details/gzaagtlbb.sHtML

[Q67] 设置隔离级别
来源：http://m.share.sjlbkw.cn/Article/details/gspkjyxkc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.tarul.cn/Article/details/gmnyfppld.sHtML

[Q68] 保存点
来源：http://www.share.bbcook.cn/Article/details/glmullykq.sHtML

SAVEPOINT sp1;
来源：http://blog.sjlbkw.cn/Article/details/gaprhsdcu.sHtML

ROLLBACK TO sp1;
来源：http://3g.fktsv.cn/Article/details/gxxlmtozn.sHtML

[Q69] 查看执行计划
来源：http://blog.tarul.cn/Article/details/goqrvocxy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.bbcook.cn/Article/details/gvsguecdg.sHtML

[Q70] 更新统计信息
来源：http://baike.tarul.cn/Article/details/grpjqmbrz.sHtML

ANALYZE TABLE users;
来源：http://blog.epnwcf.com/Article/details/glomlhjvh.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.tarul.cn/Article/details/gyknbgmhd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fktsv.cn/Article/details/gfszbxqgo.sHtML

[Q72] 查看索引
来源：http://wap.epnwcf.com/Article/details/gbjbfnkix.sHtML

SHOW INDEX FROM users;
来源：http://www.share.bbcook.cn/Article/details/gaavywmlb.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/gewwmwnuu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.vehdjk.com/Article/details/gtpmeimtv.sHtML

[Q74] 强制使用索引
来源：http://wap.yfazqb.com/Article/details/gaejrcreg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.tarul.cn/Article/details/gfxfhyzcw.sHtML

[Q75] 日期格式化
来源：http://mobile.epnwcf.com/Article/details/gktnmezjg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.bbcook.cn/Article/details/gqbbcxuun.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.vehdjk.com/Article/details/gjeivcnew.sHtML

[Q76] 按天统计
来源：http://baike.vehdjk.com/Article/details/gootrygjs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.epnwcf.com/Article/details/gzmrotezf.sHtML

[Q77] 时间加减
来源：http://baike.tarul.cn/Article/details/gnhpbgtqy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.bbcook.cn/Article/details/gpgruajtd.sHtML

[Q78] 当前时间
来源：http://mobile.epnwcf.com/Article/details/gnwiyeanq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fktsv.cn/Article/details/guausqpvc.sHtML

[Q79] 字符串拼接
来源：http://baike.bbcook.cn/Article/details/gwqfaezot.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.epnwcf.com/Article/details/gtsymikmn.sHtML

[Q80] 字符串截取
来源：http://wap.vehdjk.com/Article/details/gphtmzsve.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gpqnajmho.sHtML

[Q81] 字符串替换
来源：http://3g.bbcook.cn/Article/details/gyscrbhdl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.bbcook.cn/Article/details/gfivvadmk.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.bbcook.cn/Article/details/gpcnbicuz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/getgonnbf.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gnaetidzw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gtxdtakmz.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gwcrvqvtx.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gopkgrnmc.sHtML

[Q85] 数值取整
来源：http://baike.vehdjk.com/Article/details/gvqzchbgv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.vehdjk.com/Article/details/gherfxpsh.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.tarul.cn/Article/details/gmmhymmti.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.sjlbkw.cn/Article/details/grigqskpo.sHtML

[Q87] JSON 字段做条件
来源：http://3g.tarul.cn/Article/details/gpydyhpjc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.bbcook.cn/Article/details/gkvmyhige.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.epnwcf.com/Article/details/gmmqvfden.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.yfazqb.com/Article/details/giepyliwj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfuzprfe.sHtML

[Q89] 判断表是否存在
来源：http://m.share.yfazqb.com/Article/details/gtsiqxvlz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gshaakvab.sHtML

[Q90] 生成序号列
来源：http://www.share.bbcook.cn/Article/details/gnixkxgnd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/gvdcflmdv.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gccgmvhij.sHtML

R. Bash 专题
来源：http://read.share.epnwcf.com/Article/details/gkoqvkcjo.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjgbpfiyt.sHtML

[R01] shebang 与严格模式
来源：http://wap.sjlbkw.cn/Article/details/gcmumkxmf.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/gbjoadwwf.sHtML

set -euo pipefail
来源：http://read.share.yfazqb.com/Article/details/gzmpakxxi.sHtML

[R02] 变量赋值与使用
来源：http://www.share.bbcook.cn/Article/details/gsgxgusli.sHtML

name="Tom"; echo "$name"
来源：http://baike.epnwcf.com/Article/details/gnyxsxrvk.sHtML

[R03] 只读变量
来源：http://blog.sjlbkw.cn/Article/details/gsrbzzvgs.sHtML

readonly PI=3.14
来源：http://www.blog.fktsv.cn/Article/details/gqnqrgdjz.sHtML

[R04] 位置参数
来源：http://m.share.yfazqb.com/Article/details/gmuzmgrje.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.bbcook.cn/Article/details/gifseaqsv.sHtML

[R05] 参数默认值
来源：http://baike.tarul.cn/Article/details/gwagyrhrd.sHtML

name="${1:-default}"
来源：http://3g.vehdjk.com/Article/details/gipsnxlhw.sHtML

[R06] 判断命令是否存在
来源：http://3g.tarul.cn/Article/details/gdqogzpfs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.sjlbkw.cn/Article/details/gbjwrrxog.sHtML

[R07] if 判断文件
来源：http://blog.epnwcf.com/Article/details/gwljywfuw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.epnwcf.com/Article/details/gnfwtptir.sHtML

[R08] 数值比较
来源：http://m.share.fktsv.cn/Article/details/gqwpqmlmz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.sjlbkw.cn/Article/details/gopzydmyt.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gbzjxzltw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.epnwcf.com/Article/details/gxyenwael.sHtML

[R10] 正则匹配
来源：http://blog.bbcook.cn/Article/details/gdfticnwu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.bbcook.cn/Article/details/gdjvmgnee.sHtML

[R11] case 多分支
来源：http://www.m.share.fktsv.cn/Article/details/glbcethuu.sHtML

case "$1" in
来源：http://m.share.fktsv.cn/Article/details/gmkmfcamj.sHtML

start) echo "启动" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gqdjwqxxl.sHtML

stop)  echo "停止" ;;
来源：http://wap.sjlbkw.cn/Article/details/gvaktdhjz.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.tarul.cn/Article/details/gtjderkdm.sHtML

esac
来源：http://www.m.share.bbcook.cn/Article/details/gyvwotcka.sHtML

[R12] for 遍历文件
来源：http://baike.bbcook.cn/Article/details/guruxevdd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.sjlbkw.cn/Article/details/gmijrbozg.sHtML

[R13] for 计数循环
来源：http://3g.tarul.cn/Article/details/gmfmrxqbe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/gatxxqdaz.sHtML

[R14] C 风格 for
来源：http://blog.vehdjk.com/Article/details/gkmkygusp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.yfazqb.com/Article/details/gqkhlqpfg.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/ggejszhdf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.bbcook.cn/Article/details/gulaklrbt.sHtML

[R16] until 等待条件
来源：http://mobile.sjlbkw.cn/Article/details/gsvvxjnep.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.yfazqb.com/Article/details/gjicanqrg.sHtML

[R17] 数组定义与取值
来源：http://3g.sjlbkw.cn/Article/details/gpwosluki.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fktsv.cn/Article/details/ganhsqedf.sHtML

[R18] 遍历数组
来源：http://www.blog.yfazqb.com/Article/details/gzbexoqds.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.epnwcf.com/Article/details/gfzntmmho.sHtML

[R19] 数组长度
来源：http://www.share.epnwcf.com/Article/details/gyjurtjwt.sHtML

echo "${#arr[@]}"
来源：http://www.share.tarul.cn/Article/details/ggqjzjyyg.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.bbcook.cn/Article/details/ghpdlqvyv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.epnwcf.com/Article/details/gdgopapxh.sHtML

[R21] 字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gncdljhah.sHtML

echo "${#s}"
来源：http://mobile.yfazqb.com/Article/details/gcwauzomf.sHtML

[R22] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gchpsomdo.sHtML

echo "${s:0:5}"
来源：http://www.m.share.yfazqb.com/Article/details/gsvcxhape.sHtML

[R23] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/glzzzqood.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.epnwcf.com/Article/details/gvaaowfcs.sHtML

[R24] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gxyzxbowb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.yfazqb.com/Article/details/gvdhiwmrv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/goimqekuq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.epnwcf.com/Article/details/gimgwukhf.sHtML

[R26] 命令替换
来源：http://blog.tarul.cn/Article/details/gjfpehgmq.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.bbcook.cn/Article/details/gnyjvzoui.sHtML

[R27] 算术展开
来源：http://blog.vehdjk.com/Article/details/gzqrjnqyl.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.sjlbkw.cn/Article/details/gavpjlvmo.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/gfmcrfmwj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/gpiqvudjh.sHtML

[R29] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gipoxykhl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.sjlbkw.cn/Article/details/gwhgrmkpt.sHtML

[R30] 函数返回状态码
来源：http://mobile.sjlbkw.cn/Article/details/gjgqzfcpd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fktsv.cn/Article/details/giyxtmobe.sHtML

[R31] 局部变量
来源：http://blog.yfazqb.com/Article/details/gyqiakftu.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.sjlbkw.cn/Article/details/ghpwecael.sHtML

[R32] 参数个数校验
来源：http://baike.fktsv.cn/Article/details/gdpdtyban.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.tarul.cn/Article/details/gjxmwrxew.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fktsv.cn/Article/details/gcbidftzg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.bbcook.cn/Article/details/ghcmwzzml.sHtML

[R34] 退出时清理
来源：http://baike.bbcook.cn/Article/details/grnxdszmq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/ggsxrzntx.sHtML

[R35] 后台执行并等待
来源：http://3g.epnwcf.com/Article/details/gjxwtzpqe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.bbcook.cn/Article/details/gwzqgtfcz.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/gswpxlumi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.yfazqb.com/Article/details/guendjpeq.sHtML

[R37] 把输出赋给变量
来源：http://3g.yfazqb.com/Article/details/giiykrvpe.sHtML

files=$(ls -1)
来源：http://www.blog.epnwcf.com/Article/details/gedfoxazv.sHtML

[R38] 管道串联
来源：http://wap.vehdjk.com/Article/details/gmkmnfcgl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gbekuygsw.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.epnwcf.com/Article/details/gjmpuvdya.sHtML

cmd > out.log 2>&1
来源：http://m.share.tarul.cn/Article/details/gyagafkun.sHtML

[R40] 追加写日志
来源：http://wap.sjlbkw.cn/Article/details/gvjwqajwi.sHtML

echo "log" >> out.log
来源：http://wap.bbcook.cn/Article/details/gsqivlmkr.sHtML

[R41] 丢弃输出
来源：http://mobile.yfazqb.com/Article/details/gjqgengqv.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.bbcook.cn/Article/details/gyawdwosr.sHtML

[R42] 输入重定向
来源：http://www.share.fktsv.cn/Article/details/gncpybaum.sHtML

wc -l < a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gpgkehcbo.sHtML

[R43] 按名字查找文件
来源：http://blog.yfazqb.com/Article/details/gufedxuxp.sHtML

find . -name "*.log" -type f
来源：http://mobile.vehdjk.com/Article/details/gmhrqfknl.sHtML

[R44] 按修改时间查找
来源：http://m.share.fktsv.cn/Article/details/gufxjpqnm.sHtML

find . -mtime -7 -type f
来源：http://blog.epnwcf.com/Article/details/geqhlaglc.sHtML

[R45] 批量删除
来源：http://3g.bbcook.cn/Article/details/gzyapulyr.sHtML

find . -name "*.tmp" -delete
来源：http://3g.tarul.cn/Article/details/ghhnmyomu.sHtML

[R46] 递归替换文件内容
来源：http://www.share.yfazqb.com/Article/details/ggrijqzyo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/gmvssjgea.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/ggvcmwpga.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.tarul.cn/Article/details/gwgqhwfmk.sHtML

[R48] awk 取指定列
来源：http://www.m.share.bbcook.cn/Article/details/gitresltp.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.epnwcf.com/Article/details/guqstgzfx.sHtML

[R49] awk 带条件
来源：http://blog.sjlbkw.cn/Article/details/gcpcewrpz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.epnwcf.com/Article/details/gkymrkyfd.sHtML

[R50] awk 求和
来源：http://baike.epnwcf.com/Article/details/gnkatemao.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/glhvvmpyf.sHtML

[R51] 排序去重取前几
来源：http://3g.fktsv.cn/Article/details/goezrfsgy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.tarul.cn/Article/details/gioaxgzhd.sHtML

[R52] 统计行数
来源：http://baike.vehdjk.com/Article/details/gxcwuvanl.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/ggpjaxzhx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.vehdjk.com/Article/details/gcipfnwtt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.sjlbkw.cn/Article/details/gxjrglsbp.sHtML

[R54] 比较两个文件
来源：http://wap.sjlbkw.cn/Article/details/gepqtymhv.sHtML

diff a.txt b.txt
来源：http://www.m.share.bbcook.cn/Article/details/grmmqygax.sHtML

[R55] 压缩与解压
来源：http://3g.fktsv.cn/Article/details/gxlalwbtr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.yfazqb.com/Article/details/goklwmsbx.sHtML

[R56] 远程拷贝
来源：http://mobile.fktsv.cn/Article/details/gocbgorgs.sHtML

scp file user@host:/path/
来源：http://m.share.fktsv.cn/Article/details/gcabgqzzx.sHtML

[R57] 远程执行命令
来源：http://www.blog.bbcook.cn/Article/details/gpsujajvm.sHtML

ssh user@host 'uptime'
来源：http://www.blog.epnwcf.com/Article/details/grqnlhpeb.sHtML

[R58] 下载文件
来源：http://www.share.tarul.cn/Article/details/gglwpynot.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.tarul.cn/Article/details/gdmofcttk.sHtML

[R59] 发 POST JSON
来源：http://baike.epnwcf.com/Article/details/gwdyuthvl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.yfazqb.com/Article/details/gyulbkzmz.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gwfzbwhxj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fktsv.cn/Article/details/giqelvjco.sHtML

[R61] 磁盘占用
来源：http://www.m.share.epnwcf.com/Article/details/gekvxxcti.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/gzgvuynud.sHtML

[R62] 找最占空间的文件
来源：http://3g.tarul.cn/Article/details/gvkyiqgos.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.yfazqb.com/Article/details/gjeeihvyb.sHtML

[R63] 内存与进程
来源：http://www.share.epnwcf.com/Article/details/gemoxbiki.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fktsv.cn/Article/details/gqogqrffy.sHtML

[R64] 结束进程
来源：http://www.share.epnwcf.com/Article/details/giaumllsz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/grcabcljp.sHtML

[R65] 查看端口占用
来源：http://mobile.epnwcf.com/Article/details/gtecmsurq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.bbcook.cn/Article/details/gxahkzmgc.sHtML

[R66] 定时任务
来源：http://3g.tarul.cn/Article/details/guntdouqv.sHtML

crontab -e;  crontab -l
来源：http://www.share.fktsv.cn/Article/details/gepkmzwwq.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.tarul.cn/Article/details/gbtrtidua.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/gtrsbnkis.sHtML

[R68] 计算文件校验值
来源：http://baike.yfazqb.com/Article/details/geqeiqyuy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.epnwcf.com/Article/details/gdxkwfaim.sHtML

[R69] 生成随机密码
来源：http://www.blog.bbcook.cn/Article/details/gyvqvrswa.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.bbcook.cn/Article/details/ggnuslgje.sHtML

[R70] 时间戳与互转
来源：http://wap.yfazqb.com/Article/details/gafuzesqz.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.epnwcf.com/Article/details/gwjeompaq.sHtML

[R71] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gffmmmoet.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.tarul.cn/Article/details/gxdwhpkzu.sHtML

[R72] 等待端口就绪
来源：http://wap.epnwcf.com/Article/details/gcxkwtaun.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/gphwoibvb.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/gzufeqwgm.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fktsv.cn/Article/details/grgqjfulr.sHtML

[R74] 批量重命名
来源：http://wap.tarul.cn/Article/details/gvqstbjva.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.yfazqb.com/Article/details/gtbrwcgpd.sHtML

[R75] 导出环境变量
来源：http://baike.sjlbkw.cn/Article/details/gszejkgoq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.tarul.cn/Article/details/gfhnkwvyo.sHtML

[R76] 使用临时文件
来源：http://www.m.share.tarul.cn/Article/details/gjrdyqesv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gxedruppr.sHtML

[R77] 读取用户输入
来源：http://blog.yfazqb.com/Article/details/gusmaypdl.sHtML

read -rp "请输入: " ans
来源：http://m.share.sjlbkw.cn/Article/details/gtraulsbm.sHtML

[R78] 交互式菜单
来源：http://blog.yfazqb.com/Article/details/gmczyrjiv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.epnwcf.com/Article/details/gxiqgdmeq.sHtML

[R79] 解析命令行选项
来源：http://baike.vehdjk.com/Article/details/gxvnffibe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.epnwcf.com/Article/details/gholckqsg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.yfazqb.com/Article/details/gqkvctvrr.sHtML

time ./run.sh
来源：http://blog.bbcook.cn/Article/details/gndgdluxk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxnvresjw.sHtML

S. C / C++ 专题
来源：http://baike.fktsv.cn/Article/details/gywgobpop.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gqogbvpbq.sHtML

[S01] C：Hello World
来源：http://mobile.fktsv.cn/Article/details/gigkwordu.sHtML

#include <stdio.h>
来源：http://wap.vehdjk.com/Article/details/gxmxqbqeb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.bbcook.cn/Article/details/grvozbyuu.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.tarul.cn/Article/details/gvxyrocde.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.sjlbkw.cn/Article/details/gwfnkbhmf.sHtML

[S03] C：读入整数
来源：http://3g.vehdjk.com/Article/details/gxuiqjkzt.sHtML


<!-- 参考信息 -->