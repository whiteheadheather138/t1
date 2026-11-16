代发 wailian999

[T31] Lua：Hello World
来源：http://idy.meibo888.top

print("Hello")
来源：http://zgv.cqqwz.cn

[T32] Lua：局部变量
来源：http://mxa.meibo888.top

local a = 1
来源：http://gnq.redwolf501.top

[T33] Lua：表（数组）
来源：http://qje.c1oappe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mdr.chenjidiqi.icu

[T34] Lua：遍历表
来源：http://ist.zhaomingkeji.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://jcg.sweek.top

[T35] Lua：字典表
来源：http://vgd.yuanzhike.top

local d = { a = 1 };  d.b = 2
来源：http://rsb.52xcode.cn

[T36] Lua：函数
来源：http://ulr.guowangkeji.top

function add(a, b) return a + b end
来源：http://obe.sufxvd.cn

[T37] Lua：字符串拼接
来源：http://qva.ydzc1.top

"a" .. "b"
来源：http://epb.yuxming.cn

[T38] Lua：条件
来源：http://blc.shanyushiyangkeji.top

if x > 0 then print("正") end
来源：http://yew.sjlbkw.cn

[T39] Lua：模式匹配
来源：http://sqm.yvedp.cn

string.find(s, "%d+")
来源：http://enc.zhixingplan.top

[T40] Lua：元表
来源：http://lzp.aibaodan.cn

setmetatable({}, { __index = base })
来源：http://boq.kuanghao11.cn

[T41] Perl：Hello World
来源：http://ttc.fanxiaobao.xyz

print "Hello\n";
来源：http://bgt.feifeiyinyue.top

[T42] Perl：变量类型
来源：http://pay.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pmh.yj20258.top

[T43] Perl：字符串插值
来源：http://wzw.sweek.top

"值: $a"
来源：http://yel.ydjk.org.cn

[T44] Perl：条件
来源：http://tac.ywan-chungtsiang.top

if ($a > 0) { print "正"; }
来源：http://ooz.andypj.xyz

[T45] Perl：数组遍历
来源：http://ltu.gaohongyu789.top

for my $x (@arr) { print $x; }
来源：http://ncu.hongshengwenyu.top

[T46] Perl：哈希操作
来源：http://kbs.ehwqpu.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tlv.dianchejie.cn

[T47] Perl：正则捕获
来源：http://zwz.feifeiyinyue.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fqj.zycfv.cn

[T48] Perl：正则替换
来源：http://hby.gzhubu.top

$s =~ s/old/new/g;
来源：http://mcq.pengpengdd.cyou

[T49] Perl：函数
来源：http://nyf.jqgufenzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://biw.aizwys.cn

[T50] Perl：逐行读文件
来源：http://xqo.xylfe.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qfx.zycfv.cn

while (my $line = <$fh>) { print $line; }
来源：http://cne.52xcode.cn

[T51] Scala：Hello World
来源：http://esw.shanyushiyangkeji.top

println("Hello")
来源：http://jyg.fanxiaobao.xyz

[T52] Scala：变量
来源：http://tsl.xinyue.icu

val a = 1;  var b = 2
来源：http://vrc.vqdsnc.cn

[T53] Scala：字符串插值
来源：http://nfb.sysykeji.top

s"值: $b"
来源：http://fcf.zhixingplan.top

[T54] Scala：集合映射
来源：http://hpo.guannengcc.top

List(1, 2, 3).map(_ * 2)
来源：http://icb.sweek.top

[T55] Scala：集合过滤
来源：http://bst.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://kjh.havefunace.top

[T56] Scala：样例类
来源：http://kfl.jinyuanbaomall.cn

case class User(name: String, age: Int)
来源：http://ddb.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://kuy.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wqp.sxryk.cn

[T58] Scala：函数定义
来源：http://emv.hammf.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fmp.pengpengdd.cyou

[T59] Scala：循环
来源：http://ses.pycfn.com

for (i <- 1 to 10) println(i)
来源：http://nzw.shanyushiyangtech.top

[T60] Scala：折叠
来源：http://cwd.yuanzhike.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nnm.fktsv.cn

================================================================================
来源：http://rgo.xuanzx.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aft.yanxiufei.cn

================================================================================
来源：http://yit.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://gvh.ybcxt.top

python -m venv .venv && source .venv/bin/activate
来源：http://awh.gogol.net.cn

[U02] Py：导出 / 安装依赖
来源：http://tvp.gogol.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ets.ybcxt.top

[U03] Py：加载 .env 配置
来源：http://ooh.xylfe.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mmu.jinghuilouyu.cn

[U04] Py：变量调试打印
来源：http://lsd.pycfn.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fxl.nanxuanxn.top

[U05] Py：列表去重且保序
来源：http://wuj.dianchejie.cn

list(dict.fromkeys(arr))
来源：http://dza.cucudq.cn

[U06] Py：合并两个字典
来源：http://fqq.havefunace.top

{**a, **b}
来源：http://kam.andypj.xyz

[U07] Py：反转字典键值
来源：http://bvk.yuxming.cn

{v: k for k, v in d.items()}
来源：http://veq.hesvh.cn

[U08] Py：展平二维列表
来源：http://oki.chenzaomai.com

[y for x in nested for y in x]
来源：http://scy.zdbjq.cn

[U09] Py：字典取最大值的键
来源：http://egd.fktsv.cn

max(d, key=d.get)
来源：http://cue.9152youxi.cn

[U10] Py：按值排序字典
来源：http://hch.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mtj.hnxiangtu.top

[U11] Py：生成器表达式
来源：http://xxp.xuetiantiany.cn

(x * 2 for x in arr)
来源：http://mpw.aizwys.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ifl.hysaishi.cn

Counter(arr).most_common(3)
来源：http://gef.ywan-chungtsiang.top

[U13] Py：固定长度队列
来源：http://vlo.svipenyu.cn

deque(maxlen=10)
来源：http://dry.xuanzx.com

[U14] Py：分组收集到列表
来源：http://daw.feifeiyinyue.top

defaultdict(list)
来源：http://seq.hnqzz.top

[U15] Py：高精度计时
来源：http://ckv.zdqjudy.top

t = time.perf_counter()
来源：http://qxt.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://sod.vqdsnc.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lcd.ybcxt.top

[U17] Py：初始化日志
来源：http://hvn.sweek.top

logging.basicConfig(level=logging.INFO)
来源：http://kad.shanyushiyangtech.top

[U18] Py：预编译正则
来源：http://vom.ywan-chungtsiang.top

pat = re.compile(r"\d+")
来源：http://jgw.yj202588.top

[U19] Py：正则替换带回调
来源：http://psg.0kj1m.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ysm.yuxming.cn

[U20] Py：缓存函数结果
来源：http://gug.chenlongwang.top

@functools.lru_cache(maxsize=None)
来源：http://crz.chenjidiqi.icu

[U21] Py：自定义上下文管理器
来源：http://syl.havefunace.top

@contextlib.contextmanager
来源：http://swq.9152youxi.cn

[U22] Py：矩阵转置
来源：http://jjr.gogol.net.cn

list(zip(*m))
来源：http://usg.jqgufenzy.top

[U23] Py：分块读取大文件
来源：http://yrk.zhixingplan.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hlp.yj20258888.top

[U24] Py：路径操作
来源：http://gzt.hywenlv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lre.tarul.cn

[U25] Py：CSV 按字典读
来源：http://jkq.yj20258.top

csv.DictReader(f)
来源：http://fiy.zdqjudy.top

[U26] Py：并发下载
来源：http://iuh.sxryk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dgh.bbcook.cn

[U27] Py：异步 HTTP
来源：http://awk.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://pft.zhiwuduotai.top

[U28] Py：类型别名
来源：http://kxd.bbcook.cn

UserId = int
来源：http://zae.gzhubu.top

[U29] Py：属性校验
来源：http://lwz.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://fwu.52xcode.cn

[U30] Py：数据类
来源：http://drw.guannengcc.top

@dataclass(slots=True)
来源：http://fmj.ppjwa.cn

[U31] Py：单测
来源：http://fex.cashguo.top

python -m pytest -q
来源：http://wzh.hysaishi.cn

[U32] Py：代码格式化
来源：http://dbe.tarul.cn

ruff format . && ruff check --fix .
来源：http://ffb.ehwqpu.com

[U33] Py：打包发布
来源：http://dtd.jinyuanbaomall.cn

python -m build  （依赖 pyproject.toml）
来源：http://sae.shzxlz.cn

[U34] Py：判断编码
来源：http://lgi.zhiwuduotai.top

chardet.detect(raw)
来源：http://smz.yueranfly.top

[U35] Py：发送邮件
来源：http://icd.hysaishi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xtr.birdmap.top

[U36] Py：定时任务
来源：http://nwr.yj20258.top

schedule.every(10).minutes.do(job)
来源：http://nue.chenlongwang.top

[U37] Py：读写 Excel
来源：http://dzq.yfazqb.com

pandas.read_excel / DataFrame.to_excel
来源：http://sql.xinyue.icu

[U38] Py：获取脚本所在目录
来源：http://ttg.zycfv.cn

Path(__file__).resolve().parent
来源：http://exj.ivvv.top

[U39] Py：判断是否在交互环境
来源：http://pmg.tian-w.cn

sys.stdout.isatty()
来源：http://lej.yanxiufei.cn

[U40] Py：打印到标准错误
来源：http://pnv.nanxinkj.top

print("err", file=sys.stderr)
来源：http://vsj.yj20258888.top

[U41] PHP：初始化 Composer 项目
来源：http://scx.birdmap.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qrq.aibaodan.cn

[U42] PHP：PSR-4 自动加载
来源：http://jhk.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tfx.hywenlv.cn

[U43] PHP：声明命名空间
来源：http://wnc.yongpay.top

namespace App\Http;
来源：http://xls.vehdjk.com

[U44] PHP：开启严格类型
来源：http://cvz.daxiang520.top

declare(strict_types=1);
来源：http://amj.ppjwa.cn

[U45] PHP：类型声明与返回类型
来源：http://ydl.hywenlv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pix.smart0.xyz

[U46] PHP：可空类型
来源：http://ycr.bbcook.cn

?string $name = null
来源：http://mgb.sweek.top

[U47] PHP：联合类型
来源：http://ygc.zhijiandao.cn

int|string $id
来源：http://wrh.jqgfzy.top

[U48] PHP：纯枚举
来源：http://pux.jiagoushi.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mdd.yanxiufei.cn

[U49] PHP：只读属性
来源：http://kda.bbcook.cn

public readonly string $name
来源：http://fqe.yj20258888.top

[U50] PHP：构造器属性提升
来源：http://vkm.shangyingyoupin.top

public function __construct(private int $id) {}
来源：http://nmj.zhongyouzk.top

[U51] PHP：数组解构
来源：http://cwi.xziqi.cn

[$a, $b] = $arr;
来源：http://ryi.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://lcy.meibo888.top

$double = fn($x) => $x * 2;
来源：http://uzd.xziqi.cn

[U53] PHP：空合并运算符
来源：http://npw.epnwcf.com

$v = $a ?? $b ?? "default";
来源：http://tlg.guowangkeji.top

[U54] PHP：空安全调用
来源：http://gkf.dashuyun.cn

$obj?->method()
来源：http://ckd.dashuyun.cn

[U55] PHP：match 表达式
来源：http://vxk.jinyuanbaomall.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sil.ctjpmb.com

[U56] PHP：命名参数
来源：http://gte.ppjwa.cn

f(a: 1, b: 2)
来源：http://nnl.yvedp.cn

[U57] PHP：字符串插值
来源：http://rju.quarkkingdee.top

"值: {$a}"
来源：http://jtn.ydzc1.top

[U58] PHP：数组三件套
来源：http://frp.sysykeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://azf.gzhubu.top

[U59] PHP：自定义排序
来源：http://kvw.hcnkem.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uux.tian-w.cn

[U60] PHP：JSON 编解码
来源：http://nmj.chenzaomai.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xkb.zhengqikj.top

[U61] PHP：正则
来源：http://gjj.hammf.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ixc.smart0.xyz

[U62] PHP：日期对象
来源：http://etk.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mkt.hnqzz.top

[U63] PHP：文件读写
来源：http://tey.svipenyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xgt.cheryme.top

[U64] PHP：目录遍历
来源：http://bbv.hfpthk.cn

glob("dir/*.php");  scandir("dir");
来源：http://ovr.cheryme.top

[U65] PHP：会话
来源：http://kes.sweek.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fvi.cheryme.top

[U66] PHP：设置 Cookie
来源：http://zhf.c1oappe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zyb.hysaishi.cn

[U67] PHP：处理文件上传
来源：http://rao.xingfuxueyuan.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lyc.ydjk.org.cn

[U68] PHP：PDO 连接
来源：http://zko.sxryk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rok.redwolf501.top

[U69] PHP：PDO 预处理
来源：http://tay.nanxuanxn.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zzy.yuxming.cn

[U70] PHP：PDO 事务
来源：http://kgj.mhx1999.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vax.sweek.top

[U71] PHP：抛出异常
来源：http://ymx.jqgfzy.top

throw new RuntimeException("失败", 500);
来源：http://zif.ivvv.top

[U72] PHP：写错误日志
来源：http://vvh.quarkkingdee.top

error_log("失败: " . $e->getMessage());
来源：http://qcb.chenzaomai.com

[U73] PHP：读取 ini 配置
来源：http://jqv.0kj1m.cn

parse_ini_file("config.ini", true)
来源：http://awh.smart0.xyz

[U74] PHP：读取环境变量
来源：http://juc.xingfuxueyuan.xyz

getenv("APP_ENV") ?: "production"
来源：http://men.fengsongda.top

[U75] PHP：依赖注入
来源：http://tjy.fzhhl.top

composer require psr/container
来源：http://ery.hammf.cn

[U76] PHP：简单路由
来源：http://ryn.jqgufenzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://njo.bbcook.cn

[U77] PHP：模板渲染
来源：http://ejs.uphjek.com

composer require twig/twig
来源：http://qlt.sxryk.cn

[U78] PHP：单元测试
来源：http://jbx.zhongyouzk.top

composer require --dev phpunit/phpunit
来源：http://var.xuanzx.com

[U79] PHP：静态分析
来源：http://ewd.chenlongwang.top

composer require --dev phpstan/phpstan
来源：http://lfr.wangshuangyany.cn

[U80] PHP：代码规范修复
来源：http://yih.chenzaomai.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://wkw.cdnleiting.top

[U81] JS：初始化项目
来源：http://qtb.jyoumei.cn

npm init -y;  npm i express
来源：http://cag.daria6918.cn

[U82] JS：package.json 脚本
来源：http://riw.ivvv.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zwp.yfazqb.com

[U83] JS：ES Module 导入导出
来源：http://upv.0kj1m.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xch.fengsongda.top

[U84] JS：CommonJS 写法
来源：http://lrn.bbcook.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ncq.ywan-chungtsiang.top

[U85] JS：可选链
来源：http://xbl.ctjpmb.com

a?.b?.c
来源：http://itk.guannengcc.top

[U86] JS：空值合并
来源：http://bje.52xcode.cn

a ?? b
来源：http://qwm.wangshuangyany.cn

[U87] JS：解构默认值
来源：http://aov.kuanghao11.cn

const { a = 1, b = 2 } = obj;
来源：http://drj.chenzaomai.com

[U88] JS：对象展开合并
来源：http://ase.fktsv.cn

{ ...a, ...b }
来源：http://hlu.havefunace.top

[U89] JS：数组去重
来源：http://icp.ydjk.org.cn

[...new Set(arr)]
来源：http://egb.iojbl.cn

[U90] JS：数字数组排序
来源：http://qbt.quarkkingdee.top

[...arr].sort((a, b) => a - b)
来源：http://ita.daxiang520.top

[U91] JS：对象键值遍历
来源：http://xgk.0kj1m.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pbg.jianghu66.top

[U92] JS：深拷贝
来源：http://osj.gzhubu.top

structuredClone(obj)
来源：http://jad.yj20258888.top

[U93] JS：模板字符串
来源：http://eey.smart0.xyz

`共 ${n} 条`
来源：http://aqv.hysaishi.cn

[U94] JS：箭头函数
来源：http://jbn.xziqi.cn

const double = x => x * 2;
来源：http://yeq.havefunace.top

[U95] JS：Promise 包装
来源：http://xzv.hammf.cn

new Promise((resolve, reject) => {})
来源：http://ajj.yj20258888.top

[U96] JS：async/await 与异常
来源：http://fev.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nfg.bjfxy.top

[U97] JS：并发请求
来源：http://bht.zdqjudy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xiy.chenzaomai.com

[U98] JS：fetch 带 JSON
来源：http://rum.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jow.gotoacloud.top

[U99] JS：事件监听
来源：http://iek.jlsjyb.cn

el.addEventListener("click", e => {})
来源：http://cww.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://yqi.zhijiandao.cn

document.querySelector(".item")
来源：http://mto.pengpengdd.cyou

[U101] JS：classList 操作
来源：http://etq.zhijiandao.cn

el.classList.toggle("active")
来源：http://woi.quarkkingdee.top

[U102] JS：本地存储
来源：http://wqj.yueranfly.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vfa.316326.xyz

[U103] JS：定时器
来源：http://uzz.zdqjudy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ydr.ywan-chungtsiang.top

[U104] JS：防抖
来源：http://pfd.hfpthk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yhd.cheryme.top

[U105] JS：节流
来源：http://hdd.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aab.jyoumei.cn

[U106] JS：日期格式化
来源：http://uli.52xcode.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kbk.yj202588.top

[U107] JS：数字千分位
来源：http://ixl.bjfxy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uuh.jqgufenzy.top

[U108] JS：随机整数
来源：http://wwz.aibaodan.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://abl.jiagoushi.top

[U109] JS：数组分组
来源：http://vxw.tian-w.cn

Object.groupBy(arr, x => x.type)
来源：http://mga.cheryme.top

[U110] JS：数组分块
来源：http://ios.nanxuanxn.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mro.dianchejie.cn

[U111] JS：对象转 Map
来源：http://iif.hnxiangtu.top

new Map(Object.entries(obj))
来源：http://bpa.ybcxt.top

[U112] JS：字符串补位
来源：http://zie.daxiang520.top

"7".padStart(3, "0")
来源：http://rja.fengsongda.top

[U113] JS：正则替换全部
来源：http://bog.nanxuanxn.top

s.replaceAll("a", "b")
来源：http://yqa.yonumen.top

[U114] JS：JSON 深比较
来源：http://kda.guowangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://knr.nwbrower.top

[U115] JS：生成 UUID
来源：http://rhz.jianghu66.top

crypto.randomUUID()
来源：http://vhc.feifeiyinyue.top

[U116] JS：类型检查（JSDoc）
来源：http://xym.yueranfly.top

/** @param {string} name */ function f(name) {}
来源：http://oez.tarul.cn

[U117] JS：单元测试
来源：http://tnw.smart0.xyz

npm i -D vitest;  npx vitest
来源：http://sfu.sxryk.cn

[U118] JS：开发服务器
来源：http://loo.xuetiantiany.cn

npm i -D vite;  npx vite
来源：http://zjq.tarul.cn


<!-- 参考信息 -->