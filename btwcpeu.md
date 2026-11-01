代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.bbcook.cn/Article/details/gdnebzxtc.sHtML

[R34] 退出时清理
来源：http://m.share.epnwcf.com/Article/details/gtazcphaq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/ggewjzjrl.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/ghukvurhv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.bbcook.cn/Article/details/gqpsyhkgi.sHtML

[R36] 并发执行多个任务
来源：http://baike.sjlbkw.cn/Article/details/gtmajhlya.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.yfazqb.com/Article/details/gdwrrcnag.sHtML

[R37] 把输出赋给变量
来源：http://blog.vehdjk.com/Article/details/gnaeqcxld.sHtML

files=$(ls -1)
来源：http://www.blog.yfazqb.com/Article/details/guailxapt.sHtML

[R38] 管道串联
来源：http://mobile.tarul.cn/Article/details/gthsepjjg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fktsv.cn/Article/details/gkoqnqcno.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.vehdjk.com/Article/details/ggdvtepnt.sHtML

cmd > out.log 2>&1
来源：http://m.share.tarul.cn/Article/details/gotargtiv.sHtML

[R40] 追加写日志
来源：http://mobile.fktsv.cn/Article/details/gwkessznt.sHtML

echo "log" >> out.log
来源：http://m.share.tarul.cn/Article/details/gfwpajhrx.sHtML

[R41] 丢弃输出
来源：http://mobile.epnwcf.com/Article/details/ghlwdrtkm.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fktsv.cn/Article/details/gjaqknwru.sHtML

[R42] 输入重定向
来源：http://wap.tarul.cn/Article/details/grxhjrhmv.sHtML

wc -l < a.txt
来源：http://baike.sjlbkw.cn/Article/details/gsjdzaenc.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fktsv.cn/Article/details/gdgaajapv.sHtML

find . -name "*.log" -type f
来源：http://mobile.tarul.cn/Article/details/ghuzkpgbx.sHtML

[R44] 按修改时间查找
来源：http://blog.vehdjk.com/Article/details/gewztyvje.sHtML

find . -mtime -7 -type f
来源：http://baike.epnwcf.com/Article/details/gdhiplxfs.sHtML

[R45] 批量删除
来源：http://m.share.bbcook.cn/Article/details/gppbzqerp.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.sjlbkw.cn/Article/details/glhglemvz.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjrjkjij.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.bbcook.cn/Article/details/gklighqkt.sHtML

[R47] sed 单行替换
来源：http://www.m.share.tarul.cn/Article/details/gpxctvbam.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/guidjhocu.sHtML

[R48] awk 取指定列
来源：http://www.m.share.epnwcf.com/Article/details/gpxsxklen.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.epnwcf.com/Article/details/gdkhgxlqh.sHtML

[R49] awk 带条件
来源：http://3g.yfazqb.com/Article/details/gubjjhzmk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.tarul.cn/Article/details/gyytrqhfx.sHtML

[R50] awk 求和
来源：http://mobile.yfazqb.com/Article/details/gzkzifspw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gptqcjwla.sHtML

[R51] 排序去重取前几
来源：http://read.share.bbcook.cn/Article/details/gspjfkifo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.sjlbkw.cn/Article/details/gaidadpgz.sHtML

[R52] 统计行数
来源：http://blog.fktsv.cn/Article/details/gifcozkpg.sHtML

wc -l a.txt
来源：http://wap.bbcook.cn/Article/details/goflttgdq.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.epnwcf.com/Article/details/ghrvimwss.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fktsv.cn/Article/details/gsvwxbnqo.sHtML

[R54] 比较两个文件
来源：http://3g.vehdjk.com/Article/details/gxmjqdkva.sHtML

diff a.txt b.txt
来源：http://read.share.epnwcf.com/Article/details/gmuhsmola.sHtML

[R55] 压缩与解压
来源：http://read.share.tarul.cn/Article/details/gjqdpvyun.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.epnwcf.com/Article/details/guzhhpyux.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/gcgiprtii.sHtML

scp file user@host:/path/
来源：http://www.m.share.vehdjk.com/Article/details/gygewozfp.sHtML

[R57] 远程执行命令
来源：http://www.share.epnwcf.com/Article/details/gjxnebloc.sHtML

ssh user@host 'uptime'
来源：http://3g.tarul.cn/Article/details/gyymdnktb.sHtML

[R58] 下载文件
来源：http://www.share.bbcook.cn/Article/details/ghkqbsjna.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fktsv.cn/Article/details/gaflhlswu.sHtML

[R59] 发 POST JSON
来源：http://baike.tarul.cn/Article/details/gsybwthea.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fktsv.cn/Article/details/gpwcfisgt.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gqxmzovbb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.tarul.cn/Article/details/gbpiwqehz.sHtML

[R61] 磁盘占用
来源：http://m.share.fktsv.cn/Article/details/gxcxjdibb.sHtML

df -h;  du -sh *
来源：http://wap.bbcook.cn/Article/details/gisyqnsdy.sHtML

[R62] 找最占空间的文件
来源：http://blog.epnwcf.com/Article/details/graoupvtn.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.yfazqb.com/Article/details/gqxxrrvwf.sHtML

[R63] 内存与进程
来源：http://wap.tarul.cn/Article/details/gdqqlbltb.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fktsv.cn/Article/details/gbhkfinpq.sHtML

[R64] 结束进程
来源：http://read.share.bbcook.cn/Article/details/gohyiptcy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.bbcook.cn/Article/details/gpdpyrbxp.sHtML

[R65] 查看端口占用
来源：http://m.share.yfazqb.com/Article/details/ghpkwnviu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.yfazqb.com/Article/details/gsapmbrax.sHtML

[R66] 定时任务
来源：http://baike.epnwcf.com/Article/details/glkunrjhq.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/ghhzjhdyf.sHtML

[R67] 生成随机十六进制串
来源：http://baike.vehdjk.com/Article/details/gitazlxnp.sHtML

openssl rand -hex 16
来源：http://www.blog.epnwcf.com/Article/details/gldgvawad.sHtML

[R68] 计算文件校验值
来源：http://3g.epnwcf.com/Article/details/gmvqdmzeg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.vehdjk.com/Article/details/gbqnqivnx.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fktsv.cn/Article/details/girdiddxh.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.tarul.cn/Article/details/gqmyubfqw.sHtML

[R70] 时间戳与互转
来源：http://m.share.epnwcf.com/Article/details/ggrovbgyh.sHtML

date +%s;  date -d @1700000000
来源：http://blog.tarul.cn/Article/details/gafxnwfgh.sHtML

[R71] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gtloxoort.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.bbcook.cn/Article/details/gcpvvobfr.sHtML

[R72] 等待端口就绪
来源：http://baike.vehdjk.com/Article/details/gpntbhtua.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fktsv.cn/Article/details/gcnhrxmua.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/glnailufu.sHtML

split -l 1000 big.log part_
来源：http://m.share.bbcook.cn/Article/details/gkzirltvn.sHtML

[R74] 批量重命名
来源：http://www.m.share.fktsv.cn/Article/details/gzumuwvlh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/griatmoxo.sHtML

[R75] 导出环境变量
来源：http://wap.vehdjk.com/Article/details/giwzqsbzd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.yfazqb.com/Article/details/gwzqrykzs.sHtML

[R76] 使用临时文件
来源：http://read.share.fktsv.cn/Article/details/gezfmidhq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/gapjwjkjj.sHtML

[R77] 读取用户输入
来源：http://mobile.bbcook.cn/Article/details/ggurctwbr.sHtML

read -rp "请输入: " ans
来源：http://read.share.fktsv.cn/Article/details/gocsqnqmf.sHtML

[R78] 交互式菜单
来源：http://m.share.yfazqb.com/Article/details/gnnyfeits.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.bbcook.cn/Article/details/glkkocdgk.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.bbcook.cn/Article/details/gfvtnxtiv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.sjlbkw.cn/Article/details/ggyayojbk.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.yfazqb.com/Article/details/gaindzcfq.sHtML

time ./run.sh
来源：http://baike.epnwcf.com/Article/details/gmsbfisxi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gjhtmgwfm.sHtML

S. C / C++ 专题
来源：http://mobile.sjlbkw.cn/Article/details/gosgkchgc.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gftsalnpi.sHtML

[S01] C：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/grhjjxebo.sHtML

#include <stdio.h>
来源：http://baike.bbcook.cn/Article/details/gmdjsilod.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.yfazqb.com/Article/details/gpciczmhu.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.bbcook.cn/Article/details/gwdtwlhzg.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fktsv.cn/Article/details/gzkoylxen.sHtML

[S03] C：读入整数
来源：http://3g.fktsv.cn/Article/details/gvftbgjiq.sHtML

int x; scanf("%d", &x);
来源：http://wap.tarul.cn/Article/details/glfumnsmf.sHtML

[S04] C：字符串复制
来源：http://wap.bbcook.cn/Article/details/gjhsqflne.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gkqafpozn.sHtML

[S05] C：字符串长度
来源：http://baike.epnwcf.com/Article/details/gyqgbkdgc.sHtML

strlen(s)
来源：http://www.m.share.fktsv.cn/Article/details/gkfuagasy.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/gekqmbvam.sHtML

strcmp(a, b) == 0
来源：http://m.share.fktsv.cn/Article/details/gdvdkiquz.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fktsv.cn/Article/details/gygicqfdm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.tarul.cn/Article/details/gfbhcaesm.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/gzzesefeb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.sjlbkw.cn/Article/details/ggpdoafze.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.tarul.cn/Article/details/gikucvsgq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.sjlbkw.cn/Article/details/gqcphypkw.sHtML

[S10] C：指针与解引用
来源：http://3g.tarul.cn/Article/details/gswwbtaoh.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.bbcook.cn/Article/details/gvpbppijz.sHtML

[S11] C：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gpdhupihn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.vehdjk.com/Article/details/gkajqpvgy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.epnwcf.com/Article/details/gnahjmyqd.sHtML

fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gdeyxhwzn.sHtML

[S12] C：写文件
来源：http://mobile.bbcook.cn/Article/details/gtacvpzqh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gsorkhzzb.sHtML

[S13] C：宏定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzxsxzhz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.yfazqb.com/Article/details/gcstmpobu.sHtML

[S14] C：枚举
来源：http://blog.epnwcf.com/Article/details/gsiguftwz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/gddkyhpiw.sHtML

[S15] C：类型转换
来源：http://3g.fktsv.cn/Article/details/guxcnybpq.sHtML

(double) a / b
来源：http://baike.bbcook.cn/Article/details/gvlggqwsi.sHtML

[S16] C：位操作置位
来源：http://www.blog.fktsv.cn/Article/details/gkteqkbiq.sHtML

x |= (1 << 3);
来源：http://www.blog.epnwcf.com/Article/details/gpxmqidpn.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gxqivtyyj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.bbcook.cn/Article/details/grytvlffi.sHtML

[S18] C：命令行参数
来源：http://mobile.fktsv.cn/Article/details/gqygctdkm.sHtML

int main(int argc, char **argv)
来源：http://www.blog.sjlbkw.cn/Article/details/gcpgwgscv.sHtML

[S19] C：快速排序
来源：http://www.m.share.vehdjk.com/Article/details/gyxpfpgfl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gjrssnrli.sHtML

[S20] C：二分查找
来源：http://blog.yfazqb.com/Article/details/gepglkgqp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/gkadbpbjh.sHtML

[S21] C：字符类别判断
来源：http://blog.epnwcf.com/Article/details/gboclwvpk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fktsv.cn/Article/details/gghwwbzev.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.bbcook.cn/Article/details/gindivagu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/gajyfrcfp.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/gydoxuxum.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.epnwcf.com/Article/details/gmflnoklp.sHtML

[S24] C：获取本地时间
来源：http://www.share.fktsv.cn/Article/details/gfmeukmmm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.bbcook.cn/Article/details/gbgdeolsh.sHtML

[S25] C：内存拷贝
来源：http://www.share.yfazqb.com/Article/details/gptrxespk.sHtML

memcpy(dst, src, n);
来源：http://read.share.sjlbkw.cn/Article/details/gqgvcfssp.sHtML

[S26] C：内存清零
来源：http://wap.fktsv.cn/Article/details/guyfaqjmj.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.bbcook.cn/Article/details/guyqubxed.sHtML

[S27] C：定义常量
来源：http://3g.sjlbkw.cn/Article/details/gheifmcvi.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gdqomiuqm.sHtML

[S28] C：静态变量
来源：http://m.share.tarul.cn/Article/details/gfnijzgzm.sHtML

static int counter = 0;
来源：http://3g.bbcook.cn/Article/details/grnnqisvj.sHtML

[S29] C：变参函数
来源：http://www.share.bbcook.cn/Article/details/gmiseredi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.bbcook.cn/Article/details/gddpysjpz.sHtML

[S30] C：头文件保护
来源：http://read.share.bbcook.cn/Article/details/gbjrutpho.sHtML

#ifndef X_H
来源：http://www.blog.yfazqb.com/Article/details/gbevrssbk.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/gkpidreuh.sHtML

#endif
来源：http://www.m.share.fktsv.cn/Article/details/gaebskiwd.sHtML

[S31] C++：Hello World
来源：http://www.blog.tarul.cn/Article/details/gqwgtlxdr.sHtML

#include <iostream>
来源：http://3g.bbcook.cn/Article/details/gnmthepem.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gvssqqbzl.sHtML

[S32] C++：字符串
来源：http://mobile.vehdjk.com/Article/details/gpkmwzhyp.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.sjlbkw.cn/Article/details/gwbfoasva.sHtML

[S33] C++：vector 增删
来源：http://mobile.epnwcf.com/Article/details/gqrtfqavm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fktsv.cn/Article/details/gdgouibir.sHtML

[S34] C++：遍历 vector
来源：http://m.share.sjlbkw.cn/Article/details/gxpjzvctg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.tarul.cn/Article/details/glugahodk.sHtML

[S35] C++：map
来源：http://www.share.tarul.cn/Article/details/grulecrpu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gvxhmgtnv.sHtML

[S36] C++：unordered_map
来源：http://mobile.sjlbkw.cn/Article/details/ghnykfdsg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/geyvubmhw.sHtML

[S37] C++：set
来源：http://m.share.epnwcf.com/Article/details/gvrxjcvwz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.epnwcf.com/Article/details/gjyozgeml.sHtML

[S38] C++：排序
来源：http://baike.tarul.cn/Article/details/glzhnwzkm.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.tarul.cn/Article/details/gdghuiolf.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.bbcook.cn/Article/details/geejsdshr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fktsv.cn/Article/details/gwywifwgy.sHtML

[S40] C++：查找元素
来源：http://read.share.vehdjk.com/Article/details/gxgqsftxs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.epnwcf.com/Article/details/gjpqmoiau.sHtML

[S41] C++：类与构造函数
来源：http://wap.yfazqb.com/Article/details/gmszhggmr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.vehdjk.com/Article/details/gksqrzwxf.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.vehdjk.com/Article/details/gzikisslj.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.tarul.cn/Article/details/gsphojfju.sHtML

[S43] C++：智能指针
来源：http://read.share.fktsv.cn/Article/details/ghmpfrhiw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gwnnvtxpu.sHtML

[S44] C++：引用传参
来源：http://wap.tarul.cn/Article/details/gaobfvvnt.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.sjlbkw.cn/Article/details/gymdfzlkh.sHtML

[S45] C++：lambda
来源：http://m.share.vehdjk.com/Article/details/gltaahpxv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gcugtuigx.sHtML

[S46] C++：函数模板
来源：http://blog.epnwcf.com/Article/details/gzsjwfkuc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.vehdjk.com/Article/details/gsqsztfzq.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.sjlbkw.cn/Article/details/gdnktzivn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.epnwcf.com/Article/details/gpjftspzk.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gdmzjutxb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.yfazqb.com/Article/details/gjgmesysc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.bbcook.cn/Article/details/gpawvccxr.sHtML

[S49] C++：写文件
来源：http://www.share.tarul.cn/Article/details/gewmjfwbw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.sjlbkw.cn/Article/details/gnkcfsetc.sHtML

[S50] C++：格式化数字
来源：http://3g.bbcook.cn/Article/details/gxabswbti.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.epnwcf.com/Article/details/gbmvhfpto.sHtML

[S51] C++：显式类型转换
来源：http://m.share.epnwcf.com/Article/details/ghvyzzkuq.sHtML

static_cast<double>(a) / b
来源：http://blog.sjlbkw.cn/Article/details/gsadqvbnh.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.tarul.cn/Article/details/gsauffxsm.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.yfazqb.com/Article/details/gbjtbsbmy.sHtML

[S53] C++：移动语义
来源：http://blog.fktsv.cn/Article/details/guysvugei.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.epnwcf.com/Article/details/gbmvkoaux.sHtML

[S54] C++：异常处理
来源：http://read.share.fktsv.cn/Article/details/gckvevzsz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.vehdjk.com/Article/details/gjdamsqyt.sHtML

[S55] C++：结构化绑定
来源：http://wap.fktsv.cn/Article/details/gpsvkxhyr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.yfazqb.com/Article/details/gocxsjblp.sHtML

[S56] C++：optional
来源：http://mobile.bbcook.cn/Article/details/gphrkznfs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.bbcook.cn/Article/details/gtfmyazln.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/gkllwjgid.sHtML

constexpr int N = 10;
来源：http://blog.epnwcf.com/Article/details/ghwhfswhe.sHtML

[S58] C++：命名空间
来源：http://wap.vehdjk.com/Article/details/gzpoqrwpu.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.epnwcf.com/Article/details/glffmsfjr.sHtML

[S59] C++：静态断言
来源：http://www.share.tarul.cn/Article/details/gnhoqevwi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.bbcook.cn/Article/details/ghgpwqywh.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.yfazqb.com/Article/details/ghitzqipb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbrxvpju.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/geqbbfmlo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.tarul.cn/Article/details/ghehplzfm.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ggsinzqjy.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fktsv.cn/Article/details/gbutristh.sHtML

println("Hello")
来源：http://mobile.epnwcf.com/Article/details/gfsiteope.sHtML

[T02] Kotlin：变量
来源：http://read.share.bbcook.cn/Article/details/gdyhzsdez.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.tarul.cn/Article/details/gihnqwooh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.bbcook.cn/Article/details/gibmxaceq.sHtML

"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/glfhkwrpu.sHtML

[T04] Kotlin：空安全
来源：http://www.share.bbcook.cn/Article/details/ghsedxqye.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gksrjspce.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.sjlbkw.cn/Article/details/gkobdwuym.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.yfazqb.com/Article/details/gwtpotkxk.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.yfazqb.com/Article/details/gkcfolcxq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gejvggbvi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gpeyzgtjc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.epnwcf.com/Article/details/goskupiyo.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fktsv.cn/Article/details/gzihmnuot.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.vehdjk.com/Article/details/gfrjplmct.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/gkaaudida.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.epnwcf.com/Article/details/giqvyqquw.sHtML

[T10] Kotlin：默认参数
来源：http://wap.vehdjk.com/Article/details/gvwbomwbm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.vehdjk.com/Article/details/gcjuccwkx.sHtML

[T11] Kotlin：协程
来源：http://wap.yfazqb.com/Article/details/grfnczgkg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.yfazqb.com/Article/details/gqncaoqmo.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.vehdjk.com/Article/details/gbhauzilt.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gabsnmvha.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.yfazqb.com/Article/details/gfdhiyzvz.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fktsv.cn/Article/details/gdrhhtubl.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.bbcook.cn/Article/details/gqjfzeuaa.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fktsv.cn/Article/details/gjudpueyh.sHtML

[T15] Kotlin：接口
来源：http://read.share.fktsv.cn/Article/details/gtbqrstzx.sHtML

interface Shape { fun area(): Double }
来源：http://3g.vehdjk.com/Article/details/gqtchbiky.sHtML

[T16] Swift：Hello World
来源：http://wap.tarul.cn/Article/details/gfafzqwha.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gkdfpmlcg.sHtML

[T17] Swift：变量与常量
来源：http://wap.epnwcf.com/Article/details/gexjzhtfi.sHtML

var a = 1;  let b = 2
来源：http://www.blog.yfazqb.com/Article/details/gmgcfvphm.sHtML

[T18] Swift：字符串插值
来源：http://3g.vehdjk.com/Article/details/gcbztqtgn.sHtML

"值: \(b)"
来源：http://read.share.fktsv.cn/Article/details/gxkdihmts.sHtML

[T19] Swift：可选绑定
来源：http://wap.tarul.cn/Article/details/gouisqwwh.sHtML

if let n = opt { print(n) }
来源：http://wap.sjlbkw.cn/Article/details/guaadqcmf.sHtML

[T20] Swift：数组操作
来源：http://3g.epnwcf.com/Article/details/gwldcpdbv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.bbcook.cn/Article/details/gbswuziko.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gekffrpsu.sHtML

for x in a { print(x) }
来源：http://www.m.share.bbcook.cn/Article/details/gmpmqfbyo.sHtML

[T22] Swift：字典
来源：http://blog.epnwcf.com/Article/details/gkcczceie.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.epnwcf.com/Article/details/ggwawmzrz.sHtML

[T23] Swift：函数
来源：http://wap.sjlbkw.cn/Article/details/gmfdzifip.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.bbcook.cn/Article/details/gmwlsslcl.sHtML

[T24] Swift：闭包
来源：http://wap.epnwcf.com/Article/details/gocatdnpt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gseklmgxl.sHtML

[T25] Swift：结构体
来源：http://www.m.share.sjlbkw.cn/Article/details/gkylojeez.sHtML

struct P { var x: Int }
来源：http://m.share.fktsv.cn/Article/details/gmayugkfh.sHtML

[T26] Swift：类与重写
来源：http://www.share.fktsv.cn/Article/details/gvpzjttba.sHtML

class A: Base { override func f() {} }
来源：http://baike.bbcook.cn/Article/details/ghyxfzuti.sHtML

[T27] Swift：错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gmxmwgees.sHtML

do { try f() } catch { print(error) }
来源：http://blog.epnwcf.com/Article/details/gimrevayv.sHtML

[T28] Swift：枚举
来源：http://m.share.yfazqb.com/Article/details/gwpwnmegl.sHtML

enum Color { case red, green }
来源：http://m.share.bbcook.cn/Article/details/gpshtaouy.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.tarul.cn/Article/details/gshcpnhkp.sHtML

guard let x = opt else { return }
来源：http://3g.sjlbkw.cn/Article/details/gchehbzmq.sHtML

[T30] Swift：协议
来源：http://www.share.vehdjk.com/Article/details/gclrexdzc.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.vehdjk.com/Article/details/ggbwzxlln.sHtML

[T31] Lua：Hello World
来源：http://blog.vehdjk.com/Article/details/gzztnxpqf.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gztkxrgtd.sHtML

[T32] Lua：局部变量
来源：http://www.share.epnwcf.com/Article/details/grifofiln.sHtML

local a = 1
来源：http://blog.yfazqb.com/Article/details/gftticavy.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.epnwcf.com/Article/details/grbfniwmk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.epnwcf.com/Article/details/gdclmrcpl.sHtML

[T34] Lua：遍历表
来源：http://blog.tarul.cn/Article/details/gjovgnadb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fktsv.cn/Article/details/gemufmlyc.sHtML

[T35] Lua：字典表
来源：http://baike.epnwcf.com/Article/details/gsramqlsz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.vehdjk.com/Article/details/gdbeouzmu.sHtML

[T36] Lua：函数
来源：http://3g.fktsv.cn/Article/details/gcxtlszkv.sHtML

function add(a, b) return a + b end
来源：http://wap.tarul.cn/Article/details/gzwucokvs.sHtML


<!-- 参考信息 -->