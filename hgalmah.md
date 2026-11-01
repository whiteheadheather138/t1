代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/gqudbrnct.sHtML

[R18] 遍历数组
来源：http://read.share.sjlbkw.cn/Article/details/gnqfpsnml.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.yfazqb.com/Article/details/ggseivpzf.sHtML

[R19] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/gzqmnrhpl.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.bbcook.cn/Article/details/gdrgxlgmm.sHtML

[R20] 关联数组（字典）
来源：http://3g.epnwcf.com/Article/details/gamzpwhfp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.tarul.cn/Article/details/grigwzefk.sHtML

[R21] 字符串长度
来源：http://m.share.bbcook.cn/Article/details/gpekhswjs.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/gmihnhxnc.sHtML

[R22] 截取子串
来源：http://mobile.vehdjk.com/Article/details/gpdxpksmg.sHtML

echo "${s:0:5}"
来源：http://www.share.yfazqb.com/Article/details/gmfkeccee.sHtML

[R23] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gdvnvhgrx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.tarul.cn/Article/details/gjsrnejec.sHtML

[R24] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gytxyphtn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.tarul.cn/Article/details/gtavuipmu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.tarul.cn/Article/details/gegjgygku.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.tarul.cn/Article/details/grtmbjcwh.sHtML

[R26] 命令替换
来源：http://baike.bbcook.cn/Article/details/glsjdakfs.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.tarul.cn/Article/details/gaaflanfj.sHtML

[R27] 算术展开
来源：http://3g.yfazqb.com/Article/details/gluhctrpl.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.tarul.cn/Article/details/gofetzxha.sHtML

[R28] 浮点运算
来源：http://3g.vehdjk.com/Article/details/gllerlpmn.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.vehdjk.com/Article/details/gcxuoybuj.sHtML

[R29] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gfkqfrzik.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjkmelyv.sHtML

[R30] 函数返回状态码
来源：http://blog.vehdjk.com/Article/details/gtjuucibm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.yfazqb.com/Article/details/ggmnnvbts.sHtML

[R31] 局部变量
来源：http://3g.fktsv.cn/Article/details/ghwjxuljx.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fktsv.cn/Article/details/gdiyydhpu.sHtML

[R32] 参数个数校验
来源：http://www.m.share.bbcook.cn/Article/details/gmkznryou.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gkppyendx.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.vehdjk.com/Article/details/gqgtqoccu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.yfazqb.com/Article/details/gxqyfjhzt.sHtML

[R34] 退出时清理
来源：http://www.m.share.bbcook.cn/Article/details/gdoflgegi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/gdukzrpsr.sHtML

[R35] 后台执行并等待
来源：http://blog.yfazqb.com/Article/details/gnuyjwftq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.vehdjk.com/Article/details/gdbdcdqih.sHtML

[R36] 并发执行多个任务
来源：http://3g.bbcook.cn/Article/details/gobgyixbi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.bbcook.cn/Article/details/gkuiaayay.sHtML

[R37] 把输出赋给变量
来源：http://m.share.tarul.cn/Article/details/gvkuedxfr.sHtML

files=$(ls -1)
来源：http://mobile.vehdjk.com/Article/details/gvmctciwb.sHtML

[R38] 管道串联
来源：http://3g.fktsv.cn/Article/details/gviylqwap.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.sjlbkw.cn/Article/details/gfanqoqrn.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.vehdjk.com/Article/details/gxitzespi.sHtML

cmd > out.log 2>&1
来源：http://mobile.sjlbkw.cn/Article/details/gweamhevg.sHtML

[R40] 追加写日志
来源：http://www.share.vehdjk.com/Article/details/gwvwdjiae.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/gsrpencnu.sHtML

[R41] 丢弃输出
来源：http://wap.tarul.cn/Article/details/gdofpmuyr.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.epnwcf.com/Article/details/gnyymcrsf.sHtML

[R42] 输入重定向
来源：http://wap.bbcook.cn/Article/details/gftwchzay.sHtML

wc -l < a.txt
来源：http://3g.fktsv.cn/Article/details/gpcvuvoac.sHtML

[R43] 按名字查找文件
来源：http://m.share.sjlbkw.cn/Article/details/gueoidirz.sHtML

find . -name "*.log" -type f
来源：http://baike.yfazqb.com/Article/details/giyamhbzd.sHtML

[R44] 按修改时间查找
来源：http://wap.bbcook.cn/Article/details/gcokfwubj.sHtML

find . -mtime -7 -type f
来源：http://read.share.tarul.cn/Article/details/gliezuhut.sHtML

[R45] 批量删除
来源：http://m.share.epnwcf.com/Article/details/gayyefhzi.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.tarul.cn/Article/details/gfykjoaok.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fktsv.cn/Article/details/gdqfuycec.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.epnwcf.com/Article/details/gftehnaks.sHtML

[R47] sed 单行替换
来源：http://www.blog.vehdjk.com/Article/details/gjksbjlct.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/grigordmd.sHtML

[R48] awk 取指定列
来源：http://read.share.yfazqb.com/Article/details/grifyjkpv.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.tarul.cn/Article/details/gurljhjyl.sHtML

[R49] awk 带条件
来源：http://3g.vehdjk.com/Article/details/gqvhoenlo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fktsv.cn/Article/details/gfgenuhus.sHtML

[R50] awk 求和
来源：http://www.m.share.tarul.cn/Article/details/gunjqxoee.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.bbcook.cn/Article/details/gnrxqtzfp.sHtML

[R51] 排序去重取前几
来源：http://mobile.tarul.cn/Article/details/gkpwkynoh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.vehdjk.com/Article/details/gufegblpo.sHtML

[R52] 统计行数
来源：http://www.blog.epnwcf.com/Article/details/gwbfapnod.sHtML

wc -l a.txt
来源：http://wap.sjlbkw.cn/Article/details/gkpaesbzw.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.yfazqb.com/Article/details/gritqzizd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.epnwcf.com/Article/details/gvduwsiix.sHtML

[R54] 比较两个文件
来源：http://3g.yfazqb.com/Article/details/ghrvztpjq.sHtML

diff a.txt b.txt
来源：http://baike.sjlbkw.cn/Article/details/gafgsbbhl.sHtML

[R55] 压缩与解压
来源：http://3g.vehdjk.com/Article/details/gdslsohrz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gdztoeopv.sHtML

[R56] 远程拷贝
来源：http://read.share.fktsv.cn/Article/details/gdrswxaec.sHtML

scp file user@host:/path/
来源：http://www.share.yfazqb.com/Article/details/gkriteenv.sHtML

[R57] 远程执行命令
来源：http://read.share.fktsv.cn/Article/details/gsvwoecok.sHtML

ssh user@host 'uptime'
来源：http://3g.tarul.cn/Article/details/gllhxkrkp.sHtML

[R58] 下载文件
来源：http://blog.sjlbkw.cn/Article/details/gaomcyrhe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.epnwcf.com/Article/details/ghjwyzsym.sHtML

[R59] 发 POST JSON
来源：http://read.share.vehdjk.com/Article/details/gdmzezipj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.yfazqb.com/Article/details/gkwqczfvu.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gdgkcxayf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.yfazqb.com/Article/details/gluwjjynz.sHtML

[R61] 磁盘占用
来源：http://www.m.share.yfazqb.com/Article/details/gttoewwzj.sHtML

df -h;  du -sh *
来源：http://3g.yfazqb.com/Article/details/giowtqgrt.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fktsv.cn/Article/details/gqffaoyfg.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.vehdjk.com/Article/details/gbwyhltan.sHtML

[R63] 内存与进程
来源：http://mobile.sjlbkw.cn/Article/details/gmpaumscy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.bbcook.cn/Article/details/gbwefugor.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gegaqpytn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.sjlbkw.cn/Article/details/gdcainslf.sHtML

[R65] 查看端口占用
来源：http://www.m.share.tarul.cn/Article/details/ggtfuqvzz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.tarul.cn/Article/details/gkudtwsnp.sHtML

[R66] 定时任务
来源：http://www.share.bbcook.cn/Article/details/gtcgpmmbf.sHtML

crontab -e;  crontab -l
来源：http://blog.vehdjk.com/Article/details/geltzsszw.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fktsv.cn/Article/details/gfmxsiihy.sHtML

openssl rand -hex 16
来源：http://read.share.fktsv.cn/Article/details/gcymtiblt.sHtML

[R68] 计算文件校验值
来源：http://wap.sjlbkw.cn/Article/details/gnquxmtuy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.bbcook.cn/Article/details/gzylwrdef.sHtML

[R69] 生成随机密码
来源：http://mobile.tarul.cn/Article/details/gzyvqndzr.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gbnehrhxn.sHtML

[R70] 时间戳与互转
来源：http://mobile.epnwcf.com/Article/details/gnanvnzoy.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.vehdjk.com/Article/details/gksjldmlg.sHtML

[R71] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gtdqrjzhn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.bbcook.cn/Article/details/gfuqejiio.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.sjlbkw.cn/Article/details/gbntbzbwp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/gvyexlykt.sHtML

[R73] 分割大日志
来源：http://m.share.bbcook.cn/Article/details/gqbgfangq.sHtML

split -l 1000 big.log part_
来源：http://read.share.fktsv.cn/Article/details/gwuuwkuya.sHtML

[R74] 批量重命名
来源：http://mobile.tarul.cn/Article/details/gathmycxm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.epnwcf.com/Article/details/gryscrvxy.sHtML

[R75] 导出环境变量
来源：http://www.share.vehdjk.com/Article/details/ggjalezce.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fktsv.cn/Article/details/gtdosenok.sHtML

[R76] 使用临时文件
来源：http://www.share.vehdjk.com/Article/details/gxscnuayy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/givikbqxr.sHtML

[R77] 读取用户输入
来源：http://3g.fktsv.cn/Article/details/gijhjdbum.sHtML

read -rp "请输入: " ans
来源：http://www.blog.tarul.cn/Article/details/gaxiucssj.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/glgtwimlu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.tarul.cn/Article/details/gocsbozwh.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.vehdjk.com/Article/details/geywtfdcv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.vehdjk.com/Article/details/gdknpuaeb.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.yfazqb.com/Article/details/gspncifim.sHtML

time ./run.sh
来源：http://www.share.yfazqb.com/Article/details/gkxqruhrd.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gfpqhevfn.sHtML

S. C / C++ 专题
来源：http://m.share.yfazqb.com/Article/details/gsmeqviih.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmveuvyn.sHtML

[S01] C：Hello World
来源：http://wap.fktsv.cn/Article/details/gzespudin.sHtML

#include <stdio.h>
来源：http://m.share.tarul.cn/Article/details/geihcdrqg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.vehdjk.com/Article/details/gtbmexdrr.sHtML

[S02] C：变量与格式化输出
来源：http://baike.vehdjk.com/Article/details/gopzjcfjk.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.sjlbkw.cn/Article/details/gkwhhfnwu.sHtML

[S03] C：读入整数
来源：http://www.blog.fktsv.cn/Article/details/gtiedyaak.sHtML

int x; scanf("%d", &x);
来源：http://blog.bbcook.cn/Article/details/gdteajthk.sHtML

[S04] C：字符串复制
来源：http://wap.epnwcf.com/Article/details/gfmgcfynk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gsihkytrm.sHtML

[S05] C：字符串长度
来源：http://3g.vehdjk.com/Article/details/gfqlkdzwi.sHtML

strlen(s)
来源：http://www.share.bbcook.cn/Article/details/gxdqdfcom.sHtML

[S06] C：字符串比较
来源：http://m.share.fktsv.cn/Article/details/guwwlxedt.sHtML

strcmp(a, b) == 0
来源：http://baike.vehdjk.com/Article/details/gsuqqzplj.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/gmcwesqru.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.epnwcf.com/Article/details/geioldpno.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.bbcook.cn/Article/details/gydalmpqa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.yfazqb.com/Article/details/goupyxlir.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.sjlbkw.cn/Article/details/gaoulgzja.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.sjlbkw.cn/Article/details/grgryqjan.sHtML

[S10] C：指针与解引用
来源：http://www.share.bbcook.cn/Article/details/gegbbfdws.sHtML

int *p = &a;  *p = 5;
来源：http://blog.tarul.cn/Article/details/ghtkwzhuf.sHtML

[S11] C：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gmbrpneqw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fktsv.cn/Article/details/grptbvgsw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gmensisfq.sHtML

fclose(f);
来源：http://3g.fktsv.cn/Article/details/gxtqakukx.sHtML

[S12] C：写文件
来源：http://wap.fktsv.cn/Article/details/gwkdvntxg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fktsv.cn/Article/details/gyficshyf.sHtML

[S13] C：宏定义
来源：http://www.m.share.fktsv.cn/Article/details/gfmfeoenz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.vehdjk.com/Article/details/gekficgkj.sHtML

[S14] C：枚举
来源：http://baike.fktsv.cn/Article/details/gpljowiuz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.bbcook.cn/Article/details/gstgddatw.sHtML

[S15] C：类型转换
来源：http://www.blog.fktsv.cn/Article/details/gwwbkexpb.sHtML

(double) a / b
来源：http://3g.bbcook.cn/Article/details/gwctvitim.sHtML

[S16] C：位操作置位
来源：http://m.share.bbcook.cn/Article/details/gxpssuskd.sHtML

x |= (1 << 3);
来源：http://www.m.share.yfazqb.com/Article/details/gqmsuwatb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gjlmxwtie.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/gelleevft.sHtML

[S18] C：命令行参数
来源：http://www.share.vehdjk.com/Article/details/gcvicmwmp.sHtML

int main(int argc, char **argv)
来源：http://read.share.vehdjk.com/Article/details/gfwzfysrs.sHtML

[S19] C：快速排序
来源：http://read.share.yfazqb.com/Article/details/gcjjdywgr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gfbyowoco.sHtML

[S20] C：二分查找
来源：http://blog.fktsv.cn/Article/details/gprdbivxx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/gtzozwqyp.sHtML

[S21] C：字符类别判断
来源：http://blog.vehdjk.com/Article/details/gzibbpvkp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.yfazqb.com/Article/details/gpsnopmuz.sHtML

[S22] C：字符串转数字
来源：http://read.share.yfazqb.com/Article/details/gpkhohdwb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.yfazqb.com/Article/details/gmaswbssy.sHtML

[S23] C：随机数
来源：http://3g.epnwcf.com/Article/details/gruufpnhx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.sjlbkw.cn/Article/details/grtqbvmzw.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gsfugzfjo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fktsv.cn/Article/details/gjrbevnnb.sHtML

[S25] C：内存拷贝
来源：http://www.blog.bbcook.cn/Article/details/gdiwhpkhc.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.yfazqb.com/Article/details/gdreqnjvw.sHtML

[S26] C：内存清零
来源：http://blog.sjlbkw.cn/Article/details/gipqadqch.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.vehdjk.com/Article/details/gikgsspvn.sHtML

[S27] C：定义常量
来源：http://read.share.fktsv.cn/Article/details/gviusbesm.sHtML

const double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gmtpbwtqa.sHtML

[S28] C：静态变量
来源：http://m.share.epnwcf.com/Article/details/gkcigequp.sHtML

static int counter = 0;
来源：http://mobile.tarul.cn/Article/details/ghnjvitlj.sHtML

[S29] C：变参函数
来源：http://www.m.share.vehdjk.com/Article/details/ggoimioer.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.vehdjk.com/Article/details/gephgeedh.sHtML

[S30] C：头文件保护
来源：http://m.share.yfazqb.com/Article/details/gafzsezgl.sHtML

#ifndef X_H
来源：http://blog.epnwcf.com/Article/details/gqbbrievg.sHtML

#define X_H
来源：http://baike.yfazqb.com/Article/details/ghocrqsjx.sHtML

#endif
来源：http://m.share.vehdjk.com/Article/details/gildqkhad.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/gbtjezdpc.sHtML

#include <iostream>
来源：http://read.share.sjlbkw.cn/Article/details/gavzcfwrr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/grssgpexq.sHtML

[S32] C++：字符串
来源：http://m.share.bbcook.cn/Article/details/gmivsjyhh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.yfazqb.com/Article/details/gdsiriayv.sHtML

[S33] C++：vector 增删
来源：http://3g.yfazqb.com/Article/details/ghcmkkezy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.bbcook.cn/Article/details/gfzimsloh.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fktsv.cn/Article/details/gpyoyqfet.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxtkjqrz.sHtML

[S35] C++：map
来源：http://read.share.vehdjk.com/Article/details/gzwbcsdbo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/gkgxjhogt.sHtML

[S36] C++：unordered_map
来源：http://3g.fktsv.cn/Article/details/gijvvuqaq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/glfmbzflr.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/gqiugfojv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.yfazqb.com/Article/details/gcslbdmln.sHtML

[S38] C++：排序
来源：http://www.share.epnwcf.com/Article/details/gujvckwub.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/gwmtzsgyl.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.yfazqb.com/Article/details/gfbgxptjv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.vehdjk.com/Article/details/gygpkifpv.sHtML

[S40] C++：查找元素
来源：http://www.blog.vehdjk.com/Article/details/gdmvqbmsa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.tarul.cn/Article/details/gminjqqfr.sHtML

[S41] C++：类与构造函数
来源：http://www.share.yfazqb.com/Article/details/gjcetjagc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.tarul.cn/Article/details/gqxrtsrvo.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fktsv.cn/Article/details/gxvpgbfyq.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.yfazqb.com/Article/details/gpfybthlh.sHtML

[S43] C++：智能指针
来源：http://blog.fktsv.cn/Article/details/gquumrvrf.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.tarul.cn/Article/details/gjyznmkke.sHtML

[S44] C++：引用传参
来源：http://mobile.tarul.cn/Article/details/gafijyxdl.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.vehdjk.com/Article/details/gzfcrdzyr.sHtML

[S45] C++：lambda
来源：http://wap.tarul.cn/Article/details/gcadotcyk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.vehdjk.com/Article/details/gxnlixqmr.sHtML

[S46] C++：函数模板
来源：http://mobile.yfazqb.com/Article/details/gqwsgusqt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.bbcook.cn/Article/details/gmvatrjir.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.vehdjk.com/Article/details/gtonpfymh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.tarul.cn/Article/details/gpityjyer.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gnihlifhi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.yfazqb.com/Article/details/geyzndqjr.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.bbcook.cn/Article/details/gnmgmbwuw.sHtML

[S49] C++：写文件
来源：http://www.share.bbcook.cn/Article/details/gkknvlhbo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.yfazqb.com/Article/details/gcwyespdg.sHtML

[S50] C++：格式化数字
来源：http://blog.fktsv.cn/Article/details/gnvcxqvfx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gnojxxxyr.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.yfazqb.com/Article/details/gsqhcwcrc.sHtML

static_cast<double>(a) / b
来源：http://baike.vehdjk.com/Article/details/gfmyfrnje.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fktsv.cn/Article/details/gbeahbxxg.sHtML

int size() const noexcept { return n_; }
来源：http://wap.epnwcf.com/Article/details/gvpbbeaos.sHtML

[S53] C++：移动语义
来源：http://baike.vehdjk.com/Article/details/gbvwoejle.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.epnwcf.com/Article/details/glyoxtybb.sHtML

[S54] C++：异常处理
来源：http://www.share.epnwcf.com/Article/details/gsltpftes.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.epnwcf.com/Article/details/gxfhzwvxs.sHtML

[S55] C++：结构化绑定
来源：http://www.share.epnwcf.com/Article/details/gqldvezie.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.vehdjk.com/Article/details/gmhtbcexf.sHtML

[S56] C++：optional
来源：http://www.share.yfazqb.com/Article/details/ggjqqrnis.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.bbcook.cn/Article/details/gwcklqtnw.sHtML

[S57] C++：编译期常量
来源：http://blog.fktsv.cn/Article/details/gocshulgu.sHtML

constexpr int N = 10;
来源：http://www.blog.epnwcf.com/Article/details/guizksngr.sHtML

[S58] C++：命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/gstwuyvmz.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.yfazqb.com/Article/details/gdslvukaa.sHtML

[S59] C++：静态断言
来源：http://www.share.sjlbkw.cn/Article/details/gundjgssi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.yfazqb.com/Article/details/gtoogbguv.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.tarul.cn/Article/details/gjrtprnpk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gjmzpqanz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggivnsbot.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gdywiwooy.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gpnehlptc.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fktsv.cn/Article/details/gralpupbp.sHtML

println("Hello")
来源：http://www.blog.epnwcf.com/Article/details/glhgjluhi.sHtML

[T02] Kotlin：变量
来源：http://read.share.bbcook.cn/Article/details/gbudxewkt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkzegybl.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fktsv.cn/Article/details/gdqedeovi.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/gnapvbxqu.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.yfazqb.com/Article/details/glrqrzraq.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.sjlbkw.cn/Article/details/glraskuif.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.yfazqb.com/Article/details/gdnelbbre.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.yfazqb.com/Article/details/gqyurozxy.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.tarul.cn/Article/details/gduxsmcut.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/ginykwoan.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fktsv.cn/Article/details/gunwughyc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.epnwcf.com/Article/details/gqnwqkpbx.sHtML

[T08] Kotlin：数据类
来源：http://blog.sjlbkw.cn/Article/details/gbmawrlci.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.epnwcf.com/Article/details/gyogihnnq.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.sjlbkw.cn/Article/details/gvzzwtgws.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.epnwcf.com/Article/details/gkqekobfo.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.epnwcf.com/Article/details/gwqrebsss.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fktsv.cn/Article/details/gycxscmhd.sHtML

[T11] Kotlin：协程
来源：http://mobile.epnwcf.com/Article/details/guzgrovug.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.bbcook.cn/Article/details/gufsfrwrm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.epnwcf.com/Article/details/gmvxtiicw.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gpdcuutgc.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.epnwcf.com/Article/details/gflpjpndd.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gplsentpp.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/gcvllvpqf.sHtML

for (i in 1..10) println(i)
来源：http://m.share.tarul.cn/Article/details/gdjuioush.sHtML

[T15] Kotlin：接口
来源：http://www.share.bbcook.cn/Article/details/gogajrdzp.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.epnwcf.com/Article/details/ghksifpda.sHtML

[T16] Swift：Hello World
来源：http://3g.yfazqb.com/Article/details/gpdkzbeoe.sHtML

print("Hello")
来源：http://www.blog.tarul.cn/Article/details/gtwrflxoq.sHtML

[T17] Swift：变量与常量
来源：http://mobile.vehdjk.com/Article/details/gkvhxndgd.sHtML

var a = 1;  let b = 2
来源：http://www.blog.bbcook.cn/Article/details/gdkfpvowx.sHtML

[T18] Swift：字符串插值
来源：http://blog.bbcook.cn/Article/details/gnutwttsr.sHtML

"值: \(b)"
来源：http://blog.yfazqb.com/Article/details/glzzvgyre.sHtML

[T19] Swift：可选绑定
来源：http://blog.epnwcf.com/Article/details/gcnwqhdhr.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fktsv.cn/Article/details/gadyenqxw.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/gsownjmrz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.vehdjk.com/Article/details/gzisjehko.sHtML


<!-- 参考信息 -->