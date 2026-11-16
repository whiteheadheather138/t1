代发 wailian999

[T31] Lua：Hello World
来源：http://vxv.pengpengdd.cyou

print("Hello")
来源：http://upe.chenjidiqi.icu

[T32] Lua：局部变量
来源：http://ahu.feifeiyinyue.top

local a = 1
来源：http://blz.c1oappe.top

[T33] Lua：表（数组）
来源：http://kvk.xinyue.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://ylv.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://efd.shangyingyoupin.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xvi.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://syj.c1oappe.top

local d = { a = 1 };  d.b = 2
来源：http://qwm.shzxlz.cn

[T36] Lua：函数
来源：http://jcr.52xcode.cn

function add(a, b) return a + b end
来源：http://wmq.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://klr.yfazqb.com

"a" .. "b"
来源：http://uwf.ivvv.top

[T38] Lua：条件
来源：http://jcn.hcnkem.com

if x > 0 then print("正") end
来源：http://hje.yvedp.cn

[T39] Lua：模式匹配
来源：http://arl.kuanghao11.cn

string.find(s, "%d+")
来源：http://tzb.fehbvm.com

[T40] Lua：元表
来源：http://jel.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://pni.bjfxy.top

[T41] Perl：Hello World
来源：http://etz.ctjpmb.com

print "Hello\n";
来源：http://ava.ydjk.org.cn

[T42] Perl：变量类型
来源：http://lkf.fehbvm.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jrp.iojbl.cn

[T43] Perl：字符串插值
来源：http://sdd.haohaochexian.top

"值: $a"
来源：http://hkx.xinyue.icu

[T44] Perl：条件
来源：http://awg.9152youxi.cn

if ($a > 0) { print "正"; }
来源：http://ywt.pengpengdd.cyou

[T45] Perl：数组遍历
来源：http://fmo.shuidangran.top

for my $x (@arr) { print $x; }
来源：http://zzi.xylfe.cn

[T46] Perl：哈希操作
来源：http://qur.zhaomingkeji.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kfh.9152youxi.cn

[T47] Perl：正则捕获
来源：http://rof.jqgfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yaq.zdbjq.cn

[T48] Perl：正则替换
来源：http://kfc.haohaochexian.top

$s =~ s/old/new/g;
来源：http://wix.vehdjk.com

[T49] Perl：函数
来源：http://lwc.shuidangran.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bxy.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://duf.wangdashe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qfx.haohaochexian.top

while (my $line = <$fh>) { print $line; }
来源：http://yfu.chenzaomai.com

[T51] Scala：Hello World
来源：http://iau.bjfxy.top

println("Hello")
来源：http://ebi.jlsjyb.cn

[T52] Scala：变量
来源：http://irt.sjlbkw.cn

val a = 1;  var b = 2
来源：http://xpf.ybcxt.top

[T53] Scala：字符串插值
来源：http://qhz.nwbrower.top

s"值: $b"
来源：http://oqe.hongshengwenyu.top

[T54] Scala：集合映射
来源：http://tom.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://dqy.chenjidiqi.icu

[T55] Scala：集合过滤
来源：http://sby.guannengcc.top

List(1, 2, 3).filter(_ > 1)
来源：http://ujg.redwolf501.top

[T56] Scala：样例类
来源：http://zby.cashguo.top

case class User(name: String, age: Int)
来源：http://jpg.cucudq.cn

[T57] Scala：模式匹配
来源：http://gwl.shuidangran.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zze.hywenlv.cn

[T58] Scala：函数定义
来源：http://sht.ybcxt.top

def add(a: Int, b: Int): Int = a + b
来源：http://zjt.tarul.cn

[T59] Scala：循环
来源：http://mvk.cucudq.cn

for (i <- 1 to 10) println(i)
来源：http://cjs.xingfuxueyuan.xyz

[T60] Scala：折叠
来源：http://ftd.jinqigfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hed.chenzaomai.com

================================================================================
来源：http://cvj.fehbvm.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://njd.pengpengdd.cyou

================================================================================
来源：http://vtu.zycfv.cn

[U01] Py：创建虚拟环境
来源：http://aja.smart0.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://bus.dashuyun.cn

[U02] Py：导出 / 安装依赖
来源：http://syp.quarkkingdee.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dqx.zhijiandao.cn

[U03] Py：加载 .env 配置
来源：http://lbl.shuidangran.top

from dotenv import load_dotenv; load_dotenv()
来源：http://znp.aizwys.cn

[U04] Py：变量调试打印
来源：http://qmz.wangdashe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://brv.daxiang520.top

[U05] Py：列表去重且保序
来源：http://gev.zhijiandao.cn

list(dict.fromkeys(arr))
来源：http://pec.epnwcf.com

[U06] Py：合并两个字典
来源：http://vrx.jinqigufen.top

{**a, **b}
来源：http://mpq.ehwqpu.com

[U07] Py：反转字典键值
来源：http://dfm.chenlongwang.top

{v: k for k, v in d.items()}
来源：http://xmp.epnwcf.com

[U08] Py：展平二维列表
来源：http://syl.nanxuanxn.top

[y for x in nested for y in x]
来源：http://fcd.cqqwz.cn

[U09] Py：字典取最大值的键
来源：http://uqh.xuanzx.com

max(d, key=d.get)
来源：http://mdk.52xcode.cn

[U10] Py：按值排序字典
来源：http://udj.cucudq.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lza.cucudq.cn

[U11] Py：生成器表达式
来源：http://qbc.xuetiantiany.cn

(x * 2 for x in arr)
来源：http://cyk.yuanzhike.top

[U12] Py：取出现最多的 3 个元素
来源：http://dwr.yueranfly.top

Counter(arr).most_common(3)
来源：http://azk.wangdashe.top

[U13] Py：固定长度队列
来源：http://bsa.hongshengwenyu.top

deque(maxlen=10)
来源：http://pwv.hesvh.cn

[U14] Py：分组收集到列表
来源：http://qwx.jqgfzy.top

defaultdict(list)
来源：http://vxq.jinqigfzy.top

[U15] Py：高精度计时
来源：http://awk.uphjek.com

t = time.perf_counter()
来源：http://emn.fehbvm.com

[U16] Py：命令行参数解析
来源：http://zgr.fzhhl.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dds.kuanghao11.cn

[U17] Py：初始化日志
来源：http://wdm.fzhhl.top

logging.basicConfig(level=logging.INFO)
来源：http://ghc.aibaodan.cn

[U18] Py：预编译正则
来源：http://bxa.jianghu66.top

pat = re.compile(r"\d+")
来源：http://tzi.hysaishi.cn

[U19] Py：正则替换带回调
来源：http://lct.ppjwa.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ufk.snrcjt.cn

[U20] Py：缓存函数结果
来源：http://tzl.xziqi.cn

@functools.lru_cache(maxsize=None)
来源：http://het.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://qhg.haohaochexian.top

@contextlib.contextmanager
来源：http://zrl.zhoulong.xyz

[U22] Py：矩阵转置
来源：http://hjv.hongshengwenyu.top

list(zip(*m))
来源：http://ykm.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://rrz.cheryme.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qty.jqgfzy.top

[U24] Py：路径操作
来源：http://dtv.tarul.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://isy.jyoumei.cn

[U25] Py：CSV 按字典读
来源：http://xgz.snrcjt.cn

csv.DictReader(f)
来源：http://tie.yuanzhike.top

[U26] Py：并发下载
来源：http://ykp.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bjl.havefunace.top

[U27] Py：异步 HTTP
来源：http://jdm.yj202588.top

aiohttp.ClientSession() 配合 async with
来源：http://pyi.fehbvm.com

[U28] Py：类型别名
来源：http://mci.jinqigfzy.top

UserId = int
来源：http://ded.jinqigufen.top

[U29] Py：属性校验
来源：http://dbh.tarul.cn

@property 与 @x.setter 配合
来源：http://nad.gzhubu.top

[U30] Py：数据类
来源：http://qje.pycfn.com

@dataclass(slots=True)
来源：http://osk.andypj.xyz

[U31] Py：单测
来源：http://efr.nanxinkj.top

python -m pytest -q
来源：http://tif.chenlongwang.top

[U32] Py：代码格式化
来源：http://oyq.jianghu66.top

ruff format . && ruff check --fix .
来源：http://ggy.epnwcf.com

[U33] Py：打包发布
来源：http://fsh.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://wjq.zhixingplan.top

[U34] Py：判断编码
来源：http://vqc.fehbvm.com

chardet.detect(raw)
来源：http://fgr.guowangkeji.top

[U35] Py：发送邮件
来源：http://htv.aibaodan.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wgo.jinqigufen.top

[U36] Py：定时任务
来源：http://ajq.ctjpmb.com

schedule.every(10).minutes.do(job)
来源：http://nft.jinqigufen.top

[U37] Py：读写 Excel
来源：http://voe.xziqi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ugh.nanxuanxn.top

[U38] Py：获取脚本所在目录
来源：http://bdf.birdmap.top

Path(__file__).resolve().parent
来源：http://swk.zhijiandao.cn

[U39] Py：判断是否在交互环境
来源：http://czb.zdqjudy.top

sys.stdout.isatty()
来源：http://vbm.hesvh.cn

[U40] Py：打印到标准错误
来源：http://nue.jinyuanbaomall.cn

print("err", file=sys.stderr)
来源：http://wtw.xuetiantiany.cn

[U41] PHP：初始化 Composer 项目
来源：http://oyx.jinqigufen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://psi.zdbjq.cn

[U42] PHP：PSR-4 自动加载
来源：http://ztz.jinqigfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://avo.0kj1m.cn

[U43] PHP：声明命名空间
来源：http://abp.shangyingyoupin.top

namespace App\Http;
来源：http://vcp.ctjpmb.com

[U44] PHP：开启严格类型
来源：http://jfk.pycfn.com

declare(strict_types=1);
来源：http://nny.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://iej.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nnt.nanxuanxn.top

[U46] PHP：可空类型
来源：http://tnf.tianlin.xyz

?string $name = null
来源：http://iiw.aizwys.cn

[U47] PHP：联合类型
来源：http://oik.aibaodan.cn

int|string $id
来源：http://ftb.zhoulong.xyz

[U48] PHP：纯枚举
来源：http://rrx.epnwcf.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pyu.jqgufenzy.top

[U49] PHP：只读属性
来源：http://pcq.zhaomingkeji.xyz

public readonly string $name
来源：http://umw.daxiang520.top

[U50] PHP：构造器属性提升
来源：http://rbl.wangdashe.top

public function __construct(private int $id) {}
来源：http://ggk.fengsongda.top

[U51] PHP：数组解构
来源：http://tkl.fktsv.cn

[$a, $b] = $arr;
来源：http://xaf.ybcxt.top

[U52] PHP：箭头函数
来源：http://byf.shanyushiyangtech.top

$double = fn($x) => $x * 2;
来源：http://vhw.xingfuxueyuan.xyz

[U53] PHP：空合并运算符
来源：http://pau.bjfxy.top

$v = $a ?? $b ?? "default";
来源：http://uxm.ehwqpu.com

[U54] PHP：空安全调用
来源：http://pma.haohaochexian.top

$obj?->method()
来源：http://plq.hfpthk.cn

[U55] PHP：match 表达式
来源：http://iug.mhx1999.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iym.zdqjudy.top

[U56] PHP：命名参数
来源：http://opa.shanyushiyangtech.top

f(a: 1, b: 2)
来源：http://mhr.dianchejie.cn

[U57] PHP：字符串插值
来源：http://cus.ydzc1.top

"值: {$a}"
来源：http://bro.ivvv.top

[U58] PHP：数组三件套
来源：http://bib.bbcook.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wfd.snrcjt.cn

[U59] PHP：自定义排序
来源：http://npm.cucudq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ncb.iojbl.cn

[U60] PHP：JSON 编解码
来源：http://lqu.jianghu66.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gmg.jinqigufen.top

[U61] PHP：正则
来源：http://axs.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hvn.jqgufenzy.top

[U62] PHP：日期对象
来源：http://enm.hywenlv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vbu.nwbrower.top

[U63] PHP：文件读写
来源：http://rlg.shzxlz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rcs.yueranfly.top

[U64] PHP：目录遍历
来源：http://psm.ppjwa.cn

glob("dir/*.php");  scandir("dir");
来源：http://vwr.ivvv.top

[U65] PHP：会话
来源：http://onq.yj20258888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vyf.haohaochexian.top

[U66] PHP：设置 Cookie
来源：http://wdg.jyoumei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dxl.cashguo.top

[U67] PHP：处理文件上传
来源：http://wvi.hongshengwenyu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tzc.yongpay.top

[U68] PHP：PDO 连接
来源：http://yio.jlsjyb.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://doa.jyoumei.cn

[U69] PHP：PDO 预处理
来源：http://dex.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nri.gotoacloud.top

[U70] PHP：PDO 事务
来源：http://kqm.cqqwz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hjj.wangdashe.top

[U71] PHP：抛出异常
来源：http://ghv.zhixingplan.top

throw new RuntimeException("失败", 500);
来源：http://yar.yuanzhike.top

[U72] PHP：写错误日志
来源：http://lio.yonumen.top

error_log("失败: " . $e->getMessage());
来源：http://dus.cdnleiting.top

[U73] PHP：读取 ini 配置
来源：http://hyl.shanyushiyangtech.top

parse_ini_file("config.ini", true)
来源：http://tef.jinyuanbaomall.cn

[U74] PHP：读取环境变量
来源：http://vgw.jinghuilouyu.cn

getenv("APP_ENV") ?: "production"
来源：http://ola.shanyushiyangtech.top

[U75] PHP：依赖注入
来源：http://rze.fzhhl.top

composer require psr/container
来源：http://qyk.kuanghao11.cn

[U76] PHP：简单路由
来源：http://uip.andypj.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gxo.tianlin.xyz

[U77] PHP：模板渲染
来源：http://gsk.gzhubu.top

composer require twig/twig
来源：http://qnm.sysykeji.top

[U78] PHP：单元测试
来源：http://aoq.0kj1m.cn

composer require --dev phpunit/phpunit
来源：http://bta.yongpay.top

[U79] PHP：静态分析
来源：http://kwl.0kj1m.cn

composer require --dev phpstan/phpstan
来源：http://afm.jinghuilouyu.cn

[U80] PHP：代码规范修复
来源：http://ejf.cashguo.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zdq.cucudq.cn

[U81] JS：初始化项目
来源：http://sdt.shanyushiyangkeji.top

npm init -y;  npm i express
来源：http://qxi.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://exk.bjfxy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tdy.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://hdf.dianchejie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qdd.xziqi.cn

[U84] JS：CommonJS 写法
来源：http://njm.yj20258.top

module.exports = { a };  const { a } = require("./m");
来源：http://eeo.yongpay.top

[U85] JS：可选链
来源：http://bau.gzhubu.top

a?.b?.c
来源：http://afo.yanxiufei.cn

[U86] JS：空值合并
来源：http://jxb.guannengcc.top

a ?? b
来源：http://wdg.yj20258888.top

[U87] JS：解构默认值
来源：http://nek.hesvh.cn

const { a = 1, b = 2 } = obj;
来源：http://dau.cucudq.cn

[U88] JS：对象展开合并
来源：http://qbq.xuanzx.com

{ ...a, ...b }
来源：http://uwb.shangyingyoupin.top

[U89] JS：数组去重
来源：http://fdh.hfpthk.cn

[...new Set(arr)]
来源：http://qkc.c1oappe.top

[U90] JS：数字数组排序
来源：http://yzd.andypj.xyz

[...arr].sort((a, b) => a - b)
来源：http://czk.jinyuanbaomall.cn

[U91] JS：对象键值遍历
来源：http://fzi.hnqzz.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mux.vehdjk.com

[U92] JS：深拷贝
来源：http://ujc.bjfxy.top

structuredClone(obj)
来源：http://dzr.gogol.net.cn

[U93] JS：模板字符串
来源：http://qcg.ydzc1.top

`共 ${n} 条`
来源：http://eov.jinghuilouyu.cn

[U94] JS：箭头函数
来源：http://ihl.hammf.cn

const double = x => x * 2;
来源：http://ger.yanxiufei.cn

[U95] JS：Promise 包装
来源：http://nby.zhixingplan.top

new Promise((resolve, reject) => {})
来源：http://zlo.yongpay.top

[U96] JS：async/await 与异常
来源：http://esp.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nhb.ehwqpu.com

[U97] JS：并发请求
来源：http://uqn.andypj.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://yjo.zhiwuduotai.top

[U98] JS：fetch 带 JSON
来源：http://bup.hnqzz.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qpc.ehwqpu.com

[U99] JS：事件监听
来源：http://hxa.aizwys.cn

el.addEventListener("click", e => {})
来源：http://xxo.yueranfly.top

[U100] JS：DOM 查询
来源：http://uxv.aibaodan.cn

document.querySelector(".item")
来源：http://ryg.meibo888.top

[U101] JS：classList 操作
来源：http://qww.vqdsnc.cn

el.classList.toggle("active")
来源：http://fgo.haohaochexian.top

[U102] JS：本地存储
来源：http://pbi.vqdsnc.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mmh.zhengqikj.top

[U103] JS：定时器
来源：http://xmx.hnxiangtu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ugh.c1oappe.top

[U104] JS：防抖
来源：http://vde.feifeiyinyue.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://twe.bjfxy.top

[U105] JS：节流
来源：http://dzt.quarkkingdee.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ufi.nwbrower.top

[U106] JS：日期格式化
来源：http://eyx.zhongyouzk.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://axx.mhx1999.top

[U107] JS：数字千分位
来源：http://gli.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://col.fktsv.cn

[U108] JS：随机整数
来源：http://kaj.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xfg.52xcode.cn

[U109] JS：数组分组
来源：http://kvs.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://vqz.zhiwuduotai.top

[U110] JS：数组分块
来源：http://iji.shanyushiyangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fku.nanxuanxn.top

[U111] JS：对象转 Map
来源：http://wai.xziqi.cn

new Map(Object.entries(obj))
来源：http://tex.0kj1m.cn

[U112] JS：字符串补位
来源：http://obu.52xcode.cn

"7".padStart(3, "0")
来源：http://cqx.wangdashe.top

[U113] JS：正则替换全部
来源：http://uuz.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://doz.bbcook.cn

[U114] JS：JSON 深比较
来源：http://zmc.zhoulong.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://uhj.zhaomingkeji.xyz

[U115] JS：生成 UUID
来源：http://xvk.jinghuilouyu.cn

crypto.randomUUID()
来源：http://ulw.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://qni.aibaodan.cn

/** @param {string} name */ function f(name) {}
来源：http://eat.fengsongda.top

[U117] JS：单元测试
来源：http://mjy.sweek.top

npm i -D vitest;  npx vitest
来源：http://lyt.bjfxy.top

[U118] JS：开发服务器
来源：http://uvi.9152youxi.cn

npm i -D vite;  npx vite
来源：http://tie.jianghu66.top


<!-- 参考信息 -->