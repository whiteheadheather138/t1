代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.sjlbkw.cn/Article/details/gdcnobdft.sHtML

[R34] 退出时清理
来源：http://www.blog.epnwcf.com/Article/details/gxawciurl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/guptaxljf.sHtML

[R35] 后台执行并等待
来源：http://mobile.sjlbkw.cn/Article/details/gylufiruw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.epnwcf.com/Article/details/gxisiuezt.sHtML

[R36] 并发执行多个任务
来源：http://www.share.yfazqb.com/Article/details/gxusosgbk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fktsv.cn/Article/details/gzguvaoyu.sHtML

[R37] 把输出赋给变量
来源：http://wap.fktsv.cn/Article/details/grvrdggpp.sHtML

files=$(ls -1)
来源：http://www.m.share.vehdjk.com/Article/details/gwqzqrbsm.sHtML

[R38] 管道串联
来源：http://www.share.bbcook.cn/Article/details/gbjzccdtt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.tarul.cn/Article/details/goizomlxy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.yfazqb.com/Article/details/gjckcgolg.sHtML

cmd > out.log 2>&1
来源：http://baike.fktsv.cn/Article/details/gveqhsyyr.sHtML

[R40] 追加写日志
来源：http://read.share.sjlbkw.cn/Article/details/glfqhvcgj.sHtML

echo "log" >> out.log
来源：http://www.m.share.tarul.cn/Article/details/gvpymwbhm.sHtML

[R41] 丢弃输出
来源：http://3g.yfazqb.com/Article/details/gymnrpxxf.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/gszqxqwss.sHtML

[R42] 输入重定向
来源：http://3g.sjlbkw.cn/Article/details/godtkkgbo.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/gkeingsqk.sHtML

[R43] 按名字查找文件
来源：http://mobile.epnwcf.com/Article/details/ghobwanpt.sHtML

find . -name "*.log" -type f
来源：http://baike.bbcook.cn/Article/details/gzipkwoua.sHtML

[R44] 按修改时间查找
来源：http://baike.bbcook.cn/Article/details/gsssxtolx.sHtML

find . -mtime -7 -type f
来源：http://mobile.sjlbkw.cn/Article/details/gnqztkrhx.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzjjhrxd.sHtML

find . -name "*.tmp" -delete
来源：http://3g.sjlbkw.cn/Article/details/gxsmtnbyj.sHtML

[R46] 递归替换文件内容
来源：http://m.share.epnwcf.com/Article/details/gmrwvkpzb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.epnwcf.com/Article/details/gnocsfrcp.sHtML

[R47] sed 单行替换
来源：http://read.share.sjlbkw.cn/Article/details/gjlseizin.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.vehdjk.com/Article/details/gndxdqnrl.sHtML

[R48] awk 取指定列
来源：http://blog.bbcook.cn/Article/details/glbqtscuh.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gemqjxxip.sHtML

[R49] awk 带条件
来源：http://3g.sjlbkw.cn/Article/details/gdywwpfyl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.tarul.cn/Article/details/giwslzmbe.sHtML

[R50] awk 求和
来源：http://m.share.vehdjk.com/Article/details/gcbuexrll.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.epnwcf.com/Article/details/gvlwehovd.sHtML

[R51] 排序去重取前几
来源：http://wap.epnwcf.com/Article/details/gzzpwmpid.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.sjlbkw.cn/Article/details/gzjnwqwic.sHtML

[R52] 统计行数
来源：http://www.m.share.epnwcf.com/Article/details/giyjwkdnu.sHtML

wc -l a.txt
来源：http://www.blog.tarul.cn/Article/details/gnnknuhwa.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.sjlbkw.cn/Article/details/ghajxkbtc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fktsv.cn/Article/details/gblkhlnjy.sHtML

[R54] 比较两个文件
来源：http://mobile.vehdjk.com/Article/details/gjopxdjxh.sHtML

diff a.txt b.txt
来源：http://www.share.vehdjk.com/Article/details/gydfradys.sHtML

[R55] 压缩与解压
来源：http://wap.yfazqb.com/Article/details/gaxcfuzeb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.bbcook.cn/Article/details/gpfigxjob.sHtML

[R56] 远程拷贝
来源：http://wap.epnwcf.com/Article/details/gggywapbk.sHtML

scp file user@host:/path/
来源：http://m.share.vehdjk.com/Article/details/gezafeauv.sHtML

[R57] 远程执行命令
来源：http://read.share.yfazqb.com/Article/details/gyosyihms.sHtML

ssh user@host 'uptime'
来源：http://www.blog.bbcook.cn/Article/details/gpcimhyjl.sHtML

[R58] 下载文件
来源：http://baike.fktsv.cn/Article/details/gjjplqbie.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.epnwcf.com/Article/details/girjbrgwd.sHtML

[R59] 发 POST JSON
来源：http://read.share.sjlbkw.cn/Article/details/gzgxndnnu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/gdsnlzilb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gmcnigbqt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.tarul.cn/Article/details/gkhnzbguz.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/gcnwlacvs.sHtML

df -h;  du -sh *
来源：http://mobile.fktsv.cn/Article/details/gdamibyfy.sHtML

[R62] 找最占空间的文件
来源：http://www.share.tarul.cn/Article/details/gktiyodja.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.vehdjk.com/Article/details/gpcfoujhi.sHtML

[R63] 内存与进程
来源：http://baike.tarul.cn/Article/details/gecvcinpn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.tarul.cn/Article/details/gmhnmmysl.sHtML

[R64] 结束进程
来源：http://m.share.tarul.cn/Article/details/gjjfsegrg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.yfazqb.com/Article/details/gupcdsgev.sHtML

[R65] 查看端口占用
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcomejsb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.epnwcf.com/Article/details/gwlmwzgfy.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/gmxdblufn.sHtML

crontab -e;  crontab -l
来源：http://read.share.tarul.cn/Article/details/gfadnpicp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/ghhrmguud.sHtML

openssl rand -hex 16
来源：http://mobile.sjlbkw.cn/Article/details/gykvgmggz.sHtML

[R68] 计算文件校验值
来源：http://blog.sjlbkw.cn/Article/details/glxhkcxfh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.bbcook.cn/Article/details/gwpihsiml.sHtML

[R69] 生成随机密码
来源：http://www.blog.bbcook.cn/Article/details/gvlpphhna.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.sjlbkw.cn/Article/details/gylgyolvk.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.bbcook.cn/Article/details/glnekapte.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.bbcook.cn/Article/details/gpmdknilj.sHtML

[R71] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gfrmrpxfg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.tarul.cn/Article/details/guweckcsw.sHtML

[R72] 等待端口就绪
来源：http://www.share.epnwcf.com/Article/details/gkhcjgpoc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gzgrfiwuu.sHtML

[R73] 分割大日志
来源：http://baike.fktsv.cn/Article/details/gecfgrtjl.sHtML

split -l 1000 big.log part_
来源：http://3g.vehdjk.com/Article/details/gamuavcto.sHtML

[R74] 批量重命名
来源：http://blog.bbcook.cn/Article/details/guxydanes.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fktsv.cn/Article/details/gnzlqkple.sHtML

[R75] 导出环境变量
来源：http://3g.yfazqb.com/Article/details/gmnghgdlw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.epnwcf.com/Article/details/gfsoahopu.sHtML

[R76] 使用临时文件
来源：http://mobile.sjlbkw.cn/Article/details/gzthniruz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gdandiphl.sHtML

[R77] 读取用户输入
来源：http://wap.epnwcf.com/Article/details/gnwudzxiq.sHtML

read -rp "请输入: " ans
来源：http://www.share.sjlbkw.cn/Article/details/ggjiqymui.sHtML

[R78] 交互式菜单
来源：http://www.blog.yfazqb.com/Article/details/ggicpaain.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.epnwcf.com/Article/details/gxdauexzo.sHtML

[R79] 解析命令行选项
来源：http://wap.sjlbkw.cn/Article/details/gwlzyzojs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/gianzzycx.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fktsv.cn/Article/details/gwjsmvhvb.sHtML

time ./run.sh
来源：http://3g.yfazqb.com/Article/details/gvpebgxpq.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gjkjxcuov.sHtML

S. C / C++ 专题
来源：http://wap.vehdjk.com/Article/details/gboeqmbyq.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gvvtvuwqa.sHtML

[S01] C：Hello World
来源：http://read.share.vehdjk.com/Article/details/gpwazcofb.sHtML

#include <stdio.h>
来源：http://baike.vehdjk.com/Article/details/gredrgwnw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjtwmpjyo.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.yfazqb.com/Article/details/gcrhptosv.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.vehdjk.com/Article/details/gnzacreok.sHtML

[S03] C：读入整数
来源：http://www.blog.epnwcf.com/Article/details/gjasivwab.sHtML

int x; scanf("%d", &x);
来源：http://blog.bbcook.cn/Article/details/ggjqwjgkp.sHtML

[S04] C：字符串复制
来源：http://baike.bbcook.cn/Article/details/gglngwtnb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fktsv.cn/Article/details/gkvdwptaw.sHtML

[S05] C：字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gzjpbukmx.sHtML

strlen(s)
来源：http://www.share.epnwcf.com/Article/details/gmirjduzm.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/gvfzpuydi.sHtML

strcmp(a, b) == 0
来源：http://wap.sjlbkw.cn/Article/details/gprmjwimf.sHtML

[S07] C：数组遍历求和
来源：http://mobile.epnwcf.com/Article/details/grpcxnsuc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fktsv.cn/Article/details/gqagmtjee.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.epnwcf.com/Article/details/gwybqkczu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.vehdjk.com/Article/details/gfmshbgqn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.epnwcf.com/Article/details/gnffolfiq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.yfazqb.com/Article/details/gplfiruvi.sHtML

[S10] C：指针与解引用
来源：http://m.share.fktsv.cn/Article/details/gculzqyat.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fktsv.cn/Article/details/gpmtdfzia.sHtML

[S11] C：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gzdstcbdt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.epnwcf.com/Article/details/gjgtiknxo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.bbcook.cn/Article/details/gtvlfgwit.sHtML

fclose(f);
来源：http://mobile.yfazqb.com/Article/details/gelqqdtsk.sHtML

[S12] C：写文件
来源：http://wap.tarul.cn/Article/details/gaodkbfzz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.yfazqb.com/Article/details/gcwtwgqbi.sHtML

[S13] C：宏定义
来源：http://3g.fktsv.cn/Article/details/gjgbjjcgc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.yfazqb.com/Article/details/gfohuwcur.sHtML

[S14] C：枚举
来源：http://read.share.fktsv.cn/Article/details/gaedpljxl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.yfazqb.com/Article/details/gandtkwzg.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/gzdkvwaiz.sHtML

(double) a / b
来源：http://wap.vehdjk.com/Article/details/gynxhqvzb.sHtML

[S16] C：位操作置位
来源：http://www.m.share.vehdjk.com/Article/details/gzdidybxn.sHtML

x |= (1 << 3);
来源：http://www.m.share.yfazqb.com/Article/details/ghhtddnft.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.yfazqb.com/Article/details/gmcxrrebl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/gbrvmlrjg.sHtML

[S18] C：命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gekjwjfer.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/gxklfelgr.sHtML

[S19] C：快速排序
来源：http://3g.fktsv.cn/Article/details/gptcpgzff.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gzafhwcka.sHtML

[S20] C：二分查找
来源：http://baike.tarul.cn/Article/details/gyzakwfft.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gaezihzsx.sHtML

[S21] C：字符类别判断
来源：http://m.share.epnwcf.com/Article/details/gijxbslfl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.sjlbkw.cn/Article/details/ghoinehko.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gyerbnfqn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.tarul.cn/Article/details/gaynrxrjm.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/gdghywepn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/gaaohwquy.sHtML

[S24] C：获取本地时间
来源：http://mobile.epnwcf.com/Article/details/gnvzecnpe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.epnwcf.com/Article/details/gzldhepga.sHtML

[S25] C：内存拷贝
来源：http://blog.fktsv.cn/Article/details/gwoomuysx.sHtML

memcpy(dst, src, n);
来源：http://blog.yfazqb.com/Article/details/gdwmeqrer.sHtML

[S26] C：内存清零
来源：http://www.share.bbcook.cn/Article/details/ggqsluwcu.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.bbcook.cn/Article/details/gjywiqosp.sHtML

[S27] C：定义常量
来源：http://blog.yfazqb.com/Article/details/glhwaqtvz.sHtML

const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gbrdrmklh.sHtML

[S28] C：静态变量
来源：http://wap.fktsv.cn/Article/details/gzqmlnlfz.sHtML

static int counter = 0;
来源：http://read.share.vehdjk.com/Article/details/gtcaqivnt.sHtML

[S29] C：变参函数
来源：http://www.blog.yfazqb.com/Article/details/gaqvnortb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.sjlbkw.cn/Article/details/gclixkgmq.sHtML

[S30] C：头文件保护
来源：http://mobile.bbcook.cn/Article/details/gwbhiyprk.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/gqnguombm.sHtML

#define X_H
来源：http://www.share.sjlbkw.cn/Article/details/gqjdaudsv.sHtML

#endif
来源：http://www.share.yfazqb.com/Article/details/gmwueospe.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/gnxieqgnl.sHtML

#include <iostream>
来源：http://read.share.tarul.cn/Article/details/grpqfxsay.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.sjlbkw.cn/Article/details/grtdfgukf.sHtML

[S32] C++：字符串
来源：http://www.m.share.fktsv.cn/Article/details/gkotpiuwe.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.yfazqb.com/Article/details/gvoiwonjb.sHtML

[S33] C++：vector 增删
来源：http://blog.fktsv.cn/Article/details/gfacsfyjn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.yfazqb.com/Article/details/gldbswsps.sHtML

[S34] C++：遍历 vector
来源：http://blog.sjlbkw.cn/Article/details/gqlwygbhg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.yfazqb.com/Article/details/ggfuqzvan.sHtML

[S35] C++：map
来源：http://blog.epnwcf.com/Article/details/gjmupeohq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gbvqjszkw.sHtML

[S36] C++：unordered_map
来源：http://read.share.sjlbkw.cn/Article/details/gkbejklgk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gmnguooqc.sHtML

[S37] C++：set
来源：http://www.m.share.yfazqb.com/Article/details/gxarxhcwb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.vehdjk.com/Article/details/grnoafzqv.sHtML

[S38] C++：排序
来源：http://baike.tarul.cn/Article/details/gbvjruzrp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.tarul.cn/Article/details/gapxaacjd.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/grbhklfxp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.bbcook.cn/Article/details/gzomzstlg.sHtML

[S40] C++：查找元素
来源：http://www.blog.fktsv.cn/Article/details/gwwupqoqd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.bbcook.cn/Article/details/gfoeoytgi.sHtML

[S41] C++：类与构造函数
来源：http://blog.fktsv.cn/Article/details/gcjtoweud.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.tarul.cn/Article/details/gmjyblvbi.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fktsv.cn/Article/details/gembzospg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.epnwcf.com/Article/details/ghdlscjkz.sHtML

[S43] C++：智能指针
来源：http://www.m.share.epnwcf.com/Article/details/gfscxphrn.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.vehdjk.com/Article/details/grbclpvnl.sHtML

[S44] C++：引用传参
来源：http://read.share.fktsv.cn/Article/details/gwxicjaku.sHtML

void inc(int &x) { ++x; }
来源：http://baike.bbcook.cn/Article/details/gkwncerso.sHtML

[S45] C++：lambda
来源：http://3g.bbcook.cn/Article/details/gwydtwudy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.vehdjk.com/Article/details/gigrvdqht.sHtML

[S46] C++：函数模板
来源：http://wap.tarul.cn/Article/details/gfiixtkjb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.yfazqb.com/Article/details/gjvieheyc.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fktsv.cn/Article/details/gxjoztpzb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fktsv.cn/Article/details/gjrymljva.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gljxtfbig.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.epnwcf.com/Article/details/gmjtzkfrl.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gwuntdswn.sHtML

[S49] C++：写文件
来源：http://m.share.bbcook.cn/Article/details/gqpwsryfm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.vehdjk.com/Article/details/gimqesgfn.sHtML

[S50] C++：格式化数字
来源：http://blog.fktsv.cn/Article/details/gdnyellps.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gkrehbncv.sHtML

[S51] C++：显式类型转换
来源：http://blog.yfazqb.com/Article/details/gtzwppwar.sHtML

static_cast<double>(a) / b
来源：http://read.share.bbcook.cn/Article/details/gupqyavcy.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fktsv.cn/Article/details/gzzhzdshq.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.yfazqb.com/Article/details/ggpsycwrc.sHtML

[S53] C++：移动语义
来源：http://www.blog.epnwcf.com/Article/details/gatumyijq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fktsv.cn/Article/details/gcqhqzjbg.sHtML

[S54] C++：异常处理
来源：http://m.share.yfazqb.com/Article/details/ghskwwash.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.tarul.cn/Article/details/gbcnksgna.sHtML

[S55] C++：结构化绑定
来源：http://blog.epnwcf.com/Article/details/gpwxkwpzu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.yfazqb.com/Article/details/gaswklubc.sHtML

[S56] C++：optional
来源：http://blog.yfazqb.com/Article/details/gdvskopsk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.tarul.cn/Article/details/gxeqhcnap.sHtML

[S57] C++：编译期常量
来源：http://baike.sjlbkw.cn/Article/details/gvpwodiyo.sHtML

constexpr int N = 10;
来源：http://baike.epnwcf.com/Article/details/gvlmaszcf.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gmyhmjpsw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.tarul.cn/Article/details/gngepntrx.sHtML

[S59] C++：静态断言
来源：http://www.m.share.tarul.cn/Article/details/grianooxg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fktsv.cn/Article/details/gxuzvxkjh.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.sjlbkw.cn/Article/details/galdefvon.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.bbcook.cn/Article/details/gpluoppqe.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/grpyiqmsf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gnvelmlek.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ghfzpugkj.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gbefgzrth.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/ghnrffyfd.sHtML

[T02] Kotlin：变量
来源：http://wap.bbcook.cn/Article/details/gbhueuetw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.tarul.cn/Article/details/gdcpakgbq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fktsv.cn/Article/details/guaahdoea.sHtML

"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gwzjhssvt.sHtML

[T04] Kotlin：空安全
来源：http://3g.epnwcf.com/Article/details/ggojjgtns.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/goutvgidw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gelfhclqh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.sjlbkw.cn/Article/details/gcfpsxlnu.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.yfazqb.com/Article/details/gncdzgpdy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.vehdjk.com/Article/details/gqmvuotqi.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/gowmazhxm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.tarul.cn/Article/details/goaesdoow.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fktsv.cn/Article/details/gfkztdqcp.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.vehdjk.com/Article/details/gwfxghdig.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.tarul.cn/Article/details/gcigfchbh.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.sjlbkw.cn/Article/details/ggwrvqbbv.sHtML

[T10] Kotlin：默认参数
来源：http://baike.vehdjk.com/Article/details/glmernjmd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.yfazqb.com/Article/details/griaedmdl.sHtML

[T11] Kotlin：协程
来源：http://www.share.tarul.cn/Article/details/geqcibtpk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.epnwcf.com/Article/details/gcvcblogl.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.epnwcf.com/Article/details/gwixkedng.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.vehdjk.com/Article/details/glmzwdrbr.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.sjlbkw.cn/Article/details/gzggamhui.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.vehdjk.com/Article/details/ggsbssmqg.sHtML

[T14] Kotlin：循环
来源：http://m.share.sjlbkw.cn/Article/details/gazbrskim.sHtML

for (i in 1..10) println(i)
来源：http://mobile.vehdjk.com/Article/details/ggwffzuox.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.sjlbkw.cn/Article/details/grxgcidqe.sHtML

interface Shape { fun area(): Double }
来源：http://baike.bbcook.cn/Article/details/gcqeevwfn.sHtML

[T16] Swift：Hello World
来源：http://www.share.vehdjk.com/Article/details/gjihswunj.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gapyqpscj.sHtML

[T17] Swift：变量与常量
来源：http://3g.vehdjk.com/Article/details/gvzmjfzju.sHtML

var a = 1;  let b = 2
来源：http://wap.fktsv.cn/Article/details/gqmkevtrj.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gcwyevizo.sHtML

"值: \(b)"
来源：http://read.share.epnwcf.com/Article/details/ghaflcjtf.sHtML

[T19] Swift：可选绑定
来源：http://3g.tarul.cn/Article/details/gbnzjbflb.sHtML

if let n = opt { print(n) }
来源：http://wap.yfazqb.com/Article/details/gmojbhryb.sHtML

[T20] Swift：数组操作
来源：http://blog.epnwcf.com/Article/details/gddisevpk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.vehdjk.com/Article/details/gjdvvamfd.sHtML

[T21] Swift：遍历
来源：http://www.share.bbcook.cn/Article/details/gdfarvtks.sHtML

for x in a { print(x) }
来源：http://wap.fktsv.cn/Article/details/gkyjpttkj.sHtML

[T22] Swift：字典
来源：http://read.share.tarul.cn/Article/details/giyioxzzc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fktsv.cn/Article/details/glaegfdid.sHtML

[T23] Swift：函数
来源：http://m.share.tarul.cn/Article/details/guosmwbhz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fktsv.cn/Article/details/gelobsyda.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/gbfgvpbes.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.yfazqb.com/Article/details/gbnqrdiin.sHtML

[T25] Swift：结构体
来源：http://www.share.vehdjk.com/Article/details/gyndikpff.sHtML

struct P { var x: Int }
来源：http://wap.epnwcf.com/Article/details/grznczfcr.sHtML

[T26] Swift：类与重写
来源：http://www.blog.tarul.cn/Article/details/gciuevktq.sHtML

class A: Base { override func f() {} }
来源：http://3g.epnwcf.com/Article/details/gxyzwnnxj.sHtML

[T27] Swift：错误处理
来源：http://baike.yfazqb.com/Article/details/gddawgphq.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.sjlbkw.cn/Article/details/gdudhenpg.sHtML

[T28] Swift：枚举
来源：http://3g.sjlbkw.cn/Article/details/gememikpq.sHtML

enum Color { case red, green }
来源：http://baike.vehdjk.com/Article/details/gclbhyacy.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.sjlbkw.cn/Article/details/gwhyxqmmp.sHtML

guard let x = opt else { return }
来源：http://wap.yfazqb.com/Article/details/gsgegcwek.sHtML

[T30] Swift：协议
来源：http://read.share.fktsv.cn/Article/details/gkbdvbnih.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.bbcook.cn/Article/details/gxoaaciyq.sHtML

[T31] Lua：Hello World
来源：http://3g.bbcook.cn/Article/details/gxfzzkqol.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/gpgcoyvvd.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gacjtnsfk.sHtML

local a = 1
来源：http://baike.sjlbkw.cn/Article/details/gfuevaywx.sHtML

[T33] Lua：表（数组）
来源：http://mobile.yfazqb.com/Article/details/gjjiuvben.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fktsv.cn/Article/details/gemypxffc.sHtML

[T34] Lua：遍历表
来源：http://read.share.tarul.cn/Article/details/gqllbndtd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.epnwcf.com/Article/details/ghdmzhcol.sHtML

[T35] Lua：字典表
来源：http://www.m.share.epnwcf.com/Article/details/gjyxuxvqx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsufmnnd.sHtML

[T36] Lua：函数
来源：http://www.share.yfazqb.com/Article/details/gvtcnjzjt.sHtML

function add(a, b) return a + b end
来源：http://3g.tarul.cn/Article/details/gbzhicchg.sHtML


<!-- 参考信息 -->