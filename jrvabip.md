代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.epnwcf.com/Article/details/glprhruld.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.bbcook.cn/Article/details/gqwyofcdc.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.tarul.cn/Article/details/gunhwxgbw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fktsv.cn/Article/details/gxwbreeap.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/gzvzrrscb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.tarul.cn/Article/details/gtznpjnja.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.vehdjk.com/Article/details/ggmgtxvsd.sHtML

[Q41] 多表连接
来源：http://www.m.share.bbcook.cn/Article/details/gtyzlpnvq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.bbcook.cn/Article/details/gblkhpxbm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.vehdjk.com/Article/details/gjmxmvbny.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gwxnjnbrb.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.epnwcf.com/Article/details/gfetgdtyv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.epnwcf.com/Article/details/gbisktuph.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.bbcook.cn/Article/details/ggownekqy.sHtML

[Q43] 标量子查询
来源：http://3g.tarul.cn/Article/details/gajwscgbg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.epnwcf.com/Article/details/ghztdkpvu.sHtML

[Q44] IN 子查询
来源：http://baike.bbcook.cn/Article/details/gitjcpvde.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.yfazqb.com/Article/details/gkqefpaur.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.yfazqb.com/Article/details/glaijjhws.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gygrfirrd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.bbcook.cn/Article/details/gsecptudo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gwepnheqv.sHtML

[Q47] 与平均值比较
来源：http://www.blog.tarul.cn/Article/details/gnvmpcrbf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fktsv.cn/Article/details/gomglnmrg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gkzqnqtgh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fktsv.cn/Article/details/ggrcnzsdw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsemdwig.sHtML

[Q49] 更新单行
来源：http://baike.yfazqb.com/Article/details/gknfjjbyn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gjnrdshjj.sHtML

[Q50] 批量更新
来源：http://read.share.epnwcf.com/Article/details/gbuuqdpwn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gtitfdwos.sHtML

[Q51] 用子查询更新
来源：http://3g.yfazqb.com/Article/details/gxitdbrbb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.vehdjk.com/Article/details/grcgcbjyl.sHtML

[Q52] 删除指定行
来源：http://3g.tarul.cn/Article/details/gnnnnvpak.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/gglbgbvjo.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fktsv.cn/Article/details/gqyksgpbg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.yfazqb.com/Article/details/gsamjrrgf.sHtML

[Q54] 清空表
来源：http://mobile.yfazqb.com/Article/details/gynjuzsdj.sHtML

TRUNCATE TABLE logs;
来源：http://3g.yfazqb.com/Article/details/gozvfoluz.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gldkxblpo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fktsv.cn/Article/details/gzunvprjx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.yfazqb.com/Article/details/gituzilvm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gzqjuiapa.sHtML

[Q57] 行号
来源：http://blog.sjlbkw.cn/Article/details/gzvcgygzx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.tarul.cn/Article/details/gjvswkanr.sHtML

[Q58] 累计求和
来源：http://www.m.share.vehdjk.com/Article/details/gpzgukspx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.yfazqb.com/Article/details/gszwpjwth.sHtML

[Q59] 分组内累计
来源：http://3g.vehdjk.com/Article/details/gwzqbjsbs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gvosdpgto.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.bbcook.cn/Article/details/gybirccov.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.tarul.cn/Article/details/gcvantrgm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.epnwcf.com/Article/details/grbugzwbs.sHtML

[Q61] 移动平均
来源：http://read.share.tarul.cn/Article/details/gplyqgvwd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gmvoxbhuv.sHtML

[Q62] 分组占比
来源：http://m.share.epnwcf.com/Article/details/gquybyaks.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gjefpoxqu.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/gtczeeipt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.yfazqb.com/Article/details/gsukyqzvr.sHtML

[Q64] 提交事务
来源：http://wap.yfazqb.com/Article/details/gnbybjzsk.sHtML

COMMIT;
来源：http://read.share.bbcook.cn/Article/details/gyahpyrbt.sHtML

[Q65] 回滚事务
来源：http://blog.vehdjk.com/Article/details/gneqigski.sHtML

ROLLBACK;
来源：http://read.share.epnwcf.com/Article/details/gsywcgnsf.sHtML

[Q66] 行锁查询
来源：http://3g.vehdjk.com/Article/details/ggqfuynpo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.yfazqb.com/Article/details/gffzxciys.sHtML

[Q67] 设置隔离级别
来源：http://read.share.tarul.cn/Article/details/gbbkypxaj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.yfazqb.com/Article/details/gaagoekwe.sHtML

[Q68] 保存点
来源：http://www.blog.epnwcf.com/Article/details/gxivgzyap.sHtML

SAVEPOINT sp1;
来源：http://m.share.vehdjk.com/Article/details/gdopwqgqb.sHtML

ROLLBACK TO sp1;
来源：http://3g.yfazqb.com/Article/details/guwrzrvzm.sHtML

[Q69] 查看执行计划
来源：http://blog.yfazqb.com/Article/details/grdmndtps.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.tarul.cn/Article/details/gzitvejav.sHtML

[Q70] 更新统计信息
来源：http://wap.yfazqb.com/Article/details/guncekpvg.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.vehdjk.com/Article/details/gvrtxrlfo.sHtML

[Q71] 查看建表语句
来源：http://www.share.epnwcf.com/Article/details/gymdjfahv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.bbcook.cn/Article/details/gkqeczpfd.sHtML

[Q72] 查看索引
来源：http://3g.vehdjk.com/Article/details/gcujgkugx.sHtML

SHOW INDEX FROM users;
来源：http://mobile.tarul.cn/Article/details/giqjdhgwl.sHtML

[Q73] 查看表状态
来源：http://mobile.fktsv.cn/Article/details/gciuohfsj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gvawxhlxi.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fktsv.cn/Article/details/gsutfwrar.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.vehdjk.com/Article/details/gsrshfsut.sHtML

[Q75] 日期格式化
来源：http://3g.fktsv.cn/Article/details/ghjgyqeae.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.vehdjk.com/Article/details/guycuprbj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fktsv.cn/Article/details/gyszxqzgt.sHtML

[Q76] 按天统计
来源：http://mobile.vehdjk.com/Article/details/grhljhvpm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.epnwcf.com/Article/details/gkphrpynf.sHtML

[Q77] 时间加减
来源：http://mobile.bbcook.cn/Article/details/ggirlsciv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.epnwcf.com/Article/details/gyjaojhpt.sHtML

[Q78] 当前时间
来源：http://m.share.fktsv.cn/Article/details/gcsimkkbj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.bbcook.cn/Article/details/gbnpeecjl.sHtML

[Q79] 字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gzjpybfpm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcczxmmk.sHtML

[Q80] 字符串截取
来源：http://baike.sjlbkw.cn/Article/details/gpwzlnepp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gzlgufuea.sHtML

[Q81] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gmyiyfbez.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/ghsdcmgdd.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.vehdjk.com/Article/details/gqgpptobh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.tarul.cn/Article/details/ggqaidtxe.sHtML

[Q83] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gidtiqqdb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/guozdlpug.sHtML

[Q84] 去除首尾空格
来源：http://mobile.yfazqb.com/Article/details/gtbrsgcfk.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gxxnlarot.sHtML

[Q85] 数值取整
来源：http://blog.tarul.cn/Article/details/gvhulrggq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.epnwcf.com/Article/details/gxrqczisg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.tarul.cn/Article/details/gvlkotqar.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.bbcook.cn/Article/details/geihlmebn.sHtML

[Q87] JSON 字段做条件
来源：http://wap.epnwcf.com/Article/details/gcfydxxrt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.sjlbkw.cn/Article/details/gylizjsby.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.bbcook.cn/Article/details/gvjxysdrq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.bbcook.cn/Article/details/gkcjeshax.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gtdwbewvz.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.tarul.cn/Article/details/gluoyljuu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.vehdjk.com/Article/details/grztsytex.sHtML

[Q90] 生成序号列
来源：http://blog.tarul.cn/Article/details/gqclnsgns.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/globabyjf.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grwdiqgni.sHtML

R. Bash 专题
来源：http://www.blog.tarul.cn/Article/details/gddqbdoyv.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsfazohty.sHtML

[R01] shebang 与严格模式
来源：http://read.share.tarul.cn/Article/details/gtuyepxzy.sHtML

#!/usr/bin/env bash
来源：http://www.share.bbcook.cn/Article/details/gszghtuui.sHtML

set -euo pipefail
来源：http://blog.vehdjk.com/Article/details/gidoczkpt.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.tarul.cn/Article/details/gnzgicweb.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.epnwcf.com/Article/details/gljdarwqn.sHtML

[R03] 只读变量
来源：http://mobile.fktsv.cn/Article/details/gkmvgygtv.sHtML

readonly PI=3.14
来源：http://m.share.yfazqb.com/Article/details/gblawrsit.sHtML

[R04] 位置参数
来源：http://read.share.bbcook.cn/Article/details/gaatryygl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.tarul.cn/Article/details/gudarkebj.sHtML

[R05] 参数默认值
来源：http://read.share.tarul.cn/Article/details/gsdhrinim.sHtML

name="${1:-default}"
来源：http://wap.sjlbkw.cn/Article/details/gxssbjioe.sHtML

[R06] 判断命令是否存在
来源：http://m.share.tarul.cn/Article/details/gxjisosev.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.vehdjk.com/Article/details/godwkiyua.sHtML

[R07] if 判断文件
来源：http://3g.tarul.cn/Article/details/gfvqtekaj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.vehdjk.com/Article/details/ggpneyjsl.sHtML

[R08] 数值比较
来源：http://read.share.fktsv.cn/Article/details/gxwldmeaj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gfhelziia.sHtML

[R09] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/gdcozejqg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.bbcook.cn/Article/details/gogcdwllq.sHtML

[R10] 正则匹配
来源：http://read.share.epnwcf.com/Article/details/goaxiruta.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/gvksdcsif.sHtML

[R11] case 多分支
来源：http://baike.bbcook.cn/Article/details/gkbwdbqrn.sHtML

case "$1" in
来源：http://www.share.vehdjk.com/Article/details/gbxgdvaih.sHtML

start) echo "启动" ;;
来源：http://wap.vehdjk.com/Article/details/gpsqpvtlk.sHtML

stop)  echo "停止" ;;
来源：http://wap.epnwcf.com/Article/details/gkjlvbkoe.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gliowgsoj.sHtML

esac
来源：http://www.m.share.bbcook.cn/Article/details/glizvsvpw.sHtML

[R12] for 遍历文件
来源：http://www.share.bbcook.cn/Article/details/gryspholy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.sjlbkw.cn/Article/details/guluhgvlf.sHtML

[R13] for 计数循环
来源：http://3g.tarul.cn/Article/details/ghrkskubw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gcadcbxgj.sHtML

[R14] C 风格 for
来源：http://m.share.tarul.cn/Article/details/gqoxjzvkg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/gdvhhmnrc.sHtML

[R15] while 逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/ghcbnymwi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.sjlbkw.cn/Article/details/gepmhgwqm.sHtML

[R16] until 等待条件
来源：http://3g.sjlbkw.cn/Article/details/gorqyhjux.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.sjlbkw.cn/Article/details/giokufoeu.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.vehdjk.com/Article/details/gogfwkrjv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.yfazqb.com/Article/details/gvhrsmxlv.sHtML

[R18] 遍历数组
来源：http://www.blog.tarul.cn/Article/details/gmzuuxxfz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.bbcook.cn/Article/details/gkmlpbscu.sHtML

[R19] 数组长度
来源：http://wap.tarul.cn/Article/details/gdukgcklq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.yfazqb.com/Article/details/gtztmopai.sHtML

[R20] 关联数组（字典）
来源：http://read.share.sjlbkw.cn/Article/details/gvewwwubm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/gvhpxucxx.sHtML

[R21] 字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/goavxkxgy.sHtML

echo "${#s}"
来源：http://mobile.vehdjk.com/Article/details/gcbppvebc.sHtML

[R22] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gdvxdsitv.sHtML

echo "${s:0:5}"
来源：http://baike.fktsv.cn/Article/details/gqaccvipm.sHtML

[R23] 字符串替换
来源：http://wap.fktsv.cn/Article/details/gnvwfkyyp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.yfazqb.com/Article/details/ghwqmdcfe.sHtML

[R24] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gkjbtflgm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.vehdjk.com/Article/details/gktuiuugc.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.sjlbkw.cn/Article/details/gqslrnysw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.tarul.cn/Article/details/gpmrdxfrr.sHtML

[R26] 命令替换
来源：http://read.share.sjlbkw.cn/Article/details/gazesxafy.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.vehdjk.com/Article/details/gssaotkyn.sHtML

[R27] 算术展开
来源：http://blog.bbcook.cn/Article/details/guvbzofaa.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fktsv.cn/Article/details/giqovpqqq.sHtML

[R28] 浮点运算
来源：http://blog.sjlbkw.cn/Article/details/gpwyyrazv.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.epnwcf.com/Article/details/gxfhgkbmh.sHtML

[R29] 定义函数
来源：http://www.share.bbcook.cn/Article/details/gldwtrham.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.sjlbkw.cn/Article/details/gbskfigsk.sHtML

[R30] 函数返回状态码
来源：http://blog.sjlbkw.cn/Article/details/glaejqfui.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fktsv.cn/Article/details/gfwlcrhny.sHtML

[R31] 局部变量
来源：http://www.blog.tarul.cn/Article/details/ggmsrkwxs.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.sjlbkw.cn/Article/details/gerywysbr.sHtML

[R32] 参数个数校验
来源：http://baike.fktsv.cn/Article/details/gbecrosfy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gtvgxxsgv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.tarul.cn/Article/details/goyuwdycw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.bbcook.cn/Article/details/gyqrelxdx.sHtML

[R34] 退出时清理
来源：http://www.blog.vehdjk.com/Article/details/godzkqsle.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/guxdillsy.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fktsv.cn/Article/details/gvgbcadkl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.sjlbkw.cn/Article/details/gckbfhvmt.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.vehdjk.com/Article/details/gpawuwonc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.yfazqb.com/Article/details/geiyxdhsy.sHtML

[R37] 把输出赋给变量
来源：http://3g.fktsv.cn/Article/details/gcplwoykk.sHtML

files=$(ls -1)
来源：http://baike.yfazqb.com/Article/details/gwfolrsqd.sHtML

[R38] 管道串联
来源：http://www.m.share.vehdjk.com/Article/details/gkyvqgztr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.vehdjk.com/Article/details/gfyvycxco.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/gcwnzdmwf.sHtML

cmd > out.log 2>&1
来源：http://www.share.yfazqb.com/Article/details/giztgyobl.sHtML

[R40] 追加写日志
来源：http://wap.epnwcf.com/Article/details/gelpykwan.sHtML

echo "log" >> out.log
来源：http://mobile.epnwcf.com/Article/details/gwfgtnizp.sHtML

[R41] 丢弃输出
来源：http://m.share.sjlbkw.cn/Article/details/gzgiulgus.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/gjxrypcrb.sHtML

[R42] 输入重定向
来源：http://m.share.fktsv.cn/Article/details/grkczgolr.sHtML

wc -l < a.txt
来源：http://www.share.yfazqb.com/Article/details/gaajgqeiq.sHtML

[R43] 按名字查找文件
来源：http://mobile.vehdjk.com/Article/details/gckaihwku.sHtML

find . -name "*.log" -type f
来源：http://www.share.tarul.cn/Article/details/gsactxksg.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/glklnvwan.sHtML

find . -mtime -7 -type f
来源：http://wap.fktsv.cn/Article/details/gtwokcwbi.sHtML

[R45] 批量删除
来源：http://m.share.fktsv.cn/Article/details/gnlnvtsgj.sHtML

find . -name "*.tmp" -delete
来源：http://blog.vehdjk.com/Article/details/ghqcknlel.sHtML

[R46] 递归替换文件内容
来源：http://baike.bbcook.cn/Article/details/gzjtnqzff.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.bbcook.cn/Article/details/ggeothhpu.sHtML

[R47] sed 单行替换
来源：http://www.blog.epnwcf.com/Article/details/goxxgyjnn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.epnwcf.com/Article/details/gaijkevaw.sHtML

[R48] awk 取指定列
来源：http://mobile.sjlbkw.cn/Article/details/gkymxiwka.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.tarul.cn/Article/details/gocwbaeco.sHtML

[R49] awk 带条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrkhtydd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.epnwcf.com/Article/details/gcgvosfyy.sHtML

[R50] awk 求和
来源：http://blog.tarul.cn/Article/details/gzoyczklr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gdtzvrkbz.sHtML

[R51] 排序去重取前几
来源：http://baike.vehdjk.com/Article/details/gmrzbvpma.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsfqzllt.sHtML

[R52] 统计行数
来源：http://mobile.tarul.cn/Article/details/gwqygynts.sHtML

wc -l a.txt
来源：http://blog.yfazqb.com/Article/details/gzxglsvgm.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.bbcook.cn/Article/details/gqxjqpvpq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gbrnevsxu.sHtML

[R54] 比较两个文件
来源：http://mobile.epnwcf.com/Article/details/grwvdqaun.sHtML

diff a.txt b.txt
来源：http://m.share.epnwcf.com/Article/details/gkknhuixi.sHtML

[R55] 压缩与解压
来源：http://mobile.epnwcf.com/Article/details/gnanlzgzq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/grztsaxgx.sHtML

[R56] 远程拷贝
来源：http://baike.yfazqb.com/Article/details/gjrpnviwr.sHtML

scp file user@host:/path/
来源：http://www.m.share.bbcook.cn/Article/details/grhjwgtyh.sHtML

[R57] 远程执行命令
来源：http://read.share.tarul.cn/Article/details/ggfdgulse.sHtML

ssh user@host 'uptime'
来源：http://read.share.bbcook.cn/Article/details/gqmtldpdw.sHtML

[R58] 下载文件
来源：http://blog.fktsv.cn/Article/details/gbvbquhua.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.bbcook.cn/Article/details/grhzunhao.sHtML

[R59] 发 POST JSON
来源：http://baike.bbcook.cn/Article/details/gfpkkliid.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.bbcook.cn/Article/details/gdrgdjlym.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gyngidmuk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.yfazqb.com/Article/details/gvpwzdhlv.sHtML

[R61] 磁盘占用
来源：http://read.share.tarul.cn/Article/details/gsqsqtjrg.sHtML

df -h;  du -sh *
来源：http://baike.bbcook.cn/Article/details/glhubpuyg.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.yfazqb.com/Article/details/gvlkuxqru.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.epnwcf.com/Article/details/goevuuwfy.sHtML

[R63] 内存与进程
来源：http://baike.bbcook.cn/Article/details/ghrprwwny.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.sjlbkw.cn/Article/details/gnozmmdph.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/gepcxgshw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/gkvblotdz.sHtML

[R65] 查看端口占用
来源：http://blog.tarul.cn/Article/details/gvqypbxgr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.epnwcf.com/Article/details/gfewxaqzq.sHtML

[R66] 定时任务
来源：http://m.share.bbcook.cn/Article/details/gckecdnhp.sHtML

crontab -e;  crontab -l
来源：http://baike.sjlbkw.cn/Article/details/gjkpkqgfb.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.bbcook.cn/Article/details/gsyjuhrcp.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/gcydsrqxf.sHtML

[R68] 计算文件校验值
来源：http://blog.bbcook.cn/Article/details/gjsueomlx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fktsv.cn/Article/details/gmrbocqwy.sHtML

[R69] 生成随机密码
来源：http://blog.tarul.cn/Article/details/gmxackvxn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.yfazqb.com/Article/details/gwftyjxbg.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/gofhmvvoq.sHtML

date +%s;  date -d @1700000000
来源：http://blog.tarul.cn/Article/details/gzteazbaj.sHtML

[R71] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gaoaqbetb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.yfazqb.com/Article/details/gpiaubbvn.sHtML

[R72] 等待端口就绪
来源：http://baike.vehdjk.com/Article/details/gbcndlrtw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/gffawbwzr.sHtML

[R73] 分割大日志
来源：http://baike.epnwcf.com/Article/details/gmhxctpab.sHtML

split -l 1000 big.log part_
来源：http://m.share.tarul.cn/Article/details/gvgyagtmu.sHtML

[R74] 批量重命名
来源：http://www.m.share.fktsv.cn/Article/details/gnduzclmx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fktsv.cn/Article/details/gqfhjwjri.sHtML

[R75] 导出环境变量
来源：http://www.share.yfazqb.com/Article/details/gerdxyvxv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/gmzkpassc.sHtML

[R76] 使用临时文件
来源：http://www.blog.yfazqb.com/Article/details/gcsjztyvk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/gdtsofumz.sHtML

[R77] 读取用户输入
来源：http://read.share.bbcook.cn/Article/details/gdmtilthd.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.bbcook.cn/Article/details/ggxiyksxy.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fktsv.cn/Article/details/girtiktfw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/gryjkmwfv.sHtML

[R79] 解析命令行选项
来源：http://read.share.epnwcf.com/Article/details/gxaqrjabo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.bbcook.cn/Article/details/gzztezvfe.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.epnwcf.com/Article/details/gttwkqbuw.sHtML

time ./run.sh
来源：http://www.share.fktsv.cn/Article/details/gwivxcund.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvgysogke.sHtML

S. C / C++ 专题
来源：http://blog.tarul.cn/Article/details/gjfcyjyij.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gofofszjj.sHtML

[S01] C：Hello World
来源：http://read.share.tarul.cn/Article/details/gpevyipmp.sHtML

#include <stdio.h>
来源：http://blog.vehdjk.com/Article/details/gzifnmloa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fktsv.cn/Article/details/gtorhhpvf.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.bbcook.cn/Article/details/gkjumfbvk.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fktsv.cn/Article/details/gsywsrlnx.sHtML

[S03] C：读入整数
来源：http://3g.sjlbkw.cn/Article/details/gygzmauqb.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gzyiersvm.sHtML

[S04] C：字符串复制
来源：http://www.share.fktsv.cn/Article/details/gaubojspa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.yfazqb.com/Article/details/gvxaybohk.sHtML

[S05] C：字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/givruqoso.sHtML

strlen(s)
来源：http://blog.epnwcf.com/Article/details/gdaxamscv.sHtML

[S06] C：字符串比较
来源：http://m.share.vehdjk.com/Article/details/grwjmngze.sHtML

strcmp(a, b) == 0
来源：http://www.share.yfazqb.com/Article/details/gylxrjarq.sHtML

[S07] C：数组遍历求和
来源：http://wap.vehdjk.com/Article/details/guabyjedd.sHtML


<!-- 参考信息 -->