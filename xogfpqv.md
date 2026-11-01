代发 wailian999

readonly PI=3.14
来源：http://blog.vehdjk.com/Article/details/gapbdeleo.sHtML

[R04] 位置参数
来源：http://m.share.bbcook.cn/Article/details/gxtzauxoi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.yfazqb.com/Article/details/geswinyfi.sHtML

[R05] 参数默认值
来源：http://3g.vehdjk.com/Article/details/gzrswncmh.sHtML

name="${1:-default}"
来源：http://mobile.vehdjk.com/Article/details/gpwroudgx.sHtML

[R06] 判断命令是否存在
来源：http://3g.bbcook.cn/Article/details/gvkslpdjt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gwneulvoa.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gauuzugpl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gmyaghgqc.sHtML

[R08] 数值比较
来源：http://baike.vehdjk.com/Article/details/gvwfelrqk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.yfazqb.com/Article/details/gwiolwcbs.sHtML

[R09] 字符串比较
来源：http://mobile.bbcook.cn/Article/details/gdowthmnz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fktsv.cn/Article/details/gkaitjtyi.sHtML

[R10] 正则匹配
来源：http://read.share.tarul.cn/Article/details/gswneuzfd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gdagzixjb.sHtML

[R11] case 多分支
来源：http://baike.tarul.cn/Article/details/guboxqagk.sHtML

case "$1" in
来源：http://www.m.share.tarul.cn/Article/details/ghjzxjsvx.sHtML

start) echo "启动" ;;
来源：http://3g.fktsv.cn/Article/details/garnuaumm.sHtML

stop)  echo "停止" ;;
来源：http://3g.epnwcf.com/Article/details/giccfcjyl.sHtML

*)     echo "未知命令" ;;
来源：http://blog.tarul.cn/Article/details/gdinlmvxq.sHtML

esac
来源：http://www.share.sjlbkw.cn/Article/details/gketqyudw.sHtML

[R12] for 遍历文件
来源：http://wap.epnwcf.com/Article/details/gpeabjecq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.yfazqb.com/Article/details/gpyhorlvp.sHtML

[R13] for 计数循环
来源：http://3g.yfazqb.com/Article/details/gbpkpcavn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/gjvjgqcvx.sHtML

[R14] C 风格 for
来源：http://mobile.fktsv.cn/Article/details/glgwtrqxq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/gkoeohmcb.sHtML

[R15] while 逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gpugkzusr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.vehdjk.com/Article/details/gvnmxrska.sHtML

[R16] until 等待条件
来源：http://mobile.bbcook.cn/Article/details/gxdkrvvnw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.bbcook.cn/Article/details/grcjzjyjb.sHtML

[R17] 数组定义与取值
来源：http://baike.epnwcf.com/Article/details/gfhgctldi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.sjlbkw.cn/Article/details/gthcvuzbg.sHtML

[R18] 遍历数组
来源：http://www.share.sjlbkw.cn/Article/details/gvlyjdulq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fktsv.cn/Article/details/gmkitlqik.sHtML

[R19] 数组长度
来源：http://www.blog.tarul.cn/Article/details/gjhzdkxjs.sHtML

echo "${#arr[@]}"
来源：http://mobile.bbcook.cn/Article/details/gishiqsau.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.yfazqb.com/Article/details/gcppjmjjg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.bbcook.cn/Article/details/grrfckrkf.sHtML

[R21] 字符串长度
来源：http://m.share.bbcook.cn/Article/details/gbeyjfhfp.sHtML

echo "${#s}"
来源：http://blog.tarul.cn/Article/details/gccyjjlbk.sHtML

[R22] 截取子串
来源：http://m.share.epnwcf.com/Article/details/gijratmny.sHtML

echo "${s:0:5}"
来源：http://www.blog.tarul.cn/Article/details/grkntwisu.sHtML

[R23] 字符串替换
来源：http://3g.epnwcf.com/Article/details/grndshljq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.vehdjk.com/Article/details/gducegqpx.sHtML

[R24] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/grfncbstr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.tarul.cn/Article/details/grbnbjzkp.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.bbcook.cn/Article/details/gluddiljr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.yfazqb.com/Article/details/ginlkykph.sHtML

[R26] 命令替换
来源：http://www.m.share.vehdjk.com/Article/details/gkkypwlbi.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.sjlbkw.cn/Article/details/grwewajpi.sHtML

[R27] 算术展开
来源：http://www.blog.yfazqb.com/Article/details/gunhelnaz.sHtML

echo $((1 + 2 * 3))
来源：http://3g.bbcook.cn/Article/details/gqyiqmxym.sHtML

[R28] 浮点运算
来源：http://wap.sjlbkw.cn/Article/details/gcmdasljv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.sjlbkw.cn/Article/details/guunflsem.sHtML

[R29] 定义函数
来源：http://wap.fktsv.cn/Article/details/gyioemddp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.vehdjk.com/Article/details/gwmtjhnuv.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/gkoobwjhi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxalztvqm.sHtML

[R31] 局部变量
来源：http://3g.fktsv.cn/Article/details/gimpyvljy.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.tarul.cn/Article/details/gwmievfzk.sHtML

[R32] 参数个数校验
来源：http://3g.vehdjk.com/Article/details/gtzibekab.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gcouxlkkd.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.yfazqb.com/Article/details/guxsfsqzk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.epnwcf.com/Article/details/gygukugzd.sHtML

[R34] 退出时清理
来源：http://mobile.epnwcf.com/Article/details/gjbacbryn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/gdxwpbpcd.sHtML

[R35] 后台执行并等待
来源：http://baike.yfazqb.com/Article/details/gfqikclco.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.yfazqb.com/Article/details/gebbyedif.sHtML

[R36] 并发执行多个任务
来源：http://baike.sjlbkw.cn/Article/details/gbfkvyuyc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fktsv.cn/Article/details/gdrfsiasq.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fktsv.cn/Article/details/geoafcyfr.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/gqhegkaue.sHtML

[R38] 管道串联
来源：http://wap.bbcook.cn/Article/details/ghdqsdpsz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fktsv.cn/Article/details/gwafjxovh.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/ggrzbfvpd.sHtML

cmd > out.log 2>&1
来源：http://3g.epnwcf.com/Article/details/glxtavspi.sHtML

[R40] 追加写日志
来源：http://wap.sjlbkw.cn/Article/details/guaeeqjuw.sHtML

echo "log" >> out.log
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcswuyln.sHtML

[R41] 丢弃输出
来源：http://read.share.bbcook.cn/Article/details/gkzyidwht.sHtML

cmd >/dev/null 2>&1
来源：http://baike.epnwcf.com/Article/details/gzkquqdbq.sHtML

[R42] 输入重定向
来源：http://www.m.share.tarul.cn/Article/details/gebidjlgc.sHtML

wc -l < a.txt
来源：http://read.share.epnwcf.com/Article/details/gqcnjqskt.sHtML

[R43] 按名字查找文件
来源：http://read.share.sjlbkw.cn/Article/details/gidghjuke.sHtML

find . -name "*.log" -type f
来源：http://3g.fktsv.cn/Article/details/gvbezigoo.sHtML

[R44] 按修改时间查找
来源：http://baike.bbcook.cn/Article/details/gwwansrhd.sHtML

find . -mtime -7 -type f
来源：http://read.share.epnwcf.com/Article/details/grtqodoxc.sHtML

[R45] 批量删除
来源：http://www.m.share.bbcook.cn/Article/details/gdggbwswi.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fktsv.cn/Article/details/gicyccdkb.sHtML

[R46] 递归替换文件内容
来源：http://3g.bbcook.cn/Article/details/gsiropvbx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.yfazqb.com/Article/details/gqooqskvw.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/gygkflsok.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fktsv.cn/Article/details/guojlsncu.sHtML

[R48] awk 取指定列
来源：http://wap.epnwcf.com/Article/details/gtqtdnhfc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gqgfbsslj.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/geejdyvml.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.tarul.cn/Article/details/gigkuqmqq.sHtML

[R50] awk 求和
来源：http://3g.vehdjk.com/Article/details/gushcabut.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.epnwcf.com/Article/details/gggzqipmj.sHtML

[R51] 排序去重取前几
来源：http://m.share.fktsv.cn/Article/details/gtlumbptx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/garfsyugj.sHtML

[R52] 统计行数
来源：http://www.m.share.bbcook.cn/Article/details/gigbgvtvy.sHtML

wc -l a.txt
来源：http://www.share.epnwcf.com/Article/details/gtzhtuyhb.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.sjlbkw.cn/Article/details/gojtcskpq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fktsv.cn/Article/details/gvkzwjinj.sHtML

[R54] 比较两个文件
来源：http://m.share.sjlbkw.cn/Article/details/gpbyheizi.sHtML

diff a.txt b.txt
来源：http://blog.bbcook.cn/Article/details/gupxtojfe.sHtML

[R55] 压缩与解压
来源：http://read.share.yfazqb.com/Article/details/gcthfvyov.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.bbcook.cn/Article/details/gntmpvyya.sHtML

[R56] 远程拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gartttoht.sHtML

scp file user@host:/path/
来源：http://wap.epnwcf.com/Article/details/gvltgzvmh.sHtML

[R57] 远程执行命令
来源：http://mobile.vehdjk.com/Article/details/gsvrwstno.sHtML

ssh user@host 'uptime'
来源：http://3g.epnwcf.com/Article/details/gozeeouun.sHtML

[R58] 下载文件
来源：http://baike.epnwcf.com/Article/details/gdwpftdbm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.sjlbkw.cn/Article/details/gbtpnwqmz.sHtML

[R59] 发 POST JSON
来源：http://mobile.tarul.cn/Article/details/glbakenfc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.epnwcf.com/Article/details/gvrghmibn.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.epnwcf.com/Article/details/gdzpiclcd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.bbcook.cn/Article/details/gnwtznnhh.sHtML

[R61] 磁盘占用
来源：http://www.blog.tarul.cn/Article/details/gefjbnxxy.sHtML

df -h;  du -sh *
来源：http://www.m.share.fktsv.cn/Article/details/guffletpn.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/gkctbrldw.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.vehdjk.com/Article/details/giodwlbry.sHtML

[R63] 内存与进程
来源：http://m.share.epnwcf.com/Article/details/ggpycswtl.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.sjlbkw.cn/Article/details/garzewelw.sHtML

[R64] 结束进程
来源：http://mobile.yfazqb.com/Article/details/gjzvkfxfs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.tarul.cn/Article/details/grjhcjimt.sHtML

[R65] 查看端口占用
来源：http://www.blog.tarul.cn/Article/details/gvxcfjjuz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.epnwcf.com/Article/details/gymnckpks.sHtML

[R66] 定时任务
来源：http://baike.fktsv.cn/Article/details/goqvmhois.sHtML

crontab -e;  crontab -l
来源：http://mobile.vehdjk.com/Article/details/gekblksfw.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.sjlbkw.cn/Article/details/ggsfnnlin.sHtML

openssl rand -hex 16
来源：http://www.blog.tarul.cn/Article/details/gphrfltkg.sHtML

[R68] 计算文件校验值
来源：http://3g.fktsv.cn/Article/details/gyfsqqevq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.epnwcf.com/Article/details/gpppobhcc.sHtML

[R69] 生成随机密码
来源：http://baike.tarul.cn/Article/details/gxuqemnjq.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.tarul.cn/Article/details/gdpjcwljz.sHtML

[R70] 时间戳与互转
来源：http://m.share.sjlbkw.cn/Article/details/gzxrtvmeq.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.tarul.cn/Article/details/ghmankjdr.sHtML

[R71] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gvfcknlui.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.bbcook.cn/Article/details/ggholuqtx.sHtML

[R72] 等待端口就绪
来源：http://www.blog.yfazqb.com/Article/details/goxchgrfe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/guvjrbakq.sHtML

[R73] 分割大日志
来源：http://www.share.fktsv.cn/Article/details/gmopnlzww.sHtML

split -l 1000 big.log part_
来源：http://blog.vehdjk.com/Article/details/gdkhfnxxv.sHtML

[R74] 批量重命名
来源：http://m.share.fktsv.cn/Article/details/gombkcslg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.sjlbkw.cn/Article/details/goonzjdle.sHtML

[R75] 导出环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gsyonfikv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.yfazqb.com/Article/details/gtwmwwqoi.sHtML

[R76] 使用临时文件
来源：http://www.share.vehdjk.com/Article/details/gtrzsaqsv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gqajsxfwd.sHtML

[R77] 读取用户输入
来源：http://read.share.tarul.cn/Article/details/gfbxnacih.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.yfazqb.com/Article/details/gdznfeeli.sHtML

[R78] 交互式菜单
来源：http://www.m.share.epnwcf.com/Article/details/giyurbmdv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.vehdjk.com/Article/details/gpgoffwre.sHtML

[R79] 解析命令行选项
来源：http://baike.fktsv.cn/Article/details/grylvjskc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.epnwcf.com/Article/details/gasbdccwg.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.yfazqb.com/Article/details/gfgmdwgcb.sHtML

time ./run.sh
来源：http://wap.tarul.cn/Article/details/glciigbsq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdwmhhqgo.sHtML

S. C / C++ 专题
来源：http://m.share.vehdjk.com/Article/details/gykvibgnv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gacfjasho.sHtML

[S01] C：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gqguslwvk.sHtML

#include <stdio.h>
来源：http://www.share.fktsv.cn/Article/details/gazkcqqxi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fktsv.cn/Article/details/gmyvmvmyq.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.yfazqb.com/Article/details/gegjcmrhl.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fktsv.cn/Article/details/grztqferm.sHtML

[S03] C：读入整数
来源：http://baike.fktsv.cn/Article/details/gazfdrmpc.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.tarul.cn/Article/details/gbdlkdfyl.sHtML

[S04] C：字符串复制
来源：http://www.m.share.bbcook.cn/Article/details/gracvhqni.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.vehdjk.com/Article/details/godxmnjuf.sHtML

[S05] C：字符串长度
来源：http://blog.vehdjk.com/Article/details/geykjlhth.sHtML

strlen(s)
来源：http://wap.epnwcf.com/Article/details/gbevieqoc.sHtML

[S06] C：字符串比较
来源：http://blog.fktsv.cn/Article/details/gptbpgscr.sHtML

strcmp(a, b) == 0
来源：http://read.share.vehdjk.com/Article/details/gmvhcmnok.sHtML

[S07] C：数组遍历求和
来源：http://m.share.epnwcf.com/Article/details/gnqqerhtb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.bbcook.cn/Article/details/ghewunrje.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.vehdjk.com/Article/details/gdehosiga.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.sjlbkw.cn/Article/details/gkqpthldq.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.tarul.cn/Article/details/gmwxbeumr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.tarul.cn/Article/details/ghqmcrzkx.sHtML

[S10] C：指针与解引用
来源：http://www.share.tarul.cn/Article/details/gxjsiegtl.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fktsv.cn/Article/details/ghjpjjzoj.sHtML

[S11] C：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/ggixneeis.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.vehdjk.com/Article/details/gyvnnwxrc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.epnwcf.com/Article/details/gweiqwotw.sHtML

fclose(f);
来源：http://baike.epnwcf.com/Article/details/gxvgbpxtr.sHtML

[S12] C：写文件
来源：http://mobile.tarul.cn/Article/details/gqnpthtmi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.epnwcf.com/Article/details/ggngucrou.sHtML

[S13] C：宏定义
来源：http://read.share.epnwcf.com/Article/details/gprzglqqy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.yfazqb.com/Article/details/gfvuhilxr.sHtML

[S14] C：枚举
来源：http://3g.yfazqb.com/Article/details/gxegnfjfe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.sjlbkw.cn/Article/details/gbvvtrswp.sHtML

[S15] C：类型转换
来源：http://read.share.fktsv.cn/Article/details/giebsduxn.sHtML

(double) a / b
来源：http://mobile.epnwcf.com/Article/details/gsodxtvdl.sHtML

[S16] C：位操作置位
来源：http://m.share.fktsv.cn/Article/details/gyereqfsv.sHtML

x |= (1 << 3);
来源：http://baike.fktsv.cn/Article/details/guusydnso.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fktsv.cn/Article/details/gvgtrqqeo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fktsv.cn/Article/details/gwstfcxak.sHtML

[S18] C：命令行参数
来源：http://m.share.yfazqb.com/Article/details/gaszjfauf.sHtML

int main(int argc, char **argv)
来源：http://blog.vehdjk.com/Article/details/gczvyiqfw.sHtML

[S19] C：快速排序
来源：http://baike.epnwcf.com/Article/details/gqedwcivj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/ghgtaxmvi.sHtML

[S20] C：二分查找
来源：http://read.share.fktsv.cn/Article/details/gomnbfqtj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/gtuqlqerl.sHtML

[S21] C：字符类别判断
来源：http://3g.epnwcf.com/Article/details/gwehqfhda.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.sjlbkw.cn/Article/details/gqpsfscfl.sHtML

[S22] C：字符串转数字
来源：http://www.share.bbcook.cn/Article/details/gfbiiypxk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/glnbxfvjn.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/grlgqptvd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.yfazqb.com/Article/details/gtcnsbngl.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.bbcook.cn/Article/details/gplppueiq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.bbcook.cn/Article/details/gvdllmdaa.sHtML

[S25] C：内存拷贝
来源：http://wap.fktsv.cn/Article/details/giusvaoky.sHtML

memcpy(dst, src, n);
来源：http://mobile.tarul.cn/Article/details/gaxvpmjht.sHtML

[S26] C：内存清零
来源：http://www.m.share.tarul.cn/Article/details/guopizkpk.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.yfazqb.com/Article/details/gkvjltvdd.sHtML

[S27] C：定义常量
来源：http://www.share.vehdjk.com/Article/details/giooslkzb.sHtML

const double PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/guosnodso.sHtML

[S28] C：静态变量
来源：http://m.share.fktsv.cn/Article/details/grnrpqhmm.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/gvkkpzcrt.sHtML

[S29] C：变参函数
来源：http://www.blog.tarul.cn/Article/details/gzaacxaqh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfromcoug.sHtML

[S30] C：头文件保护
来源：http://3g.tarul.cn/Article/details/geshukybs.sHtML

#ifndef X_H
来源：http://read.share.yfazqb.com/Article/details/gcjpkjbqm.sHtML

#define X_H
来源：http://m.share.bbcook.cn/Article/details/grlaysscl.sHtML

#endif
来源：http://wap.fktsv.cn/Article/details/glkfhjvii.sHtML

[S31] C++：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gwdvdrknw.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gcsgyzxmt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/giioohqgs.sHtML

[S32] C++：字符串
来源：http://read.share.bbcook.cn/Article/details/gbvelekqv.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.yfazqb.com/Article/details/gjkvzigsz.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/gnndggvpp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.vehdjk.com/Article/details/gyuxrfiut.sHtML

[S34] C++：遍历 vector
来源：http://www.share.tarul.cn/Article/details/gtgrhxjsk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/ghgwozysk.sHtML

[S35] C++：map
来源：http://m.share.vehdjk.com/Article/details/glaawzsxc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/guipttftr.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.yfazqb.com/Article/details/gmzmwzkpp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gaoyinxqt.sHtML

[S37] C++：set
来源：http://m.share.bbcook.cn/Article/details/geknokacp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.epnwcf.com/Article/details/ghaseooxk.sHtML

[S38] C++：排序
来源：http://3g.sjlbkw.cn/Article/details/gxwsjnhwz.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.epnwcf.com/Article/details/goziwwjnk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.epnwcf.com/Article/details/gmxyxdkdh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/gfvajbxmw.sHtML

[S40] C++：查找元素
来源：http://mobile.vehdjk.com/Article/details/gneqqxhbj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.yfazqb.com/Article/details/gxdqobbxe.sHtML

[S41] C++：类与构造函数
来源：http://wap.sjlbkw.cn/Article/details/gfrgssxhx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/ggswrhbrd.sHtML

[S42] C++：继承与虚函数
来源：http://baike.vehdjk.com/Article/details/gokbhzmzx.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.vehdjk.com/Article/details/gcstuxael.sHtML

[S43] C++：智能指针
来源：http://read.share.bbcook.cn/Article/details/gqapcxndd.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.yfazqb.com/Article/details/geumfetzw.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/grasiislj.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.tarul.cn/Article/details/gteznzlni.sHtML

[S45] C++：lambda
来源：http://3g.vehdjk.com/Article/details/gszkvrzfz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gkuwdmsbz.sHtML

[S46] C++：函数模板
来源：http://wap.bbcook.cn/Article/details/gunjjhhik.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.epnwcf.com/Article/details/gvaitpqxt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.sjlbkw.cn/Article/details/gntswcyie.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.epnwcf.com/Article/details/guhjusnaa.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gqpurhdun.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.tarul.cn/Article/details/gmamcekjh.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fktsv.cn/Article/details/gxajfymfc.sHtML

[S49] C++：写文件
来源：http://m.share.vehdjk.com/Article/details/gmvlzhxbl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fktsv.cn/Article/details/gsucjyora.sHtML

[S50] C++：格式化数字
来源：http://blog.vehdjk.com/Article/details/gmhhhdsjb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gkfmcfyqs.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fktsv.cn/Article/details/gmxozzyfk.sHtML

static_cast<double>(a) / b
来源：http://3g.fktsv.cn/Article/details/gagjblnto.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.epnwcf.com/Article/details/gjfvynjel.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/gayriyhfa.sHtML

[S53] C++：移动语义
来源：http://www.m.share.tarul.cn/Article/details/ghzyvhwmd.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fktsv.cn/Article/details/gtcygacar.sHtML

[S54] C++：异常处理
来源：http://mobile.sjlbkw.cn/Article/details/gddanjqka.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.yfazqb.com/Article/details/gglhgwyqo.sHtML

[S55] C++：结构化绑定
来源：http://baike.bbcook.cn/Article/details/gzxthwtue.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/guywfsojf.sHtML

[S56] C++：optional
来源：http://wap.yfazqb.com/Article/details/gxdviivoi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.bbcook.cn/Article/details/gafwuimvz.sHtML

[S57] C++：编译期常量
来源：http://m.share.bbcook.cn/Article/details/gieraocqa.sHtML

constexpr int N = 10;
来源：http://3g.sjlbkw.cn/Article/details/gqfcrfxaa.sHtML

[S58] C++：命名空间
来源：http://wap.tarul.cn/Article/details/gustccsqw.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.bbcook.cn/Article/details/gktdkhktw.sHtML

[S59] C++：静态断言
来源：http://www.m.share.epnwcf.com/Article/details/gfqhmgdlk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.sjlbkw.cn/Article/details/gajgofppe.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.epnwcf.com/Article/details/gwxvymktt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.epnwcf.com/Article/details/gwnyqezzn.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gqsqfhtfk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gamttphxg.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gwjxxtimo.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gfopshouv.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gvzvtmylo.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.vehdjk.com/Article/details/gaxuoujqw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.tarul.cn/Article/details/gacriaqce.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.sjlbkw.cn/Article/details/goiwrbklr.sHtML

"值: $b"
来源：http://baike.bbcook.cn/Article/details/gfqbuksra.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/gtehlatxw.sHtML

val n: String? = null;  n?.length
来源：http://mobile.vehdjk.com/Article/details/gaknpxjae.sHtML


<!-- 参考信息 -->