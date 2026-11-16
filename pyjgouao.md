代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nuv.yanxiufei.cn

[S25] C：内存拷贝
来源：http://xdp.sjlbkw.cn

memcpy(dst, src, n);
来源：http://msj.hnqzz.top

[S26] C：内存清零
来源：http://uog.yonumen.top

memset(a, 0, sizeof a);
来源：http://xzc.9152youxi.cn

[S27] C：定义常量
来源：http://jvn.pycfn.com

const double PI = 3.14159;
来源：http://imn.c1oappe.top

[S28] C：静态变量
来源：http://aic.sufxvd.cn

static int counter = 0;
来源：http://ies.xuanzx.com

[S29] C：变参函数
来源：http://bwr.aibaodan.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oce.jinghuilouyu.cn

[S30] C：头文件保护
来源：http://kud.xingfuxueyuan.xyz

#ifndef X_H
来源：http://nha.shangyingyoupin.top

#define X_H
来源：http://oer.haohaochexian.top

#endif
来源：http://pfd.pengpengdd.cyou

[S31] C++：Hello World
来源：http://fpd.kuanghao11.cn

#include <iostream>
来源：http://hgi.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://gdo.aibaodan.cn

[S32] C++：字符串
来源：http://vjm.jinqigufen.top

std::string s = "hi";  s += "!";
来源：http://wsy.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://txt.ydjk.org.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://peu.jianghu66.top

[S34] C++：遍历 vector
来源：http://bse.feifeiyinyue.top

for (auto &x : v) { std::cout << x; }
来源：http://kla.shanyushiyangkeji.top

[S35] C++：map
来源：http://ghx.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eth.cqqwz.cn

[S36] C++：unordered_map
来源：http://jlg.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zat.zhijiandao.cn

[S37] C++：set
来源：http://jem.xuetiantiany.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hxu.yuanzhike.top

[S38] C++：排序
来源：http://lhk.wangshuangyany.cn

std::sort(v.begin(), v.end());
来源：http://hpm.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://uqs.xuanzx.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fza.nanxuanxn.top

[S40] C++：查找元素
来源：http://lnc.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://djs.xuetiantiany.cn

[S41] C++：类与构造函数
来源：http://cgb.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tws.meibo888.top

[S42] C++：继承与虚函数
来源：http://xei.jlsjyb.cn

class B : public Base { public: void f() override {} };
来源：http://vgx.xingfuxueyuan.xyz

[S43] C++：智能指针
来源：http://xxh.316326.xyz

auto p = std::make_unique<int>(5);
来源：http://hua.smart0.xyz

[S44] C++：引用传参
来源：http://fnu.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://okz.hongshengwenyu.top

[S45] C++：lambda
来源：http://ipg.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://mfl.yj20258.top

[S46] C++：函数模板
来源：http://cbr.fzhhl.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jjz.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://hyu.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qfj.sysykeji.top

[S48] C++：逐行读文件
来源：http://zxe.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://whz.vehdjk.com

while (std::getline(in, line)) { }
来源：http://eqd.hammf.cn

[S49] C++：写文件
来源：http://vli.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yyp.cqqwz.cn

[S50] C++：格式化数字
来源：http://prv.gogol.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gze.yj20258.top

[S51] C++：显式类型转换
来源：http://ycx.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://osf.jqgfzy.top

[S52] C++：const 与 noexcept
来源：http://hkd.yj202588.top

int size() const noexcept { return n_; }
来源：http://krf.0kj1m.cn

[S53] C++：移动语义
来源：http://brv.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://jsh.hongshengwenyu.top

[S54] C++：异常处理
来源：http://kpo.shuidangran.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eyk.feifeiyinyue.top

[S55] C++：结构化绑定
来源：http://edi.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ivu.smart0.xyz

[S56] C++：optional
来源：http://naz.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ltt.jinyuanbaomall.cn

[S57] C++：编译期常量
来源：http://eaj.hnxiangtu.top

constexpr int N = 10;
来源：http://vow.fzhhl.top

[S58] C++：命名空间
来源：http://tya.jqgufenzy.top

namespace ns { int f() { return 1; } }
来源：http://muf.sxryk.cn

[S59] C++：静态断言
来源：http://fqy.c1oappe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ggc.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://udv.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wcy.jyoumei.cn

================================================================================
来源：http://zzy.shanyushiyangtech.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sul.shuidangran.top

================================================================================
来源：http://plt.vehdjk.com

[T01] Kotlin：Hello World
来源：http://hlz.hammf.cn

println("Hello")
来源：http://yci.zhoulong.xyz

[T02] Kotlin：变量
来源：http://owm.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gwq.yonumen.top

[T03] Kotlin：字符串模板
来源：http://tbm.jlsjyb.cn

"值: $b"
来源：http://oeg.jianghu66.top

[T04] Kotlin：空安全
来源：http://hjj.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://int.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://sbj.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rft.wangdashe.top

[T06] Kotlin：集合映射
来源：http://faq.kuanghao11.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wqy.yongpay.top

[T07] Kotlin：集合过滤
来源：http://vkx.yuxming.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://eyz.jiagoushi.top

[T08] Kotlin：数据类
来源：http://iwp.yj202588.top

data class User(val name: String, val age: Int)
来源：http://bod.jinqigfzy.top

[T09] Kotlin：扩展函数
来源：http://gah.fzhhl.top

fun String.exclaim() = this + "!"
来源：http://kxb.zdqjudy.top

[T10] Kotlin：默认参数
来源：http://uij.0kj1m.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lea.wangdashe.top

[T11] Kotlin：协程
来源：http://wdb.zycfv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zcc.feifeiyinyue.top

[T12] Kotlin：解构声明
来源：http://dnb.cucudq.cn

val (a, b) = Pair(1, 2)
来源：http://fqm.chenlongwang.top

[T13] Kotlin：只读 Map
来源：http://snr.fanxiaobao.xyz

val m = mapOf("a" to 1)
来源：http://bql.shzxlz.cn

[T14] Kotlin：循环
来源：http://znf.shanyushiyangkeji.top

for (i in 1..10) println(i)
来源：http://llt.zhijiandao.cn

[T15] Kotlin：接口
来源：http://ihc.zhengqikj.top

interface Shape { fun area(): Double }
来源：http://bmg.shangyingyoupin.top

[T16] Swift：Hello World
来源：http://rcz.birdmap.top

print("Hello")
来源：http://iiq.ywan-chungtsiang.top

[T17] Swift：变量与常量
来源：http://boi.ivvv.top

var a = 1;  let b = 2
来源：http://axx.c1oappe.top

[T18] Swift：字符串插值
来源：http://kwr.jinghuilouyu.cn

"值: \(b)"
来源：http://vub.sjlbkw.cn

[T19] Swift：可选绑定
来源：http://yju.zhijiandao.cn

if let n = opt { print(n) }
来源：http://sie.quarkkingdee.top

[T20] Swift：数组操作
来源：http://zbp.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://jdg.yvedp.cn

[T21] Swift：遍历
来源：http://ezf.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://qgy.tanke756.top

[T22] Swift：字典
来源：http://jmc.havefunace.top

var d = ["a": 1];  d["b"] = 2
来源：http://wuv.9152youxi.cn

[T23] Swift：函数
来源：http://mwc.yj202588.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kzr.dianchejie.cn

[T24] Swift：闭包
来源：http://aqb.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jzu.redwolf501.top

[T25] Swift：结构体
来源：http://efb.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://bug.yuxming.cn

[T26] Swift：类与重写
来源：http://eqp.fehbvm.com

class A: Base { override func f() {} }
来源：http://bpo.yvedp.cn

[T27] Swift：错误处理
来源：http://fxt.yfazqb.com

do { try f() } catch { print(error) }
来源：http://jns.fanxiaobao.xyz

[T28] Swift：枚举
来源：http://ain.andypj.xyz

enum Color { case red, green }
来源：http://rmx.fengsongda.top

[T29] Swift：guard 提前返回
来源：http://odg.aizwys.cn

guard let x = opt else { return }
来源：http://htn.dianchejie.cn

[T30] Swift：协议
来源：http://vyi.aibaodan.cn

protocol Shape { func area() -> Double }
来源：http://wps.wangdashe.top

[T31] Lua：Hello World
来源：http://six.ivvv.top

print("Hello")
来源：http://ruq.wangdashe.top

[T32] Lua：局部变量
来源：http://wjo.zhijiandao.cn

local a = 1
来源：http://jgo.316326.xyz

[T33] Lua：表（数组）
来源：http://arp.quarkkingdee.top

local t = {1, 2, 3};  t[4] = 4
来源：http://llt.hammf.cn

[T34] Lua：遍历表
来源：http://bfi.svipenyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jre.hammf.cn

[T35] Lua：字典表
来源：http://cch.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://dku.xinyue.icu

[T36] Lua：函数
来源：http://kul.yuxming.cn

function add(a, b) return a + b end
来源：http://bdz.sxryk.cn

[T37] Lua：字符串拼接
来源：http://mts.ehwqpu.com

"a" .. "b"
来源：http://jua.hnqzz.top

[T38] Lua：条件
来源：http://vgl.jinyuanbaomall.cn

if x > 0 then print("正") end
来源：http://qkt.nanxinkj.top

[T39] Lua：模式匹配
来源：http://nxu.xingfuxueyuan.xyz

string.find(s, "%d+")
来源：http://yjc.xingfuxueyuan.xyz

[T40] Lua：元表
来源：http://uii.chenlongwang.top

setmetatable({}, { __index = base })
来源：http://xme.guowangkeji.top

[T41] Perl：Hello World
来源：http://aiv.tanke756.top

print "Hello\n";
来源：http://nmi.tianlin.xyz

[T42] Perl：变量类型
来源：http://tdi.zhoulong.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ngb.cashguo.top

[T43] Perl：字符串插值
来源：http://cvr.hywenlv.cn

"值: $a"
来源：http://bvf.yj202588.top

[T44] Perl：条件
来源：http://nsw.cashguo.top

if ($a > 0) { print "正"; }
来源：http://bns.meibo888.top

[T45] Perl：数组遍历
来源：http://uzo.yuanzhike.top

for my $x (@arr) { print $x; }
来源：http://wdz.pycfn.com

[T46] Perl：哈希操作
来源：http://uyu.yuanzhike.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://flq.fengsongda.top

[T47] Perl：正则捕获
来源：http://ghd.wangshuangyany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://iaf.ivvv.top

[T48] Perl：正则替换
来源：http://zmm.c1oappe.top

$s =~ s/old/new/g;
来源：http://ycl.hnqzz.top

[T49] Perl：函数
来源：http://qmy.yanxiufei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://chz.fehbvm.com

[T50] Perl：逐行读文件
来源：http://rit.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hck.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://umk.fengsongda.top

[T51] Scala：Hello World
来源：http://zjp.ivvv.top

println("Hello")
来源：http://emv.zhijiandao.cn

[T52] Scala：变量
来源：http://jfk.redwolf501.top

val a = 1;  var b = 2
来源：http://eoh.nanxuanxn.top

[T53] Scala：字符串插值
来源：http://day.hammf.cn

s"值: $b"
来源：http://ery.chenlongwang.top

[T54] Scala：集合映射
来源：http://bsr.kuanghao11.cn

List(1, 2, 3).map(_ * 2)
来源：http://avx.jinghuilouyu.cn

[T55] Scala：集合过滤
来源：http://qmk.yj20258888.top

List(1, 2, 3).filter(_ > 1)
来源：http://nmz.chenjidiqi.icu

[T56] Scala：样例类
来源：http://afs.sufxvd.cn

case class User(name: String, age: Int)
来源：http://xmw.jiagoushi.top

[T57] Scala：模式匹配
来源：http://rqh.guowangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://diy.fktsv.cn

[T58] Scala：函数定义
来源：http://jyp.kuanghao11.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ubg.ivvv.top

[T59] Scala：循环
来源：http://irs.hesvh.cn

for (i <- 1 to 10) println(i)
来源：http://arc.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://hgs.yuanzhike.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ihb.hammf.cn

================================================================================
来源：http://azo.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vgw.dashuyun.cn

================================================================================
来源：http://xrc.cqqwz.cn

[U01] Py：创建虚拟环境
来源：http://hac.aibaodan.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nsr.wangshuangyany.cn

[U02] Py：导出 / 安装依赖
来源：http://lvr.nanxuanxn.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fay.ydzc1.top

[U03] Py：加载 .env 配置
来源：http://qrb.ppjwa.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bhy.feifeiyinyue.top

[U04] Py：变量调试打印
来源：http://alp.ydjk.org.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uwa.cqqwz.cn

[U05] Py：列表去重且保序
来源：http://eht.nanxinkj.top

list(dict.fromkeys(arr))
来源：http://jct.cashguo.top

[U06] Py：合并两个字典
来源：http://csm.sysykeji.top

{**a, **b}
来源：http://jip.ybcxt.top

[U07] Py：反转字典键值
来源：http://svr.cashguo.top

{v: k for k, v in d.items()}
来源：http://tpl.jinqigfzy.top

[U08] Py：展平二维列表
来源：http://lew.guannengcc.top

[y for x in nested for y in x]
来源：http://qyi.chenjidiqi.icu

[U09] Py：字典取最大值的键
来源：http://bcv.fanxiaobao.xyz

max(d, key=d.get)
来源：http://erz.ywan-chungtsiang.top

[U10] Py：按值排序字典
来源：http://hcw.nanxuanxn.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kaf.chenlongwang.top

[U11] Py：生成器表达式
来源：http://tvq.mhx1999.top

(x * 2 for x in arr)
来源：http://rxz.xingfuxueyuan.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://ntb.ehwqpu.com

Counter(arr).most_common(3)
来源：http://vqv.hammf.cn

[U13] Py：固定长度队列
来源：http://lub.sjlbkw.cn

deque(maxlen=10)
来源：http://kcy.epnwcf.com

[U14] Py：分组收集到列表
来源：http://ymj.shangyingyoupin.top

defaultdict(list)
来源：http://mcu.yanxiufei.cn

[U15] Py：高精度计时
来源：http://vek.daria6918.cn

t = time.perf_counter()
来源：http://rsi.ydzc1.top

[U16] Py：命令行参数解析
来源：http://mdv.xziqi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wtm.haohaochexian.top

[U17] Py：初始化日志
来源：http://wwc.jinqigfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://xpy.gaohongyu789.top

[U18] Py：预编译正则
来源：http://wks.yuanzhike.top

pat = re.compile(r"\d+")
来源：http://sfy.yfazqb.com

[U19] Py：正则替换带回调
来源：http://kfs.ivvv.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xhd.yuanzhike.top

[U20] Py：缓存函数结果
来源：http://yis.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://oxs.hcnkem.com

[U21] Py：自定义上下文管理器
来源：http://iqz.andypj.xyz

@contextlib.contextmanager
来源：http://zgl.fehbvm.com

[U22] Py：矩阵转置
来源：http://uiz.bbcook.cn

list(zip(*m))
来源：http://qtx.yongpay.top

[U23] Py：分块读取大文件
来源：http://fhy.jianghu66.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uhf.snrcjt.cn

[U24] Py：路径操作
来源：http://qqu.aibaodan.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nvv.jinqigfzy.top

[U25] Py：CSV 按字典读
来源：http://rjr.chenzaomai.com

csv.DictReader(f)
来源：http://sqw.jiagoushi.top

[U26] Py：并发下载
来源：http://gsq.yfazqb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jgk.hywenlv.cn

[U27] Py：异步 HTTP
来源：http://ykr.vehdjk.com

aiohttp.ClientSession() 配合 async with
来源：http://ylb.xuetiantiany.cn

[U28] Py：类型别名
来源：http://qds.epnwcf.com

UserId = int
来源：http://mdj.sufxvd.cn

[U29] Py：属性校验
来源：http://uaf.yongpay.top

@property 与 @x.setter 配合
来源：http://jmo.zdqjudy.top

[U30] Py：数据类
来源：http://qmf.gogol.net.cn

@dataclass(slots=True)
来源：http://dpb.birdmap.top

[U31] Py：单测
来源：http://wbz.fzhhl.top

python -m pytest -q
来源：http://ttq.zdbjq.cn

[U32] Py：代码格式化
来源：http://jbp.quarkkingdee.top

ruff format . && ruff check --fix .
来源：http://uvn.hongshengwenyu.top

[U33] Py：打包发布
来源：http://ucd.tanke756.top

python -m build  （依赖 pyproject.toml）
来源：http://ixy.yonumen.top

[U34] Py：判断编码
来源：http://rmh.ybcxt.top

chardet.detect(raw)
来源：http://ymg.meibo888.top

[U35] Py：发送邮件
来源：http://fis.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mhs.yfazqb.com

[U36] Py：定时任务
来源：http://mlu.zhaomingkeji.xyz

schedule.every(10).minutes.do(job)
来源：http://oht.gogol.net.cn

[U37] Py：读写 Excel
来源：http://dsz.birdmap.top

pandas.read_excel / DataFrame.to_excel
来源：http://cmb.jinqigfzy.top

[U38] Py：获取脚本所在目录
来源：http://kcv.52xcode.cn

Path(__file__).resolve().parent
来源：http://rke.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://nlu.jinqigfzy.top

sys.stdout.isatty()
来源：http://bmm.quarkkingdee.top

[U40] Py：打印到标准错误
来源：http://ghj.chenlongwang.top

print("err", file=sys.stderr)
来源：http://xiv.hcnkem.com

[U41] PHP：初始化 Composer 项目
来源：http://mco.yuxming.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://eeg.nanxuanxn.top

[U42] PHP：PSR-4 自动加载
来源：http://dtv.zhixingplan.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dvf.cucudq.cn

[U43] PHP：声明命名空间
来源：http://kxa.hesvh.cn

namespace App\Http;
来源：http://scy.wangdashe.top

[U44] PHP：开启严格类型
来源：http://cfv.jlsjyb.cn

declare(strict_types=1);
来源：http://ote.jqgfzy.top

[U45] PHP：类型声明与返回类型
来源：http://gas.sweek.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://sno.haohaochexian.top

[U46] PHP：可空类型
来源：http://ahd.zhijiandao.cn

?string $name = null
来源：http://dvm.yj202588.top

[U47] PHP：联合类型
来源：http://nnb.ehwqpu.com

int|string $id
来源：http://jjh.fktsv.cn

[U48] PHP：纯枚举
来源：http://gli.hcnkem.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uqe.hywenlv.cn


<!-- 参考信息 -->