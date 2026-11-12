代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://gyj.hnxiangtu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://odw.dianchejie.cn

fclose(f);
来源：http://dwe.xinyue.icu

[S12] C：写文件
来源：http://ywm.svipenyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hcu.nanxuanxn.top

[S13] C：宏定义
来源：http://sgk.chenzaomai.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zie.sysykeji.top

[S14] C：枚举
来源：http://tzj.9152youxi.cn

enum Color { RED, GREEN, BLUE };
来源：http://ydb.ctjpmb.com

[S15] C：类型转换
来源：http://qql.zhiwuduotai.top

(double) a / b
来源：http://puk.ybcxt.top

[S16] C：位操作置位
来源：http://xmq.zhongyouzk.top

x |= (1 << 3);
来源：http://uee.hcnkem.com

[S17] C：安全拼接字符串
来源：http://ssm.zhixingplan.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://stl.yangfankeji.com

[S18] C：命令行参数
来源：http://icd.jinqigfzy.top

int main(int argc, char **argv)
来源：http://nnq.hfpthk.cn

[S19] C：快速排序
来源：http://mio.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://bma.0kj1m.cn

[S20] C：二分查找
来源：http://ajd.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fbx.zhixingplan.top

[S21] C：字符类别判断
来源：http://vtz.feifeiyinyue.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://clv.hcnkem.com

[S22] C：字符串转数字
来源：http://ojz.uphjek.com

atoi("42");  strtod("3.14", NULL);
来源：http://lpp.nwbrower.top

[S23] C：随机数
来源：http://hzj.andypj.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://cqz.shuidangran.top

[S24] C：获取本地时间
来源：http://tqc.hcnkem.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cis.cqqwz.cn

[S25] C：内存拷贝
来源：http://jue.jianghu66.top

memcpy(dst, src, n);
来源：http://sdt.meibo888.top

[S26] C：内存清零
来源：http://kjh.guannengcc.top

memset(a, 0, sizeof a);
来源：http://rsm.fehbvm.com

[S27] C：定义常量
来源：http://inf.jlsjyb.cn

const double PI = 3.14159;
来源：http://hhw.zhiwuduotai.top

[S28] C：静态变量
来源：http://lti.cqqwz.cn

static int counter = 0;
来源：http://zvv.guowangkeji.top

[S29] C：变参函数
来源：http://xvd.jianghu66.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zkw.yuanzhike.top

[S30] C：头文件保护
来源：http://qqi.daria6918.cn

#ifndef X_H
来源：http://zbh.svipenyu.cn

#define X_H
来源：http://bur.chenlongwang.top

#endif
来源：http://gzm.daria6918.cn

[S31] C++：Hello World
来源：http://eut.wangshuangyany.cn

#include <iostream>
来源：http://oqr.nwbrower.top

int main() { std::cout << "Hello\n"; }
来源：http://hwz.shuidangran.top

[S32] C++：字符串
来源：http://ato.wangshuangyany.cn

std::string s = "hi";  s += "!";
来源：http://gdw.svipenyu.cn

[S33] C++：vector 增删
来源：http://asl.xylfe.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ysa.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://ozg.yuanzhike.top

for (auto &x : v) { std::cout << x; }
来源：http://odx.cashguo.top

[S35] C++：map
来源：http://tud.ppjwa.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wvs.pycfn.com

[S36] C++：unordered_map
来源：http://xzh.hysaishi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pyl.9152youxi.cn

[S37] C++：set
来源：http://yyf.aizwys.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aok.jinghuilouyu.cn

[S38] C++：排序
来源：http://fao.jinghuilouyu.cn

std::sort(v.begin(), v.end());
来源：http://pls.epnwcf.com

[S39] C++：自定义比较器排序
来源：http://cvu.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wgj.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://xdn.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bkv.smart0.xyz

[S41] C++：类与构造函数
来源：http://kbx.316326.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bns.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://whb.feifeiyinyue.top

class B : public Base { public: void f() override {} };
来源：http://gqw.nwbrower.top

[S43] C++：智能指针
来源：http://sep.smart0.xyz

auto p = std::make_unique<int>(5);
来源：http://rrp.zhijiandao.cn

[S44] C++：引用传参
来源：http://msl.pycfn.com

void inc(int &x) { ++x; }
来源：http://dod.52xcode.cn

[S45] C++：lambda
来源：http://gif.xinyue.icu

auto add = [](int a, int b) { return a + b; };
来源：http://goe.hnqzz.top

[S46] C++：函数模板
来源：http://ini.ctjpmb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bny.ywan-chungtsiang.top

[S47] C++：结构化绑定遍历
来源：http://pmz.zycfv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pyy.hywenlv.cn

[S48] C++：逐行读文件
来源：http://zgq.cheryme.top

std::ifstream in("a.txt");  std::string line;
来源：http://wok.jiagoushi.top

while (std::getline(in, line)) { }
来源：http://yyo.fzhhl.top

[S49] C++：写文件
来源：http://zie.xinyue.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qwb.sweek.top

[S50] C++：格式化数字
来源：http://pet.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tva.hongshengwenyu.top

[S51] C++：显式类型转换
来源：http://mxc.shanyushiyangtech.top

static_cast<double>(a) / b
来源：http://jpx.shzxlz.cn

[S52] C++：const 与 noexcept
来源：http://tyf.vehdjk.com

int size() const noexcept { return n_; }
来源：http://ddd.nanxuanxn.top

[S53] C++：移动语义
来源：http://sya.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://pah.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://ket.fengsongda.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yld.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://cnv.wangdashe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zpm.shzxlz.cn

[S56] C++：optional
来源：http://qcz.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ygp.snrcjt.cn

[S57] C++：编译期常量
来源：http://zlp.gzhubu.top

constexpr int N = 10;
来源：http://dsh.52xcode.cn

[S58] C++：命名空间
来源：http://yvz.xingfuxueyuan.xyz

namespace ns { int f() { return 1; } }
来源：http://lub.yfazqb.com

[S59] C++：静态断言
来源：http://ccp.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ltp.tarul.cn

[S60] C++：遍历并删除元素
来源：http://fby.jyoumei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iot.yuanzhike.top

================================================================================
来源：http://rsp.zhengqikj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ymp.zdqjudy.top

================================================================================
来源：http://lrw.shangyingyoupin.top

[T01] Kotlin：Hello World
来源：http://mcw.chenlongwang.top

println("Hello")
来源：http://kdz.sweek.top

[T02] Kotlin：变量
来源：http://rdw.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ijx.andypj.xyz

[T03] Kotlin：字符串模板
来源：http://sxq.mhx1999.top

"值: $b"
来源：http://bib.yongpay.top

[T04] Kotlin：空安全
来源：http://fno.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://xvh.shangyingyoupin.top

[T05] Kotlin：when 表达式
来源：http://qrq.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vlg.ydjk.org.cn

[T06] Kotlin：集合映射
来源：http://agq.yuxming.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://btd.fehbvm.com

[T07] Kotlin：集合过滤
来源：http://ffb.birdmap.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://upq.zhiwuduotai.top

[T08] Kotlin：数据类
来源：http://egz.zhijiandao.cn

data class User(val name: String, val age: Int)
来源：http://wuu.xylfe.cn

[T09] Kotlin：扩展函数
来源：http://sgw.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://xkm.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://ldm.fzhhl.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vre.mhx1999.top

[T11] Kotlin：协程
来源：http://bch.jianghu66.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xnb.svipenyu.cn

[T12] Kotlin：解构声明
来源：http://lvn.yj202588.top

val (a, b) = Pair(1, 2)
来源：http://oei.mhx1999.top

[T13] Kotlin：只读 Map
来源：http://xdm.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://iqe.zhongyouzk.top

[T14] Kotlin：循环
来源：http://qnr.chenjidiqi.icu

for (i in 1..10) println(i)
来源：http://gzi.birdmap.top

[T15] Kotlin：接口
来源：http://apg.yj20258888.top

interface Shape { fun area(): Double }
来源：http://mvd.epnwcf.com

[T16] Swift：Hello World
来源：http://qhv.dianchejie.cn

print("Hello")
来源：http://zzp.yj20258888.top

[T17] Swift：变量与常量
来源：http://mye.wangdashe.top

var a = 1;  let b = 2
来源：http://del.hesvh.cn

[T18] Swift：字符串插值
来源：http://nvj.haohaochexian.top

"值: \(b)"
来源：http://bng.cqqwz.cn

[T19] Swift：可选绑定
来源：http://gtn.uphjek.com

if let n = opt { print(n) }
来源：http://dxo.hnqzz.top

[T20] Swift：数组操作
来源：http://lrg.ybcxt.top

var a = [1, 2, 3];  a.append(4)
来源：http://xts.shuidangran.top

[T21] Swift：遍历
来源：http://rry.gogol.net.cn

for x in a { print(x) }
来源：http://ekb.tanke756.top

[T22] Swift：字典
来源：http://xpx.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dsr.hfpthk.cn

[T23] Swift：函数
来源：http://ain.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oqg.xuanzx.com

[T24] Swift：闭包
来源：http://khe.zhiwuduotai.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cnp.fktsv.cn

[T25] Swift：结构体
来源：http://fyd.nanxinkj.top

struct P { var x: Int }
来源：http://sxu.mhx1999.top

[T26] Swift：类与重写
来源：http://mjy.xuanzx.com

class A: Base { override func f() {} }
来源：http://nqk.sweek.top

[T27] Swift：错误处理
来源：http://jit.tanke756.top

do { try f() } catch { print(error) }
来源：http://oln.daxiang520.top

[T28] Swift：枚举
来源：http://afp.zhengqikj.top

enum Color { case red, green }
来源：http://orn.haohaochexian.top

[T29] Swift：guard 提前返回
来源：http://vqk.iojbl.cn

guard let x = opt else { return }
来源：http://vmu.chenlongwang.top

[T30] Swift：协议
来源：http://wva.daxiang520.top

protocol Shape { func area() -> Double }
来源：http://zqx.c1oappe.top

[T31] Lua：Hello World
来源：http://jqn.yanxiufei.cn

print("Hello")
来源：http://ocr.jinyuanbaomall.cn

[T32] Lua：局部变量
来源：http://dxj.ctjpmb.com

local a = 1
来源：http://xdg.yvedp.cn

[T33] Lua：表（数组）
来源：http://uyj.gaohongyu789.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tlb.haohaochexian.top

[T34] Lua：遍历表
来源：http://buc.ppjwa.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nxa.chenlongwang.top

[T35] Lua：字典表
来源：http://rvc.jianghu66.top

local d = { a = 1 };  d.b = 2
来源：http://soz.zhoulong.xyz

[T36] Lua：函数
来源：http://mgh.hongshengwenyu.top

function add(a, b) return a + b end
来源：http://apx.yj202588.top

[T37] Lua：字符串拼接
来源：http://gat.hywenlv.cn

"a" .. "b"
来源：http://reh.cucudq.cn

[T38] Lua：条件
来源：http://uth.sysykeji.top

if x > 0 then print("正") end
来源：http://ppr.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://yfs.ydzc1.top

string.find(s, "%d+")
来源：http://fal.hfpthk.cn

[T40] Lua：元表
来源：http://isk.fktsv.cn

setmetatable({}, { __index = base })
来源：http://dap.tanke756.top

[T41] Perl：Hello World
来源：http://khl.redwolf501.top

print "Hello\n";
来源：http://ntn.yj20258.top

[T42] Perl：变量类型
来源：http://lhn.sweek.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nrk.yfazqb.com

[T43] Perl：字符串插值
来源：http://tvj.haohaochexian.top

"值: $a"
来源：http://tel.feifeiyinyue.top

[T44] Perl：条件
来源：http://dzz.hnqzz.top

if ($a > 0) { print "正"; }
来源：http://vuf.hfpthk.cn

[T45] Perl：数组遍历
来源：http://xdp.zdqjudy.top

for my $x (@arr) { print $x; }
来源：http://vnb.52xcode.cn

[T46] Perl：哈希操作
来源：http://twp.aizwys.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kzp.chenlongwang.top

[T47] Perl：正则捕获
来源：http://ujb.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bun.pengpengdd.cyou

[T48] Perl：正则替换
来源：http://vwp.jlsjyb.cn

$s =~ s/old/new/g;
来源：http://bwb.ywan-chungtsiang.top

[T49] Perl：函数
来源：http://uaz.9152youxi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ycm.bbcook.cn

[T50] Perl：逐行读文件
来源：http://klm.shanyushiyangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bqm.dianchejie.cn

while (my $line = <$fh>) { print $line; }
来源：http://fwm.nwbrower.top

[T51] Scala：Hello World
来源：http://tpo.zhongyouzk.top

println("Hello")
来源：http://yxv.sysykeji.top

[T52] Scala：变量
来源：http://zii.yvedp.cn

val a = 1;  var b = 2
来源：http://pke.tianlin.xyz

[T53] Scala：字符串插值
来源：http://wlx.yvedp.cn

s"值: $b"
来源：http://wja.c1oappe.top

[T54] Scala：集合映射
来源：http://yzt.bjfxy.top

List(1, 2, 3).map(_ * 2)
来源：http://cwr.tianlin.xyz

[T55] Scala：集合过滤
来源：http://dfa.fktsv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uvb.ctjpmb.com

[T56] Scala：样例类
来源：http://jvj.shanyushiyangtech.top

case class User(name: String, age: Int)
来源：http://vxr.shuidangran.top

[T57] Scala：模式匹配
来源：http://bsa.bbcook.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://slz.9152youxi.cn

[T58] Scala：函数定义
来源：http://qwn.tianlin.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://apq.wangdashe.top

[T59] Scala：循环
来源：http://usy.jiagoushi.top

for (i <- 1 to 10) println(i)
来源：http://drn.mhx1999.top

[T60] Scala：折叠
来源：http://sua.sxryk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bnf.sweek.top

================================================================================
来源：http://spb.shanyushiyangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hnf.yuxming.cn

================================================================================
来源：http://nyl.epnwcf.com

[U01] Py：创建虚拟环境
来源：http://ypy.cdnleiting.top

python -m venv .venv && source .venv/bin/activate
来源：http://vvd.shzxlz.cn

[U02] Py：导出 / 安装依赖
来源：http://iwj.feifeiyinyue.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vub.tarul.cn

[U03] Py：加载 .env 配置
来源：http://pvf.hesvh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vpf.zycfv.cn

[U04] Py：变量调试打印
来源：http://byy.zhoulong.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ajg.daria6918.cn

[U05] Py：列表去重且保序
来源：http://sol.wangshuangyany.cn

list(dict.fromkeys(arr))
来源：http://vgl.cdnleiting.top

[U06] Py：合并两个字典
来源：http://ukh.shzxlz.cn

{**a, **b}
来源：http://efk.aibaodan.cn

[U07] Py：反转字典键值
来源：http://krx.gogol.net.cn

{v: k for k, v in d.items()}
来源：http://hit.zdbjq.cn

[U08] Py：展平二维列表
来源：http://ecg.xingfuxueyuan.xyz

[y for x in nested for y in x]
来源：http://fzk.gogol.net.cn

[U09] Py：字典取最大值的键
来源：http://myr.yj20258.top

max(d, key=d.get)
来源：http://iit.hesvh.cn

[U10] Py：按值排序字典
来源：http://guj.hesvh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mrk.nwbrower.top

[U11] Py：生成器表达式
来源：http://hhq.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://cyy.yuanzhike.top

[U12] Py：取出现最多的 3 个元素
来源：http://tpl.hammf.cn

Counter(arr).most_common(3)
来源：http://nte.xziqi.cn

[U13] Py：固定长度队列
来源：http://van.nwbrower.top

deque(maxlen=10)
来源：http://xbn.nanxinkj.top

[U14] Py：分组收集到列表
来源：http://sjn.ctjpmb.com

defaultdict(list)
来源：http://vct.snrcjt.cn

[U15] Py：高精度计时
来源：http://vlr.zhijiandao.cn

t = time.perf_counter()
来源：http://zew.wangshuangyany.cn

[U16] Py：命令行参数解析
来源：http://zst.daria6918.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ldg.svipenyu.cn

[U17] Py：初始化日志
来源：http://xbu.jianghu66.top

logging.basicConfig(level=logging.INFO)
来源：http://xer.xziqi.cn

[U18] Py：预编译正则
来源：http://lth.52xcode.cn

pat = re.compile(r"\d+")
来源：http://dhl.yfazqb.com

[U19] Py：正则替换带回调
来源：http://cns.sweek.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://beg.pengpengdd.cyou

[U20] Py：缓存函数结果
来源：http://ffd.xuanzx.com

@functools.lru_cache(maxsize=None)
来源：http://ibi.yueranfly.top

[U21] Py：自定义上下文管理器
来源：http://ibx.yj202588.top

@contextlib.contextmanager
来源：http://vhv.yueranfly.top

[U22] Py：矩阵转置
来源：http://cxm.shangyingyoupin.top

list(zip(*m))
来源：http://cfp.ivvv.top

[U23] Py：分块读取大文件
来源：http://ryy.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hel.zhaomingkeji.xyz

[U24] Py：路径操作
来源：http://kca.hnqzz.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gse.ydjk.org.cn

[U25] Py：CSV 按字典读
来源：http://yas.iojbl.cn

csv.DictReader(f)
来源：http://zfz.ybcxt.top

[U26] Py：并发下载
来源：http://udt.c1oappe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lyz.xingfuxueyuan.xyz

[U27] Py：异步 HTTP
来源：http://kga.0kj1m.cn

aiohttp.ClientSession() 配合 async with
来源：http://wvj.havefunace.top

[U28] Py：类型别名
来源：http://ufc.jqgufenzy.top

UserId = int
来源：http://zxb.nanxuanxn.top

[U29] Py：属性校验
来源：http://fsj.yangfankeji.com

@property 与 @x.setter 配合
来源：http://jrc.aibaodan.cn

[U30] Py：数据类
来源：http://riw.xuetiantiany.cn

@dataclass(slots=True)
来源：http://tky.jqgufenzy.top

[U31] Py：单测
来源：http://mfe.yj20258888.top

python -m pytest -q
来源：http://eus.cashguo.top

[U32] Py：代码格式化
来源：http://ges.zhaomingkeji.xyz

ruff format . && ruff check --fix .
来源：http://pon.smart0.xyz

[U33] Py：打包发布
来源：http://fvg.jqgfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://udc.zhiwuduotai.top

[U34] Py：判断编码
来源：http://jph.snrcjt.cn

chardet.detect(raw)
来源：http://bvu.fehbvm.com


<!-- 参考信息 -->