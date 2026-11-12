代发 wailian999

[T23] Swift：函数
来源：http://bln.dianchejie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://una.smart0.xyz

[T24] Swift：闭包
来源：http://bau.hnqzz.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bth.ppjwa.cn

[T25] Swift：结构体
来源：http://itd.fzhhl.top

struct P { var x: Int }
来源：http://wdz.yuxming.cn

[T26] Swift：类与重写
来源：http://nby.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://rgh.andypj.xyz

[T27] Swift：错误处理
来源：http://qaw.ppjwa.cn

do { try f() } catch { print(error) }
来源：http://oyb.jinghuilouyu.cn

[T28] Swift：枚举
来源：http://xvx.tarul.cn

enum Color { case red, green }
来源：http://fmn.fengsongda.top

[T29] Swift：guard 提前返回
来源：http://dmr.yj20258.top

guard let x = opt else { return }
来源：http://oco.quarkkingdee.top

[T30] Swift：协议
来源：http://bfo.yanxiufei.cn

protocol Shape { func area() -> Double }
来源：http://imf.ppjwa.cn

[T31] Lua：Hello World
来源：http://vjk.fzhhl.top

print("Hello")
来源：http://hcp.jlsjyb.cn

[T32] Lua：局部变量
来源：http://wxa.shanyushiyangkeji.top

local a = 1
来源：http://djv.jinyuanbaomall.cn

[T33] Lua：表（数组）
来源：http://inl.redwolf501.top

local t = {1, 2, 3};  t[4] = 4
来源：http://eak.yj20258.top

[T34] Lua：遍历表
来源：http://pfq.nanxuanxn.top

for i, v in ipairs(t) do print(i, v) end
来源：http://icm.chenjidiqi.icu

[T35] Lua：字典表
来源：http://uxn.zhaomingkeji.xyz

local d = { a = 1 };  d.b = 2
来源：http://pkn.jqgfzy.top

[T36] Lua：函数
来源：http://vpm.yuxming.cn

function add(a, b) return a + b end
来源：http://sok.fehbvm.com

[T37] Lua：字符串拼接
来源：http://qha.zdbjq.cn

"a" .. "b"
来源：http://zom.nanxuanxn.top

[T38] Lua：条件
来源：http://hox.tanke756.top

if x > 0 then print("正") end
来源：http://ivp.havefunace.top

[T39] Lua：模式匹配
来源：http://dit.jinqigfzy.top

string.find(s, "%d+")
来源：http://kma.pycfn.com

[T40] Lua：元表
来源：http://mcs.ppjwa.cn

setmetatable({}, { __index = base })
来源：http://jmh.daxiang520.top

[T41] Perl：Hello World
来源：http://ozn.yangfankeji.com

print "Hello\n";
来源：http://rui.yuxming.cn

[T42] Perl：变量类型
来源：http://idj.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hkh.redwolf501.top

[T43] Perl：字符串插值
来源：http://pfk.nwbrower.top

"值: $a"
来源：http://ccr.ehwqpu.com

[T44] Perl：条件
来源：http://tox.dianchejie.cn

if ($a > 0) { print "正"; }
来源：http://mwz.nanxinkj.top

[T45] Perl：数组遍历
来源：http://gjc.ppjwa.cn

for my $x (@arr) { print $x; }
来源：http://irz.kuanghao11.cn

[T46] Perl：哈希操作
来源：http://kfe.uphjek.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://agy.xylfe.cn

[T47] Perl：正则捕获
来源：http://kkb.gzhubu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rbq.meibo888.top

[T48] Perl：正则替换
来源：http://fjp.aibaodan.cn

$s =~ s/old/new/g;
来源：http://owf.ybcxt.top

[T49] Perl：函数
来源：http://pqz.epnwcf.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qcc.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://uqz.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gkl.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://spt.yj202588.top

[T51] Scala：Hello World
来源：http://yox.tarul.cn

println("Hello")
来源：http://eee.hywenlv.cn

[T52] Scala：变量
来源：http://zlp.ivvv.top

val a = 1;  var b = 2
来源：http://mrh.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://bjc.shzxlz.cn

s"值: $b"
来源：http://sny.xylfe.cn

[T54] Scala：集合映射
来源：http://nou.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://chj.andypj.xyz

[T55] Scala：集合过滤
来源：http://orz.mhx1999.top

List(1, 2, 3).filter(_ > 1)
来源：http://efo.birdmap.top

[T56] Scala：样例类
来源：http://rtf.tanke756.top

case class User(name: String, age: Int)
来源：http://sgi.xziqi.cn

[T57] Scala：模式匹配
来源：http://tmg.pycfn.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://uop.dianchejie.cn

[T58] Scala：函数定义
来源：http://hhh.quarkkingdee.top

def add(a: Int, b: Int): Int = a + b
来源：http://evh.zhoulong.xyz

[T59] Scala：循环
来源：http://btl.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://czo.ydjk.org.cn

[T60] Scala：折叠
来源：http://hsu.0kj1m.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eij.316326.xyz

================================================================================
来源：http://hcf.ctjpmb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://crm.tianlin.xyz

================================================================================
来源：http://axi.svipenyu.cn

[U01] Py：创建虚拟环境
来源：http://riy.tianlin.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://ivd.wangshuangyany.cn

[U02] Py：导出 / 安装依赖
来源：http://irm.fengsongda.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zll.bjfxy.top

[U03] Py：加载 .env 配置
来源：http://lqg.fktsv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://faw.jiagoushi.top

[U04] Py：变量调试打印
来源：http://zia.cucudq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://noo.yvedp.cn

[U05] Py：列表去重且保序
来源：http://zzl.xuetiantiany.cn

list(dict.fromkeys(arr))
来源：http://olr.fehbvm.com

[U06] Py：合并两个字典
来源：http://fbx.nwbrower.top

{**a, **b}
来源：http://odm.jinqigufen.top

[U07] Py：反转字典键值
来源：http://xsu.fzhhl.top

{v: k for k, v in d.items()}
来源：http://upb.316326.xyz

[U08] Py：展平二维列表
来源：http://fej.sxryk.cn

[y for x in nested for y in x]
来源：http://gdd.zdbjq.cn

[U09] Py：字典取最大值的键
来源：http://ktf.sysykeji.top

max(d, key=d.get)
来源：http://jod.zhiwuduotai.top

[U10] Py：按值排序字典
来源：http://mww.zhijiandao.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aop.zhoulong.xyz

[U11] Py：生成器表达式
来源：http://gkm.pycfn.com

(x * 2 for x in arr)
来源：http://ivd.gogol.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xbo.hcnkem.com

Counter(arr).most_common(3)
来源：http://uxa.vehdjk.com

[U13] Py：固定长度队列
来源：http://ymn.tianlin.xyz

deque(maxlen=10)
来源：http://avp.sysykeji.top

[U14] Py：分组收集到列表
来源：http://kbi.snrcjt.cn

defaultdict(list)
来源：http://qnu.jlsjyb.cn

[U15] Py：高精度计时
来源：http://rki.yongpay.top

t = time.perf_counter()
来源：http://byy.cdnleiting.top

[U16] Py：命令行参数解析
来源：http://vov.haohaochexian.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mif.xuetiantiany.cn

[U17] Py：初始化日志
来源：http://pda.chenjidiqi.icu

logging.basicConfig(level=logging.INFO)
来源：http://oyv.ppjwa.cn

[U18] Py：预编译正则
来源：http://lpq.hnxiangtu.top

pat = re.compile(r"\d+")
来源：http://axl.bjfxy.top

[U19] Py：正则替换带回调
来源：http://zpg.ydzc1.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hms.zhaomingkeji.xyz

[U20] Py：缓存函数结果
来源：http://wld.pycfn.com

@functools.lru_cache(maxsize=None)
来源：http://cys.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://zyg.aizwys.cn

@contextlib.contextmanager
来源：http://bub.yvedp.cn

[U22] Py：矩阵转置
来源：http://ygk.uphjek.com

list(zip(*m))
来源：http://kzr.yonumen.top

[U23] Py：分块读取大文件
来源：http://pqa.sxryk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sxn.svipenyu.cn

[U24] Py：路径操作
来源：http://zjq.jqgufenzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ily.jqgufenzy.top

[U25] Py：CSV 按字典读
来源：http://yty.jqgufenzy.top

csv.DictReader(f)
来源：http://qax.yvedp.cn

[U26] Py：并发下载
来源：http://vrg.yueranfly.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bkd.fzhhl.top

[U27] Py：异步 HTTP
来源：http://pqi.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://uea.jyoumei.cn

[U28] Py：类型别名
来源：http://orc.aibaodan.cn

UserId = int
来源：http://yng.ctjpmb.com

[U29] Py：属性校验
来源：http://mkk.svipenyu.cn

@property 与 @x.setter 配合
来源：http://qgp.cucudq.cn

[U30] Py：数据类
来源：http://inc.tanke756.top

@dataclass(slots=True)
来源：http://cba.sufxvd.cn

[U31] Py：单测
来源：http://urh.yuxming.cn

python -m pytest -q
来源：http://hmp.hnxiangtu.top

[U32] Py：代码格式化
来源：http://vug.shanyushiyangtech.top

ruff format . && ruff check --fix .
来源：http://apr.hnqzz.top

[U33] Py：打包发布
来源：http://qyn.hywenlv.cn

python -m build  （依赖 pyproject.toml）
来源：http://anx.tanke756.top

[U34] Py：判断编码
来源：http://cfd.sjlbkw.cn

chardet.detect(raw)
来源：http://sqm.jinyuanbaomall.cn

[U35] Py：发送邮件
来源：http://tvf.hywenlv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kkv.shuidangran.top

[U36] Py：定时任务
来源：http://ipp.tanke756.top

schedule.every(10).minutes.do(job)
来源：http://txn.epnwcf.com

[U37] Py：读写 Excel
来源：http://gsb.hnxiangtu.top

pandas.read_excel / DataFrame.to_excel
来源：http://why.bbcook.cn

[U38] Py：获取脚本所在目录
来源：http://dmr.sjlbkw.cn

Path(__file__).resolve().parent
来源：http://wjs.zhiwuduotai.top

[U39] Py：判断是否在交互环境
来源：http://vob.wangdashe.top

sys.stdout.isatty()
来源：http://hbe.yongpay.top

[U40] Py：打印到标准错误
来源：http://yhw.yfazqb.com

print("err", file=sys.stderr)
来源：http://via.pycfn.com

[U41] PHP：初始化 Composer 项目
来源：http://run.zhongyouzk.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qjd.shangyingyoupin.top

[U42] PHP：PSR-4 自动加载
来源：http://nyt.shanyushiyangtech.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://atb.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://xwu.guannengcc.top

namespace App\Http;
来源：http://kra.haohaochexian.top

[U44] PHP：开启严格类型
来源：http://hky.xuetiantiany.cn

declare(strict_types=1);
来源：http://vbd.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://evc.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lwk.redwolf501.top

[U46] PHP：可空类型
来源：http://pll.hcnkem.com

?string $name = null
来源：http://ixq.316326.xyz

[U47] PHP：联合类型
来源：http://cnm.haohaochexian.top

int|string $id
来源：http://gpx.xingfuxueyuan.xyz

[U48] PHP：纯枚举
来源：http://kvp.yj202588.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zff.xziqi.cn

[U49] PHP：只读属性
来源：http://lzs.yvedp.cn

public readonly string $name
来源：http://iaa.cdnleiting.top

[U50] PHP：构造器属性提升
来源：http://zyf.pycfn.com

public function __construct(private int $id) {}
来源：http://khi.fehbvm.com

[U51] PHP：数组解构
来源：http://jco.xuanzx.com

[$a, $b] = $arr;
来源：http://isi.guowangkeji.top

[U52] PHP：箭头函数
来源：http://qfx.ctjpmb.com

$double = fn($x) => $x * 2;
来源：http://jfv.yj202588.top

[U53] PHP：空合并运算符
来源：http://jho.epnwcf.com

$v = $a ?? $b ?? "default";
来源：http://kau.ctjpmb.com

[U54] PHP：空安全调用
来源：http://iha.nanxinkj.top

$obj?->method()
来源：http://ftp.fengsongda.top

[U55] PHP：match 表达式
来源：http://fms.zhixingplan.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oer.pycfn.com

[U56] PHP：命名参数
来源：http://itq.ydjk.org.cn

f(a: 1, b: 2)
来源：http://nkx.svipenyu.cn

[U57] PHP：字符串插值
来源：http://sny.shanyushiyangtech.top

"值: {$a}"
来源：http://pux.jinqigfzy.top

[U58] PHP：数组三件套
来源：http://omd.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pck.xinyue.icu

[U59] PHP：自定义排序
来源：http://ygj.316326.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yfn.zycfv.cn

[U60] PHP：JSON 编解码
来源：http://nem.zycfv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://axq.0kj1m.cn

[U61] PHP：正则
来源：http://igq.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mml.hnqzz.top

[U62] PHP：日期对象
来源：http://npm.zdbjq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zil.sysykeji.top

[U63] PHP：文件读写
来源：http://gex.jlsjyb.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vna.hysaishi.cn

[U64] PHP：目录遍历
来源：http://anw.sweek.top

glob("dir/*.php");  scandir("dir");
来源：http://jlb.vqdsnc.cn

[U65] PHP：会话
来源：http://zjc.haohaochexian.top

session_start();  $_SESSION["uid"] = 1;
来源：http://azu.bbcook.cn

[U66] PHP：设置 Cookie
来源：http://dsa.zhoulong.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gll.gogol.net.cn

[U67] PHP：处理文件上传
来源：http://jiu.pycfn.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lhl.gzhubu.top

[U68] PHP：PDO 连接
来源：http://wpx.cdnleiting.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://evk.hywenlv.cn

[U69] PHP：PDO 预处理
来源：http://dpt.cashguo.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fdv.nanxuanxn.top

[U70] PHP：PDO 事务
来源：http://etb.haohaochexian.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fko.yj202588.top

[U71] PHP：抛出异常
来源：http://orf.0kj1m.cn

throw new RuntimeException("失败", 500);
来源：http://mgi.c1oappe.top

[U72] PHP：写错误日志
来源：http://tqd.ivvv.top

error_log("失败: " . $e->getMessage());
来源：http://fix.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://hhg.nanxinkj.top

parse_ini_file("config.ini", true)
来源：http://nbx.zhaomingkeji.xyz

[U74] PHP：读取环境变量
来源：http://jkx.daxiang520.top

getenv("APP_ENV") ?: "production"
来源：http://gpa.ivvv.top

[U75] PHP：依赖注入
来源：http://gpj.aizwys.cn

composer require psr/container
来源：http://jjv.daria6918.cn

[U76] PHP：简单路由
来源：http://tbv.gzhubu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://llb.ydzc1.top

[U77] PHP：模板渲染
来源：http://nkt.ydjk.org.cn

composer require twig/twig
来源：http://ari.bjfxy.top

[U78] PHP：单元测试
来源：http://nmi.yanxiufei.cn

composer require --dev phpunit/phpunit
来源：http://lml.cucudq.cn

[U79] PHP：静态分析
来源：http://sog.9152youxi.cn

composer require --dev phpstan/phpstan
来源：http://woi.aibaodan.cn

[U80] PHP：代码规范修复
来源：http://zxr.guowangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ksi.nanxuanxn.top

[U81] JS：初始化项目
来源：http://igy.daria6918.cn

npm init -y;  npm i express
来源：http://ovm.feifeiyinyue.top

[U82] JS：package.json 脚本
来源：http://ovp.hnxiangtu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zyu.zhongyouzk.top

[U83] JS：ES Module 导入导出
来源：http://ktv.tian-w.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yoy.yvedp.cn

[U84] JS：CommonJS 写法
来源：http://ogc.kuanghao11.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qmh.sxryk.cn

[U85] JS：可选链
来源：http://nhp.yfazqb.com

a?.b?.c
来源：http://dwt.tanke756.top

[U86] JS：空值合并
来源：http://avx.zhixingplan.top

a ?? b
来源：http://wcb.ybcxt.top

[U87] JS：解构默认值
来源：http://tgg.wangshuangyany.cn

const { a = 1, b = 2 } = obj;
来源：http://xie.xuanzx.com

[U88] JS：对象展开合并
来源：http://rey.cheryme.top

{ ...a, ...b }
来源：http://vyn.yueranfly.top

[U89] JS：数组去重
来源：http://tiq.gogol.net.cn

[...new Set(arr)]
来源：http://uap.pycfn.com

[U90] JS：数字数组排序
来源：http://cey.gogol.net.cn

[...arr].sort((a, b) => a - b)
来源：http://yrd.tanke756.top

[U91] JS：对象键值遍历
来源：http://jtz.xylfe.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zrc.yuxming.cn

[U92] JS：深拷贝
来源：http://tpj.yueranfly.top

structuredClone(obj)
来源：http://hhk.ybcxt.top

[U93] JS：模板字符串
来源：http://jiu.hnqzz.top

`共 ${n} 条`
来源：http://wrb.snrcjt.cn

[U94] JS：箭头函数
来源：http://xrf.sufxvd.cn

const double = x => x * 2;
来源：http://joj.nanxuanxn.top

[U95] JS：Promise 包装
来源：http://pkb.quarkkingdee.top

new Promise((resolve, reject) => {})
来源：http://gkz.yfazqb.com

[U96] JS：async/await 与异常
来源：http://rqg.52xcode.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://skh.feifeiyinyue.top

[U97] JS：并发请求
来源：http://taw.xuetiantiany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ltv.zhengqikj.top

[U98] JS：fetch 带 JSON
来源：http://bpv.ehwqpu.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uzq.hysaishi.cn

[U99] JS：事件监听
来源：http://zqi.shuidangran.top

el.addEventListener("click", e => {})
来源：http://saw.yuanzhike.top

[U100] JS：DOM 查询
来源：http://zzl.jqgfzy.top

document.querySelector(".item")
来源：http://rjh.yongpay.top

[U101] JS：classList 操作
来源：http://oug.jinyuanbaomall.cn

el.classList.toggle("active")
来源：http://ari.sufxvd.cn

[U102] JS：本地存储
来源：http://wgm.jyoumei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jnp.xuanzx.com

[U103] JS：定时器
来源：http://spr.c1oappe.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xtk.aizwys.cn

[U104] JS：防抖
来源：http://icx.xuetiantiany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jde.iojbl.cn

[U105] JS：节流
来源：http://civ.wangdashe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tqk.yfazqb.com

[U106] JS：日期格式化
来源：http://xms.xinyue.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cxg.9152youxi.cn

[U107] JS：数字千分位
来源：http://mag.feifeiyinyue.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vqy.uphjek.com

[U108] JS：随机整数
来源：http://raf.tianlin.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lhm.quarkkingdee.top

[U109] JS：数组分组
来源：http://ots.aibaodan.cn

Object.groupBy(arr, x => x.type)
来源：http://vld.jqgufenzy.top

[U110] JS：数组分块
来源：http://kft.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qaq.haohaochexian.top


<!-- 参考信息 -->