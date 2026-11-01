代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.vehdjk.com/Article/details/gzshifrzx.sHtML

[Q58] 累计求和
来源：http://wap.sjlbkw.cn/Article/details/ghiowvfjq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.bbcook.cn/Article/details/gglvrnlph.sHtML

[Q59] 分组内累计
来源：http://www.m.share.yfazqb.com/Article/details/gssduypau.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gcdhuxqre.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.tarul.cn/Article/details/gvhzciwjm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.sjlbkw.cn/Article/details/gixdmdzhw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.vehdjk.com/Article/details/ggtqfqyyr.sHtML

[Q61] 移动平均
来源：http://www.m.share.vehdjk.com/Article/details/gbckxtboe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gvpvsyxzc.sHtML

[Q62] 分组占比
来源：http://wap.bbcook.cn/Article/details/guaeukcnn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gvegihwdy.sHtML

[Q63] 开启事务
来源：http://www.m.share.fktsv.cn/Article/details/gyqdajujs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fktsv.cn/Article/details/gnjjkydfv.sHtML

[Q64] 提交事务
来源：http://wap.vehdjk.com/Article/details/gjrthjgjz.sHtML

COMMIT;
来源：http://baike.bbcook.cn/Article/details/gcmktzsbf.sHtML

[Q65] 回滚事务
来源：http://baike.bbcook.cn/Article/details/gcxqzznbv.sHtML

ROLLBACK;
来源：http://read.share.tarul.cn/Article/details/gxidlotjm.sHtML

[Q66] 行锁查询
来源：http://www.share.tarul.cn/Article/details/gatlpswiz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.epnwcf.com/Article/details/gguvjnbsi.sHtML

[Q67] 设置隔离级别
来源：http://blog.vehdjk.com/Article/details/gwprljfmx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.bbcook.cn/Article/details/gcsrdcoua.sHtML

[Q68] 保存点
来源：http://read.share.epnwcf.com/Article/details/gegapsbtf.sHtML

SAVEPOINT sp1;
来源：http://3g.vehdjk.com/Article/details/gtoqhomsm.sHtML

ROLLBACK TO sp1;
来源：http://www.share.bbcook.cn/Article/details/gkltabhnq.sHtML

[Q69] 查看执行计划
来源：http://baike.yfazqb.com/Article/details/grpjbuuxa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fktsv.cn/Article/details/grjphurol.sHtML

[Q70] 更新统计信息
来源：http://3g.yfazqb.com/Article/details/gkwbzvzbi.sHtML

ANALYZE TABLE users;
来源：http://baike.yfazqb.com/Article/details/gpsxriyhi.sHtML

[Q71] 查看建表语句
来源：http://wap.fktsv.cn/Article/details/gkylqbhwh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.yfazqb.com/Article/details/gfsmsqofq.sHtML

[Q72] 查看索引
来源：http://mobile.sjlbkw.cn/Article/details/groqfwvhr.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.tarul.cn/Article/details/goxuewboc.sHtML

[Q73] 查看表状态
来源：http://www.share.tarul.cn/Article/details/gzhhmzbhb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.yfazqb.com/Article/details/gqkqtefzr.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fktsv.cn/Article/details/gxhrhfrar.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.epnwcf.com/Article/details/gojgglvcr.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gqtzlguwp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gxdkudnqg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.sjlbkw.cn/Article/details/guutgnhrx.sHtML

[Q76] 按天统计
来源：http://mobile.fktsv.cn/Article/details/ggseqxptl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.tarul.cn/Article/details/gawjvjxxg.sHtML

[Q77] 时间加减
来源：http://blog.fktsv.cn/Article/details/gudoiyqtx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.tarul.cn/Article/details/goigimqwh.sHtML

[Q78] 当前时间
来源：http://baike.fktsv.cn/Article/details/gfuqfyopw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.bbcook.cn/Article/details/gxbsjosry.sHtML

[Q79] 字符串拼接
来源：http://baike.vehdjk.com/Article/details/gpqmyxgfl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.vehdjk.com/Article/details/gowhrdzbb.sHtML

[Q80] 字符串截取
来源：http://www.blog.epnwcf.com/Article/details/gmmchzmnq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.tarul.cn/Article/details/gysxtjqnr.sHtML

[Q81] 字符串替换
来源：http://wap.fktsv.cn/Article/details/gtdxtcxit.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.tarul.cn/Article/details/gtrrmxjmm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/gugkolgsu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/gkzuqojvi.sHtML

[Q83] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gvtjqpsso.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gzgpifmly.sHtML

[Q84] 去除首尾空格
来源：http://m.share.sjlbkw.cn/Article/details/gwexcawzv.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gkerbchfm.sHtML

[Q85] 数值取整
来源：http://blog.tarul.cn/Article/details/glojkgcyl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.bbcook.cn/Article/details/greuutejg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.bbcook.cn/Article/details/gvwpilbqy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.bbcook.cn/Article/details/gxsubnsnd.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.sjlbkw.cn/Article/details/gngyczrmv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fktsv.cn/Article/details/geqajbvsg.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.sjlbkw.cn/Article/details/givgbtron.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.bbcook.cn/Article/details/gpgnldkdh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.vehdjk.com/Article/details/guijmdffv.sHtML

[Q89] 判断表是否存在
来源：http://www.share.epnwcf.com/Article/details/gsekbolta.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.yfazqb.com/Article/details/gzvwzpywq.sHtML

[Q90] 生成序号列
来源：http://m.share.tarul.cn/Article/details/ghzbzpbdd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/gakacoilc.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gejwpmfbv.sHtML

R. Bash 专题
来源：http://3g.epnwcf.com/Article/details/gssdoaiyb.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtlfgcjgz.sHtML

[R01] shebang 与严格模式
来源：http://3g.vehdjk.com/Article/details/gukdioehh.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fktsv.cn/Article/details/gekuuheih.sHtML

set -euo pipefail
来源：http://www.blog.epnwcf.com/Article/details/gkxceviao.sHtML

[R02] 变量赋值与使用
来源：http://blog.epnwcf.com/Article/details/gnewdzuuf.sHtML

name="Tom"; echo "$name"
来源：http://mobile.vehdjk.com/Article/details/gahtkmmaf.sHtML

[R03] 只读变量
来源：http://m.share.bbcook.cn/Article/details/gryaxhnfo.sHtML

readonly PI=3.14
来源：http://m.share.vehdjk.com/Article/details/gbjrnbhcw.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/gmilfgbsv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.yfazqb.com/Article/details/gryawoniv.sHtML

[R05] 参数默认值
来源：http://www.m.share.yfazqb.com/Article/details/gmzvligbh.sHtML

name="${1:-default}"
来源：http://www.m.share.yfazqb.com/Article/details/guwcjchjy.sHtML

[R06] 判断命令是否存在
来源：http://mobile.tarul.cn/Article/details/gfaadodco.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.vehdjk.com/Article/details/gpxqxuzhl.sHtML

[R07] if 判断文件
来源：http://wap.sjlbkw.cn/Article/details/gnttwexzn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.yfazqb.com/Article/details/gpsvhlevl.sHtML

[R08] 数值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gpsrwfzlc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.bbcook.cn/Article/details/gtihgzcxq.sHtML

[R09] 字符串比较
来源：http://blog.epnwcf.com/Article/details/gbwazqjda.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.yfazqb.com/Article/details/gzyydebll.sHtML

[R10] 正则匹配
来源：http://baike.bbcook.cn/Article/details/gfayjbwbb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.sjlbkw.cn/Article/details/gcfeqlbkm.sHtML

[R11] case 多分支
来源：http://www.blog.fktsv.cn/Article/details/gkwaimcrw.sHtML

case "$1" in
来源：http://blog.epnwcf.com/Article/details/gifghwmle.sHtML

start) echo "启动" ;;
来源：http://m.share.fktsv.cn/Article/details/gnrqvoxzl.sHtML

stop)  echo "停止" ;;
来源：http://blog.fktsv.cn/Article/details/gquzdynfd.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.sjlbkw.cn/Article/details/geftyzxuo.sHtML

esac
来源：http://read.share.vehdjk.com/Article/details/gkmfawwqf.sHtML

[R12] for 遍历文件
来源：http://wap.bbcook.cn/Article/details/gdauvktnt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.sjlbkw.cn/Article/details/gsouazoke.sHtML

[R13] for 计数循环
来源：http://m.share.sjlbkw.cn/Article/details/gznekwzhq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gkdllrqzk.sHtML

[R14] C 风格 for
来源：http://m.share.tarul.cn/Article/details/gkvabrvsj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.sjlbkw.cn/Article/details/gjtgflccr.sHtML

[R15] while 逐行读文件
来源：http://wap.fktsv.cn/Article/details/glzbpljgr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.vehdjk.com/Article/details/gvazwvcng.sHtML

[R16] until 等待条件
来源：http://mobile.tarul.cn/Article/details/gwdpombne.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/gvvjmokyi.sHtML

[R17] 数组定义与取值
来源：http://blog.yfazqb.com/Article/details/getsftzgz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.vehdjk.com/Article/details/gqmnpcsbh.sHtML

[R18] 遍历数组
来源：http://blog.yfazqb.com/Article/details/gskjgetju.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.bbcook.cn/Article/details/guwenjfls.sHtML

[R19] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/geyjguqjf.sHtML

echo "${#arr[@]}"
来源：http://wap.sjlbkw.cn/Article/details/gpfpfrqjf.sHtML

[R20] 关联数组（字典）
来源：http://baike.tarul.cn/Article/details/glgmapcrx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fktsv.cn/Article/details/gpkuskthf.sHtML

[R21] 字符串长度
来源：http://mobile.vehdjk.com/Article/details/gilkvfuxr.sHtML

echo "${#s}"
来源：http://m.share.sjlbkw.cn/Article/details/gjkaqqynn.sHtML

[R22] 截取子串
来源：http://3g.vehdjk.com/Article/details/gplhvpvqj.sHtML

echo "${s:0:5}"
来源：http://blog.epnwcf.com/Article/details/gdadvspnb.sHtML

[R23] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gwuucydit.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fktsv.cn/Article/details/ggqrwpnfz.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gcxelovof.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.tarul.cn/Article/details/gpsrapgfs.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.bbcook.cn/Article/details/gsqapqblb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.epnwcf.com/Article/details/gqgofftnq.sHtML

[R26] 命令替换
来源：http://baike.tarul.cn/Article/details/gndxiawwd.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.epnwcf.com/Article/details/gypejanxq.sHtML

[R27] 算术展开
来源：http://baike.yfazqb.com/Article/details/gchvsqrky.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.yfazqb.com/Article/details/gmbvpbtwo.sHtML

[R28] 浮点运算
来源：http://3g.vehdjk.com/Article/details/gsotbjfni.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/gqjuwopdn.sHtML

[R29] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gaqexjsxy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.yfazqb.com/Article/details/gzvzqlunl.sHtML

[R30] 函数返回状态码
来源：http://www.blog.vehdjk.com/Article/details/gnahtedzv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.yfazqb.com/Article/details/giikltivp.sHtML

[R31] 局部变量
来源：http://blog.vehdjk.com/Article/details/gymjrfsae.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.vehdjk.com/Article/details/ggabuhqql.sHtML

[R32] 参数个数校验
来源：http://m.share.fktsv.cn/Article/details/gjhntwzdg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gyztgytsh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.tarul.cn/Article/details/gzhirbvmj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.vehdjk.com/Article/details/gfxfyvrsx.sHtML

[R34] 退出时清理
来源：http://3g.vehdjk.com/Article/details/gvjmxtwnq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gxegxnmhd.sHtML

[R35] 后台执行并等待
来源：http://mobile.vehdjk.com/Article/details/gevokwjgy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.vehdjk.com/Article/details/gwxwaxghz.sHtML

[R36] 并发执行多个任务
来源：http://blog.tarul.cn/Article/details/gcxlsokab.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.epnwcf.com/Article/details/gkolzzzik.sHtML

[R37] 把输出赋给变量
来源：http://blog.yfazqb.com/Article/details/gfmgpbrbc.sHtML

files=$(ls -1)
来源：http://blog.sjlbkw.cn/Article/details/gbrmbglvy.sHtML

[R38] 管道串联
来源：http://wap.sjlbkw.cn/Article/details/ghysyrenu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.sjlbkw.cn/Article/details/gsntimnik.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fktsv.cn/Article/details/gmugsyrgk.sHtML

cmd > out.log 2>&1
来源：http://wap.yfazqb.com/Article/details/gndfgyygb.sHtML

[R40] 追加写日志
来源：http://baike.fktsv.cn/Article/details/gsttqkinj.sHtML

echo "log" >> out.log
来源：http://www.m.share.fktsv.cn/Article/details/ghmpvyste.sHtML

[R41] 丢弃输出
来源：http://3g.epnwcf.com/Article/details/gaozxdkln.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/guujxnuao.sHtML

[R42] 输入重定向
来源：http://3g.bbcook.cn/Article/details/giuaahlrh.sHtML

wc -l < a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gpiavvjcs.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gxnkxsuim.sHtML

find . -name "*.log" -type f
来源：http://mobile.tarul.cn/Article/details/gnaexqtiq.sHtML

[R44] 按修改时间查找
来源：http://wap.yfazqb.com/Article/details/gxzcspoxg.sHtML

find . -mtime -7 -type f
来源：http://m.share.fktsv.cn/Article/details/gboctdoic.sHtML

[R45] 批量删除
来源：http://www.share.tarul.cn/Article/details/gidxkwwaq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/gyzvygexx.sHtML

[R46] 递归替换文件内容
来源：http://baike.tarul.cn/Article/details/ggmphjfzf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.epnwcf.com/Article/details/ganntetfw.sHtML

[R47] sed 单行替换
来源：http://mobile.sjlbkw.cn/Article/details/gyaaiplql.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.vehdjk.com/Article/details/gizeutanr.sHtML

[R48] awk 取指定列
来源：http://baike.sjlbkw.cn/Article/details/gohziuaxu.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gkweyksmz.sHtML

[R49] awk 带条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gizhxtdqj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.tarul.cn/Article/details/gbwvsgupz.sHtML

[R50] awk 求和
来源：http://www.m.share.tarul.cn/Article/details/gsvxettop.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fktsv.cn/Article/details/ghnkvupjw.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.vehdjk.com/Article/details/gvtfkhkan.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.vehdjk.com/Article/details/gaefevsev.sHtML

[R52] 统计行数
来源：http://www.blog.vehdjk.com/Article/details/gwvnrwetd.sHtML

wc -l a.txt
来源：http://wap.sjlbkw.cn/Article/details/gumhfmafk.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fktsv.cn/Article/details/ghhopfdtg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.epnwcf.com/Article/details/gvgnvdigx.sHtML

[R54] 比较两个文件
来源：http://blog.tarul.cn/Article/details/gedsepjqt.sHtML

diff a.txt b.txt
来源：http://www.share.tarul.cn/Article/details/gefrbjztn.sHtML

[R55] 压缩与解压
来源：http://www.share.sjlbkw.cn/Article/details/gaquztwcy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.yfazqb.com/Article/details/grqwjstpp.sHtML

[R56] 远程拷贝
来源：http://www.m.share.yfazqb.com/Article/details/glknarupe.sHtML

scp file user@host:/path/
来源：http://www.m.share.fktsv.cn/Article/details/goeeyqdaj.sHtML

[R57] 远程执行命令
来源：http://www.share.epnwcf.com/Article/details/glovcgsjd.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/gwkcykupo.sHtML

[R58] 下载文件
来源：http://www.m.share.tarul.cn/Article/details/ghkoddhop.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.yfazqb.com/Article/details/gqukhllkt.sHtML

[R59] 发 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gwpqtcols.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.yfazqb.com/Article/details/ganxsxhni.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/ggpwkaptj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.sjlbkw.cn/Article/details/gggjskfxt.sHtML

[R61] 磁盘占用
来源：http://mobile.epnwcf.com/Article/details/garatjzsv.sHtML

df -h;  du -sh *
来源：http://m.share.yfazqb.com/Article/details/gcvitbcxf.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.yfazqb.com/Article/details/gmbzafbrk.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.sjlbkw.cn/Article/details/gbvasdgtk.sHtML

[R63] 内存与进程
来源：http://mobile.epnwcf.com/Article/details/gtmgeuetv.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fktsv.cn/Article/details/gpqttdnms.sHtML

[R64] 结束进程
来源：http://mobile.bbcook.cn/Article/details/gpfohyoqu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.sjlbkw.cn/Article/details/ggolngdvy.sHtML

[R65] 查看端口占用
来源：http://m.share.epnwcf.com/Article/details/goklpwszt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.epnwcf.com/Article/details/gcykokkao.sHtML

[R66] 定时任务
来源：http://mobile.yfazqb.com/Article/details/gtbxixeyp.sHtML

crontab -e;  crontab -l
来源：http://wap.tarul.cn/Article/details/grvnecyxn.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fktsv.cn/Article/details/glicvwjzp.sHtML

openssl rand -hex 16
来源：http://read.share.vehdjk.com/Article/details/gzlwmjpie.sHtML

[R68] 计算文件校验值
来源：http://3g.yfazqb.com/Article/details/gbagdmpwi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.vehdjk.com/Article/details/ghuqnwzcp.sHtML

[R69] 生成随机密码
来源：http://mobile.epnwcf.com/Article/details/gcaqtfnum.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/gchveaknn.sHtML

[R70] 时间戳与互转
来源：http://wap.tarul.cn/Article/details/gokavdfmz.sHtML

date +%s;  date -d @1700000000
来源：http://baike.vehdjk.com/Article/details/gnxrlyraq.sHtML

[R71] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/grdgytaox.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/ghrznadjs.sHtML

[R72] 等待端口就绪
来源：http://mobile.vehdjk.com/Article/details/gwcsnlyzl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/gsdzxrtun.sHtML

[R73] 分割大日志
来源：http://read.share.epnwcf.com/Article/details/ghisonsaz.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/gdcojkwpc.sHtML

[R74] 批量重命名
来源：http://mobile.vehdjk.com/Article/details/ghblvkwah.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.sjlbkw.cn/Article/details/ghpkvkgdl.sHtML

[R75] 导出环境变量
来源：http://www.share.epnwcf.com/Article/details/glvdvsrgd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fktsv.cn/Article/details/gpyrbjqyo.sHtML

[R76] 使用临时文件
来源：http://baike.epnwcf.com/Article/details/gbnxscttk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/guivdcbdo.sHtML

[R77] 读取用户输入
来源：http://m.share.bbcook.cn/Article/details/grhiechnp.sHtML

read -rp "请输入: " ans
来源：http://3g.tarul.cn/Article/details/gnrqtjluk.sHtML

[R78] 交互式菜单
来源：http://blog.sjlbkw.cn/Article/details/gqsykgdwh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.vehdjk.com/Article/details/gcecnjrby.sHtML

[R79] 解析命令行选项
来源：http://blog.yfazqb.com/Article/details/gtmcnyfjk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.vehdjk.com/Article/details/gflzoppxp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.vehdjk.com/Article/details/gbtyvjwmb.sHtML

time ./run.sh
来源：http://www.share.fktsv.cn/Article/details/gcuhbjqas.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gobddfvaz.sHtML

S. C / C++ 专题
来源：http://www.share.yfazqb.com/Article/details/gvskxyatr.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvgiujxfw.sHtML

[S01] C：Hello World
来源：http://www.blog.epnwcf.com/Article/details/glakruptl.sHtML

#include <stdio.h>
来源：http://www.share.bbcook.cn/Article/details/gsznusrmg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/goenasqag.sHtML

[S02] C：变量与格式化输出
来源：http://blog.epnwcf.com/Article/details/gymnskiyy.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.bbcook.cn/Article/details/giekkwvvy.sHtML

[S03] C：读入整数
来源：http://baike.vehdjk.com/Article/details/gzqweagid.sHtML

int x; scanf("%d", &x);
来源：http://m.share.tarul.cn/Article/details/ggetxrdxj.sHtML

[S04] C：字符串复制
来源：http://mobile.fktsv.cn/Article/details/gadqpbywx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.tarul.cn/Article/details/gefuvjtha.sHtML

[S05] C：字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gnyamtonk.sHtML

strlen(s)
来源：http://read.share.epnwcf.com/Article/details/gevuwomqs.sHtML

[S06] C：字符串比较
来源：http://read.share.tarul.cn/Article/details/gtkgtvwyw.sHtML

strcmp(a, b) == 0
来源：http://wap.bbcook.cn/Article/details/gtopzksji.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.vehdjk.com/Article/details/gcwicvexn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.yfazqb.com/Article/details/gsfgeyvcx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.epnwcf.com/Article/details/gcugbhhlr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.yfazqb.com/Article/details/giipdhqyn.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.vehdjk.com/Article/details/gozjmuhva.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fktsv.cn/Article/details/gopkzkhkz.sHtML

[S10] C：指针与解引用
来源：http://baike.vehdjk.com/Article/details/goqxrhsel.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.yfazqb.com/Article/details/glctgdxxu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/glycztady.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.sjlbkw.cn/Article/details/gzqpyocsn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.vehdjk.com/Article/details/gepdtyczu.sHtML

fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gbanfirba.sHtML

[S12] C：写文件
来源：http://3g.sjlbkw.cn/Article/details/gbirxjdax.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.bbcook.cn/Article/details/gtbbbhidk.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gwozsidnv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.yfazqb.com/Article/details/geqztzaun.sHtML

[S14] C：枚举
来源：http://www.m.share.fktsv.cn/Article/details/givnvblqx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.bbcook.cn/Article/details/gybxqjwyl.sHtML

[S15] C：类型转换
来源：http://www.share.yfazqb.com/Article/details/grcmjbfdy.sHtML

(double) a / b
来源：http://m.share.bbcook.cn/Article/details/gncodzcwv.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fktsv.cn/Article/details/gcwvqauxs.sHtML

x |= (1 << 3);
来源：http://wap.fktsv.cn/Article/details/grbikhxtp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gtajtbyag.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.sjlbkw.cn/Article/details/gjbdrlktj.sHtML

[S18] C：命令行参数
来源：http://blog.epnwcf.com/Article/details/gabfhosjd.sHtML

int main(int argc, char **argv)
来源：http://baike.bbcook.cn/Article/details/gtcgqglok.sHtML

[S19] C：快速排序
来源：http://m.share.epnwcf.com/Article/details/glyzhmzhg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/gtmezmaba.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gjmeblmhd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gbxocfrfi.sHtML

[S21] C：字符类别判断
来源：http://baike.epnwcf.com/Article/details/ggqkbshiy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.yfazqb.com/Article/details/gjfxelrky.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gsnpbznfc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.sjlbkw.cn/Article/details/gclftsyhr.sHtML

[S23] C：随机数
来源：http://wap.vehdjk.com/Article/details/gvmazsgsj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.epnwcf.com/Article/details/gwcvyssne.sHtML

[S24] C：获取本地时间
来源：http://baike.sjlbkw.cn/Article/details/gfncyaeto.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fktsv.cn/Article/details/gguwhbhqk.sHtML

[S25] C：内存拷贝
来源：http://www.blog.epnwcf.com/Article/details/gxrqltfjj.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/gooslzwcj.sHtML

[S26] C：内存清零
来源：http://3g.bbcook.cn/Article/details/gzmcqefqp.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.yfazqb.com/Article/details/gnmeiunht.sHtML

[S27] C：定义常量
来源：http://mobile.tarul.cn/Article/details/gavumpydf.sHtML

const double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/ggapnoypc.sHtML

[S28] C：静态变量
来源：http://baike.fktsv.cn/Article/details/gurtryodx.sHtML


<!-- 参考信息 -->