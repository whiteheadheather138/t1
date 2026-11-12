代发 wailian999

static int counter = 0;
来源：http://mlv.nanxuanxn.top

[S29] C：变参函数
来源：http://dgf.fehbvm.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tfn.jinqigfzy.top

[S30] C：头文件保护
来源：http://owd.aizwys.cn

#ifndef X_H
来源：http://lpo.yuxming.cn

#define X_H
来源：http://gfd.hammf.cn

#endif
来源：http://dmy.fanxiaobao.xyz

[S31] C++：Hello World
来源：http://yaf.fanxiaobao.xyz

#include <iostream>
来源：http://wyg.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://pjd.ivvv.top

[S32] C++：字符串
来源：http://hit.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://sjz.zdbjq.cn

[S33] C++：vector 增删
来源：http://opo.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oax.daria6918.cn

[S34] C++：遍历 vector
来源：http://orq.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://kfk.ywan-chungtsiang.top

[S35] C++：map
来源：http://erp.jianghu66.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wkz.52xcode.cn

[S36] C++：unordered_map
来源：http://zbl.ywan-chungtsiang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uwb.jqgufenzy.top

[S37] C++：set
来源：http://bvs.feifeiyinyue.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dyu.redwolf501.top

[S38] C++：排序
来源：http://vat.epnwcf.com

std::sort(v.begin(), v.end());
来源：http://egp.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://eyj.bjfxy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aip.chenzaomai.com

[S40] C++：查找元素
来源：http://zsl.zhaomingkeji.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bgl.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://bxc.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zkv.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://vds.nwbrower.top

class B : public Base { public: void f() override {} };
来源：http://ymp.yangfankeji.com

[S43] C++：智能指针
来源：http://gql.bbcook.cn

auto p = std::make_unique<int>(5);
来源：http://hfe.yongpay.top

[S44] C++：引用传参
来源：http://pgq.meibo888.top

void inc(int &x) { ++x; }
来源：http://msf.guowangkeji.top

[S45] C++：lambda
来源：http://knn.jinghuilouyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bsq.epnwcf.com

[S46] C++：函数模板
来源：http://cnx.ydjk.org.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nwi.zhongyouzk.top

[S47] C++：结构化绑定遍历
来源：http://mfv.ydzc1.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oqh.cashguo.top

[S48] C++：逐行读文件
来源：http://fgk.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://yvt.ppjwa.cn

while (std::getline(in, line)) { }
来源：http://vpw.pycfn.com

[S49] C++：写文件
来源：http://rji.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rua.birdmap.top

[S50] C++：格式化数字
来源：http://xjt.ehwqpu.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wkz.jinqigfzy.top

[S51] C++：显式类型转换
来源：http://hml.andypj.xyz

static_cast<double>(a) / b
来源：http://stz.ivvv.top

[S52] C++：const 与 noexcept
来源：http://elj.yj202588.top

int size() const noexcept { return n_; }
来源：http://hro.wangdashe.top

[S53] C++：移动语义
来源：http://fie.guowangkeji.top

std::vector<int> w = std::move(v);
来源：http://juv.hfpthk.cn

[S54] C++：异常处理
来源：http://szt.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ogz.jiagoushi.top

[S55] C++：结构化绑定
来源：http://iud.c1oappe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dxv.hammf.cn

[S56] C++：optional
来源：http://kdu.dianchejie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mml.daria6918.cn

[S57] C++：编译期常量
来源：http://gka.haohaochexian.top

constexpr int N = 10;
来源：http://kaf.guannengcc.top

[S58] C++：命名空间
来源：http://erj.ydzc1.top

namespace ns { int f() { return 1; } }
来源：http://byu.zhiwuduotai.top

[S59] C++：静态断言
来源：http://blj.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hax.cashguo.top

[S60] C++：遍历并删除元素
来源：http://syt.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vvz.ybcxt.top

================================================================================
来源：http://fva.pengpengdd.cyou

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hvz.ivvv.top

================================================================================
来源：http://ljm.tian-w.cn

[T01] Kotlin：Hello World
来源：http://ukk.fengsongda.top

println("Hello")
来源：http://hjh.yvedp.cn

[T02] Kotlin：变量
来源：http://qdu.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vzc.sweek.top

[T03] Kotlin：字符串模板
来源：http://tiv.hcnkem.com

"值: $b"
来源：http://int.jianghu66.top

[T04] Kotlin：空安全
来源：http://ssd.yuanzhike.top

val n: String? = null;  n?.length
来源：http://fil.ydzc1.top

[T05] Kotlin：when 表达式
来源：http://xnp.sufxvd.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kvs.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://ncr.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jry.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://ray.316326.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://rwh.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://iym.c1oappe.top

data class User(val name: String, val age: Int)
来源：http://ymn.xziqi.cn

[T09] Kotlin：扩展函数
来源：http://uga.zycfv.cn

fun String.exclaim() = this + "!"
来源：http://trd.cqqwz.cn

[T10] Kotlin：默认参数
来源：http://vxq.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tfl.daria6918.cn

[T11] Kotlin：协程
来源：http://adv.wangdashe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bwo.chenlongwang.top

[T12] Kotlin：解构声明
来源：http://rtl.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://kbe.xuanzx.com

[T13] Kotlin：只读 Map
来源：http://ezq.gotoacloud.top

val m = mapOf("a" to 1)
来源：http://fge.jianghu66.top

[T14] Kotlin：循环
来源：http://qaf.yangfankeji.com

for (i in 1..10) println(i)
来源：http://aej.epnwcf.com

[T15] Kotlin：接口
来源：http://yhg.sysykeji.top

interface Shape { fun area(): Double }
来源：http://ciw.daxiang520.top

[T16] Swift：Hello World
来源：http://dys.hywenlv.cn

print("Hello")
来源：http://pur.zhaomingkeji.xyz

[T17] Swift：变量与常量
来源：http://gjx.jinqigfzy.top

var a = 1;  let b = 2
来源：http://pzw.nwbrower.top

[T18] Swift：字符串插值
来源：http://ynj.zhiwuduotai.top

"值: \(b)"
来源：http://stz.zhongyouzk.top

[T19] Swift：可选绑定
来源：http://nse.cdnleiting.top

if let n = opt { print(n) }
来源：http://twq.ehwqpu.com

[T20] Swift：数组操作
来源：http://qtm.hnqzz.top

var a = [1, 2, 3];  a.append(4)
来源：http://kmq.zdbjq.cn

[T21] Swift：遍历
来源：http://god.guannengcc.top

for x in a { print(x) }
来源：http://kwe.sysykeji.top

[T22] Swift：字典
来源：http://opv.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://wwo.yueranfly.top

[T23] Swift：函数
来源：http://xkb.hfpthk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hsj.hongshengwenyu.top

[T24] Swift：闭包
来源：http://anj.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zbk.zhengqikj.top

[T25] Swift：结构体
来源：http://lbm.sysykeji.top

struct P { var x: Int }
来源：http://bud.9152youxi.cn

[T26] Swift：类与重写
来源：http://nxv.hfpthk.cn

class A: Base { override func f() {} }
来源：http://het.yuxming.cn

[T27] Swift：错误处理
来源：http://qhr.iojbl.cn

do { try f() } catch { print(error) }
来源：http://hvz.aizwys.cn

[T28] Swift：枚举
来源：http://ivd.yvedp.cn

enum Color { case red, green }
来源：http://ifu.zdqjudy.top

[T29] Swift：guard 提前返回
来源：http://cpw.dashuyun.cn

guard let x = opt else { return }
来源：http://naf.fzhhl.top

[T30] Swift：协议
来源：http://wlz.c1oappe.top

protocol Shape { func area() -> Double }
来源：http://uyp.wangshuangyany.cn

[T31] Lua：Hello World
来源：http://iie.hfpthk.cn

print("Hello")
来源：http://njg.fanxiaobao.xyz

[T32] Lua：局部变量
来源：http://yef.jlsjyb.cn

local a = 1
来源：http://vmy.smart0.xyz

[T33] Lua：表（数组）
来源：http://wgd.cucudq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://afb.iojbl.cn

[T34] Lua：遍历表
来源：http://szt.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://itp.wangdashe.top

[T35] Lua：字典表
来源：http://syt.fktsv.cn

local d = { a = 1 };  d.b = 2
来源：http://che.vqdsnc.cn

[T36] Lua：函数
来源：http://lwv.shzxlz.cn

function add(a, b) return a + b end
来源：http://poa.zhijiandao.cn

[T37] Lua：字符串拼接
来源：http://ltc.yuxming.cn

"a" .. "b"
来源：http://xxf.haohaochexian.top

[T38] Lua：条件
来源：http://vvk.bbcook.cn

if x > 0 then print("正") end
来源：http://lcb.shuidangran.top

[T39] Lua：模式匹配
来源：http://anr.zhongyouzk.top

string.find(s, "%d+")
来源：http://xzz.cashguo.top

[T40] Lua：元表
来源：http://qdw.snrcjt.cn

setmetatable({}, { __index = base })
来源：http://ocp.zdbjq.cn

[T41] Perl：Hello World
来源：http://glo.vehdjk.com

print "Hello\n";
来源：http://zsw.yonumen.top

[T42] Perl：变量类型
来源：http://mcu.ehwqpu.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ovl.xinyue.icu

[T43] Perl：字符串插值
来源：http://lze.shanyushiyangtech.top

"值: $a"
来源：http://tnd.hnqzz.top

[T44] Perl：条件
来源：http://rmz.xingfuxueyuan.xyz

if ($a > 0) { print "正"; }
来源：http://gbp.hcnkem.com

[T45] Perl：数组遍历
来源：http://seh.316326.xyz

for my $x (@arr) { print $x; }
来源：http://uza.hesvh.cn

[T46] Perl：哈希操作
来源：http://leo.nanxuanxn.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tpp.snrcjt.cn

[T47] Perl：正则捕获
来源：http://wan.fengsongda.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lmk.ydjk.org.cn

[T48] Perl：正则替换
来源：http://gls.sjlbkw.cn

$s =~ s/old/new/g;
来源：http://ubu.gotoacloud.top

[T49] Perl：函数
来源：http://thw.52xcode.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hfq.fktsv.cn

[T50] Perl：逐行读文件
来源：http://vil.hysaishi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ils.haohaochexian.top

while (my $line = <$fh>) { print $line; }
来源：http://ctp.shuidangran.top

[T51] Scala：Hello World
来源：http://msu.smart0.xyz

println("Hello")
来源：http://nmz.xingfuxueyuan.xyz

[T52] Scala：变量
来源：http://ase.c1oappe.top

val a = 1;  var b = 2
来源：http://yym.guannengcc.top

[T53] Scala：字符串插值
来源：http://soy.hesvh.cn

s"值: $b"
来源：http://fqx.yuxming.cn

[T54] Scala：集合映射
来源：http://nuz.zhoulong.xyz

List(1, 2, 3).map(_ * 2)
来源：http://cyr.hfpthk.cn

[T55] Scala：集合过滤
来源：http://bel.hnxiangtu.top

List(1, 2, 3).filter(_ > 1)
来源：http://lpa.kuanghao11.cn

[T56] Scala：样例类
来源：http://zku.xingfuxueyuan.xyz

case class User(name: String, age: Int)
来源：http://wwd.52xcode.cn

[T57] Scala：模式匹配
来源：http://gdy.hywenlv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://txd.hammf.cn

[T58] Scala：函数定义
来源：http://uhq.yonumen.top

def add(a: Int, b: Int): Int = a + b
来源：http://wpq.hongshengwenyu.top

[T59] Scala：循环
来源：http://tft.fehbvm.com

for (i <- 1 to 10) println(i)
来源：http://ejx.zhoulong.xyz

[T60] Scala：折叠
来源：http://gfq.jianghu66.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://liy.wangshuangyany.cn

================================================================================
来源：http://qnv.nwbrower.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ugq.xuanzx.com

================================================================================
来源：http://mxi.birdmap.top

[U01] Py：创建虚拟环境
来源：http://jjg.hongshengwenyu.top

python -m venv .venv && source .venv/bin/activate
来源：http://qoi.gogol.net.cn

[U02] Py：导出 / 安装依赖
来源：http://quo.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vqz.xziqi.cn

[U03] Py：加载 .env 配置
来源：http://pqc.guowangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ifp.jinqigfzy.top

[U04] Py：变量调试打印
来源：http://oia.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oar.fktsv.cn

[U05] Py：列表去重且保序
来源：http://vjt.ehwqpu.com

list(dict.fromkeys(arr))
来源：http://tur.birdmap.top

[U06] Py：合并两个字典
来源：http://vaj.gogol.net.cn

{**a, **b}
来源：http://ipy.sxryk.cn

[U07] Py：反转字典键值
来源：http://gpf.bbcook.cn

{v: k for k, v in d.items()}
来源：http://gjc.316326.xyz

[U08] Py：展平二维列表
来源：http://ocx.52xcode.cn

[y for x in nested for y in x]
来源：http://cip.shuidangran.top

[U09] Py：字典取最大值的键
来源：http://tyg.zdqjudy.top

max(d, key=d.get)
来源：http://pcm.pycfn.com

[U10] Py：按值排序字典
来源：http://ryd.9152youxi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xyh.vehdjk.com

[U11] Py：生成器表达式
来源：http://htq.316326.xyz

(x * 2 for x in arr)
来源：http://var.yj20258.top

[U12] Py：取出现最多的 3 个元素
来源：http://tnn.jiagoushi.top

Counter(arr).most_common(3)
来源：http://fxx.c1oappe.top

[U13] Py：固定长度队列
来源：http://zwc.yfazqb.com

deque(maxlen=10)
来源：http://ltr.sysykeji.top

[U14] Py：分组收集到列表
来源：http://qzw.smart0.xyz

defaultdict(list)
来源：http://zdl.hnxiangtu.top

[U15] Py：高精度计时
来源：http://cjx.ydjk.org.cn

t = time.perf_counter()
来源：http://pyk.ywan-chungtsiang.top

[U16] Py：命令行参数解析
来源：http://pgc.0kj1m.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ils.ehwqpu.com

[U17] Py：初始化日志
来源：http://ezw.kuanghao11.cn

logging.basicConfig(level=logging.INFO)
来源：http://haz.yuanzhike.top

[U18] Py：预编译正则
来源：http://elt.chenlongwang.top

pat = re.compile(r"\d+")
来源：http://ivv.zhixingplan.top

[U19] Py：正则替换带回调
来源：http://pqp.fehbvm.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mkw.ctjpmb.com

[U20] Py：缓存函数结果
来源：http://iel.quarkkingdee.top

@functools.lru_cache(maxsize=None)
来源：http://vug.tanke756.top

[U21] Py：自定义上下文管理器
来源：http://bmp.yfazqb.com

@contextlib.contextmanager
来源：http://hml.yangfankeji.com

[U22] Py：矩阵转置
来源：http://nzx.wangshuangyany.cn

list(zip(*m))
来源：http://wyg.daxiang520.top

[U23] Py：分块读取大文件
来源：http://jtw.zhixingplan.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mln.hnqzz.top

[U24] Py：路径操作
来源：http://faq.aizwys.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qcu.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://dei.sjlbkw.cn

csv.DictReader(f)
来源：http://xmx.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://nzv.gotoacloud.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ibu.daria6918.cn

[U27] Py：异步 HTTP
来源：http://jlw.yj202588.top

aiohttp.ClientSession() 配合 async with
来源：http://odl.pycfn.com

[U28] Py：类型别名
来源：http://iys.shanyushiyangkeji.top

UserId = int
来源：http://hbf.daria6918.cn

[U29] Py：属性校验
来源：http://grz.ydjk.org.cn

@property 与 @x.setter 配合
来源：http://dbd.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://ycr.zhoulong.xyz

@dataclass(slots=True)
来源：http://usa.c1oappe.top

[U31] Py：单测
来源：http://wrf.ivvv.top

python -m pytest -q
来源：http://zkl.zdqjudy.top

[U32] Py：代码格式化
来源：http://zly.zdqjudy.top

ruff format . && ruff check --fix .
来源：http://zte.hongshengwenyu.top

[U33] Py：打包发布
来源：http://jzm.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://ung.mhx1999.top

[U34] Py：判断编码
来源：http://eds.yj202588.top

chardet.detect(raw)
来源：http://jvz.xinyue.icu

[U35] Py：发送邮件
来源：http://vye.yj202588.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gmp.9152youxi.cn

[U36] Py：定时任务
来源：http://mmx.vehdjk.com

schedule.every(10).minutes.do(job)
来源：http://zim.yuanzhike.top

[U37] Py：读写 Excel
来源：http://eqj.yfazqb.com

pandas.read_excel / DataFrame.to_excel
来源：http://yql.snrcjt.cn

[U38] Py：获取脚本所在目录
来源：http://gbd.pycfn.com

Path(__file__).resolve().parent
来源：http://frn.sweek.top

[U39] Py：判断是否在交互环境
来源：http://asr.gotoacloud.top

sys.stdout.isatty()
来源：http://zfy.quarkkingdee.top

[U40] Py：打印到标准错误
来源：http://nra.zycfv.cn

print("err", file=sys.stderr)
来源：http://tlb.sufxvd.cn

[U41] PHP：初始化 Composer 项目
来源：http://dcv.zhiwuduotai.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qit.xingfuxueyuan.xyz

[U42] PHP：PSR-4 自动加载
来源：http://hyz.snrcjt.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ssc.jlsjyb.cn

[U43] PHP：声明命名空间
来源：http://knk.jiagoushi.top

namespace App\Http;
来源：http://rci.316326.xyz

[U44] PHP：开启严格类型
来源：http://svp.tianlin.xyz

declare(strict_types=1);
来源：http://tao.nwbrower.top

[U45] PHP：类型声明与返回类型
来源：http://mcc.birdmap.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tca.quarkkingdee.top

[U46] PHP：可空类型
来源：http://pfv.tianlin.xyz

?string $name = null
来源：http://ecg.9152youxi.cn

[U47] PHP：联合类型
来源：http://xya.vehdjk.com

int|string $id
来源：http://wuu.cqqwz.cn

[U48] PHP：纯枚举
来源：http://qwz.sysykeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ynw.birdmap.top

[U49] PHP：只读属性
来源：http://kdd.ctjpmb.com

public readonly string $name
来源：http://tnv.feifeiyinyue.top

[U50] PHP：构造器属性提升
来源：http://jus.yj202588.top

public function __construct(private int $id) {}
来源：http://auo.chenjidiqi.icu

[U51] PHP：数组解构
来源：http://tid.hywenlv.cn

[$a, $b] = $arr;
来源：http://dbg.fehbvm.com

[U52] PHP：箭头函数
来源：http://bfc.hfpthk.cn

$double = fn($x) => $x * 2;
来源：http://ywd.wangdashe.top


<!-- 参考信息 -->