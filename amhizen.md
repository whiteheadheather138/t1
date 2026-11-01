代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.epnwcf.com/Article/details/gtnvltkbv.sHtML

[R16] until 等待条件
来源：http://mobile.tarul.cn/Article/details/gtjjhnhsd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/gcfqdrjeo.sHtML

[R17] 数组定义与取值
来源：http://wap.bbcook.cn/Article/details/grraqcheg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.bbcook.cn/Article/details/glrmxouqi.sHtML

[R18] 遍历数组
来源：http://mobile.tarul.cn/Article/details/gkaqlbvxo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.yfazqb.com/Article/details/gmuwatycq.sHtML

[R19] 数组长度
来源：http://m.share.fktsv.cn/Article/details/gaqcthfcs.sHtML

echo "${#arr[@]}"
来源：http://read.share.tarul.cn/Article/details/ghmjlonht.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fktsv.cn/Article/details/gktmlibfb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.sjlbkw.cn/Article/details/gczcgeagb.sHtML

[R21] 字符串长度
来源：http://blog.yfazqb.com/Article/details/gttylhpku.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/gvarnbirl.sHtML

[R22] 截取子串
来源：http://wap.vehdjk.com/Article/details/gtfwttxxw.sHtML

echo "${s:0:5}"
来源：http://3g.yfazqb.com/Article/details/ghwdeplhd.sHtML

[R23] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gtfexabnh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.bbcook.cn/Article/details/gmgejwosk.sHtML

[R24] 大小写转换
来源：http://blog.yfazqb.com/Article/details/gmdxgfdcj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.bbcook.cn/Article/details/gicidmdct.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.epnwcf.com/Article/details/ghfdbxabx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.vehdjk.com/Article/details/ggyljgxwj.sHtML

[R26] 命令替换
来源：http://mobile.yfazqb.com/Article/details/gmjgrjvqb.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.tarul.cn/Article/details/ghfzxqqsp.sHtML

[R27] 算术展开
来源：http://read.share.tarul.cn/Article/details/gskukvsdl.sHtML

echo $((1 + 2 * 3))
来源：http://wap.bbcook.cn/Article/details/gniyyywca.sHtML

[R28] 浮点运算
来源：http://mobile.tarul.cn/Article/details/gmkiauqwb.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/glqyueftj.sHtML

[R29] 定义函数
来源：http://blog.fktsv.cn/Article/details/gklroymdr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.epnwcf.com/Article/details/gknfkkxug.sHtML

[R30] 函数返回状态码
来源：http://m.share.epnwcf.com/Article/details/ghpuqylex.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.sjlbkw.cn/Article/details/gjsfeiilk.sHtML

[R31] 局部变量
来源：http://3g.fktsv.cn/Article/details/gyygbdjoe.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.epnwcf.com/Article/details/gdyuzcrah.sHtML

[R32] 参数个数校验
来源：http://www.blog.bbcook.cn/Article/details/gkqgwdthl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.tarul.cn/Article/details/gppdbfkti.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.sjlbkw.cn/Article/details/gmjymyjhq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.vehdjk.com/Article/details/geyazregn.sHtML

[R34] 退出时清理
来源：http://mobile.vehdjk.com/Article/details/ggqvlomjy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/grlhwqxjh.sHtML

[R35] 后台执行并等待
来源：http://mobile.tarul.cn/Article/details/giwknqfgg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.epnwcf.com/Article/details/grnrorhkx.sHtML

[R36] 并发执行多个任务
来源：http://wap.sjlbkw.cn/Article/details/gcjoakslz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.vehdjk.com/Article/details/gsvlmdhvj.sHtML

[R37] 把输出赋给变量
来源：http://read.share.bbcook.cn/Article/details/gjmaqeffv.sHtML

files=$(ls -1)
来源：http://3g.sjlbkw.cn/Article/details/gaqlehgtk.sHtML

[R38] 管道串联
来源：http://m.share.sjlbkw.cn/Article/details/ggclfmbpd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.epnwcf.com/Article/details/gujgcimfq.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.tarul.cn/Article/details/gnpsmhwej.sHtML

cmd > out.log 2>&1
来源：http://read.share.yfazqb.com/Article/details/gjmwixfun.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/gpksedlhg.sHtML

echo "log" >> out.log
来源：http://www.share.epnwcf.com/Article/details/gqywhoant.sHtML

[R41] 丢弃输出
来源：http://read.share.epnwcf.com/Article/details/ggfhjwttl.sHtML

cmd >/dev/null 2>&1
来源：http://wap.epnwcf.com/Article/details/gcbvixfch.sHtML

[R42] 输入重定向
来源：http://read.share.fktsv.cn/Article/details/gyilhvyop.sHtML

wc -l < a.txt
来源：http://3g.bbcook.cn/Article/details/goksbldoj.sHtML

[R43] 按名字查找文件
来源：http://read.share.bbcook.cn/Article/details/gdeqgybvl.sHtML

find . -name "*.log" -type f
来源：http://www.share.yfazqb.com/Article/details/gwdqjcpqo.sHtML

[R44] 按修改时间查找
来源：http://wap.fktsv.cn/Article/details/gwilgvxlh.sHtML

find . -mtime -7 -type f
来源：http://blog.tarul.cn/Article/details/gitgytwuz.sHtML

[R45] 批量删除
来源：http://www.m.share.fktsv.cn/Article/details/gpqpizffv.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fktsv.cn/Article/details/gqkydppxa.sHtML

[R46] 递归替换文件内容
来源：http://baike.yfazqb.com/Article/details/gsasthsnt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.sjlbkw.cn/Article/details/gedfrtesf.sHtML

[R47] sed 单行替换
来源：http://read.share.vehdjk.com/Article/details/grlilcmfb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.tarul.cn/Article/details/gtecokkao.sHtML

[R48] awk 取指定列
来源：http://m.share.epnwcf.com/Article/details/gufwvdifb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gfdocaual.sHtML

[R49] awk 带条件
来源：http://www.m.share.vehdjk.com/Article/details/gtvkawagn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.tarul.cn/Article/details/gtqfmmdci.sHtML

[R50] awk 求和
来源：http://wap.epnwcf.com/Article/details/gdkscpbsz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.vehdjk.com/Article/details/gqyakxgwz.sHtML

[R51] 排序去重取前几
来源：http://baike.epnwcf.com/Article/details/giiolspvl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.epnwcf.com/Article/details/gkhwtwyqx.sHtML

[R52] 统计行数
来源：http://www.m.share.vehdjk.com/Article/details/gybxinnoj.sHtML

wc -l a.txt
来源：http://baike.vehdjk.com/Article/details/gtryvjuqt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.bbcook.cn/Article/details/giiedawjw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.vehdjk.com/Article/details/goiagmdvv.sHtML

[R54] 比较两个文件
来源：http://blog.epnwcf.com/Article/details/gtnrtcosg.sHtML

diff a.txt b.txt
来源：http://wap.vehdjk.com/Article/details/gkzqrhlqd.sHtML

[R55] 压缩与解压
来源：http://read.share.tarul.cn/Article/details/gzuxwtdlq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.epnwcf.com/Article/details/gzqnhnjlu.sHtML

[R56] 远程拷贝
来源：http://mobile.vehdjk.com/Article/details/gzekqkyyy.sHtML

scp file user@host:/path/
来源：http://read.share.tarul.cn/Article/details/gkiooydfq.sHtML

[R57] 远程执行命令
来源：http://blog.epnwcf.com/Article/details/gjajanyub.sHtML

ssh user@host 'uptime'
来源：http://www.blog.bbcook.cn/Article/details/ghxnnxzrt.sHtML

[R58] 下载文件
来源：http://mobile.vehdjk.com/Article/details/gnmabahor.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.sjlbkw.cn/Article/details/gmkitqyam.sHtML

[R59] 发 POST JSON
来源：http://baike.vehdjk.com/Article/details/gvnanxudi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.yfazqb.com/Article/details/gfpnmxkua.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gegkynkax.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.bbcook.cn/Article/details/gkxmtoybk.sHtML

[R61] 磁盘占用
来源：http://www.blog.vehdjk.com/Article/details/ghjsuhgsw.sHtML

df -h;  du -sh *
来源：http://www.m.share.tarul.cn/Article/details/govnxhway.sHtML

[R62] 找最占空间的文件
来源：http://read.share.sjlbkw.cn/Article/details/gjzfnlnbb.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.bbcook.cn/Article/details/gmjxnfejd.sHtML

[R63] 内存与进程
来源：http://www.share.tarul.cn/Article/details/gsdqvmozb.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.tarul.cn/Article/details/gicrhylwl.sHtML

[R64] 结束进程
来源：http://read.share.epnwcf.com/Article/details/gpzygsdfs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.epnwcf.com/Article/details/gosjkyseu.sHtML

[R65] 查看端口占用
来源：http://read.share.yfazqb.com/Article/details/ghzvvesdm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.epnwcf.com/Article/details/gslzahwqu.sHtML

[R66] 定时任务
来源：http://m.share.epnwcf.com/Article/details/gzhiwctem.sHtML

crontab -e;  crontab -l
来源：http://www.blog.yfazqb.com/Article/details/gbovukbuw.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/gykbxorya.sHtML

openssl rand -hex 16
来源：http://m.share.vehdjk.com/Article/details/gygcmfzgi.sHtML

[R68] 计算文件校验值
来源：http://blog.vehdjk.com/Article/details/gdwqjokny.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.sjlbkw.cn/Article/details/getiolrvu.sHtML

[R69] 生成随机密码
来源：http://www.share.epnwcf.com/Article/details/gzajovaui.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.sjlbkw.cn/Article/details/gtyllmwsu.sHtML

[R70] 时间戳与互转
来源：http://wap.epnwcf.com/Article/details/gyvegpfym.sHtML

date +%s;  date -d @1700000000
来源：http://baike.sjlbkw.cn/Article/details/gvjtnuxkf.sHtML

[R71] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/gylwwownz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.sjlbkw.cn/Article/details/gkigzchxb.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.tarul.cn/Article/details/gwhrehrkn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnxpwbws.sHtML

[R73] 分割大日志
来源：http://www.m.share.fktsv.cn/Article/details/gndzthicu.sHtML

split -l 1000 big.log part_
来源：http://m.share.yfazqb.com/Article/details/gbnnepgoe.sHtML

[R74] 批量重命名
来源：http://read.share.tarul.cn/Article/details/gkuujnixw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.vehdjk.com/Article/details/gjcadaoak.sHtML

[R75] 导出环境变量
来源：http://blog.bbcook.cn/Article/details/ghodmkmbr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.sjlbkw.cn/Article/details/guavrsnsk.sHtML

[R76] 使用临时文件
来源：http://mobile.epnwcf.com/Article/details/gbaygjxnn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gkegrxncy.sHtML

[R77] 读取用户输入
来源：http://m.share.sjlbkw.cn/Article/details/gkfeibfkf.sHtML

read -rp "请输入: " ans
来源：http://read.share.bbcook.cn/Article/details/gwumhwszm.sHtML

[R78] 交互式菜单
来源：http://www.share.fktsv.cn/Article/details/gbftoetcv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.yfazqb.com/Article/details/gcrbaecpb.sHtML

[R79] 解析命令行选项
来源：http://3g.epnwcf.com/Article/details/gfgkfhqli.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.sjlbkw.cn/Article/details/gvfhsbiwz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.tarul.cn/Article/details/gbyjvkzwt.sHtML

time ./run.sh
来源：http://baike.yfazqb.com/Article/details/gavogifin.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtljoqntn.sHtML

S. C / C++ 专题
来源：http://www.share.yfazqb.com/Article/details/gvozgwpmg.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gftdhywfa.sHtML

[S01] C：Hello World
来源：http://baike.fktsv.cn/Article/details/giyzillxs.sHtML

#include <stdio.h>
来源：http://mobile.bbcook.cn/Article/details/gvneopaqn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.tarul.cn/Article/details/gguwaxjvu.sHtML

[S02] C：变量与格式化输出
来源：http://3g.yfazqb.com/Article/details/grssjmfip.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.epnwcf.com/Article/details/gjmxwufqi.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/gtjbnwkvz.sHtML

int x; scanf("%d", &x);
来源：http://mobile.epnwcf.com/Article/details/gaxqipcdx.sHtML

[S04] C：字符串复制
来源：http://3g.bbcook.cn/Article/details/gmxefbosk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gjunwixqw.sHtML

[S05] C：字符串长度
来源：http://baike.yfazqb.com/Article/details/gjamgomwk.sHtML

strlen(s)
来源：http://wap.sjlbkw.cn/Article/details/gbnkwjphz.sHtML

[S06] C：字符串比较
来源：http://blog.yfazqb.com/Article/details/gqgsrjguk.sHtML

strcmp(a, b) == 0
来源：http://www.share.sjlbkw.cn/Article/details/gpjuqwpoq.sHtML

[S07] C：数组遍历求和
来源：http://wap.tarul.cn/Article/details/gcrixaivt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.sjlbkw.cn/Article/details/gizwqwrkn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.sjlbkw.cn/Article/details/gbxnrqhse.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.vehdjk.com/Article/details/gtjnlwjjc.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.sjlbkw.cn/Article/details/giykyaayc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fktsv.cn/Article/details/gsxydiwvl.sHtML

[S10] C：指针与解引用
来源：http://www.blog.sjlbkw.cn/Article/details/glzxprses.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.epnwcf.com/Article/details/gezfybxso.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gseangqrx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.vehdjk.com/Article/details/gqmpgehxj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gmpdarqkn.sHtML

fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gcscegzor.sHtML

[S12] C：写文件
来源：http://www.share.sjlbkw.cn/Article/details/grfqiiwxo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.tarul.cn/Article/details/gjslcllic.sHtML

[S13] C：宏定义
来源：http://blog.epnwcf.com/Article/details/giixlstgw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.yfazqb.com/Article/details/gohiinzsx.sHtML

[S14] C：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gopwzlear.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.vehdjk.com/Article/details/gzjijqrvi.sHtML

[S15] C：类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gzkscbxgh.sHtML

(double) a / b
来源：http://blog.tarul.cn/Article/details/gpmjeyaqx.sHtML

[S16] C：位操作置位
来源：http://www.blog.vehdjk.com/Article/details/gzcwgtzgz.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/gmxatgpig.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gatfjexdq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.tarul.cn/Article/details/gskywmdek.sHtML

[S18] C：命令行参数
来源：http://3g.tarul.cn/Article/details/glhcxqcoi.sHtML

int main(int argc, char **argv)
来源：http://www.blog.bbcook.cn/Article/details/gkcbutnil.sHtML

[S19] C：快速排序
来源：http://read.share.yfazqb.com/Article/details/gsxsvtivh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/grbqlwcnr.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/guntduvoj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/ggzfxsdpp.sHtML

[S21] C：字符类别判断
来源：http://baike.tarul.cn/Article/details/gxehpkraf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/gwqriqbtr.sHtML

[S22] C：字符串转数字
来源：http://www.share.bbcook.cn/Article/details/godeyrdta.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/gnioxzuhj.sHtML

[S23] C：随机数
来源：http://read.share.tarul.cn/Article/details/ghavmqepl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.vehdjk.com/Article/details/gomzcehnt.sHtML

[S24] C：获取本地时间
来源：http://www.share.bbcook.cn/Article/details/gqrqignvg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.epnwcf.com/Article/details/gcisfctlc.sHtML

[S25] C：内存拷贝
来源：http://mobile.vehdjk.com/Article/details/gqkamxouy.sHtML

memcpy(dst, src, n);
来源：http://baike.bbcook.cn/Article/details/ghovgzgrq.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/gveskrzqc.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/gvqwoqdnl.sHtML

[S27] C：定义常量
来源：http://read.share.sjlbkw.cn/Article/details/gbgsaiecs.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gfriiiray.sHtML

[S28] C：静态变量
来源：http://baike.bbcook.cn/Article/details/gxdxnuezz.sHtML

static int counter = 0;
来源：http://baike.yfazqb.com/Article/details/gghswuvlp.sHtML

[S29] C：变参函数
来源：http://www.blog.fktsv.cn/Article/details/gjpktttbf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.epnwcf.com/Article/details/gyrwyxbfv.sHtML

[S30] C：头文件保护
来源：http://read.share.tarul.cn/Article/details/grfldntrt.sHtML

#ifndef X_H
来源：http://baike.vehdjk.com/Article/details/gjwshafbv.sHtML

#define X_H
来源：http://www.share.tarul.cn/Article/details/grzrfuybq.sHtML

#endif
来源：http://read.share.vehdjk.com/Article/details/gabuqfbbu.sHtML

[S31] C++：Hello World
来源：http://read.share.epnwcf.com/Article/details/gouvyztzc.sHtML

#include <iostream>
来源：http://3g.tarul.cn/Article/details/gbtuybehy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.epnwcf.com/Article/details/gofplqtuh.sHtML

[S32] C++：字符串
来源：http://www.m.share.yfazqb.com/Article/details/gmjdmezqk.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.yfazqb.com/Article/details/griaosykx.sHtML

[S33] C++：vector 增删
来源：http://read.share.epnwcf.com/Article/details/gdctkjrfv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.bbcook.cn/Article/details/gkclqhbkc.sHtML

[S34] C++：遍历 vector
来源：http://baike.tarul.cn/Article/details/gmuxgrdnk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.sjlbkw.cn/Article/details/giwmyezlp.sHtML

[S35] C++：map
来源：http://3g.epnwcf.com/Article/details/gzydjvpfr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gnxocbgeb.sHtML

[S36] C++：unordered_map
来源：http://wap.epnwcf.com/Article/details/gdolwjheo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gggcrlhjz.sHtML

[S37] C++：set
来源：http://wap.epnwcf.com/Article/details/gvhbbqism.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.bbcook.cn/Article/details/gmgkeokoj.sHtML

[S38] C++：排序
来源：http://read.share.tarul.cn/Article/details/gwxqqolso.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gsvdjxckx.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.vehdjk.com/Article/details/gskaxkifa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.yfazqb.com/Article/details/goxpuwect.sHtML

[S40] C++：查找元素
来源：http://mobile.fktsv.cn/Article/details/gneaywucv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.sjlbkw.cn/Article/details/gqgyvqois.sHtML

[S41] C++：类与构造函数
来源：http://baike.sjlbkw.cn/Article/details/ghxhvnkri.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.yfazqb.com/Article/details/ghufzrezx.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/ghbjnfpyi.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gnvkgnvmb.sHtML

[S43] C++：智能指针
来源：http://m.share.sjlbkw.cn/Article/details/ghaofflcq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gnjhkkfbw.sHtML

[S44] C++：引用传参
来源：http://read.share.fktsv.cn/Article/details/gjckcmpkz.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.yfazqb.com/Article/details/gmpluizzu.sHtML

[S45] C++：lambda
来源：http://www.m.share.tarul.cn/Article/details/gadeimado.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.epnwcf.com/Article/details/gpbylhryj.sHtML

[S46] C++：函数模板
来源：http://baike.bbcook.cn/Article/details/gvjufylnv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fktsv.cn/Article/details/gpzjggyyl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gskaazfho.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.epnwcf.com/Article/details/giponjvfo.sHtML

[S48] C++：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gkhfimgog.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.yfazqb.com/Article/details/ghheqbtdy.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.yfazqb.com/Article/details/gcimojnbe.sHtML

[S49] C++：写文件
来源：http://blog.vehdjk.com/Article/details/gbjujtjbd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.tarul.cn/Article/details/ggcstfnho.sHtML

[S50] C++：格式化数字
来源：http://m.share.vehdjk.com/Article/details/goiktbltf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fktsv.cn/Article/details/grpakouyw.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fktsv.cn/Article/details/gmwzcouxd.sHtML

static_cast<double>(a) / b
来源：http://read.share.epnwcf.com/Article/details/gfscgmvrc.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.yfazqb.com/Article/details/gkcotckjx.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.bbcook.cn/Article/details/gjzxzppex.sHtML

[S53] C++：移动语义
来源：http://blog.sjlbkw.cn/Article/details/gtsvtybgc.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.bbcook.cn/Article/details/ghbvnpxez.sHtML

[S54] C++：异常处理
来源：http://baike.sjlbkw.cn/Article/details/gaorwadpt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.tarul.cn/Article/details/gthygaisn.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.tarul.cn/Article/details/gbrlieyfl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.epnwcf.com/Article/details/gdoqbdcyy.sHtML

[S56] C++：optional
来源：http://blog.sjlbkw.cn/Article/details/goxjwatot.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.sjlbkw.cn/Article/details/gjxyfqcdz.sHtML

[S57] C++：编译期常量
来源：http://www.share.vehdjk.com/Article/details/gpeohsqab.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/ghrdgrwpd.sHtML

[S58] C++：命名空间
来源：http://wap.fktsv.cn/Article/details/gecebnkdt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.bbcook.cn/Article/details/glekdgbuy.sHtML

[S59] C++：静态断言
来源：http://www.blog.yfazqb.com/Article/details/gotvxlrhm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fktsv.cn/Article/details/gmwswgcxe.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.tarul.cn/Article/details/gzbkzkmnr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.bbcook.cn/Article/details/gssgzsgyz.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/geoppapoc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/gstdmzbfi.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ghpcgeotd.sHtML

[T01] Kotlin：Hello World
来源：http://3g.vehdjk.com/Article/details/ggljbnqav.sHtML

println("Hello")
来源：http://wap.fktsv.cn/Article/details/gtsrktvca.sHtML

[T02] Kotlin：变量
来源：http://baike.fktsv.cn/Article/details/gslbcatvw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.sjlbkw.cn/Article/details/gowdexxeo.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.yfazqb.com/Article/details/giplijojr.sHtML

"值: $b"
来源：http://baike.epnwcf.com/Article/details/gdppwvuyu.sHtML

[T04] Kotlin：空安全
来源：http://read.share.tarul.cn/Article/details/gsryffdxk.sHtML

val n: String? = null;  n?.length
来源：http://blog.bbcook.cn/Article/details/gyicpyhee.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.tarul.cn/Article/details/gwioccvbp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbhjklpj.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.vehdjk.com/Article/details/gitrfeigb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.bbcook.cn/Article/details/gpqlhitbj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fktsv.cn/Article/details/glgucoeja.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fktsv.cn/Article/details/gzhjqrwnt.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.yfazqb.com/Article/details/gvhtbyhuo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/gqsoiutjp.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.yfazqb.com/Article/details/ghjqaalxw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.sjlbkw.cn/Article/details/glffvtgec.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fktsv.cn/Article/details/gvxyeyrrf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.yfazqb.com/Article/details/ggmxdlhbp.sHtML

[T11] Kotlin：协程
来源：http://baike.bbcook.cn/Article/details/grxyisirj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.tarul.cn/Article/details/ghltxambb.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.tarul.cn/Article/details/ghfhxbjpa.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.tarul.cn/Article/details/gvvzdwrly.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fktsv.cn/Article/details/gytilgnds.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.epnwcf.com/Article/details/gtrxfwxzf.sHtML

[T14] Kotlin：循环
来源：http://mobile.fktsv.cn/Article/details/gtkkrbznv.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/goqczlufe.sHtML

[T15] Kotlin：接口
来源：http://baike.fktsv.cn/Article/details/gkkzuzlwh.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.yfazqb.com/Article/details/gsmbgscxs.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/gwcfbwvnb.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/gudmyothv.sHtML

[T17] Swift：变量与常量
来源：http://wap.epnwcf.com/Article/details/gqdouneky.sHtML

var a = 1;  let b = 2
来源：http://m.share.fktsv.cn/Article/details/goerrpius.sHtML

[T18] Swift：字符串插值
来源：http://blog.fktsv.cn/Article/details/gcyzfyiqm.sHtML

"值: \(b)"
来源：http://read.share.yfazqb.com/Article/details/gzdkwiuml.sHtML


<!-- 参考信息 -->