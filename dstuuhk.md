代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://m.share.yfazqb.com/Article/details/guhvtjrqb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fktsv.cn/Article/details/gzmysrzwc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.epnwcf.com/Article/details/gdlspehoe.sHtML

[Q89] 判断表是否存在
来源：http://m.share.bbcook.cn/Article/details/gllavsmxc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.yfazqb.com/Article/details/grgoubyvs.sHtML

[Q90] 生成序号列
来源：http://mobile.tarul.cn/Article/details/genfxugco.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.yfazqb.com/Article/details/gpqspqjpo.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gcedbknlz.sHtML

R. Bash 专题
来源：http://baike.sjlbkw.cn/Article/details/gtlquzexi.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gyijqrujs.sHtML

[R01] shebang 与严格模式
来源：http://mobile.sjlbkw.cn/Article/details/gwcffltbe.sHtML

#!/usr/bin/env bash
来源：http://3g.tarul.cn/Article/details/gjnwjsbvk.sHtML

set -euo pipefail
来源：http://3g.epnwcf.com/Article/details/gkgwxwslk.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.bbcook.cn/Article/details/gliguigis.sHtML

name="Tom"; echo "$name"
来源：http://m.share.bbcook.cn/Article/details/gisbcqrlo.sHtML

[R03] 只读变量
来源：http://mobile.epnwcf.com/Article/details/gzhoqwrkt.sHtML

readonly PI=3.14
来源：http://3g.vehdjk.com/Article/details/gnmoupngz.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/gmjeuszwz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.bbcook.cn/Article/details/gqwwategm.sHtML

[R05] 参数默认值
来源：http://www.m.share.fktsv.cn/Article/details/ggadreohh.sHtML

name="${1:-default}"
来源：http://3g.epnwcf.com/Article/details/gaacasyen.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fktsv.cn/Article/details/gnqkrmscb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.yfazqb.com/Article/details/gruysmonl.sHtML

[R07] if 判断文件
来源：http://blog.bbcook.cn/Article/details/gwcgtvciq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.yfazqb.com/Article/details/ggzdqsdqn.sHtML

[R08] 数值比较
来源：http://www.blog.epnwcf.com/Article/details/gzbywqrxv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.vehdjk.com/Article/details/gvgrcvihh.sHtML

[R09] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gwezuuxsu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgffmwdb.sHtML

[R10] 正则匹配
来源：http://www.share.vehdjk.com/Article/details/gwhuujtiz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gowowqsry.sHtML

[R11] case 多分支
来源：http://www.m.share.bbcook.cn/Article/details/gflognlap.sHtML

case "$1" in
来源：http://www.share.epnwcf.com/Article/details/ggafjlvco.sHtML

start) echo "启动" ;;
来源：http://blog.yfazqb.com/Article/details/gughzmlmm.sHtML

stop)  echo "停止" ;;
来源：http://wap.vehdjk.com/Article/details/gwojtujhz.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.epnwcf.com/Article/details/gcayvpmkr.sHtML

esac
来源：http://blog.vehdjk.com/Article/details/geqpbltkf.sHtML

[R12] for 遍历文件
来源：http://www.share.vehdjk.com/Article/details/gcdilzubq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.bbcook.cn/Article/details/gwpofhuma.sHtML

[R13] for 计数循环
来源：http://baike.bbcook.cn/Article/details/gjwmnlokb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/godzvtzpt.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/gtzrpvymy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gqzwghoip.sHtML

[R15] while 逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gcylngmhz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fktsv.cn/Article/details/gdtsnvlyy.sHtML

[R16] until 等待条件
来源：http://www.blog.yfazqb.com/Article/details/gflcybncr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gfjazasye.sHtML

[R17] 数组定义与取值
来源：http://m.share.vehdjk.com/Article/details/gnufiruhq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.epnwcf.com/Article/details/gsxbypesu.sHtML

[R18] 遍历数组
来源：http://www.m.share.epnwcf.com/Article/details/gdqklevcn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.sjlbkw.cn/Article/details/girapasov.sHtML

[R19] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gfzovybht.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/gvlyhgofv.sHtML

[R20] 关联数组（字典）
来源：http://mobile.epnwcf.com/Article/details/gxwovcbpg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.tarul.cn/Article/details/gtsflpgnn.sHtML

[R21] 字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gtngoaisp.sHtML

echo "${#s}"
来源：http://read.share.fktsv.cn/Article/details/gnpixfgfk.sHtML

[R22] 截取子串
来源：http://mobile.vehdjk.com/Article/details/gkmysfvio.sHtML

echo "${s:0:5}"
来源：http://m.share.tarul.cn/Article/details/gihkrbzlp.sHtML

[R23] 字符串替换
来源：http://3g.bbcook.cn/Article/details/gtqflvxpe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.epnwcf.com/Article/details/ggfqfhjtz.sHtML

[R24] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/gnfratfcq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.vehdjk.com/Article/details/gypkphgaf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.epnwcf.com/Article/details/gyymihvev.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.vehdjk.com/Article/details/garrwoyqc.sHtML

[R26] 命令替换
来源：http://read.share.bbcook.cn/Article/details/gsodocodx.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.yfazqb.com/Article/details/ghqlsemgw.sHtML

[R27] 算术展开
来源：http://www.share.vehdjk.com/Article/details/gbjyijleh.sHtML

echo $((1 + 2 * 3))
来源：http://baike.yfazqb.com/Article/details/gjdqrpxjr.sHtML

[R28] 浮点运算
来源：http://www.share.tarul.cn/Article/details/guxqjjqwy.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.epnwcf.com/Article/details/gnsdtkxcl.sHtML

[R29] 定义函数
来源：http://wap.bbcook.cn/Article/details/gcjajigni.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.sjlbkw.cn/Article/details/gmabqnnwt.sHtML

[R30] 函数返回状态码
来源：http://www.blog.yfazqb.com/Article/details/gwgluqwlk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.vehdjk.com/Article/details/gfsoqzhhk.sHtML

[R31] 局部变量
来源：http://wap.tarul.cn/Article/details/gqirwwkxl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.bbcook.cn/Article/details/gwzsakdvj.sHtML

[R32] 参数个数校验
来源：http://www.blog.tarul.cn/Article/details/gqiylwnda.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gszbhoxjb.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.tarul.cn/Article/details/gifybxghf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.epnwcf.com/Article/details/gypdalouj.sHtML

[R34] 退出时清理
来源：http://read.share.sjlbkw.cn/Article/details/gzwoeihrl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/gycrbgjzl.sHtML

[R35] 后台执行并等待
来源：http://m.share.epnwcf.com/Article/details/gndwqxvbv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.vehdjk.com/Article/details/gvrmpyzqh.sHtML

[R36] 并发执行多个任务
来源：http://3g.fktsv.cn/Article/details/gopscrlvs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.vehdjk.com/Article/details/gmpprpjvb.sHtML

[R37] 把输出赋给变量
来源：http://baike.yfazqb.com/Article/details/gvmsmmalc.sHtML

files=$(ls -1)
来源：http://mobile.vehdjk.com/Article/details/gxkschoix.sHtML

[R38] 管道串联
来源：http://m.share.sjlbkw.cn/Article/details/gubzszadz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.vehdjk.com/Article/details/gtodfftdu.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fktsv.cn/Article/details/gztwpieqh.sHtML

cmd > out.log 2>&1
来源：http://m.share.vehdjk.com/Article/details/giflnjhmt.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/gynidqcir.sHtML

echo "log" >> out.log
来源：http://3g.vehdjk.com/Article/details/ghyzjclcd.sHtML

[R41] 丢弃输出
来源：http://blog.fktsv.cn/Article/details/gcrbpfvdi.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.epnwcf.com/Article/details/gctbkvadf.sHtML

[R42] 输入重定向
来源：http://blog.fktsv.cn/Article/details/gtkricltb.sHtML

wc -l < a.txt
来源：http://3g.fktsv.cn/Article/details/grczqmwwo.sHtML

[R43] 按名字查找文件
来源：http://wap.tarul.cn/Article/details/gjskfgoxf.sHtML

find . -name "*.log" -type f
来源：http://3g.tarul.cn/Article/details/gvimjdaxq.sHtML

[R44] 按修改时间查找
来源：http://m.share.epnwcf.com/Article/details/gtwxlanhl.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/gmvzeeruq.sHtML

[R45] 批量删除
来源：http://baike.bbcook.cn/Article/details/gvavvoljt.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.epnwcf.com/Article/details/gmupfnpxx.sHtML

[R46] 递归替换文件内容
来源：http://read.share.sjlbkw.cn/Article/details/gsnehumtr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.tarul.cn/Article/details/gdpbjvevo.sHtML

[R47] sed 单行替换
来源：http://3g.fktsv.cn/Article/details/grmlndmgv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.yfazqb.com/Article/details/ginrwjsmp.sHtML

[R48] awk 取指定列
来源：http://www.blog.fktsv.cn/Article/details/grkvkdgda.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.epnwcf.com/Article/details/ggowmmwib.sHtML

[R49] awk 带条件
来源：http://www.blog.vehdjk.com/Article/details/gothetdbk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.yfazqb.com/Article/details/gayzvzktk.sHtML

[R50] awk 求和
来源：http://blog.tarul.cn/Article/details/gdehskzja.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.tarul.cn/Article/details/gpxchcoun.sHtML

[R51] 排序去重取前几
来源：http://www.share.tarul.cn/Article/details/gjopbfree.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.tarul.cn/Article/details/gaonmrrir.sHtML

[R52] 统计行数
来源：http://blog.yfazqb.com/Article/details/gnyinksgg.sHtML

wc -l a.txt
来源：http://baike.vehdjk.com/Article/details/gbywqncuk.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fktsv.cn/Article/details/grjxlvwph.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.yfazqb.com/Article/details/gsybwsdrk.sHtML

[R54] 比较两个文件
来源：http://baike.tarul.cn/Article/details/gjmsoyjfo.sHtML

diff a.txt b.txt
来源：http://www.blog.bbcook.cn/Article/details/gjrgmapzl.sHtML

[R55] 压缩与解压
来源：http://wap.yfazqb.com/Article/details/grvdvtecv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fktsv.cn/Article/details/gybqidhhz.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/giizuooft.sHtML

scp file user@host:/path/
来源：http://blog.epnwcf.com/Article/details/gxeoehnwb.sHtML

[R57] 远程执行命令
来源：http://3g.epnwcf.com/Article/details/gargdzrdy.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.epnwcf.com/Article/details/gqoishduj.sHtML

[R58] 下载文件
来源：http://mobile.fktsv.cn/Article/details/gmvjiyqse.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.tarul.cn/Article/details/gbclxdpiz.sHtML

[R59] 发 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gskmrkdnq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/gqxmrqljv.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/gpdknvnfh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/gatkipxan.sHtML

[R61] 磁盘占用
来源：http://www.blog.vehdjk.com/Article/details/gwfmisnzw.sHtML

df -h;  du -sh *
来源：http://3g.bbcook.cn/Article/details/gheatyiap.sHtML

[R62] 找最占空间的文件
来源：http://baike.yfazqb.com/Article/details/goibvqgaz.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.sjlbkw.cn/Article/details/gdfjejnps.sHtML

[R63] 内存与进程
来源：http://www.share.epnwcf.com/Article/details/gdqhkgirs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.sjlbkw.cn/Article/details/gabvgghik.sHtML

[R64] 结束进程
来源：http://blog.bbcook.cn/Article/details/gyfbnsfxj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.epnwcf.com/Article/details/ggrfssqlb.sHtML

[R65] 查看端口占用
来源：http://mobile.tarul.cn/Article/details/guxbujumv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.tarul.cn/Article/details/guephxofj.sHtML

[R66] 定时任务
来源：http://www.share.yfazqb.com/Article/details/gretgvfyn.sHtML

crontab -e;  crontab -l
来源：http://mobile.epnwcf.com/Article/details/gnvjlbtyn.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/ghphkarwj.sHtML

openssl rand -hex 16
来源：http://www.m.share.tarul.cn/Article/details/geqxvigax.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/gxwybvkdk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.tarul.cn/Article/details/goidnrxfw.sHtML

[R69] 生成随机密码
来源：http://wap.bbcook.cn/Article/details/gkisuibtw.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.yfazqb.com/Article/details/gjukjvlvd.sHtML

[R70] 时间戳与互转
来源：http://3g.epnwcf.com/Article/details/gjdkpziot.sHtML

date +%s;  date -d @1700000000
来源：http://3g.sjlbkw.cn/Article/details/gqlpacwyd.sHtML

[R71] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/gbcpctdbz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.yfazqb.com/Article/details/gvcdymlph.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.bbcook.cn/Article/details/gvxyzbvhw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gvhkpisav.sHtML

[R73] 分割大日志
来源：http://read.share.bbcook.cn/Article/details/gagdrceds.sHtML

split -l 1000 big.log part_
来源：http://wap.yfazqb.com/Article/details/gytmnnyvu.sHtML

[R74] 批量重命名
来源：http://blog.tarul.cn/Article/details/gjzckhzgi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.vehdjk.com/Article/details/gkvlcmelb.sHtML

[R75] 导出环境变量
来源：http://wap.tarul.cn/Article/details/gidmetbkf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.sjlbkw.cn/Article/details/gwngpxbva.sHtML

[R76] 使用临时文件
来源：http://baike.vehdjk.com/Article/details/getlidabq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gbqylqafl.sHtML

[R77] 读取用户输入
来源：http://www.m.share.sjlbkw.cn/Article/details/gekxbnpmt.sHtML

read -rp "请输入: " ans
来源：http://3g.yfazqb.com/Article/details/gplcyngxl.sHtML

[R78] 交互式菜单
来源：http://wap.sjlbkw.cn/Article/details/glpqfotdh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.yfazqb.com/Article/details/gvlnebczw.sHtML

[R79] 解析命令行选项
来源：http://wap.tarul.cn/Article/details/ghtrxtuxe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.sjlbkw.cn/Article/details/grvwknzra.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.sjlbkw.cn/Article/details/gntqkslbf.sHtML

time ./run.sh
来源：http://blog.epnwcf.com/Article/details/gcartypje.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gpvmsxqoh.sHtML

S. C / C++ 专题
来源：http://wap.bbcook.cn/Article/details/gviuhphgi.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gscvglokv.sHtML

[S01] C：Hello World
来源：http://baike.tarul.cn/Article/details/gkjojgihe.sHtML

#include <stdio.h>
来源：http://www.share.yfazqb.com/Article/details/gxnrvcoyb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.tarul.cn/Article/details/gxqzqdwjh.sHtML

[S02] C：变量与格式化输出
来源：http://3g.bbcook.cn/Article/details/grhpqcilq.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/gdnhuigot.sHtML

[S03] C：读入整数
来源：http://read.share.epnwcf.com/Article/details/gjxijsquw.sHtML

int x; scanf("%d", &x);
来源：http://read.share.tarul.cn/Article/details/gfkylroth.sHtML

[S04] C：字符串复制
来源：http://www.share.epnwcf.com/Article/details/gbkvmzuhh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fktsv.cn/Article/details/gxqigsflt.sHtML

[S05] C：字符串长度
来源：http://baike.vehdjk.com/Article/details/gpmbwqxud.sHtML

strlen(s)
来源：http://www.share.vehdjk.com/Article/details/gqebjelpz.sHtML

[S06] C：字符串比较
来源：http://www.share.bbcook.cn/Article/details/gncichrmi.sHtML

strcmp(a, b) == 0
来源：http://www.blog.bbcook.cn/Article/details/gnnbqpwbi.sHtML

[S07] C：数组遍历求和
来源：http://wap.vehdjk.com/Article/details/gwofwmvay.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.epnwcf.com/Article/details/gfpdteflr.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.yfazqb.com/Article/details/gqknltnam.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.sjlbkw.cn/Article/details/gujchrkpx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fktsv.cn/Article/details/gfulkmslf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.epnwcf.com/Article/details/gvdmlggbz.sHtML

[S10] C：指针与解引用
来源：http://read.share.vehdjk.com/Article/details/gfdbmrxab.sHtML

int *p = &a;  *p = 5;
来源：http://3g.bbcook.cn/Article/details/gmfayoftq.sHtML

[S11] C：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gfmilqbtj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.tarul.cn/Article/details/gfihkpumj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.bbcook.cn/Article/details/gljqojnrj.sHtML

fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gstxursij.sHtML

[S12] C：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gjzbetvab.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.epnwcf.com/Article/details/grytdllgu.sHtML

[S13] C：宏定义
来源：http://3g.sjlbkw.cn/Article/details/gvzyhuhfx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.sjlbkw.cn/Article/details/geqjnotfn.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/gdjptyndf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.bbcook.cn/Article/details/gqzkqvjcc.sHtML

[S15] C：类型转换
来源：http://www.share.fktsv.cn/Article/details/gbkpimunc.sHtML

(double) a / b
来源：http://m.share.sjlbkw.cn/Article/details/gpunaghld.sHtML

[S16] C：位操作置位
来源：http://read.share.fktsv.cn/Article/details/gfdxgyifl.sHtML

x |= (1 << 3);
来源：http://3g.tarul.cn/Article/details/gjwnwweli.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gmqzhtxag.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.bbcook.cn/Article/details/gghuagsmk.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlkncvkc.sHtML

int main(int argc, char **argv)
来源：http://mobile.tarul.cn/Article/details/glgtxsrkm.sHtML

[S19] C：快速排序
来源：http://baike.bbcook.cn/Article/details/gnsjqjjid.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gczuwwkxl.sHtML

[S20] C：二分查找
来源：http://m.share.bbcook.cn/Article/details/gsejsxruu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/giurhfyle.sHtML

[S21] C：字符类别判断
来源：http://mobile.sjlbkw.cn/Article/details/gnubnwdmf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.yfazqb.com/Article/details/gdgukeasc.sHtML

[S22] C：字符串转数字
来源：http://blog.yfazqb.com/Article/details/ggpbrhayl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.yfazqb.com/Article/details/ggewrbuns.sHtML

[S23] C：随机数
来源：http://www.share.vehdjk.com/Article/details/gbccrmdeb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.sjlbkw.cn/Article/details/gsngfuapm.sHtML

[S24] C：获取本地时间
来源：http://read.share.vehdjk.com/Article/details/gysrghwjw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fktsv.cn/Article/details/gnlpdgwam.sHtML

[S25] C：内存拷贝
来源：http://read.share.epnwcf.com/Article/details/guzotcwsg.sHtML

memcpy(dst, src, n);
来源：http://www.share.bbcook.cn/Article/details/gosdfuvuc.sHtML

[S26] C：内存清零
来源：http://m.share.bbcook.cn/Article/details/ghykzsjlx.sHtML

memset(a, 0, sizeof a);
来源：http://blog.bbcook.cn/Article/details/gopamiaea.sHtML

[S27] C：定义常量
来源：http://blog.epnwcf.com/Article/details/gshyvucxv.sHtML

const double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gfburldry.sHtML

[S28] C：静态变量
来源：http://www.m.share.yfazqb.com/Article/details/gyqdaklkz.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/gmlmslkts.sHtML

[S29] C：变参函数
来源：http://www.blog.vehdjk.com/Article/details/gpotetvlt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.vehdjk.com/Article/details/guchxzfpf.sHtML

[S30] C：头文件保护
来源：http://baike.fktsv.cn/Article/details/gnfjsqnhc.sHtML

#ifndef X_H
来源：http://m.share.fktsv.cn/Article/details/gfhsgmawu.sHtML

#define X_H
来源：http://www.blog.vehdjk.com/Article/details/ghchecflh.sHtML

#endif
来源：http://www.m.share.bbcook.cn/Article/details/gsqircfuy.sHtML

[S31] C++：Hello World
来源：http://3g.vehdjk.com/Article/details/gfjgpfbrk.sHtML

#include <iostream>
来源：http://m.share.vehdjk.com/Article/details/gjhugiqrn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fktsv.cn/Article/details/ghbsjruyr.sHtML

[S32] C++：字符串
来源：http://baike.epnwcf.com/Article/details/girhcsfte.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fktsv.cn/Article/details/grbteixzi.sHtML

[S33] C++：vector 增删
来源：http://blog.epnwcf.com/Article/details/gbmynfijj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.epnwcf.com/Article/details/gavfzporf.sHtML

[S34] C++：遍历 vector
来源：http://read.share.yfazqb.com/Article/details/gaafhjwwm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.epnwcf.com/Article/details/gsmoctlnf.sHtML

[S35] C++：map
来源：http://read.share.vehdjk.com/Article/details/gsgrbdfmn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/geiofvtwx.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.yfazqb.com/Article/details/gupabphep.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gnmmsotec.sHtML

[S37] C++：set
来源：http://m.share.vehdjk.com/Article/details/gfxcsovpu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.epnwcf.com/Article/details/gxubzpadp.sHtML

[S38] C++：排序
来源：http://www.blog.yfazqb.com/Article/details/gccfmwzis.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gtyustjte.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fktsv.cn/Article/details/gmdcfauwr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.sjlbkw.cn/Article/details/gpdveosfd.sHtML

[S40] C++：查找元素
来源：http://m.share.epnwcf.com/Article/details/gvghuftwl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/gwzozqkzs.sHtML

[S41] C++：类与构造函数
来源：http://m.share.bbcook.cn/Article/details/geaptivje.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.tarul.cn/Article/details/gqsyumonw.sHtML

[S42] C++：继承与虚函数
来源：http://baike.sjlbkw.cn/Article/details/gtullokaw.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.vehdjk.com/Article/details/ghpurqnsp.sHtML

[S43] C++：智能指针
来源：http://www.share.vehdjk.com/Article/details/gxitrrtex.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.yfazqb.com/Article/details/geypruuib.sHtML

[S44] C++：引用传参
来源：http://www.m.share.vehdjk.com/Article/details/gqghdfnaa.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.sjlbkw.cn/Article/details/gphbbzacb.sHtML

[S45] C++：lambda
来源：http://www.m.share.vehdjk.com/Article/details/gsqjumrui.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fktsv.cn/Article/details/giahpilqp.sHtML

[S46] C++：函数模板
来源：http://www.share.vehdjk.com/Article/details/ghgjlyygg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.tarul.cn/Article/details/ggqnulmet.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fktsv.cn/Article/details/gljfhmhnc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.epnwcf.com/Article/details/gbihqrvlb.sHtML

[S48] C++：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gknvwhwaa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.tarul.cn/Article/details/gqctlebmq.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.tarul.cn/Article/details/gannluxzh.sHtML

[S49] C++：写文件
来源：http://3g.tarul.cn/Article/details/gyrrfquce.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.sjlbkw.cn/Article/details/gomxtqqsq.sHtML

[S50] C++：格式化数字
来源：http://3g.vehdjk.com/Article/details/gwxptpuve.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gzrbbqrrr.sHtML

[S51] C++：显式类型转换
来源：http://read.share.vehdjk.com/Article/details/grsettqco.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.vehdjk.com/Article/details/gvsvzznee.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.tarul.cn/Article/details/glkfcwwhi.sHtML

int size() const noexcept { return n_; }
来源：http://blog.tarul.cn/Article/details/gctrivzih.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/gzpexdcpb.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/ghvbvrcuk.sHtML

[S54] C++：异常处理
来源：http://baike.vehdjk.com/Article/details/gaecbzcft.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.tarul.cn/Article/details/ggfounehm.sHtML

[S55] C++：结构化绑定
来源：http://mobile.epnwcf.com/Article/details/gwcmofsat.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.tarul.cn/Article/details/gmvkpnzvo.sHtML

[S56] C++：optional
来源：http://www.share.vehdjk.com/Article/details/gdpddcole.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/gxicultvb.sHtML

[S57] C++：编译期常量
来源：http://www.blog.sjlbkw.cn/Article/details/gqusvtyds.sHtML

constexpr int N = 10;
来源：http://baike.sjlbkw.cn/Article/details/gyxqzbwjv.sHtML

[S58] C++：命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/gfxqbbuzo.sHtML


<!-- 参考信息 -->