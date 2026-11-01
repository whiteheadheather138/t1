代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fktsv.cn/Article/details/guaorigjt.sHtML

) t WHERE rn = 1;
来源：http://baike.bbcook.cn/Article/details/gyohpzkbr.sHtML

[Q35] 内连接
来源：http://mobile.epnwcf.com/Article/details/gglgmhrsp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/ghavialtm.sHtML

[Q36] 左连接
来源：http://baike.yfazqb.com/Article/details/gzqwblyoe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/grwnrdwes.sHtML

[Q37] 右连接
来源：http://www.m.share.epnwcf.com/Article/details/giojvwcoh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fktsv.cn/Article/details/gculzyqja.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fktsv.cn/Article/details/gzuenbotr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.sjlbkw.cn/Article/details/gxhhkiduz.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.vehdjk.com/Article/details/grhudwzhp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.epnwcf.com/Article/details/gcxnknmqx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fktsv.cn/Article/details/guqapjeuj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.yfazqb.com/Article/details/gblsplxai.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.vehdjk.com/Article/details/gufrotyfu.sHtML

[Q41] 多表连接
来源：http://baike.bbcook.cn/Article/details/gstxschqt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.bbcook.cn/Article/details/gnqsdacjx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.vehdjk.com/Article/details/giniumgex.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.vehdjk.com/Article/details/geyigthni.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.vehdjk.com/Article/details/gqcpizqbw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.bbcook.cn/Article/details/gfrwffzwd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.yfazqb.com/Article/details/gxtejvqzv.sHtML

[Q43] 标量子查询
来源：http://baike.tarul.cn/Article/details/gxzbijsiy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.epnwcf.com/Article/details/gjfdkmmsr.sHtML

[Q44] IN 子查询
来源：http://mobile.epnwcf.com/Article/details/gucnhhoxo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.epnwcf.com/Article/details/gvwpbfjoq.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.tarul.cn/Article/details/gqcxezybo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/gjblgmqeo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.sjlbkw.cn/Article/details/gpzcszxls.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gscxwslty.sHtML

[Q47] 与平均值比较
来源：http://mobile.yfazqb.com/Article/details/gcrtkczbd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.epnwcf.com/Article/details/glixyqyql.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.vehdjk.com/Article/details/gbvelrcgu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.bbcook.cn/Article/details/gaahyxulx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fktsv.cn/Article/details/gmtswqtnw.sHtML

[Q49] 更新单行
来源：http://www.blog.vehdjk.com/Article/details/gxtqgmmax.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gcuptcalt.sHtML

[Q50] 批量更新
来源：http://baike.yfazqb.com/Article/details/gxturbibf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.epnwcf.com/Article/details/gwgbqtxxv.sHtML

[Q51] 用子查询更新
来源：http://mobile.yfazqb.com/Article/details/gsgmyqsov.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.sjlbkw.cn/Article/details/ghgatipdx.sHtML

[Q52] 删除指定行
来源：http://blog.sjlbkw.cn/Article/details/ggkpuxomj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gjubcekge.sHtML

[Q53] 按条件删除
来源：http://baike.tarul.cn/Article/details/gmpcbuabq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.vehdjk.com/Article/details/gdfzylyok.sHtML

[Q54] 清空表
来源：http://read.share.bbcook.cn/Article/details/gvxpcfdnl.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fktsv.cn/Article/details/gpuweqtij.sHtML

[Q55] 排名（并列占位）
来源：http://blog.sjlbkw.cn/Article/details/gofdrysxi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.tarul.cn/Article/details/gxdqqhros.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.sjlbkw.cn/Article/details/gjgxqcfmo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.yfazqb.com/Article/details/gxqxiwtdi.sHtML

[Q57] 行号
来源：http://www.share.fktsv.cn/Article/details/gomhixoes.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.yfazqb.com/Article/details/geophjobf.sHtML

[Q58] 累计求和
来源：http://www.share.yfazqb.com/Article/details/guzbzdqjk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.yfazqb.com/Article/details/garkdnwqx.sHtML

[Q59] 分组内累计
来源：http://www.share.epnwcf.com/Article/details/ggikspwca.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gwbrspeol.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fktsv.cn/Article/details/grlwuswix.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.yfazqb.com/Article/details/gntakkzxc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.vehdjk.com/Article/details/gstauohpb.sHtML

[Q61] 移动平均
来源：http://blog.tarul.cn/Article/details/giaozfrbs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gdqvkzwdo.sHtML

[Q62] 分组占比
来源：http://3g.yfazqb.com/Article/details/gtgfguqtm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gwyaevtbh.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/gyvduahnl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/gtrqwjaty.sHtML

[Q64] 提交事务
来源：http://mobile.bbcook.cn/Article/details/gfzctkdba.sHtML

COMMIT;
来源：http://www.m.share.sjlbkw.cn/Article/details/gejhfjonv.sHtML

[Q65] 回滚事务
来源：http://mobile.sjlbkw.cn/Article/details/gyxufdlos.sHtML

ROLLBACK;
来源：http://www.blog.tarul.cn/Article/details/gzvgparbv.sHtML

[Q66] 行锁查询
来源：http://3g.sjlbkw.cn/Article/details/gzqxuzxgn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.tarul.cn/Article/details/gpupbiest.sHtML

[Q67] 设置隔离级别
来源：http://m.share.yfazqb.com/Article/details/ggqzejnqc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.yfazqb.com/Article/details/gohjfkwvl.sHtML

[Q68] 保存点
来源：http://read.share.vehdjk.com/Article/details/gyyfisqlg.sHtML

SAVEPOINT sp1;
来源：http://www.blog.bbcook.cn/Article/details/gxufhjvvi.sHtML

ROLLBACK TO sp1;
来源：http://wap.tarul.cn/Article/details/gxofkvknz.sHtML

[Q69] 查看执行计划
来源：http://wap.epnwcf.com/Article/details/girmaxvhl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.sjlbkw.cn/Article/details/guluxqbxt.sHtML

[Q70] 更新统计信息
来源：http://wap.tarul.cn/Article/details/gljftikmu.sHtML

ANALYZE TABLE users;
来源：http://www.blog.sjlbkw.cn/Article/details/ghncpxrlu.sHtML

[Q71] 查看建表语句
来源：http://m.share.fktsv.cn/Article/details/gxjwbmntc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.bbcook.cn/Article/details/gdxgqfnbk.sHtML

[Q72] 查看索引
来源：http://www.m.share.fktsv.cn/Article/details/gokyflsgo.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gafypmhiq.sHtML

[Q73] 查看表状态
来源：http://read.share.tarul.cn/Article/details/gczxyvucj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.vehdjk.com/Article/details/gugyoyegp.sHtML

[Q74] 强制使用索引
来源：http://blog.fktsv.cn/Article/details/gxlxkvucm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.yfazqb.com/Article/details/gazeckuda.sHtML

[Q75] 日期格式化
来源：http://blog.tarul.cn/Article/details/gopbpgoct.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gpobbgxvm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/gdysegxdn.sHtML

[Q76] 按天统计
来源：http://www.blog.fktsv.cn/Article/details/gkhdpsqky.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fktsv.cn/Article/details/grbtaowek.sHtML

[Q77] 时间加减
来源：http://mobile.epnwcf.com/Article/details/gtapeohtf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.vehdjk.com/Article/details/gnmzvgzbe.sHtML

[Q78] 当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gdkynzcmj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fktsv.cn/Article/details/giybtiqfp.sHtML

[Q79] 字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/gvmfvuyzw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.bbcook.cn/Article/details/greihicez.sHtML

[Q80] 字符串截取
来源：http://baike.tarul.cn/Article/details/goyxaduvk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gkvedcwwo.sHtML

[Q81] 字符串替换
来源：http://read.share.yfazqb.com/Article/details/gljupyfyw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gmnrhcnws.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.sjlbkw.cn/Article/details/ghaenpnnc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gejdicyki.sHtML

[Q83] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/griwmidaz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/ggdsmnubb.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gfnyfbpoe.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gdboqsxvp.sHtML

[Q85] 数值取整
来源：http://www.blog.epnwcf.com/Article/details/genfpbzwi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.bbcook.cn/Article/details/gfnuhezrq.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.vehdjk.com/Article/details/gtjdpqqgs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fktsv.cn/Article/details/glxektmwc.sHtML

[Q87] JSON 字段做条件
来源：http://baike.bbcook.cn/Article/details/gvizghaer.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/gcjyidsik.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.vehdjk.com/Article/details/gknnbzfgo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.bbcook.cn/Article/details/gxwmcfhmf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.yfazqb.com/Article/details/gwtckkwfs.sHtML

[Q89] 判断表是否存在
来源：http://blog.epnwcf.com/Article/details/ggsxgficv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.tarul.cn/Article/details/gmpmfucac.sHtML

[Q90] 生成序号列
来源：http://read.share.bbcook.cn/Article/details/ghxaqjheh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/gzbhnggxh.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gnhqbgsfa.sHtML

R. Bash 专题
来源：http://www.share.vehdjk.com/Article/details/gapvhtfkc.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gfzmwjuvn.sHtML

[R01] shebang 与严格模式
来源：http://mobile.bbcook.cn/Article/details/gkyznybzn.sHtML

#!/usr/bin/env bash
来源：http://wap.vehdjk.com/Article/details/gbguumarx.sHtML

set -euo pipefail
来源：http://blog.bbcook.cn/Article/details/gkhnuxkhx.sHtML

[R02] 变量赋值与使用
来源：http://baike.yfazqb.com/Article/details/grpmibxhx.sHtML

name="Tom"; echo "$name"
来源：http://blog.epnwcf.com/Article/details/gsgmvuafx.sHtML

[R03] 只读变量
来源：http://www.share.vehdjk.com/Article/details/gtgpgyehl.sHtML

readonly PI=3.14
来源：http://wap.epnwcf.com/Article/details/ghblctniu.sHtML

[R04] 位置参数
来源：http://blog.bbcook.cn/Article/details/grrszffez.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.sjlbkw.cn/Article/details/ghdookqkm.sHtML

[R05] 参数默认值
来源：http://www.share.bbcook.cn/Article/details/gxhzpfguq.sHtML

name="${1:-default}"
来源：http://www.m.share.bbcook.cn/Article/details/gkccayxut.sHtML

[R06] 判断命令是否存在
来源：http://read.share.epnwcf.com/Article/details/gkgkxktdp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/gnusdxipf.sHtML

[R07] if 判断文件
来源：http://wap.tarul.cn/Article/details/gpvzfezsl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.yfazqb.com/Article/details/gbyjcpder.sHtML

[R08] 数值比较
来源：http://www.share.yfazqb.com/Article/details/gntvlpmsi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/grrlfwzmz.sHtML

[R09] 字符串比较
来源：http://www.blog.tarul.cn/Article/details/glaonvpob.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.tarul.cn/Article/details/gzhrtyseh.sHtML

[R10] 正则匹配
来源：http://blog.sjlbkw.cn/Article/details/gwhsfawkn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.vehdjk.com/Article/details/gstaewhrm.sHtML

[R11] case 多分支
来源：http://mobile.vehdjk.com/Article/details/grvbgajeh.sHtML

case "$1" in
来源：http://www.share.vehdjk.com/Article/details/gkuikafuq.sHtML

start) echo "启动" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/ggjqozyhq.sHtML

stop)  echo "停止" ;;
来源：http://wap.bbcook.cn/Article/details/gfigcgkzm.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.vehdjk.com/Article/details/gscdcudtu.sHtML

esac
来源：http://m.share.tarul.cn/Article/details/gtayggqxg.sHtML

[R12] for 遍历文件
来源：http://blog.yfazqb.com/Article/details/gcuqconrg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.yfazqb.com/Article/details/gkjwoxylr.sHtML

[R13] for 计数循环
来源：http://www.share.yfazqb.com/Article/details/gggducvea.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.tarul.cn/Article/details/girtpaqeu.sHtML

[R14] C 风格 for
来源：http://baike.yfazqb.com/Article/details/gzdyywlim.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gupimjvlu.sHtML

[R15] while 逐行读文件
来源：http://baike.vehdjk.com/Article/details/gvpihnsvy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.bbcook.cn/Article/details/gezxhsrsf.sHtML

[R16] until 等待条件
来源：http://baike.epnwcf.com/Article/details/gxdsfjbpm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/gissbtjqg.sHtML

[R17] 数组定义与取值
来源：http://read.share.fktsv.cn/Article/details/gcjxeapie.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.yfazqb.com/Article/details/gwquudnnj.sHtML

[R18] 遍历数组
来源：http://read.share.sjlbkw.cn/Article/details/gluplalpc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.vehdjk.com/Article/details/gvxrnrrsc.sHtML

[R19] 数组长度
来源：http://www.m.share.vehdjk.com/Article/details/gmugpryzp.sHtML

echo "${#arr[@]}"
来源：http://baike.fktsv.cn/Article/details/gbxwbecni.sHtML

[R20] 关联数组（字典）
来源：http://baike.yfazqb.com/Article/details/gknghnvtb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.yfazqb.com/Article/details/ghtcyujhj.sHtML

[R21] 字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gcbvtzwez.sHtML

echo "${#s}"
来源：http://mobile.epnwcf.com/Article/details/gliizfpgh.sHtML

[R22] 截取子串
来源：http://baike.vehdjk.com/Article/details/gryborjpd.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/ggvvgclyo.sHtML

[R23] 字符串替换
来源：http://m.share.fktsv.cn/Article/details/gcnijudvu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.epnwcf.com/Article/details/gipdwhgeo.sHtML

[R24] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gvsrrrxod.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.yfazqb.com/Article/details/gtvwxmhek.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.vehdjk.com/Article/details/gdgmewdwz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/ggunlcwoj.sHtML

[R26] 命令替换
来源：http://www.share.tarul.cn/Article/details/gmgvwliio.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.yfazqb.com/Article/details/gxyvvvtfk.sHtML

[R27] 算术展开
来源：http://wap.vehdjk.com/Article/details/gowhjigvp.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fktsv.cn/Article/details/gonzjfchc.sHtML

[R28] 浮点运算
来源：http://mobile.bbcook.cn/Article/details/ggrzdxphq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.bbcook.cn/Article/details/gkleqjqpa.sHtML

[R29] 定义函数
来源：http://www.blog.tarul.cn/Article/details/glnjdrioo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.yfazqb.com/Article/details/gognrdnsa.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.tarul.cn/Article/details/ggkhcarpp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fktsv.cn/Article/details/gmwebxklf.sHtML

[R31] 局部变量
来源：http://blog.sjlbkw.cn/Article/details/gnttxzdhf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.vehdjk.com/Article/details/gkggcwcjp.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fktsv.cn/Article/details/gvzhcfaad.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gdpwxpykm.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.tarul.cn/Article/details/ghujjkons.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.vehdjk.com/Article/details/gklchpngi.sHtML

[R34] 退出时清理
来源：http://read.share.fktsv.cn/Article/details/gixoeupcm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fktsv.cn/Article/details/gjpaofibi.sHtML

[R35] 后台执行并等待
来源：http://www.share.fktsv.cn/Article/details/grarxjzzd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.tarul.cn/Article/details/gibxufnfr.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.tarul.cn/Article/details/gpoemdmff.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.bbcook.cn/Article/details/gctifhhxi.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.tarul.cn/Article/details/gflaflhal.sHtML

files=$(ls -1)
来源：http://read.share.vehdjk.com/Article/details/gvpqzyxao.sHtML

[R38] 管道串联
来源：http://blog.vehdjk.com/Article/details/gvlkrbiww.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fktsv.cn/Article/details/gdnfupzki.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.bbcook.cn/Article/details/gsgdmzkib.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gltmdviyi.sHtML

[R40] 追加写日志
来源：http://mobile.vehdjk.com/Article/details/gcjnvrmvf.sHtML

echo "log" >> out.log
来源：http://mobile.tarul.cn/Article/details/gktspccrp.sHtML

[R41] 丢弃输出
来源：http://baike.vehdjk.com/Article/details/giknhrjjw.sHtML

cmd >/dev/null 2>&1
来源：http://wap.vehdjk.com/Article/details/gnndyxywf.sHtML

[R42] 输入重定向
来源：http://m.share.tarul.cn/Article/details/geimgvgwr.sHtML

wc -l < a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gzckufihk.sHtML

[R43] 按名字查找文件
来源：http://mobile.yfazqb.com/Article/details/gbekidyrc.sHtML

find . -name "*.log" -type f
来源：http://m.share.bbcook.cn/Article/details/gbjqruwhs.sHtML

[R44] 按修改时间查找
来源：http://m.share.fktsv.cn/Article/details/gaxwglhsf.sHtML

find . -mtime -7 -type f
来源：http://read.share.sjlbkw.cn/Article/details/gbnqfnumb.sHtML

[R45] 批量删除
来源：http://baike.vehdjk.com/Article/details/guutxfslw.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.epnwcf.com/Article/details/gbcspkiyt.sHtML

[R46] 递归替换文件内容
来源：http://mobile.epnwcf.com/Article/details/grblfkdns.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fktsv.cn/Article/details/geifzcttv.sHtML

[R47] sed 单行替换
来源：http://wap.vehdjk.com/Article/details/gaaeydyll.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/ghbzywecd.sHtML

[R48] awk 取指定列
来源：http://blog.epnwcf.com/Article/details/gxjzdmzlf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gyezqlhek.sHtML

[R49] awk 带条件
来源：http://www.blog.epnwcf.com/Article/details/gpndwmnps.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.bbcook.cn/Article/details/gkbnzpkab.sHtML

[R50] awk 求和
来源：http://www.share.vehdjk.com/Article/details/gnmnjwnvk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/giqtxekhq.sHtML

[R51] 排序去重取前几
来源：http://www.share.yfazqb.com/Article/details/gwhputexk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.epnwcf.com/Article/details/gytgduisp.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/gyhzlcpqx.sHtML

wc -l a.txt
来源：http://wap.tarul.cn/Article/details/gngpqinle.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/gekxtaolo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.sjlbkw.cn/Article/details/gnzufjizx.sHtML

[R54] 比较两个文件
来源：http://blog.vehdjk.com/Article/details/gjmalotug.sHtML

diff a.txt b.txt
来源：http://3g.fktsv.cn/Article/details/gljhkxihr.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/gfurenqrk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.vehdjk.com/Article/details/gepqlzlts.sHtML

[R56] 远程拷贝
来源：http://3g.sjlbkw.cn/Article/details/gyjsgbjdn.sHtML

scp file user@host:/path/
来源：http://blog.epnwcf.com/Article/details/gthapyllq.sHtML

[R57] 远程执行命令
来源：http://baike.vehdjk.com/Article/details/gvlzlooic.sHtML

ssh user@host 'uptime'
来源：http://www.blog.bbcook.cn/Article/details/gxhhcczdi.sHtML

[R58] 下载文件
来源：http://mobile.bbcook.cn/Article/details/giilrjrof.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.yfazqb.com/Article/details/gvdvpxpah.sHtML

[R59] 发 POST JSON
来源：http://wap.yfazqb.com/Article/details/gkigxbcsf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.yfazqb.com/Article/details/gqvpnuyfy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/gdcjtpmnr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.epnwcf.com/Article/details/gkfutkhtd.sHtML

[R61] 磁盘占用
来源：http://m.share.yfazqb.com/Article/details/gvlecdmdb.sHtML

df -h;  du -sh *
来源：http://mobile.bbcook.cn/Article/details/gvnyhyays.sHtML

[R62] 找最占空间的文件
来源：http://3g.sjlbkw.cn/Article/details/gctcmlabg.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.tarul.cn/Article/details/guwuqksik.sHtML

[R63] 内存与进程
来源：http://mobile.fktsv.cn/Article/details/gilhfhadp.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fktsv.cn/Article/details/gwgnmlveh.sHtML

[R64] 结束进程
来源：http://www.blog.tarul.cn/Article/details/gxuymfppe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.yfazqb.com/Article/details/gdgwtazge.sHtML

[R65] 查看端口占用
来源：http://read.share.epnwcf.com/Article/details/gfqsafapd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fktsv.cn/Article/details/gmchqjylw.sHtML

[R66] 定时任务
来源：http://3g.vehdjk.com/Article/details/gttfynxrj.sHtML

crontab -e;  crontab -l
来源：http://read.share.epnwcf.com/Article/details/glpzjqtdp.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.tarul.cn/Article/details/gjsgfpkam.sHtML

openssl rand -hex 16
来源：http://blog.bbcook.cn/Article/details/gfmferlsz.sHtML

[R68] 计算文件校验值
来源：http://m.share.vehdjk.com/Article/details/gcqfrbfve.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.vehdjk.com/Article/details/grykzzouy.sHtML

[R69] 生成随机密码
来源：http://mobile.sjlbkw.cn/Article/details/gmsrnzcaq.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/gztwdzebo.sHtML

[R70] 时间戳与互转
来源：http://www.blog.tarul.cn/Article/details/grykqnhur.sHtML

date +%s;  date -d @1700000000
来源：http://blog.sjlbkw.cn/Article/details/gurjbtyhf.sHtML

[R71] 日期格式化
来源：http://m.share.sjlbkw.cn/Article/details/ggvamobvb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.sjlbkw.cn/Article/details/grbocfjew.sHtML

[R72] 等待端口就绪
来源：http://read.share.vehdjk.com/Article/details/gkuvbnbnp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/ghbofxyqx.sHtML

[R73] 分割大日志
来源：http://www.blog.fktsv.cn/Article/details/gojwmbwjg.sHtML

split -l 1000 big.log part_
来源：http://wap.bbcook.cn/Article/details/gwxofqbfd.sHtML

[R74] 批量重命名
来源：http://wap.vehdjk.com/Article/details/gerwnljxp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.bbcook.cn/Article/details/giklvinaf.sHtML

[R75] 导出环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gqzaxrucf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.bbcook.cn/Article/details/gdxifhrtb.sHtML

[R76] 使用临时文件
来源：http://m.share.vehdjk.com/Article/details/gmvuaiwxr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/gwwrcbcto.sHtML

[R77] 读取用户输入
来源：http://3g.fktsv.cn/Article/details/gogweozng.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/ggqaxczcu.sHtML

[R78] 交互式菜单
来源：http://www.blog.yfazqb.com/Article/details/ghcdhibkp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.sjlbkw.cn/Article/details/gyttygefb.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.vehdjk.com/Article/details/grpmmfvfd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/gxdiygcxk.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.yfazqb.com/Article/details/gjhvdkttl.sHtML

time ./run.sh
来源：http://baike.fktsv.cn/Article/details/gmuohcccw.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtedpribb.sHtML

S. C / C++ 专题
来源：http://blog.sjlbkw.cn/Article/details/gfuilnjex.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gxadpoxov.sHtML

[S01] C：Hello World
来源：http://blog.epnwcf.com/Article/details/ggytpsxzb.sHtML

#include <stdio.h>
来源：http://read.share.epnwcf.com/Article/details/gjbzgxybg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.bbcook.cn/Article/details/gpjryznpl.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/gmwucqcks.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fktsv.cn/Article/details/gcaexravc.sHtML

[S03] C：读入整数
来源：http://m.share.bbcook.cn/Article/details/gczpxfghm.sHtML


<!-- 参考信息 -->