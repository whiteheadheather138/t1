代发 wailian999

[T33] Lua：表（数组）
来源：http://lld.aibaodan.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fwo.dashuyun.cn

[T34] Lua：遍历表
来源：http://bvc.hongshengwenyu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://vgd.fengsongda.top

[T35] Lua：字典表
来源：http://bew.ppjwa.cn

local d = { a = 1 };  d.b = 2
来源：http://rzn.sysykeji.top

[T36] Lua：函数
来源：http://ddq.hywenlv.cn

function add(a, b) return a + b end
来源：http://clx.pengpengdd.cyou

[T37] Lua：字符串拼接
来源：http://avw.yueranfly.top

"a" .. "b"
来源：http://ezg.shuidangran.top

[T38] Lua：条件
来源：http://nhc.aibaodan.cn

if x > 0 then print("正") end
来源：http://rjp.zhiwuduotai.top

[T39] Lua：模式匹配
来源：http://gix.uphjek.com

string.find(s, "%d+")
来源：http://aqn.nanxinkj.top

[T40] Lua：元表
来源：http://ltr.bjfxy.top

setmetatable({}, { __index = base })
来源：http://yuc.guowangkeji.top

[T41] Perl：Hello World
来源：http://ytj.aizwys.cn

print "Hello\n";
来源：http://vmj.gzhubu.top

[T42] Perl：变量类型
来源：http://edc.sxryk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zyt.ybcxt.top

[T43] Perl：字符串插值
来源：http://gfj.andypj.xyz

"值: $a"
来源：http://biw.ehwqpu.com

[T44] Perl：条件
来源：http://sgn.tanke756.top

if ($a > 0) { print "正"; }
来源：http://eku.hcnkem.com

[T45] Perl：数组遍历
来源：http://jer.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://lji.hywenlv.cn

[T46] Perl：哈希操作
来源：http://xjt.andypj.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qyd.ivvv.top

[T47] Perl：正则捕获
来源：http://ehu.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hxw.guowangkeji.top

[T48] Perl：正则替换
来源：http://dsw.c1oappe.top

$s =~ s/old/new/g;
来源：http://skn.bjfxy.top

[T49] Perl：函数
来源：http://byw.redwolf501.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yqk.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://xqk.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fsk.yangfankeji.com

while (my $line = <$fh>) { print $line; }
来源：http://kzk.daria6918.cn

[T51] Scala：Hello World
来源：http://rek.hnqzz.top

println("Hello")
来源：http://vuy.wangshuangyany.cn

[T52] Scala：变量
来源：http://lto.xuetiantiany.cn

val a = 1;  var b = 2
来源：http://lxo.hcnkem.com

[T53] Scala：字符串插值
来源：http://khp.shanyushiyangtech.top

s"值: $b"
来源：http://bby.cashguo.top

[T54] Scala：集合映射
来源：http://rac.daxiang520.top

List(1, 2, 3).map(_ * 2)
来源：http://xrf.ydzc1.top

[T55] Scala：集合过滤
来源：http://wqh.uphjek.com

List(1, 2, 3).filter(_ > 1)
来源：http://sof.yj20258888.top

[T56] Scala：样例类
来源：http://cow.c1oappe.top

case class User(name: String, age: Int)
来源：http://hae.hcnkem.com

[T57] Scala：模式匹配
来源：http://cgx.yvedp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cdl.9152youxi.cn

[T58] Scala：函数定义
来源：http://cio.jinqigfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://efr.zdbjq.cn

[T59] Scala：循环
来源：http://xxw.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://upu.guowangkeji.top

[T60] Scala：折叠
来源：http://kvv.vqdsnc.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cbi.daria6918.cn

================================================================================
来源：http://xpb.gzhubu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xsb.birdmap.top

================================================================================
来源：http://glc.yvedp.cn

[U01] Py：创建虚拟环境
来源：http://leh.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://ftt.birdmap.top

[U02] Py：导出 / 安装依赖
来源：http://czq.haohaochexian.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vys.yfazqb.com

[U03] Py：加载 .env 配置
来源：http://juf.zdqjudy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ffs.guannengcc.top

[U04] Py：变量调试打印
来源：http://hua.vehdjk.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sai.yonumen.top

[U05] Py：列表去重且保序
来源：http://uzt.52xcode.cn

list(dict.fromkeys(arr))
来源：http://qho.jinqigufen.top

[U06] Py：合并两个字典
来源：http://nqp.zhixingplan.top

{**a, **b}
来源：http://ppv.zdbjq.cn

[U07] Py：反转字典键值
来源：http://vpz.yongpay.top

{v: k for k, v in d.items()}
来源：http://ije.ydzc1.top

[U08] Py：展平二维列表
来源：http://eto.jianghu66.top

[y for x in nested for y in x]
来源：http://qkc.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://loy.ydzc1.top

max(d, key=d.get)
来源：http://swu.sjlbkw.cn

[U10] Py：按值排序字典
来源：http://xqa.bjfxy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ugs.hfpthk.cn

[U11] Py：生成器表达式
来源：http://rzb.shuidangran.top

(x * 2 for x in arr)
来源：http://cdw.uphjek.com

[U12] Py：取出现最多的 3 个元素
来源：http://gpu.vehdjk.com

Counter(arr).most_common(3)
来源：http://pfi.yfazqb.com

[U13] Py：固定长度队列
来源：http://fww.jqgfzy.top

deque(maxlen=10)
来源：http://yjz.yueranfly.top

[U14] Py：分组收集到列表
来源：http://mvy.xingfuxueyuan.xyz

defaultdict(list)
来源：http://lic.sjlbkw.cn

[U15] Py：高精度计时
来源：http://tih.hnqzz.top

t = time.perf_counter()
来源：http://zfm.havefunace.top

[U16] Py：命令行参数解析
来源：http://phs.c1oappe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sqi.daria6918.cn

[U17] Py：初始化日志
来源：http://src.xinyue.icu

logging.basicConfig(level=logging.INFO)
来源：http://ypf.nanxinkj.top

[U18] Py：预编译正则
来源：http://zvl.sufxvd.cn

pat = re.compile(r"\d+")
来源：http://akf.sxryk.cn

[U19] Py：正则替换带回调
来源：http://dgv.cashguo.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tlq.c1oappe.top

[U20] Py：缓存函数结果
来源：http://tfb.dianchejie.cn

@functools.lru_cache(maxsize=None)
来源：http://pib.jqgfzy.top

[U21] Py：自定义上下文管理器
来源：http://pdf.jinyuanbaomall.cn

@contextlib.contextmanager
来源：http://lcp.hnqzz.top

[U22] Py：矩阵转置
来源：http://ial.xylfe.cn

list(zip(*m))
来源：http://uiy.gzhubu.top

[U23] Py：分块读取大文件
来源：http://gfa.mhx1999.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://meo.sysykeji.top

[U24] Py：路径操作
来源：http://fwl.nanxinkj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qjq.sufxvd.cn

[U25] Py：CSV 按字典读
来源：http://nxz.daxiang520.top

csv.DictReader(f)
来源：http://mwu.gotoacloud.top

[U26] Py：并发下载
来源：http://lbm.jinyuanbaomall.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pmw.fzhhl.top

[U27] Py：异步 HTTP
来源：http://cbb.jqgfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://fug.jinqigufen.top

[U28] Py：类型别名
来源：http://nhb.guannengcc.top

UserId = int
来源：http://clq.zycfv.cn

[U29] Py：属性校验
来源：http://rzn.yonumen.top

@property 与 @x.setter 配合
来源：http://scz.gaohongyu789.top

[U30] Py：数据类
来源：http://doz.wangdashe.top

@dataclass(slots=True)
来源：http://gaf.wangdashe.top

[U31] Py：单测
来源：http://fab.ydzc1.top

python -m pytest -q
来源：http://tpy.iojbl.cn

[U32] Py：代码格式化
来源：http://mkk.daxiang520.top

ruff format . && ruff check --fix .
来源：http://keq.yj202588.top

[U33] Py：打包发布
来源：http://ply.shzxlz.cn

python -m build  （依赖 pyproject.toml）
来源：http://rnx.pengpengdd.cyou

[U34] Py：判断编码
来源：http://toa.daria6918.cn

chardet.detect(raw)
来源：http://ued.gaohongyu789.top

[U35] Py：发送邮件
来源：http://xdx.jyoumei.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ebb.jinqigufen.top

[U36] Py：定时任务
来源：http://ysr.zycfv.cn

schedule.every(10).minutes.do(job)
来源：http://xvs.sjlbkw.cn

[U37] Py：读写 Excel
来源：http://paq.yongpay.top

pandas.read_excel / DataFrame.to_excel
来源：http://zgt.jqgfzy.top

[U38] Py：获取脚本所在目录
来源：http://pct.tarul.cn

Path(__file__).resolve().parent
来源：http://fdh.nanxuanxn.top

[U39] Py：判断是否在交互环境
来源：http://sro.nanxuanxn.top

sys.stdout.isatty()
来源：http://gid.daria6918.cn

[U40] Py：打印到标准错误
来源：http://prh.jlsjyb.cn

print("err", file=sys.stderr)
来源：http://jxy.epnwcf.com

[U41] PHP：初始化 Composer 项目
来源：http://lvg.jinyuanbaomall.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dyk.sufxvd.cn

[U42] PHP：PSR-4 自动加载
来源：http://jry.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://onx.ppjwa.cn

[U43] PHP：声明命名空间
来源：http://eao.jinghuilouyu.cn

namespace App\Http;
来源：http://bdy.vqdsnc.cn

[U44] PHP：开启严格类型
来源：http://bbf.fengsongda.top

declare(strict_types=1);
来源：http://uga.shzxlz.cn

[U45] PHP：类型声明与返回类型
来源：http://gln.zhongyouzk.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qnw.fktsv.cn

[U46] PHP：可空类型
来源：http://dhw.ydzc1.top

?string $name = null
来源：http://xmo.redwolf501.top

[U47] PHP：联合类型
来源：http://nni.shangyingyoupin.top

int|string $id
来源：http://bio.zhengqikj.top

[U48] PHP：纯枚举
来源：http://rob.jianghu66.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jcy.fanxiaobao.xyz

[U49] PHP：只读属性
来源：http://xdj.redwolf501.top

public readonly string $name
来源：http://knr.shuidangran.top

[U50] PHP：构造器属性提升
来源：http://vju.nanxinkj.top

public function __construct(private int $id) {}
来源：http://osw.jinqigufen.top

[U51] PHP：数组解构
来源：http://dkg.redwolf501.top

[$a, $b] = $arr;
来源：http://vhz.yj20258.top

[U52] PHP：箭头函数
来源：http://awe.ydzc1.top

$double = fn($x) => $x * 2;
来源：http://uqq.cheryme.top

[U53] PHP：空合并运算符
来源：http://wwj.tarul.cn

$v = $a ?? $b ?? "default";
来源：http://ggj.xuanzx.com

[U54] PHP：空安全调用
来源：http://oet.yanxiufei.cn

$obj?->method()
来源：http://ffc.iojbl.cn

[U55] PHP：match 表达式
来源：http://dzt.yfazqb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qiz.yonumen.top

[U56] PHP：命名参数
来源：http://awf.gaohongyu789.top

f(a: 1, b: 2)
来源：http://csc.ctjpmb.com

[U57] PHP：字符串插值
来源：http://nnz.sxryk.cn

"值: {$a}"
来源：http://sqb.shzxlz.cn

[U58] PHP：数组三件套
来源：http://ste.xuetiantiany.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yni.xuetiantiany.cn

[U59] PHP：自定义排序
来源：http://fze.yj20258.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qjj.zhoulong.xyz

[U60] PHP：JSON 编解码
来源：http://fbv.aibaodan.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cmk.hysaishi.cn

[U61] PHP：正则
来源：http://lgi.zhaomingkeji.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fbl.jianghu66.top

[U62] PHP：日期对象
来源：http://ibw.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jhv.xinyue.icu

[U63] PHP：文件读写
来源：http://mfe.cucudq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://opi.fzhhl.top

[U64] PHP：目录遍历
来源：http://aok.yj20258888.top

glob("dir/*.php");  scandir("dir");
来源：http://fov.hcnkem.com

[U65] PHP：会话
来源：http://gdp.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ugi.zhengqikj.top

[U66] PHP：设置 Cookie
来源：http://zri.havefunace.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dfj.ydzc1.top

[U67] PHP：处理文件上传
来源：http://qjn.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qes.zdqjudy.top

[U68] PHP：PDO 连接
来源：http://fja.zdbjq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://duk.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://mzt.xuanzx.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qjs.zhixingplan.top

[U70] PHP：PDO 事务
来源：http://dpt.tian-w.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zje.redwolf501.top

[U71] PHP：抛出异常
来源：http://pch.tianlin.xyz

throw new RuntimeException("失败", 500);
来源：http://fqr.bbcook.cn

[U72] PHP：写错误日志
来源：http://lqs.xuetiantiany.cn

error_log("失败: " . $e->getMessage());
来源：http://wot.jinyuanbaomall.cn

[U73] PHP：读取 ini 配置
来源：http://oaq.sysykeji.top

parse_ini_file("config.ini", true)
来源：http://hra.ppjwa.cn

[U74] PHP：读取环境变量
来源：http://mor.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://auy.hnxiangtu.top

[U75] PHP：依赖注入
来源：http://ruw.nanxinkj.top

composer require psr/container
来源：http://bny.hysaishi.cn

[U76] PHP：简单路由
来源：http://hem.fehbvm.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tom.zhaomingkeji.xyz

[U77] PHP：模板渲染
来源：http://aqk.xuetiantiany.cn

composer require twig/twig
来源：http://krt.sweek.top

[U78] PHP：单元测试
来源：http://hpa.xingfuxueyuan.xyz

composer require --dev phpunit/phpunit
来源：http://czp.nwbrower.top

[U79] PHP：静态分析
来源：http://jnh.xuetiantiany.cn

composer require --dev phpstan/phpstan
来源：http://sec.hcnkem.com

[U80] PHP：代码规范修复
来源：http://jjz.0kj1m.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rja.yangfankeji.com

[U81] JS：初始化项目
来源：http://mex.tianlin.xyz

npm init -y;  npm i express
来源：http://lqs.dashuyun.cn

[U82] JS：package.json 脚本
来源：http://kvb.sjlbkw.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ghu.sweek.top

[U83] JS：ES Module 导入导出
来源：http://gaf.jinghuilouyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ltt.aibaodan.cn

[U84] JS：CommonJS 写法
来源：http://ync.cdnleiting.top

module.exports = { a };  const { a } = require("./m");
来源：http://iqp.guowangkeji.top

[U85] JS：可选链
来源：http://qdw.xylfe.cn

a?.b?.c
来源：http://mdn.gotoacloud.top

[U86] JS：空值合并
来源：http://hqj.sysykeji.top

a ?? b
来源：http://vbb.yj20258.top

[U87] JS：解构默认值
来源：http://mqz.nwbrower.top

const { a = 1, b = 2 } = obj;
来源：http://xmd.fktsv.cn

[U88] JS：对象展开合并
来源：http://izk.vqdsnc.cn

{ ...a, ...b }
来源：http://atf.ydzc1.top

[U89] JS：数组去重
来源：http://tpw.xylfe.cn

[...new Set(arr)]
来源：http://weh.yanxiufei.cn

[U90] JS：数字数组排序
来源：http://oms.uphjek.com

[...arr].sort((a, b) => a - b)
来源：http://qop.ivvv.top

[U91] JS：对象键值遍历
来源：http://hid.xuanzx.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://okb.aibaodan.cn

[U92] JS：深拷贝
来源：http://irn.fehbvm.com

structuredClone(obj)
来源：http://iaq.svipenyu.cn

[U93] JS：模板字符串
来源：http://emc.vqdsnc.cn

`共 ${n} 条`
来源：http://ick.guannengcc.top

[U94] JS：箭头函数
来源：http://rjb.yanxiufei.cn

const double = x => x * 2;
来源：http://vct.zhaomingkeji.xyz

[U95] JS：Promise 包装
来源：http://khs.shanyushiyangkeji.top

new Promise((resolve, reject) => {})
来源：http://orp.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://yqi.guowangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ynm.xuanzx.com

[U97] JS：并发请求
来源：http://vbq.zhiwuduotai.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tnz.hesvh.cn

[U98] JS：fetch 带 JSON
来源：http://bns.gaohongyu789.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jfq.fzhhl.top

[U99] JS：事件监听
来源：http://ekt.fengsongda.top

el.addEventListener("click", e => {})
来源：http://zfx.sysykeji.top

[U100] JS：DOM 查询
来源：http://jmo.haohaochexian.top

document.querySelector(".item")
来源：http://kky.0kj1m.cn

[U101] JS：classList 操作
来源：http://mgy.hongshengwenyu.top

el.classList.toggle("active")
来源：http://qkh.9152youxi.cn

[U102] JS：本地存储
来源：http://waf.ywan-chungtsiang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zwk.guowangkeji.top

[U103] JS：定时器
来源：http://qgv.jianghu66.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rnz.snrcjt.cn

[U104] JS：防抖
来源：http://anu.gzhubu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://chj.jqgufenzy.top

[U105] JS：节流
来源：http://psc.ydjk.org.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zvh.gzhubu.top

[U106] JS：日期格式化
来源：http://nyt.hnqzz.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sdw.chenjidiqi.icu

[U107] JS：数字千分位
来源：http://wbb.cheryme.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zaj.jlsjyb.cn

[U108] JS：随机整数
来源：http://rsp.fzhhl.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wok.kuanghao11.cn

[U109] JS：数组分组
来源：http://rxx.jqgufenzy.top

Object.groupBy(arr, x => x.type)
来源：http://ohb.zhongyouzk.top

[U110] JS：数组分块
来源：http://peq.guannengcc.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bka.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://jdc.shuidangran.top

new Map(Object.entries(obj))
来源：http://trz.meibo888.top

[U112] JS：字符串补位
来源：http://zol.yj202588.top

"7".padStart(3, "0")
来源：http://gwt.jyoumei.cn

[U113] JS：正则替换全部
来源：http://qyj.tanke756.top

s.replaceAll("a", "b")
来源：http://ubq.havefunace.top

[U114] JS：JSON 深比较
来源：http://urr.yangfankeji.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://kel.ppjwa.cn

[U115] JS：生成 UUID
来源：http://amb.nwbrower.top

crypto.randomUUID()
来源：http://gsd.zycfv.cn

[U116] JS：类型检查（JSDoc）
来源：http://cll.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://miv.yj202588.top

[U117] JS：单元测试
来源：http://wom.zhijiandao.cn

npm i -D vitest;  npx vitest
来源：http://snc.0kj1m.cn

[U118] JS：开发服务器
来源：http://ied.redwolf501.top

npm i -D vite;  npx vite
来源：http://kgy.hcnkem.com

[U119] JS：生产构建
来源：http://qkn.shanyushiyangtech.top

npx vite build
来源：http://ydf.zdbjq.cn

[U120] JS：读取环境变量（Vite）
来源：http://die.cucudq.cn

import.meta.env.VITE_API_URL
来源：http://cdo.svipenyu.cn


<!-- 参考信息 -->