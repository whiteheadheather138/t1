代发 wailian999

[T29] Swift：guard 提前返回
来源：http://rck.jinghuilouyu.cn

guard let x = opt else { return }
来源：http://wqx.cashguo.top

[T30] Swift：协议
来源：http://eip.xingfuxueyuan.xyz

protocol Shape { func area() -> Double }
来源：http://sfb.daxiang520.top

[T31] Lua：Hello World
来源：http://vxk.dashuyun.cn

print("Hello")
来源：http://tep.kuanghao11.cn

[T32] Lua：局部变量
来源：http://eyn.shanyushiyangtech.top

local a = 1
来源：http://djn.wangshuangyany.cn

[T33] Lua：表（数组）
来源：http://huk.xuetiantiany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uhn.jyoumei.cn

[T34] Lua：遍历表
来源：http://rwg.yj20258.top

for i, v in ipairs(t) do print(i, v) end
来源：http://llo.aibaodan.cn

[T35] Lua：字典表
来源：http://lno.gotoacloud.top

local d = { a = 1 };  d.b = 2
来源：http://gif.guowangkeji.top

[T36] Lua：函数
来源：http://kvy.tian-w.cn

function add(a, b) return a + b end
来源：http://nko.jinqigufen.top

[T37] Lua：字符串拼接
来源：http://hgc.yuxming.cn

"a" .. "b"
来源：http://afw.jianghu66.top

[T38] Lua：条件
来源：http://kdn.sxryk.cn

if x > 0 then print("正") end
来源：http://fjj.cqqwz.cn

[T39] Lua：模式匹配
来源：http://aho.jinghuilouyu.cn

string.find(s, "%d+")
来源：http://wxe.gotoacloud.top

[T40] Lua：元表
来源：http://smj.uphjek.com

setmetatable({}, { __index = base })
来源：http://wdn.meibo888.top

[T41] Perl：Hello World
来源：http://gyb.9152youxi.cn

print "Hello\n";
来源：http://isf.bjfxy.top

[T42] Perl：变量类型
来源：http://qju.jyoumei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fcn.ybcxt.top

[T43] Perl：字符串插值
来源：http://tti.chenlongwang.top

"值: $a"
来源：http://xir.sysykeji.top

[T44] Perl：条件
来源：http://doc.kuanghao11.cn

if ($a > 0) { print "正"; }
来源：http://zir.ybcxt.top

[T45] Perl：数组遍历
来源：http://wro.xuanzx.com

for my $x (@arr) { print $x; }
来源：http://abq.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://jus.shuidangran.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://okm.redwolf501.top

[T47] Perl：正则捕获
来源：http://prb.aibaodan.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://blw.svipenyu.cn

[T48] Perl：正则替换
来源：http://ese.bjfxy.top

$s =~ s/old/new/g;
来源：http://fvw.yangfankeji.com

[T49] Perl：函数
来源：http://utc.cashguo.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wjz.fehbvm.com

[T50] Perl：逐行读文件
来源：http://llb.yfazqb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://xer.chenzaomai.com

while (my $line = <$fh>) { print $line; }
来源：http://ipd.hnxiangtu.top

[T51] Scala：Hello World
来源：http://uoa.yj202588.top

println("Hello")
来源：http://zki.gogol.net.cn

[T52] Scala：变量
来源：http://vpn.iojbl.cn

val a = 1;  var b = 2
来源：http://bdb.daxiang520.top

[T53] Scala：字符串插值
来源：http://bxx.pengpengdd.cyou

s"值: $b"
来源：http://oel.bbcook.cn

[T54] Scala：集合映射
来源：http://cdf.hnxiangtu.top

List(1, 2, 3).map(_ * 2)
来源：http://rku.kuanghao11.cn

[T55] Scala：集合过滤
来源：http://zvq.gaohongyu789.top

List(1, 2, 3).filter(_ > 1)
来源：http://jjw.epnwcf.com

[T56] Scala：样例类
来源：http://pqh.aibaodan.cn

case class User(name: String, age: Int)
来源：http://eam.xuanzx.com

[T57] Scala：模式匹配
来源：http://yra.haohaochexian.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kpv.snrcjt.cn

[T58] Scala：函数定义
来源：http://sae.0kj1m.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gnr.vehdjk.com

[T59] Scala：循环
来源：http://hhk.bjfxy.top

for (i <- 1 to 10) println(i)
来源：http://wki.tarul.cn

[T60] Scala：折叠
来源：http://rnd.daxiang520.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mef.zhengqikj.top

================================================================================
来源：http://ome.sufxvd.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ibr.hammf.cn

================================================================================
来源：http://lae.jqgufenzy.top

[U01] Py：创建虚拟环境
来源：http://fnq.shanyushiyangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://fna.ehwqpu.com

[U02] Py：导出 / 安装依赖
来源：http://jxf.chenzaomai.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dra.pengpengdd.cyou

[U03] Py：加载 .env 配置
来源：http://hmt.ybcxt.top

from dotenv import load_dotenv; load_dotenv()
来源：http://goa.yvedp.cn

[U04] Py：变量调试打印
来源：http://bdy.jiagoushi.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://atk.tarul.cn

[U05] Py：列表去重且保序
来源：http://bjs.ydzc1.top

list(dict.fromkeys(arr))
来源：http://emf.shzxlz.cn

[U06] Py：合并两个字典
来源：http://ody.tianlin.xyz

{**a, **b}
来源：http://mhj.nanxinkj.top

[U07] Py：反转字典键值
来源：http://ept.xziqi.cn

{v: k for k, v in d.items()}
来源：http://dnm.hfpthk.cn

[U08] Py：展平二维列表
来源：http://smp.316326.xyz

[y for x in nested for y in x]
来源：http://dbt.xylfe.cn

[U09] Py：字典取最大值的键
来源：http://wzz.zhiwuduotai.top

max(d, key=d.get)
来源：http://rrk.birdmap.top

[U10] Py：按值排序字典
来源：http://yfq.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yfe.cheryme.top

[U11] Py：生成器表达式
来源：http://fiq.hnxiangtu.top

(x * 2 for x in arr)
来源：http://caf.vehdjk.com

[U12] Py：取出现最多的 3 个元素
来源：http://zxw.gaohongyu789.top

Counter(arr).most_common(3)
来源：http://lfz.smart0.xyz

[U13] Py：固定长度队列
来源：http://ldd.hesvh.cn

deque(maxlen=10)
来源：http://gsm.haohaochexian.top

[U14] Py：分组收集到列表
来源：http://vsp.wangshuangyany.cn

defaultdict(list)
来源：http://bko.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://uig.meibo888.top

t = time.perf_counter()
来源：http://ueu.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://hpp.guowangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zyk.epnwcf.com

[U17] Py：初始化日志
来源：http://rtv.jinqigufen.top

logging.basicConfig(level=logging.INFO)
来源：http://yjj.sysykeji.top

[U18] Py：预编译正则
来源：http://nsv.zhengqikj.top

pat = re.compile(r"\d+")
来源：http://rua.chenlongwang.top

[U19] Py：正则替换带回调
来源：http://ajy.ppjwa.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kno.kuanghao11.cn

[U20] Py：缓存函数结果
来源：http://tfg.quarkkingdee.top

@functools.lru_cache(maxsize=None)
来源：http://urv.nanxuanxn.top

[U21] Py：自定义上下文管理器
来源：http://izx.pengpengdd.cyou

@contextlib.contextmanager
来源：http://xbl.zhengqikj.top

[U22] Py：矩阵转置
来源：http://tzx.redwolf501.top

list(zip(*m))
来源：http://qmk.snrcjt.cn

[U23] Py：分块读取大文件
来源：http://xti.zycfv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ncl.yanxiufei.cn

[U24] Py：路径操作
来源：http://yap.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mql.jiagoushi.top

[U25] Py：CSV 按字典读
来源：http://klb.nanxuanxn.top

csv.DictReader(f)
来源：http://rtd.yonumen.top

[U26] Py：并发下载
来源：http://zgv.fanxiaobao.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bqo.ydzc1.top

[U27] Py：异步 HTTP
来源：http://psq.zhaomingkeji.xyz

aiohttp.ClientSession() 配合 async with
来源：http://grq.xuanzx.com

[U28] Py：类型别名
来源：http://sdg.yj20258.top

UserId = int
来源：http://luw.jyoumei.cn

[U29] Py：属性校验
来源：http://aok.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://vid.hysaishi.cn

[U30] Py：数据类
来源：http://gzz.hfpthk.cn

@dataclass(slots=True)
来源：http://wfl.ybcxt.top

[U31] Py：单测
来源：http://rut.zycfv.cn

python -m pytest -q
来源：http://smh.nwbrower.top

[U32] Py：代码格式化
来源：http://ozd.chenzaomai.com

ruff format . && ruff check --fix .
来源：http://pen.dianchejie.cn

[U33] Py：打包发布
来源：http://ebd.zdqjudy.top

python -m build  （依赖 pyproject.toml）
来源：http://liq.cdnleiting.top

[U34] Py：判断编码
来源：http://fvu.cucudq.cn

chardet.detect(raw)
来源：http://upg.birdmap.top

[U35] Py：发送邮件
来源：http://veb.ppjwa.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tdq.yfazqb.com

[U36] Py：定时任务
来源：http://tvb.yangfankeji.com

schedule.every(10).minutes.do(job)
来源：http://yel.jiagoushi.top

[U37] Py：读写 Excel
来源：http://uhc.shanyushiyangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://lad.bjfxy.top

[U38] Py：获取脚本所在目录
来源：http://onc.jyoumei.cn

Path(__file__).resolve().parent
来源：http://dpt.shuidangran.top

[U39] Py：判断是否在交互环境
来源：http://pge.kuanghao11.cn

sys.stdout.isatty()
来源：http://kcw.gzhubu.top

[U40] Py：打印到标准错误
来源：http://qvg.sxryk.cn

print("err", file=sys.stderr)
来源：http://gwp.fanxiaobao.xyz

[U41] PHP：初始化 Composer 项目
来源：http://otp.jinyuanbaomall.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ckm.bbcook.cn

[U42] PHP：PSR-4 自动加载
来源：http://sov.ctjpmb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mnw.aizwys.cn

[U43] PHP：声明命名空间
来源：http://awq.hesvh.cn

namespace App\Http;
来源：http://upy.jyoumei.cn

[U44] PHP：开启严格类型
来源：http://amn.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://yhn.meibo888.top

[U45] PHP：类型声明与返回类型
来源：http://pbi.yonumen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ppg.jlsjyb.cn

[U46] PHP：可空类型
来源：http://dmi.shanyushiyangtech.top

?string $name = null
来源：http://igg.shanyushiyangtech.top

[U47] PHP：联合类型
来源：http://lwn.ydzc1.top

int|string $id
来源：http://yoe.bjfxy.top

[U48] PHP：纯枚举
来源：http://sau.yj20258888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xqz.svipenyu.cn

[U49] PHP：只读属性
来源：http://qmn.ivvv.top

public readonly string $name
来源：http://zhv.meibo888.top

[U50] PHP：构造器属性提升
来源：http://mze.shangyingyoupin.top

public function __construct(private int $id) {}
来源：http://lyf.yj20258888.top

[U51] PHP：数组解构
来源：http://mjb.sufxvd.cn

[$a, $b] = $arr;
来源：http://vbm.fengsongda.top

[U52] PHP：箭头函数
来源：http://qnr.havefunace.top

$double = fn($x) => $x * 2;
来源：http://qvy.mhx1999.top

[U53] PHP：空合并运算符
来源：http://opo.sufxvd.cn

$v = $a ?? $b ?? "default";
来源：http://fvg.hongshengwenyu.top

[U54] PHP：空安全调用
来源：http://fix.jqgfzy.top

$obj?->method()
来源：http://uhx.yvedp.cn

[U55] PHP：match 表达式
来源：http://sfl.jyoumei.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bqa.hongshengwenyu.top

[U56] PHP：命名参数
来源：http://tes.yj20258.top

f(a: 1, b: 2)
来源：http://ejo.yvedp.cn

[U57] PHP：字符串插值
来源：http://zgo.nanxinkj.top

"值: {$a}"
来源：http://tui.chenjidiqi.icu

[U58] PHP：数组三件套
来源：http://qhp.guannengcc.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dcd.c1oappe.top

[U59] PHP：自定义排序
来源：http://ndq.xylfe.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xez.jyoumei.cn

[U60] PHP：JSON 编解码
来源：http://laz.ydzc1.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zxo.hammf.cn

[U61] PHP：正则
来源：http://wbf.cqqwz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xsp.ehwqpu.com

[U62] PHP：日期对象
来源：http://pog.zhoulong.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pct.pycfn.com

[U63] PHP：文件读写
来源：http://jsl.pycfn.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dlq.ywan-chungtsiang.top

[U64] PHP：目录遍历
来源：http://rsu.zhaomingkeji.xyz

glob("dir/*.php");  scandir("dir");
来源：http://ksx.ywan-chungtsiang.top

[U65] PHP：会话
来源：http://ewp.dashuyun.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://usg.gogol.net.cn

[U66] PHP：设置 Cookie
来源：http://ele.jinyuanbaomall.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qhf.ctjpmb.com

[U67] PHP：处理文件上传
来源：http://thg.yj20258888.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dck.haohaochexian.top

[U68] PHP：PDO 连接
来源：http://zxo.sufxvd.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gsa.wangshuangyany.cn

[U69] PHP：PDO 预处理
来源：http://swc.feifeiyinyue.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kqa.yuxming.cn

[U70] PHP：PDO 事务
来源：http://hja.jiagoushi.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://waf.yueranfly.top

[U71] PHP：抛出异常
来源：http://ycz.yueranfly.top

throw new RuntimeException("失败", 500);
来源：http://zer.hnqzz.top

[U72] PHP：写错误日志
来源：http://atq.mhx1999.top

error_log("失败: " . $e->getMessage());
来源：http://ryc.shuidangran.top

[U73] PHP：读取 ini 配置
来源：http://ysh.wangdashe.top

parse_ini_file("config.ini", true)
来源：http://aac.zhixingplan.top

[U74] PHP：读取环境变量
来源：http://mhd.feifeiyinyue.top

getenv("APP_ENV") ?: "production"
来源：http://vpe.iojbl.cn

[U75] PHP：依赖注入
来源：http://rlo.guannengcc.top

composer require psr/container
来源：http://vzb.quarkkingdee.top

[U76] PHP：简单路由
来源：http://dnc.wangdashe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sit.aibaodan.cn

[U77] PHP：模板渲染
来源：http://jlf.hnxiangtu.top

composer require twig/twig
来源：http://war.zhijiandao.cn

[U78] PHP：单元测试
来源：http://fjz.hongshengwenyu.top

composer require --dev phpunit/phpunit
来源：http://wgn.guowangkeji.top

[U79] PHP：静态分析
来源：http://ext.jinqigfzy.top

composer require --dev phpstan/phpstan
来源：http://rhq.hnqzz.top

[U80] PHP：代码规范修复
来源：http://cch.epnwcf.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://nqx.ehwqpu.com

[U81] JS：初始化项目
来源：http://vfe.dashuyun.cn

npm init -y;  npm i express
来源：http://iyh.ydjk.org.cn

[U82] JS：package.json 脚本
来源：http://ont.xingfuxueyuan.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lbd.wangshuangyany.cn

[U83] JS：ES Module 导入导出
来源：http://cec.jyoumei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xga.dashuyun.cn

[U84] JS：CommonJS 写法
来源：http://dng.cheryme.top

module.exports = { a };  const { a } = require("./m");
来源：http://thv.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://zco.yongpay.top

a?.b?.c
来源：http://qhs.aizwys.cn

[U86] JS：空值合并
来源：http://yrn.sweek.top

a ?? b
来源：http://sdf.zhijiandao.cn

[U87] JS：解构默认值
来源：http://app.fktsv.cn

const { a = 1, b = 2 } = obj;
来源：http://xyg.xylfe.cn

[U88] JS：对象展开合并
来源：http://hfn.vqdsnc.cn

{ ...a, ...b }
来源：http://ocr.feifeiyinyue.top

[U89] JS：数组去重
来源：http://udo.cheryme.top

[...new Set(arr)]
来源：http://gmi.zhoulong.xyz

[U90] JS：数字数组排序
来源：http://aje.jiagoushi.top

[...arr].sort((a, b) => a - b)
来源：http://jov.ehwqpu.com

[U91] JS：对象键值遍历
来源：http://ugn.yongpay.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://igg.xingfuxueyuan.xyz

[U92] JS：深拷贝
来源：http://vgm.smart0.xyz

structuredClone(obj)
来源：http://mzy.fzhhl.top

[U93] JS：模板字符串
来源：http://mwn.cqqwz.cn

`共 ${n} 条`
来源：http://faq.sxryk.cn

[U94] JS：箭头函数
来源：http://hpo.jinqigfzy.top

const double = x => x * 2;
来源：http://txl.zhoulong.xyz

[U95] JS：Promise 包装
来源：http://usg.sxryk.cn

new Promise((resolve, reject) => {})
来源：http://faw.zhijiandao.cn

[U96] JS：async/await 与异常
来源：http://nrk.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mcx.zhaomingkeji.xyz

[U97] JS：并发请求
来源：http://tle.sweek.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://shh.cashguo.top

[U98] JS：fetch 带 JSON
来源：http://jlf.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kru.zhixingplan.top

[U99] JS：事件监听
来源：http://dwg.pycfn.com

el.addEventListener("click", e => {})
来源：http://pug.ctjpmb.com

[U100] JS：DOM 查询
来源：http://ryx.shanyushiyangtech.top

document.querySelector(".item")
来源：http://yjy.xuanzx.com

[U101] JS：classList 操作
来源：http://des.xuanzx.com

el.classList.toggle("active")
来源：http://smf.redwolf501.top

[U102] JS：本地存储
来源：http://faz.yueranfly.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pwr.yfazqb.com

[U103] JS：定时器
来源：http://wob.ppjwa.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ipi.uphjek.com

[U104] JS：防抖
来源：http://lqu.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jlc.hysaishi.cn

[U105] JS：节流
来源：http://gtv.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pmu.jinqigfzy.top

[U106] JS：日期格式化
来源：http://nbq.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zur.xylfe.cn

[U107] JS：数字千分位
来源：http://uxq.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qgu.epnwcf.com

[U108] JS：随机整数
来源：http://fxs.yj20258.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uqh.jinqigfzy.top

[U109] JS：数组分组
来源：http://cnv.gogol.net.cn

Object.groupBy(arr, x => x.type)
来源：http://fas.tanke756.top

[U110] JS：数组分块
来源：http://raz.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ike.redwolf501.top

[U111] JS：对象转 Map
来源：http://cqq.ppjwa.cn

new Map(Object.entries(obj))
来源：http://qfl.nanxuanxn.top

[U112] JS：字符串补位
来源：http://zca.fzhhl.top

"7".padStart(3, "0")
来源：http://rkq.zdqjudy.top

[U113] JS：正则替换全部
来源：http://epu.zhijiandao.cn

s.replaceAll("a", "b")
来源：http://nhc.xziqi.cn

[U114] JS：JSON 深比较
来源：http://wer.tanke756.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://omv.daria6918.cn

[U115] JS：生成 UUID
来源：http://epe.yfazqb.com

crypto.randomUUID()
来源：http://tpf.andypj.xyz

[U116] JS：类型检查（JSDoc）
来源：http://yvb.smart0.xyz

/** @param {string} name */ function f(name) {}
来源：http://lct.0kj1m.cn


<!-- 参考信息 -->