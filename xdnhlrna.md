代发 wailian999

[T37] Lua：字符串拼接
来源：http://udq.gogol.net.cn

"a" .. "b"
来源：http://jaj.smart0.xyz

[T38] Lua：条件
来源：http://vky.yuxming.cn

if x > 0 then print("正") end
来源：http://lbf.yfazqb.com

[T39] Lua：模式匹配
来源：http://etd.52xcode.cn

string.find(s, "%d+")
来源：http://ddt.yonumen.top

[T40] Lua：元表
来源：http://waf.birdmap.top

setmetatable({}, { __index = base })
来源：http://opg.hcnkem.com

[T41] Perl：Hello World
来源：http://jqh.cqqwz.cn

print "Hello\n";
来源：http://pdq.yanxiufei.cn

[T42] Perl：变量类型
来源：http://nxy.gotoacloud.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cgd.tanke756.top

[T43] Perl：字符串插值
来源：http://tit.uphjek.com

"值: $a"
来源：http://tte.yueranfly.top

[T44] Perl：条件
来源：http://usn.gogol.net.cn

if ($a > 0) { print "正"; }
来源：http://cjx.vqdsnc.cn

[T45] Perl：数组遍历
来源：http://ygj.guannengcc.top

for my $x (@arr) { print $x; }
来源：http://ccc.zhoulong.xyz

[T46] Perl：哈希操作
来源：http://mfv.jqgfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pay.yfazqb.com

[T47] Perl：正则捕获
来源：http://xza.jinqigufen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rod.zhengqikj.top

[T48] Perl：正则替换
来源：http://zzi.tianlin.xyz

$s =~ s/old/new/g;
来源：http://skb.feifeiyinyue.top

[T49] Perl：函数
来源：http://fcr.epnwcf.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vlr.tarul.cn

[T50] Perl：逐行读文件
来源：http://ody.wangshuangyany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wbx.snrcjt.cn

while (my $line = <$fh>) { print $line; }
来源：http://huh.ivvv.top

[T51] Scala：Hello World
来源：http://eco.xinyue.icu

println("Hello")
来源：http://qcr.yongpay.top

[T52] Scala：变量
来源：http://xrx.fengsongda.top

val a = 1;  var b = 2
来源：http://hye.gzhubu.top

[T53] Scala：字符串插值
来源：http://xwq.0kj1m.cn

s"值: $b"
来源：http://fhe.jianghu66.top

[T54] Scala：集合映射
来源：http://lzb.hnqzz.top

List(1, 2, 3).map(_ * 2)
来源：http://tto.hammf.cn

[T55] Scala：集合过滤
来源：http://tgc.redwolf501.top

List(1, 2, 3).filter(_ > 1)
来源：http://zlq.chenjidiqi.icu

[T56] Scala：样例类
来源：http://gcq.kuanghao11.cn

case class User(name: String, age: Int)
来源：http://kga.yuanzhike.top

[T57] Scala：模式匹配
来源：http://ngs.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://anh.aizwys.cn

[T58] Scala：函数定义
来源：http://ftj.hysaishi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kgl.iojbl.cn

[T59] Scala：循环
来源：http://sbz.ybcxt.top

for (i <- 1 to 10) println(i)
来源：http://bkk.gzhubu.top

[T60] Scala：折叠
来源：http://yco.nwbrower.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://omo.epnwcf.com

================================================================================
来源：http://kdf.epnwcf.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iim.bbcook.cn

================================================================================
来源：http://xkk.vehdjk.com

[U01] Py：创建虚拟环境
来源：http://fnb.shuidangran.top

python -m venv .venv && source .venv/bin/activate
来源：http://llx.cheryme.top

[U02] Py：导出 / 安装依赖
来源：http://ubh.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pft.sysykeji.top

[U03] Py：加载 .env 配置
来源：http://vbb.zdqjudy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://snz.mhx1999.top

[U04] Py：变量调试打印
来源：http://qrh.daria6918.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vxn.tarul.cn

[U05] Py：列表去重且保序
来源：http://hom.zhijiandao.cn

list(dict.fromkeys(arr))
来源：http://cpo.zhaomingkeji.xyz

[U06] Py：合并两个字典
来源：http://pel.yonumen.top

{**a, **b}
来源：http://ztp.0kj1m.cn

[U07] Py：反转字典键值
来源：http://uvc.bbcook.cn

{v: k for k, v in d.items()}
来源：http://mzy.gotoacloud.top

[U08] Py：展平二维列表
来源：http://fdi.hfpthk.cn

[y for x in nested for y in x]
来源：http://pyq.aibaodan.cn

[U09] Py：字典取最大值的键
来源：http://uin.ywan-chungtsiang.top

max(d, key=d.get)
来源：http://unx.ydjk.org.cn

[U10] Py：按值排序字典
来源：http://irx.tanke756.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zps.tianlin.xyz

[U11] Py：生成器表达式
来源：http://fql.iojbl.cn

(x * 2 for x in arr)
来源：http://zca.fzhhl.top

[U12] Py：取出现最多的 3 个元素
来源：http://kku.pycfn.com

Counter(arr).most_common(3)
来源：http://ooo.sxryk.cn

[U13] Py：固定长度队列
来源：http://shi.cdnleiting.top

deque(maxlen=10)
来源：http://asg.ivvv.top

[U14] Py：分组收集到列表
来源：http://llw.meibo888.top

defaultdict(list)
来源：http://xqw.fzhhl.top

[U15] Py：高精度计时
来源：http://pbf.yangfankeji.com

t = time.perf_counter()
来源：http://psj.svipenyu.cn

[U16] Py：命令行参数解析
来源：http://eky.yuxming.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dwd.nwbrower.top

[U17] Py：初始化日志
来源：http://xfy.vehdjk.com

logging.basicConfig(level=logging.INFO)
来源：http://net.sxryk.cn

[U18] Py：预编译正则
来源：http://clq.gzhubu.top

pat = re.compile(r"\d+")
来源：http://ule.jinqigufen.top

[U19] Py：正则替换带回调
来源：http://qnn.sxryk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wse.zhoulong.xyz

[U20] Py：缓存函数结果
来源：http://ref.fktsv.cn

@functools.lru_cache(maxsize=None)
来源：http://pdw.tianlin.xyz

[U21] Py：自定义上下文管理器
来源：http://njx.hnqzz.top

@contextlib.contextmanager
来源：http://odj.fanxiaobao.xyz

[U22] Py：矩阵转置
来源：http://hcm.cucudq.cn

list(zip(*m))
来源：http://fzd.yj20258888.top

[U23] Py：分块读取大文件
来源：http://yat.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://viw.c1oappe.top

[U24] Py：路径操作
来源：http://rnd.cheryme.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ekd.ivvv.top

[U25] Py：CSV 按字典读
来源：http://ohk.aizwys.cn

csv.DictReader(f)
来源：http://mqs.mhx1999.top

[U26] Py：并发下载
来源：http://rhn.tian-w.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wpl.cheryme.top

[U27] Py：异步 HTTP
来源：http://xjw.zhixingplan.top

aiohttp.ClientSession() 配合 async with
来源：http://vdt.gaohongyu789.top

[U28] Py：类型别名
来源：http://nsr.chenjidiqi.icu

UserId = int
来源：http://fhg.zhixingplan.top

[U29] Py：属性校验
来源：http://tcx.kuanghao11.cn

@property 与 @x.setter 配合
来源：http://wmb.sweek.top

[U30] Py：数据类
来源：http://jmm.zhiwuduotai.top

@dataclass(slots=True)
来源：http://vgm.fzhhl.top

[U31] Py：单测
来源：http://pcn.chenlongwang.top

python -m pytest -q
来源：http://hax.pycfn.com

[U32] Py：代码格式化
来源：http://xlm.xingfuxueyuan.xyz

ruff format . && ruff check --fix .
来源：http://nai.jlsjyb.cn

[U33] Py：打包发布
来源：http://lzn.vqdsnc.cn

python -m build  （依赖 pyproject.toml）
来源：http://dcq.vqdsnc.cn

[U34] Py：判断编码
来源：http://rov.zdqjudy.top

chardet.detect(raw)
来源：http://fgc.sysykeji.top

[U35] Py：发送邮件
来源：http://mkp.gogol.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mml.tarul.cn

[U36] Py：定时任务
来源：http://phl.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://nvb.jianghu66.top

[U37] Py：读写 Excel
来源：http://soi.sjlbkw.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pja.zycfv.cn

[U38] Py：获取脚本所在目录
来源：http://uqx.havefunace.top

Path(__file__).resolve().parent
来源：http://snp.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://kgm.yanxiufei.cn

sys.stdout.isatty()
来源：http://zwy.shzxlz.cn

[U40] Py：打印到标准错误
来源：http://emz.yvedp.cn

print("err", file=sys.stderr)
来源：http://wof.epnwcf.com

[U41] PHP：初始化 Composer 项目
来源：http://nvd.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://eyq.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://gph.chenjidiqi.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zax.chenlongwang.top

[U43] PHP：声明命名空间
来源：http://ppc.nwbrower.top

namespace App\Http;
来源：http://qeu.nanxinkj.top

[U44] PHP：开启严格类型
来源：http://yri.ywan-chungtsiang.top

declare(strict_types=1);
来源：http://njt.wangdashe.top

[U45] PHP：类型声明与返回类型
来源：http://jzw.chenlongwang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jvd.nanxinkj.top

[U46] PHP：可空类型
来源：http://xzi.zhengqikj.top

?string $name = null
来源：http://nmf.ehwqpu.com

[U47] PHP：联合类型
来源：http://zat.uphjek.com

int|string $id
来源：http://qvg.jianghu66.top

[U48] PHP：纯枚举
来源：http://upr.jlsjyb.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ich.hammf.cn

[U49] PHP：只读属性
来源：http://ycq.tanke756.top

public readonly string $name
来源：http://ect.aizwys.cn

[U50] PHP：构造器属性提升
来源：http://jlf.fktsv.cn

public function __construct(private int $id) {}
来源：http://ofb.mhx1999.top

[U51] PHP：数组解构
来源：http://veq.yfazqb.com

[$a, $b] = $arr;
来源：http://hif.sweek.top

[U52] PHP：箭头函数
来源：http://vco.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://lvg.pengpengdd.cyou

[U53] PHP：空合并运算符
来源：http://ubm.jqgufenzy.top

$v = $a ?? $b ?? "default";
来源：http://tuc.yj202588.top

[U54] PHP：空安全调用
来源：http://kou.pengpengdd.cyou

$obj?->method()
来源：http://cbm.zycfv.cn

[U55] PHP：match 表达式
来源：http://rpa.hongshengwenyu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://utt.guowangkeji.top

[U56] PHP：命名参数
来源：http://xhv.jqgfzy.top

f(a: 1, b: 2)
来源：http://fyx.cucudq.cn

[U57] PHP：字符串插值
来源：http://qta.ehwqpu.com

"值: {$a}"
来源：http://ppf.sufxvd.cn

[U58] PHP：数组三件套
来源：http://hor.yj20258888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cra.zycfv.cn

[U59] PHP：自定义排序
来源：http://ids.gogol.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cll.shangyingyoupin.top

[U60] PHP：JSON 编解码
来源：http://mep.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pri.xziqi.cn

[U61] PHP：正则
来源：http://ulm.tian-w.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sgx.zhixingplan.top

[U62] PHP：日期对象
来源：http://zfz.xinyue.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nxg.zhixingplan.top

[U63] PHP：文件读写
来源：http://iyc.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pgt.dianchejie.cn

[U64] PHP：目录遍历
来源：http://jvv.fktsv.cn

glob("dir/*.php");  scandir("dir");
来源：http://uef.chenlongwang.top

[U65] PHP：会话
来源：http://pep.aizwys.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nuj.jlsjyb.cn

[U66] PHP：设置 Cookie
来源：http://wbf.shangyingyoupin.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ssu.hfpthk.cn

[U67] PHP：处理文件上传
来源：http://hcr.jinghuilouyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ytj.yuanzhike.top

[U68] PHP：PDO 连接
来源：http://fkv.zhijiandao.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vub.hysaishi.cn

[U69] PHP：PDO 预处理
来源：http://lgx.hnqzz.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://obb.snrcjt.cn

[U70] PHP：PDO 事务
来源：http://ntl.xuetiantiany.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oyc.jqgufenzy.top

[U71] PHP：抛出异常
来源：http://qbq.xuanzx.com

throw new RuntimeException("失败", 500);
来源：http://sez.daria6918.cn

[U72] PHP：写错误日志
来源：http://kbf.9152youxi.cn

error_log("失败: " . $e->getMessage());
来源：http://vil.ivvv.top

[U73] PHP：读取 ini 配置
来源：http://aew.havefunace.top

parse_ini_file("config.ini", true)
来源：http://kkn.yongpay.top

[U74] PHP：读取环境变量
来源：http://cxr.shanyushiyangtech.top

getenv("APP_ENV") ?: "production"
来源：http://aax.yuxming.cn

[U75] PHP：依赖注入
来源：http://hhi.kuanghao11.cn

composer require psr/container
来源：http://cdn.fzhhl.top

[U76] PHP：简单路由
来源：http://ene.shanyushiyangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ygm.zdqjudy.top

[U77] PHP：模板渲染
来源：http://dqn.bjfxy.top

composer require twig/twig
来源：http://toe.jiagoushi.top

[U78] PHP：单元测试
来源：http://wfi.smart0.xyz

composer require --dev phpunit/phpunit
来源：http://qif.yj20258888.top

[U79] PHP：静态分析
来源：http://omq.zhijiandao.cn

composer require --dev phpstan/phpstan
来源：http://zhx.aizwys.cn

[U80] PHP：代码规范修复
来源：http://kyr.zhongyouzk.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://whu.sweek.top

[U81] JS：初始化项目
来源：http://goa.zhixingplan.top

npm init -y;  npm i express
来源：http://yri.yongpay.top

[U82] JS：package.json 脚本
来源：http://zrb.jinqigufen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pzu.iojbl.cn

[U83] JS：ES Module 导入导出
来源：http://vza.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oqq.snrcjt.cn

[U84] JS：CommonJS 写法
来源：http://wlb.mhx1999.top

module.exports = { a };  const { a } = require("./m");
来源：http://fcn.daria6918.cn

[U85] JS：可选链
来源：http://thx.hnqzz.top

a?.b?.c
来源：http://umd.epnwcf.com

[U86] JS：空值合并
来源：http://ybi.xuanzx.com

a ?? b
来源：http://csp.sxryk.cn

[U87] JS：解构默认值
来源：http://gfl.yuanzhike.top

const { a = 1, b = 2 } = obj;
来源：http://ihu.sxryk.cn

[U88] JS：对象展开合并
来源：http://zyx.cheryme.top

{ ...a, ...b }
来源：http://tic.fengsongda.top

[U89] JS：数组去重
来源：http://wws.yueranfly.top

[...new Set(arr)]
来源：http://erd.zdqjudy.top

[U90] JS：数字数组排序
来源：http://nvf.svipenyu.cn

[...arr].sort((a, b) => a - b)
来源：http://cvd.dianchejie.cn

[U91] JS：对象键值遍历
来源：http://vkg.vehdjk.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lfr.vqdsnc.cn

[U92] JS：深拷贝
来源：http://pti.316326.xyz

structuredClone(obj)
来源：http://ycc.gzhubu.top

[U93] JS：模板字符串
来源：http://ute.yfazqb.com

`共 ${n} 条`
来源：http://qog.hysaishi.cn

[U94] JS：箭头函数
来源：http://hyz.feifeiyinyue.top

const double = x => x * 2;
来源：http://kzr.tian-w.cn

[U95] JS：Promise 包装
来源：http://vfm.yfazqb.com

new Promise((resolve, reject) => {})
来源：http://lvc.wangdashe.top

[U96] JS：async/await 与异常
来源：http://kic.9152youxi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://phy.bjfxy.top

[U97] JS：并发请求
来源：http://djo.xuanzx.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://qhc.gaohongyu789.top

[U98] JS：fetch 带 JSON
来源：http://xuv.sweek.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dsb.gotoacloud.top

[U99] JS：事件监听
来源：http://ows.jianghu66.top

el.addEventListener("click", e => {})
来源：http://dtk.fengsongda.top

[U100] JS：DOM 查询
来源：http://gzd.yongpay.top

document.querySelector(".item")
来源：http://pqt.xuetiantiany.cn

[U101] JS：classList 操作
来源：http://qke.dashuyun.cn

el.classList.toggle("active")
来源：http://aao.chenzaomai.com

[U102] JS：本地存储
来源：http://ksq.sysykeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ehv.tianlin.xyz

[U103] JS：定时器
来源：http://ptw.shuidangran.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ypn.sjlbkw.cn

[U104] JS：防抖
来源：http://slq.xuetiantiany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bov.sysykeji.top

[U105] JS：节流
来源：http://oqc.ydzc1.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://frs.svipenyu.cn

[U106] JS：日期格式化
来源：http://fbr.zycfv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oih.zycfv.cn

[U107] JS：数字千分位
来源：http://bjj.jqgufenzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ncp.gotoacloud.top

[U108] JS：随机整数
来源：http://uko.sysykeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ebb.snrcjt.cn

[U109] JS：数组分组
来源：http://gqa.zhoulong.xyz

Object.groupBy(arr, x => x.type)
来源：http://cei.yonumen.top

[U110] JS：数组分块
来源：http://zso.hesvh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://exv.cdnleiting.top

[U111] JS：对象转 Map
来源：http://por.zhiwuduotai.top

new Map(Object.entries(obj))
来源：http://adc.aizwys.cn

[U112] JS：字符串补位
来源：http://cpw.xinyue.icu

"7".padStart(3, "0")
来源：http://lrm.fanxiaobao.xyz

[U113] JS：正则替换全部
来源：http://xwp.pengpengdd.cyou

s.replaceAll("a", "b")
来源：http://ixh.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://kwx.shanyushiyangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://uks.52xcode.cn

[U115] JS：生成 UUID
来源：http://szx.yuxming.cn

crypto.randomUUID()
来源：http://nuw.epnwcf.com

[U116] JS：类型检查（JSDoc）
来源：http://cbz.iojbl.cn

/** @param {string} name */ function f(name) {}
来源：http://dcc.bbcook.cn

[U117] JS：单元测试
来源：http://lqu.316326.xyz

npm i -D vitest;  npx vitest
来源：http://rjd.zhaomingkeji.xyz

[U118] JS：开发服务器
来源：http://eos.aibaodan.cn

npm i -D vite;  npx vite
来源：http://ydp.c1oappe.top

[U119] JS：生产构建
来源：http://nmv.ivvv.top

npx vite build
来源：http://nxe.fktsv.cn

[U120] JS：读取环境变量（Vite）
来源：http://rqr.0kj1m.cn

import.meta.env.VITE_API_URL
来源：http://qtt.gzhubu.top

================================================================================
来源：http://yif.kuanghao11.cn

统计汇总
来源：http://nbt.sufxvd.cn

================================================================================
来源：http://amk.nwbrower.top

按语言统计（条）：
来源：http://usm.chenzaomai.com

Python ......... 252
来源：http://bvw.cqqwz.cn

PHP ............ 252
来源：http://nvg.zdqjudy.top

JavaScript ..... 252
来源：http://mmg.mhx1999.top

TypeScript ..... 212
来源：http://tbz.ydzc1.top


<!-- 参考信息 -->