代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://qau.ydjk.org.cn

[S59] C++：静态断言
来源：http://mfp.xuanzx.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://imf.daria6918.cn

[S60] C++：遍历并删除元素
来源：http://pxu.jinyuanbaomall.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tlv.snrcjt.cn

================================================================================
来源：http://xge.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lwl.tarul.cn

================================================================================
来源：http://erm.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://hym.shanyushiyangkeji.top

println("Hello")
来源：http://ifo.gzhubu.top

[T02] Kotlin：变量
来源：http://brf.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://utg.kuanghao11.cn

[T03] Kotlin：字符串模板
来源：http://dzv.daria6918.cn

"值: $b"
来源：http://oyg.tanke756.top

[T04] Kotlin：空安全
来源：http://dws.chenzaomai.com

val n: String? = null;  n?.length
来源：http://wuw.hammf.cn

[T05] Kotlin：when 表达式
来源：http://stq.sjlbkw.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pkl.fzhhl.top

[T06] Kotlin：集合映射
来源：http://med.yuxming.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rue.sweek.top

[T07] Kotlin：集合过滤
来源：http://hyl.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nwo.tian-w.cn

[T08] Kotlin：数据类
来源：http://sqm.zhengqikj.top

data class User(val name: String, val age: Int)
来源：http://dev.xuetiantiany.cn

[T09] Kotlin：扩展函数
来源：http://wln.yuanzhike.top

fun String.exclaim() = this + "!"
来源：http://xgy.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://tvg.jinghuilouyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gwu.shanyushiyangtech.top

[T11] Kotlin：协程
来源：http://dhp.sysykeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jdm.mhx1999.top

[T12] Kotlin：解构声明
来源：http://yzl.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://knp.fzhhl.top

[T13] Kotlin：只读 Map
来源：http://ixl.316326.xyz

val m = mapOf("a" to 1)
来源：http://ycd.aibaodan.cn

[T14] Kotlin：循环
来源：http://ycw.shanyushiyangtech.top

for (i in 1..10) println(i)
来源：http://aix.guowangkeji.top

[T15] Kotlin：接口
来源：http://jxi.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://myn.svipenyu.cn

[T16] Swift：Hello World
来源：http://qmu.jinyuanbaomall.cn

print("Hello")
来源：http://ftm.zhiwuduotai.top

[T17] Swift：变量与常量
来源：http://czp.xylfe.cn

var a = 1;  let b = 2
来源：http://tlp.ydzc1.top

[T18] Swift：字符串插值
来源：http://chx.uphjek.com

"值: \(b)"
来源：http://vqc.jinqigfzy.top

[T19] Swift：可选绑定
来源：http://zbi.jinghuilouyu.cn

if let n = opt { print(n) }
来源：http://bab.pycfn.com

[T20] Swift：数组操作
来源：http://rzg.chenjidiqi.icu

var a = [1, 2, 3];  a.append(4)
来源：http://txo.aibaodan.cn

[T21] Swift：遍历
来源：http://qvu.tanke756.top

for x in a { print(x) }
来源：http://mrb.zhongyouzk.top

[T22] Swift：字典
来源：http://ioj.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uhd.haohaochexian.top

[T23] Swift：函数
来源：http://cdb.xuetiantiany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dat.fzhhl.top

[T24] Swift：闭包
来源：http://ugm.snrcjt.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fpa.yanxiufei.cn

[T25] Swift：结构体
来源：http://cny.bbcook.cn

struct P { var x: Int }
来源：http://icu.aizwys.cn

[T26] Swift：类与重写
来源：http://cjm.fengsongda.top

class A: Base { override func f() {} }
来源：http://edh.wangdashe.top

[T27] Swift：错误处理
来源：http://qiw.xingfuxueyuan.xyz

do { try f() } catch { print(error) }
来源：http://pks.hcnkem.com

[T28] Swift：枚举
来源：http://uyl.yfazqb.com

enum Color { case red, green }
来源：http://spm.yuanzhike.top

[T29] Swift：guard 提前返回
来源：http://pap.tanke756.top

guard let x = opt else { return }
来源：http://rax.hfpthk.cn

[T30] Swift：协议
来源：http://mwy.nwbrower.top

protocol Shape { func area() -> Double }
来源：http://hve.yonumen.top

[T31] Lua：Hello World
来源：http://gzu.yuxming.cn

print("Hello")
来源：http://qap.jinqigfzy.top

[T32] Lua：局部变量
来源：http://kmm.zhaomingkeji.xyz

local a = 1
来源：http://pci.shuidangran.top

[T33] Lua：表（数组）
来源：http://nvj.zhengqikj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://eyb.yuxming.cn

[T34] Lua：遍历表
来源：http://sth.gzhubu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kza.svipenyu.cn

[T35] Lua：字典表
来源：http://ypz.yangfankeji.com

local d = { a = 1 };  d.b = 2
来源：http://gmy.hongshengwenyu.top

[T36] Lua：函数
来源：http://tsj.zdbjq.cn

function add(a, b) return a + b end
来源：http://rsm.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://gnt.nwbrower.top

"a" .. "b"
来源：http://llj.hnxiangtu.top

[T38] Lua：条件
来源：http://jaj.nanxuanxn.top

if x > 0 then print("正") end
来源：http://qsm.jinyuanbaomall.cn

[T39] Lua：模式匹配
来源：http://rbd.pycfn.com

string.find(s, "%d+")
来源：http://efs.yuxming.cn

[T40] Lua：元表
来源：http://gke.ctjpmb.com

setmetatable({}, { __index = base })
来源：http://biy.ivvv.top

[T41] Perl：Hello World
来源：http://tkd.yangfankeji.com

print "Hello\n";
来源：http://eqf.redwolf501.top

[T42] Perl：变量类型
来源：http://buj.cqqwz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tzn.kuanghao11.cn

[T43] Perl：字符串插值
来源：http://pss.daria6918.cn

"值: $a"
来源：http://pvm.zhijiandao.cn

[T44] Perl：条件
来源：http://qdh.redwolf501.top

if ($a > 0) { print "正"; }
来源：http://ukt.sweek.top

[T45] Perl：数组遍历
来源：http://exo.yvedp.cn

for my $x (@arr) { print $x; }
来源：http://reb.zdbjq.cn

[T46] Perl：哈希操作
来源：http://sed.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://key.ywan-chungtsiang.top

[T47] Perl：正则捕获
来源：http://vwz.epnwcf.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://ezn.snrcjt.cn

[T48] Perl：正则替换
来源：http://izs.fktsv.cn

$s =~ s/old/new/g;
来源：http://nso.tanke756.top

[T49] Perl：函数
来源：http://hrp.sjlbkw.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qms.yueranfly.top

[T50] Perl：逐行读文件
来源：http://smw.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://usg.redwolf501.top

while (my $line = <$fh>) { print $line; }
来源：http://utg.jlsjyb.cn

[T51] Scala：Hello World
来源：http://ewe.mhx1999.top

println("Hello")
来源：http://uwf.haohaochexian.top

[T52] Scala：变量
来源：http://hyd.hnqzz.top

val a = 1;  var b = 2
来源：http://rvf.tianlin.xyz

[T53] Scala：字符串插值
来源：http://kls.hcnkem.com

s"值: $b"
来源：http://upr.nanxuanxn.top

[T54] Scala：集合映射
来源：http://tnv.xingfuxueyuan.xyz

List(1, 2, 3).map(_ * 2)
来源：http://mzs.jiagoushi.top

[T55] Scala：集合过滤
来源：http://gzk.jinghuilouyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ecg.cdnleiting.top

[T56] Scala：样例类
来源：http://xhg.ivvv.top

case class User(name: String, age: Int)
来源：http://vuy.zhijiandao.cn

[T57] Scala：模式匹配
来源：http://iij.wangshuangyany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ecp.kuanghao11.cn

[T58] Scala：函数定义
来源：http://cxt.shzxlz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zyg.fanxiaobao.xyz

[T59] Scala：循环
来源：http://liq.yangfankeji.com

for (i <- 1 to 10) println(i)
来源：http://nno.yj20258.top

[T60] Scala：折叠
来源：http://haz.cdnleiting.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pid.sxryk.cn

================================================================================
来源：http://nlk.aibaodan.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vga.shangyingyoupin.top

================================================================================
来源：http://ans.daria6918.cn

[U01] Py：创建虚拟环境
来源：http://bkz.tanke756.top

python -m venv .venv && source .venv/bin/activate
来源：http://izz.xinyue.icu

[U02] Py：导出 / 安装依赖
来源：http://hww.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hkq.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://onb.bjfxy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://yvp.chenjidiqi.icu

[U04] Py：变量调试打印
来源：http://mrw.yfazqb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vbv.hnqzz.top

[U05] Py：列表去重且保序
来源：http://qng.yueranfly.top

list(dict.fromkeys(arr))
来源：http://gxf.hongshengwenyu.top

[U06] Py：合并两个字典
来源：http://shw.zdbjq.cn

{**a, **b}
来源：http://adn.0kj1m.cn

[U07] Py：反转字典键值
来源：http://dzb.zhijiandao.cn

{v: k for k, v in d.items()}
来源：http://lvg.dianchejie.cn

[U08] Py：展平二维列表
来源：http://afn.pengpengdd.cyou

[y for x in nested for y in x]
来源：http://aid.pengpengdd.cyou

[U09] Py：字典取最大值的键
来源：http://fzq.ydjk.org.cn

max(d, key=d.get)
来源：http://cvz.hywenlv.cn

[U10] Py：按值排序字典
来源：http://maf.wangshuangyany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xgf.feifeiyinyue.top

[U11] Py：生成器表达式
来源：http://pum.daria6918.cn

(x * 2 for x in arr)
来源：http://fpd.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://zdd.shangyingyoupin.top

Counter(arr).most_common(3)
来源：http://tra.cqqwz.cn

[U13] Py：固定长度队列
来源：http://ctu.pycfn.com

deque(maxlen=10)
来源：http://nwt.gaohongyu789.top

[U14] Py：分组收集到列表
来源：http://tgz.ivvv.top

defaultdict(list)
来源：http://zyc.sufxvd.cn

[U15] Py：高精度计时
来源：http://lpk.gotoacloud.top

t = time.perf_counter()
来源：http://yej.316326.xyz

[U16] Py：命令行参数解析
来源：http://ubt.bjfxy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eqn.ywan-chungtsiang.top

[U17] Py：初始化日志
来源：http://chf.hysaishi.cn

logging.basicConfig(level=logging.INFO)
来源：http://tcp.316326.xyz

[U18] Py：预编译正则
来源：http://cdq.xuanzx.com

pat = re.compile(r"\d+")
来源：http://lww.dashuyun.cn

[U19] Py：正则替换带回调
来源：http://hnk.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wwi.ybcxt.top

[U20] Py：缓存函数结果
来源：http://ebm.chenlongwang.top

@functools.lru_cache(maxsize=None)
来源：http://sti.snrcjt.cn

[U21] Py：自定义上下文管理器
来源：http://emx.chenjidiqi.icu

@contextlib.contextmanager
来源：http://pnz.ppjwa.cn

[U22] Py：矩阵转置
来源：http://vsz.jinghuilouyu.cn

list(zip(*m))
来源：http://dae.9152youxi.cn

[U23] Py：分块读取大文件
来源：http://pba.yonumen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hal.zhongyouzk.top

[U24] Py：路径操作
来源：http://meq.hywenlv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hqw.yueranfly.top

[U25] Py：CSV 按字典读
来源：http://nzl.wangshuangyany.cn

csv.DictReader(f)
来源：http://ing.zhongyouzk.top

[U26] Py：并发下载
来源：http://wfl.nanxuanxn.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fqv.yonumen.top

[U27] Py：异步 HTTP
来源：http://fjz.shangyingyoupin.top

aiohttp.ClientSession() 配合 async with
来源：http://xog.yj20258888.top

[U28] Py：类型别名
来源：http://wyk.ydzc1.top

UserId = int
来源：http://lif.pycfn.com

[U29] Py：属性校验
来源：http://mxi.fanxiaobao.xyz

@property 与 @x.setter 配合
来源：http://ljb.hnqzz.top

[U30] Py：数据类
来源：http://epv.chenlongwang.top

@dataclass(slots=True)
来源：http://cee.guowangkeji.top

[U31] Py：单测
来源：http://sjs.zhijiandao.cn

python -m pytest -q
来源：http://fls.zhongyouzk.top

[U32] Py：代码格式化
来源：http://ppp.yuanzhike.top

ruff format . && ruff check --fix .
来源：http://wkz.xinyue.icu

[U33] Py：打包发布
来源：http://xpq.vehdjk.com

python -m build  （依赖 pyproject.toml）
来源：http://fne.hywenlv.cn

[U34] Py：判断编码
来源：http://fca.sjlbkw.cn

chardet.detect(raw)
来源：http://xko.fktsv.cn

[U35] Py：发送邮件
来源：http://euw.pengpengdd.cyou

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uxf.tanke756.top

[U36] Py：定时任务
来源：http://xjs.fktsv.cn

schedule.every(10).minutes.do(job)
来源：http://vlt.hammf.cn

[U37] Py：读写 Excel
来源：http://csz.ctjpmb.com

pandas.read_excel / DataFrame.to_excel
来源：http://wle.zdbjq.cn

[U38] Py：获取脚本所在目录
来源：http://ppy.ydzc1.top

Path(__file__).resolve().parent
来源：http://jmq.shuidangran.top

[U39] Py：判断是否在交互环境
来源：http://uxa.ehwqpu.com

sys.stdout.isatty()
来源：http://jaf.fanxiaobao.xyz

[U40] Py：打印到标准错误
来源：http://bmk.yongpay.top

print("err", file=sys.stderr)
来源：http://kvp.yuanzhike.top

[U41] PHP：初始化 Composer 项目
来源：http://gkq.chenzaomai.com

composer init;  composer require guzzlehttp/guzzle
来源：http://qnx.zhaomingkeji.xyz

[U42] PHP：PSR-4 自动加载
来源：http://zej.feifeiyinyue.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mnd.birdmap.top

[U43] PHP：声明命名空间
来源：http://ckt.ehwqpu.com

namespace App\Http;
来源：http://ijl.shanyushiyangkeji.top

[U44] PHP：开启严格类型
来源：http://opp.52xcode.cn

declare(strict_types=1);
来源：http://ibu.cheryme.top

[U45] PHP：类型声明与返回类型
来源：http://obo.jinqigufen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://azt.ctjpmb.com

[U46] PHP：可空类型
来源：http://qfe.uphjek.com

?string $name = null
来源：http://qhg.ivvv.top

[U47] PHP：联合类型
来源：http://aov.cucudq.cn

int|string $id
来源：http://gyr.yueranfly.top

[U48] PHP：纯枚举
来源：http://fnw.cdnleiting.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://osp.pengpengdd.cyou

[U49] PHP：只读属性
来源：http://etn.sysykeji.top

public readonly string $name
来源：http://tiy.jyoumei.cn

[U50] PHP：构造器属性提升
来源：http://wln.fzhhl.top

public function __construct(private int $id) {}
来源：http://ezu.ppjwa.cn

[U51] PHP：数组解构
来源：http://hbh.gotoacloud.top

[$a, $b] = $arr;
来源：http://qab.ehwqpu.com

[U52] PHP：箭头函数
来源：http://axl.yj202588.top

$double = fn($x) => $x * 2;
来源：http://mqp.zhoulong.xyz

[U53] PHP：空合并运算符
来源：http://gpi.wangshuangyany.cn

$v = $a ?? $b ?? "default";
来源：http://yoi.52xcode.cn

[U54] PHP：空安全调用
来源：http://dyp.gogol.net.cn

$obj?->method()
来源：http://crk.zhengqikj.top

[U55] PHP：match 表达式
来源：http://urb.hysaishi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dgh.gogol.net.cn

[U56] PHP：命名参数
来源：http://ssd.tian-w.cn

f(a: 1, b: 2)
来源：http://php.yfazqb.com

[U57] PHP：字符串插值
来源：http://kop.shzxlz.cn

"值: {$a}"
来源：http://dfn.zdqjudy.top

[U58] PHP：数组三件套
来源：http://ane.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cfl.hnqzz.top

[U59] PHP：自定义排序
来源：http://pmg.jlsjyb.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pgt.fehbvm.com

[U60] PHP：JSON 编解码
来源：http://mbz.snrcjt.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dnn.zhijiandao.cn

[U61] PHP：正则
来源：http://ktc.pycfn.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ros.gogol.net.cn

[U62] PHP：日期对象
来源：http://kho.snrcjt.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iyd.shuidangran.top

[U63] PHP：文件读写
来源：http://ezl.ywan-chungtsiang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cuz.fzhhl.top

[U64] PHP：目录遍历
来源：http://uet.shangyingyoupin.top

glob("dir/*.php");  scandir("dir");
来源：http://ndo.yangfankeji.com

[U65] PHP：会话
来源：http://ipt.chenlongwang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xxo.zhixingplan.top

[U66] PHP：设置 Cookie
来源：http://acf.iojbl.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fjj.yj20258888.top

[U67] PHP：处理文件上传
来源：http://iiu.xuetiantiany.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yyt.bjfxy.top

[U68] PHP：PDO 连接
来源：http://fbg.haohaochexian.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://emq.ppjwa.cn

[U69] PHP：PDO 预处理
来源：http://jjo.hcnkem.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mcn.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://gae.jqgufenzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ykg.xziqi.cn

[U71] PHP：抛出异常
来源：http://snc.quarkkingdee.top

throw new RuntimeException("失败", 500);
来源：http://hfu.hysaishi.cn

[U72] PHP：写错误日志
来源：http://cth.c1oappe.top

error_log("失败: " . $e->getMessage());
来源：http://ygw.haohaochexian.top

[U73] PHP：读取 ini 配置
来源：http://onq.zhongyouzk.top

parse_ini_file("config.ini", true)
来源：http://nkx.xziqi.cn

[U74] PHP：读取环境变量
来源：http://ckt.yanxiufei.cn

getenv("APP_ENV") ?: "production"
来源：http://mhe.yj20258.top

[U75] PHP：依赖注入
来源：http://kyp.chenjidiqi.icu

composer require psr/container
来源：http://idk.shanyushiyangtech.top

[U76] PHP：简单路由
来源：http://yby.yj202588.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mol.0kj1m.cn

[U77] PHP：模板渲染
来源：http://yif.svipenyu.cn

composer require twig/twig
来源：http://fdr.xinyue.icu

[U78] PHP：单元测试
来源：http://urt.pycfn.com

composer require --dev phpunit/phpunit
来源：http://oca.zdbjq.cn

[U79] PHP：静态分析
来源：http://hwn.tianlin.xyz

composer require --dev phpstan/phpstan
来源：http://ibr.xinyue.icu

[U80] PHP：代码规范修复
来源：http://gmi.xuetiantiany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nhn.yj202588.top

[U81] JS：初始化项目
来源：http://nuz.xuanzx.com

npm init -y;  npm i express
来源：http://zda.bjfxy.top

[U82] JS：package.json 脚本
来源：http://ndh.kuanghao11.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ltk.yueranfly.top

[U83] JS：ES Module 导入导出
来源：http://ysr.zycfv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yfo.yj20258888.top

[U84] JS：CommonJS 写法
来源：http://nxz.redwolf501.top

module.exports = { a };  const { a } = require("./m");
来源：http://lqf.sysykeji.top


<!-- 参考信息 -->