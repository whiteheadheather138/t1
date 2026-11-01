代发 wailian999

case "$1" in
来源：http://wap.yfazqb.com/Article/details/gjgxoilzi.sHtML

start) echo "启动" ;;
来源：http://mobile.epnwcf.com/Article/details/glhsindyt.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gnzhsasyr.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.epnwcf.com/Article/details/gvmmiljss.sHtML

esac
来源：http://blog.yfazqb.com/Article/details/govzuemrp.sHtML

[R12] for 遍历文件
来源：http://www.blog.yfazqb.com/Article/details/gnnkyykhk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.yfazqb.com/Article/details/gjeowlbhn.sHtML

[R13] for 计数循环
来源：http://wap.epnwcf.com/Article/details/gsjxpznfu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/gsywxlfba.sHtML

[R14] C 风格 for
来源：http://3g.sjlbkw.cn/Article/details/gmjwnjvab.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/gylzymabr.sHtML

[R15] while 逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gtbclmosl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.yfazqb.com/Article/details/ghrcjpxek.sHtML

[R16] until 等待条件
来源：http://mobile.sjlbkw.cn/Article/details/gbvprfxok.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gxcgsfgmt.sHtML

[R17] 数组定义与取值
来源：http://mobile.epnwcf.com/Article/details/guugwvsqx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.bbcook.cn/Article/details/gtotjlshg.sHtML

[R18] 遍历数组
来源：http://mobile.fktsv.cn/Article/details/gyxwzymlr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.vehdjk.com/Article/details/gmxijhnbm.sHtML

[R19] 数组长度
来源：http://www.m.share.fktsv.cn/Article/details/gbkgbsdff.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/glvhxedal.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.vehdjk.com/Article/details/gtajsupts.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.vehdjk.com/Article/details/gebbtzrgn.sHtML

[R21] 字符串长度
来源：http://baike.bbcook.cn/Article/details/glyzxsnsk.sHtML

echo "${#s}"
来源：http://wap.sjlbkw.cn/Article/details/gktrlnrut.sHtML

[R22] 截取子串
来源：http://blog.fktsv.cn/Article/details/gftyykpso.sHtML

echo "${s:0:5}"
来源：http://www.blog.sjlbkw.cn/Article/details/gzwrfiaif.sHtML

[R23] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/gjkfzdhuu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.sjlbkw.cn/Article/details/gcxlfvcrd.sHtML

[R24] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gpxzterwa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.yfazqb.com/Article/details/glkenuukt.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.epnwcf.com/Article/details/gimikbjav.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.vehdjk.com/Article/details/gqztckgin.sHtML

[R26] 命令替换
来源：http://wap.sjlbkw.cn/Article/details/ghivutzyq.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.vehdjk.com/Article/details/gtywtjkpz.sHtML

[R27] 算术展开
来源：http://blog.fktsv.cn/Article/details/gkpskrrpa.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgmqcjyn.sHtML

[R28] 浮点运算
来源：http://baike.fktsv.cn/Article/details/giwfegsni.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/glinxnbcl.sHtML

[R29] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/gxltmwvau.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.tarul.cn/Article/details/gcpvobecj.sHtML

[R30] 函数返回状态码
来源：http://www.share.yfazqb.com/Article/details/gbspiryfh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fktsv.cn/Article/details/gdoiadvcf.sHtML

[R31] 局部变量
来源：http://www.share.bbcook.cn/Article/details/gdgpostaa.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.vehdjk.com/Article/details/gmcysyudg.sHtML

[R32] 参数个数校验
来源：http://m.share.vehdjk.com/Article/details/gdmrrydxh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gdbfefnox.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.tarul.cn/Article/details/ghiedcuja.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.yfazqb.com/Article/details/gcqrfulsx.sHtML

[R34] 退出时清理
来源：http://www.m.share.fktsv.cn/Article/details/grdvgokhd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/gdhthwihc.sHtML

[R35] 后台执行并等待
来源：http://www.share.fktsv.cn/Article/details/gjzwqahmn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.bbcook.cn/Article/details/gyhpimcha.sHtML

[R36] 并发执行多个任务
来源：http://3g.yfazqb.com/Article/details/gpnsqsrkw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fktsv.cn/Article/details/gakvpxrgf.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.sjlbkw.cn/Article/details/grgjeiqcy.sHtML

files=$(ls -1)
来源：http://mobile.sjlbkw.cn/Article/details/gyklufijc.sHtML

[R38] 管道串联
来源：http://www.share.tarul.cn/Article/details/gttqscbjn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.vehdjk.com/Article/details/gtueqbqij.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.yfazqb.com/Article/details/gxvltsamz.sHtML

cmd > out.log 2>&1
来源：http://blog.vehdjk.com/Article/details/gmtcwwqzn.sHtML

[R40] 追加写日志
来源：http://www.m.share.yfazqb.com/Article/details/gxnrpgdnl.sHtML

echo "log" >> out.log
来源：http://read.share.sjlbkw.cn/Article/details/gvnjrwonz.sHtML

[R41] 丢弃输出
来源：http://www.m.share.epnwcf.com/Article/details/gnxqzppyh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.bbcook.cn/Article/details/gctsjbsqc.sHtML

[R42] 输入重定向
来源：http://mobile.epnwcf.com/Article/details/gcnqwliqm.sHtML

wc -l < a.txt
来源：http://3g.tarul.cn/Article/details/gmwhugdqe.sHtML

[R43] 按名字查找文件
来源：http://www.share.bbcook.cn/Article/details/gxxlxwajm.sHtML

find . -name "*.log" -type f
来源：http://m.share.bbcook.cn/Article/details/gabzrpcdi.sHtML

[R44] 按修改时间查找
来源：http://mobile.sjlbkw.cn/Article/details/gcxrhaizv.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fktsv.cn/Article/details/ggcoceoxo.sHtML

[R45] 批量删除
来源：http://read.share.epnwcf.com/Article/details/gssvsfxbg.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.bbcook.cn/Article/details/gmirjnhrq.sHtML

[R46] 递归替换文件内容
来源：http://blog.bbcook.cn/Article/details/gcxyxvach.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.sjlbkw.cn/Article/details/gfqicllin.sHtML

[R47] sed 单行替换
来源：http://3g.yfazqb.com/Article/details/ghrckbytm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/glspywspm.sHtML

[R48] awk 取指定列
来源：http://read.share.epnwcf.com/Article/details/givqpomcm.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gsilqvcyd.sHtML

[R49] awk 带条件
来源：http://www.m.share.fktsv.cn/Article/details/gplgdijew.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.sjlbkw.cn/Article/details/gykyjuoyb.sHtML

[R50] awk 求和
来源：http://mobile.yfazqb.com/Article/details/ggytfkiry.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.bbcook.cn/Article/details/glbrpcsuk.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.bbcook.cn/Article/details/gagmcdwhn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.tarul.cn/Article/details/gtapptocg.sHtML

[R52] 统计行数
来源：http://3g.bbcook.cn/Article/details/goxdvksfi.sHtML

wc -l a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gqqbrwhts.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.tarul.cn/Article/details/ggshmkjvh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.sjlbkw.cn/Article/details/gehpuxtlc.sHtML

[R54] 比较两个文件
来源：http://baike.fktsv.cn/Article/details/gnmtcbtqu.sHtML

diff a.txt b.txt
来源：http://baike.epnwcf.com/Article/details/gnntycjax.sHtML

[R55] 压缩与解压
来源：http://m.share.epnwcf.com/Article/details/gygjkunuc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.vehdjk.com/Article/details/guwwjhjhi.sHtML

[R56] 远程拷贝
来源：http://www.share.vehdjk.com/Article/details/gzfcksnbh.sHtML

scp file user@host:/path/
来源：http://m.share.sjlbkw.cn/Article/details/gbxwsetqg.sHtML

[R57] 远程执行命令
来源：http://www.share.sjlbkw.cn/Article/details/gojroxmqc.sHtML

ssh user@host 'uptime'
来源：http://read.share.tarul.cn/Article/details/gojmbbxap.sHtML

[R58] 下载文件
来源：http://baike.fktsv.cn/Article/details/gspndsdxi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fktsv.cn/Article/details/gdctryavy.sHtML

[R59] 发 POST JSON
来源：http://3g.bbcook.cn/Article/details/gckbufwja.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.tarul.cn/Article/details/gxbeahphg.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/gekbsrtdu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.bbcook.cn/Article/details/giewvwvip.sHtML

[R61] 磁盘占用
来源：http://blog.tarul.cn/Article/details/glbpimicf.sHtML

df -h;  du -sh *
来源：http://3g.fktsv.cn/Article/details/gfxlvlazg.sHtML

[R62] 找最占空间的文件
来源：http://3g.fktsv.cn/Article/details/gpvzyvtko.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.bbcook.cn/Article/details/gkudcbekt.sHtML

[R63] 内存与进程
来源：http://blog.bbcook.cn/Article/details/glcegwkmc.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.sjlbkw.cn/Article/details/gvjutyeir.sHtML

[R64] 结束进程
来源：http://m.share.fktsv.cn/Article/details/gpmzgandq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fktsv.cn/Article/details/gtkujmhrw.sHtML

[R65] 查看端口占用
来源：http://baike.fktsv.cn/Article/details/gntofbdfh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.epnwcf.com/Article/details/gksjaqvml.sHtML

[R66] 定时任务
来源：http://mobile.vehdjk.com/Article/details/glhtgyxxx.sHtML

crontab -e;  crontab -l
来源：http://3g.tarul.cn/Article/details/gouzbhkvf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.epnwcf.com/Article/details/gzwafrzhh.sHtML

openssl rand -hex 16
来源：http://baike.tarul.cn/Article/details/grinczvvg.sHtML

[R68] 计算文件校验值
来源：http://www.share.fktsv.cn/Article/details/gbasysrbo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.vehdjk.com/Article/details/gtchmilzm.sHtML

[R69] 生成随机密码
来源：http://www.share.yfazqb.com/Article/details/gopgzkwlw.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.tarul.cn/Article/details/gpdocukaw.sHtML

[R70] 时间戳与互转
来源：http://read.share.fktsv.cn/Article/details/gvnvnbngj.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.bbcook.cn/Article/details/gdzslqhhv.sHtML

[R71] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gxjnxpiub.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fktsv.cn/Article/details/gfwvtlfsj.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fktsv.cn/Article/details/gdwjkajnd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.vehdjk.com/Article/details/gkchdblpo.sHtML

[R73] 分割大日志
来源：http://mobile.sjlbkw.cn/Article/details/gwlyfagan.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/goeoatkwb.sHtML

[R74] 批量重命名
来源：http://www.blog.yfazqb.com/Article/details/gdcurusdl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fktsv.cn/Article/details/gsrfyoqvj.sHtML

[R75] 导出环境变量
来源：http://m.share.epnwcf.com/Article/details/gnlqergbo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.sjlbkw.cn/Article/details/ghglplaps.sHtML

[R76] 使用临时文件
来源：http://m.share.tarul.cn/Article/details/gvutkxxkb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/gbtvwwgug.sHtML

[R77] 读取用户输入
来源：http://blog.sjlbkw.cn/Article/details/gqtxuepzu.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.tarul.cn/Article/details/gmvjqryfs.sHtML

[R78] 交互式菜单
来源：http://3g.vehdjk.com/Article/details/gcxsjozyl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.epnwcf.com/Article/details/gseytxfzj.sHtML

[R79] 解析命令行选项
来源：http://blog.sjlbkw.cn/Article/details/gqtmezrcf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.vehdjk.com/Article/details/gfjlxtewb.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.sjlbkw.cn/Article/details/gpgknzbwf.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/gteqiyfxy.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvxesqexw.sHtML

S. C / C++ 专题
来源：http://blog.epnwcf.com/Article/details/gvyjifkch.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gaxfvozbc.sHtML

[S01] C：Hello World
来源：http://read.share.bbcook.cn/Article/details/gbgapcpjl.sHtML

#include <stdio.h>
来源：http://blog.yfazqb.com/Article/details/glenskwfg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.bbcook.cn/Article/details/gdhehexue.sHtML

[S02] C：变量与格式化输出
来源：http://wap.yfazqb.com/Article/details/gszyhxrbc.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.tarul.cn/Article/details/gbfuipkpj.sHtML

[S03] C：读入整数
来源：http://m.share.bbcook.cn/Article/details/germmbwjb.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gqvjkincn.sHtML

[S04] C：字符串复制
来源：http://baike.sjlbkw.cn/Article/details/gumdliwgq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gibbmmjee.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/gglozvcsv.sHtML

strlen(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gvxcszbnu.sHtML

[S06] C：字符串比较
来源：http://www.share.yfazqb.com/Article/details/gkpjquczi.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.vehdjk.com/Article/details/gouevrefk.sHtML

[S07] C：数组遍历求和
来源：http://blog.tarul.cn/Article/details/geqimekco.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.sjlbkw.cn/Article/details/gwwwyssnh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.yfazqb.com/Article/details/gwgjxpaix.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.yfazqb.com/Article/details/grffyhugl.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.yfazqb.com/Article/details/gcfpltdtt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.yfazqb.com/Article/details/grnukrmqi.sHtML

[S10] C：指针与解引用
来源：http://mobile.bbcook.cn/Article/details/gswrbbjoe.sHtML

int *p = &a;  *p = 5;
来源：http://3g.yfazqb.com/Article/details/gsmobvpok.sHtML

[S11] C：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gllpaghzc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/gabmqmcds.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.epnwcf.com/Article/details/gqbaflkvq.sHtML

fclose(f);
来源：http://www.share.tarul.cn/Article/details/ggotycwxb.sHtML

[S12] C：写文件
来源：http://www.blog.epnwcf.com/Article/details/gmooqcqcr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gtxdtfcvt.sHtML

[S13] C：宏定义
来源：http://www.share.epnwcf.com/Article/details/gdrxchwlf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.tarul.cn/Article/details/gtzyyygdp.sHtML

[S14] C：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gbvuikutl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.vehdjk.com/Article/details/gmcqteovi.sHtML

[S15] C：类型转换
来源：http://mobile.epnwcf.com/Article/details/gepglesma.sHtML

(double) a / b
来源：http://www.blog.fktsv.cn/Article/details/gqdjkwewa.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/gvrpflssl.sHtML

x |= (1 << 3);
来源：http://www.m.share.tarul.cn/Article/details/glruyvgqj.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gnbomgxfb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.yfazqb.com/Article/details/gbrvndaun.sHtML

[S18] C：命令行参数
来源：http://www.share.yfazqb.com/Article/details/gzsihaeir.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gjgdtsaxy.sHtML

[S19] C：快速排序
来源：http://www.share.sjlbkw.cn/Article/details/gbxcwiami.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gzwqqetuj.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gaoqmbqfq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/glpibfqnf.sHtML

[S21] C：字符类别判断
来源：http://read.share.bbcook.cn/Article/details/ggdcouhxl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.epnwcf.com/Article/details/gqpvqehrf.sHtML

[S22] C：字符串转数字
来源：http://www.blog.sjlbkw.cn/Article/details/gicnwkeed.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.bbcook.cn/Article/details/gbvsukatl.sHtML

[S23] C：随机数
来源：http://blog.vehdjk.com/Article/details/ggammlxbe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.epnwcf.com/Article/details/gzhzklnvr.sHtML

[S24] C：获取本地时间
来源：http://blog.yfazqb.com/Article/details/glyfgsfgl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.tarul.cn/Article/details/gwrkggqbe.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gqdfrowko.sHtML

memcpy(dst, src, n);
来源：http://read.share.yfazqb.com/Article/details/gdnzugwmt.sHtML

[S26] C：内存清零
来源：http://3g.tarul.cn/Article/details/gczjsvkae.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.tarul.cn/Article/details/gayjlhwia.sHtML

[S27] C：定义常量
来源：http://mobile.bbcook.cn/Article/details/gewidkunw.sHtML

const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/glpvqlvkm.sHtML

[S28] C：静态变量
来源：http://www.blog.sjlbkw.cn/Article/details/guaovlylt.sHtML

static int counter = 0;
来源：http://www.share.fktsv.cn/Article/details/ghilvmjsq.sHtML

[S29] C：变参函数
来源：http://blog.vehdjk.com/Article/details/gyoilwghu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.sjlbkw.cn/Article/details/gcxbvliqt.sHtML

[S30] C：头文件保护
来源：http://blog.bbcook.cn/Article/details/gbbxaevwo.sHtML

#ifndef X_H
来源：http://baike.tarul.cn/Article/details/gnbfxjzce.sHtML

#define X_H
来源：http://wap.fktsv.cn/Article/details/ghipfzabb.sHtML

#endif
来源：http://wap.yfazqb.com/Article/details/gxhxodqih.sHtML

[S31] C++：Hello World
来源：http://3g.yfazqb.com/Article/details/gajrgjlxk.sHtML

#include <iostream>
来源：http://3g.yfazqb.com/Article/details/geinyoxlo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.vehdjk.com/Article/details/ggmahryuw.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gntvscbre.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.tarul.cn/Article/details/geborryuz.sHtML

[S33] C++：vector 增删
来源：http://m.share.sjlbkw.cn/Article/details/gaflwpejl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.yfazqb.com/Article/details/gejvafaqy.sHtML

[S34] C++：遍历 vector
来源：http://read.share.epnwcf.com/Article/details/gsdssmwxn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.tarul.cn/Article/details/ghsjloxfo.sHtML

[S35] C++：map
来源：http://www.share.vehdjk.com/Article/details/ghhasehns.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/guhgzogtl.sHtML

[S36] C++：unordered_map
来源：http://blog.tarul.cn/Article/details/gktookzrc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gdzvscafh.sHtML

[S37] C++：set
来源：http://3g.vehdjk.com/Article/details/gsbgacsfx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.epnwcf.com/Article/details/geclrpyzo.sHtML

[S38] C++：排序
来源：http://www.share.vehdjk.com/Article/details/gahwbdglp.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.bbcook.cn/Article/details/gqxwezgni.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.bbcook.cn/Article/details/gfxggsbuc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.epnwcf.com/Article/details/ghqowcjku.sHtML

[S40] C++：查找元素
来源：http://m.share.fktsv.cn/Article/details/gkobmddtc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.yfazqb.com/Article/details/gvmtgaqbc.sHtML

[S41] C++：类与构造函数
来源：http://m.share.vehdjk.com/Article/details/ghytomopq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.epnwcf.com/Article/details/gccgcipav.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.epnwcf.com/Article/details/gigvznnkl.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.yfazqb.com/Article/details/gdahsqoqd.sHtML

[S43] C++：智能指针
来源：http://blog.fktsv.cn/Article/details/glpoqhlzo.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.yfazqb.com/Article/details/gbulstcno.sHtML

[S44] C++：引用传参
来源：http://read.share.tarul.cn/Article/details/ggamwdmck.sHtML

void inc(int &x) { ++x; }
来源：http://wap.epnwcf.com/Article/details/gtbbigage.sHtML

[S45] C++：lambda
来源：http://m.share.sjlbkw.cn/Article/details/gvadkflee.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fktsv.cn/Article/details/gokizhfym.sHtML

[S46] C++：函数模板
来源：http://blog.vehdjk.com/Article/details/gzeinohob.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.sjlbkw.cn/Article/details/gtpespoaj.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.vehdjk.com/Article/details/gdkmfvjyt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.yfazqb.com/Article/details/gxlzdfvpj.sHtML

[S48] C++：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gepsuhesa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.vehdjk.com/Article/details/grdzvhanp.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.epnwcf.com/Article/details/gevehiyrh.sHtML

[S49] C++：写文件
来源：http://mobile.epnwcf.com/Article/details/gumyckkht.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.sjlbkw.cn/Article/details/gdknpmwtu.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.vehdjk.com/Article/details/gfmkwhigz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.bbcook.cn/Article/details/gvegosvtz.sHtML

[S51] C++：显式类型转换
来源：http://www.share.vehdjk.com/Article/details/gfnrwijrb.sHtML

static_cast<double>(a) / b
来源：http://read.share.yfazqb.com/Article/details/gwlhgjbcp.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.sjlbkw.cn/Article/details/gyqjrtbkd.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.vehdjk.com/Article/details/gzedrxxxo.sHtML

[S53] C++：移动语义
来源：http://www.share.fktsv.cn/Article/details/glghfdlss.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/gqpphlhdg.sHtML

[S54] C++：异常处理
来源：http://mobile.bbcook.cn/Article/details/gsywyswhl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.vehdjk.com/Article/details/geggwdmvq.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.vehdjk.com/Article/details/gnnfornfu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.vehdjk.com/Article/details/gmqrsiimo.sHtML

[S56] C++：optional
来源：http://www.m.share.vehdjk.com/Article/details/geyfbfupb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.bbcook.cn/Article/details/gdvqpjeqp.sHtML

[S57] C++：编译期常量
来源：http://wap.vehdjk.com/Article/details/gigvuawzq.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/gppjxtkvt.sHtML

[S58] C++：命名空间
来源：http://baike.tarul.cn/Article/details/gdmkvtnkp.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.epnwcf.com/Article/details/ggttgxqfa.sHtML

[S59] C++：静态断言
来源：http://www.share.epnwcf.com/Article/details/gkeimaqrx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.yfazqb.com/Article/details/gytvqozjx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.bbcook.cn/Article/details/gsyudtekv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gcvgffzau.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gliciyawv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.vehdjk.com/Article/details/gvjqsshvo.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gotstokvy.sHtML

[T01] Kotlin：Hello World
来源：http://baike.bbcook.cn/Article/details/gtemgjzbq.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/gfzxawvof.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.bbcook.cn/Article/details/grvdjmjrl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.yfazqb.com/Article/details/gfhsttsbk.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.epnwcf.com/Article/details/gbzkpdfnd.sHtML

"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gcdjrduhg.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.bbcook.cn/Article/details/gbpusawwn.sHtML

val n: String? = null;  n?.length
来源：http://read.share.yfazqb.com/Article/details/ggivqcakg.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.bbcook.cn/Article/details/gfonolbyl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fktsv.cn/Article/details/gafjobtgj.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.yfazqb.com/Article/details/gcihnxnqh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.yfazqb.com/Article/details/gljzuwghe.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.yfazqb.com/Article/details/gwbegpsta.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.tarul.cn/Article/details/gkuvhbiby.sHtML

[T08] Kotlin：数据类
来源：http://wap.fktsv.cn/Article/details/gwtcotvkp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvawzxml.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.sjlbkw.cn/Article/details/ggbatxnfc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.bbcook.cn/Article/details/gnhjhnqaz.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.tarul.cn/Article/details/gfmudxjqi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.tarul.cn/Article/details/gzywvidlp.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fktsv.cn/Article/details/gyhbgixfz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.yfazqb.com/Article/details/gjoqwemvn.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.bbcook.cn/Article/details/gzmfnfbmt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.epnwcf.com/Article/details/globoqhll.sHtML


<!-- 参考信息 -->