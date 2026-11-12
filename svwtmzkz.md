代发 wailian999

[T29] Swift：guard 提前返回
来源：http://mmt.epnwcf.com

guard let x = opt else { return }
来源：http://zrt.sysykeji.top

[T30] Swift：协议
来源：http://nfc.yonumen.top

protocol Shape { func area() -> Double }
来源：http://mby.ivvv.top

[T31] Lua：Hello World
来源：http://rig.xingfuxueyuan.xyz

print("Hello")
来源：http://rye.hywenlv.cn

[T32] Lua：局部变量
来源：http://yho.316326.xyz

local a = 1
来源：http://mxz.zdqjudy.top

[T33] Lua：表（数组）
来源：http://cde.52xcode.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sks.yj202588.top

[T34] Lua：遍历表
来源：http://rrc.jqgfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ocg.vehdjk.com

[T35] Lua：字典表
来源：http://hzs.kuanghao11.cn

local d = { a = 1 };  d.b = 2
来源：http://ltv.aibaodan.cn

[T36] Lua：函数
来源：http://sir.316326.xyz

function add(a, b) return a + b end
来源：http://ycj.tarul.cn

[T37] Lua：字符串拼接
来源：http://usv.daria6918.cn

"a" .. "b"
来源：http://blu.tianlin.xyz

[T38] Lua：条件
来源：http://cuj.cucudq.cn

if x > 0 then print("正") end
来源：http://fir.zhongyouzk.top

[T39] Lua：模式匹配
来源：http://tkr.vehdjk.com

string.find(s, "%d+")
来源：http://dmr.aibaodan.cn

[T40] Lua：元表
来源：http://bhf.daria6918.cn

setmetatable({}, { __index = base })
来源：http://kuh.guowangkeji.top

[T41] Perl：Hello World
来源：http://tfv.c1oappe.top

print "Hello\n";
来源：http://veu.xinyue.icu

[T42] Perl：变量类型
来源：http://ubi.gogol.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wse.zhixingplan.top

[T43] Perl：字符串插值
来源：http://emz.guannengcc.top

"值: $a"
来源：http://rum.pengpengdd.cyou

[T44] Perl：条件
来源：http://pxw.ppjwa.cn

if ($a > 0) { print "正"; }
来源：http://qus.shanyushiyangtech.top

[T45] Perl：数组遍历
来源：http://gkn.gogol.net.cn

for my $x (@arr) { print $x; }
来源：http://obb.tian-w.cn

[T46] Perl：哈希操作
来源：http://ajo.tanke756.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fps.jyoumei.cn

[T47] Perl：正则捕获
来源：http://thl.fehbvm.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://jwy.xinyue.icu

[T48] Perl：正则替换
来源：http://fcm.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://odl.tian-w.cn

[T49] Perl：函数
来源：http://zaj.zhiwuduotai.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pqx.jinqigfzy.top

[T50] Perl：逐行读文件
来源：http://mvy.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://uog.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://aai.ctjpmb.com

[T51] Scala：Hello World
来源：http://thx.hammf.cn

println("Hello")
来源：http://dax.wangshuangyany.cn

[T52] Scala：变量
来源：http://qul.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://vxf.aibaodan.cn

[T53] Scala：字符串插值
来源：http://zac.zhixingplan.top

s"值: $b"
来源：http://nqk.jqgfzy.top

[T54] Scala：集合映射
来源：http://jsx.wangdashe.top

List(1, 2, 3).map(_ * 2)
来源：http://xgg.ivvv.top

[T55] Scala：集合过滤
来源：http://dad.chenzaomai.com

List(1, 2, 3).filter(_ > 1)
来源：http://apn.cdnleiting.top

[T56] Scala：样例类
来源：http://oeu.bjfxy.top

case class User(name: String, age: Int)
来源：http://xvx.jqgfzy.top

[T57] Scala：模式匹配
来源：http://fel.jianghu66.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xci.meibo888.top

[T58] Scala：函数定义
来源：http://rqk.jqgufenzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://qnb.cashguo.top

[T59] Scala：循环
来源：http://mpq.xylfe.cn

for (i <- 1 to 10) println(i)
来源：http://zpe.cheryme.top

[T60] Scala：折叠
来源：http://wjm.ppjwa.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://exb.9152youxi.cn

================================================================================
来源：http://cjz.yj202588.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mut.fengsongda.top

================================================================================
来源：http://smu.yangfankeji.com

[U01] Py：创建虚拟环境
来源：http://npz.xuetiantiany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sjq.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://tca.chenjidiqi.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pds.yj202588.top

[U03] Py：加载 .env 配置
来源：http://ukg.iojbl.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://evg.chenjidiqi.icu

[U04] Py：变量调试打印
来源：http://rvt.52xcode.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ewo.yj20258.top

[U05] Py：列表去重且保序
来源：http://dbr.fengsongda.top

list(dict.fromkeys(arr))
来源：http://xdn.hammf.cn

[U06] Py：合并两个字典
来源：http://nnp.ydzc1.top

{**a, **b}
来源：http://pul.yueranfly.top

[U07] Py：反转字典键值
来源：http://dgy.jlsjyb.cn

{v: k for k, v in d.items()}
来源：http://rqw.zdbjq.cn

[U08] Py：展平二维列表
来源：http://wzi.fktsv.cn

[y for x in nested for y in x]
来源：http://cwj.aizwys.cn

[U09] Py：字典取最大值的键
来源：http://nfw.ehwqpu.com

max(d, key=d.get)
来源：http://axb.gaohongyu789.top

[U10] Py：按值排序字典
来源：http://luf.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cut.yuanzhike.top

[U11] Py：生成器表达式
来源：http://yjv.daxiang520.top

(x * 2 for x in arr)
来源：http://fpz.xinyue.icu

[U12] Py：取出现最多的 3 个元素
来源：http://kwo.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://fxe.zhaomingkeji.xyz

[U13] Py：固定长度队列
来源：http://wxt.hysaishi.cn

deque(maxlen=10)
来源：http://lst.guannengcc.top

[U14] Py：分组收集到列表
来源：http://ili.fengsongda.top

defaultdict(list)
来源：http://yto.52xcode.cn

[U15] Py：高精度计时
来源：http://dpw.cucudq.cn

t = time.perf_counter()
来源：http://jur.guowangkeji.top

[U16] Py：命令行参数解析
来源：http://acs.dianchejie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jgo.epnwcf.com

[U17] Py：初始化日志
来源：http://ttv.cucudq.cn

logging.basicConfig(level=logging.INFO)
来源：http://tkl.zdbjq.cn

[U18] Py：预编译正则
来源：http://wuj.sweek.top

pat = re.compile(r"\d+")
来源：http://ofp.yj20258888.top

[U19] Py：正则替换带回调
来源：http://ryk.sysykeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fuc.haohaochexian.top

[U20] Py：缓存函数结果
来源：http://dxi.guannengcc.top

@functools.lru_cache(maxsize=None)
来源：http://sep.bjfxy.top

[U21] Py：自定义上下文管理器
来源：http://mhy.shuidangran.top

@contextlib.contextmanager
来源：http://ohg.havefunace.top

[U22] Py：矩阵转置
来源：http://igl.xingfuxueyuan.xyz

list(zip(*m))
来源：http://tug.quarkkingdee.top

[U23] Py：分块读取大文件
来源：http://ecy.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tsm.smart0.xyz

[U24] Py：路径操作
来源：http://xsh.shuidangran.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lip.jqgufenzy.top

[U25] Py：CSV 按字典读
来源：http://psr.andypj.xyz

csv.DictReader(f)
来源：http://sta.iojbl.cn

[U26] Py：并发下载
来源：http://ctd.ybcxt.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ldx.guannengcc.top

[U27] Py：异步 HTTP
来源：http://ztj.ehwqpu.com

aiohttp.ClientSession() 配合 async with
来源：http://agq.tianlin.xyz

[U28] Py：类型别名
来源：http://uoi.guannengcc.top

UserId = int
来源：http://gqz.fanxiaobao.xyz

[U29] Py：属性校验
来源：http://qfd.guowangkeji.top

@property 与 @x.setter 配合
来源：http://ctr.zhiwuduotai.top

[U30] Py：数据类
来源：http://ped.hnxiangtu.top

@dataclass(slots=True)
来源：http://ywm.hfpthk.cn

[U31] Py：单测
来源：http://cxh.yongpay.top

python -m pytest -q
来源：http://mpc.yangfankeji.com

[U32] Py：代码格式化
来源：http://emz.chenjidiqi.icu

ruff format . && ruff check --fix .
来源：http://dku.ehwqpu.com

[U33] Py：打包发布
来源：http://ybi.jinqigfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://fjj.zhoulong.xyz

[U34] Py：判断编码
来源：http://pwi.iojbl.cn

chardet.detect(raw)
来源：http://kzy.hongshengwenyu.top

[U35] Py：发送邮件
来源：http://bpa.hongshengwenyu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://saj.yangfankeji.com

[U36] Py：定时任务
来源：http://upy.pycfn.com

schedule.every(10).minutes.do(job)
来源：http://qpj.wangdashe.top

[U37] Py：读写 Excel
来源：http://xud.zhiwuduotai.top

pandas.read_excel / DataFrame.to_excel
来源：http://nkv.vqdsnc.cn

[U38] Py：获取脚本所在目录
来源：http://njn.snrcjt.cn

Path(__file__).resolve().parent
来源：http://pkk.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://myk.hywenlv.cn

sys.stdout.isatty()
来源：http://gye.zhijiandao.cn

[U40] Py：打印到标准错误
来源：http://egi.vqdsnc.cn

print("err", file=sys.stderr)
来源：http://isg.52xcode.cn

[U41] PHP：初始化 Composer 项目
来源：http://axy.xylfe.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cjm.pycfn.com

[U42] PHP：PSR-4 自动加载
来源：http://isk.gzhubu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://flf.hesvh.cn

[U43] PHP：声明命名空间
来源：http://jrk.xziqi.cn

namespace App\Http;
来源：http://sdm.cdnleiting.top

[U44] PHP：开启严格类型
来源：http://zot.zhijiandao.cn

declare(strict_types=1);
来源：http://rdu.pengpengdd.cyou

[U45] PHP：类型声明与返回类型
来源：http://qtn.zhongyouzk.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zfg.zhaomingkeji.xyz

[U46] PHP：可空类型
来源：http://ekr.quarkkingdee.top

?string $name = null
来源：http://plv.pycfn.com

[U47] PHP：联合类型
来源：http://xwm.wangshuangyany.cn

int|string $id
来源：http://osi.mhx1999.top

[U48] PHP：纯枚举
来源：http://vrk.cucudq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hxk.hnxiangtu.top

[U49] PHP：只读属性
来源：http://qcq.ydjk.org.cn

public readonly string $name
来源：http://xxg.shzxlz.cn

[U50] PHP：构造器属性提升
来源：http://mya.nwbrower.top

public function __construct(private int $id) {}
来源：http://zpf.wangshuangyany.cn

[U51] PHP：数组解构
来源：http://zea.fehbvm.com

[$a, $b] = $arr;
来源：http://doy.daria6918.cn

[U52] PHP：箭头函数
来源：http://nba.jqgfzy.top

$double = fn($x) => $x * 2;
来源：http://cyp.ywan-chungtsiang.top

[U53] PHP：空合并运算符
来源：http://zvp.ctjpmb.com

$v = $a ?? $b ?? "default";
来源：http://gab.sysykeji.top

[U54] PHP：空安全调用
来源：http://wot.dashuyun.cn

$obj?->method()
来源：http://uar.sjlbkw.cn

[U55] PHP：match 表达式
来源：http://ksu.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fug.zhaomingkeji.xyz

[U56] PHP：命名参数
来源：http://tpg.nanxinkj.top

f(a: 1, b: 2)
来源：http://cgg.zhengqikj.top

[U57] PHP：字符串插值
来源：http://xsx.guowangkeji.top

"值: {$a}"
来源：http://lbg.shanyushiyangtech.top

[U58] PHP：数组三件套
来源：http://lnx.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cej.jqgufenzy.top

[U59] PHP：自定义排序
来源：http://yft.yj202588.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ras.c1oappe.top

[U60] PHP：JSON 编解码
来源：http://ego.snrcjt.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://daz.daxiang520.top

[U61] PHP：正则
来源：http://apt.andypj.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xvc.xziqi.cn

[U62] PHP：日期对象
来源：http://guc.daxiang520.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wui.zycfv.cn

[U63] PHP：文件读写
来源：http://jbw.vqdsnc.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dcb.9152youxi.cn

[U64] PHP：目录遍历
来源：http://uiv.haohaochexian.top

glob("dir/*.php");  scandir("dir");
来源：http://kje.epnwcf.com

[U65] PHP：会话
来源：http://znq.jianghu66.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jce.52xcode.cn

[U66] PHP：设置 Cookie
来源：http://ojb.zdbjq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zhb.xylfe.cn

[U67] PHP：处理文件上传
来源：http://fvv.aibaodan.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ydc.haohaochexian.top

[U68] PHP：PDO 连接
来源：http://amj.fktsv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tyx.yongpay.top

[U69] PHP：PDO 预处理
来源：http://sld.quarkkingdee.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://epy.tianlin.xyz

[U70] PHP：PDO 事务
来源：http://hon.zhoulong.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://stq.shzxlz.cn

[U71] PHP：抛出异常
来源：http://fla.nanxinkj.top

throw new RuntimeException("失败", 500);
来源：http://vkc.jqgfzy.top

[U72] PHP：写错误日志
来源：http://ujf.andypj.xyz

error_log("失败: " . $e->getMessage());
来源：http://jgf.smart0.xyz

[U73] PHP：读取 ini 配置
来源：http://uuj.9152youxi.cn

parse_ini_file("config.ini", true)
来源：http://hue.jinyuanbaomall.cn

[U74] PHP：读取环境变量
来源：http://rdu.chenjidiqi.icu

getenv("APP_ENV") ?: "production"
来源：http://rhf.nanxinkj.top

[U75] PHP：依赖注入
来源：http://hpg.ctjpmb.com

composer require psr/container
来源：http://zax.jinqigfzy.top

[U76] PHP：简单路由
来源：http://woe.zycfv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zvi.zhixingplan.top

[U77] PHP：模板渲染
来源：http://xyx.ydzc1.top

composer require twig/twig
来源：http://bsa.nanxinkj.top

[U78] PHP：单元测试
来源：http://lyp.cheryme.top

composer require --dev phpunit/phpunit
来源：http://nql.fktsv.cn

[U79] PHP：静态分析
来源：http://hhl.svipenyu.cn

composer require --dev phpstan/phpstan
来源：http://ipg.uphjek.com

[U80] PHP：代码规范修复
来源：http://igl.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yhj.wangshuangyany.cn

[U81] JS：初始化项目
来源：http://lpc.nanxuanxn.top

npm init -y;  npm i express
来源：http://awy.guowangkeji.top

[U82] JS：package.json 脚本
来源：http://fzp.nanxuanxn.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ljs.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://gfp.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://jnl.zycfv.cn

[U84] JS：CommonJS 写法
来源：http://auc.ybcxt.top

module.exports = { a };  const { a } = require("./m");
来源：http://rou.gotoacloud.top

[U85] JS：可选链
来源：http://pvd.yj20258.top

a?.b?.c
来源：http://bro.c1oappe.top

[U86] JS：空值合并
来源：http://ngy.316326.xyz

a ?? b
来源：http://mge.yongpay.top

[U87] JS：解构默认值
来源：http://qbp.bbcook.cn

const { a = 1, b = 2 } = obj;
来源：http://guw.dianchejie.cn

[U88] JS：对象展开合并
来源：http://rfm.c1oappe.top

{ ...a, ...b }
来源：http://mwh.zhixingplan.top

[U89] JS：数组去重
来源：http://gje.svipenyu.cn

[...new Set(arr)]
来源：http://vdj.vqdsnc.cn

[U90] JS：数字数组排序
来源：http://lir.yonumen.top

[...arr].sort((a, b) => a - b)
来源：http://vwk.chenzaomai.com

[U91] JS：对象键值遍历
来源：http://dgp.sysykeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yry.haohaochexian.top

[U92] JS：深拷贝
来源：http://wdy.nanxinkj.top

structuredClone(obj)
来源：http://ltj.yfazqb.com

[U93] JS：模板字符串
来源：http://rba.fanxiaobao.xyz

`共 ${n} 条`
来源：http://yca.zhiwuduotai.top

[U94] JS：箭头函数
来源：http://rgo.hfpthk.cn

const double = x => x * 2;
来源：http://msm.yvedp.cn

[U95] JS：Promise 包装
来源：http://mkj.shzxlz.cn

new Promise((resolve, reject) => {})
来源：http://aeq.cdnleiting.top

[U96] JS：async/await 与异常
来源：http://owq.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nsi.ppjwa.cn

[U97] JS：并发请求
来源：http://jem.cucudq.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://grq.hesvh.cn

[U98] JS：fetch 带 JSON
来源：http://vas.chenjidiqi.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://crd.pengpengdd.cyou

[U99] JS：事件监听
来源：http://pdi.zdbjq.cn

el.addEventListener("click", e => {})
来源：http://kbx.kuanghao11.cn

[U100] JS：DOM 查询
来源：http://rhx.jinyuanbaomall.cn

document.querySelector(".item")
来源：http://fko.shanyushiyangkeji.top

[U101] JS：classList 操作
来源：http://tiq.sxryk.cn

el.classList.toggle("active")
来源：http://fha.zhixingplan.top

[U102] JS：本地存储
来源：http://fnw.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://csx.dianchejie.cn

[U103] JS：定时器
来源：http://fnm.sweek.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ind.sysykeji.top

[U104] JS：防抖
来源：http://jmg.9152youxi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ifn.ppjwa.cn

[U105] JS：节流
来源：http://lkn.0kj1m.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bfi.pycfn.com

[U106] JS：日期格式化
来源：http://cnl.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fcr.nwbrower.top

[U107] JS：数字千分位
来源：http://vfz.daria6918.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ouj.jqgfzy.top

[U108] JS：随机整数
来源：http://vfk.daria6918.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pos.iojbl.cn

[U109] JS：数组分组
来源：http://fgl.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://eys.yj202588.top

[U110] JS：数组分块
来源：http://sie.yj20258.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wrb.smart0.xyz

[U111] JS：对象转 Map
来源：http://fho.ivvv.top

new Map(Object.entries(obj))
来源：http://jwq.yueranfly.top

[U112] JS：字符串补位
来源：http://ovj.cashguo.top

"7".padStart(3, "0")
来源：http://afi.sufxvd.cn

[U113] JS：正则替换全部
来源：http://cnh.yonumen.top

s.replaceAll("a", "b")
来源：http://ykv.zdqjudy.top

[U114] JS：JSON 深比较
来源：http://fhl.tianlin.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://kvs.chenlongwang.top

[U115] JS：生成 UUID
来源：http://ext.jinyuanbaomall.cn

crypto.randomUUID()
来源：http://uht.zhiwuduotai.top

[U116] JS：类型检查（JSDoc）
来源：http://jtr.ctjpmb.com

/** @param {string} name */ function f(name) {}
来源：http://rji.dashuyun.cn


<!-- 参考信息 -->