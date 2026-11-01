代发 wailian999

case "$1" in
来源：http://baike.epnwcf.com/Article/details/gmarbkxgj.sHtML

start) echo "启动" ;;
来源：http://mobile.sjlbkw.cn/Article/details/geocsqsrw.sHtML

stop)  echo "停止" ;;
来源：http://wap.yfazqb.com/Article/details/guqhpccmb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.tarul.cn/Article/details/gchnlgxoy.sHtML

esac
来源：http://wap.vehdjk.com/Article/details/gmctjuoum.sHtML

[R12] for 遍历文件
来源：http://blog.tarul.cn/Article/details/gvdecmlwc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.bbcook.cn/Article/details/geasxxgls.sHtML

[R13] for 计数循环
来源：http://www.share.tarul.cn/Article/details/gvblstwdk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gjmprsand.sHtML

[R14] C 风格 for
来源：http://mobile.epnwcf.com/Article/details/gqoszgkmd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gekufrhps.sHtML

[R15] while 逐行读文件
来源：http://blog.fktsv.cn/Article/details/gmpovkirh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.bbcook.cn/Article/details/gwtlypyla.sHtML

[R16] until 等待条件
来源：http://blog.sjlbkw.cn/Article/details/gxnwpupkc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gnzgevdeh.sHtML

[R17] 数组定义与取值
来源：http://m.share.bbcook.cn/Article/details/gbyheeyvd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/grhwpjdtx.sHtML

[R18] 遍历数组
来源：http://www.m.share.bbcook.cn/Article/details/gnwyvkgeo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gsgvqrtcj.sHtML

[R19] 数组长度
来源：http://blog.yfazqb.com/Article/details/gqvazevzq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.vehdjk.com/Article/details/gkfkjnbvh.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.bbcook.cn/Article/details/gbfrfwlff.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/gnosqtzri.sHtML

[R21] 字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gxcfcgkus.sHtML

echo "${#s}"
来源：http://mobile.sjlbkw.cn/Article/details/gdiczijoo.sHtML

[R22] 截取子串
来源：http://www.share.fktsv.cn/Article/details/gyikguqsj.sHtML

echo "${s:0:5}"
来源：http://www.share.fktsv.cn/Article/details/gsogijioj.sHtML

[R23] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gdtrpmkjv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.sjlbkw.cn/Article/details/grajxtuef.sHtML

[R24] 大小写转换
来源：http://3g.vehdjk.com/Article/details/genlvlxor.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.tarul.cn/Article/details/glpguhmxg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.epnwcf.com/Article/details/gkgbqhrhx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.sjlbkw.cn/Article/details/ggtxkzybz.sHtML

[R26] 命令替换
来源：http://m.share.fktsv.cn/Article/details/gpbzuxkup.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fktsv.cn/Article/details/gqvbwmilm.sHtML

[R27] 算术展开
来源：http://blog.yfazqb.com/Article/details/gkbvlxaut.sHtML

echo $((1 + 2 * 3))
来源：http://baike.vehdjk.com/Article/details/gihijzoyd.sHtML

[R28] 浮点运算
来源：http://baike.epnwcf.com/Article/details/gtmhchilr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.bbcook.cn/Article/details/gfdnrgnbl.sHtML

[R29] 定义函数
来源：http://3g.bbcook.cn/Article/details/gbionbcxk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fktsv.cn/Article/details/gnohurnwx.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/grcuydgwx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/ghpurbteh.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/gnoetiwxf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.epnwcf.com/Article/details/guvsbjbbu.sHtML

[R32] 参数个数校验
来源：http://www.share.tarul.cn/Article/details/gwufjpvie.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.epnwcf.com/Article/details/gojhzcvpi.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.sjlbkw.cn/Article/details/gbfhfixln.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.sjlbkw.cn/Article/details/gxsfpfcyi.sHtML

[R34] 退出时清理
来源：http://mobile.sjlbkw.cn/Article/details/gardvikgn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gedsxtjta.sHtML

[R35] 后台执行并等待
来源：http://www.share.sjlbkw.cn/Article/details/glmyvbedb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gcxvvkrdh.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fktsv.cn/Article/details/gkgwpjzzr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.vehdjk.com/Article/details/grcndwpag.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.yfazqb.com/Article/details/gdzsxnlvv.sHtML

files=$(ls -1)
来源：http://mobile.vehdjk.com/Article/details/gmyywhhjs.sHtML

[R38] 管道串联
来源：http://baike.yfazqb.com/Article/details/gzzicdezf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.tarul.cn/Article/details/gxdplouuc.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/glwokszbd.sHtML

cmd > out.log 2>&1
来源：http://wap.vehdjk.com/Article/details/gndivbelb.sHtML

[R40] 追加写日志
来源：http://www.blog.yfazqb.com/Article/details/gseshrvnt.sHtML

echo "log" >> out.log
来源：http://baike.vehdjk.com/Article/details/gdkzhahha.sHtML

[R41] 丢弃输出
来源：http://blog.tarul.cn/Article/details/gdywbjiaq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.bbcook.cn/Article/details/gxranufnv.sHtML

[R42] 输入重定向
来源：http://www.m.share.yfazqb.com/Article/details/giuaqhwto.sHtML

wc -l < a.txt
来源：http://blog.fktsv.cn/Article/details/gfwyduprd.sHtML

[R43] 按名字查找文件
来源：http://blog.bbcook.cn/Article/details/gntfphyor.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gohujwzln.sHtML

[R44] 按修改时间查找
来源：http://www.share.yfazqb.com/Article/details/gauhlpfnj.sHtML

find . -mtime -7 -type f
来源：http://3g.tarul.cn/Article/details/gtpdosxoo.sHtML

[R45] 批量删除
来源：http://baike.bbcook.cn/Article/details/gabboyxdq.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.tarul.cn/Article/details/gusqjwuoa.sHtML

[R46] 递归替换文件内容
来源：http://3g.bbcook.cn/Article/details/grxtwdsce.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.sjlbkw.cn/Article/details/gttjmacag.sHtML

[R47] sed 单行替换
来源：http://m.share.epnwcf.com/Article/details/gcxwjedpg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fktsv.cn/Article/details/gaikygjcy.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/gtonmults.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fktsv.cn/Article/details/gjbmbrfbk.sHtML

[R49] awk 带条件
来源：http://mobile.sjlbkw.cn/Article/details/gppdmjecg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/gepapfuih.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/goowtidwc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gqncakaxx.sHtML

[R51] 排序去重取前几
来源：http://baike.yfazqb.com/Article/details/gnpkilvya.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.bbcook.cn/Article/details/gogqsalsi.sHtML

[R52] 统计行数
来源：http://blog.tarul.cn/Article/details/gdvkhxlxp.sHtML

wc -l a.txt
来源：http://m.share.vehdjk.com/Article/details/gegrugulp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.sjlbkw.cn/Article/details/gnddoqlsj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.vehdjk.com/Article/details/gkioviexq.sHtML

[R54] 比较两个文件
来源：http://read.share.epnwcf.com/Article/details/gvjfzcaxp.sHtML

diff a.txt b.txt
来源：http://m.share.epnwcf.com/Article/details/guzbfolmz.sHtML

[R55] 压缩与解压
来源：http://3g.vehdjk.com/Article/details/gveqtwiht.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.vehdjk.com/Article/details/gncitcjvr.sHtML

[R56] 远程拷贝
来源：http://3g.epnwcf.com/Article/details/geogsvdfp.sHtML

scp file user@host:/path/
来源：http://read.share.fktsv.cn/Article/details/gwdhnqpqo.sHtML

[R57] 远程执行命令
来源：http://www.m.share.tarul.cn/Article/details/gtungthky.sHtML

ssh user@host 'uptime'
来源：http://3g.bbcook.cn/Article/details/gyhmdogue.sHtML

[R58] 下载文件
来源：http://blog.sjlbkw.cn/Article/details/guitjvqxb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fktsv.cn/Article/details/gjqvlbpyd.sHtML

[R59] 发 POST JSON
来源：http://wap.yfazqb.com/Article/details/giyetikgx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.yfazqb.com/Article/details/gwwsrxcgy.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/gdrybscxn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.tarul.cn/Article/details/glvcggerq.sHtML

[R61] 磁盘占用
来源：http://www.share.yfazqb.com/Article/details/girkjcuwn.sHtML

df -h;  du -sh *
来源：http://3g.vehdjk.com/Article/details/gllnzrhqm.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/gokgbzcyp.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.bbcook.cn/Article/details/geupyykrh.sHtML

[R63] 内存与进程
来源：http://www.blog.bbcook.cn/Article/details/goitfmtfj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.sjlbkw.cn/Article/details/gdqpejenr.sHtML

[R64] 结束进程
来源：http://blog.sjlbkw.cn/Article/details/gcjtyetjt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.tarul.cn/Article/details/gxdnihakm.sHtML

[R65] 查看端口占用
来源：http://read.share.vehdjk.com/Article/details/govxydpya.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.epnwcf.com/Article/details/gwrylnhuf.sHtML

[R66] 定时任务
来源：http://blog.epnwcf.com/Article/details/gxweancfa.sHtML

crontab -e;  crontab -l
来源：http://m.share.yfazqb.com/Article/details/giyccrmxn.sHtML

[R67] 生成随机十六进制串
来源：http://baike.bbcook.cn/Article/details/gjzwzpbha.sHtML

openssl rand -hex 16
来源：http://wap.fktsv.cn/Article/details/gmuyrtanv.sHtML

[R68] 计算文件校验值
来源：http://3g.bbcook.cn/Article/details/gmsjjeawl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.vehdjk.com/Article/details/gfvlevqso.sHtML

[R69] 生成随机密码
来源：http://www.share.yfazqb.com/Article/details/gcjrhdvdr.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.yfazqb.com/Article/details/gbfkapmln.sHtML

[R70] 时间戳与互转
来源：http://3g.vehdjk.com/Article/details/gwxuqzpus.sHtML

date +%s;  date -d @1700000000
来源：http://baike.epnwcf.com/Article/details/gpyccyqcv.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gjmmgudwm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.yfazqb.com/Article/details/govwckhll.sHtML

[R72] 等待端口就绪
来源：http://3g.tarul.cn/Article/details/gjpgejahe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/godwdyjdm.sHtML

[R73] 分割大日志
来源：http://3g.vehdjk.com/Article/details/gvgycclha.sHtML

split -l 1000 big.log part_
来源：http://m.share.epnwcf.com/Article/details/glrhwhisr.sHtML

[R74] 批量重命名
来源：http://www.share.fktsv.cn/Article/details/gzxivcmeh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.bbcook.cn/Article/details/glzisgopr.sHtML

[R75] 导出环境变量
来源：http://blog.tarul.cn/Article/details/gbknqcyco.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.vehdjk.com/Article/details/gaqsflodu.sHtML

[R76] 使用临时文件
来源：http://wap.sjlbkw.cn/Article/details/gzvsnmmub.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gzybycpkc.sHtML

[R77] 读取用户输入
来源：http://www.share.tarul.cn/Article/details/grrdqwaez.sHtML

read -rp "请输入: " ans
来源：http://read.share.tarul.cn/Article/details/gqsjmocef.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/gvbnajkbg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.yfazqb.com/Article/details/gjxeuwhbh.sHtML

[R79] 解析命令行选项
来源：http://mobile.bbcook.cn/Article/details/ggyazvodr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.sjlbkw.cn/Article/details/glbfaeamb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.yfazqb.com/Article/details/gdwqcuaaf.sHtML

time ./run.sh
来源：http://wap.epnwcf.com/Article/details/gjucwtnbe.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gesxyvrgz.sHtML

S. C / C++ 专题
来源：http://m.share.tarul.cn/Article/details/gwxwwsxkf.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gryxowtwf.sHtML

[S01] C：Hello World
来源：http://m.share.epnwcf.com/Article/details/gfjbnqjys.sHtML

#include <stdio.h>
来源：http://wap.vehdjk.com/Article/details/gtvfpxotm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.vehdjk.com/Article/details/gfsxnuzvf.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.yfazqb.com/Article/details/gmrwpoqyr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.yfazqb.com/Article/details/gufowuqsy.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gnlvexhhq.sHtML

int x; scanf("%d", &x);
来源：http://read.share.vehdjk.com/Article/details/gjptayuji.sHtML

[S04] C：字符串复制
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjrzntuv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fktsv.cn/Article/details/gbtcldyqt.sHtML

[S05] C：字符串长度
来源：http://m.share.fktsv.cn/Article/details/gswlclzqb.sHtML

strlen(s)
来源：http://www.blog.tarul.cn/Article/details/gwvxsasea.sHtML

[S06] C：字符串比较
来源：http://www.share.yfazqb.com/Article/details/gbyagmqoi.sHtML

strcmp(a, b) == 0
来源：http://baike.sjlbkw.cn/Article/details/gyopbqmns.sHtML

[S07] C：数组遍历求和
来源：http://blog.yfazqb.com/Article/details/guexlwqin.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fktsv.cn/Article/details/gyumubuzt.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fktsv.cn/Article/details/ggtgggvbb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.bbcook.cn/Article/details/gxmngwcmd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.epnwcf.com/Article/details/ggwvmxfjb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.vehdjk.com/Article/details/gvhuxqjcm.sHtML

[S10] C：指针与解引用
来源：http://3g.vehdjk.com/Article/details/gxvvufyup.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fktsv.cn/Article/details/gdiddanct.sHtML

[S11] C：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gglgznkmn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.vehdjk.com/Article/details/gtvjdtzqb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.bbcook.cn/Article/details/glvqlbrmn.sHtML

fclose(f);
来源：http://m.share.fktsv.cn/Article/details/ggmzlhhzs.sHtML

[S12] C：写文件
来源：http://baike.sjlbkw.cn/Article/details/guteueaum.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gtfuhcgwc.sHtML

[S13] C：宏定义
来源：http://mobile.vehdjk.com/Article/details/gpbqrryss.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.tarul.cn/Article/details/gprgixdhr.sHtML

[S14] C：枚举
来源：http://3g.fktsv.cn/Article/details/gcehrhbga.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.vehdjk.com/Article/details/gnonjtqyy.sHtML

[S15] C：类型转换
来源：http://baike.tarul.cn/Article/details/gxcbfmcvo.sHtML

(double) a / b
来源：http://read.share.yfazqb.com/Article/details/grcobaupr.sHtML

[S16] C：位操作置位
来源：http://3g.yfazqb.com/Article/details/gxoogzkpu.sHtML

x |= (1 << 3);
来源：http://wap.epnwcf.com/Article/details/glysqjnge.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gldejfomo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.vehdjk.com/Article/details/gdhtmvntp.sHtML

[S18] C：命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gbcarbuvq.sHtML

int main(int argc, char **argv)
来源：http://blog.bbcook.cn/Article/details/gsbrtlpnm.sHtML

[S19] C：快速排序
来源：http://mobile.tarul.cn/Article/details/gbtkkkkxi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gyxcyvqzr.sHtML

[S20] C：二分查找
来源：http://3g.sjlbkw.cn/Article/details/gtkibsgvd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gtfgbwpjr.sHtML

[S21] C：字符类别判断
来源：http://www.blog.yfazqb.com/Article/details/gcmdnjxaj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/gyhqazvta.sHtML

[S22] C：字符串转数字
来源：http://3g.yfazqb.com/Article/details/gdnrbaidy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.vehdjk.com/Article/details/gdjbcfoet.sHtML

[S23] C：随机数
来源：http://www.share.vehdjk.com/Article/details/gvfafvlbs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.tarul.cn/Article/details/gjxbxdqga.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/giyctgdxh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fktsv.cn/Article/details/gbemdpbvg.sHtML

[S25] C：内存拷贝
来源：http://www.share.vehdjk.com/Article/details/guzpmpwxk.sHtML

memcpy(dst, src, n);
来源：http://wap.vehdjk.com/Article/details/gtvugajeo.sHtML

[S26] C：内存清零
来源：http://m.share.yfazqb.com/Article/details/guevlrnvr.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/gygpttxcd.sHtML

[S27] C：定义常量
来源：http://m.share.fktsv.cn/Article/details/gapesluhh.sHtML

const double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gejrqzqqu.sHtML

[S28] C：静态变量
来源：http://mobile.sjlbkw.cn/Article/details/gmdhpeaxj.sHtML

static int counter = 0;
来源：http://wap.tarul.cn/Article/details/gmytzsqnx.sHtML

[S29] C：变参函数
来源：http://wap.sjlbkw.cn/Article/details/ghqitthzg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.tarul.cn/Article/details/gopbmfzyl.sHtML

[S30] C：头文件保护
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwmyvzyu.sHtML

#ifndef X_H
来源：http://mobile.fktsv.cn/Article/details/gxjdnpanl.sHtML

#define X_H
来源：http://baike.tarul.cn/Article/details/gbcbtqmck.sHtML

#endif
来源：http://wap.yfazqb.com/Article/details/gayyjxdqc.sHtML

[S31] C++：Hello World
来源：http://read.share.fktsv.cn/Article/details/gsfckveal.sHtML

#include <iostream>
来源：http://www.blog.yfazqb.com/Article/details/gyylqarol.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.epnwcf.com/Article/details/gxhshvgyj.sHtML

[S32] C++：字符串
来源：http://blog.yfazqb.com/Article/details/gxeuawbar.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.tarul.cn/Article/details/gsxkvrrpt.sHtML

[S33] C++：vector 增删
来源：http://www.blog.sjlbkw.cn/Article/details/gfabihibh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gobnrnrjd.sHtML

[S34] C++：遍历 vector
来源：http://www.share.bbcook.cn/Article/details/gezixmeug.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fktsv.cn/Article/details/gnrmiavvn.sHtML

[S35] C++：map
来源：http://mobile.bbcook.cn/Article/details/gdnrnvigd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gvoskgmzp.sHtML

[S36] C++：unordered_map
来源：http://3g.bbcook.cn/Article/details/gctfzpmjr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/gnposlual.sHtML

[S37] C++：set
来源：http://www.share.epnwcf.com/Article/details/gzmqjzoxx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fktsv.cn/Article/details/grsstujai.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/grisfoagi.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.bbcook.cn/Article/details/grobfjmaw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.vehdjk.com/Article/details/gljbabbiu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.tarul.cn/Article/details/gfhgzlxsh.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fktsv.cn/Article/details/gacqgeyjs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.yfazqb.com/Article/details/gzaswojhv.sHtML

[S41] C++：类与构造函数
来源：http://3g.sjlbkw.cn/Article/details/gfoqqebuy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fktsv.cn/Article/details/gdbdvdbou.sHtML

[S42] C++：继承与虚函数
来源：http://3g.tarul.cn/Article/details/gxaakrinx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.yfazqb.com/Article/details/gdugmqzkv.sHtML

[S43] C++：智能指针
来源：http://read.share.bbcook.cn/Article/details/gyodetfua.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/gjyughshs.sHtML

[S44] C++：引用传参
来源：http://www.share.epnwcf.com/Article/details/gahvilngl.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.yfazqb.com/Article/details/gpyirpnyc.sHtML

[S45] C++：lambda
来源：http://m.share.epnwcf.com/Article/details/gwulxanaj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gcqcmpylf.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gofoitqyt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.tarul.cn/Article/details/ghnmilunh.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.vehdjk.com/Article/details/gpyavmpyj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.tarul.cn/Article/details/govjaqyun.sHtML

[S48] C++：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/goaxoujcd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fktsv.cn/Article/details/gcqilbjfc.sHtML

while (std::getline(in, line)) { }
来源：http://blog.yfazqb.com/Article/details/gbzxxcrvd.sHtML

[S49] C++：写文件
来源：http://baike.fktsv.cn/Article/details/gvjmspihc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.epnwcf.com/Article/details/gmcbbqcgp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.epnwcf.com/Article/details/gbwoyerdx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.vehdjk.com/Article/details/gquqczmam.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.bbcook.cn/Article/details/gvgzmcbjx.sHtML

static_cast<double>(a) / b
来源：http://baike.bbcook.cn/Article/details/gtkhmrzks.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.sjlbkw.cn/Article/details/gicvnyoyr.sHtML

int size() const noexcept { return n_; }
来源：http://3g.bbcook.cn/Article/details/gzjfnaqdr.sHtML

[S53] C++：移动语义
来源：http://mobile.tarul.cn/Article/details/gkkyvktqo.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/gnuihulkr.sHtML

[S54] C++：异常处理
来源：http://www.blog.fktsv.cn/Article/details/gratofudy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.tarul.cn/Article/details/gwhnvqwxx.sHtML

[S55] C++：结构化绑定
来源：http://3g.bbcook.cn/Article/details/gnhnkuqiz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.yfazqb.com/Article/details/gvclzwyvl.sHtML

[S56] C++：optional
来源：http://blog.yfazqb.com/Article/details/gloedvpgc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fktsv.cn/Article/details/gkthliqiu.sHtML

[S57] C++：编译期常量
来源：http://mobile.sjlbkw.cn/Article/details/gdxzrnzij.sHtML

constexpr int N = 10;
来源：http://wap.epnwcf.com/Article/details/gizwjsand.sHtML

[S58] C++：命名空间
来源：http://mobile.bbcook.cn/Article/details/gcktsswpj.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.bbcook.cn/Article/details/ggllupkkl.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/gezxslmbu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.vehdjk.com/Article/details/ggfhuthzd.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.epnwcf.com/Article/details/gmylpwlyi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.vehdjk.com/Article/details/gcdzcesac.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gngjucvwj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gtjpltmjy.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gxfsofang.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.vehdjk.com/Article/details/gpzaopdzn.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/gpsvcqlsh.sHtML

[T02] Kotlin：变量
来源：http://www.share.fktsv.cn/Article/details/gzchuaslq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.bbcook.cn/Article/details/gevnddcyi.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fktsv.cn/Article/details/gtuortuub.sHtML

"值: $b"
来源：http://read.share.bbcook.cn/Article/details/grsiqavjw.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.yfazqb.com/Article/details/gseevwoxb.sHtML

val n: String? = null;  n?.length
来源：http://www.share.bbcook.cn/Article/details/grfrgxxov.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.epnwcf.com/Article/details/gjusfmtsl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fktsv.cn/Article/details/gltcpjjhg.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.vehdjk.com/Article/details/gkmtqseso.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fktsv.cn/Article/details/getkfyogd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.yfazqb.com/Article/details/gpqfhlple.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fktsv.cn/Article/details/gmftdaijn.sHtML

[T08] Kotlin：数据类
来源：http://wap.sjlbkw.cn/Article/details/gralkykrb.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.epnwcf.com/Article/details/gibbqwkoh.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.epnwcf.com/Article/details/glkierfsc.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.bbcook.cn/Article/details/gybgvwdzd.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.vehdjk.com/Article/details/gizkhbszi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fktsv.cn/Article/details/gdvfbfcge.sHtML

[T11] Kotlin：协程
来源：http://read.share.bbcook.cn/Article/details/gnrlphgur.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.tarul.cn/Article/details/gbtdbfeby.sHtML

[T12] Kotlin：解构声明
来源：http://blog.sjlbkw.cn/Article/details/gygzcjork.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.tarul.cn/Article/details/gagkpaxur.sHtML


<!-- 参考信息 -->