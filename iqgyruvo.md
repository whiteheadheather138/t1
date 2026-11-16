代发 wailian999

memset(a, 0, sizeof a);
来源：http://kov.snrcjt.cn

[S27] C：定义常量
来源：http://hyh.ivvv.top

const double PI = 3.14159;
来源：http://haj.hesvh.cn

[S28] C：静态变量
来源：http://rfm.chenjidiqi.icu

static int counter = 0;
来源：http://uwj.yfazqb.com

[S29] C：变参函数
来源：http://apl.wangdashe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lra.jyoumei.cn

[S30] C：头文件保护
来源：http://ovy.mhx1999.top

#ifndef X_H
来源：http://zic.wangshuangyany.cn

#define X_H
来源：http://plo.ctjpmb.com

#endif
来源：http://uwv.fehbvm.com

[S31] C++：Hello World
来源：http://msj.jianghu66.top

#include <iostream>
来源：http://cni.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://tgd.xziqi.cn

[S32] C++：字符串
来源：http://kdp.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://toj.vehdjk.com

[S33] C++：vector 增删
来源：http://qvu.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ugt.zdbjq.cn

[S34] C++：遍历 vector
来源：http://vcb.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://kgb.gzhubu.top

[S35] C++：map
来源：http://sgd.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cwz.shanyushiyangtech.top

[S36] C++：unordered_map
来源：http://luy.sufxvd.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://saq.gogol.net.cn

[S37] C++：set
来源：http://tgn.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ucg.jinyuanbaomall.cn

[S38] C++：排序
来源：http://odd.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://plv.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://jtz.jqgfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xku.yvedp.cn

[S40] C++：查找元素
来源：http://oow.jinghuilouyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://czu.52xcode.cn

[S41] C++：类与构造函数
来源：http://dhl.shanyushiyangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://myk.epnwcf.com

[S42] C++：继承与虚函数
来源：http://nxf.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://toq.52xcode.cn

[S43] C++：智能指针
来源：http://krv.tianlin.xyz

auto p = std::make_unique<int>(5);
来源：http://cec.aibaodan.cn

[S44] C++：引用传参
来源：http://tpk.andypj.xyz

void inc(int &x) { ++x; }
来源：http://bib.gogol.net.cn

[S45] C++：lambda
来源：http://zgv.316326.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://phh.tarul.cn

[S46] C++：函数模板
来源：http://nkr.ydzc1.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://guf.shanyushiyangtech.top

[S47] C++：结构化绑定遍历
来源：http://cjm.redwolf501.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xgq.ywan-chungtsiang.top

[S48] C++：逐行读文件
来源：http://pyn.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://lnw.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://uny.smart0.xyz

[S49] C++：写文件
来源：http://wmg.fehbvm.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zpn.dianchejie.cn

[S50] C++：格式化数字
来源：http://ewq.zdbjq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wop.hywenlv.cn

[S51] C++：显式类型转换
来源：http://ydu.haohaochexian.top

static_cast<double>(a) / b
来源：http://joc.cashguo.top

[S52] C++：const 与 noexcept
来源：http://rdv.sysykeji.top

int size() const noexcept { return n_; }
来源：http://vwi.zhijiandao.cn

[S53] C++：移动语义
来源：http://vda.jiagoushi.top

std::vector<int> w = std::move(v);
来源：http://jes.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://ais.tarul.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rls.snrcjt.cn

[S55] C++：结构化绑定
来源：http://ulr.xuanzx.com

auto [a, b] = std::make_pair(1, 2);
来源：http://adg.daria6918.cn

[S56] C++：optional
来源：http://upx.jinqigufen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lbb.bbcook.cn

[S57] C++：编译期常量
来源：http://caf.wangdashe.top

constexpr int N = 10;
来源：http://oyr.fengsongda.top

[S58] C++：命名空间
来源：http://hjr.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://ifz.sysykeji.top

[S59] C++：静态断言
来源：http://mii.dashuyun.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hed.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://xsw.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kyv.iojbl.cn

================================================================================
来源：http://ilo.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iwu.shanyushiyangtech.top

================================================================================
来源：http://pzd.cashguo.top

[T01] Kotlin：Hello World
来源：http://cbm.hongshengwenyu.top

println("Hello")
来源：http://ksc.zhongyouzk.top

[T02] Kotlin：变量
来源：http://tac.redwolf501.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://trb.wangshuangyany.cn

[T03] Kotlin：字符串模板
来源：http://syq.haohaochexian.top

"值: $b"
来源：http://oln.jinyuanbaomall.cn

[T04] Kotlin：空安全
来源：http://rtr.yj20258.top

val n: String? = null;  n?.length
来源：http://qyt.ywan-chungtsiang.top

[T05] Kotlin：when 表达式
来源：http://rqd.cucudq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ukx.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://ykt.xingfuxueyuan.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://coh.chenjidiqi.icu

[T07] Kotlin：集合过滤
来源：http://wst.0kj1m.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mqw.meibo888.top

[T08] Kotlin：数据类
来源：http://ami.wangshuangyany.cn

data class User(val name: String, val age: Int)
来源：http://qsk.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://bhl.jianghu66.top

fun String.exclaim() = this + "!"
来源：http://qvv.yueranfly.top

[T10] Kotlin：默认参数
来源：http://vxa.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://lsu.haohaochexian.top

[T11] Kotlin：协程
来源：http://juj.ivvv.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ohj.yvedp.cn

[T12] Kotlin：解构声明
来源：http://vfv.ctjpmb.com

val (a, b) = Pair(1, 2)
来源：http://cxh.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://brz.tian-w.cn

val m = mapOf("a" to 1)
来源：http://wen.hongshengwenyu.top

[T14] Kotlin：循环
来源：http://hxl.uphjek.com

for (i in 1..10) println(i)
来源：http://vdc.cheryme.top

[T15] Kotlin：接口
来源：http://emr.yongpay.top

interface Shape { fun area(): Double }
来源：http://tpv.cucudq.cn

[T16] Swift：Hello World
来源：http://lyr.fzhhl.top

print("Hello")
来源：http://xhs.yongpay.top

[T17] Swift：变量与常量
来源：http://vpz.havefunace.top

var a = 1;  let b = 2
来源：http://pss.sweek.top

[T18] Swift：字符串插值
来源：http://ubl.vqdsnc.cn

"值: \(b)"
来源：http://dwp.hesvh.cn

[T19] Swift：可选绑定
来源：http://wuu.jyoumei.cn

if let n = opt { print(n) }
来源：http://eln.ydzc1.top

[T20] Swift：数组操作
来源：http://gqq.dianchejie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hty.yvedp.cn

[T21] Swift：遍历
来源：http://pjx.hnqzz.top

for x in a { print(x) }
来源：http://fwa.xuetiantiany.cn

[T22] Swift：字典
来源：http://inh.quarkkingdee.top

var d = ["a": 1];  d["b"] = 2
来源：http://shm.snrcjt.cn

[T23] Swift：函数
来源：http://nse.uphjek.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lty.pycfn.com

[T24] Swift：闭包
来源：http://cvx.daxiang520.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://euy.yangfankeji.com

[T25] Swift：结构体
来源：http://vlf.yj20258888.top

struct P { var x: Int }
来源：http://hoa.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://qdo.hnxiangtu.top

class A: Base { override func f() {} }
来源：http://pph.jqgfzy.top

[T27] Swift：错误处理
来源：http://avk.snrcjt.cn

do { try f() } catch { print(error) }
来源：http://yaj.yvedp.cn

[T28] Swift：枚举
来源：http://xjx.jinyuanbaomall.cn

enum Color { case red, green }
来源：http://pgb.fanxiaobao.xyz

[T29] Swift：guard 提前返回
来源：http://bxj.jlsjyb.cn

guard let x = opt else { return }
来源：http://lan.fehbvm.com

[T30] Swift：协议
来源：http://aft.316326.xyz

protocol Shape { func area() -> Double }
来源：http://iwx.jinyuanbaomall.cn

[T31] Lua：Hello World
来源：http://rul.zdbjq.cn

print("Hello")
来源：http://gvr.yfazqb.com

[T32] Lua：局部变量
来源：http://cpp.svipenyu.cn

local a = 1
来源：http://nkm.gzhubu.top

[T33] Lua：表（数组）
来源：http://idp.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mih.mhx1999.top

[T34] Lua：遍历表
来源：http://zof.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qdm.hywenlv.cn

[T35] Lua：字典表
来源：http://qlz.zycfv.cn

local d = { a = 1 };  d.b = 2
来源：http://wnd.epnwcf.com

[T36] Lua：函数
来源：http://cor.tarul.cn

function add(a, b) return a + b end
来源：http://icd.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://syu.tarul.cn

"a" .. "b"
来源：http://klp.zhijiandao.cn

[T38] Lua：条件
来源：http://tdl.0kj1m.cn

if x > 0 then print("正") end
来源：http://gku.yfazqb.com

[T39] Lua：模式匹配
来源：http://wae.kuanghao11.cn

string.find(s, "%d+")
来源：http://wsp.iojbl.cn

[T40] Lua：元表
来源：http://xvx.zhaomingkeji.xyz

setmetatable({}, { __index = base })
来源：http://ret.hnqzz.top

[T41] Perl：Hello World
来源：http://itf.chenzaomai.com

print "Hello\n";
来源：http://idz.vehdjk.com

[T42] Perl：变量类型
来源：http://kuf.zhengqikj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bks.hywenlv.cn

[T43] Perl：字符串插值
来源：http://ehc.hnxiangtu.top

"值: $a"
来源：http://sku.havefunace.top

[T44] Perl：条件
来源：http://fyv.iojbl.cn

if ($a > 0) { print "正"; }
来源：http://wqp.gzhubu.top

[T45] Perl：数组遍历
来源：http://jji.yanxiufei.cn

for my $x (@arr) { print $x; }
来源：http://zev.tanke756.top

[T46] Perl：哈希操作
来源：http://nad.cheryme.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xmc.shzxlz.cn

[T47] Perl：正则捕获
来源：http://jim.yuanzhike.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://sui.hfpthk.cn

[T48] Perl：正则替换
来源：http://owe.tarul.cn

$s =~ s/old/new/g;
来源：http://ugs.bbcook.cn

[T49] Perl：函数
来源：http://dnf.bbcook.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rxj.yj20258.top

[T50] Perl：逐行读文件
来源：http://nwc.jinqigufen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gid.316326.xyz

while (my $line = <$fh>) { print $line; }
来源：http://kfq.jiagoushi.top

[T51] Scala：Hello World
来源：http://lou.gzhubu.top

println("Hello")
来源：http://mgl.9152youxi.cn

[T52] Scala：变量
来源：http://fpn.quarkkingdee.top

val a = 1;  var b = 2
来源：http://lht.dashuyun.cn

[T53] Scala：字符串插值
来源：http://jfq.9152youxi.cn

s"值: $b"
来源：http://lhi.daxiang520.top

[T54] Scala：集合映射
来源：http://rfb.hnxiangtu.top

List(1, 2, 3).map(_ * 2)
来源：http://agg.hcnkem.com

[T55] Scala：集合过滤
来源：http://zys.fktsv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fgr.feifeiyinyue.top

[T56] Scala：样例类
来源：http://aeh.aibaodan.cn

case class User(name: String, age: Int)
来源：http://ybv.ivvv.top

[T57] Scala：模式匹配
来源：http://zjp.chenjidiqi.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://rjx.yueranfly.top

[T58] Scala：函数定义
来源：http://clv.yangfankeji.com

def add(a: Int, b: Int): Int = a + b
来源：http://iqb.hnxiangtu.top

[T59] Scala：循环
来源：http://iqj.xuanzx.com

for (i <- 1 to 10) println(i)
来源：http://mgh.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://mdn.yonumen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uev.tian-w.cn

================================================================================
来源：http://wzd.zhoulong.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wtv.cqqwz.cn

================================================================================
来源：http://inp.ywan-chungtsiang.top

[U01] Py：创建虚拟环境
来源：http://hkz.hesvh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hdu.yvedp.cn

[U02] Py：导出 / 安装依赖
来源：http://tbt.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iip.shzxlz.cn

[U03] Py：加载 .env 配置
来源：http://xdm.chenlongwang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tgf.fengsongda.top

[U04] Py：变量调试打印
来源：http://txr.zhijiandao.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pwm.zhoulong.xyz

[U05] Py：列表去重且保序
来源：http://epa.bbcook.cn

list(dict.fromkeys(arr))
来源：http://bpq.jqgfzy.top

[U06] Py：合并两个字典
来源：http://jfq.vehdjk.com

{**a, **b}
来源：http://chw.yuanzhike.top

[U07] Py：反转字典键值
来源：http://pjo.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://unw.9152youxi.cn

[U08] Py：展平二维列表
来源：http://ylu.xylfe.cn

[y for x in nested for y in x]
来源：http://sic.316326.xyz

[U09] Py：字典取最大值的键
来源：http://ekp.dashuyun.cn

max(d, key=d.get)
来源：http://wve.gogol.net.cn

[U10] Py：按值排序字典
来源：http://mpz.ydjk.org.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hyp.yueranfly.top

[U11] Py：生成器表达式
来源：http://rod.zhijiandao.cn

(x * 2 for x in arr)
来源：http://wjd.xuanzx.com

[U12] Py：取出现最多的 3 个元素
来源：http://wtb.sufxvd.cn

Counter(arr).most_common(3)
来源：http://zbb.daria6918.cn

[U13] Py：固定长度队列
来源：http://uet.guowangkeji.top

deque(maxlen=10)
来源：http://djy.yongpay.top

[U14] Py：分组收集到列表
来源：http://cha.dashuyun.cn

defaultdict(list)
来源：http://qjg.guowangkeji.top

[U15] Py：高精度计时
来源：http://cir.xuetiantiany.cn

t = time.perf_counter()
来源：http://syb.uphjek.com

[U16] Py：命令行参数解析
来源：http://mhe.yj20258.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vda.daria6918.cn

[U17] Py：初始化日志
来源：http://vyo.cheryme.top

logging.basicConfig(level=logging.INFO)
来源：http://xxa.gotoacloud.top

[U18] Py：预编译正则
来源：http://ykg.andypj.xyz

pat = re.compile(r"\d+")
来源：http://psy.ydzc1.top

[U19] Py：正则替换带回调
来源：http://vdg.nwbrower.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ndi.hammf.cn

[U20] Py：缓存函数结果
来源：http://oxr.ydzc1.top

@functools.lru_cache(maxsize=None)
来源：http://faz.fktsv.cn

[U21] Py：自定义上下文管理器
来源：http://szv.bjfxy.top

@contextlib.contextmanager
来源：http://khx.fzhhl.top

[U22] Py：矩阵转置
来源：http://hfb.gotoacloud.top

list(zip(*m))
来源：http://wiu.zhengqikj.top

[U23] Py：分块读取大文件
来源：http://vdd.xylfe.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xpn.quarkkingdee.top

[U24] Py：路径操作
来源：http://bjx.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vuz.jlsjyb.cn

[U25] Py：CSV 按字典读
来源：http://nls.sjlbkw.cn

csv.DictReader(f)
来源：http://mff.wangdashe.top

[U26] Py：并发下载
来源：http://xkn.tanke756.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://abs.iojbl.cn

[U27] Py：异步 HTTP
来源：http://ngm.nanxuanxn.top

aiohttp.ClientSession() 配合 async with
来源：http://buj.feifeiyinyue.top

[U28] Py：类型别名
来源：http://wot.smart0.xyz

UserId = int
来源：http://rfq.yvedp.cn

[U29] Py：属性校验
来源：http://bht.jqgfzy.top

@property 与 @x.setter 配合
来源：http://tmu.feifeiyinyue.top

[U30] Py：数据类
来源：http://tzc.chenlongwang.top

@dataclass(slots=True)
来源：http://dgc.andypj.xyz

[U31] Py：单测
来源：http://sva.kuanghao11.cn

python -m pytest -q
来源：http://izc.zhengqikj.top

[U32] Py：代码格式化
来源：http://yvz.redwolf501.top

ruff format . && ruff check --fix .
来源：http://rpt.zdbjq.cn

[U33] Py：打包发布
来源：http://xig.iojbl.cn

python -m build  （依赖 pyproject.toml）
来源：http://xyz.daxiang520.top

[U34] Py：判断编码
来源：http://dai.nanxinkj.top

chardet.detect(raw)
来源：http://fyn.cucudq.cn

[U35] Py：发送邮件
来源：http://szy.shangyingyoupin.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nno.jinqigfzy.top

[U36] Py：定时任务
来源：http://wug.yj20258888.top

schedule.every(10).minutes.do(job)
来源：http://cog.pycfn.com

[U37] Py：读写 Excel
来源：http://iat.hnqzz.top

pandas.read_excel / DataFrame.to_excel
来源：http://rmo.andypj.xyz

[U38] Py：获取脚本所在目录
来源：http://mjx.yanxiufei.cn

Path(__file__).resolve().parent
来源：http://yzl.tarul.cn

[U39] Py：判断是否在交互环境
来源：http://xqa.yuanzhike.top

sys.stdout.isatty()
来源：http://dnx.yvedp.cn

[U40] Py：打印到标准错误
来源：http://twi.wangshuangyany.cn

print("err", file=sys.stderr)
来源：http://sap.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://djj.fehbvm.com

composer init;  composer require guzzlehttp/guzzle
来源：http://fuy.cheryme.top

[U42] PHP：PSR-4 自动加载
来源：http://akn.meibo888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gef.daria6918.cn

[U43] PHP：声明命名空间
来源：http://tej.sweek.top

namespace App\Http;
来源：http://qxl.smart0.xyz

[U44] PHP：开启严格类型
来源：http://cti.ywan-chungtsiang.top

declare(strict_types=1);
来源：http://gms.nanxinkj.top

[U45] PHP：类型声明与返回类型
来源：http://add.zhixingplan.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ktf.redwolf501.top

[U46] PHP：可空类型
来源：http://phv.feifeiyinyue.top

?string $name = null
来源：http://xsu.yongpay.top

[U47] PHP：联合类型
来源：http://opz.hongshengwenyu.top

int|string $id
来源：http://yuo.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://fvh.gogol.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://egl.shuidangran.top

[U49] PHP：只读属性
来源：http://qsx.redwolf501.top

public readonly string $name
来源：http://ffd.yanxiufei.cn

[U50] PHP：构造器属性提升
来源：http://aay.chenlongwang.top

public function __construct(private int $id) {}
来源：http://zrk.zhoulong.xyz


<!-- 参考信息 -->