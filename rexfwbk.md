代发 wailian999

[Q80] 字符串截取
来源：http://wap.bbcook.cn/Article/details/gyqzfcmxx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gfqgcwvhd.sHtML

[Q81] 字符串替换
来源：http://3g.fktsv.cn/Article/details/gpltngckn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gzhictrxv.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.yfazqb.com/Article/details/gstmplodi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gncpbwbtc.sHtML

[Q83] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gtzwygrhv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gaaaqzvqh.sHtML

[Q84] 去除首尾空格
来源：http://read.share.yfazqb.com/Article/details/giyiqpemn.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gmixlthuw.sHtML

[Q85] 数值取整
来源：http://mobile.fktsv.cn/Article/details/ggvemuexz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.yfazqb.com/Article/details/gtiaftmjo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.bbcook.cn/Article/details/gsbecbrvt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.epnwcf.com/Article/details/gpundsnmk.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.vehdjk.com/Article/details/gdpvgerhb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.sjlbkw.cn/Article/details/geonmsehm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.vehdjk.com/Article/details/gncsbbasz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.bbcook.cn/Article/details/gtvbruech.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.epnwcf.com/Article/details/ghqojfqwu.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/geuxkkosq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.epnwcf.com/Article/details/gljstaukp.sHtML

[Q90] 生成序号列
来源：http://wap.epnwcf.com/Article/details/gokgoqpwu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.bbcook.cn/Article/details/gqldbjwsz.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gsdcmicex.sHtML

R. Bash 专题
来源：http://baike.fktsv.cn/Article/details/gwangdfuv.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvtjrkfeh.sHtML

[R01] shebang 与严格模式
来源：http://3g.yfazqb.com/Article/details/gibnbmhiq.sHtML

#!/usr/bin/env bash
来源：http://mobile.epnwcf.com/Article/details/gzrtwftgn.sHtML

set -euo pipefail
来源：http://baike.epnwcf.com/Article/details/gbemoccaj.sHtML

[R02] 变量赋值与使用
来源：http://www.share.sjlbkw.cn/Article/details/geiafctub.sHtML

name="Tom"; echo "$name"
来源：http://www.share.bbcook.cn/Article/details/gndoqplwc.sHtML

[R03] 只读变量
来源：http://m.share.epnwcf.com/Article/details/gozzkfnqk.sHtML

readonly PI=3.14
来源：http://read.share.vehdjk.com/Article/details/gbmdhsiwh.sHtML

[R04] 位置参数
来源：http://3g.epnwcf.com/Article/details/gvgihkmye.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.epnwcf.com/Article/details/gibnbiyvz.sHtML

[R05] 参数默认值
来源：http://www.share.fktsv.cn/Article/details/gowuqdtxo.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/grtgtfvla.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gltsxdori.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gzoopbmwz.sHtML

[R07] if 判断文件
来源：http://www.share.tarul.cn/Article/details/gzikmzlkk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.sjlbkw.cn/Article/details/gvqiygsbr.sHtML

[R08] 数值比较
来源：http://wap.tarul.cn/Article/details/gfnfhauev.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fktsv.cn/Article/details/gjsuybcgw.sHtML

[R09] 字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gdlbzwfci.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fktsv.cn/Article/details/gfqvgelib.sHtML

[R10] 正则匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/geglqrbmi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.sjlbkw.cn/Article/details/geosktdud.sHtML

[R11] case 多分支
来源：http://www.blog.tarul.cn/Article/details/gogsufltb.sHtML

case "$1" in
来源：http://wap.epnwcf.com/Article/details/gzigsrzfb.sHtML

start) echo "启动" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gnnctsfqb.sHtML

stop)  echo "停止" ;;
来源：http://www.share.tarul.cn/Article/details/geeradxac.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.tarul.cn/Article/details/gbusestwz.sHtML

esac
来源：http://3g.yfazqb.com/Article/details/gvzvqxner.sHtML

[R12] for 遍历文件
来源：http://blog.sjlbkw.cn/Article/details/gutlrhmyv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.tarul.cn/Article/details/glumuwucm.sHtML

[R13] for 计数循环
来源：http://www.share.yfazqb.com/Article/details/ggqkkzrny.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gfmdlchmo.sHtML

[R14] C 风格 for
来源：http://www.share.fktsv.cn/Article/details/gxklrkfds.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gjdgmlfmo.sHtML

[R15] while 逐行读文件
来源：http://m.share.tarul.cn/Article/details/gdmqqjyrk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fktsv.cn/Article/details/gvhjssvut.sHtML

[R16] until 等待条件
来源：http://blog.fktsv.cn/Article/details/gmzvkzqhj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gntbtpqoj.sHtML

[R17] 数组定义与取值
来源：http://www.share.fktsv.cn/Article/details/gzgthcwgd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/gopjziukj.sHtML

[R18] 遍历数组
来源：http://www.share.epnwcf.com/Article/details/gkboebnof.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.tarul.cn/Article/details/gtoptptqz.sHtML

[R19] 数组长度
来源：http://m.share.vehdjk.com/Article/details/gwlcalysk.sHtML

echo "${#arr[@]}"
来源：http://blog.tarul.cn/Article/details/gyhkljtuk.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.epnwcf.com/Article/details/guzcpxfnl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.epnwcf.com/Article/details/gzehttqzx.sHtML

[R21] 字符串长度
来源：http://wap.epnwcf.com/Article/details/gwxgmddzs.sHtML

echo "${#s}"
来源：http://m.share.tarul.cn/Article/details/gmlvvkacu.sHtML

[R22] 截取子串
来源：http://www.blog.yfazqb.com/Article/details/gtbbsgetx.sHtML

echo "${s:0:5}"
来源：http://m.share.sjlbkw.cn/Article/details/gnyewzeat.sHtML

[R23] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/gdplrtqpc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gwylovqrd.sHtML

[R24] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gzkuyfufe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.vehdjk.com/Article/details/glvxwjdxs.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.yfazqb.com/Article/details/gxcswnpqe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.bbcook.cn/Article/details/gavoujoqg.sHtML

[R26] 命令替换
来源：http://wap.fktsv.cn/Article/details/gcpjdwjit.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.bbcook.cn/Article/details/gbgjqvkok.sHtML

[R27] 算术展开
来源：http://read.share.epnwcf.com/Article/details/gbvmrbxds.sHtML

echo $((1 + 2 * 3))
来源：http://wap.yfazqb.com/Article/details/gpycsaoug.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/gubyuuciu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.sjlbkw.cn/Article/details/gqkstuuyx.sHtML

[R29] 定义函数
来源：http://read.share.yfazqb.com/Article/details/gfcxqbpsv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fktsv.cn/Article/details/gdykhgqnz.sHtML

[R30] 函数返回状态码
来源：http://blog.yfazqb.com/Article/details/gibodircj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.tarul.cn/Article/details/gskwkejvz.sHtML

[R31] 局部变量
来源：http://www.blog.vehdjk.com/Article/details/gqjojrfwl.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fktsv.cn/Article/details/giaxfejaw.sHtML

[R32] 参数个数校验
来源：http://baike.vehdjk.com/Article/details/gybjtbtig.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gnonbcjvg.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.bbcook.cn/Article/details/gzuddddua.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fktsv.cn/Article/details/gzdouhbpq.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/gcmuskvtr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/glrinfupl.sHtML

[R35] 后台执行并等待
来源：http://www.blog.bbcook.cn/Article/details/gsazxbuol.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.vehdjk.com/Article/details/gdhvwenfg.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.vehdjk.com/Article/details/ghjggeivn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.vehdjk.com/Article/details/gclzqmlgw.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gybbzeltn.sHtML

files=$(ls -1)
来源：http://baike.bbcook.cn/Article/details/gtqbpbwzv.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/gxnwizyzy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.yfazqb.com/Article/details/gtitdztno.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/ghljituge.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/gxqbueoxs.sHtML

[R40] 追加写日志
来源：http://read.share.yfazqb.com/Article/details/gltxuxdwe.sHtML

echo "log" >> out.log
来源：http://wap.epnwcf.com/Article/details/gmckhcozk.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/glepuxqjf.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gytmypsqu.sHtML

[R42] 输入重定向
来源：http://blog.vehdjk.com/Article/details/ggiswbjio.sHtML

wc -l < a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gnvvprfrc.sHtML

[R43] 按名字查找文件
来源：http://baike.vehdjk.com/Article/details/gakmqceir.sHtML

find . -name "*.log" -type f
来源：http://www.blog.vehdjk.com/Article/details/gagemhhrv.sHtML

[R44] 按修改时间查找
来源：http://www.share.sjlbkw.cn/Article/details/gccxxfvbw.sHtML

find . -mtime -7 -type f
来源：http://www.blog.bbcook.cn/Article/details/gnrmsfdvv.sHtML

[R45] 批量删除
来源：http://read.share.epnwcf.com/Article/details/ggtyfkjki.sHtML

find . -name "*.tmp" -delete
来源：http://3g.epnwcf.com/Article/details/gytlirhei.sHtML

[R46] 递归替换文件内容
来源：http://www.share.tarul.cn/Article/details/gihszalls.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.epnwcf.com/Article/details/gggsnydpy.sHtML

[R47] sed 单行替换
来源：http://www.m.share.epnwcf.com/Article/details/gmmdhuium.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.yfazqb.com/Article/details/gcvteccgb.sHtML

[R48] awk 取指定列
来源：http://www.blog.fktsv.cn/Article/details/gljjavanv.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gyvkysldt.sHtML

[R49] awk 带条件
来源：http://m.share.bbcook.cn/Article/details/gqqaykomf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.bbcook.cn/Article/details/gzqsajoyc.sHtML

[R50] awk 求和
来源：http://3g.bbcook.cn/Article/details/ghmfnmkgm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gmufsnxte.sHtML

[R51] 排序去重取前几
来源：http://3g.bbcook.cn/Article/details/gsvloflyw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fktsv.cn/Article/details/gvudmnsnl.sHtML

[R52] 统计行数
来源：http://baike.bbcook.cn/Article/details/gcdxmqpaq.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/gvepkvpja.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.vehdjk.com/Article/details/gmzgxrxjo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.tarul.cn/Article/details/gbzujgkys.sHtML

[R54] 比较两个文件
来源：http://mobile.epnwcf.com/Article/details/gtoeinene.sHtML

diff a.txt b.txt
来源：http://www.blog.fktsv.cn/Article/details/grvkeqmuv.sHtML

[R55] 压缩与解压
来源：http://www.blog.fktsv.cn/Article/details/gmxorkpdc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/gfmygkrhp.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/guyyblfog.sHtML

scp file user@host:/path/
来源：http://3g.epnwcf.com/Article/details/gfqemrgjh.sHtML

[R57] 远程执行命令
来源：http://blog.tarul.cn/Article/details/gnwwyxeph.sHtML

ssh user@host 'uptime'
来源：http://mobile.tarul.cn/Article/details/gqyvowzzc.sHtML

[R58] 下载文件
来源：http://www.blog.bbcook.cn/Article/details/gdyplgoaa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.vehdjk.com/Article/details/gkifzmioz.sHtML

[R59] 发 POST JSON
来源：http://www.share.yfazqb.com/Article/details/gyuvpcjpb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.vehdjk.com/Article/details/gajzzuhsy.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/gldvjkwjh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.tarul.cn/Article/details/gsnuosofm.sHtML

[R61] 磁盘占用
来源：http://m.share.fktsv.cn/Article/details/gxsctknli.sHtML

df -h;  du -sh *
来源：http://www.share.tarul.cn/Article/details/gwufpgmuq.sHtML

[R62] 找最占空间的文件
来源：http://3g.yfazqb.com/Article/details/gvxdwsvrp.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.sjlbkw.cn/Article/details/ghbsoejxd.sHtML

[R63] 内存与进程
来源：http://3g.fktsv.cn/Article/details/gopcvuqft.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.sjlbkw.cn/Article/details/gweiapozg.sHtML

[R64] 结束进程
来源：http://www.blog.vehdjk.com/Article/details/gearjqeid.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.sjlbkw.cn/Article/details/glmivgdla.sHtML

[R65] 查看端口占用
来源：http://3g.vehdjk.com/Article/details/gndmhvrpf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.sjlbkw.cn/Article/details/givzqaanq.sHtML

[R66] 定时任务
来源：http://3g.tarul.cn/Article/details/gbmvaxgaz.sHtML

crontab -e;  crontab -l
来源：http://baike.epnwcf.com/Article/details/gnfsxeyed.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/gdtfahued.sHtML

openssl rand -hex 16
来源：http://baike.epnwcf.com/Article/details/gefmbxlru.sHtML

[R68] 计算文件校验值
来源：http://mobile.fktsv.cn/Article/details/gnqdbguts.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/goambyjjx.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fktsv.cn/Article/details/gffnvpjkx.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.tarul.cn/Article/details/gbnrcpvtv.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.yfazqb.com/Article/details/gxkuzuvoe.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fktsv.cn/Article/details/gimzvsuca.sHtML

[R71] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gwrtsxenn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.tarul.cn/Article/details/gpsvgyjhu.sHtML

[R72] 等待端口就绪
来源：http://3g.tarul.cn/Article/details/gurkcxsvn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gbpshawdr.sHtML

[R73] 分割大日志
来源：http://www.blog.sjlbkw.cn/Article/details/giloggprw.sHtML

split -l 1000 big.log part_
来源：http://www.share.yfazqb.com/Article/details/gtuqmjzgc.sHtML

[R74] 批量重命名
来源：http://read.share.sjlbkw.cn/Article/details/gnijwprqz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.bbcook.cn/Article/details/ghnibyjbq.sHtML

[R75] 导出环境变量
来源：http://m.share.epnwcf.com/Article/details/gkkjjhfms.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.tarul.cn/Article/details/gtogrxcsk.sHtML

[R76] 使用临时文件
来源：http://mobile.epnwcf.com/Article/details/gelaczmzb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/ggelwvrcd.sHtML

[R77] 读取用户输入
来源：http://read.share.yfazqb.com/Article/details/gczmmmkom.sHtML

read -rp "请输入: " ans
来源：http://www.share.yfazqb.com/Article/details/gwhtzpqtl.sHtML

[R78] 交互式菜单
来源：http://3g.vehdjk.com/Article/details/glphrtvuy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.epnwcf.com/Article/details/gvuutmosq.sHtML

[R79] 解析命令行选项
来源：http://read.share.bbcook.cn/Article/details/gmwujgnic.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.yfazqb.com/Article/details/gdcnyunxk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fktsv.cn/Article/details/gimdjxhty.sHtML

time ./run.sh
来源：http://baike.sjlbkw.cn/Article/details/gtjprphkv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjxtvthwm.sHtML

S. C / C++ 专题
来源：http://mobile.sjlbkw.cn/Article/details/gmeixdqim.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnyxverxi.sHtML

[S01] C：Hello World
来源：http://read.share.bbcook.cn/Article/details/geyztylyr.sHtML

#include <stdio.h>
来源：http://read.share.tarul.cn/Article/details/gdlvqbkip.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.epnwcf.com/Article/details/gplnmabwx.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.yfazqb.com/Article/details/gyzjmtxpx.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fktsv.cn/Article/details/gtodxzoyq.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/gwfpttqbl.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/genwvmlej.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fktsv.cn/Article/details/gwridtsfl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.tarul.cn/Article/details/gyiwcizcb.sHtML

[S05] C：字符串长度
来源：http://read.share.tarul.cn/Article/details/gkkfdpxbc.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/gbrlcshyd.sHtML

[S06] C：字符串比较
来源：http://baike.vehdjk.com/Article/details/gvrdqsccj.sHtML

strcmp(a, b) == 0
来源：http://blog.vehdjk.com/Article/details/gxnxbutpa.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fktsv.cn/Article/details/ggngbgooy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.tarul.cn/Article/details/grqcdnrai.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.epnwcf.com/Article/details/gpjxypzjj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.vehdjk.com/Article/details/glfliujxl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.bbcook.cn/Article/details/gceippstm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.bbcook.cn/Article/details/guybiunpw.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gtvoiclyu.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/gyldyfsnb.sHtML

[S11] C：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gicgrqwnu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fktsv.cn/Article/details/gejgohckj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.tarul.cn/Article/details/gpfzdnwre.sHtML

fclose(f);
来源：http://m.share.fktsv.cn/Article/details/gpyxbqjiz.sHtML

[S12] C：写文件
来源：http://m.share.fktsv.cn/Article/details/gnumjsimq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gfzoratra.sHtML

[S13] C：宏定义
来源：http://m.share.epnwcf.com/Article/details/gmbabvger.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.tarul.cn/Article/details/gwldvnyza.sHtML

[S14] C：枚举
来源：http://www.blog.bbcook.cn/Article/details/gibdsoume.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.bbcook.cn/Article/details/gphzhxeij.sHtML

[S15] C：类型转换
来源：http://www.share.tarul.cn/Article/details/gyxejeaxr.sHtML

(double) a / b
来源：http://read.share.sjlbkw.cn/Article/details/goevhjxat.sHtML

[S16] C：位操作置位
来源：http://www.blog.epnwcf.com/Article/details/gdsggrswg.sHtML

x |= (1 << 3);
来源：http://mobile.vehdjk.com/Article/details/gjmbzhdve.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gjpxgcvdl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.yfazqb.com/Article/details/gtbxpnocn.sHtML

[S18] C：命令行参数
来源：http://blog.bbcook.cn/Article/details/galerouuq.sHtML

int main(int argc, char **argv)
来源：http://blog.tarul.cn/Article/details/gizgltncm.sHtML

[S19] C：快速排序
来源：http://read.share.yfazqb.com/Article/details/gwewzufdw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gjrmcmibe.sHtML

[S20] C：二分查找
来源：http://baike.bbcook.cn/Article/details/glqddjmbt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/gcohreerj.sHtML

[S21] C：字符类别判断
来源：http://wap.sjlbkw.cn/Article/details/gunaveblo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/gdyfoefaj.sHtML

[S22] C：字符串转数字
来源：http://m.share.sjlbkw.cn/Article/details/ghnkssacv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.epnwcf.com/Article/details/gyxervezm.sHtML

[S23] C：随机数
来源：http://read.share.vehdjk.com/Article/details/gmtiwpmxo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.yfazqb.com/Article/details/grlxiqslc.sHtML

[S24] C：获取本地时间
来源：http://mobile.sjlbkw.cn/Article/details/gdmdnrczn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.bbcook.cn/Article/details/gxesanpzj.sHtML

[S25] C：内存拷贝
来源：http://read.share.tarul.cn/Article/details/gxsmhxlgk.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.yfazqb.com/Article/details/gcperhhln.sHtML

[S26] C：内存清零
来源：http://www.blog.epnwcf.com/Article/details/grqnammkx.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.yfazqb.com/Article/details/gpgixdtvg.sHtML

[S27] C：定义常量
来源：http://m.share.tarul.cn/Article/details/gelozfuid.sHtML

const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gwnweptou.sHtML

[S28] C：静态变量
来源：http://www.m.share.vehdjk.com/Article/details/gvcaylxim.sHtML

static int counter = 0;
来源：http://www.m.share.epnwcf.com/Article/details/ggclekljd.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/ghijeewpq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gfvqzqbaf.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/gqmoicnki.sHtML

#ifndef X_H
来源：http://mobile.sjlbkw.cn/Article/details/gxviqoyqp.sHtML

#define X_H
来源：http://wap.yfazqb.com/Article/details/ghkzfbiwj.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gvrkvbpyy.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/gagjkentx.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/gornufzcv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fktsv.cn/Article/details/gjsonfwre.sHtML

[S32] C++：字符串
来源：http://3g.bbcook.cn/Article/details/ghfhyhzla.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.bbcook.cn/Article/details/gntkcpxyd.sHtML

[S33] C++：vector 增删
来源：http://3g.fktsv.cn/Article/details/gmxtatmwk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.bbcook.cn/Article/details/gfxznciwe.sHtML

[S34] C++：遍历 vector
来源：http://blog.bbcook.cn/Article/details/gahoouahv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.tarul.cn/Article/details/gngxrdueq.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/gqqglraub.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gmqmzeyya.sHtML

[S36] C++：unordered_map
来源：http://m.share.bbcook.cn/Article/details/gocqklzok.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/gkkolugrp.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/gaftofzvp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gfvjfsuxa.sHtML

[S38] C++：排序
来源：http://www.m.share.epnwcf.com/Article/details/gmkochxad.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gwqtkovdz.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.sjlbkw.cn/Article/details/gheothyew.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/ghudcpxqp.sHtML

[S40] C++：查找元素
来源：http://baike.sjlbkw.cn/Article/details/geezqipag.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fktsv.cn/Article/details/ghjryocqt.sHtML

[S41] C++：类与构造函数
来源：http://m.share.tarul.cn/Article/details/gwokdqtem.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.vehdjk.com/Article/details/gfaocoqea.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/grvvccahg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.yfazqb.com/Article/details/gurkflxrv.sHtML

[S43] C++：智能指针
来源：http://wap.sjlbkw.cn/Article/details/gzyhkcnma.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.yfazqb.com/Article/details/godzpemag.sHtML

[S44] C++：引用传参
来源：http://read.share.vehdjk.com/Article/details/gtazsuahu.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.epnwcf.com/Article/details/gkvvudjgb.sHtML

[S45] C++：lambda
来源：http://read.share.epnwcf.com/Article/details/gxjglpthh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/gvkynuaoj.sHtML

[S46] C++：函数模板
来源：http://blog.sjlbkw.cn/Article/details/gilsrmhtl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fktsv.cn/Article/details/gljkmlfbh.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.bbcook.cn/Article/details/gbmxgdzoe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.yfazqb.com/Article/details/gmeggolfv.sHtML

[S48] C++：逐行读文件
来源：http://baike.tarul.cn/Article/details/gsoxkeqpo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.sjlbkw.cn/Article/details/gdapjhozw.sHtML

while (std::getline(in, line)) { }
来源：http://blog.tarul.cn/Article/details/glnuciuce.sHtML

[S49] C++：写文件
来源：http://baike.fktsv.cn/Article/details/gkxqvtsxq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.sjlbkw.cn/Article/details/gsrtisfpn.sHtML

[S50] C++：格式化数字
来源：http://mobile.yfazqb.com/Article/details/gbegtwtjs.sHtML


<!-- 参考信息 -->