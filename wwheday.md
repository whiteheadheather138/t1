代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.tarul.cn/Article/details/gsehfrzip.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.yfazqb.com/Article/details/gbxmactma.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.epnwcf.com/Article/details/gufbzedfh.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.tarul.cn/Article/details/gutwljjwd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.yfazqb.com/Article/details/gmeoxaezi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.vehdjk.com/Article/details/guziysesy.sHtML

[Q43] 标量子查询
来源：http://www.blog.fktsv.cn/Article/details/gvozwrqsy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.tarul.cn/Article/details/gwfivuqff.sHtML

[Q44] IN 子查询
来源：http://www.blog.sjlbkw.cn/Article/details/gquzcmszs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.epnwcf.com/Article/details/gutovvcgx.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.vehdjk.com/Article/details/goxbtxivf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/ghtnfpixh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.vehdjk.com/Article/details/gzqpemmsj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/gpbekbyql.sHtML

[Q47] 与平均值比较
来源：http://read.share.sjlbkw.cn/Article/details/gtizpmbnl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.vehdjk.com/Article/details/glyamtcwu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.vehdjk.com/Article/details/genqhjhna.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.sjlbkw.cn/Article/details/gdkauaxzw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.epnwcf.com/Article/details/gmxnvvotv.sHtML

[Q49] 更新单行
来源：http://blog.yfazqb.com/Article/details/gidiwzakx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/gagxiggoe.sHtML

[Q50] 批量更新
来源：http://m.share.tarul.cn/Article/details/gvhvvixhv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gvbkhutwr.sHtML

[Q51] 用子查询更新
来源：http://www.share.vehdjk.com/Article/details/gybpsikon.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.sjlbkw.cn/Article/details/gemqwfkjk.sHtML

[Q52] 删除指定行
来源：http://baike.tarul.cn/Article/details/ggkatxcvv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.yfazqb.com/Article/details/gfjwzevsr.sHtML

[Q53] 按条件删除
来源：http://www.share.yfazqb.com/Article/details/gewfbujid.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.yfazqb.com/Article/details/gsouoyxka.sHtML

[Q54] 清空表
来源：http://www.m.share.fktsv.cn/Article/details/gjbelfukn.sHtML

TRUNCATE TABLE logs;
来源：http://baike.vehdjk.com/Article/details/gzjazlcwm.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fktsv.cn/Article/details/gldmloeap.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gveyscspx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fktsv.cn/Article/details/giuoomats.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/giqcrkzxh.sHtML

[Q57] 行号
来源：http://baike.fktsv.cn/Article/details/gsjfcbwpa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/ghkhrqibh.sHtML

[Q58] 累计求和
来源：http://www.m.share.tarul.cn/Article/details/gchyygmrz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gamjxbrfe.sHtML

[Q59] 分组内累计
来源：http://read.share.epnwcf.com/Article/details/gmpkvhbpx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.tarul.cn/Article/details/gghjeduak.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.tarul.cn/Article/details/gsbnkmsot.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/ghxmlmcwh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gzwsusyrw.sHtML

[Q61] 移动平均
来源：http://www.blog.tarul.cn/Article/details/gkakxmsuf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gsaeqhqzb.sHtML

[Q62] 分组占比
来源：http://www.blog.vehdjk.com/Article/details/grjpfqccg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gmtereiwr.sHtML

[Q63] 开启事务
来源：http://read.share.fktsv.cn/Article/details/goffslhgd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.tarul.cn/Article/details/gkmvyikfr.sHtML

[Q64] 提交事务
来源：http://baike.fktsv.cn/Article/details/grpsstwnl.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/gkzpmndkv.sHtML

[Q65] 回滚事务
来源：http://www.blog.bbcook.cn/Article/details/giwubtfpf.sHtML

ROLLBACK;
来源：http://read.share.vehdjk.com/Article/details/gwlomysev.sHtML

[Q66] 行锁查询
来源：http://baike.tarul.cn/Article/details/godqbpnxd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.bbcook.cn/Article/details/gfynkqjbe.sHtML

[Q67] 设置隔离级别
来源：http://wap.sjlbkw.cn/Article/details/grnudbcsu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fktsv.cn/Article/details/giggzsvcy.sHtML

[Q68] 保存点
来源：http://m.share.sjlbkw.cn/Article/details/gbuzhehew.sHtML

SAVEPOINT sp1;
来源：http://m.share.yfazqb.com/Article/details/gmpozdavm.sHtML

ROLLBACK TO sp1;
来源：http://www.share.epnwcf.com/Article/details/gxscccvsh.sHtML

[Q69] 查看执行计划
来源：http://read.share.yfazqb.com/Article/details/gwcflvuon.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.sjlbkw.cn/Article/details/gmqruluqh.sHtML

[Q70] 更新统计信息
来源：http://www.blog.epnwcf.com/Article/details/gijgtuwru.sHtML

ANALYZE TABLE users;
来源：http://baike.yfazqb.com/Article/details/gdqqqhgcs.sHtML

[Q71] 查看建表语句
来源：http://baike.tarul.cn/Article/details/gebhvural.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fktsv.cn/Article/details/gulqasuqx.sHtML

[Q72] 查看索引
来源：http://mobile.bbcook.cn/Article/details/gzmnozsbf.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gwhsxswqx.sHtML

[Q73] 查看表状态
来源：http://mobile.bbcook.cn/Article/details/gchafdbdx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.epnwcf.com/Article/details/gxkyjlvby.sHtML

[Q74] 强制使用索引
来源：http://wap.tarul.cn/Article/details/gmipyanui.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.tarul.cn/Article/details/gdkdvggqy.sHtML

[Q75] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/ghwvzxobl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gorgukrum.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.tarul.cn/Article/details/gwisubqso.sHtML

[Q76] 按天统计
来源：http://blog.tarul.cn/Article/details/gawkudzwc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/gnjltfnlw.sHtML

[Q77] 时间加减
来源：http://www.m.share.yfazqb.com/Article/details/guwguwxxd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fktsv.cn/Article/details/gsbzjbaww.sHtML

[Q78] 当前时间
来源：http://blog.yfazqb.com/Article/details/gtrgdnbji.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.yfazqb.com/Article/details/ginsbiiea.sHtML

[Q79] 字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/ggxptchuh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.tarul.cn/Article/details/gozctzwrf.sHtML

[Q80] 字符串截取
来源：http://wap.fktsv.cn/Article/details/gyhupblif.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gccmfqwdw.sHtML

[Q81] 字符串替换
来源：http://wap.tarul.cn/Article/details/gsrhnmsyp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.vehdjk.com/Article/details/gwiopngyh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.tarul.cn/Article/details/gwacysxnh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gretwiopa.sHtML

[Q83] 大小写转换
来源：http://m.share.tarul.cn/Article/details/gaiobsyky.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gtkryqblv.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.sjlbkw.cn/Article/details/ghsiyzxct.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gcefosglz.sHtML

[Q85] 数值取整
来源：http://www.share.sjlbkw.cn/Article/details/geqatntpr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.vehdjk.com/Article/details/gbfpsnwbh.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.yfazqb.com/Article/details/gkzmraoeq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.tarul.cn/Article/details/gybnumcmv.sHtML

[Q87] JSON 字段做条件
来源：http://3g.yfazqb.com/Article/details/gmpgptdke.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.epnwcf.com/Article/details/gtbdfxeld.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.sjlbkw.cn/Article/details/grswxzuvo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.vehdjk.com/Article/details/gawfukxkz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.yfazqb.com/Article/details/gecqknjjg.sHtML

[Q89] 判断表是否存在
来源：http://www.share.tarul.cn/Article/details/gqeqgbkmr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.bbcook.cn/Article/details/gpvjbawmr.sHtML

[Q90] 生成序号列
来源：http://baike.yfazqb.com/Article/details/gyztygkba.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.bbcook.cn/Article/details/guwlbwqfo.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gihyrilom.sHtML

R. Bash 专题
来源：http://3g.yfazqb.com/Article/details/gausimger.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxndeomee.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.vehdjk.com/Article/details/gfjiitpha.sHtML

#!/usr/bin/env bash
来源：http://wap.bbcook.cn/Article/details/gudjdltza.sHtML

set -euo pipefail
来源：http://www.blog.sjlbkw.cn/Article/details/gmhogihiz.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.vehdjk.com/Article/details/gvtzpdyxi.sHtML

name="Tom"; echo "$name"
来源：http://mobile.bbcook.cn/Article/details/glfgqewdd.sHtML

[R03] 只读变量
来源：http://www.blog.fktsv.cn/Article/details/gpekpqmrt.sHtML

readonly PI=3.14
来源：http://wap.bbcook.cn/Article/details/gikoxhvmq.sHtML

[R04] 位置参数
来源：http://m.share.bbcook.cn/Article/details/ghfwxpfpj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.vehdjk.com/Article/details/gfgkjkogk.sHtML

[R05] 参数默认值
来源：http://baike.fktsv.cn/Article/details/gxfnovaaw.sHtML

name="${1:-default}"
来源：http://www.blog.yfazqb.com/Article/details/gknxdjtph.sHtML

[R06] 判断命令是否存在
来源：http://3g.vehdjk.com/Article/details/gdocnaetv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.sjlbkw.cn/Article/details/gpqkgihgx.sHtML

[R07] if 判断文件
来源：http://baike.vehdjk.com/Article/details/gxouluddb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.yfazqb.com/Article/details/gauqivslu.sHtML

[R08] 数值比较
来源：http://www.m.share.bbcook.cn/Article/details/gfpmzaatn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.sjlbkw.cn/Article/details/gyftamgcr.sHtML

[R09] 字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gsbenondx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fktsv.cn/Article/details/gjgvergoh.sHtML

[R10] 正则匹配
来源：http://read.share.sjlbkw.cn/Article/details/gonijzymn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.vehdjk.com/Article/details/gkceuyzwy.sHtML

[R11] case 多分支
来源：http://www.share.epnwcf.com/Article/details/gkeetxsnm.sHtML

case "$1" in
来源：http://www.blog.fktsv.cn/Article/details/gpdbxzmgi.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/gbsshievj.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fktsv.cn/Article/details/guxlcnbau.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gfzdlakni.sHtML

esac
来源：http://www.blog.bbcook.cn/Article/details/gverizunx.sHtML

[R12] for 遍历文件
来源：http://blog.vehdjk.com/Article/details/gclslgrmr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.bbcook.cn/Article/details/gkizwlpjd.sHtML

[R13] for 计数循环
来源：http://www.blog.tarul.cn/Article/details/gsuybnzfn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/grmdzfvay.sHtML

[R14] C 风格 for
来源：http://m.share.yfazqb.com/Article/details/glfxfjing.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gluaehnyx.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gjnlhdpzv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.tarul.cn/Article/details/ggchzgaba.sHtML

[R16] until 等待条件
来源：http://www.m.share.fktsv.cn/Article/details/gdjrgcldg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gbtnefpcz.sHtML

[R17] 数组定义与取值
来源：http://m.share.bbcook.cn/Article/details/gbztlfmaw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.bbcook.cn/Article/details/grgqqovbg.sHtML

[R18] 遍历数组
来源：http://blog.epnwcf.com/Article/details/glgqqqfea.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.epnwcf.com/Article/details/gmovhsize.sHtML

[R19] 数组长度
来源：http://m.share.tarul.cn/Article/details/getqqgjxv.sHtML

echo "${#arr[@]}"
来源：http://3g.yfazqb.com/Article/details/guewxgqsk.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.epnwcf.com/Article/details/gokppccap.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/gguqdyfka.sHtML

[R21] 字符串长度
来源：http://wap.bbcook.cn/Article/details/gftnfwprj.sHtML

echo "${#s}"
来源：http://read.share.vehdjk.com/Article/details/gnuidtopv.sHtML

[R22] 截取子串
来源：http://wap.vehdjk.com/Article/details/gxdjkqdyq.sHtML

echo "${s:0:5}"
来源：http://baike.sjlbkw.cn/Article/details/gyspnrtju.sHtML

[R23] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/gmcbesarh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fktsv.cn/Article/details/gteudgxwx.sHtML

[R24] 大小写转换
来源：http://3g.tarul.cn/Article/details/gwlltccuk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.yfazqb.com/Article/details/glcckwfks.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.vehdjk.com/Article/details/gosqyalcw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.yfazqb.com/Article/details/gnyvsqwgg.sHtML

[R26] 命令替换
来源：http://3g.sjlbkw.cn/Article/details/grfdvawtl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.tarul.cn/Article/details/gfsklyxpc.sHtML

[R27] 算术展开
来源：http://www.m.share.tarul.cn/Article/details/gqwlyjtlv.sHtML

echo $((1 + 2 * 3))
来源：http://blog.vehdjk.com/Article/details/gndrgexif.sHtML

[R28] 浮点运算
来源：http://3g.fktsv.cn/Article/details/gioskvoem.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.bbcook.cn/Article/details/gukchqisd.sHtML

[R29] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/gidqqudww.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.bbcook.cn/Article/details/gegumpuyj.sHtML

[R30] 函数返回状态码
来源：http://baike.fktsv.cn/Article/details/geesmfhdg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.vehdjk.com/Article/details/gxsgxqxvo.sHtML

[R31] 局部变量
来源：http://3g.yfazqb.com/Article/details/gqocvlxmx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.vehdjk.com/Article/details/gpvwlwqjz.sHtML

[R32] 参数个数校验
来源：http://m.share.vehdjk.com/Article/details/gosubreaq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.tarul.cn/Article/details/gkirycywz.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fktsv.cn/Article/details/gkavkdzbd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.epnwcf.com/Article/details/ghkwwwavu.sHtML

[R34] 退出时清理
来源：http://read.share.yfazqb.com/Article/details/gqqkigllj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gfsurhlxz.sHtML

[R35] 后台执行并等待
来源：http://wap.fktsv.cn/Article/details/garsyrget.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.tarul.cn/Article/details/ggazksgcu.sHtML

[R36] 并发执行多个任务
来源：http://mobile.tarul.cn/Article/details/gprdouhxy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.yfazqb.com/Article/details/gfkpyssdf.sHtML

[R37] 把输出赋给变量
来源：http://blog.epnwcf.com/Article/details/geuafepzo.sHtML

files=$(ls -1)
来源：http://3g.sjlbkw.cn/Article/details/gytefhgtg.sHtML

[R38] 管道串联
来源：http://m.share.yfazqb.com/Article/details/gobinxeil.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.epnwcf.com/Article/details/ggiwcpayi.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.epnwcf.com/Article/details/grvoldeqc.sHtML

cmd > out.log 2>&1
来源：http://www.blog.vehdjk.com/Article/details/gqhyhturz.sHtML

[R40] 追加写日志
来源：http://www.share.tarul.cn/Article/details/gangucylk.sHtML

echo "log" >> out.log
来源：http://www.share.epnwcf.com/Article/details/gukqtgsmg.sHtML

[R41] 丢弃输出
来源：http://baike.bbcook.cn/Article/details/gbriatlem.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.yfazqb.com/Article/details/gblzxdiau.sHtML

[R42] 输入重定向
来源：http://www.share.sjlbkw.cn/Article/details/gzwzfzmwc.sHtML

wc -l < a.txt
来源：http://wap.bbcook.cn/Article/details/gqlfwfner.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.tarul.cn/Article/details/gyjvkcxkl.sHtML

find . -name "*.log" -type f
来源：http://blog.epnwcf.com/Article/details/guvlinfsa.sHtML

[R44] 按修改时间查找
来源：http://www.blog.tarul.cn/Article/details/gcqtntbpl.sHtML

find . -mtime -7 -type f
来源：http://www.share.bbcook.cn/Article/details/gwvvqhlrt.sHtML

[R45] 批量删除
来源：http://mobile.bbcook.cn/Article/details/grsyfibtd.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.vehdjk.com/Article/details/gcvocepoq.sHtML

[R46] 递归替换文件内容
来源：http://3g.sjlbkw.cn/Article/details/gnmbundba.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.sjlbkw.cn/Article/details/gxbklzqkn.sHtML

[R47] sed 单行替换
来源：http://wap.bbcook.cn/Article/details/gpibxutts.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gberjifta.sHtML

[R48] awk 取指定列
来源：http://www.share.sjlbkw.cn/Article/details/gztpoqslh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gfwfnkzyl.sHtML

[R49] awk 带条件
来源：http://www.m.share.bbcook.cn/Article/details/gooeakvwg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.epnwcf.com/Article/details/gsdgczhbq.sHtML

[R50] awk 求和
来源：http://m.share.sjlbkw.cn/Article/details/gqdiazzcf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fktsv.cn/Article/details/gbosttmgl.sHtML

[R51] 排序去重取前几
来源：http://blog.sjlbkw.cn/Article/details/gwvbpvbbo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.bbcook.cn/Article/details/gwrsijefh.sHtML

[R52] 统计行数
来源：http://m.share.bbcook.cn/Article/details/goseamqfs.sHtML

wc -l a.txt
来源：http://read.share.epnwcf.com/Article/details/gmvvfdyhx.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.tarul.cn/Article/details/gsbwxojxd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.bbcook.cn/Article/details/gcvrzypkl.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/gzdcgrffw.sHtML

diff a.txt b.txt
来源：http://www.blog.fktsv.cn/Article/details/gzhslwquy.sHtML

[R55] 压缩与解压
来源：http://www.m.share.vehdjk.com/Article/details/gdlvrvcsi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.bbcook.cn/Article/details/gjsthneva.sHtML

[R56] 远程拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gjptzhjdr.sHtML

scp file user@host:/path/
来源：http://blog.bbcook.cn/Article/details/gutydknuz.sHtML

[R57] 远程执行命令
来源：http://3g.sjlbkw.cn/Article/details/gjhuqsynp.sHtML

ssh user@host 'uptime'
来源：http://wap.sjlbkw.cn/Article/details/gtiktpimm.sHtML

[R58] 下载文件
来源：http://www.blog.yfazqb.com/Article/details/gcsghqopl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.bbcook.cn/Article/details/gqhkpvasu.sHtML

[R59] 发 POST JSON
来源：http://baike.tarul.cn/Article/details/ggcxhljxq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.yfazqb.com/Article/details/gicwossml.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/gdacmcukm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fktsv.cn/Article/details/grzjeanzq.sHtML

[R61] 磁盘占用
来源：http://www.m.share.epnwcf.com/Article/details/gauxigssk.sHtML

df -h;  du -sh *
来源：http://baike.yfazqb.com/Article/details/gbosyqeup.sHtML

[R62] 找最占空间的文件
来源：http://wap.fktsv.cn/Article/details/gabrefomr.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.vehdjk.com/Article/details/gyppljgbm.sHtML

[R63] 内存与进程
来源：http://baike.bbcook.cn/Article/details/gfevcnzup.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.sjlbkw.cn/Article/details/ggzpxuhra.sHtML

[R64] 结束进程
来源：http://read.share.epnwcf.com/Article/details/gzsqogqab.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fktsv.cn/Article/details/gbmthvrjn.sHtML

[R65] 查看端口占用
来源：http://3g.fktsv.cn/Article/details/gfigujhxl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.bbcook.cn/Article/details/gotuammjy.sHtML

[R66] 定时任务
来源：http://read.share.vehdjk.com/Article/details/gqokplotz.sHtML

crontab -e;  crontab -l
来源：http://mobile.sjlbkw.cn/Article/details/guwbrpdhx.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fktsv.cn/Article/details/gbfktwlrd.sHtML

openssl rand -hex 16
来源：http://wap.tarul.cn/Article/details/gnofxypfq.sHtML

[R68] 计算文件校验值
来源：http://www.share.epnwcf.com/Article/details/guviqtvcq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.vehdjk.com/Article/details/gqjrawcva.sHtML

[R69] 生成随机密码
来源：http://mobile.yfazqb.com/Article/details/gsokccsin.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.sjlbkw.cn/Article/details/gtpgzldhg.sHtML

[R70] 时间戳与互转
来源：http://3g.tarul.cn/Article/details/gwlazhpus.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.vehdjk.com/Article/details/gjidbhnse.sHtML

[R71] 日期格式化
来源：http://read.share.tarul.cn/Article/details/gpeymublq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.sjlbkw.cn/Article/details/gwlzbzkcz.sHtML

[R72] 等待端口就绪
来源：http://wap.epnwcf.com/Article/details/gmgjildpt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.bbcook.cn/Article/details/gjoxncxrr.sHtML

[R73] 分割大日志
来源：http://read.share.tarul.cn/Article/details/gvcvkigar.sHtML

split -l 1000 big.log part_
来源：http://mobile.epnwcf.com/Article/details/gzcpgkmbk.sHtML

[R74] 批量重命名
来源：http://3g.sjlbkw.cn/Article/details/gknvrayty.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.epnwcf.com/Article/details/gxmgbrdov.sHtML

[R75] 导出环境变量
来源：http://3g.vehdjk.com/Article/details/gvlxboazs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.bbcook.cn/Article/details/grccxcaub.sHtML

[R76] 使用临时文件
来源：http://wap.epnwcf.com/Article/details/gagbcoomd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/gwhuvmeur.sHtML

[R77] 读取用户输入
来源：http://baike.yfazqb.com/Article/details/ghhhnahkh.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/goigfvjvz.sHtML

[R78] 交互式菜单
来源：http://blog.fktsv.cn/Article/details/geblefgkd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.tarul.cn/Article/details/gifxlulgm.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/gprwmhbqd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.vehdjk.com/Article/details/gqibdvmvr.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.yfazqb.com/Article/details/giwmzdbls.sHtML

time ./run.sh
来源：http://www.blog.fktsv.cn/Article/details/gbspjpvis.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gukcsegdc.sHtML

S. C / C++ 专题
来源：http://www.blog.epnwcf.com/Article/details/gsjvpjvtw.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjqvhsynf.sHtML

[S01] C：Hello World
来源：http://3g.vehdjk.com/Article/details/gfxhveudk.sHtML

#include <stdio.h>
来源：http://wap.fktsv.cn/Article/details/gfsfjhnkv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.sjlbkw.cn/Article/details/gijnwpfmh.sHtML

[S02] C：变量与格式化输出
来源：http://3g.sjlbkw.cn/Article/details/glylsjtev.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.yfazqb.com/Article/details/gprzviuek.sHtML

[S03] C：读入整数
来源：http://3g.fktsv.cn/Article/details/gkervmtji.sHtML

int x; scanf("%d", &x);
来源：http://wap.yfazqb.com/Article/details/glshgklrg.sHtML

[S04] C：字符串复制
来源：http://www.blog.sjlbkw.cn/Article/details/gtdefvhts.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.yfazqb.com/Article/details/grddwiwco.sHtML

[S05] C：字符串长度
来源：http://www.share.bbcook.cn/Article/details/geypnsypw.sHtML

strlen(s)
来源：http://wap.sjlbkw.cn/Article/details/gejtxecli.sHtML

[S06] C：字符串比较
来源：http://www.blog.tarul.cn/Article/details/gksewcvfk.sHtML

strcmp(a, b) == 0
来源：http://m.share.epnwcf.com/Article/details/goeisfmmu.sHtML

[S07] C：数组遍历求和
来源：http://blog.yfazqb.com/Article/details/gwvyhajka.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.yfazqb.com/Article/details/giieznrwt.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fktsv.cn/Article/details/gbkapvnfe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.tarul.cn/Article/details/gpdgybfzy.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.sjlbkw.cn/Article/details/gjrskxqvp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/gpytfnjkb.sHtML

[S10] C：指针与解引用
来源：http://www.blog.sjlbkw.cn/Article/details/gzgorskby.sHtML

int *p = &a;  *p = 5;
来源：http://3g.epnwcf.com/Article/details/gddfehxhl.sHtML

[S11] C：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gnrsuvgvu.sHtML


<!-- 参考信息 -->