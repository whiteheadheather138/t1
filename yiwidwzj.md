代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tcn.nanxinkj.top

[R10] 正则匹配
来源：http://tye.yj20258888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fyj.pycfn.com

[R11] case 多分支
来源：http://bfw.zhijiandao.cn

case "$1" in
来源：http://pcs.yuanzhike.top

start) echo "启动" ;;
来源：http://bvi.epnwcf.com

stop)  echo "停止" ;;
来源：http://cpc.tianlin.xyz

*)     echo "未知命令" ;;
来源：http://xky.feifeiyinyue.top

esac
来源：http://kpl.svipenyu.cn

[R12] for 遍历文件
来源：http://rct.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://lfe.sufxvd.cn

[R13] for 计数循环
来源：http://dsn.c1oappe.top

for i in {1..10}; do echo "$i"; done
来源：http://sic.fzhhl.top

[R14] C 风格 for
来源：http://kxv.zhaomingkeji.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fyc.epnwcf.com

[R15] while 逐行读文件
来源：http://lih.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qap.xuanzx.com

[R16] until 等待条件
来源：http://btb.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sbu.yanxiufei.cn

[R17] 数组定义与取值
来源：http://beg.cqqwz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://eor.shanyushiyangtech.top

[R18] 遍历数组
来源：http://idx.zhijiandao.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wtt.ivvv.top

[R19] 数组长度
来源：http://yqm.cqqwz.cn

echo "${#arr[@]}"
来源：http://gul.dianchejie.cn

[R20] 关联数组（字典）
来源：http://bdf.tarul.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wjc.jiagoushi.top

[R21] 字符串长度
来源：http://ebe.jlsjyb.cn

echo "${#s}"
来源：http://bme.sufxvd.cn

[R22] 截取子串
来源：http://gaz.yj20258888.top

echo "${s:0:5}"
来源：http://kuc.vehdjk.com

[R23] 字符串替换
来源：http://mbs.uphjek.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://har.sjlbkw.cn

[R24] 大小写转换
来源：http://lpu.shanyushiyangtech.top

echo "${s^^}"; echo "${s,,}"
来源：http://wqz.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://vht.mhx1999.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ezi.cucudq.cn

[R26] 命令替换
来源：http://hud.tarul.cn

now=$(date +%F); echo "$now"
来源：http://jeq.pengpengdd.cyou

[R27] 算术展开
来源：http://cbt.yj20258.top

echo $((1 + 2 * 3))
来源：http://jxl.sweek.top

[R28] 浮点运算
来源：http://hsi.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://sqc.havefunace.top

[R29] 定义函数
来源：http://rmq.bbcook.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uzc.quarkkingdee.top

[R30] 函数返回状态码
来源：http://qbb.hysaishi.cn

f() { return 0; }; f || echo "失败了"
来源：http://prh.yueranfly.top

[R31] 局部变量
来源：http://npt.cdnleiting.top

f() { local x=1; echo "$x"; }
来源：http://zpa.jinqigfzy.top

[R32] 参数个数校验
来源：http://bzm.tanke756.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iws.aizwys.cn

[R33] 捕获错误并提示行号
来源：http://flm.fengsongda.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rns.cdnleiting.top

[R34] 退出时清理
来源：http://fmi.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pqb.chenjidiqi.icu

[R35] 后台执行并等待
来源：http://epy.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://cqt.yvedp.cn

[R36] 并发执行多个任务
来源：http://ssg.haohaochexian.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fzw.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://mlz.feifeiyinyue.top

files=$(ls -1)
来源：http://kty.gogol.net.cn

[R38] 管道串联
来源：http://nym.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://lar.9152youxi.cn

[R39] 重定向标准输出与错误
来源：http://hok.snrcjt.cn

cmd > out.log 2>&1
来源：http://pds.aizwys.cn

[R40] 追加写日志
来源：http://ido.hysaishi.cn

echo "log" >> out.log
来源：http://gng.tarul.cn

[R41] 丢弃输出
来源：http://yao.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://rmx.yuanzhike.top

[R42] 输入重定向
来源：http://pew.shuidangran.top

wc -l < a.txt
来源：http://vjp.guowangkeji.top

[R43] 按名字查找文件
来源：http://gux.hcnkem.com

find . -name "*.log" -type f
来源：http://jja.yfazqb.com

[R44] 按修改时间查找
来源：http://odp.bjfxy.top

find . -mtime -7 -type f
来源：http://clp.jqgfzy.top

[R45] 批量删除
来源：http://spw.sysykeji.top

find . -name "*.tmp" -delete
来源：http://wlq.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://nrt.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://auj.yfazqb.com

[R47] sed 单行替换
来源：http://nqb.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fmv.yongpay.top

[R48] awk 取指定列
来源：http://iah.meibo888.top

awk '{print $1, $3}' a.txt
来源：http://ann.zhixingplan.top

[R49] awk 带条件
来源：http://kid.tianlin.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kdy.redwolf501.top

[R50] awk 求和
来源：http://wyz.haohaochexian.top

awk '{s += $2} END {print s}' a.txt
来源：http://mqj.nwbrower.top

[R51] 排序去重取前几
来源：http://cxy.xylfe.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uwn.zhaomingkeji.xyz

[R52] 统计行数
来源：http://tlg.zhiwuduotai.top

wc -l a.txt
来源：http://xkp.pengpengdd.cyou

[R53] 查看文件头与实时尾
来源：http://tdj.yuxming.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qcp.aizwys.cn

[R54] 比较两个文件
来源：http://lov.andypj.xyz

diff a.txt b.txt
来源：http://grv.yuanzhike.top

[R55] 压缩与解压
来源：http://vgl.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ftd.zhongyouzk.top

[R56] 远程拷贝
来源：http://ucr.shzxlz.cn

scp file user@host:/path/
来源：http://cej.zycfv.cn

[R57] 远程执行命令
来源：http://iun.fzhhl.top

ssh user@host 'uptime'
来源：http://vgz.zdbjq.cn

[R58] 下载文件
来源：http://xed.yuxming.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mjr.jqgufenzy.top

[R59] 发 POST JSON
来源：http://yed.jinyuanbaomall.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ekx.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://tjh.xinyue.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jav.yuxming.cn

[R61] 磁盘占用
来源：http://jqk.jyoumei.cn

df -h;  du -sh *
来源：http://xbg.pengpengdd.cyou

[R62] 找最占空间的文件
来源：http://cyp.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://pjh.havefunace.top

[R63] 内存与进程
来源：http://mbz.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://kxc.9152youxi.cn

[R64] 结束进程
来源：http://ppc.jqgufenzy.top

kill -9 $(pgrep -f app.py)
来源：http://nmm.meibo888.top

[R65] 查看端口占用
来源：http://trh.zdqjudy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nsl.jinqigfzy.top

[R66] 定时任务
来源：http://loh.guannengcc.top

crontab -e;  crontab -l
来源：http://aly.zycfv.cn

[R67] 生成随机十六进制串
来源：http://qes.shzxlz.cn

openssl rand -hex 16
来源：http://fzm.gotoacloud.top

[R68] 计算文件校验值
来源：http://ojp.zdbjq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qbv.chenjidiqi.icu

[R69] 生成随机密码
来源：http://qma.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://ovf.hywenlv.cn

[R70] 时间戳与互转
来源：http://tpp.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://ajp.daria6918.cn

[R71] 日期格式化
来源：http://kwd.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://npt.9152youxi.cn

[R72] 等待端口就绪
来源：http://tcz.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://bsn.sweek.top

[R73] 分割大日志
来源：http://zfc.nwbrower.top

split -l 1000 big.log part_
来源：http://upx.haohaochexian.top

[R74] 批量重命名
来源：http://jld.aibaodan.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bup.yuxming.cn

[R75] 导出环境变量
来源：http://can.jianghu66.top

export PATH="$HOME/bin:$PATH"
来源：http://ovq.jianghu66.top

[R76] 使用临时文件
来源：http://gye.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://asl.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://flt.0kj1m.cn

read -rp "请输入: " ans
来源：http://mxn.tanke756.top

[R78] 交互式菜单
来源：http://rnf.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://izb.ctjpmb.com

[R79] 解析命令行选项
来源：http://ftc.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gnu.jlsjyb.cn

[R80] 查看脚本执行耗时
来源：http://fon.sufxvd.cn

time ./run.sh
来源：http://shz.yueranfly.top

================================================================================
来源：http://mvk.ydzc1.top

S. C / C++ 专题
来源：http://wyq.9152youxi.cn

================================================================================
来源：http://yng.zhengqikj.top

[S01] C：Hello World
来源：http://rsf.shanyushiyangkeji.top

#include <stdio.h>
来源：http://xbf.hnxiangtu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gmb.pycfn.com

[S02] C：变量与格式化输出
来源：http://txz.jianghu66.top

int a = 10; printf("%d\n", a);
来源：http://xxy.zhongyouzk.top

[S03] C：读入整数
来源：http://inw.ctjpmb.com

int x; scanf("%d", &x);
来源：http://mfs.wangshuangyany.cn

[S04] C：字符串复制
来源：http://wmy.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://kqq.ydjk.org.cn

[S05] C：字符串长度
来源：http://xpn.cqqwz.cn

strlen(s)
来源：http://ivu.tanke756.top

[S06] C：字符串比较
来源：http://osu.fengsongda.top

strcmp(a, b) == 0
来源：http://yul.yueranfly.top

[S07] C：数组遍历求和
来源：http://jzm.yvedp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zvh.cashguo.top

[S08] C：动态内存分配与释放
来源：http://dgo.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hgc.daria6918.cn

[S09] C：结构体定义与初始化
来源：http://gtb.yonumen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xqp.chenzaomai.com

[S10] C：指针与解引用
来源：http://isx.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://fgq.cdnleiting.top

[S11] C：逐行读文件
来源：http://jsu.tian-w.cn

FILE *f = fopen("a.txt", "r");
来源：http://gjq.0kj1m.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iva.sjlbkw.cn

fclose(f);
来源：http://tnl.zdqjudy.top

[S12] C：写文件
来源：http://rfx.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ppl.hongshengwenyu.top

[S13] C：宏定义
来源：http://sdy.sufxvd.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://myd.jinqigufen.top

[S14] C：枚举
来源：http://jxk.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://mhw.dianchejie.cn

[S15] C：类型转换
来源：http://gdv.yfazqb.com

(double) a / b
来源：http://uga.yj202588.top

[S16] C：位操作置位
来源：http://hyb.sufxvd.cn

x |= (1 << 3);
来源：http://ogh.sjlbkw.cn

[S17] C：安全拼接字符串
来源：http://ddx.zhixingplan.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mas.chenzaomai.com

[S18] C：命令行参数
来源：http://wwz.sweek.top

int main(int argc, char **argv)
来源：http://pre.zhengqikj.top

[S19] C：快速排序
来源：http://xro.nwbrower.top

qsort(a, n, sizeof(int), cmp);
来源：http://snq.shzxlz.cn

[S20] C：二分查找
来源：http://xwk.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tby.hcnkem.com

[S21] C：字符类别判断
来源：http://rxk.hysaishi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://roi.mhx1999.top

[S22] C：字符串转数字
来源：http://zqr.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://dyb.hnxiangtu.top

[S23] C：随机数
来源：http://edl.zdqjudy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rcg.jyoumei.cn

[S24] C：获取本地时间
来源：http://sak.hesvh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qry.vehdjk.com

[S25] C：内存拷贝
来源：http://dvw.ybcxt.top

memcpy(dst, src, n);
来源：http://crd.sjlbkw.cn

[S26] C：内存清零
来源：http://swv.bjfxy.top

memset(a, 0, sizeof a);
来源：http://reo.hesvh.cn

[S27] C：定义常量
来源：http://nho.cqqwz.cn

const double PI = 3.14159;
来源：http://wbg.jianghu66.top

[S28] C：静态变量
来源：http://qkc.guannengcc.top

static int counter = 0;
来源：http://khc.shuidangran.top

[S29] C：变参函数
来源：http://agy.fzhhl.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://olj.gotoacloud.top

[S30] C：头文件保护
来源：http://cfm.wangdashe.top

#ifndef X_H
来源：http://aun.cdnleiting.top

#define X_H
来源：http://ufl.0kj1m.cn

#endif
来源：http://udj.zhengqikj.top

[S31] C++：Hello World
来源：http://ato.yueranfly.top

#include <iostream>
来源：http://zqc.nanxuanxn.top

int main() { std::cout << "Hello\n"; }
来源：http://nip.yuxming.cn

[S32] C++：字符串
来源：http://ahn.meibo888.top

std::string s = "hi";  s += "!";
来源：http://thl.havefunace.top

[S33] C++：vector 增删
来源：http://yze.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://apk.svipenyu.cn

[S34] C++：遍历 vector
来源：http://sjr.hongshengwenyu.top

for (auto &x : v) { std::cout << x; }
来源：http://osy.hysaishi.cn

[S35] C++：map
来源：http://rxf.fehbvm.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://evy.yueranfly.top

[S36] C++：unordered_map
来源：http://lde.wangdashe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rrj.fktsv.cn

[S37] C++：set
来源：http://cuc.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tmo.ivvv.top

[S38] C++：排序
来源：http://qgg.haohaochexian.top

std::sort(v.begin(), v.end());
来源：http://xcr.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://xus.shuidangran.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aew.epnwcf.com

[S40] C++：查找元素
来源：http://efr.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://htk.andypj.xyz

[S41] C++：类与构造函数
来源：http://ksa.nanxinkj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mzt.shangyingyoupin.top

[S42] C++：继承与虚函数
来源：http://kpv.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://muz.zdbjq.cn

[S43] C++：智能指针
来源：http://kxm.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://zhh.zhiwuduotai.top

[S44] C++：引用传参
来源：http://ltl.yvedp.cn

void inc(int &x) { ++x; }
来源：http://gfv.chenlongwang.top

[S45] C++：lambda
来源：http://bew.ywan-chungtsiang.top

auto add = [](int a, int b) { return a + b; };
来源：http://syx.nwbrower.top

[S46] C++：函数模板
来源：http://bnt.jlsjyb.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://puj.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://ozy.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://daj.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://sip.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://tsc.52xcode.cn

while (std::getline(in, line)) { }
来源：http://lmm.snrcjt.cn

[S49] C++：写文件
来源：http://ovv.daria6918.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ccp.xuanzx.com

[S50] C++：格式化数字
来源：http://ckq.ydzc1.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aek.daria6918.cn

[S51] C++：显式类型转换
来源：http://ywj.fzhhl.top

static_cast<double>(a) / b
来源：http://ujb.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://icc.wangdashe.top

int size() const noexcept { return n_; }
来源：http://ngy.ivvv.top

[S53] C++：移动语义
来源：http://cle.yuanzhike.top

std::vector<int> w = std::move(v);
来源：http://ewf.yuanzhike.top

[S54] C++：异常处理
来源：http://qkx.sweek.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ets.pengpengdd.cyou

[S55] C++：结构化绑定
来源：http://nlr.nanxinkj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fme.fktsv.cn

[S56] C++：optional
来源：http://qky.zdbjq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dhw.nanxinkj.top

[S57] C++：编译期常量
来源：http://iar.zhijiandao.cn

constexpr int N = 10;
来源：http://vkf.jyoumei.cn

[S58] C++：命名空间
来源：http://stm.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://fmj.daxiang520.top

[S59] C++：静态断言
来源：http://byr.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jyr.svipenyu.cn

[S60] C++：遍历并删除元素
来源：http://tlj.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vjw.hcnkem.com

================================================================================
来源：http://nhh.vqdsnc.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://klp.zhoulong.xyz

================================================================================
来源：http://lhu.zhixingplan.top

[T01] Kotlin：Hello World
来源：http://hny.guannengcc.top

println("Hello")
来源：http://ohv.jinqigfzy.top

[T02] Kotlin：变量
来源：http://usy.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vdb.xuanzx.com

[T03] Kotlin：字符串模板
来源：http://sas.jinqigufen.top

"值: $b"
来源：http://jxh.ydjk.org.cn

[T04] Kotlin：空安全
来源：http://opk.chenlongwang.top

val n: String? = null;  n?.length
来源：http://tel.hysaishi.cn

[T05] Kotlin：when 表达式
来源：http://xiu.fktsv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uzq.yj202588.top

[T06] Kotlin：集合映射
来源：http://hje.ydzc1.top

listOf(1, 2, 3).map { it * 2 }
来源：http://oxa.xingfuxueyuan.xyz

[T07] Kotlin：集合过滤
来源：http://qrs.fanxiaobao.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://bep.redwolf501.top

[T08] Kotlin：数据类
来源：http://vhj.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://qpj.52xcode.cn

[T09] Kotlin：扩展函数
来源：http://wbr.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://igc.uphjek.com

[T10] Kotlin：默认参数
来源：http://vhd.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oqw.hfpthk.cn


<!-- 参考信息 -->