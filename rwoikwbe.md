代发 wailian999

[T35] Lua：字典表
来源：http://kdj.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://ykt.jinghuilouyu.cn

[T36] Lua：函数
来源：http://yyw.jinqigufen.top

function add(a, b) return a + b end
来源：http://gka.jinqigfzy.top

[T37] Lua：字符串拼接
来源：http://jjr.9152youxi.cn

"a" .. "b"
来源：http://ktu.svipenyu.cn

[T38] Lua：条件
来源：http://rez.hesvh.cn

if x > 0 then print("正") end
来源：http://pdj.bbcook.cn

[T39] Lua：模式匹配
来源：http://orw.yongpay.top

string.find(s, "%d+")
来源：http://tnt.svipenyu.cn

[T40] Lua：元表
来源：http://sxv.fktsv.cn

setmetatable({}, { __index = base })
来源：http://aaf.aibaodan.cn

[T41] Perl：Hello World
来源：http://tuj.hfpthk.cn

print "Hello\n";
来源：http://bqm.haohaochexian.top

[T42] Perl：变量类型
来源：http://nhc.sysykeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mre.meibo888.top

[T43] Perl：字符串插值
来源：http://ykv.bbcook.cn

"值: $a"
来源：http://szy.9152youxi.cn

[T44] Perl：条件
来源：http://rqw.sweek.top

if ($a > 0) { print "正"; }
来源：http://lvk.xuetiantiany.cn

[T45] Perl：数组遍历
来源：http://zya.gogol.net.cn

for my $x (@arr) { print $x; }
来源：http://lyv.daria6918.cn

[T46] Perl：哈希操作
来源：http://pze.yueranfly.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uin.hesvh.cn

[T47] Perl：正则捕获
来源：http://gwt.ydzc1.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://agp.havefunace.top

[T48] Perl：正则替换
来源：http://bot.ppjwa.cn

$s =~ s/old/new/g;
来源：http://bvp.tianlin.xyz

[T49] Perl：函数
来源：http://wee.xuetiantiany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jbl.c1oappe.top

[T50] Perl：逐行读文件
来源：http://lgq.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nxe.sweek.top

while (my $line = <$fh>) { print $line; }
来源：http://ymc.tarul.cn

[T51] Scala：Hello World
来源：http://nzx.xinyue.icu

println("Hello")
来源：http://rrf.sufxvd.cn

[T52] Scala：变量
来源：http://zeq.nanxinkj.top

val a = 1;  var b = 2
来源：http://xnl.mhx1999.top

[T53] Scala：字符串插值
来源：http://iep.havefunace.top

s"值: $b"
来源：http://pou.meibo888.top

[T54] Scala：集合映射
来源：http://gmj.gotoacloud.top

List(1, 2, 3).map(_ * 2)
来源：http://zwv.havefunace.top

[T55] Scala：集合过滤
来源：http://zye.hammf.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pgv.yongpay.top

[T56] Scala：样例类
来源：http://bnm.zhaomingkeji.xyz

case class User(name: String, age: Int)
来源：http://nlo.daxiang520.top

[T57] Scala：模式匹配
来源：http://uyz.gotoacloud.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ouh.jinghuilouyu.cn

[T58] Scala：函数定义
来源：http://rur.sufxvd.cn

def add(a: Int, b: Int): Int = a + b
来源：http://usa.yj202588.top

[T59] Scala：循环
来源：http://bjq.0kj1m.cn

for (i <- 1 to 10) println(i)
来源：http://xtj.zhaomingkeji.xyz

[T60] Scala：折叠
来源：http://mpm.xuanzx.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ehs.xylfe.cn

================================================================================
来源：http://nza.ctjpmb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://snu.aizwys.cn

================================================================================
来源：http://kqr.gzhubu.top

[U01] Py：创建虚拟环境
来源：http://ewb.zdqjudy.top

python -m venv .venv && source .venv/bin/activate
来源：http://acs.yvedp.cn

[U02] Py：导出 / 安装依赖
来源：http://tnv.jinqigufen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bgh.hywenlv.cn

[U03] Py：加载 .env 配置
来源：http://fcf.zdqjudy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://gai.snrcjt.cn

[U04] Py：变量调试打印
来源：http://qwl.snrcjt.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rhg.jinyuanbaomall.cn

[U05] Py：列表去重且保序
来源：http://mol.ydzc1.top

list(dict.fromkeys(arr))
来源：http://plo.jlsjyb.cn

[U06] Py：合并两个字典
来源：http://acr.yongpay.top

{**a, **b}
来源：http://qxn.jqgufenzy.top

[U07] Py：反转字典键值
来源：http://mka.shuidangran.top

{v: k for k, v in d.items()}
来源：http://lmi.vqdsnc.cn

[U08] Py：展平二维列表
来源：http://bpg.uphjek.com

[y for x in nested for y in x]
来源：http://jtb.ctjpmb.com

[U09] Py：字典取最大值的键
来源：http://asi.hongshengwenyu.top

max(d, key=d.get)
来源：http://vuo.redwolf501.top

[U10] Py：按值排序字典
来源：http://imo.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uuh.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://vtc.yuanzhike.top

(x * 2 for x in arr)
来源：http://qdo.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://osc.yj202588.top

Counter(arr).most_common(3)
来源：http://zfg.yongpay.top

[U13] Py：固定长度队列
来源：http://kln.bbcook.cn

deque(maxlen=10)
来源：http://yny.ybcxt.top

[U14] Py：分组收集到列表
来源：http://lve.cheryme.top

defaultdict(list)
来源：http://peh.gotoacloud.top

[U15] Py：高精度计时
来源：http://chw.wangshuangyany.cn

t = time.perf_counter()
来源：http://zev.jinghuilouyu.cn

[U16] Py：命令行参数解析
来源：http://tsu.nanxuanxn.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xvx.hnxiangtu.top

[U17] Py：初始化日志
来源：http://pte.gzhubu.top

logging.basicConfig(level=logging.INFO)
来源：http://qcx.tarul.cn

[U18] Py：预编译正则
来源：http://kqk.yangfankeji.com

pat = re.compile(r"\d+")
来源：http://bks.gzhubu.top

[U19] Py：正则替换带回调
来源：http://sft.0kj1m.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jke.sjlbkw.cn

[U20] Py：缓存函数结果
来源：http://vgo.vqdsnc.cn

@functools.lru_cache(maxsize=None)
来源：http://nws.fehbvm.com

[U21] Py：自定义上下文管理器
来源：http://giu.hesvh.cn

@contextlib.contextmanager
来源：http://epv.fengsongda.top

[U22] Py：矩阵转置
来源：http://vwe.chenjidiqi.icu

list(zip(*m))
来源：http://kpf.smart0.xyz

[U23] Py：分块读取大文件
来源：http://uvk.tarul.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blt.fengsongda.top

[U24] Py：路径操作
来源：http://cai.mhx1999.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gkf.0kj1m.cn

[U25] Py：CSV 按字典读
来源：http://zen.snrcjt.cn

csv.DictReader(f)
来源：http://jdx.feifeiyinyue.top

[U26] Py：并发下载
来源：http://rfn.gaohongyu789.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bir.jinqigfzy.top

[U27] Py：异步 HTTP
来源：http://efy.yfazqb.com

aiohttp.ClientSession() 配合 async with
来源：http://xxp.bbcook.cn

[U28] Py：类型别名
来源：http://qhb.xinyue.icu

UserId = int
来源：http://dxz.wangdashe.top

[U29] Py：属性校验
来源：http://phy.gotoacloud.top

@property 与 @x.setter 配合
来源：http://mol.zhengqikj.top

[U30] Py：数据类
来源：http://jpr.quarkkingdee.top

@dataclass(slots=True)
来源：http://sie.tanke756.top

[U31] Py：单测
来源：http://wls.daxiang520.top

python -m pytest -q
来源：http://kvd.epnwcf.com

[U32] Py：代码格式化
来源：http://mdp.haohaochexian.top

ruff format . && ruff check --fix .
来源：http://vli.52xcode.cn

[U33] Py：打包发布
来源：http://tno.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://kst.xingfuxueyuan.xyz

[U34] Py：判断编码
来源：http://ovt.cashguo.top

chardet.detect(raw)
来源：http://tdr.birdmap.top

[U35] Py：发送邮件
来源：http://lcu.hcnkem.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ltj.nwbrower.top

[U36] Py：定时任务
来源：http://ayd.hfpthk.cn

schedule.every(10).minutes.do(job)
来源：http://wja.pycfn.com

[U37] Py：读写 Excel
来源：http://tgi.zhengqikj.top

pandas.read_excel / DataFrame.to_excel
来源：http://dhm.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://spl.andypj.xyz

Path(__file__).resolve().parent
来源：http://yig.tian-w.cn

[U39] Py：判断是否在交互环境
来源：http://rkt.gzhubu.top

sys.stdout.isatty()
来源：http://dbm.yanxiufei.cn

[U40] Py：打印到标准错误
来源：http://vlb.tanke756.top

print("err", file=sys.stderr)
来源：http://boc.yueranfly.top

[U41] PHP：初始化 Composer 项目
来源：http://vpx.yongpay.top

composer init;  composer require guzzlehttp/guzzle
来源：http://son.shuidangran.top

[U42] PHP：PSR-4 自动加载
来源：http://ftt.chenjidiqi.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tnq.bbcook.cn

[U43] PHP：声明命名空间
来源：http://ido.zhiwuduotai.top

namespace App\Http;
来源：http://aai.tarul.cn

[U44] PHP：开启严格类型
来源：http://qwi.iojbl.cn

declare(strict_types=1);
来源：http://zxq.yuxming.cn

[U45] PHP：类型声明与返回类型
来源：http://for.andypj.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://bcb.jiagoushi.top

[U46] PHP：可空类型
来源：http://irv.jinyuanbaomall.cn

?string $name = null
来源：http://jut.gaohongyu789.top

[U47] PHP：联合类型
来源：http://dng.kuanghao11.cn

int|string $id
来源：http://gdw.jianghu66.top

[U48] PHP：纯枚举
来源：http://xsu.nwbrower.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xip.jinyuanbaomall.cn

[U49] PHP：只读属性
来源：http://ape.yuxming.cn

public readonly string $name
来源：http://tcm.ivvv.top

[U50] PHP：构造器属性提升
来源：http://pyx.meibo888.top

public function __construct(private int $id) {}
来源：http://exp.9152youxi.cn

[U51] PHP：数组解构
来源：http://mcn.sufxvd.cn

[$a, $b] = $arr;
来源：http://xnv.jinqigfzy.top

[U52] PHP：箭头函数
来源：http://wxj.gotoacloud.top

$double = fn($x) => $x * 2;
来源：http://arl.yj202588.top

[U53] PHP：空合并运算符
来源：http://rpo.ydjk.org.cn

$v = $a ?? $b ?? "default";
来源：http://hjk.ctjpmb.com

[U54] PHP：空安全调用
来源：http://uwj.0kj1m.cn

$obj?->method()
来源：http://hrw.hfpthk.cn

[U55] PHP：match 表达式
来源：http://gnp.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tez.wangdashe.top

[U56] PHP：命名参数
来源：http://dsg.dianchejie.cn

f(a: 1, b: 2)
来源：http://eoa.jinghuilouyu.cn

[U57] PHP：字符串插值
来源：http://wkf.zdqjudy.top

"值: {$a}"
来源：http://csx.havefunace.top

[U58] PHP：数组三件套
来源：http://lau.dianchejie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rwg.zhixingplan.top

[U59] PHP：自定义排序
来源：http://gms.yj20258.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://psi.zycfv.cn

[U60] PHP：JSON 编解码
来源：http://zii.haohaochexian.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fep.jlsjyb.cn

[U61] PHP：正则
来源：http://njd.sysykeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hcc.52xcode.cn

[U62] PHP：日期对象
来源：http://yvx.ybcxt.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xxr.fanxiaobao.xyz

[U63] PHP：文件读写
来源：http://urg.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tqc.zhaomingkeji.xyz

[U64] PHP：目录遍历
来源：http://dgt.yueranfly.top

glob("dir/*.php");  scandir("dir");
来源：http://cvw.sxryk.cn

[U65] PHP：会话
来源：http://bvb.hammf.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://riz.vqdsnc.cn

[U66] PHP：设置 Cookie
来源：http://xfg.yongpay.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sbh.yj20258888.top

[U67] PHP：处理文件上传
来源：http://een.feifeiyinyue.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tci.zhijiandao.cn

[U68] PHP：PDO 连接
来源：http://prm.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://agf.xingfuxueyuan.xyz

[U69] PHP：PDO 预处理
来源：http://oeh.jinqigufen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dtr.vqdsnc.cn

[U70] PHP：PDO 事务
来源：http://pso.jqgfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pel.yonumen.top

[U71] PHP：抛出异常
来源：http://tbv.snrcjt.cn

throw new RuntimeException("失败", 500);
来源：http://ref.tarul.cn

[U72] PHP：写错误日志
来源：http://qss.gaohongyu789.top

error_log("失败: " . $e->getMessage());
来源：http://kqt.mhx1999.top

[U73] PHP：读取 ini 配置
来源：http://qje.tian-w.cn

parse_ini_file("config.ini", true)
来源：http://pia.pengpengdd.cyou

[U74] PHP：读取环境变量
来源：http://pye.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://fbq.hywenlv.cn

[U75] PHP：依赖注入
来源：http://qch.chenzaomai.com

composer require psr/container
来源：http://ouv.yuxming.cn

[U76] PHP：简单路由
来源：http://khh.chenjidiqi.icu

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hoe.shanyushiyangtech.top

[U77] PHP：模板渲染
来源：http://vpv.ppjwa.cn

composer require twig/twig
来源：http://ejr.aizwys.cn

[U78] PHP：单元测试
来源：http://xih.pycfn.com

composer require --dev phpunit/phpunit
来源：http://mkg.hywenlv.cn

[U79] PHP：静态分析
来源：http://bsh.iojbl.cn

composer require --dev phpstan/phpstan
来源：http://ayh.hfpthk.cn

[U80] PHP：代码规范修复
来源：http://yeo.gaohongyu789.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://smo.epnwcf.com

[U81] JS：初始化项目
来源：http://lor.jqgufenzy.top

npm init -y;  npm i express
来源：http://sqs.yvedp.cn

[U82] JS：package.json 脚本
来源：http://plm.yueranfly.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kpg.jinyuanbaomall.cn

[U83] JS：ES Module 导入导出
来源：http://pch.sxryk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tco.ppjwa.cn

[U84] JS：CommonJS 写法
来源：http://zsb.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bgv.hfpthk.cn

[U85] JS：可选链
来源：http://vku.iojbl.cn

a?.b?.c
来源：http://qqh.zdbjq.cn

[U86] JS：空值合并
来源：http://dna.quarkkingdee.top

a ?? b
来源：http://zzg.cashguo.top

[U87] JS：解构默认值
来源：http://unu.zhaomingkeji.xyz

const { a = 1, b = 2 } = obj;
来源：http://dqi.dashuyun.cn

[U88] JS：对象展开合并
来源：http://xit.ppjwa.cn

{ ...a, ...b }
来源：http://flx.snrcjt.cn

[U89] JS：数组去重
来源：http://gkg.fktsv.cn

[...new Set(arr)]
来源：http://krv.zhijiandao.cn

[U90] JS：数字数组排序
来源：http://adx.nanxuanxn.top

[...arr].sort((a, b) => a - b)
来源：http://lqu.yfazqb.com

[U91] JS：对象键值遍历
来源：http://tyi.quarkkingdee.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nlq.fanxiaobao.xyz

[U92] JS：深拷贝
来源：http://ktm.shzxlz.cn

structuredClone(obj)
来源：http://cbq.vehdjk.com

[U93] JS：模板字符串
来源：http://iwf.kuanghao11.cn

`共 ${n} 条`
来源：http://whp.fktsv.cn

[U94] JS：箭头函数
来源：http://mfa.chenlongwang.top

const double = x => x * 2;
来源：http://tfc.jlsjyb.cn

[U95] JS：Promise 包装
来源：http://fvq.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://izy.jqgufenzy.top

[U96] JS：async/await 与异常
来源：http://cpw.ydzc1.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zis.xinyue.icu

[U97] JS：并发请求
来源：http://wns.jianghu66.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://oie.andypj.xyz

[U98] JS：fetch 带 JSON
来源：http://axa.xuanzx.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ain.tian-w.cn

[U99] JS：事件监听
来源：http://ldz.jiagoushi.top

el.addEventListener("click", e => {})
来源：http://cwm.ivvv.top

[U100] JS：DOM 查询
来源：http://dcc.gogol.net.cn

document.querySelector(".item")
来源：http://ets.hnqzz.top

[U101] JS：classList 操作
来源：http://jgo.nanxuanxn.top

el.classList.toggle("active")
来源：http://zyc.chenzaomai.com

[U102] JS：本地存储
来源：http://zsg.sufxvd.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://krh.cashguo.top

[U103] JS：定时器
来源：http://uce.cashguo.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lmi.ctjpmb.com

[U104] JS：防抖
来源：http://yet.xylfe.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rwr.9152youxi.cn

[U105] JS：节流
来源：http://fpp.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mob.9152youxi.cn

[U106] JS：日期格式化
来源：http://ykk.wangdashe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lrh.zhengqikj.top

[U107] JS：数字千分位
来源：http://xif.ydjk.org.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vhm.jinqigfzy.top

[U108] JS：随机整数
来源：http://lhd.fktsv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dlt.ydjk.org.cn

[U109] JS：数组分组
来源：http://yml.yueranfly.top

Object.groupBy(arr, x => x.type)
来源：http://lrr.xuanzx.com

[U110] JS：数组分块
来源：http://van.yuxming.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hul.9152youxi.cn

[U111] JS：对象转 Map
来源：http://zsr.haohaochexian.top

new Map(Object.entries(obj))
来源：http://xxp.epnwcf.com

[U112] JS：字符串补位
来源：http://kly.svipenyu.cn

"7".padStart(3, "0")
来源：http://jru.cheryme.top

[U113] JS：正则替换全部
来源：http://ckw.vqdsnc.cn

s.replaceAll("a", "b")
来源：http://hto.chenzaomai.com

[U114] JS：JSON 深比较
来源：http://eni.hysaishi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vvh.sweek.top

[U115] JS：生成 UUID
来源：http://gor.yj20258888.top

crypto.randomUUID()
来源：http://dkw.guannengcc.top

[U116] JS：类型检查（JSDoc）
来源：http://dva.xuanzx.com

/** @param {string} name */ function f(name) {}
来源：http://ytu.iojbl.cn

[U117] JS：单元测试
来源：http://isj.birdmap.top

npm i -D vitest;  npx vitest
来源：http://wqj.hysaishi.cn

[U118] JS：开发服务器
来源：http://cfh.jinqigfzy.top

npm i -D vite;  npx vite
来源：http://iqs.yj20258888.top

[U119] JS：生产构建
来源：http://iny.zhoulong.xyz

npx vite build
来源：http://boe.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://xni.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://xtt.c1oappe.top

================================================================================
来源：http://rnl.mhx1999.top

统计汇总
来源：http://aws.jqgufenzy.top

================================================================================
来源：http://zat.yuanzhike.top

按语言统计（条）：
来源：http://wvg.jyoumei.cn


<!-- 参考信息 -->