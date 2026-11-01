代发 wailian999

[Q48] CTE 公用表表达式
来源：http://wap.tarul.cn/Article/details/guvnjbcvf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.yfazqb.com/Article/details/gpwbngbpf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.vehdjk.com/Article/details/goyuxvomj.sHtML

[Q49] 更新单行
来源：http://m.share.epnwcf.com/Article/details/gwcmibiya.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/getamovqu.sHtML

[Q50] 批量更新
来源：http://www.m.share.yfazqb.com/Article/details/gkqpnpked.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.yfazqb.com/Article/details/gxqcgsujz.sHtML

[Q51] 用子查询更新
来源：http://read.share.tarul.cn/Article/details/gvhtencoe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/gfyzuxtsd.sHtML

[Q52] 删除指定行
来源：http://3g.sjlbkw.cn/Article/details/gkbcvybgb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gicpzyojf.sHtML

[Q53] 按条件删除
来源：http://wap.fktsv.cn/Article/details/geolhysff.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fktsv.cn/Article/details/gkyalxarz.sHtML

[Q54] 清空表
来源：http://mobile.tarul.cn/Article/details/gnrirdahp.sHtML

TRUNCATE TABLE logs;
来源：http://wap.yfazqb.com/Article/details/gntpodyhg.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.sjlbkw.cn/Article/details/gxxwxtyqc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gmzeahsgy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.vehdjk.com/Article/details/golccihnc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.bbcook.cn/Article/details/gfbpqyudn.sHtML

[Q57] 行号
来源：http://baike.sjlbkw.cn/Article/details/gacysgfbk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/ggacqjmod.sHtML

[Q58] 累计求和
来源：http://blog.epnwcf.com/Article/details/gdbfdekbv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.epnwcf.com/Article/details/guljsqbko.sHtML

[Q59] 分组内累计
来源：http://m.share.fktsv.cn/Article/details/gqkcemxrx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gmupywsss.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.vehdjk.com/Article/details/gltstpyaa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.tarul.cn/Article/details/gfaosoeah.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gsvashdya.sHtML

[Q61] 移动平均
来源：http://blog.tarul.cn/Article/details/gktkiaabz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/guqtqggeq.sHtML

[Q62] 分组占比
来源：http://www.blog.fktsv.cn/Article/details/gvtiwhcyi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gvpjfzhra.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/gebcjgbxj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.vehdjk.com/Article/details/ghwahphmd.sHtML

[Q64] 提交事务
来源：http://www.blog.epnwcf.com/Article/details/gvfnhmjzg.sHtML

COMMIT;
来源：http://baike.fktsv.cn/Article/details/gcqclypux.sHtML

[Q65] 回滚事务
来源：http://mobile.tarul.cn/Article/details/gnijxwiva.sHtML

ROLLBACK;
来源：http://www.m.share.bbcook.cn/Article/details/glrojrqiw.sHtML

[Q66] 行锁查询
来源：http://baike.epnwcf.com/Article/details/gyefderho.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fktsv.cn/Article/details/gjogvtgcw.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fktsv.cn/Article/details/gaalrvizv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/gemezmirk.sHtML

[Q68] 保存点
来源：http://www.blog.vehdjk.com/Article/details/ghxrdzgtd.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gpkkfwife.sHtML

ROLLBACK TO sp1;
来源：http://read.share.yfazqb.com/Article/details/gqfeccflm.sHtML

[Q69] 查看执行计划
来源：http://mobile.tarul.cn/Article/details/gdtcbqpab.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.tarul.cn/Article/details/ggiyyzkro.sHtML

[Q70] 更新统计信息
来源：http://read.share.fktsv.cn/Article/details/geqksqsta.sHtML

ANALYZE TABLE users;
来源：http://mobile.bbcook.cn/Article/details/gramslbrr.sHtML

[Q71] 查看建表语句
来源：http://baike.fktsv.cn/Article/details/gbteatkvp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/glhmchcpf.sHtML

[Q72] 查看索引
来源：http://www.m.share.epnwcf.com/Article/details/gwwpzzybd.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gldxzucuc.sHtML

[Q73] 查看表状态
来源：http://3g.fktsv.cn/Article/details/ggmnmzwfk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.vehdjk.com/Article/details/gfoterbwj.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.vehdjk.com/Article/details/genqjrfrt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.yfazqb.com/Article/details/ginwotzmu.sHtML

[Q75] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gwsvxcsmw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gebryxpcf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.sjlbkw.cn/Article/details/ggwzuccmq.sHtML

[Q76] 按天统计
来源：http://blog.fktsv.cn/Article/details/gdiicydjf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.tarul.cn/Article/details/gtkqwxihb.sHtML

[Q77] 时间加减
来源：http://m.share.bbcook.cn/Article/details/grliwwjzm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.bbcook.cn/Article/details/gqeenrzrh.sHtML

[Q78] 当前时间
来源：http://m.share.tarul.cn/Article/details/gbheajlgh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/gihfrqsfb.sHtML

[Q79] 字符串拼接
来源：http://mobile.vehdjk.com/Article/details/gfwagmllu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.vehdjk.com/Article/details/gwdekzwkn.sHtML

[Q80] 字符串截取
来源：http://blog.yfazqb.com/Article/details/gcufvnxxa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.tarul.cn/Article/details/gzqbvckeg.sHtML

[Q81] 字符串替换
来源：http://3g.sjlbkw.cn/Article/details/gywlxvkba.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.tarul.cn/Article/details/ghbchzkci.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/gqmznfyhm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gurtwzyld.sHtML

[Q83] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/ggliaassd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/goobwjpfr.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fktsv.cn/Article/details/grgsvncaj.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/grfganyhs.sHtML

[Q85] 数值取整
来源：http://blog.sjlbkw.cn/Article/details/gkpjhhyws.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.yfazqb.com/Article/details/gvtaumoaa.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.vehdjk.com/Article/details/gdjhswohm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.vehdjk.com/Article/details/gbyoeoehh.sHtML

[Q87] JSON 字段做条件
来源：http://3g.epnwcf.com/Article/details/gexwlytux.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.yfazqb.com/Article/details/gmrmtizkp.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.tarul.cn/Article/details/gaxilhklr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.yfazqb.com/Article/details/gedxecept.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gxucpwcqq.sHtML

[Q89] 判断表是否存在
来源：http://m.share.bbcook.cn/Article/details/gqtnsdwvc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.sjlbkw.cn/Article/details/gkzpeoeaa.sHtML

[Q90] 生成序号列
来源：http://wap.yfazqb.com/Article/details/ggsnjkzce.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.vehdjk.com/Article/details/gzuxviykn.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gpbchssib.sHtML

R. Bash 专题
来源：http://mobile.yfazqb.com/Article/details/gpegcpmpj.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gkmwmocla.sHtML

[R01] shebang 与严格模式
来源：http://wap.bbcook.cn/Article/details/gvgapulay.sHtML

#!/usr/bin/env bash
来源：http://wap.sjlbkw.cn/Article/details/giabbqjaf.sHtML

set -euo pipefail
来源：http://m.share.tarul.cn/Article/details/gvlkecwns.sHtML

[R02] 变量赋值与使用
来源：http://read.share.sjlbkw.cn/Article/details/gmuuccxlj.sHtML

name="Tom"; echo "$name"
来源：http://mobile.epnwcf.com/Article/details/gntdmyqos.sHtML

[R03] 只读变量
来源：http://www.share.bbcook.cn/Article/details/gfpyjwdtg.sHtML

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/gsprgdgro.sHtML

[R04] 位置参数
来源：http://www.blog.epnwcf.com/Article/details/gimjryrzh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fktsv.cn/Article/details/gufpazytz.sHtML

[R05] 参数默认值
来源：http://m.share.tarul.cn/Article/details/ghuchsonq.sHtML

name="${1:-default}"
来源：http://baike.tarul.cn/Article/details/gerhtcbwr.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.tarul.cn/Article/details/gtbmnlooa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/gsncgppbp.sHtML

[R07] if 判断文件
来源：http://wap.bbcook.cn/Article/details/gpyxdevuh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.yfazqb.com/Article/details/gsriaukgf.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/gsccvhwtr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.bbcook.cn/Article/details/gjwsbydbd.sHtML

[R09] 字符串比较
来源：http://mobile.fktsv.cn/Article/details/gsdcyrvfx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.vehdjk.com/Article/details/gqzjgbunt.sHtML

[R10] 正则匹配
来源：http://mobile.tarul.cn/Article/details/ghtlfhgtj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.vehdjk.com/Article/details/gnhtditzs.sHtML

[R11] case 多分支
来源：http://www.m.share.epnwcf.com/Article/details/gxtukgeed.sHtML

case "$1" in
来源：http://www.share.tarul.cn/Article/details/ghgtcnnrb.sHtML

start) echo "启动" ;;
来源：http://3g.epnwcf.com/Article/details/gvxtnwues.sHtML

stop)  echo "停止" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gvqajazhz.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.bbcook.cn/Article/details/gcmegmqak.sHtML

esac
来源：http://mobile.bbcook.cn/Article/details/giainunbr.sHtML

[R12] for 遍历文件
来源：http://www.share.tarul.cn/Article/details/gukahfpgg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fktsv.cn/Article/details/ggtlzvhjk.sHtML

[R13] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gtojfpjrf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gziuezqhx.sHtML

[R14] C 风格 for
来源：http://mobile.sjlbkw.cn/Article/details/gzhywlivt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gdehoqtgf.sHtML

[R15] while 逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gknzgvbhz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.yfazqb.com/Article/details/gawmvidys.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gavcyzjhv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gehrrvwkq.sHtML

[R17] 数组定义与取值
来源：http://m.share.sjlbkw.cn/Article/details/grlbrkolb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fktsv.cn/Article/details/guytwuhfq.sHtML

[R18] 遍历数组
来源：http://wap.tarul.cn/Article/details/gxpdefhkj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.sjlbkw.cn/Article/details/ghzdlrctk.sHtML

[R19] 数组长度
来源：http://blog.epnwcf.com/Article/details/gujufrufa.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/gajtkviou.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.epnwcf.com/Article/details/gwtfqpeix.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.vehdjk.com/Article/details/gptifxerd.sHtML

[R21] 字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/glnolgjzl.sHtML

echo "${#s}"
来源：http://blog.sjlbkw.cn/Article/details/gbtnjzacb.sHtML

[R22] 截取子串
来源：http://www.blog.tarul.cn/Article/details/gxqffgloa.sHtML

echo "${s:0:5}"
来源：http://m.share.fktsv.cn/Article/details/glzfihdpt.sHtML

[R23] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gitmnahhe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.sjlbkw.cn/Article/details/ghuulygyj.sHtML

[R24] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gkiokjjht.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.sjlbkw.cn/Article/details/gecebwadn.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.vehdjk.com/Article/details/gsdxvscfn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.tarul.cn/Article/details/geysxnqnd.sHtML

[R26] 命令替换
来源：http://m.share.fktsv.cn/Article/details/gmtgvinhf.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fktsv.cn/Article/details/gqjnasxfd.sHtML

[R27] 算术展开
来源：http://blog.epnwcf.com/Article/details/gxgkqeukq.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.sjlbkw.cn/Article/details/gqrlkkqle.sHtML

[R28] 浮点运算
来源：http://3g.epnwcf.com/Article/details/gphrdysxz.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/gewswdtma.sHtML

[R29] 定义函数
来源：http://baike.fktsv.cn/Article/details/gygznyith.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.yfazqb.com/Article/details/gmzpyijfz.sHtML

[R30] 函数返回状态码
来源：http://blog.tarul.cn/Article/details/gtxmikpdf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.yfazqb.com/Article/details/geltpwxpu.sHtML

[R31] 局部变量
来源：http://baike.fktsv.cn/Article/details/gytnxiekb.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.tarul.cn/Article/details/gvumfwxzh.sHtML

[R32] 参数个数校验
来源：http://www.share.bbcook.cn/Article/details/ghrkztjcg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghatdswkb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.vehdjk.com/Article/details/ggvksrwki.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.yfazqb.com/Article/details/gpchzgctk.sHtML

[R34] 退出时清理
来源：http://www.m.share.sjlbkw.cn/Article/details/gydssszio.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gillkfswu.sHtML

[R35] 后台执行并等待
来源：http://3g.bbcook.cn/Article/details/gpprnhfrw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.epnwcf.com/Article/details/gefoltfhd.sHtML

[R36] 并发执行多个任务
来源：http://read.share.tarul.cn/Article/details/gfdsworac.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fktsv.cn/Article/details/glqmqqhxx.sHtML

[R37] 把输出赋给变量
来源：http://wap.vehdjk.com/Article/details/grusloqrx.sHtML

files=$(ls -1)
来源：http://www.m.share.tarul.cn/Article/details/gqfkqvtrg.sHtML

[R38] 管道串联
来源：http://blog.epnwcf.com/Article/details/grnyexsns.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.yfazqb.com/Article/details/gjkapomfl.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.epnwcf.com/Article/details/ghgcdzjml.sHtML

cmd > out.log 2>&1
来源：http://blog.fktsv.cn/Article/details/ghdpmkvus.sHtML

[R40] 追加写日志
来源：http://baike.yfazqb.com/Article/details/gwdcoeoow.sHtML

echo "log" >> out.log
来源：http://wap.sjlbkw.cn/Article/details/gpqfppoub.sHtML

[R41] 丢弃输出
来源：http://m.share.yfazqb.com/Article/details/guuikdysf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/ggspmeyzf.sHtML

[R42] 输入重定向
来源：http://www.blog.fktsv.cn/Article/details/gsvtwdyju.sHtML

wc -l < a.txt
来源：http://baike.tarul.cn/Article/details/gzsixtdcd.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fktsv.cn/Article/details/ghsvhohsw.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.tarul.cn/Article/details/gedamidkp.sHtML

[R44] 按修改时间查找
来源：http://www.share.yfazqb.com/Article/details/giodcfeel.sHtML

find . -mtime -7 -type f
来源：http://blog.fktsv.cn/Article/details/gpzrgdnca.sHtML

[R45] 批量删除
来源：http://blog.vehdjk.com/Article/details/godkolmwn.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/gwlszhnuk.sHtML

[R46] 递归替换文件内容
来源：http://3g.bbcook.cn/Article/details/gkfuvhtrh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.sjlbkw.cn/Article/details/goxdiycrq.sHtML

[R47] sed 单行替换
来源：http://www.share.bbcook.cn/Article/details/gbriqezwt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.yfazqb.com/Article/details/glqljwvac.sHtML

[R48] awk 取指定列
来源：http://m.share.yfazqb.com/Article/details/gdiitzvgt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gflpmsmaa.sHtML

[R49] awk 带条件
来源：http://www.blog.fktsv.cn/Article/details/gmyjsuvcy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.bbcook.cn/Article/details/gqwgkvchi.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/grtzpxjwj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.bbcook.cn/Article/details/ghjqwertl.sHtML

[R51] 排序去重取前几
来源：http://3g.bbcook.cn/Article/details/gjaqiuucw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/gohqcdbns.sHtML

[R52] 统计行数
来源：http://read.share.epnwcf.com/Article/details/gzufqadwx.sHtML

wc -l a.txt
来源：http://3g.fktsv.cn/Article/details/gxztshpfm.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.sjlbkw.cn/Article/details/gekcntatn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fktsv.cn/Article/details/gyjlcqmnc.sHtML

[R54] 比较两个文件
来源：http://www.share.epnwcf.com/Article/details/gvyocnihv.sHtML

diff a.txt b.txt
来源：http://m.share.bbcook.cn/Article/details/gpcwqbfsj.sHtML

[R55] 压缩与解压
来源：http://www.blog.yfazqb.com/Article/details/gtnhibjlw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.sjlbkw.cn/Article/details/gcmxwbuyo.sHtML

[R56] 远程拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gvajvkmei.sHtML

scp file user@host:/path/
来源：http://read.share.epnwcf.com/Article/details/gggxsqokv.sHtML

[R57] 远程执行命令
来源：http://www.blog.vehdjk.com/Article/details/gkzhivovz.sHtML

ssh user@host 'uptime'
来源：http://wap.bbcook.cn/Article/details/grgrbfdyw.sHtML

[R58] 下载文件
来源：http://read.share.fktsv.cn/Article/details/gjtsgwwqq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.yfazqb.com/Article/details/gvjwyoxic.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gkxwxtkhx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.yfazqb.com/Article/details/gfoiqrogx.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gzrilxqdf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.sjlbkw.cn/Article/details/gqlgzqwta.sHtML

[R61] 磁盘占用
来源：http://mobile.bbcook.cn/Article/details/gniizxvvk.sHtML

df -h;  du -sh *
来源：http://wap.tarul.cn/Article/details/gdefzirda.sHtML

[R62] 找最占空间的文件
来源：http://blog.bbcook.cn/Article/details/gleudriww.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.tarul.cn/Article/details/giyvvnhtg.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gafkfqfys.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fktsv.cn/Article/details/gcmxhuswe.sHtML

[R64] 结束进程
来源：http://m.share.sjlbkw.cn/Article/details/gzpgrwuad.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fktsv.cn/Article/details/gwfekfbys.sHtML

[R65] 查看端口占用
来源：http://baike.sjlbkw.cn/Article/details/grlpuuhrn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fktsv.cn/Article/details/gmoxzqesa.sHtML

[R66] 定时任务
来源：http://www.blog.vehdjk.com/Article/details/gxjdflzqc.sHtML

crontab -e;  crontab -l
来源：http://read.share.sjlbkw.cn/Article/details/gheqndxls.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.yfazqb.com/Article/details/gwotlvwhs.sHtML

openssl rand -hex 16
来源：http://wap.fktsv.cn/Article/details/ggfamwpdu.sHtML

[R68] 计算文件校验值
来源：http://www.blog.bbcook.cn/Article/details/gpemdzdkw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.yfazqb.com/Article/details/gwasoyjcs.sHtML

[R69] 生成随机密码
来源：http://wap.bbcook.cn/Article/details/gvmkoqebq.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.bbcook.cn/Article/details/gngarjfwf.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/guiaekpwb.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/gnzvohrkz.sHtML

[R71] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/gnevscqyz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.yfazqb.com/Article/details/gvmvfnjjk.sHtML

[R72] 等待端口就绪
来源：http://blog.tarul.cn/Article/details/gpxehtbyq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gfjrcyavp.sHtML

[R73] 分割大日志
来源：http://m.share.vehdjk.com/Article/details/grhncqdtb.sHtML

split -l 1000 big.log part_
来源：http://mobile.bbcook.cn/Article/details/gonclvekg.sHtML

[R74] 批量重命名
来源：http://wap.yfazqb.com/Article/details/gpzmnvzje.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.sjlbkw.cn/Article/details/gymgcgwnn.sHtML

[R75] 导出环境变量
来源：http://baike.yfazqb.com/Article/details/gdiqxaaid.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.bbcook.cn/Article/details/gykckxcwm.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/gvrdzlvom.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/ggdkacbgi.sHtML

[R77] 读取用户输入
来源：http://wap.yfazqb.com/Article/details/gtfptrhix.sHtML

read -rp "请输入: " ans
来源：http://www.share.fktsv.cn/Article/details/glovvlcpw.sHtML

[R78] 交互式菜单
来源：http://www.blog.yfazqb.com/Article/details/gouoemdcu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.tarul.cn/Article/details/gzdhgqccv.sHtML

[R79] 解析命令行选项
来源：http://read.share.epnwcf.com/Article/details/gwugozaph.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.bbcook.cn/Article/details/gkdtxpfds.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.tarul.cn/Article/details/gxbobrmwc.sHtML

time ./run.sh
来源：http://blog.yfazqb.com/Article/details/gxpuuahol.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gkleigfiy.sHtML

S. C / C++ 专题
来源：http://read.share.yfazqb.com/Article/details/gxcunteyx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gntfriiup.sHtML

[S01] C：Hello World
来源：http://3g.sjlbkw.cn/Article/details/givgjkdoy.sHtML

#include <stdio.h>
来源：http://mobile.tarul.cn/Article/details/gvuanqcrc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fktsv.cn/Article/details/gscbobhbx.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fktsv.cn/Article/details/gzvtvivgs.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.epnwcf.com/Article/details/glrzhrgno.sHtML

[S03] C：读入整数
来源：http://www.blog.fktsv.cn/Article/details/gbuexlqee.sHtML

int x; scanf("%d", &x);
来源：http://baike.bbcook.cn/Article/details/gentvbwrk.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/gdiaumhlt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.sjlbkw.cn/Article/details/gvghupcqk.sHtML

[S05] C：字符串长度
来源：http://blog.epnwcf.com/Article/details/gogkjwhly.sHtML

strlen(s)
来源：http://www.blog.yfazqb.com/Article/details/gapnddhsz.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/gccpxeetd.sHtML

strcmp(a, b) == 0
来源：http://www.blog.vehdjk.com/Article/details/gsijxflge.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fktsv.cn/Article/details/gbqinsvpk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/gqujyvgfx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.bbcook.cn/Article/details/gyktnetrv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.tarul.cn/Article/details/guwzkvpfy.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.vehdjk.com/Article/details/gcgqefbnu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.bbcook.cn/Article/details/groxhkgjb.sHtML

[S10] C：指针与解引用
来源：http://mobile.epnwcf.com/Article/details/gcpmonepx.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fktsv.cn/Article/details/gpcedyqiz.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/giauqduob.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fktsv.cn/Article/details/gznbehkiq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.epnwcf.com/Article/details/gkuqjgywi.sHtML

fclose(f);
来源：http://wap.vehdjk.com/Article/details/gkkujjwuo.sHtML

[S12] C：写文件
来源：http://www.blog.yfazqb.com/Article/details/gqpbtuxxj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.vehdjk.com/Article/details/gnoeupzis.sHtML

[S13] C：宏定义
来源：http://read.share.epnwcf.com/Article/details/gwbsthosv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.epnwcf.com/Article/details/gqssrljsc.sHtML

[S14] C：枚举
来源：http://read.share.bbcook.cn/Article/details/gwdlzmnox.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.epnwcf.com/Article/details/gmayovmge.sHtML

[S15] C：类型转换
来源：http://mobile.bbcook.cn/Article/details/gpronnamd.sHtML

(double) a / b
来源：http://mobile.yfazqb.com/Article/details/gsijydxoa.sHtML

[S16] C：位操作置位
来源：http://3g.epnwcf.com/Article/details/gaostzroy.sHtML

x |= (1 << 3);
来源：http://3g.epnwcf.com/Article/details/gyrluctvb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/ggddwhcbk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.epnwcf.com/Article/details/gwjnkgcfc.sHtML

[S18] C：命令行参数
来源：http://mobile.sjlbkw.cn/Article/details/gpgzaytts.sHtML


<!-- 参考信息 -->