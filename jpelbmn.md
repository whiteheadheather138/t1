代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.vehdjk.com/Article/details/gutxpyitm.sHtML

[R16] until 等待条件
来源：http://mobile.yfazqb.com/Article/details/gcvuoxkwo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gddnrjrcw.sHtML

[R17] 数组定义与取值
来源：http://mobile.vehdjk.com/Article/details/grgvyuirh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.vehdjk.com/Article/details/gabvmrmge.sHtML

[R18] 遍历数组
来源：http://www.share.bbcook.cn/Article/details/guvaqauhu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/gbpvylytn.sHtML

[R19] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/ghxarlxhe.sHtML

echo "${#arr[@]}"
来源：http://3g.yfazqb.com/Article/details/gedjpmqwj.sHtML

[R20] 关联数组（字典）
来源：http://m.share.yfazqb.com/Article/details/ginyxjxag.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.tarul.cn/Article/details/gakhfwzlb.sHtML

[R21] 字符串长度
来源：http://3g.yfazqb.com/Article/details/gmgolztkh.sHtML

echo "${#s}"
来源：http://read.share.tarul.cn/Article/details/gkneieehg.sHtML

[R22] 截取子串
来源：http://m.share.bbcook.cn/Article/details/gkejvttmf.sHtML

echo "${s:0:5}"
来源：http://www.m.share.yfazqb.com/Article/details/gwnfeseas.sHtML

[R23] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gavagfvtp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.vehdjk.com/Article/details/gerkpgarz.sHtML

[R24] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gpigofjis.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.vehdjk.com/Article/details/gstbniain.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fktsv.cn/Article/details/gpevonpos.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/gydufcwmk.sHtML

[R26] 命令替换
来源：http://www.blog.bbcook.cn/Article/details/gxrrkfuqd.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.sjlbkw.cn/Article/details/grwhnqmzj.sHtML

[R27] 算术展开
来源：http://www.blog.yfazqb.com/Article/details/glhizrmkl.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.tarul.cn/Article/details/gyddoaeye.sHtML

[R28] 浮点运算
来源：http://3g.bbcook.cn/Article/details/gvknnmxzf.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fktsv.cn/Article/details/grfnjjyyn.sHtML

[R29] 定义函数
来源：http://3g.fktsv.cn/Article/details/gsikmccxq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gfvmhrozl.sHtML

[R30] 函数返回状态码
来源：http://baike.vehdjk.com/Article/details/gpmzxvjwe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.yfazqb.com/Article/details/gsnqlvtqk.sHtML

[R31] 局部变量
来源：http://mobile.epnwcf.com/Article/details/gcvdqdxcd.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.yfazqb.com/Article/details/gqogozkju.sHtML

[R32] 参数个数校验
来源：http://read.share.yfazqb.com/Article/details/gtdwhqkdy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gntvbjrit.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.bbcook.cn/Article/details/gbqgjtnkv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.tarul.cn/Article/details/gheyfuelb.sHtML

[R34] 退出时清理
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsxkzebd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gfafmaafd.sHtML

[R35] 后台执行并等待
来源：http://3g.fktsv.cn/Article/details/ghlrfqbvg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fktsv.cn/Article/details/gcztgxgdy.sHtML

[R36] 并发执行多个任务
来源：http://read.share.tarul.cn/Article/details/gyuokiqmk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.yfazqb.com/Article/details/gtfvnjysb.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.sjlbkw.cn/Article/details/glgwjewwu.sHtML

files=$(ls -1)
来源：http://mobile.sjlbkw.cn/Article/details/gdvodzmnr.sHtML

[R38] 管道串联
来源：http://blog.fktsv.cn/Article/details/gyqztxhea.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.tarul.cn/Article/details/gmsuoavud.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.epnwcf.com/Article/details/gmjqcbmmb.sHtML

cmd > out.log 2>&1
来源：http://m.share.fktsv.cn/Article/details/gxrvzcnfv.sHtML

[R40] 追加写日志
来源：http://read.share.bbcook.cn/Article/details/gxbbroadd.sHtML

echo "log" >> out.log
来源：http://3g.epnwcf.com/Article/details/gyuridwyg.sHtML

[R41] 丢弃输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtewsxaq.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.yfazqb.com/Article/details/gpeikfqjl.sHtML

[R42] 输入重定向
来源：http://baike.bbcook.cn/Article/details/gnofzdtmt.sHtML

wc -l < a.txt
来源：http://blog.sjlbkw.cn/Article/details/gdhwehzky.sHtML

[R43] 按名字查找文件
来源：http://wap.fktsv.cn/Article/details/gmpltbmqe.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gaqkusskl.sHtML

[R44] 按修改时间查找
来源：http://m.share.vehdjk.com/Article/details/gpoojxjjl.sHtML

find . -mtime -7 -type f
来源：http://wap.vehdjk.com/Article/details/gxmoetewv.sHtML

[R45] 批量删除
来源：http://baike.sjlbkw.cn/Article/details/gxpzphpmq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.vehdjk.com/Article/details/geflqzkrx.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gvkedzsqr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.sjlbkw.cn/Article/details/gpxvexktj.sHtML

[R47] sed 单行替换
来源：http://blog.bbcook.cn/Article/details/gsuvvtwvj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/gqowafevf.sHtML

[R48] awk 取指定列
来源：http://m.share.sjlbkw.cn/Article/details/gdfdnitto.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.epnwcf.com/Article/details/gbtolbzeg.sHtML

[R49] awk 带条件
来源：http://baike.epnwcf.com/Article/details/govwnintb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.yfazqb.com/Article/details/gvipujesz.sHtML

[R50] awk 求和
来源：http://3g.bbcook.cn/Article/details/gqcgpopld.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fktsv.cn/Article/details/ggpnkyjzk.sHtML

[R51] 排序去重取前几
来源：http://baike.yfazqb.com/Article/details/grskwircs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.bbcook.cn/Article/details/gxchvcxah.sHtML

[R52] 统计行数
来源：http://www.m.share.bbcook.cn/Article/details/ghgcbmolr.sHtML

wc -l a.txt
来源：http://blog.tarul.cn/Article/details/ghsgxunlq.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.bbcook.cn/Article/details/gcitzzcoa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fktsv.cn/Article/details/gaalmrnuc.sHtML

[R54] 比较两个文件
来源：http://baike.bbcook.cn/Article/details/grlrzcgne.sHtML

diff a.txt b.txt
来源：http://www.blog.vehdjk.com/Article/details/grlugjqfs.sHtML

[R55] 压缩与解压
来源：http://baike.epnwcf.com/Article/details/guykrjotm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.sjlbkw.cn/Article/details/gefvmnrxv.sHtML

[R56] 远程拷贝
来源：http://read.share.tarul.cn/Article/details/gqtbmeamf.sHtML

scp file user@host:/path/
来源：http://blog.tarul.cn/Article/details/gddaxdhxp.sHtML

[R57] 远程执行命令
来源：http://mobile.epnwcf.com/Article/details/grmhtuysb.sHtML

ssh user@host 'uptime'
来源：http://blog.yfazqb.com/Article/details/gyxdfkoou.sHtML

[R58] 下载文件
来源：http://3g.fktsv.cn/Article/details/gasyftyur.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.epnwcf.com/Article/details/gubcrvksn.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/goabzerem.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.yfazqb.com/Article/details/gqzjwzhle.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gtvuswtfc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.vehdjk.com/Article/details/galhqanlt.sHtML

[R61] 磁盘占用
来源：http://wap.bbcook.cn/Article/details/ggdkgndgb.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/gxoxuaqka.sHtML

[R62] 找最占空间的文件
来源：http://read.share.sjlbkw.cn/Article/details/gpyyxlmqc.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.yfazqb.com/Article/details/gfzdfzqvq.sHtML

[R63] 内存与进程
来源：http://mobile.fktsv.cn/Article/details/gblrynvsl.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.vehdjk.com/Article/details/gwnckkbhy.sHtML

[R64] 结束进程
来源：http://www.share.bbcook.cn/Article/details/guyqpkaez.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.tarul.cn/Article/details/gtcretpvk.sHtML

[R65] 查看端口占用
来源：http://www.m.share.vehdjk.com/Article/details/giznacopu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.epnwcf.com/Article/details/gkqjxouak.sHtML

[R66] 定时任务
来源：http://3g.bbcook.cn/Article/details/gstudrupk.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/gydnarhos.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.tarul.cn/Article/details/ghtlxfmmk.sHtML

openssl rand -hex 16
来源：http://mobile.yfazqb.com/Article/details/gafeusbpd.sHtML

[R68] 计算文件校验值
来源：http://baike.vehdjk.com/Article/details/gqgzidgdt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.vehdjk.com/Article/details/gpmpmzdkz.sHtML

[R69] 生成随机密码
来源：http://mobile.fktsv.cn/Article/details/gsiagqnpk.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.bbcook.cn/Article/details/gpcemgvqv.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gomykjsxm.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fktsv.cn/Article/details/ggxonnmca.sHtML

[R71] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gawbjemrk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.vehdjk.com/Article/details/gqjazfvhj.sHtML

[R72] 等待端口就绪
来源：http://m.share.sjlbkw.cn/Article/details/goixvcyqq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/gptktxkhn.sHtML

[R73] 分割大日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gailgtrup.sHtML

split -l 1000 big.log part_
来源：http://www.blog.tarul.cn/Article/details/gwyfxwlvn.sHtML

[R74] 批量重命名
来源：http://blog.epnwcf.com/Article/details/gcrkkscsb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.epnwcf.com/Article/details/gjulbjngj.sHtML

[R75] 导出环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gozqntdut.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.vehdjk.com/Article/details/glzluhmlj.sHtML

[R76] 使用临时文件
来源：http://baike.epnwcf.com/Article/details/gqowjqwoz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/gtdcpsxay.sHtML

[R77] 读取用户输入
来源：http://read.share.bbcook.cn/Article/details/gcpfhluuk.sHtML

read -rp "请输入: " ans
来源：http://www.blog.tarul.cn/Article/details/ghwscxpsj.sHtML

[R78] 交互式菜单
来源：http://wap.fktsv.cn/Article/details/gkypjmknx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.sjlbkw.cn/Article/details/gmzugqsbr.sHtML

[R79] 解析命令行选项
来源：http://m.share.fktsv.cn/Article/details/gbdlcjkxo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/gonwdpyht.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.vehdjk.com/Article/details/gchmyrfqr.sHtML

time ./run.sh
来源：http://read.share.sjlbkw.cn/Article/details/gxbbejvfq.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gcapejpou.sHtML

S. C / C++ 专题
来源：http://m.share.tarul.cn/Article/details/gfgriiysu.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gicdocsxv.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gjcatbmxn.sHtML

#include <stdio.h>
来源：http://baike.fktsv.cn/Article/details/gmnnijnud.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gocwkxrwc.sHtML

[S02] C：变量与格式化输出
来源：http://baike.sjlbkw.cn/Article/details/guzxazpfh.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.sjlbkw.cn/Article/details/geyotjeay.sHtML

[S03] C：读入整数
来源：http://wap.fktsv.cn/Article/details/gbpcvxtqa.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.sjlbkw.cn/Article/details/gfiqsdiri.sHtML

[S04] C：字符串复制
来源：http://mobile.epnwcf.com/Article/details/gqcrgoefg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fktsv.cn/Article/details/gdeyghhny.sHtML

[S05] C：字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gtcdcnida.sHtML

strlen(s)
来源：http://wap.yfazqb.com/Article/details/gahkfsjrj.sHtML

[S06] C：字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gamlvpbke.sHtML

strcmp(a, b) == 0
来源：http://baike.tarul.cn/Article/details/gipcbvufd.sHtML

[S07] C：数组遍历求和
来源：http://baike.tarul.cn/Article/details/gbnroltqr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.bbcook.cn/Article/details/gyipsfsod.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.tarul.cn/Article/details/gguibvkkf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.yfazqb.com/Article/details/gpiahdiat.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.bbcook.cn/Article/details/gosnwvumq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.epnwcf.com/Article/details/gzqwgjkdi.sHtML

[S10] C：指针与解引用
来源：http://blog.epnwcf.com/Article/details/ghivhvyls.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.bbcook.cn/Article/details/gfeekngdj.sHtML

[S11] C：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gyrhhimys.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.yfazqb.com/Article/details/gvvfsgsjy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.tarul.cn/Article/details/gavttligm.sHtML

fclose(f);
来源：http://mobile.yfazqb.com/Article/details/gbqkwwqsz.sHtML

[S12] C：写文件
来源：http://wap.yfazqb.com/Article/details/gsbionzvf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.epnwcf.com/Article/details/gyxuaqnfm.sHtML

[S13] C：宏定义
来源：http://read.share.bbcook.cn/Article/details/grgecihkl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.bbcook.cn/Article/details/germcdlan.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/ggemeptev.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.epnwcf.com/Article/details/gkvcexdqt.sHtML

[S15] C：类型转换
来源：http://m.share.tarul.cn/Article/details/gqlzmmwbp.sHtML

(double) a / b
来源：http://m.share.sjlbkw.cn/Article/details/gafnbwkif.sHtML

[S16] C：位操作置位
来源：http://blog.sjlbkw.cn/Article/details/gxmvtuila.sHtML

x |= (1 << 3);
来源：http://read.share.vehdjk.com/Article/details/gzbrzplpq.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.vehdjk.com/Article/details/grsblvgub.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.bbcook.cn/Article/details/grsnnqubi.sHtML

[S18] C：命令行参数
来源：http://wap.epnwcf.com/Article/details/ggsfcegsz.sHtML

int main(int argc, char **argv)
来源：http://wap.epnwcf.com/Article/details/guwtrhbas.sHtML

[S19] C：快速排序
来源：http://www.share.yfazqb.com/Article/details/gpcbnnrok.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gdsqhuany.sHtML

[S20] C：二分查找
来源：http://mobile.fktsv.cn/Article/details/gpnymhljg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/gcvivhpwv.sHtML

[S21] C：字符类别判断
来源：http://www.share.tarul.cn/Article/details/gnkgswoen.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.vehdjk.com/Article/details/gsvgqjoqu.sHtML

[S22] C：字符串转数字
来源：http://m.share.vehdjk.com/Article/details/glxpusxqr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.tarul.cn/Article/details/gyocrbxrr.sHtML

[S23] C：随机数
来源：http://3g.vehdjk.com/Article/details/gwhqioved.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.bbcook.cn/Article/details/gqlmvdnav.sHtML

[S24] C：获取本地时间
来源：http://m.share.bbcook.cn/Article/details/gkulpqlpd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fktsv.cn/Article/details/gfccrdqav.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/gohgnqbcs.sHtML

memcpy(dst, src, n);
来源：http://www.share.vehdjk.com/Article/details/gefcbnffw.sHtML

[S26] C：内存清零
来源：http://read.share.tarul.cn/Article/details/gavpywral.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fktsv.cn/Article/details/gndeniojr.sHtML

[S27] C：定义常量
来源：http://blog.yfazqb.com/Article/details/gvcyzexxc.sHtML

const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gmitnotfk.sHtML

[S28] C：静态变量
来源：http://mobile.tarul.cn/Article/details/gmcugkdvi.sHtML

static int counter = 0;
来源：http://www.m.share.vehdjk.com/Article/details/gxwbgjumy.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/gadtfrllg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.vehdjk.com/Article/details/gtekqqvyf.sHtML

[S30] C：头文件保护
来源：http://www.m.share.yfazqb.com/Article/details/gwnabzaip.sHtML

#ifndef X_H
来源：http://www.m.share.yfazqb.com/Article/details/gwmvqanzl.sHtML

#define X_H
来源：http://wap.yfazqb.com/Article/details/gpriuvguk.sHtML

#endif
来源：http://blog.vehdjk.com/Article/details/gjxtgcgrc.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gabufiyto.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/gkyaowzbp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fktsv.cn/Article/details/gbmsqagio.sHtML

[S32] C++：字符串
来源：http://www.share.vehdjk.com/Article/details/gkgxmxsib.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.tarul.cn/Article/details/gqztbbehl.sHtML

[S33] C++：vector 增删
来源：http://wap.epnwcf.com/Article/details/gqtxbegog.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.bbcook.cn/Article/details/grsvokipb.sHtML

[S34] C++：遍历 vector
来源：http://www.share.yfazqb.com/Article/details/gtcuntmod.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.yfazqb.com/Article/details/ghqzcgxty.sHtML

[S35] C++：map
来源：http://read.share.tarul.cn/Article/details/gwkzowwkx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gbmntscyr.sHtML

[S36] C++：unordered_map
来源：http://mobile.sjlbkw.cn/Article/details/gvpwoyvmn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gbexmtbhd.sHtML

[S37] C++：set
来源：http://www.blog.fktsv.cn/Article/details/gfndtkebe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/gvnhqgnll.sHtML

[S38] C++：排序
来源：http://m.share.epnwcf.com/Article/details/gcfqecvzd.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/gwdkiyqwc.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gjrgyjoca.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/gclksdoli.sHtML

[S40] C++：查找元素
来源：http://m.share.sjlbkw.cn/Article/details/gbhgfixlg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.vehdjk.com/Article/details/ganflwrhs.sHtML

[S41] C++：类与构造函数
来源：http://mobile.yfazqb.com/Article/details/gfrznictk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.sjlbkw.cn/Article/details/gjzbqqtls.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.vehdjk.com/Article/details/gkjjgqseo.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fktsv.cn/Article/details/gpiwjupug.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gkorbeenp.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.yfazqb.com/Article/details/girsppykc.sHtML

[S44] C++：引用传参
来源：http://read.share.fktsv.cn/Article/details/gexlzzhat.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.vehdjk.com/Article/details/glucvzutm.sHtML

[S45] C++：lambda
来源：http://read.share.epnwcf.com/Article/details/giqrrvscy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.epnwcf.com/Article/details/gkqbbifum.sHtML

[S46] C++：函数模板
来源：http://baike.tarul.cn/Article/details/ghohdxhcx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.tarul.cn/Article/details/gsbxwyigv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.bbcook.cn/Article/details/gvewxwznn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.epnwcf.com/Article/details/gzbokwlwe.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gbhmgdlai.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.vehdjk.com/Article/details/ggvvcnlcq.sHtML

while (std::getline(in, line)) { }
来源：http://blog.sjlbkw.cn/Article/details/gvwbpfitm.sHtML

[S49] C++：写文件
来源：http://baike.tarul.cn/Article/details/grujcvzcv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.yfazqb.com/Article/details/gjguczkzv.sHtML

[S50] C++：格式化数字
来源：http://read.share.sjlbkw.cn/Article/details/gmdwuexyz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gqaaigolj.sHtML

[S51] C++：显式类型转换
来源：http://blog.tarul.cn/Article/details/gqbwgeirn.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fktsv.cn/Article/details/gosqbtnkb.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.vehdjk.com/Article/details/goxlrfdtc.sHtML

int size() const noexcept { return n_; }
来源：http://wap.vehdjk.com/Article/details/grgxvywuy.sHtML

[S53] C++：移动语义
来源：http://mobile.vehdjk.com/Article/details/gvyjywdis.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.vehdjk.com/Article/details/gtoncyiru.sHtML

[S54] C++：异常处理
来源：http://read.share.sjlbkw.cn/Article/details/gsdddflol.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.vehdjk.com/Article/details/gijidzwns.sHtML

[S55] C++：结构化绑定
来源：http://wap.yfazqb.com/Article/details/gklistgci.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.vehdjk.com/Article/details/gfgkaimwh.sHtML

[S56] C++：optional
来源：http://baike.vehdjk.com/Article/details/gzvjwfmdo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.vehdjk.com/Article/details/gcibfqwjs.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fktsv.cn/Article/details/gkzqmsdtt.sHtML

constexpr int N = 10;
来源：http://baike.tarul.cn/Article/details/geomfwxtt.sHtML

[S58] C++：命名空间
来源：http://baike.vehdjk.com/Article/details/guhkitpti.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.yfazqb.com/Article/details/ggnldkjxv.sHtML

[S59] C++：静态断言
来源：http://wap.bbcook.cn/Article/details/gvxgxqcdz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.bbcook.cn/Article/details/gxcwmzjqd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gwuajlvvq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/gwgoouqmi.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gxykrgzog.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.vehdjk.com/Article/details/gkwfbfaut.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gauwvxqjy.sHtML

[T01] Kotlin：Hello World
来源：http://3g.epnwcf.com/Article/details/gjrsrahqm.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gbxvreyyl.sHtML

[T02] Kotlin：变量
来源：http://www.blog.yfazqb.com/Article/details/gmmiabgat.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.sjlbkw.cn/Article/details/gorfeuyql.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.yfazqb.com/Article/details/gwwspehqm.sHtML

"值: $b"
来源：http://wap.yfazqb.com/Article/details/glqwdfape.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.epnwcf.com/Article/details/gugcmkapq.sHtML

val n: String? = null;  n?.length
来源：http://baike.sjlbkw.cn/Article/details/gspzpmbqi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/grultofhn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fktsv.cn/Article/details/gmplnkvjd.sHtML

[T06] Kotlin：集合映射
来源：http://3g.tarul.cn/Article/details/gsmrfypyt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/gsztazffx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gsqkpwrgt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fktsv.cn/Article/details/gohmgdgyt.sHtML

[T08] Kotlin：数据类
来源：http://mobile.vehdjk.com/Article/details/gcrpsuytw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gfnxtycai.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.yfazqb.com/Article/details/gynbnhxhg.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.tarul.cn/Article/details/ggblbvlqx.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.yfazqb.com/Article/details/gugorairf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.epnwcf.com/Article/details/gopuhrrds.sHtML

[T11] Kotlin：协程
来源：http://www.blog.bbcook.cn/Article/details/gpefluqfk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.yfazqb.com/Article/details/gtigijdgv.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.sjlbkw.cn/Article/details/gxrzdisec.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.tarul.cn/Article/details/ggtsjyflg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.vehdjk.com/Article/details/gkxvdzygz.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.vehdjk.com/Article/details/gwasyacsa.sHtML

[T14] Kotlin：循环
来源：http://baike.yfazqb.com/Article/details/gkyyzeqcl.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/gesnetggu.sHtML

[T15] Kotlin：接口
来源：http://www.share.yfazqb.com/Article/details/gllxteyzl.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fktsv.cn/Article/details/gxfwdtgdu.sHtML

[T16] Swift：Hello World
来源：http://blog.bbcook.cn/Article/details/gkxpevfzg.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/gfkcvzvsd.sHtML

[T17] Swift：变量与常量
来源：http://blog.epnwcf.com/Article/details/gufcttsnh.sHtML

var a = 1;  let b = 2
来源：http://blog.vehdjk.com/Article/details/gpzpvpfij.sHtML

[T18] Swift：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gqzqacius.sHtML

"值: \(b)"
来源：http://wap.epnwcf.com/Article/details/gfmqruoms.sHtML


<!-- 参考信息 -->