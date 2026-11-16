代发 wailian999

[T29] Swift：guard 提前返回
来源：http://zum.jqgufenzy.top

guard let x = opt else { return }
来源：http://bgp.kuanghao11.cn

[T30] Swift：协议
来源：http://afk.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://pxh.hfpthk.cn

[T31] Lua：Hello World
来源：http://oqk.xziqi.cn

print("Hello")
来源：http://xsw.tarul.cn

[T32] Lua：局部变量
来源：http://wnc.yfazqb.com

local a = 1
来源：http://uez.fengsongda.top

[T33] Lua：表（数组）
来源：http://kbn.ybcxt.top

local t = {1, 2, 3};  t[4] = 4
来源：http://srn.hongshengwenyu.top

[T34] Lua：遍历表
来源：http://dan.0kj1m.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cow.feifeiyinyue.top

[T35] Lua：字典表
来源：http://gru.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://qml.ydzc1.top

[T36] Lua：函数
来源：http://fgx.fengsongda.top

function add(a, b) return a + b end
来源：http://vsu.fehbvm.com

[T37] Lua：字符串拼接
来源：http://ijn.jinqigufen.top

"a" .. "b"
来源：http://qvn.52xcode.cn

[T38] Lua：条件
来源：http://kix.guannengcc.top

if x > 0 then print("正") end
来源：http://mus.guowangkeji.top

[T39] Lua：模式匹配
来源：http://obg.gaohongyu789.top

string.find(s, "%d+")
来源：http://ulx.yj20258888.top

[T40] Lua：元表
来源：http://ipo.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://gzy.bjfxy.top

[T41] Perl：Hello World
来源：http://gbh.snrcjt.cn

print "Hello\n";
来源：http://dcf.yfazqb.com

[T42] Perl：变量类型
来源：http://wbi.xylfe.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kqp.redwolf501.top

[T43] Perl：字符串插值
来源：http://nzk.zdqjudy.top

"值: $a"
来源：http://vao.vqdsnc.cn

[T44] Perl：条件
来源：http://nod.jiagoushi.top

if ($a > 0) { print "正"; }
来源：http://pla.jinqigufen.top

[T45] Perl：数组遍历
来源：http://vup.hesvh.cn

for my $x (@arr) { print $x; }
来源：http://act.jlsjyb.cn

[T46] Perl：哈希操作
来源：http://tcg.sufxvd.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uhq.yvedp.cn

[T47] Perl：正则捕获
来源：http://kkp.ydjk.org.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hic.hammf.cn

[T48] Perl：正则替换
来源：http://cpy.dianchejie.cn

$s =~ s/old/new/g;
来源：http://jdf.zhongyouzk.top

[T49] Perl：函数
来源：http://gdj.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tym.c1oappe.top

[T50] Perl：逐行读文件
来源：http://ttk.dashuyun.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vee.jlsjyb.cn

while (my $line = <$fh>) { print $line; }
来源：http://bhl.hfpthk.cn

[T51] Scala：Hello World
来源：http://qsg.nanxuanxn.top

println("Hello")
来源：http://vyi.jyoumei.cn

[T52] Scala：变量
来源：http://ikw.hnxiangtu.top

val a = 1;  var b = 2
来源：http://oxj.sufxvd.cn

[T53] Scala：字符串插值
来源：http://cpq.smart0.xyz

s"值: $b"
来源：http://qwn.jlsjyb.cn

[T54] Scala：集合映射
来源：http://ejg.xingfuxueyuan.xyz

List(1, 2, 3).map(_ * 2)
来源：http://ptu.sweek.top

[T55] Scala：集合过滤
来源：http://cpu.tianlin.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://tyg.fzhhl.top

[T56] Scala：样例类
来源：http://xzo.ydzc1.top

case class User(name: String, age: Int)
来源：http://caq.xingfuxueyuan.xyz

[T57] Scala：模式匹配
来源：http://ize.xziqi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://iyx.zhongyouzk.top

[T58] Scala：函数定义
来源：http://ibg.daria6918.cn

def add(a: Int, b: Int): Int = a + b
来源：http://upj.daxiang520.top

[T59] Scala：循环
来源：http://kwr.xuanzx.com

for (i <- 1 to 10) println(i)
来源：http://aoa.hcnkem.com

[T60] Scala：折叠
来源：http://jgh.ppjwa.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zod.yj202588.top

================================================================================
来源：http://udf.zhongyouzk.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://glp.9152youxi.cn

================================================================================
来源：http://mqo.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://ltt.pycfn.com

python -m venv .venv && source .venv/bin/activate
来源：http://ozd.yj20258.top

[U02] Py：导出 / 安装依赖
来源：http://hdq.jianghu66.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ncb.hnqzz.top

[U03] Py：加载 .env 配置
来源：http://ywo.zycfv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qjv.iojbl.cn

[U04] Py：变量调试打印
来源：http://nuw.jinghuilouyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jxy.snrcjt.cn

[U05] Py：列表去重且保序
来源：http://neu.shanyushiyangtech.top

list(dict.fromkeys(arr))
来源：http://zdn.smart0.xyz

[U06] Py：合并两个字典
来源：http://fxb.tian-w.cn

{**a, **b}
来源：http://jba.vehdjk.com

[U07] Py：反转字典键值
来源：http://zhc.9152youxi.cn

{v: k for k, v in d.items()}
来源：http://ykv.redwolf501.top

[U08] Py：展平二维列表
来源：http://kme.hesvh.cn

[y for x in nested for y in x]
来源：http://wab.yongpay.top

[U09] Py：字典取最大值的键
来源：http://ayc.sysykeji.top

max(d, key=d.get)
来源：http://nte.yvedp.cn

[U10] Py：按值排序字典
来源：http://qgn.hongshengwenyu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ugq.xinyue.icu

[U11] Py：生成器表达式
来源：http://wvz.smart0.xyz

(x * 2 for x in arr)
来源：http://dok.hammf.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vnf.yvedp.cn

Counter(arr).most_common(3)
来源：http://lye.cucudq.cn

[U13] Py：固定长度队列
来源：http://wbl.tanke756.top

deque(maxlen=10)
来源：http://anl.nanxuanxn.top

[U14] Py：分组收集到列表
来源：http://qxv.svipenyu.cn

defaultdict(list)
来源：http://akd.fzhhl.top

[U15] Py：高精度计时
来源：http://wxq.dianchejie.cn

t = time.perf_counter()
来源：http://irf.vqdsnc.cn

[U16] Py：命令行参数解析
来源：http://xjf.xylfe.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kbp.nwbrower.top

[U17] Py：初始化日志
来源：http://xhj.andypj.xyz

logging.basicConfig(level=logging.INFO)
来源：http://egk.wangshuangyany.cn

[U18] Py：预编译正则
来源：http://qzu.hywenlv.cn

pat = re.compile(r"\d+")
来源：http://dqu.nwbrower.top

[U19] Py：正则替换带回调
来源：http://scw.ywan-chungtsiang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ccv.zdbjq.cn

[U20] Py：缓存函数结果
来源：http://cvw.cashguo.top

@functools.lru_cache(maxsize=None)
来源：http://uhe.gotoacloud.top

[U21] Py：自定义上下文管理器
来源：http://ugw.shangyingyoupin.top

@contextlib.contextmanager
来源：http://bqq.vehdjk.com

[U22] Py：矩阵转置
来源：http://gal.vqdsnc.cn

list(zip(*m))
来源：http://sec.ctjpmb.com

[U23] Py：分块读取大文件
来源：http://qeb.hysaishi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dpy.cqqwz.cn

[U24] Py：路径操作
来源：http://jzx.fzhhl.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jny.zycfv.cn

[U25] Py：CSV 按字典读
来源：http://nbi.yj202588.top

csv.DictReader(f)
来源：http://ysb.cashguo.top

[U26] Py：并发下载
来源：http://ohf.guowangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xyf.bbcook.cn

[U27] Py：异步 HTTP
来源：http://lih.zycfv.cn

aiohttp.ClientSession() 配合 async with
来源：http://wgw.gaohongyu789.top

[U28] Py：类型别名
来源：http://scf.jinqigufen.top

UserId = int
来源：http://hxm.cheryme.top

[U29] Py：属性校验
来源：http://tka.gotoacloud.top

@property 与 @x.setter 配合
来源：http://mfa.snrcjt.cn

[U30] Py：数据类
来源：http://xzg.gzhubu.top

@dataclass(slots=True)
来源：http://ius.9152youxi.cn

[U31] Py：单测
来源：http://wxp.gaohongyu789.top

python -m pytest -q
来源：http://oke.nanxuanxn.top

[U32] Py：代码格式化
来源：http://sne.cheryme.top

ruff format . && ruff check --fix .
来源：http://vxw.dianchejie.cn

[U33] Py：打包发布
来源：http://fgw.yvedp.cn

python -m build  （依赖 pyproject.toml）
来源：http://sdm.fehbvm.com

[U34] Py：判断编码
来源：http://vlw.shzxlz.cn

chardet.detect(raw)
来源：http://fix.yfazqb.com

[U35] Py：发送邮件
来源：http://zji.yuxming.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ysd.guowangkeji.top

[U36] Py：定时任务
来源：http://pqo.hysaishi.cn

schedule.every(10).minutes.do(job)
来源：http://xht.hcnkem.com

[U37] Py：读写 Excel
来源：http://bvt.gzhubu.top

pandas.read_excel / DataFrame.to_excel
来源：http://xcf.yvedp.cn

[U38] Py：获取脚本所在目录
来源：http://auf.cdnleiting.top

Path(__file__).resolve().parent
来源：http://bco.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://pbq.ydjk.org.cn

sys.stdout.isatty()
来源：http://dhw.ywan-chungtsiang.top

[U40] Py：打印到标准错误
来源：http://zfx.dianchejie.cn

print("err", file=sys.stderr)
来源：http://xip.gogol.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://fxs.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://feq.jlsjyb.cn

[U42] PHP：PSR-4 自动加载
来源：http://uxv.guowangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vfh.jinqigfzy.top

[U43] PHP：声明命名空间
来源：http://tno.tarul.cn

namespace App\Http;
来源：http://jeq.0kj1m.cn

[U44] PHP：开启严格类型
来源：http://vqd.haohaochexian.top

declare(strict_types=1);
来源：http://fwo.yongpay.top

[U45] PHP：类型声明与返回类型
来源：http://aur.shuidangran.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qck.birdmap.top

[U46] PHP：可空类型
来源：http://vkq.yangfankeji.com

?string $name = null
来源：http://xee.ehwqpu.com

[U47] PHP：联合类型
来源：http://okw.ivvv.top

int|string $id
来源：http://hss.zhixingplan.top

[U48] PHP：纯枚举
来源：http://lin.hnqzz.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pfm.yj20258888.top

[U49] PHP：只读属性
来源：http://qfs.yj202588.top

public readonly string $name
来源：http://mcr.cucudq.cn

[U50] PHP：构造器属性提升
来源：http://ept.ydjk.org.cn

public function __construct(private int $id) {}
来源：http://tja.havefunace.top

[U51] PHP：数组解构
来源：http://rot.ydzc1.top

[$a, $b] = $arr;
来源：http://smf.epnwcf.com

[U52] PHP：箭头函数
来源：http://bwl.sufxvd.cn

$double = fn($x) => $x * 2;
来源：http://byz.tian-w.cn

[U53] PHP：空合并运算符
来源：http://wht.hammf.cn

$v = $a ?? $b ?? "default";
来源：http://guj.svipenyu.cn

[U54] PHP：空安全调用
来源：http://owo.redwolf501.top

$obj?->method()
来源：http://shv.vehdjk.com

[U55] PHP：match 表达式
来源：http://rcw.cucudq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ixd.nwbrower.top

[U56] PHP：命名参数
来源：http://cuv.tarul.cn

f(a: 1, b: 2)
来源：http://ktb.hnqzz.top

[U57] PHP：字符串插值
来源：http://rif.c1oappe.top

"值: {$a}"
来源：http://icv.guowangkeji.top

[U58] PHP：数组三件套
来源：http://xwr.jinyuanbaomall.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kcf.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://quw.tanke756.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://owz.guannengcc.top

[U60] PHP：JSON 编解码
来源：http://cfd.52xcode.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tfj.gogol.net.cn

[U61] PHP：正则
来源：http://icb.hcnkem.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://khq.hywenlv.cn

[U62] PHP：日期对象
来源：http://zaz.bbcook.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wqw.zycfv.cn

[U63] PHP：文件读写
来源：http://evk.birdmap.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vmt.jinqigfzy.top

[U64] PHP：目录遍历
来源：http://odv.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://dji.fktsv.cn

[U65] PHP：会话
来源：http://bmh.xuetiantiany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lqn.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://nxw.yueranfly.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lef.yueranfly.top

[U67] PHP：处理文件上传
来源：http://wbg.yuxming.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aos.zhijiandao.cn

[U68] PHP：PDO 连接
来源：http://xpw.ivvv.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://txl.chenjidiqi.icu

[U69] PHP：PDO 预处理
来源：http://rnt.fzhhl.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ysn.0kj1m.cn

[U70] PHP：PDO 事务
来源：http://wxp.chenlongwang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tyi.redwolf501.top

[U71] PHP：抛出异常
来源：http://dgo.sufxvd.cn

throw new RuntimeException("失败", 500);
来源：http://ftn.nwbrower.top

[U72] PHP：写错误日志
来源：http://dkj.fanxiaobao.xyz

error_log("失败: " . $e->getMessage());
来源：http://vst.yongpay.top

[U73] PHP：读取 ini 配置
来源：http://itr.shzxlz.cn

parse_ini_file("config.ini", true)
来源：http://zel.zhoulong.xyz

[U74] PHP：读取环境变量
来源：http://cix.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://bkp.zhengqikj.top

[U75] PHP：依赖注入
来源：http://udc.andypj.xyz

composer require psr/container
来源：http://gmw.chenlongwang.top

[U76] PHP：简单路由
来源：http://hmq.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lnj.shangyingyoupin.top

[U77] PHP：模板渲染
来源：http://yfr.sweek.top

composer require twig/twig
来源：http://hbv.tanke756.top

[U78] PHP：单元测试
来源：http://yrh.fktsv.cn

composer require --dev phpunit/phpunit
来源：http://srl.xuanzx.com

[U79] PHP：静态分析
来源：http://xqc.yongpay.top

composer require --dev phpstan/phpstan
来源：http://wgn.hongshengwenyu.top

[U80] PHP：代码规范修复
来源：http://yxb.jianghu66.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ytv.jianghu66.top

[U81] JS：初始化项目
来源：http://gyb.nanxinkj.top

npm init -y;  npm i express
来源：http://fxu.jyoumei.cn

[U82] JS：package.json 脚本
来源：http://des.c1oappe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://emn.cdnleiting.top

[U83] JS：ES Module 导入导出
来源：http://urd.zhaomingkeji.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://skt.cashguo.top

[U84] JS：CommonJS 写法
来源：http://wpg.aibaodan.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hov.mhx1999.top

[U85] JS：可选链
来源：http://ttp.9152youxi.cn

a?.b?.c
来源：http://rcj.daxiang520.top

[U86] JS：空值合并
来源：http://bbo.yonumen.top

a ?? b
来源：http://erv.yj202588.top

[U87] JS：解构默认值
来源：http://gsd.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://zpl.gogol.net.cn

[U88] JS：对象展开合并
来源：http://lkm.dashuyun.cn

{ ...a, ...b }
来源：http://iet.jianghu66.top

[U89] JS：数组去重
来源：http://gad.nwbrower.top

[...new Set(arr)]
来源：http://twt.chenjidiqi.icu

[U90] JS：数字数组排序
来源：http://bsy.aibaodan.cn

[...arr].sort((a, b) => a - b)
来源：http://xbp.guowangkeji.top

[U91] JS：对象键值遍历
来源：http://fxz.havefunace.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zcx.cucudq.cn

[U92] JS：深拷贝
来源：http://xib.c1oappe.top

structuredClone(obj)
来源：http://qss.ctjpmb.com

[U93] JS：模板字符串
来源：http://wyo.dianchejie.cn

`共 ${n} 条`
来源：http://igw.zhaomingkeji.xyz

[U94] JS：箭头函数
来源：http://rup.tarul.cn

const double = x => x * 2;
来源：http://qvt.zhiwuduotai.top

[U95] JS：Promise 包装
来源：http://ixp.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://itb.sufxvd.cn

[U96] JS：async/await 与异常
来源：http://yzm.tian-w.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nvw.feifeiyinyue.top

[U97] JS：并发请求
来源：http://cgx.fktsv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xqt.yfazqb.com

[U98] JS：fetch 带 JSON
来源：http://uyv.xuanzx.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bsg.yanxiufei.cn

[U99] JS：事件监听
来源：http://qxh.yanxiufei.cn

el.addEventListener("click", e => {})
来源：http://lqz.snrcjt.cn

[U100] JS：DOM 查询
来源：http://gms.feifeiyinyue.top

document.querySelector(".item")
来源：http://cch.redwolf501.top

[U101] JS：classList 操作
来源：http://osh.xylfe.cn

el.classList.toggle("active")
来源：http://sqx.cheryme.top

[U102] JS：本地存储
来源：http://ekj.redwolf501.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bvc.meibo888.top

[U103] JS：定时器
来源：http://fnb.jinghuilouyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eiv.xziqi.cn

[U104] JS：防抖
来源：http://rsg.daria6918.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://edt.yueranfly.top

[U105] JS：节流
来源：http://dst.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tij.meibo888.top

[U106] JS：日期格式化
来源：http://wzn.sufxvd.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://plu.zdbjq.cn

[U107] JS：数字千分位
来源：http://rtf.tian-w.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mbe.wangdashe.top

[U108] JS：随机整数
来源：http://exz.gotoacloud.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vtj.ydjk.org.cn

[U109] JS：数组分组
来源：http://gnf.yj202588.top

Object.groupBy(arr, x => x.type)
来源：http://eut.gaohongyu789.top

[U110] JS：数组分块
来源：http://ery.epnwcf.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bbb.jinyuanbaomall.cn

[U111] JS：对象转 Map
来源：http://rib.jinyuanbaomall.cn

new Map(Object.entries(obj))
来源：http://mhg.iojbl.cn

[U112] JS：字符串补位
来源：http://wjk.fktsv.cn

"7".padStart(3, "0")
来源：http://clh.chenlongwang.top

[U113] JS：正则替换全部
来源：http://qax.fanxiaobao.xyz

s.replaceAll("a", "b")
来源：http://vjv.9152youxi.cn

[U114] JS：JSON 深比较
来源：http://lnb.zhengqikj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hlv.zhengqikj.top

[U115] JS：生成 UUID
来源：http://nzg.bjfxy.top

crypto.randomUUID()
来源：http://daf.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://gik.bbcook.cn

/** @param {string} name */ function f(name) {}
来源：http://nnm.jiagoushi.top


<!-- 参考信息 -->