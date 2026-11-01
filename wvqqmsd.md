代发 wailian999

echo "${#s}"
来源：http://3g.bbcook.cn/Article/details/gmdicwphw.sHtML

[R22] 截取子串
来源：http://3g.epnwcf.com/Article/details/gxnfyhxpt.sHtML

echo "${s:0:5}"
来源：http://www.share.sjlbkw.cn/Article/details/gwjxeyely.sHtML

[R23] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gspwzfvhb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.tarul.cn/Article/details/gosszcihd.sHtML

[R24] 大小写转换
来源：http://baike.fktsv.cn/Article/details/gvdbbkesm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.tarul.cn/Article/details/gyqlmrrtq.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.tarul.cn/Article/details/gocbmbvca.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.tarul.cn/Article/details/gicbqflkn.sHtML

[R26] 命令替换
来源：http://blog.bbcook.cn/Article/details/gfbgwqvin.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.yfazqb.com/Article/details/gfbeqrvru.sHtML

[R27] 算术展开
来源：http://baike.epnwcf.com/Article/details/gqwgqgnfc.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.yfazqb.com/Article/details/gqggahjvl.sHtML

[R28] 浮点运算
来源：http://www.blog.epnwcf.com/Article/details/gtoqrandz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.bbcook.cn/Article/details/gvzbumwxb.sHtML

[R29] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gteknoslt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fktsv.cn/Article/details/glogpqwok.sHtML

[R30] 函数返回状态码
来源：http://m.share.yfazqb.com/Article/details/guhknpwqq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.vehdjk.com/Article/details/gffzbferz.sHtML

[R31] 局部变量
来源：http://3g.bbcook.cn/Article/details/gwizthcbp.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/gkvhpixqn.sHtML

[R32] 参数个数校验
来源：http://wap.epnwcf.com/Article/details/gxcadgfcg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gxamgzcyr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fktsv.cn/Article/details/gqdmaffmz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.bbcook.cn/Article/details/goevklyrd.sHtML

[R34] 退出时清理
来源：http://www.m.share.sjlbkw.cn/Article/details/gstbhdkgb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/gjcotgsry.sHtML

[R35] 后台执行并等待
来源：http://3g.tarul.cn/Article/details/gtnxajpld.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.bbcook.cn/Article/details/gbgmkvooa.sHtML

[R36] 并发执行多个任务
来源：http://m.share.yfazqb.com/Article/details/gpclsbczu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.bbcook.cn/Article/details/guncvbrof.sHtML

[R37] 把输出赋给变量
来源：http://www.share.bbcook.cn/Article/details/gosnzszsl.sHtML

files=$(ls -1)
来源：http://m.share.fktsv.cn/Article/details/gwcivgfuy.sHtML

[R38] 管道串联
来源：http://www.blog.vehdjk.com/Article/details/ganktzxvp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.yfazqb.com/Article/details/gbxrslids.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.sjlbkw.cn/Article/details/gonzbtcll.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/ghtvlesow.sHtML

[R40] 追加写日志
来源：http://blog.vehdjk.com/Article/details/gisisdnua.sHtML

echo "log" >> out.log
来源：http://www.share.vehdjk.com/Article/details/gneuesbho.sHtML

[R41] 丢弃输出
来源：http://m.share.sjlbkw.cn/Article/details/gjlscclnd.sHtML

cmd >/dev/null 2>&1
来源：http://3g.yfazqb.com/Article/details/geiavobko.sHtML

[R42] 输入重定向
来源：http://baike.tarul.cn/Article/details/gqtuupwyn.sHtML

wc -l < a.txt
来源：http://read.share.tarul.cn/Article/details/gbqtzxmiw.sHtML

[R43] 按名字查找文件
来源：http://3g.tarul.cn/Article/details/gkafsvcbb.sHtML

find . -name "*.log" -type f
来源：http://blog.bbcook.cn/Article/details/gicyonudy.sHtML

[R44] 按修改时间查找
来源：http://wap.tarul.cn/Article/details/gzmngtokt.sHtML

find . -mtime -7 -type f
来源：http://baike.epnwcf.com/Article/details/grahbueol.sHtML

[R45] 批量删除
来源：http://www.m.share.epnwcf.com/Article/details/gqdxazfek.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.epnwcf.com/Article/details/gwczoyjap.sHtML

[R46] 递归替换文件内容
来源：http://3g.bbcook.cn/Article/details/gqrnvsvft.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/gpjofrtks.sHtML

[R47] sed 单行替换
来源：http://baike.epnwcf.com/Article/details/gcygpxrqm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.vehdjk.com/Article/details/gtyzpuyyq.sHtML

[R48] awk 取指定列
来源：http://baike.tarul.cn/Article/details/ghitjglpg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/glxaylbrl.sHtML

[R49] awk 带条件
来源：http://wap.fktsv.cn/Article/details/gxexoygbn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.vehdjk.com/Article/details/gjjpjxflr.sHtML

[R50] awk 求和
来源：http://blog.yfazqb.com/Article/details/gldptnavu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/ghyyijplo.sHtML

[R51] 排序去重取前几
来源：http://mobile.epnwcf.com/Article/details/gbdktjrui.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.bbcook.cn/Article/details/gcrpzckgd.sHtML

[R52] 统计行数
来源：http://blog.bbcook.cn/Article/details/ghinhkiqd.sHtML

wc -l a.txt
来源：http://www.share.yfazqb.com/Article/details/gxseqexdr.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/gguqryfmt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.sjlbkw.cn/Article/details/gxjmswgak.sHtML

[R54] 比较两个文件
来源：http://m.share.fktsv.cn/Article/details/gawgdbvpy.sHtML

diff a.txt b.txt
来源：http://www.share.bbcook.cn/Article/details/gdivvlyei.sHtML

[R55] 压缩与解压
来源：http://mobile.tarul.cn/Article/details/gyunkbiel.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gmzdplzwz.sHtML

[R56] 远程拷贝
来源：http://baike.fktsv.cn/Article/details/guohfczzx.sHtML

scp file user@host:/path/
来源：http://wap.vehdjk.com/Article/details/gbrrzqwjx.sHtML

[R57] 远程执行命令
来源：http://read.share.bbcook.cn/Article/details/ghvsyadmo.sHtML

ssh user@host 'uptime'
来源：http://wap.bbcook.cn/Article/details/gqxtodzxx.sHtML

[R58] 下载文件
来源：http://m.share.tarul.cn/Article/details/gtjedndvh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.tarul.cn/Article/details/gskcpaetv.sHtML

[R59] 发 POST JSON
来源：http://read.share.tarul.cn/Article/details/gefbulbos.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.epnwcf.com/Article/details/ggjwmjxua.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/gicaftlcm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.vehdjk.com/Article/details/gvjqnyvff.sHtML

[R61] 磁盘占用
来源：http://baike.vehdjk.com/Article/details/gqnayjfdm.sHtML

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/gyjhzxuvj.sHtML

[R62] 找最占空间的文件
来源：http://wap.bbcook.cn/Article/details/guamlkdyv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.tarul.cn/Article/details/ggtrjjjbe.sHtML

[R63] 内存与进程
来源：http://wap.epnwcf.com/Article/details/gehrldjyp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fktsv.cn/Article/details/gqvvmmodg.sHtML

[R64] 结束进程
来源：http://www.blog.yfazqb.com/Article/details/gcsrpklgu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.vehdjk.com/Article/details/gbzcsqibl.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fktsv.cn/Article/details/ggcagldvz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.vehdjk.com/Article/details/ghiafhaog.sHtML

[R66] 定时任务
来源：http://mobile.bbcook.cn/Article/details/gqnornebm.sHtML

crontab -e;  crontab -l
来源：http://read.share.vehdjk.com/Article/details/gvnidthbn.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.tarul.cn/Article/details/gpyrmkbcq.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/gkofdldha.sHtML

[R68] 计算文件校验值
来源：http://mobile.yfazqb.com/Article/details/gppmakxbf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gtkdpngkp.sHtML

[R69] 生成随机密码
来源：http://baike.yfazqb.com/Article/details/golaggncp.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.yfazqb.com/Article/details/gksbvoyqo.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/gwkmwwjpn.sHtML

date +%s;  date -d @1700000000
来源：http://baike.tarul.cn/Article/details/gzninzxij.sHtML

[R71] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/ggfyehqrr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.sjlbkw.cn/Article/details/ghzmgmpdv.sHtML

[R72] 等待端口就绪
来源：http://wap.tarul.cn/Article/details/gbyiaqqqe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gpeaczhkh.sHtML

[R73] 分割大日志
来源：http://read.share.vehdjk.com/Article/details/gbzntcytx.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/gbkbxawnq.sHtML

[R74] 批量重命名
来源：http://blog.epnwcf.com/Article/details/gmfhrlosi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.vehdjk.com/Article/details/ghaburcja.sHtML

[R75] 导出环境变量
来源：http://blog.sjlbkw.cn/Article/details/ghehonoof.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.vehdjk.com/Article/details/gofnkdkso.sHtML

[R76] 使用临时文件
来源：http://baike.vehdjk.com/Article/details/gnypkaiec.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/ggzusaybi.sHtML

[R77] 读取用户输入
来源：http://blog.vehdjk.com/Article/details/gmdnzquez.sHtML

read -rp "请输入: " ans
来源：http://wap.epnwcf.com/Article/details/goxohpmnn.sHtML

[R78] 交互式菜单
来源：http://blog.epnwcf.com/Article/details/ggqaqxzef.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.epnwcf.com/Article/details/ggzxrawdr.sHtML

[R79] 解析命令行选项
来源：http://read.share.fktsv.cn/Article/details/gccikpryo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.sjlbkw.cn/Article/details/goywdkelb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.sjlbkw.cn/Article/details/gsyiiwojh.sHtML

time ./run.sh
来源：http://www.blog.vehdjk.com/Article/details/gloxsgkfh.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbzhdnfmv.sHtML

S. C / C++ 专题
来源：http://mobile.tarul.cn/Article/details/glcydcjod.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ganbfrmqk.sHtML

[S01] C：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gorgsrvql.sHtML

#include <stdio.h>
来源：http://mobile.yfazqb.com/Article/details/gvlfefgut.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.epnwcf.com/Article/details/gbctvguhd.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/giptlqaiw.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.yfazqb.com/Article/details/gwauoirjm.sHtML

[S03] C：读入整数
来源：http://www.m.share.fktsv.cn/Article/details/gblfhktkj.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.epnwcf.com/Article/details/gwdcvietm.sHtML

[S04] C：字符串复制
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcyrfbzl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.vehdjk.com/Article/details/gbowdwmsv.sHtML

[S05] C：字符串长度
来源：http://read.share.tarul.cn/Article/details/gvgyavybj.sHtML

strlen(s)
来源：http://baike.fktsv.cn/Article/details/ghslkreoy.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/gutavojmh.sHtML

strcmp(a, b) == 0
来源：http://m.share.sjlbkw.cn/Article/details/glsswjhhi.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.yfazqb.com/Article/details/gzsdbivwq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.tarul.cn/Article/details/gkotpecdi.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.yfazqb.com/Article/details/gfeqloqxk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.bbcook.cn/Article/details/gubauzcef.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.yfazqb.com/Article/details/gjrsuemyj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.vehdjk.com/Article/details/gbowvzqjn.sHtML

[S10] C：指针与解引用
来源：http://baike.fktsv.cn/Article/details/ghydpbooq.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fktsv.cn/Article/details/gxfaictzw.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gufqqxnco.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.tarul.cn/Article/details/grtpvtwgr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.sjlbkw.cn/Article/details/gxurmbsin.sHtML

fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/gdbdhunvm.sHtML

[S12] C：写文件
来源：http://m.share.bbcook.cn/Article/details/gzxsxsntc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/giltapykp.sHtML

[S13] C：宏定义
来源：http://blog.fktsv.cn/Article/details/gscpujdnf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.tarul.cn/Article/details/gwdhdpvte.sHtML

[S14] C：枚举
来源：http://3g.tarul.cn/Article/details/gjqrtoxmx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.bbcook.cn/Article/details/gklhuclcf.sHtML

[S15] C：类型转换
来源：http://wap.sjlbkw.cn/Article/details/gmibjgzmn.sHtML

(double) a / b
来源：http://3g.tarul.cn/Article/details/gxnjbebnh.sHtML

[S16] C：位操作置位
来源：http://mobile.sjlbkw.cn/Article/details/gvqrtwmun.sHtML

x |= (1 << 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/getnalboc.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fktsv.cn/Article/details/gozireahx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fktsv.cn/Article/details/gylmylmbr.sHtML

[S18] C：命令行参数
来源：http://blog.bbcook.cn/Article/details/gofdbmidc.sHtML

int main(int argc, char **argv)
来源：http://baike.fktsv.cn/Article/details/gadvbsamd.sHtML

[S19] C：快速排序
来源：http://m.share.bbcook.cn/Article/details/gcfshvrbu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gvothxcta.sHtML

[S20] C：二分查找
来源：http://blog.vehdjk.com/Article/details/glnncqtnb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gwzjnwmrg.sHtML

[S21] C：字符类别判断
来源：http://read.share.yfazqb.com/Article/details/gokmlyult.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.epnwcf.com/Article/details/gnaceztwh.sHtML

[S22] C：字符串转数字
来源：http://www.share.epnwcf.com/Article/details/gcufkvoad.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fktsv.cn/Article/details/gmhbeygyf.sHtML

[S23] C：随机数
来源：http://mobile.vehdjk.com/Article/details/gbwfarqiv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.sjlbkw.cn/Article/details/gbwsjavef.sHtML

[S24] C：获取本地时间
来源：http://m.share.fktsv.cn/Article/details/gawzjtmpo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.sjlbkw.cn/Article/details/gztjavffl.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/grbvdmrsd.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/gsterzyzt.sHtML

[S26] C：内存清零
来源：http://m.share.epnwcf.com/Article/details/glemvglnw.sHtML

memset(a, 0, sizeof a);
来源：http://baike.yfazqb.com/Article/details/gyeulcjdf.sHtML

[S27] C：定义常量
来源：http://baike.tarul.cn/Article/details/giiqmxuui.sHtML

const double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gqzgsccub.sHtML

[S28] C：静态变量
来源：http://mobile.sjlbkw.cn/Article/details/gizyhtivm.sHtML

static int counter = 0;
来源：http://3g.tarul.cn/Article/details/grsclkdku.sHtML

[S29] C：变参函数
来源：http://3g.tarul.cn/Article/details/gubgvjlwm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.bbcook.cn/Article/details/gaqxwdxig.sHtML

[S30] C：头文件保护
来源：http://wap.bbcook.cn/Article/details/gjtiuptqu.sHtML

#ifndef X_H
来源：http://read.share.bbcook.cn/Article/details/gzxeokprj.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/gblglmpmx.sHtML

#endif
来源：http://www.share.bbcook.cn/Article/details/gidofrbyu.sHtML

[S31] C++：Hello World
来源：http://mobile.bbcook.cn/Article/details/gyseffecn.sHtML

#include <iostream>
来源：http://blog.yfazqb.com/Article/details/gmiqmqrix.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.sjlbkw.cn/Article/details/gxykpgkvh.sHtML

[S32] C++：字符串
来源：http://baike.bbcook.cn/Article/details/gvapcglhq.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/gtnshmuvs.sHtML

[S33] C++：vector 增删
来源：http://3g.epnwcf.com/Article/details/gjhlrvumj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnaktdst.sHtML

[S34] C++：遍历 vector
来源：http://www.share.tarul.cn/Article/details/gvhomkkol.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.bbcook.cn/Article/details/gjlbmwccc.sHtML

[S35] C++：map
来源：http://mobile.bbcook.cn/Article/details/ggynmjplp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gemsprhsw.sHtML

[S36] C++：unordered_map
来源：http://wap.bbcook.cn/Article/details/gmtnmxdip.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/guebbpndr.sHtML

[S37] C++：set
来源：http://baike.fktsv.cn/Article/details/glbjuupwa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/gkztxitvy.sHtML

[S38] C++：排序
来源：http://blog.fktsv.cn/Article/details/grqgeciph.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/ggjmkqukr.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.epnwcf.com/Article/details/gmwjgglpw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.bbcook.cn/Article/details/gfvfygbeu.sHtML

[S40] C++：查找元素
来源：http://wap.bbcook.cn/Article/details/gmwxxyxwr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gexjymcha.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fktsv.cn/Article/details/gowrrjywc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.tarul.cn/Article/details/gikyfgxvh.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.sjlbkw.cn/Article/details/gmswkzgtp.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.yfazqb.com/Article/details/geurqswsg.sHtML

[S43] C++：智能指针
来源：http://baike.sjlbkw.cn/Article/details/ghebmrylx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fktsv.cn/Article/details/gigfajgag.sHtML

[S44] C++：引用传参
来源：http://m.share.tarul.cn/Article/details/gcyklysyx.sHtML

void inc(int &x) { ++x; }
来源：http://3g.bbcook.cn/Article/details/genaljxlr.sHtML

[S45] C++：lambda
来源：http://3g.tarul.cn/Article/details/galdnyqcs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.tarul.cn/Article/details/gdtihkzal.sHtML

[S46] C++：函数模板
来源：http://m.share.fktsv.cn/Article/details/gppefumze.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fktsv.cn/Article/details/gfatanink.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.epnwcf.com/Article/details/ghrgnzyei.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fktsv.cn/Article/details/ghvokrksz.sHtML

[S48] C++：逐行读文件
来源：http://blog.tarul.cn/Article/details/gqzdyagsf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.vehdjk.com/Article/details/gbuqfceia.sHtML

while (std::getline(in, line)) { }
来源：http://baike.yfazqb.com/Article/details/guazwsllp.sHtML

[S49] C++：写文件
来源：http://baike.sjlbkw.cn/Article/details/guaqagjiq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fktsv.cn/Article/details/gqyonxwft.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/gphhvyvkv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gnfarqvdr.sHtML

[S51] C++：显式类型转换
来源：http://m.share.bbcook.cn/Article/details/gwwgqatiy.sHtML

static_cast<double>(a) / b
来源：http://baike.bbcook.cn/Article/details/gnzhfvcxo.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fktsv.cn/Article/details/ghxkyuphe.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/gaaeceupw.sHtML

[S53] C++：移动语义
来源：http://www.share.sjlbkw.cn/Article/details/gnvsqewcb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.epnwcf.com/Article/details/gzabtlfji.sHtML

[S54] C++：异常处理
来源：http://www.blog.epnwcf.com/Article/details/gnjkupowl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.epnwcf.com/Article/details/glnfnnixb.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.epnwcf.com/Article/details/glheilazl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.vehdjk.com/Article/details/gatdneyuq.sHtML

[S56] C++：optional
来源：http://mobile.sjlbkw.cn/Article/details/gqwddykev.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.tarul.cn/Article/details/ggkidqcbm.sHtML

[S57] C++：编译期常量
来源：http://m.share.epnwcf.com/Article/details/gdfjuezha.sHtML

constexpr int N = 10;
来源：http://read.share.bbcook.cn/Article/details/gckciidcc.sHtML

[S58] C++：命名空间
来源：http://blog.vehdjk.com/Article/details/gdxwuczdf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.tarul.cn/Article/details/gosehqifb.sHtML

[S59] C++：静态断言
来源：http://www.blog.vehdjk.com/Article/details/gamehfool.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.epnwcf.com/Article/details/gxudpfits.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.yfazqb.com/Article/details/gcoyskczp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.vehdjk.com/Article/details/grusbtcvw.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gluhrmiyc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.epnwcf.com/Article/details/gdebmtbdp.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gpnkazwtz.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gwmfvhvzu.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gwzscobmt.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.yfazqb.com/Article/details/glhnoniqk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.vehdjk.com/Article/details/gbnqfblzd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.bbcook.cn/Article/details/godmblenp.sHtML

"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gyvbechup.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/gldxxgevs.sHtML

val n: String? = null;  n?.length
来源：http://m.share.tarul.cn/Article/details/gvlabrwqg.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.sjlbkw.cn/Article/details/gijgtzjzm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gzygpzfke.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fktsv.cn/Article/details/gaslseowv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.bbcook.cn/Article/details/gnautwily.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.vehdjk.com/Article/details/gmpridels.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.vehdjk.com/Article/details/gderlnlgj.sHtML

[T08] Kotlin：数据类
来源：http://www.share.yfazqb.com/Article/details/gfyglabhu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.epnwcf.com/Article/details/gzucinfcs.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.sjlbkw.cn/Article/details/gvewpwgcr.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.bbcook.cn/Article/details/ggndxtxnq.sHtML

[T10] Kotlin：默认参数
来源：http://3g.bbcook.cn/Article/details/gwgspqtlt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.tarul.cn/Article/details/gfbmzidee.sHtML

[T11] Kotlin：协程
来源：http://m.share.bbcook.cn/Article/details/gvvipqzhv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.sjlbkw.cn/Article/details/gfezewdci.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.epnwcf.com/Article/details/gfsbjgznu.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.tarul.cn/Article/details/gtjtlxqgf.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.yfazqb.com/Article/details/gakbesaat.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.tarul.cn/Article/details/gaelibiiw.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/glsymzhuz.sHtML

for (i in 1..10) println(i)
来源：http://wap.yfazqb.com/Article/details/gdzvgjxrr.sHtML

[T15] Kotlin：接口
来源：http://3g.tarul.cn/Article/details/gaxkzrbjg.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.tarul.cn/Article/details/gogxbqoph.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/guhoxfchs.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/gjansglik.sHtML

[T17] Swift：变量与常量
来源：http://baike.yfazqb.com/Article/details/gjjxfegck.sHtML

var a = 1;  let b = 2
来源：http://read.share.bbcook.cn/Article/details/gkswosjif.sHtML

[T18] Swift：字符串插值
来源：http://3g.bbcook.cn/Article/details/gjefpdjje.sHtML

"值: \(b)"
来源：http://blog.epnwcf.com/Article/details/gmxskcopg.sHtML

[T19] Swift：可选绑定
来源：http://www.share.bbcook.cn/Article/details/gtrvzvjgw.sHtML

if let n = opt { print(n) }
来源：http://mobile.vehdjk.com/Article/details/ggxahoril.sHtML

[T20] Swift：数组操作
来源：http://baike.yfazqb.com/Article/details/gsfeicnlk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gljapkkxq.sHtML

[T21] Swift：遍历
来源：http://read.share.fktsv.cn/Article/details/gvkzaoyst.sHtML

for x in a { print(x) }
来源：http://baike.vehdjk.com/Article/details/gnnxxsflf.sHtML

[T22] Swift：字典
来源：http://wap.bbcook.cn/Article/details/gtgjrlqiq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.vehdjk.com/Article/details/giuplqyeh.sHtML

[T23] Swift：函数
来源：http://baike.tarul.cn/Article/details/gtpwccvew.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fktsv.cn/Article/details/gfcqktbgh.sHtML

[T24] Swift：闭包
来源：http://baike.epnwcf.com/Article/details/ghehwpqhl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fktsv.cn/Article/details/govvwgavb.sHtML


<!-- 参考信息 -->