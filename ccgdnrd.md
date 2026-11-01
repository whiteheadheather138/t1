代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://read.share.bbcook.cn/Article/details/gaetkkbmh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fktsv.cn/Article/details/gceoflhbf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.yfazqb.com/Article/details/gpjotnhmx.sHtML

[Q89] 判断表是否存在
来源：http://wap.vehdjk.com/Article/details/gkiveivzx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.sjlbkw.cn/Article/details/guogmvwkx.sHtML

[Q90] 生成序号列
来源：http://m.share.vehdjk.com/Article/details/gjgwtdypd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.tarul.cn/Article/details/gzudalogj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmeyldknb.sHtML

R. Bash 专题
来源：http://www.share.tarul.cn/Article/details/gshqsidme.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gtbjugntw.sHtML

[R01] shebang 与严格模式
来源：http://wap.yfazqb.com/Article/details/gzjvdwkep.sHtML

#!/usr/bin/env bash
来源：http://www.share.sjlbkw.cn/Article/details/golxglmnp.sHtML

set -euo pipefail
来源：http://m.share.yfazqb.com/Article/details/gjukkmele.sHtML

[R02] 变量赋值与使用
来源：http://m.share.bbcook.cn/Article/details/gncqzftty.sHtML

name="Tom"; echo "$name"
来源：http://m.share.bbcook.cn/Article/details/grxfjvbsq.sHtML

[R03] 只读变量
来源：http://m.share.yfazqb.com/Article/details/gkhizaekw.sHtML

readonly PI=3.14
来源：http://www.m.share.epnwcf.com/Article/details/gxphgesbd.sHtML

[R04] 位置参数
来源：http://read.share.fktsv.cn/Article/details/geqyyzkiy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.bbcook.cn/Article/details/gajrkwirm.sHtML

[R05] 参数默认值
来源：http://www.share.vehdjk.com/Article/details/guwjsdanf.sHtML

name="${1:-default}"
来源：http://wap.sjlbkw.cn/Article/details/gximlhwhm.sHtML

[R06] 判断命令是否存在
来源：http://3g.bbcook.cn/Article/details/gizlitsvr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gannlxynl.sHtML

[R07] if 判断文件
来源：http://www.m.share.fktsv.cn/Article/details/goopayhuz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gfkgyqmyr.sHtML

[R08] 数值比较
来源：http://read.share.bbcook.cn/Article/details/gnpgqagqo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.bbcook.cn/Article/details/guhintwmi.sHtML

[R09] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/gzqtxugfw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.bbcook.cn/Article/details/gbzhgxzcm.sHtML

[R10] 正则匹配
来源：http://read.share.fktsv.cn/Article/details/gkpssdqyx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fktsv.cn/Article/details/gxxvmmtxx.sHtML

[R11] case 多分支
来源：http://wap.fktsv.cn/Article/details/gelbxovny.sHtML

case "$1" in
来源：http://mobile.fktsv.cn/Article/details/guguxkgjg.sHtML

start) echo "启动" ;;
来源：http://blog.bbcook.cn/Article/details/gmdajaubg.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gpvxtgpos.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.yfazqb.com/Article/details/gjmxcvjqu.sHtML

esac
来源：http://www.m.share.yfazqb.com/Article/details/ghnigakew.sHtML

[R12] for 遍历文件
来源：http://www.share.sjlbkw.cn/Article/details/gajtoyvik.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.epnwcf.com/Article/details/ggofbckoy.sHtML

[R13] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gevuzgldk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gglrxtnem.sHtML

[R14] C 风格 for
来源：http://mobile.yfazqb.com/Article/details/gqhlcwdaa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/gefarfwcl.sHtML

[R15] while 逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gtaalxvtl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gseziebzc.sHtML

[R16] until 等待条件
来源：http://wap.epnwcf.com/Article/details/gqneaatjw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/groxybqct.sHtML

[R17] 数组定义与取值
来源：http://www.blog.bbcook.cn/Article/details/gjdyewjkh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fktsv.cn/Article/details/gltpccdgq.sHtML

[R18] 遍历数组
来源：http://mobile.tarul.cn/Article/details/grbdovadr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.sjlbkw.cn/Article/details/gtrqsrsiw.sHtML

[R19] 数组长度
来源：http://wap.vehdjk.com/Article/details/gnbmriltw.sHtML

echo "${#arr[@]}"
来源：http://blog.vehdjk.com/Article/details/goraipahm.sHtML

[R20] 关联数组（字典）
来源：http://read.share.yfazqb.com/Article/details/ggbfforou.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.yfazqb.com/Article/details/gvgqskzod.sHtML

[R21] 字符串长度
来源：http://blog.bbcook.cn/Article/details/gktuqfnap.sHtML

echo "${#s}"
来源：http://www.blog.vehdjk.com/Article/details/gxmsminis.sHtML

[R22] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gupxobggp.sHtML

echo "${s:0:5}"
来源：http://www.share.fktsv.cn/Article/details/gweqiokuj.sHtML

[R23] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/grxxqdity.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.tarul.cn/Article/details/gqakgsqvz.sHtML

[R24] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gufoxkqad.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.vehdjk.com/Article/details/gkymdcbnu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.vehdjk.com/Article/details/ghwmjkpvt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.sjlbkw.cn/Article/details/gqxbooabd.sHtML

[R26] 命令替换
来源：http://baike.vehdjk.com/Article/details/glalsuaqw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.bbcook.cn/Article/details/gmusnbegg.sHtML

[R27] 算术展开
来源：http://wap.bbcook.cn/Article/details/guvxkisxl.sHtML

echo $((1 + 2 * 3))
来源：http://baike.bbcook.cn/Article/details/gipmefjvj.sHtML

[R28] 浮点运算
来源：http://3g.bbcook.cn/Article/details/gzkggtpxb.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.tarul.cn/Article/details/gkarkjbkd.sHtML

[R29] 定义函数
来源：http://www.share.vehdjk.com/Article/details/gnlceoaiu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.vehdjk.com/Article/details/gqtwrmgyc.sHtML

[R30] 函数返回状态码
来源：http://blog.epnwcf.com/Article/details/ggpdrfckj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gdsqldxrx.sHtML

[R31] 局部变量
来源：http://3g.epnwcf.com/Article/details/gtvmzfxbl.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.epnwcf.com/Article/details/gignmpkuj.sHtML

[R32] 参数个数校验
来源：http://mobile.tarul.cn/Article/details/geamgdzrb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gycmfffcy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fktsv.cn/Article/details/ggchcjzma.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.epnwcf.com/Article/details/gzueehepg.sHtML

[R34] 退出时清理
来源：http://www.share.tarul.cn/Article/details/grjyxfzrw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gzvlrgpwu.sHtML

[R35] 后台执行并等待
来源：http://www.blog.bbcook.cn/Article/details/gmkrfgyff.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.bbcook.cn/Article/details/gsyrtwaat.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/gtpcnnouv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.epnwcf.com/Article/details/gxxmxvxtj.sHtML

[R37] 把输出赋给变量
来源：http://mobile.tarul.cn/Article/details/gsivybawj.sHtML

files=$(ls -1)
来源：http://read.share.yfazqb.com/Article/details/gwsntpkzo.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/glwmcjxvb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fktsv.cn/Article/details/gfbendorg.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/ghvrqowki.sHtML

cmd > out.log 2>&1
来源：http://www.share.fktsv.cn/Article/details/gamtutpma.sHtML

[R40] 追加写日志
来源：http://www.blog.tarul.cn/Article/details/gnpumwkqe.sHtML

echo "log" >> out.log
来源：http://read.share.yfazqb.com/Article/details/gxqutjwne.sHtML

[R41] 丢弃输出
来源：http://wap.tarul.cn/Article/details/gxduvbqtb.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/gogjakufw.sHtML

[R42] 输入重定向
来源：http://wap.fktsv.cn/Article/details/gavvqcqfs.sHtML

wc -l < a.txt
来源：http://read.share.epnwcf.com/Article/details/gkpkvuqjq.sHtML

[R43] 按名字查找文件
来源：http://3g.epnwcf.com/Article/details/gypcqnicf.sHtML

find . -name "*.log" -type f
来源：http://www.share.fktsv.cn/Article/details/gypooxhip.sHtML

[R44] 按修改时间查找
来源：http://m.share.epnwcf.com/Article/details/ghcucbswi.sHtML

find . -mtime -7 -type f
来源：http://mobile.bbcook.cn/Article/details/gbagohxgr.sHtML

[R45] 批量删除
来源：http://www.blog.yfazqb.com/Article/details/gjagwmxpl.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gvfzlztjp.sHtML

[R46] 递归替换文件内容
来源：http://3g.vehdjk.com/Article/details/gxuxajigu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.epnwcf.com/Article/details/gxxdirazo.sHtML

[R47] sed 单行替换
来源：http://read.share.epnwcf.com/Article/details/gvceytndr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.tarul.cn/Article/details/grmxdpkaf.sHtML

[R48] awk 取指定列
来源：http://www.share.bbcook.cn/Article/details/gkkrnrxfh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gdxrcfhif.sHtML

[R49] awk 带条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gegxluqla.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.tarul.cn/Article/details/gozogezea.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/gpftteqsh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.tarul.cn/Article/details/gqixauiun.sHtML

[R51] 排序去重取前几
来源：http://m.share.vehdjk.com/Article/details/gsdsbixzm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.sjlbkw.cn/Article/details/gjjczhfxw.sHtML

[R52] 统计行数
来源：http://www.m.share.tarul.cn/Article/details/gkjljktqi.sHtML

wc -l a.txt
来源：http://www.m.share.tarul.cn/Article/details/gmuwzzncq.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.epnwcf.com/Article/details/gesepbcav.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.vehdjk.com/Article/details/gtazrpdcq.sHtML

[R54] 比较两个文件
来源：http://m.share.vehdjk.com/Article/details/glfckmgyz.sHtML

diff a.txt b.txt
来源：http://3g.sjlbkw.cn/Article/details/gtcuukgax.sHtML

[R55] 压缩与解压
来源：http://m.share.sjlbkw.cn/Article/details/ghzcgtfaj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.bbcook.cn/Article/details/gqorkajwu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gevzqchag.sHtML

scp file user@host:/path/
来源：http://3g.tarul.cn/Article/details/gcenpgpen.sHtML

[R57] 远程执行命令
来源：http://www.share.sjlbkw.cn/Article/details/gwmylsdmf.sHtML

ssh user@host 'uptime'
来源：http://www.share.sjlbkw.cn/Article/details/gaylxdigv.sHtML

[R58] 下载文件
来源：http://baike.fktsv.cn/Article/details/gvrzsjkbs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.epnwcf.com/Article/details/gyawvzpwo.sHtML

[R59] 发 POST JSON
来源：http://blog.yfazqb.com/Article/details/gwdpsvaji.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.sjlbkw.cn/Article/details/gjygjaqjb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gnktapbzw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/glzqnzhnt.sHtML

[R61] 磁盘占用
来源：http://m.share.tarul.cn/Article/details/glftnejzy.sHtML

df -h;  du -sh *
来源：http://www.share.fktsv.cn/Article/details/gbexlcxeb.sHtML

[R62] 找最占空间的文件
来源：http://m.share.vehdjk.com/Article/details/gcfnoevrc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fktsv.cn/Article/details/gwygmdaoe.sHtML

[R63] 内存与进程
来源：http://wap.yfazqb.com/Article/details/gnwkchteg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.epnwcf.com/Article/details/gtgolyhbm.sHtML

[R64] 结束进程
来源：http://m.share.yfazqb.com/Article/details/gjkksborb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.sjlbkw.cn/Article/details/gfkkqgtmh.sHtML

[R65] 查看端口占用
来源：http://wap.yfazqb.com/Article/details/gofcnjpeg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.epnwcf.com/Article/details/gdgxsmjhv.sHtML

[R66] 定时任务
来源：http://mobile.bbcook.cn/Article/details/gmjrpsjes.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.yfazqb.com/Article/details/gujjwilie.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.tarul.cn/Article/details/gekrxkpjx.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/gubzuenpp.sHtML

[R68] 计算文件校验值
来源：http://3g.vehdjk.com/Article/details/gccnjgitk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.sjlbkw.cn/Article/details/gseemojzn.sHtML

[R69] 生成随机密码
来源：http://3g.fktsv.cn/Article/details/gnqhrzyum.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.yfazqb.com/Article/details/gednfbhvu.sHtML

[R70] 时间戳与互转
来源：http://blog.bbcook.cn/Article/details/gghryydev.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.epnwcf.com/Article/details/glbiqywax.sHtML

[R71] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gsrmgesot.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.tarul.cn/Article/details/gvcbqvamr.sHtML

[R72] 等待端口就绪
来源：http://baike.sjlbkw.cn/Article/details/gzmelfcpf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/gzjsxceao.sHtML

[R73] 分割大日志
来源：http://www.blog.sjlbkw.cn/Article/details/grcgjwtix.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/gnuxrnlli.sHtML

[R74] 批量重命名
来源：http://mobile.sjlbkw.cn/Article/details/gynmfnfat.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.sjlbkw.cn/Article/details/gmuedcywf.sHtML

[R75] 导出环境变量
来源：http://baike.yfazqb.com/Article/details/ghiphvjer.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.tarul.cn/Article/details/gsrudlvtc.sHtML

[R76] 使用临时文件
来源：http://www.blog.bbcook.cn/Article/details/gzrhwrcbm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.vehdjk.com/Article/details/gppgmjevx.sHtML

[R77] 读取用户输入
来源：http://wap.sjlbkw.cn/Article/details/gmztrucff.sHtML

read -rp "请输入: " ans
来源：http://www.share.tarul.cn/Article/details/gbtcflvuj.sHtML

[R78] 交互式菜单
来源：http://read.share.vehdjk.com/Article/details/glnbgsodh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/gchoqxseo.sHtML

[R79] 解析命令行选项
来源：http://baike.vehdjk.com/Article/details/gknlbhrzj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.vehdjk.com/Article/details/grvjoribt.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.vehdjk.com/Article/details/gxicywjjg.sHtML

time ./run.sh
来源：http://www.share.fktsv.cn/Article/details/gcaxwknpi.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzwldpvip.sHtML

S. C / C++ 专题
来源：http://baike.yfazqb.com/Article/details/ghzvxeufk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkjgoxawe.sHtML

[S01] C：Hello World
来源：http://www.share.yfazqb.com/Article/details/gjqcwshoi.sHtML

#include <stdio.h>
来源：http://www.m.share.epnwcf.com/Article/details/gtwquqawg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.vehdjk.com/Article/details/gvpncydsm.sHtML

[S02] C：变量与格式化输出
来源：http://3g.tarul.cn/Article/details/gajemziwe.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.bbcook.cn/Article/details/gflvxtztx.sHtML

[S03] C：读入整数
来源：http://blog.epnwcf.com/Article/details/googliaqu.sHtML

int x; scanf("%d", &x);
来源：http://blog.fktsv.cn/Article/details/gyxsoidhd.sHtML

[S04] C：字符串复制
来源：http://baike.epnwcf.com/Article/details/gqdpwuujt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.tarul.cn/Article/details/grlcmdrhr.sHtML

[S05] C：字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gjhmzdlyf.sHtML

strlen(s)
来源：http://blog.vehdjk.com/Article/details/gzqrzeuzd.sHtML

[S06] C：字符串比较
来源：http://blog.bbcook.cn/Article/details/gnkwjzxph.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/gbibubyxv.sHtML

[S07] C：数组遍历求和
来源：http://mobile.bbcook.cn/Article/details/gurmswyyw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.vehdjk.com/Article/details/gddrkzifi.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.epnwcf.com/Article/details/gjyzhqahw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.sjlbkw.cn/Article/details/gdooixxjy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.yfazqb.com/Article/details/glraeigps.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.tarul.cn/Article/details/gujxjdxsm.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gnlritdyo.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.epnwcf.com/Article/details/gctkrbkvz.sHtML

[S11] C：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/ghzwauonp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.yfazqb.com/Article/details/glgorpigk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.epnwcf.com/Article/details/gzjgxwocc.sHtML

fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/gfveoxyvb.sHtML

[S12] C：写文件
来源：http://wap.vehdjk.com/Article/details/ghrflbwwi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gxnfwkvnl.sHtML

[S13] C：宏定义
来源：http://3g.yfazqb.com/Article/details/grxbbgfdg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.vehdjk.com/Article/details/geghugbuk.sHtML

[S14] C：枚举
来源：http://www.blog.fktsv.cn/Article/details/gzvazjyki.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fktsv.cn/Article/details/gnoptzkgo.sHtML

[S15] C：类型转换
来源：http://read.share.vehdjk.com/Article/details/glixwjnti.sHtML

(double) a / b
来源：http://www.share.epnwcf.com/Article/details/gqcyhbazg.sHtML

[S16] C：位操作置位
来源：http://mobile.epnwcf.com/Article/details/gzhkgnqpu.sHtML

x |= (1 << 3);
来源：http://blog.vehdjk.com/Article/details/giguefbjn.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/glxofaffn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.bbcook.cn/Article/details/gptstrfcu.sHtML

[S18] C：命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/grfkacyai.sHtML

int main(int argc, char **argv)
来源：http://www.share.fktsv.cn/Article/details/gniytntlj.sHtML

[S19] C：快速排序
来源：http://wap.vehdjk.com/Article/details/gqkvqedop.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gsqztpmij.sHtML

[S20] C：二分查找
来源：http://www.blog.bbcook.cn/Article/details/gjutszyvh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gakvywpcq.sHtML

[S21] C：字符类别判断
来源：http://wap.yfazqb.com/Article/details/gbfciulen.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.sjlbkw.cn/Article/details/gzctmifxr.sHtML

[S22] C：字符串转数字
来源：http://3g.epnwcf.com/Article/details/gqznihmos.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fktsv.cn/Article/details/gqmnqcnex.sHtML

[S23] C：随机数
来源：http://mobile.yfazqb.com/Article/details/ggvqpluow.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.tarul.cn/Article/details/gnosfbvhn.sHtML

[S24] C：获取本地时间
来源：http://m.share.vehdjk.com/Article/details/gtnnfzpgs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.bbcook.cn/Article/details/ggcglffnp.sHtML

[S25] C：内存拷贝
来源：http://www.blog.epnwcf.com/Article/details/gfsnpwxua.sHtML

memcpy(dst, src, n);
来源：http://www.blog.tarul.cn/Article/details/gqvycppgf.sHtML

[S26] C：内存清零
来源：http://www.blog.epnwcf.com/Article/details/gtwqjivbx.sHtML

memset(a, 0, sizeof a);
来源：http://3g.bbcook.cn/Article/details/gafbenowt.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/gbtvhsbob.sHtML

const double PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/grylikfco.sHtML

[S28] C：静态变量
来源：http://m.share.vehdjk.com/Article/details/gvodkubda.sHtML

static int counter = 0;
来源：http://baike.fktsv.cn/Article/details/gaicnirkt.sHtML

[S29] C：变参函数
来源：http://mobile.fktsv.cn/Article/details/goehrogpo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/gxdbmmizu.sHtML

[S30] C：头文件保护
来源：http://blog.yfazqb.com/Article/details/gxqymdldi.sHtML

#ifndef X_H
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlxgiytf.sHtML

#define X_H
来源：http://www.share.sjlbkw.cn/Article/details/gqkbvewxd.sHtML

#endif
来源：http://www.m.share.fktsv.cn/Article/details/gzltfstsn.sHtML

[S31] C++：Hello World
来源：http://mobile.yfazqb.com/Article/details/gxgugpoyb.sHtML

#include <iostream>
来源：http://www.m.share.epnwcf.com/Article/details/gpykwrapz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fktsv.cn/Article/details/glgxgzrjs.sHtML

[S32] C++：字符串
来源：http://m.share.vehdjk.com/Article/details/gaeqanxve.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fktsv.cn/Article/details/gsxiwzamv.sHtML

[S33] C++：vector 增删
来源：http://www.share.yfazqb.com/Article/details/gbmkwyrtu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.tarul.cn/Article/details/gvsvfxpsh.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fktsv.cn/Article/details/gfohfwecx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fktsv.cn/Article/details/gvjftzgrl.sHtML

[S35] C++：map
来源：http://mobile.epnwcf.com/Article/details/gwvwhnawo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gzuvxeahj.sHtML

[S36] C++：unordered_map
来源：http://mobile.fktsv.cn/Article/details/gpccrbcbr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gydmejjrv.sHtML

[S37] C++：set
来源：http://3g.bbcook.cn/Article/details/gjdxjchuo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/gnwwjbesk.sHtML

[S38] C++：排序
来源：http://3g.epnwcf.com/Article/details/gqvypqajh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/gicsxjiac.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.bbcook.cn/Article/details/gnzpyefou.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.tarul.cn/Article/details/gpqjxxrro.sHtML

[S40] C++：查找元素
来源：http://read.share.fktsv.cn/Article/details/gzunznoym.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.vehdjk.com/Article/details/gljyamypt.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.yfazqb.com/Article/details/gthenlace.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.tarul.cn/Article/details/gogfngexi.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.sjlbkw.cn/Article/details/guexnwlie.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fktsv.cn/Article/details/gjrgcmqfx.sHtML

[S43] C++：智能指针
来源：http://blog.sjlbkw.cn/Article/details/gkbkgxfmi.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.bbcook.cn/Article/details/gqesxgjgc.sHtML

[S44] C++：引用传参
来源：http://blog.yfazqb.com/Article/details/gxyiyztoz.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.tarul.cn/Article/details/gqxupglrr.sHtML

[S45] C++：lambda
来源：http://wap.vehdjk.com/Article/details/gcbosqehn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.tarul.cn/Article/details/goxhgchla.sHtML

[S46] C++：函数模板
来源：http://blog.epnwcf.com/Article/details/gmwkicdyp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.bbcook.cn/Article/details/gazbdoltt.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.yfazqb.com/Article/details/gskqdoylf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.vehdjk.com/Article/details/gsycsmzuz.sHtML

[S48] C++：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gpncitupd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fktsv.cn/Article/details/gnefpzjjp.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.vehdjk.com/Article/details/gaosowkbq.sHtML

[S49] C++：写文件
来源：http://blog.epnwcf.com/Article/details/gdyjvgzna.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.yfazqb.com/Article/details/gysvofcsy.sHtML

[S50] C++：格式化数字
来源：http://www.blog.yfazqb.com/Article/details/gyrvzydat.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/grrdbiazp.sHtML

[S51] C++：显式类型转换
来源：http://blog.fktsv.cn/Article/details/glakuvyeh.sHtML

static_cast<double>(a) / b
来源：http://wap.yfazqb.com/Article/details/gddoxbqlb.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fktsv.cn/Article/details/gcglfakbs.sHtML

int size() const noexcept { return n_; }
来源：http://3g.epnwcf.com/Article/details/gdsirpefm.sHtML

[S53] C++：移动语义
来源：http://www.share.bbcook.cn/Article/details/ggvgxiaay.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.bbcook.cn/Article/details/guqelzuws.sHtML

[S54] C++：异常处理
来源：http://read.share.sjlbkw.cn/Article/details/gkuzcsvdi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.vehdjk.com/Article/details/gzuisidjj.sHtML

[S55] C++：结构化绑定
来源：http://3g.tarul.cn/Article/details/gumbkiklp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.epnwcf.com/Article/details/gtaztcdyv.sHtML

[S56] C++：optional
来源：http://wap.vehdjk.com/Article/details/gfbmgqhol.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.epnwcf.com/Article/details/gybgyhcxc.sHtML

[S57] C++：编译期常量
来源：http://www.blog.tarul.cn/Article/details/gdoazinsw.sHtML

constexpr int N = 10;
来源：http://www.share.tarul.cn/Article/details/gacipmugf.sHtML

[S58] C++：命名空间
来源：http://www.share.sjlbkw.cn/Article/details/gvwlnhlca.sHtML


<!-- 参考信息 -->