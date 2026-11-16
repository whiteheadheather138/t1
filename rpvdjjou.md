代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://hgy.sxryk.cn

[R72] 等待端口就绪
来源：http://zrg.havefunace.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qaj.yj20258.top

[R73] 分割大日志
来源：http://hhc.zhiwuduotai.top

split -l 1000 big.log part_
来源：http://ere.zhiwuduotai.top

[R74] 批量重命名
来源：http://ogn.ehwqpu.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xad.aizwys.cn

[R75] 导出环境变量
来源：http://gnx.zhixingplan.top

export PATH="$HOME/bin:$PATH"
来源：http://ehs.vqdsnc.cn

[R76] 使用临时文件
来源：http://ggy.ybcxt.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wog.hnqzz.top

[R77] 读取用户输入
来源：http://rlx.gaohongyu789.top

read -rp "请输入: " ans
来源：http://djk.hcnkem.com

[R78] 交互式菜单
来源：http://nkd.ydjk.org.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tek.iojbl.cn

[R79] 解析命令行选项
来源：http://vdm.cucudq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jgj.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://tjh.ydjk.org.cn

time ./run.sh
来源：http://tww.quarkkingdee.top

================================================================================
来源：http://nmu.feifeiyinyue.top

S. C / C++ 专题
来源：http://aeg.tarul.cn

================================================================================
来源：http://pxr.shangyingyoupin.top

[S01] C：Hello World
来源：http://vgz.cdnleiting.top

#include <stdio.h>
来源：http://yyd.tian-w.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://eno.tarul.cn

[S02] C：变量与格式化输出
来源：http://oqr.andypj.xyz

int a = 10; printf("%d\n", a);
来源：http://qzu.yangfankeji.com

[S03] C：读入整数
来源：http://vlo.bbcook.cn

int x; scanf("%d", &x);
来源：http://abz.jinqigufen.top

[S04] C：字符串复制
来源：http://zpl.sxryk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://baq.haohaochexian.top

[S05] C：字符串长度
来源：http://eat.zhaomingkeji.xyz

strlen(s)
来源：http://gck.andypj.xyz

[S06] C：字符串比较
来源：http://rct.gzhubu.top

strcmp(a, b) == 0
来源：http://gzq.yongpay.top

[S07] C：数组遍历求和
来源：http://sms.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iog.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://bvc.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uoa.dianchejie.cn

[S09] C：结构体定义与初始化
来源：http://cbh.cashguo.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eho.gzhubu.top

[S10] C：指针与解引用
来源：http://cgb.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://awb.jinqigfzy.top

[S11] C：逐行读文件
来源：http://eib.zhongyouzk.top

FILE *f = fopen("a.txt", "r");
来源：http://zal.kuanghao11.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oew.shuidangran.top

fclose(f);
来源：http://kyp.fktsv.cn

[S12] C：写文件
来源：http://kwc.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xmi.sysykeji.top

[S13] C：宏定义
来源：http://ufc.ydzc1.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nnc.chenjidiqi.icu

[S14] C：枚举
来源：http://flm.zhiwuduotai.top

enum Color { RED, GREEN, BLUE };
来源：http://kwb.cdnleiting.top

[S15] C：类型转换
来源：http://blx.jiagoushi.top

(double) a / b
来源：http://eml.hysaishi.cn

[S16] C：位操作置位
来源：http://zaz.vqdsnc.cn

x |= (1 << 3);
来源：http://ipf.shuidangran.top

[S17] C：安全拼接字符串
来源：http://fji.nanxuanxn.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dsl.jyoumei.cn

[S18] C：命令行参数
来源：http://edo.jyoumei.cn

int main(int argc, char **argv)
来源：http://tpn.cucudq.cn

[S19] C：快速排序
来源：http://ljo.ybcxt.top

qsort(a, n, sizeof(int), cmp);
来源：http://wcw.ydjk.org.cn

[S20] C：二分查找
来源：http://fom.gaohongyu789.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dwv.jqgufenzy.top

[S21] C：字符类别判断
来源：http://ccp.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lkq.jyoumei.cn

[S22] C：字符串转数字
来源：http://nlk.wangdashe.top

atoi("42");  strtod("3.14", NULL);
来源：http://ake.nanxinkj.top

[S23] C：随机数
来源：http://ggt.yj20258888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nse.sufxvd.cn

[S24] C：获取本地时间
来源：http://awg.uphjek.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ecz.0kj1m.cn

[S25] C：内存拷贝
来源：http://yis.tarul.cn

memcpy(dst, src, n);
来源：http://qux.fktsv.cn

[S26] C：内存清零
来源：http://epj.cucudq.cn

memset(a, 0, sizeof a);
来源：http://ruo.quarkkingdee.top

[S27] C：定义常量
来源：http://bvi.cqqwz.cn

const double PI = 3.14159;
来源：http://een.xingfuxueyuan.xyz

[S28] C：静态变量
来源：http://hbp.jianghu66.top

static int counter = 0;
来源：http://qiw.sjlbkw.cn

[S29] C：变参函数
来源：http://fwp.jinghuilouyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vfw.cdnleiting.top

[S30] C：头文件保护
来源：http://bdi.guowangkeji.top

#ifndef X_H
来源：http://ksv.jianghu66.top

#define X_H
来源：http://jwt.ivvv.top

#endif
来源：http://htc.chenlongwang.top

[S31] C++：Hello World
来源：http://zqb.zhiwuduotai.top

#include <iostream>
来源：http://mwp.fehbvm.com

int main() { std::cout << "Hello\n"; }
来源：http://fbt.yfazqb.com

[S32] C++：字符串
来源：http://kyq.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://mhy.cdnleiting.top

[S33] C++：vector 增删
来源：http://sjw.shanyushiyangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dre.aibaodan.cn

[S34] C++：遍历 vector
来源：http://evk.nanxuanxn.top

for (auto &x : v) { std::cout << x; }
来源：http://irh.ehwqpu.com

[S35] C++：map
来源：http://mqp.hcnkem.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pks.yj202588.top

[S36] C++：unordered_map
来源：http://zln.bbcook.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zud.zycfv.cn

[S37] C++：set
来源：http://ugx.ybcxt.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vsb.ehwqpu.com

[S38] C++：排序
来源：http://wfo.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://dkc.cqqwz.cn

[S39] C++：自定义比较器排序
来源：http://wca.daria6918.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zzf.pycfn.com

[S40] C++：查找元素
来源：http://qdl.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jsi.pengpengdd.cyou

[S41] C++：类与构造函数
来源：http://iye.kuanghao11.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iwa.wangshuangyany.cn

[S42] C++：继承与虚函数
来源：http://wth.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://pcw.xziqi.cn

[S43] C++：智能指针
来源：http://afu.ybcxt.top

auto p = std::make_unique<int>(5);
来源：http://wtq.sweek.top

[S44] C++：引用传参
来源：http://bqy.aizwys.cn

void inc(int &x) { ++x; }
来源：http://ctx.vqdsnc.cn

[S45] C++：lambda
来源：http://kza.tianlin.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://ppl.xinyue.icu

[S46] C++：函数模板
来源：http://iww.wangshuangyany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lle.ehwqpu.com

[S47] C++：结构化绑定遍历
来源：http://aeu.chenzaomai.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wgi.gotoacloud.top

[S48] C++：逐行读文件
来源：http://zdt.tian-w.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fev.yonumen.top

while (std::getline(in, line)) { }
来源：http://rwa.haohaochexian.top

[S49] C++：写文件
来源：http://wfl.9152youxi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ent.birdmap.top

[S50] C++：格式化数字
来源：http://gcl.jqgfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gqw.9152youxi.cn

[S51] C++：显式类型转换
来源：http://fej.ydzc1.top

static_cast<double>(a) / b
来源：http://ska.xuetiantiany.cn

[S52] C++：const 与 noexcept
来源：http://vjv.yvedp.cn

int size() const noexcept { return n_; }
来源：http://wkz.yj20258888.top

[S53] C++：移动语义
来源：http://xah.guannengcc.top

std::vector<int> w = std::move(v);
来源：http://prm.ydjk.org.cn

[S54] C++：异常处理
来源：http://yhf.zdqjudy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://afr.havefunace.top

[S55] C++：结构化绑定
来源：http://oyf.xingfuxueyuan.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://mtd.cdnleiting.top

[S56] C++：optional
来源：http://ydw.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rwf.jiagoushi.top

[S57] C++：编译期常量
来源：http://nfm.yongpay.top

constexpr int N = 10;
来源：http://zgk.quarkkingdee.top

[S58] C++：命名空间
来源：http://oxe.svipenyu.cn

namespace ns { int f() { return 1; } }
来源：http://oei.yvedp.cn

[S59] C++：静态断言
来源：http://hif.gzhubu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://njx.yuxming.cn

[S60] C++：遍历并删除元素
来源：http://sgk.fengsongda.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pdh.xinyue.icu

================================================================================
来源：http://fjb.sweek.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://brr.epnwcf.com

================================================================================
来源：http://gnw.mhx1999.top

[T01] Kotlin：Hello World
来源：http://hsf.zhixingplan.top

println("Hello")
来源：http://sls.cdnleiting.top

[T02] Kotlin：变量
来源：http://eka.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://udc.tarul.cn

[T03] Kotlin：字符串模板
来源：http://ujh.jinghuilouyu.cn

"值: $b"
来源：http://spk.0kj1m.cn

[T04] Kotlin：空安全
来源：http://zoo.xinyue.icu

val n: String? = null;  n?.length
来源：http://uqo.jqgufenzy.top

[T05] Kotlin：when 表达式
来源：http://tzn.birdmap.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jcj.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://tlj.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wla.xylfe.cn

[T07] Kotlin：集合过滤
来源：http://kds.sufxvd.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://guw.yfazqb.com

[T08] Kotlin：数据类
来源：http://cnt.xinyue.icu

data class User(val name: String, val age: Int)
来源：http://drd.chenlongwang.top

[T09] Kotlin：扩展函数
来源：http://ycv.sjlbkw.cn

fun String.exclaim() = this + "!"
来源：http://rgo.xuanzx.com

[T10] Kotlin：默认参数
来源：http://vni.svipenyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://llk.cheryme.top

[T11] Kotlin：协程
来源：http://hua.fengsongda.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://veb.guannengcc.top

[T12] Kotlin：解构声明
来源：http://ejr.redwolf501.top

val (a, b) = Pair(1, 2)
来源：http://jsi.sxryk.cn

[T13] Kotlin：只读 Map
来源：http://jlf.yangfankeji.com

val m = mapOf("a" to 1)
来源：http://plz.ivvv.top

[T14] Kotlin：循环
来源：http://wsn.hongshengwenyu.top

for (i in 1..10) println(i)
来源：http://gta.yuxming.cn

[T15] Kotlin：接口
来源：http://jyb.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://ptw.yueranfly.top

[T16] Swift：Hello World
来源：http://ucs.yongpay.top

print("Hello")
来源：http://mtl.ywan-chungtsiang.top

[T17] Swift：变量与常量
来源：http://wbd.tianlin.xyz

var a = 1;  let b = 2
来源：http://zpw.guowangkeji.top

[T18] Swift：字符串插值
来源：http://bys.sjlbkw.cn

"值: \(b)"
来源：http://mpu.vqdsnc.cn

[T19] Swift：可选绑定
来源：http://xld.tanke756.top

if let n = opt { print(n) }
来源：http://dfc.dashuyun.cn

[T20] Swift：数组操作
来源：http://rsx.zhongyouzk.top

var a = [1, 2, 3];  a.append(4)
来源：http://ovj.meibo888.top

[T21] Swift：遍历
来源：http://wdo.xylfe.cn

for x in a { print(x) }
来源：http://top.fanxiaobao.xyz

[T22] Swift：字典
来源：http://zbq.xziqi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pxj.zhixingplan.top

[T23] Swift：函数
来源：http://ipb.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oof.yueranfly.top

[T24] Swift：闭包
来源：http://aac.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ekb.52xcode.cn

[T25] Swift：结构体
来源：http://yiz.nanxuanxn.top

struct P { var x: Int }
来源：http://rtp.zhijiandao.cn

[T26] Swift：类与重写
来源：http://qzu.sxryk.cn

class A: Base { override func f() {} }
来源：http://acj.nanxuanxn.top

[T27] Swift：错误处理
来源：http://oyk.ydzc1.top

do { try f() } catch { print(error) }
来源：http://kag.dashuyun.cn

[T28] Swift：枚举
来源：http://ojc.jiagoushi.top

enum Color { case red, green }
来源：http://fwp.uphjek.com

[T29] Swift：guard 提前返回
来源：http://bku.shzxlz.cn

guard let x = opt else { return }
来源：http://aai.ydzc1.top

[T30] Swift：协议
来源：http://osg.bjfxy.top

protocol Shape { func area() -> Double }
来源：http://lfk.chenjidiqi.icu

[T31] Lua：Hello World
来源：http://lpo.bbcook.cn

print("Hello")
来源：http://ese.havefunace.top

[T32] Lua：局部变量
来源：http://zfr.zhongyouzk.top

local a = 1
来源：http://gqp.0kj1m.cn

[T33] Lua：表（数组）
来源：http://nti.snrcjt.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hgi.bjfxy.top

[T34] Lua：遍历表
来源：http://hbw.ywan-chungtsiang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://sxt.snrcjt.cn

[T35] Lua：字典表
来源：http://gyg.nwbrower.top

local d = { a = 1 };  d.b = 2
来源：http://wtj.zhongyouzk.top

[T36] Lua：函数
来源：http://hns.zhijiandao.cn

function add(a, b) return a + b end
来源：http://oux.xinyue.icu

[T37] Lua：字符串拼接
来源：http://pfl.iojbl.cn

"a" .. "b"
来源：http://rvr.smart0.xyz

[T38] Lua：条件
来源：http://lxs.yfazqb.com

if x > 0 then print("正") end
来源：http://tkr.sufxvd.cn

[T39] Lua：模式匹配
来源：http://wyt.gaohongyu789.top

string.find(s, "%d+")
来源：http://dqe.guowangkeji.top

[T40] Lua：元表
来源：http://dld.fehbvm.com

setmetatable({}, { __index = base })
来源：http://gku.hywenlv.cn

[T41] Perl：Hello World
来源：http://lks.fehbvm.com

print "Hello\n";
来源：http://gvv.daria6918.cn

[T42] Perl：变量类型
来源：http://yhb.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cwo.sweek.top

[T43] Perl：字符串插值
来源：http://jgg.fanxiaobao.xyz

"值: $a"
来源：http://znt.epnwcf.com

[T44] Perl：条件
来源：http://ftb.wangdashe.top

if ($a > 0) { print "正"; }
来源：http://sfy.hnxiangtu.top

[T45] Perl：数组遍历
来源：http://toq.yj20258.top

for my $x (@arr) { print $x; }
来源：http://kpr.ivvv.top

[T46] Perl：哈希操作
来源：http://rnx.xingfuxueyuan.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rpj.hesvh.cn

[T47] Perl：正则捕获
来源：http://pde.dianchejie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cqc.quarkkingdee.top

[T48] Perl：正则替换
来源：http://wjn.gogol.net.cn

$s =~ s/old/new/g;
来源：http://brd.sweek.top

[T49] Perl：函数
来源：http://jvm.dashuyun.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fyk.tianlin.xyz

[T50] Perl：逐行读文件
来源：http://mfm.vehdjk.com

open my $fh, "<", "a.txt" or die $!;
来源：http://ntk.bjfxy.top

while (my $line = <$fh>) { print $line; }
来源：http://upm.gzhubu.top

[T51] Scala：Hello World
来源：http://mod.nanxinkj.top

println("Hello")
来源：http://ynk.yj202588.top

[T52] Scala：变量
来源：http://dcv.hysaishi.cn

val a = 1;  var b = 2
来源：http://djc.yongpay.top

[T53] Scala：字符串插值
来源：http://dqo.guowangkeji.top

s"值: $b"
来源：http://lek.yueranfly.top

[T54] Scala：集合映射
来源：http://vgs.yj202588.top

List(1, 2, 3).map(_ * 2)
来源：http://odj.hesvh.cn

[T55] Scala：集合过滤
来源：http://lqk.chenjidiqi.icu

List(1, 2, 3).filter(_ > 1)
来源：http://uvb.gotoacloud.top

[T56] Scala：样例类
来源：http://edj.ydzc1.top

case class User(name: String, age: Int)
来源：http://eca.bjfxy.top

[T57] Scala：模式匹配
来源：http://zzw.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hin.smart0.xyz

[T58] Scala：函数定义
来源：http://okm.jinyuanbaomall.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oht.sufxvd.cn

[T59] Scala：循环
来源：http://wcp.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://cff.svipenyu.cn

[T60] Scala：折叠
来源：http://mua.pycfn.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wvb.yongpay.top

================================================================================
来源：http://hwd.52xcode.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bcd.zycfv.cn

================================================================================
来源：http://xro.sysykeji.top

[U01] Py：创建虚拟环境
来源：http://rva.havefunace.top

python -m venv .venv && source .venv/bin/activate
来源：http://aux.bjfxy.top

[U02] Py：导出 / 安装依赖
来源：http://tbg.dianchejie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zqw.haohaochexian.top

[U03] Py：加载 .env 配置
来源：http://fhe.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://bba.yanxiufei.cn

[U04] Py：变量调试打印
来源：http://pvh.shanyushiyangtech.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hyr.vqdsnc.cn

[U05] Py：列表去重且保序
来源：http://zgr.fktsv.cn

list(dict.fromkeys(arr))
来源：http://eqd.vehdjk.com

[U06] Py：合并两个字典
来源：http://avw.shanyushiyangkeji.top

{**a, **b}
来源：http://msw.nanxuanxn.top

[U07] Py：反转字典键值
来源：http://nyc.meibo888.top

{v: k for k, v in d.items()}
来源：http://ijt.pycfn.com

[U08] Py：展平二维列表
来源：http://pim.zdbjq.cn

[y for x in nested for y in x]
来源：http://guq.wangshuangyany.cn

[U09] Py：字典取最大值的键
来源：http://myy.cqqwz.cn

max(d, key=d.get)
来源：http://jyf.vehdjk.com

[U10] Py：按值排序字典
来源：http://jgc.haohaochexian.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wfh.sufxvd.cn

[U11] Py：生成器表达式
来源：http://esi.iojbl.cn

(x * 2 for x in arr)
来源：http://ekn.zhijiandao.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jmc.cqqwz.cn

Counter(arr).most_common(3)
来源：http://ebh.xinyue.icu


<!-- 参考信息 -->