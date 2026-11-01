代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.blog.bbcook.cn/Article/details/gacuyjark.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.bbcook.cn/Article/details/glyxrfcfj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.epnwcf.com/Article/details/gwwqxoghe.sHtML

[Q89] 判断表是否存在
来源：http://baike.sjlbkw.cn/Article/details/gvzgbeorv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fktsv.cn/Article/details/gelghrgrw.sHtML

[Q90] 生成序号列
来源：http://3g.yfazqb.com/Article/details/glbcwncon.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.tarul.cn/Article/details/gkgszpvlc.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gmflmfgld.sHtML

R. Bash 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gfooqghoz.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gtktdczwp.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.sjlbkw.cn/Article/details/gyneotowf.sHtML

#!/usr/bin/env bash
来源：http://read.share.bbcook.cn/Article/details/gkihwwjbp.sHtML

set -euo pipefail
来源：http://baike.fktsv.cn/Article/details/gaxztajpa.sHtML

[R02] 变量赋值与使用
来源：http://baike.epnwcf.com/Article/details/gcjqxdbrq.sHtML

name="Tom"; echo "$name"
来源：http://wap.fktsv.cn/Article/details/gwlnwtolq.sHtML

[R03] 只读变量
来源：http://m.share.tarul.cn/Article/details/gmaqwtmkk.sHtML

readonly PI=3.14
来源：http://www.blog.epnwcf.com/Article/details/gijakdmca.sHtML

[R04] 位置参数
来源：http://www.m.share.vehdjk.com/Article/details/gkjxbjwtc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.sjlbkw.cn/Article/details/gwknqzxdf.sHtML

[R05] 参数默认值
来源：http://www.share.sjlbkw.cn/Article/details/gdkibgfgj.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/gdglcsxqx.sHtML

[R06] 判断命令是否存在
来源：http://3g.bbcook.cn/Article/details/gexmgqppq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/galhumrke.sHtML

[R07] if 判断文件
来源：http://read.share.vehdjk.com/Article/details/gltjupzwo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.sjlbkw.cn/Article/details/gqnzstels.sHtML

[R08] 数值比较
来源：http://www.m.share.bbcook.cn/Article/details/gertnfmay.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.vehdjk.com/Article/details/gfsifyaqh.sHtML

[R09] 字符串比较
来源：http://mobile.tarul.cn/Article/details/gphwdsido.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.bbcook.cn/Article/details/gjjmmhktq.sHtML

[R10] 正则匹配
来源：http://blog.fktsv.cn/Article/details/gbgngfsfe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gctzplard.sHtML

[R11] case 多分支
来源：http://blog.tarul.cn/Article/details/ggwyaqmir.sHtML

case "$1" in
来源：http://3g.sjlbkw.cn/Article/details/gpeecqgqk.sHtML

start) echo "启动" ;;
来源：http://baike.fktsv.cn/Article/details/gglhxduxm.sHtML

stop)  echo "停止" ;;
来源：http://www.share.epnwcf.com/Article/details/gterhckcz.sHtML

*)     echo "未知命令" ;;
来源：http://blog.vehdjk.com/Article/details/gzgskvkgg.sHtML

esac
来源：http://www.m.share.epnwcf.com/Article/details/guqzeqjqk.sHtML

[R12] for 遍历文件
来源：http://www.blog.bbcook.cn/Article/details/gtihgzhit.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.yfazqb.com/Article/details/gynsnqmts.sHtML

[R13] for 计数循环
来源：http://www.m.share.sjlbkw.cn/Article/details/giuhycuet.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/grdcjblpu.sHtML

[R14] C 风格 for
来源：http://baike.tarul.cn/Article/details/gtwdccpqb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/goaqopvjr.sHtML

[R15] while 逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gzzguhmzt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.tarul.cn/Article/details/ghnrbmhzu.sHtML

[R16] until 等待条件
来源：http://blog.fktsv.cn/Article/details/ghlkfnayn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/ggeiphbhu.sHtML

[R17] 数组定义与取值
来源：http://m.share.yfazqb.com/Article/details/gggokdaua.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.sjlbkw.cn/Article/details/gxdkrlkys.sHtML

[R18] 遍历数组
来源：http://m.share.sjlbkw.cn/Article/details/gbtbddgfj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.sjlbkw.cn/Article/details/gudgqxkuu.sHtML

[R19] 数组长度
来源：http://www.blog.epnwcf.com/Article/details/guwqjnhdv.sHtML

echo "${#arr[@]}"
来源：http://www.share.bbcook.cn/Article/details/gtcejnudv.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.vehdjk.com/Article/details/gwuiiaovm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/gyqijcjbu.sHtML

[R21] 字符串长度
来源：http://mobile.vehdjk.com/Article/details/gquxlekgm.sHtML

echo "${#s}"
来源：http://www.share.vehdjk.com/Article/details/ghixnsdpc.sHtML

[R22] 截取子串
来源：http://wap.epnwcf.com/Article/details/gbniixyyv.sHtML

echo "${s:0:5}"
来源：http://read.share.tarul.cn/Article/details/gfrwygfov.sHtML

[R23] 字符串替换
来源：http://read.share.tarul.cn/Article/details/gvikzksbc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.yfazqb.com/Article/details/gtrmxwioc.sHtML

[R24] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/goyhepjrw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.bbcook.cn/Article/details/gvphdande.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.vehdjk.com/Article/details/gltesepzp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.yfazqb.com/Article/details/ggmcvzpks.sHtML

[R26] 命令替换
来源：http://blog.yfazqb.com/Article/details/giezwdbyd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.bbcook.cn/Article/details/gagxtgxnx.sHtML

[R27] 算术展开
来源：http://mobile.bbcook.cn/Article/details/gigspjhvi.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.tarul.cn/Article/details/gdciscsun.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/gpyhepnoh.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.yfazqb.com/Article/details/ggpnlaqvm.sHtML

[R29] 定义函数
来源：http://baike.bbcook.cn/Article/details/guubobhep.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.epnwcf.com/Article/details/gnpyphgmg.sHtML

[R30] 函数返回状态码
来源：http://blog.sjlbkw.cn/Article/details/gtrkfalzm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.bbcook.cn/Article/details/gsadrdvdd.sHtML

[R31] 局部变量
来源：http://www.m.share.tarul.cn/Article/details/grurmwpvo.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fktsv.cn/Article/details/guengsspm.sHtML

[R32] 参数个数校验
来源：http://blog.yfazqb.com/Article/details/ggyeqhiun.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/gfqtjraxu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.vehdjk.com/Article/details/gdmwzyvsd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.vehdjk.com/Article/details/govhvkxxz.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/grfjobmqv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/gmtbdeptn.sHtML

[R35] 后台执行并等待
来源：http://read.share.epnwcf.com/Article/details/gjnsnhgxw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fktsv.cn/Article/details/gnomacuev.sHtML

[R36] 并发执行多个任务
来源：http://m.share.epnwcf.com/Article/details/gagtqvgbq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/gkocljtus.sHtML

[R37] 把输出赋给变量
来源：http://3g.sjlbkw.cn/Article/details/gimvhbkia.sHtML

files=$(ls -1)
来源：http://blog.epnwcf.com/Article/details/gawuhucxq.sHtML

[R38] 管道串联
来源：http://baike.yfazqb.com/Article/details/gpsscrtpn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.sjlbkw.cn/Article/details/goxyvzggo.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.vehdjk.com/Article/details/gxanoqbyi.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/glllqkqji.sHtML

[R40] 追加写日志
来源：http://wap.sjlbkw.cn/Article/details/gzeqqgphv.sHtML

echo "log" >> out.log
来源：http://www.m.share.sjlbkw.cn/Article/details/geaxrrqro.sHtML

[R41] 丢弃输出
来源：http://mobile.fktsv.cn/Article/details/gwmpompkp.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fktsv.cn/Article/details/gjzbovuyw.sHtML

[R42] 输入重定向
来源：http://read.share.sjlbkw.cn/Article/details/gookdwxpu.sHtML

wc -l < a.txt
来源：http://mobile.tarul.cn/Article/details/gezelncvr.sHtML

[R43] 按名字查找文件
来源：http://read.share.epnwcf.com/Article/details/gamljpimh.sHtML

find . -name "*.log" -type f
来源：http://m.share.bbcook.cn/Article/details/gketncnfj.sHtML

[R44] 按修改时间查找
来源：http://baike.sjlbkw.cn/Article/details/gikydkjxt.sHtML

find . -mtime -7 -type f
来源：http://www.share.sjlbkw.cn/Article/details/glyipcmmu.sHtML

[R45] 批量删除
来源：http://blog.sjlbkw.cn/Article/details/gzlnrrubt.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/gppuquerq.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fktsv.cn/Article/details/giqbwkdbv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.sjlbkw.cn/Article/details/gfugpdxwd.sHtML

[R47] sed 单行替换
来源：http://www.m.share.bbcook.cn/Article/details/gslgheslq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.vehdjk.com/Article/details/ghhnnytxq.sHtML

[R48] awk 取指定列
来源：http://m.share.epnwcf.com/Article/details/gpcutpbbv.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/ghhplqzeq.sHtML

[R49] awk 带条件
来源：http://mobile.fktsv.cn/Article/details/gapejtnre.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fktsv.cn/Article/details/gfjlcthal.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/gndkaiiwr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gshdeyppz.sHtML

[R51] 排序去重取前几
来源：http://m.share.sjlbkw.cn/Article/details/gfjypjtkt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.vehdjk.com/Article/details/ghbwgyaoo.sHtML

[R52] 统计行数
来源：http://3g.vehdjk.com/Article/details/gquhpaiok.sHtML

wc -l a.txt
来源：http://blog.vehdjk.com/Article/details/grxostvlk.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.bbcook.cn/Article/details/gmwcyalmj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.vehdjk.com/Article/details/gcrfnivil.sHtML

[R54] 比较两个文件
来源：http://read.share.tarul.cn/Article/details/gcgecfxqt.sHtML

diff a.txt b.txt
来源：http://3g.epnwcf.com/Article/details/gammkpchf.sHtML

[R55] 压缩与解压
来源：http://mobile.tarul.cn/Article/details/gstmknnwl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.tarul.cn/Article/details/gpijyfvzp.sHtML

[R56] 远程拷贝
来源：http://mobile.vehdjk.com/Article/details/gsewnjvve.sHtML

scp file user@host:/path/
来源：http://mobile.sjlbkw.cn/Article/details/gzxhkkymq.sHtML

[R57] 远程执行命令
来源：http://m.share.fktsv.cn/Article/details/gmltogoye.sHtML

ssh user@host 'uptime'
来源：http://baike.bbcook.cn/Article/details/gjlakmkww.sHtML

[R58] 下载文件
来源：http://3g.yfazqb.com/Article/details/gzhesrtjl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.epnwcf.com/Article/details/gpiembyyx.sHtML

[R59] 发 POST JSON
来源：http://blog.epnwcf.com/Article/details/gizjfsabp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.yfazqb.com/Article/details/ggggadrqd.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gucsyjcga.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.yfazqb.com/Article/details/grnvtfqcp.sHtML

[R61] 磁盘占用
来源：http://www.blog.yfazqb.com/Article/details/gdccjwdty.sHtML

df -h;  du -sh *
来源：http://baike.sjlbkw.cn/Article/details/gobmtqrzz.sHtML

[R62] 找最占空间的文件
来源：http://www.share.epnwcf.com/Article/details/grvsmdjyb.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.tarul.cn/Article/details/gpcoyrbye.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gchmxdand.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.epnwcf.com/Article/details/gslfdvych.sHtML

[R64] 结束进程
来源：http://wap.vehdjk.com/Article/details/gmedqecpw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.epnwcf.com/Article/details/gkqimvqep.sHtML

[R65] 查看端口占用
来源：http://www.blog.tarul.cn/Article/details/gzuektisa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.epnwcf.com/Article/details/gzwytoalv.sHtML

[R66] 定时任务
来源：http://3g.vehdjk.com/Article/details/gswedfueo.sHtML

crontab -e;  crontab -l
来源：http://wap.fktsv.cn/Article/details/gylbfwxfs.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.yfazqb.com/Article/details/ggqezfxyt.sHtML

openssl rand -hex 16
来源：http://blog.tarul.cn/Article/details/gydatpfes.sHtML

[R68] 计算文件校验值
来源：http://www.blog.epnwcf.com/Article/details/gkrfnppow.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fktsv.cn/Article/details/gdiulzhyi.sHtML

[R69] 生成随机密码
来源：http://baike.vehdjk.com/Article/details/gusynzits.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.sjlbkw.cn/Article/details/gioogtygp.sHtML

[R70] 时间戳与互转
来源：http://mobile.fktsv.cn/Article/details/ggoakguvn.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fktsv.cn/Article/details/gcfajlrbz.sHtML

[R71] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gchsoypvd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.yfazqb.com/Article/details/gfgvctcqu.sHtML

[R72] 等待端口就绪
来源：http://wap.bbcook.cn/Article/details/gcsesszgy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gkkvrhjzv.sHtML

[R73] 分割大日志
来源：http://mobile.tarul.cn/Article/details/gaklfffyv.sHtML

split -l 1000 big.log part_
来源：http://www.blog.epnwcf.com/Article/details/glgrxhuxw.sHtML

[R74] 批量重命名
来源：http://3g.bbcook.cn/Article/details/gakrvhqxt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.sjlbkw.cn/Article/details/gstbibwoq.sHtML

[R75] 导出环境变量
来源：http://www.share.fktsv.cn/Article/details/gnwubblvf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.bbcook.cn/Article/details/gnhrvkelo.sHtML

[R76] 使用临时文件
来源：http://read.share.epnwcf.com/Article/details/gesikxnhj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/gfdstzkhk.sHtML

[R77] 读取用户输入
来源：http://wap.sjlbkw.cn/Article/details/gggbipsva.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/gtcanugtj.sHtML

[R78] 交互式菜单
来源：http://3g.epnwcf.com/Article/details/gqjkwvmcq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/gqcjlyrfq.sHtML

[R79] 解析命令行选项
来源：http://mobile.fktsv.cn/Article/details/ggicsrdzk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdfoiery.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.epnwcf.com/Article/details/gzpbdzgfp.sHtML

time ./run.sh
来源：http://baike.tarul.cn/Article/details/gerukosjk.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvynpchef.sHtML

S. C / C++ 专题
来源：http://www.m.share.vehdjk.com/Article/details/gnttsxpyv.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gzntwfkqb.sHtML

[S01] C：Hello World
来源：http://www.blog.vehdjk.com/Article/details/geymyjrxl.sHtML

#include <stdio.h>
来源：http://blog.yfazqb.com/Article/details/ggeyufcun.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.yfazqb.com/Article/details/gjbsjeqfz.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.tarul.cn/Article/details/gzgvyidgi.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.tarul.cn/Article/details/gfsierzly.sHtML

[S03] C：读入整数
来源：http://wap.bbcook.cn/Article/details/gdisptwuc.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.bbcook.cn/Article/details/gsqvcacom.sHtML

[S04] C：字符串复制
来源：http://www.m.share.bbcook.cn/Article/details/gwgzqqhif.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.yfazqb.com/Article/details/gdnwqufiy.sHtML

[S05] C：字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gflgyjkmp.sHtML

strlen(s)
来源：http://mobile.vehdjk.com/Article/details/gymeaviff.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/goakmvdie.sHtML

strcmp(a, b) == 0
来源：http://m.share.epnwcf.com/Article/details/gkjkpxbii.sHtML

[S07] C：数组遍历求和
来源：http://www.share.yfazqb.com/Article/details/gaqxzaotp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.bbcook.cn/Article/details/gczojhjcs.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.tarul.cn/Article/details/gqikrmfkf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.epnwcf.com/Article/details/ghmbfqexj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fktsv.cn/Article/details/gffoplkzp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.tarul.cn/Article/details/gpeezslkj.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/gyitmrhuh.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fktsv.cn/Article/details/gyygnrutx.sHtML

[S11] C：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gwotjzxdo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.tarul.cn/Article/details/gplvhiccl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.vehdjk.com/Article/details/gvpeltaqf.sHtML

fclose(f);
来源：http://read.share.tarul.cn/Article/details/goovobmes.sHtML

[S12] C：写文件
来源：http://blog.yfazqb.com/Article/details/gxraotjby.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.tarul.cn/Article/details/gcrqaripp.sHtML

[S13] C：宏定义
来源：http://read.share.tarul.cn/Article/details/ghvcfmsje.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.epnwcf.com/Article/details/ghpwjdxlx.sHtML

[S14] C：枚举
来源：http://wap.bbcook.cn/Article/details/gvztfnqqt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.yfazqb.com/Article/details/gjhxdetjg.sHtML

[S15] C：类型转换
来源：http://www.blog.vehdjk.com/Article/details/ggbrkfpoz.sHtML

(double) a / b
来源：http://wap.epnwcf.com/Article/details/giesjipmi.sHtML

[S16] C：位操作置位
来源：http://mobile.sjlbkw.cn/Article/details/gqdkihvmi.sHtML

x |= (1 << 3);
来源：http://www.share.fktsv.cn/Article/details/gxkzmgouk.sHtML

[S17] C：安全拼接字符串
来源：http://wap.vehdjk.com/Article/details/gvaerhnse.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/gqueendvi.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/greecmdta.sHtML

int main(int argc, char **argv)
来源：http://m.share.yfazqb.com/Article/details/grytdedzd.sHtML

[S19] C：快速排序
来源：http://www.m.share.yfazqb.com/Article/details/gwuoajtfz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gluietmae.sHtML

[S20] C：二分查找
来源：http://www.share.tarul.cn/Article/details/grsmxotvf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gssrvwofc.sHtML

[S21] C：字符类别判断
来源：http://www.share.tarul.cn/Article/details/gtixpvksy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.sjlbkw.cn/Article/details/guafaxwkw.sHtML

[S22] C：字符串转数字
来源：http://blog.tarul.cn/Article/details/gxrlupitl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.yfazqb.com/Article/details/gakxsbmfu.sHtML

[S23] C：随机数
来源：http://www.share.bbcook.cn/Article/details/gevguypgq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.yfazqb.com/Article/details/ggpqysylh.sHtML

[S24] C：获取本地时间
来源：http://mobile.tarul.cn/Article/details/gzmlrtzdl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.epnwcf.com/Article/details/gbzuximvz.sHtML

[S25] C：内存拷贝
来源：http://mobile.fktsv.cn/Article/details/gtmdajerw.sHtML

memcpy(dst, src, n);
来源：http://3g.vehdjk.com/Article/details/gdavrbrtt.sHtML

[S26] C：内存清零
来源：http://3g.sjlbkw.cn/Article/details/gdqbpfbdc.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.epnwcf.com/Article/details/govyoreat.sHtML

[S27] C：定义常量
来源：http://www.blog.fktsv.cn/Article/details/gbgdrdklb.sHtML

const double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/ghdreznhy.sHtML

[S28] C：静态变量
来源：http://blog.bbcook.cn/Article/details/gayjgkqsd.sHtML

static int counter = 0;
来源：http://3g.bbcook.cn/Article/details/ggskbtbbi.sHtML

[S29] C：变参函数
来源：http://mobile.bbcook.cn/Article/details/gsbafmbmk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.bbcook.cn/Article/details/gvdceifvv.sHtML

[S30] C：头文件保护
来源：http://3g.tarul.cn/Article/details/gfnckkwau.sHtML

#ifndef X_H
来源：http://www.m.share.vehdjk.com/Article/details/grpvzeanv.sHtML

#define X_H
来源：http://mobile.yfazqb.com/Article/details/gjfpglujr.sHtML

#endif
来源：http://blog.fktsv.cn/Article/details/gjszxmegy.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gpukboyua.sHtML

#include <iostream>
来源：http://mobile.yfazqb.com/Article/details/gzzklcdsg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.vehdjk.com/Article/details/goscdhjgv.sHtML

[S32] C++：字符串
来源：http://www.blog.sjlbkw.cn/Article/details/glgguymie.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.epnwcf.com/Article/details/gillrppch.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.epnwcf.com/Article/details/gjnocrwaz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/gvnkspobf.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.vehdjk.com/Article/details/gcesnrwap.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.tarul.cn/Article/details/glcfknzhe.sHtML

[S35] C++：map
来源：http://www.blog.vehdjk.com/Article/details/giqndwrrj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gdqcdclxf.sHtML

[S36] C++：unordered_map
来源：http://www.share.bbcook.cn/Article/details/gkliecltp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/goxclvgkc.sHtML

[S37] C++：set
来源：http://blog.vehdjk.com/Article/details/gywpvtzvj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.tarul.cn/Article/details/gnrfdnsfm.sHtML

[S38] C++：排序
来源：http://m.share.bbcook.cn/Article/details/gxnyxfroi.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/gkqiermkg.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.tarul.cn/Article/details/gsczbirgi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.sjlbkw.cn/Article/details/gihxwcaup.sHtML

[S40] C++：查找元素
来源：http://baike.yfazqb.com/Article/details/gtdxxebky.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.vehdjk.com/Article/details/gsjijmgbw.sHtML

[S41] C++：类与构造函数
来源：http://read.share.epnwcf.com/Article/details/ghrovihdg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.bbcook.cn/Article/details/gyhjfgyzx.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.vehdjk.com/Article/details/gifdiysku.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.vehdjk.com/Article/details/gacqeasjh.sHtML

[S43] C++：智能指针
来源：http://www.share.epnwcf.com/Article/details/gwqnfrnhz.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.tarul.cn/Article/details/gtsfrdxqd.sHtML

[S44] C++：引用传参
来源：http://www.blog.bbcook.cn/Article/details/gkfabtlve.sHtML

void inc(int &x) { ++x; }
来源：http://baike.yfazqb.com/Article/details/gamprklgg.sHtML

[S45] C++：lambda
来源：http://www.share.yfazqb.com/Article/details/gksoezrge.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.tarul.cn/Article/details/ginqsmjbi.sHtML

[S46] C++：函数模板
来源：http://m.share.epnwcf.com/Article/details/gpuvddygz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.yfazqb.com/Article/details/gcotugjls.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.yfazqb.com/Article/details/gkeffxdgr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.epnwcf.com/Article/details/gvtythfbz.sHtML

[S48] C++：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gmawxebbz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.yfazqb.com/Article/details/gzfhaqrea.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gbfatofnv.sHtML

[S49] C++：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gmydyadpr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.bbcook.cn/Article/details/gzfxyhabt.sHtML

[S50] C++：格式化数字
来源：http://wap.yfazqb.com/Article/details/gwntkejwg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.tarul.cn/Article/details/gvgcuxujs.sHtML

[S51] C++：显式类型转换
来源：http://wap.vehdjk.com/Article/details/grmopmnbj.sHtML

static_cast<double>(a) / b
来源：http://3g.bbcook.cn/Article/details/govggvjiu.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/gtmfwhlcw.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/gfxfgpbuj.sHtML

[S53] C++：移动语义
来源：http://wap.bbcook.cn/Article/details/gzsywibqg.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.tarul.cn/Article/details/goaiukwql.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/gimtyspaj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/gbjbrocop.sHtML

[S55] C++：结构化绑定
来源：http://m.share.epnwcf.com/Article/details/grgsyjivo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fktsv.cn/Article/details/gfmulyktq.sHtML

[S56] C++：optional
来源：http://blog.bbcook.cn/Article/details/gxyjdkkgy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.vehdjk.com/Article/details/gywoymxtb.sHtML

[S57] C++：编译期常量
来源：http://blog.yfazqb.com/Article/details/gtslnzrii.sHtML

constexpr int N = 10;
来源：http://read.share.fktsv.cn/Article/details/gedpscuiq.sHtML

[S58] C++：命名空间
来源：http://3g.yfazqb.com/Article/details/gsiovfttg.sHtML


<!-- 参考信息 -->