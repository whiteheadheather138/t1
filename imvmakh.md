代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fktsv.cn/Article/details/gpjcrtltb.sHtML

[R34] 退出时清理
来源：http://www.share.fktsv.cn/Article/details/gkrczsuga.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gpkyrehai.sHtML

[R35] 后台执行并等待
来源：http://blog.epnwcf.com/Article/details/gqeohlxwd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.yfazqb.com/Article/details/gvdvigjwh.sHtML

[R36] 并发执行多个任务
来源：http://3g.sjlbkw.cn/Article/details/gaakdfqyp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.tarul.cn/Article/details/gcjujsset.sHtML

[R37] 把输出赋给变量
来源：http://read.share.sjlbkw.cn/Article/details/ganwvbevs.sHtML

files=$(ls -1)
来源：http://baike.tarul.cn/Article/details/gpigkeneb.sHtML

[R38] 管道串联
来源：http://www.m.share.fktsv.cn/Article/details/gflptznsk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fktsv.cn/Article/details/gbqclobjg.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.bbcook.cn/Article/details/gukikcbfm.sHtML

cmd > out.log 2>&1
来源：http://m.share.epnwcf.com/Article/details/gjttsjsmc.sHtML

[R40] 追加写日志
来源：http://read.share.tarul.cn/Article/details/gozgmxtww.sHtML

echo "log" >> out.log
来源：http://3g.epnwcf.com/Article/details/gzpunnenj.sHtML

[R41] 丢弃输出
来源：http://3g.fktsv.cn/Article/details/gtzadzqra.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.vehdjk.com/Article/details/gkuxvwwhs.sHtML

[R42] 输入重定向
来源：http://mobile.epnwcf.com/Article/details/gchzntqtj.sHtML

wc -l < a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrhzhspu.sHtML

[R43] 按名字查找文件
来源：http://blog.fktsv.cn/Article/details/gonhnzhzb.sHtML

find . -name "*.log" -type f
来源：http://baike.epnwcf.com/Article/details/grppedxax.sHtML

[R44] 按修改时间查找
来源：http://www.share.tarul.cn/Article/details/gbuxmqpmj.sHtML

find . -mtime -7 -type f
来源：http://baike.tarul.cn/Article/details/glcvdhvvv.sHtML

[R45] 批量删除
来源：http://m.share.fktsv.cn/Article/details/glcfekcyg.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fktsv.cn/Article/details/gkvhzazoz.sHtML

[R46] 递归替换文件内容
来源：http://m.share.sjlbkw.cn/Article/details/gqhkyeufs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.sjlbkw.cn/Article/details/gohjliqkg.sHtML

[R47] sed 单行替换
来源：http://www.m.share.tarul.cn/Article/details/gyhlecrdc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.bbcook.cn/Article/details/gseerkiiw.sHtML

[R48] awk 取指定列
来源：http://www.share.bbcook.cn/Article/details/gulqimsog.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gvzqlzuwm.sHtML

[R49] awk 带条件
来源：http://www.m.share.yfazqb.com/Article/details/gamglqmwa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.epnwcf.com/Article/details/ghwbrealj.sHtML

[R50] awk 求和
来源：http://mobile.epnwcf.com/Article/details/giitpkxkh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gmcthgpbv.sHtML

[R51] 排序去重取前几
来源：http://m.share.fktsv.cn/Article/details/gnxeotlpb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.tarul.cn/Article/details/gjrtpbzmj.sHtML

[R52] 统计行数
来源：http://3g.yfazqb.com/Article/details/gcraodvqo.sHtML

wc -l a.txt
来源：http://m.share.epnwcf.com/Article/details/gdjcqliev.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.vehdjk.com/Article/details/gncemzoez.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.tarul.cn/Article/details/gprpqlwlk.sHtML

[R54] 比较两个文件
来源：http://www.blog.epnwcf.com/Article/details/gnrxrorhe.sHtML

diff a.txt b.txt
来源：http://baike.vehdjk.com/Article/details/gwurbiifu.sHtML

[R55] 压缩与解压
来源：http://m.share.sjlbkw.cn/Article/details/gfchcqoyt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.epnwcf.com/Article/details/gdrliwtig.sHtML

[R56] 远程拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gvshkdkmd.sHtML

scp file user@host:/path/
来源：http://www.m.share.tarul.cn/Article/details/gstzjvgqa.sHtML

[R57] 远程执行命令
来源：http://wap.yfazqb.com/Article/details/gyqsjchyf.sHtML

ssh user@host 'uptime'
来源：http://mobile.fktsv.cn/Article/details/ghgygouzy.sHtML

[R58] 下载文件
来源：http://mobile.yfazqb.com/Article/details/gdlzkugmm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.yfazqb.com/Article/details/gqxaaatzh.sHtML

[R59] 发 POST JSON
来源：http://blog.tarul.cn/Article/details/gprsodmwk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fktsv.cn/Article/details/gwtqryukj.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/ggjlpfyhf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.yfazqb.com/Article/details/gbmwasaxz.sHtML

[R61] 磁盘占用
来源：http://www.blog.bbcook.cn/Article/details/glyfaegld.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/guqggiqxd.sHtML

[R62] 找最占空间的文件
来源：http://3g.fktsv.cn/Article/details/gvyrbaiyj.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.sjlbkw.cn/Article/details/gmvyftlvu.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/gcljbwnyn.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.epnwcf.com/Article/details/gtukqpqdf.sHtML

[R64] 结束进程
来源：http://www.m.share.bbcook.cn/Article/details/gzgfrqbfo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.bbcook.cn/Article/details/gsfalfgvt.sHtML

[R65] 查看端口占用
来源：http://wap.sjlbkw.cn/Article/details/gmqcwtsyd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.sjlbkw.cn/Article/details/gdwqkvszu.sHtML

[R66] 定时任务
来源：http://3g.fktsv.cn/Article/details/gnidahemd.sHtML

crontab -e;  crontab -l
来源：http://3g.fktsv.cn/Article/details/gtmmblazk.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fktsv.cn/Article/details/gisrlpueq.sHtML

openssl rand -hex 16
来源：http://read.share.sjlbkw.cn/Article/details/gdsxwjacm.sHtML

[R68] 计算文件校验值
来源：http://read.share.fktsv.cn/Article/details/gtkyfcwjv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/gilqvvivp.sHtML

[R69] 生成随机密码
来源：http://mobile.sjlbkw.cn/Article/details/gplcquhpl.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.tarul.cn/Article/details/gcxqlynsk.sHtML

[R70] 时间戳与互转
来源：http://3g.sjlbkw.cn/Article/details/gcszhprla.sHtML

date +%s;  date -d @1700000000
来源：http://3g.sjlbkw.cn/Article/details/gyewxdlvk.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gxuufwhsp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.sjlbkw.cn/Article/details/gqheajqhv.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fktsv.cn/Article/details/gndsalpli.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/gkxfnhyaz.sHtML

[R73] 分割大日志
来源：http://www.m.share.vehdjk.com/Article/details/gcyrhdhtg.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.sjlbkw.cn/Article/details/guseofwot.sHtML

[R74] 批量重命名
来源：http://www.share.sjlbkw.cn/Article/details/gvytbmcui.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.tarul.cn/Article/details/gyfoheptp.sHtML

[R75] 导出环境变量
来源：http://mobile.vehdjk.com/Article/details/gujvpbcrm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.sjlbkw.cn/Article/details/gewyoncpw.sHtML

[R76] 使用临时文件
来源：http://www.share.yfazqb.com/Article/details/gyhxzqabd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gudiivzzs.sHtML

[R77] 读取用户输入
来源：http://blog.epnwcf.com/Article/details/guexplbnr.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.vehdjk.com/Article/details/gmdddgyiv.sHtML

[R78] 交互式菜单
来源：http://read.share.fktsv.cn/Article/details/gbisniwvc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.bbcook.cn/Article/details/groqtfmii.sHtML

[R79] 解析命令行选项
来源：http://read.share.tarul.cn/Article/details/guvkmdvxq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/ghotimrhz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.epnwcf.com/Article/details/gbiqxwnbo.sHtML

time ./run.sh
来源：http://blog.fktsv.cn/Article/details/gavhplqeo.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glxvygytv.sHtML

S. C / C++ 专题
来源：http://www.m.share.fktsv.cn/Article/details/gunjzvcfi.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/geiqxmjaa.sHtML

[S01] C：Hello World
来源：http://mobile.tarul.cn/Article/details/gzmpvoqug.sHtML

#include <stdio.h>
来源：http://wap.fktsv.cn/Article/details/ghmzspncd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbqziwdtw.sHtML

[S02] C：变量与格式化输出
来源：http://blog.sjlbkw.cn/Article/details/gcflufxzx.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.vehdjk.com/Article/details/gugbdtkbi.sHtML

[S03] C：读入整数
来源：http://baike.epnwcf.com/Article/details/gxbppruef.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.bbcook.cn/Article/details/gtdgdlqwf.sHtML

[S04] C：字符串复制
来源：http://www.share.fktsv.cn/Article/details/gqwejfxqg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.bbcook.cn/Article/details/gduklwjuj.sHtML

[S05] C：字符串长度
来源：http://blog.yfazqb.com/Article/details/gknkzldti.sHtML

strlen(s)
来源：http://www.m.share.fktsv.cn/Article/details/glxttscuk.sHtML

[S06] C：字符串比较
来源：http://mobile.epnwcf.com/Article/details/gubmbnhyf.sHtML

strcmp(a, b) == 0
来源：http://baike.sjlbkw.cn/Article/details/gpptvjeor.sHtML

[S07] C：数组遍历求和
来源：http://baike.fktsv.cn/Article/details/gaoivlkrc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fktsv.cn/Article/details/gujoxiqoc.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.epnwcf.com/Article/details/gadvqyrvm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.yfazqb.com/Article/details/glrfhsrhp.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.sjlbkw.cn/Article/details/gxfepnnxy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.yfazqb.com/Article/details/gllocqufg.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gaglaazjj.sHtML

int *p = &a;  *p = 5;
来源：http://baike.vehdjk.com/Article/details/gnzmbghbs.sHtML

[S11] C：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gnuhzvlcb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.bbcook.cn/Article/details/gmtvxiluh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.sjlbkw.cn/Article/details/gwysbtpnj.sHtML

fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gcpbyxcjs.sHtML

[S12] C：写文件
来源：http://blog.tarul.cn/Article/details/geohzymgu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.yfazqb.com/Article/details/gztlkhogl.sHtML

[S13] C：宏定义
来源：http://www.share.tarul.cn/Article/details/gjkvqjitr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.vehdjk.com/Article/details/getvywijq.sHtML

[S14] C：枚举
来源：http://blog.tarul.cn/Article/details/gudvsyont.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.sjlbkw.cn/Article/details/gybalugqq.sHtML

[S15] C：类型转换
来源：http://www.share.fktsv.cn/Article/details/gmeqawfen.sHtML

(double) a / b
来源：http://mobile.fktsv.cn/Article/details/gdnizlxuv.sHtML

[S16] C：位操作置位
来源：http://www.share.tarul.cn/Article/details/gawhvxmrk.sHtML

x |= (1 << 3);
来源：http://www.blog.fktsv.cn/Article/details/gkjznvxni.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/grzvtbdbs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.sjlbkw.cn/Article/details/gdlozyuzn.sHtML

[S18] C：命令行参数
来源：http://www.blog.fktsv.cn/Article/details/gpsilfiks.sHtML

int main(int argc, char **argv)
来源：http://wap.vehdjk.com/Article/details/ghysomuyi.sHtML

[S19] C：快速排序
来源：http://baike.epnwcf.com/Article/details/gzawhivsk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gtxckkgen.sHtML

[S20] C：二分查找
来源：http://baike.yfazqb.com/Article/details/gtxrudhvi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/ggvznmxan.sHtML

[S21] C：字符类别判断
来源：http://read.share.yfazqb.com/Article/details/gplsxjezj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.tarul.cn/Article/details/goixzhouo.sHtML

[S22] C：字符串转数字
来源：http://www.share.yfazqb.com/Article/details/gitdhepow.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.bbcook.cn/Article/details/gcvmhhklj.sHtML

[S23] C：随机数
来源：http://mobile.epnwcf.com/Article/details/gwvxctbxp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.vehdjk.com/Article/details/ggebwirxs.sHtML

[S24] C：获取本地时间
来源：http://www.blog.epnwcf.com/Article/details/gpsyzncyl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/gialkrvnw.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gywatjhqh.sHtML

memcpy(dst, src, n);
来源：http://wap.vehdjk.com/Article/details/gnudliqmr.sHtML

[S26] C：内存清零
来源：http://www.m.share.bbcook.cn/Article/details/gomgzemfd.sHtML

memset(a, 0, sizeof a);
来源：http://blog.epnwcf.com/Article/details/gjmytgctf.sHtML

[S27] C：定义常量
来源：http://m.share.vehdjk.com/Article/details/gkzdxymvv.sHtML

const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/ghgwhfiqd.sHtML

[S28] C：静态变量
来源：http://mobile.sjlbkw.cn/Article/details/gedivhujt.sHtML

static int counter = 0;
来源：http://baike.tarul.cn/Article/details/gxilyjfyv.sHtML

[S29] C：变参函数
来源：http://mobile.yfazqb.com/Article/details/gwzyjgbhu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fktsv.cn/Article/details/giadloagp.sHtML

[S30] C：头文件保护
来源：http://read.share.epnwcf.com/Article/details/giuwwfabd.sHtML

#ifndef X_H
来源：http://www.share.epnwcf.com/Article/details/gwvtgbcyk.sHtML

#define X_H
来源：http://3g.bbcook.cn/Article/details/gsxljkaga.sHtML

#endif
来源：http://blog.sjlbkw.cn/Article/details/gfrhjdwft.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gjciwulgb.sHtML

#include <iostream>
来源：http://blog.sjlbkw.cn/Article/details/ggqxiobem.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/glnusszko.sHtML

[S32] C++：字符串
来源：http://wap.tarul.cn/Article/details/gelatxjnj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.epnwcf.com/Article/details/gzxkggkxq.sHtML

[S33] C++：vector 增删
来源：http://baike.yfazqb.com/Article/details/gclfpvtnr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.epnwcf.com/Article/details/gufdaopzk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.epnwcf.com/Article/details/gpoavxzbw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.tarul.cn/Article/details/gkqijhvlp.sHtML

[S35] C++：map
来源：http://www.share.sjlbkw.cn/Article/details/gdduovpqi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gtkgojjfk.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.yfazqb.com/Article/details/gsmoajtbg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gzbvdozys.sHtML

[S37] C++：set
来源：http://mobile.bbcook.cn/Article/details/gfajzxnup.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.tarul.cn/Article/details/gdywwzbxw.sHtML

[S38] C++：排序
来源：http://3g.bbcook.cn/Article/details/guleomlph.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.bbcook.cn/Article/details/gbhqajgar.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fktsv.cn/Article/details/gjklhtrpy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.epnwcf.com/Article/details/ghvuicxnc.sHtML

[S40] C++：查找元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnmauuth.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.epnwcf.com/Article/details/gimdygyhu.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.epnwcf.com/Article/details/gvqnsdkou.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fktsv.cn/Article/details/gqpexvble.sHtML

[S42] C++：继承与虚函数
来源：http://3g.vehdjk.com/Article/details/gnhaowjwx.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.yfazqb.com/Article/details/grngujcvz.sHtML

[S43] C++：智能指针
来源：http://wap.tarul.cn/Article/details/gyrptwjvx.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.epnwcf.com/Article/details/ggdjwfzfo.sHtML

[S44] C++：引用传参
来源：http://mobile.tarul.cn/Article/details/gaylzymaq.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.bbcook.cn/Article/details/gtadottxp.sHtML

[S45] C++：lambda
来源：http://read.share.fktsv.cn/Article/details/gmfdwgxty.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.bbcook.cn/Article/details/goyicyzqf.sHtML

[S46] C++：函数模板
来源：http://www.blog.vehdjk.com/Article/details/ggprsavpn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.yfazqb.com/Article/details/grfziohdw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gutssptgs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fktsv.cn/Article/details/givooschf.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gaaurrbcc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.tarul.cn/Article/details/gfzxgpqpk.sHtML

while (std::getline(in, line)) { }
来源：http://blog.epnwcf.com/Article/details/gpigphwrr.sHtML

[S49] C++：写文件
来源：http://mobile.vehdjk.com/Article/details/grzjrmxvu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.tarul.cn/Article/details/gancegmcw.sHtML

[S50] C++：格式化数字
来源：http://wap.vehdjk.com/Article/details/gylfgdxoe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gwzeqzhxc.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/ghnlqlfam.sHtML

static_cast<double>(a) / b
来源：http://m.share.tarul.cn/Article/details/gafnfgbqs.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.epnwcf.com/Article/details/gfcmcqzje.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.vehdjk.com/Article/details/gcpatfdbk.sHtML

[S53] C++：移动语义
来源：http://read.share.fktsv.cn/Article/details/gbqjxoedk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.sjlbkw.cn/Article/details/gvalfuhog.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fktsv.cn/Article/details/gehmlgzrd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fktsv.cn/Article/details/gujrkeoxa.sHtML

[S55] C++：结构化绑定
来源：http://mobile.sjlbkw.cn/Article/details/gpzjauqvp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.bbcook.cn/Article/details/gldrhthhl.sHtML

[S56] C++：optional
来源：http://mobile.epnwcf.com/Article/details/gjdrpruny.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fktsv.cn/Article/details/gyjlarzws.sHtML

[S57] C++：编译期常量
来源：http://read.share.bbcook.cn/Article/details/gmzutttbd.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/goencovcy.sHtML

[S58] C++：命名空间
来源：http://mobile.vehdjk.com/Article/details/gpghbfiue.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.bbcook.cn/Article/details/gcpnhojfe.sHtML

[S59] C++：静态断言
来源：http://wap.yfazqb.com/Article/details/gkyxahsui.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.sjlbkw.cn/Article/details/gtkuxrlgu.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fktsv.cn/Article/details/glxnhuxun.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/gueipqtzs.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghfqttnmk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fktsv.cn/Article/details/gjrmgkbob.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gwdrratvr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.epnwcf.com/Article/details/gbfosqjac.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/gdakhrhuj.sHtML

[T02] Kotlin：变量
来源：http://m.share.bbcook.cn/Article/details/gcpzyjmtr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.yfazqb.com/Article/details/gtuokmkva.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/gkkzedsdq.sHtML

"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gklrftywi.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.tarul.cn/Article/details/gylfuruyf.sHtML

val n: String? = null;  n?.length
来源：http://read.share.epnwcf.com/Article/details/ggpfzadrt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.yfazqb.com/Article/details/gfynvijcq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.vehdjk.com/Article/details/gfdgospdb.sHtML

[T06] Kotlin：集合映射
来源：http://baike.vehdjk.com/Article/details/ghopoevzj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gyefalaid.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gwmihggdr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.epnwcf.com/Article/details/gpwcwavcb.sHtML

[T08] Kotlin：数据类
来源：http://www.share.yfazqb.com/Article/details/gdcutbbgj.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fktsv.cn/Article/details/goaltouia.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.epnwcf.com/Article/details/gbzoigxbf.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.epnwcf.com/Article/details/glawdbyiu.sHtML

[T10] Kotlin：默认参数
来源：http://baike.sjlbkw.cn/Article/details/gbzvqgfis.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.epnwcf.com/Article/details/grbkfrvlq.sHtML

[T11] Kotlin：协程
来源：http://m.share.fktsv.cn/Article/details/gahicgapy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.tarul.cn/Article/details/ghbaglwkh.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fktsv.cn/Article/details/gpauosbnr.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.epnwcf.com/Article/details/gsporuqrf.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.vehdjk.com/Article/details/gwdmswwdb.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.tarul.cn/Article/details/gzhmhaseq.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhzaowsv.sHtML

for (i in 1..10) println(i)
来源：http://www.share.yfazqb.com/Article/details/gqqwylvov.sHtML

[T15] Kotlin：接口
来源：http://wap.tarul.cn/Article/details/gzoklmgcg.sHtML

interface Shape { fun area(): Double }
来源：http://baike.epnwcf.com/Article/details/gvoxlgvik.sHtML

[T16] Swift：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gdkcdumfk.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/grhvycfvj.sHtML

[T17] Swift：变量与常量
来源：http://blog.sjlbkw.cn/Article/details/gmayygyus.sHtML

var a = 1;  let b = 2
来源：http://www.share.tarul.cn/Article/details/gdvddopwc.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gnrpfcfkc.sHtML

"值: \(b)"
来源：http://m.share.vehdjk.com/Article/details/glrdssdot.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/gthmcdfsq.sHtML

if let n = opt { print(n) }
来源：http://baike.yfazqb.com/Article/details/gndgebmtm.sHtML

[T20] Swift：数组操作
来源：http://read.share.fktsv.cn/Article/details/gkifajtkz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.tarul.cn/Article/details/ghjytkepa.sHtML

[T21] Swift：遍历
来源：http://read.share.tarul.cn/Article/details/gijfwdrbs.sHtML

for x in a { print(x) }
来源：http://mobile.tarul.cn/Article/details/gdnvmsmet.sHtML

[T22] Swift：字典
来源：http://www.share.fktsv.cn/Article/details/gsmnxeubb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.yfazqb.com/Article/details/gboyqwriq.sHtML

[T23] Swift：函数
来源：http://blog.sjlbkw.cn/Article/details/gntlmpouf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.yfazqb.com/Article/details/gdcoklout.sHtML

[T24] Swift：闭包
来源：http://mobile.vehdjk.com/Article/details/gukdgxfpf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gzrgpydaj.sHtML

[T25] Swift：结构体
来源：http://read.share.fktsv.cn/Article/details/ghiikcbqq.sHtML

struct P { var x: Int }
来源：http://www.blog.fktsv.cn/Article/details/glhnuoncz.sHtML

[T26] Swift：类与重写
来源：http://blog.tarul.cn/Article/details/gfycrjrxf.sHtML

class A: Base { override func f() {} }
来源：http://www.share.yfazqb.com/Article/details/gufeogwdf.sHtML

[T27] Swift：错误处理
来源：http://www.blog.vehdjk.com/Article/details/ggwwugyvc.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fktsv.cn/Article/details/gyqdmdafd.sHtML

[T28] Swift：枚举
来源：http://m.share.yfazqb.com/Article/details/gnqrwpmcs.sHtML

enum Color { case red, green }
来源：http://read.share.vehdjk.com/Article/details/giqakitfm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/giubugiso.sHtML

guard let x = opt else { return }
来源：http://mobile.bbcook.cn/Article/details/gnncflvkf.sHtML

[T30] Swift：协议
来源：http://www.blog.sjlbkw.cn/Article/details/goeqodolg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.tarul.cn/Article/details/gppffsrlb.sHtML

[T31] Lua：Hello World
来源：http://www.share.vehdjk.com/Article/details/ghrdypumh.sHtML

print("Hello")
来源：http://www.blog.tarul.cn/Article/details/gapykdwsj.sHtML

[T32] Lua：局部变量
来源：http://read.share.vehdjk.com/Article/details/gomemxepp.sHtML

local a = 1
来源：http://www.m.share.tarul.cn/Article/details/grykdyhxg.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.vehdjk.com/Article/details/guhtcjmvc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.tarul.cn/Article/details/giuzegavf.sHtML

[T34] Lua：遍历表
来源：http://3g.bbcook.cn/Article/details/gxutbvdsa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.bbcook.cn/Article/details/ghoxjzczn.sHtML

[T35] Lua：字典表
来源：http://m.share.yfazqb.com/Article/details/gisysgjma.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.yfazqb.com/Article/details/gqblzuecm.sHtML

[T36] Lua：函数
来源：http://www.share.sjlbkw.cn/Article/details/gexhkatac.sHtML

function add(a, b) return a + b end
来源：http://mobile.epnwcf.com/Article/details/geiinvdsz.sHtML


<!-- 参考信息 -->