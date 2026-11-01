代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fktsv.cn/Article/details/gvvbinhro.sHtML

[Q90] 生成序号列
来源：http://3g.tarul.cn/Article/details/gfdzpnrrh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.bbcook.cn/Article/details/gizkyiebd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gibngpykn.sHtML

R. Bash 专题
来源：http://read.share.fktsv.cn/Article/details/gicwsethg.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ggebtvlae.sHtML

[R01] shebang 与严格模式
来源：http://3g.yfazqb.com/Article/details/gclhswgkp.sHtML

#!/usr/bin/env bash
来源：http://mobile.bbcook.cn/Article/details/gefdcghxd.sHtML

set -euo pipefail
来源：http://www.m.share.fktsv.cn/Article/details/grcmchfgn.sHtML

[R02] 变量赋值与使用
来源：http://3g.yfazqb.com/Article/details/gfnczstwu.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.epnwcf.com/Article/details/gvposzsff.sHtML

[R03] 只读变量
来源：http://wap.bbcook.cn/Article/details/gaccsqhxx.sHtML

readonly PI=3.14
来源：http://www.blog.epnwcf.com/Article/details/glrbkuume.sHtML

[R04] 位置参数
来源：http://www.blog.fktsv.cn/Article/details/gleuluqnf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.yfazqb.com/Article/details/giqwksovy.sHtML

[R05] 参数默认值
来源：http://m.share.epnwcf.com/Article/details/gwizahctn.sHtML

name="${1:-default}"
来源：http://www.m.share.fktsv.cn/Article/details/geulxmthe.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fktsv.cn/Article/details/gohfcyspl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/gbitfmqni.sHtML

[R07] if 判断文件
来源：http://www.m.share.fktsv.cn/Article/details/gnegrkgul.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.epnwcf.com/Article/details/gawegfxrg.sHtML

[R08] 数值比较
来源：http://wap.bbcook.cn/Article/details/grufnzfnm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.tarul.cn/Article/details/ganczzdgy.sHtML

[R09] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/gyqxvonou.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.yfazqb.com/Article/details/guuhkvyil.sHtML

[R10] 正则匹配
来源：http://www.blog.fktsv.cn/Article/details/gakbqugxj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fktsv.cn/Article/details/gfqtlpoqa.sHtML

[R11] case 多分支
来源：http://baike.tarul.cn/Article/details/gncpdcjxs.sHtML

case "$1" in
来源：http://blog.bbcook.cn/Article/details/gxxnpbrou.sHtML

start) echo "启动" ;;
来源：http://mobile.fktsv.cn/Article/details/gwoeylnxx.sHtML

stop)  echo "停止" ;;
来源：http://blog.sjlbkw.cn/Article/details/gcbqlfwmm.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.tarul.cn/Article/details/gcspvapej.sHtML

esac
来源：http://baike.yfazqb.com/Article/details/gcxywhxoc.sHtML

[R12] for 遍历文件
来源：http://baike.bbcook.cn/Article/details/gewgserqr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.tarul.cn/Article/details/goeicsnne.sHtML

[R13] for 计数循环
来源：http://blog.yfazqb.com/Article/details/gjgxfprqz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/gmppfpdnr.sHtML

[R14] C 风格 for
来源：http://wap.epnwcf.com/Article/details/gofqclyxg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/gszisiuqp.sHtML

[R15] while 逐行读文件
来源：http://www.share.tarul.cn/Article/details/gmurwsdaz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.epnwcf.com/Article/details/gfjnhpzus.sHtML

[R16] until 等待条件
来源：http://www.blog.tarul.cn/Article/details/gedgunzqg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gmrlekzae.sHtML

[R17] 数组定义与取值
来源：http://blog.bbcook.cn/Article/details/gqpkpxtjz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.vehdjk.com/Article/details/gyzqhmenf.sHtML

[R18] 遍历数组
来源：http://3g.tarul.cn/Article/details/gofdnxllh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.sjlbkw.cn/Article/details/gbdvstlwp.sHtML

[R19] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/goddffsdz.sHtML

echo "${#arr[@]}"
来源：http://blog.epnwcf.com/Article/details/gjsryeksw.sHtML

[R20] 关联数组（字典）
来源：http://baike.vehdjk.com/Article/details/ggpriaxmq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.vehdjk.com/Article/details/gevxbcetr.sHtML

[R21] 字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gqrjymuov.sHtML

echo "${#s}"
来源：http://www.m.share.fktsv.cn/Article/details/gpyipveuc.sHtML

[R22] 截取子串
来源：http://baike.tarul.cn/Article/details/gpwherukb.sHtML

echo "${s:0:5}"
来源：http://www.blog.sjlbkw.cn/Article/details/gllehhdzt.sHtML

[R23] 字符串替换
来源：http://read.share.tarul.cn/Article/details/gcxtcqoot.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.tarul.cn/Article/details/gsutsgrit.sHtML

[R24] 大小写转换
来源：http://baike.tarul.cn/Article/details/gwprelovl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.sjlbkw.cn/Article/details/gyqjyjkbj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.epnwcf.com/Article/details/gxddlboul.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fktsv.cn/Article/details/gxuhoycat.sHtML

[R26] 命令替换
来源：http://m.share.epnwcf.com/Article/details/gwuwkwdai.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.yfazqb.com/Article/details/gvibupccr.sHtML

[R27] 算术展开
来源：http://3g.epnwcf.com/Article/details/gmchhcenq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fktsv.cn/Article/details/gntgdbefi.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/gvyspkbwo.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.vehdjk.com/Article/details/gretwmylm.sHtML

[R29] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gjzcqhwqf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.vehdjk.com/Article/details/gijpwhsek.sHtML

[R30] 函数返回状态码
来源：http://blog.tarul.cn/Article/details/gqnqjoolk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.tarul.cn/Article/details/gsmwahssw.sHtML

[R31] 局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gnmwnqxqb.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.epnwcf.com/Article/details/gmaddwhmz.sHtML

[R32] 参数个数校验
来源：http://blog.yfazqb.com/Article/details/grkoepshj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.tarul.cn/Article/details/gczurhpfi.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.epnwcf.com/Article/details/gxzqubpzt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.tarul.cn/Article/details/gukxgemwx.sHtML

[R34] 退出时清理
来源：http://www.share.tarul.cn/Article/details/ggfwfwlzs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gzxzgyiyr.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fktsv.cn/Article/details/glbiyrffk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gxblbcwbp.sHtML

[R36] 并发执行多个任务
来源：http://mobile.yfazqb.com/Article/details/gdkhiewqo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.vehdjk.com/Article/details/ghyxgapuq.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.vehdjk.com/Article/details/gtuafsrny.sHtML

files=$(ls -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gbnfuhbwt.sHtML

[R38] 管道串联
来源：http://www.share.tarul.cn/Article/details/gvzcquuii.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.bbcook.cn/Article/details/gbjjdsrgz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.yfazqb.com/Article/details/gtzroccda.sHtML

cmd > out.log 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/goowpgobd.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/glgstjlmk.sHtML

echo "log" >> out.log
来源：http://m.share.sjlbkw.cn/Article/details/getkyshis.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/gsfnhvfar.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/gvzboqgtk.sHtML

[R42] 输入重定向
来源：http://3g.tarul.cn/Article/details/gqjynmhdp.sHtML

wc -l < a.txt
来源：http://m.share.tarul.cn/Article/details/gpgzgvuzb.sHtML

[R43] 按名字查找文件
来源：http://mobile.bbcook.cn/Article/details/gephpbvly.sHtML

find . -name "*.log" -type f
来源：http://mobile.epnwcf.com/Article/details/gpgxoclgy.sHtML

[R44] 按修改时间查找
来源：http://read.share.yfazqb.com/Article/details/gwzgqgoin.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.yfazqb.com/Article/details/gifyxmkzs.sHtML

[R45] 批量删除
来源：http://3g.fktsv.cn/Article/details/ggjdkbvsr.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fktsv.cn/Article/details/gkbyackwr.sHtML

[R46] 递归替换文件内容
来源：http://www.share.bbcook.cn/Article/details/gttptrzsb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.epnwcf.com/Article/details/gdhlhevki.sHtML

[R47] sed 单行替换
来源：http://3g.tarul.cn/Article/details/gupwacmrk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/gongrqmhy.sHtML

[R48] awk 取指定列
来源：http://baike.vehdjk.com/Article/details/gfyujieyl.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.tarul.cn/Article/details/gxxcguule.sHtML

[R49] awk 带条件
来源：http://3g.epnwcf.com/Article/details/gqjqldlkv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.bbcook.cn/Article/details/gmneljfse.sHtML

[R50] awk 求和
来源：http://baike.yfazqb.com/Article/details/grgrgfgax.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fktsv.cn/Article/details/grfngsbbv.sHtML

[R51] 排序去重取前几
来源：http://3g.fktsv.cn/Article/details/gqmijwucz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fktsv.cn/Article/details/gkpysotdu.sHtML

[R52] 统计行数
来源：http://www.blog.bbcook.cn/Article/details/gexuupjvd.sHtML

wc -l a.txt
来源：http://www.share.bbcook.cn/Article/details/gzrvldraa.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.bbcook.cn/Article/details/gyqfbzbyq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gzbykcoag.sHtML

[R54] 比较两个文件
来源：http://www.blog.fktsv.cn/Article/details/gkbbvptyt.sHtML

diff a.txt b.txt
来源：http://baike.yfazqb.com/Article/details/gabgmkiht.sHtML

[R55] 压缩与解压
来源：http://www.blog.epnwcf.com/Article/details/gtmccedfm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.sjlbkw.cn/Article/details/gspwdsnll.sHtML

[R56] 远程拷贝
来源：http://blog.epnwcf.com/Article/details/gyimcmbsa.sHtML

scp file user@host:/path/
来源：http://www.share.tarul.cn/Article/details/gkexfkwiy.sHtML

[R57] 远程执行命令
来源：http://wap.fktsv.cn/Article/details/gjlqkxubg.sHtML

ssh user@host 'uptime'
来源：http://blog.fktsv.cn/Article/details/gnltuupig.sHtML

[R58] 下载文件
来源：http://baike.epnwcf.com/Article/details/gawljunux.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.epnwcf.com/Article/details/gnhjawhkd.sHtML

[R59] 发 POST JSON
来源：http://wap.bbcook.cn/Article/details/gqvffhijt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.vehdjk.com/Article/details/gcfybhnzq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gfnvsviys.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.bbcook.cn/Article/details/gkedsyxlt.sHtML

[R61] 磁盘占用
来源：http://blog.fktsv.cn/Article/details/gdlevapwf.sHtML

df -h;  du -sh *
来源：http://wap.bbcook.cn/Article/details/gaalxejnb.sHtML

[R62] 找最占空间的文件
来源：http://wap.epnwcf.com/Article/details/giddizmjz.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fktsv.cn/Article/details/gibepxhce.sHtML

[R63] 内存与进程
来源：http://www.blog.fktsv.cn/Article/details/gbyrnweeu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.epnwcf.com/Article/details/grmzskucl.sHtML

[R64] 结束进程
来源：http://m.share.yfazqb.com/Article/details/gsngyfbly.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.bbcook.cn/Article/details/gvgloqvaa.sHtML

[R65] 查看端口占用
来源：http://www.blog.yfazqb.com/Article/details/gipabdahy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.epnwcf.com/Article/details/gvypxbvsg.sHtML

[R66] 定时任务
来源：http://www.blog.tarul.cn/Article/details/gbnlusntu.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.tarul.cn/Article/details/gqazrbmta.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.epnwcf.com/Article/details/gvykxhjiv.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/gilfdcfcl.sHtML

[R68] 计算文件校验值
来源：http://www.blog.bbcook.cn/Article/details/gcbipgswg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.yfazqb.com/Article/details/gfdutqiqf.sHtML

[R69] 生成随机密码
来源：http://blog.vehdjk.com/Article/details/gctpjbsht.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.yfazqb.com/Article/details/gikawvenv.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.epnwcf.com/Article/details/gipcakzzt.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.yfazqb.com/Article/details/gnfhnhkfj.sHtML

[R71] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gyjgukicr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.epnwcf.com/Article/details/gyqtxgtwh.sHtML

[R72] 等待端口就绪
来源：http://baike.vehdjk.com/Article/details/ggfguuqbx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gyqmtvlvw.sHtML

[R73] 分割大日志
来源：http://m.share.sjlbkw.cn/Article/details/gizrcwczh.sHtML

split -l 1000 big.log part_
来源：http://m.share.yfazqb.com/Article/details/gljihyfcy.sHtML

[R74] 批量重命名
来源：http://3g.sjlbkw.cn/Article/details/guhkbgyeb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.epnwcf.com/Article/details/gtwegwyrr.sHtML

[R75] 导出环境变量
来源：http://wap.vehdjk.com/Article/details/gshcnrtne.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.bbcook.cn/Article/details/gsxmfwuux.sHtML

[R76] 使用临时文件
来源：http://blog.tarul.cn/Article/details/glpoetobs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/gyrnbqvpj.sHtML

[R77] 读取用户输入
来源：http://read.share.yfazqb.com/Article/details/gckujplvd.sHtML

read -rp "请输入: " ans
来源：http://mobile.epnwcf.com/Article/details/giazkhxzq.sHtML

[R78] 交互式菜单
来源：http://read.share.tarul.cn/Article/details/gpdsngodg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.tarul.cn/Article/details/gqwubbzng.sHtML

[R79] 解析命令行选项
来源：http://3g.fktsv.cn/Article/details/gcavvomwa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.vehdjk.com/Article/details/gkchnupjj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.tarul.cn/Article/details/ggnrlzfjw.sHtML

time ./run.sh
来源：http://3g.sjlbkw.cn/Article/details/gizzfupks.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gyofdajdh.sHtML

S. C / C++ 专题
来源：http://m.share.bbcook.cn/Article/details/giagjtzpm.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/guhzjydkz.sHtML

[S01] C：Hello World
来源：http://wap.yfazqb.com/Article/details/golvlbqki.sHtML

#include <stdio.h>
来源：http://baike.vehdjk.com/Article/details/gaduavokk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.vehdjk.com/Article/details/gwgkhqikk.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgixtkct.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.vehdjk.com/Article/details/gcyjhqtrf.sHtML

[S03] C：读入整数
来源：http://read.share.tarul.cn/Article/details/gyepxsayj.sHtML

int x; scanf("%d", &x);
来源：http://www.share.vehdjk.com/Article/details/gevawasqd.sHtML

[S04] C：字符串复制
来源：http://www.m.share.yfazqb.com/Article/details/goeqdeyyb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fktsv.cn/Article/details/gidmydclc.sHtML

[S05] C：字符串长度
来源：http://wap.bbcook.cn/Article/details/gozsutmoo.sHtML

strlen(s)
来源：http://baike.tarul.cn/Article/details/gataczhnz.sHtML

[S06] C：字符串比较
来源：http://mobile.bbcook.cn/Article/details/gtypvvntd.sHtML

strcmp(a, b) == 0
来源：http://read.share.yfazqb.com/Article/details/gfzxyhmyp.sHtML

[S07] C：数组遍历求和
来源：http://3g.yfazqb.com/Article/details/grudcodjn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.epnwcf.com/Article/details/gzmohxrjv.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gznzkvvjh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.bbcook.cn/Article/details/gqgpdrstb.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.epnwcf.com/Article/details/gagsdcfot.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.bbcook.cn/Article/details/gqwuvxreg.sHtML

[S10] C：指针与解引用
来源：http://m.share.yfazqb.com/Article/details/govkmyxcv.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.bbcook.cn/Article/details/glgxqcngr.sHtML

[S11] C：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gckaelpxe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.epnwcf.com/Article/details/gdqbbdlyx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fktsv.cn/Article/details/glcfaswyl.sHtML

fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gnxxtyzci.sHtML

[S12] C：写文件
来源：http://www.share.fktsv.cn/Article/details/grltarrvt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.yfazqb.com/Article/details/gowozvuul.sHtML

[S13] C：宏定义
来源：http://blog.fktsv.cn/Article/details/gndhwggml.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.vehdjk.com/Article/details/gewyqxchw.sHtML

[S14] C：枚举
来源：http://m.share.epnwcf.com/Article/details/gofygcmcw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.vehdjk.com/Article/details/glhajgllp.sHtML

[S15] C：类型转换
来源：http://read.share.epnwcf.com/Article/details/gagtmfkjf.sHtML

(double) a / b
来源：http://3g.vehdjk.com/Article/details/gwcalmfus.sHtML

[S16] C：位操作置位
来源：http://www.m.share.vehdjk.com/Article/details/gcqhdexdp.sHtML

x |= (1 << 3);
来源：http://www.blog.fktsv.cn/Article/details/gewgpnodf.sHtML

[S17] C：安全拼接字符串
来源：http://baike.yfazqb.com/Article/details/gbelqbcyv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.tarul.cn/Article/details/gvquwyqgo.sHtML

[S18] C：命令行参数
来源：http://wap.sjlbkw.cn/Article/details/giurmtffv.sHtML

int main(int argc, char **argv)
来源：http://www.share.sjlbkw.cn/Article/details/gnyuevzrk.sHtML

[S19] C：快速排序
来源：http://3g.epnwcf.com/Article/details/gbxnamakz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gozgfoawg.sHtML

[S20] C：二分查找
来源：http://www.share.bbcook.cn/Article/details/gchwpxsfz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/guswvairo.sHtML

[S21] C：字符类别判断
来源：http://www.blog.bbcook.cn/Article/details/ggxxnhfgr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.sjlbkw.cn/Article/details/gexhsbayj.sHtML

[S22] C：字符串转数字
来源：http://read.share.fktsv.cn/Article/details/gnswpcfmz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.bbcook.cn/Article/details/gaehxekay.sHtML

[S23] C：随机数
来源：http://baike.sjlbkw.cn/Article/details/guxquavpj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.yfazqb.com/Article/details/geuobmfan.sHtML

[S24] C：获取本地时间
来源：http://www.share.epnwcf.com/Article/details/goioeyarz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.bbcook.cn/Article/details/gmwctksdt.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/grobzxznk.sHtML

memcpy(dst, src, n);
来源：http://read.share.vehdjk.com/Article/details/gojmfomgr.sHtML

[S26] C：内存清零
来源：http://m.share.tarul.cn/Article/details/gbupovwkv.sHtML

memset(a, 0, sizeof a);
来源：http://blog.epnwcf.com/Article/details/guqibiggh.sHtML

[S27] C：定义常量
来源：http://read.share.bbcook.cn/Article/details/gtpygnwvh.sHtML

const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gjbsqyfxp.sHtML

[S28] C：静态变量
来源：http://www.share.sjlbkw.cn/Article/details/gwhihxtzw.sHtML

static int counter = 0;
来源：http://www.share.yfazqb.com/Article/details/gdhbowces.sHtML

[S29] C：变参函数
来源：http://3g.bbcook.cn/Article/details/ggncxjgjo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fktsv.cn/Article/details/gupctnmpf.sHtML

[S30] C：头文件保护
来源：http://www.m.share.tarul.cn/Article/details/gycogbyke.sHtML

#ifndef X_H
来源：http://www.m.share.vehdjk.com/Article/details/gnvscqhko.sHtML

#define X_H
来源：http://baike.sjlbkw.cn/Article/details/gfayxbowy.sHtML

#endif
来源：http://www.m.share.tarul.cn/Article/details/grqgmikgx.sHtML

[S31] C++：Hello World
来源：http://mobile.vehdjk.com/Article/details/gnbwgjzty.sHtML

#include <iostream>
来源：http://wap.yfazqb.com/Article/details/ghrbujxgc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.tarul.cn/Article/details/gxvydsgoz.sHtML

[S32] C++：字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/geemzartp.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.tarul.cn/Article/details/ggsdonrfm.sHtML

[S33] C++：vector 增删
来源：http://www.share.sjlbkw.cn/Article/details/gxgjxxuvp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.sjlbkw.cn/Article/details/gtcuxytia.sHtML

[S34] C++：遍历 vector
来源：http://www.share.vehdjk.com/Article/details/gslxqmxzg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.tarul.cn/Article/details/gekuymmtb.sHtML

[S35] C++：map
来源：http://mobile.fktsv.cn/Article/details/gocmqqbfz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gimtmigvt.sHtML

[S36] C++：unordered_map
来源：http://baike.vehdjk.com/Article/details/gculjgoan.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/ggasofqqx.sHtML

[S37] C++：set
来源：http://mobile.yfazqb.com/Article/details/gotwbutyt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/gegimpjhd.sHtML

[S38] C++：排序
来源：http://www.blog.tarul.cn/Article/details/gacddppbw.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fktsv.cn/Article/details/gzgbywynw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.yfazqb.com/Article/details/gapmzdgmi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.epnwcf.com/Article/details/gmkerbjwi.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fktsv.cn/Article/details/gzlstpkxt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/gjyhemrre.sHtML

[S41] C++：类与构造函数
来源：http://baike.fktsv.cn/Article/details/gqtagkwes.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fktsv.cn/Article/details/gafmexrms.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.bbcook.cn/Article/details/gplfpzxlc.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.sjlbkw.cn/Article/details/ghnxoriuo.sHtML

[S43] C++：智能指针
来源：http://www.share.vehdjk.com/Article/details/gsmqtgjlx.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.yfazqb.com/Article/details/gjzsjhydg.sHtML

[S44] C++：引用传参
来源：http://mobile.yfazqb.com/Article/details/grqqsrspo.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fktsv.cn/Article/details/gufelvaem.sHtML

[S45] C++：lambda
来源：http://www.m.share.yfazqb.com/Article/details/gfxjhdtjo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.yfazqb.com/Article/details/gokdirxdu.sHtML

[S46] C++：函数模板
来源：http://www.m.share.yfazqb.com/Article/details/gtgwnxluz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.bbcook.cn/Article/details/gunnkkshs.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.vehdjk.com/Article/details/gefzhuwbd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.sjlbkw.cn/Article/details/gnvbpiaxx.sHtML

[S48] C++：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gbzbdmpcn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.epnwcf.com/Article/details/gkuhjldve.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fktsv.cn/Article/details/gynuefpuo.sHtML

[S49] C++：写文件
来源：http://wap.sjlbkw.cn/Article/details/gkibmjuoe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.tarul.cn/Article/details/gevwbtwqy.sHtML

[S50] C++：格式化数字
来源：http://baike.sjlbkw.cn/Article/details/getqkgyno.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gmuijmyfq.sHtML

[S51] C++：显式类型转换
来源：http://3g.yfazqb.com/Article/details/ghzoijciv.sHtML

static_cast<double>(a) / b
来源：http://read.share.epnwcf.com/Article/details/ghgqhwtad.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.sjlbkw.cn/Article/details/gqxowhzzf.sHtML

int size() const noexcept { return n_; }
来源：http://baike.epnwcf.com/Article/details/gukttjxkq.sHtML

[S53] C++：移动语义
来源：http://mobile.epnwcf.com/Article/details/geomfdoui.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.yfazqb.com/Article/details/gowbigvdo.sHtML

[S54] C++：异常处理
来源：http://baike.tarul.cn/Article/details/gdztswpcf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.yfazqb.com/Article/details/gfwuejjuu.sHtML

[S55] C++：结构化绑定
来源：http://m.share.yfazqb.com/Article/details/grqceawwe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.vehdjk.com/Article/details/gaxzmwvxp.sHtML

[S56] C++：optional
来源：http://read.share.fktsv.cn/Article/details/glyxrtxdt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.epnwcf.com/Article/details/gsvztybbe.sHtML

[S57] C++：编译期常量
来源：http://mobile.epnwcf.com/Article/details/gjqkawlrb.sHtML

constexpr int N = 10;
来源：http://baike.tarul.cn/Article/details/ggspsectf.sHtML

[S58] C++：命名空间
来源：http://wap.sjlbkw.cn/Article/details/gzhpmsnlz.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.tarul.cn/Article/details/gxvnuvpgv.sHtML

[S59] C++：静态断言
来源：http://m.share.vehdjk.com/Article/details/gitdygmng.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.bbcook.cn/Article/details/gnizapukw.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.bbcook.cn/Article/details/gqhxdmdoz.sHtML


<!-- 参考信息 -->