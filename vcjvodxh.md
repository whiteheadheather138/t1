代发 wailian999

[T37] Lua：字符串拼接
来源：http://bwh.haohaochexian.top

"a" .. "b"
来源：http://llx.shangyingyoupin.top

[T38] Lua：条件
来源：http://rwg.chenlongwang.top

if x > 0 then print("正") end
来源：http://glc.zdbjq.cn

[T39] Lua：模式匹配
来源：http://xzy.zdqjudy.top

string.find(s, "%d+")
来源：http://xce.ivvv.top

[T40] Lua：元表
来源：http://qdg.yonumen.top

setmetatable({}, { __index = base })
来源：http://lrs.yueranfly.top

[T41] Perl：Hello World
来源：http://gqw.shzxlz.cn

print "Hello\n";
来源：http://iqm.sjlbkw.cn

[T42] Perl：变量类型
来源：http://luu.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ryx.wangdashe.top

[T43] Perl：字符串插值
来源：http://hjr.hnqzz.top

"值: $a"
来源：http://vql.zhixingplan.top

[T44] Perl：条件
来源：http://xzs.vehdjk.com

if ($a > 0) { print "正"; }
来源：http://kpo.uphjek.com

[T45] Perl：数组遍历
来源：http://scd.chenjidiqi.icu

for my $x (@arr) { print $x; }
来源：http://mro.fehbvm.com

[T46] Perl：哈希操作
来源：http://yom.wangshuangyany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://udq.ydzc1.top

[T47] Perl：正则捕获
来源：http://dia.chenzaomai.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://ish.hongshengwenyu.top

[T48] Perl：正则替换
来源：http://krs.zhiwuduotai.top

$s =~ s/old/new/g;
来源：http://jak.havefunace.top

[T49] Perl：函数
来源：http://ike.meibo888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nrc.ybcxt.top

[T50] Perl：逐行读文件
来源：http://lzw.tarul.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xhw.hysaishi.cn

while (my $line = <$fh>) { print $line; }
来源：http://wdk.zycfv.cn

[T51] Scala：Hello World
来源：http://qth.andypj.xyz

println("Hello")
来源：http://gkz.zdqjudy.top

[T52] Scala：变量
来源：http://yuw.guannengcc.top

val a = 1;  var b = 2
来源：http://syz.sysykeji.top

[T53] Scala：字符串插值
来源：http://qzy.sweek.top

s"值: $b"
来源：http://zhe.bjfxy.top

[T54] Scala：集合映射
来源：http://pbu.daxiang520.top

List(1, 2, 3).map(_ * 2)
来源：http://hhc.meibo888.top

[T55] Scala：集合过滤
来源：http://xyv.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://kli.nwbrower.top

[T56] Scala：样例类
来源：http://fhu.jinyuanbaomall.cn

case class User(name: String, age: Int)
来源：http://geq.hywenlv.cn

[T57] Scala：模式匹配
来源：http://kbn.snrcjt.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ifq.yangfankeji.com

[T58] Scala：函数定义
来源：http://pbr.chenzaomai.com

def add(a: Int, b: Int): Int = a + b
来源：http://owj.cheryme.top

[T59] Scala：循环
来源：http://lmr.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://xlt.zycfv.cn

[T60] Scala：折叠
来源：http://hbs.yj202588.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vlq.svipenyu.cn

================================================================================
来源：http://bij.daria6918.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://acq.uphjek.com

================================================================================
来源：http://ecl.vehdjk.com

[U01] Py：创建虚拟环境
来源：http://tkx.pengpengdd.cyou

python -m venv .venv && source .venv/bin/activate
来源：http://bod.jinghuilouyu.cn

[U02] Py：导出 / 安装依赖
来源：http://atl.aizwys.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pkv.xuanzx.com

[U03] Py：加载 .env 配置
来源：http://rgo.xuetiantiany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tqe.guannengcc.top

[U04] Py：变量调试打印
来源：http://qbg.hywenlv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ivv.chenlongwang.top

[U05] Py：列表去重且保序
来源：http://bai.sxryk.cn

list(dict.fromkeys(arr))
来源：http://wni.cashguo.top

[U06] Py：合并两个字典
来源：http://kdj.shuidangran.top

{**a, **b}
来源：http://orl.sweek.top

[U07] Py：反转字典键值
来源：http://guq.daxiang520.top

{v: k for k, v in d.items()}
来源：http://swn.daria6918.cn

[U08] Py：展平二维列表
来源：http://bot.ppjwa.cn

[y for x in nested for y in x]
来源：http://kxd.birdmap.top

[U09] Py：字典取最大值的键
来源：http://uum.zdqjudy.top

max(d, key=d.get)
来源：http://ikd.hongshengwenyu.top

[U10] Py：按值排序字典
来源：http://pvt.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cxd.mhx1999.top

[U11] Py：生成器表达式
来源：http://upg.hongshengwenyu.top

(x * 2 for x in arr)
来源：http://gxy.ywan-chungtsiang.top

[U12] Py：取出现最多的 3 个元素
来源：http://xjz.hnqzz.top

Counter(arr).most_common(3)
来源：http://nba.yj20258888.top

[U13] Py：固定长度队列
来源：http://wfp.hywenlv.cn

deque(maxlen=10)
来源：http://duv.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://kvq.dianchejie.cn

defaultdict(list)
来源：http://wmp.yueranfly.top

[U15] Py：高精度计时
来源：http://svw.ctjpmb.com

t = time.perf_counter()
来源：http://zrm.dashuyun.cn

[U16] Py：命令行参数解析
来源：http://pqz.jqgufenzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jjp.yongpay.top

[U17] Py：初始化日志
来源：http://qbo.ydzc1.top

logging.basicConfig(level=logging.INFO)
来源：http://ekz.sufxvd.cn

[U18] Py：预编译正则
来源：http://pxx.haohaochexian.top

pat = re.compile(r"\d+")
来源：http://ltc.hnxiangtu.top

[U19] Py：正则替换带回调
来源：http://wgx.yuanzhike.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pdy.yuanzhike.top

[U20] Py：缓存函数结果
来源：http://kcf.sweek.top

@functools.lru_cache(maxsize=None)
来源：http://gqf.gotoacloud.top

[U21] Py：自定义上下文管理器
来源：http://tav.zhengqikj.top

@contextlib.contextmanager
来源：http://kto.haohaochexian.top

[U22] Py：矩阵转置
来源：http://eit.quarkkingdee.top

list(zip(*m))
来源：http://wxt.xuetiantiany.cn

[U23] Py：分块读取大文件
来源：http://hqa.tarul.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://riu.yonumen.top

[U24] Py：路径操作
来源：http://ljt.aibaodan.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qmw.gzhubu.top

[U25] Py：CSV 按字典读
来源：http://rab.316326.xyz

csv.DictReader(f)
来源：http://lad.redwolf501.top

[U26] Py：并发下载
来源：http://eoj.yanxiufei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fix.zycfv.cn

[U27] Py：异步 HTTP
来源：http://prd.jinghuilouyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://bog.shzxlz.cn

[U28] Py：类型别名
来源：http://vkr.hammf.cn

UserId = int
来源：http://gbu.jiagoushi.top

[U29] Py：属性校验
来源：http://zkp.fanxiaobao.xyz

@property 与 @x.setter 配合
来源：http://xel.nanxinkj.top

[U30] Py：数据类
来源：http://hpg.daxiang520.top

@dataclass(slots=True)
来源：http://irx.fktsv.cn

[U31] Py：单测
来源：http://fax.316326.xyz

python -m pytest -q
来源：http://uof.yj20258.top

[U32] Py：代码格式化
来源：http://zbt.xuetiantiany.cn

ruff format . && ruff check --fix .
来源：http://url.sweek.top

[U33] Py：打包发布
来源：http://lqh.sxryk.cn

python -m build  （依赖 pyproject.toml）
来源：http://los.jinqigufen.top

[U34] Py：判断编码
来源：http://pjd.guowangkeji.top

chardet.detect(raw)
来源：http://ink.sweek.top

[U35] Py：发送邮件
来源：http://fjv.jlsjyb.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bhl.daria6918.cn

[U36] Py：定时任务
来源：http://ccd.svipenyu.cn

schedule.every(10).minutes.do(job)
来源：http://eta.hammf.cn

[U37] Py：读写 Excel
来源：http://fim.zhengqikj.top

pandas.read_excel / DataFrame.to_excel
来源：http://afc.sysykeji.top

[U38] Py：获取脚本所在目录
来源：http://zeb.bbcook.cn

Path(__file__).resolve().parent
来源：http://nlg.gaohongyu789.top

[U39] Py：判断是否在交互环境
来源：http://qyp.sxryk.cn

sys.stdout.isatty()
来源：http://ipe.svipenyu.cn

[U40] Py：打印到标准错误
来源：http://yuh.hammf.cn

print("err", file=sys.stderr)
来源：http://hmu.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://erk.aibaodan.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qwm.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://jtp.jlsjyb.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rzc.iojbl.cn

[U43] PHP：声明命名空间
来源：http://zxv.jinyuanbaomall.cn

namespace App\Http;
来源：http://pdb.havefunace.top

[U44] PHP：开启严格类型
来源：http://xre.yfazqb.com

declare(strict_types=1);
来源：http://zco.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://eij.pycfn.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://jts.ppjwa.cn

[U46] PHP：可空类型
来源：http://fkh.sjlbkw.cn

?string $name = null
来源：http://yto.0kj1m.cn

[U47] PHP：联合类型
来源：http://eej.nanxuanxn.top

int|string $id
来源：http://jxk.xuetiantiany.cn

[U48] PHP：纯枚举
来源：http://mew.vqdsnc.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pev.yongpay.top

[U49] PHP：只读属性
来源：http://vba.cqqwz.cn

public readonly string $name
来源：http://jde.316326.xyz

[U50] PHP：构造器属性提升
来源：http://iwk.quarkkingdee.top

public function __construct(private int $id) {}
来源：http://yjj.cashguo.top

[U51] PHP：数组解构
来源：http://ydw.fanxiaobao.xyz

[$a, $b] = $arr;
来源：http://ncn.guowangkeji.top

[U52] PHP：箭头函数
来源：http://wuv.uphjek.com

$double = fn($x) => $x * 2;
来源：http://rll.chenzaomai.com

[U53] PHP：空合并运算符
来源：http://nxe.sysykeji.top

$v = $a ?? $b ?? "default";
来源：http://jkx.zhijiandao.cn

[U54] PHP：空安全调用
来源：http://caf.sysykeji.top

$obj?->method()
来源：http://vzy.feifeiyinyue.top

[U55] PHP：match 表达式
来源：http://zpk.hnxiangtu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pkw.wangshuangyany.cn

[U56] PHP：命名参数
来源：http://nax.fzhhl.top

f(a: 1, b: 2)
来源：http://mqc.hnqzz.top

[U57] PHP：字符串插值
来源：http://aqo.andypj.xyz

"值: {$a}"
来源：http://rin.shzxlz.cn

[U58] PHP：数组三件套
来源：http://hzj.kuanghao11.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rje.hywenlv.cn

[U59] PHP：自定义排序
来源：http://qwn.jinghuilouyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hcm.birdmap.top

[U60] PHP：JSON 编解码
来源：http://dyt.xziqi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ssf.gotoacloud.top

[U61] PHP：正则
来源：http://qub.zhixingplan.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tcq.yj20258.top

[U62] PHP：日期对象
来源：http://gzk.wangshuangyany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aib.hysaishi.cn

[U63] PHP：文件读写
来源：http://jlt.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pkr.jlsjyb.cn

[U64] PHP：目录遍历
来源：http://spw.sufxvd.cn

glob("dir/*.php");  scandir("dir");
来源：http://sek.jinqigufen.top

[U65] PHP：会话
来源：http://fqx.52xcode.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wex.zhixingplan.top

[U66] PHP：设置 Cookie
来源：http://tvp.nwbrower.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nsp.316326.xyz

[U67] PHP：处理文件上传
来源：http://hwb.havefunace.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wlc.zycfv.cn

[U68] PHP：PDO 连接
来源：http://atj.zhijiandao.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fgd.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://spi.sufxvd.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vut.jinyuanbaomall.cn

[U70] PHP：PDO 事务
来源：http://bxi.nanxuanxn.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vzh.sufxvd.cn

[U71] PHP：抛出异常
来源：http://nym.xingfuxueyuan.xyz

throw new RuntimeException("失败", 500);
来源：http://rhh.xuanzx.com

[U72] PHP：写错误日志
来源：http://ans.shanyushiyangtech.top

error_log("失败: " . $e->getMessage());
来源：http://pyo.52xcode.cn

[U73] PHP：读取 ini 配置
来源：http://zqu.fehbvm.com

parse_ini_file("config.ini", true)
来源：http://bks.jyoumei.cn

[U74] PHP：读取环境变量
来源：http://gpl.yanxiufei.cn

getenv("APP_ENV") ?: "production"
来源：http://cui.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://dlo.zhiwuduotai.top

composer require psr/container
来源：http://vbf.jinghuilouyu.cn

[U76] PHP：简单路由
来源：http://zur.xziqi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gnf.epnwcf.com

[U77] PHP：模板渲染
来源：http://rxq.ppjwa.cn

composer require twig/twig
来源：http://ekc.feifeiyinyue.top

[U78] PHP：单元测试
来源：http://pkn.vehdjk.com

composer require --dev phpunit/phpunit
来源：http://jcu.jinqigufen.top

[U79] PHP：静态分析
来源：http://ydl.xinyue.icu

composer require --dev phpstan/phpstan
来源：http://tbo.jianghu66.top

[U80] PHP：代码规范修复
来源：http://nsi.wangdashe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://smi.iojbl.cn

[U81] JS：初始化项目
来源：http://ftz.daxiang520.top

npm init -y;  npm i express
来源：http://tkl.xylfe.cn

[U82] JS：package.json 脚本
来源：http://qjj.yanxiufei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://its.guowangkeji.top

[U83] JS：ES Module 导入导出
来源：http://idm.uphjek.com

export const a = 1;  import { a } from "./m.js";
来源：http://tdk.ydzc1.top

[U84] JS：CommonJS 写法
来源：http://cba.hysaishi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qbg.pycfn.com

[U85] JS：可选链
来源：http://oee.daxiang520.top

a?.b?.c
来源：http://bxu.shanyushiyangtech.top

[U86] JS：空值合并
来源：http://ftc.daria6918.cn

a ?? b
来源：http://jyo.mhx1999.top

[U87] JS：解构默认值
来源：http://zol.yueranfly.top

const { a = 1, b = 2 } = obj;
来源：http://eri.xziqi.cn

[U88] JS：对象展开合并
来源：http://pxw.yj20258888.top

{ ...a, ...b }
来源：http://zjv.pengpengdd.cyou

[U89] JS：数组去重
来源：http://afz.xylfe.cn

[...new Set(arr)]
来源：http://xem.cqqwz.cn

[U90] JS：数字数组排序
来源：http://sbp.iojbl.cn

[...arr].sort((a, b) => a - b)
来源：http://ohh.ppjwa.cn

[U91] JS：对象键值遍历
来源：http://iwq.hysaishi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mnd.sysykeji.top

[U92] JS：深拷贝
来源：http://xbx.zdbjq.cn

structuredClone(obj)
来源：http://cgq.jianghu66.top

[U93] JS：模板字符串
来源：http://dpy.jinghuilouyu.cn

`共 ${n} 条`
来源：http://doa.hnxiangtu.top

[U94] JS：箭头函数
来源：http://ncr.kuanghao11.cn

const double = x => x * 2;
来源：http://lny.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://ihz.gaohongyu789.top

new Promise((resolve, reject) => {})
来源：http://pcv.ydzc1.top

[U96] JS：async/await 与异常
来源：http://smo.dianchejie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pzy.svipenyu.cn

[U97] JS：并发请求
来源：http://csl.ppjwa.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://omc.sweek.top

[U98] JS：fetch 带 JSON
来源：http://xkc.ydzc1.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hxb.316326.xyz

[U99] JS：事件监听
来源：http://xpt.yj20258.top

el.addEventListener("click", e => {})
来源：http://tpc.jiagoushi.top

[U100] JS：DOM 查询
来源：http://yjk.cashguo.top

document.querySelector(".item")
来源：http://chj.jianghu66.top

[U101] JS：classList 操作
来源：http://vgg.dashuyun.cn

el.classList.toggle("active")
来源：http://rfx.tarul.cn

[U102] JS：本地存储
来源：http://mzx.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://lwn.yj202588.top

[U103] JS：定时器
来源：http://nxp.jinghuilouyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://clr.iojbl.cn

[U104] JS：防抖
来源：http://vjn.epnwcf.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rok.ivvv.top

[U105] JS：节流
来源：http://dwr.dashuyun.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://esr.tarul.cn

[U106] JS：日期格式化
来源：http://hkk.zhiwuduotai.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ken.chenlongwang.top

[U107] JS：数字千分位
来源：http://mct.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sgr.pengpengdd.cyou

[U108] JS：随机整数
来源：http://woe.iojbl.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://spr.quarkkingdee.top

[U109] JS：数组分组
来源：http://vxv.nanxinkj.top

Object.groupBy(arr, x => x.type)
来源：http://poc.sysykeji.top

[U110] JS：数组分块
来源：http://ifb.hnqzz.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://brx.cheryme.top

[U111] JS：对象转 Map
来源：http://llq.yuanzhike.top

new Map(Object.entries(obj))
来源：http://jvb.chenjidiqi.icu

[U112] JS：字符串补位
来源：http://rdq.pycfn.com

"7".padStart(3, "0")
来源：http://zlg.tian-w.cn

[U113] JS：正则替换全部
来源：http://rou.shzxlz.cn

s.replaceAll("a", "b")
来源：http://als.gotoacloud.top

[U114] JS：JSON 深比较
来源：http://lez.jqgfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pyn.shangyingyoupin.top

[U115] JS：生成 UUID
来源：http://oul.9152youxi.cn

crypto.randomUUID()
来源：http://xeo.daxiang520.top

[U116] JS：类型检查（JSDoc）
来源：http://obd.vqdsnc.cn

/** @param {string} name */ function f(name) {}
来源：http://nrr.dianchejie.cn

[U117] JS：单元测试
来源：http://sqb.yonumen.top

npm i -D vitest;  npx vitest
来源：http://ojv.gaohongyu789.top

[U118] JS：开发服务器
来源：http://pum.fengsongda.top

npm i -D vite;  npx vite
来源：http://trw.andypj.xyz

[U119] JS：生产构建
来源：http://ayo.sxryk.cn

npx vite build
来源：http://zlw.jqgufenzy.top

[U120] JS：读取环境变量（Vite）
来源：http://ltf.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://nxz.zhaomingkeji.xyz

================================================================================
来源：http://pen.wangdashe.top

统计汇总
来源：http://sel.wangshuangyany.cn

================================================================================
来源：http://jnt.zycfv.cn

按语言统计（条）：
来源：http://yjh.fehbvm.com

Python ......... 252
来源：http://pqs.jlsjyb.cn

PHP ............ 252
来源：http://itj.zhixingplan.top

JavaScript ..... 252
来源：http://ymz.pengpengdd.cyou

TypeScript ..... 212
来源：http://szu.uphjek.com


<!-- 参考信息 -->