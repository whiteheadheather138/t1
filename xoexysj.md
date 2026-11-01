代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.yfazqb.com/Article/details/gmutvndub.sHtML

[R34] 退出时清理
来源：http://m.share.tarul.cn/Article/details/gbciaeocf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gsmdfolol.sHtML

[R35] 后台执行并等待
来源：http://wap.tarul.cn/Article/details/gnfotfhzv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.sjlbkw.cn/Article/details/gxeoatqeg.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.bbcook.cn/Article/details/grvpmdyxs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.epnwcf.com/Article/details/gxahnbhhl.sHtML

[R37] 把输出赋给变量
来源：http://blog.bbcook.cn/Article/details/gowqpzlyy.sHtML

files=$(ls -1)
来源：http://m.share.vehdjk.com/Article/details/gkscojvyg.sHtML

[R38] 管道串联
来源：http://www.blog.yfazqb.com/Article/details/gamauxeoy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fktsv.cn/Article/details/gcmnenkfb.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fktsv.cn/Article/details/gdlcrrzgm.sHtML

cmd > out.log 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gkyxnecdr.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/gvfcqhegd.sHtML

echo "log" >> out.log
来源：http://baike.fktsv.cn/Article/details/gzpsrxkqv.sHtML

[R41] 丢弃输出
来源：http://wap.yfazqb.com/Article/details/gnteamooe.sHtML

cmd >/dev/null 2>&1
来源：http://blog.bbcook.cn/Article/details/gahdunmge.sHtML

[R42] 输入重定向
来源：http://www.m.share.epnwcf.com/Article/details/ghpzolnuw.sHtML

wc -l < a.txt
来源：http://wap.sjlbkw.cn/Article/details/gvikvclvy.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fktsv.cn/Article/details/gdgtfysxa.sHtML

find . -name "*.log" -type f
来源：http://read.share.sjlbkw.cn/Article/details/gqitaqtoz.sHtML

[R44] 按修改时间查找
来源：http://blog.fktsv.cn/Article/details/gbctyiyqq.sHtML

find . -mtime -7 -type f
来源：http://3g.tarul.cn/Article/details/gogwaykmj.sHtML

[R45] 批量删除
来源：http://m.share.epnwcf.com/Article/details/gugvrqcds.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/gpgehnpyj.sHtML

[R46] 递归替换文件内容
来源：http://wap.sjlbkw.cn/Article/details/geemmfbzw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.tarul.cn/Article/details/gvpuiftsi.sHtML

[R47] sed 单行替换
来源：http://baike.yfazqb.com/Article/details/ghptmjgrp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.vehdjk.com/Article/details/gbtqgtpyx.sHtML

[R48] awk 取指定列
来源：http://baike.bbcook.cn/Article/details/gwwmstitl.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.vehdjk.com/Article/details/gnvxijuod.sHtML

[R49] awk 带条件
来源：http://baike.tarul.cn/Article/details/gzqionpyb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.sjlbkw.cn/Article/details/gjxbohxeg.sHtML

[R50] awk 求和
来源：http://www.blog.bbcook.cn/Article/details/gcazxhzfn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gsxcopuqi.sHtML

[R51] 排序去重取前几
来源：http://baike.bbcook.cn/Article/details/gblabqrct.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fktsv.cn/Article/details/gpsimgutl.sHtML

[R52] 统计行数
来源：http://3g.vehdjk.com/Article/details/gqklmexew.sHtML

wc -l a.txt
来源：http://m.share.vehdjk.com/Article/details/gafrjkhzu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.sjlbkw.cn/Article/details/gkupagpgm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.vehdjk.com/Article/details/gftahbbws.sHtML

[R54] 比较两个文件
来源：http://read.share.sjlbkw.cn/Article/details/gjkhenkgw.sHtML

diff a.txt b.txt
来源：http://wap.tarul.cn/Article/details/gogyeyhcb.sHtML

[R55] 压缩与解压
来源：http://wap.bbcook.cn/Article/details/greyniqtr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.vehdjk.com/Article/details/gbbzuxnaj.sHtML

[R56] 远程拷贝
来源：http://mobile.vehdjk.com/Article/details/gwtzhsysg.sHtML

scp file user@host:/path/
来源：http://m.share.tarul.cn/Article/details/gtfptavpq.sHtML

[R57] 远程执行命令
来源：http://3g.tarul.cn/Article/details/gaixgmsat.sHtML

ssh user@host 'uptime'
来源：http://3g.epnwcf.com/Article/details/gpooxbubl.sHtML

[R58] 下载文件
来源：http://3g.yfazqb.com/Article/details/golrvorog.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/ggrisqrdu.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/grijihvyf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.epnwcf.com/Article/details/gavgmerdi.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/gqmamlhbp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.sjlbkw.cn/Article/details/gjnwqebch.sHtML

[R61] 磁盘占用
来源：http://read.share.bbcook.cn/Article/details/gvtvykpul.sHtML

df -h;  du -sh *
来源：http://www.share.fktsv.cn/Article/details/gxxdigzxr.sHtML

[R62] 找最占空间的文件
来源：http://read.share.vehdjk.com/Article/details/gyihelvsk.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.vehdjk.com/Article/details/gvcnwpqag.sHtML

[R63] 内存与进程
来源：http://wap.sjlbkw.cn/Article/details/glmzgoyxp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fktsv.cn/Article/details/gaxcvdyqp.sHtML

[R64] 结束进程
来源：http://www.share.bbcook.cn/Article/details/gpbtawzao.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.sjlbkw.cn/Article/details/giyqmzzve.sHtML

[R65] 查看端口占用
来源：http://read.share.yfazqb.com/Article/details/gfhhcughc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fktsv.cn/Article/details/gbnuvhgcy.sHtML

[R66] 定时任务
来源：http://read.share.tarul.cn/Article/details/guenjiyij.sHtML

crontab -e;  crontab -l
来源：http://www.share.tarul.cn/Article/details/gryfbrujw.sHtML

[R67] 生成随机十六进制串
来源：http://3g.yfazqb.com/Article/details/gqkvjchjq.sHtML

openssl rand -hex 16
来源：http://www.m.share.epnwcf.com/Article/details/gfghsmsnv.sHtML

[R68] 计算文件校验值
来源：http://mobile.vehdjk.com/Article/details/gbgbimavl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fktsv.cn/Article/details/gzduxgfhh.sHtML

[R69] 生成随机密码
来源：http://3g.epnwcf.com/Article/details/ggljsfzpu.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.sjlbkw.cn/Article/details/ggqhfhuux.sHtML

[R70] 时间戳与互转
来源：http://blog.tarul.cn/Article/details/gusftksci.sHtML

date +%s;  date -d @1700000000
来源：http://wap.yfazqb.com/Article/details/gxkfqzfil.sHtML

[R71] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gclubywgy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.sjlbkw.cn/Article/details/gbflawizd.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gjpuoqlsz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gzyrpfbgh.sHtML

[R73] 分割大日志
来源：http://www.m.share.bbcook.cn/Article/details/giepogbzn.sHtML

split -l 1000 big.log part_
来源：http://baike.tarul.cn/Article/details/gmthrmtix.sHtML

[R74] 批量重命名
来源：http://m.share.fktsv.cn/Article/details/gjlentvkk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.epnwcf.com/Article/details/gjetfyspa.sHtML

[R75] 导出环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gzxvkhecy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fktsv.cn/Article/details/gqydqvwon.sHtML

[R76] 使用临时文件
来源：http://read.share.yfazqb.com/Article/details/gonehsafo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsxhyafn.sHtML

[R77] 读取用户输入
来源：http://www.blog.sjlbkw.cn/Article/details/gifqwdvrk.sHtML

read -rp "请输入: " ans
来源：http://mobile.fktsv.cn/Article/details/gktgucgkv.sHtML

[R78] 交互式菜单
来源：http://www.share.tarul.cn/Article/details/gaptfhunh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fktsv.cn/Article/details/gptthkxso.sHtML

[R79] 解析命令行选项
来源：http://read.share.fktsv.cn/Article/details/gfwyppoxp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fktsv.cn/Article/details/gadgvytpo.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.epnwcf.com/Article/details/gvdztpujs.sHtML

time ./run.sh
来源：http://mobile.bbcook.cn/Article/details/gncmnvajg.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbbcgpkfa.sHtML

S. C / C++ 专题
来源：http://3g.tarul.cn/Article/details/givvdcibs.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gyaqxqzjh.sHtML

[S01] C：Hello World
来源：http://wap.yfazqb.com/Article/details/gfhonffjs.sHtML

#include <stdio.h>
来源：http://3g.vehdjk.com/Article/details/givgphegz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fktsv.cn/Article/details/gjcdcmcoc.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.epnwcf.com/Article/details/gijhplzrc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.bbcook.cn/Article/details/gqtjsecyf.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/gmioioiku.sHtML

int x; scanf("%d", &x);
来源：http://www.share.yfazqb.com/Article/details/giuqipfon.sHtML

[S04] C：字符串复制
来源：http://m.share.epnwcf.com/Article/details/gjdaoraki.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.epnwcf.com/Article/details/gejwtntct.sHtML

[S05] C：字符串长度
来源：http://www.share.bbcook.cn/Article/details/gpkthfxza.sHtML

strlen(s)
来源：http://baike.epnwcf.com/Article/details/gzggudzky.sHtML

[S06] C：字符串比较
来源：http://read.share.epnwcf.com/Article/details/gigurpnyx.sHtML

strcmp(a, b) == 0
来源：http://wap.sjlbkw.cn/Article/details/gfhjctmut.sHtML

[S07] C：数组遍历求和
来源：http://read.share.tarul.cn/Article/details/gehepcctc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.tarul.cn/Article/details/gklgrgkfr.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.epnwcf.com/Article/details/gowbijxub.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.tarul.cn/Article/details/gvkqvubjz.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fktsv.cn/Article/details/gicaesmna.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.yfazqb.com/Article/details/gbvxetjxn.sHtML

[S10] C：指针与解引用
来源：http://blog.sjlbkw.cn/Article/details/gqupddkfz.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.yfazqb.com/Article/details/gkdhjiyuu.sHtML

[S11] C：逐行读文件
来源：http://read.share.tarul.cn/Article/details/gyyyixsep.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.tarul.cn/Article/details/ghwnakwth.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.vehdjk.com/Article/details/geltgpudq.sHtML

fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/gcrdktthu.sHtML

[S12] C：写文件
来源：http://baike.yfazqb.com/Article/details/gkzgzznir.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.yfazqb.com/Article/details/gcsukfipc.sHtML

[S13] C：宏定义
来源：http://blog.yfazqb.com/Article/details/geefoijhk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/gmkkhaodi.sHtML

[S14] C：枚举
来源：http://wap.yfazqb.com/Article/details/gnevvuzlj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fktsv.cn/Article/details/glemmcwao.sHtML

[S15] C：类型转换
来源：http://blog.tarul.cn/Article/details/ggmvnklea.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcpxgtrq.sHtML

[S16] C：位操作置位
来源：http://read.share.vehdjk.com/Article/details/gddjhpwaj.sHtML

x |= (1 << 3);
来源：http://www.m.share.epnwcf.com/Article/details/gcbnlpnwo.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gorthjxvl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.vehdjk.com/Article/details/geokobeex.sHtML

[S18] C：命令行参数
来源：http://3g.fktsv.cn/Article/details/gsnwxybcy.sHtML

int main(int argc, char **argv)
来源：http://m.share.tarul.cn/Article/details/gvfypalal.sHtML

[S19] C：快速排序
来源：http://baike.fktsv.cn/Article/details/glsxlqzkl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gezqnoohc.sHtML

[S20] C：二分查找
来源：http://blog.vehdjk.com/Article/details/gxyvomhph.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gbxvmgbgx.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.vehdjk.com/Article/details/gnitzkjqr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.yfazqb.com/Article/details/gnfltbexa.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gknriddua.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.bbcook.cn/Article/details/glhauqwwr.sHtML

[S23] C：随机数
来源：http://www.share.vehdjk.com/Article/details/gsopjuyqw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.vehdjk.com/Article/details/gmgqyjxdm.sHtML

[S24] C：获取本地时间
来源：http://3g.fktsv.cn/Article/details/gkgnbtlbg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.epnwcf.com/Article/details/gcnybhsng.sHtML

[S25] C：内存拷贝
来源：http://m.share.tarul.cn/Article/details/gpjosnssu.sHtML

memcpy(dst, src, n);
来源：http://m.share.bbcook.cn/Article/details/gnqzondst.sHtML

[S26] C：内存清零
来源：http://m.share.bbcook.cn/Article/details/gvjyipzhj.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.vehdjk.com/Article/details/gkpfhqkca.sHtML

[S27] C：定义常量
来源：http://mobile.vehdjk.com/Article/details/gdsyfpafu.sHtML

const double PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gmvikjzxm.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/gqvtayhad.sHtML

static int counter = 0;
来源：http://www.share.tarul.cn/Article/details/gwwjvbeja.sHtML

[S29] C：变参函数
来源：http://blog.tarul.cn/Article/details/ghaerycca.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.bbcook.cn/Article/details/gyzwplscv.sHtML

[S30] C：头文件保护
来源：http://wap.fktsv.cn/Article/details/gxrfeqcgn.sHtML

#ifndef X_H
来源：http://wap.vehdjk.com/Article/details/gyatenvyn.sHtML

#define X_H
来源：http://blog.bbcook.cn/Article/details/gvbelduku.sHtML

#endif
来源：http://mobile.epnwcf.com/Article/details/gtxhywgmo.sHtML

[S31] C++：Hello World
来源：http://3g.vehdjk.com/Article/details/gyifxnasv.sHtML

#include <iostream>
来源：http://wap.epnwcf.com/Article/details/ggujtpbdm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.vehdjk.com/Article/details/gypditqol.sHtML

[S32] C++：字符串
来源：http://m.share.tarul.cn/Article/details/ggqvpnwux.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.sjlbkw.cn/Article/details/gykjphlci.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.yfazqb.com/Article/details/gdskivjbz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.bbcook.cn/Article/details/gmdapfbff.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.epnwcf.com/Article/details/gkbitbgnz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.tarul.cn/Article/details/gvikcjzbr.sHtML

[S35] C++：map
来源：http://www.m.share.yfazqb.com/Article/details/gyvdrjhkg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gsfukxyud.sHtML

[S36] C++：unordered_map
来源：http://3g.fktsv.cn/Article/details/ghuniwris.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gissfzisk.sHtML

[S37] C++：set
来源：http://3g.sjlbkw.cn/Article/details/geekzgcya.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fktsv.cn/Article/details/gpopmstkc.sHtML

[S38] C++：排序
来源：http://www.share.yfazqb.com/Article/details/ghathuxes.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.epnwcf.com/Article/details/gvyasxlyo.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/gqtorkpzq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.epnwcf.com/Article/details/goaogczmt.sHtML

[S40] C++：查找元素
来源：http://www.share.sjlbkw.cn/Article/details/gwokergny.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fktsv.cn/Article/details/gjknbqejg.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gtoajsppq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.tarul.cn/Article/details/grnfikhxu.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.sjlbkw.cn/Article/details/geoyzjzcy.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.sjlbkw.cn/Article/details/gdbzczxwe.sHtML

[S43] C++：智能指针
来源：http://m.share.bbcook.cn/Article/details/gbdimzvlq.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/gepjlwneq.sHtML

[S44] C++：引用传参
来源：http://www.share.yfazqb.com/Article/details/gdwymyjdg.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.vehdjk.com/Article/details/gksutuxtg.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gfwsyvzvj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/gqyigawse.sHtML

[S46] C++：函数模板
来源：http://blog.fktsv.cn/Article/details/glhmspmng.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.yfazqb.com/Article/details/glieouroa.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.sjlbkw.cn/Article/details/gzmmaatyd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.tarul.cn/Article/details/gyestkhkf.sHtML

[S48] C++：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gaqcbxyqj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.vehdjk.com/Article/details/ggvtcjmfq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.bbcook.cn/Article/details/glecqpird.sHtML

[S49] C++：写文件
来源：http://www.share.sjlbkw.cn/Article/details/gljxkrqcg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/goimfxztf.sHtML

[S50] C++：格式化数字
来源：http://blog.tarul.cn/Article/details/gnbihjrff.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fktsv.cn/Article/details/gffsoqrmh.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.yfazqb.com/Article/details/gxvcruvxv.sHtML

static_cast<double>(a) / b
来源：http://www.share.fktsv.cn/Article/details/gshuummil.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.sjlbkw.cn/Article/details/gbslforry.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.yfazqb.com/Article/details/gdymtahbw.sHtML

[S53] C++：移动语义
来源：http://blog.fktsv.cn/Article/details/guhtoyjey.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fktsv.cn/Article/details/gbgnokfxe.sHtML

[S54] C++：异常处理
来源：http://baike.tarul.cn/Article/details/gmwcwtzqu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.tarul.cn/Article/details/goyvtybpr.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fktsv.cn/Article/details/grgidabmi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.yfazqb.com/Article/details/gkhhybccu.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/gdzeykgqp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.epnwcf.com/Article/details/gerrofsmo.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.vehdjk.com/Article/details/gjbedrvam.sHtML

constexpr int N = 10;
来源：http://3g.sjlbkw.cn/Article/details/gojtfuqrx.sHtML

[S58] C++：命名空间
来源：http://read.share.epnwcf.com/Article/details/ghalsopys.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fktsv.cn/Article/details/gelczybxy.sHtML

[S59] C++：静态断言
来源：http://www.blog.vehdjk.com/Article/details/govmqfkpd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.bbcook.cn/Article/details/giorzjwhy.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/gapmfiotk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.epnwcf.com/Article/details/gtrpcojcf.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ggpdcrgka.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.vehdjk.com/Article/details/gnmdrcyiz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gzjkbiqch.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.bbcook.cn/Article/details/godwhuxqs.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gjxqbbqkl.sHtML

[T02] Kotlin：变量
来源：http://www.share.bbcook.cn/Article/details/gnrqzqmmz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.tarul.cn/Article/details/gyfiahoib.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.sjlbkw.cn/Article/details/glryorsqi.sHtML

"值: $b"
来源：http://wap.epnwcf.com/Article/details/gmkvfxkek.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.bbcook.cn/Article/details/ghmysjeev.sHtML

val n: String? = null;  n?.length
来源：http://blog.epnwcf.com/Article/details/gvqtfanbv.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.sjlbkw.cn/Article/details/gowodjuty.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.bbcook.cn/Article/details/gygpuxbpi.sHtML

[T06] Kotlin：集合映射
来源：http://baike.tarul.cn/Article/details/gpmyciden.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.epnwcf.com/Article/details/glxjrebvj.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.epnwcf.com/Article/details/gicpyotam.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fktsv.cn/Article/details/gadqkevgb.sHtML

[T08] Kotlin：数据类
来源：http://read.share.bbcook.cn/Article/details/gpasasnpw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.vehdjk.com/Article/details/ghkoaenzp.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.yfazqb.com/Article/details/gwbcssijm.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.epnwcf.com/Article/details/geuniqjps.sHtML

[T10] Kotlin：默认参数
来源：http://blog.tarul.cn/Article/details/gpolvppgd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.yfazqb.com/Article/details/grfvrippx.sHtML

[T11] Kotlin：协程
来源：http://www.blog.bbcook.cn/Article/details/gyihodtvr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.vehdjk.com/Article/details/gahggavys.sHtML

[T12] Kotlin：解构声明
来源：http://blog.vehdjk.com/Article/details/ghugbacqh.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.vehdjk.com/Article/details/ghgnsyzfb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.yfazqb.com/Article/details/giyfarbvv.sHtML

val m = mapOf("a" to 1)
来源：http://3g.tarul.cn/Article/details/gptnppxrd.sHtML

[T14] Kotlin：循环
来源：http://mobile.sjlbkw.cn/Article/details/gjubtvxjq.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gsptkcqde.sHtML

[T15] Kotlin：接口
来源：http://baike.fktsv.cn/Article/details/gyjfxpijb.sHtML

interface Shape { fun area(): Double }
来源：http://blog.sjlbkw.cn/Article/details/gsutxdxmt.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gsffcqrwa.sHtML

print("Hello")
来源：http://mobile.vehdjk.com/Article/details/gjvdtirdf.sHtML

[T17] Swift：变量与常量
来源：http://3g.yfazqb.com/Article/details/glmlisbsl.sHtML

var a = 1;  let b = 2
来源：http://www.share.vehdjk.com/Article/details/glrvxdulk.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/gcghwtfvq.sHtML

"值: \(b)"
来源：http://blog.tarul.cn/Article/details/gznxdxrkj.sHtML

[T19] Swift：可选绑定
来源：http://mobile.tarul.cn/Article/details/gsvmzhzku.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.yfazqb.com/Article/details/gmtebnjcb.sHtML

[T20] Swift：数组操作
来源：http://baike.yfazqb.com/Article/details/gqwhmtkon.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.yfazqb.com/Article/details/ghsgnrsxz.sHtML

[T21] Swift：遍历
来源：http://read.share.tarul.cn/Article/details/gcwzuwxpm.sHtML

for x in a { print(x) }
来源：http://mobile.bbcook.cn/Article/details/gzcjdzscu.sHtML

[T22] Swift：字典
来源：http://blog.sjlbkw.cn/Article/details/glpgwcdvu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.yfazqb.com/Article/details/gastdlgba.sHtML

[T23] Swift：函数
来源：http://www.blog.tarul.cn/Article/details/glmtpondq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.vehdjk.com/Article/details/ggkjjfear.sHtML

[T24] Swift：闭包
来源：http://3g.tarul.cn/Article/details/geltlmdeq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.epnwcf.com/Article/details/graoszrko.sHtML

[T25] Swift：结构体
来源：http://read.share.yfazqb.com/Article/details/gckbyplbc.sHtML

struct P { var x: Int }
来源：http://baike.epnwcf.com/Article/details/gsqtxbgyh.sHtML

[T26] Swift：类与重写
来源：http://read.share.fktsv.cn/Article/details/gfkcroiew.sHtML

class A: Base { override func f() {} }
来源：http://wap.vehdjk.com/Article/details/gzturzmeh.sHtML

[T27] Swift：错误处理
来源：http://baike.epnwcf.com/Article/details/gjbvwlqoe.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.yfazqb.com/Article/details/gptwfhjui.sHtML

[T28] Swift：枚举
来源：http://mobile.tarul.cn/Article/details/gnpdsanns.sHtML

enum Color { case red, green }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbjohfgg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.sjlbkw.cn/Article/details/gskoenhnn.sHtML

guard let x = opt else { return }
来源：http://baike.fktsv.cn/Article/details/gaxumttuu.sHtML

[T30] Swift：协议
来源：http://m.share.bbcook.cn/Article/details/gmwtlcrjk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.yfazqb.com/Article/details/ggjbqdpew.sHtML

[T31] Lua：Hello World
来源：http://blog.epnwcf.com/Article/details/guhruoqfk.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gcyexnohz.sHtML

[T32] Lua：局部变量
来源：http://m.share.vehdjk.com/Article/details/gotxmbdeb.sHtML

local a = 1
来源：http://read.share.bbcook.cn/Article/details/gqplqdmdu.sHtML

[T33] Lua：表（数组）
来源：http://blog.yfazqb.com/Article/details/gjjhmgfln.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.tarul.cn/Article/details/gbtocyihy.sHtML

[T34] Lua：遍历表
来源：http://blog.sjlbkw.cn/Article/details/gdkgynhnj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.yfazqb.com/Article/details/gosnqfxwr.sHtML

[T35] Lua：字典表
来源：http://m.share.sjlbkw.cn/Article/details/gjwciznvz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.epnwcf.com/Article/details/grgbqeyof.sHtML

[T36] Lua：函数
来源：http://m.share.bbcook.cn/Article/details/gpvhtvclw.sHtML

function add(a, b) return a + b end
来源：http://wap.sjlbkw.cn/Article/details/gzeahttzq.sHtML


<!-- 参考信息 -->