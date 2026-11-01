代发 wailian999

case "$1" in
来源：http://mobile.fktsv.cn/Article/details/gqbpqfjid.sHtML

start) echo "启动" ;;
来源：http://3g.fktsv.cn/Article/details/gyousmeqt.sHtML

stop)  echo "停止" ;;
来源：http://3g.vehdjk.com/Article/details/ggfsluxrr.sHtML

*)     echo "未知命令" ;;
来源：http://3g.vehdjk.com/Article/details/grprccjis.sHtML

esac
来源：http://www.share.fktsv.cn/Article/details/gnkkmiczx.sHtML

[R12] for 遍历文件
来源：http://baike.epnwcf.com/Article/details/gxqtnwjdf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.tarul.cn/Article/details/gxhvljndk.sHtML

[R13] for 计数循环
来源：http://3g.sjlbkw.cn/Article/details/glpavpcty.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/goiljrbkw.sHtML

[R14] C 风格 for
来源：http://www.share.sjlbkw.cn/Article/details/gphxsvrwn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gsazujpkt.sHtML

[R15] while 逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gmzvaksdp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.tarul.cn/Article/details/gjilzxwfj.sHtML

[R16] until 等待条件
来源：http://wap.yfazqb.com/Article/details/ggswtlmuk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/gsgptrctm.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.yfazqb.com/Article/details/gsbmafstx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.bbcook.cn/Article/details/ggwmooqfp.sHtML

[R18] 遍历数组
来源：http://read.share.bbcook.cn/Article/details/gimaqprrp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fktsv.cn/Article/details/gbvzrliuj.sHtML

[R19] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gvopjkwha.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.tarul.cn/Article/details/gkoygptol.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fktsv.cn/Article/details/gfontodia.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.sjlbkw.cn/Article/details/gocluoncx.sHtML

[R21] 字符串长度
来源：http://wap.bbcook.cn/Article/details/gzspdmyke.sHtML

echo "${#s}"
来源：http://read.share.sjlbkw.cn/Article/details/ghngphtaq.sHtML

[R22] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gimniahls.sHtML

echo "${s:0:5}"
来源：http://www.blog.bbcook.cn/Article/details/glpygpkso.sHtML

[R23] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gsjtucktl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.epnwcf.com/Article/details/gmqlhbgbt.sHtML

[R24] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/gfabxyusu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fktsv.cn/Article/details/giavqyfqk.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.epnwcf.com/Article/details/gmmpcjqft.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.tarul.cn/Article/details/gmsnafqdv.sHtML

[R26] 命令替换
来源：http://www.m.share.epnwcf.com/Article/details/gbcrjonyn.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.tarul.cn/Article/details/gwhvdipml.sHtML

[R27] 算术展开
来源：http://www.blog.bbcook.cn/Article/details/gpifpzdlp.sHtML

echo $((1 + 2 * 3))
来源：http://baike.vehdjk.com/Article/details/gwupijojs.sHtML

[R28] 浮点运算
来源：http://m.share.yfazqb.com/Article/details/gycuribgk.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fktsv.cn/Article/details/gtfhmjkxp.sHtML

[R29] 定义函数
来源：http://read.share.vehdjk.com/Article/details/grdxhlhgg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.yfazqb.com/Article/details/gmxlfgxcm.sHtML

[R30] 函数返回状态码
来源：http://m.share.fktsv.cn/Article/details/guhojqewa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.bbcook.cn/Article/details/gioxieyiz.sHtML

[R31] 局部变量
来源：http://www.m.share.vehdjk.com/Article/details/gpijtgide.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.epnwcf.com/Article/details/gftcgpqmv.sHtML

[R32] 参数个数校验
来源：http://3g.bbcook.cn/Article/details/gfceqytaw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/gnxxjnswm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.tarul.cn/Article/details/ghrrhsdqh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.yfazqb.com/Article/details/grtnyasxi.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/gjthvykof.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/gfuypgkkk.sHtML

[R35] 后台执行并等待
来源：http://read.share.yfazqb.com/Article/details/gxlydiqrw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.vehdjk.com/Article/details/gzeqiylko.sHtML

[R36] 并发执行多个任务
来源：http://wap.sjlbkw.cn/Article/details/giloktgej.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fktsv.cn/Article/details/gfkwwjksj.sHtML

[R37] 把输出赋给变量
来源：http://3g.vehdjk.com/Article/details/gvozkevqn.sHtML

files=$(ls -1)
来源：http://www.m.share.bbcook.cn/Article/details/gutzqctvx.sHtML

[R38] 管道串联
来源：http://www.blog.fktsv.cn/Article/details/gljjfoocq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fktsv.cn/Article/details/golkfhqvs.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.sjlbkw.cn/Article/details/ghicvclkx.sHtML

cmd > out.log 2>&1
来源：http://mobile.bbcook.cn/Article/details/gsxvztppz.sHtML

[R40] 追加写日志
来源：http://read.share.fktsv.cn/Article/details/gphisafgj.sHtML

echo "log" >> out.log
来源：http://mobile.yfazqb.com/Article/details/gvjapesav.sHtML

[R41] 丢弃输出
来源：http://blog.fktsv.cn/Article/details/gsxmshytd.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.epnwcf.com/Article/details/gdpbmciac.sHtML

[R42] 输入重定向
来源：http://baike.epnwcf.com/Article/details/gdqkvplpd.sHtML

wc -l < a.txt
来源：http://mobile.yfazqb.com/Article/details/gdyosflij.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gviaqcrkt.sHtML

find . -name "*.log" -type f
来源：http://wap.epnwcf.com/Article/details/gywktzrbo.sHtML

[R44] 按修改时间查找
来源：http://baike.epnwcf.com/Article/details/gjeudjxbh.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fktsv.cn/Article/details/gsvptfyvx.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/gffyskwzc.sHtML

find . -name "*.tmp" -delete
来源：http://wap.bbcook.cn/Article/details/gtdsmvjtc.sHtML

[R46] 递归替换文件内容
来源：http://wap.fktsv.cn/Article/details/gccrysvdl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.yfazqb.com/Article/details/gzsijsvgy.sHtML

[R47] sed 单行替换
来源：http://3g.epnwcf.com/Article/details/gaidmoffs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.yfazqb.com/Article/details/gegagihlj.sHtML

[R48] awk 取指定列
来源：http://m.share.tarul.cn/Article/details/gdquosrfu.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.tarul.cn/Article/details/gvttnzwfc.sHtML

[R49] awk 带条件
来源：http://m.share.bbcook.cn/Article/details/gsshaojoj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.epnwcf.com/Article/details/gkvhstwef.sHtML

[R50] awk 求和
来源：http://read.share.yfazqb.com/Article/details/gbqemwstx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fktsv.cn/Article/details/grngawcot.sHtML

[R51] 排序去重取前几
来源：http://mobile.bbcook.cn/Article/details/gripkvdmb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.vehdjk.com/Article/details/gdybfzuyr.sHtML

[R52] 统计行数
来源：http://www.blog.sjlbkw.cn/Article/details/gsglzrdjw.sHtML

wc -l a.txt
来源：http://wap.epnwcf.com/Article/details/ghwuoemii.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.tarul.cn/Article/details/gjdizoamh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fktsv.cn/Article/details/gjfoxjgkg.sHtML

[R54] 比较两个文件
来源：http://blog.vehdjk.com/Article/details/gjlqggsza.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/gmxeuljwi.sHtML

[R55] 压缩与解压
来源：http://mobile.yfazqb.com/Article/details/gxbuqbpcz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/giscmsrsw.sHtML

[R56] 远程拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gjagwgtav.sHtML

scp file user@host:/path/
来源：http://www.blog.epnwcf.com/Article/details/gwdqkbyyf.sHtML

[R57] 远程执行命令
来源：http://www.blog.fktsv.cn/Article/details/giyacbuuk.sHtML

ssh user@host 'uptime'
来源：http://baike.tarul.cn/Article/details/ghcragcrb.sHtML

[R58] 下载文件
来源：http://m.share.vehdjk.com/Article/details/glekuayot.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.epnwcf.com/Article/details/gmkuefbyn.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/gdiqjbupr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.bbcook.cn/Article/details/gbjbapgfp.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gimmhalda.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/gkkbprwao.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/gxgzffxnu.sHtML

df -h;  du -sh *
来源：http://www.blog.vehdjk.com/Article/details/gzedsywnn.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.vehdjk.com/Article/details/gbsaxspft.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.sjlbkw.cn/Article/details/gqoggbsad.sHtML

[R63] 内存与进程
来源：http://mobile.tarul.cn/Article/details/ggikympbs.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.sjlbkw.cn/Article/details/gptyubpuf.sHtML

[R64] 结束进程
来源：http://baike.tarul.cn/Article/details/gtbpkdcjn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.tarul.cn/Article/details/gqffirklw.sHtML

[R65] 查看端口占用
来源：http://www.m.share.bbcook.cn/Article/details/gdaojmjar.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fktsv.cn/Article/details/gpgdotsha.sHtML

[R66] 定时任务
来源：http://www.share.fktsv.cn/Article/details/gromykptv.sHtML

crontab -e;  crontab -l
来源：http://m.share.yfazqb.com/Article/details/gitrxtpah.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.sjlbkw.cn/Article/details/gndauyxxy.sHtML

openssl rand -hex 16
来源：http://wap.bbcook.cn/Article/details/gtmtksawk.sHtML

[R68] 计算文件校验值
来源：http://read.share.bbcook.cn/Article/details/gpsfizyzf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.bbcook.cn/Article/details/gggjpihhf.sHtML

[R69] 生成随机密码
来源：http://baike.tarul.cn/Article/details/gzlhnefwe.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/guubvlbas.sHtML

[R70] 时间戳与互转
来源：http://m.share.tarul.cn/Article/details/ggpgjxvrm.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.sjlbkw.cn/Article/details/gvlkhnrke.sHtML

[R71] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gngthsqtx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.vehdjk.com/Article/details/gouozwkid.sHtML

[R72] 等待端口就绪
来源：http://3g.tarul.cn/Article/details/gbtfwdmej.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/goyipfsxt.sHtML

[R73] 分割大日志
来源：http://baike.sjlbkw.cn/Article/details/gierltubg.sHtML

split -l 1000 big.log part_
来源：http://www.share.vehdjk.com/Article/details/gpjngbmtm.sHtML

[R74] 批量重命名
来源：http://3g.tarul.cn/Article/details/gjkvgaizk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.vehdjk.com/Article/details/gxtkvecyj.sHtML

[R75] 导出环境变量
来源：http://mobile.epnwcf.com/Article/details/gvxycykkk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.bbcook.cn/Article/details/giairgdhq.sHtML

[R76] 使用临时文件
来源：http://blog.sjlbkw.cn/Article/details/grnorailw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/goadwvqqx.sHtML

[R77] 读取用户输入
来源：http://blog.sjlbkw.cn/Article/details/gzrixcswy.sHtML

read -rp "请输入: " ans
来源：http://read.share.yfazqb.com/Article/details/geiropjci.sHtML

[R78] 交互式菜单
来源：http://wap.vehdjk.com/Article/details/garbutuar.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.vehdjk.com/Article/details/gyyohxpwf.sHtML

[R79] 解析命令行选项
来源：http://3g.fktsv.cn/Article/details/glhkxeqim.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.yfazqb.com/Article/details/gatuzwoui.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.tarul.cn/Article/details/gcfelohtm.sHtML

time ./run.sh
来源：http://www.blog.epnwcf.com/Article/details/gwidrkyvp.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gsddmllbm.sHtML

S. C / C++ 专题
来源：http://www.m.share.vehdjk.com/Article/details/gcibfssnn.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ggpzvgmos.sHtML

[S01] C：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/ggbehauaw.sHtML

#include <stdio.h>
来源：http://www.m.share.yfazqb.com/Article/details/gjmbihkxn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/gfujinzql.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fktsv.cn/Article/details/gzqmvccxv.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fktsv.cn/Article/details/gqdxkveii.sHtML

[S03] C：读入整数
来源：http://read.share.yfazqb.com/Article/details/gfrvrqmjp.sHtML

int x; scanf("%d", &x);
来源：http://blog.vehdjk.com/Article/details/gcdokwasy.sHtML

[S04] C：字符串复制
来源：http://www.share.sjlbkw.cn/Article/details/gjeqtjzip.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.yfazqb.com/Article/details/gqaceebte.sHtML

[S05] C：字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gbuvshcno.sHtML

strlen(s)
来源：http://www.m.share.vehdjk.com/Article/details/gsieygvhy.sHtML

[S06] C：字符串比较
来源：http://m.share.epnwcf.com/Article/details/gooduxmgq.sHtML

strcmp(a, b) == 0
来源：http://blog.bbcook.cn/Article/details/grhxwneka.sHtML

[S07] C：数组遍历求和
来源：http://wap.vehdjk.com/Article/details/gfazdyyex.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.epnwcf.com/Article/details/gidjszztg.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.vehdjk.com/Article/details/gxzjwcsbi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.yfazqb.com/Article/details/gfvbvegvw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.tarul.cn/Article/details/guvovlwit.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.yfazqb.com/Article/details/grmxshjpl.sHtML

[S10] C：指针与解引用
来源：http://wap.tarul.cn/Article/details/gzhsubnku.sHtML

int *p = &a;  *p = 5;
来源：http://wap.bbcook.cn/Article/details/geoouojhy.sHtML

[S11] C：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/grzpxkxqp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.vehdjk.com/Article/details/gxybuhunk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.epnwcf.com/Article/details/grhgkswls.sHtML

fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gihstpjvf.sHtML

[S12] C：写文件
来源：http://wap.fktsv.cn/Article/details/gtpfkansx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gngwagyhq.sHtML

[S13] C：宏定义
来源：http://baike.yfazqb.com/Article/details/gdjlmyotu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.epnwcf.com/Article/details/ghqkflhzw.sHtML

[S14] C：枚举
来源：http://3g.epnwcf.com/Article/details/gjoajpgel.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.tarul.cn/Article/details/gytioefch.sHtML

[S15] C：类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbfxoqjw.sHtML

(double) a / b
来源：http://www.m.share.fktsv.cn/Article/details/gymjwfrim.sHtML

[S16] C：位操作置位
来源：http://www.share.vehdjk.com/Article/details/gqybsjjip.sHtML

x |= (1 << 3);
来源：http://m.share.yfazqb.com/Article/details/gztuytcof.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.yfazqb.com/Article/details/ghqhsyvao.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.epnwcf.com/Article/details/ghbomyriy.sHtML

[S18] C：命令行参数
来源：http://www.blog.vehdjk.com/Article/details/gxveyugmc.sHtML

int main(int argc, char **argv)
来源：http://m.share.bbcook.cn/Article/details/gzvxgulpq.sHtML

[S19] C：快速排序
来源：http://www.m.share.bbcook.cn/Article/details/gsbzmiocd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gymmngzav.sHtML

[S20] C：二分查找
来源：http://www.blog.sjlbkw.cn/Article/details/geovccknt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/grdwkvdgl.sHtML

[S21] C：字符类别判断
来源：http://3g.epnwcf.com/Article/details/gquurfecf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fktsv.cn/Article/details/gnxzethhg.sHtML

[S22] C：字符串转数字
来源：http://m.share.sjlbkw.cn/Article/details/gdqybsmvz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.bbcook.cn/Article/details/gruckluab.sHtML

[S23] C：随机数
来源：http://m.share.vehdjk.com/Article/details/giyyklmyq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.epnwcf.com/Article/details/gurpjtiog.sHtML

[S24] C：获取本地时间
来源：http://wap.bbcook.cn/Article/details/gmbpjhmxy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.yfazqb.com/Article/details/givwelemp.sHtML

[S25] C：内存拷贝
来源：http://3g.tarul.cn/Article/details/gnemjbtke.sHtML

memcpy(dst, src, n);
来源：http://read.share.epnwcf.com/Article/details/gpeshnqnv.sHtML

[S26] C：内存清零
来源：http://blog.sjlbkw.cn/Article/details/giqqljfts.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/guekllbaf.sHtML

[S27] C：定义常量
来源：http://read.share.tarul.cn/Article/details/gkwcjpuoj.sHtML

const double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gbguxlbnz.sHtML

[S28] C：静态变量
来源：http://www.m.share.yfazqb.com/Article/details/gsphwkhhq.sHtML

static int counter = 0;
来源：http://wap.epnwcf.com/Article/details/gkjfcgufy.sHtML

[S29] C：变参函数
来源：http://baike.fktsv.cn/Article/details/ggkvewjli.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.vehdjk.com/Article/details/gfazxlzkq.sHtML

[S30] C：头文件保护
来源：http://m.share.sjlbkw.cn/Article/details/gqvzvkibq.sHtML

#ifndef X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gqmmlzgnv.sHtML

#define X_H
来源：http://read.share.vehdjk.com/Article/details/gztfrynev.sHtML

#endif
来源：http://read.share.sjlbkw.cn/Article/details/gcqozfmpq.sHtML

[S31] C++：Hello World
来源：http://baike.tarul.cn/Article/details/gxbuknhsl.sHtML

#include <iostream>
来源：http://www.share.sjlbkw.cn/Article/details/gfkupvait.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.tarul.cn/Article/details/gnuutxofv.sHtML

[S32] C++：字符串
来源：http://m.share.bbcook.cn/Article/details/gernmfpkh.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.vehdjk.com/Article/details/gbbthmtto.sHtML

[S33] C++：vector 增删
来源：http://www.share.epnwcf.com/Article/details/gpwwhfaql.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.sjlbkw.cn/Article/details/ghtxtpuim.sHtML

[S34] C++：遍历 vector
来源：http://www.share.bbcook.cn/Article/details/gzvxkfnkp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbgioctbt.sHtML

[S35] C++：map
来源：http://read.share.tarul.cn/Article/details/glhygbbnq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gqdraubrc.sHtML

[S36] C++：unordered_map
来源：http://www.share.yfazqb.com/Article/details/gmxpcrvow.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/ginhlkmfk.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/gojclzpoe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fktsv.cn/Article/details/grocpcpgh.sHtML

[S38] C++：排序
来源：http://read.share.tarul.cn/Article/details/gacolpbzk.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.bbcook.cn/Article/details/gekxshtef.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.epnwcf.com/Article/details/ggiabnblr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.yfazqb.com/Article/details/ghrljhzxo.sHtML

[S40] C++：查找元素
来源：http://m.share.sjlbkw.cn/Article/details/ggjbnjxjg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.epnwcf.com/Article/details/glmocpsoo.sHtML

[S41] C++：类与构造函数
来源：http://3g.bbcook.cn/Article/details/gxjqnzaub.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.bbcook.cn/Article/details/gckrjnbab.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.sjlbkw.cn/Article/details/gkfnxzrqt.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.bbcook.cn/Article/details/gpvcumdrb.sHtML

[S43] C++：智能指针
来源：http://blog.sjlbkw.cn/Article/details/gychvrhdh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.tarul.cn/Article/details/gezpvrpez.sHtML

[S44] C++：引用传参
来源：http://www.share.sjlbkw.cn/Article/details/gklwjgpli.sHtML

void inc(int &x) { ++x; }
来源：http://wap.yfazqb.com/Article/details/guorzmtiq.sHtML

[S45] C++：lambda
来源：http://3g.tarul.cn/Article/details/gvfqpbwkf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.epnwcf.com/Article/details/gmkwioaua.sHtML

[S46] C++：函数模板
来源：http://wap.sjlbkw.cn/Article/details/gkozbfmch.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.yfazqb.com/Article/details/gpooootpo.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.epnwcf.com/Article/details/grcjqogby.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fktsv.cn/Article/details/gygtvsqks.sHtML

[S48] C++：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gbguovnbs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.sjlbkw.cn/Article/details/gbafmfvhm.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.epnwcf.com/Article/details/gucuhqzza.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/glizewveb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.yfazqb.com/Article/details/gowyphxav.sHtML

[S50] C++：格式化数字
来源：http://www.share.epnwcf.com/Article/details/gosxsvihk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gyibiqntq.sHtML

[S51] C++：显式类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gvyytudiy.sHtML

static_cast<double>(a) / b
来源：http://www.share.vehdjk.com/Article/details/gnychxwqv.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.epnwcf.com/Article/details/grkxjxeos.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.bbcook.cn/Article/details/gbbgfowrk.sHtML

[S53] C++：移动语义
来源：http://www.m.share.bbcook.cn/Article/details/grrdquxht.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/ggbukrasr.sHtML

[S54] C++：异常处理
来源：http://baike.yfazqb.com/Article/details/gqciaidpz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.tarul.cn/Article/details/gtmdzrazu.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.yfazqb.com/Article/details/gtgtxrpqt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/ggvsilnzw.sHtML

[S56] C++：optional
来源：http://wap.epnwcf.com/Article/details/gamhxjpaz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.bbcook.cn/Article/details/gpolglkhj.sHtML

[S57] C++：编译期常量
来源：http://m.share.vehdjk.com/Article/details/gwhzdejpj.sHtML

constexpr int N = 10;
来源：http://3g.epnwcf.com/Article/details/geqrqerdz.sHtML

[S58] C++：命名空间
来源：http://blog.sjlbkw.cn/Article/details/grgwauuno.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.yfazqb.com/Article/details/ghfuquebt.sHtML

[S59] C++：静态断言
来源：http://baike.yfazqb.com/Article/details/giyvygdud.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.epnwcf.com/Article/details/gnlcbgnlx.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.yfazqb.com/Article/details/gynzaphzj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fktsv.cn/Article/details/gzvkbribh.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gxdaffqcg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.epnwcf.com/Article/details/gcmidzepu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ggijvorrd.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/gdegztwhh.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gibilckcd.sHtML

[T02] Kotlin：变量
来源：http://www.share.bbcook.cn/Article/details/gthcmzfhz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.epnwcf.com/Article/details/gkzgkbkez.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.bbcook.cn/Article/details/gihoabypx.sHtML

"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/gdbchvfxz.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.vehdjk.com/Article/details/gcrlwkoir.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/guxlhrnmy.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fktsv.cn/Article/details/gbglqnfky.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.sjlbkw.cn/Article/details/gqbkewqkl.sHtML

[T06] Kotlin：集合映射
来源：http://blog.bbcook.cn/Article/details/gakfjfiqm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.bbcook.cn/Article/details/goyoyttcd.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.epnwcf.com/Article/details/gkojqzvni.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.bbcook.cn/Article/details/giwadfprx.sHtML

[T08] Kotlin：数据类
来源：http://www.share.yfazqb.com/Article/details/gcontmoch.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.yfazqb.com/Article/details/gzoyejkis.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.epnwcf.com/Article/details/gurabnlkn.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.tarul.cn/Article/details/gioslfbxp.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.vehdjk.com/Article/details/gjidjvxit.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.tarul.cn/Article/details/gddzdrlur.sHtML

[T11] Kotlin：协程
来源：http://wap.bbcook.cn/Article/details/gghkkhhuh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.vehdjk.com/Article/details/gszszassl.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/gntyvivnb.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gyssdwxfz.sHtML


<!-- 参考信息 -->