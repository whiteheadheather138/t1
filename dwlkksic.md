代发 wailian999

static int counter = 0;
来源：http://xay.sxryk.cn

[S29] C：变参函数
来源：http://lvs.pengpengdd.cyou

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lto.tianlin.xyz

[S30] C：头文件保护
来源：http://gda.yfazqb.com

#ifndef X_H
来源：http://gpz.iojbl.cn

#define X_H
来源：http://pkx.jlsjyb.cn

#endif
来源：http://mvl.yanxiufei.cn

[S31] C++：Hello World
来源：http://kvv.shanyushiyangkeji.top

#include <iostream>
来源：http://rmx.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://zho.shangyingyoupin.top

[S32] C++：字符串
来源：http://fff.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://aeg.dashuyun.cn

[S33] C++：vector 增删
来源：http://oge.yuanzhike.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iue.zdbjq.cn

[S34] C++：遍历 vector
来源：http://lkl.tanke756.top

for (auto &x : v) { std::cout << x; }
来源：http://wjm.snrcjt.cn

[S35] C++：map
来源：http://yfl.yueranfly.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vfu.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://vvz.jqgufenzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://twh.tarul.cn

[S37] C++：set
来源：http://uzh.ywan-chungtsiang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iic.redwolf501.top

[S38] C++：排序
来源：http://xrv.sweek.top

std::sort(v.begin(), v.end());
来源：http://lgk.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://zxj.jlsjyb.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://stu.tarul.cn

[S40] C++：查找元素
来源：http://uaa.quarkkingdee.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lms.guannengcc.top

[S41] C++：类与构造函数
来源：http://oex.jianghu66.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vyd.xinyue.icu

[S42] C++：继承与虚函数
来源：http://oht.feifeiyinyue.top

class B : public Base { public: void f() override {} };
来源：http://eqx.zhixingplan.top

[S43] C++：智能指针
来源：http://fts.ywan-chungtsiang.top

auto p = std::make_unique<int>(5);
来源：http://qgb.ywan-chungtsiang.top

[S44] C++：引用传参
来源：http://ntv.aizwys.cn

void inc(int &x) { ++x; }
来源：http://erm.jianghu66.top

[S45] C++：lambda
来源：http://euu.yuxming.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ifo.yvedp.cn

[S46] C++：函数模板
来源：http://cdd.cqqwz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vzg.meibo888.top

[S47] C++：结构化绑定遍历
来源：http://icq.ydjk.org.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://onf.quarkkingdee.top

[S48] C++：逐行读文件
来源：http://yaa.xinyue.icu

std::ifstream in("a.txt");  std::string line;
来源：http://wzc.jinyuanbaomall.cn

while (std::getline(in, line)) { }
来源：http://iju.pengpengdd.cyou

[S49] C++：写文件
来源：http://zuw.gzhubu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dcm.yangfankeji.com

[S50] C++：格式化数字
来源：http://wmh.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ucf.pycfn.com

[S51] C++：显式类型转换
来源：http://ltc.yueranfly.top

static_cast<double>(a) / b
来源：http://vkm.vehdjk.com

[S52] C++：const 与 noexcept
来源：http://gxd.vehdjk.com

int size() const noexcept { return n_; }
来源：http://zvq.gaohongyu789.top

[S53] C++：移动语义
来源：http://oss.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://mdd.sufxvd.cn

[S54] C++：异常处理
来源：http://bxq.ydzc1.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ooe.shzxlz.cn

[S55] C++：结构化绑定
来源：http://biy.uphjek.com

auto [a, b] = std::make_pair(1, 2);
来源：http://dfm.sxryk.cn

[S56] C++：optional
来源：http://hsg.guannengcc.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jtp.redwolf501.top

[S57] C++：编译期常量
来源：http://fvh.svipenyu.cn

constexpr int N = 10;
来源：http://akw.zdqjudy.top

[S58] C++：命名空间
来源：http://jca.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://fyh.hcnkem.com

[S59] C++：静态断言
来源：http://xxy.jinqigufen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://akg.gaohongyu789.top

[S60] C++：遍历并删除元素
来源：http://njq.zdqjudy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rwj.yfazqb.com

================================================================================
来源：http://zxb.shzxlz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bwg.yuxming.cn

================================================================================
来源：http://nyl.hongshengwenyu.top

[T01] Kotlin：Hello World
来源：http://kzv.birdmap.top

println("Hello")
来源：http://ldq.cdnleiting.top

[T02] Kotlin：变量
来源：http://twk.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wgu.sxryk.cn

[T03] Kotlin：字符串模板
来源：http://rnq.sufxvd.cn

"值: $b"
来源：http://sgo.ctjpmb.com

[T04] Kotlin：空安全
来源：http://jyd.fehbvm.com

val n: String? = null;  n?.length
来源：http://gpw.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://veo.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qgu.birdmap.top

[T06] Kotlin：集合映射
来源：http://vrd.haohaochexian.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tvc.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://pfr.jianghu66.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qtb.0kj1m.cn

[T08] Kotlin：数据类
来源：http://jrv.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://cvk.jiagoushi.top

[T09] Kotlin：扩展函数
来源：http://yvo.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://osl.jqgufenzy.top

[T10] Kotlin：默认参数
来源：http://ehq.sxryk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gtp.haohaochexian.top

[T11] Kotlin：协程
来源：http://zud.zdbjq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bfo.zhoulong.xyz

[T12] Kotlin：解构声明
来源：http://eay.hywenlv.cn

val (a, b) = Pair(1, 2)
来源：http://vhw.gaohongyu789.top

[T13] Kotlin：只读 Map
来源：http://rcz.uphjek.com

val m = mapOf("a" to 1)
来源：http://qyg.uphjek.com

[T14] Kotlin：循环
来源：http://hrq.zhiwuduotai.top

for (i in 1..10) println(i)
来源：http://cfp.316326.xyz

[T15] Kotlin：接口
来源：http://cyw.aibaodan.cn

interface Shape { fun area(): Double }
来源：http://uld.zhongyouzk.top

[T16] Swift：Hello World
来源：http://jkr.vqdsnc.cn

print("Hello")
来源：http://hfu.aibaodan.cn

[T17] Swift：变量与常量
来源：http://ucm.zhongyouzk.top

var a = 1;  let b = 2
来源：http://gei.vehdjk.com

[T18] Swift：字符串插值
来源：http://xpq.wangshuangyany.cn

"值: \(b)"
来源：http://lbj.zhaomingkeji.xyz

[T19] Swift：可选绑定
来源：http://hnn.fzhhl.top

if let n = opt { print(n) }
来源：http://mpf.nanxinkj.top

[T20] Swift：数组操作
来源：http://yvk.zdqjudy.top

var a = [1, 2, 3];  a.append(4)
来源：http://kzl.cashguo.top

[T21] Swift：遍历
来源：http://tjs.meibo888.top

for x in a { print(x) }
来源：http://pdw.xingfuxueyuan.xyz

[T22] Swift：字典
来源：http://hus.zhongyouzk.top

var d = ["a": 1];  d["b"] = 2
来源：http://cmf.haohaochexian.top

[T23] Swift：函数
来源：http://ztk.wangdashe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hth.gzhubu.top

[T24] Swift：闭包
来源：http://exy.xylfe.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oci.jqgfzy.top

[T25] Swift：结构体
来源：http://skq.iojbl.cn

struct P { var x: Int }
来源：http://fwm.zhengqikj.top

[T26] Swift：类与重写
来源：http://fjj.tianlin.xyz

class A: Base { override func f() {} }
来源：http://pbt.hywenlv.cn

[T27] Swift：错误处理
来源：http://qla.hesvh.cn

do { try f() } catch { print(error) }
来源：http://gla.aibaodan.cn

[T28] Swift：枚举
来源：http://stt.sjlbkw.cn

enum Color { case red, green }
来源：http://kya.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://yva.zhengqikj.top

guard let x = opt else { return }
来源：http://zjw.wangshuangyany.cn

[T30] Swift：协议
来源：http://xhs.hywenlv.cn

protocol Shape { func area() -> Double }
来源：http://bik.jinyuanbaomall.cn

[T31] Lua：Hello World
来源：http://nwr.yj20258888.top

print("Hello")
来源：http://nsb.xziqi.cn

[T32] Lua：局部变量
来源：http://bpn.kuanghao11.cn

local a = 1
来源：http://wsn.haohaochexian.top

[T33] Lua：表（数组）
来源：http://tlh.tarul.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sbn.gogol.net.cn

[T34] Lua：遍历表
来源：http://qvu.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kmm.xuetiantiany.cn

[T35] Lua：字典表
来源：http://tsd.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://ekt.sxryk.cn

[T36] Lua：函数
来源：http://oax.cucudq.cn

function add(a, b) return a + b end
来源：http://iot.ppjwa.cn

[T37] Lua：字符串拼接
来源：http://egv.9152youxi.cn

"a" .. "b"
来源：http://hrq.birdmap.top

[T38] Lua：条件
来源：http://mmo.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://ohb.xingfuxueyuan.xyz

[T39] Lua：模式匹配
来源：http://zuu.hfpthk.cn

string.find(s, "%d+")
来源：http://oxa.xingfuxueyuan.xyz

[T40] Lua：元表
来源：http://uso.yvedp.cn

setmetatable({}, { __index = base })
来源：http://don.yj202588.top

[T41] Perl：Hello World
来源：http://hqk.fehbvm.com

print "Hello\n";
来源：http://mpj.ydjk.org.cn

[T42] Perl：变量类型
来源：http://swv.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wpz.zhoulong.xyz

[T43] Perl：字符串插值
来源：http://yvu.hnxiangtu.top

"值: $a"
来源：http://xav.ppjwa.cn

[T44] Perl：条件
来源：http://lvn.c1oappe.top

if ($a > 0) { print "正"; }
来源：http://has.jyoumei.cn

[T45] Perl：数组遍历
来源：http://upt.wangshuangyany.cn

for my $x (@arr) { print $x; }
来源：http://qdm.fehbvm.com

[T46] Perl：哈希操作
来源：http://ilz.52xcode.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yrn.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://cla.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://gua.c1oappe.top

[T48] Perl：正则替换
来源：http://cpq.zycfv.cn

$s =~ s/old/new/g;
来源：http://xvc.hesvh.cn

[T49] Perl：函数
来源：http://zer.9152youxi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jcv.snrcjt.cn

[T50] Perl：逐行读文件
来源：http://wmg.vqdsnc.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lht.jinyuanbaomall.cn

while (my $line = <$fh>) { print $line; }
来源：http://icn.jqgfzy.top

[T51] Scala：Hello World
来源：http://udy.hesvh.cn

println("Hello")
来源：http://fjo.gotoacloud.top

[T52] Scala：变量
来源：http://lxb.tianlin.xyz

val a = 1;  var b = 2
来源：http://rwp.chenjidiqi.icu

[T53] Scala：字符串插值
来源：http://rqa.9152youxi.cn

s"值: $b"
来源：http://mki.redwolf501.top

[T54] Scala：集合映射
来源：http://fot.hfpthk.cn

List(1, 2, 3).map(_ * 2)
来源：http://hrk.yuanzhike.top

[T55] Scala：集合过滤
来源：http://xnj.shanyushiyangtech.top

List(1, 2, 3).filter(_ > 1)
来源：http://vlg.hfpthk.cn

[T56] Scala：样例类
来源：http://wgo.birdmap.top

case class User(name: String, age: Int)
来源：http://otz.meibo888.top

[T57] Scala：模式匹配
来源：http://vkf.kuanghao11.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hlr.guannengcc.top

[T58] Scala：函数定义
来源：http://faq.daxiang520.top

def add(a: Int, b: Int): Int = a + b
来源：http://zst.jqgfzy.top

[T59] Scala：循环
来源：http://jnw.tianlin.xyz

for (i <- 1 to 10) println(i)
来源：http://ydm.wangdashe.top

[T60] Scala：折叠
来源：http://wpw.jianghu66.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://onv.hongshengwenyu.top

================================================================================
来源：http://atj.hesvh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cre.chenjidiqi.icu

================================================================================
来源：http://lqz.yanxiufei.cn

[U01] Py：创建虚拟环境
来源：http://qxa.aibaodan.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rxo.chenjidiqi.icu

[U02] Py：导出 / 安装依赖
来源：http://kgd.sufxvd.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://azh.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://tfi.zhijiandao.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://olb.yfazqb.com

[U04] Py：变量调试打印
来源：http://rjv.sweek.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qah.hfpthk.cn

[U05] Py：列表去重且保序
来源：http://tfy.andypj.xyz

list(dict.fromkeys(arr))
来源：http://lgu.xylfe.cn

[U06] Py：合并两个字典
来源：http://iki.snrcjt.cn

{**a, **b}
来源：http://dgr.yj20258.top

[U07] Py：反转字典键值
来源：http://oou.fehbvm.com

{v: k for k, v in d.items()}
来源：http://rui.sxryk.cn

[U08] Py：展平二维列表
来源：http://cxl.zhixingplan.top

[y for x in nested for y in x]
来源：http://vvs.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://qer.bbcook.cn

max(d, key=d.get)
来源：http://wxi.ybcxt.top

[U10] Py：按值排序字典
来源：http://gmr.hesvh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cnz.316326.xyz

[U11] Py：生成器表达式
来源：http://itd.hysaishi.cn

(x * 2 for x in arr)
来源：http://avy.andypj.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://zwe.hesvh.cn

Counter(arr).most_common(3)
来源：http://pne.zhengqikj.top

[U13] Py：固定长度队列
来源：http://uya.xuanzx.com

deque(maxlen=10)
来源：http://lyn.yj20258888.top

[U14] Py：分组收集到列表
来源：http://mfj.fanxiaobao.xyz

defaultdict(list)
来源：http://evn.chenlongwang.top

[U15] Py：高精度计时
来源：http://xtx.9152youxi.cn

t = time.perf_counter()
来源：http://ibs.uphjek.com

[U16] Py：命令行参数解析
来源：http://ngq.xingfuxueyuan.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uhb.jqgfzy.top

[U17] Py：初始化日志
来源：http://unp.yonumen.top

logging.basicConfig(level=logging.INFO)
来源：http://hun.ybcxt.top

[U18] Py：预编译正则
来源：http://ryt.yanxiufei.cn

pat = re.compile(r"\d+")
来源：http://wdz.nwbrower.top

[U19] Py：正则替换带回调
来源：http://ttf.cheryme.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ggo.smart0.xyz

[U20] Py：缓存函数结果
来源：http://sol.jiagoushi.top

@functools.lru_cache(maxsize=None)
来源：http://aoc.jlsjyb.cn

[U21] Py：自定义上下文管理器
来源：http://zxc.sweek.top

@contextlib.contextmanager
来源：http://eqn.sjlbkw.cn

[U22] Py：矩阵转置
来源：http://hrw.nanxuanxn.top

list(zip(*m))
来源：http://evj.hongshengwenyu.top

[U23] Py：分块读取大文件
来源：http://pho.snrcjt.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fig.fzhhl.top

[U24] Py：路径操作
来源：http://onr.zhiwuduotai.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hla.jqgufenzy.top

[U25] Py：CSV 按字典读
来源：http://lmx.wangdashe.top

csv.DictReader(f)
来源：http://thh.fktsv.cn

[U26] Py：并发下载
来源：http://gau.yangfankeji.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xww.gaohongyu789.top

[U27] Py：异步 HTTP
来源：http://ziz.fehbvm.com

aiohttp.ClientSession() 配合 async with
来源：http://gfp.shzxlz.cn

[U28] Py：类型别名
来源：http://yty.jyoumei.cn

UserId = int
来源：http://eyq.jlsjyb.cn

[U29] Py：属性校验
来源：http://rqc.xuetiantiany.cn

@property 与 @x.setter 配合
来源：http://hwh.yongpay.top

[U30] Py：数据类
来源：http://gjp.xylfe.cn

@dataclass(slots=True)
来源：http://aov.shangyingyoupin.top

[U31] Py：单测
来源：http://bny.yuxming.cn

python -m pytest -q
来源：http://nrc.nanxinkj.top

[U32] Py：代码格式化
来源：http://lfa.shanyushiyangkeji.top

ruff format . && ruff check --fix .
来源：http://pca.wangshuangyany.cn

[U33] Py：打包发布
来源：http://ilz.fktsv.cn

python -m build  （依赖 pyproject.toml）
来源：http://fnr.dashuyun.cn

[U34] Py：判断编码
来源：http://kgt.chenzaomai.com

chardet.detect(raw)
来源：http://kmk.epnwcf.com

[U35] Py：发送邮件
来源：http://gcc.zhengqikj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hlz.zhengqikj.top

[U36] Py：定时任务
来源：http://piu.hywenlv.cn

schedule.every(10).minutes.do(job)
来源：http://kbu.ppjwa.cn

[U37] Py：读写 Excel
来源：http://pgj.bjfxy.top

pandas.read_excel / DataFrame.to_excel
来源：http://gvo.ydjk.org.cn

[U38] Py：获取脚本所在目录
来源：http://pcs.zhijiandao.cn

Path(__file__).resolve().parent
来源：http://tsf.cucudq.cn

[U39] Py：判断是否在交互环境
来源：http://zcz.jinghuilouyu.cn

sys.stdout.isatty()
来源：http://mgr.sxryk.cn

[U40] Py：打印到标准错误
来源：http://wnb.cqqwz.cn

print("err", file=sys.stderr)
来源：http://osa.xingfuxueyuan.xyz

[U41] PHP：初始化 Composer 项目
来源：http://nyd.cdnleiting.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vhc.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://yws.tanke756.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://goa.hesvh.cn

[U43] PHP：声明命名空间
来源：http://ydp.xingfuxueyuan.xyz

namespace App\Http;
来源：http://bdd.c1oappe.top

[U44] PHP：开启严格类型
来源：http://xkv.yueranfly.top

declare(strict_types=1);
来源：http://kph.fzhhl.top

[U45] PHP：类型声明与返回类型
来源：http://lip.shangyingyoupin.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://rjw.yuanzhike.top

[U46] PHP：可空类型
来源：http://kdq.ydzc1.top

?string $name = null
来源：http://ljl.tarul.cn

[U47] PHP：联合类型
来源：http://ixz.0kj1m.cn

int|string $id
来源：http://fss.xziqi.cn

[U48] PHP：纯枚举
来源：http://aul.yfazqb.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rbo.meibo888.top

[U49] PHP：只读属性
来源：http://tfi.andypj.xyz

public readonly string $name
来源：http://pxz.yangfankeji.com

[U50] PHP：构造器属性提升
来源：http://gwt.mhx1999.top

public function __construct(private int $id) {}
来源：http://qqm.shuidangran.top

[U51] PHP：数组解构
来源：http://ube.chenlongwang.top

[$a, $b] = $arr;
来源：http://pah.meibo888.top

[U52] PHP：箭头函数
来源：http://ezn.birdmap.top

$double = fn($x) => $x * 2;
来源：http://tze.andypj.xyz


<!-- 参考信息 -->