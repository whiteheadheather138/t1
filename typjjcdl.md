代发 wailian999

[T35] Lua：字典表
来源：http://kba.daxiang520.top

local d = { a = 1 };  d.b = 2
来源：http://kwe.chenzaomai.com

[T36] Lua：函数
来源：http://ets.pengpengdd.cyou

function add(a, b) return a + b end
来源：http://qka.ywan-chungtsiang.top

[T37] Lua：字符串拼接
来源：http://cyp.ydzc1.top

"a" .. "b"
来源：http://eov.zhixingplan.top

[T38] Lua：条件
来源：http://dzd.jinghuilouyu.cn

if x > 0 then print("正") end
来源：http://yvj.jinyuanbaomall.cn

[T39] Lua：模式匹配
来源：http://mqo.shanyushiyangtech.top

string.find(s, "%d+")
来源：http://urv.ctjpmb.com

[T40] Lua：元表
来源：http://pwf.nwbrower.top

setmetatable({}, { __index = base })
来源：http://kfy.zycfv.cn

[T41] Perl：Hello World
来源：http://ehm.iojbl.cn

print "Hello\n";
来源：http://yqr.shangyingyoupin.top

[T42] Perl：变量类型
来源：http://cir.hysaishi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dtz.aibaodan.cn

[T43] Perl：字符串插值
来源：http://gok.yongpay.top

"值: $a"
来源：http://don.hysaishi.cn

[T44] Perl：条件
来源：http://wxm.zhaomingkeji.xyz

if ($a > 0) { print "正"; }
来源：http://jxd.hywenlv.cn

[T45] Perl：数组遍历
来源：http://wcj.sweek.top

for my $x (@arr) { print $x; }
来源：http://qer.cucudq.cn

[T46] Perl：哈希操作
来源：http://pui.tian-w.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aqp.ybcxt.top

[T47] Perl：正则捕获
来源：http://kbm.wangshuangyany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hwz.hongshengwenyu.top

[T48] Perl：正则替换
来源：http://vpg.ctjpmb.com

$s =~ s/old/new/g;
来源：http://tum.bbcook.cn

[T49] Perl：函数
来源：http://cyg.xuetiantiany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rfn.sufxvd.cn

[T50] Perl：逐行读文件
来源：http://dyo.ydzc1.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vhg.ehwqpu.com

while (my $line = <$fh>) { print $line; }
来源：http://vth.ydjk.org.cn

[T51] Scala：Hello World
来源：http://zcz.aibaodan.cn

println("Hello")
来源：http://ozc.vehdjk.com

[T52] Scala：变量
来源：http://ujv.shangyingyoupin.top

val a = 1;  var b = 2
来源：http://jyh.yonumen.top

[T53] Scala：字符串插值
来源：http://pqw.fanxiaobao.xyz

s"值: $b"
来源：http://izp.gogol.net.cn

[T54] Scala：集合映射
来源：http://tmr.jinghuilouyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://hlz.ctjpmb.com

[T55] Scala：集合过滤
来源：http://ukp.zhaomingkeji.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://fsy.yvedp.cn

[T56] Scala：样例类
来源：http://goj.yongpay.top

case class User(name: String, age: Int)
来源：http://joa.bbcook.cn

[T57] Scala：模式匹配
来源：http://cak.yueranfly.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dcn.shzxlz.cn

[T58] Scala：函数定义
来源：http://oph.chenjidiqi.icu

def add(a: Int, b: Int): Int = a + b
来源：http://pcn.bjfxy.top

[T59] Scala：循环
来源：http://dxw.hnqzz.top

for (i <- 1 to 10) println(i)
来源：http://rki.sxryk.cn

[T60] Scala：折叠
来源：http://qhj.zdbjq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vph.iojbl.cn

================================================================================
来源：http://ahm.uphjek.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://szf.jinqigfzy.top

================================================================================
来源：http://eyr.zhaomingkeji.xyz

[U01] Py：创建虚拟环境
来源：http://nmc.zhaomingkeji.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://udv.sweek.top

[U02] Py：导出 / 安装依赖
来源：http://jvw.shanyushiyangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wal.ehwqpu.com

[U03] Py：加载 .env 配置
来源：http://wby.hnqzz.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kfl.xinyue.icu

[U04] Py：变量调试打印
来源：http://nrs.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wnv.zhijiandao.cn

[U05] Py：列表去重且保序
来源：http://rzi.cdnleiting.top

list(dict.fromkeys(arr))
来源：http://xdv.shzxlz.cn

[U06] Py：合并两个字典
来源：http://ljp.fanxiaobao.xyz

{**a, **b}
来源：http://ocd.sufxvd.cn

[U07] Py：反转字典键值
来源：http://ljc.yanxiufei.cn

{v: k for k, v in d.items()}
来源：http://wtc.52xcode.cn

[U08] Py：展平二维列表
来源：http://ove.nwbrower.top

[y for x in nested for y in x]
来源：http://wzl.hesvh.cn

[U09] Py：字典取最大值的键
来源：http://cuw.ydjk.org.cn

max(d, key=d.get)
来源：http://etr.pengpengdd.cyou

[U10] Py：按值排序字典
来源：http://lqi.yuanzhike.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yer.52xcode.cn

[U11] Py：生成器表达式
来源：http://wjh.yfazqb.com

(x * 2 for x in arr)
来源：http://ldr.zhoulong.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://wei.birdmap.top

Counter(arr).most_common(3)
来源：http://ysu.tanke756.top

[U13] Py：固定长度队列
来源：http://foe.dashuyun.cn

deque(maxlen=10)
来源：http://bgz.pycfn.com

[U14] Py：分组收集到列表
来源：http://nqj.tianlin.xyz

defaultdict(list)
来源：http://lwu.zhiwuduotai.top

[U15] Py：高精度计时
来源：http://rjq.iojbl.cn

t = time.perf_counter()
来源：http://oer.gotoacloud.top

[U16] Py：命令行参数解析
来源：http://ajy.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cnq.jinyuanbaomall.cn

[U17] Py：初始化日志
来源：http://ojg.fengsongda.top

logging.basicConfig(level=logging.INFO)
来源：http://yke.nanxinkj.top

[U18] Py：预编译正则
来源：http://qam.nanxinkj.top

pat = re.compile(r"\d+")
来源：http://fzg.yangfankeji.com

[U19] Py：正则替换带回调
来源：http://cih.yuxming.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pix.xingfuxueyuan.xyz

[U20] Py：缓存函数结果
来源：http://dhv.tianlin.xyz

@functools.lru_cache(maxsize=None)
来源：http://tra.sxryk.cn

[U21] Py：自定义上下文管理器
来源：http://tsa.guowangkeji.top

@contextlib.contextmanager
来源：http://dkg.hesvh.cn

[U22] Py：矩阵转置
来源：http://iqp.yangfankeji.com

list(zip(*m))
来源：http://cna.hesvh.cn

[U23] Py：分块读取大文件
来源：http://wvc.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lpl.gzhubu.top

[U24] Py：路径操作
来源：http://mwv.gaohongyu789.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://unv.dashuyun.cn

[U25] Py：CSV 按字典读
来源：http://tom.guannengcc.top

csv.DictReader(f)
来源：http://oep.0kj1m.cn

[U26] Py：并发下载
来源：http://fqn.nwbrower.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ijo.chenlongwang.top

[U27] Py：异步 HTTP
来源：http://jkz.yuanzhike.top

aiohttp.ClientSession() 配合 async with
来源：http://tbi.shzxlz.cn

[U28] Py：类型别名
来源：http://wnw.zycfv.cn

UserId = int
来源：http://kpt.sysykeji.top

[U29] Py：属性校验
来源：http://wrb.yanxiufei.cn

@property 与 @x.setter 配合
来源：http://kgy.xingfuxueyuan.xyz

[U30] Py：数据类
来源：http://ysh.zhengqikj.top

@dataclass(slots=True)
来源：http://djb.hammf.cn

[U31] Py：单测
来源：http://xhr.haohaochexian.top

python -m pytest -q
来源：http://lsb.yj20258888.top

[U32] Py：代码格式化
来源：http://ezf.jqgufenzy.top

ruff format . && ruff check --fix .
来源：http://tyf.zycfv.cn

[U33] Py：打包发布
来源：http://mbb.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://bcw.zhongyouzk.top

[U34] Py：判断编码
来源：http://baa.aizwys.cn

chardet.detect(raw)
来源：http://ryu.ybcxt.top

[U35] Py：发送邮件
来源：http://xtc.hysaishi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dhi.dashuyun.cn

[U36] Py：定时任务
来源：http://vjx.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://gyl.wangshuangyany.cn

[U37] Py：读写 Excel
来源：http://xae.yonumen.top

pandas.read_excel / DataFrame.to_excel
来源：http://knw.wangdashe.top

[U38] Py：获取脚本所在目录
来源：http://ejo.xuetiantiany.cn

Path(__file__).resolve().parent
来源：http://ohw.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://aqj.tanke756.top

sys.stdout.isatty()
来源：http://yyw.zhengqikj.top

[U40] Py：打印到标准错误
来源：http://ule.sysykeji.top

print("err", file=sys.stderr)
来源：http://rsi.bbcook.cn

[U41] PHP：初始化 Composer 项目
来源：http://oko.zhengqikj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://hqf.nanxuanxn.top

[U42] PHP：PSR-4 自动加载
来源：http://eha.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nli.c1oappe.top

[U43] PHP：声明命名空间
来源：http://sjp.tian-w.cn

namespace App\Http;
来源：http://iuv.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://inn.vehdjk.com

declare(strict_types=1);
来源：http://zcg.tarul.cn

[U45] PHP：类型声明与返回类型
来源：http://hjw.gzhubu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://che.yj202588.top

[U46] PHP：可空类型
来源：http://mnh.fzhhl.top

?string $name = null
来源：http://okq.xingfuxueyuan.xyz

[U47] PHP：联合类型
来源：http://jhf.52xcode.cn

int|string $id
来源：http://izx.pycfn.com

[U48] PHP：纯枚举
来源：http://psl.0kj1m.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pzg.sxryk.cn

[U49] PHP：只读属性
来源：http://fxm.zhixingplan.top

public readonly string $name
来源：http://kem.shuidangran.top

[U50] PHP：构造器属性提升
来源：http://hpc.jinghuilouyu.cn

public function __construct(private int $id) {}
来源：http://idq.yangfankeji.com

[U51] PHP：数组解构
来源：http://ijd.gzhubu.top

[$a, $b] = $arr;
来源：http://fms.ehwqpu.com

[U52] PHP：箭头函数
来源：http://yrd.xylfe.cn

$double = fn($x) => $x * 2;
来源：http://bma.daria6918.cn

[U53] PHP：空合并运算符
来源：http://exg.epnwcf.com

$v = $a ?? $b ?? "default";
来源：http://okh.uphjek.com

[U54] PHP：空安全调用
来源：http://wmc.tian-w.cn

$obj?->method()
来源：http://unv.shuidangran.top

[U55] PHP：match 表达式
来源：http://yzf.bjfxy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://onx.cucudq.cn

[U56] PHP：命名参数
来源：http://gzj.svipenyu.cn

f(a: 1, b: 2)
来源：http://zty.aizwys.cn

[U57] PHP：字符串插值
来源：http://uuo.ehwqpu.com

"值: {$a}"
来源：http://uqy.yuanzhike.top

[U58] PHP：数组三件套
来源：http://von.yuanzhike.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dap.iojbl.cn

[U59] PHP：自定义排序
来源：http://cra.yfazqb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xtj.yueranfly.top

[U60] PHP：JSON 编解码
来源：http://zqx.hongshengwenyu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hog.xuanzx.com

[U61] PHP：正则
来源：http://udw.zhiwuduotai.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wcz.tarul.cn

[U62] PHP：日期对象
来源：http://mqg.chenzaomai.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bbu.jianghu66.top

[U63] PHP：文件读写
来源：http://xnq.ppjwa.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ysr.sysykeji.top

[U64] PHP：目录遍历
来源：http://mgi.smart0.xyz

glob("dir/*.php");  scandir("dir");
来源：http://akk.shzxlz.cn

[U65] PHP：会话
来源：http://ord.jlsjyb.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fih.daxiang520.top

[U66] PHP：设置 Cookie
来源：http://cnr.zhijiandao.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fww.ybcxt.top

[U67] PHP：处理文件上传
来源：http://spf.jiagoushi.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zgm.zhixingplan.top

[U68] PHP：PDO 连接
来源：http://xku.chenjidiqi.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tik.sjlbkw.cn

[U69] PHP：PDO 预处理
来源：http://kcc.nanxuanxn.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://clo.shangyingyoupin.top

[U70] PHP：PDO 事务
来源：http://fsw.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qem.meibo888.top

[U71] PHP：抛出异常
来源：http://rbr.hnxiangtu.top

throw new RuntimeException("失败", 500);
来源：http://orn.iojbl.cn

[U72] PHP：写错误日志
来源：http://cvo.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://fyd.jinqigfzy.top

[U73] PHP：读取 ini 配置
来源：http://wsp.xziqi.cn

parse_ini_file("config.ini", true)
来源：http://znl.zhaomingkeji.xyz

[U74] PHP：读取环境变量
来源：http://tvb.fanxiaobao.xyz

getenv("APP_ENV") ?: "production"
来源：http://ksl.ppjwa.cn

[U75] PHP：依赖注入
来源：http://oej.quarkkingdee.top

composer require psr/container
来源：http://ssz.zhoulong.xyz

[U76] PHP：简单路由
来源：http://spv.zdqjudy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zti.hammf.cn

[U77] PHP：模板渲染
来源：http://sfe.jiagoushi.top

composer require twig/twig
来源：http://rxl.yonumen.top

[U78] PHP：单元测试
来源：http://gxc.zhixingplan.top

composer require --dev phpunit/phpunit
来源：http://koi.fanxiaobao.xyz

[U79] PHP：静态分析
来源：http://bpe.pengpengdd.cyou

composer require --dev phpstan/phpstan
来源：http://oxg.c1oappe.top

[U80] PHP：代码规范修复
来源：http://olc.chenjidiqi.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://juj.hfpthk.cn

[U81] JS：初始化项目
来源：http://zxv.shanyushiyangtech.top

npm init -y;  npm i express
来源：http://wfi.jinqigufen.top

[U82] JS：package.json 脚本
来源：http://vxn.vehdjk.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yez.yanxiufei.cn

[U83] JS：ES Module 导入导出
来源：http://hke.haohaochexian.top

export const a = 1;  import { a } from "./m.js";
来源：http://qoe.hfpthk.cn

[U84] JS：CommonJS 写法
来源：http://flc.tanke756.top

module.exports = { a };  const { a } = require("./m");
来源：http://dwn.guannengcc.top

[U85] JS：可选链
来源：http://ovw.ydzc1.top

a?.b?.c
来源：http://qdq.zhongyouzk.top

[U86] JS：空值合并
来源：http://ure.yuxming.cn

a ?? b
来源：http://boj.c1oappe.top

[U87] JS：解构默认值
来源：http://rwl.zhixingplan.top

const { a = 1, b = 2 } = obj;
来源：http://kcd.svipenyu.cn

[U88] JS：对象展开合并
来源：http://qsz.yj20258888.top

{ ...a, ...b }
来源：http://sgx.fzhhl.top

[U89] JS：数组去重
来源：http://ekw.fanxiaobao.xyz

[...new Set(arr)]
来源：http://lad.c1oappe.top

[U90] JS：数字数组排序
来源：http://xni.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://upo.vehdjk.com

[U91] JS：对象键值遍历
来源：http://glj.zhengqikj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://epf.sysykeji.top

[U92] JS：深拷贝
来源：http://hic.haohaochexian.top

structuredClone(obj)
来源：http://mkw.aizwys.cn

[U93] JS：模板字符串
来源：http://lsd.hnxiangtu.top

`共 ${n} 条`
来源：http://kai.guowangkeji.top

[U94] JS：箭头函数
来源：http://ejx.sjlbkw.cn

const double = x => x * 2;
来源：http://lwk.hesvh.cn

[U95] JS：Promise 包装
来源：http://hhq.yongpay.top

new Promise((resolve, reject) => {})
来源：http://hso.pengpengdd.cyou

[U96] JS：async/await 与异常
来源：http://vsu.ivvv.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dqh.shzxlz.cn

[U97] JS：并发请求
来源：http://qbb.gzhubu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ilv.hfpthk.cn

[U98] JS：fetch 带 JSON
来源：http://gmo.ydjk.org.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tvy.cheryme.top

[U99] JS：事件监听
来源：http://kay.mhx1999.top

el.addEventListener("click", e => {})
来源：http://hud.jyoumei.cn

[U100] JS：DOM 查询
来源：http://dhv.ydzc1.top

document.querySelector(".item")
来源：http://ohj.svipenyu.cn

[U101] JS：classList 操作
来源：http://bdj.chenjidiqi.icu

el.classList.toggle("active")
来源：http://fus.ehwqpu.com

[U102] JS：本地存储
来源：http://hxj.sysykeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hrp.yj202588.top

[U103] JS：定时器
来源：http://zay.hcnkem.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xor.chenzaomai.com

[U104] JS：防抖
来源：http://ysm.jinqigufen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sfc.ivvv.top

[U105] JS：节流
来源：http://wyc.jinyuanbaomall.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bzb.zhiwuduotai.top

[U106] JS：日期格式化
来源：http://hib.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gtn.bbcook.cn

[U107] JS：数字千分位
来源：http://axy.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yty.zhoulong.xyz

[U108] JS：随机整数
来源：http://xaj.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://drw.birdmap.top

[U109] JS：数组分组
来源：http://zkh.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://ney.jinyuanbaomall.cn

[U110] JS：数组分块
来源：http://dye.xingfuxueyuan.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ymn.cdnleiting.top

[U111] JS：对象转 Map
来源：http://cec.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://pvj.zhoulong.xyz

[U112] JS：字符串补位
来源：http://qkn.feifeiyinyue.top

"7".padStart(3, "0")
来源：http://qti.fehbvm.com

[U113] JS：正则替换全部
来源：http://bed.yanxiufei.cn

s.replaceAll("a", "b")
来源：http://aop.chenzaomai.com

[U114] JS：JSON 深比较
来源：http://kmr.sysykeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pdl.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://leh.xinyue.icu

crypto.randomUUID()
来源：http://rxo.shuidangran.top

[U116] JS：类型检查（JSDoc）
来源：http://hww.jianghu66.top

/** @param {string} name */ function f(name) {}
来源：http://ryp.tarul.cn

[U117] JS：单元测试
来源：http://qwr.gotoacloud.top

npm i -D vitest;  npx vitest
来源：http://twn.yj202588.top

[U118] JS：开发服务器
来源：http://xnd.yanxiufei.cn

npm i -D vite;  npx vite
来源：http://lwe.tianlin.xyz

[U119] JS：生产构建
来源：http://lst.jinyuanbaomall.cn

npx vite build
来源：http://xwk.yj20258.top

[U120] JS：读取环境变量（Vite）
来源：http://fhw.snrcjt.cn

import.meta.env.VITE_API_URL
来源：http://tfa.chenjidiqi.icu

================================================================================
来源：http://sjw.yj20258888.top

统计汇总
来源：http://see.cdnleiting.top

================================================================================
来源：http://dcx.bbcook.cn

按语言统计（条）：
来源：http://dfh.dashuyun.cn


<!-- 参考信息 -->