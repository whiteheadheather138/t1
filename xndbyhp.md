代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.epnwcf.com/Article/details/gchstmoia.sHtML

[R36] 并发执行多个任务
来源：http://read.share.sjlbkw.cn/Article/details/gbbjmginy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fktsv.cn/Article/details/gtqfyvrpt.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.sjlbkw.cn/Article/details/gmonfwvyy.sHtML

files=$(ls -1)
来源：http://wap.yfazqb.com/Article/details/gachbznhy.sHtML

[R38] 管道串联
来源：http://wap.tarul.cn/Article/details/gauezsbrw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.yfazqb.com/Article/details/glaiunrbc.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.bbcook.cn/Article/details/giuxwojee.sHtML

cmd > out.log 2>&1
来源：http://blog.vehdjk.com/Article/details/goytyapvs.sHtML

[R40] 追加写日志
来源：http://www.blog.sjlbkw.cn/Article/details/gabtnrdot.sHtML

echo "log" >> out.log
来源：http://www.blog.tarul.cn/Article/details/gmsmflbbm.sHtML

[R41] 丢弃输出
来源：http://3g.fktsv.cn/Article/details/gmjxulkdj.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fktsv.cn/Article/details/golywthmv.sHtML

[R42] 输入重定向
来源：http://mobile.epnwcf.com/Article/details/gdpejnjeh.sHtML

wc -l < a.txt
来源：http://www.blog.epnwcf.com/Article/details/gskjgzyjt.sHtML

[R43] 按名字查找文件
来源：http://3g.tarul.cn/Article/details/gyjvvwkiu.sHtML

find . -name "*.log" -type f
来源：http://www.blog.yfazqb.com/Article/details/gosqjprow.sHtML

[R44] 按修改时间查找
来源：http://blog.vehdjk.com/Article/details/gqyiizjrg.sHtML

find . -mtime -7 -type f
来源：http://m.share.tarul.cn/Article/details/gqonxfgvm.sHtML

[R45] 批量删除
来源：http://www.share.tarul.cn/Article/details/gvdezdder.sHtML

find . -name "*.tmp" -delete
来源：http://3g.tarul.cn/Article/details/gfvddsagf.sHtML

[R46] 递归替换文件内容
来源：http://wap.tarul.cn/Article/details/gumzdcdhp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.bbcook.cn/Article/details/gjljhicfb.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/glddisktw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.yfazqb.com/Article/details/gniholewm.sHtML

[R48] awk 取指定列
来源：http://www.blog.yfazqb.com/Article/details/gmpkfmaqa.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.bbcook.cn/Article/details/gulbowlti.sHtML

[R49] awk 带条件
来源：http://3g.tarul.cn/Article/details/gzfwthgle.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.tarul.cn/Article/details/gquqioyoa.sHtML

[R50] awk 求和
来源：http://m.share.fktsv.cn/Article/details/gynbssjju.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.vehdjk.com/Article/details/gbueqmbau.sHtML

[R51] 排序去重取前几
来源：http://3g.vehdjk.com/Article/details/ghvsfwzij.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.bbcook.cn/Article/details/gboklosza.sHtML

[R52] 统计行数
来源：http://m.share.fktsv.cn/Article/details/gvlsihrxj.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gulicqjod.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fktsv.cn/Article/details/gmujtmych.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.yfazqb.com/Article/details/gsdsxynor.sHtML

[R54] 比较两个文件
来源：http://www.blog.vehdjk.com/Article/details/gtkyocric.sHtML

diff a.txt b.txt
来源：http://www.m.share.fktsv.cn/Article/details/gwkqlroqw.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/gjfbleugz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.bbcook.cn/Article/details/gqauflurm.sHtML

[R56] 远程拷贝
来源：http://m.share.vehdjk.com/Article/details/glxcuqpku.sHtML

scp file user@host:/path/
来源：http://www.m.share.bbcook.cn/Article/details/gkgyjyduk.sHtML

[R57] 远程执行命令
来源：http://www.blog.epnwcf.com/Article/details/gdfmvdfus.sHtML

ssh user@host 'uptime'
来源：http://wap.sjlbkw.cn/Article/details/gvekcggyv.sHtML

[R58] 下载文件
来源：http://m.share.tarul.cn/Article/details/gtvvpfriq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fktsv.cn/Article/details/gnqaetjeo.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/gkvsutvel.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.yfazqb.com/Article/details/gmiondjuh.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/gsnvfjnfd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.sjlbkw.cn/Article/details/gynmhqsxd.sHtML

[R61] 磁盘占用
来源：http://baike.tarul.cn/Article/details/gbmjuqkvv.sHtML

df -h;  du -sh *
来源：http://blog.vehdjk.com/Article/details/gcphzzcwu.sHtML

[R62] 找最占空间的文件
来源：http://mobile.epnwcf.com/Article/details/gqnigkwzo.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.sjlbkw.cn/Article/details/gcbqaabhr.sHtML

[R63] 内存与进程
来源：http://baike.yfazqb.com/Article/details/gmfnkewqd.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.bbcook.cn/Article/details/geuaqajzx.sHtML

[R64] 结束进程
来源：http://mobile.bbcook.cn/Article/details/glwhzobcg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.vehdjk.com/Article/details/glluifyui.sHtML

[R65] 查看端口占用
来源：http://3g.yfazqb.com/Article/details/glvvzaggm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.vehdjk.com/Article/details/gfgopharn.sHtML

[R66] 定时任务
来源：http://www.m.share.bbcook.cn/Article/details/gsipenpom.sHtML

crontab -e;  crontab -l
来源：http://www.share.epnwcf.com/Article/details/gbzzimdoa.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.tarul.cn/Article/details/gmcpuoisk.sHtML

openssl rand -hex 16
来源：http://read.share.sjlbkw.cn/Article/details/gcfnsxbty.sHtML

[R68] 计算文件校验值
来源：http://www.share.yfazqb.com/Article/details/gjgeonycs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.yfazqb.com/Article/details/goifnamgc.sHtML

[R69] 生成随机密码
来源：http://mobile.epnwcf.com/Article/details/gdiqryszh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.vehdjk.com/Article/details/geeezufqy.sHtML

[R70] 时间戳与互转
来源：http://www.share.epnwcf.com/Article/details/gaiuzcybt.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.vehdjk.com/Article/details/gttcbmhyh.sHtML

[R71] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gyuixgnor.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.vehdjk.com/Article/details/glxaexuqg.sHtML

[R72] 等待端口就绪
来源：http://baike.bbcook.cn/Article/details/gymydgjyx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gzilfukpt.sHtML

[R73] 分割大日志
来源：http://mobile.fktsv.cn/Article/details/gfhlvglbz.sHtML

split -l 1000 big.log part_
来源：http://read.share.bbcook.cn/Article/details/geomhqskj.sHtML

[R74] 批量重命名
来源：http://www.blog.tarul.cn/Article/details/gmfzvxeym.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fktsv.cn/Article/details/gdnfeickx.sHtML

[R75] 导出环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gqvjuinjl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.bbcook.cn/Article/details/gictpcuzp.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/gzsyhblag.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gqtsixbwq.sHtML

[R77] 读取用户输入
来源：http://read.share.sjlbkw.cn/Article/details/gczglqmtb.sHtML

read -rp "请输入: " ans
来源：http://read.share.fktsv.cn/Article/details/gnfmlcoij.sHtML

[R78] 交互式菜单
来源：http://www.blog.fktsv.cn/Article/details/gmhbzrqyn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.bbcook.cn/Article/details/gwyemzibd.sHtML

[R79] 解析命令行选项
来源：http://3g.bbcook.cn/Article/details/gifhwausi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.vehdjk.com/Article/details/gxbbireia.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.bbcook.cn/Article/details/grgfhpcbq.sHtML

time ./run.sh
来源：http://www.blog.vehdjk.com/Article/details/glqqqzfly.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gnxworxoj.sHtML

S. C / C++ 专题
来源：http://www.m.share.epnwcf.com/Article/details/gyadwjxez.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvdaorijj.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/gkcejkysw.sHtML

#include <stdio.h>
来源：http://read.share.vehdjk.com/Article/details/gsmgprtws.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.vehdjk.com/Article/details/gvuiwwrqj.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.yfazqb.com/Article/details/grmniifci.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.tarul.cn/Article/details/gvriqsrjm.sHtML

[S03] C：读入整数
来源：http://www.blog.fktsv.cn/Article/details/gkhmpkbpj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.tarul.cn/Article/details/gbucndatw.sHtML

[S04] C：字符串复制
来源：http://baike.sjlbkw.cn/Article/details/gnvcqhuao.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.bbcook.cn/Article/details/gwphdextg.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/grdaswpzy.sHtML

strlen(s)
来源：http://baike.yfazqb.com/Article/details/gnooozvfh.sHtML

[S06] C：字符串比较
来源：http://3g.vehdjk.com/Article/details/grxsdjjzt.sHtML

strcmp(a, b) == 0
来源：http://baike.tarul.cn/Article/details/gfefszeml.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fktsv.cn/Article/details/gfgjjagbm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fktsv.cn/Article/details/ggdcyublt.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.sjlbkw.cn/Article/details/gkizkbiwm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fktsv.cn/Article/details/gwrnfktrf.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.epnwcf.com/Article/details/gmwqipdoa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.bbcook.cn/Article/details/gfwnpwbmo.sHtML

[S10] C：指针与解引用
来源：http://wap.bbcook.cn/Article/details/gnhtquaum.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.vehdjk.com/Article/details/gunkyxsqh.sHtML

[S11] C：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gquwhlfhk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.yfazqb.com/Article/details/gtazytudi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fktsv.cn/Article/details/guoitabdk.sHtML

fclose(f);
来源：http://wap.yfazqb.com/Article/details/gbsgyskrm.sHtML

[S12] C：写文件
来源：http://www.blog.fktsv.cn/Article/details/gxchpqfxd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.tarul.cn/Article/details/gcouedncg.sHtML

[S13] C：宏定义
来源：http://3g.vehdjk.com/Article/details/ghlqagrin.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.tarul.cn/Article/details/gqyfxdlpr.sHtML

[S14] C：枚举
来源：http://mobile.yfazqb.com/Article/details/gpwpmrixz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.vehdjk.com/Article/details/godeqrbvs.sHtML

[S15] C：类型转换
来源：http://wap.yfazqb.com/Article/details/gbudpmrut.sHtML

(double) a / b
来源：http://3g.yfazqb.com/Article/details/ginfhusrf.sHtML

[S16] C：位操作置位
来源：http://www.blog.yfazqb.com/Article/details/gigzxxnje.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/geattjajh.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/ggstdifpl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.tarul.cn/Article/details/gleueizom.sHtML

[S18] C：命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/gyhagajxx.sHtML

int main(int argc, char **argv)
来源：http://baike.epnwcf.com/Article/details/gytukrrgq.sHtML

[S19] C：快速排序
来源：http://www.blog.yfazqb.com/Article/details/gdslkrkxl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gceylgiqx.sHtML

[S20] C：二分查找
来源：http://www.m.share.bbcook.cn/Article/details/gxheukzsq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gklpgdigo.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.tarul.cn/Article/details/gcevxbgci.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.vehdjk.com/Article/details/gdlovftjs.sHtML

[S22] C：字符串转数字
来源：http://www.share.yfazqb.com/Article/details/gxqqjzpci.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.epnwcf.com/Article/details/glabdbhji.sHtML

[S23] C：随机数
来源：http://mobile.vehdjk.com/Article/details/gputrxmzb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.bbcook.cn/Article/details/gteahyydr.sHtML

[S24] C：获取本地时间
来源：http://3g.sjlbkw.cn/Article/details/garqqxfgl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/gtquipijw.sHtML

[S25] C：内存拷贝
来源：http://read.share.bbcook.cn/Article/details/gwefrmsdq.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.tarul.cn/Article/details/gtuprddzj.sHtML

[S26] C：内存清零
来源：http://www.share.vehdjk.com/Article/details/gcryzfsnn.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.yfazqb.com/Article/details/gkytccqqs.sHtML

[S27] C：定义常量
来源：http://m.share.fktsv.cn/Article/details/gghekfbjf.sHtML

const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gwzfhrwqd.sHtML

[S28] C：静态变量
来源：http://blog.tarul.cn/Article/details/ghndmeete.sHtML

static int counter = 0;
来源：http://mobile.sjlbkw.cn/Article/details/guqjmbzhn.sHtML

[S29] C：变参函数
来源：http://blog.tarul.cn/Article/details/gpiqinavp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.tarul.cn/Article/details/gjcctsckt.sHtML

[S30] C：头文件保护
来源：http://read.share.fktsv.cn/Article/details/gqfwcjivx.sHtML

#ifndef X_H
来源：http://read.share.epnwcf.com/Article/details/gffqisvrz.sHtML

#define X_H
来源：http://www.m.share.vehdjk.com/Article/details/gappixmpf.sHtML

#endif
来源：http://mobile.epnwcf.com/Article/details/grcylthzp.sHtML

[S31] C++：Hello World
来源：http://read.share.tarul.cn/Article/details/gdfhszxfa.sHtML

#include <iostream>
来源：http://mobile.sjlbkw.cn/Article/details/gvzhvjzer.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.epnwcf.com/Article/details/gzqsanljk.sHtML

[S32] C++：字符串
来源：http://3g.tarul.cn/Article/details/gxtbmykom.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.yfazqb.com/Article/details/gutogtgvi.sHtML

[S33] C++：vector 增删
来源：http://mobile.tarul.cn/Article/details/gvxteefng.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.sjlbkw.cn/Article/details/ghhyarypn.sHtML

[S34] C++：遍历 vector
来源：http://mobile.yfazqb.com/Article/details/gbewjudew.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fktsv.cn/Article/details/gkxhtykyy.sHtML

[S35] C++：map
来源：http://blog.bbcook.cn/Article/details/gdsgaaqxp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gmrblaqhy.sHtML

[S36] C++：unordered_map
来源：http://3g.yfazqb.com/Article/details/gcdblwask.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gcvjxpeyu.sHtML

[S37] C++：set
来源：http://3g.bbcook.cn/Article/details/gsyflzvmr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fktsv.cn/Article/details/gdqrbzvpj.sHtML

[S38] C++：排序
来源：http://www.blog.sjlbkw.cn/Article/details/gfxqoklac.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.vehdjk.com/Article/details/gozxmjkhs.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.epnwcf.com/Article/details/gidddrxof.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.tarul.cn/Article/details/gtrmtypvr.sHtML

[S40] C++：查找元素
来源：http://m.share.bbcook.cn/Article/details/gvftuaooo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fktsv.cn/Article/details/ghmmogwvc.sHtML

[S41] C++：类与构造函数
来源：http://wap.tarul.cn/Article/details/gctofsyhe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.sjlbkw.cn/Article/details/ggdbbwqca.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/gybmoxghu.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.vehdjk.com/Article/details/gslcgncnh.sHtML

[S43] C++：智能指针
来源：http://mobile.tarul.cn/Article/details/gwyokjqiq.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fktsv.cn/Article/details/grnqjupgd.sHtML

[S44] C++：引用传参
来源：http://www.share.sjlbkw.cn/Article/details/gdgjvtanf.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fktsv.cn/Article/details/glsjrcthx.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/goognqnxt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.epnwcf.com/Article/details/gacgshsgi.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gwthditoj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.yfazqb.com/Article/details/gxosmfwkf.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.epnwcf.com/Article/details/ghpzhjpsc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.bbcook.cn/Article/details/gssumcpuj.sHtML

[S48] C++：逐行读文件
来源：http://3g.tarul.cn/Article/details/gtdnllnft.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fktsv.cn/Article/details/ghekchapv.sHtML

while (std::getline(in, line)) { }
来源：http://blog.sjlbkw.cn/Article/details/gcqbkzgiy.sHtML

[S49] C++：写文件
来源：http://www.share.fktsv.cn/Article/details/gizccncwf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.tarul.cn/Article/details/gbakvsfsg.sHtML

[S50] C++：格式化数字
来源：http://m.share.sjlbkw.cn/Article/details/gxtiagskw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gcklwhcfg.sHtML

[S51] C++：显式类型转换
来源：http://baike.vehdjk.com/Article/details/gqpmjkmhy.sHtML

static_cast<double>(a) / b
来源：http://m.share.fktsv.cn/Article/details/ghbfkyweb.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fktsv.cn/Article/details/gnbokmbun.sHtML

int size() const noexcept { return n_; }
来源：http://blog.sjlbkw.cn/Article/details/gfcrsiicu.sHtML

[S53] C++：移动语义
来源：http://www.share.sjlbkw.cn/Article/details/gremyppuw.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.tarul.cn/Article/details/gottccgpj.sHtML

[S54] C++：异常处理
来源：http://www.share.bbcook.cn/Article/details/gdphdohux.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.vehdjk.com/Article/details/gechavsjg.sHtML

[S55] C++：结构化绑定
来源：http://m.share.yfazqb.com/Article/details/gyxaupbjb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.epnwcf.com/Article/details/gwayouckr.sHtML

[S56] C++：optional
来源：http://www.m.share.vehdjk.com/Article/details/gntfoheyf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.yfazqb.com/Article/details/gbizrzrzs.sHtML

[S57] C++：编译期常量
来源：http://blog.tarul.cn/Article/details/gydniuzwn.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/ghtwzogsw.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gpwvtsuam.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.yfazqb.com/Article/details/gihnznggt.sHtML

[S59] C++：静态断言
来源：http://www.m.share.bbcook.cn/Article/details/ggadlbbuf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.yfazqb.com/Article/details/gnqarkiul.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.tarul.cn/Article/details/gqilskave.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gdccvjvga.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gebszjolf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/ghyzcvqdf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfddjooqu.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fktsv.cn/Article/details/gejxqfdlb.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gwsuuszwx.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fktsv.cn/Article/details/gxvlckncu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.bbcook.cn/Article/details/gofzgcvlb.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.vehdjk.com/Article/details/gsrnskxyh.sHtML

"值: $b"
来源：http://www.blog.tarul.cn/Article/details/gimqxxjhm.sHtML

[T04] Kotlin：空安全
来源：http://m.share.sjlbkw.cn/Article/details/gulvocqbr.sHtML

val n: String? = null;  n?.length
来源：http://3g.sjlbkw.cn/Article/details/geddjaony.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.vehdjk.com/Article/details/ghxvycgpy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.yfazqb.com/Article/details/gglmfqaln.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.tarul.cn/Article/details/gjlrtkjox.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.bbcook.cn/Article/details/gsrookugq.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.epnwcf.com/Article/details/gazdylxfc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.epnwcf.com/Article/details/grqmzdhis.sHtML

[T08] Kotlin：数据类
来源：http://m.share.sjlbkw.cn/Article/details/gtolrulfv.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.tarul.cn/Article/details/gdizrvdiq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fktsv.cn/Article/details/gdpqydybs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.epnwcf.com/Article/details/gdataldju.sHtML

[T10] Kotlin：默认参数
来源：http://3g.yfazqb.com/Article/details/gamdflwgr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.sjlbkw.cn/Article/details/gducfzpko.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/grrasftro.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.sjlbkw.cn/Article/details/geudelfqe.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/gkovuloji.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gexmzaarz.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.sjlbkw.cn/Article/details/gcsxzoqio.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.tarul.cn/Article/details/gbczlolpo.sHtML

[T14] Kotlin：循环
来源：http://read.share.fktsv.cn/Article/details/ghpstmkla.sHtML

for (i in 1..10) println(i)
来源：http://blog.epnwcf.com/Article/details/glicpowhh.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.tarul.cn/Article/details/gqvgzwima.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.vehdjk.com/Article/details/gmzuvsjwy.sHtML

[T16] Swift：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gbjhdiqfw.sHtML

print("Hello")
来源：http://baike.sjlbkw.cn/Article/details/goifmufvh.sHtML

[T17] Swift：变量与常量
来源：http://blog.tarul.cn/Article/details/guujfkbki.sHtML

var a = 1;  let b = 2
来源：http://m.share.yfazqb.com/Article/details/gaqcbydil.sHtML

[T18] Swift：字符串插值
来源：http://3g.bbcook.cn/Article/details/gzzoknykl.sHtML

"值: \(b)"
来源：http://www.share.sjlbkw.cn/Article/details/gblvliaov.sHtML

[T19] Swift：可选绑定
来源：http://blog.tarul.cn/Article/details/gaivbgacg.sHtML

if let n = opt { print(n) }
来源：http://wap.vehdjk.com/Article/details/gbrnlwrqa.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvqxitdq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.bbcook.cn/Article/details/gvahwkbyy.sHtML

[T21] Swift：遍历
来源：http://www.blog.vehdjk.com/Article/details/ghzifctlg.sHtML

for x in a { print(x) }
来源：http://www.m.share.vehdjk.com/Article/details/gjixgubgq.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/ghwjjabxr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.yfazqb.com/Article/details/gnsvoaqys.sHtML

[T23] Swift：函数
来源：http://www.blog.bbcook.cn/Article/details/ggogeqsiy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.tarul.cn/Article/details/gbqxxvxuo.sHtML

[T24] Swift：闭包
来源：http://wap.fktsv.cn/Article/details/gwmrmxfqm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.bbcook.cn/Article/details/ghognssre.sHtML

[T25] Swift：结构体
来源：http://baike.sjlbkw.cn/Article/details/gujipjkha.sHtML

struct P { var x: Int }
来源：http://3g.yfazqb.com/Article/details/ghwouszgp.sHtML

[T26] Swift：类与重写
来源：http://mobile.fktsv.cn/Article/details/gfrybeylb.sHtML

class A: Base { override func f() {} }
来源：http://baike.fktsv.cn/Article/details/gwilocvgj.sHtML

[T27] Swift：错误处理
来源：http://3g.yfazqb.com/Article/details/gyoenknzu.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.vehdjk.com/Article/details/gymjgngdo.sHtML

[T28] Swift：枚举
来源：http://blog.fktsv.cn/Article/details/gggbghouo.sHtML

enum Color { case red, green }
来源：http://baike.fktsv.cn/Article/details/gtkgxocsv.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.sjlbkw.cn/Article/details/gfhfxwulk.sHtML

guard let x = opt else { return }
来源：http://baike.vehdjk.com/Article/details/gkyzvkjmh.sHtML

[T30] Swift：协议
来源：http://mobile.tarul.cn/Article/details/gqbfgowah.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.vehdjk.com/Article/details/gxbutxfai.sHtML

[T31] Lua：Hello World
来源：http://read.share.bbcook.cn/Article/details/gaaimudtv.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gpescbvmb.sHtML

[T32] Lua：局部变量
来源：http://blog.yfazqb.com/Article/details/gffdrkyyi.sHtML

local a = 1
来源：http://www.share.tarul.cn/Article/details/gwwjcqxyh.sHtML

[T33] Lua：表（数组）
来源：http://mobile.bbcook.cn/Article/details/gsywakpsx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.vehdjk.com/Article/details/giuskfsni.sHtML

[T34] Lua：遍历表
来源：http://baike.vehdjk.com/Article/details/gsofcehey.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fktsv.cn/Article/details/gmlezetmj.sHtML

[T35] Lua：字典表
来源：http://baike.epnwcf.com/Article/details/gtyckvolt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.tarul.cn/Article/details/gvcsxojdw.sHtML

[T36] Lua：函数
来源：http://3g.tarul.cn/Article/details/ghkmdenwj.sHtML

function add(a, b) return a + b end
来源：http://blog.sjlbkw.cn/Article/details/gbrtoqnsl.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gnybkyfms.sHtML

"a" .. "b"
来源：http://wap.epnwcf.com/Article/details/gxluwfqey.sHtML

[T38] Lua：条件
来源：http://www.blog.sjlbkw.cn/Article/details/gejzaqriw.sHtML

if x > 0 then print("正") end
来源：http://www.blog.epnwcf.com/Article/details/gglpjyaxt.sHtML


<!-- 参考信息 -->