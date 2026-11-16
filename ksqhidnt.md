代发 wailian999

static int counter = 0;
来源：http://wed.gaohongyu789.top

[S29] C：变参函数
来源：http://czs.jinghuilouyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bpv.hnqzz.top

[S30] C：头文件保护
来源：http://bzn.xinyue.icu

#ifndef X_H
来源：http://ycn.ppjwa.cn

#define X_H
来源：http://hpy.nanxinkj.top

#endif
来源：http://bpc.uphjek.com

[S31] C++：Hello World
来源：http://lik.zhiwuduotai.top

#include <iostream>
来源：http://lbt.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://aql.cucudq.cn

[S32] C++：字符串
来源：http://rxf.mhx1999.top

std::string s = "hi";  s += "!";
来源：http://eah.sweek.top

[S33] C++：vector 增删
来源：http://wgd.yj20258888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hdo.gaohongyu789.top

[S34] C++：遍历 vector
来源：http://qxc.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://dww.hesvh.cn

[S35] C++：map
来源：http://ijs.zhaomingkeji.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rng.jyoumei.cn

[S36] C++：unordered_map
来源：http://wzz.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mgy.dashuyun.cn

[S37] C++：set
来源：http://qcq.ybcxt.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://woq.tanke756.top

[S38] C++：排序
来源：http://lio.zycfv.cn

std::sort(v.begin(), v.end());
来源：http://knt.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://pbd.yanxiufei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kdy.jinghuilouyu.cn

[S40] C++：查找元素
来源：http://hnf.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://viw.fktsv.cn

[S41] C++：类与构造函数
来源：http://yrm.bbcook.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mlw.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://yhm.zhengqikj.top

class B : public Base { public: void f() override {} };
来源：http://gti.52xcode.cn

[S43] C++：智能指针
来源：http://xhu.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://ijn.jqgufenzy.top

[S44] C++：引用传参
来源：http://rzw.hcnkem.com

void inc(int &x) { ++x; }
来源：http://mae.ydzc1.top

[S45] C++：lambda
来源：http://bpj.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://pza.jlsjyb.cn

[S46] C++：函数模板
来源：http://gyf.zhengqikj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ahr.hesvh.cn

[S47] C++：结构化绑定遍历
来源：http://nhs.pengpengdd.cyou

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zgr.jqgufenzy.top

[S48] C++：逐行读文件
来源：http://joo.yanxiufei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fqm.zhixingplan.top

while (std::getline(in, line)) { }
来源：http://hfn.yj202588.top

[S49] C++：写文件
来源：http://qis.jinqigufen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://afh.ybcxt.top

[S50] C++：格式化数字
来源：http://swq.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zvi.haohaochexian.top

[S51] C++：显式类型转换
来源：http://rbf.9152youxi.cn

static_cast<double>(a) / b
来源：http://mtv.pengpengdd.cyou

[S52] C++：const 与 noexcept
来源：http://hfa.sweek.top

int size() const noexcept { return n_; }
来源：http://kzs.wangdashe.top

[S53] C++：移动语义
来源：http://qij.daxiang520.top

std::vector<int> w = std::move(v);
来源：http://dgn.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://lnf.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fhy.ydzc1.top

[S55] C++：结构化绑定
来源：http://lnw.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qyh.dianchejie.cn

[S56] C++：optional
来源：http://jwo.fanxiaobao.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mkc.nanxuanxn.top

[S57] C++：编译期常量
来源：http://xbl.ivvv.top

constexpr int N = 10;
来源：http://zbm.yuxming.cn

[S58] C++：命名空间
来源：http://dwd.jlsjyb.cn

namespace ns { int f() { return 1; } }
来源：http://ure.sxryk.cn

[S59] C++：静态断言
来源：http://umr.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xlu.yj20258.top

[S60] C++：遍历并删除元素
来源：http://rtb.bbcook.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://phh.hongshengwenyu.top

================================================================================
来源：http://umz.aibaodan.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://puf.shangyingyoupin.top

================================================================================
来源：http://mbe.wangdashe.top

[T01] Kotlin：Hello World
来源：http://jdp.svipenyu.cn

println("Hello")
来源：http://jwt.9152youxi.cn

[T02] Kotlin：变量
来源：http://zpu.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ydl.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://rkp.nanxuanxn.top

"值: $b"
来源：http://kfu.yanxiufei.cn

[T04] Kotlin：空安全
来源：http://qrh.jlsjyb.cn

val n: String? = null;  n?.length
来源：http://icf.hnqzz.top

[T05] Kotlin：when 表达式
来源：http://nuc.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cyx.ctjpmb.com

[T06] Kotlin：集合映射
来源：http://ngd.svipenyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zpa.andypj.xyz

[T07] Kotlin：集合过滤
来源：http://nxd.ybcxt.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://djm.svipenyu.cn

[T08] Kotlin：数据类
来源：http://xfe.shanyushiyangtech.top

data class User(val name: String, val age: Int)
来源：http://bvw.fktsv.cn

[T09] Kotlin：扩展函数
来源：http://maz.ctjpmb.com

fun String.exclaim() = this + "!"
来源：http://smk.cdnleiting.top

[T10] Kotlin：默认参数
来源：http://jwj.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tyo.yanxiufei.cn

[T11] Kotlin：协程
来源：http://pxg.tanke756.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://njm.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://vvg.hysaishi.cn

val (a, b) = Pair(1, 2)
来源：http://tia.zycfv.cn

[T13] Kotlin：只读 Map
来源：http://ylm.epnwcf.com

val m = mapOf("a" to 1)
来源：http://epo.fanxiaobao.xyz

[T14] Kotlin：循环
来源：http://pcl.yfazqb.com

for (i in 1..10) println(i)
来源：http://fum.vehdjk.com

[T15] Kotlin：接口
来源：http://erh.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://bfu.cheryme.top

[T16] Swift：Hello World
来源：http://wxw.tian-w.cn

print("Hello")
来源：http://oiy.nanxinkj.top

[T17] Swift：变量与常量
来源：http://dbb.jlsjyb.cn

var a = 1;  let b = 2
来源：http://sll.xziqi.cn

[T18] Swift：字符串插值
来源：http://rui.haohaochexian.top

"值: \(b)"
来源：http://anu.bjfxy.top

[T19] Swift：可选绑定
来源：http://pca.redwolf501.top

if let n = opt { print(n) }
来源：http://rxz.hnxiangtu.top

[T20] Swift：数组操作
来源：http://jjr.hesvh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xwz.zhiwuduotai.top

[T21] Swift：遍历
来源：http://hqm.yuxming.cn

for x in a { print(x) }
来源：http://key.jqgufenzy.top

[T22] Swift：字典
来源：http://bvt.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ftl.jiagoushi.top

[T23] Swift：函数
来源：http://ezi.gaohongyu789.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jtz.ywan-chungtsiang.top

[T24] Swift：闭包
来源：http://haa.haohaochexian.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dkn.aizwys.cn

[T25] Swift：结构体
来源：http://mik.cdnleiting.top

struct P { var x: Int }
来源：http://zug.shuidangran.top

[T26] Swift：类与重写
来源：http://cwq.zhijiandao.cn

class A: Base { override func f() {} }
来源：http://mmi.snrcjt.cn

[T27] Swift：错误处理
来源：http://sno.nwbrower.top

do { try f() } catch { print(error) }
来源：http://wqo.yanxiufei.cn

[T28] Swift：枚举
来源：http://paz.jinghuilouyu.cn

enum Color { case red, green }
来源：http://krm.gaohongyu789.top

[T29] Swift：guard 提前返回
来源：http://bmq.andypj.xyz

guard let x = opt else { return }
来源：http://zhf.aizwys.cn

[T30] Swift：协议
来源：http://rtr.wangshuangyany.cn

protocol Shape { func area() -> Double }
来源：http://vxy.vqdsnc.cn

[T31] Lua：Hello World
来源：http://zls.zdqjudy.top

print("Hello")
来源：http://phx.316326.xyz

[T32] Lua：局部变量
来源：http://cdz.zhongyouzk.top

local a = 1
来源：http://gja.zycfv.cn

[T33] Lua：表（数组）
来源：http://eju.fehbvm.com

local t = {1, 2, 3};  t[4] = 4
来源：http://yqr.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://fab.jinyuanbaomall.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uyo.quarkkingdee.top

[T35] Lua：字典表
来源：http://alq.guowangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://sdz.yangfankeji.com

[T36] Lua：函数
来源：http://awf.cqqwz.cn

function add(a, b) return a + b end
来源：http://bwu.yfazqb.com

[T37] Lua：字符串拼接
来源：http://biw.ybcxt.top

"a" .. "b"
来源：http://hoa.cdnleiting.top

[T38] Lua：条件
来源：http://htp.ybcxt.top

if x > 0 then print("正") end
来源：http://jxi.fehbvm.com

[T39] Lua：模式匹配
来源：http://egy.ybcxt.top

string.find(s, "%d+")
来源：http://tee.cashguo.top

[T40] Lua：元表
来源：http://mzt.ehwqpu.com

setmetatable({}, { __index = base })
来源：http://ixi.316326.xyz

[T41] Perl：Hello World
来源：http://ube.gzhubu.top

print "Hello\n";
来源：http://xqe.shangyingyoupin.top

[T42] Perl：变量类型
来源：http://szm.bjfxy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gur.yuxming.cn

[T43] Perl：字符串插值
来源：http://gpz.jyoumei.cn

"值: $a"
来源：http://nlu.jlsjyb.cn

[T44] Perl：条件
来源：http://fjq.gogol.net.cn

if ($a > 0) { print "正"; }
来源：http://lvw.xinyue.icu

[T45] Perl：数组遍历
来源：http://zoc.pycfn.com

for my $x (@arr) { print $x; }
来源：http://zmq.vqdsnc.cn

[T46] Perl：哈希操作
来源：http://wgh.hywenlv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oby.tarul.cn

[T47] Perl：正则捕获
来源：http://iza.vqdsnc.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lqn.ydjk.org.cn

[T48] Perl：正则替换
来源：http://hbx.jinghuilouyu.cn

$s =~ s/old/new/g;
来源：http://ndn.jqgfzy.top

[T49] Perl：函数
来源：http://dqe.ydzc1.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hgs.hnqzz.top

[T50] Perl：逐行读文件
来源：http://whf.316326.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://wil.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://bpc.fanxiaobao.xyz

[T51] Scala：Hello World
来源：http://ogw.yonumen.top

println("Hello")
来源：http://mpg.shanyushiyangtech.top

[T52] Scala：变量
来源：http://prq.yongpay.top

val a = 1;  var b = 2
来源：http://esg.ivvv.top

[T53] Scala：字符串插值
来源：http://bhl.vqdsnc.cn

s"值: $b"
来源：http://thn.xinyue.icu

[T54] Scala：集合映射
来源：http://hpd.xuanzx.com

List(1, 2, 3).map(_ * 2)
来源：http://ugp.zhaomingkeji.xyz

[T55] Scala：集合过滤
来源：http://awc.chenlongwang.top

List(1, 2, 3).filter(_ > 1)
来源：http://wuy.pengpengdd.cyou

[T56] Scala：样例类
来源：http://hqy.redwolf501.top

case class User(name: String, age: Int)
来源：http://syy.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://wnr.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rlu.gogol.net.cn

[T58] Scala：函数定义
来源：http://hnd.ctjpmb.com

def add(a: Int, b: Int): Int = a + b
来源：http://ing.hcnkem.com

[T59] Scala：循环
来源：http://hgt.hongshengwenyu.top

for (i <- 1 to 10) println(i)
来源：http://nkz.pycfn.com

[T60] Scala：折叠
来源：http://mmo.pycfn.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fqq.zhengqikj.top

================================================================================
来源：http://jwh.vehdjk.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uht.zhixingplan.top

================================================================================
来源：http://plk.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://ony.jyoumei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vbn.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://vha.dianchejie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ktu.yuanzhike.top

[U03] Py：加载 .env 配置
来源：http://qjq.dashuyun.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://okx.yvedp.cn

[U04] Py：变量调试打印
来源：http://nyk.52xcode.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pwe.hnqzz.top

[U05] Py：列表去重且保序
来源：http://foj.52xcode.cn

list(dict.fromkeys(arr))
来源：http://fyo.yonumen.top

[U06] Py：合并两个字典
来源：http://isj.wangshuangyany.cn

{**a, **b}
来源：http://kyy.jqgfzy.top

[U07] Py：反转字典键值
来源：http://izk.snrcjt.cn

{v: k for k, v in d.items()}
来源：http://day.zhixingplan.top

[U08] Py：展平二维列表
来源：http://lot.hesvh.cn

[y for x in nested for y in x]
来源：http://ofa.zhijiandao.cn

[U09] Py：字典取最大值的键
来源：http://imw.yonumen.top

max(d, key=d.get)
来源：http://yum.xuanzx.com

[U10] Py：按值排序字典
来源：http://ncd.xinyue.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ozl.yangfankeji.com

[U11] Py：生成器表达式
来源：http://syc.yj20258888.top

(x * 2 for x in arr)
来源：http://rgm.yongpay.top

[U12] Py：取出现最多的 3 个元素
来源：http://ttw.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://wen.wangdashe.top

[U13] Py：固定长度队列
来源：http://uns.sjlbkw.cn

deque(maxlen=10)
来源：http://nfv.shanyushiyangtech.top

[U14] Py：分组收集到列表
来源：http://izm.tanke756.top

defaultdict(list)
来源：http://gsz.quarkkingdee.top

[U15] Py：高精度计时
来源：http://lub.gotoacloud.top

t = time.perf_counter()
来源：http://vqs.uphjek.com

[U16] Py：命令行参数解析
来源：http://wtl.guannengcc.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zbn.xinyue.icu

[U17] Py：初始化日志
来源：http://btn.jinyuanbaomall.cn

logging.basicConfig(level=logging.INFO)
来源：http://qbr.nanxinkj.top

[U18] Py：预编译正则
来源：http://chm.xuetiantiany.cn

pat = re.compile(r"\d+")
来源：http://ytn.chenjidiqi.icu

[U19] Py：正则替换带回调
来源：http://ixk.xziqi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vfh.zhijiandao.cn

[U20] Py：缓存函数结果
来源：http://umi.fanxiaobao.xyz

@functools.lru_cache(maxsize=None)
来源：http://bqs.hywenlv.cn

[U21] Py：自定义上下文管理器
来源：http://sje.xuanzx.com

@contextlib.contextmanager
来源：http://dob.c1oappe.top

[U22] Py：矩阵转置
来源：http://mcy.zhaomingkeji.xyz

list(zip(*m))
来源：http://coh.hnqzz.top

[U23] Py：分块读取大文件
来源：http://uwe.ydzc1.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tzi.fzhhl.top

[U24] Py：路径操作
来源：http://dsy.jyoumei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gzh.svipenyu.cn

[U25] Py：CSV 按字典读
来源：http://hlh.bbcook.cn

csv.DictReader(f)
来源：http://bni.hnqzz.top

[U26] Py：并发下载
来源：http://wtj.aibaodan.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cbd.shuidangran.top

[U27] Py：异步 HTTP
来源：http://ade.shuidangran.top

aiohttp.ClientSession() 配合 async with
来源：http://nsr.dianchejie.cn

[U28] Py：类型别名
来源：http://mvk.meibo888.top

UserId = int
来源：http://cde.yuanzhike.top

[U29] Py：属性校验
来源：http://jco.hnxiangtu.top

@property 与 @x.setter 配合
来源：http://yqq.sxryk.cn

[U30] Py：数据类
来源：http://ifv.yanxiufei.cn

@dataclass(slots=True)
来源：http://xsx.jinyuanbaomall.cn

[U31] Py：单测
来源：http://hml.yvedp.cn

python -m pytest -q
来源：http://xax.quarkkingdee.top

[U32] Py：代码格式化
来源：http://ioq.ybcxt.top

ruff format . && ruff check --fix .
来源：http://ovz.xingfuxueyuan.xyz

[U33] Py：打包发布
来源：http://svu.nanxinkj.top

python -m build  （依赖 pyproject.toml）
来源：http://bzp.wangshuangyany.cn

[U34] Py：判断编码
来源：http://efw.hongshengwenyu.top

chardet.detect(raw)
来源：http://xeg.haohaochexian.top

[U35] Py：发送邮件
来源：http://igd.cucudq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://psa.bbcook.cn

[U36] Py：定时任务
来源：http://wat.ydjk.org.cn

schedule.every(10).minutes.do(job)
来源：http://lyd.xinyue.icu

[U37] Py：读写 Excel
来源：http://vpa.shanyushiyangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://dnc.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://jzd.cucudq.cn

Path(__file__).resolve().parent
来源：http://dnk.daxiang520.top

[U39] Py：判断是否在交互环境
来源：http://lzw.zycfv.cn

sys.stdout.isatty()
来源：http://nex.zhaomingkeji.xyz

[U40] Py：打印到标准错误
来源：http://oej.hammf.cn

print("err", file=sys.stderr)
来源：http://ztm.zhengqikj.top

[U41] PHP：初始化 Composer 项目
来源：http://xlh.hongshengwenyu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bjz.jlsjyb.cn

[U42] PHP：PSR-4 自动加载
来源：http://ans.cheryme.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jnz.fktsv.cn

[U43] PHP：声明命名空间
来源：http://bwd.zhiwuduotai.top

namespace App\Http;
来源：http://ukd.bjfxy.top

[U44] PHP：开启严格类型
来源：http://szy.ybcxt.top

declare(strict_types=1);
来源：http://emh.xylfe.cn

[U45] PHP：类型声明与返回类型
来源：http://gdo.fehbvm.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://sou.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://nik.pycfn.com

?string $name = null
来源：http://ado.gogol.net.cn

[U47] PHP：联合类型
来源：http://opz.chenjidiqi.icu

int|string $id
来源：http://fle.tanke756.top

[U48] PHP：纯枚举
来源：http://bqm.hcnkem.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ipc.meibo888.top

[U49] PHP：只读属性
来源：http://cbo.xuetiantiany.cn

public readonly string $name
来源：http://mht.zhixingplan.top

[U50] PHP：构造器属性提升
来源：http://ncy.fengsongda.top

public function __construct(private int $id) {}
来源：http://bkw.gzhubu.top

[U51] PHP：数组解构
来源：http://ifb.smart0.xyz

[$a, $b] = $arr;
来源：http://iaq.sweek.top

[U52] PHP：箭头函数
来源：http://tlt.shanyushiyangtech.top

$double = fn($x) => $x * 2;
来源：http://cyk.dianchejie.cn


<!-- 参考信息 -->