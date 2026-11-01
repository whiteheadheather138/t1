代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://m.share.tarul.cn/Article/details/giizqdbzp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.sjlbkw.cn/Article/details/gntxkcceh.sHtML

[Q43] 标量子查询
来源：http://m.share.epnwcf.com/Article/details/grifybvmy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fktsv.cn/Article/details/givulugau.sHtML

[Q44] IN 子查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzrdzpkt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fktsv.cn/Article/details/ghpicfzst.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.bbcook.cn/Article/details/ggqbrxukt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gpoyoimvn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.yfazqb.com/Article/details/gugegpqjl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.sjlbkw.cn/Article/details/gheuhkusr.sHtML

[Q47] 与平均值比较
来源：http://m.share.sjlbkw.cn/Article/details/gpnkcuqmd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.tarul.cn/Article/details/glchekbjx.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.bbcook.cn/Article/details/gzugfajib.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.vehdjk.com/Article/details/gygiqyrpa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.yfazqb.com/Article/details/gnvyktgoh.sHtML

[Q49] 更新单行
来源：http://wap.fktsv.cn/Article/details/gopynoiyc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gcindochh.sHtML

[Q50] 批量更新
来源：http://www.share.epnwcf.com/Article/details/gqmlfnblu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.vehdjk.com/Article/details/gcvdfxvam.sHtML

[Q51] 用子查询更新
来源：http://www.share.fktsv.cn/Article/details/gbwmtynic.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gxurbkeav.sHtML

[Q52] 删除指定行
来源：http://read.share.yfazqb.com/Article/details/gsfsbghqh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/glsgrtdxe.sHtML

[Q53] 按条件删除
来源：http://3g.epnwcf.com/Article/details/gwidthxcz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fktsv.cn/Article/details/gvhdychps.sHtML

[Q54] 清空表
来源：http://blog.vehdjk.com/Article/details/gzxhwnlav.sHtML

TRUNCATE TABLE logs;
来源：http://baike.yfazqb.com/Article/details/gxdjrhvuf.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbujrofze.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.epnwcf.com/Article/details/gkvxusdpt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.epnwcf.com/Article/details/gcvukkgnz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.vehdjk.com/Article/details/gjoukjceb.sHtML

[Q57] 行号
来源：http://baike.fktsv.cn/Article/details/gfzvxhapk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.tarul.cn/Article/details/gwbhohnrc.sHtML

[Q58] 累计求和
来源：http://blog.bbcook.cn/Article/details/guqahcbbt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fktsv.cn/Article/details/gbchepdpp.sHtML

[Q59] 分组内累计
来源：http://3g.epnwcf.com/Article/details/gvibuhbjx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gbokmvtpx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.sjlbkw.cn/Article/details/gssjkamas.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fktsv.cn/Article/details/ggedlbide.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.tarul.cn/Article/details/gxrocfbck.sHtML

[Q61] 移动平均
来源：http://blog.bbcook.cn/Article/details/gtjtzvita.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/ggmhnhdjh.sHtML

[Q62] 分组占比
来源：http://baike.vehdjk.com/Article/details/grtlzikmo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gfjmdgnmj.sHtML

[Q63] 开启事务
来源：http://read.share.bbcook.cn/Article/details/grtwqrsth.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.bbcook.cn/Article/details/gzscgggig.sHtML

[Q64] 提交事务
来源：http://mobile.yfazqb.com/Article/details/gptmsejwb.sHtML

COMMIT;
来源：http://blog.fktsv.cn/Article/details/gezvzivrv.sHtML

[Q65] 回滚事务
来源：http://m.share.tarul.cn/Article/details/gxfhxsrao.sHtML

ROLLBACK;
来源：http://www.share.tarul.cn/Article/details/gpoulvpik.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fktsv.cn/Article/details/gngatfzvw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.tarul.cn/Article/details/gwqaeoutr.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.epnwcf.com/Article/details/gpdubsnks.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.yfazqb.com/Article/details/gsqqvihsc.sHtML

[Q68] 保存点
来源：http://www.blog.epnwcf.com/Article/details/gzcrahmuj.sHtML

SAVEPOINT sp1;
来源：http://3g.sjlbkw.cn/Article/details/ghkfajlqj.sHtML

ROLLBACK TO sp1;
来源：http://blog.bbcook.cn/Article/details/gjjmeypic.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gxfawtway.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.vehdjk.com/Article/details/gxwkgiwrv.sHtML

[Q70] 更新统计信息
来源：http://m.share.epnwcf.com/Article/details/gwnouslzi.sHtML

ANALYZE TABLE users;
来源：http://www.blog.bbcook.cn/Article/details/gxlgkzrvf.sHtML

[Q71] 查看建表语句
来源：http://blog.vehdjk.com/Article/details/ggnmgmjnv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.bbcook.cn/Article/details/gdoczwdcn.sHtML

[Q72] 查看索引
来源：http://wap.vehdjk.com/Article/details/gnsqmsotc.sHtML

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/guhpxritl.sHtML

[Q73] 查看表状态
来源：http://3g.epnwcf.com/Article/details/gflqevsty.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.bbcook.cn/Article/details/gmuqkkyrw.sHtML

[Q74] 强制使用索引
来源：http://baike.vehdjk.com/Article/details/goyeoqasp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.vehdjk.com/Article/details/gnzhspyfn.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gueyjqcut.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fktsv.cn/Article/details/ghrijiaww.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fktsv.cn/Article/details/gfwwwznsv.sHtML

[Q76] 按天统计
来源：http://www.share.epnwcf.com/Article/details/gfeqchsgf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fktsv.cn/Article/details/grsbemvpm.sHtML

[Q77] 时间加减
来源：http://read.share.fktsv.cn/Article/details/gklqegqpe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.sjlbkw.cn/Article/details/gztgyaxgg.sHtML

[Q78] 当前时间
来源：http://m.share.epnwcf.com/Article/details/gurzlffkn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.tarul.cn/Article/details/gfbroueux.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gczmecymo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.vehdjk.com/Article/details/gotgggigd.sHtML

[Q80] 字符串截取
来源：http://baike.vehdjk.com/Article/details/gxkvzbbkz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.tarul.cn/Article/details/glhssxutt.sHtML

[Q81] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/guoxearft.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.vehdjk.com/Article/details/gukkhphvp.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.bbcook.cn/Article/details/gdstoojci.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gzlvfgzjj.sHtML

[Q83] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gfjkdzdnk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/guwiinkzn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.epnwcf.com/Article/details/gxpdryrwf.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gsxwlzjye.sHtML

[Q85] 数值取整
来源：http://wap.bbcook.cn/Article/details/gdtyajdrw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.tarul.cn/Article/details/gjjudofqr.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.sjlbkw.cn/Article/details/gclgflyyd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.tarul.cn/Article/details/gdgrmlwsb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.bbcook.cn/Article/details/ghpmtfuea.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.vehdjk.com/Article/details/gxeuembui.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.sjlbkw.cn/Article/details/gaxezbnhf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.sjlbkw.cn/Article/details/gvwcbklxn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.tarul.cn/Article/details/grfwaropj.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/ggzzsqbnn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gxajfzxbu.sHtML

[Q90] 生成序号列
来源：http://blog.tarul.cn/Article/details/gooblfgfv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fktsv.cn/Article/details/gshbruhap.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gpcwdjknh.sHtML

R. Bash 专题
来源：http://www.blog.fktsv.cn/Article/details/grgeurntn.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gvlhdkdvu.sHtML

[R01] shebang 与严格模式
来源：http://wap.epnwcf.com/Article/details/geznyxwas.sHtML

#!/usr/bin/env bash
来源：http://baike.yfazqb.com/Article/details/gdsfdfwqs.sHtML

set -euo pipefail
来源：http://www.blog.sjlbkw.cn/Article/details/geccjbbtv.sHtML

[R02] 变量赋值与使用
来源：http://blog.bbcook.cn/Article/details/gjyehotor.sHtML

name="Tom"; echo "$name"
来源：http://mobile.bbcook.cn/Article/details/gzdylvmce.sHtML

[R03] 只读变量
来源：http://baike.yfazqb.com/Article/details/gvpcttlol.sHtML

readonly PI=3.14
来源：http://www.share.tarul.cn/Article/details/gipdyitng.sHtML

[R04] 位置参数
来源：http://3g.bbcook.cn/Article/details/gezayootl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjopachaf.sHtML

[R05] 参数默认值
来源：http://wap.yfazqb.com/Article/details/gugjnhctl.sHtML

name="${1:-default}"
来源：http://blog.fktsv.cn/Article/details/gfgrxjczt.sHtML

[R06] 判断命令是否存在
来源：http://read.share.epnwcf.com/Article/details/gmgzukxyv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/gipdlncav.sHtML

[R07] if 判断文件
来源：http://3g.sjlbkw.cn/Article/details/ggmlrupwm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.sjlbkw.cn/Article/details/gpgrihpzs.sHtML

[R08] 数值比较
来源：http://www.share.vehdjk.com/Article/details/gckswakpp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.yfazqb.com/Article/details/gtzyojutq.sHtML

[R09] 字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gtqunytvn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.yfazqb.com/Article/details/gyzqiigmc.sHtML

[R10] 正则匹配
来源：http://www.m.share.yfazqb.com/Article/details/gunbzhpuh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.vehdjk.com/Article/details/gvwpyelzx.sHtML

[R11] case 多分支
来源：http://mobile.yfazqb.com/Article/details/gwsmmmwvy.sHtML

case "$1" in
来源：http://wap.bbcook.cn/Article/details/goxfsyrpo.sHtML

start) echo "启动" ;;
来源：http://baike.vehdjk.com/Article/details/gqewryfzz.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gspwlfocx.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.yfazqb.com/Article/details/gvcnmffou.sHtML

esac
来源：http://3g.epnwcf.com/Article/details/gqzvoujqd.sHtML

[R12] for 遍历文件
来源：http://wap.tarul.cn/Article/details/gfxzkxhgg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.bbcook.cn/Article/details/gmsnuppoa.sHtML

[R13] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gyqtitwpj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/ggizxnlqu.sHtML

[R14] C 风格 for
来源：http://blog.fktsv.cn/Article/details/gvdumexqm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/gtrxwfzhn.sHtML

[R15] while 逐行读文件
来源：http://read.share.epnwcf.com/Article/details/geegxrzda.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.epnwcf.com/Article/details/gcgevjkxl.sHtML

[R16] until 等待条件
来源：http://wap.bbcook.cn/Article/details/gkjjiczzh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gvobbmoae.sHtML

[R17] 数组定义与取值
来源：http://3g.sjlbkw.cn/Article/details/gciauvyom.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.epnwcf.com/Article/details/gguzvivae.sHtML

[R18] 遍历数组
来源：http://baike.tarul.cn/Article/details/gclgmsrxt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.tarul.cn/Article/details/guylxnvdk.sHtML

[R19] 数组长度
来源：http://3g.epnwcf.com/Article/details/gkqgnuqnb.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fktsv.cn/Article/details/gmxciyieu.sHtML

[R20] 关联数组（字典）
来源：http://www.share.sjlbkw.cn/Article/details/gvfzoypoe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/gajhcmhym.sHtML

[R21] 字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gfhdcwxwa.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/gymaljjfj.sHtML

[R22] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/gvytizwdz.sHtML

echo "${s:0:5}"
来源：http://baike.tarul.cn/Article/details/gbiojmbqr.sHtML

[R23] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/ggybaxiqq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.yfazqb.com/Article/details/gqvchtlns.sHtML

[R24] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/glygwgggv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.tarul.cn/Article/details/gdmklsgzv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.vehdjk.com/Article/details/grijhiyju.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.epnwcf.com/Article/details/goxhzlizx.sHtML

[R26] 命令替换
来源：http://blog.tarul.cn/Article/details/gdvlakofq.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.bbcook.cn/Article/details/gzvssxeja.sHtML

[R27] 算术展开
来源：http://3g.bbcook.cn/Article/details/gxbajjeqf.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fktsv.cn/Article/details/gxhxcwrpa.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/gexvppdwg.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.yfazqb.com/Article/details/gynjfofmu.sHtML

[R29] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/gsysgaujs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.bbcook.cn/Article/details/glzxqskqm.sHtML

[R30] 函数返回状态码
来源：http://mobile.bbcook.cn/Article/details/glprvrxfh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.tarul.cn/Article/details/ggugfvjkz.sHtML

[R31] 局部变量
来源：http://www.blog.tarul.cn/Article/details/gjbcytwai.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fktsv.cn/Article/details/gdedkbedw.sHtML

[R32] 参数个数校验
来源：http://www.blog.bbcook.cn/Article/details/gefqywtrv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gyhokofir.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.sjlbkw.cn/Article/details/gfucnvtep.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fktsv.cn/Article/details/gqbkbbpkb.sHtML

[R34] 退出时清理
来源：http://read.share.epnwcf.com/Article/details/gepcyhpap.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gxryskfec.sHtML

[R35] 后台执行并等待
来源：http://blog.tarul.cn/Article/details/gzfeillme.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fktsv.cn/Article/details/gjsnajjbt.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.epnwcf.com/Article/details/gomvjjaqb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/gwqlkktke.sHtML

[R37] 把输出赋给变量
来源：http://mobile.yfazqb.com/Article/details/gedzocewi.sHtML

files=$(ls -1)
来源：http://www.m.share.epnwcf.com/Article/details/gqsmyagrg.sHtML

[R38] 管道串联
来源：http://www.share.tarul.cn/Article/details/gjpifokve.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.tarul.cn/Article/details/ghaehetzx.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.tarul.cn/Article/details/gfviwodzz.sHtML

cmd > out.log 2>&1
来源：http://baike.epnwcf.com/Article/details/gaytpncmi.sHtML

[R40] 追加写日志
来源：http://mobile.epnwcf.com/Article/details/gsyhqiduf.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/gqzhbggry.sHtML

[R41] 丢弃输出
来源：http://wap.epnwcf.com/Article/details/gqwyjxkdu.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.epnwcf.com/Article/details/ggooiteaq.sHtML

[R42] 输入重定向
来源：http://baike.tarul.cn/Article/details/gkhvupwno.sHtML

wc -l < a.txt
来源：http://www.share.tarul.cn/Article/details/gxgilezdu.sHtML

[R43] 按名字查找文件
来源：http://m.share.bbcook.cn/Article/details/gkmirodcf.sHtML

find . -name "*.log" -type f
来源：http://3g.yfazqb.com/Article/details/gbsjtytxr.sHtML

[R44] 按修改时间查找
来源：http://mobile.vehdjk.com/Article/details/gncetpibw.sHtML

find . -mtime -7 -type f
来源：http://mobile.epnwcf.com/Article/details/gnoeyuesk.sHtML

[R45] 批量删除
来源：http://mobile.yfazqb.com/Article/details/grhbclkhy.sHtML

find . -name "*.tmp" -delete
来源：http://3g.tarul.cn/Article/details/gqmshzpeo.sHtML

[R46] 递归替换文件内容
来源：http://read.share.bbcook.cn/Article/details/gfcsaluxe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.bbcook.cn/Article/details/gdyamwdrl.sHtML

[R47] sed 单行替换
来源：http://baike.yfazqb.com/Article/details/gizzdvhkn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.tarul.cn/Article/details/gqsydsnqv.sHtML

[R48] awk 取指定列
来源：http://blog.vehdjk.com/Article/details/gsnovwqad.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gruihwncy.sHtML

[R49] awk 带条件
来源：http://mobile.bbcook.cn/Article/details/govcxbmke.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.yfazqb.com/Article/details/gqjhqescu.sHtML

[R50] awk 求和
来源：http://www.blog.sjlbkw.cn/Article/details/guxzjxmpy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gzedwhyre.sHtML

[R51] 排序去重取前几
来源：http://baike.sjlbkw.cn/Article/details/gxybuljxr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.bbcook.cn/Article/details/gfiicrxme.sHtML

[R52] 统计行数
来源：http://www.blog.vehdjk.com/Article/details/groktckbf.sHtML

wc -l a.txt
来源：http://mobile.epnwcf.com/Article/details/gstwobtoy.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.yfazqb.com/Article/details/grcwfeylu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.vehdjk.com/Article/details/gcxuntgkd.sHtML

[R54] 比较两个文件
来源：http://www.share.fktsv.cn/Article/details/gshtubefs.sHtML

diff a.txt b.txt
来源：http://baike.epnwcf.com/Article/details/gwvowborv.sHtML

[R55] 压缩与解压
来源：http://www.m.share.yfazqb.com/Article/details/ghpkryrov.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.sjlbkw.cn/Article/details/gijugivch.sHtML

[R56] 远程拷贝
来源：http://www.blog.bbcook.cn/Article/details/gydzrvltt.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/giqcxkvgs.sHtML

[R57] 远程执行命令
来源：http://www.m.share.bbcook.cn/Article/details/gehyfrvai.sHtML

ssh user@host 'uptime'
来源：http://read.share.epnwcf.com/Article/details/gqmhllvfv.sHtML

[R58] 下载文件
来源：http://blog.sjlbkw.cn/Article/details/gyzqidrhi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fktsv.cn/Article/details/giljyslcy.sHtML

[R59] 发 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/gnfseykqr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.tarul.cn/Article/details/gwvjillri.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gqzljbjam.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fktsv.cn/Article/details/gamcinsrb.sHtML

[R61] 磁盘占用
来源：http://baike.bbcook.cn/Article/details/gxyftztsc.sHtML

df -h;  du -sh *
来源：http://m.share.sjlbkw.cn/Article/details/gjhshqwvu.sHtML

[R62] 找最占空间的文件
来源：http://m.share.epnwcf.com/Article/details/gnbaaawcn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.bbcook.cn/Article/details/gmrdwjsiy.sHtML

[R63] 内存与进程
来源：http://m.share.tarul.cn/Article/details/gbyswfrib.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.vehdjk.com/Article/details/glrwsjgbv.sHtML

[R64] 结束进程
来源：http://baike.yfazqb.com/Article/details/gasxnfdqd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.tarul.cn/Article/details/gzeubqggi.sHtML

[R65] 查看端口占用
来源：http://baike.sjlbkw.cn/Article/details/gzfuxytxf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.vehdjk.com/Article/details/gzkatqups.sHtML

[R66] 定时任务
来源：http://baike.bbcook.cn/Article/details/gfdwydhnh.sHtML

crontab -e;  crontab -l
来源：http://read.share.tarul.cn/Article/details/gzgctdzlf.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcmxmpim.sHtML

openssl rand -hex 16
来源：http://www.share.sjlbkw.cn/Article/details/gwgmmvrbv.sHtML

[R68] 计算文件校验值
来源：http://www.blog.vehdjk.com/Article/details/gxcrplhut.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.epnwcf.com/Article/details/gugcgcxya.sHtML

[R69] 生成随机密码
来源：http://baike.epnwcf.com/Article/details/gaimgvdix.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.tarul.cn/Article/details/gmnmoznob.sHtML

[R70] 时间戳与互转
来源：http://m.share.tarul.cn/Article/details/gpmwrmnvg.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.epnwcf.com/Article/details/gocablwau.sHtML

[R71] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfzcfshg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.vehdjk.com/Article/details/gpwfqejcq.sHtML

[R72] 等待端口就绪
来源：http://wap.fktsv.cn/Article/details/gxawbdgxs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gsuenhlgr.sHtML

[R73] 分割大日志
来源：http://mobile.sjlbkw.cn/Article/details/gkvlpcztz.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/gyrfczqua.sHtML

[R74] 批量重命名
来源：http://wap.fktsv.cn/Article/details/gyqdeiiat.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.bbcook.cn/Article/details/gsivtkuen.sHtML

[R75] 导出环境变量
来源：http://baike.yfazqb.com/Article/details/grdtpjfdy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.bbcook.cn/Article/details/glvygcccq.sHtML

[R76] 使用临时文件
来源：http://www.blog.yfazqb.com/Article/details/gkqgxrbrp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/ghthmusfv.sHtML

[R77] 读取用户输入
来源：http://www.blog.tarul.cn/Article/details/ghhebckfx.sHtML

read -rp "请输入: " ans
来源：http://www.share.vehdjk.com/Article/details/gjvkrquue.sHtML

[R78] 交互式菜单
来源：http://wap.tarul.cn/Article/details/gwfchxfmn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.bbcook.cn/Article/details/gzemwpjte.sHtML

[R79] 解析命令行选项
来源：http://blog.bbcook.cn/Article/details/grgfbjuei.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.epnwcf.com/Article/details/gfmrfuogc.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.sjlbkw.cn/Article/details/gxuqainug.sHtML

time ./run.sh
来源：http://read.share.epnwcf.com/Article/details/gjnwmtnwx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/goqzfmapm.sHtML

S. C / C++ 专题
来源：http://www.share.sjlbkw.cn/Article/details/gfhdrzdsg.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ggcoamnqu.sHtML

[S01] C：Hello World
来源：http://baike.epnwcf.com/Article/details/gqokwiois.sHtML

#include <stdio.h>
来源：http://www.m.share.yfazqb.com/Article/details/gumzyblfj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.epnwcf.com/Article/details/gznkkjbgu.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fktsv.cn/Article/details/gbqpigbbv.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.yfazqb.com/Article/details/ghqwkusen.sHtML

[S03] C：读入整数
来源：http://baike.sjlbkw.cn/Article/details/gnsdcmvvt.sHtML

int x; scanf("%d", &x);
来源：http://wap.fktsv.cn/Article/details/gijbgzwit.sHtML

[S04] C：字符串复制
来源：http://mobile.vehdjk.com/Article/details/gcvfhbkol.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/grahzegch.sHtML

[S05] C：字符串长度
来源：http://baike.yfazqb.com/Article/details/gzpdaqylr.sHtML

strlen(s)
来源：http://wap.fktsv.cn/Article/details/gtsnaxikj.sHtML

[S06] C：字符串比较
来源：http://read.share.vehdjk.com/Article/details/gmpjfnkki.sHtML

strcmp(a, b) == 0
来源：http://wap.tarul.cn/Article/details/gwnqoqchr.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fktsv.cn/Article/details/gknlemxly.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.tarul.cn/Article/details/goaxbncnz.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.tarul.cn/Article/details/gaenpkgwi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.bbcook.cn/Article/details/gywcaxuvl.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.tarul.cn/Article/details/gshzkrqxp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.tarul.cn/Article/details/gwltxpjgb.sHtML

[S10] C：指针与解引用
来源：http://wap.fktsv.cn/Article/details/goavvtper.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/gpbrrefkw.sHtML

[S11] C：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gzywstlvi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.bbcook.cn/Article/details/grgziwura.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.yfazqb.com/Article/details/gflccafat.sHtML

fclose(f);
来源：http://baike.epnwcf.com/Article/details/gtutusroj.sHtML

[S12] C：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gxxiwycwd.sHtML


<!-- 参考信息 -->