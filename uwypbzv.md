代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.vehdjk.com/Article/details/grskzdzeh.sHtML

[R16] until 等待条件
来源：http://www.m.share.vehdjk.com/Article/details/grijalqmi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/ggbllysfi.sHtML

[R17] 数组定义与取值
来源：http://read.share.epnwcf.com/Article/details/grgjwpuyo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/goazwekmc.sHtML

[R18] 遍历数组
来源：http://blog.fktsv.cn/Article/details/gezmikhuc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.sjlbkw.cn/Article/details/gdbhjtebi.sHtML

[R19] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gcslmfptk.sHtML

echo "${#arr[@]}"
来源：http://www.share.sjlbkw.cn/Article/details/gnolrabin.sHtML

[R20] 关联数组（字典）
来源：http://mobile.vehdjk.com/Article/details/glxjseqms.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.tarul.cn/Article/details/gqtinmeiv.sHtML

[R21] 字符串长度
来源：http://read.share.fktsv.cn/Article/details/ghszhgahp.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/gygfxxwbb.sHtML

[R22] 截取子串
来源：http://m.share.epnwcf.com/Article/details/gofjelevq.sHtML

echo "${s:0:5}"
来源：http://3g.vehdjk.com/Article/details/grcshnwqu.sHtML

[R23] 字符串替换
来源：http://blog.yfazqb.com/Article/details/gyfnyalxa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.sjlbkw.cn/Article/details/gdespwezj.sHtML

[R24] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/glbolvryb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fktsv.cn/Article/details/gooenzldr.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.tarul.cn/Article/details/gpipbxqet.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.tarul.cn/Article/details/gsqlpsxsd.sHtML

[R26] 命令替换
来源：http://www.m.share.tarul.cn/Article/details/guxrlfxnv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.epnwcf.com/Article/details/gaghpnurj.sHtML

[R27] 算术展开
来源：http://www.blog.vehdjk.com/Article/details/gstbpbpav.sHtML

echo $((1 + 2 * 3))
来源：http://3g.vehdjk.com/Article/details/gsiecbbuq.sHtML

[R28] 浮点运算
来源：http://3g.sjlbkw.cn/Article/details/gcqvdysdy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.epnwcf.com/Article/details/gtsgxojlw.sHtML

[R29] 定义函数
来源：http://read.share.epnwcf.com/Article/details/gqlsycycn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.vehdjk.com/Article/details/gtdtbnfga.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.vehdjk.com/Article/details/gqrgfczcs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fktsv.cn/Article/details/gwlaxkklq.sHtML

[R31] 局部变量
来源：http://baike.epnwcf.com/Article/details/gnupkrzxh.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.tarul.cn/Article/details/ggysmgwuq.sHtML

[R32] 参数个数校验
来源：http://read.share.vehdjk.com/Article/details/gepruuxxc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.bbcook.cn/Article/details/grcbhsuhv.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.yfazqb.com/Article/details/gkkrrjoft.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.bbcook.cn/Article/details/grlinhsid.sHtML

[R34] 退出时清理
来源：http://www.blog.bbcook.cn/Article/details/gchoohyqw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.vehdjk.com/Article/details/gpfqfekge.sHtML

[R35] 后台执行并等待
来源：http://m.share.fktsv.cn/Article/details/gyykgfaqy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.vehdjk.com/Article/details/gewcidbss.sHtML

[R36] 并发执行多个任务
来源：http://m.share.epnwcf.com/Article/details/gbmmkbvip.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.yfazqb.com/Article/details/glffhsbxs.sHtML

[R37] 把输出赋给变量
来源：http://baike.bbcook.cn/Article/details/guoxdkmld.sHtML

files=$(ls -1)
来源：http://baike.yfazqb.com/Article/details/gnidbgnan.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/gqgwyzfjf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.bbcook.cn/Article/details/gahhrchax.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.epnwcf.com/Article/details/gjyytarsh.sHtML

cmd > out.log 2>&1
来源：http://m.share.yfazqb.com/Article/details/giawtvrpp.sHtML

[R40] 追加写日志
来源：http://read.share.yfazqb.com/Article/details/guhusnnsx.sHtML

echo "log" >> out.log
来源：http://mobile.sjlbkw.cn/Article/details/gcotruoyn.sHtML

[R41] 丢弃输出
来源：http://3g.tarul.cn/Article/details/guycmqezq.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gpgcpsjyc.sHtML

[R42] 输入重定向
来源：http://m.share.epnwcf.com/Article/details/gysuztlvc.sHtML

wc -l < a.txt
来源：http://www.m.share.epnwcf.com/Article/details/geqwxvgic.sHtML

[R43] 按名字查找文件
来源：http://baike.epnwcf.com/Article/details/gxpxpjahm.sHtML

find . -name "*.log" -type f
来源：http://3g.bbcook.cn/Article/details/gbytzkxxe.sHtML

[R44] 按修改时间查找
来源：http://blog.tarul.cn/Article/details/gmuaixcsy.sHtML

find . -mtime -7 -type f
来源：http://www.share.epnwcf.com/Article/details/grcfjglon.sHtML

[R45] 批量删除
来源：http://www.share.tarul.cn/Article/details/gbfpfijrg.sHtML

find . -name "*.tmp" -delete
来源：http://3g.sjlbkw.cn/Article/details/glmsoajih.sHtML

[R46] 递归替换文件内容
来源：http://mobile.sjlbkw.cn/Article/details/guiwipfdy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.vehdjk.com/Article/details/gatnopjwl.sHtML

[R47] sed 单行替换
来源：http://baike.fktsv.cn/Article/details/gxxwxenmr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gunyuruwt.sHtML

[R48] awk 取指定列
来源：http://3g.sjlbkw.cn/Article/details/gkwghgrzc.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.tarul.cn/Article/details/gqgllljsb.sHtML

[R49] awk 带条件
来源：http://3g.fktsv.cn/Article/details/gtcsniucn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.epnwcf.com/Article/details/gwbuivuqc.sHtML

[R50] awk 求和
来源：http://wap.bbcook.cn/Article/details/ghfbcrney.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.vehdjk.com/Article/details/ggnujbaof.sHtML

[R51] 排序去重取前几
来源：http://read.share.tarul.cn/Article/details/gfybtzgvf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.epnwcf.com/Article/details/ggvmwxcsf.sHtML

[R52] 统计行数
来源：http://mobile.vehdjk.com/Article/details/gqjvoohjm.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/gyzjdhssv.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.epnwcf.com/Article/details/gyopalqgd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.sjlbkw.cn/Article/details/gizjgwwxq.sHtML

[R54] 比较两个文件
来源：http://www.share.epnwcf.com/Article/details/grazxktsh.sHtML

diff a.txt b.txt
来源：http://wap.tarul.cn/Article/details/gsfpwmvor.sHtML

[R55] 压缩与解压
来源：http://m.share.tarul.cn/Article/details/gjdzfwabj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.epnwcf.com/Article/details/gprhgfplt.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/glybkbbfn.sHtML

scp file user@host:/path/
来源：http://3g.tarul.cn/Article/details/gmcnfhdiy.sHtML

[R57] 远程执行命令
来源：http://blog.vehdjk.com/Article/details/gebtlhenl.sHtML

ssh user@host 'uptime'
来源：http://www.share.tarul.cn/Article/details/gzbeehpuo.sHtML

[R58] 下载文件
来源：http://3g.bbcook.cn/Article/details/gewidkmzo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.yfazqb.com/Article/details/gnzoiquyo.sHtML

[R59] 发 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gfzmitzkp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/guwretbmi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gkihuchfc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.tarul.cn/Article/details/gdgyraads.sHtML

[R61] 磁盘占用
来源：http://read.share.fktsv.cn/Article/details/gvbbjmtxs.sHtML

df -h;  du -sh *
来源：http://m.share.epnwcf.com/Article/details/gumxschhk.sHtML

[R62] 找最占空间的文件
来源：http://blog.vehdjk.com/Article/details/gjxruasjp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.sjlbkw.cn/Article/details/guryrniwp.sHtML

[R63] 内存与进程
来源：http://wap.vehdjk.com/Article/details/gdvuwxsmo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyyfbhke.sHtML

[R64] 结束进程
来源：http://read.share.vehdjk.com/Article/details/gxhugfuag.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.bbcook.cn/Article/details/gohzygxta.sHtML

[R65] 查看端口占用
来源：http://3g.sjlbkw.cn/Article/details/gqmgjlcxm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.bbcook.cn/Article/details/gwnwzbspo.sHtML

[R66] 定时任务
来源：http://read.share.yfazqb.com/Article/details/goaebnhei.sHtML

crontab -e;  crontab -l
来源：http://baike.fktsv.cn/Article/details/gtbsvgvtv.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzjpfuka.sHtML

openssl rand -hex 16
来源：http://read.share.epnwcf.com/Article/details/gumxmuznk.sHtML

[R68] 计算文件校验值
来源：http://m.share.tarul.cn/Article/details/gaqtgyxxz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.vehdjk.com/Article/details/gszegzmnm.sHtML

[R69] 生成随机密码
来源：http://www.m.share.vehdjk.com/Article/details/gcdmabems.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/gaigocxqo.sHtML

[R70] 时间戳与互转
来源：http://3g.vehdjk.com/Article/details/ghjcumpkm.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.sjlbkw.cn/Article/details/gvlhlkbxq.sHtML

[R71] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gufrvfnog.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.epnwcf.com/Article/details/goscratew.sHtML

[R72] 等待端口就绪
来源：http://blog.yfazqb.com/Article/details/glxokyufl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/guysjbujd.sHtML

[R73] 分割大日志
来源：http://blog.yfazqb.com/Article/details/gtbxapupg.sHtML

split -l 1000 big.log part_
来源：http://www.blog.tarul.cn/Article/details/grtvcivpl.sHtML

[R74] 批量重命名
来源：http://www.share.vehdjk.com/Article/details/gdwtqktdz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.epnwcf.com/Article/details/gbcscbdll.sHtML

[R75] 导出环境变量
来源：http://m.share.yfazqb.com/Article/details/gcbhlwsrl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.yfazqb.com/Article/details/guxxipxqf.sHtML

[R76] 使用临时文件
来源：http://wap.tarul.cn/Article/details/gqnapwzar.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gbbdhclmw.sHtML

[R77] 读取用户输入
来源：http://mobile.vehdjk.com/Article/details/gykizkxix.sHtML

read -rp "请输入: " ans
来源：http://mobile.fktsv.cn/Article/details/gpojycsfz.sHtML

[R78] 交互式菜单
来源：http://wap.tarul.cn/Article/details/gybgbkwyd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.epnwcf.com/Article/details/gftiozcby.sHtML

[R79] 解析命令行选项
来源：http://www.share.sjlbkw.cn/Article/details/gnuqdbenj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.yfazqb.com/Article/details/gidvurejr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fktsv.cn/Article/details/gxwwdtcyc.sHtML

time ./run.sh
来源：http://mobile.yfazqb.com/Article/details/gmlebifet.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwzpsbqeu.sHtML

S. C / C++ 专题
来源：http://wap.yfazqb.com/Article/details/gatxvtilz.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gaujqzilm.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/gaetfiikg.sHtML

#include <stdio.h>
来源：http://baike.tarul.cn/Article/details/glmdqhaxb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/getxkofhc.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.yfazqb.com/Article/details/gjbejnmwi.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.yfazqb.com/Article/details/gmlyfhsyp.sHtML

[S03] C：读入整数
来源：http://m.share.vehdjk.com/Article/details/gjropicks.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gosqzlklu.sHtML

[S04] C：字符串复制
来源：http://www.blog.fktsv.cn/Article/details/gxhfgjaib.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.vehdjk.com/Article/details/gqgucnxqb.sHtML

[S05] C：字符串长度
来源：http://3g.vehdjk.com/Article/details/gskyuwfxy.sHtML

strlen(s)
来源：http://mobile.bbcook.cn/Article/details/gpmgmzflu.sHtML

[S06] C：字符串比较
来源：http://www.share.bbcook.cn/Article/details/gmyvsbojl.sHtML

strcmp(a, b) == 0
来源：http://3g.tarul.cn/Article/details/gebucdgur.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gulrokcor.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.tarul.cn/Article/details/ghohcfmsr.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.vehdjk.com/Article/details/gpwbpqeuo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fktsv.cn/Article/details/gqbmvsfiu.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.vehdjk.com/Article/details/glcydjlrk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.vehdjk.com/Article/details/gzoyzlqgn.sHtML

[S10] C：指针与解引用
来源：http://baike.tarul.cn/Article/details/guffxinor.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.tarul.cn/Article/details/gkrbihwuk.sHtML

[S11] C：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gmxhtidnx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fktsv.cn/Article/details/gkiuchrxy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gbhtxbzce.sHtML

fclose(f);
来源：http://www.share.vehdjk.com/Article/details/ghvlfffts.sHtML

[S12] C：写文件
来源：http://baike.epnwcf.com/Article/details/gorrdjefi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.epnwcf.com/Article/details/gbdvjzudn.sHtML

[S13] C：宏定义
来源：http://m.share.bbcook.cn/Article/details/gbxsyopsv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.tarul.cn/Article/details/gguknaqkz.sHtML

[S14] C：枚举
来源：http://www.blog.epnwcf.com/Article/details/gtopywker.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.yfazqb.com/Article/details/gqqbdbbfj.sHtML

[S15] C：类型转换
来源：http://baike.epnwcf.com/Article/details/gsktscfnh.sHtML

(double) a / b
来源：http://baike.yfazqb.com/Article/details/grgmhqpil.sHtML

[S16] C：位操作置位
来源：http://www.m.share.tarul.cn/Article/details/gummqspyv.sHtML

x |= (1 << 3);
来源：http://www.share.vehdjk.com/Article/details/gdpxqjknl.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gcchqzsug.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.yfazqb.com/Article/details/gpatpwhrp.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/gmnsuigfc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.yfazqb.com/Article/details/gwxdxihbg.sHtML

[S19] C：快速排序
来源：http://read.share.fktsv.cn/Article/details/grquezyyh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/grmimnspq.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gtyncbbzn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gpxzdmles.sHtML

[S21] C：字符类别判断
来源：http://blog.fktsv.cn/Article/details/gysngonco.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.sjlbkw.cn/Article/details/gjqgqnycv.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gctmirfln.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.epnwcf.com/Article/details/gtdlvyhro.sHtML

[S23] C：随机数
来源：http://mobile.sjlbkw.cn/Article/details/gumgelsoi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fktsv.cn/Article/details/ghiwxfbll.sHtML

[S24] C：获取本地时间
来源：http://read.share.vehdjk.com/Article/details/gsiqxlgdz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.epnwcf.com/Article/details/givvkrewm.sHtML

[S25] C：内存拷贝
来源：http://www.share.yfazqb.com/Article/details/guzrwyebz.sHtML

memcpy(dst, src, n);
来源：http://mobile.yfazqb.com/Article/details/gjouohqgn.sHtML

[S26] C：内存清零
来源：http://read.share.tarul.cn/Article/details/gqtaqxppa.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gklbjtdpj.sHtML

[S27] C：定义常量
来源：http://wap.sjlbkw.cn/Article/details/gbfuchntl.sHtML

const double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gozsvhsxf.sHtML

[S28] C：静态变量
来源：http://www.m.share.yfazqb.com/Article/details/gkwpdbafw.sHtML

static int counter = 0;
来源：http://www.blog.epnwcf.com/Article/details/ggbnjfhhq.sHtML

[S29] C：变参函数
来源：http://read.share.yfazqb.com/Article/details/gpjrwnqwr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.sjlbkw.cn/Article/details/gfewjnqbt.sHtML

[S30] C：头文件保护
来源：http://www.blog.yfazqb.com/Article/details/gdzfpxrwm.sHtML

#ifndef X_H
来源：http://www.share.yfazqb.com/Article/details/gzfknldwf.sHtML

#define X_H
来源：http://read.share.fktsv.cn/Article/details/gdztszjhw.sHtML

#endif
来源：http://blog.vehdjk.com/Article/details/getxixxzs.sHtML

[S31] C++：Hello World
来源：http://read.share.yfazqb.com/Article/details/guphafjfn.sHtML

#include <iostream>
来源：http://m.share.sjlbkw.cn/Article/details/gjinskuzo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.tarul.cn/Article/details/gkenjbnjr.sHtML

[S32] C++：字符串
来源：http://m.share.epnwcf.com/Article/details/goqttqvnu.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.yfazqb.com/Article/details/ggikovjvn.sHtML

[S33] C++：vector 增删
来源：http://mobile.tarul.cn/Article/details/gghesggpk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/guoqamjki.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.sjlbkw.cn/Article/details/gwbdrprkd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.tarul.cn/Article/details/gjhmmrerc.sHtML

[S35] C++：map
来源：http://blog.yfazqb.com/Article/details/gyoavfrtd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gkagrwdwp.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.vehdjk.com/Article/details/gbigdwden.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/gxtqoorxy.sHtML

[S37] C++：set
来源：http://mobile.epnwcf.com/Article/details/gtjurhipx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.vehdjk.com/Article/details/gnpcdblhn.sHtML

[S38] C++：排序
来源：http://read.share.yfazqb.com/Article/details/gajmjzxht.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.bbcook.cn/Article/details/gbdyrxbat.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.tarul.cn/Article/details/gypifmqal.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.sjlbkw.cn/Article/details/grijhkqhz.sHtML

[S40] C++：查找元素
来源：http://mobile.tarul.cn/Article/details/guohhqrgg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gnqgayhir.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fktsv.cn/Article/details/gvmtsvifu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.sjlbkw.cn/Article/details/ghmujnsxc.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.tarul.cn/Article/details/gndjijicg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.tarul.cn/Article/details/gmvljlzww.sHtML

[S43] C++：智能指针
来源：http://blog.epnwcf.com/Article/details/gfkxjvsuo.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.epnwcf.com/Article/details/gfbiahyao.sHtML

[S44] C++：引用传参
来源：http://wap.yfazqb.com/Article/details/gjrgzsctc.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/grrmqybdc.sHtML

[S45] C++：lambda
来源：http://read.share.epnwcf.com/Article/details/gsqkcjcrp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.epnwcf.com/Article/details/gcsogappm.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/gdlzygzpc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.tarul.cn/Article/details/gyvmrtymn.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fktsv.cn/Article/details/gbarhcwju.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.epnwcf.com/Article/details/gwjqeoonl.sHtML

[S48] C++：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gpfswauto.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.tarul.cn/Article/details/gecnjrpnx.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.bbcook.cn/Article/details/gbqlyksyb.sHtML

[S49] C++：写文件
来源：http://www.blog.epnwcf.com/Article/details/gmfqihnwj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fktsv.cn/Article/details/gzifeddzf.sHtML

[S50] C++：格式化数字
来源：http://www.share.tarul.cn/Article/details/ggvhuxelx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/ghapvyqas.sHtML

[S51] C++：显式类型转换
来源：http://3g.sjlbkw.cn/Article/details/gnstqpkyw.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/gesmyknhb.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.bbcook.cn/Article/details/gbnzhstir.sHtML

int size() const noexcept { return n_; }
来源：http://baike.yfazqb.com/Article/details/gpobrmxoz.sHtML

[S53] C++：移动语义
来源：http://wap.yfazqb.com/Article/details/gztefujfk.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.vehdjk.com/Article/details/gxdjtisla.sHtML

[S54] C++：异常处理
来源：http://read.share.epnwcf.com/Article/details/gzeysmlgb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gtqjxahvx.sHtML

[S55] C++：结构化绑定
来源：http://mobile.vehdjk.com/Article/details/gbjzpqwnj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fktsv.cn/Article/details/gbuyimbwb.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/gcpglsypr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.bbcook.cn/Article/details/ghvomgsgf.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.tarul.cn/Article/details/gutzrspfj.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqlwpluu.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gvgdrrqxw.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.yfazqb.com/Article/details/ggnvbcxpd.sHtML

[S59] C++：静态断言
来源：http://read.share.sjlbkw.cn/Article/details/ggltsweed.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.tarul.cn/Article/details/gathopgww.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.yfazqb.com/Article/details/gepcxglbr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/gqethyliu.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gsopachrh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.epnwcf.com/Article/details/gklpomygl.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gopxglhlo.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.yfazqb.com/Article/details/glfiocmyz.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gwngojixy.sHtML

[T02] Kotlin：变量
来源：http://www.blog.epnwcf.com/Article/details/gryxrbrvu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.sjlbkw.cn/Article/details/gryvtmnog.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.vehdjk.com/Article/details/gtzvtssdn.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/ghgtbvayz.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/gwwhivygu.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gyefzgxbl.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.bbcook.cn/Article/details/gyxniezph.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.tarul.cn/Article/details/gseuetzra.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fktsv.cn/Article/details/gystmxwuo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.bbcook.cn/Article/details/gglgksnqb.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.yfazqb.com/Article/details/gdlopkcbg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.vehdjk.com/Article/details/gngknadqt.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.vehdjk.com/Article/details/gpopeiulk.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gctwukotj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.yfazqb.com/Article/details/guygozrwt.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.sjlbkw.cn/Article/details/gntgihvkn.sHtML

[T10] Kotlin：默认参数
来源：http://3g.yfazqb.com/Article/details/gfhgojday.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.sjlbkw.cn/Article/details/gxjojdbtb.sHtML

[T11] Kotlin：协程
来源：http://www.share.epnwcf.com/Article/details/getmhyrhl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fktsv.cn/Article/details/gbzbkapxo.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fktsv.cn/Article/details/grrpchcwi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.tarul.cn/Article/details/gzqyoxqla.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.vehdjk.com/Article/details/gxscdqptd.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.epnwcf.com/Article/details/gcefopeav.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.epnwcf.com/Article/details/gsmvhxwak.sHtML

for (i in 1..10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/gfyhzbffd.sHtML

[T15] Kotlin：接口
来源：http://www.blog.epnwcf.com/Article/details/gtnzbnxdq.sHtML

interface Shape { fun area(): Double }
来源：http://3g.bbcook.cn/Article/details/gkuyaabwt.sHtML

[T16] Swift：Hello World
来源：http://read.share.epnwcf.com/Article/details/gnvftheqk.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gcvcflusq.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.epnwcf.com/Article/details/gqcqkyrka.sHtML

var a = 1;  let b = 2
来源：http://wap.bbcook.cn/Article/details/gcgnsjrxd.sHtML

[T18] Swift：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gzkrrrdrk.sHtML

"值: \(b)"
来源：http://m.share.tarul.cn/Article/details/gtordyutj.sHtML


<!-- 参考信息 -->