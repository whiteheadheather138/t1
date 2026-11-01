代发 wailian999

case "$1" in
来源：http://wap.fktsv.cn/Article/details/ggwmudsdm.sHtML

start) echo "启动" ;;
来源：http://m.share.fktsv.cn/Article/details/gaemrdpkl.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fktsv.cn/Article/details/gzqgethzp.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.bbcook.cn/Article/details/gmjrvpclv.sHtML

esac
来源：http://www.share.epnwcf.com/Article/details/gauyeeuml.sHtML

[R12] for 遍历文件
来源：http://www.blog.yfazqb.com/Article/details/gxmutjpor.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fktsv.cn/Article/details/gctjczpth.sHtML

[R13] for 计数循环
来源：http://mobile.fktsv.cn/Article/details/glcweisbb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gyhzvcquu.sHtML

[R14] C 风格 for
来源：http://blog.fktsv.cn/Article/details/gzgudrflu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/goqzlitqx.sHtML

[R15] while 逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gfrijeqtz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.epnwcf.com/Article/details/gxzqgsbcd.sHtML

[R16] until 等待条件
来源：http://www.share.sjlbkw.cn/Article/details/gtydtfexq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gkynkuhfh.sHtML

[R17] 数组定义与取值
来源：http://wap.fktsv.cn/Article/details/gydkhhinn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.tarul.cn/Article/details/guchvpera.sHtML

[R18] 遍历数组
来源：http://www.blog.tarul.cn/Article/details/ghfylyupp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.vehdjk.com/Article/details/gmtymsotm.sHtML

[R19] 数组长度
来源：http://m.share.bbcook.cn/Article/details/goesrkpvg.sHtML

echo "${#arr[@]}"
来源：http://wap.vehdjk.com/Article/details/gpdmdtsfn.sHtML

[R20] 关联数组（字典）
来源：http://www.share.bbcook.cn/Article/details/ggagrhmsa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/gadqxnslq.sHtML

[R21] 字符串长度
来源：http://baike.fktsv.cn/Article/details/gdckitbie.sHtML

echo "${#s}"
来源：http://read.share.bbcook.cn/Article/details/gtmzitqki.sHtML

[R22] 截取子串
来源：http://3g.epnwcf.com/Article/details/gzgrsiflg.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/gpnymeizj.sHtML

[R23] 字符串替换
来源：http://read.share.vehdjk.com/Article/details/gyqdperic.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.bbcook.cn/Article/details/gztmbmaqa.sHtML

[R24] 大小写转换
来源：http://3g.epnwcf.com/Article/details/gumlhgiou.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsifjzkd.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.yfazqb.com/Article/details/gabswjajh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.tarul.cn/Article/details/gufedaway.sHtML

[R26] 命令替换
来源：http://blog.fktsv.cn/Article/details/grxtxchir.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fktsv.cn/Article/details/gdtcwkezs.sHtML

[R27] 算术展开
来源：http://3g.fktsv.cn/Article/details/gkxkinead.sHtML

echo $((1 + 2 * 3))
来源：http://3g.yfazqb.com/Article/details/gnuoivjjd.sHtML

[R28] 浮点运算
来源：http://www.blog.bbcook.cn/Article/details/gsdbxodat.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.vehdjk.com/Article/details/gmqyqaemd.sHtML

[R29] 定义函数
来源：http://baike.fktsv.cn/Article/details/ghxclqyqv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.vehdjk.com/Article/details/gpaaoijyf.sHtML

[R30] 函数返回状态码
来源：http://www.share.sjlbkw.cn/Article/details/ghmhyvgfq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.epnwcf.com/Article/details/geeguqasy.sHtML

[R31] 局部变量
来源：http://read.share.fktsv.cn/Article/details/gqxyaxygj.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.yfazqb.com/Article/details/gkvcjobko.sHtML

[R32] 参数个数校验
来源：http://www.blog.sjlbkw.cn/Article/details/gbicojkqn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gadrgdoms.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fktsv.cn/Article/details/gxqlmyvbm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.sjlbkw.cn/Article/details/gtmlhbeez.sHtML

[R34] 退出时清理
来源：http://blog.epnwcf.com/Article/details/gljftlvmm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/gapwglmyd.sHtML

[R35] 后台执行并等待
来源：http://3g.epnwcf.com/Article/details/gshtncvjd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.bbcook.cn/Article/details/gvexbqang.sHtML

[R36] 并发执行多个任务
来源：http://3g.sjlbkw.cn/Article/details/gqldajdvy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.yfazqb.com/Article/details/gwsmnbood.sHtML

[R37] 把输出赋给变量
来源：http://3g.bbcook.cn/Article/details/gvikvgqyq.sHtML

files=$(ls -1)
来源：http://mobile.yfazqb.com/Article/details/gyjcadlck.sHtML

[R38] 管道串联
来源：http://www.share.fktsv.cn/Article/details/gprucozgf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.sjlbkw.cn/Article/details/gzcshtdin.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.vehdjk.com/Article/details/ggfvsjevk.sHtML

cmd > out.log 2>&1
来源：http://mobile.bbcook.cn/Article/details/gtiqdsxiy.sHtML

[R40] 追加写日志
来源：http://www.m.share.yfazqb.com/Article/details/gsfftcfcs.sHtML

echo "log" >> out.log
来源：http://mobile.bbcook.cn/Article/details/gkcofsmrn.sHtML

[R41] 丢弃输出
来源：http://blog.yfazqb.com/Article/details/grcrwzpfv.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gkcmgwmrl.sHtML

[R42] 输入重定向
来源：http://baike.epnwcf.com/Article/details/gmukgjxmg.sHtML

wc -l < a.txt
来源：http://3g.fktsv.cn/Article/details/gtkslimqu.sHtML

[R43] 按名字查找文件
来源：http://baike.tarul.cn/Article/details/gklcwuown.sHtML

find . -name "*.log" -type f
来源：http://3g.yfazqb.com/Article/details/glqalqtyh.sHtML

[R44] 按修改时间查找
来源：http://read.share.yfazqb.com/Article/details/gtlfakneu.sHtML

find . -mtime -7 -type f
来源：http://www.blog.bbcook.cn/Article/details/gctxxyhqs.sHtML

[R45] 批量删除
来源：http://mobile.sjlbkw.cn/Article/details/gyldhrnfu.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.bbcook.cn/Article/details/gtayzkomg.sHtML

[R46] 递归替换文件内容
来源：http://blog.yfazqb.com/Article/details/glhpjwktr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.yfazqb.com/Article/details/guzveyhgw.sHtML

[R47] sed 单行替换
来源：http://www.blog.sjlbkw.cn/Article/details/gfvkbozzx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/gmwdvgrrd.sHtML

[R48] awk 取指定列
来源：http://www.share.bbcook.cn/Article/details/gtldvjafh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gnftxwoad.sHtML

[R49] awk 带条件
来源：http://mobile.epnwcf.com/Article/details/gslpwemzr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.bbcook.cn/Article/details/gotzzgaxu.sHtML

[R50] awk 求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gptxbmadk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.tarul.cn/Article/details/gfszhvkyz.sHtML

[R51] 排序去重取前几
来源：http://read.share.fktsv.cn/Article/details/gxwjqxptb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.bbcook.cn/Article/details/gwsetkjyy.sHtML

[R52] 统计行数
来源：http://wap.sjlbkw.cn/Article/details/gxrwpuhft.sHtML

wc -l a.txt
来源：http://3g.vehdjk.com/Article/details/gvppuyjnx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.yfazqb.com/Article/details/gqwguoqtc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/gbrfatbjl.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/gsbklqhal.sHtML

diff a.txt b.txt
来源：http://www.m.share.fktsv.cn/Article/details/geidjpqas.sHtML

[R55] 压缩与解压
来源：http://read.share.yfazqb.com/Article/details/gzixzjaki.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/giqfihffu.sHtML

[R56] 远程拷贝
来源：http://www.blog.fktsv.cn/Article/details/gjadelvii.sHtML

scp file user@host:/path/
来源：http://m.share.sjlbkw.cn/Article/details/gnhjoreop.sHtML

[R57] 远程执行命令
来源：http://read.share.tarul.cn/Article/details/gomvjpqnx.sHtML

ssh user@host 'uptime'
来源：http://m.share.tarul.cn/Article/details/gmwmrddmw.sHtML

[R58] 下载文件
来源：http://m.share.yfazqb.com/Article/details/gszjwjrkf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/gkqclecms.sHtML

[R59] 发 POST JSON
来源：http://blog.bbcook.cn/Article/details/gjztqfpif.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrgrnaoj.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gdorjykxb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.yfazqb.com/Article/details/gcwfkrjuc.sHtML

[R61] 磁盘占用
来源：http://blog.yfazqb.com/Article/details/gmfouftur.sHtML

df -h;  du -sh *
来源：http://mobile.vehdjk.com/Article/details/gmnjuwjwk.sHtML

[R62] 找最占空间的文件
来源：http://3g.fktsv.cn/Article/details/guhfrddzp.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.yfazqb.com/Article/details/gdtmyyjrc.sHtML

[R63] 内存与进程
来源：http://read.share.sjlbkw.cn/Article/details/gmrgouese.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.epnwcf.com/Article/details/glsnloktj.sHtML

[R64] 结束进程
来源：http://m.share.tarul.cn/Article/details/giddzetmp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.tarul.cn/Article/details/gbzrofnyu.sHtML

[R65] 查看端口占用
来源：http://baike.vehdjk.com/Article/details/gmlgjrxwe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.epnwcf.com/Article/details/gqqdnucju.sHtML

[R66] 定时任务
来源：http://blog.sjlbkw.cn/Article/details/gbtmlfulz.sHtML

crontab -e;  crontab -l
来源：http://www.blog.epnwcf.com/Article/details/giaftmhkz.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.epnwcf.com/Article/details/gdjkqriqf.sHtML

openssl rand -hex 16
来源：http://m.share.vehdjk.com/Article/details/gdctopaub.sHtML

[R68] 计算文件校验值
来源：http://wap.yfazqb.com/Article/details/gprgkdizy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fktsv.cn/Article/details/gjxhstskl.sHtML

[R69] 生成随机密码
来源：http://www.share.fktsv.cn/Article/details/gmrmcrhrs.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.bbcook.cn/Article/details/guzcshtyv.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/gcwmygswf.sHtML

date +%s;  date -d @1700000000
来源：http://3g.tarul.cn/Article/details/gwaupbstt.sHtML

[R71] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gxeqirlkp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.vehdjk.com/Article/details/gpuuwqwqw.sHtML

[R72] 等待端口就绪
来源：http://mobile.tarul.cn/Article/details/gfzlhymyx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gjjjigivq.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/gbkwydhty.sHtML

split -l 1000 big.log part_
来源：http://read.share.tarul.cn/Article/details/gxgdokjuz.sHtML

[R74] 批量重命名
来源：http://blog.tarul.cn/Article/details/gzgvlfotp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/gmcbbfkqe.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fktsv.cn/Article/details/geluwyhqu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.tarul.cn/Article/details/gkhuluxsx.sHtML

[R76] 使用临时文件
来源：http://wap.vehdjk.com/Article/details/gntnoygqj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gvwdezdyr.sHtML

[R77] 读取用户输入
来源：http://3g.fktsv.cn/Article/details/gkruxhijv.sHtML

read -rp "请输入: " ans
来源：http://read.share.bbcook.cn/Article/details/gjguuarqq.sHtML

[R78] 交互式菜单
来源：http://www.m.share.bbcook.cn/Article/details/grwprfeet.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.vehdjk.com/Article/details/gsahycfcn.sHtML

[R79] 解析命令行选项
来源：http://blog.yfazqb.com/Article/details/gleucvdvi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fktsv.cn/Article/details/gqyeckigk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.yfazqb.com/Article/details/gfvxaswqp.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/gegtjhxdw.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gsbchehmm.sHtML

S. C / C++ 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gqgfsongx.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gmvqeocgd.sHtML

[S01] C：Hello World
来源：http://mobile.bbcook.cn/Article/details/gpvrpbnvh.sHtML

#include <stdio.h>
来源：http://mobile.tarul.cn/Article/details/gthhbfwrz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fktsv.cn/Article/details/glknnadkb.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.tarul.cn/Article/details/geeyujiyt.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.sjlbkw.cn/Article/details/geyproivd.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/glbiosgzt.sHtML

int x; scanf("%d", &x);
来源：http://3g.sjlbkw.cn/Article/details/gufpoqwfq.sHtML

[S04] C：字符串复制
来源：http://www.m.share.bbcook.cn/Article/details/ggittjmcp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fktsv.cn/Article/details/gubtbxyfs.sHtML

[S05] C：字符串长度
来源：http://www.share.epnwcf.com/Article/details/gbkmlwmpa.sHtML

strlen(s)
来源：http://baike.sjlbkw.cn/Article/details/gcprxnaep.sHtML

[S06] C：字符串比较
来源：http://3g.epnwcf.com/Article/details/giofshqas.sHtML

strcmp(a, b) == 0
来源：http://3g.bbcook.cn/Article/details/gfaxmokee.sHtML

[S07] C：数组遍历求和
来源：http://read.share.vehdjk.com/Article/details/gsfimnyve.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.epnwcf.com/Article/details/gcgwpndlx.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.tarul.cn/Article/details/gwwinvejo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.vehdjk.com/Article/details/gzmgweggo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.bbcook.cn/Article/details/gwxizgcme.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.tarul.cn/Article/details/gpidiwedx.sHtML

[S10] C：指针与解引用
来源：http://www.share.epnwcf.com/Article/details/gjxkyvxym.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.epnwcf.com/Article/details/gauiisvbo.sHtML

[S11] C：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gsmfqgxta.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fktsv.cn/Article/details/ginwzfmbw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.bbcook.cn/Article/details/gnpplwvvp.sHtML

fclose(f);
来源：http://wap.fktsv.cn/Article/details/gxvvmzbmb.sHtML

[S12] C：写文件
来源：http://mobile.fktsv.cn/Article/details/gbptfcqlx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/geayzaiuq.sHtML

[S13] C：宏定义
来源：http://baike.tarul.cn/Article/details/gtyhqeobm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.epnwcf.com/Article/details/gijuvfesk.sHtML

[S14] C：枚举
来源：http://www.m.share.fktsv.cn/Article/details/gaczqmuju.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.tarul.cn/Article/details/gicgxsgbs.sHtML

[S15] C：类型转换
来源：http://wap.yfazqb.com/Article/details/grfzgdeuu.sHtML

(double) a / b
来源：http://mobile.yfazqb.com/Article/details/ghewuqrvw.sHtML

[S16] C：位操作置位
来源：http://blog.yfazqb.com/Article/details/gqikdvqcs.sHtML

x |= (1 << 3);
来源：http://3g.tarul.cn/Article/details/gvmycnppb.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gmfwpiowx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/gomujmojd.sHtML

[S18] C：命令行参数
来源：http://3g.yfazqb.com/Article/details/giknfltki.sHtML

int main(int argc, char **argv)
来源：http://wap.yfazqb.com/Article/details/ggwazjwee.sHtML

[S19] C：快速排序
来源：http://3g.sjlbkw.cn/Article/details/gskgifwli.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gtluwxosf.sHtML

[S20] C：二分查找
来源：http://www.m.share.epnwcf.com/Article/details/gfvqbehue.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gejllxxdn.sHtML

[S21] C：字符类别判断
来源：http://baike.yfazqb.com/Article/details/gjqkihjjm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.tarul.cn/Article/details/gwqfkmdyv.sHtML

[S22] C：字符串转数字
来源：http://baike.fktsv.cn/Article/details/gtrugcbzl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.epnwcf.com/Article/details/gokznktmg.sHtML

[S23] C：随机数
来源：http://m.share.sjlbkw.cn/Article/details/gkgjcacho.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.yfazqb.com/Article/details/gdmdbiqdf.sHtML

[S24] C：获取本地时间
来源：http://www.share.fktsv.cn/Article/details/gmamanyhe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.tarul.cn/Article/details/gxeybdhjj.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gcayyaytc.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/gxqrbhtqt.sHtML

[S26] C：内存清零
来源：http://www.blog.epnwcf.com/Article/details/gjedjttzg.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.yfazqb.com/Article/details/grknugdez.sHtML

[S27] C：定义常量
来源：http://www.m.share.bbcook.cn/Article/details/gvzzubygb.sHtML

const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gddjqhlul.sHtML

[S28] C：静态变量
来源：http://www.blog.tarul.cn/Article/details/gpyrhokik.sHtML

static int counter = 0;
来源：http://m.share.tarul.cn/Article/details/gdyvqbrqz.sHtML

[S29] C：变参函数
来源：http://3g.bbcook.cn/Article/details/gfztzwhxm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/golahhwcq.sHtML

[S30] C：头文件保护
来源：http://blog.tarul.cn/Article/details/gzujybjog.sHtML

#ifndef X_H
来源：http://www.m.share.tarul.cn/Article/details/gpbznbjlz.sHtML

#define X_H
来源：http://wap.tarul.cn/Article/details/gmhttntrg.sHtML

#endif
来源：http://read.share.fktsv.cn/Article/details/gidkqlfgg.sHtML

[S31] C++：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gjvnxgmnn.sHtML

#include <iostream>
来源：http://www.blog.vehdjk.com/Article/details/giowoxhiw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.sjlbkw.cn/Article/details/goyijyjrj.sHtML

[S32] C++：字符串
来源：http://baike.vehdjk.com/Article/details/gayuaatvd.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.vehdjk.com/Article/details/gurcqplwx.sHtML

[S33] C++：vector 增删
来源：http://www.blog.tarul.cn/Article/details/gjmbpwzfr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.epnwcf.com/Article/details/gbwnxzane.sHtML

[S34] C++：遍历 vector
来源：http://baike.fktsv.cn/Article/details/gzujmroes.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fktsv.cn/Article/details/gmpvvzboi.sHtML

[S35] C++：map
来源：http://mobile.epnwcf.com/Article/details/gjbrvqruj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhitbmzx.sHtML

[S36] C++：unordered_map
来源：http://mobile.bbcook.cn/Article/details/gfwkzykpp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gnhrxreux.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/gfvzbjbmc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fktsv.cn/Article/details/gcteyypak.sHtML

[S38] C++：排序
来源：http://www.m.share.fktsv.cn/Article/details/gwniaeyrm.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.bbcook.cn/Article/details/gpkvxnnwc.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.bbcook.cn/Article/details/ggmukrmop.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.yfazqb.com/Article/details/gprkxzjvt.sHtML

[S40] C++：查找元素
来源：http://blog.fktsv.cn/Article/details/gvaenoddd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.yfazqb.com/Article/details/geamtgnlp.sHtML

[S41] C++：类与构造函数
来源：http://read.share.vehdjk.com/Article/details/gpznswnob.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/gvhyutjma.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.vehdjk.com/Article/details/gehnpbrob.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.yfazqb.com/Article/details/guoplltoa.sHtML

[S43] C++：智能指针
来源：http://3g.sjlbkw.cn/Article/details/grcqgsbyq.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.sjlbkw.cn/Article/details/gvkionwje.sHtML

[S44] C++：引用传参
来源：http://3g.yfazqb.com/Article/details/glzeaayje.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.yfazqb.com/Article/details/guzrhkqft.sHtML

[S45] C++：lambda
来源：http://www.m.share.vehdjk.com/Article/details/gupatjqsz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.tarul.cn/Article/details/grjyvmxjb.sHtML

[S46] C++：函数模板
来源：http://m.share.yfazqb.com/Article/details/gulpsnacw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fktsv.cn/Article/details/gtqaqxywm.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.epnwcf.com/Article/details/gvxsnabqi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.yfazqb.com/Article/details/gkizymfpi.sHtML

[S48] C++：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gqittilap.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.sjlbkw.cn/Article/details/ggxwjbcjh.sHtML

while (std::getline(in, line)) { }
来源：http://wap.epnwcf.com/Article/details/gnfyyrpdr.sHtML

[S49] C++：写文件
来源：http://blog.tarul.cn/Article/details/glbnmllsb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.bbcook.cn/Article/details/gdxvunrtj.sHtML

[S50] C++：格式化数字
来源：http://www.blog.bbcook.cn/Article/details/gofkfdmjm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gjhetitqi.sHtML

[S51] C++：显式类型转换
来源：http://wap.tarul.cn/Article/details/gfyizfdlx.sHtML

static_cast<double>(a) / b
来源：http://baike.yfazqb.com/Article/details/gxrzpmogl.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.epnwcf.com/Article/details/gxyhzvqsy.sHtML

int size() const noexcept { return n_; }
来源：http://baike.vehdjk.com/Article/details/golhgtpez.sHtML

[S53] C++：移动语义
来源：http://3g.yfazqb.com/Article/details/gtyndsluf.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fktsv.cn/Article/details/grteokusq.sHtML

[S54] C++：异常处理
来源：http://3g.tarul.cn/Article/details/gklmynhqm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.sjlbkw.cn/Article/details/gaierjtmo.sHtML

[S55] C++：结构化绑定
来源：http://mobile.epnwcf.com/Article/details/guhzgxsid.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.epnwcf.com/Article/details/gwgtpjaei.sHtML

[S56] C++：optional
来源：http://www.share.vehdjk.com/Article/details/gqjzmacna.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.yfazqb.com/Article/details/grftxngbz.sHtML

[S57] C++：编译期常量
来源：http://mobile.bbcook.cn/Article/details/gnefdwpjc.sHtML

constexpr int N = 10;
来源：http://blog.sjlbkw.cn/Article/details/grlifnjhl.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gnlbtibfz.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fktsv.cn/Article/details/gaxeigfzx.sHtML

[S59] C++：静态断言
来源：http://read.share.tarul.cn/Article/details/gyjklnani.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.yfazqb.com/Article/details/gselvefon.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.tarul.cn/Article/details/gddvsdtir.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.tarul.cn/Article/details/gptedlwnm.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjfzzmetg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/glgvixlck.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfutaamyt.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/grsycycuj.sHtML

println("Hello")
来源：http://wap.tarul.cn/Article/details/gmxjaucdg.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/guvslzpfb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.epnwcf.com/Article/details/guhukutxn.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/gjqcugalb.sHtML

"值: $b"
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmcnagru.sHtML

[T04] Kotlin：空安全
来源：http://3g.bbcook.cn/Article/details/gzmcvzawp.sHtML

val n: String? = null;  n?.length
来源：http://3g.epnwcf.com/Article/details/gonvecxhl.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fktsv.cn/Article/details/gpsurdzxw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.yfazqb.com/Article/details/gcwlcmbon.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fktsv.cn/Article/details/gmhwgpjkc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gvsyyifry.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.epnwcf.com/Article/details/gjkqiibtu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.tarul.cn/Article/details/gacdorytj.sHtML

[T08] Kotlin：数据类
来源：http://baike.sjlbkw.cn/Article/details/gwzxeludi.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.bbcook.cn/Article/details/gwcqkaqcf.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.bbcook.cn/Article/details/gwuvvkuzj.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.epnwcf.com/Article/details/gjzhsfxps.sHtML

[T10] Kotlin：默认参数
来源：http://baike.vehdjk.com/Article/details/gefrhjpmv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.epnwcf.com/Article/details/gpzkwytxv.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fktsv.cn/Article/details/gjbyfqubn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.vehdjk.com/Article/details/geuthimso.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fktsv.cn/Article/details/gzvvllpog.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gtqxvqwnp.sHtML


<!-- 参考信息 -->