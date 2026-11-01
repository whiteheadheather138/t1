代发 wailian999

esac
来源：http://read.share.sjlbkw.cn/Article/details/gpnlbbpxk.sHtML

[R12] for 遍历文件
来源：http://blog.epnwcf.com/Article/details/gukdszizk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.sjlbkw.cn/Article/details/gpiwmsafd.sHtML

[R13] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gwcqmmkqh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.yfazqb.com/Article/details/gonibjhzq.sHtML

[R14] C 风格 for
来源：http://mobile.fktsv.cn/Article/details/gmvpdmngf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/ghbqhotzr.sHtML

[R15] while 逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/ghgxhxaer.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.vehdjk.com/Article/details/gusrrnvks.sHtML

[R16] until 等待条件
来源：http://mobile.vehdjk.com/Article/details/gpjzsuyuq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gqdwqimgw.sHtML

[R17] 数组定义与取值
来源：http://3g.fktsv.cn/Article/details/gdvybuytb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.vehdjk.com/Article/details/gnbowqzuy.sHtML

[R18] 遍历数组
来源：http://read.share.fktsv.cn/Article/details/guhxqfxwk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.epnwcf.com/Article/details/gwkmpfycy.sHtML

[R19] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/geugnpfvq.sHtML

echo "${#arr[@]}"
来源：http://3g.sjlbkw.cn/Article/details/gyinxwkfn.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fktsv.cn/Article/details/gloetluwo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.yfazqb.com/Article/details/galvzicaq.sHtML

[R21] 字符串长度
来源：http://3g.vehdjk.com/Article/details/gcxqgilpq.sHtML

echo "${#s}"
来源：http://blog.bbcook.cn/Article/details/gohjpvjls.sHtML

[R22] 截取子串
来源：http://www.share.fktsv.cn/Article/details/gmmzpvcdh.sHtML

echo "${s:0:5}"
来源：http://www.share.bbcook.cn/Article/details/gscatrhjy.sHtML

[R23] 字符串替换
来源：http://3g.sjlbkw.cn/Article/details/gmxccgavu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.yfazqb.com/Article/details/gvxyaulpd.sHtML

[R24] 大小写转换
来源：http://mobile.vehdjk.com/Article/details/goklahetr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.yfazqb.com/Article/details/gijbhumhz.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.epnwcf.com/Article/details/geeyesyis.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gltnwvplm.sHtML

[R26] 命令替换
来源：http://m.share.epnwcf.com/Article/details/gpysetygx.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gywuapzgi.sHtML

[R27] 算术展开
来源：http://www.blog.sjlbkw.cn/Article/details/grajxswhr.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.bbcook.cn/Article/details/giwgfymzn.sHtML

[R28] 浮点运算
来源：http://mobile.vehdjk.com/Article/details/ghagqgpem.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.bbcook.cn/Article/details/gyyceiwod.sHtML

[R29] 定义函数
来源：http://www.blog.yfazqb.com/Article/details/gzrfppjqx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fktsv.cn/Article/details/glidrxsue.sHtML

[R30] 函数返回状态码
来源：http://www.share.fktsv.cn/Article/details/gpppyuzyc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.yfazqb.com/Article/details/gprwqdqxn.sHtML

[R31] 局部变量
来源：http://blog.sjlbkw.cn/Article/details/gdtqedoud.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.tarul.cn/Article/details/glzqfvcue.sHtML

[R32] 参数个数校验
来源：http://blog.vehdjk.com/Article/details/gihljliya.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/gszzibfcj.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.yfazqb.com/Article/details/gxyvcpthy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.tarul.cn/Article/details/gmywjvvsp.sHtML

[R34] 退出时清理
来源：http://mobile.yfazqb.com/Article/details/gvgwyvade.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.sjlbkw.cn/Article/details/giwbhkcpa.sHtML

[R35] 后台执行并等待
来源：http://baike.yfazqb.com/Article/details/gslmvievq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.epnwcf.com/Article/details/gecktbkiz.sHtML

[R36] 并发执行多个任务
来源：http://m.share.bbcook.cn/Article/details/gqwjjsjea.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.sjlbkw.cn/Article/details/gclpiluxd.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/gslwzqwck.sHtML

files=$(ls -1)
来源：http://blog.sjlbkw.cn/Article/details/gkhtdwcqu.sHtML

[R38] 管道串联
来源：http://www.share.bbcook.cn/Article/details/grmjkhgvp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.epnwcf.com/Article/details/gfvgficlg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.yfazqb.com/Article/details/gkgvpqybv.sHtML

cmd > out.log 2>&1
来源：http://read.share.yfazqb.com/Article/details/gferwaszq.sHtML

[R40] 追加写日志
来源：http://www.share.fktsv.cn/Article/details/gczunszab.sHtML

echo "log" >> out.log
来源：http://mobile.fktsv.cn/Article/details/gvqamsbrl.sHtML

[R41] 丢弃输出
来源：http://www.share.vehdjk.com/Article/details/gncgdsijl.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gzizkdevd.sHtML

[R42] 输入重定向
来源：http://www.blog.yfazqb.com/Article/details/ghnsdlbsc.sHtML

wc -l < a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gyrqjdwan.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fktsv.cn/Article/details/gmidtyosp.sHtML

find . -name "*.log" -type f
来源：http://read.share.bbcook.cn/Article/details/gpcesaoyo.sHtML

[R44] 按修改时间查找
来源：http://mobile.yfazqb.com/Article/details/ghykkffyq.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.yfazqb.com/Article/details/gfgwhmvdi.sHtML

[R45] 批量删除
来源：http://www.m.share.bbcook.cn/Article/details/gpbiapwsi.sHtML

find . -name "*.tmp" -delete
来源：http://blog.tarul.cn/Article/details/gsrgyykrs.sHtML

[R46] 递归替换文件内容
来源：http://baike.fktsv.cn/Article/details/gfflffynq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fktsv.cn/Article/details/gmgunfruh.sHtML

[R47] sed 单行替换
来源：http://read.share.vehdjk.com/Article/details/gdfrqxfce.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.yfazqb.com/Article/details/geryyyrfb.sHtML

[R48] awk 取指定列
来源：http://www.blog.yfazqb.com/Article/details/gilfxtxdn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gfazvofjx.sHtML

[R49] awk 带条件
来源：http://www.blog.fktsv.cn/Article/details/gwhbeyxtq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.bbcook.cn/Article/details/gseexlsao.sHtML

[R50] awk 求和
来源：http://read.share.sjlbkw.cn/Article/details/gxtjtddsf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.vehdjk.com/Article/details/glftzhdsx.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/gasbfcnpx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/gfovpotdk.sHtML

[R52] 统计行数
来源：http://wap.vehdjk.com/Article/details/gfwwppyoe.sHtML

wc -l a.txt
来源：http://mobile.yfazqb.com/Article/details/ggssyaifd.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.vehdjk.com/Article/details/gwhzxkgiv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.sjlbkw.cn/Article/details/gjaadfezl.sHtML

[R54] 比较两个文件
来源：http://wap.bbcook.cn/Article/details/gkxnndujd.sHtML

diff a.txt b.txt
来源：http://mobile.epnwcf.com/Article/details/goqpnlzbw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.tarul.cn/Article/details/gntwhjdbk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/genglcuye.sHtML

[R56] 远程拷贝
来源：http://3g.vehdjk.com/Article/details/ghhdrbzqa.sHtML

scp file user@host:/path/
来源：http://mobile.yfazqb.com/Article/details/gacdjhqjt.sHtML

[R57] 远程执行命令
来源：http://wap.bbcook.cn/Article/details/gzcmdddky.sHtML

ssh user@host 'uptime'
来源：http://blog.epnwcf.com/Article/details/gztyefbmw.sHtML

[R58] 下载文件
来源：http://3g.vehdjk.com/Article/details/gnyfhtlgy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.bbcook.cn/Article/details/grpizerwa.sHtML

[R59] 发 POST JSON
来源：http://wap.yfazqb.com/Article/details/gyyboyush.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.sjlbkw.cn/Article/details/giyyexonm.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gbqbsnnxn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.yfazqb.com/Article/details/gziuohfdu.sHtML

[R61] 磁盘占用
来源：http://read.share.epnwcf.com/Article/details/gipqwodcv.sHtML

df -h;  du -sh *
来源：http://m.share.sjlbkw.cn/Article/details/gehnsjmxj.sHtML

[R62] 找最占空间的文件
来源：http://baike.tarul.cn/Article/details/gugseffgm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.vehdjk.com/Article/details/gskpfhtts.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/gyxgodegz.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.bbcook.cn/Article/details/ghgjrohvp.sHtML

[R64] 结束进程
来源：http://www.share.tarul.cn/Article/details/gquqcscrz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.vehdjk.com/Article/details/guclsqolt.sHtML

[R65] 查看端口占用
来源：http://read.share.bbcook.cn/Article/details/gslqugfec.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.tarul.cn/Article/details/ghmckpmks.sHtML

[R66] 定时任务
来源：http://www.m.share.yfazqb.com/Article/details/ghrmfsdoy.sHtML

crontab -e;  crontab -l
来源：http://m.share.vehdjk.com/Article/details/gokotckpg.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/gaqhodgio.sHtML

openssl rand -hex 16
来源：http://m.share.bbcook.cn/Article/details/goueoymey.sHtML

[R68] 计算文件校验值
来源：http://blog.vehdjk.com/Article/details/ghzejteoz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.vehdjk.com/Article/details/grpzvufco.sHtML

[R69] 生成随机密码
来源：http://m.share.yfazqb.com/Article/details/gwiwtyvts.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fktsv.cn/Article/details/gvaclkxde.sHtML

[R70] 时间戳与互转
来源：http://m.share.epnwcf.com/Article/details/gwiigzyha.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/guaojflsz.sHtML

[R71] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gvqjncnpj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.tarul.cn/Article/details/gnserdfzl.sHtML

[R72] 等待端口就绪
来源：http://www.blog.tarul.cn/Article/details/gwfhlnprv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gowomyvlu.sHtML

[R73] 分割大日志
来源：http://read.share.epnwcf.com/Article/details/gmiyppfeq.sHtML

split -l 1000 big.log part_
来源：http://www.blog.yfazqb.com/Article/details/gjypzhlcu.sHtML

[R74] 批量重命名
来源：http://www.blog.vehdjk.com/Article/details/gadrvjlob.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.tarul.cn/Article/details/ggsfvsgrs.sHtML

[R75] 导出环境变量
来源：http://wap.fktsv.cn/Article/details/gpleakwxp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.tarul.cn/Article/details/grtmnwtrr.sHtML

[R76] 使用临时文件
来源：http://www.m.share.bbcook.cn/Article/details/gcnluhsoz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/gaenulwav.sHtML

[R77] 读取用户输入
来源：http://www.share.fktsv.cn/Article/details/glbovurwk.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fktsv.cn/Article/details/gwfgwfiyu.sHtML

[R78] 交互式菜单
来源：http://m.share.fktsv.cn/Article/details/gmlqpxbbg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.tarul.cn/Article/details/gtjpbepoo.sHtML

[R79] 解析命令行选项
来源：http://read.share.vehdjk.com/Article/details/giyjhzzob.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fktsv.cn/Article/details/gttmwkhfx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.epnwcf.com/Article/details/gfgajrnkc.sHtML

time ./run.sh
来源：http://wap.bbcook.cn/Article/details/guuqqyohm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gveboulid.sHtML

S. C / C++ 专题
来源：http://3g.yfazqb.com/Article/details/gcphumbvk.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gkhrkqwcp.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/ghdmgdgme.sHtML

#include <stdio.h>
来源：http://www.blog.epnwcf.com/Article/details/gdqslzprv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.yfazqb.com/Article/details/gnhnxdxcf.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.tarul.cn/Article/details/gzxtigdvf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.yfazqb.com/Article/details/gespokimv.sHtML

[S03] C：读入整数
来源：http://3g.vehdjk.com/Article/details/gdhyvqcdb.sHtML

int x; scanf("%d", &x);
来源：http://blog.epnwcf.com/Article/details/ggjqgovml.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/gqmpogcjo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.yfazqb.com/Article/details/gpqslnltb.sHtML

[S05] C：字符串长度
来源：http://wap.vehdjk.com/Article/details/gvtokfyic.sHtML

strlen(s)
来源：http://www.share.bbcook.cn/Article/details/goorihzbr.sHtML

[S06] C：字符串比较
来源：http://blog.yfazqb.com/Article/details/gqsxxmlkp.sHtML

strcmp(a, b) == 0
来源：http://www.blog.sjlbkw.cn/Article/details/ghyrraomf.sHtML

[S07] C：数组遍历求和
来源：http://read.share.vehdjk.com/Article/details/gvewzzkkx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.epnwcf.com/Article/details/govmbmfmm.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.epnwcf.com/Article/details/gunulxoio.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.yfazqb.com/Article/details/gqrlvmkkl.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.bbcook.cn/Article/details/gyinzcqic.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.sjlbkw.cn/Article/details/gdvktscrl.sHtML

[S10] C：指针与解引用
来源：http://mobile.fktsv.cn/Article/details/gwspdgldt.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.epnwcf.com/Article/details/guucuzxmz.sHtML

[S11] C：逐行读文件
来源：http://baike.tarul.cn/Article/details/gpixsztkj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.vehdjk.com/Article/details/gkrpemtwk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.bbcook.cn/Article/details/gldobmqkx.sHtML

fclose(f);
来源：http://3g.fktsv.cn/Article/details/gfsjjnppm.sHtML

[S12] C：写文件
来源：http://www.share.vehdjk.com/Article/details/gcccgjwcb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.tarul.cn/Article/details/ggdybdxxt.sHtML

[S13] C：宏定义
来源：http://www.m.share.fktsv.cn/Article/details/gvnptpbdn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.yfazqb.com/Article/details/gzviolemn.sHtML

[S14] C：枚举
来源：http://baike.tarul.cn/Article/details/gezregvgy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.sjlbkw.cn/Article/details/gvbyhzgmu.sHtML

[S15] C：类型转换
来源：http://wap.sjlbkw.cn/Article/details/gmrrxiybr.sHtML

(double) a / b
来源：http://baike.fktsv.cn/Article/details/gdftmnxhl.sHtML

[S16] C：位操作置位
来源：http://www.m.share.yfazqb.com/Article/details/gxepkbgye.sHtML

x |= (1 << 3);
来源：http://blog.tarul.cn/Article/details/gwyudixuu.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/gayjkvnpc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.vehdjk.com/Article/details/guuytnuaq.sHtML

[S18] C：命令行参数
来源：http://baike.fktsv.cn/Article/details/gitvyzsho.sHtML

int main(int argc, char **argv)
来源：http://www.share.sjlbkw.cn/Article/details/gsgdmxzms.sHtML

[S19] C：快速排序
来源：http://blog.tarul.cn/Article/details/ghvgnivka.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gfwkjfifi.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gxtcdnqay.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gmcivkzlb.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fktsv.cn/Article/details/gxvfyyjgb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fktsv.cn/Article/details/gpvupvydz.sHtML

[S22] C：字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/gpmloqkyz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.vehdjk.com/Article/details/gqwfzjojd.sHtML

[S23] C：随机数
来源：http://www.m.share.yfazqb.com/Article/details/grzsmtpjz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.tarul.cn/Article/details/gyzajfxbx.sHtML

[S24] C：获取本地时间
来源：http://blog.tarul.cn/Article/details/gbinmegay.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.bbcook.cn/Article/details/ggtlzwqgt.sHtML

[S25] C：内存拷贝
来源：http://m.share.yfazqb.com/Article/details/gtzwudfxb.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/gzpzfdjej.sHtML

[S26] C：内存清零
来源：http://www.m.share.bbcook.cn/Article/details/gagnxrycb.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fktsv.cn/Article/details/gxqtsnenz.sHtML

[S27] C：定义常量
来源：http://3g.epnwcf.com/Article/details/gbescfode.sHtML

const double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/ghmmqjlsh.sHtML

[S28] C：静态变量
来源：http://wap.fktsv.cn/Article/details/gafaryogc.sHtML

static int counter = 0;
来源：http://baike.yfazqb.com/Article/details/gforkueqn.sHtML

[S29] C：变参函数
来源：http://wap.sjlbkw.cn/Article/details/gaoxuzeaw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/gkasipdcw.sHtML

[S30] C：头文件保护
来源：http://www.m.share.yfazqb.com/Article/details/gcvnmrftg.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/gpymzqugn.sHtML

#define X_H
来源：http://www.blog.fktsv.cn/Article/details/gklultzbe.sHtML

#endif
来源：http://3g.fktsv.cn/Article/details/gefswckqd.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/gzxjioezi.sHtML

#include <iostream>
来源：http://wap.bbcook.cn/Article/details/gixgzcesa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.sjlbkw.cn/Article/details/gvqhzvldx.sHtML

[S32] C++：字符串
来源：http://baike.sjlbkw.cn/Article/details/genxvvoty.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.epnwcf.com/Article/details/gqochllez.sHtML

[S33] C++：vector 增删
来源：http://blog.yfazqb.com/Article/details/gsodvpjfa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.sjlbkw.cn/Article/details/giroynyqw.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fktsv.cn/Article/details/gngwihapt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.vehdjk.com/Article/details/ghlfwvuzl.sHtML

[S35] C++：map
来源：http://m.share.yfazqb.com/Article/details/ggeagmfzf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gdkpmqoix.sHtML

[S36] C++：unordered_map
来源：http://mobile.sjlbkw.cn/Article/details/gdkvrnevk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gubjzaqyj.sHtML

[S37] C++：set
来源：http://3g.vehdjk.com/Article/details/gkogwwkwd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fktsv.cn/Article/details/ggqgrpocy.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gqgnggvtz.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.bbcook.cn/Article/details/gppfxgdzu.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.tarul.cn/Article/details/gqjrdtsdn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.epnwcf.com/Article/details/gthrjggcd.sHtML

[S40] C++：查找元素
来源：http://3g.yfazqb.com/Article/details/gcqncyyhd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.tarul.cn/Article/details/gwoukvyzs.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.vehdjk.com/Article/details/gqugrdsql.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.sjlbkw.cn/Article/details/gfxeakfzv.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.bbcook.cn/Article/details/gkaqecegh.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.tarul.cn/Article/details/gnorapiow.sHtML

[S43] C++：智能指针
来源：http://www.share.yfazqb.com/Article/details/gypzsoffc.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/gbsxvyulk.sHtML

[S44] C++：引用传参
来源：http://www.share.fktsv.cn/Article/details/gmtykkmji.sHtML

void inc(int &x) { ++x; }
来源：http://baike.vehdjk.com/Article/details/gofqcjelt.sHtML

[S45] C++：lambda
来源：http://blog.bbcook.cn/Article/details/gimsvmgoz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.yfazqb.com/Article/details/gyljccqmo.sHtML

[S46] C++：函数模板
来源：http://m.share.bbcook.cn/Article/details/gktemprjb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrlsxkyy.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.bbcook.cn/Article/details/gpetcozhb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.vehdjk.com/Article/details/gddlduerv.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gbcuyoojx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.sjlbkw.cn/Article/details/gszzsfaia.sHtML

while (std::getline(in, line)) { }
来源：http://blog.vehdjk.com/Article/details/gfwvczpdv.sHtML

[S49] C++：写文件
来源：http://www.blog.bbcook.cn/Article/details/ghszbnvtk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.yfazqb.com/Article/details/grozsqior.sHtML

[S50] C++：格式化数字
来源：http://read.share.tarul.cn/Article/details/gtqzrwswc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.vehdjk.com/Article/details/ghjsgvlka.sHtML

[S51] C++：显式类型转换
来源：http://wap.yfazqb.com/Article/details/gaaqvorbc.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fktsv.cn/Article/details/gigszlicn.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.tarul.cn/Article/details/ghzrsjclk.sHtML

int size() const noexcept { return n_; }
来源：http://baike.bbcook.cn/Article/details/gstiibmdb.sHtML

[S53] C++：移动语义
来源：http://blog.epnwcf.com/Article/details/gzdfgnayn.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.bbcook.cn/Article/details/gatfmkpvh.sHtML

[S54] C++：异常处理
来源：http://www.m.share.vehdjk.com/Article/details/gnypvqika.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.bbcook.cn/Article/details/gpfgcgmlg.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.yfazqb.com/Article/details/gftzyaejh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.bbcook.cn/Article/details/glbwmthkp.sHtML

[S56] C++：optional
来源：http://3g.sjlbkw.cn/Article/details/gkowhumgf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.yfazqb.com/Article/details/gmqjqpyhf.sHtML

[S57] C++：编译期常量
来源：http://www.blog.bbcook.cn/Article/details/goqrfvydg.sHtML

constexpr int N = 10;
来源：http://wap.yfazqb.com/Article/details/gaxixmxmp.sHtML

[S58] C++：命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gjwsennrx.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fktsv.cn/Article/details/gwdtecnjl.sHtML

[S59] C++：静态断言
来源：http://read.share.tarul.cn/Article/details/geyelzdxx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.yfazqb.com/Article/details/gzjwfnavh.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.sjlbkw.cn/Article/details/gxtpghrjy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.tarul.cn/Article/details/goyzvpldu.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gccmldytx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gldpyocmn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmcslgclq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gnuygyhbn.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gyxzpxuwf.sHtML

[T02] Kotlin：变量
来源：http://m.share.yfazqb.com/Article/details/gxuavkmfu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.yfazqb.com/Article/details/gsjgkdizs.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fktsv.cn/Article/details/grqthlweu.sHtML

"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/gzazskeag.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/gpdoatado.sHtML

val n: String? = null;  n?.length
来源：http://blog.tarul.cn/Article/details/gdnbpgtdw.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.vehdjk.com/Article/details/gkydbrsna.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.sjlbkw.cn/Article/details/gsqfsgate.sHtML

[T06] Kotlin：集合映射
来源：http://blog.tarul.cn/Article/details/gkoygeqdz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fktsv.cn/Article/details/gigfftmta.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gtbzmfhzv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.yfazqb.com/Article/details/gdqrrnltf.sHtML

[T08] Kotlin：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gcqynypkv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gndvylshe.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.tarul.cn/Article/details/gyugfzqpr.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fktsv.cn/Article/details/gwhvlbdve.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fktsv.cn/Article/details/gxemdkatc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.yfazqb.com/Article/details/gclydkuet.sHtML

[T11] Kotlin：协程
来源：http://www.blog.tarul.cn/Article/details/gknllbyao.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.yfazqb.com/Article/details/ggukiqmgo.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fktsv.cn/Article/details/ggfcqlhww.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gdxgnehtn.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.yfazqb.com/Article/details/grrdrkbkw.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gpqdytdir.sHtML

[T14] Kotlin：循环
来源：http://www.blog.yfazqb.com/Article/details/ggeloncxh.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.vehdjk.com/Article/details/genczbvke.sHtML


<!-- 参考信息 -->