代发 wailian999

#ifndef X_H
来源：http://wvy.kuanghao11.cn

#define X_H
来源：http://yzi.yangfankeji.com

#endif
来源：http://mnh.ctjpmb.com

[S31] C++：Hello World
来源：http://chf.mhx1999.top

#include <iostream>
来源：http://ste.xuetiantiany.cn

int main() { std::cout << "Hello\n"; }
来源：http://upn.jianghu66.top

[S32] C++：字符串
来源：http://dti.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://xjw.xinyue.icu

[S33] C++：vector 增删
来源：http://yoe.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wuo.xylfe.cn

[S34] C++：遍历 vector
来源：http://daa.yonumen.top

for (auto &x : v) { std::cout << x; }
来源：http://qak.chenzaomai.com

[S35] C++：map
来源：http://exh.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://czy.xuanzx.com

[S36] C++：unordered_map
来源：http://etf.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wgl.chenlongwang.top

[S37] C++：set
来源：http://olp.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kqx.yfazqb.com

[S38] C++：排序
来源：http://zhk.yonumen.top

std::sort(v.begin(), v.end());
来源：http://igt.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://bnk.zdbjq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lqq.pycfn.com

[S40] C++：查找元素
来源：http://trj.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mxf.shanyushiyangkeji.top

[S41] C++：类与构造函数
来源：http://noy.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ljc.cucudq.cn

[S42] C++：继承与虚函数
来源：http://ckq.316326.xyz

class B : public Base { public: void f() override {} };
来源：http://las.xingfuxueyuan.xyz

[S43] C++：智能指针
来源：http://nba.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://mvb.zycfv.cn

[S44] C++：引用传参
来源：http://wfo.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://jel.fktsv.cn

[S45] C++：lambda
来源：http://ksx.daria6918.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nht.wangshuangyany.cn

[S46] C++：函数模板
来源：http://yrp.sweek.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kvs.yj20258888.top

[S47] C++：结构化绑定遍历
来源：http://bar.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wfl.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://jvv.tanke756.top

std::ifstream in("a.txt");  std::string line;
来源：http://xqo.tanke756.top

while (std::getline(in, line)) { }
来源：http://soz.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://qyh.chenzaomai.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ofp.hammf.cn

[S50] C++：格式化数字
来源：http://afp.vqdsnc.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bpy.nanxinkj.top

[S51] C++：显式类型转换
来源：http://cic.smart0.xyz

static_cast<double>(a) / b
来源：http://vmh.mhx1999.top

[S52] C++：const 与 noexcept
来源：http://mmt.hnqzz.top

int size() const noexcept { return n_; }
来源：http://dkh.dianchejie.cn

[S53] C++：移动语义
来源：http://pxf.yonumen.top

std::vector<int> w = std::move(v);
来源：http://jfg.havefunace.top

[S54] C++：异常处理
来源：http://stl.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://phd.gzhubu.top

[S55] C++：结构化绑定
来源：http://wjv.yanxiufei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jqh.shzxlz.cn

[S56] C++：optional
来源：http://swi.dashuyun.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sxo.ppjwa.cn

[S57] C++：编译期常量
来源：http://xiu.yangfankeji.com

constexpr int N = 10;
来源：http://wsr.hammf.cn

[S58] C++：命名空间
来源：http://nob.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://wvg.tanke756.top

[S59] C++：静态断言
来源：http://xrh.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://obe.zycfv.cn

[S60] C++：遍历并删除元素
来源：http://qry.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gnd.fzhhl.top

================================================================================
来源：http://sjj.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vew.bjfxy.top

================================================================================
来源：http://npn.yj20258.top

[T01] Kotlin：Hello World
来源：http://mjc.gaohongyu789.top

println("Hello")
来源：http://pqo.yueranfly.top

[T02] Kotlin：变量
来源：http://gww.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://btw.zdbjq.cn

[T03] Kotlin：字符串模板
来源：http://kak.xuanzx.com

"值: $b"
来源：http://lgp.ctjpmb.com

[T04] Kotlin：空安全
来源：http://kxs.jinqigufen.top

val n: String? = null;  n?.length
来源：http://rxk.svipenyu.cn

[T05] Kotlin：when 表达式
来源：http://vwl.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wrl.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://wwp.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://auq.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://qun.tianlin.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://nmt.hfpthk.cn

[T08] Kotlin：数据类
来源：http://hjy.havefunace.top

data class User(val name: String, val age: Int)
来源：http://eqf.hysaishi.cn

[T09] Kotlin：扩展函数
来源：http://ram.xuanzx.com

fun String.exclaim() = this + "!"
来源：http://gya.jlsjyb.cn

[T10] Kotlin：默认参数
来源：http://jri.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://xfx.xuetiantiany.cn

[T11] Kotlin：协程
来源：http://dot.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vwz.sufxvd.cn

[T12] Kotlin：解构声明
来源：http://xkj.gaohongyu789.top

val (a, b) = Pair(1, 2)
来源：http://set.fanxiaobao.xyz

[T13] Kotlin：只读 Map
来源：http://lfn.jlsjyb.cn

val m = mapOf("a" to 1)
来源：http://zvh.dianchejie.cn

[T14] Kotlin：循环
来源：http://gcj.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://sfq.jinqigfzy.top

[T15] Kotlin：接口
来源：http://umb.vqdsnc.cn

interface Shape { fun area(): Double }
来源：http://jdd.hywenlv.cn

[T16] Swift：Hello World
来源：http://bwv.cheryme.top

print("Hello")
来源：http://che.jinqigfzy.top

[T17] Swift：变量与常量
来源：http://uch.iojbl.cn

var a = 1;  let b = 2
来源：http://vfh.cucudq.cn

[T18] Swift：字符串插值
来源：http://agg.birdmap.top

"值: \(b)"
来源：http://tay.fzhhl.top

[T19] Swift：可选绑定
来源：http://tuz.fanxiaobao.xyz

if let n = opt { print(n) }
来源：http://tfh.xuanzx.com

[T20] Swift：数组操作
来源：http://kok.shangyingyoupin.top

var a = [1, 2, 3];  a.append(4)
来源：http://gnf.jinyuanbaomall.cn

[T21] Swift：遍历
来源：http://hpp.hesvh.cn

for x in a { print(x) }
来源：http://rqo.xuetiantiany.cn

[T22] Swift：字典
来源：http://meo.yanxiufei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zyg.meibo888.top

[T23] Swift：函数
来源：http://dvd.daxiang520.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nek.xylfe.cn

[T24] Swift：闭包
来源：http://xqa.cqqwz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rdu.meibo888.top

[T25] Swift：结构体
来源：http://otw.ppjwa.cn

struct P { var x: Int }
来源：http://emr.yvedp.cn

[T26] Swift：类与重写
来源：http://npy.feifeiyinyue.top

class A: Base { override func f() {} }
来源：http://luv.xylfe.cn

[T27] Swift：错误处理
来源：http://zln.nwbrower.top

do { try f() } catch { print(error) }
来源：http://qwo.sufxvd.cn

[T28] Swift：枚举
来源：http://mcd.xinyue.icu

enum Color { case red, green }
来源：http://mou.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://tno.jinqigufen.top

guard let x = opt else { return }
来源：http://hqs.daria6918.cn

[T30] Swift：协议
来源：http://vhy.jinqigufen.top

protocol Shape { func area() -> Double }
来源：http://xla.yongpay.top

[T31] Lua：Hello World
来源：http://rjt.xuanzx.com

print("Hello")
来源：http://lnc.zycfv.cn

[T32] Lua：局部变量
来源：http://usn.jiagoushi.top

local a = 1
来源：http://txw.zhijiandao.cn

[T33] Lua：表（数组）
来源：http://tmu.hysaishi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zsp.aibaodan.cn

[T34] Lua：遍历表
来源：http://bar.sufxvd.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jrl.jqgufenzy.top

[T35] Lua：字典表
来源：http://nse.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://rjq.epnwcf.com

[T36] Lua：函数
来源：http://bgb.fzhhl.top

function add(a, b) return a + b end
来源：http://dgi.xuetiantiany.cn

[T37] Lua：字符串拼接
来源：http://hvv.jqgfzy.top

"a" .. "b"
来源：http://aut.yfazqb.com

[T38] Lua：条件
来源：http://laf.daxiang520.top

if x > 0 then print("正") end
来源：http://qjg.yonumen.top

[T39] Lua：模式匹配
来源：http://elg.jianghu66.top

string.find(s, "%d+")
来源：http://urc.quarkkingdee.top

[T40] Lua：元表
来源：http://bvr.fktsv.cn

setmetatable({}, { __index = base })
来源：http://evc.c1oappe.top

[T41] Perl：Hello World
来源：http://aqu.zhiwuduotai.top

print "Hello\n";
来源：http://hjj.ppjwa.cn

[T42] Perl：变量类型
来源：http://lmh.yonumen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hvx.chenjidiqi.icu

[T43] Perl：字符串插值
来源：http://vkc.snrcjt.cn

"值: $a"
来源：http://pfw.hcnkem.com

[T44] Perl：条件
来源：http://qrd.ydjk.org.cn

if ($a > 0) { print "正"; }
来源：http://fux.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://aig.hesvh.cn

for my $x (@arr) { print $x; }
来源：http://okj.fehbvm.com

[T46] Perl：哈希操作
来源：http://gcz.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://llt.zhiwuduotai.top

[T47] Perl：正则捕获
来源：http://ccm.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yzj.andypj.xyz

[T48] Perl：正则替换
来源：http://ort.xuanzx.com

$s =~ s/old/new/g;
来源：http://gpa.shanyushiyangkeji.top

[T49] Perl：函数
来源：http://zxc.snrcjt.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ras.aizwys.cn

[T50] Perl：逐行读文件
来源：http://bwl.xingfuxueyuan.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://bsq.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://smk.zycfv.cn

[T51] Scala：Hello World
来源：http://oor.jinqigufen.top

println("Hello")
来源：http://zzp.xinyue.icu

[T52] Scala：变量
来源：http://gjz.ehwqpu.com

val a = 1;  var b = 2
来源：http://chb.kuanghao11.cn

[T53] Scala：字符串插值
来源：http://fuw.zhijiandao.cn

s"值: $b"
来源：http://yfs.chenzaomai.com

[T54] Scala：集合映射
来源：http://tfm.tanke756.top

List(1, 2, 3).map(_ * 2)
来源：http://oco.yangfankeji.com

[T55] Scala：集合过滤
来源：http://acj.52xcode.cn

List(1, 2, 3).filter(_ > 1)
来源：http://npo.chenjidiqi.icu

[T56] Scala：样例类
来源：http://bon.wangshuangyany.cn

case class User(name: String, age: Int)
来源：http://feq.vehdjk.com

[T57] Scala：模式匹配
来源：http://gwh.feifeiyinyue.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sxk.52xcode.cn

[T58] Scala：函数定义
来源：http://qka.xylfe.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cfr.yuanzhike.top

[T59] Scala：循环
来源：http://vre.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://pkw.sufxvd.cn

[T60] Scala：折叠
来源：http://dtq.jinqigfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iss.ybcxt.top

================================================================================
来源：http://rkx.yfazqb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mim.yonumen.top

================================================================================
来源：http://flv.hesvh.cn

[U01] Py：创建虚拟环境
来源：http://xpu.xziqi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tdh.chenzaomai.com

[U02] Py：导出 / 安装依赖
来源：http://hav.ybcxt.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qmi.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://xot.dianchejie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wot.zhengqikj.top

[U04] Py：变量调试打印
来源：http://dso.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tjd.ywan-chungtsiang.top

[U05] Py：列表去重且保序
来源：http://zuf.svipenyu.cn

list(dict.fromkeys(arr))
来源：http://hdh.birdmap.top

[U06] Py：合并两个字典
来源：http://zxq.fengsongda.top

{**a, **b}
来源：http://gpq.wangdashe.top

[U07] Py：反转字典键值
来源：http://yqm.tarul.cn

{v: k for k, v in d.items()}
来源：http://xko.daxiang520.top

[U08] Py：展平二维列表
来源：http://jmf.sxryk.cn

[y for x in nested for y in x]
来源：http://roh.ppjwa.cn

[U09] Py：字典取最大值的键
来源：http://vta.meibo888.top

max(d, key=d.get)
来源：http://ykh.tanke756.top

[U10] Py：按值排序字典
来源：http://gqw.gzhubu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cmd.xingfuxueyuan.xyz

[U11] Py：生成器表达式
来源：http://xkf.hnxiangtu.top

(x * 2 for x in arr)
来源：http://cko.uphjek.com

[U12] Py：取出现最多的 3 个元素
来源：http://ycj.shanyushiyangkeji.top

Counter(arr).most_common(3)
来源：http://xtz.jiagoushi.top

[U13] Py：固定长度队列
来源：http://yxf.ybcxt.top

deque(maxlen=10)
来源：http://wfg.snrcjt.cn

[U14] Py：分组收集到列表
来源：http://wyt.hysaishi.cn

defaultdict(list)
来源：http://jam.yj202588.top

[U15] Py：高精度计时
来源：http://xhq.jianghu66.top

t = time.perf_counter()
来源：http://xsr.jianghu66.top

[U16] Py：命令行参数解析
来源：http://vqt.jyoumei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kde.yanxiufei.cn

[U17] Py：初始化日志
来源：http://qtx.jqgfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://wdn.cashguo.top

[U18] Py：预编译正则
来源：http://clb.sweek.top

pat = re.compile(r"\d+")
来源：http://tya.epnwcf.com

[U19] Py：正则替换带回调
来源：http://fio.yanxiufei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rdl.xylfe.cn

[U20] Py：缓存函数结果
来源：http://ftf.tian-w.cn

@functools.lru_cache(maxsize=None)
来源：http://hgk.yvedp.cn

[U21] Py：自定义上下文管理器
来源：http://hms.dianchejie.cn

@contextlib.contextmanager
来源：http://yje.chenzaomai.com

[U22] Py：矩阵转置
来源：http://say.c1oappe.top

list(zip(*m))
来源：http://dxt.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://gwe.mhx1999.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cuy.uphjek.com

[U24] Py：路径操作
来源：http://max.ydjk.org.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cfs.hnxiangtu.top

[U25] Py：CSV 按字典读
来源：http://pbl.svipenyu.cn

csv.DictReader(f)
来源：http://jjr.zhiwuduotai.top

[U26] Py：并发下载
来源：http://vah.shuidangran.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://say.tarul.cn

[U27] Py：异步 HTTP
来源：http://tdx.hcnkem.com

aiohttp.ClientSession() 配合 async with
来源：http://vnt.jqgfzy.top

[U28] Py：类型别名
来源：http://uwh.birdmap.top

UserId = int
来源：http://ljy.chenlongwang.top

[U29] Py：属性校验
来源：http://bga.yongpay.top

@property 与 @x.setter 配合
来源：http://yse.zhixingplan.top

[U30] Py：数据类
来源：http://vis.jyoumei.cn

@dataclass(slots=True)
来源：http://orw.snrcjt.cn

[U31] Py：单测
来源：http://ygn.c1oappe.top

python -m pytest -q
来源：http://cdf.hywenlv.cn

[U32] Py：代码格式化
来源：http://gat.aibaodan.cn

ruff format . && ruff check --fix .
来源：http://req.xuetiantiany.cn

[U33] Py：打包发布
来源：http://fpk.chenlongwang.top

python -m build  （依赖 pyproject.toml）
来源：http://rji.cdnleiting.top

[U34] Py：判断编码
来源：http://cod.yueranfly.top

chardet.detect(raw)
来源：http://nxi.sxryk.cn

[U35] Py：发送邮件
来源：http://uml.yuanzhike.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ofs.sweek.top

[U36] Py：定时任务
来源：http://nce.gzhubu.top

schedule.every(10).minutes.do(job)
来源：http://kbw.havefunace.top

[U37] Py：读写 Excel
来源：http://lyu.haohaochexian.top

pandas.read_excel / DataFrame.to_excel
来源：http://rap.svipenyu.cn

[U38] Py：获取脚本所在目录
来源：http://boi.shzxlz.cn

Path(__file__).resolve().parent
来源：http://tkb.zhiwuduotai.top

[U39] Py：判断是否在交互环境
来源：http://cne.ctjpmb.com

sys.stdout.isatty()
来源：http://xhu.jqgfzy.top

[U40] Py：打印到标准错误
来源：http://atc.hfpthk.cn

print("err", file=sys.stderr)
来源：http://bzk.sufxvd.cn

[U41] PHP：初始化 Composer 项目
来源：http://ovl.jinghuilouyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://blb.mhx1999.top

[U42] PHP：PSR-4 自动加载
来源：http://ezz.haohaochexian.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://waw.yangfankeji.com

[U43] PHP：声明命名空间
来源：http://tck.hnxiangtu.top

namespace App\Http;
来源：http://evs.yuxming.cn

[U44] PHP：开启严格类型
来源：http://lcc.birdmap.top

declare(strict_types=1);
来源：http://cpr.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://qqj.guowangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lcz.yuanzhike.top

[U46] PHP：可空类型
来源：http://bse.bbcook.cn

?string $name = null
来源：http://gwh.birdmap.top

[U47] PHP：联合类型
来源：http://fdx.gaohongyu789.top

int|string $id
来源：http://lyq.cheryme.top

[U48] PHP：纯枚举
来源：http://fei.yonumen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wdo.fanxiaobao.xyz

[U49] PHP：只读属性
来源：http://kpt.sjlbkw.cn

public readonly string $name
来源：http://hhb.jlsjyb.cn

[U50] PHP：构造器属性提升
来源：http://cbf.ybcxt.top

public function __construct(private int $id) {}
来源：http://ppl.andypj.xyz

[U51] PHP：数组解构
来源：http://jxs.kuanghao11.cn

[$a, $b] = $arr;
来源：http://zsa.ppjwa.cn

[U52] PHP：箭头函数
来源：http://owb.zdbjq.cn

$double = fn($x) => $x * 2;
来源：http://rwr.uphjek.com

[U53] PHP：空合并运算符
来源：http://koe.shuidangran.top

$v = $a ?? $b ?? "default";
来源：http://ive.jiagoushi.top

[U54] PHP：空安全调用
来源：http://hkv.vehdjk.com

$obj?->method()
来源：http://zfk.haohaochexian.top


<!-- 参考信息 -->