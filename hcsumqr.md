代发 wailian999

echo "${#arr[@]}"
来源：http://read.share.epnwcf.com/Article/details/gwcfdxrnr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fktsv.cn/Article/details/gifbfxgwd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvzhowkn.sHtML

[R21] 字符串长度
来源：http://m.share.bbcook.cn/Article/details/gbehbsgce.sHtML

echo "${#s}"
来源：http://read.share.sjlbkw.cn/Article/details/gkkbradqm.sHtML

[R22] 截取子串
来源：http://blog.yfazqb.com/Article/details/gctcmjfgp.sHtML

echo "${s:0:5}"
来源：http://www.blog.fktsv.cn/Article/details/gbrrirphp.sHtML

[R23] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/guusqsqze.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.yfazqb.com/Article/details/gysfbwnif.sHtML

[R24] 大小写转换
来源：http://blog.bbcook.cn/Article/details/glvdvlzge.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.sjlbkw.cn/Article/details/gldomhmos.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.tarul.cn/Article/details/gnqieaypx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.sjlbkw.cn/Article/details/gajwtkltr.sHtML

[R26] 命令替换
来源：http://baike.sjlbkw.cn/Article/details/ggxapqkqb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fktsv.cn/Article/details/gjrfgdvnc.sHtML

[R27] 算术展开
来源：http://baike.epnwcf.com/Article/details/gislpxghd.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.sjlbkw.cn/Article/details/gsrfhdbyj.sHtML

[R28] 浮点运算
来源：http://baike.epnwcf.com/Article/details/gdkuattfq.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.yfazqb.com/Article/details/gjnwdyouh.sHtML

[R29] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gkqkvoyff.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.sjlbkw.cn/Article/details/gvpixuwla.sHtML

[R30] 函数返回状态码
来源：http://www.share.vehdjk.com/Article/details/ghfnlqafz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.bbcook.cn/Article/details/ggriygnpr.sHtML

[R31] 局部变量
来源：http://baike.vehdjk.com/Article/details/gbjygvrlu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.bbcook.cn/Article/details/gcvjolqpe.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fktsv.cn/Article/details/gbyqqutkv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/gluekvhgw.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.vehdjk.com/Article/details/gtqsvwkra.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.yfazqb.com/Article/details/gqtfuyjcr.sHtML

[R34] 退出时清理
来源：http://mobile.yfazqb.com/Article/details/gwervaeop.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.sjlbkw.cn/Article/details/gvbbtijvz.sHtML

[R35] 后台执行并等待
来源：http://wap.vehdjk.com/Article/details/gbicjrofh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.epnwcf.com/Article/details/gxditdiid.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/gltkhdniy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fktsv.cn/Article/details/gmvegwqra.sHtML

[R37] 把输出赋给变量
来源：http://blog.vehdjk.com/Article/details/gzmwljiic.sHtML

files=$(ls -1)
来源：http://www.share.yfazqb.com/Article/details/ggeydswtf.sHtML

[R38] 管道串联
来源：http://baike.fktsv.cn/Article/details/giuuriioy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.vehdjk.com/Article/details/ggnvfxrnm.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.yfazqb.com/Article/details/gzwxpwgmj.sHtML

cmd > out.log 2>&1
来源：http://mobile.fktsv.cn/Article/details/gjeoscwem.sHtML

[R40] 追加写日志
来源：http://blog.fktsv.cn/Article/details/gtrnfiolo.sHtML

echo "log" >> out.log
来源：http://blog.yfazqb.com/Article/details/gehxsknit.sHtML

[R41] 丢弃输出
来源：http://blog.yfazqb.com/Article/details/gtnomcfzo.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.vehdjk.com/Article/details/gwuulverd.sHtML

[R42] 输入重定向
来源：http://www.blog.bbcook.cn/Article/details/gkzfhxzye.sHtML

wc -l < a.txt
来源：http://baike.tarul.cn/Article/details/gghooxoxs.sHtML

[R43] 按名字查找文件
来源：http://read.share.tarul.cn/Article/details/gtsyfcasn.sHtML

find . -name "*.log" -type f
来源：http://mobile.yfazqb.com/Article/details/gztpkwvyo.sHtML

[R44] 按修改时间查找
来源：http://read.share.tarul.cn/Article/details/googzknqb.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.yfazqb.com/Article/details/gbxufwadj.sHtML

[R45] 批量删除
来源：http://www.m.share.vehdjk.com/Article/details/geibdjesn.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fktsv.cn/Article/details/gkhtubwxg.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.tarul.cn/Article/details/ghmwmotbn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.sjlbkw.cn/Article/details/gjabzvidq.sHtML

[R47] sed 单行替换
来源：http://mobile.vehdjk.com/Article/details/gxdctjspj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.epnwcf.com/Article/details/gkovguhka.sHtML

[R48] awk 取指定列
来源：http://baike.bbcook.cn/Article/details/gppwepauv.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.epnwcf.com/Article/details/gmcfxtzsd.sHtML

[R49] awk 带条件
来源：http://www.share.vehdjk.com/Article/details/gautsedyf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.epnwcf.com/Article/details/gpuwsapyl.sHtML

[R50] awk 求和
来源：http://baike.tarul.cn/Article/details/gsoocfqva.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/goozfgaiv.sHtML

[R51] 排序去重取前几
来源：http://www.blog.epnwcf.com/Article/details/giknkgjmt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.vehdjk.com/Article/details/gqfcfnvda.sHtML

[R52] 统计行数
来源：http://baike.vehdjk.com/Article/details/gmbohdkze.sHtML

wc -l a.txt
来源：http://baike.tarul.cn/Article/details/gvujzirlx.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.bbcook.cn/Article/details/ggdjtnwme.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/glrqsgpih.sHtML

[R54] 比较两个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gbaiackqk.sHtML

diff a.txt b.txt
来源：http://baike.bbcook.cn/Article/details/guxcirthm.sHtML

[R55] 压缩与解压
来源：http://wap.epnwcf.com/Article/details/gadsgfrdu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fktsv.cn/Article/details/galavsrvb.sHtML

[R56] 远程拷贝
来源：http://wap.yfazqb.com/Article/details/gassvqflk.sHtML

scp file user@host:/path/
来源：http://3g.epnwcf.com/Article/details/gwsivavfl.sHtML

[R57] 远程执行命令
来源：http://mobile.tarul.cn/Article/details/gyglqilvn.sHtML

ssh user@host 'uptime'
来源：http://read.share.fktsv.cn/Article/details/gzccubtvk.sHtML

[R58] 下载文件
来源：http://baike.vehdjk.com/Article/details/gscinemro.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.tarul.cn/Article/details/gsjgitjyd.sHtML

[R59] 发 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gxujpghrc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/gfhwimcay.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gsxaeapwf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.tarul.cn/Article/details/gutfjqfju.sHtML

[R61] 磁盘占用
来源：http://3g.epnwcf.com/Article/details/gibdpdaba.sHtML

df -h;  du -sh *
来源：http://wap.bbcook.cn/Article/details/gyexkqxfe.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.yfazqb.com/Article/details/guqmgtrmu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.vehdjk.com/Article/details/guxihxgug.sHtML

[R63] 内存与进程
来源：http://m.share.vehdjk.com/Article/details/gnbsrhyqq.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.yfazqb.com/Article/details/gjtqklqtf.sHtML

[R64] 结束进程
来源：http://m.share.sjlbkw.cn/Article/details/ggjylwenx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.tarul.cn/Article/details/glmjjmdjg.sHtML

[R65] 查看端口占用
来源：http://blog.sjlbkw.cn/Article/details/gocdqnmbf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.epnwcf.com/Article/details/gxyusbtse.sHtML

[R66] 定时任务
来源：http://read.share.bbcook.cn/Article/details/gdecrrjjq.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbjlrflt.sHtML

[R67] 生成随机十六进制串
来源：http://3g.bbcook.cn/Article/details/gtxxviszg.sHtML

openssl rand -hex 16
来源：http://www.share.tarul.cn/Article/details/giiucywgt.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.epnwcf.com/Article/details/gkrqaxdcu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.tarul.cn/Article/details/gndwwclcb.sHtML

[R69] 生成随机密码
来源：http://blog.bbcook.cn/Article/details/grtlipnsx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.yfazqb.com/Article/details/gbvipfuvx.sHtML

[R70] 时间戳与互转
来源：http://m.share.sjlbkw.cn/Article/details/gxjgxisdd.sHtML

date +%s;  date -d @1700000000
来源：http://wap.yfazqb.com/Article/details/gfwooavdd.sHtML

[R71] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gmloxtimd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.bbcook.cn/Article/details/gqmxffbnf.sHtML

[R72] 等待端口就绪
来源：http://blog.fktsv.cn/Article/details/gaqznqsxr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/ghajhwswz.sHtML

[R73] 分割大日志
来源：http://m.share.sjlbkw.cn/Article/details/goazxxgln.sHtML

split -l 1000 big.log part_
来源：http://blog.tarul.cn/Article/details/gzlzdqobr.sHtML

[R74] 批量重命名
来源：http://wap.yfazqb.com/Article/details/googbqcfm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/gcwjfwnnn.sHtML

[R75] 导出环境变量
来源：http://wap.epnwcf.com/Article/details/gnfkcbhru.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.sjlbkw.cn/Article/details/gsocvuoit.sHtML

[R76] 使用临时文件
来源：http://read.share.vehdjk.com/Article/details/gsjlwrgjw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gtdlrhadk.sHtML

[R77] 读取用户输入
来源：http://read.share.tarul.cn/Article/details/gorajkahd.sHtML

read -rp "请输入: " ans
来源：http://baike.sjlbkw.cn/Article/details/gmznigvlq.sHtML

[R78] 交互式菜单
来源：http://www.m.share.tarul.cn/Article/details/ghpwbxkrf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.sjlbkw.cn/Article/details/gvlthxtsi.sHtML

[R79] 解析命令行选项
来源：http://read.share.fktsv.cn/Article/details/gjxvnpxxl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.sjlbkw.cn/Article/details/gyywbvbvr.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.vehdjk.com/Article/details/geubxjhgy.sHtML

time ./run.sh
来源：http://mobile.yfazqb.com/Article/details/gkehuqbgj.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ggxgewjgv.sHtML

S. C / C++ 专题
来源：http://m.share.epnwcf.com/Article/details/gnrwowhbu.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grvdgabwd.sHtML

[S01] C：Hello World
来源：http://www.share.yfazqb.com/Article/details/gfpzdtcel.sHtML

#include <stdio.h>
来源：http://3g.epnwcf.com/Article/details/gqibpubhw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.bbcook.cn/Article/details/gezaoipsa.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gfrthimfa.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fktsv.cn/Article/details/grforkgsf.sHtML

[S03] C：读入整数
来源：http://www.m.share.bbcook.cn/Article/details/gnmfcamcd.sHtML

int x; scanf("%d", &x);
来源：http://mobile.yfazqb.com/Article/details/grhmydleq.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/glsavosxa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.tarul.cn/Article/details/gqjxyvidu.sHtML

[S05] C：字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gqaicnrtg.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/gtnirfywb.sHtML

[S06] C：字符串比较
来源：http://read.share.yfazqb.com/Article/details/grlxrwvxv.sHtML

strcmp(a, b) == 0
来源：http://m.share.epnwcf.com/Article/details/gjddgehvz.sHtML

[S07] C：数组遍历求和
来源：http://baike.vehdjk.com/Article/details/gdyfbdqjc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.sjlbkw.cn/Article/details/gqmjbtnqa.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.vehdjk.com/Article/details/gjnmamtnf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.epnwcf.com/Article/details/gztghsddi.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.sjlbkw.cn/Article/details/gyeprffoe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.sjlbkw.cn/Article/details/grawygcve.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.tarul.cn/Article/details/gaguruwed.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.vehdjk.com/Article/details/gmvkjabll.sHtML

[S11] C：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gmrgczaac.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.tarul.cn/Article/details/gzkroxqoq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.yfazqb.com/Article/details/gmrtplhqw.sHtML

fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gzfyzfgsx.sHtML

[S12] C：写文件
来源：http://mobile.bbcook.cn/Article/details/gfveuzbon.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gzfmkcxwu.sHtML

[S13] C：宏定义
来源：http://www.m.share.tarul.cn/Article/details/glarnwxqw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.sjlbkw.cn/Article/details/gsmupvqtl.sHtML

[S14] C：枚举
来源：http://mobile.epnwcf.com/Article/details/gwkjutbuu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.yfazqb.com/Article/details/genaegewc.sHtML

[S15] C：类型转换
来源：http://read.share.vehdjk.com/Article/details/gghatlpny.sHtML

(double) a / b
来源：http://www.m.share.vehdjk.com/Article/details/gfzkwspvy.sHtML

[S16] C：位操作置位
来源：http://3g.sjlbkw.cn/Article/details/gjiybnhlo.sHtML

x |= (1 << 3);
来源：http://baike.fktsv.cn/Article/details/gqjhqnjov.sHtML

[S17] C：安全拼接字符串
来源：http://baike.yfazqb.com/Article/details/gowkrufes.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.yfazqb.com/Article/details/gcltpwayw.sHtML

[S18] C：命令行参数
来源：http://mobile.sjlbkw.cn/Article/details/gdvdpkhtx.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.vehdjk.com/Article/details/gseahstgv.sHtML

[S19] C：快速排序
来源：http://www.m.share.epnwcf.com/Article/details/gsaruizyj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/gnmfuqoav.sHtML

[S20] C：二分查找
来源：http://m.share.bbcook.cn/Article/details/gjbamexuv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gimbuggjt.sHtML

[S21] C：字符类别判断
来源：http://3g.fktsv.cn/Article/details/govkawfps.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/gopjxraxm.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.tarul.cn/Article/details/guyqduoha.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.epnwcf.com/Article/details/gpkfagutm.sHtML

[S23] C：随机数
来源：http://blog.fktsv.cn/Article/details/gfhdaktay.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.bbcook.cn/Article/details/gwnkanhqi.sHtML

[S24] C：获取本地时间
来源：http://www.blog.vehdjk.com/Article/details/glthdukfd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.sjlbkw.cn/Article/details/gscuxbygl.sHtML

[S25] C：内存拷贝
来源：http://read.share.fktsv.cn/Article/details/ghlmhylmq.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/givlwnfok.sHtML

[S26] C：内存清零
来源：http://wap.tarul.cn/Article/details/gfetmxptu.sHtML

memset(a, 0, sizeof a);
来源：http://baike.epnwcf.com/Article/details/gitioyvzw.sHtML

[S27] C：定义常量
来源：http://wap.yfazqb.com/Article/details/guzuiwlvv.sHtML

const double PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gfrsrbgke.sHtML

[S28] C：静态变量
来源：http://www.blog.fktsv.cn/Article/details/gktjdpkhz.sHtML

static int counter = 0;
来源：http://baike.fktsv.cn/Article/details/gjkqmixrk.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/grlatsokz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.vehdjk.com/Article/details/gyzkwdkhy.sHtML

[S30] C：头文件保护
来源：http://blog.bbcook.cn/Article/details/gctchosmk.sHtML

#ifndef X_H
来源：http://blog.vehdjk.com/Article/details/gqieaiyfs.sHtML

#define X_H
来源：http://m.share.epnwcf.com/Article/details/gfoaabdcl.sHtML

#endif
来源：http://3g.yfazqb.com/Article/details/gvrycrehv.sHtML

[S31] C++：Hello World
来源：http://mobile.bbcook.cn/Article/details/gsljqcklg.sHtML

#include <iostream>
来源：http://www.m.share.vehdjk.com/Article/details/gqzwctdfq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.tarul.cn/Article/details/gdtuldsjj.sHtML

[S32] C++：字符串
来源：http://www.blog.sjlbkw.cn/Article/details/ggfrdjjrs.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fktsv.cn/Article/details/gizyuxkoj.sHtML

[S33] C++：vector 增删
来源：http://3g.epnwcf.com/Article/details/grjychxtd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.tarul.cn/Article/details/gwkdrhole.sHtML

[S34] C++：遍历 vector
来源：http://baike.epnwcf.com/Article/details/ghwvqknfu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fktsv.cn/Article/details/gbhnwjjza.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gblbacmzz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gucuzjeso.sHtML

[S36] C++：unordered_map
来源：http://read.share.fktsv.cn/Article/details/gkdmjqiis.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gbadgorib.sHtML

[S37] C++：set
来源：http://read.share.fktsv.cn/Article/details/gofetjmsj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.bbcook.cn/Article/details/gqtayeidy.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gvkmsyfde.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gaaczibak.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.sjlbkw.cn/Article/details/giqnarnaj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.vehdjk.com/Article/details/gbxtliptr.sHtML

[S40] C++：查找元素
来源：http://mobile.yfazqb.com/Article/details/gcjniktsj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.epnwcf.com/Article/details/grchaudwh.sHtML

[S41] C++：类与构造函数
来源：http://www.share.bbcook.cn/Article/details/gvdhgkrdo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fktsv.cn/Article/details/gokwepyli.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/gqaxhtqeg.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fktsv.cn/Article/details/giocpfmww.sHtML

[S43] C++：智能指针
来源：http://m.share.epnwcf.com/Article/details/guqiqluca.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.yfazqb.com/Article/details/gmukihewv.sHtML

[S44] C++：引用传参
来源：http://www.share.epnwcf.com/Article/details/gkymhzooj.sHtML

void inc(int &x) { ++x; }
来源：http://3g.sjlbkw.cn/Article/details/gqgpjgnbz.sHtML

[S45] C++：lambda
来源：http://www.share.sjlbkw.cn/Article/details/gjzwtmonf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.epnwcf.com/Article/details/gomuwnidy.sHtML

[S46] C++：函数模板
来源：http://3g.bbcook.cn/Article/details/gxjclcshx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.bbcook.cn/Article/details/gxlltbqog.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fktsv.cn/Article/details/gjygbjppk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fktsv.cn/Article/details/gqgdshufa.sHtML

[S48] C++：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gzkjljllq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fktsv.cn/Article/details/gvputatlf.sHtML

while (std::getline(in, line)) { }
来源：http://baike.sjlbkw.cn/Article/details/gaqmkazfx.sHtML

[S49] C++：写文件
来源：http://m.share.vehdjk.com/Article/details/ghrgxrrnd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.bbcook.cn/Article/details/gzsbfijpb.sHtML

[S50] C++：格式化数字
来源：http://mobile.vehdjk.com/Article/details/gzzcpzkwq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gobyssmep.sHtML

[S51] C++：显式类型转换
来源：http://m.share.tarul.cn/Article/details/gthwajdun.sHtML

static_cast<double>(a) / b
来源：http://read.share.tarul.cn/Article/details/gbzcwugxi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.bbcook.cn/Article/details/giwkivjwu.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fktsv.cn/Article/details/goktxqttc.sHtML

[S53] C++：移动语义
来源：http://baike.sjlbkw.cn/Article/details/gwmxmpgrb.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.vehdjk.com/Article/details/gjddwmeha.sHtML

[S54] C++：异常处理
来源：http://www.m.share.epnwcf.com/Article/details/gzpkabwid.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.yfazqb.com/Article/details/getouxfqv.sHtML

[S55] C++：结构化绑定
来源：http://3g.tarul.cn/Article/details/gmgeabepc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.epnwcf.com/Article/details/gajpjovyq.sHtML

[S56] C++：optional
来源：http://read.share.epnwcf.com/Article/details/gkmflesnp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fktsv.cn/Article/details/gjjcxpauu.sHtML

[S57] C++：编译期常量
来源：http://blog.fktsv.cn/Article/details/gehcltjlk.sHtML

constexpr int N = 10;
来源：http://wap.fktsv.cn/Article/details/gemvcmmag.sHtML

[S58] C++：命名空间
来源：http://wap.epnwcf.com/Article/details/ggxxbigdn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.tarul.cn/Article/details/gbmzhfcae.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/gahhgufmt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fktsv.cn/Article/details/gperyhlau.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.vehdjk.com/Article/details/garygoliz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gpehjvzpv.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gfbzxsfzm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.tarul.cn/Article/details/gpzveyhnf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gqqwwscpk.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/ghchmaivt.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gjetplhop.sHtML

[T02] Kotlin：变量
来源：http://m.share.bbcook.cn/Article/details/gzdxjswdn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyazmrfm.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fktsv.cn/Article/details/gikgnwdwi.sHtML

"值: $b"
来源：http://baike.epnwcf.com/Article/details/gsakotwdq.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/gnmpkecfp.sHtML

val n: String? = null;  n?.length
来源：http://m.share.bbcook.cn/Article/details/gkoysgexl.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.epnwcf.com/Article/details/gialladxl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.yfazqb.com/Article/details/grqhmusdt.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fktsv.cn/Article/details/gjpmehzqu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.bbcook.cn/Article/details/gihyjdvzq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.vehdjk.com/Article/details/gbeqjzeuh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.bbcook.cn/Article/details/gudqnckxj.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.yfazqb.com/Article/details/gmvmzmfun.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/gjputklrj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.yfazqb.com/Article/details/ggpstsdrk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.yfazqb.com/Article/details/gugwhvhmk.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.tarul.cn/Article/details/gsyzozivw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.tarul.cn/Article/details/gxsvgcoiq.sHtML

[T11] Kotlin：协程
来源：http://www.blog.sjlbkw.cn/Article/details/gyukpczqk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.yfazqb.com/Article/details/gkdnaydmr.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.bbcook.cn/Article/details/gyesuwbqu.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.bbcook.cn/Article/details/ghccotfkj.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.vehdjk.com/Article/details/gxzipgubi.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.bbcook.cn/Article/details/gphelhqwe.sHtML

[T14] Kotlin：循环
来源：http://3g.tarul.cn/Article/details/gczroksls.sHtML

for (i in 1..10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/glglrrxeu.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fktsv.cn/Article/details/gltkgadfj.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fktsv.cn/Article/details/gblldeeoo.sHtML

[T16] Swift：Hello World
来源：http://mobile.bbcook.cn/Article/details/gtyftueyx.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gfamikfli.sHtML

[T17] Swift：变量与常量
来源：http://baike.vehdjk.com/Article/details/gzdjbkvnq.sHtML

var a = 1;  let b = 2
来源：http://wap.epnwcf.com/Article/details/gxhjuorjm.sHtML

[T18] Swift：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gzwzyfskz.sHtML

"值: \(b)"
来源：http://blog.tarul.cn/Article/details/gdfhhgylb.sHtML

[T19] Swift：可选绑定
来源：http://blog.sjlbkw.cn/Article/details/gabidwkxk.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqppupch.sHtML

[T20] Swift：数组操作
来源：http://www.blog.epnwcf.com/Article/details/gtlcjkkjz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.bbcook.cn/Article/details/gofrkwrfi.sHtML

[T21] Swift：遍历
来源：http://baike.fktsv.cn/Article/details/geuwysjxh.sHtML

for x in a { print(x) }
来源：http://www.share.sjlbkw.cn/Article/details/gavpwtbyh.sHtML

[T22] Swift：字典
来源：http://read.share.sjlbkw.cn/Article/details/gwyjtwwfl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.yfazqb.com/Article/details/gtcijemeg.sHtML


<!-- 参考信息 -->