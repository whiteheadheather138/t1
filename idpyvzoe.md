代发 wailian999

[T31] Lua：Hello World
来源：http://zma.52xcode.cn

print("Hello")
来源：http://sbd.fengsongda.top

[T32] Lua：局部变量
来源：http://kje.zhiwuduotai.top

local a = 1
来源：http://awu.guowangkeji.top

[T33] Lua：表（数组）
来源：http://fjs.ivvv.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hfo.sjlbkw.cn

[T34] Lua：遍历表
来源：http://sfx.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://pzk.redwolf501.top

[T35] Lua：字典表
来源：http://nur.zdqjudy.top

local d = { a = 1 };  d.b = 2
来源：http://tmc.redwolf501.top

[T36] Lua：函数
来源：http://kcf.ybcxt.top

function add(a, b) return a + b end
来源：http://zmw.zdbjq.cn

[T37] Lua：字符串拼接
来源：http://ybr.zycfv.cn

"a" .. "b"
来源：http://unn.hcnkem.com

[T38] Lua：条件
来源：http://slv.hnqzz.top

if x > 0 then print("正") end
来源：http://osf.guannengcc.top

[T39] Lua：模式匹配
来源：http://jrn.gotoacloud.top

string.find(s, "%d+")
来源：http://nqc.tanke756.top

[T40] Lua：元表
来源：http://uwx.hnxiangtu.top

setmetatable({}, { __index = base })
来源：http://gcv.zhiwuduotai.top

[T41] Perl：Hello World
来源：http://jvu.zhoulong.xyz

print "Hello\n";
来源：http://njq.uphjek.com

[T42] Perl：变量类型
来源：http://mss.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lbo.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://hai.hysaishi.cn

"值: $a"
来源：http://onv.shanyushiyangtech.top

[T44] Perl：条件
来源：http://jmw.chenlongwang.top

if ($a > 0) { print "正"; }
来源：http://rsp.ppjwa.cn

[T45] Perl：数组遍历
来源：http://hmy.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://raz.ybcxt.top

[T46] Perl：哈希操作
来源：http://yyg.gotoacloud.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gmm.c1oappe.top

[T47] Perl：正则捕获
来源：http://ekh.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://pyo.bjfxy.top

[T48] Perl：正则替换
来源：http://icc.sxryk.cn

$s =~ s/old/new/g;
来源：http://izc.feifeiyinyue.top

[T49] Perl：函数
来源：http://ufo.uphjek.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tnu.ivvv.top

[T50] Perl：逐行读文件
来源：http://isp.xuetiantiany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kro.xinyue.icu

while (my $line = <$fh>) { print $line; }
来源：http://dao.cqqwz.cn

[T51] Scala：Hello World
来源：http://nft.daria6918.cn

println("Hello")
来源：http://yna.0kj1m.cn

[T52] Scala：变量
来源：http://eog.jlsjyb.cn

val a = 1;  var b = 2
来源：http://zfo.hesvh.cn

[T53] Scala：字符串插值
来源：http://fyt.vehdjk.com

s"值: $b"
来源：http://wkz.wangdashe.top

[T54] Scala：集合映射
来源：http://xrz.kuanghao11.cn

List(1, 2, 3).map(_ * 2)
来源：http://ivs.zdbjq.cn

[T55] Scala：集合过滤
来源：http://vnr.wangdashe.top

List(1, 2, 3).filter(_ > 1)
来源：http://goo.tianlin.xyz

[T56] Scala：样例类
来源：http://vuo.xingfuxueyuan.xyz

case class User(name: String, age: Int)
来源：http://iug.xziqi.cn

[T57] Scala：模式匹配
来源：http://cjg.daria6918.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qom.yuxming.cn

[T58] Scala：函数定义
来源：http://hif.fzhhl.top

def add(a: Int, b: Int): Int = a + b
来源：http://dgn.nanxuanxn.top

[T59] Scala：循环
来源：http://fyn.cucudq.cn

for (i <- 1 to 10) println(i)
来源：http://mhr.ehwqpu.com

[T60] Scala：折叠
来源：http://zhw.gogol.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iuu.nwbrower.top

================================================================================
来源：http://rsw.hnqzz.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ung.jianghu66.top

================================================================================
来源：http://zyh.meibo888.top

[U01] Py：创建虚拟环境
来源：http://nes.shzxlz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vru.zycfv.cn

[U02] Py：导出 / 安装依赖
来源：http://bze.cqqwz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qia.316326.xyz

[U03] Py：加载 .env 配置
来源：http://zfp.shangyingyoupin.top

from dotenv import load_dotenv; load_dotenv()
来源：http://weh.ppjwa.cn

[U04] Py：变量调试打印
来源：http://cai.jinqigfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fzh.jyoumei.cn

[U05] Py：列表去重且保序
来源：http://pag.yuxming.cn

list(dict.fromkeys(arr))
来源：http://fdz.hongshengwenyu.top

[U06] Py：合并两个字典
来源：http://zpv.zhongyouzk.top

{**a, **b}
来源：http://kia.yj20258.top

[U07] Py：反转字典键值
来源：http://bhn.wangshuangyany.cn

{v: k for k, v in d.items()}
来源：http://nww.nanxinkj.top

[U08] Py：展平二维列表
来源：http://dcw.vehdjk.com

[y for x in nested for y in x]
来源：http://ayf.yueranfly.top

[U09] Py：字典取最大值的键
来源：http://dld.chenlongwang.top

max(d, key=d.get)
来源：http://ljp.cqqwz.cn

[U10] Py：按值排序字典
来源：http://vqv.sxryk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ftc.hcnkem.com

[U11] Py：生成器表达式
来源：http://nrv.bjfxy.top

(x * 2 for x in arr)
来源：http://dan.snrcjt.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uuo.9152youxi.cn

Counter(arr).most_common(3)
来源：http://tds.ydjk.org.cn

[U13] Py：固定长度队列
来源：http://qnq.shanyushiyangtech.top

deque(maxlen=10)
来源：http://jvq.mhx1999.top

[U14] Py：分组收集到列表
来源：http://kzm.jqgfzy.top

defaultdict(list)
来源：http://gmu.sjlbkw.cn

[U15] Py：高精度计时
来源：http://drd.wangshuangyany.cn

t = time.perf_counter()
来源：http://cjz.ybcxt.top

[U16] Py：命令行参数解析
来源：http://hjm.sxryk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zyp.jinghuilouyu.cn

[U17] Py：初始化日志
来源：http://oqz.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://qdu.cashguo.top

[U18] Py：预编译正则
来源：http://edd.zdqjudy.top

pat = re.compile(r"\d+")
来源：http://jgh.epnwcf.com

[U19] Py：正则替换带回调
来源：http://xsm.zhengqikj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zfh.xinyue.icu

[U20] Py：缓存函数结果
来源：http://bvd.shzxlz.cn

@functools.lru_cache(maxsize=None)
来源：http://vhm.0kj1m.cn

[U21] Py：自定义上下文管理器
来源：http://cro.havefunace.top

@contextlib.contextmanager
来源：http://ssg.hammf.cn

[U22] Py：矩阵转置
来源：http://ikd.zhongyouzk.top

list(zip(*m))
来源：http://dmv.xuanzx.com

[U23] Py：分块读取大文件
来源：http://nxy.andypj.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iyb.cdnleiting.top

[U24] Py：路径操作
来源：http://ppc.xuetiantiany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mvq.gaohongyu789.top

[U25] Py：CSV 按字典读
来源：http://wog.fengsongda.top

csv.DictReader(f)
来源：http://vjv.zdbjq.cn

[U26] Py：并发下载
来源：http://baa.jinqigfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://toh.tianlin.xyz

[U27] Py：异步 HTTP
来源：http://qwl.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://omi.nanxuanxn.top

[U28] Py：类型别名
来源：http://ezy.aizwys.cn

UserId = int
来源：http://ddn.zhixingplan.top

[U29] Py：属性校验
来源：http://wwg.cheryme.top

@property 与 @x.setter 配合
来源：http://iwb.bbcook.cn

[U30] Py：数据类
来源：http://rvi.zhengqikj.top

@dataclass(slots=True)
来源：http://bor.yangfankeji.com

[U31] Py：单测
来源：http://ntc.bbcook.cn

python -m pytest -q
来源：http://hou.vehdjk.com

[U32] Py：代码格式化
来源：http://oej.fehbvm.com

ruff format . && ruff check --fix .
来源：http://lfg.nanxinkj.top

[U33] Py：打包发布
来源：http://sbz.mhx1999.top

python -m build  （依赖 pyproject.toml）
来源：http://cwy.birdmap.top

[U34] Py：判断编码
来源：http://qyx.dianchejie.cn

chardet.detect(raw)
来源：http://cml.gzhubu.top

[U35] Py：发送邮件
来源：http://ovw.0kj1m.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bzl.fengsongda.top

[U36] Py：定时任务
来源：http://mbk.redwolf501.top

schedule.every(10).minutes.do(job)
来源：http://mxr.fzhhl.top

[U37] Py：读写 Excel
来源：http://xwb.snrcjt.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yxc.nwbrower.top

[U38] Py：获取脚本所在目录
来源：http://zig.yanxiufei.cn

Path(__file__).resolve().parent
来源：http://drb.wangshuangyany.cn

[U39] Py：判断是否在交互环境
来源：http://gvr.snrcjt.cn

sys.stdout.isatty()
来源：http://htg.iojbl.cn

[U40] Py：打印到标准错误
来源：http://ewq.jlsjyb.cn

print("err", file=sys.stderr)
来源：http://vtk.guowangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://qhn.ywan-chungtsiang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rgt.yvedp.cn

[U42] PHP：PSR-4 自动加载
来源：http://rmo.fzhhl.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ymo.ywan-chungtsiang.top

[U43] PHP：声明命名空间
来源：http://pcx.yvedp.cn

namespace App\Http;
来源：http://ltc.hnqzz.top

[U44] PHP：开启严格类型
来源：http://qxc.cucudq.cn

declare(strict_types=1);
来源：http://zpo.zdbjq.cn

[U45] PHP：类型声明与返回类型
来源：http://drj.aibaodan.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://trk.svipenyu.cn

[U46] PHP：可空类型
来源：http://rdp.sysykeji.top

?string $name = null
来源：http://psk.guannengcc.top

[U47] PHP：联合类型
来源：http://wte.jqgufenzy.top

int|string $id
来源：http://qow.aibaodan.cn

[U48] PHP：纯枚举
来源：http://urv.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://stm.havefunace.top

[U49] PHP：只读属性
来源：http://wpb.yuanzhike.top

public readonly string $name
来源：http://qcq.meibo888.top

[U50] PHP：构造器属性提升
来源：http://sls.yueranfly.top

public function __construct(private int $id) {}
来源：http://uuy.xylfe.cn

[U51] PHP：数组解构
来源：http://eal.redwolf501.top

[$a, $b] = $arr;
来源：http://lsk.hysaishi.cn

[U52] PHP：箭头函数
来源：http://kfq.jianghu66.top

$double = fn($x) => $x * 2;
来源：http://rdb.ywan-chungtsiang.top

[U53] PHP：空合并运算符
来源：http://qcp.fzhhl.top

$v = $a ?? $b ?? "default";
来源：http://dxo.9152youxi.cn

[U54] PHP：空安全调用
来源：http://dsi.aibaodan.cn

$obj?->method()
来源：http://ypo.fanxiaobao.xyz

[U55] PHP：match 表达式
来源：http://cpv.dashuyun.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qyq.hammf.cn

[U56] PHP：命名参数
来源：http://qxy.zhengqikj.top

f(a: 1, b: 2)
来源：http://ssu.ivvv.top

[U57] PHP：字符串插值
来源：http://bpw.dashuyun.cn

"值: {$a}"
来源：http://onk.tarul.cn

[U58] PHP：数组三件套
来源：http://mcu.yonumen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uap.sweek.top

[U59] PHP：自定义排序
来源：http://sch.hnxiangtu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://axy.birdmap.top

[U60] PHP：JSON 编解码
来源：http://wwm.zhengqikj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ruc.daria6918.cn

[U61] PHP：正则
来源：http://riv.yangfankeji.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ado.cashguo.top

[U62] PHP：日期对象
来源：http://lbk.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://map.shuidangran.top

[U63] PHP：文件读写
来源：http://cwp.yj202588.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jbk.jlsjyb.cn

[U64] PHP：目录遍历
来源：http://cxn.tanke756.top

glob("dir/*.php");  scandir("dir");
来源：http://kih.andypj.xyz

[U65] PHP：会话
来源：http://cur.sxryk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ajp.sweek.top

[U66] PHP：设置 Cookie
来源：http://foc.hysaishi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zvl.uphjek.com

[U67] PHP：处理文件上传
来源：http://lei.yvedp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bgj.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://rsz.ivvv.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cnk.wangdashe.top

[U69] PHP：PDO 预处理
来源：http://amd.chenlongwang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qgb.yj20258888.top

[U70] PHP：PDO 事务
来源：http://bwv.tanke756.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nkq.jinqigfzy.top

[U71] PHP：抛出异常
来源：http://xmq.c1oappe.top

throw new RuntimeException("失败", 500);
来源：http://hfl.jyoumei.cn

[U72] PHP：写错误日志
来源：http://wjq.zhaomingkeji.xyz

error_log("失败: " . $e->getMessage());
来源：http://yiz.yj202588.top

[U73] PHP：读取 ini 配置
来源：http://qrc.jiagoushi.top

parse_ini_file("config.ini", true)
来源：http://rpq.yj202588.top

[U74] PHP：读取环境变量
来源：http://mpt.zhaomingkeji.xyz

getenv("APP_ENV") ?: "production"
来源：http://mtc.jinqigfzy.top

[U75] PHP：依赖注入
来源：http://bjh.xziqi.cn

composer require psr/container
来源：http://auh.cucudq.cn

[U76] PHP：简单路由
来源：http://qjd.jlsjyb.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://isv.ehwqpu.com

[U77] PHP：模板渲染
来源：http://ukp.mhx1999.top

composer require twig/twig
来源：http://gjn.quarkkingdee.top

[U78] PHP：单元测试
来源：http://tdc.daxiang520.top

composer require --dev phpunit/phpunit
来源：http://nra.iojbl.cn

[U79] PHP：静态分析
来源：http://gnh.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://daz.nanxinkj.top

[U80] PHP：代码规范修复
来源：http://nqm.daria6918.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jqm.yj20258888.top

[U81] JS：初始化项目
来源：http://lvy.aizwys.cn

npm init -y;  npm i express
来源：http://ifp.vqdsnc.cn

[U82] JS：package.json 脚本
来源：http://gze.jiagoushi.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mpx.zhengqikj.top

[U83] JS：ES Module 导入导出
来源：http://jir.snrcjt.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bao.hongshengwenyu.top

[U84] JS：CommonJS 写法
来源：http://gyb.yongpay.top

module.exports = { a };  const { a } = require("./m");
来源：http://nby.gaohongyu789.top

[U85] JS：可选链
来源：http://flt.jlsjyb.cn

a?.b?.c
来源：http://kvc.pycfn.com

[U86] JS：空值合并
来源：http://itc.9152youxi.cn

a ?? b
来源：http://vnj.gotoacloud.top

[U87] JS：解构默认值
来源：http://ibg.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://ogl.epnwcf.com

[U88] JS：对象展开合并
来源：http://lvc.hammf.cn

{ ...a, ...b }
来源：http://ppi.52xcode.cn

[U89] JS：数组去重
来源：http://ity.vqdsnc.cn

[...new Set(arr)]
来源：http://pay.gaohongyu789.top

[U90] JS：数字数组排序
来源：http://smw.yueranfly.top

[...arr].sort((a, b) => a - b)
来源：http://ctu.tanke756.top

[U91] JS：对象键值遍历
来源：http://esz.shuidangran.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://guu.zhongyouzk.top

[U92] JS：深拷贝
来源：http://jiw.hnxiangtu.top

structuredClone(obj)
来源：http://qmj.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://olk.birdmap.top

`共 ${n} 条`
来源：http://sxp.hongshengwenyu.top

[U94] JS：箭头函数
来源：http://gnd.hywenlv.cn

const double = x => x * 2;
来源：http://ogn.fanxiaobao.xyz

[U95] JS：Promise 包装
来源：http://kly.zhengqikj.top

new Promise((resolve, reject) => {})
来源：http://jyx.yvedp.cn

[U96] JS：async/await 与异常
来源：http://zbz.zdbjq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jbh.yuxming.cn

[U97] JS：并发请求
来源：http://myu.xinyue.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://goc.pengpengdd.cyou

[U98] JS：fetch 带 JSON
来源：http://lhu.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eej.ppjwa.cn

[U99] JS：事件监听
来源：http://vhj.sufxvd.cn

el.addEventListener("click", e => {})
来源：http://pox.cdnleiting.top

[U100] JS：DOM 查询
来源：http://ylu.yuxming.cn

document.querySelector(".item")
来源：http://hqv.ydzc1.top

[U101] JS：classList 操作
来源：http://pmx.jqgufenzy.top

el.classList.toggle("active")
来源：http://zwt.shuidangran.top

[U102] JS：本地存储
来源：http://qrp.daria6918.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cns.ctjpmb.com

[U103] JS：定时器
来源：http://nsn.hywenlv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mpf.jlsjyb.cn

[U104] JS：防抖
来源：http://yqj.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lmm.hongshengwenyu.top

[U105] JS：节流
来源：http://ziq.shuidangran.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://skk.shuidangran.top

[U106] JS：日期格式化
来源：http://wmt.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xja.nanxuanxn.top

[U107] JS：数字千分位
来源：http://srv.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gyv.fehbvm.com

[U108] JS：随机整数
来源：http://ayi.fehbvm.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fzb.gogol.net.cn

[U109] JS：数组分组
来源：http://qzx.yuxming.cn

Object.groupBy(arr, x => x.type)
来源：http://lpd.hfpthk.cn

[U110] JS：数组分块
来源：http://ogk.guannengcc.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bfp.jyoumei.cn

[U111] JS：对象转 Map
来源：http://noi.hnqzz.top

new Map(Object.entries(obj))
来源：http://dnj.dianchejie.cn

[U112] JS：字符串补位
来源：http://ezw.hnqzz.top

"7".padStart(3, "0")
来源：http://ccm.ppjwa.cn

[U113] JS：正则替换全部
来源：http://bld.guowangkeji.top

s.replaceAll("a", "b")
来源：http://bdr.shanyushiyangtech.top

[U114] JS：JSON 深比较
来源：http://mpa.jiagoushi.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vry.smart0.xyz

[U115] JS：生成 UUID
来源：http://qri.hesvh.cn

crypto.randomUUID()
来源：http://yby.xuetiantiany.cn

[U116] JS：类型检查（JSDoc）
来源：http://feh.zhixingplan.top

/** @param {string} name */ function f(name) {}
来源：http://mrq.smart0.xyz

[U117] JS：单元测试
来源：http://rfj.tian-w.cn

npm i -D vitest;  npx vitest
来源：http://jyq.jqgufenzy.top

[U118] JS：开发服务器
来源：http://fva.tarul.cn

npm i -D vite;  npx vite
来源：http://nsr.jyoumei.cn


<!-- 参考信息 -->