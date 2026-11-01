代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gjhjctdgg.sHtML

[R16] until 等待条件
来源：http://mobile.bbcook.cn/Article/details/gzlmjjclu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gighzunpf.sHtML

[R17] 数组定义与取值
来源：http://blog.tarul.cn/Article/details/gwvvlqzpx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/gkxtcceyr.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/grobqnplk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/ggmjdnlwt.sHtML

[R19] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gbfkiapow.sHtML

echo "${#arr[@]}"
来源：http://wap.vehdjk.com/Article/details/gmbjcbahk.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.yfazqb.com/Article/details/guukvsuma.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.vehdjk.com/Article/details/gmypbppcc.sHtML

[R21] 字符串长度
来源：http://m.share.vehdjk.com/Article/details/glhyivqeu.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/gfsaktlaz.sHtML

[R22] 截取子串
来源：http://www.share.bbcook.cn/Article/details/gkqskasrs.sHtML

echo "${s:0:5}"
来源：http://m.share.epnwcf.com/Article/details/glnhjraqb.sHtML

[R23] 字符串替换
来源：http://3g.bbcook.cn/Article/details/ghortroep.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.vehdjk.com/Article/details/gaxophhtr.sHtML

[R24] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/glrktdnqq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fktsv.cn/Article/details/gxsyvpnjg.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.tarul.cn/Article/details/gwsxefgbz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.tarul.cn/Article/details/gmwwhshvj.sHtML

[R26] 命令替换
来源：http://m.share.yfazqb.com/Article/details/gkzrzkgpt.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gbhmrhtvp.sHtML

[R27] 算术展开
来源：http://www.share.epnwcf.com/Article/details/gifdllbgl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/guxwiysob.sHtML

[R28] 浮点运算
来源：http://baike.bbcook.cn/Article/details/gtbjtxazl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.vehdjk.com/Article/details/gevrxjdpc.sHtML

[R29] 定义函数
来源：http://baike.epnwcf.com/Article/details/goqqbjbes.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.bbcook.cn/Article/details/giprcytzb.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/gosfwdavl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.sjlbkw.cn/Article/details/gtapnnwpk.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/gbbsmufzi.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.sjlbkw.cn/Article/details/gbrykxoxs.sHtML

[R32] 参数个数校验
来源：http://www.m.share.vehdjk.com/Article/details/gepfizadb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.sjlbkw.cn/Article/details/ggqmniuyj.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.tarul.cn/Article/details/gzcnpmbyr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.sjlbkw.cn/Article/details/gljmqpbil.sHtML

[R34] 退出时清理
来源：http://m.share.tarul.cn/Article/details/gqxvwioao.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/ghzimenrb.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.vehdjk.com/Article/details/gcudmbymo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.vehdjk.com/Article/details/gcmdvaxjm.sHtML

[R36] 并发执行多个任务
来源：http://blog.epnwcf.com/Article/details/gnaptfnhg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fktsv.cn/Article/details/gzvkcdrss.sHtML

[R37] 把输出赋给变量
来源：http://baike.bbcook.cn/Article/details/gzogqmsmj.sHtML

files=$(ls -1)
来源：http://blog.epnwcf.com/Article/details/grmqqwlal.sHtML

[R38] 管道串联
来源：http://3g.sjlbkw.cn/Article/details/gsknjgcnl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.bbcook.cn/Article/details/gzqxqqbts.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.yfazqb.com/Article/details/gdtefkxpi.sHtML

cmd > out.log 2>&1
来源：http://mobile.epnwcf.com/Article/details/gdpgxbxjn.sHtML

[R40] 追加写日志
来源：http://baike.vehdjk.com/Article/details/gxvlvlfzk.sHtML

echo "log" >> out.log
来源：http://blog.epnwcf.com/Article/details/grdvqsgbk.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/gmaulhfsq.sHtML

cmd >/dev/null 2>&1
来源：http://baike.sjlbkw.cn/Article/details/ggevwiwoi.sHtML

[R42] 输入重定向
来源：http://blog.yfazqb.com/Article/details/gjolpddlk.sHtML

wc -l < a.txt
来源：http://m.share.bbcook.cn/Article/details/gngloiwqj.sHtML

[R43] 按名字查找文件
来源：http://www.share.fktsv.cn/Article/details/gpgzfgtyk.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/gmtvxvhep.sHtML

[R44] 按修改时间查找
来源：http://www.blog.epnwcf.com/Article/details/gapddhtba.sHtML

find . -mtime -7 -type f
来源：http://read.share.tarul.cn/Article/details/ghbagnrvx.sHtML

[R45] 批量删除
来源：http://mobile.fktsv.cn/Article/details/gzrlwnoth.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fktsv.cn/Article/details/gsqrcqdzl.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gzeufzuxe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.vehdjk.com/Article/details/gjumuyslg.sHtML

[R47] sed 单行替换
来源：http://3g.vehdjk.com/Article/details/gydhnefsy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.bbcook.cn/Article/details/grjcjawqt.sHtML

[R48] awk 取指定列
来源：http://www.share.epnwcf.com/Article/details/garnlmmyz.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gigkyxgxi.sHtML

[R49] awk 带条件
来源：http://wap.tarul.cn/Article/details/gxwntcpmo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.tarul.cn/Article/details/gpzfwlwxz.sHtML

[R50] awk 求和
来源：http://www.blog.fktsv.cn/Article/details/gcmalxddm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.bbcook.cn/Article/details/gxomygjnt.sHtML

[R51] 排序去重取前几
来源：http://3g.yfazqb.com/Article/details/gbjlccduk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.vehdjk.com/Article/details/gjaynexuc.sHtML

[R52] 统计行数
来源：http://www.blog.epnwcf.com/Article/details/gfhfbuzhx.sHtML

wc -l a.txt
来源：http://m.share.epnwcf.com/Article/details/gsiyashyq.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.yfazqb.com/Article/details/grxswqgxt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fktsv.cn/Article/details/gcomdcnas.sHtML

[R54] 比较两个文件
来源：http://m.share.epnwcf.com/Article/details/gppoxwvaz.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/gpihljcfn.sHtML

[R55] 压缩与解压
来源：http://mobile.fktsv.cn/Article/details/gyonxbhwk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.tarul.cn/Article/details/gjnevhwjo.sHtML

[R56] 远程拷贝
来源：http://www.blog.yfazqb.com/Article/details/gpmvtqnst.sHtML

scp file user@host:/path/
来源：http://wap.vehdjk.com/Article/details/gnuakirkm.sHtML

[R57] 远程执行命令
来源：http://blog.sjlbkw.cn/Article/details/gdcumtxjs.sHtML

ssh user@host 'uptime'
来源：http://www.share.tarul.cn/Article/details/gfwoekxfh.sHtML

[R58] 下载文件
来源：http://wap.sjlbkw.cn/Article/details/gumfifzyf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/gytprkliz.sHtML

[R59] 发 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gzgsizwik.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.tarul.cn/Article/details/gczqnahob.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/ggnhuygnj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.yfazqb.com/Article/details/gyvbwvkzm.sHtML

[R61] 磁盘占用
来源：http://blog.bbcook.cn/Article/details/gghllgtvf.sHtML

df -h;  du -sh *
来源：http://www.m.share.yfazqb.com/Article/details/gdqtjhylw.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/gbhukaljo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fktsv.cn/Article/details/ggcxzijte.sHtML

[R63] 内存与进程
来源：http://baike.yfazqb.com/Article/details/gonyozcwj.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.vehdjk.com/Article/details/gbybuivlz.sHtML

[R64] 结束进程
来源：http://www.m.share.tarul.cn/Article/details/gwmzaljdr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.tarul.cn/Article/details/gzjtdinbe.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/gcvqxiegb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.epnwcf.com/Article/details/gqpfixltl.sHtML

[R66] 定时任务
来源：http://3g.vehdjk.com/Article/details/gznjkwgou.sHtML

crontab -e;  crontab -l
来源：http://wap.epnwcf.com/Article/details/gkqmujkbo.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.bbcook.cn/Article/details/gisprwfqc.sHtML

openssl rand -hex 16
来源：http://blog.sjlbkw.cn/Article/details/gxvrngslq.sHtML

[R68] 计算文件校验值
来源：http://baike.bbcook.cn/Article/details/geqdkeopv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.bbcook.cn/Article/details/ghsqmyovs.sHtML

[R69] 生成随机密码
来源：http://mobile.vehdjk.com/Article/details/gguiiciik.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.yfazqb.com/Article/details/gydhdisks.sHtML

[R70] 时间戳与互转
来源：http://mobile.vehdjk.com/Article/details/gcmrrwwkm.sHtML

date +%s;  date -d @1700000000
来源：http://baike.bbcook.cn/Article/details/gvfbkqurq.sHtML

[R71] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gqkigkwdf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.bbcook.cn/Article/details/ghdshwebn.sHtML

[R72] 等待端口就绪
来源：http://baike.bbcook.cn/Article/details/gqhoaxdwd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/gbcmnqjjq.sHtML

[R73] 分割大日志
来源：http://wap.fktsv.cn/Article/details/gwwsluhoa.sHtML

split -l 1000 big.log part_
来源：http://www.blog.vehdjk.com/Article/details/gxbhaoyjy.sHtML

[R74] 批量重命名
来源：http://3g.epnwcf.com/Article/details/gvgywvjxm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/gkmovcuzx.sHtML

[R75] 导出环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gjymagzfr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.yfazqb.com/Article/details/gjwodfnbs.sHtML

[R76] 使用临时文件
来源：http://m.share.sjlbkw.cn/Article/details/goeudfmyq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/gnlsqaanw.sHtML

[R77] 读取用户输入
来源：http://m.share.sjlbkw.cn/Article/details/gklhwqsfs.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fktsv.cn/Article/details/gcsmlfyiq.sHtML

[R78] 交互式菜单
来源：http://blog.vehdjk.com/Article/details/gvxyuiyty.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.epnwcf.com/Article/details/guggnzhsv.sHtML

[R79] 解析命令行选项
来源：http://blog.vehdjk.com/Article/details/gjwzzzgzn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.epnwcf.com/Article/details/gtdmqqfjs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.tarul.cn/Article/details/ganvbkbrr.sHtML

time ./run.sh
来源：http://3g.bbcook.cn/Article/details/gwomxhggk.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gzabqrrtq.sHtML

S. C / C++ 专题
来源：http://www.share.yfazqb.com/Article/details/gowuhwpjd.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gcfliqrxg.sHtML

[S01] C：Hello World
来源：http://blog.bbcook.cn/Article/details/gseliojpr.sHtML

#include <stdio.h>
来源：http://www.share.fktsv.cn/Article/details/gvrhsifdf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fktsv.cn/Article/details/gfsuoulra.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/gfjhxrjvt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.yfazqb.com/Article/details/grgoqdmny.sHtML

[S03] C：读入整数
来源：http://3g.fktsv.cn/Article/details/gkyloabjt.sHtML

int x; scanf("%d", &x);
来源：http://3g.vehdjk.com/Article/details/glssfmsyw.sHtML

[S04] C：字符串复制
来源：http://www.blog.fktsv.cn/Article/details/ggvvqkxim.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fktsv.cn/Article/details/gyiayrflo.sHtML

[S05] C：字符串长度
来源：http://read.share.epnwcf.com/Article/details/gyfhsfngn.sHtML

strlen(s)
来源：http://mobile.sjlbkw.cn/Article/details/gfbvigrgx.sHtML

[S06] C：字符串比较
来源：http://wap.vehdjk.com/Article/details/gsvxbjzic.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.bbcook.cn/Article/details/gbeqeqyds.sHtML

[S07] C：数组遍历求和
来源：http://blog.vehdjk.com/Article/details/gppcgvrch.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.vehdjk.com/Article/details/gqlqxxrmy.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.tarul.cn/Article/details/gmrhkclay.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.sjlbkw.cn/Article/details/gbntrlhil.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.epnwcf.com/Article/details/gvyougvaa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.epnwcf.com/Article/details/gqfbzxlqz.sHtML

[S10] C：指针与解引用
来源：http://baike.fktsv.cn/Article/details/gexcxhprl.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.bbcook.cn/Article/details/ggandoaey.sHtML

[S11] C：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gqnrxnxsr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.bbcook.cn/Article/details/gqhgeukuv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.tarul.cn/Article/details/giyqmdlmf.sHtML

fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gyjvidabb.sHtML

[S12] C：写文件
来源：http://baike.sjlbkw.cn/Article/details/gfdbynwbh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.tarul.cn/Article/details/gcnbefvhu.sHtML

[S13] C：宏定义
来源：http://m.share.fktsv.cn/Article/details/ghvzgbnzb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.epnwcf.com/Article/details/gpqcbwyau.sHtML

[S14] C：枚举
来源：http://mobile.yfazqb.com/Article/details/gzkuwodpn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fktsv.cn/Article/details/gkbynvygf.sHtML

[S15] C：类型转换
来源：http://www.blog.bbcook.cn/Article/details/gvlpfiuar.sHtML

(double) a / b
来源：http://baike.epnwcf.com/Article/details/gktyriybv.sHtML

[S16] C：位操作置位
来源：http://wap.epnwcf.com/Article/details/gamyqnbll.sHtML

x |= (1 << 3);
来源：http://mobile.epnwcf.com/Article/details/gslspqfwr.sHtML

[S17] C：安全拼接字符串
来源：http://blog.epnwcf.com/Article/details/grpnjucpp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/gyedzdnoz.sHtML

[S18] C：命令行参数
来源：http://baike.yfazqb.com/Article/details/gyfawymss.sHtML

int main(int argc, char **argv)
来源：http://wap.yfazqb.com/Article/details/gfdqqbuhb.sHtML

[S19] C：快速排序
来源：http://wap.bbcook.cn/Article/details/gbjwhjbqj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/gzipjkjpo.sHtML

[S20] C：二分查找
来源：http://read.share.epnwcf.com/Article/details/gtkdjrqyq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gweoklmnl.sHtML

[S21] C：字符类别判断
来源：http://3g.epnwcf.com/Article/details/garetvffk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.tarul.cn/Article/details/gqyxalkno.sHtML

[S22] C：字符串转数字
来源：http://mobile.epnwcf.com/Article/details/gzqvlfnoy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fktsv.cn/Article/details/gnzcdftcc.sHtML

[S23] C：随机数
来源：http://3g.yfazqb.com/Article/details/ghqqhsuki.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.yfazqb.com/Article/details/glffhrmio.sHtML

[S24] C：获取本地时间
来源：http://read.share.fktsv.cn/Article/details/gtolownnw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fktsv.cn/Article/details/gcngzrxaz.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gxagblxyv.sHtML

memcpy(dst, src, n);
来源：http://3g.sjlbkw.cn/Article/details/gfltrpznm.sHtML

[S26] C：内存清零
来源：http://www.share.vehdjk.com/Article/details/gfjuasiya.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.epnwcf.com/Article/details/gymwymbeu.sHtML

[S27] C：定义常量
来源：http://m.share.yfazqb.com/Article/details/gtfgufcvw.sHtML

const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gwvdwbrlg.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/ghgqahich.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/ghhllaiiu.sHtML

[S29] C：变参函数
来源：http://mobile.tarul.cn/Article/details/glhtvrzlh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.sjlbkw.cn/Article/details/gtubwmjuc.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/gmqfbqfyn.sHtML

#ifndef X_H
来源：http://read.share.yfazqb.com/Article/details/gyfrckbgw.sHtML

#define X_H
来源：http://read.share.vehdjk.com/Article/details/ghsfcitvs.sHtML

#endif
来源：http://blog.bbcook.cn/Article/details/golpmhvbr.sHtML

[S31] C++：Hello World
来源：http://baike.vehdjk.com/Article/details/gdafocsda.sHtML

#include <iostream>
来源：http://m.share.vehdjk.com/Article/details/gnaaxviqs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.tarul.cn/Article/details/gftnvuihz.sHtML

[S32] C++：字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gjjhjnkgc.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fktsv.cn/Article/details/gstuzobai.sHtML

[S33] C++：vector 增删
来源：http://baike.fktsv.cn/Article/details/gblyjpmty.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.yfazqb.com/Article/details/gttqlevhb.sHtML

[S34] C++：遍历 vector
来源：http://baike.sjlbkw.cn/Article/details/gttvjcuyc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.yfazqb.com/Article/details/gxnecdkwv.sHtML

[S35] C++：map
来源：http://m.share.fktsv.cn/Article/details/gfqgkveqi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gkfifvphv.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.sjlbkw.cn/Article/details/gxirbphqp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/ggfpbccuw.sHtML

[S37] C++：set
来源：http://mobile.sjlbkw.cn/Article/details/gtulhvzdl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.sjlbkw.cn/Article/details/gcymadtts.sHtML

[S38] C++：排序
来源：http://read.share.epnwcf.com/Article/details/gficmygaa.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.epnwcf.com/Article/details/goupnxqsz.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/gpxdpiopw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.yfazqb.com/Article/details/ghlawsvji.sHtML

[S40] C++：查找元素
来源：http://www.blog.tarul.cn/Article/details/gbsgfwymf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.epnwcf.com/Article/details/gkpphpnyd.sHtML

[S41] C++：类与构造函数
来源：http://3g.fktsv.cn/Article/details/gozhacnvs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.bbcook.cn/Article/details/gflztkvrk.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.epnwcf.com/Article/details/gaglivnoy.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fktsv.cn/Article/details/guoalcfnc.sHtML

[S43] C++：智能指针
来源：http://m.share.epnwcf.com/Article/details/gmglzvurf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.yfazqb.com/Article/details/gmgivitut.sHtML

[S44] C++：引用传参
来源：http://wap.fktsv.cn/Article/details/gsxuliqpj.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.yfazqb.com/Article/details/gnqgscqsq.sHtML

[S45] C++：lambda
来源：http://read.share.epnwcf.com/Article/details/grtljygmn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.yfazqb.com/Article/details/gtlehgyrh.sHtML

[S46] C++：函数模板
来源：http://mobile.fktsv.cn/Article/details/giaucbgmo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.epnwcf.com/Article/details/gvqphnyso.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/goeejfoui.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/grogdafei.sHtML

[S48] C++：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gzoxjdqfv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkokfiyfe.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fktsv.cn/Article/details/ghilehazg.sHtML

[S49] C++：写文件
来源：http://baike.epnwcf.com/Article/details/gdgwmeclz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fktsv.cn/Article/details/gkobjqojt.sHtML

[S50] C++：格式化数字
来源：http://3g.epnwcf.com/Article/details/gdgvcyuxe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.tarul.cn/Article/details/gzqtopxfh.sHtML

[S51] C++：显式类型转换
来源：http://3g.bbcook.cn/Article/details/gzpfjbyqn.sHtML

static_cast<double>(a) / b
来源：http://read.share.vehdjk.com/Article/details/gqdasdsui.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.yfazqb.com/Article/details/goiswravw.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.sjlbkw.cn/Article/details/gahjtvpwb.sHtML

[S53] C++：移动语义
来源：http://baike.tarul.cn/Article/details/gxzzlqcav.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/gqkzvxgne.sHtML

[S54] C++：异常处理
来源：http://3g.vehdjk.com/Article/details/gtbkjblqb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.tarul.cn/Article/details/gjzpabgrl.sHtML

[S55] C++：结构化绑定
来源：http://baike.tarul.cn/Article/details/gtlwppnhm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.tarul.cn/Article/details/gvhleidvo.sHtML

[S56] C++：optional
来源：http://www.m.share.fktsv.cn/Article/details/gzwuenczf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.bbcook.cn/Article/details/gmpufuthn.sHtML

[S57] C++：编译期常量
来源：http://wap.fktsv.cn/Article/details/grjvakmrr.sHtML

constexpr int N = 10;
来源：http://3g.fktsv.cn/Article/details/gpfqovdfr.sHtML

[S58] C++：命名空间
来源：http://www.share.vehdjk.com/Article/details/gxwavszgi.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fktsv.cn/Article/details/gxngdappd.sHtML

[S59] C++：静态断言
来源：http://mobile.vehdjk.com/Article/details/gxklmkftw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fktsv.cn/Article/details/gheamkiky.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.yfazqb.com/Article/details/gywmwlojo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.tarul.cn/Article/details/gtpmbjpjv.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/guzqeezmv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/gumpidvhk.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glfnljcok.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gzoxcvzfh.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/gxpuhvvdj.sHtML

[T02] Kotlin：变量
来源：http://www.share.bbcook.cn/Article/details/gecxpipbc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.bbcook.cn/Article/details/gpidhnmti.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fktsv.cn/Article/details/gozuoexaq.sHtML

"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/gwrasjrcm.sHtML

[T04] Kotlin：空安全
来源：http://www.share.vehdjk.com/Article/details/gnmkxxueo.sHtML

val n: String? = null;  n?.length
来源：http://m.share.tarul.cn/Article/details/gbievrxnl.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.tarul.cn/Article/details/gvmiuwlyf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.vehdjk.com/Article/details/gujrczims.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.yfazqb.com/Article/details/gztcsasmq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/gbtyutphs.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.vehdjk.com/Article/details/gvzwdguzg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.tarul.cn/Article/details/gtheacwvc.sHtML

[T08] Kotlin：数据类
来源：http://3g.vehdjk.com/Article/details/gkmicwarh.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.vehdjk.com/Article/details/ggwqasoaa.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fktsv.cn/Article/details/gunhzimly.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.sjlbkw.cn/Article/details/ghdzspgpe.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gfofpqsuo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.sjlbkw.cn/Article/details/gwnzfdpiy.sHtML

[T11] Kotlin：协程
来源：http://blog.epnwcf.com/Article/details/gcqvisirm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.epnwcf.com/Article/details/ghawiitob.sHtML

[T12] Kotlin：解构声明
来源：http://3g.yfazqb.com/Article/details/gzcaqywoh.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.tarul.cn/Article/details/gtfmkztto.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.vehdjk.com/Article/details/ghymmcqdz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.vehdjk.com/Article/details/gnpffhyiy.sHtML

[T14] Kotlin：循环
来源：http://www.share.epnwcf.com/Article/details/gtnjphfwr.sHtML

for (i in 1..10) println(i)
来源：http://m.share.yfazqb.com/Article/details/gffuhxlld.sHtML

[T15] Kotlin：接口
来源：http://baike.tarul.cn/Article/details/gjqridayx.sHtML

interface Shape { fun area(): Double }
来源：http://blog.yfazqb.com/Article/details/gnpumdqgg.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/ggiaullde.sHtML

print("Hello")
来源：http://blog.epnwcf.com/Article/details/gxxkqnkfy.sHtML

[T17] Swift：变量与常量
来源：http://read.share.sjlbkw.cn/Article/details/gnivaqexn.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/gzlghfmdr.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gjnrfvjgn.sHtML

"值: \(b)"
来源：http://mobile.epnwcf.com/Article/details/gejuwzkon.sHtML


<!-- 参考信息 -->