代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.tarul.cn/Article/details/gmeqmdvod.sHtML

[R30] 函数返回状态码
来源：http://mobile.vehdjk.com/Article/details/gsjrauneg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fktsv.cn/Article/details/grpkerjye.sHtML

[R31] 局部变量
来源：http://baike.yfazqb.com/Article/details/gfihdrdsf.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.sjlbkw.cn/Article/details/gortmvfes.sHtML

[R32] 参数个数校验
来源：http://www.share.vehdjk.com/Article/details/goivhmpfe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/gdyyqtoxj.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.yfazqb.com/Article/details/gaakwdszb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/gthpbialx.sHtML

[R34] 退出时清理
来源：http://www.blog.tarul.cn/Article/details/gyngqwbmn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gtjhrtrqz.sHtML

[R35] 后台执行并等待
来源：http://read.share.bbcook.cn/Article/details/gvahvixge.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.bbcook.cn/Article/details/gbxxpbxjk.sHtML

[R36] 并发执行多个任务
来源：http://baike.yfazqb.com/Article/details/gdontsndt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fktsv.cn/Article/details/gqzuwlhrx.sHtML

[R37] 把输出赋给变量
来源：http://mobile.sjlbkw.cn/Article/details/gvzevcsae.sHtML

files=$(ls -1)
来源：http://3g.epnwcf.com/Article/details/gauedmslt.sHtML

[R38] 管道串联
来源：http://wap.fktsv.cn/Article/details/gvubzusvs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.sjlbkw.cn/Article/details/ggyddbfrn.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.tarul.cn/Article/details/goqqrsxdi.sHtML

cmd > out.log 2>&1
来源：http://read.share.bbcook.cn/Article/details/gnnsvlmll.sHtML

[R40] 追加写日志
来源：http://blog.tarul.cn/Article/details/gckrltyni.sHtML

echo "log" >> out.log
来源：http://blog.epnwcf.com/Article/details/gzrqhordx.sHtML

[R41] 丢弃输出
来源：http://read.share.sjlbkw.cn/Article/details/gmoyrxvcd.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.yfazqb.com/Article/details/gjmqdxxse.sHtML

[R42] 输入重定向
来源：http://www.share.epnwcf.com/Article/details/gaujljfml.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/gtjqhsioe.sHtML

[R43] 按名字查找文件
来源：http://www.blog.bbcook.cn/Article/details/giewvbutl.sHtML

find . -name "*.log" -type f
来源：http://baike.sjlbkw.cn/Article/details/gkokebnwo.sHtML

[R44] 按修改时间查找
来源：http://baike.sjlbkw.cn/Article/details/gdqhqzjwy.sHtML

find . -mtime -7 -type f
来源：http://m.share.epnwcf.com/Article/details/gjdovhmey.sHtML

[R45] 批量删除
来源：http://www.blog.fktsv.cn/Article/details/gcdxyvkph.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.sjlbkw.cn/Article/details/gqwbsqhtk.sHtML

[R46] 递归替换文件内容
来源：http://www.share.sjlbkw.cn/Article/details/gmhhqhhjf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.vehdjk.com/Article/details/gminspdgp.sHtML

[R47] sed 单行替换
来源：http://www.blog.vehdjk.com/Article/details/gsrselcja.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.epnwcf.com/Article/details/gkfhbqcny.sHtML

[R48] awk 取指定列
来源：http://read.share.epnwcf.com/Article/details/gyaisifre.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.epnwcf.com/Article/details/gvsmpohwc.sHtML

[R49] awk 带条件
来源：http://www.m.share.vehdjk.com/Article/details/ghojbugbh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.vehdjk.com/Article/details/gxkguzfou.sHtML

[R50] awk 求和
来源：http://baike.tarul.cn/Article/details/gbvjnzafi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gmerxivgt.sHtML

[R51] 排序去重取前几
来源：http://blog.sjlbkw.cn/Article/details/gqycnkmhs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.yfazqb.com/Article/details/gyvlkhvct.sHtML

[R52] 统计行数
来源：http://m.share.vehdjk.com/Article/details/gxqlnhode.sHtML

wc -l a.txt
来源：http://3g.bbcook.cn/Article/details/gzwntvpum.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.vehdjk.com/Article/details/gtmhomtuc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.yfazqb.com/Article/details/gsaiizaoh.sHtML

[R54] 比较两个文件
来源：http://m.share.vehdjk.com/Article/details/gllrlmemr.sHtML

diff a.txt b.txt
来源：http://www.m.share.tarul.cn/Article/details/gusohdsyq.sHtML

[R55] 压缩与解压
来源：http://m.share.vehdjk.com/Article/details/ghtqmcqgd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.epnwcf.com/Article/details/gjrwpfnde.sHtML

[R56] 远程拷贝
来源：http://blog.fktsv.cn/Article/details/grsumxfhp.sHtML

scp file user@host:/path/
来源：http://www.m.share.vehdjk.com/Article/details/gjulhztpg.sHtML

[R57] 远程执行命令
来源：http://m.share.bbcook.cn/Article/details/gimigdama.sHtML

ssh user@host 'uptime'
来源：http://m.share.vehdjk.com/Article/details/gycjttfyq.sHtML

[R58] 下载文件
来源：http://blog.fktsv.cn/Article/details/gdxrmnfow.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.sjlbkw.cn/Article/details/glaeowlnt.sHtML

[R59] 发 POST JSON
来源：http://m.share.yfazqb.com/Article/details/ggklgznhk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.bbcook.cn/Article/details/gooihkvek.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/gbjvukcli.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.sjlbkw.cn/Article/details/gmorzhlcm.sHtML

[R61] 磁盘占用
来源：http://wap.vehdjk.com/Article/details/gtgvdjvmj.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/grzvmgsmj.sHtML

[R62] 找最占空间的文件
来源：http://3g.tarul.cn/Article/details/gtjwnybvu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.epnwcf.com/Article/details/gdhjekgre.sHtML

[R63] 内存与进程
来源：http://www.share.fktsv.cn/Article/details/ghjrhrfkk.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.sjlbkw.cn/Article/details/gsgawxddc.sHtML

[R64] 结束进程
来源：http://www.m.share.epnwcf.com/Article/details/gdpcreqzy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.sjlbkw.cn/Article/details/gzehhddtk.sHtML

[R65] 查看端口占用
来源：http://read.share.tarul.cn/Article/details/gkiarhntq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.bbcook.cn/Article/details/gqhxsgnxd.sHtML

[R66] 定时任务
来源：http://blog.sjlbkw.cn/Article/details/gygkiktmx.sHtML

crontab -e;  crontab -l
来源：http://wap.fktsv.cn/Article/details/gjvjxdxim.sHtML

[R67] 生成随机十六进制串
来源：http://baike.vehdjk.com/Article/details/geavbfmgy.sHtML

openssl rand -hex 16
来源：http://baike.epnwcf.com/Article/details/garimlbxw.sHtML

[R68] 计算文件校验值
来源：http://mobile.sjlbkw.cn/Article/details/gdsdbppwl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.vehdjk.com/Article/details/gjqvoteze.sHtML

[R69] 生成随机密码
来源：http://www.blog.fktsv.cn/Article/details/ggxszcfkj.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.yfazqb.com/Article/details/gwkqpjppn.sHtML

[R70] 时间戳与互转
来源：http://m.share.epnwcf.com/Article/details/gfsvhvddl.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.yfazqb.com/Article/details/gppuhyzhu.sHtML

[R71] 日期格式化
来源：http://www.blog.vehdjk.com/Article/details/gxpeobfip.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.vehdjk.com/Article/details/gwryqystt.sHtML

[R72] 等待端口就绪
来源：http://mobile.yfazqb.com/Article/details/gygbfzooo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gagtfgyku.sHtML

[R73] 分割大日志
来源：http://wap.sjlbkw.cn/Article/details/gszsygdez.sHtML

split -l 1000 big.log part_
来源：http://wap.epnwcf.com/Article/details/gigsjqqyf.sHtML

[R74] 批量重命名
来源：http://3g.bbcook.cn/Article/details/gykvcvpja.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.vehdjk.com/Article/details/gvucpsezo.sHtML

[R75] 导出环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpbuzwmj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.yfazqb.com/Article/details/gctrjzzil.sHtML

[R76] 使用临时文件
来源：http://blog.epnwcf.com/Article/details/giqfyiqai.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gdvjetink.sHtML

[R77] 读取用户输入
来源：http://www.share.fktsv.cn/Article/details/gcppipybj.sHtML

read -rp "请输入: " ans
来源：http://baike.yfazqb.com/Article/details/gjtmndknn.sHtML

[R78] 交互式菜单
来源：http://www.m.share.bbcook.cn/Article/details/gqfeocakt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.epnwcf.com/Article/details/gefpybzsw.sHtML

[R79] 解析命令行选项
来源：http://3g.fktsv.cn/Article/details/gjbostcbl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.epnwcf.com/Article/details/gvwwtntau.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/gqpxhtuln.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/gfjlqjwzn.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdtrlcepm.sHtML

S. C / C++ 专题
来源：http://baike.fktsv.cn/Article/details/gjzlmlcgg.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gismptmgo.sHtML

[S01] C：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gqopqyxbk.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/gyfoefkio.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.vehdjk.com/Article/details/gzrrfqkpk.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fktsv.cn/Article/details/gscwmuclq.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.sjlbkw.cn/Article/details/gunqfrbdi.sHtML

[S03] C：读入整数
来源：http://blog.tarul.cn/Article/details/gvmdgavxt.sHtML

int x; scanf("%d", &x);
来源：http://wap.bbcook.cn/Article/details/gbhblrhfm.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/gtxqlzede.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.vehdjk.com/Article/details/gggysdqtc.sHtML

[S05] C：字符串长度
来源：http://3g.fktsv.cn/Article/details/govsljgkt.sHtML

strlen(s)
来源：http://www.share.bbcook.cn/Article/details/gpfrcgfin.sHtML

[S06] C：字符串比较
来源：http://mobile.yfazqb.com/Article/details/gwpyywggi.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/gwaaixnde.sHtML

[S07] C：数组遍历求和
来源：http://read.share.epnwcf.com/Article/details/gpkgxwtdr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.yfazqb.com/Article/details/gfhjrrlpb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.epnwcf.com/Article/details/gfcgqmdmf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.tarul.cn/Article/details/gqyujoolb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.yfazqb.com/Article/details/gwbarawyw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/grnpwhrsp.sHtML

[S10] C：指针与解引用
来源：http://wap.yfazqb.com/Article/details/gjoswavwe.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.epnwcf.com/Article/details/gpnfnrzqf.sHtML

[S11] C：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gizhakvra.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.bbcook.cn/Article/details/gggovbuyh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fktsv.cn/Article/details/gnumteamn.sHtML

fclose(f);
来源：http://wap.yfazqb.com/Article/details/gzzcbiihu.sHtML

[S12] C：写文件
来源：http://3g.yfazqb.com/Article/details/gjymozrnb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/ggcddyanf.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/ggasezecz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.sjlbkw.cn/Article/details/gyarotmcq.sHtML

[S14] C：枚举
来源：http://m.share.bbcook.cn/Article/details/gzarkesao.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.epnwcf.com/Article/details/godjplsjl.sHtML

[S15] C：类型转换
来源：http://mobile.fktsv.cn/Article/details/gkpuhuyla.sHtML

(double) a / b
来源：http://baike.fktsv.cn/Article/details/gdqhaipkd.sHtML

[S16] C：位操作置位
来源：http://read.share.epnwcf.com/Article/details/gfbcdyyyb.sHtML

x |= (1 << 3);
来源：http://read.share.yfazqb.com/Article/details/gcxrbdcxl.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gznoghsft.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.bbcook.cn/Article/details/guqcobtab.sHtML

[S18] C：命令行参数
来源：http://baike.tarul.cn/Article/details/grsszlpoa.sHtML

int main(int argc, char **argv)
来源：http://blog.yfazqb.com/Article/details/gwvbtljnz.sHtML

[S19] C：快速排序
来源：http://mobile.yfazqb.com/Article/details/gijgoyvha.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gsniovily.sHtML

[S20] C：二分查找
来源：http://m.share.sjlbkw.cn/Article/details/gynnizuuw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/gpeljlioo.sHtML

[S21] C：字符类别判断
来源：http://read.share.bbcook.cn/Article/details/gislruxme.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.sjlbkw.cn/Article/details/gfpzifecs.sHtML

[S22] C：字符串转数字
来源：http://baike.bbcook.cn/Article/details/gficskwyl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fktsv.cn/Article/details/gszuzkuvn.sHtML

[S23] C：随机数
来源：http://wap.bbcook.cn/Article/details/gjwmdwicu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.vehdjk.com/Article/details/gatwflbix.sHtML

[S24] C：获取本地时间
来源：http://wap.sjlbkw.cn/Article/details/gpkdjgaij.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.vehdjk.com/Article/details/gxtinpkyv.sHtML

[S25] C：内存拷贝
来源：http://mobile.yfazqb.com/Article/details/gcnouesch.sHtML

memcpy(dst, src, n);
来源：http://m.share.fktsv.cn/Article/details/gnepzdrmj.sHtML

[S26] C：内存清零
来源：http://mobile.vehdjk.com/Article/details/gquczniio.sHtML

memset(a, 0, sizeof a);
来源：http://blog.epnwcf.com/Article/details/gycguiouz.sHtML

[S27] C：定义常量
来源：http://blog.bbcook.cn/Article/details/ghbpxsbkc.sHtML

const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gsubcszrd.sHtML

[S28] C：静态变量
来源：http://blog.sjlbkw.cn/Article/details/grtgxhnas.sHtML

static int counter = 0;
来源：http://mobile.sjlbkw.cn/Article/details/gxmnobxve.sHtML

[S29] C：变参函数
来源：http://www.blog.fktsv.cn/Article/details/gwialnycj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fktsv.cn/Article/details/gcnujnvtp.sHtML

[S30] C：头文件保护
来源：http://wap.fktsv.cn/Article/details/gcxkafvaz.sHtML

#ifndef X_H
来源：http://baike.vehdjk.com/Article/details/geoelnqdn.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/gkpgiwccg.sHtML

#endif
来源：http://www.m.share.bbcook.cn/Article/details/gwccujsfv.sHtML

[S31] C++：Hello World
来源：http://3g.tarul.cn/Article/details/gpscolbvn.sHtML

#include <iostream>
来源：http://www.m.share.vehdjk.com/Article/details/gxtsmtzqf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fktsv.cn/Article/details/glopuvcsb.sHtML

[S32] C++：字符串
来源：http://3g.bbcook.cn/Article/details/gtacgsmtm.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/gaanblmcv.sHtML

[S33] C++：vector 增删
来源：http://blog.bbcook.cn/Article/details/gepvlnjgr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.bbcook.cn/Article/details/guufotdvi.sHtML

[S34] C++：遍历 vector
来源：http://3g.tarul.cn/Article/details/gglanfbae.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.sjlbkw.cn/Article/details/gfbhgotue.sHtML

[S35] C++：map
来源：http://blog.vehdjk.com/Article/details/gisgtfgtm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gezbkeorl.sHtML

[S36] C++：unordered_map
来源：http://www.share.tarul.cn/Article/details/gjnrggdsn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/gkuobbwkj.sHtML

[S37] C++：set
来源：http://m.share.tarul.cn/Article/details/ghmivlsdg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fktsv.cn/Article/details/gryzukccd.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gvfxzavyl.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fktsv.cn/Article/details/gfxagkanz.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.sjlbkw.cn/Article/details/groyoqgdg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.epnwcf.com/Article/details/gygzznkbe.sHtML

[S40] C++：查找元素
来源：http://read.share.yfazqb.com/Article/details/gduwqrxrw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.vehdjk.com/Article/details/glnnvukbo.sHtML

[S41] C++：类与构造函数
来源：http://baike.tarul.cn/Article/details/gvhsmpgjd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.bbcook.cn/Article/details/gxnahveat.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.sjlbkw.cn/Article/details/gawpjpfmk.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.tarul.cn/Article/details/gdcmjjgdf.sHtML

[S43] C++：智能指针
来源：http://read.share.epnwcf.com/Article/details/geiveybbi.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.tarul.cn/Article/details/gtxsaijml.sHtML

[S44] C++：引用传参
来源：http://www.share.yfazqb.com/Article/details/griwdbzob.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.yfazqb.com/Article/details/gtaayfnxy.sHtML

[S45] C++：lambda
来源：http://baike.vehdjk.com/Article/details/gswaglhnz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.yfazqb.com/Article/details/glfvdezgm.sHtML

[S46] C++：函数模板
来源：http://wap.tarul.cn/Article/details/gjsaibqdv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.bbcook.cn/Article/details/gkeqiuaxh.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fktsv.cn/Article/details/gjyosuupi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.yfazqb.com/Article/details/glcjjtuid.sHtML

[S48] C++：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/ghjsvhwiq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/gagnjvzsw.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gwhtxhunk.sHtML

[S49] C++：写文件
来源：http://3g.epnwcf.com/Article/details/gmskmhqva.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.yfazqb.com/Article/details/gqnebdxuf.sHtML

[S50] C++：格式化数字
来源：http://baike.sjlbkw.cn/Article/details/ggpdtcuiz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.epnwcf.com/Article/details/gjrlaoedp.sHtML

[S51] C++：显式类型转换
来源：http://3g.yfazqb.com/Article/details/gvyzsduzr.sHtML

static_cast<double>(a) / b
来源：http://m.share.vehdjk.com/Article/details/gnmzhqkzi.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.sjlbkw.cn/Article/details/gwwvlmhzq.sHtML

int size() const noexcept { return n_; }
来源：http://blog.bbcook.cn/Article/details/gcyeknrvh.sHtML

[S53] C++：移动语义
来源：http://www.share.tarul.cn/Article/details/gsqobxdrs.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/glluelbav.sHtML

[S54] C++：异常处理
来源：http://blog.fktsv.cn/Article/details/gvrsqmzsv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.yfazqb.com/Article/details/grsoekidb.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/gafhcyoyf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gffekpzgy.sHtML

[S56] C++：optional
来源：http://mobile.bbcook.cn/Article/details/goywdzhwt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.sjlbkw.cn/Article/details/gxdcycukg.sHtML

[S57] C++：编译期常量
来源：http://baike.yfazqb.com/Article/details/geqfuzhmu.sHtML

constexpr int N = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gcieuxusb.sHtML

[S58] C++：命名空间
来源：http://baike.tarul.cn/Article/details/ggvwomefp.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.tarul.cn/Article/details/gaoringif.sHtML

[S59] C++：静态断言
来源：http://read.share.vehdjk.com/Article/details/gkjhnpvas.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.tarul.cn/Article/details/gojcrykbr.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.tarul.cn/Article/details/guimidjns.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.bbcook.cn/Article/details/gcycxixvf.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkmrsixwa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.bbcook.cn/Article/details/gphspctrw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gkngdekmj.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gdpgarlht.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gvxoiyokh.sHtML

[T02] Kotlin：变量
来源：http://www.share.epnwcf.com/Article/details/gjeqzozdv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.vehdjk.com/Article/details/gaxoiqdtq.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fktsv.cn/Article/details/gtnnzmivl.sHtML

"值: $b"
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsuozgug.sHtML

[T04] Kotlin：空安全
来源：http://blog.yfazqb.com/Article/details/glmfhcuvz.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fktsv.cn/Article/details/gtlbniyex.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.vehdjk.com/Article/details/getdxtgsb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.epnwcf.com/Article/details/gipkzrjhn.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gnoxffjhh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fktsv.cn/Article/details/ggxglfckl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/ghcxmgnki.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fktsv.cn/Article/details/gxhmngpkf.sHtML

[T08] Kotlin：数据类
来源：http://3g.fktsv.cn/Article/details/grynzovhx.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.bbcook.cn/Article/details/gvyfsatue.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.yfazqb.com/Article/details/gvimosexm.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.epnwcf.com/Article/details/gtauioooj.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.yfazqb.com/Article/details/gwztgnmqh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.bbcook.cn/Article/details/gcvxuwcme.sHtML

[T11] Kotlin：协程
来源：http://3g.vehdjk.com/Article/details/ggwbvtmcu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.tarul.cn/Article/details/gebryjoua.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/gwetedkpe.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gkwvxlxev.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.epnwcf.com/Article/details/guwjwrqit.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.yfazqb.com/Article/details/gvlfrnwfd.sHtML

[T14] Kotlin：循环
来源：http://blog.bbcook.cn/Article/details/gnpvqetxp.sHtML

for (i in 1..10) println(i)
来源：http://3g.yfazqb.com/Article/details/gjemumttc.sHtML

[T15] Kotlin：接口
来源：http://blog.tarul.cn/Article/details/gkxdklply.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.sjlbkw.cn/Article/details/grqvdazfy.sHtML

[T16] Swift：Hello World
来源：http://m.share.yfazqb.com/Article/details/gornkaucn.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gtbqzcbmr.sHtML

[T17] Swift：变量与常量
来源：http://read.share.yfazqb.com/Article/details/gqcknetna.sHtML

var a = 1;  let b = 2
来源：http://3g.sjlbkw.cn/Article/details/gllqmnhvh.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gvxbcwhpo.sHtML

"值: \(b)"
来源：http://www.share.bbcook.cn/Article/details/gufbwbtku.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.bbcook.cn/Article/details/gtahsbzpd.sHtML

if let n = opt { print(n) }
来源：http://www.share.fktsv.cn/Article/details/gmpepuykw.sHtML

[T20] Swift：数组操作
来源：http://blog.vehdjk.com/Article/details/gdvsdrqjx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.yfazqb.com/Article/details/gamgwetke.sHtML

[T21] Swift：遍历
来源：http://wap.vehdjk.com/Article/details/guzwhswgo.sHtML

for x in a { print(x) }
来源：http://read.share.sjlbkw.cn/Article/details/gcmyntwmv.sHtML

[T22] Swift：字典
来源：http://m.share.vehdjk.com/Article/details/gzsgpttxu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.tarul.cn/Article/details/gbxcdzvwh.sHtML

[T23] Swift：函数
来源：http://read.share.epnwcf.com/Article/details/gtorfppag.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fktsv.cn/Article/details/gzrvtzwrx.sHtML

[T24] Swift：闭包
来源：http://3g.tarul.cn/Article/details/gabqkoipj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gefybfrxc.sHtML

[T25] Swift：结构体
来源：http://www.share.tarul.cn/Article/details/gmbkrwdim.sHtML

struct P { var x: Int }
来源：http://m.share.tarul.cn/Article/details/gxgovkxhd.sHtML

[T26] Swift：类与重写
来源：http://blog.sjlbkw.cn/Article/details/gcaphlrjw.sHtML

class A: Base { override func f() {} }
来源：http://read.share.tarul.cn/Article/details/grzahnlwe.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.yfazqb.com/Article/details/gjqdtitxl.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.epnwcf.com/Article/details/gcamcbcos.sHtML

[T28] Swift：枚举
来源：http://www.share.vehdjk.com/Article/details/ggnfsahfp.sHtML

enum Color { case red, green }
来源：http://mobile.tarul.cn/Article/details/gidmrzfpe.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.yfazqb.com/Article/details/gpngmvswt.sHtML

guard let x = opt else { return }
来源：http://wap.yfazqb.com/Article/details/gootafdbk.sHtML

[T30] Swift：协议
来源：http://blog.fktsv.cn/Article/details/gozrkojsk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.yfazqb.com/Article/details/gnhupbpwi.sHtML

[T31] Lua：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gjelmldrj.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/ghqmyytrn.sHtML

[T32] Lua：局部变量
来源：http://blog.bbcook.cn/Article/details/gqanxpknt.sHtML

local a = 1
来源：http://m.share.epnwcf.com/Article/details/geeymezet.sHtML


<!-- 参考信息 -->