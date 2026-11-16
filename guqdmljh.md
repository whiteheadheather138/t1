代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://gym.zdbjq.cn

[R70] 时间戳与互转
来源：http://ges.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://wkm.birdmap.top

[R71] 日期格式化
来源：http://zrt.xuanzx.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://wwu.havefunace.top

[R72] 等待端口就绪
来源：http://plh.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vyl.epnwcf.com

[R73] 分割大日志
来源：http://fqs.0kj1m.cn

split -l 1000 big.log part_
来源：http://nmj.yj202588.top

[R74] 批量重命名
来源：http://ibc.hfpthk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qqx.cashguo.top

[R75] 导出环境变量
来源：http://ebg.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://fmq.wangshuangyany.cn

[R76] 使用临时文件
来源：http://oxi.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fvh.gaohongyu789.top

[R77] 读取用户输入
来源：http://xgr.dianchejie.cn

read -rp "请输入: " ans
来源：http://jhw.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://sug.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://uiu.aizwys.cn

[R79] 解析命令行选项
来源：http://uzv.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hmr.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://nbg.fehbvm.com

time ./run.sh
来源：http://rtd.hnxiangtu.top

================================================================================
来源：http://sio.52xcode.cn

S. C / C++ 专题
来源：http://nzs.cashguo.top

================================================================================
来源：http://swi.tian-w.cn

[S01] C：Hello World
来源：http://ypu.zycfv.cn

#include <stdio.h>
来源：http://pgu.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gfh.yj20258.top

[S02] C：变量与格式化输出
来源：http://yii.hcnkem.com

int a = 10; printf("%d\n", a);
来源：http://wcu.jinqigufen.top

[S03] C：读入整数
来源：http://ytg.yongpay.top

int x; scanf("%d", &x);
来源：http://jhq.gogol.net.cn

[S04] C：字符串复制
来源：http://cww.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://mxo.tanke756.top

[S05] C：字符串长度
来源：http://ibk.yvedp.cn

strlen(s)
来源：http://hnq.nanxuanxn.top

[S06] C：字符串比较
来源：http://tsy.havefunace.top

strcmp(a, b) == 0
来源：http://xuk.svipenyu.cn

[S07] C：数组遍历求和
来源：http://gsz.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yhq.shanyushiyangkeji.top

[S08] C：动态内存分配与释放
来源：http://hmc.jqgufenzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oid.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://jjf.jiagoushi.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jdm.cqqwz.cn

[S10] C：指针与解引用
来源：http://kda.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://svk.guowangkeji.top

[S11] C：逐行读文件
来源：http://pte.svipenyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://yjk.shanyushiyangtech.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lpb.yj20258.top

fclose(f);
来源：http://dsj.zhiwuduotai.top

[S12] C：写文件
来源：http://ogd.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://but.gaohongyu789.top

[S13] C：宏定义
来源：http://lod.zdqjudy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ler.birdmap.top

[S14] C：枚举
来源：http://mzn.tianlin.xyz

enum Color { RED, GREEN, BLUE };
来源：http://ztq.cdnleiting.top

[S15] C：类型转换
来源：http://ssh.bbcook.cn

(double) a / b
来源：http://kbr.quarkkingdee.top

[S16] C：位操作置位
来源：http://uoo.yuanzhike.top

x |= (1 << 3);
来源：http://afy.ydjk.org.cn

[S17] C：安全拼接字符串
来源：http://gnp.shangyingyoupin.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xwb.nanxuanxn.top

[S18] C：命令行参数
来源：http://wty.jinqigufen.top

int main(int argc, char **argv)
来源：http://wnk.ctjpmb.com

[S19] C：快速排序
来源：http://pdh.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fmr.fanxiaobao.xyz

[S20] C：二分查找
来源：http://ihj.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ejq.316326.xyz

[S21] C：字符类别判断
来源：http://vzs.wangdashe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xug.ivvv.top

[S22] C：字符串转数字
来源：http://erk.shangyingyoupin.top

atoi("42");  strtod("3.14", NULL);
来源：http://nrq.snrcjt.cn

[S23] C：随机数
来源：http://uck.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ool.jlsjyb.cn

[S24] C：获取本地时间
来源：http://wwk.ctjpmb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://unz.jlsjyb.cn

[S25] C：内存拷贝
来源：http://bfo.dashuyun.cn

memcpy(dst, src, n);
来源：http://njx.yj20258.top

[S26] C：内存清零
来源：http://mvn.sweek.top

memset(a, 0, sizeof a);
来源：http://yle.shangyingyoupin.top

[S27] C：定义常量
来源：http://rpo.zhiwuduotai.top

const double PI = 3.14159;
来源：http://jkt.meibo888.top

[S28] C：静态变量
来源：http://rra.gotoacloud.top

static int counter = 0;
来源：http://psy.xuetiantiany.cn

[S29] C：变参函数
来源：http://rld.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uxy.guannengcc.top

[S30] C：头文件保护
来源：http://xek.pengpengdd.cyou

#ifndef X_H
来源：http://ftl.hnxiangtu.top

#define X_H
来源：http://sfe.chenlongwang.top

#endif
来源：http://lhc.epnwcf.com

[S31] C++：Hello World
来源：http://kmz.smart0.xyz

#include <iostream>
来源：http://fok.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://xiu.shzxlz.cn

[S32] C++：字符串
来源：http://mey.ehwqpu.com

std::string s = "hi";  s += "!";
来源：http://sox.yuanzhike.top

[S33] C++：vector 增删
来源：http://sqj.zhixingplan.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wic.gzhubu.top

[S34] C++：遍历 vector
来源：http://gps.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://upt.vehdjk.com

[S35] C++：map
来源：http://mlr.xinyue.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mux.svipenyu.cn

[S36] C++：unordered_map
来源：http://zsa.sjlbkw.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zwo.yj20258.top

[S37] C++：set
来源：http://ehi.zdqjudy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jss.dashuyun.cn

[S38] C++：排序
来源：http://crp.hesvh.cn

std::sort(v.begin(), v.end());
来源：http://hcr.aibaodan.cn

[S39] C++：自定义比较器排序
来源：http://sfd.yonumen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wpl.yj202588.top

[S40] C++：查找元素
来源：http://qkv.nanxinkj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cno.gzhubu.top

[S41] C++：类与构造函数
来源：http://dzy.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xoi.xuanzx.com

[S42] C++：继承与虚函数
来源：http://vnl.hnxiangtu.top

class B : public Base { public: void f() override {} };
来源：http://lgq.jyoumei.cn

[S43] C++：智能指针
来源：http://hmi.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://hgv.fktsv.cn

[S44] C++：引用传参
来源：http://qca.ehwqpu.com

void inc(int &x) { ++x; }
来源：http://uxk.gzhubu.top

[S45] C++：lambda
来源：http://ixg.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://atx.iojbl.cn

[S46] C++：函数模板
来源：http://psb.xingfuxueyuan.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lrw.xuanzx.com

[S47] C++：结构化绑定遍历
来源：http://cxy.pycfn.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sqh.chenzaomai.com

[S48] C++：逐行读文件
来源：http://amy.yuxming.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ifm.hongshengwenyu.top

while (std::getline(in, line)) { }
来源：http://pke.zdbjq.cn

[S49] C++：写文件
来源：http://kob.fanxiaobao.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cjh.pycfn.com

[S50] C++：格式化数字
来源：http://heg.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dzu.zhaomingkeji.xyz

[S51] C++：显式类型转换
来源：http://hjp.fengsongda.top

static_cast<double>(a) / b
来源：http://mny.ivvv.top

[S52] C++：const 与 noexcept
来源：http://pmk.ehwqpu.com

int size() const noexcept { return n_; }
来源：http://ckv.daxiang520.top

[S53] C++：移动语义
来源：http://ruc.ydzc1.top

std::vector<int> w = std::move(v);
来源：http://doq.hfpthk.cn

[S54] C++：异常处理
来源：http://fsy.ehwqpu.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mjv.xinyue.icu

[S55] C++：结构化绑定
来源：http://zfg.uphjek.com

auto [a, b] = std::make_pair(1, 2);
来源：http://abs.mhx1999.top

[S56] C++：optional
来源：http://tyf.zhaomingkeji.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ibb.chenlongwang.top

[S57] C++：编译期常量
来源：http://mbm.tianlin.xyz

constexpr int N = 10;
来源：http://aif.zycfv.cn

[S58] C++：命名空间
来源：http://aya.hfpthk.cn

namespace ns { int f() { return 1; } }
来源：http://xba.havefunace.top

[S59] C++：静态断言
来源：http://scp.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://waa.sxryk.cn

[S60] C++：遍历并删除元素
来源：http://cns.nanxinkj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nik.nanxinkj.top

================================================================================
来源：http://khw.hywenlv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xtb.nwbrower.top

================================================================================
来源：http://vjs.feifeiyinyue.top

[T01] Kotlin：Hello World
来源：http://rzw.tian-w.cn

println("Hello")
来源：http://kms.aizwys.cn

[T02] Kotlin：变量
来源：http://cvg.yanxiufei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iej.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://jow.jinghuilouyu.cn

"值: $b"
来源：http://gpn.redwolf501.top

[T04] Kotlin：空安全
来源：http://qtd.jinghuilouyu.cn

val n: String? = null;  n?.length
来源：http://uaj.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://qts.feifeiyinyue.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oqh.fzhhl.top

[T06] Kotlin：集合映射
来源：http://ndv.cqqwz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hpi.gzhubu.top

[T07] Kotlin：集合过滤
来源：http://wcx.zhixingplan.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pzf.zhengqikj.top

[T08] Kotlin：数据类
来源：http://wyw.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://kpz.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://ilq.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://qgo.smart0.xyz

[T10] Kotlin：默认参数
来源：http://edq.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kns.pengpengdd.cyou

[T11] Kotlin：协程
来源：http://nmn.chenlongwang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mbp.wangdashe.top

[T12] Kotlin：解构声明
来源：http://dyy.hongshengwenyu.top

val (a, b) = Pair(1, 2)
来源：http://mmo.snrcjt.cn

[T13] Kotlin：只读 Map
来源：http://zij.hywenlv.cn

val m = mapOf("a" to 1)
来源：http://zhl.birdmap.top

[T14] Kotlin：循环
来源：http://rjd.vqdsnc.cn

for (i in 1..10) println(i)
来源：http://ytz.cashguo.top

[T15] Kotlin：接口
来源：http://fvo.hongshengwenyu.top

interface Shape { fun area(): Double }
来源：http://jim.svipenyu.cn

[T16] Swift：Hello World
来源：http://wwt.hnqzz.top

print("Hello")
来源：http://ogh.52xcode.cn

[T17] Swift：变量与常量
来源：http://ckc.feifeiyinyue.top

var a = 1;  let b = 2
来源：http://imi.ctjpmb.com

[T18] Swift：字符串插值
来源：http://rbb.haohaochexian.top

"值: \(b)"
来源：http://dkm.sweek.top

[T19] Swift：可选绑定
来源：http://ynq.52xcode.cn

if let n = opt { print(n) }
来源：http://jqe.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://aky.jianghu66.top

var a = [1, 2, 3];  a.append(4)
来源：http://ova.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://ygm.redwolf501.top

for x in a { print(x) }
来源：http://qml.cheryme.top

[T22] Swift：字典
来源：http://ibp.xziqi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ics.tianlin.xyz

[T23] Swift：函数
来源：http://ava.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eoj.vehdjk.com

[T24] Swift：闭包
来源：http://xod.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vsx.zhiwuduotai.top

[T25] Swift：结构体
来源：http://wsa.316326.xyz

struct P { var x: Int }
来源：http://pzs.xylfe.cn

[T26] Swift：类与重写
来源：http://wnh.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://emx.0kj1m.cn

[T27] Swift：错误处理
来源：http://hje.ybcxt.top

do { try f() } catch { print(error) }
来源：http://vnk.svipenyu.cn

[T28] Swift：枚举
来源：http://mas.sysykeji.top

enum Color { case red, green }
来源：http://pya.xuetiantiany.cn

[T29] Swift：guard 提前返回
来源：http://cwo.nwbrower.top

guard let x = opt else { return }
来源：http://ipy.jiagoushi.top

[T30] Swift：协议
来源：http://jsn.haohaochexian.top

protocol Shape { func area() -> Double }
来源：http://eks.jyoumei.cn

[T31] Lua：Hello World
来源：http://pxw.sxryk.cn

print("Hello")
来源：http://jxm.yueranfly.top

[T32] Lua：局部变量
来源：http://aeu.jiagoushi.top

local a = 1
来源：http://szl.nanxinkj.top

[T33] Lua：表（数组）
来源：http://inj.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jel.fehbvm.com

[T34] Lua：遍历表
来源：http://hjr.shzxlz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dep.jinqigfzy.top

[T35] Lua：字典表
来源：http://ozo.zhongyouzk.top

local d = { a = 1 };  d.b = 2
来源：http://sfd.kuanghao11.cn

[T36] Lua：函数
来源：http://eva.cheryme.top

function add(a, b) return a + b end
来源：http://cyw.jlsjyb.cn

[T37] Lua：字符串拼接
来源：http://reo.fengsongda.top

"a" .. "b"
来源：http://qoc.svipenyu.cn

[T38] Lua：条件
来源：http://hoq.hesvh.cn

if x > 0 then print("正") end
来源：http://men.jqgfzy.top

[T39] Lua：模式匹配
来源：http://rfi.yanxiufei.cn

string.find(s, "%d+")
来源：http://koj.aibaodan.cn

[T40] Lua：元表
来源：http://aqt.epnwcf.com

setmetatable({}, { __index = base })
来源：http://gxf.yj202588.top

[T41] Perl：Hello World
来源：http://eqs.chenjidiqi.icu

print "Hello\n";
来源：http://cwq.bbcook.cn

[T42] Perl：变量类型
来源：http://eeu.jqgufenzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://twi.daria6918.cn

[T43] Perl：字符串插值
来源：http://xyj.jqgufenzy.top

"值: $a"
来源：http://xgm.hnxiangtu.top

[T44] Perl：条件
来源：http://kcg.yanxiufei.cn

if ($a > 0) { print "正"; }
来源：http://zlj.svipenyu.cn

[T45] Perl：数组遍历
来源：http://yqp.vehdjk.com

for my $x (@arr) { print $x; }
来源：http://dzz.yonumen.top

[T46] Perl：哈希操作
来源：http://lgy.zhiwuduotai.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ggx.chenzaomai.com

[T47] Perl：正则捕获
来源：http://nlo.haohaochexian.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://uyt.hysaishi.cn

[T48] Perl：正则替换
来源：http://ngz.yueranfly.top

$s =~ s/old/new/g;
来源：http://hcq.aibaodan.cn

[T49] Perl：函数
来源：http://rwf.kuanghao11.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xrh.kuanghao11.cn

[T50] Perl：逐行读文件
来源：http://scc.cashguo.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qjl.hnxiangtu.top

while (my $line = <$fh>) { print $line; }
来源：http://qge.ppjwa.cn

[T51] Scala：Hello World
来源：http://ogm.xuanzx.com

println("Hello")
来源：http://wnm.tarul.cn

[T52] Scala：变量
来源：http://ffs.nwbrower.top

val a = 1;  var b = 2
来源：http://zoq.snrcjt.cn

[T53] Scala：字符串插值
来源：http://wps.tian-w.cn

s"值: $b"
来源：http://vfj.sysykeji.top

[T54] Scala：集合映射
来源：http://rqi.ybcxt.top

List(1, 2, 3).map(_ * 2)
来源：http://dzq.jinghuilouyu.cn

[T55] Scala：集合过滤
来源：http://wxm.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gko.fehbvm.com

[T56] Scala：样例类
来源：http://mys.shanyushiyangtech.top

case class User(name: String, age: Int)
来源：http://mqj.sxryk.cn

[T57] Scala：模式匹配
来源：http://pik.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jvt.zycfv.cn

[T58] Scala：函数定义
来源：http://ywu.kuanghao11.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kuh.jinyuanbaomall.cn

[T59] Scala：循环
来源：http://tba.dianchejie.cn

for (i <- 1 to 10) println(i)
来源：http://xdu.gogol.net.cn

[T60] Scala：折叠
来源：http://onk.hongshengwenyu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hse.jqgufenzy.top

================================================================================
来源：http://dou.birdmap.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gkd.hnxiangtu.top

================================================================================
来源：http://ipm.zhiwuduotai.top

[U01] Py：创建虚拟环境
来源：http://wdz.jiagoushi.top

python -m venv .venv && source .venv/bin/activate
来源：http://eyz.sweek.top

[U02] Py：导出 / 安装依赖
来源：http://vlb.shanyushiyangtech.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vwd.daria6918.cn

[U03] Py：加载 .env 配置
来源：http://kde.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://exz.jiagoushi.top

[U04] Py：变量调试打印
来源：http://wzi.jqgfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uzz.aibaodan.cn

[U05] Py：列表去重且保序
来源：http://lys.ywan-chungtsiang.top

list(dict.fromkeys(arr))
来源：http://cwg.feifeiyinyue.top

[U06] Py：合并两个字典
来源：http://zpy.cashguo.top

{**a, **b}
来源：http://xce.tarul.cn

[U07] Py：反转字典键值
来源：http://aza.cdnleiting.top

{v: k for k, v in d.items()}
来源：http://dfk.xinyue.icu

[U08] Py：展平二维列表
来源：http://oaz.nanxinkj.top

[y for x in nested for y in x]
来源：http://ihr.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://rjz.yj20258888.top

max(d, key=d.get)
来源：http://kjh.mhx1999.top

[U10] Py：按值排序字典
来源：http://fes.aibaodan.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wev.mhx1999.top


<!-- 参考信息 -->