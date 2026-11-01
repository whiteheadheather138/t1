代发 wailian999

[Q44] IN 子查询
来源：http://baike.vehdjk.com/Article/details/geakqwqvo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.bbcook.cn/Article/details/gvdfcldnd.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.vehdjk.com/Article/details/gunogrzbl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/gbfmktuch.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.sjlbkw.cn/Article/details/gvfxwbhjl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.yfazqb.com/Article/details/guhhkjfjh.sHtML

[Q47] 与平均值比较
来源：http://baike.bbcook.cn/Article/details/gammvonlh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.sjlbkw.cn/Article/details/glzvefsuu.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fktsv.cn/Article/details/gpwddlldi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.sjlbkw.cn/Article/details/gadgikjpa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.epnwcf.com/Article/details/gudjjggsq.sHtML

[Q49] 更新单行
来源：http://blog.yfazqb.com/Article/details/gynviumwn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/gzaivcync.sHtML

[Q50] 批量更新
来源：http://blog.fktsv.cn/Article/details/ghhitxpaw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.tarul.cn/Article/details/gkdwrnczt.sHtML

[Q51] 用子查询更新
来源：http://read.share.yfazqb.com/Article/details/grxgwjrcv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.epnwcf.com/Article/details/gnnrxgvvk.sHtML

[Q52] 删除指定行
来源：http://m.share.vehdjk.com/Article/details/guuxbzcyk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/ggiilfnde.sHtML

[Q53] 按条件删除
来源：http://mobile.epnwcf.com/Article/details/gvpvjwjpe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.yfazqb.com/Article/details/gmgqadano.sHtML

[Q54] 清空表
来源：http://www.blog.yfazqb.com/Article/details/grtniliav.sHtML

TRUNCATE TABLE logs;
来源：http://baike.yfazqb.com/Article/details/gclytlbsd.sHtML

[Q55] 排名（并列占位）
来源：http://blog.sjlbkw.cn/Article/details/gyyaoxgys.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gtzrkuvmo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.epnwcf.com/Article/details/gpreciwxt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.vehdjk.com/Article/details/gkfxjppuu.sHtML

[Q57] 行号
来源：http://blog.bbcook.cn/Article/details/gozzfasrl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.epnwcf.com/Article/details/gpvvvznid.sHtML

[Q58] 累计求和
来源：http://blog.tarul.cn/Article/details/glenubvlp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gzogdquqi.sHtML

[Q59] 分组内累计
来源：http://baike.bbcook.cn/Article/details/gmyiekbsh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gzzhateck.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.bbcook.cn/Article/details/grxwzuhrj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.vehdjk.com/Article/details/gkmncnrwn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gqavnungp.sHtML

[Q61] 移动平均
来源：http://mobile.vehdjk.com/Article/details/gngrlybnr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gsqyohqas.sHtML

[Q62] 分组占比
来源：http://blog.fktsv.cn/Article/details/gfqktuvqe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gfrmstjak.sHtML

[Q63] 开启事务
来源：http://m.share.tarul.cn/Article/details/gkugkyzeo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.sjlbkw.cn/Article/details/gjhzupgzr.sHtML

[Q64] 提交事务
来源：http://www.blog.tarul.cn/Article/details/guqpvcllg.sHtML

COMMIT;
来源：http://read.share.fktsv.cn/Article/details/gliqkrdnd.sHtML

[Q65] 回滚事务
来源：http://baike.epnwcf.com/Article/details/gwdaqcsud.sHtML

ROLLBACK;
来源：http://baike.vehdjk.com/Article/details/gouexbvft.sHtML

[Q66] 行锁查询
来源：http://blog.yfazqb.com/Article/details/gkfxewshk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fktsv.cn/Article/details/gbkrmvmzf.sHtML

[Q67] 设置隔离级别
来源：http://www.share.tarul.cn/Article/details/gmolppmbo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.epnwcf.com/Article/details/glkelqqih.sHtML

[Q68] 保存点
来源：http://blog.bbcook.cn/Article/details/gkzcwsdkl.sHtML

SAVEPOINT sp1;
来源：http://mobile.epnwcf.com/Article/details/gvwbtscpf.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fktsv.cn/Article/details/gmeotxeoh.sHtML

[Q69] 查看执行计划
来源：http://www.share.vehdjk.com/Article/details/gndxpbsit.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.epnwcf.com/Article/details/gvimbfkrq.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/gerfpiqwd.sHtML

ANALYZE TABLE users;
来源：http://read.share.epnwcf.com/Article/details/gptvfgtfe.sHtML

[Q71] 查看建表语句
来源：http://www.blog.yfazqb.com/Article/details/grdqjgxrn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.yfazqb.com/Article/details/gngjveckf.sHtML

[Q72] 查看索引
来源：http://www.share.tarul.cn/Article/details/guxkbytji.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gqxxiutpi.sHtML

[Q73] 查看表状态
来源：http://read.share.sjlbkw.cn/Article/details/gpflwvdsw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.vehdjk.com/Article/details/gdkwsabae.sHtML

[Q74] 强制使用索引
来源：http://wap.bbcook.cn/Article/details/gabfvjmqz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.vehdjk.com/Article/details/gtfynbeht.sHtML

[Q75] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/ghtxcqdbm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.tarul.cn/Article/details/genigvznb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.vehdjk.com/Article/details/gqredircc.sHtML

[Q76] 按天统计
来源：http://m.share.sjlbkw.cn/Article/details/gygcucryv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.sjlbkw.cn/Article/details/gblrxkelc.sHtML

[Q77] 时间加减
来源：http://mobile.tarul.cn/Article/details/geuujcxvu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.bbcook.cn/Article/details/gvvfyrdli.sHtML

[Q78] 当前时间
来源：http://blog.tarul.cn/Article/details/godgldxxq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.tarul.cn/Article/details/gajugtggw.sHtML

[Q79] 字符串拼接
来源：http://m.share.bbcook.cn/Article/details/gbuuabsad.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.vehdjk.com/Article/details/gpvkeeigh.sHtML

[Q80] 字符串截取
来源：http://wap.yfazqb.com/Article/details/gzhlvfwdx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gntixdwdr.sHtML

[Q81] 字符串替换
来源：http://baike.yfazqb.com/Article/details/gumlunjsq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.tarul.cn/Article/details/gfxgwxnmx.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.bbcook.cn/Article/details/gcxawaxzn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gfvyrmtwl.sHtML

[Q83] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gcukhpgbm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gilryyerz.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.bbcook.cn/Article/details/giwhkofhm.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gwkglqkjz.sHtML

[Q85] 数值取整
来源：http://read.share.sjlbkw.cn/Article/details/gbskttibf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.bbcook.cn/Article/details/gfiqwgong.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.bbcook.cn/Article/details/gycgdcist.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.bbcook.cn/Article/details/gtoneabls.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.yfazqb.com/Article/details/gtubbycez.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.bbcook.cn/Article/details/gldorjihu.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.epnwcf.com/Article/details/gtskqsiyv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.epnwcf.com/Article/details/ghllkapdc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fktsv.cn/Article/details/gjjyuklkl.sHtML

[Q89] 判断表是否存在
来源：http://blog.fktsv.cn/Article/details/gbeuviurn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.yfazqb.com/Article/details/gebshohbs.sHtML

[Q90] 生成序号列
来源：http://www.m.share.epnwcf.com/Article/details/gdxdjpdih.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.yfazqb.com/Article/details/gyeuxdukd.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grkcxkgdl.sHtML

R. Bash 专题
来源：http://3g.yfazqb.com/Article/details/gqqtwhcti.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gnfosxdur.sHtML

[R01] shebang 与严格模式
来源：http://read.share.yfazqb.com/Article/details/gskjnhhim.sHtML

#!/usr/bin/env bash
来源：http://3g.epnwcf.com/Article/details/gwhuarcnd.sHtML

set -euo pipefail
来源：http://www.share.tarul.cn/Article/details/gkuruvaod.sHtML

[R02] 变量赋值与使用
来源：http://baike.vehdjk.com/Article/details/gchkaygrx.sHtML

name="Tom"; echo "$name"
来源：http://wap.yfazqb.com/Article/details/gbpizpmtu.sHtML

[R03] 只读变量
来源：http://wap.yfazqb.com/Article/details/gxksjynef.sHtML

readonly PI=3.14
来源：http://wap.epnwcf.com/Article/details/gvqauvurk.sHtML

[R04] 位置参数
来源：http://m.share.epnwcf.com/Article/details/gkbdteeee.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fktsv.cn/Article/details/gnjyzpyyb.sHtML

[R05] 参数默认值
来源：http://3g.sjlbkw.cn/Article/details/gxuvkurzc.sHtML

name="${1:-default}"
来源：http://blog.sjlbkw.cn/Article/details/gtzgridgd.sHtML

[R06] 判断命令是否存在
来源：http://blog.epnwcf.com/Article/details/gehffzsgr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gvjfwlibb.sHtML

[R07] if 判断文件
来源：http://3g.yfazqb.com/Article/details/gdvnhmpkx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.vehdjk.com/Article/details/gnnhbrzst.sHtML

[R08] 数值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gelvpqtmh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.bbcook.cn/Article/details/giiehjfhy.sHtML

[R09] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gexghtnfp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/gxpamdiax.sHtML

[R10] 正则匹配
来源：http://wap.tarul.cn/Article/details/gjbrdxsxs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.tarul.cn/Article/details/gojpqspvq.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/gajslvbyo.sHtML

case "$1" in
来源：http://m.share.epnwcf.com/Article/details/gmoryqsbm.sHtML

start) echo "启动" ;;
来源：http://m.share.vehdjk.com/Article/details/glyatlqtz.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.tarul.cn/Article/details/gnqxpsyuf.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fktsv.cn/Article/details/gkuahzabi.sHtML

esac
来源：http://www.share.tarul.cn/Article/details/ghgjwncfi.sHtML

[R12] for 遍历文件
来源：http://mobile.bbcook.cn/Article/details/ggjmzinjo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fktsv.cn/Article/details/gwbmnqmbu.sHtML

[R13] for 计数循环
来源：http://m.share.tarul.cn/Article/details/gsavlmiag.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/gnxrsinyi.sHtML

[R14] C 风格 for
来源：http://mobile.yfazqb.com/Article/details/glddnlnpy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/gkbyjkrpi.sHtML

[R15] while 逐行读文件
来源：http://read.share.bbcook.cn/Article/details/ggsfmnxwm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.epnwcf.com/Article/details/gbvhffbnl.sHtML

[R16] until 等待条件
来源：http://wap.fktsv.cn/Article/details/gzlfkwyhn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/gnbymcvgl.sHtML

[R17] 数组定义与取值
来源：http://m.share.fktsv.cn/Article/details/gflbzhfri.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.vehdjk.com/Article/details/grcqrjrsm.sHtML

[R18] 遍历数组
来源：http://baike.epnwcf.com/Article/details/gtnlqvlqm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.yfazqb.com/Article/details/gzeqaotow.sHtML

[R19] 数组长度
来源：http://wap.sjlbkw.cn/Article/details/ggvjowcdp.sHtML

echo "${#arr[@]}"
来源：http://3g.epnwcf.com/Article/details/gepgvuigw.sHtML

[R20] 关联数组（字典）
来源：http://blog.epnwcf.com/Article/details/gmwvjulaq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.bbcook.cn/Article/details/glckwdhov.sHtML

[R21] 字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gahqthfve.sHtML

echo "${#s}"
来源：http://www.blog.epnwcf.com/Article/details/gwtonogau.sHtML

[R22] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/ghhstpnft.sHtML

echo "${s:0:5}"
来源：http://3g.yfazqb.com/Article/details/gefbsxoef.sHtML

[R23] 字符串替换
来源：http://baike.epnwcf.com/Article/details/gsfergotz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.sjlbkw.cn/Article/details/gnvryqegh.sHtML

[R24] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gxjxuflex.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.bbcook.cn/Article/details/germwknof.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.vehdjk.com/Article/details/gjcxagyzg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.tarul.cn/Article/details/gxnkamlit.sHtML

[R26] 命令替换
来源：http://mobile.tarul.cn/Article/details/gnawhyzcq.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.epnwcf.com/Article/details/goluwprao.sHtML

[R27] 算术展开
来源：http://wap.tarul.cn/Article/details/gywxokphj.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.tarul.cn/Article/details/gsyabbgbo.sHtML

[R28] 浮点运算
来源：http://baike.fktsv.cn/Article/details/gwiuitqzi.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.yfazqb.com/Article/details/gtdhvfwtm.sHtML

[R29] 定义函数
来源：http://www.m.share.yfazqb.com/Article/details/gcxzygmws.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.sjlbkw.cn/Article/details/givimvyrb.sHtML

[R30] 函数返回状态码
来源：http://m.share.epnwcf.com/Article/details/glepwhnha.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.yfazqb.com/Article/details/gabnhfdie.sHtML

[R31] 局部变量
来源：http://m.share.vehdjk.com/Article/details/gkaphdtqh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.vehdjk.com/Article/details/gxgyutvcy.sHtML

[R32] 参数个数校验
来源：http://read.share.epnwcf.com/Article/details/gcvrcxjev.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/gfgiuzxcf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.tarul.cn/Article/details/goobkzuxv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.epnwcf.com/Article/details/gvzhtucvg.sHtML

[R34] 退出时清理
来源：http://www.m.share.sjlbkw.cn/Article/details/gwitysfzc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gawfyosjp.sHtML

[R35] 后台执行并等待
来源：http://www.share.fktsv.cn/Article/details/gmuwspffr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.tarul.cn/Article/details/gbffsikkb.sHtML

[R36] 并发执行多个任务
来源：http://mobile.bbcook.cn/Article/details/gdymxrgok.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fktsv.cn/Article/details/gutczaeon.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/gzjgnuctm.sHtML

files=$(ls -1)
来源：http://m.share.sjlbkw.cn/Article/details/gfjvqhttw.sHtML

[R38] 管道串联
来源：http://www.m.share.yfazqb.com/Article/details/gbcopsbvw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.yfazqb.com/Article/details/gzprhbwsz.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.yfazqb.com/Article/details/gzwyigjvo.sHtML

cmd > out.log 2>&1
来源：http://www.blog.bbcook.cn/Article/details/gbiizdags.sHtML

[R40] 追加写日志
来源：http://blog.vehdjk.com/Article/details/gqjjwjzff.sHtML

echo "log" >> out.log
来源：http://wap.sjlbkw.cn/Article/details/gchtpockw.sHtML

[R41] 丢弃输出
来源：http://3g.fktsv.cn/Article/details/gllmpzkmo.sHtML

cmd >/dev/null 2>&1
来源：http://wap.epnwcf.com/Article/details/gyeszwowa.sHtML

[R42] 输入重定向
来源：http://wap.sjlbkw.cn/Article/details/gjzllvvyf.sHtML

wc -l < a.txt
来源：http://mobile.epnwcf.com/Article/details/gkhszhqaq.sHtML

[R43] 按名字查找文件
来源：http://blog.tarul.cn/Article/details/gfqutmzqc.sHtML

find . -name "*.log" -type f
来源：http://wap.fktsv.cn/Article/details/gqhypqfqs.sHtML

[R44] 按修改时间查找
来源：http://m.share.tarul.cn/Article/details/guhwilrnn.sHtML

find . -mtime -7 -type f
来源：http://www.share.vehdjk.com/Article/details/gqecighqq.sHtML

[R45] 批量删除
来源：http://mobile.bbcook.cn/Article/details/gosjfcysn.sHtML

find . -name "*.tmp" -delete
来源：http://3g.sjlbkw.cn/Article/details/gpfgylwdy.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fktsv.cn/Article/details/gwszpvals.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.bbcook.cn/Article/details/gumuooyrl.sHtML

[R47] sed 单行替换
来源：http://wap.sjlbkw.cn/Article/details/gyyqrmabx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/ggbrzmekl.sHtML

[R48] awk 取指定列
来源：http://www.blog.epnwcf.com/Article/details/gpkrwxzgo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/ghwqzfjho.sHtML

[R49] awk 带条件
来源：http://www.m.share.vehdjk.com/Article/details/gczfuomsx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.tarul.cn/Article/details/gtrsiuoua.sHtML

[R50] awk 求和
来源：http://mobile.fktsv.cn/Article/details/gjhlopddh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gxghyyage.sHtML

[R51] 排序去重取前几
来源：http://www.share.bbcook.cn/Article/details/glzfmtbsn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.epnwcf.com/Article/details/gyshxrysv.sHtML

[R52] 统计行数
来源：http://www.m.share.epnwcf.com/Article/details/gricqimpd.sHtML

wc -l a.txt
来源：http://read.share.tarul.cn/Article/details/gcqlakhzi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.vehdjk.com/Article/details/gifaajwzc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fktsv.cn/Article/details/gtynlcfbv.sHtML

[R54] 比较两个文件
来源：http://www.blog.tarul.cn/Article/details/gdvhblmcm.sHtML

diff a.txt b.txt
来源：http://3g.sjlbkw.cn/Article/details/gqhudywik.sHtML

[R55] 压缩与解压
来源：http://m.share.tarul.cn/Article/details/gdnpdpoyf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/gbbwlmmhu.sHtML

[R56] 远程拷贝
来源：http://mobile.epnwcf.com/Article/details/ggjfdzpyx.sHtML

scp file user@host:/path/
来源：http://m.share.tarul.cn/Article/details/gyqquguhu.sHtML

[R57] 远程执行命令
来源：http://mobile.bbcook.cn/Article/details/gwnupxnqn.sHtML

ssh user@host 'uptime'
来源：http://read.share.epnwcf.com/Article/details/ganhvhjeo.sHtML

[R58] 下载文件
来源：http://www.blog.vehdjk.com/Article/details/gkptxwkoo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.vehdjk.com/Article/details/gqzebcgwd.sHtML

[R59] 发 POST JSON
来源：http://www.blog.epnwcf.com/Article/details/gwonvuftk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fktsv.cn/Article/details/gtcwyqubg.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/gealxkhen.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.tarul.cn/Article/details/gvqbqvxnn.sHtML

[R61] 磁盘占用
来源：http://mobile.yfazqb.com/Article/details/goflfvduz.sHtML

df -h;  du -sh *
来源：http://m.share.sjlbkw.cn/Article/details/gmqjbkybv.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.epnwcf.com/Article/details/gaocbqzpx.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.epnwcf.com/Article/details/ggxiwdxzk.sHtML

[R63] 内存与进程
来源：http://3g.tarul.cn/Article/details/gtjumpszm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fktsv.cn/Article/details/ggfsowngg.sHtML

[R64] 结束进程
来源：http://www.m.share.tarul.cn/Article/details/gdospxtpm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.bbcook.cn/Article/details/gaiiyljxu.sHtML

[R65] 查看端口占用
来源：http://3g.tarul.cn/Article/details/gkffnzrtg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.yfazqb.com/Article/details/gpognpbol.sHtML

[R66] 定时任务
来源：http://mobile.fktsv.cn/Article/details/guzchckrv.sHtML

crontab -e;  crontab -l
来源：http://baike.tarul.cn/Article/details/gqpnvevrm.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.sjlbkw.cn/Article/details/gxvcjykhb.sHtML

openssl rand -hex 16
来源：http://m.share.vehdjk.com/Article/details/gzzxqudph.sHtML

[R68] 计算文件校验值
来源：http://3g.vehdjk.com/Article/details/geochflvk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.tarul.cn/Article/details/ggvmtkmbx.sHtML

[R69] 生成随机密码
来源：http://baike.epnwcf.com/Article/details/gejshgjdz.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.tarul.cn/Article/details/gwejehvcu.sHtML

[R70] 时间戳与互转
来源：http://baike.vehdjk.com/Article/details/gyttilrid.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fktsv.cn/Article/details/ghpymvaur.sHtML

[R71] 日期格式化
来源：http://mobile.epnwcf.com/Article/details/glzsbpmdd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.sjlbkw.cn/Article/details/gnckkfhdc.sHtML

[R72] 等待端口就绪
来源：http://www.blog.tarul.cn/Article/details/gjqbdqksh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gqzpgqkzy.sHtML

[R73] 分割大日志
来源：http://wap.bbcook.cn/Article/details/gjdhgwzbd.sHtML

split -l 1000 big.log part_
来源：http://www.share.tarul.cn/Article/details/gavbsbbkc.sHtML

[R74] 批量重命名
来源：http://3g.vehdjk.com/Article/details/griuaczmk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.tarul.cn/Article/details/gevnwcmxs.sHtML

[R75] 导出环境变量
来源：http://wap.sjlbkw.cn/Article/details/gtokqdrer.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.tarul.cn/Article/details/gzzubrjgo.sHtML

[R76] 使用临时文件
来源：http://baike.bbcook.cn/Article/details/gldhubldg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gecehwkil.sHtML

[R77] 读取用户输入
来源：http://mobile.tarul.cn/Article/details/gqbcgacvv.sHtML

read -rp "请输入: " ans
来源：http://mobile.tarul.cn/Article/details/gqyphlsse.sHtML

[R78] 交互式菜单
来源：http://mobile.vehdjk.com/Article/details/gdelaxroe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/gojgijeai.sHtML

[R79] 解析命令行选项
来源：http://read.share.fktsv.cn/Article/details/gfgewcqhf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.tarul.cn/Article/details/gtgeqlpyz.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.vehdjk.com/Article/details/gzsyuzunn.sHtML

time ./run.sh
来源：http://wap.epnwcf.com/Article/details/grwryefmf.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gddxkoaim.sHtML

S. C / C++ 专题
来源：http://read.share.yfazqb.com/Article/details/gajoyfnmp.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gamszuyau.sHtML

[S01] C：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gtpbtfvkx.sHtML

#include <stdio.h>
来源：http://read.share.tarul.cn/Article/details/gmacpbmkk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.tarul.cn/Article/details/gizugeuku.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/gfzlqetrl.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.vehdjk.com/Article/details/gtuiejalf.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gesjiykaa.sHtML

int x; scanf("%d", &x);
来源：http://3g.yfazqb.com/Article/details/gxrjypbfx.sHtML

[S04] C：字符串复制
来源：http://www.share.epnwcf.com/Article/details/gkjusxlxb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.vehdjk.com/Article/details/gdvxzyria.sHtML

[S05] C：字符串长度
来源：http://baike.bbcook.cn/Article/details/gealmgrii.sHtML

strlen(s)
来源：http://blog.fktsv.cn/Article/details/gjbdibsvk.sHtML

[S06] C：字符串比较
来源：http://wap.vehdjk.com/Article/details/gdjitgpxc.sHtML

strcmp(a, b) == 0
来源：http://mobile.tarul.cn/Article/details/ggtynfizm.sHtML

[S07] C：数组遍历求和
来源：http://read.share.yfazqb.com/Article/details/gnqjupuve.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fktsv.cn/Article/details/gxtlkppom.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.yfazqb.com/Article/details/gkeuxhakh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fktsv.cn/Article/details/gwpaafewj.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fktsv.cn/Article/details/gblueaowq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.sjlbkw.cn/Article/details/gmjhpjnsl.sHtML

[S10] C：指针与解引用
来源：http://3g.tarul.cn/Article/details/gbsewrzwm.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.vehdjk.com/Article/details/gjnuxpsfy.sHtML

[S11] C：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/grpzvydrx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.epnwcf.com/Article/details/gjdplomdr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fktsv.cn/Article/details/glrvwxopz.sHtML

fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/glsltxfsy.sHtML

[S12] C：写文件
来源：http://mobile.bbcook.cn/Article/details/gbkbetbsy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.vehdjk.com/Article/details/gfelbyytm.sHtML

[S13] C：宏定义
来源：http://mobile.vehdjk.com/Article/details/guydewbst.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/gxotznltf.sHtML

[S14] C：枚举
来源：http://wap.vehdjk.com/Article/details/gpwdnphwf.sHtML


<!-- 参考信息 -->