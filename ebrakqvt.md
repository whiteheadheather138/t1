代发 wailian999

R. Bash 专题
来源：http://zad.vqdsnc.cn

================================================================================
来源：http://rtd.c1oappe.top

[R01] shebang 与严格模式
来源：http://iag.tarul.cn

#!/usr/bin/env bash
来源：http://vqh.bbcook.cn

set -euo pipefail
来源：http://wev.sxryk.cn

[R02] 变量赋值与使用
来源：http://jbf.yuxming.cn

name="Tom"; echo "$name"
来源：http://fog.cdnleiting.top

[R03] 只读变量
来源：http://mxt.zhengqikj.top

readonly PI=3.14
来源：http://jbx.iojbl.cn

[R04] 位置参数
来源：http://ogh.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iji.jiagoushi.top

[R05] 参数默认值
来源：http://bed.yonumen.top

name="${1:-default}"
来源：http://jkx.iojbl.cn

[R06] 判断命令是否存在
来源：http://fkp.zhengqikj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sax.xingfuxueyuan.xyz

[R07] if 判断文件
来源：http://jni.yj20258888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ljs.snrcjt.cn

[R08] 数值比较
来源：http://cwh.sweek.top

if (( a > b )); then echo "a 更大"; fi
来源：http://clt.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://azn.haohaochexian.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://alr.birdmap.top

[R10] 正则匹配
来源：http://eod.yueranfly.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zpg.jinyuanbaomall.cn

[R11] case 多分支
来源：http://tvd.jqgfzy.top

case "$1" in
来源：http://cpx.meibo888.top

start) echo "启动" ;;
来源：http://ucl.sysykeji.top

stop)  echo "停止" ;;
来源：http://die.52xcode.cn

*)     echo "未知命令" ;;
来源：http://tnr.chenlongwang.top

esac
来源：http://gpk.wangdashe.top

[R12] for 遍历文件
来源：http://okp.jinqigufen.top

for f in *.txt; do echo "$f"; done
来源：http://zgu.nwbrower.top

[R13] for 计数循环
来源：http://yum.sweek.top

for i in {1..10}; do echo "$i"; done
来源：http://czy.fanxiaobao.xyz

[R14] C 风格 for
来源：http://htk.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dqx.sysykeji.top

[R15] while 逐行读文件
来源：http://osr.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nsz.hammf.cn

[R16] until 等待条件
来源：http://wbq.jlsjyb.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://soy.sufxvd.cn

[R17] 数组定义与取值
来源：http://ati.zycfv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kck.fzhhl.top

[R18] 遍历数组
来源：http://veo.zycfv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wiv.ehwqpu.com

[R19] 数组长度
来源：http://jlw.ctjpmb.com

echo "${#arr[@]}"
来源：http://pon.nanxinkj.top

[R20] 关联数组（字典）
来源：http://knf.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nsp.chenlongwang.top

[R21] 字符串长度
来源：http://byx.jinghuilouyu.cn

echo "${#s}"
来源：http://wcd.9152youxi.cn

[R22] 截取子串
来源：http://zdr.hywenlv.cn

echo "${s:0:5}"
来源：http://dpy.haohaochexian.top

[R23] 字符串替换
来源：http://mmy.shangyingyoupin.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qcn.nanxuanxn.top

[R24] 大小写转换
来源：http://eju.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://asb.ivvv.top

[R25] 去后缀 / 去前缀
来源：http://kzc.xinyue.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://jbp.nwbrower.top

[R26] 命令替换
来源：http://avv.nanxuanxn.top

now=$(date +%F); echo "$now"
来源：http://umq.bjfxy.top

[R27] 算术展开
来源：http://fct.smart0.xyz

echo $((1 + 2 * 3))
来源：http://gbn.jinyuanbaomall.cn

[R28] 浮点运算
来源：http://xhz.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://ics.zhaomingkeji.xyz

[R29] 定义函数
来源：http://jij.xuanzx.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sfx.shzxlz.cn

[R30] 函数返回状态码
来源：http://nep.yongpay.top

f() { return 0; }; f || echo "失败了"
来源：http://pls.havefunace.top

[R31] 局部变量
来源：http://rgm.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://lnc.sufxvd.cn

[R32] 参数个数校验
来源：http://yvi.ehwqpu.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://npo.zhiwuduotai.top

[R33] 捕获错误并提示行号
来源：http://yfn.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://upm.yj20258888.top

[R34] 退出时清理
来源：http://sck.zycfv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mav.xuanzx.com

[R35] 后台执行并等待
来源：http://uae.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ice.fzhhl.top

[R36] 并发执行多个任务
来源：http://clf.c1oappe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dpv.pycfn.com

[R37] 把输出赋给变量
来源：http://sjj.jyoumei.cn

files=$(ls -1)
来源：http://wla.jinyuanbaomall.cn

[R38] 管道串联
来源：http://vdb.feifeiyinyue.top

cat a.txt | grep -i error | wc -l
来源：http://zsy.chenzaomai.com

[R39] 重定向标准输出与错误
来源：http://pse.guowangkeji.top

cmd > out.log 2>&1
来源：http://gjl.bjfxy.top

[R40] 追加写日志
来源：http://tfx.fzhhl.top

echo "log" >> out.log
来源：http://gfk.fzhhl.top

[R41] 丢弃输出
来源：http://htu.uphjek.com

cmd >/dev/null 2>&1
来源：http://uda.hywenlv.cn

[R42] 输入重定向
来源：http://vlw.ivvv.top

wc -l < a.txt
来源：http://coz.snrcjt.cn

[R43] 按名字查找文件
来源：http://cgt.zhiwuduotai.top

find . -name "*.log" -type f
来源：http://ugq.gogol.net.cn

[R44] 按修改时间查找
来源：http://poo.sjlbkw.cn

find . -mtime -7 -type f
来源：http://grb.kuanghao11.cn

[R45] 批量删除
来源：http://lvq.sjlbkw.cn

find . -name "*.tmp" -delete
来源：http://htj.shzxlz.cn

[R46] 递归替换文件内容
来源：http://hce.hongshengwenyu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yxv.yangfankeji.com

[R47] sed 单行替换
来源：http://dqs.jyoumei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ies.birdmap.top

[R48] awk 取指定列
来源：http://lqr.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://beq.0kj1m.cn

[R49] awk 带条件
来源：http://vka.cdnleiting.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aae.daxiang520.top

[R50] awk 求和
来源：http://rnd.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://dnn.aizwys.cn

[R51] 排序去重取前几
来源：http://eyu.yueranfly.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dsk.hnxiangtu.top

[R52] 统计行数
来源：http://opg.yj202588.top

wc -l a.txt
来源：http://byy.yonumen.top

[R53] 查看文件头与实时尾
来源：http://psg.nanxuanxn.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rev.zdbjq.cn

[R54] 比较两个文件
来源：http://sud.chenzaomai.com

diff a.txt b.txt
来源：http://luy.shanyushiyangtech.top

[R55] 压缩与解压
来源：http://hma.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gym.hongshengwenyu.top

[R56] 远程拷贝
来源：http://lvm.fzhhl.top

scp file user@host:/path/
来源：http://ttb.xuetiantiany.cn

[R57] 远程执行命令
来源：http://ugz.9152youxi.cn

ssh user@host 'uptime'
来源：http://wge.sweek.top

[R58] 下载文件
来源：http://acz.shanyushiyangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aef.yj20258888.top

[R59] 发 POST JSON
来源：http://xnh.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://njf.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://qlk.jqgufenzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nrj.xylfe.cn

[R61] 磁盘占用
来源：http://kbs.fanxiaobao.xyz

df -h;  du -sh *
来源：http://pke.nwbrower.top

[R62] 找最占空间的文件
来源：http://ctm.vqdsnc.cn

du -ah . | sort -rh | head -10
来源：http://obq.wangshuangyany.cn

[R63] 内存与进程
来源：http://mms.jiagoushi.top

free -h;  ps aux | grep nginx
来源：http://dnm.xylfe.cn

[R64] 结束进程
来源：http://mny.316326.xyz

kill -9 $(pgrep -f app.py)
来源：http://uxd.shzxlz.cn

[R65] 查看端口占用
来源：http://tfj.svipenyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://owg.yangfankeji.com

[R66] 定时任务
来源：http://tnl.hesvh.cn

crontab -e;  crontab -l
来源：http://gfl.fengsongda.top

[R67] 生成随机十六进制串
来源：http://rwz.sxryk.cn

openssl rand -hex 16
来源：http://dvt.0kj1m.cn

[R68] 计算文件校验值
来源：http://gzx.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vvg.ctjpmb.com

[R69] 生成随机密码
来源：http://oly.ydjk.org.cn

head -c 16 /dev/urandom | base64
来源：http://mbp.cucudq.cn

[R70] 时间戳与互转
来源：http://yla.shanyushiyangtech.top

date +%s;  date -d @1700000000
来源：http://lmp.hesvh.cn

[R71] 日期格式化
来源：http://ifx.ydzc1.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://phf.redwolf501.top

[R72] 等待端口就绪
来源：http://qly.daria6918.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xdc.ppjwa.cn

[R73] 分割大日志
来源：http://fya.chenjidiqi.icu

split -l 1000 big.log part_
来源：http://rui.fehbvm.com

[R74] 批量重命名
来源：http://tsk.gaohongyu789.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oaa.zdqjudy.top

[R75] 导出环境变量
来源：http://wqp.shanyushiyangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://kve.shanyushiyangtech.top

[R76] 使用临时文件
来源：http://tzy.c1oappe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://htg.52xcode.cn

[R77] 读取用户输入
来源：http://cxm.nanxuanxn.top

read -rp "请输入: " ans
来源：http://yzg.sjlbkw.cn

[R78] 交互式菜单
来源：http://tjf.9152youxi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://njh.jqgufenzy.top

[R79] 解析命令行选项
来源：http://nei.zhaomingkeji.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qod.uphjek.com

[R80] 查看脚本执行耗时
来源：http://cet.zdbjq.cn

time ./run.sh
来源：http://sbq.nwbrower.top

================================================================================
来源：http://ifj.tian-w.cn

S. C / C++ 专题
来源：http://slz.feifeiyinyue.top

================================================================================
来源：http://ewt.vqdsnc.cn

[S01] C：Hello World
来源：http://mtw.sysykeji.top

#include <stdio.h>
来源：http://baw.bbcook.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://llz.shzxlz.cn

[S02] C：变量与格式化输出
来源：http://mwf.wangdashe.top

int a = 10; printf("%d\n", a);
来源：http://bhb.mhx1999.top

[S03] C：读入整数
来源：http://slw.jlsjyb.cn

int x; scanf("%d", &x);
来源：http://oyk.vqdsnc.cn

[S04] C：字符串复制
来源：http://lxy.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kae.nwbrower.top

[S05] C：字符串长度
来源：http://onq.zhijiandao.cn

strlen(s)
来源：http://dyt.yvedp.cn

[S06] C：字符串比较
来源：http://kmg.bjfxy.top

strcmp(a, b) == 0
来源：http://miq.hcnkem.com

[S07] C：数组遍历求和
来源：http://jyn.zhijiandao.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://enn.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://lko.shanyushiyangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zqv.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://rfd.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cbl.kuanghao11.cn

[S10] C：指针与解引用
来源：http://yhy.daria6918.cn

int *p = &a;  *p = 5;
来源：http://ogp.jlsjyb.cn

[S11] C：逐行读文件
来源：http://mqw.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://lqq.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ijd.tanke756.top

fclose(f);
来源：http://hfk.sxryk.cn

[S12] C：写文件
来源：http://nsp.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zxf.yanxiufei.cn

[S13] C：宏定义
来源：http://ied.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kbu.9152youxi.cn

[S14] C：枚举
来源：http://ttq.jqgfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://tpy.jinqigufen.top

[S15] C：类型转换
来源：http://gud.bbcook.cn

(double) a / b
来源：http://jzk.kuanghao11.cn

[S16] C：位操作置位
来源：http://eqj.c1oappe.top

x |= (1 << 3);
来源：http://tqu.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://ilx.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://thz.sufxvd.cn

[S18] C：命令行参数
来源：http://qjp.pengpengdd.cyou

int main(int argc, char **argv)
来源：http://njp.xinyue.icu

[S19] C：快速排序
来源：http://glr.fengsongda.top

qsort(a, n, sizeof(int), cmp);
来源：http://bww.sjlbkw.cn

[S20] C：二分查找
来源：http://gtv.birdmap.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tty.xziqi.cn

[S21] C：字符类别判断
来源：http://oaj.jinqigfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jue.yuxming.cn

[S22] C：字符串转数字
来源：http://qsl.hnxiangtu.top

atoi("42");  strtod("3.14", NULL);
来源：http://swp.yj202588.top

[S23] C：随机数
来源：http://tfo.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qho.guowangkeji.top

[S24] C：获取本地时间
来源：http://fpr.zycfv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ysr.gogol.net.cn

[S25] C：内存拷贝
来源：http://wvj.chenjidiqi.icu

memcpy(dst, src, n);
来源：http://vot.yvedp.cn

[S26] C：内存清零
来源：http://rll.jqgfzy.top

memset(a, 0, sizeof a);
来源：http://sdp.vqdsnc.cn

[S27] C：定义常量
来源：http://fze.bjfxy.top

const double PI = 3.14159;
来源：http://rqx.ydzc1.top

[S28] C：静态变量
来源：http://jtn.tarul.cn

static int counter = 0;
来源：http://jaf.ivvv.top

[S29] C：变参函数
来源：http://kdi.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dks.andypj.xyz

[S30] C：头文件保护
来源：http://uqz.snrcjt.cn

#ifndef X_H
来源：http://mvr.dashuyun.cn

#define X_H
来源：http://kgs.xylfe.cn

#endif
来源：http://igj.shzxlz.cn

[S31] C++：Hello World
来源：http://ukp.quarkkingdee.top

#include <iostream>
来源：http://rfz.fktsv.cn

int main() { std::cout << "Hello\n"; }
来源：http://pwy.cdnleiting.top

[S32] C++：字符串
来源：http://mtx.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://wog.vqdsnc.cn

[S33] C++：vector 增删
来源：http://wte.bjfxy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://auz.aizwys.cn

[S34] C++：遍历 vector
来源：http://tnb.ydzc1.top

for (auto &x : v) { std::cout << x; }
来源：http://cxf.yj20258.top

[S35] C++：map
来源：http://was.yanxiufei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lbg.tarul.cn

[S36] C++：unordered_map
来源：http://hxx.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cpm.shangyingyoupin.top

[S37] C++：set
来源：http://mng.dianchejie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fdq.zhaomingkeji.xyz

[S38] C++：排序
来源：http://wrs.ydjk.org.cn

std::sort(v.begin(), v.end());
来源：http://wct.jlsjyb.cn

[S39] C++：自定义比较器排序
来源：http://txr.bbcook.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kvu.hnqzz.top

[S40] C++：查找元素
来源：http://pgg.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nib.daria6918.cn

[S41] C++：类与构造函数
来源：http://osf.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iwd.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://lcn.jiagoushi.top

class B : public Base { public: void f() override {} };
来源：http://itq.shzxlz.cn

[S43] C++：智能指针
来源：http://knu.xuetiantiany.cn

auto p = std::make_unique<int>(5);
来源：http://hjo.zhengqikj.top

[S44] C++：引用传参
来源：http://atp.jinyuanbaomall.cn

void inc(int &x) { ++x; }
来源：http://gln.sweek.top

[S45] C++：lambda
来源：http://qpo.mhx1999.top

auto add = [](int a, int b) { return a + b; };
来源：http://dgt.hnxiangtu.top

[S46] C++：函数模板
来源：http://yxb.sxryk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lph.tanke756.top

[S47] C++：结构化绑定遍历
来源：http://ayv.tian-w.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://boh.hnxiangtu.top

[S48] C++：逐行读文件
来源：http://bgh.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://iwl.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://jim.xuetiantiany.cn

[S49] C++：写文件
来源：http://omz.sxryk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ois.nanxinkj.top

[S50] C++：格式化数字
来源：http://nbc.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xhr.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://ohm.smart0.xyz

static_cast<double>(a) / b
来源：http://oyf.uphjek.com

[S52] C++：const 与 noexcept
来源：http://dyk.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://aqy.pycfn.com

[S53] C++：移动语义
来源：http://qug.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://wib.yuanzhike.top

[S54] C++：异常处理
来源：http://qqn.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lhv.cucudq.cn

[S55] C++：结构化绑定
来源：http://skd.jqgfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://edc.ydzc1.top

[S56] C++：optional
来源：http://mae.jlsjyb.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ptg.birdmap.top

[S57] C++：编译期常量
来源：http://sdx.redwolf501.top

constexpr int N = 10;
来源：http://poo.dashuyun.cn

[S58] C++：命名空间
来源：http://lsu.zhongyouzk.top

namespace ns { int f() { return 1; } }
来源：http://wag.xuetiantiany.cn

[S59] C++：静态断言
来源：http://qqi.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wqu.ydzc1.top

[S60] C++：遍历并删除元素
来源：http://wqe.52xcode.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ehw.jiagoushi.top

================================================================================
来源：http://xsw.shzxlz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qpj.xinyue.icu

================================================================================
来源：http://loe.ydzc1.top


<!-- 参考信息 -->