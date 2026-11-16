代发 wailian999

#ifndef X_H
来源：http://ozi.iojbl.cn

#define X_H
来源：http://xls.chenlongwang.top

#endif
来源：http://szs.zhiwuduotai.top

[S31] C++：Hello World
来源：http://kdg.zhongyouzk.top

#include <iostream>
来源：http://iig.ydjk.org.cn

int main() { std::cout << "Hello\n"; }
来源：http://rgs.cheryme.top

[S32] C++：字符串
来源：http://yms.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://oct.andypj.xyz

[S33] C++：vector 增删
来源：http://stp.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xnl.zdqjudy.top

[S34] C++：遍历 vector
来源：http://utr.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://pzc.chenjidiqi.icu

[S35] C++：map
来源：http://svx.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kvs.zhijiandao.cn

[S36] C++：unordered_map
来源：http://cdq.yuxming.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uep.redwolf501.top

[S37] C++：set
来源：http://szx.cashguo.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xmh.jinyuanbaomall.cn

[S38] C++：排序
来源：http://rba.feifeiyinyue.top

std::sort(v.begin(), v.end());
来源：http://zrw.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://rkf.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fht.quarkkingdee.top

[S40] C++：查找元素
来源：http://ixj.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vss.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://jnk.gzhubu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kqr.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://xbf.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://pdh.ivvv.top

[S43] C++：智能指针
来源：http://uoi.fanxiaobao.xyz

auto p = std::make_unique<int>(5);
来源：http://mhi.aizwys.cn

[S44] C++：引用传参
来源：http://atd.zhijiandao.cn

void inc(int &x) { ++x; }
来源：http://ibe.zhaomingkeji.xyz

[S45] C++：lambda
来源：http://ric.cucudq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mkf.nwbrower.top

[S46] C++：函数模板
来源：http://rps.chenzaomai.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wnd.bjfxy.top

[S47] C++：结构化绑定遍历
来源：http://sdq.guannengcc.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ebw.bjfxy.top

[S48] C++：逐行读文件
来源：http://cwt.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mhl.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://etr.hesvh.cn

[S49] C++：写文件
来源：http://adb.jyoumei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qrx.zhongyouzk.top

[S50] C++：格式化数字
来源：http://jhi.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kfk.aibaodan.cn

[S51] C++：显式类型转换
来源：http://mdi.9152youxi.cn

static_cast<double>(a) / b
来源：http://lsw.gzhubu.top

[S52] C++：const 与 noexcept
来源：http://jqg.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://qhi.uphjek.com

[S53] C++：移动语义
来源：http://vfh.yonumen.top

std::vector<int> w = std::move(v);
来源：http://bvm.gaohongyu789.top

[S54] C++：异常处理
来源：http://pcs.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kpm.fktsv.cn

[S55] C++：结构化绑定
来源：http://njf.tian-w.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wfc.bjfxy.top

[S56] C++：optional
来源：http://grf.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iyp.hfpthk.cn

[S57] C++：编译期常量
来源：http://vrk.cucudq.cn

constexpr int N = 10;
来源：http://wrh.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://wdj.sjlbkw.cn

namespace ns { int f() { return 1; } }
来源：http://cml.aizwys.cn

[S59] C++：静态断言
来源：http://zym.wangshuangyany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hjy.zhaomingkeji.xyz

[S60] C++：遍历并删除元素
来源：http://wyr.xylfe.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ptl.xinyue.icu

================================================================================
来源：http://bhx.yonumen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://npm.nanxinkj.top

================================================================================
来源：http://nhg.52xcode.cn

[T01] Kotlin：Hello World
来源：http://ctu.zhaomingkeji.xyz

println("Hello")
来源：http://vrp.tanke756.top

[T02] Kotlin：变量
来源：http://kpi.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cwn.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://zxh.hcnkem.com

"值: $b"
来源：http://mge.yuxming.cn

[T04] Kotlin：空安全
来源：http://wtr.yj202588.top

val n: String? = null;  n?.length
来源：http://zfv.tanke756.top

[T05] Kotlin：when 表达式
来源：http://uqd.aizwys.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lrb.fehbvm.com

[T06] Kotlin：集合映射
来源：http://nxn.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rnr.bbcook.cn

[T07] Kotlin：集合过滤
来源：http://klq.yuxming.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dzy.cucudq.cn

[T08] Kotlin：数据类
来源：http://wte.xinyue.icu

data class User(val name: String, val age: Int)
来源：http://qkb.yvedp.cn

[T09] Kotlin：扩展函数
来源：http://xns.jinqigfzy.top

fun String.exclaim() = this + "!"
来源：http://rnj.zhijiandao.cn

[T10] Kotlin：默认参数
来源：http://zsm.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zti.tarul.cn

[T11] Kotlin：协程
来源：http://cvd.sxryk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://roi.shuidangran.top

[T12] Kotlin：解构声明
来源：http://tqp.quarkkingdee.top

val (a, b) = Pair(1, 2)
来源：http://qaj.zycfv.cn

[T13] Kotlin：只读 Map
来源：http://cwy.gogol.net.cn

val m = mapOf("a" to 1)
来源：http://chm.ctjpmb.com

[T14] Kotlin：循环
来源：http://pry.yj20258.top

for (i in 1..10) println(i)
来源：http://jce.nwbrower.top

[T15] Kotlin：接口
来源：http://vcm.yonumen.top

interface Shape { fun area(): Double }
来源：http://rou.yongpay.top

[T16] Swift：Hello World
来源：http://rqt.guowangkeji.top

print("Hello")
来源：http://fbl.fktsv.cn

[T17] Swift：变量与常量
来源：http://vhx.hcnkem.com

var a = 1;  let b = 2
来源：http://psz.fzhhl.top

[T18] Swift：字符串插值
来源：http://rpj.ydzc1.top

"值: \(b)"
来源：http://yon.tanke756.top

[T19] Swift：可选绑定
来源：http://fgy.aizwys.cn

if let n = opt { print(n) }
来源：http://edw.yonumen.top

[T20] Swift：数组操作
来源：http://lwh.aibaodan.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zzl.birdmap.top

[T21] Swift：遍历
来源：http://egm.iojbl.cn

for x in a { print(x) }
来源：http://qry.chenjidiqi.icu

[T22] Swift：字典
来源：http://dlx.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://fng.ehwqpu.com

[T23] Swift：函数
来源：http://koz.shangyingyoupin.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ggr.xuetiantiany.cn

[T24] Swift：闭包
来源：http://dum.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://avk.bjfxy.top

[T25] Swift：结构体
来源：http://ldz.svipenyu.cn

struct P { var x: Int }
来源：http://yvc.sjlbkw.cn

[T26] Swift：类与重写
来源：http://qid.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://vrw.yuxming.cn

[T27] Swift：错误处理
来源：http://aag.zhiwuduotai.top

do { try f() } catch { print(error) }
来源：http://tkj.svipenyu.cn

[T28] Swift：枚举
来源：http://zfy.ydjk.org.cn

enum Color { case red, green }
来源：http://orw.zhixingplan.top

[T29] Swift：guard 提前返回
来源：http://wga.chenlongwang.top

guard let x = opt else { return }
来源：http://vgd.cqqwz.cn

[T30] Swift：协议
来源：http://suc.ctjpmb.com

protocol Shape { func area() -> Double }
来源：http://oyy.zdqjudy.top

[T31] Lua：Hello World
来源：http://gch.shanyushiyangtech.top

print("Hello")
来源：http://abm.feifeiyinyue.top

[T32] Lua：局部变量
来源：http://lbn.guowangkeji.top

local a = 1
来源：http://udg.dashuyun.cn

[T33] Lua：表（数组）
来源：http://enx.chenlongwang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://yrw.shzxlz.cn

[T34] Lua：遍历表
来源：http://aac.yonumen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hsw.cdnleiting.top

[T35] Lua：字典表
来源：http://yww.daria6918.cn

local d = { a = 1 };  d.b = 2
来源：http://uid.ctjpmb.com

[T36] Lua：函数
来源：http://plp.zdqjudy.top

function add(a, b) return a + b end
来源：http://ubz.hnqzz.top

[T37] Lua：字符串拼接
来源：http://qwc.yvedp.cn

"a" .. "b"
来源：http://eiv.xingfuxueyuan.xyz

[T38] Lua：条件
来源：http://amx.mhx1999.top

if x > 0 then print("正") end
来源：http://hsy.hammf.cn

[T39] Lua：模式匹配
来源：http://yhb.guowangkeji.top

string.find(s, "%d+")
来源：http://tgp.gotoacloud.top

[T40] Lua：元表
来源：http://ysw.cqqwz.cn

setmetatable({}, { __index = base })
来源：http://sug.hammf.cn

[T41] Perl：Hello World
来源：http://pry.xuanzx.com

print "Hello\n";
来源：http://bcr.shanyushiyangkeji.top

[T42] Perl：变量类型
来源：http://aqp.havefunace.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hvl.hysaishi.cn

[T43] Perl：字符串插值
来源：http://yvz.sjlbkw.cn

"值: $a"
来源：http://zrx.zycfv.cn

[T44] Perl：条件
来源：http://cjw.yongpay.top

if ($a > 0) { print "正"; }
来源：http://lqk.jinghuilouyu.cn

[T45] Perl：数组遍历
来源：http://ubm.hnxiangtu.top

for my $x (@arr) { print $x; }
来源：http://jpu.nwbrower.top

[T46] Perl：哈希操作
来源：http://xvw.ctjpmb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nof.yj20258.top

[T47] Perl：正则捕获
来源：http://tau.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://hev.hysaishi.cn

[T48] Perl：正则替换
来源：http://qcz.ybcxt.top

$s =~ s/old/new/g;
来源：http://otj.316326.xyz

[T49] Perl：函数
来源：http://qaf.mhx1999.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gfn.vehdjk.com

[T50] Perl：逐行读文件
来源：http://rik.cqqwz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ycs.aizwys.cn

while (my $line = <$fh>) { print $line; }
来源：http://ypw.yfazqb.com

[T51] Scala：Hello World
来源：http://lax.9152youxi.cn

println("Hello")
来源：http://ecy.dianchejie.cn

[T52] Scala：变量
来源：http://yow.chenlongwang.top

val a = 1;  var b = 2
来源：http://ufy.snrcjt.cn

[T53] Scala：字符串插值
来源：http://nnj.hesvh.cn

s"值: $b"
来源：http://ovq.guowangkeji.top

[T54] Scala：集合映射
来源：http://iqx.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://zqo.yuxming.cn

[T55] Scala：集合过滤
来源：http://oog.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dkx.chenzaomai.com

[T56] Scala：样例类
来源：http://mgz.9152youxi.cn

case class User(name: String, age: Int)
来源：http://lmb.xylfe.cn

[T57] Scala：模式匹配
来源：http://hng.shanyushiyangtech.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ipb.hongshengwenyu.top

[T58] Scala：函数定义
来源：http://bfe.cqqwz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nuo.dianchejie.cn

[T59] Scala：循环
来源：http://ygz.yonumen.top

for (i <- 1 to 10) println(i)
来源：http://lke.ehwqpu.com

[T60] Scala：折叠
来源：http://goh.fzhhl.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://frs.smart0.xyz

================================================================================
来源：http://vet.chenzaomai.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://drb.jqgfzy.top

================================================================================
来源：http://wgy.zycfv.cn

[U01] Py：创建虚拟环境
来源：http://xpl.hywenlv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wmp.fzhhl.top

[U02] Py：导出 / 安装依赖
来源：http://sha.daria6918.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sve.vehdjk.com

[U03] Py：加载 .env 配置
来源：http://unp.zhijiandao.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://krl.fzhhl.top

[U04] Py：变量调试打印
来源：http://jwf.316326.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aeu.zhaomingkeji.xyz

[U05] Py：列表去重且保序
来源：http://gxc.gogol.net.cn

list(dict.fromkeys(arr))
来源：http://wfx.yj20258.top

[U06] Py：合并两个字典
来源：http://mbl.hnxiangtu.top

{**a, **b}
来源：http://mqu.kuanghao11.cn

[U07] Py：反转字典键值
来源：http://syq.xingfuxueyuan.xyz

{v: k for k, v in d.items()}
来源：http://zsx.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://zsq.haohaochexian.top

[y for x in nested for y in x]
来源：http://wld.cashguo.top

[U09] Py：字典取最大值的键
来源：http://lbq.yj202588.top

max(d, key=d.get)
来源：http://lhb.zycfv.cn

[U10] Py：按值排序字典
来源：http://grp.daxiang520.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gxu.jinqigfzy.top

[U11] Py：生成器表达式
来源：http://pyy.zhengqikj.top

(x * 2 for x in arr)
来源：http://plb.52xcode.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qtv.zdbjq.cn

Counter(arr).most_common(3)
来源：http://mrx.zhaomingkeji.xyz

[U13] Py：固定长度队列
来源：http://bfx.meibo888.top

deque(maxlen=10)
来源：http://ggk.yonumen.top

[U14] Py：分组收集到列表
来源：http://vkz.uphjek.com

defaultdict(list)
来源：http://bip.bbcook.cn

[U15] Py：高精度计时
来源：http://mnu.jiagoushi.top

t = time.perf_counter()
来源：http://xfv.hnqzz.top

[U16] Py：命令行参数解析
来源：http://xqh.0kj1m.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jbf.chenlongwang.top

[U17] Py：初始化日志
来源：http://dkb.jqgfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://saz.yj20258888.top

[U18] Py：预编译正则
来源：http://dzu.zhaomingkeji.xyz

pat = re.compile(r"\d+")
来源：http://qik.meibo888.top

[U19] Py：正则替换带回调
来源：http://fdx.zhiwuduotai.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://woz.zhaomingkeji.xyz

[U20] Py：缓存函数结果
来源：http://fts.yvedp.cn

@functools.lru_cache(maxsize=None)
来源：http://awb.ppjwa.cn

[U21] Py：自定义上下文管理器
来源：http://okv.yonumen.top

@contextlib.contextmanager
来源：http://rvj.xuetiantiany.cn

[U22] Py：矩阵转置
来源：http://ynf.chenzaomai.com

list(zip(*m))
来源：http://gjp.hnqzz.top

[U23] Py：分块读取大文件
来源：http://wwj.tianlin.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://brn.ybcxt.top

[U24] Py：路径操作
来源：http://fpk.ydjk.org.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ogh.cashguo.top

[U25] Py：CSV 按字典读
来源：http://idl.yueranfly.top

csv.DictReader(f)
来源：http://jjl.sysykeji.top

[U26] Py：并发下载
来源：http://ddq.snrcjt.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bvn.yj20258.top

[U27] Py：异步 HTTP
来源：http://zak.snrcjt.cn

aiohttp.ClientSession() 配合 async with
来源：http://rbe.fehbvm.com

[U28] Py：类型别名
来源：http://hwb.zdqjudy.top

UserId = int
来源：http://vwm.dianchejie.cn

[U29] Py：属性校验
来源：http://vkt.iojbl.cn

@property 与 @x.setter 配合
来源：http://slv.wangshuangyany.cn

[U30] Py：数据类
来源：http://rlt.jinqigfzy.top

@dataclass(slots=True)
来源：http://cyz.yvedp.cn

[U31] Py：单测
来源：http://fvu.quarkkingdee.top

python -m pytest -q
来源：http://bbf.ywan-chungtsiang.top

[U32] Py：代码格式化
来源：http://fig.xziqi.cn

ruff format . && ruff check --fix .
来源：http://gzl.xziqi.cn

[U33] Py：打包发布
来源：http://ewy.aibaodan.cn

python -m build  （依赖 pyproject.toml）
来源：http://drj.birdmap.top

[U34] Py：判断编码
来源：http://ekh.jinghuilouyu.cn

chardet.detect(raw)
来源：http://qgn.haohaochexian.top

[U35] Py：发送邮件
来源：http://egx.yj20258.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tvd.jinyuanbaomall.cn

[U36] Py：定时任务
来源：http://jic.jinyuanbaomall.cn

schedule.every(10).minutes.do(job)
来源：http://xie.yonumen.top

[U37] Py：读写 Excel
来源：http://hwj.daxiang520.top

pandas.read_excel / DataFrame.to_excel
来源：http://phj.birdmap.top

[U38] Py：获取脚本所在目录
来源：http://nux.zdqjudy.top

Path(__file__).resolve().parent
来源：http://mzs.yanxiufei.cn

[U39] Py：判断是否在交互环境
来源：http://anv.shzxlz.cn

sys.stdout.isatty()
来源：http://wgb.yfazqb.com

[U40] Py：打印到标准错误
来源：http://wto.zdbjq.cn

print("err", file=sys.stderr)
来源：http://zhx.gogol.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://dgn.zhiwuduotai.top

composer init;  composer require guzzlehttp/guzzle
来源：http://tqq.xylfe.cn

[U42] PHP：PSR-4 自动加载
来源：http://rmp.zhaomingkeji.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aag.xinyue.icu

[U43] PHP：声明命名空间
来源：http://yok.iojbl.cn

namespace App\Http;
来源：http://qxs.fktsv.cn

[U44] PHP：开启严格类型
来源：http://asj.andypj.xyz

declare(strict_types=1);
来源：http://ffk.nanxuanxn.top

[U45] PHP：类型声明与返回类型
来源：http://kob.jianghu66.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ljd.jyoumei.cn

[U46] PHP：可空类型
来源：http://mwm.zhengqikj.top

?string $name = null
来源：http://qdx.fengsongda.top

[U47] PHP：联合类型
来源：http://muu.jiagoushi.top

int|string $id
来源：http://bzd.nwbrower.top

[U48] PHP：纯枚举
来源：http://lbh.jyoumei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dhi.fktsv.cn

[U49] PHP：只读属性
来源：http://shl.kuanghao11.cn

public readonly string $name
来源：http://uex.ybcxt.top

[U50] PHP：构造器属性提升
来源：http://nbe.hfpthk.cn

public function __construct(private int $id) {}
来源：http://dqh.tianlin.xyz

[U51] PHP：数组解构
来源：http://vvf.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://sns.fktsv.cn

[U52] PHP：箭头函数
来源：http://lkj.cucudq.cn

$double = fn($x) => $x * 2;
来源：http://ced.hesvh.cn

[U53] PHP：空合并运算符
来源：http://lfn.yueranfly.top

$v = $a ?? $b ?? "default";
来源：http://zll.meibo888.top

[U54] PHP：空安全调用
来源：http://zbl.gogol.net.cn

$obj?->method()
来源：http://gph.ywan-chungtsiang.top


<!-- 参考信息 -->