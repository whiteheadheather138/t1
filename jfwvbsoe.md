代发 wailian999

R. Bash 专题
来源：http://wao.chenzaomai.com

================================================================================
来源：http://cyb.uphjek.com

[R01] shebang 与严格模式
来源：http://vvk.havefunace.top

#!/usr/bin/env bash
来源：http://ddr.daria6918.cn

set -euo pipefail
来源：http://jub.fehbvm.com

[R02] 变量赋值与使用
来源：http://fkh.aibaodan.cn

name="Tom"; echo "$name"
来源：http://xth.fanxiaobao.xyz

[R03] 只读变量
来源：http://pcw.kuanghao11.cn

readonly PI=3.14
来源：http://zzo.zhongyouzk.top

[R04] 位置参数
来源：http://wzb.52xcode.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://edk.haohaochexian.top

[R05] 参数默认值
来源：http://zly.sweek.top

name="${1:-default}"
来源：http://lex.hcnkem.com

[R06] 判断命令是否存在
来源：http://lra.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ufy.havefunace.top

[R07] if 判断文件
来源：http://ehu.nanxuanxn.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ftb.ehwqpu.com

[R08] 数值比较
来源：http://fgv.sxryk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sbn.daria6918.cn

[R09] 字符串比较
来源：http://dfm.yj202588.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zzr.hammf.cn

[R10] 正则匹配
来源：http://phb.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sju.hcnkem.com

[R11] case 多分支
来源：http://qqb.ydzc1.top

case "$1" in
来源：http://nqy.sysykeji.top

start) echo "启动" ;;
来源：http://rmc.yueranfly.top

stop)  echo "停止" ;;
来源：http://amu.gzhubu.top

*)     echo "未知命令" ;;
来源：http://vbs.yongpay.top

esac
来源：http://krb.zhaomingkeji.xyz

[R12] for 遍历文件
来源：http://yah.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://ukd.jinghuilouyu.cn

[R13] for 计数循环
来源：http://unq.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://xah.gzhubu.top

[R14] C 风格 for
来源：http://gzx.52xcode.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pmo.yonumen.top

[R15] while 逐行读文件
来源：http://hyw.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dgl.316326.xyz

[R16] until 等待条件
来源：http://zez.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wvi.shanyushiyangkeji.top

[R17] 数组定义与取值
来源：http://tkw.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://biv.zhaomingkeji.xyz

[R18] 遍历数组
来源：http://lhl.gaohongyu789.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ioy.xuanzx.com

[R19] 数组长度
来源：http://wrx.jianghu66.top

echo "${#arr[@]}"
来源：http://kjm.0kj1m.cn

[R20] 关联数组（字典）
来源：http://vxx.tanke756.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hjf.yuxming.cn

[R21] 字符串长度
来源：http://jni.yanxiufei.cn

echo "${#s}"
来源：http://pfv.zhiwuduotai.top

[R22] 截取子串
来源：http://yht.aibaodan.cn

echo "${s:0:5}"
来源：http://ihe.gaohongyu789.top

[R23] 字符串替换
来源：http://zow.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://utd.aibaodan.cn

[R24] 大小写转换
来源：http://vwz.hfpthk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gmf.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://hfh.jinyuanbaomall.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://adi.sxryk.cn

[R26] 命令替换
来源：http://lso.aibaodan.cn

now=$(date +%F); echo "$now"
来源：http://qid.shangyingyoupin.top

[R27] 算术展开
来源：http://wye.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://pkc.hcnkem.com

[R28] 浮点运算
来源：http://pbq.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://aqc.sweek.top

[R29] 定义函数
来源：http://lel.yvedp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zfj.jinqigfzy.top

[R30] 函数返回状态码
来源：http://qmn.yj20258888.top

f() { return 0; }; f || echo "失败了"
来源：http://yxy.chenzaomai.com

[R31] 局部变量
来源：http://yrd.havefunace.top

f() { local x=1; echo "$x"; }
来源：http://zpu.tianlin.xyz

[R32] 参数个数校验
来源：http://xod.c1oappe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rvc.jinyuanbaomall.cn

[R33] 捕获错误并提示行号
来源：http://tij.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ayj.svipenyu.cn

[R34] 退出时清理
来源：http://lms.zdbjq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rlm.pycfn.com

[R35] 后台执行并等待
来源：http://swu.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jdh.xinyue.icu

[R36] 并发执行多个任务
来源：http://qlj.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gsg.fengsongda.top

[R37] 把输出赋给变量
来源：http://dgf.zhiwuduotai.top

files=$(ls -1)
来源：http://vjb.chenlongwang.top

[R38] 管道串联
来源：http://rmq.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://pup.zhaomingkeji.xyz

[R39] 重定向标准输出与错误
来源：http://pvr.tian-w.cn

cmd > out.log 2>&1
来源：http://ggy.andypj.xyz

[R40] 追加写日志
来源：http://lvx.shangyingyoupin.top

echo "log" >> out.log
来源：http://bvi.zycfv.cn

[R41] 丢弃输出
来源：http://btr.316326.xyz

cmd >/dev/null 2>&1
来源：http://tis.uphjek.com

[R42] 输入重定向
来源：http://evy.c1oappe.top

wc -l < a.txt
来源：http://zro.uphjek.com

[R43] 按名字查找文件
来源：http://rxp.vehdjk.com

find . -name "*.log" -type f
来源：http://kde.tarul.cn

[R44] 按修改时间查找
来源：http://xly.sxryk.cn

find . -mtime -7 -type f
来源：http://eoc.yongpay.top

[R45] 批量删除
来源：http://yog.ybcxt.top

find . -name "*.tmp" -delete
来源：http://mxh.fzhhl.top

[R46] 递归替换文件内容
来源：http://yml.ywan-chungtsiang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xhf.sufxvd.cn

[R47] sed 单行替换
来源：http://pon.tanke756.top

sed -i 's/foo/bar/g' a.txt
来源：http://psn.shzxlz.cn

[R48] awk 取指定列
来源：http://guk.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://zfc.chenlongwang.top

[R49] awk 带条件
来源：http://bxc.tianlin.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ptg.zhongyouzk.top

[R50] awk 求和
来源：http://fjv.andypj.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://fkn.zhongyouzk.top

[R51] 排序去重取前几
来源：http://glt.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://unn.xziqi.cn

[R52] 统计行数
来源：http://ijj.zhaomingkeji.xyz

wc -l a.txt
来源：http://rfe.xziqi.cn

[R53] 查看文件头与实时尾
来源：http://gto.tian-w.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xok.zhoulong.xyz

[R54] 比较两个文件
来源：http://mdo.0kj1m.cn

diff a.txt b.txt
来源：http://afz.jlsjyb.cn

[R55] 压缩与解压
来源：http://bsi.zhongyouzk.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zva.nwbrower.top

[R56] 远程拷贝
来源：http://kpn.chenzaomai.com

scp file user@host:/path/
来源：http://mtf.yj20258.top

[R57] 远程执行命令
来源：http://nzb.ppjwa.cn

ssh user@host 'uptime'
来源：http://gro.svipenyu.cn

[R58] 下载文件
来源：http://fop.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gpc.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://igk.cucudq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://srv.zdbjq.cn

[R60] 只看 HTTP 状态码
来源：http://nys.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mct.ydjk.org.cn

[R61] 磁盘占用
来源：http://wot.hammf.cn

df -h;  du -sh *
来源：http://ayb.mhx1999.top

[R62] 找最占空间的文件
来源：http://ejf.cheryme.top

du -ah . | sort -rh | head -10
来源：http://sgy.jianghu66.top

[R63] 内存与进程
来源：http://qlt.havefunace.top

free -h;  ps aux | grep nginx
来源：http://lux.mhx1999.top

[R64] 结束进程
来源：http://cjp.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://ybn.shanyushiyangkeji.top

[R65] 查看端口占用
来源：http://sbg.ivvv.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sxc.jlsjyb.cn

[R66] 定时任务
来源：http://ypw.epnwcf.com

crontab -e;  crontab -l
来源：http://tbk.zhoulong.xyz

[R67] 生成随机十六进制串
来源：http://ijo.9152youxi.cn

openssl rand -hex 16
来源：http://oqg.wangdashe.top

[R68] 计算文件校验值
来源：http://yml.hammf.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lnb.fzhhl.top

[R69] 生成随机密码
来源：http://puh.bjfxy.top

head -c 16 /dev/urandom | base64
来源：http://xsv.zhixingplan.top

[R70] 时间戳与互转
来源：http://fwq.mhx1999.top

date +%s;  date -d @1700000000
来源：http://dvz.nwbrower.top

[R71] 日期格式化
来源：http://daq.yangfankeji.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://zli.xuanzx.com

[R72] 等待端口就绪
来源：http://cva.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://pqy.smart0.xyz

[R73] 分割大日志
来源：http://yju.hfpthk.cn

split -l 1000 big.log part_
来源：http://yjf.tanke756.top

[R74] 批量重命名
来源：http://cnz.dianchejie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://var.shzxlz.cn

[R75] 导出环境变量
来源：http://qql.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://tjq.chenzaomai.com

[R76] 使用临时文件
来源：http://nuz.jqgufenzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iup.chenlongwang.top

[R77] 读取用户输入
来源：http://zbn.zhongyouzk.top

read -rp "请输入: " ans
来源：http://vxf.tian-w.cn

[R78] 交互式菜单
来源：http://iwf.daria6918.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vnj.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://vsv.jqgufenzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yst.dashuyun.cn

[R80] 查看脚本执行耗时
来源：http://ovs.chenjidiqi.icu

time ./run.sh
来源：http://hox.fehbvm.com

================================================================================
来源：http://uko.cheryme.top

S. C / C++ 专题
来源：http://juo.yuxming.cn

================================================================================
来源：http://bjn.yuxming.cn

[S01] C：Hello World
来源：http://hbc.yueranfly.top

#include <stdio.h>
来源：http://mma.sjlbkw.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cws.bbcook.cn

[S02] C：变量与格式化输出
来源：http://tno.hnxiangtu.top

int a = 10; printf("%d\n", a);
来源：http://mei.gogol.net.cn

[S03] C：读入整数
来源：http://nja.birdmap.top

int x; scanf("%d", &x);
来源：http://egv.nanxinkj.top

[S04] C：字符串复制
来源：http://brt.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://dim.xinyue.icu

[S05] C：字符串长度
来源：http://dur.c1oappe.top

strlen(s)
来源：http://tmf.nwbrower.top

[S06] C：字符串比较
来源：http://nbv.hongshengwenyu.top

strcmp(a, b) == 0
来源：http://bpz.jianghu66.top

[S07] C：数组遍历求和
来源：http://wbu.xingfuxueyuan.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pbt.daxiang520.top

[S08] C：动态内存分配与释放
来源：http://mdr.bbcook.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oyj.cucudq.cn

[S09] C：结构体定义与初始化
来源：http://zjk.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dtj.yuxming.cn

[S10] C：指针与解引用
来源：http://rhr.uphjek.com

int *p = &a;  *p = 5;
来源：http://xet.gaohongyu789.top

[S11] C：逐行读文件
来源：http://hnw.shzxlz.cn

FILE *f = fopen("a.txt", "r");
来源：http://olw.hysaishi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://elf.ywan-chungtsiang.top

fclose(f);
来源：http://nsa.zhijiandao.cn

[S12] C：写文件
来源：http://seg.ppjwa.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jjh.mhx1999.top

[S13] C：宏定义
来源：http://nzm.c1oappe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kkq.yangfankeji.com

[S14] C：枚举
来源：http://pck.gaohongyu789.top

enum Color { RED, GREEN, BLUE };
来源：http://oxn.gzhubu.top

[S15] C：类型转换
来源：http://upv.yfazqb.com

(double) a / b
来源：http://czs.ywan-chungtsiang.top

[S16] C：位操作置位
来源：http://cac.0kj1m.cn

x |= (1 << 3);
来源：http://soz.jqgfzy.top

[S17] C：安全拼接字符串
来源：http://ljx.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://avb.jinyuanbaomall.cn

[S18] C：命令行参数
来源：http://opr.zhaomingkeji.xyz

int main(int argc, char **argv)
来源：http://cgp.jinghuilouyu.cn

[S19] C：快速排序
来源：http://yyk.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://gwv.redwolf501.top

[S20] C：二分查找
来源：http://bzp.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://okg.gaohongyu789.top

[S21] C：字符类别判断
来源：http://rkq.shangyingyoupin.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ujx.hnxiangtu.top

[S22] C：字符串转数字
来源：http://tev.iojbl.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jsd.hcnkem.com

[S23] C：随机数
来源：http://bnc.shanyushiyangtech.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nix.sweek.top

[S24] C：获取本地时间
来源：http://ndi.hcnkem.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kiz.9152youxi.cn

[S25] C：内存拷贝
来源：http://jtb.0kj1m.cn

memcpy(dst, src, n);
来源：http://cgw.yvedp.cn

[S26] C：内存清零
来源：http://chj.yonumen.top

memset(a, 0, sizeof a);
来源：http://gzd.ydzc1.top

[S27] C：定义常量
来源：http://whe.shangyingyoupin.top

const double PI = 3.14159;
来源：http://nlh.daria6918.cn

[S28] C：静态变量
来源：http://dlv.zdbjq.cn

static int counter = 0;
来源：http://fzr.meibo888.top

[S29] C：变参函数
来源：http://huw.0kj1m.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nxi.iojbl.cn

[S30] C：头文件保护
来源：http://hnz.sweek.top

#ifndef X_H
来源：http://pyi.yfazqb.com

#define X_H
来源：http://hdu.sufxvd.cn

#endif
来源：http://akm.gzhubu.top

[S31] C++：Hello World
来源：http://wzi.wangdashe.top

#include <iostream>
来源：http://mix.yuxming.cn

int main() { std::cout << "Hello\n"; }
来源：http://eck.hnqzz.top

[S32] C++：字符串
来源：http://pec.yonumen.top

std::string s = "hi";  s += "!";
来源：http://pdl.uphjek.com

[S33] C++：vector 增删
来源：http://xat.quarkkingdee.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rpg.hcnkem.com

[S34] C++：遍历 vector
来源：http://rkp.andypj.xyz

for (auto &x : v) { std::cout << x; }
来源：http://wis.shuidangran.top

[S35] C++：map
来源：http://jrf.uphjek.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rui.epnwcf.com

[S36] C++：unordered_map
来源：http://xrf.aibaodan.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mcg.sxryk.cn

[S37] C++：set
来源：http://lrj.xingfuxueyuan.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uvp.jinqigfzy.top

[S38] C++：排序
来源：http://prd.jinghuilouyu.cn

std::sort(v.begin(), v.end());
来源：http://fyd.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://ipk.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ncr.svipenyu.cn

[S40] C++：查找元素
来源：http://jfo.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ero.fanxiaobao.xyz

[S41] C++：类与构造函数
来源：http://ukn.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tqb.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://wbi.smart0.xyz

class B : public Base { public: void f() override {} };
来源：http://uqk.316326.xyz

[S43] C++：智能指针
来源：http://szk.zhongyouzk.top

auto p = std::make_unique<int>(5);
来源：http://pqs.tanke756.top

[S44] C++：引用传参
来源：http://fsc.hammf.cn

void inc(int &x) { ++x; }
来源：http://hbg.hywenlv.cn

[S45] C++：lambda
来源：http://xag.guowangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://bqd.hongshengwenyu.top

[S46] C++：函数模板
来源：http://qpm.hfpthk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://grl.vehdjk.com

[S47] C++：结构化绑定遍历
来源：http://mcy.feifeiyinyue.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ayk.52xcode.cn

[S48] C++：逐行读文件
来源：http://cyp.jinghuilouyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nad.snrcjt.cn

while (std::getline(in, line)) { }
来源：http://ltg.hesvh.cn

[S49] C++：写文件
来源：http://enx.fanxiaobao.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rxs.nwbrower.top

[S50] C++：格式化数字
来源：http://rfv.quarkkingdee.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dlu.hywenlv.cn

[S51] C++：显式类型转换
来源：http://ihg.c1oappe.top

static_cast<double>(a) / b
来源：http://yrn.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://rcn.cqqwz.cn

int size() const noexcept { return n_; }
来源：http://jcz.xuetiantiany.cn

[S53] C++：移动语义
来源：http://ben.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://ykk.nwbrower.top

[S54] C++：异常处理
来源：http://bqh.yanxiufei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://osu.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://yvk.yuanzhike.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bdk.jinghuilouyu.cn

[S56] C++：optional
来源：http://qdn.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rcl.svipenyu.cn

[S57] C++：编译期常量
来源：http://dcn.tanke756.top

constexpr int N = 10;
来源：http://ale.yueranfly.top

[S58] C++：命名空间
来源：http://zym.jianghu66.top

namespace ns { int f() { return 1; } }
来源：http://msv.fzhhl.top

[S59] C++：静态断言
来源：http://gts.chenjidiqi.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wye.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://rzl.meibo888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cnz.epnwcf.com

================================================================================
来源：http://boh.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ebs.yuanzhike.top

================================================================================
来源：http://ibw.ybcxt.top


<!-- 参考信息 -->