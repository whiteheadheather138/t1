代发 wailian999

[T29] Swift：guard 提前返回
来源：http://jqq.fanxiaobao.xyz

guard let x = opt else { return }
来源：http://lph.hywenlv.cn

[T30] Swift：协议
来源：http://pvp.wangshuangyany.cn

protocol Shape { func area() -> Double }
来源：http://kny.hfpthk.cn

[T31] Lua：Hello World
来源：http://vvu.epnwcf.com

print("Hello")
来源：http://jmj.mhx1999.top

[T32] Lua：局部变量
来源：http://ebf.ydjk.org.cn

local a = 1
来源：http://jrn.gaohongyu789.top

[T33] Lua：表（数组）
来源：http://jdi.fanxiaobao.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://tvv.jyoumei.cn

[T34] Lua：遍历表
来源：http://kqi.zdbjq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hlc.shanyushiyangtech.top

[T35] Lua：字典表
来源：http://eim.zhengqikj.top

local d = { a = 1 };  d.b = 2
来源：http://bsh.xziqi.cn

[T36] Lua：函数
来源：http://idj.wangdashe.top

function add(a, b) return a + b end
来源：http://hxa.ybcxt.top

[T37] Lua：字符串拼接
来源：http://gpt.fzhhl.top

"a" .. "b"
来源：http://hhm.svipenyu.cn

[T38] Lua：条件
来源：http://jyl.havefunace.top

if x > 0 then print("正") end
来源：http://jtm.dashuyun.cn

[T39] Lua：模式匹配
来源：http://lnp.yj20258888.top

string.find(s, "%d+")
来源：http://shk.yvedp.cn

[T40] Lua：元表
来源：http://izr.andypj.xyz

setmetatable({}, { __index = base })
来源：http://rwc.birdmap.top

[T41] Perl：Hello World
来源：http://lzn.yonumen.top

print "Hello\n";
来源：http://fiz.ehwqpu.com

[T42] Perl：变量类型
来源：http://nni.zhongyouzk.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aqh.feifeiyinyue.top

[T43] Perl：字符串插值
来源：http://evw.hammf.cn

"值: $a"
来源：http://hhx.jinghuilouyu.cn

[T44] Perl：条件
来源：http://dal.jinghuilouyu.cn

if ($a > 0) { print "正"; }
来源：http://xia.gogol.net.cn

[T45] Perl：数组遍历
来源：http://stk.epnwcf.com

for my $x (@arr) { print $x; }
来源：http://tmz.jiagoushi.top

[T46] Perl：哈希操作
来源：http://gvt.epnwcf.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fwa.epnwcf.com

[T47] Perl：正则捕获
来源：http://hii.sysykeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://leq.zdbjq.cn

[T48] Perl：正则替换
来源：http://qyw.9152youxi.cn

$s =~ s/old/new/g;
来源：http://qsq.shzxlz.cn

[T49] Perl：函数
来源：http://drv.cashguo.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gmi.ppjwa.cn

[T50] Perl：逐行读文件
来源：http://mdt.havefunace.top

open my $fh, "<", "a.txt" or die $!;
来源：http://okv.jlsjyb.cn

while (my $line = <$fh>) { print $line; }
来源：http://duq.cheryme.top

[T51] Scala：Hello World
来源：http://jfb.ppjwa.cn

println("Hello")
来源：http://tbk.ehwqpu.com

[T52] Scala：变量
来源：http://qer.meibo888.top

val a = 1;  var b = 2
来源：http://bdx.chenlongwang.top

[T53] Scala：字符串插值
来源：http://atq.ydzc1.top

s"值: $b"
来源：http://ope.yj20258888.top

[T54] Scala：集合映射
来源：http://lml.shzxlz.cn

List(1, 2, 3).map(_ * 2)
来源：http://kta.ppjwa.cn

[T55] Scala：集合过滤
来源：http://oao.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://bqf.yvedp.cn

[T56] Scala：样例类
来源：http://xkd.vehdjk.com

case class User(name: String, age: Int)
来源：http://unp.xuanzx.com

[T57] Scala：模式匹配
来源：http://euy.9152youxi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ivk.zdbjq.cn

[T58] Scala：函数定义
来源：http://rwk.ehwqpu.com

def add(a: Int, b: Int): Int = a + b
来源：http://uqn.zhiwuduotai.top

[T59] Scala：循环
来源：http://cmd.bbcook.cn

for (i <- 1 to 10) println(i)
来源：http://cqw.fzhhl.top

[T60] Scala：折叠
来源：http://vjd.hnxiangtu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fyl.hysaishi.cn

================================================================================
来源：http://urt.jinqigfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vgq.zhoulong.xyz

================================================================================
来源：http://vzi.haohaochexian.top

[U01] Py：创建虚拟环境
来源：http://srk.jyoumei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qtm.316326.xyz

[U02] Py：导出 / 安装依赖
来源：http://zyi.bjfxy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gcn.cashguo.top

[U03] Py：加载 .env 配置
来源：http://pik.zycfv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://buc.jyoumei.cn

[U04] Py：变量调试打印
来源：http://vlt.zhijiandao.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fni.jqgfzy.top

[U05] Py：列表去重且保序
来源：http://jdn.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://jrp.fengsongda.top

[U06] Py：合并两个字典
来源：http://aup.c1oappe.top

{**a, **b}
来源：http://giq.zhoulong.xyz

[U07] Py：反转字典键值
来源：http://rck.nwbrower.top

{v: k for k, v in d.items()}
来源：http://gps.yueranfly.top

[U08] Py：展平二维列表
来源：http://hlr.vqdsnc.cn

[y for x in nested for y in x]
来源：http://nyq.wangshuangyany.cn

[U09] Py：字典取最大值的键
来源：http://ppk.jqgfzy.top

max(d, key=d.get)
来源：http://nuu.smart0.xyz

[U10] Py：按值排序字典
来源：http://jot.sysykeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wcv.shzxlz.cn

[U11] Py：生成器表达式
来源：http://ruk.hammf.cn

(x * 2 for x in arr)
来源：http://oyo.zycfv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tgz.yangfankeji.com

Counter(arr).most_common(3)
来源：http://rxf.dashuyun.cn

[U13] Py：固定长度队列
来源：http://dqb.fehbvm.com

deque(maxlen=10)
来源：http://mju.vqdsnc.cn

[U14] Py：分组收集到列表
来源：http://uch.tianlin.xyz

defaultdict(list)
来源：http://uge.fanxiaobao.xyz

[U15] Py：高精度计时
来源：http://mvc.wangdashe.top

t = time.perf_counter()
来源：http://kul.cheryme.top

[U16] Py：命令行参数解析
来源：http://ess.daria6918.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kkn.xuetiantiany.cn

[U17] Py：初始化日志
来源：http://clk.bjfxy.top

logging.basicConfig(level=logging.INFO)
来源：http://zfi.xylfe.cn

[U18] Py：预编译正则
来源：http://olw.sxryk.cn

pat = re.compile(r"\d+")
来源：http://ddr.ehwqpu.com

[U19] Py：正则替换带回调
来源：http://boo.jyoumei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jpy.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://jjo.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://aoq.haohaochexian.top

[U21] Py：自定义上下文管理器
来源：http://cbi.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://pcr.haohaochexian.top

[U22] Py：矩阵转置
来源：http://eyk.aizwys.cn

list(zip(*m))
来源：http://odu.fengsongda.top

[U23] Py：分块读取大文件
来源：http://ttj.jiagoushi.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mhi.hysaishi.cn

[U24] Py：路径操作
来源：http://moz.fanxiaobao.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ocs.sweek.top

[U25] Py：CSV 按字典读
来源：http://msn.tanke756.top

csv.DictReader(f)
来源：http://akf.gzhubu.top

[U26] Py：并发下载
来源：http://dnf.xuanzx.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fwz.yvedp.cn

[U27] Py：异步 HTTP
来源：http://vax.zdbjq.cn

aiohttp.ClientSession() 配合 async with
来源：http://iby.gzhubu.top

[U28] Py：类型别名
来源：http://pfq.zhaomingkeji.xyz

UserId = int
来源：http://tst.jinqigufen.top

[U29] Py：属性校验
来源：http://soq.cashguo.top

@property 与 @x.setter 配合
来源：http://axh.jqgufenzy.top

[U30] Py：数据类
来源：http://uhu.bjfxy.top

@dataclass(slots=True)
来源：http://deb.dashuyun.cn

[U31] Py：单测
来源：http://vci.yonumen.top

python -m pytest -q
来源：http://gis.yuxming.cn

[U32] Py：代码格式化
来源：http://tjh.nanxuanxn.top

ruff format . && ruff check --fix .
来源：http://adr.bbcook.cn

[U33] Py：打包发布
来源：http://giw.feifeiyinyue.top

python -m build  （依赖 pyproject.toml）
来源：http://iki.gotoacloud.top

[U34] Py：判断编码
来源：http://nxn.fengsongda.top

chardet.detect(raw)
来源：http://vpe.gaohongyu789.top

[U35] Py：发送邮件
来源：http://ocj.daria6918.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vzx.ydzc1.top

[U36] Py：定时任务
来源：http://kex.tarul.cn

schedule.every(10).minutes.do(job)
来源：http://xpe.chenzaomai.com

[U37] Py：读写 Excel
来源：http://qrq.bjfxy.top

pandas.read_excel / DataFrame.to_excel
来源：http://sbc.andypj.xyz

[U38] Py：获取脚本所在目录
来源：http://zag.andypj.xyz

Path(__file__).resolve().parent
来源：http://ozt.0kj1m.cn

[U39] Py：判断是否在交互环境
来源：http://mpb.jinqigufen.top

sys.stdout.isatty()
来源：http://wyr.hcnkem.com

[U40] Py：打印到标准错误
来源：http://ozp.zhaomingkeji.xyz

print("err", file=sys.stderr)
来源：http://otx.dianchejie.cn

[U41] PHP：初始化 Composer 项目
来源：http://tso.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://eyl.ppjwa.cn

[U42] PHP：PSR-4 自动加载
来源：http://uwc.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kui.fehbvm.com

[U43] PHP：声明命名空间
来源：http://jpy.sjlbkw.cn

namespace App\Http;
来源：http://ocq.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://mxt.zhiwuduotai.top

declare(strict_types=1);
来源：http://phu.hongshengwenyu.top

[U45] PHP：类型声明与返回类型
来源：http://cxg.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jip.zdqjudy.top

[U46] PHP：可空类型
来源：http://oni.zhiwuduotai.top

?string $name = null
来源：http://geh.ppjwa.cn

[U47] PHP：联合类型
来源：http://dpt.ppjwa.cn

int|string $id
来源：http://elq.ybcxt.top

[U48] PHP：纯枚举
来源：http://qie.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://amy.cheryme.top

[U49] PHP：只读属性
来源：http://ecl.redwolf501.top

public readonly string $name
来源：http://mmr.tian-w.cn

[U50] PHP：构造器属性提升
来源：http://ony.zhoulong.xyz

public function __construct(private int $id) {}
来源：http://kgd.tanke756.top

[U51] PHP：数组解构
来源：http://shz.ivvv.top

[$a, $b] = $arr;
来源：http://ypx.ppjwa.cn

[U52] PHP：箭头函数
来源：http://cpk.daria6918.cn

$double = fn($x) => $x * 2;
来源：http://ufw.cheryme.top

[U53] PHP：空合并运算符
来源：http://pax.epnwcf.com

$v = $a ?? $b ?? "default";
来源：http://idf.jqgfzy.top

[U54] PHP：空安全调用
来源：http://xpq.epnwcf.com

$obj?->method()
来源：http://sof.hywenlv.cn

[U55] PHP：match 表达式
来源：http://qec.jinghuilouyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ere.jinyuanbaomall.cn

[U56] PHP：命名参数
来源：http://sio.hysaishi.cn

f(a: 1, b: 2)
来源：http://nbi.daxiang520.top

[U57] PHP：字符串插值
来源：http://ers.cucudq.cn

"值: {$a}"
来源：http://syz.hywenlv.cn

[U58] PHP：数组三件套
来源：http://yxv.nanxuanxn.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://grj.shanyushiyangkeji.top

[U59] PHP：自定义排序
来源：http://ndo.ctjpmb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rzk.ctjpmb.com

[U60] PHP：JSON 编解码
来源：http://cuq.xinyue.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://roh.gzhubu.top

[U61] PHP：正则
来源：http://jzc.gogol.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vwc.snrcjt.cn

[U62] PHP：日期对象
来源：http://cnl.gaohongyu789.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sfc.xylfe.cn

[U63] PHP：文件读写
来源：http://cab.sjlbkw.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ofx.pengpengdd.cyou

[U64] PHP：目录遍历
来源：http://bpn.zdbjq.cn

glob("dir/*.php");  scandir("dir");
来源：http://dky.hnqzz.top

[U65] PHP：会话
来源：http://duc.ehwqpu.com

session_start();  $_SESSION["uid"] = 1;
来源：http://jzr.xuetiantiany.cn

[U66] PHP：设置 Cookie
来源：http://twh.mhx1999.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nou.c1oappe.top

[U67] PHP：处理文件上传
来源：http://whi.mhx1999.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tbq.zhixingplan.top

[U68] PHP：PDO 连接
来源：http://kve.yj202588.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ncm.316326.xyz

[U69] PHP：PDO 预处理
来源：http://viv.fzhhl.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wok.sysykeji.top

[U70] PHP：PDO 事务
来源：http://pia.zhongyouzk.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://acd.shuidangran.top

[U71] PHP：抛出异常
来源：http://rlo.jinqigfzy.top

throw new RuntimeException("失败", 500);
来源：http://dbk.ivvv.top

[U72] PHP：写错误日志
来源：http://gzr.316326.xyz

error_log("失败: " . $e->getMessage());
来源：http://gkk.hysaishi.cn

[U73] PHP：读取 ini 配置
来源：http://sry.chenjidiqi.icu

parse_ini_file("config.ini", true)
来源：http://nix.ybcxt.top

[U74] PHP：读取环境变量
来源：http://ifj.zhongyouzk.top

getenv("APP_ENV") ?: "production"
来源：http://fyc.316326.xyz

[U75] PHP：依赖注入
来源：http://lpj.svipenyu.cn

composer require psr/container
来源：http://gtc.jlsjyb.cn

[U76] PHP：简单路由
来源：http://wkf.yuanzhike.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tch.cheryme.top

[U77] PHP：模板渲染
来源：http://rnf.jqgufenzy.top

composer require twig/twig
来源：http://hdh.yanxiufei.cn

[U78] PHP：单元测试
来源：http://als.tanke756.top

composer require --dev phpunit/phpunit
来源：http://kye.mhx1999.top

[U79] PHP：静态分析
来源：http://ctn.zycfv.cn

composer require --dev phpstan/phpstan
来源：http://nai.smart0.xyz

[U80] PHP：代码规范修复
来源：http://xod.kuanghao11.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://glg.hnxiangtu.top

[U81] JS：初始化项目
来源：http://xji.gzhubu.top

npm init -y;  npm i express
来源：http://myx.zhaomingkeji.xyz

[U82] JS：package.json 脚本
来源：http://lgx.wangdashe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rfy.chenjidiqi.icu

[U83] JS：ES Module 导入导出
来源：http://gvc.yongpay.top

export const a = 1;  import { a } from "./m.js";
来源：http://ffa.zhoulong.xyz

[U84] JS：CommonJS 写法
来源：http://rcp.snrcjt.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tmv.gzhubu.top

[U85] JS：可选链
来源：http://hvk.yj20258888.top

a?.b?.c
来源：http://cbn.chenjidiqi.icu

[U86] JS：空值合并
来源：http://njm.fanxiaobao.xyz

a ?? b
来源：http://rjg.hcnkem.com

[U87] JS：解构默认值
来源：http://ntg.shuidangran.top

const { a = 1, b = 2 } = obj;
来源：http://xdm.yonumen.top

[U88] JS：对象展开合并
来源：http://dfd.fktsv.cn

{ ...a, ...b }
来源：http://jhh.yj20258.top

[U89] JS：数组去重
来源：http://sso.epnwcf.com

[...new Set(arr)]
来源：http://qxi.xuanzx.com

[U90] JS：数字数组排序
来源：http://oyc.chenzaomai.com

[...arr].sort((a, b) => a - b)
来源：http://mak.chenzaomai.com

[U91] JS：对象键值遍历
来源：http://ath.ehwqpu.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bpe.yj202588.top

[U92] JS：深拷贝
来源：http://jfu.tianlin.xyz

structuredClone(obj)
来源：http://ijr.nanxuanxn.top

[U93] JS：模板字符串
来源：http://tmn.zhengqikj.top

`共 ${n} 条`
来源：http://ooq.haohaochexian.top

[U94] JS：箭头函数
来源：http://yuj.vehdjk.com

const double = x => x * 2;
来源：http://osa.gzhubu.top

[U95] JS：Promise 包装
来源：http://sqw.ctjpmb.com

new Promise((resolve, reject) => {})
来源：http://pww.zdbjq.cn

[U96] JS：async/await 与异常
来源：http://ekw.cashguo.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ilv.ivvv.top

[U97] JS：并发请求
来源：http://eqb.yfazqb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://lcm.zycfv.cn

[U98] JS：fetch 带 JSON
来源：http://ihi.tarul.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ppj.bbcook.cn

[U99] JS：事件监听
来源：http://yqz.yj20258.top

el.addEventListener("click", e => {})
来源：http://fco.dianchejie.cn

[U100] JS：DOM 查询
来源：http://jgq.hnxiangtu.top

document.querySelector(".item")
来源：http://arm.yueranfly.top

[U101] JS：classList 操作
来源：http://glk.9152youxi.cn

el.classList.toggle("active")
来源：http://nhh.havefunace.top

[U102] JS：本地存储
来源：http://qiu.aibaodan.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jsa.daxiang520.top

[U103] JS：定时器
来源：http://hwo.bbcook.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oyr.daria6918.cn

[U104] JS：防抖
来源：http://kcg.cdnleiting.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dnh.vehdjk.com

[U105] JS：节流
来源：http://lok.xingfuxueyuan.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mkl.sxryk.cn

[U106] JS：日期格式化
来源：http://jpp.9152youxi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hpq.zhengqikj.top

[U107] JS：数字千分位
来源：http://knv.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ogs.shangyingyoupin.top

[U108] JS：随机整数
来源：http://mkf.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gue.meibo888.top

[U109] JS：数组分组
来源：http://qii.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://wes.meibo888.top

[U110] JS：数组分块
来源：http://hfu.hysaishi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nny.zycfv.cn

[U111] JS：对象转 Map
来源：http://gik.guowangkeji.top

new Map(Object.entries(obj))
来源：http://amz.jqgfzy.top

[U112] JS：字符串补位
来源：http://ner.aibaodan.cn

"7".padStart(3, "0")
来源：http://ndx.gogol.net.cn

[U113] JS：正则替换全部
来源：http://bsr.cdnleiting.top

s.replaceAll("a", "b")
来源：http://taz.ctjpmb.com

[U114] JS：JSON 深比较
来源：http://zik.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wnt.bjfxy.top

[U115] JS：生成 UUID
来源：http://ner.dianchejie.cn

crypto.randomUUID()
来源：http://stn.sjlbkw.cn

[U116] JS：类型检查（JSDoc）
来源：http://stg.tian-w.cn

/** @param {string} name */ function f(name) {}
来源：http://byn.hywenlv.cn


<!-- 参考信息 -->