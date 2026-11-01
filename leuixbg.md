代发 wailian999

readonly PI=3.14
来源：http://read.share.yfazqb.com/Article/details/gdordtoyd.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/gazihqvfz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.epnwcf.com/Article/details/gyugiienp.sHtML

[R05] 参数默认值
来源：http://read.share.fktsv.cn/Article/details/gcxtbtswb.sHtML

name="${1:-default}"
来源：http://blog.epnwcf.com/Article/details/gujsimmug.sHtML

[R06] 判断命令是否存在
来源：http://3g.vehdjk.com/Article/details/gbjsaupql.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/guouzjhix.sHtML

[R07] if 判断文件
来源：http://3g.fktsv.cn/Article/details/gjkbikxyu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gzuskjkep.sHtML

[R08] 数值比较
来源：http://www.m.share.tarul.cn/Article/details/grbsrpeqk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.epnwcf.com/Article/details/gifscpedu.sHtML

[R09] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/gwocuawju.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.vehdjk.com/Article/details/gxjwucjrl.sHtML

[R10] 正则匹配
来源：http://www.m.share.tarul.cn/Article/details/grjnptzbg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.vehdjk.com/Article/details/gcklihode.sHtML

[R11] case 多分支
来源：http://m.share.vehdjk.com/Article/details/gszhssjqr.sHtML

case "$1" in
来源：http://baike.tarul.cn/Article/details/gaziwhkhf.sHtML

start) echo "启动" ;;
来源：http://3g.bbcook.cn/Article/details/gahlgvryb.sHtML

stop)  echo "停止" ;;
来源：http://blog.bbcook.cn/Article/details/gkcqjdfrq.sHtML

*)     echo "未知命令" ;;
来源：http://baike.epnwcf.com/Article/details/gfvchgmgr.sHtML

esac
来源：http://baike.tarul.cn/Article/details/gqsagjapg.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/gluxebkvx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.yfazqb.com/Article/details/gicxrwjse.sHtML

[R13] for 计数循环
来源：http://www.share.yfazqb.com/Article/details/gnqqtupjh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.yfazqb.com/Article/details/gnspqxccx.sHtML

[R14] C 风格 for
来源：http://baike.fktsv.cn/Article/details/gxpgxjddj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/gvaunwhqr.sHtML

[R15] while 逐行读文件
来源：http://baike.epnwcf.com/Article/details/gnktxwuxb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fktsv.cn/Article/details/gdiwelnbi.sHtML

[R16] until 等待条件
来源：http://blog.epnwcf.com/Article/details/gkoupzbhg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gigyfdkzw.sHtML

[R17] 数组定义与取值
来源：http://baike.yfazqb.com/Article/details/gheizxcmf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fktsv.cn/Article/details/gtibgdmrr.sHtML

[R18] 遍历数组
来源：http://blog.vehdjk.com/Article/details/gmyvfcory.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.epnwcf.com/Article/details/gimexmcgv.sHtML

[R19] 数组长度
来源：http://blog.epnwcf.com/Article/details/glthiytzh.sHtML

echo "${#arr[@]}"
来源：http://mobile.fktsv.cn/Article/details/gepbkdybi.sHtML

[R20] 关联数组（字典）
来源：http://baike.epnwcf.com/Article/details/gmxuhlymu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.yfazqb.com/Article/details/gpdnenvmh.sHtML

[R21] 字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gqdziouco.sHtML

echo "${#s}"
来源：http://www.blog.sjlbkw.cn/Article/details/guugsvfqs.sHtML

[R22] 截取子串
来源：http://m.share.bbcook.cn/Article/details/gyqwatjwu.sHtML

echo "${s:0:5}"
来源：http://www.blog.bbcook.cn/Article/details/gxmbcpizl.sHtML

[R23] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/glufsaojx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.bbcook.cn/Article/details/gbxxhyvsh.sHtML

[R24] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gnfrkcpow.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.tarul.cn/Article/details/gohhqqalo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.epnwcf.com/Article/details/gqrecwhpp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fktsv.cn/Article/details/guuauinpc.sHtML

[R26] 命令替换
来源：http://baike.vehdjk.com/Article/details/goylnaico.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.vehdjk.com/Article/details/gkobwmref.sHtML

[R27] 算术展开
来源：http://read.share.sjlbkw.cn/Article/details/gyjikhrlp.sHtML

echo $((1 + 2 * 3))
来源：http://blog.epnwcf.com/Article/details/grhcfoigl.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/gbtqqsrie.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.bbcook.cn/Article/details/gaxdujjns.sHtML

[R29] 定义函数
来源：http://blog.bbcook.cn/Article/details/guvwlmayf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fktsv.cn/Article/details/gtuxcwoop.sHtML

[R30] 函数返回状态码
来源：http://mobile.vehdjk.com/Article/details/gvkkztmrl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fktsv.cn/Article/details/gstkevfbo.sHtML

[R31] 局部变量
来源：http://mobile.bbcook.cn/Article/details/glsblfotb.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.vehdjk.com/Article/details/gpszqzepj.sHtML

[R32] 参数个数校验
来源：http://baike.sjlbkw.cn/Article/details/givliemmz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gwtaozvul.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.bbcook.cn/Article/details/gvtvvuila.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.vehdjk.com/Article/details/gpotvarmd.sHtML

[R34] 退出时清理
来源：http://baike.bbcook.cn/Article/details/gbsruewft.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/gxysfvesq.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/gvtlaldkq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.vehdjk.com/Article/details/grqcgkjxe.sHtML

[R36] 并发执行多个任务
来源：http://www.share.vehdjk.com/Article/details/gajxxtdix.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.sjlbkw.cn/Article/details/gaoafywqp.sHtML

[R37] 把输出赋给变量
来源：http://baike.epnwcf.com/Article/details/ggcghoduq.sHtML

files=$(ls -1)
来源：http://3g.bbcook.cn/Article/details/gknqjqlbl.sHtML

[R38] 管道串联
来源：http://mobile.tarul.cn/Article/details/gblievxgk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.bbcook.cn/Article/details/gvwhjdlnp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.bbcook.cn/Article/details/goagxhviu.sHtML

cmd > out.log 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gytcfbtvc.sHtML

[R40] 追加写日志
来源：http://www.share.bbcook.cn/Article/details/gjigbfzqx.sHtML

echo "log" >> out.log
来源：http://3g.tarul.cn/Article/details/gbtxipcgw.sHtML

[R41] 丢弃输出
来源：http://3g.bbcook.cn/Article/details/gcefzidiv.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fktsv.cn/Article/details/gsvtlqcwn.sHtML

[R42] 输入重定向
来源：http://www.share.bbcook.cn/Article/details/glhfewlip.sHtML

wc -l < a.txt
来源：http://www.share.yfazqb.com/Article/details/gmjnmkujz.sHtML

[R43] 按名字查找文件
来源：http://blog.vehdjk.com/Article/details/grgrizveh.sHtML

find . -name "*.log" -type f
来源：http://m.share.bbcook.cn/Article/details/gnvdpnucv.sHtML

[R44] 按修改时间查找
来源：http://www.share.tarul.cn/Article/details/gyuekawcc.sHtML

find . -mtime -7 -type f
来源：http://www.share.sjlbkw.cn/Article/details/gabpwbzge.sHtML

[R45] 批量删除
来源：http://mobile.vehdjk.com/Article/details/ghkvlsvso.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gdkurloor.sHtML

[R46] 递归替换文件内容
来源：http://m.share.bbcook.cn/Article/details/gnwreftfh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.sjlbkw.cn/Article/details/gdyvtxwws.sHtML

[R47] sed 单行替换
来源：http://read.share.tarul.cn/Article/details/gycrrayvi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.bbcook.cn/Article/details/ggrqqqtko.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/grlkomtzn.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fktsv.cn/Article/details/gjsvvkzmq.sHtML

[R49] awk 带条件
来源：http://baike.yfazqb.com/Article/details/gbiypeuxr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.yfazqb.com/Article/details/gekwuwekn.sHtML

[R50] awk 求和
来源：http://www.m.share.vehdjk.com/Article/details/gkexhzlce.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fktsv.cn/Article/details/gzqpmwtle.sHtML

[R51] 排序去重取前几
来源：http://mobile.sjlbkw.cn/Article/details/guunosxmw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.epnwcf.com/Article/details/gzfowrqxv.sHtML

[R52] 统计行数
来源：http://www.m.share.yfazqb.com/Article/details/gubxogyyv.sHtML

wc -l a.txt
来源：http://3g.bbcook.cn/Article/details/gjzbwzhht.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.vehdjk.com/Article/details/ggjhwpncr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.bbcook.cn/Article/details/gvfmobdnw.sHtML

[R54] 比较两个文件
来源：http://mobile.sjlbkw.cn/Article/details/gjyghqmrt.sHtML

diff a.txt b.txt
来源：http://3g.yfazqb.com/Article/details/gibwdyzry.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fktsv.cn/Article/details/gtqfsdzrl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.bbcook.cn/Article/details/gbqhoyyum.sHtML

[R56] 远程拷贝
来源：http://m.share.yfazqb.com/Article/details/gpbxqratz.sHtML

scp file user@host:/path/
来源：http://baike.yfazqb.com/Article/details/gaajjxqgv.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fktsv.cn/Article/details/ggflnxaqf.sHtML

ssh user@host 'uptime'
来源：http://www.share.yfazqb.com/Article/details/gjnspdddy.sHtML

[R58] 下载文件
来源：http://www.share.bbcook.cn/Article/details/gxxnwfjto.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/geyvivacq.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/guvuduchf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.sjlbkw.cn/Article/details/gkyjkasqr.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/gjcexlpsq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.sjlbkw.cn/Article/details/gwdwuyizz.sHtML

[R61] 磁盘占用
来源：http://mobile.epnwcf.com/Article/details/gmsoujukb.sHtML

df -h;  du -sh *
来源：http://wap.fktsv.cn/Article/details/gsbypjgot.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.vehdjk.com/Article/details/gtivxidwb.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.yfazqb.com/Article/details/gtpkwncgi.sHtML

[R63] 内存与进程
来源：http://www.m.share.bbcook.cn/Article/details/gmqfnsobc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.bbcook.cn/Article/details/ghgjlihkd.sHtML

[R64] 结束进程
来源：http://www.share.tarul.cn/Article/details/grjnpgxzl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.yfazqb.com/Article/details/gnsoukxyy.sHtML

[R65] 查看端口占用
来源：http://m.share.sjlbkw.cn/Article/details/gidninwss.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.yfazqb.com/Article/details/gappkcmfd.sHtML

[R66] 定时任务
来源：http://mobile.yfazqb.com/Article/details/gxfznihdy.sHtML

crontab -e;  crontab -l
来源：http://baike.vehdjk.com/Article/details/ggljtktgg.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fktsv.cn/Article/details/gbkmwhjks.sHtML

openssl rand -hex 16
来源：http://baike.yfazqb.com/Article/details/gujvyniit.sHtML

[R68] 计算文件校验值
来源：http://baike.epnwcf.com/Article/details/glhlmstrr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.epnwcf.com/Article/details/gkjjwcbdy.sHtML

[R69] 生成随机密码
来源：http://read.share.tarul.cn/Article/details/gbquamqqf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.sjlbkw.cn/Article/details/gzkoqgvsl.sHtML

[R70] 时间戳与互转
来源：http://mobile.sjlbkw.cn/Article/details/gwmyvjjsy.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.sjlbkw.cn/Article/details/gzbajyjkf.sHtML

[R71] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/goactldwp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.vehdjk.com/Article/details/gvzwhuzjz.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fktsv.cn/Article/details/gczmubwnp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/gowotwzcm.sHtML

[R73] 分割大日志
来源：http://wap.bbcook.cn/Article/details/ghzbuxyuo.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/geddssxei.sHtML

[R74] 批量重命名
来源：http://www.share.bbcook.cn/Article/details/gjtgxjjfp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.vehdjk.com/Article/details/gnmzkazqd.sHtML

[R75] 导出环境变量
来源：http://wap.fktsv.cn/Article/details/gkofgrepg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.yfazqb.com/Article/details/gaoblkqyc.sHtML

[R76] 使用临时文件
来源：http://wap.yfazqb.com/Article/details/gvjlmpgvs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gfpyjclsv.sHtML

[R77] 读取用户输入
来源：http://3g.bbcook.cn/Article/details/gyulvzsbk.sHtML

read -rp "请输入: " ans
来源：http://read.share.epnwcf.com/Article/details/gitvkcmjv.sHtML

[R78] 交互式菜单
来源：http://3g.fktsv.cn/Article/details/gfdgmhrpz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.bbcook.cn/Article/details/gnckxfxiq.sHtML

[R79] 解析命令行选项
来源：http://read.share.fktsv.cn/Article/details/gokpbdehu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.vehdjk.com/Article/details/grwefhynk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.bbcook.cn/Article/details/gjunfrxki.sHtML

time ./run.sh
来源：http://www.blog.vehdjk.com/Article/details/gwzawsguz.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grwjhjvtv.sHtML

S. C / C++ 专题
来源：http://blog.vehdjk.com/Article/details/gkwhjkvue.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtdmmfzr.sHtML

[S01] C：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gpzbkwoot.sHtML

#include <stdio.h>
来源：http://blog.vehdjk.com/Article/details/gxvtxxqib.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/gqovcgkgo.sHtML

[S02] C：变量与格式化输出
来源：http://baike.tarul.cn/Article/details/gpxeiwxtd.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.sjlbkw.cn/Article/details/gixlwnftf.sHtML

[S03] C：读入整数
来源：http://m.share.bbcook.cn/Article/details/gssyybwrf.sHtML

int x; scanf("%d", &x);
来源：http://www.share.bbcook.cn/Article/details/gjipfzdgk.sHtML

[S04] C：字符串复制
来源：http://mobile.sjlbkw.cn/Article/details/gadnypwbn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.bbcook.cn/Article/details/gpfngpahj.sHtML

[S05] C：字符串长度
来源：http://baike.fktsv.cn/Article/details/grcoytqtn.sHtML

strlen(s)
来源：http://m.share.epnwcf.com/Article/details/gpysywzah.sHtML

[S06] C：字符串比较
来源：http://wap.vehdjk.com/Article/details/gacxqycam.sHtML

strcmp(a, b) == 0
来源：http://www.share.sjlbkw.cn/Article/details/glfqetlbd.sHtML

[S07] C：数组遍历求和
来源：http://www.share.bbcook.cn/Article/details/getheawtd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.sjlbkw.cn/Article/details/gnmjvcokk.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.epnwcf.com/Article/details/glhwehluv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.sjlbkw.cn/Article/details/gbjjcbfyj.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.epnwcf.com/Article/details/gmnetgiqa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.vehdjk.com/Article/details/gqojxqihz.sHtML

[S10] C：指针与解引用
来源：http://blog.bbcook.cn/Article/details/ggjmmiung.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/gxblbzqxw.sHtML

[S11] C：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gjuzhkhhj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.yfazqb.com/Article/details/gxavgznxs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.bbcook.cn/Article/details/gtdhamrht.sHtML

fclose(f);
来源：http://blog.yfazqb.com/Article/details/gryrfsimx.sHtML

[S12] C：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/goozomfmv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/grhvgwrhg.sHtML

[S13] C：宏定义
来源：http://m.share.bbcook.cn/Article/details/gzoxhlior.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.vehdjk.com/Article/details/gqgwnzhou.sHtML

[S14] C：枚举
来源：http://m.share.tarul.cn/Article/details/gudgtbkal.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.tarul.cn/Article/details/gdlzbrssu.sHtML

[S15] C：类型转换
来源：http://blog.sjlbkw.cn/Article/details/gilyxjnya.sHtML

(double) a / b
来源：http://3g.epnwcf.com/Article/details/gwrarrbnx.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fktsv.cn/Article/details/gtihfuyyz.sHtML

x |= (1 << 3);
来源：http://mobile.sjlbkw.cn/Article/details/gjfcwifua.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fktsv.cn/Article/details/giogcnxzx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.vehdjk.com/Article/details/gypxrvjmx.sHtML

[S18] C：命令行参数
来源：http://m.share.tarul.cn/Article/details/gwyxbukxi.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fktsv.cn/Article/details/gpxwyvasf.sHtML

[S19] C：快速排序
来源：http://www.blog.sjlbkw.cn/Article/details/gebwiqpea.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/guqhvnoua.sHtML

[S20] C：二分查找
来源：http://blog.fktsv.cn/Article/details/gdwdkaqml.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gdamoogid.sHtML

[S21] C：字符类别判断
来源：http://blog.tarul.cn/Article/details/gvqjehnhg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.epnwcf.com/Article/details/guylkgdqq.sHtML

[S22] C：字符串转数字
来源：http://3g.bbcook.cn/Article/details/gpoysizqf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.epnwcf.com/Article/details/gubgwspni.sHtML

[S23] C：随机数
来源：http://3g.fktsv.cn/Article/details/goxiceoud.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.bbcook.cn/Article/details/gbqfrette.sHtML

[S24] C：获取本地时间
来源：http://mobile.sjlbkw.cn/Article/details/giejoszye.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.vehdjk.com/Article/details/gxhzejsng.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/gypdrkqmk.sHtML

memcpy(dst, src, n);
来源：http://mobile.yfazqb.com/Article/details/ghddzedkh.sHtML

[S26] C：内存清零
来源：http://wap.bbcook.cn/Article/details/giuotsncl.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.bbcook.cn/Article/details/goxwxnkii.sHtML

[S27] C：定义常量
来源：http://baike.sjlbkw.cn/Article/details/ganqoebgo.sHtML

const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gmgtnywyo.sHtML

[S28] C：静态变量
来源：http://mobile.bbcook.cn/Article/details/gnqocetma.sHtML

static int counter = 0;
来源：http://mobile.yfazqb.com/Article/details/glkikpcyd.sHtML

[S29] C：变参函数
来源：http://read.share.sjlbkw.cn/Article/details/gsuilanvz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.bbcook.cn/Article/details/gijsvcmjj.sHtML

[S30] C：头文件保护
来源：http://baike.yfazqb.com/Article/details/gyennfznz.sHtML

#ifndef X_H
来源：http://www.blog.fktsv.cn/Article/details/gdeoasqfq.sHtML

#define X_H
来源：http://blog.bbcook.cn/Article/details/gvpnioyrs.sHtML

#endif
来源：http://m.share.fktsv.cn/Article/details/gtacrfcag.sHtML

[S31] C++：Hello World
来源：http://read.share.bbcook.cn/Article/details/gjtqzrrme.sHtML

#include <iostream>
来源：http://www.share.vehdjk.com/Article/details/gtxoovovh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fktsv.cn/Article/details/gpglencmy.sHtML

[S32] C++：字符串
来源：http://mobile.fktsv.cn/Article/details/gakljisaa.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.tarul.cn/Article/details/gfvdmqljr.sHtML

[S33] C++：vector 增删
来源：http://mobile.epnwcf.com/Article/details/gfcswiost.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.bbcook.cn/Article/details/ghdrqeske.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/gpwjrauuf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.bbcook.cn/Article/details/gktbnwhlt.sHtML

[S35] C++：map
来源：http://3g.epnwcf.com/Article/details/gchxnonim.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/grqeuqjrq.sHtML

[S36] C++：unordered_map
来源：http://blog.tarul.cn/Article/details/gnwwdzhnb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gnxzwsvca.sHtML

[S37] C++：set
来源：http://wap.sjlbkw.cn/Article/details/ggfmjvckq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/ghtegtpeh.sHtML

[S38] C++：排序
来源：http://blog.bbcook.cn/Article/details/gjymugepp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gksqenvlf.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.sjlbkw.cn/Article/details/gxpwcbcia.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.tarul.cn/Article/details/ghhyxwzke.sHtML

[S40] C++：查找元素
来源：http://baike.fktsv.cn/Article/details/gkjabwkut.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.epnwcf.com/Article/details/gwneyiizp.sHtML

[S41] C++：类与构造函数
来源：http://wap.fktsv.cn/Article/details/gbqlfmike.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.tarul.cn/Article/details/gdpvxhckq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/gfsutfnwz.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fktsv.cn/Article/details/geqivqpvk.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fktsv.cn/Article/details/gbdzkhmwt.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fktsv.cn/Article/details/gfyibcswj.sHtML

[S44] C++：引用传参
来源：http://www.m.share.yfazqb.com/Article/details/gyjfanzry.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.epnwcf.com/Article/details/gxrlpeidx.sHtML

[S45] C++：lambda
来源：http://baike.fktsv.cn/Article/details/glqfnshqj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.yfazqb.com/Article/details/gtfqwftvu.sHtML

[S46] C++：函数模板
来源：http://wap.fktsv.cn/Article/details/gjxuevawf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.vehdjk.com/Article/details/gwfzppmkf.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.tarul.cn/Article/details/gjqqftwmq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.sjlbkw.cn/Article/details/gycmgbzdz.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gqvqhtvaa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.epnwcf.com/Article/details/ggzgjbewh.sHtML

while (std::getline(in, line)) { }
来源：http://baike.epnwcf.com/Article/details/gxwysdecz.sHtML

[S49] C++：写文件
来源：http://read.share.fktsv.cn/Article/details/gurwbwmky.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.tarul.cn/Article/details/gynjhmesn.sHtML

[S50] C++：格式化数字
来源：http://mobile.yfazqb.com/Article/details/gnqejimnp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gcwjnhtso.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fktsv.cn/Article/details/gnoeddxmo.sHtML

static_cast<double>(a) / b
来源：http://baike.yfazqb.com/Article/details/gjspdqufi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.yfazqb.com/Article/details/gxiiwipgi.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fktsv.cn/Article/details/gusmhemwq.sHtML

[S53] C++：移动语义
来源：http://www.blog.tarul.cn/Article/details/ghvsmedzy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.vehdjk.com/Article/details/glhnkmgde.sHtML

[S54] C++：异常处理
来源：http://www.share.epnwcf.com/Article/details/ghtdcabhv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.vehdjk.com/Article/details/gtdqgnfih.sHtML

[S55] C++：结构化绑定
来源：http://3g.yfazqb.com/Article/details/gpkgrmvqn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fktsv.cn/Article/details/greclnuzr.sHtML

[S56] C++：optional
来源：http://read.share.sjlbkw.cn/Article/details/ghqlcyayw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.epnwcf.com/Article/details/gcrcozqjr.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.vehdjk.com/Article/details/gxflqdxgz.sHtML

constexpr int N = 10;
来源：http://3g.yfazqb.com/Article/details/gxiwcrhgh.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/gvfqhlags.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.epnwcf.com/Article/details/gddculeby.sHtML

[S59] C++：静态断言
来源：http://www.share.vehdjk.com/Article/details/gfocahnlu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fktsv.cn/Article/details/ggdoixgbi.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/guaampvto.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.vehdjk.com/Article/details/gicmbycno.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfplddypc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gfxoffelh.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gqbxqjpif.sHtML

[T01] Kotlin：Hello World
来源：http://blog.bbcook.cn/Article/details/gtavshnjk.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gqhwaypss.sHtML

[T02] Kotlin：变量
来源：http://3g.tarul.cn/Article/details/ghwdgwnml.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.sjlbkw.cn/Article/details/gbspvbsgj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.sjlbkw.cn/Article/details/gqexthrvj.sHtML

"值: $b"
来源：http://www.blog.fktsv.cn/Article/details/gfyebtnot.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fktsv.cn/Article/details/gsgngnwer.sHtML

val n: String? = null;  n?.length
来源：http://m.share.tarul.cn/Article/details/gsxvmxvan.sHtML


<!-- 参考信息 -->