代发 wailian999

static int counter = 0;
来源：http://dfj.xinyue.icu

[S29] C：变参函数
来源：http://twj.shanyushiyangtech.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hdx.c1oappe.top

[S30] C：头文件保护
来源：http://sxy.fehbvm.com

#ifndef X_H
来源：http://glq.xingfuxueyuan.xyz

#define X_H
来源：http://ibl.cdnleiting.top

#endif
来源：http://ppe.shangyingyoupin.top

[S31] C++：Hello World
来源：http://fdm.yuanzhike.top

#include <iostream>
来源：http://kul.fktsv.cn

int main() { std::cout << "Hello\n"; }
来源：http://vlf.hongshengwenyu.top

[S32] C++：字符串
来源：http://ywx.xuanzx.com

std::string s = "hi";  s += "!";
来源：http://iom.shzxlz.cn

[S33] C++：vector 增删
来源：http://iqg.andypj.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ozy.tianlin.xyz

[S34] C++：遍历 vector
来源：http://nyx.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://zzg.xuetiantiany.cn

[S35] C++：map
来源：http://dqi.ybcxt.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jgl.uphjek.com

[S36] C++：unordered_map
来源：http://ety.hysaishi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kxr.hywenlv.cn

[S37] C++：set
来源：http://kgr.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qis.tian-w.cn

[S38] C++：排序
来源：http://nvd.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://hep.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://tjq.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rns.jqgufenzy.top

[S40] C++：查找元素
来源：http://bxu.sxryk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ist.fzhhl.top

[S41] C++：类与构造函数
来源：http://vhs.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eqi.yueranfly.top

[S42] C++：继承与虚函数
来源：http://jjo.dashuyun.cn

class B : public Base { public: void f() override {} };
来源：http://qyh.nanxuanxn.top

[S43] C++：智能指针
来源：http://avw.daria6918.cn

auto p = std::make_unique<int>(5);
来源：http://las.cdnleiting.top

[S44] C++：引用传参
来源：http://zbw.gzhubu.top

void inc(int &x) { ++x; }
来源：http://ywh.zhixingplan.top

[S45] C++：lambda
来源：http://mlm.bbcook.cn

auto add = [](int a, int b) { return a + b; };
来源：http://six.yj202588.top

[S46] C++：函数模板
来源：http://yjb.zhijiandao.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mfw.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://qfh.316326.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://syq.yanxiufei.cn

[S48] C++：逐行读文件
来源：http://jeo.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://fof.meibo888.top

while (std::getline(in, line)) { }
来源：http://nwl.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://isv.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qkt.bjfxy.top

[S50] C++：格式化数字
来源：http://rgf.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hte.bbcook.cn

[S51] C++：显式类型转换
来源：http://epu.cheryme.top

static_cast<double>(a) / b
来源：http://mtx.sufxvd.cn

[S52] C++：const 与 noexcept
来源：http://rcm.cheryme.top

int size() const noexcept { return n_; }
来源：http://gbr.yanxiufei.cn

[S53] C++：移动语义
来源：http://icl.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://jbi.shangyingyoupin.top

[S54] C++：异常处理
来源：http://ijb.redwolf501.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rpf.xinyue.icu

[S55] C++：结构化绑定
来源：http://bux.yanxiufei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://svg.ywan-chungtsiang.top

[S56] C++：optional
来源：http://zmh.hesvh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ruu.mhx1999.top

[S57] C++：编译期常量
来源：http://pxd.hywenlv.cn

constexpr int N = 10;
来源：http://taa.fehbvm.com

[S58] C++：命名空间
来源：http://opn.uphjek.com

namespace ns { int f() { return 1; } }
来源：http://ngp.zdqjudy.top

[S59] C++：静态断言
来源：http://bkn.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bmj.yj20258888.top

[S60] C++：遍历并删除元素
来源：http://jtw.ydjk.org.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://snt.tarul.cn

================================================================================
来源：http://hsy.52xcode.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cep.bbcook.cn

================================================================================
来源：http://myq.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://xyc.hysaishi.cn

println("Hello")
来源：http://oeo.mhx1999.top

[T02] Kotlin：变量
来源：http://ige.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jqx.ivvv.top

[T03] Kotlin：字符串模板
来源：http://cms.fehbvm.com

"值: $b"
来源：http://brd.jianghu66.top

[T04] Kotlin：空安全
来源：http://tva.snrcjt.cn

val n: String? = null;  n?.length
来源：http://dir.zdbjq.cn

[T05] Kotlin：when 表达式
来源：http://sbe.nwbrower.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vhq.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://sbi.uphjek.com

listOf(1, 2, 3).map { it * 2 }
来源：http://juf.birdmap.top

[T07] Kotlin：集合过滤
来源：http://bzl.nanxinkj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pfe.zhoulong.xyz

[T08] Kotlin：数据类
来源：http://lpk.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://ith.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://akf.cucudq.cn

fun String.exclaim() = this + "!"
来源：http://usu.nanxuanxn.top

[T10] Kotlin：默认参数
来源：http://jfr.andypj.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://wnz.yj202588.top

[T11] Kotlin：协程
来源：http://uay.pengpengdd.cyou

GlobalScope.launch { delay(1000); println("done") }
来源：http://gnq.nwbrower.top

[T12] Kotlin：解构声明
来源：http://eaj.dashuyun.cn

val (a, b) = Pair(1, 2)
来源：http://ysf.ydjk.org.cn

[T13] Kotlin：只读 Map
来源：http://ted.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://qnv.aibaodan.cn

[T14] Kotlin：循环
来源：http://wne.ehwqpu.com

for (i in 1..10) println(i)
来源：http://lsh.meibo888.top

[T15] Kotlin：接口
来源：http://ahk.jqgufenzy.top

interface Shape { fun area(): Double }
来源：http://zru.sxryk.cn

[T16] Swift：Hello World
来源：http://wqy.hammf.cn

print("Hello")
来源：http://xaq.quarkkingdee.top

[T17] Swift：变量与常量
来源：http://xtr.zhaomingkeji.xyz

var a = 1;  let b = 2
来源：http://lpe.guannengcc.top

[T18] Swift：字符串插值
来源：http://rqm.snrcjt.cn

"值: \(b)"
来源：http://ldj.wangdashe.top

[T19] Swift：可选绑定
来源：http://ipu.zhijiandao.cn

if let n = opt { print(n) }
来源：http://gmm.birdmap.top

[T20] Swift：数组操作
来源：http://ynv.fzhhl.top

var a = [1, 2, 3];  a.append(4)
来源：http://clk.yonumen.top

[T21] Swift：遍历
来源：http://dxc.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://xtb.xylfe.cn

[T22] Swift：字典
来源：http://cxt.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://wyz.hammf.cn

[T23] Swift：函数
来源：http://mjj.gaohongyu789.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kvr.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://lrq.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://epr.aizwys.cn

[T25] Swift：结构体
来源：http://aot.ywan-chungtsiang.top

struct P { var x: Int }
来源：http://yvb.yueranfly.top

[T26] Swift：类与重写
来源：http://bld.sjlbkw.cn

class A: Base { override func f() {} }
来源：http://twv.tian-w.cn

[T27] Swift：错误处理
来源：http://fek.shzxlz.cn

do { try f() } catch { print(error) }
来源：http://tnm.jianghu66.top

[T28] Swift：枚举
来源：http://hsx.quarkkingdee.top

enum Color { case red, green }
来源：http://dmt.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://wek.fanxiaobao.xyz

guard let x = opt else { return }
来源：http://fej.bjfxy.top

[T30] Swift：协议
来源：http://gho.yanxiufei.cn

protocol Shape { func area() -> Double }
来源：http://llt.fanxiaobao.xyz

[T31] Lua：Hello World
来源：http://int.mhx1999.top

print("Hello")
来源：http://rjd.hammf.cn

[T32] Lua：局部变量
来源：http://xby.redwolf501.top

local a = 1
来源：http://cvp.vqdsnc.cn

[T33] Lua：表（数组）
来源：http://lmi.jqgufenzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://sxv.hesvh.cn

[T34] Lua：遍历表
来源：http://nig.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ojc.ywan-chungtsiang.top

[T35] Lua：字典表
来源：http://kap.zhoulong.xyz

local d = { a = 1 };  d.b = 2
来源：http://zfx.zdbjq.cn

[T36] Lua：函数
来源：http://cbi.jiagoushi.top

function add(a, b) return a + b end
来源：http://dce.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://foh.yonumen.top

"a" .. "b"
来源：http://hhx.zhongyouzk.top

[T38] Lua：条件
来源：http://tpk.xuanzx.com

if x > 0 then print("正") end
来源：http://xvw.316326.xyz

[T39] Lua：模式匹配
来源：http://sgm.snrcjt.cn

string.find(s, "%d+")
来源：http://dmd.yuanzhike.top

[T40] Lua：元表
来源：http://opt.nwbrower.top

setmetatable({}, { __index = base })
来源：http://avw.epnwcf.com

[T41] Perl：Hello World
来源：http://qqe.nanxuanxn.top

print "Hello\n";
来源：http://eul.jinyuanbaomall.cn

[T42] Perl：变量类型
来源：http://hrg.nwbrower.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xhw.yueranfly.top

[T43] Perl：字符串插值
来源：http://hzi.jyoumei.cn

"值: $a"
来源：http://jsd.zhiwuduotai.top

[T44] Perl：条件
来源：http://fnm.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://aiw.shanyushiyangtech.top

[T45] Perl：数组遍历
来源：http://swl.gzhubu.top

for my $x (@arr) { print $x; }
来源：http://wwa.hnqzz.top

[T46] Perl：哈希操作
来源：http://ifw.redwolf501.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://prq.sweek.top

[T47] Perl：正则捕获
来源：http://pwy.feifeiyinyue.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kmf.meibo888.top

[T48] Perl：正则替换
来源：http://ccv.zhengqikj.top

$s =~ s/old/new/g;
来源：http://yjc.zycfv.cn

[T49] Perl：函数
来源：http://njt.xinyue.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yiu.iojbl.cn

[T50] Perl：逐行读文件
来源：http://ddu.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zjq.guannengcc.top

while (my $line = <$fh>) { print $line; }
来源：http://xwc.hywenlv.cn

[T51] Scala：Hello World
来源：http://pal.hysaishi.cn

println("Hello")
来源：http://zsi.jinyuanbaomall.cn

[T52] Scala：变量
来源：http://jjn.redwolf501.top

val a = 1;  var b = 2
来源：http://tse.xziqi.cn

[T53] Scala：字符串插值
来源：http://sfu.shuidangran.top

s"值: $b"
来源：http://bis.gotoacloud.top

[T54] Scala：集合映射
来源：http://yeb.jinghuilouyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://nqz.zdbjq.cn

[T55] Scala：集合过滤
来源：http://ymg.zhongyouzk.top

List(1, 2, 3).filter(_ > 1)
来源：http://rfr.xylfe.cn

[T56] Scala：样例类
来源：http://mwn.snrcjt.cn

case class User(name: String, age: Int)
来源：http://bou.yonumen.top

[T57] Scala：模式匹配
来源：http://dos.52xcode.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://txd.cashguo.top

[T58] Scala：函数定义
来源：http://qax.sjlbkw.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wrb.zdqjudy.top

[T59] Scala：循环
来源：http://odd.xziqi.cn

for (i <- 1 to 10) println(i)
来源：http://gqm.9152youxi.cn

[T60] Scala：折叠
来源：http://isv.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://unw.jqgfzy.top

================================================================================
来源：http://szn.aibaodan.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ebn.nanxuanxn.top

================================================================================
来源：http://mid.tarul.cn

[U01] Py：创建虚拟环境
来源：http://oxe.yfazqb.com

python -m venv .venv && source .venv/bin/activate
来源：http://hwf.birdmap.top

[U02] Py：导出 / 安装依赖
来源：http://grc.gotoacloud.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fur.bjfxy.top

[U03] Py：加载 .env 配置
来源：http://elf.fengsongda.top

from dotenv import load_dotenv; load_dotenv()
来源：http://txk.fengsongda.top

[U04] Py：变量调试打印
来源：http://tgk.cucudq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iga.zhiwuduotai.top

[U05] Py：列表去重且保序
来源：http://byy.jinyuanbaomall.cn

list(dict.fromkeys(arr))
来源：http://qyr.bbcook.cn

[U06] Py：合并两个字典
来源：http://ubb.cdnleiting.top

{**a, **b}
来源：http://liz.quarkkingdee.top

[U07] Py：反转字典键值
来源：http://vva.daria6918.cn

{v: k for k, v in d.items()}
来源：http://lhf.redwolf501.top

[U08] Py：展平二维列表
来源：http://ipm.gzhubu.top

[y for x in nested for y in x]
来源：http://utl.xylfe.cn

[U09] Py：字典取最大值的键
来源：http://jrv.fehbvm.com

max(d, key=d.get)
来源：http://ubp.hfpthk.cn

[U10] Py：按值排序字典
来源：http://eaw.gogol.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pft.yongpay.top

[U11] Py：生成器表达式
来源：http://uut.jqgufenzy.top

(x * 2 for x in arr)
来源：http://hsd.aibaodan.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xir.shzxlz.cn

Counter(arr).most_common(3)
来源：http://lko.hnqzz.top

[U13] Py：固定长度队列
来源：http://vtp.zhijiandao.cn

deque(maxlen=10)
来源：http://olx.ivvv.top

[U14] Py：分组收集到列表
来源：http://ogw.wangdashe.top

defaultdict(list)
来源：http://ntq.jinyuanbaomall.cn

[U15] Py：高精度计时
来源：http://gls.feifeiyinyue.top

t = time.perf_counter()
来源：http://isc.xinyue.icu

[U16] Py：命令行参数解析
来源：http://zlk.fanxiaobao.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qef.xuanzx.com

[U17] Py：初始化日志
来源：http://boi.shuidangran.top

logging.basicConfig(level=logging.INFO)
来源：http://yyq.yonumen.top

[U18] Py：预编译正则
来源：http://dpb.fktsv.cn

pat = re.compile(r"\d+")
来源：http://vyy.xinyue.icu

[U19] Py：正则替换带回调
来源：http://hom.fktsv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zlm.nanxuanxn.top

[U20] Py：缓存函数结果
来源：http://pxn.pycfn.com

@functools.lru_cache(maxsize=None)
来源：http://euy.yvedp.cn

[U21] Py：自定义上下文管理器
来源：http://gdb.zycfv.cn

@contextlib.contextmanager
来源：http://rkv.zdqjudy.top

[U22] Py：矩阵转置
来源：http://sif.nanxinkj.top

list(zip(*m))
来源：http://lsn.shanyushiyangkeji.top

[U23] Py：分块读取大文件
来源：http://coz.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kkz.sysykeji.top

[U24] Py：路径操作
来源：http://cpj.cqqwz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dib.bjfxy.top

[U25] Py：CSV 按字典读
来源：http://sns.jqgfzy.top

csv.DictReader(f)
来源：http://ajy.aibaodan.cn

[U26] Py：并发下载
来源：http://ejx.yfazqb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dqb.yj20258.top

[U27] Py：异步 HTTP
来源：http://iua.zhiwuduotai.top

aiohttp.ClientSession() 配合 async with
来源：http://ktr.zhoulong.xyz

[U28] Py：类型别名
来源：http://bwk.jinghuilouyu.cn

UserId = int
来源：http://ujw.ivvv.top

[U29] Py：属性校验
来源：http://mnr.jyoumei.cn

@property 与 @x.setter 配合
来源：http://mem.bjfxy.top

[U30] Py：数据类
来源：http://mam.kuanghao11.cn

@dataclass(slots=True)
来源：http://oxu.ctjpmb.com

[U31] Py：单测
来源：http://aox.sufxvd.cn

python -m pytest -q
来源：http://ioh.sweek.top

[U32] Py：代码格式化
来源：http://qxf.jinqigfzy.top

ruff format . && ruff check --fix .
来源：http://ibr.yuxming.cn

[U33] Py：打包发布
来源：http://wtz.bbcook.cn

python -m build  （依赖 pyproject.toml）
来源：http://jpm.zdqjudy.top

[U34] Py：判断编码
来源：http://bye.uphjek.com

chardet.detect(raw)
来源：http://rvz.hnqzz.top

[U35] Py：发送邮件
来源：http://reb.guannengcc.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fzm.hongshengwenyu.top

[U36] Py：定时任务
来源：http://ict.yuxming.cn

schedule.every(10).minutes.do(job)
来源：http://wtp.zhoulong.xyz

[U37] Py：读写 Excel
来源：http://ymp.xziqi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dei.hnqzz.top

[U38] Py：获取脚本所在目录
来源：http://bhj.zhijiandao.cn

Path(__file__).resolve().parent
来源：http://ccc.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://ovk.hnxiangtu.top

sys.stdout.isatty()
来源：http://rdm.guannengcc.top

[U40] Py：打印到标准错误
来源：http://adh.zhongyouzk.top

print("err", file=sys.stderr)
来源：http://rfd.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://lxc.yj20258.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ena.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://dqa.zdbjq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://djw.yangfankeji.com

[U43] PHP：声明命名空间
来源：http://owl.xinyue.icu

namespace App\Http;
来源：http://gyd.zhoulong.xyz

[U44] PHP：开启严格类型
来源：http://dpl.yuanzhike.top

declare(strict_types=1);
来源：http://tii.nanxuanxn.top

[U45] PHP：类型声明与返回类型
来源：http://cxe.shanyushiyangtech.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pzd.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://reu.bjfxy.top

?string $name = null
来源：http://kcp.sxryk.cn

[U47] PHP：联合类型
来源：http://ege.chenlongwang.top

int|string $id
来源：http://pns.yj20258.top

[U48] PHP：纯枚举
来源：http://mrq.jinghuilouyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bnb.shanyushiyangkeji.top

[U49] PHP：只读属性
来源：http://ekj.zhengqikj.top

public readonly string $name
来源：http://fnm.pycfn.com

[U50] PHP：构造器属性提升
来源：http://zeq.tarul.cn

public function __construct(private int $id) {}
来源：http://guf.ehwqpu.com

[U51] PHP：数组解构
来源：http://zhl.jinyuanbaomall.cn

[$a, $b] = $arr;
来源：http://oxh.xylfe.cn

[U52] PHP：箭头函数
来源：http://hjn.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://rwe.pengpengdd.cyou


<!-- 参考信息 -->