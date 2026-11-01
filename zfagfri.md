代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.epnwcf.com/Article/details/gxzrlbanz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.tarul.cn/Article/details/ggavqfkqu.sHtML

[Q43] 标量子查询
来源：http://read.share.sjlbkw.cn/Article/details/gicagnrlg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fktsv.cn/Article/details/gzvztkgid.sHtML

[Q44] IN 子查询
来源：http://read.share.fktsv.cn/Article/details/gygyvlnih.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/gujtbywmg.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.yfazqb.com/Article/details/gkkkspwiv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/gbxtnaxpm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fktsv.cn/Article/details/gbdapwwaj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.epnwcf.com/Article/details/gsucptmht.sHtML

[Q47] 与平均值比较
来源：http://m.share.fktsv.cn/Article/details/gqgqmzpad.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.epnwcf.com/Article/details/gayzbehqr.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.bbcook.cn/Article/details/gxkgikwhh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fktsv.cn/Article/details/glkymzxqe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/gorblngxv.sHtML

[Q49] 更新单行
来源：http://read.share.fktsv.cn/Article/details/gslsmlnnb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/gaufnsuzf.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/gzymotjdv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fktsv.cn/Article/details/gjhaiwisl.sHtML

[Q51] 用子查询更新
来源：http://mobile.fktsv.cn/Article/details/gwayfmsqa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.vehdjk.com/Article/details/gylyedhmc.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/gbsahhuzb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gkfqfnstt.sHtML

[Q53] 按条件删除
来源：http://baike.fktsv.cn/Article/details/ggbmahsej.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.tarul.cn/Article/details/gdvhrymys.sHtML

[Q54] 清空表
来源：http://www.m.share.fktsv.cn/Article/details/gqlzzwosl.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.epnwcf.com/Article/details/goyyvcjll.sHtML

[Q55] 排名（并列占位）
来源：http://3g.sjlbkw.cn/Article/details/gqygeeyqq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.yfazqb.com/Article/details/gwrjywuql.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.epnwcf.com/Article/details/gmclldksv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.epnwcf.com/Article/details/gqtklxfgc.sHtML

[Q57] 行号
来源：http://mobile.sjlbkw.cn/Article/details/gszeyvglv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gemkodobg.sHtML

[Q58] 累计求和
来源：http://mobile.vehdjk.com/Article/details/gdlhcgvig.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gxcuvymjd.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/glgzjnfxi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.vehdjk.com/Article/details/gaprtwvvw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.sjlbkw.cn/Article/details/gtoligibp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.bbcook.cn/Article/details/gmedberqp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.tarul.cn/Article/details/gszvraiis.sHtML

[Q61] 移动平均
来源：http://www.share.tarul.cn/Article/details/gtvmvzlcy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gvhtteknf.sHtML

[Q62] 分组占比
来源：http://3g.fktsv.cn/Article/details/gaqmegixf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/ghpqrubbu.sHtML

[Q63] 开启事务
来源：http://baike.fktsv.cn/Article/details/gvbonreqa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.epnwcf.com/Article/details/gzsfzpigw.sHtML

[Q64] 提交事务
来源：http://wap.tarul.cn/Article/details/ghhvikohl.sHtML

COMMIT;
来源：http://www.blog.epnwcf.com/Article/details/gacbadour.sHtML

[Q65] 回滚事务
来源：http://www.m.share.yfazqb.com/Article/details/gnswfcsap.sHtML

ROLLBACK;
来源：http://wap.vehdjk.com/Article/details/gzeczauij.sHtML

[Q66] 行锁查询
来源：http://m.share.tarul.cn/Article/details/gvariumaw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.yfazqb.com/Article/details/gacantexl.sHtML

[Q67] 设置隔离级别
来源：http://wap.sjlbkw.cn/Article/details/gdmukccmv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.bbcook.cn/Article/details/gukgbbgow.sHtML

[Q68] 保存点
来源：http://read.share.vehdjk.com/Article/details/gvwkomzed.sHtML

SAVEPOINT sp1;
来源：http://www.share.fktsv.cn/Article/details/grjefshdm.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.yfazqb.com/Article/details/gvdjwggxa.sHtML

[Q69] 查看执行计划
来源：http://m.share.sjlbkw.cn/Article/details/gskjfihjw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/gpznfdxim.sHtML

[Q70] 更新统计信息
来源：http://mobile.vehdjk.com/Article/details/gpzodatgv.sHtML

ANALYZE TABLE users;
来源：http://www.share.tarul.cn/Article/details/giohayvhh.sHtML

[Q71] 查看建表语句
来源：http://www.share.epnwcf.com/Article/details/gcceaaxgr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.vehdjk.com/Article/details/gjxdqscdw.sHtML

[Q72] 查看索引
来源：http://www.m.share.yfazqb.com/Article/details/gjjtqblra.sHtML

SHOW INDEX FROM users;
来源：http://m.share.bbcook.cn/Article/details/gryxxrygl.sHtML

[Q73] 查看表状态
来源：http://baike.vehdjk.com/Article/details/gsebypvzw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.sjlbkw.cn/Article/details/gvrnakahu.sHtML

[Q74] 强制使用索引
来源：http://www.blog.yfazqb.com/Article/details/gzgnnqouc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.sjlbkw.cn/Article/details/gmujeziun.sHtML

[Q75] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gusafoerx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjdnbwkn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.yfazqb.com/Article/details/gjblugunv.sHtML

[Q76] 按天统计
来源：http://3g.sjlbkw.cn/Article/details/gyrufwfmb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.sjlbkw.cn/Article/details/gfqtvhboh.sHtML

[Q77] 时间加减
来源：http://m.share.vehdjk.com/Article/details/gfebyxhmy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/gpiahgjnq.sHtML

[Q78] 当前时间
来源：http://wap.sjlbkw.cn/Article/details/goqultakq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.epnwcf.com/Article/details/gdxheaznn.sHtML

[Q79] 字符串拼接
来源：http://3g.fktsv.cn/Article/details/gbmfratcm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.tarul.cn/Article/details/gtsexgbrf.sHtML

[Q80] 字符串截取
来源：http://3g.yfazqb.com/Article/details/ghjgbnrrz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gpjjypqjd.sHtML

[Q81] 字符串替换
来源：http://blog.tarul.cn/Article/details/gbbgtytbq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.vehdjk.com/Article/details/gwyvktkdr.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.tarul.cn/Article/details/gtezbdnbu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gphhwkoik.sHtML

[Q83] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gwujknrzc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gdyymbwki.sHtML

[Q84] 去除首尾空格
来源：http://blog.tarul.cn/Article/details/gpznjrpfc.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/grdgmsyll.sHtML

[Q85] 数值取整
来源：http://wap.fktsv.cn/Article/details/ggxanpslp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.bbcook.cn/Article/details/gyltpnzhu.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.vehdjk.com/Article/details/gdnrqaubw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fktsv.cn/Article/details/grkzxmuei.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/gsiuknsrf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.epnwcf.com/Article/details/gioipqjvb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.sjlbkw.cn/Article/details/gxoqsailk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fktsv.cn/Article/details/gdkwinwxh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gzsdtpxlf.sHtML

[Q89] 判断表是否存在
来源：http://m.share.vehdjk.com/Article/details/gnpgyghfy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.bbcook.cn/Article/details/gxcivytml.sHtML

[Q90] 生成序号列
来源：http://wap.fktsv.cn/Article/details/ggobuwacy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fktsv.cn/Article/details/gftayltuj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/guejmsiuv.sHtML

R. Bash 专题
来源：http://baike.vehdjk.com/Article/details/guiujdhmk.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjnwctoly.sHtML

[R01] shebang 与严格模式
来源：http://read.share.tarul.cn/Article/details/guvfgqdag.sHtML

#!/usr/bin/env bash
来源：http://3g.tarul.cn/Article/details/grmiqayjj.sHtML

set -euo pipefail
来源：http://wap.tarul.cn/Article/details/gpcsuhvvz.sHtML

[R02] 变量赋值与使用
来源：http://3g.tarul.cn/Article/details/ghnbctbrd.sHtML

name="Tom"; echo "$name"
来源：http://www.share.sjlbkw.cn/Article/details/gwkefprxz.sHtML

[R03] 只读变量
来源：http://read.share.sjlbkw.cn/Article/details/gpptssxec.sHtML

readonly PI=3.14
来源：http://mobile.fktsv.cn/Article/details/gmkopbukv.sHtML

[R04] 位置参数
来源：http://m.share.bbcook.cn/Article/details/gsrvmhjgw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.bbcook.cn/Article/details/gzxupfiqk.sHtML

[R05] 参数默认值
来源：http://www.share.yfazqb.com/Article/details/guqnupkwf.sHtML

name="${1:-default}"
来源：http://mobile.sjlbkw.cn/Article/details/gtevlbnft.sHtML

[R06] 判断命令是否存在
来源：http://3g.sjlbkw.cn/Article/details/gnhtjwulj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.vehdjk.com/Article/details/gjkdyfjwp.sHtML

[R07] if 判断文件
来源：http://m.share.vehdjk.com/Article/details/gjkuoraup.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.tarul.cn/Article/details/gqufdlwuh.sHtML

[R08] 数值比较
来源：http://mobile.bbcook.cn/Article/details/gshdguiza.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.vehdjk.com/Article/details/gmayszzgf.sHtML

[R09] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/gvqtasvhe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.sjlbkw.cn/Article/details/gbxtkfibg.sHtML

[R10] 正则匹配
来源：http://www.m.share.bbcook.cn/Article/details/gnwwzddva.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.bbcook.cn/Article/details/gamejibjn.sHtML

[R11] case 多分支
来源：http://3g.bbcook.cn/Article/details/gysyenloo.sHtML

case "$1" in
来源：http://www.m.share.fktsv.cn/Article/details/gvoznrfjk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gnwdjfmiq.sHtML

stop)  echo "停止" ;;
来源：http://mobile.bbcook.cn/Article/details/gizvdbqux.sHtML

*)     echo "未知命令" ;;
来源：http://blog.sjlbkw.cn/Article/details/glcgfuxrc.sHtML

esac
来源：http://wap.vehdjk.com/Article/details/gsxnmzaqf.sHtML

[R12] for 遍历文件
来源：http://blog.fktsv.cn/Article/details/gmxseexqn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.yfazqb.com/Article/details/gfefhqwyj.sHtML

[R13] for 计数循环
来源：http://blog.bbcook.cn/Article/details/germnawud.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gqimpecxq.sHtML

[R14] C 风格 for
来源：http://m.share.sjlbkw.cn/Article/details/gbykuixor.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/gakmmxgki.sHtML

[R15] while 逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gtgrxklps.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.sjlbkw.cn/Article/details/gymjwmstn.sHtML

[R16] until 等待条件
来源：http://mobile.vehdjk.com/Article/details/guqhixfku.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gvpybotkx.sHtML

[R17] 数组定义与取值
来源：http://baike.vehdjk.com/Article/details/glwnkkzkm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fktsv.cn/Article/details/gdkuctfsz.sHtML

[R18] 遍历数组
来源：http://read.share.bbcook.cn/Article/details/gcwsyylje.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.tarul.cn/Article/details/gtdvayemi.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gnmjwsebp.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.vehdjk.com/Article/details/giartzftf.sHtML

[R20] 关联数组（字典）
来源：http://m.share.epnwcf.com/Article/details/gsdjdmdle.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fktsv.cn/Article/details/gzuuguglp.sHtML

[R21] 字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gnozmfvmp.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gbxhnbjxk.sHtML

[R22] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbbjyrgc.sHtML

echo "${s:0:5}"
来源：http://mobile.vehdjk.com/Article/details/gdszfbntl.sHtML

[R23] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/golvucoin.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fktsv.cn/Article/details/gwlapdvtt.sHtML

[R24] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gcwocwmjd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.sjlbkw.cn/Article/details/grokijytz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.vehdjk.com/Article/details/gixscrjmw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fktsv.cn/Article/details/gxjjcmtpr.sHtML

[R26] 命令替换
来源：http://read.share.tarul.cn/Article/details/gwgezbior.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.bbcook.cn/Article/details/gnsrxxahx.sHtML

[R27] 算术展开
来源：http://baike.yfazqb.com/Article/details/gtjluowrc.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.bbcook.cn/Article/details/gjtbwhczy.sHtML

[R28] 浮点运算
来源：http://wap.sjlbkw.cn/Article/details/gltdiybwi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.bbcook.cn/Article/details/guhimlbog.sHtML

[R29] 定义函数
来源：http://blog.epnwcf.com/Article/details/glorzsbso.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gvhfjrnli.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gluksfxbu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.yfazqb.com/Article/details/gqnimedkr.sHtML

[R31] 局部变量
来源：http://www.share.yfazqb.com/Article/details/gwioqwbjq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.epnwcf.com/Article/details/gpzqdisig.sHtML

[R32] 参数个数校验
来源：http://www.m.share.bbcook.cn/Article/details/gwoovjyok.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/gxldupnzl.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fktsv.cn/Article/details/gamcnvbhl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.epnwcf.com/Article/details/gxtacqkxk.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gllxdtwsb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.bbcook.cn/Article/details/gctollwfx.sHtML

[R35] 后台执行并等待
来源：http://read.share.bbcook.cn/Article/details/gcuxspntd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.yfazqb.com/Article/details/gcdbnfaes.sHtML

[R36] 并发执行多个任务
来源：http://baike.fktsv.cn/Article/details/gykkqyvwh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.vehdjk.com/Article/details/gdkkyyurx.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.yfazqb.com/Article/details/gvetpugsa.sHtML

files=$(ls -1)
来源：http://mobile.fktsv.cn/Article/details/ggvgpnzzx.sHtML

[R38] 管道串联
来源：http://baike.bbcook.cn/Article/details/gcwihddnc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fktsv.cn/Article/details/gnpxsycjp.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fktsv.cn/Article/details/goukndlep.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/gvillhmny.sHtML

[R40] 追加写日志
来源：http://www.m.share.yfazqb.com/Article/details/gihultxfv.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/gnbdspeke.sHtML

[R41] 丢弃输出
来源：http://read.share.epnwcf.com/Article/details/gnacqepls.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gegymovmt.sHtML

[R42] 输入重定向
来源：http://www.blog.vehdjk.com/Article/details/ggdsfvqhu.sHtML

wc -l < a.txt
来源：http://blog.fktsv.cn/Article/details/gezizdyqy.sHtML

[R43] 按名字查找文件
来源：http://read.share.vehdjk.com/Article/details/gwnqgybfu.sHtML

find . -name "*.log" -type f
来源：http://www.share.fktsv.cn/Article/details/gisbjhjma.sHtML

[R44] 按修改时间查找
来源：http://mobile.fktsv.cn/Article/details/gmiqidwaz.sHtML

find . -mtime -7 -type f
来源：http://mobile.tarul.cn/Article/details/gknnscixh.sHtML

[R45] 批量删除
来源：http://baike.tarul.cn/Article/details/ggqymjknc.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.bbcook.cn/Article/details/gdtsdsuuj.sHtML

[R46] 递归替换文件内容
来源：http://wap.vehdjk.com/Article/details/gndkcflgf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.bbcook.cn/Article/details/gqtdhmfin.sHtML

[R47] sed 单行替换
来源：http://m.share.vehdjk.com/Article/details/gdopcecbs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fktsv.cn/Article/details/gismvphba.sHtML

[R48] awk 取指定列
来源：http://read.share.bbcook.cn/Article/details/gavqozxgw.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gdmrtygyu.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/gckbanzso.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.vehdjk.com/Article/details/gtygkxhjb.sHtML

[R50] awk 求和
来源：http://mobile.sjlbkw.cn/Article/details/gppdzepdc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fktsv.cn/Article/details/gfsctxujv.sHtML

[R51] 排序去重取前几
来源：http://mobile.epnwcf.com/Article/details/gwxpjjpsb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fktsv.cn/Article/details/glgddpdtz.sHtML

[R52] 统计行数
来源：http://read.share.yfazqb.com/Article/details/gmncfwmvg.sHtML

wc -l a.txt
来源：http://www.share.fktsv.cn/Article/details/gtqgxxetx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.tarul.cn/Article/details/gvvvfmafx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gwzdwdqen.sHtML

[R54] 比较两个文件
来源：http://mobile.epnwcf.com/Article/details/gxjmffoek.sHtML

diff a.txt b.txt
来源：http://wap.tarul.cn/Article/details/gcbifmgzp.sHtML

[R55] 压缩与解压
来源：http://baike.yfazqb.com/Article/details/gsxkkqzmc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.sjlbkw.cn/Article/details/gflozopcb.sHtML

[R56] 远程拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gnazsfuta.sHtML

scp file user@host:/path/
来源：http://mobile.epnwcf.com/Article/details/geaenqycp.sHtML

[R57] 远程执行命令
来源：http://www.blog.yfazqb.com/Article/details/guccdbwkl.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/gjfjjhtkk.sHtML

[R58] 下载文件
来源：http://read.share.tarul.cn/Article/details/gwdwfczcl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fktsv.cn/Article/details/gesxfcpjx.sHtML

[R59] 发 POST JSON
来源：http://read.share.tarul.cn/Article/details/gpfapephq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.tarul.cn/Article/details/gmbiugrda.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.bbcook.cn/Article/details/gzqrzazho.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.sjlbkw.cn/Article/details/gvdcjvzhg.sHtML

[R61] 磁盘占用
来源：http://wap.bbcook.cn/Article/details/gwizszffv.sHtML

df -h;  du -sh *
来源：http://mobile.tarul.cn/Article/details/gzsgylqks.sHtML

[R62] 找最占空间的文件
来源：http://wap.vehdjk.com/Article/details/grtyqsapz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.yfazqb.com/Article/details/giptuuyxk.sHtML

[R63] 内存与进程
来源：http://www.m.share.epnwcf.com/Article/details/gtajarouo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.epnwcf.com/Article/details/gbjzgemgu.sHtML

[R64] 结束进程
来源：http://m.share.bbcook.cn/Article/details/gcawdvytr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.tarul.cn/Article/details/gjqpuetny.sHtML

[R65] 查看端口占用
来源：http://www.share.sjlbkw.cn/Article/details/gqfjvgzzw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.yfazqb.com/Article/details/guersihqp.sHtML

[R66] 定时任务
来源：http://blog.epnwcf.com/Article/details/gihdtwmth.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/gswwbgpzr.sHtML

[R67] 生成随机十六进制串
来源：http://3g.tarul.cn/Article/details/gdpohfjky.sHtML

openssl rand -hex 16
来源：http://www.share.yfazqb.com/Article/details/gxiknixxa.sHtML

[R68] 计算文件校验值
来源：http://blog.epnwcf.com/Article/details/gnivulwyh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fktsv.cn/Article/details/gzhrnzkrv.sHtML

[R69] 生成随机密码
来源：http://3g.yfazqb.com/Article/details/gcxyvvjyn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.bbcook.cn/Article/details/gqicjhvzk.sHtML

[R70] 时间戳与互转
来源：http://m.share.epnwcf.com/Article/details/gwshcrkia.sHtML

date +%s;  date -d @1700000000
来源：http://wap.tarul.cn/Article/details/gurdnkqnb.sHtML

[R71] 日期格式化
来源：http://www.blog.vehdjk.com/Article/details/ghleiintw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.bbcook.cn/Article/details/gbhjiowbl.sHtML

[R72] 等待端口就绪
来源：http://www.share.tarul.cn/Article/details/grxhvjxxf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.sjlbkw.cn/Article/details/gohokcues.sHtML

[R73] 分割大日志
来源：http://www.blog.epnwcf.com/Article/details/gfywcynyw.sHtML

split -l 1000 big.log part_
来源：http://www.share.yfazqb.com/Article/details/guztxynar.sHtML

[R74] 批量重命名
来源：http://mobile.fktsv.cn/Article/details/gspxkpcxn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/gzqhlhtqx.sHtML

[R75] 导出环境变量
来源：http://baike.vehdjk.com/Article/details/gcvwhrscd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.yfazqb.com/Article/details/gwizvwjbw.sHtML

[R76] 使用临时文件
来源：http://www.m.share.yfazqb.com/Article/details/ghxivarpr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gqpnzcsvl.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/gqnodpzbk.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.epnwcf.com/Article/details/gwtyefrpk.sHtML

[R78] 交互式菜单
来源：http://www.blog.sjlbkw.cn/Article/details/gakocqpfo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.vehdjk.com/Article/details/gjhxbikxv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.epnwcf.com/Article/details/gdkpqsnll.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.vehdjk.com/Article/details/geeubaqzg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/grymxkxqk.sHtML

time ./run.sh
来源：http://wap.sjlbkw.cn/Article/details/gmpotvtfp.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvenybzio.sHtML

S. C / C++ 专题
来源：http://3g.epnwcf.com/Article/details/gyvxzxoyf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gvjdqvbod.sHtML

[S01] C：Hello World
来源：http://read.share.fktsv.cn/Article/details/gznvibysv.sHtML

#include <stdio.h>
来源：http://baike.tarul.cn/Article/details/gnfvokuvx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fktsv.cn/Article/details/gvdhaxkwy.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.epnwcf.com/Article/details/gakjzagmw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.bbcook.cn/Article/details/gnofqwtag.sHtML

[S03] C：读入整数
来源：http://blog.yfazqb.com/Article/details/gpynzifvu.sHtML

int x; scanf("%d", &x);
来源：http://read.share.bbcook.cn/Article/details/grsytvzby.sHtML

[S04] C：字符串复制
来源：http://www.blog.bbcook.cn/Article/details/gdmuanseu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.vehdjk.com/Article/details/gxtzhnwcj.sHtML

[S05] C：字符串长度
来源：http://wap.vehdjk.com/Article/details/guitkztwi.sHtML

strlen(s)
来源：http://www.share.fktsv.cn/Article/details/gjnjpbqpa.sHtML

[S06] C：字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/gxjjorbhb.sHtML

strcmp(a, b) == 0
来源：http://read.share.bbcook.cn/Article/details/gnkrtmgdq.sHtML

[S07] C：数组遍历求和
来源：http://blog.epnwcf.com/Article/details/gdkwbgugj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.tarul.cn/Article/details/gtvwaoabd.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fktsv.cn/Article/details/gjddntagf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.sjlbkw.cn/Article/details/gfoqdkmcv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.tarul.cn/Article/details/geekowwya.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.tarul.cn/Article/details/goyyfkpdx.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.yfazqb.com/Article/details/gzacmgxkk.sHtML

int *p = &a;  *p = 5;
来源：http://3g.yfazqb.com/Article/details/gfonrmbsl.sHtML

[S11] C：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gccziiyhz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.tarul.cn/Article/details/glapfenag.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fktsv.cn/Article/details/gxtfujkom.sHtML

fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gezsynvqs.sHtML

[S12] C：写文件
来源：http://baike.epnwcf.com/Article/details/gmlsbvxtr.sHtML


<!-- 参考信息 -->