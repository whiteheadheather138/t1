代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.yfazqb.com/Article/details/gjhlsalwx.sHtML

[R10] 正则匹配
来源：http://www.share.yfazqb.com/Article/details/gskedvdze.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/guhzzdboh.sHtML

[R11] case 多分支
来源：http://read.share.tarul.cn/Article/details/gkhyxresg.sHtML

case "$1" in
来源：http://read.share.fktsv.cn/Article/details/goadeyuyy.sHtML

start) echo "启动" ;;
来源：http://read.share.bbcook.cn/Article/details/gdinqdvfv.sHtML

stop)  echo "停止" ;;
来源：http://blog.vehdjk.com/Article/details/gevnmqsjh.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.yfazqb.com/Article/details/gcsvjafqp.sHtML

esac
来源：http://mobile.yfazqb.com/Article/details/gyvdknysm.sHtML

[R12] for 遍历文件
来源：http://3g.sjlbkw.cn/Article/details/gafqdtyrq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.epnwcf.com/Article/details/gfnkwqjmk.sHtML

[R13] for 计数循环
来源：http://read.share.yfazqb.com/Article/details/gputvumxo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/glripieya.sHtML

[R14] C 风格 for
来源：http://m.share.fktsv.cn/Article/details/gmffxougp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/ghnogohqz.sHtML

[R15] while 逐行读文件
来源：http://read.share.tarul.cn/Article/details/ghgbhrjhe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.tarul.cn/Article/details/gfveiwdmi.sHtML

[R16] until 等待条件
来源：http://read.share.tarul.cn/Article/details/gsfzbvdyk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gptneavop.sHtML

[R17] 数组定义与取值
来源：http://mobile.sjlbkw.cn/Article/details/gmgekyeju.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.yfazqb.com/Article/details/gamwsytmi.sHtML

[R18] 遍历数组
来源：http://m.share.tarul.cn/Article/details/gjpctjfvz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.vehdjk.com/Article/details/gomgcovze.sHtML

[R19] 数组长度
来源：http://www.share.epnwcf.com/Article/details/gccwzzajc.sHtML

echo "${#arr[@]}"
来源：http://read.share.tarul.cn/Article/details/gzgoyncjy.sHtML

[R20] 关联数组（字典）
来源：http://3g.fktsv.cn/Article/details/guatwfhgq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.epnwcf.com/Article/details/gspwxfhln.sHtML

[R21] 字符串长度
来源：http://wap.epnwcf.com/Article/details/gdoxlwiaj.sHtML

echo "${#s}"
来源：http://blog.bbcook.cn/Article/details/gpfqelfaj.sHtML

[R22] 截取子串
来源：http://wap.epnwcf.com/Article/details/gynopiivy.sHtML

echo "${s:0:5}"
来源：http://wap.tarul.cn/Article/details/giimqqhbv.sHtML

[R23] 字符串替换
来源：http://wap.fktsv.cn/Article/details/gnragbeca.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.tarul.cn/Article/details/gjlqkxqoy.sHtML

[R24] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gfzdhsbbr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.epnwcf.com/Article/details/gpipchnzr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.sjlbkw.cn/Article/details/gsvyrkqxk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.bbcook.cn/Article/details/grnffppcd.sHtML

[R26] 命令替换
来源：http://3g.sjlbkw.cn/Article/details/gonrzteea.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.yfazqb.com/Article/details/gaaoqiosl.sHtML

[R27] 算术展开
来源：http://mobile.bbcook.cn/Article/details/gjglaxtbx.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.vehdjk.com/Article/details/gqohtmqne.sHtML

[R28] 浮点运算
来源：http://baike.yfazqb.com/Article/details/gdnbkhgru.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/gwyhbyjns.sHtML

[R29] 定义函数
来源：http://blog.tarul.cn/Article/details/gazfvfmhj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.tarul.cn/Article/details/gnjfuovnl.sHtML

[R30] 函数返回状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gtwifgtvb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.bbcook.cn/Article/details/ggtbhnygv.sHtML

[R31] 局部变量
来源：http://baike.epnwcf.com/Article/details/gkplyrspq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.yfazqb.com/Article/details/gxzvhinev.sHtML

[R32] 参数个数校验
来源：http://www.m.share.sjlbkw.cn/Article/details/gftcoidwv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.tarul.cn/Article/details/gwuzmmdmy.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.yfazqb.com/Article/details/gdshrgyhv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkfxytjk.sHtML

[R34] 退出时清理
来源：http://www.m.share.epnwcf.com/Article/details/gjegdhtvn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.bbcook.cn/Article/details/gjahvdxfe.sHtML

[R35] 后台执行并等待
来源：http://read.share.yfazqb.com/Article/details/gdyukbozo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.sjlbkw.cn/Article/details/gboprcztu.sHtML

[R36] 并发执行多个任务
来源：http://read.share.yfazqb.com/Article/details/gdykaqydx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.vehdjk.com/Article/details/gkjftjjoo.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.bbcook.cn/Article/details/ghcfewtin.sHtML

files=$(ls -1)
来源：http://m.share.fktsv.cn/Article/details/gatvoaxei.sHtML

[R38] 管道串联
来源：http://blog.epnwcf.com/Article/details/ggfsfyhrm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gfiebtbck.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/glrbgubef.sHtML

cmd > out.log 2>&1
来源：http://blog.epnwcf.com/Article/details/gcrtrzysu.sHtML

[R40] 追加写日志
来源：http://baike.fktsv.cn/Article/details/gddqyndws.sHtML

echo "log" >> out.log
来源：http://www.blog.yfazqb.com/Article/details/gzrxtmbej.sHtML

[R41] 丢弃输出
来源：http://blog.yfazqb.com/Article/details/gvguoivva.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/gkelzfxok.sHtML

[R42] 输入重定向
来源：http://baike.sjlbkw.cn/Article/details/gsqicnlxu.sHtML

wc -l < a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gflrzynyn.sHtML

[R43] 按名字查找文件
来源：http://3g.tarul.cn/Article/details/gljkjnjoj.sHtML

find . -name "*.log" -type f
来源：http://mobile.bbcook.cn/Article/details/gbfkrkfqo.sHtML

[R44] 按修改时间查找
来源：http://read.share.sjlbkw.cn/Article/details/gigfhkbxe.sHtML

find . -mtime -7 -type f
来源：http://3g.vehdjk.com/Article/details/gvqeofhgm.sHtML

[R45] 批量删除
来源：http://mobile.yfazqb.com/Article/details/gwqdylueb.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.epnwcf.com/Article/details/gttdvgkvs.sHtML

[R46] 递归替换文件内容
来源：http://m.share.tarul.cn/Article/details/gsgoivjvw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fktsv.cn/Article/details/grxojmbzp.sHtML

[R47] sed 单行替换
来源：http://wap.bbcook.cn/Article/details/gyabkkmkt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.epnwcf.com/Article/details/grxqhdvir.sHtML

[R48] awk 取指定列
来源：http://read.share.fktsv.cn/Article/details/gapijehns.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gwjuycvgn.sHtML

[R49] awk 带条件
来源：http://www.share.bbcook.cn/Article/details/gemhxbcsh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.yfazqb.com/Article/details/geunweide.sHtML

[R50] awk 求和
来源：http://read.share.vehdjk.com/Article/details/gaocpdtiv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.vehdjk.com/Article/details/ggzwljhht.sHtML

[R51] 排序去重取前几
来源：http://wap.fktsv.cn/Article/details/gbbmepyha.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.bbcook.cn/Article/details/ggtxhnapy.sHtML

[R52] 统计行数
来源：http://m.share.fktsv.cn/Article/details/gsjxpgjav.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gwrsxgygt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.sjlbkw.cn/Article/details/gomwdrfpf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.yfazqb.com/Article/details/gfwuhoqrr.sHtML

[R54] 比较两个文件
来源：http://www.m.share.epnwcf.com/Article/details/gayuzctjy.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/gesqnwcjf.sHtML

[R55] 压缩与解压
来源：http://read.share.bbcook.cn/Article/details/gfcleinsw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.sjlbkw.cn/Article/details/ghfusnned.sHtML

[R56] 远程拷贝
来源：http://baike.sjlbkw.cn/Article/details/gpppoyayp.sHtML

scp file user@host:/path/
来源：http://baike.sjlbkw.cn/Article/details/gqalfhvrs.sHtML

[R57] 远程执行命令
来源：http://read.share.yfazqb.com/Article/details/gmmwovagf.sHtML

ssh user@host 'uptime'
来源：http://read.share.fktsv.cn/Article/details/grtibbijp.sHtML

[R58] 下载文件
来源：http://m.share.yfazqb.com/Article/details/gxrfgocsp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.sjlbkw.cn/Article/details/gwudpcznl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gnjrgyfhy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.tarul.cn/Article/details/gezvmxbxr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/giyzsljbp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.vehdjk.com/Article/details/gloxmybfe.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/gdplyogjh.sHtML

df -h;  du -sh *
来源：http://www.m.share.tarul.cn/Article/details/gysarfcdf.sHtML

[R62] 找最占空间的文件
来源：http://3g.bbcook.cn/Article/details/geucihraq.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.yfazqb.com/Article/details/guojgegvq.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/gscdwylhb.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.vehdjk.com/Article/details/gbwcbhizw.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/gdzxqiekx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.vehdjk.com/Article/details/glncjfhcx.sHtML

[R65] 查看端口占用
来源：http://m.share.vehdjk.com/Article/details/gvetfupbu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fktsv.cn/Article/details/giwjktqhl.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/gpmxyvjxl.sHtML

crontab -e;  crontab -l
来源：http://wap.tarul.cn/Article/details/gezixusrf.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fktsv.cn/Article/details/gidbambzx.sHtML

openssl rand -hex 16
来源：http://m.share.tarul.cn/Article/details/gpqjfqofu.sHtML

[R68] 计算文件校验值
来源：http://www.blog.tarul.cn/Article/details/gjsgheuzz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.epnwcf.com/Article/details/gqowhwrtf.sHtML

[R69] 生成随机密码
来源：http://www.blog.sjlbkw.cn/Article/details/gpfunwyla.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.bbcook.cn/Article/details/gknxbcebg.sHtML

[R70] 时间戳与互转
来源：http://m.share.fktsv.cn/Article/details/grihtalca.sHtML

date +%s;  date -d @1700000000
来源：http://blog.tarul.cn/Article/details/gojfzhgfe.sHtML

[R71] 日期格式化
来源：http://3g.vehdjk.com/Article/details/grcnidkkm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.yfazqb.com/Article/details/gvebihmap.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.vehdjk.com/Article/details/gftgeyxqx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/gbsqmdjrf.sHtML

[R73] 分割大日志
来源：http://read.share.yfazqb.com/Article/details/gfuhrpgvp.sHtML

split -l 1000 big.log part_
来源：http://www.blog.bbcook.cn/Article/details/gcddiqiag.sHtML

[R74] 批量重命名
来源：http://blog.vehdjk.com/Article/details/gsmkcfatf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fktsv.cn/Article/details/gmfqhkyug.sHtML

[R75] 导出环境变量
来源：http://read.share.yfazqb.com/Article/details/gswetevcj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.vehdjk.com/Article/details/gtbbfnviq.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/gqowrltpj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/gatljirzl.sHtML

[R77] 读取用户输入
来源：http://mobile.fktsv.cn/Article/details/gwaeaoibx.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/gfmneaznr.sHtML

[R78] 交互式菜单
来源：http://m.share.tarul.cn/Article/details/gqxcvqgxf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.yfazqb.com/Article/details/giyffetxb.sHtML

[R79] 解析命令行选项
来源：http://baike.epnwcf.com/Article/details/gpjamnkve.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/goufeiuvg.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/gxchlyuyq.sHtML

time ./run.sh
来源：http://baike.tarul.cn/Article/details/gawbtarfn.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gosopifcx.sHtML

S. C / C++ 专题
来源：http://read.share.bbcook.cn/Article/details/gqvywyaff.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gbvmuihcw.sHtML

[S01] C：Hello World
来源：http://3g.fktsv.cn/Article/details/gicozhgbl.sHtML

#include <stdio.h>
来源：http://blog.epnwcf.com/Article/details/gvzzepnee.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.vehdjk.com/Article/details/ghssgxqji.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.yfazqb.com/Article/details/gkjwmsynu.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.yfazqb.com/Article/details/gkhcalssu.sHtML

[S03] C：读入整数
来源：http://baike.yfazqb.com/Article/details/gxqgwyabi.sHtML

int x; scanf("%d", &x);
来源：http://www.share.epnwcf.com/Article/details/gftdtpgmc.sHtML

[S04] C：字符串复制
来源：http://m.share.vehdjk.com/Article/details/gfoccjhfx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.tarul.cn/Article/details/glcbevcpf.sHtML

[S05] C：字符串长度
来源：http://blog.tarul.cn/Article/details/gjuenvawk.sHtML

strlen(s)
来源：http://mobile.yfazqb.com/Article/details/gzrpcpguj.sHtML

[S06] C：字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gwaxxnckb.sHtML

strcmp(a, b) == 0
来源：http://blog.vehdjk.com/Article/details/gsdhpyqeu.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fktsv.cn/Article/details/gllpmikbr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.vehdjk.com/Article/details/gmxzboezd.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.bbcook.cn/Article/details/gfvixxhfx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.vehdjk.com/Article/details/ghdadmfod.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.yfazqb.com/Article/details/gmvhyaqli.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.tarul.cn/Article/details/ggdoaudet.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gubnqhycq.sHtML

int *p = &a;  *p = 5;
来源：http://wap.yfazqb.com/Article/details/gwxnfbzoi.sHtML

[S11] C：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/ggvcuzplw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.tarul.cn/Article/details/gmhzcrsyj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.vehdjk.com/Article/details/gbdkufkwy.sHtML

fclose(f);
来源：http://blog.tarul.cn/Article/details/gclouxnoz.sHtML

[S12] C：写文件
来源：http://mobile.tarul.cn/Article/details/gdagmollh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/gwojcfcrp.sHtML

[S13] C：宏定义
来源：http://blog.sjlbkw.cn/Article/details/gzvvlxuup.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.epnwcf.com/Article/details/giravmnqn.sHtML

[S14] C：枚举
来源：http://www.share.yfazqb.com/Article/details/gwbxaozti.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.yfazqb.com/Article/details/ghnekikgq.sHtML

[S15] C：类型转换
来源：http://www.m.share.epnwcf.com/Article/details/glkdmsbsh.sHtML

(double) a / b
来源：http://read.share.yfazqb.com/Article/details/gbzhbcicx.sHtML

[S16] C：位操作置位
来源：http://www.blog.sjlbkw.cn/Article/details/gmpdcbins.sHtML

x |= (1 << 3);
来源：http://wap.tarul.cn/Article/details/gihvsdvbk.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gabcmjzcg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/gxosmrxvg.sHtML

[S18] C：命令行参数
来源：http://www.m.share.tarul.cn/Article/details/gvntsjqdm.sHtML

int main(int argc, char **argv)
来源：http://3g.vehdjk.com/Article/details/ghfixcypo.sHtML

[S19] C：快速排序
来源：http://www.blog.fktsv.cn/Article/details/ghwmcmubc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/gyecetxwu.sHtML

[S20] C：二分查找
来源：http://m.share.yfazqb.com/Article/details/gqgkyhvxb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gkrrrrbru.sHtML

[S21] C：字符类别判断
来源：http://3g.epnwcf.com/Article/details/gdvsjqkln.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.sjlbkw.cn/Article/details/ggvebwchs.sHtML

[S22] C：字符串转数字
来源：http://read.share.bbcook.cn/Article/details/gctmuywwp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.tarul.cn/Article/details/gpixsdlfa.sHtML

[S23] C：随机数
来源：http://read.share.epnwcf.com/Article/details/gpumbsyku.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.vehdjk.com/Article/details/guqcphbme.sHtML

[S24] C：获取本地时间
来源：http://read.share.epnwcf.com/Article/details/gnkigmqpm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.yfazqb.com/Article/details/gyxyqivwh.sHtML

[S25] C：内存拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gpkdxwibr.sHtML

memcpy(dst, src, n);
来源：http://3g.sjlbkw.cn/Article/details/gebrlivsr.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/gtyaydlqg.sHtML

memset(a, 0, sizeof a);
来源：http://blog.bbcook.cn/Article/details/gokdmiyyl.sHtML

[S27] C：定义常量
来源：http://wap.tarul.cn/Article/details/gvlvajrgr.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gvnsjfebv.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/gwevgasij.sHtML

static int counter = 0;
来源：http://baike.yfazqb.com/Article/details/gnsshtoom.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/gpevulapp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.epnwcf.com/Article/details/gzqbcrwku.sHtML

[S30] C：头文件保护
来源：http://m.share.bbcook.cn/Article/details/gxkubhtir.sHtML

#ifndef X_H
来源：http://m.share.epnwcf.com/Article/details/gdtjndpaq.sHtML

#define X_H
来源：http://read.share.bbcook.cn/Article/details/ghrsuxnmy.sHtML

#endif
来源：http://mobile.fktsv.cn/Article/details/gwklphvrl.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/gscfyplxz.sHtML

#include <iostream>
来源：http://www.blog.bbcook.cn/Article/details/gkjkvuxlh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gzevdgpev.sHtML

[S32] C++：字符串
来源：http://m.share.fktsv.cn/Article/details/glnlkwtzy.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.bbcook.cn/Article/details/gmmawnxpf.sHtML

[S33] C++：vector 增删
来源：http://www.share.vehdjk.com/Article/details/gzmbqbpoc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fktsv.cn/Article/details/gyvregcnp.sHtML

[S34] C++：遍历 vector
来源：http://baike.epnwcf.com/Article/details/gkeefxrde.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.bbcook.cn/Article/details/gltzzxiec.sHtML

[S35] C++：map
来源：http://mobile.epnwcf.com/Article/details/gwiydhgxl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gqygklisz.sHtML

[S36] C++：unordered_map
来源：http://mobile.yfazqb.com/Article/details/gkyhxhkxt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/giqmfxodh.sHtML

[S37] C++：set
来源：http://blog.epnwcf.com/Article/details/gqxzpzmrk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.tarul.cn/Article/details/gavkqeqqr.sHtML

[S38] C++：排序
来源：http://m.share.bbcook.cn/Article/details/gcskghlvq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/ghyqlawwg.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.vehdjk.com/Article/details/gizidzsgu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.vehdjk.com/Article/details/gzlzfxhqr.sHtML

[S40] C++：查找元素
来源：http://read.share.vehdjk.com/Article/details/gkauirckr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fktsv.cn/Article/details/gloxpshnj.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.vehdjk.com/Article/details/gkyiipsqj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fktsv.cn/Article/details/grqobvwkv.sHtML

[S42] C++：继承与虚函数
来源：http://baike.yfazqb.com/Article/details/gkwoijmvp.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.bbcook.cn/Article/details/gflrkslwx.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gfeasplny.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fktsv.cn/Article/details/gsylqlori.sHtML

[S44] C++：引用传参
来源：http://www.blog.vehdjk.com/Article/details/gejllfdzq.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/gbrmtaajw.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gqnciwiwh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.bbcook.cn/Article/details/gjrsbclgy.sHtML

[S46] C++：函数模板
来源：http://3g.vehdjk.com/Article/details/gbraucshv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.epnwcf.com/Article/details/ggojpyfop.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fktsv.cn/Article/details/gbevwzkds.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/guenwwlzg.sHtML

[S48] C++：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gwgztzrrg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gblxsenqg.sHtML

while (std::getline(in, line)) { }
来源：http://baike.epnwcf.com/Article/details/gxtudpzru.sHtML

[S49] C++：写文件
来源：http://www.blog.vehdjk.com/Article/details/gwezifiqh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.tarul.cn/Article/details/gebhafbsm.sHtML

[S50] C++：格式化数字
来源：http://m.share.yfazqb.com/Article/details/gxspytokj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.tarul.cn/Article/details/gfnbguloj.sHtML

[S51] C++：显式类型转换
来源：http://baike.tarul.cn/Article/details/gcmlfyrvo.sHtML

static_cast<double>(a) / b
来源：http://3g.sjlbkw.cn/Article/details/gnqrwdwhx.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.vehdjk.com/Article/details/gwgkqtqfo.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.sjlbkw.cn/Article/details/gewpcvszf.sHtML

[S53] C++：移动语义
来源：http://read.share.tarul.cn/Article/details/giuysjeyt.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.sjlbkw.cn/Article/details/gsfvueeet.sHtML

[S54] C++：异常处理
来源：http://www.share.tarul.cn/Article/details/gqaxlkcnj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.yfazqb.com/Article/details/gdrrkyxsu.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fktsv.cn/Article/details/gkojnclvj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/gwrrajave.sHtML

[S56] C++：optional
来源：http://mobile.fktsv.cn/Article/details/ghoszwiby.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.vehdjk.com/Article/details/gpjckkawu.sHtML

[S57] C++：编译期常量
来源：http://m.share.epnwcf.com/Article/details/gbuhofptc.sHtML

constexpr int N = 10;
来源：http://read.share.tarul.cn/Article/details/gewziriaj.sHtML

[S58] C++：命名空间
来源：http://www.share.bbcook.cn/Article/details/guspdvtko.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fktsv.cn/Article/details/gnmpdkzsh.sHtML

[S59] C++：静态断言
来源：http://read.share.tarul.cn/Article/details/gwywykstm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.bbcook.cn/Article/details/ggrxakdfk.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.epnwcf.com/Article/details/gqzvxegfv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.yfazqb.com/Article/details/golpkwmjl.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gseaolpdr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gudzssywn.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvaunnmaa.sHtML

[T01] Kotlin：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gymxfjqed.sHtML

println("Hello")
来源：http://3g.fktsv.cn/Article/details/gqsqrjgau.sHtML

[T02] Kotlin：变量
来源：http://www.share.yfazqb.com/Article/details/gzttfwlpk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.bbcook.cn/Article/details/gxcdddyby.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/goyajxkqs.sHtML

"值: $b"
来源：http://3g.epnwcf.com/Article/details/gnvdmjfrd.sHtML

[T04] Kotlin：空安全
来源：http://read.share.tarul.cn/Article/details/geqklxlda.sHtML

val n: String? = null;  n?.length
来源：http://blog.vehdjk.com/Article/details/gkrzyicyi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.tarul.cn/Article/details/gvrrnpsxt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fktsv.cn/Article/details/gqsdcpwxt.sHtML

[T06] Kotlin：集合映射
来源：http://wap.sjlbkw.cn/Article/details/gquaciwtl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fktsv.cn/Article/details/goqbioglo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gflhezrqy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.sjlbkw.cn/Article/details/gumobyaxw.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.vehdjk.com/Article/details/gqgwentiv.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.tarul.cn/Article/details/gvgdtfgqu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.sjlbkw.cn/Article/details/gozqrvsdr.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fktsv.cn/Article/details/glhrzraaj.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.vehdjk.com/Article/details/gisisxeby.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.tarul.cn/Article/details/gjasvvhet.sHtML


<!-- 参考信息 -->