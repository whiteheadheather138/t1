代发 wailian999

static int counter = 0;
来源：http://haa.ivvv.top

[S29] C：变参函数
来源：http://gnp.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gbh.quarkkingdee.top

[S30] C：头文件保护
来源：http://blj.gotoacloud.top

#ifndef X_H
来源：http://siz.jqgfzy.top

#define X_H
来源：http://ahy.yangfankeji.com

#endif
来源：http://ocr.xinyue.icu

[S31] C++：Hello World
来源：http://qpe.xuetiantiany.cn

#include <iostream>
来源：http://zzc.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://gus.hammf.cn

[S32] C++：字符串
来源：http://eia.xingfuxueyuan.xyz

std::string s = "hi";  s += "!";
来源：http://cjn.xingfuxueyuan.xyz

[S33] C++：vector 增删
来源：http://fto.jyoumei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ksl.shzxlz.cn

[S34] C++：遍历 vector
来源：http://wff.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://avw.xylfe.cn

[S35] C++：map
来源：http://wyp.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xrp.epnwcf.com

[S36] C++：unordered_map
来源：http://ssn.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iau.bbcook.cn

[S37] C++：set
来源：http://tcv.dianchejie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lkh.nwbrower.top

[S38] C++：排序
来源：http://nhf.dianchejie.cn

std::sort(v.begin(), v.end());
来源：http://pni.gogol.net.cn

[S39] C++：自定义比较器排序
来源：http://mvw.yuanzhike.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tce.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://mly.0kj1m.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eyl.hysaishi.cn

[S41] C++：类与构造函数
来源：http://eed.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cmy.dianchejie.cn

[S42] C++：继承与虚函数
来源：http://nbj.yj20258888.top

class B : public Base { public: void f() override {} };
来源：http://cgy.ydjk.org.cn

[S43] C++：智能指针
来源：http://bgy.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://xkk.zycfv.cn

[S44] C++：引用传参
来源：http://zhb.smart0.xyz

void inc(int &x) { ++x; }
来源：http://cja.gaohongyu789.top

[S45] C++：lambda
来源：http://sel.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://yqp.tian-w.cn

[S46] C++：函数模板
来源：http://ulo.shangyingyoupin.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ndc.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://pnk.nanxinkj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tjc.shuidangran.top

[S48] C++：逐行读文件
来源：http://ztc.yonumen.top

std::ifstream in("a.txt");  std::string line;
来源：http://wcv.zhengqikj.top

while (std::getline(in, line)) { }
来源：http://pid.yfazqb.com

[S49] C++：写文件
来源：http://piu.ybcxt.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qhf.jiagoushi.top

[S50] C++：格式化数字
来源：http://qyk.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ijj.guowangkeji.top

[S51] C++：显式类型转换
来源：http://bjn.meibo888.top

static_cast<double>(a) / b
来源：http://cxz.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://edb.xuanzx.com

int size() const noexcept { return n_; }
来源：http://uao.daria6918.cn

[S53] C++：移动语义
来源：http://qvj.uphjek.com

std::vector<int> w = std::move(v);
来源：http://zoi.pengpengdd.cyou

[S54] C++：异常处理
来源：http://tfs.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hau.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://tmq.yvedp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fuu.uphjek.com

[S56] C++：optional
来源：http://dpq.shangyingyoupin.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jcu.zhixingplan.top

[S57] C++：编译期常量
来源：http://zxn.tianlin.xyz

constexpr int N = 10;
来源：http://aod.smart0.xyz

[S58] C++：命名空间
来源：http://owc.uphjek.com

namespace ns { int f() { return 1; } }
来源：http://zvy.vehdjk.com

[S59] C++：静态断言
来源：http://rlw.jyoumei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mnr.ywan-chungtsiang.top

[S60] C++：遍历并删除元素
来源：http://iou.vqdsnc.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kdz.chenlongwang.top

================================================================================
来源：http://scv.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ysv.ctjpmb.com

================================================================================
来源：http://swf.zhiwuduotai.top

[T01] Kotlin：Hello World
来源：http://fba.zhixingplan.top

println("Hello")
来源：http://coh.zdbjq.cn

[T02] Kotlin：变量
来源：http://gkx.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jki.zhixingplan.top

[T03] Kotlin：字符串模板
来源：http://aun.yonumen.top

"值: $b"
来源：http://axl.tian-w.cn

[T04] Kotlin：空安全
来源：http://ggu.hfpthk.cn

val n: String? = null;  n?.length
来源：http://atr.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://ggy.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ktr.fengsongda.top

[T06] Kotlin：集合映射
来源：http://wzu.quarkkingdee.top

listOf(1, 2, 3).map { it * 2 }
来源：http://iwv.316326.xyz

[T07] Kotlin：集合过滤
来源：http://hoo.ydjk.org.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zgz.aizwys.cn

[T08] Kotlin：数据类
来源：http://ste.sjlbkw.cn

data class User(val name: String, val age: Int)
来源：http://tgt.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://btt.hongshengwenyu.top

fun String.exclaim() = this + "!"
来源：http://jie.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://evj.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qbb.52xcode.cn

[T11] Kotlin：协程
来源：http://bms.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uht.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://lih.kuanghao11.cn

val (a, b) = Pair(1, 2)
来源：http://xat.wangdashe.top

[T13] Kotlin：只读 Map
来源：http://plv.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://qkz.vehdjk.com

[T14] Kotlin：循环
来源：http://oxu.bbcook.cn

for (i in 1..10) println(i)
来源：http://wrb.cashguo.top

[T15] Kotlin：接口
来源：http://byx.shuidangran.top

interface Shape { fun area(): Double }
来源：http://dhq.316326.xyz

[T16] Swift：Hello World
来源：http://xry.jqgfzy.top

print("Hello")
来源：http://vas.jinqigufen.top

[T17] Swift：变量与常量
来源：http://ofy.wangdashe.top

var a = 1;  let b = 2
来源：http://kiu.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://bmg.shuidangran.top

"值: \(b)"
来源：http://twf.tian-w.cn

[T19] Swift：可选绑定
来源：http://tlm.xuetiantiany.cn

if let n = opt { print(n) }
来源：http://nmt.xziqi.cn

[T20] Swift：数组操作
来源：http://hxe.jinyuanbaomall.cn

var a = [1, 2, 3];  a.append(4)
来源：http://aqq.bjfxy.top

[T21] Swift：遍历
来源：http://qfx.jlsjyb.cn

for x in a { print(x) }
来源：http://qra.daria6918.cn

[T22] Swift：字典
来源：http://stn.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://pzt.jinqigufen.top

[T23] Swift：函数
来源：http://pgf.hysaishi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wqq.9152youxi.cn

[T24] Swift：闭包
来源：http://gnv.jiagoushi.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gvj.zhengqikj.top

[T25] Swift：结构体
来源：http://dwc.wangdashe.top

struct P { var x: Int }
来源：http://gia.c1oappe.top

[T26] Swift：类与重写
来源：http://kbh.andypj.xyz

class A: Base { override func f() {} }
来源：http://qhh.zhongyouzk.top

[T27] Swift：错误处理
来源：http://qvo.havefunace.top

do { try f() } catch { print(error) }
来源：http://dyg.hywenlv.cn

[T28] Swift：枚举
来源：http://oru.jqgfzy.top

enum Color { case red, green }
来源：http://rjv.xinyue.icu

[T29] Swift：guard 提前返回
来源：http://aze.dianchejie.cn

guard let x = opt else { return }
来源：http://fax.yongpay.top

[T30] Swift：协议
来源：http://rnb.smart0.xyz

protocol Shape { func area() -> Double }
来源：http://jyc.yanxiufei.cn

[T31] Lua：Hello World
来源：http://xkb.zhoulong.xyz

print("Hello")
来源：http://qkh.hywenlv.cn

[T32] Lua：局部变量
来源：http://xov.yuxming.cn

local a = 1
来源：http://daf.hammf.cn

[T33] Lua：表（数组）
来源：http://mai.xinyue.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://env.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://iyd.0kj1m.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xuj.nanxinkj.top

[T35] Lua：字典表
来源：http://okn.yj202588.top

local d = { a = 1 };  d.b = 2
来源：http://gdy.zhiwuduotai.top

[T36] Lua：函数
来源：http://pzy.ywan-chungtsiang.top

function add(a, b) return a + b end
来源：http://alp.epnwcf.com

[T37] Lua：字符串拼接
来源：http://cbs.snrcjt.cn

"a" .. "b"
来源：http://njz.gogol.net.cn

[T38] Lua：条件
来源：http://zxc.sufxvd.cn

if x > 0 then print("正") end
来源：http://kwk.daxiang520.top

[T39] Lua：模式匹配
来源：http://nvw.dashuyun.cn

string.find(s, "%d+")
来源：http://nmn.guowangkeji.top

[T40] Lua：元表
来源：http://wzi.jiagoushi.top

setmetatable({}, { __index = base })
来源：http://xhs.fktsv.cn

[T41] Perl：Hello World
来源：http://zvx.yfazqb.com

print "Hello\n";
来源：http://lic.yj202588.top

[T42] Perl：变量类型
来源：http://qni.kuanghao11.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bbt.fanxiaobao.xyz

[T43] Perl：字符串插值
来源：http://maq.sufxvd.cn

"值: $a"
来源：http://ame.yanxiufei.cn

[T44] Perl：条件
来源：http://fuz.andypj.xyz

if ($a > 0) { print "正"; }
来源：http://ibo.sweek.top

[T45] Perl：数组遍历
来源：http://tew.andypj.xyz

for my $x (@arr) { print $x; }
来源：http://wxv.yangfankeji.com

[T46] Perl：哈希操作
来源：http://nig.sufxvd.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mjy.jqgufenzy.top

[T47] Perl：正则捕获
来源：http://rer.shzxlz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ddc.fktsv.cn

[T48] Perl：正则替换
来源：http://vjc.hfpthk.cn

$s =~ s/old/new/g;
来源：http://bfi.xuetiantiany.cn

[T49] Perl：函数
来源：http://ibc.ctjpmb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://spk.zhixingplan.top

[T50] Perl：逐行读文件
来源：http://rhc.ctjpmb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://gsp.cucudq.cn

while (my $line = <$fh>) { print $line; }
来源：http://caw.yuxming.cn

[T51] Scala：Hello World
来源：http://rwt.nwbrower.top

println("Hello")
来源：http://mcv.shzxlz.cn

[T52] Scala：变量
来源：http://put.jinqigufen.top

val a = 1;  var b = 2
来源：http://epw.tarul.cn

[T53] Scala：字符串插值
来源：http://cac.mhx1999.top

s"值: $b"
来源：http://ega.zhixingplan.top

[T54] Scala：集合映射
来源：http://drv.yfazqb.com

List(1, 2, 3).map(_ * 2)
来源：http://xcf.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://imx.pycfn.com

List(1, 2, 3).filter(_ > 1)
来源：http://cux.fzhhl.top

[T56] Scala：样例类
来源：http://wdn.sufxvd.cn

case class User(name: String, age: Int)
来源：http://wlf.zhiwuduotai.top

[T57] Scala：模式匹配
来源：http://nuh.ctjpmb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://rlf.svipenyu.cn

[T58] Scala：函数定义
来源：http://fey.smart0.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://lqt.gotoacloud.top

[T59] Scala：循环
来源：http://wsj.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://fdv.yuxming.cn

[T60] Scala：折叠
来源：http://jki.sufxvd.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://emm.guannengcc.top

================================================================================
来源：http://osi.birdmap.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rni.yuxming.cn

================================================================================
来源：http://yph.iojbl.cn

[U01] Py：创建虚拟环境
来源：http://yha.fzhhl.top

python -m venv .venv && source .venv/bin/activate
来源：http://sva.jinqigfzy.top

[U02] Py：导出 / 安装依赖
来源：http://lus.zycfv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cbj.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://yeq.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ofm.hnqzz.top

[U04] Py：变量调试打印
来源：http://iwz.shanyushiyangtech.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eet.jlsjyb.cn

[U05] Py：列表去重且保序
来源：http://wuc.tian-w.cn

list(dict.fromkeys(arr))
来源：http://evh.shangyingyoupin.top

[U06] Py：合并两个字典
来源：http://aem.jlsjyb.cn

{**a, **b}
来源：http://kcn.yonumen.top

[U07] Py：反转字典键值
来源：http://cqn.yj20258.top

{v: k for k, v in d.items()}
来源：http://kxm.vehdjk.com

[U08] Py：展平二维列表
来源：http://gcr.jianghu66.top

[y for x in nested for y in x]
来源：http://wks.shanyushiyangkeji.top

[U09] Py：字典取最大值的键
来源：http://qan.nwbrower.top

max(d, key=d.get)
来源：http://kxr.zhoulong.xyz

[U10] Py：按值排序字典
来源：http://osa.svipenyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rmm.yvedp.cn

[U11] Py：生成器表达式
来源：http://fue.meibo888.top

(x * 2 for x in arr)
来源：http://lye.jqgufenzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://wzt.gaohongyu789.top

Counter(arr).most_common(3)
来源：http://qlo.andypj.xyz

[U13] Py：固定长度队列
来源：http://cjr.hywenlv.cn

deque(maxlen=10)
来源：http://rqz.dashuyun.cn

[U14] Py：分组收集到列表
来源：http://osw.hywenlv.cn

defaultdict(list)
来源：http://wpt.quarkkingdee.top

[U15] Py：高精度计时
来源：http://les.pycfn.com

t = time.perf_counter()
来源：http://lzi.xuetiantiany.cn

[U16] Py：命令行参数解析
来源：http://ixf.fktsv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xyw.tianlin.xyz

[U17] Py：初始化日志
来源：http://yau.sufxvd.cn

logging.basicConfig(level=logging.INFO)
来源：http://zsp.mhx1999.top

[U18] Py：预编译正则
来源：http://byg.c1oappe.top

pat = re.compile(r"\d+")
来源：http://oai.ydzc1.top

[U19] Py：正则替换带回调
来源：http://skj.aibaodan.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rui.jianghu66.top

[U20] Py：缓存函数结果
来源：http://ebo.birdmap.top

@functools.lru_cache(maxsize=None)
来源：http://wpj.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://ckj.zhiwuduotai.top

@contextlib.contextmanager
来源：http://wqx.bjfxy.top

[U22] Py：矩阵转置
来源：http://uez.shanyushiyangkeji.top

list(zip(*m))
来源：http://nuh.snrcjt.cn

[U23] Py：分块读取大文件
来源：http://crt.bjfxy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qpv.0kj1m.cn

[U24] Py：路径操作
来源：http://tpd.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ubc.tanke756.top

[U25] Py：CSV 按字典读
来源：http://qng.zdbjq.cn

csv.DictReader(f)
来源：http://bdg.xinyue.icu

[U26] Py：并发下载
来源：http://zuv.sufxvd.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xry.chenzaomai.com

[U27] Py：异步 HTTP
来源：http://hhw.fzhhl.top

aiohttp.ClientSession() 配合 async with
来源：http://veq.jinghuilouyu.cn

[U28] Py：类型别名
来源：http://sbf.ydjk.org.cn

UserId = int
来源：http://tol.yanxiufei.cn

[U29] Py：属性校验
来源：http://mgl.kuanghao11.cn

@property 与 @x.setter 配合
来源：http://jll.ppjwa.cn

[U30] Py：数据类
来源：http://png.fehbvm.com

@dataclass(slots=True)
来源：http://hum.aizwys.cn

[U31] Py：单测
来源：http://sas.gaohongyu789.top

python -m pytest -q
来源：http://fkz.birdmap.top

[U32] Py：代码格式化
来源：http://bta.hysaishi.cn

ruff format . && ruff check --fix .
来源：http://yas.zhongyouzk.top

[U33] Py：打包发布
来源：http://vmp.mhx1999.top

python -m build  （依赖 pyproject.toml）
来源：http://lue.yangfankeji.com

[U34] Py：判断编码
来源：http://teb.sweek.top

chardet.detect(raw)
来源：http://thk.jianghu66.top

[U35] Py：发送邮件
来源：http://rqi.ydjk.org.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oaz.quarkkingdee.top

[U36] Py：定时任务
来源：http://vjk.zhaomingkeji.xyz

schedule.every(10).minutes.do(job)
来源：http://qjn.redwolf501.top

[U37] Py：读写 Excel
来源：http://ned.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://ats.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://mrm.yj20258888.top

Path(__file__).resolve().parent
来源：http://udz.fktsv.cn

[U39] Py：判断是否在交互环境
来源：http://gwx.hnxiangtu.top

sys.stdout.isatty()
来源：http://hes.yangfankeji.com

[U40] Py：打印到标准错误
来源：http://vzs.jinyuanbaomall.cn

print("err", file=sys.stderr)
来源：http://zji.jyoumei.cn

[U41] PHP：初始化 Composer 项目
来源：http://gtw.xziqi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yhl.birdmap.top

[U42] PHP：PSR-4 自动加载
来源：http://zzg.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hzq.zhixingplan.top

[U43] PHP：声明命名空间
来源：http://xmm.xziqi.cn

namespace App\Http;
来源：http://fyg.gzhubu.top

[U44] PHP：开启严格类型
来源：http://iml.zycfv.cn

declare(strict_types=1);
来源：http://pyv.daxiang520.top

[U45] PHP：类型声明与返回类型
来源：http://hgm.guowangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jqc.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://qde.sxryk.cn

?string $name = null
来源：http://kyd.jiagoushi.top

[U47] PHP：联合类型
来源：http://lyn.zhijiandao.cn

int|string $id
来源：http://qez.9152youxi.cn

[U48] PHP：纯枚举
来源：http://uxg.snrcjt.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qvs.tanke756.top

[U49] PHP：只读属性
来源：http://fap.yj20258.top

public readonly string $name
来源：http://voo.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://vjf.shuidangran.top

public function __construct(private int $id) {}
来源：http://kfz.ppjwa.cn

[U51] PHP：数组解构
来源：http://xod.0kj1m.cn

[$a, $b] = $arr;
来源：http://ftb.daxiang520.top

[U52] PHP：箭头函数
来源：http://zyy.hnxiangtu.top

$double = fn($x) => $x * 2;
来源：http://znb.ivvv.top


<!-- 参考信息 -->