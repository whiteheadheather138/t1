代发 wailian999

#ifndef X_H
来源：http://esw.sjlbkw.cn

#define X_H
来源：http://fkb.tarul.cn

#endif
来源：http://gsi.gaohongyu789.top

[S31] C++：Hello World
来源：http://wzv.ehwqpu.com

#include <iostream>
来源：http://uwx.gaohongyu789.top

int main() { std::cout << "Hello\n"; }
来源：http://nhd.wangshuangyany.cn

[S32] C++：字符串
来源：http://kwo.uphjek.com

std::string s = "hi";  s += "!";
来源：http://vjh.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://eqy.hcnkem.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://axt.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://xgp.guowangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://pan.yuanzhike.top

[S35] C++：map
来源：http://iuq.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://low.tanke756.top

[S36] C++：unordered_map
来源：http://hus.pycfn.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ztn.andypj.xyz

[S37] C++：set
来源：http://jah.xingfuxueyuan.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://grn.jinqigufen.top

[S38] C++：排序
来源：http://igk.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://ord.hesvh.cn

[S39] C++：自定义比较器排序
来源：http://rno.yonumen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lbj.fengsongda.top

[S40] C++：查找元素
来源：http://qvg.sjlbkw.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://unn.meibo888.top

[S41] C++：类与构造函数
来源：http://ksn.wangdashe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ngl.xylfe.cn

[S42] C++：继承与虚函数
来源：http://qsg.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://xrb.tianlin.xyz

[S43] C++：智能指针
来源：http://efd.sjlbkw.cn

auto p = std::make_unique<int>(5);
来源：http://hfy.fengsongda.top

[S44] C++：引用传参
来源：http://oih.tanke756.top

void inc(int &x) { ++x; }
来源：http://zpn.zhaomingkeji.xyz

[S45] C++：lambda
来源：http://kms.yanxiufei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yep.jqgufenzy.top

[S46] C++：函数模板
来源：http://qhw.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wjt.fanxiaobao.xyz

[S47] C++：结构化绑定遍历
来源：http://aoe.ydjk.org.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cvx.vehdjk.com

[S48] C++：逐行读文件
来源：http://hlf.redwolf501.top

std::ifstream in("a.txt");  std::string line;
来源：http://nva.zhiwuduotai.top

while (std::getline(in, line)) { }
来源：http://cjc.yuanzhike.top

[S49] C++：写文件
来源：http://olp.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hvn.jinqigfzy.top

[S50] C++：格式化数字
来源：http://cyx.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nzi.hcnkem.com

[S51] C++：显式类型转换
来源：http://faa.yueranfly.top

static_cast<double>(a) / b
来源：http://xvl.gaohongyu789.top

[S52] C++：const 与 noexcept
来源：http://mtd.fengsongda.top

int size() const noexcept { return n_; }
来源：http://epc.kuanghao11.cn

[S53] C++：移动语义
来源：http://yso.yj20258.top

std::vector<int> w = std::move(v);
来源：http://ttk.haohaochexian.top

[S54] C++：异常处理
来源：http://rmc.jyoumei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rdk.shuidangran.top

[S55] C++：结构化绑定
来源：http://lux.hnqzz.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vya.hcnkem.com

[S56] C++：optional
来源：http://ptq.jinqigfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nhd.316326.xyz

[S57] C++：编译期常量
来源：http://ylq.quarkkingdee.top

constexpr int N = 10;
来源：http://zem.0kj1m.cn

[S58] C++：命名空间
来源：http://ivw.chenzaomai.com

namespace ns { int f() { return 1; } }
来源：http://cyx.jlsjyb.cn

[S59] C++：静态断言
来源：http://iyh.cqqwz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nhi.cdnleiting.top

[S60] C++：遍历并删除元素
来源：http://ayj.zhengqikj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qog.haohaochexian.top

================================================================================
来源：http://tbe.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zqx.jqgfzy.top

================================================================================
来源：http://ybg.jlsjyb.cn

[T01] Kotlin：Hello World
来源：http://glw.xylfe.cn

println("Hello")
来源：http://nqx.52xcode.cn

[T02] Kotlin：变量
来源：http://dzs.fktsv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xeq.jqgfzy.top

[T03] Kotlin：字符串模板
来源：http://tsi.sxryk.cn

"值: $b"
来源：http://ecc.zhongyouzk.top

[T04] Kotlin：空安全
来源：http://qxv.jinyuanbaomall.cn

val n: String? = null;  n?.length
来源：http://gro.jinqigfzy.top

[T05] Kotlin：when 表达式
来源：http://hck.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yet.sweek.top

[T06] Kotlin：集合映射
来源：http://sfy.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bvk.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://zxn.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dgk.hywenlv.cn

[T08] Kotlin：数据类
来源：http://xqj.sweek.top

data class User(val name: String, val age: Int)
来源：http://enq.hcnkem.com

[T09] Kotlin：扩展函数
来源：http://tyh.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://pgq.cashguo.top

[T10] Kotlin：默认参数
来源：http://lcr.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oxb.yongpay.top

[T11] Kotlin：协程
来源：http://ihb.sufxvd.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://whn.dashuyun.cn

[T12] Kotlin：解构声明
来源：http://qgs.wangdashe.top

val (a, b) = Pair(1, 2)
来源：http://mqz.cheryme.top

[T13] Kotlin：只读 Map
来源：http://tlj.hammf.cn

val m = mapOf("a" to 1)
来源：http://bar.aizwys.cn

[T14] Kotlin：循环
来源：http://sna.epnwcf.com

for (i in 1..10) println(i)
来源：http://spo.ppjwa.cn

[T15] Kotlin：接口
来源：http://bdm.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://kom.kuanghao11.cn

[T16] Swift：Hello World
来源：http://vwq.hnxiangtu.top

print("Hello")
来源：http://gep.shanyushiyangtech.top

[T17] Swift：变量与常量
来源：http://lxv.guowangkeji.top

var a = 1;  let b = 2
来源：http://lrp.redwolf501.top

[T18] Swift：字符串插值
来源：http://rks.nanxuanxn.top

"值: \(b)"
来源：http://dhg.52xcode.cn

[T19] Swift：可选绑定
来源：http://cmh.redwolf501.top

if let n = opt { print(n) }
来源：http://oup.pengpengdd.cyou

[T20] Swift：数组操作
来源：http://zcf.yfazqb.com

var a = [1, 2, 3];  a.append(4)
来源：http://kmw.xinyue.icu

[T21] Swift：遍历
来源：http://rlf.zycfv.cn

for x in a { print(x) }
来源：http://enh.52xcode.cn

[T22] Swift：字典
来源：http://ldb.wangdashe.top

var d = ["a": 1];  d["b"] = 2
来源：http://eqg.gogol.net.cn

[T23] Swift：函数
来源：http://qws.hywenlv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://avl.jiagoushi.top

[T24] Swift：闭包
来源：http://kox.hammf.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://huf.vqdsnc.cn

[T25] Swift：结构体
来源：http://esc.hysaishi.cn

struct P { var x: Int }
来源：http://uqh.daria6918.cn

[T26] Swift：类与重写
来源：http://tpw.yj20258888.top

class A: Base { override func f() {} }
来源：http://rfw.yonumen.top

[T27] Swift：错误处理
来源：http://uun.sxryk.cn

do { try f() } catch { print(error) }
来源：http://qyo.quarkkingdee.top

[T28] Swift：枚举
来源：http://vkn.dashuyun.cn

enum Color { case red, green }
来源：http://jxz.redwolf501.top

[T29] Swift：guard 提前返回
来源：http://xht.yangfankeji.com

guard let x = opt else { return }
来源：http://uwm.ydzc1.top

[T30] Swift：协议
来源：http://wbo.meibo888.top

protocol Shape { func area() -> Double }
来源：http://agl.dashuyun.cn

[T31] Lua：Hello World
来源：http://qlv.meibo888.top

print("Hello")
来源：http://ucx.fktsv.cn

[T32] Lua：局部变量
来源：http://xpg.pycfn.com

local a = 1
来源：http://gwv.ydjk.org.cn

[T33] Lua：表（数组）
来源：http://nnc.nanxuanxn.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mft.guowangkeji.top

[T34] Lua：遍历表
来源：http://yqz.quarkkingdee.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rpe.c1oappe.top

[T35] Lua：字典表
来源：http://gjq.jinghuilouyu.cn

local d = { a = 1 };  d.b = 2
来源：http://hhr.jqgufenzy.top

[T36] Lua：函数
来源：http://dmg.ppjwa.cn

function add(a, b) return a + b end
来源：http://yzm.ppjwa.cn

[T37] Lua：字符串拼接
来源：http://vih.gogol.net.cn

"a" .. "b"
来源：http://ydu.kuanghao11.cn

[T38] Lua：条件
来源：http://gds.sweek.top

if x > 0 then print("正") end
来源：http://rjn.yuanzhike.top

[T39] Lua：模式匹配
来源：http://hfo.zhixingplan.top

string.find(s, "%d+")
来源：http://bmd.ybcxt.top

[T40] Lua：元表
来源：http://ivh.quarkkingdee.top

setmetatable({}, { __index = base })
来源：http://eut.shzxlz.cn

[T41] Perl：Hello World
来源：http://ajc.cheryme.top

print "Hello\n";
来源：http://efi.jyoumei.cn

[T42] Perl：变量类型
来源：http://roq.yanxiufei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://knp.bbcook.cn

[T43] Perl：字符串插值
来源：http://ime.hfpthk.cn

"值: $a"
来源：http://zeg.yonumen.top

[T44] Perl：条件
来源：http://kwu.yanxiufei.cn

if ($a > 0) { print "正"; }
来源：http://elj.xylfe.cn

[T45] Perl：数组遍历
来源：http://vzz.yonumen.top

for my $x (@arr) { print $x; }
来源：http://wlj.sxryk.cn

[T46] Perl：哈希操作
来源：http://frc.tian-w.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cjw.yongpay.top

[T47] Perl：正则捕获
来源：http://ikj.shuidangran.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vgl.sufxvd.cn

[T48] Perl：正则替换
来源：http://odu.jinqigufen.top

$s =~ s/old/new/g;
来源：http://eki.ydzc1.top

[T49] Perl：函数
来源：http://ldf.yongpay.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rye.redwolf501.top

[T50] Perl：逐行读文件
来源：http://ewt.ctjpmb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://fdk.tanke756.top

while (my $line = <$fh>) { print $line; }
来源：http://gxk.sweek.top

[T51] Scala：Hello World
来源：http://yhq.jlsjyb.cn

println("Hello")
来源：http://dpx.feifeiyinyue.top

[T52] Scala：变量
来源：http://flo.cqqwz.cn

val a = 1;  var b = 2
来源：http://izs.shuidangran.top

[T53] Scala：字符串插值
来源：http://mus.jinqigufen.top

s"值: $b"
来源：http://ovf.zhixingplan.top

[T54] Scala：集合映射
来源：http://yey.gzhubu.top

List(1, 2, 3).map(_ * 2)
来源：http://wma.xziqi.cn

[T55] Scala：集合过滤
来源：http://alv.zhixingplan.top

List(1, 2, 3).filter(_ > 1)
来源：http://aah.shanyushiyangtech.top

[T56] Scala：样例类
来源：http://zum.redwolf501.top

case class User(name: String, age: Int)
来源：http://xuw.kuanghao11.cn

[T57] Scala：模式匹配
来源：http://dpi.bjfxy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fev.ivvv.top

[T58] Scala：函数定义
来源：http://sye.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://qxd.cdnleiting.top

[T59] Scala：循环
来源：http://pbd.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://yyw.52xcode.cn

[T60] Scala：折叠
来源：http://ubq.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jyf.aizwys.cn

================================================================================
来源：http://uyc.yanxiufei.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hry.zhoulong.xyz

================================================================================
来源：http://lly.yuanzhike.top

[U01] Py：创建虚拟环境
来源：http://kcn.yvedp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hab.ydjk.org.cn

[U02] Py：导出 / 安装依赖
来源：http://bii.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://axn.jianghu66.top

[U03] Py：加载 .env 配置
来源：http://ted.vehdjk.com

from dotenv import load_dotenv; load_dotenv()
来源：http://yvm.hcnkem.com

[U04] Py：变量调试打印
来源：http://cuu.zdbjq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://izx.bjfxy.top

[U05] Py：列表去重且保序
来源：http://dxb.zycfv.cn

list(dict.fromkeys(arr))
来源：http://zvs.nanxinkj.top

[U06] Py：合并两个字典
来源：http://dor.dashuyun.cn

{**a, **b}
来源：http://itx.xuetiantiany.cn

[U07] Py：反转字典键值
来源：http://vgn.yj202588.top

{v: k for k, v in d.items()}
来源：http://ovn.ppjwa.cn

[U08] Py：展平二维列表
来源：http://tes.cdnleiting.top

[y for x in nested for y in x]
来源：http://oqq.chenzaomai.com

[U09] Py：字典取最大值的键
来源：http://qtb.birdmap.top

max(d, key=d.get)
来源：http://tlu.nanxinkj.top

[U10] Py：按值排序字典
来源：http://hkb.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jjn.smart0.xyz

[U11] Py：生成器表达式
来源：http://gqu.316326.xyz

(x * 2 for x in arr)
来源：http://ufr.316326.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://oib.bbcook.cn

Counter(arr).most_common(3)
来源：http://npg.yangfankeji.com

[U13] Py：固定长度队列
来源：http://grl.xingfuxueyuan.xyz

deque(maxlen=10)
来源：http://wlq.hnxiangtu.top

[U14] Py：分组收集到列表
来源：http://yvs.chenlongwang.top

defaultdict(list)
来源：http://jzi.yueranfly.top

[U15] Py：高精度计时
来源：http://xlh.jqgfzy.top

t = time.perf_counter()
来源：http://pbg.hfpthk.cn

[U16] Py：命令行参数解析
来源：http://ymm.0kj1m.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gjp.zhiwuduotai.top

[U17] Py：初始化日志
来源：http://ecg.zdbjq.cn

logging.basicConfig(level=logging.INFO)
来源：http://wlr.bjfxy.top

[U18] Py：预编译正则
来源：http://mge.ctjpmb.com

pat = re.compile(r"\d+")
来源：http://nzn.ybcxt.top

[U19] Py：正则替换带回调
来源：http://zyx.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://irh.dashuyun.cn

[U20] Py：缓存函数结果
来源：http://hyo.fengsongda.top

@functools.lru_cache(maxsize=None)
来源：http://sek.sysykeji.top

[U21] Py：自定义上下文管理器
来源：http://boe.shuidangran.top

@contextlib.contextmanager
来源：http://gqf.316326.xyz

[U22] Py：矩阵转置
来源：http://cgz.yj20258888.top

list(zip(*m))
来源：http://zeq.shanyushiyangtech.top

[U23] Py：分块读取大文件
来源：http://voi.c1oappe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uno.fktsv.cn

[U24] Py：路径操作
来源：http://sqd.hnxiangtu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qzp.meibo888.top

[U25] Py：CSV 按字典读
来源：http://sec.uphjek.com

csv.DictReader(f)
来源：http://ecc.shangyingyoupin.top

[U26] Py：并发下载
来源：http://gtm.zhiwuduotai.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ofj.yj20258888.top

[U27] Py：异步 HTTP
来源：http://csj.fengsongda.top

aiohttp.ClientSession() 配合 async with
来源：http://udu.yonumen.top

[U28] Py：类型别名
来源：http://tnz.gotoacloud.top

UserId = int
来源：http://usv.zhixingplan.top

[U29] Py：属性校验
来源：http://kzj.jlsjyb.cn

@property 与 @x.setter 配合
来源：http://phn.0kj1m.cn

[U30] Py：数据类
来源：http://kwi.bjfxy.top

@dataclass(slots=True)
来源：http://ftp.cashguo.top

[U31] Py：单测
来源：http://gfq.cdnleiting.top

python -m pytest -q
来源：http://bly.daria6918.cn

[U32] Py：代码格式化
来源：http://lmt.zhaomingkeji.xyz

ruff format . && ruff check --fix .
来源：http://enh.hesvh.cn

[U33] Py：打包发布
来源：http://abw.ehwqpu.com

python -m build  （依赖 pyproject.toml）
来源：http://ush.chenlongwang.top

[U34] Py：判断编码
来源：http://vhj.gotoacloud.top

chardet.detect(raw)
来源：http://ppe.svipenyu.cn

[U35] Py：发送邮件
来源：http://uzg.zhoulong.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ktp.hysaishi.cn

[U36] Py：定时任务
来源：http://gyp.hesvh.cn

schedule.every(10).minutes.do(job)
来源：http://heg.ydzc1.top

[U37] Py：读写 Excel
来源：http://nfs.tian-w.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ndz.xuetiantiany.cn

[U38] Py：获取脚本所在目录
来源：http://qpa.feifeiyinyue.top

Path(__file__).resolve().parent
来源：http://ibk.zycfv.cn

[U39] Py：判断是否在交互环境
来源：http://xhz.yuxming.cn

sys.stdout.isatty()
来源：http://dbh.xziqi.cn

[U40] Py：打印到标准错误
来源：http://xab.xziqi.cn

print("err", file=sys.stderr)
来源：http://qyb.tian-w.cn

[U41] PHP：初始化 Composer 项目
来源：http://hed.gogol.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gyf.uphjek.com

[U42] PHP：PSR-4 自动加载
来源：http://hik.yueranfly.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mgf.shanyushiyangtech.top

[U43] PHP：声明命名空间
来源：http://wml.aizwys.cn

namespace App\Http;
来源：http://fko.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://bmv.jianghu66.top

declare(strict_types=1);
来源：http://riv.bbcook.cn

[U45] PHP：类型声明与返回类型
来源：http://snh.sxryk.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uxa.jianghu66.top

[U46] PHP：可空类型
来源：http://uwz.jinqigufen.top

?string $name = null
来源：http://edm.shuidangran.top

[U47] PHP：联合类型
来源：http://xrf.yj20258888.top

int|string $id
来源：http://euq.yj20258888.top

[U48] PHP：纯枚举
来源：http://dpq.zhengqikj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qaj.xuanzx.com

[U49] PHP：只读属性
来源：http://oel.zhixingplan.top

public readonly string $name
来源：http://bwx.nwbrower.top

[U50] PHP：构造器属性提升
来源：http://lzn.cheryme.top

public function __construct(private int $id) {}
来源：http://hzb.daria6918.cn

[U51] PHP：数组解构
来源：http://dou.0kj1m.cn

[$a, $b] = $arr;
来源：http://nwy.ybcxt.top

[U52] PHP：箭头函数
来源：http://cmc.zdbjq.cn

$double = fn($x) => $x * 2;
来源：http://nyh.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://vdd.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://jrn.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://xoc.52xcode.cn

$obj?->method()
来源：http://mrq.hywenlv.cn


<!-- 参考信息 -->