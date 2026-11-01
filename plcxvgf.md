代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.tarul.cn/Article/details/gjnenoqgm.sHtML

) t WHERE rn = 1;
来源：http://wap.fktsv.cn/Article/details/gaqqqvaqy.sHtML

[Q35] 内连接
来源：http://3g.epnwcf.com/Article/details/gjrqparnj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzemjubim.sHtML

[Q36] 左连接
来源：http://read.share.tarul.cn/Article/details/gzspqnoep.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gfrapxkle.sHtML

[Q37] 右连接
来源：http://3g.yfazqb.com/Article/details/gwchvkimy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fktsv.cn/Article/details/gfxzveszm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.bbcook.cn/Article/details/gmmvdvwwt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.vehdjk.com/Article/details/gtlvucfjk.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.sjlbkw.cn/Article/details/gyccjqhlu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.vehdjk.com/Article/details/gnlgvlnvk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fktsv.cn/Article/details/gdizlirxc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.yfazqb.com/Article/details/glazqyopk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.tarul.cn/Article/details/gwiblbvaf.sHtML

[Q41] 多表连接
来源：http://m.share.epnwcf.com/Article/details/gbluhrikn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/gtqinjskq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.vehdjk.com/Article/details/gudpopbpk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.sjlbkw.cn/Article/details/goqcspqbn.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.yfazqb.com/Article/details/gntmzluqa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.sjlbkw.cn/Article/details/gedcaftmo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.tarul.cn/Article/details/goiohjhxt.sHtML

[Q43] 标量子查询
来源：http://wap.vehdjk.com/Article/details/gboncdikg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.sjlbkw.cn/Article/details/gskhhtfoo.sHtML

[Q44] IN 子查询
来源：http://wap.bbcook.cn/Article/details/gbxdsdjsj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.yfazqb.com/Article/details/gbfxfmyaz.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fktsv.cn/Article/details/gbhekscvt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gbuxwmfvx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.epnwcf.com/Article/details/glbmkzjdr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gdhqnoztx.sHtML

[Q47] 与平均值比较
来源：http://www.share.sjlbkw.cn/Article/details/ghmugnlyf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.bbcook.cn/Article/details/gekchdrgl.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.sjlbkw.cn/Article/details/gmuvtcbtx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.tarul.cn/Article/details/gbvbjwvss.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.vehdjk.com/Article/details/grwsvymfk.sHtML

[Q49] 更新单行
来源：http://www.share.fktsv.cn/Article/details/gllyotuig.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.tarul.cn/Article/details/goywlmuhb.sHtML

[Q50] 批量更新
来源：http://wap.sjlbkw.cn/Article/details/gxkywjyai.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fktsv.cn/Article/details/gnzilfuni.sHtML

[Q51] 用子查询更新
来源：http://www.share.yfazqb.com/Article/details/gifnobwhi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.sjlbkw.cn/Article/details/gycinwhva.sHtML

[Q52] 删除指定行
来源：http://m.share.tarul.cn/Article/details/glssgpbxf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gbemvebxw.sHtML

[Q53] 按条件删除
来源：http://baike.tarul.cn/Article/details/gljtsmhyl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.epnwcf.com/Article/details/gubquaufx.sHtML

[Q54] 清空表
来源：http://blog.fktsv.cn/Article/details/ggvmrsifa.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.vehdjk.com/Article/details/gcoogpykq.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.tarul.cn/Article/details/gcddchikj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.tarul.cn/Article/details/gzovlvjqv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fktsv.cn/Article/details/gxkdajuog.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gtofuuyfa.sHtML

[Q57] 行号
来源：http://blog.tarul.cn/Article/details/gdeqtsykj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gidyidtoz.sHtML

[Q58] 累计求和
来源：http://www.m.share.yfazqb.com/Article/details/gxppgfasa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gkngvfphu.sHtML

[Q59] 分组内累计
来源：http://read.share.yfazqb.com/Article/details/ggisrrqah.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gukgqekdf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.epnwcf.com/Article/details/gcnjejkzt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.sjlbkw.cn/Article/details/gyfyvsbhw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.tarul.cn/Article/details/gpsqlsoll.sHtML

[Q61] 移动平均
来源：http://wap.yfazqb.com/Article/details/gpmpxaujm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/glgkuqsbz.sHtML

[Q62] 分组占比
来源：http://3g.epnwcf.com/Article/details/gcwerzfvv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/gwlpkmjhs.sHtML

[Q63] 开启事务
来源：http://3g.yfazqb.com/Article/details/ghqjqnugq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.vehdjk.com/Article/details/giaritzki.sHtML

[Q64] 提交事务
来源：http://m.share.fktsv.cn/Article/details/ggmpcjztl.sHtML

COMMIT;
来源：http://www.share.yfazqb.com/Article/details/gzbtozsis.sHtML

[Q65] 回滚事务
来源：http://mobile.epnwcf.com/Article/details/goyarclti.sHtML

ROLLBACK;
来源：http://www.share.sjlbkw.cn/Article/details/glvmradxp.sHtML

[Q66] 行锁查询
来源：http://baike.tarul.cn/Article/details/gdrjbouov.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.yfazqb.com/Article/details/gtqczzubu.sHtML

[Q67] 设置隔离级别
来源：http://blog.sjlbkw.cn/Article/details/gwpuckokx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.yfazqb.com/Article/details/gqiasuyyh.sHtML

[Q68] 保存点
来源：http://baike.fktsv.cn/Article/details/glikwhhot.sHtML

SAVEPOINT sp1;
来源：http://blog.sjlbkw.cn/Article/details/grntzpupp.sHtML

ROLLBACK TO sp1;
来源：http://3g.fktsv.cn/Article/details/gufrdrlpz.sHtML

[Q69] 查看执行计划
来源：http://3g.tarul.cn/Article/details/grcixfrjz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.bbcook.cn/Article/details/gdmgiqzmv.sHtML

[Q70] 更新统计信息
来源：http://mobile.bbcook.cn/Article/details/gwwbyanak.sHtML

ANALYZE TABLE users;
来源：http://wap.yfazqb.com/Article/details/gklhhctgs.sHtML

[Q71] 查看建表语句
来源：http://baike.bbcook.cn/Article/details/goowevdow.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.epnwcf.com/Article/details/gvujzlqfw.sHtML

[Q72] 查看索引
来源：http://www.share.fktsv.cn/Article/details/gaeflinvt.sHtML

SHOW INDEX FROM users;
来源：http://m.share.yfazqb.com/Article/details/gmqocubcp.sHtML

[Q73] 查看表状态
来源：http://baike.tarul.cn/Article/details/gvpsjvdse.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.bbcook.cn/Article/details/gxieuefjr.sHtML

[Q74] 强制使用索引
来源：http://baike.yfazqb.com/Article/details/gjeibaqkl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.epnwcf.com/Article/details/gkgjbnnlp.sHtML

[Q75] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gglaxljqg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.epnwcf.com/Article/details/godidrhee.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.vehdjk.com/Article/details/ggvfgotbb.sHtML

[Q76] 按天统计
来源：http://www.m.share.fktsv.cn/Article/details/gtjdzqwav.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.tarul.cn/Article/details/gmcraijlq.sHtML

[Q77] 时间加减
来源：http://3g.bbcook.cn/Article/details/gnmzisghn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.epnwcf.com/Article/details/guupdppxl.sHtML

[Q78] 当前时间
来源：http://mobile.vehdjk.com/Article/details/gcqpidpwv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.sjlbkw.cn/Article/details/gmxisgqyi.sHtML

[Q79] 字符串拼接
来源：http://blog.vehdjk.com/Article/details/gqhprkbbw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.epnwcf.com/Article/details/gkqvrweoi.sHtML

[Q80] 字符串截取
来源：http://baike.vehdjk.com/Article/details/grfqaayxp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gakvwxgmv.sHtML

[Q81] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gkbtoqbdv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gupxilcaz.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.yfazqb.com/Article/details/gszmlfzov.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gramuyzsd.sHtML

[Q83] 大小写转换
来源：http://3g.vehdjk.com/Article/details/glmqvtxgo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gghhsghsa.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fktsv.cn/Article/details/gikrifscc.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gnivugchm.sHtML

[Q85] 数值取整
来源：http://www.m.share.fktsv.cn/Article/details/gydomnbls.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.yfazqb.com/Article/details/guwavxtzc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fktsv.cn/Article/details/gwsrrqgjr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.bbcook.cn/Article/details/gapkqxhjk.sHtML

[Q87] JSON 字段做条件
来源：http://blog.bbcook.cn/Article/details/gxifgnjgx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.vehdjk.com/Article/details/gufyvqqct.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrkzbawl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.sjlbkw.cn/Article/details/gbrjaowap.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.bbcook.cn/Article/details/gbyiqazjk.sHtML

[Q89] 判断表是否存在
来源：http://wap.tarul.cn/Article/details/gdhurhyxj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.bbcook.cn/Article/details/gqhcgtjzg.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/gnxwwailx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.sjlbkw.cn/Article/details/gtascjzbd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gtjmbagri.sHtML

R. Bash 专题
来源：http://wap.yfazqb.com/Article/details/gynapvxuj.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gjfcfowtk.sHtML

[R01] shebang 与严格模式
来源：http://3g.fktsv.cn/Article/details/glysqhwrr.sHtML

#!/usr/bin/env bash
来源：http://www.blog.tarul.cn/Article/details/gtzwydcew.sHtML

set -euo pipefail
来源：http://m.share.bbcook.cn/Article/details/gvxjgrgjf.sHtML

[R02] 变量赋值与使用
来源：http://3g.vehdjk.com/Article/details/grcghgggx.sHtML

name="Tom"; echo "$name"
来源：http://wap.epnwcf.com/Article/details/gktzfcexi.sHtML

[R03] 只读变量
来源：http://mobile.epnwcf.com/Article/details/gvdjljdlb.sHtML

readonly PI=3.14
来源：http://www.share.epnwcf.com/Article/details/gouhnxunt.sHtML

[R04] 位置参数
来源：http://blog.epnwcf.com/Article/details/gtqnolbam.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.vehdjk.com/Article/details/gnpuubvkc.sHtML

[R05] 参数默认值
来源：http://read.share.vehdjk.com/Article/details/grkxofkrh.sHtML

name="${1:-default}"
来源：http://m.share.tarul.cn/Article/details/gaiijbbbz.sHtML

[R06] 判断命令是否存在
来源：http://read.share.yfazqb.com/Article/details/gcbboaqil.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/googhczyi.sHtML

[R07] if 判断文件
来源：http://m.share.yfazqb.com/Article/details/gxymhcmih.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.bbcook.cn/Article/details/gnawfuoho.sHtML

[R08] 数值比较
来源：http://blog.tarul.cn/Article/details/gwuboujtn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.tarul.cn/Article/details/gnvwmjngv.sHtML

[R09] 字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gumrgsdtr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/gegdlwekp.sHtML

[R10] 正则匹配
来源：http://www.m.share.bbcook.cn/Article/details/gdjgpsedw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.bbcook.cn/Article/details/gtiebkewl.sHtML

[R11] case 多分支
来源：http://wap.vehdjk.com/Article/details/gfaspmabq.sHtML

case "$1" in
来源：http://www.m.share.bbcook.cn/Article/details/gaszjaplr.sHtML

start) echo "启动" ;;
来源：http://www.blog.vehdjk.com/Article/details/gxucvvcji.sHtML

stop)  echo "停止" ;;
来源：http://blog.bbcook.cn/Article/details/gibecgwav.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.bbcook.cn/Article/details/gxtzvimly.sHtML

esac
来源：http://blog.epnwcf.com/Article/details/gxxavhlqw.sHtML

[R12] for 遍历文件
来源：http://wap.vehdjk.com/Article/details/gpmylcuzb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.epnwcf.com/Article/details/gspbmdsps.sHtML

[R13] for 计数循环
来源：http://wap.yfazqb.com/Article/details/gpkyvtsoa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/ghlubpaer.sHtML

[R14] C 风格 for
来源：http://3g.fktsv.cn/Article/details/geayxuopb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/gbttouhwf.sHtML

[R15] while 逐行读文件
来源：http://baike.tarul.cn/Article/details/gaupgqekn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.tarul.cn/Article/details/gfbhdnxzu.sHtML

[R16] until 等待条件
来源：http://www.blog.tarul.cn/Article/details/gjiqmlxjb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gvqpaqaaw.sHtML

[R17] 数组定义与取值
来源：http://read.share.tarul.cn/Article/details/gybyrhwpe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fktsv.cn/Article/details/gipptyekl.sHtML

[R18] 遍历数组
来源：http://mobile.yfazqb.com/Article/details/glrqlamrj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.bbcook.cn/Article/details/gebijpbde.sHtML

[R19] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gptytrhbr.sHtML

echo "${#arr[@]}"
来源：http://m.share.epnwcf.com/Article/details/gzoiptcns.sHtML

[R20] 关联数组（字典）
来源：http://baike.bbcook.cn/Article/details/gptywyupq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.yfazqb.com/Article/details/gepontbva.sHtML

[R21] 字符串长度
来源：http://blog.vehdjk.com/Article/details/gimwdzkzn.sHtML

echo "${#s}"
来源：http://www.share.epnwcf.com/Article/details/gaheqeqtn.sHtML

[R22] 截取子串
来源：http://read.share.yfazqb.com/Article/details/grnmtndiv.sHtML

echo "${s:0:5}"
来源：http://read.share.tarul.cn/Article/details/goagotluy.sHtML

[R23] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gkzhrsylb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.vehdjk.com/Article/details/gvunjawit.sHtML

[R24] 大小写转换
来源：http://3g.epnwcf.com/Article/details/ggqmaupqh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fktsv.cn/Article/details/gxbrsjcyp.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.yfazqb.com/Article/details/gscwnubvs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.bbcook.cn/Article/details/gfickcagw.sHtML

[R26] 命令替换
来源：http://www.share.bbcook.cn/Article/details/guhtnufex.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.yfazqb.com/Article/details/gjjjedyzo.sHtML

[R27] 算术展开
来源：http://www.share.fktsv.cn/Article/details/glpepzild.sHtML

echo $((1 + 2 * 3))
来源：http://3g.bbcook.cn/Article/details/gmggqtzkb.sHtML

[R28] 浮点运算
来源：http://www.m.share.tarul.cn/Article/details/gjartgobn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.bbcook.cn/Article/details/gkmpmwmxr.sHtML

[R29] 定义函数
来源：http://wap.epnwcf.com/Article/details/gsqongjtc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.sjlbkw.cn/Article/details/gtbdgjice.sHtML

[R30] 函数返回状态码
来源：http://www.blog.vehdjk.com/Article/details/gqupzyqnx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.tarul.cn/Article/details/gmwjbaaxq.sHtML

[R31] 局部变量
来源：http://www.blog.yfazqb.com/Article/details/gqcthvywo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/gpbxtcroq.sHtML

[R32] 参数个数校验
来源：http://blog.vehdjk.com/Article/details/grwoxbheu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.yfazqb.com/Article/details/ggvlxznnx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.epnwcf.com/Article/details/gqcbblonf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/glganuhsm.sHtML

[R34] 退出时清理
来源：http://m.share.sjlbkw.cn/Article/details/gcjwgnjwk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gyjzblhsj.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.yfazqb.com/Article/details/gzzjayjcr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.tarul.cn/Article/details/gndlanjyw.sHtML

[R36] 并发执行多个任务
来源：http://mobile.epnwcf.com/Article/details/gadlekgrh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.bbcook.cn/Article/details/gwmzidykm.sHtML

[R37] 把输出赋给变量
来源：http://www.share.vehdjk.com/Article/details/gyzxrrkfb.sHtML

files=$(ls -1)
来源：http://www.blog.epnwcf.com/Article/details/gglbvnwtz.sHtML

[R38] 管道串联
来源：http://baike.epnwcf.com/Article/details/gvdohleus.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.tarul.cn/Article/details/gmiasjwyj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.sjlbkw.cn/Article/details/grkmsdcbg.sHtML

cmd > out.log 2>&1
来源：http://wap.tarul.cn/Article/details/gpgzlihmf.sHtML

[R40] 追加写日志
来源：http://baike.vehdjk.com/Article/details/gwaqiptuq.sHtML

echo "log" >> out.log
来源：http://wap.tarul.cn/Article/details/gnxzyscva.sHtML

[R41] 丢弃输出
来源：http://read.share.sjlbkw.cn/Article/details/gfmdumfrm.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gqhjsdpgh.sHtML

[R42] 输入重定向
来源：http://read.share.yfazqb.com/Article/details/gjxabkmjd.sHtML

wc -l < a.txt
来源：http://www.blog.bbcook.cn/Article/details/gynevussg.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fktsv.cn/Article/details/gyidyzwek.sHtML

find . -name "*.log" -type f
来源：http://mobile.yfazqb.com/Article/details/gtuouoang.sHtML

[R44] 按修改时间查找
来源：http://baike.tarul.cn/Article/details/gvbosldke.sHtML

find . -mtime -7 -type f
来源：http://3g.fktsv.cn/Article/details/gneuayuht.sHtML

[R45] 批量删除
来源：http://mobile.yfazqb.com/Article/details/gonmutcis.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.epnwcf.com/Article/details/grqbcoozw.sHtML

[R46] 递归替换文件内容
来源：http://baike.yfazqb.com/Article/details/gknwrtuub.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.epnwcf.com/Article/details/galrpwjfz.sHtML

[R47] sed 单行替换
来源：http://blog.vehdjk.com/Article/details/grcecjczo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.yfazqb.com/Article/details/gkvuorbmb.sHtML

[R48] awk 取指定列
来源：http://m.share.tarul.cn/Article/details/ggqjxxfhq.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.epnwcf.com/Article/details/gsmcpanfh.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/goudylljl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.vehdjk.com/Article/details/gxiwliuxg.sHtML

[R50] awk 求和
来源：http://wap.bbcook.cn/Article/details/gxduxvgqc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gaghvkwij.sHtML

[R51] 排序去重取前几
来源：http://wap.vehdjk.com/Article/details/ggtsskypw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.vehdjk.com/Article/details/gmiexkjdq.sHtML

[R52] 统计行数
来源：http://3g.vehdjk.com/Article/details/gsltmcuoz.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/grswjousi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.sjlbkw.cn/Article/details/grswlcnvo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fktsv.cn/Article/details/gryjdqohj.sHtML

[R54] 比较两个文件
来源：http://baike.epnwcf.com/Article/details/glrmdinjd.sHtML

diff a.txt b.txt
来源：http://read.share.yfazqb.com/Article/details/grmkpfbma.sHtML

[R55] 压缩与解压
来源：http://baike.epnwcf.com/Article/details/grukzessf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.epnwcf.com/Article/details/gvcugkoib.sHtML

[R56] 远程拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gqtxsjuqn.sHtML

scp file user@host:/path/
来源：http://www.share.fktsv.cn/Article/details/gyljeniih.sHtML

[R57] 远程执行命令
来源：http://m.share.epnwcf.com/Article/details/gfpqbszbe.sHtML

ssh user@host 'uptime'
来源：http://www.share.bbcook.cn/Article/details/gxknkdihx.sHtML

[R58] 下载文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvyuggju.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.tarul.cn/Article/details/gouhncmvs.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gqypgildy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.bbcook.cn/Article/details/gpanxhtnz.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/gczkwsmyk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.bbcook.cn/Article/details/gpognnbab.sHtML

[R61] 磁盘占用
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfbxmzfb.sHtML

df -h;  du -sh *
来源：http://baike.epnwcf.com/Article/details/gpumgljsp.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.epnwcf.com/Article/details/gnrddkzof.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.yfazqb.com/Article/details/gqexbfmsl.sHtML

[R63] 内存与进程
来源：http://m.share.bbcook.cn/Article/details/grqqnqglj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.vehdjk.com/Article/details/gfqyebvmg.sHtML

[R64] 结束进程
来源：http://wap.vehdjk.com/Article/details/gvgiprikv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.yfazqb.com/Article/details/gpezznnwu.sHtML

[R65] 查看端口占用
来源：http://www.blog.sjlbkw.cn/Article/details/gsjvjrmpp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.bbcook.cn/Article/details/gyoyxbmbn.sHtML

[R66] 定时任务
来源：http://baike.yfazqb.com/Article/details/goktiovwt.sHtML

crontab -e;  crontab -l
来源：http://baike.yfazqb.com/Article/details/gamfonayz.sHtML

[R67] 生成随机十六进制串
来源：http://wap.vehdjk.com/Article/details/gnseibhmi.sHtML

openssl rand -hex 16
来源：http://read.share.tarul.cn/Article/details/geylsztbm.sHtML

[R68] 计算文件校验值
来源：http://baike.epnwcf.com/Article/details/gdazchykt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.epnwcf.com/Article/details/gjdgnqhqf.sHtML

[R69] 生成随机密码
来源：http://m.share.sjlbkw.cn/Article/details/gltjsbkkm.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.yfazqb.com/Article/details/gnegppoow.sHtML

[R70] 时间戳与互转
来源：http://blog.bbcook.cn/Article/details/ghznvijyu.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.sjlbkw.cn/Article/details/gkezrwhyk.sHtML

[R71] 日期格式化
来源：http://blog.yfazqb.com/Article/details/grocfdtwa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.sjlbkw.cn/Article/details/gdsrzajlk.sHtML

[R72] 等待端口就绪
来源：http://baike.tarul.cn/Article/details/gzqstuspc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/gullwjffp.sHtML

[R73] 分割大日志
来源：http://www.share.yfazqb.com/Article/details/gblxwimaw.sHtML

split -l 1000 big.log part_
来源：http://read.share.tarul.cn/Article/details/gbhwirtno.sHtML

[R74] 批量重命名
来源：http://baike.epnwcf.com/Article/details/gjpilabio.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.vehdjk.com/Article/details/gzubkxbhb.sHtML

[R75] 导出环境变量
来源：http://mobile.yfazqb.com/Article/details/gqgtpbxsy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.epnwcf.com/Article/details/gtfonkgku.sHtML

[R76] 使用临时文件
来源：http://www.m.share.epnwcf.com/Article/details/gblyfokpv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.vehdjk.com/Article/details/gzopudarv.sHtML

[R77] 读取用户输入
来源：http://read.share.tarul.cn/Article/details/gshhcbnro.sHtML

read -rp "请输入: " ans
来源：http://www.share.vehdjk.com/Article/details/grhronwvz.sHtML

[R78] 交互式菜单
来源：http://wap.tarul.cn/Article/details/goraylxqx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.epnwcf.com/Article/details/gmcbnugyh.sHtML

[R79] 解析命令行选项
来源：http://m.share.yfazqb.com/Article/details/gfzjwhdsb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/giexsuupg.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.yfazqb.com/Article/details/gqsbnqued.sHtML

time ./run.sh
来源：http://www.share.tarul.cn/Article/details/gtedirovp.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gyliqqjsd.sHtML

S. C / C++ 专题
来源：http://m.share.epnwcf.com/Article/details/gdvyqlrpv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjqsjrkkz.sHtML

[S01] C：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gzsamvrum.sHtML

#include <stdio.h>
来源：http://wap.tarul.cn/Article/details/glmtaithe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.sjlbkw.cn/Article/details/gacsdyjue.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.vehdjk.com/Article/details/gkilxktso.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.sjlbkw.cn/Article/details/gwnoooijj.sHtML

[S03] C：读入整数
来源：http://blog.sjlbkw.cn/Article/details/gzxfprrvt.sHtML


<!-- 参考信息 -->