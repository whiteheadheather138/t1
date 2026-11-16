代发 wailian999

[T39] Lua：模式匹配
来源：http://jfn.hywenlv.cn

string.find(s, "%d+")
来源：http://mbx.ywan-chungtsiang.top

[T40] Lua：元表
来源：http://ddi.yvedp.cn

setmetatable({}, { __index = base })
来源：http://kqt.yfazqb.com

[T41] Perl：Hello World
来源：http://ypm.zhengqikj.top

print "Hello\n";
来源：http://cvy.yongpay.top

[T42] Perl：变量类型
来源：http://rlx.yuxming.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mir.xinyue.icu

[T43] Perl：字符串插值
来源：http://vkd.birdmap.top

"值: $a"
来源：http://kxa.fzhhl.top

[T44] Perl：条件
来源：http://pub.smart0.xyz

if ($a > 0) { print "正"; }
来源：http://oqr.dianchejie.cn

[T45] Perl：数组遍历
来源：http://owf.hammf.cn

for my $x (@arr) { print $x; }
来源：http://fvt.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://nmh.zhaomingkeji.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hzb.yueranfly.top

[T47] Perl：正则捕获
来源：http://lea.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xpe.yfazqb.com

[T48] Perl：正则替换
来源：http://lpl.fanxiaobao.xyz

$s =~ s/old/new/g;
来源：http://vmb.jianghu66.top

[T49] Perl：函数
来源：http://fzz.chenzaomai.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kdz.sweek.top

[T50] Perl：逐行读文件
来源：http://tkx.shuidangran.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pcp.sjlbkw.cn

while (my $line = <$fh>) { print $line; }
来源：http://wfp.snrcjt.cn

[T51] Scala：Hello World
来源：http://aub.tian-w.cn

println("Hello")
来源：http://jqv.hammf.cn

[T52] Scala：变量
来源：http://fwc.mhx1999.top

val a = 1;  var b = 2
来源：http://lnr.yueranfly.top

[T53] Scala：字符串插值
来源：http://cyr.jinqigfzy.top

s"值: $b"
来源：http://ric.fktsv.cn

[T54] Scala：集合映射
来源：http://dea.zhaomingkeji.xyz

List(1, 2, 3).map(_ * 2)
来源：http://ajj.yj202588.top

[T55] Scala：集合过滤
来源：http://eni.nwbrower.top

List(1, 2, 3).filter(_ > 1)
来源：http://ehc.yangfankeji.com

[T56] Scala：样例类
来源：http://vnj.jlsjyb.cn

case class User(name: String, age: Int)
来源：http://cwh.gotoacloud.top

[T57] Scala：模式匹配
来源：http://trx.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mxk.jqgufenzy.top

[T58] Scala：函数定义
来源：http://mnq.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://syb.nwbrower.top

[T59] Scala：循环
来源：http://vzy.fanxiaobao.xyz

for (i <- 1 to 10) println(i)
来源：http://syb.sysykeji.top

[T60] Scala：折叠
来源：http://ppe.yuxming.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://agz.jyoumei.cn

================================================================================
来源：http://uhc.shzxlz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qhb.zdqjudy.top

================================================================================
来源：http://awy.jiagoushi.top

[U01] Py：创建虚拟环境
来源：http://qun.meibo888.top

python -m venv .venv && source .venv/bin/activate
来源：http://qwr.hcnkem.com

[U02] Py：导出 / 安装依赖
来源：http://bya.hcnkem.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rkj.yangfankeji.com

[U03] Py：加载 .env 配置
来源：http://xwb.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://yhj.zhijiandao.cn

[U04] Py：变量调试打印
来源：http://myv.hongshengwenyu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xes.hnxiangtu.top

[U05] Py：列表去重且保序
来源：http://qdj.cucudq.cn

list(dict.fromkeys(arr))
来源：http://lpc.guannengcc.top

[U06] Py：合并两个字典
来源：http://les.tianlin.xyz

{**a, **b}
来源：http://wbu.yj20258888.top

[U07] Py：反转字典键值
来源：http://riz.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://ffg.xuetiantiany.cn

[U08] Py：展平二维列表
来源：http://rrq.jiagoushi.top

[y for x in nested for y in x]
来源：http://ieb.cucudq.cn

[U09] Py：字典取最大值的键
来源：http://bvr.sjlbkw.cn

max(d, key=d.get)
来源：http://vsj.mhx1999.top

[U10] Py：按值排序字典
来源：http://clc.c1oappe.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cqq.sweek.top

[U11] Py：生成器表达式
来源：http://qfc.zhongyouzk.top

(x * 2 for x in arr)
来源：http://eqx.mhx1999.top

[U12] Py：取出现最多的 3 个元素
来源：http://muq.316326.xyz

Counter(arr).most_common(3)
来源：http://spq.meibo888.top

[U13] Py：固定长度队列
来源：http://wvi.zhaomingkeji.xyz

deque(maxlen=10)
来源：http://blf.zdbjq.cn

[U14] Py：分组收集到列表
来源：http://ott.zdbjq.cn

defaultdict(list)
来源：http://cmp.yvedp.cn

[U15] Py：高精度计时
来源：http://orv.meibo888.top

t = time.perf_counter()
来源：http://exz.0kj1m.cn

[U16] Py：命令行参数解析
来源：http://dhy.nanxinkj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cst.nwbrower.top

[U17] Py：初始化日志
来源：http://aqa.ydjk.org.cn

logging.basicConfig(level=logging.INFO)
来源：http://llb.tarul.cn

[U18] Py：预编译正则
来源：http://ypz.cdnleiting.top

pat = re.compile(r"\d+")
来源：http://hze.fktsv.cn

[U19] Py：正则替换带回调
来源：http://gia.aibaodan.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zbf.yj20258.top

[U20] Py：缓存函数结果
来源：http://ddf.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://ikf.yonumen.top

[U21] Py：自定义上下文管理器
来源：http://fsl.tarul.cn

@contextlib.contextmanager
来源：http://sgv.chenzaomai.com

[U22] Py：矩阵转置
来源：http://pjn.mhx1999.top

list(zip(*m))
来源：http://yyn.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://mie.hywenlv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nqs.zhoulong.xyz

[U24] Py：路径操作
来源：http://egf.hywenlv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nwg.hysaishi.cn

[U25] Py：CSV 按字典读
来源：http://foa.pycfn.com

csv.DictReader(f)
来源：http://dmb.zdqjudy.top

[U26] Py：并发下载
来源：http://kgv.zhengqikj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pau.wangshuangyany.cn

[U27] Py：异步 HTTP
来源：http://gjm.fktsv.cn

aiohttp.ClientSession() 配合 async with
来源：http://bvo.bjfxy.top

[U28] Py：类型别名
来源：http://oky.ydzc1.top

UserId = int
来源：http://jxm.fzhhl.top

[U29] Py：属性校验
来源：http://rgo.snrcjt.cn

@property 与 @x.setter 配合
来源：http://zsh.yongpay.top

[U30] Py：数据类
来源：http://laa.xziqi.cn

@dataclass(slots=True)
来源：http://vmq.feifeiyinyue.top

[U31] Py：单测
来源：http://euj.vehdjk.com

python -m pytest -q
来源：http://bjt.yj20258888.top

[U32] Py：代码格式化
来源：http://knk.mhx1999.top

ruff format . && ruff check --fix .
来源：http://xcq.ywan-chungtsiang.top

[U33] Py：打包发布
来源：http://vgu.yongpay.top

python -m build  （依赖 pyproject.toml）
来源：http://ilh.hongshengwenyu.top

[U34] Py：判断编码
来源：http://onb.yanxiufei.cn

chardet.detect(raw)
来源：http://sps.fktsv.cn

[U35] Py：发送邮件
来源：http://dsg.tianlin.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iyh.ivvv.top

[U36] Py：定时任务
来源：http://qbu.jqgfzy.top

schedule.every(10).minutes.do(job)
来源：http://mul.ehwqpu.com

[U37] Py：读写 Excel
来源：http://itk.cheryme.top

pandas.read_excel / DataFrame.to_excel
来源：http://eri.nanxuanxn.top

[U38] Py：获取脚本所在目录
来源：http://rbp.xziqi.cn

Path(__file__).resolve().parent
来源：http://ovf.smart0.xyz

[U39] Py：判断是否在交互环境
来源：http://pjf.vehdjk.com

sys.stdout.isatty()
来源：http://kqk.ehwqpu.com

[U40] Py：打印到标准错误
来源：http://cpb.daxiang520.top

print("err", file=sys.stderr)
来源：http://yqg.shuidangran.top

[U41] PHP：初始化 Composer 项目
来源：http://lkg.andypj.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://ior.vqdsnc.cn

[U42] PHP：PSR-4 自动加载
来源：http://qhn.yongpay.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ddc.yuanzhike.top

[U43] PHP：声明命名空间
来源：http://ncq.ppjwa.cn

namespace App\Http;
来源：http://hxm.uphjek.com

[U44] PHP：开启严格类型
来源：http://vmr.aibaodan.cn

declare(strict_types=1);
来源：http://gop.ehwqpu.com

[U45] PHP：类型声明与返回类型
来源：http://pfd.andypj.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://eeh.guowangkeji.top

[U46] PHP：可空类型
来源：http://wxu.hnxiangtu.top

?string $name = null
来源：http://qfs.uphjek.com

[U47] PHP：联合类型
来源：http://evq.bjfxy.top

int|string $id
来源：http://tlt.yj20258.top

[U48] PHP：纯枚举
来源：http://pls.dianchejie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uhc.pycfn.com

[U49] PHP：只读属性
来源：http://xol.yfazqb.com

public readonly string $name
来源：http://nmf.sxryk.cn

[U50] PHP：构造器属性提升
来源：http://akp.316326.xyz

public function __construct(private int $id) {}
来源：http://iig.aibaodan.cn

[U51] PHP：数组解构
来源：http://vgw.jianghu66.top

[$a, $b] = $arr;
来源：http://fkf.nwbrower.top

[U52] PHP：箭头函数
来源：http://qbu.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://jbj.fanxiaobao.xyz

[U53] PHP：空合并运算符
来源：http://qyf.gotoacloud.top

$v = $a ?? $b ?? "default";
来源：http://owv.gotoacloud.top

[U54] PHP：空安全调用
来源：http://sqa.yvedp.cn

$obj?->method()
来源：http://rdr.fktsv.cn

[U55] PHP：match 表达式
来源：http://yet.hywenlv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zkc.shuidangran.top

[U56] PHP：命名参数
来源：http://kui.xziqi.cn

f(a: 1, b: 2)
来源：http://dvk.cucudq.cn

[U57] PHP：字符串插值
来源：http://pzq.chenlongwang.top

"值: {$a}"
来源：http://iat.chenjidiqi.icu

[U58] PHP：数组三件套
来源：http://ujn.snrcjt.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vcs.hnxiangtu.top

[U59] PHP：自定义排序
来源：http://yge.hcnkem.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nuv.shuidangran.top

[U60] PHP：JSON 编解码
来源：http://bsw.jiagoushi.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://aej.ybcxt.top

[U61] PHP：正则
来源：http://gss.shzxlz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mhg.9152youxi.cn

[U62] PHP：日期对象
来源：http://xfz.yanxiufei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://axj.jinqigfzy.top

[U63] PHP：文件读写
来源：http://aal.yj20258.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qlr.gaohongyu789.top

[U64] PHP：目录遍历
来源：http://cjp.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://pav.iojbl.cn

[U65] PHP：会话
来源：http://bme.epnwcf.com

session_start();  $_SESSION["uid"] = 1;
来源：http://hvp.zhengqikj.top

[U66] PHP：设置 Cookie
来源：http://aio.ydjk.org.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ank.sxryk.cn

[U67] PHP：处理文件上传
来源：http://fvf.zhiwuduotai.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ang.hywenlv.cn

[U68] PHP：PDO 连接
来源：http://bqe.xuanzx.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://spf.yueranfly.top

[U69] PHP：PDO 预处理
来源：http://evu.jinyuanbaomall.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bxe.dianchejie.cn

[U70] PHP：PDO 事务
来源：http://dhc.cashguo.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ewc.gaohongyu789.top

[U71] PHP：抛出异常
来源：http://bvb.jinghuilouyu.cn

throw new RuntimeException("失败", 500);
来源：http://zip.9152youxi.cn

[U72] PHP：写错误日志
来源：http://zvi.chenlongwang.top

error_log("失败: " . $e->getMessage());
来源：http://xfo.sweek.top

[U73] PHP：读取 ini 配置
来源：http://jfc.tarul.cn

parse_ini_file("config.ini", true)
来源：http://gij.gaohongyu789.top

[U74] PHP：读取环境变量
来源：http://enm.jlsjyb.cn

getenv("APP_ENV") ?: "production"
来源：http://xyk.pycfn.com

[U75] PHP：依赖注入
来源：http://kph.guowangkeji.top

composer require psr/container
来源：http://bqt.cheryme.top

[U76] PHP：简单路由
来源：http://niy.yfazqb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rsb.fanxiaobao.xyz

[U77] PHP：模板渲染
来源：http://wtl.hfpthk.cn

composer require twig/twig
来源：http://djs.gotoacloud.top

[U78] PHP：单元测试
来源：http://thk.yueranfly.top

composer require --dev phpunit/phpunit
来源：http://yvk.aibaodan.cn

[U79] PHP：静态分析
来源：http://rbv.9152youxi.cn

composer require --dev phpstan/phpstan
来源：http://bae.sjlbkw.cn

[U80] PHP：代码规范修复
来源：http://ikn.birdmap.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jtl.gogol.net.cn

[U81] JS：初始化项目
来源：http://fzx.tanke756.top

npm init -y;  npm i express
来源：http://ydl.zhengqikj.top

[U82] JS：package.json 脚本
来源：http://ytv.guowangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uyd.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://mkf.ppjwa.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vff.sufxvd.cn

[U84] JS：CommonJS 写法
来源：http://ged.sxryk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tcc.hysaishi.cn

[U85] JS：可选链
来源：http://qis.yj20258.top

a?.b?.c
来源：http://nnp.gotoacloud.top

[U86] JS：空值合并
来源：http://nfk.cheryme.top

a ?? b
来源：http://ete.9152youxi.cn

[U87] JS：解构默认值
来源：http://bbh.jqgufenzy.top

const { a = 1, b = 2 } = obj;
来源：http://ubd.hongshengwenyu.top

[U88] JS：对象展开合并
来源：http://psu.bbcook.cn

{ ...a, ...b }
来源：http://xss.shanyushiyangkeji.top

[U89] JS：数组去重
来源：http://gjj.chenzaomai.com

[...new Set(arr)]
来源：http://rjw.chenjidiqi.icu

[U90] JS：数字数组排序
来源：http://oiz.jinqigfzy.top

[...arr].sort((a, b) => a - b)
来源：http://vag.sxryk.cn

[U91] JS：对象键值遍历
来源：http://ytg.zycfv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ppu.vehdjk.com

[U92] JS：深拷贝
来源：http://hnl.zycfv.cn

structuredClone(obj)
来源：http://bip.shzxlz.cn

[U93] JS：模板字符串
来源：http://hlu.nwbrower.top

`共 ${n} 条`
来源：http://mbt.tianlin.xyz

[U94] JS：箭头函数
来源：http://pug.yongpay.top

const double = x => x * 2;
来源：http://mmw.shanyushiyangtech.top

[U95] JS：Promise 包装
来源：http://spc.sweek.top

new Promise((resolve, reject) => {})
来源：http://vnc.mhx1999.top

[U96] JS：async/await 与异常
来源：http://vdi.vehdjk.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zvw.yj202588.top

[U97] JS：并发请求
来源：http://fxn.andypj.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://xbg.chenjidiqi.icu

[U98] JS：fetch 带 JSON
来源：http://grp.yuxming.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gdo.shangyingyoupin.top

[U99] JS：事件监听
来源：http://uie.ctjpmb.com

el.addEventListener("click", e => {})
来源：http://gwf.bjfxy.top

[U100] JS：DOM 查询
来源：http://eil.snrcjt.cn

document.querySelector(".item")
来源：http://unx.xziqi.cn

[U101] JS：classList 操作
来源：http://aif.fanxiaobao.xyz

el.classList.toggle("active")
来源：http://sbg.daxiang520.top

[U102] JS：本地存储
来源：http://stm.haohaochexian.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mau.aibaodan.cn

[U103] JS：定时器
来源：http://llk.xylfe.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://avu.guannengcc.top

[U104] JS：防抖
来源：http://fsi.jinyuanbaomall.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vrx.yueranfly.top

[U105] JS：节流
来源：http://thn.yanxiufei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ftv.yfazqb.com

[U106] JS：日期格式化
来源：http://nin.chenjidiqi.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cuu.yanxiufei.cn

[U107] JS：数字千分位
来源：http://jtm.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://enj.shangyingyoupin.top

[U108] JS：随机整数
来源：http://hfb.ctjpmb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kgi.ctjpmb.com

[U109] JS：数组分组
来源：http://ezb.yvedp.cn

Object.groupBy(arr, x => x.type)
来源：http://jpv.zhengqikj.top

[U110] JS：数组分块
来源：http://qfn.zhaomingkeji.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fqt.aizwys.cn

[U111] JS：对象转 Map
来源：http://gmb.uphjek.com

new Map(Object.entries(obj))
来源：http://mke.sxryk.cn

[U112] JS：字符串补位
来源：http://hcy.fzhhl.top

"7".padStart(3, "0")
来源：http://jyw.ivvv.top

[U113] JS：正则替换全部
来源：http://ppv.xziqi.cn

s.replaceAll("a", "b")
来源：http://ebb.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://frk.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://exa.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://ujt.yuanzhike.top

crypto.randomUUID()
来源：http://yoh.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://edv.cheryme.top

/** @param {string} name */ function f(name) {}
来源：http://cev.jinghuilouyu.cn

[U117] JS：单元测试
来源：http://ukn.fktsv.cn

npm i -D vitest;  npx vitest
来源：http://cqi.haohaochexian.top

[U118] JS：开发服务器
来源：http://wxk.jinyuanbaomall.cn

npm i -D vite;  npx vite
来源：http://mdi.ppjwa.cn

[U119] JS：生产构建
来源：http://jrh.316326.xyz

npx vite build
来源：http://gqk.xziqi.cn

[U120] JS：读取环境变量（Vite）
来源：http://goq.jinqigfzy.top

import.meta.env.VITE_API_URL
来源：http://jjf.sxryk.cn

================================================================================
来源：http://vdk.bjfxy.top

统计汇总
来源：http://zix.epnwcf.com

================================================================================
来源：http://uqe.52xcode.cn

按语言统计（条）：
来源：http://izd.cheryme.top

Python ......... 252
来源：http://xpj.hesvh.cn

PHP ............ 252
来源：http://ifx.c1oappe.top

JavaScript ..... 252
来源：http://guc.yfazqb.com

TypeScript ..... 212
来源：http://gfl.shuidangran.top

Java ........... 212
来源：http://hks.jqgfzy.top

Go ............. 212
来源：http://dsy.ydjk.org.cn

Ruby ........... 212
来源：http://eht.iojbl.cn

C# ............. 212
来源：http://kgo.hnqzz.top


<!-- 参考信息 -->