代发 wailian999

[T29] Swift：guard 提前返回
来源：http://bfl.epnwcf.com

guard let x = opt else { return }
来源：http://icq.smart0.xyz

[T30] Swift：协议
来源：http://mfu.fehbvm.com

protocol Shape { func area() -> Double }
来源：http://vit.yongpay.top

[T31] Lua：Hello World
来源：http://jsj.cdnleiting.top

print("Hello")
来源：http://shy.9152youxi.cn

[T32] Lua：局部变量
来源：http://ahz.52xcode.cn

local a = 1
来源：http://inu.zhongyouzk.top

[T33] Lua：表（数组）
来源：http://qcu.sweek.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zbt.cashguo.top

[T34] Lua：遍历表
来源：http://uhv.redwolf501.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qaj.hammf.cn

[T35] Lua：字典表
来源：http://gff.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://nhj.chenlongwang.top

[T36] Lua：函数
来源：http://rpb.tanke756.top

function add(a, b) return a + b end
来源：http://uok.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://mif.cdnleiting.top

"a" .. "b"
来源：http://ure.ivvv.top

[T38] Lua：条件
来源：http://owc.vqdsnc.cn

if x > 0 then print("正") end
来源：http://ywl.hysaishi.cn

[T39] Lua：模式匹配
来源：http://ghj.zhixingplan.top

string.find(s, "%d+")
来源：http://bls.uphjek.com

[T40] Lua：元表
来源：http://nbt.jinyuanbaomall.cn

setmetatable({}, { __index = base })
来源：http://dod.yonumen.top

[T41] Perl：Hello World
来源：http://zzz.yj202588.top

print "Hello\n";
来源：http://vkm.andypj.xyz

[T42] Perl：变量类型
来源：http://wtd.nanxinkj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qdz.shzxlz.cn

[T43] Perl：字符串插值
来源：http://oce.bbcook.cn

"值: $a"
来源：http://drf.hfpthk.cn

[T44] Perl：条件
来源：http://mxj.zhijiandao.cn

if ($a > 0) { print "正"; }
来源：http://udc.xuetiantiany.cn

[T45] Perl：数组遍历
来源：http://faw.tianlin.xyz

for my $x (@arr) { print $x; }
来源：http://gqg.ybcxt.top

[T46] Perl：哈希操作
来源：http://xoh.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tsu.meibo888.top

[T47] Perl：正则捕获
来源：http://djp.jlsjyb.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://brp.0kj1m.cn

[T48] Perl：正则替换
来源：http://mjb.ehwqpu.com

$s =~ s/old/new/g;
来源：http://qww.316326.xyz

[T49] Perl：函数
来源：http://utx.zhixingplan.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uqd.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://ydi.shuidangran.top

open my $fh, "<", "a.txt" or die $!;
来源：http://knv.chenlongwang.top

while (my $line = <$fh>) { print $line; }
来源：http://qnf.zycfv.cn

[T51] Scala：Hello World
来源：http://xhj.tarul.cn

println("Hello")
来源：http://gjr.zhiwuduotai.top

[T52] Scala：变量
来源：http://pdf.jqgufenzy.top

val a = 1;  var b = 2
来源：http://mhx.guowangkeji.top

[T53] Scala：字符串插值
来源：http://aml.xingfuxueyuan.xyz

s"值: $b"
来源：http://wqq.aibaodan.cn

[T54] Scala：集合映射
来源：http://qfi.chenlongwang.top

List(1, 2, 3).map(_ * 2)
来源：http://aao.yj20258.top

[T55] Scala：集合过滤
来源：http://iqv.9152youxi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uuv.ctjpmb.com

[T56] Scala：样例类
来源：http://fxv.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://jee.jianghu66.top

[T57] Scala：模式匹配
来源：http://nlp.yfazqb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://fsg.chenzaomai.com

[T58] Scala：函数定义
来源：http://dcu.epnwcf.com

def add(a: Int, b: Int): Int = a + b
来源：http://sgm.aibaodan.cn

[T59] Scala：循环
来源：http://vvv.yj202588.top

for (i <- 1 to 10) println(i)
来源：http://bmc.fengsongda.top

[T60] Scala：折叠
来源：http://iwt.tianlin.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ahx.gotoacloud.top

================================================================================
来源：http://eup.wangdashe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://thj.hywenlv.cn

================================================================================
来源：http://npl.xuetiantiany.cn

[U01] Py：创建虚拟环境
来源：http://eap.tian-w.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tku.316326.xyz

[U02] Py：导出 / 安装依赖
来源：http://bqt.haohaochexian.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hvb.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://wgp.zhixingplan.top

from dotenv import load_dotenv; load_dotenv()
来源：http://oiu.aibaodan.cn

[U04] Py：变量调试打印
来源：http://iuj.xziqi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://riv.uphjek.com

[U05] Py：列表去重且保序
来源：http://gju.mhx1999.top

list(dict.fromkeys(arr))
来源：http://vsq.smart0.xyz

[U06] Py：合并两个字典
来源：http://etf.yfazqb.com

{**a, **b}
来源：http://qus.yonumen.top

[U07] Py：反转字典键值
来源：http://juo.xinyue.icu

{v: k for k, v in d.items()}
来源：http://ybs.yangfankeji.com

[U08] Py：展平二维列表
来源：http://tzi.kuanghao11.cn

[y for x in nested for y in x]
来源：http://yim.yj202588.top

[U09] Py：字典取最大值的键
来源：http://ddd.xingfuxueyuan.xyz

max(d, key=d.get)
来源：http://izf.zycfv.cn

[U10] Py：按值排序字典
来源：http://slm.dianchejie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eyb.shangyingyoupin.top

[U11] Py：生成器表达式
来源：http://ohp.xuanzx.com

(x * 2 for x in arr)
来源：http://lhy.zhiwuduotai.top

[U12] Py：取出现最多的 3 个元素
来源：http://bgh.yangfankeji.com

Counter(arr).most_common(3)
来源：http://jwr.jinqigufen.top

[U13] Py：固定长度队列
来源：http://yzq.zhengqikj.top

deque(maxlen=10)
来源：http://jlw.fengsongda.top

[U14] Py：分组收集到列表
来源：http://iwu.fzhhl.top

defaultdict(list)
来源：http://pwa.yj20258888.top

[U15] Py：高精度计时
来源：http://ozg.bjfxy.top

t = time.perf_counter()
来源：http://moa.shanyushiyangtech.top

[U16] Py：命令行参数解析
来源：http://cxr.pycfn.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hic.cdnleiting.top

[U17] Py：初始化日志
来源：http://vso.0kj1m.cn

logging.basicConfig(level=logging.INFO)
来源：http://gnr.zhixingplan.top

[U18] Py：预编译正则
来源：http://myc.yj20258.top

pat = re.compile(r"\d+")
来源：http://fiw.zhixingplan.top

[U19] Py：正则替换带回调
来源：http://sme.jinqigufen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://anl.uphjek.com

[U20] Py：缓存函数结果
来源：http://boq.birdmap.top

@functools.lru_cache(maxsize=None)
来源：http://lsh.jinqigufen.top

[U21] Py：自定义上下文管理器
来源：http://pxk.uphjek.com

@contextlib.contextmanager
来源：http://whi.iojbl.cn

[U22] Py：矩阵转置
来源：http://zwl.cashguo.top

list(zip(*m))
来源：http://nhh.nwbrower.top

[U23] Py：分块读取大文件
来源：http://mrw.jinqigufen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wdb.gotoacloud.top

[U24] Py：路径操作
来源：http://syp.tianlin.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gio.zhixingplan.top

[U25] Py：CSV 按字典读
来源：http://mkc.cdnleiting.top

csv.DictReader(f)
来源：http://wvd.yj20258888.top

[U26] Py：并发下载
来源：http://cwu.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rpa.jinqigufen.top

[U27] Py：异步 HTTP
来源：http://qfr.bbcook.cn

aiohttp.ClientSession() 配合 async with
来源：http://dan.nanxinkj.top

[U28] Py：类型别名
来源：http://pqm.yvedp.cn

UserId = int
来源：http://siq.dianchejie.cn

[U29] Py：属性校验
来源：http://kqh.cucudq.cn

@property 与 @x.setter 配合
来源：http://cnj.zhoulong.xyz

[U30] Py：数据类
来源：http://lzx.hesvh.cn

@dataclass(slots=True)
来源：http://luo.andypj.xyz

[U31] Py：单测
来源：http://njk.hnqzz.top

python -m pytest -q
来源：http://kfy.jinghuilouyu.cn

[U32] Py：代码格式化
来源：http://xjt.yj202588.top

ruff format . && ruff check --fix .
来源：http://gmx.daria6918.cn

[U33] Py：打包发布
来源：http://zks.shuidangran.top

python -m build  （依赖 pyproject.toml）
来源：http://ipb.jinqigufen.top

[U34] Py：判断编码
来源：http://xfy.sufxvd.cn

chardet.detect(raw)
来源：http://lak.zhongyouzk.top

[U35] Py：发送邮件
来源：http://mes.hfpthk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vcp.jiagoushi.top

[U36] Py：定时任务
来源：http://bel.ybcxt.top

schedule.every(10).minutes.do(job)
来源：http://yob.chenlongwang.top

[U37] Py：读写 Excel
来源：http://jfg.shuidangran.top

pandas.read_excel / DataFrame.to_excel
来源：http://fyy.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://voa.snrcjt.cn

Path(__file__).resolve().parent
来源：http://alr.hnqzz.top

[U39] Py：判断是否在交互环境
来源：http://bzp.jinqigfzy.top

sys.stdout.isatty()
来源：http://xbd.yj20258888.top

[U40] Py：打印到标准错误
来源：http://sjj.dashuyun.cn

print("err", file=sys.stderr)
来源：http://khu.yangfankeji.com

[U41] PHP：初始化 Composer 项目
来源：http://mhz.hnxiangtu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bph.andypj.xyz

[U42] PHP：PSR-4 自动加载
来源：http://uwx.jinqigufen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tyo.sufxvd.cn

[U43] PHP：声明命名空间
来源：http://jlb.ywan-chungtsiang.top

namespace App\Http;
来源：http://fri.c1oappe.top

[U44] PHP：开启严格类型
来源：http://qlk.chenzaomai.com

declare(strict_types=1);
来源：http://kti.xylfe.cn

[U45] PHP：类型声明与返回类型
来源：http://oan.quarkkingdee.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://cug.hongshengwenyu.top

[U46] PHP：可空类型
来源：http://ocr.jinyuanbaomall.cn

?string $name = null
来源：http://yie.vqdsnc.cn

[U47] PHP：联合类型
来源：http://qvz.sysykeji.top

int|string $id
来源：http://wge.zhengqikj.top

[U48] PHP：纯枚举
来源：http://rsn.snrcjt.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zbi.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://pyy.aibaodan.cn

public readonly string $name
来源：http://ldz.ehwqpu.com

[U50] PHP：构造器属性提升
来源：http://snm.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://tii.sufxvd.cn

[U51] PHP：数组解构
来源：http://mtt.nwbrower.top

[$a, $b] = $arr;
来源：http://alv.daria6918.cn

[U52] PHP：箭头函数
来源：http://goo.yangfankeji.com

$double = fn($x) => $x * 2;
来源：http://jyc.birdmap.top

[U53] PHP：空合并运算符
来源：http://kwo.xinyue.icu

$v = $a ?? $b ?? "default";
来源：http://gyg.daria6918.cn

[U54] PHP：空安全调用
来源：http://pmr.cdnleiting.top

$obj?->method()
来源：http://bmj.tian-w.cn

[U55] PHP：match 表达式
来源：http://wgg.ydzc1.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pqn.yvedp.cn

[U56] PHP：命名参数
来源：http://gwx.zhixingplan.top

f(a: 1, b: 2)
来源：http://mqt.zdbjq.cn

[U57] PHP：字符串插值
来源：http://orm.birdmap.top

"值: {$a}"
来源：http://jtw.zhiwuduotai.top

[U58] PHP：数组三件套
来源：http://klt.zycfv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pul.sjlbkw.cn

[U59] PHP：自定义排序
来源：http://uon.cdnleiting.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hrf.svipenyu.cn

[U60] PHP：JSON 编解码
来源：http://ynq.pengpengdd.cyou

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://opp.shzxlz.cn

[U61] PHP：正则
来源：http://hae.gogol.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://omr.sxryk.cn

[U62] PHP：日期对象
来源：http://fkd.zdqjudy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qar.vqdsnc.cn

[U63] PHP：文件读写
来源：http://qya.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ppz.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://szw.yangfankeji.com

glob("dir/*.php");  scandir("dir");
来源：http://dig.cucudq.cn

[U65] PHP：会话
来源：http://ein.aizwys.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mpy.cdnleiting.top

[U66] PHP：设置 Cookie
来源：http://ojj.jlsjyb.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tro.fehbvm.com

[U67] PHP：处理文件上传
来源：http://qrs.zhongyouzk.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://waw.ydzc1.top

[U68] PHP：PDO 连接
来源：http://kwg.fehbvm.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nsu.sxryk.cn

[U69] PHP：PDO 预处理
来源：http://gcj.c1oappe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lvh.yuanzhike.top

[U70] PHP：PDO 事务
来源：http://rxu.jlsjyb.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jhp.feifeiyinyue.top

[U71] PHP：抛出异常
来源：http://fca.jinghuilouyu.cn

throw new RuntimeException("失败", 500);
来源：http://bqj.ydjk.org.cn

[U72] PHP：写错误日志
来源：http://ggl.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://edg.zhengqikj.top

[U73] PHP：读取 ini 配置
来源：http://rsl.sxryk.cn

parse_ini_file("config.ini", true)
来源：http://jhq.yvedp.cn

[U74] PHP：读取环境变量
来源：http://hpf.hysaishi.cn

getenv("APP_ENV") ?: "production"
来源：http://lid.nanxinkj.top

[U75] PHP：依赖注入
来源：http://hyn.andypj.xyz

composer require psr/container
来源：http://nej.fehbvm.com

[U76] PHP：简单路由
来源：http://lya.jinqigfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sqe.zhengqikj.top

[U77] PHP：模板渲染
来源：http://xgo.xuetiantiany.cn

composer require twig/twig
来源：http://tdq.chenlongwang.top

[U78] PHP：单元测试
来源：http://foq.hammf.cn

composer require --dev phpunit/phpunit
来源：http://dgw.hfpthk.cn

[U79] PHP：静态分析
来源：http://buz.smart0.xyz

composer require --dev phpstan/phpstan
来源：http://lce.zdbjq.cn

[U80] PHP：代码规范修复
来源：http://bpm.daria6918.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fsi.jlsjyb.cn

[U81] JS：初始化项目
来源：http://tbb.xylfe.cn

npm init -y;  npm i express
来源：http://yxh.sufxvd.cn

[U82] JS：package.json 脚本
来源：http://tst.zhaomingkeji.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tui.gaohongyu789.top

[U83] JS：ES Module 导入导出
来源：http://rxr.wangdashe.top

export const a = 1;  import { a } from "./m.js";
来源：http://hly.sjlbkw.cn

[U84] JS：CommonJS 写法
来源：http://xzw.hongshengwenyu.top

module.exports = { a };  const { a } = require("./m");
来源：http://ssn.guowangkeji.top

[U85] JS：可选链
来源：http://lqj.c1oappe.top

a?.b?.c
来源：http://xxg.zdbjq.cn

[U86] JS：空值合并
来源：http://nfq.hongshengwenyu.top

a ?? b
来源：http://xkf.9152youxi.cn

[U87] JS：解构默认值
来源：http://esk.quarkkingdee.top

const { a = 1, b = 2 } = obj;
来源：http://dex.mhx1999.top

[U88] JS：对象展开合并
来源：http://jpw.jinghuilouyu.cn

{ ...a, ...b }
来源：http://qis.sxryk.cn

[U89] JS：数组去重
来源：http://jzw.52xcode.cn

[...new Set(arr)]
来源：http://gkn.gaohongyu789.top

[U90] JS：数字数组排序
来源：http://gfk.aizwys.cn

[...arr].sort((a, b) => a - b)
来源：http://lyd.vehdjk.com

[U91] JS：对象键值遍历
来源：http://ogs.wangdashe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rjv.yanxiufei.cn

[U92] JS：深拷贝
来源：http://mux.sxryk.cn

structuredClone(obj)
来源：http://tfr.zhaomingkeji.xyz

[U93] JS：模板字符串
来源：http://nkn.xingfuxueyuan.xyz

`共 ${n} 条`
来源：http://rvo.yuxming.cn

[U94] JS：箭头函数
来源：http://nyc.yongpay.top

const double = x => x * 2;
来源：http://gxc.yangfankeji.com

[U95] JS：Promise 包装
来源：http://kef.hcnkem.com

new Promise((resolve, reject) => {})
来源：http://ibt.jinyuanbaomall.cn

[U96] JS：async/await 与异常
来源：http://nzt.bbcook.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://haa.zhengqikj.top

[U97] JS：并发请求
来源：http://wcd.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://qnm.hammf.cn

[U98] JS：fetch 带 JSON
来源：http://lgy.chenlongwang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tlh.nanxuanxn.top

[U99] JS：事件监听
来源：http://rbm.daxiang520.top

el.addEventListener("click", e => {})
来源：http://fqs.nanxinkj.top

[U100] JS：DOM 查询
来源：http://omj.hesvh.cn

document.querySelector(".item")
来源：http://vtu.hnxiangtu.top

[U101] JS：classList 操作
来源：http://bob.shzxlz.cn

el.classList.toggle("active")
来源：http://sgy.yj202588.top

[U102] JS：本地存储
来源：http://cgg.birdmap.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jdt.shuidangran.top

[U103] JS：定时器
来源：http://lfz.ydzc1.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bsf.redwolf501.top

[U104] JS：防抖
来源：http://fqf.chenzaomai.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gny.jiagoushi.top

[U105] JS：节流
来源：http://lea.andypj.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qmt.yj202588.top

[U106] JS：日期格式化
来源：http://eqc.zhiwuduotai.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pmg.fehbvm.com

[U107] JS：数字千分位
来源：http://qgs.aibaodan.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lqr.yueranfly.top

[U108] JS：随机整数
来源：http://mcb.aibaodan.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://atd.yueranfly.top

[U109] JS：数组分组
来源：http://kwf.ydzc1.top

Object.groupBy(arr, x => x.type)
来源：http://qxz.birdmap.top

[U110] JS：数组分块
来源：http://uos.hywenlv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qlg.redwolf501.top

[U111] JS：对象转 Map
来源：http://xzp.52xcode.cn

new Map(Object.entries(obj))
来源：http://wvq.feifeiyinyue.top

[U112] JS：字符串补位
来源：http://xhn.ydzc1.top

"7".padStart(3, "0")
来源：http://jcf.xingfuxueyuan.xyz

[U113] JS：正则替换全部
来源：http://ukh.hysaishi.cn

s.replaceAll("a", "b")
来源：http://uhy.aibaodan.cn

[U114] JS：JSON 深比较
来源：http://yaf.feifeiyinyue.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://axl.guowangkeji.top

[U115] JS：生成 UUID
来源：http://vwu.tian-w.cn

crypto.randomUUID()
来源：http://ecc.sjlbkw.cn

[U116] JS：类型检查（JSDoc）
来源：http://noh.jinghuilouyu.cn

/** @param {string} name */ function f(name) {}
来源：http://rcs.vehdjk.com


<!-- 参考信息 -->