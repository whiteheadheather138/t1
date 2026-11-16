代发 wailian999

set -euo pipefail
来源：http://czt.yfazqb.com

[R02] 变量赋值与使用
来源：http://nbr.ydzc1.top

name="Tom"; echo "$name"
来源：http://qhu.yvedp.cn

[R03] 只读变量
来源：http://yzc.hesvh.cn

readonly PI=3.14
来源：http://dtj.shangyingyoupin.top

[R04] 位置参数
来源：http://naa.52xcode.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qxh.ydzc1.top

[R05] 参数默认值
来源：http://cav.nanxuanxn.top

name="${1:-default}"
来源：http://oxj.fktsv.cn

[R06] 判断命令是否存在
来源：http://efn.jinyuanbaomall.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ear.hcnkem.com

[R07] if 判断文件
来源：http://kmw.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://egh.daria6918.cn

[R08] 数值比较
来源：http://cuz.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qlk.hywenlv.cn

[R09] 字符串比较
来源：http://zzr.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mov.aizwys.cn

[R10] 正则匹配
来源：http://bmm.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fmq.ybcxt.top

[R11] case 多分支
来源：http://bpr.yueranfly.top

case "$1" in
来源：http://ecn.sxryk.cn

start) echo "启动" ;;
来源：http://kpa.svipenyu.cn

stop)  echo "停止" ;;
来源：http://seq.dianchejie.cn

*)     echo "未知命令" ;;
来源：http://hvw.ywan-chungtsiang.top

esac
来源：http://jma.yvedp.cn

[R12] for 遍历文件
来源：http://eak.yfazqb.com

for f in *.txt; do echo "$f"; done
来源：http://vhu.jinqigfzy.top

[R13] for 计数循环
来源：http://myr.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://hsd.yuanzhike.top

[R14] C 风格 for
来源：http://bpv.fzhhl.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wki.hesvh.cn

[R15] while 逐行读文件
来源：http://dzp.tian-w.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jea.gzhubu.top

[R16] until 等待条件
来源：http://osy.xylfe.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iws.vqdsnc.cn

[R17] 数组定义与取值
来源：http://esp.xingfuxueyuan.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://gax.wangdashe.top

[R18] 遍历数组
来源：http://prs.aizwys.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iji.bbcook.cn

[R19] 数组长度
来源：http://tmn.jlsjyb.cn

echo "${#arr[@]}"
来源：http://fxm.cucudq.cn

[R20] 关联数组（字典）
来源：http://vtb.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nzk.yfazqb.com

[R21] 字符串长度
来源：http://vld.hfpthk.cn

echo "${#s}"
来源：http://cas.cqqwz.cn

[R22] 截取子串
来源：http://our.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://wxn.shanyushiyangtech.top

[R23] 字符串替换
来源：http://sns.wangdashe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jus.tarul.cn

[R24] 大小写转换
来源：http://qft.zdqjudy.top

echo "${s^^}"; echo "${s,,}"
来源：http://mpq.vehdjk.com

[R25] 去后缀 / 去前缀
来源：http://wkb.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pjf.fengsongda.top

[R26] 命令替换
来源：http://kcr.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://dck.tarul.cn

[R27] 算术展开
来源：http://osw.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://vcs.sufxvd.cn

[R28] 浮点运算
来源：http://ofs.cheryme.top

echo "scale=2; 10/3" | bc
来源：http://ofp.xuanzx.com

[R29] 定义函数
来源：http://jym.nanxuanxn.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://otl.jinghuilouyu.cn

[R30] 函数返回状态码
来源：http://xtj.wangdashe.top

f() { return 0; }; f || echo "失败了"
来源：http://rjl.cucudq.cn

[R31] 局部变量
来源：http://ebx.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://hky.chenzaomai.com

[R32] 参数个数校验
来源：http://bwc.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://flj.snrcjt.cn

[R33] 捕获错误并提示行号
来源：http://yvl.sysykeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oek.tanke756.top

[R34] 退出时清理
来源：http://tun.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://vhq.yongpay.top

[R35] 后台执行并等待
来源：http://tjy.svipenyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jkv.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://bxj.ehwqpu.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nqi.yuxming.cn

[R37] 把输出赋给变量
来源：http://nab.hongshengwenyu.top

files=$(ls -1)
来源：http://mxv.jqgufenzy.top

[R38] 管道串联
来源：http://gck.hywenlv.cn

cat a.txt | grep -i error | wc -l
来源：http://jmh.nwbrower.top

[R39] 重定向标准输出与错误
来源：http://bpq.ppjwa.cn

cmd > out.log 2>&1
来源：http://hzb.wangshuangyany.cn

[R40] 追加写日志
来源：http://trj.zhiwuduotai.top

echo "log" >> out.log
来源：http://sfn.zdqjudy.top

[R41] 丢弃输出
来源：http://izs.guowangkeji.top

cmd >/dev/null 2>&1
来源：http://dln.fzhhl.top

[R42] 输入重定向
来源：http://brl.hcnkem.com

wc -l < a.txt
来源：http://bso.tanke756.top

[R43] 按名字查找文件
来源：http://tul.316326.xyz

find . -name "*.log" -type f
来源：http://kok.sweek.top

[R44] 按修改时间查找
来源：http://rvy.bjfxy.top

find . -mtime -7 -type f
来源：http://uld.ywan-chungtsiang.top

[R45] 批量删除
来源：http://pen.pycfn.com

find . -name "*.tmp" -delete
来源：http://ykn.zhijiandao.cn

[R46] 递归替换文件内容
来源：http://yrz.gzhubu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yaj.fktsv.cn

[R47] sed 单行替换
来源：http://krv.xuetiantiany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://olk.ywan-chungtsiang.top

[R48] awk 取指定列
来源：http://zjm.yuanzhike.top

awk '{print $1, $3}' a.txt
来源：http://nat.yuxming.cn

[R49] awk 带条件
来源：http://mci.gaohongyu789.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mqh.ivvv.top

[R50] awk 求和
来源：http://lhw.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://xay.svipenyu.cn

[R51] 排序去重取前几
来源：http://tna.ppjwa.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ufd.redwolf501.top

[R52] 统计行数
来源：http://hsi.daria6918.cn

wc -l a.txt
来源：http://rma.yvedp.cn

[R53] 查看文件头与实时尾
来源：http://epr.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qen.zhongyouzk.top

[R54] 比较两个文件
来源：http://twt.yfazqb.com

diff a.txt b.txt
来源：http://hzi.daxiang520.top

[R55] 压缩与解压
来源：http://wqo.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qin.0kj1m.cn

[R56] 远程拷贝
来源：http://edx.aibaodan.cn

scp file user@host:/path/
来源：http://vuy.snrcjt.cn

[R57] 远程执行命令
来源：http://lxo.fehbvm.com

ssh user@host 'uptime'
来源：http://iwd.gaohongyu789.top

[R58] 下载文件
来源：http://ipt.ehwqpu.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ued.dianchejie.cn

[R59] 发 POST JSON
来源：http://nev.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kiq.gogol.net.cn

[R60] 只看 HTTP 状态码
来源：http://zmh.hammf.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mom.yueranfly.top

[R61] 磁盘占用
来源：http://whq.fktsv.cn

df -h;  du -sh *
来源：http://uxr.xziqi.cn

[R62] 找最占空间的文件
来源：http://rwm.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://rpc.yangfankeji.com

[R63] 内存与进程
来源：http://oxl.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://njc.xziqi.cn

[R64] 结束进程
来源：http://wdm.redwolf501.top

kill -9 $(pgrep -f app.py)
来源：http://oxv.yangfankeji.com

[R65] 查看端口占用
来源：http://iql.birdmap.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qdu.wangshuangyany.cn

[R66] 定时任务
来源：http://yxr.andypj.xyz

crontab -e;  crontab -l
来源：http://qgt.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://fez.jinghuilouyu.cn

openssl rand -hex 16
来源：http://mhj.xuanzx.com

[R68] 计算文件校验值
来源：http://thg.cheryme.top

sha256sum a.txt;  md5sum a.txt
来源：http://khk.zhijiandao.cn

[R69] 生成随机密码
来源：http://hqi.ivvv.top

head -c 16 /dev/urandom | base64
来源：http://hpz.jqgfzy.top

[R70] 时间戳与互转
来源：http://oov.haohaochexian.top

date +%s;  date -d @1700000000
来源：http://fdd.tarul.cn

[R71] 日期格式化
来源：http://tip.jlsjyb.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ncc.xuanzx.com

[R72] 等待端口就绪
来源：http://gol.chenlongwang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://you.ydjk.org.cn

[R73] 分割大日志
来源：http://fwi.shuidangran.top

split -l 1000 big.log part_
来源：http://zsp.havefunace.top

[R74] 批量重命名
来源：http://ugu.gaohongyu789.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://did.sweek.top

[R75] 导出环境变量
来源：http://nbr.zdbjq.cn

export PATH="$HOME/bin:$PATH"
来源：http://bwr.hnxiangtu.top

[R76] 使用临时文件
来源：http://omw.zdqjudy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qda.sxryk.cn

[R77] 读取用户输入
来源：http://ujz.mhx1999.top

read -rp "请输入: " ans
来源：http://trb.yongpay.top

[R78] 交互式菜单
来源：http://ffn.bjfxy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://afx.zhongyouzk.top

[R79] 解析命令行选项
来源：http://ldc.hnxiangtu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fuc.wangdashe.top

[R80] 查看脚本执行耗时
来源：http://iwq.cqqwz.cn

time ./run.sh
来源：http://flk.yuanzhike.top

================================================================================
来源：http://vmd.xinyue.icu

S. C / C++ 专题
来源：http://goa.smart0.xyz

================================================================================
来源：http://wyx.uphjek.com

[S01] C：Hello World
来源：http://xls.havefunace.top

#include <stdio.h>
来源：http://ula.316326.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://agj.xziqi.cn

[S02] C：变量与格式化输出
来源：http://qmx.hnxiangtu.top

int a = 10; printf("%d\n", a);
来源：http://lpc.zhaomingkeji.xyz

[S03] C：读入整数
来源：http://qbw.zdbjq.cn

int x; scanf("%d", &x);
来源：http://roe.shzxlz.cn

[S04] C：字符串复制
来源：http://skr.xinyue.icu

char dst[32]; strcpy(dst, "hi");
来源：http://ftj.zhaomingkeji.xyz

[S05] C：字符串长度
来源：http://gxv.uphjek.com

strlen(s)
来源：http://wpd.zycfv.cn

[S06] C：字符串比较
来源：http://eie.smart0.xyz

strcmp(a, b) == 0
来源：http://ekk.gzhubu.top

[S07] C：数组遍历求和
来源：http://pdo.yangfankeji.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bak.tanke756.top

[S08] C：动态内存分配与释放
来源：http://cho.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jhy.kuanghao11.cn

[S09] C：结构体定义与初始化
来源：http://win.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aqq.316326.xyz

[S10] C：指针与解引用
来源：http://eqs.fengsongda.top

int *p = &a;  *p = 5;
来源：http://hzg.epnwcf.com

[S11] C：逐行读文件
来源：http://ybm.nwbrower.top

FILE *f = fopen("a.txt", "r");
来源：http://ncc.sjlbkw.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dkg.yueranfly.top

fclose(f);
来源：http://cdw.snrcjt.cn

[S12] C：写文件
来源：http://cdp.zdqjudy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://olw.wangshuangyany.cn

[S13] C：宏定义
来源：http://bxv.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hmu.svipenyu.cn

[S14] C：枚举
来源：http://mry.52xcode.cn

enum Color { RED, GREEN, BLUE };
来源：http://nvl.jianghu66.top

[S15] C：类型转换
来源：http://rce.daxiang520.top

(double) a / b
来源：http://zey.wangshuangyany.cn

[S16] C：位操作置位
来源：http://igt.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://mqb.yvedp.cn

[S17] C：安全拼接字符串
来源：http://uqd.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jlj.daria6918.cn

[S18] C：命令行参数
来源：http://myb.fengsongda.top

int main(int argc, char **argv)
来源：http://okd.chenzaomai.com

[S19] C：快速排序
来源：http://msp.52xcode.cn

qsort(a, n, sizeof(int), cmp);
来源：http://elj.gzhubu.top

[S20] C：二分查找
来源：http://wul.yueranfly.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fng.aizwys.cn

[S21] C：字符类别判断
来源：http://zsi.andypj.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pow.cqqwz.cn

[S22] C：字符串转数字
来源：http://vyu.hongshengwenyu.top

atoi("42");  strtod("3.14", NULL);
来源：http://por.vehdjk.com

[S23] C：随机数
来源：http://bmw.gotoacloud.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oyz.yj202588.top

[S24] C：获取本地时间
来源：http://lqe.uphjek.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xug.yonumen.top

[S25] C：内存拷贝
来源：http://dae.0kj1m.cn

memcpy(dst, src, n);
来源：http://uml.nwbrower.top

[S26] C：内存清零
来源：http://yga.shanyushiyangkeji.top

memset(a, 0, sizeof a);
来源：http://qpr.cashguo.top

[S27] C：定义常量
来源：http://nsx.sysykeji.top

const double PI = 3.14159;
来源：http://ioq.kuanghao11.cn

[S28] C：静态变量
来源：http://syt.kuanghao11.cn

static int counter = 0;
来源：http://dxr.shuidangran.top

[S29] C：变参函数
来源：http://xwk.pengpengdd.cyou

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://njz.shanyushiyangkeji.top

[S30] C：头文件保护
来源：http://uoa.zdqjudy.top

#ifndef X_H
来源：http://ufq.fzhhl.top

#define X_H
来源：http://tsy.meibo888.top

#endif
来源：http://nbm.gaohongyu789.top

[S31] C++：Hello World
来源：http://jvx.xinyue.icu

#include <iostream>
来源：http://nfr.zhixingplan.top

int main() { std::cout << "Hello\n"; }
来源：http://ubv.tarul.cn

[S32] C++：字符串
来源：http://rgb.ydjk.org.cn

std::string s = "hi";  s += "!";
来源：http://lao.xuanzx.com

[S33] C++：vector 增删
来源：http://qij.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wyd.aibaodan.cn

[S34] C++：遍历 vector
来源：http://qhl.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://pow.shangyingyoupin.top

[S35] C++：map
来源：http://zvj.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dxq.ybcxt.top

[S36] C++：unordered_map
来源：http://ibf.zhongyouzk.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hvq.quarkkingdee.top

[S37] C++：set
来源：http://mjc.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bcc.aibaodan.cn

[S38] C++：排序
来源：http://dzn.fanxiaobao.xyz

std::sort(v.begin(), v.end());
来源：http://hxs.cucudq.cn

[S39] C++：自定义比较器排序
来源：http://yir.gaohongyu789.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cxe.svipenyu.cn

[S40] C++：查找元素
来源：http://igu.zhongyouzk.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://riv.ppjwa.cn

[S41] C++：类与构造函数
来源：http://smy.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://awo.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://hcx.mhx1999.top

class B : public Base { public: void f() override {} };
来源：http://jla.zhengqikj.top

[S43] C++：智能指针
来源：http://zer.pengpengdd.cyou

auto p = std::make_unique<int>(5);
来源：http://bgv.hysaishi.cn

[S44] C++：引用传参
来源：http://txo.shanyushiyangtech.top

void inc(int &x) { ++x; }
来源：http://sio.andypj.xyz

[S45] C++：lambda
来源：http://ifo.redwolf501.top

auto add = [](int a, int b) { return a + b; };
来源：http://jov.shuidangran.top

[S46] C++：函数模板
来源：http://wnb.hcnkem.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wpe.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://oer.tanke756.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mfh.andypj.xyz

[S48] C++：逐行读文件
来源：http://qmf.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://kfq.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://ktu.aizwys.cn

[S49] C++：写文件
来源：http://zmq.ydzc1.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cws.hnxiangtu.top

[S50] C++：格式化数字
来源：http://xpu.52xcode.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dqh.zdqjudy.top

[S51] C++：显式类型转换
来源：http://gxs.zhixingplan.top

static_cast<double>(a) / b
来源：http://cvr.zhixingplan.top

[S52] C++：const 与 noexcept
来源：http://wcn.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://mrv.haohaochexian.top

[S53] C++：移动语义
来源：http://wqk.feifeiyinyue.top

std::vector<int> w = std::move(v);
来源：http://lgj.hfpthk.cn

[S54] C++：异常处理
来源：http://ngf.ehwqpu.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zcv.ppjwa.cn

[S55] C++：结构化绑定
来源：http://gyn.daria6918.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://crf.aibaodan.cn

[S56] C++：optional
来源：http://psi.gotoacloud.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fmg.tian-w.cn

[S57] C++：编译期常量
来源：http://ysz.wangdashe.top

constexpr int N = 10;
来源：http://xgu.iojbl.cn

[S58] C++：命名空间
来源：http://igp.hfpthk.cn

namespace ns { int f() { return 1; } }
来源：http://guu.gogol.net.cn

[S59] C++：静态断言
来源：http://umv.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fgn.tanke756.top

[S60] C++：遍历并删除元素
来源：http://cfr.vqdsnc.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uym.zycfv.cn

================================================================================
来源：http://ojm.zhiwuduotai.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jil.jiagoushi.top

================================================================================
来源：http://nsy.jqgfzy.top

[T01] Kotlin：Hello World
来源：http://ncx.jlsjyb.cn

println("Hello")
来源：http://qhk.ydjk.org.cn

[T02] Kotlin：变量
来源：http://zoa.pycfn.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yid.jinqigfzy.top


<!-- 参考信息 -->