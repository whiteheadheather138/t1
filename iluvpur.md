代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://mobile.bbcook.cn/Article/details/gmpvfsihq.sHtML

[S59] C++：静态断言
来源：http://www.m.share.vehdjk.com/Article/details/gzwcgakkk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.bbcook.cn/Article/details/gvpgsrthx.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.bbcook.cn/Article/details/gukqhrmok.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/geozyqmwb.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gyjyiqcya.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.bbcook.cn/Article/details/gbheyadii.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gasdmykii.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.bbcook.cn/Article/details/gbdvdxqxs.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/gcvcnadff.sHtML

[T02] Kotlin：变量
来源：http://m.share.fktsv.cn/Article/details/gqixtpzyf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.epnwcf.com/Article/details/gbwglrwii.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/ggbtyivjm.sHtML

"值: $b"
来源：http://m.share.bbcook.cn/Article/details/gnzmmkeug.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/gqmdrknpm.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.tarul.cn/Article/details/gvdafvndo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.epnwcf.com/Article/details/gmxqfogpn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.vehdjk.com/Article/details/gzoxegkwu.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.tarul.cn/Article/details/gjasyqafi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fktsv.cn/Article/details/gzefxtdoa.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gslgamker.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.yfazqb.com/Article/details/grcvydzlu.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.epnwcf.com/Article/details/grwpbrqph.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.tarul.cn/Article/details/gmgoufsiu.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.sjlbkw.cn/Article/details/guwymotzm.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fktsv.cn/Article/details/ggclermcw.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.vehdjk.com/Article/details/gixmjvozl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.epnwcf.com/Article/details/gkktikehl.sHtML

[T11] Kotlin：协程
来源：http://www.blog.bbcook.cn/Article/details/gagfevzop.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.vehdjk.com/Article/details/gzzecepio.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.epnwcf.com/Article/details/graxekalb.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gxzjubrjv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.bbcook.cn/Article/details/grhihjekj.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.vehdjk.com/Article/details/gndcynyyd.sHtML

[T14] Kotlin：循环
来源：http://wap.sjlbkw.cn/Article/details/gqcavscku.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fktsv.cn/Article/details/gxonsican.sHtML

[T15] Kotlin：接口
来源：http://www.share.fktsv.cn/Article/details/gbrxgnpnv.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.yfazqb.com/Article/details/gnvydyntt.sHtML

[T16] Swift：Hello World
来源：http://baike.bbcook.cn/Article/details/gilvwobzj.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gloxpjalq.sHtML

[T17] Swift：变量与常量
来源：http://mobile.tarul.cn/Article/details/gkkmfjzni.sHtML

var a = 1;  let b = 2
来源：http://read.share.yfazqb.com/Article/details/gjulxqpko.sHtML

[T18] Swift：字符串插值
来源：http://baike.yfazqb.com/Article/details/gfynfvmfp.sHtML

"值: \(b)"
来源：http://www.m.share.vehdjk.com/Article/details/gjyzlrvli.sHtML

[T19] Swift：可选绑定
来源：http://m.share.bbcook.cn/Article/details/gqyyhxnro.sHtML

if let n = opt { print(n) }
来源：http://read.share.fktsv.cn/Article/details/gloypinuz.sHtML

[T20] Swift：数组操作
来源：http://baike.fktsv.cn/Article/details/gijzphwqq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.bbcook.cn/Article/details/gyuiqddva.sHtML

[T21] Swift：遍历
来源：http://baike.yfazqb.com/Article/details/gqaijyxmi.sHtML

for x in a { print(x) }
来源：http://m.share.sjlbkw.cn/Article/details/gowgbauyj.sHtML

[T22] Swift：字典
来源：http://read.share.epnwcf.com/Article/details/gopjfebms.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.sjlbkw.cn/Article/details/gqqytmppe.sHtML

[T23] Swift：函数
来源：http://blog.bbcook.cn/Article/details/gxejltwsd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.bbcook.cn/Article/details/govfvysrw.sHtML

[T24] Swift：闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmerpbpj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.bbcook.cn/Article/details/gxsietudf.sHtML

[T25] Swift：结构体
来源：http://www.share.vehdjk.com/Article/details/gphpzmnoi.sHtML

struct P { var x: Int }
来源：http://www.m.share.fktsv.cn/Article/details/gxydhcszd.sHtML

[T26] Swift：类与重写
来源：http://m.share.yfazqb.com/Article/details/gpkttrlzd.sHtML

class A: Base { override func f() {} }
来源：http://mobile.yfazqb.com/Article/details/gobfqnjej.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gplqxflwt.sHtML

do { try f() } catch { print(error) }
来源：http://3g.yfazqb.com/Article/details/gthwipift.sHtML

[T28] Swift：枚举
来源：http://www.blog.bbcook.cn/Article/details/gclxzsptq.sHtML

enum Color { case red, green }
来源：http://www.blog.tarul.cn/Article/details/gemgkjhcg.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.sjlbkw.cn/Article/details/gjhrbqyhi.sHtML

guard let x = opt else { return }
来源：http://www.blog.yfazqb.com/Article/details/gddcviyng.sHtML

[T30] Swift：协议
来源：http://m.share.epnwcf.com/Article/details/gtsddkrja.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.bbcook.cn/Article/details/gsvajtzch.sHtML

[T31] Lua：Hello World
来源：http://mobile.yfazqb.com/Article/details/gnkvybcmi.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gcfwkeyin.sHtML

[T32] Lua：局部变量
来源：http://read.share.yfazqb.com/Article/details/gdyrbxifp.sHtML

local a = 1
来源：http://www.share.tarul.cn/Article/details/gjklztsgr.sHtML

[T33] Lua：表（数组）
来源：http://www.share.vehdjk.com/Article/details/gaxffcsze.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.sjlbkw.cn/Article/details/gpxfzjukq.sHtML

[T34] Lua：遍历表
来源：http://wap.tarul.cn/Article/details/gvasfhcns.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fktsv.cn/Article/details/gzcqvefoq.sHtML

[T35] Lua：字典表
来源：http://baike.sjlbkw.cn/Article/details/gqimmqtcw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.vehdjk.com/Article/details/gshqaygxd.sHtML

[T36] Lua：函数
来源：http://3g.epnwcf.com/Article/details/gihhujtdj.sHtML

function add(a, b) return a + b end
来源：http://baike.fktsv.cn/Article/details/gsidnrpjc.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/gtxtitunk.sHtML

"a" .. "b"
来源：http://www.m.share.tarul.cn/Article/details/gtzdpdzmj.sHtML

[T38] Lua：条件
来源：http://www.blog.fktsv.cn/Article/details/gmkfdlicr.sHtML

if x > 0 then print("正") end
来源：http://blog.sjlbkw.cn/Article/details/gzrcesedh.sHtML

[T39] Lua：模式匹配
来源：http://baike.epnwcf.com/Article/details/gdhkyrhzi.sHtML

string.find(s, "%d+")
来源：http://baike.epnwcf.com/Article/details/gefkupzny.sHtML

[T40] Lua：元表
来源：http://www.blog.yfazqb.com/Article/details/gakcljouc.sHtML

setmetatable({}, { __index = base })
来源：http://baike.vehdjk.com/Article/details/gxmxbmcle.sHtML

[T41] Perl：Hello World
来源：http://m.share.vehdjk.com/Article/details/gjujyinng.sHtML

print "Hello\n";
来源：http://www.m.share.yfazqb.com/Article/details/gcxwmqzrb.sHtML

[T42] Perl：变量类型
来源：http://mobile.epnwcf.com/Article/details/gdcxinpbw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.vehdjk.com/Article/details/gliyuplmg.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gfrkiiekd.sHtML

"值: $a"
来源：http://baike.epnwcf.com/Article/details/gojfpadpd.sHtML

[T44] Perl：条件
来源：http://www.blog.sjlbkw.cn/Article/details/gwyfqklqf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.bbcook.cn/Article/details/gjuqszkwo.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.yfazqb.com/Article/details/gmhfkwymi.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fktsv.cn/Article/details/gclcfxnpl.sHtML

[T46] Perl：哈希操作
来源：http://wap.epnwcf.com/Article/details/giyvptmzs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.yfazqb.com/Article/details/gshcjotml.sHtML

[T47] Perl：正则捕获
来源：http://wap.sjlbkw.cn/Article/details/gqecvoxho.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.yfazqb.com/Article/details/geazernwm.sHtML

[T48] Perl：正则替换
来源：http://m.share.sjlbkw.cn/Article/details/gihhdkqdh.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.epnwcf.com/Article/details/gbllaszti.sHtML

[T49] Perl：函数
来源：http://www.share.fktsv.cn/Article/details/gvyhdchpa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gvzapybhs.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gtpuzecdv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.tarul.cn/Article/details/gvizsuenc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.tarul.cn/Article/details/gyckbtpqy.sHtML

[T51] Scala：Hello World
来源：http://www.share.vehdjk.com/Article/details/gvfjkjjwp.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/gvwavverz.sHtML

[T52] Scala：变量
来源：http://www.m.share.vehdjk.com/Article/details/gxdktplsq.sHtML

val a = 1;  var b = 2
来源：http://blog.bbcook.cn/Article/details/gcunkdppw.sHtML

[T53] Scala：字符串插值
来源：http://mobile.tarul.cn/Article/details/glvxkmhlz.sHtML

s"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gebakarbw.sHtML

[T54] Scala：集合映射
来源：http://mobile.yfazqb.com/Article/details/gwublqmvv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gjizjmbvk.sHtML

[T55] Scala：集合过滤
来源：http://read.share.tarul.cn/Article/details/gsgqxwtye.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fktsv.cn/Article/details/gqwxmelzw.sHtML

[T56] Scala：样例类
来源：http://m.share.sjlbkw.cn/Article/details/gzmuxxmfr.sHtML

case class User(name: String, age: Int)
来源：http://wap.epnwcf.com/Article/details/gztkuutwj.sHtML

[T57] Scala：模式匹配
来源：http://read.share.epnwcf.com/Article/details/gnmaugvag.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gwfpqpgto.sHtML

[T58] Scala：函数定义
来源：http://3g.vehdjk.com/Article/details/gotbzqcav.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.tarul.cn/Article/details/gqcgqaqsq.sHtML

[T59] Scala：循环
来源：http://3g.fktsv.cn/Article/details/gprxjnqhw.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.tarul.cn/Article/details/gpmjifrsu.sHtML

[T60] Scala：折叠
来源：http://m.share.bbcook.cn/Article/details/gdjwvoohi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fktsv.cn/Article/details/gizuxxjom.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjygkvbxo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/gzcvaihjo.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gtukkyyzm.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.epnwcf.com/Article/details/ghudfcpyq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.tarul.cn/Article/details/gbyuigoth.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.epnwcf.com/Article/details/gjgurajvt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.sjlbkw.cn/Article/details/glgcnzihz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.tarul.cn/Article/details/gfeakuach.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fktsv.cn/Article/details/gzayjujef.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fktsv.cn/Article/details/gbdkbkwum.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.yfazqb.com/Article/details/gzdwqnbjw.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.vehdjk.com/Article/details/gozfzshpc.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fktsv.cn/Article/details/gofezfvus.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.yfazqb.com/Article/details/gojndnxsh.sHtML

{**a, **b}
来源：http://wap.sjlbkw.cn/Article/details/ghhjdoacz.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.bbcook.cn/Article/details/grwfcslnz.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.vehdjk.com/Article/details/gwtvwwbeb.sHtML

[U08] Py：展平二维列表
来源：http://m.share.vehdjk.com/Article/details/gvjqrsjpw.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.tarul.cn/Article/details/gofptyfhc.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.sjlbkw.cn/Article/details/gtrrlcgeh.sHtML

max(d, key=d.get)
来源：http://m.share.sjlbkw.cn/Article/details/gybtbqqbu.sHtML

[U10] Py：按值排序字典
来源：http://wap.bbcook.cn/Article/details/ggqskcytv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fktsv.cn/Article/details/guiwnenkw.sHtML

[U11] Py：生成器表达式
来源：http://3g.fktsv.cn/Article/details/ggrlnpoqn.sHtML

(x * 2 for x in arr)
来源：http://mobile.sjlbkw.cn/Article/details/gozwaysgy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.yfazqb.com/Article/details/grajuyjov.sHtML

Counter(arr).most_common(3)
来源：http://wap.tarul.cn/Article/details/gusjozell.sHtML

[U13] Py：固定长度队列
来源：http://3g.sjlbkw.cn/Article/details/goadqcory.sHtML

deque(maxlen=10)
来源：http://blog.bbcook.cn/Article/details/gswjyokiu.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fktsv.cn/Article/details/gdnraznkl.sHtML

defaultdict(list)
来源：http://wap.bbcook.cn/Article/details/gaqpdoqfw.sHtML

[U15] Py：高精度计时
来源：http://mobile.yfazqb.com/Article/details/ghjismanc.sHtML

t = time.perf_counter()
来源：http://wap.fktsv.cn/Article/details/gzcnuzjwn.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fktsv.cn/Article/details/gvcmyrizp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.epnwcf.com/Article/details/gylsmoakr.sHtML

[U17] Py：初始化日志
来源：http://3g.bbcook.cn/Article/details/gerundtpw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.sjlbkw.cn/Article/details/gcwuxffbc.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fktsv.cn/Article/details/gowgilaze.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/goatguosb.sHtML

[U19] Py：正则替换带回调
来源：http://3g.epnwcf.com/Article/details/gbyulovjr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.vehdjk.com/Article/details/grmxhqmrq.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.vehdjk.com/Article/details/gwiahetap.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyygzhxh.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.vehdjk.com/Article/details/gwtqwwqpd.sHtML

@contextlib.contextmanager
来源：http://m.share.sjlbkw.cn/Article/details/geuvxxved.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.tarul.cn/Article/details/getglmroz.sHtML

list(zip(*m))
来源：http://wap.vehdjk.com/Article/details/gqjsqoyty.sHtML

[U23] Py：分块读取大文件
来源：http://blog.sjlbkw.cn/Article/details/gpasksoxo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.epnwcf.com/Article/details/gruojcamo.sHtML

[U24] Py：路径操作
来源：http://blog.sjlbkw.cn/Article/details/gndsgfmtp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.epnwcf.com/Article/details/gedrsdzwl.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fktsv.cn/Article/details/gkvtaxhie.sHtML

csv.DictReader(f)
来源：http://read.share.fktsv.cn/Article/details/goqmmzywb.sHtML

[U26] Py：并发下载
来源：http://3g.fktsv.cn/Article/details/gboiatrdr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.yfazqb.com/Article/details/gcoqvctjh.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.yfazqb.com/Article/details/guodoydbf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.bbcook.cn/Article/details/gqwsukkwq.sHtML

[U28] Py：类型别名
来源：http://baike.vehdjk.com/Article/details/gcrxuvonz.sHtML

UserId = int
来源：http://wap.bbcook.cn/Article/details/gezpuzfxi.sHtML

[U29] Py：属性校验
来源：http://blog.fktsv.cn/Article/details/gnqertqsh.sHtML

@property 与 @x.setter 配合
来源：http://www.share.vehdjk.com/Article/details/gkltwvqzy.sHtML

[U30] Py：数据类
来源：http://m.share.epnwcf.com/Article/details/gkybtqbcm.sHtML

@dataclass(slots=True)
来源：http://blog.sjlbkw.cn/Article/details/gbajixjrk.sHtML

[U31] Py：单测
来源：http://read.share.vehdjk.com/Article/details/guhmfsuob.sHtML

python -m pytest -q
来源：http://wap.sjlbkw.cn/Article/details/gvmyeitno.sHtML

[U32] Py：代码格式化
来源：http://baike.epnwcf.com/Article/details/gukepwbkf.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.tarul.cn/Article/details/gygzarons.sHtML

[U33] Py：打包发布
来源：http://baike.epnwcf.com/Article/details/gfozhutle.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.tarul.cn/Article/details/gqetrdatf.sHtML

[U34] Py：判断编码
来源：http://read.share.tarul.cn/Article/details/gczbkplky.sHtML

chardet.detect(raw)
来源：http://wap.epnwcf.com/Article/details/gjwizevbu.sHtML

[U35] Py：发送邮件
来源：http://www.blog.tarul.cn/Article/details/gbeicxnrw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.epnwcf.com/Article/details/gcfljaurz.sHtML

[U36] Py：定时任务
来源：http://www.blog.yfazqb.com/Article/details/gspzwmxny.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.bbcook.cn/Article/details/gfjyhjmrh.sHtML

[U37] Py：读写 Excel
来源：http://blog.vehdjk.com/Article/details/gbeicfoln.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.yfazqb.com/Article/details/ggqbxmmdk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fktsv.cn/Article/details/gnyoxifyw.sHtML

Path(__file__).resolve().parent
来源：http://baike.yfazqb.com/Article/details/gmakngxrh.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.tarul.cn/Article/details/ggbauuykr.sHtML

sys.stdout.isatty()
来源：http://mobile.tarul.cn/Article/details/gllybyvof.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fktsv.cn/Article/details/grfsgmpbd.sHtML

print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gagpailei.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.vehdjk.com/Article/details/ggmmtvayf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.tarul.cn/Article/details/gzbsvfsth.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fktsv.cn/Article/details/gaakgvuws.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.tarul.cn/Article/details/gtzklzncq.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.tarul.cn/Article/details/gsuwisthf.sHtML

namespace App\Http;
来源：http://mobile.tarul.cn/Article/details/geqrxhcqq.sHtML

[U44] PHP：开启严格类型
来源：http://blog.sjlbkw.cn/Article/details/gnmdmcfqo.sHtML

declare(strict_types=1);
来源：http://www.share.tarul.cn/Article/details/gnssnpysz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fktsv.cn/Article/details/gcyxacjbt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gaddhwitq.sHtML

[U46] PHP：可空类型
来源：http://wap.vehdjk.com/Article/details/gdmnawvon.sHtML

?string $name = null
来源：http://wap.tarul.cn/Article/details/garlqcdpy.sHtML

[U47] PHP：联合类型
来源：http://wap.tarul.cn/Article/details/glwfwpbwe.sHtML

int|string $id
来源：http://blog.tarul.cn/Article/details/gfnvplroq.sHtML

[U48] PHP：纯枚举
来源：http://wap.sjlbkw.cn/Article/details/gptibntef.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.sjlbkw.cn/Article/details/glrgkpsbz.sHtML

[U49] PHP：只读属性
来源：http://www.blog.epnwcf.com/Article/details/gbhkzezdm.sHtML

public readonly string $name
来源：http://m.share.yfazqb.com/Article/details/guwhtmpwt.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.yfazqb.com/Article/details/gvdnfieqo.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.tarul.cn/Article/details/grevglbbn.sHtML

[U51] PHP：数组解构
来源：http://www.blog.bbcook.cn/Article/details/gruwkbswv.sHtML

[$a, $b] = $arr;
来源：http://mobile.bbcook.cn/Article/details/gwpphrsuw.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.vehdjk.com/Article/details/gpiilzfoe.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fktsv.cn/Article/details/ghndlpfjl.sHtML

[U53] PHP：空合并运算符
来源：http://baike.tarul.cn/Article/details/gvcwajlpl.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.bbcook.cn/Article/details/gxqietmse.sHtML

[U54] PHP：空安全调用
来源：http://read.share.bbcook.cn/Article/details/gzujghzby.sHtML

$obj?->method()
来源：http://mobile.fktsv.cn/Article/details/gdftealci.sHtML

[U55] PHP：match 表达式
来源：http://3g.tarul.cn/Article/details/gavrqkcrk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.tarul.cn/Article/details/gtllbvtck.sHtML

[U56] PHP：命名参数
来源：http://blog.tarul.cn/Article/details/gzcmkuwzr.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/ghwrjflfb.sHtML

[U57] PHP：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gkwpzjdcv.sHtML

"值: {$a}"
来源：http://m.share.vehdjk.com/Article/details/gcblynpxu.sHtML

[U58] PHP：数组三件套
来源：http://mobile.sjlbkw.cn/Article/details/gostpjfvu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.yfazqb.com/Article/details/gudfuivxc.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.bbcook.cn/Article/details/gfbgslnkw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.bbcook.cn/Article/details/gimrkvwws.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fktsv.cn/Article/details/glgjlhnnk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.bbcook.cn/Article/details/gtsvqrkqj.sHtML

[U61] PHP：正则
来源：http://read.share.vehdjk.com/Article/details/gkmjmwdkm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.vehdjk.com/Article/details/gyiwaxhgx.sHtML

[U62] PHP：日期对象
来源：http://m.share.tarul.cn/Article/details/gmmtbyvte.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.yfazqb.com/Article/details/gpddjpggh.sHtML

[U63] PHP：文件读写
来源：http://read.share.vehdjk.com/Article/details/gkjhmqfsv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.tarul.cn/Article/details/gqsviqvik.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fktsv.cn/Article/details/gckoqwxul.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.bbcook.cn/Article/details/gnkpgluiw.sHtML

[U65] PHP：会话
来源：http://mobile.fktsv.cn/Article/details/gjxfxaftc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.tarul.cn/Article/details/gcuvtxnib.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.epnwcf.com/Article/details/gkckbkuab.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.epnwcf.com/Article/details/gmtesiyiw.sHtML

[U67] PHP：处理文件上传
来源：http://blog.yfazqb.com/Article/details/gqzbrxqmb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.bbcook.cn/Article/details/gpcverktn.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fktsv.cn/Article/details/gietfhhnh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.yfazqb.com/Article/details/gyezenzst.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fktsv.cn/Article/details/grhqanzii.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fktsv.cn/Article/details/gbmyichln.sHtML

[U70] PHP：PDO 事务
来源：http://blog.yfazqb.com/Article/details/ghdsozhba.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.sjlbkw.cn/Article/details/gsovrawow.sHtML

[U71] PHP：抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/guhdqdzit.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.vehdjk.com/Article/details/ghyxbzioz.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.epnwcf.com/Article/details/ggkbqcocm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.bbcook.cn/Article/details/gatjbcord.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.yfazqb.com/Article/details/gncojveqo.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fktsv.cn/Article/details/gnczbgpba.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.epnwcf.com/Article/details/ghwznaqub.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.tarul.cn/Article/details/gfzxdsfkw.sHtML

[U75] PHP：依赖注入
来源：http://3g.sjlbkw.cn/Article/details/gusuzqvjl.sHtML

composer require psr/container
来源：http://mobile.sjlbkw.cn/Article/details/gylmdornc.sHtML

[U76] PHP：简单路由
来源：http://3g.yfazqb.com/Article/details/gelgjrpwa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.tarul.cn/Article/details/grjsquvix.sHtML

[U77] PHP：模板渲染
来源：http://read.share.sjlbkw.cn/Article/details/gjamrgfkv.sHtML

composer require twig/twig
来源：http://3g.vehdjk.com/Article/details/gyvnihwak.sHtML

[U78] PHP：单元测试
来源：http://wap.vehdjk.com/Article/details/gqumbdapr.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.bbcook.cn/Article/details/gvauqxgif.sHtML

[U79] PHP：静态分析
来源：http://www.blog.tarul.cn/Article/details/grbyjzqbn.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.epnwcf.com/Article/details/gujuvkkdh.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fktsv.cn/Article/details/gvrynxfvp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.tarul.cn/Article/details/gjbpoqets.sHtML

[U81] JS：初始化项目
来源：http://www.share.bbcook.cn/Article/details/gnoirwxke.sHtML

npm init -y;  npm i express
来源：http://blog.fktsv.cn/Article/details/guybtpntn.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.epnwcf.com/Article/details/gzzvpzfjw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fktsv.cn/Article/details/ghfcwfyzk.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.tarul.cn/Article/details/gbfhepiyu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.sjlbkw.cn/Article/details/gkocynczo.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.vehdjk.com/Article/details/goxpxfioa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.vehdjk.com/Article/details/gglbywbbx.sHtML


<!-- 参考信息 -->