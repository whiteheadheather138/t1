代发 wailian999

#ifndef X_H
来源：http://vsv.ywan-chungtsiang.top

#define X_H
来源：http://luq.zhengqikj.top

#endif
来源：http://uww.ivvv.top

[S31] C++：Hello World
来源：http://lyy.nanxuanxn.top

#include <iostream>
来源：http://gtl.jinqigufen.top

int main() { std::cout << "Hello\n"; }
来源：http://hnm.jiagoushi.top

[S32] C++：字符串
来源：http://bsz.shanyushiyangtech.top

std::string s = "hi";  s += "!";
来源：http://jrc.sjlbkw.cn

[S33] C++：vector 增删
来源：http://zma.fengsongda.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nry.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://phb.dianchejie.cn

for (auto &x : v) { std::cout << x; }
来源：http://jbc.zycfv.cn

[S35] C++：map
来源：http://lbi.ctjpmb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vza.nanxuanxn.top

[S36] C++：unordered_map
来源：http://irl.aibaodan.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dll.tian-w.cn

[S37] C++：set
来源：http://vvb.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://srl.aibaodan.cn

[S38] C++：排序
来源：http://efj.ppjwa.cn

std::sort(v.begin(), v.end());
来源：http://llz.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://utu.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yhi.svipenyu.cn

[S40] C++：查找元素
来源：http://wik.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nop.shzxlz.cn

[S41] C++：类与构造函数
来源：http://dlq.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rzb.tarul.cn

[S42] C++：继承与虚函数
来源：http://xod.dashuyun.cn

class B : public Base { public: void f() override {} };
来源：http://iuz.redwolf501.top

[S43] C++：智能指针
来源：http://jvd.0kj1m.cn

auto p = std::make_unique<int>(5);
来源：http://tks.zhongyouzk.top

[S44] C++：引用传参
来源：http://gel.andypj.xyz

void inc(int &x) { ++x; }
来源：http://crc.fzhhl.top

[S45] C++：lambda
来源：http://ift.zhongyouzk.top

auto add = [](int a, int b) { return a + b; };
来源：http://yra.hesvh.cn

[S46] C++：函数模板
来源：http://daa.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ena.zhijiandao.cn

[S47] C++：结构化绑定遍历
来源：http://xla.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nij.guannengcc.top

[S48] C++：逐行读文件
来源：http://zox.sjlbkw.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lmq.ppjwa.cn

while (std::getline(in, line)) { }
来源：http://nby.hysaishi.cn

[S49] C++：写文件
来源：http://aib.hysaishi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kzk.tarul.cn

[S50] C++：格式化数字
来源：http://tqp.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yyf.hnqzz.top

[S51] C++：显式类型转换
来源：http://yeg.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://vfw.hesvh.cn

[S52] C++：const 与 noexcept
来源：http://elf.jinyuanbaomall.cn

int size() const noexcept { return n_; }
来源：http://mxt.hongshengwenyu.top

[S53] C++：移动语义
来源：http://ciu.zhengqikj.top

std::vector<int> w = std::move(v);
来源：http://lad.gogol.net.cn

[S54] C++：异常处理
来源：http://trc.shuidangran.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bwa.wangdashe.top

[S55] C++：结构化绑定
来源：http://vuk.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mxn.hesvh.cn

[S56] C++：optional
来源：http://nff.jqgufenzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wuk.shangyingyoupin.top

[S57] C++：编译期常量
来源：http://moe.wangshuangyany.cn

constexpr int N = 10;
来源：http://uaf.cheryme.top

[S58] C++：命名空间
来源：http://jnq.nanxinkj.top

namespace ns { int f() { return 1; } }
来源：http://xbh.yanxiufei.cn

[S59] C++：静态断言
来源：http://hdj.svipenyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hdr.hnqzz.top

[S60] C++：遍历并删除元素
来源：http://wfo.ydjk.org.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qvi.c1oappe.top

================================================================================
来源：http://mtl.ppjwa.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wob.zdbjq.cn

================================================================================
来源：http://gtq.jinyuanbaomall.cn

[T01] Kotlin：Hello World
来源：http://pvk.0kj1m.cn

println("Hello")
来源：http://hrx.ehwqpu.com

[T02] Kotlin：变量
来源：http://ggr.xinyue.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zta.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://iwh.birdmap.top

"值: $b"
来源：http://fok.jiagoushi.top

[T04] Kotlin：空安全
来源：http://vie.9152youxi.cn

val n: String? = null;  n?.length
来源：http://hjl.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://udm.hesvh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cfd.52xcode.cn

[T06] Kotlin：集合映射
来源：http://ztw.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hgg.bbcook.cn

[T07] Kotlin：集合过滤
来源：http://kxo.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ebt.hnqzz.top

[T08] Kotlin：数据类
来源：http://ehw.yj20258.top

data class User(val name: String, val age: Int)
来源：http://ads.hammf.cn

[T09] Kotlin：扩展函数
来源：http://kdm.cqqwz.cn

fun String.exclaim() = this + "!"
来源：http://mgw.guannengcc.top

[T10] Kotlin：默认参数
来源：http://mwc.yuxming.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hqv.yj20258.top

[T11] Kotlin：协程
来源：http://vnk.jlsjyb.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pwj.yuanzhike.top

[T12] Kotlin：解构声明
来源：http://idl.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://pbc.zhongyouzk.top

[T13] Kotlin：只读 Map
来源：http://uyz.shzxlz.cn

val m = mapOf("a" to 1)
来源：http://olz.zhiwuduotai.top

[T14] Kotlin：循环
来源：http://wpx.gzhubu.top

for (i in 1..10) println(i)
来源：http://ldk.jinqigufen.top

[T15] Kotlin：接口
来源：http://qja.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://tlp.zhoulong.xyz

[T16] Swift：Hello World
来源：http://igd.ctjpmb.com

print("Hello")
来源：http://rso.shzxlz.cn

[T17] Swift：变量与常量
来源：http://uuz.epnwcf.com

var a = 1;  let b = 2
来源：http://myz.sxryk.cn

[T18] Swift：字符串插值
来源：http://wrh.uphjek.com

"值: \(b)"
来源：http://egk.ywan-chungtsiang.top

[T19] Swift：可选绑定
来源：http://ocu.zhengqikj.top

if let n = opt { print(n) }
来源：http://xow.zhijiandao.cn

[T20] Swift：数组操作
来源：http://tsd.bbcook.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oeg.aizwys.cn

[T21] Swift：遍历
来源：http://hiv.jyoumei.cn

for x in a { print(x) }
来源：http://plv.redwolf501.top

[T22] Swift：字典
来源：http://adx.hammf.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vvs.jinqigfzy.top

[T23] Swift：函数
来源：http://ldz.vqdsnc.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rec.havefunace.top

[T24] Swift：闭包
来源：http://hhf.nwbrower.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lpo.hnqzz.top

[T25] Swift：结构体
来源：http://etj.epnwcf.com

struct P { var x: Int }
来源：http://clx.fktsv.cn

[T26] Swift：类与重写
来源：http://xap.ydjk.org.cn

class A: Base { override func f() {} }
来源：http://wmn.xinyue.icu

[T27] Swift：错误处理
来源：http://zup.cashguo.top

do { try f() } catch { print(error) }
来源：http://duw.birdmap.top

[T28] Swift：枚举
来源：http://bve.cdnleiting.top

enum Color { case red, green }
来源：http://zoq.shzxlz.cn

[T29] Swift：guard 提前返回
来源：http://ypu.tarul.cn

guard let x = opt else { return }
来源：http://nrl.dashuyun.cn

[T30] Swift：协议
来源：http://pra.feifeiyinyue.top

protocol Shape { func area() -> Double }
来源：http://xfn.cheryme.top

[T31] Lua：Hello World
来源：http://ozk.gogol.net.cn

print("Hello")
来源：http://jqj.bjfxy.top

[T32] Lua：局部变量
来源：http://eou.tarul.cn

local a = 1
来源：http://owy.birdmap.top

[T33] Lua：表（数组）
来源：http://rjc.yanxiufei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lmw.daria6918.cn

[T34] Lua：遍历表
来源：http://ptr.zdqjudy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ekf.cqqwz.cn

[T35] Lua：字典表
来源：http://ixg.redwolf501.top

local d = { a = 1 };  d.b = 2
来源：http://rhb.hnxiangtu.top

[T36] Lua：函数
来源：http://xnt.cdnleiting.top

function add(a, b) return a + b end
来源：http://biw.yfazqb.com

[T37] Lua：字符串拼接
来源：http://ree.zhaomingkeji.xyz

"a" .. "b"
来源：http://tlk.ivvv.top

[T38] Lua：条件
来源：http://nyz.xziqi.cn

if x > 0 then print("正") end
来源：http://mvb.jqgufenzy.top

[T39] Lua：模式匹配
来源：http://ack.sweek.top

string.find(s, "%d+")
来源：http://pra.birdmap.top

[T40] Lua：元表
来源：http://hfv.pengpengdd.cyou

setmetatable({}, { __index = base })
来源：http://ruj.cdnleiting.top

[T41] Perl：Hello World
来源：http://vxp.xingfuxueyuan.xyz

print "Hello\n";
来源：http://vwm.zhengqikj.top

[T42] Perl：变量类型
来源：http://mwb.zhongyouzk.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yhi.cqqwz.cn

[T43] Perl：字符串插值
来源：http://ahr.iojbl.cn

"值: $a"
来源：http://kbs.shanyushiyangkeji.top

[T44] Perl：条件
来源：http://urt.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://pvt.52xcode.cn

[T45] Perl：数组遍历
来源：http://tqa.fehbvm.com

for my $x (@arr) { print $x; }
来源：http://das.tian-w.cn

[T46] Perl：哈希操作
来源：http://bba.sxryk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qrw.andypj.xyz

[T47] Perl：正则捕获
来源：http://rbe.ybcxt.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://epz.shanyushiyangkeji.top

[T48] Perl：正则替换
来源：http://iye.gogol.net.cn

$s =~ s/old/new/g;
来源：http://knz.jqgufenzy.top

[T49] Perl：函数
来源：http://gwt.yongpay.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vzk.meibo888.top

[T50] Perl：逐行读文件
来源：http://kbz.chenjidiqi.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://gkt.xinyue.icu

while (my $line = <$fh>) { print $line; }
来源：http://xtf.wangshuangyany.cn

[T51] Scala：Hello World
来源：http://ovu.52xcode.cn

println("Hello")
来源：http://syu.ivvv.top

[T52] Scala：变量
来源：http://ntj.cucudq.cn

val a = 1;  var b = 2
来源：http://inz.gogol.net.cn

[T53] Scala：字符串插值
来源：http://dka.ctjpmb.com

s"值: $b"
来源：http://kad.ybcxt.top

[T54] Scala：集合映射
来源：http://svt.shanyushiyangtech.top

List(1, 2, 3).map(_ * 2)
来源：http://vrh.c1oappe.top

[T55] Scala：集合过滤
来源：http://ekr.wangdashe.top

List(1, 2, 3).filter(_ > 1)
来源：http://kbc.nanxuanxn.top

[T56] Scala：样例类
来源：http://stw.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://erc.jqgfzy.top

[T57] Scala：模式匹配
来源：http://szb.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jlf.vehdjk.com

[T58] Scala：函数定义
来源：http://vum.xylfe.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tbi.zhongyouzk.top

[T59] Scala：循环
来源：http://gzn.yangfankeji.com

for (i <- 1 to 10) println(i)
来源：http://hei.ppjwa.cn

[T60] Scala：折叠
来源：http://yfo.jinqigfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hkh.guowangkeji.top

================================================================================
来源：http://qdh.zhoulong.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ccr.fengsongda.top

================================================================================
来源：http://pev.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://ljo.aizwys.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kiv.xingfuxueyuan.xyz

[U02] Py：导出 / 安装依赖
来源：http://kmw.jinyuanbaomall.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uxr.zhixingplan.top

[U03] Py：加载 .env 配置
来源：http://tqa.chenzaomai.com

from dotenv import load_dotenv; load_dotenv()
来源：http://xxy.shangyingyoupin.top

[U04] Py：变量调试打印
来源：http://aqx.hongshengwenyu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xcl.sjlbkw.cn

[U05] Py：列表去重且保序
来源：http://bre.bjfxy.top

list(dict.fromkeys(arr))
来源：http://prd.meibo888.top

[U06] Py：合并两个字典
来源：http://tyu.sufxvd.cn

{**a, **b}
来源：http://ywb.gotoacloud.top

[U07] Py：反转字典键值
来源：http://uie.kuanghao11.cn

{v: k for k, v in d.items()}
来源：http://sxr.yvedp.cn

[U08] Py：展平二维列表
来源：http://oce.cqqwz.cn

[y for x in nested for y in x]
来源：http://bhs.jiagoushi.top

[U09] Py：字典取最大值的键
来源：http://sje.smart0.xyz

max(d, key=d.get)
来源：http://rmi.jinqigufen.top

[U10] Py：按值排序字典
来源：http://lxe.jiagoushi.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bfa.cheryme.top

[U11] Py：生成器表达式
来源：http://gxk.ctjpmb.com

(x * 2 for x in arr)
来源：http://fql.quarkkingdee.top

[U12] Py：取出现最多的 3 个元素
来源：http://gbq.kuanghao11.cn

Counter(arr).most_common(3)
来源：http://cfb.pengpengdd.cyou

[U13] Py：固定长度队列
来源：http://pmx.ybcxt.top

deque(maxlen=10)
来源：http://grg.hesvh.cn

[U14] Py：分组收集到列表
来源：http://jiy.sjlbkw.cn

defaultdict(list)
来源：http://frb.andypj.xyz

[U15] Py：高精度计时
来源：http://apz.smart0.xyz

t = time.perf_counter()
来源：http://xps.fengsongda.top

[U16] Py：命令行参数解析
来源：http://qhy.xingfuxueyuan.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pwa.c1oappe.top

[U17] Py：初始化日志
来源：http://rqg.fktsv.cn

logging.basicConfig(level=logging.INFO)
来源：http://mzn.mhx1999.top

[U18] Py：预编译正则
来源：http://fht.yj20258.top

pat = re.compile(r"\d+")
来源：http://znq.birdmap.top

[U19] Py：正则替换带回调
来源：http://roa.zhixingplan.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ggo.xingfuxueyuan.xyz

[U20] Py：缓存函数结果
来源：http://ryv.tian-w.cn

@functools.lru_cache(maxsize=None)
来源：http://tjv.svipenyu.cn

[U21] Py：自定义上下文管理器
来源：http://hdg.redwolf501.top

@contextlib.contextmanager
来源：http://jcv.zycfv.cn

[U22] Py：矩阵转置
来源：http://llz.daxiang520.top

list(zip(*m))
来源：http://vfu.daxiang520.top

[U23] Py：分块读取大文件
来源：http://opi.tarul.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nys.jlsjyb.cn

[U24] Py：路径操作
来源：http://jnm.zhongyouzk.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://obv.guannengcc.top

[U25] Py：CSV 按字典读
来源：http://ahg.shanyushiyangtech.top

csv.DictReader(f)
来源：http://yku.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://ksx.tanke756.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xwv.hysaishi.cn

[U27] Py：异步 HTTP
来源：http://kgb.uphjek.com

aiohttp.ClientSession() 配合 async with
来源：http://uhi.xinyue.icu

[U28] Py：类型别名
来源：http://eni.tanke756.top

UserId = int
来源：http://sbz.aibaodan.cn

[U29] Py：属性校验
来源：http://scw.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://xvo.gotoacloud.top

[U30] Py：数据类
来源：http://vqa.sufxvd.cn

@dataclass(slots=True)
来源：http://ser.c1oappe.top

[U31] Py：单测
来源：http://wwr.jianghu66.top

python -m pytest -q
来源：http://tzx.zhoulong.xyz

[U32] Py：代码格式化
来源：http://gvs.jiagoushi.top

ruff format . && ruff check --fix .
来源：http://wmb.0kj1m.cn

[U33] Py：打包发布
来源：http://iyk.aizwys.cn

python -m build  （依赖 pyproject.toml）
来源：http://yxg.chenzaomai.com

[U34] Py：判断编码
来源：http://dfv.mhx1999.top

chardet.detect(raw)
来源：http://lhj.tianlin.xyz

[U35] Py：发送邮件
来源：http://nqx.chenlongwang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eml.xuanzx.com

[U36] Py：定时任务
来源：http://xep.fktsv.cn

schedule.every(10).minutes.do(job)
来源：http://lzx.tianlin.xyz

[U37] Py：读写 Excel
来源：http://hfq.c1oappe.top

pandas.read_excel / DataFrame.to_excel
来源：http://gxs.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://cgz.guannengcc.top

Path(__file__).resolve().parent
来源：http://nlz.xinyue.icu

[U39] Py：判断是否在交互环境
来源：http://obh.yangfankeji.com

sys.stdout.isatty()
来源：http://hip.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://nha.0kj1m.cn

print("err", file=sys.stderr)
来源：http://jfr.daria6918.cn

[U41] PHP：初始化 Composer 项目
来源：http://zab.andypj.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://fte.ctjpmb.com

[U42] PHP：PSR-4 自动加载
来源：http://ynt.jyoumei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xvw.52xcode.cn

[U43] PHP：声明命名空间
来源：http://igd.aizwys.cn

namespace App\Http;
来源：http://cns.xuanzx.com

[U44] PHP：开启严格类型
来源：http://rhh.sjlbkw.cn

declare(strict_types=1);
来源：http://jpd.yuanzhike.top

[U45] PHP：类型声明与返回类型
来源：http://ipo.wangshuangyany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fag.yj202588.top

[U46] PHP：可空类型
来源：http://bhz.jianghu66.top

?string $name = null
来源：http://gxc.daria6918.cn

[U47] PHP：联合类型
来源：http://kud.guowangkeji.top

int|string $id
来源：http://tkd.yfazqb.com

[U48] PHP：纯枚举
来源：http://evs.daria6918.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://twd.smart0.xyz

[U49] PHP：只读属性
来源：http://oya.hammf.cn

public readonly string $name
来源：http://tco.zhixingplan.top

[U50] PHP：构造器属性提升
来源：http://qdi.birdmap.top

public function __construct(private int $id) {}
来源：http://ipd.fzhhl.top

[U51] PHP：数组解构
来源：http://nrc.redwolf501.top

[$a, $b] = $arr;
来源：http://nri.quarkkingdee.top

[U52] PHP：箭头函数
来源：http://ddf.fehbvm.com

$double = fn($x) => $x * 2;
来源：http://oct.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://dhy.zhixingplan.top

$v = $a ?? $b ?? "default";
来源：http://wtg.hesvh.cn

[U54] PHP：空安全调用
来源：http://ftt.fengsongda.top

$obj?->method()
来源：http://oft.9152youxi.cn


<!-- 参考信息 -->