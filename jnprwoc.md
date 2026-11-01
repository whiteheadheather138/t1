代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/gsjpbxjcq.sHtML

[R14] C 风格 for
来源：http://wap.yfazqb.com/Article/details/gdftmrqhz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gggmktbso.sHtML

[R15] while 逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gqmnrkgio.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.yfazqb.com/Article/details/guhjgxybx.sHtML

[R16] until 等待条件
来源：http://mobile.fktsv.cn/Article/details/gpqqwoihj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gufowkvny.sHtML

[R17] 数组定义与取值
来源：http://m.share.tarul.cn/Article/details/ghdypflam.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/guyokgezt.sHtML

[R18] 遍历数组
来源：http://wap.vehdjk.com/Article/details/gqoajrqzg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fktsv.cn/Article/details/gywcpkuyb.sHtML

[R19] 数组长度
来源：http://m.share.bbcook.cn/Article/details/gdqdoocan.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/gblssahgq.sHtML

[R20] 关联数组（字典）
来源：http://blog.fktsv.cn/Article/details/gvfxvsjya.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.sjlbkw.cn/Article/details/gsdkfvwit.sHtML

[R21] 字符串长度
来源：http://baike.epnwcf.com/Article/details/gqtjnpzbi.sHtML

echo "${#s}"
来源：http://read.share.fktsv.cn/Article/details/gcauwmudu.sHtML

[R22] 截取子串
来源：http://wap.epnwcf.com/Article/details/gvisumzac.sHtML

echo "${s:0:5}"
来源：http://read.share.tarul.cn/Article/details/gigxfngjz.sHtML

[R23] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gcmnokgpt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.vehdjk.com/Article/details/gohuxoevj.sHtML

[R24] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gqpqgsliy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.epnwcf.com/Article/details/gagzqapln.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fktsv.cn/Article/details/gzqtholsf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.sjlbkw.cn/Article/details/giogmfytb.sHtML

[R26] 命令替换
来源：http://m.share.yfazqb.com/Article/details/gzkfhlqib.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fktsv.cn/Article/details/gfhfdmvks.sHtML

[R27] 算术展开
来源：http://baike.fktsv.cn/Article/details/gvwgppixp.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.vehdjk.com/Article/details/gsziemqlr.sHtML

[R28] 浮点运算
来源：http://www.share.yfazqb.com/Article/details/gxhthoess.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.yfazqb.com/Article/details/gvcpdzrof.sHtML

[R29] 定义函数
来源：http://www.blog.tarul.cn/Article/details/gpeporamc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.vehdjk.com/Article/details/gwhuqdyuf.sHtML

[R30] 函数返回状态码
来源：http://m.share.bbcook.cn/Article/details/gtchvvczi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.vehdjk.com/Article/details/gwkggroge.sHtML

[R31] 局部变量
来源：http://read.share.sjlbkw.cn/Article/details/gwlcugqto.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.epnwcf.com/Article/details/grcmvwujo.sHtML

[R32] 参数个数校验
来源：http://read.share.epnwcf.com/Article/details/gelwtacpd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/gdgiysmhx.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.bbcook.cn/Article/details/gofrwmhef.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.sjlbkw.cn/Article/details/gxyovhtkz.sHtML

[R34] 退出时清理
来源：http://baike.tarul.cn/Article/details/goqqlbnmm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gtpjpdrub.sHtML

[R35] 后台执行并等待
来源：http://3g.sjlbkw.cn/Article/details/ggjezpuos.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.yfazqb.com/Article/details/grvdgxhdn.sHtML

[R36] 并发执行多个任务
来源：http://m.share.yfazqb.com/Article/details/gypashxii.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/gosyvhcnr.sHtML

[R37] 把输出赋给变量
来源：http://baike.epnwcf.com/Article/details/goxatjcgl.sHtML

files=$(ls -1)
来源：http://baike.epnwcf.com/Article/details/gamhkvvqf.sHtML

[R38] 管道串联
来源：http://m.share.tarul.cn/Article/details/gncaxqghd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fktsv.cn/Article/details/gkopkisrt.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.tarul.cn/Article/details/gxlsqtjoq.sHtML

cmd > out.log 2>&1
来源：http://www.share.fktsv.cn/Article/details/gmwigtcxl.sHtML

[R40] 追加写日志
来源：http://www.share.fktsv.cn/Article/details/gpgkclzfe.sHtML

echo "log" >> out.log
来源：http://baike.sjlbkw.cn/Article/details/gpvmjeism.sHtML

[R41] 丢弃输出
来源：http://baike.bbcook.cn/Article/details/gfrvwfoba.sHtML

cmd >/dev/null 2>&1
来源：http://3g.epnwcf.com/Article/details/gmpwqehpm.sHtML

[R42] 输入重定向
来源：http://mobile.fktsv.cn/Article/details/gwbdzmisu.sHtML

wc -l < a.txt
来源：http://wap.vehdjk.com/Article/details/gwpepzkps.sHtML

[R43] 按名字查找文件
来源：http://3g.tarul.cn/Article/details/gbftjwngw.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fktsv.cn/Article/details/gnxlwpoxp.sHtML

[R44] 按修改时间查找
来源：http://read.share.fktsv.cn/Article/details/gcsnyqhvp.sHtML

find . -mtime -7 -type f
来源：http://m.share.fktsv.cn/Article/details/gmaiqcwvv.sHtML

[R45] 批量删除
来源：http://mobile.epnwcf.com/Article/details/gubrcmffb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.epnwcf.com/Article/details/gqkixvhxg.sHtML

[R46] 递归替换文件内容
来源：http://baike.fktsv.cn/Article/details/gbithmwtd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.epnwcf.com/Article/details/guecuhiwb.sHtML

[R47] sed 单行替换
来源：http://www.blog.fktsv.cn/Article/details/geudoarke.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.bbcook.cn/Article/details/gsdfcvvri.sHtML

[R48] awk 取指定列
来源：http://wap.fktsv.cn/Article/details/gxdvklzjc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gdgvmepbx.sHtML

[R49] awk 带条件
来源：http://wap.bbcook.cn/Article/details/grxjdesxt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fktsv.cn/Article/details/gkjzmxsbh.sHtML

[R50] awk 求和
来源：http://baike.fktsv.cn/Article/details/gebtconcd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.tarul.cn/Article/details/gjnqrvuec.sHtML

[R51] 排序去重取前几
来源：http://blog.yfazqb.com/Article/details/gboyglhpr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.bbcook.cn/Article/details/gxemiorps.sHtML

[R52] 统计行数
来源：http://blog.vehdjk.com/Article/details/gabpxpjas.sHtML

wc -l a.txt
来源：http://baike.tarul.cn/Article/details/gwfvnjxps.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.tarul.cn/Article/details/girovrcyi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.sjlbkw.cn/Article/details/gvlkxmemk.sHtML

[R54] 比较两个文件
来源：http://read.share.sjlbkw.cn/Article/details/gcjknyzaj.sHtML

diff a.txt b.txt
来源：http://read.share.sjlbkw.cn/Article/details/gcalhhkwv.sHtML

[R55] 压缩与解压
来源：http://wap.bbcook.cn/Article/details/gcneoqqfp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/gqedkwada.sHtML

[R56] 远程拷贝
来源：http://baike.vehdjk.com/Article/details/gwlptylih.sHtML

scp file user@host:/path/
来源：http://blog.sjlbkw.cn/Article/details/gplyopquv.sHtML

[R57] 远程执行命令
来源：http://baike.vehdjk.com/Article/details/gofngokha.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gtuoligfc.sHtML

[R58] 下载文件
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxpifaez.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.epnwcf.com/Article/details/gtfqpgahl.sHtML

[R59] 发 POST JSON
来源：http://blog.epnwcf.com/Article/details/gnjsudrvc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.tarul.cn/Article/details/gvcwemkqn.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/guhlqfczj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.yfazqb.com/Article/details/ggtkxxpis.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/giovbfsgx.sHtML

df -h;  du -sh *
来源：http://baike.epnwcf.com/Article/details/glslnnmrl.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/giegehnky.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.bbcook.cn/Article/details/gfpipvala.sHtML

[R63] 内存与进程
来源：http://wap.tarul.cn/Article/details/gtgdylqhk.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.yfazqb.com/Article/details/gxxklyfuk.sHtML

[R64] 结束进程
来源：http://www.m.share.fktsv.cn/Article/details/ggcbqcabo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fktsv.cn/Article/details/gbbfjyqgh.sHtML

[R65] 查看端口占用
来源：http://wap.epnwcf.com/Article/details/ggrjacvhk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.vehdjk.com/Article/details/grqdjadpx.sHtML

[R66] 定时任务
来源：http://www.blog.fktsv.cn/Article/details/glpjzdggo.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/gzuhyjtiy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.tarul.cn/Article/details/gnttnnmmj.sHtML

openssl rand -hex 16
来源：http://www.m.share.yfazqb.com/Article/details/gvfgwukpk.sHtML

[R68] 计算文件校验值
来源：http://www.share.tarul.cn/Article/details/ghjfyomgo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.tarul.cn/Article/details/gmcaoypkd.sHtML

[R69] 生成随机密码
来源：http://3g.sjlbkw.cn/Article/details/glstswxmf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.epnwcf.com/Article/details/gutnfjfig.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/gwvteaoch.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.yfazqb.com/Article/details/gjuiazyii.sHtML

[R71] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gasltdish.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.yfazqb.com/Article/details/ghnarhwfj.sHtML

[R72] 等待端口就绪
来源：http://www.blog.sjlbkw.cn/Article/details/gctkteyie.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/gyyorjaae.sHtML

[R73] 分割大日志
来源：http://read.share.vehdjk.com/Article/details/gwcfqkuet.sHtML

split -l 1000 big.log part_
来源：http://www.share.sjlbkw.cn/Article/details/gaoyayaim.sHtML

[R74] 批量重命名
来源：http://read.share.vehdjk.com/Article/details/gatqesrdk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.yfazqb.com/Article/details/gjxdivjiz.sHtML

[R75] 导出环境变量
来源：http://baike.sjlbkw.cn/Article/details/gpmazcapo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fktsv.cn/Article/details/gumtjsfew.sHtML

[R76] 使用临时文件
来源：http://baike.fktsv.cn/Article/details/gmuoqybwx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gvxooqpdh.sHtML

[R77] 读取用户输入
来源：http://m.share.tarul.cn/Article/details/ggynoxhyw.sHtML

read -rp "请输入: " ans
来源：http://read.share.bbcook.cn/Article/details/gcdfrpzvt.sHtML

[R78] 交互式菜单
来源：http://www.share.tarul.cn/Article/details/glxblestt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fktsv.cn/Article/details/gflzjnbbz.sHtML

[R79] 解析命令行选项
来源：http://3g.yfazqb.com/Article/details/goqqaddcs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fktsv.cn/Article/details/gsywiiusf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.vehdjk.com/Article/details/gtutmovpm.sHtML

time ./run.sh
来源：http://mobile.tarul.cn/Article/details/glfjioknv.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gplqzueny.sHtML

S. C / C++ 专题
来源：http://wap.fktsv.cn/Article/details/gdqhoeycm.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvpkobhbr.sHtML

[S01] C：Hello World
来源：http://blog.tarul.cn/Article/details/gimoibyuw.sHtML

#include <stdio.h>
来源：http://www.share.fktsv.cn/Article/details/gvbtehrdj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/glimgxrgb.sHtML

[S02] C：变量与格式化输出
来源：http://blog.tarul.cn/Article/details/guatxuoqb.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.epnwcf.com/Article/details/gguwsylsy.sHtML

[S03] C：读入整数
来源：http://m.share.sjlbkw.cn/Article/details/gguxmbmwq.sHtML

int x; scanf("%d", &x);
来源：http://wap.fktsv.cn/Article/details/gfqjttjfc.sHtML

[S04] C：字符串复制
来源：http://www.blog.bbcook.cn/Article/details/gxzfjekia.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.epnwcf.com/Article/details/gnqgpgexl.sHtML

[S05] C：字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/grtudybob.sHtML

strlen(s)
来源：http://www.m.share.fktsv.cn/Article/details/gbnrzsedc.sHtML

[S06] C：字符串比较
来源：http://read.share.fktsv.cn/Article/details/gaplvdzqz.sHtML

strcmp(a, b) == 0
来源：http://3g.bbcook.cn/Article/details/gpqsihtbz.sHtML

[S07] C：数组遍历求和
来源：http://baike.bbcook.cn/Article/details/gqkwuibba.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/gqvunxwli.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.yfazqb.com/Article/details/gnvhqpgdb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fktsv.cn/Article/details/goowqcmvq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.tarul.cn/Article/details/gdxeajzvt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fktsv.cn/Article/details/gqycssshs.sHtML

[S10] C：指针与解引用
来源：http://wap.epnwcf.com/Article/details/gzmfvzlhm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.sjlbkw.cn/Article/details/gatxntdgt.sHtML

[S11] C：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gepoictin.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fktsv.cn/Article/details/gvakobjlp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.tarul.cn/Article/details/gwdztsojr.sHtML

fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gtduihggn.sHtML

[S12] C：写文件
来源：http://wap.bbcook.cn/Article/details/gzirgxqsq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.epnwcf.com/Article/details/grmmfezbl.sHtML

[S13] C：宏定义
来源：http://www.share.vehdjk.com/Article/details/gpytaswhb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.bbcook.cn/Article/details/gdqiieoey.sHtML

[S14] C：枚举
来源：http://www.blog.bbcook.cn/Article/details/gudkawydb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.tarul.cn/Article/details/gvcwqwrpk.sHtML

[S15] C：类型转换
来源：http://mobile.fktsv.cn/Article/details/gkdknwwvx.sHtML

(double) a / b
来源：http://baike.vehdjk.com/Article/details/guwknzkia.sHtML

[S16] C：位操作置位
来源：http://wap.yfazqb.com/Article/details/gcazthpuq.sHtML

x |= (1 << 3);
来源：http://read.share.fktsv.cn/Article/details/gxmdfyxtn.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.tarul.cn/Article/details/gflimmasz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.sjlbkw.cn/Article/details/geendjhxr.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/gssokqscc.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/gwuzsiomc.sHtML

[S19] C：快速排序
来源：http://wap.tarul.cn/Article/details/gtobhtcos.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gbzmsbgsk.sHtML

[S20] C：二分查找
来源：http://3g.vehdjk.com/Article/details/gmznwjjoq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gispzvsot.sHtML

[S21] C：字符类别判断
来源：http://www.blog.bbcook.cn/Article/details/gxknelzgw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.sjlbkw.cn/Article/details/ggnauvnzy.sHtML

[S22] C：字符串转数字
来源：http://mobile.bbcook.cn/Article/details/gmrxgeosu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.epnwcf.com/Article/details/gxypyffpg.sHtML

[S23] C：随机数
来源：http://read.share.yfazqb.com/Article/details/gzrpqyywx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.tarul.cn/Article/details/gdhryzpeg.sHtML

[S24] C：获取本地时间
来源：http://www.blog.vehdjk.com/Article/details/glzfwkhcb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fktsv.cn/Article/details/gbbnbxmne.sHtML

[S25] C：内存拷贝
来源：http://www.blog.epnwcf.com/Article/details/gyzfcqgoh.sHtML

memcpy(dst, src, n);
来源：http://read.share.fktsv.cn/Article/details/gfmtayeng.sHtML

[S26] C：内存清零
来源：http://m.share.bbcook.cn/Article/details/guzfpiasc.sHtML

memset(a, 0, sizeof a);
来源：http://blog.tarul.cn/Article/details/gdnargrkm.sHtML

[S27] C：定义常量
来源：http://mobile.vehdjk.com/Article/details/glrysfdgy.sHtML

const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/ghhmwetep.sHtML

[S28] C：静态变量
来源：http://m.share.tarul.cn/Article/details/goziyqrrk.sHtML

static int counter = 0;
来源：http://read.share.bbcook.cn/Article/details/geobljbwq.sHtML

[S29] C：变参函数
来源：http://www.blog.fktsv.cn/Article/details/gpwewejom.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.vehdjk.com/Article/details/gimxosyot.sHtML

[S30] C：头文件保护
来源：http://mobile.epnwcf.com/Article/details/gnrfpxcui.sHtML

#ifndef X_H
来源：http://m.share.yfazqb.com/Article/details/gwfqjannj.sHtML

#define X_H
来源：http://www.m.share.tarul.cn/Article/details/gborqsjak.sHtML

#endif
来源：http://mobile.tarul.cn/Article/details/guansbquq.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gasercutg.sHtML

#include <iostream>
来源：http://www.m.share.sjlbkw.cn/Article/details/godlvivto.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fktsv.cn/Article/details/geaqcyebq.sHtML

[S32] C++：字符串
来源：http://blog.bbcook.cn/Article/details/gmrfxgyfw.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.sjlbkw.cn/Article/details/gweqnbitw.sHtML

[S33] C++：vector 增删
来源：http://blog.tarul.cn/Article/details/gxfpranka.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/ghnpklbxe.sHtML

[S34] C++：遍历 vector
来源：http://wap.bbcook.cn/Article/details/gvwroobnd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.yfazqb.com/Article/details/gzvitnefd.sHtML

[S35] C++：map
来源：http://3g.fktsv.cn/Article/details/gsggieugg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/guwxjrecd.sHtML

[S36] C++：unordered_map
来源：http://baike.epnwcf.com/Article/details/guqpptwlk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gszcingbb.sHtML

[S37] C++：set
来源：http://www.m.share.tarul.cn/Article/details/grbvhiafc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/gfnahrtrk.sHtML

[S38] C++：排序
来源：http://3g.tarul.cn/Article/details/gxkelvhms.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.yfazqb.com/Article/details/gkrwfilji.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.vehdjk.com/Article/details/giccgvmyw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.sjlbkw.cn/Article/details/gjubjymqe.sHtML

[S40] C++：查找元素
来源：http://read.share.yfazqb.com/Article/details/ghdsqielc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/gomsnsdwq.sHtML

[S41] C++：类与构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gpxpwtcto.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.vehdjk.com/Article/details/genqfxgul.sHtML

[S42] C++：继承与虚函数
来源：http://baike.vehdjk.com/Article/details/gfsfhdpsr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fktsv.cn/Article/details/ghgtcmouh.sHtML

[S43] C++：智能指针
来源：http://www.m.share.vehdjk.com/Article/details/gahrildwp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.yfazqb.com/Article/details/gcrztajqr.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/gdbpowanv.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.bbcook.cn/Article/details/gehfosmme.sHtML

[S45] C++：lambda
来源：http://baike.vehdjk.com/Article/details/gzikptgoy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.epnwcf.com/Article/details/gjippkkyw.sHtML

[S46] C++：函数模板
来源：http://baike.fktsv.cn/Article/details/gdwsjhiyw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.sjlbkw.cn/Article/details/gsixniqen.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.bbcook.cn/Article/details/glbtzcgki.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.bbcook.cn/Article/details/gothbsytd.sHtML

[S48] C++：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/genkbxpgy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.epnwcf.com/Article/details/gehoexayp.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.tarul.cn/Article/details/gajhnohql.sHtML

[S49] C++：写文件
来源：http://3g.epnwcf.com/Article/details/gwcfsfvum.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/glcienptt.sHtML

[S50] C++：格式化数字
来源：http://read.share.vehdjk.com/Article/details/gfvjzwogq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.tarul.cn/Article/details/gghvxckkm.sHtML

[S51] C++：显式类型转换
来源：http://www.share.bbcook.cn/Article/details/gvxzhjyyf.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gstfzwtdk.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.tarul.cn/Article/details/gvyxnhrul.sHtML

int size() const noexcept { return n_; }
来源：http://baike.sjlbkw.cn/Article/details/gnrezvkpr.sHtML

[S53] C++：移动语义
来源：http://www.blog.fktsv.cn/Article/details/gbjfkjfwh.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.vehdjk.com/Article/details/gnabmdgki.sHtML

[S54] C++：异常处理
来源：http://www.share.yfazqb.com/Article/details/glpwcuhde.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.sjlbkw.cn/Article/details/gkxrqlwec.sHtML

[S55] C++：结构化绑定
来源：http://blog.fktsv.cn/Article/details/gzyvtmujz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fktsv.cn/Article/details/gghyeeptq.sHtML

[S56] C++：optional
来源：http://www.blog.yfazqb.com/Article/details/gbbuilbji.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fktsv.cn/Article/details/gxbtvpsqx.sHtML

[S57] C++：编译期常量
来源：http://blog.sjlbkw.cn/Article/details/gmaaoywvs.sHtML

constexpr int N = 10;
来源：http://m.share.epnwcf.com/Article/details/gyastynlx.sHtML

[S58] C++：命名空间
来源：http://wap.fktsv.cn/Article/details/gfelwjyru.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.epnwcf.com/Article/details/gddwofoce.sHtML

[S59] C++：静态断言
来源：http://baike.tarul.cn/Article/details/giqceoehy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.yfazqb.com/Article/details/gcuxbpbho.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gfomkypsy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.epnwcf.com/Article/details/ggqwhvuiz.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gvfzmselj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.tarul.cn/Article/details/gpcfzvqpp.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmhyyybbd.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.tarul.cn/Article/details/gvkwddoig.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gkbgpzgtq.sHtML

[T02] Kotlin：变量
来源：http://m.share.epnwcf.com/Article/details/geropthlk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.epnwcf.com/Article/details/gqyywsknx.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.yfazqb.com/Article/details/gighgkpcj.sHtML

"值: $b"
来源：http://www.share.bbcook.cn/Article/details/ggohvdtxw.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/gxdbnigbe.sHtML

val n: String? = null;  n?.length
来源：http://mobile.vehdjk.com/Article/details/guttcomar.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.tarul.cn/Article/details/guhbpskcx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.tarul.cn/Article/details/gctunlclc.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fktsv.cn/Article/details/gbzcenykr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.epnwcf.com/Article/details/gvhgucjis.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gbxhwsjsy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gdlxzmdbh.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fktsv.cn/Article/details/ghplptdjg.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.epnwcf.com/Article/details/glphwlhwx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/gjogurteb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.tarul.cn/Article/details/gferpylfd.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.yfazqb.com/Article/details/gzpydftte.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.epnwcf.com/Article/details/glkqrfwbj.sHtML

[T11] Kotlin：协程
来源：http://mobile.vehdjk.com/Article/details/ghbdwmgsh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.tarul.cn/Article/details/gunrvyquh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.tarul.cn/Article/details/gpzfzstwp.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.tarul.cn/Article/details/gwtoaxejs.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.yfazqb.com/Article/details/gozzrcxcw.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.bbcook.cn/Article/details/glxeeajds.sHtML

[T14] Kotlin：循环
来源：http://baike.epnwcf.com/Article/details/gowzijoju.sHtML

for (i in 1..10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gbuwewonm.sHtML

[T15] Kotlin：接口
来源：http://www.blog.yfazqb.com/Article/details/guvxmgojh.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fktsv.cn/Article/details/gdybqpkwi.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gxyzswilb.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gvvrlayio.sHtML


<!-- 参考信息 -->