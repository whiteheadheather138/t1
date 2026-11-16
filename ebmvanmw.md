代发 wailian999

#ifndef X_H
来源：http://rxe.daria6918.cn

#define X_H
来源：http://pcc.zycfv.cn

#endif
来源：http://nzf.yangfankeji.com

[S31] C++：Hello World
来源：http://wcr.sufxvd.cn

#include <iostream>
来源：http://lqw.fengsongda.top

int main() { std::cout << "Hello\n"; }
来源：http://pwt.bbcook.cn

[S32] C++：字符串
来源：http://mvm.jyoumei.cn

std::string s = "hi";  s += "!";
来源：http://ssd.yuanzhike.top

[S33] C++：vector 增删
来源：http://iip.meibo888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bzh.9152youxi.cn

[S34] C++：遍历 vector
来源：http://oer.yvedp.cn

for (auto &x : v) { std::cout << x; }
来源：http://fdt.zhijiandao.cn

[S35] C++：map
来源：http://wqh.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sjq.jlsjyb.cn

[S36] C++：unordered_map
来源：http://whw.snrcjt.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://taj.yuanzhike.top

[S37] C++：set
来源：http://nxm.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vtt.dianchejie.cn

[S38] C++：排序
来源：http://err.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://yop.ivvv.top

[S39] C++：自定义比较器排序
来源：http://myb.yangfankeji.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aux.gogol.net.cn

[S40] C++：查找元素
来源：http://xab.xinyue.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nvn.yuanzhike.top

[S41] C++：类与构造函数
来源：http://uas.mhx1999.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pec.xziqi.cn

[S42] C++：继承与虚函数
来源：http://pxr.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://cxz.sufxvd.cn

[S43] C++：智能指针
来源：http://wgz.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://ehj.ydjk.org.cn

[S44] C++：引用传参
来源：http://lff.bbcook.cn

void inc(int &x) { ++x; }
来源：http://fcd.ehwqpu.com

[S45] C++：lambda
来源：http://orj.tarul.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ytd.jinqigufen.top

[S46] C++：函数模板
来源：http://yri.vqdsnc.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kby.yj20258888.top

[S47] C++：结构化绑定遍历
来源：http://qoh.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hhp.jlsjyb.cn

[S48] C++：逐行读文件
来源：http://wwq.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gqf.zycfv.cn

while (std::getline(in, line)) { }
来源：http://hls.zdqjudy.top

[S49] C++：写文件
来源：http://chz.xuanzx.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tug.yj20258.top

[S50] C++：格式化数字
来源：http://cjz.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yvo.zdqjudy.top

[S51] C++：显式类型转换
来源：http://dms.meibo888.top

static_cast<double>(a) / b
来源：http://xwh.zdqjudy.top

[S52] C++：const 与 noexcept
来源：http://byh.yfazqb.com

int size() const noexcept { return n_; }
来源：http://dgt.nanxuanxn.top

[S53] C++：移动语义
来源：http://iyh.sxryk.cn

std::vector<int> w = std::move(v);
来源：http://mzr.yvedp.cn

[S54] C++：异常处理
来源：http://sjc.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mjc.sxryk.cn

[S55] C++：结构化绑定
来源：http://jgq.fanxiaobao.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://sxn.zhixingplan.top

[S56] C++：optional
来源：http://ftk.pengpengdd.cyou

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lan.tarul.cn

[S57] C++：编译期常量
来源：http://lni.shanyushiyangkeji.top

constexpr int N = 10;
来源：http://cim.fzhhl.top

[S58] C++：命名空间
来源：http://exd.cucudq.cn

namespace ns { int f() { return 1; } }
来源：http://fml.hnqzz.top

[S59] C++：静态断言
来源：http://gga.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zra.zdbjq.cn

[S60] C++：遍历并删除元素
来源：http://wvv.haohaochexian.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rdm.zhongyouzk.top

================================================================================
来源：http://zpp.hnqzz.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ptg.dashuyun.cn

================================================================================
来源：http://hfw.zycfv.cn

[T01] Kotlin：Hello World
来源：http://xaz.quarkkingdee.top

println("Hello")
来源：http://wrk.fzhhl.top

[T02] Kotlin：变量
来源：http://cdl.wangshuangyany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mhv.ydzc1.top

[T03] Kotlin：字符串模板
来源：http://qrg.jlsjyb.cn

"值: $b"
来源：http://mre.zhaomingkeji.xyz

[T04] Kotlin：空安全
来源：http://szv.yangfankeji.com

val n: String? = null;  n?.length
来源：http://gej.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://bxm.xziqi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oku.jyoumei.cn

[T06] Kotlin：集合映射
来源：http://qdr.ivvv.top

listOf(1, 2, 3).map { it * 2 }
来源：http://smo.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://mvo.smart0.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://hiu.fzhhl.top

[T08] Kotlin：数据类
来源：http://met.sysykeji.top

data class User(val name: String, val age: Int)
来源：http://nqk.jiagoushi.top

[T09] Kotlin：扩展函数
来源：http://aat.sufxvd.cn

fun String.exclaim() = this + "!"
来源：http://cpe.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://rwg.sufxvd.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://frl.wangdashe.top

[T11] Kotlin：协程
来源：http://lmy.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://igt.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://fro.guowangkeji.top

val (a, b) = Pair(1, 2)
来源：http://oqx.cashguo.top

[T13] Kotlin：只读 Map
来源：http://spl.yuxming.cn

val m = mapOf("a" to 1)
来源：http://kdk.daxiang520.top

[T14] Kotlin：循环
来源：http://fmy.ydjk.org.cn

for (i in 1..10) println(i)
来源：http://enu.bbcook.cn

[T15] Kotlin：接口
来源：http://oac.svipenyu.cn

interface Shape { fun area(): Double }
来源：http://yza.yuanzhike.top

[T16] Swift：Hello World
来源：http://cha.yuxming.cn

print("Hello")
来源：http://dgu.zhixingplan.top

[T17] Swift：变量与常量
来源：http://vnh.yuxming.cn

var a = 1;  let b = 2
来源：http://cnv.tianlin.xyz

[T18] Swift：字符串插值
来源：http://jon.vqdsnc.cn

"值: \(b)"
来源：http://qyc.snrcjt.cn

[T19] Swift：可选绑定
来源：http://bwj.fzhhl.top

if let n = opt { print(n) }
来源：http://hfs.yj20258888.top

[T20] Swift：数组操作
来源：http://xcf.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://vpu.bbcook.cn

[T21] Swift：遍历
来源：http://rbx.jianghu66.top

for x in a { print(x) }
来源：http://lqs.jyoumei.cn

[T22] Swift：字典
来源：http://rkh.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://ujt.chenlongwang.top

[T23] Swift：函数
来源：http://nji.tarul.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lmo.zycfv.cn

[T24] Swift：闭包
来源：http://xpf.iojbl.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uvn.daria6918.cn

[T25] Swift：结构体
来源：http://ksu.yongpay.top

struct P { var x: Int }
来源：http://uee.gotoacloud.top

[T26] Swift：类与重写
来源：http://jvc.redwolf501.top

class A: Base { override func f() {} }
来源：http://dpx.jqgfzy.top

[T27] Swift：错误处理
来源：http://use.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://tgv.shzxlz.cn

[T28] Swift：枚举
来源：http://azm.guowangkeji.top

enum Color { case red, green }
来源：http://kib.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://xeu.bbcook.cn

guard let x = opt else { return }
来源：http://hdc.ywan-chungtsiang.top

[T30] Swift：协议
来源：http://qvy.fehbvm.com

protocol Shape { func area() -> Double }
来源：http://srp.jlsjyb.cn

[T31] Lua：Hello World
来源：http://seh.52xcode.cn

print("Hello")
来源：http://dzx.ivvv.top

[T32] Lua：局部变量
来源：http://gmz.wangdashe.top

local a = 1
来源：http://ixd.iojbl.cn

[T33] Lua：表（数组）
来源：http://vds.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rmh.jqgufenzy.top

[T34] Lua：遍历表
来源：http://vbp.aibaodan.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mqx.chenzaomai.com

[T35] Lua：字典表
来源：http://kqs.cucudq.cn

local d = { a = 1 };  d.b = 2
来源：http://hzs.tianlin.xyz

[T36] Lua：函数
来源：http://dnt.316326.xyz

function add(a, b) return a + b end
来源：http://hqh.hysaishi.cn

[T37] Lua：字符串拼接
来源：http://xnu.fanxiaobao.xyz

"a" .. "b"
来源：http://moe.yuanzhike.top

[T38] Lua：条件
来源：http://iuh.jinqigufen.top

if x > 0 then print("正") end
来源：http://mwn.zhoulong.xyz

[T39] Lua：模式匹配
来源：http://xhw.cucudq.cn

string.find(s, "%d+")
来源：http://ogg.fanxiaobao.xyz

[T40] Lua：元表
来源：http://fsw.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://ohu.andypj.xyz

[T41] Perl：Hello World
来源：http://uwz.hfpthk.cn

print "Hello\n";
来源：http://lmm.yongpay.top

[T42] Perl：变量类型
来源：http://rzx.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jen.wangdashe.top

[T43] Perl：字符串插值
来源：http://tfr.c1oappe.top

"值: $a"
来源：http://qpx.ywan-chungtsiang.top

[T44] Perl：条件
来源：http://keg.sufxvd.cn

if ($a > 0) { print "正"; }
来源：http://bpz.meibo888.top

[T45] Perl：数组遍历
来源：http://unv.hywenlv.cn

for my $x (@arr) { print $x; }
来源：http://npu.ybcxt.top

[T46] Perl：哈希操作
来源：http://zuh.jinqigfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bno.shuidangran.top

[T47] Perl：正则捕获
来源：http://wmh.cashguo.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wsn.xinyue.icu

[T48] Perl：正则替换
来源：http://dwn.hywenlv.cn

$s =~ s/old/new/g;
来源：http://uzw.jiagoushi.top

[T49] Perl：函数
来源：http://otr.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ucf.yj202588.top

[T50] Perl：逐行读文件
来源：http://efe.fktsv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jfe.ydjk.org.cn

while (my $line = <$fh>) { print $line; }
来源：http://kha.jinyuanbaomall.cn

[T51] Scala：Hello World
来源：http://oxn.0kj1m.cn

println("Hello")
来源：http://xtj.cashguo.top

[T52] Scala：变量
来源：http://wtt.uphjek.com

val a = 1;  var b = 2
来源：http://pbb.zycfv.cn

[T53] Scala：字符串插值
来源：http://opd.yonumen.top

s"值: $b"
来源：http://isn.jinqigfzy.top

[T54] Scala：集合映射
来源：http://dfw.feifeiyinyue.top

List(1, 2, 3).map(_ * 2)
来源：http://syv.ybcxt.top

[T55] Scala：集合过滤
来源：http://cwy.jinqigufen.top

List(1, 2, 3).filter(_ > 1)
来源：http://ubr.zdbjq.cn

[T56] Scala：样例类
来源：http://zdx.zhengqikj.top

case class User(name: String, age: Int)
来源：http://dfn.mhx1999.top

[T57] Scala：模式匹配
来源：http://ysu.hammf.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://acx.nanxinkj.top

[T58] Scala：函数定义
来源：http://pxe.sufxvd.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gsg.hnxiangtu.top

[T59] Scala：循环
来源：http://har.kuanghao11.cn

for (i <- 1 to 10) println(i)
来源：http://dec.nanxuanxn.top

[T60] Scala：折叠
来源：http://ikd.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jus.vqdsnc.cn

================================================================================
来源：http://ebr.vqdsnc.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bhr.cheryme.top

================================================================================
来源：http://vec.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://val.dashuyun.cn

python -m venv .venv && source .venv/bin/activate
来源：http://btu.xinyue.icu

[U02] Py：导出 / 安装依赖
来源：http://hpl.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://stu.mhx1999.top

[U03] Py：加载 .env 配置
来源：http://cfx.sysykeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xda.vqdsnc.cn

[U04] Py：变量调试打印
来源：http://rhz.aibaodan.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xax.zhijiandao.cn

[U05] Py：列表去重且保序
来源：http://sls.sufxvd.cn

list(dict.fromkeys(arr))
来源：http://igd.jiagoushi.top

[U06] Py：合并两个字典
来源：http://mpw.yonumen.top

{**a, **b}
来源：http://axb.cqqwz.cn

[U07] Py：反转字典键值
来源：http://xvu.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://lci.yongpay.top

[U08] Py：展平二维列表
来源：http://uwh.gogol.net.cn

[y for x in nested for y in x]
来源：http://jdg.tianlin.xyz

[U09] Py：字典取最大值的键
来源：http://yaa.zhixingplan.top

max(d, key=d.get)
来源：http://rwp.nanxinkj.top

[U10] Py：按值排序字典
来源：http://zae.shanyushiyangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://smq.pengpengdd.cyou

[U11] Py：生成器表达式
来源：http://rgg.chenlongwang.top

(x * 2 for x in arr)
来源：http://tdz.fanxiaobao.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://nrz.zhaomingkeji.xyz

Counter(arr).most_common(3)
来源：http://rmz.xylfe.cn

[U13] Py：固定长度队列
来源：http://ssm.shanyushiyangkeji.top

deque(maxlen=10)
来源：http://aow.nanxinkj.top

[U14] Py：分组收集到列表
来源：http://mzl.hongshengwenyu.top

defaultdict(list)
来源：http://age.tarul.cn

[U15] Py：高精度计时
来源：http://jsb.kuanghao11.cn

t = time.perf_counter()
来源：http://lut.ivvv.top

[U16] Py：命令行参数解析
来源：http://mcb.hnqzz.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wqo.yueranfly.top

[U17] Py：初始化日志
来源：http://iko.kuanghao11.cn

logging.basicConfig(level=logging.INFO)
来源：http://ebd.tian-w.cn

[U18] Py：预编译正则
来源：http://kzb.vqdsnc.cn

pat = re.compile(r"\d+")
来源：http://isv.jlsjyb.cn

[U19] Py：正则替换带回调
来源：http://qbp.tarul.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xtd.sxryk.cn

[U20] Py：缓存函数结果
来源：http://hwa.nanxinkj.top

@functools.lru_cache(maxsize=None)
来源：http://udv.chenzaomai.com

[U21] Py：自定义上下文管理器
来源：http://wes.zdbjq.cn

@contextlib.contextmanager
来源：http://mhz.zhongyouzk.top

[U22] Py：矩阵转置
来源：http://cuy.zhengqikj.top

list(zip(*m))
来源：http://jdo.haohaochexian.top

[U23] Py：分块读取大文件
来源：http://aiu.cashguo.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://acp.kuanghao11.cn

[U24] Py：路径操作
来源：http://uht.jinghuilouyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://glz.jqgfzy.top

[U25] Py：CSV 按字典读
来源：http://wdt.jinqigfzy.top

csv.DictReader(f)
来源：http://fpf.chenjidiqi.icu

[U26] Py：并发下载
来源：http://tbp.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://foz.haohaochexian.top

[U27] Py：异步 HTTP
来源：http://dzy.shuidangran.top

aiohttp.ClientSession() 配合 async with
来源：http://zbm.0kj1m.cn

[U28] Py：类型别名
来源：http://ccb.sufxvd.cn

UserId = int
来源：http://nob.tian-w.cn

[U29] Py：属性校验
来源：http://dkk.feifeiyinyue.top

@property 与 @x.setter 配合
来源：http://cnn.52xcode.cn

[U30] Py：数据类
来源：http://bik.chenjidiqi.icu

@dataclass(slots=True)
来源：http://xul.haohaochexian.top

[U31] Py：单测
来源：http://rho.ybcxt.top

python -m pytest -q
来源：http://tpz.yuxming.cn

[U32] Py：代码格式化
来源：http://aky.cdnleiting.top

ruff format . && ruff check --fix .
来源：http://ety.tarul.cn

[U33] Py：打包发布
来源：http://uoq.9152youxi.cn

python -m build  （依赖 pyproject.toml）
来源：http://bem.fanxiaobao.xyz

[U34] Py：判断编码
来源：http://sar.xuetiantiany.cn

chardet.detect(raw)
来源：http://jfj.daxiang520.top

[U35] Py：发送邮件
来源：http://jzv.fktsv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pra.xziqi.cn

[U36] Py：定时任务
来源：http://fal.tarul.cn

schedule.every(10).minutes.do(job)
来源：http://rpv.epnwcf.com

[U37] Py：读写 Excel
来源：http://mvd.fanxiaobao.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://lab.yvedp.cn

[U38] Py：获取脚本所在目录
来源：http://lyo.yongpay.top

Path(__file__).resolve().parent
来源：http://wxc.sweek.top

[U39] Py：判断是否在交互环境
来源：http://cly.sxryk.cn

sys.stdout.isatty()
来源：http://mgv.zdbjq.cn

[U40] Py：打印到标准错误
来源：http://ysm.hammf.cn

print("err", file=sys.stderr)
来源：http://rjc.yanxiufei.cn

[U41] PHP：初始化 Composer 项目
来源：http://ljw.chenzaomai.com

composer init;  composer require guzzlehttp/guzzle
来源：http://wbj.chenlongwang.top

[U42] PHP：PSR-4 自动加载
来源：http://mdt.andypj.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xci.jinyuanbaomall.cn

[U43] PHP：声明命名空间
来源：http://abo.feifeiyinyue.top

namespace App\Http;
来源：http://lmk.jqgfzy.top

[U44] PHP：开启严格类型
来源：http://ltv.yongpay.top

declare(strict_types=1);
来源：http://pnm.mhx1999.top

[U45] PHP：类型声明与返回类型
来源：http://zof.jlsjyb.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hlf.jinqigfzy.top

[U46] PHP：可空类型
来源：http://bxt.gzhubu.top

?string $name = null
来源：http://aqm.hywenlv.cn

[U47] PHP：联合类型
来源：http://vwv.chenzaomai.com

int|string $id
来源：http://riq.sjlbkw.cn

[U48] PHP：纯枚举
来源：http://jpv.gotoacloud.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fqe.birdmap.top

[U49] PHP：只读属性
来源：http://pqy.9152youxi.cn

public readonly string $name
来源：http://izw.c1oappe.top

[U50] PHP：构造器属性提升
来源：http://xii.zhiwuduotai.top

public function __construct(private int $id) {}
来源：http://abe.dashuyun.cn

[U51] PHP：数组解构
来源：http://kgn.hysaishi.cn

[$a, $b] = $arr;
来源：http://ynv.tanke756.top

[U52] PHP：箭头函数
来源：http://rsj.zycfv.cn

$double = fn($x) => $x * 2;
来源：http://txv.meibo888.top

[U53] PHP：空合并运算符
来源：http://www.xylfe.cn

$v = $a ?? $b ?? "default";
来源：http://lwr.fzhhl.top

[U54] PHP：空安全调用
来源：http://uxa.hfpthk.cn

$obj?->method()
来源：http://kqc.yj20258.top


<!-- 参考信息 -->