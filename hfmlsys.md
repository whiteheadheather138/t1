代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.tarul.cn/Article/details/gwgwudayp.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/gpatcbddt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.bbcook.cn/Article/details/gmwqadglx.sHtML

[R31] 局部变量
来源：http://mobile.tarul.cn/Article/details/gejyzsiko.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fktsv.cn/Article/details/gxkjenctl.sHtML

[R32] 参数个数校验
来源：http://read.share.tarul.cn/Article/details/gknetdlat.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gxefvlqhl.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fktsv.cn/Article/details/gtrbzvglb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.epnwcf.com/Article/details/gpstywyyo.sHtML

[R34] 退出时清理
来源：http://m.share.tarul.cn/Article/details/gloundoym.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gxtugscws.sHtML

[R35] 后台执行并等待
来源：http://baike.tarul.cn/Article/details/grtharmiu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.yfazqb.com/Article/details/gstgqbcxs.sHtML

[R36] 并发执行多个任务
来源：http://read.share.bbcook.cn/Article/details/gfvnetdmj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.sjlbkw.cn/Article/details/gekmlnmhe.sHtML

[R37] 把输出赋给变量
来源：http://3g.vehdjk.com/Article/details/gmexdnjsm.sHtML

files=$(ls -1)
来源：http://blog.vehdjk.com/Article/details/glrfkdpux.sHtML

[R38] 管道串联
来源：http://baike.sjlbkw.cn/Article/details/gddqliokd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.vehdjk.com/Article/details/gpwbrxzip.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.sjlbkw.cn/Article/details/gqsonhfgr.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/gcetlzxha.sHtML

[R40] 追加写日志
来源：http://blog.bbcook.cn/Article/details/gezbbuzqu.sHtML

echo "log" >> out.log
来源：http://baike.sjlbkw.cn/Article/details/gejzwhdla.sHtML

[R41] 丢弃输出
来源：http://m.share.vehdjk.com/Article/details/gsqyxmqfg.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gaxrmndpx.sHtML

[R42] 输入重定向
来源：http://wap.vehdjk.com/Article/details/gfpeonnxq.sHtML

wc -l < a.txt
来源：http://www.m.share.tarul.cn/Article/details/glyfmdwzt.sHtML

[R43] 按名字查找文件
来源：http://m.share.epnwcf.com/Article/details/gcgyeyars.sHtML

find . -name "*.log" -type f
来源：http://www.share.bbcook.cn/Article/details/gpxnzjezr.sHtML

[R44] 按修改时间查找
来源：http://mobile.sjlbkw.cn/Article/details/gvoyvzfqo.sHtML

find . -mtime -7 -type f
来源：http://www.share.fktsv.cn/Article/details/gpqwsjotk.sHtML

[R45] 批量删除
来源：http://baike.bbcook.cn/Article/details/gyndsvdgb.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.yfazqb.com/Article/details/gkzpbjhro.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.yfazqb.com/Article/details/guuecguns.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.vehdjk.com/Article/details/gvslusgeq.sHtML

[R47] sed 单行替换
来源：http://wap.bbcook.cn/Article/details/gayagdrlb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/gyisknwpg.sHtML

[R48] awk 取指定列
来源：http://www.blog.vehdjk.com/Article/details/ghgmhedhp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gyidvavzp.sHtML

[R49] awk 带条件
来源：http://3g.epnwcf.com/Article/details/ggkxhkjhf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.sjlbkw.cn/Article/details/gkzjfodbs.sHtML

[R50] awk 求和
来源：http://read.share.bbcook.cn/Article/details/ghzpmaosr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gfcrfdbze.sHtML

[R51] 排序去重取前几
来源：http://wap.sjlbkw.cn/Article/details/gndpcvpmu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fktsv.cn/Article/details/gdnlwglmt.sHtML

[R52] 统计行数
来源：http://read.share.bbcook.cn/Article/details/gxvcieuwb.sHtML

wc -l a.txt
来源：http://3g.fktsv.cn/Article/details/gtadwghfq.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.vehdjk.com/Article/details/gbpxsfxtn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.tarul.cn/Article/details/gtfmppmmf.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/gbvjcxoiq.sHtML

diff a.txt b.txt
来源：http://baike.vehdjk.com/Article/details/grvmztryp.sHtML

[R55] 压缩与解压
来源：http://3g.bbcook.cn/Article/details/gzjpmiumc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.bbcook.cn/Article/details/gttvwojwd.sHtML

[R56] 远程拷贝
来源：http://read.share.fktsv.cn/Article/details/gykoirikv.sHtML

scp file user@host:/path/
来源：http://wap.tarul.cn/Article/details/gkiwiixit.sHtML

[R57] 远程执行命令
来源：http://www.m.share.yfazqb.com/Article/details/giifvsxhp.sHtML

ssh user@host 'uptime'
来源：http://read.share.epnwcf.com/Article/details/gzkdfsjee.sHtML

[R58] 下载文件
来源：http://www.m.share.bbcook.cn/Article/details/gdhxqfptq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/gwhdsxkkg.sHtML

[R59] 发 POST JSON
来源：http://mobile.bbcook.cn/Article/details/gmuhmuwiw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/gyovwhxrd.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.bbcook.cn/Article/details/gsseabyfs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.yfazqb.com/Article/details/gdfxxdbyx.sHtML

[R61] 磁盘占用
来源：http://www.share.vehdjk.com/Article/details/gkmumolaa.sHtML

df -h;  du -sh *
来源：http://www.share.fktsv.cn/Article/details/gzqhhgtfx.sHtML

[R62] 找最占空间的文件
来源：http://wap.vehdjk.com/Article/details/gsbwweimc.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.tarul.cn/Article/details/geweadodo.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/gkejiacxt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.tarul.cn/Article/details/gzkacrdrs.sHtML

[R64] 结束进程
来源：http://baike.yfazqb.com/Article/details/gzvcasvth.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.bbcook.cn/Article/details/gvenyqcpb.sHtML

[R65] 查看端口占用
来源：http://m.share.fktsv.cn/Article/details/glvjlnumz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fktsv.cn/Article/details/glsizcnzm.sHtML

[R66] 定时任务
来源：http://3g.vehdjk.com/Article/details/ghlqplkhu.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/gfkcnqzmz.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.sjlbkw.cn/Article/details/gbebhzodu.sHtML

openssl rand -hex 16
来源：http://baike.vehdjk.com/Article/details/ghudfawjl.sHtML

[R68] 计算文件校验值
来源：http://mobile.yfazqb.com/Article/details/gvsrmsses.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.bbcook.cn/Article/details/gkhevisae.sHtML

[R69] 生成随机密码
来源：http://3g.bbcook.cn/Article/details/gxvsgenll.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.tarul.cn/Article/details/gucyozihs.sHtML

[R70] 时间戳与互转
来源：http://mobile.yfazqb.com/Article/details/gtqxmuich.sHtML

date +%s;  date -d @1700000000
来源：http://baike.vehdjk.com/Article/details/geawgnqay.sHtML

[R71] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/gdlxhqzlf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.sjlbkw.cn/Article/details/gtyjauyhf.sHtML

[R72] 等待端口就绪
来源：http://3g.yfazqb.com/Article/details/gnimroegs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gvwpshyze.sHtML

[R73] 分割大日志
来源：http://mobile.bbcook.cn/Article/details/gdinxjrmk.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/gphuwjhxt.sHtML

[R74] 批量重命名
来源：http://blog.fktsv.cn/Article/details/gmxbooppr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/gvpmlbpnd.sHtML

[R75] 导出环境变量
来源：http://wap.vehdjk.com/Article/details/gibyhivun.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.vehdjk.com/Article/details/grdlxnfky.sHtML

[R76] 使用临时文件
来源：http://blog.bbcook.cn/Article/details/glbfreqsz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gokbxelow.sHtML

[R77] 读取用户输入
来源：http://3g.tarul.cn/Article/details/gnamtocqz.sHtML

read -rp "请输入: " ans
来源：http://mobile.fktsv.cn/Article/details/gdgpqfqxz.sHtML

[R78] 交互式菜单
来源：http://read.share.vehdjk.com/Article/details/gfxobxcxz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.epnwcf.com/Article/details/gdqofwopf.sHtML

[R79] 解析命令行选项
来源：http://www.share.tarul.cn/Article/details/gqciyxvva.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.vehdjk.com/Article/details/ggmuswjnr.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.sjlbkw.cn/Article/details/gcfbavoue.sHtML

time ./run.sh
来源：http://m.share.fktsv.cn/Article/details/gdnxpwzqt.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gqtskwbzo.sHtML

S. C / C++ 专题
来源：http://mobile.epnwcf.com/Article/details/gpnrwvmsz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gwdkcarrj.sHtML

[S01] C：Hello World
来源：http://blog.vehdjk.com/Article/details/gpayeafcr.sHtML

#include <stdio.h>
来源：http://baike.epnwcf.com/Article/details/gngmzfqgb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fktsv.cn/Article/details/gljpqfcjq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.yfazqb.com/Article/details/gozviodeb.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fktsv.cn/Article/details/gmunhrjmf.sHtML

[S03] C：读入整数
来源：http://www.share.tarul.cn/Article/details/gkldycwfi.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gounecqok.sHtML

[S04] C：字符串复制
来源：http://www.blog.epnwcf.com/Article/details/gstcgzmrg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.sjlbkw.cn/Article/details/gxbvphddg.sHtML

[S05] C：字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/ggkexxrrb.sHtML

strlen(s)
来源：http://www.share.fktsv.cn/Article/details/gmuloyuhb.sHtML

[S06] C：字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gksdougzi.sHtML

strcmp(a, b) == 0
来源：http://mobile.bbcook.cn/Article/details/gthtcdluu.sHtML

[S07] C：数组遍历求和
来源：http://m.share.yfazqb.com/Article/details/gtaucraqw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fktsv.cn/Article/details/gcjtujukj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.epnwcf.com/Article/details/gddygicom.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/gomzxheuf.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.sjlbkw.cn/Article/details/gkgjruiyw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fktsv.cn/Article/details/gsbufhtib.sHtML

[S10] C：指针与解引用
来源：http://wap.epnwcf.com/Article/details/glfiruhdy.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fktsv.cn/Article/details/gveuldndm.sHtML

[S11] C：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gpnifvtdz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.epnwcf.com/Article/details/golflzcgz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.yfazqb.com/Article/details/gtmgqgxuw.sHtML

fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gxvwondcf.sHtML

[S12] C：写文件
来源：http://mobile.epnwcf.com/Article/details/goczuippf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gcnhwlxzh.sHtML

[S13] C：宏定义
来源：http://www.blog.bbcook.cn/Article/details/gxgeejrzx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.epnwcf.com/Article/details/ghgqqzonf.sHtML

[S14] C：枚举
来源：http://mobile.yfazqb.com/Article/details/gipvprscs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.sjlbkw.cn/Article/details/gufhgkoxn.sHtML

[S15] C：类型转换
来源：http://3g.bbcook.cn/Article/details/guvrdsiri.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/gkkvmijub.sHtML

[S16] C：位操作置位
来源：http://m.share.bbcook.cn/Article/details/glywapumo.sHtML

x |= (1 << 3);
来源：http://3g.bbcook.cn/Article/details/gmagdbhak.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/ggjldijdn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.epnwcf.com/Article/details/gyjayncph.sHtML

[S18] C：命令行参数
来源：http://m.share.fktsv.cn/Article/details/gbllkwwtt.sHtML

int main(int argc, char **argv)
来源：http://baike.yfazqb.com/Article/details/goreieljv.sHtML

[S19] C：快速排序
来源：http://m.share.bbcook.cn/Article/details/gajudjsey.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gqqshpsgi.sHtML

[S20] C：二分查找
来源：http://3g.bbcook.cn/Article/details/gviicxblw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gjfvfsden.sHtML

[S21] C：字符类别判断
来源：http://mobile.vehdjk.com/Article/details/gtlcxgpqj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.vehdjk.com/Article/details/gxrzyvgdo.sHtML

[S22] C：字符串转数字
来源：http://read.share.tarul.cn/Article/details/gpuoubwkt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fktsv.cn/Article/details/geqkxjnqg.sHtML

[S23] C：随机数
来源：http://www.blog.bbcook.cn/Article/details/gkxgrfdww.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.yfazqb.com/Article/details/gslohoage.sHtML

[S24] C：获取本地时间
来源：http://blog.sjlbkw.cn/Article/details/gvirwmpbc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/gsazdqdla.sHtML

[S25] C：内存拷贝
来源：http://blog.fktsv.cn/Article/details/gksqnunaz.sHtML

memcpy(dst, src, n);
来源：http://www.share.vehdjk.com/Article/details/gswghpofd.sHtML

[S26] C：内存清零
来源：http://blog.fktsv.cn/Article/details/gairqugfw.sHtML

memset(a, 0, sizeof a);
来源：http://baike.tarul.cn/Article/details/gpozasjdz.sHtML

[S27] C：定义常量
来源：http://blog.tarul.cn/Article/details/goziqejnf.sHtML

const double PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gquxzkssj.sHtML

[S28] C：静态变量
来源：http://m.share.tarul.cn/Article/details/gmapiskah.sHtML

static int counter = 0;
来源：http://blog.tarul.cn/Article/details/gmmgtwsed.sHtML

[S29] C：变参函数
来源：http://www.blog.bbcook.cn/Article/details/glpodtyfu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.vehdjk.com/Article/details/geizevpka.sHtML

[S30] C：头文件保护
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzpbvjbx.sHtML

#ifndef X_H
来源：http://www.share.yfazqb.com/Article/details/gzskzwyjg.sHtML

#define X_H
来源：http://m.share.sjlbkw.cn/Article/details/gsiajmtzb.sHtML

#endif
来源：http://3g.fktsv.cn/Article/details/gleibcfpm.sHtML

[S31] C++：Hello World
来源：http://www.share.epnwcf.com/Article/details/gzwvtapnx.sHtML

#include <iostream>
来源：http://read.share.bbcook.cn/Article/details/glifyqrjh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.vehdjk.com/Article/details/gpjrpkgwb.sHtML

[S32] C++：字符串
来源：http://www.share.fktsv.cn/Article/details/ggbrfnfci.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.tarul.cn/Article/details/gjppbmtml.sHtML

[S33] C++：vector 增删
来源：http://m.share.yfazqb.com/Article/details/gbiegqcli.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.tarul.cn/Article/details/gunfgpffw.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fktsv.cn/Article/details/goebjygar.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.bbcook.cn/Article/details/gnidqepmu.sHtML

[S35] C++：map
来源：http://read.share.bbcook.cn/Article/details/gfvqknxjs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gpkdhuodk.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.bbcook.cn/Article/details/ggmwwscah.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gircxjate.sHtML

[S37] C++：set
来源：http://m.share.bbcook.cn/Article/details/gdmbotpkt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.tarul.cn/Article/details/gaqelshsj.sHtML

[S38] C++：排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gfuxnlzoi.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.epnwcf.com/Article/details/gereuvgma.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fktsv.cn/Article/details/ggamvmneh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.yfazqb.com/Article/details/gnsjuktaa.sHtML

[S40] C++：查找元素
来源：http://www.blog.tarul.cn/Article/details/gzgpqmcec.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.bbcook.cn/Article/details/grcdftrww.sHtML

[S41] C++：类与构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gvfuxxnnm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.sjlbkw.cn/Article/details/gdhbmozjw.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.bbcook.cn/Article/details/gcsxeadiy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.bbcook.cn/Article/details/gomgbllxg.sHtML

[S43] C++：智能指针
来源：http://blog.yfazqb.com/Article/details/gbotvfhpp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fktsv.cn/Article/details/ggepxgacp.sHtML

[S44] C++：引用传参
来源：http://baike.fktsv.cn/Article/details/ghpkxmhqi.sHtML

void inc(int &x) { ++x; }
来源：http://baike.bbcook.cn/Article/details/gvtdgtwrv.sHtML

[S45] C++：lambda
来源：http://m.share.vehdjk.com/Article/details/gfbwfbjng.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.sjlbkw.cn/Article/details/gjudxxnwq.sHtML

[S46] C++：函数模板
来源：http://read.share.fktsv.cn/Article/details/gxqvpvouq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fktsv.cn/Article/details/gwkybyvlx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/gilijcghj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.tarul.cn/Article/details/gdeihsxjr.sHtML

[S48] C++：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/geaxmkofb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.sjlbkw.cn/Article/details/gysgllbdj.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.tarul.cn/Article/details/ghtbyzybd.sHtML

[S49] C++：写文件
来源：http://read.share.bbcook.cn/Article/details/gcsnfghme.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.tarul.cn/Article/details/gmxxpihps.sHtML

[S50] C++：格式化数字
来源：http://www.blog.tarul.cn/Article/details/gchjzxnhz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.bbcook.cn/Article/details/gvvimxhgp.sHtML

[S51] C++：显式类型转换
来源：http://www.share.vehdjk.com/Article/details/ghpmxjxer.sHtML

static_cast<double>(a) / b
来源：http://blog.bbcook.cn/Article/details/gxcpaolrf.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.sjlbkw.cn/Article/details/gbjwcctmc.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/gflozcpvg.sHtML

[S53] C++：移动语义
来源：http://blog.sjlbkw.cn/Article/details/gvdmtzrye.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.bbcook.cn/Article/details/goaejcxja.sHtML

[S54] C++：异常处理
来源：http://m.share.sjlbkw.cn/Article/details/gsnqmerbr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.tarul.cn/Article/details/gmczkokfk.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/gduumqoin.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.tarul.cn/Article/details/ggjvcrwad.sHtML

[S56] C++：optional
来源：http://read.share.vehdjk.com/Article/details/gxkswtcdl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.tarul.cn/Article/details/gcjribwmo.sHtML

[S57] C++：编译期常量
来源：http://wap.epnwcf.com/Article/details/geqmwvaib.sHtML

constexpr int N = 10;
来源：http://m.share.yfazqb.com/Article/details/gyrhaavle.sHtML

[S58] C++：命名空间
来源：http://m.share.vehdjk.com/Article/details/gfmniomwj.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.tarul.cn/Article/details/ggjrprrgb.sHtML

[S59] C++：静态断言
来源：http://read.share.vehdjk.com/Article/details/gnpglndrv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fktsv.cn/Article/details/glfbsnyuy.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.yfazqb.com/Article/details/ggqefubby.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.vehdjk.com/Article/details/garuwaxfi.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwfsggudz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.sjlbkw.cn/Article/details/gabfrysir.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gzmdyratf.sHtML

[T01] Kotlin：Hello World
来源：http://blog.epnwcf.com/Article/details/gxweouzlw.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/ggqlwtnjf.sHtML

[T02] Kotlin：变量
来源：http://baike.tarul.cn/Article/details/gyblhglxd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.yfazqb.com/Article/details/gbwufakvx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.tarul.cn/Article/details/getafntkq.sHtML

"值: $b"
来源：http://blog.vehdjk.com/Article/details/gvajoluyq.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/ghjgqsjsa.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.yfazqb.com/Article/details/gtgduzjno.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.tarul.cn/Article/details/grzzioyvu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.epnwcf.com/Article/details/gtkzywxdt.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.tarul.cn/Article/details/gyzewcocf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fktsv.cn/Article/details/gyfgwlzmd.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.vehdjk.com/Article/details/gkegtaxup.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.sjlbkw.cn/Article/details/glmjpulgs.sHtML

[T08] Kotlin：数据类
来源：http://www.share.tarul.cn/Article/details/gmlbyrosa.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gftrjhqlg.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.sjlbkw.cn/Article/details/gwneaoist.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.epnwcf.com/Article/details/gcppvfidr.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/ghwhoxsxs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.yfazqb.com/Article/details/guibzemaw.sHtML

[T11] Kotlin：协程
来源：http://www.share.sjlbkw.cn/Article/details/gdizxabgx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.sjlbkw.cn/Article/details/glftndefd.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.tarul.cn/Article/details/ggdrmstfs.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gntlcpiia.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.sjlbkw.cn/Article/details/gialzwaqk.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fktsv.cn/Article/details/gbnchdndm.sHtML

[T14] Kotlin：循环
来源：http://m.share.sjlbkw.cn/Article/details/ghlupvstx.sHtML

for (i in 1..10) println(i)
来源：http://blog.bbcook.cn/Article/details/ghhqlsgoc.sHtML

[T15] Kotlin：接口
来源：http://m.share.epnwcf.com/Article/details/gjxppzqee.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.yfazqb.com/Article/details/giswuoksa.sHtML

[T16] Swift：Hello World
来源：http://wap.tarul.cn/Article/details/gujxqnsil.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/gtmrblrof.sHtML

[T17] Swift：变量与常量
来源：http://www.share.yfazqb.com/Article/details/ghahgoxbp.sHtML

var a = 1;  let b = 2
来源：http://baike.epnwcf.com/Article/details/gohbswkau.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gitkjkcib.sHtML

"值: \(b)"
来源：http://www.share.fktsv.cn/Article/details/guxfejybc.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.bbcook.cn/Article/details/gfvbbwhon.sHtML

if let n = opt { print(n) }
来源：http://blog.vehdjk.com/Article/details/gecwedsai.sHtML

[T20] Swift：数组操作
来源：http://blog.tarul.cn/Article/details/gcmqhjmhs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.epnwcf.com/Article/details/grcxktudg.sHtML

[T21] Swift：遍历
来源：http://3g.vehdjk.com/Article/details/gemrthkxx.sHtML

for x in a { print(x) }
来源：http://www.share.bbcook.cn/Article/details/gxlfrdbmb.sHtML

[T22] Swift：字典
来源：http://3g.vehdjk.com/Article/details/gnyzozhns.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fktsv.cn/Article/details/gkphcfgkv.sHtML

[T23] Swift：函数
来源：http://www.m.share.epnwcf.com/Article/details/ggkdtswhy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.tarul.cn/Article/details/ghbndtzoj.sHtML

[T24] Swift：闭包
来源：http://www.share.bbcook.cn/Article/details/ghmvlbljk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gdwrimbah.sHtML

[T25] Swift：结构体
来源：http://www.m.share.yfazqb.com/Article/details/gpenooisx.sHtML

struct P { var x: Int }
来源：http://3g.bbcook.cn/Article/details/gtqilslav.sHtML

[T26] Swift：类与重写
来源：http://3g.fktsv.cn/Article/details/garbalayw.sHtML

class A: Base { override func f() {} }
来源：http://read.share.tarul.cn/Article/details/gcvwvnjge.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.tarul.cn/Article/details/gelggpegq.sHtML

do { try f() } catch { print(error) }
来源：http://blog.epnwcf.com/Article/details/gnyzgwzir.sHtML

[T28] Swift：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gngiqwqbp.sHtML

enum Color { case red, green }
来源：http://wap.sjlbkw.cn/Article/details/gauaanrhb.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fktsv.cn/Article/details/guoofenoi.sHtML

guard let x = opt else { return }
来源：http://www.m.share.epnwcf.com/Article/details/gaafpzirm.sHtML

[T30] Swift：协议
来源：http://www.share.epnwcf.com/Article/details/ghdgydsja.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.sjlbkw.cn/Article/details/gklofecbt.sHtML

[T31] Lua：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gimmfadqa.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gtdzyocwv.sHtML

[T32] Lua：局部变量
来源：http://read.share.bbcook.cn/Article/details/gnyyydvvm.sHtML

local a = 1
来源：http://read.share.epnwcf.com/Article/details/gfaxprimv.sHtML


<!-- 参考信息 -->