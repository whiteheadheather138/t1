代发 wailian999

#ifndef X_H
来源：http://boz.quarkkingdee.top

#define X_H
来源：http://eyb.cqqwz.cn

#endif
来源：http://yyx.xylfe.cn

[S31] C++：Hello World
来源：http://aug.cdnleiting.top

#include <iostream>
来源：http://wdm.52xcode.cn

int main() { std::cout << "Hello\n"; }
来源：http://aga.shanyushiyangtech.top

[S32] C++：字符串
来源：http://xjg.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://chz.tarul.cn

[S33] C++：vector 增删
来源：http://mfe.ehwqpu.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ipf.xziqi.cn

[S34] C++：遍历 vector
来源：http://hcl.feifeiyinyue.top

for (auto &x : v) { std::cout << x; }
来源：http://rdu.fanxiaobao.xyz

[S35] C++：map
来源：http://vzv.sufxvd.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ggc.jiagoushi.top

[S36] C++：unordered_map
来源：http://mep.birdmap.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://slc.chenlongwang.top

[S37] C++：set
来源：http://rff.aibaodan.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://frj.xinyue.icu

[S38] C++：排序
来源：http://wbi.nanxuanxn.top

std::sort(v.begin(), v.end());
来源：http://sfx.yuanzhike.top

[S39] C++：自定义比较器排序
来源：http://qci.zhengqikj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rex.ctjpmb.com

[S40] C++：查找元素
来源：http://hxv.fktsv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://slt.kuanghao11.cn

[S41] C++：类与构造函数
来源：http://dgo.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ehb.meibo888.top

[S42] C++：继承与虚函数
来源：http://asd.jinqigufen.top

class B : public Base { public: void f() override {} };
来源：http://sas.hywenlv.cn

[S43] C++：智能指针
来源：http://ajh.guannengcc.top

auto p = std::make_unique<int>(5);
来源：http://oxs.nanxuanxn.top

[S44] C++：引用传参
来源：http://nnx.aizwys.cn

void inc(int &x) { ++x; }
来源：http://smc.zycfv.cn

[S45] C++：lambda
来源：http://mtr.shanyushiyangtech.top

auto add = [](int a, int b) { return a + b; };
来源：http://aii.ppjwa.cn

[S46] C++：函数模板
来源：http://xnk.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://akw.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://tpf.jlsjyb.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tab.yanxiufei.cn

[S48] C++：逐行读文件
来源：http://ndf.wangdashe.top

std::ifstream in("a.txt");  std::string line;
来源：http://qlx.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://adi.cucudq.cn

[S49] C++：写文件
来源：http://hsq.zhaomingkeji.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qnt.svipenyu.cn

[S50] C++：格式化数字
来源：http://zwu.sufxvd.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ewh.c1oappe.top

[S51] C++：显式类型转换
来源：http://njl.gzhubu.top

static_cast<double>(a) / b
来源：http://vgm.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://pii.chenlongwang.top

int size() const noexcept { return n_; }
来源：http://wnj.daria6918.cn

[S53] C++：移动语义
来源：http://qct.ivvv.top

std::vector<int> w = std::move(v);
来源：http://oco.feifeiyinyue.top

[S54] C++：异常处理
来源：http://efg.shuidangran.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xwo.ehwqpu.com

[S55] C++：结构化绑定
来源：http://vlj.nanxuanxn.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ehz.tanke756.top

[S56] C++：optional
来源：http://cvt.quarkkingdee.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ydy.zhixingplan.top

[S57] C++：编译期常量
来源：http://wqq.hongshengwenyu.top

constexpr int N = 10;
来源：http://jfq.tanke756.top

[S58] C++：命名空间
来源：http://dqc.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://stu.zhixingplan.top

[S59] C++：静态断言
来源：http://vru.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cyx.quarkkingdee.top

[S60] C++：遍历并删除元素
来源：http://ifz.tian-w.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bzz.nanxinkj.top

================================================================================
来源：http://hdg.andypj.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rnq.zhiwuduotai.top

================================================================================
来源：http://ctv.tianlin.xyz

[T01] Kotlin：Hello World
来源：http://gym.jqgfzy.top

println("Hello")
来源：http://wts.shuidangran.top

[T02] Kotlin：变量
来源：http://rcf.hcnkem.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jlt.ydjk.org.cn

[T03] Kotlin：字符串模板
来源：http://wqx.chenjidiqi.icu

"值: $b"
来源：http://syq.jinyuanbaomall.cn

[T04] Kotlin：空安全
来源：http://eje.vqdsnc.cn

val n: String? = null;  n?.length
来源：http://iaz.aibaodan.cn

[T05] Kotlin：when 表达式
来源：http://ygb.shanyushiyangtech.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jrd.nanxinkj.top

[T06] Kotlin：集合映射
来源：http://kof.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mee.jqgufenzy.top

[T07] Kotlin：集合过滤
来源：http://pfw.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sig.shuidangran.top

[T08] Kotlin：数据类
来源：http://hzr.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://qnh.smart0.xyz

[T09] Kotlin：扩展函数
来源：http://usv.tarul.cn

fun String.exclaim() = this + "!"
来源：http://phy.andypj.xyz

[T10] Kotlin：默认参数
来源：http://xlv.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kzz.bjfxy.top

[T11] Kotlin：协程
来源：http://gqp.nanxuanxn.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jah.0kj1m.cn

[T12] Kotlin：解构声明
来源：http://ykp.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://yup.cqqwz.cn

[T13] Kotlin：只读 Map
来源：http://awq.hesvh.cn

val m = mapOf("a" to 1)
来源：http://gcv.daxiang520.top

[T14] Kotlin：循环
来源：http://jwc.hnqzz.top

for (i in 1..10) println(i)
来源：http://hlm.zhixingplan.top

[T15] Kotlin：接口
来源：http://dsd.daria6918.cn

interface Shape { fun area(): Double }
来源：http://svp.yanxiufei.cn

[T16] Swift：Hello World
来源：http://goh.feifeiyinyue.top

print("Hello")
来源：http://nuh.feifeiyinyue.top

[T17] Swift：变量与常量
来源：http://qaj.jinghuilouyu.cn

var a = 1;  let b = 2
来源：http://ewp.yuanzhike.top

[T18] Swift：字符串插值
来源：http://izi.jinyuanbaomall.cn

"值: \(b)"
来源：http://ldu.nanxuanxn.top

[T19] Swift：可选绑定
来源：http://fzw.yueranfly.top

if let n = opt { print(n) }
来源：http://mrv.iojbl.cn

[T20] Swift：数组操作
来源：http://mma.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jar.wangdashe.top

[T21] Swift：遍历
来源：http://pkp.nanxinkj.top

for x in a { print(x) }
来源：http://yxm.yangfankeji.com

[T22] Swift：字典
来源：http://mls.zhixingplan.top

var d = ["a": 1];  d["b"] = 2
来源：http://ece.jiagoushi.top

[T23] Swift：函数
来源：http://vbk.ctjpmb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jfj.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://vcq.haohaochexian.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rjs.fktsv.cn

[T25] Swift：结构体
来源：http://uvk.shanyushiyangkeji.top

struct P { var x: Int }
来源：http://tjx.hesvh.cn

[T26] Swift：类与重写
来源：http://btl.tanke756.top

class A: Base { override func f() {} }
来源：http://kso.haohaochexian.top

[T27] Swift：错误处理
来源：http://ocl.zdbjq.cn

do { try f() } catch { print(error) }
来源：http://gvl.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://ior.daxiang520.top

enum Color { case red, green }
来源：http://kli.ppjwa.cn

[T29] Swift：guard 提前返回
来源：http://voc.pycfn.com

guard let x = opt else { return }
来源：http://agz.shangyingyoupin.top

[T30] Swift：协议
来源：http://rrj.aibaodan.cn

protocol Shape { func area() -> Double }
来源：http://wzt.hnqzz.top

[T31] Lua：Hello World
来源：http://zqq.quarkkingdee.top

print("Hello")
来源：http://hgk.zdqjudy.top

[T32] Lua：局部变量
来源：http://dax.hfpthk.cn

local a = 1
来源：http://iud.sjlbkw.cn

[T33] Lua：表（数组）
来源：http://win.yonumen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cdb.yvedp.cn

[T34] Lua：遍历表
来源：http://qtc.shzxlz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vnu.zhijiandao.cn

[T35] Lua：字典表
来源：http://ykw.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://akh.yvedp.cn

[T36] Lua：函数
来源：http://cik.hcnkem.com

function add(a, b) return a + b end
来源：http://baa.zdbjq.cn

[T37] Lua：字符串拼接
来源：http://vzi.vqdsnc.cn

"a" .. "b"
来源：http://hnt.cheryme.top

[T38] Lua：条件
来源：http://ykr.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://ixl.jinghuilouyu.cn

[T39] Lua：模式匹配
来源：http://onk.yueranfly.top

string.find(s, "%d+")
来源：http://ufp.jqgfzy.top

[T40] Lua：元表
来源：http://lno.jyoumei.cn

setmetatable({}, { __index = base })
来源：http://lgf.daxiang520.top

[T41] Perl：Hello World
来源：http://taj.hnxiangtu.top

print "Hello\n";
来源：http://kye.jianghu66.top

[T42] Perl：变量类型
来源：http://mib.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qeu.daxiang520.top

[T43] Perl：字符串插值
来源：http://grf.pengpengdd.cyou

"值: $a"
来源：http://goo.hysaishi.cn

[T44] Perl：条件
来源：http://agn.havefunace.top

if ($a > 0) { print "正"; }
来源：http://uls.gzhubu.top

[T45] Perl：数组遍历
来源：http://akd.jinghuilouyu.cn

for my $x (@arr) { print $x; }
来源：http://khz.cqqwz.cn

[T46] Perl：哈希操作
来源：http://usg.shanyushiyangtech.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://omd.ivvv.top

[T47] Perl：正则捕获
来源：http://okr.ehwqpu.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://eun.zhongyouzk.top

[T48] Perl：正则替换
来源：http://iit.iojbl.cn

$s =~ s/old/new/g;
来源：http://mhv.yanxiufei.cn

[T49] Perl：函数
来源：http://anb.gzhubu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://flq.nanxinkj.top

[T50] Perl：逐行读文件
来源：http://qhg.haohaochexian.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pqf.yongpay.top

while (my $line = <$fh>) { print $line; }
来源：http://fff.meibo888.top

[T51] Scala：Hello World
来源：http://xev.shanyushiyangkeji.top

println("Hello")
来源：http://ftp.tianlin.xyz

[T52] Scala：变量
来源：http://tjh.jinqigfzy.top

val a = 1;  var b = 2
来源：http://rrm.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://lfl.ppjwa.cn

s"值: $b"
来源：http://hmq.hysaishi.cn

[T54] Scala：集合映射
来源：http://tvg.9152youxi.cn

List(1, 2, 3).map(_ * 2)
来源：http://dyq.redwolf501.top

[T55] Scala：集合过滤
来源：http://nhg.zhengqikj.top

List(1, 2, 3).filter(_ > 1)
来源：http://dbz.jyoumei.cn

[T56] Scala：样例类
来源：http://mwi.dashuyun.cn

case class User(name: String, age: Int)
来源：http://vor.havefunace.top

[T57] Scala：模式匹配
来源：http://exc.havefunace.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ves.316326.xyz

[T58] Scala：函数定义
来源：http://fmm.fehbvm.com

def add(a: Int, b: Int): Int = a + b
来源：http://kuz.bbcook.cn

[T59] Scala：循环
来源：http://beq.hongshengwenyu.top

for (i <- 1 to 10) println(i)
来源：http://bts.cheryme.top

[T60] Scala：折叠
来源：http://cad.hnxiangtu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vbi.9152youxi.cn

================================================================================
来源：http://tng.nanxuanxn.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jqx.zhixingplan.top

================================================================================
来源：http://aeg.tanke756.top

[U01] Py：创建虚拟环境
来源：http://tww.dianchejie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zjh.tianlin.xyz

[U02] Py：导出 / 安装依赖
来源：http://kvf.nanxuanxn.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nst.shanyushiyangtech.top

[U03] Py：加载 .env 配置
来源：http://xzl.hnxiangtu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jzi.hnxiangtu.top

[U04] Py：变量调试打印
来源：http://kzv.feifeiyinyue.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uzi.nanxuanxn.top

[U05] Py：列表去重且保序
来源：http://xxl.c1oappe.top

list(dict.fromkeys(arr))
来源：http://rco.zhongyouzk.top

[U06] Py：合并两个字典
来源：http://ekj.iojbl.cn

{**a, **b}
来源：http://akh.daria6918.cn

[U07] Py：反转字典键值
来源：http://loo.havefunace.top

{v: k for k, v in d.items()}
来源：http://nsj.yueranfly.top

[U08] Py：展平二维列表
来源：http://blh.tanke756.top

[y for x in nested for y in x]
来源：http://cib.sufxvd.cn

[U09] Py：字典取最大值的键
来源：http://nln.tarul.cn

max(d, key=d.get)
来源：http://sog.ehwqpu.com

[U10] Py：按值排序字典
来源：http://str.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cfi.jinqigfzy.top

[U11] Py：生成器表达式
来源：http://keq.jqgfzy.top

(x * 2 for x in arr)
来源：http://ctd.zhongyouzk.top

[U12] Py：取出现最多的 3 个元素
来源：http://xoi.haohaochexian.top

Counter(arr).most_common(3)
来源：http://kaz.redwolf501.top

[U13] Py：固定长度队列
来源：http://los.ywan-chungtsiang.top

deque(maxlen=10)
来源：http://pnr.tanke756.top

[U14] Py：分组收集到列表
来源：http://rld.yangfankeji.com

defaultdict(list)
来源：http://xyh.yonumen.top

[U15] Py：高精度计时
来源：http://ist.yanxiufei.cn

t = time.perf_counter()
来源：http://eyv.yj20258888.top

[U16] Py：命令行参数解析
来源：http://mgo.aizwys.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://idn.guowangkeji.top

[U17] Py：初始化日志
来源：http://sle.cashguo.top

logging.basicConfig(level=logging.INFO)
来源：http://wzh.cdnleiting.top

[U18] Py：预编译正则
来源：http://zmo.epnwcf.com

pat = re.compile(r"\d+")
来源：http://unh.yanxiufei.cn

[U19] Py：正则替换带回调
来源：http://vqd.sweek.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jmf.jlsjyb.cn

[U20] Py：缓存函数结果
来源：http://cuy.zhoulong.xyz

@functools.lru_cache(maxsize=None)
来源：http://kpd.smart0.xyz

[U21] Py：自定义上下文管理器
来源：http://hkr.gaohongyu789.top

@contextlib.contextmanager
来源：http://pry.kuanghao11.cn

[U22] Py：矩阵转置
来源：http://nnw.bjfxy.top

list(zip(*m))
来源：http://pvh.shangyingyoupin.top

[U23] Py：分块读取大文件
来源：http://ttf.sysykeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gps.aizwys.cn

[U24] Py：路径操作
来源：http://fmh.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cub.jinyuanbaomall.cn

[U25] Py：CSV 按字典读
来源：http://jua.andypj.xyz

csv.DictReader(f)
来源：http://nrn.sufxvd.cn

[U26] Py：并发下载
来源：http://zgy.yj202588.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uvz.yongpay.top

[U27] Py：异步 HTTP
来源：http://ibj.hnxiangtu.top

aiohttp.ClientSession() 配合 async with
来源：http://zkh.sysykeji.top

[U28] Py：类型别名
来源：http://viz.gotoacloud.top

UserId = int
来源：http://cmd.epnwcf.com

[U29] Py：属性校验
来源：http://mly.tianlin.xyz

@property 与 @x.setter 配合
来源：http://hzi.sysykeji.top

[U30] Py：数据类
来源：http://aqu.ywan-chungtsiang.top

@dataclass(slots=True)
来源：http://kzx.wangdashe.top

[U31] Py：单测
来源：http://ypz.yonumen.top

python -m pytest -q
来源：http://wpb.nanxuanxn.top

[U32] Py：代码格式化
来源：http://iai.cdnleiting.top

ruff format . && ruff check --fix .
来源：http://pdn.cheryme.top

[U33] Py：打包发布
来源：http://hod.yonumen.top

python -m build  （依赖 pyproject.toml）
来源：http://kte.jinyuanbaomall.cn

[U34] Py：判断编码
来源：http://kqm.yj20258.top

chardet.detect(raw)
来源：http://tnu.shzxlz.cn

[U35] Py：发送邮件
来源：http://uat.gaohongyu789.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cpm.hesvh.cn

[U36] Py：定时任务
来源：http://mmm.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://ghh.shzxlz.cn

[U37] Py：读写 Excel
来源：http://rxu.zhiwuduotai.top

pandas.read_excel / DataFrame.to_excel
来源：http://aci.hnqzz.top

[U38] Py：获取脚本所在目录
来源：http://bio.redwolf501.top

Path(__file__).resolve().parent
来源：http://tio.zhaomingkeji.xyz

[U39] Py：判断是否在交互环境
来源：http://woi.yj202588.top

sys.stdout.isatty()
来源：http://yzp.sufxvd.cn

[U40] Py：打印到标准错误
来源：http://req.smart0.xyz

print("err", file=sys.stderr)
来源：http://vgl.zhijiandao.cn

[U41] PHP：初始化 Composer 项目
来源：http://myf.yvedp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mmm.jinghuilouyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://qdz.redwolf501.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xhe.cqqwz.cn

[U43] PHP：声明命名空间
来源：http://ddl.jqgufenzy.top

namespace App\Http;
来源：http://gpg.jyoumei.cn

[U44] PHP：开启严格类型
来源：http://jxd.sxryk.cn

declare(strict_types=1);
来源：http://flt.chenzaomai.com

[U45] PHP：类型声明与返回类型
来源：http://yry.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://flj.hesvh.cn

[U46] PHP：可空类型
来源：http://vcx.hysaishi.cn

?string $name = null
来源：http://avq.yueranfly.top

[U47] PHP：联合类型
来源：http://pjv.tianlin.xyz

int|string $id
来源：http://svp.guowangkeji.top

[U48] PHP：纯枚举
来源：http://nhz.gogol.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zev.hammf.cn

[U49] PHP：只读属性
来源：http://uuv.xingfuxueyuan.xyz

public readonly string $name
来源：http://gqo.kuanghao11.cn

[U50] PHP：构造器属性提升
来源：http://pwr.zhijiandao.cn

public function __construct(private int $id) {}
来源：http://lxh.zhoulong.xyz

[U51] PHP：数组解构
来源：http://emh.zhaomingkeji.xyz

[$a, $b] = $arr;
来源：http://crp.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://vgq.xinyue.icu

$double = fn($x) => $x * 2;
来源：http://lfw.zycfv.cn

[U53] PHP：空合并运算符
来源：http://ogw.cdnleiting.top

$v = $a ?? $b ?? "default";
来源：http://vxy.sufxvd.cn

[U54] PHP：空安全调用
来源：http://yvw.zhijiandao.cn

$obj?->method()
来源：http://mwr.tian-w.cn


<!-- 参考信息 -->