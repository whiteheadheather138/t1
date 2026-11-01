代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://3g.vehdjk.com/Article/details/gibehkwiu.sHtML

[R32] 参数个数校验
来源：http://www.share.epnwcf.com/Article/details/gcfbcrhgq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gdcribstg.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.vehdjk.com/Article/details/gyanurucn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.vehdjk.com/Article/details/gblermpgb.sHtML

[R34] 退出时清理
来源：http://www.m.share.bbcook.cn/Article/details/gwmhnmqhe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.bbcook.cn/Article/details/gpwivudcm.sHtML

[R35] 后台执行并等待
来源：http://read.share.vehdjk.com/Article/details/gvgmlfbsx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fktsv.cn/Article/details/gkbcalkhz.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/gryuwribk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.epnwcf.com/Article/details/gqbkomsxs.sHtML

[R37] 把输出赋给变量
来源：http://read.share.vehdjk.com/Article/details/grtuakkug.sHtML

files=$(ls -1)
来源：http://blog.fktsv.cn/Article/details/gcognwdqp.sHtML

[R38] 管道串联
来源：http://3g.vehdjk.com/Article/details/grvkauloz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.epnwcf.com/Article/details/gutyvpfpy.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.sjlbkw.cn/Article/details/glsqpxvky.sHtML

cmd > out.log 2>&1
来源：http://www.blog.vehdjk.com/Article/details/gghepvcll.sHtML

[R40] 追加写日志
来源：http://m.share.yfazqb.com/Article/details/grmimqakq.sHtML

echo "log" >> out.log
来源：http://baike.vehdjk.com/Article/details/gxclykvvk.sHtML

[R41] 丢弃输出
来源：http://blog.bbcook.cn/Article/details/gmfxrmrxb.sHtML

cmd >/dev/null 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gfjdpmmtk.sHtML

[R42] 输入重定向
来源：http://www.m.share.yfazqb.com/Article/details/gwaigebot.sHtML

wc -l < a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gyxbcfcsi.sHtML

[R43] 按名字查找文件
来源：http://mobile.fktsv.cn/Article/details/gbntwwdrm.sHtML

find . -name "*.log" -type f
来源：http://blog.sjlbkw.cn/Article/details/gvpojztrz.sHtML

[R44] 按修改时间查找
来源：http://wap.epnwcf.com/Article/details/guqbbacjz.sHtML

find . -mtime -7 -type f
来源：http://www.share.fktsv.cn/Article/details/gnxfsjgjp.sHtML

[R45] 批量删除
来源：http://mobile.vehdjk.com/Article/details/gzddbnsat.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.vehdjk.com/Article/details/glzqwidwq.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.vehdjk.com/Article/details/gpegjgchy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.epnwcf.com/Article/details/gkacwjuyg.sHtML

[R47] sed 单行替换
来源：http://www.share.yfazqb.com/Article/details/gaszajgdi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gfyewwjuu.sHtML

[R48] awk 取指定列
来源：http://read.share.vehdjk.com/Article/details/gismdscgo.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gbnbdywsg.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/gualrhpca.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.bbcook.cn/Article/details/ggmhevgrq.sHtML

[R50] awk 求和
来源：http://wap.yfazqb.com/Article/details/gkzzbcyzc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gkpruldyb.sHtML

[R51] 排序去重取前几
来源：http://baike.fktsv.cn/Article/details/gtcvtolnn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.tarul.cn/Article/details/gcrzymkex.sHtML

[R52] 统计行数
来源：http://www.share.bbcook.cn/Article/details/gekbfwfsh.sHtML

wc -l a.txt
来源：http://wap.fktsv.cn/Article/details/gvznwrfxi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.vehdjk.com/Article/details/gfndaxbvd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.sjlbkw.cn/Article/details/gxkdrnfqo.sHtML

[R54] 比较两个文件
来源：http://blog.epnwcf.com/Article/details/gzgzmhvmc.sHtML

diff a.txt b.txt
来源：http://3g.epnwcf.com/Article/details/ghelmzvta.sHtML

[R55] 压缩与解压
来源：http://www.blog.vehdjk.com/Article/details/gkoevrudk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.sjlbkw.cn/Article/details/gznhvcxzz.sHtML

[R56] 远程拷贝
来源：http://3g.vehdjk.com/Article/details/gmodfraqt.sHtML

scp file user@host:/path/
来源：http://www.blog.vehdjk.com/Article/details/gnfusnuis.sHtML

[R57] 远程执行命令
来源：http://3g.fktsv.cn/Article/details/gownvwkny.sHtML

ssh user@host 'uptime'
来源：http://www.share.tarul.cn/Article/details/gcrytmofp.sHtML

[R58] 下载文件
来源：http://m.share.vehdjk.com/Article/details/gpntjndef.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fktsv.cn/Article/details/gdpecpobc.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gdhgkmoqi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.yfazqb.com/Article/details/gkmscppoh.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/goktgpbqm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/ggufkuvpo.sHtML

[R61] 磁盘占用
来源：http://baike.fktsv.cn/Article/details/gpbxywlko.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/gqvzsnbhz.sHtML

[R62] 找最占空间的文件
来源：http://blog.vehdjk.com/Article/details/gqwwszjvm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.epnwcf.com/Article/details/gobwxcqtd.sHtML

[R63] 内存与进程
来源：http://www.blog.fktsv.cn/Article/details/gneunanez.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.sjlbkw.cn/Article/details/gomifjpii.sHtML

[R64] 结束进程
来源：http://m.share.sjlbkw.cn/Article/details/gznodrfwy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.sjlbkw.cn/Article/details/gfordwijn.sHtML

[R65] 查看端口占用
来源：http://blog.fktsv.cn/Article/details/gdqlbcvpx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.bbcook.cn/Article/details/giprwujak.sHtML

[R66] 定时任务
来源：http://www.m.share.yfazqb.com/Article/details/gtwfkubwa.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/grmbnesdr.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/gkxelagkm.sHtML

openssl rand -hex 16
来源：http://www.share.yfazqb.com/Article/details/gtnlsimmo.sHtML

[R68] 计算文件校验值
来源：http://mobile.fktsv.cn/Article/details/gbhcclovz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.yfazqb.com/Article/details/gzflbxycd.sHtML

[R69] 生成随机密码
来源：http://m.share.sjlbkw.cn/Article/details/gpxwwrygw.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.yfazqb.com/Article/details/ghrykpyll.sHtML

[R70] 时间戳与互转
来源：http://baike.vehdjk.com/Article/details/gjjyodvlo.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.bbcook.cn/Article/details/gtpyrtigd.sHtML

[R71] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gsvxyavol.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.yfazqb.com/Article/details/gddnidory.sHtML

[R72] 等待端口就绪
来源：http://read.share.fktsv.cn/Article/details/gcpsdpqkz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.sjlbkw.cn/Article/details/gydbfcmzb.sHtML

[R73] 分割大日志
来源：http://www.blog.tarul.cn/Article/details/gukjgwfho.sHtML

split -l 1000 big.log part_
来源：http://m.share.yfazqb.com/Article/details/gibxdhanx.sHtML

[R74] 批量重命名
来源：http://www.blog.yfazqb.com/Article/details/ghuymacqe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.bbcook.cn/Article/details/gxriosymg.sHtML

[R75] 导出环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gwqbziwxx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.epnwcf.com/Article/details/gnoibtzhn.sHtML

[R76] 使用临时文件
来源：http://m.share.tarul.cn/Article/details/gpzcabsic.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gpfbzklah.sHtML

[R77] 读取用户输入
来源：http://blog.bbcook.cn/Article/details/gkmhkkyuh.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fktsv.cn/Article/details/giciptfsx.sHtML

[R78] 交互式菜单
来源：http://baike.vehdjk.com/Article/details/gncuahebj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.epnwcf.com/Article/details/gzenznuvn.sHtML

[R79] 解析命令行选项
来源：http://baike.fktsv.cn/Article/details/goreiorpm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.tarul.cn/Article/details/gboferzqx.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.bbcook.cn/Article/details/geufhovtx.sHtML

time ./run.sh
来源：http://wap.sjlbkw.cn/Article/details/gvjdhtqwn.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gihhwhgat.sHtML

S. C / C++ 专题
来源：http://www.share.sjlbkw.cn/Article/details/gqriytopt.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gyhuomqho.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/ggivfldds.sHtML

#include <stdio.h>
来源：http://www.m.share.bbcook.cn/Article/details/ghcbouuqs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/gzzesykpm.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gojzuvgqw.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.epnwcf.com/Article/details/glwgvwzpn.sHtML

[S03] C：读入整数
来源：http://baike.fktsv.cn/Article/details/gtgabeaqh.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.bbcook.cn/Article/details/gpbnddgmy.sHtML

[S04] C：字符串复制
来源：http://3g.yfazqb.com/Article/details/gqgkwdzbs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gsqkskmnu.sHtML

[S05] C：字符串长度
来源：http://m.share.yfazqb.com/Article/details/greqlgpds.sHtML

strlen(s)
来源：http://m.share.bbcook.cn/Article/details/gmyphthgu.sHtML

[S06] C：字符串比较
来源：http://www.share.yfazqb.com/Article/details/guhyklbzx.sHtML

strcmp(a, b) == 0
来源：http://blog.bbcook.cn/Article/details/ggnzkbzfv.sHtML

[S07] C：数组遍历求和
来源：http://mobile.tarul.cn/Article/details/gvjdagife.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/goncpxggz.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.epnwcf.com/Article/details/ginyazdrp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/gltmleltn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.bbcook.cn/Article/details/guvziepxf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fktsv.cn/Article/details/gesojsegl.sHtML

[S10] C：指针与解引用
来源：http://www.share.fktsv.cn/Article/details/gxxehuxsb.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.tarul.cn/Article/details/gghbnbbba.sHtML

[S11] C：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gemjqvpgg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.vehdjk.com/Article/details/gdqlhqbgy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.epnwcf.com/Article/details/gqjgjhzzb.sHtML

fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gkvirwytu.sHtML

[S12] C：写文件
来源：http://wap.fktsv.cn/Article/details/gweusheoz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.tarul.cn/Article/details/gdefyvogc.sHtML

[S13] C：宏定义
来源：http://m.share.sjlbkw.cn/Article/details/gaumqwbmf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.tarul.cn/Article/details/gydydsazk.sHtML

[S14] C：枚举
来源：http://m.share.tarul.cn/Article/details/gwofsejkf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.vehdjk.com/Article/details/gwjgujoot.sHtML

[S15] C：类型转换
来源：http://3g.epnwcf.com/Article/details/ggkaridkt.sHtML

(double) a / b
来源：http://blog.tarul.cn/Article/details/gpybikhed.sHtML

[S16] C：位操作置位
来源：http://3g.tarul.cn/Article/details/gaekssvwe.sHtML

x |= (1 << 3);
来源：http://wap.fktsv.cn/Article/details/gukxehpgz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gvuleyift.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.yfazqb.com/Article/details/gfqbztcht.sHtML

[S18] C：命令行参数
来源：http://mobile.bbcook.cn/Article/details/gslhmxddl.sHtML

int main(int argc, char **argv)
来源：http://m.share.tarul.cn/Article/details/gnfbjhwso.sHtML

[S19] C：快速排序
来源：http://3g.fktsv.cn/Article/details/gcffufxov.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gjjhothsp.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gzkrhrvxo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gvahehuih.sHtML

[S21] C：字符类别判断
来源：http://www.share.tarul.cn/Article/details/grsydqrvu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.tarul.cn/Article/details/gzsbhsmmr.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.bbcook.cn/Article/details/gszncdbao.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.tarul.cn/Article/details/gpulqying.sHtML

[S23] C：随机数
来源：http://www.blog.yfazqb.com/Article/details/gnsbkfvbz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.sjlbkw.cn/Article/details/gbyfmyuiw.sHtML

[S24] C：获取本地时间
来源：http://www.share.tarul.cn/Article/details/gztbegpmm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.epnwcf.com/Article/details/gscpullzw.sHtML

[S25] C：内存拷贝
来源：http://www.blog.yfazqb.com/Article/details/gktdyvkcc.sHtML

memcpy(dst, src, n);
来源：http://3g.vehdjk.com/Article/details/guizznhnh.sHtML

[S26] C：内存清零
来源：http://wap.vehdjk.com/Article/details/gtxogfoet.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/ggtxucpap.sHtML

[S27] C：定义常量
来源：http://www.m.share.bbcook.cn/Article/details/gxptdbcnx.sHtML

const double PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gdcgcyrko.sHtML

[S28] C：静态变量
来源：http://read.share.fktsv.cn/Article/details/gbuwftfzd.sHtML

static int counter = 0;
来源：http://www.m.share.tarul.cn/Article/details/gesavflmn.sHtML

[S29] C：变参函数
来源：http://mobile.tarul.cn/Article/details/gdiaoymae.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.bbcook.cn/Article/details/gkhitpzwf.sHtML

[S30] C：头文件保护
来源：http://blog.bbcook.cn/Article/details/gfzfymaiz.sHtML

#ifndef X_H
来源：http://3g.vehdjk.com/Article/details/gvsvwgmsh.sHtML

#define X_H
来源：http://3g.epnwcf.com/Article/details/gdjelxiep.sHtML

#endif
来源：http://www.share.tarul.cn/Article/details/ginfmxfwh.sHtML

[S31] C++：Hello World
来源：http://m.share.yfazqb.com/Article/details/gfdplcign.sHtML

#include <iostream>
来源：http://3g.fktsv.cn/Article/details/gkowqygkl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.sjlbkw.cn/Article/details/gyzixtmvk.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gmsbwcwzv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.vehdjk.com/Article/details/gfwhdojxe.sHtML

[S33] C++：vector 增删
来源：http://www.share.sjlbkw.cn/Article/details/gumndbvol.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fktsv.cn/Article/details/gntzhlwrr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.sjlbkw.cn/Article/details/gumftddmf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.sjlbkw.cn/Article/details/gechxnrjn.sHtML

[S35] C++：map
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnduphfq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gmlpjfkpq.sHtML

[S36] C++：unordered_map
来源：http://blog.epnwcf.com/Article/details/gzpuyteqd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/ghmdhpzej.sHtML

[S37] C++：set
来源：http://m.share.fktsv.cn/Article/details/gdetsvqwc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.epnwcf.com/Article/details/gzwyqqona.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gqiiokhfo.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.tarul.cn/Article/details/garnugmos.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.tarul.cn/Article/details/gbzaumocp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.sjlbkw.cn/Article/details/gxfzjdyzd.sHtML

[S40] C++：查找元素
来源：http://blog.fktsv.cn/Article/details/goatzpjtq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fktsv.cn/Article/details/gkfnzpkhw.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gjhcghnca.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.yfazqb.com/Article/details/gtirpcfin.sHtML

[S42] C++：继承与虚函数
来源：http://wap.epnwcf.com/Article/details/gqdlnjtjq.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.epnwcf.com/Article/details/gkuyklvtk.sHtML

[S43] C++：智能指针
来源：http://baike.sjlbkw.cn/Article/details/gygznmokj.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fktsv.cn/Article/details/gkbscwvvb.sHtML

[S44] C++：引用传参
来源：http://read.share.tarul.cn/Article/details/gevvibwhd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/ggoqelgwy.sHtML

[S45] C++：lambda
来源：http://baike.fktsv.cn/Article/details/gynnuuejk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.yfazqb.com/Article/details/gviqssoyx.sHtML

[S46] C++：函数模板
来源：http://read.share.yfazqb.com/Article/details/gybiiyqzs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.vehdjk.com/Article/details/gnabwlazb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.tarul.cn/Article/details/gipswhwza.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fktsv.cn/Article/details/grqyduykh.sHtML

[S48] C++：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gfsuwakve.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.sjlbkw.cn/Article/details/gbobhqjvv.sHtML

while (std::getline(in, line)) { }
来源：http://baike.tarul.cn/Article/details/gsqsaqhet.sHtML

[S49] C++：写文件
来源：http://baike.tarul.cn/Article/details/gxmhxzgto.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.yfazqb.com/Article/details/ghyhhpbld.sHtML

[S50] C++：格式化数字
来源：http://www.blog.sjlbkw.cn/Article/details/gdjjcxilf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gagsepusu.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fktsv.cn/Article/details/gzrewyicj.sHtML

static_cast<double>(a) / b
来源：http://wap.tarul.cn/Article/details/glqirinbh.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.bbcook.cn/Article/details/gzylfzngz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.bbcook.cn/Article/details/gikcwmsqe.sHtML

[S53] C++：移动语义
来源：http://www.m.share.vehdjk.com/Article/details/gjpkfxsbj.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.epnwcf.com/Article/details/gtojnakji.sHtML

[S54] C++：异常处理
来源：http://baike.fktsv.cn/Article/details/gffpearrt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fktsv.cn/Article/details/gaiekjlhw.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/guhrcfgaf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/geribafpg.sHtML

[S56] C++：optional
来源：http://www.share.epnwcf.com/Article/details/gpcdzmslz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.yfazqb.com/Article/details/gtjyecckl.sHtML

[S57] C++：编译期常量
来源：http://mobile.fktsv.cn/Article/details/gpoixxpnw.sHtML

constexpr int N = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/glwwiyyba.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gzsdtxjch.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/gtjlvtkdb.sHtML

[S59] C++：静态断言
来源：http://mobile.tarul.cn/Article/details/gniekutef.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.bbcook.cn/Article/details/glfngxbxt.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/gdfazvubk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.vehdjk.com/Article/details/ggjvocphj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkkmhdxxu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.sjlbkw.cn/Article/details/gfjdyvpvi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqbhtkosw.sHtML

[T01] Kotlin：Hello World
来源：http://3g.yfazqb.com/Article/details/gkvsvlzua.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/gvyohrkld.sHtML

[T02] Kotlin：变量
来源：http://3g.epnwcf.com/Article/details/gqbyclpsj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.epnwcf.com/Article/details/gpznbqfot.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.yfazqb.com/Article/details/gvvjxbdci.sHtML

"值: $b"
来源：http://www.share.tarul.cn/Article/details/gtpjsmslt.sHtML

[T04] Kotlin：空安全
来源：http://read.share.vehdjk.com/Article/details/gdcsxjivb.sHtML

val n: String? = null;  n?.length
来源：http://read.share.epnwcf.com/Article/details/gtqgojkok.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.sjlbkw.cn/Article/details/gubiiwzse.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.tarul.cn/Article/details/gmzfnmgnt.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.epnwcf.com/Article/details/gncxijvhv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.bbcook.cn/Article/details/glwqhseze.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gtridymzg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.bbcook.cn/Article/details/gkotfexiz.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.sjlbkw.cn/Article/details/ggyrjifxh.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.sjlbkw.cn/Article/details/gwsptxvwt.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.tarul.cn/Article/details/gueybryqj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.vehdjk.com/Article/details/gayfbzffo.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gxrvydcqf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.epnwcf.com/Article/details/gzjaqpvvu.sHtML

[T11] Kotlin：协程
来源：http://wap.fktsv.cn/Article/details/gadxumfwi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.epnwcf.com/Article/details/gqpqoxayd.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fktsv.cn/Article/details/ghqjkhrqw.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/gcltiozjf.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.yfazqb.com/Article/details/gmsbvskek.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.vehdjk.com/Article/details/gzbcgttux.sHtML

[T14] Kotlin：循环
来源：http://www.share.vehdjk.com/Article/details/gwluemhkw.sHtML

for (i in 1..10) println(i)
来源：http://mobile.epnwcf.com/Article/details/grtibojlc.sHtML

[T15] Kotlin：接口
来源：http://www.blog.tarul.cn/Article/details/gimwmxeyy.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.yfazqb.com/Article/details/ghbkhhdqi.sHtML

[T16] Swift：Hello World
来源：http://m.share.vehdjk.com/Article/details/gfegkzldf.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gqpawwfwr.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fktsv.cn/Article/details/ggxovzvyw.sHtML

var a = 1;  let b = 2
来源：http://3g.bbcook.cn/Article/details/gegylkqnx.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gsmwfqeca.sHtML

"值: \(b)"
来源：http://3g.epnwcf.com/Article/details/gvfvlkujf.sHtML

[T19] Swift：可选绑定
来源：http://read.share.yfazqb.com/Article/details/gyzhejeth.sHtML

if let n = opt { print(n) }
来源：http://www.blog.sjlbkw.cn/Article/details/ghmmblsvt.sHtML

[T20] Swift：数组操作
来源：http://mobile.epnwcf.com/Article/details/gmfxguagw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/gihntfaqf.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fktsv.cn/Article/details/guqdfkcup.sHtML

for x in a { print(x) }
来源：http://read.share.fktsv.cn/Article/details/gjqvygare.sHtML

[T22] Swift：字典
来源：http://www.share.bbcook.cn/Article/details/gtkwaxsqw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.bbcook.cn/Article/details/gkzrtujqy.sHtML

[T23] Swift：函数
来源：http://www.blog.tarul.cn/Article/details/gjpzjgiif.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fktsv.cn/Article/details/gwxsystbv.sHtML

[T24] Swift：闭包
来源：http://read.share.epnwcf.com/Article/details/gupyzteyi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gwfifuidh.sHtML

[T25] Swift：结构体
来源：http://www.share.vehdjk.com/Article/details/gaubvcbce.sHtML

struct P { var x: Int }
来源：http://mobile.vehdjk.com/Article/details/gymmjvovk.sHtML

[T26] Swift：类与重写
来源：http://3g.bbcook.cn/Article/details/gtmqjjcsa.sHtML

class A: Base { override func f() {} }
来源：http://baike.fktsv.cn/Article/details/ghzywjdjh.sHtML

[T27] Swift：错误处理
来源：http://wap.tarul.cn/Article/details/gxfganaty.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fktsv.cn/Article/details/gweabuwig.sHtML

[T28] Swift：枚举
来源：http://www.blog.bbcook.cn/Article/details/gjzmxpolt.sHtML

enum Color { case red, green }
来源：http://www.m.share.fktsv.cn/Article/details/gwcazjgcu.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.bbcook.cn/Article/details/gqauswwdo.sHtML

guard let x = opt else { return }
来源：http://mobile.sjlbkw.cn/Article/details/geivebdzb.sHtML

[T30] Swift：协议
来源：http://blog.tarul.cn/Article/details/gvlphxhwl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.yfazqb.com/Article/details/gaiqfuwvz.sHtML

[T31] Lua：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gazqxcehm.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gtreneeli.sHtML

[T32] Lua：局部变量
来源：http://3g.bbcook.cn/Article/details/giqhybewo.sHtML

local a = 1
来源：http://blog.vehdjk.com/Article/details/gaffedqvf.sHtML

[T33] Lua：表（数组）
来源：http://wap.vehdjk.com/Article/details/gmipjnpgv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.yfazqb.com/Article/details/gnbounzxc.sHtML

[T34] Lua：遍历表
来源：http://mobile.vehdjk.com/Article/details/gvxzejzts.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fktsv.cn/Article/details/gnehwzswc.sHtML


<!-- 参考信息 -->