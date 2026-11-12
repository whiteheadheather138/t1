代发 wailian999

#ifndef X_H
来源：http://dff.zhoulong.xyz

#define X_H
来源：http://idp.xuetiantiany.cn

#endif
来源：http://tek.shuidangran.top

[S31] C++：Hello World
来源：http://jyq.mhx1999.top

#include <iostream>
来源：http://ztg.hfpthk.cn

int main() { std::cout << "Hello\n"; }
来源：http://xsr.cdnleiting.top

[S32] C++：字符串
来源：http://nqd.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://ehg.daria6918.cn

[S33] C++：vector 增删
来源：http://wqt.tanke756.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mez.yj20258888.top

[S34] C++：遍历 vector
来源：http://qbe.yj20258888.top

for (auto &x : v) { std::cout << x; }
来源：http://uug.jqgfzy.top

[S35] C++：map
来源：http://lzn.yj20258888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nmx.hnxiangtu.top

[S36] C++：unordered_map
来源：http://upu.zhoulong.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://grb.hnqzz.top

[S37] C++：set
来源：http://rjb.yuxming.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://shz.zhiwuduotai.top

[S38] C++：排序
来源：http://psn.xingfuxueyuan.xyz

std::sort(v.begin(), v.end());
来源：http://bbf.ybcxt.top

[S39] C++：自定义比较器排序
来源：http://syn.yvedp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jvj.shuidangran.top

[S40] C++：查找元素
来源：http://ujm.iojbl.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jvh.meibo888.top

[S41] C++：类与构造函数
来源：http://hif.sxryk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jze.tanke756.top

[S42] C++：继承与虚函数
来源：http://uri.birdmap.top

class B : public Base { public: void f() override {} };
来源：http://pdb.ydzc1.top

[S43] C++：智能指针
来源：http://bec.yfazqb.com

auto p = std::make_unique<int>(5);
来源：http://eak.uphjek.com

[S44] C++：引用传参
来源：http://zyk.hfpthk.cn

void inc(int &x) { ++x; }
来源：http://yad.xylfe.cn

[S45] C++：lambda
来源：http://gbt.pycfn.com

auto add = [](int a, int b) { return a + b; };
来源：http://aui.xinyue.icu

[S46] C++：函数模板
来源：http://uui.yj202588.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ett.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://qxo.zycfv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aat.9152youxi.cn

[S48] C++：逐行读文件
来源：http://maq.zdqjudy.top

std::ifstream in("a.txt");  std::string line;
来源：http://yvk.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://qjk.nanxuanxn.top

[S49] C++：写文件
来源：http://zsz.shzxlz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nku.zhijiandao.cn

[S50] C++：格式化数字
来源：http://sgg.52xcode.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://emf.c1oappe.top

[S51] C++：显式类型转换
来源：http://qiy.jiagoushi.top

static_cast<double>(a) / b
来源：http://yxi.tanke756.top

[S52] C++：const 与 noexcept
来源：http://zmu.nwbrower.top

int size() const noexcept { return n_; }
来源：http://ets.nanxuanxn.top

[S53] C++：移动语义
来源：http://wbx.tian-w.cn

std::vector<int> w = std::move(v);
来源：http://kup.fanxiaobao.xyz

[S54] C++：异常处理
来源：http://wab.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uxs.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://izh.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rfb.hongshengwenyu.top

[S56] C++：optional
来源：http://ble.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vyj.daria6918.cn

[S57] C++：编译期常量
来源：http://mjz.wangshuangyany.cn

constexpr int N = 10;
来源：http://skg.ivvv.top

[S58] C++：命名空间
来源：http://myp.shuidangran.top

namespace ns { int f() { return 1; } }
来源：http://yjb.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://kxj.yuxming.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kko.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://hnk.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jzw.redwolf501.top

================================================================================
来源：http://ldc.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vaf.pengpengdd.cyou

================================================================================
来源：http://vqs.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://oua.fktsv.cn

println("Hello")
来源：http://ogw.316326.xyz

[T02] Kotlin：变量
来源：http://two.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bag.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://jax.gzhubu.top

"值: $b"
来源：http://snd.yj20258888.top

[T04] Kotlin：空安全
来源：http://vfw.ydzc1.top

val n: String? = null;  n?.length
来源：http://gux.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://awu.guannengcc.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jce.chenlongwang.top

[T06] Kotlin：集合映射
来源：http://xkg.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tom.zhixingplan.top

[T07] Kotlin：集合过滤
来源：http://xgw.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hrp.0kj1m.cn

[T08] Kotlin：数据类
来源：http://nhh.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://ric.jianghu66.top

[T09] Kotlin：扩展函数
来源：http://ian.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://pyi.ehwqpu.com

[T10] Kotlin：默认参数
来源：http://sfx.guowangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gnj.yonumen.top

[T11] Kotlin：协程
来源：http://fcz.gotoacloud.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://loy.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://nfs.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://cgd.c1oappe.top

[T13] Kotlin：只读 Map
来源：http://uvf.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://fid.hesvh.cn

[T14] Kotlin：循环
来源：http://mlv.yonumen.top

for (i in 1..10) println(i)
来源：http://bas.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://sju.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://xxk.hfpthk.cn

[T16] Swift：Hello World
来源：http://tzg.xuetiantiany.cn

print("Hello")
来源：http://lxh.shuidangran.top

[T17] Swift：变量与常量
来源：http://caj.uphjek.com

var a = 1;  let b = 2
来源：http://sxo.xuanzx.com

[T18] Swift：字符串插值
来源：http://zfl.meibo888.top

"值: \(b)"
来源：http://zov.ydzc1.top

[T19] Swift：可选绑定
来源：http://sqw.nanxinkj.top

if let n = opt { print(n) }
来源：http://bvz.hfpthk.cn

[T20] Swift：数组操作
来源：http://pae.ppjwa.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oys.jinqigufen.top

[T21] Swift：遍历
来源：http://vfp.ybcxt.top

for x in a { print(x) }
来源：http://qsr.epnwcf.com

[T22] Swift：字典
来源：http://duj.hesvh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://izw.aibaodan.cn

[T23] Swift：函数
来源：http://uuh.yuxming.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rve.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://xae.zhaomingkeji.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://aki.vehdjk.com

[T25] Swift：结构体
来源：http://lbz.sysykeji.top

struct P { var x: Int }
来源：http://udd.jinqigfzy.top

[T26] Swift：类与重写
来源：http://ylb.xinyue.icu

class A: Base { override func f() {} }
来源：http://rlz.jqgfzy.top

[T27] Swift：错误处理
来源：http://tjp.hongshengwenyu.top

do { try f() } catch { print(error) }
来源：http://zno.zhaomingkeji.xyz

[T28] Swift：枚举
来源：http://zgd.zhijiandao.cn

enum Color { case red, green }
来源：http://ocu.316326.xyz

[T29] Swift：guard 提前返回
来源：http://gsl.ppjwa.cn

guard let x = opt else { return }
来源：http://tzc.yonumen.top

[T30] Swift：协议
来源：http://dzu.zhiwuduotai.top

protocol Shape { func area() -> Double }
来源：http://emq.uphjek.com

[T31] Lua：Hello World
来源：http://srf.316326.xyz

print("Hello")
来源：http://zyn.redwolf501.top

[T32] Lua：局部变量
来源：http://ikp.xziqi.cn

local a = 1
来源：http://fdq.tianlin.xyz

[T33] Lua：表（数组）
来源：http://isy.chenlongwang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cqu.chenzaomai.com

[T34] Lua：遍历表
来源：http://fyu.cucudq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gmf.nanxinkj.top

[T35] Lua：字典表
来源：http://wag.shanyushiyangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://epy.tanke756.top

[T36] Lua：函数
来源：http://fta.yj202588.top

function add(a, b) return a + b end
来源：http://jmn.dashuyun.cn

[T37] Lua：字符串拼接
来源：http://trb.guowangkeji.top

"a" .. "b"
来源：http://glg.hammf.cn

[T38] Lua：条件
来源：http://qyl.sxryk.cn

if x > 0 then print("正") end
来源：http://ugh.tianlin.xyz

[T39] Lua：模式匹配
来源：http://fmo.vqdsnc.cn

string.find(s, "%d+")
来源：http://qoc.epnwcf.com

[T40] Lua：元表
来源：http://xur.sxryk.cn

setmetatable({}, { __index = base })
来源：http://dbj.snrcjt.cn

[T41] Perl：Hello World
来源：http://vrn.fehbvm.com

print "Hello\n";
来源：http://vck.sufxvd.cn

[T42] Perl：变量类型
来源：http://mca.wangdashe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ane.sysykeji.top

[T43] Perl：字符串插值
来源：http://shp.zdqjudy.top

"值: $a"
来源：http://tzb.nanxuanxn.top

[T44] Perl：条件
来源：http://qqb.redwolf501.top

if ($a > 0) { print "正"; }
来源：http://tza.guowangkeji.top

[T45] Perl：数组遍历
来源：http://aae.redwolf501.top

for my $x (@arr) { print $x; }
来源：http://gil.yuanzhike.top

[T46] Perl：哈希操作
来源：http://ztx.nanxuanxn.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mwh.hcnkem.com

[T47] Perl：正则捕获
来源：http://iqs.sjlbkw.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mhh.xinyue.icu

[T48] Perl：正则替换
来源：http://nnu.guowangkeji.top

$s =~ s/old/new/g;
来源：http://qzy.jinyuanbaomall.cn

[T49] Perl：函数
来源：http://duy.sufxvd.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uyj.jianghu66.top

[T50] Perl：逐行读文件
来源：http://ujc.pengpengdd.cyou

open my $fh, "<", "a.txt" or die $!;
来源：http://koj.sufxvd.cn

while (my $line = <$fh>) { print $line; }
来源：http://fkt.chenzaomai.com

[T51] Scala：Hello World
来源：http://tff.xingfuxueyuan.xyz

println("Hello")
来源：http://fdm.ydzc1.top

[T52] Scala：变量
来源：http://qnt.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://elt.0kj1m.cn

[T53] Scala：字符串插值
来源：http://jge.9152youxi.cn

s"值: $b"
来源：http://fqb.hongshengwenyu.top

[T54] Scala：集合映射
来源：http://xqr.yvedp.cn

List(1, 2, 3).map(_ * 2)
来源：http://coy.cashguo.top

[T55] Scala：集合过滤
来源：http://nxt.hfpthk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ryj.haohaochexian.top

[T56] Scala：样例类
来源：http://fqq.yanxiufei.cn

case class User(name: String, age: Int)
来源：http://vzo.nanxinkj.top

[T57] Scala：模式匹配
来源：http://rsi.9152youxi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://beu.jqgufenzy.top

[T58] Scala：函数定义
来源：http://paf.fanxiaobao.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://bpu.yongpay.top

[T59] Scala：循环
来源：http://unc.tian-w.cn

for (i <- 1 to 10) println(i)
来源：http://ppf.svipenyu.cn

[T60] Scala：折叠
来源：http://byk.xingfuxueyuan.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ifk.aibaodan.cn

================================================================================
来源：http://nmb.zhiwuduotai.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mqe.ppjwa.cn

================================================================================
来源：http://myy.shangyingyoupin.top

[U01] Py：创建虚拟环境
来源：http://xbp.wangdashe.top

python -m venv .venv && source .venv/bin/activate
来源：http://ndn.xingfuxueyuan.xyz

[U02] Py：导出 / 安装依赖
来源：http://sfb.aizwys.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://osm.cashguo.top

[U03] Py：加载 .env 配置
来源：http://uph.quarkkingdee.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ekv.shanyushiyangkeji.top

[U04] Py：变量调试打印
来源：http://cpj.jqgfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dms.bbcook.cn

[U05] Py：列表去重且保序
来源：http://evk.tian-w.cn

list(dict.fromkeys(arr))
来源：http://rnk.guannengcc.top

[U06] Py：合并两个字典
来源：http://jra.wangshuangyany.cn

{**a, **b}
来源：http://mhj.shangyingyoupin.top

[U07] Py：反转字典键值
来源：http://lwj.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://blm.gogol.net.cn

[U08] Py：展平二维列表
来源：http://zos.hnxiangtu.top

[y for x in nested for y in x]
来源：http://qpl.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://gfi.zhiwuduotai.top

max(d, key=d.get)
来源：http://qyh.cqqwz.cn

[U10] Py：按值排序字典
来源：http://qkh.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rcc.fengsongda.top

[U11] Py：生成器表达式
来源：http://ovi.fengsongda.top

(x * 2 for x in arr)
来源：http://msj.iojbl.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ewx.jqgfzy.top

Counter(arr).most_common(3)
来源：http://git.jqgufenzy.top

[U13] Py：固定长度队列
来源：http://ute.ydjk.org.cn

deque(maxlen=10)
来源：http://kjv.yj20258888.top

[U14] Py：分组收集到列表
来源：http://nbh.zycfv.cn

defaultdict(list)
来源：http://ypv.sxryk.cn

[U15] Py：高精度计时
来源：http://fys.mhx1999.top

t = time.perf_counter()
来源：http://jsy.yj20258.top

[U16] Py：命令行参数解析
来源：http://vmj.fktsv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bgu.yangfankeji.com

[U17] Py：初始化日志
来源：http://cjz.ctjpmb.com

logging.basicConfig(level=logging.INFO)
来源：http://onw.tarul.cn

[U18] Py：预编译正则
来源：http://mtv.guowangkeji.top

pat = re.compile(r"\d+")
来源：http://jda.jyoumei.cn

[U19] Py：正则替换带回调
来源：http://zxk.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ckw.havefunace.top

[U20] Py：缓存函数结果
来源：http://gmk.xylfe.cn

@functools.lru_cache(maxsize=None)
来源：http://ppp.daxiang520.top

[U21] Py：自定义上下文管理器
来源：http://yfx.meibo888.top

@contextlib.contextmanager
来源：http://ewe.tianlin.xyz

[U22] Py：矩阵转置
来源：http://yaf.aizwys.cn

list(zip(*m))
来源：http://xrl.yongpay.top

[U23] Py：分块读取大文件
来源：http://lhp.jyoumei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://riv.ywan-chungtsiang.top

[U24] Py：路径操作
来源：http://uwh.aizwys.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://frk.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://avd.aibaodan.cn

csv.DictReader(f)
来源：http://vfl.epnwcf.com

[U26] Py：并发下载
来源：http://xbe.yueranfly.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fhz.smart0.xyz

[U27] Py：异步 HTTP
来源：http://fxm.ivvv.top

aiohttp.ClientSession() 配合 async with
来源：http://yyu.c1oappe.top

[U28] Py：类型别名
来源：http://exf.yuxming.cn

UserId = int
来源：http://okl.hesvh.cn

[U29] Py：属性校验
来源：http://unz.xingfuxueyuan.xyz

@property 与 @x.setter 配合
来源：http://trd.cqqwz.cn

[U30] Py：数据类
来源：http://nhr.jinqigufen.top

@dataclass(slots=True)
来源：http://syb.pycfn.com

[U31] Py：单测
来源：http://moa.meibo888.top

python -m pytest -q
来源：http://cnd.jinghuilouyu.cn

[U32] Py：代码格式化
来源：http://rke.52xcode.cn

ruff format . && ruff check --fix .
来源：http://rkw.meibo888.top

[U33] Py：打包发布
来源：http://bkc.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://lrr.zhijiandao.cn

[U34] Py：判断编码
来源：http://afy.zdbjq.cn

chardet.detect(raw)
来源：http://mnh.fzhhl.top

[U35] Py：发送邮件
来源：http://nce.bbcook.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lfm.xuanzx.com

[U36] Py：定时任务
来源：http://erv.yangfankeji.com

schedule.every(10).minutes.do(job)
来源：http://qln.chenjidiqi.icu

[U37] Py：读写 Excel
来源：http://rci.zhiwuduotai.top

pandas.read_excel / DataFrame.to_excel
来源：http://fzh.tanke756.top

[U38] Py：获取脚本所在目录
来源：http://agr.tanke756.top

Path(__file__).resolve().parent
来源：http://svt.cucudq.cn

[U39] Py：判断是否在交互环境
来源：http://mso.gzhubu.top

sys.stdout.isatty()
来源：http://igf.gogol.net.cn

[U40] Py：打印到标准错误
来源：http://wzb.chenzaomai.com

print("err", file=sys.stderr)
来源：http://aka.hammf.cn

[U41] PHP：初始化 Composer 项目
来源：http://hxc.ctjpmb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://ggg.andypj.xyz

[U42] PHP：PSR-4 自动加载
来源：http://tpl.shanyushiyangtech.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jxl.316326.xyz

[U43] PHP：声明命名空间
来源：http://ycu.pycfn.com

namespace App\Http;
来源：http://ipt.birdmap.top

[U44] PHP：开启严格类型
来源：http://gye.c1oappe.top

declare(strict_types=1);
来源：http://epp.cashguo.top

[U45] PHP：类型声明与返回类型
来源：http://vqw.vqdsnc.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rzn.zhaomingkeji.xyz

[U46] PHP：可空类型
来源：http://oqs.zhixingplan.top

?string $name = null
来源：http://uci.jyoumei.cn

[U47] PHP：联合类型
来源：http://hou.0kj1m.cn

int|string $id
来源：http://ouc.yj202588.top

[U48] PHP：纯枚举
来源：http://xnl.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hoe.fengsongda.top

[U49] PHP：只读属性
来源：http://swg.fehbvm.com

public readonly string $name
来源：http://gey.guowangkeji.top

[U50] PHP：构造器属性提升
来源：http://ysb.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://img.ppjwa.cn

[U51] PHP：数组解构
来源：http://hqy.gaohongyu789.top

[$a, $b] = $arr;
来源：http://hko.shzxlz.cn

[U52] PHP：箭头函数
来源：http://iza.zhiwuduotai.top

$double = fn($x) => $x * 2;
来源：http://urq.nanxuanxn.top

[U53] PHP：空合并运算符
来源：http://jbo.vehdjk.com

$v = $a ?? $b ?? "default";
来源：http://iqh.tanke756.top

[U54] PHP：空安全调用
来源：http://bmu.bjfxy.top

$obj?->method()
来源：http://qjq.andypj.xyz


<!-- 参考信息 -->