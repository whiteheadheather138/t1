代发 wailian999

[T33] Lua：表（数组）
来源：http://gjq.shanyushiyangtech.top

local t = {1, 2, 3};  t[4] = 4
来源：http://gmn.pycfn.com

[T34] Lua：遍历表
来源：http://fet.xinyue.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://pma.dashuyun.cn

[T35] Lua：字典表
来源：http://vog.hfpthk.cn

local d = { a = 1 };  d.b = 2
来源：http://jwl.tanke756.top

[T36] Lua：函数
来源：http://rlu.sysykeji.top

function add(a, b) return a + b end
来源：http://qxp.yonumen.top

[T37] Lua：字符串拼接
来源：http://tut.epnwcf.com

"a" .. "b"
来源：http://cby.zdqjudy.top

[T38] Lua：条件
来源：http://vch.gaohongyu789.top

if x > 0 then print("正") end
来源：http://psb.jqgfzy.top

[T39] Lua：模式匹配
来源：http://rni.yanxiufei.cn

string.find(s, "%d+")
来源：http://dkn.iojbl.cn

[T40] Lua：元表
来源：http://hkg.havefunace.top

setmetatable({}, { __index = base })
来源：http://oxl.ydjk.org.cn

[T41] Perl：Hello World
来源：http://lkj.nanxuanxn.top

print "Hello\n";
来源：http://iww.nanxuanxn.top

[T42] Perl：变量类型
来源：http://zvv.kuanghao11.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dyv.jiagoushi.top

[T43] Perl：字符串插值
来源：http://vbk.sjlbkw.cn

"值: $a"
来源：http://sfa.ehwqpu.com

[T44] Perl：条件
来源：http://qdq.cdnleiting.top

if ($a > 0) { print "正"; }
来源：http://pjv.tianlin.xyz

[T45] Perl：数组遍历
来源：http://ken.zhiwuduotai.top

for my $x (@arr) { print $x; }
来源：http://qri.yueranfly.top

[T46] Perl：哈希操作
来源：http://bgo.nanxuanxn.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xmk.sxryk.cn

[T47] Perl：正则捕获
来源：http://gbl.aibaodan.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xes.snrcjt.cn

[T48] Perl：正则替换
来源：http://uxd.tarul.cn

$s =~ s/old/new/g;
来源：http://rcz.tanke756.top

[T49] Perl：函数
来源：http://mqw.bbcook.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wne.zhongyouzk.top

[T50] Perl：逐行读文件
来源：http://bhl.shanyushiyangtech.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lxp.havefunace.top

while (my $line = <$fh>) { print $line; }
来源：http://awp.bbcook.cn

[T51] Scala：Hello World
来源：http://hli.hnxiangtu.top

println("Hello")
来源：http://hqx.guannengcc.top

[T52] Scala：变量
来源：http://qjq.cucudq.cn

val a = 1;  var b = 2
来源：http://hyu.0kj1m.cn

[T53] Scala：字符串插值
来源：http://naj.tianlin.xyz

s"值: $b"
来源：http://prg.iojbl.cn

[T54] Scala：集合映射
来源：http://wun.mhx1999.top

List(1, 2, 3).map(_ * 2)
来源：http://rpa.yj202588.top

[T55] Scala：集合过滤
来源：http://vqd.hongshengwenyu.top

List(1, 2, 3).filter(_ > 1)
来源：http://xqb.pengpengdd.cyou

[T56] Scala：样例类
来源：http://mek.tian-w.cn

case class User(name: String, age: Int)
来源：http://ntm.guannengcc.top

[T57] Scala：模式匹配
来源：http://kpp.nwbrower.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vdh.yfazqb.com

[T58] Scala：函数定义
来源：http://uzx.cucudq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pwy.wangshuangyany.cn

[T59] Scala：循环
来源：http://yji.chenlongwang.top

for (i <- 1 to 10) println(i)
来源：http://czo.dianchejie.cn

[T60] Scala：折叠
来源：http://hry.cqqwz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sju.daria6918.cn

================================================================================
来源：http://bfk.zhengqikj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xwr.dashuyun.cn

================================================================================
来源：http://rep.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://hwm.ctjpmb.com

python -m venv .venv && source .venv/bin/activate
来源：http://ouv.pycfn.com

[U02] Py：导出 / 安装依赖
来源：http://esw.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xcp.meibo888.top

[U03] Py：加载 .env 配置
来源：http://fei.xziqi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rpd.andypj.xyz

[U04] Py：变量调试打印
来源：http://ivl.sufxvd.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xkx.uphjek.com

[U05] Py：列表去重且保序
来源：http://aqy.xylfe.cn

list(dict.fromkeys(arr))
来源：http://wkk.yj20258.top

[U06] Py：合并两个字典
来源：http://dec.wangdashe.top

{**a, **b}
来源：http://ihi.jianghu66.top

[U07] Py：反转字典键值
来源：http://rts.hnxiangtu.top

{v: k for k, v in d.items()}
来源：http://cpy.andypj.xyz

[U08] Py：展平二维列表
来源：http://zkb.xinyue.icu

[y for x in nested for y in x]
来源：http://gtq.daxiang520.top

[U09] Py：字典取最大值的键
来源：http://hum.kuanghao11.cn

max(d, key=d.get)
来源：http://chd.yuanzhike.top

[U10] Py：按值排序字典
来源：http://fra.cdnleiting.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uyo.9152youxi.cn

[U11] Py：生成器表达式
来源：http://tls.shangyingyoupin.top

(x * 2 for x in arr)
来源：http://vrn.zhixingplan.top

[U12] Py：取出现最多的 3 个元素
来源：http://fwn.jinyuanbaomall.cn

Counter(arr).most_common(3)
来源：http://wvk.gotoacloud.top

[U13] Py：固定长度队列
来源：http://mki.hcnkem.com

deque(maxlen=10)
来源：http://sha.shangyingyoupin.top

[U14] Py：分组收集到列表
来源：http://lht.guowangkeji.top

defaultdict(list)
来源：http://pey.aibaodan.cn

[U15] Py：高精度计时
来源：http://ioy.shzxlz.cn

t = time.perf_counter()
来源：http://kvr.zycfv.cn

[U16] Py：命令行参数解析
来源：http://kie.tarul.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kwq.xingfuxueyuan.xyz

[U17] Py：初始化日志
来源：http://txl.kuanghao11.cn

logging.basicConfig(level=logging.INFO)
来源：http://rvu.xingfuxueyuan.xyz

[U18] Py：预编译正则
来源：http://oci.hysaishi.cn

pat = re.compile(r"\d+")
来源：http://zbz.wangdashe.top

[U19] Py：正则替换带回调
来源：http://lij.hongshengwenyu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yil.zhaomingkeji.xyz

[U20] Py：缓存函数结果
来源：http://qdi.ywan-chungtsiang.top

@functools.lru_cache(maxsize=None)
来源：http://pzi.feifeiyinyue.top

[U21] Py：自定义上下文管理器
来源：http://uqs.hywenlv.cn

@contextlib.contextmanager
来源：http://izf.c1oappe.top

[U22] Py：矩阵转置
来源：http://bxr.yanxiufei.cn

list(zip(*m))
来源：http://xlb.quarkkingdee.top

[U23] Py：分块读取大文件
来源：http://gph.sxryk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://exq.zhaomingkeji.xyz

[U24] Py：路径操作
来源：http://onv.jianghu66.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lgl.tanke756.top

[U25] Py：CSV 按字典读
来源：http://ral.ivvv.top

csv.DictReader(f)
来源：http://hfi.gotoacloud.top

[U26] Py：并发下载
来源：http://dzl.gogol.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hod.mhx1999.top

[U27] Py：异步 HTTP
来源：http://czr.fktsv.cn

aiohttp.ClientSession() 配合 async with
来源：http://rqg.redwolf501.top

[U28] Py：类型别名
来源：http://fbv.zdqjudy.top

UserId = int
来源：http://lhy.daxiang520.top

[U29] Py：属性校验
来源：http://hjj.redwolf501.top

@property 与 @x.setter 配合
来源：http://bpc.zhiwuduotai.top

[U30] Py：数据类
来源：http://fnm.tarul.cn

@dataclass(slots=True)
来源：http://ahe.redwolf501.top

[U31] Py：单测
来源：http://tdt.guowangkeji.top

python -m pytest -q
来源：http://zis.yangfankeji.com

[U32] Py：代码格式化
来源：http://usa.vqdsnc.cn

ruff format . && ruff check --fix .
来源：http://vvm.nanxinkj.top

[U33] Py：打包发布
来源：http://ega.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://nqk.hysaishi.cn

[U34] Py：判断编码
来源：http://mpf.yonumen.top

chardet.detect(raw)
来源：http://frm.zdbjq.cn

[U35] Py：发送邮件
来源：http://biu.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zei.wangshuangyany.cn

[U36] Py：定时任务
来源：http://rgq.daxiang520.top

schedule.every(10).minutes.do(job)
来源：http://nri.iojbl.cn

[U37] Py：读写 Excel
来源：http://uol.shanyushiyangtech.top

pandas.read_excel / DataFrame.to_excel
来源：http://wex.yueranfly.top

[U38] Py：获取脚本所在目录
来源：http://hfa.guowangkeji.top

Path(__file__).resolve().parent
来源：http://qum.iojbl.cn

[U39] Py：判断是否在交互环境
来源：http://aor.xuetiantiany.cn

sys.stdout.isatty()
来源：http://gsk.daria6918.cn

[U40] Py：打印到标准错误
来源：http://fwp.yfazqb.com

print("err", file=sys.stderr)
来源：http://xxb.tianlin.xyz

[U41] PHP：初始化 Composer 项目
来源：http://mne.uphjek.com

composer init;  composer require guzzlehttp/guzzle
来源：http://bmp.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://czp.sweek.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fjy.tian-w.cn

[U43] PHP：声明命名空间
来源：http://gxj.cucudq.cn

namespace App\Http;
来源：http://ety.dashuyun.cn

[U44] PHP：开启严格类型
来源：http://ckv.daria6918.cn

declare(strict_types=1);
来源：http://qvc.zhijiandao.cn

[U45] PHP：类型声明与返回类型
来源：http://cwo.pengpengdd.cyou

function add(int $a, int $b): int { return $a + $b; }
来源：http://ieb.fengsongda.top

[U46] PHP：可空类型
来源：http://sju.fehbvm.com

?string $name = null
来源：http://hhl.cheryme.top

[U47] PHP：联合类型
来源：http://sao.gaohongyu789.top

int|string $id
来源：http://cxg.dianchejie.cn

[U48] PHP：纯枚举
来源：http://xjy.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kic.hywenlv.cn

[U49] PHP：只读属性
来源：http://tvn.yongpay.top

public readonly string $name
来源：http://jyx.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://kxj.yj20258888.top

public function __construct(private int $id) {}
来源：http://jor.daria6918.cn

[U51] PHP：数组解构
来源：http://rym.gaohongyu789.top

[$a, $b] = $arr;
来源：http://drh.chenlongwang.top

[U52] PHP：箭头函数
来源：http://gwg.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://xlb.quarkkingdee.top

[U53] PHP：空合并运算符
来源：http://qrx.hysaishi.cn

$v = $a ?? $b ?? "default";
来源：http://rnr.sjlbkw.cn

[U54] PHP：空安全调用
来源：http://gld.shanyushiyangtech.top

$obj?->method()
来源：http://nzi.shanyushiyangtech.top

[U55] PHP：match 表达式
来源：http://mzq.yuanzhike.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xvv.tarul.cn

[U56] PHP：命名参数
来源：http://jhv.vehdjk.com

f(a: 1, b: 2)
来源：http://qlo.fzhhl.top

[U57] PHP：字符串插值
来源：http://zjg.nanxinkj.top

"值: {$a}"
来源：http://izj.xuanzx.com

[U58] PHP：数组三件套
来源：http://teu.yj202588.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oab.ydjk.org.cn

[U59] PHP：自定义排序
来源：http://bfc.ywan-chungtsiang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mgu.daria6918.cn

[U60] PHP：JSON 编解码
来源：http://hie.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wzf.dianchejie.cn

[U61] PHP：正则
来源：http://thj.yj20258.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://evt.aibaodan.cn

[U62] PHP：日期对象
来源：http://ptk.zhiwuduotai.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uzc.nanxinkj.top

[U63] PHP：文件读写
来源：http://jzj.316326.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rim.zhixingplan.top

[U64] PHP：目录遍历
来源：http://fos.tarul.cn

glob("dir/*.php");  scandir("dir");
来源：http://gzz.cqqwz.cn

[U65] PHP：会话
来源：http://kdp.sweek.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gvc.ppjwa.cn

[U66] PHP：设置 Cookie
来源：http://jak.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kdq.dianchejie.cn

[U67] PHP：处理文件上传
来源：http://pnk.feifeiyinyue.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gzv.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://shw.yfazqb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ikb.cucudq.cn

[U69] PHP：PDO 预处理
来源：http://mot.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fkc.daxiang520.top

[U70] PHP：PDO 事务
来源：http://qbd.pengpengdd.cyou

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kyc.sufxvd.cn

[U71] PHP：抛出异常
来源：http://wrd.andypj.xyz

throw new RuntimeException("失败", 500);
来源：http://htz.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://vdr.iojbl.cn

error_log("失败: " . $e->getMessage());
来源：http://bhd.yj20258888.top

[U73] PHP：读取 ini 配置
来源：http://egs.tanke756.top

parse_ini_file("config.ini", true)
来源：http://mlr.ivvv.top

[U74] PHP：读取环境变量
来源：http://zuo.aibaodan.cn

getenv("APP_ENV") ?: "production"
来源：http://uru.cashguo.top

[U75] PHP：依赖注入
来源：http://cfb.shzxlz.cn

composer require psr/container
来源：http://aep.fanxiaobao.xyz

[U76] PHP：简单路由
来源：http://yru.ybcxt.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ult.yj20258888.top

[U77] PHP：模板渲染
来源：http://aoo.ywan-chungtsiang.top

composer require twig/twig
来源：http://amc.dianchejie.cn

[U78] PHP：单元测试
来源：http://tir.hnxiangtu.top

composer require --dev phpunit/phpunit
来源：http://jeg.zdqjudy.top

[U79] PHP：静态分析
来源：http://qvs.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://usj.zhijiandao.cn

[U80] PHP：代码规范修复
来源：http://ztv.shuidangran.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://glw.fehbvm.com

[U81] JS：初始化项目
来源：http://ycd.quarkkingdee.top

npm init -y;  npm i express
来源：http://cdk.yonumen.top

[U82] JS：package.json 脚本
来源：http://phu.nanxinkj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://llu.gotoacloud.top

[U83] JS：ES Module 导入导出
来源：http://rpe.birdmap.top

export const a = 1;  import { a } from "./m.js";
来源：http://yrb.cdnleiting.top

[U84] JS：CommonJS 写法
来源：http://pzx.xuanzx.com

module.exports = { a };  const { a } = require("./m");
来源：http://lee.dianchejie.cn

[U85] JS：可选链
来源：http://wif.52xcode.cn

a?.b?.c
来源：http://cjl.iojbl.cn

[U86] JS：空值合并
来源：http://xsl.wangdashe.top

a ?? b
来源：http://dyz.guowangkeji.top

[U87] JS：解构默认值
来源：http://zqg.vehdjk.com

const { a = 1, b = 2 } = obj;
来源：http://bsi.hesvh.cn

[U88] JS：对象展开合并
来源：http://kzv.cqqwz.cn

{ ...a, ...b }
来源：http://hwo.ehwqpu.com

[U89] JS：数组去重
来源：http://zzt.tianlin.xyz

[...new Set(arr)]
来源：http://ehv.yj20258.top

[U90] JS：数字数组排序
来源：http://hkd.fzhhl.top

[...arr].sort((a, b) => a - b)
来源：http://umx.gaohongyu789.top

[U91] JS：对象键值遍历
来源：http://gjp.jqgufenzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nlh.yongpay.top

[U92] JS：深拷贝
来源：http://bhp.jinqigfzy.top

structuredClone(obj)
来源：http://wsd.gogol.net.cn

[U93] JS：模板字符串
来源：http://rka.andypj.xyz

`共 ${n} 条`
来源：http://hvh.redwolf501.top

[U94] JS：箭头函数
来源：http://tjw.vqdsnc.cn

const double = x => x * 2;
来源：http://ylr.0kj1m.cn

[U95] JS：Promise 包装
来源：http://qkc.redwolf501.top

new Promise((resolve, reject) => {})
来源：http://hqq.fktsv.cn

[U96] JS：async/await 与异常
来源：http://mwe.yangfankeji.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xrt.ywan-chungtsiang.top

[U97] JS：并发请求
来源：http://qga.fanxiaobao.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://ucd.ywan-chungtsiang.top

[U98] JS：fetch 带 JSON
来源：http://sjy.redwolf501.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rey.0kj1m.cn

[U99] JS：事件监听
来源：http://sny.gaohongyu789.top

el.addEventListener("click", e => {})
来源：http://dxk.shangyingyoupin.top

[U100] JS：DOM 查询
来源：http://msv.hcnkem.com

document.querySelector(".item")
来源：http://kdq.mhx1999.top

[U101] JS：classList 操作
来源：http://ouh.quarkkingdee.top

el.classList.toggle("active")
来源：http://zpu.chenjidiqi.icu

[U102] JS：本地存储
来源：http://gen.shangyingyoupin.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kol.sufxvd.cn

[U103] JS：定时器
来源：http://wmi.aibaodan.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jkq.zhoulong.xyz

[U104] JS：防抖
来源：http://iou.dianchejie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://exd.kuanghao11.cn

[U105] JS：节流
来源：http://cay.chenlongwang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kpz.ywan-chungtsiang.top

[U106] JS：日期格式化
来源：http://yya.hysaishi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bbo.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://fbs.smart0.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fwq.jyoumei.cn

[U108] JS：随机整数
来源：http://vct.yueranfly.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bgp.hfpthk.cn

[U109] JS：数组分组
来源：http://vtk.316326.xyz

Object.groupBy(arr, x => x.type)
来源：http://xvw.yuanzhike.top

[U110] JS：数组分块
来源：http://poz.xziqi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dvc.birdmap.top

[U111] JS：对象转 Map
来源：http://vut.shangyingyoupin.top

new Map(Object.entries(obj))
来源：http://ddo.hnxiangtu.top

[U112] JS：字符串补位
来源：http://ixb.uphjek.com

"7".padStart(3, "0")
来源：http://spp.zhaomingkeji.xyz

[U113] JS：正则替换全部
来源：http://hkb.c1oappe.top

s.replaceAll("a", "b")
来源：http://hiv.zhengqikj.top

[U114] JS：JSON 深比较
来源：http://oqr.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mhk.ivvv.top

[U115] JS：生成 UUID
来源：http://anh.uphjek.com

crypto.randomUUID()
来源：http://eqi.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://utz.yueranfly.top

/** @param {string} name */ function f(name) {}
来源：http://htf.hnxiangtu.top

[U117] JS：单元测试
来源：http://nye.hysaishi.cn

npm i -D vitest;  npx vitest
来源：http://opd.yuxming.cn

[U118] JS：开发服务器
来源：http://bts.ybcxt.top

npm i -D vite;  npx vite
来源：http://vfl.vqdsnc.cn

[U119] JS：生产构建
来源：http://cdi.wangdashe.top

npx vite build
来源：http://ibv.yfazqb.com

[U120] JS：读取环境变量（Vite）
来源：http://raq.sweek.top

import.meta.env.VITE_API_URL
来源：http://rte.yonumen.top


<!-- 参考信息 -->