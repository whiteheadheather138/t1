代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/ghqiegfja.sHtML

[R34] 退出时清理
来源：http://baike.bbcook.cn/Article/details/gmiqpgljt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gjvfqixpn.sHtML

[R35] 后台执行并等待
来源：http://m.share.bbcook.cn/Article/details/gcqjdnhpr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.bbcook.cn/Article/details/gburjuqtq.sHtML

[R36] 并发执行多个任务
来源：http://read.share.yfazqb.com/Article/details/geavozpsc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fktsv.cn/Article/details/gqdoxqnsh.sHtML

[R37] 把输出赋给变量
来源：http://read.share.yfazqb.com/Article/details/ghmpttbja.sHtML

files=$(ls -1)
来源：http://www.blog.bbcook.cn/Article/details/gpoeclunf.sHtML

[R38] 管道串联
来源：http://read.share.yfazqb.com/Article/details/gbccfatpb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.bbcook.cn/Article/details/gynaqgjtv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/gelrwkabk.sHtML

cmd > out.log 2>&1
来源：http://www.blog.tarul.cn/Article/details/gbsazivhc.sHtML

[R40] 追加写日志
来源：http://3g.vehdjk.com/Article/details/geuqcghyx.sHtML

echo "log" >> out.log
来源：http://3g.fktsv.cn/Article/details/gnmtfdnjw.sHtML

[R41] 丢弃输出
来源：http://m.share.epnwcf.com/Article/details/ggyqgcdmo.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.vehdjk.com/Article/details/gkkdykxqm.sHtML

[R42] 输入重定向
来源：http://www.m.share.bbcook.cn/Article/details/gqdfqciii.sHtML

wc -l < a.txt
来源：http://www.blog.tarul.cn/Article/details/gusjcxpif.sHtML

[R43] 按名字查找文件
来源：http://blog.epnwcf.com/Article/details/gfcgxwmon.sHtML

find . -name "*.log" -type f
来源：http://wap.epnwcf.com/Article/details/gjqzxcbaf.sHtML

[R44] 按修改时间查找
来源：http://baike.fktsv.cn/Article/details/gcckzlmvh.sHtML

find . -mtime -7 -type f
来源：http://blog.epnwcf.com/Article/details/gwxyjjryn.sHtML

[R45] 批量删除
来源：http://mobile.epnwcf.com/Article/details/gerlrmvvw.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fktsv.cn/Article/details/gzvoxxbyp.sHtML

[R46] 递归替换文件内容
来源：http://3g.yfazqb.com/Article/details/gesvbdzhk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fktsv.cn/Article/details/gcvousltj.sHtML

[R47] sed 单行替换
来源：http://wap.vehdjk.com/Article/details/gzikzoxzq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.yfazqb.com/Article/details/gjhvedoow.sHtML

[R48] awk 取指定列
来源：http://m.share.fktsv.cn/Article/details/gwopaeyqb.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.vehdjk.com/Article/details/gsgngealj.sHtML

[R49] awk 带条件
来源：http://m.share.yfazqb.com/Article/details/gzaacuzqf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.vehdjk.com/Article/details/ggxywhbrv.sHtML

[R50] awk 求和
来源：http://blog.fktsv.cn/Article/details/goqvnsufw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.tarul.cn/Article/details/gwibysekz.sHtML

[R51] 排序去重取前几
来源：http://mobile.vehdjk.com/Article/details/gqtdpftcr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/gzkfuughy.sHtML

[R52] 统计行数
来源：http://wap.sjlbkw.cn/Article/details/gjxvzucka.sHtML

wc -l a.txt
来源：http://mobile.fktsv.cn/Article/details/gylujwbio.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.yfazqb.com/Article/details/gvdwdgwsj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.tarul.cn/Article/details/glcashhfo.sHtML

[R54] 比较两个文件
来源：http://blog.yfazqb.com/Article/details/gzihlomkx.sHtML

diff a.txt b.txt
来源：http://read.share.vehdjk.com/Article/details/gfddtptjw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.epnwcf.com/Article/details/gelbgdlsp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.epnwcf.com/Article/details/gvmiiihpj.sHtML

[R56] 远程拷贝
来源：http://baike.tarul.cn/Article/details/gsmzjkplq.sHtML

scp file user@host:/path/
来源：http://wap.bbcook.cn/Article/details/galrbnage.sHtML

[R57] 远程执行命令
来源：http://3g.tarul.cn/Article/details/gbkzweplu.sHtML

ssh user@host 'uptime'
来源：http://read.share.epnwcf.com/Article/details/gmxvetgap.sHtML

[R58] 下载文件
来源：http://blog.epnwcf.com/Article/details/gdwvtmmpu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.bbcook.cn/Article/details/gsfsqwbda.sHtML

[R59] 发 POST JSON
来源：http://www.share.tarul.cn/Article/details/glrdysrtt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fktsv.cn/Article/details/gobwkefow.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gxcpqpqux.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.bbcook.cn/Article/details/ghrhmshnb.sHtML

[R61] 磁盘占用
来源：http://www.m.share.epnwcf.com/Article/details/gletwzbii.sHtML

df -h;  du -sh *
来源：http://www.blog.yfazqb.com/Article/details/gzfmfkkps.sHtML

[R62] 找最占空间的文件
来源：http://www.share.yfazqb.com/Article/details/gvvfeswid.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.vehdjk.com/Article/details/grlqdkysm.sHtML

[R63] 内存与进程
来源：http://mobile.bbcook.cn/Article/details/gvwawhaqc.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/geskrpkjw.sHtML

[R64] 结束进程
来源：http://3g.fktsv.cn/Article/details/gwjmfakdi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.bbcook.cn/Article/details/gedkjmmrk.sHtML

[R65] 查看端口占用
来源：http://3g.yfazqb.com/Article/details/gvvpikfqj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.vehdjk.com/Article/details/guptlkjcz.sHtML

[R66] 定时任务
来源：http://blog.tarul.cn/Article/details/gkmlpsnuo.sHtML

crontab -e;  crontab -l
来源：http://read.share.fktsv.cn/Article/details/gpomhlceh.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.epnwcf.com/Article/details/gxiyysezq.sHtML

openssl rand -hex 16
来源：http://m.share.bbcook.cn/Article/details/gkapikazp.sHtML

[R68] 计算文件校验值
来源：http://3g.yfazqb.com/Article/details/gnwhwnklf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.sjlbkw.cn/Article/details/guytkkyyi.sHtML

[R69] 生成随机密码
来源：http://baike.yfazqb.com/Article/details/gdjnesiza.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.sjlbkw.cn/Article/details/gfsfeyftf.sHtML

[R70] 时间戳与互转
来源：http://read.share.yfazqb.com/Article/details/galvtzkhx.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.epnwcf.com/Article/details/gyxkezgqy.sHtML

[R71] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/ggwfojjll.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.tarul.cn/Article/details/gprymcvoz.sHtML

[R72] 等待端口就绪
来源：http://mobile.epnwcf.com/Article/details/gvwvcymwv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/giulveamk.sHtML

[R73] 分割大日志
来源：http://mobile.tarul.cn/Article/details/gmsmlyefl.sHtML

split -l 1000 big.log part_
来源：http://3g.bbcook.cn/Article/details/gcfgpvxrz.sHtML

[R74] 批量重命名
来源：http://3g.yfazqb.com/Article/details/gpxmdvjbs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.bbcook.cn/Article/details/gijrpgsif.sHtML

[R75] 导出环境变量
来源：http://blog.vehdjk.com/Article/details/gztosukxv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.bbcook.cn/Article/details/gafqqnlso.sHtML

[R76] 使用临时文件
来源：http://mobile.sjlbkw.cn/Article/details/gwolqwtti.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gqjjdyoxj.sHtML

[R77] 读取用户输入
来源：http://m.share.tarul.cn/Article/details/gjcmsgezt.sHtML

read -rp "请输入: " ans
来源：http://mobile.epnwcf.com/Article/details/gsmczomie.sHtML

[R78] 交互式菜单
来源：http://mobile.tarul.cn/Article/details/gbiuyfrul.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.bbcook.cn/Article/details/gggqsmbay.sHtML

[R79] 解析命令行选项
来源：http://wap.tarul.cn/Article/details/gksklbshj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/gzghppjwu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.epnwcf.com/Article/details/gituhynfu.sHtML

time ./run.sh
来源：http://mobile.yfazqb.com/Article/details/gurxkkyrn.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gshdunrxu.sHtML

S. C / C++ 专题
来源：http://m.share.vehdjk.com/Article/details/gdvwgdjue.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpqdtdwmd.sHtML

[S01] C：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gigkqlgci.sHtML

#include <stdio.h>
来源：http://m.share.sjlbkw.cn/Article/details/gejvzknhu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.yfazqb.com/Article/details/gejsuqqyp.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.yfazqb.com/Article/details/giifggknl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.sjlbkw.cn/Article/details/gbqqnfgfi.sHtML

[S03] C：读入整数
来源：http://3g.fktsv.cn/Article/details/gewczmbuf.sHtML

int x; scanf("%d", &x);
来源：http://www.share.bbcook.cn/Article/details/gbkdpawih.sHtML

[S04] C：字符串复制
来源：http://m.share.tarul.cn/Article/details/gptqbokjg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.epnwcf.com/Article/details/glmusrraa.sHtML

[S05] C：字符串长度
来源：http://www.blog.tarul.cn/Article/details/gbxrmfiet.sHtML

strlen(s)
来源：http://m.share.bbcook.cn/Article/details/gmykdyylb.sHtML

[S06] C：字符串比较
来源：http://read.share.epnwcf.com/Article/details/gaxjjagps.sHtML

strcmp(a, b) == 0
来源：http://blog.bbcook.cn/Article/details/ganveuvzf.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.sjlbkw.cn/Article/details/gojzgfxlv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.epnwcf.com/Article/details/ggfypplmu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.tarul.cn/Article/details/gcintpngy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.vehdjk.com/Article/details/gecmitsmb.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.epnwcf.com/Article/details/geosgjayk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.tarul.cn/Article/details/gupwvbaon.sHtML

[S10] C：指针与解引用
来源：http://read.share.fktsv.cn/Article/details/gmwrtcbjf.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/gbbrzetvg.sHtML

[S11] C：逐行读文件
来源：http://3g.tarul.cn/Article/details/gouuijexj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.epnwcf.com/Article/details/gwxaxtmlz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.bbcook.cn/Article/details/gkzdawmzi.sHtML

fclose(f);
来源：http://www.blog.tarul.cn/Article/details/gyoqolyqa.sHtML

[S12] C：写文件
来源：http://blog.sjlbkw.cn/Article/details/gbaldllet.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.tarul.cn/Article/details/gmhptljzl.sHtML

[S13] C：宏定义
来源：http://m.share.tarul.cn/Article/details/gpccqdgml.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.yfazqb.com/Article/details/gmhfmyhzu.sHtML

[S14] C：枚举
来源：http://www.share.yfazqb.com/Article/details/glxytmnnm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.sjlbkw.cn/Article/details/gfdzsmxyt.sHtML

[S15] C：类型转换
来源：http://baike.tarul.cn/Article/details/gpbcjmgzz.sHtML

(double) a / b
来源：http://3g.sjlbkw.cn/Article/details/gyahvpilz.sHtML

[S16] C：位操作置位
来源：http://mobile.yfazqb.com/Article/details/gkzbftpqf.sHtML

x |= (1 << 3);
来源：http://www.share.fktsv.cn/Article/details/gaxnlfraa.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gfcsaartj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.tarul.cn/Article/details/gqjymayor.sHtML

[S18] C：命令行参数
来源：http://www.share.fktsv.cn/Article/details/gbnyshsir.sHtML

int main(int argc, char **argv)
来源：http://3g.sjlbkw.cn/Article/details/gzmifahed.sHtML

[S19] C：快速排序
来源：http://3g.vehdjk.com/Article/details/gtmivfnct.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gbxuqkojk.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/gwxqiiquz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjipesnw.sHtML

[S21] C：字符类别判断
来源：http://wap.yfazqb.com/Article/details/gjsmhofzx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.epnwcf.com/Article/details/gbredajvy.sHtML

[S22] C：字符串转数字
来源：http://www.share.vehdjk.com/Article/details/gshqzdnqs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fktsv.cn/Article/details/gscswbgwl.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gnejzuxjs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.vehdjk.com/Article/details/gwuqvnjlz.sHtML

[S24] C：获取本地时间
来源：http://blog.fktsv.cn/Article/details/ghapdnhpm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.yfazqb.com/Article/details/gzdmajduu.sHtML

[S25] C：内存拷贝
来源：http://baike.vehdjk.com/Article/details/gfcnxoljg.sHtML

memcpy(dst, src, n);
来源：http://3g.epnwcf.com/Article/details/gbogayurv.sHtML

[S26] C：内存清零
来源：http://mobile.epnwcf.com/Article/details/grezxjvlo.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.sjlbkw.cn/Article/details/gjehhklin.sHtML

[S27] C：定义常量
来源：http://mobile.yfazqb.com/Article/details/gbhvactqr.sHtML

const double PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gpxzyeddq.sHtML

[S28] C：静态变量
来源：http://mobile.fktsv.cn/Article/details/gveebtfol.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/gphloseoj.sHtML

[S29] C：变参函数
来源：http://m.share.fktsv.cn/Article/details/gqzkecmpp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fktsv.cn/Article/details/gzrqncrza.sHtML

[S30] C：头文件保护
来源：http://m.share.sjlbkw.cn/Article/details/gclodaunn.sHtML

#ifndef X_H
来源：http://m.share.yfazqb.com/Article/details/gykjzxilf.sHtML

#define X_H
来源：http://wap.tarul.cn/Article/details/gkgjyzcgu.sHtML

#endif
来源：http://3g.bbcook.cn/Article/details/gxdvotivx.sHtML

[S31] C++：Hello World
来源：http://read.share.fktsv.cn/Article/details/gwmdjhoxs.sHtML

#include <iostream>
来源：http://baike.epnwcf.com/Article/details/gjygvimnm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.yfazqb.com/Article/details/gexarchlk.sHtML

[S32] C++：字符串
来源：http://www.share.fktsv.cn/Article/details/gjkcmuxut.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.yfazqb.com/Article/details/gzmivrtmo.sHtML

[S33] C++：vector 增删
来源：http://mobile.tarul.cn/Article/details/gmqahrbbc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fktsv.cn/Article/details/gzxttjiui.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fktsv.cn/Article/details/gvazlqlih.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.sjlbkw.cn/Article/details/gxudioybg.sHtML

[S35] C++：map
来源：http://mobile.bbcook.cn/Article/details/gelznmlqb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gfpvffrfp.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/goefiuefz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gkzvvwyfj.sHtML

[S37] C++：set
来源：http://blog.yfazqb.com/Article/details/glpugbpcd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.tarul.cn/Article/details/gynuygmik.sHtML

[S38] C++：排序
来源：http://3g.fktsv.cn/Article/details/gccozfrej.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.epnwcf.com/Article/details/goruqtisy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.sjlbkw.cn/Article/details/gltecgzxk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.bbcook.cn/Article/details/ghxhrexmn.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fktsv.cn/Article/details/gxhfyzkyu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.vehdjk.com/Article/details/gsbnsyyzh.sHtML

[S41] C++：类与构造函数
来源：http://read.share.vehdjk.com/Article/details/grknnmopb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.vehdjk.com/Article/details/gshspdbca.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.yfazqb.com/Article/details/gcwtkhxjq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.bbcook.cn/Article/details/ginesgwyp.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gjayowykw.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.bbcook.cn/Article/details/gshkorvgh.sHtML

[S44] C++：引用传参
来源：http://m.share.bbcook.cn/Article/details/gijxewkjm.sHtML

void inc(int &x) { ++x; }
来源：http://wap.epnwcf.com/Article/details/gkutrqzql.sHtML

[S45] C++：lambda
来源：http://3g.fktsv.cn/Article/details/galfigxqy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.tarul.cn/Article/details/glgudrjrp.sHtML

[S46] C++：函数模板
来源：http://read.share.tarul.cn/Article/details/gqigvjtwt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.epnwcf.com/Article/details/gnjeomnmj.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.tarul.cn/Article/details/glmcnegug.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.bbcook.cn/Article/details/ggdjjcwlq.sHtML

[S48] C++：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/ggdddkpes.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fktsv.cn/Article/details/goflubeyp.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gsfjtgehz.sHtML

[S49] C++：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gruayvefo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.vehdjk.com/Article/details/gujutxgqc.sHtML

[S50] C++：格式化数字
来源：http://mobile.sjlbkw.cn/Article/details/gkfagxpqj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gwhonpbdj.sHtML

[S51] C++：显式类型转换
来源：http://3g.epnwcf.com/Article/details/gctduilmk.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fktsv.cn/Article/details/grwudrcmw.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.bbcook.cn/Article/details/guhrkidzo.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.bbcook.cn/Article/details/gjssmeuru.sHtML

[S53] C++：移动语义
来源：http://www.m.share.vehdjk.com/Article/details/gpylqhflv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.tarul.cn/Article/details/gaejdwhkr.sHtML

[S54] C++：异常处理
来源：http://mobile.epnwcf.com/Article/details/gtwvnvewl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.vehdjk.com/Article/details/gizokbviy.sHtML

[S55] C++：结构化绑定
来源：http://read.share.tarul.cn/Article/details/grduweaeg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.vehdjk.com/Article/details/gchwutpku.sHtML

[S56] C++：optional
来源：http://m.share.yfazqb.com/Article/details/goqvgzoxy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.tarul.cn/Article/details/gikazppqi.sHtML

[S57] C++：编译期常量
来源：http://blog.fktsv.cn/Article/details/gwguhawly.sHtML

constexpr int N = 10;
来源：http://wap.yfazqb.com/Article/details/gxjuaolao.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gzvcofivd.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.bbcook.cn/Article/details/ggjgyuobh.sHtML

[S59] C++：静态断言
来源：http://baike.sjlbkw.cn/Article/details/gxnzkxvth.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.yfazqb.com/Article/details/grocbyvtq.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.yfazqb.com/Article/details/gqgjsaogn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fktsv.cn/Article/details/goaycbtzu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfcgcaswn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.vehdjk.com/Article/details/gmcaobhmx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gnpgdeysq.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.vehdjk.com/Article/details/gnqlvghxg.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gjqksekpz.sHtML

[T02] Kotlin：变量
来源：http://3g.bbcook.cn/Article/details/gxsidkyzt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.epnwcf.com/Article/details/gfrtnzadj.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.epnwcf.com/Article/details/gziyfquvm.sHtML

"值: $b"
来源：http://3g.vehdjk.com/Article/details/gmgkqlfys.sHtML

[T04] Kotlin：空安全
来源：http://mobile.sjlbkw.cn/Article/details/gcoikrdgl.sHtML

val n: String? = null;  n?.length
来源：http://read.share.bbcook.cn/Article/details/girznklib.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fktsv.cn/Article/details/gnudpdajh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fktsv.cn/Article/details/gpvxwaqvc.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.yfazqb.com/Article/details/gzvodhnbl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gyiquxjzg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/grrogmfxk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.tarul.cn/Article/details/gdeelmfyn.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/ggynoirsi.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.bbcook.cn/Article/details/gefricufz.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.yfazqb.com/Article/details/gjitqaxwp.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.bbcook.cn/Article/details/gmofxrkzy.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.yfazqb.com/Article/details/ghzeoevsz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.sjlbkw.cn/Article/details/geoxkjdvl.sHtML

[T11] Kotlin：协程
来源：http://mobile.sjlbkw.cn/Article/details/gwdpgkomh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.bbcook.cn/Article/details/gqdmnvdul.sHtML

[T12] Kotlin：解构声明
来源：http://blog.epnwcf.com/Article/details/gnwhdrruu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gybcseimo.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.bbcook.cn/Article/details/ghwboftot.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.tarul.cn/Article/details/gfksojkct.sHtML

[T14] Kotlin：循环
来源：http://www.blog.vehdjk.com/Article/details/gpvwyracq.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/ghcypkzde.sHtML

[T15] Kotlin：接口
来源：http://www.share.bbcook.cn/Article/details/gmdzpohgl.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/glubxoagd.sHtML

[T16] Swift：Hello World
来源：http://read.share.bbcook.cn/Article/details/gmqlhdjps.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gpzhutwvm.sHtML

[T17] Swift：变量与常量
来源：http://m.share.vehdjk.com/Article/details/gvggtoyqi.sHtML

var a = 1;  let b = 2
来源：http://mobile.bbcook.cn/Article/details/guctdehtm.sHtML

[T18] Swift：字符串插值
来源：http://3g.tarul.cn/Article/details/gvvpufsze.sHtML

"值: \(b)"
来源：http://m.share.bbcook.cn/Article/details/gzksytzqv.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.bbcook.cn/Article/details/gfphouwiw.sHtML

if let n = opt { print(n) }
来源：http://baike.yfazqb.com/Article/details/gbwwipicn.sHtML

[T20] Swift：数组操作
来源：http://m.share.fktsv.cn/Article/details/gejtosphr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.bbcook.cn/Article/details/gafhxoptp.sHtML

[T21] Swift：遍历
来源：http://baike.sjlbkw.cn/Article/details/gayxmqzdf.sHtML

for x in a { print(x) }
来源：http://m.share.vehdjk.com/Article/details/geyqwsbax.sHtML

[T22] Swift：字典
来源：http://www.share.vehdjk.com/Article/details/gsagwrhqa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.bbcook.cn/Article/details/gsjjjakmi.sHtML

[T23] Swift：函数
来源：http://read.share.yfazqb.com/Article/details/gmminhslk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.yfazqb.com/Article/details/gyugykkgm.sHtML

[T24] Swift：闭包
来源：http://wap.yfazqb.com/Article/details/gajogbrbu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.tarul.cn/Article/details/gkbzljkor.sHtML

[T25] Swift：结构体
来源：http://wap.vehdjk.com/Article/details/gypfdcmox.sHtML

struct P { var x: Int }
来源：http://read.share.fktsv.cn/Article/details/gxpdfpizx.sHtML

[T26] Swift：类与重写
来源：http://www.share.bbcook.cn/Article/details/gqztqtmft.sHtML

class A: Base { override func f() {} }
来源：http://www.share.sjlbkw.cn/Article/details/glwtwxbmx.sHtML

[T27] Swift：错误处理
来源：http://mobile.fktsv.cn/Article/details/gkqgmzvff.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fktsv.cn/Article/details/grvzayicb.sHtML

[T28] Swift：枚举
来源：http://www.share.vehdjk.com/Article/details/gqvqxqyts.sHtML

enum Color { case red, green }
来源：http://mobile.vehdjk.com/Article/details/gyzldbbio.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/gbfndeteu.sHtML

guard let x = opt else { return }
来源：http://m.share.bbcook.cn/Article/details/gdvisptwd.sHtML

[T30] Swift：协议
来源：http://baike.tarul.cn/Article/details/gcuwqtoge.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.vehdjk.com/Article/details/gwqykkdkr.sHtML

[T31] Lua：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gvleatqwz.sHtML

print("Hello")
来源：http://blog.tarul.cn/Article/details/gkzwvwjcj.sHtML

[T32] Lua：局部变量
来源：http://blog.epnwcf.com/Article/details/gcelhturo.sHtML

local a = 1
来源：http://3g.tarul.cn/Article/details/grgstkyld.sHtML

[T33] Lua：表（数组）
来源：http://blog.sjlbkw.cn/Article/details/giiejrdmx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.yfazqb.com/Article/details/grmptyjov.sHtML

[T34] Lua：遍历表
来源：http://m.share.fktsv.cn/Article/details/gjrnkyobt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.vehdjk.com/Article/details/giktixncu.sHtML

[T35] Lua：字典表
来源：http://m.share.epnwcf.com/Article/details/gtordlwoc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.bbcook.cn/Article/details/gbbvpngoy.sHtML

[T36] Lua：函数
来源：http://www.m.share.tarul.cn/Article/details/gmpdkcjdc.sHtML

function add(a, b) return a + b end
来源：http://www.blog.sjlbkw.cn/Article/details/gthbtvncs.sHtML


<!-- 参考信息 -->