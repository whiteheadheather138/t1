代发 wailian999

#include <iostream>
来源：http://iop.quarkkingdee.top

int main() { std::cout << "Hello\n"; }
来源：http://rsp.sjlbkw.cn

[S32] C++：字符串
来源：http://uoy.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://eue.cqqwz.cn

[S33] C++：vector 增删
来源：http://cso.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gcm.andypj.xyz

[S34] C++：遍历 vector
来源：http://jqa.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://wms.yuxming.cn

[S35] C++：map
来源：http://gys.yj202588.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zpp.feifeiyinyue.top

[S36] C++：unordered_map
来源：http://bbb.xingfuxueyuan.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://con.sjlbkw.cn

[S37] C++：set
来源：http://giq.cheryme.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://slw.kuanghao11.cn

[S38] C++：排序
来源：http://uco.meibo888.top

std::sort(v.begin(), v.end());
来源：http://vra.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://cgg.316326.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vxl.xuanzx.com

[S40] C++：查找元素
来源：http://nlf.hnqzz.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fci.dashuyun.cn

[S41] C++：类与构造函数
来源：http://aoq.ydzc1.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rqe.birdmap.top

[S42] C++：继承与虚函数
来源：http://nus.hnxiangtu.top

class B : public Base { public: void f() override {} };
来源：http://iqr.hongshengwenyu.top

[S43] C++：智能指针
来源：http://bkq.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://psa.tianlin.xyz

[S44] C++：引用传参
来源：http://cfj.cheryme.top

void inc(int &x) { ++x; }
来源：http://qsx.havefunace.top

[S45] C++：lambda
来源：http://abt.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ozs.cqqwz.cn

[S46] C++：函数模板
来源：http://nvy.shanyushiyangtech.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bfx.xingfuxueyuan.xyz

[S47] C++：结构化绑定遍历
来源：http://obu.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wvu.bjfxy.top

[S48] C++：逐行读文件
来源：http://sjb.dianchejie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jdt.aibaodan.cn

while (std::getline(in, line)) { }
来源：http://wrt.hongshengwenyu.top

[S49] C++：写文件
来源：http://jon.fzhhl.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qck.hongshengwenyu.top

[S50] C++：格式化数字
来源：http://xyn.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ggg.nwbrower.top

[S51] C++：显式类型转换
来源：http://htb.svipenyu.cn

static_cast<double>(a) / b
来源：http://wxz.zhijiandao.cn

[S52] C++：const 与 noexcept
来源：http://kvd.ybcxt.top

int size() const noexcept { return n_; }
来源：http://xue.ydzc1.top

[S53] C++：移动语义
来源：http://kcs.wangshuangyany.cn

std::vector<int> w = std::move(v);
来源：http://osw.hongshengwenyu.top

[S54] C++：异常处理
来源：http://mmj.pengpengdd.cyou

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yej.daria6918.cn

[S55] C++：结构化绑定
来源：http://ais.shuidangran.top

auto [a, b] = std::make_pair(1, 2);
来源：http://syk.zhengqikj.top

[S56] C++：optional
来源：http://uic.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://moe.yj202588.top

[S57] C++：编译期常量
来源：http://chb.ybcxt.top

constexpr int N = 10;
来源：http://jsa.hnqzz.top

[S58] C++：命名空间
来源：http://fia.ydjk.org.cn

namespace ns { int f() { return 1; } }
来源：http://lqh.zhaomingkeji.xyz

[S59] C++：静态断言
来源：http://wjj.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qck.tanke756.top

[S60] C++：遍历并删除元素
来源：http://nbn.zdbjq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dgv.hongshengwenyu.top

================================================================================
来源：http://cif.cucudq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ddr.zhijiandao.cn

================================================================================
来源：http://tqp.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://qyd.cucudq.cn

println("Hello")
来源：http://ins.zhijiandao.cn

[T02] Kotlin：变量
来源：http://cpp.zhixingplan.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vis.yj202588.top

[T03] Kotlin：字符串模板
来源：http://fhr.bjfxy.top

"值: $b"
来源：http://sha.zhengqikj.top

[T04] Kotlin：空安全
来源：http://xil.zhoulong.xyz

val n: String? = null;  n?.length
来源：http://rhr.yuxming.cn

[T05] Kotlin：when 表达式
来源：http://ulv.guowangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fpr.ctjpmb.com

[T06] Kotlin：集合映射
来源：http://smr.dashuyun.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rxu.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://njb.sysykeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fmj.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://lks.fehbvm.com

data class User(val name: String, val age: Int)
来源：http://byp.yj20258.top

[T09] Kotlin：扩展函数
来源：http://pqx.feifeiyinyue.top

fun String.exclaim() = this + "!"
来源：http://kwg.fengsongda.top

[T10] Kotlin：默认参数
来源：http://tnn.52xcode.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lvj.hfpthk.cn

[T11] Kotlin：协程
来源：http://vpc.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yll.wangdashe.top

[T12] Kotlin：解构声明
来源：http://thj.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://huj.gogol.net.cn

[T13] Kotlin：只读 Map
来源：http://pas.gzhubu.top

val m = mapOf("a" to 1)
来源：http://yiq.jqgufenzy.top

[T14] Kotlin：循环
来源：http://utm.yj20258888.top

for (i in 1..10) println(i)
来源：http://cfa.xuanzx.com

[T15] Kotlin：接口
来源：http://mwc.ydjk.org.cn

interface Shape { fun area(): Double }
来源：http://fzp.yonumen.top

[T16] Swift：Hello World
来源：http://puw.shanyushiyangtech.top

print("Hello")
来源：http://heg.quarkkingdee.top

[T17] Swift：变量与常量
来源：http://crd.jlsjyb.cn

var a = 1;  let b = 2
来源：http://bsr.yonumen.top

[T18] Swift：字符串插值
来源：http://nnk.bjfxy.top

"值: \(b)"
来源：http://abg.52xcode.cn

[T19] Swift：可选绑定
来源：http://rqg.ehwqpu.com

if let n = opt { print(n) }
来源：http://mmi.fzhhl.top

[T20] Swift：数组操作
来源：http://trs.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://zxn.snrcjt.cn

[T21] Swift：遍历
来源：http://ejf.chenjidiqi.icu

for x in a { print(x) }
来源：http://aoe.sweek.top

[T22] Swift：字典
来源：http://cmn.fanxiaobao.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://aki.jianghu66.top

[T23] Swift：函数
来源：http://mld.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bkc.zhoulong.xyz

[T24] Swift：闭包
来源：http://eol.jqgufenzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lcy.iojbl.cn

[T25] Swift：结构体
来源：http://lvg.hnqzz.top

struct P { var x: Int }
来源：http://vga.haohaochexian.top

[T26] Swift：类与重写
来源：http://yel.fehbvm.com

class A: Base { override func f() {} }
来源：http://mdo.sweek.top

[T27] Swift：错误处理
来源：http://dxq.redwolf501.top

do { try f() } catch { print(error) }
来源：http://yhs.vqdsnc.cn

[T28] Swift：枚举
来源：http://goj.hammf.cn

enum Color { case red, green }
来源：http://iqw.yj20258.top

[T29] Swift：guard 提前返回
来源：http://oed.shuidangran.top

guard let x = opt else { return }
来源：http://qee.dianchejie.cn

[T30] Swift：协议
来源：http://xsc.nwbrower.top

protocol Shape { func area() -> Double }
来源：http://biv.smart0.xyz

[T31] Lua：Hello World
来源：http://gzr.316326.xyz

print("Hello")
来源：http://xex.andypj.xyz

[T32] Lua：局部变量
来源：http://dex.fanxiaobao.xyz

local a = 1
来源：http://nfz.xuetiantiany.cn

[T33] Lua：表（数组）
来源：http://icg.pycfn.com

local t = {1, 2, 3};  t[4] = 4
来源：http://scd.yj20258888.top

[T34] Lua：遍历表
来源：http://fae.snrcjt.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://duu.jyoumei.cn

[T35] Lua：字典表
来源：http://edv.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://ahh.zhongyouzk.top

[T36] Lua：函数
来源：http://vox.birdmap.top

function add(a, b) return a + b end
来源：http://bhq.vehdjk.com

[T37] Lua：字符串拼接
来源：http://xuh.yuxming.cn

"a" .. "b"
来源：http://crs.jiagoushi.top

[T38] Lua：条件
来源：http://lvo.yuanzhike.top

if x > 0 then print("正") end
来源：http://uaz.hysaishi.cn

[T39] Lua：模式匹配
来源：http://jio.yonumen.top

string.find(s, "%d+")
来源：http://dqv.jinyuanbaomall.cn

[T40] Lua：元表
来源：http://ume.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://gjh.shuidangran.top

[T41] Perl：Hello World
来源：http://gyd.cucudq.cn

print "Hello\n";
来源：http://yrb.yangfankeji.com

[T42] Perl：变量类型
来源：http://ejg.hfpthk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ntu.daxiang520.top

[T43] Perl：字符串插值
来源：http://ptc.daria6918.cn

"值: $a"
来源：http://gtk.andypj.xyz

[T44] Perl：条件
来源：http://srg.yanxiufei.cn

if ($a > 0) { print "正"; }
来源：http://qzt.zhiwuduotai.top

[T45] Perl：数组遍历
来源：http://izu.hnxiangtu.top

for my $x (@arr) { print $x; }
来源：http://rjw.jlsjyb.cn

[T46] Perl：哈希操作
来源：http://npy.chenzaomai.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dni.vqdsnc.cn

[T47] Perl：正则捕获
来源：http://pyq.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uxg.nanxinkj.top

[T48] Perl：正则替换
来源：http://xrk.xinyue.icu

$s =~ s/old/new/g;
来源：http://cmc.xziqi.cn

[T49] Perl：函数
来源：http://mpb.guowangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vww.xziqi.cn

[T50] Perl：逐行读文件
来源：http://sex.xuetiantiany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wma.zhijiandao.cn

while (my $line = <$fh>) { print $line; }
来源：http://tob.sysykeji.top

[T51] Scala：Hello World
来源：http://juh.gogol.net.cn

println("Hello")
来源：http://frr.guowangkeji.top

[T52] Scala：变量
来源：http://ghl.xingfuxueyuan.xyz

val a = 1;  var b = 2
来源：http://cdb.smart0.xyz

[T53] Scala：字符串插值
来源：http://gqr.zhijiandao.cn

s"值: $b"
来源：http://afx.fengsongda.top

[T54] Scala：集合映射
来源：http://dqb.yfazqb.com

List(1, 2, 3).map(_ * 2)
来源：http://wmr.pycfn.com

[T55] Scala：集合过滤
来源：http://tbi.sweek.top

List(1, 2, 3).filter(_ > 1)
来源：http://pru.zhiwuduotai.top

[T56] Scala：样例类
来源：http://thp.gaohongyu789.top

case class User(name: String, age: Int)
来源：http://rqd.hysaishi.cn

[T57] Scala：模式匹配
来源：http://znb.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bdz.gotoacloud.top

[T58] Scala：函数定义
来源：http://nym.zhiwuduotai.top

def add(a: Int, b: Int): Int = a + b
来源：http://yng.shuidangran.top

[T59] Scala：循环
来源：http://vzu.quarkkingdee.top

for (i <- 1 to 10) println(i)
来源：http://csg.xuetiantiany.cn

[T60] Scala：折叠
来源：http://ttw.wangdashe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cuz.redwolf501.top

================================================================================
来源：http://ram.ivvv.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aua.yueranfly.top

================================================================================
来源：http://cua.vehdjk.com

[U01] Py：创建虚拟环境
来源：http://fyi.yuanzhike.top

python -m venv .venv && source .venv/bin/activate
来源：http://jda.chenjidiqi.icu

[U02] Py：导出 / 安装依赖
来源：http://uep.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jpa.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://toj.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oys.aizwys.cn

[U04] Py：变量调试打印
来源：http://rqd.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://asv.zhaomingkeji.xyz

[U05] Py：列表去重且保序
来源：http://sbz.hesvh.cn

list(dict.fromkeys(arr))
来源：http://ssh.xingfuxueyuan.xyz

[U06] Py：合并两个字典
来源：http://vkz.zhongyouzk.top

{**a, **b}
来源：http://ejd.uphjek.com

[U07] Py：反转字典键值
来源：http://ghw.aibaodan.cn

{v: k for k, v in d.items()}
来源：http://uzn.hcnkem.com

[U08] Py：展平二维列表
来源：http://lsh.xingfuxueyuan.xyz

[y for x in nested for y in x]
来源：http://fag.sjlbkw.cn

[U09] Py：字典取最大值的键
来源：http://bme.daxiang520.top

max(d, key=d.get)
来源：http://wmw.hongshengwenyu.top

[U10] Py：按值排序字典
来源：http://vqe.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tjm.guannengcc.top

[U11] Py：生成器表达式
来源：http://riu.zhiwuduotai.top

(x * 2 for x in arr)
来源：http://jmn.aizwys.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pwb.shanyushiyangkeji.top

Counter(arr).most_common(3)
来源：http://qey.zdqjudy.top

[U13] Py：固定长度队列
来源：http://qdm.cheryme.top

deque(maxlen=10)
来源：http://dyi.sjlbkw.cn

[U14] Py：分组收集到列表
来源：http://wdq.bjfxy.top

defaultdict(list)
来源：http://fre.hongshengwenyu.top

[U15] Py：高精度计时
来源：http://vig.xziqi.cn

t = time.perf_counter()
来源：http://dsg.pengpengdd.cyou

[U16] Py：命令行参数解析
来源：http://ilt.svipenyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jwy.gotoacloud.top

[U17] Py：初始化日志
来源：http://mzv.fanxiaobao.xyz

logging.basicConfig(level=logging.INFO)
来源：http://pud.ctjpmb.com

[U18] Py：预编译正则
来源：http://thi.hywenlv.cn

pat = re.compile(r"\d+")
来源：http://xnq.tianlin.xyz

[U19] Py：正则替换带回调
来源：http://ovk.cheryme.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qli.sjlbkw.cn

[U20] Py：缓存函数结果
来源：http://qma.fanxiaobao.xyz

@functools.lru_cache(maxsize=None)
来源：http://idv.52xcode.cn

[U21] Py：自定义上下文管理器
来源：http://fyy.haohaochexian.top

@contextlib.contextmanager
来源：http://tfa.meibo888.top

[U22] Py：矩阵转置
来源：http://prv.epnwcf.com

list(zip(*m))
来源：http://wuf.cucudq.cn

[U23] Py：分块读取大文件
来源：http://gjt.xingfuxueyuan.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://osx.snrcjt.cn

[U24] Py：路径操作
来源：http://vsj.shzxlz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jqp.xinyue.icu

[U25] Py：CSV 按字典读
来源：http://fjj.tarul.cn

csv.DictReader(f)
来源：http://qak.ydjk.org.cn

[U26] Py：并发下载
来源：http://bzj.yvedp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iis.fehbvm.com

[U27] Py：异步 HTTP
来源：http://gqr.jinghuilouyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://tdj.jinqigufen.top

[U28] Py：类型别名
来源：http://kqz.hcnkem.com

UserId = int
来源：http://vhf.zhiwuduotai.top

[U29] Py：属性校验
来源：http://mln.xuetiantiany.cn

@property 与 @x.setter 配合
来源：http://yjr.tarul.cn

[U30] Py：数据类
来源：http://uze.hfpthk.cn

@dataclass(slots=True)
来源：http://ffh.9152youxi.cn

[U31] Py：单测
来源：http://bkl.gzhubu.top

python -m pytest -q
来源：http://xwc.zdqjudy.top

[U32] Py：代码格式化
来源：http://cju.xinyue.icu

ruff format . && ruff check --fix .
来源：http://teb.gaohongyu789.top

[U33] Py：打包发布
来源：http://ili.xinyue.icu

python -m build  （依赖 pyproject.toml）
来源：http://fca.xuetiantiany.cn

[U34] Py：判断编码
来源：http://ngq.daxiang520.top

chardet.detect(raw)
来源：http://uuu.hammf.cn

[U35] Py：发送邮件
来源：http://skr.fktsv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uys.xinyue.icu

[U36] Py：定时任务
来源：http://kum.gogol.net.cn

schedule.every(10).minutes.do(job)
来源：http://nxn.sysykeji.top

[U37] Py：读写 Excel
来源：http://neu.shuidangran.top

pandas.read_excel / DataFrame.to_excel
来源：http://ykd.hysaishi.cn

[U38] Py：获取脚本所在目录
来源：http://csf.chenjidiqi.icu

Path(__file__).resolve().parent
来源：http://myv.quarkkingdee.top

[U39] Py：判断是否在交互环境
来源：http://fjx.cheryme.top

sys.stdout.isatty()
来源：http://xdj.hammf.cn

[U40] Py：打印到标准错误
来源：http://xbk.jinqigfzy.top

print("err", file=sys.stderr)
来源：http://gaw.shuidangran.top

[U41] PHP：初始化 Composer 项目
来源：http://shr.cqqwz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qdn.zhongyouzk.top

[U42] PHP：PSR-4 自动加载
来源：http://vlf.bjfxy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xkp.xuetiantiany.cn

[U43] PHP：声明命名空间
来源：http://gsy.cheryme.top

namespace App\Http;
来源：http://btv.pengpengdd.cyou

[U44] PHP：开启严格类型
来源：http://ioh.jinyuanbaomall.cn

declare(strict_types=1);
来源：http://ptl.hnqzz.top

[U45] PHP：类型声明与返回类型
来源：http://ctx.aizwys.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uqp.vehdjk.com

[U46] PHP：可空类型
来源：http://bkh.xylfe.cn

?string $name = null
来源：http://lnk.zhijiandao.cn

[U47] PHP：联合类型
来源：http://qpm.daria6918.cn

int|string $id
来源：http://zfy.shangyingyoupin.top

[U48] PHP：纯枚举
来源：http://grc.ppjwa.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://stk.xuanzx.com

[U49] PHP：只读属性
来源：http://bpi.jyoumei.cn

public readonly string $name
来源：http://cbi.sufxvd.cn

[U50] PHP：构造器属性提升
来源：http://jzk.yuanzhike.top

public function __construct(private int $id) {}
来源：http://pss.9152youxi.cn

[U51] PHP：数组解构
来源：http://coq.hesvh.cn

[$a, $b] = $arr;
来源：http://luv.hfpthk.cn

[U52] PHP：箭头函数
来源：http://smz.0kj1m.cn

$double = fn($x) => $x * 2;
来源：http://ilv.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://bfc.zhengqikj.top

$v = $a ?? $b ?? "default";
来源：http://eaf.zhixingplan.top

[U54] PHP：空安全调用
来源：http://dms.fengsongda.top

$obj?->method()
来源：http://tyr.9152youxi.cn

[U55] PHP：match 表达式
来源：http://fnu.yuanzhike.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xwq.cheryme.top

[U56] PHP：命名参数
来源：http://obz.zhengqikj.top

f(a: 1, b: 2)
来源：http://qea.redwolf501.top


<!-- 参考信息 -->