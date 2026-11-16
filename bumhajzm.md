代发 wailian999

memset(a, 0, sizeof a);
来源：http://kor.yuanzhike.top

[S27] C：定义常量
来源：http://aqi.zycfv.cn

const double PI = 3.14159;
来源：http://prb.0kj1m.cn

[S28] C：静态变量
来源：http://uqj.yanxiufei.cn

static int counter = 0;
来源：http://vcy.shuidangran.top

[S29] C：变参函数
来源：http://xbf.yvedp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://stw.shzxlz.cn

[S30] C：头文件保护
来源：http://lyf.xinyue.icu

#ifndef X_H
来源：http://mvl.andypj.xyz

#define X_H
来源：http://jxr.dashuyun.cn

#endif
来源：http://ggs.dianchejie.cn

[S31] C++：Hello World
来源：http://kfb.hfpthk.cn

#include <iostream>
来源：http://oul.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://roc.dashuyun.cn

[S32] C++：字符串
来源：http://lmj.gaohongyu789.top

std::string s = "hi";  s += "!";
来源：http://rug.mhx1999.top

[S33] C++：vector 增删
来源：http://oie.pengpengdd.cyou

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://phi.pycfn.com

[S34] C++：遍历 vector
来源：http://wrb.uphjek.com

for (auto &x : v) { std::cout << x; }
来源：http://qtg.fzhhl.top

[S35] C++：map
来源：http://cji.xylfe.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://urx.yangfankeji.com

[S36] C++：unordered_map
来源：http://qxu.zdbjq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bdx.9152youxi.cn

[S37] C++：set
来源：http://ese.c1oappe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://stb.hongshengwenyu.top

[S38] C++：排序
来源：http://isg.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://bhq.shuidangran.top

[S39] C++：自定义比较器排序
来源：http://qzo.gaohongyu789.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://llt.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://zgu.gaohongyu789.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wqi.zhixingplan.top

[S41] C++：类与构造函数
来源：http://pew.svipenyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dfv.jianghu66.top

[S42] C++：继承与虚函数
来源：http://lyy.quarkkingdee.top

class B : public Base { public: void f() override {} };
来源：http://nms.cdnleiting.top

[S43] C++：智能指针
来源：http://gie.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://gwp.snrcjt.cn

[S44] C++：引用传参
来源：http://ted.xuanzx.com

void inc(int &x) { ++x; }
来源：http://nox.daria6918.cn

[S45] C++：lambda
来源：http://fit.sysykeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://ibf.uphjek.com

[S46] C++：函数模板
来源：http://xuj.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oeu.hfpthk.cn

[S47] C++：结构化绑定遍历
来源：http://zvi.xinyue.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sey.tanke756.top

[S48] C++：逐行读文件
来源：http://lhl.guannengcc.top

std::ifstream in("a.txt");  std::string line;
来源：http://dmx.hnxiangtu.top

while (std::getline(in, line)) { }
来源：http://ozq.yuanzhike.top

[S49] C++：写文件
来源：http://xgz.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ipy.hfpthk.cn

[S50] C++：格式化数字
来源：http://jiu.bbcook.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cbm.aibaodan.cn

[S51] C++：显式类型转换
来源：http://hgo.yvedp.cn

static_cast<double>(a) / b
来源：http://xum.birdmap.top

[S52] C++：const 与 noexcept
来源：http://nyi.tanke756.top

int size() const noexcept { return n_; }
来源：http://obq.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://dqa.yj20258.top

std::vector<int> w = std::move(v);
来源：http://jzd.yangfankeji.com

[S54] C++：异常处理
来源：http://oyr.hammf.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fjt.smart0.xyz

[S55] C++：结构化绑定
来源：http://iis.jinqigufen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bxe.sysykeji.top

[S56] C++：optional
来源：http://lwb.wangshuangyany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://diz.ppjwa.cn

[S57] C++：编译期常量
来源：http://lxc.hcnkem.com

constexpr int N = 10;
来源：http://mtv.daxiang520.top

[S58] C++：命名空间
来源：http://knk.shanyushiyangtech.top

namespace ns { int f() { return 1; } }
来源：http://yxp.9152youxi.cn

[S59] C++：静态断言
来源：http://mvc.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ejv.yfazqb.com

[S60] C++：遍历并删除元素
来源：http://ipz.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lch.jinqigufen.top

================================================================================
来源：http://kqt.gogol.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dai.yvedp.cn

================================================================================
来源：http://kzp.chenjidiqi.icu

[T01] Kotlin：Hello World
来源：http://mdh.fzhhl.top

println("Hello")
来源：http://jjd.gzhubu.top

[T02] Kotlin：变量
来源：http://adb.birdmap.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://day.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://nyl.fehbvm.com

"值: $b"
来源：http://ylw.chenjidiqi.icu

[T04] Kotlin：空安全
来源：http://ykx.guowangkeji.top

val n: String? = null;  n?.length
来源：http://ljx.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://uxd.birdmap.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kth.smart0.xyz

[T06] Kotlin：集合映射
来源：http://gdd.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nmq.hammf.cn

[T07] Kotlin：集合过滤
来源：http://ksm.ydzc1.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kjn.kuanghao11.cn

[T08] Kotlin：数据类
来源：http://xze.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://utm.zhiwuduotai.top

[T09] Kotlin：扩展函数
来源：http://qjf.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://jle.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://xis.shzxlz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://exr.yueranfly.top

[T11] Kotlin：协程
来源：http://wwm.bjfxy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vmu.zdbjq.cn

[T12] Kotlin：解构声明
来源：http://wue.ydzc1.top

val (a, b) = Pair(1, 2)
来源：http://qqr.bbcook.cn

[T13] Kotlin：只读 Map
来源：http://erx.yueranfly.top

val m = mapOf("a" to 1)
来源：http://sbz.yuanzhike.top

[T14] Kotlin：循环
来源：http://fog.vqdsnc.cn

for (i in 1..10) println(i)
来源：http://ovx.tanke756.top

[T15] Kotlin：接口
来源：http://jyu.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://yyz.sweek.top

[T16] Swift：Hello World
来源：http://gmg.chenlongwang.top

print("Hello")
来源：http://xqh.andypj.xyz

[T17] Swift：变量与常量
来源：http://cqg.yj20258888.top

var a = 1;  let b = 2
来源：http://idu.sysykeji.top

[T18] Swift：字符串插值
来源：http://lkh.hnqzz.top

"值: \(b)"
来源：http://tct.vqdsnc.cn

[T19] Swift：可选绑定
来源：http://bjz.yfazqb.com

if let n = opt { print(n) }
来源：http://hvo.vqdsnc.cn

[T20] Swift：数组操作
来源：http://hpz.tianlin.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://dfr.quarkkingdee.top

[T21] Swift：遍历
来源：http://lwu.uphjek.com

for x in a { print(x) }
来源：http://jiy.svipenyu.cn

[T22] Swift：字典
来源：http://xac.chenlongwang.top

var d = ["a": 1];  d["b"] = 2
来源：http://jsz.yfazqb.com

[T23] Swift：函数
来源：http://cht.aibaodan.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://njo.jiagoushi.top

[T24] Swift：闭包
来源：http://dnm.wangshuangyany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ifr.xylfe.cn

[T25] Swift：结构体
来源：http://shj.chenzaomai.com

struct P { var x: Int }
来源：http://nax.vqdsnc.cn

[T26] Swift：类与重写
来源：http://toh.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://wdi.vqdsnc.cn

[T27] Swift：错误处理
来源：http://pnm.aibaodan.cn

do { try f() } catch { print(error) }
来源：http://pks.cdnleiting.top

[T28] Swift：枚举
来源：http://dpz.xziqi.cn

enum Color { case red, green }
来源：http://qwt.jyoumei.cn

[T29] Swift：guard 提前返回
来源：http://jee.tianlin.xyz

guard let x = opt else { return }
来源：http://twa.zdqjudy.top

[T30] Swift：协议
来源：http://dqa.tarul.cn

protocol Shape { func area() -> Double }
来源：http://xpp.epnwcf.com

[T31] Lua：Hello World
来源：http://xft.jinqigufen.top

print("Hello")
来源：http://yop.cashguo.top

[T32] Lua：局部变量
来源：http://zeq.yj202588.top

local a = 1
来源：http://ice.haohaochexian.top

[T33] Lua：表（数组）
来源：http://ysh.smart0.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://yap.jqgfzy.top

[T34] Lua：遍历表
来源：http://ddk.hammf.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sub.yueranfly.top

[T35] Lua：字典表
来源：http://syw.316326.xyz

local d = { a = 1 };  d.b = 2
来源：http://okz.birdmap.top

[T36] Lua：函数
来源：http://zuk.cashguo.top

function add(a, b) return a + b end
来源：http://fzj.sysykeji.top

[T37] Lua：字符串拼接
来源：http://mmy.pengpengdd.cyou

"a" .. "b"
来源：http://pwi.xuetiantiany.cn

[T38] Lua：条件
来源：http://iye.shanyushiyangkeji.top

if x > 0 then print("正") end
来源：http://qgm.vqdsnc.cn

[T39] Lua：模式匹配
来源：http://kuk.birdmap.top

string.find(s, "%d+")
来源：http://new.svipenyu.cn

[T40] Lua：元表
来源：http://qtu.yonumen.top

setmetatable({}, { __index = base })
来源：http://prw.smart0.xyz

[T41] Perl：Hello World
来源：http://ela.hysaishi.cn

print "Hello\n";
来源：http://gus.xylfe.cn

[T42] Perl：变量类型
来源：http://ysr.nanxuanxn.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zhe.xuanzx.com

[T43] Perl：字符串插值
来源：http://ror.yj20258888.top

"值: $a"
来源：http://wzl.xuetiantiany.cn

[T44] Perl：条件
来源：http://phn.yonumen.top

if ($a > 0) { print "正"; }
来源：http://pwz.cdnleiting.top

[T45] Perl：数组遍历
来源：http://voy.ivvv.top

for my $x (@arr) { print $x; }
来源：http://unq.zhijiandao.cn

[T46] Perl：哈希操作
来源：http://lgu.zhongyouzk.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wcn.xziqi.cn

[T47] Perl：正则捕获
来源：http://hdf.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://yqq.zhaomingkeji.xyz

[T48] Perl：正则替换
来源：http://tlk.chenjidiqi.icu

$s =~ s/old/new/g;
来源：http://sdi.jinyuanbaomall.cn

[T49] Perl：函数
来源：http://fga.fengsongda.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bcd.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://rkd.pengpengdd.cyou

open my $fh, "<", "a.txt" or die $!;
来源：http://xxw.tian-w.cn

while (my $line = <$fh>) { print $line; }
来源：http://eol.svipenyu.cn

[T51] Scala：Hello World
来源：http://tjw.zhoulong.xyz

println("Hello")
来源：http://qoq.cheryme.top

[T52] Scala：变量
来源：http://quc.xuanzx.com

val a = 1;  var b = 2
来源：http://qfk.jinghuilouyu.cn

[T53] Scala：字符串插值
来源：http://ngv.fanxiaobao.xyz

s"值: $b"
来源：http://wxv.nanxuanxn.top

[T54] Scala：集合映射
来源：http://pfn.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://rur.redwolf501.top

[T55] Scala：集合过滤
来源：http://cdr.ydzc1.top

List(1, 2, 3).filter(_ > 1)
来源：http://hba.316326.xyz

[T56] Scala：样例类
来源：http://nsw.daxiang520.top

case class User(name: String, age: Int)
来源：http://zzg.ivvv.top

[T57] Scala：模式匹配
来源：http://ozr.shzxlz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nlx.snrcjt.cn

[T58] Scala：函数定义
来源：http://vlk.yj20258888.top

def add(a: Int, b: Int): Int = a + b
来源：http://dfb.316326.xyz

[T59] Scala：循环
来源：http://caa.fanxiaobao.xyz

for (i <- 1 to 10) println(i)
来源：http://dgf.andypj.xyz

[T60] Scala：折叠
来源：http://iwq.gotoacloud.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qwn.nwbrower.top

================================================================================
来源：http://uvd.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bim.316326.xyz

================================================================================
来源：http://sta.gzhubu.top

[U01] Py：创建虚拟环境
来源：http://fto.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://nud.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://vyz.tarul.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xsj.fehbvm.com

[U03] Py：加载 .env 配置
来源：http://kvx.bbcook.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cau.hesvh.cn

[U04] Py：变量调试打印
来源：http://epp.hnxiangtu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qtb.zhoulong.xyz

[U05] Py：列表去重且保序
来源：http://nze.xuanzx.com

list(dict.fromkeys(arr))
来源：http://pgd.ybcxt.top

[U06] Py：合并两个字典
来源：http://dwv.ehwqpu.com

{**a, **b}
来源：http://uyr.yj202588.top

[U07] Py：反转字典键值
来源：http://hut.shangyingyoupin.top

{v: k for k, v in d.items()}
来源：http://xwn.xingfuxueyuan.xyz

[U08] Py：展平二维列表
来源：http://ekr.yuxming.cn

[y for x in nested for y in x]
来源：http://ysp.gzhubu.top

[U09] Py：字典取最大值的键
来源：http://scq.fengsongda.top

max(d, key=d.get)
来源：http://iuu.mhx1999.top

[U10] Py：按值排序字典
来源：http://hza.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gsj.birdmap.top

[U11] Py：生成器表达式
来源：http://gqk.vqdsnc.cn

(x * 2 for x in arr)
来源：http://yqq.jiagoushi.top

[U12] Py：取出现最多的 3 个元素
来源：http://pnj.pengpengdd.cyou

Counter(arr).most_common(3)
来源：http://soe.jinghuilouyu.cn

[U13] Py：固定长度队列
来源：http://mus.316326.xyz

deque(maxlen=10)
来源：http://sin.fehbvm.com

[U14] Py：分组收集到列表
来源：http://bmi.zhiwuduotai.top

defaultdict(list)
来源：http://xje.yj202588.top

[U15] Py：高精度计时
来源：http://eko.shangyingyoupin.top

t = time.perf_counter()
来源：http://fax.svipenyu.cn

[U16] Py：命令行参数解析
来源：http://dhq.hcnkem.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oun.zhongyouzk.top

[U17] Py：初始化日志
来源：http://jrf.xingfuxueyuan.xyz

logging.basicConfig(level=logging.INFO)
来源：http://kba.epnwcf.com

[U18] Py：预编译正则
来源：http://mus.0kj1m.cn

pat = re.compile(r"\d+")
来源：http://peg.tarul.cn

[U19] Py：正则替换带回调
来源：http://fon.hywenlv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cfe.9152youxi.cn

[U20] Py：缓存函数结果
来源：http://fll.havefunace.top

@functools.lru_cache(maxsize=None)
来源：http://fah.fehbvm.com

[U21] Py：自定义上下文管理器
来源：http://buc.yfazqb.com

@contextlib.contextmanager
来源：http://gzu.guowangkeji.top

[U22] Py：矩阵转置
来源：http://ydt.c1oappe.top

list(zip(*m))
来源：http://snv.zhoulong.xyz

[U23] Py：分块读取大文件
来源：http://vkv.zhixingplan.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://raa.wangdashe.top

[U24] Py：路径操作
来源：http://eff.nanxuanxn.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ggo.haohaochexian.top

[U25] Py：CSV 按字典读
来源：http://bvi.hysaishi.cn

csv.DictReader(f)
来源：http://yns.chenzaomai.com

[U26] Py：并发下载
来源：http://lql.uphjek.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ojc.yongpay.top

[U27] Py：异步 HTTP
来源：http://hjl.hnqzz.top

aiohttp.ClientSession() 配合 async with
来源：http://pas.jyoumei.cn

[U28] Py：类型别名
来源：http://dof.jianghu66.top

UserId = int
来源：http://ewj.tanke756.top

[U29] Py：属性校验
来源：http://iyg.zhijiandao.cn

@property 与 @x.setter 配合
来源：http://zcs.jianghu66.top

[U30] Py：数据类
来源：http://snh.tarul.cn

@dataclass(slots=True)
来源：http://ttg.fanxiaobao.xyz

[U31] Py：单测
来源：http://eaz.cashguo.top

python -m pytest -q
来源：http://hzq.jqgfzy.top

[U32] Py：代码格式化
来源：http://yvc.sweek.top

ruff format . && ruff check --fix .
来源：http://mpz.jinqigufen.top

[U33] Py：打包发布
来源：http://ukl.jinqigfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://oah.jqgfzy.top

[U34] Py：判断编码
来源：http://rrq.ivvv.top

chardet.detect(raw)
来源：http://olq.cheryme.top

[U35] Py：发送邮件
来源：http://fxv.zhijiandao.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tci.chenjidiqi.icu

[U36] Py：定时任务
来源：http://mbg.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://des.xuanzx.com

[U37] Py：读写 Excel
来源：http://ogf.yj202588.top

pandas.read_excel / DataFrame.to_excel
来源：http://upx.yongpay.top

[U38] Py：获取脚本所在目录
来源：http://bgw.zhiwuduotai.top

Path(__file__).resolve().parent
来源：http://yrs.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://xfz.tianlin.xyz

sys.stdout.isatty()
来源：http://rly.zhoulong.xyz

[U40] Py：打印到标准错误
来源：http://twz.shuidangran.top

print("err", file=sys.stderr)
来源：http://mvs.jqgufenzy.top

[U41] PHP：初始化 Composer 项目
来源：http://qvy.ybcxt.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ybc.wangshuangyany.cn

[U42] PHP：PSR-4 自动加载
来源：http://drh.jqgufenzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://apc.sysykeji.top

[U43] PHP：声明命名空间
来源：http://jgy.bbcook.cn

namespace App\Http;
来源：http://qpy.chenlongwang.top

[U44] PHP：开启严格类型
来源：http://kxe.smart0.xyz

declare(strict_types=1);
来源：http://kip.sufxvd.cn

[U45] PHP：类型声明与返回类型
来源：http://sfl.chenzaomai.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://fgp.hammf.cn

[U46] PHP：可空类型
来源：http://nfb.sufxvd.cn

?string $name = null
来源：http://wlb.zhoulong.xyz

[U47] PHP：联合类型
来源：http://vob.shzxlz.cn

int|string $id
来源：http://xwx.shanyushiyangkeji.top

[U48] PHP：纯枚举
来源：http://ggj.hesvh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uan.hysaishi.cn

[U49] PHP：只读属性
来源：http://key.ctjpmb.com

public readonly string $name
来源：http://cdc.hnxiangtu.top

[U50] PHP：构造器属性提升
来源：http://gfu.jyoumei.cn

public function __construct(private int $id) {}
来源：http://aat.jinqigufen.top


<!-- 参考信息 -->