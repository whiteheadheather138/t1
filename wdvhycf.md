代发 wailian999

[Q44] IN 子查询
来源：http://www.blog.epnwcf.com/Article/details/gaxebrnlv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.yfazqb.com/Article/details/gsvqpvovq.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fktsv.cn/Article/details/gdvsdnbmc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gowbxipnd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fktsv.cn/Article/details/griryqspa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gwgybcvyh.sHtML

[Q47] 与平均值比较
来源：http://mobile.tarul.cn/Article/details/gxzmcoirc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fktsv.cn/Article/details/gbftlutnx.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.tarul.cn/Article/details/gxqwzvhia.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.vehdjk.com/Article/details/gkmtqgkjp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.yfazqb.com/Article/details/gqiwmcjne.sHtML

[Q49] 更新单行
来源：http://baike.sjlbkw.cn/Article/details/govyjbzms.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.sjlbkw.cn/Article/details/ghfrgwgfs.sHtML

[Q50] 批量更新
来源：http://3g.epnwcf.com/Article/details/gyikqfyiy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fktsv.cn/Article/details/gumjixkes.sHtML

[Q51] 用子查询更新
来源：http://read.share.yfazqb.com/Article/details/ggrmcqbly.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.sjlbkw.cn/Article/details/gpsapiaty.sHtML

[Q52] 删除指定行
来源：http://3g.vehdjk.com/Article/details/gozyhjowc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/gczooktsc.sHtML

[Q53] 按条件删除
来源：http://wap.tarul.cn/Article/details/gbesnhktz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fktsv.cn/Article/details/gdcxwwrur.sHtML

[Q54] 清空表
来源：http://baike.bbcook.cn/Article/details/gxxylhfcw.sHtML

TRUNCATE TABLE logs;
来源：http://blog.bbcook.cn/Article/details/gdcdjxfet.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.yfazqb.com/Article/details/gragmikan.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gamymogtx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.sjlbkw.cn/Article/details/gyndkvrse.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.tarul.cn/Article/details/ggdqsegye.sHtML

[Q57] 行号
来源：http://blog.fktsv.cn/Article/details/gltdxdwqq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fktsv.cn/Article/details/gcnkfldyl.sHtML

[Q58] 累计求和
来源：http://blog.epnwcf.com/Article/details/glsdkotqg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.yfazqb.com/Article/details/gyurdhuha.sHtML

[Q59] 分组内累计
来源：http://www.share.epnwcf.com/Article/details/ghqjjiwms.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gshtwwsvc.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.vehdjk.com/Article/details/gezvgoldh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fktsv.cn/Article/details/gswlhkrso.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gwtbxviol.sHtML

[Q61] 移动平均
来源：http://www.share.vehdjk.com/Article/details/gacifxaie.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gcackjrza.sHtML

[Q62] 分组占比
来源：http://3g.vehdjk.com/Article/details/gyswhvxbh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/glzhwqzlv.sHtML

[Q63] 开启事务
来源：http://m.share.sjlbkw.cn/Article/details/gsgdtgqfk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.bbcook.cn/Article/details/gcaxanwrg.sHtML

[Q64] 提交事务
来源：http://wap.fktsv.cn/Article/details/gdovzeafb.sHtML

COMMIT;
来源：http://www.share.tarul.cn/Article/details/grggsvrft.sHtML

[Q65] 回滚事务
来源：http://www.share.fktsv.cn/Article/details/gholxfdxx.sHtML

ROLLBACK;
来源：http://blog.epnwcf.com/Article/details/gruivawfb.sHtML

[Q66] 行锁查询
来源：http://www.blog.fktsv.cn/Article/details/ggeetnque.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.epnwcf.com/Article/details/gghihpsik.sHtML

[Q67] 设置隔离级别
来源：http://baike.vehdjk.com/Article/details/gyoknzead.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fktsv.cn/Article/details/gnnnkoaxi.sHtML

[Q68] 保存点
来源：http://blog.sjlbkw.cn/Article/details/guytblnza.sHtML

SAVEPOINT sp1;
来源：http://read.share.epnwcf.com/Article/details/gsfcnvfdy.sHtML

ROLLBACK TO sp1;
来源：http://blog.tarul.cn/Article/details/gtztgxmml.sHtML

[Q69] 查看执行计划
来源：http://blog.yfazqb.com/Article/details/geogsjjfr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.epnwcf.com/Article/details/gququnohm.sHtML

[Q70] 更新统计信息
来源：http://baike.vehdjk.com/Article/details/gipijpkrl.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.yfazqb.com/Article/details/grjregugz.sHtML

[Q71] 查看建表语句
来源：http://mobile.sjlbkw.cn/Article/details/gjftnjrfy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.yfazqb.com/Article/details/gnbtrdlsj.sHtML

[Q72] 查看索引
来源：http://www.m.share.sjlbkw.cn/Article/details/galgqsuvo.sHtML

SHOW INDEX FROM users;
来源：http://wap.bbcook.cn/Article/details/glnpbduha.sHtML

[Q73] 查看表状态
来源：http://blog.epnwcf.com/Article/details/gnvihjsqr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.tarul.cn/Article/details/gyrczegzq.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gcetjxztb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.sjlbkw.cn/Article/details/gmgxehulb.sHtML

[Q75] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gbbrxmnxe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.tarul.cn/Article/details/grhqzoqxe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.tarul.cn/Article/details/gqvfibrtf.sHtML

[Q76] 按天统计
来源：http://mobile.fktsv.cn/Article/details/gwxpigvbn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.yfazqb.com/Article/details/gwismimps.sHtML

[Q77] 时间加减
来源：http://baike.bbcook.cn/Article/details/ggibckvdi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fktsv.cn/Article/details/grtwyyyif.sHtML

[Q78] 当前时间
来源：http://www.share.vehdjk.com/Article/details/gpesfsxnl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.epnwcf.com/Article/details/gugmdiiai.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.vehdjk.com/Article/details/giwxmwbbq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/gcfkvspzi.sHtML

[Q80] 字符串截取
来源：http://m.share.bbcook.cn/Article/details/gezvuyqet.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.vehdjk.com/Article/details/ghinpgoak.sHtML

[Q81] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gmpcmzpku.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.epnwcf.com/Article/details/gtsxmxmqf.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.vehdjk.com/Article/details/guqkiivcw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/ggujytgug.sHtML

[Q83] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/gxoqwtrxi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gyfplsxfm.sHtML

[Q84] 去除首尾空格
来源：http://blog.epnwcf.com/Article/details/gleqtubfg.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gontzblkz.sHtML

[Q85] 数值取整
来源：http://www.m.share.vehdjk.com/Article/details/gdowqgjzz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.vehdjk.com/Article/details/ghaalujjj.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fktsv.cn/Article/details/ghfyubkmo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.yfazqb.com/Article/details/gnhvjcgmt.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.yfazqb.com/Article/details/gndyqdykc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.epnwcf.com/Article/details/gtekwnixt.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.yfazqb.com/Article/details/grzcnfrcu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.sjlbkw.cn/Article/details/grgncujlh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.bbcook.cn/Article/details/gmorurbta.sHtML

[Q89] 判断表是否存在
来源：http://blog.bbcook.cn/Article/details/gjonbvghh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.sjlbkw.cn/Article/details/gkyywpwbq.sHtML

[Q90] 生成序号列
来源：http://read.share.fktsv.cn/Article/details/gddyhrjvw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.bbcook.cn/Article/details/ggusrjtgd.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfamlgzjh.sHtML

R. Bash 专题
来源：http://m.share.fktsv.cn/Article/details/gboatshua.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gpbwykkdq.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.epnwcf.com/Article/details/gxaykqleg.sHtML

#!/usr/bin/env bash
来源：http://wap.yfazqb.com/Article/details/glwljbrxt.sHtML

set -euo pipefail
来源：http://read.share.bbcook.cn/Article/details/gwaphwtbv.sHtML

[R02] 变量赋值与使用
来源：http://read.share.bbcook.cn/Article/details/gkpiicqby.sHtML

name="Tom"; echo "$name"
来源：http://baike.vehdjk.com/Article/details/gjjbuwsdj.sHtML

[R03] 只读变量
来源：http://baike.sjlbkw.cn/Article/details/guljpamhl.sHtML

readonly PI=3.14
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbshrgpc.sHtML

[R04] 位置参数
来源：http://mobile.vehdjk.com/Article/details/gjzkjzlnm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.yfazqb.com/Article/details/gufztzdbp.sHtML

[R05] 参数默认值
来源：http://m.share.bbcook.cn/Article/details/gzjfanvwo.sHtML

name="${1:-default}"
来源：http://www.blog.tarul.cn/Article/details/gwausjrns.sHtML

[R06] 判断命令是否存在
来源：http://3g.yfazqb.com/Article/details/ghqspsqwh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/gjlxgnifv.sHtML

[R07] if 判断文件
来源：http://www.blog.yfazqb.com/Article/details/gnpxhpvtp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.tarul.cn/Article/details/goyhgopea.sHtML

[R08] 数值比较
来源：http://www.share.yfazqb.com/Article/details/gvgivomwb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.bbcook.cn/Article/details/gjmkjrtwn.sHtML

[R09] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/ggsizdlpo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/gypkallxw.sHtML

[R10] 正则匹配
来源：http://m.share.fktsv.cn/Article/details/gijpmdgvo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.bbcook.cn/Article/details/guviepysj.sHtML

[R11] case 多分支
来源：http://wap.vehdjk.com/Article/details/giwuekzif.sHtML

case "$1" in
来源：http://www.m.share.bbcook.cn/Article/details/gokrooyyp.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/gyfppbsof.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.tarul.cn/Article/details/gtqukvxab.sHtML

*)     echo "未知命令" ;;
来源：http://3g.sjlbkw.cn/Article/details/gzhsvyuff.sHtML

esac
来源：http://wap.sjlbkw.cn/Article/details/gpltbyuti.sHtML

[R12] for 遍历文件
来源：http://read.share.sjlbkw.cn/Article/details/gxyaaghus.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.vehdjk.com/Article/details/gwsunwscx.sHtML

[R13] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/ghixvpwqg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/grylpjjug.sHtML

[R14] C 风格 for
来源：http://read.share.yfazqb.com/Article/details/gdllhgvij.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gentjgdrl.sHtML

[R15] while 逐行读文件
来源：http://blog.tarul.cn/Article/details/gbeefbwln.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.tarul.cn/Article/details/gusrwibsh.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/goshjshum.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/gjjmndvfn.sHtML

[R17] 数组定义与取值
来源：http://wap.vehdjk.com/Article/details/grcomdvgo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/gcployirj.sHtML

[R18] 遍历数组
来源：http://blog.epnwcf.com/Article/details/ghrhhonib.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/gbxxqxhvo.sHtML

[R19] 数组长度
来源：http://www.share.epnwcf.com/Article/details/gvrwhrwdz.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/gqdtrtqbj.sHtML

[R20] 关联数组（字典）
来源：http://3g.fktsv.cn/Article/details/gbxtyokrq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/ghobtsboa.sHtML

[R21] 字符串长度
来源：http://read.share.tarul.cn/Article/details/gnhtmoaxy.sHtML

echo "${#s}"
来源：http://3g.epnwcf.com/Article/details/gfpedapis.sHtML

[R22] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gehwwadru.sHtML

echo "${s:0:5}"
来源：http://mobile.vehdjk.com/Article/details/gwagbtumi.sHtML

[R23] 字符串替换
来源：http://blog.fktsv.cn/Article/details/guxhilfij.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.sjlbkw.cn/Article/details/gaqqgnenu.sHtML

[R24] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gqgfftylg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.vehdjk.com/Article/details/gnxidledh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.vehdjk.com/Article/details/gtkfkzcfg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.vehdjk.com/Article/details/gpvzzduza.sHtML

[R26] 命令替换
来源：http://www.m.share.vehdjk.com/Article/details/gmazinovc.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fktsv.cn/Article/details/ggugfmsnv.sHtML

[R27] 算术展开
来源：http://mobile.bbcook.cn/Article/details/guydywekp.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.tarul.cn/Article/details/glgaubquk.sHtML

[R28] 浮点运算
来源：http://www.share.epnwcf.com/Article/details/gyrfqkynn.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/gnhgcyqmi.sHtML

[R29] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/glhbjvmgy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fktsv.cn/Article/details/gcbcfskme.sHtML

[R30] 函数返回状态码
来源：http://read.share.fktsv.cn/Article/details/gobxxkiyr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.vehdjk.com/Article/details/gpbyfsnon.sHtML

[R31] 局部变量
来源：http://blog.vehdjk.com/Article/details/ggjokupcz.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.bbcook.cn/Article/details/gohwxznsb.sHtML

[R32] 参数个数校验
来源：http://baike.sjlbkw.cn/Article/details/gtprrnxlh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/gtbuzdswe.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fktsv.cn/Article/details/gligsmggj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.bbcook.cn/Article/details/gglsfzcya.sHtML

[R34] 退出时清理
来源：http://m.share.vehdjk.com/Article/details/gsbdecaff.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gobobhmik.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fktsv.cn/Article/details/gkalmuvor.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.sjlbkw.cn/Article/details/gkmkrsntf.sHtML

[R36] 并发执行多个任务
来源：http://blog.epnwcf.com/Article/details/glbcarnej.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.sjlbkw.cn/Article/details/gaovueyqd.sHtML

[R37] 把输出赋给变量
来源：http://read.share.yfazqb.com/Article/details/gjaygvizn.sHtML

files=$(ls -1)
来源：http://wap.yfazqb.com/Article/details/gtdhyiivp.sHtML

[R38] 管道串联
来源：http://wap.vehdjk.com/Article/details/ghsleofni.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fktsv.cn/Article/details/gjkzygowi.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.vehdjk.com/Article/details/ggvlbquqx.sHtML

cmd > out.log 2>&1
来源：http://mobile.bbcook.cn/Article/details/gyudtgtcc.sHtML

[R40] 追加写日志
来源：http://www.share.epnwcf.com/Article/details/gyfcwfymu.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/gcwhjabfm.sHtML

[R41] 丢弃输出
来源：http://read.share.yfazqb.com/Article/details/gmwbhvcls.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fktsv.cn/Article/details/geczuhows.sHtML

[R42] 输入重定向
来源：http://read.share.vehdjk.com/Article/details/gbaathsid.sHtML

wc -l < a.txt
来源：http://blog.sjlbkw.cn/Article/details/gmunutjyn.sHtML

[R43] 按名字查找文件
来源：http://www.share.yfazqb.com/Article/details/gunckcbac.sHtML

find . -name "*.log" -type f
来源：http://blog.epnwcf.com/Article/details/gwueaitlg.sHtML

[R44] 按修改时间查找
来源：http://www.share.tarul.cn/Article/details/gisqsglcz.sHtML

find . -mtime -7 -type f
来源：http://www.share.epnwcf.com/Article/details/gnynxbaya.sHtML

[R45] 批量删除
来源：http://www.share.bbcook.cn/Article/details/gucbyabff.sHtML

find . -name "*.tmp" -delete
来源：http://blog.epnwcf.com/Article/details/gprimzczh.sHtML

[R46] 递归替换文件内容
来源：http://read.share.epnwcf.com/Article/details/gxarwpozh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.yfazqb.com/Article/details/gczjpkpvv.sHtML

[R47] sed 单行替换
来源：http://blog.fktsv.cn/Article/details/gefwhgghq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.tarul.cn/Article/details/gtvzngqkz.sHtML

[R48] awk 取指定列
来源：http://wap.bbcook.cn/Article/details/gknoldyro.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fktsv.cn/Article/details/ggcdymcnt.sHtML

[R49] awk 带条件
来源：http://baike.vehdjk.com/Article/details/germaecfm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.tarul.cn/Article/details/gonhitbxi.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/ggcxnvntm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.vehdjk.com/Article/details/gloarwjyn.sHtML

[R51] 排序去重取前几
来源：http://mobile.fktsv.cn/Article/details/gchemfeea.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.vehdjk.com/Article/details/giglshjlh.sHtML

[R52] 统计行数
来源：http://read.share.bbcook.cn/Article/details/gqvzxgkay.sHtML

wc -l a.txt
来源：http://www.share.bbcook.cn/Article/details/gszzpnvrt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.yfazqb.com/Article/details/glbtxdqeb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.epnwcf.com/Article/details/gprqlffuf.sHtML

[R54] 比较两个文件
来源：http://baike.vehdjk.com/Article/details/gszlyqcyf.sHtML

diff a.txt b.txt
来源：http://baike.vehdjk.com/Article/details/gpteoaraj.sHtML

[R55] 压缩与解压
来源：http://www.blog.sjlbkw.cn/Article/details/gcdguhlfe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.bbcook.cn/Article/details/gfffdnrxf.sHtML

[R56] 远程拷贝
来源：http://baike.tarul.cn/Article/details/gfsunxrsl.sHtML

scp file user@host:/path/
来源：http://mobile.sjlbkw.cn/Article/details/gilfwuhmc.sHtML

[R57] 远程执行命令
来源：http://mobile.tarul.cn/Article/details/guqghzrrw.sHtML

ssh user@host 'uptime'
来源：http://m.share.sjlbkw.cn/Article/details/gvvqppxje.sHtML

[R58] 下载文件
来源：http://baike.yfazqb.com/Article/details/gauljysgm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.bbcook.cn/Article/details/gxitaward.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/gzhhxhvbv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.bbcook.cn/Article/details/goplcyxeb.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/giozemvzu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fktsv.cn/Article/details/gpctjawei.sHtML

[R61] 磁盘占用
来源：http://blog.yfazqb.com/Article/details/gvwwtnzcu.sHtML

df -h;  du -sh *
来源：http://read.share.yfazqb.com/Article/details/gjcvmkakw.sHtML

[R62] 找最占空间的文件
来源：http://baike.tarul.cn/Article/details/gkvdkgtdh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.yfazqb.com/Article/details/gmiveuojg.sHtML

[R63] 内存与进程
来源：http://blog.bbcook.cn/Article/details/gqhccvshu.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.bbcook.cn/Article/details/gieldqwlv.sHtML

[R64] 结束进程
来源：http://read.share.epnwcf.com/Article/details/gphpkfvzo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.yfazqb.com/Article/details/gmsjlfbpk.sHtML

[R65] 查看端口占用
来源：http://read.share.sjlbkw.cn/Article/details/gpswexsfn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fktsv.cn/Article/details/gntrxbmhs.sHtML

[R66] 定时任务
来源：http://wap.sjlbkw.cn/Article/details/gawovjlmq.sHtML

crontab -e;  crontab -l
来源：http://baike.tarul.cn/Article/details/gunorszyt.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fktsv.cn/Article/details/gilzwxrmk.sHtML

openssl rand -hex 16
来源：http://3g.yfazqb.com/Article/details/gtjtcveve.sHtML

[R68] 计算文件校验值
来源：http://m.share.tarul.cn/Article/details/gqdmteqwb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gzydditge.sHtML

[R69] 生成随机密码
来源：http://baike.epnwcf.com/Article/details/grzmsnxot.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fktsv.cn/Article/details/gjljeggtw.sHtML

[R70] 时间戳与互转
来源：http://read.share.fktsv.cn/Article/details/gijykazrg.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.vehdjk.com/Article/details/gsmysofdk.sHtML

[R71] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gvtdkflqz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.bbcook.cn/Article/details/gfbmwjyxg.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fktsv.cn/Article/details/gfnbdzidi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/gsednbeta.sHtML

[R73] 分割大日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrrzaegl.sHtML

split -l 1000 big.log part_
来源：http://www.share.epnwcf.com/Article/details/gcubwqorm.sHtML

[R74] 批量重命名
来源：http://www.m.share.fktsv.cn/Article/details/gefxckbxq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fktsv.cn/Article/details/gaomskqox.sHtML

[R75] 导出环境变量
来源：http://www.blog.bbcook.cn/Article/details/golhsyaez.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fktsv.cn/Article/details/gxlpggpbq.sHtML

[R76] 使用临时文件
来源：http://m.share.tarul.cn/Article/details/gwkolsbzl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/glkjiooum.sHtML

[R77] 读取用户输入
来源：http://3g.yfazqb.com/Article/details/gsjmrdbpy.sHtML

read -rp "请输入: " ans
来源：http://m.share.bbcook.cn/Article/details/gdjbhxidd.sHtML

[R78] 交互式菜单
来源：http://read.share.tarul.cn/Article/details/gsyicfszy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.tarul.cn/Article/details/gdvepostx.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gjpmyshwc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.sjlbkw.cn/Article/details/gfgcwqgdi.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fktsv.cn/Article/details/grbewjzku.sHtML

time ./run.sh
来源：http://mobile.yfazqb.com/Article/details/gluxgyqfu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gmjksujwe.sHtML

S. C / C++ 专题
来源：http://www.share.epnwcf.com/Article/details/ghxwvlvwk.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbrdvbvqn.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gibrmwvri.sHtML

#include <stdio.h>
来源：http://baike.bbcook.cn/Article/details/grkysmrzv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.epnwcf.com/Article/details/gxngnrgbm.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.tarul.cn/Article/details/gqaoakirl.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.bbcook.cn/Article/details/gfbelldbi.sHtML

[S03] C：读入整数
来源：http://www.blog.fktsv.cn/Article/details/grhawlgnc.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjjhxeic.sHtML

[S04] C：字符串复制
来源：http://m.share.yfazqb.com/Article/details/gprenzutq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.tarul.cn/Article/details/gpdgfacyl.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/gekzbadnl.sHtML

strlen(s)
来源：http://m.share.vehdjk.com/Article/details/gugswcoic.sHtML

[S06] C：字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gfrzahhfa.sHtML

strcmp(a, b) == 0
来源：http://www.share.fktsv.cn/Article/details/gxeyequku.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/gqwrxajud.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.tarul.cn/Article/details/gyeuiodyd.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.yfazqb.com/Article/details/gpimsedfv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.bbcook.cn/Article/details/gbylxphsp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.yfazqb.com/Article/details/godtiextw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.tarul.cn/Article/details/gxvuiania.sHtML

[S10] C：指针与解引用
来源：http://wap.vehdjk.com/Article/details/gkulytlhw.sHtML

int *p = &a;  *p = 5;
来源：http://wap.vehdjk.com/Article/details/gyojlyrdx.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gmgptulnj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.vehdjk.com/Article/details/gjhuxiiug.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.yfazqb.com/Article/details/ghhbsftgk.sHtML

fclose(f);
来源：http://blog.vehdjk.com/Article/details/gsuzcumno.sHtML

[S12] C：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gfjhnnfeb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.tarul.cn/Article/details/ghbeabbpx.sHtML

[S13] C：宏定义
来源：http://wap.bbcook.cn/Article/details/gzgqzfeed.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.tarul.cn/Article/details/gogvsybfg.sHtML

[S14] C：枚举
来源：http://mobile.vehdjk.com/Article/details/gopxzfeta.sHtML


<!-- 参考信息 -->