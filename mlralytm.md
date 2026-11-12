代发 wailian999

[Q82] 字符长度与字节长度
来源：http://xtn.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jol.shzxlz.cn

[Q83] 大小写转换
来源：http://spt.iojbl.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pke.haohaochexian.top

[Q84] 去除首尾空格
来源：http://crf.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://qnv.kuanghao11.cn

[Q85] 数值取整
来源：http://lml.ydzc1.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bie.ehwqpu.com

[Q86] 读取 JSON 字段
来源：http://xox.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dwb.pycfn.com

[Q87] JSON 字段做条件
来源：http://onm.uphjek.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jcl.zhaomingkeji.xyz

[Q88] 行转列（条件聚合）
来源：http://poi.yonumen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gon.vqdsnc.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dmr.yonumen.top

[Q89] 判断表是否存在
来源：http://gty.yvedp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://spc.gogol.net.cn

[Q90] 生成序号列
来源：http://kan.fengsongda.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ndl.ybcxt.top

================================================================================
来源：http://smb.xziqi.cn

R. Bash 专题
来源：http://hsc.daria6918.cn

================================================================================
来源：http://wly.ydzc1.top

[R01] shebang 与严格模式
来源：http://ido.fengsongda.top

#!/usr/bin/env bash
来源：http://kdj.0kj1m.cn

set -euo pipefail
来源：http://wah.zhijiandao.cn

[R02] 变量赋值与使用
来源：http://dwg.sweek.top

name="Tom"; echo "$name"
来源：http://vfl.sxryk.cn

[R03] 只读变量
来源：http://gua.tarul.cn

readonly PI=3.14
来源：http://xbn.zhoulong.xyz

[R04] 位置参数
来源：http://fhb.hywenlv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mhc.uphjek.com

[R05] 参数默认值
来源：http://mxb.shuidangran.top

name="${1:-default}"
来源：http://nsr.ywan-chungtsiang.top

[R06] 判断命令是否存在
来源：http://qkb.zdbjq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qwf.gzhubu.top

[R07] if 判断文件
来源：http://cjp.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zob.gaohongyu789.top

[R08] 数值比较
来源：http://wav.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://egk.gotoacloud.top

[R09] 字符串比较
来源：http://zpi.ybcxt.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eyg.jqgfzy.top

[R10] 正则匹配
来源：http://dhf.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kmp.chenjidiqi.icu

[R11] case 多分支
来源：http://cry.shuidangran.top

case "$1" in
来源：http://phx.xylfe.cn

start) echo "启动" ;;
来源：http://pdz.pycfn.com

stop)  echo "停止" ;;
来源：http://zuq.ybcxt.top

*)     echo "未知命令" ;;
来源：http://yjg.wangshuangyany.cn

esac
来源：http://adw.havefunace.top

[R12] for 遍历文件
来源：http://jyj.zhixingplan.top

for f in *.txt; do echo "$f"; done
来源：http://dni.jinqigfzy.top

[R13] for 计数循环
来源：http://eqq.jinqigfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://tsp.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://fkb.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://owp.jinqigfzy.top

[R15] while 逐行读文件
来源：http://his.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zdm.52xcode.cn

[R16] until 等待条件
来源：http://dor.sweek.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ggh.gogol.net.cn

[R17] 数组定义与取值
来源：http://bsz.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://kmc.aibaodan.cn

[R18] 遍历数组
来源：http://gsa.epnwcf.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://odg.ydzc1.top

[R19] 数组长度
来源：http://koj.yongpay.top

echo "${#arr[@]}"
来源：http://hbw.tanke756.top

[R20] 关联数组（字典）
来源：http://tzr.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lje.zhixingplan.top

[R21] 字符串长度
来源：http://mlh.mhx1999.top

echo "${#s}"
来源：http://ovl.smart0.xyz

[R22] 截取子串
来源：http://hgn.hnqzz.top

echo "${s:0:5}"
来源：http://mly.316326.xyz

[R23] 字符串替换
来源：http://bey.jinghuilouyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ddi.zhixingplan.top

[R24] 大小写转换
来源：http://bde.zhengqikj.top

echo "${s^^}"; echo "${s,,}"
来源：http://cyf.vehdjk.com

[R25] 去后缀 / 去前缀
来源：http://tkr.vehdjk.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://fsc.ppjwa.cn

[R26] 命令替换
来源：http://kdi.bjfxy.top

now=$(date +%F); echo "$now"
来源：http://bgd.svipenyu.cn

[R27] 算术展开
来源：http://frs.mhx1999.top

echo $((1 + 2 * 3))
来源：http://yms.jinqigfzy.top

[R28] 浮点运算
来源：http://kix.iojbl.cn

echo "scale=2; 10/3" | bc
来源：http://mel.hywenlv.cn

[R29] 定义函数
来源：http://sfa.uphjek.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jid.yfazqb.com

[R30] 函数返回状态码
来源：http://hnh.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://iwo.hammf.cn

[R31] 局部变量
来源：http://nni.zdbjq.cn

f() { local x=1; echo "$x"; }
来源：http://trs.dashuyun.cn

[R32] 参数个数校验
来源：http://ugn.zhixingplan.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qhw.tian-w.cn

[R33] 捕获错误并提示行号
来源：http://uol.yangfankeji.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vhu.chenzaomai.com

[R34] 退出时清理
来源：http://tik.jqgfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://xcu.hcnkem.com

[R35] 后台执行并等待
来源：http://hvf.guannengcc.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wkr.feifeiyinyue.top

[R36] 并发执行多个任务
来源：http://xyh.fengsongda.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pla.chenjidiqi.icu

[R37] 把输出赋给变量
来源：http://pek.gogol.net.cn

files=$(ls -1)
来源：http://czj.smart0.xyz

[R38] 管道串联
来源：http://wam.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://tee.hnxiangtu.top

[R39] 重定向标准输出与错误
来源：http://ncj.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://lvp.shuidangran.top

[R40] 追加写日志
来源：http://olm.meibo888.top

echo "log" >> out.log
来源：http://msp.havefunace.top

[R41] 丢弃输出
来源：http://mzq.bjfxy.top

cmd >/dev/null 2>&1
来源：http://sks.ydzc1.top

[R42] 输入重定向
来源：http://dzf.aibaodan.cn

wc -l < a.txt
来源：http://vsr.iojbl.cn

[R43] 按名字查找文件
来源：http://plq.tanke756.top

find . -name "*.log" -type f
来源：http://ybr.cashguo.top

[R44] 按修改时间查找
来源：http://oec.hnxiangtu.top

find . -mtime -7 -type f
来源：http://wxq.jinyuanbaomall.cn

[R45] 批量删除
来源：http://lej.ivvv.top

find . -name "*.tmp" -delete
来源：http://txg.smart0.xyz

[R46] 递归替换文件内容
来源：http://blu.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vra.feifeiyinyue.top

[R47] sed 单行替换
来源：http://yjw.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://axw.smart0.xyz

[R48] awk 取指定列
来源：http://xol.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://wnz.svipenyu.cn

[R49] awk 带条件
来源：http://wpv.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kmn.sweek.top

[R50] awk 求和
来源：http://bxt.chenzaomai.com

awk '{s += $2} END {print s}' a.txt
来源：http://ttw.ehwqpu.com

[R51] 排序去重取前几
来源：http://cbn.epnwcf.com

sort a.txt | uniq -c | sort -rn | head
来源：http://yne.nanxuanxn.top

[R52] 统计行数
来源：http://zml.shanyushiyangtech.top

wc -l a.txt
来源：http://pnl.shanyushiyangkeji.top

[R53] 查看文件头与实时尾
来源：http://mxw.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dbp.guannengcc.top

[R54] 比较两个文件
来源：http://kjk.shuidangran.top

diff a.txt b.txt
来源：http://ahm.zhaomingkeji.xyz

[R55] 压缩与解压
来源：http://xgd.ivvv.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cux.sweek.top

[R56] 远程拷贝
来源：http://vye.fktsv.cn

scp file user@host:/path/
来源：http://kcw.jqgufenzy.top

[R57] 远程执行命令
来源：http://frw.meibo888.top

ssh user@host 'uptime'
来源：http://ksm.iojbl.cn

[R58] 下载文件
来源：http://bml.bjfxy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kcu.gaohongyu789.top

[R59] 发 POST JSON
来源：http://vxf.zhoulong.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://reb.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://bwz.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tmj.andypj.xyz

[R61] 磁盘占用
来源：http://wff.gzhubu.top

df -h;  du -sh *
来源：http://kxo.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://jox.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://xmk.aizwys.cn

[R63] 内存与进程
来源：http://yaa.yj20258888.top

free -h;  ps aux | grep nginx
来源：http://uue.shanyushiyangkeji.top

[R64] 结束进程
来源：http://btr.tianlin.xyz

kill -9 $(pgrep -f app.py)
来源：http://ybj.gzhubu.top

[R65] 查看端口占用
来源：http://buw.52xcode.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bxl.haohaochexian.top

[R66] 定时任务
来源：http://fmu.ivvv.top

crontab -e;  crontab -l
来源：http://zsh.meibo888.top

[R67] 生成随机十六进制串
来源：http://mcr.hnxiangtu.top

openssl rand -hex 16
来源：http://dxj.yuxming.cn

[R68] 计算文件校验值
来源：http://tpa.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yzm.nanxinkj.top

[R69] 生成随机密码
来源：http://iwo.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://sie.ivvv.top

[R70] 时间戳与互转
来源：http://llj.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://alf.ppjwa.cn

[R71] 日期格式化
来源：http://sot.hfpthk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xji.aizwys.cn

[R72] 等待端口就绪
来源：http://zgs.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uvx.hywenlv.cn

[R73] 分割大日志
来源：http://nyr.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://bbw.zhijiandao.cn

[R74] 批量重命名
来源：http://kfb.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oxe.haohaochexian.top

[R75] 导出环境变量
来源：http://pnh.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://gtl.yanxiufei.cn

[R76] 使用临时文件
来源：http://xlm.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fir.snrcjt.cn

[R77] 读取用户输入
来源：http://lqb.hnqzz.top

read -rp "请输入: " ans
来源：http://npp.0kj1m.cn

[R78] 交互式菜单
来源：http://tzp.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zzw.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://tkt.jqgfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ues.guowangkeji.top

[R80] 查看脚本执行耗时
来源：http://rpu.zhoulong.xyz

time ./run.sh
来源：http://rzb.iojbl.cn

================================================================================
来源：http://lag.haohaochexian.top

S. C / C++ 专题
来源：http://rii.jinghuilouyu.cn

================================================================================
来源：http://ndm.smart0.xyz

[S01] C：Hello World
来源：http://xti.jinyuanbaomall.cn

#include <stdio.h>
来源：http://pxb.iojbl.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xcg.yfazqb.com

[S02] C：变量与格式化输出
来源：http://iam.xylfe.cn

int a = 10; printf("%d\n", a);
来源：http://hwe.shanyushiyangkeji.top

[S03] C：读入整数
来源：http://hwm.zdbjq.cn

int x; scanf("%d", &x);
来源：http://yzp.aizwys.cn

[S04] C：字符串复制
来源：http://mxo.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://tto.316326.xyz

[S05] C：字符串长度
来源：http://zcx.yongpay.top

strlen(s)
来源：http://tay.tianlin.xyz

[S06] C：字符串比较
来源：http://fae.cashguo.top

strcmp(a, b) == 0
来源：http://lwc.cqqwz.cn

[S07] C：数组遍历求和
来源：http://ymh.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://joi.yanxiufei.cn

[S08] C：动态内存分配与释放
来源：http://rwu.nwbrower.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rqd.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://oin.jqgufenzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kzz.52xcode.cn

[S10] C：指针与解引用
来源：http://rdf.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://uyi.hysaishi.cn

[S11] C：逐行读文件
来源：http://huz.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://ksm.ctjpmb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://zzi.zhixingplan.top

fclose(f);
来源：http://kha.cqqwz.cn

[S12] C：写文件
来源：http://rjz.sysykeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nuz.guowangkeji.top

[S13] C：宏定义
来源：http://vrg.ybcxt.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://svf.yuanzhike.top

[S14] C：枚举
来源：http://ena.jianghu66.top

enum Color { RED, GREEN, BLUE };
来源：http://vvo.xziqi.cn

[S15] C：类型转换
来源：http://zft.sjlbkw.cn

(double) a / b
来源：http://ebh.bjfxy.top

[S16] C：位操作置位
来源：http://tpk.smart0.xyz

x |= (1 << 3);
来源：http://ppp.ydjk.org.cn

[S17] C：安全拼接字符串
来源：http://zdd.zycfv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tho.zhengqikj.top

[S18] C：命令行参数
来源：http://ikc.snrcjt.cn

int main(int argc, char **argv)
来源：http://alk.feifeiyinyue.top

[S19] C：快速排序
来源：http://ajd.gaohongyu789.top

qsort(a, n, sizeof(int), cmp);
来源：http://zdv.jinyuanbaomall.cn

[S20] C：二分查找
来源：http://vzj.gotoacloud.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mqh.bjfxy.top

[S21] C：字符类别判断
来源：http://jak.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://whe.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://oqp.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://ocv.aibaodan.cn

[S23] C：随机数
来源：http://lcx.xylfe.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pru.snrcjt.cn

[S24] C：获取本地时间
来源：http://ylb.hammf.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://icq.gotoacloud.top

[S25] C：内存拷贝
来源：http://kya.hesvh.cn

memcpy(dst, src, n);
来源：http://ozh.tian-w.cn

[S26] C：内存清零
来源：http://ror.havefunace.top

memset(a, 0, sizeof a);
来源：http://nof.tian-w.cn

[S27] C：定义常量
来源：http://efk.xingfuxueyuan.xyz

const double PI = 3.14159;
来源：http://vrd.tarul.cn

[S28] C：静态变量
来源：http://amx.svipenyu.cn

static int counter = 0;
来源：http://bjv.cheryme.top

[S29] C：变参函数
来源：http://pvb.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fmh.guannengcc.top

[S30] C：头文件保护
来源：http://xpd.uphjek.com

#ifndef X_H
来源：http://mym.fktsv.cn

#define X_H
来源：http://hnb.yueranfly.top

#endif
来源：http://nwa.hnxiangtu.top

[S31] C++：Hello World
来源：http://ivp.xingfuxueyuan.xyz

#include <iostream>
来源：http://flf.shzxlz.cn

int main() { std::cout << "Hello\n"; }
来源：http://mzi.nanxinkj.top

[S32] C++：字符串
来源：http://yky.9152youxi.cn

std::string s = "hi";  s += "!";
来源：http://tio.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://lqv.cucudq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dir.fktsv.cn

[S34] C++：遍历 vector
来源：http://yuv.gzhubu.top

for (auto &x : v) { std::cout << x; }
来源：http://gpx.feifeiyinyue.top

[S35] C++：map
来源：http://tte.nanxuanxn.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://shh.yj20258888.top

[S36] C++：unordered_map
来源：http://nad.yj20258888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://win.yonumen.top

[S37] C++：set
来源：http://tby.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://exl.zhiwuduotai.top

[S38] C++：排序
来源：http://nzt.aizwys.cn

std::sort(v.begin(), v.end());
来源：http://fdr.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://cwn.dianchejie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dom.yuanzhike.top

[S40] C++：查找元素
来源：http://aor.jinghuilouyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ift.ctjpmb.com

[S41] C++：类与构造函数
来源：http://jgx.jyoumei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ean.gzhubu.top

[S42] C++：继承与虚函数
来源：http://ikf.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://gli.daria6918.cn

[S43] C++：智能指针
来源：http://mtj.zycfv.cn

auto p = std::make_unique<int>(5);
来源：http://blp.jqgufenzy.top

[S44] C++：引用传参
来源：http://kbb.yj202588.top

void inc(int &x) { ++x; }
来源：http://ulo.wangdashe.top

[S45] C++：lambda
来源：http://maf.yongpay.top

auto add = [](int a, int b) { return a + b; };
来源：http://njg.fzhhl.top

[S46] C++：函数模板
来源：http://qea.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ybx.tanke756.top

[S47] C++：结构化绑定遍历
来源：http://bgm.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zih.xingfuxueyuan.xyz

[S48] C++：逐行读文件
来源：http://ajg.yj20258.top

std::ifstream in("a.txt");  std::string line;
来源：http://cfu.nanxinkj.top

while (std::getline(in, line)) { }
来源：http://anb.jqgfzy.top

[S49] C++：写文件
来源：http://shv.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zrz.jiagoushi.top

[S50] C++：格式化数字
来源：http://zpb.chenzaomai.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fwe.zycfv.cn

[S51] C++：显式类型转换
来源：http://dob.pycfn.com

static_cast<double>(a) / b
来源：http://xcp.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://vrj.xingfuxueyuan.xyz


<!-- 参考信息 -->