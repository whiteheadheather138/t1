代发 wailian999

[Q76] 按天统计
来源：http://mobile.epnwcf.com/Article/details/gtqiaevch.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.tarul.cn/Article/details/gbgjdkeii.sHtML

[Q77] 时间加减
来源：http://blog.yfazqb.com/Article/details/giwfivmkt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.yfazqb.com/Article/details/gtgbqszov.sHtML

[Q78] 当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gsocghrqj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.bbcook.cn/Article/details/grgzfsxli.sHtML

[Q79] 字符串拼接
来源：http://blog.tarul.cn/Article/details/ghufbvnhn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fktsv.cn/Article/details/glsjgczkm.sHtML

[Q80] 字符串截取
来源：http://wap.epnwcf.com/Article/details/gfhtjmyyq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.tarul.cn/Article/details/giehcuiwe.sHtML

[Q81] 字符串替换
来源：http://3g.sjlbkw.cn/Article/details/gyfwfctrw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.tarul.cn/Article/details/gwolbqyhm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.epnwcf.com/Article/details/gwmoqtooc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gpuxqosye.sHtML

[Q83] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gycbhmtyg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gupdwtckb.sHtML

[Q84] 去除首尾空格
来源：http://wap.epnwcf.com/Article/details/gruiujqlg.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gogosozid.sHtML

[Q85] 数值取整
来源：http://3g.fktsv.cn/Article/details/guhwpodte.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gjwqmbqcu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.tarul.cn/Article/details/gaiyjyyvx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.bbcook.cn/Article/details/gzjrgagnx.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fktsv.cn/Article/details/gjuagswzx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.bbcook.cn/Article/details/gnqragpbh.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/gbjhjmaqj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fktsv.cn/Article/details/ghyioxezy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gdxcbbzur.sHtML

[Q89] 判断表是否存在
来源：http://wap.sjlbkw.cn/Article/details/goyhjknsv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fktsv.cn/Article/details/ghyoxmaep.sHtML

[Q90] 生成序号列
来源：http://wap.vehdjk.com/Article/details/gaztzdibr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fktsv.cn/Article/details/gnskexrny.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/guhtdnyzp.sHtML

R. Bash 专题
来源：http://mobile.fktsv.cn/Article/details/gmwdvvdif.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggmwsmhgo.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/gafjjtoav.sHtML

#!/usr/bin/env bash
来源：http://baike.fktsv.cn/Article/details/gopxkjagg.sHtML

set -euo pipefail
来源：http://blog.fktsv.cn/Article/details/grdffhijc.sHtML

[R02] 变量赋值与使用
来源：http://baike.tarul.cn/Article/details/guyosxydk.sHtML

name="Tom"; echo "$name"
来源：http://m.share.tarul.cn/Article/details/gsvhpqkhg.sHtML

[R03] 只读变量
来源：http://3g.bbcook.cn/Article/details/gbvjprwpf.sHtML

readonly PI=3.14
来源：http://www.share.epnwcf.com/Article/details/ghfuzslsm.sHtML

[R04] 位置参数
来源：http://blog.bbcook.cn/Article/details/gmfjsmxhn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.bbcook.cn/Article/details/gelfrsnze.sHtML

[R05] 参数默认值
来源：http://baike.bbcook.cn/Article/details/gcvqcyvpm.sHtML

name="${1:-default}"
来源：http://www.m.share.fktsv.cn/Article/details/ghyehybfa.sHtML

[R06] 判断命令是否存在
来源：http://mobile.vehdjk.com/Article/details/gonsxsztp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gglwchsyn.sHtML

[R07] if 判断文件
来源：http://read.share.bbcook.cn/Article/details/gnuiktzyt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.bbcook.cn/Article/details/gyizxkvff.sHtML

[R08] 数值比较
来源：http://baike.epnwcf.com/Article/details/ghwswuqxw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.epnwcf.com/Article/details/gflqsymgw.sHtML

[R09] 字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/gewxjovlp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.vehdjk.com/Article/details/gfeterjct.sHtML

[R10] 正则匹配
来源：http://wap.tarul.cn/Article/details/gkzqgjphm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fktsv.cn/Article/details/givnjselh.sHtML

[R11] case 多分支
来源：http://www.share.sjlbkw.cn/Article/details/gezcclvwu.sHtML

case "$1" in
来源：http://wap.sjlbkw.cn/Article/details/gymcbszvn.sHtML

start) echo "启动" ;;
来源：http://baike.tarul.cn/Article/details/gckzztxsf.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.tarul.cn/Article/details/gykithccd.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fktsv.cn/Article/details/gjjjgifgv.sHtML

esac
来源：http://mobile.bbcook.cn/Article/details/gqovoescm.sHtML

[R12] for 遍历文件
来源：http://wap.yfazqb.com/Article/details/gczpmegel.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.bbcook.cn/Article/details/gjxywenwy.sHtML

[R13] for 计数循环
来源：http://wap.tarul.cn/Article/details/gaqomhqny.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gcmbsjhqb.sHtML

[R14] C 风格 for
来源：http://wap.sjlbkw.cn/Article/details/gxfcvnzwy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gfhtyxitp.sHtML

[R15] while 逐行读文件
来源：http://www.share.fktsv.cn/Article/details/griaylxbr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.bbcook.cn/Article/details/gujhksaxe.sHtML

[R16] until 等待条件
来源：http://m.share.vehdjk.com/Article/details/gemoochpp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/grpkhiiak.sHtML

[R17] 数组定义与取值
来源：http://read.share.vehdjk.com/Article/details/gvosfufhg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.tarul.cn/Article/details/gfhaqmdad.sHtML

[R18] 遍历数组
来源：http://www.m.share.epnwcf.com/Article/details/grtexkdsk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/gdzoslenl.sHtML

[R19] 数组长度
来源：http://wap.yfazqb.com/Article/details/gtxindiyo.sHtML

echo "${#arr[@]}"
来源：http://mobile.epnwcf.com/Article/details/godsywqeh.sHtML

[R20] 关联数组（字典）
来源：http://blog.yfazqb.com/Article/details/gouelwipg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.vehdjk.com/Article/details/gekululwr.sHtML

[R21] 字符串长度
来源：http://m.share.vehdjk.com/Article/details/genvikkdp.sHtML

echo "${#s}"
来源：http://read.share.yfazqb.com/Article/details/grgmbircl.sHtML

[R22] 截取子串
来源：http://3g.yfazqb.com/Article/details/gipwgtkli.sHtML

echo "${s:0:5}"
来源：http://www.blog.sjlbkw.cn/Article/details/gillqcstt.sHtML

[R23] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/gzujrlafp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.epnwcf.com/Article/details/gcgoopbcs.sHtML

[R24] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/ggfaqkggu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fktsv.cn/Article/details/grpptqfgr.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fktsv.cn/Article/details/ggdqrzuzn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/gqshndalt.sHtML

[R26] 命令替换
来源：http://www.share.yfazqb.com/Article/details/gucktlcta.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.vehdjk.com/Article/details/glahstdse.sHtML

[R27] 算术展开
来源：http://www.share.bbcook.cn/Article/details/gylhtqcbl.sHtML

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/gjfzompar.sHtML

[R28] 浮点运算
来源：http://www.m.share.fktsv.cn/Article/details/gfzvqvexs.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.vehdjk.com/Article/details/gvjjoorwb.sHtML

[R29] 定义函数
来源：http://wap.yfazqb.com/Article/details/gkedgogxg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.epnwcf.com/Article/details/gmaqiumag.sHtML

[R30] 函数返回状态码
来源：http://blog.sjlbkw.cn/Article/details/gxxogsjsa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.yfazqb.com/Article/details/gnhqtyudu.sHtML

[R31] 局部变量
来源：http://wap.vehdjk.com/Article/details/guhydxogw.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.yfazqb.com/Article/details/ghkrvmfus.sHtML

[R32] 参数个数校验
来源：http://3g.tarul.cn/Article/details/ggwknkehg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gbwxfwrbi.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.sjlbkw.cn/Article/details/giperocuz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.tarul.cn/Article/details/glufduqhd.sHtML

[R34] 退出时清理
来源：http://mobile.epnwcf.com/Article/details/gycickemg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/ggjstyksi.sHtML

[R35] 后台执行并等待
来源：http://www.share.vehdjk.com/Article/details/gbkjnnyqo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.tarul.cn/Article/details/gqlwgcqst.sHtML

[R36] 并发执行多个任务
来源：http://baike.tarul.cn/Article/details/gtbqkovzg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.sjlbkw.cn/Article/details/gcrtejiea.sHtML

[R37] 把输出赋给变量
来源：http://wap.vehdjk.com/Article/details/gawoioguq.sHtML

files=$(ls -1)
来源：http://wap.bbcook.cn/Article/details/gxlwugmrs.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/gyqolydxi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.yfazqb.com/Article/details/gbccyrvct.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.yfazqb.com/Article/details/ggdzgcswv.sHtML

cmd > out.log 2>&1
来源：http://3g.epnwcf.com/Article/details/gfrrsibqy.sHtML

[R40] 追加写日志
来源：http://m.share.bbcook.cn/Article/details/gyzfxlsev.sHtML

echo "log" >> out.log
来源：http://wap.fktsv.cn/Article/details/geomzewkq.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/gtumesimz.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.epnwcf.com/Article/details/gupdklwbq.sHtML

[R42] 输入重定向
来源：http://mobile.bbcook.cn/Article/details/gfzsxugql.sHtML

wc -l < a.txt
来源：http://www.blog.yfazqb.com/Article/details/gflufiyrj.sHtML

[R43] 按名字查找文件
来源：http://wap.bbcook.cn/Article/details/gmebuhmnm.sHtML

find . -name "*.log" -type f
来源：http://baike.vehdjk.com/Article/details/grrfknpuo.sHtML

[R44] 按修改时间查找
来源：http://blog.tarul.cn/Article/details/gtyiukwoq.sHtML

find . -mtime -7 -type f
来源：http://www.share.yfazqb.com/Article/details/glodrpbcd.sHtML

[R45] 批量删除
来源：http://www.m.share.epnwcf.com/Article/details/golrnrrms.sHtML

find . -name "*.tmp" -delete
来源：http://blog.yfazqb.com/Article/details/gxveudjmu.sHtML

[R46] 递归替换文件内容
来源：http://blog.vehdjk.com/Article/details/gatuurcyj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fktsv.cn/Article/details/gulmsibhk.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/gndfqfrpb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/ggjorifpx.sHtML

[R48] awk 取指定列
来源：http://baike.vehdjk.com/Article/details/gdrwvtnhm.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gznvvbspf.sHtML

[R49] awk 带条件
来源：http://www.share.sjlbkw.cn/Article/details/gxfflghzc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.epnwcf.com/Article/details/glbxazgoj.sHtML

[R50] awk 求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gxejzersw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.vehdjk.com/Article/details/gihyuzxvo.sHtML

[R51] 排序去重取前几
来源：http://www.blog.sjlbkw.cn/Article/details/gcggvpnpi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.tarul.cn/Article/details/gmodgfyrz.sHtML

[R52] 统计行数
来源：http://www.blog.bbcook.cn/Article/details/gzhyndtff.sHtML

wc -l a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gstfsqkku.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.tarul.cn/Article/details/goujuqswn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.yfazqb.com/Article/details/gukzlstlx.sHtML

[R54] 比较两个文件
来源：http://wap.epnwcf.com/Article/details/gvszdqhuq.sHtML

diff a.txt b.txt
来源：http://www.m.share.fktsv.cn/Article/details/gjdbebhtj.sHtML

[R55] 压缩与解压
来源：http://www.share.sjlbkw.cn/Article/details/govlpqlim.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/gljqxixvq.sHtML

[R56] 远程拷贝
来源：http://blog.epnwcf.com/Article/details/gvibltqmp.sHtML

scp file user@host:/path/
来源：http://3g.bbcook.cn/Article/details/ggsdexwuq.sHtML

[R57] 远程执行命令
来源：http://baike.fktsv.cn/Article/details/ggbnogpup.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/gxjgveqvh.sHtML

[R58] 下载文件
来源：http://www.share.yfazqb.com/Article/details/gysjywawn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.sjlbkw.cn/Article/details/ggftndbwz.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gkdtyriao.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.sjlbkw.cn/Article/details/glvmaixjr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gmpnglypt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.bbcook.cn/Article/details/gtewmjwxw.sHtML

[R61] 磁盘占用
来源：http://read.share.fktsv.cn/Article/details/gqgvnuzfw.sHtML

df -h;  du -sh *
来源：http://www.share.fktsv.cn/Article/details/ghapzjppw.sHtML

[R62] 找最占空间的文件
来源：http://mobile.vehdjk.com/Article/details/gekxkuwgc.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.bbcook.cn/Article/details/ghjsultog.sHtML

[R63] 内存与进程
来源：http://3g.sjlbkw.cn/Article/details/gowqnonqj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.epnwcf.com/Article/details/gvwrfhqjc.sHtML

[R64] 结束进程
来源：http://mobile.bbcook.cn/Article/details/gcwdfvtfq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.yfazqb.com/Article/details/gdrzkyedi.sHtML

[R65] 查看端口占用
来源：http://mobile.epnwcf.com/Article/details/gqljfswph.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.epnwcf.com/Article/details/gecaqlrum.sHtML

[R66] 定时任务
来源：http://www.share.fktsv.cn/Article/details/gbuzagycx.sHtML

crontab -e;  crontab -l
来源：http://m.share.yfazqb.com/Article/details/ggvsbysuh.sHtML

[R67] 生成随机十六进制串
来源：http://blog.tarul.cn/Article/details/gysquzscp.sHtML

openssl rand -hex 16
来源：http://wap.fktsv.cn/Article/details/gdnmjmklx.sHtML

[R68] 计算文件校验值
来源：http://m.share.tarul.cn/Article/details/gonfrsyhh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.bbcook.cn/Article/details/gactkqvqf.sHtML

[R69] 生成随机密码
来源：http://3g.epnwcf.com/Article/details/gkeewtrjf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.tarul.cn/Article/details/gnibxwnpi.sHtML

[R70] 时间戳与互转
来源：http://mobile.yfazqb.com/Article/details/gfkxikhfi.sHtML

date +%s;  date -d @1700000000
来源：http://3g.sjlbkw.cn/Article/details/gngiabuge.sHtML

[R71] 日期格式化
来源：http://read.share.tarul.cn/Article/details/gjcwibihq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.vehdjk.com/Article/details/goaxxmhlb.sHtML

[R72] 等待端口就绪
来源：http://wap.tarul.cn/Article/details/gxtygtrwm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gofegkdjm.sHtML

[R73] 分割大日志
来源：http://wap.yfazqb.com/Article/details/gtderucmx.sHtML

split -l 1000 big.log part_
来源：http://mobile.sjlbkw.cn/Article/details/gknriquyi.sHtML

[R74] 批量重命名
来源：http://read.share.sjlbkw.cn/Article/details/gmwbcgmkm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.epnwcf.com/Article/details/gqrghghec.sHtML

[R75] 导出环境变量
来源：http://wap.sjlbkw.cn/Article/details/glalgkdhx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.epnwcf.com/Article/details/gntavdtwc.sHtML

[R76] 使用临时文件
来源：http://www.share.fktsv.cn/Article/details/gcvujnbnz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/govyeuxkw.sHtML

[R77] 读取用户输入
来源：http://m.share.yfazqb.com/Article/details/gjxmjjhyq.sHtML

read -rp "请输入: " ans
来源：http://www.blog.sjlbkw.cn/Article/details/gkisjxghd.sHtML

[R78] 交互式菜单
来源：http://www.share.yfazqb.com/Article/details/gcizqvwml.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.epnwcf.com/Article/details/gwxatvynk.sHtML

[R79] 解析命令行选项
来源：http://m.share.sjlbkw.cn/Article/details/gmozjbwdi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.sjlbkw.cn/Article/details/gobonxteb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlsrxtec.sHtML

time ./run.sh
来源：http://read.share.sjlbkw.cn/Article/details/gghknugxe.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gxovihzqt.sHtML

S. C / C++ 专题
来源：http://wap.vehdjk.com/Article/details/gamczdrnk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gnnsgczko.sHtML

[S01] C：Hello World
来源：http://read.share.fktsv.cn/Article/details/gjamvvfuj.sHtML

#include <stdio.h>
来源：http://www.blog.epnwcf.com/Article/details/gawrarkei.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.yfazqb.com/Article/details/gvzecspst.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gwjklhfkn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.bbcook.cn/Article/details/gcfrizuoq.sHtML

[S03] C：读入整数
来源：http://www.blog.yfazqb.com/Article/details/guizhkqtv.sHtML

int x; scanf("%d", &x);
来源：http://baike.epnwcf.com/Article/details/gftjodneg.sHtML

[S04] C：字符串复制
来源：http://www.blog.fktsv.cn/Article/details/gzjoudokh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.epnwcf.com/Article/details/gxopxkoxp.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/guqztilsa.sHtML

strlen(s)
来源：http://baike.vehdjk.com/Article/details/gudkjhdny.sHtML

[S06] C：字符串比较
来源：http://wap.epnwcf.com/Article/details/gzutjvllg.sHtML

strcmp(a, b) == 0
来源：http://m.share.fktsv.cn/Article/details/gkcukdamz.sHtML

[S07] C：数组遍历求和
来源：http://wap.bbcook.cn/Article/details/gqspbwfyt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.vehdjk.com/Article/details/goiifnngc.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.sjlbkw.cn/Article/details/geqokhdfk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.yfazqb.com/Article/details/gwerrijxi.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.sjlbkw.cn/Article/details/gpizrtukl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fktsv.cn/Article/details/gjaivgkgh.sHtML

[S10] C：指针与解引用
来源：http://read.share.sjlbkw.cn/Article/details/gfiggjmlv.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghalxjmne.sHtML

[S11] C：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gvmctbfnm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.vehdjk.com/Article/details/gnueyitra.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.vehdjk.com/Article/details/gerrmcmrt.sHtML

fclose(f);
来源：http://www.share.bbcook.cn/Article/details/gopjvrbzd.sHtML

[S12] C：写文件
来源：http://3g.epnwcf.com/Article/details/gliwpdkmp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gvkcegvaq.sHtML

[S13] C：宏定义
来源：http://3g.bbcook.cn/Article/details/gwinocswd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.sjlbkw.cn/Article/details/gzujnnsas.sHtML

[S14] C：枚举
来源：http://www.blog.fktsv.cn/Article/details/gkeodnavu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.bbcook.cn/Article/details/grlqseeyg.sHtML

[S15] C：类型转换
来源：http://www.m.share.yfazqb.com/Article/details/gpfhlckbq.sHtML

(double) a / b
来源：http://wap.epnwcf.com/Article/details/gmmxckige.sHtML

[S16] C：位操作置位
来源：http://m.share.bbcook.cn/Article/details/gpspnkspw.sHtML

x |= (1 << 3);
来源：http://baike.epnwcf.com/Article/details/gtxtzkumg.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.tarul.cn/Article/details/gnxiltdne.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.yfazqb.com/Article/details/gvdipkdqq.sHtML

[S18] C：命令行参数
来源：http://baike.bbcook.cn/Article/details/geoympbvn.sHtML

int main(int argc, char **argv)
来源：http://read.share.sjlbkw.cn/Article/details/glygqsuoz.sHtML

[S19] C：快速排序
来源：http://read.share.bbcook.cn/Article/details/gjxagpxzx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gtxkvbcya.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/gioceqalz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/ghiooqzoo.sHtML

[S21] C：字符类别判断
来源：http://mobile.sjlbkw.cn/Article/details/gdxipnrup.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.bbcook.cn/Article/details/guusgimhu.sHtML

[S22] C：字符串转数字
来源：http://read.share.sjlbkw.cn/Article/details/gktmkcoje.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.sjlbkw.cn/Article/details/gbukrxjot.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/gidhaqzsb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.tarul.cn/Article/details/gbwuygcao.sHtML

[S24] C：获取本地时间
来源：http://read.share.bbcook.cn/Article/details/giubkrcdo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.bbcook.cn/Article/details/gkxkwrfal.sHtML

[S25] C：内存拷贝
来源：http://blog.bbcook.cn/Article/details/ggdjtpkyj.sHtML

memcpy(dst, src, n);
来源：http://wap.sjlbkw.cn/Article/details/gnohdswxh.sHtML

[S26] C：内存清零
来源：http://m.share.tarul.cn/Article/details/gcxtloutv.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.epnwcf.com/Article/details/gtstmwpnh.sHtML

[S27] C：定义常量
来源：http://3g.tarul.cn/Article/details/gdqkqyors.sHtML

const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gyerqfnid.sHtML

[S28] C：静态变量
来源：http://read.share.yfazqb.com/Article/details/gpxdfgffz.sHtML

static int counter = 0;
来源：http://www.blog.epnwcf.com/Article/details/gtfyofqpr.sHtML

[S29] C：变参函数
来源：http://blog.yfazqb.com/Article/details/gacwpdggp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gzswmvfzl.sHtML

[S30] C：头文件保护
来源：http://baike.fktsv.cn/Article/details/gidfmzzgk.sHtML

#ifndef X_H
来源：http://mobile.yfazqb.com/Article/details/gmxbuzngr.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/gawdytflo.sHtML

#endif
来源：http://www.blog.vehdjk.com/Article/details/gubbzmdpz.sHtML

[S31] C++：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gzckrjetl.sHtML

#include <iostream>
来源：http://m.share.tarul.cn/Article/details/ghjueazhw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fktsv.cn/Article/details/gbpsvmgyj.sHtML

[S32] C++：字符串
来源：http://m.share.epnwcf.com/Article/details/gdotkucbd.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/gffnaqtyl.sHtML

[S33] C++：vector 增删
来源：http://3g.sjlbkw.cn/Article/details/glfnlotmq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.epnwcf.com/Article/details/gwtsftrjh.sHtML

[S34] C++：遍历 vector
来源：http://mobile.bbcook.cn/Article/details/gssogqxdm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.yfazqb.com/Article/details/gnzpzqkzc.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gqrvonhba.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gvtchghsf.sHtML

[S36] C++：unordered_map
来源：http://m.share.yfazqb.com/Article/details/gvvawftwk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/gdlhgsuva.sHtML

[S37] C++：set
来源：http://read.share.yfazqb.com/Article/details/gxkqikjui.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.epnwcf.com/Article/details/grsjrgfdy.sHtML

[S38] C++：排序
来源：http://wap.sjlbkw.cn/Article/details/gbnclkapk.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/ghjfjmhay.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.bbcook.cn/Article/details/gqrilfzeh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.epnwcf.com/Article/details/ghrcokquc.sHtML

[S40] C++：查找元素
来源：http://3g.vehdjk.com/Article/details/gjazszlnn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.yfazqb.com/Article/details/glyvllwbf.sHtML

[S41] C++：类与构造函数
来源：http://www.share.tarul.cn/Article/details/gteknwghd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/gwxuxscgi.sHtML

[S42] C++：继承与虚函数
来源：http://wap.vehdjk.com/Article/details/gynayhjam.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.tarul.cn/Article/details/gvteztwiq.sHtML

[S43] C++：智能指针
来源：http://m.share.vehdjk.com/Article/details/gvgoniyom.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.tarul.cn/Article/details/gxamrlqvi.sHtML

[S44] C++：引用传参
来源：http://blog.yfazqb.com/Article/details/gjtslzytn.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.vehdjk.com/Article/details/gfamoohzq.sHtML

[S45] C++：lambda
来源：http://mobile.fktsv.cn/Article/details/glbiwrtjq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.tarul.cn/Article/details/gcrgddwuf.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/gktaelctz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.epnwcf.com/Article/details/gypegwlew.sHtML


<!-- 参考信息 -->