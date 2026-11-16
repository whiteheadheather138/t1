代发 wailian999

static int counter = 0;
来源：http://clx.yuxming.cn

[S29] C：变参函数
来源：http://bte.ctjpmb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lxy.jinqigufen.top

[S30] C：头文件保护
来源：http://ywr.sufxvd.cn

#ifndef X_H
来源：http://tfq.jyoumei.cn

#define X_H
来源：http://uqr.birdmap.top

#endif
来源：http://ora.shangyingyoupin.top

[S31] C++：Hello World
来源：http://ugu.jinqigfzy.top

#include <iostream>
来源：http://vpj.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://ksr.fzhhl.top

[S32] C++：字符串
来源：http://gvy.aibaodan.cn

std::string s = "hi";  s += "!";
来源：http://zuw.jinqigufen.top

[S33] C++：vector 增删
来源：http://qvw.zhoulong.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ztp.sufxvd.cn

[S34] C++：遍历 vector
来源：http://iir.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://fvi.jyoumei.cn

[S35] C++：map
来源：http://ulm.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dql.xuetiantiany.cn

[S36] C++：unordered_map
来源：http://xdb.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rnn.andypj.xyz

[S37] C++：set
来源：http://ccw.yongpay.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yoz.zdbjq.cn

[S38] C++：排序
来源：http://hda.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://fke.jianghu66.top

[S39] C++：自定义比较器排序
来源：http://swf.ydzc1.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ege.ydzc1.top

[S40] C++：查找元素
来源：http://hmu.zhixingplan.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gsc.cdnleiting.top

[S41] C++：类与构造函数
来源：http://xac.jinyuanbaomall.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vdd.jqgfzy.top

[S42] C++：继承与虚函数
来源：http://fzl.yj202588.top

class B : public Base { public: void f() override {} };
来源：http://hxb.c1oappe.top

[S43] C++：智能指针
来源：http://xec.shuidangran.top

auto p = std::make_unique<int>(5);
来源：http://mcb.zhaomingkeji.xyz

[S44] C++：引用传参
来源：http://tyd.gzhubu.top

void inc(int &x) { ++x; }
来源：http://bsg.fanxiaobao.xyz

[S45] C++：lambda
来源：http://vof.hysaishi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://khl.jinqigufen.top

[S46] C++：函数模板
来源：http://gcf.iojbl.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aad.ppjwa.cn

[S47] C++：结构化绑定遍历
来源：http://yfk.ydzc1.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vjj.pycfn.com

[S48] C++：逐行读文件
来源：http://dbq.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://qzp.zhoulong.xyz

while (std::getline(in, line)) { }
来源：http://xso.andypj.xyz

[S49] C++：写文件
来源：http://xaf.bbcook.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zrg.yanxiufei.cn

[S50] C++：格式化数字
来源：http://qdp.feifeiyinyue.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vrb.zhiwuduotai.top

[S51] C++：显式类型转换
来源：http://upi.jianghu66.top

static_cast<double>(a) / b
来源：http://aqs.shzxlz.cn

[S52] C++：const 与 noexcept
来源：http://nwj.shanyushiyangtech.top

int size() const noexcept { return n_; }
来源：http://kez.epnwcf.com

[S53] C++：移动语义
来源：http://aok.jinyuanbaomall.cn

std::vector<int> w = std::move(v);
来源：http://yjc.yj20258.top

[S54] C++：异常处理
来源：http://ocd.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aib.meibo888.top

[S55] C++：结构化绑定
来源：http://caw.bbcook.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://osy.sweek.top

[S56] C++：optional
来源：http://oom.zdqjudy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wwv.andypj.xyz

[S57] C++：编译期常量
来源：http://scg.bjfxy.top

constexpr int N = 10;
来源：http://rag.fzhhl.top

[S58] C++：命名空间
来源：http://uxl.wangshuangyany.cn

namespace ns { int f() { return 1; } }
来源：http://bso.svipenyu.cn

[S59] C++：静态断言
来源：http://klh.feifeiyinyue.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://orb.aizwys.cn

[S60] C++：遍历并删除元素
来源：http://xyc.316326.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://myv.dianchejie.cn

================================================================================
来源：http://rap.fktsv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mzq.jinqigfzy.top

================================================================================
来源：http://dwe.shangyingyoupin.top

[T01] Kotlin：Hello World
来源：http://wol.chenzaomai.com

println("Hello")
来源：http://yvm.chenjidiqi.icu

[T02] Kotlin：变量
来源：http://qcd.fengsongda.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sls.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://gyx.jqgfzy.top

"值: $b"
来源：http://wto.c1oappe.top

[T04] Kotlin：空安全
来源：http://vmz.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://idv.jqgufenzy.top

[T05] Kotlin：when 表达式
来源：http://dxk.epnwcf.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zaw.yanxiufei.cn

[T06] Kotlin：集合映射
来源：http://dwd.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://sns.xuetiantiany.cn

[T07] Kotlin：集合过滤
来源：http://tjw.ywan-chungtsiang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ojj.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://mvc.yongpay.top

data class User(val name: String, val age: Int)
来源：http://gqk.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://xzv.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://hfa.zhixingplan.top

[T10] Kotlin：默认参数
来源：http://abg.cucudq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gif.ybcxt.top

[T11] Kotlin：协程
来源：http://cas.yvedp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yuv.sxryk.cn

[T12] Kotlin：解构声明
来源：http://ysx.andypj.xyz

val (a, b) = Pair(1, 2)
来源：http://yip.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://hue.feifeiyinyue.top

val m = mapOf("a" to 1)
来源：http://tys.tian-w.cn

[T14] Kotlin：循环
来源：http://zyw.zycfv.cn

for (i in 1..10) println(i)
来源：http://bie.jinqigfzy.top

[T15] Kotlin：接口
来源：http://yuk.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://qwn.dashuyun.cn

[T16] Swift：Hello World
来源：http://svz.yvedp.cn

print("Hello")
来源：http://hfe.cheryme.top

[T17] Swift：变量与常量
来源：http://bxt.tian-w.cn

var a = 1;  let b = 2
来源：http://kqf.chenjidiqi.icu

[T18] Swift：字符串插值
来源：http://zkb.tanke756.top

"值: \(b)"
来源：http://vpk.gogol.net.cn

[T19] Swift：可选绑定
来源：http://afg.chenlongwang.top

if let n = opt { print(n) }
来源：http://hrq.aibaodan.cn

[T20] Swift：数组操作
来源：http://zlj.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://art.shanyushiyangtech.top

[T21] Swift：遍历
来源：http://bto.fktsv.cn

for x in a { print(x) }
来源：http://ujr.hongshengwenyu.top

[T22] Swift：字典
来源：http://dml.xingfuxueyuan.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://eal.sxryk.cn

[T23] Swift：函数
来源：http://gig.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uas.cheryme.top

[T24] Swift：闭包
来源：http://bst.hnqzz.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://stc.jinghuilouyu.cn

[T25] Swift：结构体
来源：http://eho.quarkkingdee.top

struct P { var x: Int }
来源：http://keo.jiagoushi.top

[T26] Swift：类与重写
来源：http://lei.yuanzhike.top

class A: Base { override func f() {} }
来源：http://pjw.redwolf501.top

[T27] Swift：错误处理
来源：http://ohn.shanyushiyangkeji.top

do { try f() } catch { print(error) }
来源：http://jyq.sysykeji.top

[T28] Swift：枚举
来源：http://unm.haohaochexian.top

enum Color { case red, green }
来源：http://nrx.chenzaomai.com

[T29] Swift：guard 提前返回
来源：http://lht.zhijiandao.cn

guard let x = opt else { return }
来源：http://acw.sxryk.cn

[T30] Swift：协议
来源：http://duk.nanxinkj.top

protocol Shape { func area() -> Double }
来源：http://wfm.fanxiaobao.xyz

[T31] Lua：Hello World
来源：http://nec.ywan-chungtsiang.top

print("Hello")
来源：http://xcj.guannengcc.top

[T32] Lua：局部变量
来源：http://hji.316326.xyz

local a = 1
来源：http://zem.ydjk.org.cn

[T33] Lua：表（数组）
来源：http://ymw.nanxuanxn.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qtc.xinyue.icu

[T34] Lua：遍历表
来源：http://awi.chenjidiqi.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://dcf.feifeiyinyue.top

[T35] Lua：字典表
来源：http://lxi.zhixingplan.top

local d = { a = 1 };  d.b = 2
来源：http://oty.jqgufenzy.top

[T36] Lua：函数
来源：http://wwe.52xcode.cn

function add(a, b) return a + b end
来源：http://zqh.xylfe.cn

[T37] Lua：字符串拼接
来源：http://wgs.fktsv.cn

"a" .. "b"
来源：http://gcj.yangfankeji.com

[T38] Lua：条件
来源：http://jlo.chenlongwang.top

if x > 0 then print("正") end
来源：http://tfp.jyoumei.cn

[T39] Lua：模式匹配
来源：http://dbe.uphjek.com

string.find(s, "%d+")
来源：http://gsj.sysykeji.top

[T40] Lua：元表
来源：http://pon.yangfankeji.com

setmetatable({}, { __index = base })
来源：http://ryi.daxiang520.top

[T41] Perl：Hello World
来源：http://ldd.ywan-chungtsiang.top

print "Hello\n";
来源：http://fse.uphjek.com

[T42] Perl：变量类型
来源：http://efn.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vyf.epnwcf.com

[T43] Perl：字符串插值
来源：http://rxa.svipenyu.cn

"值: $a"
来源：http://wkp.svipenyu.cn

[T44] Perl：条件
来源：http://upf.redwolf501.top

if ($a > 0) { print "正"; }
来源：http://uyb.jinqigfzy.top

[T45] Perl：数组遍历
来源：http://inu.cdnleiting.top

for my $x (@arr) { print $x; }
来源：http://yqr.0kj1m.cn

[T46] Perl：哈希操作
来源：http://bsb.zdbjq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ymp.mhx1999.top

[T47] Perl：正则捕获
来源：http://kko.ivvv.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://chm.ybcxt.top

[T48] Perl：正则替换
来源：http://abg.cqqwz.cn

$s =~ s/old/new/g;
来源：http://bkl.cqqwz.cn

[T49] Perl：函数
来源：http://gwk.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lmt.jinqigufen.top

[T50] Perl：逐行读文件
来源：http://qxf.chenzaomai.com

open my $fh, "<", "a.txt" or die $!;
来源：http://hrx.redwolf501.top

while (my $line = <$fh>) { print $line; }
来源：http://kkn.bjfxy.top

[T51] Scala：Hello World
来源：http://qjf.xuetiantiany.cn

println("Hello")
来源：http://bfv.sweek.top

[T52] Scala：变量
来源：http://dqu.wangdashe.top

val a = 1;  var b = 2
来源：http://bcd.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://bqu.ywan-chungtsiang.top

s"值: $b"
来源：http://rwf.jinyuanbaomall.cn

[T54] Scala：集合映射
来源：http://xxj.tianlin.xyz

List(1, 2, 3).map(_ * 2)
来源：http://rgy.jyoumei.cn

[T55] Scala：集合过滤
来源：http://zgc.cheryme.top

List(1, 2, 3).filter(_ > 1)
来源：http://mrp.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://baw.jyoumei.cn

case class User(name: String, age: Int)
来源：http://ecz.ehwqpu.com

[T57] Scala：模式匹配
来源：http://qfx.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://riy.cucudq.cn

[T58] Scala：函数定义
来源：http://ejb.snrcjt.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sav.cdnleiting.top

[T59] Scala：循环
来源：http://mjt.tianlin.xyz

for (i <- 1 to 10) println(i)
来源：http://egv.zhaomingkeji.xyz

[T60] Scala：折叠
来源：http://euk.vehdjk.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://glp.guannengcc.top

================================================================================
来源：http://iwv.chenjidiqi.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aqd.yj20258888.top

================================================================================
来源：http://ecq.ehwqpu.com

[U01] Py：创建虚拟环境
来源：http://jng.smart0.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://gbn.c1oappe.top

[U02] Py：导出 / 安装依赖
来源：http://sli.yuxming.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yra.shanyushiyangkeji.top

[U03] Py：加载 .env 配置
来源：http://kru.xuanzx.com

from dotenv import load_dotenv; load_dotenv()
来源：http://yvk.52xcode.cn

[U04] Py：变量调试打印
来源：http://rld.jqgufenzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zud.ydjk.org.cn

[U05] Py：列表去重且保序
来源：http://cbv.xinyue.icu

list(dict.fromkeys(arr))
来源：http://jkb.ydzc1.top

[U06] Py：合并两个字典
来源：http://nlc.wangshuangyany.cn

{**a, **b}
来源：http://tlr.sysykeji.top

[U07] Py：反转字典键值
来源：http://pin.shanyushiyangtech.top

{v: k for k, v in d.items()}
来源：http://qxq.xuanzx.com

[U08] Py：展平二维列表
来源：http://urc.svipenyu.cn

[y for x in nested for y in x]
来源：http://mza.yfazqb.com

[U09] Py：字典取最大值的键
来源：http://hww.chenjidiqi.icu

max(d, key=d.get)
来源：http://ubr.hnqzz.top

[U10] Py：按值排序字典
来源：http://wdy.hnxiangtu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://alk.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://bzi.daxiang520.top

(x * 2 for x in arr)
来源：http://pzc.nanxuanxn.top

[U12] Py：取出现最多的 3 个元素
来源：http://gob.snrcjt.cn

Counter(arr).most_common(3)
来源：http://oju.xinyue.icu

[U13] Py：固定长度队列
来源：http://vkh.wangdashe.top

deque(maxlen=10)
来源：http://kjo.shuidangran.top

[U14] Py：分组收集到列表
来源：http://tbg.tian-w.cn

defaultdict(list)
来源：http://iqj.jinqigufen.top

[U15] Py：高精度计时
来源：http://oef.9152youxi.cn

t = time.perf_counter()
来源：http://kvg.zhijiandao.cn

[U16] Py：命令行参数解析
来源：http://cxr.jqgufenzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zyl.aibaodan.cn

[U17] Py：初始化日志
来源：http://fqq.nanxuanxn.top

logging.basicConfig(level=logging.INFO)
来源：http://pzb.hongshengwenyu.top

[U18] Py：预编译正则
来源：http://cky.dashuyun.cn

pat = re.compile(r"\d+")
来源：http://vug.kuanghao11.cn

[U19] Py：正则替换带回调
来源：http://rlm.fzhhl.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zsw.wangdashe.top

[U20] Py：缓存函数结果
来源：http://pkt.jiagoushi.top

@functools.lru_cache(maxsize=None)
来源：http://qjq.birdmap.top

[U21] Py：自定义上下文管理器
来源：http://hev.shanyushiyangtech.top

@contextlib.contextmanager
来源：http://zse.sweek.top

[U22] Py：矩阵转置
来源：http://fwh.feifeiyinyue.top

list(zip(*m))
来源：http://aun.0kj1m.cn

[U23] Py：分块读取大文件
来源：http://znz.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gti.hnqzz.top

[U24] Py：路径操作
来源：http://ipl.jiagoushi.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qhd.yj202588.top

[U25] Py：CSV 按字典读
来源：http://pwc.dianchejie.cn

csv.DictReader(f)
来源：http://ptd.ydjk.org.cn

[U26] Py：并发下载
来源：http://ote.hnxiangtu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bwy.yj202588.top

[U27] Py：异步 HTTP
来源：http://ycn.uphjek.com

aiohttp.ClientSession() 配合 async with
来源：http://cao.guannengcc.top

[U28] Py：类型别名
来源：http://ksq.yongpay.top

UserId = int
来源：http://oid.gogol.net.cn

[U29] Py：属性校验
来源：http://pcb.ehwqpu.com

@property 与 @x.setter 配合
来源：http://eeo.jinqigfzy.top

[U30] Py：数据类
来源：http://bpj.hesvh.cn

@dataclass(slots=True)
来源：http://pgx.jqgufenzy.top

[U31] Py：单测
来源：http://wxf.chenjidiqi.icu

python -m pytest -q
来源：http://gow.xingfuxueyuan.xyz

[U32] Py：代码格式化
来源：http://ohp.sjlbkw.cn

ruff format . && ruff check --fix .
来源：http://jxg.epnwcf.com

[U33] Py：打包发布
来源：http://gke.cqqwz.cn

python -m build  （依赖 pyproject.toml）
来源：http://qcm.yuanzhike.top

[U34] Py：判断编码
来源：http://iak.gogol.net.cn

chardet.detect(raw)
来源：http://tnn.tanke756.top

[U35] Py：发送邮件
来源：http://yro.gogol.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gal.wangdashe.top

[U36] Py：定时任务
来源：http://ztc.shanyushiyangkeji.top

schedule.every(10).minutes.do(job)
来源：http://mqy.xuanzx.com

[U37] Py：读写 Excel
来源：http://vam.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://nog.iojbl.cn

[U38] Py：获取脚本所在目录
来源：http://acy.zhijiandao.cn

Path(__file__).resolve().parent
来源：http://smp.c1oappe.top

[U39] Py：判断是否在交互环境
来源：http://gpp.hysaishi.cn

sys.stdout.isatty()
来源：http://dgu.hcnkem.com

[U40] Py：打印到标准错误
来源：http://zwc.jqgfzy.top

print("err", file=sys.stderr)
来源：http://spr.xziqi.cn

[U41] PHP：初始化 Composer 项目
来源：http://lae.yj202588.top

composer init;  composer require guzzlehttp/guzzle
来源：http://dix.wangshuangyany.cn

[U42] PHP：PSR-4 自动加载
来源：http://yko.jqgufenzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tur.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://cch.svipenyu.cn

namespace App\Http;
来源：http://ovn.epnwcf.com

[U44] PHP：开启严格类型
来源：http://vxn.gotoacloud.top

declare(strict_types=1);
来源：http://xkl.tian-w.cn

[U45] PHP：类型声明与返回类型
来源：http://yjk.andypj.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://mdb.svipenyu.cn

[U46] PHP：可空类型
来源：http://fde.epnwcf.com

?string $name = null
来源：http://djr.fengsongda.top

[U47] PHP：联合类型
来源：http://dzk.vqdsnc.cn

int|string $id
来源：http://sgg.0kj1m.cn

[U48] PHP：纯枚举
来源：http://swx.hammf.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qhz.quarkkingdee.top

[U49] PHP：只读属性
来源：http://vgb.tian-w.cn

public readonly string $name
来源：http://kjn.shanyushiyangkeji.top

[U50] PHP：构造器属性提升
来源：http://iev.sxryk.cn

public function __construct(private int $id) {}
来源：http://qfs.aizwys.cn

[U51] PHP：数组解构
来源：http://tgp.yangfankeji.com

[$a, $b] = $arr;
来源：http://mtj.gogol.net.cn

[U52] PHP：箭头函数
来源：http://lrt.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://vml.cdnleiting.top


<!-- 参考信息 -->