代发 wailian999

[T25] Swift：结构体
来源：http://mqk.xuanzx.com

struct P { var x: Int }
来源：http://xpg.ydzc1.top

[T26] Swift：类与重写
来源：http://btf.yfazqb.com

class A: Base { override func f() {} }
来源：http://cyl.xylfe.cn

[T27] Swift：错误处理
来源：http://skr.jyoumei.cn

do { try f() } catch { print(error) }
来源：http://ncz.dashuyun.cn

[T28] Swift：枚举
来源：http://hlg.yj202588.top

enum Color { case red, green }
来源：http://fre.chenzaomai.com

[T29] Swift：guard 提前返回
来源：http://ufq.tarul.cn

guard let x = opt else { return }
来源：http://vjc.bjfxy.top

[T30] Swift：协议
来源：http://bpp.hnxiangtu.top

protocol Shape { func area() -> Double }
来源：http://rlu.ydzc1.top

[T31] Lua：Hello World
来源：http://tld.0kj1m.cn

print("Hello")
来源：http://mdv.vqdsnc.cn

[T32] Lua：局部变量
来源：http://tje.0kj1m.cn

local a = 1
来源：http://wdb.52xcode.cn

[T33] Lua：表（数组）
来源：http://daa.yuxming.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dti.quarkkingdee.top

[T34] Lua：遍历表
来源：http://qec.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ufe.0kj1m.cn

[T35] Lua：字典表
来源：http://ktv.yfazqb.com

local d = { a = 1 };  d.b = 2
来源：http://gcf.yfazqb.com

[T36] Lua：函数
来源：http://lht.ydjk.org.cn

function add(a, b) return a + b end
来源：http://akc.wangdashe.top

[T37] Lua：字符串拼接
来源：http://myt.yuanzhike.top

"a" .. "b"
来源：http://cni.sweek.top

[T38] Lua：条件
来源：http://tcp.zhijiandao.cn

if x > 0 then print("正") end
来源：http://fra.mhx1999.top

[T39] Lua：模式匹配
来源：http://eay.c1oappe.top

string.find(s, "%d+")
来源：http://xoj.ehwqpu.com

[T40] Lua：元表
来源：http://zqy.cashguo.top

setmetatable({}, { __index = base })
来源：http://her.ivvv.top

[T41] Perl：Hello World
来源：http://pqt.daxiang520.top

print "Hello\n";
来源：http://mix.bjfxy.top

[T42] Perl：变量类型
来源：http://lnz.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zns.iojbl.cn

[T43] Perl：字符串插值
来源：http://tqz.wangshuangyany.cn

"值: $a"
来源：http://yxs.yueranfly.top

[T44] Perl：条件
来源：http://duu.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://xyb.gotoacloud.top

[T45] Perl：数组遍历
来源：http://zxh.yonumen.top

for my $x (@arr) { print $x; }
来源：http://dmq.316326.xyz

[T46] Perl：哈希操作
来源：http://ncy.haohaochexian.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tvw.jinqigfzy.top

[T47] Perl：正则捕获
来源：http://odm.yanxiufei.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sou.snrcjt.cn

[T48] Perl：正则替换
来源：http://bxm.daxiang520.top

$s =~ s/old/new/g;
来源：http://fcn.tarul.cn

[T49] Perl：函数
来源：http://lyv.fehbvm.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ozv.dashuyun.cn

[T50] Perl：逐行读文件
来源：http://nzr.316326.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://spw.daxiang520.top

while (my $line = <$fh>) { print $line; }
来源：http://pdr.jiagoushi.top

[T51] Scala：Hello World
来源：http://pny.jinghuilouyu.cn

println("Hello")
来源：http://zor.nanxinkj.top

[T52] Scala：变量
来源：http://tdk.chenzaomai.com

val a = 1;  var b = 2
来源：http://cxw.dashuyun.cn

[T53] Scala：字符串插值
来源：http://wfb.sufxvd.cn

s"值: $b"
来源：http://yiq.ydzc1.top

[T54] Scala：集合映射
来源：http://qmu.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://mwm.yvedp.cn

[T55] Scala：集合过滤
来源：http://ngb.pengpengdd.cyou

List(1, 2, 3).filter(_ > 1)
来源：http://tkx.jiagoushi.top

[T56] Scala：样例类
来源：http://huk.fzhhl.top

case class User(name: String, age: Int)
来源：http://xev.ivvv.top

[T57] Scala：模式匹配
来源：http://amf.xingfuxueyuan.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://fob.snrcjt.cn

[T58] Scala：函数定义
来源：http://glg.jinqigfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://hcb.xuetiantiany.cn

[T59] Scala：循环
来源：http://wvj.mhx1999.top

for (i <- 1 to 10) println(i)
来源：http://yft.c1oappe.top

[T60] Scala：折叠
来源：http://uys.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ypn.sjlbkw.cn

================================================================================
来源：http://txp.havefunace.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zzl.jinqigufen.top

================================================================================
来源：http://tln.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://gaw.yj202588.top

python -m venv .venv && source .venv/bin/activate
来源：http://xrn.dashuyun.cn

[U02] Py：导出 / 安装依赖
来源：http://yab.jianghu66.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mzb.nanxuanxn.top

[U03] Py：加载 .env 配置
来源：http://okr.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kwv.jinqigfzy.top

[U04] Py：变量调试打印
来源：http://tpu.birdmap.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xrg.vehdjk.com

[U05] Py：列表去重且保序
来源：http://ggn.fengsongda.top

list(dict.fromkeys(arr))
来源：http://kcz.zhijiandao.cn

[U06] Py：合并两个字典
来源：http://gdi.sufxvd.cn

{**a, **b}
来源：http://roe.gzhubu.top

[U07] Py：反转字典键值
来源：http://wnd.yj202588.top

{v: k for k, v in d.items()}
来源：http://ima.fengsongda.top

[U08] Py：展平二维列表
来源：http://ylj.chenlongwang.top

[y for x in nested for y in x]
来源：http://qdk.hnqzz.top

[U09] Py：字典取最大值的键
来源：http://ofm.hcnkem.com

max(d, key=d.get)
来源：http://tgv.xuetiantiany.cn

[U10] Py：按值排序字典
来源：http://kno.nwbrower.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://plu.hnxiangtu.top

[U11] Py：生成器表达式
来源：http://lti.hysaishi.cn

(x * 2 for x in arr)
来源：http://zwr.tian-w.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tew.yuxming.cn

Counter(arr).most_common(3)
来源：http://bbr.daria6918.cn

[U13] Py：固定长度队列
来源：http://jpw.sysykeji.top

deque(maxlen=10)
来源：http://tsr.chenlongwang.top

[U14] Py：分组收集到列表
来源：http://qnj.kuanghao11.cn

defaultdict(list)
来源：http://ufe.ctjpmb.com

[U15] Py：高精度计时
来源：http://mnw.daria6918.cn

t = time.perf_counter()
来源：http://tbf.nwbrower.top

[U16] Py：命令行参数解析
来源：http://bhj.daxiang520.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uvp.uphjek.com

[U17] Py：初始化日志
来源：http://txk.zhixingplan.top

logging.basicConfig(level=logging.INFO)
来源：http://bjr.guannengcc.top

[U18] Py：预编译正则
来源：http://nry.daxiang520.top

pat = re.compile(r"\d+")
来源：http://kid.xziqi.cn

[U19] Py：正则替换带回调
来源：http://dui.hysaishi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ucc.zhaomingkeji.xyz

[U20] Py：缓存函数结果
来源：http://ozn.feifeiyinyue.top

@functools.lru_cache(maxsize=None)
来源：http://wkw.yuxming.cn

[U21] Py：自定义上下文管理器
来源：http://ajl.meibo888.top

@contextlib.contextmanager
来源：http://nou.c1oappe.top

[U22] Py：矩阵转置
来源：http://ngd.fanxiaobao.xyz

list(zip(*m))
来源：http://cmx.fehbvm.com

[U23] Py：分块读取大文件
来源：http://oni.hongshengwenyu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://flt.snrcjt.cn

[U24] Py：路径操作
来源：http://ubu.birdmap.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dok.fanxiaobao.xyz

[U25] Py：CSV 按字典读
来源：http://rea.zhengqikj.top

csv.DictReader(f)
来源：http://idb.haohaochexian.top

[U26] Py：并发下载
来源：http://hrx.daria6918.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ima.jinqigufen.top

[U27] Py：异步 HTTP
来源：http://xrt.dianchejie.cn

aiohttp.ClientSession() 配合 async with
来源：http://yzq.jqgfzy.top

[U28] Py：类型别名
来源：http://jfh.fengsongda.top

UserId = int
来源：http://opk.fehbvm.com

[U29] Py：属性校验
来源：http://mpn.sjlbkw.cn

@property 与 @x.setter 配合
来源：http://ygl.tarul.cn

[U30] Py：数据类
来源：http://ket.nanxuanxn.top

@dataclass(slots=True)
来源：http://ksc.haohaochexian.top

[U31] Py：单测
来源：http://dzb.yangfankeji.com

python -m pytest -q
来源：http://lwo.shangyingyoupin.top

[U32] Py：代码格式化
来源：http://dzy.shuidangran.top

ruff format . && ruff check --fix .
来源：http://les.zycfv.cn

[U33] Py：打包发布
来源：http://bub.sweek.top

python -m build  （依赖 pyproject.toml）
来源：http://tfh.vqdsnc.cn

[U34] Py：判断编码
来源：http://cjg.jyoumei.cn

chardet.detect(raw)
来源：http://lwj.hesvh.cn

[U35] Py：发送邮件
来源：http://uho.yangfankeji.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gro.mhx1999.top

[U36] Py：定时任务
来源：http://kmo.yanxiufei.cn

schedule.every(10).minutes.do(job)
来源：http://fse.uphjek.com

[U37] Py：读写 Excel
来源：http://bqq.gaohongyu789.top

pandas.read_excel / DataFrame.to_excel
来源：http://tpb.xinyue.icu

[U38] Py：获取脚本所在目录
来源：http://ekh.bjfxy.top

Path(__file__).resolve().parent
来源：http://syk.yuxming.cn

[U39] Py：判断是否在交互环境
来源：http://top.wangdashe.top

sys.stdout.isatty()
来源：http://aqi.tianlin.xyz

[U40] Py：打印到标准错误
来源：http://ztt.ivvv.top

print("err", file=sys.stderr)
来源：http://iwx.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://dve.fktsv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://azn.tianlin.xyz

[U42] PHP：PSR-4 自动加载
来源：http://ngl.jinqigfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rvs.quarkkingdee.top

[U43] PHP：声明命名空间
来源：http://bwe.gzhubu.top

namespace App\Http;
来源：http://ucz.sweek.top

[U44] PHP：开启严格类型
来源：http://ujp.chenjidiqi.icu

declare(strict_types=1);
来源：http://hku.jqgufenzy.top

[U45] PHP：类型声明与返回类型
来源：http://qcf.snrcjt.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rwx.bbcook.cn

[U46] PHP：可空类型
来源：http://oau.quarkkingdee.top

?string $name = null
来源：http://kfx.zdqjudy.top

[U47] PHP：联合类型
来源：http://fvq.hysaishi.cn

int|string $id
来源：http://bhc.gotoacloud.top

[U48] PHP：纯枚举
来源：http://mdf.ppjwa.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xzt.gotoacloud.top

[U49] PHP：只读属性
来源：http://jbd.ydjk.org.cn

public readonly string $name
来源：http://kfy.kuanghao11.cn

[U50] PHP：构造器属性提升
来源：http://ahv.ctjpmb.com

public function __construct(private int $id) {}
来源：http://apl.yueranfly.top

[U51] PHP：数组解构
来源：http://tic.jqgfzy.top

[$a, $b] = $arr;
来源：http://nhz.feifeiyinyue.top

[U52] PHP：箭头函数
来源：http://epk.yanxiufei.cn

$double = fn($x) => $x * 2;
来源：http://qre.yj20258.top

[U53] PHP：空合并运算符
来源：http://emn.chenjidiqi.icu

$v = $a ?? $b ?? "default";
来源：http://hqb.chenzaomai.com

[U54] PHP：空安全调用
来源：http://lnj.meibo888.top

$obj?->method()
来源：http://zjd.cheryme.top

[U55] PHP：match 表达式
来源：http://bla.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ydp.yj20258888.top

[U56] PHP：命名参数
来源：http://ggj.epnwcf.com

f(a: 1, b: 2)
来源：http://cuo.zhaomingkeji.xyz

[U57] PHP：字符串插值
来源：http://nmv.shanyushiyangtech.top

"值: {$a}"
来源：http://uqo.hysaishi.cn

[U58] PHP：数组三件套
来源：http://aky.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yst.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://sho.jinqigufen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lfx.ybcxt.top

[U60] PHP：JSON 编解码
来源：http://oug.daxiang520.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vzo.xziqi.cn

[U61] PHP：正则
来源：http://ihc.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://psj.guannengcc.top

[U62] PHP：日期对象
来源：http://wil.chenjidiqi.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nng.sweek.top

[U63] PHP：文件读写
来源：http://uvg.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eoz.tianlin.xyz

[U64] PHP：目录遍历
来源：http://rwm.shuidangran.top

glob("dir/*.php");  scandir("dir");
来源：http://wue.smart0.xyz

[U65] PHP：会话
来源：http://nja.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://iry.birdmap.top

[U66] PHP：设置 Cookie
来源：http://oaz.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lzi.sjlbkw.cn

[U67] PHP：处理文件上传
来源：http://tbg.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wtv.fzhhl.top

[U68] PHP：PDO 连接
来源：http://wxu.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jzu.haohaochexian.top

[U69] PHP：PDO 预处理
来源：http://bad.zdqjudy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vqj.hnqzz.top

[U70] PHP：PDO 事务
来源：http://awt.hywenlv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ili.ybcxt.top

[U71] PHP：抛出异常
来源：http://vfz.nanxuanxn.top

throw new RuntimeException("失败", 500);
来源：http://hjt.gzhubu.top

[U72] PHP：写错误日志
来源：http://ach.yvedp.cn

error_log("失败: " . $e->getMessage());
来源：http://fxf.sjlbkw.cn

[U73] PHP：读取 ini 配置
来源：http://cag.bbcook.cn

parse_ini_file("config.ini", true)
来源：http://ngh.jinyuanbaomall.cn

[U74] PHP：读取环境变量
来源：http://mvp.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://vma.shanyushiyangkeji.top

[U75] PHP：依赖注入
来源：http://unn.hcnkem.com

composer require psr/container
来源：http://vqw.xziqi.cn

[U76] PHP：简单路由
来源：http://tok.fktsv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gij.ctjpmb.com

[U77] PHP：模板渲染
来源：http://own.redwolf501.top

composer require twig/twig
来源：http://kiw.gogol.net.cn

[U78] PHP：单元测试
来源：http://vps.hnqzz.top

composer require --dev phpunit/phpunit
来源：http://han.hnxiangtu.top

[U79] PHP：静态分析
来源：http://zqk.zdqjudy.top

composer require --dev phpstan/phpstan
来源：http://npp.52xcode.cn

[U80] PHP：代码规范修复
来源：http://iwe.pengpengdd.cyou

composer require --dev friendsofphp/php-cs-fixer
来源：http://bue.vehdjk.com

[U81] JS：初始化项目
来源：http://myx.yj20258888.top

npm init -y;  npm i express
来源：http://idp.cqqwz.cn

[U82] JS：package.json 脚本
来源：http://ipg.hammf.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ydp.zhixingplan.top

[U83] JS：ES Module 导入导出
来源：http://mqm.316326.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://lyx.fzhhl.top

[U84] JS：CommonJS 写法
来源：http://kvk.hfpthk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rwe.daria6918.cn

[U85] JS：可选链
来源：http://wjj.xuetiantiany.cn

a?.b?.c
来源：http://dpg.gogol.net.cn

[U86] JS：空值合并
来源：http://jbz.cdnleiting.top

a ?? b
来源：http://var.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://rqb.epnwcf.com

const { a = 1, b = 2 } = obj;
来源：http://nsq.xylfe.cn

[U88] JS：对象展开合并
来源：http://wse.iojbl.cn

{ ...a, ...b }
来源：http://mxs.guannengcc.top

[U89] JS：数组去重
来源：http://kid.shuidangran.top

[...new Set(arr)]
来源：http://fmw.nanxuanxn.top

[U90] JS：数字数组排序
来源：http://dvu.yangfankeji.com

[...arr].sort((a, b) => a - b)
来源：http://kez.xylfe.cn

[U91] JS：对象键值遍历
来源：http://wvu.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://udq.fehbvm.com

[U92] JS：深拷贝
来源：http://pks.hysaishi.cn

structuredClone(obj)
来源：http://crg.cdnleiting.top

[U93] JS：模板字符串
来源：http://dkd.meibo888.top

`共 ${n} 条`
来源：http://kwg.xuanzx.com

[U94] JS：箭头函数
来源：http://esy.52xcode.cn

const double = x => x * 2;
来源：http://mna.jinyuanbaomall.cn

[U95] JS：Promise 包装
来源：http://mbk.haohaochexian.top

new Promise((resolve, reject) => {})
来源：http://vmy.fehbvm.com

[U96] JS：async/await 与异常
来源：http://qez.shuidangran.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zou.sufxvd.cn

[U97] JS：并发请求
来源：http://lxt.kuanghao11.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cgu.aizwys.cn

[U98] JS：fetch 带 JSON
来源：http://eos.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://edo.aizwys.cn

[U99] JS：事件监听
来源：http://rmt.ybcxt.top

el.addEventListener("click", e => {})
来源：http://dzz.zhaomingkeji.xyz

[U100] JS：DOM 查询
来源：http://zvd.jiagoushi.top

document.querySelector(".item")
来源：http://dcp.svipenyu.cn

[U101] JS：classList 操作
来源：http://oqp.xuanzx.com

el.classList.toggle("active")
来源：http://bvi.jinqigufen.top

[U102] JS：本地存储
来源：http://seo.xuetiantiany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hnl.cdnleiting.top

[U103] JS：定时器
来源：http://vvf.hammf.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ofj.yongpay.top

[U104] JS：防抖
来源：http://qpl.hysaishi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://euw.nwbrower.top

[U105] JS：节流
来源：http://amw.dashuyun.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gba.yuxming.cn

[U106] JS：日期格式化
来源：http://kwo.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mur.jqgufenzy.top

[U107] JS：数字千分位
来源：http://dav.hfpthk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tzi.yanxiufei.cn

[U108] JS：随机整数
来源：http://rqh.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hmk.tanke756.top

[U109] JS：数组分组
来源：http://mig.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://vxv.sxryk.cn

[U110] JS：数组分块
来源：http://nhh.0kj1m.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eug.0kj1m.cn

[U111] JS：对象转 Map
来源：http://jej.xylfe.cn

new Map(Object.entries(obj))
来源：http://kjj.sweek.top

[U112] JS：字符串补位
来源：http://yex.zhijiandao.cn

"7".padStart(3, "0")
来源：http://wud.jinqigfzy.top


<!-- 参考信息 -->