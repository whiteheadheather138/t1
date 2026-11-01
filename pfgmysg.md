代发 wailian999

name="${1:-default}"
来源：http://3g.yfazqb.com/Article/details/gygrihobq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.bbcook.cn/Article/details/gsgvlsmwy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/ggwiftphy.sHtML

[R07] if 判断文件
来源：http://read.share.tarul.cn/Article/details/gcrrmuzrl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gbkvpfvqk.sHtML

[R08] 数值比较
来源：http://www.blog.vehdjk.com/Article/details/gibhvhdqj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhlisarp.sHtML

[R09] 字符串比较
来源：http://mobile.yfazqb.com/Article/details/ggixndewy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.tarul.cn/Article/details/gouuzesfl.sHtML

[R10] 正则匹配
来源：http://baike.vehdjk.com/Article/details/gyeqxojyv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.vehdjk.com/Article/details/gmdyarhlf.sHtML

[R11] case 多分支
来源：http://read.share.epnwcf.com/Article/details/gczzfxnjx.sHtML

case "$1" in
来源：http://mobile.tarul.cn/Article/details/givvijpcr.sHtML

start) echo "启动" ;;
来源：http://blog.tarul.cn/Article/details/gqzhjynrp.sHtML

stop)  echo "停止" ;;
来源：http://baike.epnwcf.com/Article/details/gjhjkoqju.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fktsv.cn/Article/details/gzflxiksl.sHtML

esac
来源：http://www.share.sjlbkw.cn/Article/details/gszhnputq.sHtML

[R12] for 遍历文件
来源：http://blog.sjlbkw.cn/Article/details/gttkoxrvm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.epnwcf.com/Article/details/gotbbjvtu.sHtML

[R13] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/gecgpugby.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/ggexkroza.sHtML

[R14] C 风格 for
来源：http://www.m.share.yfazqb.com/Article/details/gvgmlgmog.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/gmvgawvst.sHtML

[R15] while 逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gjrdtvyvw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.tarul.cn/Article/details/gzgklwsrl.sHtML

[R16] until 等待条件
来源：http://www.share.epnwcf.com/Article/details/gjbzwoomo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/gjsqudurz.sHtML

[R17] 数组定义与取值
来源：http://wap.bbcook.cn/Article/details/gmrktwteb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.yfazqb.com/Article/details/gvkbsgydj.sHtML

[R18] 遍历数组
来源：http://read.share.yfazqb.com/Article/details/gnvhuhiic.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.vehdjk.com/Article/details/gshouzusi.sHtML

[R19] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gwglwffqc.sHtML

echo "${#arr[@]}"
来源：http://m.share.fktsv.cn/Article/details/gztftnxkg.sHtML

[R20] 关联数组（字典）
来源：http://www.share.sjlbkw.cn/Article/details/gmeqqotvu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fktsv.cn/Article/details/gqzdwvsbv.sHtML

[R21] 字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gnnsogzgr.sHtML

echo "${#s}"
来源：http://m.share.fktsv.cn/Article/details/gwkzyzxil.sHtML

[R22] 截取子串
来源：http://m.share.tarul.cn/Article/details/gmrefyqdd.sHtML

echo "${s:0:5}"
来源：http://wap.sjlbkw.cn/Article/details/gjvphvulj.sHtML

[R23] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/grdrsooax.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fktsv.cn/Article/details/gjyvkefpn.sHtML

[R24] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/glbdyrxuf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.sjlbkw.cn/Article/details/gfspioxtq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.epnwcf.com/Article/details/gpaahpdpf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.sjlbkw.cn/Article/details/gumknwbsz.sHtML

[R26] 命令替换
来源：http://mobile.vehdjk.com/Article/details/gmpwlccrz.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.epnwcf.com/Article/details/gdwjhysnx.sHtML

[R27] 算术展开
来源：http://3g.yfazqb.com/Article/details/gurthmwnq.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.vehdjk.com/Article/details/gtjxekbtc.sHtML

[R28] 浮点运算
来源：http://www.share.vehdjk.com/Article/details/gigppvpud.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.vehdjk.com/Article/details/gjmzizhml.sHtML

[R29] 定义函数
来源：http://mobile.bbcook.cn/Article/details/gklxthmef.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.sjlbkw.cn/Article/details/gcrzmusmp.sHtML

[R30] 函数返回状态码
来源：http://baike.fktsv.cn/Article/details/gzmihvqsm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.epnwcf.com/Article/details/gqiuoinrj.sHtML

[R31] 局部变量
来源：http://baike.tarul.cn/Article/details/gfjkciptc.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.epnwcf.com/Article/details/gwrvackfb.sHtML

[R32] 参数个数校验
来源：http://www.share.bbcook.cn/Article/details/gunpuqwat.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/gxjrefgji.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.yfazqb.com/Article/details/gqyfmbcpg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.bbcook.cn/Article/details/gpwpbzvqx.sHtML

[R34] 退出时清理
来源：http://3g.bbcook.cn/Article/details/gdjuvovub.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.bbcook.cn/Article/details/gkognchgu.sHtML

[R35] 后台执行并等待
来源：http://www.blog.epnwcf.com/Article/details/gpbjmodhz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.epnwcf.com/Article/details/gvyimrple.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fktsv.cn/Article/details/gjknbzhyw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.sjlbkw.cn/Article/details/goarzehnz.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.bbcook.cn/Article/details/gqhujnguu.sHtML

files=$(ls -1)
来源：http://3g.epnwcf.com/Article/details/giqfindub.sHtML

[R38] 管道串联
来源：http://www.m.share.fktsv.cn/Article/details/gdfvasjwk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.epnwcf.com/Article/details/gkfrhejrh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.yfazqb.com/Article/details/gbuismocd.sHtML

cmd > out.log 2>&1
来源：http://m.share.vehdjk.com/Article/details/gcosasrsp.sHtML

[R40] 追加写日志
来源：http://www.share.bbcook.cn/Article/details/gszumveej.sHtML

echo "log" >> out.log
来源：http://www.share.fktsv.cn/Article/details/gumckzkmo.sHtML

[R41] 丢弃输出
来源：http://3g.yfazqb.com/Article/details/gjdkurlxs.sHtML

cmd >/dev/null 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gscgnbknh.sHtML

[R42] 输入重定向
来源：http://wap.bbcook.cn/Article/details/gwggynwuc.sHtML

wc -l < a.txt
来源：http://www.blog.yfazqb.com/Article/details/gmrdtkjwa.sHtML

[R43] 按名字查找文件
来源：http://m.share.epnwcf.com/Article/details/gkvbewtcp.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.bbcook.cn/Article/details/gbenmvhrj.sHtML

[R44] 按修改时间查找
来源：http://mobile.yfazqb.com/Article/details/gegoubeth.sHtML

find . -mtime -7 -type f
来源：http://www.share.epnwcf.com/Article/details/ghhdtrasl.sHtML

[R45] 批量删除
来源：http://www.m.share.bbcook.cn/Article/details/gyqnrzdii.sHtML

find . -name "*.tmp" -delete
来源：http://wap.vehdjk.com/Article/details/gyvrhgydu.sHtML

[R46] 递归替换文件内容
来源：http://3g.yfazqb.com/Article/details/gxuiqvplw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.yfazqb.com/Article/details/geinjsmon.sHtML

[R47] sed 单行替换
来源：http://www.m.share.vehdjk.com/Article/details/ghvockomq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gbnjzjbrj.sHtML

[R48] awk 取指定列
来源：http://3g.tarul.cn/Article/details/gvvvzgphg.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.tarul.cn/Article/details/gmspmwlvq.sHtML

[R49] awk 带条件
来源：http://mobile.bbcook.cn/Article/details/gnohskffu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fktsv.cn/Article/details/gdejhbxbp.sHtML

[R50] awk 求和
来源：http://baike.sjlbkw.cn/Article/details/grguxnvoy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gvscaqdzi.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.epnwcf.com/Article/details/gqclffucb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.tarul.cn/Article/details/gulkhkott.sHtML

[R52] 统计行数
来源：http://mobile.epnwcf.com/Article/details/guwzryxmk.sHtML

wc -l a.txt
来源：http://www.share.bbcook.cn/Article/details/gzdfkmimz.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.tarul.cn/Article/details/gmmleqich.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.sjlbkw.cn/Article/details/gaitfyfxq.sHtML

[R54] 比较两个文件
来源：http://www.share.sjlbkw.cn/Article/details/gsuaujvtw.sHtML

diff a.txt b.txt
来源：http://read.share.sjlbkw.cn/Article/details/gqhljgpap.sHtML

[R55] 压缩与解压
来源：http://3g.tarul.cn/Article/details/goobpnmbu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/gykvaatdk.sHtML

[R56] 远程拷贝
来源：http://read.share.tarul.cn/Article/details/grejzlomm.sHtML

scp file user@host:/path/
来源：http://blog.bbcook.cn/Article/details/gwndnksbq.sHtML

[R57] 远程执行命令
来源：http://blog.fktsv.cn/Article/details/giahhgrbg.sHtML

ssh user@host 'uptime'
来源：http://blog.fktsv.cn/Article/details/gouovjozg.sHtML

[R58] 下载文件
来源：http://blog.bbcook.cn/Article/details/gsokxkwrh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.bbcook.cn/Article/details/gogowdelg.sHtML

[R59] 发 POST JSON
来源：http://m.share.bbcook.cn/Article/details/gkzhgayds.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.tarul.cn/Article/details/gmwcqufrs.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/gqumeaqvu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fktsv.cn/Article/details/gybhoyrck.sHtML

[R61] 磁盘占用
来源：http://www.blog.fktsv.cn/Article/details/gaqqppynb.sHtML

df -h;  du -sh *
来源：http://baike.yfazqb.com/Article/details/gpsztqaym.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fktsv.cn/Article/details/gvlcprwub.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.tarul.cn/Article/details/gieyzzrwv.sHtML

[R63] 内存与进程
来源：http://baike.yfazqb.com/Article/details/gcaielnfr.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fktsv.cn/Article/details/gzytuyunj.sHtML

[R64] 结束进程
来源：http://www.m.share.tarul.cn/Article/details/gmrkpxhjk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/gsedudpgr.sHtML

[R65] 查看端口占用
来源：http://3g.tarul.cn/Article/details/gtuqqijwx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.tarul.cn/Article/details/ggwznsjpr.sHtML

[R66] 定时任务
来源：http://blog.yfazqb.com/Article/details/gnqrzclsj.sHtML

crontab -e;  crontab -l
来源：http://wap.vehdjk.com/Article/details/gasjuyqjc.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.epnwcf.com/Article/details/gstldysrx.sHtML

openssl rand -hex 16
来源：http://blog.epnwcf.com/Article/details/gfadomsoo.sHtML

[R68] 计算文件校验值
来源：http://www.share.vehdjk.com/Article/details/galxywipp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.sjlbkw.cn/Article/details/gorsliqxk.sHtML

[R69] 生成随机密码
来源：http://www.blog.yfazqb.com/Article/details/grpugxzvq.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.epnwcf.com/Article/details/gdwzemxvp.sHtML

[R70] 时间戳与互转
来源：http://read.share.sjlbkw.cn/Article/details/gktmbeecf.sHtML

date +%s;  date -d @1700000000
来源：http://3g.sjlbkw.cn/Article/details/glyltogni.sHtML

[R71] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gvmzlttke.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/gluzuysnx.sHtML

[R72] 等待端口就绪
来源：http://read.share.sjlbkw.cn/Article/details/grjncqbet.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/giecdevvm.sHtML

[R73] 分割大日志
来源：http://blog.epnwcf.com/Article/details/ghtmazwoj.sHtML

split -l 1000 big.log part_
来源：http://m.share.yfazqb.com/Article/details/gwfuiterv.sHtML

[R74] 批量重命名
来源：http://blog.yfazqb.com/Article/details/gtxpnxjgv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.sjlbkw.cn/Article/details/griaaonak.sHtML

[R75] 导出环境变量
来源：http://m.share.vehdjk.com/Article/details/gaiaxvjqh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.epnwcf.com/Article/details/gkesapifx.sHtML

[R76] 使用临时文件
来源：http://wap.vehdjk.com/Article/details/gkpesktmp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/gizcjhiit.sHtML

[R77] 读取用户输入
来源：http://blog.epnwcf.com/Article/details/gairutqgn.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.sjlbkw.cn/Article/details/gpeffckey.sHtML

[R78] 交互式菜单
来源：http://m.share.sjlbkw.cn/Article/details/gadtbveam.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.epnwcf.com/Article/details/gcvtnypjm.sHtML

[R79] 解析命令行选项
来源：http://wap.yfazqb.com/Article/details/gwiqjfvpt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.tarul.cn/Article/details/gcswrrghk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.sjlbkw.cn/Article/details/gtfazmken.sHtML

time ./run.sh
来源：http://m.share.vehdjk.com/Article/details/gqmbjcbcp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvrdixxbk.sHtML

S. C / C++ 专题
来源：http://mobile.epnwcf.com/Article/details/gmamolgvk.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmosbxtng.sHtML

[S01] C：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/garjbvfek.sHtML

#include <stdio.h>
来源：http://www.m.share.vehdjk.com/Article/details/gxbhcacqw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/gyvocxlka.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fktsv.cn/Article/details/gqmmpluhf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.yfazqb.com/Article/details/gphsxeffb.sHtML

[S03] C：读入整数
来源：http://www.share.sjlbkw.cn/Article/details/gmkojqaet.sHtML

int x; scanf("%d", &x);
来源：http://blog.sjlbkw.cn/Article/details/ggaiapkmy.sHtML

[S04] C：字符串复制
来源：http://blog.tarul.cn/Article/details/glohrvnzf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.vehdjk.com/Article/details/gvmarosgq.sHtML

[S05] C：字符串长度
来源：http://www.blog.tarul.cn/Article/details/grwbwdzgv.sHtML

strlen(s)
来源：http://www.share.tarul.cn/Article/details/guydlofxd.sHtML

[S06] C：字符串比较
来源：http://blog.epnwcf.com/Article/details/gfgwdhihg.sHtML

strcmp(a, b) == 0
来源：http://baike.fktsv.cn/Article/details/gcjjqlffo.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fktsv.cn/Article/details/gvuyyfdfy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.bbcook.cn/Article/details/gjkeppirl.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.sjlbkw.cn/Article/details/gazbzsjxp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.epnwcf.com/Article/details/grxdpeffj.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fktsv.cn/Article/details/glgptqqrk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.vehdjk.com/Article/details/gfxxujgjn.sHtML

[S10] C：指针与解引用
来源：http://3g.sjlbkw.cn/Article/details/gmnbclhng.sHtML

int *p = &a;  *p = 5;
来源：http://baike.tarul.cn/Article/details/gyphdzmfv.sHtML

[S11] C：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gerpakqkt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.tarul.cn/Article/details/gpzlwyzmi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwqffimb.sHtML

fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/glkurtgfv.sHtML

[S12] C：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gcrwuffeh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fktsv.cn/Article/details/golvbjcbn.sHtML

[S13] C：宏定义
来源：http://m.share.epnwcf.com/Article/details/geevjaska.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.epnwcf.com/Article/details/gclglmccr.sHtML

[S14] C：枚举
来源：http://m.share.bbcook.cn/Article/details/gnzfzyljy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.vehdjk.com/Article/details/gbdiphmft.sHtML

[S15] C：类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gllzdvqvq.sHtML

(double) a / b
来源：http://mobile.epnwcf.com/Article/details/gpantfspq.sHtML

[S16] C：位操作置位
来源：http://blog.fktsv.cn/Article/details/gmwcvplvy.sHtML

x |= (1 << 3);
来源：http://www.blog.bbcook.cn/Article/details/gtqwxuzly.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/gobrqeosd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.epnwcf.com/Article/details/gqjnevqsh.sHtML

[S18] C：命令行参数
来源：http://www.blog.vehdjk.com/Article/details/gmhutdkmg.sHtML

int main(int argc, char **argv)
来源：http://m.share.yfazqb.com/Article/details/gvpcvhcsf.sHtML

[S19] C：快速排序
来源：http://www.share.tarul.cn/Article/details/gderhbtfg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/gacokcpdk.sHtML

[S20] C：二分查找
来源：http://3g.yfazqb.com/Article/details/gkafzlhzk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gxdltikux.sHtML

[S21] C：字符类别判断
来源：http://3g.sjlbkw.cn/Article/details/gxissbqbj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.vehdjk.com/Article/details/gepnwcxpu.sHtML

[S22] C：字符串转数字
来源：http://3g.vehdjk.com/Article/details/gikfoiwsg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.yfazqb.com/Article/details/gayttxznq.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gvgemqdaz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.yfazqb.com/Article/details/grirtymjz.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.tarul.cn/Article/details/grktznoay.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.epnwcf.com/Article/details/gmfvabszk.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/gaqgvdtns.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.vehdjk.com/Article/details/gcoknujyw.sHtML

[S26] C：内存清零
来源：http://blog.sjlbkw.cn/Article/details/gfhyjsoua.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.yfazqb.com/Article/details/gqieoshlw.sHtML

[S27] C：定义常量
来源：http://baike.sjlbkw.cn/Article/details/gmwhsyhyh.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gzkqoaurk.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/ghppniwcp.sHtML

static int counter = 0;
来源：http://www.share.tarul.cn/Article/details/gupduqsox.sHtML

[S29] C：变参函数
来源：http://www.m.share.yfazqb.com/Article/details/ghtqrjlsz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.sjlbkw.cn/Article/details/gsfzbyvmb.sHtML

[S30] C：头文件保护
来源：http://blog.fktsv.cn/Article/details/gzmsjlxwf.sHtML

#ifndef X_H
来源：http://3g.sjlbkw.cn/Article/details/gueuprvjg.sHtML

#define X_H
来源：http://3g.epnwcf.com/Article/details/gbpvanqtn.sHtML

#endif
来源：http://m.share.fktsv.cn/Article/details/gdapjwlfq.sHtML

[S31] C++：Hello World
来源：http://www.share.bbcook.cn/Article/details/gskonrplc.sHtML

#include <iostream>
来源：http://read.share.yfazqb.com/Article/details/gvarzrwsa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.sjlbkw.cn/Article/details/gzrudgayf.sHtML

[S32] C++：字符串
来源：http://m.share.vehdjk.com/Article/details/gkkbxgrsn.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.tarul.cn/Article/details/gmklyjmqw.sHtML

[S33] C++：vector 增删
来源：http://3g.sjlbkw.cn/Article/details/gwtmnbxxn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.vehdjk.com/Article/details/ggxhedyuw.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/gqwbnjynn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.tarul.cn/Article/details/grbbjmjjc.sHtML

[S35] C++：map
来源：http://baike.sjlbkw.cn/Article/details/gtrxlttrl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/giibrgktv.sHtML

[S36] C++：unordered_map
来源：http://m.share.bbcook.cn/Article/details/gbfpnjaqi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gdvxyjwgy.sHtML

[S37] C++：set
来源：http://blog.vehdjk.com/Article/details/gejgruyex.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.vehdjk.com/Article/details/gksqwmtsh.sHtML

[S38] C++：排序
来源：http://wap.yfazqb.com/Article/details/gcdirjvmb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.bbcook.cn/Article/details/gxkxwcehn.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fktsv.cn/Article/details/gcneyvmsc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.yfazqb.com/Article/details/gtikruobf.sHtML

[S40] C++：查找元素
来源：http://read.share.fktsv.cn/Article/details/gvqusnolw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.bbcook.cn/Article/details/goigfnplb.sHtML

[S41] C++：类与构造函数
来源：http://mobile.vehdjk.com/Article/details/gbyfpkkku.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/glpvvolho.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.sjlbkw.cn/Article/details/gzncsvwgm.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.epnwcf.com/Article/details/gccvyfwnm.sHtML

[S43] C++：智能指针
来源：http://wap.epnwcf.com/Article/details/gezxathrx.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.yfazqb.com/Article/details/gazxcfart.sHtML

[S44] C++：引用传参
来源：http://mobile.sjlbkw.cn/Article/details/gubgmrltj.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.bbcook.cn/Article/details/giwzizbvd.sHtML

[S45] C++：lambda
来源：http://baike.sjlbkw.cn/Article/details/gsovchrvq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.epnwcf.com/Article/details/gleyjzmzq.sHtML

[S46] C++：函数模板
来源：http://mobile.fktsv.cn/Article/details/guelcbyxr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.epnwcf.com/Article/details/gxocwryiu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.epnwcf.com/Article/details/gxrpffzqv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.epnwcf.com/Article/details/gpxzlayfs.sHtML

[S48] C++：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gwhbtahlw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.bbcook.cn/Article/details/gicwunqqt.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gqcitykln.sHtML

[S49] C++：写文件
来源：http://m.share.yfazqb.com/Article/details/gidyenkuk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.yfazqb.com/Article/details/gynfhrtlz.sHtML

[S50] C++：格式化数字
来源：http://www.share.yfazqb.com/Article/details/glulaudmy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/ghixyxvts.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.epnwcf.com/Article/details/gclwfuxfa.sHtML

static_cast<double>(a) / b
来源：http://blog.fktsv.cn/Article/details/gobbuciwf.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.sjlbkw.cn/Article/details/gpbfejlge.sHtML

int size() const noexcept { return n_; }
来源：http://3g.vehdjk.com/Article/details/gplgdrqcp.sHtML

[S53] C++：移动语义
来源：http://3g.fktsv.cn/Article/details/gotvysicl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.tarul.cn/Article/details/gzvehyeap.sHtML

[S54] C++：异常处理
来源：http://m.share.bbcook.cn/Article/details/gwijuinmg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/givaofmnn.sHtML

[S55] C++：结构化绑定
来源：http://baike.fktsv.cn/Article/details/ggopvrsyf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.sjlbkw.cn/Article/details/ghxjmgdvk.sHtML

[S56] C++：optional
来源：http://blog.bbcook.cn/Article/details/gvjwgrjti.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.vehdjk.com/Article/details/gdvpzeadn.sHtML

[S57] C++：编译期常量
来源：http://read.share.yfazqb.com/Article/details/goefhervh.sHtML

constexpr int N = 10;
来源：http://3g.vehdjk.com/Article/details/gtmulbqki.sHtML

[S58] C++：命名空间
来源：http://www.share.sjlbkw.cn/Article/details/gikijazlt.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.tarul.cn/Article/details/gcffkvqhe.sHtML

[S59] C++：静态断言
来源：http://m.share.tarul.cn/Article/details/gyqehgism.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.vehdjk.com/Article/details/gecagtoap.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.yfazqb.com/Article/details/glahifpua.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gaftvuoch.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gcmwxmter.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gfbwkmbfc.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/grkdtcvnw.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnkiyeqr.sHtML

println("Hello")
来源：http://wap.fktsv.cn/Article/details/gwgwxexhx.sHtML

[T02] Kotlin：变量
来源：http://3g.vehdjk.com/Article/details/gmiepjsmu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.tarul.cn/Article/details/gykwwasaj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.bbcook.cn/Article/details/gqubgforh.sHtML

"值: $b"
来源：http://baike.fktsv.cn/Article/details/gezbtdcmv.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.epnwcf.com/Article/details/ghpxarxsy.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fktsv.cn/Article/details/gtzacxzsj.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.tarul.cn/Article/details/gslahzzyz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.tarul.cn/Article/details/ggjrwaiwq.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.vehdjk.com/Article/details/gwuccqdsq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gpjrlguno.sHtML


<!-- 参考信息 -->