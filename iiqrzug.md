代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.yfazqb.com/Article/details/govhvnpxs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.yfazqb.com/Article/details/gfvmguuab.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/gfcrhgtjh.sHtML

[Q41] 多表连接
来源：http://m.share.sjlbkw.cn/Article/details/gsdtrsxzo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.epnwcf.com/Article/details/grfcgwgud.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.epnwcf.com/Article/details/gjjwolesz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.vehdjk.com/Article/details/ghynysbvu.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.sjlbkw.cn/Article/details/gauqtmfet.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/gzhrlhmea.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.sjlbkw.cn/Article/details/gnqbasrrm.sHtML

[Q43] 标量子查询
来源：http://baike.fktsv.cn/Article/details/gvbwjoora.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.yfazqb.com/Article/details/gbsplotyp.sHtML

[Q44] IN 子查询
来源：http://wap.bbcook.cn/Article/details/gaghvqdyg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.tarul.cn/Article/details/gewomjnph.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fktsv.cn/Article/details/gxckqkdwz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.tarul.cn/Article/details/gdjgzfeuz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.tarul.cn/Article/details/gpovnlvsf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gmszvgeqr.sHtML

[Q47] 与平均值比较
来源：http://m.share.sjlbkw.cn/Article/details/gmvuzokmn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.tarul.cn/Article/details/gpnkrettu.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.vehdjk.com/Article/details/glyhgpgjb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.bbcook.cn/Article/details/gnmjtwwws.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.epnwcf.com/Article/details/gydyuyebv.sHtML

[Q49] 更新单行
来源：http://blog.fktsv.cn/Article/details/gjemijwjl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/gpifrdmla.sHtML

[Q50] 批量更新
来源：http://blog.yfazqb.com/Article/details/gphdipxey.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fktsv.cn/Article/details/gdqpkjwfs.sHtML

[Q51] 用子查询更新
来源：http://www.blog.yfazqb.com/Article/details/gytusfuql.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.tarul.cn/Article/details/gesgymtik.sHtML

[Q52] 删除指定行
来源：http://baike.yfazqb.com/Article/details/gbjbsqghw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/getropjkc.sHtML

[Q53] 按条件删除
来源：http://3g.fktsv.cn/Article/details/gutjvkotz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.vehdjk.com/Article/details/gyfhpotjc.sHtML

[Q54] 清空表
来源：http://www.blog.epnwcf.com/Article/details/gmetkaxni.sHtML

TRUNCATE TABLE logs;
来源：http://wap.sjlbkw.cn/Article/details/gulnlkwvy.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.tarul.cn/Article/details/gpnbbnzpg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.epnwcf.com/Article/details/gechfugjk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.yfazqb.com/Article/details/gosfumuiz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gieuefidq.sHtML

[Q57] 行号
来源：http://m.share.vehdjk.com/Article/details/gpjwkrygh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fktsv.cn/Article/details/gyihnnboz.sHtML

[Q58] 累计求和
来源：http://wap.bbcook.cn/Article/details/girdewweg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gzodnllqm.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/gykljsaef.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gqefjkagt.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.vehdjk.com/Article/details/giwwvpwcz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.bbcook.cn/Article/details/gqatjtbwo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.tarul.cn/Article/details/gcpbdzevd.sHtML

[Q61] 移动平均
来源：http://mobile.fktsv.cn/Article/details/gzsbfxiyr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/ggrbpvatv.sHtML

[Q62] 分组占比
来源：http://www.blog.vehdjk.com/Article/details/gzdnrrmbt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gsmpcpmqg.sHtML

[Q63] 开启事务
来源：http://m.share.tarul.cn/Article/details/gutkhetcr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.vehdjk.com/Article/details/gjofehqop.sHtML

[Q64] 提交事务
来源：http://read.share.tarul.cn/Article/details/guryfumiq.sHtML

COMMIT;
来源：http://baike.yfazqb.com/Article/details/gcwcvxbnd.sHtML

[Q65] 回滚事务
来源：http://www.blog.vehdjk.com/Article/details/gognizecj.sHtML

ROLLBACK;
来源：http://read.share.epnwcf.com/Article/details/gvfcxwsfw.sHtML

[Q66] 行锁查询
来源：http://baike.epnwcf.com/Article/details/gxsraoczn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.yfazqb.com/Article/details/gaaxxyqew.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fktsv.cn/Article/details/glkglybkn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.tarul.cn/Article/details/gfeyucoff.sHtML

[Q68] 保存点
来源：http://blog.yfazqb.com/Article/details/gajqbmgtx.sHtML

SAVEPOINT sp1;
来源：http://www.share.vehdjk.com/Article/details/gsqrmshef.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fktsv.cn/Article/details/gocultzef.sHtML

[Q69] 查看执行计划
来源：http://www.blog.vehdjk.com/Article/details/gywndauph.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.sjlbkw.cn/Article/details/gyvtemqth.sHtML

[Q70] 更新统计信息
来源：http://blog.yfazqb.com/Article/details/gsgcstgar.sHtML

ANALYZE TABLE users;
来源：http://m.share.tarul.cn/Article/details/gbklcmpai.sHtML

[Q71] 查看建表语句
来源：http://www.blog.sjlbkw.cn/Article/details/gcjqkbivi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.bbcook.cn/Article/details/gcaqgmbmn.sHtML

[Q72] 查看索引
来源：http://baike.vehdjk.com/Article/details/gnaatfbvr.sHtML

SHOW INDEX FROM users;
来源：http://baike.fktsv.cn/Article/details/gmbaesayr.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/gtgsuxlnq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.tarul.cn/Article/details/gksliqpij.sHtML

[Q74] 强制使用索引
来源：http://wap.yfazqb.com/Article/details/gngpqqpvi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.bbcook.cn/Article/details/gvwmxohdy.sHtML

[Q75] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/gvkmojjlm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/goqsxesoy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.yfazqb.com/Article/details/gbvdnlawu.sHtML

[Q76] 按天统计
来源：http://www.share.epnwcf.com/Article/details/gokfeqlsv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.sjlbkw.cn/Article/details/gshupuglp.sHtML

[Q77] 时间加减
来源：http://blog.epnwcf.com/Article/details/ggczefsls.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/gsnbtshsq.sHtML

[Q78] 当前时间
来源：http://www.blog.vehdjk.com/Article/details/ghvokgpoa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.epnwcf.com/Article/details/gggqqcpoh.sHtML

[Q79] 字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gurzbcnkh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.yfazqb.com/Article/details/gdzawiynv.sHtML

[Q80] 字符串截取
来源：http://www.m.share.tarul.cn/Article/details/grrusnexz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gjropsqxd.sHtML

[Q81] 字符串替换
来源：http://wap.yfazqb.com/Article/details/gbybhauwm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.tarul.cn/Article/details/gorwlnyhb.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.epnwcf.com/Article/details/gounserni.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gtgmmgnzw.sHtML

[Q83] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/gubxfskkb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gwwqcijdx.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.epnwcf.com/Article/details/gejbkxyfn.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gtshhepnn.sHtML

[Q85] 数值取整
来源：http://m.share.tarul.cn/Article/details/gonplebvu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.tarul.cn/Article/details/gmrhadhcq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.tarul.cn/Article/details/gwybtdqpa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.yfazqb.com/Article/details/guvufjige.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.epnwcf.com/Article/details/gkufskrao.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.tarul.cn/Article/details/gpfozagih.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.yfazqb.com/Article/details/gidslgytx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fktsv.cn/Article/details/gielcozva.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.tarul.cn/Article/details/glnshvlkh.sHtML

[Q89] 判断表是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gklbspgof.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.vehdjk.com/Article/details/gseaybhvx.sHtML

[Q90] 生成序号列
来源：http://baike.fktsv.cn/Article/details/gukbpheqm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.bbcook.cn/Article/details/gofgxtkvx.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gllpqfpqz.sHtML

R. Bash 专题
来源：http://3g.yfazqb.com/Article/details/ggbmyjctm.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gfdjmjuje.sHtML

[R01] shebang 与严格模式
来源：http://blog.bbcook.cn/Article/details/gwbkiqcau.sHtML

#!/usr/bin/env bash
来源：http://blog.fktsv.cn/Article/details/gkfbwqffo.sHtML

set -euo pipefail
来源：http://baike.vehdjk.com/Article/details/gpikhrifp.sHtML

[R02] 变量赋值与使用
来源：http://3g.fktsv.cn/Article/details/gaqowdege.sHtML

name="Tom"; echo "$name"
来源：http://wap.sjlbkw.cn/Article/details/gysmgwstl.sHtML

[R03] 只读变量
来源：http://www.m.share.fktsv.cn/Article/details/gmjjlylic.sHtML

readonly PI=3.14
来源：http://blog.tarul.cn/Article/details/gtzvousrh.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/gnohqnugo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.epnwcf.com/Article/details/ghbiuadzi.sHtML

[R05] 参数默认值
来源：http://wap.vehdjk.com/Article/details/goyzyjtus.sHtML

name="${1:-default}"
来源：http://read.share.sjlbkw.cn/Article/details/gzawkdryw.sHtML

[R06] 判断命令是否存在
来源：http://m.share.yfazqb.com/Article/details/gqkunyzqk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/gkpujiiht.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/grzvrdsrt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.tarul.cn/Article/details/gpllzyhvy.sHtML

[R08] 数值比较
来源：http://www.share.sjlbkw.cn/Article/details/gwxvtkrxv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.vehdjk.com/Article/details/gzmakoajx.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gjndnranu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.sjlbkw.cn/Article/details/gwtwiujna.sHtML

[R10] 正则匹配
来源：http://www.share.vehdjk.com/Article/details/gqrkjckky.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.epnwcf.com/Article/details/gcgmlkuew.sHtML

[R11] case 多分支
来源：http://3g.bbcook.cn/Article/details/gexkztalc.sHtML

case "$1" in
来源：http://3g.yfazqb.com/Article/details/gewmueywt.sHtML

start) echo "启动" ;;
来源：http://www.blog.tarul.cn/Article/details/gauyhpeit.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fktsv.cn/Article/details/gwsogqxut.sHtML

*)     echo "未知命令" ;;
来源：http://3g.vehdjk.com/Article/details/gzvpkdkfq.sHtML

esac
来源：http://www.blog.bbcook.cn/Article/details/gkqnlqadc.sHtML

[R12] for 遍历文件
来源：http://baike.bbcook.cn/Article/details/grhaxsask.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.sjlbkw.cn/Article/details/gjbfoqhdr.sHtML

[R13] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gyowkackw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gmqvlmayp.sHtML

[R14] C 风格 for
来源：http://baike.bbcook.cn/Article/details/gdlvydxch.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/givwdhhue.sHtML

[R15] while 逐行读文件
来源：http://3g.bbcook.cn/Article/details/gfucoigly.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.yfazqb.com/Article/details/gsojkjlsr.sHtML

[R16] until 等待条件
来源：http://www.blog.epnwcf.com/Article/details/gyuwarblo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/geamfuugo.sHtML

[R17] 数组定义与取值
来源：http://m.share.fktsv.cn/Article/details/gqfwfjdti.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fktsv.cn/Article/details/glziwdjbm.sHtML

[R18] 遍历数组
来源：http://www.share.fktsv.cn/Article/details/gdlwrlwcv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fktsv.cn/Article/details/gkcppiida.sHtML

[R19] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzwkatbv.sHtML

echo "${#arr[@]}"
来源：http://mobile.sjlbkw.cn/Article/details/gkgxksmkc.sHtML

[R20] 关联数组（字典）
来源：http://m.share.tarul.cn/Article/details/gxueikkzj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.vehdjk.com/Article/details/gkrwiufte.sHtML

[R21] 字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/grdoqyerf.sHtML

echo "${#s}"
来源：http://read.share.fktsv.cn/Article/details/ghgdpaxlb.sHtML

[R22] 截取子串
来源：http://read.share.bbcook.cn/Article/details/gmipexktf.sHtML

echo "${s:0:5}"
来源：http://blog.fktsv.cn/Article/details/gaxgmgirx.sHtML

[R23] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gxtvkxgus.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.yfazqb.com/Article/details/gnmphqrij.sHtML

[R24] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gxkizrytn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fktsv.cn/Article/details/gpbzfsgvz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.bbcook.cn/Article/details/gjsmjguuh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.tarul.cn/Article/details/ghpmsdeus.sHtML

[R26] 命令替换
来源：http://blog.vehdjk.com/Article/details/gifsgwcou.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.yfazqb.com/Article/details/grxeahejl.sHtML

[R27] 算术展开
来源：http://wap.epnwcf.com/Article/details/gololoqiq.sHtML

echo $((1 + 2 * 3))
来源：http://blog.yfazqb.com/Article/details/glqjyrdbb.sHtML

[R28] 浮点运算
来源：http://read.share.fktsv.cn/Article/details/ggshefyel.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.sjlbkw.cn/Article/details/gxzufpkjq.sHtML

[R29] 定义函数
来源：http://baike.vehdjk.com/Article/details/gaegmjdiq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.vehdjk.com/Article/details/ghhjrwbsa.sHtML

[R30] 函数返回状态码
来源：http://baike.yfazqb.com/Article/details/gxwudpahl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.sjlbkw.cn/Article/details/gpcrgzsle.sHtML

[R31] 局部变量
来源：http://m.share.fktsv.cn/Article/details/gzcsdtcrg.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.yfazqb.com/Article/details/gsxjilzwv.sHtML

[R32] 参数个数校验
来源：http://www.m.share.bbcook.cn/Article/details/gysnznhkn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gashlwxpe.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.bbcook.cn/Article/details/gxwibcwhn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fktsv.cn/Article/details/gkhribyif.sHtML

[R34] 退出时清理
来源：http://mobile.epnwcf.com/Article/details/gxeenqkaq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/gyxczqidl.sHtML

[R35] 后台执行并等待
来源：http://www.blog.tarul.cn/Article/details/gkjfjblgr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.vehdjk.com/Article/details/gvpsszdcx.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.epnwcf.com/Article/details/gqqaynswb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.tarul.cn/Article/details/gbzlwgbvd.sHtML

[R37] 把输出赋给变量
来源：http://mobile.tarul.cn/Article/details/gemmvlldo.sHtML

files=$(ls -1)
来源：http://baike.bbcook.cn/Article/details/gdyvaqims.sHtML

[R38] 管道串联
来源：http://wap.bbcook.cn/Article/details/gcfdolbnd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.bbcook.cn/Article/details/gtdilospa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fktsv.cn/Article/details/gppmthgds.sHtML

cmd > out.log 2>&1
来源：http://blog.fktsv.cn/Article/details/gxixveymn.sHtML

[R40] 追加写日志
来源：http://m.share.tarul.cn/Article/details/gwelfatfa.sHtML

echo "log" >> out.log
来源：http://www.share.yfazqb.com/Article/details/galnfydtp.sHtML

[R41] 丢弃输出
来源：http://mobile.sjlbkw.cn/Article/details/gftvdhjtz.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gckneooho.sHtML

[R42] 输入重定向
来源：http://wap.fktsv.cn/Article/details/gjutavryu.sHtML

wc -l < a.txt
来源：http://m.share.fktsv.cn/Article/details/gxidkujfj.sHtML

[R43] 按名字查找文件
来源：http://blog.vehdjk.com/Article/details/gmozvioct.sHtML

find . -name "*.log" -type f
来源：http://m.share.vehdjk.com/Article/details/gaaxndkwi.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkeketwp.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.tarul.cn/Article/details/glgucurqc.sHtML

[R45] 批量删除
来源：http://read.share.vehdjk.com/Article/details/ggniqoqyt.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/gpyewpbav.sHtML

[R46] 递归替换文件内容
来源：http://m.share.bbcook.cn/Article/details/gyewzcjhr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.epnwcf.com/Article/details/gdfseqxnb.sHtML

[R47] sed 单行替换
来源：http://baike.epnwcf.com/Article/details/gahsgeufp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.yfazqb.com/Article/details/gjenljwxt.sHtML

[R48] awk 取指定列
来源：http://mobile.epnwcf.com/Article/details/gppaylvjx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gqdfjdwdy.sHtML

[R49] awk 带条件
来源：http://3g.epnwcf.com/Article/details/gwjuxzgmk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fktsv.cn/Article/details/gsgvswguv.sHtML

[R50] awk 求和
来源：http://m.share.epnwcf.com/Article/details/gsclypmjs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.vehdjk.com/Article/details/gnyugbbsu.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/gwrcwytjl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.epnwcf.com/Article/details/guyujhnnr.sHtML

[R52] 统计行数
来源：http://www.m.share.fktsv.cn/Article/details/gpcomqcoa.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/gameklags.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/gmplrggbr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.bbcook.cn/Article/details/gvldsaqbh.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/grgyzshia.sHtML

diff a.txt b.txt
来源：http://www.blog.fktsv.cn/Article/details/gezhfytpm.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/gtbvghppp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.epnwcf.com/Article/details/giuuucxnk.sHtML

[R56] 远程拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gxelycwlu.sHtML

scp file user@host:/path/
来源：http://wap.fktsv.cn/Article/details/gegawjqvi.sHtML

[R57] 远程执行命令
来源：http://www.m.share.vehdjk.com/Article/details/gvbicvixk.sHtML

ssh user@host 'uptime'
来源：http://www.share.bbcook.cn/Article/details/gvzqvagbj.sHtML

[R58] 下载文件
来源：http://read.share.bbcook.cn/Article/details/gwlpovnqm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.yfazqb.com/Article/details/gikfqhzod.sHtML

[R59] 发 POST JSON
来源：http://m.share.vehdjk.com/Article/details/gbohhdhqn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.bbcook.cn/Article/details/gyizadjvs.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gmrgxhfqb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fktsv.cn/Article/details/gfeufbflw.sHtML

[R61] 磁盘占用
来源：http://m.share.fktsv.cn/Article/details/gikrozdqm.sHtML

df -h;  du -sh *
来源：http://baike.epnwcf.com/Article/details/gfkbgypqm.sHtML

[R62] 找最占空间的文件
来源：http://mobile.yfazqb.com/Article/details/gppyxrwqv.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fktsv.cn/Article/details/gpqfqojls.sHtML

[R63] 内存与进程
来源：http://mobile.yfazqb.com/Article/details/gvaktstrg.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.vehdjk.com/Article/details/gqvxjmpva.sHtML

[R64] 结束进程
来源：http://www.share.fktsv.cn/Article/details/glfwhgrql.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvyjglxb.sHtML

[R65] 查看端口占用
来源：http://m.share.bbcook.cn/Article/details/gizpodwgc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.yfazqb.com/Article/details/gqrcxnyka.sHtML

[R66] 定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gpnwpvjxi.sHtML

crontab -e;  crontab -l
来源：http://3g.vehdjk.com/Article/details/gqrjbbued.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.yfazqb.com/Article/details/gzshcwzip.sHtML

openssl rand -hex 16
来源：http://www.blog.fktsv.cn/Article/details/gvxvivbof.sHtML

[R68] 计算文件校验值
来源：http://3g.epnwcf.com/Article/details/gyheqnhwp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.tarul.cn/Article/details/gizklpswu.sHtML

[R69] 生成随机密码
来源：http://wap.vehdjk.com/Article/details/gtzneomyj.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.epnwcf.com/Article/details/gkqpxekvj.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.epnwcf.com/Article/details/gwwdqbofu.sHtML

date +%s;  date -d @1700000000
来源：http://baike.yfazqb.com/Article/details/gpeemlmvq.sHtML

[R71] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gkayzichp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.bbcook.cn/Article/details/gcpxgzgfu.sHtML

[R72] 等待端口就绪
来源：http://3g.vehdjk.com/Article/details/gbttrcukj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/glvuvxdff.sHtML

[R73] 分割大日志
来源：http://m.share.epnwcf.com/Article/details/gmnifdrkf.sHtML

split -l 1000 big.log part_
来源：http://www.blog.vehdjk.com/Article/details/gjsjfovvs.sHtML

[R74] 批量重命名
来源：http://wap.fktsv.cn/Article/details/gqslfjrcz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.epnwcf.com/Article/details/gjtuxeomo.sHtML

[R75] 导出环境变量
来源：http://3g.fktsv.cn/Article/details/gkdvxialp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.yfazqb.com/Article/details/gtqpiykgw.sHtML

[R76] 使用临时文件
来源：http://3g.yfazqb.com/Article/details/gkwphgiyf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gpcllfzqh.sHtML

[R77] 读取用户输入
来源：http://blog.vehdjk.com/Article/details/gbbxhthux.sHtML

read -rp "请输入: " ans
来源：http://www.share.vehdjk.com/Article/details/glnkzfcwe.sHtML

[R78] 交互式菜单
来源：http://www.share.vehdjk.com/Article/details/gpwfqcctv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fktsv.cn/Article/details/gebrjirje.sHtML

[R79] 解析命令行选项
来源：http://read.share.bbcook.cn/Article/details/goqtvqdny.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.bbcook.cn/Article/details/gqsrqnycn.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.yfazqb.com/Article/details/ghnpoqnsr.sHtML

time ./run.sh
来源：http://mobile.sjlbkw.cn/Article/details/gxuizkazp.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtkvubqyi.sHtML

S. C / C++ 专题
来源：http://www.share.tarul.cn/Article/details/gshlbqeoy.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gbexyoens.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gxyqezuyr.sHtML

#include <stdio.h>
来源：http://www.m.share.vehdjk.com/Article/details/gdhdfupcd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.tarul.cn/Article/details/gkrcejuxd.sHtML

[S02] C：变量与格式化输出
来源：http://3g.bbcook.cn/Article/details/gtyazihgo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.sjlbkw.cn/Article/details/gklireula.sHtML

[S03] C：读入整数
来源：http://blog.tarul.cn/Article/details/gidvktpaa.sHtML

int x; scanf("%d", &x);
来源：http://baike.fktsv.cn/Article/details/gtjydifub.sHtML

[S04] C：字符串复制
来源：http://baike.epnwcf.com/Article/details/gyfqvmzdn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.epnwcf.com/Article/details/gzinmjgbm.sHtML

[S05] C：字符串长度
来源：http://blog.epnwcf.com/Article/details/gtxferfir.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/ghjhleoxb.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/gijfssmya.sHtML

strcmp(a, b) == 0
来源：http://3g.vehdjk.com/Article/details/gqhhkrulr.sHtML

[S07] C：数组遍历求和
来源：http://read.share.tarul.cn/Article/details/gskupwflv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.vehdjk.com/Article/details/gwnniayut.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.vehdjk.com/Article/details/gskkezzhw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.bbcook.cn/Article/details/gqksiosxo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.tarul.cn/Article/details/gldswvvrt.sHtML


<!-- 参考信息 -->