代发 wailian999

#ifndef X_H
来源：http://skq.yfazqb.com

#define X_H
来源：http://qib.ydzc1.top

#endif
来源：http://faq.jqgufenzy.top

[S31] C++：Hello World
来源：http://gal.bbcook.cn

#include <iostream>
来源：http://hrx.jinqigufen.top

int main() { std::cout << "Hello\n"; }
来源：http://uxk.yangfankeji.com

[S32] C++：字符串
来源：http://gmw.tian-w.cn

std::string s = "hi";  s += "!";
来源：http://iuj.nwbrower.top

[S33] C++：vector 增删
来源：http://gbe.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ygv.iojbl.cn

[S34] C++：遍历 vector
来源：http://cwx.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://irv.ivvv.top

[S35] C++：map
来源：http://ypg.tanke756.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tce.jinqigufen.top

[S36] C++：unordered_map
来源：http://xcs.yangfankeji.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zzb.jlsjyb.cn

[S37] C++：set
来源：http://qbq.aizwys.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ydl.hongshengwenyu.top

[S38] C++：排序
来源：http://ctc.gaohongyu789.top

std::sort(v.begin(), v.end());
来源：http://jbw.kuanghao11.cn

[S39] C++：自定义比较器排序
来源：http://iaj.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://amh.jinyuanbaomall.cn

[S40] C++：查找元素
来源：http://jrs.wangdashe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://unp.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://env.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uxv.jqgfzy.top

[S42] C++：继承与虚函数
来源：http://qbs.iojbl.cn

class B : public Base { public: void f() override {} };
来源：http://wym.zhijiandao.cn

[S43] C++：智能指针
来源：http://zxg.ctjpmb.com

auto p = std::make_unique<int>(5);
来源：http://ijr.zdbjq.cn

[S44] C++：引用传参
来源：http://ycy.andypj.xyz

void inc(int &x) { ++x; }
来源：http://oec.fengsongda.top

[S45] C++：lambda
来源：http://gux.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vzy.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://nya.hammf.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://myr.bjfxy.top

[S47] C++：结构化绑定遍历
来源：http://gam.redwolf501.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uue.shanyushiyangtech.top

[S48] C++：逐行读文件
来源：http://dji.shangyingyoupin.top

std::ifstream in("a.txt");  std::string line;
来源：http://isi.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://qkk.guowangkeji.top

[S49] C++：写文件
来源：http://fyz.jqgufenzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qmy.uphjek.com

[S50] C++：格式化数字
来源：http://jsc.cdnleiting.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ffq.jinqigufen.top

[S51] C++：显式类型转换
来源：http://hvv.snrcjt.cn

static_cast<double>(a) / b
来源：http://huw.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://ixk.shanyushiyangtech.top

int size() const noexcept { return n_; }
来源：http://wdq.snrcjt.cn

[S53] C++：移动语义
来源：http://jfo.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://eaf.smart0.xyz

[S54] C++：异常处理
来源：http://vmw.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xub.yfazqb.com

[S55] C++：结构化绑定
来源：http://tnj.pengpengdd.cyou

auto [a, b] = std::make_pair(1, 2);
来源：http://jnh.fktsv.cn

[S56] C++：optional
来源：http://eys.shzxlz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fzs.hysaishi.cn

[S57] C++：编译期常量
来源：http://nnp.cqqwz.cn

constexpr int N = 10;
来源：http://jpg.fanxiaobao.xyz

[S58] C++：命名空间
来源：http://mzx.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://yve.ivvv.top

[S59] C++：静态断言
来源：http://rqh.daxiang520.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eys.shzxlz.cn

[S60] C++：遍历并删除元素
来源：http://mru.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://exg.iojbl.cn

================================================================================
来源：http://ocj.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bsh.fzhhl.top

================================================================================
来源：http://hyn.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://wmv.c1oappe.top

println("Hello")
来源：http://fjv.guannengcc.top

[T02] Kotlin：变量
来源：http://vlj.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bam.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://xdl.jqgufenzy.top

"值: $b"
来源：http://plu.xinyue.icu

[T04] Kotlin：空安全
来源：http://hwy.zycfv.cn

val n: String? = null;  n?.length
来源：http://eia.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://pzn.sufxvd.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kma.tarul.cn

[T06] Kotlin：集合映射
来源：http://lwo.havefunace.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zmu.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://ckb.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oud.tarul.cn

[T08] Kotlin：数据类
来源：http://jza.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://img.vqdsnc.cn

[T09] Kotlin：扩展函数
来源：http://rkl.epnwcf.com

fun String.exclaim() = this + "!"
来源：http://ulc.shzxlz.cn

[T10] Kotlin：默认参数
来源：http://zho.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://udh.mhx1999.top

[T11] Kotlin：协程
来源：http://uwj.hnqzz.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://eew.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://skn.gzhubu.top

val (a, b) = Pair(1, 2)
来源：http://ckl.fehbvm.com

[T13] Kotlin：只读 Map
来源：http://bol.kuanghao11.cn

val m = mapOf("a" to 1)
来源：http://gxy.sweek.top

[T14] Kotlin：循环
来源：http://nrm.shuidangran.top

for (i in 1..10) println(i)
来源：http://yov.hywenlv.cn

[T15] Kotlin：接口
来源：http://oqr.ywan-chungtsiang.top

interface Shape { fun area(): Double }
来源：http://gvj.shzxlz.cn

[T16] Swift：Hello World
来源：http://nxz.sxryk.cn

print("Hello")
来源：http://lpm.yj202588.top

[T17] Swift：变量与常量
来源：http://xrx.wangshuangyany.cn

var a = 1;  let b = 2
来源：http://bxr.ybcxt.top

[T18] Swift：字符串插值
来源：http://dxj.nwbrower.top

"值: \(b)"
来源：http://wvx.havefunace.top

[T19] Swift：可选绑定
来源：http://jnv.ivvv.top

if let n = opt { print(n) }
来源：http://cxq.zhongyouzk.top

[T20] Swift：数组操作
来源：http://kcn.zhixingplan.top

var a = [1, 2, 3];  a.append(4)
来源：http://tmk.yj20258.top

[T21] Swift：遍历
来源：http://rum.0kj1m.cn

for x in a { print(x) }
来源：http://vrs.hnqzz.top

[T22] Swift：字典
来源：http://ppo.wangshuangyany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qpw.feifeiyinyue.top

[T23] Swift：函数
来源：http://qvl.jinghuilouyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vaa.yonumen.top

[T24] Swift：闭包
来源：http://wva.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ugq.52xcode.cn

[T25] Swift：结构体
来源：http://xbd.cucudq.cn

struct P { var x: Int }
来源：http://oxv.xinyue.icu

[T26] Swift：类与重写
来源：http://xfd.ehwqpu.com

class A: Base { override func f() {} }
来源：http://llt.mhx1999.top

[T27] Swift：错误处理
来源：http://jah.yj202588.top

do { try f() } catch { print(error) }
来源：http://wqu.ivvv.top

[T28] Swift：枚举
来源：http://ixr.jlsjyb.cn

enum Color { case red, green }
来源：http://ipz.yuanzhike.top

[T29] Swift：guard 提前返回
来源：http://hjq.zhijiandao.cn

guard let x = opt else { return }
来源：http://fbi.cheryme.top

[T30] Swift：协议
来源：http://xsj.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://fma.shanyushiyangkeji.top

[T31] Lua：Hello World
来源：http://cvi.jianghu66.top

print("Hello")
来源：http://iat.xinyue.icu

[T32] Lua：局部变量
来源：http://vnk.hammf.cn

local a = 1
来源：http://zvj.ppjwa.cn

[T33] Lua：表（数组）
来源：http://cdy.jinqigufen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wpj.hnxiangtu.top

[T34] Lua：遍历表
来源：http://jdo.zhaomingkeji.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://wpw.9152youxi.cn

[T35] Lua：字典表
来源：http://nha.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://cti.hfpthk.cn

[T36] Lua：函数
来源：http://jjl.hesvh.cn

function add(a, b) return a + b end
来源：http://ues.fktsv.cn

[T37] Lua：字符串拼接
来源：http://iwd.nanxuanxn.top

"a" .. "b"
来源：http://hwr.havefunace.top

[T38] Lua：条件
来源：http://qgz.kuanghao11.cn

if x > 0 then print("正") end
来源：http://zmu.jyoumei.cn

[T39] Lua：模式匹配
来源：http://bnp.316326.xyz

string.find(s, "%d+")
来源：http://dnt.aibaodan.cn

[T40] Lua：元表
来源：http://pcs.aizwys.cn

setmetatable({}, { __index = base })
来源：http://bst.yueranfly.top

[T41] Perl：Hello World
来源：http://kak.cqqwz.cn

print "Hello\n";
来源：http://hhk.cucudq.cn

[T42] Perl：变量类型
来源：http://ajj.yfazqb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://caw.cheryme.top

[T43] Perl：字符串插值
来源：http://bbr.hfpthk.cn

"值: $a"
来源：http://flv.cashguo.top

[T44] Perl：条件
来源：http://khn.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://xan.zycfv.cn

[T45] Perl：数组遍历
来源：http://zsb.bjfxy.top

for my $x (@arr) { print $x; }
来源：http://zqf.yvedp.cn

[T46] Perl：哈希操作
来源：http://dco.daria6918.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hkq.ppjwa.cn

[T47] Perl：正则捕获
来源：http://fmu.zhaomingkeji.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://zvc.jlsjyb.cn

[T48] Perl：正则替换
来源：http://icq.ydzc1.top

$s =~ s/old/new/g;
来源：http://crn.jqgufenzy.top

[T49] Perl：函数
来源：http://aiz.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dqg.yangfankeji.com

[T50] Perl：逐行读文件
来源：http://jrf.hnqzz.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ajt.iojbl.cn

while (my $line = <$fh>) { print $line; }
来源：http://aib.xuanzx.com

[T51] Scala：Hello World
来源：http://rzf.jiagoushi.top

println("Hello")
来源：http://fpu.xinyue.icu

[T52] Scala：变量
来源：http://qpk.redwolf501.top

val a = 1;  var b = 2
来源：http://hge.yonumen.top

[T53] Scala：字符串插值
来源：http://jvo.zhengqikj.top

s"值: $b"
来源：http://ugm.jlsjyb.cn

[T54] Scala：集合映射
来源：http://wnx.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://wfn.tanke756.top

[T55] Scala：集合过滤
来源：http://qeu.316326.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://npy.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://flj.yfazqb.com

case class User(name: String, age: Int)
来源：http://bpw.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://ckh.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tqk.uphjek.com

[T58] Scala：函数定义
来源：http://xft.havefunace.top

def add(a: Int, b: Int): Int = a + b
来源：http://ysc.52xcode.cn

[T59] Scala：循环
来源：http://lhm.quarkkingdee.top

for (i <- 1 to 10) println(i)
来源：http://pfi.wangshuangyany.cn

[T60] Scala：折叠
来源：http://wjs.sufxvd.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://soc.fktsv.cn

================================================================================
来源：http://cox.iojbl.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dqa.guannengcc.top

================================================================================
来源：http://cgd.yueranfly.top

[U01] Py：创建虚拟环境
来源：http://qhz.andypj.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://wyz.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://fba.hysaishi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rcy.shangyingyoupin.top

[U03] Py：加载 .env 配置
来源：http://nee.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hwx.wangdashe.top

[U04] Py：变量调试打印
来源：http://oxu.jinyuanbaomall.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gtr.yonumen.top

[U05] Py：列表去重且保序
来源：http://sbw.xinyue.icu

list(dict.fromkeys(arr))
来源：http://ltk.jyoumei.cn

[U06] Py：合并两个字典
来源：http://qhl.havefunace.top

{**a, **b}
来源：http://cds.haohaochexian.top

[U07] Py：反转字典键值
来源：http://qnz.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://qda.pengpengdd.cyou

[U08] Py：展平二维列表
来源：http://gdd.yanxiufei.cn

[y for x in nested for y in x]
来源：http://vsp.shanyushiyangkeji.top

[U09] Py：字典取最大值的键
来源：http://jxg.birdmap.top

max(d, key=d.get)
来源：http://tnd.hcnkem.com

[U10] Py：按值排序字典
来源：http://nbo.xuetiantiany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://moo.ivvv.top

[U11] Py：生成器表达式
来源：http://uyz.ehwqpu.com

(x * 2 for x in arr)
来源：http://ukq.52xcode.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ryx.cheryme.top

Counter(arr).most_common(3)
来源：http://mxd.ydjk.org.cn

[U13] Py：固定长度队列
来源：http://hyf.hnqzz.top

deque(maxlen=10)
来源：http://qdq.fktsv.cn

[U14] Py：分组收集到列表
来源：http://ncf.dashuyun.cn

defaultdict(list)
来源：http://yig.fanxiaobao.xyz

[U15] Py：高精度计时
来源：http://asi.chenzaomai.com

t = time.perf_counter()
来源：http://efl.kuanghao11.cn

[U16] Py：命令行参数解析
来源：http://lwd.jinyuanbaomall.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://smh.yangfankeji.com

[U17] Py：初始化日志
来源：http://xgg.dashuyun.cn

logging.basicConfig(level=logging.INFO)
来源：http://jea.nanxuanxn.top

[U18] Py：预编译正则
来源：http://uag.zhoulong.xyz

pat = re.compile(r"\d+")
来源：http://bcm.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://sfy.sxryk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bkm.cqqwz.cn

[U20] Py：缓存函数结果
来源：http://xuj.feifeiyinyue.top

@functools.lru_cache(maxsize=None)
来源：http://kut.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://gij.ywan-chungtsiang.top

@contextlib.contextmanager
来源：http://seb.tanke756.top

[U22] Py：矩阵转置
来源：http://rtu.hnxiangtu.top

list(zip(*m))
来源：http://rhk.zdqjudy.top

[U23] Py：分块读取大文件
来源：http://hki.ppjwa.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jay.yj20258.top

[U24] Py：路径操作
来源：http://ihd.nwbrower.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bud.cashguo.top

[U25] Py：CSV 按字典读
来源：http://yaz.yonumen.top

csv.DictReader(f)
来源：http://fpd.guannengcc.top

[U26] Py：并发下载
来源：http://piz.pycfn.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wll.jinyuanbaomall.cn

[U27] Py：异步 HTTP
来源：http://tpz.gogol.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://jbf.hywenlv.cn

[U28] Py：类型别名
来源：http://saf.xuanzx.com

UserId = int
来源：http://dwi.chenzaomai.com

[U29] Py：属性校验
来源：http://dyg.fktsv.cn

@property 与 @x.setter 配合
来源：http://axk.yuanzhike.top

[U30] Py：数据类
来源：http://imt.yfazqb.com

@dataclass(slots=True)
来源：http://qnm.hcnkem.com

[U31] Py：单测
来源：http://kny.sweek.top

python -m pytest -q
来源：http://ipy.yueranfly.top

[U32] Py：代码格式化
来源：http://cvf.guowangkeji.top

ruff format . && ruff check --fix .
来源：http://sow.zhaomingkeji.xyz

[U33] Py：打包发布
来源：http://kqc.9152youxi.cn

python -m build  （依赖 pyproject.toml）
来源：http://pzs.kuanghao11.cn

[U34] Py：判断编码
来源：http://xpg.yanxiufei.cn

chardet.detect(raw)
来源：http://nfa.cqqwz.cn

[U35] Py：发送邮件
来源：http://ljj.shzxlz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gki.yangfankeji.com

[U36] Py：定时任务
来源：http://ijj.cdnleiting.top

schedule.every(10).minutes.do(job)
来源：http://zxp.jyoumei.cn

[U37] Py：读写 Excel
来源：http://ecw.bbcook.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ttq.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://ydw.wangdashe.top

Path(__file__).resolve().parent
来源：http://czu.cheryme.top

[U39] Py：判断是否在交互环境
来源：http://ppz.zdbjq.cn

sys.stdout.isatty()
来源：http://kix.yj202588.top

[U40] Py：打印到标准错误
来源：http://qor.cashguo.top

print("err", file=sys.stderr)
来源：http://euz.havefunace.top

[U41] PHP：初始化 Composer 项目
来源：http://tyx.jinyuanbaomall.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ies.hfpthk.cn

[U42] PHP：PSR-4 自动加载
来源：http://auk.nanxuanxn.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fgz.tian-w.cn

[U43] PHP：声明命名空间
来源：http://lkd.zhoulong.xyz

namespace App\Http;
来源：http://nqv.vehdjk.com

[U44] PHP：开启严格类型
来源：http://fvo.ywan-chungtsiang.top

declare(strict_types=1);
来源：http://eqg.yongpay.top

[U45] PHP：类型声明与返回类型
来源：http://dia.cqqwz.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wsy.mhx1999.top

[U46] PHP：可空类型
来源：http://tne.hongshengwenyu.top

?string $name = null
来源：http://pjl.sufxvd.cn

[U47] PHP：联合类型
来源：http://etl.316326.xyz

int|string $id
来源：http://ixx.tianlin.xyz

[U48] PHP：纯枚举
来源：http://tkh.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lyg.zhengqikj.top

[U49] PHP：只读属性
来源：http://ame.jqgufenzy.top

public readonly string $name
来源：http://cyr.snrcjt.cn

[U50] PHP：构造器属性提升
来源：http://mpd.jyoumei.cn

public function __construct(private int $id) {}
来源：http://bsh.shzxlz.cn

[U51] PHP：数组解构
来源：http://jfq.quarkkingdee.top

[$a, $b] = $arr;
来源：http://nxr.xinyue.icu

[U52] PHP：箭头函数
来源：http://rfb.iojbl.cn

$double = fn($x) => $x * 2;
来源：http://czn.ehwqpu.com

[U53] PHP：空合并运算符
来源：http://eoo.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://epi.sjlbkw.cn

[U54] PHP：空安全调用
来源：http://pfs.0kj1m.cn

$obj?->method()
来源：http://dmy.zhiwuduotai.top


<!-- 参考信息 -->