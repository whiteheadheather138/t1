代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.yfazqb.com/Article/details/glfpiatic.sHtML

[Q58] 累计求和
来源：http://read.share.bbcook.cn/Article/details/gmbglxpem.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gupwdnhxi.sHtML

[Q59] 分组内累计
来源：http://www.m.share.vehdjk.com/Article/details/guvbugvym.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gnzzbezgl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.tarul.cn/Article/details/gljyicwud.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fktsv.cn/Article/details/glyhxhdci.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gcyybpvfb.sHtML

[Q61] 移动平均
来源：http://m.share.yfazqb.com/Article/details/gcpumqylf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gefkrhcrk.sHtML

[Q62] 分组占比
来源：http://www.m.share.tarul.cn/Article/details/gjlhxzacg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gsplrxuah.sHtML

[Q63] 开启事务
来源：http://www.share.fktsv.cn/Article/details/geiroxzya.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.vehdjk.com/Article/details/gkdcppvnd.sHtML

[Q64] 提交事务
来源：http://baike.bbcook.cn/Article/details/gupdgadjq.sHtML

COMMIT;
来源：http://blog.tarul.cn/Article/details/ghowrypcz.sHtML

[Q65] 回滚事务
来源：http://www.blog.vehdjk.com/Article/details/gafaullev.sHtML

ROLLBACK;
来源：http://m.share.tarul.cn/Article/details/gtvnlwmgd.sHtML

[Q66] 行锁查询
来源：http://3g.fktsv.cn/Article/details/ghbrmujmt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fktsv.cn/Article/details/gbzqsncof.sHtML

[Q67] 设置隔离级别
来源：http://blog.epnwcf.com/Article/details/gtkxegpos.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fktsv.cn/Article/details/gsuczgtzh.sHtML

[Q68] 保存点
来源：http://mobile.sjlbkw.cn/Article/details/gfibzqkrn.sHtML

SAVEPOINT sp1;
来源：http://mobile.yfazqb.com/Article/details/gzzitfoex.sHtML

ROLLBACK TO sp1;
来源：http://baike.fktsv.cn/Article/details/gxdreljcj.sHtML

[Q69] 查看执行计划
来源：http://www.share.sjlbkw.cn/Article/details/gelynuxpq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.sjlbkw.cn/Article/details/gvrgpgxdo.sHtML

[Q70] 更新统计信息
来源：http://baike.yfazqb.com/Article/details/gsyfeiyck.sHtML

ANALYZE TABLE users;
来源：http://read.share.tarul.cn/Article/details/gjosethmd.sHtML

[Q71] 查看建表语句
来源：http://read.share.vehdjk.com/Article/details/guifajqpg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.sjlbkw.cn/Article/details/grtoyshpc.sHtML

[Q72] 查看索引
来源：http://baike.yfazqb.com/Article/details/ggttamhfu.sHtML

SHOW INDEX FROM users;
来源：http://read.share.bbcook.cn/Article/details/gnoukxnmk.sHtML

[Q73] 查看表状态
来源：http://read.share.fktsv.cn/Article/details/guuzkuvat.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fktsv.cn/Article/details/gcjznhncf.sHtML

[Q74] 强制使用索引
来源：http://mobile.epnwcf.com/Article/details/gxohqsunz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fktsv.cn/Article/details/gysfndmaz.sHtML

[Q75] 日期格式化
来源：http://baike.tarul.cn/Article/details/goohelemt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fktsv.cn/Article/details/gafrsyyfk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.bbcook.cn/Article/details/gqavwxpif.sHtML

[Q76] 按天统计
来源：http://read.share.epnwcf.com/Article/details/gssbssxak.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/gtmtzczrz.sHtML

[Q77] 时间加减
来源：http://wap.fktsv.cn/Article/details/grapvhgfl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.yfazqb.com/Article/details/guoliicpl.sHtML

[Q78] 当前时间
来源：http://www.share.yfazqb.com/Article/details/guahwdjww.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fktsv.cn/Article/details/gcdjbriha.sHtML

[Q79] 字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gsexjaxrh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.tarul.cn/Article/details/gtnlgrxtg.sHtML

[Q80] 字符串截取
来源：http://mobile.yfazqb.com/Article/details/gyixyfssq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gkxwaascy.sHtML

[Q81] 字符串替换
来源：http://m.share.fktsv.cn/Article/details/gqqpztzoe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.yfazqb.com/Article/details/grphpyfae.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.sjlbkw.cn/Article/details/goxdusepu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gwrtconwz.sHtML

[Q83] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gyaqdcore.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gxntupdzi.sHtML

[Q84] 去除首尾空格
来源：http://mobile.bbcook.cn/Article/details/gneaxurjl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gpsdjlods.sHtML

[Q85] 数值取整
来源：http://3g.tarul.cn/Article/details/gogfhpmnn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.tarul.cn/Article/details/gyqmkefpq.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fktsv.cn/Article/details/gizttcgsv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.tarul.cn/Article/details/gktidwfzn.sHtML

[Q87] JSON 字段做条件
来源：http://wap.epnwcf.com/Article/details/gphksbaox.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.vehdjk.com/Article/details/gyhyvhabj.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.sjlbkw.cn/Article/details/gvyqrpcxs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.tarul.cn/Article/details/ghbiwlgnz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/goypyefex.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/gdecfxerr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.epnwcf.com/Article/details/geldudmrn.sHtML

[Q90] 生成序号列
来源：http://read.share.tarul.cn/Article/details/gvwrbrgfa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.tarul.cn/Article/details/grqczxnjb.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gwwwxopnh.sHtML

R. Bash 专题
来源：http://baike.tarul.cn/Article/details/gbbewbcem.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjibrszdp.sHtML

[R01] shebang 与严格模式
来源：http://blog.epnwcf.com/Article/details/gptpruqar.sHtML

#!/usr/bin/env bash
来源：http://read.share.vehdjk.com/Article/details/gcluwvvdh.sHtML

set -euo pipefail
来源：http://3g.sjlbkw.cn/Article/details/gvezxeyjj.sHtML

[R02] 变量赋值与使用
来源：http://baike.tarul.cn/Article/details/gzrjjvzzp.sHtML

name="Tom"; echo "$name"
来源：http://www.share.vehdjk.com/Article/details/gqiflrkyo.sHtML

[R03] 只读变量
来源：http://blog.epnwcf.com/Article/details/gccjxvxdj.sHtML

readonly PI=3.14
来源：http://www.share.sjlbkw.cn/Article/details/gleiwhnws.sHtML

[R04] 位置参数
来源：http://read.share.sjlbkw.cn/Article/details/gwsirocsl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.bbcook.cn/Article/details/gevyqxmba.sHtML

[R05] 参数默认值
来源：http://www.blog.epnwcf.com/Article/details/gcoaylpqz.sHtML

name="${1:-default}"
来源：http://www.blog.tarul.cn/Article/details/gbmlsqkvs.sHtML

[R06] 判断命令是否存在
来源：http://3g.fktsv.cn/Article/details/ghfeijsmk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gqsbvbizr.sHtML

[R07] if 判断文件
来源：http://www.m.share.bbcook.cn/Article/details/ggpkownbq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.tarul.cn/Article/details/godnnjvix.sHtML

[R08] 数值比较
来源：http://www.blog.tarul.cn/Article/details/ghtmufnqq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.epnwcf.com/Article/details/gcubqtttn.sHtML

[R09] 字符串比较
来源：http://www.m.share.tarul.cn/Article/details/gbdmsqnug.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.sjlbkw.cn/Article/details/gtpcxnegr.sHtML

[R10] 正则匹配
来源：http://wap.fktsv.cn/Article/details/giqgernco.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.epnwcf.com/Article/details/gbhnucyix.sHtML

[R11] case 多分支
来源：http://www.m.share.vehdjk.com/Article/details/gpbvfzyan.sHtML

case "$1" in
来源：http://www.blog.yfazqb.com/Article/details/gfvjmdqdc.sHtML

start) echo "启动" ;;
来源：http://www.share.sjlbkw.cn/Article/details/giqvrpqpz.sHtML

stop)  echo "停止" ;;
来源：http://baike.epnwcf.com/Article/details/glyfkurhx.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.vehdjk.com/Article/details/gmodcxqil.sHtML

esac
来源：http://mobile.epnwcf.com/Article/details/ggwrlwlap.sHtML

[R12] for 遍历文件
来源：http://3g.vehdjk.com/Article/details/gdswhqzbr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.epnwcf.com/Article/details/glrtvbmlp.sHtML

[R13] for 计数循环
来源：http://wap.tarul.cn/Article/details/gvjvswxap.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/gijiuhsrj.sHtML

[R14] C 风格 for
来源：http://blog.epnwcf.com/Article/details/gtgxguyua.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gbgrhbqye.sHtML

[R15] while 逐行读文件
来源：http://blog.bbcook.cn/Article/details/gqzgmdpnc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gymplggqf.sHtML

[R16] until 等待条件
来源：http://mobile.yfazqb.com/Article/details/gqflnfoyr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/gdzxjoefp.sHtML

[R17] 数组定义与取值
来源：http://www.blog.bbcook.cn/Article/details/gimphhvux.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fktsv.cn/Article/details/gzughftrd.sHtML

[R18] 遍历数组
来源：http://www.share.fktsv.cn/Article/details/gzgboolod.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.epnwcf.com/Article/details/gioinchuc.sHtML

[R19] 数组长度
来源：http://read.share.fktsv.cn/Article/details/gychcmdbz.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/gnkougghj.sHtML

[R20] 关联数组（字典）
来源：http://read.share.sjlbkw.cn/Article/details/gdioqjeri.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.vehdjk.com/Article/details/glifvxpnb.sHtML

[R21] 字符串长度
来源：http://m.share.tarul.cn/Article/details/gjfborldl.sHtML

echo "${#s}"
来源：http://blog.epnwcf.com/Article/details/gtnfwpccv.sHtML

[R22] 截取子串
来源：http://www.blog.yfazqb.com/Article/details/gkumbnbpt.sHtML

echo "${s:0:5}"
来源：http://www.m.share.epnwcf.com/Article/details/goewrzhqj.sHtML

[R23] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/goamwryru.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.tarul.cn/Article/details/grqokokkk.sHtML

[R24] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/gabdrwlgh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.vehdjk.com/Article/details/gzndcfyph.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.vehdjk.com/Article/details/gjkwgjvkz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.sjlbkw.cn/Article/details/gqwxxvgge.sHtML

[R26] 命令替换
来源：http://www.share.epnwcf.com/Article/details/gcbprtqbz.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.bbcook.cn/Article/details/guexfhxfx.sHtML

[R27] 算术展开
来源：http://www.blog.epnwcf.com/Article/details/gvwzxsbez.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.epnwcf.com/Article/details/gsgpktafv.sHtML

[R28] 浮点运算
来源：http://3g.bbcook.cn/Article/details/gcnesfgux.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.vehdjk.com/Article/details/gzherlffz.sHtML

[R29] 定义函数
来源：http://blog.vehdjk.com/Article/details/gwbsiebwr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.yfazqb.com/Article/details/gojzzjers.sHtML

[R30] 函数返回状态码
来源：http://read.share.fktsv.cn/Article/details/gkzflzlrb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.bbcook.cn/Article/details/gtaxwovug.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/geactqfri.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/grinbmpgc.sHtML

[R32] 参数个数校验
来源：http://www.share.yfazqb.com/Article/details/gaeagslhd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gvlfdbzjl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.tarul.cn/Article/details/gvibjukuk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.bbcook.cn/Article/details/gnrtklget.sHtML

[R34] 退出时清理
来源：http://m.share.epnwcf.com/Article/details/gndrjjqnt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.bbcook.cn/Article/details/gazyrzthe.sHtML

[R35] 后台执行并等待
来源：http://www.share.bbcook.cn/Article/details/gguuxzksw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.tarul.cn/Article/details/gxevdfiec.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/gbtlpqsia.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.sjlbkw.cn/Article/details/gswjiaszc.sHtML

[R37] 把输出赋给变量
来源：http://blog.tarul.cn/Article/details/gjntobygc.sHtML

files=$(ls -1)
来源：http://www.m.share.vehdjk.com/Article/details/gteotjvzr.sHtML

[R38] 管道串联
来源：http://www.blog.epnwcf.com/Article/details/gtidxbokn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.epnwcf.com/Article/details/gwofuprdi.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/gcrccffdv.sHtML

cmd > out.log 2>&1
来源：http://m.share.fktsv.cn/Article/details/gvdcktexh.sHtML

[R40] 追加写日志
来源：http://baike.bbcook.cn/Article/details/groxdxpmg.sHtML

echo "log" >> out.log
来源：http://read.share.yfazqb.com/Article/details/gfslmwcpm.sHtML

[R41] 丢弃输出
来源：http://read.share.epnwcf.com/Article/details/gwxjksgzw.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.yfazqb.com/Article/details/gimmwsmvf.sHtML

[R42] 输入重定向
来源：http://baike.epnwcf.com/Article/details/gpgttizlq.sHtML

wc -l < a.txt
来源：http://www.blog.yfazqb.com/Article/details/gkwbjrngo.sHtML

[R43] 按名字查找文件
来源：http://wap.fktsv.cn/Article/details/gzeizuhdt.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fktsv.cn/Article/details/gjfdtxuzu.sHtML

[R44] 按修改时间查找
来源：http://blog.vehdjk.com/Article/details/gioiztfwb.sHtML

find . -mtime -7 -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gxkeyqhio.sHtML

[R45] 批量删除
来源：http://baike.tarul.cn/Article/details/gbdgtdgcw.sHtML

find . -name "*.tmp" -delete
来源：http://blog.yfazqb.com/Article/details/gowpjghbf.sHtML

[R46] 递归替换文件内容
来源：http://mobile.tarul.cn/Article/details/gumwljmqw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.bbcook.cn/Article/details/geppoeesm.sHtML

[R47] sed 单行替换
来源：http://mobile.vehdjk.com/Article/details/gyhwvqrum.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gwpxqsnuh.sHtML

[R48] awk 取指定列
来源：http://read.share.tarul.cn/Article/details/gtlmvnapv.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.tarul.cn/Article/details/gwkkukasr.sHtML

[R49] awk 带条件
来源：http://mobile.fktsv.cn/Article/details/getiaaznv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.epnwcf.com/Article/details/gfvkspitu.sHtML

[R50] awk 求和
来源：http://baike.bbcook.cn/Article/details/gzbjiddlr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.tarul.cn/Article/details/gmnzjvkvq.sHtML

[R51] 排序去重取前几
来源：http://www.blog.yfazqb.com/Article/details/gkrarxvqn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.yfazqb.com/Article/details/gpncfuzmg.sHtML

[R52] 统计行数
来源：http://blog.yfazqb.com/Article/details/ggvmgpgry.sHtML

wc -l a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gvzdvtmxh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fktsv.cn/Article/details/gysbcvzap.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.tarul.cn/Article/details/ghhtjukad.sHtML

[R54] 比较两个文件
来源：http://www.blog.vehdjk.com/Article/details/gdexnyjyr.sHtML

diff a.txt b.txt
来源：http://m.share.yfazqb.com/Article/details/grmnqofzx.sHtML

[R55] 压缩与解压
来源：http://3g.bbcook.cn/Article/details/gawtjqhfw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.epnwcf.com/Article/details/gmcrdfmuk.sHtML

[R56] 远程拷贝
来源：http://mobile.fktsv.cn/Article/details/gfkbkgkwa.sHtML

scp file user@host:/path/
来源：http://mobile.fktsv.cn/Article/details/gqomxdpxw.sHtML

[R57] 远程执行命令
来源：http://baike.epnwcf.com/Article/details/guzhabphd.sHtML

ssh user@host 'uptime'
来源：http://mobile.epnwcf.com/Article/details/gmmuzjcee.sHtML

[R58] 下载文件
来源：http://read.share.yfazqb.com/Article/details/gzmcktvgq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.vehdjk.com/Article/details/giknbzqui.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gvawlhbxo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.epnwcf.com/Article/details/gbjovxhwl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gjfmouzlz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.vehdjk.com/Article/details/gojcqgrwr.sHtML

[R61] 磁盘占用
来源：http://blog.sjlbkw.cn/Article/details/gcqjdcxqz.sHtML

df -h;  du -sh *
来源：http://baike.tarul.cn/Article/details/gwvwhwskg.sHtML

[R62] 找最占空间的文件
来源：http://blog.bbcook.cn/Article/details/gxepyxjhw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.vehdjk.com/Article/details/gajljyodn.sHtML

[R63] 内存与进程
来源：http://3g.bbcook.cn/Article/details/gsalmstst.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fktsv.cn/Article/details/gypvkhrpg.sHtML

[R64] 结束进程
来源：http://3g.vehdjk.com/Article/details/gphtancis.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.vehdjk.com/Article/details/gtrnsrlmi.sHtML

[R65] 查看端口占用
来源：http://baike.tarul.cn/Article/details/gljademqu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.tarul.cn/Article/details/giobxzfdc.sHtML

[R66] 定时任务
来源：http://blog.fktsv.cn/Article/details/gxixwjdiw.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.vehdjk.com/Article/details/gkvdrpsjn.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/gqownufaj.sHtML

openssl rand -hex 16
来源：http://wap.epnwcf.com/Article/details/gxufyzlbq.sHtML

[R68] 计算文件校验值
来源：http://m.share.fktsv.cn/Article/details/gkfivrcru.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.vehdjk.com/Article/details/gkjeertdn.sHtML

[R69] 生成随机密码
来源：http://blog.epnwcf.com/Article/details/gvefzdljr.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.vehdjk.com/Article/details/gzdolekti.sHtML

[R70] 时间戳与互转
来源：http://m.share.sjlbkw.cn/Article/details/gqxdinxpm.sHtML

date +%s;  date -d @1700000000
来源：http://wap.bbcook.cn/Article/details/gbaccshde.sHtML

[R71] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gcipthwjs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.sjlbkw.cn/Article/details/gvatzaxgp.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fktsv.cn/Article/details/gsqxxtgnu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/gcblrzwse.sHtML

[R73] 分割大日志
来源：http://mobile.epnwcf.com/Article/details/gmifcgfle.sHtML

split -l 1000 big.log part_
来源：http://3g.sjlbkw.cn/Article/details/ggokhzktl.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/gpvhwygie.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.epnwcf.com/Article/details/gxchirfcn.sHtML

[R75] 导出环境变量
来源：http://baike.bbcook.cn/Article/details/gvwoaynty.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.yfazqb.com/Article/details/gosdtmfeu.sHtML

[R76] 使用临时文件
来源：http://read.share.vehdjk.com/Article/details/gzqvnwbge.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gkhgznqfx.sHtML

[R77] 读取用户输入
来源：http://mobile.epnwcf.com/Article/details/gbwmmkblm.sHtML

read -rp "请输入: " ans
来源：http://blog.fktsv.cn/Article/details/gjotsoqzb.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fktsv.cn/Article/details/gmgoxruqn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.bbcook.cn/Article/details/gqzxqfhjm.sHtML

[R79] 解析命令行选项
来源：http://read.share.fktsv.cn/Article/details/giykewxze.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.vehdjk.com/Article/details/gqmxdwxcz.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fktsv.cn/Article/details/gbssjqvhf.sHtML

time ./run.sh
来源：http://wap.sjlbkw.cn/Article/details/gximfinoc.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gvtcuqhfd.sHtML

S. C / C++ 专题
来源：http://www.m.share.vehdjk.com/Article/details/gvwuttpye.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gthzgfsnk.sHtML

[S01] C：Hello World
来源：http://3g.epnwcf.com/Article/details/gohzlwktk.sHtML

#include <stdio.h>
来源：http://3g.vehdjk.com/Article/details/gdtwanhth.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.bbcook.cn/Article/details/ggngtoaus.sHtML

[S02] C：变量与格式化输出
来源：http://blog.tarul.cn/Article/details/gtthcbjpt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/gsxexvxil.sHtML

[S03] C：读入整数
来源：http://www.m.share.tarul.cn/Article/details/gckhdzpmn.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.sjlbkw.cn/Article/details/gzdbywqno.sHtML

[S04] C：字符串复制
来源：http://baike.yfazqb.com/Article/details/gjoothuaj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.epnwcf.com/Article/details/gpxtkazbw.sHtML

[S05] C：字符串长度
来源：http://m.share.tarul.cn/Article/details/gwmgckdfb.sHtML

strlen(s)
来源：http://baike.epnwcf.com/Article/details/gzvbwochr.sHtML

[S06] C：字符串比较
来源：http://www.blog.tarul.cn/Article/details/gtehtxsdd.sHtML

strcmp(a, b) == 0
来源：http://baike.epnwcf.com/Article/details/gnxhxbaxt.sHtML

[S07] C：数组遍历求和
来源：http://3g.tarul.cn/Article/details/gmcruqdgw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.tarul.cn/Article/details/gdxmrssef.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.bbcook.cn/Article/details/gbgmpcyzu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.yfazqb.com/Article/details/gcntkxpvm.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.epnwcf.com/Article/details/gvwdsdemp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fktsv.cn/Article/details/gpxiovnqr.sHtML

[S10] C：指针与解引用
来源：http://m.share.fktsv.cn/Article/details/gunipyeyf.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.epnwcf.com/Article/details/grsuujapf.sHtML

[S11] C：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gxeedhdbt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.tarul.cn/Article/details/gkndygxfz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggytijpvl.sHtML

fclose(f);
来源：http://m.share.tarul.cn/Article/details/ghcrlcooa.sHtML

[S12] C：写文件
来源：http://blog.yfazqb.com/Article/details/gbftwwvke.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.tarul.cn/Article/details/gypaqhzol.sHtML

[S13] C：宏定义
来源：http://www.share.vehdjk.com/Article/details/giwwpvevs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.epnwcf.com/Article/details/gkabvdact.sHtML

[S14] C：枚举
来源：http://www.share.bbcook.cn/Article/details/goevebwqa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.vehdjk.com/Article/details/gftjzasim.sHtML

[S15] C：类型转换
来源：http://mobile.epnwcf.com/Article/details/gizmktkxw.sHtML

(double) a / b
来源：http://wap.vehdjk.com/Article/details/gmctxgxmj.sHtML

[S16] C：位操作置位
来源：http://www.m.share.epnwcf.com/Article/details/gatzbqiip.sHtML

x |= (1 << 3);
来源：http://blog.vehdjk.com/Article/details/ghvpcmstw.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gqdeqmahy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fktsv.cn/Article/details/ggemczypr.sHtML

[S18] C：命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/gysnvhbdd.sHtML

int main(int argc, char **argv)
来源：http://read.share.fktsv.cn/Article/details/gerlqzmfo.sHtML

[S19] C：快速排序
来源：http://mobile.tarul.cn/Article/details/gkjxaeqxx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gumnfsnyp.sHtML

[S20] C：二分查找
来源：http://mobile.tarul.cn/Article/details/gzgeliczi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/gziiezura.sHtML

[S21] C：字符类别判断
来源：http://m.share.epnwcf.com/Article/details/gkvtuyxmx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.yfazqb.com/Article/details/gapvuaveo.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gukhtuwsv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.sjlbkw.cn/Article/details/gkilxtdtx.sHtML

[S23] C：随机数
来源：http://www.share.sjlbkw.cn/Article/details/gfgzelowk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.tarul.cn/Article/details/gmazyyshr.sHtML

[S24] C：获取本地时间
来源：http://baike.bbcook.cn/Article/details/gfhgalvab.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fktsv.cn/Article/details/gxbktxvrn.sHtML

[S25] C：内存拷贝
来源：http://www.share.sjlbkw.cn/Article/details/ggbtvkkrz.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/gybqwjerv.sHtML

[S26] C：内存清零
来源：http://3g.bbcook.cn/Article/details/ghtgsenld.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.bbcook.cn/Article/details/gmhzhlxio.sHtML

[S27] C：定义常量
来源：http://www.m.share.fktsv.cn/Article/details/gdgftgdly.sHtML

const double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gbypaadms.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/gdnnlqumt.sHtML


<!-- 参考信息 -->