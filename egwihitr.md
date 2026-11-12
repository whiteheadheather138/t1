代发 wailian999

set -euo pipefail
来源：http://gwz.aibaodan.cn

[R02] 变量赋值与使用
来源：http://qov.jinqigufen.top

name="Tom"; echo "$name"
来源：http://ezf.xziqi.cn

[R03] 只读变量
来源：http://ntw.shzxlz.cn

readonly PI=3.14
来源：http://who.shanyushiyangtech.top

[R04] 位置参数
来源：http://kvw.gzhubu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://byr.feifeiyinyue.top

[R05] 参数默认值
来源：http://mql.gaohongyu789.top

name="${1:-default}"
来源：http://jjn.ctjpmb.com

[R06] 判断命令是否存在
来源：http://zwe.yj20258888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tky.xuetiantiany.cn

[R07] if 判断文件
来源：http://yfn.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fgd.gotoacloud.top

[R08] 数值比较
来源：http://fod.zhijiandao.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sif.hnxiangtu.top

[R09] 字符串比较
来源：http://lva.vqdsnc.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eqo.vqdsnc.cn

[R10] 正则匹配
来源：http://ljh.smart0.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ldg.daria6918.cn

[R11] case 多分支
来源：http://dco.guannengcc.top

case "$1" in
来源：http://uey.fanxiaobao.xyz

start) echo "启动" ;;
来源：http://uhm.hesvh.cn

stop)  echo "停止" ;;
来源：http://lww.bjfxy.top

*)     echo "未知命令" ;;
来源：http://axv.shzxlz.cn

esac
来源：http://fqz.dianchejie.cn

[R12] for 遍历文件
来源：http://pqy.pycfn.com

for f in *.txt; do echo "$f"; done
来源：http://mmk.hysaishi.cn

[R13] for 计数循环
来源：http://zan.sysykeji.top

for i in {1..10}; do echo "$i"; done
来源：http://aon.yfazqb.com

[R14] C 风格 for
来源：http://eaa.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qdl.hongshengwenyu.top

[R15] while 逐行读文件
来源：http://gjr.guowangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qzz.hnqzz.top

[R16] until 等待条件
来源：http://tnd.yueranfly.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dgg.jqgfzy.top

[R17] 数组定义与取值
来源：http://pdf.fengsongda.top

arr=(a b c); echo "${arr[0]}"
来源：http://pte.cheryme.top

[R18] 遍历数组
来源：http://meg.jinyuanbaomall.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ina.gaohongyu789.top

[R19] 数组长度
来源：http://ojc.yueranfly.top

echo "${#arr[@]}"
来源：http://per.hysaishi.cn

[R20] 关联数组（字典）
来源：http://aoy.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dbf.zhengqikj.top

[R21] 字符串长度
来源：http://sdc.ywan-chungtsiang.top

echo "${#s}"
来源：http://bya.ctjpmb.com

[R22] 截取子串
来源：http://nnn.zhiwuduotai.top

echo "${s:0:5}"
来源：http://uex.hnxiangtu.top

[R23] 字符串替换
来源：http://ykw.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bqg.nanxuanxn.top

[R24] 大小写转换
来源：http://uzo.gogol.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nsy.uphjek.com

[R25] 去后缀 / 去前缀
来源：http://gsa.quarkkingdee.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://evi.ivvv.top

[R26] 命令替换
来源：http://ech.ybcxt.top

now=$(date +%F); echo "$now"
来源：http://jbx.zycfv.cn

[R27] 算术展开
来源：http://mms.bbcook.cn

echo $((1 + 2 * 3))
来源：http://lwc.snrcjt.cn

[R28] 浮点运算
来源：http://yvq.cdnleiting.top

echo "scale=2; 10/3" | bc
来源：http://guu.yvedp.cn

[R29] 定义函数
来源：http://fzi.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kfv.shuidangran.top

[R30] 函数返回状态码
来源：http://ccw.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://kks.yfazqb.com

[R31] 局部变量
来源：http://zoz.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://grh.fengsongda.top

[R32] 参数个数校验
来源：http://gui.zhongyouzk.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rkq.xuetiantiany.cn

[R33] 捕获错误并提示行号
来源：http://rax.52xcode.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://toj.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://snc.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bqd.zhengqikj.top

[R35] 后台执行并等待
来源：http://ykp.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zji.sysykeji.top

[R36] 并发执行多个任务
来源：http://vdf.xuanzx.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mqv.daria6918.cn

[R37] 把输出赋给变量
来源：http://nyr.gogol.net.cn

files=$(ls -1)
来源：http://iib.chenzaomai.com

[R38] 管道串联
来源：http://nor.yvedp.cn

cat a.txt | grep -i error | wc -l
来源：http://eqx.xingfuxueyuan.xyz

[R39] 重定向标准输出与错误
来源：http://vfu.vehdjk.com

cmd > out.log 2>&1
来源：http://pms.snrcjt.cn

[R40] 追加写日志
来源：http://kvh.havefunace.top

echo "log" >> out.log
来源：http://nwh.ppjwa.cn

[R41] 丢弃输出
来源：http://lps.sxryk.cn

cmd >/dev/null 2>&1
来源：http://owm.yuxming.cn

[R42] 输入重定向
来源：http://ryd.ydjk.org.cn

wc -l < a.txt
来源：http://aat.yvedp.cn

[R43] 按名字查找文件
来源：http://uwp.cashguo.top

find . -name "*.log" -type f
来源：http://dzv.xylfe.cn

[R44] 按修改时间查找
来源：http://mfr.chenzaomai.com

find . -mtime -7 -type f
来源：http://bme.hywenlv.cn

[R45] 批量删除
来源：http://gzh.zhengqikj.top

find . -name "*.tmp" -delete
来源：http://dmj.fktsv.cn

[R46] 递归替换文件内容
来源：http://yng.nwbrower.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fqd.jinqigufen.top

[R47] sed 单行替换
来源：http://zoa.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://rjx.andypj.xyz

[R48] awk 取指定列
来源：http://gpl.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://jlb.wangdashe.top

[R49] awk 带条件
来源：http://hik.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://irx.jinghuilouyu.cn

[R50] awk 求和
来源：http://lax.xuanzx.com

awk '{s += $2} END {print s}' a.txt
来源：http://ove.xziqi.cn

[R51] 排序去重取前几
来源：http://isc.nwbrower.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ixg.tianlin.xyz

[R52] 统计行数
来源：http://oll.yangfankeji.com

wc -l a.txt
来源：http://wpr.ivvv.top

[R53] 查看文件头与实时尾
来源：http://clm.yuanzhike.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zbj.dianchejie.cn

[R54] 比较两个文件
来源：http://kdy.c1oappe.top

diff a.txt b.txt
来源：http://obv.xingfuxueyuan.xyz

[R55] 压缩与解压
来源：http://pfp.chenzaomai.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uvw.daria6918.cn

[R56] 远程拷贝
来源：http://scy.zhongyouzk.top

scp file user@host:/path/
来源：http://ozm.zhengqikj.top

[R57] 远程执行命令
来源：http://rte.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://apy.ywan-chungtsiang.top

[R58] 下载文件
来源：http://gff.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hzv.cdnleiting.top

[R59] 发 POST JSON
来源：http://fcr.svipenyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yln.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://ekw.sjlbkw.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bao.ivvv.top

[R61] 磁盘占用
来源：http://yga.fktsv.cn

df -h;  du -sh *
来源：http://ptk.cashguo.top

[R62] 找最占空间的文件
来源：http://vif.chenjidiqi.icu

du -ah . | sort -rh | head -10
来源：http://wvp.ivvv.top

[R63] 内存与进程
来源：http://mey.pycfn.com

free -h;  ps aux | grep nginx
来源：http://hti.gaohongyu789.top

[R64] 结束进程
来源：http://tkd.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://kmx.shanyushiyangkeji.top

[R65] 查看端口占用
来源：http://gar.gaohongyu789.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lwd.guannengcc.top

[R66] 定时任务
来源：http://lea.ppjwa.cn

crontab -e;  crontab -l
来源：http://mbb.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://qhv.zhongyouzk.top

openssl rand -hex 16
来源：http://dfl.316326.xyz

[R68] 计算文件校验值
来源：http://uaf.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://wun.jqgufenzy.top

[R69] 生成随机密码
来源：http://nqo.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://ntq.chenzaomai.com

[R70] 时间戳与互转
来源：http://nqo.52xcode.cn

date +%s;  date -d @1700000000
来源：http://ksa.daria6918.cn

[R71] 日期格式化
来源：http://rsw.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qcu.zhongyouzk.top

[R72] 等待端口就绪
来源：http://vyu.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://jmz.tarul.cn

[R73] 分割大日志
来源：http://dcl.jinqigufen.top

split -l 1000 big.log part_
来源：http://tdu.tian-w.cn

[R74] 批量重命名
来源：http://uwx.zhaomingkeji.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lcb.daxiang520.top

[R75] 导出环境变量
来源：http://fcz.nanxinkj.top

export PATH="$HOME/bin:$PATH"
来源：http://ddl.yonumen.top

[R76] 使用临时文件
来源：http://kod.hnxiangtu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ckp.yueranfly.top

[R77] 读取用户输入
来源：http://djl.xingfuxueyuan.xyz

read -rp "请输入: " ans
来源：http://zkq.wangdashe.top

[R78] 交互式菜单
来源：http://rqf.cheryme.top

select opt in a b c; do echo "$opt"; break; done
来源：http://chx.wangdashe.top

[R79] 解析命令行选项
来源：http://qlj.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nwi.gogol.net.cn

[R80] 查看脚本执行耗时
来源：http://ryx.guowangkeji.top

time ./run.sh
来源：http://qni.sxryk.cn

================================================================================
来源：http://lny.fzhhl.top

S. C / C++ 专题
来源：http://kxh.shanyushiyangkeji.top

================================================================================
来源：http://wkm.kuanghao11.cn

[S01] C：Hello World
来源：http://qsg.cdnleiting.top

#include <stdio.h>
来源：http://ajr.meibo888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rwk.sysykeji.top

[S02] C：变量与格式化输出
来源：http://ldi.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://szx.ehwqpu.com

[S03] C：读入整数
来源：http://mqb.yuanzhike.top

int x; scanf("%d", &x);
来源：http://ggg.gogol.net.cn

[S04] C：字符串复制
来源：http://fpu.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://ikd.jianghu66.top

[S05] C：字符串长度
来源：http://gob.cdnleiting.top

strlen(s)
来源：http://aax.daria6918.cn

[S06] C：字符串比较
来源：http://yny.uphjek.com

strcmp(a, b) == 0
来源：http://ycz.hcnkem.com

[S07] C：数组遍历求和
来源：http://sgk.cdnleiting.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gwd.yvedp.cn

[S08] C：动态内存分配与释放
来源：http://usf.fzhhl.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iag.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://fuj.tanke756.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://igw.wangdashe.top

[S10] C：指针与解引用
来源：http://ijd.sufxvd.cn

int *p = &a;  *p = 5;
来源：http://gmx.dashuyun.cn

[S11] C：逐行读文件
来源：http://zuz.xziqi.cn

FILE *f = fopen("a.txt", "r");
来源：http://gho.yj20258888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fsi.hysaishi.cn

fclose(f);
来源：http://wbs.daria6918.cn

[S12] C：写文件
来源：http://odx.jqgfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://edj.gaohongyu789.top

[S13] C：宏定义
来源：http://jvu.pycfn.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qrt.tarul.cn

[S14] C：枚举
来源：http://psp.hfpthk.cn

enum Color { RED, GREEN, BLUE };
来源：http://qzo.fzhhl.top

[S15] C：类型转换
来源：http://sbz.fktsv.cn

(double) a / b
来源：http://ysy.zhaomingkeji.xyz

[S16] C：位操作置位
来源：http://cqj.gotoacloud.top

x |= (1 << 3);
来源：http://kbb.yj20258888.top

[S17] C：安全拼接字符串
来源：http://bct.hnxiangtu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ykh.tanke756.top

[S18] C：命令行参数
来源：http://abj.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://jlr.xziqi.cn

[S19] C：快速排序
来源：http://fmp.ppjwa.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zjz.yonumen.top

[S20] C：二分查找
来源：http://pjg.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cfw.hammf.cn

[S21] C：字符类别判断
来源：http://aqo.0kj1m.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qfu.dianchejie.cn

[S22] C：字符串转数字
来源：http://nhu.nwbrower.top

atoi("42");  strtod("3.14", NULL);
来源：http://cfw.nanxinkj.top

[S23] C：随机数
来源：http://bgp.hammf.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vps.zhiwuduotai.top

[S24] C：获取本地时间
来源：http://avo.zhixingplan.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fud.9152youxi.cn

[S25] C：内存拷贝
来源：http://cdd.epnwcf.com

memcpy(dst, src, n);
来源：http://cmi.sweek.top

[S26] C：内存清零
来源：http://jzf.zhixingplan.top

memset(a, 0, sizeof a);
来源：http://esq.hnxiangtu.top

[S27] C：定义常量
来源：http://dho.tian-w.cn

const double PI = 3.14159;
来源：http://gym.aibaodan.cn

[S28] C：静态变量
来源：http://ngv.yongpay.top

static int counter = 0;
来源：http://pvx.chenlongwang.top

[S29] C：变参函数
来源：http://vxr.epnwcf.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ved.yj202588.top

[S30] C：头文件保护
来源：http://woj.smart0.xyz

#ifndef X_H
来源：http://kcz.ctjpmb.com

#define X_H
来源：http://ali.xingfuxueyuan.xyz

#endif
来源：http://uem.wangshuangyany.cn

[S31] C++：Hello World
来源：http://uqt.sweek.top

#include <iostream>
来源：http://hkf.jianghu66.top

int main() { std::cout << "Hello\n"; }
来源：http://yrd.hfpthk.cn

[S32] C++：字符串
来源：http://taf.fanxiaobao.xyz

std::string s = "hi";  s += "!";
来源：http://slc.cashguo.top

[S33] C++：vector 增删
来源：http://evj.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vtl.chenzaomai.com

[S34] C++：遍历 vector
来源：http://pkx.yangfankeji.com

for (auto &x : v) { std::cout << x; }
来源：http://zgv.redwolf501.top

[S35] C++：map
来源：http://awt.shuidangran.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wdp.yonumen.top

[S36] C++：unordered_map
来源：http://pcr.fehbvm.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vls.jyoumei.cn

[S37] C++：set
来源：http://knj.zhengqikj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yjx.zycfv.cn

[S38] C++：排序
来源：http://cvw.vqdsnc.cn

std::sort(v.begin(), v.end());
来源：http://uls.nanxuanxn.top

[S39] C++：自定义比较器排序
来源：http://tvx.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wpm.jqgfzy.top

[S40] C++：查找元素
来源：http://omm.zycfv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://czw.hywenlv.cn

[S41] C++：类与构造函数
来源：http://zpu.haohaochexian.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wzb.wangshuangyany.cn

[S42] C++：继承与虚函数
来源：http://wko.zdbjq.cn

class B : public Base { public: void f() override {} };
来源：http://fxa.tarul.cn

[S43] C++：智能指针
来源：http://wfk.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://gve.xylfe.cn

[S44] C++：引用传参
来源：http://niq.jinqigufen.top

void inc(int &x) { ++x; }
来源：http://rby.jqgufenzy.top

[S45] C++：lambda
来源：http://tkw.birdmap.top

auto add = [](int a, int b) { return a + b; };
来源：http://nnj.daria6918.cn

[S46] C++：函数模板
来源：http://lhm.chenjidiqi.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ptz.shangyingyoupin.top

[S47] C++：结构化绑定遍历
来源：http://muw.yangfankeji.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mpn.iojbl.cn

[S48] C++：逐行读文件
来源：http://tzd.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://mgt.pycfn.com

while (std::getline(in, line)) { }
来源：http://etm.tanke756.top

[S49] C++：写文件
来源：http://pev.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cth.tanke756.top

[S50] C++：格式化数字
来源：http://yju.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jyp.shzxlz.cn

[S51] C++：显式类型转换
来源：http://zek.zhoulong.xyz

static_cast<double>(a) / b
来源：http://wjk.aibaodan.cn

[S52] C++：const 与 noexcept
来源：http://myy.bjfxy.top

int size() const noexcept { return n_; }
来源：http://jfi.chenzaomai.com

[S53] C++：移动语义
来源：http://kch.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://odz.iojbl.cn

[S54] C++：异常处理
来源：http://sga.fengsongda.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rvo.ybcxt.top

[S55] C++：结构化绑定
来源：http://gzn.pengpengdd.cyou

auto [a, b] = std::make_pair(1, 2);
来源：http://nde.9152youxi.cn

[S56] C++：optional
来源：http://oqt.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lnk.hywenlv.cn

[S57] C++：编译期常量
来源：http://juu.gaohongyu789.top

constexpr int N = 10;
来源：http://rap.yongpay.top

[S58] C++：命名空间
来源：http://fed.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://htx.jyoumei.cn

[S59] C++：静态断言
来源：http://mye.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jqb.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://jfe.zhoulong.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://let.havefunace.top

================================================================================
来源：http://awm.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vov.yfazqb.com

================================================================================
来源：http://heg.xuetiantiany.cn

[T01] Kotlin：Hello World
来源：http://kuc.pycfn.com

println("Hello")
来源：http://bfj.chenzaomai.com

[T02] Kotlin：变量
来源：http://cja.dashuyun.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wmu.feifeiyinyue.top


<!-- 参考信息 -->