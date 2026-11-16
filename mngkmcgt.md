代发 wailian999

ssh user@host 'uptime'
来源：http://zbt.ywan-chungtsiang.top

[R58] 下载文件
来源：http://uoz.xinyue.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fnd.yanxiufei.cn

[R59] 发 POST JSON
来源：http://pxp.dashuyun.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zwx.sweek.top

[R60] 只看 HTTP 状态码
来源：http://wzg.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yfe.jqgufenzy.top

[R61] 磁盘占用
来源：http://noq.bbcook.cn

df -h;  du -sh *
来源：http://gdu.fanxiaobao.xyz

[R62] 找最占空间的文件
来源：http://vmq.sxryk.cn

du -ah . | sort -rh | head -10
来源：http://qpi.zhijiandao.cn

[R63] 内存与进程
来源：http://aoy.gotoacloud.top

free -h;  ps aux | grep nginx
来源：http://ull.fktsv.cn

[R64] 结束进程
来源：http://mgu.svipenyu.cn

kill -9 $(pgrep -f app.py)
来源：http://ugf.tianlin.xyz

[R65] 查看端口占用
来源：http://znw.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vbk.nanxuanxn.top

[R66] 定时任务
来源：http://dix.hnqzz.top

crontab -e;  crontab -l
来源：http://lxy.jinghuilouyu.cn

[R67] 生成随机十六进制串
来源：http://hzr.xuanzx.com

openssl rand -hex 16
来源：http://xhx.xingfuxueyuan.xyz

[R68] 计算文件校验值
来源：http://iii.gotoacloud.top

sha256sum a.txt;  md5sum a.txt
来源：http://riq.yuxming.cn

[R69] 生成随机密码
来源：http://hzy.yanxiufei.cn

head -c 16 /dev/urandom | base64
来源：http://nfw.zdbjq.cn

[R70] 时间戳与互转
来源：http://duq.ppjwa.cn

date +%s;  date -d @1700000000
来源：http://kgg.fktsv.cn

[R71] 日期格式化
来源：http://syc.yj202588.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dss.chenlongwang.top

[R72] 等待端口就绪
来源：http://ely.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://jha.ctjpmb.com

[R73] 分割大日志
来源：http://hdq.vqdsnc.cn

split -l 1000 big.log part_
来源：http://llc.shanyushiyangkeji.top

[R74] 批量重命名
来源：http://xle.fanxiaobao.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ujt.sweek.top

[R75] 导出环境变量
来源：http://bzy.ydjk.org.cn

export PATH="$HOME/bin:$PATH"
来源：http://pmx.hammf.cn

[R76] 使用临时文件
来源：http://yjo.cheryme.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://azd.vehdjk.com

[R77] 读取用户输入
来源：http://srq.aizwys.cn

read -rp "请输入: " ans
来源：http://ecd.aizwys.cn

[R78] 交互式菜单
来源：http://usz.jinghuilouyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://iph.zhoulong.xyz

[R79] 解析命令行选项
来源：http://yrv.fktsv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vev.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://qch.jinqigfzy.top

time ./run.sh
来源：http://lyf.0kj1m.cn

================================================================================
来源：http://ujb.shangyingyoupin.top

S. C / C++ 专题
来源：http://yhz.xinyue.icu

================================================================================
来源：http://suj.xingfuxueyuan.xyz

[S01] C：Hello World
来源：http://slh.tarul.cn

#include <stdio.h>
来源：http://egb.wangshuangyany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hfi.sufxvd.cn

[S02] C：变量与格式化输出
来源：http://wtb.ydjk.org.cn

int a = 10; printf("%d\n", a);
来源：http://cym.sufxvd.cn

[S03] C：读入整数
来源：http://kzo.hammf.cn

int x; scanf("%d", &x);
来源：http://qxv.ivvv.top

[S04] C：字符串复制
来源：http://zjj.tarul.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eqn.yongpay.top

[S05] C：字符串长度
来源：http://yha.redwolf501.top

strlen(s)
来源：http://akl.yonumen.top

[S06] C：字符串比较
来源：http://crm.daxiang520.top

strcmp(a, b) == 0
来源：http://jik.hnqzz.top

[S07] C：数组遍历求和
来源：http://rkz.jianghu66.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yma.daxiang520.top

[S08] C：动态内存分配与释放
来源：http://fbn.zhijiandao.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fho.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://wgd.aibaodan.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jjn.yj202588.top

[S10] C：指针与解引用
来源：http://pta.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://nfu.jqgufenzy.top

[S11] C：逐行读文件
来源：http://dzh.cdnleiting.top

FILE *f = fopen("a.txt", "r");
来源：http://uru.iojbl.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dcd.sxryk.cn

fclose(f);
来源：http://lqu.tian-w.cn

[S12] C：写文件
来源：http://jfu.tianlin.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xth.cucudq.cn

[S13] C：宏定义
来源：http://sbt.yueranfly.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://agz.zhiwuduotai.top

[S14] C：枚举
来源：http://xbg.zdbjq.cn

enum Color { RED, GREEN, BLUE };
来源：http://ojg.fanxiaobao.xyz

[S15] C：类型转换
来源：http://avp.shangyingyoupin.top

(double) a / b
来源：http://ejj.guannengcc.top

[S16] C：位操作置位
来源：http://qsx.dashuyun.cn

x |= (1 << 3);
来源：http://djh.fengsongda.top

[S17] C：安全拼接字符串
来源：http://jtf.hnxiangtu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nub.fehbvm.com

[S18] C：命令行参数
来源：http://ovf.yj20258.top

int main(int argc, char **argv)
来源：http://zxp.zhongyouzk.top

[S19] C：快速排序
来源：http://voq.hnxiangtu.top

qsort(a, n, sizeof(int), cmp);
来源：http://eig.jianghu66.top

[S20] C：二分查找
来源：http://cda.ydjk.org.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ymw.nanxuanxn.top

[S21] C：字符类别判断
来源：http://qru.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cwp.yj20258888.top

[S22] C：字符串转数字
来源：http://sjp.sweek.top

atoi("42");  strtod("3.14", NULL);
来源：http://ndz.ehwqpu.com

[S23] C：随机数
来源：http://cwx.zhongyouzk.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xfh.gaohongyu789.top

[S24] C：获取本地时间
来源：http://njp.aibaodan.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gqc.iojbl.cn

[S25] C：内存拷贝
来源：http://duf.gogol.net.cn

memcpy(dst, src, n);
来源：http://fhs.ctjpmb.com

[S26] C：内存清零
来源：http://nuj.shanyushiyangtech.top

memset(a, 0, sizeof a);
来源：http://cur.zhijiandao.cn

[S27] C：定义常量
来源：http://psu.chenlongwang.top

const double PI = 3.14159;
来源：http://tuc.zhengqikj.top

[S28] C：静态变量
来源：http://eny.sjlbkw.cn

static int counter = 0;
来源：http://svn.aizwys.cn

[S29] C：变参函数
来源：http://tac.gogol.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://atw.ivvv.top

[S30] C：头文件保护
来源：http://ghg.ydjk.org.cn

#ifndef X_H
来源：http://osx.ivvv.top

#define X_H
来源：http://scn.hfpthk.cn

#endif
来源：http://kdb.zhongyouzk.top

[S31] C++：Hello World
来源：http://qyl.birdmap.top

#include <iostream>
来源：http://dsy.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://fqf.haohaochexian.top

[S32] C++：字符串
来源：http://ijc.xziqi.cn

std::string s = "hi";  s += "!";
来源：http://cix.cheryme.top

[S33] C++：vector 增删
来源：http://ylz.yj202588.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zai.aizwys.cn

[S34] C++：遍历 vector
来源：http://qrk.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://klw.zhaomingkeji.xyz

[S35] C++：map
来源：http://crb.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zck.yj20258888.top

[S36] C++：unordered_map
来源：http://rmc.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dnw.ywan-chungtsiang.top

[S37] C++：set
来源：http://iij.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oyy.tian-w.cn

[S38] C++：排序
来源：http://elx.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://kym.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://uvd.shuidangran.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ity.jiagoushi.top

[S40] C++：查找元素
来源：http://pvx.aibaodan.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blg.hongshengwenyu.top

[S41] C++：类与构造函数
来源：http://flt.bjfxy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sgn.bbcook.cn

[S42] C++：继承与虚函数
来源：http://faj.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://llp.hysaishi.cn

[S43] C++：智能指针
来源：http://pzq.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://jqw.chenzaomai.com

[S44] C++：引用传参
来源：http://fsy.cheryme.top

void inc(int &x) { ++x; }
来源：http://ezy.zycfv.cn

[S45] C++：lambda
来源：http://zwq.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://urw.hnqzz.top

[S46] C++：函数模板
来源：http://eee.vqdsnc.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://whr.snrcjt.cn

[S47] C++：结构化绑定遍历
来源：http://nyl.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dgf.shanyushiyangtech.top

[S48] C++：逐行读文件
来源：http://zit.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://yqu.fengsongda.top

while (std::getline(in, line)) { }
来源：http://jdq.fzhhl.top

[S49] C++：写文件
来源：http://zfj.aizwys.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kma.jqgufenzy.top

[S50] C++：格式化数字
来源：http://fcl.zhoulong.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bdl.fzhhl.top

[S51] C++：显式类型转换
来源：http://nab.jlsjyb.cn

static_cast<double>(a) / b
来源：http://isa.yj20258.top

[S52] C++：const 与 noexcept
来源：http://ytg.zhixingplan.top

int size() const noexcept { return n_; }
来源：http://lpt.tanke756.top

[S53] C++：移动语义
来源：http://evm.jinyuanbaomall.cn

std::vector<int> w = std::move(v);
来源：http://jkl.andypj.xyz

[S54] C++：异常处理
来源：http://arx.cdnleiting.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ubl.snrcjt.cn

[S55] C++：结构化绑定
来源：http://sun.sweek.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cdv.hysaishi.cn

[S56] C++：optional
来源：http://buc.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pcg.vqdsnc.cn

[S57] C++：编译期常量
来源：http://iww.zhengqikj.top

constexpr int N = 10;
来源：http://bim.yuanzhike.top

[S58] C++：命名空间
来源：http://ffd.xingfuxueyuan.xyz

namespace ns { int f() { return 1; } }
来源：http://paj.ydzc1.top

[S59] C++：静态断言
来源：http://kfk.jyoumei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dgp.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://pyb.chenlongwang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rhi.jqgufenzy.top

================================================================================
来源：http://gwl.ivvv.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://haw.gogol.net.cn

================================================================================
来源：http://lev.hnqzz.top

[T01] Kotlin：Hello World
来源：http://zzt.ybcxt.top

println("Hello")
来源：http://kap.yongpay.top

[T02] Kotlin：变量
来源：http://tmd.sufxvd.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://etk.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://txc.svipenyu.cn

"值: $b"
来源：http://rjl.shangyingyoupin.top

[T04] Kotlin：空安全
来源：http://lrj.sufxvd.cn

val n: String? = null;  n?.length
来源：http://oat.fzhhl.top

[T05] Kotlin：when 表达式
来源：http://lpy.gaohongyu789.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ssr.fengsongda.top

[T06] Kotlin：集合映射
来源：http://gsg.xziqi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://piu.ivvv.top

[T07] Kotlin：集合过滤
来源：http://bpr.ybcxt.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lid.ctjpmb.com

[T08] Kotlin：数据类
来源：http://gac.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://dbn.vqdsnc.cn

[T09] Kotlin：扩展函数
来源：http://rfc.birdmap.top

fun String.exclaim() = this + "!"
来源：http://ypx.ehwqpu.com

[T10] Kotlin：默认参数
来源：http://iwn.zhaomingkeji.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://jjs.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://voa.ctjpmb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://skh.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://edo.316326.xyz

val (a, b) = Pair(1, 2)
来源：http://kel.52xcode.cn

[T13] Kotlin：只读 Map
来源：http://vdn.yangfankeji.com

val m = mapOf("a" to 1)
来源：http://nsl.hfpthk.cn

[T14] Kotlin：循环
来源：http://tsm.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://gqk.yfazqb.com

[T15] Kotlin：接口
来源：http://fkj.fzhhl.top

interface Shape { fun area(): Double }
来源：http://zpb.ydjk.org.cn

[T16] Swift：Hello World
来源：http://epw.aibaodan.cn

print("Hello")
来源：http://zaq.cdnleiting.top

[T17] Swift：变量与常量
来源：http://omv.sxryk.cn

var a = 1;  let b = 2
来源：http://pyq.hfpthk.cn

[T18] Swift：字符串插值
来源：http://fhe.zhongyouzk.top

"值: \(b)"
来源：http://nwc.xuetiantiany.cn

[T19] Swift：可选绑定
来源：http://aiz.shangyingyoupin.top

if let n = opt { print(n) }
来源：http://qvf.nwbrower.top

[T20] Swift：数组操作
来源：http://kpn.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://qgw.yj202588.top

[T21] Swift：遍历
来源：http://hyp.ppjwa.cn

for x in a { print(x) }
来源：http://kif.sxryk.cn

[T22] Swift：字典
来源：http://upm.zdbjq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://coh.havefunace.top

[T23] Swift：函数
来源：http://vpq.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lig.tianlin.xyz

[T24] Swift：闭包
来源：http://jep.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://acj.jianghu66.top

[T25] Swift：结构体
来源：http://fkc.nwbrower.top

struct P { var x: Int }
来源：http://aoh.hfpthk.cn

[T26] Swift：类与重写
来源：http://txd.hnqzz.top

class A: Base { override func f() {} }
来源：http://dsi.xuetiantiany.cn

[T27] Swift：错误处理
来源：http://lsy.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://lej.birdmap.top

[T28] Swift：枚举
来源：http://kse.xuetiantiany.cn

enum Color { case red, green }
来源：http://rmw.hysaishi.cn

[T29] Swift：guard 提前返回
来源：http://mte.daxiang520.top

guard let x = opt else { return }
来源：http://nhm.yangfankeji.com

[T30] Swift：协议
来源：http://kjs.tanke756.top

protocol Shape { func area() -> Double }
来源：http://fwm.hongshengwenyu.top

[T31] Lua：Hello World
来源：http://lzs.iojbl.cn

print("Hello")
来源：http://sya.aibaodan.cn

[T32] Lua：局部变量
来源：http://qfo.svipenyu.cn

local a = 1
来源：http://fif.yvedp.cn

[T33] Lua：表（数组）
来源：http://loz.guannengcc.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kym.hongshengwenyu.top

[T34] Lua：遍历表
来源：http://qar.kuanghao11.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://edw.hcnkem.com

[T35] Lua：字典表
来源：http://ccp.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://zbl.jlsjyb.cn

[T36] Lua：函数
来源：http://siw.iojbl.cn

function add(a, b) return a + b end
来源：http://fkt.52xcode.cn

[T37] Lua：字符串拼接
来源：http://yze.mhx1999.top

"a" .. "b"
来源：http://jdh.yuxming.cn

[T38] Lua：条件
来源：http://hlj.yuanzhike.top

if x > 0 then print("正") end
来源：http://bym.ybcxt.top

[T39] Lua：模式匹配
来源：http://qdf.sysykeji.top

string.find(s, "%d+")
来源：http://vvm.jiagoushi.top

[T40] Lua：元表
来源：http://lnb.guannengcc.top

setmetatable({}, { __index = base })
来源：http://nfq.gzhubu.top

[T41] Perl：Hello World
来源：http://zut.zhijiandao.cn

print "Hello\n";
来源：http://mll.hnxiangtu.top

[T42] Perl：变量类型
来源：http://xmq.zhaomingkeji.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://frc.zhoulong.xyz

[T43] Perl：字符串插值
来源：http://hon.jinyuanbaomall.cn

"值: $a"
来源：http://fkn.fktsv.cn

[T44] Perl：条件
来源：http://brr.aizwys.cn

if ($a > 0) { print "正"; }
来源：http://cvm.bbcook.cn

[T45] Perl：数组遍历
来源：http://hca.bbcook.cn

for my $x (@arr) { print $x; }
来源：http://pin.jinqigufen.top

[T46] Perl：哈希操作
来源：http://umf.jinqigfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eno.dashuyun.cn

[T47] Perl：正则捕获
来源：http://dhy.shanyushiyangtech.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qhl.xziqi.cn

[T48] Perl：正则替换
来源：http://vff.shangyingyoupin.top

$s =~ s/old/new/g;
来源：http://kvg.uphjek.com

[T49] Perl：函数
来源：http://hav.shzxlz.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tet.9152youxi.cn

[T50] Perl：逐行读文件
来源：http://xzc.birdmap.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jmv.snrcjt.cn

while (my $line = <$fh>) { print $line; }
来源：http://hxq.vehdjk.com

[T51] Scala：Hello World
来源：http://lcz.0kj1m.cn

println("Hello")
来源：http://ugy.jiagoushi.top

[T52] Scala：变量
来源：http://hvb.shangyingyoupin.top

val a = 1;  var b = 2
来源：http://nym.yj20258888.top

[T53] Scala：字符串插值
来源：http://hjr.ppjwa.cn

s"值: $b"
来源：http://fsd.hcnkem.com

[T54] Scala：集合映射
来源：http://phs.ydzc1.top

List(1, 2, 3).map(_ * 2)
来源：http://mmt.sysykeji.top

[T55] Scala：集合过滤
来源：http://vga.havefunace.top

List(1, 2, 3).filter(_ > 1)
来源：http://iep.jinghuilouyu.cn

[T56] Scala：样例类
来源：http://jmn.yvedp.cn

case class User(name: String, age: Int)
来源：http://rbj.cucudq.cn

[T57] Scala：模式匹配
来源：http://mac.ydzc1.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zje.nanxinkj.top

[T58] Scala：函数定义
来源：http://jvv.cqqwz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fus.pycfn.com

[T59] Scala：循环
来源：http://jlx.bbcook.cn

for (i <- 1 to 10) println(i)
来源：http://jfy.zhiwuduotai.top

[T60] Scala：折叠
来源：http://dmb.gotoacloud.top


<!-- 参考信息 -->