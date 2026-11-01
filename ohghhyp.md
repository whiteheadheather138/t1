代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.epnwcf.com/Article/details/gzjhjtyme.sHtML

[Q90] 生成序号列
来源：http://wap.epnwcf.com/Article/details/gwygajipi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fktsv.cn/Article/details/gynxpaeiz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gntpwyvsu.sHtML

R. Bash 专题
来源：http://www.m.share.tarul.cn/Article/details/gvgcgxotv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gcfgfbkdv.sHtML

[R01] shebang 与严格模式
来源：http://baike.sjlbkw.cn/Article/details/gvcowhhxq.sHtML

#!/usr/bin/env bash
来源：http://blog.fktsv.cn/Article/details/gmyyvfybp.sHtML

set -euo pipefail
来源：http://www.m.share.bbcook.cn/Article/details/gzffaykgd.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.tarul.cn/Article/details/gibqerguc.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.sjlbkw.cn/Article/details/gmtalyqsa.sHtML

[R03] 只读变量
来源：http://www.m.share.yfazqb.com/Article/details/giwuvxrko.sHtML

readonly PI=3.14
来源：http://baike.vehdjk.com/Article/details/gdbvacxhb.sHtML

[R04] 位置参数
来源：http://blog.tarul.cn/Article/details/ghghaoied.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.epnwcf.com/Article/details/gaqgerfsp.sHtML

[R05] 参数默认值
来源：http://wap.bbcook.cn/Article/details/grfjaaczh.sHtML

name="${1:-default}"
来源：http://mobile.vehdjk.com/Article/details/gyezmetlk.sHtML

[R06] 判断命令是否存在
来源：http://blog.bbcook.cn/Article/details/grryerqlk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gkyjapwqa.sHtML

[R07] if 判断文件
来源：http://m.share.epnwcf.com/Article/details/glnurckuf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gszpyozzb.sHtML

[R08] 数值比较
来源：http://mobile.sjlbkw.cn/Article/details/gkqqcljjy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gtbpezubn.sHtML

[R09] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gwslgedlc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.bbcook.cn/Article/details/grpqkbpwq.sHtML

[R10] 正则匹配
来源：http://www.blog.vehdjk.com/Article/details/guobaolkx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gbdxhufms.sHtML

[R11] case 多分支
来源：http://www.share.vehdjk.com/Article/details/ghehuremd.sHtML

case "$1" in
来源：http://blog.bbcook.cn/Article/details/gugarjxke.sHtML

start) echo "启动" ;;
来源：http://baike.bbcook.cn/Article/details/gftvuosgv.sHtML

stop)  echo "停止" ;;
来源：http://wap.yfazqb.com/Article/details/ghunwpmkr.sHtML

*)     echo "未知命令" ;;
来源：http://wap.sjlbkw.cn/Article/details/gnkylrcms.sHtML

esac
来源：http://m.share.fktsv.cn/Article/details/gcomyfbme.sHtML

[R12] for 遍历文件
来源：http://blog.vehdjk.com/Article/details/gisdswqqv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fktsv.cn/Article/details/gucwngmis.sHtML

[R13] for 计数循环
来源：http://www.share.epnwcf.com/Article/details/giywfaeta.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/goybxdzcn.sHtML

[R14] C 风格 for
来源：http://blog.tarul.cn/Article/details/gfvpfoqxy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/gyrcrnbmh.sHtML

[R15] while 逐行读文件
来源：http://baike.vehdjk.com/Article/details/gjspncihn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.sjlbkw.cn/Article/details/gakxnhznw.sHtML

[R16] until 等待条件
来源：http://baike.sjlbkw.cn/Article/details/gawbhdddx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.yfazqb.com/Article/details/gxooeambm.sHtML

[R17] 数组定义与取值
来源：http://www.share.yfazqb.com/Article/details/gqxjbumui.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fktsv.cn/Article/details/gyrdozgyi.sHtML

[R18] 遍历数组
来源：http://baike.tarul.cn/Article/details/gjkjssyev.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.epnwcf.com/Article/details/gbzbxtlck.sHtML

[R19] 数组长度
来源：http://mobile.yfazqb.com/Article/details/gtbdrmxre.sHtML

echo "${#arr[@]}"
来源：http://mobile.tarul.cn/Article/details/gdotbvabr.sHtML

[R20] 关联数组（字典）
来源：http://m.share.yfazqb.com/Article/details/gknebbhtz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/giaxzdmuu.sHtML

[R21] 字符串长度
来源：http://blog.fktsv.cn/Article/details/gmvlcicrl.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gmhbxbioz.sHtML

[R22] 截取子串
来源：http://baike.epnwcf.com/Article/details/gvvccsrvj.sHtML

echo "${s:0:5}"
来源：http://baike.tarul.cn/Article/details/gvvfizgxv.sHtML

[R23] 字符串替换
来源：http://www.m.share.vehdjk.com/Article/details/gybfomeiv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.sjlbkw.cn/Article/details/gogduwdrb.sHtML

[R24] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gyyeplsot.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.bbcook.cn/Article/details/giszegahc.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.yfazqb.com/Article/details/gcrobzexk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.epnwcf.com/Article/details/gozfuwlce.sHtML

[R26] 命令替换
来源：http://3g.bbcook.cn/Article/details/gedflqqqr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.vehdjk.com/Article/details/gfkbnnjab.sHtML

[R27] 算术展开
来源：http://www.m.share.vehdjk.com/Article/details/gccwmsurq.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.tarul.cn/Article/details/gavehotig.sHtML

[R28] 浮点运算
来源：http://read.share.vehdjk.com/Article/details/ghhkiolla.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.tarul.cn/Article/details/ggjwibwzr.sHtML

[R29] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/gzizuyfku.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.yfazqb.com/Article/details/gdbmsjrxo.sHtML

[R30] 函数返回状态码
来源：http://m.share.vehdjk.com/Article/details/guvzcnvid.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.vehdjk.com/Article/details/gmqwnfsah.sHtML

[R31] 局部变量
来源：http://wap.fktsv.cn/Article/details/gsznteamz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/giydjjabz.sHtML

[R32] 参数个数校验
来源：http://wap.yfazqb.com/Article/details/ghspxezrt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gdtozcrmj.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fktsv.cn/Article/details/gldbhbocb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fktsv.cn/Article/details/gbkdnpcdc.sHtML

[R34] 退出时清理
来源：http://m.share.vehdjk.com/Article/details/gnuxeexyw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/gozuevmuz.sHtML

[R35] 后台执行并等待
来源：http://www.blog.yfazqb.com/Article/details/gqimkcebq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.tarul.cn/Article/details/gadcsxxjv.sHtML

[R36] 并发执行多个任务
来源：http://baike.bbcook.cn/Article/details/gecxktdfo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.sjlbkw.cn/Article/details/gbauqqwkw.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.tarul.cn/Article/details/gscnowzma.sHtML

files=$(ls -1)
来源：http://blog.vehdjk.com/Article/details/gjrajxsvi.sHtML

[R38] 管道串联
来源：http://www.m.share.tarul.cn/Article/details/gbipgottp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fktsv.cn/Article/details/gbebsfbec.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.sjlbkw.cn/Article/details/gtbntkuhh.sHtML

cmd > out.log 2>&1
来源：http://m.share.fktsv.cn/Article/details/gnqvzbcxr.sHtML

[R40] 追加写日志
来源：http://www.blog.bbcook.cn/Article/details/glolkykyj.sHtML

echo "log" >> out.log
来源：http://www.m.share.fktsv.cn/Article/details/ghldgnmuz.sHtML

[R41] 丢弃输出
来源：http://mobile.tarul.cn/Article/details/gzimjmole.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gukpufcgw.sHtML

[R42] 输入重定向
来源：http://blog.tarul.cn/Article/details/gdkaldctb.sHtML

wc -l < a.txt
来源：http://m.share.tarul.cn/Article/details/gnkhibtvi.sHtML

[R43] 按名字查找文件
来源：http://blog.epnwcf.com/Article/details/gffpytxnt.sHtML

find . -name "*.log" -type f
来源：http://www.share.fktsv.cn/Article/details/gbaeqomhj.sHtML

[R44] 按修改时间查找
来源：http://wap.tarul.cn/Article/details/gztulqkpi.sHtML

find . -mtime -7 -type f
来源：http://3g.sjlbkw.cn/Article/details/gsahmcaow.sHtML

[R45] 批量删除
来源：http://read.share.epnwcf.com/Article/details/ghudgxtda.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/gfkjlkzvs.sHtML

[R46] 递归替换文件内容
来源：http://read.share.sjlbkw.cn/Article/details/gzcpvytuz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.tarul.cn/Article/details/gmbpdebmn.sHtML

[R47] sed 单行替换
来源：http://wap.yfazqb.com/Article/details/gkyiygycy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.yfazqb.com/Article/details/glpilfgne.sHtML

[R48] awk 取指定列
来源：http://www.blog.yfazqb.com/Article/details/gpqgumheo.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.tarul.cn/Article/details/gcvozsmri.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/gtlajejpo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.yfazqb.com/Article/details/gcxtjjadi.sHtML

[R50] awk 求和
来源：http://3g.sjlbkw.cn/Article/details/gsxccfgrh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gsrleiljx.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.yfazqb.com/Article/details/gtwaikkaj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.bbcook.cn/Article/details/gfnuvsmrj.sHtML

[R52] 统计行数
来源：http://m.share.epnwcf.com/Article/details/gebsvdbev.sHtML

wc -l a.txt
来源：http://baike.tarul.cn/Article/details/gdgcboxko.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.epnwcf.com/Article/details/gogbwhkvl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.tarul.cn/Article/details/gojgujeyk.sHtML

[R54] 比较两个文件
来源：http://wap.vehdjk.com/Article/details/gibpclwes.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/gvxppxteo.sHtML

[R55] 压缩与解压
来源：http://www.share.tarul.cn/Article/details/gzeptjakb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.sjlbkw.cn/Article/details/gyxmojoie.sHtML

[R56] 远程拷贝
来源：http://read.share.vehdjk.com/Article/details/gxinipofn.sHtML

scp file user@host:/path/
来源：http://www.share.sjlbkw.cn/Article/details/gmuhiwgor.sHtML

[R57] 远程执行命令
来源：http://m.share.yfazqb.com/Article/details/gnoiiulum.sHtML

ssh user@host 'uptime'
来源：http://mobile.tarul.cn/Article/details/gsuejfqbj.sHtML

[R58] 下载文件
来源：http://read.share.yfazqb.com/Article/details/gkpfwlhss.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.tarul.cn/Article/details/gruyxdvcn.sHtML

[R59] 发 POST JSON
来源：http://www.blog.epnwcf.com/Article/details/gouwnpnym.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.vehdjk.com/Article/details/guoibqmdi.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/gsgstdsuw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.tarul.cn/Article/details/ghlzzxwwl.sHtML

[R61] 磁盘占用
来源：http://blog.sjlbkw.cn/Article/details/gnunmobyg.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/gqdfuchoj.sHtML

[R62] 找最占空间的文件
来源：http://mobile.tarul.cn/Article/details/gsbztrfwo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.tarul.cn/Article/details/guivhouxc.sHtML

[R63] 内存与进程
来源：http://blog.bbcook.cn/Article/details/gshwxtzpr.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.vehdjk.com/Article/details/gzqflcjgn.sHtML

[R64] 结束进程
来源：http://m.share.bbcook.cn/Article/details/grntonrlc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fktsv.cn/Article/details/grkubnswf.sHtML

[R65] 查看端口占用
来源：http://www.share.yfazqb.com/Article/details/gczhawsrt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/gcabwkfhz.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gtszsdgbu.sHtML

crontab -e;  crontab -l
来源：http://mobile.fktsv.cn/Article/details/gbwztmzba.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.tarul.cn/Article/details/gyddwmrzr.sHtML

openssl rand -hex 16
来源：http://www.m.share.vehdjk.com/Article/details/gtktkmpya.sHtML

[R68] 计算文件校验值
来源：http://3g.vehdjk.com/Article/details/gmmirfhtg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.bbcook.cn/Article/details/gfvupwwqj.sHtML

[R69] 生成随机密码
来源：http://read.share.fktsv.cn/Article/details/gybxclano.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.yfazqb.com/Article/details/gjlvxcvjv.sHtML

[R70] 时间戳与互转
来源：http://baike.sjlbkw.cn/Article/details/gktbldpgw.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fktsv.cn/Article/details/gnixgeimj.sHtML

[R71] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gvrxsysrk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fktsv.cn/Article/details/gtfrdzgbp.sHtML

[R72] 等待端口就绪
来源：http://baike.vehdjk.com/Article/details/gejiqnuik.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnpuekce.sHtML

[R73] 分割大日志
来源：http://baike.yfazqb.com/Article/details/gftlqcphs.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnoliuzl.sHtML

[R74] 批量重命名
来源：http://www.share.yfazqb.com/Article/details/glcgygcov.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.sjlbkw.cn/Article/details/goegxarkk.sHtML

[R75] 导出环境变量
来源：http://www.blog.epnwcf.com/Article/details/gapbdhabe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fktsv.cn/Article/details/gckgdoekk.sHtML

[R76] 使用临时文件
来源：http://wap.tarul.cn/Article/details/gljhrezrf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gxvxjgngy.sHtML

[R77] 读取用户输入
来源：http://www.blog.fktsv.cn/Article/details/gwlshinfl.sHtML

read -rp "请输入: " ans
来源：http://wap.sjlbkw.cn/Article/details/gjmzlpvnx.sHtML

[R78] 交互式菜单
来源：http://3g.sjlbkw.cn/Article/details/girrbfjha.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.tarul.cn/Article/details/ghjalthcp.sHtML

[R79] 解析命令行选项
来源：http://wap.tarul.cn/Article/details/gpnlfjurp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.yfazqb.com/Article/details/gtcccxtas.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.sjlbkw.cn/Article/details/gfpcgzxfc.sHtML

time ./run.sh
来源：http://wap.yfazqb.com/Article/details/gawiqbizm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gofanunyh.sHtML

S. C / C++ 专题
来源：http://mobile.vehdjk.com/Article/details/gbrtqwhen.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gkorgfqhv.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gtehvwpef.sHtML

#include <stdio.h>
来源：http://mobile.vehdjk.com/Article/details/gmjzdaigb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.vehdjk.com/Article/details/ghkolxamj.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.tarul.cn/Article/details/glslcxqnn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.epnwcf.com/Article/details/gycsqpqlp.sHtML

[S03] C：读入整数
来源：http://baike.tarul.cn/Article/details/gfdaveqft.sHtML

int x; scanf("%d", &x);
来源：http://www.share.tarul.cn/Article/details/gzyxydvco.sHtML

[S04] C：字符串复制
来源：http://3g.fktsv.cn/Article/details/ginfgflgb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.vehdjk.com/Article/details/grhtjbzse.sHtML

[S05] C：字符串长度
来源：http://wap.tarul.cn/Article/details/gavgsnudg.sHtML

strlen(s)
来源：http://baike.tarul.cn/Article/details/gxftfgypg.sHtML

[S06] C：字符串比较
来源：http://baike.fktsv.cn/Article/details/gaakufvtw.sHtML

strcmp(a, b) == 0
来源：http://blog.tarul.cn/Article/details/ghzkwaedq.sHtML

[S07] C：数组遍历求和
来源：http://mobile.epnwcf.com/Article/details/griuugfyp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.bbcook.cn/Article/details/ghuyfutqo.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.tarul.cn/Article/details/gqzhbyxsy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.yfazqb.com/Article/details/gbwqijvlh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fktsv.cn/Article/details/gizxmycwa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fktsv.cn/Article/details/gyowzhlwv.sHtML

[S10] C：指针与解引用
来源：http://read.share.yfazqb.com/Article/details/gnrupvupj.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.tarul.cn/Article/details/gobdsrehy.sHtML

[S11] C：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gggkytrgo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.vehdjk.com/Article/details/gbvmkpdkj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.vehdjk.com/Article/details/glyhmxvkb.sHtML

fclose(f);
来源：http://3g.bbcook.cn/Article/details/gdgzicojz.sHtML

[S12] C：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gsqcakhaz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gaarkuddu.sHtML

[S13] C：宏定义
来源：http://wap.tarul.cn/Article/details/grwjrltai.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fktsv.cn/Article/details/geezoouuc.sHtML

[S14] C：枚举
来源：http://www.blog.yfazqb.com/Article/details/gmutkrxrc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fktsv.cn/Article/details/gaqtvgimk.sHtML

[S15] C：类型转换
来源：http://wap.epnwcf.com/Article/details/gzaxchjqm.sHtML

(double) a / b
来源：http://wap.fktsv.cn/Article/details/gnzpbmypq.sHtML

[S16] C：位操作置位
来源：http://www.share.vehdjk.com/Article/details/geufbsgeg.sHtML

x |= (1 << 3);
来源：http://www.blog.vehdjk.com/Article/details/gwqoudifw.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gumwdfanm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.epnwcf.com/Article/details/gcwnbqcig.sHtML

[S18] C：命令行参数
来源：http://m.share.fktsv.cn/Article/details/gpypbinxu.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/gdajnayke.sHtML

[S19] C：快速排序
来源：http://www.share.sjlbkw.cn/Article/details/gjhhykblo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkczuevcr.sHtML

[S20] C：二分查找
来源：http://www.blog.epnwcf.com/Article/details/grmvrohac.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gxznvorjl.sHtML

[S21] C：字符类别判断
来源：http://baike.yfazqb.com/Article/details/gkfpsdmmc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fktsv.cn/Article/details/gaoccksdz.sHtML

[S22] C：字符串转数字
来源：http://read.share.fktsv.cn/Article/details/gljcegvau.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/gofmeczgb.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gpizlzghc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.sjlbkw.cn/Article/details/grjuarxbz.sHtML

[S24] C：获取本地时间
来源：http://baike.fktsv.cn/Article/details/gcsmnckuf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.epnwcf.com/Article/details/gywxujwcp.sHtML

[S25] C：内存拷贝
来源：http://mobile.bbcook.cn/Article/details/godgeccyw.sHtML

memcpy(dst, src, n);
来源：http://www.share.fktsv.cn/Article/details/gdogswmtg.sHtML

[S26] C：内存清零
来源：http://read.share.tarul.cn/Article/details/gyvzgnxoi.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.bbcook.cn/Article/details/gzszskjdw.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/gpjhleyzo.sHtML

const double PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/guydsafyb.sHtML

[S28] C：静态变量
来源：http://read.share.fktsv.cn/Article/details/gjynhebtd.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/gmmfbqbff.sHtML

[S29] C：变参函数
来源：http://blog.bbcook.cn/Article/details/gpyoxrpmf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.sjlbkw.cn/Article/details/gzwtuxhqt.sHtML

[S30] C：头文件保护
来源：http://wap.sjlbkw.cn/Article/details/ggyjyzvmk.sHtML

#ifndef X_H
来源：http://mobile.vehdjk.com/Article/details/ghcmjlpnc.sHtML

#define X_H
来源：http://www.m.share.fktsv.cn/Article/details/gxyrrmfdl.sHtML

#endif
来源：http://m.share.vehdjk.com/Article/details/gvpbylbax.sHtML

[S31] C++：Hello World
来源：http://www.share.tarul.cn/Article/details/gtpshgung.sHtML

#include <iostream>
来源：http://blog.vehdjk.com/Article/details/guhmoqoid.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.sjlbkw.cn/Article/details/gfrkbbxme.sHtML

[S32] C++：字符串
来源：http://www.blog.epnwcf.com/Article/details/gnhpsmcyw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.yfazqb.com/Article/details/gcunqcsss.sHtML

[S33] C++：vector 增删
来源：http://3g.fktsv.cn/Article/details/gcbhyxdpy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fktsv.cn/Article/details/gxibdxxlm.sHtML

[S34] C++：遍历 vector
来源：http://mobile.sjlbkw.cn/Article/details/ghsfditbr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.yfazqb.com/Article/details/gskvmeyvr.sHtML

[S35] C++：map
来源：http://read.share.tarul.cn/Article/details/guyqgevrj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gpajodtjr.sHtML

[S36] C++：unordered_map
来源：http://wap.yfazqb.com/Article/details/gqpjrkgwg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/ggxehdvoc.sHtML

[S37] C++：set
来源：http://3g.sjlbkw.cn/Article/details/gejhclkyl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.tarul.cn/Article/details/gaimbzkxq.sHtML

[S38] C++：排序
来源：http://3g.fktsv.cn/Article/details/gfinynenj.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fktsv.cn/Article/details/geahbuxfn.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.epnwcf.com/Article/details/gwksbchqz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fktsv.cn/Article/details/gfsmbgkoh.sHtML

[S40] C++：查找元素
来源：http://www.share.yfazqb.com/Article/details/ghnpjjhzb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.vehdjk.com/Article/details/gkrqrewmp.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/gugivcdju.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.vehdjk.com/Article/details/gxrgxzvxs.sHtML

[S42] C++：继承与虚函数
来源：http://wap.vehdjk.com/Article/details/gdqhfmkxk.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.sjlbkw.cn/Article/details/gjfkidjkj.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/gpgvpedhp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.bbcook.cn/Article/details/gzpfurrpe.sHtML

[S44] C++：引用传参
来源：http://wap.yfazqb.com/Article/details/gspotijip.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.tarul.cn/Article/details/glbgyartr.sHtML

[S45] C++：lambda
来源：http://m.share.bbcook.cn/Article/details/gqcelfiaf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fktsv.cn/Article/details/ghkkvpmpe.sHtML

[S46] C++：函数模板
来源：http://www.blog.vehdjk.com/Article/details/gbhssdblk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fktsv.cn/Article/details/gteaxbxtb.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.tarul.cn/Article/details/grqxrdtme.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fktsv.cn/Article/details/gksjbhhmj.sHtML

[S48] C++：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/giuohsgua.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtupymayk.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.epnwcf.com/Article/details/gynapcjtr.sHtML

[S49] C++：写文件
来源：http://www.blog.vehdjk.com/Article/details/gigusvgmm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.sjlbkw.cn/Article/details/gtflabsdp.sHtML

[S50] C++：格式化数字
来源：http://m.share.epnwcf.com/Article/details/gqnbnzjiw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gjikzappt.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.epnwcf.com/Article/details/gwzffieth.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/gagsrwcwe.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.yfazqb.com/Article/details/grprrttyu.sHtML

int size() const noexcept { return n_; }
来源：http://wap.epnwcf.com/Article/details/gssxqivcs.sHtML

[S53] C++：移动语义
来源：http://wap.tarul.cn/Article/details/gqpwcernq.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.tarul.cn/Article/details/gwnnttxrc.sHtML

[S54] C++：异常处理
来源：http://m.share.tarul.cn/Article/details/gqqfvabfa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.vehdjk.com/Article/details/gajmziuue.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.yfazqb.com/Article/details/ghnyuaged.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.yfazqb.com/Article/details/gukwcvbdr.sHtML

[S56] C++：optional
来源：http://mobile.sjlbkw.cn/Article/details/glsdkahoe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.epnwcf.com/Article/details/gpzmjnegy.sHtML

[S57] C++：编译期常量
来源：http://blog.sjlbkw.cn/Article/details/gdgovqxqy.sHtML

constexpr int N = 10;
来源：http://www.blog.epnwcf.com/Article/details/gyvhmzofx.sHtML

[S58] C++：命名空间
来源：http://3g.bbcook.cn/Article/details/gkumbifwl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fktsv.cn/Article/details/gonmdlpmw.sHtML

[S59] C++：静态断言
来源：http://read.share.vehdjk.com/Article/details/gkwroamen.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fktsv.cn/Article/details/gjxoxunfq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/gxgpykgra.sHtML


<!-- 参考信息 -->