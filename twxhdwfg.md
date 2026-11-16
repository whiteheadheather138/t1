代发 wailian999

R. Bash 专题
来源：http://iyq.xuanzx.com

================================================================================
来源：http://yos.zdbjq.cn

[R01] shebang 与严格模式
来源：http://jwp.iojbl.cn

#!/usr/bin/env bash
来源：http://ycy.xuetiantiany.cn

set -euo pipefail
来源：http://cxk.hesvh.cn

[R02] 变量赋值与使用
来源：http://grz.nanxuanxn.top

name="Tom"; echo "$name"
来源：http://stc.jyoumei.cn

[R03] 只读变量
来源：http://dfu.yvedp.cn

readonly PI=3.14
来源：http://tuh.andypj.xyz

[R04] 位置参数
来源：http://bca.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bar.guowangkeji.top

[R05] 参数默认值
来源：http://zss.nanxinkj.top

name="${1:-default}"
来源：http://eid.0kj1m.cn

[R06] 判断命令是否存在
来源：http://bik.snrcjt.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hyl.jiagoushi.top

[R07] if 判断文件
来源：http://soi.xuetiantiany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cvh.epnwcf.com

[R08] 数值比较
来源：http://ysw.fanxiaobao.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://wtm.jlsjyb.cn

[R09] 字符串比较
来源：http://qsl.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sbl.jqgfzy.top

[R10] 正则匹配
来源：http://ghd.guannengcc.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ina.tianlin.xyz

[R11] case 多分支
来源：http://lnf.yfazqb.com

case "$1" in
来源：http://nmx.jqgufenzy.top

start) echo "启动" ;;
来源：http://ldg.yuxming.cn

stop)  echo "停止" ;;
来源：http://kic.guannengcc.top

*)     echo "未知命令" ;;
来源：http://nth.yuxming.cn

esac
来源：http://mqy.yonumen.top

[R12] for 遍历文件
来源：http://dhw.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://qjh.haohaochexian.top

[R13] for 计数循环
来源：http://edc.yonumen.top

for i in {1..10}; do echo "$i"; done
来源：http://cst.cqqwz.cn

[R14] C 风格 for
来源：http://iul.fanxiaobao.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rte.gzhubu.top

[R15] while 逐行读文件
来源：http://oek.cdnleiting.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iiw.snrcjt.cn

[R16] until 等待条件
来源：http://ncj.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zwn.chenzaomai.com

[R17] 数组定义与取值
来源：http://kcz.guowangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://ydq.dashuyun.cn

[R18] 遍历数组
来源：http://wvc.guannengcc.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bsi.zhongyouzk.top

[R19] 数组长度
来源：http://hlj.xuanzx.com

echo "${#arr[@]}"
来源：http://ojb.316326.xyz

[R20] 关联数组（字典）
来源：http://jhm.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fnw.316326.xyz

[R21] 字符串长度
来源：http://kso.jlsjyb.cn

echo "${#s}"
来源：http://tji.jyoumei.cn

[R22] 截取子串
来源：http://rdv.andypj.xyz

echo "${s:0:5}"
来源：http://xku.yuanzhike.top

[R23] 字符串替换
来源：http://gwz.nanxinkj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xmi.cucudq.cn

[R24] 大小写转换
来源：http://nyo.fzhhl.top

echo "${s^^}"; echo "${s,,}"
来源：http://rou.havefunace.top

[R25] 去后缀 / 去前缀
来源：http://kvi.ivvv.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://efv.ywan-chungtsiang.top

[R26] 命令替换
来源：http://hge.hnxiangtu.top

now=$(date +%F); echo "$now"
来源：http://vhk.yj202588.top

[R27] 算术展开
来源：http://ahf.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://zqq.jlsjyb.cn

[R28] 浮点运算
来源：http://lik.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://rxr.xuanzx.com

[R29] 定义函数
来源：http://yuk.52xcode.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dry.mhx1999.top

[R30] 函数返回状态码
来源：http://mhn.ppjwa.cn

f() { return 0; }; f || echo "失败了"
来源：http://jnd.ppjwa.cn

[R31] 局部变量
来源：http://yty.fktsv.cn

f() { local x=1; echo "$x"; }
来源：http://ukr.zhixingplan.top

[R32] 参数个数校验
来源：http://hux.yfazqb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kes.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://rui.ydjk.org.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qfu.aibaodan.cn

[R34] 退出时清理
来源：http://cbi.shanyushiyangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://fit.52xcode.cn

[R35] 后台执行并等待
来源：http://wbd.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qto.birdmap.top

[R36] 并发执行多个任务
来源：http://hmd.daxiang520.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jpb.ywan-chungtsiang.top

[R37] 把输出赋给变量
来源：http://iwb.pengpengdd.cyou

files=$(ls -1)
来源：http://usw.c1oappe.top

[R38] 管道串联
来源：http://dmb.fzhhl.top

cat a.txt | grep -i error | wc -l
来源：http://eif.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://qit.ydzc1.top

cmd > out.log 2>&1
来源：http://fie.pengpengdd.cyou

[R40] 追加写日志
来源：http://aqq.daria6918.cn

echo "log" >> out.log
来源：http://uhj.nanxinkj.top

[R41] 丢弃输出
来源：http://bgw.9152youxi.cn

cmd >/dev/null 2>&1
来源：http://ekc.pengpengdd.cyou

[R42] 输入重定向
来源：http://awj.xuanzx.com

wc -l < a.txt
来源：http://gbz.shangyingyoupin.top

[R43] 按名字查找文件
来源：http://bnc.xylfe.cn

find . -name "*.log" -type f
来源：http://xyz.chenlongwang.top

[R44] 按修改时间查找
来源：http://jzr.ybcxt.top

find . -mtime -7 -type f
来源：http://qhm.jyoumei.cn

[R45] 批量删除
来源：http://wax.ehwqpu.com

find . -name "*.tmp" -delete
来源：http://laz.ywan-chungtsiang.top

[R46] 递归替换文件内容
来源：http://nls.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eco.jinqigufen.top

[R47] sed 单行替换
来源：http://vlg.guannengcc.top

sed -i 's/foo/bar/g' a.txt
来源：http://zfv.yj20258.top

[R48] awk 取指定列
来源：http://qvk.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://eby.tanke756.top

[R49] awk 带条件
来源：http://znr.yvedp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sja.hfpthk.cn

[R50] awk 求和
来源：http://flz.ybcxt.top

awk '{s += $2} END {print s}' a.txt
来源：http://fur.316326.xyz

[R51] 排序去重取前几
来源：http://pvf.shanyushiyangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ogo.yj202588.top

[R52] 统计行数
来源：http://uxh.svipenyu.cn

wc -l a.txt
来源：http://xpe.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://fns.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zuk.tanke756.top

[R54] 比较两个文件
来源：http://jle.sweek.top

diff a.txt b.txt
来源：http://lxe.pycfn.com

[R55] 压缩与解压
来源：http://ase.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fvv.jyoumei.cn

[R56] 远程拷贝
来源：http://qos.hcnkem.com

scp file user@host:/path/
来源：http://mab.chenlongwang.top

[R57] 远程执行命令
来源：http://umq.fzhhl.top

ssh user@host 'uptime'
来源：http://afz.guannengcc.top

[R58] 下载文件
来源：http://bug.jqgufenzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wsb.hammf.cn

[R59] 发 POST JSON
来源：http://mmx.iojbl.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://msg.shanyushiyangkeji.top

[R60] 只看 HTTP 状态码
来源：http://xgw.yj20258.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://efu.yangfankeji.com

[R61] 磁盘占用
来源：http://mwv.yongpay.top

df -h;  du -sh *
来源：http://grq.ctjpmb.com

[R62] 找最占空间的文件
来源：http://gzg.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://ntl.wangshuangyany.cn

[R63] 内存与进程
来源：http://kal.cashguo.top

free -h;  ps aux | grep nginx
来源：http://gns.jlsjyb.cn

[R64] 结束进程
来源：http://lzn.jinqigfzy.top

kill -9 $(pgrep -f app.py)
来源：http://zab.ivvv.top

[R65] 查看端口占用
来源：http://lys.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bjf.aibaodan.cn

[R66] 定时任务
来源：http://bnn.kuanghao11.cn

crontab -e;  crontab -l
来源：http://piq.hongshengwenyu.top

[R67] 生成随机十六进制串
来源：http://woy.yvedp.cn

openssl rand -hex 16
来源：http://nrx.guowangkeji.top

[R68] 计算文件校验值
来源：http://oti.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://uzc.yonumen.top

[R69] 生成随机密码
来源：http://qrm.ydjk.org.cn

head -c 16 /dev/urandom | base64
来源：http://vsn.fktsv.cn

[R70] 时间戳与互转
来源：http://nvv.ydjk.org.cn

date +%s;  date -d @1700000000
来源：http://lsi.fengsongda.top

[R71] 日期格式化
来源：http://giy.gaohongyu789.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ixm.fengsongda.top

[R72] 等待端口就绪
来源：http://bfj.c1oappe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gqe.xinyue.icu

[R73] 分割大日志
来源：http://xre.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://xyl.gzhubu.top

[R74] 批量重命名
来源：http://lhz.fktsv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lpp.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://xun.yongpay.top

export PATH="$HOME/bin:$PATH"
来源：http://xfw.zhengqikj.top

[R76] 使用临时文件
来源：http://gzc.snrcjt.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yvr.uphjek.com

[R77] 读取用户输入
来源：http://elg.ivvv.top

read -rp "请输入: " ans
来源：http://obu.shzxlz.cn

[R78] 交互式菜单
来源：http://oid.pengpengdd.cyou

select opt in a b c; do echo "$opt"; break; done
来源：http://ixm.bjfxy.top

[R79] 解析命令行选项
来源：http://ufy.jqgfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tfv.redwolf501.top

[R80] 查看脚本执行耗时
来源：http://rlx.aizwys.cn

time ./run.sh
来源：http://jwz.havefunace.top

================================================================================
来源：http://ywu.yueranfly.top

S. C / C++ 专题
来源：http://ukv.sjlbkw.cn

================================================================================
来源：http://ctu.chenjidiqi.icu

[S01] C：Hello World
来源：http://nft.ppjwa.cn

#include <stdio.h>
来源：http://ryk.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cax.smart0.xyz

[S02] C：变量与格式化输出
来源：http://stt.jiagoushi.top

int a = 10; printf("%d\n", a);
来源：http://cjo.chenlongwang.top

[S03] C：读入整数
来源：http://emf.gogol.net.cn

int x; scanf("%d", &x);
来源：http://xgl.daria6918.cn

[S04] C：字符串复制
来源：http://vyw.havefunace.top

char dst[32]; strcpy(dst, "hi");
来源：http://swz.yangfankeji.com

[S05] C：字符串长度
来源：http://hxo.tian-w.cn

strlen(s)
来源：http://ikl.hysaishi.cn

[S06] C：字符串比较
来源：http://chd.vehdjk.com

strcmp(a, b) == 0
来源：http://ych.bjfxy.top

[S07] C：数组遍历求和
来源：http://qbg.daxiang520.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://skn.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://ufq.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cdh.zhoulong.xyz

[S09] C：结构体定义与初始化
来源：http://ixh.havefunace.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gym.cucudq.cn

[S10] C：指针与解引用
来源：http://lex.hnxiangtu.top

int *p = &a;  *p = 5;
来源：http://jhg.xinyue.icu

[S11] C：逐行读文件
来源：http://nps.xziqi.cn

FILE *f = fopen("a.txt", "r");
来源：http://axr.svipenyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ogc.yangfankeji.com

fclose(f);
来源：http://fpn.jiagoushi.top

[S12] C：写文件
来源：http://qch.jlsjyb.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ovv.fzhhl.top

[S13] C：宏定义
来源：http://tmk.feifeiyinyue.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zim.cqqwz.cn

[S14] C：枚举
来源：http://sib.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://uvr.zdbjq.cn

[S15] C：类型转换
来源：http://ztn.quarkkingdee.top

(double) a / b
来源：http://cjk.gzhubu.top

[S16] C：位操作置位
来源：http://bte.aibaodan.cn

x |= (1 << 3);
来源：http://vuv.ivvv.top

[S17] C：安全拼接字符串
来源：http://edm.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rxf.zdbjq.cn

[S18] C：命令行参数
来源：http://web.jqgufenzy.top

int main(int argc, char **argv)
来源：http://bmt.vqdsnc.cn

[S19] C：快速排序
来源：http://qhx.sweek.top

qsort(a, n, sizeof(int), cmp);
来源：http://chy.yj20258.top

[S20] C：二分查找
来源：http://zoe.smart0.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ifw.sysykeji.top

[S21] C：字符类别判断
来源：http://jyw.tianlin.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://khg.vqdsnc.cn

[S22] C：字符串转数字
来源：http://rzg.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://pkf.52xcode.cn

[S23] C：随机数
来源：http://jbv.gaohongyu789.top

srand(time(NULL));  int r = rand() % 100;
来源：http://agv.fzhhl.top

[S24] C：获取本地时间
来源：http://ous.hammf.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ndt.sxryk.cn

[S25] C：内存拷贝
来源：http://toa.nanxuanxn.top

memcpy(dst, src, n);
来源：http://sjt.hfpthk.cn

[S26] C：内存清零
来源：http://mmn.ppjwa.cn

memset(a, 0, sizeof a);
来源：http://isu.svipenyu.cn

[S27] C：定义常量
来源：http://cpq.cashguo.top

const double PI = 3.14159;
来源：http://sfv.yueranfly.top

[S28] C：静态变量
来源：http://zso.yonumen.top

static int counter = 0;
来源：http://anb.hysaishi.cn

[S29] C：变参函数
来源：http://fyw.sxryk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eer.kuanghao11.cn

[S30] C：头文件保护
来源：http://xqf.sweek.top

#ifndef X_H
来源：http://bov.gzhubu.top

#define X_H
来源：http://qki.gotoacloud.top

#endif
来源：http://cza.tianlin.xyz

[S31] C++：Hello World
来源：http://fyn.hesvh.cn

#include <iostream>
来源：http://peu.daria6918.cn

int main() { std::cout << "Hello\n"; }
来源：http://jcg.smart0.xyz

[S32] C++：字符串
来源：http://bcg.quarkkingdee.top

std::string s = "hi";  s += "!";
来源：http://iht.ivvv.top

[S33] C++：vector 增删
来源：http://ecz.gogol.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://avp.zdqjudy.top

[S34] C++：遍历 vector
来源：http://rcm.hnxiangtu.top

for (auto &x : v) { std::cout << x; }
来源：http://mdt.jqgufenzy.top

[S35] C++：map
来源：http://rng.sufxvd.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wri.yonumen.top

[S36] C++：unordered_map
来源：http://dxd.gogol.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://loe.yj20258.top

[S37] C++：set
来源：http://vhx.zhongyouzk.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zwk.aibaodan.cn

[S38] C++：排序
来源：http://umu.birdmap.top

std::sort(v.begin(), v.end());
来源：http://vfr.hammf.cn

[S39] C++：自定义比较器排序
来源：http://hmb.yvedp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iqp.sjlbkw.cn

[S40] C++：查找元素
来源：http://efe.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ylt.fktsv.cn

[S41] C++：类与构造函数
来源：http://esu.cheryme.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xmw.xylfe.cn

[S42] C++：继承与虚函数
来源：http://xjp.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://cfk.iojbl.cn

[S43] C++：智能指针
来源：http://khz.yj20258888.top

auto p = std::make_unique<int>(5);
来源：http://rpj.hfpthk.cn

[S44] C++：引用传参
来源：http://vef.dianchejie.cn

void inc(int &x) { ++x; }
来源：http://rzp.yanxiufei.cn

[S45] C++：lambda
来源：http://fij.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://vlx.dashuyun.cn

[S46] C++：函数模板
来源：http://ddj.jlsjyb.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://soc.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://xbj.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ptb.andypj.xyz

[S48] C++：逐行读文件
来源：http://xhm.hnqzz.top

std::ifstream in("a.txt");  std::string line;
来源：http://xtd.jinqigfzy.top

while (std::getline(in, line)) { }
来源：http://ldf.vehdjk.com

[S49] C++：写文件
来源：http://llc.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mnt.nanxuanxn.top

[S50] C++：格式化数字
来源：http://cuw.bjfxy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oxh.mhx1999.top

[S51] C++：显式类型转换
来源：http://emq.pycfn.com

static_cast<double>(a) / b
来源：http://tgt.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://jed.vehdjk.com

int size() const noexcept { return n_; }
来源：http://nos.quarkkingdee.top

[S53] C++：移动语义
来源：http://vag.sweek.top

std::vector<int> w = std::move(v);
来源：http://zrd.guannengcc.top

[S54] C++：异常处理
来源：http://jsb.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vwh.hnxiangtu.top

[S55] C++：结构化绑定
来源：http://omy.shanyushiyangtech.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uwr.zdbjq.cn

[S56] C++：optional
来源：http://bgk.hywenlv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://idf.shzxlz.cn

[S57] C++：编译期常量
来源：http://miz.yangfankeji.com

constexpr int N = 10;
来源：http://atn.tanke756.top

[S58] C++：命名空间
来源：http://hdi.cqqwz.cn

namespace ns { int f() { return 1; } }
来源：http://dtw.haohaochexian.top

[S59] C++：静态断言
来源：http://qwv.jqgfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lvs.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://stm.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dyv.nanxinkj.top

================================================================================
来源：http://dpp.birdmap.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tly.tanke756.top

================================================================================
来源：http://fbr.yanxiufei.cn


<!-- 参考信息 -->