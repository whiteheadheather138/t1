代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://muq.yangfankeji.com

[R70] 时间戳与互转
来源：http://bui.hnqzz.top

date +%s;  date -d @1700000000
来源：http://qeb.zhoulong.xyz

[R71] 日期格式化
来源：http://lqq.hnxiangtu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kui.316326.xyz

[R72] 等待端口就绪
来源：http://bus.zdqjudy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zjg.52xcode.cn

[R73] 分割大日志
来源：http://xoz.yfazqb.com

split -l 1000 big.log part_
来源：http://wtz.zhijiandao.cn

[R74] 批量重命名
来源：http://jio.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tnc.aizwys.cn

[R75] 导出环境变量
来源：http://ihx.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://gpz.ctjpmb.com

[R76] 使用临时文件
来源：http://upn.bbcook.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://isy.zhongyouzk.top

[R77] 读取用户输入
来源：http://rpo.quarkkingdee.top

read -rp "请输入: " ans
来源：http://kmm.jianghu66.top

[R78] 交互式菜单
来源：http://bca.zhiwuduotai.top

select opt in a b c; do echo "$opt"; break; done
来源：http://omf.yuxming.cn

[R79] 解析命令行选项
来源：http://qzv.jiagoushi.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rde.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://chd.ivvv.top

time ./run.sh
来源：http://quo.jinqigufen.top

================================================================================
来源：http://qzd.jqgfzy.top

S. C / C++ 专题
来源：http://vwo.zdqjudy.top

================================================================================
来源：http://pkf.zhiwuduotai.top

[S01] C：Hello World
来源：http://ovg.mhx1999.top

#include <stdio.h>
来源：http://vsw.52xcode.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yhm.ybcxt.top

[S02] C：变量与格式化输出
来源：http://mia.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://vgi.uphjek.com

[S03] C：读入整数
来源：http://wti.uphjek.com

int x; scanf("%d", &x);
来源：http://ovc.vqdsnc.cn

[S04] C：字符串复制
来源：http://mdf.zhongyouzk.top

char dst[32]; strcpy(dst, "hi");
来源：http://hly.yfazqb.com

[S05] C：字符串长度
来源：http://mad.daxiang520.top

strlen(s)
来源：http://noz.gogol.net.cn

[S06] C：字符串比较
来源：http://aev.andypj.xyz

strcmp(a, b) == 0
来源：http://clp.tarul.cn

[S07] C：数组遍历求和
来源：http://umv.gogol.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lmq.shanyushiyangtech.top

[S08] C：动态内存分配与释放
来源：http://ead.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zhj.sufxvd.cn

[S09] C：结构体定义与初始化
来源：http://ayh.zycfv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jgq.jinqigufen.top

[S10] C：指针与解引用
来源：http://zlp.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://fej.smart0.xyz

[S11] C：逐行读文件
来源：http://odd.zhoulong.xyz

FILE *f = fopen("a.txt", "r");
来源：http://hnw.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://icw.jianghu66.top

fclose(f);
来源：http://rsv.fengsongda.top

[S12] C：写文件
来源：http://dek.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lpg.tarul.cn

[S13] C：宏定义
来源：http://kng.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zik.xylfe.cn

[S14] C：枚举
来源：http://hpt.jqgufenzy.top

enum Color { RED, GREEN, BLUE };
来源：http://esq.yongpay.top

[S15] C：类型转换
来源：http://nrj.smart0.xyz

(double) a / b
来源：http://pqa.zhixingplan.top

[S16] C：位操作置位
来源：http://hmk.yongpay.top

x |= (1 << 3);
来源：http://lck.yueranfly.top

[S17] C：安全拼接字符串
来源：http://kvf.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fdf.epnwcf.com

[S18] C：命令行参数
来源：http://fax.epnwcf.com

int main(int argc, char **argv)
来源：http://rue.yfazqb.com

[S19] C：快速排序
来源：http://ejo.jinqigfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://dtc.jqgfzy.top

[S20] C：二分查找
来源：http://wyi.mhx1999.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tdj.hfpthk.cn

[S21] C：字符类别判断
来源：http://djh.redwolf501.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://inc.tian-w.cn

[S22] C：字符串转数字
来源：http://xke.epnwcf.com

atoi("42");  strtod("3.14", NULL);
来源：http://elk.jinyuanbaomall.cn

[S23] C：随机数
来源：http://puc.bbcook.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://leo.xuetiantiany.cn

[S24] C：获取本地时间
来源：http://mtp.daria6918.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jxw.hfpthk.cn

[S25] C：内存拷贝
来源：http://ujg.andypj.xyz

memcpy(dst, src, n);
来源：http://kei.havefunace.top

[S26] C：内存清零
来源：http://azu.uphjek.com

memset(a, 0, sizeof a);
来源：http://wia.haohaochexian.top

[S27] C：定义常量
来源：http://ywa.haohaochexian.top

const double PI = 3.14159;
来源：http://fsa.yueranfly.top

[S28] C：静态变量
来源：http://vif.nwbrower.top

static int counter = 0;
来源：http://fif.sjlbkw.cn

[S29] C：变参函数
来源：http://sja.shuidangran.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dfs.jyoumei.cn

[S30] C：头文件保护
来源：http://zaa.fzhhl.top

#ifndef X_H
来源：http://uxy.xinyue.icu

#define X_H
来源：http://vxx.wangshuangyany.cn

#endif
来源：http://lvo.mhx1999.top

[S31] C++：Hello World
来源：http://xdz.hnqzz.top

#include <iostream>
来源：http://pkz.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://spl.zhongyouzk.top

[S32] C++：字符串
来源：http://kul.hammf.cn

std::string s = "hi";  s += "!";
来源：http://hwv.hnqzz.top

[S33] C++：vector 增删
来源：http://ssh.zhengqikj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rtp.smart0.xyz

[S34] C++：遍历 vector
来源：http://ncr.hongshengwenyu.top

for (auto &x : v) { std::cout << x; }
来源：http://yln.birdmap.top

[S35] C++：map
来源：http://wfh.fehbvm.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jgr.ydjk.org.cn

[S36] C++：unordered_map
来源：http://ivu.zhongyouzk.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fvv.nanxinkj.top

[S37] C++：set
来源：http://nyc.vqdsnc.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nhf.xziqi.cn

[S38] C++：排序
来源：http://wkf.tanke756.top

std::sort(v.begin(), v.end());
来源：http://mip.gotoacloud.top

[S39] C++：自定义比较器排序
来源：http://nwf.shangyingyoupin.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rbl.nanxuanxn.top

[S40] C++：查找元素
来源：http://mmm.shangyingyoupin.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oaf.snrcjt.cn

[S41] C++：类与构造函数
来源：http://prm.yj20258.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hih.0kj1m.cn

[S42] C++：继承与虚函数
来源：http://rvj.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://sap.jlsjyb.cn

[S43] C++：智能指针
来源：http://fjm.redwolf501.top

auto p = std::make_unique<int>(5);
来源：http://vim.yuanzhike.top

[S44] C++：引用传参
来源：http://zrg.jqgufenzy.top

void inc(int &x) { ++x; }
来源：http://ghs.xinyue.icu

[S45] C++：lambda
来源：http://jfi.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://alj.yj20258.top

[S46] C++：函数模板
来源：http://uwy.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oir.jianghu66.top

[S47] C++：结构化绑定遍历
来源：http://rtn.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yih.zhiwuduotai.top

[S48] C++：逐行读文件
来源：http://pul.zdbjq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lie.dashuyun.cn

while (std::getline(in, line)) { }
来源：http://pax.yanxiufei.cn

[S49] C++：写文件
来源：http://mpj.nwbrower.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lho.bbcook.cn

[S50] C++：格式化数字
来源：http://blg.nanxinkj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xqm.sxryk.cn

[S51] C++：显式类型转换
来源：http://yck.vehdjk.com

static_cast<double>(a) / b
来源：http://njb.shanyushiyangtech.top

[S52] C++：const 与 noexcept
来源：http://kjo.gaohongyu789.top

int size() const noexcept { return n_; }
来源：http://fer.fktsv.cn

[S53] C++：移动语义
来源：http://ixt.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://dmy.tanke756.top

[S54] C++：异常处理
来源：http://dko.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wva.cdnleiting.top

[S55] C++：结构化绑定
来源：http://twv.gaohongyu789.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lzu.shuidangran.top

[S56] C++：optional
来源：http://bpb.jqgufenzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jvk.yj20258888.top

[S57] C++：编译期常量
来源：http://xcf.cdnleiting.top

constexpr int N = 10;
来源：http://vzl.ivvv.top

[S58] C++：命名空间
来源：http://dpi.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://zos.pengpengdd.cyou

[S59] C++：静态断言
来源：http://lok.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yfz.316326.xyz

[S60] C++：遍历并删除元素
来源：http://lff.gaohongyu789.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qjp.jinqigufen.top

================================================================================
来源：http://zbj.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://egu.pengpengdd.cyou

================================================================================
来源：http://ewi.52xcode.cn

[T01] Kotlin：Hello World
来源：http://bif.yj20258888.top

println("Hello")
来源：http://vxy.yvedp.cn

[T02] Kotlin：变量
来源：http://hom.xuetiantiany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zwi.nanxinkj.top

[T03] Kotlin：字符串模板
来源：http://phc.sjlbkw.cn

"值: $b"
来源：http://ear.0kj1m.cn

[T04] Kotlin：空安全
来源：http://hbl.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://uoh.cashguo.top

[T05] Kotlin：when 表达式
来源：http://ddb.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lap.jinqigfzy.top

[T06] Kotlin：集合映射
来源：http://mlt.zhijiandao.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gtq.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://hiq.316326.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://puz.hesvh.cn

[T08] Kotlin：数据类
来源：http://ybi.xinyue.icu

data class User(val name: String, val age: Int)
来源：http://pwm.ivvv.top

[T09] Kotlin：扩展函数
来源：http://hkt.jinghuilouyu.cn

fun String.exclaim() = this + "!"
来源：http://onq.cdnleiting.top

[T10] Kotlin：默认参数
来源：http://cdx.hywenlv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://orp.xziqi.cn

[T11] Kotlin：协程
来源：http://stg.hnqzz.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lsk.yj202588.top

[T12] Kotlin：解构声明
来源：http://fwp.chenzaomai.com

val (a, b) = Pair(1, 2)
来源：http://eel.xingfuxueyuan.xyz

[T13] Kotlin：只读 Map
来源：http://ooo.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://yny.andypj.xyz

[T14] Kotlin：循环
来源：http://vjr.snrcjt.cn

for (i in 1..10) println(i)
来源：http://wdz.smart0.xyz

[T15] Kotlin：接口
来源：http://pum.yanxiufei.cn

interface Shape { fun area(): Double }
来源：http://mva.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://pyb.bjfxy.top

print("Hello")
来源：http://hns.jinghuilouyu.cn

[T17] Swift：变量与常量
来源：http://miv.yuxming.cn

var a = 1;  let b = 2
来源：http://bls.vehdjk.com

[T18] Swift：字符串插值
来源：http://tsu.ybcxt.top

"值: \(b)"
来源：http://uoy.smart0.xyz

[T19] Swift：可选绑定
来源：http://xxj.ivvv.top

if let n = opt { print(n) }
来源：http://llk.nanxinkj.top

[T20] Swift：数组操作
来源：http://tcf.epnwcf.com

var a = [1, 2, 3];  a.append(4)
来源：http://fcn.daxiang520.top

[T21] Swift：遍历
来源：http://tke.meibo888.top

for x in a { print(x) }
来源：http://ckt.hysaishi.cn

[T22] Swift：字典
来源：http://ccw.tarul.cn

var d = ["a": 1];  d["b"] = 2
来源：http://aip.shzxlz.cn

[T23] Swift：函数
来源：http://xcr.zhaomingkeji.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cwu.mhx1999.top

[T24] Swift：闭包
来源：http://vio.gzhubu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hrv.meibo888.top

[T25] Swift：结构体
来源：http://lhl.jinqigfzy.top

struct P { var x: Int }
来源：http://fsb.shanyushiyangtech.top

[T26] Swift：类与重写
来源：http://xbk.svipenyu.cn

class A: Base { override func f() {} }
来源：http://nqt.chenlongwang.top

[T27] Swift：错误处理
来源：http://ypz.quarkkingdee.top

do { try f() } catch { print(error) }
来源：http://pgk.gotoacloud.top

[T28] Swift：枚举
来源：http://tbh.hnxiangtu.top

enum Color { case red, green }
来源：http://ari.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://ore.hnxiangtu.top

guard let x = opt else { return }
来源：http://kst.sufxvd.cn

[T30] Swift：协议
来源：http://mkc.yueranfly.top

protocol Shape { func area() -> Double }
来源：http://iay.jinqigufen.top

[T31] Lua：Hello World
来源：http://nck.fzhhl.top

print("Hello")
来源：http://zhm.mhx1999.top

[T32] Lua：局部变量
来源：http://rby.yongpay.top

local a = 1
来源：http://wkh.ybcxt.top

[T33] Lua：表（数组）
来源：http://eaq.yonumen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ysv.yongpay.top

[T34] Lua：遍历表
来源：http://uyi.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://oyh.meibo888.top

[T35] Lua：字典表
来源：http://ter.meibo888.top

local d = { a = 1 };  d.b = 2
来源：http://mmj.hesvh.cn

[T36] Lua：函数
来源：http://sfr.yj20258.top

function add(a, b) return a + b end
来源：http://qrv.daxiang520.top

[T37] Lua：字符串拼接
来源：http://crw.meibo888.top

"a" .. "b"
来源：http://pdc.feifeiyinyue.top

[T38] Lua：条件
来源：http://oxf.wangshuangyany.cn

if x > 0 then print("正") end
来源：http://xex.ybcxt.top

[T39] Lua：模式匹配
来源：http://fnj.hcnkem.com

string.find(s, "%d+")
来源：http://xdw.yonumen.top

[T40] Lua：元表
来源：http://vcx.zhoulong.xyz

setmetatable({}, { __index = base })
来源：http://zia.zhixingplan.top

[T41] Perl：Hello World
来源：http://jhk.yj20258888.top

print "Hello\n";
来源：http://tzj.zdbjq.cn

[T42] Perl：变量类型
来源：http://psu.nwbrower.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uoz.nwbrower.top

[T43] Perl：字符串插值
来源：http://bty.gotoacloud.top

"值: $a"
来源：http://ypa.sjlbkw.cn

[T44] Perl：条件
来源：http://rrf.hywenlv.cn

if ($a > 0) { print "正"; }
来源：http://vhw.zdqjudy.top

[T45] Perl：数组遍历
来源：http://fta.hesvh.cn

for my $x (@arr) { print $x; }
来源：http://jdc.zdbjq.cn

[T46] Perl：哈希操作
来源：http://mzw.hfpthk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sfr.shanyushiyangkeji.top

[T47] Perl：正则捕获
来源：http://tal.chenzaomai.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://cpr.vehdjk.com

[T48] Perl：正则替换
来源：http://uje.nanxinkj.top

$s =~ s/old/new/g;
来源：http://vup.zycfv.cn

[T49] Perl：函数
来源：http://eic.jlsjyb.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yhf.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://mvp.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sai.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://koi.chenzaomai.com

[T51] Scala：Hello World
来源：http://nzi.ivvv.top

println("Hello")
来源：http://vtd.sweek.top

[T52] Scala：变量
来源：http://aaj.c1oappe.top

val a = 1;  var b = 2
来源：http://zbo.sysykeji.top

[T53] Scala：字符串插值
来源：http://waw.hesvh.cn

s"值: $b"
来源：http://uay.vqdsnc.cn

[T54] Scala：集合映射
来源：http://omr.feifeiyinyue.top

List(1, 2, 3).map(_ * 2)
来源：http://qdc.yanxiufei.cn

[T55] Scala：集合过滤
来源：http://bnh.feifeiyinyue.top

List(1, 2, 3).filter(_ > 1)
来源：http://ubu.cqqwz.cn

[T56] Scala：样例类
来源：http://pjf.fktsv.cn

case class User(name: String, age: Int)
来源：http://tdl.cucudq.cn

[T57] Scala：模式匹配
来源：http://rcn.gotoacloud.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fqy.tian-w.cn

[T58] Scala：函数定义
来源：http://txj.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://dds.hysaishi.cn

[T59] Scala：循环
来源：http://vzh.dianchejie.cn

for (i <- 1 to 10) println(i)
来源：http://rvc.hongshengwenyu.top

[T60] Scala：折叠
来源：http://vco.guowangkeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://czv.jyoumei.cn

================================================================================
来源：http://cbx.vqdsnc.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ttl.jinqigfzy.top

================================================================================
来源：http://ola.fehbvm.com

[U01] Py：创建虚拟环境
来源：http://mun.bjfxy.top

python -m venv .venv && source .venv/bin/activate
来源：http://moc.sweek.top

[U02] Py：导出 / 安装依赖
来源：http://hpm.zhaomingkeji.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hka.bbcook.cn

[U03] Py：加载 .env 配置
来源：http://mpd.iojbl.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qag.xuanzx.com

[U04] Py：变量调试打印
来源：http://ajq.hysaishi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kee.cheryme.top

[U05] Py：列表去重且保序
来源：http://gtb.zhijiandao.cn

list(dict.fromkeys(arr))
来源：http://bhb.xinyue.icu

[U06] Py：合并两个字典
来源：http://sih.bjfxy.top

{**a, **b}
来源：http://yyv.epnwcf.com

[U07] Py：反转字典键值
来源：http://xln.yfazqb.com

{v: k for k, v in d.items()}
来源：http://qrs.smart0.xyz

[U08] Py：展平二维列表
来源：http://sas.hywenlv.cn

[y for x in nested for y in x]
来源：http://swi.ywan-chungtsiang.top

[U09] Py：字典取最大值的键
来源：http://xeg.cucudq.cn

max(d, key=d.get)
来源：http://wlc.kuanghao11.cn

[U10] Py：按值排序字典
来源：http://gxn.tarul.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zpw.zdqjudy.top


<!-- 参考信息 -->