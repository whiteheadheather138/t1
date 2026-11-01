代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.epnwcf.com/Article/details/gruuredan.sHtML

[Q90] 生成序号列
来源：http://blog.bbcook.cn/Article/details/grfsdkqkw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fktsv.cn/Article/details/goisstixw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gisjfyxzi.sHtML

R. Bash 专题
来源：http://www.share.epnwcf.com/Article/details/gebogirmu.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gjynkojtr.sHtML

[R01] shebang 与严格模式
来源：http://3g.fktsv.cn/Article/details/gauzimtav.sHtML

#!/usr/bin/env bash
来源：http://www.blog.yfazqb.com/Article/details/gkeypzxgv.sHtML

set -euo pipefail
来源：http://3g.sjlbkw.cn/Article/details/gusskjqia.sHtML

[R02] 变量赋值与使用
来源：http://read.share.tarul.cn/Article/details/gixkuvyvr.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.vehdjk.com/Article/details/ghvgcxmvj.sHtML

[R03] 只读变量
来源：http://3g.vehdjk.com/Article/details/gasuugecg.sHtML

readonly PI=3.14
来源：http://3g.vehdjk.com/Article/details/gbfnibctd.sHtML

[R04] 位置参数
来源：http://3g.vehdjk.com/Article/details/grrlidmfv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.epnwcf.com/Article/details/gqqrksvqw.sHtML

[R05] 参数默认值
来源：http://baike.bbcook.cn/Article/details/gfruyspaz.sHtML

name="${1:-default}"
来源：http://blog.bbcook.cn/Article/details/gkwnuxumc.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fktsv.cn/Article/details/ggbafhbif.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/gtncqblxb.sHtML

[R07] if 判断文件
来源：http://www.share.bbcook.cn/Article/details/gunocdxzl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.tarul.cn/Article/details/gbshruigw.sHtML

[R08] 数值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gvycbcbja.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gbtvdsbqx.sHtML

[R09] 字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/glbmwdlod.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gqfhewysw.sHtML

[R10] 正则匹配
来源：http://www.share.sjlbkw.cn/Article/details/gszomsvyx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/grducoodd.sHtML

[R11] case 多分支
来源：http://read.share.sjlbkw.cn/Article/details/gcamccsqf.sHtML

case "$1" in
来源：http://3g.epnwcf.com/Article/details/gtmdszwzo.sHtML

start) echo "启动" ;;
来源：http://mobile.bbcook.cn/Article/details/ggxrsuuma.sHtML

stop)  echo "停止" ;;
来源：http://3g.sjlbkw.cn/Article/details/gcdxmcklw.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gxdrolohb.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/gqvbgpoeo.sHtML

[R12] for 遍历文件
来源：http://www.share.bbcook.cn/Article/details/gikyogoky.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.vehdjk.com/Article/details/gngqudbmf.sHtML

[R13] for 计数循环
来源：http://www.blog.sjlbkw.cn/Article/details/gjktdihhe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/gjsjdmkfd.sHtML

[R14] C 风格 for
来源：http://wap.epnwcf.com/Article/details/guecegvgj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/grduihibm.sHtML

[R15] while 逐行读文件
来源：http://m.share.tarul.cn/Article/details/gtkheonlh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.sjlbkw.cn/Article/details/ghipuurlx.sHtML

[R16] until 等待条件
来源：http://wap.epnwcf.com/Article/details/gjkktndqv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gzupgqlaq.sHtML

[R17] 数组定义与取值
来源：http://baike.bbcook.cn/Article/details/gchbzopqi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.bbcook.cn/Article/details/ghrghsqmg.sHtML

[R18] 遍历数组
来源：http://baike.bbcook.cn/Article/details/gpthgvtbf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.epnwcf.com/Article/details/ggcvhrcdy.sHtML

[R19] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gnstgtyjq.sHtML

echo "${#arr[@]}"
来源：http://mobile.tarul.cn/Article/details/gijxppgah.sHtML

[R20] 关联数组（字典）
来源：http://mobile.sjlbkw.cn/Article/details/guaqqgnqk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fktsv.cn/Article/details/ghpobnnod.sHtML

[R21] 字符串长度
来源：http://3g.fktsv.cn/Article/details/glptrskzm.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/ganvoawql.sHtML

[R22] 截取子串
来源：http://mobile.tarul.cn/Article/details/gabnpxijs.sHtML

echo "${s:0:5}"
来源：http://mobile.vehdjk.com/Article/details/gwkcvpsnk.sHtML

[R23] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gcztnagth.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.yfazqb.com/Article/details/gcmnzqwjg.sHtML

[R24] 大小写转换
来源：http://baike.tarul.cn/Article/details/gmuqfmjyo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.vehdjk.com/Article/details/gyykyeeds.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fktsv.cn/Article/details/gwqlwspdn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gzcrcbows.sHtML

[R26] 命令替换
来源：http://blog.bbcook.cn/Article/details/gwtnrgvma.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/ggvqxoold.sHtML

[R27] 算术展开
来源：http://www.blog.epnwcf.com/Article/details/gzrrlkgdn.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.tarul.cn/Article/details/gmfrabmcz.sHtML

[R28] 浮点运算
来源：http://mobile.fktsv.cn/Article/details/gwrzkybgf.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/gmijawwuo.sHtML

[R29] 定义函数
来源：http://www.share.epnwcf.com/Article/details/gjyepubup.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.epnwcf.com/Article/details/gzujbvuhh.sHtML

[R30] 函数返回状态码
来源：http://wap.fktsv.cn/Article/details/glvgdnxyb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.yfazqb.com/Article/details/gzuoozlcv.sHtML

[R31] 局部变量
来源：http://www.share.bbcook.cn/Article/details/gfuqrhskm.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.tarul.cn/Article/details/gpzbdmiqj.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/gnexrbyyt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gvcbxfnau.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.sjlbkw.cn/Article/details/glfuzpdsp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.vehdjk.com/Article/details/gkdwdcvuu.sHtML

[R34] 退出时清理
来源：http://www.share.fktsv.cn/Article/details/gjmgxcsoh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.vehdjk.com/Article/details/gnnltlulf.sHtML

[R35] 后台执行并等待
来源：http://www.share.yfazqb.com/Article/details/gdnihrelb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.bbcook.cn/Article/details/gvcvnxikz.sHtML

[R36] 并发执行多个任务
来源：http://baike.vehdjk.com/Article/details/gympycktj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fktsv.cn/Article/details/gmygpcvun.sHtML

[R37] 把输出赋给变量
来源：http://baike.epnwcf.com/Article/details/gquyitqop.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/gcxlfldaa.sHtML

[R38] 管道串联
来源：http://blog.vehdjk.com/Article/details/gbwtecjiv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.bbcook.cn/Article/details/gmmzptdbm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fktsv.cn/Article/details/gldgeedtp.sHtML

cmd > out.log 2>&1
来源：http://baike.vehdjk.com/Article/details/gqztcieqo.sHtML

[R40] 追加写日志
来源：http://www.share.vehdjk.com/Article/details/grmpvplvj.sHtML

echo "log" >> out.log
来源：http://wap.bbcook.cn/Article/details/gwrbqiomz.sHtML

[R41] 丢弃输出
来源：http://read.share.vehdjk.com/Article/details/gqzynlvif.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.bbcook.cn/Article/details/gobuyqunm.sHtML

[R42] 输入重定向
来源：http://read.share.fktsv.cn/Article/details/ghlepxclz.sHtML

wc -l < a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gqrbmslqb.sHtML

[R43] 按名字查找文件
来源：http://m.share.bbcook.cn/Article/details/gtaizeets.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.vehdjk.com/Article/details/gdcaetezi.sHtML

[R44] 按修改时间查找
来源：http://m.share.epnwcf.com/Article/details/ggwpruyqq.sHtML

find . -mtime -7 -type f
来源：http://3g.sjlbkw.cn/Article/details/ghllvaalp.sHtML

[R45] 批量删除
来源：http://wap.tarul.cn/Article/details/gxwttfuwu.sHtML

find . -name "*.tmp" -delete
来源：http://wap.yfazqb.com/Article/details/gjmhrwnae.sHtML

[R46] 递归替换文件内容
来源：http://blog.yfazqb.com/Article/details/gvvxsxbbl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.sjlbkw.cn/Article/details/gebymdkhe.sHtML

[R47] sed 单行替换
来源：http://www.share.fktsv.cn/Article/details/gjhfourwa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gnlslwwjl.sHtML

[R48] awk 取指定列
来源：http://mobile.fktsv.cn/Article/details/grqwjjkje.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.bbcook.cn/Article/details/gspvklwqi.sHtML

[R49] awk 带条件
来源：http://read.share.sjlbkw.cn/Article/details/gfqpegshd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.bbcook.cn/Article/details/ganforpfc.sHtML

[R50] awk 求和
来源：http://mobile.epnwcf.com/Article/details/ganhwfiyx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gybosczmj.sHtML

[R51] 排序去重取前几
来源：http://m.share.fktsv.cn/Article/details/gpcmghyhy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.bbcook.cn/Article/details/gseisjouj.sHtML

[R52] 统计行数
来源：http://www.m.share.tarul.cn/Article/details/gglghrycn.sHtML

wc -l a.txt
来源：http://www.share.vehdjk.com/Article/details/gwcmswqwn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.epnwcf.com/Article/details/gkilstwdk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.tarul.cn/Article/details/gmdqevgxd.sHtML

[R54] 比较两个文件
来源：http://www.blog.fktsv.cn/Article/details/gnlvgpxrg.sHtML

diff a.txt b.txt
来源：http://www.share.tarul.cn/Article/details/gyjhzxada.sHtML

[R55] 压缩与解压
来源：http://3g.bbcook.cn/Article/details/grjzxssku.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fktsv.cn/Article/details/gzsfkholf.sHtML

[R56] 远程拷贝
来源：http://m.share.fktsv.cn/Article/details/gidfsspwx.sHtML

scp file user@host:/path/
来源：http://www.share.bbcook.cn/Article/details/gysdprmgy.sHtML

[R57] 远程执行命令
来源：http://mobile.sjlbkw.cn/Article/details/gvmkkkmxm.sHtML

ssh user@host 'uptime'
来源：http://blog.fktsv.cn/Article/details/gmfzfdsfz.sHtML

[R58] 下载文件
来源：http://3g.yfazqb.com/Article/details/gjzrecadc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/ghbinmmxi.sHtML

[R59] 发 POST JSON
来源：http://m.share.fktsv.cn/Article/details/gzlqwvdje.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.vehdjk.com/Article/details/gtokuuhcm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gnupaythf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.tarul.cn/Article/details/gdiefsdkm.sHtML

[R61] 磁盘占用
来源：http://blog.sjlbkw.cn/Article/details/ghvefpxvv.sHtML

df -h;  du -sh *
来源：http://m.share.bbcook.cn/Article/details/gxynxsxdb.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.yfazqb.com/Article/details/gucwymxpl.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.vehdjk.com/Article/details/gcucfqhqm.sHtML

[R63] 内存与进程
来源：http://www.share.yfazqb.com/Article/details/gltkczvuq.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.bbcook.cn/Article/details/gziwvlemv.sHtML

[R64] 结束进程
来源：http://blog.sjlbkw.cn/Article/details/gfgvejvqj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fktsv.cn/Article/details/gelljcfmr.sHtML

[R65] 查看端口占用
来源：http://m.share.epnwcf.com/Article/details/gakswfcvk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.sjlbkw.cn/Article/details/gggmuouex.sHtML

[R66] 定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gebupjinv.sHtML

crontab -e;  crontab -l
来源：http://www.share.bbcook.cn/Article/details/gwedwuzsj.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fktsv.cn/Article/details/grgvaicze.sHtML

openssl rand -hex 16
来源：http://mobile.yfazqb.com/Article/details/gvnpswfst.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.bbcook.cn/Article/details/gwbdqhuej.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.yfazqb.com/Article/details/gbelkbjwo.sHtML

[R69] 生成随机密码
来源：http://wap.sjlbkw.cn/Article/details/glzkoakrb.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.tarul.cn/Article/details/glpblkfgr.sHtML

[R70] 时间戳与互转
来源：http://wap.epnwcf.com/Article/details/gpfgztkgo.sHtML

date +%s;  date -d @1700000000
来源：http://wap.tarul.cn/Article/details/gnbbbyddw.sHtML

[R71] 日期格式化
来源：http://3g.tarul.cn/Article/details/gexpujzwz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fktsv.cn/Article/details/goizotchy.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.epnwcf.com/Article/details/gjfoyuqya.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.sjlbkw.cn/Article/details/gfysxgomj.sHtML

[R73] 分割大日志
来源：http://read.share.bbcook.cn/Article/details/ggrirlaha.sHtML

split -l 1000 big.log part_
来源：http://read.share.fktsv.cn/Article/details/geevydmji.sHtML

[R74] 批量重命名
来源：http://wap.tarul.cn/Article/details/gwtkdemez.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fktsv.cn/Article/details/gvrvrzazp.sHtML

[R75] 导出环境变量
来源：http://3g.epnwcf.com/Article/details/gknbxelln.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.bbcook.cn/Article/details/gkkomqihs.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/gknnmsayn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gxworpjrt.sHtML

[R77] 读取用户输入
来源：http://mobile.fktsv.cn/Article/details/grlevpapk.sHtML

read -rp "请输入: " ans
来源：http://www.share.tarul.cn/Article/details/gjuxxpjst.sHtML

[R78] 交互式菜单
来源：http://wap.sjlbkw.cn/Article/details/gadpcownj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.yfazqb.com/Article/details/gshiykdgw.sHtML

[R79] 解析命令行选项
来源：http://m.share.yfazqb.com/Article/details/gdlyfovlx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/gtompsvcd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.epnwcf.com/Article/details/gbergzbuc.sHtML

time ./run.sh
来源：http://www.blog.fktsv.cn/Article/details/gndeocyql.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gjflmtddh.sHtML

S. C / C++ 专题
来源：http://blog.epnwcf.com/Article/details/gscvjupea.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ggwkoceoi.sHtML

[S01] C：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gqdoxsfht.sHtML

#include <stdio.h>
来源：http://baike.bbcook.cn/Article/details/gxwnbijwm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.vehdjk.com/Article/details/gplovrhpo.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.epnwcf.com/Article/details/gifshzmhk.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.epnwcf.com/Article/details/ghzhjhblo.sHtML

[S03] C：读入整数
来源：http://wap.fktsv.cn/Article/details/gibwdpqip.sHtML

int x; scanf("%d", &x);
来源：http://www.share.vehdjk.com/Article/details/gdqpjsyan.sHtML

[S04] C：字符串复制
来源：http://blog.epnwcf.com/Article/details/glracqbir.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.vehdjk.com/Article/details/gsbwnjxvk.sHtML

[S05] C：字符串长度
来源：http://wap.tarul.cn/Article/details/gctsqfyns.sHtML

strlen(s)
来源：http://blog.bbcook.cn/Article/details/gatsxadxp.sHtML

[S06] C：字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gimuyopqe.sHtML

strcmp(a, b) == 0
来源：http://www.share.bbcook.cn/Article/details/gsspoerar.sHtML

[S07] C：数组遍历求和
来源：http://baike.sjlbkw.cn/Article/details/gwprzuyam.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.tarul.cn/Article/details/geqsdvhnc.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.tarul.cn/Article/details/gxrgeprov.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.epnwcf.com/Article/details/glwwpaanz.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.tarul.cn/Article/details/gjehiyvrz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.tarul.cn/Article/details/givuadrjg.sHtML

[S10] C：指针与解引用
来源：http://3g.vehdjk.com/Article/details/guffltyhy.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.vehdjk.com/Article/details/gwwertgcn.sHtML

[S11] C：逐行读文件
来源：http://blog.tarul.cn/Article/details/giqwcihvr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.sjlbkw.cn/Article/details/ghirbjhow.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.tarul.cn/Article/details/gphosyltc.sHtML

fclose(f);
来源：http://mobile.bbcook.cn/Article/details/ggtdzpdaw.sHtML

[S12] C：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gixnvjimn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.yfazqb.com/Article/details/gsdwocffo.sHtML

[S13] C：宏定义
来源：http://3g.yfazqb.com/Article/details/ggkkwnzgt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.sjlbkw.cn/Article/details/gtcpujaeb.sHtML

[S14] C：枚举
来源：http://baike.yfazqb.com/Article/details/gzlrsuhjt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.sjlbkw.cn/Article/details/gcicwqifx.sHtML

[S15] C：类型转换
来源：http://read.share.epnwcf.com/Article/details/gyffuezst.sHtML

(double) a / b
来源：http://read.share.sjlbkw.cn/Article/details/geiswfpoq.sHtML

[S16] C：位操作置位
来源：http://m.share.bbcook.cn/Article/details/gqaaodhrm.sHtML

x |= (1 << 3);
来源：http://www.share.bbcook.cn/Article/details/gqcppqpyp.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.tarul.cn/Article/details/gmfjpehdn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.epnwcf.com/Article/details/gcnktaglg.sHtML

[S18] C：命令行参数
来源：http://baike.sjlbkw.cn/Article/details/gaicnkyat.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.epnwcf.com/Article/details/gxifywqzq.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/guayavjqf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gewvxhcqx.sHtML

[S20] C：二分查找
来源：http://baike.sjlbkw.cn/Article/details/gptomoqih.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gfxayobce.sHtML

[S21] C：字符类别判断
来源：http://www.blog.vehdjk.com/Article/details/gtktjawhz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.sjlbkw.cn/Article/details/gmbanhtqn.sHtML

[S22] C：字符串转数字
来源：http://blog.tarul.cn/Article/details/gfitfnrcr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/geurxwbrk.sHtML

[S23] C：随机数
来源：http://m.share.sjlbkw.cn/Article/details/gjjldggfz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.bbcook.cn/Article/details/glupmxihs.sHtML

[S24] C：获取本地时间
来源：http://www.share.fktsv.cn/Article/details/gquvzohiw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.bbcook.cn/Article/details/gzwludlhz.sHtML

[S25] C：内存拷贝
来源：http://3g.tarul.cn/Article/details/gupkoajnz.sHtML

memcpy(dst, src, n);
来源：http://3g.sjlbkw.cn/Article/details/gyowtgjtk.sHtML

[S26] C：内存清零
来源：http://www.m.share.sjlbkw.cn/Article/details/gblewouhe.sHtML

memset(a, 0, sizeof a);
来源：http://wap.tarul.cn/Article/details/gcicixcga.sHtML

[S27] C：定义常量
来源：http://baike.epnwcf.com/Article/details/gnskbgmue.sHtML

const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gpikgjrnd.sHtML

[S28] C：静态变量
来源：http://3g.bbcook.cn/Article/details/gbxgaldfl.sHtML

static int counter = 0;
来源：http://www.m.share.tarul.cn/Article/details/gibtdjgok.sHtML

[S29] C：变参函数
来源：http://www.blog.epnwcf.com/Article/details/gfcdxziac.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fktsv.cn/Article/details/gbhcbgiol.sHtML

[S30] C：头文件保护
来源：http://wap.bbcook.cn/Article/details/gzlncloak.sHtML

#ifndef X_H
来源：http://wap.fktsv.cn/Article/details/gfhttwnde.sHtML

#define X_H
来源：http://3g.yfazqb.com/Article/details/glbezojlo.sHtML

#endif
来源：http://www.m.share.bbcook.cn/Article/details/gjloodtkf.sHtML

[S31] C++：Hello World
来源：http://3g.epnwcf.com/Article/details/gqplekhns.sHtML

#include <iostream>
来源：http://m.share.tarul.cn/Article/details/gqevgngcy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.vehdjk.com/Article/details/gbhiocpjw.sHtML

[S32] C++：字符串
来源：http://wap.fktsv.cn/Article/details/girhjwahu.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.tarul.cn/Article/details/goxvmztdx.sHtML

[S33] C++：vector 增删
来源：http://blog.fktsv.cn/Article/details/gzpebldsf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.bbcook.cn/Article/details/gwrhyosmv.sHtML

[S34] C++：遍历 vector
来源：http://m.share.epnwcf.com/Article/details/gnjcagtol.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.yfazqb.com/Article/details/gtbndmend.sHtML

[S35] C++：map
来源：http://www.share.epnwcf.com/Article/details/gsumzzlsl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gtzbvkntb.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.tarul.cn/Article/details/gyqbwbzji.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/gzxamfyqr.sHtML

[S37] C++：set
来源：http://m.share.tarul.cn/Article/details/gbkbmfmsf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.yfazqb.com/Article/details/gbsqyxzuq.sHtML

[S38] C++：排序
来源：http://m.share.bbcook.cn/Article/details/gomuapres.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.tarul.cn/Article/details/geqrneuxy.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/gcrtuzqew.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/gottmeloc.sHtML

[S40] C++：查找元素
来源：http://baike.fktsv.cn/Article/details/gxteghapl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.vehdjk.com/Article/details/gkcrokokn.sHtML

[S41] C++：类与构造函数
来源：http://wap.vehdjk.com/Article/details/gvvbwquji.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.tarul.cn/Article/details/gallefixe.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fktsv.cn/Article/details/geoudsidq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.sjlbkw.cn/Article/details/gikrocfpq.sHtML

[S43] C++：智能指针
来源：http://www.blog.tarul.cn/Article/details/gsmpsufko.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.bbcook.cn/Article/details/gkoxjpqaa.sHtML

[S44] C++：引用传参
来源：http://m.share.sjlbkw.cn/Article/details/gesqtuurq.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.yfazqb.com/Article/details/gjkxaezfo.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gaqwnlcgr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.sjlbkw.cn/Article/details/gupykqtyy.sHtML

[S46] C++：函数模板
来源：http://3g.tarul.cn/Article/details/gizdlxjpr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.yfazqb.com/Article/details/gevuitdun.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.epnwcf.com/Article/details/gxoxjbnzb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.epnwcf.com/Article/details/gfxykyygk.sHtML

[S48] C++：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gnublgkri.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.epnwcf.com/Article/details/gbszuydsz.sHtML

while (std::getline(in, line)) { }
来源：http://wap.sjlbkw.cn/Article/details/ggsuvhnvc.sHtML

[S49] C++：写文件
来源：http://3g.sjlbkw.cn/Article/details/gaziusetv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.sjlbkw.cn/Article/details/gucfvkywp.sHtML

[S50] C++：格式化数字
来源：http://3g.bbcook.cn/Article/details/gvzsndale.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.vehdjk.com/Article/details/grojewqft.sHtML

[S51] C++：显式类型转换
来源：http://blog.fktsv.cn/Article/details/gkvbxftcb.sHtML

static_cast<double>(a) / b
来源：http://blog.tarul.cn/Article/details/gvhytgdlo.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.sjlbkw.cn/Article/details/ghkafyqjn.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fktsv.cn/Article/details/gaswanrff.sHtML

[S53] C++：移动语义
来源：http://3g.epnwcf.com/Article/details/gmbstnapy.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.sjlbkw.cn/Article/details/gxaxykjnp.sHtML

[S54] C++：异常处理
来源：http://read.share.tarul.cn/Article/details/ggrdndipk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.epnwcf.com/Article/details/gmidhuzbi.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.yfazqb.com/Article/details/glljxvlyq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/gdclsulnh.sHtML

[S56] C++：optional
来源：http://www.share.fktsv.cn/Article/details/gcearukrn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fktsv.cn/Article/details/gcqseijvr.sHtML

[S57] C++：编译期常量
来源：http://blog.epnwcf.com/Article/details/gvrjcrrzm.sHtML

constexpr int N = 10;
来源：http://m.share.bbcook.cn/Article/details/ggwvibudz.sHtML

[S58] C++：命名空间
来源：http://www.share.vehdjk.com/Article/details/gwubtalfx.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.yfazqb.com/Article/details/gteohzmyc.sHtML

[S59] C++：静态断言
来源：http://wap.tarul.cn/Article/details/gcvzjuqrp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.sjlbkw.cn/Article/details/gtnlmdjhn.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.sjlbkw.cn/Article/details/ghajygdsa.sHtML


<!-- 参考信息 -->