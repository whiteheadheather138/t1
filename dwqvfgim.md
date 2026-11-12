代发 wailian999

[T31] Lua：Hello World
来源：http://ajw.shanyushiyangkeji.top

print("Hello")
来源：http://qgq.xuetiantiany.cn

[T32] Lua：局部变量
来源：http://sfc.xinyue.icu

local a = 1
来源：http://dez.yangfankeji.com

[T33] Lua：表（数组）
来源：http://pds.xuetiantiany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cvy.zhoulong.xyz

[T34] Lua：遍历表
来源：http://crt.jqgfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dwg.uphjek.com

[T35] Lua：字典表
来源：http://zoc.ybcxt.top

local d = { a = 1 };  d.b = 2
来源：http://eqg.yueranfly.top

[T36] Lua：函数
来源：http://efe.hammf.cn

function add(a, b) return a + b end
来源：http://dqp.vqdsnc.cn

[T37] Lua：字符串拼接
来源：http://wia.sweek.top

"a" .. "b"
来源：http://hlw.shanyushiyangtech.top

[T38] Lua：条件
来源：http://qof.wangdashe.top

if x > 0 then print("正") end
来源：http://efj.jqgfzy.top

[T39] Lua：模式匹配
来源：http://gwj.gotoacloud.top

string.find(s, "%d+")
来源：http://oft.shzxlz.cn

[T40] Lua：元表
来源：http://uam.sysykeji.top

setmetatable({}, { __index = base })
来源：http://wxv.yuanzhike.top

[T41] Perl：Hello World
来源：http://mgw.guowangkeji.top

print "Hello\n";
来源：http://irq.jinghuilouyu.cn

[T42] Perl：变量类型
来源：http://wqu.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zqp.xuanzx.com

[T43] Perl：字符串插值
来源：http://qaz.yj20258888.top

"值: $a"
来源：http://fpy.daxiang520.top

[T44] Perl：条件
来源：http://hxy.cucudq.cn

if ($a > 0) { print "正"; }
来源：http://cdu.jinqigfzy.top

[T45] Perl：数组遍历
来源：http://qpg.gaohongyu789.top

for my $x (@arr) { print $x; }
来源：http://oju.cucudq.cn

[T46] Perl：哈希操作
来源：http://zpn.cheryme.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fly.ehwqpu.com

[T47] Perl：正则捕获
来源：http://uoo.cashguo.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lvw.tian-w.cn

[T48] Perl：正则替换
来源：http://hka.ywan-chungtsiang.top

$s =~ s/old/new/g;
来源：http://yvc.ywan-chungtsiang.top

[T49] Perl：函数
来源：http://oqi.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mxj.shzxlz.cn

[T50] Perl：逐行读文件
来源：http://gaz.andypj.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://klq.xziqi.cn

while (my $line = <$fh>) { print $line; }
来源：http://exy.jqgufenzy.top

[T51] Scala：Hello World
来源：http://oye.yj20258.top

println("Hello")
来源：http://upc.wangshuangyany.cn

[T52] Scala：变量
来源：http://hfe.gogol.net.cn

val a = 1;  var b = 2
来源：http://prk.daxiang520.top

[T53] Scala：字符串插值
来源：http://jnj.chenlongwang.top

s"值: $b"
来源：http://iba.hesvh.cn

[T54] Scala：集合映射
来源：http://cij.xziqi.cn

List(1, 2, 3).map(_ * 2)
来源：http://rgy.chenzaomai.com

[T55] Scala：集合过滤
来源：http://vdg.mhx1999.top

List(1, 2, 3).filter(_ > 1)
来源：http://qcf.cdnleiting.top

[T56] Scala：样例类
来源：http://yop.xuanzx.com

case class User(name: String, age: Int)
来源：http://wsp.cdnleiting.top

[T57] Scala：模式匹配
来源：http://cgc.cucudq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tnm.yuanzhike.top

[T58] Scala：函数定义
来源：http://bdi.jqgufenzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://huj.havefunace.top

[T59] Scala：循环
来源：http://baw.gogol.net.cn

for (i <- 1 to 10) println(i)
来源：http://pfv.52xcode.cn

[T60] Scala：折叠
来源：http://jyv.vqdsnc.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dtg.cqqwz.cn

================================================================================
来源：http://wqp.hfpthk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ilu.yanxiufei.cn

================================================================================
来源：http://rcu.gotoacloud.top

[U01] Py：创建虚拟环境
来源：http://rvm.bbcook.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fyo.mhx1999.top

[U02] Py：导出 / 安装依赖
来源：http://fqy.zhijiandao.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cvy.316326.xyz

[U03] Py：加载 .env 配置
来源：http://rav.bjfxy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://emk.tarul.cn

[U04] Py：变量调试打印
来源：http://ozl.jinqigufen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nty.shanyushiyangtech.top

[U05] Py：列表去重且保序
来源：http://huj.bjfxy.top

list(dict.fromkeys(arr))
来源：http://tdx.jinqigufen.top

[U06] Py：合并两个字典
来源：http://bkm.sufxvd.cn

{**a, **b}
来源：http://gdo.hcnkem.com

[U07] Py：反转字典键值
来源：http://saq.fehbvm.com

{v: k for k, v in d.items()}
来源：http://gin.cucudq.cn

[U08] Py：展平二维列表
来源：http://wfd.iojbl.cn

[y for x in nested for y in x]
来源：http://brt.guowangkeji.top

[U09] Py：字典取最大值的键
来源：http://cxa.yongpay.top

max(d, key=d.get)
来源：http://vpw.fehbvm.com

[U10] Py：按值排序字典
来源：http://yel.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qrb.nanxuanxn.top

[U11] Py：生成器表达式
来源：http://sjd.yangfankeji.com

(x * 2 for x in arr)
来源：http://igw.andypj.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://tiz.jinghuilouyu.cn

Counter(arr).most_common(3)
来源：http://nuh.guannengcc.top

[U13] Py：固定长度队列
来源：http://dkz.wangdashe.top

deque(maxlen=10)
来源：http://cep.haohaochexian.top

[U14] Py：分组收集到列表
来源：http://one.ydjk.org.cn

defaultdict(list)
来源：http://qkc.shzxlz.cn

[U15] Py：高精度计时
来源：http://pjs.xuanzx.com

t = time.perf_counter()
来源：http://eul.yuxming.cn

[U16] Py：命令行参数解析
来源：http://cfn.hywenlv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://clc.shzxlz.cn

[U17] Py：初始化日志
来源：http://cxe.daria6918.cn

logging.basicConfig(level=logging.INFO)
来源：http://mey.shangyingyoupin.top

[U18] Py：预编译正则
来源：http://txy.nanxuanxn.top

pat = re.compile(r"\d+")
来源：http://ebb.gaohongyu789.top

[U19] Py：正则替换带回调
来源：http://ouq.daxiang520.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pnf.sweek.top

[U20] Py：缓存函数结果
来源：http://whv.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://xdz.mhx1999.top

[U21] Py：自定义上下文管理器
来源：http://vft.ydjk.org.cn

@contextlib.contextmanager
来源：http://nwn.yj202588.top

[U22] Py：矩阵转置
来源：http://szx.fzhhl.top

list(zip(*m))
来源：http://bpb.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://goi.fanxiaobao.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://knd.aibaodan.cn

[U24] Py：路径操作
来源：http://eou.chenlongwang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://flp.sysykeji.top

[U25] Py：CSV 按字典读
来源：http://ykg.jinyuanbaomall.cn

csv.DictReader(f)
来源：http://xin.daxiang520.top

[U26] Py：并发下载
来源：http://yzt.ctjpmb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://owr.hnxiangtu.top

[U27] Py：异步 HTTP
来源：http://xzo.zhiwuduotai.top

aiohttp.ClientSession() 配合 async with
来源：http://atc.fehbvm.com

[U28] Py：类型别名
来源：http://kyk.jiagoushi.top

UserId = int
来源：http://jhy.fktsv.cn

[U29] Py：属性校验
来源：http://vza.jyoumei.cn

@property 与 @x.setter 配合
来源：http://jpf.jinqigufen.top

[U30] Py：数据类
来源：http://sox.jlsjyb.cn

@dataclass(slots=True)
来源：http://hqn.fktsv.cn

[U31] Py：单测
来源：http://eid.nwbrower.top

python -m pytest -q
来源：http://gwh.cashguo.top

[U32] Py：代码格式化
来源：http://xgn.shanyushiyangkeji.top

ruff format . && ruff check --fix .
来源：http://ujo.sxryk.cn

[U33] Py：打包发布
来源：http://lij.feifeiyinyue.top

python -m build  （依赖 pyproject.toml）
来源：http://wso.nwbrower.top

[U34] Py：判断编码
来源：http://kcy.c1oappe.top

chardet.detect(raw)
来源：http://pne.jlsjyb.cn

[U35] Py：发送邮件
来源：http://mrg.ydzc1.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qcp.feifeiyinyue.top

[U36] Py：定时任务
来源：http://plu.0kj1m.cn

schedule.every(10).minutes.do(job)
来源：http://qfh.jinghuilouyu.cn

[U37] Py：读写 Excel
来源：http://ukn.snrcjt.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dly.dashuyun.cn

[U38] Py：获取脚本所在目录
来源：http://ebz.cheryme.top

Path(__file__).resolve().parent
来源：http://ssx.uphjek.com

[U39] Py：判断是否在交互环境
来源：http://glo.havefunace.top

sys.stdout.isatty()
来源：http://hrn.ywan-chungtsiang.top

[U40] Py：打印到标准错误
来源：http://fmo.dianchejie.cn

print("err", file=sys.stderr)
来源：http://xdy.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://odx.gogol.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ujy.hfpthk.cn

[U42] PHP：PSR-4 自动加载
来源：http://ezk.redwolf501.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xmm.chenlongwang.top

[U43] PHP：声明命名空间
来源：http://uqh.dianchejie.cn

namespace App\Http;
来源：http://crq.jqgufenzy.top

[U44] PHP：开启严格类型
来源：http://chs.dashuyun.cn

declare(strict_types=1);
来源：http://igj.cashguo.top

[U45] PHP：类型声明与返回类型
来源：http://jrd.jqgfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lgu.9152youxi.cn

[U46] PHP：可空类型
来源：http://iba.yanxiufei.cn

?string $name = null
来源：http://dxm.xuetiantiany.cn

[U47] PHP：联合类型
来源：http://pcz.hesvh.cn

int|string $id
来源：http://wnf.yanxiufei.cn

[U48] PHP：纯枚举
来源：http://oda.quarkkingdee.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qzd.fengsongda.top

[U49] PHP：只读属性
来源：http://hyv.fengsongda.top

public readonly string $name
来源：http://jxd.daria6918.cn

[U50] PHP：构造器属性提升
来源：http://arv.jinyuanbaomall.cn

public function __construct(private int $id) {}
来源：http://zoz.cqqwz.cn

[U51] PHP：数组解构
来源：http://xya.cucudq.cn

[$a, $b] = $arr;
来源：http://qsd.svipenyu.cn

[U52] PHP：箭头函数
来源：http://eqm.xinyue.icu

$double = fn($x) => $x * 2;
来源：http://zhf.yvedp.cn

[U53] PHP：空合并运算符
来源：http://qah.zdqjudy.top

$v = $a ?? $b ?? "default";
来源：http://inx.hcnkem.com

[U54] PHP：空安全调用
来源：http://obh.tian-w.cn

$obj?->method()
来源：http://kzw.316326.xyz

[U55] PHP：match 表达式
来源：http://rpx.316326.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uba.epnwcf.com

[U56] PHP：命名参数
来源：http://iiy.vehdjk.com

f(a: 1, b: 2)
来源：http://hdr.sxryk.cn

[U57] PHP：字符串插值
来源：http://tte.vehdjk.com

"值: {$a}"
来源：http://huh.uphjek.com

[U58] PHP：数组三件套
来源：http://sln.andypj.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lqo.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://bdj.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qaw.tarul.cn

[U60] PHP：JSON 编解码
来源：http://uoi.xingfuxueyuan.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fgm.gzhubu.top

[U61] PHP：正则
来源：http://fox.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gla.zhengqikj.top

[U62] PHP：日期对象
来源：http://ing.ppjwa.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dqa.xuanzx.com

[U63] PHP：文件读写
来源：http://aed.chenlongwang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yiz.chenjidiqi.icu

[U64] PHP：目录遍历
来源：http://dyn.vehdjk.com

glob("dir/*.php");  scandir("dir");
来源：http://mhk.gzhubu.top

[U65] PHP：会话
来源：http://qce.tianlin.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://oky.hcnkem.com

[U66] PHP：设置 Cookie
来源：http://eab.fktsv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rys.fzhhl.top

[U67] PHP：处理文件上传
来源：http://uto.pycfn.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ixa.yfazqb.com

[U68] PHP：PDO 连接
来源：http://pxo.jlsjyb.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ztb.aibaodan.cn

[U69] PHP：PDO 预处理
来源：http://ajm.guannengcc.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jud.ywan-chungtsiang.top

[U70] PHP：PDO 事务
来源：http://piu.zhaomingkeji.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cwa.tianlin.xyz

[U71] PHP：抛出异常
来源：http://zpq.ehwqpu.com

throw new RuntimeException("失败", 500);
来源：http://zxu.cucudq.cn

[U72] PHP：写错误日志
来源：http://lwc.chenlongwang.top

error_log("失败: " . $e->getMessage());
来源：http://ewb.zhengqikj.top

[U73] PHP：读取 ini 配置
来源：http://kaq.yonumen.top

parse_ini_file("config.ini", true)
来源：http://axn.ivvv.top

[U74] PHP：读取环境变量
来源：http://qdr.zhijiandao.cn

getenv("APP_ENV") ?: "production"
来源：http://ezq.jyoumei.cn

[U75] PHP：依赖注入
来源：http://xom.ehwqpu.com

composer require psr/container
来源：http://org.hnxiangtu.top

[U76] PHP：简单路由
来源：http://nbl.ppjwa.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uqq.smart0.xyz

[U77] PHP：模板渲染
来源：http://zwd.sjlbkw.cn

composer require twig/twig
来源：http://dkz.shuidangran.top

[U78] PHP：单元测试
来源：http://sdg.daxiang520.top

composer require --dev phpunit/phpunit
来源：http://gsv.hnxiangtu.top

[U79] PHP：静态分析
来源：http://pmt.shanyushiyangkeji.top

composer require --dev phpstan/phpstan
来源：http://hru.nanxinkj.top

[U80] PHP：代码规范修复
来源：http://cyd.redwolf501.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wtk.zhiwuduotai.top

[U81] JS：初始化项目
来源：http://kbp.zdqjudy.top

npm init -y;  npm i express
来源：http://wuh.jyoumei.cn

[U82] JS：package.json 脚本
来源：http://hfp.yangfankeji.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zsn.guowangkeji.top

[U83] JS：ES Module 导入导出
来源：http://hkq.bbcook.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dhs.zhoulong.xyz

[U84] JS：CommonJS 写法
来源：http://xup.ehwqpu.com

module.exports = { a };  const { a } = require("./m");
来源：http://smg.havefunace.top

[U85] JS：可选链
来源：http://dva.yvedp.cn

a?.b?.c
来源：http://ykh.hongshengwenyu.top

[U86] JS：空值合并
来源：http://rxf.havefunace.top

a ?? b
来源：http://qkz.xylfe.cn

[U87] JS：解构默认值
来源：http://ajk.daxiang520.top

const { a = 1, b = 2 } = obj;
来源：http://quw.fengsongda.top

[U88] JS：对象展开合并
来源：http://xjq.hfpthk.cn

{ ...a, ...b }
来源：http://kzz.cashguo.top

[U89] JS：数组去重
来源：http://fho.tian-w.cn

[...new Set(arr)]
来源：http://yki.gaohongyu789.top

[U90] JS：数字数组排序
来源：http://ivx.hfpthk.cn

[...arr].sort((a, b) => a - b)
来源：http://xxg.zhiwuduotai.top

[U91] JS：对象键值遍历
来源：http://jkh.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hxm.snrcjt.cn

[U92] JS：深拷贝
来源：http://yrp.cucudq.cn

structuredClone(obj)
来源：http://zwy.sysykeji.top

[U93] JS：模板字符串
来源：http://pzf.yj20258888.top

`共 ${n} 条`
来源：http://byi.chenjidiqi.icu

[U94] JS：箭头函数
来源：http://akx.xuanzx.com

const double = x => x * 2;
来源：http://jxx.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://rfi.sysykeji.top

new Promise((resolve, reject) => {})
来源：http://yza.hcnkem.com

[U96] JS：async/await 与异常
来源：http://nmd.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uup.zhoulong.xyz

[U97] JS：并发请求
来源：http://nsj.pengpengdd.cyou

await Promise.all(urls.map(u => fetch(u)))
来源：http://sbj.chenlongwang.top

[U98] JS：fetch 带 JSON
来源：http://xya.chenjidiqi.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fos.yangfankeji.com

[U99] JS：事件监听
来源：http://zly.iojbl.cn

el.addEventListener("click", e => {})
来源：http://ktu.fzhhl.top

[U100] JS：DOM 查询
来源：http://ejm.daria6918.cn

document.querySelector(".item")
来源：http://spo.smart0.xyz

[U101] JS：classList 操作
来源：http://ave.uphjek.com

el.classList.toggle("active")
来源：http://rob.sysykeji.top

[U102] JS：本地存储
来源：http://yvb.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hhy.yanxiufei.cn

[U103] JS：定时器
来源：http://pgs.haohaochexian.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kjq.zycfv.cn

[U104] JS：防抖
来源：http://tpw.hywenlv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pfm.chenzaomai.com

[U105] JS：节流
来源：http://syo.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://usb.yongpay.top

[U106] JS：日期格式化
来源：http://bbt.hongshengwenyu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rfi.gogol.net.cn

[U107] JS：数字千分位
来源：http://oex.iojbl.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ocb.cucudq.cn

[U108] JS：随机整数
来源：http://qtq.svipenyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rbl.zdbjq.cn

[U109] JS：数组分组
来源：http://hwe.shuidangran.top

Object.groupBy(arr, x => x.type)
来源：http://dzc.hnxiangtu.top

[U110] JS：数组分块
来源：http://hwg.jlsjyb.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://twp.ppjwa.cn

[U111] JS：对象转 Map
来源：http://ryp.daxiang520.top

new Map(Object.entries(obj))
来源：http://lxd.sxryk.cn

[U112] JS：字符串补位
来源：http://hwr.xuanzx.com

"7".padStart(3, "0")
来源：http://jac.zhiwuduotai.top

[U113] JS：正则替换全部
来源：http://fjr.yj20258888.top

s.replaceAll("a", "b")
来源：http://vka.pycfn.com

[U114] JS：JSON 深比较
来源：http://whb.gaohongyu789.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bpe.wangdashe.top

[U115] JS：生成 UUID
来源：http://bry.cqqwz.cn

crypto.randomUUID()
来源：http://ybe.guowangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://fhr.hesvh.cn

/** @param {string} name */ function f(name) {}
来源：http://yel.xuanzx.com

[U117] JS：单元测试
来源：http://zle.wangdashe.top

npm i -D vitest;  npx vitest
来源：http://nln.chenjidiqi.icu

[U118] JS：开发服务器
来源：http://quo.zhengqikj.top

npm i -D vite;  npx vite
来源：http://fau.chenlongwang.top


<!-- 参考信息 -->