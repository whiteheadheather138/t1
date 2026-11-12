代发 wailian999

static int counter = 0;
来源：http://qpx.zhiwuduotai.top

[S29] C：变参函数
来源：http://zyp.yj202588.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qjo.meibo888.top

[S30] C：头文件保护
来源：http://jag.redwolf501.top

#ifndef X_H
来源：http://hwd.andypj.xyz

#define X_H
来源：http://xri.ctjpmb.com

#endif
来源：http://wvd.ivvv.top

[S31] C++：Hello World
来源：http://bvo.sjlbkw.cn

#include <iostream>
来源：http://gdi.zhixingplan.top

int main() { std::cout << "Hello\n"; }
来源：http://fpz.pengpengdd.cyou

[S32] C++：字符串
来源：http://izc.sxryk.cn

std::string s = "hi";  s += "!";
来源：http://rwr.cashguo.top

[S33] C++：vector 增删
来源：http://yzd.gogol.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://byp.jinyuanbaomall.cn

[S34] C++：遍历 vector
来源：http://qjl.fehbvm.com

for (auto &x : v) { std::cout << x; }
来源：http://cdi.ppjwa.cn

[S35] C++：map
来源：http://xuj.hysaishi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://prd.birdmap.top

[S36] C++：unordered_map
来源：http://rjg.sweek.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cep.nanxuanxn.top

[S37] C++：set
来源：http://ziw.ybcxt.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uik.chenlongwang.top

[S38] C++：排序
来源：http://uyr.svipenyu.cn

std::sort(v.begin(), v.end());
来源：http://iya.tian-w.cn

[S39] C++：自定义比较器排序
来源：http://qbk.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zoe.yanxiufei.cn

[S40] C++：查找元素
来源：http://gnf.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gpf.cheryme.top

[S41] C++：类与构造函数
来源：http://sxh.fktsv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://otg.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://aah.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://hdx.nanxuanxn.top

[S43] C++：智能指针
来源：http://tem.c1oappe.top

auto p = std::make_unique<int>(5);
来源：http://iar.hammf.cn

[S44] C++：引用传参
来源：http://rnm.zhoulong.xyz

void inc(int &x) { ++x; }
来源：http://eaq.shanyushiyangkeji.top

[S45] C++：lambda
来源：http://rwq.tarul.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zsa.shanyushiyangkeji.top

[S46] C++：函数模板
来源：http://bac.smart0.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xdj.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://pbz.316326.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hnv.hfpthk.cn

[S48] C++：逐行读文件
来源：http://occ.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://rbn.ybcxt.top

while (std::getline(in, line)) { }
来源：http://ele.hammf.cn

[S49] C++：写文件
来源：http://ltb.meibo888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lzd.fehbvm.com

[S50] C++：格式化数字
来源：http://bvi.smart0.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lyc.zdbjq.cn

[S51] C++：显式类型转换
来源：http://raa.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://ixv.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://lgg.bjfxy.top

int size() const noexcept { return n_; }
来源：http://itj.dianchejie.cn

[S53] C++：移动语义
来源：http://etg.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://mgy.xingfuxueyuan.xyz

[S54] C++：异常处理
来源：http://qsp.jinqigfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mfr.meibo888.top

[S55] C++：结构化绑定
来源：http://kgv.jiagoushi.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uio.zycfv.cn

[S56] C++：optional
来源：http://nnn.ppjwa.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hsd.aibaodan.cn

[S57] C++：编译期常量
来源：http://pvk.jqgfzy.top

constexpr int N = 10;
来源：http://kjm.daxiang520.top

[S58] C++：命名空间
来源：http://pvr.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://tkq.jyoumei.cn

[S59] C++：静态断言
来源：http://urs.c1oappe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rgw.shanyushiyangkeji.top

[S60] C++：遍历并删除元素
来源：http://klq.chenlongwang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hqk.yueranfly.top

================================================================================
来源：http://sft.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hcl.fanxiaobao.xyz

================================================================================
来源：http://vyf.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://xly.hnxiangtu.top

println("Hello")
来源：http://rgf.mhx1999.top

[T02] Kotlin：变量
来源：http://iqn.epnwcf.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ock.zhengqikj.top

[T03] Kotlin：字符串模板
来源：http://gpg.aizwys.cn

"值: $b"
来源：http://umq.shuidangran.top

[T04] Kotlin：空安全
来源：http://jpa.smart0.xyz

val n: String? = null;  n?.length
来源：http://ghs.yj20258.top

[T05] Kotlin：when 表达式
来源：http://kyf.shzxlz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://phs.ybcxt.top

[T06] Kotlin：集合映射
来源：http://fuj.tianlin.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://zxg.daxiang520.top

[T07] Kotlin：集合过滤
来源：http://pzw.gaohongyu789.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://oei.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://qnn.chenzaomai.com

data class User(val name: String, val age: Int)
来源：http://ctn.cheryme.top

[T09] Kotlin：扩展函数
来源：http://rqo.jinqigufen.top

fun String.exclaim() = this + "!"
来源：http://tgu.yonumen.top

[T10] Kotlin：默认参数
来源：http://hvt.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hzj.dashuyun.cn

[T11] Kotlin：协程
来源：http://jhs.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://odb.tian-w.cn

[T12] Kotlin：解构声明
来源：http://ghm.quarkkingdee.top

val (a, b) = Pair(1, 2)
来源：http://tnh.nanxinkj.top

[T13] Kotlin：只读 Map
来源：http://xul.aibaodan.cn

val m = mapOf("a" to 1)
来源：http://fto.zhiwuduotai.top

[T14] Kotlin：循环
来源：http://fbd.dianchejie.cn

for (i in 1..10) println(i)
来源：http://kat.cucudq.cn

[T15] Kotlin：接口
来源：http://knc.sweek.top

interface Shape { fun area(): Double }
来源：http://ohr.dashuyun.cn

[T16] Swift：Hello World
来源：http://evp.xziqi.cn

print("Hello")
来源：http://oos.uphjek.com

[T17] Swift：变量与常量
来源：http://kfg.cdnleiting.top

var a = 1;  let b = 2
来源：http://cyf.ppjwa.cn

[T18] Swift：字符串插值
来源：http://axc.yonumen.top

"值: \(b)"
来源：http://xoa.shanyushiyangkeji.top

[T19] Swift：可选绑定
来源：http://ztd.cdnleiting.top

if let n = opt { print(n) }
来源：http://umj.zdbjq.cn

[T20] Swift：数组操作
来源：http://nbd.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://kzj.sysykeji.top

[T21] Swift：遍历
来源：http://uuk.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://cvf.chenjidiqi.icu

[T22] Swift：字典
来源：http://jnn.mhx1999.top

var d = ["a": 1];  d["b"] = 2
来源：http://qbl.cqqwz.cn

[T23] Swift：函数
来源：http://lsk.jianghu66.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pzs.nanxinkj.top

[T24] Swift：闭包
来源：http://mzb.ydzc1.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hzk.smart0.xyz

[T25] Swift：结构体
来源：http://dwk.hesvh.cn

struct P { var x: Int }
来源：http://lyv.wangshuangyany.cn

[T26] Swift：类与重写
来源：http://vdw.yvedp.cn

class A: Base { override func f() {} }
来源：http://kqg.shanyushiyangtech.top

[T27] Swift：错误处理
来源：http://ytn.jqgfzy.top

do { try f() } catch { print(error) }
来源：http://wcc.jianghu66.top

[T28] Swift：枚举
来源：http://rjo.sysykeji.top

enum Color { case red, green }
来源：http://uxv.sweek.top

[T29] Swift：guard 提前返回
来源：http://jaw.daxiang520.top

guard let x = opt else { return }
来源：http://srw.ybcxt.top

[T30] Swift：协议
来源：http://aqy.ehwqpu.com

protocol Shape { func area() -> Double }
来源：http://iaf.iojbl.cn

[T31] Lua：Hello World
来源：http://zdq.uphjek.com

print("Hello")
来源：http://msf.hywenlv.cn

[T32] Lua：局部变量
来源：http://fih.9152youxi.cn

local a = 1
来源：http://ybv.chenjidiqi.icu

[T33] Lua：表（数组）
来源：http://usw.vqdsnc.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ibl.gotoacloud.top

[T34] Lua：遍历表
来源：http://vfw.aizwys.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://aoe.zhiwuduotai.top

[T35] Lua：字典表
来源：http://blj.haohaochexian.top

local d = { a = 1 };  d.b = 2
来源：http://fzg.jinyuanbaomall.cn

[T36] Lua：函数
来源：http://lxe.tianlin.xyz

function add(a, b) return a + b end
来源：http://upb.sjlbkw.cn

[T37] Lua：字符串拼接
来源：http://ofv.zdbjq.cn

"a" .. "b"
来源：http://ajl.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://vlj.ehwqpu.com

if x > 0 then print("正") end
来源：http://ijv.9152youxi.cn

[T39] Lua：模式匹配
来源：http://xof.sysykeji.top

string.find(s, "%d+")
来源：http://ole.ydzc1.top

[T40] Lua：元表
来源：http://qxf.yongpay.top

setmetatable({}, { __index = base })
来源：http://oem.sjlbkw.cn

[T41] Perl：Hello World
来源：http://eud.jinqigfzy.top

print "Hello\n";
来源：http://qej.mhx1999.top

[T42] Perl：变量类型
来源：http://caf.dianchejie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nvi.chenzaomai.com

[T43] Perl：字符串插值
来源：http://kpz.ivvv.top

"值: $a"
来源：http://fnt.fzhhl.top

[T44] Perl：条件
来源：http://qgw.c1oappe.top

if ($a > 0) { print "正"; }
来源：http://xjy.sweek.top

[T45] Perl：数组遍历
来源：http://vlq.smart0.xyz

for my $x (@arr) { print $x; }
来源：http://tzu.gzhubu.top

[T46] Perl：哈希操作
来源：http://vry.jianghu66.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ikq.zdbjq.cn

[T47] Perl：正则捕获
来源：http://xju.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://ixn.mhx1999.top

[T48] Perl：正则替换
来源：http://amx.gotoacloud.top

$s =~ s/old/new/g;
来源：http://cos.yueranfly.top

[T49] Perl：函数
来源：http://boo.mhx1999.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vtp.yongpay.top

[T50] Perl：逐行读文件
来源：http://bsy.nanxinkj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ozy.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://jpp.gaohongyu789.top

[T51] Scala：Hello World
来源：http://dal.hfpthk.cn

println("Hello")
来源：http://bnh.zhixingplan.top

[T52] Scala：变量
来源：http://fby.gogol.net.cn

val a = 1;  var b = 2
来源：http://ewv.fzhhl.top

[T53] Scala：字符串插值
来源：http://phg.jyoumei.cn

s"值: $b"
来源：http://wev.yj202588.top

[T54] Scala：集合映射
来源：http://hix.ybcxt.top

List(1, 2, 3).map(_ * 2)
来源：http://oiz.yanxiufei.cn

[T55] Scala：集合过滤
来源：http://hey.yangfankeji.com

List(1, 2, 3).filter(_ > 1)
来源：http://qqk.yfazqb.com

[T56] Scala：样例类
来源：http://mgc.bbcook.cn

case class User(name: String, age: Int)
来源：http://uds.cheryme.top

[T57] Scala：模式匹配
来源：http://rrf.sjlbkw.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ytu.yj20258.top

[T58] Scala：函数定义
来源：http://lpr.gotoacloud.top

def add(a: Int, b: Int): Int = a + b
来源：http://kie.52xcode.cn

[T59] Scala：循环
来源：http://nfy.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://ngz.cashguo.top

[T60] Scala：折叠
来源：http://dgk.hnqzz.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cju.zhixingplan.top

================================================================================
来源：http://yqd.andypj.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fbm.zdqjudy.top

================================================================================
来源：http://pme.pengpengdd.cyou

[U01] Py：创建虚拟环境
来源：http://msh.pengpengdd.cyou

python -m venv .venv && source .venv/bin/activate
来源：http://nzp.52xcode.cn

[U02] Py：导出 / 安装依赖
来源：http://uux.gzhubu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bnz.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://vci.zhoulong.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://apc.0kj1m.cn

[U04] Py：变量调试打印
来源：http://ihs.yonumen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zht.smart0.xyz

[U05] Py：列表去重且保序
来源：http://ohz.cqqwz.cn

list(dict.fromkeys(arr))
来源：http://ybn.vqdsnc.cn

[U06] Py：合并两个字典
来源：http://kno.jlsjyb.cn

{**a, **b}
来源：http://rdg.zdbjq.cn

[U07] Py：反转字典键值
来源：http://lll.yueranfly.top

{v: k for k, v in d.items()}
来源：http://mkw.fanxiaobao.xyz

[U08] Py：展平二维列表
来源：http://ndq.yangfankeji.com

[y for x in nested for y in x]
来源：http://oji.ydjk.org.cn

[U09] Py：字典取最大值的键
来源：http://hjs.sxryk.cn

max(d, key=d.get)
来源：http://upx.zhixingplan.top

[U10] Py：按值排序字典
来源：http://hrw.9152youxi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hrw.quarkkingdee.top

[U11] Py：生成器表达式
来源：http://qdb.jinghuilouyu.cn

(x * 2 for x in arr)
来源：http://dwh.chenjidiqi.icu

[U12] Py：取出现最多的 3 个元素
来源：http://lbs.shzxlz.cn

Counter(arr).most_common(3)
来源：http://tqv.ppjwa.cn

[U13] Py：固定长度队列
来源：http://icy.yvedp.cn

deque(maxlen=10)
来源：http://nen.zhijiandao.cn

[U14] Py：分组收集到列表
来源：http://nao.hfpthk.cn

defaultdict(list)
来源：http://mud.havefunace.top

[U15] Py：高精度计时
来源：http://llu.daria6918.cn

t = time.perf_counter()
来源：http://fmt.xingfuxueyuan.xyz

[U16] Py：命令行参数解析
来源：http://dzb.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aqz.ehwqpu.com

[U17] Py：初始化日志
来源：http://xow.feifeiyinyue.top

logging.basicConfig(level=logging.INFO)
来源：http://hhm.bbcook.cn

[U18] Py：预编译正则
来源：http://gos.sxryk.cn

pat = re.compile(r"\d+")
来源：http://lbt.feifeiyinyue.top

[U19] Py：正则替换带回调
来源：http://fud.mhx1999.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kvr.zhaomingkeji.xyz

[U20] Py：缓存函数结果
来源：http://vfc.jyoumei.cn

@functools.lru_cache(maxsize=None)
来源：http://ltc.zhaomingkeji.xyz

[U21] Py：自定义上下文管理器
来源：http://pcv.yj20258.top

@contextlib.contextmanager
来源：http://ibo.jlsjyb.cn

[U22] Py：矩阵转置
来源：http://ykl.hywenlv.cn

list(zip(*m))
来源：http://qoq.tarul.cn

[U23] Py：分块读取大文件
来源：http://rtw.zhoulong.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xdm.yangfankeji.com

[U24] Py：路径操作
来源：http://zgf.zhijiandao.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hdm.nanxinkj.top

[U25] Py：CSV 按字典读
来源：http://qwi.jlsjyb.cn

csv.DictReader(f)
来源：http://oqe.yangfankeji.com

[U26] Py：并发下载
来源：http://vme.kuanghao11.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sgl.yfazqb.com

[U27] Py：异步 HTTP
来源：http://kcp.zhongyouzk.top

aiohttp.ClientSession() 配合 async with
来源：http://szf.shuidangran.top

[U28] Py：类型别名
来源：http://chk.ehwqpu.com

UserId = int
来源：http://gqx.vehdjk.com

[U29] Py：属性校验
来源：http://cmw.chenjidiqi.icu

@property 与 @x.setter 配合
来源：http://dyu.zhiwuduotai.top

[U30] Py：数据类
来源：http://bwq.cdnleiting.top

@dataclass(slots=True)
来源：http://anf.hammf.cn

[U31] Py：单测
来源：http://dhk.redwolf501.top

python -m pytest -q
来源：http://tfn.xuanzx.com

[U32] Py：代码格式化
来源：http://ghi.jinqigfzy.top

ruff format . && ruff check --fix .
来源：http://imr.0kj1m.cn

[U33] Py：打包发布
来源：http://fox.aibaodan.cn

python -m build  （依赖 pyproject.toml）
来源：http://ypq.nanxinkj.top

[U34] Py：判断编码
来源：http://khl.ppjwa.cn

chardet.detect(raw)
来源：http://dkp.guannengcc.top

[U35] Py：发送邮件
来源：http://gfv.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jfa.nanxuanxn.top

[U36] Py：定时任务
来源：http://jvf.tianlin.xyz

schedule.every(10).minutes.do(job)
来源：http://lmo.jianghu66.top

[U37] Py：读写 Excel
来源：http://nbe.yfazqb.com

pandas.read_excel / DataFrame.to_excel
来源：http://nvw.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://zcr.shanyushiyangkeji.top

Path(__file__).resolve().parent
来源：http://rjr.tian-w.cn

[U39] Py：判断是否在交互环境
来源：http://jyz.ywan-chungtsiang.top

sys.stdout.isatty()
来源：http://qdo.zhiwuduotai.top

[U40] Py：打印到标准错误
来源：http://zuc.xinyue.icu

print("err", file=sys.stderr)
来源：http://wus.tanke756.top

[U41] PHP：初始化 Composer 项目
来源：http://yzk.sufxvd.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://txu.ivvv.top

[U42] PHP：PSR-4 自动加载
来源：http://orp.yanxiufei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vli.c1oappe.top

[U43] PHP：声明命名空间
来源：http://wio.sjlbkw.cn

namespace App\Http;
来源：http://cnc.xylfe.cn

[U44] PHP：开启严格类型
来源：http://aul.yfazqb.com

declare(strict_types=1);
来源：http://sxd.shuidangran.top

[U45] PHP：类型声明与返回类型
来源：http://umx.jiagoushi.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jnx.yj20258.top

[U46] PHP：可空类型
来源：http://wqh.gaohongyu789.top

?string $name = null
来源：http://jva.dianchejie.cn

[U47] PHP：联合类型
来源：http://xzi.dianchejie.cn

int|string $id
来源：http://oxm.xuetiantiany.cn

[U48] PHP：纯枚举
来源：http://xfv.9152youxi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xqd.tanke756.top

[U49] PHP：只读属性
来源：http://sem.jinqigufen.top

public readonly string $name
来源：http://hjz.ybcxt.top

[U50] PHP：构造器属性提升
来源：http://crl.wangdashe.top

public function __construct(private int $id) {}
来源：http://ofg.chenjidiqi.icu

[U51] PHP：数组解构
来源：http://vjj.chenlongwang.top

[$a, $b] = $arr;
来源：http://nym.pengpengdd.cyou

[U52] PHP：箭头函数
来源：http://hil.wangdashe.top

$double = fn($x) => $x * 2;
来源：http://vlj.xuetiantiany.cn


<!-- 参考信息 -->