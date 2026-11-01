代发 wailian999

echo $((1 + 2 * 3))
来源：http://blog.fktsv.cn/Article/details/gvnmfegkn.sHtML

[R28] 浮点运算
来源：http://baike.epnwcf.com/Article/details/gnixnswmm.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.tarul.cn/Article/details/gyvizyoxc.sHtML

[R29] 定义函数
来源：http://www.share.fktsv.cn/Article/details/golgepuey.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.sjlbkw.cn/Article/details/ggazezbcb.sHtML

[R30] 函数返回状态码
来源：http://baike.vehdjk.com/Article/details/gfepuyxfo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.yfazqb.com/Article/details/ghgpmtlqd.sHtML

[R31] 局部变量
来源：http://m.share.yfazqb.com/Article/details/gjmaafuxa.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.yfazqb.com/Article/details/gobncxteq.sHtML

[R32] 参数个数校验
来源：http://www.blog.fktsv.cn/Article/details/gssstaesu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/goiwnpxzm.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.tarul.cn/Article/details/glirrjkaj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fktsv.cn/Article/details/ggpwywuqq.sHtML

[R34] 退出时清理
来源：http://wap.yfazqb.com/Article/details/gzeehyqoy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/goztcbrxb.sHtML

[R35] 后台执行并等待
来源：http://wap.vehdjk.com/Article/details/gvlofycjt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcseybdk.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.bbcook.cn/Article/details/ghzqguodi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.tarul.cn/Article/details/geyfkxiuu.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.epnwcf.com/Article/details/gufdwrwby.sHtML

files=$(ls -1)
来源：http://www.m.share.bbcook.cn/Article/details/giqcxybgd.sHtML

[R38] 管道串联
来源：http://blog.vehdjk.com/Article/details/glldrrmrf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.epnwcf.com/Article/details/ghztgcrkg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fktsv.cn/Article/details/gknwirfhh.sHtML

cmd > out.log 2>&1
来源：http://mobile.yfazqb.com/Article/details/gofzosiyz.sHtML

[R40] 追加写日志
来源：http://baike.tarul.cn/Article/details/grbijujup.sHtML

echo "log" >> out.log
来源：http://wap.yfazqb.com/Article/details/gxiycmpzy.sHtML

[R41] 丢弃输出
来源：http://wap.sjlbkw.cn/Article/details/gcbqbqezh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.tarul.cn/Article/details/gmghftsct.sHtML

[R42] 输入重定向
来源：http://www.m.share.epnwcf.com/Article/details/gilwzdahf.sHtML

wc -l < a.txt
来源：http://m.share.yfazqb.com/Article/details/grpkyyaxl.sHtML

[R43] 按名字查找文件
来源：http://read.share.bbcook.cn/Article/details/gfwlnyqls.sHtML

find . -name "*.log" -type f
来源：http://read.share.bbcook.cn/Article/details/gpozqymlm.sHtML

[R44] 按修改时间查找
来源：http://read.share.epnwcf.com/Article/details/gwxohiano.sHtML

find . -mtime -7 -type f
来源：http://blog.tarul.cn/Article/details/gelgwklhm.sHtML

[R45] 批量删除
来源：http://www.blog.vehdjk.com/Article/details/gxdniegrn.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fktsv.cn/Article/details/gxbfqezlr.sHtML

[R46] 递归替换文件内容
来源：http://blog.yfazqb.com/Article/details/gjwdoovzt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.epnwcf.com/Article/details/gnrxckpxq.sHtML

[R47] sed 单行替换
来源：http://wap.fktsv.cn/Article/details/gdjryajhb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gavjakygm.sHtML

[R48] awk 取指定列
来源：http://www.m.share.yfazqb.com/Article/details/grjzssgtu.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.tarul.cn/Article/details/gvzegulzb.sHtML

[R49] awk 带条件
来源：http://www.m.share.bbcook.cn/Article/details/gcbxykzbd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.yfazqb.com/Article/details/giapvwoye.sHtML

[R50] awk 求和
来源：http://mobile.sjlbkw.cn/Article/details/geufpgnod.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/ggjyblpwj.sHtML

[R51] 排序去重取前几
来源：http://m.share.vehdjk.com/Article/details/gtwrasmua.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.yfazqb.com/Article/details/glqneaxji.sHtML

[R52] 统计行数
来源：http://www.m.share.fktsv.cn/Article/details/geoxrtzow.sHtML

wc -l a.txt
来源：http://www.share.epnwcf.com/Article/details/gvqdjwieg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.bbcook.cn/Article/details/ghlsjgetl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.tarul.cn/Article/details/gzkeybgwh.sHtML

[R54] 比较两个文件
来源：http://blog.bbcook.cn/Article/details/gwbilrbjb.sHtML

diff a.txt b.txt
来源：http://www.m.share.tarul.cn/Article/details/gykavhydj.sHtML

[R55] 压缩与解压
来源：http://blog.tarul.cn/Article/details/gjtkgyrkg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.bbcook.cn/Article/details/grxcbovsz.sHtML

[R56] 远程拷贝
来源：http://3g.epnwcf.com/Article/details/gozhorrho.sHtML

scp file user@host:/path/
来源：http://www.blog.yfazqb.com/Article/details/gwtlqvfrg.sHtML

[R57] 远程执行命令
来源：http://3g.yfazqb.com/Article/details/gqkemfown.sHtML

ssh user@host 'uptime'
来源：http://3g.sjlbkw.cn/Article/details/gwcofkluu.sHtML

[R58] 下载文件
来源：http://m.share.bbcook.cn/Article/details/gdujqjfjk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.sjlbkw.cn/Article/details/gtkyxjvew.sHtML

[R59] 发 POST JSON
来源：http://baike.vehdjk.com/Article/details/gvycswwyd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.vehdjk.com/Article/details/gwutifnyj.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/gojhvpukn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.epnwcf.com/Article/details/gzgvopqyq.sHtML

[R61] 磁盘占用
来源：http://m.share.fktsv.cn/Article/details/gnohcehoe.sHtML

df -h;  du -sh *
来源：http://www.blog.bbcook.cn/Article/details/glkuamkps.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/glpkccpmm.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.yfazqb.com/Article/details/gixlwykiy.sHtML

[R63] 内存与进程
来源：http://mobile.yfazqb.com/Article/details/gudampqqj.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fktsv.cn/Article/details/goxymvdvw.sHtML

[R64] 结束进程
来源：http://www.blog.yfazqb.com/Article/details/gcednpats.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.vehdjk.com/Article/details/ghpfjzyqd.sHtML

[R65] 查看端口占用
来源：http://www.blog.sjlbkw.cn/Article/details/ggschuyzz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fktsv.cn/Article/details/gxiqgkbqy.sHtML

[R66] 定时任务
来源：http://read.share.tarul.cn/Article/details/grdkxqeff.sHtML

crontab -e;  crontab -l
来源：http://blog.fktsv.cn/Article/details/gqzgpcsvi.sHtML

[R67] 生成随机十六进制串
来源：http://wap.bbcook.cn/Article/details/grvhnpkwa.sHtML

openssl rand -hex 16
来源：http://www.blog.fktsv.cn/Article/details/gydlqgrcb.sHtML

[R68] 计算文件校验值
来源：http://blog.vehdjk.com/Article/details/gbdlkjszp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fktsv.cn/Article/details/gpjvhmikk.sHtML

[R69] 生成随机密码
来源：http://baike.tarul.cn/Article/details/ghlibzvju.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.yfazqb.com/Article/details/gedwzepwj.sHtML

[R70] 时间戳与互转
来源：http://www.blog.yfazqb.com/Article/details/ggquzjlsk.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.epnwcf.com/Article/details/gotjsskog.sHtML

[R71] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gzxzzymut.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.epnwcf.com/Article/details/gnngsuqzd.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/gpupovgnu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/gqwwubkii.sHtML

[R73] 分割大日志
来源：http://wap.tarul.cn/Article/details/gjedmxekj.sHtML

split -l 1000 big.log part_
来源：http://blog.tarul.cn/Article/details/grdhsjjrx.sHtML

[R74] 批量重命名
来源：http://www.m.share.tarul.cn/Article/details/gsoewztif.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.vehdjk.com/Article/details/gxfzklohs.sHtML

[R75] 导出环境变量
来源：http://blog.vehdjk.com/Article/details/gafesmmsl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.vehdjk.com/Article/details/gguvaqwmi.sHtML

[R76] 使用临时文件
来源：http://www.share.yfazqb.com/Article/details/gzzwtecpj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/glanszefv.sHtML

[R77] 读取用户输入
来源：http://3g.fktsv.cn/Article/details/gwxdrxyre.sHtML

read -rp "请输入: " ans
来源：http://wap.sjlbkw.cn/Article/details/grfjligcb.sHtML

[R78] 交互式菜单
来源：http://blog.epnwcf.com/Article/details/gacwxtiga.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/gzfzhigpu.sHtML

[R79] 解析命令行选项
来源：http://wap.vehdjk.com/Article/details/gcggxuwsx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.sjlbkw.cn/Article/details/gmdaybpkk.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.bbcook.cn/Article/details/gjlzgdici.sHtML

time ./run.sh
来源：http://www.blog.fktsv.cn/Article/details/giabcewzp.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gevekrtsc.sHtML

S. C / C++ 专题
来源：http://blog.vehdjk.com/Article/details/gwbszxaad.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gveqifzad.sHtML

[S01] C：Hello World
来源：http://mobile.epnwcf.com/Article/details/guviowqbp.sHtML

#include <stdio.h>
来源：http://blog.yfazqb.com/Article/details/gpcakffqw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/gqybykeee.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.sjlbkw.cn/Article/details/gocltqaxh.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.bbcook.cn/Article/details/gpsmpehuy.sHtML

[S03] C：读入整数
来源：http://blog.vehdjk.com/Article/details/gffzkvqhm.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.epnwcf.com/Article/details/gvndbjquy.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/ggacmyzzy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fktsv.cn/Article/details/gkacuitre.sHtML

[S05] C：字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gfkxagfcb.sHtML

strlen(s)
来源：http://www.share.yfazqb.com/Article/details/gldhimcvm.sHtML

[S06] C：字符串比较
来源：http://www.blog.epnwcf.com/Article/details/giwfhpnzq.sHtML

strcmp(a, b) == 0
来源：http://blog.yfazqb.com/Article/details/goaggxbqf.sHtML

[S07] C：数组遍历求和
来源：http://baike.bbcook.cn/Article/details/gvflsnfov.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.bbcook.cn/Article/details/gklxmacdv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdaxpsre.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.tarul.cn/Article/details/gixnmqgnz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.tarul.cn/Article/details/gszifscox.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fktsv.cn/Article/details/gfbazvuzj.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gafelngqr.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.tarul.cn/Article/details/gkmdhcjnb.sHtML

[S11] C：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gpsnzbgch.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.bbcook.cn/Article/details/gbfwyndox.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.tarul.cn/Article/details/gcochldlg.sHtML

fclose(f);
来源：http://wap.vehdjk.com/Article/details/gkmrgvutf.sHtML

[S12] C：写文件
来源：http://www.share.vehdjk.com/Article/details/giybtzrvo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gumgkvqul.sHtML

[S13] C：宏定义
来源：http://blog.tarul.cn/Article/details/gemoahlzz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.sjlbkw.cn/Article/details/gebigoxyi.sHtML

[S14] C：枚举
来源：http://www.blog.bbcook.cn/Article/details/gxnnselms.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.vehdjk.com/Article/details/gjuaeoaul.sHtML

[S15] C：类型转换
来源：http://m.share.vehdjk.com/Article/details/gmqkirfpb.sHtML

(double) a / b
来源：http://3g.sjlbkw.cn/Article/details/gikufeysq.sHtML

[S16] C：位操作置位
来源：http://read.share.fktsv.cn/Article/details/geyfhncyd.sHtML

x |= (1 << 3);
来源：http://baike.sjlbkw.cn/Article/details/gwlctidvk.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/gtkugwnek.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.yfazqb.com/Article/details/gvmyhqgog.sHtML

[S18] C：命令行参数
来源：http://read.share.fktsv.cn/Article/details/gpacuwcea.sHtML

int main(int argc, char **argv)
来源：http://www.blog.tarul.cn/Article/details/gccwhaldx.sHtML

[S19] C：快速排序
来源：http://m.share.bbcook.cn/Article/details/guvyfvcul.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/glaywmgto.sHtML

[S20] C：二分查找
来源：http://www.share.vehdjk.com/Article/details/grwskefxl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gjzvknejl.sHtML

[S21] C：字符类别判断
来源：http://blog.tarul.cn/Article/details/grmfuvuig.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.bbcook.cn/Article/details/gwzgjmlqg.sHtML

[S22] C：字符串转数字
来源：http://mobile.yfazqb.com/Article/details/glgvjxsvo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fktsv.cn/Article/details/gdwpetrks.sHtML

[S23] C：随机数
来源：http://3g.yfazqb.com/Article/details/gvduyrkar.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.sjlbkw.cn/Article/details/gtswqqlvu.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.tarul.cn/Article/details/gzolmdwle.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.yfazqb.com/Article/details/gfvujinis.sHtML

[S25] C：内存拷贝
来源：http://blog.vehdjk.com/Article/details/gxxvsqblb.sHtML

memcpy(dst, src, n);
来源：http://read.share.vehdjk.com/Article/details/gmxkksmli.sHtML

[S26] C：内存清零
来源：http://wap.fktsv.cn/Article/details/gsktklrwn.sHtML

memset(a, 0, sizeof a);
来源：http://wap.tarul.cn/Article/details/gumudxooz.sHtML

[S27] C：定义常量
来源：http://wap.epnwcf.com/Article/details/glkoaggtt.sHtML

const double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gdbsnyzoz.sHtML

[S28] C：静态变量
来源：http://mobile.tarul.cn/Article/details/gslmwzaob.sHtML

static int counter = 0;
来源：http://baike.tarul.cn/Article/details/gjtqvefjs.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/gwqwygzsf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.vehdjk.com/Article/details/gqddpekey.sHtML

[S30] C：头文件保护
来源：http://www.blog.fktsv.cn/Article/details/gglfwenij.sHtML

#ifndef X_H
来源：http://blog.epnwcf.com/Article/details/gtijdcbjd.sHtML

#define X_H
来源：http://read.share.sjlbkw.cn/Article/details/gtvjnksya.sHtML

#endif
来源：http://baike.fktsv.cn/Article/details/gerhgkfqb.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/grezfxiaw.sHtML

#include <iostream>
来源：http://3g.bbcook.cn/Article/details/gpgmxtwxt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/grymesnif.sHtML

[S32] C++：字符串
来源：http://mobile.yfazqb.com/Article/details/gyinhfytp.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.yfazqb.com/Article/details/ghpbqxcbc.sHtML

[S33] C++：vector 增删
来源：http://wap.sjlbkw.cn/Article/details/gvlaarxfg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.sjlbkw.cn/Article/details/gshjtsyyq.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.vehdjk.com/Article/details/gwysagwaz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.vehdjk.com/Article/details/ggvcwrhvc.sHtML

[S35] C++：map
来源：http://www.blog.fktsv.cn/Article/details/gtgcaozph.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gvjchdfyz.sHtML

[S36] C++：unordered_map
来源：http://wap.sjlbkw.cn/Article/details/gtqsmejpw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gcqwzvbfm.sHtML

[S37] C++：set
来源：http://blog.sjlbkw.cn/Article/details/glktvurxt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.bbcook.cn/Article/details/gpzjhkmxb.sHtML

[S38] C++：排序
来源：http://baike.tarul.cn/Article/details/grmfqoalx.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fktsv.cn/Article/details/grgkrfrzg.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.yfazqb.com/Article/details/gtijsoqip.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fktsv.cn/Article/details/ggaowxcce.sHtML

[S40] C++：查找元素
来源：http://www.blog.sjlbkw.cn/Article/details/gfesbdwtk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fktsv.cn/Article/details/gsljdigoc.sHtML

[S41] C++：类与构造函数
来源：http://read.share.tarul.cn/Article/details/gtavtfpsc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.yfazqb.com/Article/details/gtxhykkbo.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.bbcook.cn/Article/details/gowqexooi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.tarul.cn/Article/details/gnwgwvolu.sHtML

[S43] C++：智能指针
来源：http://read.share.fktsv.cn/Article/details/gnvqeijme.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.bbcook.cn/Article/details/gpnypcpyb.sHtML

[S44] C++：引用传参
来源：http://m.share.bbcook.cn/Article/details/gujhgkviu.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.epnwcf.com/Article/details/gdrkoptgn.sHtML

[S45] C++：lambda
来源：http://www.share.tarul.cn/Article/details/gewauinyc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.vehdjk.com/Article/details/gieazmyhk.sHtML

[S46] C++：函数模板
来源：http://3g.bbcook.cn/Article/details/gilfoixfy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/gdxoddcgr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.epnwcf.com/Article/details/goenkgbbb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/giyhtpkln.sHtML

[S48] C++：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gjwhwcfuw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/gcczehckz.sHtML

while (std::getline(in, line)) { }
来源：http://3g.bbcook.cn/Article/details/gvrphfbug.sHtML

[S49] C++：写文件
来源：http://baike.sjlbkw.cn/Article/details/gfexsrbye.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.bbcook.cn/Article/details/gbugppwes.sHtML

[S50] C++：格式化数字
来源：http://baike.epnwcf.com/Article/details/gzfqqdjtt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gletuvtea.sHtML

[S51] C++：显式类型转换
来源：http://blog.yfazqb.com/Article/details/grydprmzv.sHtML

static_cast<double>(a) / b
来源：http://www.share.tarul.cn/Article/details/gbxamrliq.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.epnwcf.com/Article/details/gqcwxzqfn.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.yfazqb.com/Article/details/goitykejs.sHtML

[S53] C++：移动语义
来源：http://baike.sjlbkw.cn/Article/details/gzqfznpts.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.sjlbkw.cn/Article/details/gkltggsfl.sHtML

[S54] C++：异常处理
来源：http://mobile.vehdjk.com/Article/details/gjuolsocw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.tarul.cn/Article/details/guqvmnrwy.sHtML

[S55] C++：结构化绑定
来源：http://baike.yfazqb.com/Article/details/gzlznpvrn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/gtzbcswuv.sHtML

[S56] C++：optional
来源：http://baike.epnwcf.com/Article/details/gahsafgqi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.vehdjk.com/Article/details/geduhftem.sHtML

[S57] C++：编译期常量
来源：http://mobile.fktsv.cn/Article/details/gqedupnsy.sHtML

constexpr int N = 10;
来源：http://www.share.tarul.cn/Article/details/gjlbpgove.sHtML

[S58] C++：命名空间
来源：http://www.blog.bbcook.cn/Article/details/gixmkeyhc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fktsv.cn/Article/details/gdgdeuamm.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/grvwleueb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fktsv.cn/Article/details/gikzqtmyu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.tarul.cn/Article/details/gmfmuyqhc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.epnwcf.com/Article/details/guakddrry.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gaxwblecm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.vehdjk.com/Article/details/gsbribgez.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ggstflisw.sHtML

[T01] Kotlin：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gtiutyhxa.sHtML

println("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gxgcjlnob.sHtML

[T02] Kotlin：变量
来源：http://www.blog.tarul.cn/Article/details/gpfnpmiqt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fktsv.cn/Article/details/gxuyzzoqy.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.tarul.cn/Article/details/gjfxlkmkm.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/gortxbyir.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.yfazqb.com/Article/details/gneicdqdx.sHtML

val n: String? = null;  n?.length
来源：http://m.share.yfazqb.com/Article/details/gryrrnkjq.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.epnwcf.com/Article/details/gghmdqfpl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.sjlbkw.cn/Article/details/glraaonem.sHtML

[T06] Kotlin：集合映射
来源：http://wap.vehdjk.com/Article/details/gqidsbybl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/giswlntbo.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.bbcook.cn/Article/details/grhmfhspy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.yfazqb.com/Article/details/gmrqkmusd.sHtML

[T08] Kotlin：数据类
来源：http://wap.epnwcf.com/Article/details/gjkqdgxuu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/ggvqllhbg.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.sjlbkw.cn/Article/details/gzageezlf.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.yfazqb.com/Article/details/gboobunac.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.bbcook.cn/Article/details/gvcdhcrii.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.vehdjk.com/Article/details/ghtawbiuu.sHtML

[T11] Kotlin：协程
来源：http://3g.bbcook.cn/Article/details/ggspohnnl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.sjlbkw.cn/Article/details/gnllhdcpt.sHtML

[T12] Kotlin：解构声明
来源：http://baike.tarul.cn/Article/details/gbymcbepq.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gdvrdonyi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fktsv.cn/Article/details/glirazxrw.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fktsv.cn/Article/details/gjhngryxf.sHtML

[T14] Kotlin：循环
来源：http://wap.yfazqb.com/Article/details/gymzbobxb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.epnwcf.com/Article/details/gthoydwcl.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.sjlbkw.cn/Article/details/grfsvsuij.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.yfazqb.com/Article/details/gjtjflerf.sHtML

[T16] Swift：Hello World
来源：http://wap.vehdjk.com/Article/details/ggrcpxvqz.sHtML

print("Hello")
来源：http://wap.yfazqb.com/Article/details/gyoyixnsj.sHtML

[T17] Swift：变量与常量
来源：http://blog.vehdjk.com/Article/details/ghoyabunb.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gbrqlufby.sHtML

[T18] Swift：字符串插值
来源：http://blog.fktsv.cn/Article/details/gglbknibl.sHtML

"值: \(b)"
来源：http://blog.bbcook.cn/Article/details/gvdliigzj.sHtML

[T19] Swift：可选绑定
来源：http://wap.bbcook.cn/Article/details/gfjdozhzk.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdtuhzvm.sHtML

[T20] Swift：数组操作
来源：http://wap.tarul.cn/Article/details/gjcyjxeqz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.sjlbkw.cn/Article/details/gfrcumodg.sHtML

[T21] Swift：遍历
来源：http://www.blog.fktsv.cn/Article/details/gjhwpgxrd.sHtML

for x in a { print(x) }
来源：http://www.m.share.yfazqb.com/Article/details/gqttfmmco.sHtML

[T22] Swift：字典
来源：http://wap.tarul.cn/Article/details/grttaxsyt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.sjlbkw.cn/Article/details/gxytcoosw.sHtML

[T23] Swift：函数
来源：http://baike.epnwcf.com/Article/details/govzpxzjf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.tarul.cn/Article/details/gmdenrvcf.sHtML

[T24] Swift：闭包
来源：http://mobile.vehdjk.com/Article/details/gzqnqwjcg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gsizeevqy.sHtML

[T25] Swift：结构体
来源：http://read.share.bbcook.cn/Article/details/gyjxvypft.sHtML

struct P { var x: Int }
来源：http://m.share.fktsv.cn/Article/details/gyroyssfp.sHtML

[T26] Swift：类与重写
来源：http://baike.vehdjk.com/Article/details/gbgmuvbej.sHtML

class A: Base { override func f() {} }
来源：http://baike.tarul.cn/Article/details/gyepvpkwv.sHtML

[T27] Swift：错误处理
来源：http://3g.fktsv.cn/Article/details/gqyzkpkpb.sHtML

do { try f() } catch { print(error) }
来源：http://blog.bbcook.cn/Article/details/gtfqawwqc.sHtML

[T28] Swift：枚举
来源：http://blog.bbcook.cn/Article/details/gdgriaupm.sHtML

enum Color { case red, green }
来源：http://3g.tarul.cn/Article/details/gptwbpeso.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.yfazqb.com/Article/details/galdukxxc.sHtML

guard let x = opt else { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcmtcfwg.sHtML

[T30] Swift：协议
来源：http://read.share.fktsv.cn/Article/details/gnakrmaek.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.epnwcf.com/Article/details/gdrpfbfkt.sHtML


<!-- 参考信息 -->