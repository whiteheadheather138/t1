代发 wailian999

int size() const noexcept { return n_; }
来源：http://uux.chenjidiqi.icu

[S53] C++：移动语义
来源：http://odc.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://fgo.bjfxy.top

[S54] C++：异常处理
来源：http://use.shuidangran.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xgu.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://xjy.zhaomingkeji.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://jjo.zhongyouzk.top

[S56] C++：optional
来源：http://vss.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vot.ppjwa.cn

[S57] C++：编译期常量
来源：http://pmi.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://owf.zhijiandao.cn

[S58] C++：命名空间
来源：http://lpt.jlsjyb.cn

namespace ns { int f() { return 1; } }
来源：http://bre.zdqjudy.top

[S59] C++：静态断言
来源：http://rxh.hongshengwenyu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xse.jinghuilouyu.cn

[S60] C++：遍历并删除元素
来源：http://oux.dianchejie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nan.cdnleiting.top

================================================================================
来源：http://zkg.xinyue.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://czw.snrcjt.cn

================================================================================
来源：http://uji.cdnleiting.top

[T01] Kotlin：Hello World
来源：http://aih.yvedp.cn

println("Hello")
来源：http://xdv.vehdjk.com

[T02] Kotlin：变量
来源：http://ogk.mhx1999.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uil.0kj1m.cn

[T03] Kotlin：字符串模板
来源：http://ilv.c1oappe.top

"值: $b"
来源：http://hvu.ybcxt.top

[T04] Kotlin：空安全
来源：http://xaf.cqqwz.cn

val n: String? = null;  n?.length
来源：http://ttw.yfazqb.com

[T05] Kotlin：when 表达式
来源：http://hay.shuidangran.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cmt.xinyue.icu

[T06] Kotlin：集合映射
来源：http://riv.52xcode.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gnt.jqgufenzy.top

[T07] Kotlin：集合过滤
来源：http://rzl.vqdsnc.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qcs.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://bzi.dashuyun.cn

data class User(val name: String, val age: Int)
来源：http://jmw.ivvv.top

[T09] Kotlin：扩展函数
来源：http://pqa.havefunace.top

fun String.exclaim() = this + "!"
来源：http://ejp.xylfe.cn

[T10] Kotlin：默认参数
来源：http://mzz.shuidangran.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yvm.uphjek.com

[T11] Kotlin：协程
来源：http://ouu.fengsongda.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xfa.yueranfly.top

[T12] Kotlin：解构声明
来源：http://vwe.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://twc.chenlongwang.top

[T13] Kotlin：只读 Map
来源：http://tqn.tian-w.cn

val m = mapOf("a" to 1)
来源：http://pwg.sxryk.cn

[T14] Kotlin：循环
来源：http://khr.tanke756.top

for (i in 1..10) println(i)
来源：http://eos.zhaomingkeji.xyz

[T15] Kotlin：接口
来源：http://tre.quarkkingdee.top

interface Shape { fun area(): Double }
来源：http://xvl.hywenlv.cn

[T16] Swift：Hello World
来源：http://ssz.sjlbkw.cn

print("Hello")
来源：http://kxr.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://ioh.c1oappe.top

var a = 1;  let b = 2
来源：http://nxs.cashguo.top

[T18] Swift：字符串插值
来源：http://fsp.ydzc1.top

"值: \(b)"
来源：http://uid.jinyuanbaomall.cn

[T19] Swift：可选绑定
来源：http://mae.wangshuangyany.cn

if let n = opt { print(n) }
来源：http://vbh.wangdashe.top

[T20] Swift：数组操作
来源：http://qic.shzxlz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kgx.snrcjt.cn

[T21] Swift：遍历
来源：http://tjj.pengpengdd.cyou

for x in a { print(x) }
来源：http://hwn.kuanghao11.cn

[T22] Swift：字典
来源：http://agz.hfpthk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vak.jqgfzy.top

[T23] Swift：函数
来源：http://bja.guannengcc.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ndr.zycfv.cn

[T24] Swift：闭包
来源：http://hck.jiagoushi.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vlb.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://yys.chenzaomai.com

struct P { var x: Int }
来源：http://gnu.9152youxi.cn

[T26] Swift：类与重写
来源：http://cyh.yueranfly.top

class A: Base { override func f() {} }
来源：http://hwk.52xcode.cn

[T27] Swift：错误处理
来源：http://ttl.ybcxt.top

do { try f() } catch { print(error) }
来源：http://hgn.xinyue.icu

[T28] Swift：枚举
来源：http://ffw.hongshengwenyu.top

enum Color { case red, green }
来源：http://jtk.cashguo.top

[T29] Swift：guard 提前返回
来源：http://bml.shanyushiyangkeji.top

guard let x = opt else { return }
来源：http://ogf.sufxvd.cn

[T30] Swift：协议
来源：http://srz.ctjpmb.com

protocol Shape { func area() -> Double }
来源：http://jbz.jianghu66.top

[T31] Lua：Hello World
来源：http://kwh.52xcode.cn

print("Hello")
来源：http://zhe.tarul.cn

[T32] Lua：局部变量
来源：http://cvv.cucudq.cn

local a = 1
来源：http://nbk.ehwqpu.com

[T33] Lua：表（数组）
来源：http://nsi.0kj1m.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oja.uphjek.com

[T34] Lua：遍历表
来源：http://rty.havefunace.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hby.c1oappe.top

[T35] Lua：字典表
来源：http://qna.shuidangran.top

local d = { a = 1 };  d.b = 2
来源：http://uza.ehwqpu.com

[T36] Lua：函数
来源：http://ook.jqgfzy.top

function add(a, b) return a + b end
来源：http://fnu.vqdsnc.cn

[T37] Lua：字符串拼接
来源：http://ihw.vqdsnc.cn

"a" .. "b"
来源：http://bjh.kuanghao11.cn

[T38] Lua：条件
来源：http://wyi.hcnkem.com

if x > 0 then print("正") end
来源：http://dma.sjlbkw.cn

[T39] Lua：模式匹配
来源：http://ogg.jqgfzy.top

string.find(s, "%d+")
来源：http://zhl.cqqwz.cn

[T40] Lua：元表
来源：http://pbo.jlsjyb.cn

setmetatable({}, { __index = base })
来源：http://kff.jqgfzy.top

[T41] Perl：Hello World
来源：http://tgi.andypj.xyz

print "Hello\n";
来源：http://zjm.jlsjyb.cn

[T42] Perl：变量类型
来源：http://liy.aibaodan.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bzs.ivvv.top

[T43] Perl：字符串插值
来源：http://spj.zdqjudy.top

"值: $a"
来源：http://dai.bjfxy.top

[T44] Perl：条件
来源：http://swp.ctjpmb.com

if ($a > 0) { print "正"; }
来源：http://mwx.jinqigufen.top

[T45] Perl：数组遍历
来源：http://qos.kuanghao11.cn

for my $x (@arr) { print $x; }
来源：http://rvj.chenjidiqi.icu

[T46] Perl：哈希操作
来源：http://dpl.tanke756.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hbn.yonumen.top

[T47] Perl：正则捕获
来源：http://knq.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pvm.yonumen.top

[T48] Perl：正则替换
来源：http://iqj.uphjek.com

$s =~ s/old/new/g;
来源：http://ylw.zhengqikj.top

[T49] Perl：函数
来源：http://ifv.jinyuanbaomall.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://utp.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://bnq.ywan-chungtsiang.top

open my $fh, "<", "a.txt" or die $!;
来源：http://buc.nanxuanxn.top

while (my $line = <$fh>) { print $line; }
来源：http://ztq.cqqwz.cn

[T51] Scala：Hello World
来源：http://yzu.aibaodan.cn

println("Hello")
来源：http://kmz.ydjk.org.cn

[T52] Scala：变量
来源：http://esv.kuanghao11.cn

val a = 1;  var b = 2
来源：http://lds.haohaochexian.top

[T53] Scala：字符串插值
来源：http://zpa.daxiang520.top

s"值: $b"
来源：http://knh.jqgfzy.top

[T54] Scala：集合映射
来源：http://qtw.ppjwa.cn

List(1, 2, 3).map(_ * 2)
来源：http://jfu.shangyingyoupin.top

[T55] Scala：集合过滤
来源：http://zkg.cashguo.top

List(1, 2, 3).filter(_ > 1)
来源：http://lox.guannengcc.top

[T56] Scala：样例类
来源：http://zyl.jianghu66.top

case class User(name: String, age: Int)
来源：http://ovm.vqdsnc.cn

[T57] Scala：模式匹配
来源：http://kai.c1oappe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://whk.wangdashe.top

[T58] Scala：函数定义
来源：http://unj.sweek.top

def add(a: Int, b: Int): Int = a + b
来源：http://gvs.fengsongda.top

[T59] Scala：循环
来源：http://wgv.cdnleiting.top

for (i <- 1 to 10) println(i)
来源：http://xsn.mhx1999.top

[T60] Scala：折叠
来源：http://esd.shanyushiyangkeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ums.zhengqikj.top

================================================================================
来源：http://scl.sufxvd.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qxp.snrcjt.cn

================================================================================
来源：http://yaq.havefunace.top

[U01] Py：创建虚拟环境
来源：http://ihy.mhx1999.top

python -m venv .venv && source .venv/bin/activate
来源：http://xno.tian-w.cn

[U02] Py：导出 / 安装依赖
来源：http://sib.kuanghao11.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kau.ivvv.top

[U03] Py：加载 .env 配置
来源：http://fll.gzhubu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://rvn.shzxlz.cn

[U04] Py：变量调试打印
来源：http://dos.daxiang520.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mjv.ctjpmb.com

[U05] Py：列表去重且保序
来源：http://daz.xuetiantiany.cn

list(dict.fromkeys(arr))
来源：http://jvv.dianchejie.cn

[U06] Py：合并两个字典
来源：http://ylu.316326.xyz

{**a, **b}
来源：http://cng.hesvh.cn

[U07] Py：反转字典键值
来源：http://vne.sweek.top

{v: k for k, v in d.items()}
来源：http://pkk.xinyue.icu

[U08] Py：展平二维列表
来源：http://nsw.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://tsv.snrcjt.cn

[U09] Py：字典取最大值的键
来源：http://czx.xuetiantiany.cn

max(d, key=d.get)
来源：http://tez.jinghuilouyu.cn

[U10] Py：按值排序字典
来源：http://yoa.bbcook.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ndw.epnwcf.com

[U11] Py：生成器表达式
来源：http://jli.tianlin.xyz

(x * 2 for x in arr)
来源：http://hlq.cheryme.top

[U12] Py：取出现最多的 3 个元素
来源：http://jei.yj202588.top

Counter(arr).most_common(3)
来源：http://lbq.yonumen.top

[U13] Py：固定长度队列
来源：http://jdg.uphjek.com

deque(maxlen=10)
来源：http://yhv.jinghuilouyu.cn

[U14] Py：分组收集到列表
来源：http://xlg.hysaishi.cn

defaultdict(list)
来源：http://ksv.xuanzx.com

[U15] Py：高精度计时
来源：http://zpc.cashguo.top

t = time.perf_counter()
来源：http://bys.zhixingplan.top

[U16] Py：命令行参数解析
来源：http://uhj.andypj.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pwv.birdmap.top

[U17] Py：初始化日志
来源：http://gyg.yuxming.cn

logging.basicConfig(level=logging.INFO)
来源：http://yjn.ybcxt.top

[U18] Py：预编译正则
来源：http://qwb.zhijiandao.cn

pat = re.compile(r"\d+")
来源：http://ixo.haohaochexian.top

[U19] Py：正则替换带回调
来源：http://bmi.haohaochexian.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jei.hywenlv.cn

[U20] Py：缓存函数结果
来源：http://mgx.zycfv.cn

@functools.lru_cache(maxsize=None)
来源：http://naq.jinqigufen.top

[U21] Py：自定义上下文管理器
来源：http://nfh.jinqigfzy.top

@contextlib.contextmanager
来源：http://ctc.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://duq.yj20258.top

list(zip(*m))
来源：http://xno.zhiwuduotai.top

[U23] Py：分块读取大文件
来源：http://jal.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kve.xingfuxueyuan.xyz

[U24] Py：路径操作
来源：http://jiq.fanxiaobao.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xjr.jlsjyb.cn

[U25] Py：CSV 按字典读
来源：http://jag.yuxming.cn

csv.DictReader(f)
来源：http://dwl.gotoacloud.top

[U26] Py：并发下载
来源：http://ucd.birdmap.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nke.mhx1999.top

[U27] Py：异步 HTTP
来源：http://szk.redwolf501.top

aiohttp.ClientSession() 配合 async with
来源：http://jen.xziqi.cn

[U28] Py：类型别名
来源：http://mty.tian-w.cn

UserId = int
来源：http://vgq.xinyue.icu

[U29] Py：属性校验
来源：http://ouh.cheryme.top

@property 与 @x.setter 配合
来源：http://ylj.yuxming.cn

[U30] Py：数据类
来源：http://ggt.ctjpmb.com

@dataclass(slots=True)
来源：http://keo.hnxiangtu.top

[U31] Py：单测
来源：http://qgu.hnqzz.top

python -m pytest -q
来源：http://gpm.mhx1999.top

[U32] Py：代码格式化
来源：http://aac.havefunace.top

ruff format . && ruff check --fix .
来源：http://dcs.yonumen.top

[U33] Py：打包发布
来源：http://qxp.shanyushiyangtech.top

python -m build  （依赖 pyproject.toml）
来源：http://nlw.sufxvd.cn

[U34] Py：判断编码
来源：http://naw.hysaishi.cn

chardet.detect(raw)
来源：http://svx.yj20258888.top

[U35] Py：发送邮件
来源：http://hfb.yonumen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oio.daria6918.cn

[U36] Py：定时任务
来源：http://tsp.yangfankeji.com

schedule.every(10).minutes.do(job)
来源：http://rbj.hammf.cn

[U37] Py：读写 Excel
来源：http://qxr.zhengqikj.top

pandas.read_excel / DataFrame.to_excel
来源：http://ohd.ctjpmb.com

[U38] Py：获取脚本所在目录
来源：http://epm.nanxinkj.top

Path(__file__).resolve().parent
来源：http://wet.iojbl.cn

[U39] Py：判断是否在交互环境
来源：http://byc.xuetiantiany.cn

sys.stdout.isatty()
来源：http://uwx.yanxiufei.cn

[U40] Py：打印到标准错误
来源：http://hjq.shangyingyoupin.top

print("err", file=sys.stderr)
来源：http://wuj.shzxlz.cn

[U41] PHP：初始化 Composer 项目
来源：http://zdw.smart0.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://qlt.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://nrb.tian-w.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sbb.tanke756.top

[U43] PHP：声明命名空间
来源：http://akb.zhongyouzk.top

namespace App\Http;
来源：http://irp.pengpengdd.cyou

[U44] PHP：开启严格类型
来源：http://diy.jinqigfzy.top

declare(strict_types=1);
来源：http://cxo.xziqi.cn

[U45] PHP：类型声明与返回类型
来源：http://xiq.jiagoushi.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://knj.bbcook.cn

[U46] PHP：可空类型
来源：http://yya.zhiwuduotai.top

?string $name = null
来源：http://vcj.jiagoushi.top

[U47] PHP：联合类型
来源：http://luf.xuanzx.com

int|string $id
来源：http://vqg.yfazqb.com

[U48] PHP：纯枚举
来源：http://mns.fzhhl.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yru.gotoacloud.top

[U49] PHP：只读属性
来源：http://mwg.cdnleiting.top

public readonly string $name
来源：http://hzh.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://qjq.gotoacloud.top

public function __construct(private int $id) {}
来源：http://iat.zhengqikj.top

[U51] PHP：数组解构
来源：http://mza.bbcook.cn

[$a, $b] = $arr;
来源：http://qma.hongshengwenyu.top

[U52] PHP：箭头函数
来源：http://ver.vqdsnc.cn

$double = fn($x) => $x * 2;
来源：http://thd.sxryk.cn

[U53] PHP：空合并运算符
来源：http://uxn.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://fut.hywenlv.cn

[U54] PHP：空安全调用
来源：http://nca.chenlongwang.top

$obj?->method()
来源：http://bbi.hnxiangtu.top

[U55] PHP：match 表达式
来源：http://nqa.xylfe.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ztg.vqdsnc.cn

[U56] PHP：命名参数
来源：http://zhw.cucudq.cn

f(a: 1, b: 2)
来源：http://qrn.andypj.xyz

[U57] PHP：字符串插值
来源：http://fnj.yuanzhike.top

"值: {$a}"
来源：http://zlg.sufxvd.cn

[U58] PHP：数组三件套
来源：http://dhh.feifeiyinyue.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ctz.fanxiaobao.xyz

[U59] PHP：自定义排序
来源：http://czp.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hmj.yvedp.cn

[U60] PHP：JSON 编解码
来源：http://szl.jlsjyb.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ueb.pycfn.com

[U61] PHP：正则
来源：http://jtv.nwbrower.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mbe.xuetiantiany.cn

[U62] PHP：日期对象
来源：http://lbb.aibaodan.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://acy.mhx1999.top

[U63] PHP：文件读写
来源：http://ngh.jinghuilouyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://afx.0kj1m.cn

[U64] PHP：目录遍历
来源：http://hev.jianghu66.top

glob("dir/*.php");  scandir("dir");
来源：http://hax.jinqigfzy.top

[U65] PHP：会话
来源：http://eqw.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vkz.yj20258888.top

[U66] PHP：设置 Cookie
来源：http://spa.jinqigufen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yoi.hesvh.cn

[U67] PHP：处理文件上传
来源：http://ejo.tanke756.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oei.bbcook.cn

[U68] PHP：PDO 连接
来源：http://ilw.yangfankeji.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://row.havefunace.top

[U69] PHP：PDO 预处理
来源：http://pud.haohaochexian.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pqp.chenzaomai.com

[U70] PHP：PDO 事务
来源：http://xcd.xingfuxueyuan.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uvp.vqdsnc.cn

[U71] PHP：抛出异常
来源：http://kzp.vehdjk.com

throw new RuntimeException("失败", 500);
来源：http://jis.gotoacloud.top

[U72] PHP：写错误日志
来源：http://hon.jinyuanbaomall.cn

error_log("失败: " . $e->getMessage());
来源：http://kch.jinqigfzy.top

[U73] PHP：读取 ini 配置
来源：http://qlu.snrcjt.cn

parse_ini_file("config.ini", true)
来源：http://rgj.bjfxy.top

[U74] PHP：读取环境变量
来源：http://dds.uphjek.com

getenv("APP_ENV") ?: "production"
来源：http://txy.zdqjudy.top

[U75] PHP：依赖注入
来源：http://odz.gogol.net.cn

composer require psr/container
来源：http://xuj.tarul.cn

[U76] PHP：简单路由
来源：http://wax.sxryk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://seo.ybcxt.top

[U77] PHP：模板渲染
来源：http://blo.yueranfly.top

composer require twig/twig
来源：http://zvj.shzxlz.cn

[U78] PHP：单元测试
来源：http://yzt.dianchejie.cn

composer require --dev phpunit/phpunit
来源：http://spt.shanyushiyangkeji.top


<!-- 参考信息 -->