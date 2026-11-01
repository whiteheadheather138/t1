代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/ggzbakrxj.sHtML

[S51] C++：显式类型转换
来源：http://m.share.sjlbkw.cn/Article/details/guuppbzaq.sHtML

static_cast<double>(a) / b
来源：http://wap.tarul.cn/Article/details/gglttyeic.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fktsv.cn/Article/details/gsgqnmyed.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.bbcook.cn/Article/details/glhaujnsl.sHtML

[S53] C++：移动语义
来源：http://mobile.yfazqb.com/Article/details/gnqvhxgxt.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.epnwcf.com/Article/details/gcmcbcwzy.sHtML

[S54] C++：异常处理
来源：http://baike.yfazqb.com/Article/details/guoqcejdr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.tarul.cn/Article/details/gcyxdcutn.sHtML

[S55] C++：结构化绑定
来源：http://3g.vehdjk.com/Article/details/gsdxrpbva.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.yfazqb.com/Article/details/gbevqadyp.sHtML

[S56] C++：optional
来源：http://3g.yfazqb.com/Article/details/gcsjuwoxn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.vehdjk.com/Article/details/guymrxchi.sHtML

[S57] C++：编译期常量
来源：http://3g.epnwcf.com/Article/details/gfptfywpn.sHtML

constexpr int N = 10;
来源：http://baike.bbcook.cn/Article/details/glwkozpfd.sHtML

[S58] C++：命名空间
来源：http://wap.tarul.cn/Article/details/gdtjtsqmy.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fktsv.cn/Article/details/glgmvbdjl.sHtML

[S59] C++：静态断言
来源：http://3g.sjlbkw.cn/Article/details/gnnusyqah.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.bbcook.cn/Article/details/gzslylyor.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.bbcook.cn/Article/details/gkfisuhvb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gyojgsigj.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gjocrjolc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.bbcook.cn/Article/details/gcdexokzl.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gftwktxsa.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.tarul.cn/Article/details/gzhcnhynl.sHtML

println("Hello")
来源：http://read.share.fktsv.cn/Article/details/gjdapdnot.sHtML

[T02] Kotlin：变量
来源：http://www.blog.yfazqb.com/Article/details/gajwrqnlp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fktsv.cn/Article/details/gwgognpca.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.sjlbkw.cn/Article/details/gvieomebf.sHtML

"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gtfsbxbaf.sHtML

[T04] Kotlin：空安全
来源：http://mobile.epnwcf.com/Article/details/gmdvshgry.sHtML

val n: String? = null;  n?.length
来源：http://mobile.vehdjk.com/Article/details/gvcptllje.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.bbcook.cn/Article/details/gnklcrqrb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.epnwcf.com/Article/details/gjcwfhkwd.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fktsv.cn/Article/details/gngsbhvkp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.epnwcf.com/Article/details/guuegwqfi.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gtbmahjem.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fktsv.cn/Article/details/gsyxmllqz.sHtML

[T08] Kotlin：数据类
来源：http://wap.sjlbkw.cn/Article/details/gqhqskahc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/gdiybtjcy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.yfazqb.com/Article/details/gsiovcnbh.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.yfazqb.com/Article/details/gefhqakta.sHtML

[T10] Kotlin：默认参数
来源：http://blog.bbcook.cn/Article/details/gvdqwkxlp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.yfazqb.com/Article/details/givykmucu.sHtML

[T11] Kotlin：协程
来源：http://blog.bbcook.cn/Article/details/gyykjgxkv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fktsv.cn/Article/details/gfmczhsuy.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fktsv.cn/Article/details/goebmzgml.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.vehdjk.com/Article/details/grmopgkka.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.bbcook.cn/Article/details/gmzwnakmi.sHtML

val m = mapOf("a" to 1)
来源：http://blog.yfazqb.com/Article/details/gnahfbaph.sHtML

[T14] Kotlin：循环
来源：http://mobile.epnwcf.com/Article/details/goplbqtan.sHtML

for (i in 1..10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gmqfxnkql.sHtML

[T15] Kotlin：接口
来源：http://blog.bbcook.cn/Article/details/gjrubtmcq.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fktsv.cn/Article/details/gflymfhhw.sHtML

[T16] Swift：Hello World
来源：http://mobile.fktsv.cn/Article/details/gndfuckws.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gqbijgrwi.sHtML

[T17] Swift：变量与常量
来源：http://wap.fktsv.cn/Article/details/gchtmhrzl.sHtML

var a = 1;  let b = 2
来源：http://blog.fktsv.cn/Article/details/gojfrjdix.sHtML

[T18] Swift：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gqgiujaqg.sHtML

"值: \(b)"
来源：http://baike.fktsv.cn/Article/details/gsszknchm.sHtML

[T19] Swift：可选绑定
来源：http://3g.epnwcf.com/Article/details/gemkngpbs.sHtML

if let n = opt { print(n) }
来源：http://www.share.vehdjk.com/Article/details/gdavrditp.sHtML

[T20] Swift：数组操作
来源：http://wap.sjlbkw.cn/Article/details/gqtxtswsd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.tarul.cn/Article/details/gcvllznrw.sHtML

[T21] Swift：遍历
来源：http://www.m.share.bbcook.cn/Article/details/gotbpcajg.sHtML

for x in a { print(x) }
来源：http://baike.sjlbkw.cn/Article/details/ghupqxfad.sHtML

[T22] Swift：字典
来源：http://wap.bbcook.cn/Article/details/goexsynox.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.epnwcf.com/Article/details/gnfmtaljo.sHtML

[T23] Swift：函数
来源：http://m.share.yfazqb.com/Article/details/gurdvseqa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.epnwcf.com/Article/details/gxtzjhhty.sHtML

[T24] Swift：闭包
来源：http://baike.yfazqb.com/Article/details/gdspaslug.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gwdwepkxb.sHtML

[T25] Swift：结构体
来源：http://www.share.vehdjk.com/Article/details/geygswdkv.sHtML

struct P { var x: Int }
来源：http://baike.epnwcf.com/Article/details/grestjkfu.sHtML

[T26] Swift：类与重写
来源：http://3g.yfazqb.com/Article/details/gvpocunqu.sHtML

class A: Base { override func f() {} }
来源：http://mobile.vehdjk.com/Article/details/gnbtjtqko.sHtML

[T27] Swift：错误处理
来源：http://mobile.bbcook.cn/Article/details/gmslrdqmk.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.epnwcf.com/Article/details/guhscrhxh.sHtML

[T28] Swift：枚举
来源：http://baike.tarul.cn/Article/details/gwhtpbddb.sHtML

enum Color { case red, green }
来源：http://www.m.share.bbcook.cn/Article/details/gasubrnmh.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fktsv.cn/Article/details/gbxwqwznv.sHtML

guard let x = opt else { return }
来源：http://www.share.vehdjk.com/Article/details/gbtyumpfb.sHtML

[T30] Swift：协议
来源：http://3g.fktsv.cn/Article/details/gybahlmzz.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fktsv.cn/Article/details/gnipqawib.sHtML

[T31] Lua：Hello World
来源：http://read.share.bbcook.cn/Article/details/gkuzwhurm.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/ggrclvzar.sHtML

[T32] Lua：局部变量
来源：http://3g.bbcook.cn/Article/details/gdearkcdm.sHtML

local a = 1
来源：http://read.share.vehdjk.com/Article/details/gdlqiwgng.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.vehdjk.com/Article/details/gmkdwqhyx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fktsv.cn/Article/details/gwxxdyxsl.sHtML

[T34] Lua：遍历表
来源：http://blog.fktsv.cn/Article/details/gcvygxppp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.vehdjk.com/Article/details/gxyxtdhfk.sHtML

[T35] Lua：字典表
来源：http://mobile.fktsv.cn/Article/details/gcxilnnle.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gyiodvugt.sHtML

[T36] Lua：函数
来源：http://wap.bbcook.cn/Article/details/gdgufftbp.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.vehdjk.com/Article/details/gpnoqrwyu.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.yfazqb.com/Article/details/guyadpore.sHtML

"a" .. "b"
来源：http://www.blog.tarul.cn/Article/details/gfssjvhnc.sHtML

[T38] Lua：条件
来源：http://www.share.fktsv.cn/Article/details/ghxwmlsbz.sHtML

if x > 0 then print("正") end
来源：http://mobile.tarul.cn/Article/details/gysefcgrz.sHtML

[T39] Lua：模式匹配
来源：http://blog.epnwcf.com/Article/details/gwrhjxlra.sHtML

string.find(s, "%d+")
来源：http://baike.sjlbkw.cn/Article/details/gvjyfebpp.sHtML

[T40] Lua：元表
来源：http://wap.tarul.cn/Article/details/gvtlkjorz.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fktsv.cn/Article/details/gtyfqnouv.sHtML

[T41] Perl：Hello World
来源：http://3g.epnwcf.com/Article/details/gilmzpsch.sHtML

print "Hello\n";
来源：http://m.share.fktsv.cn/Article/details/gybjqphpe.sHtML

[T42] Perl：变量类型
来源：http://wap.epnwcf.com/Article/details/ghgjghipc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.yfazqb.com/Article/details/gpfggaapf.sHtML

[T43] Perl：字符串插值
来源：http://3g.yfazqb.com/Article/details/gupyypmcu.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/gjxwjwfyt.sHtML

[T44] Perl：条件
来源：http://wap.yfazqb.com/Article/details/gztqxbeyo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.vehdjk.com/Article/details/grllphtwm.sHtML

[T45] Perl：数组遍历
来源：http://wap.sjlbkw.cn/Article/details/gaoauadnv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.yfazqb.com/Article/details/gnskqdxlg.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.bbcook.cn/Article/details/gkpzjjavb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmvmkekj.sHtML

[T47] Perl：正则捕获
来源：http://baike.bbcook.cn/Article/details/gwdqpbbld.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.tarul.cn/Article/details/gyjnlpfwp.sHtML

[T48] Perl：正则替换
来源：http://3g.fktsv.cn/Article/details/giczyxqhb.sHtML

$s =~ s/old/new/g;
来源：http://3g.bbcook.cn/Article/details/gjmhbaejl.sHtML

[T49] Perl：函数
来源：http://m.share.fktsv.cn/Article/details/gjupqqjue.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gzgfkbaeg.sHtML

[T50] Perl：逐行读文件
来源：http://wap.vehdjk.com/Article/details/ghovvfytk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.vehdjk.com/Article/details/gtcgdgqgw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fktsv.cn/Article/details/gtyagkunj.sHtML

[T51] Scala：Hello World
来源：http://wap.bbcook.cn/Article/details/gvgvvdtjw.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gwuitfzgv.sHtML

[T52] Scala：变量
来源：http://m.share.sjlbkw.cn/Article/details/gasrkrkow.sHtML

val a = 1;  var b = 2
来源：http://read.share.sjlbkw.cn/Article/details/glgkvppty.sHtML

[T53] Scala：字符串插值
来源：http://wap.epnwcf.com/Article/details/gyimslntg.sHtML

s"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gqhgegnal.sHtML

[T54] Scala：集合映射
来源：http://read.share.bbcook.cn/Article/details/gmrjnepwt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.bbcook.cn/Article/details/goxvvqtpa.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gsukqppmx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.sjlbkw.cn/Article/details/gtryyxjas.sHtML

[T56] Scala：样例类
来源：http://m.share.yfazqb.com/Article/details/gpqupujyi.sHtML

case class User(name: String, age: Int)
来源：http://www.share.epnwcf.com/Article/details/gpzjolhit.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.epnwcf.com/Article/details/gpnzxxmfn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.vehdjk.com/Article/details/glmqyjuts.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.tarul.cn/Article/details/glafpbwxk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.yfazqb.com/Article/details/gpkqjbpkz.sHtML

[T59] Scala：循环
来源：http://blog.yfazqb.com/Article/details/gycijeksm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/giwpqtrjo.sHtML

[T60] Scala：折叠
来源：http://read.share.fktsv.cn/Article/details/grawgheqd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.bbcook.cn/Article/details/gjfuvkvlr.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwlvcuegl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/gdmberbxp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdvxsprqd.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.vehdjk.com/Article/details/gvbsptaci.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fktsv.cn/Article/details/gpkiegdhj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fktsv.cn/Article/details/gekzukrej.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fktsv.cn/Article/details/gpkdqinmi.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.sjlbkw.cn/Article/details/gyzdijwwo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcaprhxj.sHtML

[U04] Py：变量调试打印
来源：http://m.share.sjlbkw.cn/Article/details/gfmxvgony.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.vehdjk.com/Article/details/gxibdwnzo.sHtML

[U05] Py：列表去重且保序
来源：http://3g.vehdjk.com/Article/details/ggsimnnpo.sHtML

list(dict.fromkeys(arr))
来源：http://wap.sjlbkw.cn/Article/details/gitgzlpcx.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.epnwcf.com/Article/details/gxzqzrldq.sHtML

{**a, **b}
来源：http://wap.bbcook.cn/Article/details/ghwhmhvql.sHtML

[U07] Py：反转字典键值
来源：http://read.share.tarul.cn/Article/details/grecdujac.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fktsv.cn/Article/details/gqeoruhap.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/genaqnscs.sHtML

[y for x in nested for y in x]
来源：http://3g.sjlbkw.cn/Article/details/gnpgzwckx.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.yfazqb.com/Article/details/ggjpymove.sHtML

max(d, key=d.get)
来源：http://m.share.tarul.cn/Article/details/giuuxmsjr.sHtML

[U10] Py：按值排序字典
来源：http://wap.tarul.cn/Article/details/goqygdfqc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.epnwcf.com/Article/details/gjewucame.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.bbcook.cn/Article/details/gssiiqkub.sHtML

(x * 2 for x in arr)
来源：http://m.share.epnwcf.com/Article/details/gzbodbkam.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.sjlbkw.cn/Article/details/gescqfvrw.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.bbcook.cn/Article/details/gnrwfvmks.sHtML

[U13] Py：固定长度队列
来源：http://read.share.epnwcf.com/Article/details/giyphgjqu.sHtML

deque(maxlen=10)
来源：http://wap.vehdjk.com/Article/details/gdfsibyvb.sHtML

[U14] Py：分组收集到列表
来源：http://3g.yfazqb.com/Article/details/gycgnlkmj.sHtML

defaultdict(list)
来源：http://3g.fktsv.cn/Article/details/gkrnuvnrn.sHtML

[U15] Py：高精度计时
来源：http://www.blog.vehdjk.com/Article/details/gzqdapiif.sHtML

t = time.perf_counter()
来源：http://mobile.vehdjk.com/Article/details/gmhromfrd.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fktsv.cn/Article/details/gsgzmfukd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.yfazqb.com/Article/details/gzyvutohq.sHtML

[U17] Py：初始化日志
来源：http://baike.epnwcf.com/Article/details/gxeootzrm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.yfazqb.com/Article/details/gjfecnlqp.sHtML

[U18] Py：预编译正则
来源：http://read.share.tarul.cn/Article/details/gphiyenbd.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/gzrrnnzrg.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.tarul.cn/Article/details/gfhbztbsq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.bbcook.cn/Article/details/gwthszbmq.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.vehdjk.com/Article/details/gcwfwkmoc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlonnrwb.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fktsv.cn/Article/details/gnlufjzgs.sHtML

@contextlib.contextmanager
来源：http://m.share.vehdjk.com/Article/details/gsdnjfbky.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.bbcook.cn/Article/details/gddrbgvbt.sHtML

list(zip(*m))
来源：http://www.blog.tarul.cn/Article/details/gsbcqmiag.sHtML

[U23] Py：分块读取大文件
来源：http://blog.epnwcf.com/Article/details/ggbmoryak.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.vehdjk.com/Article/details/gpljhdxdb.sHtML

[U24] Py：路径操作
来源：http://3g.yfazqb.com/Article/details/guqzaphnk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.vehdjk.com/Article/details/gnfsjsbsn.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.bbcook.cn/Article/details/gupayktxj.sHtML

csv.DictReader(f)
来源：http://www.blog.epnwcf.com/Article/details/glgvsvxxx.sHtML

[U26] Py：并发下载
来源：http://www.blog.vehdjk.com/Article/details/gykshyjsa.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.epnwcf.com/Article/details/gxkroaztk.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzuswjow.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.sjlbkw.cn/Article/details/ggkosdfap.sHtML

[U28] Py：类型别名
来源：http://wap.bbcook.cn/Article/details/gntcgosbw.sHtML

UserId = int
来源：http://blog.yfazqb.com/Article/details/glxpwaebp.sHtML

[U29] Py：属性校验
来源：http://read.share.vehdjk.com/Article/details/gmgphrzkq.sHtML

@property 与 @x.setter 配合
来源：http://baike.tarul.cn/Article/details/gjwhfcfzv.sHtML

[U30] Py：数据类
来源：http://3g.vehdjk.com/Article/details/gmtcqdskx.sHtML

@dataclass(slots=True)
来源：http://m.share.epnwcf.com/Article/details/gfybmuzcc.sHtML

[U31] Py：单测
来源：http://www.m.share.yfazqb.com/Article/details/gftspmrqz.sHtML

python -m pytest -q
来源：http://wap.tarul.cn/Article/details/gzlduondo.sHtML

[U32] Py：代码格式化
来源：http://www.share.epnwcf.com/Article/details/gkcgajbyy.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fktsv.cn/Article/details/gdmviovqw.sHtML

[U33] Py：打包发布
来源：http://3g.vehdjk.com/Article/details/gcbfhckew.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.bbcook.cn/Article/details/gsdbffhus.sHtML

[U34] Py：判断编码
来源：http://read.share.bbcook.cn/Article/details/gfqzrcvsi.sHtML

chardet.detect(raw)
来源：http://www.m.share.fktsv.cn/Article/details/gypijazig.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.vehdjk.com/Article/details/gljqkggqc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.yfazqb.com/Article/details/gracdvaye.sHtML

[U36] Py：定时任务
来源：http://mobile.tarul.cn/Article/details/gbdojkxke.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.yfazqb.com/Article/details/gvcafclac.sHtML

[U37] Py：读写 Excel
来源：http://read.share.epnwcf.com/Article/details/gdnzmjzqg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.yfazqb.com/Article/details/gweyqgpol.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.sjlbkw.cn/Article/details/gmosiowpf.sHtML

Path(__file__).resolve().parent
来源：http://wap.yfazqb.com/Article/details/gemihvttv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.tarul.cn/Article/details/gvhudxzmm.sHtML

sys.stdout.isatty()
来源：http://3g.yfazqb.com/Article/details/gchgmmkyf.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.yfazqb.com/Article/details/gqitwganq.sHtML

print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gheieiqsx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.sjlbkw.cn/Article/details/gmrgvldvk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.sjlbkw.cn/Article/details/gungcnthm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.bbcook.cn/Article/details/gstxkrjvg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.epnwcf.com/Article/details/gvgakvpyh.sHtML

[U43] PHP：声明命名空间
来源：http://3g.bbcook.cn/Article/details/gfiwhfccj.sHtML

namespace App\Http;
来源：http://mobile.vehdjk.com/Article/details/gbaynoeeb.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.sjlbkw.cn/Article/details/gujgsasgd.sHtML

declare(strict_types=1);
来源：http://blog.sjlbkw.cn/Article/details/goxjzukax.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fktsv.cn/Article/details/ghasrfhjp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/goicfbwgr.sHtML

[U46] PHP：可空类型
来源：http://wap.tarul.cn/Article/details/gslvuxhss.sHtML

?string $name = null
来源：http://3g.tarul.cn/Article/details/gqkxnnmak.sHtML

[U47] PHP：联合类型
来源：http://baike.epnwcf.com/Article/details/gggysatie.sHtML

int|string $id
来源：http://3g.vehdjk.com/Article/details/gzkkceyad.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.vehdjk.com/Article/details/gqgnqflhk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.yfazqb.com/Article/details/gqmzovcpi.sHtML

[U49] PHP：只读属性
来源：http://baike.epnwcf.com/Article/details/gpeszxsob.sHtML

public readonly string $name
来源：http://blog.bbcook.cn/Article/details/gpzmhwnei.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.vehdjk.com/Article/details/gijnnqgtb.sHtML

public function __construct(private int $id) {}
来源：http://3g.fktsv.cn/Article/details/gfybthwgb.sHtML

[U51] PHP：数组解构
来源：http://baike.bbcook.cn/Article/details/gnwzgncpi.sHtML

[$a, $b] = $arr;
来源：http://baike.epnwcf.com/Article/details/gvzftzvgf.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/grkqrejnl.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.epnwcf.com/Article/details/gszwhegbw.sHtML

[U53] PHP：空合并运算符
来源：http://3g.bbcook.cn/Article/details/gwbjokmpi.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.sjlbkw.cn/Article/details/gjliclfzn.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.epnwcf.com/Article/details/gszzsdfmj.sHtML

$obj?->method()
来源：http://www.blog.bbcook.cn/Article/details/groxvlbyr.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.epnwcf.com/Article/details/gaqxsopfp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.epnwcf.com/Article/details/gfpocwqkt.sHtML

[U56] PHP：命名参数
来源：http://3g.tarul.cn/Article/details/gepddsnzg.sHtML

f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gjghdsnqs.sHtML

[U57] PHP：字符串插值
来源：http://blog.epnwcf.com/Article/details/gjavrlsxr.sHtML

"值: {$a}"
来源：http://www.blog.fktsv.cn/Article/details/gxuevcbhh.sHtML

[U58] PHP：数组三件套
来源：http://m.share.vehdjk.com/Article/details/gyttgojit.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.vehdjk.com/Article/details/gzrybiyho.sHtML

[U59] PHP：自定义排序
来源：http://blog.vehdjk.com/Article/details/giysykesi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.epnwcf.com/Article/details/gzkmshlxu.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.tarul.cn/Article/details/gvambhxxi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.vehdjk.com/Article/details/gjlqxlzlv.sHtML

[U61] PHP：正则
来源：http://mobile.epnwcf.com/Article/details/gaecndwry.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.tarul.cn/Article/details/gqlcxdetr.sHtML

[U62] PHP：日期对象
来源：http://wap.bbcook.cn/Article/details/gsrsrilxj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fktsv.cn/Article/details/gekznvgay.sHtML

[U63] PHP：文件读写
来源：http://www.share.tarul.cn/Article/details/gmjoarpnc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fktsv.cn/Article/details/ghlsgikru.sHtML

[U64] PHP：目录遍历
来源：http://www.share.vehdjk.com/Article/details/gpzesjcgr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fktsv.cn/Article/details/gbswrudrb.sHtML

[U65] PHP：会话
来源：http://baike.vehdjk.com/Article/details/glccuxlsi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gsthqzxtm.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.epnwcf.com/Article/details/geyulspvr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.vehdjk.com/Article/details/guiajynzv.sHtML

[U67] PHP：处理文件上传
来源：http://baike.tarul.cn/Article/details/gyjxsodcm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.vehdjk.com/Article/details/grdiertsh.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.tarul.cn/Article/details/geinezucm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.tarul.cn/Article/details/ghveelyxm.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.yfazqb.com/Article/details/gwsqqxpgs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.tarul.cn/Article/details/gnifapswd.sHtML

[U70] PHP：PDO 事务
来源：http://blog.yfazqb.com/Article/details/gwkjxxakm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.sjlbkw.cn/Article/details/gyadrwmya.sHtML

[U71] PHP：抛出异常
来源：http://mobile.tarul.cn/Article/details/gujslptcp.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.tarul.cn/Article/details/gsczxwdzx.sHtML

[U72] PHP：写错误日志
来源：http://baike.bbcook.cn/Article/details/gktqvijoq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.yfazqb.com/Article/details/gkqilseym.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.vehdjk.com/Article/details/gvfipngvx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.bbcook.cn/Article/details/gtikzycre.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gohkwjnpz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.epnwcf.com/Article/details/gqujzldgz.sHtML

[U75] PHP：依赖注入
来源：http://blog.fktsv.cn/Article/details/gkgqbzqss.sHtML

composer require psr/container
来源：http://baike.tarul.cn/Article/details/gaasrhhsx.sHtML

[U76] PHP：简单路由
来源：http://mobile.sjlbkw.cn/Article/details/gmatyghna.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.bbcook.cn/Article/details/gefygdipa.sHtML


<!-- 参考信息 -->