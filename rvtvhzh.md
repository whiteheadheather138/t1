代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://blog.fktsv.cn/Article/details/gniycrcop.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fktsv.cn/Article/details/gigwftihr.sHtML

[Q43] 标量子查询
来源：http://read.share.sjlbkw.cn/Article/details/gzfqkmvkv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.sjlbkw.cn/Article/details/gteeropui.sHtML

[Q44] IN 子查询
来源：http://m.share.sjlbkw.cn/Article/details/gvvauapgi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/gvnykhskq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.sjlbkw.cn/Article/details/gczwfjuga.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gmpdmygmg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.tarul.cn/Article/details/gbycmvkxf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gpmidxsvd.sHtML

[Q47] 与平均值比较
来源：http://m.share.tarul.cn/Article/details/gjylhsxfu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.bbcook.cn/Article/details/ghzayyjzw.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.epnwcf.com/Article/details/gznqlzcjy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.bbcook.cn/Article/details/gxwuqsxjn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fktsv.cn/Article/details/gqimagzuq.sHtML

[Q49] 更新单行
来源：http://blog.yfazqb.com/Article/details/gjgkpyywr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gadmfkewx.sHtML

[Q50] 批量更新
来源：http://wap.fktsv.cn/Article/details/gorpyxfls.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.epnwcf.com/Article/details/gqtkawhni.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gtxrclvwm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.epnwcf.com/Article/details/garzpjfos.sHtML

[Q52] 删除指定行
来源：http://blog.bbcook.cn/Article/details/gyooeudyy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gmpnbjord.sHtML

[Q53] 按条件删除
来源：http://baike.sjlbkw.cn/Article/details/gwxzruxqs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.epnwcf.com/Article/details/gubwfqlvl.sHtML

[Q54] 清空表
来源：http://www.share.epnwcf.com/Article/details/gcvarvbba.sHtML

TRUNCATE TABLE logs;
来源：http://3g.epnwcf.com/Article/details/gykjztags.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.vehdjk.com/Article/details/gizmtwqax.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.epnwcf.com/Article/details/gtqyxfxtr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.yfazqb.com/Article/details/gvdfuqsbk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/gnxtusbxd.sHtML

[Q57] 行号
来源：http://m.share.fktsv.cn/Article/details/ghvhcubjd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gmixssxef.sHtML

[Q58] 累计求和
来源：http://read.share.vehdjk.com/Article/details/gmrjvfaqn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gqboaiors.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/grbqylgnl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gjjwquvvc.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.epnwcf.com/Article/details/ggexhnils.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.vehdjk.com/Article/details/gzjnjjbic.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmpjmhix.sHtML

[Q61] 移动平均
来源：http://www.share.yfazqb.com/Article/details/gdnafkbci.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gxvqvkezp.sHtML

[Q62] 分组占比
来源：http://mobile.tarul.cn/Article/details/gpbcehlvj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gucnhypho.sHtML

[Q63] 开启事务
来源：http://www.share.epnwcf.com/Article/details/glntchmtz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fktsv.cn/Article/details/gvookqyey.sHtML

[Q64] 提交事务
来源：http://www.share.fktsv.cn/Article/details/gmlxnuwor.sHtML

COMMIT;
来源：http://mobile.tarul.cn/Article/details/gjrhmcegv.sHtML

[Q65] 回滚事务
来源：http://blog.vehdjk.com/Article/details/goqgwdavm.sHtML

ROLLBACK;
来源：http://mobile.vehdjk.com/Article/details/ggathvtiq.sHtML

[Q66] 行锁查询
来源：http://baike.tarul.cn/Article/details/gmhrrimgv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.epnwcf.com/Article/details/gctqltkzj.sHtML

[Q67] 设置隔离级别
来源：http://wap.bbcook.cn/Article/details/gzeezoxex.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.vehdjk.com/Article/details/gwybcoifw.sHtML

[Q68] 保存点
来源：http://www.blog.yfazqb.com/Article/details/gcwqbjuwq.sHtML

SAVEPOINT sp1;
来源：http://mobile.tarul.cn/Article/details/gsmctgcjk.sHtML

ROLLBACK TO sp1;
来源：http://mobile.tarul.cn/Article/details/gpbjdnvom.sHtML

[Q69] 查看执行计划
来源：http://mobile.yfazqb.com/Article/details/gxwepgfdy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.vehdjk.com/Article/details/gpoliptdh.sHtML

[Q70] 更新统计信息
来源：http://blog.bbcook.cn/Article/details/gvnbaymla.sHtML

ANALYZE TABLE users;
来源：http://www.share.fktsv.cn/Article/details/gtebrdlwi.sHtML

[Q71] 查看建表语句
来源：http://3g.fktsv.cn/Article/details/gkrmqpcwr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.tarul.cn/Article/details/gzyahjhzk.sHtML

[Q72] 查看索引
来源：http://www.m.share.vehdjk.com/Article/details/gafsqtuxi.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gjmvdrpms.sHtML

[Q73] 查看表状态
来源：http://3g.bbcook.cn/Article/details/gofvrtqgy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.vehdjk.com/Article/details/gysuqrfku.sHtML

[Q74] 强制使用索引
来源：http://blog.yfazqb.com/Article/details/giosvwzot.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.bbcook.cn/Article/details/gptfssgmo.sHtML

[Q75] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gjashymyu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fktsv.cn/Article/details/grlzdhhkb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.epnwcf.com/Article/details/gnfxaqrxk.sHtML

[Q76] 按天统计
来源：http://3g.vehdjk.com/Article/details/gcppmeviy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.vehdjk.com/Article/details/gbeduwmhu.sHtML

[Q77] 时间加减
来源：http://blog.sjlbkw.cn/Article/details/gpsuvnjhw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fktsv.cn/Article/details/gwdhohjmr.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/gfczwhnua.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.bbcook.cn/Article/details/gsiqwrzts.sHtML

[Q79] 字符串拼接
来源：http://baike.epnwcf.com/Article/details/gfjerrjgk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.bbcook.cn/Article/details/gyhiqvfwq.sHtML

[Q80] 字符串截取
来源：http://www.share.epnwcf.com/Article/details/giweucvze.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gizcndsse.sHtML

[Q81] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gujndemyb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.epnwcf.com/Article/details/gemebtazn.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.vehdjk.com/Article/details/glevtzelm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gvhrxzclq.sHtML

[Q83] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gylspqoeu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gwsknttda.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.vehdjk.com/Article/details/gmfzkclgr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gkjxmjhlt.sHtML

[Q85] 数值取整
来源：http://www.share.fktsv.cn/Article/details/gdcqnpjai.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.sjlbkw.cn/Article/details/gwhfkwylv.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.vehdjk.com/Article/details/gyzceaiof.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.sjlbkw.cn/Article/details/gvjnvanfy.sHtML

[Q87] JSON 字段做条件
来源：http://3g.bbcook.cn/Article/details/gmygylwsw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.epnwcf.com/Article/details/gqrxkhoae.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.bbcook.cn/Article/details/gxjfvcymb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.epnwcf.com/Article/details/gfbcrkfld.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.bbcook.cn/Article/details/gejzyvgfj.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.vehdjk.com/Article/details/giuzxglbt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fktsv.cn/Article/details/gexltxqov.sHtML

[Q90] 生成序号列
来源：http://blog.tarul.cn/Article/details/gzclhmzum.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.vehdjk.com/Article/details/grfzxdnxe.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/goiqlndbv.sHtML

R. Bash 专题
来源：http://blog.fktsv.cn/Article/details/gtocrlzgt.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gxbrihlrc.sHtML

[R01] shebang 与严格模式
来源：http://mobile.sjlbkw.cn/Article/details/gpsznsqwx.sHtML

#!/usr/bin/env bash
来源：http://read.share.yfazqb.com/Article/details/gwvnmkwlc.sHtML

set -euo pipefail
来源：http://www.blog.sjlbkw.cn/Article/details/gvyrppyng.sHtML

[R02] 变量赋值与使用
来源：http://wap.epnwcf.com/Article/details/gwqhesoqh.sHtML

name="Tom"; echo "$name"
来源：http://3g.tarul.cn/Article/details/glfdjujew.sHtML

[R03] 只读变量
来源：http://read.share.bbcook.cn/Article/details/gughihcmr.sHtML

readonly PI=3.14
来源：http://www.m.share.bbcook.cn/Article/details/gdtcjkhnp.sHtML

[R04] 位置参数
来源：http://read.share.epnwcf.com/Article/details/gmcczlsni.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.yfazqb.com/Article/details/gtsihnrwg.sHtML

[R05] 参数默认值
来源：http://blog.sjlbkw.cn/Article/details/gpmnlqoop.sHtML

name="${1:-default}"
来源：http://m.share.yfazqb.com/Article/details/guwjdxbeo.sHtML

[R06] 判断命令是否存在
来源：http://m.share.vehdjk.com/Article/details/gkkpmbyol.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/gaadudcrd.sHtML

[R07] if 判断文件
来源：http://www.share.yfazqb.com/Article/details/gdsibrjyn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.epnwcf.com/Article/details/gaeyfvyrn.sHtML

[R08] 数值比较
来源：http://blog.epnwcf.com/Article/details/gyhtniido.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.epnwcf.com/Article/details/ghosmhlca.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gymwqrbla.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.epnwcf.com/Article/details/gskhsgocv.sHtML

[R10] 正则匹配
来源：http://www.share.vehdjk.com/Article/details/gekvwulcm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.vehdjk.com/Article/details/gbppzolek.sHtML

[R11] case 多分支
来源：http://blog.bbcook.cn/Article/details/gemiqejkz.sHtML

case "$1" in
来源：http://blog.bbcook.cn/Article/details/gkrbnjjvv.sHtML

start) echo "启动" ;;
来源：http://mobile.yfazqb.com/Article/details/gnxctbhiq.sHtML

stop)  echo "停止" ;;
来源：http://wap.sjlbkw.cn/Article/details/gdygghboj.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.sjlbkw.cn/Article/details/grhaejwga.sHtML

esac
来源：http://wap.fktsv.cn/Article/details/gyvxqvcjn.sHtML

[R12] for 遍历文件
来源：http://blog.epnwcf.com/Article/details/gotxaydgi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.tarul.cn/Article/details/gfajhfczt.sHtML

[R13] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/ginfeamkt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.bbcook.cn/Article/details/gfwalsodf.sHtML

[R14] C 风格 for
来源：http://m.share.yfazqb.com/Article/details/gspismdbu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/gczsdsvxl.sHtML

[R15] while 逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gtzctivng.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.epnwcf.com/Article/details/gdzjeywjm.sHtML

[R16] until 等待条件
来源：http://www.share.fktsv.cn/Article/details/gwqfsqpwi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.yfazqb.com/Article/details/gayxvdiwy.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.yfazqb.com/Article/details/gtotcalow.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.epnwcf.com/Article/details/gqxwdwcll.sHtML

[R18] 遍历数组
来源：http://3g.fktsv.cn/Article/details/gzjgmtdju.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.vehdjk.com/Article/details/gccjptuvr.sHtML

[R19] 数组长度
来源：http://wap.sjlbkw.cn/Article/details/gevqrpidw.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.yfazqb.com/Article/details/gddftiahd.sHtML

[R20] 关联数组（字典）
来源：http://blog.yfazqb.com/Article/details/gdyherktn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.vehdjk.com/Article/details/gbflsuiuv.sHtML

[R21] 字符串长度
来源：http://m.share.yfazqb.com/Article/details/gdaimczfz.sHtML

echo "${#s}"
来源：http://wap.fktsv.cn/Article/details/gawwqreph.sHtML

[R22] 截取子串
来源：http://3g.epnwcf.com/Article/details/gltwfwreg.sHtML

echo "${s:0:5}"
来源：http://www.share.epnwcf.com/Article/details/gxryfeegk.sHtML

[R23] 字符串替换
来源：http://m.share.sjlbkw.cn/Article/details/gxdyzssqa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fktsv.cn/Article/details/gbjsjvrwm.sHtML

[R24] 大小写转换
来源：http://m.share.tarul.cn/Article/details/ggjzjuksn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.tarul.cn/Article/details/gyyetfwmx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/gpwvgeekx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.epnwcf.com/Article/details/gqfephbsx.sHtML

[R26] 命令替换
来源：http://www.share.vehdjk.com/Article/details/guxjpezbh.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.sjlbkw.cn/Article/details/gtdrnozwq.sHtML

[R27] 算术展开
来源：http://www.share.tarul.cn/Article/details/grfycmube.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.tarul.cn/Article/details/gtmztuxwy.sHtML

[R28] 浮点运算
来源：http://www.share.vehdjk.com/Article/details/gklfeelif.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fktsv.cn/Article/details/gcanfsiys.sHtML

[R29] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/glwacwjtg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fktsv.cn/Article/details/gektvpjfk.sHtML

[R30] 函数返回状态码
来源：http://m.share.tarul.cn/Article/details/geuocdttu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.yfazqb.com/Article/details/gplkjievl.sHtML

[R31] 局部变量
来源：http://m.share.fktsv.cn/Article/details/ghwmmsbvf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.yfazqb.com/Article/details/gjtjfmatn.sHtML

[R32] 参数个数校验
来源：http://m.share.bbcook.cn/Article/details/gjmvheqcn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/geqcwoomn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.yfazqb.com/Article/details/grjgwoyqu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.epnwcf.com/Article/details/ggdxvoxnh.sHtML

[R34] 退出时清理
来源：http://blog.bbcook.cn/Article/details/gajqewzqt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gqbzrqlyh.sHtML

[R35] 后台执行并等待
来源：http://www.blog.bbcook.cn/Article/details/gkyopocgq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.tarul.cn/Article/details/gifmdojly.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.bbcook.cn/Article/details/gpcqpishr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.bbcook.cn/Article/details/gsjquwvni.sHtML

[R37] 把输出赋给变量
来源：http://mobile.yfazqb.com/Article/details/gwemmwoca.sHtML

files=$(ls -1)
来源：http://read.share.vehdjk.com/Article/details/gohwwjyli.sHtML

[R38] 管道串联
来源：http://baike.tarul.cn/Article/details/ghkypwztp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.bbcook.cn/Article/details/gdxfblfhc.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.bbcook.cn/Article/details/gqpireftr.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gnqdyomxw.sHtML

[R40] 追加写日志
来源：http://3g.vehdjk.com/Article/details/genrkoopu.sHtML

echo "log" >> out.log
来源：http://wap.yfazqb.com/Article/details/gbcehuows.sHtML

[R41] 丢弃输出
来源：http://www.share.fktsv.cn/Article/details/ghoatwavx.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fktsv.cn/Article/details/gmikgdkjc.sHtML

[R42] 输入重定向
来源：http://read.share.bbcook.cn/Article/details/glrtaswcd.sHtML

wc -l < a.txt
来源：http://read.share.yfazqb.com/Article/details/gvmpoimiw.sHtML

[R43] 按名字查找文件
来源：http://wap.yfazqb.com/Article/details/glwbxrbgm.sHtML

find . -name "*.log" -type f
来源：http://blog.vehdjk.com/Article/details/gjhawjitk.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.epnwcf.com/Article/details/gveeycjmx.sHtML

find . -mtime -7 -type f
来源：http://mobile.bbcook.cn/Article/details/glcpuludf.sHtML

[R45] 批量删除
来源：http://wap.sjlbkw.cn/Article/details/ggqxlmfiu.sHtML

find . -name "*.tmp" -delete
来源：http://3g.tarul.cn/Article/details/gehumxvrz.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.vehdjk.com/Article/details/gstbmynfq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.bbcook.cn/Article/details/gjxqcwyew.sHtML

[R47] sed 单行替换
来源：http://blog.sjlbkw.cn/Article/details/gaedrjhvv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.yfazqb.com/Article/details/gtmopqukx.sHtML

[R48] awk 取指定列
来源：http://m.share.tarul.cn/Article/details/gdyfgzpqq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrshvzhp.sHtML

[R49] awk 带条件
来源：http://3g.yfazqb.com/Article/details/gkdhatdsf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.sjlbkw.cn/Article/details/gjqhdlhlg.sHtML

[R50] awk 求和
来源：http://baike.fktsv.cn/Article/details/gpbtcjigz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gnsngzarn.sHtML

[R51] 排序去重取前几
来源：http://mobile.vehdjk.com/Article/details/gcfyywzfz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.yfazqb.com/Article/details/gszsgqjtj.sHtML

[R52] 统计行数
来源：http://m.share.vehdjk.com/Article/details/gugkxdsee.sHtML

wc -l a.txt
来源：http://baike.yfazqb.com/Article/details/gxouutpvm.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.sjlbkw.cn/Article/details/gclvpeylb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.bbcook.cn/Article/details/gpssxjdkd.sHtML

[R54] 比较两个文件
来源：http://wap.epnwcf.com/Article/details/gcuylqfky.sHtML

diff a.txt b.txt
来源：http://blog.sjlbkw.cn/Article/details/gqlgktuxl.sHtML

[R55] 压缩与解压
来源：http://m.share.sjlbkw.cn/Article/details/gavfidlqw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.sjlbkw.cn/Article/details/gquprhjdn.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gemimkryw.sHtML

scp file user@host:/path/
来源：http://blog.fktsv.cn/Article/details/gszgtghoc.sHtML

[R57] 远程执行命令
来源：http://wap.sjlbkw.cn/Article/details/gyopscmpd.sHtML

ssh user@host 'uptime'
来源：http://3g.sjlbkw.cn/Article/details/ghbqcagdw.sHtML

[R58] 下载文件
来源：http://www.m.share.bbcook.cn/Article/details/gufsmkbxq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/gszxttqgg.sHtML

[R59] 发 POST JSON
来源：http://3g.bbcook.cn/Article/details/geslqmnsp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.epnwcf.com/Article/details/gioxjllua.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gfshfuqwm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fktsv.cn/Article/details/gehhixvbp.sHtML

[R61] 磁盘占用
来源：http://www.share.fktsv.cn/Article/details/gxsmkutza.sHtML

df -h;  du -sh *
来源：http://mobile.sjlbkw.cn/Article/details/gfftaxtyz.sHtML

[R62] 找最占空间的文件
来源：http://www.share.sjlbkw.cn/Article/details/gyhzfhjhd.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.bbcook.cn/Article/details/gdqxlposx.sHtML

[R63] 内存与进程
来源：http://baike.vehdjk.com/Article/details/gfcforwqi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.epnwcf.com/Article/details/gvnizglxa.sHtML

[R64] 结束进程
来源：http://www.m.share.vehdjk.com/Article/details/gglokqzri.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.bbcook.cn/Article/details/gnnbcnbko.sHtML

[R65] 查看端口占用
来源：http://www.blog.tarul.cn/Article/details/gloxzoqdm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.yfazqb.com/Article/details/gxszniphw.sHtML

[R66] 定时任务
来源：http://blog.sjlbkw.cn/Article/details/gtqydpjhi.sHtML

crontab -e;  crontab -l
来源：http://blog.yfazqb.com/Article/details/gbxkbasnj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/gpyzqljml.sHtML

openssl rand -hex 16
来源：http://www.blog.epnwcf.com/Article/details/gdatrdito.sHtML

[R68] 计算文件校验值
来源：http://3g.tarul.cn/Article/details/gxnjwkrgc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fktsv.cn/Article/details/grcgehrtq.sHtML

[R69] 生成随机密码
来源：http://blog.tarul.cn/Article/details/gurrcokzp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fktsv.cn/Article/details/gyqhdwwtx.sHtML

[R70] 时间戳与互转
来源：http://www.blog.vehdjk.com/Article/details/grctovfjy.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.vehdjk.com/Article/details/gvfeadhjw.sHtML

[R71] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/gdwtipoax.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.yfazqb.com/Article/details/gdbfuyfei.sHtML

[R72] 等待端口就绪
来源：http://wap.sjlbkw.cn/Article/details/gtfktdjdc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gdirhlctw.sHtML

[R73] 分割大日志
来源：http://wap.bbcook.cn/Article/details/gilugmxih.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/gsmnbkujy.sHtML

[R74] 批量重命名
来源：http://www.m.share.bbcook.cn/Article/details/giajqfsuf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.epnwcf.com/Article/details/gdnzuthhz.sHtML

[R75] 导出环境变量
来源：http://m.share.bbcook.cn/Article/details/gtcvryszl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.tarul.cn/Article/details/gobdneqvd.sHtML

[R76] 使用临时文件
来源：http://blog.bbcook.cn/Article/details/gcxsmymzw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.yfazqb.com/Article/details/ggjsxxikt.sHtML

[R77] 读取用户输入
来源：http://3g.tarul.cn/Article/details/gvfkbgxbi.sHtML

read -rp "请输入: " ans
来源：http://mobile.fktsv.cn/Article/details/gzuouhiaf.sHtML

[R78] 交互式菜单
来源：http://www.m.share.epnwcf.com/Article/details/gzxnoqivx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.sjlbkw.cn/Article/details/gcfsuaury.sHtML

[R79] 解析命令行选项
来源：http://m.share.tarul.cn/Article/details/gsvyvosqb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.vehdjk.com/Article/details/gkieksgqw.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.sjlbkw.cn/Article/details/gjshuciau.sHtML

time ./run.sh
来源：http://www.blog.vehdjk.com/Article/details/gllfckvpd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/goetwaarq.sHtML

S. C / C++ 专题
来源：http://www.m.share.bbcook.cn/Article/details/gfsjewbwx.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gxrrcyrwj.sHtML

[S01] C：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gujqyqgnk.sHtML

#include <stdio.h>
来源：http://m.share.fktsv.cn/Article/details/gavxmqtwc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.bbcook.cn/Article/details/gotmysskp.sHtML

[S02] C：变量与格式化输出
来源：http://blog.tarul.cn/Article/details/gjmhpfldc.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fktsv.cn/Article/details/gtqwmmefn.sHtML

[S03] C：读入整数
来源：http://blog.tarul.cn/Article/details/gsokctxqh.sHtML

int x; scanf("%d", &x);
来源：http://3g.bbcook.cn/Article/details/geazncpea.sHtML

[S04] C：字符串复制
来源：http://3g.epnwcf.com/Article/details/gjzaczptz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.epnwcf.com/Article/details/gmpvxxoyh.sHtML

[S05] C：字符串长度
来源：http://blog.yfazqb.com/Article/details/goukdhcup.sHtML

strlen(s)
来源：http://www.blog.vehdjk.com/Article/details/ginvatuvk.sHtML

[S06] C：字符串比较
来源：http://baike.epnwcf.com/Article/details/gvhcwxqww.sHtML

strcmp(a, b) == 0
来源：http://baike.fktsv.cn/Article/details/gkhlfhrjz.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.vehdjk.com/Article/details/gifvadqwp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.sjlbkw.cn/Article/details/gymhlpmua.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fktsv.cn/Article/details/gnwlfadjf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.sjlbkw.cn/Article/details/gtguydeyi.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.bbcook.cn/Article/details/giqtbcqmd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fktsv.cn/Article/details/gwyyvxiek.sHtML

[S10] C：指针与解引用
来源：http://blog.fktsv.cn/Article/details/gxqlzcpha.sHtML

int *p = &a;  *p = 5;
来源：http://wap.vehdjk.com/Article/details/gwfivqngj.sHtML

[S11] C：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gugxajndx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fktsv.cn/Article/details/gcpibwtts.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gesclglkh.sHtML

fclose(f);
来源：http://www.share.tarul.cn/Article/details/gezsqlnvv.sHtML

[S12] C：写文件
来源：http://3g.tarul.cn/Article/details/galigkqcx.sHtML


<!-- 参考信息 -->