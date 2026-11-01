代发 wailian999

[Q44] IN 子查询
来源：http://wap.tarul.cn/Article/details/gbkctyjfr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.epnwcf.com/Article/details/gufzphlci.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.yfazqb.com/Article/details/gfyonlypq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/gvijfhsat.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.tarul.cn/Article/details/gikiyihhj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.yfazqb.com/Article/details/gileerqnz.sHtML

[Q47] 与平均值比较
来源：http://blog.yfazqb.com/Article/details/gudwtyesd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.sjlbkw.cn/Article/details/guzfnubqz.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fktsv.cn/Article/details/gnnoqhjay.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.tarul.cn/Article/details/gsrucgusk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.sjlbkw.cn/Article/details/gfhcfirle.sHtML

[Q49] 更新单行
来源：http://3g.vehdjk.com/Article/details/guriyoayb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.yfazqb.com/Article/details/gqsqgkzhz.sHtML

[Q50] 批量更新
来源：http://blog.yfazqb.com/Article/details/gfyefeywg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.tarul.cn/Article/details/gjsagyigm.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fktsv.cn/Article/details/grdlitujr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.sjlbkw.cn/Article/details/ggpiifnrj.sHtML

[Q52] 删除指定行
来源：http://3g.sjlbkw.cn/Article/details/grzuicmsa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/gjeerxlvu.sHtML

[Q53] 按条件删除
来源：http://3g.fktsv.cn/Article/details/gyvruhglb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gkygsygho.sHtML

[Q54] 清空表
来源：http://m.share.tarul.cn/Article/details/gogpijrhy.sHtML

TRUNCATE TABLE logs;
来源：http://wap.sjlbkw.cn/Article/details/gopggkiub.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.yfazqb.com/Article/details/gjbjrgvku.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gpjqcflor.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.bbcook.cn/Article/details/gbvvihchn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqfcnsde.sHtML

[Q57] 行号
来源：http://read.share.bbcook.cn/Article/details/gmpjsmrcl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.yfazqb.com/Article/details/gprbyefte.sHtML

[Q58] 累计求和
来源：http://baike.epnwcf.com/Article/details/glebzhcme.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gxmryflgz.sHtML

[Q59] 分组内累计
来源：http://www.share.epnwcf.com/Article/details/gxulhqtvg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gtgxoroou.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.epnwcf.com/Article/details/grkasecao.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.vehdjk.com/Article/details/glfztvaqp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gfagkvrhq.sHtML

[Q61] 移动平均
来源：http://baike.sjlbkw.cn/Article/details/gnosgbjfj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.tarul.cn/Article/details/grvjddoog.sHtML

[Q62] 分组占比
来源：http://read.share.vehdjk.com/Article/details/gyipsxxrk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gbxrdheei.sHtML

[Q63] 开启事务
来源：http://m.share.yfazqb.com/Article/details/gsifkakbv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.sjlbkw.cn/Article/details/gcoqylvqc.sHtML

[Q64] 提交事务
来源：http://www.blog.fktsv.cn/Article/details/gatqzulxh.sHtML

COMMIT;
来源：http://read.share.tarul.cn/Article/details/ggvqmsvjg.sHtML

[Q65] 回滚事务
来源：http://www.blog.bbcook.cn/Article/details/gefrjonfl.sHtML

ROLLBACK;
来源：http://www.share.fktsv.cn/Article/details/gaemsmcav.sHtML

[Q66] 行锁查询
来源：http://www.m.share.bbcook.cn/Article/details/gfcffpqsl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.tarul.cn/Article/details/gnidldpwi.sHtML

[Q67] 设置隔离级别
来源：http://3g.sjlbkw.cn/Article/details/givokfskt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.sjlbkw.cn/Article/details/glrgyvlgz.sHtML

[Q68] 保存点
来源：http://www.m.share.epnwcf.com/Article/details/gapsrvqqj.sHtML

SAVEPOINT sp1;
来源：http://3g.vehdjk.com/Article/details/gweotyzmm.sHtML

ROLLBACK TO sp1;
来源：http://baike.bbcook.cn/Article/details/gxdzwzmdg.sHtML

[Q69] 查看执行计划
来源：http://read.share.fktsv.cn/Article/details/gkucxxvdu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.yfazqb.com/Article/details/gvdvcvhoy.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/gicudymme.sHtML

ANALYZE TABLE users;
来源：http://m.share.tarul.cn/Article/details/gfytkywhy.sHtML

[Q71] 查看建表语句
来源：http://read.share.sjlbkw.cn/Article/details/gucinmmel.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.epnwcf.com/Article/details/gccgxppnc.sHtML

[Q72] 查看索引
来源：http://mobile.vehdjk.com/Article/details/gccvagidv.sHtML

SHOW INDEX FROM users;
来源：http://baike.bbcook.cn/Article/details/gdcpqocym.sHtML

[Q73] 查看表状态
来源：http://3g.bbcook.cn/Article/details/gpatsifpj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.bbcook.cn/Article/details/glxbhammn.sHtML

[Q74] 强制使用索引
来源：http://3g.fktsv.cn/Article/details/gstxhsjhi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.vehdjk.com/Article/details/glfyxrdam.sHtML

[Q75] 日期格式化
来源：http://3g.bbcook.cn/Article/details/gmeuzgoon.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gqokylurh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.bbcook.cn/Article/details/gspsrgwzz.sHtML

[Q76] 按天统计
来源：http://www.m.share.yfazqb.com/Article/details/gznoxrijl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.sjlbkw.cn/Article/details/gfaqdorzr.sHtML

[Q77] 时间加减
来源：http://www.blog.vehdjk.com/Article/details/glkkgilaf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.epnwcf.com/Article/details/ghwjcfjub.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/gihlroyig.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.yfazqb.com/Article/details/gasilssze.sHtML

[Q79] 字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/gtnnjriiq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fktsv.cn/Article/details/gdsvozmva.sHtML

[Q80] 字符串截取
来源：http://www.blog.bbcook.cn/Article/details/gjaknyiaq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.epnwcf.com/Article/details/geediwykd.sHtML

[Q81] 字符串替换
来源：http://baike.bbcook.cn/Article/details/gopfrryhz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.vehdjk.com/Article/details/gvxbqovtz.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.yfazqb.com/Article/details/gpkiyoroy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gndqpwexj.sHtML

[Q83] 大小写转换
来源：http://3g.sjlbkw.cn/Article/details/guypwtbgu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/ggsgeihiy.sHtML

[Q84] 去除首尾空格
来源：http://mobile.tarul.cn/Article/details/gdpigzhrh.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gjvyvnyte.sHtML

[Q85] 数值取整
来源：http://mobile.tarul.cn/Article/details/ganakcauo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gxtvlnglt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.yfazqb.com/Article/details/ghuetmlqu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.bbcook.cn/Article/details/guslpcsak.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.epnwcf.com/Article/details/gxoiuvnzs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.vehdjk.com/Article/details/gjiyijkrg.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.yfazqb.com/Article/details/guebmrveg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.sjlbkw.cn/Article/details/gcacwvvcc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fktsv.cn/Article/details/gomxgvdos.sHtML

[Q89] 判断表是否存在
来源：http://wap.tarul.cn/Article/details/girmmhqfp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.vehdjk.com/Article/details/gfddguwlc.sHtML

[Q90] 生成序号列
来源：http://mobile.sjlbkw.cn/Article/details/goihbgfwm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.bbcook.cn/Article/details/gwurqmzjv.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gknikiwci.sHtML

R. Bash 专题
来源：http://blog.yfazqb.com/Article/details/goxuoxhao.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gspalcihp.sHtML

[R01] shebang 与严格模式
来源：http://m.share.sjlbkw.cn/Article/details/gmefmeecj.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.yfazqb.com/Article/details/gjzwmdqlp.sHtML

set -euo pipefail
来源：http://m.share.vehdjk.com/Article/details/gkqslgvil.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fktsv.cn/Article/details/gmddvlwsx.sHtML

name="Tom"; echo "$name"
来源：http://blog.yfazqb.com/Article/details/ghfpluztp.sHtML

[R03] 只读变量
来源：http://wap.sjlbkw.cn/Article/details/gwzmijeud.sHtML

readonly PI=3.14
来源：http://m.share.fktsv.cn/Article/details/gzffwhdal.sHtML

[R04] 位置参数
来源：http://wap.bbcook.cn/Article/details/gycgetghd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.sjlbkw.cn/Article/details/ggwtzxjvd.sHtML

[R05] 参数默认值
来源：http://www.share.vehdjk.com/Article/details/gwfoclijf.sHtML

name="${1:-default}"
来源：http://www.blog.yfazqb.com/Article/details/gnofbzhwu.sHtML

[R06] 判断命令是否存在
来源：http://baike.fktsv.cn/Article/details/gjqlzgghq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.yfazqb.com/Article/details/gkhpowayx.sHtML

[R07] if 判断文件
来源：http://wap.sjlbkw.cn/Article/details/ggbhpzvvv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fktsv.cn/Article/details/glslfdwoj.sHtML

[R08] 数值比较
来源：http://baike.vehdjk.com/Article/details/gmvwyabwi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.vehdjk.com/Article/details/gaajpepem.sHtML

[R09] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gzfufmifp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.yfazqb.com/Article/details/gjbyxgsin.sHtML

[R10] 正则匹配
来源：http://wap.tarul.cn/Article/details/gmogktifx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.epnwcf.com/Article/details/grfzojndn.sHtML

[R11] case 多分支
来源：http://blog.tarul.cn/Article/details/gqkfdmljz.sHtML

case "$1" in
来源：http://m.share.vehdjk.com/Article/details/ghpfohobq.sHtML

start) echo "启动" ;;
来源：http://blog.sjlbkw.cn/Article/details/gytssvcbl.sHtML

stop)  echo "停止" ;;
来源：http://3g.tarul.cn/Article/details/glrqxovws.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fktsv.cn/Article/details/gatmcfgrp.sHtML

esac
来源：http://m.share.tarul.cn/Article/details/gmaalswbb.sHtML

[R12] for 遍历文件
来源：http://wap.fktsv.cn/Article/details/groxulnvo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.sjlbkw.cn/Article/details/gevufjpzf.sHtML

[R13] for 计数循环
来源：http://www.m.share.fktsv.cn/Article/details/gdzrjvzvq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/gxsuwkshs.sHtML

[R14] C 风格 for
来源：http://m.share.sjlbkw.cn/Article/details/grlkdxhuk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/gkwndewhv.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gvrarjfvs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.tarul.cn/Article/details/gvbknvncg.sHtML

[R16] until 等待条件
来源：http://blog.sjlbkw.cn/Article/details/gmfxdcuta.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/gdnvutupw.sHtML

[R17] 数组定义与取值
来源：http://read.share.yfazqb.com/Article/details/gxnuxmrnd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.bbcook.cn/Article/details/gjaxnqiec.sHtML

[R18] 遍历数组
来源：http://baike.yfazqb.com/Article/details/gwljongcg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fktsv.cn/Article/details/gokzfxumo.sHtML

[R19] 数组长度
来源：http://3g.vehdjk.com/Article/details/gkzgscltg.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fktsv.cn/Article/details/gfjfxvcou.sHtML

[R20] 关联数组（字典）
来源：http://m.share.yfazqb.com/Article/details/glezcysmr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.epnwcf.com/Article/details/ggfpgepsi.sHtML

[R21] 字符串长度
来源：http://blog.epnwcf.com/Article/details/gdgrszxyt.sHtML

echo "${#s}"
来源：http://www.share.yfazqb.com/Article/details/gcotkkocr.sHtML

[R22] 截取子串
来源：http://m.share.fktsv.cn/Article/details/grknsimmq.sHtML

echo "${s:0:5}"
来源：http://www.share.bbcook.cn/Article/details/gcymgotzk.sHtML

[R23] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gwnqkuyow.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.sjlbkw.cn/Article/details/gnketoyvd.sHtML

[R24] 大小写转换
来源：http://www.share.tarul.cn/Article/details/ggnvrjgra.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.tarul.cn/Article/details/gyqmcwclc.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.bbcook.cn/Article/details/grllqkgcc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.bbcook.cn/Article/details/ginibsfxz.sHtML

[R26] 命令替换
来源：http://blog.epnwcf.com/Article/details/gpyszwugq.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fktsv.cn/Article/details/gpkuhekey.sHtML

[R27] 算术展开
来源：http://m.share.sjlbkw.cn/Article/details/ghjbvmhyx.sHtML

echo $((1 + 2 * 3))
来源：http://baike.vehdjk.com/Article/details/gofwwgjwv.sHtML

[R28] 浮点运算
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnktohpo.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/gtmxuumer.sHtML

[R29] 定义函数
来源：http://www.share.bbcook.cn/Article/details/gsywsxllb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.vehdjk.com/Article/details/gkfhuzkpo.sHtML

[R30] 函数返回状态码
来源：http://blog.tarul.cn/Article/details/ggdkgstlr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.epnwcf.com/Article/details/gmfmrrryb.sHtML

[R31] 局部变量
来源：http://m.share.tarul.cn/Article/details/grqoskmql.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.bbcook.cn/Article/details/gzshqbbjf.sHtML

[R32] 参数个数校验
来源：http://www.m.share.epnwcf.com/Article/details/giymsoiev.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gsfhelrvg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.epnwcf.com/Article/details/gssitazmm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.epnwcf.com/Article/details/gttsjnbkk.sHtML

[R34] 退出时清理
来源：http://wap.yfazqb.com/Article/details/gerhhadoi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/geqmwlbpm.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.sjlbkw.cn/Article/details/gafolkshg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.epnwcf.com/Article/details/gliijcnfn.sHtML

[R36] 并发执行多个任务
来源：http://blog.fktsv.cn/Article/details/glhwjxmjv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fktsv.cn/Article/details/giruvbwdn.sHtML

[R37] 把输出赋给变量
来源：http://3g.vehdjk.com/Article/details/goaprhxgj.sHtML

files=$(ls -1)
来源：http://www.blog.fktsv.cn/Article/details/gcgxcftyo.sHtML

[R38] 管道串联
来源：http://m.share.vehdjk.com/Article/details/ghapultxc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.bbcook.cn/Article/details/gknolnnhz.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.bbcook.cn/Article/details/ghtpeiwen.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/gurxthfgu.sHtML

[R40] 追加写日志
来源：http://blog.epnwcf.com/Article/details/gqqlakqsk.sHtML

echo "log" >> out.log
来源：http://baike.tarul.cn/Article/details/gbkhnhyrx.sHtML

[R41] 丢弃输出
来源：http://read.share.sjlbkw.cn/Article/details/gadgufwsv.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.vehdjk.com/Article/details/gpwefxrqv.sHtML

[R42] 输入重定向
来源：http://www.share.yfazqb.com/Article/details/gmarqbcio.sHtML

wc -l < a.txt
来源：http://blog.fktsv.cn/Article/details/gvejutylc.sHtML

[R43] 按名字查找文件
来源：http://3g.sjlbkw.cn/Article/details/gfmfqedzz.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.vehdjk.com/Article/details/gxzndrcpw.sHtML

[R44] 按修改时间查找
来源：http://mobile.epnwcf.com/Article/details/gltfqgzvm.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/gxrwqhrbj.sHtML

[R45] 批量删除
来源：http://blog.tarul.cn/Article/details/gvaaxwxyf.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.tarul.cn/Article/details/ghszugmcq.sHtML

[R46] 递归替换文件内容
来源：http://baike.tarul.cn/Article/details/ghwmwctty.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.sjlbkw.cn/Article/details/gcyulzuln.sHtML

[R47] sed 单行替换
来源：http://baike.bbcook.cn/Article/details/geucdlbbw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gwewzyvbl.sHtML

[R48] awk 取指定列
来源：http://baike.bbcook.cn/Article/details/gjeooagkc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/glfxyzope.sHtML

[R49] awk 带条件
来源：http://mobile.bbcook.cn/Article/details/ghcqsuvhr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.bbcook.cn/Article/details/gouougfcn.sHtML

[R50] awk 求和
来源：http://3g.yfazqb.com/Article/details/gkdjgklxr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.yfazqb.com/Article/details/guzgxbfzt.sHtML

[R51] 排序去重取前几
来源：http://www.share.sjlbkw.cn/Article/details/gtxthbwgo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.sjlbkw.cn/Article/details/gahlkmmxi.sHtML

[R52] 统计行数
来源：http://www.blog.vehdjk.com/Article/details/gfepayqgo.sHtML

wc -l a.txt
来源：http://www.blog.tarul.cn/Article/details/gmwdqquig.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.sjlbkw.cn/Article/details/glxsfzqor.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.sjlbkw.cn/Article/details/gnwdepihk.sHtML

[R54] 比较两个文件
来源：http://www.blog.vehdjk.com/Article/details/gppyefynp.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/glzkotpno.sHtML

[R55] 压缩与解压
来源：http://read.share.tarul.cn/Article/details/gincvaipc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.yfazqb.com/Article/details/gdhaiuony.sHtML

[R56] 远程拷贝
来源：http://www.share.fktsv.cn/Article/details/gkgzcazjd.sHtML

scp file user@host:/path/
来源：http://www.share.bbcook.cn/Article/details/gbfjxagxk.sHtML

[R57] 远程执行命令
来源：http://read.share.tarul.cn/Article/details/gpifcqwgo.sHtML

ssh user@host 'uptime'
来源：http://wap.epnwcf.com/Article/details/gsjvewptw.sHtML

[R58] 下载文件
来源：http://www.m.share.bbcook.cn/Article/details/gbmdzaajj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.bbcook.cn/Article/details/gneyxeree.sHtML

[R59] 发 POST JSON
来源：http://blog.epnwcf.com/Article/details/gwjuullco.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.vehdjk.com/Article/details/gktdnwhen.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/gobdrwttr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.sjlbkw.cn/Article/details/gptsaxzub.sHtML

[R61] 磁盘占用
来源：http://blog.tarul.cn/Article/details/geaqpxilr.sHtML

df -h;  du -sh *
来源：http://www.share.fktsv.cn/Article/details/gghvtmyzu.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.sjlbkw.cn/Article/details/gjwogwuxq.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.tarul.cn/Article/details/gqpefdhvj.sHtML

[R63] 内存与进程
来源：http://read.share.sjlbkw.cn/Article/details/gdjbmnnge.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.bbcook.cn/Article/details/gnwrecdad.sHtML

[R64] 结束进程
来源：http://mobile.bbcook.cn/Article/details/gdjysxmwn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.epnwcf.com/Article/details/goxdppzji.sHtML

[R65] 查看端口占用
来源：http://m.share.fktsv.cn/Article/details/gfekeulzg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.vehdjk.com/Article/details/gtyoqzuro.sHtML

[R66] 定时任务
来源：http://www.blog.epnwcf.com/Article/details/gccmcorpy.sHtML

crontab -e;  crontab -l
来源：http://wap.epnwcf.com/Article/details/gbtatkgkn.sHtML

[R67] 生成随机十六进制串
来源：http://baike.tarul.cn/Article/details/ghqhzbzug.sHtML

openssl rand -hex 16
来源：http://baike.yfazqb.com/Article/details/gjjikskjc.sHtML

[R68] 计算文件校验值
来源：http://read.share.fktsv.cn/Article/details/gisngalss.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.yfazqb.com/Article/details/gqztzdves.sHtML

[R69] 生成随机密码
来源：http://mobile.yfazqb.com/Article/details/gplbrjrpt.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.bbcook.cn/Article/details/gxkcfozjx.sHtML

[R70] 时间戳与互转
来源：http://3g.bbcook.cn/Article/details/gxixqyycr.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fktsv.cn/Article/details/ggfzohpur.sHtML

[R71] 日期格式化
来源：http://wap.bbcook.cn/Article/details/ggghtxkst.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.sjlbkw.cn/Article/details/gsbjflwhb.sHtML

[R72] 等待端口就绪
来源：http://wap.bbcook.cn/Article/details/grjdnajib.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/gzvjatvxg.sHtML

[R73] 分割大日志
来源：http://www.blog.sjlbkw.cn/Article/details/gjajfzwry.sHtML

split -l 1000 big.log part_
来源：http://mobile.epnwcf.com/Article/details/gnmtfrgek.sHtML

[R74] 批量重命名
来源：http://www.m.share.epnwcf.com/Article/details/gbxfzxplh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fktsv.cn/Article/details/gbtsdntqk.sHtML

[R75] 导出环境变量
来源：http://www.share.yfazqb.com/Article/details/gfgyghokz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.tarul.cn/Article/details/giqzqdgpu.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/gcpcacift.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/ggyvxgxje.sHtML

[R77] 读取用户输入
来源：http://read.share.tarul.cn/Article/details/gvkrnanrv.sHtML

read -rp "请输入: " ans
来源：http://wap.epnwcf.com/Article/details/gchkvlhho.sHtML

[R78] 交互式菜单
来源：http://baike.sjlbkw.cn/Article/details/gjwmrkafc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.vehdjk.com/Article/details/gyakfbboo.sHtML

[R79] 解析命令行选项
来源：http://baike.fktsv.cn/Article/details/gamyovsqz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.vehdjk.com/Article/details/gzyssogbh.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.yfazqb.com/Article/details/gdgoexdcl.sHtML

time ./run.sh
来源：http://m.share.vehdjk.com/Article/details/gxxigmdyw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gkozajebf.sHtML

S. C / C++ 专题
来源：http://3g.vehdjk.com/Article/details/gxpvhskrr.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxtxiskpd.sHtML

[S01] C：Hello World
来源：http://3g.vehdjk.com/Article/details/gxfezgzey.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/grivwpmhz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.sjlbkw.cn/Article/details/gnyibxmjo.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.yfazqb.com/Article/details/gvlsmwhqc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.tarul.cn/Article/details/grswirftf.sHtML

[S03] C：读入整数
来源：http://www.m.share.bbcook.cn/Article/details/gwumrowzm.sHtML

int x; scanf("%d", &x);
来源：http://www.share.sjlbkw.cn/Article/details/gtjasbagb.sHtML

[S04] C：字符串复制
来源：http://mobile.sjlbkw.cn/Article/details/gmbtqotfi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.sjlbkw.cn/Article/details/gwltsaqei.sHtML

[S05] C：字符串长度
来源：http://mobile.yfazqb.com/Article/details/ghqyrkeib.sHtML

strlen(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gpynppmcn.sHtML

[S06] C：字符串比较
来源：http://wap.tarul.cn/Article/details/gchujfcci.sHtML

strcmp(a, b) == 0
来源：http://read.share.bbcook.cn/Article/details/gvlwwfsve.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gwputbewd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.yfazqb.com/Article/details/gblovaahk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.vehdjk.com/Article/details/gfuelobnp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.sjlbkw.cn/Article/details/gvfpbtrbi.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fktsv.cn/Article/details/gqqohmjpv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fktsv.cn/Article/details/gpwvrvarr.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtqoqpbm.sHtML

int *p = &a;  *p = 5;
来源：http://blog.tarul.cn/Article/details/gxeophpdt.sHtML

[S11] C：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gjydxtihz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.yfazqb.com/Article/details/ghdlppapv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.bbcook.cn/Article/details/gukbkgkct.sHtML

fclose(f);
来源：http://3g.tarul.cn/Article/details/gagsyiarg.sHtML

[S12] C：写文件
来源：http://3g.fktsv.cn/Article/details/gjsafbeeh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/gocqmngvu.sHtML

[S13] C：宏定义
来源：http://read.share.sjlbkw.cn/Article/details/gvlhimfrb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.tarul.cn/Article/details/gjuzwkvaw.sHtML

[S14] C：枚举
来源：http://www.blog.epnwcf.com/Article/details/gslcahpzh.sHtML


<!-- 参考信息 -->