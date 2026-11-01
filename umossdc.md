代发 wailian999

[S41] C++：类与构造函数
来源：http://wap.yfazqb.com/Article/details/gmgcgvtws.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.sjlbkw.cn/Article/details/gehndybyc.sHtML

[S42] C++：继承与虚函数
来源：http://baike.bbcook.cn/Article/details/gcyropcap.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.epnwcf.com/Article/details/gjtgpyulp.sHtML

[S43] C++：智能指针
来源：http://blog.yfazqb.com/Article/details/gvdtoggbk.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.bbcook.cn/Article/details/gwvcrzhqx.sHtML

[S44] C++：引用传参
来源：http://www.share.sjlbkw.cn/Article/details/gumivyklf.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.tarul.cn/Article/details/gzfpfrchx.sHtML

[S45] C++：lambda
来源：http://mobile.yfazqb.com/Article/details/gomvfkfby.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.vehdjk.com/Article/details/gfjnyhvhv.sHtML

[S46] C++：函数模板
来源：http://read.share.fktsv.cn/Article/details/gxovqieyu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.epnwcf.com/Article/details/gyruonupv.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.yfazqb.com/Article/details/ggsqjisvz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fktsv.cn/Article/details/gopmasvjd.sHtML

[S48] C++：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gdftsjvzh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fktsv.cn/Article/details/gbmfsblwg.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fktsv.cn/Article/details/goakqkzoo.sHtML

[S49] C++：写文件
来源：http://blog.yfazqb.com/Article/details/grgoxcthh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fktsv.cn/Article/details/gzduypjjv.sHtML

[S50] C++：格式化数字
来源：http://mobile.vehdjk.com/Article/details/gtadwhcup.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gsihrccsq.sHtML

[S51] C++：显式类型转换
来源：http://3g.sjlbkw.cn/Article/details/grceunhic.sHtML

static_cast<double>(a) / b
来源：http://m.share.bbcook.cn/Article/details/gscxblqya.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.epnwcf.com/Article/details/gxcuboaei.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.vehdjk.com/Article/details/gxkwovrfw.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/giftobjsy.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fktsv.cn/Article/details/geinrvbry.sHtML

[S54] C++：异常处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gzddhjmpt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.tarul.cn/Article/details/gwbruumsz.sHtML

[S55] C++：结构化绑定
来源：http://wap.bbcook.cn/Article/details/geqhuhofl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.epnwcf.com/Article/details/gbkvczzsv.sHtML

[S56] C++：optional
来源：http://baike.sjlbkw.cn/Article/details/gjwzszmht.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fktsv.cn/Article/details/gyjhdgkcj.sHtML

[S57] C++：编译期常量
来源：http://m.share.tarul.cn/Article/details/glqpjljqp.sHtML

constexpr int N = 10;
来源：http://m.share.tarul.cn/Article/details/gggyvxwuh.sHtML

[S58] C++：命名空间
来源：http://blog.sjlbkw.cn/Article/details/gfdbrafds.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.vehdjk.com/Article/details/gfqlewoqn.sHtML

[S59] C++：静态断言
来源：http://www.blog.tarul.cn/Article/details/gzpqrooie.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.vehdjk.com/Article/details/gtqasnpqc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.tarul.cn/Article/details/grtfjvigs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gvawncdfe.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gggifkhhc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.sjlbkw.cn/Article/details/gfaklpzwx.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gakjnlqbh.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.vehdjk.com/Article/details/gadgnaech.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gapvkuasg.sHtML

[T02] Kotlin：变量
来源：http://m.share.vehdjk.com/Article/details/gdictcrcb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fktsv.cn/Article/details/gotdackwt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.epnwcf.com/Article/details/gynghskqx.sHtML

"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/ggrdcznjs.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fktsv.cn/Article/details/gdfrhywkv.sHtML

val n: String? = null;  n?.length
来源：http://blog.vehdjk.com/Article/details/ggnhxjbop.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.tarul.cn/Article/details/gxxbakvlp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gjcuamacx.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/gogxjmqyw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gydcszmzk.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.yfazqb.com/Article/details/gcigjdodi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.vehdjk.com/Article/details/gcxdjyaew.sHtML

[T08] Kotlin：数据类
来源：http://wap.bbcook.cn/Article/details/gfaysgsuu.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.bbcook.cn/Article/details/gwcxhowfh.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fktsv.cn/Article/details/giguwlcce.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.sjlbkw.cn/Article/details/gbwpnimsk.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.tarul.cn/Article/details/gyuloxczu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.bbcook.cn/Article/details/gzjwdlrxf.sHtML

[T11] Kotlin：协程
来源：http://baike.sjlbkw.cn/Article/details/glpqtlhbe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.tarul.cn/Article/details/gfvxlzojm.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.vehdjk.com/Article/details/gkbtewetj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gzkhykhme.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.epnwcf.com/Article/details/gnhbvoptm.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.bbcook.cn/Article/details/gndooslhv.sHtML

[T14] Kotlin：循环
来源：http://wap.yfazqb.com/Article/details/gsiygyhau.sHtML

for (i in 1..10) println(i)
来源：http://baike.vehdjk.com/Article/details/gnnwwpnre.sHtML

[T15] Kotlin：接口
来源：http://www.share.sjlbkw.cn/Article/details/grupwsflu.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gokaifflk.sHtML

[T16] Swift：Hello World
来源：http://m.share.bbcook.cn/Article/details/gkltfydml.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gncgvsezf.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fktsv.cn/Article/details/gqstrrgpl.sHtML

var a = 1;  let b = 2
来源：http://read.share.vehdjk.com/Article/details/gupqkvzpb.sHtML

[T18] Swift：字符串插值
来源：http://baike.yfazqb.com/Article/details/gufzzvner.sHtML

"值: \(b)"
来源：http://3g.epnwcf.com/Article/details/gpfeluzca.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.yfazqb.com/Article/details/gyvmqkudp.sHtML

if let n = opt { print(n) }
来源：http://wap.vehdjk.com/Article/details/gzcxzldbl.sHtML

[T20] Swift：数组操作
来源：http://mobile.bbcook.cn/Article/details/gchhvfirn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.sjlbkw.cn/Article/details/gkrtwyaub.sHtML

[T21] Swift：遍历
来源：http://www.share.sjlbkw.cn/Article/details/gaeyylolj.sHtML

for x in a { print(x) }
来源：http://read.share.tarul.cn/Article/details/gwysvnkxx.sHtML

[T22] Swift：字典
来源：http://3g.vehdjk.com/Article/details/gkstillvr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.vehdjk.com/Article/details/gjgkmuuar.sHtML

[T23] Swift：函数
来源：http://3g.fktsv.cn/Article/details/gfftvffnd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.bbcook.cn/Article/details/grxmptrkr.sHtML

[T24] Swift：闭包
来源：http://wap.epnwcf.com/Article/details/gxczegbsf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.epnwcf.com/Article/details/gdfacidxz.sHtML

[T25] Swift：结构体
来源：http://www.blog.fktsv.cn/Article/details/gunctgeov.sHtML

struct P { var x: Int }
来源：http://blog.tarul.cn/Article/details/giaxbkaco.sHtML

[T26] Swift：类与重写
来源：http://read.share.fktsv.cn/Article/details/gnbpgltrf.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fktsv.cn/Article/details/gvvclhikx.sHtML

[T27] Swift：错误处理
来源：http://read.share.bbcook.cn/Article/details/gpucmmcsv.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.sjlbkw.cn/Article/details/gjhhztivm.sHtML

[T28] Swift：枚举
来源：http://www.share.fktsv.cn/Article/details/glrmjacvq.sHtML

enum Color { case red, green }
来源：http://wap.bbcook.cn/Article/details/glxyvldxp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.sjlbkw.cn/Article/details/gwtujmbhi.sHtML

guard let x = opt else { return }
来源：http://m.share.fktsv.cn/Article/details/gcnmdkuns.sHtML

[T30] Swift：协议
来源：http://mobile.yfazqb.com/Article/details/glwtqpnxh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.bbcook.cn/Article/details/gtdfkfpfd.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/goledovot.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gjyywqghc.sHtML

[T32] Lua：局部变量
来源：http://mobile.yfazqb.com/Article/details/gnduocvwj.sHtML

local a = 1
来源：http://read.share.bbcook.cn/Article/details/gypfioqgs.sHtML

[T33] Lua：表（数组）
来源：http://3g.tarul.cn/Article/details/gcqklljne.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fktsv.cn/Article/details/gttldxrjc.sHtML

[T34] Lua：遍历表
来源：http://www.blog.vehdjk.com/Article/details/gikllestk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.sjlbkw.cn/Article/details/gebvwqhay.sHtML

[T35] Lua：字典表
来源：http://baike.epnwcf.com/Article/details/ggrwimtfg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.epnwcf.com/Article/details/gcpenlnvi.sHtML

[T36] Lua：函数
来源：http://mobile.vehdjk.com/Article/details/gocfwwhyl.sHtML

function add(a, b) return a + b end
来源：http://3g.tarul.cn/Article/details/gakszzfdb.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.epnwcf.com/Article/details/gfgysqhzw.sHtML

"a" .. "b"
来源：http://blog.epnwcf.com/Article/details/gflmgaoys.sHtML

[T38] Lua：条件
来源：http://blog.sjlbkw.cn/Article/details/gilntzvnc.sHtML

if x > 0 then print("正") end
来源：http://baike.tarul.cn/Article/details/gmrblokjh.sHtML

[T39] Lua：模式匹配
来源：http://www.share.vehdjk.com/Article/details/gkskmsdnb.sHtML

string.find(s, "%d+")
来源：http://blog.fktsv.cn/Article/details/gzrjbtbsg.sHtML

[T40] Lua：元表
来源：http://m.share.vehdjk.com/Article/details/gyxmuwmrx.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.bbcook.cn/Article/details/gltqtwklt.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gttnorxta.sHtML

print "Hello\n";
来源：http://read.share.epnwcf.com/Article/details/gcxlsxaty.sHtML

[T42] Perl：变量类型
来源：http://blog.epnwcf.com/Article/details/gcwhbrrsx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.tarul.cn/Article/details/gjqnphwlb.sHtML

[T43] Perl：字符串插值
来源：http://mobile.vehdjk.com/Article/details/ggwssxebd.sHtML

"值: $a"
来源：http://m.share.sjlbkw.cn/Article/details/gmqufidjz.sHtML

[T44] Perl：条件
来源：http://m.share.epnwcf.com/Article/details/gfxqlmyhi.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.bbcook.cn/Article/details/gdwfgkgmv.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.vehdjk.com/Article/details/gjzmmirwc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.vehdjk.com/Article/details/gxfymhprw.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fktsv.cn/Article/details/gesrwxvqs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.vehdjk.com/Article/details/grrnlszep.sHtML

[T47] Perl：正则捕获
来源：http://wap.epnwcf.com/Article/details/gxjwhkuao.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.tarul.cn/Article/details/gootkeaxi.sHtML

[T48] Perl：正则替换
来源：http://read.share.yfazqb.com/Article/details/gbcgejnrf.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhjmvfsv.sHtML

[T49] Perl：函数
来源：http://www.blog.epnwcf.com/Article/details/gcexsskye.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gmjwpccts.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/guenexqdi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.epnwcf.com/Article/details/gxpumxnfs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.yfazqb.com/Article/details/gcwscsmml.sHtML

[T51] Scala：Hello World
来源：http://wap.tarul.cn/Article/details/gqeaskwrj.sHtML

println("Hello")
来源：http://blog.bbcook.cn/Article/details/geuucsacu.sHtML

[T52] Scala：变量
来源：http://mobile.vehdjk.com/Article/details/gnjwmctik.sHtML

val a = 1;  var b = 2
来源：http://blog.epnwcf.com/Article/details/gmkdfnhzs.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gblibeqle.sHtML

s"值: $b"
来源：http://wap.vehdjk.com/Article/details/gbbnbkeap.sHtML

[T54] Scala：集合映射
来源：http://blog.vehdjk.com/Article/details/gxyatknia.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.yfazqb.com/Article/details/gulnluokb.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gnrvkmhhp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fktsv.cn/Article/details/gikcjlyjp.sHtML

[T56] Scala：样例类
来源：http://www.blog.fktsv.cn/Article/details/grvhfemtb.sHtML

case class User(name: String, age: Int)
来源：http://baike.yfazqb.com/Article/details/gycuudojl.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyxiufyg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fktsv.cn/Article/details/gpnshmjzo.sHtML

[T58] Scala：函数定义
来源：http://www.blog.tarul.cn/Article/details/ghfetvgkq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.epnwcf.com/Article/details/gykiigzwd.sHtML

[T59] Scala：循环
来源：http://3g.yfazqb.com/Article/details/gcfmlvpbb.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gmcxfjmmo.sHtML

[T60] Scala：折叠
来源：http://m.share.tarul.cn/Article/details/gfdbmlbik.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.sjlbkw.cn/Article/details/gsqytusvi.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxzzxjylx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gbtksawjn.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjlnfjpf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.tarul.cn/Article/details/gwwbrstjr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fktsv.cn/Article/details/gfbuozkpx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.epnwcf.com/Article/details/grpeubaxl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.tarul.cn/Article/details/gzkwrwatg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.vehdjk.com/Article/details/gtfzexbpg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fktsv.cn/Article/details/goozrjxvq.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.sjlbkw.cn/Article/details/gudscqhes.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.yfazqb.com/Article/details/gdxbszlfc.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.bbcook.cn/Article/details/glfrylrkm.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/gnwqcfmit.sHtML

[U06] Py：合并两个字典
来源：http://m.share.bbcook.cn/Article/details/goxudpxru.sHtML

{**a, **b}
来源：http://www.share.sjlbkw.cn/Article/details/gwnryrrsv.sHtML

[U07] Py：反转字典键值
来源：http://www.share.yfazqb.com/Article/details/gjianzsot.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.bbcook.cn/Article/details/gezmmqhfj.sHtML

[U08] Py：展平二维列表
来源：http://m.share.vehdjk.com/Article/details/gvxjdqtut.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.yfazqb.com/Article/details/giwrlozab.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.bbcook.cn/Article/details/gpdsyielg.sHtML

max(d, key=d.get)
来源：http://www.blog.fktsv.cn/Article/details/gpeoxuzzx.sHtML

[U10] Py：按值排序字典
来源：http://baike.bbcook.cn/Article/details/ghkmhlkme.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.vehdjk.com/Article/details/gieeqvttd.sHtML

[U11] Py：生成器表达式
来源：http://wap.tarul.cn/Article/details/glvcdblto.sHtML

(x * 2 for x in arr)
来源：http://blog.yfazqb.com/Article/details/gsmolyutg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.sjlbkw.cn/Article/details/gojonbcsq.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.bbcook.cn/Article/details/gzogdhwek.sHtML

[U13] Py：固定长度队列
来源：http://baike.sjlbkw.cn/Article/details/gtncycaaq.sHtML

deque(maxlen=10)
来源：http://mobile.tarul.cn/Article/details/gcanvtgkz.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.yfazqb.com/Article/details/gzufdthks.sHtML

defaultdict(list)
来源：http://www.m.share.yfazqb.com/Article/details/gvaiwasli.sHtML

[U15] Py：高精度计时
来源：http://www.blog.yfazqb.com/Article/details/gyosmlrni.sHtML

t = time.perf_counter()
来源：http://blog.vehdjk.com/Article/details/gwxzseobj.sHtML

[U16] Py：命令行参数解析
来源：http://baike.sjlbkw.cn/Article/details/glorpscsp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fktsv.cn/Article/details/ghmzesroz.sHtML

[U17] Py：初始化日志
来源：http://mobile.vehdjk.com/Article/details/gjyffprmc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fktsv.cn/Article/details/gbehvrdvg.sHtML

[U18] Py：预编译正则
来源：http://m.share.epnwcf.com/Article/details/goqoobxbq.sHtML

pat = re.compile(r"\d+")
来源：http://baike.tarul.cn/Article/details/gdpwniqge.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.vehdjk.com/Article/details/gsyznvcmp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fktsv.cn/Article/details/gmnlmiqan.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.yfazqb.com/Article/details/grulxynvs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.epnwcf.com/Article/details/gyhpdrnpx.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.sjlbkw.cn/Article/details/gitvdndim.sHtML

@contextlib.contextmanager
来源：http://blog.vehdjk.com/Article/details/gjzzctdkq.sHtML

[U22] Py：矩阵转置
来源：http://3g.bbcook.cn/Article/details/gtuzkrzzn.sHtML

list(zip(*m))
来源：http://m.share.yfazqb.com/Article/details/gbubbfecq.sHtML

[U23] Py：分块读取大文件
来源：http://blog.vehdjk.com/Article/details/gywibwacj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.sjlbkw.cn/Article/details/gdxqqisbr.sHtML

[U24] Py：路径操作
来源：http://www.m.share.tarul.cn/Article/details/gwpnjrpsf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.tarul.cn/Article/details/gmjaebjiu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.vehdjk.com/Article/details/giczfhlcz.sHtML

csv.DictReader(f)
来源：http://mobile.epnwcf.com/Article/details/guvoxkyer.sHtML

[U26] Py：并发下载
来源：http://baike.sjlbkw.cn/Article/details/gohxcgxky.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.epnwcf.com/Article/details/ggvfwcwmd.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.yfazqb.com/Article/details/gqtxptncx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.vehdjk.com/Article/details/gckvmnwfu.sHtML

[U28] Py：类型别名
来源：http://m.share.tarul.cn/Article/details/ghmcjcmmw.sHtML

UserId = int
来源：http://www.m.share.epnwcf.com/Article/details/ghjmoyzki.sHtML

[U29] Py：属性校验
来源：http://baike.epnwcf.com/Article/details/gqjqwsuac.sHtML

@property 与 @x.setter 配合
来源：http://baike.yfazqb.com/Article/details/gpyrkudgp.sHtML

[U30] Py：数据类
来源：http://3g.tarul.cn/Article/details/ghienijcc.sHtML

@dataclass(slots=True)
来源：http://read.share.fktsv.cn/Article/details/gstbxmmjv.sHtML

[U31] Py：单测
来源：http://3g.yfazqb.com/Article/details/gcqjvjuow.sHtML

python -m pytest -q
来源：http://m.share.tarul.cn/Article/details/gjuxugjva.sHtML

[U32] Py：代码格式化
来源：http://3g.epnwcf.com/Article/details/gqhxrqudv.sHtML

ruff format . && ruff check --fix .
来源：http://3g.sjlbkw.cn/Article/details/guqlqekib.sHtML

[U33] Py：打包发布
来源：http://mobile.tarul.cn/Article/details/grhglhwog.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.yfazqb.com/Article/details/guapgybgj.sHtML

[U34] Py：判断编码
来源：http://www.m.share.epnwcf.com/Article/details/gcavljnac.sHtML

chardet.detect(raw)
来源：http://3g.epnwcf.com/Article/details/gizwshaqk.sHtML

[U35] Py：发送邮件
来源：http://www.blog.epnwcf.com/Article/details/gepqpoqou.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.tarul.cn/Article/details/gryyasfwl.sHtML

[U36] Py：定时任务
来源：http://www.blog.vehdjk.com/Article/details/gwfvngjil.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.tarul.cn/Article/details/gqzcbxpib.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.yfazqb.com/Article/details/gfsfpdvuw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fktsv.cn/Article/details/gcrykrczb.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.yfazqb.com/Article/details/ghzxfrvgl.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fktsv.cn/Article/details/gwtgqpnhi.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.bbcook.cn/Article/details/gxrtodsgs.sHtML

sys.stdout.isatty()
来源：http://read.share.fktsv.cn/Article/details/gwbvgzecz.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.tarul.cn/Article/details/gnlzcngjk.sHtML

print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gwtidpuro.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.bbcook.cn/Article/details/gztkirioj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fktsv.cn/Article/details/gwlkdxoul.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.yfazqb.com/Article/details/gxmettwmp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.bbcook.cn/Article/details/gpwwxlxth.sHtML

[U43] PHP：声明命名空间
来源：http://blog.bbcook.cn/Article/details/gyuscbaht.sHtML

namespace App\Http;
来源：http://www.share.vehdjk.com/Article/details/gwbzrztww.sHtML

[U44] PHP：开启严格类型
来源：http://blog.tarul.cn/Article/details/gqknvrsoc.sHtML

declare(strict_types=1);
来源：http://mobile.vehdjk.com/Article/details/gupvgyecn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.tarul.cn/Article/details/gcytmccnz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gqsqcabkh.sHtML

[U46] PHP：可空类型
来源：http://baike.tarul.cn/Article/details/gydftkqti.sHtML

?string $name = null
来源：http://read.share.sjlbkw.cn/Article/details/gkztxuvxj.sHtML

[U47] PHP：联合类型
来源：http://blog.fktsv.cn/Article/details/grkhfncuf.sHtML

int|string $id
来源：http://www.blog.sjlbkw.cn/Article/details/glqtikprd.sHtML

[U48] PHP：纯枚举
来源：http://wap.vehdjk.com/Article/details/gsdetluad.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.yfazqb.com/Article/details/gbczgqzkm.sHtML

[U49] PHP：只读属性
来源：http://baike.sjlbkw.cn/Article/details/gbancrxbs.sHtML

public readonly string $name
来源：http://read.share.tarul.cn/Article/details/guclifkuv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.yfazqb.com/Article/details/gxytkhdga.sHtML

public function __construct(private int $id) {}
来源：http://baike.bbcook.cn/Article/details/gdxbeespu.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.yfazqb.com/Article/details/gzqqozrwc.sHtML

[$a, $b] = $arr;
来源：http://m.share.vehdjk.com/Article/details/gonjvyeog.sHtML

[U52] PHP：箭头函数
来源：http://blog.fktsv.cn/Article/details/gsrvixjci.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.sjlbkw.cn/Article/details/gflsnibgc.sHtML

[U53] PHP：空合并运算符
来源：http://baike.sjlbkw.cn/Article/details/gbuqwgdir.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.bbcook.cn/Article/details/gvsopxqdu.sHtML

[U54] PHP：空安全调用
来源：http://read.share.vehdjk.com/Article/details/gnnlwxofc.sHtML

$obj?->method()
来源：http://3g.bbcook.cn/Article/details/gwrikqyzd.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gbzysnmzi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fktsv.cn/Article/details/gocjwsvfk.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gorsolvrl.sHtML

f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gcbzrqnsh.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gecwqtyqv.sHtML

"值: {$a}"
来源：http://3g.tarul.cn/Article/details/gmelfdecz.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.sjlbkw.cn/Article/details/gbvyiyjxq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.bbcook.cn/Article/details/ghoflvmhb.sHtML

[U59] PHP：自定义排序
来源：http://read.share.epnwcf.com/Article/details/gzghgwaaz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.epnwcf.com/Article/details/gfnowrmlm.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fktsv.cn/Article/details/ggcjqisyp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.bbcook.cn/Article/details/gboltaxxg.sHtML

[U61] PHP：正则
来源：http://m.share.sjlbkw.cn/Article/details/gohhlnpjv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwndippe.sHtML

[U62] PHP：日期对象
来源：http://blog.tarul.cn/Article/details/gsjcbupls.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.vehdjk.com/Article/details/gknjgwndk.sHtML

[U63] PHP：文件读写
来源：http://3g.epnwcf.com/Article/details/gplmytlnm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.vehdjk.com/Article/details/gfjnjeqqo.sHtML

[U64] PHP：目录遍历
来源：http://wap.tarul.cn/Article/details/gjwhqhrmn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.epnwcf.com/Article/details/gehtnfcze.sHtML

[U65] PHP：会话
来源：http://m.share.fktsv.cn/Article/details/gyldtwmhe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fktsv.cn/Article/details/gtimzqnjq.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.bbcook.cn/Article/details/gnlmmmjmi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fktsv.cn/Article/details/gxjwvdxzp.sHtML


<!-- 参考信息 -->