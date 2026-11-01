代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.vehdjk.com/Article/details/geqsxrprl.sHtML

[Q90] 生成序号列
来源：http://mobile.epnwcf.com/Article/details/ggfrltmsg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdulfgnx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnlyeqnqg.sHtML

R. Bash 专题
来源：http://www.share.vehdjk.com/Article/details/gqphxtlma.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gqycepenr.sHtML

[R01] shebang 与严格模式
来源：http://3g.fktsv.cn/Article/details/grbctahfo.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.vehdjk.com/Article/details/gxdyhtdxy.sHtML

set -euo pipefail
来源：http://blog.tarul.cn/Article/details/glqayrjhq.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fktsv.cn/Article/details/gbqhnpwmr.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.vehdjk.com/Article/details/gdysykbyt.sHtML

[R03] 只读变量
来源：http://www.share.vehdjk.com/Article/details/gcvuhvaks.sHtML

readonly PI=3.14
来源：http://read.share.yfazqb.com/Article/details/gcbcmunhy.sHtML

[R04] 位置参数
来源：http://www.blog.tarul.cn/Article/details/giuyojiou.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/gpqqyyrru.sHtML

[R05] 参数默认值
来源：http://wap.bbcook.cn/Article/details/gjujrropr.sHtML

name="${1:-default}"
来源：http://baike.bbcook.cn/Article/details/gkuvvzume.sHtML

[R06] 判断命令是否存在
来源：http://read.share.epnwcf.com/Article/details/gyonzyvlg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.sjlbkw.cn/Article/details/gtrebejvl.sHtML

[R07] if 判断文件
来源：http://www.share.yfazqb.com/Article/details/gqqxcsgoh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gadpxyels.sHtML

[R08] 数值比较
来源：http://read.share.vehdjk.com/Article/details/gpdphivov.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.sjlbkw.cn/Article/details/gotqawtkx.sHtML

[R09] 字符串比较
来源：http://read.share.tarul.cn/Article/details/gbjloouzp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.yfazqb.com/Article/details/gmzqmtfyq.sHtML

[R10] 正则匹配
来源：http://3g.yfazqb.com/Article/details/gclkhzjdu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.tarul.cn/Article/details/ghgmzbetk.sHtML

[R11] case 多分支
来源：http://www.blog.sjlbkw.cn/Article/details/giuxecwnv.sHtML

case "$1" in
来源：http://www.share.epnwcf.com/Article/details/gggdhzwsk.sHtML

start) echo "启动" ;;
来源：http://mobile.fktsv.cn/Article/details/gilpkawkm.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gkehgovpg.sHtML

*)     echo "未知命令" ;;
来源：http://wap.tarul.cn/Article/details/gfmmijafd.sHtML

esac
来源：http://3g.bbcook.cn/Article/details/ghwhncvme.sHtML

[R12] for 遍历文件
来源：http://www.share.epnwcf.com/Article/details/grrrnegmy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.bbcook.cn/Article/details/gnwazbqdd.sHtML

[R13] for 计数循环
来源：http://m.share.sjlbkw.cn/Article/details/gvmgasnot.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/ggqsdoqvn.sHtML

[R14] C 风格 for
来源：http://www.m.share.yfazqb.com/Article/details/gtdgscgpj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gwhlpuqrk.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/gwxpdpjoh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.sjlbkw.cn/Article/details/gqejpeoah.sHtML

[R16] until 等待条件
来源：http://baike.epnwcf.com/Article/details/gzrtetfye.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gmlqqnspi.sHtML

[R17] 数组定义与取值
来源：http://baike.vehdjk.com/Article/details/gyiluyosq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.vehdjk.com/Article/details/gmfzymxer.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/ghqdybvvg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.tarul.cn/Article/details/glohzzhdp.sHtML

[R19] 数组长度
来源：http://3g.yfazqb.com/Article/details/ggxriozuu.sHtML

echo "${#arr[@]}"
来源：http://3g.fktsv.cn/Article/details/genntdgry.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fktsv.cn/Article/details/gfqbsjydi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/gcgrcjrbt.sHtML

[R21] 字符串长度
来源：http://mobile.yfazqb.com/Article/details/gtcxlpjbv.sHtML

echo "${#s}"
来源：http://m.share.epnwcf.com/Article/details/gpqawzwlr.sHtML

[R22] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gsqezvkjc.sHtML

echo "${s:0:5}"
来源：http://read.share.vehdjk.com/Article/details/gmwebylmc.sHtML

[R23] 字符串替换
来源：http://m.share.fktsv.cn/Article/details/gnhvvrwox.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.yfazqb.com/Article/details/gxbagutip.sHtML

[R24] 大小写转换
来源：http://baike.fktsv.cn/Article/details/giltrgqhz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.epnwcf.com/Article/details/gowjprlqr.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fktsv.cn/Article/details/gmvphjzuy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.vehdjk.com/Article/details/gfyhvuuld.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/gclynmwrj.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.yfazqb.com/Article/details/grnfxcaff.sHtML

[R27] 算术展开
来源：http://mobile.tarul.cn/Article/details/gtlitnivy.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.bbcook.cn/Article/details/grfzeawbp.sHtML

[R28] 浮点运算
来源：http://read.share.vehdjk.com/Article/details/gykjmldmu.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/ghufnumme.sHtML

[R29] 定义函数
来源：http://baike.fktsv.cn/Article/details/galovaywh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fktsv.cn/Article/details/gkbalvjta.sHtML

[R30] 函数返回状态码
来源：http://www.blog.bbcook.cn/Article/details/gnukprtof.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.tarul.cn/Article/details/grqgygvaq.sHtML

[R31] 局部变量
来源：http://www.blog.bbcook.cn/Article/details/gbdwdggtu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.bbcook.cn/Article/details/ghhjeqriy.sHtML

[R32] 参数个数校验
来源：http://www.blog.epnwcf.com/Article/details/gnjlmepic.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gbylwopnt.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.vehdjk.com/Article/details/glyinmoee.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.tarul.cn/Article/details/gyuwchzbk.sHtML

[R34] 退出时清理
来源：http://www.share.epnwcf.com/Article/details/gwjnztatl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/gqmuswfgv.sHtML

[R35] 后台执行并等待
来源：http://m.share.fktsv.cn/Article/details/gxsrprnxr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.vehdjk.com/Article/details/gqriexcub.sHtML

[R36] 并发执行多个任务
来源：http://3g.bbcook.cn/Article/details/gujlxsdgd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.bbcook.cn/Article/details/gqlqiifff.sHtML

[R37] 把输出赋给变量
来源：http://m.share.tarul.cn/Article/details/gropzeksq.sHtML

files=$(ls -1)
来源：http://blog.fktsv.cn/Article/details/gbdozvkgk.sHtML

[R38] 管道串联
来源：http://www.blog.fktsv.cn/Article/details/gvbimdzut.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.yfazqb.com/Article/details/gvriwlpkw.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fktsv.cn/Article/details/gklhymana.sHtML

cmd > out.log 2>&1
来源：http://wap.epnwcf.com/Article/details/ggxblnlrt.sHtML

[R40] 追加写日志
来源：http://www.m.share.bbcook.cn/Article/details/glwlohjyj.sHtML

echo "log" >> out.log
来源：http://baike.tarul.cn/Article/details/gxvewpfuh.sHtML

[R41] 丢弃输出
来源：http://baike.vehdjk.com/Article/details/gsayhlwtb.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.tarul.cn/Article/details/gfqnrhucq.sHtML

[R42] 输入重定向
来源：http://baike.fktsv.cn/Article/details/gtiunajai.sHtML

wc -l < a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gslqfmtve.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.vehdjk.com/Article/details/gfpytoitk.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/gdxwsmjzu.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.vehdjk.com/Article/details/givtjvocd.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/gmyzfvqrn.sHtML

[R45] 批量删除
来源：http://www.share.fktsv.cn/Article/details/gfczofngu.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fktsv.cn/Article/details/gsywnwnbs.sHtML

[R46] 递归替换文件内容
来源：http://m.share.bbcook.cn/Article/details/gnoshackg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.epnwcf.com/Article/details/gaisfxksk.sHtML

[R47] sed 单行替换
来源：http://www.blog.tarul.cn/Article/details/gbvxvlcey.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.yfazqb.com/Article/details/glgmevkta.sHtML

[R48] awk 取指定列
来源：http://wap.bbcook.cn/Article/details/gpmmfrbvi.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gujmguejc.sHtML

[R49] awk 带条件
来源：http://www.m.share.vehdjk.com/Article/details/grtrasvhn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fktsv.cn/Article/details/gwammehff.sHtML

[R50] awk 求和
来源：http://3g.fktsv.cn/Article/details/ggerzkngf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fktsv.cn/Article/details/grrjedvzo.sHtML

[R51] 排序去重取前几
来源：http://www.share.fktsv.cn/Article/details/grfyocefo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.tarul.cn/Article/details/gjghcssey.sHtML

[R52] 统计行数
来源：http://read.share.yfazqb.com/Article/details/gdtigsbvb.sHtML

wc -l a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gwnprnakn.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.vehdjk.com/Article/details/gmlnqmxup.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fktsv.cn/Article/details/gdxdwsfzn.sHtML

[R54] 比较两个文件
来源：http://wap.tarul.cn/Article/details/gqljvjkcl.sHtML

diff a.txt b.txt
来源：http://3g.tarul.cn/Article/details/gxlftssfj.sHtML

[R55] 压缩与解压
来源：http://blog.bbcook.cn/Article/details/gevejlnzl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.bbcook.cn/Article/details/gzqwwhtzu.sHtML

[R56] 远程拷贝
来源：http://3g.yfazqb.com/Article/details/gpvmbdfls.sHtML

scp file user@host:/path/
来源：http://mobile.epnwcf.com/Article/details/gvrpxkfuk.sHtML

[R57] 远程执行命令
来源：http://www.share.tarul.cn/Article/details/gljmfptwi.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.vehdjk.com/Article/details/gliqllfyt.sHtML

[R58] 下载文件
来源：http://wap.vehdjk.com/Article/details/grfmsureh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/giporasww.sHtML

[R59] 发 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/guwtfzxgk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.sjlbkw.cn/Article/details/gzvknwnzo.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gqfjwrigz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.sjlbkw.cn/Article/details/gzpkiuqfa.sHtML

[R61] 磁盘占用
来源：http://www.blog.vehdjk.com/Article/details/gvouabzdk.sHtML

df -h;  du -sh *
来源：http://www.blog.epnwcf.com/Article/details/gppfmjimx.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.vehdjk.com/Article/details/ggkpagtuq.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.vehdjk.com/Article/details/ghaklutck.sHtML

[R63] 内存与进程
来源：http://www.m.share.vehdjk.com/Article/details/gxkwrrykh.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.sjlbkw.cn/Article/details/ggfqwgell.sHtML

[R64] 结束进程
来源：http://blog.bbcook.cn/Article/details/gaiqyshra.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/gkcbsyykc.sHtML

[R65] 查看端口占用
来源：http://m.share.sjlbkw.cn/Article/details/gwwqmztmz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.bbcook.cn/Article/details/gzgcvtqgk.sHtML

[R66] 定时任务
来源：http://www.blog.vehdjk.com/Article/details/gcvrpjufs.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/gpyriepoa.sHtML

[R67] 生成随机十六进制串
来源：http://3g.sjlbkw.cn/Article/details/gwunyrnky.sHtML

openssl rand -hex 16
来源：http://m.share.sjlbkw.cn/Article/details/gosptlgmo.sHtML

[R68] 计算文件校验值
来源：http://mobile.tarul.cn/Article/details/gizrwlnoy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.bbcook.cn/Article/details/ggvrcqhad.sHtML

[R69] 生成随机密码
来源：http://read.share.fktsv.cn/Article/details/gxrzoqxbb.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fktsv.cn/Article/details/grxacgzsh.sHtML

[R70] 时间戳与互转
来源：http://read.share.yfazqb.com/Article/details/gcjafmqot.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fktsv.cn/Article/details/gacuivsfj.sHtML

[R71] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gjlrizqro.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fktsv.cn/Article/details/geyeomvlh.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fktsv.cn/Article/details/gmsmmnoud.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fktsv.cn/Article/details/gwfgovuce.sHtML

[R73] 分割大日志
来源：http://mobile.yfazqb.com/Article/details/gzzmkiugm.sHtML

split -l 1000 big.log part_
来源：http://mobile.fktsv.cn/Article/details/gvilndmvp.sHtML

[R74] 批量重命名
来源：http://read.share.tarul.cn/Article/details/ghcimgjzo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.bbcook.cn/Article/details/gwlmeumri.sHtML

[R75] 导出环境变量
来源：http://read.share.yfazqb.com/Article/details/ghodcmehl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.epnwcf.com/Article/details/gnjrncsxp.sHtML

[R76] 使用临时文件
来源：http://baike.tarul.cn/Article/details/gebugxmbb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/gjyexxisb.sHtML

[R77] 读取用户输入
来源：http://baike.fktsv.cn/Article/details/gjgrzrwjs.sHtML

read -rp "请输入: " ans
来源：http://m.share.vehdjk.com/Article/details/ggpkoqkcn.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/gcnddmyjd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.bbcook.cn/Article/details/gocxofgrp.sHtML

[R79] 解析命令行选项
来源：http://www.blog.yfazqb.com/Article/details/gqbkslxml.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.epnwcf.com/Article/details/gikcajopz.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.tarul.cn/Article/details/gywcuewfz.sHtML

time ./run.sh
来源：http://m.share.fktsv.cn/Article/details/gsttqvkos.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggcwcwols.sHtML

S. C / C++ 专题
来源：http://blog.fktsv.cn/Article/details/gtkxjsmxk.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gipllntds.sHtML

[S01] C：Hello World
来源：http://blog.fktsv.cn/Article/details/gjkwdqrbb.sHtML

#include <stdio.h>
来源：http://wap.tarul.cn/Article/details/gadovczun.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fktsv.cn/Article/details/gfrkyqvuw.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.epnwcf.com/Article/details/gsuemwhts.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.epnwcf.com/Article/details/gxjhwmusz.sHtML

[S03] C：读入整数
来源：http://www.blog.fktsv.cn/Article/details/gluudpdyr.sHtML

int x; scanf("%d", &x);
来源：http://m.share.sjlbkw.cn/Article/details/gjqrqssud.sHtML

[S04] C：字符串复制
来源：http://3g.tarul.cn/Article/details/gtfdyqyqn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.epnwcf.com/Article/details/guxptxmso.sHtML

[S05] C：字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gkqglupsh.sHtML

strlen(s)
来源：http://m.share.vehdjk.com/Article/details/giudafsgn.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/gknhuplun.sHtML

strcmp(a, b) == 0
来源：http://wap.epnwcf.com/Article/details/gvgotpafj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/glpqnkfmy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.epnwcf.com/Article/details/gfkmdpmef.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.tarul.cn/Article/details/gpmwdrouh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.bbcook.cn/Article/details/gbrkhwifq.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.yfazqb.com/Article/details/gldnputun.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.sjlbkw.cn/Article/details/gnscebfph.sHtML

[S10] C：指针与解引用
来源：http://m.share.tarul.cn/Article/details/gimajqjua.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.sjlbkw.cn/Article/details/gxmczvyrm.sHtML

[S11] C：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gevtpqsel.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.bbcook.cn/Article/details/gfatngtke.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.tarul.cn/Article/details/gvrxcdfmh.sHtML

fclose(f);
来源：http://baike.yfazqb.com/Article/details/gwxigrnkk.sHtML

[S12] C：写文件
来源：http://baike.sjlbkw.cn/Article/details/gvlwbgdbj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/ggzsttssu.sHtML

[S13] C：宏定义
来源：http://mobile.bbcook.cn/Article/details/gqbcqloej.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.vehdjk.com/Article/details/gumvcppbe.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/gjlaomgjc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.bbcook.cn/Article/details/gepbenohh.sHtML

[S15] C：类型转换
来源：http://www.share.yfazqb.com/Article/details/gwlazizbh.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/gbzhlrsku.sHtML

[S16] C：位操作置位
来源：http://www.blog.sjlbkw.cn/Article/details/gydtyuoaw.sHtML

x |= (1 << 3);
来源：http://www.share.vehdjk.com/Article/details/gkuvxzfas.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gtkmhgmtx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.yfazqb.com/Article/details/gpvojhrbo.sHtML

[S18] C：命令行参数
来源：http://m.share.yfazqb.com/Article/details/gpusujchj.sHtML

int main(int argc, char **argv)
来源：http://baike.epnwcf.com/Article/details/gohrfedoj.sHtML

[S19] C：快速排序
来源：http://wap.yfazqb.com/Article/details/gqgvhjycq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/gobdvjojl.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/gzztjziit.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gsrgrtbhk.sHtML

[S21] C：字符类别判断
来源：http://read.share.bbcook.cn/Article/details/gugzjleos.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fktsv.cn/Article/details/gqnsoikfc.sHtML

[S22] C：字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/guiwfyuoh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.yfazqb.com/Article/details/ggantsomz.sHtML

[S23] C：随机数
来源：http://www.share.vehdjk.com/Article/details/gdblkfbfq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.sjlbkw.cn/Article/details/gnrmymcrs.sHtML

[S24] C：获取本地时间
来源：http://read.share.yfazqb.com/Article/details/geznoxflm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.tarul.cn/Article/details/ggifyzdqi.sHtML

[S25] C：内存拷贝
来源：http://blog.sjlbkw.cn/Article/details/gnbvjqzjl.sHtML

memcpy(dst, src, n);
来源：http://baike.tarul.cn/Article/details/gqrxfwrpr.sHtML

[S26] C：内存清零
来源：http://mobile.epnwcf.com/Article/details/gowgkbmad.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/ggzcdphou.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/godzsxnmb.sHtML

const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gfaddfues.sHtML

[S28] C：静态变量
来源：http://m.share.yfazqb.com/Article/details/gojkhzzlq.sHtML

static int counter = 0;
来源：http://m.share.vehdjk.com/Article/details/glmzyvzrq.sHtML

[S29] C：变参函数
来源：http://mobile.bbcook.cn/Article/details/gnhqsraey.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.sjlbkw.cn/Article/details/gozwkfrso.sHtML

[S30] C：头文件保护
来源：http://wap.tarul.cn/Article/details/gfwtssfmk.sHtML

#ifndef X_H
来源：http://mobile.yfazqb.com/Article/details/gkdkqnnru.sHtML

#define X_H
来源：http://read.share.yfazqb.com/Article/details/gxxcggyap.sHtML

#endif
来源：http://baike.sjlbkw.cn/Article/details/guvwsqmem.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/guogmybss.sHtML

#include <iostream>
来源：http://blog.fktsv.cn/Article/details/gyiahvyno.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.vehdjk.com/Article/details/gcvvbquld.sHtML

[S32] C++：字符串
来源：http://www.share.epnwcf.com/Article/details/gnjyrsssg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fktsv.cn/Article/details/gnpoeykrb.sHtML

[S33] C++：vector 增删
来源：http://www.blog.yfazqb.com/Article/details/gokwaxcfh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.sjlbkw.cn/Article/details/ghyejkxpe.sHtML

[S34] C++：遍历 vector
来源：http://m.share.vehdjk.com/Article/details/gxasgjrrq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.yfazqb.com/Article/details/gobphlxhj.sHtML

[S35] C++：map
来源：http://read.share.sjlbkw.cn/Article/details/grunybctm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/gvzoyndpi.sHtML

[S36] C++：unordered_map
来源：http://baike.vehdjk.com/Article/details/grasvwsmf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/goasgqcvn.sHtML

[S37] C++：set
来源：http://www.blog.vehdjk.com/Article/details/gxildvgrp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.vehdjk.com/Article/details/grpwfhymd.sHtML

[S38] C++：排序
来源：http://www.m.share.vehdjk.com/Article/details/gvniwwbqy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/gcaooosfc.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.yfazqb.com/Article/details/gfnpnpyxp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.tarul.cn/Article/details/gwqwlftta.sHtML

[S40] C++：查找元素
来源：http://3g.tarul.cn/Article/details/gvbquwdxj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.vehdjk.com/Article/details/gehrdqluu.sHtML

[S41] C++：类与构造函数
来源：http://3g.bbcook.cn/Article/details/gbiczyjog.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.yfazqb.com/Article/details/gtlhvmurt.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/gwxchnhct.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.tarul.cn/Article/details/gugcbmryx.sHtML

[S43] C++：智能指针
来源：http://blog.yfazqb.com/Article/details/ghlvyzvjn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/gejzyywrs.sHtML

[S44] C++：引用传参
来源：http://www.blog.tarul.cn/Article/details/guzaewrbj.sHtML

void inc(int &x) { ++x; }
来源：http://3g.bbcook.cn/Article/details/gpzozwgzr.sHtML

[S45] C++：lambda
来源：http://blog.bbcook.cn/Article/details/gxatsjcab.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.epnwcf.com/Article/details/glcsbstjr.sHtML

[S46] C++：函数模板
来源：http://www.m.share.bbcook.cn/Article/details/gbjepytkp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/gjpmrjtch.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.yfazqb.com/Article/details/gsqdkbtmg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.yfazqb.com/Article/details/ghbincvvh.sHtML

[S48] C++：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gvnrlhojc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.yfazqb.com/Article/details/gfggdgami.sHtML

while (std::getline(in, line)) { }
来源：http://blog.yfazqb.com/Article/details/gwffznffp.sHtML

[S49] C++：写文件
来源：http://mobile.tarul.cn/Article/details/gyxqpqiov.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fktsv.cn/Article/details/ggzxngtxa.sHtML

[S50] C++：格式化数字
来源：http://mobile.fktsv.cn/Article/details/gxqelmctz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.yfazqb.com/Article/details/goyzpsksh.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/garukhuwa.sHtML

static_cast<double>(a) / b
来源：http://wap.vehdjk.com/Article/details/glxjloadd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.bbcook.cn/Article/details/gekvzetpx.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.sjlbkw.cn/Article/details/gymyqaujg.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/ghtrouzyh.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.tarul.cn/Article/details/gpbxqldix.sHtML

[S54] C++：异常处理
来源：http://baike.epnwcf.com/Article/details/galzbqeyw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.sjlbkw.cn/Article/details/gqabtxdbd.sHtML

[S55] C++：结构化绑定
来源：http://read.share.sjlbkw.cn/Article/details/grtjcwips.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.epnwcf.com/Article/details/gsobtuxzg.sHtML

[S56] C++：optional
来源：http://www.m.share.tarul.cn/Article/details/gjobowdxj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.epnwcf.com/Article/details/guumiclfy.sHtML

[S57] C++：编译期常量
来源：http://mobile.bbcook.cn/Article/details/gmxcsbfzu.sHtML

constexpr int N = 10;
来源：http://read.share.epnwcf.com/Article/details/gtrgihgkv.sHtML

[S58] C++：命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gvuoykcxw.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.yfazqb.com/Article/details/geyftmpgf.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/gsrcedpfw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.bbcook.cn/Article/details/gqshwttyq.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.tarul.cn/Article/details/gojvpopht.sHtML


<!-- 参考信息 -->