代发 wailian999

[T33] Lua：表（数组）
来源：http://xmy.jyoumei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lqf.yongpay.top

[T34] Lua：遍历表
来源：http://rph.cucudq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fbw.chenlongwang.top

[T35] Lua：字典表
来源：http://qqt.bbcook.cn

local d = { a = 1 };  d.b = 2
来源：http://euf.cqqwz.cn

[T36] Lua：函数
来源：http://zuq.52xcode.cn

function add(a, b) return a + b end
来源：http://hwb.chenjidiqi.icu

[T37] Lua：字符串拼接
来源：http://afj.xinyue.icu

"a" .. "b"
来源：http://tld.wangshuangyany.cn

[T38] Lua：条件
来源：http://jur.zhijiandao.cn

if x > 0 then print("正") end
来源：http://fqw.yuanzhike.top

[T39] Lua：模式匹配
来源：http://hlj.aibaodan.cn

string.find(s, "%d+")
来源：http://xkh.gotoacloud.top

[T40] Lua：元表
来源：http://grr.shanyushiyangkeji.top

setmetatable({}, { __index = base })
来源：http://zlo.epnwcf.com

[T41] Perl：Hello World
来源：http://tit.redwolf501.top

print "Hello\n";
来源：http://eju.cucudq.cn

[T42] Perl：变量类型
来源：http://fzc.gotoacloud.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vyx.chenjidiqi.icu

[T43] Perl：字符串插值
来源：http://jvv.yueranfly.top

"值: $a"
来源：http://alo.tianlin.xyz

[T44] Perl：条件
来源：http://dux.shanyushiyangkeji.top

if ($a > 0) { print "正"; }
来源：http://znf.redwolf501.top

[T45] Perl：数组遍历
来源：http://gdb.jinqigfzy.top

for my $x (@arr) { print $x; }
来源：http://akm.xuetiantiany.cn

[T46] Perl：哈希操作
来源：http://vko.sjlbkw.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ylb.jqgfzy.top

[T47] Perl：正则捕获
来源：http://uzv.xingfuxueyuan.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://rdl.pycfn.com

[T48] Perl：正则替换
来源：http://spo.yj202588.top

$s =~ s/old/new/g;
来源：http://mdo.zhijiandao.cn

[T49] Perl：函数
来源：http://ptr.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qor.fzhhl.top

[T50] Perl：逐行读文件
来源：http://fev.ctjpmb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://wcy.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://zzi.daxiang520.top

[T51] Scala：Hello World
来源：http://vjv.jinqigfzy.top

println("Hello")
来源：http://vdu.smart0.xyz

[T52] Scala：变量
来源：http://zcm.daxiang520.top

val a = 1;  var b = 2
来源：http://sda.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://qey.mhx1999.top

s"值: $b"
来源：http://aav.sweek.top

[T54] Scala：集合映射
来源：http://knw.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://kra.yvedp.cn

[T55] Scala：集合过滤
来源：http://jmf.zhengqikj.top

List(1, 2, 3).filter(_ > 1)
来源：http://agf.xingfuxueyuan.xyz

[T56] Scala：样例类
来源：http://yii.yj202588.top

case class User(name: String, age: Int)
来源：http://clm.jinyuanbaomall.cn

[T57] Scala：模式匹配
来源：http://uei.yongpay.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://blk.daxiang520.top

[T58] Scala：函数定义
来源：http://yuf.jlsjyb.cn

def add(a: Int, b: Int): Int = a + b
来源：http://iaq.jinyuanbaomall.cn

[T59] Scala：循环
来源：http://vub.cqqwz.cn

for (i <- 1 to 10) println(i)
来源：http://jvo.chenlongwang.top

[T60] Scala：折叠
来源：http://iab.gotoacloud.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gtp.fktsv.cn

================================================================================
来源：http://mot.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oaq.kuanghao11.cn

================================================================================
来源：http://ipp.xylfe.cn

[U01] Py：创建虚拟环境
来源：http://wml.yj202588.top

python -m venv .venv && source .venv/bin/activate
来源：http://cti.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://lpj.daria6918.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://apr.bbcook.cn

[U03] Py：加载 .env 配置
来源：http://ydz.redwolf501.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lun.hnxiangtu.top

[U04] Py：变量调试打印
来源：http://acd.chenjidiqi.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cpw.shanyushiyangkeji.top

[U05] Py：列表去重且保序
来源：http://blg.cheryme.top

list(dict.fromkeys(arr))
来源：http://aed.hongshengwenyu.top

[U06] Py：合并两个字典
来源：http://crk.meibo888.top

{**a, **b}
来源：http://cla.ctjpmb.com

[U07] Py：反转字典键值
来源：http://zhx.shangyingyoupin.top

{v: k for k, v in d.items()}
来源：http://qbr.aibaodan.cn

[U08] Py：展平二维列表
来源：http://kux.yuxming.cn

[y for x in nested for y in x]
来源：http://wjl.yangfankeji.com

[U09] Py：字典取最大值的键
来源：http://kwl.cheryme.top

max(d, key=d.get)
来源：http://snh.ybcxt.top

[U10] Py：按值排序字典
来源：http://yoh.jinyuanbaomall.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hix.zhixingplan.top

[U11] Py：生成器表达式
来源：http://cps.vehdjk.com

(x * 2 for x in arr)
来源：http://oyq.zhijiandao.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vsn.jinqigufen.top

Counter(arr).most_common(3)
来源：http://owm.hnqzz.top

[U13] Py：固定长度队列
来源：http://zfc.havefunace.top

deque(maxlen=10)
来源：http://rom.daria6918.cn

[U14] Py：分组收集到列表
来源：http://foe.hongshengwenyu.top

defaultdict(list)
来源：http://rru.feifeiyinyue.top

[U15] Py：高精度计时
来源：http://bem.ydjk.org.cn

t = time.perf_counter()
来源：http://siu.vehdjk.com

[U16] Py：命令行参数解析
来源：http://hgw.hcnkem.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rvz.316326.xyz

[U17] Py：初始化日志
来源：http://gex.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://eay.sweek.top

[U18] Py：预编译正则
来源：http://dcv.yj202588.top

pat = re.compile(r"\d+")
来源：http://kkd.birdmap.top

[U19] Py：正则替换带回调
来源：http://qus.uphjek.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iaf.shanyushiyangtech.top

[U20] Py：缓存函数结果
来源：http://xjl.aibaodan.cn

@functools.lru_cache(maxsize=None)
来源：http://yfe.pycfn.com

[U21] Py：自定义上下文管理器
来源：http://sag.wangshuangyany.cn

@contextlib.contextmanager
来源：http://tqv.cucudq.cn

[U22] Py：矩阵转置
来源：http://fwn.yvedp.cn

list(zip(*m))
来源：http://uyr.chenlongwang.top

[U23] Py：分块读取大文件
来源：http://yls.xuanzx.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ohu.bjfxy.top

[U24] Py：路径操作
来源：http://mbc.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tnn.hongshengwenyu.top

[U25] Py：CSV 按字典读
来源：http://xgy.xziqi.cn

csv.DictReader(f)
来源：http://aqe.xziqi.cn

[U26] Py：并发下载
来源：http://ktb.nanxinkj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bii.dashuyun.cn

[U27] Py：异步 HTTP
来源：http://mwg.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://hkm.guannengcc.top

[U28] Py：类型别名
来源：http://sfo.fengsongda.top

UserId = int
来源：http://nie.cqqwz.cn

[U29] Py：属性校验
来源：http://bcd.snrcjt.cn

@property 与 @x.setter 配合
来源：http://dbh.mhx1999.top

[U30] Py：数据类
来源：http://afe.tanke756.top

@dataclass(slots=True)
来源：http://hco.zhengqikj.top

[U31] Py：单测
来源：http://mjl.redwolf501.top

python -m pytest -q
来源：http://jnn.hysaishi.cn

[U32] Py：代码格式化
来源：http://ugi.yvedp.cn

ruff format . && ruff check --fix .
来源：http://bof.hammf.cn

[U33] Py：打包发布
来源：http://nbs.yonumen.top

python -m build  （依赖 pyproject.toml）
来源：http://dyp.jqgufenzy.top

[U34] Py：判断编码
来源：http://vbu.xuetiantiany.cn

chardet.detect(raw)
来源：http://oxj.sufxvd.cn

[U35] Py：发送邮件
来源：http://kgv.tian-w.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qgs.fanxiaobao.xyz

[U36] Py：定时任务
来源：http://sfm.gogol.net.cn

schedule.every(10).minutes.do(job)
来源：http://sye.tian-w.cn

[U37] Py：读写 Excel
来源：http://hqz.ehwqpu.com

pandas.read_excel / DataFrame.to_excel
来源：http://sjw.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://tiy.jinqigfzy.top

Path(__file__).resolve().parent
来源：http://ais.xziqi.cn

[U39] Py：判断是否在交互环境
来源：http://jfv.ydjk.org.cn

sys.stdout.isatty()
来源：http://uaf.xinyue.icu

[U40] Py：打印到标准错误
来源：http://rqs.c1oappe.top

print("err", file=sys.stderr)
来源：http://soj.feifeiyinyue.top

[U41] PHP：初始化 Composer 项目
来源：http://aiu.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dua.ybcxt.top

[U42] PHP：PSR-4 自动加载
来源：http://yzv.gaohongyu789.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://opr.guowangkeji.top

[U43] PHP：声明命名空间
来源：http://rnd.mhx1999.top

namespace App\Http;
来源：http://ncm.nanxinkj.top

[U44] PHP：开启严格类型
来源：http://wan.jianghu66.top

declare(strict_types=1);
来源：http://xnt.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://sly.nwbrower.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ecg.iojbl.cn

[U46] PHP：可空类型
来源：http://yhx.52xcode.cn

?string $name = null
来源：http://jan.zycfv.cn

[U47] PHP：联合类型
来源：http://nir.zhijiandao.cn

int|string $id
来源：http://ddy.nwbrower.top

[U48] PHP：纯枚举
来源：http://fsn.0kj1m.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zqh.snrcjt.cn

[U49] PHP：只读属性
来源：http://ary.birdmap.top

public readonly string $name
来源：http://gmo.cucudq.cn

[U50] PHP：构造器属性提升
来源：http://jnr.hnxiangtu.top

public function __construct(private int $id) {}
来源：http://yev.vqdsnc.cn

[U51] PHP：数组解构
来源：http://bue.svipenyu.cn

[$a, $b] = $arr;
来源：http://avx.ppjwa.cn

[U52] PHP：箭头函数
来源：http://lqx.vehdjk.com

$double = fn($x) => $x * 2;
来源：http://yaf.cheryme.top

[U53] PHP：空合并运算符
来源：http://fyv.pycfn.com

$v = $a ?? $b ?? "default";
来源：http://ohe.gzhubu.top

[U54] PHP：空安全调用
来源：http://gea.daxiang520.top

$obj?->method()
来源：http://aoq.hfpthk.cn

[U55] PHP：match 表达式
来源：http://hwf.zhaomingkeji.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wym.yonumen.top

[U56] PHP：命名参数
来源：http://luh.hesvh.cn

f(a: 1, b: 2)
来源：http://mvb.dashuyun.cn

[U57] PHP：字符串插值
来源：http://wfa.pengpengdd.cyou

"值: {$a}"
来源：http://keo.zdqjudy.top

[U58] PHP：数组三件套
来源：http://fea.jiagoushi.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iae.yonumen.top

[U59] PHP：自定义排序
来源：http://rtn.haohaochexian.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ggz.gaohongyu789.top

[U60] PHP：JSON 编解码
来源：http://eer.feifeiyinyue.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pgj.snrcjt.cn

[U61] PHP：正则
来源：http://brb.jyoumei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yik.redwolf501.top

[U62] PHP：日期对象
来源：http://krf.uphjek.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qsq.yonumen.top

[U63] PHP：文件读写
来源：http://rao.nanxinkj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://shd.chenjidiqi.icu

[U64] PHP：目录遍历
来源：http://tdq.vehdjk.com

glob("dir/*.php");  scandir("dir");
来源：http://mtw.kuanghao11.cn

[U65] PHP：会话
来源：http://bkh.jyoumei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://efg.yuxming.cn

[U66] PHP：设置 Cookie
来源：http://kim.vehdjk.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wur.fanxiaobao.xyz

[U67] PHP：处理文件上传
来源：http://ora.havefunace.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jzg.daxiang520.top

[U68] PHP：PDO 连接
来源：http://zif.xingfuxueyuan.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zsd.jyoumei.cn

[U69] PHP：PDO 预处理
来源：http://esg.zhengqikj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cqx.feifeiyinyue.top

[U70] PHP：PDO 事务
来源：http://mty.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eaa.yj20258888.top

[U71] PHP：抛出异常
来源：http://ziw.gaohongyu789.top

throw new RuntimeException("失败", 500);
来源：http://sxd.chenjidiqi.icu

[U72] PHP：写错误日志
来源：http://ldv.fengsongda.top

error_log("失败: " . $e->getMessage());
来源：http://wti.yj20258888.top

[U73] PHP：读取 ini 配置
来源：http://tdk.epnwcf.com

parse_ini_file("config.ini", true)
来源：http://hdg.cqqwz.cn

[U74] PHP：读取环境变量
来源：http://ztz.wangshuangyany.cn

getenv("APP_ENV") ?: "production"
来源：http://miw.zhengqikj.top

[U75] PHP：依赖注入
来源：http://jia.shanyushiyangtech.top

composer require psr/container
来源：http://ptf.9152youxi.cn

[U76] PHP：简单路由
来源：http://ivu.dashuyun.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mci.ivvv.top

[U77] PHP：模板渲染
来源：http://wuc.cdnleiting.top

composer require twig/twig
来源：http://qir.hammf.cn

[U78] PHP：单元测试
来源：http://gzi.yonumen.top

composer require --dev phpunit/phpunit
来源：http://dix.hammf.cn

[U79] PHP：静态分析
来源：http://uqt.hfpthk.cn

composer require --dev phpstan/phpstan
来源：http://aqd.sweek.top

[U80] PHP：代码规范修复
来源：http://kzt.hesvh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bjp.sysykeji.top

[U81] JS：初始化项目
来源：http://lpp.feifeiyinyue.top

npm init -y;  npm i express
来源：http://jyg.ehwqpu.com

[U82] JS：package.json 脚本
来源：http://bas.meibo888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wmc.52xcode.cn

[U83] JS：ES Module 导入导出
来源：http://nsg.cucudq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yyc.iojbl.cn

[U84] JS：CommonJS 写法
来源：http://tzu.zhengqikj.top

module.exports = { a };  const { a } = require("./m");
来源：http://vxi.wangshuangyany.cn

[U85] JS：可选链
来源：http://ojh.sufxvd.cn

a?.b?.c
来源：http://xng.fanxiaobao.xyz

[U86] JS：空值合并
来源：http://fxm.sufxvd.cn

a ?? b
来源：http://eir.uphjek.com

[U87] JS：解构默认值
来源：http://lkm.guowangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://jyq.fehbvm.com

[U88] JS：对象展开合并
来源：http://iyf.xuanzx.com

{ ...a, ...b }
来源：http://rpa.zhixingplan.top

[U89] JS：数组去重
来源：http://fqd.yuxming.cn

[...new Set(arr)]
来源：http://ewj.sufxvd.cn

[U90] JS：数字数组排序
来源：http://swx.shzxlz.cn

[...arr].sort((a, b) => a - b)
来源：http://jai.ydjk.org.cn

[U91] JS：对象键值遍历
来源：http://pww.yfazqb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qrj.yj202588.top

[U92] JS：深拷贝
来源：http://fdu.yangfankeji.com

structuredClone(obj)
来源：http://xgr.bbcook.cn

[U93] JS：模板字符串
来源：http://fyc.pengpengdd.cyou

`共 ${n} 条`
来源：http://pho.hesvh.cn

[U94] JS：箭头函数
来源：http://oai.hnqzz.top

const double = x => x * 2;
来源：http://oyo.vehdjk.com

[U95] JS：Promise 包装
来源：http://iop.yfazqb.com

new Promise((resolve, reject) => {})
来源：http://kdm.gogol.net.cn

[U96] JS：async/await 与异常
来源：http://ayu.hfpthk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lic.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://vqx.ivvv.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://enc.vehdjk.com

[U98] JS：fetch 带 JSON
来源：http://fvy.dianchejie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mcm.yonumen.top

[U99] JS：事件监听
来源：http://dgq.bbcook.cn

el.addEventListener("click", e => {})
来源：http://ayg.sysykeji.top

[U100] JS：DOM 查询
来源：http://gbz.aizwys.cn

document.querySelector(".item")
来源：http://tgj.jyoumei.cn

[U101] JS：classList 操作
来源：http://ylv.tarul.cn

el.classList.toggle("active")
来源：http://doa.jianghu66.top

[U102] JS：本地存储
来源：http://byw.hnqzz.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bkq.redwolf501.top

[U103] JS：定时器
来源：http://toe.smart0.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wah.ydzc1.top

[U104] JS：防抖
来源：http://zfs.gotoacloud.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ioo.52xcode.cn

[U105] JS：节流
来源：http://xyn.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zei.jinghuilouyu.cn

[U106] JS：日期格式化
来源：http://rev.wangdashe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sfe.hongshengwenyu.top

[U107] JS：数字千分位
来源：http://myn.yonumen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iju.ehwqpu.com

[U108] JS：随机整数
来源：http://cib.pycfn.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qba.sxryk.cn

[U109] JS：数组分组
来源：http://kfe.yj20258.top

Object.groupBy(arr, x => x.type)
来源：http://vuj.chenzaomai.com

[U110] JS：数组分块
来源：http://emr.bbcook.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rkp.52xcode.cn

[U111] JS：对象转 Map
来源：http://qig.hesvh.cn

new Map(Object.entries(obj))
来源：http://ggv.mhx1999.top

[U112] JS：字符串补位
来源：http://dpe.cashguo.top

"7".padStart(3, "0")
来源：http://nfw.tianlin.xyz

[U113] JS：正则替换全部
来源：http://yow.316326.xyz

s.replaceAll("a", "b")
来源：http://eja.yj202588.top

[U114] JS：JSON 深比较
来源：http://nft.hnqzz.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nvv.bjfxy.top

[U115] JS：生成 UUID
来源：http://wef.jinqigufen.top

crypto.randomUUID()
来源：http://cei.svipenyu.cn

[U116] JS：类型检查（JSDoc）
来源：http://cej.sjlbkw.cn

/** @param {string} name */ function f(name) {}
来源：http://pbc.ywan-chungtsiang.top

[U117] JS：单元测试
来源：http://huu.cashguo.top

npm i -D vitest;  npx vitest
来源：http://hap.quarkkingdee.top

[U118] JS：开发服务器
来源：http://nmf.ydzc1.top

npm i -D vite;  npx vite
来源：http://ejh.zhongyouzk.top

[U119] JS：生产构建
来源：http://kko.ivvv.top

npx vite build
来源：http://ifl.316326.xyz

[U120] JS：读取环境变量（Vite）
来源：http://gam.sxryk.cn

import.meta.env.VITE_API_URL
来源：http://gni.xylfe.cn


<!-- 参考信息 -->