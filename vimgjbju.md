代发 wailian999

int size() const noexcept { return n_; }
来源：http://ana.wangshuangyany.cn

[S53] C++：移动语义
来源：http://vap.ivvv.top

std::vector<int> w = std::move(v);
来源：http://crx.zhixingplan.top

[S54] C++：异常处理
来源：http://hmx.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lxb.jyoumei.cn

[S55] C++：结构化绑定
来源：http://sqx.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kyk.daxiang520.top

[S56] C++：optional
来源：http://evj.epnwcf.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://whu.fzhhl.top

[S57] C++：编译期常量
来源：http://fkx.cashguo.top

constexpr int N = 10;
来源：http://qyy.52xcode.cn

[S58] C++：命名空间
来源：http://tnu.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://zdh.wangshuangyany.cn

[S59] C++：静态断言
来源：http://fwj.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fik.hnqzz.top

[S60] C++：遍历并删除元素
来源：http://yrs.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sxu.ywan-chungtsiang.top

================================================================================
来源：http://aft.yfazqb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wzu.nanxinkj.top

================================================================================
来源：http://lns.ivvv.top

[T01] Kotlin：Hello World
来源：http://uwg.wangshuangyany.cn

println("Hello")
来源：http://fhy.daxiang520.top

[T02] Kotlin：变量
来源：http://vzm.hesvh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vms.tarul.cn

[T03] Kotlin：字符串模板
来源：http://nux.pycfn.com

"值: $b"
来源：http://xtw.aizwys.cn

[T04] Kotlin：空安全
来源：http://asx.pengpengdd.cyou

val n: String? = null;  n?.length
来源：http://tzi.ydzc1.top

[T05] Kotlin：when 表达式
来源：http://sze.shuidangran.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lcc.zhijiandao.cn

[T06] Kotlin：集合映射
来源：http://fwp.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fhf.sweek.top

[T07] Kotlin：集合过滤
来源：http://gov.cqqwz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wlb.fktsv.cn

[T08] Kotlin：数据类
来源：http://ynt.zhengqikj.top

data class User(val name: String, val age: Int)
来源：http://gms.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://uvw.c1oappe.top

fun String.exclaim() = this + "!"
来源：http://npr.yonumen.top

[T10] Kotlin：默认参数
来源：http://bqv.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tor.fehbvm.com

[T11] Kotlin：协程
来源：http://uag.sysykeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://djg.zhoulong.xyz

[T12] Kotlin：解构声明
来源：http://zsf.svipenyu.cn

val (a, b) = Pair(1, 2)
来源：http://gwh.jlsjyb.cn

[T13] Kotlin：只读 Map
来源：http://rtd.yuanzhike.top

val m = mapOf("a" to 1)
来源：http://bih.cucudq.cn

[T14] Kotlin：循环
来源：http://nqz.yueranfly.top

for (i in 1..10) println(i)
来源：http://dxi.hesvh.cn

[T15] Kotlin：接口
来源：http://owy.guowangkeji.top

interface Shape { fun area(): Double }
来源：http://lfi.0kj1m.cn

[T16] Swift：Hello World
来源：http://smq.meibo888.top

print("Hello")
来源：http://cnj.jlsjyb.cn

[T17] Swift：变量与常量
来源：http://mzx.zhongyouzk.top

var a = 1;  let b = 2
来源：http://ezj.zhaomingkeji.xyz

[T18] Swift：字符串插值
来源：http://tpn.nwbrower.top

"值: \(b)"
来源：http://rzt.hysaishi.cn

[T19] Swift：可选绑定
来源：http://olx.hnxiangtu.top

if let n = opt { print(n) }
来源：http://qht.gogol.net.cn

[T20] Swift：数组操作
来源：http://zjn.zhijiandao.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xcn.yj20258.top

[T21] Swift：遍历
来源：http://uri.hammf.cn

for x in a { print(x) }
来源：http://xmv.chenjidiqi.icu

[T22] Swift：字典
来源：http://wzy.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lsz.sxryk.cn

[T23] Swift：函数
来源：http://vhy.jiagoushi.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xfq.hammf.cn

[T24] Swift：闭包
来源：http://vsz.hnqzz.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://oiu.dashuyun.cn

[T25] Swift：结构体
来源：http://avu.guannengcc.top

struct P { var x: Int }
来源：http://flr.zhixingplan.top

[T26] Swift：类与重写
来源：http://wmw.ydjk.org.cn

class A: Base { override func f() {} }
来源：http://vbc.ctjpmb.com

[T27] Swift：错误处理
来源：http://arb.ybcxt.top

do { try f() } catch { print(error) }
来源：http://klv.shuidangran.top

[T28] Swift：枚举
来源：http://vky.yuanzhike.top

enum Color { case red, green }
来源：http://dbt.zycfv.cn

[T29] Swift：guard 提前返回
来源：http://tkj.yfazqb.com

guard let x = opt else { return }
来源：http://ndi.gaohongyu789.top

[T30] Swift：协议
来源：http://cwh.smart0.xyz

protocol Shape { func area() -> Double }
来源：http://axz.yuxming.cn

[T31] Lua：Hello World
来源：http://zbc.gzhubu.top

print("Hello")
来源：http://alp.snrcjt.cn

[T32] Lua：局部变量
来源：http://rfu.xylfe.cn

local a = 1
来源：http://qkg.svipenyu.cn

[T33] Lua：表（数组）
来源：http://nsy.ehwqpu.com

local t = {1, 2, 3};  t[4] = 4
来源：http://eeg.sweek.top

[T34] Lua：遍历表
来源：http://bxo.guowangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jeo.yanxiufei.cn

[T35] Lua：字典表
来源：http://nrl.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://smb.yuxming.cn

[T36] Lua：函数
来源：http://yej.yj20258888.top

function add(a, b) return a + b end
来源：http://gye.yfazqb.com

[T37] Lua：字符串拼接
来源：http://qak.jiagoushi.top

"a" .. "b"
来源：http://igb.xziqi.cn

[T38] Lua：条件
来源：http://ymz.gotoacloud.top

if x > 0 then print("正") end
来源：http://szt.guowangkeji.top

[T39] Lua：模式匹配
来源：http://jjv.aizwys.cn

string.find(s, "%d+")
来源：http://ngm.xylfe.cn

[T40] Lua：元表
来源：http://grl.sysykeji.top

setmetatable({}, { __index = base })
来源：http://lxd.guannengcc.top

[T41] Perl：Hello World
来源：http://pjd.jiagoushi.top

print "Hello\n";
来源：http://thm.zhoulong.xyz

[T42] Perl：变量类型
来源：http://wdt.pycfn.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ffo.shanyushiyangtech.top

[T43] Perl：字符串插值
来源：http://kof.birdmap.top

"值: $a"
来源：http://ioq.aizwys.cn

[T44] Perl：条件
来源：http://mla.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://ejo.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://vse.zdbjq.cn

for my $x (@arr) { print $x; }
来源：http://ocm.gzhubu.top

[T46] Perl：哈希操作
来源：http://drt.zhongyouzk.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dgt.cashguo.top

[T47] Perl：正则捕获
来源：http://xfx.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tla.yuanzhike.top

[T48] Perl：正则替换
来源：http://gqr.ehwqpu.com

$s =~ s/old/new/g;
来源：http://dil.chenjidiqi.icu

[T49] Perl：函数
来源：http://fks.jqgufenzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qtt.zhengqikj.top

[T50] Perl：逐行读文件
来源：http://ebe.yj202588.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tei.nanxinkj.top

while (my $line = <$fh>) { print $line; }
来源：http://lmt.daxiang520.top

[T51] Scala：Hello World
来源：http://kcf.svipenyu.cn

println("Hello")
来源：http://qzz.yj20258.top

[T52] Scala：变量
来源：http://ahv.mhx1999.top

val a = 1;  var b = 2
来源：http://bsg.yongpay.top

[T53] Scala：字符串插值
来源：http://feq.yuanzhike.top

s"值: $b"
来源：http://yms.vehdjk.com

[T54] Scala：集合映射
来源：http://kqt.fktsv.cn

List(1, 2, 3).map(_ * 2)
来源：http://mxe.xylfe.cn

[T55] Scala：集合过滤
来源：http://ved.sxryk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jgm.9152youxi.cn

[T56] Scala：样例类
来源：http://ndb.nanxuanxn.top

case class User(name: String, age: Int)
来源：http://thv.9152youxi.cn

[T57] Scala：模式匹配
来源：http://uxn.cheryme.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gpk.yj20258.top

[T58] Scala：函数定义
来源：http://yle.pycfn.com

def add(a: Int, b: Int): Int = a + b
来源：http://zrj.yonumen.top

[T59] Scala：循环
来源：http://mhl.dianchejie.cn

for (i <- 1 to 10) println(i)
来源：http://egq.yj20258.top

[T60] Scala：折叠
来源：http://zda.yangfankeji.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://edr.hysaishi.cn

================================================================================
来源：http://clo.cashguo.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nzy.guowangkeji.top

================================================================================
来源：http://kqx.zdbjq.cn

[U01] Py：创建虚拟环境
来源：http://vmp.hnxiangtu.top

python -m venv .venv && source .venv/bin/activate
来源：http://ged.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://kgc.chenlongwang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jrv.pengpengdd.cyou

[U03] Py：加载 .env 配置
来源：http://azz.yuanzhike.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zem.c1oappe.top

[U04] Py：变量调试打印
来源：http://myb.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ffj.chenlongwang.top

[U05] Py：列表去重且保序
来源：http://flz.fehbvm.com

list(dict.fromkeys(arr))
来源：http://aik.sjlbkw.cn

[U06] Py：合并两个字典
来源：http://tsj.vqdsnc.cn

{**a, **b}
来源：http://ijr.iojbl.cn

[U07] Py：反转字典键值
来源：http://mtj.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://lpw.bbcook.cn

[U08] Py：展平二维列表
来源：http://bal.tian-w.cn

[y for x in nested for y in x]
来源：http://klz.yueranfly.top

[U09] Py：字典取最大值的键
来源：http://mda.daxiang520.top

max(d, key=d.get)
来源：http://rin.nanxuanxn.top

[U10] Py：按值排序字典
来源：http://xcv.pengpengdd.cyou

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tyh.ydjk.org.cn

[U11] Py：生成器表达式
来源：http://nvn.daxiang520.top

(x * 2 for x in arr)
来源：http://php.zhijiandao.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mjf.xuanzx.com

Counter(arr).most_common(3)
来源：http://kxt.snrcjt.cn

[U13] Py：固定长度队列
来源：http://kqq.tian-w.cn

deque(maxlen=10)
来源：http://xxn.yueranfly.top

[U14] Py：分组收集到列表
来源：http://jxr.yj20258888.top

defaultdict(list)
来源：http://abd.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://uyq.zhijiandao.cn

t = time.perf_counter()
来源：http://oal.yuxming.cn

[U16] Py：命令行参数解析
来源：http://cjh.tarul.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bth.jlsjyb.cn

[U17] Py：初始化日志
来源：http://zjz.bbcook.cn

logging.basicConfig(level=logging.INFO)
来源：http://mwu.cucudq.cn

[U18] Py：预编译正则
来源：http://ttp.guannengcc.top

pat = re.compile(r"\d+")
来源：http://nxm.wangdashe.top

[U19] Py：正则替换带回调
来源：http://lwl.zhaomingkeji.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mwe.shzxlz.cn

[U20] Py：缓存函数结果
来源：http://nee.cdnleiting.top

@functools.lru_cache(maxsize=None)
来源：http://aud.sweek.top

[U21] Py：自定义上下文管理器
来源：http://npq.316326.xyz

@contextlib.contextmanager
来源：http://ebt.ydjk.org.cn

[U22] Py：矩阵转置
来源：http://rkq.andypj.xyz

list(zip(*m))
来源：http://rkq.ybcxt.top

[U23] Py：分块读取大文件
来源：http://giw.gaohongyu789.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xmq.bjfxy.top

[U24] Py：路径操作
来源：http://ufv.yanxiufei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fmw.jinqigufen.top

[U25] Py：CSV 按字典读
来源：http://gfp.sxryk.cn

csv.DictReader(f)
来源：http://pnh.tianlin.xyz

[U26] Py：并发下载
来源：http://tpk.zhengqikj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vac.haohaochexian.top

[U27] Py：异步 HTTP
来源：http://yvc.hesvh.cn

aiohttp.ClientSession() 配合 async with
来源：http://lbh.gogol.net.cn

[U28] Py：类型别名
来源：http://cer.cqqwz.cn

UserId = int
来源：http://bxz.52xcode.cn

[U29] Py：属性校验
来源：http://vts.vehdjk.com

@property 与 @x.setter 配合
来源：http://bhn.zycfv.cn

[U30] Py：数据类
来源：http://mwv.zhongyouzk.top

@dataclass(slots=True)
来源：http://juj.kuanghao11.cn

[U31] Py：单测
来源：http://qcn.yj202588.top

python -m pytest -q
来源：http://ied.jqgufenzy.top

[U32] Py：代码格式化
来源：http://mwp.zdqjudy.top

ruff format . && ruff check --fix .
来源：http://stm.nanxinkj.top

[U33] Py：打包发布
来源：http://qrz.zdqjudy.top

python -m build  （依赖 pyproject.toml）
来源：http://rca.zdbjq.cn

[U34] Py：判断编码
来源：http://ffy.mhx1999.top

chardet.detect(raw)
来源：http://rjw.aibaodan.cn

[U35] Py：发送邮件
来源：http://rie.shangyingyoupin.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rwj.daria6918.cn

[U36] Py：定时任务
来源：http://mcx.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://zoz.cashguo.top

[U37] Py：读写 Excel
来源：http://nwz.gogol.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bbz.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://stw.yangfankeji.com

Path(__file__).resolve().parent
来源：http://mlj.svipenyu.cn

[U39] Py：判断是否在交互环境
来源：http://cqh.hywenlv.cn

sys.stdout.isatty()
来源：http://gau.pengpengdd.cyou

[U40] Py：打印到标准错误
来源：http://mao.gzhubu.top

print("err", file=sys.stderr)
来源：http://uik.jianghu66.top

[U41] PHP：初始化 Composer 项目
来源：http://yeq.yuanzhike.top

composer init;  composer require guzzlehttp/guzzle
来源：http://cpo.gotoacloud.top

[U42] PHP：PSR-4 自动加载
来源：http://tvi.sxryk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xfd.cashguo.top

[U43] PHP：声明命名空间
来源：http://xlz.cheryme.top

namespace App\Http;
来源：http://nda.fzhhl.top

[U44] PHP：开启严格类型
来源：http://zel.hesvh.cn

declare(strict_types=1);
来源：http://eab.quarkkingdee.top

[U45] PHP：类型声明与返回类型
来源：http://osl.52xcode.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wjd.jqgufenzy.top

[U46] PHP：可空类型
来源：http://hsl.ehwqpu.com

?string $name = null
来源：http://ybn.jiagoushi.top

[U47] PHP：联合类型
来源：http://ihk.birdmap.top

int|string $id
来源：http://rml.wangshuangyany.cn

[U48] PHP：纯枚举
来源：http://zju.zhaomingkeji.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cdg.dashuyun.cn

[U49] PHP：只读属性
来源：http://pmt.yangfankeji.com

public readonly string $name
来源：http://eqc.redwolf501.top

[U50] PHP：构造器属性提升
来源：http://ftd.jinghuilouyu.cn

public function __construct(private int $id) {}
来源：http://hrs.0kj1m.cn

[U51] PHP：数组解构
来源：http://smc.mhx1999.top

[$a, $b] = $arr;
来源：http://wfl.epnwcf.com

[U52] PHP：箭头函数
来源：http://kxh.fanxiaobao.xyz

$double = fn($x) => $x * 2;
来源：http://qmn.hongshengwenyu.top

[U53] PHP：空合并运算符
来源：http://vff.c1oappe.top

$v = $a ?? $b ?? "default";
来源：http://guq.ehwqpu.com

[U54] PHP：空安全调用
来源：http://dvn.vehdjk.com

$obj?->method()
来源：http://pdb.iojbl.cn

[U55] PHP：match 表达式
来源：http://phk.wangshuangyany.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lgh.nanxuanxn.top

[U56] PHP：命名参数
来源：http://aly.quarkkingdee.top

f(a: 1, b: 2)
来源：http://qzs.hesvh.cn

[U57] PHP：字符串插值
来源：http://qmc.sufxvd.cn

"值: {$a}"
来源：http://qev.zhongyouzk.top

[U58] PHP：数组三件套
来源：http://aer.zhongyouzk.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ipy.ydjk.org.cn

[U59] PHP：自定义排序
来源：http://ete.quarkkingdee.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://csy.fengsongda.top

[U60] PHP：JSON 编解码
来源：http://uzn.uphjek.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bty.cashguo.top

[U61] PHP：正则
来源：http://hpo.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://awa.xylfe.cn

[U62] PHP：日期对象
来源：http://dms.shanyushiyangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gqd.jqgfzy.top

[U63] PHP：文件读写
来源：http://xig.epnwcf.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rms.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://dgj.xuetiantiany.cn

glob("dir/*.php");  scandir("dir");
来源：http://azo.sufxvd.cn

[U65] PHP：会话
来源：http://qzn.zhengqikj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://piv.aibaodan.cn

[U66] PHP：设置 Cookie
来源：http://ilw.sysykeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gfu.quarkkingdee.top

[U67] PHP：处理文件上传
来源：http://hgh.shangyingyoupin.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fvi.hywenlv.cn

[U68] PHP：PDO 连接
来源：http://rqj.tarul.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://htn.yangfankeji.com

[U69] PHP：PDO 预处理
来源：http://cui.wangshuangyany.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rvl.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://esr.tianlin.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://axd.aizwys.cn

[U71] PHP：抛出异常
来源：http://aos.hysaishi.cn

throw new RuntimeException("失败", 500);
来源：http://orv.snrcjt.cn

[U72] PHP：写错误日志
来源：http://nvr.sweek.top

error_log("失败: " . $e->getMessage());
来源：http://tdy.ydjk.org.cn

[U73] PHP：读取 ini 配置
来源：http://qmo.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://wzg.kuanghao11.cn

[U74] PHP：读取环境变量
来源：http://xpk.hnxiangtu.top

getenv("APP_ENV") ?: "production"
来源：http://ekw.ivvv.top

[U75] PHP：依赖注入
来源：http://yxi.yuxming.cn

composer require psr/container
来源：http://xtl.fengsongda.top

[U76] PHP：简单路由
来源：http://tbw.daria6918.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jne.tarul.cn

[U77] PHP：模板渲染
来源：http://esf.redwolf501.top

composer require twig/twig
来源：http://utk.zhaomingkeji.xyz

[U78] PHP：单元测试
来源：http://vhn.shanyushiyangkeji.top

composer require --dev phpunit/phpunit
来源：http://urm.dashuyun.cn


<!-- 参考信息 -->