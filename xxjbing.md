代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gtsekthcu.sHtML

[S51] C++：显式类型转换
来源：http://baike.epnwcf.com/Article/details/gujaoezhr.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fktsv.cn/Article/details/gsiiciyun.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.epnwcf.com/Article/details/gajdewedj.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gjahizwzp.sHtML

[S53] C++：移动语义
来源：http://read.share.epnwcf.com/Article/details/gdujskcvb.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.bbcook.cn/Article/details/gxqxyidbe.sHtML

[S54] C++：异常处理
来源：http://3g.vehdjk.com/Article/details/gdrwjkmrm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.bbcook.cn/Article/details/glznsxrpz.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fktsv.cn/Article/details/gkujkmxze.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fktsv.cn/Article/details/gqlmjxalq.sHtML

[S56] C++：optional
来源：http://mobile.bbcook.cn/Article/details/gkbmyjdlx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fktsv.cn/Article/details/gegsywjbx.sHtML

[S57] C++：编译期常量
来源：http://mobile.vehdjk.com/Article/details/ghezjgszy.sHtML

constexpr int N = 10;
来源：http://mobile.fktsv.cn/Article/details/gkyrieheg.sHtML

[S58] C++：命名空间
来源：http://www.share.tarul.cn/Article/details/gmpyhomnb.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fktsv.cn/Article/details/ghipqmxxv.sHtML

[S59] C++：静态断言
来源：http://wap.vehdjk.com/Article/details/gojkknxbk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.epnwcf.com/Article/details/gotkkqwst.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.yfazqb.com/Article/details/gyvuafojj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/gyaxzscvk.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gudguwodc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gwnjfvezq.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxumvbdsu.sHtML

[T01] Kotlin：Hello World
来源：http://wap.vehdjk.com/Article/details/gcxxsiikl.sHtML

println("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gazsffkds.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gykntrkik.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.epnwcf.com/Article/details/gjgvxqtre.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.epnwcf.com/Article/details/gjyvbfjwv.sHtML

"值: $b"
来源：http://www.share.yfazqb.com/Article/details/ghoihtozp.sHtML

[T04] Kotlin：空安全
来源：http://wap.vehdjk.com/Article/details/gseqbowxg.sHtML

val n: String? = null;  n?.length
来源：http://wap.vehdjk.com/Article/details/gyobeplfu.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.tarul.cn/Article/details/gqnselvfw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fktsv.cn/Article/details/gauxrggzz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.bbcook.cn/Article/details/gkzwfbhoo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gdkejouvt.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.bbcook.cn/Article/details/gsbjywuho.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.epnwcf.com/Article/details/ghynqoqht.sHtML

[T08] Kotlin：数据类
来源：http://mobile.sjlbkw.cn/Article/details/ghrzjousu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/goctwuqkw.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.tarul.cn/Article/details/ggwxqebqh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fktsv.cn/Article/details/gnquzqzhs.sHtML

[T10] Kotlin：默认参数
来源：http://baike.bbcook.cn/Article/details/ggepxydrr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.vehdjk.com/Article/details/gpuhlsmsz.sHtML

[T11] Kotlin：协程
来源：http://baike.bbcook.cn/Article/details/gqbknhtaq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.vehdjk.com/Article/details/guulqoago.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.bbcook.cn/Article/details/gftucahbp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gocqgplaj.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.sjlbkw.cn/Article/details/gjqcxhthh.sHtML

val m = mapOf("a" to 1)
来源：http://baike.yfazqb.com/Article/details/gqdculxej.sHtML

[T14] Kotlin：循环
来源：http://wap.vehdjk.com/Article/details/gsxigtyzn.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.bbcook.cn/Article/details/gejmzpita.sHtML

[T15] Kotlin：接口
来源：http://m.share.tarul.cn/Article/details/gzfvdblre.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fktsv.cn/Article/details/gzbehbure.sHtML

[T16] Swift：Hello World
来源：http://wap.bbcook.cn/Article/details/gzqxwiuec.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gzgaqtcmr.sHtML

[T17] Swift：变量与常量
来源：http://www.share.sjlbkw.cn/Article/details/gjkzgnvrq.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gawyhuvug.sHtML

[T18] Swift：字符串插值
来源：http://m.share.tarul.cn/Article/details/gffbqrfar.sHtML

"值: \(b)"
来源：http://3g.fktsv.cn/Article/details/gunlhvmxi.sHtML

[T19] Swift：可选绑定
来源：http://m.share.yfazqb.com/Article/details/gyoujjaks.sHtML

if let n = opt { print(n) }
来源：http://blog.epnwcf.com/Article/details/ggmvzugrx.sHtML

[T20] Swift：数组操作
来源：http://3g.epnwcf.com/Article/details/gjswebfrs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fktsv.cn/Article/details/gsqmozpgs.sHtML

[T21] Swift：遍历
来源：http://baike.bbcook.cn/Article/details/gscmdhcer.sHtML

for x in a { print(x) }
来源：http://www.blog.tarul.cn/Article/details/gvrhljpkt.sHtML

[T22] Swift：字典
来源：http://blog.sjlbkw.cn/Article/details/gcyfkuniz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/gdbqpoacv.sHtML

[T23] Swift：函数
来源：http://www.share.epnwcf.com/Article/details/gzdipgzlc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.vehdjk.com/Article/details/gpyezoisi.sHtML

[T24] Swift：闭包
来源：http://wap.epnwcf.com/Article/details/gwayekyov.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gvihlgsxb.sHtML

[T25] Swift：结构体
来源：http://www.blog.epnwcf.com/Article/details/gpnupkise.sHtML

struct P { var x: Int }
来源：http://read.share.sjlbkw.cn/Article/details/ghzjakuiq.sHtML

[T26] Swift：类与重写
来源：http://read.share.fktsv.cn/Article/details/gnvmwaewv.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fktsv.cn/Article/details/gjdfykxiq.sHtML

[T27] Swift：错误处理
来源：http://m.share.bbcook.cn/Article/details/glungqdmg.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.vehdjk.com/Article/details/grkdebpzz.sHtML

[T28] Swift：枚举
来源：http://3g.yfazqb.com/Article/details/gnsdarlzy.sHtML

enum Color { case red, green }
来源：http://m.share.vehdjk.com/Article/details/gnbanuycd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.epnwcf.com/Article/details/gpgjfgxfd.sHtML

guard let x = opt else { return }
来源：http://wap.bbcook.cn/Article/details/ghoaninje.sHtML

[T30] Swift：协议
来源：http://www.m.share.fktsv.cn/Article/details/guirlmedo.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.vehdjk.com/Article/details/ggcbwslny.sHtML

[T31] Lua：Hello World
来源：http://read.share.epnwcf.com/Article/details/gcmezwgma.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/gcrssdzfv.sHtML

[T32] Lua：局部变量
来源：http://blog.epnwcf.com/Article/details/gbxogaiat.sHtML

local a = 1
来源：http://www.share.epnwcf.com/Article/details/gubpxvdxi.sHtML

[T33] Lua：表（数组）
来源：http://blog.vehdjk.com/Article/details/gsfovuxwn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.vehdjk.com/Article/details/ghmoxoibc.sHtML

[T34] Lua：遍历表
来源：http://3g.yfazqb.com/Article/details/ggxmsupti.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.epnwcf.com/Article/details/gnrreugvl.sHtML

[T35] Lua：字典表
来源：http://www.blog.epnwcf.com/Article/details/ghnohzedv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gpsaajvda.sHtML

[T36] Lua：函数
来源：http://wap.bbcook.cn/Article/details/gxqqudqof.sHtML

function add(a, b) return a + b end
来源：http://mobile.sjlbkw.cn/Article/details/gofyhyeup.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/gopkwtinr.sHtML

"a" .. "b"
来源：http://www.share.vehdjk.com/Article/details/gguhzcyqu.sHtML

[T38] Lua：条件
来源：http://read.share.fktsv.cn/Article/details/gpojvaark.sHtML

if x > 0 then print("正") end
来源：http://www.blog.tarul.cn/Article/details/gpwhuzkec.sHtML

[T39] Lua：模式匹配
来源：http://read.share.tarul.cn/Article/details/gyrfytyye.sHtML

string.find(s, "%d+")
来源：http://mobile.sjlbkw.cn/Article/details/gffdtinvq.sHtML

[T40] Lua：元表
来源：http://www.m.share.tarul.cn/Article/details/gbvohuifx.sHtML

setmetatable({}, { __index = base })
来源：http://wap.sjlbkw.cn/Article/details/gilrcmeni.sHtML

[T41] Perl：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gguimvpct.sHtML

print "Hello\n";
来源：http://blog.tarul.cn/Article/details/gfwvpfwwl.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.vehdjk.com/Article/details/glbhnumei.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.bbcook.cn/Article/details/ggezrifmu.sHtML

[T43] Perl：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gtccjqywo.sHtML

"值: $a"
来源：http://wap.vehdjk.com/Article/details/ggonagixv.sHtML

[T44] Perl：条件
来源：http://m.share.tarul.cn/Article/details/gesijhgrq.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.bbcook.cn/Article/details/gakoikfyu.sHtML

[T45] Perl：数组遍历
来源：http://blog.vehdjk.com/Article/details/gvbhtdjms.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.bbcook.cn/Article/details/gcevnbbhy.sHtML

[T46] Perl：哈希操作
来源：http://read.share.sjlbkw.cn/Article/details/gkgophlwf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/ggqgpcqvn.sHtML

[T47] Perl：正则捕获
来源：http://3g.tarul.cn/Article/details/gpkdgskmq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.sjlbkw.cn/Article/details/glzjzmopu.sHtML

[T48] Perl：正则替换
来源：http://wap.sjlbkw.cn/Article/details/ghezsczjy.sHtML

$s =~ s/old/new/g;
来源：http://www.share.epnwcf.com/Article/details/gmecaslfv.sHtML

[T49] Perl：函数
来源：http://www.share.tarul.cn/Article/details/gwdimzxso.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gdpqrosix.sHtML

[T50] Perl：逐行读文件
来源：http://wap.tarul.cn/Article/details/gdrsluoeq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.bbcook.cn/Article/details/gykwfqrgz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.yfazqb.com/Article/details/gjdlmdqln.sHtML

[T51] Scala：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gssveetsd.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gcosfrqxz.sHtML

[T52] Scala：变量
来源：http://m.share.yfazqb.com/Article/details/gibfyrueb.sHtML

val a = 1;  var b = 2
来源：http://baike.epnwcf.com/Article/details/glwtfggiy.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gdihvwwae.sHtML

s"值: $b"
来源：http://baike.yfazqb.com/Article/details/gerxtiaco.sHtML

[T54] Scala：集合映射
来源：http://mobile.tarul.cn/Article/details/gwxfrxfii.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gtjhfunow.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gpmzkihji.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fktsv.cn/Article/details/gcghzqido.sHtML

[T56] Scala：样例类
来源：http://m.share.sjlbkw.cn/Article/details/gunyfxtnw.sHtML

case class User(name: String, age: Int)
来源：http://baike.yfazqb.com/Article/details/gavtcwjye.sHtML

[T57] Scala：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/glmcokkjx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.tarul.cn/Article/details/goqtqtkpn.sHtML

[T58] Scala：函数定义
来源：http://read.share.yfazqb.com/Article/details/gfaksphce.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuihfkjt.sHtML

[T59] Scala：循环
来源：http://baike.tarul.cn/Article/details/gkfowbssq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gtenvihmn.sHtML

[T60] Scala：折叠
来源：http://www.m.share.yfazqb.com/Article/details/gaxcrtifa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.epnwcf.com/Article/details/gkfplxzdd.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gflxgcsak.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.vehdjk.com/Article/details/gzaxldmyp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/graqymmmp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.epnwcf.com/Article/details/grnlenfum.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fktsv.cn/Article/details/gywxyjqja.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.vehdjk.com/Article/details/gxbgeltik.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.sjlbkw.cn/Article/details/gdrbqleip.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.vehdjk.com/Article/details/ghrdezalw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.sjlbkw.cn/Article/details/gdaeigdqy.sHtML

[U04] Py：变量调试打印
来源：http://3g.vehdjk.com/Article/details/ggvhwpnxz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.epnwcf.com/Article/details/gudyvckfm.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.vehdjk.com/Article/details/gvayqqsgd.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gjvsvtzxs.sHtML

[U06] Py：合并两个字典
来源：http://blog.bbcook.cn/Article/details/gyjpddmqy.sHtML

{**a, **b}
来源：http://wap.yfazqb.com/Article/details/gkfpppblp.sHtML

[U07] Py：反转字典键值
来源：http://3g.epnwcf.com/Article/details/grxonpgef.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.sjlbkw.cn/Article/details/gqztjcker.sHtML

[U08] Py：展平二维列表
来源：http://www.share.epnwcf.com/Article/details/gtlsiyjnv.sHtML

[y for x in nested for y in x]
来源：http://wap.sjlbkw.cn/Article/details/gzqdnxjaq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.epnwcf.com/Article/details/glfgqnjss.sHtML

max(d, key=d.get)
来源：http://read.share.epnwcf.com/Article/details/gbrbcmyfb.sHtML

[U10] Py：按值排序字典
来源：http://mobile.epnwcf.com/Article/details/gtogfjwmh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.tarul.cn/Article/details/gqejgcwvl.sHtML

[U11] Py：生成器表达式
来源：http://wap.bbcook.cn/Article/details/gztcjiaze.sHtML

(x * 2 for x in arr)
来源：http://m.share.bbcook.cn/Article/details/goktjaozz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fktsv.cn/Article/details/grjdisigm.sHtML

Counter(arr).most_common(3)
来源：http://www.share.sjlbkw.cn/Article/details/gaswybqng.sHtML

[U13] Py：固定长度队列
来源：http://blog.fktsv.cn/Article/details/gqkjdchhf.sHtML

deque(maxlen=10)
来源：http://3g.fktsv.cn/Article/details/gkfsqlnli.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.vehdjk.com/Article/details/gcmwlqfob.sHtML

defaultdict(list)
来源：http://wap.sjlbkw.cn/Article/details/gbipchbhs.sHtML

[U15] Py：高精度计时
来源：http://read.share.fktsv.cn/Article/details/gncohjbfp.sHtML

t = time.perf_counter()
来源：http://baike.yfazqb.com/Article/details/gbtknurle.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.vehdjk.com/Article/details/gbhhzvwga.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.yfazqb.com/Article/details/gvvrxnccy.sHtML

[U17] Py：初始化日志
来源：http://www.share.yfazqb.com/Article/details/gbxdtgaok.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.bbcook.cn/Article/details/gufurhmgu.sHtML

[U18] Py：预编译正则
来源：http://3g.fktsv.cn/Article/details/gbzbtirhh.sHtML

pat = re.compile(r"\d+")
来源：http://3g.bbcook.cn/Article/details/gqplgqpqc.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fktsv.cn/Article/details/gzvupwbfv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.bbcook.cn/Article/details/gvdbanksh.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.bbcook.cn/Article/details/guiztcxks.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.epnwcf.com/Article/details/ghcraoonv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fktsv.cn/Article/details/ggyehujim.sHtML

@contextlib.contextmanager
来源：http://read.share.tarul.cn/Article/details/gllgapzvj.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.bbcook.cn/Article/details/gooruewzx.sHtML

list(zip(*m))
来源：http://www.m.share.fktsv.cn/Article/details/gxvvnlfqb.sHtML

[U23] Py：分块读取大文件
来源：http://blog.tarul.cn/Article/details/gwejynyhm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.vehdjk.com/Article/details/gviwwfrya.sHtML

[U24] Py：路径操作
来源：http://blog.yfazqb.com/Article/details/gcmqpagdi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/gcryndeip.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.sjlbkw.cn/Article/details/gtazhfqzi.sHtML

csv.DictReader(f)
来源：http://baike.sjlbkw.cn/Article/details/gzaafacre.sHtML

[U26] Py：并发下载
来源：http://www.share.sjlbkw.cn/Article/details/gqpdrgilm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.tarul.cn/Article/details/gmxtajfha.sHtML

[U27] Py：异步 HTTP
来源：http://baike.tarul.cn/Article/details/ghisimugs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.yfazqb.com/Article/details/gjqgybyof.sHtML

[U28] Py：类型别名
来源：http://wap.bbcook.cn/Article/details/gghapdewp.sHtML

UserId = int
来源：http://3g.vehdjk.com/Article/details/gtkhhxhge.sHtML

[U29] Py：属性校验
来源：http://wap.epnwcf.com/Article/details/gtdoioknt.sHtML

@property 与 @x.setter 配合
来源：http://wap.fktsv.cn/Article/details/gvhytrwnn.sHtML

[U30] Py：数据类
来源：http://read.share.yfazqb.com/Article/details/gsdrtrzwe.sHtML

@dataclass(slots=True)
来源：http://blog.vehdjk.com/Article/details/gkcnxgmcc.sHtML

[U31] Py：单测
来源：http://wap.yfazqb.com/Article/details/gatzpmung.sHtML

python -m pytest -q
来源：http://blog.fktsv.cn/Article/details/gymxgwofm.sHtML

[U32] Py：代码格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gflxhnshx.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fktsv.cn/Article/details/gudzjfqia.sHtML

[U33] Py：打包发布
来源：http://blog.epnwcf.com/Article/details/gepzkcgvz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.tarul.cn/Article/details/glrkzphrj.sHtML

[U34] Py：判断编码
来源：http://3g.yfazqb.com/Article/details/gzydoxvkg.sHtML

chardet.detect(raw)
来源：http://m.share.sjlbkw.cn/Article/details/gvriwygyk.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.yfazqb.com/Article/details/gcwlytgmj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.tarul.cn/Article/details/gbltruzie.sHtML

[U36] Py：定时任务
来源：http://m.share.tarul.cn/Article/details/gzwagxyed.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.sjlbkw.cn/Article/details/grdlptslm.sHtML

[U37] Py：读写 Excel
来源：http://wap.sjlbkw.cn/Article/details/ghlcpcvcx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.sjlbkw.cn/Article/details/gwbfhjgxk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.tarul.cn/Article/details/gjcnktrdo.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.yfazqb.com/Article/details/gkryybomn.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.yfazqb.com/Article/details/gkmfvkyzm.sHtML

sys.stdout.isatty()
来源：http://www.share.bbcook.cn/Article/details/grftsnlrc.sHtML

[U40] Py：打印到标准错误
来源：http://blog.vehdjk.com/Article/details/guepjfglw.sHtML

print("err", file=sys.stderr)
来源：http://m.share.sjlbkw.cn/Article/details/gfthsntjh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.epnwcf.com/Article/details/gccteqawl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fktsv.cn/Article/details/ggjvoorjt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.yfazqb.com/Article/details/ggcvxekpv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjunzhbw.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.tarul.cn/Article/details/gykkkkgli.sHtML

namespace App\Http;
来源：http://www.m.share.tarul.cn/Article/details/gcuhdfnih.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fktsv.cn/Article/details/gbgbmcnge.sHtML

declare(strict_types=1);
来源：http://blog.bbcook.cn/Article/details/gpzvbeytp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.yfazqb.com/Article/details/gqshzxhdh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gewpxmwnd.sHtML

[U46] PHP：可空类型
来源：http://m.share.sjlbkw.cn/Article/details/gxaqqsuiw.sHtML

?string $name = null
来源：http://www.blog.sjlbkw.cn/Article/details/gpzjptzqd.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgblkibh.sHtML

int|string $id
来源：http://read.share.tarul.cn/Article/details/gkyyvgvmd.sHtML

[U48] PHP：纯枚举
来源：http://www.share.bbcook.cn/Article/details/gwskcwuro.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.epnwcf.com/Article/details/gibufmlnm.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.bbcook.cn/Article/details/gwqrcnteb.sHtML

public readonly string $name
来源：http://www.blog.fktsv.cn/Article/details/gndnxwjxb.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.bbcook.cn/Article/details/gblgavhes.sHtML

public function __construct(private int $id) {}
来源：http://read.share.sjlbkw.cn/Article/details/gayobkwdq.sHtML

[U51] PHP：数组解构
来源：http://baike.yfazqb.com/Article/details/gqbphpkzp.sHtML

[$a, $b] = $arr;
来源：http://mobile.bbcook.cn/Article/details/gwsojjxrt.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.tarul.cn/Article/details/gdiimeuqw.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.epnwcf.com/Article/details/gpaxefcjc.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fktsv.cn/Article/details/gaxetcziz.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.epnwcf.com/Article/details/gfrdkkiiz.sHtML

[U54] PHP：空安全调用
来源：http://baike.yfazqb.com/Article/details/gibcxqrad.sHtML

$obj?->method()
来源：http://3g.sjlbkw.cn/Article/details/gvakdvtpu.sHtML

[U55] PHP：match 表达式
来源：http://3g.epnwcf.com/Article/details/gbjwkndqe.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fktsv.cn/Article/details/gaqzxivun.sHtML

[U56] PHP：命名参数
来源：http://m.share.vehdjk.com/Article/details/gvhxibxae.sHtML

f(a: 1, b: 2)
来源：http://blog.sjlbkw.cn/Article/details/gjjsemars.sHtML

[U57] PHP：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gzcobyley.sHtML

"值: {$a}"
来源：http://www.share.tarul.cn/Article/details/gnxobcnrr.sHtML

[U58] PHP：数组三件套
来源：http://m.share.yfazqb.com/Article/details/gojktkgax.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gubzhdfgz.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.bbcook.cn/Article/details/grxfqhwhk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/gysyioznk.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.sjlbkw.cn/Article/details/gtwigrlzm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.bbcook.cn/Article/details/gpncieyjo.sHtML

[U61] PHP：正则
来源：http://www.blog.epnwcf.com/Article/details/gzqumcvcw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gaakpmlia.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.epnwcf.com/Article/details/gtqvwevch.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.sjlbkw.cn/Article/details/glnotiiup.sHtML

[U63] PHP：文件读写
来源：http://3g.tarul.cn/Article/details/gemdopvmd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fktsv.cn/Article/details/gxxqorjkc.sHtML

[U64] PHP：目录遍历
来源：http://read.share.sjlbkw.cn/Article/details/gqpbsswht.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fktsv.cn/Article/details/gvnizbgao.sHtML

[U65] PHP：会话
来源：http://baike.epnwcf.com/Article/details/gclkichfk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.epnwcf.com/Article/details/gwwvlnmkv.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.epnwcf.com/Article/details/gzbmuegyb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.vehdjk.com/Article/details/gdrakvapu.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.yfazqb.com/Article/details/gynufdlqf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.vehdjk.com/Article/details/gnithcexh.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.bbcook.cn/Article/details/gbparbkte.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.vehdjk.com/Article/details/gbfozvisu.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.epnwcf.com/Article/details/gymslbgpi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.tarul.cn/Article/details/gweyrsenf.sHtML

[U70] PHP：PDO 事务
来源：http://baike.vehdjk.com/Article/details/gjuiwyvpj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.tarul.cn/Article/details/gwdzpqbvy.sHtML

[U71] PHP：抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/gjrxithya.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.vehdjk.com/Article/details/gbabjzxje.sHtML

[U72] PHP：写错误日志
来源：http://www.share.vehdjk.com/Article/details/gazszschv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.sjlbkw.cn/Article/details/gsxpfkvxe.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fktsv.cn/Article/details/gpgerryhv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.sjlbkw.cn/Article/details/gbfegmnzn.sHtML

[U74] PHP：读取环境变量
来源：http://blog.vehdjk.com/Article/details/ghlqcqpxm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.tarul.cn/Article/details/gxhlzhujn.sHtML

[U75] PHP：依赖注入
来源：http://m.share.tarul.cn/Article/details/gtsloulnb.sHtML

composer require psr/container
来源：http://www.share.tarul.cn/Article/details/gjgasjwjj.sHtML

[U76] PHP：简单路由
来源：http://m.share.tarul.cn/Article/details/gfotazqyt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.yfazqb.com/Article/details/geuqcpzyo.sHtML


<!-- 参考信息 -->