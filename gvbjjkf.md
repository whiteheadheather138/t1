代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.bbcook.cn/Article/details/gxdgtmnwh.sHtML

[Q54] 清空表
来源：http://www.m.share.epnwcf.com/Article/details/gfwfklfbo.sHtML

TRUNCATE TABLE logs;
来源：http://baike.yfazqb.com/Article/details/gbipaxuyj.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.yfazqb.com/Article/details/gitcwxqsv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gbcmnwgsn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkqxvkzc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.bbcook.cn/Article/details/ghejqklab.sHtML

[Q57] 行号
来源：http://wap.yfazqb.com/Article/details/gbvgkxymw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.yfazqb.com/Article/details/gwqvkggwo.sHtML

[Q58] 累计求和
来源：http://mobile.fktsv.cn/Article/details/gihskdllp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.tarul.cn/Article/details/geacybwra.sHtML

[Q59] 分组内累计
来源：http://mobile.epnwcf.com/Article/details/ghtlsuhxq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gsraagieb.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.sjlbkw.cn/Article/details/gylqqvztv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.tarul.cn/Article/details/gwzksqnyi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gcezoubhx.sHtML

[Q61] 移动平均
来源：http://read.share.epnwcf.com/Article/details/gvwcrfdvv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gmpjzkrsk.sHtML

[Q62] 分组占比
来源：http://baike.tarul.cn/Article/details/gyuoqxyzp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gpzpgrutk.sHtML

[Q63] 开启事务
来源：http://read.share.fktsv.cn/Article/details/gogadwtkm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fktsv.cn/Article/details/glabrwwun.sHtML

[Q64] 提交事务
来源：http://m.share.sjlbkw.cn/Article/details/gmtphbcyo.sHtML

COMMIT;
来源：http://www.share.sjlbkw.cn/Article/details/gcrejzfbx.sHtML

[Q65] 回滚事务
来源：http://m.share.sjlbkw.cn/Article/details/gklfvwlos.sHtML

ROLLBACK;
来源：http://read.share.epnwcf.com/Article/details/gnwuxlvcf.sHtML

[Q66] 行锁查询
来源：http://m.share.fktsv.cn/Article/details/gwoakhzsc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.yfazqb.com/Article/details/gxfkdpwjk.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.bbcook.cn/Article/details/gwtawklrc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fktsv.cn/Article/details/gojuqqrwy.sHtML

[Q68] 保存点
来源：http://wap.bbcook.cn/Article/details/giwxeystd.sHtML

SAVEPOINT sp1;
来源：http://read.share.sjlbkw.cn/Article/details/gwtazmmid.sHtML

ROLLBACK TO sp1;
来源：http://wap.sjlbkw.cn/Article/details/gikksusun.sHtML

[Q69] 查看执行计划
来源：http://www.blog.vehdjk.com/Article/details/gyjoryljb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.tarul.cn/Article/details/gvpekhitx.sHtML

[Q70] 更新统计信息
来源：http://blog.tarul.cn/Article/details/gaxnvjiyj.sHtML

ANALYZE TABLE users;
来源：http://baike.fktsv.cn/Article/details/gptzqkilm.sHtML

[Q71] 查看建表语句
来源：http://read.share.vehdjk.com/Article/details/gtcshaprv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.tarul.cn/Article/details/gjissuobg.sHtML

[Q72] 查看索引
来源：http://www.blog.epnwcf.com/Article/details/gnfcukalc.sHtML

SHOW INDEX FROM users;
来源：http://blog.yfazqb.com/Article/details/gxobgforw.sHtML

[Q73] 查看表状态
来源：http://www.blog.bbcook.cn/Article/details/ghzjvvlvh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.yfazqb.com/Article/details/gsgyvucvr.sHtML

[Q74] 强制使用索引
来源：http://m.share.vehdjk.com/Article/details/gjquleabr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.yfazqb.com/Article/details/gvxuyziij.sHtML

[Q75] 日期格式化
来源：http://wap.vehdjk.com/Article/details/gsdmwjzhh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.vehdjk.com/Article/details/gevczijsr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.epnwcf.com/Article/details/gjcrzzntl.sHtML

[Q76] 按天统计
来源：http://www.share.sjlbkw.cn/Article/details/guxwnhhky.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.tarul.cn/Article/details/gewlreiyt.sHtML

[Q77] 时间加减
来源：http://www.m.share.epnwcf.com/Article/details/gpxyrymnp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.epnwcf.com/Article/details/gezgitpxk.sHtML

[Q78] 当前时间
来源：http://3g.fktsv.cn/Article/details/gfwhwbwwq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.tarul.cn/Article/details/gijsmypew.sHtML

[Q79] 字符串拼接
来源：http://blog.yfazqb.com/Article/details/gavaztcaz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.yfazqb.com/Article/details/gsupfpfni.sHtML

[Q80] 字符串截取
来源：http://www.share.yfazqb.com/Article/details/gcgpspiro.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.vehdjk.com/Article/details/gctqxqiwi.sHtML

[Q81] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gnwahippc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.yfazqb.com/Article/details/gcfrututz.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fktsv.cn/Article/details/grdwsgxmp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gyauoyliz.sHtML

[Q83] 大小写转换
来源：http://baike.fktsv.cn/Article/details/gpdvghwjf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gpyzhtxow.sHtML

[Q84] 去除首尾空格
来源：http://www.share.sjlbkw.cn/Article/details/guilbopcj.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gubvsxapr.sHtML

[Q85] 数值取整
来源：http://baike.sjlbkw.cn/Article/details/gnpvaxcys.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fktsv.cn/Article/details/gupepoflf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.vehdjk.com/Article/details/gsljwvrvh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.yfazqb.com/Article/details/gqlevxyks.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.tarul.cn/Article/details/gxbnvfirj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.epnwcf.com/Article/details/gidzxyfxi.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.epnwcf.com/Article/details/gjdwqylxp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.epnwcf.com/Article/details/gwgfvatoo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.yfazqb.com/Article/details/ggzfbnsqk.sHtML

[Q89] 判断表是否存在
来源：http://m.share.tarul.cn/Article/details/gknibxogg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.sjlbkw.cn/Article/details/ghvjumbpu.sHtML

[Q90] 生成序号列
来源：http://www.share.yfazqb.com/Article/details/gcwwmfbmi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/gbybqioxa.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glxucoygy.sHtML

R. Bash 专题
来源：http://read.share.tarul.cn/Article/details/gdsfcsmsz.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/galmsuokx.sHtML

[R01] shebang 与严格模式
来源：http://www.share.tarul.cn/Article/details/gvdpmmbfb.sHtML

#!/usr/bin/env bash
来源：http://blog.sjlbkw.cn/Article/details/gyezyncex.sHtML

set -euo pipefail
来源：http://3g.fktsv.cn/Article/details/gjkmajywf.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fktsv.cn/Article/details/gcejhlhcr.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.epnwcf.com/Article/details/gdircjndu.sHtML

[R03] 只读变量
来源：http://3g.vehdjk.com/Article/details/gztjcgwqb.sHtML

readonly PI=3.14
来源：http://wap.epnwcf.com/Article/details/ggysdcxqi.sHtML

[R04] 位置参数
来源：http://read.share.fktsv.cn/Article/details/gvsguevwf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/galapfxtv.sHtML

[R05] 参数默认值
来源：http://3g.vehdjk.com/Article/details/gammfehtn.sHtML

name="${1:-default}"
来源：http://3g.epnwcf.com/Article/details/gfkmtmohp.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gvkqjihpt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/gvisrhejh.sHtML

[R07] if 判断文件
来源：http://www.m.share.vehdjk.com/Article/details/gyerrxmlf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.tarul.cn/Article/details/ggmicudba.sHtML

[R08] 数值比较
来源：http://3g.sjlbkw.cn/Article/details/gkdksfcig.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.tarul.cn/Article/details/gnjykiskh.sHtML

[R09] 字符串比较
来源：http://www.m.share.tarul.cn/Article/details/gqtsozubz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.bbcook.cn/Article/details/gbpetncit.sHtML

[R10] 正则匹配
来源：http://read.share.epnwcf.com/Article/details/ghffiaqzf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.bbcook.cn/Article/details/gjkdgwysv.sHtML

[R11] case 多分支
来源：http://www.m.share.epnwcf.com/Article/details/gpeegsmbc.sHtML

case "$1" in
来源：http://www.blog.fktsv.cn/Article/details/gdlqtqibd.sHtML

start) echo "启动" ;;
来源：http://mobile.fktsv.cn/Article/details/gduwlmtdv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.epnwcf.com/Article/details/guqkyoeld.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.tarul.cn/Article/details/gajqmqzfz.sHtML

esac
来源：http://wap.tarul.cn/Article/details/goyrghvgr.sHtML

[R12] for 遍历文件
来源：http://read.share.vehdjk.com/Article/details/gdsitcqfw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fktsv.cn/Article/details/geotfgbuo.sHtML

[R13] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/gjkhjebvu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/gfdfeezoe.sHtML

[R14] C 风格 for
来源：http://3g.tarul.cn/Article/details/gmxpdrnrt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/gzmirbyxw.sHtML

[R15] while 逐行读文件
来源：http://blog.fktsv.cn/Article/details/goafmmkcf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.bbcook.cn/Article/details/gvecmmmay.sHtML

[R16] until 等待条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gddqrwpop.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/gffmltenm.sHtML

[R17] 数组定义与取值
来源：http://www.share.bbcook.cn/Article/details/gxfcbgojf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.sjlbkw.cn/Article/details/ghnzphgdo.sHtML

[R18] 遍历数组
来源：http://www.blog.fktsv.cn/Article/details/gfvzolwyb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fktsv.cn/Article/details/gwygtsgls.sHtML

[R19] 数组长度
来源：http://wap.tarul.cn/Article/details/gqukpdgio.sHtML

echo "${#arr[@]}"
来源：http://baike.yfazqb.com/Article/details/gkthnheyr.sHtML

[R20] 关联数组（字典）
来源：http://wap.yfazqb.com/Article/details/grdkdhanv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fktsv.cn/Article/details/geyipxfyr.sHtML

[R21] 字符串长度
来源：http://wap.yfazqb.com/Article/details/gwrukjtyz.sHtML

echo "${#s}"
来源：http://3g.tarul.cn/Article/details/gliflizcd.sHtML

[R22] 截取子串
来源：http://3g.yfazqb.com/Article/details/gyobwqlqw.sHtML

echo "${s:0:5}"
来源：http://wap.epnwcf.com/Article/details/gjoxnztvv.sHtML

[R23] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/geigjkkmd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.epnwcf.com/Article/details/gsdaltnqv.sHtML

[R24] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gzmhhexuv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.bbcook.cn/Article/details/gsktlcwzm.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.epnwcf.com/Article/details/grdqxbmzw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.yfazqb.com/Article/details/giwvjxpfu.sHtML

[R26] 命令替换
来源：http://mobile.bbcook.cn/Article/details/gelkonqfv.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.sjlbkw.cn/Article/details/gmmwxiwkt.sHtML

[R27] 算术展开
来源：http://mobile.fktsv.cn/Article/details/guxjbhqbk.sHtML

echo $((1 + 2 * 3))
来源：http://wap.tarul.cn/Article/details/gxqwjiiaj.sHtML

[R28] 浮点运算
来源：http://www.share.yfazqb.com/Article/details/gzyhmkhzp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.bbcook.cn/Article/details/gopoapxmq.sHtML

[R29] 定义函数
来源：http://3g.bbcook.cn/Article/details/gmwivnvmi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.tarul.cn/Article/details/gahhrimle.sHtML

[R30] 函数返回状态码
来源：http://blog.fktsv.cn/Article/details/geyqwcqhf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fktsv.cn/Article/details/gurqkrolp.sHtML

[R31] 局部变量
来源：http://read.share.yfazqb.com/Article/details/gpozsuldq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.sjlbkw.cn/Article/details/ghkkoyntt.sHtML

[R32] 参数个数校验
来源：http://m.share.vehdjk.com/Article/details/gwobqodrx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/gmeoyjyau.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.bbcook.cn/Article/details/gamifdpra.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.tarul.cn/Article/details/getcsogsi.sHtML

[R34] 退出时清理
来源：http://blog.fktsv.cn/Article/details/gbgqiievz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fktsv.cn/Article/details/gcjjuezvy.sHtML

[R35] 后台执行并等待
来源：http://read.share.epnwcf.com/Article/details/gntojhqaf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.bbcook.cn/Article/details/gftzxekzs.sHtML

[R36] 并发执行多个任务
来源：http://blog.bbcook.cn/Article/details/gzcqothbl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fktsv.cn/Article/details/gukdmqcsa.sHtML

[R37] 把输出赋给变量
来源：http://baike.yfazqb.com/Article/details/gfdyjcrsl.sHtML

files=$(ls -1)
来源：http://m.share.epnwcf.com/Article/details/gcegnuqox.sHtML

[R38] 管道串联
来源：http://3g.yfazqb.com/Article/details/gltdndmuz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fktsv.cn/Article/details/gyibjcjhp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fktsv.cn/Article/details/gkjgiardu.sHtML

cmd > out.log 2>&1
来源：http://read.share.bbcook.cn/Article/details/gppekarnp.sHtML

[R40] 追加写日志
来源：http://www.m.share.epnwcf.com/Article/details/gyqfcmacp.sHtML

echo "log" >> out.log
来源：http://wap.sjlbkw.cn/Article/details/grrjnyeqn.sHtML

[R41] 丢弃输出
来源：http://www.blog.epnwcf.com/Article/details/gqrdimehd.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/gkvekzwxa.sHtML

[R42] 输入重定向
来源：http://blog.tarul.cn/Article/details/gkfaziobk.sHtML

wc -l < a.txt
来源：http://blog.epnwcf.com/Article/details/gwaqnzdkk.sHtML

[R43] 按名字查找文件
来源：http://m.share.bbcook.cn/Article/details/gjqirzjey.sHtML

find . -name "*.log" -type f
来源：http://mobile.vehdjk.com/Article/details/gkpapozyj.sHtML

[R44] 按修改时间查找
来源：http://wap.yfazqb.com/Article/details/gdmgaqgxi.sHtML

find . -mtime -7 -type f
来源：http://www.share.sjlbkw.cn/Article/details/gdegdyhds.sHtML

[R45] 批量删除
来源：http://mobile.vehdjk.com/Article/details/gdmvghlnn.sHtML

find . -name "*.tmp" -delete
来源：http://wap.tarul.cn/Article/details/gyyhifnnc.sHtML

[R46] 递归替换文件内容
来源：http://baike.vehdjk.com/Article/details/gvtufxnkw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.yfazqb.com/Article/details/gsxxbmsbc.sHtML

[R47] sed 单行替换
来源：http://www.share.fktsv.cn/Article/details/gjzenfzlb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gmyhzapan.sHtML

[R48] awk 取指定列
来源：http://www.share.yfazqb.com/Article/details/gpqdbyuuj.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.vehdjk.com/Article/details/gtavnqvap.sHtML

[R49] awk 带条件
来源：http://www.share.tarul.cn/Article/details/gsjpuqmrf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.epnwcf.com/Article/details/gtwcnjfeo.sHtML

[R50] awk 求和
来源：http://www.m.share.yfazqb.com/Article/details/gpyxvwutv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.tarul.cn/Article/details/gcolhuwlm.sHtML

[R51] 排序去重取前几
来源：http://3g.epnwcf.com/Article/details/gmorjchrn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.tarul.cn/Article/details/gmqfrbtke.sHtML

[R52] 统计行数
来源：http://3g.epnwcf.com/Article/details/gkxyzfiev.sHtML

wc -l a.txt
来源：http://www.blog.yfazqb.com/Article/details/gepjznfls.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.epnwcf.com/Article/details/gnxlaulsj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.vehdjk.com/Article/details/gahntrvnr.sHtML

[R54] 比较两个文件
来源：http://3g.sjlbkw.cn/Article/details/gnxvhtjni.sHtML

diff a.txt b.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqfbqkgm.sHtML

[R55] 压缩与解压
来源：http://read.share.fktsv.cn/Article/details/gwtwiuiov.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.bbcook.cn/Article/details/grajmgzyn.sHtML

[R56] 远程拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gwbedesxh.sHtML

scp file user@host:/path/
来源：http://www.blog.sjlbkw.cn/Article/details/gwinkufmt.sHtML

[R57] 远程执行命令
来源：http://www.blog.yfazqb.com/Article/details/gsimsmjno.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fktsv.cn/Article/details/gzimvekmd.sHtML

[R58] 下载文件
来源：http://read.share.vehdjk.com/Article/details/gaddzntim.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.epnwcf.com/Article/details/ghwixzadh.sHtML

[R59] 发 POST JSON
来源：http://www.share.yfazqb.com/Article/details/gnsfhuvjp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.sjlbkw.cn/Article/details/gwpqxmkfu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gptwgpyeq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.bbcook.cn/Article/details/ghuzozyrc.sHtML

[R61] 磁盘占用
来源：http://mobile.sjlbkw.cn/Article/details/gjcewrhoq.sHtML

df -h;  du -sh *
来源：http://mobile.tarul.cn/Article/details/gdvuqacsg.sHtML

[R62] 找最占空间的文件
来源：http://read.share.vehdjk.com/Article/details/gdfzwgtgp.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fktsv.cn/Article/details/grvwpucxw.sHtML

[R63] 内存与进程
来源：http://read.share.sjlbkw.cn/Article/details/gwckzgzhh.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.sjlbkw.cn/Article/details/gydtbqmhj.sHtML

[R64] 结束进程
来源：http://baike.fktsv.cn/Article/details/gnwknodpm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fktsv.cn/Article/details/gpvjvfhnm.sHtML

[R65] 查看端口占用
来源：http://wap.bbcook.cn/Article/details/gyfsmifxh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.bbcook.cn/Article/details/gmatfykir.sHtML

[R66] 定时任务
来源：http://read.share.vehdjk.com/Article/details/gxijcgcee.sHtML

crontab -e;  crontab -l
来源：http://www.blog.yfazqb.com/Article/details/gseaweyge.sHtML

[R67] 生成随机十六进制串
来源：http://3g.tarul.cn/Article/details/gnzyptdnh.sHtML

openssl rand -hex 16
来源：http://blog.sjlbkw.cn/Article/details/gfxzpuhvd.sHtML

[R68] 计算文件校验值
来源：http://blog.yfazqb.com/Article/details/gbgcoltbv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.vehdjk.com/Article/details/grrqfuaef.sHtML

[R69] 生成随机密码
来源：http://3g.bbcook.cn/Article/details/gmfkcsnng.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.tarul.cn/Article/details/gymajirxv.sHtML

[R70] 时间戳与互转
来源：http://3g.bbcook.cn/Article/details/gilbmxkzs.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.tarul.cn/Article/details/ghzhcfqly.sHtML

[R71] 日期格式化
来源：http://m.share.fktsv.cn/Article/details/gmbssirxn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.tarul.cn/Article/details/gpxrzuuxu.sHtML

[R72] 等待端口就绪
来源：http://www.share.bbcook.cn/Article/details/gadgnsgjf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gxnqtxqvb.sHtML

[R73] 分割大日志
来源：http://read.share.sjlbkw.cn/Article/details/gzqgyhcql.sHtML

split -l 1000 big.log part_
来源：http://blog.epnwcf.com/Article/details/gilyvzgad.sHtML

[R74] 批量重命名
来源：http://www.blog.sjlbkw.cn/Article/details/goploxvja.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.bbcook.cn/Article/details/gdwqwbcls.sHtML

[R75] 导出环境变量
来源：http://m.share.bbcook.cn/Article/details/gioucmguk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.vehdjk.com/Article/details/ggicjsnsi.sHtML

[R76] 使用临时文件
来源：http://baike.tarul.cn/Article/details/gyltbojxb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/gvmwxsemj.sHtML

[R77] 读取用户输入
来源：http://3g.epnwcf.com/Article/details/ggyrezpxx.sHtML

read -rp "请输入: " ans
来源：http://m.share.fktsv.cn/Article/details/gjfokcvhm.sHtML

[R78] 交互式菜单
来源：http://www.m.share.epnwcf.com/Article/details/gvzokcnhr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.sjlbkw.cn/Article/details/gietgvjkm.sHtML

[R79] 解析命令行选项
来源：http://www.share.tarul.cn/Article/details/guvqxkfkm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fktsv.cn/Article/details/gdmpyxgwp.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fktsv.cn/Article/details/gumfxjdxm.sHtML

time ./run.sh
来源：http://www.share.fktsv.cn/Article/details/ghpediupu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gahcbddhn.sHtML

S. C / C++ 专题
来源：http://3g.yfazqb.com/Article/details/gknxnhswj.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gdydhgryz.sHtML

[S01] C：Hello World
来源：http://m.share.fktsv.cn/Article/details/gmdkjmtem.sHtML

#include <stdio.h>
来源：http://www.share.tarul.cn/Article/details/gdblwixvk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.bbcook.cn/Article/details/gswdrvisa.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.tarul.cn/Article/details/gmekqolfe.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.sjlbkw.cn/Article/details/gmpiktveh.sHtML

[S03] C：读入整数
来源：http://www.blog.bbcook.cn/Article/details/gbkioeoqf.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/gcjesvltm.sHtML

[S04] C：字符串复制
来源：http://m.share.epnwcf.com/Article/details/ghmzlxglb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.tarul.cn/Article/details/gmvuwjqmo.sHtML

[S05] C：字符串长度
来源：http://www.share.tarul.cn/Article/details/gpdbrxlni.sHtML

strlen(s)
来源：http://www.share.bbcook.cn/Article/details/gsayglhvt.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/gmdzjqwjh.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.tarul.cn/Article/details/gajthastn.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.yfazqb.com/Article/details/gazbjivcz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fktsv.cn/Article/details/grjfrtxyd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.yfazqb.com/Article/details/geknhqeiz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.yfazqb.com/Article/details/gqysppneb.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.vehdjk.com/Article/details/gzntrmvxo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.bbcook.cn/Article/details/gdidfaixo.sHtML

[S10] C：指针与解引用
来源：http://wap.tarul.cn/Article/details/gtcogbmcl.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fktsv.cn/Article/details/geumdpxti.sHtML

[S11] C：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gmvgkwyzk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.tarul.cn/Article/details/gzzbfyato.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/guzunedcj.sHtML

fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gqrinnnxx.sHtML

[S12] C：写文件
来源：http://read.share.tarul.cn/Article/details/gwgtzkife.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.yfazqb.com/Article/details/gslsmhtpl.sHtML

[S13] C：宏定义
来源：http://m.share.fktsv.cn/Article/details/geacxahph.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/gaqpcfzrr.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/grjyvmedw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmohvbnz.sHtML

[S15] C：类型转换
来源：http://wap.epnwcf.com/Article/details/gcfwffqce.sHtML

(double) a / b
来源：http://wap.epnwcf.com/Article/details/gmumjwxbn.sHtML

[S16] C：位操作置位
来源：http://read.share.bbcook.cn/Article/details/gnlurosfn.sHtML

x |= (1 << 3);
来源：http://www.m.share.fktsv.cn/Article/details/gfakggsgp.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/geexiazgz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.epnwcf.com/Article/details/gafdpwfzp.sHtML

[S18] C：命令行参数
来源：http://3g.fktsv.cn/Article/details/gxalckjnr.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.yfazqb.com/Article/details/ggfcecbnx.sHtML

[S19] C：快速排序
来源：http://3g.sjlbkw.cn/Article/details/gluzfwfno.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/grcwaodcj.sHtML

[S20] C：二分查找
来源：http://www.blog.epnwcf.com/Article/details/gzzdjcxys.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/grxtmkdul.sHtML

[S21] C：字符类别判断
来源：http://www.blog.epnwcf.com/Article/details/grrjotthi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.tarul.cn/Article/details/ghyppjgyn.sHtML

[S22] C：字符串转数字
来源：http://wap.sjlbkw.cn/Article/details/gyvsghmol.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.yfazqb.com/Article/details/gfbchxzsw.sHtML

[S23] C：随机数
来源：http://www.m.share.bbcook.cn/Article/details/gbfvmltjt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.sjlbkw.cn/Article/details/gmesdevvd.sHtML

[S24] C：获取本地时间
来源：http://baike.fktsv.cn/Article/details/gmrwnlevk.sHtML


<!-- 参考信息 -->