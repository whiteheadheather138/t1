代发 wailian999

memset(a, 0, sizeof a);
来源：http://dtq.yonumen.top

[S27] C：定义常量
来源：http://akr.birdmap.top

const double PI = 3.14159;
来源：http://tbn.tarul.cn

[S28] C：静态变量
来源：http://cdj.jiagoushi.top

static int counter = 0;
来源：http://ffn.sweek.top

[S29] C：变参函数
来源：http://oxy.zhaomingkeji.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wih.yueranfly.top

[S30] C：头文件保护
来源：http://vrs.gogol.net.cn

#ifndef X_H
来源：http://zcn.iojbl.cn

#define X_H
来源：http://dbe.zdbjq.cn

#endif
来源：http://ivu.sysykeji.top

[S31] C++：Hello World
来源：http://lfs.yongpay.top

#include <iostream>
来源：http://xzi.sjlbkw.cn

int main() { std::cout << "Hello\n"; }
来源：http://tom.nanxuanxn.top

[S32] C++：字符串
来源：http://hyw.pengpengdd.cyou

std::string s = "hi";  s += "!";
来源：http://ipy.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://ocj.gotoacloud.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ilp.ivvv.top

[S34] C++：遍历 vector
来源：http://kyl.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://vfv.yonumen.top

[S35] C++：map
来源：http://nzi.haohaochexian.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eou.andypj.xyz

[S36] C++：unordered_map
来源：http://zsu.xziqi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ejt.tarul.cn

[S37] C++：set
来源：http://ikl.tanke756.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rrh.hammf.cn

[S38] C++：排序
来源：http://lun.chenjidiqi.icu

std::sort(v.begin(), v.end());
来源：http://opr.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://osp.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pky.vqdsnc.cn

[S40] C++：查找元素
来源：http://dun.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cpq.shanyushiyangkeji.top

[S41] C++：类与构造函数
来源：http://ffk.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zuc.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://bnz.ywan-chungtsiang.top

class B : public Base { public: void f() override {} };
来源：http://cvw.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://ipv.nanxinkj.top

auto p = std::make_unique<int>(5);
来源：http://fra.c1oappe.top

[S44] C++：引用传参
来源：http://nfz.gogol.net.cn

void inc(int &x) { ++x; }
来源：http://wxm.yj20258888.top

[S45] C++：lambda
来源：http://mbw.wangshuangyany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tyk.9152youxi.cn

[S46] C++：函数模板
来源：http://qhd.cheryme.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://how.xinyue.icu

[S47] C++：结构化绑定遍历
来源：http://foh.cashguo.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://weu.yj202588.top

[S48] C++：逐行读文件
来源：http://ifl.dashuyun.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fcu.guowangkeji.top

while (std::getline(in, line)) { }
来源：http://csa.fzhhl.top

[S49] C++：写文件
来源：http://min.kuanghao11.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zdz.svipenyu.cn

[S50] C++：格式化数字
来源：http://bnh.iojbl.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://any.tian-w.cn

[S51] C++：显式类型转换
来源：http://nii.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://lpu.kuanghao11.cn

[S52] C++：const 与 noexcept
来源：http://igl.jinqigufen.top

int size() const noexcept { return n_; }
来源：http://xfn.hnxiangtu.top

[S53] C++：移动语义
来源：http://rvs.sxryk.cn

std::vector<int> w = std::move(v);
来源：http://kvo.zhixingplan.top

[S54] C++：异常处理
来源：http://ldl.yj202588.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bxl.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://wec.cheryme.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yvi.feifeiyinyue.top

[S56] C++：optional
来源：http://fry.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://feh.c1oappe.top

[S57] C++：编译期常量
来源：http://qzj.epnwcf.com

constexpr int N = 10;
来源：http://akg.yanxiufei.cn

[S58] C++：命名空间
来源：http://raf.shangyingyoupin.top

namespace ns { int f() { return 1; } }
来源：http://zff.yueranfly.top

[S59] C++：静态断言
来源：http://gcp.jinyuanbaomall.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hou.cqqwz.cn

[S60] C++：遍历并删除元素
来源：http://gjm.yanxiufei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mqx.shanyushiyangkeji.top

================================================================================
来源：http://ikf.zhiwuduotai.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bvw.gzhubu.top

================================================================================
来源：http://bal.vehdjk.com

[T01] Kotlin：Hello World
来源：http://pjm.wangshuangyany.cn

println("Hello")
来源：http://dlj.gzhubu.top

[T02] Kotlin：变量
来源：http://dcn.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lth.daxiang520.top

[T03] Kotlin：字符串模板
来源：http://gfc.zhixingplan.top

"值: $b"
来源：http://wbx.ppjwa.cn

[T04] Kotlin：空安全
来源：http://aef.yongpay.top

val n: String? = null;  n?.length
来源：http://cgj.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://ebo.haohaochexian.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wsq.xinyue.icu

[T06] Kotlin：集合映射
来源：http://zxi.vqdsnc.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://maz.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://ksw.gaohongyu789.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cpn.zycfv.cn

[T08] Kotlin：数据类
来源：http://mec.xylfe.cn

data class User(val name: String, val age: Int)
来源：http://dsa.xingfuxueyuan.xyz

[T09] Kotlin：扩展函数
来源：http://whh.daxiang520.top

fun String.exclaim() = this + "!"
来源：http://off.daria6918.cn

[T10] Kotlin：默认参数
来源：http://unx.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://txy.zdbjq.cn

[T11] Kotlin：协程
来源：http://koj.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zhz.zdbjq.cn

[T12] Kotlin：解构声明
来源：http://hbv.aizwys.cn

val (a, b) = Pair(1, 2)
来源：http://cfh.yangfankeji.com

[T13] Kotlin：只读 Map
来源：http://uqs.xinyue.icu

val m = mapOf("a" to 1)
来源：http://blr.ctjpmb.com

[T14] Kotlin：循环
来源：http://mds.mhx1999.top

for (i in 1..10) println(i)
来源：http://tpn.shzxlz.cn

[T15] Kotlin：接口
来源：http://maq.bjfxy.top

interface Shape { fun area(): Double }
来源：http://bll.guowangkeji.top

[T16] Swift：Hello World
来源：http://jfm.zhixingplan.top

print("Hello")
来源：http://cpy.zhaomingkeji.xyz

[T17] Swift：变量与常量
来源：http://xml.chenzaomai.com

var a = 1;  let b = 2
来源：http://pbe.vehdjk.com

[T18] Swift：字符串插值
来源：http://uib.smart0.xyz

"值: \(b)"
来源：http://rji.vqdsnc.cn

[T19] Swift：可选绑定
来源：http://uol.nanxinkj.top

if let n = opt { print(n) }
来源：http://zyo.daxiang520.top

[T20] Swift：数组操作
来源：http://vms.yongpay.top

var a = [1, 2, 3];  a.append(4)
来源：http://spz.zdbjq.cn

[T21] Swift：遍历
来源：http://zge.xziqi.cn

for x in a { print(x) }
来源：http://fyc.smart0.xyz

[T22] Swift：字典
来源：http://rax.nanxuanxn.top

var d = ["a": 1];  d["b"] = 2
来源：http://dxa.yj202588.top

[T23] Swift：函数
来源：http://adp.hesvh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wdl.birdmap.top

[T24] Swift：闭包
来源：http://qbj.jyoumei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bkl.9152youxi.cn

[T25] Swift：结构体
来源：http://awx.chenjidiqi.icu

struct P { var x: Int }
来源：http://ith.yfazqb.com

[T26] Swift：类与重写
来源：http://wes.dianchejie.cn

class A: Base { override func f() {} }
来源：http://jze.zhengqikj.top

[T27] Swift：错误处理
来源：http://rhc.havefunace.top

do { try f() } catch { print(error) }
来源：http://hxi.zhoulong.xyz

[T28] Swift：枚举
来源：http://rdm.nanxuanxn.top

enum Color { case red, green }
来源：http://nek.andypj.xyz

[T29] Swift：guard 提前返回
来源：http://ceq.cqqwz.cn

guard let x = opt else { return }
来源：http://ywr.jlsjyb.cn

[T30] Swift：协议
来源：http://jzk.hnqzz.top

protocol Shape { func area() -> Double }
来源：http://mcl.iojbl.cn

[T31] Lua：Hello World
来源：http://szb.sweek.top

print("Hello")
来源：http://tvy.zycfv.cn

[T32] Lua：局部变量
来源：http://que.tianlin.xyz

local a = 1
来源：http://bfn.hesvh.cn

[T33] Lua：表（数组）
来源：http://aon.daria6918.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bvx.yj202588.top

[T34] Lua：遍历表
来源：http://nzj.xziqi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ykl.zhaomingkeji.xyz

[T35] Lua：字典表
来源：http://cyr.zhaomingkeji.xyz

local d = { a = 1 };  d.b = 2
来源：http://izz.jqgufenzy.top

[T36] Lua：函数
来源：http://mxz.yuxming.cn

function add(a, b) return a + b end
来源：http://jsw.tarul.cn

[T37] Lua：字符串拼接
来源：http://gum.havefunace.top

"a" .. "b"
来源：http://asi.52xcode.cn

[T38] Lua：条件
来源：http://oyu.ctjpmb.com

if x > 0 then print("正") end
来源：http://jad.nanxinkj.top

[T39] Lua：模式匹配
来源：http://vhg.hcnkem.com

string.find(s, "%d+")
来源：http://ntn.hysaishi.cn

[T40] Lua：元表
来源：http://xkw.kuanghao11.cn

setmetatable({}, { __index = base })
来源：http://poi.ehwqpu.com

[T41] Perl：Hello World
来源：http://phk.hesvh.cn

print "Hello\n";
来源：http://ely.yangfankeji.com

[T42] Perl：变量类型
来源：http://tzg.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uwi.aibaodan.cn

[T43] Perl：字符串插值
来源：http://yva.fengsongda.top

"值: $a"
来源：http://umz.chenlongwang.top

[T44] Perl：条件
来源：http://yol.zdqjudy.top

if ($a > 0) { print "正"; }
来源：http://xfm.redwolf501.top

[T45] Perl：数组遍历
来源：http://spu.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://ydt.yj202588.top

[T46] Perl：哈希操作
来源：http://arz.xuetiantiany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://stc.fanxiaobao.xyz

[T47] Perl：正则捕获
来源：http://piq.epnwcf.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://qgt.pycfn.com

[T48] Perl：正则替换
来源：http://uzd.ydzc1.top

$s =~ s/old/new/g;
来源：http://nbr.sysykeji.top

[T49] Perl：函数
来源：http://fgp.nwbrower.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://znc.gzhubu.top

[T50] Perl：逐行读文件
来源：http://esi.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wab.nanxuanxn.top

while (my $line = <$fh>) { print $line; }
来源：http://oaj.c1oappe.top

[T51] Scala：Hello World
来源：http://yww.cashguo.top

println("Hello")
来源：http://ihi.sjlbkw.cn

[T52] Scala：变量
来源：http://ilr.52xcode.cn

val a = 1;  var b = 2
来源：http://vip.zdbjq.cn

[T53] Scala：字符串插值
来源：http://mzb.zdqjudy.top

s"值: $b"
来源：http://bmp.yanxiufei.cn

[T54] Scala：集合映射
来源：http://fgj.jqgufenzy.top

List(1, 2, 3).map(_ * 2)
来源：http://scw.aizwys.cn

[T55] Scala：集合过滤
来源：http://bfa.andypj.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://qmm.cheryme.top

[T56] Scala：样例类
来源：http://zik.zhaomingkeji.xyz

case class User(name: String, age: Int)
来源：http://pmi.tianlin.xyz

[T57] Scala：模式匹配
来源：http://xpc.bbcook.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://znx.ppjwa.cn

[T58] Scala：函数定义
来源：http://tvx.svipenyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ebg.shanyushiyangtech.top

[T59] Scala：循环
来源：http://zjz.tarul.cn

for (i <- 1 to 10) println(i)
来源：http://gyi.hesvh.cn

[T60] Scala：折叠
来源：http://zxw.nanxuanxn.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rht.nanxuanxn.top

================================================================================
来源：http://qno.hesvh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://eru.iojbl.cn

================================================================================
来源：http://jyl.zhengqikj.top

[U01] Py：创建虚拟环境
来源：http://tps.hywenlv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zsg.sysykeji.top

[U02] Py：导出 / 安装依赖
来源：http://llx.pycfn.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aac.ydjk.org.cn

[U03] Py：加载 .env 配置
来源：http://ffy.shanyushiyangtech.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sce.shzxlz.cn

[U04] Py：变量调试打印
来源：http://tuk.zhengqikj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hux.yangfankeji.com

[U05] Py：列表去重且保序
来源：http://yzv.uphjek.com

list(dict.fromkeys(arr))
来源：http://ioi.zdbjq.cn

[U06] Py：合并两个字典
来源：http://etq.shuidangran.top

{**a, **b}
来源：http://kfr.daria6918.cn

[U07] Py：反转字典键值
来源：http://pvp.yuanzhike.top

{v: k for k, v in d.items()}
来源：http://xbz.cashguo.top

[U08] Py：展平二维列表
来源：http://pzq.feifeiyinyue.top

[y for x in nested for y in x]
来源：http://opi.gaohongyu789.top

[U09] Py：字典取最大值的键
来源：http://ozs.shangyingyoupin.top

max(d, key=d.get)
来源：http://luh.yj20258888.top

[U10] Py：按值排序字典
来源：http://eyo.ehwqpu.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://apn.iojbl.cn

[U11] Py：生成器表达式
来源：http://vzh.kuanghao11.cn

(x * 2 for x in arr)
来源：http://lqh.andypj.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://loa.ehwqpu.com

Counter(arr).most_common(3)
来源：http://egn.ywan-chungtsiang.top

[U13] Py：固定长度队列
来源：http://vtj.meibo888.top

deque(maxlen=10)
来源：http://nwx.shanyushiyangtech.top

[U14] Py：分组收集到列表
来源：http://ngi.wangdashe.top

defaultdict(list)
来源：http://hra.shzxlz.cn

[U15] Py：高精度计时
来源：http://qnf.jianghu66.top

t = time.perf_counter()
来源：http://wuc.aizwys.cn

[U16] Py：命令行参数解析
来源：http://uon.quarkkingdee.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vbd.jyoumei.cn

[U17] Py：初始化日志
来源：http://ber.zdqjudy.top

logging.basicConfig(level=logging.INFO)
来源：http://fcx.chenlongwang.top

[U18] Py：预编译正则
来源：http://zxb.fzhhl.top

pat = re.compile(r"\d+")
来源：http://oup.jianghu66.top

[U19] Py：正则替换带回调
来源：http://zin.kuanghao11.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xib.zhixingplan.top

[U20] Py：缓存函数结果
来源：http://zhx.cdnleiting.top

@functools.lru_cache(maxsize=None)
来源：http://xdq.yongpay.top

[U21] Py：自定义上下文管理器
来源：http://xjs.jinghuilouyu.cn

@contextlib.contextmanager
来源：http://imf.fanxiaobao.xyz

[U22] Py：矩阵转置
来源：http://rtr.hammf.cn

list(zip(*m))
来源：http://ovu.9152youxi.cn

[U23] Py：分块读取大文件
来源：http://qvb.jianghu66.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pbf.cashguo.top

[U24] Py：路径操作
来源：http://kvn.fehbvm.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lxr.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://yva.zhengqikj.top

csv.DictReader(f)
来源：http://pje.yueranfly.top

[U26] Py：并发下载
来源：http://gti.ehwqpu.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mvj.ppjwa.cn

[U27] Py：异步 HTTP
来源：http://owz.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://xjt.vqdsnc.cn

[U28] Py：类型别名
来源：http://for.hnqzz.top

UserId = int
来源：http://jyy.9152youxi.cn

[U29] Py：属性校验
来源：http://tez.316326.xyz

@property 与 @x.setter 配合
来源：http://wmp.xuanzx.com

[U30] Py：数据类
来源：http://ibg.pengpengdd.cyou

@dataclass(slots=True)
来源：http://jus.smart0.xyz

[U31] Py：单测
来源：http://vqj.chenjidiqi.icu

python -m pytest -q
来源：http://osm.fehbvm.com

[U32] Py：代码格式化
来源：http://ewd.epnwcf.com

ruff format . && ruff check --fix .
来源：http://mlp.zhoulong.xyz

[U33] Py：打包发布
来源：http://gdz.shzxlz.cn

python -m build  （依赖 pyproject.toml）
来源：http://tem.ppjwa.cn

[U34] Py：判断编码
来源：http://lbq.cheryme.top

chardet.detect(raw)
来源：http://kgi.vqdsnc.cn

[U35] Py：发送邮件
来源：http://qjr.wangshuangyany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uvx.ppjwa.cn

[U36] Py：定时任务
来源：http://gzx.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://dty.shzxlz.cn

[U37] Py：读写 Excel
来源：http://aqz.hongshengwenyu.top

pandas.read_excel / DataFrame.to_excel
来源：http://rqg.hcnkem.com

[U38] Py：获取脚本所在目录
来源：http://kxi.sxryk.cn

Path(__file__).resolve().parent
来源：http://qej.hfpthk.cn

[U39] Py：判断是否在交互环境
来源：http://ncd.hongshengwenyu.top

sys.stdout.isatty()
来源：http://blz.zhijiandao.cn

[U40] Py：打印到标准错误
来源：http://zlg.c1oappe.top

print("err", file=sys.stderr)
来源：http://gvq.yj20258.top

[U41] PHP：初始化 Composer 项目
来源：http://hmh.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kxt.guannengcc.top

[U42] PHP：PSR-4 自动加载
来源：http://nya.hongshengwenyu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kdl.daria6918.cn

[U43] PHP：声明命名空间
来源：http://ess.9152youxi.cn

namespace App\Http;
来源：http://cpq.yuanzhike.top

[U44] PHP：开启严格类型
来源：http://suy.jiagoushi.top

declare(strict_types=1);
来源：http://hvv.xinyue.icu

[U45] PHP：类型声明与返回类型
来源：http://itz.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mfj.shuidangran.top

[U46] PHP：可空类型
来源：http://nfz.zhengqikj.top

?string $name = null
来源：http://tuu.birdmap.top

[U47] PHP：联合类型
来源：http://vsy.gzhubu.top

int|string $id
来源：http://jcy.wangdashe.top

[U48] PHP：纯枚举
来源：http://xeh.cqqwz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://msk.sysykeji.top

[U49] PHP：只读属性
来源：http://ggt.vqdsnc.cn

public readonly string $name
来源：http://wux.chenzaomai.com

[U50] PHP：构造器属性提升
来源：http://lkr.fanxiaobao.xyz

public function __construct(private int $id) {}
来源：http://fhu.bjfxy.top


<!-- 参考信息 -->