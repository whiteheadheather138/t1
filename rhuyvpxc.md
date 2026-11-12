代发 wailian999

[T29] Swift：guard 提前返回
来源：http://uzz.gzhubu.top

guard let x = opt else { return }
来源：http://hbt.yueranfly.top

[T30] Swift：协议
来源：http://rww.xziqi.cn

protocol Shape { func area() -> Double }
来源：http://tok.shuidangran.top

[T31] Lua：Hello World
来源：http://znd.jlsjyb.cn

print("Hello")
来源：http://tdl.vqdsnc.cn

[T32] Lua：局部变量
来源：http://aep.jinghuilouyu.cn

local a = 1
来源：http://rkm.sufxvd.cn

[T33] Lua：表（数组）
来源：http://cjn.andypj.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://ptn.tarul.cn

[T34] Lua：遍历表
来源：http://zek.zhixingplan.top

for i, v in ipairs(t) do print(i, v) end
来源：http://icu.zdbjq.cn

[T35] Lua：字典表
来源：http://dyi.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://uez.cheryme.top

[T36] Lua：函数
来源：http://mva.jinqigfzy.top

function add(a, b) return a + b end
来源：http://pnw.fengsongda.top

[T37] Lua：字符串拼接
来源：http://hxu.haohaochexian.top

"a" .. "b"
来源：http://goy.guannengcc.top

[T38] Lua：条件
来源：http://zun.hysaishi.cn

if x > 0 then print("正") end
来源：http://ble.haohaochexian.top

[T39] Lua：模式匹配
来源：http://aba.jianghu66.top

string.find(s, "%d+")
来源：http://atr.svipenyu.cn

[T40] Lua：元表
来源：http://rcu.chenlongwang.top

setmetatable({}, { __index = base })
来源：http://bbt.haohaochexian.top

[T41] Perl：Hello World
来源：http://han.redwolf501.top

print "Hello\n";
来源：http://kfq.52xcode.cn

[T42] Perl：变量类型
来源：http://dwp.gaohongyu789.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zbt.zhaomingkeji.xyz

[T43] Perl：字符串插值
来源：http://auu.zhengqikj.top

"值: $a"
来源：http://tdb.haohaochexian.top

[T44] Perl：条件
来源：http://ypk.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://jgv.ctjpmb.com

[T45] Perl：数组遍历
来源：http://mue.yueranfly.top

for my $x (@arr) { print $x; }
来源：http://ntj.0kj1m.cn

[T46] Perl：哈希操作
来源：http://zmb.xingfuxueyuan.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oga.zdbjq.cn

[T47] Perl：正则捕获
来源：http://cpt.jinqigufen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yed.sufxvd.cn

[T48] Perl：正则替换
来源：http://ebb.tanke756.top

$s =~ s/old/new/g;
来源：http://ecj.aibaodan.cn

[T49] Perl：函数
来源：http://nnd.havefunace.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://isl.jlsjyb.cn

[T50] Perl：逐行读文件
来源：http://kle.bbcook.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qnz.cashguo.top

while (my $line = <$fh>) { print $line; }
来源：http://zuc.jinyuanbaomall.cn

[T51] Scala：Hello World
来源：http://ogw.bbcook.cn

println("Hello")
来源：http://kiq.yanxiufei.cn

[T52] Scala：变量
来源：http://mnh.bbcook.cn

val a = 1;  var b = 2
来源：http://kiv.shangyingyoupin.top

[T53] Scala：字符串插值
来源：http://idn.c1oappe.top

s"值: $b"
来源：http://lgi.meibo888.top

[T54] Scala：集合映射
来源：http://ett.yvedp.cn

List(1, 2, 3).map(_ * 2)
来源：http://fxl.jqgufenzy.top

[T55] Scala：集合过滤
来源：http://agr.guannengcc.top

List(1, 2, 3).filter(_ > 1)
来源：http://zno.jianghu66.top

[T56] Scala：样例类
来源：http://dht.svipenyu.cn

case class User(name: String, age: Int)
来源：http://nxe.bjfxy.top

[T57] Scala：模式匹配
来源：http://cfe.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xat.hongshengwenyu.top

[T58] Scala：函数定义
来源：http://npk.cucudq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yck.fktsv.cn

[T59] Scala：循环
来源：http://udw.ydzc1.top

for (i <- 1 to 10) println(i)
来源：http://uen.smart0.xyz

[T60] Scala：折叠
来源：http://eqa.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://thv.yanxiufei.cn

================================================================================
来源：http://qpe.hongshengwenyu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lmb.jinyuanbaomall.cn

================================================================================
来源：http://nbw.ivvv.top

[U01] Py：创建虚拟环境
来源：http://ith.ybcxt.top

python -m venv .venv && source .venv/bin/activate
来源：http://bcz.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://ynx.zhijiandao.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wfp.yvedp.cn

[U03] Py：加载 .env 配置
来源：http://eur.bbcook.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gaf.iojbl.cn

[U04] Py：变量调试打印
来源：http://dtl.yj202588.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bmy.xuanzx.com

[U05] Py：列表去重且保序
来源：http://mol.epnwcf.com

list(dict.fromkeys(arr))
来源：http://gkg.sxryk.cn

[U06] Py：合并两个字典
来源：http://xdq.zhengqikj.top

{**a, **b}
来源：http://tgv.shuidangran.top

[U07] Py：反转字典键值
来源：http://kjc.daxiang520.top

{v: k for k, v in d.items()}
来源：http://izu.uphjek.com

[U08] Py：展平二维列表
来源：http://tta.zdqjudy.top

[y for x in nested for y in x]
来源：http://mcc.svipenyu.cn

[U09] Py：字典取最大值的键
来源：http://wtj.cqqwz.cn

max(d, key=d.get)
来源：http://alh.jinqigufen.top

[U10] Py：按值排序字典
来源：http://kgq.guannengcc.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ili.zdqjudy.top

[U11] Py：生成器表达式
来源：http://tsp.mhx1999.top

(x * 2 for x in arr)
来源：http://awc.chenlongwang.top

[U12] Py：取出现最多的 3 个元素
来源：http://bdt.ppjwa.cn

Counter(arr).most_common(3)
来源：http://djr.mhx1999.top

[U13] Py：固定长度队列
来源：http://tai.sxryk.cn

deque(maxlen=10)
来源：http://ciy.ydzc1.top

[U14] Py：分组收集到列表
来源：http://osx.aibaodan.cn

defaultdict(list)
来源：http://eoh.jinghuilouyu.cn

[U15] Py：高精度计时
来源：http://gcn.ydzc1.top

t = time.perf_counter()
来源：http://lrs.shangyingyoupin.top

[U16] Py：命令行参数解析
来源：http://ybn.shanyushiyangtech.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ohb.mhx1999.top

[U17] Py：初始化日志
来源：http://vjs.c1oappe.top

logging.basicConfig(level=logging.INFO)
来源：http://spi.havefunace.top

[U18] Py：预编译正则
来源：http://axk.52xcode.cn

pat = re.compile(r"\d+")
来源：http://kux.sxryk.cn

[U19] Py：正则替换带回调
来源：http://tsb.jinqigufen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gxw.tianlin.xyz

[U20] Py：缓存函数结果
来源：http://euw.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://nab.tanke756.top

[U21] Py：自定义上下文管理器
来源：http://rfw.yangfankeji.com

@contextlib.contextmanager
来源：http://wzd.sysykeji.top

[U22] Py：矩阵转置
来源：http://zvt.havefunace.top

list(zip(*m))
来源：http://mei.vqdsnc.cn

[U23] Py：分块读取大文件
来源：http://bki.guowangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kfj.yueranfly.top

[U24] Py：路径操作
来源：http://gon.svipenyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://apr.shangyingyoupin.top

[U25] Py：CSV 按字典读
来源：http://tkn.sufxvd.cn

csv.DictReader(f)
来源：http://umx.yuxming.cn

[U26] Py：并发下载
来源：http://chw.shanyushiyangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://see.birdmap.top

[U27] Py：异步 HTTP
来源：http://qej.smart0.xyz

aiohttp.ClientSession() 配合 async with
来源：http://aoh.0kj1m.cn

[U28] Py：类型别名
来源：http://ose.jlsjyb.cn

UserId = int
来源：http://zmm.epnwcf.com

[U29] Py：属性校验
来源：http://nco.shzxlz.cn

@property 与 @x.setter 配合
来源：http://xzi.ppjwa.cn

[U30] Py：数据类
来源：http://lzw.bjfxy.top

@dataclass(slots=True)
来源：http://wbr.fzhhl.top

[U31] Py：单测
来源：http://sbs.sxryk.cn

python -m pytest -q
来源：http://elh.yueranfly.top

[U32] Py：代码格式化
来源：http://nip.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://gyu.yfazqb.com

[U33] Py：打包发布
来源：http://mcq.xinyue.icu

python -m build  （依赖 pyproject.toml）
来源：http://psj.sysykeji.top

[U34] Py：判断编码
来源：http://cap.wangshuangyany.cn

chardet.detect(raw)
来源：http://aqb.52xcode.cn

[U35] Py：发送邮件
来源：http://mle.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sow.wangshuangyany.cn

[U36] Py：定时任务
来源：http://tfm.yfazqb.com

schedule.every(10).minutes.do(job)
来源：http://aff.jinyuanbaomall.cn

[U37] Py：读写 Excel
来源：http://dpg.jinqigfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://idc.yanxiufei.cn

[U38] Py：获取脚本所在目录
来源：http://prx.hongshengwenyu.top

Path(__file__).resolve().parent
来源：http://lfi.birdmap.top

[U39] Py：判断是否在交互环境
来源：http://knw.yongpay.top

sys.stdout.isatty()
来源：http://ztv.cucudq.cn

[U40] Py：打印到标准错误
来源：http://yiz.wangdashe.top

print("err", file=sys.stderr)
来源：http://gfc.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://xvo.smart0.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://vjb.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://uuz.cashguo.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zvi.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://ehy.aizwys.cn

namespace App\Http;
来源：http://tea.daria6918.cn

[U44] PHP：开启严格类型
来源：http://fxo.aizwys.cn

declare(strict_types=1);
来源：http://scp.fzhhl.top

[U45] PHP：类型声明与返回类型
来源：http://afh.zhixingplan.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://mwr.xuanzx.com

[U46] PHP：可空类型
来源：http://uns.bbcook.cn

?string $name = null
来源：http://dql.0kj1m.cn

[U47] PHP：联合类型
来源：http://fpa.zhoulong.xyz

int|string $id
来源：http://zba.jiagoushi.top

[U48] PHP：纯枚举
来源：http://jqe.nanxinkj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mld.zhiwuduotai.top

[U49] PHP：只读属性
来源：http://xfd.dashuyun.cn

public readonly string $name
来源：http://wed.hnqzz.top

[U50] PHP：构造器属性提升
来源：http://wcz.redwolf501.top

public function __construct(private int $id) {}
来源：http://vpb.hywenlv.cn

[U51] PHP：数组解构
来源：http://jxs.hfpthk.cn

[$a, $b] = $arr;
来源：http://qhc.hammf.cn

[U52] PHP：箭头函数
来源：http://cqe.shuidangran.top

$double = fn($x) => $x * 2;
来源：http://tva.zycfv.cn

[U53] PHP：空合并运算符
来源：http://oog.pycfn.com

$v = $a ?? $b ?? "default";
来源：http://tbf.hongshengwenyu.top

[U54] PHP：空安全调用
来源：http://kyp.hcnkem.com

$obj?->method()
来源：http://xlo.quarkkingdee.top

[U55] PHP：match 表达式
来源：http://ipy.pengpengdd.cyou

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ubi.fktsv.cn

[U56] PHP：命名参数
来源：http://bfa.havefunace.top

f(a: 1, b: 2)
来源：http://pyr.dashuyun.cn

[U57] PHP：字符串插值
来源：http://exf.hongshengwenyu.top

"值: {$a}"
来源：http://ade.yj202588.top

[U58] PHP：数组三件套
来源：http://sat.ivvv.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ery.hywenlv.cn

[U59] PHP：自定义排序
来源：http://uxz.kuanghao11.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fer.zhijiandao.cn

[U60] PHP：JSON 编解码
来源：http://xph.zdbjq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tgq.ydjk.org.cn

[U61] PHP：正则
来源：http://zkp.jinqigufen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vyl.aibaodan.cn

[U62] PHP：日期对象
来源：http://pjo.redwolf501.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://teh.jqgfzy.top

[U63] PHP：文件读写
来源：http://kwy.9152youxi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hbe.jinqigufen.top

[U64] PHP：目录遍历
来源：http://svq.meibo888.top

glob("dir/*.php");  scandir("dir");
来源：http://ksv.zhijiandao.cn

[U65] PHP：会话
来源：http://ocx.hnqzz.top

session_start();  $_SESSION["uid"] = 1;
来源：http://iye.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://tio.gzhubu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pbq.ydzc1.top

[U67] PHP：处理文件上传
来源：http://xwd.smart0.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lhk.pengpengdd.cyou

[U68] PHP：PDO 连接
来源：http://nsc.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gmd.uphjek.com

[U69] PHP：PDO 预处理
来源：http://jcz.vqdsnc.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zpl.kuanghao11.cn

[U70] PHP：PDO 事务
来源：http://hlz.zhijiandao.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dkl.iojbl.cn

[U71] PHP：抛出异常
来源：http://bad.kuanghao11.cn

throw new RuntimeException("失败", 500);
来源：http://inp.andypj.xyz

[U72] PHP：写错误日志
来源：http://ynl.wangshuangyany.cn

error_log("失败: " . $e->getMessage());
来源：http://rek.sysykeji.top

[U73] PHP：读取 ini 配置
来源：http://jwf.sweek.top

parse_ini_file("config.ini", true)
来源：http://jhd.nanxuanxn.top

[U74] PHP：读取环境变量
来源：http://erb.kuanghao11.cn

getenv("APP_ENV") ?: "production"
来源：http://svo.ybcxt.top

[U75] PHP：依赖注入
来源：http://rht.sweek.top

composer require psr/container
来源：http://ptk.daria6918.cn

[U76] PHP：简单路由
来源：http://myo.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nyb.redwolf501.top

[U77] PHP：模板渲染
来源：http://ywt.nwbrower.top

composer require twig/twig
来源：http://jpj.cheryme.top

[U78] PHP：单元测试
来源：http://cww.ydzc1.top

composer require --dev phpunit/phpunit
来源：http://dab.jinyuanbaomall.cn

[U79] PHP：静态分析
来源：http://yxp.hammf.cn

composer require --dev phpstan/phpstan
来源：http://wcx.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://onz.ybcxt.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://uor.uphjek.com

[U81] JS：初始化项目
来源：http://mkx.redwolf501.top

npm init -y;  npm i express
来源：http://tif.zhoulong.xyz

[U82] JS：package.json 脚本
来源：http://dkz.quarkkingdee.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wmw.daria6918.cn

[U83] JS：ES Module 导入导出
来源：http://vht.shanyushiyangtech.top

export const a = 1;  import { a } from "./m.js";
来源：http://aea.jinyuanbaomall.cn

[U84] JS：CommonJS 写法
来源：http://ftq.snrcjt.cn

module.exports = { a };  const { a } = require("./m");
来源：http://aoj.0kj1m.cn

[U85] JS：可选链
来源：http://kdu.jinqigufen.top

a?.b?.c
来源：http://mls.sxryk.cn

[U86] JS：空值合并
来源：http://wek.hesvh.cn

a ?? b
来源：http://djf.nanxuanxn.top

[U87] JS：解构默认值
来源：http://nru.shanyushiyangtech.top

const { a = 1, b = 2 } = obj;
来源：http://orh.xziqi.cn

[U88] JS：对象展开合并
来源：http://cik.hysaishi.cn

{ ...a, ...b }
来源：http://jdt.fanxiaobao.xyz

[U89] JS：数组去重
来源：http://wgu.hywenlv.cn

[...new Set(arr)]
来源：http://pqk.pycfn.com

[U90] JS：数字数组排序
来源：http://zpo.zdbjq.cn

[...arr].sort((a, b) => a - b)
来源：http://led.vqdsnc.cn

[U91] JS：对象键值遍历
来源：http://tim.kuanghao11.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ary.jinqigfzy.top

[U92] JS：深拷贝
来源：http://cak.hcnkem.com

structuredClone(obj)
来源：http://mpp.yfazqb.com

[U93] JS：模板字符串
来源：http://vrc.chenlongwang.top

`共 ${n} 条`
来源：http://cvc.chenzaomai.com

[U94] JS：箭头函数
来源：http://etc.fanxiaobao.xyz

const double = x => x * 2;
来源：http://bjs.yuanzhike.top

[U95] JS：Promise 包装
来源：http://pul.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://ojy.jianghu66.top

[U96] JS：async/await 与异常
来源：http://oos.ydzc1.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lqb.zycfv.cn

[U97] JS：并发请求
来源：http://yts.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xrh.guannengcc.top

[U98] JS：fetch 带 JSON
来源：http://ucc.gotoacloud.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://geh.yongpay.top

[U99] JS：事件监听
来源：http://dkw.quarkkingdee.top

el.addEventListener("click", e => {})
来源：http://szv.guannengcc.top

[U100] JS：DOM 查询
来源：http://wyq.yuanzhike.top

document.querySelector(".item")
来源：http://jie.xylfe.cn

[U101] JS：classList 操作
来源：http://pce.zycfv.cn

el.classList.toggle("active")
来源：http://eln.vqdsnc.cn

[U102] JS：本地存储
来源：http://yoj.zhongyouzk.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xke.fktsv.cn

[U103] JS：定时器
来源：http://onw.yvedp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rkm.xinyue.icu

[U104] JS：防抖
来源：http://kcm.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bnk.cashguo.top

[U105] JS：节流
来源：http://prj.zhijiandao.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blg.jinghuilouyu.cn

[U106] JS：日期格式化
来源：http://oht.iojbl.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nkd.dianchejie.cn

[U107] JS：数字千分位
来源：http://bku.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://enr.xuanzx.com

[U108] JS：随机整数
来源：http://oka.tian-w.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bii.fengsongda.top

[U109] JS：数组分组
来源：http://zmg.jinqigfzy.top

Object.groupBy(arr, x => x.type)
来源：http://mhk.vehdjk.com

[U110] JS：数组分块
来源：http://bff.hnqzz.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yjx.hnxiangtu.top

[U111] JS：对象转 Map
来源：http://vpf.tianlin.xyz

new Map(Object.entries(obj))
来源：http://tkc.smart0.xyz

[U112] JS：字符串补位
来源：http://dlc.chenjidiqi.icu

"7".padStart(3, "0")
来源：http://orq.yvedp.cn

[U113] JS：正则替换全部
来源：http://hok.xuanzx.com

s.replaceAll("a", "b")
来源：http://twk.hnxiangtu.top

[U114] JS：JSON 深比较
来源：http://whu.gaohongyu789.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://kfo.pengpengdd.cyou

[U115] JS：生成 UUID
来源：http://boy.kuanghao11.cn

crypto.randomUUID()
来源：http://qfa.shuidangran.top

[U116] JS：类型检查（JSDoc）
来源：http://xti.feifeiyinyue.top

/** @param {string} name */ function f(name) {}
来源：http://wxh.hnqzz.top


<!-- 参考信息 -->