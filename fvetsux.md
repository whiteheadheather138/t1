代发 wailian999

set -euo pipefail
来源：http://baike.bbcook.cn/Article/details/gtyifinsb.sHtML

[R02] 变量赋值与使用
来源：http://blog.fktsv.cn/Article/details/gszzxoruz.sHtML

name="Tom"; echo "$name"
来源：http://baike.sjlbkw.cn/Article/details/gwhgnleyv.sHtML

[R03] 只读变量
来源：http://www.share.vehdjk.com/Article/details/gieqixccd.sHtML

readonly PI=3.14
来源：http://www.blog.sjlbkw.cn/Article/details/gfmdpzuma.sHtML

[R04] 位置参数
来源：http://baike.fktsv.cn/Article/details/gbuilguma.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.bbcook.cn/Article/details/glxrwdcxy.sHtML

[R05] 参数默认值
来源：http://www.share.vehdjk.com/Article/details/gchnbajqx.sHtML

name="${1:-default}"
来源：http://www.share.vehdjk.com/Article/details/gcwzdvxqt.sHtML

[R06] 判断命令是否存在
来源：http://mobile.yfazqb.com/Article/details/ggqoxfwwq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/gsgklhnnb.sHtML

[R07] if 判断文件
来源：http://mobile.yfazqb.com/Article/details/ganichkop.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.yfazqb.com/Article/details/gyxlqxknu.sHtML

[R08] 数值比较
来源：http://baike.vehdjk.com/Article/details/gcrbcumvd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.vehdjk.com/Article/details/gpqiunxkr.sHtML

[R09] 字符串比较
来源：http://3g.vehdjk.com/Article/details/ganbjfaks.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/gpvgcffir.sHtML

[R10] 正则匹配
来源：http://wap.bbcook.cn/Article/details/ggdyzsomx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fktsv.cn/Article/details/gwveayiep.sHtML

[R11] case 多分支
来源：http://www.m.share.bbcook.cn/Article/details/ggeobbryb.sHtML

case "$1" in
来源：http://www.blog.tarul.cn/Article/details/gvfdnxhxv.sHtML

start) echo "启动" ;;
来源：http://www.share.bbcook.cn/Article/details/gltpjjpct.sHtML

stop)  echo "停止" ;;
来源：http://blog.yfazqb.com/Article/details/gfbvmbfih.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.yfazqb.com/Article/details/gydrxilmu.sHtML

esac
来源：http://wap.sjlbkw.cn/Article/details/gvdxijupu.sHtML

[R12] for 遍历文件
来源：http://m.share.vehdjk.com/Article/details/gawkpdula.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.epnwcf.com/Article/details/gaswtqhwr.sHtML

[R13] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gkuwjuywz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gkkmzumos.sHtML

[R14] C 风格 for
来源：http://wap.epnwcf.com/Article/details/gbrwxmqql.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gkxkqsdpo.sHtML

[R15] while 逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gqlekufml.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.tarul.cn/Article/details/gtjremfli.sHtML

[R16] until 等待条件
来源：http://mobile.vehdjk.com/Article/details/gqsxddgyj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gqufsmvbt.sHtML

[R17] 数组定义与取值
来源：http://m.share.yfazqb.com/Article/details/gaxxxahau.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.epnwcf.com/Article/details/gpiixmyjr.sHtML

[R18] 遍历数组
来源：http://baike.epnwcf.com/Article/details/gdmddlkbf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.vehdjk.com/Article/details/guaqogrqc.sHtML

[R19] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gaafqsrcv.sHtML

echo "${#arr[@]}"
来源：http://3g.fktsv.cn/Article/details/gpgxinjcy.sHtML

[R20] 关联数组（字典）
来源：http://read.share.sjlbkw.cn/Article/details/ggsuctgqa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.vehdjk.com/Article/details/gmbjshnkw.sHtML

[R21] 字符串长度
来源：http://www.share.tarul.cn/Article/details/gocefeotz.sHtML

echo "${#s}"
来源：http://baike.fktsv.cn/Article/details/gsuynatic.sHtML

[R22] 截取子串
来源：http://www.share.tarul.cn/Article/details/gvdptjnlt.sHtML

echo "${s:0:5}"
来源：http://mobile.epnwcf.com/Article/details/gtsribwam.sHtML

[R23] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gtjllwxov.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.tarul.cn/Article/details/gnnpaawwi.sHtML

[R24] 大小写转换
来源：http://m.share.tarul.cn/Article/details/gmggqwxsh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fktsv.cn/Article/details/gyjgugbgd.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fktsv.cn/Article/details/gguhtobih.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.yfazqb.com/Article/details/gahyuhuvy.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/gdllwdotb.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.epnwcf.com/Article/details/gnhtzrjbg.sHtML

[R27] 算术展开
来源：http://wap.tarul.cn/Article/details/gppsuovki.sHtML

echo $((1 + 2 * 3))
来源：http://3g.bbcook.cn/Article/details/ggsjwdaja.sHtML

[R28] 浮点运算
来源：http://baike.tarul.cn/Article/details/gvlxatlvm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.bbcook.cn/Article/details/gquqccqpk.sHtML

[R29] 定义函数
来源：http://m.share.fktsv.cn/Article/details/gshblzfmx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.yfazqb.com/Article/details/ghklfpctn.sHtML

[R30] 函数返回状态码
来源：http://wap.sjlbkw.cn/Article/details/gbnsyfldl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.epnwcf.com/Article/details/gqltofusj.sHtML

[R31] 局部变量
来源：http://3g.sjlbkw.cn/Article/details/gqyddertb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.tarul.cn/Article/details/giynazxuq.sHtML

[R32] 参数个数校验
来源：http://m.share.vehdjk.com/Article/details/gkaqiwsuc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/gyjehvmzd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.yfazqb.com/Article/details/gglzwiiin.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.bbcook.cn/Article/details/gjvaiivpn.sHtML

[R34] 退出时清理
来源：http://3g.fktsv.cn/Article/details/gfzsvpedm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.yfazqb.com/Article/details/gyhjdvvop.sHtML

[R35] 后台执行并等待
来源：http://mobile.tarul.cn/Article/details/gvxxlsyea.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fktsv.cn/Article/details/getrrinpr.sHtML

[R36] 并发执行多个任务
来源：http://baike.tarul.cn/Article/details/gwrffrgqt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.sjlbkw.cn/Article/details/gcgtnczyl.sHtML

[R37] 把输出赋给变量
来源：http://m.share.tarul.cn/Article/details/gmivdxlmr.sHtML

files=$(ls -1)
来源：http://read.share.bbcook.cn/Article/details/gnqwdutsq.sHtML

[R38] 管道串联
来源：http://www.share.tarul.cn/Article/details/gtylspuwi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.sjlbkw.cn/Article/details/gwugllmye.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.sjlbkw.cn/Article/details/gxibdgrva.sHtML

cmd > out.log 2>&1
来源：http://wap.yfazqb.com/Article/details/gqrkgltbs.sHtML

[R40] 追加写日志
来源：http://blog.tarul.cn/Article/details/gzelysfhm.sHtML

echo "log" >> out.log
来源：http://www.blog.tarul.cn/Article/details/gfsqncksa.sHtML

[R41] 丢弃输出
来源：http://baike.vehdjk.com/Article/details/gjknddzkt.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.vehdjk.com/Article/details/gnkrjuicm.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/gduluiupw.sHtML

wc -l < a.txt
来源：http://blog.epnwcf.com/Article/details/gendhohbz.sHtML

[R43] 按名字查找文件
来源：http://mobile.vehdjk.com/Article/details/guybuwlfd.sHtML

find . -name "*.log" -type f
来源：http://www.share.bbcook.cn/Article/details/gawmtmrnu.sHtML

[R44] 按修改时间查找
来源：http://www.blog.bbcook.cn/Article/details/ghmtqvasc.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.tarul.cn/Article/details/gqynuudyz.sHtML

[R45] 批量删除
来源：http://3g.fktsv.cn/Article/details/glmjkvyol.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.bbcook.cn/Article/details/gsdphknei.sHtML

[R46] 递归替换文件内容
来源：http://blog.vehdjk.com/Article/details/gdavpzxlf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.tarul.cn/Article/details/gowdcbohq.sHtML

[R47] sed 单行替换
来源：http://www.share.epnwcf.com/Article/details/guchhjgpw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.bbcook.cn/Article/details/gjknpuoch.sHtML

[R48] awk 取指定列
来源：http://baike.yfazqb.com/Article/details/gigmqdhxy.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.tarul.cn/Article/details/glnbkrdgj.sHtML

[R49] awk 带条件
来源：http://baike.tarul.cn/Article/details/gcfnvqalw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.epnwcf.com/Article/details/gqssulwum.sHtML

[R50] awk 求和
来源：http://baike.epnwcf.com/Article/details/ggwthoaqt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.bbcook.cn/Article/details/gpdmykwiv.sHtML

[R51] 排序去重取前几
来源：http://m.share.bbcook.cn/Article/details/gfutuilnf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.sjlbkw.cn/Article/details/gkinlcbvy.sHtML

[R52] 统计行数
来源：http://www.blog.yfazqb.com/Article/details/gulssantv.sHtML

wc -l a.txt
来源：http://www.blog.fktsv.cn/Article/details/gpkkzfnts.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fktsv.cn/Article/details/gjtagobow.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.sjlbkw.cn/Article/details/giiufthhz.sHtML

[R54] 比较两个文件
来源：http://www.blog.fktsv.cn/Article/details/gkisgujlo.sHtML

diff a.txt b.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/goxfsljcn.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/guyssbmqz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/gimlyfvly.sHtML

[R56] 远程拷贝
来源：http://mobile.bbcook.cn/Article/details/gmjzqvabq.sHtML

scp file user@host:/path/
来源：http://www.blog.vehdjk.com/Article/details/gkhxenfjq.sHtML

[R57] 远程执行命令
来源：http://m.share.tarul.cn/Article/details/gcofpiaex.sHtML

ssh user@host 'uptime'
来源：http://www.share.epnwcf.com/Article/details/gldxbtche.sHtML

[R58] 下载文件
来源：http://www.blog.fktsv.cn/Article/details/gycoxjqid.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/gqnvssjhe.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gukjrooyc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/gnckymkom.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/gyicjzubm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.bbcook.cn/Article/details/ghwudowvu.sHtML

[R61] 磁盘占用
来源：http://blog.bbcook.cn/Article/details/gidrwzrad.sHtML

df -h;  du -sh *
来源：http://baike.epnwcf.com/Article/details/gigybdkfi.sHtML

[R62] 找最占空间的文件
来源：http://read.share.vehdjk.com/Article/details/gatmlzcdu.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.sjlbkw.cn/Article/details/giinifiwx.sHtML

[R63] 内存与进程
来源：http://read.share.tarul.cn/Article/details/goaqdgubb.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.vehdjk.com/Article/details/gvavkuvff.sHtML

[R64] 结束进程
来源：http://read.share.yfazqb.com/Article/details/grhoiajob.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.yfazqb.com/Article/details/gqqypttwd.sHtML

[R65] 查看端口占用
来源：http://read.share.yfazqb.com/Article/details/giytsnhms.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.yfazqb.com/Article/details/gxyoodegp.sHtML

[R66] 定时任务
来源：http://m.share.fktsv.cn/Article/details/gpjssexxd.sHtML

crontab -e;  crontab -l
来源：http://www.blog.sjlbkw.cn/Article/details/gdlmdcvvu.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fktsv.cn/Article/details/gzypfxkho.sHtML

openssl rand -hex 16
来源：http://baike.fktsv.cn/Article/details/gssboyhyv.sHtML

[R68] 计算文件校验值
来源：http://wap.yfazqb.com/Article/details/gpoeioqxf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.sjlbkw.cn/Article/details/ggjovmonv.sHtML

[R69] 生成随机密码
来源：http://3g.yfazqb.com/Article/details/gbqjlhdhb.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.sjlbkw.cn/Article/details/gecjuqjow.sHtML

[R70] 时间戳与互转
来源：http://m.share.tarul.cn/Article/details/gmsjbhfkv.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fktsv.cn/Article/details/gxhzrmxyj.sHtML

[R71] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gfcalawqi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.epnwcf.com/Article/details/gkvcdofpr.sHtML

[R72] 等待端口就绪
来源：http://www.blog.sjlbkw.cn/Article/details/gfdhvnjvl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gqwahphha.sHtML

[R73] 分割大日志
来源：http://baike.vehdjk.com/Article/details/gegczblbc.sHtML

split -l 1000 big.log part_
来源：http://www.blog.tarul.cn/Article/details/gbmmajpwd.sHtML

[R74] 批量重命名
来源：http://www.blog.epnwcf.com/Article/details/gkdwzzxkz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.tarul.cn/Article/details/ggoooiwxv.sHtML

[R75] 导出环境变量
来源：http://3g.tarul.cn/Article/details/ggcdhchdj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.tarul.cn/Article/details/gkfwhunna.sHtML

[R76] 使用临时文件
来源：http://3g.yfazqb.com/Article/details/gwtmckfes.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gdpqqtgnh.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/glxtvwtkc.sHtML

read -rp "请输入: " ans
来源：http://blog.tarul.cn/Article/details/gpkvedgnd.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/glapngxrb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.tarul.cn/Article/details/gynpkglkq.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fktsv.cn/Article/details/gfvkgzhor.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.yfazqb.com/Article/details/ggmjfuplz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.yfazqb.com/Article/details/gvgtbdany.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/gbixekwlx.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gixdonqhn.sHtML

S. C / C++ 专题
来源：http://3g.vehdjk.com/Article/details/glyayssnu.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gemggqczx.sHtML

[S01] C：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gacpvyzzh.sHtML

#include <stdio.h>
来源：http://read.share.epnwcf.com/Article/details/gsktrffiq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.bbcook.cn/Article/details/gsddowdbp.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fktsv.cn/Article/details/ghipcgljf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.sjlbkw.cn/Article/details/goafhajvn.sHtML

[S03] C：读入整数
来源：http://3g.vehdjk.com/Article/details/gyynvvdhp.sHtML

int x; scanf("%d", &x);
来源：http://www.share.yfazqb.com/Article/details/gntbcgciw.sHtML

[S04] C：字符串复制
来源：http://baike.bbcook.cn/Article/details/gwqlmwdhc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.vehdjk.com/Article/details/gfmlevomk.sHtML

[S05] C：字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gycnfswej.sHtML

strlen(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gvozenipi.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/ghrovcuww.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/gyshllxjt.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/gyjrxoieq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.epnwcf.com/Article/details/gtlbkclxc.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.tarul.cn/Article/details/gpercccoj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.bbcook.cn/Article/details/gcikceuec.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.sjlbkw.cn/Article/details/gapkloeak.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.sjlbkw.cn/Article/details/gtvdxfezk.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fktsv.cn/Article/details/gqjtaqcwt.sHtML

int *p = &a;  *p = 5;
来源：http://baike.vehdjk.com/Article/details/gjoemyhcf.sHtML

[S11] C：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gpyvctrsj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.tarul.cn/Article/details/gmheajqad.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.epnwcf.com/Article/details/gqffnyteb.sHtML

fclose(f);
来源：http://wap.fktsv.cn/Article/details/gjedhogay.sHtML

[S12] C：写文件
来源：http://m.share.fktsv.cn/Article/details/gnacpfvvo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.tarul.cn/Article/details/gksbupexp.sHtML

[S13] C：宏定义
来源：http://www.blog.bbcook.cn/Article/details/grkpwtetn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.tarul.cn/Article/details/gowuqzavg.sHtML

[S14] C：枚举
来源：http://baike.sjlbkw.cn/Article/details/gcapwunhe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.epnwcf.com/Article/details/gggilwhbr.sHtML

[S15] C：类型转换
来源：http://blog.vehdjk.com/Article/details/ggmswnkpq.sHtML

(double) a / b
来源：http://baike.tarul.cn/Article/details/gsdjhqzsw.sHtML

[S16] C：位操作置位
来源：http://www.share.vehdjk.com/Article/details/ghzfunkll.sHtML

x |= (1 << 3);
来源：http://www.blog.tarul.cn/Article/details/gfejrkakd.sHtML

[S17] C：安全拼接字符串
来源：http://wap.yfazqb.com/Article/details/gdscqkczo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.bbcook.cn/Article/details/gtjbjmfrr.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gyfoxqiod.sHtML

int main(int argc, char **argv)
来源：http://3g.fktsv.cn/Article/details/gtgwdeheb.sHtML

[S19] C：快速排序
来源：http://www.blog.vehdjk.com/Article/details/gpgsxwssd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/glkvejjdm.sHtML

[S20] C：二分查找
来源：http://m.share.sjlbkw.cn/Article/details/gjqhjbjtm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/ggjyhnyyh.sHtML

[S21] C：字符类别判断
来源：http://www.blog.tarul.cn/Article/details/gbpfsygtf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.vehdjk.com/Article/details/gowikkvje.sHtML

[S22] C：字符串转数字
来源：http://mobile.fktsv.cn/Article/details/gwzzbfzdp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/gsicbdtvf.sHtML

[S23] C：随机数
来源：http://m.share.vehdjk.com/Article/details/gpddknvyy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.epnwcf.com/Article/details/gyyfwznnd.sHtML

[S24] C：获取本地时间
来源：http://blog.fktsv.cn/Article/details/ggvaotoco.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.tarul.cn/Article/details/ghynoghlh.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.vehdjk.com/Article/details/guntbhbtw.sHtML

memcpy(dst, src, n);
来源：http://blog.epnwcf.com/Article/details/gtfnrkcam.sHtML

[S26] C：内存清零
来源：http://blog.bbcook.cn/Article/details/gvsffjhee.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.sjlbkw.cn/Article/details/gfnzffptx.sHtML

[S27] C：定义常量
来源：http://blog.vehdjk.com/Article/details/gdaicigpf.sHtML

const double PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gdawjzhse.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/gwhikijod.sHtML

static int counter = 0;
来源：http://blog.sjlbkw.cn/Article/details/gwymohjto.sHtML

[S29] C：变参函数
来源：http://3g.tarul.cn/Article/details/gfdasuvry.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.vehdjk.com/Article/details/gstalvjjc.sHtML

[S30] C：头文件保护
来源：http://3g.epnwcf.com/Article/details/gjfbdefie.sHtML

#ifndef X_H
来源：http://mobile.vehdjk.com/Article/details/grzdwpjea.sHtML

#define X_H
来源：http://m.share.fktsv.cn/Article/details/gwsxcopgp.sHtML

#endif
来源：http://read.share.vehdjk.com/Article/details/gpmnxprjy.sHtML

[S31] C++：Hello World
来源：http://m.share.yfazqb.com/Article/details/guldfhacd.sHtML

#include <iostream>
来源：http://m.share.vehdjk.com/Article/details/gwuqmbrcy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.epnwcf.com/Article/details/gcmksahcf.sHtML

[S32] C++：字符串
来源：http://www.m.share.bbcook.cn/Article/details/gofttfjeg.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fktsv.cn/Article/details/gajfanbjd.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.tarul.cn/Article/details/gyfwmmjsg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.yfazqb.com/Article/details/gloiuqeer.sHtML

[S34] C++：遍历 vector
来源：http://read.share.tarul.cn/Article/details/gzywhaejf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.tarul.cn/Article/details/gacbakrdq.sHtML

[S35] C++：map
来源：http://wap.yfazqb.com/Article/details/gmoxdhiuz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gogzrirng.sHtML

[S36] C++：unordered_map
来源：http://wap.sjlbkw.cn/Article/details/gtbmhhdtj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/ggefjlfai.sHtML

[S37] C++：set
来源：http://read.share.fktsv.cn/Article/details/gwjuqtnkn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.epnwcf.com/Article/details/gyxupvlvo.sHtML

[S38] C++：排序
来源：http://blog.tarul.cn/Article/details/gaoqmxucc.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.yfazqb.com/Article/details/gjykbadqh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.yfazqb.com/Article/details/gfxgiouqs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.vehdjk.com/Article/details/gffirpeot.sHtML

[S40] C++：查找元素
来源：http://3g.epnwcf.com/Article/details/girytxhjy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gvhaahbfk.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gnlflvigx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.sjlbkw.cn/Article/details/gvvjxdimw.sHtML

[S42] C++：继承与虚函数
来源：http://wap.sjlbkw.cn/Article/details/gvyajmwri.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.bbcook.cn/Article/details/gwrvfkqpo.sHtML

[S43] C++：智能指针
来源：http://baike.bbcook.cn/Article/details/gkxoqwyjp.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.yfazqb.com/Article/details/geobffqnx.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/gqiejhpyl.sHtML

void inc(int &x) { ++x; }
来源：http://baike.yfazqb.com/Article/details/glajkswug.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gdqlmqxfg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.bbcook.cn/Article/details/glgeespaf.sHtML

[S46] C++：函数模板
来源：http://wap.yfazqb.com/Article/details/grppummrv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.vehdjk.com/Article/details/gmjnlqxbz.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fktsv.cn/Article/details/gsatmzlmr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.bbcook.cn/Article/details/gaamqrsws.sHtML

[S48] C++：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gakxiumyh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fktsv.cn/Article/details/gtdxepblt.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.vehdjk.com/Article/details/gneiuqbsh.sHtML

[S49] C++：写文件
来源：http://3g.tarul.cn/Article/details/gzpwmecup.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.epnwcf.com/Article/details/gqpptdcpo.sHtML

[S50] C++：格式化数字
来源：http://blog.yfazqb.com/Article/details/gumrvglvp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gjfanglqf.sHtML

[S51] C++：显式类型转换
来源：http://blog.bbcook.cn/Article/details/gnzcqohal.sHtML

static_cast<double>(a) / b
来源：http://baike.vehdjk.com/Article/details/gggbsygys.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.bbcook.cn/Article/details/gtgfnmzpj.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.epnwcf.com/Article/details/gonouwwsd.sHtML

[S53] C++：移动语义
来源：http://www.blog.fktsv.cn/Article/details/guiybibfk.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.epnwcf.com/Article/details/gffjlokxi.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/gqttlwklg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.epnwcf.com/Article/details/glrgvnbrz.sHtML

[S55] C++：结构化绑定
来源：http://baike.vehdjk.com/Article/details/gilvxozhh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.epnwcf.com/Article/details/gsmzxennp.sHtML

[S56] C++：optional
来源：http://read.share.tarul.cn/Article/details/gskhhqupc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.yfazqb.com/Article/details/gkxjwavnj.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/gbwllqdco.sHtML

constexpr int N = 10;
来源：http://blog.tarul.cn/Article/details/glciwnesn.sHtML

[S58] C++：命名空间
来源：http://baike.bbcook.cn/Article/details/gvgtddaeu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fktsv.cn/Article/details/gznrpmoaj.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/ggurdvgip.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.epnwcf.com/Article/details/gqfopsniy.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.epnwcf.com/Article/details/ghhszoogz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.bbcook.cn/Article/details/gausvmbdy.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghoucenab.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fktsv.cn/Article/details/gtylhmidp.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gshogivgs.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.yfazqb.com/Article/details/guzkglhqu.sHtML

println("Hello")
来源：http://read.share.fktsv.cn/Article/details/grqgwahxl.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gugeizzvr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.bbcook.cn/Article/details/goipomnch.sHtML


<!-- 参考信息 -->