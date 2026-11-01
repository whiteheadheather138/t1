代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.blog.vehdjk.com/Article/details/gawloamet.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.vehdjk.com/Article/details/gzlxymaez.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.tarul.cn/Article/details/gqlitudix.sHtML

[Q89] 判断表是否存在
来源：http://wap.bbcook.cn/Article/details/gfekcxjro.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fktsv.cn/Article/details/giyszsugz.sHtML

[Q90] 生成序号列
来源：http://m.share.tarul.cn/Article/details/gwmjeqqxn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.vehdjk.com/Article/details/gdtrdnekp.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxbxtwoso.sHtML

R. Bash 专题
来源：http://read.share.sjlbkw.cn/Article/details/gereoatdr.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gziivdvvs.sHtML

[R01] shebang 与严格模式
来源：http://www.share.bbcook.cn/Article/details/gxnwvxbyy.sHtML

#!/usr/bin/env bash
来源：http://wap.vehdjk.com/Article/details/gcgvzqbek.sHtML

set -euo pipefail
来源：http://baike.epnwcf.com/Article/details/grcdzscwh.sHtML

[R02] 变量赋值与使用
来源：http://www.share.epnwcf.com/Article/details/gadpxtkaa.sHtML

name="Tom"; echo "$name"
来源：http://3g.bbcook.cn/Article/details/guxomzucp.sHtML

[R03] 只读变量
来源：http://www.blog.bbcook.cn/Article/details/gwokpxuja.sHtML

readonly PI=3.14
来源：http://read.share.sjlbkw.cn/Article/details/gkwnkipwz.sHtML

[R04] 位置参数
来源：http://m.share.sjlbkw.cn/Article/details/geusjdmna.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.vehdjk.com/Article/details/gmlnzremh.sHtML

[R05] 参数默认值
来源：http://mobile.bbcook.cn/Article/details/gqgcffrak.sHtML

name="${1:-default}"
来源：http://blog.yfazqb.com/Article/details/gvtrwgihi.sHtML

[R06] 判断命令是否存在
来源：http://www.share.epnwcf.com/Article/details/gbsgpvkui.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/gsmyzfyxe.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gqadbzaaq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.bbcook.cn/Article/details/gfhgpjfox.sHtML

[R08] 数值比较
来源：http://read.share.tarul.cn/Article/details/gtbdzzwnp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gbwspfudg.sHtML

[R09] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gwynagowu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.epnwcf.com/Article/details/gaqtnrfgf.sHtML

[R10] 正则匹配
来源：http://read.share.epnwcf.com/Article/details/guqerouvu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gizduwgph.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/gxkfaswmy.sHtML

case "$1" in
来源：http://www.m.share.vehdjk.com/Article/details/gnbzotght.sHtML

start) echo "启动" ;;
来源：http://m.share.vehdjk.com/Article/details/gzujkmphl.sHtML

stop)  echo "停止" ;;
来源：http://www.share.epnwcf.com/Article/details/ghleoersg.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.bbcook.cn/Article/details/gksqhzrny.sHtML

esac
来源：http://blog.fktsv.cn/Article/details/gzidfrcwq.sHtML

[R12] for 遍历文件
来源：http://m.share.fktsv.cn/Article/details/gxbdmysfo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.vehdjk.com/Article/details/gvxhytkyp.sHtML

[R13] for 计数循环
来源：http://www.m.share.epnwcf.com/Article/details/gfkrrdiql.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/gxlvoswqa.sHtML

[R14] C 风格 for
来源：http://www.blog.vehdjk.com/Article/details/guauihcsi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/ghhzaoomb.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvmzgyke.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.epnwcf.com/Article/details/gvxlvzgdi.sHtML

[R16] until 等待条件
来源：http://m.share.vehdjk.com/Article/details/geecgcrnx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/ginqxmaot.sHtML

[R17] 数组定义与取值
来源：http://blog.yfazqb.com/Article/details/gsikylngp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.sjlbkw.cn/Article/details/gguxqhbpw.sHtML

[R18] 遍历数组
来源：http://wap.bbcook.cn/Article/details/gcebttqzn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fktsv.cn/Article/details/gtcjcjtha.sHtML

[R19] 数组长度
来源：http://wap.sjlbkw.cn/Article/details/gkxugwvjz.sHtML

echo "${#arr[@]}"
来源：http://mobile.tarul.cn/Article/details/gszvgwjuz.sHtML

[R20] 关联数组（字典）
来源：http://mobile.tarul.cn/Article/details/gphdtsgvi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.sjlbkw.cn/Article/details/gewgkpllp.sHtML

[R21] 字符串长度
来源：http://baike.tarul.cn/Article/details/gcaymcvge.sHtML

echo "${#s}"
来源：http://blog.fktsv.cn/Article/details/ggufvjmon.sHtML

[R22] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/ghdjjoegp.sHtML

echo "${s:0:5}"
来源：http://m.share.vehdjk.com/Article/details/gzaplyhqh.sHtML

[R23] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gcwdoizsb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.sjlbkw.cn/Article/details/gkldapjmj.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gesttcszo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fktsv.cn/Article/details/ghutsywmd.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.bbcook.cn/Article/details/gzqriofkm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.tarul.cn/Article/details/gqzrfciys.sHtML

[R26] 命令替换
来源：http://m.share.epnwcf.com/Article/details/gkrddvnqh.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.tarul.cn/Article/details/gobtzqllp.sHtML

[R27] 算术展开
来源：http://www.share.vehdjk.com/Article/details/gyjuoqpie.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fktsv.cn/Article/details/goybokbna.sHtML

[R28] 浮点运算
来源：http://m.share.yfazqb.com/Article/details/glhpvtguh.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.epnwcf.com/Article/details/grfwbachz.sHtML

[R29] 定义函数
来源：http://mobile.yfazqb.com/Article/details/gqcbmcpwq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.tarul.cn/Article/details/gsxdgcoez.sHtML

[R30] 函数返回状态码
来源：http://m.share.sjlbkw.cn/Article/details/gwynajwtj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.vehdjk.com/Article/details/gxuuvfqif.sHtML

[R31] 局部变量
来源：http://m.share.yfazqb.com/Article/details/guzzaknsh.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.tarul.cn/Article/details/gxcshfpob.sHtML

[R32] 参数个数校验
来源：http://m.share.vehdjk.com/Article/details/gykpzcynv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/gnbuitmsc.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fktsv.cn/Article/details/gwrtpiwim.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fktsv.cn/Article/details/guvneilbk.sHtML

[R34] 退出时清理
来源：http://www.blog.sjlbkw.cn/Article/details/gqmkcjfvk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gpeontfxd.sHtML

[R35] 后台执行并等待
来源：http://wap.sjlbkw.cn/Article/details/gwxzdswry.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.epnwcf.com/Article/details/ghwmuhbxw.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/gyjqgtmit.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fktsv.cn/Article/details/gisvaskzu.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/gglsmuadi.sHtML

files=$(ls -1)
来源：http://baike.bbcook.cn/Article/details/gbidujpmt.sHtML

[R38] 管道串联
来源：http://blog.tarul.cn/Article/details/gnfblyhpn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.yfazqb.com/Article/details/gqzwmjcqm.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.sjlbkw.cn/Article/details/ghvhwurxc.sHtML

cmd > out.log 2>&1
来源：http://m.share.yfazqb.com/Article/details/gvqnncaup.sHtML

[R40] 追加写日志
来源：http://mobile.vehdjk.com/Article/details/gskgaxqem.sHtML

echo "log" >> out.log
来源：http://3g.vehdjk.com/Article/details/gwfjmipmm.sHtML

[R41] 丢弃输出
来源：http://www.m.share.yfazqb.com/Article/details/gdlwobjwn.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.bbcook.cn/Article/details/ggnuqxthi.sHtML

[R42] 输入重定向
来源：http://3g.fktsv.cn/Article/details/grarhrult.sHtML

wc -l < a.txt
来源：http://read.share.vehdjk.com/Article/details/glimuhnbb.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.yfazqb.com/Article/details/gximlnugc.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/govbhckkw.sHtML

[R44] 按修改时间查找
来源：http://baike.tarul.cn/Article/details/gfdujnkvl.sHtML

find . -mtime -7 -type f
来源：http://wap.sjlbkw.cn/Article/details/gqzgelgqq.sHtML

[R45] 批量删除
来源：http://read.share.sjlbkw.cn/Article/details/gdjyqiiwq.sHtML

find . -name "*.tmp" -delete
来源：http://baike.yfazqb.com/Article/details/glrpefcvt.sHtML

[R46] 递归替换文件内容
来源：http://blog.vehdjk.com/Article/details/gjfkqrdhg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.yfazqb.com/Article/details/gubnzdkkv.sHtML

[R47] sed 单行替换
来源：http://m.share.bbcook.cn/Article/details/guogbtobx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fktsv.cn/Article/details/glmnovpbv.sHtML

[R48] awk 取指定列
来源：http://www.share.vehdjk.com/Article/details/ggalmyjgs.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gkcwulxnb.sHtML

[R49] awk 带条件
来源：http://mobile.epnwcf.com/Article/details/gzjqqqmvt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.tarul.cn/Article/details/gkkzpqwrr.sHtML

[R50] awk 求和
来源：http://baike.tarul.cn/Article/details/geqzvniik.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gkifynkdi.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fktsv.cn/Article/details/gfhyggiei.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.epnwcf.com/Article/details/gqmbnrfpy.sHtML

[R52] 统计行数
来源：http://read.share.bbcook.cn/Article/details/gnyomgnnu.sHtML

wc -l a.txt
来源：http://www.blog.epnwcf.com/Article/details/gzdzcfknz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.sjlbkw.cn/Article/details/ggljnpkak.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fktsv.cn/Article/details/gbureglcl.sHtML

[R54] 比较两个文件
来源：http://wap.vehdjk.com/Article/details/gogmhcmls.sHtML

diff a.txt b.txt
来源：http://3g.fktsv.cn/Article/details/glsdfxofw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.tarul.cn/Article/details/ggcokprmk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/gjdifhgrz.sHtML

[R56] 远程拷贝
来源：http://wap.vehdjk.com/Article/details/gnizshkrw.sHtML

scp file user@host:/path/
来源：http://www.m.share.yfazqb.com/Article/details/gwownqwws.sHtML

[R57] 远程执行命令
来源：http://wap.yfazqb.com/Article/details/gsuebjlbz.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gwociurnn.sHtML

[R58] 下载文件
来源：http://www.share.bbcook.cn/Article/details/gmlaxxgvc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.yfazqb.com/Article/details/gtoeajtsw.sHtML

[R59] 发 POST JSON
来源：http://m.share.bbcook.cn/Article/details/gottrwzgd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.yfazqb.com/Article/details/gsrtbbmjt.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gmdgcdwur.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.bbcook.cn/Article/details/gcsvgctdg.sHtML

[R61] 磁盘占用
来源：http://blog.tarul.cn/Article/details/gpvlarkin.sHtML

df -h;  du -sh *
来源：http://www.share.sjlbkw.cn/Article/details/gvnpmbgsc.sHtML

[R62] 找最占空间的文件
来源：http://mobile.epnwcf.com/Article/details/gtblcckyy.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.tarul.cn/Article/details/glwdnzxei.sHtML

[R63] 内存与进程
来源：http://m.share.fktsv.cn/Article/details/giywcpkzf.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.yfazqb.com/Article/details/gbqkhrkcj.sHtML

[R64] 结束进程
来源：http://baike.tarul.cn/Article/details/glkakbodz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.epnwcf.com/Article/details/gqkcewjqu.sHtML

[R65] 查看端口占用
来源：http://baike.sjlbkw.cn/Article/details/gdmvysjyb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.epnwcf.com/Article/details/gfcejfctr.sHtML

[R66] 定时任务
来源：http://read.share.vehdjk.com/Article/details/ganzvgecu.sHtML

crontab -e;  crontab -l
来源：http://read.share.yfazqb.com/Article/details/gjmbzsolm.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.epnwcf.com/Article/details/gayzqjnaa.sHtML

openssl rand -hex 16
来源：http://3g.epnwcf.com/Article/details/gwffcgoan.sHtML

[R68] 计算文件校验值
来源：http://3g.fktsv.cn/Article/details/gklbntxez.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.tarul.cn/Article/details/gktqpdfco.sHtML

[R69] 生成随机密码
来源：http://baike.vehdjk.com/Article/details/gsosndddj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.tarul.cn/Article/details/gdorqohcw.sHtML

[R70] 时间戳与互转
来源：http://mobile.vehdjk.com/Article/details/gpfrnkszh.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.yfazqb.com/Article/details/gmfqkwtcv.sHtML

[R71] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gklwfoxqg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.tarul.cn/Article/details/gajnurgec.sHtML

[R72] 等待端口就绪
来源：http://3g.sjlbkw.cn/Article/details/gzscjxqth.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gmzgvqdsc.sHtML

[R73] 分割大日志
来源：http://read.share.yfazqb.com/Article/details/gljtgjkon.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.vehdjk.com/Article/details/gcwwxohsp.sHtML

[R74] 批量重命名
来源：http://wap.yfazqb.com/Article/details/gcusytflf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.sjlbkw.cn/Article/details/gnalpkaga.sHtML

[R75] 导出环境变量
来源：http://read.share.bbcook.cn/Article/details/gvbcixpdo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.epnwcf.com/Article/details/gfdzhgsdy.sHtML

[R76] 使用临时文件
来源：http://wap.bbcook.cn/Article/details/grimftyoh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fktsv.cn/Article/details/gnfbtmkgo.sHtML

[R77] 读取用户输入
来源：http://blog.tarul.cn/Article/details/gsgjhijhy.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/gqxgfaujn.sHtML

[R78] 交互式菜单
来源：http://www.blog.yfazqb.com/Article/details/geazanhzi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.bbcook.cn/Article/details/gcloapijk.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.yfazqb.com/Article/details/gmwxuyzua.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.epnwcf.com/Article/details/gmzlsdukg.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/gpguaxstb.sHtML

time ./run.sh
来源：http://read.share.tarul.cn/Article/details/ggjblygpw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gkzgsewoe.sHtML

S. C / C++ 专题
来源：http://www.blog.yfazqb.com/Article/details/gozqwikjy.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gsnwlckmm.sHtML

[S01] C：Hello World
来源：http://baike.fktsv.cn/Article/details/gzinvzolj.sHtML

#include <stdio.h>
来源：http://3g.vehdjk.com/Article/details/gkjpzmgji.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.tarul.cn/Article/details/gwtvkiepd.sHtML

[S02] C：变量与格式化输出
来源：http://3g.vehdjk.com/Article/details/ggetndusz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.tarul.cn/Article/details/gimlvlawk.sHtML

[S03] C：读入整数
来源：http://www.m.share.tarul.cn/Article/details/gvnddgpln.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.bbcook.cn/Article/details/gdftvzkwc.sHtML

[S04] C：字符串复制
来源：http://m.share.vehdjk.com/Article/details/gxhkxmlvm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.bbcook.cn/Article/details/gvcethsty.sHtML

[S05] C：字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gwewplvly.sHtML

strlen(s)
来源：http://m.share.tarul.cn/Article/details/ghdlkphuv.sHtML

[S06] C：字符串比较
来源：http://wap.tarul.cn/Article/details/gdeqqfoah.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/ggstasywq.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.tarul.cn/Article/details/gqhuoeuvd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fktsv.cn/Article/details/gfrvnyjzu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.yfazqb.com/Article/details/gaijkopsp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.vehdjk.com/Article/details/gakdpfhzw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.tarul.cn/Article/details/gddpyamig.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.vehdjk.com/Article/details/ggzwbngqg.sHtML

[S10] C：指针与解引用
来源：http://www.share.tarul.cn/Article/details/gbfldjgra.sHtML

int *p = &a;  *p = 5;
来源：http://blog.bbcook.cn/Article/details/gizmewhfz.sHtML

[S11] C：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gcduzeojc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.epnwcf.com/Article/details/gqwedymgv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.yfazqb.com/Article/details/gqqybghmk.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gyduartdb.sHtML

[S12] C：写文件
来源：http://www.blog.yfazqb.com/Article/details/gtspowjgc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.vehdjk.com/Article/details/ghefcowkp.sHtML

[S13] C：宏定义
来源：http://blog.yfazqb.com/Article/details/gxosoixjn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.epnwcf.com/Article/details/gcbwljjmb.sHtML

[S14] C：枚举
来源：http://www.m.share.vehdjk.com/Article/details/gqehtmxus.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.sjlbkw.cn/Article/details/gejiwkjuj.sHtML

[S15] C：类型转换
来源：http://baike.yfazqb.com/Article/details/gzuqjnvmw.sHtML

(double) a / b
来源：http://www.share.bbcook.cn/Article/details/gtlydteff.sHtML

[S16] C：位操作置位
来源：http://www.share.epnwcf.com/Article/details/ggheicyqg.sHtML

x |= (1 << 3);
来源：http://www.share.sjlbkw.cn/Article/details/gwxkirnwf.sHtML

[S17] C：安全拼接字符串
来源：http://wap.bbcook.cn/Article/details/genidpetq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.bbcook.cn/Article/details/gphzinois.sHtML

[S18] C：命令行参数
来源：http://www.share.bbcook.cn/Article/details/geqgzqffq.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.yfazqb.com/Article/details/gqqesnekd.sHtML

[S19] C：快速排序
来源：http://www.m.share.fktsv.cn/Article/details/geszmpcbp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gyehsfnuw.sHtML

[S20] C：二分查找
来源：http://baike.tarul.cn/Article/details/gpoqirhhs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gjdwthqxa.sHtML

[S21] C：字符类别判断
来源：http://blog.vehdjk.com/Article/details/gxpicluit.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fktsv.cn/Article/details/gggjghcqc.sHtML

[S22] C：字符串转数字
来源：http://mobile.bbcook.cn/Article/details/gwvuvpyqt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.bbcook.cn/Article/details/gtdcfpryg.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/gvecrlsve.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fktsv.cn/Article/details/gltyvaiqr.sHtML

[S24] C：获取本地时间
来源：http://blog.vehdjk.com/Article/details/gxpnszngx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.epnwcf.com/Article/details/gvtfkfsoy.sHtML

[S25] C：内存拷贝
来源：http://wap.sjlbkw.cn/Article/details/gykjygxhm.sHtML

memcpy(dst, src, n);
来源：http://3g.yfazqb.com/Article/details/gcquoenat.sHtML

[S26] C：内存清零
来源：http://blog.bbcook.cn/Article/details/gkqdgnvyy.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/gnpcvosip.sHtML

[S27] C：定义常量
来源：http://www.blog.sjlbkw.cn/Article/details/ghhkzeyyc.sHtML

const double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gpthopcsd.sHtML

[S28] C：静态变量
来源：http://m.share.epnwcf.com/Article/details/gyxjfknst.sHtML

static int counter = 0;
来源：http://3g.fktsv.cn/Article/details/gfcgekpyf.sHtML

[S29] C：变参函数
来源：http://blog.fktsv.cn/Article/details/grjxippez.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.vehdjk.com/Article/details/gejvmwpjn.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fktsv.cn/Article/details/gajanfrzn.sHtML

#ifndef X_H
来源：http://mobile.tarul.cn/Article/details/gimgoxecp.sHtML

#define X_H
来源：http://read.share.bbcook.cn/Article/details/gbhrykljz.sHtML

#endif
来源：http://3g.sjlbkw.cn/Article/details/gsyiebxfr.sHtML

[S31] C++：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gvxubtvve.sHtML

#include <iostream>
来源：http://blog.fktsv.cn/Article/details/gpxcvvvou.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.epnwcf.com/Article/details/ghjfztkgm.sHtML

[S32] C++：字符串
来源：http://blog.sjlbkw.cn/Article/details/gejgykmbx.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fktsv.cn/Article/details/gchqlwmwb.sHtML

[S33] C++：vector 增删
来源：http://baike.vehdjk.com/Article/details/gtroncgzy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.sjlbkw.cn/Article/details/gwpaxxqdg.sHtML

[S34] C++：遍历 vector
来源：http://3g.fktsv.cn/Article/details/gleqkofrt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.yfazqb.com/Article/details/gomhhrbqr.sHtML

[S35] C++：map
来源：http://3g.yfazqb.com/Article/details/gzcslzmgz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/gfuzertlz.sHtML

[S36] C++：unordered_map
来源：http://baike.vehdjk.com/Article/details/gdqregrot.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gwahjlckv.sHtML

[S37] C++：set
来源：http://wap.yfazqb.com/Article/details/goqvjmscq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/gwahauoio.sHtML

[S38] C++：排序
来源：http://blog.bbcook.cn/Article/details/gxiqmcidv.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fktsv.cn/Article/details/gdhbbbyqa.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.bbcook.cn/Article/details/gzvrxblvd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.yfazqb.com/Article/details/gnnzydsbg.sHtML

[S40] C++：查找元素
来源：http://mobile.yfazqb.com/Article/details/gsrkirjip.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.vehdjk.com/Article/details/gpmsjqwhg.sHtML

[S41] C++：类与构造函数
来源：http://m.share.vehdjk.com/Article/details/gulojbqnw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.yfazqb.com/Article/details/gbvtmvcej.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/gotscqgwu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/gxcjpazky.sHtML

[S43] C++：智能指针
来源：http://www.blog.epnwcf.com/Article/details/gkpftvkjt.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fktsv.cn/Article/details/gtbucnaxv.sHtML

[S44] C++：引用传参
来源：http://www.blog.sjlbkw.cn/Article/details/gvwahgakb.sHtML

void inc(int &x) { ++x; }
来源：http://wap.tarul.cn/Article/details/gzhvugmvm.sHtML

[S45] C++：lambda
来源：http://m.share.sjlbkw.cn/Article/details/glqvjnauz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/gzljhwgut.sHtML

[S46] C++：函数模板
来源：http://mobile.vehdjk.com/Article/details/gbaxsnspm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.yfazqb.com/Article/details/gdztqgurd.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.sjlbkw.cn/Article/details/ggqxnlhon.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/gmnpfhdoq.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gowcxtcsm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.sjlbkw.cn/Article/details/gsbbdmnte.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.vehdjk.com/Article/details/gnydhuckx.sHtML

[S49] C++：写文件
来源：http://blog.yfazqb.com/Article/details/gulvjfnlc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.vehdjk.com/Article/details/gptnkrces.sHtML

[S50] C++：格式化数字
来源：http://read.share.tarul.cn/Article/details/gjutkravy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/grmxajjfv.sHtML

[S51] C++：显式类型转换
来源：http://3g.vehdjk.com/Article/details/gzktmhfuu.sHtML

static_cast<double>(a) / b
来源：http://www.share.vehdjk.com/Article/details/gyphyicak.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.vehdjk.com/Article/details/gcdykhbtd.sHtML

int size() const noexcept { return n_; }
来源：http://blog.tarul.cn/Article/details/gxtgtducq.sHtML

[S53] C++：移动语义
来源：http://read.share.sjlbkw.cn/Article/details/gxkdypkmz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.epnwcf.com/Article/details/gvdrxambk.sHtML

[S54] C++：异常处理
来源：http://m.share.epnwcf.com/Article/details/gdmwpghwi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fktsv.cn/Article/details/grqppgguo.sHtML

[S55] C++：结构化绑定
来源：http://www.share.tarul.cn/Article/details/gevgfgvvk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.vehdjk.com/Article/details/gbrexlfbr.sHtML

[S56] C++：optional
来源：http://wap.vehdjk.com/Article/details/gujjbgxxv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.bbcook.cn/Article/details/gvrlmqtua.sHtML

[S57] C++：编译期常量
来源：http://blog.bbcook.cn/Article/details/gibjgzczl.sHtML

constexpr int N = 10;
来源：http://blog.vehdjk.com/Article/details/gupnnlyyg.sHtML

[S58] C++：命名空间
来源：http://read.share.vehdjk.com/Article/details/gqwirdhkq.sHtML


<!-- 参考信息 -->