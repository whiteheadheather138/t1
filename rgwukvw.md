代发 wailian999

[Q48] CTE 公用表表达式
来源：http://baike.sjlbkw.cn/Article/details/gwnfxkkbn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.tarul.cn/Article/details/gksodncoz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.bbcook.cn/Article/details/gwkzgmfvn.sHtML

[Q49] 更新单行
来源：http://www.blog.vehdjk.com/Article/details/gunmmbzrh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gkrjoxcew.sHtML

[Q50] 批量更新
来源：http://m.share.bbcook.cn/Article/details/ghjmpuxgd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.tarul.cn/Article/details/ggoloftjl.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.vehdjk.com/Article/details/gjytglgwa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.tarul.cn/Article/details/gnvllsunl.sHtML

[Q52] 删除指定行
来源：http://m.share.sjlbkw.cn/Article/details/gswcgkhhd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fktsv.cn/Article/details/gwfygntas.sHtML

[Q53] 按条件删除
来源：http://wap.fktsv.cn/Article/details/gxdnysoax.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.tarul.cn/Article/details/gigcipzue.sHtML

[Q54] 清空表
来源：http://blog.yfazqb.com/Article/details/gsefvryly.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.vehdjk.com/Article/details/gxaunyvcb.sHtML

[Q55] 排名（并列占位）
来源：http://baike.epnwcf.com/Article/details/gmaprmzzk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gbouaoazp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fktsv.cn/Article/details/gamzorbdg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/glelrjhrw.sHtML

[Q57] 行号
来源：http://mobile.vehdjk.com/Article/details/gkpkwrkfm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fktsv.cn/Article/details/gjyvroybq.sHtML

[Q58] 累计求和
来源：http://mobile.bbcook.cn/Article/details/gkvcnaiwl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.yfazqb.com/Article/details/gqpkbnhdf.sHtML

[Q59] 分组内累计
来源：http://m.share.fktsv.cn/Article/details/gmenmulmk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gstcwaozj.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.tarul.cn/Article/details/gafeehmhm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.epnwcf.com/Article/details/gffcighyw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gsdoonsim.sHtML

[Q61] 移动平均
来源：http://www.blog.bbcook.cn/Article/details/gyvwekxls.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/ggirgolwv.sHtML

[Q62] 分组占比
来源：http://m.share.fktsv.cn/Article/details/grjqcnjvg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gengpqsog.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/gyzvlpolm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.tarul.cn/Article/details/gknzrbben.sHtML

[Q64] 提交事务
来源：http://wap.sjlbkw.cn/Article/details/grznumnxi.sHtML

COMMIT;
来源：http://www.blog.vehdjk.com/Article/details/gtjmkeeco.sHtML

[Q65] 回滚事务
来源：http://3g.vehdjk.com/Article/details/grjnqzipf.sHtML

ROLLBACK;
来源：http://wap.vehdjk.com/Article/details/glegqdriq.sHtML

[Q66] 行锁查询
来源：http://www.blog.epnwcf.com/Article/details/gpaohtxmx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.yfazqb.com/Article/details/giikuizcm.sHtML

[Q67] 设置隔离级别
来源：http://mobile.sjlbkw.cn/Article/details/gzvfflgal.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.epnwcf.com/Article/details/gesmfxgjq.sHtML

[Q68] 保存点
来源：http://baike.tarul.cn/Article/details/gghxsweom.sHtML

SAVEPOINT sp1;
来源：http://wap.tarul.cn/Article/details/ggzvxgevs.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.bbcook.cn/Article/details/ghxzwsfpo.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gxfourqjj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.sjlbkw.cn/Article/details/gbpmfudzp.sHtML

[Q70] 更新统计信息
来源：http://mobile.yfazqb.com/Article/details/gwwupjyqw.sHtML

ANALYZE TABLE users;
来源：http://www.share.bbcook.cn/Article/details/gwflsqgfu.sHtML

[Q71] 查看建表语句
来源：http://wap.bbcook.cn/Article/details/gorxjwsbf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.epnwcf.com/Article/details/gdyuwyvcq.sHtML

[Q72] 查看索引
来源：http://mobile.yfazqb.com/Article/details/gcqfdsdst.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.tarul.cn/Article/details/gnrkppzqz.sHtML

[Q73] 查看表状态
来源：http://www.blog.bbcook.cn/Article/details/gugftiqrk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.epnwcf.com/Article/details/gvdexytan.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fktsv.cn/Article/details/glkyucsme.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.vehdjk.com/Article/details/gylodjeqz.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/ggzhtxcdb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.tarul.cn/Article/details/guqnsmmlw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.epnwcf.com/Article/details/gaynruxuc.sHtML

[Q76] 按天统计
来源：http://www.blog.bbcook.cn/Article/details/gsjzhhudr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fktsv.cn/Article/details/ghjzubwhh.sHtML

[Q77] 时间加减
来源：http://www.m.share.fktsv.cn/Article/details/ghfnlbnpk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfucstgx.sHtML

[Q78] 当前时间
来源：http://mobile.sjlbkw.cn/Article/details/ghpiyuhhl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.tarul.cn/Article/details/gmiyjwnzi.sHtML

[Q79] 字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gvveiwebw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.tarul.cn/Article/details/gxdqtzobh.sHtML

[Q80] 字符串截取
来源：http://www.share.tarul.cn/Article/details/grifbytva.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.tarul.cn/Article/details/gotcrcjjf.sHtML

[Q81] 字符串替换
来源：http://baike.tarul.cn/Article/details/gbqyshanj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.epnwcf.com/Article/details/gfxhtezph.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.vehdjk.com/Article/details/gynorneht.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/gglcweodl.sHtML

[Q83] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gkygtaizl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gkylxiwob.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fktsv.cn/Article/details/gnpwslyhf.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gdnltuqmr.sHtML

[Q85] 数值取整
来源：http://read.share.epnwcf.com/Article/details/gknfmcmch.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.tarul.cn/Article/details/ggmhezsth.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.vehdjk.com/Article/details/gbihdkddk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.bbcook.cn/Article/details/gdstofrxx.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/gsuuijccs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.yfazqb.com/Article/details/gqokppowo.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.yfazqb.com/Article/details/geybrxpow.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.epnwcf.com/Article/details/gvrzyodgq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.tarul.cn/Article/details/gfdicpnbk.sHtML

[Q89] 判断表是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gblgvkrwa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.tarul.cn/Article/details/gdbagodvc.sHtML

[Q90] 生成序号列
来源：http://blog.epnwcf.com/Article/details/gesryaqop.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.vehdjk.com/Article/details/gaemmtffw.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grekqzbws.sHtML

R. Bash 专题
来源：http://3g.bbcook.cn/Article/details/gaplqqdwi.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/giknbasjk.sHtML

[R01] shebang 与严格模式
来源：http://blog.sjlbkw.cn/Article/details/grawgxnzc.sHtML

#!/usr/bin/env bash
来源：http://wap.sjlbkw.cn/Article/details/geumfprob.sHtML

set -euo pipefail
来源：http://www.share.sjlbkw.cn/Article/details/gbhvjcskr.sHtML

[R02] 变量赋值与使用
来源：http://baike.yfazqb.com/Article/details/gdeositdg.sHtML

name="Tom"; echo "$name"
来源：http://m.share.sjlbkw.cn/Article/details/guloyyjfr.sHtML

[R03] 只读变量
来源：http://mobile.yfazqb.com/Article/details/gpqlhfgaq.sHtML

readonly PI=3.14
来源：http://3g.yfazqb.com/Article/details/gymhdriri.sHtML

[R04] 位置参数
来源：http://www.share.tarul.cn/Article/details/gxtnayhzz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.yfazqb.com/Article/details/ggrrlbdih.sHtML

[R05] 参数默认值
来源：http://3g.vehdjk.com/Article/details/grumuyywk.sHtML

name="${1:-default}"
来源：http://www.blog.yfazqb.com/Article/details/gjqkzlrck.sHtML

[R06] 判断命令是否存在
来源：http://wap.sjlbkw.cn/Article/details/gfjvrzlxu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/ginxrqfyj.sHtML

[R07] if 判断文件
来源：http://mobile.sjlbkw.cn/Article/details/gkdpdndcb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.epnwcf.com/Article/details/gdqsnmacq.sHtML

[R08] 数值比较
来源：http://mobile.bbcook.cn/Article/details/giebepbsa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.bbcook.cn/Article/details/gccannmlt.sHtML

[R09] 字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/gynctrmsv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gfhndukpm.sHtML

[R10] 正则匹配
来源：http://www.share.fktsv.cn/Article/details/guotbxxun.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.vehdjk.com/Article/details/ggpdszpkj.sHtML

[R11] case 多分支
来源：http://wap.tarul.cn/Article/details/gcfwkqekv.sHtML

case "$1" in
来源：http://baike.fktsv.cn/Article/details/gaxobaefn.sHtML

start) echo "启动" ;;
来源：http://www.share.fktsv.cn/Article/details/gaxdaadrq.sHtML

stop)  echo "停止" ;;
来源：http://mobile.epnwcf.com/Article/details/gcporbltp.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.tarul.cn/Article/details/gvbwxxllc.sHtML

esac
来源：http://baike.fktsv.cn/Article/details/ghgyhhruv.sHtML

[R12] for 遍历文件
来源：http://www.share.sjlbkw.cn/Article/details/gpzegcxjb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.sjlbkw.cn/Article/details/ggozpjuza.sHtML

[R13] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/ggaovbakh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/gmtazdbwd.sHtML

[R14] C 风格 for
来源：http://m.share.fktsv.cn/Article/details/gchrmobir.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/giopnuhdg.sHtML

[R15] while 逐行读文件
来源：http://baike.bbcook.cn/Article/details/ghdrzjvij.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.tarul.cn/Article/details/geljciuiz.sHtML

[R16] until 等待条件
来源：http://read.share.vehdjk.com/Article/details/givdlpuft.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/grqzpnesv.sHtML

[R17] 数组定义与取值
来源：http://read.share.fktsv.cn/Article/details/gqulfmmgn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.epnwcf.com/Article/details/gmseeozrc.sHtML

[R18] 遍历数组
来源：http://3g.bbcook.cn/Article/details/gmgahyuje.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/ghgjtgjix.sHtML

[R19] 数组长度
来源：http://m.share.bbcook.cn/Article/details/ggycrgxtt.sHtML

echo "${#arr[@]}"
来源：http://baike.bbcook.cn/Article/details/gupsgdwir.sHtML

[R20] 关联数组（字典）
来源：http://baike.bbcook.cn/Article/details/gnlvoiucw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.epnwcf.com/Article/details/gbezwqnze.sHtML

[R21] 字符串长度
来源：http://read.share.vehdjk.com/Article/details/gfieerdko.sHtML

echo "${#s}"
来源：http://wap.bbcook.cn/Article/details/gwkpcagos.sHtML

[R22] 截取子串
来源：http://wap.vehdjk.com/Article/details/ggewtfbey.sHtML

echo "${s:0:5}"
来源：http://m.share.fktsv.cn/Article/details/gltcnahaz.sHtML

[R23] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/gpipatiol.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.yfazqb.com/Article/details/gptzqvefc.sHtML

[R24] 大小写转换
来源：http://3g.fktsv.cn/Article/details/gbpmyvehy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.epnwcf.com/Article/details/gjreaplwa.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.sjlbkw.cn/Article/details/gyoidzwdh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fktsv.cn/Article/details/grvkmbgdv.sHtML

[R26] 命令替换
来源：http://www.share.epnwcf.com/Article/details/gdhghccpw.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.epnwcf.com/Article/details/gtnboyvcm.sHtML

[R27] 算术展开
来源：http://m.share.fktsv.cn/Article/details/gfbhykqgt.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.epnwcf.com/Article/details/gppklhwda.sHtML

[R28] 浮点运算
来源：http://3g.vehdjk.com/Article/details/gwwkmzygg.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.epnwcf.com/Article/details/gvwcdiqfb.sHtML

[R29] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gvhzeupui.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.vehdjk.com/Article/details/gakbvccsu.sHtML

[R30] 函数返回状态码
来源：http://3g.vehdjk.com/Article/details/gdcrxykno.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.tarul.cn/Article/details/gjcbewxnl.sHtML

[R31] 局部变量
来源：http://baike.yfazqb.com/Article/details/gtlspfyql.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.tarul.cn/Article/details/gtakkqjpt.sHtML

[R32] 参数个数校验
来源：http://m.share.sjlbkw.cn/Article/details/grqxzluug.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.sjlbkw.cn/Article/details/gmfotluyy.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/gzhaanwur.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.bbcook.cn/Article/details/garzhrool.sHtML

[R34] 退出时清理
来源：http://www.share.epnwcf.com/Article/details/gatagwuda.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gqdaiidmn.sHtML

[R35] 后台执行并等待
来源：http://mobile.sjlbkw.cn/Article/details/gszhpjcdh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.bbcook.cn/Article/details/gbvjzuihj.sHtML

[R36] 并发执行多个任务
来源：http://m.share.yfazqb.com/Article/details/gfuadfqbp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.epnwcf.com/Article/details/ghggriwwd.sHtML

[R37] 把输出赋给变量
来源：http://baike.yfazqb.com/Article/details/grbqxlmmp.sHtML

files=$(ls -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghiuzofqp.sHtML

[R38] 管道串联
来源：http://wap.epnwcf.com/Article/details/gkwhpqkly.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.yfazqb.com/Article/details/gxgcnpzjn.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.sjlbkw.cn/Article/details/gkparftdg.sHtML

cmd > out.log 2>&1
来源：http://baike.epnwcf.com/Article/details/gnhuxiuyr.sHtML

[R40] 追加写日志
来源：http://www.share.sjlbkw.cn/Article/details/gfrdfhurm.sHtML

echo "log" >> out.log
来源：http://www.m.share.yfazqb.com/Article/details/gzdwfudcs.sHtML

[R41] 丢弃输出
来源：http://baike.bbcook.cn/Article/details/ggfwermxf.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.vehdjk.com/Article/details/guwtjlrpm.sHtML

[R42] 输入重定向
来源：http://baike.vehdjk.com/Article/details/gcrphmxxs.sHtML

wc -l < a.txt
来源：http://wap.sjlbkw.cn/Article/details/gyenyjylh.sHtML

[R43] 按名字查找文件
来源：http://www.share.sjlbkw.cn/Article/details/gdowbgpag.sHtML

find . -name "*.log" -type f
来源：http://wap.vehdjk.com/Article/details/gjhseuthd.sHtML

[R44] 按修改时间查找
来源：http://3g.sjlbkw.cn/Article/details/gjpasbkjj.sHtML

find . -mtime -7 -type f
来源：http://www.share.vehdjk.com/Article/details/gpiewaaig.sHtML

[R45] 批量删除
来源：http://baike.bbcook.cn/Article/details/gnvitpcxa.sHtML

find . -name "*.tmp" -delete
来源：http://3g.epnwcf.com/Article/details/gsxjyabvn.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fktsv.cn/Article/details/ggmpzydyl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.epnwcf.com/Article/details/gaxgiqoea.sHtML

[R47] sed 单行替换
来源：http://www.m.share.vehdjk.com/Article/details/gvlfxbpqj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.tarul.cn/Article/details/gwvgilypw.sHtML

[R48] awk 取指定列
来源：http://3g.yfazqb.com/Article/details/gdmiiljne.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gfhyyjgdy.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/gsynsrfcb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.yfazqb.com/Article/details/gnsjkjkka.sHtML

[R50] awk 求和
来源：http://mobile.epnwcf.com/Article/details/gkthcvyfi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gtvosmvaw.sHtML

[R51] 排序去重取前几
来源：http://wap.sjlbkw.cn/Article/details/gwfgqhanh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/gzbgvcwiu.sHtML

[R52] 统计行数
来源：http://www.m.share.sjlbkw.cn/Article/details/gelsirxao.sHtML

wc -l a.txt
来源：http://wap.fktsv.cn/Article/details/gmxonhuoj.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/ggzqsjnck.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.yfazqb.com/Article/details/gcgvdptxw.sHtML

[R54] 比较两个文件
来源：http://3g.fktsv.cn/Article/details/gcitsjohz.sHtML

diff a.txt b.txt
来源：http://blog.vehdjk.com/Article/details/gezpsllvd.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/guljlhtzy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.epnwcf.com/Article/details/gaaicplia.sHtML

[R56] 远程拷贝
来源：http://baike.sjlbkw.cn/Article/details/gomartfwr.sHtML

scp file user@host:/path/
来源：http://read.share.epnwcf.com/Article/details/gyjrezane.sHtML

[R57] 远程执行命令
来源：http://3g.fktsv.cn/Article/details/gceeftimu.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.epnwcf.com/Article/details/geqvgzzph.sHtML

[R58] 下载文件
来源：http://www.blog.tarul.cn/Article/details/gkwiticnq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.tarul.cn/Article/details/gobxreiud.sHtML

[R59] 发 POST JSON
来源：http://m.share.tarul.cn/Article/details/goqstjdrb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.yfazqb.com/Article/details/gtsidqizf.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/gqojuktkr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.epnwcf.com/Article/details/gezhyqhjl.sHtML

[R61] 磁盘占用
来源：http://3g.tarul.cn/Article/details/gxokrmgyh.sHtML

df -h;  du -sh *
来源：http://read.share.tarul.cn/Article/details/gedknadrc.sHtML

[R62] 找最占空间的文件
来源：http://3g.fktsv.cn/Article/details/ggkzhfpbb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.epnwcf.com/Article/details/geqbsfvrk.sHtML

[R63] 内存与进程
来源：http://wap.yfazqb.com/Article/details/gkctejqwu.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.sjlbkw.cn/Article/details/gwmoimfrf.sHtML

[R64] 结束进程
来源：http://read.share.vehdjk.com/Article/details/gnvtdkqso.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.sjlbkw.cn/Article/details/gvfeoccal.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fktsv.cn/Article/details/ghxfoskae.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvqbbmtb.sHtML

[R66] 定时任务
来源：http://wap.yfazqb.com/Article/details/ghttepiiy.sHtML

crontab -e;  crontab -l
来源：http://blog.tarul.cn/Article/details/gyanfspge.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.tarul.cn/Article/details/glsuqsrhq.sHtML

openssl rand -hex 16
来源：http://m.share.vehdjk.com/Article/details/gtikuwnqw.sHtML

[R68] 计算文件校验值
来源：http://www.share.fktsv.cn/Article/details/gblsmcruc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gulnmpdtf.sHtML

[R69] 生成随机密码
来源：http://mobile.sjlbkw.cn/Article/details/guncshmwf.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.tarul.cn/Article/details/gsoqdtrnd.sHtML

[R70] 时间戳与互转
来源：http://blog.tarul.cn/Article/details/gdeazyram.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.vehdjk.com/Article/details/gqywwsucd.sHtML

[R71] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gvofeufps.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.vehdjk.com/Article/details/gitvdibpi.sHtML

[R72] 等待端口就绪
来源：http://www.share.vehdjk.com/Article/details/gtnotoazd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/gjpjktwhp.sHtML

[R73] 分割大日志
来源：http://wap.bbcook.cn/Article/details/gycjursgd.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/gejrntsqx.sHtML

[R74] 批量重命名
来源：http://m.share.vehdjk.com/Article/details/gvavffpzm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.vehdjk.com/Article/details/gksymabpm.sHtML

[R75] 导出环境变量
来源：http://m.share.bbcook.cn/Article/details/gmperkira.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.tarul.cn/Article/details/gjubmybqg.sHtML

[R76] 使用临时文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gopdqxjiq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/gqsgijxrs.sHtML

[R77] 读取用户输入
来源：http://baike.fktsv.cn/Article/details/gsbtzfprp.sHtML

read -rp "请输入: " ans
来源：http://read.share.tarul.cn/Article/details/gbfppoxjc.sHtML

[R78] 交互式菜单
来源：http://mobile.tarul.cn/Article/details/gcohnfpxb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.vehdjk.com/Article/details/gmwrmueyy.sHtML

[R79] 解析命令行选项
来源：http://read.share.tarul.cn/Article/details/glrocrnrc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.yfazqb.com/Article/details/gtqgcdaco.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.epnwcf.com/Article/details/gclkhwcvc.sHtML

time ./run.sh
来源：http://3g.epnwcf.com/Article/details/gewdxsdgf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvdbigkfg.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/gyaxpizxl.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvuawerzy.sHtML

[S01] C：Hello World
来源：http://3g.fktsv.cn/Article/details/guuaqvpqw.sHtML

#include <stdio.h>
来源：http://blog.bbcook.cn/Article/details/gkhybzbmt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fktsv.cn/Article/details/ggsujfvzp.sHtML

[S02] C：变量与格式化输出
来源：http://wap.tarul.cn/Article/details/goraxmcbk.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fktsv.cn/Article/details/gfugvlmvs.sHtML

[S03] C：读入整数
来源：http://wap.vehdjk.com/Article/details/gjfmzlgnv.sHtML

int x; scanf("%d", &x);
来源：http://mobile.tarul.cn/Article/details/gvuecftsm.sHtML

[S04] C：字符串复制
来源：http://wap.epnwcf.com/Article/details/gudbfyvij.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.sjlbkw.cn/Article/details/gslnclksl.sHtML

[S05] C：字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/ggucwcpyd.sHtML

strlen(s)
来源：http://www.share.bbcook.cn/Article/details/ggafnnaqj.sHtML

[S06] C：字符串比较
来源：http://www.m.share.tarul.cn/Article/details/gfhjajayp.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.tarul.cn/Article/details/gycvqylya.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fktsv.cn/Article/details/gstkgovsd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.sjlbkw.cn/Article/details/gulcyisbt.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fktsv.cn/Article/details/gbbrdzzma.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.sjlbkw.cn/Article/details/grvqxmhrx.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.bbcook.cn/Article/details/gdjnfhukz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.epnwcf.com/Article/details/gquziqarg.sHtML

[S10] C：指针与解引用
来源：http://blog.vehdjk.com/Article/details/gahoaelae.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.vehdjk.com/Article/details/gthdkdati.sHtML

[S11] C：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/ghcrccbzf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.vehdjk.com/Article/details/gdggmcvbm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fktsv.cn/Article/details/gjchjzoic.sHtML

fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gyrpuvece.sHtML

[S12] C：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gsvvyonjk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gopgmzlzb.sHtML

[S13] C：宏定义
来源：http://wap.bbcook.cn/Article/details/gqestipxr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.epnwcf.com/Article/details/gbezhnvcv.sHtML

[S14] C：枚举
来源：http://wap.sjlbkw.cn/Article/details/gjnmpossl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.tarul.cn/Article/details/gerfnqbja.sHtML

[S15] C：类型转换
来源：http://baike.vehdjk.com/Article/details/gsjxwzlwn.sHtML

(double) a / b
来源：http://mobile.tarul.cn/Article/details/gsmljaiet.sHtML

[S16] C：位操作置位
来源：http://www.m.share.yfazqb.com/Article/details/gbkbdbgpp.sHtML

x |= (1 << 3);
来源：http://read.share.tarul.cn/Article/details/greopnmgf.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gxsqhmvet.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.vehdjk.com/Article/details/gogblbxut.sHtML

[S18] C：命令行参数
来源：http://blog.yfazqb.com/Article/details/gcrhcgexj.sHtML


<!-- 参考信息 -->