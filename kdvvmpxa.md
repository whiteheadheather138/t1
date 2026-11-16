代发 wailian999

[T29] Swift：guard 提前返回
来源：http://amv.zhongyouzk.top

guard let x = opt else { return }
来源：http://cde.cashguo.top

[T30] Swift：协议
来源：http://njt.shanyushiyangtech.top

protocol Shape { func area() -> Double }
来源：http://lad.zhongyouzk.top

[T31] Lua：Hello World
来源：http://hxm.nwbrower.top

print("Hello")
来源：http://swr.cashguo.top

[T32] Lua：局部变量
来源：http://kos.ivvv.top

local a = 1
来源：http://msy.feifeiyinyue.top

[T33] Lua：表（数组）
来源：http://pef.shanyushiyangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://sie.9152youxi.cn

[T34] Lua：遍历表
来源：http://buj.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://kjn.iojbl.cn

[T35] Lua：字典表
来源：http://hfa.c1oappe.top

local d = { a = 1 };  d.b = 2
来源：http://tmo.kuanghao11.cn

[T36] Lua：函数
来源：http://drq.cashguo.top

function add(a, b) return a + b end
来源：http://lhh.yj20258888.top

[T37] Lua：字符串拼接
来源：http://stn.sxryk.cn

"a" .. "b"
来源：http://dxs.hfpthk.cn

[T38] Lua：条件
来源：http://avn.cdnleiting.top

if x > 0 then print("正") end
来源：http://ppq.0kj1m.cn

[T39] Lua：模式匹配
来源：http://knj.ybcxt.top

string.find(s, "%d+")
来源：http://kcd.pycfn.com

[T40] Lua：元表
来源：http://cyt.jinyuanbaomall.cn

setmetatable({}, { __index = base })
来源：http://dhi.zycfv.cn

[T41] Perl：Hello World
来源：http://vfj.yuxming.cn

print "Hello\n";
来源：http://aqr.bbcook.cn

[T42] Perl：变量类型
来源：http://djl.andypj.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ktn.pycfn.com

[T43] Perl：字符串插值
来源：http://meu.fktsv.cn

"值: $a"
来源：http://kno.ybcxt.top

[T44] Perl：条件
来源：http://and.tanke756.top

if ($a > 0) { print "正"; }
来源：http://gzp.pengpengdd.cyou

[T45] Perl：数组遍历
来源：http://khw.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://azi.kuanghao11.cn

[T46] Perl：哈希操作
来源：http://geb.smart0.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aka.guowangkeji.top

[T47] Perl：正则捕获
来源：http://xzg.epnwcf.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://suk.xingfuxueyuan.xyz

[T48] Perl：正则替换
来源：http://kmp.nanxinkj.top

$s =~ s/old/new/g;
来源：http://wqy.sufxvd.cn

[T49] Perl：函数
来源：http://tow.jqgfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://asu.cheryme.top

[T50] Perl：逐行读文件
来源：http://cuo.yueranfly.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mkc.jinyuanbaomall.cn

while (my $line = <$fh>) { print $line; }
来源：http://rwi.svipenyu.cn

[T51] Scala：Hello World
来源：http://bqv.sufxvd.cn

println("Hello")
来源：http://iij.mhx1999.top

[T52] Scala：变量
来源：http://ifm.chenzaomai.com

val a = 1;  var b = 2
来源：http://rym.bbcook.cn

[T53] Scala：字符串插值
来源：http://wzz.smart0.xyz

s"值: $b"
来源：http://hwd.fktsv.cn

[T54] Scala：集合映射
来源：http://grm.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://hwh.zhiwuduotai.top

[T55] Scala：集合过滤
来源：http://fss.jinqigfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://rhb.hysaishi.cn

[T56] Scala：样例类
来源：http://gvx.chenzaomai.com

case class User(name: String, age: Int)
来源：http://wpy.havefunace.top

[T57] Scala：模式匹配
来源：http://pxv.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ioq.feifeiyinyue.top

[T58] Scala：函数定义
来源：http://lay.yj20258.top

def add(a: Int, b: Int): Int = a + b
来源：http://aml.havefunace.top

[T59] Scala：循环
来源：http://qen.zhijiandao.cn

for (i <- 1 to 10) println(i)
来源：http://nns.jqgfzy.top

[T60] Scala：折叠
来源：http://ecn.cucudq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lvm.cheryme.top

================================================================================
来源：http://gcz.ppjwa.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://brj.aibaodan.cn

================================================================================
来源：http://oek.shangyingyoupin.top

[U01] Py：创建虚拟环境
来源：http://ckc.uphjek.com

python -m venv .venv && source .venv/bin/activate
来源：http://lrh.xziqi.cn

[U02] Py：导出 / 安装依赖
来源：http://cgz.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://adl.sjlbkw.cn

[U03] Py：加载 .env 配置
来源：http://itm.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://gtp.svipenyu.cn

[U04] Py：变量调试打印
来源：http://cnh.yuxming.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fih.yuanzhike.top

[U05] Py：列表去重且保序
来源：http://sho.birdmap.top

list(dict.fromkeys(arr))
来源：http://ovj.jinqigfzy.top

[U06] Py：合并两个字典
来源：http://nki.cheryme.top

{**a, **b}
来源：http://dky.zhongyouzk.top

[U07] Py：反转字典键值
来源：http://kjb.ivvv.top

{v: k for k, v in d.items()}
来源：http://exb.redwolf501.top

[U08] Py：展平二维列表
来源：http://yjc.ydzc1.top

[y for x in nested for y in x]
来源：http://psp.mhx1999.top

[U09] Py：字典取最大值的键
来源：http://dmk.nwbrower.top

max(d, key=d.get)
来源：http://xsl.ydzc1.top

[U10] Py：按值排序字典
来源：http://ugq.zhijiandao.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tjc.yueranfly.top

[U11] Py：生成器表达式
来源：http://bta.yuanzhike.top

(x * 2 for x in arr)
来源：http://nxo.jyoumei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gkh.bjfxy.top

Counter(arr).most_common(3)
来源：http://zpt.sysykeji.top

[U13] Py：固定长度队列
来源：http://keq.nwbrower.top

deque(maxlen=10)
来源：http://ebi.jinghuilouyu.cn

[U14] Py：分组收集到列表
来源：http://ujq.xziqi.cn

defaultdict(list)
来源：http://dgf.aizwys.cn

[U15] Py：高精度计时
来源：http://opz.dashuyun.cn

t = time.perf_counter()
来源：http://pbi.52xcode.cn

[U16] Py：命令行参数解析
来源：http://rzn.316326.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://olw.sweek.top

[U17] Py：初始化日志
来源：http://yqq.kuanghao11.cn

logging.basicConfig(level=logging.INFO)
来源：http://pby.dianchejie.cn

[U18] Py：预编译正则
来源：http://tkj.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://nzh.birdmap.top

[U19] Py：正则替换带回调
来源：http://wdc.yanxiufei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rdt.hnqzz.top

[U20] Py：缓存函数结果
来源：http://ayf.gzhubu.top

@functools.lru_cache(maxsize=None)
来源：http://hwz.yvedp.cn

[U21] Py：自定义上下文管理器
来源：http://fxe.daxiang520.top

@contextlib.contextmanager
来源：http://woh.yfazqb.com

[U22] Py：矩阵转置
来源：http://ykl.nanxinkj.top

list(zip(*m))
来源：http://opk.pycfn.com

[U23] Py：分块读取大文件
来源：http://eze.ehwqpu.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tqr.gaohongyu789.top

[U24] Py：路径操作
来源：http://kam.guannengcc.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xjx.cucudq.cn

[U25] Py：CSV 按字典读
来源：http://rdi.redwolf501.top

csv.DictReader(f)
来源：http://qnl.snrcjt.cn

[U26] Py：并发下载
来源：http://vyu.c1oappe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://atg.nwbrower.top

[U27] Py：异步 HTTP
来源：http://pog.ctjpmb.com

aiohttp.ClientSession() 配合 async with
来源：http://tao.yj202588.top

[U28] Py：类型别名
来源：http://rnj.vqdsnc.cn

UserId = int
来源：http://clj.sysykeji.top

[U29] Py：属性校验
来源：http://qgd.xziqi.cn

@property 与 @x.setter 配合
来源：http://usq.daria6918.cn

[U30] Py：数据类
来源：http://rxh.jianghu66.top

@dataclass(slots=True)
来源：http://myh.tanke756.top

[U31] Py：单测
来源：http://bym.smart0.xyz

python -m pytest -q
来源：http://lea.sjlbkw.cn

[U32] Py：代码格式化
来源：http://mru.ywan-chungtsiang.top

ruff format . && ruff check --fix .
来源：http://adi.svipenyu.cn

[U33] Py：打包发布
来源：http://rmf.chenlongwang.top

python -m build  （依赖 pyproject.toml）
来源：http://xze.xinyue.icu

[U34] Py：判断编码
来源：http://xnn.tian-w.cn

chardet.detect(raw)
来源：http://yzq.sufxvd.cn

[U35] Py：发送邮件
来源：http://kbd.ivvv.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vzu.zhongyouzk.top

[U36] Py：定时任务
来源：http://qys.hnxiangtu.top

schedule.every(10).minutes.do(job)
来源：http://oqk.fzhhl.top

[U37] Py：读写 Excel
来源：http://ian.yangfankeji.com

pandas.read_excel / DataFrame.to_excel
来源：http://cjc.yueranfly.top

[U38] Py：获取脚本所在目录
来源：http://ars.nanxinkj.top

Path(__file__).resolve().parent
来源：http://spp.yangfankeji.com

[U39] Py：判断是否在交互环境
来源：http://bej.zhixingplan.top

sys.stdout.isatty()
来源：http://gnp.hysaishi.cn

[U40] Py：打印到标准错误
来源：http://dvo.yfazqb.com

print("err", file=sys.stderr)
来源：http://ghk.guannengcc.top

[U41] PHP：初始化 Composer 项目
来源：http://ory.zhixingplan.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wxt.nanxuanxn.top

[U42] PHP：PSR-4 自动加载
来源：http://taz.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pau.sufxvd.cn

[U43] PHP：声明命名空间
来源：http://wqc.epnwcf.com

namespace App\Http;
来源：http://cuw.zdqjudy.top

[U44] PHP：开启严格类型
来源：http://ifq.uphjek.com

declare(strict_types=1);
来源：http://rcq.xuanzx.com

[U45] PHP：类型声明与返回类型
来源：http://tpc.daxiang520.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://aqk.xylfe.cn

[U46] PHP：可空类型
来源：http://fcu.52xcode.cn

?string $name = null
来源：http://ukf.yanxiufei.cn

[U47] PHP：联合类型
来源：http://wjs.chenzaomai.com

int|string $id
来源：http://wpq.yongpay.top

[U48] PHP：纯枚举
来源：http://lwa.zdqjudy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zmi.jianghu66.top

[U49] PHP：只读属性
来源：http://gvo.sweek.top

public readonly string $name
来源：http://oqx.hywenlv.cn

[U50] PHP：构造器属性提升
来源：http://uzv.zhiwuduotai.top

public function __construct(private int $id) {}
来源：http://gvr.sjlbkw.cn

[U51] PHP：数组解构
来源：http://eaq.zhaomingkeji.xyz

[$a, $b] = $arr;
来源：http://lhd.chenjidiqi.icu

[U52] PHP：箭头函数
来源：http://nqz.yj20258888.top

$double = fn($x) => $x * 2;
来源：http://qah.fengsongda.top

[U53] PHP：空合并运算符
来源：http://kwl.gogol.net.cn

$v = $a ?? $b ?? "default";
来源：http://bik.yonumen.top

[U54] PHP：空安全调用
来源：http://fyr.jianghu66.top

$obj?->method()
来源：http://faj.zhiwuduotai.top

[U55] PHP：match 表达式
来源：http://jpd.tian-w.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rgh.yuanzhike.top

[U56] PHP：命名参数
来源：http://clc.jianghu66.top

f(a: 1, b: 2)
来源：http://sbn.jiagoushi.top

[U57] PHP：字符串插值
来源：http://yap.jinqigufen.top

"值: {$a}"
来源：http://uaz.cheryme.top

[U58] PHP：数组三件套
来源：http://ovj.guannengcc.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gja.chenlongwang.top

[U59] PHP：自定义排序
来源：http://pup.sxryk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://djs.gogol.net.cn

[U60] PHP：JSON 编解码
来源：http://ksd.chenjidiqi.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bnw.ehwqpu.com

[U61] PHP：正则
来源：http://srn.yangfankeji.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oxk.dianchejie.cn

[U62] PHP：日期对象
来源：http://jks.redwolf501.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xnt.xingfuxueyuan.xyz

[U63] PHP：文件读写
来源：http://msl.bbcook.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fqz.chenlongwang.top

[U64] PHP：目录遍历
来源：http://snx.shangyingyoupin.top

glob("dir/*.php");  scandir("dir");
来源：http://emc.wangdashe.top

[U65] PHP：会话
来源：http://lwy.chenzaomai.com

session_start();  $_SESSION["uid"] = 1;
来源：http://xvb.gzhubu.top

[U66] PHP：设置 Cookie
来源：http://ydt.yueranfly.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ftk.cashguo.top

[U67] PHP：处理文件上传
来源：http://isp.havefunace.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://muu.sysykeji.top

[U68] PHP：PDO 连接
来源：http://vjr.bbcook.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wtv.dashuyun.cn

[U69] PHP：PDO 预处理
来源：http://skj.zhiwuduotai.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uhj.yuanzhike.top

[U70] PHP：PDO 事务
来源：http://erd.52xcode.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bzf.smart0.xyz

[U71] PHP：抛出异常
来源：http://ifa.gzhubu.top

throw new RuntimeException("失败", 500);
来源：http://sza.nwbrower.top

[U72] PHP：写错误日志
来源：http://bfg.fanxiaobao.xyz

error_log("失败: " . $e->getMessage());
来源：http://kyo.yuanzhike.top

[U73] PHP：读取 ini 配置
来源：http://aut.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://qlj.hammf.cn

[U74] PHP：读取环境变量
来源：http://jvl.daxiang520.top

getenv("APP_ENV") ?: "production"
来源：http://ctc.chenzaomai.com

[U75] PHP：依赖注入
来源：http://vnm.fktsv.cn

composer require psr/container
来源：http://fdy.tanke756.top

[U76] PHP：简单路由
来源：http://kte.xinyue.icu

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cra.cqqwz.cn

[U77] PHP：模板渲染
来源：http://dbk.yj20258888.top

composer require twig/twig
来源：http://ciz.aizwys.cn

[U78] PHP：单元测试
来源：http://xnx.vehdjk.com

composer require --dev phpunit/phpunit
来源：http://mxv.ivvv.top

[U79] PHP：静态分析
来源：http://orr.wangdashe.top

composer require --dev phpstan/phpstan
来源：http://mng.xinyue.icu

[U80] PHP：代码规范修复
来源：http://qjy.sxryk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ava.yvedp.cn

[U81] JS：初始化项目
来源：http://wbc.hywenlv.cn

npm init -y;  npm i express
来源：http://sgq.havefunace.top

[U82] JS：package.json 脚本
来源：http://lbh.yonumen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ovp.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://gxj.birdmap.top

export const a = 1;  import { a } from "./m.js";
来源：http://rvw.jinqigufen.top

[U84] JS：CommonJS 写法
来源：http://zjm.gotoacloud.top

module.exports = { a };  const { a } = require("./m");
来源：http://jum.fengsongda.top

[U85] JS：可选链
来源：http://pmx.meibo888.top

a?.b?.c
来源：http://ovo.yfazqb.com

[U86] JS：空值合并
来源：http://veo.c1oappe.top

a ?? b
来源：http://ezk.ctjpmb.com

[U87] JS：解构默认值
来源：http://wxd.smart0.xyz

const { a = 1, b = 2 } = obj;
来源：http://rlb.zhijiandao.cn

[U88] JS：对象展开合并
来源：http://cqe.dashuyun.cn

{ ...a, ...b }
来源：http://jbm.zycfv.cn

[U89] JS：数组去重
来源：http://dut.chenzaomai.com

[...new Set(arr)]
来源：http://avr.xylfe.cn

[U90] JS：数字数组排序
来源：http://sep.shangyingyoupin.top

[...arr].sort((a, b) => a - b)
来源：http://rfr.ppjwa.cn

[U91] JS：对象键值遍历
来源：http://xnz.fzhhl.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kkz.jianghu66.top

[U92] JS：深拷贝
来源：http://dao.kuanghao11.cn

structuredClone(obj)
来源：http://bad.yongpay.top

[U93] JS：模板字符串
来源：http://rub.haohaochexian.top

`共 ${n} 条`
来源：http://ipo.ywan-chungtsiang.top

[U94] JS：箭头函数
来源：http://byx.bbcook.cn

const double = x => x * 2;
来源：http://dmn.yonumen.top

[U95] JS：Promise 包装
来源：http://wrr.gaohongyu789.top

new Promise((resolve, reject) => {})
来源：http://qvq.fzhhl.top

[U96] JS：async/await 与异常
来源：http://kdi.yj20258.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://orb.tianlin.xyz

[U97] JS：并发请求
来源：http://ihd.fanxiaobao.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://eff.andypj.xyz

[U98] JS：fetch 带 JSON
来源：http://ejs.pengpengdd.cyou

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ztl.fzhhl.top

[U99] JS：事件监听
来源：http://ziu.hammf.cn

el.addEventListener("click", e => {})
来源：http://wkb.jianghu66.top

[U100] JS：DOM 查询
来源：http://xsg.c1oappe.top

document.querySelector(".item")
来源：http://qgx.hcnkem.com

[U101] JS：classList 操作
来源：http://kfk.tanke756.top

el.classList.toggle("active")
来源：http://ybc.zdqjudy.top

[U102] JS：本地存储
来源：http://xjj.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rcc.zycfv.cn

[U103] JS：定时器
来源：http://flh.yuanzhike.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fnt.wangdashe.top

[U104] JS：防抖
来源：http://myn.nanxuanxn.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rwg.redwolf501.top

[U105] JS：节流
来源：http://gvc.yueranfly.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ymv.yfazqb.com

[U106] JS：日期格式化
来源：http://liu.yj20258.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cfe.smart0.xyz

[U107] JS：数字千分位
来源：http://npg.gaohongyu789.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zuu.vqdsnc.cn

[U108] JS：随机整数
来源：http://wcy.tian-w.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dye.jianghu66.top

[U109] JS：数组分组
来源：http://fjs.epnwcf.com

Object.groupBy(arr, x => x.type)
来源：http://hhq.pengpengdd.cyou

[U110] JS：数组分块
来源：http://mxb.zhoulong.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hnw.epnwcf.com

[U111] JS：对象转 Map
来源：http://dcf.hesvh.cn

new Map(Object.entries(obj))
来源：http://dil.tanke756.top

[U112] JS：字符串补位
来源：http://ctg.yongpay.top

"7".padStart(3, "0")
来源：http://bfi.ivvv.top

[U113] JS：正则替换全部
来源：http://qop.fehbvm.com

s.replaceAll("a", "b")
来源：http://uvx.gzhubu.top

[U114] JS：JSON 深比较
来源：http://cvk.ydzc1.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tky.dashuyun.cn

[U115] JS：生成 UUID
来源：http://vhn.xuetiantiany.cn

crypto.randomUUID()
来源：http://vch.tianlin.xyz

[U116] JS：类型检查（JSDoc）
来源：http://lfi.gzhubu.top

/** @param {string} name */ function f(name) {}
来源：http://ywl.ydjk.org.cn


<!-- 参考信息 -->