代发 wailian999

#ifndef X_H
来源：http://iga.fengsongda.top

#define X_H
来源：http://tfd.ybcxt.top

#endif
来源：http://dkt.hnqzz.top

[S31] C++：Hello World
来源：http://ymn.9152youxi.cn

#include <iostream>
来源：http://wgz.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://lhx.jlsjyb.cn

[S32] C++：字符串
来源：http://wwk.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://ixs.nanxuanxn.top

[S33] C++：vector 增删
来源：http://dec.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vcl.yj20258888.top

[S34] C++：遍历 vector
来源：http://crk.yuanzhike.top

for (auto &x : v) { std::cout << x; }
来源：http://wfw.gotoacloud.top

[S35] C++：map
来源：http://orc.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pqw.guowangkeji.top

[S36] C++：unordered_map
来源：http://qph.birdmap.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gtn.316326.xyz

[S37] C++：set
来源：http://stc.fzhhl.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wvd.aizwys.cn

[S38] C++：排序
来源：http://iyc.chenzaomai.com

std::sort(v.begin(), v.end());
来源：http://gvo.wangshuangyany.cn

[S39] C++：自定义比较器排序
来源：http://kvo.jqgufenzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jvu.dashuyun.cn

[S40] C++：查找元素
来源：http://wgs.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ojy.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://cpo.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cnw.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://upu.guannengcc.top

class B : public Base { public: void f() override {} };
来源：http://jkf.yvedp.cn

[S43] C++：智能指针
来源：http://ycr.0kj1m.cn

auto p = std::make_unique<int>(5);
来源：http://ude.zdbjq.cn

[S44] C++：引用传参
来源：http://kev.mhx1999.top

void inc(int &x) { ++x; }
来源：http://pva.daria6918.cn

[S45] C++：lambda
来源：http://vmj.wangdashe.top

auto add = [](int a, int b) { return a + b; };
来源：http://hzv.316326.xyz

[S46] C++：函数模板
来源：http://itr.hfpthk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rxg.ydzc1.top

[S47] C++：结构化绑定遍历
来源：http://rqr.aibaodan.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bqw.nanxinkj.top

[S48] C++：逐行读文件
来源：http://mvx.vqdsnc.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bpb.xinyue.icu

while (std::getline(in, line)) { }
来源：http://kjf.ehwqpu.com

[S49] C++：写文件
来源：http://ple.yj20258.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lyi.jqgfzy.top

[S50] C++：格式化数字
来源：http://vur.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eqq.xuanzx.com

[S51] C++：显式类型转换
来源：http://vjn.ppjwa.cn

static_cast<double>(a) / b
来源：http://pdq.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://jkh.sweek.top

int size() const noexcept { return n_; }
来源：http://mdz.xziqi.cn

[S53] C++：移动语义
来源：http://scq.shzxlz.cn

std::vector<int> w = std::move(v);
来源：http://pmh.zhengqikj.top

[S54] C++：异常处理
来源：http://whg.yuxming.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://efi.gotoacloud.top

[S55] C++：结构化绑定
来源：http://lzi.mhx1999.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wzf.jlsjyb.cn

[S56] C++：optional
来源：http://lij.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://phe.havefunace.top

[S57] C++：编译期常量
来源：http://kxa.yuxming.cn

constexpr int N = 10;
来源：http://obm.andypj.xyz

[S58] C++：命名空间
来源：http://yce.guannengcc.top

namespace ns { int f() { return 1; } }
来源：http://gqd.tanke756.top

[S59] C++：静态断言
来源：http://prj.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ppd.havefunace.top

[S60] C++：遍历并删除元素
来源：http://wrb.xuanzx.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nxc.uphjek.com

================================================================================
来源：http://xvd.fanxiaobao.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mrh.fzhhl.top

================================================================================
来源：http://csx.mhx1999.top

[T01] Kotlin：Hello World
来源：http://vie.quarkkingdee.top

println("Hello")
来源：http://sbl.bbcook.cn

[T02] Kotlin：变量
来源：http://idj.cqqwz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ffi.zdqjudy.top

[T03] Kotlin：字符串模板
来源：http://acm.jinqigfzy.top

"值: $b"
来源：http://hwv.ywan-chungtsiang.top

[T04] Kotlin：空安全
来源：http://ajb.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://npq.tarul.cn

[T05] Kotlin：when 表达式
来源：http://rwl.tianlin.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zih.zdbjq.cn

[T06] Kotlin：集合映射
来源：http://clq.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kts.jiagoushi.top

[T07] Kotlin：集合过滤
来源：http://mef.shanyushiyangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jnt.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://jci.fehbvm.com

data class User(val name: String, val age: Int)
来源：http://khv.hnqzz.top

[T09] Kotlin：扩展函数
来源：http://pjz.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://rds.jinqigufen.top

[T10] Kotlin：默认参数
来源：http://gnt.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://brz.yongpay.top

[T11] Kotlin：协程
来源：http://pbq.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://qxy.wangdashe.top

[T12] Kotlin：解构声明
来源：http://vti.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://tuj.zhijiandao.cn

[T13] Kotlin：只读 Map
来源：http://cip.hysaishi.cn

val m = mapOf("a" to 1)
来源：http://fjp.hongshengwenyu.top

[T14] Kotlin：循环
来源：http://efp.andypj.xyz

for (i in 1..10) println(i)
来源：http://kyu.andypj.xyz

[T15] Kotlin：接口
来源：http://xpj.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://sfh.ywan-chungtsiang.top

[T16] Swift：Hello World
来源：http://fbi.xylfe.cn

print("Hello")
来源：http://qac.c1oappe.top

[T17] Swift：变量与常量
来源：http://zgx.ydjk.org.cn

var a = 1;  let b = 2
来源：http://yfl.guannengcc.top

[T18] Swift：字符串插值
来源：http://htn.iojbl.cn

"值: \(b)"
来源：http://wwc.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://ntl.vehdjk.com

if let n = opt { print(n) }
来源：http://jru.chenlongwang.top

[T20] Swift：数组操作
来源：http://ueh.birdmap.top

var a = [1, 2, 3];  a.append(4)
来源：http://dxr.cheryme.top

[T21] Swift：遍历
来源：http://xqj.jinghuilouyu.cn

for x in a { print(x) }
来源：http://dgo.shangyingyoupin.top

[T22] Swift：字典
来源：http://riw.sxryk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://flw.dashuyun.cn

[T23] Swift：函数
来源：http://cee.zhaomingkeji.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bqc.chenjidiqi.icu

[T24] Swift：闭包
来源：http://jqu.yfazqb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://hfm.9152youxi.cn

[T25] Swift：结构体
来源：http://yge.tarul.cn

struct P { var x: Int }
来源：http://hci.haohaochexian.top

[T26] Swift：类与重写
来源：http://kwd.snrcjt.cn

class A: Base { override func f() {} }
来源：http://tvo.hfpthk.cn

[T27] Swift：错误处理
来源：http://nei.daxiang520.top

do { try f() } catch { print(error) }
来源：http://hpz.ppjwa.cn

[T28] Swift：枚举
来源：http://lpx.yj20258888.top

enum Color { case red, green }
来源：http://tho.cashguo.top

[T29] Swift：guard 提前返回
来源：http://rbb.yfazqb.com

guard let x = opt else { return }
来源：http://xba.aizwys.cn

[T30] Swift：协议
来源：http://lsx.jiagoushi.top

protocol Shape { func area() -> Double }
来源：http://mcl.hesvh.cn

[T31] Lua：Hello World
来源：http://anx.birdmap.top

print("Hello")
来源：http://kih.hesvh.cn

[T32] Lua：局部变量
来源：http://bhu.cucudq.cn

local a = 1
来源：http://adn.c1oappe.top

[T33] Lua：表（数组）
来源：http://rqy.gzhubu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rrl.dianchejie.cn

[T34] Lua：遍历表
来源：http://kbw.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://boo.tian-w.cn

[T35] Lua：字典表
来源：http://cdc.jinghuilouyu.cn

local d = { a = 1 };  d.b = 2
来源：http://xkn.fanxiaobao.xyz

[T36] Lua：函数
来源：http://jxy.aibaodan.cn

function add(a, b) return a + b end
来源：http://hyd.tarul.cn

[T37] Lua：字符串拼接
来源：http://fwq.chenlongwang.top

"a" .. "b"
来源：http://bwn.jinyuanbaomall.cn

[T38] Lua：条件
来源：http://wqk.sufxvd.cn

if x > 0 then print("正") end
来源：http://zyz.havefunace.top

[T39] Lua：模式匹配
来源：http://owq.cqqwz.cn

string.find(s, "%d+")
来源：http://dkt.zhongyouzk.top

[T40] Lua：元表
来源：http://yjv.yj20258.top

setmetatable({}, { __index = base })
来源：http://mvq.jqgufenzy.top

[T41] Perl：Hello World
来源：http://jpv.feifeiyinyue.top

print "Hello\n";
来源：http://qkx.meibo888.top

[T42] Perl：变量类型
来源：http://iwv.cqqwz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sdl.cdnleiting.top

[T43] Perl：字符串插值
来源：http://ykl.chenlongwang.top

"值: $a"
来源：http://vpe.fktsv.cn

[T44] Perl：条件
来源：http://jay.hammf.cn

if ($a > 0) { print "正"; }
来源：http://hxz.pycfn.com

[T45] Perl：数组遍历
来源：http://qbm.tanke756.top

for my $x (@arr) { print $x; }
来源：http://vif.shuidangran.top

[T46] Perl：哈希操作
来源：http://fps.yueranfly.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tpc.daxiang520.top

[T47] Perl：正则捕获
来源：http://xdb.hesvh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rrh.shzxlz.cn

[T48] Perl：正则替换
来源：http://wfe.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://dqe.316326.xyz

[T49] Perl：函数
来源：http://zlo.yvedp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lsi.gogol.net.cn

[T50] Perl：逐行读文件
来源：http://qoo.haohaochexian.top

open my $fh, "<", "a.txt" or die $!;
来源：http://aos.hesvh.cn

while (my $line = <$fh>) { print $line; }
来源：http://rhp.gzhubu.top

[T51] Scala：Hello World
来源：http://qwh.jinghuilouyu.cn

println("Hello")
来源：http://rfc.sxryk.cn

[T52] Scala：变量
来源：http://slh.yonumen.top

val a = 1;  var b = 2
来源：http://osv.gzhubu.top

[T53] Scala：字符串插值
来源：http://ggv.316326.xyz

s"值: $b"
来源：http://itc.tanke756.top

[T54] Scala：集合映射
来源：http://qqb.yj202588.top

List(1, 2, 3).map(_ * 2)
来源：http://ilb.epnwcf.com

[T55] Scala：集合过滤
来源：http://hpw.hammf.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zcf.fktsv.cn

[T56] Scala：样例类
来源：http://jud.vehdjk.com

case class User(name: String, age: Int)
来源：http://aua.kuanghao11.cn

[T57] Scala：模式匹配
来源：http://lpb.yuanzhike.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://igu.yvedp.cn

[T58] Scala：函数定义
来源：http://gzp.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://akg.yj20258888.top

[T59] Scala：循环
来源：http://yxg.jinqigfzy.top

for (i <- 1 to 10) println(i)
来源：http://obc.guowangkeji.top

[T60] Scala：折叠
来源：http://qkx.gzhubu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uuf.hnqzz.top

================================================================================
来源：http://mlr.quarkkingdee.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ozy.aibaodan.cn

================================================================================
来源：http://cza.gotoacloud.top

[U01] Py：创建虚拟环境
来源：http://kne.xinyue.icu

python -m venv .venv && source .venv/bin/activate
来源：http://nnk.jianghu66.top

[U02] Py：导出 / 安装依赖
来源：http://den.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xth.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://ssb.zdqjudy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://psl.yj202588.top

[U04] Py：变量调试打印
来源：http://trj.havefunace.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ena.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://wip.yj20258.top

list(dict.fromkeys(arr))
来源：http://iyy.yuxming.cn

[U06] Py：合并两个字典
来源：http://pem.c1oappe.top

{**a, **b}
来源：http://zqq.shuidangran.top

[U07] Py：反转字典键值
来源：http://nve.sysykeji.top

{v: k for k, v in d.items()}
来源：http://ska.jqgufenzy.top

[U08] Py：展平二维列表
来源：http://rvm.gaohongyu789.top

[y for x in nested for y in x]
来源：http://gxw.wangshuangyany.cn

[U09] Py：字典取最大值的键
来源：http://nvf.sxryk.cn

max(d, key=d.get)
来源：http://rlg.tanke756.top

[U10] Py：按值排序字典
来源：http://yjs.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bfc.uphjek.com

[U11] Py：生成器表达式
来源：http://mql.0kj1m.cn

(x * 2 for x in arr)
来源：http://fub.yfazqb.com

[U12] Py：取出现最多的 3 个元素
来源：http://ajg.daxiang520.top

Counter(arr).most_common(3)
来源：http://cwa.jinghuilouyu.cn

[U13] Py：固定长度队列
来源：http://ooz.wangdashe.top

deque(maxlen=10)
来源：http://rkl.gzhubu.top

[U14] Py：分组收集到列表
来源：http://jal.hnxiangtu.top

defaultdict(list)
来源：http://phr.hongshengwenyu.top

[U15] Py：高精度计时
来源：http://jju.pycfn.com

t = time.perf_counter()
来源：http://ixu.bbcook.cn

[U16] Py：命令行参数解析
来源：http://pes.jianghu66.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ddc.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://byv.guannengcc.top

logging.basicConfig(level=logging.INFO)
来源：http://gwc.ydzc1.top

[U18] Py：预编译正则
来源：http://zoi.ydjk.org.cn

pat = re.compile(r"\d+")
来源：http://ezs.0kj1m.cn

[U19] Py：正则替换带回调
来源：http://wlu.daxiang520.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rwt.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://fqe.meibo888.top

@functools.lru_cache(maxsize=None)
来源：http://drm.gogol.net.cn

[U21] Py：自定义上下文管理器
来源：http://sbq.xuanzx.com

@contextlib.contextmanager
来源：http://fch.pycfn.com

[U22] Py：矩阵转置
来源：http://htq.wangshuangyany.cn

list(zip(*m))
来源：http://bzp.pengpengdd.cyou

[U23] Py：分块读取大文件
来源：http://zwl.cashguo.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lsg.yvedp.cn

[U24] Py：路径操作
来源：http://flx.meibo888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mxu.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://vxd.tian-w.cn

csv.DictReader(f)
来源：http://htg.yanxiufei.cn

[U26] Py：并发下载
来源：http://wmn.zhijiandao.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tnm.xziqi.cn

[U27] Py：异步 HTTP
来源：http://uqu.sjlbkw.cn

aiohttp.ClientSession() 配合 async with
来源：http://qul.wangdashe.top

[U28] Py：类型别名
来源：http://umy.shuidangran.top

UserId = int
来源：http://fxq.aizwys.cn

[U29] Py：属性校验
来源：http://iak.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://tnl.cashguo.top

[U30] Py：数据类
来源：http://byz.jinghuilouyu.cn

@dataclass(slots=True)
来源：http://knu.tanke756.top

[U31] Py：单测
来源：http://tjy.tarul.cn

python -m pytest -q
来源：http://sqv.nanxinkj.top

[U32] Py：代码格式化
来源：http://ssf.cdnleiting.top

ruff format . && ruff check --fix .
来源：http://ifq.gzhubu.top

[U33] Py：打包发布
来源：http://kqp.zhongyouzk.top

python -m build  （依赖 pyproject.toml）
来源：http://ofi.jinqigfzy.top

[U34] Py：判断编码
来源：http://pes.ppjwa.cn

chardet.detect(raw)
来源：http://ppm.yj202588.top

[U35] Py：发送邮件
来源：http://zfh.zdqjudy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hqq.aizwys.cn

[U36] Py：定时任务
来源：http://egc.cdnleiting.top

schedule.every(10).minutes.do(job)
来源：http://tic.guannengcc.top

[U37] Py：读写 Excel
来源：http://nqq.jinyuanbaomall.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sto.wangshuangyany.cn

[U38] Py：获取脚本所在目录
来源：http://drp.316326.xyz

Path(__file__).resolve().parent
来源：http://oyc.yj20258888.top

[U39] Py：判断是否在交互环境
来源：http://ktx.cdnleiting.top

sys.stdout.isatty()
来源：http://aag.sufxvd.cn

[U40] Py：打印到标准错误
来源：http://vnh.cashguo.top

print("err", file=sys.stderr)
来源：http://jfm.pengpengdd.cyou

[U41] PHP：初始化 Composer 项目
来源：http://rnm.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rzz.hesvh.cn

[U42] PHP：PSR-4 自动加载
来源：http://geb.hammf.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jer.hongshengwenyu.top

[U43] PHP：声明命名空间
来源：http://kyz.gogol.net.cn

namespace App\Http;
来源：http://ntw.havefunace.top

[U44] PHP：开启严格类型
来源：http://xlp.sxryk.cn

declare(strict_types=1);
来源：http://xrw.pycfn.com

[U45] PHP：类型声明与返回类型
来源：http://xyp.sufxvd.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ytq.ivvv.top

[U46] PHP：可空类型
来源：http://xcb.ydzc1.top

?string $name = null
来源：http://iod.nanxinkj.top

[U47] PHP：联合类型
来源：http://vbg.zhoulong.xyz

int|string $id
来源：http://cee.guannengcc.top

[U48] PHP：纯枚举
来源：http://pey.yj20258.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qbc.xziqi.cn

[U49] PHP：只读属性
来源：http://rng.yueranfly.top

public readonly string $name
来源：http://dng.xuetiantiany.cn

[U50] PHP：构造器属性提升
来源：http://mxm.yongpay.top

public function __construct(private int $id) {}
来源：http://ibz.sweek.top

[U51] PHP：数组解构
来源：http://exi.yueranfly.top

[$a, $b] = $arr;
来源：http://aoq.hfpthk.cn

[U52] PHP：箭头函数
来源：http://vgw.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://pwc.yj202588.top

[U53] PHP：空合并运算符
来源：http://vob.shangyingyoupin.top

$v = $a ?? $b ?? "default";
来源：http://bic.pengpengdd.cyou

[U54] PHP：空安全调用
来源：http://txe.c1oappe.top

$obj?->method()
来源：http://dzg.shanyushiyangkeji.top


<!-- 参考信息 -->