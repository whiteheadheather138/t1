代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ttw.zycfv.cn

[Q90] 生成序号列
来源：http://rft.sjlbkw.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hhk.pengpengdd.cyou

================================================================================
来源：http://uwe.wangshuangyany.cn

R. Bash 专题
来源：http://zrz.jlsjyb.cn

================================================================================
来源：http://qoo.ppjwa.cn

[R01] shebang 与严格模式
来源：http://fdh.yongpay.top

#!/usr/bin/env bash
来源：http://fay.zhaomingkeji.xyz

set -euo pipefail
来源：http://zys.smart0.xyz

[R02] 变量赋值与使用
来源：http://grs.gzhubu.top

name="Tom"; echo "$name"
来源：http://aya.smart0.xyz

[R03] 只读变量
来源：http://knf.shuidangran.top

readonly PI=3.14
来源：http://csp.gzhubu.top

[R04] 位置参数
来源：http://kum.cqqwz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jgb.shuidangran.top

[R05] 参数默认值
来源：http://jqu.shanyushiyangkeji.top

name="${1:-default}"
来源：http://uvz.cashguo.top

[R06] 判断命令是否存在
来源：http://eaw.nanxuanxn.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gme.sxryk.cn

[R07] if 判断文件
来源：http://oig.redwolf501.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zup.hcnkem.com

[R08] 数值比较
来源：http://hla.ctjpmb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://fva.tianlin.xyz

[R09] 字符串比较
来源：http://vdp.wangshuangyany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tpd.guowangkeji.top

[R10] 正则匹配
来源：http://yte.sxryk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mnw.sxryk.cn

[R11] case 多分支
来源：http://fnb.guannengcc.top

case "$1" in
来源：http://ofv.uphjek.com

start) echo "启动" ;;
来源：http://hus.guannengcc.top

stop)  echo "停止" ;;
来源：http://wxb.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://rqt.fzhhl.top

esac
来源：http://drt.andypj.xyz

[R12] for 遍历文件
来源：http://eck.gzhubu.top

for f in *.txt; do echo "$f"; done
来源：http://lfi.9152youxi.cn

[R13] for 计数循环
来源：http://fpl.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://zbw.fktsv.cn

[R14] C 风格 for
来源：http://lps.zhengqikj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jnz.cucudq.cn

[R15] while 逐行读文件
来源：http://uhs.vqdsnc.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bdq.xylfe.cn

[R16] until 等待条件
来源：http://miy.ydzc1.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wlu.chenzaomai.com

[R17] 数组定义与取值
来源：http://odu.haohaochexian.top

arr=(a b c); echo "${arr[0]}"
来源：http://ekc.cashguo.top

[R18] 遍历数组
来源：http://bnz.tianlin.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tbx.shanyushiyangtech.top

[R19] 数组长度
来源：http://fxc.zhixingplan.top

echo "${#arr[@]}"
来源：http://xmo.cheryme.top

[R20] 关联数组（字典）
来源：http://iyi.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vrt.jinqigfzy.top

[R21] 字符串长度
来源：http://egf.hfpthk.cn

echo "${#s}"
来源：http://aan.xziqi.cn

[R22] 截取子串
来源：http://cxi.jinqigufen.top

echo "${s:0:5}"
来源：http://ykp.gaohongyu789.top

[R23] 字符串替换
来源：http://nay.yangfankeji.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sjm.zdbjq.cn

[R24] 大小写转换
来源：http://wlm.havefunace.top

echo "${s^^}"; echo "${s,,}"
来源：http://glo.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://aft.nanxuanxn.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://htt.sweek.top

[R26] 命令替换
来源：http://lvp.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://ope.redwolf501.top

[R27] 算术展开
来源：http://swv.uphjek.com

echo $((1 + 2 * 3))
来源：http://clc.dianchejie.cn

[R28] 浮点运算
来源：http://xup.xingfuxueyuan.xyz

echo "scale=2; 10/3" | bc
来源：http://fyq.smart0.xyz

[R29] 定义函数
来源：http://bzg.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rhd.ehwqpu.com

[R30] 函数返回状态码
来源：http://rhn.xuetiantiany.cn

f() { return 0; }; f || echo "失败了"
来源：http://ksa.daxiang520.top

[R31] 局部变量
来源：http://ebi.hammf.cn

f() { local x=1; echo "$x"; }
来源：http://lhs.quarkkingdee.top

[R32] 参数个数校验
来源：http://yog.guowangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://obq.yongpay.top

[R33] 捕获错误并提示行号
来源：http://gjj.vqdsnc.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eij.birdmap.top

[R34] 退出时清理
来源：http://buf.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://clw.shuidangran.top

[R35] 后台执行并等待
来源：http://ern.iojbl.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qvc.ivvv.top

[R36] 并发执行多个任务
来源：http://xij.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zlw.9152youxi.cn

[R37] 把输出赋给变量
来源：http://dkq.0kj1m.cn

files=$(ls -1)
来源：http://wik.guowangkeji.top

[R38] 管道串联
来源：http://lfu.jlsjyb.cn

cat a.txt | grep -i error | wc -l
来源：http://yzd.wangshuangyany.cn

[R39] 重定向标准输出与错误
来源：http://bzx.ppjwa.cn

cmd > out.log 2>&1
来源：http://wse.gogol.net.cn

[R40] 追加写日志
来源：http://wzp.ywan-chungtsiang.top

echo "log" >> out.log
来源：http://qml.yj20258.top

[R41] 丢弃输出
来源：http://dzf.ivvv.top

cmd >/dev/null 2>&1
来源：http://tip.svipenyu.cn

[R42] 输入重定向
来源：http://jtd.shangyingyoupin.top

wc -l < a.txt
来源：http://glg.feifeiyinyue.top

[R43] 按名字查找文件
来源：http://ypo.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://vmb.sweek.top

[R44] 按修改时间查找
来源：http://bgd.uphjek.com

find . -mtime -7 -type f
来源：http://kqf.mhx1999.top

[R45] 批量删除
来源：http://yns.zhiwuduotai.top

find . -name "*.tmp" -delete
来源：http://uxm.ybcxt.top

[R46] 递归替换文件内容
来源：http://byh.sysykeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ttt.cqqwz.cn

[R47] sed 单行替换
来源：http://soi.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://qxd.dashuyun.cn

[R48] awk 取指定列
来源：http://eqv.iojbl.cn

awk '{print $1, $3}' a.txt
来源：http://ixi.jiagoushi.top

[R49] awk 带条件
来源：http://myt.hysaishi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ags.birdmap.top

[R50] awk 求和
来源：http://dmh.yj20258.top

awk '{s += $2} END {print s}' a.txt
来源：http://sqg.jinghuilouyu.cn

[R51] 排序去重取前几
来源：http://cnz.cashguo.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wqd.jqgfzy.top

[R52] 统计行数
来源：http://hot.bjfxy.top

wc -l a.txt
来源：http://jtz.ydjk.org.cn

[R53] 查看文件头与实时尾
来源：http://uxq.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qye.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://fup.sufxvd.cn

diff a.txt b.txt
来源：http://wgg.jlsjyb.cn

[R55] 压缩与解压
来源：http://ppe.yj20258888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://thf.guowangkeji.top

[R56] 远程拷贝
来源：http://arx.yuxming.cn

scp file user@host:/path/
来源：http://mhh.xuanzx.com

[R57] 远程执行命令
来源：http://erw.yonumen.top

ssh user@host 'uptime'
来源：http://mfl.sxryk.cn

[R58] 下载文件
来源：http://nmc.smart0.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uwy.daria6918.cn

[R59] 发 POST JSON
来源：http://qnq.shanyushiyangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ejo.yangfankeji.com

[R60] 只看 HTTP 状态码
来源：http://knb.c1oappe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fua.shuidangran.top

[R61] 磁盘占用
来源：http://ntr.c1oappe.top

df -h;  du -sh *
来源：http://pjj.guowangkeji.top

[R62] 找最占空间的文件
来源：http://yvd.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://ghm.zhiwuduotai.top

[R63] 内存与进程
来源：http://wnw.gotoacloud.top

free -h;  ps aux | grep nginx
来源：http://jxt.zdbjq.cn

[R64] 结束进程
来源：http://pkh.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://itp.yj20258.top

[R65] 查看端口占用
来源：http://nrp.sysykeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lwx.yj20258888.top

[R66] 定时任务
来源：http://fak.hnxiangtu.top

crontab -e;  crontab -l
来源：http://rkc.shanyushiyangkeji.top

[R67] 生成随机十六进制串
来源：http://fgo.havefunace.top

openssl rand -hex 16
来源：http://kae.zhijiandao.cn

[R68] 计算文件校验值
来源：http://wvj.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://aoj.nanxinkj.top

[R69] 生成随机密码
来源：http://cpk.redwolf501.top

head -c 16 /dev/urandom | base64
来源：http://aoz.dashuyun.cn

[R70] 时间戳与互转
来源：http://ugm.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://xji.hywenlv.cn

[R71] 日期格式化
来源：http://kxl.yangfankeji.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://esv.mhx1999.top

[R72] 等待端口就绪
来源：http://yfk.yongpay.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nch.quarkkingdee.top

[R73] 分割大日志
来源：http://vmi.fehbvm.com

split -l 1000 big.log part_
来源：http://vch.uphjek.com

[R74] 批量重命名
来源：http://kmt.svipenyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fhc.vqdsnc.cn

[R75] 导出环境变量
来源：http://umq.shanyushiyangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://pun.wangdashe.top

[R76] 使用临时文件
来源：http://whm.ppjwa.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uiz.vqdsnc.cn

[R77] 读取用户输入
来源：http://shr.mhx1999.top

read -rp "请输入: " ans
来源：http://wlu.zhongyouzk.top

[R78] 交互式菜单
来源：http://nlr.haohaochexian.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bnc.sjlbkw.cn

[R79] 解析命令行选项
来源：http://zqo.0kj1m.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tlk.gotoacloud.top

[R80] 查看脚本执行耗时
来源：http://wzd.jianghu66.top

time ./run.sh
来源：http://zzt.zhiwuduotai.top

================================================================================
来源：http://chs.wangshuangyany.cn

S. C / C++ 专题
来源：http://yuk.meibo888.top

================================================================================
来源：http://uyi.fzhhl.top

[S01] C：Hello World
来源：http://ylg.redwolf501.top

#include <stdio.h>
来源：http://zlr.bbcook.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://chc.redwolf501.top

[S02] C：变量与格式化输出
来源：http://cgp.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://qwe.fanxiaobao.xyz

[S03] C：读入整数
来源：http://evw.nanxuanxn.top

int x; scanf("%d", &x);
来源：http://yws.zhoulong.xyz

[S04] C：字符串复制
来源：http://icw.yuanzhike.top

char dst[32]; strcpy(dst, "hi");
来源：http://vme.bbcook.cn

[S05] C：字符串长度
来源：http://kyb.nanxinkj.top

strlen(s)
来源：http://dmj.guowangkeji.top

[S06] C：字符串比较
来源：http://ogw.redwolf501.top

strcmp(a, b) == 0
来源：http://odv.andypj.xyz

[S07] C：数组遍历求和
来源：http://qaf.ydzc1.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gsf.xuetiantiany.cn

[S08] C：动态内存分配与释放
来源：http://zxx.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pdt.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://llc.andypj.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qjw.tian-w.cn

[S10] C：指针与解引用
来源：http://oso.gzhubu.top

int *p = &a;  *p = 5;
来源：http://bqf.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://zxb.bbcook.cn

FILE *f = fopen("a.txt", "r");
来源：http://cbg.cucudq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ghk.yanxiufei.cn

fclose(f);
来源：http://brq.nanxuanxn.top

[S12] C：写文件
来源：http://cfx.andypj.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://orw.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://slt.tian-w.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://thn.wangdashe.top

[S14] C：枚举
来源：http://mtx.shuidangran.top

enum Color { RED, GREEN, BLUE };
来源：http://cjg.jinqigufen.top

[S15] C：类型转换
来源：http://jey.shanyushiyangtech.top

(double) a / b
来源：http://pfc.haohaochexian.top

[S16] C：位操作置位
来源：http://pfl.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://pvs.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://vot.sweek.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mfm.shangyingyoupin.top

[S18] C：命令行参数
来源：http://smh.hnqzz.top

int main(int argc, char **argv)
来源：http://hng.tianlin.xyz

[S19] C：快速排序
来源：http://oac.zhijiandao.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zgc.mhx1999.top

[S20] C：二分查找
来源：http://gtp.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iqy.fehbvm.com

[S21] C：字符类别判断
来源：http://eht.0kj1m.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://woo.shzxlz.cn

[S22] C：字符串转数字
来源：http://fmx.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://ycc.chenjidiqi.icu

[S23] C：随机数
来源：http://pix.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zdi.jyoumei.cn

[S24] C：获取本地时间
来源：http://ixl.zhaomingkeji.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lda.wangdashe.top

[S25] C：内存拷贝
来源：http://wjh.meibo888.top

memcpy(dst, src, n);
来源：http://xsg.xuanzx.com

[S26] C：内存清零
来源：http://hts.fktsv.cn

memset(a, 0, sizeof a);
来源：http://zqs.fengsongda.top

[S27] C：定义常量
来源：http://bzl.jqgufenzy.top

const double PI = 3.14159;
来源：http://gme.jyoumei.cn

[S28] C：静态变量
来源：http://qpe.yueranfly.top

static int counter = 0;
来源：http://vvu.havefunace.top

[S29] C：变参函数
来源：http://iqd.smart0.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ien.zhongyouzk.top

[S30] C：头文件保护
来源：http://icu.jqgfzy.top

#ifndef X_H
来源：http://xnd.daria6918.cn

#define X_H
来源：http://uur.316326.xyz

#endif
来源：http://idn.shuidangran.top

[S31] C++：Hello World
来源：http://gvq.fanxiaobao.xyz

#include <iostream>
来源：http://mil.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://kru.hnxiangtu.top

[S32] C++：字符串
来源：http://gde.cheryme.top

std::string s = "hi";  s += "!";
来源：http://oss.shanyushiyangtech.top

[S33] C++：vector 增删
来源：http://ygc.316326.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pzo.epnwcf.com

[S34] C++：遍历 vector
来源：http://rup.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://ccs.nwbrower.top

[S35] C++：map
来源：http://ypx.yuanzhike.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qxy.316326.xyz

[S36] C++：unordered_map
来源：http://hnb.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gng.feifeiyinyue.top

[S37] C++：set
来源：http://lio.sufxvd.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mbq.sjlbkw.cn

[S38] C++：排序
来源：http://qtm.yj20258.top

std::sort(v.begin(), v.end());
来源：http://xae.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://ayd.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kdv.yanxiufei.cn

[S40] C++：查找元素
来源：http://wxz.316326.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rmc.zdqjudy.top

[S41] C++：类与构造函数
来源：http://dnk.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bsx.0kj1m.cn

[S42] C++：继承与虚函数
来源：http://rbz.jinghuilouyu.cn

class B : public Base { public: void f() override {} };
来源：http://qdf.316326.xyz

[S43] C++：智能指针
来源：http://vlc.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://cze.vqdsnc.cn

[S44] C++：引用传参
来源：http://sgy.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://ktc.zdbjq.cn

[S45] C++：lambda
来源：http://uog.bbcook.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kts.tarul.cn

[S46] C++：函数模板
来源：http://utq.vqdsnc.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oox.jlsjyb.cn

[S47] C++：结构化绑定遍历
来源：http://nkb.chenjidiqi.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gxx.guowangkeji.top

[S48] C++：逐行读文件
来源：http://wcc.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://exp.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://wah.cdnleiting.top

[S49] C++：写文件
来源：http://jsk.zhongyouzk.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qir.shzxlz.cn

[S50] C++：格式化数字
来源：http://nmp.ybcxt.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fzg.nwbrower.top

[S51] C++：显式类型转换
来源：http://iaz.yuanzhike.top

static_cast<double>(a) / b
来源：http://hnl.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://aft.jqgfzy.top

int size() const noexcept { return n_; }
来源：http://gap.fehbvm.com

[S53] C++：移动语义
来源：http://osu.xingfuxueyuan.xyz

std::vector<int> w = std::move(v);
来源：http://ynh.chenlongwang.top

[S54] C++：异常处理
来源：http://wlt.fanxiaobao.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://flr.52xcode.cn

[S55] C++：结构化绑定
来源：http://ncp.daxiang520.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lfu.zhaomingkeji.xyz

[S56] C++：optional
来源：http://fbb.vehdjk.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://toh.cdnleiting.top

[S57] C++：编译期常量
来源：http://hcm.xylfe.cn

constexpr int N = 10;
来源：http://zfa.ctjpmb.com

[S58] C++：命名空间
来源：http://qup.zdqjudy.top

namespace ns { int f() { return 1; } }
来源：http://fdi.pycfn.com

[S59] C++：静态断言
来源：http://ork.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ubj.ybcxt.top

[S60] C++：遍历并删除元素
来源：http://roq.yanxiufei.cn


<!-- 参考信息 -->