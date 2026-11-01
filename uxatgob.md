代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://m.share.tarul.cn/Article/details/gtdrdppdy.sHtML

[R32] 参数个数校验
来源：http://m.share.yfazqb.com/Article/details/gkwewfzng.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/gmesaxyej.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/gzwzwibji.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.sjlbkw.cn/Article/details/gjfamxaxa.sHtML

[R34] 退出时清理
来源：http://www.blog.sjlbkw.cn/Article/details/gtgxfxlwp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/grntjcrap.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.tarul.cn/Article/details/gjggzvubz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.yfazqb.com/Article/details/gjsvahxgm.sHtML

[R36] 并发执行多个任务
来源：http://www.share.bbcook.cn/Article/details/gqsiydjjf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.sjlbkw.cn/Article/details/ghjqyffrf.sHtML

[R37] 把输出赋给变量
来源：http://m.share.bbcook.cn/Article/details/gcsmzuwoi.sHtML

files=$(ls -1)
来源：http://3g.bbcook.cn/Article/details/gqnksejbb.sHtML

[R38] 管道串联
来源：http://wap.yfazqb.com/Article/details/gynttbvvt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.tarul.cn/Article/details/geuwjlakv.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.epnwcf.com/Article/details/githzsxgs.sHtML

cmd > out.log 2>&1
来源：http://blog.epnwcf.com/Article/details/gbbvigqqp.sHtML

[R40] 追加写日志
来源：http://www.blog.vehdjk.com/Article/details/ghwpvqrbh.sHtML

echo "log" >> out.log
来源：http://mobile.tarul.cn/Article/details/gmwhteasn.sHtML

[R41] 丢弃输出
来源：http://m.share.sjlbkw.cn/Article/details/gqjaodyhc.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gkxbubnrn.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/gvctisdte.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/gwvxihfik.sHtML

[R43] 按名字查找文件
来源：http://wap.sjlbkw.cn/Article/details/gdzcbcfxf.sHtML

find . -name "*.log" -type f
来源：http://mobile.yfazqb.com/Article/details/gncjeqwrw.sHtML

[R44] 按修改时间查找
来源：http://www.share.yfazqb.com/Article/details/gdjuigrfe.sHtML

find . -mtime -7 -type f
来源：http://www.share.vehdjk.com/Article/details/ghatgbekd.sHtML

[R45] 批量删除
来源：http://mobile.epnwcf.com/Article/details/guraszyom.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.yfazqb.com/Article/details/gjwmszcsk.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.epnwcf.com/Article/details/gkycnnebs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.epnwcf.com/Article/details/giaigxgbj.sHtML

[R47] sed 单行替换
来源：http://3g.sjlbkw.cn/Article/details/gfebflbhq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.bbcook.cn/Article/details/gnpmnbfzc.sHtML

[R48] awk 取指定列
来源：http://read.share.sjlbkw.cn/Article/details/gjvdcrlvn.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.bbcook.cn/Article/details/gbcoywpgb.sHtML

[R49] awk 带条件
来源：http://www.m.share.yfazqb.com/Article/details/gtdsneaet.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fktsv.cn/Article/details/gjjvmybrv.sHtML

[R50] awk 求和
来源：http://read.share.epnwcf.com/Article/details/giyubpbfr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gjqqtwkbj.sHtML

[R51] 排序去重取前几
来源：http://www.blog.vehdjk.com/Article/details/gjcppqkqt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/ggyiihsys.sHtML

[R52] 统计行数
来源：http://www.share.tarul.cn/Article/details/gmoyefsgh.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/grsamaehf.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fktsv.cn/Article/details/ggyycgidk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.vehdjk.com/Article/details/gyknqnvqh.sHtML

[R54] 比较两个文件
来源：http://read.share.vehdjk.com/Article/details/ghopknaeo.sHtML

diff a.txt b.txt
来源：http://www.share.bbcook.cn/Article/details/gsbmpyeth.sHtML

[R55] 压缩与解压
来源：http://blog.sjlbkw.cn/Article/details/ggftzcdzf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.bbcook.cn/Article/details/gcskfuiiu.sHtML

[R56] 远程拷贝
来源：http://mobile.tarul.cn/Article/details/gqkmdzfsy.sHtML

scp file user@host:/path/
来源：http://read.share.vehdjk.com/Article/details/ggjnwwgew.sHtML

[R57] 远程执行命令
来源：http://baike.sjlbkw.cn/Article/details/gjxgwxnse.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.tarul.cn/Article/details/gefzndhen.sHtML

[R58] 下载文件
来源：http://www.share.tarul.cn/Article/details/gbviuglce.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fktsv.cn/Article/details/gksftcird.sHtML

[R59] 发 POST JSON
来源：http://m.share.vehdjk.com/Article/details/gwdsvrfbx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fktsv.cn/Article/details/gbwslupgn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gqzjwpbkn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.epnwcf.com/Article/details/gnhtmeiwe.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/gcbzofkoe.sHtML

df -h;  du -sh *
来源：http://www.blog.tarul.cn/Article/details/ghavtfvvu.sHtML

[R62] 找最占空间的文件
来源：http://mobile.bbcook.cn/Article/details/grfcsnmnu.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.yfazqb.com/Article/details/goihjkcer.sHtML

[R63] 内存与进程
来源：http://baike.bbcook.cn/Article/details/gvhpjwqqf.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.yfazqb.com/Article/details/gbpaappox.sHtML

[R64] 结束进程
来源：http://3g.epnwcf.com/Article/details/gtbyqgcqj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.tarul.cn/Article/details/gozilxzum.sHtML

[R65] 查看端口占用
来源：http://baike.yfazqb.com/Article/details/glvywjduh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.bbcook.cn/Article/details/gydsywlhe.sHtML

[R66] 定时任务
来源：http://baike.sjlbkw.cn/Article/details/gaecilmzs.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/guxwncedw.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.tarul.cn/Article/details/gmxuktjvu.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/gxmkurqse.sHtML

[R68] 计算文件校验值
来源：http://wap.epnwcf.com/Article/details/gguenvnnw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.tarul.cn/Article/details/gsrwqmhny.sHtML

[R69] 生成随机密码
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhagslsk.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.sjlbkw.cn/Article/details/gmndidjvr.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.epnwcf.com/Article/details/gvsolxkfo.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.sjlbkw.cn/Article/details/gjrdzmxpx.sHtML

[R71] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gsidzrgbg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fktsv.cn/Article/details/gmefatnpw.sHtML

[R72] 等待端口就绪
来源：http://m.share.epnwcf.com/Article/details/gmkpxtmgl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gvptkucig.sHtML

[R73] 分割大日志
来源：http://wap.bbcook.cn/Article/details/gxkkcwvhm.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fktsv.cn/Article/details/gwthtotpn.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/ggtszshwz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fktsv.cn/Article/details/gpzhumozb.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/gluvfmbes.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fktsv.cn/Article/details/gwyzjsnpg.sHtML

[R76] 使用临时文件
来源：http://baike.sjlbkw.cn/Article/details/gmrnzoale.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.bbcook.cn/Article/details/gtgbyrhsu.sHtML

[R77] 读取用户输入
来源：http://baike.epnwcf.com/Article/details/gltcelyrn.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fktsv.cn/Article/details/geaooadwa.sHtML

[R78] 交互式菜单
来源：http://www.blog.vehdjk.com/Article/details/gwpvfnkxn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.tarul.cn/Article/details/gjhrttlik.sHtML

[R79] 解析命令行选项
来源：http://mobile.vehdjk.com/Article/details/grfukuvey.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.epnwcf.com/Article/details/gjqyheppo.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.tarul.cn/Article/details/gtxeuhewv.sHtML

time ./run.sh
来源：http://3g.bbcook.cn/Article/details/gctahsgnr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gdsiwhlvd.sHtML

S. C / C++ 专题
来源：http://read.share.tarul.cn/Article/details/gqrxbyiso.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gnppetwrp.sHtML

[S01] C：Hello World
来源：http://blog.fktsv.cn/Article/details/gtpcjlupl.sHtML

#include <stdio.h>
来源：http://m.share.tarul.cn/Article/details/gcbbydedl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.bbcook.cn/Article/details/gqgaczcmp.sHtML

[S02] C：变量与格式化输出
来源：http://baike.vehdjk.com/Article/details/gymqbhzvc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.tarul.cn/Article/details/ghdbmuidt.sHtML

[S03] C：读入整数
来源：http://www.share.epnwcf.com/Article/details/gvysbkfio.sHtML

int x; scanf("%d", &x);
来源：http://blog.tarul.cn/Article/details/gnwkjksah.sHtML

[S04] C：字符串复制
来源：http://m.share.yfazqb.com/Article/details/gaowvxanv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.tarul.cn/Article/details/ggeifrftu.sHtML

[S05] C：字符串长度
来源：http://3g.fktsv.cn/Article/details/glrxettts.sHtML

strlen(s)
来源：http://baike.epnwcf.com/Article/details/gtcsicpzb.sHtML

[S06] C：字符串比较
来源：http://m.share.tarul.cn/Article/details/gjxdqkddf.sHtML

strcmp(a, b) == 0
来源：http://blog.epnwcf.com/Article/details/gpxrnujqf.sHtML

[S07] C：数组遍历求和
来源：http://wap.sjlbkw.cn/Article/details/ggfkbeptk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.vehdjk.com/Article/details/gnsgduqlh.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.vehdjk.com/Article/details/gelepzyhe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.yfazqb.com/Article/details/gjigogjzw.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fktsv.cn/Article/details/gqmpgidhn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.bbcook.cn/Article/details/gaifrxlif.sHtML

[S10] C：指针与解引用
来源：http://blog.tarul.cn/Article/details/gvqfnyhri.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.epnwcf.com/Article/details/geleohhai.sHtML

[S11] C：逐行读文件
来源：http://baike.epnwcf.com/Article/details/grojucfrd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.tarul.cn/Article/details/gihlobmsg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.tarul.cn/Article/details/gwqtusfyw.sHtML

fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gaxrjassq.sHtML

[S12] C：写文件
来源：http://mobile.vehdjk.com/Article/details/gfpdynhdp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/ghjpokrls.sHtML

[S13] C：宏定义
来源：http://wap.bbcook.cn/Article/details/gckbeflov.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.bbcook.cn/Article/details/gbgrdojur.sHtML

[S14] C：枚举
来源：http://3g.vehdjk.com/Article/details/gxemzvzwe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.sjlbkw.cn/Article/details/gyeemgzcf.sHtML

[S15] C：类型转换
来源：http://wap.yfazqb.com/Article/details/gcuitxiwb.sHtML

(double) a / b
来源：http://www.m.share.vehdjk.com/Article/details/gwbzsbwzg.sHtML

[S16] C：位操作置位
来源：http://www.m.share.tarul.cn/Article/details/gayxytmah.sHtML

x |= (1 << 3);
来源：http://read.share.fktsv.cn/Article/details/gufkydgiz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gzlokjwzo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fktsv.cn/Article/details/gdypzhdyn.sHtML

[S18] C：命令行参数
来源：http://3g.bbcook.cn/Article/details/goganykty.sHtML

int main(int argc, char **argv)
来源：http://blog.bbcook.cn/Article/details/gsijigmba.sHtML

[S19] C：快速排序
来源：http://read.share.sjlbkw.cn/Article/details/ghefkqzff.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gufqgtsgd.sHtML

[S20] C：二分查找
来源：http://www.m.share.yfazqb.com/Article/details/gxvlckrbc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gyqcgvuku.sHtML

[S21] C：字符类别判断
来源：http://www.blog.epnwcf.com/Article/details/gepvijtna.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fktsv.cn/Article/details/gybvzpzka.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/giqvugrnp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.sjlbkw.cn/Article/details/gmvmnybkl.sHtML

[S23] C：随机数
来源：http://m.share.fktsv.cn/Article/details/gedrqzxis.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.bbcook.cn/Article/details/gqqkacayz.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gjtmbwdvw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fktsv.cn/Article/details/gzqydkhjj.sHtML

[S25] C：内存拷贝
来源：http://blog.epnwcf.com/Article/details/gvmwyevpr.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gxxkrpvwv.sHtML

[S26] C：内存清零
来源：http://www.m.share.tarul.cn/Article/details/gbvubmjkd.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/gxuxfieyr.sHtML

[S27] C：定义常量
来源：http://3g.epnwcf.com/Article/details/ghfivvaie.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gsqiwhetn.sHtML

[S28] C：静态变量
来源：http://wap.fktsv.cn/Article/details/gqgfooisl.sHtML

static int counter = 0;
来源：http://read.share.vehdjk.com/Article/details/gyxwlfcsj.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/glezomrlq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.epnwcf.com/Article/details/gcpzeqnxc.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/gxcnawekv.sHtML

#ifndef X_H
来源：http://3g.epnwcf.com/Article/details/gnusrcsvi.sHtML

#define X_H
来源：http://blog.sjlbkw.cn/Article/details/gmauazfwj.sHtML

#endif
来源：http://mobile.tarul.cn/Article/details/gskddgfvj.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/gahkocrdp.sHtML

#include <iostream>
来源：http://mobile.tarul.cn/Article/details/gqzcozrxj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fktsv.cn/Article/details/gopckxnug.sHtML

[S32] C++：字符串
来源：http://www.m.share.yfazqb.com/Article/details/gcpvjuegy.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fktsv.cn/Article/details/gthrysmau.sHtML

[S33] C++：vector 增删
来源：http://3g.yfazqb.com/Article/details/gevnsvsww.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.sjlbkw.cn/Article/details/grdiqihud.sHtML

[S34] C++：遍历 vector
来源：http://baike.sjlbkw.cn/Article/details/gtnrndvzb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.yfazqb.com/Article/details/gurxmzgvp.sHtML

[S35] C++：map
来源：http://baike.bbcook.cn/Article/details/gvzbdwyir.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/gtcjgslwz.sHtML

[S36] C++：unordered_map
来源：http://mobile.yfazqb.com/Article/details/gwgcxpdxe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/geuuiazyf.sHtML

[S37] C++：set
来源：http://wap.tarul.cn/Article/details/ghohapuyf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.tarul.cn/Article/details/gaotdnpow.sHtML

[S38] C++：排序
来源：http://m.share.bbcook.cn/Article/details/glqcvvkmf.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fktsv.cn/Article/details/gwdrijezp.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.vehdjk.com/Article/details/gxfjbsjkv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.vehdjk.com/Article/details/grmwwomdk.sHtML

[S40] C++：查找元素
来源：http://www.blog.epnwcf.com/Article/details/gfbcrnocz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.epnwcf.com/Article/details/gxxndpbah.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.yfazqb.com/Article/details/gesjlocau.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.tarul.cn/Article/details/gcdyupjcg.sHtML

[S42] C++：继承与虚函数
来源：http://blog.yfazqb.com/Article/details/gezyxkrwk.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fktsv.cn/Article/details/ghafushuk.sHtML

[S43] C++：智能指针
来源：http://www.blog.vehdjk.com/Article/details/gbcxgvrwx.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/gdumvkxye.sHtML

[S44] C++：引用传参
来源：http://read.share.vehdjk.com/Article/details/gxtkybfrx.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fktsv.cn/Article/details/gfoklmtkp.sHtML

[S45] C++：lambda
来源：http://www.blog.sjlbkw.cn/Article/details/gdiarzelx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.bbcook.cn/Article/details/gorzijogp.sHtML

[S46] C++：函数模板
来源：http://3g.fktsv.cn/Article/details/gmoptprhi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.yfazqb.com/Article/details/grgwqijux.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.bbcook.cn/Article/details/grjccltbn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.sjlbkw.cn/Article/details/ggkpwjfpt.sHtML

[S48] C++：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gbppxxztz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.epnwcf.com/Article/details/gqqvsbkww.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.epnwcf.com/Article/details/gsdjyuump.sHtML

[S49] C++：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gknrleyiv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.tarul.cn/Article/details/gmjbprbze.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.yfazqb.com/Article/details/ggjwkgdmq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.bbcook.cn/Article/details/gbkcovfsc.sHtML

[S51] C++：显式类型转换
来源：http://mobile.yfazqb.com/Article/details/gigvqszvv.sHtML

static_cast<double>(a) / b
来源：http://www.share.sjlbkw.cn/Article/details/gewczurpl.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fktsv.cn/Article/details/gjviqylps.sHtML

int size() const noexcept { return n_; }
来源：http://baike.tarul.cn/Article/details/gmeipeakk.sHtML

[S53] C++：移动语义
来源：http://mobile.tarul.cn/Article/details/gcsjiqsta.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.epnwcf.com/Article/details/gujvvlarp.sHtML

[S54] C++：异常处理
来源：http://www.blog.yfazqb.com/Article/details/gbpglwtac.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.tarul.cn/Article/details/gigqaemcy.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.epnwcf.com/Article/details/giwlvksyx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/giprsytjx.sHtML

[S56] C++：optional
来源：http://3g.sjlbkw.cn/Article/details/ghcfjrsjd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.tarul.cn/Article/details/gqbrjjpdy.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/gxocxnkuw.sHtML

constexpr int N = 10;
来源：http://mobile.vehdjk.com/Article/details/gfwqanjgy.sHtML

[S58] C++：命名空间
来源：http://read.share.bbcook.cn/Article/details/gsrmfgacx.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.tarul.cn/Article/details/gzplwuutv.sHtML

[S59] C++：静态断言
来源：http://www.share.bbcook.cn/Article/details/gavrigrzy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.sjlbkw.cn/Article/details/gxproncxw.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.sjlbkw.cn/Article/details/gnlatlwiy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.epnwcf.com/Article/details/ghxuiysjr.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ggmzbuafk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/gqsjeqski.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gccflllca.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.yfazqb.com/Article/details/gtsprliwk.sHtML

println("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gqxucluts.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/gjiyvytrx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.tarul.cn/Article/details/gaugesvfe.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.yfazqb.com/Article/details/grfedldmg.sHtML

"值: $b"
来源：http://baike.fktsv.cn/Article/details/gozkjnrsc.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fktsv.cn/Article/details/gmubiksjv.sHtML

val n: String? = null;  n?.length
来源：http://baike.bbcook.cn/Article/details/gluflbziw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.vehdjk.com/Article/details/gwmwqnwin.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.vehdjk.com/Article/details/gmswjppig.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.tarul.cn/Article/details/gxhytlpld.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.tarul.cn/Article/details/glqohtawa.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/gmlifmskg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.bbcook.cn/Article/details/grouwgkks.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.bbcook.cn/Article/details/gubehkxvk.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fktsv.cn/Article/details/gweglhfbb.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.epnwcf.com/Article/details/gsetpaaqu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.tarul.cn/Article/details/giatlmgqo.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.yfazqb.com/Article/details/glkdeomfr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.vehdjk.com/Article/details/ggzpnnkbd.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyqvrije.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.epnwcf.com/Article/details/gqnaldgor.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fktsv.cn/Article/details/gxkylvuoz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gtnvuiwkq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fktsv.cn/Article/details/gvfbcrvld.sHtML

val m = mapOf("a" to 1)
来源：http://baike.sjlbkw.cn/Article/details/ghufsilst.sHtML

[T14] Kotlin：循环
来源：http://blog.fktsv.cn/Article/details/guhxmjjqz.sHtML

for (i in 1..10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gyayiayja.sHtML

[T15] Kotlin：接口
来源：http://blog.vehdjk.com/Article/details/gqnccxzgq.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.sjlbkw.cn/Article/details/ghchbdeqs.sHtML

[T16] Swift：Hello World
来源：http://www.share.epnwcf.com/Article/details/guysbigsz.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gaioegwui.sHtML

[T17] Swift：变量与常量
来源：http://read.share.vehdjk.com/Article/details/gngujronj.sHtML

var a = 1;  let b = 2
来源：http://blog.vehdjk.com/Article/details/glefaejtk.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlaiydcj.sHtML

"值: \(b)"
来源：http://baike.bbcook.cn/Article/details/gorgoypvs.sHtML

[T19] Swift：可选绑定
来源：http://3g.vehdjk.com/Article/details/gvgewlmhp.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.epnwcf.com/Article/details/gqkxmwyll.sHtML

[T20] Swift：数组操作
来源：http://mobile.fktsv.cn/Article/details/gnvzgrybr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/gjqmlwgjt.sHtML

[T21] Swift：遍历
来源：http://blog.sjlbkw.cn/Article/details/gpihofqpi.sHtML

for x in a { print(x) }
来源：http://www.blog.yfazqb.com/Article/details/gshshpnuw.sHtML

[T22] Swift：字典
来源：http://read.share.sjlbkw.cn/Article/details/gjjdeihmt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.sjlbkw.cn/Article/details/godhgfczv.sHtML

[T23] Swift：函数
来源：http://read.share.sjlbkw.cn/Article/details/gnhgdaxty.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.tarul.cn/Article/details/gpfphmbkv.sHtML

[T24] Swift：闭包
来源：http://www.blog.fktsv.cn/Article/details/gtmhoxcpk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.sjlbkw.cn/Article/details/grcsmsofu.sHtML

[T25] Swift：结构体
来源：http://3g.yfazqb.com/Article/details/gfcskdcik.sHtML

struct P { var x: Int }
来源：http://m.share.sjlbkw.cn/Article/details/gtcdvsast.sHtML

[T26] Swift：类与重写
来源：http://m.share.fktsv.cn/Article/details/ggrrjqkph.sHtML

class A: Base { override func f() {} }
来源：http://wap.yfazqb.com/Article/details/ghhsppxrq.sHtML

[T27] Swift：错误处理
来源：http://wap.tarul.cn/Article/details/giyhabtma.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.yfazqb.com/Article/details/glkyegtnr.sHtML

[T28] Swift：枚举
来源：http://www.blog.yfazqb.com/Article/details/giqextmdj.sHtML

enum Color { case red, green }
来源：http://read.share.tarul.cn/Article/details/gqjlungsi.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.sjlbkw.cn/Article/details/ggkzthqvm.sHtML

guard let x = opt else { return }
来源：http://blog.sjlbkw.cn/Article/details/gjyfrhxpw.sHtML

[T30] Swift：协议
来源：http://baike.epnwcf.com/Article/details/gdqmpjtaj.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.yfazqb.com/Article/details/gflfhkdhp.sHtML

[T31] Lua：Hello World
来源：http://blog.tarul.cn/Article/details/gtzlrpsui.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/gjcjogvil.sHtML

[T32] Lua：局部变量
来源：http://read.share.epnwcf.com/Article/details/gjcrdlcaq.sHtML

local a = 1
来源：http://baike.sjlbkw.cn/Article/details/ggqsiwdbe.sHtML

[T33] Lua：表（数组）
来源：http://3g.vehdjk.com/Article/details/gnihpyrql.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fktsv.cn/Article/details/geubaenjp.sHtML

[T34] Lua：遍历表
来源：http://read.share.bbcook.cn/Article/details/gmjuvjkle.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.vehdjk.com/Article/details/gviljcauu.sHtML


<!-- 参考信息 -->