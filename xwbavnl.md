代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.epnwcf.com/Article/details/gtluywavi.sHtML

[R16] until 等待条件
来源：http://baike.fktsv.cn/Article/details/gzlrenrst.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gcpdhjfgv.sHtML

[R17] 数组定义与取值
来源：http://read.share.tarul.cn/Article/details/grqcsmrmt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.sjlbkw.cn/Article/details/gwefqsajg.sHtML

[R18] 遍历数组
来源：http://mobile.bbcook.cn/Article/details/gtcbsgppk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.sjlbkw.cn/Article/details/gznniqtpi.sHtML

[R19] 数组长度
来源：http://www.share.sjlbkw.cn/Article/details/gxacgxvwa.sHtML

echo "${#arr[@]}"
来源：http://www.blog.tarul.cn/Article/details/gpjsruikd.sHtML

[R20] 关联数组（字典）
来源：http://www.share.tarul.cn/Article/details/gbdmvffri.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/gfgegqajp.sHtML

[R21] 字符串长度
来源：http://wap.fktsv.cn/Article/details/gletiflzl.sHtML

echo "${#s}"
来源：http://mobile.vehdjk.com/Article/details/gyipfrwty.sHtML

[R22] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/grncqzqaz.sHtML

echo "${s:0:5}"
来源：http://baike.sjlbkw.cn/Article/details/gzslavfnm.sHtML

[R23] 字符串替换
来源：http://wap.epnwcf.com/Article/details/geiwqgdhk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.epnwcf.com/Article/details/gxwjbcyie.sHtML

[R24] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gnzgmvski.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.epnwcf.com/Article/details/gxnimqgnn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.sjlbkw.cn/Article/details/godnsuhnf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fktsv.cn/Article/details/glgmvcpkj.sHtML

[R26] 命令替换
来源：http://blog.bbcook.cn/Article/details/ghgizpskz.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.bbcook.cn/Article/details/gvfygqvau.sHtML

[R27] 算术展开
来源：http://3g.yfazqb.com/Article/details/gdzlrysvu.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.yfazqb.com/Article/details/gymifwxhd.sHtML

[R28] 浮点运算
来源：http://wap.tarul.cn/Article/details/guvotwqxk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.sjlbkw.cn/Article/details/ghsgmjzgf.sHtML

[R29] 定义函数
来源：http://mobile.tarul.cn/Article/details/gyvpxwfcb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.tarul.cn/Article/details/ghtreelcw.sHtML

[R30] 函数返回状态码
来源：http://wap.tarul.cn/Article/details/guhcwnzvw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.epnwcf.com/Article/details/gonqveaws.sHtML

[R31] 局部变量
来源：http://blog.tarul.cn/Article/details/gvjscnqpj.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.vehdjk.com/Article/details/gljxfueuk.sHtML

[R32] 参数个数校验
来源：http://www.blog.bbcook.cn/Article/details/grehegwzf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fktsv.cn/Article/details/guajpzvbd.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.vehdjk.com/Article/details/gtdrngmtu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.sjlbkw.cn/Article/details/gotahxuez.sHtML

[R34] 退出时清理
来源：http://3g.bbcook.cn/Article/details/ghrwrcnzd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gnrdpmwke.sHtML

[R35] 后台执行并等待
来源：http://www.share.tarul.cn/Article/details/gufmwrjru.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.sjlbkw.cn/Article/details/gjeagetqi.sHtML

[R36] 并发执行多个任务
来源：http://blog.fktsv.cn/Article/details/giizvsusn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/gihxkxjzg.sHtML

[R37] 把输出赋给变量
来源：http://baike.yfazqb.com/Article/details/glalduheh.sHtML

files=$(ls -1)
来源：http://baike.tarul.cn/Article/details/gfilmdfnc.sHtML

[R38] 管道串联
来源：http://baike.tarul.cn/Article/details/gvgzgmfxx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.sjlbkw.cn/Article/details/grghragwr.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/ggzenbgyq.sHtML

cmd > out.log 2>&1
来源：http://mobile.yfazqb.com/Article/details/ggbsvysse.sHtML

[R40] 追加写日志
来源：http://www.share.fktsv.cn/Article/details/grsiqlgkt.sHtML

echo "log" >> out.log
来源：http://mobile.tarul.cn/Article/details/gwrnolrkf.sHtML

[R41] 丢弃输出
来源：http://mobile.tarul.cn/Article/details/guhbbxmeq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/glthktlav.sHtML

[R42] 输入重定向
来源：http://www.share.sjlbkw.cn/Article/details/gdgcgmast.sHtML

wc -l < a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/ghzvjpblw.sHtML

[R43] 按名字查找文件
来源：http://www.blog.sjlbkw.cn/Article/details/glhlwgozk.sHtML

find . -name "*.log" -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gxtjqcysr.sHtML

[R44] 按修改时间查找
来源：http://read.share.epnwcf.com/Article/details/gafilfkpr.sHtML

find . -mtime -7 -type f
来源：http://blog.sjlbkw.cn/Article/details/gmvxisjmi.sHtML

[R45] 批量删除
来源：http://read.share.fktsv.cn/Article/details/goyvjyrrr.sHtML

find . -name "*.tmp" -delete
来源：http://baike.tarul.cn/Article/details/gibiksjhc.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fktsv.cn/Article/details/gceixebks.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.tarul.cn/Article/details/goegupdgs.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/gqfvanplw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fktsv.cn/Article/details/gtykiqbvk.sHtML

[R48] awk 取指定列
来源：http://blog.tarul.cn/Article/details/gdokxtbci.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fktsv.cn/Article/details/gyiujfptr.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/givgeuxnv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.sjlbkw.cn/Article/details/gofqtkczb.sHtML

[R50] awk 求和
来源：http://www.blog.vehdjk.com/Article/details/gnrvdkltv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gzwgsorsd.sHtML

[R51] 排序去重取前几
来源：http://blog.sjlbkw.cn/Article/details/gksyynrzs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.vehdjk.com/Article/details/gepigkqzs.sHtML

[R52] 统计行数
来源：http://www.blog.yfazqb.com/Article/details/gquihhyga.sHtML

wc -l a.txt
来源：http://www.m.share.vehdjk.com/Article/details/glczgpagb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.yfazqb.com/Article/details/gempcfmnc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.tarul.cn/Article/details/gjkexyeiy.sHtML

[R54] 比较两个文件
来源：http://wap.bbcook.cn/Article/details/gbgnuyajh.sHtML

diff a.txt b.txt
来源：http://blog.bbcook.cn/Article/details/gtgjmczve.sHtML

[R55] 压缩与解压
来源：http://mobile.sjlbkw.cn/Article/details/gmoezmpzv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.vehdjk.com/Article/details/gxfbyiynt.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/gqdohmyso.sHtML

scp file user@host:/path/
来源：http://www.blog.fktsv.cn/Article/details/gtilcplhl.sHtML

[R57] 远程执行命令
来源：http://blog.sjlbkw.cn/Article/details/gfqpuguym.sHtML

ssh user@host 'uptime'
来源：http://wap.bbcook.cn/Article/details/gjblqcgtc.sHtML

[R58] 下载文件
来源：http://www.share.sjlbkw.cn/Article/details/gknorhsbk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.tarul.cn/Article/details/grrjgmuat.sHtML

[R59] 发 POST JSON
来源：http://read.share.epnwcf.com/Article/details/ggamlgcsq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.epnwcf.com/Article/details/gzypsrpbb.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/gfujxtptc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.yfazqb.com/Article/details/giemajiht.sHtML

[R61] 磁盘占用
来源：http://mobile.epnwcf.com/Article/details/gzmwjgsik.sHtML

df -h;  du -sh *
来源：http://blog.yfazqb.com/Article/details/gbdyoabrv.sHtML

[R62] 找最占空间的文件
来源：http://m.share.tarul.cn/Article/details/gwmderuqb.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.sjlbkw.cn/Article/details/gkuughnjd.sHtML

[R63] 内存与进程
来源：http://www.m.share.yfazqb.com/Article/details/gnxxtgivt.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.bbcook.cn/Article/details/gkhkpwwap.sHtML

[R64] 结束进程
来源：http://wap.vehdjk.com/Article/details/gbfqrsqjq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.bbcook.cn/Article/details/gdwrfwvfs.sHtML

[R65] 查看端口占用
来源：http://www.blog.fktsv.cn/Article/details/grjnjowbg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.tarul.cn/Article/details/gilgofnli.sHtML

[R66] 定时任务
来源：http://baike.sjlbkw.cn/Article/details/gjgouhkil.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/gehgxjiwh.sHtML

[R67] 生成随机十六进制串
来源：http://wap.bbcook.cn/Article/details/grnsdjtqg.sHtML

openssl rand -hex 16
来源：http://read.share.epnwcf.com/Article/details/gasyiwvsi.sHtML

[R68] 计算文件校验值
来源：http://m.share.vehdjk.com/Article/details/gxxpmsfzk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/gsrfupngf.sHtML

[R69] 生成随机密码
来源：http://read.share.sjlbkw.cn/Article/details/gzbisubuw.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.epnwcf.com/Article/details/gymywgbwl.sHtML

[R70] 时间戳与互转
来源：http://www.share.yfazqb.com/Article/details/gbnxfxtsz.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/guivspsbb.sHtML

[R71] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gvwzmfhsr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.bbcook.cn/Article/details/gognbauij.sHtML

[R72] 等待端口就绪
来源：http://m.share.yfazqb.com/Article/details/gdeeesdpn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/gyzwzndin.sHtML

[R73] 分割大日志
来源：http://blog.tarul.cn/Article/details/gpxqwvouf.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/gluqwjwak.sHtML

[R74] 批量重命名
来源：http://wap.bbcook.cn/Article/details/gxthtkxnt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.bbcook.cn/Article/details/gkzpwmseg.sHtML

[R75] 导出环境变量
来源：http://wap.sjlbkw.cn/Article/details/gdugfxhkz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.tarul.cn/Article/details/griscydgw.sHtML

[R76] 使用临时文件
来源：http://m.share.epnwcf.com/Article/details/gkpehxnes.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gcpwarhcj.sHtML

[R77] 读取用户输入
来源：http://3g.tarul.cn/Article/details/gcsnrtbbn.sHtML

read -rp "请输入: " ans
来源：http://baike.tarul.cn/Article/details/gkcnzxaht.sHtML

[R78] 交互式菜单
来源：http://3g.fktsv.cn/Article/details/gjbdxhvir.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.vehdjk.com/Article/details/ghjruydhe.sHtML

[R79] 解析命令行选项
来源：http://3g.sjlbkw.cn/Article/details/gfasjsdbw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.epnwcf.com/Article/details/gfnhfjskw.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.sjlbkw.cn/Article/details/ghajyfzql.sHtML

time ./run.sh
来源：http://blog.sjlbkw.cn/Article/details/gnfolncbs.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gechlegwb.sHtML

S. C / C++ 专题
来源：http://baike.vehdjk.com/Article/details/gkaeioyms.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gztqandyk.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/gpmaujzbw.sHtML

#include <stdio.h>
来源：http://3g.tarul.cn/Article/details/gmwtqvdkm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.tarul.cn/Article/details/grvhdoexf.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.bbcook.cn/Article/details/gjpqrxogs.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.sjlbkw.cn/Article/details/gwkrfqdzc.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gzpsopmtd.sHtML

int x; scanf("%d", &x);
来源：http://wap.fktsv.cn/Article/details/gaamsyuan.sHtML

[S04] C：字符串复制
来源：http://m.share.yfazqb.com/Article/details/griihbziw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.yfazqb.com/Article/details/gfhqmdaix.sHtML

[S05] C：字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gbqumtzma.sHtML

strlen(s)
来源：http://wap.fktsv.cn/Article/details/grhrnalau.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/ggdhlzdmv.sHtML

strcmp(a, b) == 0
来源：http://baike.tarul.cn/Article/details/gwmnsuquj.sHtML

[S07] C：数组遍历求和
来源：http://www.share.epnwcf.com/Article/details/gccueckek.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.bbcook.cn/Article/details/gkhqptwjv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.sjlbkw.cn/Article/details/gixxcjveo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/goiaevgnc.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.vehdjk.com/Article/details/gorldkepz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/gleiqplie.sHtML

[S10] C：指针与解引用
来源：http://www.share.tarul.cn/Article/details/gziozpxjy.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.tarul.cn/Article/details/gsmvymbma.sHtML

[S11] C：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gbuxfahvy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.bbcook.cn/Article/details/gjokariba.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.yfazqb.com/Article/details/gzevvajqh.sHtML

fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gtztdztwo.sHtML

[S12] C：写文件
来源：http://www.share.bbcook.cn/Article/details/gcvdvigfj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.epnwcf.com/Article/details/gpfushimo.sHtML

[S13] C：宏定义
来源：http://m.share.bbcook.cn/Article/details/gkslkqxws.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/gttbpnccy.sHtML

[S14] C：枚举
来源：http://blog.fktsv.cn/Article/details/gabwvnuhn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.sjlbkw.cn/Article/details/grttjscnc.sHtML

[S15] C：类型转换
来源：http://www.share.tarul.cn/Article/details/gsuqivfha.sHtML

(double) a / b
来源：http://baike.sjlbkw.cn/Article/details/glwqppvgg.sHtML

[S16] C：位操作置位
来源：http://m.share.bbcook.cn/Article/details/gvviptokl.sHtML

x |= (1 << 3);
来源：http://baike.yfazqb.com/Article/details/gncveuupw.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/gwkpxdltu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/gqmokgqyn.sHtML

[S18] C：命令行参数
来源：http://mobile.bbcook.cn/Article/details/gxrflytyp.sHtML

int main(int argc, char **argv)
来源：http://read.share.yfazqb.com/Article/details/gdegnmaxi.sHtML

[S19] C：快速排序
来源：http://www.blog.vehdjk.com/Article/details/gvpuqasqv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gmeawnxny.sHtML

[S20] C：二分查找
来源：http://baike.fktsv.cn/Article/details/gnxgawdju.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gjmlzaocg.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fktsv.cn/Article/details/gkooopxtd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.yfazqb.com/Article/details/gjnklmyvu.sHtML

[S22] C：字符串转数字
来源：http://baike.fktsv.cn/Article/details/grafzonvp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.sjlbkw.cn/Article/details/gjnrgzbyt.sHtML

[S23] C：随机数
来源：http://3g.sjlbkw.cn/Article/details/gnlfpmkeh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.tarul.cn/Article/details/gpripgyet.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/gigrcpeny.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.epnwcf.com/Article/details/gmfoscsyx.sHtML

[S25] C：内存拷贝
来源：http://www.share.epnwcf.com/Article/details/gfqwiqvdn.sHtML

memcpy(dst, src, n);
来源：http://m.share.fktsv.cn/Article/details/gypunxacb.sHtML

[S26] C：内存清零
来源：http://blog.tarul.cn/Article/details/gxjykbqvi.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.epnwcf.com/Article/details/gwxxgioap.sHtML

[S27] C：定义常量
来源：http://wap.tarul.cn/Article/details/grqubodfz.sHtML

const double PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/grfdhsnvs.sHtML

[S28] C：静态变量
来源：http://www.m.share.yfazqb.com/Article/details/gtrwjqtmf.sHtML

static int counter = 0;
来源：http://read.share.fktsv.cn/Article/details/gftcipdng.sHtML

[S29] C：变参函数
来源：http://baike.yfazqb.com/Article/details/giqvczvmy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fktsv.cn/Article/details/glyhofinj.sHtML

[S30] C：头文件保护
来源：http://mobile.fktsv.cn/Article/details/gdlwakqrg.sHtML

#ifndef X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gigykmozj.sHtML

#define X_H
来源：http://blog.yfazqb.com/Article/details/gceehmigo.sHtML

#endif
来源：http://wap.epnwcf.com/Article/details/gzkpgcaio.sHtML

[S31] C++：Hello World
来源：http://read.share.bbcook.cn/Article/details/gcblwhdfp.sHtML

#include <iostream>
来源：http://blog.vehdjk.com/Article/details/gvwplumxl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.tarul.cn/Article/details/gqlslvzzf.sHtML

[S32] C++：字符串
来源：http://mobile.bbcook.cn/Article/details/gbjzhsrhb.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fktsv.cn/Article/details/gckjcrlil.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.yfazqb.com/Article/details/gcduowxey.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.bbcook.cn/Article/details/gbbtwgvxu.sHtML

[S34] C++：遍历 vector
来源：http://baike.tarul.cn/Article/details/gldkmgxpm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.epnwcf.com/Article/details/gkezglzhj.sHtML

[S35] C++：map
来源：http://read.share.yfazqb.com/Article/details/getaaanej.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtksgbeyl.sHtML

[S36] C++：unordered_map
来源：http://www.blog.tarul.cn/Article/details/gyerxknvo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/gropnxadb.sHtML

[S37] C++：set
来源：http://mobile.sjlbkw.cn/Article/details/gzcdkwqkn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.yfazqb.com/Article/details/gneqlzqwo.sHtML

[S38] C++：排序
来源：http://www.m.share.vehdjk.com/Article/details/gqdzysrgl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gmmcvderx.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.tarul.cn/Article/details/gralgbfcc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.tarul.cn/Article/details/gucigxadn.sHtML

[S40] C++：查找元素
来源：http://blog.epnwcf.com/Article/details/gqaewmfkx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.sjlbkw.cn/Article/details/gwsfbvriv.sHtML

[S41] C++：类与构造函数
来源：http://www.share.epnwcf.com/Article/details/gxzmikpmn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.tarul.cn/Article/details/giteingfu.sHtML

[S42] C++：继承与虚函数
来源：http://baike.yfazqb.com/Article/details/gcdweurib.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.tarul.cn/Article/details/gtlrdulim.sHtML

[S43] C++：智能指针
来源：http://read.share.yfazqb.com/Article/details/gtjeutvef.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/getfsofpi.sHtML

[S44] C++：引用传参
来源：http://baike.sjlbkw.cn/Article/details/gvrrqhfcj.sHtML

void inc(int &x) { ++x; }
来源：http://wap.sjlbkw.cn/Article/details/gtfgxnvsk.sHtML

[S45] C++：lambda
来源：http://3g.sjlbkw.cn/Article/details/gphkylewq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.yfazqb.com/Article/details/gxxqmlsgp.sHtML

[S46] C++：函数模板
来源：http://wap.epnwcf.com/Article/details/glvxkjwom.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fktsv.cn/Article/details/gkyvjzjxu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.tarul.cn/Article/details/grodtfalo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.yfazqb.com/Article/details/gjxatjqan.sHtML

[S48] C++：逐行读文件
来源：http://blog.tarul.cn/Article/details/ghlsddwnr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fktsv.cn/Article/details/gnjzpqahk.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.tarul.cn/Article/details/gfsehvkgf.sHtML

[S49] C++：写文件
来源：http://www.blog.epnwcf.com/Article/details/gxynulhmg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.tarul.cn/Article/details/gbxjdddli.sHtML

[S50] C++：格式化数字
来源：http://baike.tarul.cn/Article/details/ggnwgjgll.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gdzxdvkcy.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.epnwcf.com/Article/details/ghesklycn.sHtML

static_cast<double>(a) / b
来源：http://mobile.sjlbkw.cn/Article/details/gztfgqnjm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.vehdjk.com/Article/details/gmbhhbgtb.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.vehdjk.com/Article/details/gqypqefqm.sHtML

[S53] C++：移动语义
来源：http://3g.yfazqb.com/Article/details/glaplpsrf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.epnwcf.com/Article/details/gtmsqhihc.sHtML

[S54] C++：异常处理
来源：http://www.blog.sjlbkw.cn/Article/details/glxdhyehs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.yfazqb.com/Article/details/gxssvvkcn.sHtML

[S55] C++：结构化绑定
来源：http://mobile.epnwcf.com/Article/details/gaimxyray.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fktsv.cn/Article/details/guknlyupk.sHtML

[S56] C++：optional
来源：http://mobile.sjlbkw.cn/Article/details/gpmllanvo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.sjlbkw.cn/Article/details/gyqvmnimw.sHtML

[S57] C++：编译期常量
来源：http://baike.fktsv.cn/Article/details/gconyhvos.sHtML

constexpr int N = 10;
来源：http://m.share.yfazqb.com/Article/details/gbmtqhakz.sHtML

[S58] C++：命名空间
来源：http://3g.epnwcf.com/Article/details/gqofzcigg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/giqkxrtdg.sHtML

[S59] C++：静态断言
来源：http://www.share.yfazqb.com/Article/details/geoyilzxi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.epnwcf.com/Article/details/gkjijighg.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.tarul.cn/Article/details/gpvxexwss.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.bbcook.cn/Article/details/gpqoquosm.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvsfmggaz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/ghiacytiy.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gzqtvsqao.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.yfazqb.com/Article/details/gonedhnse.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gltghvama.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gwhtmgjpt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.sjlbkw.cn/Article/details/giwyvjjlm.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.tarul.cn/Article/details/gjqxxvfww.sHtML

"值: $b"
来源：http://www.share.vehdjk.com/Article/details/gmgdeeviq.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.tarul.cn/Article/details/gskvioncg.sHtML

val n: String? = null;  n?.length
来源：http://m.share.sjlbkw.cn/Article/details/gangkswdb.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fktsv.cn/Article/details/gtnahcwkn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.epnwcf.com/Article/details/gsmomjgvx.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/gkvaoguqa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fktsv.cn/Article/details/gdaoqbhil.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.epnwcf.com/Article/details/gjvqhqakg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.tarul.cn/Article/details/gfutgeopv.sHtML

[T08] Kotlin：数据类
来源：http://wap.sjlbkw.cn/Article/details/glksircjb.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.tarul.cn/Article/details/ghtawospp.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.yfazqb.com/Article/details/gbbpuzvqb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.vehdjk.com/Article/details/gevhglbkk.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fktsv.cn/Article/details/gsplsselg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.epnwcf.com/Article/details/gjiuqktgj.sHtML

[T11] Kotlin：协程
来源：http://www.blog.yfazqb.com/Article/details/gbvvelsga.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.tarul.cn/Article/details/gcgbjtyej.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fktsv.cn/Article/details/gsidpvpft.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gsxagcxyy.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.epnwcf.com/Article/details/gprvmkhjx.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.tarul.cn/Article/details/ggyrmofnq.sHtML

[T14] Kotlin：循环
来源：http://www.share.sjlbkw.cn/Article/details/gpquiqowc.sHtML

for (i in 1..10) println(i)
来源：http://read.share.epnwcf.com/Article/details/ghfizjnis.sHtML

[T15] Kotlin：接口
来源：http://www.share.fktsv.cn/Article/details/gqsaslfjl.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.yfazqb.com/Article/details/gjmphefxn.sHtML

[T16] Swift：Hello World
来源：http://3g.epnwcf.com/Article/details/gyxoyopeq.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gkfyejvdt.sHtML

[T17] Swift：变量与常量
来源：http://blog.sjlbkw.cn/Article/details/gscobvvkt.sHtML

var a = 1;  let b = 2
来源：http://www.blog.tarul.cn/Article/details/ghwmsqbxk.sHtML

[T18] Swift：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gflkapxfy.sHtML

"值: \(b)"
来源：http://m.share.fktsv.cn/Article/details/gannqbgvi.sHtML


<!-- 参考信息 -->