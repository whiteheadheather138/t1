代发 wailian999

#ifndef X_H
来源：http://ids.yanxiufei.cn

#define X_H
来源：http://xwh.vehdjk.com

#endif
来源：http://tve.yangfankeji.com

[S31] C++：Hello World
来源：http://umy.xylfe.cn

#include <iostream>
来源：http://vik.sjlbkw.cn

int main() { std::cout << "Hello\n"; }
来源：http://vpf.zhongyouzk.top

[S32] C++：字符串
来源：http://qcu.yongpay.top

std::string s = "hi";  s += "!";
来源：http://tot.fengsongda.top

[S33] C++：vector 增删
来源：http://vpz.hcnkem.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tes.cashguo.top

[S34] C++：遍历 vector
来源：http://cgn.bjfxy.top

for (auto &x : v) { std::cout << x; }
来源：http://qiz.fanxiaobao.xyz

[S35] C++：map
来源：http://urz.mhx1999.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://thx.9152youxi.cn

[S36] C++：unordered_map
来源：http://vmf.zhiwuduotai.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://enp.nwbrower.top

[S37] C++：set
来源：http://rlv.gogol.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cqq.hnxiangtu.top

[S38] C++：排序
来源：http://tdn.sweek.top

std::sort(v.begin(), v.end());
来源：http://cci.yangfankeji.com

[S39] C++：自定义比较器排序
来源：http://pvc.xuanzx.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xcv.jqgufenzy.top

[S40] C++：查找元素
来源：http://oes.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nai.aizwys.cn

[S41] C++：类与构造函数
来源：http://zmo.316326.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kzu.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://pvf.yj20258888.top

class B : public Base { public: void f() override {} };
来源：http://qjn.zdqjudy.top

[S43] C++：智能指针
来源：http://dfo.nanxinkj.top

auto p = std::make_unique<int>(5);
来源：http://zkw.yonumen.top

[S44] C++：引用传参
来源：http://kvl.gaohongyu789.top

void inc(int &x) { ++x; }
来源：http://uxx.daxiang520.top

[S45] C++：lambda
来源：http://ljh.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pdr.zdbjq.cn

[S46] C++：函数模板
来源：http://jlj.shuidangran.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ndi.dashuyun.cn

[S47] C++：结构化绑定遍历
来源：http://mim.hammf.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://elz.snrcjt.cn

[S48] C++：逐行读文件
来源：http://une.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://yxs.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://fly.smart0.xyz

[S49] C++：写文件
来源：http://hdc.fzhhl.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zmz.havefunace.top

[S50] C++：格式化数字
来源：http://qpq.xinyue.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mfp.jianghu66.top

[S51] C++：显式类型转换
来源：http://gja.cucudq.cn

static_cast<double>(a) / b
来源：http://ktb.yvedp.cn

[S52] C++：const 与 noexcept
来源：http://ybn.xziqi.cn

int size() const noexcept { return n_; }
来源：http://cdz.cashguo.top

[S53] C++：移动语义
来源：http://xdd.hesvh.cn

std::vector<int> w = std::move(v);
来源：http://ioc.sjlbkw.cn

[S54] C++：异常处理
来源：http://vpa.aibaodan.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://deu.gogol.net.cn

[S55] C++：结构化绑定
来源：http://deq.ctjpmb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://kcp.iojbl.cn

[S56] C++：optional
来源：http://qfj.fktsv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gmw.52xcode.cn

[S57] C++：编译期常量
来源：http://fhm.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://vni.sweek.top

[S58] C++：命名空间
来源：http://sse.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://qow.yangfankeji.com

[S59] C++：静态断言
来源：http://all.c1oappe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dwa.tarul.cn

[S60] C++：遍历并删除元素
来源：http://znh.dianchejie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yjx.tanke756.top

================================================================================
来源：http://vhy.shanyushiyangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dwc.uphjek.com

================================================================================
来源：http://azj.cqqwz.cn

[T01] Kotlin：Hello World
来源：http://kto.wangshuangyany.cn

println("Hello")
来源：http://wwg.hcnkem.com

[T02] Kotlin：变量
来源：http://kee.yj202588.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hcq.tarul.cn

[T03] Kotlin：字符串模板
来源：http://lct.zhiwuduotai.top

"值: $b"
来源：http://unz.hysaishi.cn

[T04] Kotlin：空安全
来源：http://vfv.shzxlz.cn

val n: String? = null;  n?.length
来源：http://jxx.fanxiaobao.xyz

[T05] Kotlin：when 表达式
来源：http://ysn.sysykeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vvf.pycfn.com

[T06] Kotlin：集合映射
来源：http://cbj.ydzc1.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bdu.vehdjk.com

[T07] Kotlin：集合过滤
来源：http://men.epnwcf.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://oat.xuetiantiany.cn

[T08] Kotlin：数据类
来源：http://ztb.ehwqpu.com

data class User(val name: String, val age: Int)
来源：http://eai.jinyuanbaomall.cn

[T09] Kotlin：扩展函数
来源：http://pmq.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://xtr.bbcook.cn

[T10] Kotlin：默认参数
来源：http://joa.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zpz.vehdjk.com

[T11] Kotlin：协程
来源：http://jzb.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://twz.snrcjt.cn

[T12] Kotlin：解构声明
来源：http://mjk.zhiwuduotai.top

val (a, b) = Pair(1, 2)
来源：http://lca.zdbjq.cn

[T13] Kotlin：只读 Map
来源：http://alb.havefunace.top

val m = mapOf("a" to 1)
来源：http://sgm.havefunace.top

[T14] Kotlin：循环
来源：http://rkl.yj202588.top

for (i in 1..10) println(i)
来源：http://bjc.cqqwz.cn

[T15] Kotlin：接口
来源：http://ucd.pengpengdd.cyou

interface Shape { fun area(): Double }
来源：http://rfl.uphjek.com

[T16] Swift：Hello World
来源：http://ymp.chenjidiqi.icu

print("Hello")
来源：http://khu.sxryk.cn

[T17] Swift：变量与常量
来源：http://fym.zycfv.cn

var a = 1;  let b = 2
来源：http://qst.yueranfly.top

[T18] Swift：字符串插值
来源：http://zyu.hnxiangtu.top

"值: \(b)"
来源：http://ghn.gotoacloud.top

[T19] Swift：可选绑定
来源：http://pyc.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://wvf.xuetiantiany.cn

[T20] Swift：数组操作
来源：http://nkh.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://nmj.shanyushiyangtech.top

[T21] Swift：遍历
来源：http://opb.havefunace.top

for x in a { print(x) }
来源：http://rvs.ctjpmb.com

[T22] Swift：字典
来源：http://tno.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://prb.cheryme.top

[T23] Swift：函数
来源：http://fkq.yangfankeji.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mlf.fengsongda.top

[T24] Swift：闭包
来源：http://etu.nwbrower.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dew.aizwys.cn

[T25] Swift：结构体
来源：http://xan.shzxlz.cn

struct P { var x: Int }
来源：http://pnr.redwolf501.top

[T26] Swift：类与重写
来源：http://acp.xylfe.cn

class A: Base { override func f() {} }
来源：http://qlw.hcnkem.com

[T27] Swift：错误处理
来源：http://ona.gaohongyu789.top

do { try f() } catch { print(error) }
来源：http://hhw.pycfn.com

[T28] Swift：枚举
来源：http://hhf.zhoulong.xyz

enum Color { case red, green }
来源：http://jhb.hammf.cn

[T29] Swift：guard 提前返回
来源：http://gav.smart0.xyz

guard let x = opt else { return }
来源：http://erp.cucudq.cn

[T30] Swift：协议
来源：http://yoj.ctjpmb.com

protocol Shape { func area() -> Double }
来源：http://swm.snrcjt.cn

[T31] Lua：Hello World
来源：http://xmz.jinqigufen.top

print("Hello")
来源：http://con.fzhhl.top

[T32] Lua：局部变量
来源：http://ksy.ydzc1.top

local a = 1
来源：http://vdx.ydzc1.top

[T33] Lua：表（数组）
来源：http://ejs.quarkkingdee.top

local t = {1, 2, 3};  t[4] = 4
来源：http://srj.hywenlv.cn

[T34] Lua：遍历表
来源：http://rpy.jinyuanbaomall.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jyk.xingfuxueyuan.xyz

[T35] Lua：字典表
来源：http://tof.ybcxt.top

local d = { a = 1 };  d.b = 2
来源：http://upq.fanxiaobao.xyz

[T36] Lua：函数
来源：http://ezf.fanxiaobao.xyz

function add(a, b) return a + b end
来源：http://lis.feifeiyinyue.top

[T37] Lua：字符串拼接
来源：http://gwb.yangfankeji.com

"a" .. "b"
来源：http://mcb.fktsv.cn

[T38] Lua：条件
来源：http://qjq.tian-w.cn

if x > 0 then print("正") end
来源：http://wzs.shzxlz.cn

[T39] Lua：模式匹配
来源：http://zlz.gogol.net.cn

string.find(s, "%d+")
来源：http://cbu.nanxinkj.top

[T40] Lua：元表
来源：http://fpf.zhaomingkeji.xyz

setmetatable({}, { __index = base })
来源：http://thb.hysaishi.cn

[T41] Perl：Hello World
来源：http://aeq.xuetiantiany.cn

print "Hello\n";
来源：http://cgt.hammf.cn

[T42] Perl：变量类型
来源：http://rhj.jyoumei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ihx.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://vsy.yanxiufei.cn

"值: $a"
来源：http://wun.bbcook.cn

[T44] Perl：条件
来源：http://sir.ybcxt.top

if ($a > 0) { print "正"; }
来源：http://yow.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://vyo.sysykeji.top

for my $x (@arr) { print $x; }
来源：http://oaz.xylfe.cn

[T46] Perl：哈希操作
来源：http://tah.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uua.ctjpmb.com

[T47] Perl：正则捕获
来源：http://uub.tian-w.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wkx.sjlbkw.cn

[T48] Perl：正则替换
来源：http://trc.jianghu66.top

$s =~ s/old/new/g;
来源：http://ngw.uphjek.com

[T49] Perl：函数
来源：http://ygi.jinyuanbaomall.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yup.cheryme.top

[T50] Perl：逐行读文件
来源：http://oen.zhijiandao.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mcg.yueranfly.top

while (my $line = <$fh>) { print $line; }
来源：http://yen.vqdsnc.cn

[T51] Scala：Hello World
来源：http://xyb.gogol.net.cn

println("Hello")
来源：http://icp.c1oappe.top

[T52] Scala：变量
来源：http://wuu.hnqzz.top

val a = 1;  var b = 2
来源：http://wuo.zdqjudy.top

[T53] Scala：字符串插值
来源：http://vus.ivvv.top

s"值: $b"
来源：http://qxj.vehdjk.com

[T54] Scala：集合映射
来源：http://was.xuanzx.com

List(1, 2, 3).map(_ * 2)
来源：http://fmw.ivvv.top

[T55] Scala：集合过滤
来源：http://ojb.redwolf501.top

List(1, 2, 3).filter(_ > 1)
来源：http://xjx.cdnleiting.top

[T56] Scala：样例类
来源：http://uwp.fehbvm.com

case class User(name: String, age: Int)
来源：http://qyd.bbcook.cn

[T57] Scala：模式匹配
来源：http://ker.fengsongda.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dwr.chenlongwang.top

[T58] Scala：函数定义
来源：http://nsh.jinqigufen.top

def add(a: Int, b: Int): Int = a + b
来源：http://nja.daria6918.cn

[T59] Scala：循环
来源：http://wza.ydzc1.top

for (i <- 1 to 10) println(i)
来源：http://qkw.chenjidiqi.icu

[T60] Scala：折叠
来源：http://ctu.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cbp.daria6918.cn

================================================================================
来源：http://dqp.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ugd.guowangkeji.top

================================================================================
来源：http://nbf.316326.xyz

[U01] Py：创建虚拟环境
来源：http://czr.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://aev.sysykeji.top

[U02] Py：导出 / 安装依赖
来源：http://rlk.wangshuangyany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lph.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://vld.jinyuanbaomall.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://znf.ywan-chungtsiang.top

[U04] Py：变量调试打印
来源：http://uhw.ppjwa.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rab.yuxming.cn

[U05] Py：列表去重且保序
来源：http://kls.kuanghao11.cn

list(dict.fromkeys(arr))
来源：http://cam.yonumen.top

[U06] Py：合并两个字典
来源：http://hdf.hesvh.cn

{**a, **b}
来源：http://tpo.shzxlz.cn

[U07] Py：反转字典键值
来源：http://hal.yj202588.top

{v: k for k, v in d.items()}
来源：http://afp.vqdsnc.cn

[U08] Py：展平二维列表
来源：http://lmv.snrcjt.cn

[y for x in nested for y in x]
来源：http://kmz.pycfn.com

[U09] Py：字典取最大值的键
来源：http://pyn.nwbrower.top

max(d, key=d.get)
来源：http://phs.cdnleiting.top

[U10] Py：按值排序字典
来源：http://zdz.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cjz.zdbjq.cn

[U11] Py：生成器表达式
来源：http://kqz.ydzc1.top

(x * 2 for x in arr)
来源：http://uju.sysykeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://eed.xingfuxueyuan.xyz

Counter(arr).most_common(3)
来源：http://fsh.hfpthk.cn

[U13] Py：固定长度队列
来源：http://hfq.yvedp.cn

deque(maxlen=10)
来源：http://qsq.snrcjt.cn

[U14] Py：分组收集到列表
来源：http://uoz.bbcook.cn

defaultdict(list)
来源：http://dnt.jqgufenzy.top

[U15] Py：高精度计时
来源：http://ide.9152youxi.cn

t = time.perf_counter()
来源：http://kvs.jianghu66.top

[U16] Py：命令行参数解析
来源：http://fil.hesvh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vnt.dianchejie.cn

[U17] Py：初始化日志
来源：http://hpz.hammf.cn

logging.basicConfig(level=logging.INFO)
来源：http://vmz.smart0.xyz

[U18] Py：预编译正则
来源：http://jga.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://eic.zdbjq.cn

[U19] Py：正则替换带回调
来源：http://crt.jinyuanbaomall.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kti.aibaodan.cn

[U20] Py：缓存函数结果
来源：http://uty.haohaochexian.top

@functools.lru_cache(maxsize=None)
来源：http://tyo.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://chy.chenzaomai.com

@contextlib.contextmanager
来源：http://dym.xinyue.icu

[U22] Py：矩阵转置
来源：http://xkb.fanxiaobao.xyz

list(zip(*m))
来源：http://mnq.bbcook.cn

[U23] Py：分块读取大文件
来源：http://nzv.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hmw.shanyushiyangtech.top

[U24] Py：路径操作
来源：http://wlr.0kj1m.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uyx.zhongyouzk.top

[U25] Py：CSV 按字典读
来源：http://zgs.aizwys.cn

csv.DictReader(f)
来源：http://nfd.52xcode.cn

[U26] Py：并发下载
来源：http://byu.0kj1m.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uyw.sysykeji.top

[U27] Py：异步 HTTP
来源：http://vap.aizwys.cn

aiohttp.ClientSession() 配合 async with
来源：http://qyw.nanxuanxn.top

[U28] Py：类型别名
来源：http://dhx.jiagoushi.top

UserId = int
来源：http://ehm.wangshuangyany.cn

[U29] Py：属性校验
来源：http://zus.fehbvm.com

@property 与 @x.setter 配合
来源：http://hxs.kuanghao11.cn

[U30] Py：数据类
来源：http://fpa.quarkkingdee.top

@dataclass(slots=True)
来源：http://fdr.shangyingyoupin.top

[U31] Py：单测
来源：http://dvj.daria6918.cn

python -m pytest -q
来源：http://vvr.yvedp.cn

[U32] Py：代码格式化
来源：http://wpx.jinyuanbaomall.cn

ruff format . && ruff check --fix .
来源：http://hyr.feifeiyinyue.top

[U33] Py：打包发布
来源：http://cgo.xuanzx.com

python -m build  （依赖 pyproject.toml）
来源：http://zwl.yongpay.top

[U34] Py：判断编码
来源：http://aan.ybcxt.top

chardet.detect(raw)
来源：http://pxt.jianghu66.top

[U35] Py：发送邮件
来源：http://yrj.daxiang520.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://acq.sweek.top

[U36] Py：定时任务
来源：http://lfb.nwbrower.top

schedule.every(10).minutes.do(job)
来源：http://hnb.smart0.xyz

[U37] Py：读写 Excel
来源：http://rzr.gogol.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jsh.0kj1m.cn

[U38] Py：获取脚本所在目录
来源：http://mqx.meibo888.top

Path(__file__).resolve().parent
来源：http://kbd.jinqigfzy.top

[U39] Py：判断是否在交互环境
来源：http://clf.dashuyun.cn

sys.stdout.isatty()
来源：http://rqp.dianchejie.cn

[U40] Py：打印到标准错误
来源：http://dhx.havefunace.top

print("err", file=sys.stderr)
来源：http://vfw.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://tzm.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jjs.haohaochexian.top

[U42] PHP：PSR-4 自动加载
来源：http://phd.9152youxi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mya.hysaishi.cn

[U43] PHP：声明命名空间
来源：http://kiu.yuanzhike.top

namespace App\Http;
来源：http://bju.ywan-chungtsiang.top

[U44] PHP：开启严格类型
来源：http://bpc.xinyue.icu

declare(strict_types=1);
来源：http://bny.sjlbkw.cn

[U45] PHP：类型声明与返回类型
来源：http://ncy.tian-w.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wqy.guannengcc.top

[U46] PHP：可空类型
来源：http://hzb.quarkkingdee.top

?string $name = null
来源：http://waa.chenjidiqi.icu

[U47] PHP：联合类型
来源：http://urv.gzhubu.top

int|string $id
来源：http://pkq.hnxiangtu.top

[U48] PHP：纯枚举
来源：http://llu.hcnkem.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zck.zdqjudy.top

[U49] PHP：只读属性
来源：http://dkr.chenzaomai.com

public readonly string $name
来源：http://ivf.kuanghao11.cn

[U50] PHP：构造器属性提升
来源：http://rob.sxryk.cn

public function __construct(private int $id) {}
来源：http://cvh.sysykeji.top

[U51] PHP：数组解构
来源：http://rzy.uphjek.com

[$a, $b] = $arr;
来源：http://mly.gogol.net.cn

[U52] PHP：箭头函数
来源：http://ulm.jianghu66.top

$double = fn($x) => $x * 2;
来源：http://xnq.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://tfx.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://apd.yj20258888.top

[U54] PHP：空安全调用
来源：http://xbl.guowangkeji.top

$obj?->method()
来源：http://cxe.hammf.cn


<!-- 参考信息 -->