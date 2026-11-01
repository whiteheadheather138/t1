代发 wailian999

set -euo pipefail
来源：http://baike.tarul.cn/Article/details/grsdkmbcw.sHtML

[R02] 变量赋值与使用
来源：http://3g.vehdjk.com/Article/details/gwuonhcwc.sHtML

name="Tom"; echo "$name"
来源：http://m.share.tarul.cn/Article/details/goqirfffk.sHtML

[R03] 只读变量
来源：http://www.m.share.epnwcf.com/Article/details/gnkupspmg.sHtML

readonly PI=3.14
来源：http://3g.fktsv.cn/Article/details/glznivmko.sHtML

[R04] 位置参数
来源：http://wap.tarul.cn/Article/details/gqodzhdiy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/gvhlhldrr.sHtML

[R05] 参数默认值
来源：http://m.share.epnwcf.com/Article/details/gvijqurge.sHtML

name="${1:-default}"
来源：http://www.m.share.bbcook.cn/Article/details/guiztxzaw.sHtML

[R06] 判断命令是否存在
来源：http://3g.vehdjk.com/Article/details/gpmxiktqz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fktsv.cn/Article/details/gvehemesb.sHtML

[R07] if 判断文件
来源：http://www.m.share.yfazqb.com/Article/details/gvkblsmwd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gwszuhbuq.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/greprmjui.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.epnwcf.com/Article/details/gqgjanlmb.sHtML

[R09] 字符串比较
来源：http://mobile.tarul.cn/Article/details/gozmjnbof.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.epnwcf.com/Article/details/gthjnwgbx.sHtML

[R10] 正则匹配
来源：http://www.blog.vehdjk.com/Article/details/gzsohbmrg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fktsv.cn/Article/details/gpwnjocbw.sHtML

[R11] case 多分支
来源：http://baike.sjlbkw.cn/Article/details/ggirwazty.sHtML

case "$1" in
来源：http://www.share.bbcook.cn/Article/details/ghnaoqvgd.sHtML

start) echo "启动" ;;
来源：http://baike.fktsv.cn/Article/details/gjccovxtn.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.epnwcf.com/Article/details/guqlrcpol.sHtML

*)     echo "未知命令" ;;
来源：http://3g.tarul.cn/Article/details/gxioxzrnr.sHtML

esac
来源：http://www.share.sjlbkw.cn/Article/details/glbofvwto.sHtML

[R12] for 遍历文件
来源：http://www.share.yfazqb.com/Article/details/gczbzfvlg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.sjlbkw.cn/Article/details/gebuqzupc.sHtML

[R13] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gimzhwteu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/goliqirez.sHtML

[R14] C 风格 for
来源：http://wap.vehdjk.com/Article/details/gojwfbvbk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/gmbxzcvbs.sHtML

[R15] while 逐行读文件
来源：http://blog.epnwcf.com/Article/details/gfuwttjiy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.bbcook.cn/Article/details/gzbbjlucr.sHtML

[R16] until 等待条件
来源：http://blog.epnwcf.com/Article/details/gobmlucsy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/gpsazygag.sHtML

[R17] 数组定义与取值
来源：http://www.blog.bbcook.cn/Article/details/gcsiyzbcg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.vehdjk.com/Article/details/gnbexuure.sHtML

[R18] 遍历数组
来源：http://m.share.yfazqb.com/Article/details/gndtwtdxf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fktsv.cn/Article/details/ghjviwfgp.sHtML

[R19] 数组长度
来源：http://3g.yfazqb.com/Article/details/gkpwelubz.sHtML

echo "${#arr[@]}"
来源：http://wap.epnwcf.com/Article/details/gnsmdxoau.sHtML

[R20] 关联数组（字典）
来源：http://blog.tarul.cn/Article/details/gisnztlta.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.tarul.cn/Article/details/gkwupguie.sHtML

[R21] 字符串长度
来源：http://blog.vehdjk.com/Article/details/gtkivtidf.sHtML

echo "${#s}"
来源：http://www.share.vehdjk.com/Article/details/gcxehvxbz.sHtML

[R22] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gqkhbdvdt.sHtML

echo "${s:0:5}"
来源：http://mobile.sjlbkw.cn/Article/details/gxnxjiqsn.sHtML

[R23] 字符串替换
来源：http://blog.tarul.cn/Article/details/gqnvsycfj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.yfazqb.com/Article/details/gmzvpcjjf.sHtML

[R24] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gfunumpws.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.vehdjk.com/Article/details/gwhyyaoju.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.vehdjk.com/Article/details/gknojiofj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fktsv.cn/Article/details/ghbesupjm.sHtML

[R26] 命令替换
来源：http://read.share.bbcook.cn/Article/details/guopyjciy.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.vehdjk.com/Article/details/gruittewe.sHtML

[R27] 算术展开
来源：http://3g.tarul.cn/Article/details/giuzwbxuq.sHtML

echo $((1 + 2 * 3))
来源：http://baike.bbcook.cn/Article/details/gisgzduog.sHtML

[R28] 浮点运算
来源：http://www.blog.yfazqb.com/Article/details/ghdbbqebs.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.sjlbkw.cn/Article/details/gxyzthjfn.sHtML

[R29] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gralihkvl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.vehdjk.com/Article/details/gbdxzsqsu.sHtML

[R30] 函数返回状态码
来源：http://m.share.vehdjk.com/Article/details/ggjfjpgrn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/gmnzdsdsl.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/gofazmxxr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.yfazqb.com/Article/details/gtmvobymp.sHtML

[R32] 参数个数校验
来源：http://baike.yfazqb.com/Article/details/gibpyebzf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/gmmxiiamo.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fktsv.cn/Article/details/glbuyckpd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.tarul.cn/Article/details/gdtiguzdn.sHtML

[R34] 退出时清理
来源：http://www.share.vehdjk.com/Article/details/godfzcbes.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.bbcook.cn/Article/details/gknducmfx.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/gsdihplgb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.tarul.cn/Article/details/ghrojuzbz.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/gajiqtgjr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.sjlbkw.cn/Article/details/ghkiyutjh.sHtML

[R37] 把输出赋给变量
来源：http://www.share.tarul.cn/Article/details/goedhzufl.sHtML

files=$(ls -1)
来源：http://baike.tarul.cn/Article/details/gkbaxoefb.sHtML

[R38] 管道串联
来源：http://mobile.sjlbkw.cn/Article/details/gojrsfqsb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fktsv.cn/Article/details/gozkduvhw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.tarul.cn/Article/details/gtdpauwxc.sHtML

cmd > out.log 2>&1
来源：http://3g.tarul.cn/Article/details/gvkowrxgs.sHtML

[R40] 追加写日志
来源：http://wap.sjlbkw.cn/Article/details/ghzbqkgtj.sHtML

echo "log" >> out.log
来源：http://blog.sjlbkw.cn/Article/details/gvtqpvfbz.sHtML

[R41] 丢弃输出
来源：http://3g.bbcook.cn/Article/details/gkfztkprd.sHtML

cmd >/dev/null 2>&1
来源：http://3g.epnwcf.com/Article/details/glgumllam.sHtML

[R42] 输入重定向
来源：http://www.share.epnwcf.com/Article/details/ghjixzbvs.sHtML

wc -l < a.txt
来源：http://www.share.fktsv.cn/Article/details/gyvzozgzu.sHtML

[R43] 按名字查找文件
来源：http://mobile.fktsv.cn/Article/details/gjlpfjezp.sHtML

find . -name "*.log" -type f
来源：http://blog.tarul.cn/Article/details/gmlaichnu.sHtML

[R44] 按修改时间查找
来源：http://blog.tarul.cn/Article/details/gdotahsxy.sHtML

find . -mtime -7 -type f
来源：http://www.share.yfazqb.com/Article/details/geyxcppyk.sHtML

[R45] 批量删除
来源：http://m.share.tarul.cn/Article/details/ggwipvghu.sHtML

find . -name "*.tmp" -delete
来源：http://wap.vehdjk.com/Article/details/gmciitqhg.sHtML

[R46] 递归替换文件内容
来源：http://mobile.sjlbkw.cn/Article/details/gxtkgtida.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.tarul.cn/Article/details/gqifpazjj.sHtML

[R47] sed 单行替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyizjgat.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.tarul.cn/Article/details/gdacwvgwh.sHtML

[R48] awk 取指定列
来源：http://www.blog.epnwcf.com/Article/details/guhgpkmcm.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gzakawlee.sHtML

[R49] awk 带条件
来源：http://3g.sjlbkw.cn/Article/details/gyxwmfdcu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.tarul.cn/Article/details/gvhchtnvr.sHtML

[R50] awk 求和
来源：http://read.share.yfazqb.com/Article/details/gakcptgmf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gjpdijyer.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fktsv.cn/Article/details/gkydtqasj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.yfazqb.com/Article/details/geddjzcjy.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/grahslokq.sHtML

wc -l a.txt
来源：http://3g.yfazqb.com/Article/details/gqqzitcvv.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.epnwcf.com/Article/details/ginvgxdtu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.vehdjk.com/Article/details/gomcpyhae.sHtML

[R54] 比较两个文件
来源：http://www.share.tarul.cn/Article/details/gbtfqiisa.sHtML

diff a.txt b.txt
来源：http://www.m.share.vehdjk.com/Article/details/ggwvmjmus.sHtML

[R55] 压缩与解压
来源：http://wap.bbcook.cn/Article/details/gssuobmme.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fktsv.cn/Article/details/gjoetpvua.sHtML

[R56] 远程拷贝
来源：http://baike.vehdjk.com/Article/details/giufsfxgd.sHtML

scp file user@host:/path/
来源：http://www.m.share.tarul.cn/Article/details/gbfnilbue.sHtML

[R57] 远程执行命令
来源：http://m.share.fktsv.cn/Article/details/gazhadiyk.sHtML

ssh user@host 'uptime'
来源：http://3g.bbcook.cn/Article/details/gqurcyilo.sHtML

[R58] 下载文件
来源：http://read.share.yfazqb.com/Article/details/gsyqxnrbi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/gejgjpiie.sHtML

[R59] 发 POST JSON
来源：http://www.share.tarul.cn/Article/details/gqshyqgyq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.yfazqb.com/Article/details/gwqkmgzip.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gnrwxtgwy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.tarul.cn/Article/details/gtnsltanr.sHtML

[R61] 磁盘占用
来源：http://www.m.share.epnwcf.com/Article/details/gnekilnkg.sHtML

df -h;  du -sh *
来源：http://www.share.vehdjk.com/Article/details/gmavyhwto.sHtML

[R62] 找最占空间的文件
来源：http://www.share.tarul.cn/Article/details/gflnawcti.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.bbcook.cn/Article/details/gwdotxour.sHtML

[R63] 内存与进程
来源：http://www.blog.bbcook.cn/Article/details/gvhyeprri.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.yfazqb.com/Article/details/gwrxnhoxr.sHtML

[R64] 结束进程
来源：http://mobile.yfazqb.com/Article/details/gtgyfuifw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.sjlbkw.cn/Article/details/gruykbasl.sHtML

[R65] 查看端口占用
来源：http://blog.sjlbkw.cn/Article/details/gylbrmthq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fktsv.cn/Article/details/gchgkwanx.sHtML

[R66] 定时任务
来源：http://read.share.vehdjk.com/Article/details/gipdnlzpa.sHtML

crontab -e;  crontab -l
来源：http://blog.epnwcf.com/Article/details/gawxnbqdg.sHtML

[R67] 生成随机十六进制串
来源：http://wap.epnwcf.com/Article/details/gfmvbudvv.sHtML

openssl rand -hex 16
来源：http://mobile.vehdjk.com/Article/details/giyggfhoa.sHtML

[R68] 计算文件校验值
来源：http://www.share.epnwcf.com/Article/details/gtmzytvud.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.tarul.cn/Article/details/gsewfravd.sHtML

[R69] 生成随机密码
来源：http://m.share.yfazqb.com/Article/details/gzvldgter.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.epnwcf.com/Article/details/gqtpomkuj.sHtML

[R70] 时间戳与互转
来源：http://blog.fktsv.cn/Article/details/gqffhgklx.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.sjlbkw.cn/Article/details/goywjllbz.sHtML

[R71] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gzowkgoch.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.epnwcf.com/Article/details/glblfsiyf.sHtML

[R72] 等待端口就绪
来源：http://m.share.fktsv.cn/Article/details/gzzcueglr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gbgodeghd.sHtML

[R73] 分割大日志
来源：http://blog.fktsv.cn/Article/details/gsmhkdvvl.sHtML

split -l 1000 big.log part_
来源：http://mobile.bbcook.cn/Article/details/gtoxdojfj.sHtML

[R74] 批量重命名
来源：http://www.share.epnwcf.com/Article/details/gagsgdlgs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fktsv.cn/Article/details/grdkpiqvy.sHtML

[R75] 导出环境变量
来源：http://wap.sjlbkw.cn/Article/details/gcfbihcqm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.tarul.cn/Article/details/gcwjsqreb.sHtML

[R76] 使用临时文件
来源：http://mobile.epnwcf.com/Article/details/gcgzvrifv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/grueflwic.sHtML

[R77] 读取用户输入
来源：http://3g.vehdjk.com/Article/details/godvidgdo.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/gueencosc.sHtML

[R78] 交互式菜单
来源：http://baike.fktsv.cn/Article/details/gpuwucqzz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.epnwcf.com/Article/details/gqigcvycj.sHtML

[R79] 解析命令行选项
来源：http://3g.yfazqb.com/Article/details/gflctlffs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.tarul.cn/Article/details/gykppsjgs.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.epnwcf.com/Article/details/gzqnuucfc.sHtML

time ./run.sh
来源：http://www.m.share.tarul.cn/Article/details/gqdytylzx.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gbvtslcjm.sHtML

S. C / C++ 专题
来源：http://mobile.fktsv.cn/Article/details/gryhvgvsm.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gvsiuiwdb.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/gbebvpizl.sHtML

#include <stdio.h>
来源：http://m.share.sjlbkw.cn/Article/details/ghskfrgqg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/grzjxmlyk.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.tarul.cn/Article/details/gsauwhnjz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fktsv.cn/Article/details/ggzfhrptw.sHtML

[S03] C：读入整数
来源：http://read.share.yfazqb.com/Article/details/gkgpjhkma.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gdxdizaph.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/gwxazsyfu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.tarul.cn/Article/details/gkwvktxeb.sHtML

[S05] C：字符串长度
来源：http://baike.bbcook.cn/Article/details/galmyxuzx.sHtML

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/gxzwtozhp.sHtML

[S06] C：字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbhozlab.sHtML

strcmp(a, b) == 0
来源：http://3g.epnwcf.com/Article/details/gpgqntixv.sHtML

[S07] C：数组遍历求和
来源：http://www.share.sjlbkw.cn/Article/details/gqsrrsbix.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.bbcook.cn/Article/details/gzaqmossr.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.epnwcf.com/Article/details/gjpkhkwnc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.yfazqb.com/Article/details/gxakosroo.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.tarul.cn/Article/details/gbslewpme.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.tarul.cn/Article/details/gvdjdwvzw.sHtML

[S10] C：指针与解引用
来源：http://m.share.fktsv.cn/Article/details/gwbomlhux.sHtML

int *p = &a;  *p = 5;
来源：http://wap.yfazqb.com/Article/details/gcyvtzaii.sHtML

[S11] C：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/giiyrgmvh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fktsv.cn/Article/details/geiahktbq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.vehdjk.com/Article/details/ggvqheriv.sHtML

fclose(f);
来源：http://www.share.tarul.cn/Article/details/gqybiocvc.sHtML

[S12] C：写文件
来源：http://mobile.vehdjk.com/Article/details/genmvvupc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.yfazqb.com/Article/details/golaazxgh.sHtML

[S13] C：宏定义
来源：http://wap.tarul.cn/Article/details/gpsgbzzvp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.epnwcf.com/Article/details/gwttceeqn.sHtML

[S14] C：枚举
来源：http://mobile.bbcook.cn/Article/details/gtqybxjxj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.sjlbkw.cn/Article/details/gedhuzbqu.sHtML

[S15] C：类型转换
来源：http://baike.epnwcf.com/Article/details/gkbbzeapr.sHtML

(double) a / b
来源：http://read.share.fktsv.cn/Article/details/gjuburhxd.sHtML

[S16] C：位操作置位
来源：http://baike.epnwcf.com/Article/details/gkogmfowq.sHtML

x |= (1 << 3);
来源：http://www.share.sjlbkw.cn/Article/details/gnyshvarn.sHtML

[S17] C：安全拼接字符串
来源：http://blog.epnwcf.com/Article/details/gerhsymls.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.vehdjk.com/Article/details/gomwajqay.sHtML

[S18] C：命令行参数
来源：http://baike.vehdjk.com/Article/details/guvhjhshi.sHtML

int main(int argc, char **argv)
来源：http://blog.sjlbkw.cn/Article/details/ghcvfirqv.sHtML

[S19] C：快速排序
来源：http://www.blog.yfazqb.com/Article/details/ggdgajqal.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gnivmhcwv.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/ggygejfvb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gjkxklutz.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.vehdjk.com/Article/details/gnglsutos.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.bbcook.cn/Article/details/guixqtkuq.sHtML

[S22] C：字符串转数字
来源：http://mobile.yfazqb.com/Article/details/gujgqmzwh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/giihlzouh.sHtML

[S23] C：随机数
来源：http://www.share.sjlbkw.cn/Article/details/gyxnlppyr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.bbcook.cn/Article/details/gnuoxmxna.sHtML

[S24] C：获取本地时间
来源：http://www.share.fktsv.cn/Article/details/gltkviciq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.vehdjk.com/Article/details/gvaewwlkw.sHtML

[S25] C：内存拷贝
来源：http://m.share.fktsv.cn/Article/details/gqmooqtaj.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/gfrounycg.sHtML

[S26] C：内存清零
来源：http://baike.epnwcf.com/Article/details/geltpbeps.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/groskbiho.sHtML

[S27] C：定义常量
来源：http://read.share.bbcook.cn/Article/details/gzgdzxnpv.sHtML

const double PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gmcpthdju.sHtML

[S28] C：静态变量
来源：http://blog.yfazqb.com/Article/details/gqdxptxlj.sHtML

static int counter = 0;
来源：http://baike.yfazqb.com/Article/details/gdocquivm.sHtML

[S29] C：变参函数
来源：http://m.share.fktsv.cn/Article/details/gxpxegjxg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.bbcook.cn/Article/details/gvjskhbrk.sHtML

[S30] C：头文件保护
来源：http://m.share.fktsv.cn/Article/details/goxejtvkb.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/gnmnewkjb.sHtML

#define X_H
来源：http://www.blog.tarul.cn/Article/details/gqcjrlbaq.sHtML

#endif
来源：http://3g.bbcook.cn/Article/details/gccxoebcc.sHtML

[S31] C++：Hello World
来源：http://baike.epnwcf.com/Article/details/gyyaeqxne.sHtML

#include <iostream>
来源：http://read.share.fktsv.cn/Article/details/gcqxhutbu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/gowaqnttb.sHtML

[S32] C++：字符串
来源：http://baike.yfazqb.com/Article/details/gjfeiddzc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.vehdjk.com/Article/details/gklzpzzfw.sHtML

[S33] C++：vector 增删
来源：http://read.share.epnwcf.com/Article/details/gzfjrelaj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.epnwcf.com/Article/details/gnqcurmuj.sHtML

[S34] C++：遍历 vector
来源：http://wap.fktsv.cn/Article/details/gsntsyyog.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.yfazqb.com/Article/details/gwkqakvxi.sHtML

[S35] C++：map
来源：http://m.share.sjlbkw.cn/Article/details/guoqhkbji.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gqyfburec.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gzasozpzi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gdjfjcsmf.sHtML

[S37] C++：set
来源：http://mobile.yfazqb.com/Article/details/giguhmmlq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.epnwcf.com/Article/details/gposjvuvw.sHtML

[S38] C++：排序
来源：http://blog.sjlbkw.cn/Article/details/gwpyegslz.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.bbcook.cn/Article/details/gyrhjtrpo.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.epnwcf.com/Article/details/gtotoxfjn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.bbcook.cn/Article/details/gbfikssux.sHtML

[S40] C++：查找元素
来源：http://wap.fktsv.cn/Article/details/gqpovebgj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.epnwcf.com/Article/details/ghqiejsdw.sHtML

[S41] C++：类与构造函数
来源：http://m.share.vehdjk.com/Article/details/gpjvbybhc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.vehdjk.com/Article/details/gigrrjqux.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.epnwcf.com/Article/details/gcvmnbsjx.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.sjlbkw.cn/Article/details/gfdvstikv.sHtML

[S43] C++：智能指针
来源：http://mobile.bbcook.cn/Article/details/grsigwzqi.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.sjlbkw.cn/Article/details/grulpqxgf.sHtML

[S44] C++：引用传参
来源：http://blog.sjlbkw.cn/Article/details/gspzhawmc.sHtML

void inc(int &x) { ++x; }
来源：http://3g.yfazqb.com/Article/details/gocwcnvch.sHtML

[S45] C++：lambda
来源：http://www.blog.yfazqb.com/Article/details/ggvdgelfa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.epnwcf.com/Article/details/gvecuncdu.sHtML

[S46] C++：函数模板
来源：http://www.m.share.epnwcf.com/Article/details/geclbpydu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fktsv.cn/Article/details/gtbufrjzr.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.sjlbkw.cn/Article/details/gvsmirfwc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.bbcook.cn/Article/details/gjkwvjudz.sHtML

[S48] C++：逐行读文件
来源：http://wap.tarul.cn/Article/details/gcikmqpkz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fktsv.cn/Article/details/gnazwbcne.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fktsv.cn/Article/details/gtppkppnd.sHtML

[S49] C++：写文件
来源：http://wap.bbcook.cn/Article/details/gbqdzdhkn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.yfazqb.com/Article/details/gmkrjabpi.sHtML

[S50] C++：格式化数字
来源：http://read.share.sjlbkw.cn/Article/details/gatobceum.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gtwkqheqo.sHtML

[S51] C++：显式类型转换
来源：http://m.share.vehdjk.com/Article/details/gfhpxrhwe.sHtML

static_cast<double>(a) / b
来源：http://www.share.bbcook.cn/Article/details/gennzsrxm.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.sjlbkw.cn/Article/details/genwjoacb.sHtML

int size() const noexcept { return n_; }
来源：http://blog.yfazqb.com/Article/details/gsbqpxxtp.sHtML

[S53] C++：移动语义
来源：http://mobile.vehdjk.com/Article/details/gyjlcugwb.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.epnwcf.com/Article/details/gfxruwqcy.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fktsv.cn/Article/details/grssxsotu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fktsv.cn/Article/details/gvfwsphil.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.vehdjk.com/Article/details/gxrroebiz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.tarul.cn/Article/details/gnoedhjuq.sHtML

[S56] C++：optional
来源：http://baike.epnwcf.com/Article/details/gsqjrqfsd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.sjlbkw.cn/Article/details/gzihstxdn.sHtML

[S57] C++：编译期常量
来源：http://3g.sjlbkw.cn/Article/details/givqctjuh.sHtML

constexpr int N = 10;
来源：http://3g.bbcook.cn/Article/details/gmpeqbtuc.sHtML

[S58] C++：命名空间
来源：http://read.share.vehdjk.com/Article/details/gioujczku.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.tarul.cn/Article/details/geskjypve.sHtML

[S59] C++：静态断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwcnwoyw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.sjlbkw.cn/Article/details/gjnklgbxy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.bbcook.cn/Article/details/gjveykecd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.yfazqb.com/Article/details/gywmvlaau.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpocygbfd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.bbcook.cn/Article/details/gdsfrghcf.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/geacoojef.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/gcebslngw.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gikeblojy.sHtML

[T02] Kotlin：变量
来源：http://www.blog.vehdjk.com/Article/details/glcgdeuqx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.sjlbkw.cn/Article/details/gkghifsho.sHtML


<!-- 参考信息 -->