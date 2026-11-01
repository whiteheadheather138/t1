代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.vehdjk.com/Article/details/ggcxoykxz.sHtML

[R34] 退出时清理
来源：http://www.m.share.tarul.cn/Article/details/glgtjlpuf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gkeohdgjs.sHtML

[R35] 后台执行并等待
来源：http://mobile.vehdjk.com/Article/details/guqgiouqf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.sjlbkw.cn/Article/details/gtelxupal.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/gjlhrxihj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.vehdjk.com/Article/details/gsupfzeki.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.tarul.cn/Article/details/gstzlyqcv.sHtML

files=$(ls -1)
来源：http://wap.yfazqb.com/Article/details/gbgvexhlp.sHtML

[R38] 管道串联
来源：http://blog.bbcook.cn/Article/details/gyyuemjli.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.yfazqb.com/Article/details/gcbfnfidr.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.vehdjk.com/Article/details/gyhznutvg.sHtML

cmd > out.log 2>&1
来源：http://3g.epnwcf.com/Article/details/glkrpwete.sHtML

[R40] 追加写日志
来源：http://read.share.yfazqb.com/Article/details/gxyoippxf.sHtML

echo "log" >> out.log
来源：http://www.blog.yfazqb.com/Article/details/guclqgdvr.sHtML

[R41] 丢弃输出
来源：http://www.share.bbcook.cn/Article/details/gnfkkvshp.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gimaadcew.sHtML

[R42] 输入重定向
来源：http://www.blog.bbcook.cn/Article/details/gavjvsrtv.sHtML

wc -l < a.txt
来源：http://read.share.yfazqb.com/Article/details/glniqzgqy.sHtML

[R43] 按名字查找文件
来源：http://blog.epnwcf.com/Article/details/gxehkdoux.sHtML

find . -name "*.log" -type f
来源：http://m.share.epnwcf.com/Article/details/grubyeuty.sHtML

[R44] 按修改时间查找
来源：http://wap.yfazqb.com/Article/details/gnvlbiouu.sHtML

find . -mtime -7 -type f
来源：http://m.share.tarul.cn/Article/details/gtbnvspbi.sHtML

[R45] 批量删除
来源：http://mobile.vehdjk.com/Article/details/gvbgwtlib.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.epnwcf.com/Article/details/gcpoavvkm.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.vehdjk.com/Article/details/gdzxmewfy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.bbcook.cn/Article/details/grrocaonl.sHtML

[R47] sed 单行替换
来源：http://m.share.tarul.cn/Article/details/gnnqtfzul.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.tarul.cn/Article/details/gtgdnxepm.sHtML

[R48] awk 取指定列
来源：http://mobile.sjlbkw.cn/Article/details/gvdtrjfck.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fktsv.cn/Article/details/gthzrwqju.sHtML

[R49] awk 带条件
来源：http://www.blog.bbcook.cn/Article/details/gqoyolocm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.vehdjk.com/Article/details/gnubhsjrc.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/gjinowppb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gufmdaebn.sHtML

[R51] 排序去重取前几
来源：http://read.share.sjlbkw.cn/Article/details/gkqkfjffu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/ghbyucoyt.sHtML

[R52] 统计行数
来源：http://baike.sjlbkw.cn/Article/details/gdrpxphtb.sHtML

wc -l a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gfppzztbr.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fktsv.cn/Article/details/gbeocxyzk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.sjlbkw.cn/Article/details/gjzyvnpfr.sHtML

[R54] 比较两个文件
来源：http://m.share.fktsv.cn/Article/details/gvrlfquyf.sHtML

diff a.txt b.txt
来源：http://www.blog.fktsv.cn/Article/details/glzlgatjl.sHtML

[R55] 压缩与解压
来源：http://www.share.fktsv.cn/Article/details/gliaypqyq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.bbcook.cn/Article/details/gvkxbvauv.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/gbuvfxjzm.sHtML

scp file user@host:/path/
来源：http://read.share.epnwcf.com/Article/details/gdljvmqyh.sHtML

[R57] 远程执行命令
来源：http://m.share.sjlbkw.cn/Article/details/gqvnplnri.sHtML

ssh user@host 'uptime'
来源：http://baike.fktsv.cn/Article/details/gnylkizrn.sHtML

[R58] 下载文件
来源：http://wap.bbcook.cn/Article/details/gkjqapfwu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.tarul.cn/Article/details/ghvnzxedi.sHtML

[R59] 发 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/gptslkiyf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.sjlbkw.cn/Article/details/gkcxeryha.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gvadzbhlf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.bbcook.cn/Article/details/gitaatity.sHtML

[R61] 磁盘占用
来源：http://wap.bbcook.cn/Article/details/gqgwejjfm.sHtML

df -h;  du -sh *
来源：http://blog.yfazqb.com/Article/details/gybjxodax.sHtML

[R62] 找最占空间的文件
来源：http://read.share.yfazqb.com/Article/details/gqmbjomou.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.epnwcf.com/Article/details/gndsruwwd.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gdgcxsozm.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.sjlbkw.cn/Article/details/ghugktljr.sHtML

[R64] 结束进程
来源：http://3g.sjlbkw.cn/Article/details/gtguxjjpz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.vehdjk.com/Article/details/gqbzdfbdn.sHtML

[R65] 查看端口占用
来源：http://3g.sjlbkw.cn/Article/details/ghenomouc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.tarul.cn/Article/details/gbddejfla.sHtML

[R66] 定时任务
来源：http://www.m.share.yfazqb.com/Article/details/gdbbmgdwo.sHtML

crontab -e;  crontab -l
来源：http://m.share.tarul.cn/Article/details/grzkzzaii.sHtML

[R67] 生成随机十六进制串
来源：http://wap.sjlbkw.cn/Article/details/ggqjketsr.sHtML

openssl rand -hex 16
来源：http://www.share.vehdjk.com/Article/details/gzyqqrghj.sHtML

[R68] 计算文件校验值
来源：http://3g.bbcook.cn/Article/details/grmasdjcy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.yfazqb.com/Article/details/glzxmhwvs.sHtML

[R69] 生成随机密码
来源：http://www.share.sjlbkw.cn/Article/details/gqwnvnigi.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.vehdjk.com/Article/details/gmndaunrx.sHtML

[R70] 时间戳与互转
来源：http://m.share.vehdjk.com/Article/details/gcxpvncdg.sHtML

date +%s;  date -d @1700000000
来源：http://blog.epnwcf.com/Article/details/gmrljglez.sHtML

[R71] 日期格式化
来源：http://wap.yfazqb.com/Article/details/girjdiowe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.epnwcf.com/Article/details/gbdmjzhjb.sHtML

[R72] 等待端口就绪
来源：http://wap.vehdjk.com/Article/details/gtehwhukt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.sjlbkw.cn/Article/details/ggmuotmot.sHtML

[R73] 分割大日志
来源：http://baike.yfazqb.com/Article/details/gqfhqertl.sHtML

split -l 1000 big.log part_
来源：http://blog.bbcook.cn/Article/details/ghvywwmfa.sHtML

[R74] 批量重命名
来源：http://baike.epnwcf.com/Article/details/gkwxnggbn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwjahmrn.sHtML

[R75] 导出环境变量
来源：http://blog.tarul.cn/Article/details/gbenubuwz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.bbcook.cn/Article/details/gmcgdltwt.sHtML

[R76] 使用临时文件
来源：http://www.m.share.vehdjk.com/Article/details/gfmrhifwt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/groyaiqlp.sHtML

[R77] 读取用户输入
来源：http://www.blog.fktsv.cn/Article/details/ggsfktawb.sHtML

read -rp "请输入: " ans
来源：http://blog.bbcook.cn/Article/details/gbaoxqilo.sHtML

[R78] 交互式菜单
来源：http://blog.yfazqb.com/Article/details/gjquixekr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fktsv.cn/Article/details/gncxujyvw.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.bbcook.cn/Article/details/gqvrmdlag.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.vehdjk.com/Article/details/gygfitlah.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.vehdjk.com/Article/details/gqzfbqyak.sHtML

time ./run.sh
来源：http://www.share.yfazqb.com/Article/details/gtadlohkn.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/glkvgldix.sHtML

S. C / C++ 专题
来源：http://baike.vehdjk.com/Article/details/gmmbzjwbw.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmsggwfn.sHtML

[S01] C：Hello World
来源：http://baike.fktsv.cn/Article/details/goggzhgib.sHtML

#include <stdio.h>
来源：http://www.m.share.bbcook.cn/Article/details/genadgwvp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.vehdjk.com/Article/details/gorvtcytd.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.yfazqb.com/Article/details/ggxjcmxdd.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.yfazqb.com/Article/details/gyemsvnec.sHtML

[S03] C：读入整数
来源：http://www.blog.sjlbkw.cn/Article/details/gzkkcrpru.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.yfazqb.com/Article/details/gyjgllaau.sHtML

[S04] C：字符串复制
来源：http://www.share.fktsv.cn/Article/details/gbuszabrg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.vehdjk.com/Article/details/gdkejifas.sHtML

[S05] C：字符串长度
来源：http://www.share.epnwcf.com/Article/details/gcyvbkcho.sHtML

strlen(s)
来源：http://mobile.sjlbkw.cn/Article/details/gdwjysojr.sHtML

[S06] C：字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gziotccjk.sHtML

strcmp(a, b) == 0
来源：http://m.share.tarul.cn/Article/details/gkjgefpiq.sHtML

[S07] C：数组遍历求和
来源：http://m.share.epnwcf.com/Article/details/gcbqzkkht.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.yfazqb.com/Article/details/gwkizflhw.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.sjlbkw.cn/Article/details/gravhizoc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.vehdjk.com/Article/details/gkneyzpvc.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fktsv.cn/Article/details/giyuvljjm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.yfazqb.com/Article/details/grrxzcjsx.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.yfazqb.com/Article/details/gqwbnzzjq.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.vehdjk.com/Article/details/gnmxaupfx.sHtML

[S11] C：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gnvdhrtvi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.yfazqb.com/Article/details/gaqwfknqw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.yfazqb.com/Article/details/ghleipjmv.sHtML

fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/grrisidij.sHtML

[S12] C：写文件
来源：http://read.share.fktsv.cn/Article/details/gxwktygtl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gdznbqxte.sHtML

[S13] C：宏定义
来源：http://wap.yfazqb.com/Article/details/gihbrwwhe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/gtxfiiqiu.sHtML

[S14] C：枚举
来源：http://3g.vehdjk.com/Article/details/ghyfzlshe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.tarul.cn/Article/details/gnmzleznj.sHtML

[S15] C：类型转换
来源：http://blog.yfazqb.com/Article/details/ggsbumdqd.sHtML

(double) a / b
来源：http://blog.bbcook.cn/Article/details/glzlxgmzm.sHtML

[S16] C：位操作置位
来源：http://read.share.epnwcf.com/Article/details/gnvojxnhu.sHtML

x |= (1 << 3);
来源：http://www.blog.tarul.cn/Article/details/gpadlohug.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.yfazqb.com/Article/details/gqnzgsvcn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.epnwcf.com/Article/details/gnqliptyj.sHtML

[S18] C：命令行参数
来源：http://blog.tarul.cn/Article/details/gslsaqpbi.sHtML

int main(int argc, char **argv)
来源：http://baike.tarul.cn/Article/details/gvpproses.sHtML

[S19] C：快速排序
来源：http://m.share.yfazqb.com/Article/details/gfoiuruqo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/ghroxesce.sHtML

[S20] C：二分查找
来源：http://blog.yfazqb.com/Article/details/gadmdjmdq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gldsjdgkh.sHtML

[S21] C：字符类别判断
来源：http://3g.bbcook.cn/Article/details/gwhbmziyk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/gpwjoqtej.sHtML

[S22] C：字符串转数字
来源：http://wap.fktsv.cn/Article/details/gzrjhtmyc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fktsv.cn/Article/details/glrauwijh.sHtML

[S23] C：随机数
来源：http://wap.fktsv.cn/Article/details/gcndjullo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.tarul.cn/Article/details/gkbkvfisk.sHtML

[S24] C：获取本地时间
来源：http://read.share.sjlbkw.cn/Article/details/gfmudzyep.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.vehdjk.com/Article/details/glaeefucr.sHtML

[S25] C：内存拷贝
来源：http://baike.fktsv.cn/Article/details/gzevhoswe.sHtML

memcpy(dst, src, n);
来源：http://baike.bbcook.cn/Article/details/gypgdymhx.sHtML

[S26] C：内存清零
来源：http://wap.yfazqb.com/Article/details/gnsgvdfne.sHtML

memset(a, 0, sizeof a);
来源：http://3g.epnwcf.com/Article/details/gmvcsbdok.sHtML

[S27] C：定义常量
来源：http://www.share.yfazqb.com/Article/details/gduiuuzxa.sHtML

const double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gcjgxdlfr.sHtML

[S28] C：静态变量
来源：http://wap.tarul.cn/Article/details/gwyegsknz.sHtML

static int counter = 0;
来源：http://mobile.epnwcf.com/Article/details/gthqcdebj.sHtML

[S29] C：变参函数
来源：http://read.share.tarul.cn/Article/details/getvduisw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fktsv.cn/Article/details/gvzhzwqon.sHtML

[S30] C：头文件保护
来源：http://mobile.sjlbkw.cn/Article/details/gbfynuchs.sHtML

#ifndef X_H
来源：http://baike.tarul.cn/Article/details/gkgmchupr.sHtML

#define X_H
来源：http://read.share.fktsv.cn/Article/details/gnofaxqsz.sHtML

#endif
来源：http://3g.bbcook.cn/Article/details/gtakcpvtv.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gtvimzoug.sHtML

#include <iostream>
来源：http://3g.vehdjk.com/Article/details/gojafjcic.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.sjlbkw.cn/Article/details/gmmwjqipz.sHtML

[S32] C++：字符串
来源：http://www.share.yfazqb.com/Article/details/gdxfxdfey.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.tarul.cn/Article/details/geqwfpocu.sHtML

[S33] C++：vector 增删
来源：http://m.share.bbcook.cn/Article/details/grgvlvzas.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.tarul.cn/Article/details/gvbuytkch.sHtML

[S34] C++：遍历 vector
来源：http://read.share.epnwcf.com/Article/details/gpjaxtitb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.sjlbkw.cn/Article/details/gaqbwwtkg.sHtML

[S35] C++：map
来源：http://wap.fktsv.cn/Article/details/gbsxuluag.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gdtumtcqk.sHtML

[S36] C++：unordered_map
来源：http://wap.fktsv.cn/Article/details/gubhhhath.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/gdrivpzng.sHtML

[S37] C++：set
来源：http://mobile.vehdjk.com/Article/details/gjylzbgqn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gopzuuctf.sHtML

[S38] C++：排序
来源：http://www.share.epnwcf.com/Article/details/gxkpnpnxu.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.vehdjk.com/Article/details/gimpprlib.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.yfazqb.com/Article/details/gzxorcgaj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.vehdjk.com/Article/details/gfdjkfttl.sHtML

[S40] C++：查找元素
来源：http://3g.epnwcf.com/Article/details/gmwpcenvy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.bbcook.cn/Article/details/gixnkbqox.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.tarul.cn/Article/details/gwtwfuide.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.bbcook.cn/Article/details/gmjglpklp.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/gggjbghne.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fktsv.cn/Article/details/gumeikuog.sHtML

[S43] C++：智能指针
来源：http://3g.yfazqb.com/Article/details/gpjfkwqck.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.sjlbkw.cn/Article/details/ghcalwjip.sHtML

[S44] C++：引用传参
来源：http://blog.yfazqb.com/Article/details/guapnqvpi.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fktsv.cn/Article/details/gdvklqcju.sHtML

[S45] C++：lambda
来源：http://blog.sjlbkw.cn/Article/details/grlzwsvup.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fktsv.cn/Article/details/ggqpgeavl.sHtML

[S46] C++：函数模板
来源：http://read.share.epnwcf.com/Article/details/gvojhkhpq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.sjlbkw.cn/Article/details/gmlqmalad.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.sjlbkw.cn/Article/details/gtwqftfnt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.bbcook.cn/Article/details/gaprovqug.sHtML

[S48] C++：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gpdtkjbvv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.vehdjk.com/Article/details/gyhqyyqii.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fktsv.cn/Article/details/gfrkhnunk.sHtML

[S49] C++：写文件
来源：http://3g.tarul.cn/Article/details/gspkecpua.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.yfazqb.com/Article/details/gmjjopnqt.sHtML

[S50] C++：格式化数字
来源：http://mobile.sjlbkw.cn/Article/details/gvrwaxghp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.bbcook.cn/Article/details/gakymcotg.sHtML

[S51] C++：显式类型转换
来源：http://read.share.vehdjk.com/Article/details/ggmozbphl.sHtML

static_cast<double>(a) / b
来源：http://www.share.vehdjk.com/Article/details/gvjlzgmyb.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.epnwcf.com/Article/details/gtctgiqnu.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.tarul.cn/Article/details/gatvmsaix.sHtML

[S53] C++：移动语义
来源：http://www.share.vehdjk.com/Article/details/grjplipdc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.epnwcf.com/Article/details/gnskwssni.sHtML

[S54] C++：异常处理
来源：http://3g.tarul.cn/Article/details/ghhdkpjxq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.sjlbkw.cn/Article/details/gndsfzzre.sHtML

[S55] C++：结构化绑定
来源：http://www.share.bbcook.cn/Article/details/gblggrczi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.epnwcf.com/Article/details/gdqfrucba.sHtML

[S56] C++：optional
来源：http://blog.bbcook.cn/Article/details/gfbtezpib.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.yfazqb.com/Article/details/gfjnzecbd.sHtML

[S57] C++：编译期常量
来源：http://www.blog.sjlbkw.cn/Article/details/gkkoieqbp.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/gvozsqruj.sHtML

[S58] C++：命名空间
来源：http://www.blog.tarul.cn/Article/details/gsuahwanh.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.tarul.cn/Article/details/gxwutgoov.sHtML

[S59] C++：静态断言
来源：http://www.blog.tarul.cn/Article/details/gabpaustt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.vehdjk.com/Article/details/gccxfxely.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/gmhyuggcg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gehbnhaup.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gczlavumj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.tarul.cn/Article/details/gotalirpm.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gplulffdo.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/gfwhkyauv.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/goydmxfon.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gvywvqkbc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.vehdjk.com/Article/details/gohghgobm.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.sjlbkw.cn/Article/details/gqlceayfr.sHtML

"值: $b"
来源：http://baike.epnwcf.com/Article/details/gzdevslue.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.epnwcf.com/Article/details/grpyfgmhg.sHtML

val n: String? = null;  n?.length
来源：http://wap.bbcook.cn/Article/details/gzbthgark.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/glcmicogo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.epnwcf.com/Article/details/ggzxouzvs.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fktsv.cn/Article/details/gdacqnbtl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/ggcwwnrgt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gytsulwrd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.sjlbkw.cn/Article/details/ggutqmiew.sHtML

[T08] Kotlin：数据类
来源：http://mobile.bbcook.cn/Article/details/gbcainbkb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.yfazqb.com/Article/details/gvwqyqswy.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.vehdjk.com/Article/details/gnxqgrlay.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.yfazqb.com/Article/details/geiydawdv.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.yfazqb.com/Article/details/gketwfazb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.epnwcf.com/Article/details/gjthbvael.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/giccmdbfc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fktsv.cn/Article/details/gvhkfdfwl.sHtML

[T12] Kotlin：解构声明
来源：http://wap.tarul.cn/Article/details/glueisgao.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/gkkmemqbo.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.yfazqb.com/Article/details/ggfmlgckv.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.sjlbkw.cn/Article/details/gcgqupzdm.sHtML

[T14] Kotlin：循环
来源：http://baike.yfazqb.com/Article/details/gkhvmzijx.sHtML

for (i in 1..10) println(i)
来源：http://blog.yfazqb.com/Article/details/gcrvwbmnw.sHtML

[T15] Kotlin：接口
来源：http://www.share.bbcook.cn/Article/details/gvtsrstad.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.epnwcf.com/Article/details/gtuqjjlbv.sHtML

[T16] Swift：Hello World
来源：http://www.share.fktsv.cn/Article/details/gxriczofb.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/gxzeegzhb.sHtML

[T17] Swift：变量与常量
来源：http://mobile.tarul.cn/Article/details/gghivoeqq.sHtML

var a = 1;  let b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gxkzqzxnh.sHtML

[T18] Swift：字符串插值
来源：http://3g.fktsv.cn/Article/details/gptgisyzj.sHtML

"值: \(b)"
来源：http://blog.tarul.cn/Article/details/gubwwtwgw.sHtML

[T19] Swift：可选绑定
来源：http://wap.vehdjk.com/Article/details/gimelgtxj.sHtML

if let n = opt { print(n) }
来源：http://m.share.tarul.cn/Article/details/gfxznvcur.sHtML

[T20] Swift：数组操作
来源：http://www.share.fktsv.cn/Article/details/gbehvhbfr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.epnwcf.com/Article/details/gkgaxehsx.sHtML

[T21] Swift：遍历
来源：http://m.share.bbcook.cn/Article/details/gadaraabu.sHtML

for x in a { print(x) }
来源：http://read.share.fktsv.cn/Article/details/gyqbiifgu.sHtML

[T22] Swift：字典
来源：http://3g.sjlbkw.cn/Article/details/ggwbmxfzd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.yfazqb.com/Article/details/gegpkysnf.sHtML

[T23] Swift：函数
来源：http://www.m.share.epnwcf.com/Article/details/gcmdhyyiu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.tarul.cn/Article/details/glwkvzspb.sHtML

[T24] Swift：闭包
来源：http://blog.fktsv.cn/Article/details/glihzdtkw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/goffecoga.sHtML

[T25] Swift：结构体
来源：http://www.m.share.epnwcf.com/Article/details/gkmxjoxxm.sHtML

struct P { var x: Int }
来源：http://baike.tarul.cn/Article/details/gepoxoqir.sHtML

[T26] Swift：类与重写
来源：http://mobile.fktsv.cn/Article/details/goclpyqls.sHtML

class A: Base { override func f() {} }
来源：http://blog.fktsv.cn/Article/details/ghjijarxq.sHtML

[T27] Swift：错误处理
来源：http://blog.fktsv.cn/Article/details/glncrzmsf.sHtML

do { try f() } catch { print(error) }
来源：http://baike.vehdjk.com/Article/details/gywsjmysm.sHtML

[T28] Swift：枚举
来源：http://blog.sjlbkw.cn/Article/details/gmuryeonb.sHtML

enum Color { case red, green }
来源：http://read.share.vehdjk.com/Article/details/gmyzjamxx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.tarul.cn/Article/details/gibexgnoz.sHtML

guard let x = opt else { return }
来源：http://read.share.bbcook.cn/Article/details/gceakzlwo.sHtML

[T30] Swift：协议
来源：http://www.m.share.tarul.cn/Article/details/gcaqljvpf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.sjlbkw.cn/Article/details/gssgcelvh.sHtML

[T31] Lua：Hello World
来源：http://www.share.bbcook.cn/Article/details/gjgyzzplz.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gddqvzqmr.sHtML

[T32] Lua：局部变量
来源：http://baike.epnwcf.com/Article/details/gsszgggia.sHtML

local a = 1
来源：http://m.share.epnwcf.com/Article/details/gcjqjzopm.sHtML

[T33] Lua：表（数组）
来源：http://baike.tarul.cn/Article/details/giedgdqua.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.vehdjk.com/Article/details/guxvbqbsx.sHtML

[T34] Lua：遍历表
来源：http://blog.yfazqb.com/Article/details/gxyctpazw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.sjlbkw.cn/Article/details/gccvshwob.sHtML

[T35] Lua：字典表
来源：http://baike.bbcook.cn/Article/details/goiwldoue.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.vehdjk.com/Article/details/gnsmwpkpi.sHtML

[T36] Lua：函数
来源：http://www.share.yfazqb.com/Article/details/gtunhtohz.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.bbcook.cn/Article/details/guyumtkzf.sHtML


<!-- 参考信息 -->