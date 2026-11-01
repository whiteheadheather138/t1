代发 wailian999

readonly PI=3.14
来源：http://www.m.share.tarul.cn/Article/details/gxqirowtj.sHtML

[R04] 位置参数
来源：http://baike.fktsv.cn/Article/details/gtmtufapu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fktsv.cn/Article/details/gnahpyqaz.sHtML

[R05] 参数默认值
来源：http://www.share.yfazqb.com/Article/details/gjyqfsncx.sHtML

name="${1:-default}"
来源：http://3g.vehdjk.com/Article/details/gcmybpumt.sHtML

[R06] 判断命令是否存在
来源：http://blog.yfazqb.com/Article/details/gnrlxftmj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gkzrlslpc.sHtML

[R07] if 判断文件
来源：http://www.m.share.vehdjk.com/Article/details/gjwvqybmz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.epnwcf.com/Article/details/gzmgfmbzz.sHtML

[R08] 数值比较
来源：http://read.share.epnwcf.com/Article/details/gxaucocsg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.sjlbkw.cn/Article/details/gmsgvhjqv.sHtML

[R09] 字符串比较
来源：http://blog.tarul.cn/Article/details/gyggcfvrx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.bbcook.cn/Article/details/gggsmxnjf.sHtML

[R10] 正则匹配
来源：http://www.blog.yfazqb.com/Article/details/gskbnustb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.sjlbkw.cn/Article/details/gmhwohdht.sHtML

[R11] case 多分支
来源：http://read.share.fktsv.cn/Article/details/gwbohsowx.sHtML

case "$1" in
来源：http://3g.tarul.cn/Article/details/guemgfjxq.sHtML

start) echo "启动" ;;
来源：http://wap.vehdjk.com/Article/details/gmdmqnkxk.sHtML

stop)  echo "停止" ;;
来源：http://wap.epnwcf.com/Article/details/gxmpretbg.sHtML

*)     echo "未知命令" ;;
来源：http://baike.bbcook.cn/Article/details/gjmmlkrfi.sHtML

esac
来源：http://www.share.sjlbkw.cn/Article/details/gcwavnuob.sHtML

[R12] for 遍历文件
来源：http://wap.vehdjk.com/Article/details/gacaynodp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fktsv.cn/Article/details/gijgumaaf.sHtML

[R13] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gxgjyleml.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/gpkebfqru.sHtML

[R14] C 风格 for
来源：http://3g.fktsv.cn/Article/details/gqmwbghpv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gpvtaybxd.sHtML

[R15] while 逐行读文件
来源：http://m.share.fktsv.cn/Article/details/ghyrrpsuc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fktsv.cn/Article/details/gulpnkpwr.sHtML

[R16] until 等待条件
来源：http://baike.yfazqb.com/Article/details/gawnhhsdf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gpypourzd.sHtML

[R17] 数组定义与取值
来源：http://3g.epnwcf.com/Article/details/gaogcwyea.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.bbcook.cn/Article/details/gqyqoadip.sHtML

[R18] 遍历数组
来源：http://3g.epnwcf.com/Article/details/gonexjafv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.bbcook.cn/Article/details/gjxqkcjfn.sHtML

[R19] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/gbvdyqxdm.sHtML

echo "${#arr[@]}"
来源：http://read.share.yfazqb.com/Article/details/gpjubaoyy.sHtML

[R20] 关联数组（字典）
来源：http://mobile.tarul.cn/Article/details/gcylachxq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.yfazqb.com/Article/details/gqrnoewyd.sHtML

[R21] 字符串长度
来源：http://read.share.yfazqb.com/Article/details/graojnmoa.sHtML

echo "${#s}"
来源：http://baike.sjlbkw.cn/Article/details/godlimyou.sHtML

[R22] 截取子串
来源：http://blog.tarul.cn/Article/details/gpwkijoxr.sHtML

echo "${s:0:5}"
来源：http://m.share.vehdjk.com/Article/details/gzvxknhjr.sHtML

[R23] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gbndcddvx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.tarul.cn/Article/details/gtaldlxhl.sHtML

[R24] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gvplwndjo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.epnwcf.com/Article/details/ginmqqgnx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.bbcook.cn/Article/details/gcvtrqiep.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.sjlbkw.cn/Article/details/gxdwyluyn.sHtML

[R26] 命令替换
来源：http://baike.sjlbkw.cn/Article/details/gyvwjjtrc.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.yfazqb.com/Article/details/gujjreptk.sHtML

[R27] 算术展开
来源：http://mobile.fktsv.cn/Article/details/gpwcouopm.sHtML

echo $((1 + 2 * 3))
来源：http://wap.tarul.cn/Article/details/ghvegidkm.sHtML

[R28] 浮点运算
来源：http://wap.epnwcf.com/Article/details/grtsurhdi.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.sjlbkw.cn/Article/details/gdlcyuxni.sHtML

[R29] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/gcucvunfp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.yfazqb.com/Article/details/gvbucdrak.sHtML

[R30] 函数返回状态码
来源：http://read.share.tarul.cn/Article/details/ghhvggjiy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.yfazqb.com/Article/details/gnahmxufm.sHtML

[R31] 局部变量
来源：http://baike.fktsv.cn/Article/details/gwgaxmjuh.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.vehdjk.com/Article/details/gbxonmukm.sHtML

[R32] 参数个数校验
来源：http://wap.epnwcf.com/Article/details/grvjlgxxm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.yfazqb.com/Article/details/gyzjmmrhq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.epnwcf.com/Article/details/gunutprtg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.yfazqb.com/Article/details/gzmfxteok.sHtML

[R34] 退出时清理
来源：http://baike.sjlbkw.cn/Article/details/gyxdfpdxb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gxunxgpht.sHtML

[R35] 后台执行并等待
来源：http://www.share.vehdjk.com/Article/details/geunkeodz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.sjlbkw.cn/Article/details/gtnwnfdfh.sHtML

[R36] 并发执行多个任务
来源：http://m.share.tarul.cn/Article/details/gtvipucmt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.bbcook.cn/Article/details/gcigwjpmn.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.tarul.cn/Article/details/giamdkyop.sHtML

files=$(ls -1)
来源：http://mobile.yfazqb.com/Article/details/gnvdiywby.sHtML

[R38] 管道串联
来源：http://blog.sjlbkw.cn/Article/details/gdwgpxuqx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.tarul.cn/Article/details/gnjgwtoxs.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/guvvqijqn.sHtML

cmd > out.log 2>&1
来源：http://www.share.sjlbkw.cn/Article/details/gtitawtzf.sHtML

[R40] 追加写日志
来源：http://www.m.share.tarul.cn/Article/details/gfbkkrotr.sHtML

echo "log" >> out.log
来源：http://wap.vehdjk.com/Article/details/ghwiiyovr.sHtML

[R41] 丢弃输出
来源：http://www.blog.bbcook.cn/Article/details/gslfspatt.sHtML

cmd >/dev/null 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gcheslbcu.sHtML

[R42] 输入重定向
来源：http://blog.sjlbkw.cn/Article/details/gitltizek.sHtML

wc -l < a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gvbzpsrlz.sHtML

[R43] 按名字查找文件
来源：http://read.share.vehdjk.com/Article/details/giiyekooh.sHtML

find . -name "*.log" -type f
来源：http://blog.bbcook.cn/Article/details/gjbwmswus.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gfnwljwuw.sHtML

find . -mtime -7 -type f
来源：http://mobile.bbcook.cn/Article/details/gdbrmasdv.sHtML

[R45] 批量删除
来源：http://mobile.vehdjk.com/Article/details/gukbuvcqj.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.bbcook.cn/Article/details/gdqjrqiow.sHtML

[R46] 递归替换文件内容
来源：http://baike.vehdjk.com/Article/details/gpathipwh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.vehdjk.com/Article/details/gddwtrpen.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/gvbxqdeto.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/gtdyqmtzu.sHtML

[R48] awk 取指定列
来源：http://blog.bbcook.cn/Article/details/gnefmltet.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.epnwcf.com/Article/details/gqapgnjhf.sHtML

[R49] awk 带条件
来源：http://www.blog.vehdjk.com/Article/details/gikjpderd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fktsv.cn/Article/details/ggjmcwbtp.sHtML

[R50] awk 求和
来源：http://mobile.vehdjk.com/Article/details/ghrcbsphk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/ghxycjzhj.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.vehdjk.com/Article/details/gzqesfibo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fktsv.cn/Article/details/gkbpvtgly.sHtML

[R52] 统计行数
来源：http://blog.epnwcf.com/Article/details/gmkoanmdz.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/gueryzcnw.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.tarul.cn/Article/details/gcyexnopw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.tarul.cn/Article/details/gouuugsen.sHtML

[R54] 比较两个文件
来源：http://mobile.epnwcf.com/Article/details/gwfcvxrlb.sHtML

diff a.txt b.txt
来源：http://blog.sjlbkw.cn/Article/details/gjaqfycmr.sHtML

[R55] 压缩与解压
来源：http://read.share.yfazqb.com/Article/details/gcnnclcia.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.yfazqb.com/Article/details/gvdkwbmpw.sHtML

[R56] 远程拷贝
来源：http://www.blog.bbcook.cn/Article/details/gqhmrzhrb.sHtML

scp file user@host:/path/
来源：http://3g.yfazqb.com/Article/details/gjzyawxft.sHtML

[R57] 远程执行命令
来源：http://read.share.bbcook.cn/Article/details/gkbpjisvh.sHtML

ssh user@host 'uptime'
来源：http://www.share.vehdjk.com/Article/details/gykavugou.sHtML

[R58] 下载文件
来源：http://www.share.sjlbkw.cn/Article/details/ghdnhtguj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.epnwcf.com/Article/details/gutehkejn.sHtML

[R59] 发 POST JSON
来源：http://3g.bbcook.cn/Article/details/glulhtafd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fktsv.cn/Article/details/grsoiiqpj.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/gjfgnhmjz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/gugmmjmhr.sHtML

[R61] 磁盘占用
来源：http://www.m.share.tarul.cn/Article/details/gifzsmfxr.sHtML

df -h;  du -sh *
来源：http://www.m.share.sjlbkw.cn/Article/details/grliinnww.sHtML

[R62] 找最占空间的文件
来源：http://blog.sjlbkw.cn/Article/details/ghkdmhfyk.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.epnwcf.com/Article/details/gborwxfne.sHtML

[R63] 内存与进程
来源：http://read.share.epnwcf.com/Article/details/ganeiiifw.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fktsv.cn/Article/details/ghvymleel.sHtML

[R64] 结束进程
来源：http://blog.epnwcf.com/Article/details/grpklyfdb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.epnwcf.com/Article/details/gfrbtubig.sHtML

[R65] 查看端口占用
来源：http://www.share.vehdjk.com/Article/details/gsewztdli.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.bbcook.cn/Article/details/gozqbftxu.sHtML

[R66] 定时任务
来源：http://3g.sjlbkw.cn/Article/details/gtmdghlvn.sHtML

crontab -e;  crontab -l
来源：http://read.share.fktsv.cn/Article/details/ghuzyrwyd.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.bbcook.cn/Article/details/gsnxbwbpd.sHtML

openssl rand -hex 16
来源：http://3g.epnwcf.com/Article/details/glkngvrou.sHtML

[R68] 计算文件校验值
来源：http://wap.bbcook.cn/Article/details/gnpokgtjv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gtbrvzcxf.sHtML

[R69] 生成随机密码
来源：http://blog.tarul.cn/Article/details/grwkpecta.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.epnwcf.com/Article/details/gyxqivvdx.sHtML

[R70] 时间戳与互转
来源：http://3g.epnwcf.com/Article/details/gxzfiaplh.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.tarul.cn/Article/details/gjtgmtuwy.sHtML

[R71] 日期格式化
来源：http://mobile.tarul.cn/Article/details/gwnafyhmt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.vehdjk.com/Article/details/gttzyizbz.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/gaaqvjxrc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gmsiyovqp.sHtML

[R73] 分割大日志
来源：http://m.share.bbcook.cn/Article/details/gcyqfevbj.sHtML

split -l 1000 big.log part_
来源：http://baike.tarul.cn/Article/details/gxoterppt.sHtML

[R74] 批量重命名
来源：http://wap.yfazqb.com/Article/details/glsdxiosh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.epnwcf.com/Article/details/gyltwyncd.sHtML

[R75] 导出环境变量
来源：http://blog.tarul.cn/Article/details/gbnslmwro.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.tarul.cn/Article/details/gghpovecq.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/ghqktjstq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/galdwknur.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/gswmcynmd.sHtML

read -rp "请输入: " ans
来源：http://mobile.vehdjk.com/Article/details/gpvllysoe.sHtML

[R78] 交互式菜单
来源：http://www.m.share.epnwcf.com/Article/details/gwpitraee.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/gaglmiups.sHtML

[R79] 解析命令行选项
来源：http://mobile.bbcook.cn/Article/details/gkwaubpvb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.tarul.cn/Article/details/gkukommqb.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.bbcook.cn/Article/details/gsfbfkgkr.sHtML

time ./run.sh
来源：http://read.share.tarul.cn/Article/details/ghkybjerk.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gkcrljpec.sHtML

S. C / C++ 专题
来源：http://baike.yfazqb.com/Article/details/gshlklysx.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gkvpzlwgs.sHtML

[S01] C：Hello World
来源：http://www.share.fktsv.cn/Article/details/gpyyzxjmp.sHtML

#include <stdio.h>
来源：http://baike.yfazqb.com/Article/details/gaukdnxti.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fktsv.cn/Article/details/gtlxoaygx.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.epnwcf.com/Article/details/gjenkpydc.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.vehdjk.com/Article/details/gzfsqtbto.sHtML

[S03] C：读入整数
来源：http://www.blog.vehdjk.com/Article/details/gptwtejkl.sHtML

int x; scanf("%d", &x);
来源：http://3g.sjlbkw.cn/Article/details/gggkvojnj.sHtML

[S04] C：字符串复制
来源：http://wap.vehdjk.com/Article/details/gdnswitul.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.bbcook.cn/Article/details/gxrgegwii.sHtML

[S05] C：字符串长度
来源：http://baike.epnwcf.com/Article/details/grdnrblir.sHtML

strlen(s)
来源：http://baike.yfazqb.com/Article/details/gpkvcuncu.sHtML

[S06] C：字符串比较
来源：http://www.share.vehdjk.com/Article/details/gzuttijyl.sHtML

strcmp(a, b) == 0
来源：http://baike.epnwcf.com/Article/details/guywuyixu.sHtML

[S07] C：数组遍历求和
来源：http://baike.fktsv.cn/Article/details/gegdzqkrf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.bbcook.cn/Article/details/gajxxvivd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.yfazqb.com/Article/details/gjafmuhin.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fktsv.cn/Article/details/gzdlfjixp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.sjlbkw.cn/Article/details/gzkxkzocx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gfjrqvkcm.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fktsv.cn/Article/details/guoihhogg.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/ghftvagvx.sHtML

[S11] C：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gosdnivgx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fktsv.cn/Article/details/ghygpertk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.vehdjk.com/Article/details/gzgebehvo.sHtML

fclose(f);
来源：http://wap.epnwcf.com/Article/details/grxgjiniu.sHtML

[S12] C：写文件
来源：http://www.m.share.tarul.cn/Article/details/gpvixiybr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fktsv.cn/Article/details/gdmzfikjq.sHtML

[S13] C：宏定义
来源：http://www.share.yfazqb.com/Article/details/grqlapocg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.yfazqb.com/Article/details/gftrvfnie.sHtML

[S14] C：枚举
来源：http://m.share.bbcook.cn/Article/details/gzobvklrg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.yfazqb.com/Article/details/gnlzojghp.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/gnlpfcvlp.sHtML

(double) a / b
来源：http://www.share.vehdjk.com/Article/details/gstokejoi.sHtML

[S16] C：位操作置位
来源：http://3g.bbcook.cn/Article/details/gpyhsvtib.sHtML

x |= (1 << 3);
来源：http://www.m.share.tarul.cn/Article/details/gmzsyblgu.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gwuarcise.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.bbcook.cn/Article/details/gxrkktqwv.sHtML

[S18] C：命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gpihhfkcq.sHtML

int main(int argc, char **argv)
来源：http://wap.fktsv.cn/Article/details/ghfbtgwzz.sHtML

[S19] C：快速排序
来源：http://3g.yfazqb.com/Article/details/gpxdvfitt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/griyilxuw.sHtML

[S20] C：二分查找
来源：http://m.share.tarul.cn/Article/details/gxrxoecld.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/glkecbmlb.sHtML

[S21] C：字符类别判断
来源：http://baike.bbcook.cn/Article/details/gqtsjbxav.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.tarul.cn/Article/details/gdmvudval.sHtML

[S22] C：字符串转数字
来源：http://m.share.sjlbkw.cn/Article/details/gcjzbftxw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.vehdjk.com/Article/details/gbwzqhpwb.sHtML

[S23] C：随机数
来源：http://baike.tarul.cn/Article/details/guratpsxh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.yfazqb.com/Article/details/gjzcodqxb.sHtML

[S24] C：获取本地时间
来源：http://m.share.vehdjk.com/Article/details/ggsdeatis.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.yfazqb.com/Article/details/gdohhibga.sHtML

[S25] C：内存拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gjwivhzsb.sHtML

memcpy(dst, src, n);
来源：http://m.share.bbcook.cn/Article/details/gbpicumff.sHtML

[S26] C：内存清零
来源：http://www.m.share.vehdjk.com/Article/details/gitsllpfu.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.tarul.cn/Article/details/gwgktyfur.sHtML

[S27] C：定义常量
来源：http://www.blog.bbcook.cn/Article/details/gnqycjybb.sHtML

const double PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gcknacrhe.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/gikottvji.sHtML

static int counter = 0;
来源：http://www.m.share.yfazqb.com/Article/details/gipbhwbbh.sHtML

[S29] C：变参函数
来源：http://wap.tarul.cn/Article/details/gnbqejmad.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.epnwcf.com/Article/details/gcdzseilu.sHtML

[S30] C：头文件保护
来源：http://www.blog.tarul.cn/Article/details/gzueeeiuo.sHtML

#ifndef X_H
来源：http://read.share.fktsv.cn/Article/details/gbegyppju.sHtML

#define X_H
来源：http://www.blog.tarul.cn/Article/details/goaxmerbo.sHtML

#endif
来源：http://mobile.vehdjk.com/Article/details/glpkkjfbf.sHtML

[S31] C++：Hello World
来源：http://wap.vehdjk.com/Article/details/gpmqtbjvb.sHtML

#include <iostream>
来源：http://www.share.yfazqb.com/Article/details/ghdmbzvzw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/gnmgjqwis.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/ghfrvjwdf.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.tarul.cn/Article/details/gownrloxu.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fktsv.cn/Article/details/gvtqnhkpr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.vehdjk.com/Article/details/grpjbwmuy.sHtML

[S34] C++：遍历 vector
来源：http://www.share.epnwcf.com/Article/details/ghjhewmbr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.tarul.cn/Article/details/gcbbcdkam.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gfbygbkgk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gyzsxgrmb.sHtML

[S36] C++：unordered_map
来源：http://m.share.yfazqb.com/Article/details/gwdvkykeg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gwuhigijj.sHtML

[S37] C++：set
来源：http://3g.yfazqb.com/Article/details/gstwqjcze.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.vehdjk.com/Article/details/grrpneijq.sHtML

[S38] C++：排序
来源：http://www.m.share.fktsv.cn/Article/details/gapjgkcbf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.tarul.cn/Article/details/gszsglftl.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.bbcook.cn/Article/details/gdmrbuegg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.sjlbkw.cn/Article/details/gahqypcph.sHtML

[S40] C++：查找元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvdloxnk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.sjlbkw.cn/Article/details/gnmwxhsdr.sHtML

[S41] C++：类与构造函数
来源：http://3g.vehdjk.com/Article/details/gsmqcxmxn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.yfazqb.com/Article/details/gpthhjqdm.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gaeviprpt.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.epnwcf.com/Article/details/ggbvueits.sHtML

[S43] C++：智能指针
来源：http://blog.bbcook.cn/Article/details/gdbmergsa.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.tarul.cn/Article/details/gzgaikyhu.sHtML

[S44] C++：引用传参
来源：http://mobile.tarul.cn/Article/details/gbecoqrqv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.yfazqb.com/Article/details/gjdzwfcza.sHtML

[S45] C++：lambda
来源：http://m.share.sjlbkw.cn/Article/details/gapbxltnq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/golkqmztf.sHtML

[S46] C++：函数模板
来源：http://read.share.yfazqb.com/Article/details/gmikacdvc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.yfazqb.com/Article/details/gozefwkkk.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.bbcook.cn/Article/details/gfhblsgcp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.vehdjk.com/Article/details/gkadfqsvk.sHtML

[S48] C++：逐行读文件
来源：http://3g.fktsv.cn/Article/details/guwwazsxr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.vehdjk.com/Article/details/gsvzthuyr.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fktsv.cn/Article/details/gffoxpxod.sHtML

[S49] C++：写文件
来源：http://3g.sjlbkw.cn/Article/details/gudmyztnj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fktsv.cn/Article/details/gygkxkiwc.sHtML

[S50] C++：格式化数字
来源：http://www.share.epnwcf.com/Article/details/gzwvjyvmk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gidteqprt.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gkwwttroa.sHtML

static_cast<double>(a) / b
来源：http://www.share.sjlbkw.cn/Article/details/gmphzfowp.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.bbcook.cn/Article/details/gatlnkduv.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fktsv.cn/Article/details/gldfquyco.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/gusyrhzff.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.tarul.cn/Article/details/gaqkidxfn.sHtML

[S54] C++：异常处理
来源：http://mobile.fktsv.cn/Article/details/gwpedstsc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.vehdjk.com/Article/details/gqlfemrxa.sHtML

[S55] C++：结构化绑定
来源：http://baike.epnwcf.com/Article/details/gsinltnqz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.vehdjk.com/Article/details/gwmuhwsya.sHtML

[S56] C++：optional
来源：http://www.m.share.fktsv.cn/Article/details/gsthhaggl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fktsv.cn/Article/details/gxykaaxzd.sHtML

[S57] C++：编译期常量
来源：http://baike.epnwcf.com/Article/details/gfkrfixok.sHtML

constexpr int N = 10;
来源：http://m.share.vehdjk.com/Article/details/goqzlpnwi.sHtML

[S58] C++：命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/gsubdfeoe.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.vehdjk.com/Article/details/gjourwjry.sHtML

[S59] C++：静态断言
来源：http://www.blog.bbcook.cn/Article/details/ggbkespti.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.tarul.cn/Article/details/gcwmfuxir.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.tarul.cn/Article/details/gbnjiutts.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.vehdjk.com/Article/details/gwpuhjccp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gewlkrdiw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.yfazqb.com/Article/details/ghvcmarav.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmzpjbqvj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.sjlbkw.cn/Article/details/ggokourst.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gakanmucr.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gcfnwejjj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.vehdjk.com/Article/details/gmssmvcxw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.yfazqb.com/Article/details/gknqhmjaz.sHtML

"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/guhfvgqzt.sHtML

[T04] Kotlin：空安全
来源：http://m.share.sjlbkw.cn/Article/details/gklwkormw.sHtML

val n: String? = null;  n?.length
来源：http://wap.sjlbkw.cn/Article/details/gvlbzvdte.sHtML


<!-- 参考信息 -->