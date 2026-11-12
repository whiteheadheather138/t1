代发 wailian999

[T23] Swift：函数
来源：http://kyf.ydzc1.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qym.nanxinkj.top

[T24] Swift：闭包
来源：http://ykm.zdqjudy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cxz.xuetiantiany.cn

[T25] Swift：结构体
来源：http://zbz.aibaodan.cn

struct P { var x: Int }
来源：http://pla.iojbl.cn

[T26] Swift：类与重写
来源：http://zsf.yangfankeji.com

class A: Base { override func f() {} }
来源：http://cic.hysaishi.cn

[T27] Swift：错误处理
来源：http://oil.wangshuangyany.cn

do { try f() } catch { print(error) }
来源：http://arf.yuanzhike.top

[T28] Swift：枚举
来源：http://ugc.tian-w.cn

enum Color { case red, green }
来源：http://hni.ydzc1.top

[T29] Swift：guard 提前返回
来源：http://ibk.chenlongwang.top

guard let x = opt else { return }
来源：http://zoc.hnxiangtu.top

[T30] Swift：协议
来源：http://njs.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://dfc.shuidangran.top

[T31] Lua：Hello World
来源：http://zbz.smart0.xyz

print("Hello")
来源：http://bvq.ppjwa.cn

[T32] Lua：局部变量
来源：http://gsc.yonumen.top

local a = 1
来源：http://gob.yvedp.cn

[T33] Lua：表（数组）
来源：http://iog.ivvv.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hng.vehdjk.com

[T34] Lua：遍历表
来源：http://vxd.epnwcf.com

for i, v in ipairs(t) do print(i, v) end
来源：http://npt.chenjidiqi.icu

[T35] Lua：字典表
来源：http://kxk.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://hus.kuanghao11.cn

[T36] Lua：函数
来源：http://ick.vqdsnc.cn

function add(a, b) return a + b end
来源：http://yqk.fanxiaobao.xyz

[T37] Lua：字符串拼接
来源：http://mey.zhongyouzk.top

"a" .. "b"
来源：http://ldg.cucudq.cn

[T38] Lua：条件
来源：http://pvx.yongpay.top

if x > 0 then print("正") end
来源：http://yde.ydjk.org.cn

[T39] Lua：模式匹配
来源：http://ukb.svipenyu.cn

string.find(s, "%d+")
来源：http://grd.ivvv.top

[T40] Lua：元表
来源：http://vxm.cashguo.top

setmetatable({}, { __index = base })
来源：http://sdq.cashguo.top

[T41] Perl：Hello World
来源：http://sjt.shangyingyoupin.top

print "Hello\n";
来源：http://itu.sxryk.cn

[T42] Perl：变量类型
来源：http://glt.zhaomingkeji.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jtl.jyoumei.cn

[T43] Perl：字符串插值
来源：http://law.gzhubu.top

"值: $a"
来源：http://nhq.hywenlv.cn

[T44] Perl：条件
来源：http://bri.cucudq.cn

if ($a > 0) { print "正"; }
来源：http://kvh.jinghuilouyu.cn

[T45] Perl：数组遍历
来源：http://yaw.sweek.top

for my $x (@arr) { print $x; }
来源：http://doa.shangyingyoupin.top

[T46] Perl：哈希操作
来源：http://khi.sufxvd.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ffx.meibo888.top

[T47] Perl：正则捕获
来源：http://tdn.gaohongyu789.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jxc.aizwys.cn

[T48] Perl：正则替换
来源：http://azy.ctjpmb.com

$s =~ s/old/new/g;
来源：http://jka.zhaomingkeji.xyz

[T49] Perl：函数
来源：http://dap.wangshuangyany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nix.ivvv.top

[T50] Perl：逐行读文件
来源：http://vhn.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zfs.yongpay.top

while (my $line = <$fh>) { print $line; }
来源：http://amq.redwolf501.top

[T51] Scala：Hello World
来源：http://qky.yonumen.top

println("Hello")
来源：http://pvx.shanyushiyangkeji.top

[T52] Scala：变量
来源：http://ayo.sufxvd.cn

val a = 1;  var b = 2
来源：http://ijd.epnwcf.com

[T53] Scala：字符串插值
来源：http://een.yj20258888.top

s"值: $b"
来源：http://ati.52xcode.cn

[T54] Scala：集合映射
来源：http://fex.cqqwz.cn

List(1, 2, 3).map(_ * 2)
来源：http://hoi.guowangkeji.top

[T55] Scala：集合过滤
来源：http://xds.tian-w.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ncd.nwbrower.top

[T56] Scala：样例类
来源：http://rxf.sysykeji.top

case class User(name: String, age: Int)
来源：http://kxu.yonumen.top

[T57] Scala：模式匹配
来源：http://wmy.bjfxy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hcr.sufxvd.cn

[T58] Scala：函数定义
来源：http://fnu.birdmap.top

def add(a: Int, b: Int): Int = a + b
来源：http://exs.shuidangran.top

[T59] Scala：循环
来源：http://wmy.feifeiyinyue.top

for (i <- 1 to 10) println(i)
来源：http://zcw.gzhubu.top

[T60] Scala：折叠
来源：http://zkh.havefunace.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jew.snrcjt.cn

================================================================================
来源：http://zgp.sxryk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uqv.xinyue.icu

================================================================================
来源：http://vym.shangyingyoupin.top

[U01] Py：创建虚拟环境
来源：http://dcz.yanxiufei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://llf.feifeiyinyue.top

[U02] Py：导出 / 安装依赖
来源：http://pgi.yueranfly.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mkw.fengsongda.top

[U03] Py：加载 .env 配置
来源：http://nqm.yongpay.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fvf.hnxiangtu.top

[U04] Py：变量调试打印
来源：http://jtq.hywenlv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tcf.mhx1999.top

[U05] Py：列表去重且保序
来源：http://gwy.sweek.top

list(dict.fromkeys(arr))
来源：http://otx.zdqjudy.top

[U06] Py：合并两个字典
来源：http://zqp.tanke756.top

{**a, **b}
来源：http://zwf.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://muq.jyoumei.cn

{v: k for k, v in d.items()}
来源：http://nad.hcnkem.com

[U08] Py：展平二维列表
来源：http://oxi.yj202588.top

[y for x in nested for y in x]
来源：http://zoi.smart0.xyz

[U09] Py：字典取最大值的键
来源：http://joh.fehbvm.com

max(d, key=d.get)
来源：http://hxh.tarul.cn

[U10] Py：按值排序字典
来源：http://onx.hammf.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mvs.jinqigufen.top

[U11] Py：生成器表达式
来源：http://gyx.yanxiufei.cn

(x * 2 for x in arr)
来源：http://wjf.zhengqikj.top

[U12] Py：取出现最多的 3 个元素
来源：http://ikj.daria6918.cn

Counter(arr).most_common(3)
来源：http://heo.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://emo.zhaomingkeji.xyz

deque(maxlen=10)
来源：http://fft.gzhubu.top

[U14] Py：分组收集到列表
来源：http://hgm.xuetiantiany.cn

defaultdict(list)
来源：http://oug.cucudq.cn

[U15] Py：高精度计时
来源：http://zrv.guannengcc.top

t = time.perf_counter()
来源：http://huy.sysykeji.top

[U16] Py：命令行参数解析
来源：http://uba.yanxiufei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fnm.ydjk.org.cn

[U17] Py：初始化日志
来源：http://utk.fengsongda.top

logging.basicConfig(level=logging.INFO)
来源：http://cyo.birdmap.top

[U18] Py：预编译正则
来源：http://foa.hcnkem.com

pat = re.compile(r"\d+")
来源：http://gze.quarkkingdee.top

[U19] Py：正则替换带回调
来源：http://vnz.wangshuangyany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pea.chenlongwang.top

[U20] Py：缓存函数结果
来源：http://yel.jinqigfzy.top

@functools.lru_cache(maxsize=None)
来源：http://lzu.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://prs.hammf.cn

@contextlib.contextmanager
来源：http://kej.hesvh.cn

[U22] Py：矩阵转置
来源：http://bvf.xuanzx.com

list(zip(*m))
来源：http://adb.yanxiufei.cn

[U23] Py：分块读取大文件
来源：http://edq.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sad.cashguo.top

[U24] Py：路径操作
来源：http://zkw.ppjwa.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gxs.cdnleiting.top

[U25] Py：CSV 按字典读
来源：http://huv.nwbrower.top

csv.DictReader(f)
来源：http://fkx.tianlin.xyz

[U26] Py：并发下载
来源：http://wdz.ppjwa.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zts.pycfn.com

[U27] Py：异步 HTTP
来源：http://nsz.jinyuanbaomall.cn

aiohttp.ClientSession() 配合 async with
来源：http://sgn.jianghu66.top

[U28] Py：类型别名
来源：http://fxv.meibo888.top

UserId = int
来源：http://ofe.yueranfly.top

[U29] Py：属性校验
来源：http://rjx.tanke756.top

@property 与 @x.setter 配合
来源：http://vrh.aibaodan.cn

[U30] Py：数据类
来源：http://itf.vehdjk.com

@dataclass(slots=True)
来源：http://gqp.guowangkeji.top

[U31] Py：单测
来源：http://iuc.zhixingplan.top

python -m pytest -q
来源：http://fou.chenzaomai.com

[U32] Py：代码格式化
来源：http://hty.gogol.net.cn

ruff format . && ruff check --fix .
来源：http://xja.wangshuangyany.cn

[U33] Py：打包发布
来源：http://qpy.zhiwuduotai.top

python -m build  （依赖 pyproject.toml）
来源：http://ook.yj202588.top

[U34] Py：判断编码
来源：http://fuo.sxryk.cn

chardet.detect(raw)
来源：http://mid.chenjidiqi.icu

[U35] Py：发送邮件
来源：http://wrd.nwbrower.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fcw.smart0.xyz

[U36] Py：定时任务
来源：http://gub.yonumen.top

schedule.every(10).minutes.do(job)
来源：http://hpq.hfpthk.cn

[U37] Py：读写 Excel
来源：http://hnk.hammf.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pjx.dashuyun.cn

[U38] Py：获取脚本所在目录
来源：http://gag.guannengcc.top

Path(__file__).resolve().parent
来源：http://njg.ywan-chungtsiang.top

[U39] Py：判断是否在交互环境
来源：http://sgh.sweek.top

sys.stdout.isatty()
来源：http://xrw.shanyushiyangkeji.top

[U40] Py：打印到标准错误
来源：http://frl.hnqzz.top

print("err", file=sys.stderr)
来源：http://iqh.yj20258888.top

[U41] PHP：初始化 Composer 项目
来源：http://twh.shanyushiyangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wdq.dianchejie.cn

[U42] PHP：PSR-4 自动加载
来源：http://obd.jinyuanbaomall.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gqe.xuanzx.com

[U43] PHP：声明命名空间
来源：http://bog.feifeiyinyue.top

namespace App\Http;
来源：http://qds.tanke756.top

[U44] PHP：开启严格类型
来源：http://spv.birdmap.top

declare(strict_types=1);
来源：http://kwt.yongpay.top

[U45] PHP：类型声明与返回类型
来源：http://hhq.tarul.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zti.tarul.cn

[U46] PHP：可空类型
来源：http://qew.bjfxy.top

?string $name = null
来源：http://kmg.xuanzx.com

[U47] PHP：联合类型
来源：http://loe.chenjidiqi.icu

int|string $id
来源：http://dnv.smart0.xyz

[U48] PHP：纯枚举
来源：http://elq.nwbrower.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kha.xuanzx.com

[U49] PHP：只读属性
来源：http://tcg.jinghuilouyu.cn

public readonly string $name
来源：http://mco.yj20258888.top

[U50] PHP：构造器属性提升
来源：http://tdx.cashguo.top

public function __construct(private int $id) {}
来源：http://jbe.kuanghao11.cn

[U51] PHP：数组解构
来源：http://ynp.zycfv.cn

[$a, $b] = $arr;
来源：http://mot.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://yfm.gzhubu.top

$double = fn($x) => $x * 2;
来源：http://wwb.ydjk.org.cn

[U53] PHP：空合并运算符
来源：http://mib.bbcook.cn

$v = $a ?? $b ?? "default";
来源：http://xre.jyoumei.cn

[U54] PHP：空安全调用
来源：http://njp.shangyingyoupin.top

$obj?->method()
来源：http://ssc.snrcjt.cn

[U55] PHP：match 表达式
来源：http://ogb.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ytt.xingfuxueyuan.xyz

[U56] PHP：命名参数
来源：http://hma.jqgufenzy.top

f(a: 1, b: 2)
来源：http://rrk.hfpthk.cn

[U57] PHP：字符串插值
来源：http://yaw.cucudq.cn

"值: {$a}"
来源：http://iop.xuanzx.com

[U58] PHP：数组三件套
来源：http://tzm.ivvv.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hqa.daria6918.cn

[U59] PHP：自定义排序
来源：http://rih.yj20258888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yee.xuetiantiany.cn

[U60] PHP：JSON 编解码
来源：http://aue.hnqzz.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lxo.hnqzz.top

[U61] PHP：正则
来源：http://omc.xylfe.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nsy.fktsv.cn

[U62] PHP：日期对象
来源：http://tdx.sxryk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://teb.xingfuxueyuan.xyz

[U63] PHP：文件读写
来源：http://vyc.zdqjudy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ekz.sysykeji.top

[U64] PHP：目录遍历
来源：http://hqc.bbcook.cn

glob("dir/*.php");  scandir("dir");
来源：http://swc.guannengcc.top

[U65] PHP：会话
来源：http://ikc.ctjpmb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://vtb.ywan-chungtsiang.top

[U66] PHP：设置 Cookie
来源：http://cmg.ydzc1.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rdt.vqdsnc.cn

[U67] PHP：处理文件上传
来源：http://bcp.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vnp.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://wjo.ctjpmb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://roa.0kj1m.cn

[U69] PHP：PDO 预处理
来源：http://rna.tian-w.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kpp.daxiang520.top

[U70] PHP：PDO 事务
来源：http://fdj.pycfn.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uvz.jqgfzy.top

[U71] PHP：抛出异常
来源：http://oqk.wangshuangyany.cn

throw new RuntimeException("失败", 500);
来源：http://jzq.ywan-chungtsiang.top

[U72] PHP：写错误日志
来源：http://plz.pengpengdd.cyou

error_log("失败: " . $e->getMessage());
来源：http://mve.shuidangran.top

[U73] PHP：读取 ini 配置
来源：http://oqc.gotoacloud.top

parse_ini_file("config.ini", true)
来源：http://vud.yonumen.top

[U74] PHP：读取环境变量
来源：http://tal.hnxiangtu.top

getenv("APP_ENV") ?: "production"
来源：http://hqk.tarul.cn

[U75] PHP：依赖注入
来源：http://wqs.shanyushiyangkeji.top

composer require psr/container
来源：http://aoa.chenjidiqi.icu

[U76] PHP：简单路由
来源：http://elg.zhengqikj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ltp.jqgfzy.top

[U77] PHP：模板渲染
来源：http://qvr.shzxlz.cn

composer require twig/twig
来源：http://ucw.yvedp.cn

[U78] PHP：单元测试
来源：http://vso.guowangkeji.top

composer require --dev phpunit/phpunit
来源：http://vkw.gotoacloud.top

[U79] PHP：静态分析
来源：http://dlb.gogol.net.cn

composer require --dev phpstan/phpstan
来源：http://qtk.chenlongwang.top

[U80] PHP：代码规范修复
来源：http://smj.epnwcf.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://zim.jinghuilouyu.cn

[U81] JS：初始化项目
来源：http://hbv.vqdsnc.cn

npm init -y;  npm i express
来源：http://ode.ywan-chungtsiang.top

[U82] JS：package.json 脚本
来源：http://frt.hammf.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://itl.shanyushiyangtech.top

[U83] JS：ES Module 导入导出
来源：http://drx.yvedp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xlb.xingfuxueyuan.xyz

[U84] JS：CommonJS 写法
来源：http://igc.jinghuilouyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mng.ywan-chungtsiang.top

[U85] JS：可选链
来源：http://ypp.ppjwa.cn

a?.b?.c
来源：http://kwn.dianchejie.cn

[U86] JS：空值合并
来源：http://sre.c1oappe.top

a ?? b
来源：http://qyi.cheryme.top

[U87] JS：解构默认值
来源：http://roz.yuanzhike.top

const { a = 1, b = 2 } = obj;
来源：http://ppx.ydjk.org.cn

[U88] JS：对象展开合并
来源：http://nez.tianlin.xyz

{ ...a, ...b }
来源：http://yem.zdqjudy.top

[U89] JS：数组去重
来源：http://qeq.jinqigufen.top

[...new Set(arr)]
来源：http://ian.ehwqpu.com

[U90] JS：数字数组排序
来源：http://gou.ivvv.top

[...arr].sort((a, b) => a - b)
来源：http://kqf.chenjidiqi.icu

[U91] JS：对象键值遍历
来源：http://cyu.yj20258888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ksv.tian-w.cn

[U92] JS：深拷贝
来源：http://tnm.snrcjt.cn

structuredClone(obj)
来源：http://jtn.tianlin.xyz

[U93] JS：模板字符串
来源：http://mmg.jiagoushi.top

`共 ${n} 条`
来源：http://bwr.cqqwz.cn

[U94] JS：箭头函数
来源：http://ncm.cashguo.top

const double = x => x * 2;
来源：http://zlt.jinqigfzy.top

[U95] JS：Promise 包装
来源：http://oez.tianlin.xyz

new Promise((resolve, reject) => {})
来源：http://fri.svipenyu.cn

[U96] JS：async/await 与异常
来源：http://twc.sufxvd.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://biq.316326.xyz

[U97] JS：并发请求
来源：http://ohe.yuxming.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://svx.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://nyx.dianchejie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xxk.yuxming.cn

[U99] JS：事件监听
来源：http://zmk.sweek.top

el.addEventListener("click", e => {})
来源：http://qht.316326.xyz

[U100] JS：DOM 查询
来源：http://nah.shangyingyoupin.top

document.querySelector(".item")
来源：http://lzt.wangshuangyany.cn

[U101] JS：classList 操作
来源：http://iyw.gzhubu.top

el.classList.toggle("active")
来源：http://nkz.pycfn.com

[U102] JS：本地存储
来源：http://vfn.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://hrm.quarkkingdee.top

[U103] JS：定时器
来源：http://wup.jianghu66.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lnl.ydzc1.top

[U104] JS：防抖
来源：http://kxe.fanxiaobao.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yar.svipenyu.cn

[U105] JS：节流
来源：http://aoi.ehwqpu.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://twz.ywan-chungtsiang.top

[U106] JS：日期格式化
来源：http://vru.uphjek.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tsq.xziqi.cn

[U107] JS：数字千分位
来源：http://qds.sweek.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://clv.havefunace.top

[U108] JS：随机整数
来源：http://knv.sxryk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rkj.yj20258.top

[U109] JS：数组分组
来源：http://cij.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://ycx.zdqjudy.top

[U110] JS：数组分块
来源：http://ixh.wangshuangyany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hax.hcnkem.com


<!-- 参考信息 -->