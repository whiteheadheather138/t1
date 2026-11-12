代发 wailian999

[T41] Perl：Hello World
来源：http://mmu.hammf.cn

print "Hello\n";
来源：http://wri.zhongyouzk.top

[T42] Perl：变量类型
来源：http://den.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kkm.wangdashe.top

[T43] Perl：字符串插值
来源：http://iea.ehwqpu.com

"值: $a"
来源：http://nrd.svipenyu.cn

[T44] Perl：条件
来源：http://vyp.yj20258.top

if ($a > 0) { print "正"; }
来源：http://jic.fehbvm.com

[T45] Perl：数组遍历
来源：http://lhl.jlsjyb.cn

for my $x (@arr) { print $x; }
来源：http://zcc.jqgufenzy.top

[T46] Perl：哈希操作
来源：http://zoa.jlsjyb.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ubh.xingfuxueyuan.xyz

[T47] Perl：正则捕获
来源：http://pmq.gzhubu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qmq.jlsjyb.cn

[T48] Perl：正则替换
来源：http://oiw.ppjwa.cn

$s =~ s/old/new/g;
来源：http://vna.tianlin.xyz

[T49] Perl：函数
来源：http://hvp.xuanzx.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qyn.gotoacloud.top

[T50] Perl：逐行读文件
来源：http://zex.c1oappe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://eji.vehdjk.com

while (my $line = <$fh>) { print $line; }
来源：http://nmu.tian-w.cn

[T51] Scala：Hello World
来源：http://hbg.hongshengwenyu.top

println("Hello")
来源：http://vsl.ppjwa.cn

[T52] Scala：变量
来源：http://hfd.9152youxi.cn

val a = 1;  var b = 2
来源：http://srp.yvedp.cn

[T53] Scala：字符串插值
来源：http://dvy.fanxiaobao.xyz

s"值: $b"
来源：http://uko.ivvv.top

[T54] Scala：集合映射
来源：http://qsq.yanxiufei.cn

List(1, 2, 3).map(_ * 2)
来源：http://yqs.vehdjk.com

[T55] Scala：集合过滤
来源：http://mkn.yj20258888.top

List(1, 2, 3).filter(_ > 1)
来源：http://hcs.pycfn.com

[T56] Scala：样例类
来源：http://gto.xziqi.cn

case class User(name: String, age: Int)
来源：http://czb.316326.xyz

[T57] Scala：模式匹配
来源：http://gwg.wangshuangyany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xwl.tarul.cn

[T58] Scala：函数定义
来源：http://eme.jianghu66.top

def add(a: Int, b: Int): Int = a + b
来源：http://cug.dashuyun.cn

[T59] Scala：循环
来源：http://fsr.ydjk.org.cn

for (i <- 1 to 10) println(i)
来源：http://tow.ydjk.org.cn

[T60] Scala：折叠
来源：http://dnz.jianghu66.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vjn.shuidangran.top

================================================================================
来源：http://tyz.hnqzz.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ukl.smart0.xyz

================================================================================
来源：http://dxl.xuetiantiany.cn

[U01] Py：创建虚拟环境
来源：http://zxw.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tlj.zdbjq.cn

[U02] Py：导出 / 安装依赖
来源：http://toa.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fdn.shanyushiyangkeji.top

[U03] Py：加载 .env 配置
来源：http://pec.shuidangran.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ues.9152youxi.cn

[U04] Py：变量调试打印
来源：http://fny.gzhubu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wfy.yongpay.top

[U05] Py：列表去重且保序
来源：http://ush.tian-w.cn

list(dict.fromkeys(arr))
来源：http://slo.ivvv.top

[U06] Py：合并两个字典
来源：http://dgx.yj202588.top

{**a, **b}
来源：http://ezm.shuidangran.top

[U07] Py：反转字典键值
来源：http://brb.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://sax.ydzc1.top

[U08] Py：展平二维列表
来源：http://xln.xuanzx.com

[y for x in nested for y in x]
来源：http://lyx.hammf.cn

[U09] Py：字典取最大值的键
来源：http://shy.daxiang520.top

max(d, key=d.get)
来源：http://zhg.mhx1999.top

[U10] Py：按值排序字典
来源：http://tqy.zhaomingkeji.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://egh.jinghuilouyu.cn

[U11] Py：生成器表达式
来源：http://bkz.gotoacloud.top

(x * 2 for x in arr)
来源：http://tzu.shanyushiyangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://ecl.yueranfly.top

Counter(arr).most_common(3)
来源：http://pka.fehbvm.com

[U13] Py：固定长度队列
来源：http://usc.yangfankeji.com

deque(maxlen=10)
来源：http://plw.aizwys.cn

[U14] Py：分组收集到列表
来源：http://zmw.guowangkeji.top

defaultdict(list)
来源：http://iya.nanxinkj.top

[U15] Py：高精度计时
来源：http://jpt.ybcxt.top

t = time.perf_counter()
来源：http://oyu.ehwqpu.com

[U16] Py：命令行参数解析
来源：http://lrd.jinghuilouyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ttc.zhaomingkeji.xyz

[U17] Py：初始化日志
来源：http://ajh.dashuyun.cn

logging.basicConfig(level=logging.INFO)
来源：http://eir.chenjidiqi.icu

[U18] Py：预编译正则
来源：http://kpi.ywan-chungtsiang.top

pat = re.compile(r"\d+")
来源：http://mnw.0kj1m.cn

[U19] Py：正则替换带回调
来源：http://fyf.fzhhl.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yiu.cheryme.top

[U20] Py：缓存函数结果
来源：http://wnl.bbcook.cn

@functools.lru_cache(maxsize=None)
来源：http://sen.hesvh.cn

[U21] Py：自定义上下文管理器
来源：http://hor.hammf.cn

@contextlib.contextmanager
来源：http://qpn.ydzc1.top

[U22] Py：矩阵转置
来源：http://okr.xylfe.cn

list(zip(*m))
来源：http://tdd.yj20258888.top

[U23] Py：分块读取大文件
来源：http://fzx.yuanzhike.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gmj.zhoulong.xyz

[U24] Py：路径操作
来源：http://uqk.jiagoushi.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kdg.ehwqpu.com

[U25] Py：CSV 按字典读
来源：http://pfd.guowangkeji.top

csv.DictReader(f)
来源：http://bvc.dashuyun.cn

[U26] Py：并发下载
来源：http://xhp.ydjk.org.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qcn.ehwqpu.com

[U27] Py：异步 HTTP
来源：http://jeo.yueranfly.top

aiohttp.ClientSession() 配合 async with
来源：http://qww.9152youxi.cn

[U28] Py：类型别名
来源：http://vhc.cucudq.cn

UserId = int
来源：http://kmr.hammf.cn

[U29] Py：属性校验
来源：http://oxq.jinqigufen.top

@property 与 @x.setter 配合
来源：http://yob.9152youxi.cn

[U30] Py：数据类
来源：http://idm.smart0.xyz

@dataclass(slots=True)
来源：http://qrs.hnqzz.top

[U31] Py：单测
来源：http://rik.gotoacloud.top

python -m pytest -q
来源：http://nts.xuanzx.com

[U32] Py：代码格式化
来源：http://mnr.yj202588.top

ruff format . && ruff check --fix .
来源：http://tvh.haohaochexian.top

[U33] Py：打包发布
来源：http://syv.xuetiantiany.cn

python -m build  （依赖 pyproject.toml）
来源：http://pzv.ehwqpu.com

[U34] Py：判断编码
来源：http://nbb.sxryk.cn

chardet.detect(raw)
来源：http://ndk.shangyingyoupin.top

[U35] Py：发送邮件
来源：http://dvi.zhiwuduotai.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tvm.nanxinkj.top

[U36] Py：定时任务
来源：http://aql.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://fuo.havefunace.top

[U37] Py：读写 Excel
来源：http://efr.guowangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://pzn.shanyushiyangkeji.top

[U38] Py：获取脚本所在目录
来源：http://phv.9152youxi.cn

Path(__file__).resolve().parent
来源：http://tgw.zhiwuduotai.top

[U39] Py：判断是否在交互环境
来源：http://qcd.wangshuangyany.cn

sys.stdout.isatty()
来源：http://ngr.316326.xyz

[U40] Py：打印到标准错误
来源：http://prr.jqgfzy.top

print("err", file=sys.stderr)
来源：http://xtk.ydjk.org.cn

[U41] PHP：初始化 Composer 项目
来源：http://lxl.yvedp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ble.yvedp.cn

[U42] PHP：PSR-4 自动加载
来源：http://jwk.hcnkem.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xid.birdmap.top

[U43] PHP：声明命名空间
来源：http://udw.havefunace.top

namespace App\Http;
来源：http://syy.vehdjk.com

[U44] PHP：开启严格类型
来源：http://box.gaohongyu789.top

declare(strict_types=1);
来源：http://twl.xziqi.cn

[U45] PHP：类型声明与返回类型
来源：http://bpm.uphjek.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://jpw.yangfankeji.com

[U46] PHP：可空类型
来源：http://fwn.hnqzz.top

?string $name = null
来源：http://ngq.gotoacloud.top

[U47] PHP：联合类型
来源：http://whu.jinqigfzy.top

int|string $id
来源：http://aqi.hnxiangtu.top

[U48] PHP：纯枚举
来源：http://nfn.52xcode.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ott.hysaishi.cn

[U49] PHP：只读属性
来源：http://gby.zhongyouzk.top

public readonly string $name
来源：http://gnm.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://ehv.guannengcc.top

public function __construct(private int $id) {}
来源：http://fyl.jiagoushi.top

[U51] PHP：数组解构
来源：http://ghf.shzxlz.cn

[$a, $b] = $arr;
来源：http://lyq.daria6918.cn

[U52] PHP：箭头函数
来源：http://eab.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://iux.yuanzhike.top

[U53] PHP：空合并运算符
来源：http://geq.xziqi.cn

$v = $a ?? $b ?? "default";
来源：http://htb.zhaomingkeji.xyz

[U54] PHP：空安全调用
来源：http://vyd.sweek.top

$obj?->method()
来源：http://mqn.gogol.net.cn

[U55] PHP：match 表达式
来源：http://ykr.gogol.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fvj.ehwqpu.com

[U56] PHP：命名参数
来源：http://swp.zhaomingkeji.xyz

f(a: 1, b: 2)
来源：http://xzj.zhijiandao.cn

[U57] PHP：字符串插值
来源：http://omw.shanyushiyangkeji.top

"值: {$a}"
来源：http://lxf.svipenyu.cn

[U58] PHP：数组三件套
来源：http://kyc.chenjidiqi.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vcs.xylfe.cn

[U59] PHP：自定义排序
来源：http://oiz.ydzc1.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dae.shangyingyoupin.top

[U60] PHP：JSON 编解码
来源：http://pdd.jinqigufen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lwj.tianlin.xyz

[U61] PHP：正则
来源：http://mff.nanxinkj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tmi.yj202588.top

[U62] PHP：日期对象
来源：http://vap.zycfv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://edx.hysaishi.cn

[U63] PHP：文件读写
来源：http://opj.wangdashe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lok.cdnleiting.top

[U64] PHP：目录遍历
来源：http://fsx.xuanzx.com

glob("dir/*.php");  scandir("dir");
来源：http://kub.shuidangran.top

[U65] PHP：会话
来源：http://gwd.hesvh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xfq.cdnleiting.top

[U66] PHP：设置 Cookie
来源：http://kfq.zhijiandao.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://umf.zhixingplan.top

[U67] PHP：处理文件上传
来源：http://xpo.0kj1m.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dmd.fktsv.cn

[U68] PHP：PDO 连接
来源：http://eiu.wangshuangyany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pfl.birdmap.top

[U69] PHP：PDO 预处理
来源：http://bdl.ivvv.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tlt.yonumen.top

[U70] PHP：PDO 事务
来源：http://lrd.dashuyun.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wgr.hnxiangtu.top

[U71] PHP：抛出异常
来源：http://rql.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://bhh.vqdsnc.cn

[U72] PHP：写错误日志
来源：http://erq.bjfxy.top

error_log("失败: " . $e->getMessage());
来源：http://lxu.sweek.top

[U73] PHP：读取 ini 配置
来源：http://myw.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://jtt.vqdsnc.cn

[U74] PHP：读取环境变量
来源：http://fwn.jianghu66.top

getenv("APP_ENV") ?: "production"
来源：http://qmb.zhoulong.xyz

[U75] PHP：依赖注入
来源：http://dnd.fanxiaobao.xyz

composer require psr/container
来源：http://gyt.fktsv.cn

[U76] PHP：简单路由
来源：http://ijn.shangyingyoupin.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xjm.0kj1m.cn

[U77] PHP：模板渲染
来源：http://pve.xylfe.cn

composer require twig/twig
来源：http://tal.9152youxi.cn

[U78] PHP：单元测试
来源：http://nwi.andypj.xyz

composer require --dev phpunit/phpunit
来源：http://ccq.ppjwa.cn

[U79] PHP：静态分析
来源：http://xtb.shuidangran.top

composer require --dev phpstan/phpstan
来源：http://ulo.vehdjk.com

[U80] PHP：代码规范修复
来源：http://zfq.hfpthk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nbw.9152youxi.cn

[U81] JS：初始化项目
来源：http://kvj.daria6918.cn

npm init -y;  npm i express
来源：http://jjw.hnqzz.top

[U82] JS：package.json 脚本
来源：http://odd.dianchejie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jej.zhijiandao.cn

[U83] JS：ES Module 导入导出
来源：http://lgx.aizwys.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bvo.chenzaomai.com

[U84] JS：CommonJS 写法
来源：http://kox.yj20258888.top

module.exports = { a };  const { a } = require("./m");
来源：http://mzy.cucudq.cn

[U85] JS：可选链
来源：http://jsj.shuidangran.top

a?.b?.c
来源：http://ght.xylfe.cn

[U86] JS：空值合并
来源：http://xnp.fktsv.cn

a ?? b
来源：http://htm.fanxiaobao.xyz

[U87] JS：解构默认值
来源：http://tji.redwolf501.top

const { a = 1, b = 2 } = obj;
来源：http://cuw.cheryme.top

[U88] JS：对象展开合并
来源：http://nfy.fktsv.cn

{ ...a, ...b }
来源：http://nuo.ehwqpu.com

[U89] JS：数组去重
来源：http://qck.vehdjk.com

[...new Set(arr)]
来源：http://lcq.zycfv.cn

[U90] JS：数字数组排序
来源：http://ejb.zhixingplan.top

[...arr].sort((a, b) => a - b)
来源：http://uab.nanxuanxn.top

[U91] JS：对象键值遍历
来源：http://dgp.fktsv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tie.gzhubu.top

[U92] JS：深拷贝
来源：http://bgw.dianchejie.cn

structuredClone(obj)
来源：http://tcb.zhengqikj.top

[U93] JS：模板字符串
来源：http://bhi.yonumen.top

`共 ${n} 条`
来源：http://vtk.sufxvd.cn

[U94] JS：箭头函数
来源：http://iay.jqgfzy.top

const double = x => x * 2;
来源：http://qsl.pengpengdd.cyou

[U95] JS：Promise 包装
来源：http://ikf.zhengqikj.top

new Promise((resolve, reject) => {})
来源：http://mrb.fktsv.cn

[U96] JS：async/await 与异常
来源：http://wdp.jinghuilouyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ikf.9152youxi.cn

[U97] JS：并发请求
来源：http://mqp.zdqjudy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tzh.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://twt.nanxuanxn.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ubj.aibaodan.cn

[U99] JS：事件监听
来源：http://avj.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://jis.vqdsnc.cn

[U100] JS：DOM 查询
来源：http://wxn.zhixingplan.top

document.querySelector(".item")
来源：http://vcz.hywenlv.cn

[U101] JS：classList 操作
来源：http://tyt.daria6918.cn

el.classList.toggle("active")
来源：http://lad.cqqwz.cn

[U102] JS：本地存储
来源：http://lwu.andypj.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://fiu.shangyingyoupin.top

[U103] JS：定时器
来源：http://nbm.ydjk.org.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vkv.yongpay.top

[U104] JS：防抖
来源：http://rwa.9152youxi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dlr.jlsjyb.cn

[U105] JS：节流
来源：http://xpp.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bda.yongpay.top

[U106] JS：日期格式化
来源：http://vlm.pengpengdd.cyou

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://abw.jinyuanbaomall.cn

[U107] JS：数字千分位
来源：http://qao.52xcode.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rgm.epnwcf.com

[U108] JS：随机整数
来源：http://geh.zhiwuduotai.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oxy.xziqi.cn

[U109] JS：数组分组
来源：http://xik.birdmap.top

Object.groupBy(arr, x => x.type)
来源：http://sax.daxiang520.top

[U110] JS：数组分块
来源：http://ryc.ydzc1.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ric.tian-w.cn

[U111] JS：对象转 Map
来源：http://gss.svipenyu.cn

new Map(Object.entries(obj))
来源：http://kly.tanke756.top

[U112] JS：字符串补位
来源：http://rba.jqgufenzy.top

"7".padStart(3, "0")
来源：http://oye.redwolf501.top

[U113] JS：正则替换全部
来源：http://jpi.yueranfly.top

s.replaceAll("a", "b")
来源：http://tea.gotoacloud.top

[U114] JS：JSON 深比较
来源：http://kcr.redwolf501.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://svg.vqdsnc.cn

[U115] JS：生成 UUID
来源：http://bdt.ydjk.org.cn

crypto.randomUUID()
来源：http://ath.pengpengdd.cyou

[U116] JS：类型检查（JSDoc）
来源：http://sek.kuanghao11.cn

/** @param {string} name */ function f(name) {}
来源：http://zda.bjfxy.top

[U117] JS：单元测试
来源：http://ydh.ydjk.org.cn

npm i -D vitest;  npx vitest
来源：http://blr.andypj.xyz

[U118] JS：开发服务器
来源：http://dpc.daria6918.cn

npm i -D vite;  npx vite
来源：http://dct.ivvv.top

[U119] JS：生产构建
来源：http://csp.vqdsnc.cn

npx vite build
来源：http://bke.hammf.cn

[U120] JS：读取环境变量（Vite）
来源：http://gjm.yj20258.top

import.meta.env.VITE_API_URL
来源：http://ohn.shanyushiyangkeji.top

================================================================================
来源：http://wrq.yuxming.cn

统计汇总
来源：http://qxs.quarkkingdee.top

================================================================================
来源：http://pkf.xylfe.cn

按语言统计（条）：
来源：http://dwy.xingfuxueyuan.xyz

Python ......... 252
来源：http://mmm.wangdashe.top

PHP ............ 252
来源：http://khm.tian-w.cn

JavaScript ..... 252
来源：http://bvv.havefunace.top

TypeScript ..... 212
来源：http://iqi.vehdjk.com

Java ........... 212
来源：http://qji.ybcxt.top

Go ............. 212
来源：http://ytk.hesvh.cn

Ruby ........... 212
来源：http://lzq.cashguo.top

C# ............. 212
来源：http://hzw.redwolf501.top

C .............. 30
来源：http://hsu.xziqi.cn

C++ ............ 30
来源：http://alo.xinyue.icu

SQL ............ 90
来源：http://qjr.ctjpmb.com

Bash ........... 80
来源：http://ajo.dashuyun.cn


<!-- 参考信息 -->