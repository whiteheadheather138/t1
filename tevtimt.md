代发 wailian999

set -euo pipefail
来源：http://baike.bbcook.cn/Article/details/gznnrlmyp.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwutrqad.sHtML

name="Tom"; echo "$name"
来源：http://m.share.sjlbkw.cn/Article/details/giilwkjgt.sHtML

[R03] 只读变量
来源：http://wap.tarul.cn/Article/details/gpxokpqbd.sHtML

readonly PI=3.14
来源：http://www.share.bbcook.cn/Article/details/gdwfptavb.sHtML

[R04] 位置参数
来源：http://www.blog.tarul.cn/Article/details/glpxfnxbe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.yfazqb.com/Article/details/ghfyiwwmm.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/gcftkgreq.sHtML

name="${1:-default}"
来源：http://blog.sjlbkw.cn/Article/details/gpdzmzogr.sHtML

[R06] 判断命令是否存在
来源：http://www.share.yfazqb.com/Article/details/gjocbrcoe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gbrcksrua.sHtML

[R07] if 判断文件
来源：http://baike.fktsv.cn/Article/details/glggzhrwe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.vehdjk.com/Article/details/gokbnrztc.sHtML

[R08] 数值比较
来源：http://mobile.yfazqb.com/Article/details/gmhrewiyr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.epnwcf.com/Article/details/gjbkweuah.sHtML

[R09] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gcnzmebjq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.tarul.cn/Article/details/gjhzagnhy.sHtML

[R10] 正则匹配
来源：http://m.share.yfazqb.com/Article/details/gzeiqrlaz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.bbcook.cn/Article/details/ggbrolhry.sHtML

[R11] case 多分支
来源：http://www.blog.tarul.cn/Article/details/gcapykklx.sHtML

case "$1" in
来源：http://www.blog.vehdjk.com/Article/details/gbrilplyi.sHtML

start) echo "启动" ;;
来源：http://www.m.share.tarul.cn/Article/details/gohlkdjaz.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.tarul.cn/Article/details/gmwqetaow.sHtML

*)     echo "未知命令" ;;
来源：http://blog.sjlbkw.cn/Article/details/gbeoviwxh.sHtML

esac
来源：http://www.blog.tarul.cn/Article/details/gygrapwpr.sHtML

[R12] for 遍历文件
来源：http://wap.vehdjk.com/Article/details/gcsmogwwy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.epnwcf.com/Article/details/gpwiexdnq.sHtML

[R13] for 计数循环
来源：http://baike.bbcook.cn/Article/details/gntllgkcm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/ggzzsdjih.sHtML

[R14] C 风格 for
来源：http://3g.sjlbkw.cn/Article/details/gjxdxgvsp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/gyidmnead.sHtML

[R15] while 逐行读文件
来源：http://baike.fktsv.cn/Article/details/gomdjhglm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.sjlbkw.cn/Article/details/gpahapkgu.sHtML

[R16] until 等待条件
来源：http://read.share.yfazqb.com/Article/details/gimwvmduv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gbyrzvwae.sHtML

[R17] 数组定义与取值
来源：http://3g.yfazqb.com/Article/details/gyyotfuky.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.bbcook.cn/Article/details/gphbslhhp.sHtML

[R18] 遍历数组
来源：http://wap.epnwcf.com/Article/details/ghhvkujnk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.sjlbkw.cn/Article/details/gojzfbzoq.sHtML

[R19] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/grhfplwee.sHtML

echo "${#arr[@]}"
来源：http://m.share.tarul.cn/Article/details/gexjucapn.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.epnwcf.com/Article/details/gijrwukik.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/grvenmzjn.sHtML

[R21] 字符串长度
来源：http://blog.tarul.cn/Article/details/gyehkadxn.sHtML

echo "${#s}"
来源：http://mobile.tarul.cn/Article/details/ggigzrwwj.sHtML

[R22] 截取子串
来源：http://blog.tarul.cn/Article/details/gdxgsygnv.sHtML

echo "${s:0:5}"
来源：http://read.share.yfazqb.com/Article/details/gadrgeflr.sHtML

[R23] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gyazfeimu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.yfazqb.com/Article/details/gmonycagr.sHtML

[R24] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gulasdyul.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fktsv.cn/Article/details/guzlutlsb.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.sjlbkw.cn/Article/details/gnqomcucw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.vehdjk.com/Article/details/gelxsunpf.sHtML

[R26] 命令替换
来源：http://3g.epnwcf.com/Article/details/gjfphzyrn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.yfazqb.com/Article/details/gdvirtdsv.sHtML

[R27] 算术展开
来源：http://wap.epnwcf.com/Article/details/glupuhsng.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.vehdjk.com/Article/details/gnoewszff.sHtML

[R28] 浮点运算
来源：http://baike.epnwcf.com/Article/details/glrkawcbn.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fktsv.cn/Article/details/gumuckswt.sHtML

[R29] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/gzisglgmv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fktsv.cn/Article/details/gxdxzxpgz.sHtML

[R30] 函数返回状态码
来源：http://wap.vehdjk.com/Article/details/gmgmtokms.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.yfazqb.com/Article/details/gguwljzwq.sHtML

[R31] 局部变量
来源：http://wap.yfazqb.com/Article/details/gtbijyepv.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.epnwcf.com/Article/details/ghadltgul.sHtML

[R32] 参数个数校验
来源：http://www.blog.sjlbkw.cn/Article/details/gkijggvfz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/goizrnlzo.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.epnwcf.com/Article/details/goqefavyt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.tarul.cn/Article/details/gyjibgzzn.sHtML

[R34] 退出时清理
来源：http://blog.vehdjk.com/Article/details/gqmsbniih.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/gumgaxakc.sHtML

[R35] 后台执行并等待
来源：http://baike.bbcook.cn/Article/details/gjrvtstow.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.tarul.cn/Article/details/gbbtbyfsd.sHtML

[R36] 并发执行多个任务
来源：http://3g.epnwcf.com/Article/details/gpxhfpilp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.vehdjk.com/Article/details/gamzukxtv.sHtML

[R37] 把输出赋给变量
来源：http://m.share.sjlbkw.cn/Article/details/grdhjfhti.sHtML

files=$(ls -1)
来源：http://blog.bbcook.cn/Article/details/gwukqnngq.sHtML

[R38] 管道串联
来源：http://www.blog.epnwcf.com/Article/details/guoovgmtx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.epnwcf.com/Article/details/gcsasnvvo.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fktsv.cn/Article/details/gssfkamvk.sHtML

cmd > out.log 2>&1
来源：http://mobile.sjlbkw.cn/Article/details/ghbjoidka.sHtML

[R40] 追加写日志
来源：http://3g.vehdjk.com/Article/details/gifxavblt.sHtML

echo "log" >> out.log
来源：http://read.share.bbcook.cn/Article/details/gjsumzbtj.sHtML

[R41] 丢弃输出
来源：http://wap.tarul.cn/Article/details/gebupahuy.sHtML

cmd >/dev/null 2>&1
来源：http://3g.tarul.cn/Article/details/gadadewxk.sHtML

[R42] 输入重定向
来源：http://read.share.bbcook.cn/Article/details/gcmqgtwiv.sHtML

wc -l < a.txt
来源：http://www.m.share.fktsv.cn/Article/details/geepqnbtg.sHtML

[R43] 按名字查找文件
来源：http://m.share.yfazqb.com/Article/details/gkuhgkrug.sHtML

find . -name "*.log" -type f
来源：http://mobile.epnwcf.com/Article/details/gnyizwluk.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gwuluieti.sHtML

find . -mtime -7 -type f
来源：http://www.share.fktsv.cn/Article/details/gnfllauoo.sHtML

[R45] 批量删除
来源：http://www.share.sjlbkw.cn/Article/details/gadxeaizw.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.sjlbkw.cn/Article/details/gjreavpzf.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.yfazqb.com/Article/details/gakkkgsdf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.sjlbkw.cn/Article/details/gbqlsynmy.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/guzzwvxpd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.tarul.cn/Article/details/ghlfvkawd.sHtML

[R48] awk 取指定列
来源：http://mobile.bbcook.cn/Article/details/gpyxnzzyf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gwdkuagyg.sHtML

[R49] awk 带条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gyklgoghh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.yfazqb.com/Article/details/gneddirrj.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/gdqfbplal.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.tarul.cn/Article/details/gfkulggbg.sHtML

[R51] 排序去重取前几
来源：http://blog.bbcook.cn/Article/details/gnttdiekz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.yfazqb.com/Article/details/gccolckip.sHtML

[R52] 统计行数
来源：http://blog.bbcook.cn/Article/details/gejviwjxz.sHtML

wc -l a.txt
来源：http://m.share.epnwcf.com/Article/details/ghnebswit.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.tarul.cn/Article/details/gfctvhpsi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.tarul.cn/Article/details/ghwdlhnfr.sHtML

[R54] 比较两个文件
来源：http://mobile.yfazqb.com/Article/details/grhgxzdev.sHtML

diff a.txt b.txt
来源：http://wap.sjlbkw.cn/Article/details/gvxopvbmx.sHtML

[R55] 压缩与解压
来源：http://blog.vehdjk.com/Article/details/gsgoxxcqt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.yfazqb.com/Article/details/gkaoabjcc.sHtML

[R56] 远程拷贝
来源：http://blog.tarul.cn/Article/details/gxyqronmv.sHtML

scp file user@host:/path/
来源：http://3g.epnwcf.com/Article/details/gfkmeibjd.sHtML

[R57] 远程执行命令
来源：http://mobile.epnwcf.com/Article/details/gjottndzr.sHtML

ssh user@host 'uptime'
来源：http://mobile.sjlbkw.cn/Article/details/gymjvomjq.sHtML

[R58] 下载文件
来源：http://mobile.vehdjk.com/Article/details/gnfecnyjf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/goyvehzfs.sHtML

[R59] 发 POST JSON
来源：http://m.share.yfazqb.com/Article/details/gfbxxfbnr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.epnwcf.com/Article/details/gwtihcsso.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/glvktbwsh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fktsv.cn/Article/details/gwhwshycq.sHtML

[R61] 磁盘占用
来源：http://m.share.fktsv.cn/Article/details/gmuaqoqty.sHtML

df -h;  du -sh *
来源：http://www.m.share.fktsv.cn/Article/details/gbxumrzta.sHtML

[R62] 找最占空间的文件
来源：http://baike.sjlbkw.cn/Article/details/gufknhizd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.vehdjk.com/Article/details/gzmtbtvls.sHtML

[R63] 内存与进程
来源：http://www.m.share.tarul.cn/Article/details/gtvnqtbwd.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.bbcook.cn/Article/details/gnpomulsl.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/gtleaeqxb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.epnwcf.com/Article/details/gcdbfkwig.sHtML

[R65] 查看端口占用
来源：http://m.share.sjlbkw.cn/Article/details/gyiyylmkd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.vehdjk.com/Article/details/gemuiizvg.sHtML

[R66] 定时任务
来源：http://m.share.epnwcf.com/Article/details/ggsbpztlq.sHtML

crontab -e;  crontab -l
来源：http://www.blog.yfazqb.com/Article/details/gbnpjlhji.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fktsv.cn/Article/details/gthwfonqt.sHtML

openssl rand -hex 16
来源：http://www.blog.yfazqb.com/Article/details/gkkuoffhq.sHtML

[R68] 计算文件校验值
来源：http://www.blog.yfazqb.com/Article/details/gsibgsewc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gxhqnvfjy.sHtML

[R69] 生成随机密码
来源：http://blog.fktsv.cn/Article/details/gzcqwwque.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.vehdjk.com/Article/details/gyaixuvpc.sHtML

[R70] 时间戳与互转
来源：http://m.share.epnwcf.com/Article/details/gjvvmolca.sHtML

date +%s;  date -d @1700000000
来源：http://blog.sjlbkw.cn/Article/details/gzyvmicre.sHtML

[R71] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/gtgtwpngg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.vehdjk.com/Article/details/gsmxwvlhq.sHtML

[R72] 等待端口就绪
来源：http://read.share.epnwcf.com/Article/details/gzwsxhdrs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gguagfoud.sHtML

[R73] 分割大日志
来源：http://www.m.share.fktsv.cn/Article/details/gomvpsveg.sHtML

split -l 1000 big.log part_
来源：http://3g.yfazqb.com/Article/details/gdrqucylx.sHtML

[R74] 批量重命名
来源：http://m.share.tarul.cn/Article/details/gwhmvhlta.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.yfazqb.com/Article/details/gthdnkpca.sHtML

[R75] 导出环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/geqhviing.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.bbcook.cn/Article/details/gfwykforw.sHtML

[R76] 使用临时文件
来源：http://www.blog.epnwcf.com/Article/details/gjrapgfrm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/ggyaflcoa.sHtML

[R77] 读取用户输入
来源：http://www.blog.sjlbkw.cn/Article/details/gdkinbxee.sHtML

read -rp "请输入: " ans
来源：http://mobile.yfazqb.com/Article/details/gnzlcajbn.sHtML

[R78] 交互式菜单
来源：http://wap.tarul.cn/Article/details/gghbgbfwc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.tarul.cn/Article/details/gmoxtkgih.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.epnwcf.com/Article/details/gtryryrgo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fktsv.cn/Article/details/golctldsw.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.yfazqb.com/Article/details/gobkkhvfy.sHtML

time ./run.sh
来源：http://www.blog.vehdjk.com/Article/details/glrzyazes.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/granhluet.sHtML

S. C / C++ 专题
来源：http://baike.epnwcf.com/Article/details/gukkuuhjr.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gaonsilvm.sHtML

[S01] C：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/ggffncqvi.sHtML

#include <stdio.h>
来源：http://wap.vehdjk.com/Article/details/gadycfahr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fktsv.cn/Article/details/gtebxlrlp.sHtML

[S02] C：变量与格式化输出
来源：http://blog.epnwcf.com/Article/details/gpdkkgcmq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.vehdjk.com/Article/details/gniugxwqi.sHtML

[S03] C：读入整数
来源：http://www.share.epnwcf.com/Article/details/gxmgpsmip.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.sjlbkw.cn/Article/details/gqgbiqlpj.sHtML

[S04] C：字符串复制
来源：http://read.share.vehdjk.com/Article/details/gsezrhrjx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.sjlbkw.cn/Article/details/glpktwaza.sHtML

[S05] C：字符串长度
来源：http://wap.tarul.cn/Article/details/gpwfcfowv.sHtML

strlen(s)
来源：http://www.m.share.vehdjk.com/Article/details/gbhwxlpgf.sHtML

[S06] C：字符串比较
来源：http://mobile.fktsv.cn/Article/details/gtajjvtrw.sHtML

strcmp(a, b) == 0
来源：http://3g.epnwcf.com/Article/details/gttxzdfrz.sHtML

[S07] C：数组遍历求和
来源：http://baike.fktsv.cn/Article/details/gjokhxxsb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.tarul.cn/Article/details/gvvqeslxk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.epnwcf.com/Article/details/gyhmdfljh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.sjlbkw.cn/Article/details/gpuskslhx.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.sjlbkw.cn/Article/details/geovdlkok.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.epnwcf.com/Article/details/gkroanfwu.sHtML

[S10] C：指针与解引用
来源：http://read.share.bbcook.cn/Article/details/gfivirehi.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.yfazqb.com/Article/details/gcvsdaigw.sHtML

[S11] C：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gtobmvmvd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fktsv.cn/Article/details/gtjjxozgu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.tarul.cn/Article/details/gcnnhklzd.sHtML

fclose(f);
来源：http://blog.epnwcf.com/Article/details/gzynlwfuz.sHtML

[S12] C：写文件
来源：http://www.blog.tarul.cn/Article/details/gsoyjbubj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.epnwcf.com/Article/details/gxwonfkrd.sHtML

[S13] C：宏定义
来源：http://www.share.tarul.cn/Article/details/gndakfdym.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.sjlbkw.cn/Article/details/gbkzobuij.sHtML

[S14] C：枚举
来源：http://www.share.vehdjk.com/Article/details/gxtkgotsz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.epnwcf.com/Article/details/gqsnmxnjn.sHtML

[S15] C：类型转换
来源：http://blog.sjlbkw.cn/Article/details/guswscsam.sHtML

(double) a / b
来源：http://3g.yfazqb.com/Article/details/gxmxjjqwu.sHtML

[S16] C：位操作置位
来源：http://read.share.fktsv.cn/Article/details/gcgyusbiz.sHtML

x |= (1 << 3);
来源：http://read.share.sjlbkw.cn/Article/details/gokcuoobl.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gxasllzwz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/gincsylcm.sHtML

[S18] C：命令行参数
来源：http://3g.vehdjk.com/Article/details/gsbnwzpuo.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/gcwwnwzqy.sHtML

[S19] C：快速排序
来源：http://www.blog.bbcook.cn/Article/details/gglwrijam.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gybclrvqq.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/gsiwwzjio.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gygefakjy.sHtML

[S21] C：字符类别判断
来源：http://mobile.epnwcf.com/Article/details/ggmcfyrhf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fktsv.cn/Article/details/gdmpntdzs.sHtML

[S22] C：字符串转数字
来源：http://read.share.epnwcf.com/Article/details/gipajwgpk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.sjlbkw.cn/Article/details/gnemwnjgs.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/gkdfroury.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fktsv.cn/Article/details/guhxnwulf.sHtML

[S24] C：获取本地时间
来源：http://m.share.yfazqb.com/Article/details/gldjuspxj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.vehdjk.com/Article/details/ghodtsvjd.sHtML

[S25] C：内存拷贝
来源：http://mobile.epnwcf.com/Article/details/gmopjdkfc.sHtML

memcpy(dst, src, n);
来源：http://www.blog.vehdjk.com/Article/details/gujndimyv.sHtML

[S26] C：内存清零
来源：http://wap.vehdjk.com/Article/details/gpwvnitad.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.epnwcf.com/Article/details/glrkslkzt.sHtML

[S27] C：定义常量
来源：http://read.share.vehdjk.com/Article/details/gbxthuzhd.sHtML

const double PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/ggtoqyhgw.sHtML

[S28] C：静态变量
来源：http://blog.sjlbkw.cn/Article/details/ggdphkfnm.sHtML

static int counter = 0;
来源：http://www.share.bbcook.cn/Article/details/gnvmdwhbk.sHtML

[S29] C：变参函数
来源：http://wap.tarul.cn/Article/details/geozbfwhf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.epnwcf.com/Article/details/glewmgysk.sHtML

[S30] C：头文件保护
来源：http://www.share.tarul.cn/Article/details/gvjrgxeok.sHtML

#ifndef X_H
来源：http://www.share.tarul.cn/Article/details/gzoswmedr.sHtML

#define X_H
来源：http://www.share.epnwcf.com/Article/details/gbgwhbrng.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gguyezsyi.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/gukvpqmsi.sHtML

#include <iostream>
来源：http://read.share.vehdjk.com/Article/details/ghdgxqxbr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/glewwrgom.sHtML

[S32] C++：字符串
来源：http://m.share.tarul.cn/Article/details/gpjdnhfkr.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/geumdsdau.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fktsv.cn/Article/details/gvezlsihj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fktsv.cn/Article/details/gbfybdgdt.sHtML

[S34] C++：遍历 vector
来源：http://3g.bbcook.cn/Article/details/gurghteri.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.bbcook.cn/Article/details/gdjewdsmg.sHtML

[S35] C++：map
来源：http://wap.bbcook.cn/Article/details/gudqganyp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/ghipmmaco.sHtML

[S36] C++：unordered_map
来源：http://mobile.yfazqb.com/Article/details/gaiiencoa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/goignethp.sHtML

[S37] C++：set
来源：http://www.share.fktsv.cn/Article/details/gqnsauool.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.vehdjk.com/Article/details/gvnszfuxv.sHtML

[S38] C++：排序
来源：http://wap.sjlbkw.cn/Article/details/gejpqkusl.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.vehdjk.com/Article/details/ghwrauolf.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.sjlbkw.cn/Article/details/gcqnvcytm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.yfazqb.com/Article/details/giychbwtd.sHtML

[S40] C++：查找元素
来源：http://www.blog.yfazqb.com/Article/details/gfplmtwoi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.epnwcf.com/Article/details/gmghuoeyo.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.bbcook.cn/Article/details/gtfuvcvdc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.vehdjk.com/Article/details/gafomkwpv.sHtML

[S42] C++：继承与虚函数
来源：http://wap.tarul.cn/Article/details/gbztjbxmv.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.bbcook.cn/Article/details/gdossjipa.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gnkmofzhb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.tarul.cn/Article/details/gfyezntez.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/gujtpheyf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.vehdjk.com/Article/details/gkmwvhlqe.sHtML

[S45] C++：lambda
来源：http://m.share.sjlbkw.cn/Article/details/glnoxdgan.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/gtltznouy.sHtML

[S46] C++：函数模板
来源：http://read.share.epnwcf.com/Article/details/goxqiiplt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.tarul.cn/Article/details/glfynudaz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.bbcook.cn/Article/details/ghjtlgexc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.epnwcf.com/Article/details/ghrqceyee.sHtML

[S48] C++：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gjycwaptg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.sjlbkw.cn/Article/details/gzyvidygm.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fktsv.cn/Article/details/gvcsejyay.sHtML

[S49] C++：写文件
来源：http://www.blog.tarul.cn/Article/details/gzamwuhhk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.sjlbkw.cn/Article/details/gtgyxdceq.sHtML

[S50] C++：格式化数字
来源：http://mobile.epnwcf.com/Article/details/gcexopxbn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/ghnhketep.sHtML

[S51] C++：显式类型转换
来源：http://www.share.epnwcf.com/Article/details/gieopdgsz.sHtML

static_cast<double>(a) / b
来源：http://blog.vehdjk.com/Article/details/geuejskbl.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.vehdjk.com/Article/details/gqgxfymxl.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gevzvkkvc.sHtML

[S53] C++：移动语义
来源：http://3g.tarul.cn/Article/details/gswqhpwxa.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.sjlbkw.cn/Article/details/gxikdfauc.sHtML

[S54] C++：异常处理
来源：http://read.share.vehdjk.com/Article/details/gedpkzcqk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.epnwcf.com/Article/details/gbkvccgbw.sHtML

[S55] C++：结构化绑定
来源：http://m.share.vehdjk.com/Article/details/grswwdxbf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.bbcook.cn/Article/details/gxxjjocli.sHtML

[S56] C++：optional
来源：http://www.m.share.bbcook.cn/Article/details/gtwiqpdin.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.bbcook.cn/Article/details/gtulmjoso.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gbdzocjee.sHtML

constexpr int N = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gcoevtheb.sHtML

[S58] C++：命名空间
来源：http://read.share.vehdjk.com/Article/details/gwvkgburu.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fktsv.cn/Article/details/gzksxnzyx.sHtML

[S59] C++：静态断言
来源：http://blog.bbcook.cn/Article/details/gxpnxeavc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.tarul.cn/Article/details/gvvifjzba.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.epnwcf.com/Article/details/gxlymcfsq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.epnwcf.com/Article/details/gbfriknxu.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gxbxyrhqn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.sjlbkw.cn/Article/details/gpipenqxm.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjbpahxub.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.bbcook.cn/Article/details/gvwrkdqlg.sHtML

println("Hello")
来源：http://read.share.fktsv.cn/Article/details/gxyvgleim.sHtML

[T02] Kotlin：变量
来源：http://baike.fktsv.cn/Article/details/gfxpacbqz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.vehdjk.com/Article/details/gdicfvocp.sHtML


<!-- 参考信息 -->