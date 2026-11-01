代发 wailian999

SHOW INDEX FROM users;
来源：http://wap.vehdjk.com/Article/details/ghhbnezbn.sHtML

[Q73] 查看表状态
来源：http://3g.fktsv.cn/Article/details/gmgyjbczt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.epnwcf.com/Article/details/glclkeosb.sHtML

[Q74] 强制使用索引
来源：http://3g.vehdjk.com/Article/details/gulgfbpiv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.vehdjk.com/Article/details/gjvypxfrn.sHtML

[Q75] 日期格式化
来源：http://baike.fktsv.cn/Article/details/guzddjvjb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.vehdjk.com/Article/details/ggdycmlzm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.yfazqb.com/Article/details/giurlinpf.sHtML

[Q76] 按天统计
来源：http://mobile.sjlbkw.cn/Article/details/gzgvxtsqe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.tarul.cn/Article/details/gplxexriu.sHtML

[Q77] 时间加减
来源：http://www.share.fktsv.cn/Article/details/gyldpiang.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.bbcook.cn/Article/details/gxrqwyrye.sHtML

[Q78] 当前时间
来源：http://mobile.tarul.cn/Article/details/gzrnuholp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fktsv.cn/Article/details/gxiwjhvnh.sHtML

[Q79] 字符串拼接
来源：http://m.share.tarul.cn/Article/details/gmbpredzb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.epnwcf.com/Article/details/giswzdima.sHtML

[Q80] 字符串截取
来源：http://www.m.share.sjlbkw.cn/Article/details/gxylfoilo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gpygmtcwo.sHtML

[Q81] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/gquixzeip.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.bbcook.cn/Article/details/gtmmgehow.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.vehdjk.com/Article/details/gobmsmewr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/ghzabutgo.sHtML

[Q83] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gugkpkkwx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/grrnpiyvc.sHtML

[Q84] 去除首尾空格
来源：http://mobile.tarul.cn/Article/details/gkjcvypas.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gczsmxfhs.sHtML

[Q85] 数值取整
来源：http://baike.sjlbkw.cn/Article/details/gdhlohcqn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.tarul.cn/Article/details/gooniwbar.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fktsv.cn/Article/details/gxrfhcndm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.yfazqb.com/Article/details/gixntdiue.sHtML

[Q87] JSON 字段做条件
来源：http://wap.sjlbkw.cn/Article/details/gfmffvoif.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.bbcook.cn/Article/details/gcslinhnl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.vehdjk.com/Article/details/gabbhyynz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fktsv.cn/Article/details/ghkpmcynu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.epnwcf.com/Article/details/gnrqafouj.sHtML

[Q89] 判断表是否存在
来源：http://baike.yfazqb.com/Article/details/gziiriikm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.bbcook.cn/Article/details/gpcfigntq.sHtML

[Q90] 生成序号列
来源：http://wap.epnwcf.com/Article/details/googxhvlz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.tarul.cn/Article/details/gtrpuuhzy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gkfajtdlt.sHtML

R. Bash 专题
来源：http://baike.bbcook.cn/Article/details/gupugjjno.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ggckzjtxl.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.vehdjk.com/Article/details/gbtjvzddi.sHtML

#!/usr/bin/env bash
来源：http://mobile.sjlbkw.cn/Article/details/gefpevzxh.sHtML

set -euo pipefail
来源：http://baike.yfazqb.com/Article/details/ghlqfimwg.sHtML

[R02] 变量赋值与使用
来源：http://mobile.sjlbkw.cn/Article/details/gtxnssyht.sHtML

name="Tom"; echo "$name"
来源：http://mobile.yfazqb.com/Article/details/gxulqwdjd.sHtML

[R03] 只读变量
来源：http://mobile.tarul.cn/Article/details/gmlxtnemb.sHtML

readonly PI=3.14
来源：http://3g.tarul.cn/Article/details/gffyxwhgb.sHtML

[R04] 位置参数
来源：http://www.share.tarul.cn/Article/details/gtreptyoi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fktsv.cn/Article/details/gkabjiqct.sHtML

[R05] 参数默认值
来源：http://www.share.yfazqb.com/Article/details/geymqekvv.sHtML

name="${1:-default}"
来源：http://wap.fktsv.cn/Article/details/ghvbosnel.sHtML

[R06] 判断命令是否存在
来源：http://blog.tarul.cn/Article/details/gpryjecqw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gqemwcfkc.sHtML

[R07] if 判断文件
来源：http://www.m.share.tarul.cn/Article/details/gvykzgcty.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.bbcook.cn/Article/details/gysdbryqk.sHtML

[R08] 数值比较
来源：http://mobile.sjlbkw.cn/Article/details/gjfujtdik.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gzowuwxay.sHtML

[R09] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gviojorpq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gogqiglnw.sHtML

[R10] 正则匹配
来源：http://www.blog.vehdjk.com/Article/details/gdpeshdmy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.epnwcf.com/Article/details/gubxshwur.sHtML

[R11] case 多分支
来源：http://www.blog.yfazqb.com/Article/details/gzuykihov.sHtML

case "$1" in
来源：http://3g.tarul.cn/Article/details/gwsnpxore.sHtML

start) echo "启动" ;;
来源：http://blog.tarul.cn/Article/details/gcycssrdo.sHtML

stop)  echo "停止" ;;
来源：http://wap.tarul.cn/Article/details/gqirvlllh.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gabaqtitd.sHtML

esac
来源：http://mobile.bbcook.cn/Article/details/gjdzcvkbi.sHtML

[R12] for 遍历文件
来源：http://read.share.yfazqb.com/Article/details/gncmeiged.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fktsv.cn/Article/details/ggvrwhpyw.sHtML

[R13] for 计数循环
来源：http://www.m.share.bbcook.cn/Article/details/goqarfmij.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/gynrzfnjr.sHtML

[R14] C 风格 for
来源：http://m.share.bbcook.cn/Article/details/gcajupsjm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/gunbolexj.sHtML

[R15] while 逐行读文件
来源：http://blog.bbcook.cn/Article/details/gtqqxuaot.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fktsv.cn/Article/details/gyjkprsyq.sHtML

[R16] until 等待条件
来源：http://baike.bbcook.cn/Article/details/ganaczbcd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/givblsezw.sHtML

[R17] 数组定义与取值
来源：http://blog.epnwcf.com/Article/details/gujmsbnop.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fktsv.cn/Article/details/gzchsmxye.sHtML

[R18] 遍历数组
来源：http://www.blog.epnwcf.com/Article/details/gdascnmvu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/gguijmtat.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/gmoztkwox.sHtML

echo "${#arr[@]}"
来源：http://www.share.yfazqb.com/Article/details/gtugtazce.sHtML

[R20] 关联数组（字典）
来源：http://mobile.epnwcf.com/Article/details/gjjxbvnkq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.sjlbkw.cn/Article/details/gelwzrixr.sHtML

[R21] 字符串长度
来源：http://m.share.fktsv.cn/Article/details/gdwetovzw.sHtML

echo "${#s}"
来源：http://m.share.yfazqb.com/Article/details/gpqhrjevx.sHtML

[R22] 截取子串
来源：http://3g.fktsv.cn/Article/details/gkrzntdrh.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/ghunwpkfj.sHtML

[R23] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gdqjnizij.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.vehdjk.com/Article/details/gtiltlzhv.sHtML

[R24] 大小写转换
来源：http://baike.tarul.cn/Article/details/gxhnuqjpu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.vehdjk.com/Article/details/gwidrncuu.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.epnwcf.com/Article/details/gnfuqfhxw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.yfazqb.com/Article/details/gmqyftniu.sHtML

[R26] 命令替换
来源：http://read.share.yfazqb.com/Article/details/ggivmvfxh.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gknizyzxu.sHtML

[R27] 算术展开
来源：http://www.blog.bbcook.cn/Article/details/gkirlhidb.sHtML

echo $((1 + 2 * 3))
来源：http://wap.sjlbkw.cn/Article/details/glsjckgnv.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/gkqboyelu.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/gjzaoogjj.sHtML

[R29] 定义函数
来源：http://www.share.bbcook.cn/Article/details/gnaobhvae.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.sjlbkw.cn/Article/details/gnsvrdfyz.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/gkzqlunub.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.tarul.cn/Article/details/gpgsveaws.sHtML

[R31] 局部变量
来源：http://3g.bbcook.cn/Article/details/gpdfklahi.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.epnwcf.com/Article/details/gtuvyhjtn.sHtML

[R32] 参数个数校验
来源：http://read.share.fktsv.cn/Article/details/gitytrlqw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/gtildixyg.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.sjlbkw.cn/Article/details/gdicyadte.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fktsv.cn/Article/details/gcrsggkfd.sHtML

[R34] 退出时清理
来源：http://wap.tarul.cn/Article/details/gdozwcpvl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.yfazqb.com/Article/details/gpvrkkhhm.sHtML

[R35] 后台执行并等待
来源：http://blog.epnwcf.com/Article/details/gmtntfigt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.bbcook.cn/Article/details/gquxgdkrj.sHtML

[R36] 并发执行多个任务
来源：http://blog.sjlbkw.cn/Article/details/gwsnyasuk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.yfazqb.com/Article/details/gdbazhrgc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.sjlbkw.cn/Article/details/girzusojm.sHtML

files=$(ls -1)
来源：http://read.share.bbcook.cn/Article/details/gkuurxlwx.sHtML

[R38] 管道串联
来源：http://m.share.vehdjk.com/Article/details/grakazxhz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.tarul.cn/Article/details/gxyhfazcc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.vehdjk.com/Article/details/grrohgqlo.sHtML

cmd > out.log 2>&1
来源：http://3g.epnwcf.com/Article/details/ggszfeayd.sHtML

[R40] 追加写日志
来源：http://blog.vehdjk.com/Article/details/gdhexhbfn.sHtML

echo "log" >> out.log
来源：http://www.m.share.fktsv.cn/Article/details/gmwvehtle.sHtML

[R41] 丢弃输出
来源：http://3g.fktsv.cn/Article/details/gpqqfakjm.sHtML

cmd >/dev/null 2>&1
来源：http://3g.yfazqb.com/Article/details/giottgccv.sHtML

[R42] 输入重定向
来源：http://www.share.epnwcf.com/Article/details/gectnzwvu.sHtML

wc -l < a.txt
来源：http://read.share.epnwcf.com/Article/details/gmmegajjn.sHtML

[R43] 按名字查找文件
来源：http://read.share.sjlbkw.cn/Article/details/gzyerwxhy.sHtML

find . -name "*.log" -type f
来源：http://www.share.bbcook.cn/Article/details/gbpgijrzs.sHtML

[R44] 按修改时间查找
来源：http://blog.sjlbkw.cn/Article/details/ghemjysvl.sHtML

find . -mtime -7 -type f
来源：http://read.share.yfazqb.com/Article/details/gnpgiovnv.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/gzccojzfo.sHtML

find . -name "*.tmp" -delete
来源：http://baike.tarul.cn/Article/details/gcqgpwczg.sHtML

[R46] 递归替换文件内容
来源：http://blog.fktsv.cn/Article/details/gysovzsmg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.bbcook.cn/Article/details/gqhwyehzc.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/gwucqhzaf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.bbcook.cn/Article/details/gkbuoxkig.sHtML

[R48] awk 取指定列
来源：http://mobile.fktsv.cn/Article/details/gljawfjqs.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.yfazqb.com/Article/details/giqcucvah.sHtML

[R49] awk 带条件
来源：http://www.m.share.fktsv.cn/Article/details/gkwzawdof.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.vehdjk.com/Article/details/gjlaqormo.sHtML

[R50] awk 求和
来源：http://m.share.bbcook.cn/Article/details/gcsedaigc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gectoqxol.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.epnwcf.com/Article/details/gknblggev.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.bbcook.cn/Article/details/gwrpaszhw.sHtML

[R52] 统计行数
来源：http://baike.tarul.cn/Article/details/gpopeqbzd.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/gdxujeatz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.sjlbkw.cn/Article/details/gnyhszjzk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gozzsabre.sHtML

[R54] 比较两个文件
来源：http://blog.bbcook.cn/Article/details/gdthdrwhc.sHtML

diff a.txt b.txt
来源：http://blog.epnwcf.com/Article/details/gyuhxuolq.sHtML

[R55] 压缩与解压
来源：http://blog.bbcook.cn/Article/details/gqynpplrg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.yfazqb.com/Article/details/gecfwikjz.sHtML

[R56] 远程拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gwzyxqiuv.sHtML

scp file user@host:/path/
来源：http://m.share.yfazqb.com/Article/details/gjjshzytq.sHtML

[R57] 远程执行命令
来源：http://www.share.tarul.cn/Article/details/gkrnasobj.sHtML

ssh user@host 'uptime'
来源：http://blog.yfazqb.com/Article/details/gjgzqheku.sHtML

[R58] 下载文件
来源：http://baike.epnwcf.com/Article/details/gzwopxfyh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.vehdjk.com/Article/details/gekviscbc.sHtML

[R59] 发 POST JSON
来源：http://read.share.bbcook.cn/Article/details/gymwmdltj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.vehdjk.com/Article/details/gzbjbonrr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gbjlknmcc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.yfazqb.com/Article/details/gbppxeudh.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fktsv.cn/Article/details/gnttmxrti.sHtML

df -h;  du -sh *
来源：http://m.share.bbcook.cn/Article/details/ggvmelcnj.sHtML

[R62] 找最占空间的文件
来源：http://wap.vehdjk.com/Article/details/gixojxlkc.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.sjlbkw.cn/Article/details/ggioeffpq.sHtML

[R63] 内存与进程
来源：http://3g.sjlbkw.cn/Article/details/gayvuwcxk.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.vehdjk.com/Article/details/grbavnaqp.sHtML

[R64] 结束进程
来源：http://www.share.epnwcf.com/Article/details/gvsphodnj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.yfazqb.com/Article/details/gesavjyxr.sHtML

[R65] 查看端口占用
来源：http://www.blog.vehdjk.com/Article/details/ggjqferzj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.sjlbkw.cn/Article/details/gbhowhcej.sHtML

[R66] 定时任务
来源：http://3g.yfazqb.com/Article/details/gatkbzgwk.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gboygqelo.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.epnwcf.com/Article/details/geeavjxsm.sHtML

openssl rand -hex 16
来源：http://wap.bbcook.cn/Article/details/gkowevuuv.sHtML

[R68] 计算文件校验值
来源：http://www.share.epnwcf.com/Article/details/gywnxfecj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.tarul.cn/Article/details/gomjvcino.sHtML

[R69] 生成随机密码
来源：http://blog.bbcook.cn/Article/details/gqjrtwito.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.yfazqb.com/Article/details/gayxgmtkr.sHtML

[R70] 时间戳与互转
来源：http://baike.sjlbkw.cn/Article/details/gejfixbxm.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.yfazqb.com/Article/details/gmjcpbops.sHtML

[R71] 日期格式化
来源：http://blog.bbcook.cn/Article/details/gmxatyvxa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.vehdjk.com/Article/details/godcamlmv.sHtML

[R72] 等待端口就绪
来源：http://mobile.sjlbkw.cn/Article/details/ghnkhrhqp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gpbetipzs.sHtML

[R73] 分割大日志
来源：http://mobile.bbcook.cn/Article/details/gmtpwhwbk.sHtML

split -l 1000 big.log part_
来源：http://3g.bbcook.cn/Article/details/gqwxsdcsi.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/grmrhugev.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.tarul.cn/Article/details/gzovxfqwd.sHtML

[R75] 导出环境变量
来源：http://www.share.vehdjk.com/Article/details/gpakfbyyd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.bbcook.cn/Article/details/gmxiaofge.sHtML

[R76] 使用临时文件
来源：http://www.share.tarul.cn/Article/details/grjoezizf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gapdabspa.sHtML

[R77] 读取用户输入
来源：http://www.m.share.epnwcf.com/Article/details/grjeguheo.sHtML

read -rp "请输入: " ans
来源：http://mobile.bbcook.cn/Article/details/gtunrcznv.sHtML

[R78] 交互式菜单
来源：http://baike.tarul.cn/Article/details/gexhnygja.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.sjlbkw.cn/Article/details/gvdurmuhp.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gthbykrfa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.bbcook.cn/Article/details/gxvhwdyij.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.vehdjk.com/Article/details/gkwyyrqtw.sHtML

time ./run.sh
来源：http://blog.yfazqb.com/Article/details/gvipjdzrd.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gnweyxpej.sHtML

S. C / C++ 专题
来源：http://3g.tarul.cn/Article/details/gepuwmbmw.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxwqlwzkl.sHtML

[S01] C：Hello World
来源：http://3g.sjlbkw.cn/Article/details/giafidqcu.sHtML

#include <stdio.h>
来源：http://wap.vehdjk.com/Article/details/gtbtldcba.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.bbcook.cn/Article/details/gfptqlqnl.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.epnwcf.com/Article/details/gkawlngso.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fktsv.cn/Article/details/gehgsfzmc.sHtML

[S03] C：读入整数
来源：http://wap.vehdjk.com/Article/details/gyxddbica.sHtML

int x; scanf("%d", &x);
来源：http://baike.epnwcf.com/Article/details/gohewzztv.sHtML

[S04] C：字符串复制
来源：http://www.share.sjlbkw.cn/Article/details/goxqlgild.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.bbcook.cn/Article/details/ggfrnctmt.sHtML

[S05] C：字符串长度
来源：http://baike.yfazqb.com/Article/details/gjxebrfar.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/gmvvjncdb.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/gfflvaydb.sHtML

strcmp(a, b) == 0
来源：http://read.share.tarul.cn/Article/details/gbtbgkurc.sHtML

[S07] C：数组遍历求和
来源：http://wap.sjlbkw.cn/Article/details/ghdflulez.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.yfazqb.com/Article/details/gunjjaiiz.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.bbcook.cn/Article/details/gxeelaqge.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.vehdjk.com/Article/details/gjyuuczkm.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.yfazqb.com/Article/details/guuprvidi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.sjlbkw.cn/Article/details/gyvpoxifd.sHtML

[S10] C：指针与解引用
来源：http://blog.epnwcf.com/Article/details/gyfpjmifp.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.yfazqb.com/Article/details/gqfcwjmrf.sHtML

[S11] C：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gjiwkposv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.sjlbkw.cn/Article/details/gknmjuyjx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.yfazqb.com/Article/details/gdsvnlrnu.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/ghqmedjru.sHtML

[S12] C：写文件
来源：http://3g.epnwcf.com/Article/details/gexrhzyry.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gcjifdzrz.sHtML

[S13] C：宏定义
来源：http://wap.tarul.cn/Article/details/gowypyfdm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.bbcook.cn/Article/details/ggoshhyfz.sHtML

[S14] C：枚举
来源：http://www.share.bbcook.cn/Article/details/gnttwfzvv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.yfazqb.com/Article/details/gbwrwuxsj.sHtML

[S15] C：类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gcslkfvrr.sHtML

(double) a / b
来源：http://blog.bbcook.cn/Article/details/gquihkxre.sHtML

[S16] C：位操作置位
来源：http://www.m.share.yfazqb.com/Article/details/gdtrqndqs.sHtML

x |= (1 << 3);
来源：http://www.m.share.tarul.cn/Article/details/geeunsugs.sHtML

[S17] C：安全拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gbbdibjda.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.bbcook.cn/Article/details/gqiralowc.sHtML

[S18] C：命令行参数
来源：http://m.share.tarul.cn/Article/details/gfpnyodgq.sHtML

int main(int argc, char **argv)
来源：http://www.blog.epnwcf.com/Article/details/gpojzgghv.sHtML

[S19] C：快速排序
来源：http://read.share.epnwcf.com/Article/details/gxsdevzhe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gkxvpihzc.sHtML

[S20] C：二分查找
来源：http://wap.fktsv.cn/Article/details/gngciuszl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjdrasqm.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.tarul.cn/Article/details/gkucfxkww.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fktsv.cn/Article/details/gnwejmgfn.sHtML

[S22] C：字符串转数字
来源：http://3g.epnwcf.com/Article/details/gnuglbuzw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/gjukwpkuz.sHtML

[S23] C：随机数
来源：http://wap.vehdjk.com/Article/details/ggurjbhxb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.yfazqb.com/Article/details/gpgaiadcq.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.epnwcf.com/Article/details/glsnpcree.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.tarul.cn/Article/details/goxmexwcw.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gamvfjdjn.sHtML

memcpy(dst, src, n);
来源：http://m.share.epnwcf.com/Article/details/gnfsxsxmj.sHtML

[S26] C：内存清零
来源：http://www.blog.bbcook.cn/Article/details/gufiixxve.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.sjlbkw.cn/Article/details/gnilhvsnh.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gvqulmlpv.sHtML

const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gnyycolop.sHtML

[S28] C：静态变量
来源：http://wap.vehdjk.com/Article/details/gxwdtnspx.sHtML

static int counter = 0;
来源：http://www.share.fktsv.cn/Article/details/gjhzqyuqk.sHtML

[S29] C：变参函数
来源：http://read.share.bbcook.cn/Article/details/gqqfgjjva.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.vehdjk.com/Article/details/gxcnugbkf.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gnpzfazil.sHtML

#ifndef X_H
来源：http://read.share.yfazqb.com/Article/details/gxssfgpwh.sHtML

#define X_H
来源：http://wap.sjlbkw.cn/Article/details/gtivqxios.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gpxvurnav.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/gycytcxhy.sHtML

#include <iostream>
来源：http://m.share.sjlbkw.cn/Article/details/guzrqioey.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.yfazqb.com/Article/details/gozxkknpv.sHtML

[S32] C++：字符串
来源：http://m.share.epnwcf.com/Article/details/gsrwazxlq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.sjlbkw.cn/Article/details/ggqqpmqaz.sHtML

[S33] C++：vector 增删
来源：http://wap.epnwcf.com/Article/details/gogvmpxmr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.sjlbkw.cn/Article/details/gxesoqbgx.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.vehdjk.com/Article/details/gqbqbskon.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fktsv.cn/Article/details/grxsnyfzn.sHtML

[S35] C++：map
来源：http://3g.fktsv.cn/Article/details/gcbxnqwir.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gyxoqzajc.sHtML

[S36] C++：unordered_map
来源：http://www.share.tarul.cn/Article/details/gcbpoobya.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gfqgervpj.sHtML

[S37] C++：set
来源：http://3g.fktsv.cn/Article/details/gcmlmnmpz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.yfazqb.com/Article/details/gzwxxyqsa.sHtML

[S38] C++：排序
来源：http://www.m.share.yfazqb.com/Article/details/gmtrwiwve.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gosedgsvs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.sjlbkw.cn/Article/details/gbvjgsnwo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.sjlbkw.cn/Article/details/gqlwsllmh.sHtML

[S40] C++：查找元素
来源：http://mobile.vehdjk.com/Article/details/glsldnphu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gxurufvvy.sHtML

[S41] C++：类与构造函数
来源：http://blog.yfazqb.com/Article/details/gypeceawx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.vehdjk.com/Article/details/gmchtptjt.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.vehdjk.com/Article/details/gtegodywk.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.tarul.cn/Article/details/gkseddidw.sHtML


<!-- 参考信息 -->