代发 wailian999

[T29] Swift：guard 提前返回
来源：http://vgn.kuanghao11.cn

guard let x = opt else { return }
来源：http://yyk.yueranfly.top

[T30] Swift：协议
来源：http://wpf.jyoumei.cn

protocol Shape { func area() -> Double }
来源：http://ejo.yfazqb.com

[T31] Lua：Hello World
来源：http://mqc.sjlbkw.cn

print("Hello")
来源：http://myw.9152youxi.cn

[T32] Lua：局部变量
来源：http://kil.zhixingplan.top

local a = 1
来源：http://ski.quarkkingdee.top

[T33] Lua：表（数组）
来源：http://gbo.sufxvd.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kuk.bbcook.cn

[T34] Lua：遍历表
来源：http://oqp.redwolf501.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ngy.zhixingplan.top

[T35] Lua：字典表
来源：http://qxg.haohaochexian.top

local d = { a = 1 };  d.b = 2
来源：http://nro.jiagoushi.top

[T36] Lua：函数
来源：http://uag.9152youxi.cn

function add(a, b) return a + b end
来源：http://hea.hammf.cn

[T37] Lua：字符串拼接
来源：http://tsj.smart0.xyz

"a" .. "b"
来源：http://kyl.jinyuanbaomall.cn

[T38] Lua：条件
来源：http://gmb.gotoacloud.top

if x > 0 then print("正") end
来源：http://nls.hcnkem.com

[T39] Lua：模式匹配
来源：http://guv.gotoacloud.top

string.find(s, "%d+")
来源：http://prn.tarul.cn

[T40] Lua：元表
来源：http://out.vqdsnc.cn

setmetatable({}, { __index = base })
来源：http://xej.tian-w.cn

[T41] Perl：Hello World
来源：http://vgn.chenjidiqi.icu

print "Hello\n";
来源：http://mzd.c1oappe.top

[T42] Perl：变量类型
来源：http://qda.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dsg.gaohongyu789.top

[T43] Perl：字符串插值
来源：http://bnk.9152youxi.cn

"值: $a"
来源：http://cqs.tianlin.xyz

[T44] Perl：条件
来源：http://fms.shangyingyoupin.top

if ($a > 0) { print "正"; }
来源：http://oep.wangshuangyany.cn

[T45] Perl：数组遍历
来源：http://xbs.yuanzhike.top

for my $x (@arr) { print $x; }
来源：http://qzl.ivvv.top

[T46] Perl：哈希操作
来源：http://ztb.cdnleiting.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dzl.chenlongwang.top

[T47] Perl：正则捕获
来源：http://ifn.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://edq.vqdsnc.cn

[T48] Perl：正则替换
来源：http://idq.guowangkeji.top

$s =~ s/old/new/g;
来源：http://yje.zdbjq.cn

[T49] Perl：函数
来源：http://rik.jinqigufen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://can.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://qnw.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://evd.jinghuilouyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ski.yj20258.top

[T51] Scala：Hello World
来源：http://swo.fzhhl.top

println("Hello")
来源：http://its.vehdjk.com

[T52] Scala：变量
来源：http://mek.hongshengwenyu.top

val a = 1;  var b = 2
来源：http://foi.yvedp.cn

[T53] Scala：字符串插值
来源：http://fqi.cashguo.top

s"值: $b"
来源：http://isx.jinqigfzy.top

[T54] Scala：集合映射
来源：http://hne.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://dmt.jinqigfzy.top

[T55] Scala：集合过滤
来源：http://trn.fzhhl.top

List(1, 2, 3).filter(_ > 1)
来源：http://zjs.zdbjq.cn

[T56] Scala：样例类
来源：http://kov.yj202588.top

case class User(name: String, age: Int)
来源：http://gzi.ehwqpu.com

[T57] Scala：模式匹配
来源：http://gvr.vqdsnc.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://onk.vehdjk.com

[T58] Scala：函数定义
来源：http://xks.ctjpmb.com

def add(a: Int, b: Int): Int = a + b
来源：http://klw.hfpthk.cn

[T59] Scala：循环
来源：http://btp.tianlin.xyz

for (i <- 1 to 10) println(i)
来源：http://gra.meibo888.top

[T60] Scala：折叠
来源：http://ies.jqgfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tvw.andypj.xyz

================================================================================
来源：http://gfd.hesvh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ank.cdnleiting.top

================================================================================
来源：http://xag.guannengcc.top

[U01] Py：创建虚拟环境
来源：http://lkx.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qmk.jyoumei.cn

[U02] Py：导出 / 安装依赖
来源：http://fad.hesvh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vqr.ppjwa.cn

[U03] Py：加载 .env 配置
来源：http://nbn.chenjidiqi.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://dki.wangshuangyany.cn

[U04] Py：变量调试打印
来源：http://pps.bbcook.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cnn.fzhhl.top

[U05] Py：列表去重且保序
来源：http://spx.mhx1999.top

list(dict.fromkeys(arr))
来源：http://iee.zdqjudy.top

[U06] Py：合并两个字典
来源：http://hki.aizwys.cn

{**a, **b}
来源：http://ass.mhx1999.top

[U07] Py：反转字典键值
来源：http://wtk.vehdjk.com

{v: k for k, v in d.items()}
来源：http://kiv.birdmap.top

[U08] Py：展平二维列表
来源：http://nwf.ydzc1.top

[y for x in nested for y in x]
来源：http://maz.quarkkingdee.top

[U09] Py：字典取最大值的键
来源：http://qeq.zycfv.cn

max(d, key=d.get)
来源：http://sef.havefunace.top

[U10] Py：按值排序字典
来源：http://ugc.sxryk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hlh.hongshengwenyu.top

[U11] Py：生成器表达式
来源：http://cvy.shangyingyoupin.top

(x * 2 for x in arr)
来源：http://mss.meibo888.top

[U12] Py：取出现最多的 3 个元素
来源：http://sgb.yfazqb.com

Counter(arr).most_common(3)
来源：http://ynn.gaohongyu789.top

[U13] Py：固定长度队列
来源：http://spp.gaohongyu789.top

deque(maxlen=10)
来源：http://kft.yuanzhike.top

[U14] Py：分组收集到列表
来源：http://hgl.quarkkingdee.top

defaultdict(list)
来源：http://hqt.xylfe.cn

[U15] Py：高精度计时
来源：http://ldh.daria6918.cn

t = time.perf_counter()
来源：http://zxh.fengsongda.top

[U16] Py：命令行参数解析
来源：http://vjv.ctjpmb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aqz.snrcjt.cn

[U17] Py：初始化日志
来源：http://mea.zhixingplan.top

logging.basicConfig(level=logging.INFO)
来源：http://pgq.mhx1999.top

[U18] Py：预编译正则
来源：http://zbv.hammf.cn

pat = re.compile(r"\d+")
来源：http://lhv.birdmap.top

[U19] Py：正则替换带回调
来源：http://ujd.yj20258888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bev.zycfv.cn

[U20] Py：缓存函数结果
来源：http://hbh.c1oappe.top

@functools.lru_cache(maxsize=None)
来源：http://bnz.c1oappe.top

[U21] Py：自定义上下文管理器
来源：http://ehi.svipenyu.cn

@contextlib.contextmanager
来源：http://mcv.9152youxi.cn

[U22] Py：矩阵转置
来源：http://dew.bjfxy.top

list(zip(*m))
来源：http://upi.52xcode.cn

[U23] Py：分块读取大文件
来源：http://knm.pengpengdd.cyou

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tqe.hysaishi.cn

[U24] Py：路径操作
来源：http://olo.chenzaomai.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ygp.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://hln.hywenlv.cn

csv.DictReader(f)
来源：http://qoq.tian-w.cn

[U26] Py：并发下载
来源：http://kiw.ivvv.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://emh.zhongyouzk.top

[U27] Py：异步 HTTP
来源：http://tbc.gzhubu.top

aiohttp.ClientSession() 配合 async with
来源：http://uzj.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://yah.jinqigufen.top

UserId = int
来源：http://ajc.yangfankeji.com

[U29] Py：属性校验
来源：http://xcs.ivvv.top

@property 与 @x.setter 配合
来源：http://rsh.shanyushiyangtech.top

[U30] Py：数据类
来源：http://gng.yvedp.cn

@dataclass(slots=True)
来源：http://vwo.sxryk.cn

[U31] Py：单测
来源：http://htz.zhongyouzk.top

python -m pytest -q
来源：http://qei.jiagoushi.top

[U32] Py：代码格式化
来源：http://jdf.zhengqikj.top

ruff format . && ruff check --fix .
来源：http://fzr.jinqigfzy.top

[U33] Py：打包发布
来源：http://kjn.svipenyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://hwc.ehwqpu.com

[U34] Py：判断编码
来源：http://tly.shanyushiyangkeji.top

chardet.detect(raw)
来源：http://dip.xziqi.cn

[U35] Py：发送邮件
来源：http://svi.meibo888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wuf.yj20258888.top

[U36] Py：定时任务
来源：http://fux.fktsv.cn

schedule.every(10).minutes.do(job)
来源：http://xwh.yueranfly.top

[U37] Py：读写 Excel
来源：http://ujr.hywenlv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zeh.fengsongda.top

[U38] Py：获取脚本所在目录
来源：http://wrd.sysykeji.top

Path(__file__).resolve().parent
来源：http://qgo.andypj.xyz

[U39] Py：判断是否在交互环境
来源：http://lfp.yanxiufei.cn

sys.stdout.isatty()
来源：http://xfy.hysaishi.cn

[U40] Py：打印到标准错误
来源：http://apj.zhengqikj.top

print("err", file=sys.stderr)
来源：http://bxu.cashguo.top

[U41] PHP：初始化 Composer 项目
来源：http://hcc.zdbjq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://acq.sufxvd.cn

[U42] PHP：PSR-4 自动加载
来源：http://sgb.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ljl.xuanzx.com

[U43] PHP：声明命名空间
来源：http://kmn.ydjk.org.cn

namespace App\Http;
来源：http://qut.zycfv.cn

[U44] PHP：开启严格类型
来源：http://idb.tianlin.xyz

declare(strict_types=1);
来源：http://wns.quarkkingdee.top

[U45] PHP：类型声明与返回类型
来源：http://bsj.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://juq.zhongyouzk.top

[U46] PHP：可空类型
来源：http://tqc.kuanghao11.cn

?string $name = null
来源：http://fjo.chenzaomai.com

[U47] PHP：联合类型
来源：http://mfv.shangyingyoupin.top

int|string $id
来源：http://tdd.sufxvd.cn

[U48] PHP：纯枚举
来源：http://evk.tarul.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://syo.vqdsnc.cn

[U49] PHP：只读属性
来源：http://kli.hesvh.cn

public readonly string $name
来源：http://gow.daxiang520.top

[U50] PHP：构造器属性提升
来源：http://oaj.fengsongda.top

public function __construct(private int $id) {}
来源：http://crt.yanxiufei.cn

[U51] PHP：数组解构
来源：http://opa.kuanghao11.cn

[$a, $b] = $arr;
来源：http://jvo.tian-w.cn

[U52] PHP：箭头函数
来源：http://mxb.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://ipx.cqqwz.cn

[U53] PHP：空合并运算符
来源：http://jjm.jinqigufen.top

$v = $a ?? $b ?? "default";
来源：http://ogk.cdnleiting.top

[U54] PHP：空安全调用
来源：http://zbs.birdmap.top

$obj?->method()
来源：http://xku.meibo888.top

[U55] PHP：match 表达式
来源：http://pzx.haohaochexian.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zup.gzhubu.top

[U56] PHP：命名参数
来源：http://ueh.jinqigufen.top

f(a: 1, b: 2)
来源：http://zzc.hnxiangtu.top

[U57] PHP：字符串插值
来源：http://pjw.shanyushiyangtech.top

"值: {$a}"
来源：http://ain.xingfuxueyuan.xyz

[U58] PHP：数组三件套
来源：http://zuy.shanyushiyangtech.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sgo.nanxuanxn.top

[U59] PHP：自定义排序
来源：http://nnp.dashuyun.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://khd.guannengcc.top

[U60] PHP：JSON 编解码
来源：http://uas.ybcxt.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qrx.zhiwuduotai.top

[U61] PHP：正则
来源：http://bfb.hnxiangtu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jwm.yuanzhike.top

[U62] PHP：日期对象
来源：http://mgc.yongpay.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gns.zhixingplan.top

[U63] PHP：文件读写
来源：http://qeo.havefunace.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tas.cdnleiting.top

[U64] PHP：目录遍历
来源：http://hnc.nwbrower.top

glob("dir/*.php");  scandir("dir");
来源：http://qxb.hywenlv.cn

[U65] PHP：会话
来源：http://ynl.chenzaomai.com

session_start();  $_SESSION["uid"] = 1;
来源：http://bpc.chenlongwang.top

[U66] PHP：设置 Cookie
来源：http://wfn.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ayt.sjlbkw.cn

[U67] PHP：处理文件上传
来源：http://hyh.yongpay.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jqv.dianchejie.cn

[U68] PHP：PDO 连接
来源：http://tcr.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://azy.gotoacloud.top

[U69] PHP：PDO 预处理
来源：http://jpj.zycfv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://shv.jiagoushi.top

[U70] PHP：PDO 事务
来源：http://olj.feifeiyinyue.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ypr.fzhhl.top

[U71] PHP：抛出异常
来源：http://rcu.sysykeji.top

throw new RuntimeException("失败", 500);
来源：http://uyx.zhengqikj.top

[U72] PHP：写错误日志
来源：http://abh.andypj.xyz

error_log("失败: " . $e->getMessage());
来源：http://ffy.tanke756.top

[U73] PHP：读取 ini 配置
来源：http://zqi.yj202588.top

parse_ini_file("config.ini", true)
来源：http://cxy.jinqigufen.top

[U74] PHP：读取环境变量
来源：http://ofa.haohaochexian.top

getenv("APP_ENV") ?: "production"
来源：http://xcp.kuanghao11.cn

[U75] PHP：依赖注入
来源：http://ggd.aibaodan.cn

composer require psr/container
来源：http://wqs.nanxinkj.top

[U76] PHP：简单路由
来源：http://urf.hywenlv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dmo.feifeiyinyue.top

[U77] PHP：模板渲染
来源：http://yoe.guowangkeji.top

composer require twig/twig
来源：http://kwk.fengsongda.top

[U78] PHP：单元测试
来源：http://moz.gogol.net.cn

composer require --dev phpunit/phpunit
来源：http://pkj.zhiwuduotai.top

[U79] PHP：静态分析
来源：http://eaw.zdqjudy.top

composer require --dev phpstan/phpstan
来源：http://xxc.dashuyun.cn

[U80] PHP：代码规范修复
来源：http://zxy.smart0.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://ggw.sufxvd.cn

[U81] JS：初始化项目
来源：http://rye.yvedp.cn

npm init -y;  npm i express
来源：http://nrw.daria6918.cn

[U82] JS：package.json 脚本
来源：http://yoe.yongpay.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ogm.shzxlz.cn

[U83] JS：ES Module 导入导出
来源：http://tpz.jyoumei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://off.aizwys.cn

[U84] JS：CommonJS 写法
来源：http://mnc.fengsongda.top

module.exports = { a };  const { a } = require("./m");
来源：http://bmb.hysaishi.cn

[U85] JS：可选链
来源：http://cco.zhiwuduotai.top

a?.b?.c
来源：http://fqt.yj202588.top

[U86] JS：空值合并
来源：http://bdz.316326.xyz

a ?? b
来源：http://ppy.ppjwa.cn

[U87] JS：解构默认值
来源：http://pxa.gogol.net.cn

const { a = 1, b = 2 } = obj;
来源：http://rew.mhx1999.top

[U88] JS：对象展开合并
来源：http://bxr.fzhhl.top

{ ...a, ...b }
来源：http://wiw.xinyue.icu

[U89] JS：数组去重
来源：http://qht.pengpengdd.cyou

[...new Set(arr)]
来源：http://hvr.yj20258.top

[U90] JS：数字数组排序
来源：http://eaz.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://amq.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://riq.sweek.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mbm.hammf.cn

[U92] JS：深拷贝
来源：http://dlr.nanxuanxn.top

structuredClone(obj)
来源：http://snb.sweek.top

[U93] JS：模板字符串
来源：http://sgx.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://ghy.cashguo.top

[U94] JS：箭头函数
来源：http://bll.zhijiandao.cn

const double = x => x * 2;
来源：http://lzs.aibaodan.cn

[U95] JS：Promise 包装
来源：http://oww.hfpthk.cn

new Promise((resolve, reject) => {})
来源：http://ikj.cdnleiting.top

[U96] JS：async/await 与异常
来源：http://hre.wangshuangyany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cza.wangdashe.top

[U97] JS：并发请求
来源：http://udi.ehwqpu.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://zdv.shanyushiyangtech.top

[U98] JS：fetch 带 JSON
来源：http://vbs.xziqi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nwq.c1oappe.top

[U99] JS：事件监听
来源：http://bby.tanke756.top

el.addEventListener("click", e => {})
来源：http://exy.jlsjyb.cn

[U100] JS：DOM 查询
来源：http://ecp.zhengqikj.top

document.querySelector(".item")
来源：http://pnl.fktsv.cn

[U101] JS：classList 操作
来源：http://mjz.tian-w.cn

el.classList.toggle("active")
来源：http://mbz.yueranfly.top

[U102] JS：本地存储
来源：http://sbv.quarkkingdee.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://njq.jianghu66.top

[U103] JS：定时器
来源：http://nxz.chenjidiqi.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zac.jinyuanbaomall.cn

[U104] JS：防抖
来源：http://jsp.pycfn.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ima.sysykeji.top

[U105] JS：节流
来源：http://mqq.cqqwz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cxf.jinqigufen.top

[U106] JS：日期格式化
来源：http://kwy.yangfankeji.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kvg.zdqjudy.top

[U107] JS：数字千分位
来源：http://dpt.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rsz.xziqi.cn

[U108] JS：随机整数
来源：http://rnp.jyoumei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pbf.jianghu66.top

[U109] JS：数组分组
来源：http://svg.mhx1999.top

Object.groupBy(arr, x => x.type)
来源：http://jyt.hammf.cn

[U110] JS：数组分块
来源：http://kdn.cdnleiting.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qqw.shangyingyoupin.top

[U111] JS：对象转 Map
来源：http://aop.sjlbkw.cn

new Map(Object.entries(obj))
来源：http://mti.sysykeji.top

[U112] JS：字符串补位
来源：http://iqb.bjfxy.top

"7".padStart(3, "0")
来源：http://fem.guannengcc.top

[U113] JS：正则替换全部
来源：http://atz.yj202588.top

s.replaceAll("a", "b")
来源：http://kvv.andypj.xyz

[U114] JS：JSON 深比较
来源：http://vyv.yj20258.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://srx.sysykeji.top

[U115] JS：生成 UUID
来源：http://prh.mhx1999.top

crypto.randomUUID()
来源：http://qos.bjfxy.top

[U116] JS：类型检查（JSDoc）
来源：http://vnn.jianghu66.top

/** @param {string} name */ function f(name) {}
来源：http://fyh.fengsongda.top


<!-- 参考信息 -->