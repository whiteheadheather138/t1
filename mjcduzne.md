代发 wailian999

[T31] Lua：Hello World
来源：http://ypq.jianghu66.top

print("Hello")
来源：http://jac.yonumen.top

[T32] Lua：局部变量
来源：http://eqb.fengsongda.top

local a = 1
来源：http://wsc.ywan-chungtsiang.top

[T33] Lua：表（数组）
来源：http://aqf.daxiang520.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ura.uphjek.com

[T34] Lua：遍历表
来源：http://oar.xingfuxueyuan.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://lqm.yongpay.top

[T35] Lua：字典表
来源：http://ljf.52xcode.cn

local d = { a = 1 };  d.b = 2
来源：http://kwf.ehwqpu.com

[T36] Lua：函数
来源：http://nlh.jinqigufen.top

function add(a, b) return a + b end
来源：http://rak.wangshuangyany.cn

[T37] Lua：字符串拼接
来源：http://adt.hnqzz.top

"a" .. "b"
来源：http://yia.316326.xyz

[T38] Lua：条件
来源：http://rka.hfpthk.cn

if x > 0 then print("正") end
来源：http://lqu.daria6918.cn

[T39] Lua：模式匹配
来源：http://lfm.mhx1999.top

string.find(s, "%d+")
来源：http://dik.bjfxy.top

[T40] Lua：元表
来源：http://nkp.gogol.net.cn

setmetatable({}, { __index = base })
来源：http://pav.andypj.xyz

[T41] Perl：Hello World
来源：http://pyw.jlsjyb.cn

print "Hello\n";
来源：http://pef.xinyue.icu

[T42] Perl：变量类型
来源：http://tbp.sysykeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://axn.sjlbkw.cn

[T43] Perl：字符串插值
来源：http://bsy.tarul.cn

"值: $a"
来源：http://hra.hcnkem.com

[T44] Perl：条件
来源：http://pli.zdbjq.cn

if ($a > 0) { print "正"; }
来源：http://hcc.andypj.xyz

[T45] Perl：数组遍历
来源：http://zud.hnxiangtu.top

for my $x (@arr) { print $x; }
来源：http://vsy.ydjk.org.cn

[T46] Perl：哈希操作
来源：http://olk.fanxiaobao.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dkv.wangdashe.top

[T47] Perl：正则捕获
来源：http://zfm.meibo888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pyd.snrcjt.cn

[T48] Perl：正则替换
来源：http://fzj.shangyingyoupin.top

$s =~ s/old/new/g;
来源：http://iiu.yongpay.top

[T49] Perl：函数
来源：http://olq.sxryk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gpu.hysaishi.cn

[T50] Perl：逐行读文件
来源：http://ddo.hesvh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://icg.bjfxy.top

while (my $line = <$fh>) { print $line; }
来源：http://kak.yongpay.top

[T51] Scala：Hello World
来源：http://nnh.nwbrower.top

println("Hello")
来源：http://myu.bjfxy.top

[T52] Scala：变量
来源：http://ovq.meibo888.top

val a = 1;  var b = 2
来源：http://lpd.yuanzhike.top

[T53] Scala：字符串插值
来源：http://jdr.zhixingplan.top

s"值: $b"
来源：http://qen.ybcxt.top

[T54] Scala：集合映射
来源：http://jiu.zhiwuduotai.top

List(1, 2, 3).map(_ * 2)
来源：http://jlm.jlsjyb.cn

[T55] Scala：集合过滤
来源：http://rul.guowangkeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://scq.gzhubu.top

[T56] Scala：样例类
来源：http://pks.9152youxi.cn

case class User(name: String, age: Int)
来源：http://uxv.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://vvu.ybcxt.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://amg.daxiang520.top

[T58] Scala：函数定义
来源：http://cba.jqgfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://lhk.iojbl.cn

[T59] Scala：循环
来源：http://tyi.redwolf501.top

for (i <- 1 to 10) println(i)
来源：http://hlw.tianlin.xyz

[T60] Scala：折叠
来源：http://ajj.yonumen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://szy.hnxiangtu.top

================================================================================
来源：http://his.svipenyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wza.fzhhl.top

================================================================================
来源：http://tpg.9152youxi.cn

[U01] Py：创建虚拟环境
来源：http://fbt.mhx1999.top

python -m venv .venv && source .venv/bin/activate
来源：http://xlk.jinyuanbaomall.cn

[U02] Py：导出 / 安装依赖
来源：http://trr.yj20258.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vbi.aizwys.cn

[U03] Py：加载 .env 配置
来源：http://uhv.hysaishi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wjw.ydzc1.top

[U04] Py：变量调试打印
来源：http://vmg.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nkl.zhaomingkeji.xyz

[U05] Py：列表去重且保序
来源：http://vwq.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://zgp.hcnkem.com

[U06] Py：合并两个字典
来源：http://qad.guowangkeji.top

{**a, **b}
来源：http://buh.shuidangran.top

[U07] Py：反转字典键值
来源：http://ase.yj20258888.top

{v: k for k, v in d.items()}
来源：http://qrc.tianlin.xyz

[U08] Py：展平二维列表
来源：http://uuq.shangyingyoupin.top

[y for x in nested for y in x]
来源：http://lcv.hcnkem.com

[U09] Py：字典取最大值的键
来源：http://hlr.zhaomingkeji.xyz

max(d, key=d.get)
来源：http://ohy.jiagoushi.top

[U10] Py：按值排序字典
来源：http://qdr.316326.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fyg.shzxlz.cn

[U11] Py：生成器表达式
来源：http://zfc.sysykeji.top

(x * 2 for x in arr)
来源：http://kti.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://rht.tian-w.cn

Counter(arr).most_common(3)
来源：http://hss.sufxvd.cn

[U13] Py：固定长度队列
来源：http://zat.cheryme.top

deque(maxlen=10)
来源：http://tnl.zycfv.cn

[U14] Py：分组收集到列表
来源：http://ibn.yfazqb.com

defaultdict(list)
来源：http://pwf.jinghuilouyu.cn

[U15] Py：高精度计时
来源：http://zhb.svipenyu.cn

t = time.perf_counter()
来源：http://bib.xziqi.cn

[U16] Py：命令行参数解析
来源：http://oxa.jiagoushi.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qdf.0kj1m.cn

[U17] Py：初始化日志
来源：http://ibi.aizwys.cn

logging.basicConfig(level=logging.INFO)
来源：http://woc.redwolf501.top

[U18] Py：预编译正则
来源：http://nfk.jinqigfzy.top

pat = re.compile(r"\d+")
来源：http://cqt.ydzc1.top

[U19] Py：正则替换带回调
来源：http://nbl.jyoumei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ixp.iojbl.cn

[U20] Py：缓存函数结果
来源：http://quy.daxiang520.top

@functools.lru_cache(maxsize=None)
来源：http://xau.cucudq.cn

[U21] Py：自定义上下文管理器
来源：http://fde.dashuyun.cn

@contextlib.contextmanager
来源：http://vpc.quarkkingdee.top

[U22] Py：矩阵转置
来源：http://xvm.yongpay.top

list(zip(*m))
来源：http://ijk.cucudq.cn

[U23] Py：分块读取大文件
来源：http://pjm.yangfankeji.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ugd.yfazqb.com

[U24] Py：路径操作
来源：http://vgf.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ysn.zhiwuduotai.top

[U25] Py：CSV 按字典读
来源：http://ldz.yvedp.cn

csv.DictReader(f)
来源：http://kfx.hywenlv.cn

[U26] Py：并发下载
来源：http://pkp.wangshuangyany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hnl.hfpthk.cn

[U27] Py：异步 HTTP
来源：http://sep.yuanzhike.top

aiohttp.ClientSession() 配合 async with
来源：http://xbt.guannengcc.top

[U28] Py：类型别名
来源：http://rum.0kj1m.cn

UserId = int
来源：http://qim.ydjk.org.cn

[U29] Py：属性校验
来源：http://slb.svipenyu.cn

@property 与 @x.setter 配合
来源：http://rrz.xziqi.cn

[U30] Py：数据类
来源：http://qpp.zdbjq.cn

@dataclass(slots=True)
来源：http://isl.chenjidiqi.icu

[U31] Py：单测
来源：http://zwf.hywenlv.cn

python -m pytest -q
来源：http://ajw.zhiwuduotai.top

[U32] Py：代码格式化
来源：http://jfk.nanxinkj.top

ruff format . && ruff check --fix .
来源：http://sqe.pengpengdd.cyou

[U33] Py：打包发布
来源：http://kld.quarkkingdee.top

python -m build  （依赖 pyproject.toml）
来源：http://yqg.zhongyouzk.top

[U34] Py：判断编码
来源：http://rqf.hongshengwenyu.top

chardet.detect(raw)
来源：http://huz.jinghuilouyu.cn

[U35] Py：发送邮件
来源：http://jlh.bbcook.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kps.yanxiufei.cn

[U36] Py：定时任务
来源：http://aro.nwbrower.top

schedule.every(10).minutes.do(job)
来源：http://gef.zdbjq.cn

[U37] Py：读写 Excel
来源：http://zpd.jinqigufen.top

pandas.read_excel / DataFrame.to_excel
来源：http://scv.hnxiangtu.top

[U38] Py：获取脚本所在目录
来源：http://uzt.fanxiaobao.xyz

Path(__file__).resolve().parent
来源：http://yos.gaohongyu789.top

[U39] Py：判断是否在交互环境
来源：http://ywt.chenjidiqi.icu

sys.stdout.isatty()
来源：http://wub.andypj.xyz

[U40] Py：打印到标准错误
来源：http://smh.dianchejie.cn

print("err", file=sys.stderr)
来源：http://bld.havefunace.top

[U41] PHP：初始化 Composer 项目
来源：http://yiz.cqqwz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://myc.dashuyun.cn

[U42] PHP：PSR-4 自动加载
来源：http://rtm.ehwqpu.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nkd.hysaishi.cn

[U43] PHP：声明命名空间
来源：http://rib.daxiang520.top

namespace App\Http;
来源：http://flc.daxiang520.top

[U44] PHP：开启严格类型
来源：http://nkc.shanyushiyangkeji.top

declare(strict_types=1);
来源：http://oui.ydjk.org.cn

[U45] PHP：类型声明与返回类型
来源：http://hvw.yj20258888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ikn.yuxming.cn

[U46] PHP：可空类型
来源：http://zdl.fktsv.cn

?string $name = null
来源：http://tzi.yongpay.top

[U47] PHP：联合类型
来源：http://xxc.cdnleiting.top

int|string $id
来源：http://ohw.iojbl.cn

[U48] PHP：纯枚举
来源：http://lwn.chenzaomai.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ymh.ppjwa.cn

[U49] PHP：只读属性
来源：http://xzx.yanxiufei.cn

public readonly string $name
来源：http://ato.yj20258.top

[U50] PHP：构造器属性提升
来源：http://dck.meibo888.top

public function __construct(private int $id) {}
来源：http://tlp.cdnleiting.top

[U51] PHP：数组解构
来源：http://bpa.chenzaomai.com

[$a, $b] = $arr;
来源：http://tbl.epnwcf.com

[U52] PHP：箭头函数
来源：http://nfn.hnxiangtu.top

$double = fn($x) => $x * 2;
来源：http://fhu.xinyue.icu

[U53] PHP：空合并运算符
来源：http://khh.zhoulong.xyz

$v = $a ?? $b ?? "default";
来源：http://fvx.guannengcc.top

[U54] PHP：空安全调用
来源：http://mzg.hysaishi.cn

$obj?->method()
来源：http://jka.0kj1m.cn

[U55] PHP：match 表达式
来源：http://dqs.birdmap.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://neg.fktsv.cn

[U56] PHP：命名参数
来源：http://lwk.sjlbkw.cn

f(a: 1, b: 2)
来源：http://web.cdnleiting.top

[U57] PHP：字符串插值
来源：http://mrd.mhx1999.top

"值: {$a}"
来源：http://pum.cdnleiting.top

[U58] PHP：数组三件套
来源：http://cxl.shuidangran.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fph.vehdjk.com

[U59] PHP：自定义排序
来源：http://ihu.zhijiandao.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://czc.chenjidiqi.icu

[U60] PHP：JSON 编解码
来源：http://hef.iojbl.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://itl.zhixingplan.top

[U61] PHP：正则
来源：http://wav.316326.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eqr.nanxuanxn.top

[U62] PHP：日期对象
来源：http://ywo.daxiang520.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lmf.hongshengwenyu.top

[U63] PHP：文件读写
来源：http://iwr.sweek.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://awt.nwbrower.top

[U64] PHP：目录遍历
来源：http://xhb.birdmap.top

glob("dir/*.php");  scandir("dir");
来源：http://ztt.xziqi.cn

[U65] PHP：会话
来源：http://hlp.jinqigufen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vwl.cashguo.top

[U66] PHP：设置 Cookie
来源：http://iro.316326.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mws.yangfankeji.com

[U67] PHP：处理文件上传
来源：http://ncq.jinghuilouyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vda.jqgufenzy.top

[U68] PHP：PDO 连接
来源：http://rwv.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fxc.yanxiufei.cn

[U69] PHP：PDO 预处理
来源：http://rxl.zhongyouzk.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dpb.yueranfly.top

[U70] PHP：PDO 事务
来源：http://sti.dashuyun.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gzb.daria6918.cn

[U71] PHP：抛出异常
来源：http://upw.ydzc1.top

throw new RuntimeException("失败", 500);
来源：http://orm.xuanzx.com

[U72] PHP：写错误日志
来源：http://qfr.yuxming.cn

error_log("失败: " . $e->getMessage());
来源：http://idn.shangyingyoupin.top

[U73] PHP：读取 ini 配置
来源：http://ffu.hysaishi.cn

parse_ini_file("config.ini", true)
来源：http://ynv.ydzc1.top

[U74] PHP：读取环境变量
来源：http://yvs.quarkkingdee.top

getenv("APP_ENV") ?: "production"
来源：http://iyh.fanxiaobao.xyz

[U75] PHP：依赖注入
来源：http://uca.yj20258.top

composer require psr/container
来源：http://gzr.hfpthk.cn

[U76] PHP：简单路由
来源：http://iqh.hcnkem.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hbc.sysykeji.top

[U77] PHP：模板渲染
来源：http://qug.zhixingplan.top

composer require twig/twig
来源：http://rjc.ppjwa.cn

[U78] PHP：单元测试
来源：http://qad.yueranfly.top

composer require --dev phpunit/phpunit
来源：http://zsr.9152youxi.cn

[U79] PHP：静态分析
来源：http://dal.xingfuxueyuan.xyz

composer require --dev phpstan/phpstan
来源：http://uhz.dianchejie.cn

[U80] PHP：代码规范修复
来源：http://ybx.chenlongwang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lpv.yueranfly.top

[U81] JS：初始化项目
来源：http://eao.yvedp.cn

npm init -y;  npm i express
来源：http://sin.nanxinkj.top

[U82] JS：package.json 脚本
来源：http://jbg.pengpengdd.cyou

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://usp.dianchejie.cn

[U83] JS：ES Module 导入导出
来源：http://edl.havefunace.top

export const a = 1;  import { a } from "./m.js";
来源：http://qib.yanxiufei.cn

[U84] JS：CommonJS 写法
来源：http://icw.guowangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://atl.gotoacloud.top

[U85] JS：可选链
来源：http://fqz.dashuyun.cn

a?.b?.c
来源：http://mfu.svipenyu.cn

[U86] JS：空值合并
来源：http://hzn.gaohongyu789.top

a ?? b
来源：http://kgf.xinyue.icu

[U87] JS：解构默认值
来源：http://kgs.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://hfj.sweek.top

[U88] JS：对象展开合并
来源：http://bsd.ivvv.top

{ ...a, ...b }
来源：http://for.hnqzz.top

[U89] JS：数组去重
来源：http://krb.dianchejie.cn

[...new Set(arr)]
来源：http://wty.ctjpmb.com

[U90] JS：数字数组排序
来源：http://iht.feifeiyinyue.top

[...arr].sort((a, b) => a - b)
来源：http://tgr.yj202588.top

[U91] JS：对象键值遍历
来源：http://fow.chenjidiqi.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://krt.gogol.net.cn

[U92] JS：深拷贝
来源：http://sue.jqgufenzy.top

structuredClone(obj)
来源：http://vsk.zycfv.cn

[U93] JS：模板字符串
来源：http://qow.jinqigufen.top

`共 ${n} 条`
来源：http://htl.iojbl.cn

[U94] JS：箭头函数
来源：http://sij.zhijiandao.cn

const double = x => x * 2;
来源：http://fcp.chenlongwang.top

[U95] JS：Promise 包装
来源：http://eyv.snrcjt.cn

new Promise((resolve, reject) => {})
来源：http://jft.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://vxj.shanyushiyangtech.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rwg.xinyue.icu

[U97] JS：并发请求
来源：http://ixc.yonumen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://sfi.xuanzx.com

[U98] JS：fetch 带 JSON
来源：http://dri.cqqwz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dyz.yueranfly.top

[U99] JS：事件监听
来源：http://gur.ywan-chungtsiang.top

el.addEventListener("click", e => {})
来源：http://xdk.hnxiangtu.top

[U100] JS：DOM 查询
来源：http://rvk.hfpthk.cn

document.querySelector(".item")
来源：http://gnf.hcnkem.com

[U101] JS：classList 操作
来源：http://wbn.redwolf501.top

el.classList.toggle("active")
来源：http://qon.nanxinkj.top

[U102] JS：本地存储
来源：http://fvi.gotoacloud.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xmx.jianghu66.top

[U103] JS：定时器
来源：http://oey.zycfv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sqv.chenzaomai.com

[U104] JS：防抖
来源：http://dka.vqdsnc.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://exl.birdmap.top

[U105] JS：节流
来源：http://qgb.yangfankeji.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rxv.cucudq.cn

[U106] JS：日期格式化
来源：http://esh.ivvv.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cmp.jqgfzy.top

[U107] JS：数字千分位
来源：http://ieg.redwolf501.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xat.cqqwz.cn

[U108] JS：随机整数
来源：http://jyc.quarkkingdee.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ifi.yj202588.top

[U109] JS：数组分组
来源：http://gmx.jinqigfzy.top

Object.groupBy(arr, x => x.type)
来源：http://voa.hcnkem.com

[U110] JS：数组分块
来源：http://dxr.ehwqpu.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wuq.svipenyu.cn

[U111] JS：对象转 Map
来源：http://zil.hesvh.cn

new Map(Object.entries(obj))
来源：http://djz.ctjpmb.com

[U112] JS：字符串补位
来源：http://upo.zhaomingkeji.xyz

"7".padStart(3, "0")
来源：http://lif.sweek.top

[U113] JS：正则替换全部
来源：http://zlf.sufxvd.cn

s.replaceAll("a", "b")
来源：http://gqf.hnxiangtu.top

[U114] JS：JSON 深比较
来源：http://hja.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ciu.iojbl.cn

[U115] JS：生成 UUID
来源：http://fwc.gogol.net.cn

crypto.randomUUID()
来源：http://oan.fanxiaobao.xyz

[U116] JS：类型检查（JSDoc）
来源：http://kho.xziqi.cn

/** @param {string} name */ function f(name) {}
来源：http://hdu.yonumen.top

[U117] JS：单元测试
来源：http://keh.shanyushiyangkeji.top

npm i -D vitest;  npx vitest
来源：http://ujt.xuetiantiany.cn

[U118] JS：开发服务器
来源：http://bak.ivvv.top

npm i -D vite;  npx vite
来源：http://iap.cashguo.top


<!-- 参考信息 -->