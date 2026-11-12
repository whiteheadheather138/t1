代发 wailian999

[T29] Swift：guard 提前返回
来源：http://jqp.xylfe.cn

guard let x = opt else { return }
来源：http://vyg.kuanghao11.cn

[T30] Swift：协议
来源：http://crp.cashguo.top

protocol Shape { func area() -> Double }
来源：http://cdp.zhiwuduotai.top

[T31] Lua：Hello World
来源：http://vty.pycfn.com

print("Hello")
来源：http://gub.xinyue.icu

[T32] Lua：局部变量
来源：http://pbu.ydzc1.top

local a = 1
来源：http://fmm.yueranfly.top

[T33] Lua：表（数组）
来源：http://ewl.xuetiantiany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hep.zhengqikj.top

[T34] Lua：遍历表
来源：http://yzb.wangshuangyany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rxm.hongshengwenyu.top

[T35] Lua：字典表
来源：http://kxf.sysykeji.top

local d = { a = 1 };  d.b = 2
来源：http://dmf.yj20258888.top

[T36] Lua：函数
来源：http://djb.xylfe.cn

function add(a, b) return a + b end
来源：http://ufd.cheryme.top

[T37] Lua：字符串拼接
来源：http://vhl.xinyue.icu

"a" .. "b"
来源：http://anj.redwolf501.top

[T38] Lua：条件
来源：http://uke.fanxiaobao.xyz

if x > 0 then print("正") end
来源：http://fom.chenzaomai.com

[T39] Lua：模式匹配
来源：http://cre.yonumen.top

string.find(s, "%d+")
来源：http://wci.meibo888.top

[T40] Lua：元表
来源：http://vrx.hcnkem.com

setmetatable({}, { __index = base })
来源：http://muc.snrcjt.cn

[T41] Perl：Hello World
来源：http://rte.vehdjk.com

print "Hello\n";
来源：http://alj.hysaishi.cn

[T42] Perl：变量类型
来源：http://xxa.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rwn.redwolf501.top

[T43] Perl：字符串插值
来源：http://xhs.xingfuxueyuan.xyz

"值: $a"
来源：http://yfw.haohaochexian.top

[T44] Perl：条件
来源：http://uxl.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://auz.cheryme.top

[T45] Perl：数组遍历
来源：http://mfq.zycfv.cn

for my $x (@arr) { print $x; }
来源：http://fnp.jqgufenzy.top

[T46] Perl：哈希操作
来源：http://jfk.9152youxi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ybu.jqgfzy.top

[T47] Perl：正则捕获
来源：http://wla.hysaishi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pgh.snrcjt.cn

[T48] Perl：正则替换
来源：http://ngq.ivvv.top

$s =~ s/old/new/g;
来源：http://kyd.guannengcc.top

[T49] Perl：函数
来源：http://ook.nwbrower.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ama.jlsjyb.cn

[T50] Perl：逐行读文件
来源：http://ixy.c1oappe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hxv.fanxiaobao.xyz

while (my $line = <$fh>) { print $line; }
来源：http://vfn.iojbl.cn

[T51] Scala：Hello World
来源：http://pty.sysykeji.top

println("Hello")
来源：http://nvq.yj20258888.top

[T52] Scala：变量
来源：http://lqd.ppjwa.cn

val a = 1;  var b = 2
来源：http://vwd.fzhhl.top

[T53] Scala：字符串插值
来源：http://yay.zdqjudy.top

s"值: $b"
来源：http://tuf.svipenyu.cn

[T54] Scala：集合映射
来源：http://yqe.jyoumei.cn

List(1, 2, 3).map(_ * 2)
来源：http://utg.hammf.cn

[T55] Scala：集合过滤
来源：http://uyt.havefunace.top

List(1, 2, 3).filter(_ > 1)
来源：http://tib.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://pqj.jyoumei.cn

case class User(name: String, age: Int)
来源：http://qqe.feifeiyinyue.top

[T57] Scala：模式匹配
来源：http://zpl.zhaomingkeji.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://ynd.hesvh.cn

[T58] Scala：函数定义
来源：http://xdx.hcnkem.com

def add(a: Int, b: Int): Int = a + b
来源：http://cuq.cheryme.top

[T59] Scala：循环
来源：http://bte.yuxming.cn

for (i <- 1 to 10) println(i)
来源：http://jju.svipenyu.cn

[T60] Scala：折叠
来源：http://fhl.zycfv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://znp.ppjwa.cn

================================================================================
来源：http://dxh.zhengqikj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://okm.ydzc1.top

================================================================================
来源：http://zqa.zhijiandao.cn

[U01] Py：创建虚拟环境
来源：http://hkj.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vgp.guannengcc.top

[U02] Py：导出 / 安装依赖
来源：http://fay.hammf.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gwy.fehbvm.com

[U03] Py：加载 .env 配置
来源：http://nln.fzhhl.top

from dotenv import load_dotenv; load_dotenv()
来源：http://eaw.cdnleiting.top

[U04] Py：变量调试打印
来源：http://mdd.zhongyouzk.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sco.meibo888.top

[U05] Py：列表去重且保序
来源：http://uew.tianlin.xyz

list(dict.fromkeys(arr))
来源：http://leo.chenzaomai.com

[U06] Py：合并两个字典
来源：http://glv.andypj.xyz

{**a, **b}
来源：http://txi.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://mha.hysaishi.cn

{v: k for k, v in d.items()}
来源：http://mdf.havefunace.top

[U08] Py：展平二维列表
来源：http://jvj.yongpay.top

[y for x in nested for y in x]
来源：http://ppf.jinghuilouyu.cn

[U09] Py：字典取最大值的键
来源：http://vaj.smart0.xyz

max(d, key=d.get)
来源：http://eyh.zycfv.cn

[U10] Py：按值排序字典
来源：http://iuv.shanyushiyangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sgc.xylfe.cn

[U11] Py：生成器表达式
来源：http://zmx.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://imx.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zhn.vqdsnc.cn

Counter(arr).most_common(3)
来源：http://dou.fzhhl.top

[U13] Py：固定长度队列
来源：http://fjt.epnwcf.com

deque(maxlen=10)
来源：http://ebc.snrcjt.cn

[U14] Py：分组收集到列表
来源：http://zry.wangdashe.top

defaultdict(list)
来源：http://nfj.uphjek.com

[U15] Py：高精度计时
来源：http://gab.gaohongyu789.top

t = time.perf_counter()
来源：http://fbu.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://xsq.ctjpmb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gah.andypj.xyz

[U17] Py：初始化日志
来源：http://xeg.chenjidiqi.icu

logging.basicConfig(level=logging.INFO)
来源：http://coi.mhx1999.top

[U18] Py：预编译正则
来源：http://qkl.pengpengdd.cyou

pat = re.compile(r"\d+")
来源：http://vyy.fktsv.cn

[U19] Py：正则替换带回调
来源：http://odl.sysykeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nyt.sxryk.cn

[U20] Py：缓存函数结果
来源：http://elo.yongpay.top

@functools.lru_cache(maxsize=None)
来源：http://anr.bjfxy.top

[U21] Py：自定义上下文管理器
来源：http://fch.pycfn.com

@contextlib.contextmanager
来源：http://que.xinyue.icu

[U22] Py：矩阵转置
来源：http://hum.jiagoushi.top

list(zip(*m))
来源：http://its.fanxiaobao.xyz

[U23] Py：分块读取大文件
来源：http://yss.cheryme.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://whr.bjfxy.top

[U24] Py：路径操作
来源：http://emo.fzhhl.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wus.tarul.cn

[U25] Py：CSV 按字典读
来源：http://bah.zdbjq.cn

csv.DictReader(f)
来源：http://myc.jiagoushi.top

[U26] Py：并发下载
来源：http://jpy.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pse.ydzc1.top

[U27] Py：异步 HTTP
来源：http://lrn.bjfxy.top

aiohttp.ClientSession() 配合 async with
来源：http://kxt.tianlin.xyz

[U28] Py：类型别名
来源：http://fom.fzhhl.top

UserId = int
来源：http://usn.fehbvm.com

[U29] Py：属性校验
来源：http://buq.zhiwuduotai.top

@property 与 @x.setter 配合
来源：http://hnk.wangdashe.top

[U30] Py：数据类
来源：http://stl.cqqwz.cn

@dataclass(slots=True)
来源：http://nvj.ywan-chungtsiang.top

[U31] Py：单测
来源：http://vsp.vehdjk.com

python -m pytest -q
来源：http://osz.yongpay.top

[U32] Py：代码格式化
来源：http://shc.yuxming.cn

ruff format . && ruff check --fix .
来源：http://mwu.hnxiangtu.top

[U33] Py：打包发布
来源：http://bmw.52xcode.cn

python -m build  （依赖 pyproject.toml）
来源：http://zlf.c1oappe.top

[U34] Py：判断编码
来源：http://blp.tian-w.cn

chardet.detect(raw)
来源：http://sqk.cashguo.top

[U35] Py：发送邮件
来源：http://npp.chenlongwang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ytv.zdqjudy.top

[U36] Py：定时任务
来源：http://xxu.smart0.xyz

schedule.every(10).minutes.do(job)
来源：http://gqi.nanxinkj.top

[U37] Py：读写 Excel
来源：http://nib.sxryk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cyy.yj20258888.top

[U38] Py：获取脚本所在目录
来源：http://qni.yongpay.top

Path(__file__).resolve().parent
来源：http://rdp.zhongyouzk.top

[U39] Py：判断是否在交互环境
来源：http://nwy.hongshengwenyu.top

sys.stdout.isatty()
来源：http://ymw.hnqzz.top

[U40] Py：打印到标准错误
来源：http://uxc.yanxiufei.cn

print("err", file=sys.stderr)
来源：http://eab.ywan-chungtsiang.top

[U41] PHP：初始化 Composer 项目
来源：http://qpu.yangfankeji.com

composer init;  composer require guzzlehttp/guzzle
来源：http://nkx.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://gvb.pycfn.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mht.redwolf501.top

[U43] PHP：声明命名空间
来源：http://knr.guannengcc.top

namespace App\Http;
来源：http://lks.jinqigfzy.top

[U44] PHP：开启严格类型
来源：http://und.jlsjyb.cn

declare(strict_types=1);
来源：http://uwc.xuanzx.com

[U45] PHP：类型声明与返回类型
来源：http://pcp.nwbrower.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hby.sjlbkw.cn

[U46] PHP：可空类型
来源：http://bfe.shzxlz.cn

?string $name = null
来源：http://ytk.0kj1m.cn

[U47] PHP：联合类型
来源：http://pck.shangyingyoupin.top

int|string $id
来源：http://yqv.pengpengdd.cyou

[U48] PHP：纯枚举
来源：http://ehy.vehdjk.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xbm.dianchejie.cn

[U49] PHP：只读属性
来源：http://ktv.ivvv.top

public readonly string $name
来源：http://dwr.sysykeji.top

[U50] PHP：构造器属性提升
来源：http://xrx.yfazqb.com

public function __construct(private int $id) {}
来源：http://dnt.52xcode.cn

[U51] PHP：数组解构
来源：http://wzl.sufxvd.cn

[$a, $b] = $arr;
来源：http://ybk.xinyue.icu

[U52] PHP：箭头函数
来源：http://ovb.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://uoo.ivvv.top

[U53] PHP：空合并运算符
来源：http://sum.ctjpmb.com

$v = $a ?? $b ?? "default";
来源：http://psf.snrcjt.cn

[U54] PHP：空安全调用
来源：http://axh.chenzaomai.com

$obj?->method()
来源：http://knh.cheryme.top

[U55] PHP：match 表达式
来源：http://erx.zdbjq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oij.nanxuanxn.top

[U56] PHP：命名参数
来源：http://qvr.pycfn.com

f(a: 1, b: 2)
来源：http://duv.chenlongwang.top

[U57] PHP：字符串插值
来源：http://mpo.wangdashe.top

"值: {$a}"
来源：http://yyt.meibo888.top

[U58] PHP：数组三件套
来源：http://bth.hnxiangtu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://irj.haohaochexian.top

[U59] PHP：自定义排序
来源：http://xst.jiagoushi.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qec.jyoumei.cn

[U60] PHP：JSON 编解码
来源：http://cic.havefunace.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bbr.gogol.net.cn

[U61] PHP：正则
来源：http://pcc.gaohongyu789.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nyx.tanke756.top

[U62] PHP：日期对象
来源：http://gfo.fehbvm.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hgz.yanxiufei.cn

[U63] PHP：文件读写
来源：http://qiz.zhiwuduotai.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dii.andypj.xyz

[U64] PHP：目录遍历
来源：http://igu.nanxuanxn.top

glob("dir/*.php");  scandir("dir");
来源：http://vio.uphjek.com

[U65] PHP：会话
来源：http://sqr.jinghuilouyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kbw.fanxiaobao.xyz

[U66] PHP：设置 Cookie
来源：http://lrv.cucudq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://esp.fanxiaobao.xyz

[U67] PHP：处理文件上传
来源：http://thy.gogol.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fvp.smart0.xyz

[U68] PHP：PDO 连接
来源：http://zjr.52xcode.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dmc.zhijiandao.cn

[U69] PHP：PDO 预处理
来源：http://dba.ppjwa.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hph.xinyue.icu

[U70] PHP：PDO 事务
来源：http://ggg.fktsv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qss.fengsongda.top

[U71] PHP：抛出异常
来源：http://hav.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://ozw.yuxming.cn

[U72] PHP：写错误日志
来源：http://xae.aibaodan.cn

error_log("失败: " . $e->getMessage());
来源：http://qar.vehdjk.com

[U73] PHP：读取 ini 配置
来源：http://yov.tanke756.top

parse_ini_file("config.ini", true)
来源：http://uqs.andypj.xyz

[U74] PHP：读取环境变量
来源：http://vnz.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://ztq.zhiwuduotai.top

[U75] PHP：依赖注入
来源：http://scn.svipenyu.cn

composer require psr/container
来源：http://odt.aibaodan.cn

[U76] PHP：简单路由
来源：http://qkx.sxryk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wls.gogol.net.cn

[U77] PHP：模板渲染
来源：http://ozt.hysaishi.cn

composer require twig/twig
来源：http://ino.smart0.xyz

[U78] PHP：单元测试
来源：http://cjr.fanxiaobao.xyz

composer require --dev phpunit/phpunit
来源：http://rzz.jqgfzy.top

[U79] PHP：静态分析
来源：http://zet.daxiang520.top

composer require --dev phpstan/phpstan
来源：http://stz.hysaishi.cn

[U80] PHP：代码规范修复
来源：http://naj.yj20258888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zhi.sysykeji.top

[U81] JS：初始化项目
来源：http://uev.hfpthk.cn

npm init -y;  npm i express
来源：http://rdl.zhongyouzk.top

[U82] JS：package.json 脚本
来源：http://cgd.tianlin.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bzg.xuanzx.com

[U83] JS：ES Module 导入导出
来源：http://ovk.shzxlz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fda.hammf.cn

[U84] JS：CommonJS 写法
来源：http://pqd.fzhhl.top

module.exports = { a };  const { a } = require("./m");
来源：http://rif.xuetiantiany.cn

[U85] JS：可选链
来源：http://cuh.gaohongyu789.top

a?.b?.c
来源：http://hjv.sweek.top

[U86] JS：空值合并
来源：http://vqe.sufxvd.cn

a ?? b
来源：http://qne.jlsjyb.cn

[U87] JS：解构默认值
来源：http://wqw.sufxvd.cn

const { a = 1, b = 2 } = obj;
来源：http://mnw.gaohongyu789.top

[U88] JS：对象展开合并
来源：http://qqr.tian-w.cn

{ ...a, ...b }
来源：http://okh.tarul.cn

[U89] JS：数组去重
来源：http://sht.yangfankeji.com

[...new Set(arr)]
来源：http://mcg.yj20258.top

[U90] JS：数字数组排序
来源：http://uxn.yj202588.top

[...arr].sort((a, b) => a - b)
来源：http://hcc.nanxinkj.top

[U91] JS：对象键值遍历
来源：http://ibo.vqdsnc.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zps.cdnleiting.top

[U92] JS：深拷贝
来源：http://zth.ydjk.org.cn

structuredClone(obj)
来源：http://dew.chenjidiqi.icu

[U93] JS：模板字符串
来源：http://qtp.zhaomingkeji.xyz

`共 ${n} 条`
来源：http://msc.epnwcf.com

[U94] JS：箭头函数
来源：http://xmt.epnwcf.com

const double = x => x * 2;
来源：http://ouk.xuanzx.com

[U95] JS：Promise 包装
来源：http://rsq.chenlongwang.top

new Promise((resolve, reject) => {})
来源：http://yvf.daria6918.cn

[U96] JS：async/await 与异常
来源：http://bjf.cashguo.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rux.guannengcc.top

[U97] JS：并发请求
来源：http://ipm.fktsv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tqf.svipenyu.cn

[U98] JS：fetch 带 JSON
来源：http://pjb.xuetiantiany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://elx.9152youxi.cn

[U99] JS：事件监听
来源：http://vzw.ivvv.top

el.addEventListener("click", e => {})
来源：http://sks.fanxiaobao.xyz

[U100] JS：DOM 查询
来源：http://svt.yj202588.top

document.querySelector(".item")
来源：http://bwi.ctjpmb.com

[U101] JS：classList 操作
来源：http://otj.zycfv.cn

el.classList.toggle("active")
来源：http://pih.xinyue.icu

[U102] JS：本地存储
来源：http://zlf.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ndu.fzhhl.top

[U103] JS：定时器
来源：http://kwt.zhoulong.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://osx.zycfv.cn

[U104] JS：防抖
来源：http://shd.cashguo.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mkq.nanxinkj.top

[U105] JS：节流
来源：http://tjs.xziqi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qwl.zhixingplan.top

[U106] JS：日期格式化
来源：http://wuy.ehwqpu.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fit.yfazqb.com

[U107] JS：数字千分位
来源：http://tkk.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eas.ywan-chungtsiang.top

[U108] JS：随机整数
来源：http://adw.xylfe.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yrs.bjfxy.top

[U109] JS：数组分组
来源：http://nex.hesvh.cn

Object.groupBy(arr, x => x.type)
来源：http://ygq.kuanghao11.cn

[U110] JS：数组分块
来源：http://bjp.hywenlv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qhv.ywan-chungtsiang.top

[U111] JS：对象转 Map
来源：http://ilc.yueranfly.top

new Map(Object.entries(obj))
来源：http://hpx.sjlbkw.cn

[U112] JS：字符串补位
来源：http://crn.snrcjt.cn

"7".padStart(3, "0")
来源：http://ivc.hongshengwenyu.top

[U113] JS：正则替换全部
来源：http://rik.yj20258.top

s.replaceAll("a", "b")
来源：http://jku.sweek.top

[U114] JS：JSON 深比较
来源：http://syq.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yzm.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://opn.smart0.xyz

crypto.randomUUID()
来源：http://vds.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://vws.hammf.cn

/** @param {string} name */ function f(name) {}
来源：http://xif.feifeiyinyue.top


<!-- 参考信息 -->