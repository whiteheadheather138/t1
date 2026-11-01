代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.sjlbkw.cn/Article/details/grqzqbylo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.bbcook.cn/Article/details/gbxfcccck.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/gsbqabstt.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.vehdjk.com/Article/details/gxcqxrswo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.bbcook.cn/Article/details/gbueizdzv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fktsv.cn/Article/details/gdssbvrvr.sHtML

[Q43] 标量子查询
来源：http://baike.bbcook.cn/Article/details/gnhkyfuid.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.vehdjk.com/Article/details/gjtiupznc.sHtML

[Q44] IN 子查询
来源：http://read.share.sjlbkw.cn/Article/details/gcgrhlnqz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/germzijbh.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.bbcook.cn/Article/details/gveejddsg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.sjlbkw.cn/Article/details/grqbymvxb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fktsv.cn/Article/details/gfsxomawp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/gpwhqcwbw.sHtML

[Q47] 与平均值比较
来源：http://blog.tarul.cn/Article/details/gvozkzkbs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.vehdjk.com/Article/details/gspkpxdwd.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.vehdjk.com/Article/details/grmukzilq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.epnwcf.com/Article/details/gcsqpvmhz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.tarul.cn/Article/details/gbmfedguh.sHtML

[Q49] 更新单行
来源：http://m.share.vehdjk.com/Article/details/gsaqltldu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/gdrrfizlr.sHtML

[Q50] 批量更新
来源：http://mobile.tarul.cn/Article/details/gipddcvck.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.bbcook.cn/Article/details/gnwvmvthr.sHtML

[Q51] 用子查询更新
来源：http://3g.tarul.cn/Article/details/gcdxxxqad.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gizvoqreg.sHtML

[Q52] 删除指定行
来源：http://wap.epnwcf.com/Article/details/gfkkhnxrl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/gzqtyozsj.sHtML

[Q53] 按条件删除
来源：http://blog.fktsv.cn/Article/details/gbsfnmzos.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fktsv.cn/Article/details/gytugdlmf.sHtML

[Q54] 清空表
来源：http://3g.epnwcf.com/Article/details/gsjsqszir.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.sjlbkw.cn/Article/details/gfcsnblrh.sHtML

[Q55] 排名（并列占位）
来源：http://3g.epnwcf.com/Article/details/gdqryjhij.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.sjlbkw.cn/Article/details/gsrmvuwes.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.epnwcf.com/Article/details/galtmuwso.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.vehdjk.com/Article/details/gwdnsngrk.sHtML

[Q57] 行号
来源：http://www.share.bbcook.cn/Article/details/gpfmhiznk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.yfazqb.com/Article/details/gmrhvbtzm.sHtML

[Q58] 累计求和
来源：http://www.share.yfazqb.com/Article/details/gumxhwrud.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.vehdjk.com/Article/details/gfiumqobw.sHtML

[Q59] 分组内累计
来源：http://www.share.fktsv.cn/Article/details/gtskjkoyw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gluiqvucz.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.epnwcf.com/Article/details/gduhjgftc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.vehdjk.com/Article/details/gpehqqywg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.vehdjk.com/Article/details/gglxpzwba.sHtML

[Q61] 移动平均
来源：http://www.share.sjlbkw.cn/Article/details/gejwbmfah.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/girbobinh.sHtML

[Q62] 分组占比
来源：http://www.share.sjlbkw.cn/Article/details/gbnboplwz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gsqcglnhh.sHtML

[Q63] 开启事务
来源：http://www.share.tarul.cn/Article/details/giocshvym.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.epnwcf.com/Article/details/gnzqlhllx.sHtML

[Q64] 提交事务
来源：http://www.blog.epnwcf.com/Article/details/ggpnmqbaz.sHtML

COMMIT;
来源：http://wap.vehdjk.com/Article/details/gxczupdxn.sHtML

[Q65] 回滚事务
来源：http://wap.tarul.cn/Article/details/gzsmoqtac.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/gktanqqeb.sHtML

[Q66] 行锁查询
来源：http://wap.sjlbkw.cn/Article/details/gonmzfgbe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.tarul.cn/Article/details/gqnjtpqmy.sHtML

[Q67] 设置隔离级别
来源：http://blog.yfazqb.com/Article/details/gqwxlefgs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.bbcook.cn/Article/details/gemwotpki.sHtML

[Q68] 保存点
来源：http://m.share.tarul.cn/Article/details/gvwhodzkq.sHtML

SAVEPOINT sp1;
来源：http://www.blog.vehdjk.com/Article/details/guxfyaivt.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdipqgcft.sHtML

[Q69] 查看执行计划
来源：http://3g.epnwcf.com/Article/details/gthdbzhxp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.vehdjk.com/Article/details/gmweepudz.sHtML

[Q70] 更新统计信息
来源：http://www.share.epnwcf.com/Article/details/gznnjbnlx.sHtML

ANALYZE TABLE users;
来源：http://baike.sjlbkw.cn/Article/details/gjlxpuyaf.sHtML

[Q71] 查看建表语句
来源：http://mobile.bbcook.cn/Article/details/gkpkfthhs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fktsv.cn/Article/details/gzcvvtiwm.sHtML

[Q72] 查看索引
来源：http://baike.epnwcf.com/Article/details/gheysulgd.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.epnwcf.com/Article/details/geqhcjzeh.sHtML

[Q73] 查看表状态
来源：http://wap.yfazqb.com/Article/details/gaeguijnt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.epnwcf.com/Article/details/gtmmeoieq.sHtML

[Q74] 强制使用索引
来源：http://m.share.vehdjk.com/Article/details/gwyibinjw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.vehdjk.com/Article/details/ghzakwopk.sHtML

[Q75] 日期格式化
来源：http://read.share.fktsv.cn/Article/details/gtmccrpyn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.bbcook.cn/Article/details/gvbvjqniu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.sjlbkw.cn/Article/details/ghpqsznnr.sHtML

[Q76] 按天统计
来源：http://blog.vehdjk.com/Article/details/gcncfoefv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.tarul.cn/Article/details/gqgcvjyoy.sHtML

[Q77] 时间加减
来源：http://www.blog.sjlbkw.cn/Article/details/gklhqlvlo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.epnwcf.com/Article/details/gmthgjejr.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/glqjujmbd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.tarul.cn/Article/details/gmryroznq.sHtML

[Q79] 字符串拼接
来源：http://m.share.epnwcf.com/Article/details/gbdoaxavf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.epnwcf.com/Article/details/glvzlkwin.sHtML

[Q80] 字符串截取
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuqurnxc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.epnwcf.com/Article/details/gwxfihtdk.sHtML

[Q81] 字符串替换
来源：http://wap.fktsv.cn/Article/details/gupcmuqkw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gqfzajqkq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.tarul.cn/Article/details/gmwbqfbmr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gyojyuuyn.sHtML

[Q83] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gtpadduay.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gtwdorsas.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fktsv.cn/Article/details/geoiykojq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gsptkdptx.sHtML

[Q85] 数值取整
来源：http://3g.bbcook.cn/Article/details/gagkptcbj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.vehdjk.com/Article/details/gedeeyydo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.vehdjk.com/Article/details/gycarmamv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.tarul.cn/Article/details/ggkutawqw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.sjlbkw.cn/Article/details/gukwbjamk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.vehdjk.com/Article/details/gixeouqkh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.yfazqb.com/Article/details/gzaklgadw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fktsv.cn/Article/details/gdjepkwed.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.bbcook.cn/Article/details/gotykggeo.sHtML

[Q89] 判断表是否存在
来源：http://baike.vehdjk.com/Article/details/gwdvbabco.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.yfazqb.com/Article/details/gbumgzivc.sHtML

[Q90] 生成序号列
来源：http://baike.sjlbkw.cn/Article/details/gmzemuuoy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.yfazqb.com/Article/details/grcwcjlbh.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gsrkiamkb.sHtML

R. Bash 专题
来源：http://www.m.share.epnwcf.com/Article/details/gytakgsll.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqkxneah.sHtML

[R01] shebang 与严格模式
来源：http://www.share.sjlbkw.cn/Article/details/gfbzrugof.sHtML

#!/usr/bin/env bash
来源：http://wap.vehdjk.com/Article/details/gplgfuxxh.sHtML

set -euo pipefail
来源：http://baike.vehdjk.com/Article/details/guzfcozhq.sHtML

[R02] 变量赋值与使用
来源：http://read.share.epnwcf.com/Article/details/gctbquiog.sHtML

name="Tom"; echo "$name"
来源：http://www.share.yfazqb.com/Article/details/grmiogqew.sHtML

[R03] 只读变量
来源：http://www.blog.epnwcf.com/Article/details/gxykpvonq.sHtML

readonly PI=3.14
来源：http://www.m.share.sjlbkw.cn/Article/details/gclngidau.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/gyxadfdjr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.bbcook.cn/Article/details/gmvxucsei.sHtML

[R05] 参数默认值
来源：http://3g.epnwcf.com/Article/details/gjdaukrdy.sHtML

name="${1:-default}"
来源：http://www.m.share.bbcook.cn/Article/details/gppljzzge.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.tarul.cn/Article/details/gzoklmsld.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gtspopjst.sHtML

[R07] if 判断文件
来源：http://www.m.share.bbcook.cn/Article/details/gyijzmeil.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.epnwcf.com/Article/details/gkosfagxk.sHtML

[R08] 数值比较
来源：http://blog.fktsv.cn/Article/details/gjfvkixue.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.tarul.cn/Article/details/gegovupqw.sHtML

[R09] 字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gijvailjp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.tarul.cn/Article/details/gpjhiqkal.sHtML

[R10] 正则匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyyndykf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.epnwcf.com/Article/details/gqgtjgzyv.sHtML

[R11] case 多分支
来源：http://3g.sjlbkw.cn/Article/details/gixvtrrxd.sHtML

case "$1" in
来源：http://3g.fktsv.cn/Article/details/gnkvhnxyi.sHtML

start) echo "启动" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gjfqxflyv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.bbcook.cn/Article/details/gwzpgmrqa.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.yfazqb.com/Article/details/gtccnocdc.sHtML

esac
来源：http://www.share.epnwcf.com/Article/details/ghgbzdmdd.sHtML

[R12] for 遍历文件
来源：http://wap.sjlbkw.cn/Article/details/gfnstuigz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.bbcook.cn/Article/details/giibfxjck.sHtML

[R13] for 计数循环
来源：http://baike.bbcook.cn/Article/details/gffufeitn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gawhqqcvr.sHtML

[R14] C 风格 for
来源：http://www.share.fktsv.cn/Article/details/gpgbximyd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/guefxhdva.sHtML

[R15] while 逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gbcvpfagk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.vehdjk.com/Article/details/goyohdxle.sHtML

[R16] until 等待条件
来源：http://www.share.epnwcf.com/Article/details/gasvmxwge.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/gfsdwpcsl.sHtML

[R17] 数组定义与取值
来源：http://read.share.sjlbkw.cn/Article/details/gxlxzujpt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.vehdjk.com/Article/details/gvfigzgds.sHtML

[R18] 遍历数组
来源：http://baike.tarul.cn/Article/details/gyuncodle.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.epnwcf.com/Article/details/gbzsrrsso.sHtML

[R19] 数组长度
来源：http://3g.tarul.cn/Article/details/gtlzaijmb.sHtML

echo "${#arr[@]}"
来源：http://blog.vehdjk.com/Article/details/gbzxydzxy.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.yfazqb.com/Article/details/gehofogcx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.tarul.cn/Article/details/gyctxnxgc.sHtML

[R21] 字符串长度
来源：http://3g.bbcook.cn/Article/details/giqagmrkc.sHtML

echo "${#s}"
来源：http://www.blog.fktsv.cn/Article/details/gqqhaalgg.sHtML

[R22] 截取子串
来源：http://baike.vehdjk.com/Article/details/gmxeqtgvn.sHtML

echo "${s:0:5}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gwyjigzrm.sHtML

[R23] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/ghymbaabl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.bbcook.cn/Article/details/gvrpiemvz.sHtML

[R24] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gjhrkgjhp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.sjlbkw.cn/Article/details/gdkrtpmje.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.vehdjk.com/Article/details/gzkrybfhw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.sjlbkw.cn/Article/details/gbnlhlmcm.sHtML

[R26] 命令替换
来源：http://3g.tarul.cn/Article/details/gpzcwohwj.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fktsv.cn/Article/details/ggvngaocd.sHtML

[R27] 算术展开
来源：http://3g.sjlbkw.cn/Article/details/grqqbiriw.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.sjlbkw.cn/Article/details/grobsxvlq.sHtML

[R28] 浮点运算
来源：http://www.share.vehdjk.com/Article/details/gnnqkrhvk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.yfazqb.com/Article/details/guiuqwyud.sHtML

[R29] 定义函数
来源：http://www.blog.tarul.cn/Article/details/gilmnpbik.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.tarul.cn/Article/details/gdjinhcmy.sHtML

[R30] 函数返回状态码
来源：http://read.share.sjlbkw.cn/Article/details/gvqabbhuc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.bbcook.cn/Article/details/gvsoqbvte.sHtML

[R31] 局部变量
来源：http://wap.tarul.cn/Article/details/gkucqkdjf.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fktsv.cn/Article/details/gvpbbxiun.sHtML

[R32] 参数个数校验
来源：http://mobile.bbcook.cn/Article/details/gwptdzjvd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gbxpbxphd.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.vehdjk.com/Article/details/ghjpshnzn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.yfazqb.com/Article/details/gokchnkig.sHtML

[R34] 退出时清理
来源：http://www.share.tarul.cn/Article/details/gjdmxpwec.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/gfqosnenk.sHtML

[R35] 后台执行并等待
来源：http://mobile.yfazqb.com/Article/details/gakoonhgu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fktsv.cn/Article/details/gcmkbyeyy.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fktsv.cn/Article/details/gwgxylaza.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.bbcook.cn/Article/details/gjjhswatu.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fktsv.cn/Article/details/gcchvqcqx.sHtML

files=$(ls -1)
来源：http://read.share.vehdjk.com/Article/details/gxcprkgar.sHtML

[R38] 管道串联
来源：http://3g.fktsv.cn/Article/details/gzeahjcjq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fktsv.cn/Article/details/gxpyjnbub.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.yfazqb.com/Article/details/gynumtdnu.sHtML

cmd > out.log 2>&1
来源：http://blog.yfazqb.com/Article/details/gsinudsbh.sHtML

[R40] 追加写日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gerdretjr.sHtML

echo "log" >> out.log
来源：http://mobile.yfazqb.com/Article/details/goanzabow.sHtML

[R41] 丢弃输出
来源：http://www.blog.epnwcf.com/Article/details/gjyojfugf.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gwmajdioa.sHtML

[R42] 输入重定向
来源：http://3g.epnwcf.com/Article/details/grsvueyjt.sHtML

wc -l < a.txt
来源：http://www.share.yfazqb.com/Article/details/gpnmofprd.sHtML

[R43] 按名字查找文件
来源：http://www.share.tarul.cn/Article/details/gzdlsened.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/ggyvspjso.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.epnwcf.com/Article/details/gitpolmny.sHtML

find . -mtime -7 -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gaxcdebrg.sHtML

[R45] 批量删除
来源：http://www.m.share.bbcook.cn/Article/details/gxxwhzacn.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/glfvlcjud.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gkispkujo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.epnwcf.com/Article/details/gmxynjbqq.sHtML

[R47] sed 单行替换
来源：http://mobile.vehdjk.com/Article/details/gtdvzvmik.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.epnwcf.com/Article/details/gaxddgkmy.sHtML

[R48] awk 取指定列
来源：http://3g.sjlbkw.cn/Article/details/gmqvhjbam.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gpyynkfyp.sHtML

[R49] awk 带条件
来源：http://blog.yfazqb.com/Article/details/gybohyuby.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.epnwcf.com/Article/details/gacxcoqof.sHtML

[R50] awk 求和
来源：http://read.share.yfazqb.com/Article/details/gaeuapmia.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gthcyiuow.sHtML

[R51] 排序去重取前几
来源：http://www.blog.vehdjk.com/Article/details/gsdvekpnb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.yfazqb.com/Article/details/gqyuxgnww.sHtML

[R52] 统计行数
来源：http://www.share.fktsv.cn/Article/details/gewpgftav.sHtML

wc -l a.txt
来源：http://mobile.fktsv.cn/Article/details/gwwbqqtrx.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.epnwcf.com/Article/details/gfmkwrznh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.epnwcf.com/Article/details/gcbwonlvc.sHtML

[R54] 比较两个文件
来源：http://m.share.yfazqb.com/Article/details/gmzzvxnmp.sHtML

diff a.txt b.txt
来源：http://mobile.yfazqb.com/Article/details/gpcxtlkwz.sHtML

[R55] 压缩与解压
来源：http://read.share.fktsv.cn/Article/details/grkiagiqw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.vehdjk.com/Article/details/gfvtmuwao.sHtML

[R56] 远程拷贝
来源：http://www.share.yfazqb.com/Article/details/gtczkvuoj.sHtML

scp file user@host:/path/
来源：http://www.share.sjlbkw.cn/Article/details/goxgugnbs.sHtML

[R57] 远程执行命令
来源：http://mobile.yfazqb.com/Article/details/gynhrqjsw.sHtML

ssh user@host 'uptime'
来源：http://read.share.bbcook.cn/Article/details/grvurcued.sHtML

[R58] 下载文件
来源：http://www.m.share.epnwcf.com/Article/details/gdygifqbq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/ghwafgpjd.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/gjltuirhb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.epnwcf.com/Article/details/glyovfakb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/ghscbbsoy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.bbcook.cn/Article/details/gdzxfusww.sHtML

[R61] 磁盘占用
来源：http://www.share.bbcook.cn/Article/details/gpaosydbz.sHtML

df -h;  du -sh *
来源：http://m.share.sjlbkw.cn/Article/details/ggkvpgnqn.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/gwzusylem.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.yfazqb.com/Article/details/gekqkatlg.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gwrtrccad.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.vehdjk.com/Article/details/gxemzqslg.sHtML

[R64] 结束进程
来源：http://mobile.sjlbkw.cn/Article/details/gpvrbgzwq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.yfazqb.com/Article/details/gfdbfnrul.sHtML

[R65] 查看端口占用
来源：http://www.m.share.epnwcf.com/Article/details/gdseifgwp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.vehdjk.com/Article/details/guvhmcauo.sHtML

[R66] 定时任务
来源：http://www.share.fktsv.cn/Article/details/gtadsfkky.sHtML

crontab -e;  crontab -l
来源：http://blog.bbcook.cn/Article/details/gxqyuvgoj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.epnwcf.com/Article/details/gchbreaxl.sHtML

openssl rand -hex 16
来源：http://3g.epnwcf.com/Article/details/gpiimssbq.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.yfazqb.com/Article/details/guaytkqdc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fktsv.cn/Article/details/ggnhydegw.sHtML

[R69] 生成随机密码
来源：http://baike.epnwcf.com/Article/details/gwjdboorh.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.bbcook.cn/Article/details/giassminf.sHtML

[R70] 时间戳与互转
来源：http://baike.epnwcf.com/Article/details/ginhbtopt.sHtML

date +%s;  date -d @1700000000
来源：http://blog.epnwcf.com/Article/details/gkxbtnekc.sHtML

[R71] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gpuvexxut.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.yfazqb.com/Article/details/guwjzykzz.sHtML

[R72] 等待端口就绪
来源：http://baike.yfazqb.com/Article/details/grvtjfghr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.bbcook.cn/Article/details/gqozhvlqp.sHtML

[R73] 分割大日志
来源：http://read.share.fktsv.cn/Article/details/gwyvjltsa.sHtML

split -l 1000 big.log part_
来源：http://3g.fktsv.cn/Article/details/gazxuzmld.sHtML

[R74] 批量重命名
来源：http://read.share.tarul.cn/Article/details/gytfheqer.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/gnxroeyrr.sHtML

[R75] 导出环境变量
来源：http://blog.yfazqb.com/Article/details/gndjxnhra.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.vehdjk.com/Article/details/gxzfqmgdn.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/gwrailmro.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gkgfexprt.sHtML

[R77] 读取用户输入
来源：http://www.share.yfazqb.com/Article/details/gdgsicxss.sHtML

read -rp "请输入: " ans
来源：http://blog.yfazqb.com/Article/details/gmbpgznfw.sHtML

[R78] 交互式菜单
来源：http://www.blog.vehdjk.com/Article/details/gtxlqhtox.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.vehdjk.com/Article/details/ggfwicupu.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.bbcook.cn/Article/details/gflffuemh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.bbcook.cn/Article/details/gybbutocx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.vehdjk.com/Article/details/grbeenogp.sHtML

time ./run.sh
来源：http://read.share.sjlbkw.cn/Article/details/gscdzdhof.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gtbjzbwnq.sHtML

S. C / C++ 专题
来源：http://www.share.sjlbkw.cn/Article/details/gsskleaha.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gawjpximk.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gipsgfuht.sHtML

#include <stdio.h>
来源：http://read.share.yfazqb.com/Article/details/glohqalnm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.epnwcf.com/Article/details/gptlkvhzk.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fktsv.cn/Article/details/gbdrlqalw.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.sjlbkw.cn/Article/details/ggpfxfhgm.sHtML

[S03] C：读入整数
来源：http://wap.tarul.cn/Article/details/gatspvyqc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.epnwcf.com/Article/details/ghzyajwmh.sHtML

[S04] C：字符串复制
来源：http://www.share.yfazqb.com/Article/details/gobyqtatd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.tarul.cn/Article/details/gvhwivuzf.sHtML

[S05] C：字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gqqqkbrwh.sHtML

strlen(s)
来源：http://www.m.share.tarul.cn/Article/details/gtvsbwwpk.sHtML

[S06] C：字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gsduvhree.sHtML

strcmp(a, b) == 0
来源：http://mobile.fktsv.cn/Article/details/gpyizbqjl.sHtML

[S07] C：数组遍历求和
来源：http://baike.sjlbkw.cn/Article/details/gykoltalj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fktsv.cn/Article/details/gehqlmugk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.vehdjk.com/Article/details/gkrfibman.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.epnwcf.com/Article/details/gltxvxpnz.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.tarul.cn/Article/details/guozkdhoa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fktsv.cn/Article/details/gjemxovue.sHtML

[S10] C：指针与解引用
来源：http://baike.yfazqb.com/Article/details/grkmgwaog.sHtML

int *p = &a;  *p = 5;
来源：http://3g.tarul.cn/Article/details/gdzgeeydc.sHtML

[S11] C：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gibvosfyx.sHtML


<!-- 参考信息 -->