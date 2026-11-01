代发 wailian999

set -euo pipefail
来源：http://blog.vehdjk.com/Article/details/gutxoivhu.sHtML

[R02] 变量赋值与使用
来源：http://blog.tarul.cn/Article/details/gkaawnmxz.sHtML

name="Tom"; echo "$name"
来源：http://baike.yfazqb.com/Article/details/gfbyfnscn.sHtML

[R03] 只读变量
来源：http://m.share.bbcook.cn/Article/details/gakjcvgyl.sHtML

readonly PI=3.14
来源：http://blog.tarul.cn/Article/details/ghtzcyjrd.sHtML

[R04] 位置参数
来源：http://www.share.bbcook.cn/Article/details/gdynlnbbn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.vehdjk.com/Article/details/gaksuisoe.sHtML

[R05] 参数默认值
来源：http://wap.vehdjk.com/Article/details/gkaefllin.sHtML

name="${1:-default}"
来源：http://3g.bbcook.cn/Article/details/gfgveiwvz.sHtML

[R06] 判断命令是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gwgvkficr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/gzpgyxryj.sHtML

[R07] if 判断文件
来源：http://baike.yfazqb.com/Article/details/gaootwaah.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.tarul.cn/Article/details/gddzndpdu.sHtML

[R08] 数值比较
来源：http://www.m.share.epnwcf.com/Article/details/guvfhlwrp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gyhisilxo.sHtML

[R09] 字符串比较
来源：http://m.share.bbcook.cn/Article/details/gmdqdgetm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.epnwcf.com/Article/details/gmsbegqef.sHtML

[R10] 正则匹配
来源：http://blog.sjlbkw.cn/Article/details/gmyliwetg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.tarul.cn/Article/details/gjnsvdlcx.sHtML

[R11] case 多分支
来源：http://baike.tarul.cn/Article/details/gsgckacay.sHtML

case "$1" in
来源：http://www.blog.fktsv.cn/Article/details/giqrmesxk.sHtML

start) echo "启动" ;;
来源：http://mobile.bbcook.cn/Article/details/gcywzaiia.sHtML

stop)  echo "停止" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gtqtlngeh.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.vehdjk.com/Article/details/gcecthcqs.sHtML

esac
来源：http://www.m.share.tarul.cn/Article/details/gwivdwzsg.sHtML

[R12] for 遍历文件
来源：http://read.share.vehdjk.com/Article/details/gvhhxasrv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.tarul.cn/Article/details/gnusmnqjq.sHtML

[R13] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/gphunuqgy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/ghzdrhvaz.sHtML

[R14] C 风格 for
来源：http://baike.sjlbkw.cn/Article/details/ghzkbyefq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/gvadecxia.sHtML

[R15] while 逐行读文件
来源：http://blog.bbcook.cn/Article/details/gpuczpcut.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fktsv.cn/Article/details/guygadhza.sHtML

[R16] until 等待条件
来源：http://baike.yfazqb.com/Article/details/gopabnlqf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/glipwridm.sHtML

[R17] 数组定义与取值
来源：http://www.blog.vehdjk.com/Article/details/gnozapepx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.tarul.cn/Article/details/gskokeiyj.sHtML

[R18] 遍历数组
来源：http://www.share.fktsv.cn/Article/details/giloxzpba.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/gevuldvpd.sHtML

[R19] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gdbtqfpjq.sHtML

echo "${#arr[@]}"
来源：http://wap.vehdjk.com/Article/details/gbdglaccu.sHtML

[R20] 关联数组（字典）
来源：http://read.share.sjlbkw.cn/Article/details/guupczvjp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.epnwcf.com/Article/details/gvmdabcbu.sHtML

[R21] 字符串长度
来源：http://m.share.yfazqb.com/Article/details/gqhwxokme.sHtML

echo "${#s}"
来源：http://m.share.fktsv.cn/Article/details/gabffmamu.sHtML

[R22] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gfeycamra.sHtML

echo "${s:0:5}"
来源：http://3g.vehdjk.com/Article/details/gbuwfqveh.sHtML

[R23] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gsgowzjza.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.yfazqb.com/Article/details/gthuxscru.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gfuimwebc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.epnwcf.com/Article/details/gvdvwzaus.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/gebphvozo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.bbcook.cn/Article/details/gqtdeqjdz.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/geucwvhno.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fktsv.cn/Article/details/gufrbjppu.sHtML

[R27] 算术展开
来源：http://3g.bbcook.cn/Article/details/gyftycwdb.sHtML

echo $((1 + 2 * 3))
来源：http://baike.vehdjk.com/Article/details/gsfpwbeoe.sHtML

[R28] 浮点运算
来源：http://wap.vehdjk.com/Article/details/gmybmbzow.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/gyxeuuewq.sHtML

[R29] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/gvzmwezyc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fktsv.cn/Article/details/gfwohtsrt.sHtML

[R30] 函数返回状态码
来源：http://www.blog.epnwcf.com/Article/details/gasacxwgx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fktsv.cn/Article/details/goiueldtj.sHtML

[R31] 局部变量
来源：http://3g.vehdjk.com/Article/details/gpwfetxzr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/gmmbqhjbp.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/gckmtjnkn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.sjlbkw.cn/Article/details/gnxkouhnt.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.epnwcf.com/Article/details/giytoenjw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.sjlbkw.cn/Article/details/grwaxoznn.sHtML

[R34] 退出时清理
来源：http://baike.epnwcf.com/Article/details/gjxjyddhu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gruelglht.sHtML

[R35] 后台执行并等待
来源：http://baike.fktsv.cn/Article/details/guxhzcnyf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fktsv.cn/Article/details/gtxuuirpw.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.yfazqb.com/Article/details/gqxndxooc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.bbcook.cn/Article/details/gsnudntvu.sHtML

[R37] 把输出赋给变量
来源：http://www.share.vehdjk.com/Article/details/ggqrmajvq.sHtML

files=$(ls -1)
来源：http://baike.fktsv.cn/Article/details/gptmpwome.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/gnpgizyfc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.yfazqb.com/Article/details/gjfpslpsx.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.bbcook.cn/Article/details/gbluhhahe.sHtML

cmd > out.log 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gllfjiopn.sHtML

[R40] 追加写日志
来源：http://read.share.tarul.cn/Article/details/gptbppxgc.sHtML

echo "log" >> out.log
来源：http://baike.tarul.cn/Article/details/gomvzqkns.sHtML

[R41] 丢弃输出
来源：http://mobile.bbcook.cn/Article/details/gdfnyqykg.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/ggxbllqfo.sHtML

[R42] 输入重定向
来源：http://m.share.yfazqb.com/Article/details/gfljvphkw.sHtML

wc -l < a.txt
来源：http://read.share.yfazqb.com/Article/details/gzppztnat.sHtML

[R43] 按名字查找文件
来源：http://www.share.vehdjk.com/Article/details/gudzjjiav.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.yfazqb.com/Article/details/gukzktruj.sHtML

[R44] 按修改时间查找
来源：http://read.share.tarul.cn/Article/details/gewxvebun.sHtML

find . -mtime -7 -type f
来源：http://wap.fktsv.cn/Article/details/gfojybifb.sHtML

[R45] 批量删除
来源：http://mobile.yfazqb.com/Article/details/girqaxlmm.sHtML

find . -name "*.tmp" -delete
来源：http://blog.bbcook.cn/Article/details/gbafauqal.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.epnwcf.com/Article/details/gcmpuwuwz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.tarul.cn/Article/details/ggfqbwvvf.sHtML

[R47] sed 单行替换
来源：http://m.share.tarul.cn/Article/details/gftculiod.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.tarul.cn/Article/details/gudedtfjb.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/gsopxyybo.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gaukgumxj.sHtML

[R49] awk 带条件
来源：http://mobile.epnwcf.com/Article/details/gmnfjleny.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.epnwcf.com/Article/details/gaxftjvts.sHtML

[R50] awk 求和
来源：http://www.share.bbcook.cn/Article/details/ghclwderj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/ghsdenrvg.sHtML

[R51] 排序去重取前几
来源：http://www.blog.epnwcf.com/Article/details/ggvnbmjaf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.bbcook.cn/Article/details/gsumejoum.sHtML

[R52] 统计行数
来源：http://www.blog.vehdjk.com/Article/details/gdmxipvie.sHtML

wc -l a.txt
来源：http://wap.epnwcf.com/Article/details/glvurznuw.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fktsv.cn/Article/details/ggcveoaev.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.sjlbkw.cn/Article/details/gjxodxure.sHtML

[R54] 比较两个文件
来源：http://baike.fktsv.cn/Article/details/gexoiaqvv.sHtML

diff a.txt b.txt
来源：http://wap.sjlbkw.cn/Article/details/gbagtssyu.sHtML

[R55] 压缩与解压
来源：http://baike.fktsv.cn/Article/details/gbmcrnywa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.bbcook.cn/Article/details/gqvsvtana.sHtML

[R56] 远程拷贝
来源：http://mobile.epnwcf.com/Article/details/gxvyhvtns.sHtML

scp file user@host:/path/
来源：http://read.share.tarul.cn/Article/details/gdckmxalj.sHtML

[R57] 远程执行命令
来源：http://baike.vehdjk.com/Article/details/ggwpcfapv.sHtML

ssh user@host 'uptime'
来源：http://www.blog.bbcook.cn/Article/details/gdwxgpowc.sHtML

[R58] 下载文件
来源：http://www.blog.bbcook.cn/Article/details/ggfdztpxp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.vehdjk.com/Article/details/gwfqnxzfr.sHtML

[R59] 发 POST JSON
来源：http://www.share.bbcook.cn/Article/details/gnfqtthqy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/ggvffjiqp.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gchobxubp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.epnwcf.com/Article/details/gfnjkgivs.sHtML

[R61] 磁盘占用
来源：http://baike.sjlbkw.cn/Article/details/gdkbcmhfh.sHtML

df -h;  du -sh *
来源：http://m.share.yfazqb.com/Article/details/gpxeksrhh.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fktsv.cn/Article/details/ghvtjiolj.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.yfazqb.com/Article/details/gagggzkkt.sHtML

[R63] 内存与进程
来源：http://www.m.share.fktsv.cn/Article/details/gwfqbhltf.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.vehdjk.com/Article/details/gamqqcwhm.sHtML

[R64] 结束进程
来源：http://baike.tarul.cn/Article/details/gvklrrelm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcoosgpbb.sHtML

[R65] 查看端口占用
来源：http://read.share.bbcook.cn/Article/details/gvuofljqq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.bbcook.cn/Article/details/guisjpbbj.sHtML

[R66] 定时任务
来源：http://3g.vehdjk.com/Article/details/giokbxgge.sHtML

crontab -e;  crontab -l
来源：http://read.share.tarul.cn/Article/details/gabrctfcb.sHtML

[R67] 生成随机十六进制串
来源：http://3g.yfazqb.com/Article/details/gunadnorn.sHtML

openssl rand -hex 16
来源：http://www.share.vehdjk.com/Article/details/ghwiehrvh.sHtML

[R68] 计算文件校验值
来源：http://www.share.epnwcf.com/Article/details/gzqzvyfdr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fktsv.cn/Article/details/gqfagohnb.sHtML

[R69] 生成随机密码
来源：http://www.blog.bbcook.cn/Article/details/gqetugmpj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.tarul.cn/Article/details/gynhrxqyd.sHtML

[R70] 时间戳与互转
来源：http://m.share.sjlbkw.cn/Article/details/gzehnigjp.sHtML

date +%s;  date -d @1700000000
来源：http://baike.yfazqb.com/Article/details/gdmvejdwt.sHtML

[R71] 日期格式化
来源：http://blog.bbcook.cn/Article/details/gqnztlybj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.bbcook.cn/Article/details/gmhqlxugh.sHtML

[R72] 等待端口就绪
来源：http://read.share.vehdjk.com/Article/details/gjhwmltic.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gyxbavofw.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/ggdcjetmd.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.bbcook.cn/Article/details/glmiirphd.sHtML

[R74] 批量重命名
来源：http://m.share.epnwcf.com/Article/details/givoyhhcd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.vehdjk.com/Article/details/guahusdqj.sHtML

[R75] 导出环境变量
来源：http://mobile.bbcook.cn/Article/details/gpuaiiwew.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.yfazqb.com/Article/details/gvxsdnirx.sHtML

[R76] 使用临时文件
来源：http://www.share.yfazqb.com/Article/details/gamzqtlim.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/gkhctazxf.sHtML

[R77] 读取用户输入
来源：http://wap.sjlbkw.cn/Article/details/grlcoqurf.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/gaynknuha.sHtML

[R78] 交互式菜单
来源：http://wap.yfazqb.com/Article/details/gnqijwahj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.sjlbkw.cn/Article/details/geqfpgwbk.sHtML

[R79] 解析命令行选项
来源：http://baike.tarul.cn/Article/details/gbiikbmxt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.sjlbkw.cn/Article/details/greadippq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.yfazqb.com/Article/details/gnolcsmdr.sHtML

time ./run.sh
来源：http://mobile.vehdjk.com/Article/details/gwireackm.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/goszuqzoh.sHtML

S. C / C++ 专题
来源：http://read.share.vehdjk.com/Article/details/ghzbtgvar.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/glxorizpb.sHtML

[S01] C：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gnhdoaqzq.sHtML

#include <stdio.h>
来源：http://m.share.fktsv.cn/Article/details/gbyrvuwal.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.yfazqb.com/Article/details/gwzuvrezo.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fktsv.cn/Article/details/grvkhycls.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.bbcook.cn/Article/details/gpkybbtha.sHtML

[S03] C：读入整数
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzoquctx.sHtML

int x; scanf("%d", &x);
来源：http://baike.yfazqb.com/Article/details/gvtsuztml.sHtML

[S04] C：字符串复制
来源：http://blog.vehdjk.com/Article/details/gddgusrrp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fktsv.cn/Article/details/gfrqqupus.sHtML

[S05] C：字符串长度
来源：http://mobile.bbcook.cn/Article/details/gfycbabjs.sHtML

strlen(s)
来源：http://wap.bbcook.cn/Article/details/gdidkkfjr.sHtML

[S06] C：字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gbihulmtv.sHtML

strcmp(a, b) == 0
来源：http://wap.vehdjk.com/Article/details/grtxpnjwc.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/gpmeijoeb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.epnwcf.com/Article/details/gefthebng.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.bbcook.cn/Article/details/giftnfnxy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.vehdjk.com/Article/details/gbalgyneb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.bbcook.cn/Article/details/gvzwcprnd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.bbcook.cn/Article/details/gabixhywe.sHtML

[S10] C：指针与解引用
来源：http://wap.vehdjk.com/Article/details/gdabwpoys.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.bbcook.cn/Article/details/gxmvpadmm.sHtML

[S11] C：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gscvhupza.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fktsv.cn/Article/details/gddxlilhh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gbzrodavr.sHtML

fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gpllckeqe.sHtML

[S12] C：写文件
来源：http://blog.epnwcf.com/Article/details/gszyibaku.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/glwykldmm.sHtML

[S13] C：宏定义
来源：http://3g.epnwcf.com/Article/details/gxopgvhzy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.bbcook.cn/Article/details/gpougdunq.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/gashjlzdr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.yfazqb.com/Article/details/gjiwaijsa.sHtML

[S15] C：类型转换
来源：http://www.m.share.epnwcf.com/Article/details/gjjbueuvw.sHtML

(double) a / b
来源：http://wap.tarul.cn/Article/details/gntupylgd.sHtML

[S16] C：位操作置位
来源：http://wap.vehdjk.com/Article/details/gjqlonnsy.sHtML

x |= (1 << 3);
来源：http://www.share.bbcook.cn/Article/details/gqcuigjnd.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/goxcszasz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.bbcook.cn/Article/details/gupeiselu.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/guzmhrylo.sHtML

int main(int argc, char **argv)
来源：http://m.share.fktsv.cn/Article/details/gttrgjgzr.sHtML

[S19] C：快速排序
来源：http://www.blog.sjlbkw.cn/Article/details/gkpaosneg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gcwjwtxos.sHtML

[S20] C：二分查找
来源：http://3g.sjlbkw.cn/Article/details/gqeyqvvrd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/gxxjypyva.sHtML

[S21] C：字符类别判断
来源：http://m.share.vehdjk.com/Article/details/ghtknwvfp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.yfazqb.com/Article/details/gehdkomws.sHtML

[S22] C：字符串转数字
来源：http://m.share.sjlbkw.cn/Article/details/gnyppweax.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fktsv.cn/Article/details/gmzpdwgjs.sHtML

[S23] C：随机数
来源：http://www.share.epnwcf.com/Article/details/gzchalhcm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fktsv.cn/Article/details/gnekqsfur.sHtML

[S24] C：获取本地时间
来源：http://mobile.fktsv.cn/Article/details/giuevbcjr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.bbcook.cn/Article/details/gxaofsmkp.sHtML

[S25] C：内存拷贝
来源：http://3g.epnwcf.com/Article/details/genezggsl.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/gylavlwuv.sHtML

[S26] C：内存清零
来源：http://m.share.fktsv.cn/Article/details/gmturcsiw.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fktsv.cn/Article/details/grcpgruxn.sHtML

[S27] C：定义常量
来源：http://blog.epnwcf.com/Article/details/grrxuahvx.sHtML

const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gutqfexoi.sHtML

[S28] C：静态变量
来源：http://www.blog.epnwcf.com/Article/details/ghcfdhyoh.sHtML

static int counter = 0;
来源：http://mobile.sjlbkw.cn/Article/details/gbzcyquaz.sHtML

[S29] C：变参函数
来源：http://3g.vehdjk.com/Article/details/gvwvgdboz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.vehdjk.com/Article/details/ghxkphfxb.sHtML

[S30] C：头文件保护
来源：http://www.blog.tarul.cn/Article/details/ggpjrggjv.sHtML

#ifndef X_H
来源：http://baike.epnwcf.com/Article/details/gkgxeupku.sHtML

#define X_H
来源：http://m.share.bbcook.cn/Article/details/gldmfbghx.sHtML

#endif
来源：http://baike.fktsv.cn/Article/details/giyrdrfnj.sHtML

[S31] C++：Hello World
来源：http://m.share.fktsv.cn/Article/details/gwoinixxr.sHtML

#include <iostream>
来源：http://3g.sjlbkw.cn/Article/details/gudxrnbej.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/gfpskviog.sHtML

[S32] C++：字符串
来源：http://mobile.yfazqb.com/Article/details/guyvwapgf.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fktsv.cn/Article/details/geloguqtz.sHtML

[S33] C++：vector 增删
来源：http://mobile.bbcook.cn/Article/details/gewywazxj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.bbcook.cn/Article/details/ggjtqckdv.sHtML

[S34] C++：遍历 vector
来源：http://read.share.tarul.cn/Article/details/gbxcxfqtb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.vehdjk.com/Article/details/gcwrraacr.sHtML

[S35] C++：map
来源：http://mobile.sjlbkw.cn/Article/details/gwrcdgbvb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gdbtpzrea.sHtML

[S36] C++：unordered_map
来源：http://baike.yfazqb.com/Article/details/gntwsnpmm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gncwtstso.sHtML

[S37] C++：set
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgylanlt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.vehdjk.com/Article/details/gfeaimezz.sHtML

[S38] C++：排序
来源：http://wap.bbcook.cn/Article/details/ghbcjhatv.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.yfazqb.com/Article/details/gcgbebuzx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.bbcook.cn/Article/details/gtdobxkeb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.bbcook.cn/Article/details/gkllrdzet.sHtML

[S40] C++：查找元素
来源：http://www.share.yfazqb.com/Article/details/gwzltaors.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.vehdjk.com/Article/details/ggsyowuox.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.epnwcf.com/Article/details/giookgggt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.vehdjk.com/Article/details/gzpximxlx.sHtML

[S42] C++：继承与虚函数
来源：http://blog.bbcook.cn/Article/details/gpenqqohm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fktsv.cn/Article/details/gmexhuqwm.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/gzmdzkpwf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.epnwcf.com/Article/details/gxeqfyflb.sHtML

[S44] C++：引用传参
来源：http://baike.tarul.cn/Article/details/gyzolntzj.sHtML

void inc(int &x) { ++x; }
来源：http://3g.sjlbkw.cn/Article/details/ggsfiibam.sHtML

[S45] C++：lambda
来源：http://blog.sjlbkw.cn/Article/details/gpdmgzyjq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.tarul.cn/Article/details/gttqhgdyh.sHtML

[S46] C++：函数模板
来源：http://mobile.fktsv.cn/Article/details/gedxqbtmr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.yfazqb.com/Article/details/gvcrkedes.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.epnwcf.com/Article/details/gnqfohoor.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fktsv.cn/Article/details/gylmypsiq.sHtML

[S48] C++：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gatglvcxl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.bbcook.cn/Article/details/gcqqvjxsz.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.tarul.cn/Article/details/gyucigyxr.sHtML

[S49] C++：写文件
来源：http://www.blog.yfazqb.com/Article/details/gqyptlxhq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.bbcook.cn/Article/details/gcukigavg.sHtML

[S50] C++：格式化数字
来源：http://3g.sjlbkw.cn/Article/details/gzpwddtwf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gtjozfjxl.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/gquazmptu.sHtML

static_cast<double>(a) / b
来源：http://baike.fktsv.cn/Article/details/gpgmvgath.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.sjlbkw.cn/Article/details/gnxuqrwnu.sHtML

int size() const noexcept { return n_; }
来源：http://3g.yfazqb.com/Article/details/gxwiffwxt.sHtML

[S53] C++：移动语义
来源：http://3g.epnwcf.com/Article/details/gjsqrrsfa.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fktsv.cn/Article/details/gfhoxojwn.sHtML

[S54] C++：异常处理
来源：http://mobile.yfazqb.com/Article/details/gzhikmtfx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/ghglgpfca.sHtML

[S55] C++：结构化绑定
来源：http://3g.vehdjk.com/Article/details/gysbziqoc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fktsv.cn/Article/details/gsxhgajwa.sHtML

[S56] C++：optional
来源：http://mobile.sjlbkw.cn/Article/details/gohdpwxua.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.yfazqb.com/Article/details/grvidlnlo.sHtML

[S57] C++：编译期常量
来源：http://baike.epnwcf.com/Article/details/gxyobblue.sHtML

constexpr int N = 10;
来源：http://read.share.bbcook.cn/Article/details/gzwiaubpz.sHtML

[S58] C++：命名空间
来源：http://www.share.epnwcf.com/Article/details/geinyagoy.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fktsv.cn/Article/details/gdkzbzpan.sHtML

[S59] C++：静态断言
来源：http://www.share.vehdjk.com/Article/details/gwjbyieny.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.sjlbkw.cn/Article/details/glwhmjdcg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gbhkcrcag.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.tarul.cn/Article/details/gkdabzsan.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gijnxnfhu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.tarul.cn/Article/details/gmpeojofh.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpqxtrqtt.sHtML

[T01] Kotlin：Hello World
来源：http://baike.epnwcf.com/Article/details/gdussrygm.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gyghoglvm.sHtML

[T02] Kotlin：变量
来源：http://mobile.sjlbkw.cn/Article/details/gvbeycjdt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.yfazqb.com/Article/details/gbbsprhwq.sHtML


<!-- 参考信息 -->