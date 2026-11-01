代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.bbcook.cn/Article/details/gxdkzdjvr.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/gnhetkjgb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fktsv.cn/Article/details/ghsogsssz.sHtML

[R31] 局部变量
来源：http://baike.epnwcf.com/Article/details/ggchrxelf.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.sjlbkw.cn/Article/details/geqhfcoqa.sHtML

[R32] 参数个数校验
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdmddiyp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/gwzsxtjro.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.vehdjk.com/Article/details/gfitabeia.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.bbcook.cn/Article/details/gwpipfjwi.sHtML

[R34] 退出时清理
来源：http://read.share.sjlbkw.cn/Article/details/gddcdmpqy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gzwvmkcno.sHtML

[R35] 后台执行并等待
来源：http://wap.vehdjk.com/Article/details/gqrelbzyu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.vehdjk.com/Article/details/gnhlodkwn.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.epnwcf.com/Article/details/gslihvaor.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.tarul.cn/Article/details/gkctizxlc.sHtML

[R37] 把输出赋给变量
来源：http://wap.yfazqb.com/Article/details/ggqlqprcf.sHtML

files=$(ls -1)
来源：http://wap.yfazqb.com/Article/details/gfzirmgha.sHtML

[R38] 管道串联
来源：http://3g.tarul.cn/Article/details/gwzuvqmwv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.yfazqb.com/Article/details/gpucgxhgk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.epnwcf.com/Article/details/gcbofrgrg.sHtML

cmd > out.log 2>&1
来源：http://mobile.tarul.cn/Article/details/gvccyikci.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/gckvarshk.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/ghfontdjv.sHtML

[R41] 丢弃输出
来源：http://read.share.bbcook.cn/Article/details/gcudrxrol.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/gjhzwekht.sHtML

[R42] 输入重定向
来源：http://www.m.share.yfazqb.com/Article/details/gxjkloduj.sHtML

wc -l < a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gwyeozgto.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.yfazqb.com/Article/details/givfmyaqv.sHtML

find . -name "*.log" -type f
来源：http://baike.tarul.cn/Article/details/gwmudgpev.sHtML

[R44] 按修改时间查找
来源：http://wap.epnwcf.com/Article/details/gjdbphymq.sHtML

find . -mtime -7 -type f
来源：http://baike.epnwcf.com/Article/details/ghijygyzj.sHtML

[R45] 批量删除
来源：http://www.share.bbcook.cn/Article/details/gpntqcmtk.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.sjlbkw.cn/Article/details/gcogjmugk.sHtML

[R46] 递归替换文件内容
来源：http://wap.vehdjk.com/Article/details/gzvmykxeo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.yfazqb.com/Article/details/gmxzfaqgh.sHtML

[R47] sed 单行替换
来源：http://3g.sjlbkw.cn/Article/details/gpfnjrylw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/guyfdsvfe.sHtML

[R48] awk 取指定列
来源：http://m.share.bbcook.cn/Article/details/gsaytnqeg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gmpcyifsv.sHtML

[R49] awk 带条件
来源：http://www.m.share.vehdjk.com/Article/details/gklaoseiv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.vehdjk.com/Article/details/gvtqxifof.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/guqwllbtv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.tarul.cn/Article/details/glryyrpdl.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fktsv.cn/Article/details/gqlrekcxm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.sjlbkw.cn/Article/details/gbzfrooup.sHtML

[R52] 统计行数
来源：http://m.share.yfazqb.com/Article/details/gktuhvavh.sHtML

wc -l a.txt
来源：http://baike.fktsv.cn/Article/details/gmpsjkkxz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fktsv.cn/Article/details/gsfgfquwn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fktsv.cn/Article/details/gookvghoz.sHtML

[R54] 比较两个文件
来源：http://wap.tarul.cn/Article/details/gaofztysw.sHtML

diff a.txt b.txt
来源：http://m.share.tarul.cn/Article/details/gsyzxbntb.sHtML

[R55] 压缩与解压
来源：http://mobile.bbcook.cn/Article/details/geebyhklr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.epnwcf.com/Article/details/ghjpzglbu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gjcfpnogj.sHtML

scp file user@host:/path/
来源：http://baike.yfazqb.com/Article/details/gdqovjcwu.sHtML

[R57] 远程执行命令
来源：http://baike.vehdjk.com/Article/details/gtcwzyrle.sHtML

ssh user@host 'uptime'
来源：http://read.share.sjlbkw.cn/Article/details/gzpphduds.sHtML

[R58] 下载文件
来源：http://m.share.vehdjk.com/Article/details/gmprvzjco.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpqwpfme.sHtML

[R59] 发 POST JSON
来源：http://blog.epnwcf.com/Article/details/ggtifsjmo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.sjlbkw.cn/Article/details/gxcnhqubk.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/gpwtoutxv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.epnwcf.com/Article/details/guzxsjznf.sHtML

[R61] 磁盘占用
来源：http://wap.vehdjk.com/Article/details/ggmckgbwl.sHtML

df -h;  du -sh *
来源：http://3g.tarul.cn/Article/details/gkwqyhwir.sHtML

[R62] 找最占空间的文件
来源：http://baike.tarul.cn/Article/details/geoefnnvb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.sjlbkw.cn/Article/details/gyldhbvwc.sHtML

[R63] 内存与进程
来源：http://www.blog.sjlbkw.cn/Article/details/gsujqfeuu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fktsv.cn/Article/details/gdwyluroh.sHtML

[R64] 结束进程
来源：http://www.m.share.tarul.cn/Article/details/gvznybnvg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.vehdjk.com/Article/details/gntysqrto.sHtML

[R65] 查看端口占用
来源：http://blog.vehdjk.com/Article/details/giahpegtk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.yfazqb.com/Article/details/giovbjnpj.sHtML

[R66] 定时任务
来源：http://www.share.tarul.cn/Article/details/gcihouzek.sHtML

crontab -e;  crontab -l
来源：http://baike.fktsv.cn/Article/details/gusdzgcih.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fktsv.cn/Article/details/gbugeroiv.sHtML

openssl rand -hex 16
来源：http://m.share.yfazqb.com/Article/details/gnjzztfcf.sHtML

[R68] 计算文件校验值
来源：http://blog.sjlbkw.cn/Article/details/gnotoxbiv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fktsv.cn/Article/details/giisqyfsw.sHtML

[R69] 生成随机密码
来源：http://blog.sjlbkw.cn/Article/details/gzrjhiyzh.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.epnwcf.com/Article/details/gfrotltzh.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/gwboeqmwh.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.tarul.cn/Article/details/gdqeiogly.sHtML

[R71] 日期格式化
来源：http://wap.fktsv.cn/Article/details/goerooxyt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fktsv.cn/Article/details/gqyfnwuxx.sHtML

[R72] 等待端口就绪
来源：http://www.blog.sjlbkw.cn/Article/details/gjvqaxxpz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gjlgbclez.sHtML

[R73] 分割大日志
来源：http://m.share.vehdjk.com/Article/details/glvwcskwv.sHtML

split -l 1000 big.log part_
来源：http://www.share.tarul.cn/Article/details/gxixdfmbt.sHtML

[R74] 批量重命名
来源：http://www.share.vehdjk.com/Article/details/gwjypfler.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.sjlbkw.cn/Article/details/giwblahfp.sHtML

[R75] 导出环境变量
来源：http://blog.vehdjk.com/Article/details/grivmxjyt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.vehdjk.com/Article/details/gtcuzclne.sHtML

[R76] 使用临时文件
来源：http://3g.sjlbkw.cn/Article/details/gyxzftsnc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.vehdjk.com/Article/details/gttlnkikm.sHtML

[R77] 读取用户输入
来源：http://wap.sjlbkw.cn/Article/details/gohlpbnne.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.tarul.cn/Article/details/gsvrvrtrc.sHtML

[R78] 交互式菜单
来源：http://3g.epnwcf.com/Article/details/gkctawlnb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.sjlbkw.cn/Article/details/grwdmoktc.sHtML

[R79] 解析命令行选项
来源：http://m.share.yfazqb.com/Article/details/grmwuubyr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.vehdjk.com/Article/details/gzxwvfxev.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fktsv.cn/Article/details/gdczudmnz.sHtML

time ./run.sh
来源：http://3g.bbcook.cn/Article/details/gzhjvppfv.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqsvikzkt.sHtML

S. C / C++ 专题
来源：http://3g.sjlbkw.cn/Article/details/gxkqvgznx.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnvwxshsy.sHtML

[S01] C：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gffxnzajn.sHtML

#include <stdio.h>
来源：http://baike.fktsv.cn/Article/details/gdgpsyzgz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gestxldoi.sHtML

[S02] C：变量与格式化输出
来源：http://blog.bbcook.cn/Article/details/gtymhqmty.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.vehdjk.com/Article/details/gybtjmpot.sHtML

[S03] C：读入整数
来源：http://www.share.epnwcf.com/Article/details/gpqbdagam.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.tarul.cn/Article/details/gtpubbpkt.sHtML

[S04] C：字符串复制
来源：http://www.blog.bbcook.cn/Article/details/ghvzhlpys.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fktsv.cn/Article/details/gqgimfevw.sHtML

[S05] C：字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gvmkodnjo.sHtML

strlen(s)
来源：http://blog.vehdjk.com/Article/details/gobnsoygm.sHtML

[S06] C：字符串比较
来源：http://3g.yfazqb.com/Article/details/gxpcvvtky.sHtML

strcmp(a, b) == 0
来源：http://mobile.yfazqb.com/Article/details/gxdzdvnzl.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/gvjuphhhf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fktsv.cn/Article/details/gbkgfuiok.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fktsv.cn/Article/details/gyrcoklvb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.bbcook.cn/Article/details/glarqriqc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.sjlbkw.cn/Article/details/grhekvntv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.epnwcf.com/Article/details/gtbqkjssb.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fktsv.cn/Article/details/gepcvzucc.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.tarul.cn/Article/details/gsulmnjdv.sHtML

[S11] C：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/ghxaoqryv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fktsv.cn/Article/details/gfedfkwsw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gwbojwdyj.sHtML

fclose(f);
来源：http://wap.vehdjk.com/Article/details/gifgvrodc.sHtML

[S12] C：写文件
来源：http://3g.yfazqb.com/Article/details/gteycryhm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.bbcook.cn/Article/details/ghtpfvvdd.sHtML

[S13] C：宏定义
来源：http://3g.fktsv.cn/Article/details/gsvwghkqm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/gbpywtomy.sHtML

[S14] C：枚举
来源：http://m.share.bbcook.cn/Article/details/gnjghsqgk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.yfazqb.com/Article/details/gjfpfzmwr.sHtML

[S15] C：类型转换
来源：http://wap.sjlbkw.cn/Article/details/gdgnwdckv.sHtML

(double) a / b
来源：http://mobile.yfazqb.com/Article/details/gptnvuztd.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fktsv.cn/Article/details/gszgqivoh.sHtML

x |= (1 << 3);
来源：http://m.share.yfazqb.com/Article/details/gcqjxyrpl.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gqtodrvhi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fktsv.cn/Article/details/gaitqmhkc.sHtML

[S18] C：命令行参数
来源：http://www.share.sjlbkw.cn/Article/details/gqemjdmgc.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.vehdjk.com/Article/details/gozjvnxpc.sHtML

[S19] C：快速排序
来源：http://3g.fktsv.cn/Article/details/grnkebtfk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/grcjvbqaz.sHtML

[S20] C：二分查找
来源：http://www.share.epnwcf.com/Article/details/golazuttw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gcftubqrw.sHtML

[S21] C：字符类别判断
来源：http://mobile.fktsv.cn/Article/details/grzwycarr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.tarul.cn/Article/details/gsumlmtog.sHtML

[S22] C：字符串转数字
来源：http://baike.bbcook.cn/Article/details/gtnyfcstg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.sjlbkw.cn/Article/details/givwfxmmz.sHtML

[S23] C：随机数
来源：http://3g.sjlbkw.cn/Article/details/gnwekftxa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.tarul.cn/Article/details/gcsoxyrkq.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.yfazqb.com/Article/details/ghzoqpxvt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.yfazqb.com/Article/details/gnzvsddzh.sHtML

[S25] C：内存拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gkczzdnnv.sHtML

memcpy(dst, src, n);
来源：http://blog.fktsv.cn/Article/details/gckwltfss.sHtML

[S26] C：内存清零
来源：http://m.share.fktsv.cn/Article/details/gkooxunkt.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fktsv.cn/Article/details/gkilyotqg.sHtML

[S27] C：定义常量
来源：http://m.share.vehdjk.com/Article/details/gzbupzpaa.sHtML

const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gynhalzmx.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/gniqbdajt.sHtML

static int counter = 0;
来源：http://blog.sjlbkw.cn/Article/details/gnmvhqsud.sHtML

[S29] C：变参函数
来源：http://m.share.vehdjk.com/Article/details/gmjmwlwnh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.bbcook.cn/Article/details/gkwpckomy.sHtML

[S30] C：头文件保护
来源：http://wap.vehdjk.com/Article/details/gjwuzqwxz.sHtML

#ifndef X_H
来源：http://3g.bbcook.cn/Article/details/gazczjrxn.sHtML

#define X_H
来源：http://read.share.sjlbkw.cn/Article/details/gllwvnicz.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/ghgnwhrbo.sHtML

[S31] C++：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gkqormnls.sHtML

#include <iostream>
来源：http://blog.bbcook.cn/Article/details/gsqguwqec.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.tarul.cn/Article/details/gwgqcqhuk.sHtML

[S32] C++：字符串
来源：http://www.share.sjlbkw.cn/Article/details/gjojmbydk.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.bbcook.cn/Article/details/gmskbhstq.sHtML

[S33] C++：vector 增删
来源：http://wap.vehdjk.com/Article/details/ginywseqv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.yfazqb.com/Article/details/gwmhggxgc.sHtML

[S34] C++：遍历 vector
来源：http://baike.bbcook.cn/Article/details/gocpyfzrp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.yfazqb.com/Article/details/gilutptqz.sHtML

[S35] C++：map
来源：http://wap.yfazqb.com/Article/details/gxopogapn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gkkitshjb.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.yfazqb.com/Article/details/gojoxymol.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/glzxrxirr.sHtML

[S37] C++：set
来源：http://www.share.vehdjk.com/Article/details/gociknnrx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.tarul.cn/Article/details/guezfwvbb.sHtML

[S38] C++：排序
来源：http://www.blog.bbcook.cn/Article/details/gfqmstsnh.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.tarul.cn/Article/details/gctiojkub.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.tarul.cn/Article/details/giknzziaa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.epnwcf.com/Article/details/gkjxlxekw.sHtML

[S40] C++：查找元素
来源：http://www.blog.epnwcf.com/Article/details/giloljilt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.bbcook.cn/Article/details/gvfovtceb.sHtML

[S41] C++：类与构造函数
来源：http://mobile.yfazqb.com/Article/details/gxjokuwiq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.bbcook.cn/Article/details/gpslovuhs.sHtML

[S42] C++：继承与虚函数
来源：http://wap.vehdjk.com/Article/details/gxkatvxck.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/gcatbozts.sHtML

[S43] C++：智能指针
来源：http://mobile.fktsv.cn/Article/details/ggeysvgot.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/gmvergwtb.sHtML

[S44] C++：引用传参
来源：http://blog.vehdjk.com/Article/details/ggotskbkk.sHtML

void inc(int &x) { ++x; }
来源：http://blog.vehdjk.com/Article/details/gsnbbymqd.sHtML

[S45] C++：lambda
来源：http://www.blog.tarul.cn/Article/details/gnkdyzcqu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.bbcook.cn/Article/details/gabprbdyr.sHtML

[S46] C++：函数模板
来源：http://www.blog.sjlbkw.cn/Article/details/gcgdzbwys.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.sjlbkw.cn/Article/details/gbjmjtjwj.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.epnwcf.com/Article/details/gcvtxbtev.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.epnwcf.com/Article/details/gfjhmtahp.sHtML

[S48] C++：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gofupnnkr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.bbcook.cn/Article/details/gvlixrosn.sHtML

while (std::getline(in, line)) { }
来源：http://wap.epnwcf.com/Article/details/gxfhvcpsn.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/goedbrptz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/gotgkajnp.sHtML

[S50] C++：格式化数字
来源：http://blog.fktsv.cn/Article/details/gjomjmxzp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gmgdhmbgk.sHtML

[S51] C++：显式类型转换
来源：http://www.share.epnwcf.com/Article/details/gntkgizic.sHtML

static_cast<double>(a) / b
来源：http://www.share.tarul.cn/Article/details/gmtuolnlh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.epnwcf.com/Article/details/gjsxycvbz.sHtML

int size() const noexcept { return n_; }
来源：http://blog.bbcook.cn/Article/details/gkdscwcpk.sHtML

[S53] C++：移动语义
来源：http://wap.bbcook.cn/Article/details/gokuyxpjj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fktsv.cn/Article/details/gchgbpsvv.sHtML

[S54] C++：异常处理
来源：http://baike.bbcook.cn/Article/details/goymnseok.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.tarul.cn/Article/details/gpvxhhdhh.sHtML

[S55] C++：结构化绑定
来源：http://wap.fktsv.cn/Article/details/gfgoztdvu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.bbcook.cn/Article/details/gvrsqpeyd.sHtML

[S56] C++：optional
来源：http://blog.yfazqb.com/Article/details/gzlggytsp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.yfazqb.com/Article/details/gqfqnyteg.sHtML

[S57] C++：编译期常量
来源：http://read.share.tarul.cn/Article/details/gfnvzttpj.sHtML

constexpr int N = 10;
来源：http://read.share.epnwcf.com/Article/details/gmczhwjit.sHtML

[S58] C++：命名空间
来源：http://blog.vehdjk.com/Article/details/gmldkvjvi.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.epnwcf.com/Article/details/ghuzoezou.sHtML

[S59] C++：静态断言
来源：http://www.m.share.bbcook.cn/Article/details/grmsnxoro.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.bbcook.cn/Article/details/guyxcouns.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.yfazqb.com/Article/details/gyclvubjj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.vehdjk.com/Article/details/gzuujvrdj.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gfwvrhhom.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gevghrjxp.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gmtakjjsl.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.tarul.cn/Article/details/gaqgvgopb.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/gxrrhmjos.sHtML

[T02] Kotlin：变量
来源：http://www.blog.epnwcf.com/Article/details/gdcblfvtb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.bbcook.cn/Article/details/guojsmcrl.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.bbcook.cn/Article/details/grnvxjgdj.sHtML

"值: $b"
来源：http://3g.fktsv.cn/Article/details/gmsnbvxhe.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fktsv.cn/Article/details/gexiuoddb.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.epnwcf.com/Article/details/gonqjgbzf.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.bbcook.cn/Article/details/ggzqxibdf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.sjlbkw.cn/Article/details/gjztfuyxi.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.vehdjk.com/Article/details/gtopevuhe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.yfazqb.com/Article/details/gfbkqctgp.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/ghurnkpfu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.tarul.cn/Article/details/gmqpfsvtn.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.sjlbkw.cn/Article/details/gspqcgwkn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.epnwcf.com/Article/details/garxvohtn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.bbcook.cn/Article/details/gyhrrrrye.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.vehdjk.com/Article/details/gokwxifim.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.vehdjk.com/Article/details/golghhlgk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.vehdjk.com/Article/details/glnxtaack.sHtML

[T11] Kotlin：协程
来源：http://m.share.fktsv.cn/Article/details/gpudldbob.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fktsv.cn/Article/details/ggximlvaz.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.tarul.cn/Article/details/geixwsihz.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.vehdjk.com/Article/details/gadccywvy.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.epnwcf.com/Article/details/gqvqosgwg.sHtML

val m = mapOf("a" to 1)
来源：http://blog.sjlbkw.cn/Article/details/gsvyhojyf.sHtML

[T14] Kotlin：循环
来源：http://blog.vehdjk.com/Article/details/gqhuqtdoz.sHtML

for (i in 1..10) println(i)
来源：http://www.share.vehdjk.com/Article/details/ggbjsbbql.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.bbcook.cn/Article/details/glazekevw.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.vehdjk.com/Article/details/ghwbnbbza.sHtML

[T16] Swift：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gaagdkvvv.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gsjzjuzev.sHtML

[T17] Swift：变量与常量
来源：http://blog.vehdjk.com/Article/details/gmdtniydg.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/gxiypcosq.sHtML

[T18] Swift：字符串插值
来源：http://baike.yfazqb.com/Article/details/gojwsfsor.sHtML

"值: \(b)"
来源：http://3g.sjlbkw.cn/Article/details/giniglsqn.sHtML

[T19] Swift：可选绑定
来源：http://3g.tarul.cn/Article/details/gxgoubwet.sHtML

if let n = opt { print(n) }
来源：http://3g.yfazqb.com/Article/details/ghsqudymy.sHtML

[T20] Swift：数组操作
来源：http://mobile.sjlbkw.cn/Article/details/gielwjalg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.vehdjk.com/Article/details/gqipjjyng.sHtML

[T21] Swift：遍历
来源：http://3g.bbcook.cn/Article/details/gesblpage.sHtML

for x in a { print(x) }
来源：http://blog.yfazqb.com/Article/details/gemnmxeqv.sHtML

[T22] Swift：字典
来源：http://baike.vehdjk.com/Article/details/gclnrdcfj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fktsv.cn/Article/details/gjrmrjlsx.sHtML

[T23] Swift：函数
来源：http://read.share.yfazqb.com/Article/details/glnbblbtj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.yfazqb.com/Article/details/gelcluske.sHtML

[T24] Swift：闭包
来源：http://blog.fktsv.cn/Article/details/goxfgouqj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.epnwcf.com/Article/details/gqekeehzj.sHtML

[T25] Swift：结构体
来源：http://www.m.share.tarul.cn/Article/details/glqmdtmdn.sHtML

struct P { var x: Int }
来源：http://read.share.vehdjk.com/Article/details/grijrpanm.sHtML

[T26] Swift：类与重写
来源：http://3g.sjlbkw.cn/Article/details/gemjhbpbh.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.sjlbkw.cn/Article/details/gbuqqldkw.sHtML

[T27] Swift：错误处理
来源：http://baike.epnwcf.com/Article/details/ggcslwfef.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.bbcook.cn/Article/details/ggmtxsckl.sHtML

[T28] Swift：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gczgbreyb.sHtML

enum Color { case red, green }
来源：http://m.share.vehdjk.com/Article/details/gpingfzam.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.sjlbkw.cn/Article/details/gyshfrqsa.sHtML

guard let x = opt else { return }
来源：http://mobile.vehdjk.com/Article/details/guyddesqp.sHtML

[T30] Swift：协议
来源：http://mobile.yfazqb.com/Article/details/gqgqcoybl.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.epnwcf.com/Article/details/gnrqsdvoc.sHtML

[T31] Lua：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gihednaju.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/glgmmcoat.sHtML

[T32] Lua：局部变量
来源：http://read.share.vehdjk.com/Article/details/gwbzlnawb.sHtML

local a = 1
来源：http://wap.sjlbkw.cn/Article/details/gwaoayonj.sHtML


<!-- 参考信息 -->