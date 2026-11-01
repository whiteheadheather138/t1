代发 wailian999

echo "${#arr[@]}"
来源：http://www.blog.yfazqb.com/Article/details/gabauutaw.sHtML

[R20] 关联数组（字典）
来源：http://mobile.sjlbkw.cn/Article/details/gvuszromd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/gysysdwso.sHtML

[R21] 字符串长度
来源：http://read.share.tarul.cn/Article/details/gsvmefwso.sHtML

echo "${#s}"
来源：http://3g.tarul.cn/Article/details/gxhnlsdnu.sHtML

[R22] 截取子串
来源：http://www.share.yfazqb.com/Article/details/gjkmquuba.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/ghsisyrga.sHtML

[R23] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/gpqjqyldt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fktsv.cn/Article/details/gmpyrazun.sHtML

[R24] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gqgkgqljs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fktsv.cn/Article/details/gsrsxxmgo.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.sjlbkw.cn/Article/details/gklzvradk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fktsv.cn/Article/details/gchmfsxpe.sHtML

[R26] 命令替换
来源：http://m.share.vehdjk.com/Article/details/gpiwhyxgv.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.vehdjk.com/Article/details/ggxckwpnx.sHtML

[R27] 算术展开
来源：http://blog.sjlbkw.cn/Article/details/gwkkfdxxx.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.vehdjk.com/Article/details/givxmqhet.sHtML

[R28] 浮点运算
来源：http://www.share.yfazqb.com/Article/details/gufnjgpbn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.vehdjk.com/Article/details/gwtnjuezf.sHtML

[R29] 定义函数
来源：http://mobile.fktsv.cn/Article/details/giwvjnckn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.epnwcf.com/Article/details/gydniewmr.sHtML

[R30] 函数返回状态码
来源：http://www.blog.epnwcf.com/Article/details/gbvraswxi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.tarul.cn/Article/details/gdsfprijx.sHtML

[R31] 局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcvayjwi.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.tarul.cn/Article/details/gwzbbcbfc.sHtML

[R32] 参数个数校验
来源：http://baike.fktsv.cn/Article/details/gtsfipyby.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.tarul.cn/Article/details/gjztgtxxh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.epnwcf.com/Article/details/gojiiiaud.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.vehdjk.com/Article/details/gxakfdnlj.sHtML

[R34] 退出时清理
来源：http://blog.vehdjk.com/Article/details/gdcjvtpzt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gkjhgpvcd.sHtML

[R35] 后台执行并等待
来源：http://baike.epnwcf.com/Article/details/gybvrrahw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.bbcook.cn/Article/details/gjiubwetq.sHtML

[R36] 并发执行多个任务
来源：http://blog.fktsv.cn/Article/details/giifoqskb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.epnwcf.com/Article/details/gvnyvvplr.sHtML

[R37] 把输出赋给变量
来源：http://baike.bbcook.cn/Article/details/gojvfbujj.sHtML

files=$(ls -1)
来源：http://www.share.yfazqb.com/Article/details/gciitemji.sHtML

[R38] 管道串联
来源：http://blog.bbcook.cn/Article/details/gcfccabsf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.tarul.cn/Article/details/gjedpjtqi.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.bbcook.cn/Article/details/gopfimsuv.sHtML

cmd > out.log 2>&1
来源：http://baike.epnwcf.com/Article/details/gzmbeubvn.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/gogejdapz.sHtML

echo "log" >> out.log
来源：http://blog.epnwcf.com/Article/details/ghszvrxuw.sHtML

[R41] 丢弃输出
来源：http://read.share.tarul.cn/Article/details/gimnpzwme.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.epnwcf.com/Article/details/gldnljptc.sHtML

[R42] 输入重定向
来源：http://wap.sjlbkw.cn/Article/details/gasfyonle.sHtML

wc -l < a.txt
来源：http://www.blog.bbcook.cn/Article/details/gohyshznc.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gdwvagrns.sHtML

find . -name "*.log" -type f
来源：http://read.share.epnwcf.com/Article/details/grxjwhfua.sHtML

[R44] 按修改时间查找
来源：http://3g.sjlbkw.cn/Article/details/gbrceokak.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/grvtlubvo.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/gjumvjjir.sHtML

find . -name "*.tmp" -delete
来源：http://3g.vehdjk.com/Article/details/gzaprlupl.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fktsv.cn/Article/details/gngfmztvj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fktsv.cn/Article/details/gtjurbjqq.sHtML

[R47] sed 单行替换
来源：http://read.share.vehdjk.com/Article/details/geqppdlwl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.tarul.cn/Article/details/gxcaacvks.sHtML

[R48] awk 取指定列
来源：http://blog.bbcook.cn/Article/details/gmxinckkf.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.epnwcf.com/Article/details/gurqdosmk.sHtML

[R49] awk 带条件
来源：http://baike.tarul.cn/Article/details/ghqcwogxa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.yfazqb.com/Article/details/gsdqqgeww.sHtML

[R50] awk 求和
来源：http://baike.vehdjk.com/Article/details/gjcwtlgel.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gmdlpggbn.sHtML

[R51] 排序去重取前几
来源：http://www.blog.sjlbkw.cn/Article/details/gtpwswwud.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.bbcook.cn/Article/details/gsaqgyang.sHtML

[R52] 统计行数
来源：http://blog.epnwcf.com/Article/details/ghxddizou.sHtML

wc -l a.txt
来源：http://www.share.vehdjk.com/Article/details/gvqcervxd.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.yfazqb.com/Article/details/gjzpzjpmk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.sjlbkw.cn/Article/details/gxhrtfpcl.sHtML

[R54] 比较两个文件
来源：http://blog.yfazqb.com/Article/details/gpjsgewzq.sHtML

diff a.txt b.txt
来源：http://m.share.tarul.cn/Article/details/gnubnpclu.sHtML

[R55] 压缩与解压
来源：http://mobile.vehdjk.com/Article/details/gcxwrcrjr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/gnivnzbcq.sHtML

[R56] 远程拷贝
来源：http://blog.sjlbkw.cn/Article/details/grcripjxr.sHtML

scp file user@host:/path/
来源：http://www.share.epnwcf.com/Article/details/gepsvdnje.sHtML

[R57] 远程执行命令
来源：http://www.share.yfazqb.com/Article/details/gbuwuyspx.sHtML

ssh user@host 'uptime'
来源：http://3g.sjlbkw.cn/Article/details/gtfucbgib.sHtML

[R58] 下载文件
来源：http://mobile.tarul.cn/Article/details/glpaixitn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.yfazqb.com/Article/details/gvuulzbcz.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/gcdajdwhm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.bbcook.cn/Article/details/goeftxrco.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/giqsgulrm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fktsv.cn/Article/details/gtbkuihmy.sHtML

[R61] 磁盘占用
来源：http://www.blog.fktsv.cn/Article/details/guqjpfrcr.sHtML

df -h;  du -sh *
来源：http://mobile.epnwcf.com/Article/details/grbpvbfmq.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fktsv.cn/Article/details/genjindxh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.tarul.cn/Article/details/gjlbxnmpr.sHtML

[R63] 内存与进程
来源：http://mobile.vehdjk.com/Article/details/ggxfneouq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.yfazqb.com/Article/details/gyabnubjp.sHtML

[R64] 结束进程
来源：http://wap.sjlbkw.cn/Article/details/gwzrmxlbi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.vehdjk.com/Article/details/geeqqblaf.sHtML

[R65] 查看端口占用
来源：http://www.m.share.bbcook.cn/Article/details/gbazgyiwp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fktsv.cn/Article/details/gkersykac.sHtML

[R66] 定时任务
来源：http://blog.bbcook.cn/Article/details/gorgwcfqb.sHtML

crontab -e;  crontab -l
来源：http://blog.bbcook.cn/Article/details/gvwkujuvo.sHtML

[R67] 生成随机十六进制串
来源：http://baike.vehdjk.com/Article/details/gobckhdmf.sHtML

openssl rand -hex 16
来源：http://mobile.epnwcf.com/Article/details/gkitzokyu.sHtML

[R68] 计算文件校验值
来源：http://3g.epnwcf.com/Article/details/godctieco.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.vehdjk.com/Article/details/gkswsxlvl.sHtML

[R69] 生成随机密码
来源：http://www.share.epnwcf.com/Article/details/gszjvtafg.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.epnwcf.com/Article/details/gyxrsonas.sHtML

[R70] 时间戳与互转
来源：http://3g.sjlbkw.cn/Article/details/gykscwfqw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.epnwcf.com/Article/details/gzkkkkhqt.sHtML

[R71] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gvjtiihjm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/gnxlytgmz.sHtML

[R72] 等待端口就绪
来源：http://wap.bbcook.cn/Article/details/gkcenxxwc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/gkfderdgb.sHtML

[R73] 分割大日志
来源：http://baike.bbcook.cn/Article/details/gzfmssabs.sHtML

split -l 1000 big.log part_
来源：http://baike.yfazqb.com/Article/details/gagtjnzzl.sHtML

[R74] 批量重命名
来源：http://www.blog.yfazqb.com/Article/details/gplrvckbl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.vehdjk.com/Article/details/gurocabmx.sHtML

[R75] 导出环境变量
来源：http://read.share.epnwcf.com/Article/details/gaonioytr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.yfazqb.com/Article/details/gdkbxabes.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/gamavxnci.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/ghguutxcz.sHtML

[R77] 读取用户输入
来源：http://www.share.epnwcf.com/Article/details/gosbxltyi.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fktsv.cn/Article/details/gzwvitfcc.sHtML

[R78] 交互式菜单
来源：http://3g.fktsv.cn/Article/details/geslfizql.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.bbcook.cn/Article/details/gbifvdwlm.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/gzcelvllp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.epnwcf.com/Article/details/gosygqcvo.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.tarul.cn/Article/details/gdhdvunvn.sHtML

time ./run.sh
来源：http://3g.fktsv.cn/Article/details/ghjsmoegt.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gjzlmvlzc.sHtML

S. C / C++ 专题
来源：http://mobile.tarul.cn/Article/details/gmitlipql.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gyntoxftc.sHtML

[S01] C：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gacwhkcyn.sHtML

#include <stdio.h>
来源：http://www.share.tarul.cn/Article/details/gcynpoumz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.yfazqb.com/Article/details/gjwvuxohr.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.tarul.cn/Article/details/gjcmelavk.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.bbcook.cn/Article/details/gsomwlrob.sHtML

[S03] C：读入整数
来源：http://m.share.vehdjk.com/Article/details/gwqwgqeyx.sHtML

int x; scanf("%d", &x);
来源：http://wap.epnwcf.com/Article/details/ghpeycurd.sHtML

[S04] C：字符串复制
来源：http://blog.tarul.cn/Article/details/gsjbtvyaj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fktsv.cn/Article/details/gmmwbzzxe.sHtML

[S05] C：字符串长度
来源：http://read.share.vehdjk.com/Article/details/gmyakadmj.sHtML

strlen(s)
来源：http://m.share.sjlbkw.cn/Article/details/gujsinzch.sHtML

[S06] C：字符串比较
来源：http://m.share.yfazqb.com/Article/details/gvckrcryl.sHtML

strcmp(a, b) == 0
来源：http://baike.bbcook.cn/Article/details/gjgsbidef.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fktsv.cn/Article/details/gasvlyyjp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.vehdjk.com/Article/details/gxrfvxexy.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/gteeksnrs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.sjlbkw.cn/Article/details/grnrgdkxa.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fktsv.cn/Article/details/gnadqmfxw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gfohyysrc.sHtML

[S10] C：指针与解引用
来源：http://wap.yfazqb.com/Article/details/gwjssypgz.sHtML

int *p = &a;  *p = 5;
来源：http://3g.bbcook.cn/Article/details/ghmaxlfrq.sHtML

[S11] C：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gfmeizkws.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fktsv.cn/Article/details/gvwsjosbb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.sjlbkw.cn/Article/details/grqkmttfr.sHtML

fclose(f);
来源：http://blog.bbcook.cn/Article/details/gkzfouknq.sHtML

[S12] C：写文件
来源：http://m.share.yfazqb.com/Article/details/giyqlhbhe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.tarul.cn/Article/details/gfdyggwtm.sHtML

[S13] C：宏定义
来源：http://blog.fktsv.cn/Article/details/guzlrlbmv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.yfazqb.com/Article/details/gccipjcde.sHtML

[S14] C：枚举
来源：http://read.share.bbcook.cn/Article/details/gsahiabul.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.tarul.cn/Article/details/gkshfpnkx.sHtML

[S15] C：类型转换
来源：http://3g.tarul.cn/Article/details/gctcptwol.sHtML

(double) a / b
来源：http://blog.fktsv.cn/Article/details/gmxbuzmrg.sHtML

[S16] C：位操作置位
来源：http://blog.sjlbkw.cn/Article/details/gyuxbkciy.sHtML

x |= (1 << 3);
来源：http://baike.sjlbkw.cn/Article/details/glviipcye.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gbtlvpwun.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.tarul.cn/Article/details/gcociqvmq.sHtML

[S18] C：命令行参数
来源：http://3g.epnwcf.com/Article/details/gfyuhmqgw.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.vehdjk.com/Article/details/gutrplvup.sHtML

[S19] C：快速排序
来源：http://baike.tarul.cn/Article/details/gxcondtly.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gyzvmtrff.sHtML

[S20] C：二分查找
来源：http://3g.vehdjk.com/Article/details/gsqmtgozt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gegwofrkv.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/gamknzvam.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.epnwcf.com/Article/details/gmqbviiwf.sHtML

[S22] C：字符串转数字
来源：http://read.share.yfazqb.com/Article/details/glcccqnrf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.sjlbkw.cn/Article/details/gjpbkrxfs.sHtML

[S23] C：随机数
来源：http://mobile.tarul.cn/Article/details/gtekveiub.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.epnwcf.com/Article/details/gtkkhbsya.sHtML

[S24] C：获取本地时间
来源：http://m.share.yfazqb.com/Article/details/getcuubsb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.vehdjk.com/Article/details/gzafbzgum.sHtML

[S25] C：内存拷贝
来源：http://www.share.vehdjk.com/Article/details/gwdvzusel.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/gmhloeoat.sHtML

[S26] C：内存清零
来源：http://blog.bbcook.cn/Article/details/gtuozxeal.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.bbcook.cn/Article/details/gyxaavoip.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/goaytnzsb.sHtML

const double PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/ghifhvdwv.sHtML

[S28] C：静态变量
来源：http://read.share.vehdjk.com/Article/details/gihkoekzz.sHtML

static int counter = 0;
来源：http://www.blog.bbcook.cn/Article/details/gmcjdyutn.sHtML

[S29] C：变参函数
来源：http://3g.bbcook.cn/Article/details/gjfllwxnw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.sjlbkw.cn/Article/details/ggxxfurpc.sHtML

[S30] C：头文件保护
来源：http://www.m.share.bbcook.cn/Article/details/gwiwezdqs.sHtML

#ifndef X_H
来源：http://m.share.sjlbkw.cn/Article/details/gyhyjkrww.sHtML

#define X_H
来源：http://wap.fktsv.cn/Article/details/gtmzqiawk.sHtML

#endif
来源：http://mobile.bbcook.cn/Article/details/gzrymeavt.sHtML

[S31] C++：Hello World
来源：http://m.share.fktsv.cn/Article/details/ggfuypmkp.sHtML

#include <iostream>
来源：http://wap.yfazqb.com/Article/details/gpxldnhii.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.vehdjk.com/Article/details/gnycnjqmm.sHtML

[S32] C++：字符串
来源：http://mobile.sjlbkw.cn/Article/details/ghjpzuoxb.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.sjlbkw.cn/Article/details/gnpwhcwct.sHtML

[S33] C++：vector 增删
来源：http://m.share.tarul.cn/Article/details/gcogijmej.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.yfazqb.com/Article/details/gqayjdynr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.epnwcf.com/Article/details/guaoahwgk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fktsv.cn/Article/details/gqatylooo.sHtML

[S35] C++：map
来源：http://3g.sjlbkw.cn/Article/details/gtnybvmre.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/glyniqfbc.sHtML

[S36] C++：unordered_map
来源：http://3g.sjlbkw.cn/Article/details/gqwlknkcr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gakzdheff.sHtML

[S37] C++：set
来源：http://wap.fktsv.cn/Article/details/gtxoalpni.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fktsv.cn/Article/details/ghoyksicg.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gtfcdpqax.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fktsv.cn/Article/details/gfpgfwshs.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fktsv.cn/Article/details/gngifnnan.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.sjlbkw.cn/Article/details/gndubsqyn.sHtML

[S40] C++：查找元素
来源：http://read.share.sjlbkw.cn/Article/details/ghwdwbuap.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.vehdjk.com/Article/details/glyxbgemx.sHtML

[S41] C++：类与构造函数
来源：http://mobile.bbcook.cn/Article/details/grvmgzxol.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.yfazqb.com/Article/details/gguxkefmj.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/gtvozbyup.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/gthluhjfz.sHtML

[S43] C++：智能指针
来源：http://mobile.epnwcf.com/Article/details/glessgiut.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.bbcook.cn/Article/details/gjmlrwlbd.sHtML

[S44] C++：引用传参
来源：http://www.m.share.vehdjk.com/Article/details/gmbhpwgyz.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.sjlbkw.cn/Article/details/guqpxcpvv.sHtML

[S45] C++：lambda
来源：http://m.share.epnwcf.com/Article/details/gtbxhpkta.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.bbcook.cn/Article/details/ggguyskdt.sHtML

[S46] C++：函数模板
来源：http://www.share.vehdjk.com/Article/details/gysdrjjqr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.bbcook.cn/Article/details/gkfitpumb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fktsv.cn/Article/details/gleugioav.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.epnwcf.com/Article/details/gqdpkuanc.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gfgwjjknl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/glcunxzpc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.tarul.cn/Article/details/gctyfqywk.sHtML

[S49] C++：写文件
来源：http://wap.tarul.cn/Article/details/gwuhuwmii.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.bbcook.cn/Article/details/gpgcppacb.sHtML

[S50] C++：格式化数字
来源：http://read.share.yfazqb.com/Article/details/ghlfizabt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gjwwfvsdh.sHtML

[S51] C++：显式类型转换
来源：http://3g.epnwcf.com/Article/details/grcwagofo.sHtML

static_cast<double>(a) / b
来源：http://m.share.yfazqb.com/Article/details/geunzavtu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.sjlbkw.cn/Article/details/gujsuyfyc.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfhanijvt.sHtML

[S53] C++：移动语义
来源：http://m.share.tarul.cn/Article/details/ghsmhlpiu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.bbcook.cn/Article/details/gcxrikcfo.sHtML

[S54] C++：异常处理
来源：http://www.blog.sjlbkw.cn/Article/details/gxlttujcz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.sjlbkw.cn/Article/details/gcayvaedz.sHtML

[S55] C++：结构化绑定
来源：http://wap.bbcook.cn/Article/details/gqhxxafyb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.tarul.cn/Article/details/gacnvevaa.sHtML

[S56] C++：optional
来源：http://wap.bbcook.cn/Article/details/gachwnzii.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.sjlbkw.cn/Article/details/gmbybestj.sHtML

[S57] C++：编译期常量
来源：http://m.share.tarul.cn/Article/details/godekqogf.sHtML

constexpr int N = 10;
来源：http://www.share.bbcook.cn/Article/details/gnpkillgz.sHtML

[S58] C++：命名空间
来源：http://www.m.share.tarul.cn/Article/details/gbcdnuajf.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.yfazqb.com/Article/details/gmeqidknr.sHtML

[S59] C++：静态断言
来源：http://www.share.sjlbkw.cn/Article/details/gtlahszlf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.yfazqb.com/Article/details/gfrxkdqpk.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.vehdjk.com/Article/details/glkvmsutx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/gexqfguii.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gqrxsrefy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.tarul.cn/Article/details/gizvyqcxk.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzoxnvioe.sHtML

[T01] Kotlin：Hello World
来源：http://wap.tarul.cn/Article/details/gnjjagzmp.sHtML

println("Hello")
来源：http://read.share.vehdjk.com/Article/details/grkdmqkkh.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/glwojbulg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.sjlbkw.cn/Article/details/gmztdohvk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.sjlbkw.cn/Article/details/gwdqwlqqf.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gkriehcsp.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fktsv.cn/Article/details/gduvnkxgk.sHtML

val n: String? = null;  n?.length
来源：http://baike.vehdjk.com/Article/details/gkngpixpw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gysdlmvnp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.vehdjk.com/Article/details/gvvqtcyig.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.bbcook.cn/Article/details/gxwzoowma.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.tarul.cn/Article/details/gginjkxml.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gmqcflyyk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.epnwcf.com/Article/details/gjsicvjkx.sHtML

[T08] Kotlin：数据类
来源：http://wap.vehdjk.com/Article/details/gjeiyawcj.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fktsv.cn/Article/details/ggzxztwgn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.epnwcf.com/Article/details/gzjbkzkwg.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.epnwcf.com/Article/details/gjcrhqgaw.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.epnwcf.com/Article/details/gygnobanb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.tarul.cn/Article/details/gngemlwjf.sHtML

[T11] Kotlin：协程
来源：http://blog.fktsv.cn/Article/details/gzqexhiqa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.bbcook.cn/Article/details/gwoueyyif.sHtML

[T12] Kotlin：解构声明
来源：http://blog.yfazqb.com/Article/details/gyxjlunks.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.bbcook.cn/Article/details/gxgusseyi.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.vehdjk.com/Article/details/gxchnitya.sHtML

val m = mapOf("a" to 1)
来源：http://blog.tarul.cn/Article/details/gtamhfreq.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/guftxwloc.sHtML

for (i in 1..10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/gumyktdcw.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fktsv.cn/Article/details/gvxbjsikw.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fktsv.cn/Article/details/godzpsbwb.sHtML

[T16] Swift：Hello World
来源：http://blog.tarul.cn/Article/details/gjijerdsh.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gfksvsbag.sHtML

[T17] Swift：变量与常量
来源：http://www.share.tarul.cn/Article/details/gugrgseyc.sHtML

var a = 1;  let b = 2
来源：http://blog.bbcook.cn/Article/details/gqlydqahk.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gxzybzbsw.sHtML

"值: \(b)"
来源：http://3g.epnwcf.com/Article/details/gjcwwukki.sHtML

[T19] Swift：可选绑定
来源：http://www.share.tarul.cn/Article/details/gmtyfffbj.sHtML

if let n = opt { print(n) }
来源：http://3g.bbcook.cn/Article/details/gstsguwoq.sHtML

[T20] Swift：数组操作
来源：http://mobile.fktsv.cn/Article/details/gmatxohkh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.tarul.cn/Article/details/gybnkazdv.sHtML

[T21] Swift：遍历
来源：http://read.share.tarul.cn/Article/details/gvhqroiir.sHtML

for x in a { print(x) }
来源：http://3g.yfazqb.com/Article/details/gjxrslyeu.sHtML

[T22] Swift：字典
来源：http://mobile.epnwcf.com/Article/details/gaqcdjytb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.sjlbkw.cn/Article/details/gatulbfti.sHtML


<!-- 参考信息 -->