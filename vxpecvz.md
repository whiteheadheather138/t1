代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.tarul.cn/Article/details/gajgyidtf.sHtML

[R10] 正则匹配
来源：http://blog.tarul.cn/Article/details/gnwjndfmu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fktsv.cn/Article/details/gcemotbts.sHtML

[R11] case 多分支
来源：http://3g.epnwcf.com/Article/details/gqdnpnidd.sHtML

case "$1" in
来源：http://www.m.share.bbcook.cn/Article/details/gfybyswxy.sHtML

start) echo "启动" ;;
来源：http://3g.fktsv.cn/Article/details/gigecqfiu.sHtML

stop)  echo "停止" ;;
来源：http://baike.vehdjk.com/Article/details/gehkunhyr.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.epnwcf.com/Article/details/glroxummz.sHtML

esac
来源：http://wap.sjlbkw.cn/Article/details/gbwjkyveo.sHtML

[R12] for 遍历文件
来源：http://wap.yfazqb.com/Article/details/gfcjrhltc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.sjlbkw.cn/Article/details/gekarqbju.sHtML

[R13] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gyejdbuyq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.tarul.cn/Article/details/gmcnxebbj.sHtML

[R14] C 风格 for
来源：http://www.share.tarul.cn/Article/details/ghivuxfhb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.bbcook.cn/Article/details/gkjkqtabz.sHtML

[R15] while 逐行读文件
来源：http://wap.vehdjk.com/Article/details/gdyrhoqkr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.yfazqb.com/Article/details/gbovgndfd.sHtML

[R16] until 等待条件
来源：http://wap.epnwcf.com/Article/details/gepzzmdcm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gnitxbdns.sHtML

[R17] 数组定义与取值
来源：http://www.blog.bbcook.cn/Article/details/gbebvjuuo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.epnwcf.com/Article/details/galekujhx.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/gjbmilyxj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.epnwcf.com/Article/details/gccprqcyy.sHtML

[R19] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/ggzcgikbi.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fktsv.cn/Article/details/gyzjvobiz.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.yfazqb.com/Article/details/gcantndpu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.yfazqb.com/Article/details/grkfgexub.sHtML

[R21] 字符串长度
来源：http://m.share.fktsv.cn/Article/details/gmhfeputi.sHtML

echo "${#s}"
来源：http://m.share.sjlbkw.cn/Article/details/guicgthjl.sHtML

[R22] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/gijncnagu.sHtML

echo "${s:0:5}"
来源：http://www.share.yfazqb.com/Article/details/gpoxgkkag.sHtML

[R23] 字符串替换
来源：http://blog.yfazqb.com/Article/details/gqtulpgip.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.bbcook.cn/Article/details/gydtpfarm.sHtML

[R24] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gztnilxqv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.sjlbkw.cn/Article/details/gbwmexfwv.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.yfazqb.com/Article/details/gpwkqdbag.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.yfazqb.com/Article/details/gflcfsmje.sHtML

[R26] 命令替换
来源：http://read.share.tarul.cn/Article/details/gwknrryop.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.bbcook.cn/Article/details/giajoowqy.sHtML

[R27] 算术展开
来源：http://www.m.share.yfazqb.com/Article/details/gvxpnfego.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.vehdjk.com/Article/details/gwvpdbplz.sHtML

[R28] 浮点运算
来源：http://blog.tarul.cn/Article/details/gopynjnnl.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.tarul.cn/Article/details/gnujtgqlx.sHtML

[R29] 定义函数
来源：http://baike.fktsv.cn/Article/details/gxqkmeldz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fktsv.cn/Article/details/gblmwgrdb.sHtML

[R30] 函数返回状态码
来源：http://mobile.bbcook.cn/Article/details/gedjtxsey.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.epnwcf.com/Article/details/gmgqulnsz.sHtML

[R31] 局部变量
来源：http://blog.yfazqb.com/Article/details/ghuyduiby.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.yfazqb.com/Article/details/gyjgzidcc.sHtML

[R32] 参数个数校验
来源：http://m.share.bbcook.cn/Article/details/gmkklavgw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gbqpqqgeh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.vehdjk.com/Article/details/gzjbjwwcb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.vehdjk.com/Article/details/gawtxoejq.sHtML

[R34] 退出时清理
来源：http://blog.yfazqb.com/Article/details/gdpptdqdx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/gxpgxusul.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/grsfvgriv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.epnwcf.com/Article/details/gmdkieiun.sHtML

[R36] 并发执行多个任务
来源：http://3g.tarul.cn/Article/details/gnqtukhhu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.sjlbkw.cn/Article/details/gjkxlnkcc.sHtML

[R37] 把输出赋给变量
来源：http://m.share.tarul.cn/Article/details/gtpgwsjhz.sHtML

files=$(ls -1)
来源：http://mobile.tarul.cn/Article/details/gemqcmdgs.sHtML

[R38] 管道串联
来源：http://baike.epnwcf.com/Article/details/gmmvszzif.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fktsv.cn/Article/details/gcdegzzsv.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.bbcook.cn/Article/details/gygowrwla.sHtML

cmd > out.log 2>&1
来源：http://m.share.fktsv.cn/Article/details/gotzacnru.sHtML

[R40] 追加写日志
来源：http://wap.sjlbkw.cn/Article/details/gatczwzzu.sHtML

echo "log" >> out.log
来源：http://www.share.bbcook.cn/Article/details/gfnplffok.sHtML

[R41] 丢弃输出
来源：http://mobile.sjlbkw.cn/Article/details/gelzwtdrr.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.yfazqb.com/Article/details/guqxddbne.sHtML

[R42] 输入重定向
来源：http://wap.sjlbkw.cn/Article/details/gtzovfdqc.sHtML

wc -l < a.txt
来源：http://mobile.yfazqb.com/Article/details/gdavuropo.sHtML

[R43] 按名字查找文件
来源：http://www.share.sjlbkw.cn/Article/details/gnjtyjbll.sHtML

find . -name "*.log" -type f
来源：http://wap.sjlbkw.cn/Article/details/gttqsmawy.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.vehdjk.com/Article/details/gjtzuhzqh.sHtML

find . -mtime -7 -type f
来源：http://m.share.tarul.cn/Article/details/gxbhrzukf.sHtML

[R45] 批量删除
来源：http://m.share.yfazqb.com/Article/details/gscmhiyaz.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.tarul.cn/Article/details/gzsnzqnop.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.bbcook.cn/Article/details/gqzbqqbqs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fktsv.cn/Article/details/gydkvcnpy.sHtML

[R47] sed 单行替换
来源：http://3g.epnwcf.com/Article/details/gvovypold.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.yfazqb.com/Article/details/gzyxjayjq.sHtML

[R48] awk 取指定列
来源：http://3g.yfazqb.com/Article/details/gciizodxx.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.vehdjk.com/Article/details/gcrozsbmn.sHtML

[R49] awk 带条件
来源：http://mobile.sjlbkw.cn/Article/details/ghbncogsr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.bbcook.cn/Article/details/ghafbekrb.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/gsenioill.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.yfazqb.com/Article/details/gnzizxjvn.sHtML

[R51] 排序去重取前几
来源：http://www.share.fktsv.cn/Article/details/geszapbxz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.sjlbkw.cn/Article/details/gpvfogmly.sHtML

[R52] 统计行数
来源：http://mobile.sjlbkw.cn/Article/details/gjsfepuqh.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/gnjqgltwe.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.vehdjk.com/Article/details/ghvpqourr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.yfazqb.com/Article/details/gwevhcvpe.sHtML

[R54] 比较两个文件
来源：http://www.share.tarul.cn/Article/details/gzjllwuvt.sHtML

diff a.txt b.txt
来源：http://www.blog.epnwcf.com/Article/details/gelzeiryj.sHtML

[R55] 压缩与解压
来源：http://wap.epnwcf.com/Article/details/gbypnvfcq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.yfazqb.com/Article/details/gehlxpzvv.sHtML

[R56] 远程拷贝
来源：http://www.share.epnwcf.com/Article/details/gffawljll.sHtML

scp file user@host:/path/
来源：http://read.share.yfazqb.com/Article/details/gidmhxdxw.sHtML

[R57] 远程执行命令
来源：http://read.share.bbcook.cn/Article/details/gpqlswmcl.sHtML

ssh user@host 'uptime'
来源：http://baike.epnwcf.com/Article/details/glxcjilrj.sHtML

[R58] 下载文件
来源：http://wap.bbcook.cn/Article/details/gqnurxxam.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.vehdjk.com/Article/details/ggxidzmsq.sHtML

[R59] 发 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/gjnxpdugo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/gclysokmz.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/ggaltnvsk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.vehdjk.com/Article/details/gxbztmmnu.sHtML

[R61] 磁盘占用
来源：http://www.m.share.yfazqb.com/Article/details/gqwnniceh.sHtML

df -h;  du -sh *
来源：http://blog.tarul.cn/Article/details/gtabskuob.sHtML

[R62] 找最占空间的文件
来源：http://m.share.sjlbkw.cn/Article/details/gmkwhgdhr.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.yfazqb.com/Article/details/gjktwcxti.sHtML

[R63] 内存与进程
来源：http://3g.tarul.cn/Article/details/gpmhemgsj.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.bbcook.cn/Article/details/gzmmpjnep.sHtML

[R64] 结束进程
来源：http://wap.yfazqb.com/Article/details/gojqlmtnd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.yfazqb.com/Article/details/gniatfska.sHtML

[R65] 查看端口占用
来源：http://wap.fktsv.cn/Article/details/gpijpdbjx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.yfazqb.com/Article/details/giqgxyzcj.sHtML

[R66] 定时任务
来源：http://3g.yfazqb.com/Article/details/gjqdqkwvb.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/gcemvkjob.sHtML

[R67] 生成随机十六进制串
来源：http://baike.bbcook.cn/Article/details/glcldwbuz.sHtML

openssl rand -hex 16
来源：http://mobile.sjlbkw.cn/Article/details/gtbfhwmsn.sHtML

[R68] 计算文件校验值
来源：http://mobile.tarul.cn/Article/details/gedljzdrb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.epnwcf.com/Article/details/giklxdlbt.sHtML

[R69] 生成随机密码
来源：http://www.blog.vehdjk.com/Article/details/guzkmpfch.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.epnwcf.com/Article/details/gigkststi.sHtML

[R70] 时间戳与互转
来源：http://www.share.epnwcf.com/Article/details/gauwdtock.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.yfazqb.com/Article/details/grezxklhq.sHtML

[R71] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gwduzeqce.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.bbcook.cn/Article/details/glhomqvyk.sHtML

[R72] 等待端口就绪
来源：http://baike.tarul.cn/Article/details/gvbfaxair.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/grnoktjwn.sHtML

[R73] 分割大日志
来源：http://mobile.tarul.cn/Article/details/gyxagspqx.sHtML

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/ghzveatxt.sHtML

[R74] 批量重命名
来源：http://mobile.sjlbkw.cn/Article/details/gjinusqpo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fktsv.cn/Article/details/gjfrsxkmp.sHtML

[R75] 导出环境变量
来源：http://blog.sjlbkw.cn/Article/details/gfdsrtxoe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.tarul.cn/Article/details/goajmijyf.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/gbeenxqon.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.bbcook.cn/Article/details/gpejadptk.sHtML

[R77] 读取用户输入
来源：http://www.blog.bbcook.cn/Article/details/ghnoalngu.sHtML

read -rp "请输入: " ans
来源：http://read.share.tarul.cn/Article/details/gkhguzdsm.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/gbvzpvtbs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.tarul.cn/Article/details/gidbyftpt.sHtML

[R79] 解析命令行选项
来源：http://baike.bbcook.cn/Article/details/gzcjxjorc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/gpbsxwznx.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.epnwcf.com/Article/details/gczhprlpz.sHtML

time ./run.sh
来源：http://wap.bbcook.cn/Article/details/gipfdugye.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gknayhpgg.sHtML

S. C / C++ 专题
来源：http://blog.fktsv.cn/Article/details/gywoszjcn.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtyggqafo.sHtML

[S01] C：Hello World
来源：http://3g.fktsv.cn/Article/details/gfurnoqok.sHtML

#include <stdio.h>
来源：http://m.share.yfazqb.com/Article/details/gcpnmtaqp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.epnwcf.com/Article/details/gbovgrjcv.sHtML

[S02] C：变量与格式化输出
来源：http://wap.yfazqb.com/Article/details/gdhfikpme.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/gkumfochb.sHtML

[S03] C：读入整数
来源：http://wap.sjlbkw.cn/Article/details/gitihavqr.sHtML

int x; scanf("%d", &x);
来源：http://mobile.yfazqb.com/Article/details/gpybeyddq.sHtML

[S04] C：字符串复制
来源：http://wap.bbcook.cn/Article/details/ghucixmdf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.vehdjk.com/Article/details/gpvyskbae.sHtML

[S05] C：字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gkflssvaa.sHtML

strlen(s)
来源：http://mobile.epnwcf.com/Article/details/gcxdvdezy.sHtML

[S06] C：字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gktlcjetf.sHtML

strcmp(a, b) == 0
来源：http://m.share.yfazqb.com/Article/details/gzoblfcow.sHtML

[S07] C：数组遍历求和
来源：http://www.share.vehdjk.com/Article/details/gkbogkjax.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.sjlbkw.cn/Article/details/gfvqzpnbq.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fktsv.cn/Article/details/gvqpchyzs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.sjlbkw.cn/Article/details/gwirgdtfx.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/gkhbwhyxv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.vehdjk.com/Article/details/gtjifoiwo.sHtML

[S10] C：指针与解引用
来源：http://mobile.tarul.cn/Article/details/gczaotevm.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.bbcook.cn/Article/details/ggfrfgkph.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/grfseejud.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.vehdjk.com/Article/details/gpvvirkfp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fktsv.cn/Article/details/gfprfsvzy.sHtML

fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/gawapsmwl.sHtML

[S12] C：写文件
来源：http://blog.vehdjk.com/Article/details/grniygvhb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fktsv.cn/Article/details/gugawuhfr.sHtML

[S13] C：宏定义
来源：http://3g.bbcook.cn/Article/details/gzuiqxlhp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.tarul.cn/Article/details/gkiuaznus.sHtML

[S14] C：枚举
来源：http://blog.sjlbkw.cn/Article/details/gxlosidfv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.yfazqb.com/Article/details/gliollebw.sHtML

[S15] C：类型转换
来源：http://wap.bbcook.cn/Article/details/gmtovsjys.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdwxjojk.sHtML

[S16] C：位操作置位
来源：http://www.m.share.yfazqb.com/Article/details/gautelnda.sHtML

x |= (1 << 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhymsshy.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gfcveripz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.tarul.cn/Article/details/gazuckqqd.sHtML

[S18] C：命令行参数
来源：http://blog.tarul.cn/Article/details/gyfplzvzu.sHtML

int main(int argc, char **argv)
来源：http://read.share.fktsv.cn/Article/details/gmlkxqiht.sHtML

[S19] C：快速排序
来源：http://m.share.yfazqb.com/Article/details/gdrcsuozk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gliaysojm.sHtML

[S20] C：二分查找
来源：http://blog.fktsv.cn/Article/details/gsouycwpc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/ghfzhzexh.sHtML

[S21] C：字符类别判断
来源：http://3g.fktsv.cn/Article/details/gtbjrpeko.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.yfazqb.com/Article/details/gtpkszymt.sHtML

[S22] C：字符串转数字
来源：http://3g.vehdjk.com/Article/details/gwcxmahji.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.epnwcf.com/Article/details/ggitlcffy.sHtML

[S23] C：随机数
来源：http://m.share.sjlbkw.cn/Article/details/gwnvmupbq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.vehdjk.com/Article/details/gkfleakwg.sHtML

[S24] C：获取本地时间
来源：http://mobile.tarul.cn/Article/details/gafbtrbmu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.tarul.cn/Article/details/ggrgvmmrk.sHtML

[S25] C：内存拷贝
来源：http://blog.epnwcf.com/Article/details/ghjdctqdt.sHtML

memcpy(dst, src, n);
来源：http://www.blog.epnwcf.com/Article/details/gqwhulghn.sHtML

[S26] C：内存清零
来源：http://www.blog.epnwcf.com/Article/details/gfalljylo.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/gjhzlnqpz.sHtML

[S27] C：定义常量
来源：http://wap.sjlbkw.cn/Article/details/gxlnsvpuq.sHtML

const double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gajobekal.sHtML

[S28] C：静态变量
来源：http://baike.vehdjk.com/Article/details/glfxusqta.sHtML

static int counter = 0;
来源：http://mobile.sjlbkw.cn/Article/details/gbluirgbv.sHtML

[S29] C：变参函数
来源：http://www.blog.fktsv.cn/Article/details/gzedlhrld.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.vehdjk.com/Article/details/glxcqbaeh.sHtML

[S30] C：头文件保护
来源：http://www.share.epnwcf.com/Article/details/gooukrxyn.sHtML

#ifndef X_H
来源：http://www.share.tarul.cn/Article/details/gwsehwluz.sHtML

#define X_H
来源：http://www.share.bbcook.cn/Article/details/gvoiifors.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/gbledzztq.sHtML

[S31] C++：Hello World
来源：http://blog.vehdjk.com/Article/details/gcbgbtlcu.sHtML

#include <iostream>
来源：http://www.m.share.epnwcf.com/Article/details/gczkhuxnb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.bbcook.cn/Article/details/gdngzwmuf.sHtML

[S32] C++：字符串
来源：http://blog.vehdjk.com/Article/details/gkisbjlor.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/gwwlkjhho.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.vehdjk.com/Article/details/grztfvbvy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.yfazqb.com/Article/details/gapjclhyk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/gqzqzvseh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.yfazqb.com/Article/details/glzriipqf.sHtML

[S35] C++：map
来源：http://mobile.vehdjk.com/Article/details/gnjaepaol.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/ggylqxoud.sHtML

[S36] C++：unordered_map
来源：http://wap.yfazqb.com/Article/details/gfnwdeznp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gdljftoop.sHtML

[S37] C++：set
来源：http://mobile.sjlbkw.cn/Article/details/glpgxpera.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/gsivzufbb.sHtML

[S38] C++：排序
来源：http://baike.fktsv.cn/Article/details/gvljporde.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.yfazqb.com/Article/details/ghlubamyq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.vehdjk.com/Article/details/grehdzskj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.epnwcf.com/Article/details/gyysvlcew.sHtML

[S40] C++：查找元素
来源：http://baike.yfazqb.com/Article/details/gtgslanlz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.vehdjk.com/Article/details/gvjteewpx.sHtML

[S41] C++：类与构造函数
来源：http://m.share.tarul.cn/Article/details/gdydrffcn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.epnwcf.com/Article/details/gqnqhueql.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.bbcook.cn/Article/details/gmcexkezw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.tarul.cn/Article/details/gkhujbvny.sHtML

[S43] C++：智能指针
来源：http://wap.epnwcf.com/Article/details/gjzqkpuvq.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/gzvghwjxl.sHtML

[S44] C++：引用传参
来源：http://www.blog.bbcook.cn/Article/details/geznlerjc.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/gxqziwbvq.sHtML

[S45] C++：lambda
来源：http://m.share.bbcook.cn/Article/details/gqwheinea.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.bbcook.cn/Article/details/gakfceiee.sHtML

[S46] C++：函数模板
来源：http://baike.yfazqb.com/Article/details/gczmqvrnw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.tarul.cn/Article/details/gykcmungl.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.tarul.cn/Article/details/graisarxr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.vehdjk.com/Article/details/gxppiqcnb.sHtML

[S48] C++：逐行读文件
来源：http://baike.tarul.cn/Article/details/gschgtqag.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fktsv.cn/Article/details/gdwhpdbbo.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.bbcook.cn/Article/details/gusgakpod.sHtML

[S49] C++：写文件
来源：http://www.share.sjlbkw.cn/Article/details/gmjgouzsq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.vehdjk.com/Article/details/gpelkhlme.sHtML

[S50] C++：格式化数字
来源：http://baike.tarul.cn/Article/details/gqwwjvjtv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/gjudxkmeu.sHtML

[S51] C++：显式类型转换
来源：http://www.share.vehdjk.com/Article/details/gessltgov.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.tarul.cn/Article/details/ggsqtcjku.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fktsv.cn/Article/details/gjatgurbt.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.sjlbkw.cn/Article/details/gykhnjrmm.sHtML

[S53] C++：移动语义
来源：http://wap.fktsv.cn/Article/details/gqgamscvh.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.bbcook.cn/Article/details/gcmnfckkr.sHtML

[S54] C++：异常处理
来源：http://blog.bbcook.cn/Article/details/giceudqtp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.tarul.cn/Article/details/gbrxcrcwj.sHtML

[S55] C++：结构化绑定
来源：http://www.share.bbcook.cn/Article/details/gqkwhoevs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.vehdjk.com/Article/details/gcafkyxih.sHtML

[S56] C++：optional
来源：http://wap.epnwcf.com/Article/details/gotxqdjgn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.tarul.cn/Article/details/grfopipux.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.epnwcf.com/Article/details/gttvuwjtu.sHtML

constexpr int N = 10;
来源：http://m.share.epnwcf.com/Article/details/gjyasdhnu.sHtML

[S58] C++：命名空间
来源：http://m.share.tarul.cn/Article/details/gqalhkwko.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.vehdjk.com/Article/details/gbfoeucqf.sHtML

[S59] C++：静态断言
来源：http://3g.sjlbkw.cn/Article/details/gqsfrvwau.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.sjlbkw.cn/Article/details/gxacqulsb.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.vehdjk.com/Article/details/gphsvkept.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fktsv.cn/Article/details/gtizdjdhh.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/guiiosqam.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.tarul.cn/Article/details/guywxjvyz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gvpgvauik.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gkqiolzrs.sHtML

println("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwyqsygr.sHtML

[T02] Kotlin：变量
来源：http://www.blog.epnwcf.com/Article/details/gbcaowpbn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.sjlbkw.cn/Article/details/gdffhigej.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.sjlbkw.cn/Article/details/gnomrfcpl.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/gcaqwkmve.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.bbcook.cn/Article/details/gauorigqz.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/gmkqaogiq.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.vehdjk.com/Article/details/gurojlljy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.yfazqb.com/Article/details/gsbsdhxqd.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/ggtiryvwx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gvaldzfco.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.bbcook.cn/Article/details/gldsfrjng.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.vehdjk.com/Article/details/gzudbdadw.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.vehdjk.com/Article/details/gwgrxcapg.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.epnwcf.com/Article/details/gosemfdyt.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.yfazqb.com/Article/details/gjmuqiinn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcktuhvt.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fktsv.cn/Article/details/gngasvomt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gtnzpowlk.sHtML


<!-- 参考信息 -->