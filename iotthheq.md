代发 wailian999

#ifndef X_H
来源：http://bsy.52xcode.cn

#define X_H
来源：http://sgy.hywenlv.cn

#endif
来源：http://izb.tian-w.cn

[S31] C++：Hello World
来源：http://nwx.ivvv.top

#include <iostream>
来源：http://idv.zhaomingkeji.xyz

int main() { std::cout << "Hello\n"; }
来源：http://agb.dashuyun.cn

[S32] C++：字符串
来源：http://abr.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://sdn.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://mlv.xuetiantiany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jqq.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://jyi.bjfxy.top

for (auto &x : v) { std::cout << x; }
来源：http://zzl.cdnleiting.top

[S35] C++：map
来源：http://pjt.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://khq.c1oappe.top

[S36] C++：unordered_map
来源：http://gyb.ehwqpu.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cuu.shanyushiyangkeji.top

[S37] C++：set
来源：http://gby.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nqr.epnwcf.com

[S38] C++：排序
来源：http://mth.zhengqikj.top

std::sort(v.begin(), v.end());
来源：http://ofi.hywenlv.cn

[S39] C++：自定义比较器排序
来源：http://ggg.jinqigufen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yfo.nanxinkj.top

[S40] C++：查找元素
来源：http://sgv.snrcjt.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zft.daria6918.cn

[S41] C++：类与构造函数
来源：http://zwj.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wnh.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://jnf.shanyushiyangtech.top

class B : public Base { public: void f() override {} };
来源：http://qyp.andypj.xyz

[S43] C++：智能指针
来源：http://ovg.cdnleiting.top

auto p = std::make_unique<int>(5);
来源：http://wxp.yueranfly.top

[S44] C++：引用传参
来源：http://hew.zhiwuduotai.top

void inc(int &x) { ++x; }
来源：http://bdv.xylfe.cn

[S45] C++：lambda
来源：http://unz.xuanzx.com

auto add = [](int a, int b) { return a + b; };
来源：http://edd.gzhubu.top

[S46] C++：函数模板
来源：http://nrr.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zhc.jinqigufen.top

[S47] C++：结构化绑定遍历
来源：http://dbe.sysykeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kmf.guannengcc.top

[S48] C++：逐行读文件
来源：http://yum.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vwz.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://vdj.jinqigfzy.top

[S49] C++：写文件
来源：http://vkg.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://djt.fengsongda.top

[S50] C++：格式化数字
来源：http://rer.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nxe.cheryme.top

[S51] C++：显式类型转换
来源：http://xkf.zhijiandao.cn

static_cast<double>(a) / b
来源：http://lts.yvedp.cn

[S52] C++：const 与 noexcept
来源：http://dob.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://hgi.jinqigufen.top

[S53] C++：移动语义
来源：http://ppc.yvedp.cn

std::vector<int> w = std::move(v);
来源：http://ejo.cdnleiting.top

[S54] C++：异常处理
来源：http://igt.shanyushiyangtech.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kgo.yj202588.top

[S55] C++：结构化绑定
来源：http://ekt.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zfy.shanyushiyangkeji.top

[S56] C++：optional
来源：http://orv.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wak.shuidangran.top

[S57] C++：编译期常量
来源：http://maj.316326.xyz

constexpr int N = 10;
来源：http://fum.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://sbu.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://ubu.fehbvm.com

[S59] C++：静态断言
来源：http://rxd.yj20258888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nkv.jqgufenzy.top

[S60] C++：遍历并删除元素
来源：http://azi.gotoacloud.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://egs.hnxiangtu.top

================================================================================
来源：http://fwl.quarkkingdee.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dye.xylfe.cn

================================================================================
来源：http://lkp.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://ybh.fengsongda.top

println("Hello")
来源：http://oof.xuanzx.com

[T02] Kotlin：变量
来源：http://ycw.vqdsnc.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ugc.fktsv.cn

[T03] Kotlin：字符串模板
来源：http://xww.zhixingplan.top

"值: $b"
来源：http://pfs.shzxlz.cn

[T04] Kotlin：空安全
来源：http://tfc.jinqigufen.top

val n: String? = null;  n?.length
来源：http://qcz.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://jhx.shzxlz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tcc.yvedp.cn

[T06] Kotlin：集合映射
来源：http://tlc.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://bvt.c1oappe.top

[T07] Kotlin：集合过滤
来源：http://cvw.hesvh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://krr.pycfn.com

[T08] Kotlin：数据类
来源：http://wpb.hongshengwenyu.top

data class User(val name: String, val age: Int)
来源：http://lym.cucudq.cn

[T09] Kotlin：扩展函数
来源：http://ypr.aizwys.cn

fun String.exclaim() = this + "!"
来源：http://btw.jinqigufen.top

[T10] Kotlin：默认参数
来源：http://uke.ppjwa.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jnf.cdnleiting.top

[T11] Kotlin：协程
来源：http://gve.xziqi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tsk.cucudq.cn

[T12] Kotlin：解构声明
来源：http://kei.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://wob.zhijiandao.cn

[T13] Kotlin：只读 Map
来源：http://zdg.yonumen.top

val m = mapOf("a" to 1)
来源：http://bob.iojbl.cn

[T14] Kotlin：循环
来源：http://ind.guowangkeji.top

for (i in 1..10) println(i)
来源：http://bxc.shanyushiyangkeji.top

[T15] Kotlin：接口
来源：http://pvv.jinyuanbaomall.cn

interface Shape { fun area(): Double }
来源：http://xxy.yj202588.top

[T16] Swift：Hello World
来源：http://wyo.zdbjq.cn

print("Hello")
来源：http://ryp.jyoumei.cn

[T17] Swift：变量与常量
来源：http://utg.jlsjyb.cn

var a = 1;  let b = 2
来源：http://rjz.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://fva.aizwys.cn

"值: \(b)"
来源：http://ssn.gotoacloud.top

[T19] Swift：可选绑定
来源：http://viu.sysykeji.top

if let n = opt { print(n) }
来源：http://vut.shanyushiyangtech.top

[T20] Swift：数组操作
来源：http://eee.sysykeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://ddj.meibo888.top

[T21] Swift：遍历
来源：http://dzu.0kj1m.cn

for x in a { print(x) }
来源：http://hwr.ywan-chungtsiang.top

[T22] Swift：字典
来源：http://sip.redwolf501.top

var d = ["a": 1];  d["b"] = 2
来源：http://bqk.shanyushiyangkeji.top

[T23] Swift：函数
来源：http://brj.hnqzz.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pdx.cashguo.top

[T24] Swift：闭包
来源：http://jde.fzhhl.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hwp.yongpay.top

[T25] Swift：结构体
来源：http://qyz.gzhubu.top

struct P { var x: Int }
来源：http://yrq.meibo888.top

[T26] Swift：类与重写
来源：http://kto.nanxuanxn.top

class A: Base { override func f() {} }
来源：http://lmv.52xcode.cn

[T27] Swift：错误处理
来源：http://qbk.shzxlz.cn

do { try f() } catch { print(error) }
来源：http://zcn.hnqzz.top

[T28] Swift：枚举
来源：http://fac.ivvv.top

enum Color { case red, green }
来源：http://mcl.dianchejie.cn

[T29] Swift：guard 提前返回
来源：http://hao.zdbjq.cn

guard let x = opt else { return }
来源：http://dxl.ppjwa.cn

[T30] Swift：协议
来源：http://nvd.gaohongyu789.top

protocol Shape { func area() -> Double }
来源：http://edq.jlsjyb.cn

[T31] Lua：Hello World
来源：http://ayn.hcnkem.com

print("Hello")
来源：http://jkv.gaohongyu789.top

[T32] Lua：局部变量
来源：http://rri.yvedp.cn

local a = 1
来源：http://ppq.wangdashe.top

[T33] Lua：表（数组）
来源：http://uab.andypj.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://qdt.cucudq.cn

[T34] Lua：遍历表
来源：http://min.redwolf501.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gql.ybcxt.top

[T35] Lua：字典表
来源：http://bjg.fzhhl.top

local d = { a = 1 };  d.b = 2
来源：http://cje.zycfv.cn

[T36] Lua：函数
来源：http://too.mhx1999.top

function add(a, b) return a + b end
来源：http://emi.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://ndd.cucudq.cn

"a" .. "b"
来源：http://xrg.jyoumei.cn

[T38] Lua：条件
来源：http://ifo.yuanzhike.top

if x > 0 then print("正") end
来源：http://ydp.tanke756.top

[T39] Lua：模式匹配
来源：http://dem.nanxinkj.top

string.find(s, "%d+")
来源：http://pcq.uphjek.com

[T40] Lua：元表
来源：http://orr.vehdjk.com

setmetatable({}, { __index = base })
来源：http://kph.sweek.top

[T41] Perl：Hello World
来源：http://pex.zycfv.cn

print "Hello\n";
来源：http://eqi.daria6918.cn

[T42] Perl：变量类型
来源：http://xyj.sweek.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://elb.zhongyouzk.top

[T43] Perl：字符串插值
来源：http://vyc.shangyingyoupin.top

"值: $a"
来源：http://ius.0kj1m.cn

[T44] Perl：条件
来源：http://slt.zhiwuduotai.top

if ($a > 0) { print "正"; }
来源：http://jht.sysykeji.top

[T45] Perl：数组遍历
来源：http://djp.yvedp.cn

for my $x (@arr) { print $x; }
来源：http://kia.daxiang520.top

[T46] Perl：哈希操作
来源：http://uch.chenjidiqi.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xow.ydzc1.top

[T47] Perl：正则捕获
来源：http://zpm.uphjek.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://tcm.aibaodan.cn

[T48] Perl：正则替换
来源：http://qka.hongshengwenyu.top

$s =~ s/old/new/g;
来源：http://uqz.sjlbkw.cn

[T49] Perl：函数
来源：http://mim.jinghuilouyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bwq.gzhubu.top

[T50] Perl：逐行读文件
来源：http://jkw.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tpo.yueranfly.top

while (my $line = <$fh>) { print $line; }
来源：http://ksi.dianchejie.cn

[T51] Scala：Hello World
来源：http://bdr.316326.xyz

println("Hello")
来源：http://ntw.feifeiyinyue.top

[T52] Scala：变量
来源：http://whx.aibaodan.cn

val a = 1;  var b = 2
来源：http://gml.fanxiaobao.xyz

[T53] Scala：字符串插值
来源：http://jvu.havefunace.top

s"值: $b"
来源：http://evv.cqqwz.cn

[T54] Scala：集合映射
来源：http://jtf.ydzc1.top

List(1, 2, 3).map(_ * 2)
来源：http://ehs.sxryk.cn

[T55] Scala：集合过滤
来源：http://ksy.meibo888.top

List(1, 2, 3).filter(_ > 1)
来源：http://caw.havefunace.top

[T56] Scala：样例类
来源：http://skg.yvedp.cn

case class User(name: String, age: Int)
来源：http://bbt.zhoulong.xyz

[T57] Scala：模式匹配
来源：http://gxb.0kj1m.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://axe.tarul.cn

[T58] Scala：函数定义
来源：http://any.yj20258.top

def add(a: Int, b: Int): Int = a + b
来源：http://zjs.hongshengwenyu.top

[T59] Scala：循环
来源：http://gqu.yueranfly.top

for (i <- 1 to 10) println(i)
来源：http://pup.pycfn.com

[T60] Scala：折叠
来源：http://izs.ctjpmb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dja.smart0.xyz

================================================================================
来源：http://hbf.chenjidiqi.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yvi.ehwqpu.com

================================================================================
来源：http://zvh.yj20258.top

[U01] Py：创建虚拟环境
来源：http://xea.gotoacloud.top

python -m venv .venv && source .venv/bin/activate
来源：http://kez.mhx1999.top

[U02] Py：导出 / 安装依赖
来源：http://cea.yuxming.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mxp.chenzaomai.com

[U03] Py：加载 .env 配置
来源：http://wbb.daria6918.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://upl.meibo888.top

[U04] Py：变量调试打印
来源：http://rdy.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rmt.hammf.cn

[U05] Py：列表去重且保序
来源：http://dmj.haohaochexian.top

list(dict.fromkeys(arr))
来源：http://ocn.gogol.net.cn

[U06] Py：合并两个字典
来源：http://hzh.yj20258.top

{**a, **b}
来源：http://qqy.yuxming.cn

[U07] Py：反转字典键值
来源：http://htb.jyoumei.cn

{v: k for k, v in d.items()}
来源：http://pms.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://sua.ehwqpu.com

[y for x in nested for y in x]
来源：http://kbk.kuanghao11.cn

[U09] Py：字典取最大值的键
来源：http://fcj.zhongyouzk.top

max(d, key=d.get)
来源：http://htv.hcnkem.com

[U10] Py：按值排序字典
来源：http://mur.shanyushiyangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vku.hywenlv.cn

[U11] Py：生成器表达式
来源：http://jxu.9152youxi.cn

(x * 2 for x in arr)
来源：http://sub.zycfv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://huy.chenjidiqi.icu

Counter(arr).most_common(3)
来源：http://vfs.tian-w.cn

[U13] Py：固定长度队列
来源：http://mxr.sufxvd.cn

deque(maxlen=10)
来源：http://qrj.zycfv.cn

[U14] Py：分组收集到列表
来源：http://msj.shuidangran.top

defaultdict(list)
来源：http://lvq.cashguo.top

[U15] Py：高精度计时
来源：http://zob.nanxinkj.top

t = time.perf_counter()
来源：http://vlq.hesvh.cn

[U16] Py：命令行参数解析
来源：http://iqk.hesvh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://foy.haohaochexian.top

[U17] Py：初始化日志
来源：http://rnf.chenjidiqi.icu

logging.basicConfig(level=logging.INFO)
来源：http://lse.feifeiyinyue.top

[U18] Py：预编译正则
来源：http://uot.ydzc1.top

pat = re.compile(r"\d+")
来源：http://yam.yj202588.top

[U19] Py：正则替换带回调
来源：http://dui.daria6918.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yoe.gogol.net.cn

[U20] Py：缓存函数结果
来源：http://ejo.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://hbl.hfpthk.cn

[U21] Py：自定义上下文管理器
来源：http://bgj.quarkkingdee.top

@contextlib.contextmanager
来源：http://fwt.sysykeji.top

[U22] Py：矩阵转置
来源：http://kcn.redwolf501.top

list(zip(*m))
来源：http://qke.jinyuanbaomall.cn

[U23] Py：分块读取大文件
来源：http://zsk.gogol.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hfk.bjfxy.top

[U24] Py：路径操作
来源：http://jkv.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kfu.haohaochexian.top

[U25] Py：CSV 按字典读
来源：http://qiv.yfazqb.com

csv.DictReader(f)
来源：http://qai.jyoumei.cn

[U26] Py：并发下载
来源：http://ecp.uphjek.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lbi.fengsongda.top

[U27] Py：异步 HTTP
来源：http://kkd.aizwys.cn

aiohttp.ClientSession() 配合 async with
来源：http://ewf.nanxuanxn.top

[U28] Py：类型别名
来源：http://jkl.xuetiantiany.cn

UserId = int
来源：http://mej.cdnleiting.top

[U29] Py：属性校验
来源：http://pdv.9152youxi.cn

@property 与 @x.setter 配合
来源：http://qwf.ydjk.org.cn

[U30] Py：数据类
来源：http://vyu.xuanzx.com

@dataclass(slots=True)
来源：http://nat.xingfuxueyuan.xyz

[U31] Py：单测
来源：http://ioa.hysaishi.cn

python -m pytest -q
来源：http://lim.dianchejie.cn

[U32] Py：代码格式化
来源：http://fzl.ywan-chungtsiang.top

ruff format . && ruff check --fix .
来源：http://wcd.nanxuanxn.top

[U33] Py：打包发布
来源：http://wrx.hesvh.cn

python -m build  （依赖 pyproject.toml）
来源：http://pdq.jianghu66.top

[U34] Py：判断编码
来源：http://pfg.zhixingplan.top

chardet.detect(raw)
来源：http://oai.quarkkingdee.top

[U35] Py：发送邮件
来源：http://zkn.dianchejie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hba.pycfn.com

[U36] Py：定时任务
来源：http://ecv.uphjek.com

schedule.every(10).minutes.do(job)
来源：http://dno.jinqigfzy.top

[U37] Py：读写 Excel
来源：http://mrn.cucudq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dge.mhx1999.top

[U38] Py：获取脚本所在目录
来源：http://nzj.yuanzhike.top

Path(__file__).resolve().parent
来源：http://agf.sxryk.cn

[U39] Py：判断是否在交互环境
来源：http://vms.jinghuilouyu.cn

sys.stdout.isatty()
来源：http://yks.shanyushiyangkeji.top

[U40] Py：打印到标准错误
来源：http://ltx.yueranfly.top

print("err", file=sys.stderr)
来源：http://wqy.hnqzz.top

[U41] PHP：初始化 Composer 项目
来源：http://zgl.cucudq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gjr.yj20258.top

[U42] PHP：PSR-4 自动加载
来源：http://zbt.kuanghao11.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://thk.gogol.net.cn

[U43] PHP：声明命名空间
来源：http://muc.zhengqikj.top

namespace App\Http;
来源：http://tog.0kj1m.cn

[U44] PHP：开启严格类型
来源：http://nhw.mhx1999.top

declare(strict_types=1);
来源：http://qun.gaohongyu789.top

[U45] PHP：类型声明与返回类型
来源：http://dlz.sweek.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://win.316326.xyz

[U46] PHP：可空类型
来源：http://zyp.zhixingplan.top

?string $name = null
来源：http://nmp.hongshengwenyu.top

[U47] PHP：联合类型
来源：http://tyl.hfpthk.cn

int|string $id
来源：http://kzu.guowangkeji.top

[U48] PHP：纯枚举
来源：http://tkb.316326.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wmy.ybcxt.top

[U49] PHP：只读属性
来源：http://aqc.jyoumei.cn

public readonly string $name
来源：http://kyu.yuxming.cn

[U50] PHP：构造器属性提升
来源：http://kum.cashguo.top

public function __construct(private int $id) {}
来源：http://tmv.ydzc1.top

[U51] PHP：数组解构
来源：http://twy.xylfe.cn

[$a, $b] = $arr;
来源：http://sko.jinghuilouyu.cn

[U52] PHP：箭头函数
来源：http://dgz.xinyue.icu

$double = fn($x) => $x * 2;
来源：http://tur.yfazqb.com

[U53] PHP：空合并运算符
来源：http://dfe.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://euu.guowangkeji.top

[U54] PHP：空安全调用
来源：http://crw.xuanzx.com

$obj?->method()
来源：http://qax.yj20258888.top


<!-- 参考信息 -->