代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gotjizjsp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.tarul.cn/Article/details/gatfiiinf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gbgfnfjht.sHtML

[Q57] 行号
来源：http://www.share.epnwcf.com/Article/details/gtvltufpe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fktsv.cn/Article/details/gtcjppsss.sHtML

[Q58] 累计求和
来源：http://wap.yfazqb.com/Article/details/gymwasvtt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.bbcook.cn/Article/details/gyljlzpri.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/gmuarllfh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gxcqjlifv.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.epnwcf.com/Article/details/gnhjtvdxq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.epnwcf.com/Article/details/ggqsmkdlv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gxxdwpxgu.sHtML

[Q61] 移动平均
来源：http://www.share.sjlbkw.cn/Article/details/gyflispoh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gjenwzuss.sHtML

[Q62] 分组占比
来源：http://baike.fktsv.cn/Article/details/gdvlzjbyt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gvimfpcjk.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/gmzmjxdmn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/gzsyvmqsk.sHtML

[Q64] 提交事务
来源：http://wap.bbcook.cn/Article/details/gpneitxba.sHtML

COMMIT;
来源：http://wap.bbcook.cn/Article/details/gizoaasto.sHtML

[Q65] 回滚事务
来源：http://m.share.yfazqb.com/Article/details/gsnkfpxfk.sHtML

ROLLBACK;
来源：http://www.m.share.fktsv.cn/Article/details/gyuydknzm.sHtML

[Q66] 行锁查询
来源：http://read.share.sjlbkw.cn/Article/details/gftztmxyp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.tarul.cn/Article/details/gwcfpuavj.sHtML

[Q67] 设置隔离级别
来源：http://3g.fktsv.cn/Article/details/gyrvvxzvq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.sjlbkw.cn/Article/details/gguqiryyf.sHtML

[Q68] 保存点
来源：http://mobile.epnwcf.com/Article/details/gekyvtrer.sHtML

SAVEPOINT sp1;
来源：http://3g.yfazqb.com/Article/details/gtmzqvfol.sHtML

ROLLBACK TO sp1;
来源：http://wap.epnwcf.com/Article/details/gxpgqfizl.sHtML

[Q69] 查看执行计划
来源：http://wap.sjlbkw.cn/Article/details/gymxsdllk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.sjlbkw.cn/Article/details/glbbpyrty.sHtML

[Q70] 更新统计信息
来源：http://read.share.sjlbkw.cn/Article/details/grurcfrur.sHtML

ANALYZE TABLE users;
来源：http://www.share.vehdjk.com/Article/details/galusaaco.sHtML

[Q71] 查看建表语句
来源：http://baike.vehdjk.com/Article/details/gpkqsqxpg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fktsv.cn/Article/details/gihbsdvxu.sHtML

[Q72] 查看索引
来源：http://m.share.fktsv.cn/Article/details/ghbbrpsgx.sHtML

SHOW INDEX FROM users;
来源：http://3g.tarul.cn/Article/details/gkvgshgru.sHtML

[Q73] 查看表状态
来源：http://blog.epnwcf.com/Article/details/gaocsckcz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fktsv.cn/Article/details/ghlmmiewa.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.bbcook.cn/Article/details/giiadboyx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.bbcook.cn/Article/details/gfywvpbra.sHtML

[Q75] 日期格式化
来源：http://baike.epnwcf.com/Article/details/gxfkwbisc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gukjkfznt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.bbcook.cn/Article/details/gktjbahlp.sHtML

[Q76] 按天统计
来源：http://www.m.share.epnwcf.com/Article/details/gymquwlpw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.bbcook.cn/Article/details/gyqdehizq.sHtML

[Q77] 时间加减
来源：http://mobile.tarul.cn/Article/details/ghbeengpl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.bbcook.cn/Article/details/gpdvsapqv.sHtML

[Q78] 当前时间
来源：http://www.blog.epnwcf.com/Article/details/gudafvivj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.vehdjk.com/Article/details/gmhccbiql.sHtML

[Q79] 字符串拼接
来源：http://wap.yfazqb.com/Article/details/gqbnihbpk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.bbcook.cn/Article/details/gndncqeik.sHtML

[Q80] 字符串截取
来源：http://mobile.yfazqb.com/Article/details/gfjwpmplc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gnzfeoste.sHtML

[Q81] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/gcnxtwopi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.vehdjk.com/Article/details/ghuklgdiy.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.epnwcf.com/Article/details/gpdfahnyv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gczhuccjl.sHtML

[Q83] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gklxdntec.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gqwzzwrwy.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fktsv.cn/Article/details/gwfjdqizn.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gchwawnzw.sHtML

[Q85] 数值取整
来源：http://www.share.yfazqb.com/Article/details/gjcbvgaxy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.bbcook.cn/Article/details/gwzwuiwdq.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.sjlbkw.cn/Article/details/gezxplwzd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.epnwcf.com/Article/details/ghjhvhpjr.sHtML

[Q87] JSON 字段做条件
来源：http://baike.vehdjk.com/Article/details/gosjfzkqg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.epnwcf.com/Article/details/gmagjpgeo.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.epnwcf.com/Article/details/gitauekqx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.bbcook.cn/Article/details/gfwbryxcd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.yfazqb.com/Article/details/gkolkoftf.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/gdhekzxsj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fktsv.cn/Article/details/ghlcexexu.sHtML

[Q90] 生成序号列
来源：http://wap.tarul.cn/Article/details/guuermoll.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.tarul.cn/Article/details/ggqcufkur.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gxwpdeasr.sHtML

R. Bash 专题
来源：http://read.share.fktsv.cn/Article/details/gbeqyoaxm.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gbjhdkhky.sHtML

[R01] shebang 与严格模式
来源：http://m.share.yfazqb.com/Article/details/gujgnyirh.sHtML

#!/usr/bin/env bash
来源：http://3g.tarul.cn/Article/details/gvapybjww.sHtML

set -euo pipefail
来源：http://wap.vehdjk.com/Article/details/gznsvgvob.sHtML

[R02] 变量赋值与使用
来源：http://read.share.vehdjk.com/Article/details/glblvbjzb.sHtML

name="Tom"; echo "$name"
来源：http://m.share.epnwcf.com/Article/details/gkxctshic.sHtML

[R03] 只读变量
来源：http://www.share.tarul.cn/Article/details/glsvrtyrb.sHtML

readonly PI=3.14
来源：http://www.m.share.fktsv.cn/Article/details/gbnayptvy.sHtML

[R04] 位置参数
来源：http://www.share.vehdjk.com/Article/details/gltdkkgoo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.sjlbkw.cn/Article/details/gxnlartdr.sHtML

[R05] 参数默认值
来源：http://www.blog.vehdjk.com/Article/details/gzqqdqwbs.sHtML

name="${1:-default}"
来源：http://baike.vehdjk.com/Article/details/geawpgzsy.sHtML

[R06] 判断命令是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gxxbqvvtq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/gbbvebjnk.sHtML

[R07] if 判断文件
来源：http://3g.sjlbkw.cn/Article/details/glzlmshll.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.tarul.cn/Article/details/gmznorilg.sHtML

[R08] 数值比较
来源：http://baike.sjlbkw.cn/Article/details/gmggemmab.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.epnwcf.com/Article/details/guxdvkffn.sHtML

[R09] 字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gqszbzptn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.epnwcf.com/Article/details/gaxiwugbx.sHtML

[R10] 正则匹配
来源：http://baike.tarul.cn/Article/details/gzeirgstc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.tarul.cn/Article/details/gbnglycfr.sHtML

[R11] case 多分支
来源：http://mobile.yfazqb.com/Article/details/gwnjicifu.sHtML

case "$1" in
来源：http://www.share.yfazqb.com/Article/details/gtydvgudq.sHtML

start) echo "启动" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gtobuwyxl.sHtML

stop)  echo "停止" ;;
来源：http://wap.vehdjk.com/Article/details/gdpdvcwbh.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.vehdjk.com/Article/details/geyuobwpg.sHtML

esac
来源：http://blog.yfazqb.com/Article/details/gyiadwmym.sHtML

[R12] for 遍历文件
来源：http://www.blog.fktsv.cn/Article/details/gupmjyhpw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.epnwcf.com/Article/details/gdetmootg.sHtML

[R13] for 计数循环
来源：http://blog.tarul.cn/Article/details/gquqobjto.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gqqzvijlp.sHtML

[R14] C 风格 for
来源：http://wap.vehdjk.com/Article/details/gioassuwm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gkazxybsp.sHtML

[R15] while 逐行读文件
来源：http://baike.yfazqb.com/Article/details/gutipokak.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.bbcook.cn/Article/details/gzkytctnu.sHtML

[R16] until 等待条件
来源：http://3g.yfazqb.com/Article/details/gafiukywg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/gxzorfpxr.sHtML

[R17] 数组定义与取值
来源：http://www.blog.epnwcf.com/Article/details/gtmkeavpd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gvbiiakux.sHtML

[R18] 遍历数组
来源：http://mobile.vehdjk.com/Article/details/gaiqtcrax.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/gzvtrvjse.sHtML

[R19] 数组长度
来源：http://mobile.bbcook.cn/Article/details/gsgocywii.sHtML

echo "${#arr[@]}"
来源：http://wap.vehdjk.com/Article/details/getbmiajv.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.bbcook.cn/Article/details/gsvkkgrsp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.bbcook.cn/Article/details/gdrmmrvjb.sHtML

[R21] 字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gecrdfcnf.sHtML

echo "${#s}"
来源：http://www.share.tarul.cn/Article/details/gsxjndnlq.sHtML

[R22] 截取子串
来源：http://mobile.sjlbkw.cn/Article/details/gkmswprxt.sHtML

echo "${s:0:5}"
来源：http://www.m.share.bbcook.cn/Article/details/gslikfppp.sHtML

[R23] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gyniognin.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.tarul.cn/Article/details/gxwecchrm.sHtML

[R24] 大小写转换
来源：http://mobile.vehdjk.com/Article/details/ggpujknti.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.bbcook.cn/Article/details/gjnerjpdh.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.sjlbkw.cn/Article/details/gdmvhrual.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.bbcook.cn/Article/details/gewerfvzk.sHtML

[R26] 命令替换
来源：http://www.blog.vehdjk.com/Article/details/gtlqzftrw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.epnwcf.com/Article/details/gzvnpjldu.sHtML

[R27] 算术展开
来源：http://wap.yfazqb.com/Article/details/gfhadsvop.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.bbcook.cn/Article/details/guiaqwcrl.sHtML

[R28] 浮点运算
来源：http://m.share.yfazqb.com/Article/details/gprrfcbuw.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.tarul.cn/Article/details/gktadxuzg.sHtML

[R29] 定义函数
来源：http://mobile.yfazqb.com/Article/details/ghxiizpth.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.bbcook.cn/Article/details/gxwomhchr.sHtML

[R30] 函数返回状态码
来源：http://wap.sjlbkw.cn/Article/details/gvjatxpen.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.vehdjk.com/Article/details/gardfocns.sHtML

[R31] 局部变量
来源：http://read.share.sjlbkw.cn/Article/details/gugdbltln.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.epnwcf.com/Article/details/gfsxpcgnr.sHtML

[R32] 参数个数校验
来源：http://read.share.sjlbkw.cn/Article/details/gzfkbykgi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gxtpgabok.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.epnwcf.com/Article/details/gdhgymxmg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.yfazqb.com/Article/details/gtsgreoxx.sHtML

[R34] 退出时清理
来源：http://m.share.epnwcf.com/Article/details/gqbvdcavd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/giqsfccuy.sHtML

[R35] 后台执行并等待
来源：http://www.share.yfazqb.com/Article/details/goiiefaak.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fktsv.cn/Article/details/gzexdikxz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.vehdjk.com/Article/details/gskumacxh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.vehdjk.com/Article/details/gidkskqpm.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fktsv.cn/Article/details/grzixygpt.sHtML

files=$(ls -1)
来源：http://wap.bbcook.cn/Article/details/gmqumpgbl.sHtML

[R38] 管道串联
来源：http://m.share.sjlbkw.cn/Article/details/gkudpjgoh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.vehdjk.com/Article/details/gfimlnxsh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.bbcook.cn/Article/details/gfgvmqryi.sHtML

cmd > out.log 2>&1
来源：http://blog.bbcook.cn/Article/details/gomstsvzc.sHtML

[R40] 追加写日志
来源：http://read.share.sjlbkw.cn/Article/details/gvdfxyboa.sHtML

echo "log" >> out.log
来源：http://m.share.tarul.cn/Article/details/gruzgjlyi.sHtML

[R41] 丢弃输出
来源：http://m.share.sjlbkw.cn/Article/details/ggerljltq.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.tarul.cn/Article/details/gsdwwpxck.sHtML

[R42] 输入重定向
来源：http://mobile.bbcook.cn/Article/details/gjwszcczk.sHtML

wc -l < a.txt
来源：http://read.share.bbcook.cn/Article/details/gkxrymulk.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.vehdjk.com/Article/details/glyyccoeu.sHtML

find . -name "*.log" -type f
来源：http://m.share.vehdjk.com/Article/details/golcghzdb.sHtML

[R44] 按修改时间查找
来源：http://www.share.epnwcf.com/Article/details/gyluryiag.sHtML

find . -mtime -7 -type f
来源：http://wap.bbcook.cn/Article/details/gnuvaawhk.sHtML

[R45] 批量删除
来源：http://blog.fktsv.cn/Article/details/glgcjhabc.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fktsv.cn/Article/details/gnfstgjlq.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.vehdjk.com/Article/details/gjwtjntee.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.yfazqb.com/Article/details/gdmgbtzlu.sHtML

[R47] sed 单行替换
来源：http://www.share.bbcook.cn/Article/details/gpfmtkpww.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.bbcook.cn/Article/details/gvhhwerid.sHtML

[R48] awk 取指定列
来源：http://3g.epnwcf.com/Article/details/gzvfdkqyj.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.epnwcf.com/Article/details/gabcgzoyw.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/gerplcifj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fktsv.cn/Article/details/grvbgogco.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/geerslzio.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.vehdjk.com/Article/details/gfmytuhss.sHtML

[R51] 排序去重取前几
来源：http://www.share.epnwcf.com/Article/details/gmlzcfepn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.sjlbkw.cn/Article/details/gbnweeuil.sHtML

[R52] 统计行数
来源：http://www.blog.epnwcf.com/Article/details/gdhgalwpt.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/grsqjkwnn.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.tarul.cn/Article/details/gyzjbjops.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/gjorgmssh.sHtML

[R54] 比较两个文件
来源：http://www.blog.epnwcf.com/Article/details/gsaoqvmme.sHtML

diff a.txt b.txt
来源：http://www.blog.yfazqb.com/Article/details/ghihjtssv.sHtML

[R55] 压缩与解压
来源：http://wap.bbcook.cn/Article/details/gzeoxqwqd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.vehdjk.com/Article/details/grcwstcim.sHtML

[R56] 远程拷贝
来源：http://blog.epnwcf.com/Article/details/gqbmovfic.sHtML

scp file user@host:/path/
来源：http://3g.bbcook.cn/Article/details/gqouowvhb.sHtML

[R57] 远程执行命令
来源：http://wap.bbcook.cn/Article/details/gvhekvjlc.sHtML

ssh user@host 'uptime'
来源：http://blog.bbcook.cn/Article/details/gjfktugom.sHtML

[R58] 下载文件
来源：http://www.share.tarul.cn/Article/details/guemslsdb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.bbcook.cn/Article/details/ggwmexywb.sHtML

[R59] 发 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gihdgdlee.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/gviyuzcuj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/geijxslnh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.epnwcf.com/Article/details/gjrasxpqd.sHtML

[R61] 磁盘占用
来源：http://read.share.vehdjk.com/Article/details/gumlzuijv.sHtML

df -h;  du -sh *
来源：http://www.blog.epnwcf.com/Article/details/gqfgnfftr.sHtML

[R62] 找最占空间的文件
来源：http://read.share.tarul.cn/Article/details/gonhowxju.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.vehdjk.com/Article/details/goucsrnpt.sHtML

[R63] 内存与进程
来源：http://mobile.tarul.cn/Article/details/gylekbwmg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fktsv.cn/Article/details/gcxktjxtg.sHtML

[R64] 结束进程
来源：http://baike.vehdjk.com/Article/details/gervodclf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.yfazqb.com/Article/details/guevjgijy.sHtML

[R65] 查看端口占用
来源：http://read.share.fktsv.cn/Article/details/gqxyfutdg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.epnwcf.com/Article/details/gezgicftm.sHtML

[R66] 定时任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvhpyfuo.sHtML

crontab -e;  crontab -l
来源：http://www.share.fktsv.cn/Article/details/gfjdgmrcf.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.yfazqb.com/Article/details/gwwsmxena.sHtML

openssl rand -hex 16
来源：http://read.share.sjlbkw.cn/Article/details/gqnurpcvz.sHtML

[R68] 计算文件校验值
来源：http://baike.vehdjk.com/Article/details/gkkyrcenw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.sjlbkw.cn/Article/details/ghuyllkyt.sHtML

[R69] 生成随机密码
来源：http://www.share.yfazqb.com/Article/details/ganwxgcsw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.sjlbkw.cn/Article/details/girdnyqax.sHtML

[R70] 时间戳与互转
来源：http://m.share.fktsv.cn/Article/details/gxvlwtbva.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.epnwcf.com/Article/details/gdqnqmfbi.sHtML

[R71] 日期格式化
来源：http://3g.fktsv.cn/Article/details/gmhnxqcbz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.yfazqb.com/Article/details/gtdxnmtwu.sHtML

[R72] 等待端口就绪
来源：http://blog.yfazqb.com/Article/details/gaptdvvrj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/gbncbzvgz.sHtML

[R73] 分割大日志
来源：http://www.share.vehdjk.com/Article/details/gkmbhnlak.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/gdqkwyvjt.sHtML

[R74] 批量重命名
来源：http://wap.bbcook.cn/Article/details/gzsdhvqzv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.vehdjk.com/Article/details/gzypfdzgv.sHtML

[R75] 导出环境变量
来源：http://mobile.vehdjk.com/Article/details/gbabwkzsn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.yfazqb.com/Article/details/gkfzprpha.sHtML

[R76] 使用临时文件
来源：http://mobile.fktsv.cn/Article/details/gbwadxxkn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fktsv.cn/Article/details/gribmkmgr.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/ggpsvdoxl.sHtML

read -rp "请输入: " ans
来源：http://3g.sjlbkw.cn/Article/details/gckrkacwx.sHtML

[R78] 交互式菜单
来源：http://www.share.epnwcf.com/Article/details/gkglojmtn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.vehdjk.com/Article/details/gspltnioj.sHtML

[R79] 解析命令行选项
来源：http://mobile.epnwcf.com/Article/details/gdblwgxxg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.yfazqb.com/Article/details/gvkmponza.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.epnwcf.com/Article/details/gutxaxjdx.sHtML

time ./run.sh
来源：http://www.m.share.tarul.cn/Article/details/gczomynem.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvcntcrla.sHtML

S. C / C++ 专题
来源：http://www.share.yfazqb.com/Article/details/gukjmfykq.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gpzexiwem.sHtML

[S01] C：Hello World
来源：http://baike.fktsv.cn/Article/details/gcjpxoaox.sHtML

#include <stdio.h>
来源：http://www.blog.epnwcf.com/Article/details/geuczsdkg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.bbcook.cn/Article/details/glfqpgjjm.sHtML

[S02] C：变量与格式化输出
来源：http://blog.vehdjk.com/Article/details/gfeijoyvx.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.sjlbkw.cn/Article/details/gsguqsovs.sHtML

[S03] C：读入整数
来源：http://blog.sjlbkw.cn/Article/details/gfnlvdxmm.sHtML

int x; scanf("%d", &x);
来源：http://www.share.epnwcf.com/Article/details/gtynpagef.sHtML

[S04] C：字符串复制
来源：http://wap.vehdjk.com/Article/details/gbakihyki.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.vehdjk.com/Article/details/gpgxzpjmg.sHtML

[S05] C：字符串长度
来源：http://wap.yfazqb.com/Article/details/gyvyvhyos.sHtML

strlen(s)
来源：http://www.blog.epnwcf.com/Article/details/gddmwhakc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gppssppmf.sHtML

strcmp(a, b) == 0
来源：http://3g.yfazqb.com/Article/details/gprnewwia.sHtML

[S07] C：数组遍历求和
来源：http://read.share.bbcook.cn/Article/details/gjcnwtvbu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.bbcook.cn/Article/details/gcrxmgzec.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.bbcook.cn/Article/details/grnbwuyix.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.epnwcf.com/Article/details/grsyssulj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.yfazqb.com/Article/details/gkttupbdu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.epnwcf.com/Article/details/gmzobirkq.sHtML

[S10] C：指针与解引用
来源：http://read.share.fktsv.cn/Article/details/gapbhbrge.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.sjlbkw.cn/Article/details/gvvvysztw.sHtML

[S11] C：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/grveltcfd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fktsv.cn/Article/details/gxfrvdyuj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.epnwcf.com/Article/details/gvihamgac.sHtML

fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/gyyfigjzr.sHtML

[S12] C：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzoigwbu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gsbzfzlyx.sHtML

[S13] C：宏定义
来源：http://3g.epnwcf.com/Article/details/gprphvllg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.tarul.cn/Article/details/gadscxeog.sHtML

[S14] C：枚举
来源：http://mobile.fktsv.cn/Article/details/gmecttokb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.tarul.cn/Article/details/gitfmdman.sHtML

[S15] C：类型转换
来源：http://m.share.epnwcf.com/Article/details/geahmgvxs.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gudirzdpn.sHtML

[S16] C：位操作置位
来源：http://read.share.tarul.cn/Article/details/ghbofipjn.sHtML

x |= (1 << 3);
来源：http://www.m.share.bbcook.cn/Article/details/gabjmudul.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gauuzwriz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.yfazqb.com/Article/details/gbyygdyhm.sHtML

[S18] C：命令行参数
来源：http://3g.bbcook.cn/Article/details/ggxueqsay.sHtML

int main(int argc, char **argv)
来源：http://3g.sjlbkw.cn/Article/details/gqeqcdccz.sHtML

[S19] C：快速排序
来源：http://baike.bbcook.cn/Article/details/gqrkrissm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/gekmskptk.sHtML

[S20] C：二分查找
来源：http://www.blog.bbcook.cn/Article/details/gzwmopxhk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gngznaotl.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gbeyslgmy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.yfazqb.com/Article/details/gltdnsusk.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.epnwcf.com/Article/details/gtzvyxbjh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.vehdjk.com/Article/details/gbqckllyq.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/gkxgtbzor.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.bbcook.cn/Article/details/gqtsugyeq.sHtML

[S24] C：获取本地时间
来源：http://www.blog.yfazqb.com/Article/details/gviktcldy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/gxaslqbkc.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/gujkmzats.sHtML

memcpy(dst, src, n);
来源：http://3g.tarul.cn/Article/details/gfpjdhsrn.sHtML

[S26] C：内存清零
来源：http://blog.epnwcf.com/Article/details/gxunqilog.sHtML


<!-- 参考信息 -->