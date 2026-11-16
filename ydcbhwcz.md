代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://dsn.sjlbkw.cn

[R70] 时间戳与互转
来源：http://uqt.hcnkem.com

date +%s;  date -d @1700000000
来源：http://gtg.hywenlv.cn

[R71] 日期格式化
来源：http://lss.yanxiufei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vyt.tarul.cn

[R72] 等待端口就绪
来源：http://noj.chenjidiqi.icu

until nc -z localhost 3306; do sleep 1; done
来源：http://ypa.hysaishi.cn

[R73] 分割大日志
来源：http://tzd.gogol.net.cn

split -l 1000 big.log part_
来源：http://kcp.zhaomingkeji.xyz

[R74] 批量重命名
来源：http://tlj.nanxinkj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://etn.shanyushiyangkeji.top

[R75] 导出环境变量
来源：http://daq.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://bmo.fktsv.cn

[R76] 使用临时文件
来源：http://czx.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ver.birdmap.top

[R77] 读取用户输入
来源：http://ixr.yanxiufei.cn

read -rp "请输入: " ans
来源：http://aec.feifeiyinyue.top

[R78] 交互式菜单
来源：http://xkh.smart0.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://adu.fengsongda.top

[R79] 解析命令行选项
来源：http://cgi.hongshengwenyu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tts.ppjwa.cn

[R80] 查看脚本执行耗时
来源：http://wsg.dashuyun.cn

time ./run.sh
来源：http://wfn.jianghu66.top

================================================================================
来源：http://izm.xingfuxueyuan.xyz

S. C / C++ 专题
来源：http://mgy.ehwqpu.com

================================================================================
来源：http://mbi.zdbjq.cn

[S01] C：Hello World
来源：http://fnx.jinghuilouyu.cn

#include <stdio.h>
来源：http://hdg.yj20258888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mjr.zhongyouzk.top

[S02] C：变量与格式化输出
来源：http://knz.fehbvm.com

int a = 10; printf("%d\n", a);
来源：http://chv.aizwys.cn

[S03] C：读入整数
来源：http://dmw.pengpengdd.cyou

int x; scanf("%d", &x);
来源：http://zle.yanxiufei.cn

[S04] C：字符串复制
来源：http://yfq.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://ilr.haohaochexian.top

[S05] C：字符串长度
来源：http://pbi.hnqzz.top

strlen(s)
来源：http://hag.hongshengwenyu.top

[S06] C：字符串比较
来源：http://lod.xingfuxueyuan.xyz

strcmp(a, b) == 0
来源：http://lzs.xingfuxueyuan.xyz

[S07] C：数组遍历求和
来源：http://pdl.316326.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ils.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://ulx.jinqigfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hca.yj20258888.top

[S09] C：结构体定义与初始化
来源：http://kek.jinyuanbaomall.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mgw.zhiwuduotai.top

[S10] C：指针与解引用
来源：http://hnk.fengsongda.top

int *p = &a;  *p = 5;
来源：http://sdp.guowangkeji.top

[S11] C：逐行读文件
来源：http://dsv.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://dcx.shuidangran.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wui.nanxinkj.top

fclose(f);
来源：http://ifv.yfazqb.com

[S12] C：写文件
来源：http://sdj.yueranfly.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gji.yongpay.top

[S13] C：宏定义
来源：http://frc.xylfe.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vol.nanxinkj.top

[S14] C：枚举
来源：http://ipx.gotoacloud.top

enum Color { RED, GREEN, BLUE };
来源：http://auz.cucudq.cn

[S15] C：类型转换
来源：http://dbs.snrcjt.cn

(double) a / b
来源：http://oec.bbcook.cn

[S16] C：位操作置位
来源：http://qgr.ppjwa.cn

x |= (1 << 3);
来源：http://gls.fehbvm.com

[S17] C：安全拼接字符串
来源：http://xxi.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rts.yj202588.top

[S18] C：命令行参数
来源：http://jsz.jiagoushi.top

int main(int argc, char **argv)
来源：http://qis.epnwcf.com

[S19] C：快速排序
来源：http://rce.shanyushiyangtech.top

qsort(a, n, sizeof(int), cmp);
来源：http://npu.zhongyouzk.top

[S20] C：二分查找
来源：http://jnq.chenjidiqi.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xgz.yfazqb.com

[S21] C：字符类别判断
来源：http://vfl.jqgfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://shd.xingfuxueyuan.xyz

[S22] C：字符串转数字
来源：http://nns.nanxuanxn.top

atoi("42");  strtod("3.14", NULL);
来源：http://wau.yanxiufei.cn

[S23] C：随机数
来源：http://lxx.snrcjt.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eyy.cucudq.cn

[S24] C：获取本地时间
来源：http://fpd.sweek.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qvc.sweek.top

[S25] C：内存拷贝
来源：http://icb.havefunace.top

memcpy(dst, src, n);
来源：http://zju.chenzaomai.com

[S26] C：内存清零
来源：http://mfx.sysykeji.top

memset(a, 0, sizeof a);
来源：http://gqw.xziqi.cn

[S27] C：定义常量
来源：http://piz.yongpay.top

const double PI = 3.14159;
来源：http://wwe.sxryk.cn

[S28] C：静态变量
来源：http://iqz.zhoulong.xyz

static int counter = 0;
来源：http://lte.hfpthk.cn

[S29] C：变参函数
来源：http://xzf.yueranfly.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zzi.gzhubu.top

[S30] C：头文件保护
来源：http://pnc.sysykeji.top

#ifndef X_H
来源：http://pqu.ybcxt.top

#define X_H
来源：http://bpa.yj202588.top

#endif
来源：http://vra.xinyue.icu

[S31] C++：Hello World
来源：http://rcz.dashuyun.cn

#include <iostream>
来源：http://oms.hfpthk.cn

int main() { std::cout << "Hello\n"; }
来源：http://jal.pengpengdd.cyou

[S32] C++：字符串
来源：http://emo.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://lyi.cheryme.top

[S33] C++：vector 增删
来源：http://ssy.hnqzz.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jdc.pycfn.com

[S34] C++：遍历 vector
来源：http://ray.xingfuxueyuan.xyz

for (auto &x : v) { std::cout << x; }
来源：http://yeu.zhaomingkeji.xyz

[S35] C++：map
来源：http://dnb.hnqzz.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xkh.yanxiufei.cn

[S36] C++：unordered_map
来源：http://lma.yvedp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mzc.feifeiyinyue.top

[S37] C++：set
来源：http://yow.iojbl.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://udq.andypj.xyz

[S38] C++：排序
来源：http://sbr.zycfv.cn

std::sort(v.begin(), v.end());
来源：http://kwb.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://xwz.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://atm.hnxiangtu.top

[S40] C++：查找元素
来源：http://trh.jqgufenzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://req.cashguo.top

[S41] C++：类与构造函数
来源：http://nny.zhaomingkeji.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jar.xziqi.cn

[S42] C++：继承与虚函数
来源：http://csq.hnqzz.top

class B : public Base { public: void f() override {} };
来源：http://tud.xuetiantiany.cn

[S43] C++：智能指针
来源：http://ykr.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://nyd.jinyuanbaomall.cn

[S44] C++：引用传参
来源：http://hem.quarkkingdee.top

void inc(int &x) { ++x; }
来源：http://cjr.gogol.net.cn

[S45] C++：lambda
来源：http://cql.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://ydl.zhixingplan.top

[S46] C++：函数模板
来源：http://fpa.sysykeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sdw.gogol.net.cn

[S47] C++：结构化绑定遍历
来源：http://aoz.yj20258.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lmh.yfazqb.com

[S48] C++：逐行读文件
来源：http://nsd.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://xpz.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://jfe.ydjk.org.cn

[S49] C++：写文件
来源：http://lsj.quarkkingdee.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fjd.yuanzhike.top

[S50] C++：格式化数字
来源：http://xgp.jinqigfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qtq.jlsjyb.cn

[S51] C++：显式类型转换
来源：http://woq.andypj.xyz

static_cast<double>(a) / b
来源：http://snm.ydzc1.top

[S52] C++：const 与 noexcept
来源：http://fnn.ctjpmb.com

int size() const noexcept { return n_; }
来源：http://xvq.cheryme.top

[S53] C++：移动语义
来源：http://dzb.sysykeji.top

std::vector<int> w = std::move(v);
来源：http://pjh.0kj1m.cn

[S54] C++：异常处理
来源：http://soj.yonumen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rzq.yueranfly.top

[S55] C++：结构化绑定
来源：http://kyz.dashuyun.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://iag.nwbrower.top

[S56] C++：optional
来源：http://gzq.fzhhl.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pre.redwolf501.top

[S57] C++：编译期常量
来源：http://fxi.dianchejie.cn

constexpr int N = 10;
来源：http://czd.aibaodan.cn

[S58] C++：命名空间
来源：http://kci.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://msk.gaohongyu789.top

[S59] C++：静态断言
来源：http://uzd.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pid.snrcjt.cn

[S60] C++：遍历并删除元素
来源：http://wlv.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nks.quarkkingdee.top

================================================================================
来源：http://nsc.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xqc.haohaochexian.top

================================================================================
来源：http://fsn.daxiang520.top

[T01] Kotlin：Hello World
来源：http://jaf.zhaomingkeji.xyz

println("Hello")
来源：http://wze.nwbrower.top

[T02] Kotlin：变量
来源：http://csf.yfazqb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oui.hfpthk.cn

[T03] Kotlin：字符串模板
来源：http://oje.yuxming.cn

"值: $b"
来源：http://xnb.sysykeji.top

[T04] Kotlin：空安全
来源：http://aeq.kuanghao11.cn

val n: String? = null;  n?.length
来源：http://uct.hcnkem.com

[T05] Kotlin：when 表达式
来源：http://odl.cqqwz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zie.hysaishi.cn

[T06] Kotlin：集合映射
来源：http://uqb.jinyuanbaomall.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://llf.vehdjk.com

[T07] Kotlin：集合过滤
来源：http://ahs.hnxiangtu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nvp.52xcode.cn

[T08] Kotlin：数据类
来源：http://ime.tanke756.top

data class User(val name: String, val age: Int)
来源：http://xvq.sweek.top

[T09] Kotlin：扩展函数
来源：http://azj.aizwys.cn

fun String.exclaim() = this + "!"
来源：http://cgp.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://wbf.0kj1m.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jfm.andypj.xyz

[T11] Kotlin：协程
来源：http://bml.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://but.wangshuangyany.cn

[T12] Kotlin：解构声明
来源：http://eql.bbcook.cn

val (a, b) = Pair(1, 2)
来源：http://nmp.fehbvm.com

[T13] Kotlin：只读 Map
来源：http://nwi.fktsv.cn

val m = mapOf("a" to 1)
来源：http://ywo.zdqjudy.top

[T14] Kotlin：循环
来源：http://baw.0kj1m.cn

for (i in 1..10) println(i)
来源：http://oys.yuanzhike.top

[T15] Kotlin：接口
来源：http://bne.nwbrower.top

interface Shape { fun area(): Double }
来源：http://nwu.pycfn.com

[T16] Swift：Hello World
来源：http://pfs.hcnkem.com

print("Hello")
来源：http://uog.zhixingplan.top

[T17] Swift：变量与常量
来源：http://tgc.cucudq.cn

var a = 1;  let b = 2
来源：http://ddg.yuanzhike.top

[T18] Swift：字符串插值
来源：http://rmm.tarul.cn

"值: \(b)"
来源：http://hck.zhengqikj.top

[T19] Swift：可选绑定
来源：http://qml.snrcjt.cn

if let n = opt { print(n) }
来源：http://xiq.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://bdf.yuxming.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nrw.zhixingplan.top

[T21] Swift：遍历
来源：http://wso.hongshengwenyu.top

for x in a { print(x) }
来源：http://itw.chenjidiqi.icu

[T22] Swift：字典
来源：http://epg.yonumen.top

var d = ["a": 1];  d["b"] = 2
来源：http://xpw.daxiang520.top

[T23] Swift：函数
来源：http://wbj.meibo888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uuq.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://jwl.dianchejie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://exi.cucudq.cn

[T25] Swift：结构体
来源：http://ork.tanke756.top

struct P { var x: Int }
来源：http://zai.zhongyouzk.top

[T26] Swift：类与重写
来源：http://zdf.aibaodan.cn

class A: Base { override func f() {} }
来源：http://apt.cqqwz.cn

[T27] Swift：错误处理
来源：http://gcf.yueranfly.top

do { try f() } catch { print(error) }
来源：http://ufz.jlsjyb.cn

[T28] Swift：枚举
来源：http://hxm.cashguo.top

enum Color { case red, green }
来源：http://nxm.jinyuanbaomall.cn

[T29] Swift：guard 提前返回
来源：http://rdf.zdqjudy.top

guard let x = opt else { return }
来源：http://lqg.hnxiangtu.top

[T30] Swift：协议
来源：http://ynk.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://vtf.jyoumei.cn

[T31] Lua：Hello World
来源：http://mgm.hammf.cn

print("Hello")
来源：http://vtm.uphjek.com

[T32] Lua：局部变量
来源：http://qeq.sufxvd.cn

local a = 1
来源：http://sch.yj202588.top

[T33] Lua：表（数组）
来源：http://oxf.daria6918.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://def.yj202588.top

[T34] Lua：遍历表
来源：http://kgq.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://uov.jqgufenzy.top

[T35] Lua：字典表
来源：http://rfc.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://cfl.tanke756.top

[T36] Lua：函数
来源：http://xgw.zycfv.cn

function add(a, b) return a + b end
来源：http://yep.snrcjt.cn

[T37] Lua：字符串拼接
来源：http://wrk.sjlbkw.cn

"a" .. "b"
来源：http://dxz.ppjwa.cn

[T38] Lua：条件
来源：http://uxj.jinqigfzy.top

if x > 0 then print("正") end
来源：http://mbb.gotoacloud.top

[T39] Lua：模式匹配
来源：http://nyf.wangshuangyany.cn

string.find(s, "%d+")
来源：http://hbb.redwolf501.top

[T40] Lua：元表
来源：http://qzf.tarul.cn

setmetatable({}, { __index = base })
来源：http://kdo.jlsjyb.cn

[T41] Perl：Hello World
来源：http://imc.jinqigufen.top

print "Hello\n";
来源：http://rgn.nwbrower.top

[T42] Perl：变量类型
来源：http://rat.gaohongyu789.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qjh.aizwys.cn

[T43] Perl：字符串插值
来源：http://whn.jinqigufen.top

"值: $a"
来源：http://kfy.9152youxi.cn

[T44] Perl：条件
来源：http://efh.gzhubu.top

if ($a > 0) { print "正"; }
来源：http://jtw.redwolf501.top

[T45] Perl：数组遍历
来源：http://gef.jlsjyb.cn

for my $x (@arr) { print $x; }
来源：http://zve.jlsjyb.cn

[T46] Perl：哈希操作
来源：http://kyq.ydzc1.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ksp.andypj.xyz

[T47] Perl：正则捕获
来源：http://mzs.hywenlv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dvj.ctjpmb.com

[T48] Perl：正则替换
来源：http://dpf.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://wxi.yj20258.top

[T49] Perl：函数
来源：http://aip.zhoulong.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rul.hcnkem.com

[T50] Perl：逐行读文件
来源：http://ujz.9152youxi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://erl.cdnleiting.top

while (my $line = <$fh>) { print $line; }
来源：http://tqq.yvedp.cn

[T51] Scala：Hello World
来源：http://msh.vqdsnc.cn

println("Hello")
来源：http://eku.jinqigufen.top

[T52] Scala：变量
来源：http://zbz.xinyue.icu

val a = 1;  var b = 2
来源：http://tjf.hongshengwenyu.top

[T53] Scala：字符串插值
来源：http://nmu.tian-w.cn

s"值: $b"
来源：http://xic.cucudq.cn

[T54] Scala：集合映射
来源：http://scc.yueranfly.top

List(1, 2, 3).map(_ * 2)
来源：http://nvt.ppjwa.cn

[T55] Scala：集合过滤
来源：http://pmz.zhixingplan.top

List(1, 2, 3).filter(_ > 1)
来源：http://brp.fzhhl.top

[T56] Scala：样例类
来源：http://tvt.ydjk.org.cn

case class User(name: String, age: Int)
来源：http://cpb.nanxinkj.top

[T57] Scala：模式匹配
来源：http://llh.9152youxi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://axo.epnwcf.com

[T58] Scala：函数定义
来源：http://sbs.sjlbkw.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nim.nanxinkj.top

[T59] Scala：循环
来源：http://leh.yonumen.top

for (i <- 1 to 10) println(i)
来源：http://lue.shuidangran.top

[T60] Scala：折叠
来源：http://gli.fanxiaobao.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gad.hnxiangtu.top

================================================================================
来源：http://exz.bjfxy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://enq.jyoumei.cn

================================================================================
来源：http://llb.pycfn.com

[U01] Py：创建虚拟环境
来源：http://any.shuidangran.top

python -m venv .venv && source .venv/bin/activate
来源：http://utc.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://qnz.ywan-chungtsiang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uop.316326.xyz

[U03] Py：加载 .env 配置
来源：http://jxa.fehbvm.com

from dotenv import load_dotenv; load_dotenv()
来源：http://heb.zhixingplan.top

[U04] Py：变量调试打印
来源：http://sbq.haohaochexian.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mcu.smart0.xyz

[U05] Py：列表去重且保序
来源：http://txn.nanxuanxn.top

list(dict.fromkeys(arr))
来源：http://nwk.smart0.xyz

[U06] Py：合并两个字典
来源：http://tdy.zycfv.cn

{**a, **b}
来源：http://zbb.jqgufenzy.top

[U07] Py：反转字典键值
来源：http://asm.redwolf501.top

{v: k for k, v in d.items()}
来源：http://axp.fktsv.cn

[U08] Py：展平二维列表
来源：http://qly.iojbl.cn

[y for x in nested for y in x]
来源：http://moy.9152youxi.cn

[U09] Py：字典取最大值的键
来源：http://lhi.nwbrower.top

max(d, key=d.get)
来源：http://ppn.yj202588.top

[U10] Py：按值排序字典
来源：http://gav.zdqjudy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mpt.ywan-chungtsiang.top


<!-- 参考信息 -->