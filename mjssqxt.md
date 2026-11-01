代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://blog.vehdjk.com/Article/details/gbwuespuf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.yfazqb.com/Article/details/gyhjybxev.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gcepmlwvj.sHtML

[Q89] 判断表是否存在
来源：http://read.share.yfazqb.com/Article/details/gskqtuhzw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.yfazqb.com/Article/details/gsciexqao.sHtML

[Q90] 生成序号列
来源：http://mobile.bbcook.cn/Article/details/gturwhfuo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.vehdjk.com/Article/details/gmooxspgx.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gqpymroho.sHtML

R. Bash 专题
来源：http://mobile.yfazqb.com/Article/details/gzfmktdku.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/glhgtsite.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fktsv.cn/Article/details/guzlegkrr.sHtML

#!/usr/bin/env bash
来源：http://3g.epnwcf.com/Article/details/gzbsukpsi.sHtML

set -euo pipefail
来源：http://www.blog.bbcook.cn/Article/details/gtsmiqtsq.sHtML

[R02] 变量赋值与使用
来源：http://3g.yfazqb.com/Article/details/gmzahrviv.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.epnwcf.com/Article/details/gmlzgziay.sHtML

[R03] 只读变量
来源：http://wap.sjlbkw.cn/Article/details/gfzihrryf.sHtML

readonly PI=3.14
来源：http://blog.bbcook.cn/Article/details/ggxglpoof.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/gtfavikiu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.bbcook.cn/Article/details/gmnkcotjp.sHtML

[R05] 参数默认值
来源：http://3g.epnwcf.com/Article/details/gajqeaaxl.sHtML

name="${1:-default}"
来源：http://read.share.epnwcf.com/Article/details/gnsyritwx.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.epnwcf.com/Article/details/gmbwoemmr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gzhtkkcwt.sHtML

[R07] if 判断文件
来源：http://www.blog.vehdjk.com/Article/details/gcwgwbgpn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fktsv.cn/Article/details/gcktjucqy.sHtML

[R08] 数值比较
来源：http://3g.tarul.cn/Article/details/gfdbiyuat.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gvyncrdbd.sHtML

[R09] 字符串比较
来源：http://mobile.tarul.cn/Article/details/gidbqroku.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.vehdjk.com/Article/details/glscwbnck.sHtML

[R10] 正则匹配
来源：http://www.m.share.epnwcf.com/Article/details/gmcelcnhu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.bbcook.cn/Article/details/gwdhdwzdz.sHtML

[R11] case 多分支
来源：http://www.blog.epnwcf.com/Article/details/gvvuqvipj.sHtML

case "$1" in
来源：http://blog.yfazqb.com/Article/details/gcjxzopcj.sHtML

start) echo "启动" ;;
来源：http://3g.vehdjk.com/Article/details/gpfkqseid.sHtML

stop)  echo "停止" ;;
来源：http://3g.sjlbkw.cn/Article/details/gueqcuyly.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.epnwcf.com/Article/details/gbglmuyom.sHtML

esac
来源：http://wap.sjlbkw.cn/Article/details/gujtlrzli.sHtML

[R12] for 遍历文件
来源：http://wap.vehdjk.com/Article/details/gverwqckr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.epnwcf.com/Article/details/gwdsgzgez.sHtML

[R13] for 计数循环
来源：http://wap.epnwcf.com/Article/details/gnggcygfe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.bbcook.cn/Article/details/gyqosoidt.sHtML

[R14] C 风格 for
来源：http://baike.vehdjk.com/Article/details/garvryykv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gprzjauib.sHtML

[R15] while 逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gpoohxtwh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.sjlbkw.cn/Article/details/gqcxkmnnb.sHtML

[R16] until 等待条件
来源：http://wap.epnwcf.com/Article/details/ghyyzezav.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gypwqcomn.sHtML

[R17] 数组定义与取值
来源：http://3g.yfazqb.com/Article/details/gdbolkkiz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.bbcook.cn/Article/details/gpzwzoyzw.sHtML

[R18] 遍历数组
来源：http://www.m.share.fktsv.cn/Article/details/gqhzdbzaz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.tarul.cn/Article/details/ghpadexof.sHtML

[R19] 数组长度
来源：http://m.share.fktsv.cn/Article/details/gmdagsrbs.sHtML

echo "${#arr[@]}"
来源：http://www.blog.yfazqb.com/Article/details/gqcwexoel.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.bbcook.cn/Article/details/gwncyuuea.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.yfazqb.com/Article/details/ghnbgnihc.sHtML

[R21] 字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gmmuqnkln.sHtML

echo "${#s}"
来源：http://read.share.fktsv.cn/Article/details/gkxdwbpxg.sHtML

[R22] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gbkyidxwp.sHtML

echo "${s:0:5}"
来源：http://www.share.bbcook.cn/Article/details/gmmmyxcnp.sHtML

[R23] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/goubveszl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.vehdjk.com/Article/details/gjvdkwmlx.sHtML

[R24] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gvsdenlla.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fktsv.cn/Article/details/gnbkgibju.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fktsv.cn/Article/details/gzyshubfo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.sjlbkw.cn/Article/details/gatyndqtb.sHtML

[R26] 命令替换
来源：http://3g.bbcook.cn/Article/details/gchqxcogf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.sjlbkw.cn/Article/details/gcjdlxwyy.sHtML

[R27] 算术展开
来源：http://m.share.tarul.cn/Article/details/gkrswtnvn.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fktsv.cn/Article/details/gkhcixpna.sHtML

[R28] 浮点运算
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjkemqay.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fktsv.cn/Article/details/giijcmbrl.sHtML

[R29] 定义函数
来源：http://baike.bbcook.cn/Article/details/gwtyeckzq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.vehdjk.com/Article/details/glfayhuio.sHtML

[R30] 函数返回状态码
来源：http://www.blog.yfazqb.com/Article/details/gdvsftgyn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.tarul.cn/Article/details/ghakorild.sHtML

[R31] 局部变量
来源：http://m.share.fktsv.cn/Article/details/gsuvelbdm.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fktsv.cn/Article/details/gfgeaioqa.sHtML

[R32] 参数个数校验
来源：http://baike.sjlbkw.cn/Article/details/gszfvvqyn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gkiqtwgzg.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.vehdjk.com/Article/details/gzgppxbcg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.bbcook.cn/Article/details/goswfysxg.sHtML

[R34] 退出时清理
来源：http://mobile.sjlbkw.cn/Article/details/gpajjqqes.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gzblrdpns.sHtML

[R35] 后台执行并等待
来源：http://3g.tarul.cn/Article/details/gjvjyqnkd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.sjlbkw.cn/Article/details/gyjdqofty.sHtML

[R36] 并发执行多个任务
来源：http://www.share.tarul.cn/Article/details/gogdkdajo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.bbcook.cn/Article/details/gexxjniyv.sHtML

[R37] 把输出赋给变量
来源：http://mobile.yfazqb.com/Article/details/grtgylinv.sHtML

files=$(ls -1)
来源：http://m.share.sjlbkw.cn/Article/details/gkqigfgcz.sHtML

[R38] 管道串联
来源：http://read.share.yfazqb.com/Article/details/gwklsnytt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.sjlbkw.cn/Article/details/gyinwlghk.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.yfazqb.com/Article/details/gzuzzsfbj.sHtML

cmd > out.log 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gktbzkaqf.sHtML

[R40] 追加写日志
来源：http://www.blog.vehdjk.com/Article/details/goybscdkr.sHtML

echo "log" >> out.log
来源：http://m.share.fktsv.cn/Article/details/gqccpcywe.sHtML

[R41] 丢弃输出
来源：http://www.m.share.tarul.cn/Article/details/gjnhowdlq.sHtML

cmd >/dev/null 2>&1
来源：http://wap.epnwcf.com/Article/details/gpwsoumkf.sHtML

[R42] 输入重定向
来源：http://read.share.vehdjk.com/Article/details/gdhhnvnho.sHtML

wc -l < a.txt
来源：http://3g.bbcook.cn/Article/details/gtvtzpurh.sHtML

[R43] 按名字查找文件
来源：http://3g.fktsv.cn/Article/details/gtzrzbkpj.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/gifodygbv.sHtML

[R44] 按修改时间查找
来源：http://read.share.epnwcf.com/Article/details/gfirpspai.sHtML

find . -mtime -7 -type f
来源：http://wap.sjlbkw.cn/Article/details/glluvpoyi.sHtML

[R45] 批量删除
来源：http://m.share.sjlbkw.cn/Article/details/gfaupoltz.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.vehdjk.com/Article/details/gdipgphne.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fktsv.cn/Article/details/gotrpzlng.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.tarul.cn/Article/details/grkhpcrih.sHtML

[R47] sed 单行替换
来源：http://wap.vehdjk.com/Article/details/gdzzswaky.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fktsv.cn/Article/details/gjtzxmpkf.sHtML

[R48] awk 取指定列
来源：http://www.blog.vehdjk.com/Article/details/glaqhnwvg.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.yfazqb.com/Article/details/gamopehaf.sHtML

[R49] awk 带条件
来源：http://m.share.yfazqb.com/Article/details/glvkjtzzv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fktsv.cn/Article/details/ggkhppgvx.sHtML

[R50] awk 求和
来源：http://3g.bbcook.cn/Article/details/gsdtnbqwj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gvzgopjud.sHtML

[R51] 排序去重取前几
来源：http://www.blog.vehdjk.com/Article/details/gutulghxc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.bbcook.cn/Article/details/gbwspfgph.sHtML

[R52] 统计行数
来源：http://wap.sjlbkw.cn/Article/details/gqmsaljlb.sHtML

wc -l a.txt
来源：http://read.share.tarul.cn/Article/details/gbxcuamkv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.tarul.cn/Article/details/gquvkifcw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.epnwcf.com/Article/details/gabkjwbrh.sHtML

[R54] 比较两个文件
来源：http://mobile.vehdjk.com/Article/details/gijgpzfcw.sHtML

diff a.txt b.txt
来源：http://www.share.bbcook.cn/Article/details/gsrehtmxc.sHtML

[R55] 压缩与解压
来源：http://blog.vehdjk.com/Article/details/gbjoyumwc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.tarul.cn/Article/details/gjdzexgoq.sHtML

[R56] 远程拷贝
来源：http://blog.bbcook.cn/Article/details/gtgbqzkvj.sHtML

scp file user@host:/path/
来源：http://www.share.sjlbkw.cn/Article/details/gohvsujtr.sHtML

[R57] 远程执行命令
来源：http://read.share.tarul.cn/Article/details/gkhsriybd.sHtML

ssh user@host 'uptime'
来源：http://baike.epnwcf.com/Article/details/gpzgrciek.sHtML

[R58] 下载文件
来源：http://blog.epnwcf.com/Article/details/gyicpgzdh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/gixrwkrjb.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gkkdasrew.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.tarul.cn/Article/details/gbxdtbceq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gbteoimbn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fktsv.cn/Article/details/gaqnsmecj.sHtML

[R61] 磁盘占用
来源：http://mobile.bbcook.cn/Article/details/gyywozruk.sHtML

df -h;  du -sh *
来源：http://blog.vehdjk.com/Article/details/gcrjrfxnf.sHtML

[R62] 找最占空间的文件
来源：http://wap.sjlbkw.cn/Article/details/gbhhfzdwm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.yfazqb.com/Article/details/glkjyvnoi.sHtML

[R63] 内存与进程
来源：http://mobile.epnwcf.com/Article/details/gnvvzfvqw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/gwaeehxxi.sHtML

[R64] 结束进程
来源：http://blog.fktsv.cn/Article/details/ghdjbhkmy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.bbcook.cn/Article/details/gthkiacoo.sHtML

[R65] 查看端口占用
来源：http://blog.tarul.cn/Article/details/gjcthixae.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fktsv.cn/Article/details/gtpdjihfa.sHtML

[R66] 定时任务
来源：http://blog.tarul.cn/Article/details/gjkwtepaw.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/gynupgsad.sHtML

[R67] 生成随机十六进制串
来源：http://3g.bbcook.cn/Article/details/gzuuqesnm.sHtML

openssl rand -hex 16
来源：http://read.share.vehdjk.com/Article/details/gyuxhpfpn.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.tarul.cn/Article/details/gthkgzmdh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gvkalcfdz.sHtML

[R69] 生成随机密码
来源：http://www.m.share.vehdjk.com/Article/details/glyxavada.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.bbcook.cn/Article/details/gwhofalwa.sHtML

[R70] 时间戳与互转
来源：http://baike.epnwcf.com/Article/details/grxijgqyx.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.epnwcf.com/Article/details/gmyobytnb.sHtML

[R71] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/gdmuisyrw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.sjlbkw.cn/Article/details/gywggkzte.sHtML

[R72] 等待端口就绪
来源：http://3g.yfazqb.com/Article/details/gkvmpthbh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/ghrcchozi.sHtML

[R73] 分割大日志
来源：http://read.share.bbcook.cn/Article/details/gajoichve.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/gomnxpucx.sHtML

[R74] 批量重命名
来源：http://read.share.sjlbkw.cn/Article/details/gxkpremil.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.epnwcf.com/Article/details/grpwuxgfj.sHtML

[R75] 导出环境变量
来源：http://wap.yfazqb.com/Article/details/gvchutmlt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.tarul.cn/Article/details/gqxmormla.sHtML

[R76] 使用临时文件
来源：http://blog.tarul.cn/Article/details/ggmnzhhud.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/gaolyktta.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gcarrmkrr.sHtML

read -rp "请输入: " ans
来源：http://read.share.sjlbkw.cn/Article/details/gfgdnushx.sHtML

[R78] 交互式菜单
来源：http://www.blog.epnwcf.com/Article/details/gvczzltzg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.vehdjk.com/Article/details/gtjlvumhi.sHtML

[R79] 解析命令行选项
来源：http://baike.bbcook.cn/Article/details/gveikjvoa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.yfazqb.com/Article/details/goycztesz.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.bbcook.cn/Article/details/gokfpgypd.sHtML

time ./run.sh
来源：http://www.blog.tarul.cn/Article/details/gjtyvaosf.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmobxfiui.sHtML

S. C / C++ 专题
来源：http://read.share.yfazqb.com/Article/details/ghppkgfjr.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gephoyqqj.sHtML

[S01] C：Hello World
来源：http://read.share.vehdjk.com/Article/details/gegnxonox.sHtML

#include <stdio.h>
来源：http://www.share.sjlbkw.cn/Article/details/gwwtevrdy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.tarul.cn/Article/details/giycmdogg.sHtML

[S02] C：变量与格式化输出
来源：http://3g.yfazqb.com/Article/details/ggnbbcqyo.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.sjlbkw.cn/Article/details/gaplorsng.sHtML

[S03] C：读入整数
来源：http://www.m.share.vehdjk.com/Article/details/gnfkcdzpc.sHtML

int x; scanf("%d", &x);
来源：http://m.share.bbcook.cn/Article/details/gbbgwcptc.sHtML

[S04] C：字符串复制
来源：http://wap.fktsv.cn/Article/details/gmeamlyim.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.tarul.cn/Article/details/gvpkpjgle.sHtML

[S05] C：字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gwikeoagq.sHtML

strlen(s)
来源：http://wap.bbcook.cn/Article/details/gzfkoujxh.sHtML

[S06] C：字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/guywlnvvm.sHtML

strcmp(a, b) == 0
来源：http://3g.fktsv.cn/Article/details/gttfsaoqq.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.sjlbkw.cn/Article/details/grtcuoihx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/gmknulpaw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.epnwcf.com/Article/details/gvgxmyidg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.epnwcf.com/Article/details/gyeyeeycc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.epnwcf.com/Article/details/gljvyzmgt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fktsv.cn/Article/details/gieyfujdx.sHtML

[S10] C：指针与解引用
来源：http://blog.yfazqb.com/Article/details/gqrjokykk.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.bbcook.cn/Article/details/gnhnkvfmr.sHtML

[S11] C：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/glctwzyno.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fktsv.cn/Article/details/groivzrva.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.yfazqb.com/Article/details/ghdgxgylz.sHtML

fclose(f);
来源：http://m.share.fktsv.cn/Article/details/gxkqrwzjg.sHtML

[S12] C：写文件
来源：http://read.share.bbcook.cn/Article/details/gedpfrdrj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/gngmykilh.sHtML

[S13] C：宏定义
来源：http://www.share.yfazqb.com/Article/details/gycdbkaue.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.vehdjk.com/Article/details/gyukkpstu.sHtML

[S14] C：枚举
来源：http://m.share.sjlbkw.cn/Article/details/gmxgkrksu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.yfazqb.com/Article/details/gspxbebwh.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/gxogclxmk.sHtML

(double) a / b
来源：http://blog.fktsv.cn/Article/details/gigquqsxj.sHtML

[S16] C：位操作置位
来源：http://read.share.epnwcf.com/Article/details/gmputtfdc.sHtML

x |= (1 << 3);
来源：http://read.share.yfazqb.com/Article/details/gpupdkaki.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gaopqaeho.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.sjlbkw.cn/Article/details/gsuvfhdhn.sHtML

[S18] C：命令行参数
来源：http://baike.epnwcf.com/Article/details/gnwohkvsk.sHtML

int main(int argc, char **argv)
来源：http://wap.epnwcf.com/Article/details/gtxavaxsf.sHtML

[S19] C：快速排序
来源：http://wap.yfazqb.com/Article/details/gkibihacd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/gnhpqnzjk.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/gxlwfwtrk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gdfcvfole.sHtML

[S21] C：字符类别判断
来源：http://www.blog.vehdjk.com/Article/details/govziyjme.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.epnwcf.com/Article/details/gstobvyaz.sHtML

[S22] C：字符串转数字
来源：http://baike.vehdjk.com/Article/details/gpsxjthop.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fktsv.cn/Article/details/gavivecma.sHtML

[S23] C：随机数
来源：http://3g.tarul.cn/Article/details/gufzucxuu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fktsv.cn/Article/details/gynlamnjx.sHtML

[S24] C：获取本地时间
来源：http://3g.yfazqb.com/Article/details/gepxqvpdq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.tarul.cn/Article/details/gupftytvi.sHtML

[S25] C：内存拷贝
来源：http://read.share.tarul.cn/Article/details/gbonyoypn.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gzebpasqn.sHtML

[S26] C：内存清零
来源：http://read.share.yfazqb.com/Article/details/ghgnvykra.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.bbcook.cn/Article/details/gxvpjmscx.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/goiytvreg.sHtML

const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gvazjblqt.sHtML

[S28] C：静态变量
来源：http://www.share.vehdjk.com/Article/details/ghlnztpyy.sHtML

static int counter = 0;
来源：http://mobile.vehdjk.com/Article/details/gkvhqarux.sHtML

[S29] C：变参函数
来源：http://read.share.yfazqb.com/Article/details/gnveqidcb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gjnjpwbpw.sHtML

[S30] C：头文件保护
来源：http://mobile.fktsv.cn/Article/details/gyedklopr.sHtML

#ifndef X_H
来源：http://www.share.fktsv.cn/Article/details/gqhslnhuq.sHtML

#define X_H
来源：http://www.share.bbcook.cn/Article/details/ggaujgztp.sHtML

#endif
来源：http://mobile.vehdjk.com/Article/details/gozdenvmt.sHtML

[S31] C++：Hello World
来源：http://baike.epnwcf.com/Article/details/gnnaeuqqe.sHtML

#include <iostream>
来源：http://3g.tarul.cn/Article/details/gfqmkvqre.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.yfazqb.com/Article/details/gagaxphln.sHtML

[S32] C++：字符串
来源：http://baike.fktsv.cn/Article/details/gqaprpjbu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fktsv.cn/Article/details/gntyoomiq.sHtML

[S33] C++：vector 增删
来源：http://www.share.yfazqb.com/Article/details/gdxoxsvgs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.bbcook.cn/Article/details/gbvpvkily.sHtML

[S34] C++：遍历 vector
来源：http://baike.fktsv.cn/Article/details/gbqxqptwj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gnfcwxafz.sHtML

[S35] C++：map
来源：http://www.m.share.yfazqb.com/Article/details/gixdghbqy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gzxnpyric.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.epnwcf.com/Article/details/gmkbxeusx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/goeapskve.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/guycorgra.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.sjlbkw.cn/Article/details/gqqbkspiu.sHtML

[S38] C++：排序
来源：http://m.share.sjlbkw.cn/Article/details/gqbndmxxo.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.sjlbkw.cn/Article/details/genyqabrr.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/gzqkmsfde.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/gtyskopbl.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/glajqubrw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.tarul.cn/Article/details/ghmnfiljb.sHtML

[S41] C++：类与构造函数
来源：http://mobile.epnwcf.com/Article/details/gbuqjenyr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.tarul.cn/Article/details/glkmubhnd.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/gxcafegri.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.bbcook.cn/Article/details/gzbifdxsm.sHtML

[S43] C++：智能指针
来源：http://baike.tarul.cn/Article/details/ghsaxffsp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.sjlbkw.cn/Article/details/gzthnchmd.sHtML

[S44] C++：引用传参
来源：http://3g.bbcook.cn/Article/details/ggvjnzwgu.sHtML

void inc(int &x) { ++x; }
来源：http://baike.yfazqb.com/Article/details/gqgiikpsd.sHtML

[S45] C++：lambda
来源：http://blog.tarul.cn/Article/details/gvutxoiwe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.epnwcf.com/Article/details/gtlhfenue.sHtML

[S46] C++：函数模板
来源：http://wap.epnwcf.com/Article/details/gyeojogdz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvinxzhni.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.vehdjk.com/Article/details/ghytxifry.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.bbcook.cn/Article/details/gmnlacaas.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gixpmwphu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fktsv.cn/Article/details/gmgpftnxz.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.sjlbkw.cn/Article/details/ghxkmeudg.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/gwavwvrlp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.bbcook.cn/Article/details/gngphqheq.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/ggkgmwaqj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/ghomiytbt.sHtML

[S51] C++：显式类型转换
来源：http://read.share.vehdjk.com/Article/details/gcgmddiky.sHtML

static_cast<double>(a) / b
来源：http://www.share.epnwcf.com/Article/details/gmtwuqzjf.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.tarul.cn/Article/details/gfrcboait.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fktsv.cn/Article/details/gguawoyvu.sHtML

[S53] C++：移动语义
来源：http://baike.fktsv.cn/Article/details/goqwqojom.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.bbcook.cn/Article/details/gccbxazsu.sHtML

[S54] C++：异常处理
来源：http://m.share.epnwcf.com/Article/details/gazqnvruf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.bbcook.cn/Article/details/gralheemz.sHtML

[S55] C++：结构化绑定
来源：http://wap.epnwcf.com/Article/details/gvbaexnzt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.epnwcf.com/Article/details/gtbfuuhwr.sHtML

[S56] C++：optional
来源：http://www.m.share.tarul.cn/Article/details/galnotwtw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.tarul.cn/Article/details/glssujcgs.sHtML

[S57] C++：编译期常量
来源：http://read.share.bbcook.cn/Article/details/gorfmnfii.sHtML

constexpr int N = 10;
来源：http://www.share.fktsv.cn/Article/details/gvmetuwkk.sHtML

[S58] C++：命名空间
来源：http://www.m.share.vehdjk.com/Article/details/ghsxexqhk.sHtML


<!-- 参考信息 -->