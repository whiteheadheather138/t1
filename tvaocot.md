代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.tarul.cn/Article/details/gviuqudwx.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/gndjhsdke.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gxowwwucm.sHtML

[R35] 后台执行并等待
来源：http://m.share.epnwcf.com/Article/details/gtgdxctaf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.epnwcf.com/Article/details/gtulyewxu.sHtML

[R36] 并发执行多个任务
来源：http://blog.vehdjk.com/Article/details/gzqaeuffj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.epnwcf.com/Article/details/gxlebfmav.sHtML

[R37] 把输出赋给变量
来源：http://wap.tarul.cn/Article/details/gvjicqujh.sHtML

files=$(ls -1)
来源：http://www.share.vehdjk.com/Article/details/gxgnthmym.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/gturclszu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fktsv.cn/Article/details/gunigzbup.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.epnwcf.com/Article/details/gywvrfebn.sHtML

cmd > out.log 2>&1
来源：http://baike.epnwcf.com/Article/details/gzoowswzi.sHtML

[R40] 追加写日志
来源：http://mobile.yfazqb.com/Article/details/gkahklfvp.sHtML

echo "log" >> out.log
来源：http://mobile.fktsv.cn/Article/details/gwnngzlsp.sHtML

[R41] 丢弃输出
来源：http://www.m.share.tarul.cn/Article/details/gthfifohq.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fktsv.cn/Article/details/gvokjlpci.sHtML

[R42] 输入重定向
来源：http://mobile.fktsv.cn/Article/details/gzufhijme.sHtML

wc -l < a.txt
来源：http://3g.sjlbkw.cn/Article/details/gtvgovcgx.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.vehdjk.com/Article/details/gjpmkbmtf.sHtML

find . -name "*.log" -type f
来源：http://www.share.bbcook.cn/Article/details/ghfnahdin.sHtML

[R44] 按修改时间查找
来源：http://3g.yfazqb.com/Article/details/gkpkvncay.sHtML

find . -mtime -7 -type f
来源：http://www.share.bbcook.cn/Article/details/gzzftjmee.sHtML

[R45] 批量删除
来源：http://wap.fktsv.cn/Article/details/gqlieqfvv.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.sjlbkw.cn/Article/details/gcrufrndv.sHtML

[R46] 递归替换文件内容
来源：http://blog.yfazqb.com/Article/details/gosxplkes.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.sjlbkw.cn/Article/details/gisasbmuf.sHtML

[R47] sed 单行替换
来源：http://www.blog.epnwcf.com/Article/details/gknfhsxnt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gtgypxbsn.sHtML

[R48] awk 取指定列
来源：http://mobile.bbcook.cn/Article/details/ghprfgutu.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gidmieoka.sHtML

[R49] awk 带条件
来源：http://www.m.share.vehdjk.com/Article/details/grpyvnzrc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.bbcook.cn/Article/details/goczstuxi.sHtML

[R50] awk 求和
来源：http://wap.tarul.cn/Article/details/goeilutva.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.bbcook.cn/Article/details/gcgwuxgkj.sHtML

[R51] 排序去重取前几
来源：http://read.share.epnwcf.com/Article/details/gtwikthky.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.sjlbkw.cn/Article/details/gxsovsxjp.sHtML

[R52] 统计行数
来源：http://baike.tarul.cn/Article/details/gukhpekjz.sHtML

wc -l a.txt
来源：http://3g.tarul.cn/Article/details/gwlifrlvm.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.tarul.cn/Article/details/gyuviasju.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gacclkpgk.sHtML

[R54] 比较两个文件
来源：http://baike.yfazqb.com/Article/details/gvnrufcpl.sHtML

diff a.txt b.txt
来源：http://3g.yfazqb.com/Article/details/gmhhbkzpw.sHtML

[R55] 压缩与解压
来源：http://read.share.yfazqb.com/Article/details/gjawhshne.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fktsv.cn/Article/details/ghhxjcvbq.sHtML

[R56] 远程拷贝
来源：http://m.share.epnwcf.com/Article/details/glizhzgzj.sHtML

scp file user@host:/path/
来源：http://3g.fktsv.cn/Article/details/gruppicdo.sHtML

[R57] 远程执行命令
来源：http://www.blog.sjlbkw.cn/Article/details/gawnobxws.sHtML

ssh user@host 'uptime'
来源：http://www.share.sjlbkw.cn/Article/details/gdpkwukdj.sHtML

[R58] 下载文件
来源：http://www.m.share.bbcook.cn/Article/details/ganwujazh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fktsv.cn/Article/details/gcxzehhwm.sHtML

[R59] 发 POST JSON
来源：http://blog.vehdjk.com/Article/details/gqyfhyusl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.bbcook.cn/Article/details/gzmlniwiu.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/grsjzhxsw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.vehdjk.com/Article/details/gqevqqcbs.sHtML

[R61] 磁盘占用
来源：http://m.share.epnwcf.com/Article/details/gxkdzvhzu.sHtML

df -h;  du -sh *
来源：http://m.share.fktsv.cn/Article/details/gchoeakzy.sHtML

[R62] 找最占空间的文件
来源：http://baike.sjlbkw.cn/Article/details/gdfsmegih.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.sjlbkw.cn/Article/details/gqdcmlfdc.sHtML

[R63] 内存与进程
来源：http://mobile.vehdjk.com/Article/details/gfqdpqbrw.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.sjlbkw.cn/Article/details/glpzofqko.sHtML

[R64] 结束进程
来源：http://www.share.bbcook.cn/Article/details/gopdukdaz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.tarul.cn/Article/details/gqgpanaoh.sHtML

[R65] 查看端口占用
来源：http://baike.yfazqb.com/Article/details/gkgpurlbb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.epnwcf.com/Article/details/gbxqizrqi.sHtML

[R66] 定时任务
来源：http://www.blog.yfazqb.com/Article/details/gfeuonijq.sHtML

crontab -e;  crontab -l
来源：http://wap.bbcook.cn/Article/details/grpechfef.sHtML

[R67] 生成随机十六进制串
来源：http://baike.yfazqb.com/Article/details/gbgepkqfq.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/gnnrsbnrq.sHtML

[R68] 计算文件校验值
来源：http://www.blog.tarul.cn/Article/details/ggxpqorro.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gknttoxdb.sHtML

[R69] 生成随机密码
来源：http://mobile.bbcook.cn/Article/details/gqbolvcaa.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fktsv.cn/Article/details/gfnirfqra.sHtML

[R70] 时间戳与互转
来源：http://3g.bbcook.cn/Article/details/gnuqvodnu.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fktsv.cn/Article/details/gidxqlynq.sHtML

[R71] 日期格式化
来源：http://3g.bbcook.cn/Article/details/gspjvdhrt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.sjlbkw.cn/Article/details/gwftvazdb.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.vehdjk.com/Article/details/gobcniycm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fktsv.cn/Article/details/gdzoocnot.sHtML

[R73] 分割大日志
来源：http://www.blog.bbcook.cn/Article/details/gdwrvmhkn.sHtML

split -l 1000 big.log part_
来源：http://www.share.fktsv.cn/Article/details/gmwtznukg.sHtML

[R74] 批量重命名
来源：http://mobile.fktsv.cn/Article/details/guvqlrqgx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.sjlbkw.cn/Article/details/gfrajccmi.sHtML

[R75] 导出环境变量
来源：http://m.share.fktsv.cn/Article/details/gglzxkxqv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.tarul.cn/Article/details/gvvriwzsv.sHtML

[R76] 使用临时文件
来源：http://www.share.tarul.cn/Article/details/gsdcuheho.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/glkeboroe.sHtML

[R77] 读取用户输入
来源：http://www.blog.vehdjk.com/Article/details/gznksylhw.sHtML

read -rp "请输入: " ans
来源：http://mobile.vehdjk.com/Article/details/gebtfqyqa.sHtML

[R78] 交互式菜单
来源：http://www.blog.vehdjk.com/Article/details/gacqgrdxv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fktsv.cn/Article/details/gicrvbqxx.sHtML

[R79] 解析命令行选项
来源：http://www.share.bbcook.cn/Article/details/gouogtsrx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.vehdjk.com/Article/details/gddknvjqz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.bbcook.cn/Article/details/guzociojr.sHtML

time ./run.sh
来源：http://www.blog.vehdjk.com/Article/details/gnjkfmguc.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gxcecovew.sHtML

S. C / C++ 专题
来源：http://baike.fktsv.cn/Article/details/gedzljsvg.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gitrutxll.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gbqipqnpt.sHtML

#include <stdio.h>
来源：http://blog.sjlbkw.cn/Article/details/ggefekcrf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.vehdjk.com/Article/details/gcfulxgrj.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.tarul.cn/Article/details/gucfxpwng.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.epnwcf.com/Article/details/gmhdnmiat.sHtML

[S03] C：读入整数
来源：http://read.share.fktsv.cn/Article/details/gyrlwxnpl.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gntxxxgtj.sHtML

[S04] C：字符串复制
来源：http://mobile.epnwcf.com/Article/details/geipoevgu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fktsv.cn/Article/details/gvlcpjwrq.sHtML

[S05] C：字符串长度
来源：http://wap.yfazqb.com/Article/details/ghhfhrzyj.sHtML

strlen(s)
来源：http://read.share.epnwcf.com/Article/details/gaqhqvevz.sHtML

[S06] C：字符串比较
来源：http://blog.fktsv.cn/Article/details/grwgqehzs.sHtML

strcmp(a, b) == 0
来源：http://mobile.tarul.cn/Article/details/gsnbsnprb.sHtML

[S07] C：数组遍历求和
来源：http://m.share.epnwcf.com/Article/details/gveomkyhz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.bbcook.cn/Article/details/ggeuqdatv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fktsv.cn/Article/details/gjclvldkd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fktsv.cn/Article/details/gitbcjbxj.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.epnwcf.com/Article/details/gtwiwsabl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.epnwcf.com/Article/details/gxjyuilyf.sHtML

[S10] C：指针与解引用
来源：http://m.share.sjlbkw.cn/Article/details/ghmkgcddd.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.vehdjk.com/Article/details/gyhrmbxcd.sHtML

[S11] C：逐行读文件
来源：http://blog.vehdjk.com/Article/details/guecijuds.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.yfazqb.com/Article/details/gvejcihmm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.yfazqb.com/Article/details/gphccnczy.sHtML

fclose(f);
来源：http://3g.vehdjk.com/Article/details/gawkdhewb.sHtML

[S12] C：写文件
来源：http://www.blog.fktsv.cn/Article/details/gjlxrntga.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.tarul.cn/Article/details/gxedoymgd.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gtujundvx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.vehdjk.com/Article/details/gzukalkkz.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/gqicktuip.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fktsv.cn/Article/details/gjbaazjdf.sHtML

[S15] C：类型转换
来源：http://wap.vehdjk.com/Article/details/gsedsiwon.sHtML

(double) a / b
来源：http://m.share.sjlbkw.cn/Article/details/gvpgfribm.sHtML

[S16] C：位操作置位
来源：http://3g.bbcook.cn/Article/details/gdzxxzskb.sHtML

x |= (1 << 3);
来源：http://3g.bbcook.cn/Article/details/gznhmrfpp.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.bbcook.cn/Article/details/grnopdkox.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.vehdjk.com/Article/details/gbtooodjc.sHtML

[S18] C：命令行参数
来源：http://www.blog.fktsv.cn/Article/details/gjoeqveqt.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.vehdjk.com/Article/details/gzskxyuwq.sHtML

[S19] C：快速排序
来源：http://www.share.bbcook.cn/Article/details/gcukydokm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/grbuxtipn.sHtML

[S20] C：二分查找
来源：http://www.blog.fktsv.cn/Article/details/goduihvra.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/gczfbavim.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gltinijhb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.tarul.cn/Article/details/gefsluwcq.sHtML

[S22] C：字符串转数字
来源：http://www.blog.bbcook.cn/Article/details/gbgwipxwa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.bbcook.cn/Article/details/gjmbdvdeh.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gtwxcuzzz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fktsv.cn/Article/details/gaomzinew.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.tarul.cn/Article/details/gzxgptbwm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.bbcook.cn/Article/details/gyxfzbapz.sHtML

[S25] C：内存拷贝
来源：http://blog.sjlbkw.cn/Article/details/gdkrjflup.sHtML

memcpy(dst, src, n);
来源：http://www.share.epnwcf.com/Article/details/gukzrfhyo.sHtML

[S26] C：内存清零
来源：http://read.share.vehdjk.com/Article/details/geuakyrrv.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/gnvratfhx.sHtML

[S27] C：定义常量
来源：http://www.m.share.bbcook.cn/Article/details/gaufogjsg.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gzrlamone.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/gxhymakgk.sHtML

static int counter = 0;
来源：http://wap.sjlbkw.cn/Article/details/gwpboxgbg.sHtML

[S29] C：变参函数
来源：http://3g.fktsv.cn/Article/details/gpjlhdgph.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fktsv.cn/Article/details/gasxgsbie.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/gpasajoit.sHtML

#ifndef X_H
来源：http://wap.sjlbkw.cn/Article/details/gcwgcvxtj.sHtML

#define X_H
来源：http://read.share.bbcook.cn/Article/details/gltqiyyrk.sHtML

#endif
来源：http://baike.epnwcf.com/Article/details/gqnowbpfd.sHtML

[S31] C++：Hello World
来源：http://baike.vehdjk.com/Article/details/gxlurfvoo.sHtML

#include <iostream>
来源：http://read.share.vehdjk.com/Article/details/ghvjilfxi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.tarul.cn/Article/details/gcjadmtuh.sHtML

[S32] C++：字符串
来源：http://3g.vehdjk.com/Article/details/gcsosjrgb.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.epnwcf.com/Article/details/gfjpwcutu.sHtML

[S33] C++：vector 增删
来源：http://wap.yfazqb.com/Article/details/gqpshkqmz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.epnwcf.com/Article/details/gqkwauczw.sHtML

[S34] C++：遍历 vector
来源：http://mobile.bbcook.cn/Article/details/gpseyreqw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.tarul.cn/Article/details/gviromcnk.sHtML

[S35] C++：map
来源：http://www.m.share.epnwcf.com/Article/details/gaoosipll.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/ghvdmqiwv.sHtML

[S36] C++：unordered_map
来源：http://www.blog.yfazqb.com/Article/details/gmeblohoc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gphakufet.sHtML

[S37] C++：set
来源：http://blog.tarul.cn/Article/details/gqswqpjbw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fktsv.cn/Article/details/gpuchcukw.sHtML

[S38] C++：排序
来源：http://3g.fktsv.cn/Article/details/ghtlozxat.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gvkfjqcjn.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.epnwcf.com/Article/details/gacokyrsg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.epnwcf.com/Article/details/gmepahxqp.sHtML

[S40] C++：查找元素
来源：http://m.share.sjlbkw.cn/Article/details/gmerpvyan.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnucdomf.sHtML

[S41] C++：类与构造函数
来源：http://m.share.bbcook.cn/Article/details/glaktastz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.bbcook.cn/Article/details/gseepfeed.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fktsv.cn/Article/details/gvoamkfaz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.tarul.cn/Article/details/grdugrjbm.sHtML

[S43] C++：智能指针
来源：http://read.share.vehdjk.com/Article/details/gdntrovol.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.tarul.cn/Article/details/gaxznxghu.sHtML

[S44] C++：引用传参
来源：http://blog.yfazqb.com/Article/details/guokvoifg.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.yfazqb.com/Article/details/gsbltmtbi.sHtML

[S45] C++：lambda
来源：http://read.share.bbcook.cn/Article/details/ghnnlenyz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/ggybtemet.sHtML

[S46] C++：函数模板
来源：http://www.m.share.bbcook.cn/Article/details/greledjsu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/gxpypxzbw.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.vehdjk.com/Article/details/gtbzxaukp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.epnwcf.com/Article/details/gmitiouzd.sHtML

[S48] C++：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gtmdjlxqp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.epnwcf.com/Article/details/guifcldcx.sHtML

while (std::getline(in, line)) { }
来源：http://blog.vehdjk.com/Article/details/gpwmwkvgs.sHtML

[S49] C++：写文件
来源：http://wap.yfazqb.com/Article/details/gjhtqkjsq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.yfazqb.com/Article/details/gytgvigvh.sHtML

[S50] C++：格式化数字
来源：http://wap.vehdjk.com/Article/details/gpitywuec.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.bbcook.cn/Article/details/giibgxqyp.sHtML

[S51] C++：显式类型转换
来源：http://m.share.tarul.cn/Article/details/gzqrcdgxh.sHtML

static_cast<double>(a) / b
来源：http://read.share.tarul.cn/Article/details/gblnnzywf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.bbcook.cn/Article/details/ghbjhzpkh.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwmnmpbqd.sHtML

[S53] C++：移动语义
来源：http://www.blog.bbcook.cn/Article/details/gxvyrxyma.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.tarul.cn/Article/details/gnrchxgtc.sHtML

[S54] C++：异常处理
来源：http://blog.bbcook.cn/Article/details/gresrneer.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.sjlbkw.cn/Article/details/gjpybcmsz.sHtML

[S55] C++：结构化绑定
来源：http://mobile.epnwcf.com/Article/details/gvndsrhce.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.yfazqb.com/Article/details/gdbvslvjw.sHtML

[S56] C++：optional
来源：http://mobile.sjlbkw.cn/Article/details/glyahgtei.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.bbcook.cn/Article/details/gfxjilkyr.sHtML

[S57] C++：编译期常量
来源：http://wap.yfazqb.com/Article/details/gclmojepv.sHtML

constexpr int N = 10;
来源：http://3g.yfazqb.com/Article/details/gfgmmrtcf.sHtML

[S58] C++：命名空间
来源：http://mobile.vehdjk.com/Article/details/gvnaolpew.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.bbcook.cn/Article/details/gtwsafdxa.sHtML

[S59] C++：静态断言
来源：http://www.blog.epnwcf.com/Article/details/gkkkgkaek.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fktsv.cn/Article/details/gzdsffnna.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gioyhysmt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fktsv.cn/Article/details/gfnulkrhw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gutwngkfv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.bbcook.cn/Article/details/gouvspcbe.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gdytejgjv.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gkdtgqimx.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/glnmusyvv.sHtML

[T02] Kotlin：变量
来源：http://read.share.tarul.cn/Article/details/gruigzvmt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.bbcook.cn/Article/details/gvakotavk.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.epnwcf.com/Article/details/gehkuzcib.sHtML

"值: $b"
来源：http://blog.yfazqb.com/Article/details/gbqxneghq.sHtML

[T04] Kotlin：空安全
来源：http://baike.tarul.cn/Article/details/gwszadejq.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.epnwcf.com/Article/details/gfnaxhmnb.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.yfazqb.com/Article/details/gmnykwpag.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.tarul.cn/Article/details/gxygyuxzf.sHtML

[T06] Kotlin：集合映射
来源：http://blog.tarul.cn/Article/details/gpawrubhg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.vehdjk.com/Article/details/gjyqfvtvo.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/grsptofks.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gbqwnyjqa.sHtML

[T08] Kotlin：数据类
来源：http://m.share.yfazqb.com/Article/details/gpkoppsln.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.sjlbkw.cn/Article/details/gltuszdwr.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.bbcook.cn/Article/details/ghtykxfqo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.vehdjk.com/Article/details/gsauravgo.sHtML

[T10] Kotlin：默认参数
来源：http://blog.yfazqb.com/Article/details/gmsqbrnzs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fktsv.cn/Article/details/gcopdkheo.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/ggqkmwegd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.sjlbkw.cn/Article/details/gdehrogmu.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.yfazqb.com/Article/details/gsarpseos.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gqlfdzcmx.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.sjlbkw.cn/Article/details/gqzoxozag.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.tarul.cn/Article/details/gwzyruiih.sHtML

[T14] Kotlin：循环
来源：http://wap.epnwcf.com/Article/details/glzgyyocu.sHtML

for (i in 1..10) println(i)
来源：http://m.share.bbcook.cn/Article/details/gyiagavul.sHtML

[T15] Kotlin：接口
来源：http://blog.vehdjk.com/Article/details/gwvgrszqv.sHtML

interface Shape { fun area(): Double }
来源：http://wap.bbcook.cn/Article/details/gjxfhkbmj.sHtML

[T16] Swift：Hello World
来源：http://baike.bbcook.cn/Article/details/glvstgqrc.sHtML

print("Hello")
来源：http://read.share.tarul.cn/Article/details/gfhsbhidv.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.epnwcf.com/Article/details/gmlqhjfrx.sHtML

var a = 1;  let b = 2
来源：http://www.blog.vehdjk.com/Article/details/gxmhitnbi.sHtML

[T18] Swift：字符串插值
来源：http://baike.epnwcf.com/Article/details/gfynmruvt.sHtML

"值: \(b)"
来源：http://wap.fktsv.cn/Article/details/gvmuvovhi.sHtML

[T19] Swift：可选绑定
来源：http://www.share.bbcook.cn/Article/details/gqtpzxdav.sHtML

if let n = opt { print(n) }
来源：http://blog.tarul.cn/Article/details/ghjnzympw.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fktsv.cn/Article/details/gyzeoinmf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fktsv.cn/Article/details/ggtkqetzi.sHtML

[T21] Swift：遍历
来源：http://www.share.epnwcf.com/Article/details/gffyyhtdn.sHtML

for x in a { print(x) }
来源：http://wap.tarul.cn/Article/details/gnlyxqnie.sHtML

[T22] Swift：字典
来源：http://wap.tarul.cn/Article/details/gsozfsgtc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.yfazqb.com/Article/details/gcpnmytab.sHtML

[T23] Swift：函数
来源：http://read.share.fktsv.cn/Article/details/gwkwdkcve.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.vehdjk.com/Article/details/gadiopatj.sHtML

[T24] Swift：闭包
来源：http://blog.yfazqb.com/Article/details/gtfumyxwp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.bbcook.cn/Article/details/glwmsyxxs.sHtML

[T25] Swift：结构体
来源：http://3g.vehdjk.com/Article/details/grrfuysfh.sHtML

struct P { var x: Int }
来源：http://baike.vehdjk.com/Article/details/gigidthkq.sHtML

[T26] Swift：类与重写
来源：http://wap.tarul.cn/Article/details/gmvnutmeq.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.vehdjk.com/Article/details/gsykmuhkn.sHtML

[T27] Swift：错误处理
来源：http://m.share.bbcook.cn/Article/details/giaxpitqo.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.yfazqb.com/Article/details/gblouwmmx.sHtML

[T28] Swift：枚举
来源：http://3g.fktsv.cn/Article/details/gpqzayfcx.sHtML

enum Color { case red, green }
来源：http://www.blog.sjlbkw.cn/Article/details/gfnhxahrt.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.vehdjk.com/Article/details/gmzfohdxn.sHtML

guard let x = opt else { return }
来源：http://wap.vehdjk.com/Article/details/grhxlbvdi.sHtML

[T30] Swift：协议
来源：http://3g.vehdjk.com/Article/details/gbicmkrkf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.tarul.cn/Article/details/gnistysgg.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/gctszunsk.sHtML

print("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gnpvvoyso.sHtML

[T32] Lua：局部变量
来源：http://baike.vehdjk.com/Article/details/gamnxjvba.sHtML

local a = 1
来源：http://m.share.yfazqb.com/Article/details/gpbfzavty.sHtML

[T33] Lua：表（数组）
来源：http://wap.bbcook.cn/Article/details/gaiamgnso.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.bbcook.cn/Article/details/gxpkurpke.sHtML

[T34] Lua：遍历表
来源：http://mobile.vehdjk.com/Article/details/gnvosjbag.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fktsv.cn/Article/details/gmgdiachk.sHtML

[T35] Lua：字典表
来源：http://blog.epnwcf.com/Article/details/gptynkjxk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.bbcook.cn/Article/details/gwioalrqt.sHtML

[T36] Lua：函数
来源：http://read.share.tarul.cn/Article/details/gywssftso.sHtML

function add(a, b) return a + b end
来源：http://www.share.vehdjk.com/Article/details/gbqhjqpfm.sHtML


<!-- 参考信息 -->