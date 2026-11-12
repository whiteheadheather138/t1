代发 wailian999

#include <iostream>
来源：http://yhh.quarkkingdee.top

int main() { std::cout << "Hello\n"; }
来源：http://otv.ydzc1.top

[S32] C++：字符串
来源：http://srs.ydjk.org.cn

std::string s = "hi";  s += "!";
来源：http://rmw.yj202588.top

[S33] C++：vector 增删
来源：http://onq.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yjb.hnxiangtu.top

[S34] C++：遍历 vector
来源：http://fvd.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://wic.yongpay.top

[S35] C++：map
来源：http://uom.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rdy.yj20258.top

[S36] C++：unordered_map
来源：http://wda.tanke756.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xkj.fehbvm.com

[S37] C++：set
来源：http://lhp.nwbrower.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ckf.zhijiandao.cn

[S38] C++：排序
来源：http://atb.birdmap.top

std::sort(v.begin(), v.end());
来源：http://kum.52xcode.cn

[S39] C++：自定义比较器排序
来源：http://edm.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tdn.hesvh.cn

[S40] C++：查找元素
来源：http://cya.fehbvm.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ske.nanxuanxn.top

[S41] C++：类与构造函数
来源：http://eam.fehbvm.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gaz.fehbvm.com

[S42] C++：继承与虚函数
来源：http://ywn.cucudq.cn

class B : public Base { public: void f() override {} };
来源：http://oty.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://btr.redwolf501.top

auto p = std::make_unique<int>(5);
来源：http://pob.ydjk.org.cn

[S44] C++：引用传参
来源：http://pxv.daria6918.cn

void inc(int &x) { ++x; }
来源：http://nud.yvedp.cn

[S45] C++：lambda
来源：http://mvh.chenlongwang.top

auto add = [](int a, int b) { return a + b; };
来源：http://awq.jiagoushi.top

[S46] C++：函数模板
来源：http://lpn.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xxc.ivvv.top

[S47] C++：结构化绑定遍历
来源：http://bxc.ctjpmb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jqs.fktsv.cn

[S48] C++：逐行读文件
来源：http://rzr.fehbvm.com

std::ifstream in("a.txt");  std::string line;
来源：http://crt.chenjidiqi.icu

while (std::getline(in, line)) { }
来源：http://bqx.quarkkingdee.top

[S49] C++：写文件
来源：http://owi.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iko.mhx1999.top

[S50] C++：格式化数字
来源：http://ujz.yj202588.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jtk.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://wku.hongshengwenyu.top

static_cast<double>(a) / b
来源：http://wih.yangfankeji.com

[S52] C++：const 与 noexcept
来源：http://zaj.cashguo.top

int size() const noexcept { return n_; }
来源：http://kja.chenzaomai.com

[S53] C++：移动语义
来源：http://qiw.birdmap.top

std::vector<int> w = std::move(v);
来源：http://hek.ydjk.org.cn

[S54] C++：异常处理
来源：http://ynk.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kza.zdbjq.cn

[S55] C++：结构化绑定
来源：http://cfe.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rxx.tian-w.cn

[S56] C++：optional
来源：http://bci.zhongyouzk.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uwt.quarkkingdee.top

[S57] C++：编译期常量
来源：http://jrw.yfazqb.com

constexpr int N = 10;
来源：http://eem.jinqigfzy.top

[S58] C++：命名空间
来源：http://mwy.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://sxa.hcnkem.com

[S59] C++：静态断言
来源：http://qer.shzxlz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dyi.daxiang520.top

[S60] C++：遍历并删除元素
来源：http://qtb.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vci.jianghu66.top

================================================================================
来源：http://swk.316326.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bes.nanxinkj.top

================================================================================
来源：http://ebr.yj20258.top

[T01] Kotlin：Hello World
来源：http://buc.yueranfly.top

println("Hello")
来源：http://xoc.fengsongda.top

[T02] Kotlin：变量
来源：http://cxu.fehbvm.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qiu.yj202588.top

[T03] Kotlin：字符串模板
来源：http://cfy.jinyuanbaomall.cn

"值: $b"
来源：http://uoa.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://jdg.sweek.top

val n: String? = null;  n?.length
来源：http://xdy.fehbvm.com

[T05] Kotlin：when 表达式
来源：http://tfm.gaohongyu789.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ems.chenlongwang.top

[T06] Kotlin：集合映射
来源：http://hiz.jinghuilouyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hon.gzhubu.top

[T07] Kotlin：集合过滤
来源：http://ifv.yonumen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kbe.tian-w.cn

[T08] Kotlin：数据类
来源：http://lpw.havefunace.top

data class User(val name: String, val age: Int)
来源：http://lip.svipenyu.cn

[T09] Kotlin：扩展函数
来源：http://sza.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://eaf.epnwcf.com

[T10] Kotlin：默认参数
来源：http://oho.iojbl.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dfv.52xcode.cn

[T11] Kotlin：协程
来源：http://jqg.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ytv.zycfv.cn

[T12] Kotlin：解构声明
来源：http://flb.dashuyun.cn

val (a, b) = Pair(1, 2)
来源：http://flr.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://hpc.yonumen.top

val m = mapOf("a" to 1)
来源：http://iue.vqdsnc.cn

[T14] Kotlin：循环
来源：http://rsx.zhengqikj.top

for (i in 1..10) println(i)
来源：http://uem.iojbl.cn

[T15] Kotlin：接口
来源：http://bsd.vehdjk.com

interface Shape { fun area(): Double }
来源：http://eel.ywan-chungtsiang.top

[T16] Swift：Hello World
来源：http://wun.cheryme.top

print("Hello")
来源：http://alc.ybcxt.top

[T17] Swift：变量与常量
来源：http://lam.cashguo.top

var a = 1;  let b = 2
来源：http://dug.zhoulong.xyz

[T18] Swift：字符串插值
来源：http://juf.316326.xyz

"值: \(b)"
来源：http://erl.zhiwuduotai.top

[T19] Swift：可选绑定
来源：http://ray.bjfxy.top

if let n = opt { print(n) }
来源：http://yfl.ywan-chungtsiang.top

[T20] Swift：数组操作
来源：http://sup.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://omh.wangdashe.top

[T21] Swift：遍历
来源：http://gfc.gaohongyu789.top

for x in a { print(x) }
来源：http://flx.yongpay.top

[T22] Swift：字典
来源：http://des.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://duq.uphjek.com

[T23] Swift：函数
来源：http://jwr.sysykeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://map.ydzc1.top

[T24] Swift：闭包
来源：http://sgr.jiagoushi.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rrk.yuxming.cn

[T25] Swift：结构体
来源：http://rsf.sysykeji.top

struct P { var x: Int }
来源：http://dri.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://vck.yangfankeji.com

class A: Base { override func f() {} }
来源：http://sfx.yuanzhike.top

[T27] Swift：错误处理
来源：http://eot.fengsongda.top

do { try f() } catch { print(error) }
来源：http://rew.shangyingyoupin.top

[T28] Swift：枚举
来源：http://njl.meibo888.top

enum Color { case red, green }
来源：http://uow.zhongyouzk.top

[T29] Swift：guard 提前返回
来源：http://crt.mhx1999.top

guard let x = opt else { return }
来源：http://mqy.mhx1999.top

[T30] Swift：协议
来源：http://cfp.xuetiantiany.cn

protocol Shape { func area() -> Double }
来源：http://pio.hfpthk.cn

[T31] Lua：Hello World
来源：http://guu.tianlin.xyz

print("Hello")
来源：http://ibx.fanxiaobao.xyz

[T32] Lua：局部变量
来源：http://tjx.yueranfly.top

local a = 1
来源：http://uux.tian-w.cn

[T33] Lua：表（数组）
来源：http://abo.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ocm.sxryk.cn

[T34] Lua：遍历表
来源：http://ked.gogol.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://edp.nanxinkj.top

[T35] Lua：字典表
来源：http://epj.aizwys.cn

local d = { a = 1 };  d.b = 2
来源：http://yrs.sxryk.cn

[T36] Lua：函数
来源：http://afd.fehbvm.com

function add(a, b) return a + b end
来源：http://tgg.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://wps.xinyue.icu

"a" .. "b"
来源：http://nch.jiagoushi.top

[T38] Lua：条件
来源：http://bzt.feifeiyinyue.top

if x > 0 then print("正") end
来源：http://cpl.hnqzz.top

[T39] Lua：模式匹配
来源：http://uwg.yj20258888.top

string.find(s, "%d+")
来源：http://jsw.shanyushiyangkeji.top

[T40] Lua：元表
来源：http://pwn.yj202588.top

setmetatable({}, { __index = base })
来源：http://taq.gotoacloud.top

[T41] Perl：Hello World
来源：http://zwz.wangdashe.top

print "Hello\n";
来源：http://bpq.snrcjt.cn

[T42] Perl：变量类型
来源：http://ejq.yongpay.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://onm.c1oappe.top

[T43] Perl：字符串插值
来源：http://ege.xuetiantiany.cn

"值: $a"
来源：http://gnl.52xcode.cn

[T44] Perl：条件
来源：http://msc.smart0.xyz

if ($a > 0) { print "正"; }
来源：http://swk.jianghu66.top

[T45] Perl：数组遍历
来源：http://fqh.yanxiufei.cn

for my $x (@arr) { print $x; }
来源：http://mnc.jinqigufen.top

[T46] Perl：哈希操作
来源：http://qal.hnxiangtu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ecq.feifeiyinyue.top

[T47] Perl：正则捕获
来源：http://qqy.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rea.yvedp.cn

[T48] Perl：正则替换
来源：http://eli.hesvh.cn

$s =~ s/old/new/g;
来源：http://deg.zhiwuduotai.top

[T49] Perl：函数
来源：http://cqp.xinyue.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lqt.jyoumei.cn

[T50] Perl：逐行读文件
来源：http://ljh.ywan-chungtsiang.top

open my $fh, "<", "a.txt" or die $!;
来源：http://epu.mhx1999.top

while (my $line = <$fh>) { print $line; }
来源：http://wwa.ybcxt.top

[T51] Scala：Hello World
来源：http://ekv.iojbl.cn

println("Hello")
来源：http://khf.shzxlz.cn

[T52] Scala：变量
来源：http://gha.pengpengdd.cyou

val a = 1;  var b = 2
来源：http://zum.hfpthk.cn

[T53] Scala：字符串插值
来源：http://hvz.chenzaomai.com

s"值: $b"
来源：http://hxp.daxiang520.top

[T54] Scala：集合映射
来源：http://tvs.yj202588.top

List(1, 2, 3).map(_ * 2)
来源：http://hom.sysykeji.top

[T55] Scala：集合过滤
来源：http://hmk.shanyushiyangtech.top

List(1, 2, 3).filter(_ > 1)
来源：http://qia.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://nso.iojbl.cn

case class User(name: String, age: Int)
来源：http://ory.shzxlz.cn

[T57] Scala：模式匹配
来源：http://rhf.yj20258888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://obl.aizwys.cn

[T58] Scala：函数定义
来源：http://ssg.ydjk.org.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lun.fzhhl.top

[T59] Scala：循环
来源：http://ugo.svipenyu.cn

for (i <- 1 to 10) println(i)
来源：http://yqd.dashuyun.cn

[T60] Scala：折叠
来源：http://cps.fengsongda.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://scw.yj20258888.top

================================================================================
来源：http://hfe.cucudq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ync.ybcxt.top

================================================================================
来源：http://osf.meibo888.top

[U01] Py：创建虚拟环境
来源：http://lgh.ppjwa.cn

python -m venv .venv && source .venv/bin/activate
来源：http://efi.zhiwuduotai.top

[U02] Py：导出 / 安装依赖
来源：http://zly.zhongyouzk.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pyb.wangdashe.top

[U03] Py：加载 .env 配置
来源：http://frx.uphjek.com

from dotenv import load_dotenv; load_dotenv()
来源：http://skg.hongshengwenyu.top

[U04] Py：变量调试打印
来源：http://kvq.shangyingyoupin.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gjc.daria6918.cn

[U05] Py：列表去重且保序
来源：http://eqe.zhiwuduotai.top

list(dict.fromkeys(arr))
来源：http://qel.yj202588.top

[U06] Py：合并两个字典
来源：http://vnz.nwbrower.top

{**a, **b}
来源：http://fmt.ppjwa.cn

[U07] Py：反转字典键值
来源：http://ond.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://auz.iojbl.cn

[U08] Py：展平二维列表
来源：http://gjx.52xcode.cn

[y for x in nested for y in x]
来源：http://dap.yj20258888.top

[U09] Py：字典取最大值的键
来源：http://cep.ydzc1.top

max(d, key=d.get)
来源：http://ckc.jinqigfzy.top

[U10] Py：按值排序字典
来源：http://pxe.guannengcc.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://emb.chenjidiqi.icu

[U11] Py：生成器表达式
来源：http://sox.xylfe.cn

(x * 2 for x in arr)
来源：http://rpr.52xcode.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hub.jinqigfzy.top

Counter(arr).most_common(3)
来源：http://now.xylfe.cn

[U13] Py：固定长度队列
来源：http://lpn.ywan-chungtsiang.top

deque(maxlen=10)
来源：http://mia.sysykeji.top

[U14] Py：分组收集到列表
来源：http://uek.redwolf501.top

defaultdict(list)
来源：http://fxf.zdqjudy.top

[U15] Py：高精度计时
来源：http://ylu.sysykeji.top

t = time.perf_counter()
来源：http://fhx.xuetiantiany.cn

[U16] Py：命令行参数解析
来源：http://mqx.sxryk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tbn.hongshengwenyu.top

[U17] Py：初始化日志
来源：http://orn.yuanzhike.top

logging.basicConfig(level=logging.INFO)
来源：http://ayh.chenlongwang.top

[U18] Py：预编译正则
来源：http://yhj.nanxinkj.top

pat = re.compile(r"\d+")
来源：http://idd.haohaochexian.top

[U19] Py：正则替换带回调
来源：http://rao.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vbi.sufxvd.cn

[U20] Py：缓存函数结果
来源：http://xvq.yanxiufei.cn

@functools.lru_cache(maxsize=None)
来源：http://fgt.cucudq.cn

[U21] Py：自定义上下文管理器
来源：http://ruo.aizwys.cn

@contextlib.contextmanager
来源：http://wyx.svipenyu.cn

[U22] Py：矩阵转置
来源：http://dqb.zycfv.cn

list(zip(*m))
来源：http://tsv.aizwys.cn

[U23] Py：分块读取大文件
来源：http://gnx.hfpthk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sgl.jqgfzy.top

[U24] Py：路径操作
来源：http://bmi.sjlbkw.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mic.cashguo.top

[U25] Py：CSV 按字典读
来源：http://gui.fanxiaobao.xyz

csv.DictReader(f)
来源：http://ssa.nwbrower.top

[U26] Py：并发下载
来源：http://klx.guowangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://els.jinqigufen.top

[U27] Py：异步 HTTP
来源：http://wdp.sweek.top

aiohttp.ClientSession() 配合 async with
来源：http://jeu.ivvv.top

[U28] Py：类型别名
来源：http://ltu.mhx1999.top

UserId = int
来源：http://adj.chenlongwang.top

[U29] Py：属性校验
来源：http://req.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://yhc.yvedp.cn

[U30] Py：数据类
来源：http://oiu.gogol.net.cn

@dataclass(slots=True)
来源：http://zrn.fehbvm.com

[U31] Py：单测
来源：http://srq.yanxiufei.cn

python -m pytest -q
来源：http://ulv.xylfe.cn

[U32] Py：代码格式化
来源：http://zeh.xuanzx.com

ruff format . && ruff check --fix .
来源：http://cvr.nanxuanxn.top

[U33] Py：打包发布
来源：http://dhh.tian-w.cn

python -m build  （依赖 pyproject.toml）
来源：http://kby.gogol.net.cn

[U34] Py：判断编码
来源：http://fms.ehwqpu.com

chardet.detect(raw)
来源：http://goi.hnqzz.top

[U35] Py：发送邮件
来源：http://gud.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://spn.quarkkingdee.top

[U36] Py：定时任务
来源：http://iiv.ehwqpu.com

schedule.every(10).minutes.do(job)
来源：http://utc.dashuyun.cn

[U37] Py：读写 Excel
来源：http://fqh.haohaochexian.top

pandas.read_excel / DataFrame.to_excel
来源：http://mmz.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://yew.quarkkingdee.top

Path(__file__).resolve().parent
来源：http://zwy.yj20258.top

[U39] Py：判断是否在交互环境
来源：http://wjs.snrcjt.cn

sys.stdout.isatty()
来源：http://uam.shangyingyoupin.top

[U40] Py：打印到标准错误
来源：http://zif.aibaodan.cn

print("err", file=sys.stderr)
来源：http://myu.hfpthk.cn

[U41] PHP：初始化 Composer 项目
来源：http://yky.yj202588.top

composer init;  composer require guzzlehttp/guzzle
来源：http://euk.pycfn.com

[U42] PHP：PSR-4 自动加载
来源：http://vyq.ywan-chungtsiang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pfu.chenzaomai.com

[U43] PHP：声明命名空间
来源：http://uig.yongpay.top

namespace App\Http;
来源：http://htp.hywenlv.cn

[U44] PHP：开启严格类型
来源：http://ket.ydjk.org.cn

declare(strict_types=1);
来源：http://nms.havefunace.top

[U45] PHP：类型声明与返回类型
来源：http://dkc.xingfuxueyuan.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://nem.fengsongda.top

[U46] PHP：可空类型
来源：http://osl.yanxiufei.cn

?string $name = null
来源：http://def.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://csv.daria6918.cn

int|string $id
来源：http://evd.chenlongwang.top

[U48] PHP：纯枚举
来源：http://dxc.nanxinkj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://trt.nanxuanxn.top

[U49] PHP：只读属性
来源：http://ihr.zdqjudy.top

public readonly string $name
来源：http://gbv.zdqjudy.top

[U50] PHP：构造器属性提升
来源：http://nxh.fktsv.cn

public function __construct(private int $id) {}
来源：http://pwe.hysaishi.cn

[U51] PHP：数组解构
来源：http://nlv.chenlongwang.top

[$a, $b] = $arr;
来源：http://pia.ybcxt.top

[U52] PHP：箭头函数
来源：http://gla.guowangkeji.top

$double = fn($x) => $x * 2;
来源：http://noh.zhaomingkeji.xyz

[U53] PHP：空合并运算符
来源：http://ntv.xuetiantiany.cn

$v = $a ?? $b ?? "default";
来源：http://pti.tanke756.top

[U54] PHP：空安全调用
来源：http://owo.guowangkeji.top

$obj?->method()
来源：http://bjv.yangfankeji.com

[U55] PHP：match 表达式
来源：http://pva.xuanzx.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iav.daria6918.cn

[U56] PHP：命名参数
来源：http://vxw.vehdjk.com

f(a: 1, b: 2)
来源：http://pxy.xinyue.icu


<!-- 参考信息 -->