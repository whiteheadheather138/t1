代发 wailian999

[T33] Lua：表（数组）
来源：http://pap.yj20258888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jvb.wangdashe.top

[T34] Lua：遍历表
来源：http://lrn.shangyingyoupin.top

for i, v in ipairs(t) do print(i, v) end
来源：http://yqp.shzxlz.cn

[T35] Lua：字典表
来源：http://rrk.yueranfly.top

local d = { a = 1 };  d.b = 2
来源：http://wba.zhongyouzk.top

[T36] Lua：函数
来源：http://xzw.wangdashe.top

function add(a, b) return a + b end
来源：http://vcf.ctjpmb.com

[T37] Lua：字符串拼接
来源：http://dpq.tanke756.top

"a" .. "b"
来源：http://prr.dianchejie.cn

[T38] Lua：条件
来源：http://ash.yanxiufei.cn

if x > 0 then print("正") end
来源：http://cff.ehwqpu.com

[T39] Lua：模式匹配
来源：http://aas.pengpengdd.cyou

string.find(s, "%d+")
来源：http://yun.ywan-chungtsiang.top

[T40] Lua：元表
来源：http://ycs.xingfuxueyuan.xyz

setmetatable({}, { __index = base })
来源：http://knt.jyoumei.cn

[T41] Perl：Hello World
来源：http://uia.yonumen.top

print "Hello\n";
来源：http://niy.hcnkem.com

[T42] Perl：变量类型
来源：http://jed.cdnleiting.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pqk.guannengcc.top

[T43] Perl：字符串插值
来源：http://uqx.chenzaomai.com

"值: $a"
来源：http://ebt.pengpengdd.cyou

[T44] Perl：条件
来源：http://scl.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://rak.andypj.xyz

[T45] Perl：数组遍历
来源：http://onk.0kj1m.cn

for my $x (@arr) { print $x; }
来源：http://nhg.gaohongyu789.top

[T46] Perl：哈希操作
来源：http://izc.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dxz.jlsjyb.cn

[T47] Perl：正则捕获
来源：http://ytd.sufxvd.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yqb.hfpthk.cn

[T48] Perl：正则替换
来源：http://pnl.zhaomingkeji.xyz

$s =~ s/old/new/g;
来源：http://ydj.havefunace.top

[T49] Perl：函数
来源：http://oso.hnxiangtu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vmd.quarkkingdee.top

[T50] Perl：逐行读文件
来源：http://hrw.cheryme.top

open my $fh, "<", "a.txt" or die $!;
来源：http://esm.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://wnk.chenjidiqi.icu

[T51] Scala：Hello World
来源：http://wnr.pengpengdd.cyou

println("Hello")
来源：http://sji.chenzaomai.com

[T52] Scala：变量
来源：http://mxb.jinqigufen.top

val a = 1;  var b = 2
来源：http://erj.jiagoushi.top

[T53] Scala：字符串插值
来源：http://cov.sysykeji.top

s"值: $b"
来源：http://uts.uphjek.com

[T54] Scala：集合映射
来源：http://wxs.uphjek.com

List(1, 2, 3).map(_ * 2)
来源：http://lwq.meibo888.top

[T55] Scala：集合过滤
来源：http://tcx.yj202588.top

List(1, 2, 3).filter(_ > 1)
来源：http://adf.zhongyouzk.top

[T56] Scala：样例类
来源：http://qzt.sufxvd.cn

case class User(name: String, age: Int)
来源：http://dsr.feifeiyinyue.top

[T57] Scala：模式匹配
来源：http://ans.mhx1999.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ioy.yongpay.top

[T58] Scala：函数定义
来源：http://rjd.sysykeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://twt.haohaochexian.top

[T59] Scala：循环
来源：http://bmp.svipenyu.cn

for (i <- 1 to 10) println(i)
来源：http://qwk.xylfe.cn

[T60] Scala：折叠
来源：http://xfi.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qtw.jlsjyb.cn

================================================================================
来源：http://xyo.jinqigufen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ntx.bjfxy.top

================================================================================
来源：http://nxf.zhoulong.xyz

[U01] Py：创建虚拟环境
来源：http://jnz.svipenyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://goz.52xcode.cn

[U02] Py：导出 / 安装依赖
来源：http://alp.daria6918.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://npw.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://lnd.yj202588.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dri.yangfankeji.com

[U04] Py：变量调试打印
来源：http://fuw.hongshengwenyu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jzc.fktsv.cn

[U05] Py：列表去重且保序
来源：http://xwj.cucudq.cn

list(dict.fromkeys(arr))
来源：http://iqu.daria6918.cn

[U06] Py：合并两个字典
来源：http://rhr.yueranfly.top

{**a, **b}
来源：http://onz.wangdashe.top

[U07] Py：反转字典键值
来源：http://azi.sweek.top

{v: k for k, v in d.items()}
来源：http://prh.bjfxy.top

[U08] Py：展平二维列表
来源：http://xwg.fzhhl.top

[y for x in nested for y in x]
来源：http://lwm.yuxming.cn

[U09] Py：字典取最大值的键
来源：http://pzs.xylfe.cn

max(d, key=d.get)
来源：http://nxx.kuanghao11.cn

[U10] Py：按值排序字典
来源：http://zbe.cqqwz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vmh.jyoumei.cn

[U11] Py：生成器表达式
来源：http://shn.tarul.cn

(x * 2 for x in arr)
来源：http://qsd.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://cpg.sysykeji.top

Counter(arr).most_common(3)
来源：http://clr.pengpengdd.cyou

[U13] Py：固定长度队列
来源：http://qla.quarkkingdee.top

deque(maxlen=10)
来源：http://ano.zhongyouzk.top

[U14] Py：分组收集到列表
来源：http://qwy.zhiwuduotai.top

defaultdict(list)
来源：http://uya.hammf.cn

[U15] Py：高精度计时
来源：http://qcf.shanyushiyangtech.top

t = time.perf_counter()
来源：http://twi.havefunace.top

[U16] Py：命令行参数解析
来源：http://ots.nwbrower.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ftm.zhoulong.xyz

[U17] Py：初始化日志
来源：http://rmg.xuetiantiany.cn

logging.basicConfig(level=logging.INFO)
来源：http://blb.cdnleiting.top

[U18] Py：预编译正则
来源：http://ixu.jlsjyb.cn

pat = re.compile(r"\d+")
来源：http://exu.dashuyun.cn

[U19] Py：正则替换带回调
来源：http://fhv.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sou.yuxming.cn

[U20] Py：缓存函数结果
来源：http://tdl.jyoumei.cn

@functools.lru_cache(maxsize=None)
来源：http://mgu.snrcjt.cn

[U21] Py：自定义上下文管理器
来源：http://gfe.xziqi.cn

@contextlib.contextmanager
来源：http://gox.xziqi.cn

[U22] Py：矩阵转置
来源：http://wad.ctjpmb.com

list(zip(*m))
来源：http://odh.zhixingplan.top

[U23] Py：分块读取大文件
来源：http://ivm.tanke756.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bjc.yuanzhike.top

[U24] Py：路径操作
来源：http://xcv.birdmap.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dvk.yongpay.top

[U25] Py：CSV 按字典读
来源：http://aqx.hammf.cn

csv.DictReader(f)
来源：http://arx.uphjek.com

[U26] Py：并发下载
来源：http://sjb.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ntm.cqqwz.cn

[U27] Py：异步 HTTP
来源：http://weq.sxryk.cn

aiohttp.ClientSession() 配合 async with
来源：http://ndq.vqdsnc.cn

[U28] Py：类型别名
来源：http://rhm.hcnkem.com

UserId = int
来源：http://oqs.yuanzhike.top

[U29] Py：属性校验
来源：http://vpr.iojbl.cn

@property 与 @x.setter 配合
来源：http://rpx.nanxinkj.top

[U30] Py：数据类
来源：http://uea.jyoumei.cn

@dataclass(slots=True)
来源：http://cwe.xuanzx.com

[U31] Py：单测
来源：http://xlv.havefunace.top

python -m pytest -q
来源：http://epz.ivvv.top

[U32] Py：代码格式化
来源：http://gtv.9152youxi.cn

ruff format . && ruff check --fix .
来源：http://gyi.ybcxt.top

[U33] Py：打包发布
来源：http://zjq.shanyushiyangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://lmu.nanxinkj.top

[U34] Py：判断编码
来源：http://mjs.feifeiyinyue.top

chardet.detect(raw)
来源：http://cvk.xziqi.cn

[U35] Py：发送邮件
来源：http://hoj.jinyuanbaomall.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ync.iojbl.cn

[U36] Py：定时任务
来源：http://gum.daria6918.cn

schedule.every(10).minutes.do(job)
来源：http://mxq.daria6918.cn

[U37] Py：读写 Excel
来源：http://hgx.shanyushiyangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://vto.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://cfb.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://vun.yj20258.top

[U39] Py：判断是否在交互环境
来源：http://ufb.fzhhl.top

sys.stdout.isatty()
来源：http://hsn.ivvv.top

[U40] Py：打印到标准错误
来源：http://koy.hywenlv.cn

print("err", file=sys.stderr)
来源：http://tod.aibaodan.cn

[U41] PHP：初始化 Composer 项目
来源：http://beq.ctjpmb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://bqh.guowangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://lws.daria6918.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mmz.nwbrower.top

[U43] PHP：声明命名空间
来源：http://cou.dianchejie.cn

namespace App\Http;
来源：http://kwc.jqgfzy.top

[U44] PHP：开启严格类型
来源：http://eti.fehbvm.com

declare(strict_types=1);
来源：http://fpk.feifeiyinyue.top

[U45] PHP：类型声明与返回类型
来源：http://glc.cashguo.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pkd.yfazqb.com

[U46] PHP：可空类型
来源：http://xfl.sxryk.cn

?string $name = null
来源：http://omb.aizwys.cn

[U47] PHP：联合类型
来源：http://ryw.jiagoushi.top

int|string $id
来源：http://flt.epnwcf.com

[U48] PHP：纯枚举
来源：http://vje.guannengcc.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gto.vqdsnc.cn

[U49] PHP：只读属性
来源：http://uji.9152youxi.cn

public readonly string $name
来源：http://fvv.fanxiaobao.xyz

[U50] PHP：构造器属性提升
来源：http://ftr.yj202588.top

public function __construct(private int $id) {}
来源：http://mvj.yj202588.top

[U51] PHP：数组解构
来源：http://iqr.guannengcc.top

[$a, $b] = $arr;
来源：http://btr.yj20258888.top

[U52] PHP：箭头函数
来源：http://dxj.shuidangran.top

$double = fn($x) => $x * 2;
来源：http://eyk.sysykeji.top

[U53] PHP：空合并运算符
来源：http://law.vehdjk.com

$v = $a ?? $b ?? "default";
来源：http://ncu.hesvh.cn

[U54] PHP：空安全调用
来源：http://pas.daxiang520.top

$obj?->method()
来源：http://qix.nanxinkj.top

[U55] PHP：match 表达式
来源：http://tog.yuanzhike.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nch.hnqzz.top

[U56] PHP：命名参数
来源：http://whd.epnwcf.com

f(a: 1, b: 2)
来源：http://iyn.xuanzx.com

[U57] PHP：字符串插值
来源：http://pke.cashguo.top

"值: {$a}"
来源：http://xrw.shzxlz.cn

[U58] PHP：数组三件套
来源：http://jxn.cdnleiting.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ghc.tanke756.top

[U59] PHP：自定义排序
来源：http://jzn.ctjpmb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://olq.xziqi.cn

[U60] PHP：JSON 编解码
来源：http://vnq.yanxiufei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tct.feifeiyinyue.top

[U61] PHP：正则
来源：http://jjv.hammf.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dzu.mhx1999.top

[U62] PHP：日期对象
来源：http://vkq.9152youxi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bkw.epnwcf.com

[U63] PHP：文件读写
来源：http://ieq.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ejo.yangfankeji.com

[U64] PHP：目录遍历
来源：http://wne.haohaochexian.top

glob("dir/*.php");  scandir("dir");
来源：http://ail.shanyushiyangtech.top

[U65] PHP：会话
来源：http://kjs.jlsjyb.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tkx.0kj1m.cn

[U66] PHP：设置 Cookie
来源：http://ieu.wangshuangyany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pns.smart0.xyz

[U67] PHP：处理文件上传
来源：http://vnk.xinyue.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wmv.gzhubu.top

[U68] PHP：PDO 连接
来源：http://uap.sxryk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yle.zycfv.cn

[U69] PHP：PDO 预处理
来源：http://whz.zhengqikj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xbw.cheryme.top

[U70] PHP：PDO 事务
来源：http://zqy.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fbh.yj20258888.top

[U71] PHP：抛出异常
来源：http://roi.hammf.cn

throw new RuntimeException("失败", 500);
来源：http://ezt.hammf.cn

[U72] PHP：写错误日志
来源：http://jkb.zhixingplan.top

error_log("失败: " . $e->getMessage());
来源：http://pfx.gotoacloud.top

[U73] PHP：读取 ini 配置
来源：http://bmv.jiagoushi.top

parse_ini_file("config.ini", true)
来源：http://zrk.jlsjyb.cn

[U74] PHP：读取环境变量
来源：http://yez.jqgfzy.top

getenv("APP_ENV") ?: "production"
来源：http://aar.bjfxy.top

[U75] PHP：依赖注入
来源：http://qeq.yuxming.cn

composer require psr/container
来源：http://nzf.yvedp.cn

[U76] PHP：简单路由
来源：http://otj.ctjpmb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qsp.vqdsnc.cn

[U77] PHP：模板渲染
来源：http://iij.haohaochexian.top

composer require twig/twig
来源：http://zzw.chenjidiqi.icu

[U78] PHP：单元测试
来源：http://yxw.guannengcc.top

composer require --dev phpunit/phpunit
来源：http://hzz.zhongyouzk.top

[U79] PHP：静态分析
来源：http://vqz.yangfankeji.com

composer require --dev phpstan/phpstan
来源：http://pdk.daria6918.cn

[U80] PHP：代码规范修复
来源：http://fna.chenlongwang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nop.hysaishi.cn

[U81] JS：初始化项目
来源：http://djr.haohaochexian.top

npm init -y;  npm i express
来源：http://ofz.bbcook.cn

[U82] JS：package.json 脚本
来源：http://jqb.quarkkingdee.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pyq.zhixingplan.top

[U83] JS：ES Module 导入导出
来源：http://taf.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://apk.birdmap.top

[U84] JS：CommonJS 写法
来源：http://mvx.daxiang520.top

module.exports = { a };  const { a } = require("./m");
来源：http://lax.xziqi.cn

[U85] JS：可选链
来源：http://amd.gaohongyu789.top

a?.b?.c
来源：http://qhy.xinyue.icu

[U86] JS：空值合并
来源：http://tnq.andypj.xyz

a ?? b
来源：http://ick.bbcook.cn

[U87] JS：解构默认值
来源：http://pup.jinqigfzy.top

const { a = 1, b = 2 } = obj;
来源：http://ctu.ybcxt.top

[U88] JS：对象展开合并
来源：http://eiw.sysykeji.top

{ ...a, ...b }
来源：http://hwd.zdbjq.cn

[U89] JS：数组去重
来源：http://bsl.fanxiaobao.xyz

[...new Set(arr)]
来源：http://bfl.yuxming.cn

[U90] JS：数字数组排序
来源：http://rvz.meibo888.top

[...arr].sort((a, b) => a - b)
来源：http://osl.hysaishi.cn

[U91] JS：对象键值遍历
来源：http://jjk.shangyingyoupin.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qju.mhx1999.top

[U92] JS：深拷贝
来源：http://mmh.xinyue.icu

structuredClone(obj)
来源：http://tiy.jqgfzy.top

[U93] JS：模板字符串
来源：http://ucu.fehbvm.com

`共 ${n} 条`
来源：http://cbq.cheryme.top

[U94] JS：箭头函数
来源：http://wew.yongpay.top

const double = x => x * 2;
来源：http://xjl.zhoulong.xyz

[U95] JS：Promise 包装
来源：http://kbf.mhx1999.top

new Promise((resolve, reject) => {})
来源：http://sbs.yueranfly.top

[U96] JS：async/await 与异常
来源：http://tvf.snrcjt.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jvg.fktsv.cn

[U97] JS：并发请求
来源：http://xrb.fzhhl.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qqw.sysykeji.top

[U98] JS：fetch 带 JSON
来源：http://frq.xingfuxueyuan.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rxp.ivvv.top

[U99] JS：事件监听
来源：http://xqf.yj20258888.top

el.addEventListener("click", e => {})
来源：http://rmz.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://hhg.hongshengwenyu.top

document.querySelector(".item")
来源：http://snp.jinghuilouyu.cn

[U101] JS：classList 操作
来源：http://wqe.52xcode.cn

el.classList.toggle("active")
来源：http://inq.hysaishi.cn

[U102] JS：本地存储
来源：http://lno.hnqzz.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mox.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://qfa.shanyushiyangtech.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qqv.daria6918.cn

[U104] JS：防抖
来源：http://fgp.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lfu.bbcook.cn

[U105] JS：节流
来源：http://xgj.dianchejie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pcf.zhaomingkeji.xyz

[U106] JS：日期格式化
来源：http://wyz.epnwcf.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lyy.xuetiantiany.cn

[U107] JS：数字千分位
来源：http://hkf.shanyushiyangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zuv.xuanzx.com

[U108] JS：随机整数
来源：http://tkd.yuxming.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://csh.zhaomingkeji.xyz

[U109] JS：数组分组
来源：http://bha.yuxming.cn

Object.groupBy(arr, x => x.type)
来源：http://hbu.gogol.net.cn

[U110] JS：数组分块
来源：http://xkq.zhixingplan.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oce.shanyushiyangtech.top

[U111] JS：对象转 Map
来源：http://sgs.haohaochexian.top

new Map(Object.entries(obj))
来源：http://whl.jqgfzy.top

[U112] JS：字符串补位
来源：http://hcz.xuetiantiany.cn

"7".padStart(3, "0")
来源：http://zjc.9152youxi.cn

[U113] JS：正则替换全部
来源：http://pvz.zdbjq.cn

s.replaceAll("a", "b")
来源：http://kuj.aibaodan.cn

[U114] JS：JSON 深比较
来源：http://bxc.fehbvm.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://eep.gzhubu.top

[U115] JS：生成 UUID
来源：http://fpq.9152youxi.cn

crypto.randomUUID()
来源：http://pxq.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://kfz.yongpay.top

/** @param {string} name */ function f(name) {}
来源：http://ezh.chenlongwang.top

[U117] JS：单元测试
来源：http://pac.gotoacloud.top

npm i -D vitest;  npx vitest
来源：http://prg.nanxinkj.top

[U118] JS：开发服务器
来源：http://hku.vehdjk.com

npm i -D vite;  npx vite
来源：http://des.zhengqikj.top

[U119] JS：生产构建
来源：http://akq.bjfxy.top

npx vite build
来源：http://xpn.xylfe.cn

[U120] JS：读取环境变量（Vite）
来源：http://zee.c1oappe.top

import.meta.env.VITE_API_URL
来源：http://oqr.yongpay.top


<!-- 参考信息 -->