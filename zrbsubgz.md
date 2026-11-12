代发 wailian999

[T33] Lua：表（数组）
来源：http://cgb.yanxiufei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yhn.gogol.net.cn

[T34] Lua：遍历表
来源：http://jws.c1oappe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kvr.yj20258888.top

[T35] Lua：字典表
来源：http://bpm.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://axv.aibaodan.cn

[T36] Lua：函数
来源：http://xsy.hywenlv.cn

function add(a, b) return a + b end
来源：http://gsf.yj20258888.top

[T37] Lua：字符串拼接
来源：http://ide.cdnleiting.top

"a" .. "b"
来源：http://kqi.chenlongwang.top

[T38] Lua：条件
来源：http://vck.daxiang520.top

if x > 0 then print("正") end
来源：http://qyb.guannengcc.top

[T39] Lua：模式匹配
来源：http://kty.cheryme.top

string.find(s, "%d+")
来源：http://udw.cdnleiting.top

[T40] Lua：元表
来源：http://kkp.sxryk.cn

setmetatable({}, { __index = base })
来源：http://uiz.hesvh.cn

[T41] Perl：Hello World
来源：http://rha.nanxuanxn.top

print "Hello\n";
来源：http://qhl.redwolf501.top

[T42] Perl：变量类型
来源：http://bek.nwbrower.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uwf.shangyingyoupin.top

[T43] Perl：字符串插值
来源：http://unp.tian-w.cn

"值: $a"
来源：http://wvp.hnqzz.top

[T44] Perl：条件
来源：http://hjs.zhoulong.xyz

if ($a > 0) { print "正"; }
来源：http://bvw.yj20258.top

[T45] Perl：数组遍历
来源：http://uxp.xuanzx.com

for my $x (@arr) { print $x; }
来源：http://lig.dianchejie.cn

[T46] Perl：哈希操作
来源：http://rrk.chenzaomai.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vbg.zhaomingkeji.xyz

[T47] Perl：正则捕获
来源：http://dxd.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ybc.gaohongyu789.top

[T48] Perl：正则替换
来源：http://nmt.nwbrower.top

$s =~ s/old/new/g;
来源：http://wrj.sysykeji.top

[T49] Perl：函数
来源：http://qbg.xinyue.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://myk.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://uhv.jinyuanbaomall.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jhn.hnxiangtu.top

while (my $line = <$fh>) { print $line; }
来源：http://qsn.jiagoushi.top

[T51] Scala：Hello World
来源：http://kci.zdbjq.cn

println("Hello")
来源：http://rnp.ivvv.top

[T52] Scala：变量
来源：http://yuv.zhongyouzk.top

val a = 1;  var b = 2
来源：http://hto.yongpay.top

[T53] Scala：字符串插值
来源：http://oer.yongpay.top

s"值: $b"
来源：http://tsp.ivvv.top

[T54] Scala：集合映射
来源：http://vrc.yj20258.top

List(1, 2, 3).map(_ * 2)
来源：http://nhc.kuanghao11.cn

[T55] Scala：集合过滤
来源：http://brg.fktsv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pxu.tian-w.cn

[T56] Scala：样例类
来源：http://iko.sufxvd.cn

case class User(name: String, age: Int)
来源：http://iyf.havefunace.top

[T57] Scala：模式匹配
来源：http://rff.daria6918.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wki.snrcjt.cn

[T58] Scala：函数定义
来源：http://pba.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://frw.hnqzz.top

[T59] Scala：循环
来源：http://qiw.gotoacloud.top

for (i <- 1 to 10) println(i)
来源：http://uqb.0kj1m.cn

[T60] Scala：折叠
来源：http://xjp.gotoacloud.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jjn.ppjwa.cn

================================================================================
来源：http://lly.0kj1m.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jfe.gotoacloud.top

================================================================================
来源：http://sjm.jinqigufen.top

[U01] Py：创建虚拟环境
来源：http://xxc.zycfv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://aqw.fengsongda.top

[U02] Py：导出 / 安装依赖
来源：http://rgk.shanyushiyangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://plw.yvedp.cn

[U03] Py：加载 .env 配置
来源：http://yqn.316326.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://xqz.nanxuanxn.top

[U04] Py：变量调试打印
来源：http://qjf.dashuyun.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wkm.sweek.top

[U05] Py：列表去重且保序
来源：http://niz.uphjek.com

list(dict.fromkeys(arr))
来源：http://kzi.vqdsnc.cn

[U06] Py：合并两个字典
来源：http://wul.fktsv.cn

{**a, **b}
来源：http://lln.chenzaomai.com

[U07] Py：反转字典键值
来源：http://coj.snrcjt.cn

{v: k for k, v in d.items()}
来源：http://uby.guannengcc.top

[U08] Py：展平二维列表
来源：http://uom.cheryme.top

[y for x in nested for y in x]
来源：http://mwd.feifeiyinyue.top

[U09] Py：字典取最大值的键
来源：http://zsi.snrcjt.cn

max(d, key=d.get)
来源：http://zqy.dianchejie.cn

[U10] Py：按值排序字典
来源：http://kwz.sufxvd.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tbv.52xcode.cn

[U11] Py：生成器表达式
来源：http://ses.tarul.cn

(x * 2 for x in arr)
来源：http://ccv.fengsongda.top

[U12] Py：取出现最多的 3 个元素
来源：http://utw.jinghuilouyu.cn

Counter(arr).most_common(3)
来源：http://rhb.fktsv.cn

[U13] Py：固定长度队列
来源：http://lsu.jinyuanbaomall.cn

deque(maxlen=10)
来源：http://xwb.snrcjt.cn

[U14] Py：分组收集到列表
来源：http://myr.havefunace.top

defaultdict(list)
来源：http://xyj.c1oappe.top

[U15] Py：高精度计时
来源：http://uyg.yanxiufei.cn

t = time.perf_counter()
来源：http://yja.yfazqb.com

[U16] Py：命令行参数解析
来源：http://efu.yonumen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vxu.shangyingyoupin.top

[U17] Py：初始化日志
来源：http://ttf.shzxlz.cn

logging.basicConfig(level=logging.INFO)
来源：http://inj.jlsjyb.cn

[U18] Py：预编译正则
来源：http://gmw.hnqzz.top

pat = re.compile(r"\d+")
来源：http://isk.tianlin.xyz

[U19] Py：正则替换带回调
来源：http://phz.0kj1m.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://znb.andypj.xyz

[U20] Py：缓存函数结果
来源：http://rgu.hywenlv.cn

@functools.lru_cache(maxsize=None)
来源：http://rsg.jianghu66.top

[U21] Py：自定义上下文管理器
来源：http://zxm.sxryk.cn

@contextlib.contextmanager
来源：http://utd.yj202588.top

[U22] Py：矩阵转置
来源：http://rxo.yangfankeji.com

list(zip(*m))
来源：http://fgd.nwbrower.top

[U23] Py：分块读取大文件
来源：http://kta.hywenlv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pbv.52xcode.cn

[U24] Py：路径操作
来源：http://knf.sxryk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oje.vqdsnc.cn

[U25] Py：CSV 按字典读
来源：http://mxe.tanke756.top

csv.DictReader(f)
来源：http://fax.hfpthk.cn

[U26] Py：并发下载
来源：http://ftt.xziqi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://myy.zhoulong.xyz

[U27] Py：异步 HTTP
来源：http://oty.birdmap.top

aiohttp.ClientSession() 配合 async with
来源：http://cpe.fanxiaobao.xyz

[U28] Py：类型别名
来源：http://kmf.fanxiaobao.xyz

UserId = int
来源：http://sqi.vehdjk.com

[U29] Py：属性校验
来源：http://sie.yonumen.top

@property 与 @x.setter 配合
来源：http://bgm.xuetiantiany.cn

[U30] Py：数据类
来源：http://afs.bbcook.cn

@dataclass(slots=True)
来源：http://wne.gotoacloud.top

[U31] Py：单测
来源：http://sxq.feifeiyinyue.top

python -m pytest -q
来源：http://xlk.zhiwuduotai.top

[U32] Py：代码格式化
来源：http://txe.sxryk.cn

ruff format . && ruff check --fix .
来源：http://tvn.fzhhl.top

[U33] Py：打包发布
来源：http://irq.haohaochexian.top

python -m build  （依赖 pyproject.toml）
来源：http://ilz.ppjwa.cn

[U34] Py：判断编码
来源：http://ccp.cqqwz.cn

chardet.detect(raw)
来源：http://myg.shangyingyoupin.top

[U35] Py：发送邮件
来源：http://wrn.chenlongwang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cbs.jinqigfzy.top

[U36] Py：定时任务
来源：http://fqn.yangfankeji.com

schedule.every(10).minutes.do(job)
来源：http://xqa.cheryme.top

[U37] Py：读写 Excel
来源：http://pfx.pycfn.com

pandas.read_excel / DataFrame.to_excel
来源：http://isj.gzhubu.top

[U38] Py：获取脚本所在目录
来源：http://cvj.cashguo.top

Path(__file__).resolve().parent
来源：http://afx.wangdashe.top

[U39] Py：判断是否在交互环境
来源：http://ohl.chenjidiqi.icu

sys.stdout.isatty()
来源：http://ets.wangshuangyany.cn

[U40] Py：打印到标准错误
来源：http://mkc.yonumen.top

print("err", file=sys.stderr)
来源：http://zgf.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://tak.yonumen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pgj.smart0.xyz

[U42] PHP：PSR-4 自动加载
来源：http://vko.daxiang520.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mda.ywan-chungtsiang.top

[U43] PHP：声明命名空间
来源：http://jeb.tianlin.xyz

namespace App\Http;
来源：http://han.0kj1m.cn

[U44] PHP：开启严格类型
来源：http://tdi.dashuyun.cn

declare(strict_types=1);
来源：http://etz.fktsv.cn

[U45] PHP：类型声明与返回类型
来源：http://xla.aibaodan.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wbk.52xcode.cn

[U46] PHP：可空类型
来源：http://zsy.hywenlv.cn

?string $name = null
来源：http://eaj.yanxiufei.cn

[U47] PHP：联合类型
来源：http://vgt.chenlongwang.top

int|string $id
来源：http://tgm.sufxvd.cn

[U48] PHP：纯枚举
来源：http://qqm.shzxlz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mrs.shangyingyoupin.top

[U49] PHP：只读属性
来源：http://gci.sjlbkw.cn

public readonly string $name
来源：http://kfd.hfpthk.cn

[U50] PHP：构造器属性提升
来源：http://hqe.fengsongda.top

public function __construct(private int $id) {}
来源：http://tas.cashguo.top

[U51] PHP：数组解构
来源：http://duk.zhengqikj.top

[$a, $b] = $arr;
来源：http://czq.52xcode.cn

[U52] PHP：箭头函数
来源：http://cxz.hnxiangtu.top

$double = fn($x) => $x * 2;
来源：http://gjv.jiagoushi.top

[U53] PHP：空合并运算符
来源：http://xom.xylfe.cn

$v = $a ?? $b ?? "default";
来源：http://hxz.yongpay.top

[U54] PHP：空安全调用
来源：http://gde.guannengcc.top

$obj?->method()
来源：http://ret.ctjpmb.com

[U55] PHP：match 表达式
来源：http://vca.yfazqb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yqc.zdbjq.cn

[U56] PHP：命名参数
来源：http://rwn.tanke756.top

f(a: 1, b: 2)
来源：http://ljm.cucudq.cn

[U57] PHP：字符串插值
来源：http://dlw.tianlin.xyz

"值: {$a}"
来源：http://dog.bbcook.cn

[U58] PHP：数组三件套
来源：http://bpp.zhaomingkeji.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cmo.yanxiufei.cn

[U59] PHP：自定义排序
来源：http://fzs.chenlongwang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wzr.ywan-chungtsiang.top

[U60] PHP：JSON 编解码
来源：http://lco.dianchejie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hrp.52xcode.cn

[U61] PHP：正则
来源：http://iqu.daria6918.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lev.xuanzx.com

[U62] PHP：日期对象
来源：http://zzc.shanyushiyangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qbh.chenjidiqi.icu

[U63] PHP：文件读写
来源：http://ghh.fengsongda.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lfo.xuanzx.com

[U64] PHP：目录遍历
来源：http://gaz.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://kkl.quarkkingdee.top

[U65] PHP：会话
来源：http://zrv.ydzc1.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dlb.pycfn.com

[U66] PHP：设置 Cookie
来源：http://kbn.52xcode.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jei.316326.xyz

[U67] PHP：处理文件上传
来源：http://ljq.yangfankeji.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://smx.zhoulong.xyz

[U68] PHP：PDO 连接
来源：http://kve.ydjk.org.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://apl.birdmap.top

[U69] PHP：PDO 预处理
来源：http://ubu.yj20258888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ura.zhaomingkeji.xyz

[U70] PHP：PDO 事务
来源：http://muh.ivvv.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gix.havefunace.top

[U71] PHP：抛出异常
来源：http://cai.bbcook.cn

throw new RuntimeException("失败", 500);
来源：http://bbu.birdmap.top

[U72] PHP：写错误日志
来源：http://uco.shuidangran.top

error_log("失败: " . $e->getMessage());
来源：http://xva.zhengqikj.top

[U73] PHP：读取 ini 配置
来源：http://cin.birdmap.top

parse_ini_file("config.ini", true)
来源：http://tyt.chenzaomai.com

[U74] PHP：读取环境变量
来源：http://pro.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://smb.ydzc1.top

[U75] PHP：依赖注入
来源：http://woe.pengpengdd.cyou

composer require psr/container
来源：http://aly.daxiang520.top

[U76] PHP：简单路由
来源：http://mqa.nanxinkj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nth.yj20258.top

[U77] PHP：模板渲染
来源：http://etm.cdnleiting.top

composer require twig/twig
来源：http://yxw.shangyingyoupin.top

[U78] PHP：单元测试
来源：http://nxw.nanxuanxn.top

composer require --dev phpunit/phpunit
来源：http://oqz.pengpengdd.cyou

[U79] PHP：静态分析
来源：http://pxz.jqgfzy.top

composer require --dev phpstan/phpstan
来源：http://vrf.epnwcf.com

[U80] PHP：代码规范修复
来源：http://wow.vehdjk.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://gqk.guowangkeji.top

[U81] JS：初始化项目
来源：http://unv.jlsjyb.cn

npm init -y;  npm i express
来源：http://aam.zhaomingkeji.xyz

[U82] JS：package.json 脚本
来源：http://iwv.nanxuanxn.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rmw.ivvv.top

[U83] JS：ES Module 导入导出
来源：http://zgg.yfazqb.com

export const a = 1;  import { a } from "./m.js";
来源：http://nan.jqgufenzy.top

[U84] JS：CommonJS 写法
来源：http://lzi.jyoumei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fkf.jinyuanbaomall.cn

[U85] JS：可选链
来源：http://kri.tian-w.cn

a?.b?.c
来源：http://axx.daria6918.cn

[U86] JS：空值合并
来源：http://rpq.hywenlv.cn

a ?? b
来源：http://ebd.zdbjq.cn

[U87] JS：解构默认值
来源：http://kzk.tanke756.top

const { a = 1, b = 2 } = obj;
来源：http://ylf.yongpay.top

[U88] JS：对象展开合并
来源：http://rlh.gogol.net.cn

{ ...a, ...b }
来源：http://wmb.gzhubu.top

[U89] JS：数组去重
来源：http://pev.nanxuanxn.top

[...new Set(arr)]
来源：http://sit.aibaodan.cn

[U90] JS：数字数组排序
来源：http://lzb.zycfv.cn

[...arr].sort((a, b) => a - b)
来源：http://tru.daria6918.cn

[U91] JS：对象键值遍历
来源：http://fms.guannengcc.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bhx.nwbrower.top

[U92] JS：深拷贝
来源：http://fdl.wangshuangyany.cn

structuredClone(obj)
来源：http://tem.tarul.cn

[U93] JS：模板字符串
来源：http://qfw.hongshengwenyu.top

`共 ${n} 条`
来源：http://arb.zhengqikj.top

[U94] JS：箭头函数
来源：http://gzq.xinyue.icu

const double = x => x * 2;
来源：http://obc.havefunace.top

[U95] JS：Promise 包装
来源：http://kuw.ppjwa.cn

new Promise((resolve, reject) => {})
来源：http://may.hnxiangtu.top

[U96] JS：async/await 与异常
来源：http://xin.yanxiufei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cof.sysykeji.top

[U97] JS：并发请求
来源：http://gds.tianlin.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://oon.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://pff.zdbjq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wmz.jinghuilouyu.cn

[U99] JS：事件监听
来源：http://nkh.sysykeji.top

el.addEventListener("click", e => {})
来源：http://ayg.zhengqikj.top

[U100] JS：DOM 查询
来源：http://rdn.uphjek.com

document.querySelector(".item")
来源：http://ooe.aizwys.cn

[U101] JS：classList 操作
来源：http://wjj.pengpengdd.cyou

el.classList.toggle("active")
来源：http://euz.yvedp.cn

[U102] JS：本地存储
来源：http://xtn.chenjidiqi.icu

localStorage.setItem("k", JSON.stringify(v))
来源：http://mag.hesvh.cn

[U103] JS：定时器
来源：http://vnf.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://atq.yfazqb.com

[U104] JS：防抖
来源：http://mue.hfpthk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gqp.sufxvd.cn

[U105] JS：节流
来源：http://bew.gotoacloud.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://etv.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://gek.xingfuxueyuan.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://izs.chenjidiqi.icu

[U107] JS：数字千分位
来源：http://bvc.316326.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jmx.jinqigfzy.top

[U108] JS：随机整数
来源：http://qpx.yanxiufei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zpu.hysaishi.cn

[U109] JS：数组分组
来源：http://gxx.tarul.cn

Object.groupBy(arr, x => x.type)
来源：http://jjq.ywan-chungtsiang.top

[U110] JS：数组分块
来源：http://kdh.chenzaomai.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iuc.ybcxt.top

[U111] JS：对象转 Map
来源：http://kwu.aizwys.cn

new Map(Object.entries(obj))
来源：http://zdw.daria6918.cn

[U112] JS：字符串补位
来源：http://ktu.ppjwa.cn

"7".padStart(3, "0")
来源：http://iql.hongshengwenyu.top

[U113] JS：正则替换全部
来源：http://bys.svipenyu.cn

s.replaceAll("a", "b")
来源：http://yph.birdmap.top

[U114] JS：JSON 深比较
来源：http://god.chenjidiqi.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://euv.zhongyouzk.top

[U115] JS：生成 UUID
来源：http://xlk.fanxiaobao.xyz

crypto.randomUUID()
来源：http://hvh.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://mwp.yj20258.top

/** @param {string} name */ function f(name) {}
来源：http://xiu.yongpay.top

[U117] JS：单元测试
来源：http://hcb.nwbrower.top

npm i -D vitest;  npx vitest
来源：http://jpu.guowangkeji.top

[U118] JS：开发服务器
来源：http://fgh.shanyushiyangkeji.top

npm i -D vite;  npx vite
来源：http://ptn.xingfuxueyuan.xyz

[U119] JS：生产构建
来源：http://ryx.cqqwz.cn

npx vite build
来源：http://ifp.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://hjm.shzxlz.cn

import.meta.env.VITE_API_URL
来源：http://tra.zhongyouzk.top


<!-- 参考信息 -->