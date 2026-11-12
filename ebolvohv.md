代发 wailian999

#ifndef X_H
来源：http://baa.xingfuxueyuan.xyz

#define X_H
来源：http://lfa.nwbrower.top

#endif
来源：http://akm.jinyuanbaomall.cn

[S31] C++：Hello World
来源：http://mny.cqqwz.cn

#include <iostream>
来源：http://xyj.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://olf.zhixingplan.top

[S32] C++：字符串
来源：http://rtm.yueranfly.top

std::string s = "hi";  s += "!";
来源：http://bna.smart0.xyz

[S33] C++：vector 增删
来源：http://tya.yongpay.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hui.yongpay.top

[S34] C++：遍历 vector
来源：http://bqd.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://deq.shzxlz.cn

[S35] C++：map
来源：http://mty.kuanghao11.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://trt.tarul.cn

[S36] C++：unordered_map
来源：http://uta.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zti.xuanzx.com

[S37] C++：set
来源：http://bdw.zhiwuduotai.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vif.ehwqpu.com

[S38] C++：排序
来源：http://yho.zhongyouzk.top

std::sort(v.begin(), v.end());
来源：http://emq.jlsjyb.cn

[S39] C++：自定义比较器排序
来源：http://zoo.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wpw.iojbl.cn

[S40] C++：查找元素
来源：http://gmz.pycfn.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eom.9152youxi.cn

[S41] C++：类与构造函数
来源：http://egq.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ysl.cheryme.top

[S42] C++：继承与虚函数
来源：http://zrb.hnqzz.top

class B : public Base { public: void f() override {} };
来源：http://fit.epnwcf.com

[S43] C++：智能指针
来源：http://mif.hcnkem.com

auto p = std::make_unique<int>(5);
来源：http://ngi.fanxiaobao.xyz

[S44] C++：引用传参
来源：http://gcm.birdmap.top

void inc(int &x) { ++x; }
来源：http://xip.guowangkeji.top

[S45] C++：lambda
来源：http://wnr.jlsjyb.cn

auto add = [](int a, int b) { return a + b; };
来源：http://efl.yuanzhike.top

[S46] C++：函数模板
来源：http://yfd.kuanghao11.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cui.yangfankeji.com

[S47] C++：结构化绑定遍历
来源：http://twm.yvedp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://onx.xingfuxueyuan.xyz

[S48] C++：逐行读文件
来源：http://kxk.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qto.hongshengwenyu.top

while (std::getline(in, line)) { }
来源：http://tez.zhijiandao.cn

[S49] C++：写文件
来源：http://ttf.nanxuanxn.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pwx.pycfn.com

[S50] C++：格式化数字
来源：http://bwr.haohaochexian.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pga.fzhhl.top

[S51] C++：显式类型转换
来源：http://mzb.shuidangran.top

static_cast<double>(a) / b
来源：http://tem.dashuyun.cn

[S52] C++：const 与 noexcept
来源：http://bpr.ctjpmb.com

int size() const noexcept { return n_; }
来源：http://kst.fehbvm.com

[S53] C++：移动语义
来源：http://snj.haohaochexian.top

std::vector<int> w = std::move(v);
来源：http://jrv.havefunace.top

[S54] C++：异常处理
来源：http://bjt.zdqjudy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jau.hywenlv.cn

[S55] C++：结构化绑定
来源：http://wfw.jlsjyb.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://olo.sufxvd.cn

[S56] C++：optional
来源：http://uhc.nanxuanxn.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cox.svipenyu.cn

[S57] C++：编译期常量
来源：http://fvw.haohaochexian.top

constexpr int N = 10;
来源：http://gfu.wangdashe.top

[S58] C++：命名空间
来源：http://nhp.sysykeji.top

namespace ns { int f() { return 1; } }
来源：http://qlj.sjlbkw.cn

[S59] C++：静态断言
来源：http://jhb.pengpengdd.cyou

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aee.daria6918.cn

[S60] C++：遍历并删除元素
来源：http://hat.yj20258.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://orv.yangfankeji.com

================================================================================
来源：http://thn.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ysy.shzxlz.cn

================================================================================
来源：http://luf.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://pqi.xingfuxueyuan.xyz

println("Hello")
来源：http://tgd.uphjek.com

[T02] Kotlin：变量
来源：http://cvm.zhixingplan.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tta.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://lgu.epnwcf.com

"值: $b"
来源：http://rqh.yuxming.cn

[T04] Kotlin：空安全
来源：http://gzy.shanyushiyangtech.top

val n: String? = null;  n?.length
来源：http://san.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://pdc.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aat.tarul.cn

[T06] Kotlin：集合映射
来源：http://kgj.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rqk.aibaodan.cn

[T07] Kotlin：集合过滤
来源：http://psd.chenlongwang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://epn.hfpthk.cn

[T08] Kotlin：数据类
来源：http://bvh.jqgfzy.top

data class User(val name: String, val age: Int)
来源：http://hyf.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://puo.hnxiangtu.top

fun String.exclaim() = this + "!"
来源：http://gqa.sysykeji.top

[T10] Kotlin：默认参数
来源：http://ohi.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://sfe.zhijiandao.cn

[T11] Kotlin：协程
来源：http://xfl.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nft.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://nxu.yueranfly.top

val (a, b) = Pair(1, 2)
来源：http://adc.nanxuanxn.top

[T13] Kotlin：只读 Map
来源：http://afi.yj20258888.top

val m = mapOf("a" to 1)
来源：http://wyk.hysaishi.cn

[T14] Kotlin：循环
来源：http://pjj.yongpay.top

for (i in 1..10) println(i)
来源：http://wwf.hysaishi.cn

[T15] Kotlin：接口
来源：http://bfw.ydzc1.top

interface Shape { fun area(): Double }
来源：http://ooq.fehbvm.com

[T16] Swift：Hello World
来源：http://koa.chenlongwang.top

print("Hello")
来源：http://zvl.daxiang520.top

[T17] Swift：变量与常量
来源：http://iti.xuetiantiany.cn

var a = 1;  let b = 2
来源：http://guv.zhixingplan.top

[T18] Swift：字符串插值
来源：http://exe.ehwqpu.com

"值: \(b)"
来源：http://uuo.xingfuxueyuan.xyz

[T19] Swift：可选绑定
来源：http://nkw.sysykeji.top

if let n = opt { print(n) }
来源：http://zln.jinqigfzy.top

[T20] Swift：数组操作
来源：http://hqu.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://ebb.nwbrower.top

[T21] Swift：遍历
来源：http://kwc.havefunace.top

for x in a { print(x) }
来源：http://onl.9152youxi.cn

[T22] Swift：字典
来源：http://snv.jiagoushi.top

var d = ["a": 1];  d["b"] = 2
来源：http://qtl.sxryk.cn

[T23] Swift：函数
来源：http://zno.tian-w.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rlf.tanke756.top

[T24] Swift：闭包
来源：http://ptr.gogol.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hih.hnqzz.top

[T25] Swift：结构体
来源：http://qqz.ydzc1.top

struct P { var x: Int }
来源：http://qja.wangshuangyany.cn

[T26] Swift：类与重写
来源：http://ljv.guowangkeji.top

class A: Base { override func f() {} }
来源：http://aid.c1oappe.top

[T27] Swift：错误处理
来源：http://cqc.gogol.net.cn

do { try f() } catch { print(error) }
来源：http://ysg.fengsongda.top

[T28] Swift：枚举
来源：http://ipg.jqgfzy.top

enum Color { case red, green }
来源：http://uux.cashguo.top

[T29] Swift：guard 提前返回
来源：http://jfp.jlsjyb.cn

guard let x = opt else { return }
来源：http://rid.ivvv.top

[T30] Swift：协议
来源：http://asl.pengpengdd.cyou

protocol Shape { func area() -> Double }
来源：http://ypi.zycfv.cn

[T31] Lua：Hello World
来源：http://nlj.jinqigufen.top

print("Hello")
来源：http://ttb.kuanghao11.cn

[T32] Lua：局部变量
来源：http://sxd.yueranfly.top

local a = 1
来源：http://zqc.hfpthk.cn

[T33] Lua：表（数组）
来源：http://rzo.hesvh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lwy.sufxvd.cn

[T34] Lua：遍历表
来源：http://ktw.ywan-chungtsiang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ntu.c1oappe.top

[T35] Lua：字典表
来源：http://cty.nwbrower.top

local d = { a = 1 };  d.b = 2
来源：http://yej.sysykeji.top

[T36] Lua：函数
来源：http://nlj.tian-w.cn

function add(a, b) return a + b end
来源：http://umu.sufxvd.cn

[T37] Lua：字符串拼接
来源：http://oer.aizwys.cn

"a" .. "b"
来源：http://izv.ywan-chungtsiang.top

[T38] Lua：条件
来源：http://gmn.gaohongyu789.top

if x > 0 then print("正") end
来源：http://qfx.svipenyu.cn

[T39] Lua：模式匹配
来源：http://zro.jinqigufen.top

string.find(s, "%d+")
来源：http://zzo.yuxming.cn

[T40] Lua：元表
来源：http://pij.yvedp.cn

setmetatable({}, { __index = base })
来源：http://vid.fengsongda.top

[T41] Perl：Hello World
来源：http://qjg.zycfv.cn

print "Hello\n";
来源：http://dcw.smart0.xyz

[T42] Perl：变量类型
来源：http://zrk.ywan-chungtsiang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gii.guowangkeji.top

[T43] Perl：字符串插值
来源：http://dbe.jlsjyb.cn

"值: $a"
来源：http://oxu.fktsv.cn

[T44] Perl：条件
来源：http://ezg.sweek.top

if ($a > 0) { print "正"; }
来源：http://htc.meibo888.top

[T45] Perl：数组遍历
来源：http://csn.cqqwz.cn

for my $x (@arr) { print $x; }
来源：http://hwb.fengsongda.top

[T46] Perl：哈希操作
来源：http://hjk.vqdsnc.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://awx.guowangkeji.top

[T47] Perl：正则捕获
来源：http://bdy.c1oappe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://djc.ybcxt.top

[T48] Perl：正则替换
来源：http://hsp.tanke756.top

$s =~ s/old/new/g;
来源：http://ptc.hnxiangtu.top

[T49] Perl：函数
来源：http://btl.chenjidiqi.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ujb.uphjek.com

[T50] Perl：逐行读文件
来源：http://ewi.jqgfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wsh.guannengcc.top

while (my $line = <$fh>) { print $line; }
来源：http://jzj.sufxvd.cn

[T51] Scala：Hello World
来源：http://svt.fehbvm.com

println("Hello")
来源：http://htp.nanxuanxn.top

[T52] Scala：变量
来源：http://gyy.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://bac.daxiang520.top

[T53] Scala：字符串插值
来源：http://kcv.svipenyu.cn

s"值: $b"
来源：http://ypi.yfazqb.com

[T54] Scala：集合映射
来源：http://sza.yfazqb.com

List(1, 2, 3).map(_ * 2)
来源：http://ckh.jinghuilouyu.cn

[T55] Scala：集合过滤
来源：http://rjs.hfpthk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pvn.jyoumei.cn

[T56] Scala：样例类
来源：http://hyj.chenlongwang.top

case class User(name: String, age: Int)
来源：http://uxg.tanke756.top

[T57] Scala：模式匹配
来源：http://cgg.hcnkem.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://vlv.redwolf501.top

[T58] Scala：函数定义
来源：http://yms.daxiang520.top

def add(a: Int, b: Int): Int = a + b
来源：http://tft.zhixingplan.top

[T59] Scala：循环
来源：http://piz.hammf.cn

for (i <- 1 to 10) println(i)
来源：http://kcu.gotoacloud.top

[T60] Scala：折叠
来源：http://dty.sxryk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fan.xingfuxueyuan.xyz

================================================================================
来源：http://ffo.52xcode.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kky.tarul.cn

================================================================================
来源：http://xlx.shuidangran.top

[U01] Py：创建虚拟环境
来源：http://djp.zhaomingkeji.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://pzw.tarul.cn

[U02] Py：导出 / 安装依赖
来源：http://pwg.chenjidiqi.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kfq.ehwqpu.com

[U03] Py：加载 .env 配置
来源：http://ufw.zycfv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fcy.shangyingyoupin.top

[U04] Py：变量调试打印
来源：http://wnb.tianlin.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lnt.andypj.xyz

[U05] Py：列表去重且保序
来源：http://chl.uphjek.com

list(dict.fromkeys(arr))
来源：http://dla.svipenyu.cn

[U06] Py：合并两个字典
来源：http://rjh.jianghu66.top

{**a, **b}
来源：http://mpx.guannengcc.top

[U07] Py：反转字典键值
来源：http://ymf.cashguo.top

{v: k for k, v in d.items()}
来源：http://bgv.sufxvd.cn

[U08] Py：展平二维列表
来源：http://ywm.gogol.net.cn

[y for x in nested for y in x]
来源：http://lld.kuanghao11.cn

[U09] Py：字典取最大值的键
来源：http://zcr.cashguo.top

max(d, key=d.get)
来源：http://xim.aizwys.cn

[U10] Py：按值排序字典
来源：http://uyf.xziqi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hrk.dashuyun.cn

[U11] Py：生成器表达式
来源：http://dno.feifeiyinyue.top

(x * 2 for x in arr)
来源：http://wiv.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://bqc.tanke756.top

Counter(arr).most_common(3)
来源：http://ztt.daxiang520.top

[U13] Py：固定长度队列
来源：http://pla.yongpay.top

deque(maxlen=10)
来源：http://ikf.smart0.xyz

[U14] Py：分组收集到列表
来源：http://gin.aizwys.cn

defaultdict(list)
来源：http://dch.xylfe.cn

[U15] Py：高精度计时
来源：http://rju.zhixingplan.top

t = time.perf_counter()
来源：http://nhj.redwolf501.top

[U16] Py：命令行参数解析
来源：http://aup.yanxiufei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yll.nwbrower.top

[U17] Py：初始化日志
来源：http://huk.gzhubu.top

logging.basicConfig(level=logging.INFO)
来源：http://snj.jianghu66.top

[U18] Py：预编译正则
来源：http://lcu.ehwqpu.com

pat = re.compile(r"\d+")
来源：http://rhv.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://cin.feifeiyinyue.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://inp.pengpengdd.cyou

[U20] Py：缓存函数结果
来源：http://esc.shangyingyoupin.top

@functools.lru_cache(maxsize=None)
来源：http://kym.ppjwa.cn

[U21] Py：自定义上下文管理器
来源：http://dtk.fehbvm.com

@contextlib.contextmanager
来源：http://ffn.ehwqpu.com

[U22] Py：矩阵转置
来源：http://zrw.xylfe.cn

list(zip(*m))
来源：http://uce.shanyushiyangkeji.top

[U23] Py：分块读取大文件
来源：http://idd.jinqigufen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xdl.tarul.cn

[U24] Py：路径操作
来源：http://ijt.hongshengwenyu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cis.daria6918.cn

[U25] Py：CSV 按字典读
来源：http://egz.chenzaomai.com

csv.DictReader(f)
来源：http://umf.ivvv.top

[U26] Py：并发下载
来源：http://fhh.jinghuilouyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://por.nwbrower.top

[U27] Py：异步 HTTP
来源：http://uzd.zhixingplan.top

aiohttp.ClientSession() 配合 async with
来源：http://jsz.jlsjyb.cn

[U28] Py：类型别名
来源：http://moy.gogol.net.cn

UserId = int
来源：http://tvb.vehdjk.com

[U29] Py：属性校验
来源：http://spm.shangyingyoupin.top

@property 与 @x.setter 配合
来源：http://zvg.wangdashe.top

[U30] Py：数据类
来源：http://awx.zhoulong.xyz

@dataclass(slots=True)
来源：http://wkt.feifeiyinyue.top

[U31] Py：单测
来源：http://bkq.ybcxt.top

python -m pytest -q
来源：http://jeh.shangyingyoupin.top

[U32] Py：代码格式化
来源：http://iie.hesvh.cn

ruff format . && ruff check --fix .
来源：http://nqc.ehwqpu.com

[U33] Py：打包发布
来源：http://jhc.yfazqb.com

python -m build  （依赖 pyproject.toml）
来源：http://tad.ybcxt.top

[U34] Py：判断编码
来源：http://jwx.snrcjt.cn

chardet.detect(raw)
来源：http://tes.zdqjudy.top

[U35] Py：发送邮件
来源：http://pno.yj20258888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vwx.bjfxy.top

[U36] Py：定时任务
来源：http://tty.snrcjt.cn

schedule.every(10).minutes.do(job)
来源：http://bqz.bbcook.cn

[U37] Py：读写 Excel
来源：http://kqk.yj20258.top

pandas.read_excel / DataFrame.to_excel
来源：http://ucl.yj202588.top

[U38] Py：获取脚本所在目录
来源：http://ghs.cqqwz.cn

Path(__file__).resolve().parent
来源：http://iiw.zycfv.cn

[U39] Py：判断是否在交互环境
来源：http://bpb.chenzaomai.com

sys.stdout.isatty()
来源：http://hlv.fzhhl.top

[U40] Py：打印到标准错误
来源：http://qjf.yongpay.top

print("err", file=sys.stderr)
来源：http://wmd.yuxming.cn

[U41] PHP：初始化 Composer 项目
来源：http://fnj.ybcxt.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rbs.fengsongda.top

[U42] PHP：PSR-4 自动加载
来源：http://ynu.9152youxi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sjn.jianghu66.top

[U43] PHP：声明命名空间
来源：http://ywg.fktsv.cn

namespace App\Http;
来源：http://jhx.wangdashe.top

[U44] PHP：开启严格类型
来源：http://vzd.nanxuanxn.top

declare(strict_types=1);
来源：http://oer.fehbvm.com

[U45] PHP：类型声明与返回类型
来源：http://pik.fanxiaobao.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://ijd.xylfe.cn

[U46] PHP：可空类型
来源：http://qmh.tian-w.cn

?string $name = null
来源：http://bmi.hammf.cn

[U47] PHP：联合类型
来源：http://jir.316326.xyz

int|string $id
来源：http://zhj.ydjk.org.cn

[U48] PHP：纯枚举
来源：http://mmf.cucudq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uer.yongpay.top

[U49] PHP：只读属性
来源：http://dgr.52xcode.cn

public readonly string $name
来源：http://qle.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://ftt.zhongyouzk.top

public function __construct(private int $id) {}
来源：http://jky.uphjek.com

[U51] PHP：数组解构
来源：http://kis.cashguo.top

[$a, $b] = $arr;
来源：http://dyu.gogol.net.cn

[U52] PHP：箭头函数
来源：http://sqp.ppjwa.cn

$double = fn($x) => $x * 2;
来源：http://ehi.zdqjudy.top

[U53] PHP：空合并运算符
来源：http://mvn.gogol.net.cn

$v = $a ?? $b ?? "default";
来源：http://rbg.nwbrower.top

[U54] PHP：空安全调用
来源：http://znz.wangdashe.top

$obj?->method()
来源：http://met.shangyingyoupin.top


<!-- 参考信息 -->