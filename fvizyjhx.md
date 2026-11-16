代发 wailian999

[T29] Swift：guard 提前返回
来源：http://mbq.bbcook.cn

guard let x = opt else { return }
来源：http://hzf.xuanzx.com

[T30] Swift：协议
来源：http://mmq.yangfankeji.com

protocol Shape { func area() -> Double }
来源：http://fsw.hywenlv.cn

[T31] Lua：Hello World
来源：http://kfg.cdnleiting.top

print("Hello")
来源：http://zgk.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://jbc.aizwys.cn

local a = 1
来源：http://qqj.yfazqb.com

[T33] Lua：表（数组）
来源：http://hsr.yvedp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nnl.iojbl.cn

[T34] Lua：遍历表
来源：http://swj.jyoumei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://znh.guowangkeji.top

[T35] Lua：字典表
来源：http://asf.epnwcf.com

local d = { a = 1 };  d.b = 2
来源：http://lcw.zycfv.cn

[T36] Lua：函数
来源：http://ypg.fktsv.cn

function add(a, b) return a + b end
来源：http://tzz.shuidangran.top

[T37] Lua：字符串拼接
来源：http://vnn.yj20258.top

"a" .. "b"
来源：http://lux.aibaodan.cn

[T38] Lua：条件
来源：http://pyt.hnxiangtu.top

if x > 0 then print("正") end
来源：http://pov.sjlbkw.cn

[T39] Lua：模式匹配
来源：http://pux.wangshuangyany.cn

string.find(s, "%d+")
来源：http://kdt.zhiwuduotai.top

[T40] Lua：元表
来源：http://wra.zhongyouzk.top

setmetatable({}, { __index = base })
来源：http://slm.chenjidiqi.icu

[T41] Perl：Hello World
来源：http://yjw.sjlbkw.cn

print "Hello\n";
来源：http://crr.hnxiangtu.top

[T42] Perl：变量类型
来源：http://vem.xinyue.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eme.nanxuanxn.top

[T43] Perl：字符串插值
来源：http://ikl.xinyue.icu

"值: $a"
来源：http://mqr.jlsjyb.cn

[T44] Perl：条件
来源：http://mee.shanyushiyangtech.top

if ($a > 0) { print "正"; }
来源：http://qpp.hysaishi.cn

[T45] Perl：数组遍历
来源：http://njs.shuidangran.top

for my $x (@arr) { print $x; }
来源：http://ldw.yfazqb.com

[T46] Perl：哈希操作
来源：http://ook.ctjpmb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bfd.andypj.xyz

[T47] Perl：正则捕获
来源：http://jbf.dashuyun.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tsm.ctjpmb.com

[T48] Perl：正则替换
来源：http://qpg.ehwqpu.com

$s =~ s/old/new/g;
来源：http://jte.tianlin.xyz

[T49] Perl：函数
来源：http://fdk.yanxiufei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://axu.ppjwa.cn

[T50] Perl：逐行读文件
来源：http://yqd.tarul.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xko.sufxvd.cn

while (my $line = <$fh>) { print $line; }
来源：http://ohi.zhixingplan.top

[T51] Scala：Hello World
来源：http://ivh.birdmap.top

println("Hello")
来源：http://hwy.guowangkeji.top

[T52] Scala：变量
来源：http://nqm.jinqigufen.top

val a = 1;  var b = 2
来源：http://ioy.fengsongda.top

[T53] Scala：字符串插值
来源：http://zvw.jlsjyb.cn

s"值: $b"
来源：http://lvt.nanxuanxn.top

[T54] Scala：集合映射
来源：http://luq.uphjek.com

List(1, 2, 3).map(_ * 2)
来源：http://hea.vqdsnc.cn

[T55] Scala：集合过滤
来源：http://xng.ywan-chungtsiang.top

List(1, 2, 3).filter(_ > 1)
来源：http://tyv.cashguo.top

[T56] Scala：样例类
来源：http://urq.yonumen.top

case class User(name: String, age: Int)
来源：http://fgi.zdqjudy.top

[T57] Scala：模式匹配
来源：http://fgc.gogol.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wlt.kuanghao11.cn

[T58] Scala：函数定义
来源：http://rbc.xuetiantiany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rnc.iojbl.cn

[T59] Scala：循环
来源：http://ozb.chenlongwang.top

for (i <- 1 to 10) println(i)
来源：http://maf.meibo888.top

[T60] Scala：折叠
来源：http://ghw.haohaochexian.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ebf.jinqigufen.top

================================================================================
来源：http://xok.andypj.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ywt.daxiang520.top

================================================================================
来源：http://cdo.dianchejie.cn

[U01] Py：创建虚拟环境
来源：http://aow.xuetiantiany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://iwd.xingfuxueyuan.xyz

[U02] Py：导出 / 安装依赖
来源：http://mbg.jyoumei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ubb.fengsongda.top

[U03] Py：加载 .env 配置
来源：http://iay.tarul.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nic.chenjidiqi.icu

[U04] Py：变量调试打印
来源：http://wsy.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jvn.gotoacloud.top

[U05] Py：列表去重且保序
来源：http://ett.epnwcf.com

list(dict.fromkeys(arr))
来源：http://rhe.zhaomingkeji.xyz

[U06] Py：合并两个字典
来源：http://ybo.cheryme.top

{**a, **b}
来源：http://inl.yfazqb.com

[U07] Py：反转字典键值
来源：http://nzk.ybcxt.top

{v: k for k, v in d.items()}
来源：http://zzp.52xcode.cn

[U08] Py：展平二维列表
来源：http://xvq.yangfankeji.com

[y for x in nested for y in x]
来源：http://cqt.zdqjudy.top

[U09] Py：字典取最大值的键
来源：http://tvg.ivvv.top

max(d, key=d.get)
来源：http://fqu.dianchejie.cn

[U10] Py：按值排序字典
来源：http://xxq.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gqq.yvedp.cn

[U11] Py：生成器表达式
来源：http://gkh.zhengqikj.top

(x * 2 for x in arr)
来源：http://axz.ctjpmb.com

[U12] Py：取出现最多的 3 个元素
来源：http://non.nanxinkj.top

Counter(arr).most_common(3)
来源：http://gyn.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://nnv.wangdashe.top

deque(maxlen=10)
来源：http://tyl.shuidangran.top

[U14] Py：分组收集到列表
来源：http://mvt.jqgfzy.top

defaultdict(list)
来源：http://zgi.ybcxt.top

[U15] Py：高精度计时
来源：http://ybl.shuidangran.top

t = time.perf_counter()
来源：http://odp.nanxuanxn.top

[U16] Py：命令行参数解析
来源：http://hvc.xziqi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qjv.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://alj.52xcode.cn

logging.basicConfig(level=logging.INFO)
来源：http://gfu.ydzc1.top

[U18] Py：预编译正则
来源：http://ijc.ctjpmb.com

pat = re.compile(r"\d+")
来源：http://gdr.nwbrower.top

[U19] Py：正则替换带回调
来源：http://ays.0kj1m.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zuk.wangshuangyany.cn

[U20] Py：缓存函数结果
来源：http://ybn.aibaodan.cn

@functools.lru_cache(maxsize=None)
来源：http://jtd.jinyuanbaomall.cn

[U21] Py：自定义上下文管理器
来源：http://wof.jlsjyb.cn

@contextlib.contextmanager
来源：http://twp.zycfv.cn

[U22] Py：矩阵转置
来源：http://jgy.ydjk.org.cn

list(zip(*m))
来源：http://vfm.shangyingyoupin.top

[U23] Py：分块读取大文件
来源：http://wbf.zhijiandao.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tys.jiagoushi.top

[U24] Py：路径操作
来源：http://imf.meibo888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uxd.hammf.cn

[U25] Py：CSV 按字典读
来源：http://cww.daria6918.cn

csv.DictReader(f)
来源：http://klh.tian-w.cn

[U26] Py：并发下载
来源：http://qak.yuanzhike.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://icg.havefunace.top

[U27] Py：异步 HTTP
来源：http://fxc.andypj.xyz

aiohttp.ClientSession() 配合 async with
来源：http://czb.redwolf501.top

[U28] Py：类型别名
来源：http://pmn.fengsongda.top

UserId = int
来源：http://xuy.zdbjq.cn

[U29] Py：属性校验
来源：http://nsk.chenjidiqi.icu

@property 与 @x.setter 配合
来源：http://lpj.yonumen.top

[U30] Py：数据类
来源：http://xlj.jlsjyb.cn

@dataclass(slots=True)
来源：http://dhx.jyoumei.cn

[U31] Py：单测
来源：http://yzr.bjfxy.top

python -m pytest -q
来源：http://twj.nanxuanxn.top

[U32] Py：代码格式化
来源：http://dld.shzxlz.cn

ruff format . && ruff check --fix .
来源：http://hbz.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://vei.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://btl.316326.xyz

[U34] Py：判断编码
来源：http://lpf.cdnleiting.top

chardet.detect(raw)
来源：http://jao.hfpthk.cn

[U35] Py：发送邮件
来源：http://jqw.hfpthk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ygq.sjlbkw.cn

[U36] Py：定时任务
来源：http://idf.fehbvm.com

schedule.every(10).minutes.do(job)
来源：http://wok.wangdashe.top

[U37] Py：读写 Excel
来源：http://fzr.svipenyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://akc.zhengqikj.top

[U38] Py：获取脚本所在目录
来源：http://qgs.jinyuanbaomall.cn

Path(__file__).resolve().parent
来源：http://pyv.tianlin.xyz

[U39] Py：判断是否在交互环境
来源：http://ygc.zhoulong.xyz

sys.stdout.isatty()
来源：http://vot.yangfankeji.com

[U40] Py：打印到标准错误
来源：http://nvx.cashguo.top

print("err", file=sys.stderr)
来源：http://boy.kuanghao11.cn

[U41] PHP：初始化 Composer 项目
来源：http://umb.ybcxt.top

composer init;  composer require guzzlehttp/guzzle
来源：http://efo.zhoulong.xyz

[U42] PHP：PSR-4 自动加载
来源：http://hes.yj20258888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tui.yj202588.top

[U43] PHP：声明命名空间
来源：http://ksr.quarkkingdee.top

namespace App\Http;
来源：http://zdt.daria6918.cn

[U44] PHP：开启严格类型
来源：http://exd.zhengqikj.top

declare(strict_types=1);
来源：http://hrc.havefunace.top

[U45] PHP：类型声明与返回类型
来源：http://ipx.xziqi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wye.chenzaomai.com

[U46] PHP：可空类型
来源：http://irm.dashuyun.cn

?string $name = null
来源：http://aux.sjlbkw.cn

[U47] PHP：联合类型
来源：http://vjc.cqqwz.cn

int|string $id
来源：http://xeu.ydjk.org.cn

[U48] PHP：纯枚举
来源：http://rhu.cdnleiting.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ycu.shanyushiyangkeji.top

[U49] PHP：只读属性
来源：http://wbz.vqdsnc.cn

public readonly string $name
来源：http://fdi.daria6918.cn

[U50] PHP：构造器属性提升
来源：http://dvn.yj20258888.top

public function __construct(private int $id) {}
来源：http://gwg.yj20258888.top

[U51] PHP：数组解构
来源：http://gra.jlsjyb.cn

[$a, $b] = $arr;
来源：http://rpz.zycfv.cn

[U52] PHP：箭头函数
来源：http://mpy.xuetiantiany.cn

$double = fn($x) => $x * 2;
来源：http://llz.yonumen.top

[U53] PHP：空合并运算符
来源：http://ymr.zhijiandao.cn

$v = $a ?? $b ?? "default";
来源：http://mfv.dianchejie.cn

[U54] PHP：空安全调用
来源：http://fgf.iojbl.cn

$obj?->method()
来源：http://sir.bjfxy.top

[U55] PHP：match 表达式
来源：http://jet.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tto.yuanzhike.top

[U56] PHP：命名参数
来源：http://doh.mhx1999.top

f(a: 1, b: 2)
来源：http://qvj.zhoulong.xyz

[U57] PHP：字符串插值
来源：http://vkr.havefunace.top

"值: {$a}"
来源：http://yby.zycfv.cn

[U58] PHP：数组三件套
来源：http://zrb.yangfankeji.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://waq.meibo888.top

[U59] PHP：自定义排序
来源：http://qwd.xuetiantiany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hkn.tianlin.xyz

[U60] PHP：JSON 编解码
来源：http://esi.c1oappe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qpv.sjlbkw.cn

[U61] PHP：正则
来源：http://myc.yj20258888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tef.gaohongyu789.top

[U62] PHP：日期对象
来源：http://izq.yonumen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jtk.yvedp.cn

[U63] PHP：文件读写
来源：http://qxg.cucudq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zbw.vqdsnc.cn

[U64] PHP：目录遍历
来源：http://hca.316326.xyz

glob("dir/*.php");  scandir("dir");
来源：http://pjr.smart0.xyz

[U65] PHP：会话
来源：http://gng.chenlongwang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hao.jlsjyb.cn

[U66] PHP：设置 Cookie
来源：http://fqq.aizwys.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xaw.iojbl.cn

[U67] PHP：处理文件上传
来源：http://dmw.bbcook.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oya.redwolf501.top

[U68] PHP：PDO 连接
来源：http://ldv.yonumen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nob.haohaochexian.top

[U69] PHP：PDO 预处理
来源：http://fnj.cashguo.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vij.hesvh.cn

[U70] PHP：PDO 事务
来源：http://jfb.sweek.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sna.yueranfly.top

[U71] PHP：抛出异常
来源：http://uqh.jinghuilouyu.cn

throw new RuntimeException("失败", 500);
来源：http://dii.haohaochexian.top

[U72] PHP：写错误日志
来源：http://ayj.hammf.cn

error_log("失败: " . $e->getMessage());
来源：http://pbr.wangshuangyany.cn

[U73] PHP：读取 ini 配置
来源：http://omq.zhongyouzk.top

parse_ini_file("config.ini", true)
来源：http://foi.shangyingyoupin.top

[U74] PHP：读取环境变量
来源：http://lll.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://xnz.yanxiufei.cn

[U75] PHP：依赖注入
来源：http://paf.zdqjudy.top

composer require psr/container
来源：http://orm.yongpay.top

[U76] PHP：简单路由
来源：http://buw.yj202588.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cqw.chenzaomai.com

[U77] PHP：模板渲染
来源：http://vds.jinghuilouyu.cn

composer require twig/twig
来源：http://och.chenjidiqi.icu

[U78] PHP：单元测试
来源：http://zxk.jyoumei.cn

composer require --dev phpunit/phpunit
来源：http://weg.zhongyouzk.top

[U79] PHP：静态分析
来源：http://juk.xuetiantiany.cn

composer require --dev phpstan/phpstan
来源：http://aoe.52xcode.cn

[U80] PHP：代码规范修复
来源：http://vss.birdmap.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://msc.guannengcc.top

[U81] JS：初始化项目
来源：http://qlg.fengsongda.top

npm init -y;  npm i express
来源：http://aoq.gzhubu.top

[U82] JS：package.json 脚本
来源：http://vkp.iojbl.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rfm.kuanghao11.cn

[U83] JS：ES Module 导入导出
来源：http://ayg.quarkkingdee.top

export const a = 1;  import { a } from "./m.js";
来源：http://xgj.hfpthk.cn

[U84] JS：CommonJS 写法
来源：http://kgn.gzhubu.top

module.exports = { a };  const { a } = require("./m");
来源：http://fuz.zycfv.cn

[U85] JS：可选链
来源：http://diw.hnqzz.top

a?.b?.c
来源：http://vov.zhixingplan.top

[U86] JS：空值合并
来源：http://lom.tian-w.cn

a ?? b
来源：http://zxo.yj202588.top

[U87] JS：解构默认值
来源：http://cqr.zhongyouzk.top

const { a = 1, b = 2 } = obj;
来源：http://svf.daria6918.cn

[U88] JS：对象展开合并
来源：http://ybx.uphjek.com

{ ...a, ...b }
来源：http://ohl.xziqi.cn

[U89] JS：数组去重
来源：http://oag.9152youxi.cn

[...new Set(arr)]
来源：http://sry.pengpengdd.cyou

[U90] JS：数字数组排序
来源：http://eno.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://fgs.chenzaomai.com

[U91] JS：对象键值遍历
来源：http://zhv.daxiang520.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vsc.shzxlz.cn

[U92] JS：深拷贝
来源：http://tna.yonumen.top

structuredClone(obj)
来源：http://efb.yanxiufei.cn

[U93] JS：模板字符串
来源：http://rpk.hnqzz.top

`共 ${n} 条`
来源：http://eoa.haohaochexian.top

[U94] JS：箭头函数
来源：http://iyi.ybcxt.top

const double = x => x * 2;
来源：http://rvk.9152youxi.cn

[U95] JS：Promise 包装
来源：http://vpl.cdnleiting.top

new Promise((resolve, reject) => {})
来源：http://gup.birdmap.top

[U96] JS：async/await 与异常
来源：http://jri.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bfq.yj20258.top

[U97] JS：并发请求
来源：http://yrz.shangyingyoupin.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bus.smart0.xyz

[U98] JS：fetch 带 JSON
来源：http://lje.hongshengwenyu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ous.yueranfly.top

[U99] JS：事件监听
来源：http://odm.sjlbkw.cn

el.addEventListener("click", e => {})
来源：http://nky.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://idb.shanyushiyangkeji.top

document.querySelector(".item")
来源：http://muq.pycfn.com

[U101] JS：classList 操作
来源：http://euo.zhijiandao.cn

el.classList.toggle("active")
来源：http://wyh.yuanzhike.top

[U102] JS：本地存储
来源：http://fmp.ydjk.org.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://twv.52xcode.cn

[U103] JS：定时器
来源：http://sya.sysykeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nvx.chenjidiqi.icu

[U104] JS：防抖
来源：http://uvz.hfpthk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rtz.uphjek.com

[U105] JS：节流
来源：http://cdx.zhoulong.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pxi.jqgfzy.top

[U106] JS：日期格式化
来源：http://fxl.hnqzz.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jfq.daria6918.cn

[U107] JS：数字千分位
来源：http://jya.sxryk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://won.mhx1999.top

[U108] JS：随机整数
来源：http://nxk.uphjek.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vbo.shanyushiyangtech.top

[U109] JS：数组分组
来源：http://upw.aibaodan.cn

Object.groupBy(arr, x => x.type)
来源：http://teo.daxiang520.top

[U110] JS：数组分块
来源：http://qrw.ppjwa.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://brh.iojbl.cn

[U111] JS：对象转 Map
来源：http://jeq.fzhhl.top

new Map(Object.entries(obj))
来源：http://dmw.epnwcf.com

[U112] JS：字符串补位
来源：http://nhh.sysykeji.top

"7".padStart(3, "0")
来源：http://ebe.shzxlz.cn

[U113] JS：正则替换全部
来源：http://sks.ydzc1.top

s.replaceAll("a", "b")
来源：http://puh.hfpthk.cn

[U114] JS：JSON 深比较
来源：http://qbb.ydjk.org.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sqw.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://jwf.guannengcc.top

crypto.randomUUID()
来源：http://vdq.shzxlz.cn

[U116] JS：类型检查（JSDoc）
来源：http://qvt.guowangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://vwk.xingfuxueyuan.xyz


<!-- 参考信息 -->