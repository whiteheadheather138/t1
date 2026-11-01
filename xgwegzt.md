代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.yfazqb.com/Article/details/gastihyth.sHtML

[R34] 退出时清理
来源：http://www.blog.tarul.cn/Article/details/gznuplfwj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gblhqcvzi.sHtML

[R35] 后台执行并等待
来源：http://mobile.yfazqb.com/Article/details/gionjuden.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.vehdjk.com/Article/details/guubpfrhb.sHtML

[R36] 并发执行多个任务
来源：http://blog.bbcook.cn/Article/details/gymwmqljc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fktsv.cn/Article/details/ggnvzkuqy.sHtML

[R37] 把输出赋给变量
来源：http://m.share.yfazqb.com/Article/details/ghdyfdtpw.sHtML

files=$(ls -1)
来源：http://m.share.yfazqb.com/Article/details/gpeblqnec.sHtML

[R38] 管道串联
来源：http://www.share.yfazqb.com/Article/details/gsdurjson.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.tarul.cn/Article/details/gjbkdvuok.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/gzrlkzvgs.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/gqesbhwnh.sHtML

[R40] 追加写日志
来源：http://www.m.share.fktsv.cn/Article/details/grrfbrtzf.sHtML

echo "log" >> out.log
来源：http://3g.fktsv.cn/Article/details/gybasvare.sHtML

[R41] 丢弃输出
来源：http://baike.tarul.cn/Article/details/gthiddnah.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/gkzrakliw.sHtML

[R42] 输入重定向
来源：http://3g.tarul.cn/Article/details/gucfmflwh.sHtML

wc -l < a.txt
来源：http://baike.epnwcf.com/Article/details/grlmrjymu.sHtML

[R43] 按名字查找文件
来源：http://www.share.fktsv.cn/Article/details/gjohmqcly.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.yfazqb.com/Article/details/gqauyicza.sHtML

[R44] 按修改时间查找
来源：http://3g.tarul.cn/Article/details/gvuetymdb.sHtML

find . -mtime -7 -type f
来源：http://m.share.tarul.cn/Article/details/gtonxiugv.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/gdaqmkewx.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.yfazqb.com/Article/details/gbfjzfjmc.sHtML

[R46] 递归替换文件内容
来源：http://3g.bbcook.cn/Article/details/gjqsoyhof.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fktsv.cn/Article/details/gckodrjwr.sHtML

[R47] sed 单行替换
来源：http://blog.fktsv.cn/Article/details/gfalwqwxa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gsxjwtlap.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fktsv.cn/Article/details/guiglkecy.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.tarul.cn/Article/details/gptormxqy.sHtML

[R49] awk 带条件
来源：http://baike.vehdjk.com/Article/details/grrilunjs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fktsv.cn/Article/details/gmebcjlmf.sHtML

[R50] awk 求和
来源：http://www.share.fktsv.cn/Article/details/gggchjfvi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/ggbdnubpz.sHtML

[R51] 排序去重取前几
来源：http://blog.fktsv.cn/Article/details/grkmjokwl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fktsv.cn/Article/details/gtxqmfwsc.sHtML

[R52] 统计行数
来源：http://mobile.yfazqb.com/Article/details/gvddbtlfe.sHtML

wc -l a.txt
来源：http://mobile.epnwcf.com/Article/details/glwstkqoq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.tarul.cn/Article/details/gtprctnmk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.vehdjk.com/Article/details/gtaqfjugm.sHtML

[R54] 比较两个文件
来源：http://www.share.fktsv.cn/Article/details/gfaiipblm.sHtML

diff a.txt b.txt
来源：http://blog.tarul.cn/Article/details/gdktyicrk.sHtML

[R55] 压缩与解压
来源：http://www.m.share.vehdjk.com/Article/details/gyiyrqwpq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.tarul.cn/Article/details/gcgqqsxev.sHtML

[R56] 远程拷贝
来源：http://www.share.fktsv.cn/Article/details/gzbgrkvyi.sHtML

scp file user@host:/path/
来源：http://www.m.share.vehdjk.com/Article/details/glkfnxwco.sHtML

[R57] 远程执行命令
来源：http://www.blog.bbcook.cn/Article/details/gqaxutavb.sHtML

ssh user@host 'uptime'
来源：http://3g.tarul.cn/Article/details/gfkpalide.sHtML

[R58] 下载文件
来源：http://blog.sjlbkw.cn/Article/details/gvlwtbeji.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.bbcook.cn/Article/details/gspemilip.sHtML

[R59] 发 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gtxpcqwuy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.sjlbkw.cn/Article/details/gxjjnjghh.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gnuqnbzsb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.vehdjk.com/Article/details/gtkomzcji.sHtML

[R61] 磁盘占用
来源：http://www.m.share.epnwcf.com/Article/details/grlobmpnp.sHtML

df -h;  du -sh *
来源：http://www.m.share.epnwcf.com/Article/details/gfrdcvamg.sHtML

[R62] 找最占空间的文件
来源：http://wap.sjlbkw.cn/Article/details/gohewjrcc.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.tarul.cn/Article/details/gipzbrhgi.sHtML

[R63] 内存与进程
来源：http://3g.epnwcf.com/Article/details/gqhumhhzm.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.vehdjk.com/Article/details/gurompxcr.sHtML

[R64] 结束进程
来源：http://www.blog.epnwcf.com/Article/details/ghrwghtee.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/gmrmxgsvl.sHtML

[R65] 查看端口占用
来源：http://m.share.bbcook.cn/Article/details/gkzqpakyo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.epnwcf.com/Article/details/gogntgsel.sHtML

[R66] 定时任务
来源：http://baike.bbcook.cn/Article/details/gpcapctgj.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/gwovdbwnz.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.sjlbkw.cn/Article/details/gwclzqpef.sHtML

openssl rand -hex 16
来源：http://3g.sjlbkw.cn/Article/details/gbyhwapgf.sHtML

[R68] 计算文件校验值
来源：http://m.share.sjlbkw.cn/Article/details/gtmvnlzob.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.bbcook.cn/Article/details/goviwtygb.sHtML

[R69] 生成随机密码
来源：http://wap.epnwcf.com/Article/details/gchsxbcna.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.bbcook.cn/Article/details/ghnznsbdv.sHtML

[R70] 时间戳与互转
来源：http://read.share.vehdjk.com/Article/details/gqqobmzor.sHtML

date +%s;  date -d @1700000000
来源：http://3g.tarul.cn/Article/details/gmncohnjj.sHtML

[R71] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gbyqiixeb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.sjlbkw.cn/Article/details/gyjrrhjiv.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fktsv.cn/Article/details/gbuzehuxy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gelmvtkkx.sHtML

[R73] 分割大日志
来源：http://baike.fktsv.cn/Article/details/gwmgejwxk.sHtML

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/gpgtdrdht.sHtML

[R74] 批量重命名
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbsmiemk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.epnwcf.com/Article/details/gvckjrftu.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/gfzlgpcve.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.bbcook.cn/Article/details/gemcqkjkf.sHtML

[R76] 使用临时文件
来源：http://read.share.sjlbkw.cn/Article/details/glulkrqil.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gnrnmndte.sHtML

[R77] 读取用户输入
来源：http://blog.sjlbkw.cn/Article/details/gppwpfnks.sHtML

read -rp "请输入: " ans
来源：http://read.share.tarul.cn/Article/details/gbdkntigq.sHtML

[R78] 交互式菜单
来源：http://wap.vehdjk.com/Article/details/gojiqckmg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/gkorgoqpl.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.tarul.cn/Article/details/gwuqytczj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.vehdjk.com/Article/details/gusfqnklg.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.sjlbkw.cn/Article/details/gniqvrmkw.sHtML

time ./run.sh
来源：http://www.share.epnwcf.com/Article/details/giypkfbml.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/grcqcsrwm.sHtML

S. C / C++ 专题
来源：http://3g.sjlbkw.cn/Article/details/gxdigqinu.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gbiojeplp.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/gxduiayey.sHtML

#include <stdio.h>
来源：http://baike.sjlbkw.cn/Article/details/gmwnqbqif.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.sjlbkw.cn/Article/details/gpdsoaraj.sHtML

[S02] C：变量与格式化输出
来源：http://baike.tarul.cn/Article/details/gshorfbsb.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.vehdjk.com/Article/details/gleirdwdk.sHtML

[S03] C：读入整数
来源：http://www.m.share.vehdjk.com/Article/details/gjelfwfxe.sHtML

int x; scanf("%d", &x);
来源：http://mobile.vehdjk.com/Article/details/gxvyuagjv.sHtML

[S04] C：字符串复制
来源：http://www.m.share.tarul.cn/Article/details/gragdznzt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.yfazqb.com/Article/details/glsmfchjw.sHtML

[S05] C：字符串长度
来源：http://baike.yfazqb.com/Article/details/gefislcwx.sHtML

strlen(s)
来源：http://3g.bbcook.cn/Article/details/gxwimgghz.sHtML

[S06] C：字符串比较
来源：http://wap.fktsv.cn/Article/details/gyisudtfw.sHtML

strcmp(a, b) == 0
来源：http://m.share.fktsv.cn/Article/details/gmadvjvpi.sHtML

[S07] C：数组遍历求和
来源：http://blog.vehdjk.com/Article/details/gyfkdteap.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.yfazqb.com/Article/details/gateiyegq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fktsv.cn/Article/details/gmjrjfsuh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fktsv.cn/Article/details/gtqounnph.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.vehdjk.com/Article/details/gjdtswfxh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.sjlbkw.cn/Article/details/ghegafzny.sHtML

[S10] C：指针与解引用
来源：http://3g.epnwcf.com/Article/details/gnvxaoado.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fktsv.cn/Article/details/gckuanlhr.sHtML

[S11] C：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gsbqznzbw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.tarul.cn/Article/details/gxpuiwpgp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.yfazqb.com/Article/details/guwqcqeqm.sHtML

fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/gwtwuaucy.sHtML

[S12] C：写文件
来源：http://m.share.tarul.cn/Article/details/gyxzowoeh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.epnwcf.com/Article/details/gsklikdnj.sHtML

[S13] C：宏定义
来源：http://wap.epnwcf.com/Article/details/grrhixpep.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.bbcook.cn/Article/details/gudstwdoy.sHtML

[S14] C：枚举
来源：http://www.m.share.fktsv.cn/Article/details/gdglymxxs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.epnwcf.com/Article/details/gpzttcjyz.sHtML

[S15] C：类型转换
来源：http://3g.tarul.cn/Article/details/gsgsiyxpi.sHtML

(double) a / b
来源：http://3g.epnwcf.com/Article/details/gwrbmlhnz.sHtML

[S16] C：位操作置位
来源：http://wap.vehdjk.com/Article/details/giipcdgjh.sHtML

x |= (1 << 3);
来源：http://www.blog.epnwcf.com/Article/details/gndvalznt.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.yfazqb.com/Article/details/ggbqjgqen.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.vehdjk.com/Article/details/gjsvqqckd.sHtML

[S18] C：命令行参数
来源：http://wap.sjlbkw.cn/Article/details/gvhbcncgq.sHtML

int main(int argc, char **argv)
来源：http://read.share.fktsv.cn/Article/details/gdootygxv.sHtML

[S19] C：快速排序
来源：http://mobile.yfazqb.com/Article/details/goptyrhdo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gmbvjotmg.sHtML

[S20] C：二分查找
来源：http://read.share.sjlbkw.cn/Article/details/gxrjjsvze.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gbpclfqkt.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gwndbgghj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fktsv.cn/Article/details/gnkrllcmw.sHtML

[S22] C：字符串转数字
来源：http://www.share.bbcook.cn/Article/details/gsyfzolho.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.vehdjk.com/Article/details/gmnunyyws.sHtML

[S23] C：随机数
来源：http://www.blog.bbcook.cn/Article/details/gqiwjgqii.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.bbcook.cn/Article/details/gctuvirzl.sHtML

[S24] C：获取本地时间
来源：http://www.share.sjlbkw.cn/Article/details/ghjgfrhtf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.vehdjk.com/Article/details/gxstwnikx.sHtML

[S25] C：内存拷贝
来源：http://m.share.tarul.cn/Article/details/gixoagwta.sHtML

memcpy(dst, src, n);
来源：http://read.share.yfazqb.com/Article/details/gpespwqzb.sHtML

[S26] C：内存清零
来源：http://baike.sjlbkw.cn/Article/details/gsumxlvop.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fktsv.cn/Article/details/gdedlgjdl.sHtML

[S27] C：定义常量
来源：http://read.share.vehdjk.com/Article/details/gprvyerfz.sHtML

const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gbhruyocl.sHtML

[S28] C：静态变量
来源：http://3g.epnwcf.com/Article/details/ghmpcieud.sHtML

static int counter = 0;
来源：http://read.share.sjlbkw.cn/Article/details/gvneyjtid.sHtML

[S29] C：变参函数
来源：http://www.blog.yfazqb.com/Article/details/gxffeozdh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.epnwcf.com/Article/details/gzrekrzvc.sHtML

[S30] C：头文件保护
来源：http://3g.epnwcf.com/Article/details/gaqfzonvi.sHtML

#ifndef X_H
来源：http://m.share.bbcook.cn/Article/details/gbeodnlej.sHtML

#define X_H
来源：http://blog.fktsv.cn/Article/details/gvvusltat.sHtML

#endif
来源：http://baike.sjlbkw.cn/Article/details/gjbhxslxg.sHtML

[S31] C++：Hello World
来源：http://mobile.bbcook.cn/Article/details/ggdxcvspw.sHtML

#include <iostream>
来源：http://mobile.bbcook.cn/Article/details/gkesddmym.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.bbcook.cn/Article/details/gtgcdxphw.sHtML

[S32] C++：字符串
来源：http://www.share.vehdjk.com/Article/details/gavwjxikx.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fktsv.cn/Article/details/gjxaretxk.sHtML

[S33] C++：vector 增删
来源：http://mobile.sjlbkw.cn/Article/details/ghtykwwdl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.vehdjk.com/Article/details/gifphgnne.sHtML

[S34] C++：遍历 vector
来源：http://baike.tarul.cn/Article/details/gkidrgufq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.tarul.cn/Article/details/gewrwrqwi.sHtML

[S35] C++：map
来源：http://3g.tarul.cn/Article/details/gbgxunnle.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/ghpquzepm.sHtML

[S36] C++：unordered_map
来源：http://mobile.sjlbkw.cn/Article/details/gwioqciym.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gfqaskhie.sHtML

[S37] C++：set
来源：http://wap.sjlbkw.cn/Article/details/gskfcztiu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.vehdjk.com/Article/details/gpltmwhor.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gvpqvqgkz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.sjlbkw.cn/Article/details/gvtucwgae.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.sjlbkw.cn/Article/details/grlnnvlth.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/gkjrnysir.sHtML

[S40] C++：查找元素
来源：http://m.share.yfazqb.com/Article/details/gfpvaaoyo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.epnwcf.com/Article/details/gktehwvso.sHtML

[S41] C++：类与构造函数
来源：http://blog.fktsv.cn/Article/details/gwnwpazqz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.yfazqb.com/Article/details/gzukemduh.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fktsv.cn/Article/details/gvtrjricu.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.vehdjk.com/Article/details/grvwdcowe.sHtML

[S43] C++：智能指针
来源：http://www.m.share.epnwcf.com/Article/details/gumenlioj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.epnwcf.com/Article/details/gxhjestmm.sHtML

[S44] C++：引用传参
来源：http://blog.bbcook.cn/Article/details/gfkeebzoc.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.vehdjk.com/Article/details/gubgmsjuj.sHtML

[S45] C++：lambda
来源：http://blog.bbcook.cn/Article/details/gdmfchavf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.tarul.cn/Article/details/gwwbflzsi.sHtML

[S46] C++：函数模板
来源：http://blog.epnwcf.com/Article/details/ghcooqxcu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.epnwcf.com/Article/details/gxdbnezbu.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.sjlbkw.cn/Article/details/glruscxom.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.vehdjk.com/Article/details/ggqkrvdbw.sHtML

[S48] C++：逐行读文件
来源：http://www.share.tarul.cn/Article/details/glpsitgmi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.yfazqb.com/Article/details/gvnhsiycg.sHtML

while (std::getline(in, line)) { }
来源：http://blog.bbcook.cn/Article/details/gajazlxhd.sHtML

[S49] C++：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gvxsigroy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfdqinms.sHtML

[S50] C++：格式化数字
来源：http://mobile.epnwcf.com/Article/details/gxvzhebmd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.tarul.cn/Article/details/gqwvrobfm.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/gdnczvneo.sHtML

static_cast<double>(a) / b
来源：http://3g.yfazqb.com/Article/details/gujmpgkas.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.yfazqb.com/Article/details/gqqxmdcww.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.bbcook.cn/Article/details/ghcgvgufg.sHtML

[S53] C++：移动语义
来源：http://3g.epnwcf.com/Article/details/gjwngrcab.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.tarul.cn/Article/details/gjfgxhstl.sHtML

[S54] C++：异常处理
来源：http://m.share.epnwcf.com/Article/details/guflzxgjp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/giptrmajl.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.yfazqb.com/Article/details/gupsijyjw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.epnwcf.com/Article/details/gtddspbgg.sHtML

[S56] C++：optional
来源：http://mobile.fktsv.cn/Article/details/gyawxgthi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.bbcook.cn/Article/details/gqheemqoy.sHtML

[S57] C++：编译期常量
来源：http://www.share.bbcook.cn/Article/details/gyernizgz.sHtML

constexpr int N = 10;
来源：http://www.blog.vehdjk.com/Article/details/gliuiwxii.sHtML

[S58] C++：命名空间
来源：http://baike.yfazqb.com/Article/details/gymlgmuep.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.tarul.cn/Article/details/gnnmacqfa.sHtML

[S59] C++：静态断言
来源：http://wap.epnwcf.com/Article/details/gpzjjehqu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fktsv.cn/Article/details/gdyadoqjx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.tarul.cn/Article/details/gdhdcpafa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/gopmjnviv.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdmjaspxk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/guwfmzuvx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjyqzamvx.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fktsv.cn/Article/details/gxqajjfqk.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/gefvicerp.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gsxvemktu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.yfazqb.com/Article/details/goyqebglp.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.epnwcf.com/Article/details/gglepbwgd.sHtML

"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/gzmugqtln.sHtML

[T04] Kotlin：空安全
来源：http://3g.tarul.cn/Article/details/gxvtlzxmu.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.tarul.cn/Article/details/gowbuwrjq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/gpvmidhgb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.epnwcf.com/Article/details/gvppnqalg.sHtML

[T06] Kotlin：集合映射
来源：http://blog.yfazqb.com/Article/details/gzsddxyip.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.vehdjk.com/Article/details/gsnipdbhh.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/gruqcznyv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.bbcook.cn/Article/details/gnsnglakc.sHtML

[T08] Kotlin：数据类
来源：http://mobile.epnwcf.com/Article/details/gmwnzyvjx.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.yfazqb.com/Article/details/gebnkrnjz.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.epnwcf.com/Article/details/ggpqhrppa.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fktsv.cn/Article/details/giqjxvcfp.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.tarul.cn/Article/details/guaiymzii.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.tarul.cn/Article/details/gfgtptrgu.sHtML

[T11] Kotlin：协程
来源：http://3g.epnwcf.com/Article/details/gubajggra.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.sjlbkw.cn/Article/details/gysnkglmi.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fktsv.cn/Article/details/gqbtanoav.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.epnwcf.com/Article/details/goomszclj.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.tarul.cn/Article/details/ghwulaicr.sHtML

val m = mapOf("a" to 1)
来源：http://baike.bbcook.cn/Article/details/gjgjoadcu.sHtML

[T14] Kotlin：循环
来源：http://mobile.yfazqb.com/Article/details/gubdukhtc.sHtML

for (i in 1..10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/ghgytaaud.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/gywxnilia.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.tarul.cn/Article/details/gfvytrevt.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/gzjubpyad.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/gsskejlyg.sHtML

[T17] Swift：变量与常量
来源：http://baike.sjlbkw.cn/Article/details/gdjbceptb.sHtML

var a = 1;  let b = 2
来源：http://mobile.yfazqb.com/Article/details/gccebmzjn.sHtML

[T18] Swift：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gryhoisdz.sHtML

"值: \(b)"
来源：http://m.share.bbcook.cn/Article/details/gucnlyhqm.sHtML

[T19] Swift：可选绑定
来源：http://www.share.vehdjk.com/Article/details/gkvxikdno.sHtML

if let n = opt { print(n) }
来源：http://mobile.yfazqb.com/Article/details/gtdtvfjrk.sHtML

[T20] Swift：数组操作
来源：http://mobile.sjlbkw.cn/Article/details/gggdlxprk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.yfazqb.com/Article/details/gynjalzhi.sHtML

[T21] Swift：遍历
来源：http://blog.sjlbkw.cn/Article/details/gkfbxgtot.sHtML

for x in a { print(x) }
来源：http://baike.fktsv.cn/Article/details/goskhzglx.sHtML

[T22] Swift：字典
来源：http://wap.fktsv.cn/Article/details/gpvugrutq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.yfazqb.com/Article/details/gfurczfzf.sHtML

[T23] Swift：函数
来源：http://www.share.fktsv.cn/Article/details/garhubbvr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.epnwcf.com/Article/details/gtkqxsinx.sHtML

[T24] Swift：闭包
来源：http://read.share.yfazqb.com/Article/details/goeotjzyn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.bbcook.cn/Article/details/gaqygfwcm.sHtML

[T25] Swift：结构体
来源：http://www.blog.bbcook.cn/Article/details/gvhyikjlh.sHtML

struct P { var x: Int }
来源：http://www.blog.fktsv.cn/Article/details/gsvlgvkfd.sHtML

[T26] Swift：类与重写
来源：http://baike.bbcook.cn/Article/details/gwvfmcexp.sHtML

class A: Base { override func f() {} }
来源：http://read.share.sjlbkw.cn/Article/details/gfhnfsrkn.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.yfazqb.com/Article/details/gkupyisxs.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.epnwcf.com/Article/details/gmngbrktr.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fktsv.cn/Article/details/gjzlqxjpj.sHtML

enum Color { case red, green }
来源：http://baike.fktsv.cn/Article/details/gvsxwqrao.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.epnwcf.com/Article/details/gjqrzetjl.sHtML

guard let x = opt else { return }
来源：http://mobile.vehdjk.com/Article/details/gymjuxtyj.sHtML

[T30] Swift：协议
来源：http://www.m.share.sjlbkw.cn/Article/details/gykdnxeui.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.epnwcf.com/Article/details/gncddszxu.sHtML

[T31] Lua：Hello World
来源：http://3g.vehdjk.com/Article/details/gcsuwdnmg.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/gvxdaiqjc.sHtML

[T32] Lua：局部变量
来源：http://wap.yfazqb.com/Article/details/gusoyeqfv.sHtML

local a = 1
来源：http://www.blog.vehdjk.com/Article/details/gxxeusfen.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.vehdjk.com/Article/details/gqkrahwfi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.vehdjk.com/Article/details/gtiwfeitj.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.yfazqb.com/Article/details/gvrtiizjg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.vehdjk.com/Article/details/gmandkzuh.sHtML

[T35] Lua：字典表
来源：http://3g.tarul.cn/Article/details/gjwcsjpeh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.epnwcf.com/Article/details/gxxoyczae.sHtML

[T36] Lua：函数
来源：http://wap.sjlbkw.cn/Article/details/gvbbzjhop.sHtML

function add(a, b) return a + b end
来源：http://baike.fktsv.cn/Article/details/gtqtcutgf.sHtML


<!-- 参考信息 -->