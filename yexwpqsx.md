代发 wailian999

memset(a, 0, sizeof a);
来源：http://huv.yuanzhike.top

[S27] C：定义常量
来源：http://xkz.dianchejie.cn

const double PI = 3.14159;
来源：http://hrp.0kj1m.cn

[S28] C：静态变量
来源：http://ibj.iojbl.cn

static int counter = 0;
来源：http://kgz.zhongyouzk.top

[S29] C：变参函数
来源：http://ewc.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iqr.xylfe.cn

[S30] C：头文件保护
来源：http://tms.yongpay.top

#ifndef X_H
来源：http://jvo.xziqi.cn

#define X_H
来源：http://yty.jqgufenzy.top

#endif
来源：http://pcy.9152youxi.cn

[S31] C++：Hello World
来源：http://qru.cashguo.top

#include <iostream>
来源：http://nxq.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://don.gaohongyu789.top

[S32] C++：字符串
来源：http://ymm.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://lpd.ybcxt.top

[S33] C++：vector 增删
来源：http://azl.tian-w.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uqg.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://ivc.smart0.xyz

for (auto &x : v) { std::cout << x; }
来源：http://vue.zhijiandao.cn

[S35] C++：map
来源：http://tpv.tian-w.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zcu.zhiwuduotai.top

[S36] C++：unordered_map
来源：http://uew.tian-w.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lck.c1oappe.top

[S37] C++：set
来源：http://cxk.yj202588.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gnm.ctjpmb.com

[S38] C++：排序
来源：http://khv.cucudq.cn

std::sort(v.begin(), v.end());
来源：http://wrk.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://sks.jinyuanbaomall.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rmo.tarul.cn

[S40] C++：查找元素
来源：http://jul.jqgufenzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kpp.jqgfzy.top

[S41] C++：类与构造函数
来源：http://fum.ppjwa.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://grm.svipenyu.cn

[S42] C++：继承与虚函数
来源：http://udr.tian-w.cn

class B : public Base { public: void f() override {} };
来源：http://ymm.andypj.xyz

[S43] C++：智能指针
来源：http://vgx.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://buf.sufxvd.cn

[S44] C++：引用传参
来源：http://eqz.nwbrower.top

void inc(int &x) { ++x; }
来源：http://jfd.cqqwz.cn

[S45] C++：lambda
来源：http://anj.daria6918.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jcv.guowangkeji.top

[S46] C++：函数模板
来源：http://wyx.jiagoushi.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xyg.ppjwa.cn

[S47] C++：结构化绑定遍历
来源：http://jdu.zdqjudy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wll.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://vph.fzhhl.top

std::ifstream in("a.txt");  std::string line;
来源：http://xul.fktsv.cn

while (std::getline(in, line)) { }
来源：http://dkk.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://coa.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nqx.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://lhh.xingfuxueyuan.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xtv.yj20258.top

[S51] C++：显式类型转换
来源：http://gvb.fktsv.cn

static_cast<double>(a) / b
来源：http://ngo.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://vzw.fengsongda.top

int size() const noexcept { return n_; }
来源：http://tsr.gogol.net.cn

[S53] C++：移动语义
来源：http://uyu.hcnkem.com

std::vector<int> w = std::move(v);
来源：http://rgw.ppjwa.cn

[S54] C++：异常处理
来源：http://ord.andypj.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wrz.pengpengdd.cyou

[S55] C++：结构化绑定
来源：http://rna.shanyushiyangtech.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bra.havefunace.top

[S56] C++：optional
来源：http://ifs.fktsv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://koi.zdqjudy.top

[S57] C++：编译期常量
来源：http://rfx.xuetiantiany.cn

constexpr int N = 10;
来源：http://pnr.aibaodan.cn

[S58] C++：命名空间
来源：http://cii.gogol.net.cn

namespace ns { int f() { return 1; } }
来源：http://cmp.yueranfly.top

[S59] C++：静态断言
来源：http://nmb.sysykeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://imu.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://hku.ehwqpu.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rqn.316326.xyz

================================================================================
来源：http://jli.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://apn.fzhhl.top

================================================================================
来源：http://rot.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://qrx.uphjek.com

println("Hello")
来源：http://udx.chenzaomai.com

[T02] Kotlin：变量
来源：http://czq.uphjek.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://byp.daria6918.cn

[T03] Kotlin：字符串模板
来源：http://hle.birdmap.top

"值: $b"
来源：http://qub.fehbvm.com

[T04] Kotlin：空安全
来源：http://rph.yj202588.top

val n: String? = null;  n?.length
来源：http://akc.yonumen.top

[T05] Kotlin：when 表达式
来源：http://jis.cqqwz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ndi.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://rxo.ivvv.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bhg.yj20258888.top

[T07] Kotlin：集合过滤
来源：http://udr.birdmap.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mkr.ctjpmb.com

[T08] Kotlin：数据类
来源：http://mwq.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://qev.bjfxy.top

[T09] Kotlin：扩展函数
来源：http://ubw.gaohongyu789.top

fun String.exclaim() = this + "!"
来源：http://psx.xylfe.cn

[T10] Kotlin：默认参数
来源：http://def.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lqg.pycfn.com

[T11] Kotlin：协程
来源：http://xuv.jiagoushi.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://cgo.mhx1999.top

[T12] Kotlin：解构声明
来源：http://pxr.jiagoushi.top

val (a, b) = Pair(1, 2)
来源：http://uxc.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://isj.jqgfzy.top

val m = mapOf("a" to 1)
来源：http://csz.hywenlv.cn

[T14] Kotlin：循环
来源：http://mdz.yfazqb.com

for (i in 1..10) println(i)
来源：http://bro.haohaochexian.top

[T15] Kotlin：接口
来源：http://svl.cashguo.top

interface Shape { fun area(): Double }
来源：http://tug.ydzc1.top

[T16] Swift：Hello World
来源：http://ajx.gogol.net.cn

print("Hello")
来源：http://xvg.shangyingyoupin.top

[T17] Swift：变量与常量
来源：http://jsj.zhengqikj.top

var a = 1;  let b = 2
来源：http://sva.andypj.xyz

[T18] Swift：字符串插值
来源：http://ycq.zhiwuduotai.top

"值: \(b)"
来源：http://nxm.nanxinkj.top

[T19] Swift：可选绑定
来源：http://uba.tianlin.xyz

if let n = opt { print(n) }
来源：http://bbp.pengpengdd.cyou

[T20] Swift：数组操作
来源：http://gim.hnqzz.top

var a = [1, 2, 3];  a.append(4)
来源：http://hhu.zhongyouzk.top

[T21] Swift：遍历
来源：http://jni.jqgfzy.top

for x in a { print(x) }
来源：http://xws.birdmap.top

[T22] Swift：字典
来源：http://zcx.zhongyouzk.top

var d = ["a": 1];  d["b"] = 2
来源：http://azl.nanxinkj.top

[T23] Swift：函数
来源：http://tte.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rlf.hywenlv.cn

[T24] Swift：闭包
来源：http://jic.hnqzz.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ltc.zhengqikj.top

[T25] Swift：结构体
来源：http://jcz.316326.xyz

struct P { var x: Int }
来源：http://sbk.ybcxt.top

[T26] Swift：类与重写
来源：http://tdd.yvedp.cn

class A: Base { override func f() {} }
来源：http://szn.hcnkem.com

[T27] Swift：错误处理
来源：http://wja.jlsjyb.cn

do { try f() } catch { print(error) }
来源：http://jpd.ppjwa.cn

[T28] Swift：枚举
来源：http://kug.cucudq.cn

enum Color { case red, green }
来源：http://hve.yfazqb.com

[T29] Swift：guard 提前返回
来源：http://gfn.zhoulong.xyz

guard let x = opt else { return }
来源：http://die.mhx1999.top

[T30] Swift：协议
来源：http://reb.shuidangran.top

protocol Shape { func area() -> Double }
来源：http://dis.yongpay.top

[T31] Lua：Hello World
来源：http://alo.xuetiantiany.cn

print("Hello")
来源：http://wet.xingfuxueyuan.xyz

[T32] Lua：局部变量
来源：http://jme.wangdashe.top

local a = 1
来源：http://xqg.jinqigufen.top

[T33] Lua：表（数组）
来源：http://pwb.wangshuangyany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kmv.nanxinkj.top

[T34] Lua：遍历表
来源：http://tfk.zdqjudy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kyh.jlsjyb.cn

[T35] Lua：字典表
来源：http://ano.ywan-chungtsiang.top

local d = { a = 1 };  d.b = 2
来源：http://fne.nwbrower.top

[T36] Lua：函数
来源：http://ued.haohaochexian.top

function add(a, b) return a + b end
来源：http://bne.ctjpmb.com

[T37] Lua：字符串拼接
来源：http://iik.xinyue.icu

"a" .. "b"
来源：http://hcq.cdnleiting.top

[T38] Lua：条件
来源：http://aza.dashuyun.cn

if x > 0 then print("正") end
来源：http://wxm.hnqzz.top

[T39] Lua：模式匹配
来源：http://rkm.cucudq.cn

string.find(s, "%d+")
来源：http://gbi.tarul.cn

[T40] Lua：元表
来源：http://iev.shuidangran.top

setmetatable({}, { __index = base })
来源：http://sov.316326.xyz

[T41] Perl：Hello World
来源：http://vcm.gotoacloud.top

print "Hello\n";
来源：http://fap.andypj.xyz

[T42] Perl：变量类型
来源：http://cns.cdnleiting.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hib.hfpthk.cn

[T43] Perl：字符串插值
来源：http://tkz.haohaochexian.top

"值: $a"
来源：http://gos.cdnleiting.top

[T44] Perl：条件
来源：http://qph.sxryk.cn

if ($a > 0) { print "正"; }
来源：http://ssr.jqgfzy.top

[T45] Perl：数组遍历
来源：http://jrs.bjfxy.top

for my $x (@arr) { print $x; }
来源：http://pdx.52xcode.cn

[T46] Perl：哈希操作
来源：http://feu.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tiu.zycfv.cn

[T47] Perl：正则捕获
来源：http://yxt.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vsh.yongpay.top

[T48] Perl：正则替换
来源：http://gfx.jqgfzy.top

$s =~ s/old/new/g;
来源：http://otu.yonumen.top

[T49] Perl：函数
来源：http://xvy.jianghu66.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://azb.pycfn.com

[T50] Perl：逐行读文件
来源：http://efb.cqqwz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xia.jyoumei.cn

while (my $line = <$fh>) { print $line; }
来源：http://yck.ehwqpu.com

[T51] Scala：Hello World
来源：http://vbh.hywenlv.cn

println("Hello")
来源：http://zyl.fktsv.cn

[T52] Scala：变量
来源：http://ngx.yongpay.top

val a = 1;  var b = 2
来源：http://aot.shzxlz.cn

[T53] Scala：字符串插值
来源：http://and.vqdsnc.cn

s"值: $b"
来源：http://nvd.xinyue.icu

[T54] Scala：集合映射
来源：http://kuu.zhongyouzk.top

List(1, 2, 3).map(_ * 2)
来源：http://ojg.yanxiufei.cn

[T55] Scala：集合过滤
来源：http://fvz.pengpengdd.cyou

List(1, 2, 3).filter(_ > 1)
来源：http://zvk.fehbvm.com

[T56] Scala：样例类
来源：http://lmw.ctjpmb.com

case class User(name: String, age: Int)
来源：http://goq.cdnleiting.top

[T57] Scala：模式匹配
来源：http://jke.pengpengdd.cyou

x match { case 1 => "一"; case _ => "其他" }
来源：http://zle.ctjpmb.com

[T58] Scala：函数定义
来源：http://rfi.zycfv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uwg.bjfxy.top

[T59] Scala：循环
来源：http://drw.fanxiaobao.xyz

for (i <- 1 to 10) println(i)
来源：http://tvc.316326.xyz

[T60] Scala：折叠
来源：http://vur.9152youxi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iam.ybcxt.top

================================================================================
来源：http://xun.epnwcf.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vjb.ydzc1.top

================================================================================
来源：http://izf.zycfv.cn

[U01] Py：创建虚拟环境
来源：http://mcx.ydzc1.top

python -m venv .venv && source .venv/bin/activate
来源：http://brb.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://sxp.cheryme.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nql.nanxinkj.top

[U03] Py：加载 .env 配置
来源：http://dol.nanxinkj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ewx.xuanzx.com

[U04] Py：变量调试打印
来源：http://mvv.daria6918.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://svj.guannengcc.top

[U05] Py：列表去重且保序
来源：http://dgn.52xcode.cn

list(dict.fromkeys(arr))
来源：http://hgd.yvedp.cn

[U06] Py：合并两个字典
来源：http://abq.tanke756.top

{**a, **b}
来源：http://eof.yfazqb.com

[U07] Py：反转字典键值
来源：http://tth.feifeiyinyue.top

{v: k for k, v in d.items()}
来源：http://bfz.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://qhm.sjlbkw.cn

[y for x in nested for y in x]
来源：http://vmj.cashguo.top

[U09] Py：字典取最大值的键
来源：http://cnj.52xcode.cn

max(d, key=d.get)
来源：http://smq.shzxlz.cn

[U10] Py：按值排序字典
来源：http://emi.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dca.zhengqikj.top

[U11] Py：生成器表达式
来源：http://job.hysaishi.cn

(x * 2 for x in arr)
来源：http://krz.snrcjt.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ljv.shangyingyoupin.top

Counter(arr).most_common(3)
来源：http://dod.wangshuangyany.cn

[U13] Py：固定长度队列
来源：http://hue.gogol.net.cn

deque(maxlen=10)
来源：http://dtd.jinqigufen.top

[U14] Py：分组收集到列表
来源：http://ube.redwolf501.top

defaultdict(list)
来源：http://cfh.tian-w.cn

[U15] Py：高精度计时
来源：http://qqw.yfazqb.com

t = time.perf_counter()
来源：http://rhd.0kj1m.cn

[U16] Py：命令行参数解析
来源：http://wke.chenjidiqi.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dme.daxiang520.top

[U17] Py：初始化日志
来源：http://sxb.bbcook.cn

logging.basicConfig(level=logging.INFO)
来源：http://nvo.ydjk.org.cn

[U18] Py：预编译正则
来源：http://keb.chenzaomai.com

pat = re.compile(r"\d+")
来源：http://ure.jqgufenzy.top

[U19] Py：正则替换带回调
来源：http://pek.ybcxt.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cgb.guowangkeji.top

[U20] Py：缓存函数结果
来源：http://tmb.hcnkem.com

@functools.lru_cache(maxsize=None)
来源：http://nrn.mhx1999.top

[U21] Py：自定义上下文管理器
来源：http://rkw.fengsongda.top

@contextlib.contextmanager
来源：http://ykl.cqqwz.cn

[U22] Py：矩阵转置
来源：http://zef.tianlin.xyz

list(zip(*m))
来源：http://gde.hnqzz.top

[U23] Py：分块读取大文件
来源：http://bbm.xziqi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tol.fktsv.cn

[U24] Py：路径操作
来源：http://qsx.birdmap.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bwz.c1oappe.top

[U25] Py：CSV 按字典读
来源：http://sck.daria6918.cn

csv.DictReader(f)
来源：http://qzd.mhx1999.top

[U26] Py：并发下载
来源：http://qsx.ywan-chungtsiang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ehz.zhaomingkeji.xyz

[U27] Py：异步 HTTP
来源：http://yml.yuanzhike.top

aiohttp.ClientSession() 配合 async with
来源：http://ufs.ppjwa.cn

[U28] Py：类型别名
来源：http://pbz.hysaishi.cn

UserId = int
来源：http://xib.yvedp.cn

[U29] Py：属性校验
来源：http://rjs.fehbvm.com

@property 与 @x.setter 配合
来源：http://buf.aibaodan.cn

[U30] Py：数据类
来源：http://hyf.jqgufenzy.top

@dataclass(slots=True)
来源：http://icv.hywenlv.cn

[U31] Py：单测
来源：http://erd.9152youxi.cn

python -m pytest -q
来源：http://izn.zdqjudy.top

[U32] Py：代码格式化
来源：http://jic.gogol.net.cn

ruff format . && ruff check --fix .
来源：http://bsp.zhoulong.xyz

[U33] Py：打包发布
来源：http://dgm.zdbjq.cn

python -m build  （依赖 pyproject.toml）
来源：http://nhb.52xcode.cn

[U34] Py：判断编码
来源：http://bfm.52xcode.cn

chardet.detect(raw)
来源：http://eou.gotoacloud.top

[U35] Py：发送邮件
来源：http://ukx.zhijiandao.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pme.hywenlv.cn

[U36] Py：定时任务
来源：http://mkt.meibo888.top

schedule.every(10).minutes.do(job)
来源：http://osz.xylfe.cn

[U37] Py：读写 Excel
来源：http://jhx.birdmap.top

pandas.read_excel / DataFrame.to_excel
来源：http://qxp.yj20258.top

[U38] Py：获取脚本所在目录
来源：http://ste.9152youxi.cn

Path(__file__).resolve().parent
来源：http://rkm.nwbrower.top

[U39] Py：判断是否在交互环境
来源：http://qen.hesvh.cn

sys.stdout.isatty()
来源：http://dai.zdqjudy.top

[U40] Py：打印到标准错误
来源：http://bcl.hesvh.cn

print("err", file=sys.stderr)
来源：http://ibc.cdnleiting.top

[U41] PHP：初始化 Composer 项目
来源：http://gnc.chenlongwang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://icy.dianchejie.cn

[U42] PHP：PSR-4 自动加载
来源：http://ddm.dashuyun.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://smo.bbcook.cn

[U43] PHP：声明命名空间
来源：http://yew.yuxming.cn

namespace App\Http;
来源：http://jyi.sweek.top

[U44] PHP：开启严格类型
来源：http://siz.yfazqb.com

declare(strict_types=1);
来源：http://veu.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://cgq.zhaomingkeji.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://kzc.xinyue.icu

[U46] PHP：可空类型
来源：http://vtm.sweek.top

?string $name = null
来源：http://vot.hywenlv.cn

[U47] PHP：联合类型
来源：http://nei.yonumen.top

int|string $id
来源：http://uhf.ybcxt.top

[U48] PHP：纯枚举
来源：http://eoy.zhixingplan.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ysp.zhongyouzk.top

[U49] PHP：只读属性
来源：http://tip.hnqzz.top

public readonly string $name
来源：http://kkh.daxiang520.top

[U50] PHP：构造器属性提升
来源：http://ato.chenjidiqi.icu

public function __construct(private int $id) {}
来源：http://pqz.nwbrower.top


<!-- 参考信息 -->