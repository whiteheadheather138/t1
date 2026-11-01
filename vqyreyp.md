代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.epnwcf.com/Article/details/gbcplqquk.sHtML

[R10] 正则匹配
来源：http://wap.vehdjk.com/Article/details/gtxvejigo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.tarul.cn/Article/details/gxtvjwhfg.sHtML

[R11] case 多分支
来源：http://mobile.fktsv.cn/Article/details/ghybkaadu.sHtML

case "$1" in
来源：http://3g.epnwcf.com/Article/details/gulsmcpky.sHtML

start) echo "启动" ;;
来源：http://baike.epnwcf.com/Article/details/gezxzoxcl.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.epnwcf.com/Article/details/gwwofghsx.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gffwudpcx.sHtML

esac
来源：http://read.share.epnwcf.com/Article/details/gkwyadtub.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/gybakanfn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.epnwcf.com/Article/details/gixjmqsxk.sHtML

[R13] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gbureumky.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/ghrluxffg.sHtML

[R14] C 风格 for
来源：http://www.m.share.bbcook.cn/Article/details/gsfnehzsf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gdzswmpzc.sHtML

[R15] while 逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gdvhbgqdr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.epnwcf.com/Article/details/gvgrkstpf.sHtML

[R16] until 等待条件
来源：http://blog.sjlbkw.cn/Article/details/ggfpctezf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gnwadhgjp.sHtML

[R17] 数组定义与取值
来源：http://www.share.fktsv.cn/Article/details/gkrviwucn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.bbcook.cn/Article/details/gklvmebxg.sHtML

[R18] 遍历数组
来源：http://3g.bbcook.cn/Article/details/gswzjrhhq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.sjlbkw.cn/Article/details/gwgulbxgd.sHtML

[R19] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gjwzwblzl.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/gzyqphadb.sHtML

[R20] 关联数组（字典）
来源：http://blog.sjlbkw.cn/Article/details/gamgguogz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.epnwcf.com/Article/details/gqhtqdggp.sHtML

[R21] 字符串长度
来源：http://baike.bbcook.cn/Article/details/gxknzehrr.sHtML

echo "${#s}"
来源：http://www.blog.tarul.cn/Article/details/gelkirrbb.sHtML

[R22] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/gwzfkswvw.sHtML

echo "${s:0:5}"
来源：http://m.share.yfazqb.com/Article/details/gxydpjazl.sHtML

[R23] 字符串替换
来源：http://3g.vehdjk.com/Article/details/guitnffok.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.yfazqb.com/Article/details/gcbyanbjx.sHtML

[R24] 大小写转换
来源：http://blog.yfazqb.com/Article/details/gpahivkdb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.epnwcf.com/Article/details/ghcswrjfd.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.tarul.cn/Article/details/gfhdvxmsp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fktsv.cn/Article/details/grbcbgevm.sHtML

[R26] 命令替换
来源：http://baike.sjlbkw.cn/Article/details/gavgifukx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fktsv.cn/Article/details/gtonqjwsc.sHtML

[R27] 算术展开
来源：http://m.share.fktsv.cn/Article/details/gslctajci.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.epnwcf.com/Article/details/ggiuqmkkg.sHtML

[R28] 浮点运算
来源：http://www.m.share.tarul.cn/Article/details/gtodsewpa.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.bbcook.cn/Article/details/gdgylhlla.sHtML

[R29] 定义函数
来源：http://baike.fktsv.cn/Article/details/gbnkjycbk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.bbcook.cn/Article/details/gwrfsscnj.sHtML

[R30] 函数返回状态码
来源：http://mobile.fktsv.cn/Article/details/gxkkffhqk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.tarul.cn/Article/details/gvrwmjrfg.sHtML

[R31] 局部变量
来源：http://www.blog.bbcook.cn/Article/details/gaanvjrwm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fktsv.cn/Article/details/gjevedffy.sHtML

[R32] 参数个数校验
来源：http://3g.tarul.cn/Article/details/gryohugbx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gdslrajtv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fktsv.cn/Article/details/gzfsllhpm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.sjlbkw.cn/Article/details/gmsqcsdeb.sHtML

[R34] 退出时清理
来源：http://3g.fktsv.cn/Article/details/gkqhhgrfl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/gjcleknfr.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.bbcook.cn/Article/details/gnwudnpvq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcswholl.sHtML

[R36] 并发执行多个任务
来源：http://wap.sjlbkw.cn/Article/details/gfrefpgyd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fktsv.cn/Article/details/grqbkuhrj.sHtML

[R37] 把输出赋给变量
来源：http://blog.fktsv.cn/Article/details/gvcpjhwyl.sHtML

files=$(ls -1)
来源：http://m.share.tarul.cn/Article/details/gkibfwwsm.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/grxhhwxvp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.bbcook.cn/Article/details/gvbqikuwm.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fktsv.cn/Article/details/gvedrdzcf.sHtML

cmd > out.log 2>&1
来源：http://baike.tarul.cn/Article/details/gthkyoykj.sHtML

[R40] 追加写日志
来源：http://baike.yfazqb.com/Article/details/gzdcjufpu.sHtML

echo "log" >> out.log
来源：http://mobile.yfazqb.com/Article/details/gwsnghdbq.sHtML

[R41] 丢弃输出
来源：http://m.share.sjlbkw.cn/Article/details/goldifozq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.epnwcf.com/Article/details/gihojkrgs.sHtML

[R42] 输入重定向
来源：http://wap.bbcook.cn/Article/details/gxezdaago.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/gahywvyud.sHtML

[R43] 按名字查找文件
来源：http://www.blog.bbcook.cn/Article/details/gubmrmdqc.sHtML

find . -name "*.log" -type f
来源：http://blog.fktsv.cn/Article/details/gfwblkagr.sHtML

[R44] 按修改时间查找
来源：http://www.blog.yfazqb.com/Article/details/guhglhdol.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.bbcook.cn/Article/details/geljibxoo.sHtML

[R45] 批量删除
来源：http://m.share.vehdjk.com/Article/details/gmrdsqgxy.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.bbcook.cn/Article/details/gtlqfyjxo.sHtML

[R46] 递归替换文件内容
来源：http://m.share.bbcook.cn/Article/details/gpnmacbca.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.sjlbkw.cn/Article/details/gfsabhzuj.sHtML

[R47] sed 单行替换
来源：http://baike.sjlbkw.cn/Article/details/gpgeydmjj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.yfazqb.com/Article/details/gmzdrffzx.sHtML

[R48] awk 取指定列
来源：http://mobile.yfazqb.com/Article/details/gnrpxpscq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.bbcook.cn/Article/details/geboppzhi.sHtML

[R49] awk 带条件
来源：http://3g.vehdjk.com/Article/details/gbwulqgsv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.epnwcf.com/Article/details/gwnirqugh.sHtML

[R50] awk 求和
来源：http://blog.vehdjk.com/Article/details/gqoqtvbbc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.bbcook.cn/Article/details/gioopsjeo.sHtML

[R51] 排序去重取前几
来源：http://blog.vehdjk.com/Article/details/gjzqzdoul.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.epnwcf.com/Article/details/gbdqfedja.sHtML

[R52] 统计行数
来源：http://read.share.vehdjk.com/Article/details/gtqfpukhs.sHtML

wc -l a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gjydlthed.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fktsv.cn/Article/details/gdnyjarfq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fktsv.cn/Article/details/gbxnhnjsd.sHtML

[R54] 比较两个文件
来源：http://www.m.share.yfazqb.com/Article/details/gfdwgmfwx.sHtML

diff a.txt b.txt
来源：http://mobile.sjlbkw.cn/Article/details/gdambhgra.sHtML

[R55] 压缩与解压
来源：http://www.m.share.bbcook.cn/Article/details/giwafhoqc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/gxvrwfmeh.sHtML

[R56] 远程拷贝
来源：http://read.share.epnwcf.com/Article/details/gpatmsbus.sHtML

scp file user@host:/path/
来源：http://www.m.share.fktsv.cn/Article/details/gzvlblpps.sHtML

[R57] 远程执行命令
来源：http://baike.sjlbkw.cn/Article/details/gjiywmjwl.sHtML

ssh user@host 'uptime'
来源：http://wap.sjlbkw.cn/Article/details/guuemfhra.sHtML

[R58] 下载文件
来源：http://m.share.vehdjk.com/Article/details/gthqqhqcq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.vehdjk.com/Article/details/ggoutuhal.sHtML

[R59] 发 POST JSON
来源：http://blog.epnwcf.com/Article/details/gikhbuvhe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.sjlbkw.cn/Article/details/gtshmdzlt.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gapweuzci.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fktsv.cn/Article/details/gukitdeyr.sHtML

[R61] 磁盘占用
来源：http://baike.tarul.cn/Article/details/gfdcrnxlx.sHtML

df -h;  du -sh *
来源：http://wap.sjlbkw.cn/Article/details/gvaamxhew.sHtML

[R62] 找最占空间的文件
来源：http://read.share.epnwcf.com/Article/details/gqirltejm.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.bbcook.cn/Article/details/gyztmgelw.sHtML

[R63] 内存与进程
来源：http://read.share.vehdjk.com/Article/details/gadnadwou.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.vehdjk.com/Article/details/gnugccdcc.sHtML

[R64] 结束进程
来源：http://mobile.vehdjk.com/Article/details/ghubwjtul.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fktsv.cn/Article/details/golkuglrd.sHtML

[R65] 查看端口占用
来源：http://read.share.sjlbkw.cn/Article/details/gfbljerrb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.tarul.cn/Article/details/gtjojzxig.sHtML

[R66] 定时任务
来源：http://mobile.vehdjk.com/Article/details/gvgavzgbm.sHtML

crontab -e;  crontab -l
来源：http://www.blog.yfazqb.com/Article/details/gdjegadmm.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.sjlbkw.cn/Article/details/gzsrrrpxg.sHtML

openssl rand -hex 16
来源：http://mobile.tarul.cn/Article/details/gmrdxqpve.sHtML

[R68] 计算文件校验值
来源：http://mobile.sjlbkw.cn/Article/details/gfgjijrzj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.bbcook.cn/Article/details/grhiudvkx.sHtML

[R69] 生成随机密码
来源：http://m.share.bbcook.cn/Article/details/gxtfbtzfl.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.tarul.cn/Article/details/germrbgkt.sHtML

[R70] 时间戳与互转
来源：http://mobile.bbcook.cn/Article/details/gqcofpfcj.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.bbcook.cn/Article/details/ghimbbydo.sHtML

[R71] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gofvegoce.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.epnwcf.com/Article/details/gzsflplws.sHtML

[R72] 等待端口就绪
来源：http://read.share.bbcook.cn/Article/details/gehmaafbx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.yfazqb.com/Article/details/gscxkbzrr.sHtML

[R73] 分割大日志
来源：http://blog.epnwcf.com/Article/details/gbakcctfm.sHtML

split -l 1000 big.log part_
来源：http://read.share.tarul.cn/Article/details/gbkicjmbh.sHtML

[R74] 批量重命名
来源：http://3g.fktsv.cn/Article/details/gnikmnzxi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.yfazqb.com/Article/details/gzsnypfhj.sHtML

[R75] 导出环境变量
来源：http://www.share.epnwcf.com/Article/details/glcufyxop.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.bbcook.cn/Article/details/glmcoaurs.sHtML

[R76] 使用临时文件
来源：http://baike.vehdjk.com/Article/details/gaewqujtm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gvdlebqgg.sHtML

[R77] 读取用户输入
来源：http://3g.tarul.cn/Article/details/gwcmbpcgu.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/gyhlaicsr.sHtML

[R78] 交互式菜单
来源：http://www.blog.fktsv.cn/Article/details/gjbwesfch.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.sjlbkw.cn/Article/details/gxbykwlee.sHtML

[R79] 解析命令行选项
来源：http://blog.bbcook.cn/Article/details/gnhxyjdvn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.tarul.cn/Article/details/gsoembviv.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.epnwcf.com/Article/details/gzddcbust.sHtML

time ./run.sh
来源：http://baike.bbcook.cn/Article/details/gyvbuerzf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gyjolnheb.sHtML

S. C / C++ 专题
来源：http://read.share.yfazqb.com/Article/details/glmbnesnd.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtvxmeiay.sHtML

[S01] C：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gwrixjtpd.sHtML

#include <stdio.h>
来源：http://m.share.bbcook.cn/Article/details/ggtybdfwq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/gifykyrxm.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.bbcook.cn/Article/details/ggnnjdfeh.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.epnwcf.com/Article/details/guhmquacx.sHtML

[S03] C：读入整数
来源：http://read.share.vehdjk.com/Article/details/ggrmwkepg.sHtML

int x; scanf("%d", &x);
来源：http://3g.bbcook.cn/Article/details/ggjjuwdcg.sHtML

[S04] C：字符串复制
来源：http://www.m.share.tarul.cn/Article/details/gnsradoud.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.yfazqb.com/Article/details/gwvgwhglq.sHtML

[S05] C：字符串长度
来源：http://m.share.epnwcf.com/Article/details/gcovzzqxq.sHtML

strlen(s)
来源：http://read.share.bbcook.cn/Article/details/gvjczpvnt.sHtML

[S06] C：字符串比较
来源：http://read.share.fktsv.cn/Article/details/gslqgovpj.sHtML

strcmp(a, b) == 0
来源：http://baike.sjlbkw.cn/Article/details/gjtnqthzw.sHtML

[S07] C：数组遍历求和
来源：http://mobile.bbcook.cn/Article/details/genkvrnvt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.vehdjk.com/Article/details/gphumsnph.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.sjlbkw.cn/Article/details/gwonybdfg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.bbcook.cn/Article/details/gwsslruhs.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.yfazqb.com/Article/details/gsafwzown.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.bbcook.cn/Article/details/gaqndjkwb.sHtML

[S10] C：指针与解引用
来源：http://wap.fktsv.cn/Article/details/gvcxqgobi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/gvugdqrbb.sHtML

[S11] C：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gluwocoiv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.bbcook.cn/Article/details/gxlitcxai.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gkumrbrcb.sHtML

fclose(f);
来源：http://m.share.epnwcf.com/Article/details/gakuyrvwi.sHtML

[S12] C：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gagmdjeth.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.epnwcf.com/Article/details/ghvqsumwd.sHtML

[S13] C：宏定义
来源：http://www.share.epnwcf.com/Article/details/gnizjfteu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.tarul.cn/Article/details/gjopeyroj.sHtML

[S14] C：枚举
来源：http://www.m.share.yfazqb.com/Article/details/goifiayik.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/gjyfxjpno.sHtML

[S15] C：类型转换
来源：http://3g.epnwcf.com/Article/details/gryslnjqt.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/ggfuqzfjh.sHtML

[S16] C：位操作置位
来源：http://www.share.fktsv.cn/Article/details/ghhthiwbu.sHtML

x |= (1 << 3);
来源：http://mobile.bbcook.cn/Article/details/grvonwxek.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/givdsxjef.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.epnwcf.com/Article/details/gvmumanhb.sHtML

[S18] C：命令行参数
来源：http://3g.bbcook.cn/Article/details/gyxmzxmne.sHtML

int main(int argc, char **argv)
来源：http://mobile.yfazqb.com/Article/details/gchdktjcy.sHtML

[S19] C：快速排序
来源：http://www.share.tarul.cn/Article/details/gwfkhftaw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/ghxmdapda.sHtML

[S20] C：二分查找
来源：http://baike.bbcook.cn/Article/details/gcdipkxcd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/gebaxyvuo.sHtML

[S21] C：字符类别判断
来源：http://baike.yfazqb.com/Article/details/gnuzsrmvy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.bbcook.cn/Article/details/gcbrhzhir.sHtML

[S22] C：字符串转数字
来源：http://blog.epnwcf.com/Article/details/grcxoqbnf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.sjlbkw.cn/Article/details/grobcncfd.sHtML

[S23] C：随机数
来源：http://3g.tarul.cn/Article/details/gdcjebpnv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.tarul.cn/Article/details/gimwgirgm.sHtML

[S24] C：获取本地时间
来源：http://blog.yfazqb.com/Article/details/ggbhadras.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fktsv.cn/Article/details/gmmxcjkkl.sHtML

[S25] C：内存拷贝
来源：http://wap.tarul.cn/Article/details/goqdhkxmv.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/gjovqlobt.sHtML

[S26] C：内存清零
来源：http://mobile.bbcook.cn/Article/details/gtxiqeyob.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.vehdjk.com/Article/details/gwgtpsjhw.sHtML

[S27] C：定义常量
来源：http://www.m.share.epnwcf.com/Article/details/gkfjiioxc.sHtML

const double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gvlnbskqf.sHtML

[S28] C：静态变量
来源：http://www.m.share.yfazqb.com/Article/details/glrbdgodr.sHtML

static int counter = 0;
来源：http://www.share.tarul.cn/Article/details/gurlhvbag.sHtML

[S29] C：变参函数
来源：http://www.blog.fktsv.cn/Article/details/gozcqdhtr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.tarul.cn/Article/details/gbnarmccg.sHtML

[S30] C：头文件保护
来源：http://blog.bbcook.cn/Article/details/galouzoor.sHtML

#ifndef X_H
来源：http://blog.fktsv.cn/Article/details/gplvxfgyt.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/ggjagvjty.sHtML

#endif
来源：http://blog.tarul.cn/Article/details/ghebxeocg.sHtML

[S31] C++：Hello World
来源：http://m.share.yfazqb.com/Article/details/gadsrnmry.sHtML

#include <iostream>
来源：http://www.m.share.bbcook.cn/Article/details/gcpnbmtot.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.sjlbkw.cn/Article/details/gtlejxbcj.sHtML

[S32] C++：字符串
来源：http://baike.epnwcf.com/Article/details/gjfuckzny.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.tarul.cn/Article/details/gpnhfwnoo.sHtML

[S33] C++：vector 增删
来源：http://read.share.fktsv.cn/Article/details/gjzfkrmhd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.sjlbkw.cn/Article/details/gruxmgnpr.sHtML

[S34] C++：遍历 vector
来源：http://www.share.yfazqb.com/Article/details/gtufaduld.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.tarul.cn/Article/details/gnhziavxd.sHtML

[S35] C++：map
来源：http://wap.epnwcf.com/Article/details/gxrstvoqm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/goahidkff.sHtML

[S36] C++：unordered_map
来源：http://mobile.yfazqb.com/Article/details/gdmdkizrz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gfzxydnwj.sHtML

[S37] C++：set
来源：http://read.share.bbcook.cn/Article/details/gullvhyuh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.epnwcf.com/Article/details/gtqnperlo.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/glytntjaw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/gbftaoewk.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.yfazqb.com/Article/details/galwqlgps.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.vehdjk.com/Article/details/gfajnlzsg.sHtML

[S40] C++：查找元素
来源：http://wap.yfazqb.com/Article/details/gqxhvpwbh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fktsv.cn/Article/details/gpwdchugl.sHtML

[S41] C++：类与构造函数
来源：http://m.share.yfazqb.com/Article/details/gjgfbpeot.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/gbucechjf.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/giblrzqzq.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.sjlbkw.cn/Article/details/ghpdkribv.sHtML

[S43] C++：智能指针
来源：http://3g.tarul.cn/Article/details/goemmcdci.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fktsv.cn/Article/details/ghfebveis.sHtML

[S44] C++：引用传参
来源：http://read.share.vehdjk.com/Article/details/gruibagul.sHtML

void inc(int &x) { ++x; }
来源：http://3g.tarul.cn/Article/details/guvhdwemw.sHtML

[S45] C++：lambda
来源：http://www.m.share.epnwcf.com/Article/details/gtvbetwsl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.yfazqb.com/Article/details/gszydbsoq.sHtML

[S46] C++：函数模板
来源：http://baike.sjlbkw.cn/Article/details/gmtaqobxj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.epnwcf.com/Article/details/gnoykgkhv.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fktsv.cn/Article/details/gepbdcoye.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fktsv.cn/Article/details/gyibjrddb.sHtML

[S48] C++：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gfjihspdu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.sjlbkw.cn/Article/details/gkcizlzmu.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.vehdjk.com/Article/details/gemrbzbst.sHtML

[S49] C++：写文件
来源：http://baike.bbcook.cn/Article/details/gmndayvht.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.sjlbkw.cn/Article/details/gptnyodtr.sHtML

[S50] C++：格式化数字
来源：http://blog.yfazqb.com/Article/details/gsgkvngtv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.bbcook.cn/Article/details/ghgbwiayv.sHtML

[S51] C++：显式类型转换
来源：http://blog.fktsv.cn/Article/details/gsnsnxwzb.sHtML

static_cast<double>(a) / b
来源：http://baike.epnwcf.com/Article/details/geizwpnst.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.sjlbkw.cn/Article/details/gdaqahypy.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.yfazqb.com/Article/details/gxiyhhecc.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/gxfwvknlt.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.vehdjk.com/Article/details/gilvsatwy.sHtML

[S54] C++：异常处理
来源：http://3g.vehdjk.com/Article/details/gkpcfutto.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.yfazqb.com/Article/details/gsdgfljzs.sHtML

[S55] C++：结构化绑定
来源：http://3g.tarul.cn/Article/details/gnodykycv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.tarul.cn/Article/details/grlttzfzd.sHtML

[S56] C++：optional
来源：http://mobile.sjlbkw.cn/Article/details/gtsyutsox.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.sjlbkw.cn/Article/details/gxxvsonxf.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fktsv.cn/Article/details/gdlfuxthc.sHtML

constexpr int N = 10;
来源：http://wap.fktsv.cn/Article/details/grijwccpw.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gctorkiad.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.epnwcf.com/Article/details/gqiqmuojw.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/gbrqsiqox.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.bbcook.cn/Article/details/gvyaoixhr.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.vehdjk.com/Article/details/gksznvwjm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gxqlmndcn.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gchgbnryo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.tarul.cn/Article/details/gfzdqmcae.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/grsyqyckf.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/gwhlowyhn.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gmznrqccn.sHtML

[T02] Kotlin：变量
来源：http://www.share.sjlbkw.cn/Article/details/ginypkfyo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/gtznepbwn.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.sjlbkw.cn/Article/details/gctcgtrea.sHtML

"值: $b"
来源：http://baike.epnwcf.com/Article/details/gkftjcqed.sHtML

[T04] Kotlin：空安全
来源：http://3g.bbcook.cn/Article/details/gsewaujca.sHtML

val n: String? = null;  n?.length
来源：http://blog.epnwcf.com/Article/details/gzjcfocfx.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.epnwcf.com/Article/details/gveworwhp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.yfazqb.com/Article/details/gkhpgdbzs.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.epnwcf.com/Article/details/gfcsugdko.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.epnwcf.com/Article/details/goiqysdmu.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gzvsmomdi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.epnwcf.com/Article/details/gyvvhvjey.sHtML

[T08] Kotlin：数据类
来源：http://baike.tarul.cn/Article/details/gtkbhhqcl.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fktsv.cn/Article/details/gcdfwsibn.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.epnwcf.com/Article/details/gekthzyvu.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.yfazqb.com/Article/details/gcbpwqbnw.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fktsv.cn/Article/details/gpdcevsgm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.sjlbkw.cn/Article/details/gnunhysqz.sHtML


<!-- 参考信息 -->