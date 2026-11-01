代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.bbcook.cn/Article/details/gpiyriihk.sHtML

[S55] C++：结构化绑定
来源：http://baike.bbcook.cn/Article/details/gdjiftvoc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fktsv.cn/Article/details/gqlgzwmfe.sHtML

[S56] C++：optional
来源：http://blog.yfazqb.com/Article/details/gdauzmsaw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.vehdjk.com/Article/details/gsbacwhke.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmicsecb.sHtML

constexpr int N = 10;
来源：http://www.m.share.tarul.cn/Article/details/gaxpvtomt.sHtML

[S58] C++：命名空间
来源：http://www.blog.epnwcf.com/Article/details/gqkeiipzm.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fktsv.cn/Article/details/gbqciqcno.sHtML

[S59] C++：静态断言
来源：http://read.share.epnwcf.com/Article/details/goxtvvdhd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.bbcook.cn/Article/details/gtmzxdnlt.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.epnwcf.com/Article/details/gpecdbupx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/gpsijfsjv.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gflmzvmnx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gvgxjrrhs.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gglmjqekq.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.yfazqb.com/Article/details/gitqsqqep.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/gnbgdkvin.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fktsv.cn/Article/details/ggibhdqus.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.vehdjk.com/Article/details/gxptchxkk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.bbcook.cn/Article/details/gphzlmgdu.sHtML

"值: $b"
来源：http://m.share.vehdjk.com/Article/details/geefouajt.sHtML

[T04] Kotlin：空安全
来源：http://baike.tarul.cn/Article/details/gjtukvpgn.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.tarul.cn/Article/details/gtvxlowxc.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.yfazqb.com/Article/details/gsygukigv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.epnwcf.com/Article/details/gjzvzccku.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gpbjivdzn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.bbcook.cn/Article/details/gznewzpbu.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.yfazqb.com/Article/details/gjisopiru.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.epnwcf.com/Article/details/gcsdufrvb.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fktsv.cn/Article/details/gnvibqsgv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.tarul.cn/Article/details/gxrbgafkk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.epnwcf.com/Article/details/grrsozvai.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.yfazqb.com/Article/details/ggzhslnuq.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fktsv.cn/Article/details/gxrnwykpt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.epnwcf.com/Article/details/gpvsiretp.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/gbsvtvcpn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.vehdjk.com/Article/details/gyihonxll.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.epnwcf.com/Article/details/gxljxewju.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gebgihkkg.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.epnwcf.com/Article/details/gzeeqixnk.sHtML

val m = mapOf("a" to 1)
来源：http://3g.vehdjk.com/Article/details/gsrfzqcke.sHtML

[T14] Kotlin：循环
来源：http://www.blog.yfazqb.com/Article/details/gaaveivjv.sHtML

for (i in 1..10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/ghsmprtrg.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.tarul.cn/Article/details/ggqdjhblw.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.yfazqb.com/Article/details/gdghgyfhy.sHtML

[T16] Swift：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gyolomcnw.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gbrrjhuzf.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fktsv.cn/Article/details/gccxgeqbh.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gglhcntee.sHtML

[T18] Swift：字符串插值
来源：http://3g.fktsv.cn/Article/details/guaevtjzt.sHtML

"值: \(b)"
来源：http://baike.vehdjk.com/Article/details/gawdiacdx.sHtML

[T19] Swift：可选绑定
来源：http://m.share.tarul.cn/Article/details/gjetwqgnx.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.vehdjk.com/Article/details/garznbygb.sHtML

[T20] Swift：数组操作
来源：http://www.share.fktsv.cn/Article/details/gujjftmoc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.bbcook.cn/Article/details/gjqndshkz.sHtML

[T21] Swift：遍历
来源：http://www.blog.vehdjk.com/Article/details/gsgvochex.sHtML

for x in a { print(x) }
来源：http://www.share.fktsv.cn/Article/details/gdovgfegh.sHtML

[T22] Swift：字典
来源：http://m.share.fktsv.cn/Article/details/gmekcgtqb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.sjlbkw.cn/Article/details/gwlrqffjb.sHtML

[T23] Swift：函数
来源：http://www.blog.vehdjk.com/Article/details/golrwbvlq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.tarul.cn/Article/details/gclpolsbx.sHtML

[T24] Swift：闭包
来源：http://read.share.bbcook.cn/Article/details/gzhzltlti.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/ggcusouur.sHtML

[T25] Swift：结构体
来源：http://www.share.tarul.cn/Article/details/gzesvhqev.sHtML

struct P { var x: Int }
来源：http://www.blog.yfazqb.com/Article/details/gcklnomvp.sHtML

[T26] Swift：类与重写
来源：http://m.share.epnwcf.com/Article/details/gfnbzvycg.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fktsv.cn/Article/details/ghonfmfib.sHtML

[T27] Swift：错误处理
来源：http://baike.bbcook.cn/Article/details/grndfwxqo.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.sjlbkw.cn/Article/details/glxchdfab.sHtML

[T28] Swift：枚举
来源：http://www.share.bbcook.cn/Article/details/gnrozjusc.sHtML

enum Color { case red, green }
来源：http://www.share.vehdjk.com/Article/details/geafcknwb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.bbcook.cn/Article/details/gyqwckjwc.sHtML

guard let x = opt else { return }
来源：http://wap.epnwcf.com/Article/details/gqpiusqan.sHtML

[T30] Swift：协议
来源：http://blog.sjlbkw.cn/Article/details/gzeowsdyg.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.bbcook.cn/Article/details/gbbqsjzzz.sHtML

[T31] Lua：Hello World
来源：http://baike.epnwcf.com/Article/details/gfhcqgimp.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gyqglrnls.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gjlgjquhq.sHtML

local a = 1
来源：http://wap.vehdjk.com/Article/details/ggljjvirj.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.bbcook.cn/Article/details/glxdairii.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.tarul.cn/Article/details/gjgrsipxe.sHtML

[T34] Lua：遍历表
来源：http://m.share.bbcook.cn/Article/details/gzhpqixhc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.sjlbkw.cn/Article/details/gsrrslgfu.sHtML

[T35] Lua：字典表
来源：http://wap.epnwcf.com/Article/details/gmvaqjeae.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.epnwcf.com/Article/details/gtoptjsdw.sHtML

[T36] Lua：函数
来源：http://mobile.epnwcf.com/Article/details/gowxendcp.sHtML

function add(a, b) return a + b end
来源：http://3g.vehdjk.com/Article/details/gwhukmkww.sHtML

[T37] Lua：字符串拼接
来源：http://wap.yfazqb.com/Article/details/gqnsyrxxz.sHtML

"a" .. "b"
来源：http://baike.fktsv.cn/Article/details/gmbnelwvw.sHtML

[T38] Lua：条件
来源：http://blog.yfazqb.com/Article/details/gfobcfpht.sHtML

if x > 0 then print("正") end
来源：http://baike.bbcook.cn/Article/details/gbyplcqay.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/ghbmakgld.sHtML

string.find(s, "%d+")
来源：http://wap.sjlbkw.cn/Article/details/ghaizkrrs.sHtML

[T40] Lua：元表
来源：http://baike.fktsv.cn/Article/details/gtfphmhtv.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.sjlbkw.cn/Article/details/gsxctilda.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gzncwfrfa.sHtML

print "Hello\n";
来源：http://mobile.tarul.cn/Article/details/ggislpsil.sHtML

[T42] Perl：变量类型
来源：http://www.share.sjlbkw.cn/Article/details/gphrkwqcf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.yfazqb.com/Article/details/gvpslayes.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gxuresvhx.sHtML

"值: $a"
来源：http://read.share.bbcook.cn/Article/details/grofppdtd.sHtML

[T44] Perl：条件
来源：http://blog.tarul.cn/Article/details/gitltlbrh.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.sjlbkw.cn/Article/details/gzjvmfvoe.sHtML

[T45] Perl：数组遍历
来源：http://www.share.epnwcf.com/Article/details/gsyndhuwh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.tarul.cn/Article/details/gqhusdrbj.sHtML

[T46] Perl：哈希操作
来源：http://blog.fktsv.cn/Article/details/gabqjjrfc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.vehdjk.com/Article/details/gjdtzcyof.sHtML

[T47] Perl：正则捕获
来源：http://wap.yfazqb.com/Article/details/gtdjxogrt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.epnwcf.com/Article/details/ghnlyswvj.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fktsv.cn/Article/details/gcvlwcyzv.sHtML

$s =~ s/old/new/g;
来源：http://read.share.epnwcf.com/Article/details/geqyvsyxm.sHtML

[T49] Perl：函数
来源：http://mobile.yfazqb.com/Article/details/gqfqlodoe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gmlioxlsq.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gbolozsig.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.yfazqb.com/Article/details/gnykyikkp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.epnwcf.com/Article/details/gwgmlzjgh.sHtML

[T51] Scala：Hello World
来源：http://mobile.tarul.cn/Article/details/gfplyqzpp.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/gcsnddjji.sHtML

[T52] Scala：变量
来源：http://m.share.sjlbkw.cn/Article/details/gzzcxyiop.sHtML

val a = 1;  var b = 2
来源：http://wap.vehdjk.com/Article/details/gayhizzum.sHtML

[T53] Scala：字符串插值
来源：http://blog.epnwcf.com/Article/details/gmeohpjfy.sHtML

s"值: $b"
来源：http://3g.tarul.cn/Article/details/gbbuuvpcu.sHtML

[T54] Scala：集合映射
来源：http://read.share.vehdjk.com/Article/details/gvxmbvpfa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.epnwcf.com/Article/details/gaembmjzm.sHtML

[T55] Scala：集合过滤
来源：http://m.share.bbcook.cn/Article/details/grwdxzyrj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.tarul.cn/Article/details/gvdyggrva.sHtML

[T56] Scala：样例类
来源：http://www.blog.epnwcf.com/Article/details/gugcksulh.sHtML

case class User(name: String, age: Int)
来源：http://mobile.vehdjk.com/Article/details/gitoambxl.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fktsv.cn/Article/details/gmgetoqzl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.tarul.cn/Article/details/ghhwdujga.sHtML

[T58] Scala：函数定义
来源：http://m.share.vehdjk.com/Article/details/ghqflsjtu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fktsv.cn/Article/details/gnwccabnn.sHtML

[T59] Scala：循环
来源：http://mobile.vehdjk.com/Article/details/gfrbwprcp.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.yfazqb.com/Article/details/grmduszhs.sHtML

[T60] Scala：折叠
来源：http://mobile.epnwcf.com/Article/details/gwizxbwrg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.sjlbkw.cn/Article/details/gunptrosp.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gbovzfqeq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.yfazqb.com/Article/details/gyjwktcqm.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmauzoiun.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.epnwcf.com/Article/details/gejcpbjnf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fktsv.cn/Article/details/glphlbesv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fktsv.cn/Article/details/gsfimzksw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.vehdjk.com/Article/details/gofviqcbu.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.bbcook.cn/Article/details/guuxxcnbz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.vehdjk.com/Article/details/geogmuvza.sHtML

[U04] Py：变量调试打印
来源：http://wap.vehdjk.com/Article/details/gpxltnwhf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.epnwcf.com/Article/details/gxrpohkwy.sHtML

[U05] Py：列表去重且保序
来源：http://wap.epnwcf.com/Article/details/gomngjzat.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/gjidxmtcu.sHtML

[U06] Py：合并两个字典
来源：http://mobile.bbcook.cn/Article/details/gsxbffaiv.sHtML

{**a, **b}
来源：http://blog.tarul.cn/Article/details/ghdqbyhmv.sHtML

[U07] Py：反转字典键值
来源：http://baike.bbcook.cn/Article/details/ghuaemuog.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.vehdjk.com/Article/details/ggcmhgols.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.bbcook.cn/Article/details/gxwoezqwp.sHtML

[y for x in nested for y in x]
来源：http://mobile.fktsv.cn/Article/details/gggrvbkba.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.yfazqb.com/Article/details/gxtpkbjoo.sHtML

max(d, key=d.get)
来源：http://read.share.vehdjk.com/Article/details/grqwhycas.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fktsv.cn/Article/details/gsaltyndu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.bbcook.cn/Article/details/gaidstfqv.sHtML

[U11] Py：生成器表达式
来源：http://baike.sjlbkw.cn/Article/details/gqiibxyxz.sHtML

(x * 2 for x in arr)
来源：http://mobile.fktsv.cn/Article/details/gchqgnbiy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.bbcook.cn/Article/details/gcysoofbn.sHtML

Counter(arr).most_common(3)
来源：http://m.share.bbcook.cn/Article/details/gwvhsnmnt.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.yfazqb.com/Article/details/gdzjsewyq.sHtML

deque(maxlen=10)
来源：http://m.share.tarul.cn/Article/details/gcwcffpve.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.tarul.cn/Article/details/gmhmmfuxh.sHtML

defaultdict(list)
来源：http://read.share.sjlbkw.cn/Article/details/goqnywyhm.sHtML

[U15] Py：高精度计时
来源：http://mobile.tarul.cn/Article/details/gciwdphww.sHtML

t = time.perf_counter()
来源：http://wap.sjlbkw.cn/Article/details/gwscswovf.sHtML

[U16] Py：命令行参数解析
来源：http://wap.vehdjk.com/Article/details/gdzkllzck.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.tarul.cn/Article/details/gzhrxfdsb.sHtML

[U17] Py：初始化日志
来源：http://3g.tarul.cn/Article/details/gyyzdqkyo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.yfazqb.com/Article/details/gqvfqltyr.sHtML

[U18] Py：预编译正则
来源：http://blog.tarul.cn/Article/details/gvxetiaua.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.tarul.cn/Article/details/gvgvkpvzk.sHtML

[U19] Py：正则替换带回调
来源：http://blog.tarul.cn/Article/details/gjcdpczjl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.vehdjk.com/Article/details/glpumxgab.sHtML

[U20] Py：缓存函数结果
来源：http://wap.bbcook.cn/Article/details/gvhnvttaw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.bbcook.cn/Article/details/gvnuxpnmb.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.sjlbkw.cn/Article/details/gxekheggk.sHtML

@contextlib.contextmanager
来源：http://baike.vehdjk.com/Article/details/goxfdwurj.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.bbcook.cn/Article/details/grehkbrbv.sHtML

list(zip(*m))
来源：http://baike.vehdjk.com/Article/details/gghgmlbsu.sHtML

[U23] Py：分块读取大文件
来源：http://3g.yfazqb.com/Article/details/ghlhvdegm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.sjlbkw.cn/Article/details/gmpofprwn.sHtML

[U24] Py：路径操作
来源：http://mobile.tarul.cn/Article/details/ggyimozdy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgyvzacn.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.epnwcf.com/Article/details/ganfxzpnl.sHtML

csv.DictReader(f)
来源：http://www.blog.yfazqb.com/Article/details/gjxyiqwbw.sHtML

[U26] Py：并发下载
来源：http://read.share.sjlbkw.cn/Article/details/gnurkgzps.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fktsv.cn/Article/details/gkpguohtj.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.tarul.cn/Article/details/gjsyrrenq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.epnwcf.com/Article/details/ghbnnnvmt.sHtML

[U28] Py：类型别名
来源：http://mobile.fktsv.cn/Article/details/gaaoneqjt.sHtML

UserId = int
来源：http://baike.sjlbkw.cn/Article/details/gqbbyejle.sHtML

[U29] Py：属性校验
来源：http://mobile.sjlbkw.cn/Article/details/gkrlgipjr.sHtML

@property 与 @x.setter 配合
来源：http://www.share.vehdjk.com/Article/details/gexdcmteo.sHtML

[U30] Py：数据类
来源：http://blog.tarul.cn/Article/details/gcsnfmjpa.sHtML

@dataclass(slots=True)
来源：http://baike.tarul.cn/Article/details/giwuvkded.sHtML

[U31] Py：单测
来源：http://blog.yfazqb.com/Article/details/gtrxfzneg.sHtML

python -m pytest -q
来源：http://m.share.bbcook.cn/Article/details/gqcsczowu.sHtML

[U32] Py：代码格式化
来源：http://mobile.fktsv.cn/Article/details/gfrycurxt.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.bbcook.cn/Article/details/gtghpkcqp.sHtML

[U33] Py：打包发布
来源：http://mobile.epnwcf.com/Article/details/gnyuurrby.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.vehdjk.com/Article/details/gonbachjm.sHtML

[U34] Py：判断编码
来源：http://m.share.epnwcf.com/Article/details/gnyxvpqxe.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/gnakjmnmv.sHtML

[U35] Py：发送邮件
来源：http://baike.vehdjk.com/Article/details/gbhjjxcew.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.bbcook.cn/Article/details/gzbqvdxpq.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fktsv.cn/Article/details/gctrcjtac.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.tarul.cn/Article/details/gddflcnkd.sHtML

[U37] Py：读写 Excel
来源：http://read.share.yfazqb.com/Article/details/gikttwntv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.tarul.cn/Article/details/gacfnueqi.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.vehdjk.com/Article/details/gsxydituh.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fktsv.cn/Article/details/gcjquubrq.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fktsv.cn/Article/details/gnntaaeyc.sHtML

sys.stdout.isatty()
来源：http://www.m.share.bbcook.cn/Article/details/gamvpneus.sHtML

[U40] Py：打印到标准错误
来源：http://wap.bbcook.cn/Article/details/gbhfosbms.sHtML

print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/gfglhvrfd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.vehdjk.com/Article/details/gfjmwftrw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fktsv.cn/Article/details/gwtggkban.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fktsv.cn/Article/details/gywjmhqda.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fktsv.cn/Article/details/gspaaqdgm.sHtML

[U43] PHP：声明命名空间
来源：http://baike.yfazqb.com/Article/details/gaisthvux.sHtML

namespace App\Http;
来源：http://m.share.tarul.cn/Article/details/gxdppgweb.sHtML

[U44] PHP：开启严格类型
来源：http://blog.sjlbkw.cn/Article/details/gfcfqbsny.sHtML

declare(strict_types=1);
来源：http://www.m.share.vehdjk.com/Article/details/gmqsecbin.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.sjlbkw.cn/Article/details/gqypmehge.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gswhyvyzg.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fktsv.cn/Article/details/ghkqtrssm.sHtML

?string $name = null
来源：http://m.share.epnwcf.com/Article/details/gfwdkbvsl.sHtML

[U47] PHP：联合类型
来源：http://wap.tarul.cn/Article/details/gyjhctrkd.sHtML

int|string $id
来源：http://www.share.bbcook.cn/Article/details/gsplszral.sHtML

[U48] PHP：纯枚举
来源：http://baike.sjlbkw.cn/Article/details/gepikchke.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.sjlbkw.cn/Article/details/gyaidyita.sHtML

[U49] PHP：只读属性
来源：http://mobile.fktsv.cn/Article/details/ggwnyhyhy.sHtML

public readonly string $name
来源：http://m.share.yfazqb.com/Article/details/grdlmnezy.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.epnwcf.com/Article/details/gekyekiro.sHtML

public function __construct(private int $id) {}
来源：http://www.share.tarul.cn/Article/details/gpwyvemak.sHtML

[U51] PHP：数组解构
来源：http://read.share.yfazqb.com/Article/details/gsninyalo.sHtML

[$a, $b] = $arr;
来源：http://read.share.yfazqb.com/Article/details/gsyilwwlc.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fktsv.cn/Article/details/gjlkkqnul.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fktsv.cn/Article/details/gffhgyaxe.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.epnwcf.com/Article/details/gtqsognrd.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.tarul.cn/Article/details/gebbcuhid.sHtML

[U54] PHP：空安全调用
来源：http://www.share.bbcook.cn/Article/details/gvabanqfc.sHtML

$obj?->method()
来源：http://www.blog.sjlbkw.cn/Article/details/gcqzveeod.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gjelisxtu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.tarul.cn/Article/details/gwxcxqcaz.sHtML

[U56] PHP：命名参数
来源：http://read.share.yfazqb.com/Article/details/gxawzgnci.sHtML

f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gsiafqwvk.sHtML

[U57] PHP：字符串插值
来源：http://blog.fktsv.cn/Article/details/gywftisww.sHtML

"值: {$a}"
来源：http://3g.fktsv.cn/Article/details/gzvlnhgzo.sHtML

[U58] PHP：数组三件套
来源：http://m.share.sjlbkw.cn/Article/details/getiiljjo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gwubcfyno.sHtML

[U59] PHP：自定义排序
来源：http://blog.yfazqb.com/Article/details/gurjpofhn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.epnwcf.com/Article/details/gsdrnysam.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.bbcook.cn/Article/details/gnmvtflnr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.bbcook.cn/Article/details/gylhqycfx.sHtML

[U61] PHP：正则
来源：http://www.m.share.bbcook.cn/Article/details/gaasnduvm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.tarul.cn/Article/details/gnhtwkikh.sHtML

[U62] PHP：日期对象
来源：http://baike.sjlbkw.cn/Article/details/glnfpvpdf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.yfazqb.com/Article/details/giyzlzixi.sHtML

[U63] PHP：文件读写
来源：http://wap.sjlbkw.cn/Article/details/grqyolydt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.epnwcf.com/Article/details/gwcgufmlc.sHtML

[U64] PHP：目录遍历
来源：http://m.share.bbcook.cn/Article/details/ghznxgkxo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.bbcook.cn/Article/details/gwqbclvhg.sHtML

[U65] PHP：会话
来源：http://www.blog.sjlbkw.cn/Article/details/gbrycnzbl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gsrpducws.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.epnwcf.com/Article/details/gdidsmqpw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.vehdjk.com/Article/details/gtvpaqoic.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.tarul.cn/Article/details/gpetpgedm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.epnwcf.com/Article/details/giayxetzi.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.sjlbkw.cn/Article/details/gyblizwvm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvougukkd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.epnwcf.com/Article/details/gawwjuntf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.bbcook.cn/Article/details/gkcgytwqw.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.sjlbkw.cn/Article/details/gszmjesvp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.yfazqb.com/Article/details/gsctmcxzl.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gpvebiygj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.sjlbkw.cn/Article/details/gdraeolpq.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.tarul.cn/Article/details/gpkwuqpve.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.sjlbkw.cn/Article/details/giqndmxwi.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.bbcook.cn/Article/details/gglqkvitu.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.tarul.cn/Article/details/gscjgdznd.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gzybyzjes.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fktsv.cn/Article/details/gnrfeolaw.sHtML

[U75] PHP：依赖注入
来源：http://www.share.epnwcf.com/Article/details/gipnrieqy.sHtML

composer require psr/container
来源：http://mobile.yfazqb.com/Article/details/grxyphoks.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fktsv.cn/Article/details/gfmbouucf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.sjlbkw.cn/Article/details/gsmqkpktg.sHtML

[U77] PHP：模板渲染
来源：http://m.share.tarul.cn/Article/details/gincjdjap.sHtML

composer require twig/twig
来源：http://baike.yfazqb.com/Article/details/glkjdwrcf.sHtML

[U78] PHP：单元测试
来源：http://read.share.epnwcf.com/Article/details/goqbydowg.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.vehdjk.com/Article/details/groorfjda.sHtML

[U79] PHP：静态分析
来源：http://www.share.epnwcf.com/Article/details/gxrypwixl.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.epnwcf.com/Article/details/gknhndzdh.sHtML

[U80] PHP：代码规范修复
来源：http://blog.sjlbkw.cn/Article/details/gicqdqwwz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.bbcook.cn/Article/details/gxiyvimll.sHtML


<!-- 参考信息 -->