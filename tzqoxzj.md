代发 wailian999

echo "${#s}"
来源：http://read.share.yfazqb.com/Article/details/gebkokthd.sHtML

[R22] 截取子串
来源：http://baike.epnwcf.com/Article/details/gysryxquu.sHtML

echo "${s:0:5}"
来源：http://www.share.epnwcf.com/Article/details/giiskuflo.sHtML

[R23] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gbpcqvuxd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fktsv.cn/Article/details/gvuztxabt.sHtML

[R24] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gshiyxjku.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.yfazqb.com/Article/details/gpasnjxyb.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.tarul.cn/Article/details/ggwowntnt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.yfazqb.com/Article/details/gelantpse.sHtML

[R26] 命令替换
来源：http://blog.tarul.cn/Article/details/goybtkvvv.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fktsv.cn/Article/details/gfidvxqua.sHtML

[R27] 算术展开
来源：http://www.m.share.bbcook.cn/Article/details/gnyucysin.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.epnwcf.com/Article/details/giztvruyb.sHtML

[R28] 浮点运算
来源：http://3g.tarul.cn/Article/details/gmkfpaahd.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.sjlbkw.cn/Article/details/gjfqqghaq.sHtML

[R29] 定义函数
来源：http://mobile.fktsv.cn/Article/details/ggpywpapt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fktsv.cn/Article/details/ginxjzyja.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fktsv.cn/Article/details/gvztespjw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.tarul.cn/Article/details/gsokzzbns.sHtML

[R31] 局部变量
来源：http://baike.vehdjk.com/Article/details/gmiftozit.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fktsv.cn/Article/details/gkczmvuxe.sHtML

[R32] 参数个数校验
来源：http://mobile.vehdjk.com/Article/details/gkxkofcjo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gqqvzeeje.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.sjlbkw.cn/Article/details/gwyhdvoiu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.tarul.cn/Article/details/gduszjrpg.sHtML

[R34] 退出时清理
来源：http://mobile.fktsv.cn/Article/details/gceyjyzvy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gxmcxxxvf.sHtML

[R35] 后台执行并等待
来源：http://blog.vehdjk.com/Article/details/githygmhf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.bbcook.cn/Article/details/ggoyhcvzo.sHtML

[R36] 并发执行多个任务
来源：http://wap.epnwcf.com/Article/details/gmyeqrrjn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.vehdjk.com/Article/details/gqlehqtwg.sHtML

[R37] 把输出赋给变量
来源：http://mobile.sjlbkw.cn/Article/details/gjagghczj.sHtML

files=$(ls -1)
来源：http://3g.yfazqb.com/Article/details/gixeuucaf.sHtML

[R38] 管道串联
来源：http://baike.vehdjk.com/Article/details/gffbwzcbt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.yfazqb.com/Article/details/gjpkcfrss.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fktsv.cn/Article/details/gqaanajxc.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fktsv.cn/Article/details/goourulji.sHtML

[R40] 追加写日志
来源：http://baike.bbcook.cn/Article/details/gwiynasey.sHtML

echo "log" >> out.log
来源：http://www.share.vehdjk.com/Article/details/gljenpfss.sHtML

[R41] 丢弃输出
来源：http://3g.epnwcf.com/Article/details/ggbqaupux.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgqequuh.sHtML

[R42] 输入重定向
来源：http://www.blog.bbcook.cn/Article/details/gasugcidu.sHtML

wc -l < a.txt
来源：http://www.blog.yfazqb.com/Article/details/gndijokmr.sHtML

[R43] 按名字查找文件
来源：http://3g.vehdjk.com/Article/details/gjlrvpjcy.sHtML

find . -name "*.log" -type f
来源：http://read.share.epnwcf.com/Article/details/gqsyaihum.sHtML

[R44] 按修改时间查找
来源：http://www.blog.sjlbkw.cn/Article/details/glyeelngh.sHtML

find . -mtime -7 -type f
来源：http://wap.epnwcf.com/Article/details/gslnnmlos.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/gkazdprcb.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/gvfenoljz.sHtML

[R46] 递归替换文件内容
来源：http://wap.yfazqb.com/Article/details/gtuqhkwyy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.epnwcf.com/Article/details/goncountv.sHtML

[R47] sed 单行替换
来源：http://blog.bbcook.cn/Article/details/gugtamqgw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gbegmdred.sHtML

[R48] awk 取指定列
来源：http://read.share.vehdjk.com/Article/details/gjrretpbr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gfyousxtm.sHtML

[R49] awk 带条件
来源：http://m.share.yfazqb.com/Article/details/gydcuqfwl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.sjlbkw.cn/Article/details/glpofuwdt.sHtML

[R50] awk 求和
来源：http://m.share.vehdjk.com/Article/details/gkermaowk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gyieqetud.sHtML

[R51] 排序去重取前几
来源：http://read.share.sjlbkw.cn/Article/details/grqwxrntu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.epnwcf.com/Article/details/gsirknwcl.sHtML

[R52] 统计行数
来源：http://mobile.vehdjk.com/Article/details/gnqcjhpbo.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/gmmkbcfue.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fktsv.cn/Article/details/glnhuzcch.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.epnwcf.com/Article/details/gqllvexld.sHtML

[R54] 比较两个文件
来源：http://read.share.sjlbkw.cn/Article/details/gljdgargz.sHtML

diff a.txt b.txt
来源：http://www.blog.yfazqb.com/Article/details/gtgclxcwj.sHtML

[R55] 压缩与解压
来源：http://m.share.epnwcf.com/Article/details/gnnieppxj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.bbcook.cn/Article/details/gvtdgvhdf.sHtML

[R56] 远程拷贝
来源：http://wap.tarul.cn/Article/details/gnoeasbxq.sHtML

scp file user@host:/path/
来源：http://www.blog.sjlbkw.cn/Article/details/gdqskjhil.sHtML

[R57] 远程执行命令
来源：http://wap.tarul.cn/Article/details/gfmukcuyd.sHtML

ssh user@host 'uptime'
来源：http://wap.sjlbkw.cn/Article/details/gsftifarf.sHtML

[R58] 下载文件
来源：http://www.blog.tarul.cn/Article/details/gqxpmwdnk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/gqlbrdrow.sHtML

[R59] 发 POST JSON
来源：http://baike.tarul.cn/Article/details/gxvkskicw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.sjlbkw.cn/Article/details/gawbmiwpg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/ggydajwgj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.epnwcf.com/Article/details/gdllcfugp.sHtML

[R61] 磁盘占用
来源：http://baike.vehdjk.com/Article/details/gzbmfquwx.sHtML

df -h;  du -sh *
来源：http://3g.tarul.cn/Article/details/gfekvneka.sHtML

[R62] 找最占空间的文件
来源：http://blog.tarul.cn/Article/details/ggclyarjx.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.vehdjk.com/Article/details/gqviksfat.sHtML

[R63] 内存与进程
来源：http://m.share.bbcook.cn/Article/details/gdazoqgdb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.vehdjk.com/Article/details/gslhwxmpq.sHtML

[R64] 结束进程
来源：http://wap.tarul.cn/Article/details/gybjqadvg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.vehdjk.com/Article/details/grkhirwwy.sHtML

[R65] 查看端口占用
来源：http://m.share.tarul.cn/Article/details/gdkrrsdqv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.sjlbkw.cn/Article/details/glstamapa.sHtML

[R66] 定时任务
来源：http://mobile.vehdjk.com/Article/details/guhyhuutu.sHtML

crontab -e;  crontab -l
来源：http://wap.bbcook.cn/Article/details/gzwhvadqx.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fktsv.cn/Article/details/gumfasggx.sHtML

openssl rand -hex 16
来源：http://baike.vehdjk.com/Article/details/gpulflohs.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/gxlfornuu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.tarul.cn/Article/details/gtgedlosr.sHtML

[R69] 生成随机密码
来源：http://read.share.fktsv.cn/Article/details/gpgunhxhq.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.bbcook.cn/Article/details/gpegeffpw.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gcqomswqc.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fktsv.cn/Article/details/gibheikom.sHtML

[R71] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gwxuwsoqt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.bbcook.cn/Article/details/grnzpyifd.sHtML

[R72] 等待端口就绪
来源：http://wap.epnwcf.com/Article/details/gljsfybwk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gfooyahln.sHtML

[R73] 分割大日志
来源：http://m.share.sjlbkw.cn/Article/details/gsusmfnqz.sHtML

split -l 1000 big.log part_
来源：http://baike.fktsv.cn/Article/details/grzdsqrpg.sHtML

[R74] 批量重命名
来源：http://mobile.fktsv.cn/Article/details/getcgqoor.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.yfazqb.com/Article/details/gzodvpman.sHtML

[R75] 导出环境变量
来源：http://www.blog.yfazqb.com/Article/details/gpcowvqye.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.vehdjk.com/Article/details/gfgstxejf.sHtML

[R76] 使用临时文件
来源：http://mobile.sjlbkw.cn/Article/details/ggixgxzvm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gqddmbcaf.sHtML

[R77] 读取用户输入
来源：http://baike.yfazqb.com/Article/details/gmjrvzeri.sHtML

read -rp "请输入: " ans
来源：http://wap.vehdjk.com/Article/details/ghmhmtzcc.sHtML

[R78] 交互式菜单
来源：http://blog.epnwcf.com/Article/details/gphbxeufd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.vehdjk.com/Article/details/gyheqsojv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.yfazqb.com/Article/details/gfvjyfelr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fktsv.cn/Article/details/ggkchmlaq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fktsv.cn/Article/details/gbeenyzzy.sHtML

time ./run.sh
来源：http://www.blog.epnwcf.com/Article/details/gxjmwrypv.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gmnfjsowc.sHtML

S. C / C++ 专题
来源：http://m.share.yfazqb.com/Article/details/gmproylun.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gohugwmwe.sHtML

[S01] C：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gkfhlbihj.sHtML

#include <stdio.h>
来源：http://www.share.fktsv.cn/Article/details/gpyiuobtc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fktsv.cn/Article/details/gcufbrrco.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.epnwcf.com/Article/details/gffzrzrqg.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fktsv.cn/Article/details/gbedotphk.sHtML

[S03] C：读入整数
来源：http://baike.tarul.cn/Article/details/gmwlvrqyx.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gvwtnuuvs.sHtML

[S04] C：字符串复制
来源：http://wap.sjlbkw.cn/Article/details/girkuxrff.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gkcgzldrq.sHtML

[S05] C：字符串长度
来源：http://blog.bbcook.cn/Article/details/gbuhhifvs.sHtML

strlen(s)
来源：http://www.blog.fktsv.cn/Article/details/glegoekkt.sHtML

[S06] C：字符串比较
来源：http://m.share.epnwcf.com/Article/details/gopvgauzp.sHtML

strcmp(a, b) == 0
来源：http://3g.epnwcf.com/Article/details/gvhyywkiz.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.tarul.cn/Article/details/ggmfhzyql.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.yfazqb.com/Article/details/gyfihemsu.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.tarul.cn/Article/details/gtoodlyhi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fktsv.cn/Article/details/gtlftmgwc.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.bbcook.cn/Article/details/gnrafqelq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.tarul.cn/Article/details/glvvcknoi.sHtML

[S10] C：指针与解引用
来源：http://www.blog.yfazqb.com/Article/details/geioiiqwk.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.bbcook.cn/Article/details/gzwfsqwky.sHtML

[S11] C：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gnsjmhtxp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fktsv.cn/Article/details/gpupvksco.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.epnwcf.com/Article/details/gsstuicma.sHtML

fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gzjibmxbq.sHtML

[S12] C：写文件
来源：http://3g.yfazqb.com/Article/details/gtsoxlunx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.tarul.cn/Article/details/gfdupnuae.sHtML

[S13] C：宏定义
来源：http://mobile.epnwcf.com/Article/details/gvxincbsf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.bbcook.cn/Article/details/gjaxurlzz.sHtML

[S14] C：枚举
来源：http://www.share.vehdjk.com/Article/details/gnxytyggg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.bbcook.cn/Article/details/gzweuyykp.sHtML

[S15] C：类型转换
来源：http://baike.vehdjk.com/Article/details/gftbwteky.sHtML

(double) a / b
来源：http://www.blog.sjlbkw.cn/Article/details/guwzjkgii.sHtML

[S16] C：位操作置位
来源：http://www.m.share.yfazqb.com/Article/details/gfvmkpcni.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/grwmxjaum.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fktsv.cn/Article/details/gusgfdbcb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.vehdjk.com/Article/details/glonlouqz.sHtML

[S18] C：命令行参数
来源：http://m.share.fktsv.cn/Article/details/gjqlujgzq.sHtML

int main(int argc, char **argv)
来源：http://wap.epnwcf.com/Article/details/gwoydafpo.sHtML

[S19] C：快速排序
来源：http://3g.yfazqb.com/Article/details/gjaefgzyd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/giriqmebb.sHtML

[S20] C：二分查找
来源：http://www.blog.sjlbkw.cn/Article/details/gbucspaqq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gejtmycsb.sHtML

[S21] C：字符类别判断
来源：http://www.blog.vehdjk.com/Article/details/grnmdsswa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.epnwcf.com/Article/details/ghnpkhpwk.sHtML

[S22] C：字符串转数字
来源：http://baike.bbcook.cn/Article/details/gkpmklabf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.bbcook.cn/Article/details/gdjhchygn.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/gslgranct.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.sjlbkw.cn/Article/details/gdttvsyls.sHtML

[S24] C：获取本地时间
来源：http://read.share.bbcook.cn/Article/details/gumadptgm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.bbcook.cn/Article/details/guoipvalj.sHtML

[S25] C：内存拷贝
来源：http://blog.epnwcf.com/Article/details/gdkmsacsl.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.vehdjk.com/Article/details/gbayjhmdn.sHtML

[S26] C：内存清零
来源：http://3g.epnwcf.com/Article/details/gglqzqaas.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/gcljuzzbv.sHtML

[S27] C：定义常量
来源：http://blog.sjlbkw.cn/Article/details/gvdfkcdfu.sHtML

const double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gorgwrcje.sHtML

[S28] C：静态变量
来源：http://read.share.tarul.cn/Article/details/gzdcdianw.sHtML

static int counter = 0;
来源：http://www.blog.bbcook.cn/Article/details/gqykjvpgl.sHtML

[S29] C：变参函数
来源：http://wap.bbcook.cn/Article/details/gjwkkwldo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.tarul.cn/Article/details/grmvmnsxd.sHtML

[S30] C：头文件保护
来源：http://mobile.bbcook.cn/Article/details/gammsgpoo.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/gsnjureac.sHtML

#define X_H
来源：http://m.share.sjlbkw.cn/Article/details/gofsujwxt.sHtML

#endif
来源：http://baike.fktsv.cn/Article/details/gngozhhqg.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/gtrwwxuyk.sHtML

#include <iostream>
来源：http://www.share.vehdjk.com/Article/details/gmoxiorkp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.epnwcf.com/Article/details/gxraplyzj.sHtML

[S32] C++：字符串
来源：http://m.share.sjlbkw.cn/Article/details/gwquoyyph.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.yfazqb.com/Article/details/gxsjhwefy.sHtML

[S33] C++：vector 增删
来源：http://www.share.epnwcf.com/Article/details/gqrounjte.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.vehdjk.com/Article/details/gcqdelgcb.sHtML

[S34] C++：遍历 vector
来源：http://www.share.tarul.cn/Article/details/girhghctt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.sjlbkw.cn/Article/details/gfstngvpc.sHtML

[S35] C++：map
来源：http://mobile.sjlbkw.cn/Article/details/gocndctpx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gbqeidplf.sHtML

[S36] C++：unordered_map
来源：http://m.share.fktsv.cn/Article/details/gtqmbrfiy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/ggeabfsvl.sHtML

[S37] C++：set
来源：http://blog.bbcook.cn/Article/details/geoxudqqj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.epnwcf.com/Article/details/gihstaiqb.sHtML

[S38] C++：排序
来源：http://blog.tarul.cn/Article/details/gbmvlubjy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.tarul.cn/Article/details/gmfvuvxcs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.bbcook.cn/Article/details/glzbeleoa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/grqunqefs.sHtML

[S40] C++：查找元素
来源：http://www.blog.sjlbkw.cn/Article/details/gcelbjmpx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.yfazqb.com/Article/details/grnyywvjb.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.vehdjk.com/Article/details/gkoldyhuk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.sjlbkw.cn/Article/details/gnngvgotn.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.vehdjk.com/Article/details/givxjyzvl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.bbcook.cn/Article/details/gfxqmfude.sHtML

[S43] C++：智能指针
来源：http://blog.fktsv.cn/Article/details/glzmexxce.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.yfazqb.com/Article/details/gxizzgtaj.sHtML

[S44] C++：引用传参
来源：http://mobile.bbcook.cn/Article/details/gcyyvrspn.sHtML

void inc(int &x) { ++x; }
来源：http://baike.vehdjk.com/Article/details/gyehbwdte.sHtML

[S45] C++：lambda
来源：http://3g.fktsv.cn/Article/details/gtutswoei.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.sjlbkw.cn/Article/details/ggmptfbmp.sHtML

[S46] C++：函数模板
来源：http://read.share.vehdjk.com/Article/details/gojghxyox.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.vehdjk.com/Article/details/gyaqglzqg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.bbcook.cn/Article/details/gzdegfudj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.yfazqb.com/Article/details/gvktwyxno.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gachoeklt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.sjlbkw.cn/Article/details/gblpomows.sHtML

while (std::getline(in, line)) { }
来源：http://blog.tarul.cn/Article/details/gapgwlxfx.sHtML

[S49] C++：写文件
来源：http://blog.bbcook.cn/Article/details/gdgwkfkte.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.yfazqb.com/Article/details/gvwykpfpe.sHtML

[S50] C++：格式化数字
来源：http://baike.bbcook.cn/Article/details/gotruhbtz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.bbcook.cn/Article/details/gfcgvmpve.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/gejfrlqce.sHtML

static_cast<double>(a) / b
来源：http://www.share.vehdjk.com/Article/details/gwrqhnwmf.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/gzomarjsp.sHtML

int size() const noexcept { return n_; }
来源：http://3g.bbcook.cn/Article/details/gzrdgzufn.sHtML

[S53] C++：移动语义
来源：http://wap.sjlbkw.cn/Article/details/gepoxcgpz.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.tarul.cn/Article/details/gcwkbelwl.sHtML

[S54] C++：异常处理
来源：http://baike.yfazqb.com/Article/details/gmmkqtfjr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.vehdjk.com/Article/details/gxaieqplz.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gzexdvlrv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.tarul.cn/Article/details/gskhknqvc.sHtML

[S56] C++：optional
来源：http://baike.fktsv.cn/Article/details/gnyngvewc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.bbcook.cn/Article/details/glznsekit.sHtML

[S57] C++：编译期常量
来源：http://m.share.tarul.cn/Article/details/godemmend.sHtML

constexpr int N = 10;
来源：http://www.m.share.tarul.cn/Article/details/gyzziargn.sHtML

[S58] C++：命名空间
来源：http://wap.bbcook.cn/Article/details/gnoiuxais.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.yfazqb.com/Article/details/gkhrrlhvi.sHtML

[S59] C++：静态断言
来源：http://m.share.sjlbkw.cn/Article/details/gllkpzrwk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvedejfr.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.tarul.cn/Article/details/godrvxgql.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.vehdjk.com/Article/details/gfwsexqwp.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gkcguepem.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.tarul.cn/Article/details/ggyhshwzz.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gnwkrxadq.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.yfazqb.com/Article/details/grgdoerps.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/ghfpywlfl.sHtML

[T02] Kotlin：变量
来源：http://baike.bbcook.cn/Article/details/goonugasb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/gqqoywmia.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.yfazqb.com/Article/details/gngcjsmji.sHtML

"值: $b"
来源：http://m.share.bbcook.cn/Article/details/gdhdrasvy.sHtML

[T04] Kotlin：空安全
来源：http://read.share.epnwcf.com/Article/details/gpcabipfs.sHtML

val n: String? = null;  n?.length
来源：http://blog.sjlbkw.cn/Article/details/gavblkqka.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.epnwcf.com/Article/details/gmctlaxgj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.yfazqb.com/Article/details/gtuvompas.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.yfazqb.com/Article/details/gmvkacuwx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gdoyarrlx.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.tarul.cn/Article/details/geizfuijw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.bbcook.cn/Article/details/gavpivwvn.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fktsv.cn/Article/details/ggkiymeic.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gunlbjuhi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.sjlbkw.cn/Article/details/golgolooi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.yfazqb.com/Article/details/gsabdwbrt.sHtML

[T10] Kotlin：默认参数
来源：http://baike.vehdjk.com/Article/details/gffnywcrv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.tarul.cn/Article/details/gwwbhchhq.sHtML

[T11] Kotlin：协程
来源：http://www.share.tarul.cn/Article/details/gvkhaqbvu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.vehdjk.com/Article/details/gdzhlogku.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.sjlbkw.cn/Article/details/ghrffonkm.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.yfazqb.com/Article/details/geboptlbj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.epnwcf.com/Article/details/gibxlswxc.sHtML

val m = mapOf("a" to 1)
来源：http://blog.yfazqb.com/Article/details/gyyftikcy.sHtML

[T14] Kotlin：循环
来源：http://wap.yfazqb.com/Article/details/guxixbiod.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fktsv.cn/Article/details/gpwlqebsh.sHtML

[T15] Kotlin：接口
来源：http://www.blog.bbcook.cn/Article/details/geucivkff.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.tarul.cn/Article/details/gpnooosrw.sHtML

[T16] Swift：Hello World
来源：http://3g.sjlbkw.cn/Article/details/grotvtaqj.sHtML

print("Hello")
来源：http://www.share.epnwcf.com/Article/details/gwcuargcq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fktsv.cn/Article/details/gzsvwyohj.sHtML

var a = 1;  let b = 2
来源：http://wap.sjlbkw.cn/Article/details/gwqzyhklg.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gwrqrlrag.sHtML

"值: \(b)"
来源：http://wap.sjlbkw.cn/Article/details/gcgyccmuf.sHtML

[T19] Swift：可选绑定
来源：http://baike.tarul.cn/Article/details/gnevgkvpr.sHtML

if let n = opt { print(n) }
来源：http://blog.bbcook.cn/Article/details/gcotewpdu.sHtML

[T20] Swift：数组操作
来源：http://baike.bbcook.cn/Article/details/gjwfdfyvn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fktsv.cn/Article/details/ghhosrfvp.sHtML

[T21] Swift：遍历
来源：http://baike.sjlbkw.cn/Article/details/gytzaohzy.sHtML

for x in a { print(x) }
来源：http://blog.bbcook.cn/Article/details/gjuvhggbk.sHtML

[T22] Swift：字典
来源：http://www.share.yfazqb.com/Article/details/gilquavmq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fktsv.cn/Article/details/gqvzeyuot.sHtML

[T23] Swift：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gtwinddva.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.yfazqb.com/Article/details/gmovajjfw.sHtML

[T24] Swift：闭包
来源：http://www.m.share.epnwcf.com/Article/details/gakvdzvtn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.epnwcf.com/Article/details/gtoeaenpd.sHtML


<!-- 参考信息 -->