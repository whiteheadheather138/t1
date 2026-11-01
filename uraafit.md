代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.epnwcf.com/Article/details/gjfbbrjfo.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/gsedqbmnd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.sjlbkw.cn/Article/details/giomwqjeh.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.vehdjk.com/Article/details/ggrtzrxra.sHtML

files=$(ls -1)
来源：http://read.share.bbcook.cn/Article/details/gsuyrrtjh.sHtML

[R38] 管道串联
来源：http://wap.vehdjk.com/Article/details/gxdyycgxw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.bbcook.cn/Article/details/gjuaoqvbj.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.epnwcf.com/Article/details/gwczqmdko.sHtML

cmd > out.log 2>&1
来源：http://3g.epnwcf.com/Article/details/gzhcaxcdf.sHtML

[R40] 追加写日志
来源：http://wap.vehdjk.com/Article/details/gmhmgxrbb.sHtML

echo "log" >> out.log
来源：http://blog.epnwcf.com/Article/details/gnvdnmres.sHtML

[R41] 丢弃输出
来源：http://blog.bbcook.cn/Article/details/gmfjesvmq.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/griagnugh.sHtML

[R42] 输入重定向
来源：http://wap.fktsv.cn/Article/details/gsvewpull.sHtML

wc -l < a.txt
来源：http://mobile.fktsv.cn/Article/details/gysjynoyb.sHtML

[R43] 按名字查找文件
来源：http://www.share.tarul.cn/Article/details/gnocdorwx.sHtML

find . -name "*.log" -type f
来源：http://read.share.epnwcf.com/Article/details/gpzwtrhcn.sHtML

[R44] 按修改时间查找
来源：http://www.blog.tarul.cn/Article/details/gmowdacqb.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fktsv.cn/Article/details/gtrpnwunt.sHtML

[R45] 批量删除
来源：http://blog.fktsv.cn/Article/details/ghyroynzl.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fktsv.cn/Article/details/ggqcgufnr.sHtML

[R46] 递归替换文件内容
来源：http://mobile.bbcook.cn/Article/details/gqsyexdjv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.epnwcf.com/Article/details/ggjameewo.sHtML

[R47] sed 单行替换
来源：http://baike.sjlbkw.cn/Article/details/gbxskvibd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fktsv.cn/Article/details/gpzxaesjl.sHtML

[R48] awk 取指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/guaxlijlj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gasrmgyqt.sHtML

[R49] awk 带条件
来源：http://www.share.epnwcf.com/Article/details/gdwxuzenb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.sjlbkw.cn/Article/details/gkbewrpry.sHtML

[R50] awk 求和
来源：http://mobile.fktsv.cn/Article/details/gonxwxppq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.bbcook.cn/Article/details/gpytqhpif.sHtML

[R51] 排序去重取前几
来源：http://wap.bbcook.cn/Article/details/geivrvqyo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.vehdjk.com/Article/details/gpcxzfhyo.sHtML

[R52] 统计行数
来源：http://www.blog.bbcook.cn/Article/details/gztgcwvji.sHtML

wc -l a.txt
来源：http://wap.epnwcf.com/Article/details/gtbzpydje.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.sjlbkw.cn/Article/details/goqvrocgc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.yfazqb.com/Article/details/gircfjpmv.sHtML

[R54] 比较两个文件
来源：http://www.blog.vehdjk.com/Article/details/gvbxbihxb.sHtML

diff a.txt b.txt
来源：http://mobile.fktsv.cn/Article/details/guekosmpf.sHtML

[R55] 压缩与解压
来源：http://wap.fktsv.cn/Article/details/gmyywbnka.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.bbcook.cn/Article/details/gjgrbytjb.sHtML

[R56] 远程拷贝
来源：http://3g.tarul.cn/Article/details/gumypacwo.sHtML

scp file user@host:/path/
来源：http://blog.yfazqb.com/Article/details/gukmiirea.sHtML

[R57] 远程执行命令
来源：http://www.blog.tarul.cn/Article/details/gjuuqievl.sHtML

ssh user@host 'uptime'
来源：http://mobile.fktsv.cn/Article/details/gshhdspqh.sHtML

[R58] 下载文件
来源：http://wap.vehdjk.com/Article/details/gbpmkotym.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.yfazqb.com/Article/details/gymewmyso.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gfdbhhupi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.tarul.cn/Article/details/gtlwgopbb.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gqexbxmxy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/gnwgsntkf.sHtML

[R61] 磁盘占用
来源：http://wap.tarul.cn/Article/details/gwzoitted.sHtML

df -h;  du -sh *
来源：http://www.blog.vehdjk.com/Article/details/gkfnrsack.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.vehdjk.com/Article/details/gtbmdajet.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fktsv.cn/Article/details/gufeowwrp.sHtML

[R63] 内存与进程
来源：http://wap.epnwcf.com/Article/details/gprckvsld.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.tarul.cn/Article/details/glqmrdnrd.sHtML

[R64] 结束进程
来源：http://mobile.yfazqb.com/Article/details/gvlrvcmtv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.bbcook.cn/Article/details/gnttbxdzy.sHtML

[R65] 查看端口占用
来源：http://blog.sjlbkw.cn/Article/details/gumzfpumv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.epnwcf.com/Article/details/gagfeiiem.sHtML

[R66] 定时任务
来源：http://3g.epnwcf.com/Article/details/gxroupeju.sHtML

crontab -e;  crontab -l
来源：http://blog.fktsv.cn/Article/details/gypafvldo.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.epnwcf.com/Article/details/gpauzxend.sHtML

openssl rand -hex 16
来源：http://read.share.vehdjk.com/Article/details/gncsekxem.sHtML

[R68] 计算文件校验值
来源：http://wap.fktsv.cn/Article/details/gdtgakjng.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fktsv.cn/Article/details/gtupslnlq.sHtML

[R69] 生成随机密码
来源：http://www.share.epnwcf.com/Article/details/gspsnezug.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.epnwcf.com/Article/details/ghcvfrwof.sHtML

[R70] 时间戳与互转
来源：http://read.share.epnwcf.com/Article/details/gyvoholrh.sHtML

date +%s;  date -d @1700000000
来源：http://blog.bbcook.cn/Article/details/ghvfedzsr.sHtML

[R71] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gdotbwocq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.bbcook.cn/Article/details/gknlebqnq.sHtML

[R72] 等待端口就绪
来源：http://m.share.epnwcf.com/Article/details/gmefqfgjq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gozytznqj.sHtML

[R73] 分割大日志
来源：http://www.blog.bbcook.cn/Article/details/gqzemcwvj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.yfazqb.com/Article/details/ghxpthmtp.sHtML

[R74] 批量重命名
来源：http://m.share.epnwcf.com/Article/details/gxqhvmbry.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.sjlbkw.cn/Article/details/gbbmyeqgn.sHtML

[R75] 导出环境变量
来源：http://wap.yfazqb.com/Article/details/gncucekiw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.yfazqb.com/Article/details/gwrdfyetx.sHtML

[R76] 使用临时文件
来源：http://read.share.sjlbkw.cn/Article/details/gnvisbwzn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gmdrrmrqd.sHtML

[R77] 读取用户输入
来源：http://baike.bbcook.cn/Article/details/gpounhddp.sHtML

read -rp "请输入: " ans
来源：http://www.share.tarul.cn/Article/details/gprbgjiod.sHtML

[R78] 交互式菜单
来源：http://3g.tarul.cn/Article/details/gpyuituhe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.epnwcf.com/Article/details/gmnemprbl.sHtML

[R79] 解析命令行选项
来源：http://www.blog.sjlbkw.cn/Article/details/gytgfrhjo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.yfazqb.com/Article/details/gymflkapm.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.yfazqb.com/Article/details/gftttlbnd.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/glctlbasv.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/goqlsuldr.sHtML

S. C / C++ 专题
来源：http://blog.vehdjk.com/Article/details/gdtceiawe.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmdwojxoz.sHtML

[S01] C：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gkswqmyat.sHtML

#include <stdio.h>
来源：http://www.blog.bbcook.cn/Article/details/gvimemxnp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.vehdjk.com/Article/details/gxzgfisdm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.yfazqb.com/Article/details/geqsaotuj.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.epnwcf.com/Article/details/grsbhqaxf.sHtML

[S03] C：读入整数
来源：http://wap.epnwcf.com/Article/details/gcjwegcry.sHtML

int x; scanf("%d", &x);
来源：http://www.share.tarul.cn/Article/details/gnxywaejs.sHtML

[S04] C：字符串复制
来源：http://www.m.share.bbcook.cn/Article/details/gbpznnwxb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.bbcook.cn/Article/details/gyzgsfgza.sHtML

[S05] C：字符串长度
来源：http://mobile.yfazqb.com/Article/details/gntzplrtg.sHtML

strlen(s)
来源：http://wap.vehdjk.com/Article/details/guwsiyvfy.sHtML

[S06] C：字符串比较
来源：http://read.share.vehdjk.com/Article/details/gaakkecfd.sHtML

strcmp(a, b) == 0
来源：http://read.share.sjlbkw.cn/Article/details/glgwqlltp.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/gxcvmyhlu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.sjlbkw.cn/Article/details/gzjyvaycg.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/gzlhkdkmq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.vehdjk.com/Article/details/gwhefkgaj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.epnwcf.com/Article/details/gsebrcvvm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fktsv.cn/Article/details/gvudayipc.sHtML

[S10] C：指针与解引用
来源：http://blog.tarul.cn/Article/details/glgstsxha.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.vehdjk.com/Article/details/gswafwmgt.sHtML

[S11] C：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gsofnqzag.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fktsv.cn/Article/details/gheumlsgx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/gtgpxearv.sHtML

fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gkijxxxzr.sHtML

[S12] C：写文件
来源：http://m.share.bbcook.cn/Article/details/ghmxzuqpz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.tarul.cn/Article/details/gcvicoydz.sHtML

[S13] C：宏定义
来源：http://www.blog.tarul.cn/Article/details/gpopzfpnx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.tarul.cn/Article/details/grqnnmdiz.sHtML

[S14] C：枚举
来源：http://3g.vehdjk.com/Article/details/godigoiib.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.epnwcf.com/Article/details/gppqkgkdq.sHtML

[S15] C：类型转换
来源：http://mobile.epnwcf.com/Article/details/gaofrfseo.sHtML

(double) a / b
来源：http://m.share.vehdjk.com/Article/details/gtxivzydk.sHtML

[S16] C：位操作置位
来源：http://wap.fktsv.cn/Article/details/gcqnxrmfq.sHtML

x |= (1 << 3);
来源：http://www.blog.epnwcf.com/Article/details/goicdaxql.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/gtvuvtxyc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.tarul.cn/Article/details/gnhencgtd.sHtML

[S18] C：命令行参数
来源：http://wap.vehdjk.com/Article/details/gzewdbsbr.sHtML

int main(int argc, char **argv)
来源：http://wap.epnwcf.com/Article/details/gfdbvksnk.sHtML

[S19] C：快速排序
来源：http://baike.yfazqb.com/Article/details/gvgwzrrmm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/gkwfannbq.sHtML

[S20] C：二分查找
来源：http://www.blog.fktsv.cn/Article/details/gzhqhssil.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/geayrtmuw.sHtML

[S21] C：字符类别判断
来源：http://www.blog.sjlbkw.cn/Article/details/gcpbfofwf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.sjlbkw.cn/Article/details/gphvkiesa.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/guiowmmyn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.yfazqb.com/Article/details/gddtzgdqz.sHtML

[S23] C：随机数
来源：http://www.share.yfazqb.com/Article/details/gwoiaijas.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.vehdjk.com/Article/details/gyxhftkde.sHtML

[S24] C：获取本地时间
来源：http://read.share.epnwcf.com/Article/details/gbmtfcgzm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.sjlbkw.cn/Article/details/galzdoncr.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.bbcook.cn/Article/details/ggumpmfyh.sHtML

memcpy(dst, src, n);
来源：http://mobile.bbcook.cn/Article/details/gmjqwioaj.sHtML

[S26] C：内存清零
来源：http://3g.yfazqb.com/Article/details/geiamnpkc.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.yfazqb.com/Article/details/gkjqvppyu.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/gugwpabni.sHtML

const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gbphywbkb.sHtML

[S28] C：静态变量
来源：http://blog.vehdjk.com/Article/details/gycjexvow.sHtML

static int counter = 0;
来源：http://m.share.tarul.cn/Article/details/gwmteanxt.sHtML

[S29] C：变参函数
来源：http://www.m.share.yfazqb.com/Article/details/gyiehfyds.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.bbcook.cn/Article/details/gvblwsqvi.sHtML

[S30] C：头文件保护
来源：http://3g.tarul.cn/Article/details/gqmdgslup.sHtML

#ifndef X_H
来源：http://www.m.share.tarul.cn/Article/details/gliruqypb.sHtML

#define X_H
来源：http://www.share.sjlbkw.cn/Article/details/gexortbvj.sHtML

#endif
来源：http://3g.sjlbkw.cn/Article/details/gehntsgnx.sHtML

[S31] C++：Hello World
来源：http://3g.vehdjk.com/Article/details/gcegirgta.sHtML

#include <iostream>
来源：http://www.share.vehdjk.com/Article/details/gyrooqqhw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.bbcook.cn/Article/details/gmgbijelz.sHtML

[S32] C++：字符串
来源：http://www.share.bbcook.cn/Article/details/gtccsslti.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.bbcook.cn/Article/details/gnmawplmd.sHtML

[S33] C++：vector 增删
来源：http://baike.vehdjk.com/Article/details/gqotyouuk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.vehdjk.com/Article/details/gqkkprgwt.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/gaidsdlef.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fktsv.cn/Article/details/glcufoojc.sHtML

[S35] C++：map
来源：http://read.share.yfazqb.com/Article/details/ggtmbajbi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/gvltylamx.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.tarul.cn/Article/details/geqvwhtkl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gbhnfpkbg.sHtML

[S37] C++：set
来源：http://m.share.epnwcf.com/Article/details/gnqmwrtuh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.epnwcf.com/Article/details/gisjonliy.sHtML

[S38] C++：排序
来源：http://www.share.epnwcf.com/Article/details/gxtivfolk.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fktsv.cn/Article/details/gfwwotnde.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.bbcook.cn/Article/details/gtbqyxvcf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/gnggomxrw.sHtML

[S40] C++：查找元素
来源：http://www.share.vehdjk.com/Article/details/guwcgwlqu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fktsv.cn/Article/details/gwadcjdyo.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gxmxzfvwq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.epnwcf.com/Article/details/gqgocjpqx.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.tarul.cn/Article/details/ghzzrjlcl.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.epnwcf.com/Article/details/gzxaaaxyg.sHtML

[S43] C++：智能指针
来源：http://www.blog.tarul.cn/Article/details/gwjlcdfvn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.epnwcf.com/Article/details/gbrtejysz.sHtML

[S44] C++：引用传参
来源：http://wap.tarul.cn/Article/details/goaqmdpvr.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/gzlqsokfp.sHtML

[S45] C++：lambda
来源：http://3g.epnwcf.com/Article/details/gjlsojfbv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.vehdjk.com/Article/details/golchxgjk.sHtML

[S46] C++：函数模板
来源：http://baike.epnwcf.com/Article/details/gdpegcvuq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/gtuxrescn.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.sjlbkw.cn/Article/details/gyuixkhkx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.sjlbkw.cn/Article/details/gmeqqhugn.sHtML

[S48] C++：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gakphfghf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.tarul.cn/Article/details/gpdzqwcco.sHtML

while (std::getline(in, line)) { }
来源：http://wap.bbcook.cn/Article/details/gxmvvfhao.sHtML

[S49] C++：写文件
来源：http://3g.bbcook.cn/Article/details/gzulmalih.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.epnwcf.com/Article/details/ggvxnfowk.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.tarul.cn/Article/details/gofzntlse.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.yfazqb.com/Article/details/gjufjiqqg.sHtML

[S51] C++：显式类型转换
来源：http://m.share.sjlbkw.cn/Article/details/gtzayanjj.sHtML

static_cast<double>(a) / b
来源：http://m.share.epnwcf.com/Article/details/gnqymrmtg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.vehdjk.com/Article/details/gkoqoymwk.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.bbcook.cn/Article/details/gtufclnpg.sHtML

[S53] C++：移动语义
来源：http://baike.bbcook.cn/Article/details/gkitgwkoz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.bbcook.cn/Article/details/gglfwqxkv.sHtML

[S54] C++：异常处理
来源：http://wap.bbcook.cn/Article/details/glpxgreyv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.yfazqb.com/Article/details/gdodzbyfl.sHtML

[S55] C++：结构化绑定
来源：http://read.share.bbcook.cn/Article/details/gojnabgct.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.epnwcf.com/Article/details/glshextxa.sHtML

[S56] C++：optional
来源：http://www.m.share.epnwcf.com/Article/details/gjpblxehg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.yfazqb.com/Article/details/gtfcvrxtx.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gonbndotb.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgzqdboh.sHtML

[S58] C++：命名空间
来源：http://read.share.yfazqb.com/Article/details/geylylslf.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.sjlbkw.cn/Article/details/gdqpzdrsa.sHtML

[S59] C++：静态断言
来源：http://3g.sjlbkw.cn/Article/details/gikkrteqr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.yfazqb.com/Article/details/gngmriasq.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.vehdjk.com/Article/details/gdutzkkej.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.bbcook.cn/Article/details/gwjyoewup.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/grbkchicw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/guepewpqq.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gpmgneyqe.sHtML

[T01] Kotlin：Hello World
来源：http://blog.epnwcf.com/Article/details/geboavirx.sHtML

println("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gxzwftttm.sHtML

[T02] Kotlin：变量
来源：http://baike.vehdjk.com/Article/details/gkzrmihpg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.bbcook.cn/Article/details/gvmoxqeet.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fktsv.cn/Article/details/guuhwlajo.sHtML

"值: $b"
来源：http://blog.tarul.cn/Article/details/grohkyedi.sHtML

[T04] Kotlin：空安全
来源：http://read.share.tarul.cn/Article/details/gxkmydymy.sHtML

val n: String? = null;  n?.length
来源：http://baike.fktsv.cn/Article/details/goqjwgnis.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fktsv.cn/Article/details/gljhaosma.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.sjlbkw.cn/Article/details/gzphwbqtd.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxotoorj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gotyvbtca.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.epnwcf.com/Article/details/gotmiigqs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.yfazqb.com/Article/details/geimndlsi.sHtML

[T08] Kotlin：数据类
来源：http://read.share.yfazqb.com/Article/details/gmdrgmxcb.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fktsv.cn/Article/details/gngluzylf.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.epnwcf.com/Article/details/glvcfjvuy.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.sjlbkw.cn/Article/details/ggrxrqseu.sHtML

[T10] Kotlin：默认参数
来源：http://baike.vehdjk.com/Article/details/gksyobmaq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.vehdjk.com/Article/details/gjtyqmxmw.sHtML

[T11] Kotlin：协程
来源：http://www.share.fktsv.cn/Article/details/gtztvfden.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fktsv.cn/Article/details/grmncceur.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.epnwcf.com/Article/details/gdctvafrg.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.vehdjk.com/Article/details/ggtbvibsu.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.sjlbkw.cn/Article/details/gdcohdlsb.sHtML

val m = mapOf("a" to 1)
来源：http://baike.sjlbkw.cn/Article/details/gtxmagyxk.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fktsv.cn/Article/details/gssgqmqtx.sHtML

for (i in 1..10) println(i)
来源：http://wap.epnwcf.com/Article/details/gcsfnfjui.sHtML

[T15] Kotlin：接口
来源：http://blog.epnwcf.com/Article/details/gpqphfyhg.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.tarul.cn/Article/details/gutbrpacb.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gdbahrcfc.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/gpzoltipb.sHtML

[T17] Swift：变量与常量
来源：http://blog.sjlbkw.cn/Article/details/gjyqqondg.sHtML

var a = 1;  let b = 2
来源：http://read.share.fktsv.cn/Article/details/gadqqcieq.sHtML

[T18] Swift：字符串插值
来源：http://blog.epnwcf.com/Article/details/gqqmbykwu.sHtML

"值: \(b)"
来源：http://read.share.yfazqb.com/Article/details/gwuifuwvb.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.vehdjk.com/Article/details/gviqbntwo.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fktsv.cn/Article/details/gdtccxyna.sHtML

[T20] Swift：数组操作
来源：http://m.share.bbcook.cn/Article/details/gttvhwtqn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.bbcook.cn/Article/details/gbdcufqkh.sHtML

[T21] Swift：遍历
来源：http://3g.epnwcf.com/Article/details/ghbwrxygo.sHtML

for x in a { print(x) }
来源：http://mobile.epnwcf.com/Article/details/gbeibhnfd.sHtML

[T22] Swift：字典
来源：http://mobile.bbcook.cn/Article/details/gfpgoamiz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.sjlbkw.cn/Article/details/gdclzcqqj.sHtML

[T23] Swift：函数
来源：http://m.share.fktsv.cn/Article/details/gdofmmztv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fktsv.cn/Article/details/ggmjpzybr.sHtML

[T24] Swift：闭包
来源：http://baike.sjlbkw.cn/Article/details/gmmhaautd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gdpfyomzt.sHtML

[T25] Swift：结构体
来源：http://baike.fktsv.cn/Article/details/gpifbvhqv.sHtML

struct P { var x: Int }
来源：http://www.blog.epnwcf.com/Article/details/gyffsanno.sHtML

[T26] Swift：类与重写
来源：http://read.share.epnwcf.com/Article/details/gpimhbgfo.sHtML

class A: Base { override func f() {} }
来源：http://read.share.sjlbkw.cn/Article/details/gjbasskbn.sHtML

[T27] Swift：错误处理
来源：http://wap.fktsv.cn/Article/details/gwgycuvjo.sHtML

do { try f() } catch { print(error) }
来源：http://blog.vehdjk.com/Article/details/gwrobzthv.sHtML

[T28] Swift：枚举
来源：http://wap.yfazqb.com/Article/details/gwmmmnjpr.sHtML

enum Color { case red, green }
来源：http://www.m.share.yfazqb.com/Article/details/gtymldhua.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.epnwcf.com/Article/details/gavtfamgr.sHtML

guard let x = opt else { return }
来源：http://mobile.fktsv.cn/Article/details/guzrvfwuv.sHtML

[T30] Swift：协议
来源：http://mobile.vehdjk.com/Article/details/gcwgpgrpa.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.yfazqb.com/Article/details/getlxxpvu.sHtML

[T31] Lua：Hello World
来源：http://read.share.vehdjk.com/Article/details/gipkywbrr.sHtML

print("Hello")
来源：http://www.share.tarul.cn/Article/details/gihzugszz.sHtML

[T32] Lua：局部变量
来源：http://www.share.yfazqb.com/Article/details/gklmhllen.sHtML

local a = 1
来源：http://read.share.yfazqb.com/Article/details/gxmibnoxu.sHtML

[T33] Lua：表（数组）
来源：http://mobile.sjlbkw.cn/Article/details/gwsnuypkt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.vehdjk.com/Article/details/gafqznqls.sHtML

[T34] Lua：遍历表
来源：http://mobile.tarul.cn/Article/details/gilnfbsrf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fktsv.cn/Article/details/gjpolzcue.sHtML

[T35] Lua：字典表
来源：http://www.blog.fktsv.cn/Article/details/grmzsmldl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gjfnkujok.sHtML

[T36] Lua：函数
来源：http://m.share.yfazqb.com/Article/details/gswmknzpe.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gxobllzsp.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gfvstnwuj.sHtML

"a" .. "b"
来源：http://read.share.sjlbkw.cn/Article/details/gbvjudfov.sHtML

[T38] Lua：条件
来源：http://read.share.bbcook.cn/Article/details/guxfpeqwq.sHtML

if x > 0 then print("正") end
来源：http://www.blog.sjlbkw.cn/Article/details/gkxxpjgxc.sHtML


<!-- 参考信息 -->