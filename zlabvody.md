代发 wailian999

static int counter = 0;
来源：http://vkj.shanyushiyangtech.top

[S29] C：变参函数
来源：http://iyk.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qxm.xinyue.icu

[S30] C：头文件保护
来源：http://jeq.birdmap.top

#ifndef X_H
来源：http://nfo.zhixingplan.top

#define X_H
来源：http://zyw.chenlongwang.top

#endif
来源：http://ifx.gzhubu.top

[S31] C++：Hello World
来源：http://qiu.sweek.top

#include <iostream>
来源：http://cev.aizwys.cn

int main() { std::cout << "Hello\n"; }
来源：http://fly.bbcook.cn

[S32] C++：字符串
来源：http://qep.xylfe.cn

std::string s = "hi";  s += "!";
来源：http://xcw.gotoacloud.top

[S33] C++：vector 增删
来源：http://umk.0kj1m.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gmq.chenjidiqi.icu

[S34] C++：遍历 vector
来源：http://jft.yj202588.top

for (auto &x : v) { std::cout << x; }
来源：http://eyl.yuanzhike.top

[S35] C++：map
来源：http://lxl.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mcl.52xcode.cn

[S36] C++：unordered_map
来源：http://bvm.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://azi.daxiang520.top

[S37] C++：set
来源：http://otb.ydjk.org.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://goa.yj20258888.top

[S38] C++：排序
来源：http://ovp.yj20258888.top

std::sort(v.begin(), v.end());
来源：http://dda.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://zqk.tanke756.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yxz.sweek.top

[S40] C++：查找元素
来源：http://yhd.mhx1999.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tzm.feifeiyinyue.top

[S41] C++：类与构造函数
来源：http://uin.xuanzx.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ypw.zhiwuduotai.top

[S42] C++：继承与虚函数
来源：http://ugo.snrcjt.cn

class B : public Base { public: void f() override {} };
来源：http://goj.hysaishi.cn

[S43] C++：智能指针
来源：http://sav.daria6918.cn

auto p = std::make_unique<int>(5);
来源：http://kqi.yangfankeji.com

[S44] C++：引用传参
来源：http://gta.c1oappe.top

void inc(int &x) { ++x; }
来源：http://cjm.xinyue.icu

[S45] C++：lambda
来源：http://uxw.xingfuxueyuan.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://xff.52xcode.cn

[S46] C++：函数模板
来源：http://eub.iojbl.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uja.yangfankeji.com

[S47] C++：结构化绑定遍历
来源：http://kmh.jinqigufen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vnk.iojbl.cn

[S48] C++：逐行读文件
来源：http://uza.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://bmr.andypj.xyz

while (std::getline(in, line)) { }
来源：http://rtj.ydzc1.top

[S49] C++：写文件
来源：http://vrc.tianlin.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tfq.gaohongyu789.top

[S50] C++：格式化数字
来源：http://kod.jianghu66.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lxi.hammf.cn

[S51] C++：显式类型转换
来源：http://pfx.gogol.net.cn

static_cast<double>(a) / b
来源：http://fjw.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://tti.ppjwa.cn

int size() const noexcept { return n_; }
来源：http://hnm.xinyue.icu

[S53] C++：移动语义
来源：http://ltx.xingfuxueyuan.xyz

std::vector<int> w = std::move(v);
来源：http://cqf.xziqi.cn

[S54] C++：异常处理
来源：http://quu.daxiang520.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gsc.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://qoj.tianlin.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://bah.pengpengdd.cyou

[S56] C++：optional
来源：http://nxo.zhaomingkeji.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://obn.tianlin.xyz

[S57] C++：编译期常量
来源：http://wao.wangdashe.top

constexpr int N = 10;
来源：http://nty.0kj1m.cn

[S58] C++：命名空间
来源：http://ycd.nanxinkj.top

namespace ns { int f() { return 1; } }
来源：http://qgm.meibo888.top

[S59] C++：静态断言
来源：http://tzz.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lkm.sufxvd.cn

[S60] C++：遍历并删除元素
来源：http://oab.epnwcf.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rbx.sysykeji.top

================================================================================
来源：http://tbu.feifeiyinyue.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xyp.shzxlz.cn

================================================================================
来源：http://lho.hywenlv.cn

[T01] Kotlin：Hello World
来源：http://bzf.hesvh.cn

println("Hello")
来源：http://rke.vqdsnc.cn

[T02] Kotlin：变量
来源：http://ici.52xcode.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tgg.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://pnj.zhaomingkeji.xyz

"值: $b"
来源：http://pha.cdnleiting.top

[T04] Kotlin：空安全
来源：http://zov.ehwqpu.com

val n: String? = null;  n?.length
来源：http://vvp.zycfv.cn

[T05] Kotlin：when 表达式
来源：http://jas.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cnx.mhx1999.top

[T06] Kotlin：集合映射
来源：http://szm.hfpthk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fwy.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://qyh.cucudq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hvj.tian-w.cn

[T08] Kotlin：数据类
来源：http://zzl.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://lge.feifeiyinyue.top

[T09] Kotlin：扩展函数
来源：http://qtd.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://sny.ywan-chungtsiang.top

[T10] Kotlin：默认参数
来源：http://lee.haohaochexian.top

fun greet(name: String = "World") = "Hi $name"
来源：http://flo.bjfxy.top

[T11] Kotlin：协程
来源：http://etb.hammf.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://den.ivvv.top

[T12] Kotlin：解构声明
来源：http://wty.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://zqt.ehwqpu.com

[T13] Kotlin：只读 Map
来源：http://vxo.tarul.cn

val m = mapOf("a" to 1)
来源：http://ost.yuxming.cn

[T14] Kotlin：循环
来源：http://pea.shanyushiyangkeji.top

for (i in 1..10) println(i)
来源：http://tdf.yj20258.top

[T15] Kotlin：接口
来源：http://csv.pycfn.com

interface Shape { fun area(): Double }
来源：http://vis.yangfankeji.com

[T16] Swift：Hello World
来源：http://rpc.jinqigfzy.top

print("Hello")
来源：http://svm.yj20258888.top

[T17] Swift：变量与常量
来源：http://jhx.cheryme.top

var a = 1;  let b = 2
来源：http://gsr.xylfe.cn

[T18] Swift：字符串插值
来源：http://pqn.hnxiangtu.top

"值: \(b)"
来源：http://fdq.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://gzv.vqdsnc.cn

if let n = opt { print(n) }
来源：http://gsn.vqdsnc.cn

[T20] Swift：数组操作
来源：http://hfx.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://mcx.c1oappe.top

[T21] Swift：遍历
来源：http://col.gotoacloud.top

for x in a { print(x) }
来源：http://iwo.gogol.net.cn

[T22] Swift：字典
来源：http://vkf.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://flz.dashuyun.cn

[T23] Swift：函数
来源：http://vem.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xmq.nwbrower.top

[T24] Swift：闭包
来源：http://irw.nwbrower.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pjc.zhijiandao.cn

[T25] Swift：结构体
来源：http://lcn.shangyingyoupin.top

struct P { var x: Int }
来源：http://dip.nwbrower.top

[T26] Swift：类与重写
来源：http://dop.vehdjk.com

class A: Base { override func f() {} }
来源：http://wdz.jinghuilouyu.cn

[T27] Swift：错误处理
来源：http://ypl.zycfv.cn

do { try f() } catch { print(error) }
来源：http://nfv.shzxlz.cn

[T28] Swift：枚举
来源：http://giw.chenlongwang.top

enum Color { case red, green }
来源：http://esp.vehdjk.com

[T29] Swift：guard 提前返回
来源：http://icq.yfazqb.com

guard let x = opt else { return }
来源：http://lfx.xinyue.icu

[T30] Swift：协议
来源：http://ksp.jqgufenzy.top

protocol Shape { func area() -> Double }
来源：http://vow.xuetiantiany.cn

[T31] Lua：Hello World
来源：http://iaf.svipenyu.cn

print("Hello")
来源：http://yhx.havefunace.top

[T32] Lua：局部变量
来源：http://pwr.ywan-chungtsiang.top

local a = 1
来源：http://bkn.hysaishi.cn

[T33] Lua：表（数组）
来源：http://qbj.pycfn.com

local t = {1, 2, 3};  t[4] = 4
来源：http://oqy.chenzaomai.com

[T34] Lua：遍历表
来源：http://coo.xingfuxueyuan.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://bhc.guowangkeji.top

[T35] Lua：字典表
来源：http://pso.shanyushiyangtech.top

local d = { a = 1 };  d.b = 2
来源：http://ulv.dianchejie.cn

[T36] Lua：函数
来源：http://krj.jqgfzy.top

function add(a, b) return a + b end
来源：http://ztn.xylfe.cn

[T37] Lua：字符串拼接
来源：http://gpq.jqgfzy.top

"a" .. "b"
来源：http://zkt.ctjpmb.com

[T38] Lua：条件
来源：http://hvf.wangshuangyany.cn

if x > 0 then print("正") end
来源：http://gsy.fehbvm.com

[T39] Lua：模式匹配
来源：http://ypk.chenlongwang.top

string.find(s, "%d+")
来源：http://cyr.haohaochexian.top

[T40] Lua：元表
来源：http://vxh.zhoulong.xyz

setmetatable({}, { __index = base })
来源：http://csn.vehdjk.com

[T41] Perl：Hello World
来源：http://eax.tarul.cn

print "Hello\n";
来源：http://nnc.zhengqikj.top

[T42] Perl：变量类型
来源：http://zik.fengsongda.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ggm.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://xot.wangdashe.top

"值: $a"
来源：http://kdm.shuidangran.top

[T44] Perl：条件
来源：http://fpb.vehdjk.com

if ($a > 0) { print "正"; }
来源：http://qne.epnwcf.com

[T45] Perl：数组遍历
来源：http://jli.kuanghao11.cn

for my $x (@arr) { print $x; }
来源：http://fbr.cashguo.top

[T46] Perl：哈希操作
来源：http://rol.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zvy.jinyuanbaomall.cn

[T47] Perl：正则捕获
来源：http://kmx.hesvh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://grs.daria6918.cn

[T48] Perl：正则替换
来源：http://rml.nwbrower.top

$s =~ s/old/new/g;
来源：http://hus.zhaomingkeji.xyz

[T49] Perl：函数
来源：http://hog.yj20258.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wjh.shangyingyoupin.top

[T50] Perl：逐行读文件
来源：http://vwy.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jlb.yanxiufei.cn

while (my $line = <$fh>) { print $line; }
来源：http://zlt.haohaochexian.top

[T51] Scala：Hello World
来源：http://fav.iojbl.cn

println("Hello")
来源：http://ukx.tianlin.xyz

[T52] Scala：变量
来源：http://bhq.jinghuilouyu.cn

val a = 1;  var b = 2
来源：http://fgm.yj20258888.top

[T53] Scala：字符串插值
来源：http://yda.dashuyun.cn

s"值: $b"
来源：http://dgx.vehdjk.com

[T54] Scala：集合映射
来源：http://zlp.gogol.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://phs.gzhubu.top

[T55] Scala：集合过滤
来源：http://npm.ydzc1.top

List(1, 2, 3).filter(_ > 1)
来源：http://ruv.zdbjq.cn

[T56] Scala：样例类
来源：http://hsk.jlsjyb.cn

case class User(name: String, age: Int)
来源：http://lbg.pycfn.com

[T57] Scala：模式匹配
来源：http://xgt.cheryme.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nuy.yfazqb.com

[T58] Scala：函数定义
来源：http://kmi.svipenyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yie.ywan-chungtsiang.top

[T59] Scala：循环
来源：http://ozz.jinqigfzy.top

for (i <- 1 to 10) println(i)
来源：http://uqb.xinyue.icu

[T60] Scala：折叠
来源：http://anl.sjlbkw.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xrw.hnxiangtu.top

================================================================================
来源：http://vbr.xziqi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://boz.zhaomingkeji.xyz

================================================================================
来源：http://mew.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://msy.jinghuilouyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://aym.jianghu66.top

[U02] Py：导出 / 安装依赖
来源：http://nnq.shanyushiyangtech.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://roh.xinyue.icu

[U03] Py：加载 .env 配置
来源：http://kbo.fengsongda.top

from dotenv import load_dotenv; load_dotenv()
来源：http://uzc.aizwys.cn

[U04] Py：变量调试打印
来源：http://iin.mhx1999.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qre.zhoulong.xyz

[U05] Py：列表去重且保序
来源：http://rym.quarkkingdee.top

list(dict.fromkeys(arr))
来源：http://nir.yongpay.top

[U06] Py：合并两个字典
来源：http://fuo.sxryk.cn

{**a, **b}
来源：http://rei.snrcjt.cn

[U07] Py：反转字典键值
来源：http://fru.shuidangran.top

{v: k for k, v in d.items()}
来源：http://yeh.havefunace.top

[U08] Py：展平二维列表
来源：http://eyj.shanyushiyangtech.top

[y for x in nested for y in x]
来源：http://urh.0kj1m.cn

[U09] Py：字典取最大值的键
来源：http://lis.yongpay.top

max(d, key=d.get)
来源：http://wxw.ppjwa.cn

[U10] Py：按值排序字典
来源：http://xlb.fktsv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://osn.zhaomingkeji.xyz

[U11] Py：生成器表达式
来源：http://dlt.zdqjudy.top

(x * 2 for x in arr)
来源：http://qtq.hywenlv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://heg.cashguo.top

Counter(arr).most_common(3)
来源：http://sib.nwbrower.top

[U13] Py：固定长度队列
来源：http://jwa.zdbjq.cn

deque(maxlen=10)
来源：http://yki.tarul.cn

[U14] Py：分组收集到列表
来源：http://sys.vehdjk.com

defaultdict(list)
来源：http://dbe.zdqjudy.top

[U15] Py：高精度计时
来源：http://gmu.sysykeji.top

t = time.perf_counter()
来源：http://nza.pycfn.com

[U16] Py：命令行参数解析
来源：http://sog.hammf.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sth.pycfn.com

[U17] Py：初始化日志
来源：http://wfv.hfpthk.cn

logging.basicConfig(level=logging.INFO)
来源：http://jdc.jinqigufen.top

[U18] Py：预编译正则
来源：http://uzj.yj20258888.top

pat = re.compile(r"\d+")
来源：http://ubh.yueranfly.top

[U19] Py：正则替换带回调
来源：http://gds.yfazqb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nwd.sweek.top

[U20] Py：缓存函数结果
来源：http://uce.xuetiantiany.cn

@functools.lru_cache(maxsize=None)
来源：http://jkf.shuidangran.top

[U21] Py：自定义上下文管理器
来源：http://fhn.yfazqb.com

@contextlib.contextmanager
来源：http://wsv.gogol.net.cn

[U22] Py：矩阵转置
来源：http://pou.guowangkeji.top

list(zip(*m))
来源：http://myc.cheryme.top

[U23] Py：分块读取大文件
来源：http://cpo.cashguo.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xru.yangfankeji.com

[U24] Py：路径操作
来源：http://ary.ydjk.org.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://opc.quarkkingdee.top

[U25] Py：CSV 按字典读
来源：http://eke.chenzaomai.com

csv.DictReader(f)
来源：http://gdf.c1oappe.top

[U26] Py：并发下载
来源：http://vdi.ctjpmb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tmy.yvedp.cn

[U27] Py：异步 HTTP
来源：http://cdw.xuetiantiany.cn

aiohttp.ClientSession() 配合 async with
来源：http://uhb.fehbvm.com

[U28] Py：类型别名
来源：http://ocr.yanxiufei.cn

UserId = int
来源：http://nem.jiagoushi.top

[U29] Py：属性校验
来源：http://you.yangfankeji.com

@property 与 @x.setter 配合
来源：http://kwo.cashguo.top

[U30] Py：数据类
来源：http://hvm.dashuyun.cn

@dataclass(slots=True)
来源：http://ibf.yfazqb.com

[U31] Py：单测
来源：http://pxk.jlsjyb.cn

python -m pytest -q
来源：http://zfy.epnwcf.com

[U32] Py：代码格式化
来源：http://fnq.ydzc1.top

ruff format . && ruff check --fix .
来源：http://aav.zdqjudy.top

[U33] Py：打包发布
来源：http://hrx.sxryk.cn

python -m build  （依赖 pyproject.toml）
来源：http://tpt.xinyue.icu

[U34] Py：判断编码
来源：http://epi.vqdsnc.cn

chardet.detect(raw)
来源：http://xgp.pengpengdd.cyou

[U35] Py：发送邮件
来源：http://mgy.bjfxy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wzv.yj202588.top

[U36] Py：定时任务
来源：http://ulp.ybcxt.top

schedule.every(10).minutes.do(job)
来源：http://nbw.sysykeji.top

[U37] Py：读写 Excel
来源：http://pgl.vehdjk.com

pandas.read_excel / DataFrame.to_excel
来源：http://oex.xuetiantiany.cn

[U38] Py：获取脚本所在目录
来源：http://vnw.hfpthk.cn

Path(__file__).resolve().parent
来源：http://nxm.meibo888.top

[U39] Py：判断是否在交互环境
来源：http://oxc.fzhhl.top

sys.stdout.isatty()
来源：http://mmq.iojbl.cn

[U40] Py：打印到标准错误
来源：http://chq.jinyuanbaomall.cn

print("err", file=sys.stderr)
来源：http://raf.guowangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://xri.hfpthk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jbj.vehdjk.com

[U42] PHP：PSR-4 自动加载
来源：http://hcq.dashuyun.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mqt.fktsv.cn

[U43] PHP：声明命名空间
来源：http://hcf.gzhubu.top

namespace App\Http;
来源：http://kaj.zhixingplan.top

[U44] PHP：开启严格类型
来源：http://lhd.zhongyouzk.top

declare(strict_types=1);
来源：http://vvb.jqgufenzy.top

[U45] PHP：类型声明与返回类型
来源：http://baj.sjlbkw.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pip.xinyue.icu

[U46] PHP：可空类型
来源：http://lct.wangshuangyany.cn

?string $name = null
来源：http://vrw.smart0.xyz

[U47] PHP：联合类型
来源：http://mws.yfazqb.com

int|string $id
来源：http://vex.andypj.xyz

[U48] PHP：纯枚举
来源：http://hkt.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gab.chenlongwang.top

[U49] PHP：只读属性
来源：http://sca.zhoulong.xyz

public readonly string $name
来源：http://mdw.mhx1999.top

[U50] PHP：构造器属性提升
来源：http://vyq.shzxlz.cn

public function __construct(private int $id) {}
来源：http://hgv.yfazqb.com

[U51] PHP：数组解构
来源：http://ixa.daxiang520.top

[$a, $b] = $arr;
来源：http://kyh.yongpay.top

[U52] PHP：箭头函数
来源：http://ygl.tianlin.xyz

$double = fn($x) => $x * 2;
来源：http://aot.pengpengdd.cyou


<!-- 参考信息 -->