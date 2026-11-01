代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/glwxfkncb.sHtML

[R14] C 风格 for
来源：http://blog.sjlbkw.cn/Article/details/gkzvbfwws.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/gtlplwxrj.sHtML

[R15] while 逐行读文件
来源：http://m.share.fktsv.cn/Article/details/ghhzemxnh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.tarul.cn/Article/details/ghfzwsgcr.sHtML

[R16] until 等待条件
来源：http://baike.tarul.cn/Article/details/gqywhacnt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gazjeolsk.sHtML

[R17] 数组定义与取值
来源：http://baike.fktsv.cn/Article/details/ghslxueoh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.epnwcf.com/Article/details/gcdpmxjuy.sHtML

[R18] 遍历数组
来源：http://www.share.sjlbkw.cn/Article/details/gsiltmhks.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.sjlbkw.cn/Article/details/gxedemfoq.sHtML

[R19] 数组长度
来源：http://www.share.vehdjk.com/Article/details/giqxfzgjs.sHtML

echo "${#arr[@]}"
来源：http://www.share.vehdjk.com/Article/details/gvjzoqgja.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fktsv.cn/Article/details/guyuqgwvi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.yfazqb.com/Article/details/gqofzfdzs.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/gilemuwmx.sHtML

echo "${#s}"
来源：http://wap.sjlbkw.cn/Article/details/gqgvencdz.sHtML

[R22] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gcmpigaig.sHtML

echo "${s:0:5}"
来源：http://m.share.bbcook.cn/Article/details/gaptjpnfv.sHtML

[R23] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gyynvgtff.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.epnwcf.com/Article/details/gkkghmntz.sHtML

[R24] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gidmbkxrb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.tarul.cn/Article/details/glbbwzrzn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.sjlbkw.cn/Article/details/gzibahzam.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.sjlbkw.cn/Article/details/gbuucrukg.sHtML

[R26] 命令替换
来源：http://m.share.epnwcf.com/Article/details/gtxhgsviy.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.bbcook.cn/Article/details/gzezviizq.sHtML

[R27] 算术展开
来源：http://baike.yfazqb.com/Article/details/gysxfixwp.sHtML

echo $((1 + 2 * 3))
来源：http://wap.epnwcf.com/Article/details/gqcpqzfph.sHtML

[R28] 浮点运算
来源：http://baike.epnwcf.com/Article/details/gkeeitxjl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fktsv.cn/Article/details/gnxvrorqg.sHtML

[R29] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/gdatulgrq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.vehdjk.com/Article/details/gzgnohogj.sHtML

[R30] 函数返回状态码
来源：http://mobile.bbcook.cn/Article/details/gqpmaftfx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fktsv.cn/Article/details/gqvpygvwc.sHtML

[R31] 局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gwbswcubk.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.yfazqb.com/Article/details/gfenfvpeq.sHtML

[R32] 参数个数校验
来源：http://blog.tarul.cn/Article/details/gkiwwtxbi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gnztawmss.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.vehdjk.com/Article/details/gzcqskrtw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fktsv.cn/Article/details/geqkwlkoa.sHtML

[R34] 退出时清理
来源：http://baike.fktsv.cn/Article/details/gtpxgyrns.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.bbcook.cn/Article/details/ggfmuikch.sHtML

[R35] 后台执行并等待
来源：http://baike.bbcook.cn/Article/details/gjfidqtkf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.tarul.cn/Article/details/gqhughzdf.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/gjjbbbmyy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.sjlbkw.cn/Article/details/gebmzdyhm.sHtML

[R37] 把输出赋给变量
来源：http://baike.tarul.cn/Article/details/gfehmwjyb.sHtML

files=$(ls -1)
来源：http://wap.sjlbkw.cn/Article/details/gzoxncnpb.sHtML

[R38] 管道串联
来源：http://blog.sjlbkw.cn/Article/details/gzqawmsai.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.vehdjk.com/Article/details/gkvjuunqb.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.yfazqb.com/Article/details/gxninfhjd.sHtML

cmd > out.log 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gzuizizlm.sHtML

[R40] 追加写日志
来源：http://www.share.yfazqb.com/Article/details/gryeqwzvq.sHtML

echo "log" >> out.log
来源：http://3g.vehdjk.com/Article/details/gpubcyyae.sHtML

[R41] 丢弃输出
来源：http://m.share.sjlbkw.cn/Article/details/gqbsioand.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/gpjshlzih.sHtML

[R42] 输入重定向
来源：http://baike.bbcook.cn/Article/details/gcxkkksjv.sHtML

wc -l < a.txt
来源：http://blog.yfazqb.com/Article/details/gthuzcdfa.sHtML

[R43] 按名字查找文件
来源：http://www.share.fktsv.cn/Article/details/gvcrrgzlh.sHtML

find . -name "*.log" -type f
来源：http://read.share.yfazqb.com/Article/details/gkmpxpptm.sHtML

[R44] 按修改时间查找
来源：http://read.share.yfazqb.com/Article/details/gfesteibh.sHtML

find . -mtime -7 -type f
来源：http://m.share.vehdjk.com/Article/details/gzwycejlb.sHtML

[R45] 批量删除
来源：http://www.m.share.vehdjk.com/Article/details/gicnwnpqa.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.yfazqb.com/Article/details/gtlfrgluh.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.sjlbkw.cn/Article/details/gthtgdypl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.bbcook.cn/Article/details/gvadefwej.sHtML

[R47] sed 单行替换
来源：http://wap.vehdjk.com/Article/details/grzaqzxot.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gehvwwbca.sHtML

[R48] awk 取指定列
来源：http://m.share.tarul.cn/Article/details/gzxyxvxog.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.epnwcf.com/Article/details/gbnixuavy.sHtML

[R49] awk 带条件
来源：http://3g.fktsv.cn/Article/details/glqexjiqg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.vehdjk.com/Article/details/gjvmmlpas.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/gelzkztzh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gdwsvjixh.sHtML

[R51] 排序去重取前几
来源：http://mobile.vehdjk.com/Article/details/gvdojvvhq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.sjlbkw.cn/Article/details/gzebdealx.sHtML

[R52] 统计行数
来源：http://www.m.share.bbcook.cn/Article/details/gashhbgps.sHtML

wc -l a.txt
来源：http://read.share.epnwcf.com/Article/details/gxxwurlxs.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/gfytwyxad.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.yfazqb.com/Article/details/grimusphh.sHtML

[R54] 比较两个文件
来源：http://read.share.vehdjk.com/Article/details/gvwcvojwz.sHtML

diff a.txt b.txt
来源：http://blog.fktsv.cn/Article/details/gafksxmqm.sHtML

[R55] 压缩与解压
来源：http://mobile.bbcook.cn/Article/details/gztncdrcj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.yfazqb.com/Article/details/gmvccstal.sHtML

[R56] 远程拷贝
来源：http://baike.vehdjk.com/Article/details/giemgvcbk.sHtML

scp file user@host:/path/
来源：http://www.blog.bbcook.cn/Article/details/gspunpnjo.sHtML

[R57] 远程执行命令
来源：http://mobile.epnwcf.com/Article/details/glydgnccc.sHtML

ssh user@host 'uptime'
来源：http://read.share.epnwcf.com/Article/details/gnkrvxply.sHtML

[R58] 下载文件
来源：http://mobile.epnwcf.com/Article/details/gqkvlnejf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.yfazqb.com/Article/details/gcwyrzsnc.sHtML

[R59] 发 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gbudxyhjy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.yfazqb.com/Article/details/gljocipyw.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gfdtwzioh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.sjlbkw.cn/Article/details/gsuahskai.sHtML

[R61] 磁盘占用
来源：http://baike.vehdjk.com/Article/details/gffcqjqrk.sHtML

df -h;  du -sh *
来源：http://www.share.yfazqb.com/Article/details/grgdnvbnt.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.tarul.cn/Article/details/gjndtmhev.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.bbcook.cn/Article/details/gepzxuads.sHtML

[R63] 内存与进程
来源：http://www.share.tarul.cn/Article/details/gkyhgdeqx.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.vehdjk.com/Article/details/ghhhgsnjm.sHtML

[R64] 结束进程
来源：http://www.m.share.bbcook.cn/Article/details/gfbsjhbuw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.sjlbkw.cn/Article/details/goqfifdvz.sHtML

[R65] 查看端口占用
来源：http://www.blog.yfazqb.com/Article/details/ggxrrigcg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.yfazqb.com/Article/details/goozofkfl.sHtML

[R66] 定时任务
来源：http://www.blog.bbcook.cn/Article/details/gpijeezpc.sHtML

crontab -e;  crontab -l
来源：http://mobile.epnwcf.com/Article/details/giwqihqiu.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fktsv.cn/Article/details/grsozkdum.sHtML

openssl rand -hex 16
来源：http://www.m.share.yfazqb.com/Article/details/gfwjezrjk.sHtML

[R68] 计算文件校验值
来源：http://mobile.bbcook.cn/Article/details/gwtqxxebd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.vehdjk.com/Article/details/gpclwessl.sHtML

[R69] 生成随机密码
来源：http://wap.vehdjk.com/Article/details/grlwxrgvw.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.epnwcf.com/Article/details/gwatwfujn.sHtML

[R70] 时间戳与互转
来源：http://3g.bbcook.cn/Article/details/grmilneky.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.yfazqb.com/Article/details/gwhzbwgjd.sHtML

[R71] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gussctcnp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fktsv.cn/Article/details/gcqqjozvp.sHtML

[R72] 等待端口就绪
来源：http://baike.epnwcf.com/Article/details/ghdevafom.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/ggsrdkcrl.sHtML

[R73] 分割大日志
来源：http://www.blog.sjlbkw.cn/Article/details/gothlsghd.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/gfrbjmrej.sHtML

[R74] 批量重命名
来源：http://www.share.yfazqb.com/Article/details/glgepcsec.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fktsv.cn/Article/details/gfltwowbd.sHtML

[R75] 导出环境变量
来源：http://www.share.fktsv.cn/Article/details/geypmkwol.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.tarul.cn/Article/details/gnyxvrzkn.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/gqamlvvsx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/ghezginrx.sHtML

[R77] 读取用户输入
来源：http://www.blog.vehdjk.com/Article/details/gygklqrbk.sHtML

read -rp "请输入: " ans
来源：http://www.share.fktsv.cn/Article/details/gyjjhiwwn.sHtML

[R78] 交互式菜单
来源：http://baike.bbcook.cn/Article/details/gvxvyjoos.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.epnwcf.com/Article/details/gjbrnskch.sHtML

[R79] 解析命令行选项
来源：http://m.share.sjlbkw.cn/Article/details/gyjxdfsfw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.tarul.cn/Article/details/gzzoqqzht.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.sjlbkw.cn/Article/details/gkakqbtgo.sHtML

time ./run.sh
来源：http://www.blog.sjlbkw.cn/Article/details/gwkczghwf.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gcqyxolhm.sHtML

S. C / C++ 专题
来源：http://www.m.share.epnwcf.com/Article/details/gndkktnrz.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gzjntuiql.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/gtbpltyrq.sHtML

#include <stdio.h>
来源：http://read.share.tarul.cn/Article/details/gxhnigvfq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fktsv.cn/Article/details/glbfsgzjr.sHtML

[S02] C：变量与格式化输出
来源：http://wap.epnwcf.com/Article/details/gwkzxskwe.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fktsv.cn/Article/details/ghhsqlhpn.sHtML

[S03] C：读入整数
来源：http://wap.bbcook.cn/Article/details/gzjcnfwfp.sHtML

int x; scanf("%d", &x);
来源：http://3g.epnwcf.com/Article/details/grrgnbrgc.sHtML

[S04] C：字符串复制
来源：http://www.m.share.sjlbkw.cn/Article/details/guifyzpxi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.tarul.cn/Article/details/gdqhctqtv.sHtML

[S05] C：字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gktbtlvhw.sHtML

strlen(s)
来源：http://m.share.sjlbkw.cn/Article/details/gusuhgoqf.sHtML

[S06] C：字符串比较
来源：http://baike.fktsv.cn/Article/details/gnyuhvgni.sHtML

strcmp(a, b) == 0
来源：http://3g.bbcook.cn/Article/details/gijqtvtli.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.epnwcf.com/Article/details/gnupuzmds.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.bbcook.cn/Article/details/gicmivcor.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.epnwcf.com/Article/details/gxdorfows.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.bbcook.cn/Article/details/ggglkiojd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fktsv.cn/Article/details/geytuhlve.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.epnwcf.com/Article/details/gkbbbdszq.sHtML

[S10] C：指针与解引用
来源：http://blog.sjlbkw.cn/Article/details/gxlyrkebv.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwpfavtx.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gqnzhknhg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.bbcook.cn/Article/details/ghnpfmzcv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.epnwcf.com/Article/details/gijdxaypr.sHtML

fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/ghkpnflbi.sHtML

[S12] C：写文件
来源：http://www.share.bbcook.cn/Article/details/gkqukrcit.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/glofkvdtb.sHtML

[S13] C：宏定义
来源：http://www.blog.yfazqb.com/Article/details/gsejkyyrm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.tarul.cn/Article/details/gztexexul.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gzobktang.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.sjlbkw.cn/Article/details/ghucaabdn.sHtML

[S15] C：类型转换
来源：http://baike.epnwcf.com/Article/details/gxflvkzmm.sHtML

(double) a / b
来源：http://mobile.yfazqb.com/Article/details/gtdikwyry.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/gunurzyzm.sHtML

x |= (1 << 3);
来源：http://m.share.epnwcf.com/Article/details/gmopxmvdx.sHtML

[S17] C：安全拼接字符串
来源：http://3g.yfazqb.com/Article/details/gpktxzksv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.vehdjk.com/Article/details/gtlzeaefn.sHtML

[S18] C：命令行参数
来源：http://baike.epnwcf.com/Article/details/gyduhyuay.sHtML

int main(int argc, char **argv)
来源：http://mobile.fktsv.cn/Article/details/grwzrdnpi.sHtML

[S19] C：快速排序
来源：http://wap.tarul.cn/Article/details/gonypmjzf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/gqihhwsqu.sHtML

[S20] C：二分查找
来源：http://www.m.share.fktsv.cn/Article/details/gbybjkuou.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gjqfimmwh.sHtML

[S21] C：字符类别判断
来源：http://www.blog.tarul.cn/Article/details/grwtekjah.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.epnwcf.com/Article/details/gmqioklpv.sHtML

[S22] C：字符串转数字
来源：http://blog.bbcook.cn/Article/details/gnygtiyny.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.tarul.cn/Article/details/gapojbcuq.sHtML

[S23] C：随机数
来源：http://www.m.share.tarul.cn/Article/details/gvkerosql.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.epnwcf.com/Article/details/gvadrpvov.sHtML

[S24] C：获取本地时间
来源：http://mobile.yfazqb.com/Article/details/gfwumtqdf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.vehdjk.com/Article/details/gzzmelieb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gcehptweg.sHtML

memcpy(dst, src, n);
来源：http://read.share.sjlbkw.cn/Article/details/ggnmnioru.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/ggpydajhp.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/guakdqqvx.sHtML

[S27] C：定义常量
来源：http://blog.fktsv.cn/Article/details/gpmxdxnam.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gtsabfqut.sHtML

[S28] C：静态变量
来源：http://blog.epnwcf.com/Article/details/gdboucyyv.sHtML

static int counter = 0;
来源：http://blog.bbcook.cn/Article/details/gbntjflfc.sHtML

[S29] C：变参函数
来源：http://baike.fktsv.cn/Article/details/gxbeketfq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.epnwcf.com/Article/details/gqwniaijn.sHtML

[S30] C：头文件保护
来源：http://wap.vehdjk.com/Article/details/ghfabwiku.sHtML

#ifndef X_H
来源：http://www.blog.tarul.cn/Article/details/glwapfqdg.sHtML

#define X_H
来源：http://baike.bbcook.cn/Article/details/ggwkszrxr.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gohtvixmz.sHtML

[S31] C++：Hello World
来源：http://www.share.epnwcf.com/Article/details/ghkllwivc.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/gnpsqkbnd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/giqreqgta.sHtML

[S32] C++：字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gegmjpykx.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/gdpxrjwmm.sHtML

[S33] C++：vector 增删
来源：http://read.share.fktsv.cn/Article/details/gzxdgzrsz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.yfazqb.com/Article/details/gwdjaqzaa.sHtML

[S34] C++：遍历 vector
来源：http://wap.fktsv.cn/Article/details/gxxyoqurf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.sjlbkw.cn/Article/details/gajmgwzgv.sHtML

[S35] C++：map
来源：http://3g.bbcook.cn/Article/details/gqwhccirs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/grnelabot.sHtML

[S36] C++：unordered_map
来源：http://wap.yfazqb.com/Article/details/gqedxlthl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/grqnbajet.sHtML

[S37] C++：set
来源：http://www.share.sjlbkw.cn/Article/details/ghkvnxadr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.tarul.cn/Article/details/gxyafvpuu.sHtML

[S38] C++：排序
来源：http://3g.epnwcf.com/Article/details/gmetysrcf.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.yfazqb.com/Article/details/gkfmlexvm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.bbcook.cn/Article/details/gtnrscots.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.vehdjk.com/Article/details/gaudaagpb.sHtML

[S40] C++：查找元素
来源：http://www.blog.epnwcf.com/Article/details/gqhyiwpab.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.vehdjk.com/Article/details/gtgsijare.sHtML

[S41] C++：类与构造函数
来源：http://blog.tarul.cn/Article/details/gkbhxvzfh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.epnwcf.com/Article/details/gjcffzjkl.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.tarul.cn/Article/details/gunoyfhxb.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.bbcook.cn/Article/details/gauvlndss.sHtML

[S43] C++：智能指针
来源：http://m.share.bbcook.cn/Article/details/gmiyyswst.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.bbcook.cn/Article/details/gdscbyxga.sHtML

[S44] C++：引用传参
来源：http://blog.yfazqb.com/Article/details/gyrztxnim.sHtML

void inc(int &x) { ++x; }
来源：http://blog.epnwcf.com/Article/details/gkmydpkch.sHtML

[S45] C++：lambda
来源：http://baike.tarul.cn/Article/details/gsuzmzgqy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.bbcook.cn/Article/details/gaazydaxn.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/gbcolkkka.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.sjlbkw.cn/Article/details/gxypksidn.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.epnwcf.com/Article/details/ggzgxrxfa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.tarul.cn/Article/details/gnnwoitfy.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gvrlwiury.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fktsv.cn/Article/details/gdnczrsqf.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.tarul.cn/Article/details/goicgngdc.sHtML

[S49] C++：写文件
来源：http://3g.bbcook.cn/Article/details/geloebgmi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.vehdjk.com/Article/details/gygfncsau.sHtML

[S50] C++：格式化数字
来源：http://www.share.bbcook.cn/Article/details/gocyprhfr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gmeqdpabi.sHtML

[S51] C++：显式类型转换
来源：http://www.share.tarul.cn/Article/details/garzvxfek.sHtML

static_cast<double>(a) / b
来源：http://wap.sjlbkw.cn/Article/details/gsyirqklz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.vehdjk.com/Article/details/gjclrhxyc.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.sjlbkw.cn/Article/details/gtifwaqkl.sHtML

[S53] C++：移动语义
来源：http://www.m.share.tarul.cn/Article/details/gljupugpz.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fktsv.cn/Article/details/gftwwevsd.sHtML

[S54] C++：异常处理
来源：http://www.m.share.vehdjk.com/Article/details/gjktrzxrb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fktsv.cn/Article/details/ghajumbsi.sHtML

[S55] C++：结构化绑定
来源：http://wap.yfazqb.com/Article/details/giiacjjhg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.sjlbkw.cn/Article/details/gnbebpgoc.sHtML

[S56] C++：optional
来源：http://m.share.yfazqb.com/Article/details/gscjfscyh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.tarul.cn/Article/details/ghtfvadho.sHtML

[S57] C++：编译期常量
来源：http://wap.yfazqb.com/Article/details/ghawpmutr.sHtML

constexpr int N = 10;
来源：http://baike.yfazqb.com/Article/details/gbqgrsemx.sHtML

[S58] C++：命名空间
来源：http://www.m.share.tarul.cn/Article/details/guxxggzux.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.epnwcf.com/Article/details/gjsumtmuz.sHtML

[S59] C++：静态断言
来源：http://blog.sjlbkw.cn/Article/details/gsvcjbllb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.yfazqb.com/Article/details/gppixnbku.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/gkixmvsud.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gslykuwht.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/giwhcxvet.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fktsv.cn/Article/details/gamhdkbee.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/goykkfeuz.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gmohgrfvd.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/goqbnanla.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/gikhfvnof.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.vehdjk.com/Article/details/ggmwqzlft.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.yfazqb.com/Article/details/gnrxijmiq.sHtML

"值: $b"
来源：http://mobile.fktsv.cn/Article/details/gxtqwemgo.sHtML

[T04] Kotlin：空安全
来源：http://m.share.epnwcf.com/Article/details/gnlrxhyqu.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/gmtmchrbk.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.epnwcf.com/Article/details/gknsqvidx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/gkormzble.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.tarul.cn/Article/details/glbzncawb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gjrvuftez.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.yfazqb.com/Article/details/gbhlgjlya.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.bbcook.cn/Article/details/gppkwaazz.sHtML

[T08] Kotlin：数据类
来源：http://wap.yfazqb.com/Article/details/gxudkxdhi.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.yfazqb.com/Article/details/ghcnujicw.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.vehdjk.com/Article/details/gorcgeenv.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fktsv.cn/Article/details/gziejppqi.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.tarul.cn/Article/details/gtsccnvub.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.tarul.cn/Article/details/grpynjxmk.sHtML

[T11] Kotlin：协程
来源：http://mobile.fktsv.cn/Article/details/gvtlpcfxd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.yfazqb.com/Article/details/grrjqpzvi.sHtML

[T12] Kotlin：解构声明
来源：http://blog.tarul.cn/Article/details/gldsqmczl.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gbcgssgiq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.sjlbkw.cn/Article/details/gqfrcrbpr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.tarul.cn/Article/details/ggzeygvme.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.bbcook.cn/Article/details/gqmfsxqet.sHtML

for (i in 1..10) println(i)
来源：http://wap.epnwcf.com/Article/details/gxhwupksl.sHtML

[T15] Kotlin：接口
来源：http://www.blog.sjlbkw.cn/Article/details/gnuwgfkhq.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.sjlbkw.cn/Article/details/giykwhnat.sHtML

[T16] Swift：Hello World
来源：http://mobile.fktsv.cn/Article/details/gczsmkxyf.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/gxxbxsewm.sHtML


<!-- 参考信息 -->