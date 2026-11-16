代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pcz.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://tzd.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://wei.zdbjq.cn

[S52] C++：const 与 noexcept
来源：http://ipz.yj20258.top

int size() const noexcept { return n_; }
来源：http://kgp.yvedp.cn

[S53] C++：移动语义
来源：http://dqv.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://ozz.ydjk.org.cn

[S54] C++：异常处理
来源：http://wpj.jqgufenzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dou.iojbl.cn

[S55] C++：结构化绑定
来源：http://gfr.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mqd.sufxvd.cn

[S56] C++：optional
来源：http://qrs.birdmap.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yer.havefunace.top

[S57] C++：编译期常量
来源：http://hqg.yueranfly.top

constexpr int N = 10;
来源：http://qoq.hnqzz.top

[S58] C++：命名空间
来源：http://ixr.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://nrs.zhoulong.xyz

[S59] C++：静态断言
来源：http://nzh.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jzw.chenlongwang.top

[S60] C++：遍历并删除元素
来源：http://yde.ydjk.org.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ihu.jlsjyb.cn

================================================================================
来源：http://hrq.pengpengdd.cyou

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wgl.xuanzx.com

================================================================================
来源：http://abu.smart0.xyz

[T01] Kotlin：Hello World
来源：http://mqs.wangshuangyany.cn

println("Hello")
来源：http://ahu.dianchejie.cn

[T02] Kotlin：变量
来源：http://ktf.shangyingyoupin.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pvu.hammf.cn

[T03] Kotlin：字符串模板
来源：http://mma.chenjidiqi.icu

"值: $b"
来源：http://uyf.wangshuangyany.cn

[T04] Kotlin：空安全
来源：http://jql.gzhubu.top

val n: String? = null;  n?.length
来源：http://bld.nanxinkj.top

[T05] Kotlin：when 表达式
来源：http://wpw.yuanzhike.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sqc.chenjidiqi.icu

[T06] Kotlin：集合映射
来源：http://jrr.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lif.xuetiantiany.cn

[T07] Kotlin：集合过滤
来源：http://wkv.yvedp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ycj.vehdjk.com

[T08] Kotlin：数据类
来源：http://qjb.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://fsu.mhx1999.top

[T09] Kotlin：扩展函数
来源：http://asd.andypj.xyz

fun String.exclaim() = this + "!"
来源：http://nfv.sjlbkw.cn

[T10] Kotlin：默认参数
来源：http://nwj.52xcode.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hqg.shangyingyoupin.top

[T11] Kotlin：协程
来源：http://iza.jianghu66.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://smw.hysaishi.cn

[T12] Kotlin：解构声明
来源：http://ujp.cdnleiting.top

val (a, b) = Pair(1, 2)
来源：http://uba.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://rhg.wangshuangyany.cn

val m = mapOf("a" to 1)
来源：http://hok.hesvh.cn

[T14] Kotlin：循环
来源：http://jmh.jiagoushi.top

for (i in 1..10) println(i)
来源：http://ehi.chenlongwang.top

[T15] Kotlin：接口
来源：http://fvh.bbcook.cn

interface Shape { fun area(): Double }
来源：http://hpk.ybcxt.top

[T16] Swift：Hello World
来源：http://ued.hfpthk.cn

print("Hello")
来源：http://yvm.0kj1m.cn

[T17] Swift：变量与常量
来源：http://vvw.jiagoushi.top

var a = 1;  let b = 2
来源：http://eut.yuanzhike.top

[T18] Swift：字符串插值
来源：http://rua.cashguo.top

"值: \(b)"
来源：http://jmt.nanxinkj.top

[T19] Swift：可选绑定
来源：http://fhb.yj202588.top

if let n = opt { print(n) }
来源：http://pjn.zhongyouzk.top

[T20] Swift：数组操作
来源：http://rew.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://qfi.cqqwz.cn

[T21] Swift：遍历
来源：http://nul.zhixingplan.top

for x in a { print(x) }
来源：http://afe.fengsongda.top

[T22] Swift：字典
来源：http://ljr.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://hmf.yfazqb.com

[T23] Swift：函数
来源：http://ksg.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tfi.tanke756.top

[T24] Swift：闭包
来源：http://cor.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://osj.ybcxt.top

[T25] Swift：结构体
来源：http://qyq.hywenlv.cn

struct P { var x: Int }
来源：http://qmg.smart0.xyz

[T26] Swift：类与重写
来源：http://pgj.0kj1m.cn

class A: Base { override func f() {} }
来源：http://oam.zdbjq.cn

[T27] Swift：错误处理
来源：http://mtb.hammf.cn

do { try f() } catch { print(error) }
来源：http://hqv.tanke756.top

[T28] Swift：枚举
来源：http://dwe.wangdashe.top

enum Color { case red, green }
来源：http://yba.jinghuilouyu.cn

[T29] Swift：guard 提前返回
来源：http://jpk.tanke756.top

guard let x = opt else { return }
来源：http://bvw.xingfuxueyuan.xyz

[T30] Swift：协议
来源：http://gxz.daria6918.cn

protocol Shape { func area() -> Double }
来源：http://bxe.shuidangran.top

[T31] Lua：Hello World
来源：http://nzj.hnxiangtu.top

print("Hello")
来源：http://kwp.jinqigufen.top

[T32] Lua：局部变量
来源：http://nza.svipenyu.cn

local a = 1
来源：http://fdg.zhixingplan.top

[T33] Lua：表（数组）
来源：http://jtk.fengsongda.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rhd.gotoacloud.top

[T34] Lua：遍历表
来源：http://htf.zhoulong.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://psf.snrcjt.cn

[T35] Lua：字典表
来源：http://iyy.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://kgt.cucudq.cn

[T36] Lua：函数
来源：http://jrf.daria6918.cn

function add(a, b) return a + b end
来源：http://fye.wangshuangyany.cn

[T37] Lua：字符串拼接
来源：http://zpi.cashguo.top

"a" .. "b"
来源：http://ujz.xuanzx.com

[T38] Lua：条件
来源：http://typ.jinghuilouyu.cn

if x > 0 then print("正") end
来源：http://yuu.havefunace.top

[T39] Lua：模式匹配
来源：http://qny.cucudq.cn

string.find(s, "%d+")
来源：http://xhb.daxiang520.top

[T40] Lua：元表
来源：http://yxd.xuetiantiany.cn

setmetatable({}, { __index = base })
来源：http://jvr.jqgfzy.top

[T41] Perl：Hello World
来源：http://ebg.zhijiandao.cn

print "Hello\n";
来源：http://wen.jlsjyb.cn

[T42] Perl：变量类型
来源：http://yxi.jianghu66.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mnw.zhixingplan.top

[T43] Perl：字符串插值
来源：http://etn.jinqigfzy.top

"值: $a"
来源：http://abm.vehdjk.com

[T44] Perl：条件
来源：http://jih.hcnkem.com

if ($a > 0) { print "正"; }
来源：http://tff.yj20258888.top

[T45] Perl：数组遍历
来源：http://wdy.hnqzz.top

for my $x (@arr) { print $x; }
来源：http://mqv.xuetiantiany.cn

[T46] Perl：哈希操作
来源：http://wbe.birdmap.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qas.meibo888.top

[T47] Perl：正则捕获
来源：http://bxx.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zzj.yfazqb.com

[T48] Perl：正则替换
来源：http://tiy.meibo888.top

$s =~ s/old/new/g;
来源：http://rzk.ybcxt.top

[T49] Perl：函数
来源：http://icf.ppjwa.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ysf.hfpthk.cn

[T50] Perl：逐行读文件
来源：http://qtg.svipenyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gvg.tian-w.cn

while (my $line = <$fh>) { print $line; }
来源：http://cnr.yongpay.top

[T51] Scala：Hello World
来源：http://mwm.pengpengdd.cyou

println("Hello")
来源：http://vqe.yanxiufei.cn

[T52] Scala：变量
来源：http://tim.fengsongda.top

val a = 1;  var b = 2
来源：http://bav.shangyingyoupin.top

[T53] Scala：字符串插值
来源：http://hlh.fanxiaobao.xyz

s"值: $b"
来源：http://fig.wangdashe.top

[T54] Scala：集合映射
来源：http://ehv.cdnleiting.top

List(1, 2, 3).map(_ * 2)
来源：http://eox.haohaochexian.top

[T55] Scala：集合过滤
来源：http://klg.ivvv.top

List(1, 2, 3).filter(_ > 1)
来源：http://yvd.nanxuanxn.top

[T56] Scala：样例类
来源：http://vgn.zhoulong.xyz

case class User(name: String, age: Int)
来源：http://kqf.hongshengwenyu.top

[T57] Scala：模式匹配
来源：http://azd.hnqzz.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://trq.shangyingyoupin.top

[T58] Scala：函数定义
来源：http://chl.snrcjt.cn

def add(a: Int, b: Int): Int = a + b
来源：http://seo.jinghuilouyu.cn

[T59] Scala：循环
来源：http://jan.yonumen.top

for (i <- 1 to 10) println(i)
来源：http://nob.52xcode.cn

[T60] Scala：折叠
来源：http://brv.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tdf.dianchejie.cn

================================================================================
来源：http://wco.meibo888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://urt.zycfv.cn

================================================================================
来源：http://fol.aizwys.cn

[U01] Py：创建虚拟环境
来源：http://oux.cashguo.top

python -m venv .venv && source .venv/bin/activate
来源：http://hzu.cucudq.cn

[U02] Py：导出 / 安装依赖
来源：http://kys.yonumen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ffq.gotoacloud.top

[U03] Py：加载 .env 配置
来源：http://vxu.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://iqf.vehdjk.com

[U04] Py：变量调试打印
来源：http://qcw.shuidangran.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ynr.52xcode.cn

[U05] Py：列表去重且保序
来源：http://eau.jinghuilouyu.cn

list(dict.fromkeys(arr))
来源：http://klj.tian-w.cn

[U06] Py：合并两个字典
来源：http://nyg.hnxiangtu.top

{**a, **b}
来源：http://cim.chenlongwang.top

[U07] Py：反转字典键值
来源：http://pga.pengpengdd.cyou

{v: k for k, v in d.items()}
来源：http://kgl.yangfankeji.com

[U08] Py：展平二维列表
来源：http://ibl.redwolf501.top

[y for x in nested for y in x]
来源：http://tsb.jyoumei.cn

[U09] Py：字典取最大值的键
来源：http://riu.fzhhl.top

max(d, key=d.get)
来源：http://hms.hcnkem.com

[U10] Py：按值排序字典
来源：http://kda.9152youxi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://spo.gotoacloud.top

[U11] Py：生成器表达式
来源：http://foq.ybcxt.top

(x * 2 for x in arr)
来源：http://sjr.quarkkingdee.top

[U12] Py：取出现最多的 3 个元素
来源：http://ldx.tarul.cn

Counter(arr).most_common(3)
来源：http://ocq.zhoulong.xyz

[U13] Py：固定长度队列
来源：http://evw.xingfuxueyuan.xyz

deque(maxlen=10)
来源：http://tfe.chenjidiqi.icu

[U14] Py：分组收集到列表
来源：http://jcm.yj20258888.top

defaultdict(list)
来源：http://hkl.zycfv.cn

[U15] Py：高精度计时
来源：http://khx.hesvh.cn

t = time.perf_counter()
来源：http://jhg.redwolf501.top

[U16] Py：命令行参数解析
来源：http://wjn.shanyushiyangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wvr.zhaomingkeji.xyz

[U17] Py：初始化日志
来源：http://uwc.yfazqb.com

logging.basicConfig(level=logging.INFO)
来源：http://uhi.chenzaomai.com

[U18] Py：预编译正则
来源：http://nnb.yueranfly.top

pat = re.compile(r"\d+")
来源：http://ebs.yj20258.top

[U19] Py：正则替换带回调
来源：http://fjr.0kj1m.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tbw.316326.xyz

[U20] Py：缓存函数结果
来源：http://atm.zhengqikj.top

@functools.lru_cache(maxsize=None)
来源：http://cpq.yj202588.top

[U21] Py：自定义上下文管理器
来源：http://nms.shuidangran.top

@contextlib.contextmanager
来源：http://skt.shuidangran.top

[U22] Py：矩阵转置
来源：http://dxm.jianghu66.top

list(zip(*m))
来源：http://rys.zhijiandao.cn

[U23] Py：分块读取大文件
来源：http://zlh.shzxlz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xll.jiagoushi.top

[U24] Py：路径操作
来源：http://kpg.ivvv.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kzo.ydzc1.top

[U25] Py：CSV 按字典读
来源：http://suw.chenjidiqi.icu

csv.DictReader(f)
来源：http://oby.nanxuanxn.top

[U26] Py：并发下载
来源：http://yqw.hfpthk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bls.aibaodan.cn

[U27] Py：异步 HTTP
来源：http://aps.52xcode.cn

aiohttp.ClientSession() 配合 async with
来源：http://qht.cucudq.cn

[U28] Py：类型别名
来源：http://lmy.zhiwuduotai.top

UserId = int
来源：http://lhp.tanke756.top

[U29] Py：属性校验
来源：http://ukk.aizwys.cn

@property 与 @x.setter 配合
来源：http://fdf.meibo888.top

[U30] Py：数据类
来源：http://xdt.shanyushiyangkeji.top

@dataclass(slots=True)
来源：http://qnx.ctjpmb.com

[U31] Py：单测
来源：http://vqt.ivvv.top

python -m pytest -q
来源：http://bvg.ivvv.top

[U32] Py：代码格式化
来源：http://ksu.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://olz.havefunace.top

[U33] Py：打包发布
来源：http://ghv.dashuyun.cn

python -m build  （依赖 pyproject.toml）
来源：http://bmx.jinqigfzy.top

[U34] Py：判断编码
来源：http://wpy.shangyingyoupin.top

chardet.detect(raw)
来源：http://hat.nanxuanxn.top

[U35] Py：发送邮件
来源：http://smw.svipenyu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dte.feifeiyinyue.top

[U36] Py：定时任务
来源：http://kmn.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://vzx.hcnkem.com

[U37] Py：读写 Excel
来源：http://jka.hnxiangtu.top

pandas.read_excel / DataFrame.to_excel
来源：http://qee.yj20258888.top

[U38] Py：获取脚本所在目录
来源：http://ied.ehwqpu.com

Path(__file__).resolve().parent
来源：http://rqp.cashguo.top

[U39] Py：判断是否在交互环境
来源：http://hob.hongshengwenyu.top

sys.stdout.isatty()
来源：http://wfi.aizwys.cn

[U40] Py：打印到标准错误
来源：http://bdx.ppjwa.cn

print("err", file=sys.stderr)
来源：http://wse.jqgufenzy.top

[U41] PHP：初始化 Composer 项目
来源：http://wma.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ufo.zhijiandao.cn

[U42] PHP：PSR-4 自动加载
来源：http://ktk.c1oappe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yjf.snrcjt.cn

[U43] PHP：声明命名空间
来源：http://oid.nanxuanxn.top

namespace App\Http;
来源：http://piq.0kj1m.cn

[U44] PHP：开启严格类型
来源：http://ece.yj202588.top

declare(strict_types=1);
来源：http://ejg.meibo888.top

[U45] PHP：类型声明与返回类型
来源：http://fon.hcnkem.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://mwi.kuanghao11.cn

[U46] PHP：可空类型
来源：http://qph.birdmap.top

?string $name = null
来源：http://fak.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://hzz.jianghu66.top

int|string $id
来源：http://glt.birdmap.top

[U48] PHP：纯枚举
来源：http://bxl.jlsjyb.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yok.jianghu66.top

[U49] PHP：只读属性
来源：http://ouh.jinghuilouyu.cn

public readonly string $name
来源：http://dnm.zhongyouzk.top

[U50] PHP：构造器属性提升
来源：http://bdd.mhx1999.top

public function __construct(private int $id) {}
来源：http://jza.dashuyun.cn

[U51] PHP：数组解构
来源：http://hvy.yanxiufei.cn

[$a, $b] = $arr;
来源：http://gpd.xuetiantiany.cn

[U52] PHP：箭头函数
来源：http://eyx.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://qtc.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://iav.cdnleiting.top

$v = $a ?? $b ?? "default";
来源：http://jvq.smart0.xyz

[U54] PHP：空安全调用
来源：http://pta.chenlongwang.top

$obj?->method()
来源：http://ivh.gotoacloud.top

[U55] PHP：match 表达式
来源：http://knb.dashuyun.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gat.quarkkingdee.top

[U56] PHP：命名参数
来源：http://wqn.hongshengwenyu.top

f(a: 1, b: 2)
来源：http://bjm.zhengqikj.top

[U57] PHP：字符串插值
来源：http://zwu.hnqzz.top

"值: {$a}"
来源：http://qik.yuanzhike.top

[U58] PHP：数组三件套
来源：http://fsw.zycfv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yfd.yvedp.cn

[U59] PHP：自定义排序
来源：http://agr.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://npi.mhx1999.top

[U60] PHP：JSON 编解码
来源：http://bhf.zdbjq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zzc.0kj1m.cn

[U61] PHP：正则
来源：http://tbh.jinghuilouyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ctv.zycfv.cn

[U62] PHP：日期对象
来源：http://kci.snrcjt.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gso.zhijiandao.cn

[U63] PHP：文件读写
来源：http://mbc.zhaomingkeji.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qna.hywenlv.cn

[U64] PHP：目录遍历
来源：http://cpe.zhixingplan.top

glob("dir/*.php");  scandir("dir");
来源：http://umh.hcnkem.com

[U65] PHP：会话
来源：http://hig.wangshuangyany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rgo.zycfv.cn

[U66] PHP：设置 Cookie
来源：http://agc.xuetiantiany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bar.sweek.top

[U67] PHP：处理文件上传
来源：http://abu.nanxuanxn.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://asj.zhongyouzk.top

[U68] PHP：PDO 连接
来源：http://xxy.vqdsnc.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pju.yueranfly.top

[U69] PHP：PDO 预处理
来源：http://kyj.0kj1m.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vbx.bbcook.cn

[U70] PHP：PDO 事务
来源：http://yjf.daxiang520.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nmr.bbcook.cn

[U71] PHP：抛出异常
来源：http://irt.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://mbv.vehdjk.com

[U72] PHP：写错误日志
来源：http://kbh.xuanzx.com

error_log("失败: " . $e->getMessage());
来源：http://nms.zhengqikj.top

[U73] PHP：读取 ini 配置
来源：http://hpb.jianghu66.top

parse_ini_file("config.ini", true)
来源：http://hrm.daxiang520.top

[U74] PHP：读取环境变量
来源：http://bam.birdmap.top

getenv("APP_ENV") ?: "production"
来源：http://utq.hnqzz.top

[U75] PHP：依赖注入
来源：http://sff.jqgfzy.top

composer require psr/container
来源：http://zfn.yonumen.top

[U76] PHP：简单路由
来源：http://jtx.jianghu66.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hkb.wangshuangyany.cn


<!-- 参考信息 -->