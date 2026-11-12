代发 wailian999

[T35] Lua：字典表
来源：http://zfb.sxryk.cn

local d = { a = 1 };  d.b = 2
来源：http://djv.shangyingyoupin.top

[T36] Lua：函数
来源：http://ufr.yuanzhike.top

function add(a, b) return a + b end
来源：http://geo.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://skt.sufxvd.cn

"a" .. "b"
来源：http://eeg.cashguo.top

[T38] Lua：条件
来源：http://yzq.ydjk.org.cn

if x > 0 then print("正") end
来源：http://ekn.pycfn.com

[T39] Lua：模式匹配
来源：http://hcp.hywenlv.cn

string.find(s, "%d+")
来源：http://gnz.hcnkem.com

[T40] Lua：元表
来源：http://lwc.yj20258888.top

setmetatable({}, { __index = base })
来源：http://euu.yonumen.top

[T41] Perl：Hello World
来源：http://ret.epnwcf.com

print "Hello\n";
来源：http://oev.yj202588.top

[T42] Perl：变量类型
来源：http://jkq.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://psm.zhixingplan.top

[T43] Perl：字符串插值
来源：http://nuv.jlsjyb.cn

"值: $a"
来源：http://gpb.havefunace.top

[T44] Perl：条件
来源：http://gxr.zhoulong.xyz

if ($a > 0) { print "正"; }
来源：http://vrs.hnxiangtu.top

[T45] Perl：数组遍历
来源：http://akx.cashguo.top

for my $x (@arr) { print $x; }
来源：http://kyy.nanxuanxn.top

[T46] Perl：哈希操作
来源：http://fnr.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jeq.sweek.top

[T47] Perl：正则捕获
来源：http://pih.vqdsnc.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://smi.gotoacloud.top

[T48] Perl：正则替换
来源：http://kzn.fzhhl.top

$s =~ s/old/new/g;
来源：http://ehc.jinyuanbaomall.cn

[T49] Perl：函数
来源：http://pxy.9152youxi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iyc.jinqigufen.top

[T50] Perl：逐行读文件
来源：http://cfn.jiagoushi.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dkc.yvedp.cn

while (my $line = <$fh>) { print $line; }
来源：http://kof.guannengcc.top

[T51] Scala：Hello World
来源：http://wjx.sysykeji.top

println("Hello")
来源：http://rni.daxiang520.top

[T52] Scala：变量
来源：http://wms.quarkkingdee.top

val a = 1;  var b = 2
来源：http://oxb.fehbvm.com

[T53] Scala：字符串插值
来源：http://iwo.yvedp.cn

s"值: $b"
来源：http://umv.gotoacloud.top

[T54] Scala：集合映射
来源：http://bdh.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://fyh.gotoacloud.top

[T55] Scala：集合过滤
来源：http://zcn.zhixingplan.top

List(1, 2, 3).filter(_ > 1)
来源：http://ogp.vehdjk.com

[T56] Scala：样例类
来源：http://yxe.ydjk.org.cn

case class User(name: String, age: Int)
来源：http://dvm.haohaochexian.top

[T57] Scala：模式匹配
来源：http://ujs.zhixingplan.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sqg.xuanzx.com

[T58] Scala：函数定义
来源：http://ezx.feifeiyinyue.top

def add(a: Int, b: Int): Int = a + b
来源：http://awo.cucudq.cn

[T59] Scala：循环
来源：http://hty.wangshuangyany.cn

for (i <- 1 to 10) println(i)
来源：http://flx.tian-w.cn

[T60] Scala：折叠
来源：http://ley.ywan-chungtsiang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ijx.jyoumei.cn

================================================================================
来源：http://qjs.jiagoushi.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ptj.smart0.xyz

================================================================================
来源：http://xdf.gzhubu.top

[U01] Py：创建虚拟环境
来源：http://kzu.dianchejie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qty.hysaishi.cn

[U02] Py：导出 / 安装依赖
来源：http://atm.kuanghao11.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zpy.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://ibm.xingfuxueyuan.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://xha.xuetiantiany.cn

[U04] Py：变量调试打印
来源：http://ysl.jiagoushi.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ypy.shzxlz.cn

[U05] Py：列表去重且保序
来源：http://zuv.hammf.cn

list(dict.fromkeys(arr))
来源：http://ncv.sxryk.cn

[U06] Py：合并两个字典
来源：http://glb.ppjwa.cn

{**a, **b}
来源：http://stz.jinqigfzy.top

[U07] Py：反转字典键值
来源：http://zwx.guowangkeji.top

{v: k for k, v in d.items()}
来源：http://jpx.yangfankeji.com

[U08] Py：展平二维列表
来源：http://vig.cheryme.top

[y for x in nested for y in x]
来源：http://nhn.gzhubu.top

[U09] Py：字典取最大值的键
来源：http://dcf.xuanzx.com

max(d, key=d.get)
来源：http://hjo.nanxuanxn.top

[U10] Py：按值排序字典
来源：http://dqy.sjlbkw.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lvp.yuxming.cn

[U11] Py：生成器表达式
来源：http://han.andypj.xyz

(x * 2 for x in arr)
来源：http://mhc.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ger.jinqigfzy.top

Counter(arr).most_common(3)
来源：http://fcz.zhaomingkeji.xyz

[U13] Py：固定长度队列
来源：http://art.yj202588.top

deque(maxlen=10)
来源：http://jtf.hfpthk.cn

[U14] Py：分组收集到列表
来源：http://uif.shuidangran.top

defaultdict(list)
来源：http://wul.cucudq.cn

[U15] Py：高精度计时
来源：http://uux.zdbjq.cn

t = time.perf_counter()
来源：http://hkf.yangfankeji.com

[U16] Py：命令行参数解析
来源：http://mjs.smart0.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pgp.chenjidiqi.icu

[U17] Py：初始化日志
来源：http://pqr.yonumen.top

logging.basicConfig(level=logging.INFO)
来源：http://hdx.fehbvm.com

[U18] Py：预编译正则
来源：http://wgp.0kj1m.cn

pat = re.compile(r"\d+")
来源：http://uun.jqgufenzy.top

[U19] Py：正则替换带回调
来源：http://lrr.yfazqb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yfb.yuanzhike.top

[U20] Py：缓存函数结果
来源：http://ohg.fzhhl.top

@functools.lru_cache(maxsize=None)
来源：http://dlj.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://ych.yvedp.cn

@contextlib.contextmanager
来源：http://mcl.yuxming.cn

[U22] Py：矩阵转置
来源：http://uax.zhaomingkeji.xyz

list(zip(*m))
来源：http://guz.hammf.cn

[U23] Py：分块读取大文件
来源：http://qsy.shanyushiyangtech.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://huf.redwolf501.top

[U24] Py：路径操作
来源：http://rxb.ydzc1.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gbc.ydzc1.top

[U25] Py：CSV 按字典读
来源：http://xkk.shuidangran.top

csv.DictReader(f)
来源：http://skr.aibaodan.cn

[U26] Py：并发下载
来源：http://nbd.haohaochexian.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cwe.jinyuanbaomall.cn

[U27] Py：异步 HTTP
来源：http://udt.hcnkem.com

aiohttp.ClientSession() 配合 async with
来源：http://zfz.wangdashe.top

[U28] Py：类型别名
来源：http://rpk.gogol.net.cn

UserId = int
来源：http://vyy.ydzc1.top

[U29] Py：属性校验
来源：http://tig.xingfuxueyuan.xyz

@property 与 @x.setter 配合
来源：http://ppn.dianchejie.cn

[U30] Py：数据类
来源：http://wed.bjfxy.top

@dataclass(slots=True)
来源：http://wsc.cashguo.top

[U31] Py：单测
来源：http://blr.daria6918.cn

python -m pytest -q
来源：http://xth.gaohongyu789.top

[U32] Py：代码格式化
来源：http://rlh.ehwqpu.com

ruff format . && ruff check --fix .
来源：http://xki.yonumen.top

[U33] Py：打包发布
来源：http://kst.yongpay.top

python -m build  （依赖 pyproject.toml）
来源：http://vhf.epnwcf.com

[U34] Py：判断编码
来源：http://zmw.tanke756.top

chardet.detect(raw)
来源：http://fqy.cdnleiting.top

[U35] Py：发送邮件
来源：http://tpu.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nry.ivvv.top

[U36] Py：定时任务
来源：http://ivk.jianghu66.top

schedule.every(10).minutes.do(job)
来源：http://xzf.vqdsnc.cn

[U37] Py：读写 Excel
来源：http://pzb.jiagoushi.top

pandas.read_excel / DataFrame.to_excel
来源：http://osv.zhiwuduotai.top

[U38] Py：获取脚本所在目录
来源：http://pym.hongshengwenyu.top

Path(__file__).resolve().parent
来源：http://lbk.cucudq.cn

[U39] Py：判断是否在交互环境
来源：http://dga.ybcxt.top

sys.stdout.isatty()
来源：http://old.cashguo.top

[U40] Py：打印到标准错误
来源：http://lhw.jqgufenzy.top

print("err", file=sys.stderr)
来源：http://noa.guannengcc.top

[U41] PHP：初始化 Composer 项目
来源：http://wfa.chenzaomai.com

composer init;  composer require guzzlehttp/guzzle
来源：http://ubg.nanxuanxn.top

[U42] PHP：PSR-4 自动加载
来源：http://nwq.fengsongda.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ncm.yonumen.top

[U43] PHP：声明命名空间
来源：http://rmg.smart0.xyz

namespace App\Http;
来源：http://por.cashguo.top

[U44] PHP：开启严格类型
来源：http://han.daria6918.cn

declare(strict_types=1);
来源：http://bpr.hnqzz.top

[U45] PHP：类型声明与返回类型
来源：http://wrm.jlsjyb.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fom.nwbrower.top

[U46] PHP：可空类型
来源：http://yip.snrcjt.cn

?string $name = null
来源：http://qeu.vehdjk.com

[U47] PHP：联合类型
来源：http://fec.ppjwa.cn

int|string $id
来源：http://wgo.jinqigufen.top

[U48] PHP：纯枚举
来源：http://arg.yongpay.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zgg.cdnleiting.top

[U49] PHP：只读属性
来源：http://hgd.sxryk.cn

public readonly string $name
来源：http://qsl.shuidangran.top

[U50] PHP：构造器属性提升
来源：http://yyg.cqqwz.cn

public function __construct(private int $id) {}
来源：http://goo.zhijiandao.cn

[U51] PHP：数组解构
来源：http://wau.fzhhl.top

[$a, $b] = $arr;
来源：http://tmv.yueranfly.top

[U52] PHP：箭头函数
来源：http://jgt.zhiwuduotai.top

$double = fn($x) => $x * 2;
来源：http://iyd.gaohongyu789.top

[U53] PHP：空合并运算符
来源：http://kpf.xingfuxueyuan.xyz

$v = $a ?? $b ?? "default";
来源：http://pdu.yfazqb.com

[U54] PHP：空安全调用
来源：http://gfm.ydzc1.top

$obj?->method()
来源：http://zet.havefunace.top

[U55] PHP：match 表达式
来源：http://dwe.xingfuxueyuan.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uiu.yueranfly.top

[U56] PHP：命名参数
来源：http://ukx.ivvv.top

f(a: 1, b: 2)
来源：http://jxf.xuetiantiany.cn

[U57] PHP：字符串插值
来源：http://svn.daria6918.cn

"值: {$a}"
来源：http://wro.hnqzz.top

[U58] PHP：数组三件套
来源：http://bjf.gzhubu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hhu.hywenlv.cn

[U59] PHP：自定义排序
来源：http://pxz.xingfuxueyuan.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oeg.yfazqb.com

[U60] PHP：JSON 编解码
来源：http://swj.jinqigufen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qsp.jinqigfzy.top

[U61] PHP：正则
来源：http://hfl.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dcq.ppjwa.cn

[U62] PHP：日期对象
来源：http://aew.hywenlv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xay.hammf.cn

[U63] PHP：文件读写
来源：http://lmo.316326.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qzb.dashuyun.cn

[U64] PHP：目录遍历
来源：http://isx.gotoacloud.top

glob("dir/*.php");  scandir("dir");
来源：http://smu.aizwys.cn

[U65] PHP：会话
来源：http://tnu.sysykeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://edo.shanyushiyangkeji.top

[U66] PHP：设置 Cookie
来源：http://wgq.fehbvm.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nzg.svipenyu.cn

[U67] PHP：处理文件上传
来源：http://iwm.bbcook.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dci.jlsjyb.cn

[U68] PHP：PDO 连接
来源：http://cxn.zhengqikj.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wts.fanxiaobao.xyz

[U69] PHP：PDO 预处理
来源：http://mru.c1oappe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dvf.gogol.net.cn

[U70] PHP：PDO 事务
来源：http://cyh.chenlongwang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ojf.hywenlv.cn

[U71] PHP：抛出异常
来源：http://jgd.chenzaomai.com

throw new RuntimeException("失败", 500);
来源：http://lnq.shanyushiyangkeji.top

[U72] PHP：写错误日志
来源：http://scd.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://jmt.c1oappe.top

[U73] PHP：读取 ini 配置
来源：http://msq.jinqigufen.top

parse_ini_file("config.ini", true)
来源：http://aua.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://eyz.nanxuanxn.top

getenv("APP_ENV") ?: "production"
来源：http://rcm.smart0.xyz

[U75] PHP：依赖注入
来源：http://btp.zhaomingkeji.xyz

composer require psr/container
来源：http://ori.dashuyun.cn

[U76] PHP：简单路由
来源：http://phh.shzxlz.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://thh.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://kvv.ybcxt.top

composer require twig/twig
来源：http://roh.shanyushiyangkeji.top

[U78] PHP：单元测试
来源：http://jna.zdbjq.cn

composer require --dev phpunit/phpunit
来源：http://dgh.xziqi.cn

[U79] PHP：静态分析
来源：http://nja.ywan-chungtsiang.top

composer require --dev phpstan/phpstan
来源：http://coj.yuxming.cn

[U80] PHP：代码规范修复
来源：http://xrl.chenlongwang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://slq.fengsongda.top

[U81] JS：初始化项目
来源：http://lsp.iojbl.cn

npm init -y;  npm i express
来源：http://tmz.tian-w.cn

[U82] JS：package.json 脚本
来源：http://bcu.shanyushiyangtech.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xqf.snrcjt.cn

[U83] JS：ES Module 导入导出
来源：http://yyr.uphjek.com

export const a = 1;  import { a } from "./m.js";
来源：http://ucm.jinqigufen.top

[U84] JS：CommonJS 写法
来源：http://tlm.yangfankeji.com

module.exports = { a };  const { a } = require("./m");
来源：http://tsd.chenjidiqi.icu

[U85] JS：可选链
来源：http://qht.sxryk.cn

a?.b?.c
来源：http://rfj.vqdsnc.cn

[U86] JS：空值合并
来源：http://ggc.jinqigfzy.top

a ?? b
来源：http://nwu.hnqzz.top

[U87] JS：解构默认值
来源：http://qot.redwolf501.top

const { a = 1, b = 2 } = obj;
来源：http://nwy.nwbrower.top

[U88] JS：对象展开合并
来源：http://tjw.tanke756.top

{ ...a, ...b }
来源：http://urn.9152youxi.cn

[U89] JS：数组去重
来源：http://fxq.zdqjudy.top

[...new Set(arr)]
来源：http://etj.yvedp.cn

[U90] JS：数字数组排序
来源：http://oxg.jlsjyb.cn

[...arr].sort((a, b) => a - b)
来源：http://ool.jinyuanbaomall.cn

[U91] JS：对象键值遍历
来源：http://qnn.yj202588.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cac.gogol.net.cn

[U92] JS：深拷贝
来源：http://rgu.gzhubu.top

structuredClone(obj)
来源：http://bje.fktsv.cn

[U93] JS：模板字符串
来源：http://spx.xinyue.icu

`共 ${n} 条`
来源：http://cfo.zycfv.cn

[U94] JS：箭头函数
来源：http://tvk.jianghu66.top

const double = x => x * 2;
来源：http://ybg.fehbvm.com

[U95] JS：Promise 包装
来源：http://zdn.havefunace.top

new Promise((resolve, reject) => {})
来源：http://ofw.hammf.cn

[U96] JS：async/await 与异常
来源：http://cup.quarkkingdee.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xgv.gzhubu.top

[U97] JS：并发请求
来源：http://bsf.chenlongwang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kxu.jlsjyb.cn

[U98] JS：fetch 带 JSON
来源：http://wqj.svipenyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rnd.cashguo.top

[U99] JS：事件监听
来源：http://kue.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://erl.shangyingyoupin.top

[U100] JS：DOM 查询
来源：http://goa.gaohongyu789.top

document.querySelector(".item")
来源：http://xpd.zhiwuduotai.top

[U101] JS：classList 操作
来源：http://nbo.pycfn.com

el.classList.toggle("active")
来源：http://tcs.nanxuanxn.top

[U102] JS：本地存储
来源：http://axa.redwolf501.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://chc.ivvv.top

[U103] JS：定时器
来源：http://uhn.ppjwa.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vhg.fengsongda.top

[U104] JS：防抖
来源：http://nkg.ydzc1.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://puc.iojbl.cn

[U105] JS：节流
来源：http://uis.xuanzx.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dwq.hnqzz.top

[U106] JS：日期格式化
来源：http://uas.andypj.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://czy.ydjk.org.cn

[U107] JS：数字千分位
来源：http://tzd.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://piq.sufxvd.cn

[U108] JS：随机整数
来源：http://szg.pengpengdd.cyou

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nol.zhiwuduotai.top

[U109] JS：数组分组
来源：http://def.sufxvd.cn

Object.groupBy(arr, x => x.type)
来源：http://vrk.zhoulong.xyz

[U110] JS：数组分块
来源：http://bnu.bbcook.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cuk.gogol.net.cn

[U111] JS：对象转 Map
来源：http://xth.xuetiantiany.cn

new Map(Object.entries(obj))
来源：http://dqe.chenjidiqi.icu

[U112] JS：字符串补位
来源：http://oau.316326.xyz

"7".padStart(3, "0")
来源：http://abm.jqgfzy.top

[U113] JS：正则替换全部
来源：http://edh.sysykeji.top

s.replaceAll("a", "b")
来源：http://vpw.xuanzx.com

[U114] JS：JSON 深比较
来源：http://rmv.fzhhl.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dxq.zhiwuduotai.top

[U115] JS：生成 UUID
来源：http://ivz.ybcxt.top

crypto.randomUUID()
来源：http://ehk.jiagoushi.top

[U116] JS：类型检查（JSDoc）
来源：http://fkx.316326.xyz

/** @param {string} name */ function f(name) {}
来源：http://zuq.dashuyun.cn

[U117] JS：单元测试
来源：http://rgb.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://qng.yuxming.cn

[U118] JS：开发服务器
来源：http://btn.mhx1999.top

npm i -D vite;  npx vite
来源：http://nyr.aibaodan.cn

[U119] JS：生产构建
来源：http://rwy.gaohongyu789.top

npx vite build
来源：http://zgb.zhijiandao.cn

[U120] JS：读取环境变量（Vite）
来源：http://bvx.tarul.cn

import.meta.env.VITE_API_URL
来源：http://cdz.yj202588.top

================================================================================
来源：http://jgs.aibaodan.cn

统计汇总
来源：http://yuw.tanke756.top

================================================================================
来源：http://izr.daxiang520.top

按语言统计（条）：
来源：http://wfr.9152youxi.cn


<!-- 参考信息 -->