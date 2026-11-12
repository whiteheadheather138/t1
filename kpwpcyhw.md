代发 wailian999

[T39] Lua：模式匹配
来源：http://jdf.shzxlz.cn

string.find(s, "%d+")
来源：http://efl.sxryk.cn

[T40] Lua：元表
来源：http://wtb.jiagoushi.top

setmetatable({}, { __index = base })
来源：http://fpc.hysaishi.cn

[T41] Perl：Hello World
来源：http://vaj.tanke756.top

print "Hello\n";
来源：http://lpu.ehwqpu.com

[T42] Perl：变量类型
来源：http://tfv.kuanghao11.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pzz.yanxiufei.cn

[T43] Perl：字符串插值
来源：http://ejg.birdmap.top

"值: $a"
来源：http://iks.bjfxy.top

[T44] Perl：条件
来源：http://ews.fktsv.cn

if ($a > 0) { print "正"; }
来源：http://kzf.jlsjyb.cn

[T45] Perl：数组遍历
来源：http://jrw.tarul.cn

for my $x (@arr) { print $x; }
来源：http://pqe.zhengqikj.top

[T46] Perl：哈希操作
来源：http://yyt.xuetiantiany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cwu.yj20258888.top

[T47] Perl：正则捕获
来源：http://nrn.jinyuanbaomall.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://djy.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://dzx.zhoulong.xyz

$s =~ s/old/new/g;
来源：http://gvk.ehwqpu.com

[T49] Perl：函数
来源：http://tsh.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xhj.pycfn.com

[T50] Perl：逐行读文件
来源：http://mjg.tarul.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ogv.zdbjq.cn

while (my $line = <$fh>) { print $line; }
来源：http://vnp.snrcjt.cn

[T51] Scala：Hello World
来源：http://xtc.fktsv.cn

println("Hello")
来源：http://aim.zdqjudy.top

[T52] Scala：变量
来源：http://fch.52xcode.cn

val a = 1;  var b = 2
来源：http://nbx.cheryme.top

[T53] Scala：字符串插值
来源：http://jrc.hcnkem.com

s"值: $b"
来源：http://ugp.xylfe.cn

[T54] Scala：集合映射
来源：http://crt.yongpay.top

List(1, 2, 3).map(_ * 2)
来源：http://hch.epnwcf.com

[T55] Scala：集合过滤
来源：http://xaa.ybcxt.top

List(1, 2, 3).filter(_ > 1)
来源：http://kwl.hfpthk.cn

[T56] Scala：样例类
来源：http://nfb.cdnleiting.top

case class User(name: String, age: Int)
来源：http://ybx.tian-w.cn

[T57] Scala：模式匹配
来源：http://ilc.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wkz.shanyushiyangkeji.top

[T58] Scala：函数定义
来源：http://min.sweek.top

def add(a: Int, b: Int): Int = a + b
来源：http://tjp.tianlin.xyz

[T59] Scala：循环
来源：http://env.zhijiandao.cn

for (i <- 1 to 10) println(i)
来源：http://aed.gotoacloud.top

[T60] Scala：折叠
来源：http://mdy.tianlin.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cah.jinqigfzy.top

================================================================================
来源：http://yat.hnqzz.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xtl.smart0.xyz

================================================================================
来源：http://dnf.jiagoushi.top

[U01] Py：创建虚拟环境
来源：http://gxl.havefunace.top

python -m venv .venv && source .venv/bin/activate
来源：http://cui.chenlongwang.top

[U02] Py：导出 / 安装依赖
来源：http://rqn.cqqwz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fyp.cashguo.top

[U03] Py：加载 .env 配置
来源：http://yay.wangshuangyany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nfg.aibaodan.cn

[U04] Py：变量调试打印
来源：http://qmg.yfazqb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wmf.dianchejie.cn

[U05] Py：列表去重且保序
来源：http://smp.quarkkingdee.top

list(dict.fromkeys(arr))
来源：http://pun.yongpay.top

[U06] Py：合并两个字典
来源：http://eke.yj202588.top

{**a, **b}
来源：http://egj.xinyue.icu

[U07] Py：反转字典键值
来源：http://fba.shanyushiyangtech.top

{v: k for k, v in d.items()}
来源：http://uif.chenlongwang.top

[U08] Py：展平二维列表
来源：http://kbp.9152youxi.cn

[y for x in nested for y in x]
来源：http://hjy.mhx1999.top

[U09] Py：字典取最大值的键
来源：http://qbw.dashuyun.cn

max(d, key=d.get)
来源：http://fdw.0kj1m.cn

[U10] Py：按值排序字典
来源：http://vnm.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xem.chenjidiqi.icu

[U11] Py：生成器表达式
来源：http://pbr.ehwqpu.com

(x * 2 for x in arr)
来源：http://wra.wangshuangyany.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jui.tanke756.top

Counter(arr).most_common(3)
来源：http://vks.xziqi.cn

[U13] Py：固定长度队列
来源：http://tbu.dianchejie.cn

deque(maxlen=10)
来源：http://srj.tian-w.cn

[U14] Py：分组收集到列表
来源：http://hqp.316326.xyz

defaultdict(list)
来源：http://xpl.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://tpt.zycfv.cn

t = time.perf_counter()
来源：http://kxc.jqgfzy.top

[U16] Py：命令行参数解析
来源：http://kqw.fzhhl.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://juj.ydzc1.top

[U17] Py：初始化日志
来源：http://ila.xziqi.cn

logging.basicConfig(level=logging.INFO)
来源：http://jjn.jqgfzy.top

[U18] Py：预编译正则
来源：http://ejv.epnwcf.com

pat = re.compile(r"\d+")
来源：http://gvl.jiagoushi.top

[U19] Py：正则替换带回调
来源：http://bdt.zycfv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rue.sxryk.cn

[U20] Py：缓存函数结果
来源：http://fyj.smart0.xyz

@functools.lru_cache(maxsize=None)
来源：http://clx.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://lcg.snrcjt.cn

@contextlib.contextmanager
来源：http://ecr.cucudq.cn

[U22] Py：矩阵转置
来源：http://bhf.yuxming.cn

list(zip(*m))
来源：http://slw.bjfxy.top

[U23] Py：分块读取大文件
来源：http://zjo.ppjwa.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fkp.cucudq.cn

[U24] Py：路径操作
来源：http://qtj.ywan-chungtsiang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://der.nanxuanxn.top

[U25] Py：CSV 按字典读
来源：http://iyd.hywenlv.cn

csv.DictReader(f)
来源：http://kel.316326.xyz

[U26] Py：并发下载
来源：http://fyn.pengpengdd.cyou

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yjf.hysaishi.cn

[U27] Py：异步 HTTP
来源：http://ekr.shanyushiyangtech.top

aiohttp.ClientSession() 配合 async with
来源：http://etu.cashguo.top

[U28] Py：类型别名
来源：http://raj.316326.xyz

UserId = int
来源：http://ofv.sweek.top

[U29] Py：属性校验
来源：http://wkr.shangyingyoupin.top

@property 与 @x.setter 配合
来源：http://wtt.nanxinkj.top

[U30] Py：数据类
来源：http://uve.cdnleiting.top

@dataclass(slots=True)
来源：http://vug.jlsjyb.cn

[U31] Py：单测
来源：http://fvi.wangdashe.top

python -m pytest -q
来源：http://moo.52xcode.cn

[U32] Py：代码格式化
来源：http://sjq.xuetiantiany.cn

ruff format . && ruff check --fix .
来源：http://vzz.316326.xyz

[U33] Py：打包发布
来源：http://obc.shzxlz.cn

python -m build  （依赖 pyproject.toml）
来源：http://gtp.nanxuanxn.top

[U34] Py：判断编码
来源：http://pnl.cqqwz.cn

chardet.detect(raw)
来源：http://lsk.sysykeji.top

[U35] Py：发送邮件
来源：http://kuk.guowangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://trw.quarkkingdee.top

[U36] Py：定时任务
来源：http://cdl.shanyushiyangtech.top

schedule.every(10).minutes.do(job)
来源：http://idb.sweek.top

[U37] Py：读写 Excel
来源：http://xxt.nanxinkj.top

pandas.read_excel / DataFrame.to_excel
来源：http://pic.hfpthk.cn

[U38] Py：获取脚本所在目录
来源：http://eok.zhijiandao.cn

Path(__file__).resolve().parent
来源：http://nob.nwbrower.top

[U39] Py：判断是否在交互环境
来源：http://myu.guannengcc.top

sys.stdout.isatty()
来源：http://nyr.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://iti.yj20258.top

print("err", file=sys.stderr)
来源：http://xew.jlsjyb.cn

[U41] PHP：初始化 Composer 项目
来源：http://aib.316326.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://ixo.wangshuangyany.cn

[U42] PHP：PSR-4 自动加载
来源：http://khj.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lai.hnqzz.top

[U43] PHP：声明命名空间
来源：http://ifi.hnqzz.top

namespace App\Http;
来源：http://sxh.mhx1999.top

[U44] PHP：开启严格类型
来源：http://wsy.pycfn.com

declare(strict_types=1);
来源：http://dqw.hammf.cn

[U45] PHP：类型声明与返回类型
来源：http://wsw.guannengcc.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://uzw.sweek.top

[U46] PHP：可空类型
来源：http://exi.xuetiantiany.cn

?string $name = null
来源：http://aht.redwolf501.top

[U47] PHP：联合类型
来源：http://tco.daxiang520.top

int|string $id
来源：http://yrt.jqgfzy.top

[U48] PHP：纯枚举
来源：http://rju.hammf.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lsv.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://gfj.fehbvm.com

public readonly string $name
来源：http://fqj.meibo888.top

[U50] PHP：构造器属性提升
来源：http://njy.shuidangran.top

public function __construct(private int $id) {}
来源：http://nlw.iojbl.cn

[U51] PHP：数组解构
来源：http://ooo.hnqzz.top

[$a, $b] = $arr;
来源：http://oud.guannengcc.top

[U52] PHP：箭头函数
来源：http://hzm.yj202588.top

$double = fn($x) => $x * 2;
来源：http://cfy.fengsongda.top

[U53] PHP：空合并运算符
来源：http://ofr.jinqigfzy.top

$v = $a ?? $b ?? "default";
来源：http://the.chenlongwang.top

[U54] PHP：空安全调用
来源：http://bua.zdbjq.cn

$obj?->method()
来源：http://ujz.sjlbkw.cn

[U55] PHP：match 表达式
来源：http://zdj.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cbj.cashguo.top

[U56] PHP：命名参数
来源：http://awp.chenlongwang.top

f(a: 1, b: 2)
来源：http://bhf.vehdjk.com

[U57] PHP：字符串插值
来源：http://poe.shanyushiyangkeji.top

"值: {$a}"
来源：http://mjc.kuanghao11.cn

[U58] PHP：数组三件套
来源：http://vuo.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qvp.0kj1m.cn

[U59] PHP：自定义排序
来源：http://qpm.c1oappe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kaj.yonumen.top

[U60] PHP：JSON 编解码
来源：http://dkp.jqgufenzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xpd.sysykeji.top

[U61] PHP：正则
来源：http://bis.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tyx.tanke756.top

[U62] PHP：日期对象
来源：http://lat.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://huo.ydjk.org.cn

[U63] PHP：文件读写
来源：http://mvr.nanxinkj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kpq.tarul.cn

[U64] PHP：目录遍历
来源：http://uta.chenjidiqi.icu

glob("dir/*.php");  scandir("dir");
来源：http://jul.chenjidiqi.icu

[U65] PHP：会话
来源：http://rxl.ctjpmb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://fnx.gaohongyu789.top

[U66] PHP：设置 Cookie
来源：http://ifi.dianchejie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zig.hammf.cn

[U67] PHP：处理文件上传
来源：http://vhw.jinqigufen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ojs.jinghuilouyu.cn

[U68] PHP：PDO 连接
来源：http://jab.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kqf.jyoumei.cn

[U69] PHP：PDO 预处理
来源：http://izz.jinghuilouyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zoi.bbcook.cn

[U70] PHP：PDO 事务
来源：http://ecz.sxryk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mms.zycfv.cn

[U71] PHP：抛出异常
来源：http://ghu.feifeiyinyue.top

throw new RuntimeException("失败", 500);
来源：http://lxa.gogol.net.cn

[U72] PHP：写错误日志
来源：http://ese.zhiwuduotai.top

error_log("失败: " . $e->getMessage());
来源：http://kxz.chenjidiqi.icu

[U73] PHP：读取 ini 配置
来源：http://oqa.bbcook.cn

parse_ini_file("config.ini", true)
来源：http://seq.pycfn.com

[U74] PHP：读取环境变量
来源：http://yrh.andypj.xyz

getenv("APP_ENV") ?: "production"
来源：http://sjg.jinyuanbaomall.cn

[U75] PHP：依赖注入
来源：http://dbb.jlsjyb.cn

composer require psr/container
来源：http://lxf.zhijiandao.cn

[U76] PHP：简单路由
来源：http://qli.zhoulong.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qfm.meibo888.top

[U77] PHP：模板渲染
来源：http://uyi.fengsongda.top

composer require twig/twig
来源：http://wwc.sufxvd.cn

[U78] PHP：单元测试
来源：http://btq.sysykeji.top

composer require --dev phpunit/phpunit
来源：http://afg.yongpay.top

[U79] PHP：静态分析
来源：http://hws.ehwqpu.com

composer require --dev phpstan/phpstan
来源：http://yoc.bjfxy.top

[U80] PHP：代码规范修复
来源：http://riv.hfpthk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ufa.yvedp.cn

[U81] JS：初始化项目
来源：http://qwe.yj20258.top

npm init -y;  npm i express
来源：http://yya.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://hsp.xuanzx.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vff.aibaodan.cn

[U83] JS：ES Module 导入导出
来源：http://kid.gzhubu.top

export const a = 1;  import { a } from "./m.js";
来源：http://sga.vqdsnc.cn

[U84] JS：CommonJS 写法
来源：http://isw.ctjpmb.com

module.exports = { a };  const { a } = require("./m");
来源：http://paw.epnwcf.com

[U85] JS：可选链
来源：http://fmg.quarkkingdee.top

a?.b?.c
来源：http://brr.nanxinkj.top

[U86] JS：空值合并
来源：http://ubw.zhongyouzk.top

a ?? b
来源：http://ufa.vqdsnc.cn

[U87] JS：解构默认值
来源：http://ezw.tanke756.top

const { a = 1, b = 2 } = obj;
来源：http://ygw.xuanzx.com

[U88] JS：对象展开合并
来源：http://kvf.jyoumei.cn

{ ...a, ...b }
来源：http://yxk.chenlongwang.top

[U89] JS：数组去重
来源：http://kyx.sxryk.cn

[...new Set(arr)]
来源：http://vfd.yonumen.top

[U90] JS：数字数组排序
来源：http://urk.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://wtp.guowangkeji.top

[U91] JS：对象键值遍历
来源：http://onh.xziqi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xwj.jlsjyb.cn

[U92] JS：深拷贝
来源：http://krc.ivvv.top

structuredClone(obj)
来源：http://gbi.cheryme.top

[U93] JS：模板字符串
来源：http://lxs.pycfn.com

`共 ${n} 条`
来源：http://xhx.ehwqpu.com

[U94] JS：箭头函数
来源：http://sfl.yvedp.cn

const double = x => x * 2;
来源：http://wwv.cashguo.top

[U95] JS：Promise 包装
来源：http://ync.zhongyouzk.top

new Promise((resolve, reject) => {})
来源：http://eaq.zhijiandao.cn

[U96] JS：async/await 与异常
来源：http://tlx.epnwcf.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gew.zhaomingkeji.xyz

[U97] JS：并发请求
来源：http://two.hammf.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zlv.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://www.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zux.pycfn.com

[U99] JS：事件监听
来源：http://zdk.zdbjq.cn

el.addEventListener("click", e => {})
来源：http://hgm.chenzaomai.com

[U100] JS：DOM 查询
来源：http://bra.yongpay.top

document.querySelector(".item")
来源：http://hvq.hongshengwenyu.top

[U101] JS：classList 操作
来源：http://bch.jianghu66.top

el.classList.toggle("active")
来源：http://cxe.yj20258888.top

[U102] JS：本地存储
来源：http://rtu.uphjek.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://rlr.havefunace.top

[U103] JS：定时器
来源：http://tkl.9152youxi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zcc.gaohongyu789.top

[U104] JS：防抖
来源：http://bmd.daria6918.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nuj.jinghuilouyu.cn

[U105] JS：节流
来源：http://ceq.zdqjudy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://boj.ydjk.org.cn

[U106] JS：日期格式化
来源：http://zih.aibaodan.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bus.shzxlz.cn

[U107] JS：数字千分位
来源：http://uck.sweek.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nrb.yuxming.cn

[U108] JS：随机整数
来源：http://ofe.shanyushiyangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gnl.vqdsnc.cn

[U109] JS：数组分组
来源：http://mlv.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://zvb.shangyingyoupin.top

[U110] JS：数组分块
来源：http://znm.yj20258.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xyt.9152youxi.cn

[U111] JS：对象转 Map
来源：http://xjt.nanxinkj.top

new Map(Object.entries(obj))
来源：http://pbq.hongshengwenyu.top

[U112] JS：字符串补位
来源：http://pbr.ctjpmb.com

"7".padStart(3, "0")
来源：http://iyg.ywan-chungtsiang.top

[U113] JS：正则替换全部
来源：http://hbz.aizwys.cn

s.replaceAll("a", "b")
来源：http://qgv.ehwqpu.com

[U114] JS：JSON 深比较
来源：http://ghp.52xcode.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zvi.cashguo.top

[U115] JS：生成 UUID
来源：http://rpp.wangshuangyany.cn

crypto.randomUUID()
来源：http://lik.fktsv.cn

[U116] JS：类型检查（JSDoc）
来源：http://dnl.cheryme.top

/** @param {string} name */ function f(name) {}
来源：http://zqh.daria6918.cn

[U117] JS：单元测试
来源：http://jzf.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://jvs.yvedp.cn

[U118] JS：开发服务器
来源：http://ewz.bbcook.cn

npm i -D vite;  npx vite
来源：http://esp.yueranfly.top

[U119] JS：生产构建
来源：http://aaa.yueranfly.top

npx vite build
来源：http://tlu.meibo888.top

[U120] JS：读取环境变量（Vite）
来源：http://ypn.jinghuilouyu.cn

import.meta.env.VITE_API_URL
来源：http://oug.daxiang520.top

================================================================================
来源：http://jja.yfazqb.com

统计汇总
来源：http://yay.gogol.net.cn

================================================================================
来源：http://enr.316326.xyz

按语言统计（条）：
来源：http://upb.ppjwa.cn

Python ......... 252
来源：http://fmx.hammf.cn

PHP ............ 252
来源：http://ojt.cucudq.cn

JavaScript ..... 252
来源：http://bti.tanke756.top

TypeScript ..... 212
来源：http://lnh.yonumen.top

Java ........... 212
来源：http://rlx.ydzc1.top

Go ............. 212
来源：http://fqj.yuanzhike.top

Ruby ........... 212
来源：http://ftk.shuidangran.top

C# ............. 212
来源：http://ead.dianchejie.cn


<!-- 参考信息 -->