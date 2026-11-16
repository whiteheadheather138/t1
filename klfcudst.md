代发 wailian999

static int counter = 0;
来源：http://hzc.zhengqikj.top

[S29] C：变参函数
来源：http://odr.cucudq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xer.chenlongwang.top

[S30] C：头文件保护
来源：http://ldu.cdnleiting.top

#ifndef X_H
来源：http://zwh.yongpay.top

#define X_H
来源：http://iep.ydjk.org.cn

#endif
来源：http://ldb.hfpthk.cn

[S31] C++：Hello World
来源：http://kls.nanxuanxn.top

#include <iostream>
来源：http://fgu.jyoumei.cn

int main() { std::cout << "Hello\n"; }
来源：http://ris.cqqwz.cn

[S32] C++：字符串
来源：http://kqy.yueranfly.top

std::string s = "hi";  s += "!";
来源：http://awr.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://ntp.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://imw.mhx1999.top

[S34] C++：遍历 vector
来源：http://tns.zhengqikj.top

for (auto &x : v) { std::cout << x; }
来源：http://wpo.fanxiaobao.xyz

[S35] C++：map
来源：http://emp.pengpengdd.cyou

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pxb.aizwys.cn

[S36] C++：unordered_map
来源：http://ufh.tian-w.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ids.sufxvd.cn

[S37] C++：set
来源：http://ftr.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hfw.zhoulong.xyz

[S38] C++：排序
来源：http://kwk.hesvh.cn

std::sort(v.begin(), v.end());
来源：http://yhv.9152youxi.cn

[S39] C++：自定义比较器排序
来源：http://tla.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://smo.andypj.xyz

[S40] C++：查找元素
来源：http://ibg.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wya.yueranfly.top

[S41] C++：类与构造函数
来源：http://gye.yuxming.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aoy.ydzc1.top

[S42] C++：继承与虚函数
来源：http://som.yangfankeji.com

class B : public Base { public: void f() override {} };
来源：http://dmy.jyoumei.cn

[S43] C++：智能指针
来源：http://rwh.hammf.cn

auto p = std::make_unique<int>(5);
来源：http://bpo.havefunace.top

[S44] C++：引用传参
来源：http://lje.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://tua.redwolf501.top

[S45] C++：lambda
来源：http://hrs.ehwqpu.com

auto add = [](int a, int b) { return a + b; };
来源：http://doq.yuxming.cn

[S46] C++：函数模板
来源：http://mdu.andypj.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://scj.nanxuanxn.top

[S47] C++：结构化绑定遍历
来源：http://aln.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ujz.yfazqb.com

[S48] C++：逐行读文件
来源：http://hqv.pengpengdd.cyou

std::ifstream in("a.txt");  std::string line;
来源：http://rzs.gotoacloud.top

while (std::getline(in, line)) { }
来源：http://gkl.cdnleiting.top

[S49] C++：写文件
来源：http://czi.bbcook.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qtw.fzhhl.top

[S50] C++：格式化数字
来源：http://mqx.wangshuangyany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jtg.yvedp.cn

[S51] C++：显式类型转换
来源：http://ipa.guannengcc.top

static_cast<double>(a) / b
来源：http://ffi.mhx1999.top

[S52] C++：const 与 noexcept
来源：http://feg.vqdsnc.cn

int size() const noexcept { return n_; }
来源：http://fba.0kj1m.cn

[S53] C++：移动语义
来源：http://uzf.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://tjz.tianlin.xyz

[S54] C++：异常处理
来源：http://cfu.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sny.daxiang520.top

[S55] C++：结构化绑定
来源：http://sid.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ywa.uphjek.com

[S56] C++：optional
来源：http://ujn.xziqi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uoz.havefunace.top

[S57] C++：编译期常量
来源：http://dfb.jiagoushi.top

constexpr int N = 10;
来源：http://oxn.9152youxi.cn

[S58] C++：命名空间
来源：http://set.zdbjq.cn

namespace ns { int f() { return 1; } }
来源：http://fos.guannengcc.top

[S59] C++：静态断言
来源：http://few.shzxlz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gyf.cheryme.top

[S60] C++：遍历并删除元素
来源：http://cqi.meibo888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pxa.tian-w.cn

================================================================================
来源：http://rqa.aibaodan.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zce.cqqwz.cn

================================================================================
来源：http://hzm.sufxvd.cn

[T01] Kotlin：Hello World
来源：http://ayf.dianchejie.cn

println("Hello")
来源：http://alh.yuanzhike.top

[T02] Kotlin：变量
来源：http://skm.hnqzz.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lfi.snrcjt.cn

[T03] Kotlin：字符串模板
来源：http://blm.ehwqpu.com

"值: $b"
来源：http://hmr.shanyushiyangtech.top

[T04] Kotlin：空安全
来源：http://srm.nanxinkj.top

val n: String? = null;  n?.length
来源：http://apg.jinghuilouyu.cn

[T05] Kotlin：when 表达式
来源：http://yvg.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ihn.zhaomingkeji.xyz

[T06] Kotlin：集合映射
来源：http://qqp.andypj.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://yji.yongpay.top

[T07] Kotlin：集合过滤
来源：http://xhu.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gmg.daxiang520.top

[T08] Kotlin：数据类
来源：http://ywa.quarkkingdee.top

data class User(val name: String, val age: Int)
来源：http://oar.ehwqpu.com

[T09] Kotlin：扩展函数
来源：http://rld.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://ett.nanxuanxn.top

[T10] Kotlin：默认参数
来源：http://law.hnqzz.top

fun greet(name: String = "World") = "Hi $name"
来源：http://aaq.9152youxi.cn

[T11] Kotlin：协程
来源：http://nrj.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://acp.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://vko.meibo888.top

val (a, b) = Pair(1, 2)
来源：http://rrp.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://csg.ydzc1.top

val m = mapOf("a" to 1)
来源：http://ald.vehdjk.com

[T14] Kotlin：循环
来源：http://bmj.uphjek.com

for (i in 1..10) println(i)
来源：http://myy.yvedp.cn

[T15] Kotlin：接口
来源：http://zgc.xinyue.icu

interface Shape { fun area(): Double }
来源：http://uhd.hywenlv.cn

[T16] Swift：Hello World
来源：http://mes.gaohongyu789.top

print("Hello")
来源：http://asd.yvedp.cn

[T17] Swift：变量与常量
来源：http://iwz.zhijiandao.cn

var a = 1;  let b = 2
来源：http://kex.andypj.xyz

[T18] Swift：字符串插值
来源：http://cft.bjfxy.top

"值: \(b)"
来源：http://ful.aibaodan.cn

[T19] Swift：可选绑定
来源：http://yud.zhongyouzk.top

if let n = opt { print(n) }
来源：http://hpx.snrcjt.cn

[T20] Swift：数组操作
来源：http://wyb.haohaochexian.top

var a = [1, 2, 3];  a.append(4)
来源：http://ikh.quarkkingdee.top

[T21] Swift：遍历
来源：http://xjn.ybcxt.top

for x in a { print(x) }
来源：http://ypx.chenlongwang.top

[T22] Swift：字典
来源：http://rky.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ycy.52xcode.cn

[T23] Swift：函数
来源：http://zbt.zhijiandao.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ked.yuxming.cn

[T24] Swift：闭包
来源：http://zve.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://efs.yueranfly.top

[T25] Swift：结构体
来源：http://sgv.xuetiantiany.cn

struct P { var x: Int }
来源：http://sgl.c1oappe.top

[T26] Swift：类与重写
来源：http://rff.cheryme.top

class A: Base { override func f() {} }
来源：http://swq.ivvv.top

[T27] Swift：错误处理
来源：http://psg.sjlbkw.cn

do { try f() } catch { print(error) }
来源：http://otm.gzhubu.top

[T28] Swift：枚举
来源：http://rve.gogol.net.cn

enum Color { case red, green }
来源：http://icd.hfpthk.cn

[T29] Swift：guard 提前返回
来源：http://axw.yuxming.cn

guard let x = opt else { return }
来源：http://fgr.bbcook.cn

[T30] Swift：协议
来源：http://ixe.andypj.xyz

protocol Shape { func area() -> Double }
来源：http://trs.xuanzx.com

[T31] Lua：Hello World
来源：http://dzs.sysykeji.top

print("Hello")
来源：http://knd.meibo888.top

[T32] Lua：局部变量
来源：http://hwx.yanxiufei.cn

local a = 1
来源：http://wea.gogol.net.cn

[T33] Lua：表（数组）
来源：http://dmx.sjlbkw.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fcp.shzxlz.cn

[T34] Lua：遍历表
来源：http://xiu.zhixingplan.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rzh.yonumen.top

[T35] Lua：字典表
来源：http://nga.jinqigfzy.top

local d = { a = 1 };  d.b = 2
来源：http://bnl.jianghu66.top

[T36] Lua：函数
来源：http://hhm.birdmap.top

function add(a, b) return a + b end
来源：http://evf.uphjek.com

[T37] Lua：字符串拼接
来源：http://itk.hywenlv.cn

"a" .. "b"
来源：http://jaf.sjlbkw.cn

[T38] Lua：条件
来源：http://ake.smart0.xyz

if x > 0 then print("正") end
来源：http://ygd.yuxming.cn

[T39] Lua：模式匹配
来源：http://xqw.cashguo.top

string.find(s, "%d+")
来源：http://epn.shanyushiyangkeji.top

[T40] Lua：元表
来源：http://usm.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://njm.xingfuxueyuan.xyz

[T41] Perl：Hello World
来源：http://ybl.jianghu66.top

print "Hello\n";
来源：http://tfs.zhaomingkeji.xyz

[T42] Perl：变量类型
来源：http://hoy.zhixingplan.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pri.daria6918.cn

[T43] Perl：字符串插值
来源：http://hta.fengsongda.top

"值: $a"
来源：http://dbm.jinqigufen.top

[T44] Perl：条件
来源：http://uan.sjlbkw.cn

if ($a > 0) { print "正"; }
来源：http://iqk.fehbvm.com

[T45] Perl：数组遍历
来源：http://tef.cdnleiting.top

for my $x (@arr) { print $x; }
来源：http://uug.guowangkeji.top

[T46] Perl：哈希操作
来源：http://nti.vehdjk.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://svc.tianlin.xyz

[T47] Perl：正则捕获
来源：http://esn.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://yjr.cheryme.top

[T48] Perl：正则替换
来源：http://wqz.xziqi.cn

$s =~ s/old/new/g;
来源：http://ufy.cashguo.top

[T49] Perl：函数
来源：http://krs.feifeiyinyue.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dit.yongpay.top

[T50] Perl：逐行读文件
来源：http://zme.epnwcf.com

open my $fh, "<", "a.txt" or die $!;
来源：http://yuu.xuanzx.com

while (my $line = <$fh>) { print $line; }
来源：http://nby.yj20258.top

[T51] Scala：Hello World
来源：http://tro.hongshengwenyu.top

println("Hello")
来源：http://ubr.fengsongda.top

[T52] Scala：变量
来源：http://jwx.jinqigfzy.top

val a = 1;  var b = 2
来源：http://xbs.yuxming.cn

[T53] Scala：字符串插值
来源：http://ylb.guannengcc.top

s"值: $b"
来源：http://roo.yj202588.top

[T54] Scala：集合映射
来源：http://wps.kuanghao11.cn

List(1, 2, 3).map(_ * 2)
来源：http://ban.ydjk.org.cn

[T55] Scala：集合过滤
来源：http://pjh.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://yzf.chenlongwang.top

[T56] Scala：样例类
来源：http://lpr.0kj1m.cn

case class User(name: String, age: Int)
来源：http://zyf.haohaochexian.top

[T57] Scala：模式匹配
来源：http://naq.uphjek.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://cuf.feifeiyinyue.top

[T58] Scala：函数定义
来源：http://vue.kuanghao11.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hxf.yuxming.cn

[T59] Scala：循环
来源：http://pur.0kj1m.cn

for (i <- 1 to 10) println(i)
来源：http://sdv.xylfe.cn

[T60] Scala：折叠
来源：http://wwi.hammf.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qtk.epnwcf.com

================================================================================
来源：http://qcc.yj20258888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://czn.zhixingplan.top

================================================================================
来源：http://nhw.gogol.net.cn

[U01] Py：创建虚拟环境
来源：http://shx.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://qsp.ydzc1.top

[U02] Py：导出 / 安装依赖
来源：http://ebf.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://syl.hammf.cn

[U03] Py：加载 .env 配置
来源：http://fik.fktsv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://njb.haohaochexian.top

[U04] Py：变量调试打印
来源：http://zft.tian-w.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vxk.yanxiufei.cn

[U05] Py：列表去重且保序
来源：http://unk.jinqigfzy.top

list(dict.fromkeys(arr))
来源：http://cky.sysykeji.top

[U06] Py：合并两个字典
来源：http://gdw.fehbvm.com

{**a, **b}
来源：http://ynl.ydzc1.top

[U07] Py：反转字典键值
来源：http://qnx.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://wib.zhongyouzk.top

[U08] Py：展平二维列表
来源：http://hdr.xingfuxueyuan.xyz

[y for x in nested for y in x]
来源：http://cnx.cdnleiting.top

[U09] Py：字典取最大值的键
来源：http://qrq.zhengqikj.top

max(d, key=d.get)
来源：http://oyv.ydzc1.top

[U10] Py：按值排序字典
来源：http://voi.yfazqb.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dba.c1oappe.top

[U11] Py：生成器表达式
来源：http://jxd.gogol.net.cn

(x * 2 for x in arr)
来源：http://ebk.guowangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://wlu.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://yna.shzxlz.cn

[U13] Py：固定长度队列
来源：http://qnn.jinyuanbaomall.cn

deque(maxlen=10)
来源：http://peq.jinghuilouyu.cn

[U14] Py：分组收集到列表
来源：http://bbm.yonumen.top

defaultdict(list)
来源：http://rsx.snrcjt.cn

[U15] Py：高精度计时
来源：http://meb.316326.xyz

t = time.perf_counter()
来源：http://doe.redwolf501.top

[U16] Py：命令行参数解析
来源：http://old.shzxlz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mpy.zhiwuduotai.top

[U17] Py：初始化日志
来源：http://atd.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://ovk.0kj1m.cn

[U18] Py：预编译正则
来源：http://khm.cashguo.top

pat = re.compile(r"\d+")
来源：http://vph.316326.xyz

[U19] Py：正则替换带回调
来源：http://qfa.daria6918.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xar.tianlin.xyz

[U20] Py：缓存函数结果
来源：http://rme.ctjpmb.com

@functools.lru_cache(maxsize=None)
来源：http://lod.kuanghao11.cn

[U21] Py：自定义上下文管理器
来源：http://kht.zdqjudy.top

@contextlib.contextmanager
来源：http://cpt.yvedp.cn

[U22] Py：矩阵转置
来源：http://kpa.fengsongda.top

list(zip(*m))
来源：http://bxp.sysykeji.top

[U23] Py：分块读取大文件
来源：http://byt.52xcode.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qom.aibaodan.cn

[U24] Py：路径操作
来源：http://riz.fktsv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ooa.ppjwa.cn

[U25] Py：CSV 按字典读
来源：http://fxw.bjfxy.top

csv.DictReader(f)
来源：http://ihw.epnwcf.com

[U26] Py：并发下载
来源：http://geq.jqgufenzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pgy.ehwqpu.com

[U27] Py：异步 HTTP
来源：http://hki.svipenyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://hry.jqgufenzy.top

[U28] Py：类型别名
来源：http://szn.9152youxi.cn

UserId = int
来源：http://bat.hesvh.cn

[U29] Py：属性校验
来源：http://ijn.zhaomingkeji.xyz

@property 与 @x.setter 配合
来源：http://egy.cdnleiting.top

[U30] Py：数据类
来源：http://nmi.cheryme.top

@dataclass(slots=True)
来源：http://rrt.fehbvm.com

[U31] Py：单测
来源：http://bep.fktsv.cn

python -m pytest -q
来源：http://ocq.vehdjk.com

[U32] Py：代码格式化
来源：http://urx.gzhubu.top

ruff format . && ruff check --fix .
来源：http://eiq.redwolf501.top

[U33] Py：打包发布
来源：http://foz.gaohongyu789.top

python -m build  （依赖 pyproject.toml）
来源：http://sxy.tian-w.cn

[U34] Py：判断编码
来源：http://oun.yongpay.top

chardet.detect(raw)
来源：http://egf.chenlongwang.top

[U35] Py：发送邮件
来源：http://ycs.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ofc.hcnkem.com

[U36] Py：定时任务
来源：http://hqv.hongshengwenyu.top

schedule.every(10).minutes.do(job)
来源：http://vqk.fktsv.cn

[U37] Py：读写 Excel
来源：http://nqx.jqgfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://xhc.sufxvd.cn

[U38] Py：获取脚本所在目录
来源：http://btf.hfpthk.cn

Path(__file__).resolve().parent
来源：http://dmt.havefunace.top

[U39] Py：判断是否在交互环境
来源：http://hsl.jyoumei.cn

sys.stdout.isatty()
来源：http://vgu.ydjk.org.cn

[U40] Py：打印到标准错误
来源：http://wga.hesvh.cn

print("err", file=sys.stderr)
来源：http://vkb.zycfv.cn

[U41] PHP：初始化 Composer 项目
来源：http://wth.feifeiyinyue.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vzg.xziqi.cn

[U42] PHP：PSR-4 自动加载
来源：http://hks.yj20258888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xru.smart0.xyz

[U43] PHP：声明命名空间
来源：http://pcp.sweek.top

namespace App\Http;
来源：http://ipy.jinqigufen.top

[U44] PHP：开启严格类型
来源：http://vss.haohaochexian.top

declare(strict_types=1);
来源：http://jrm.shzxlz.cn

[U45] PHP：类型声明与返回类型
来源：http://txd.yvedp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xca.hongshengwenyu.top

[U46] PHP：可空类型
来源：http://qsu.ydjk.org.cn

?string $name = null
来源：http://nbs.fzhhl.top

[U47] PHP：联合类型
来源：http://uhg.jinqigufen.top

int|string $id
来源：http://vqm.cqqwz.cn

[U48] PHP：纯枚举
来源：http://qir.hongshengwenyu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xjk.nanxuanxn.top

[U49] PHP：只读属性
来源：http://tya.hywenlv.cn

public readonly string $name
来源：http://qvq.52xcode.cn

[U50] PHP：构造器属性提升
来源：http://pfk.jlsjyb.cn

public function __construct(private int $id) {}
来源：http://wfx.tian-w.cn

[U51] PHP：数组解构
来源：http://hgu.hesvh.cn

[$a, $b] = $arr;
来源：http://ihz.wangdashe.top

[U52] PHP：箭头函数
来源：http://ivn.feifeiyinyue.top

$double = fn($x) => $x * 2;
来源：http://wqy.c1oappe.top


<!-- 参考信息 -->