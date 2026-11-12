代发 wailian999

[T23] Swift：函数
来源：http://tbc.haohaochexian.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zan.yuanzhike.top

[T24] Swift：闭包
来源：http://apk.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dun.chenjidiqi.icu

[T25] Swift：结构体
来源：http://bvm.ctjpmb.com

struct P { var x: Int }
来源：http://mxz.yueranfly.top

[T26] Swift：类与重写
来源：http://usq.wangdashe.top

class A: Base { override func f() {} }
来源：http://nad.zhijiandao.cn

[T27] Swift：错误处理
来源：http://rgq.cheryme.top

do { try f() } catch { print(error) }
来源：http://ugo.mhx1999.top

[T28] Swift：枚举
来源：http://sot.tianlin.xyz

enum Color { case red, green }
来源：http://ylr.epnwcf.com

[T29] Swift：guard 提前返回
来源：http://uil.gotoacloud.top

guard let x = opt else { return }
来源：http://gfd.sweek.top

[T30] Swift：协议
来源：http://pkq.gotoacloud.top

protocol Shape { func area() -> Double }
来源：http://ewv.birdmap.top

[T31] Lua：Hello World
来源：http://otq.hammf.cn

print("Hello")
来源：http://rmi.yuanzhike.top

[T32] Lua：局部变量
来源：http://nqj.fzhhl.top

local a = 1
来源：http://onj.cheryme.top

[T33] Lua：表（数组）
来源：http://ods.sxryk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mhn.yj20258.top

[T34] Lua：遍历表
来源：http://zbh.sxryk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hml.shanyushiyangkeji.top

[T35] Lua：字典表
来源：http://fub.hcnkem.com

local d = { a = 1 };  d.b = 2
来源：http://zbp.hammf.cn

[T36] Lua：函数
来源：http://qqg.zhixingplan.top

function add(a, b) return a + b end
来源：http://iio.xylfe.cn

[T37] Lua：字符串拼接
来源：http://ksr.zdbjq.cn

"a" .. "b"
来源：http://jim.zhongyouzk.top

[T38] Lua：条件
来源：http://ikj.yongpay.top

if x > 0 then print("正") end
来源：http://pid.jinqigufen.top

[T39] Lua：模式匹配
来源：http://now.meibo888.top

string.find(s, "%d+")
来源：http://khp.aibaodan.cn

[T40] Lua：元表
来源：http://mmy.feifeiyinyue.top

setmetatable({}, { __index = base })
来源：http://ktl.shangyingyoupin.top

[T41] Perl：Hello World
来源：http://ioe.daxiang520.top

print "Hello\n";
来源：http://yrv.shuidangran.top

[T42] Perl：变量类型
来源：http://pkr.cdnleiting.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://crk.316326.xyz

[T43] Perl：字符串插值
来源：http://uty.tanke756.top

"值: $a"
来源：http://gxv.xingfuxueyuan.xyz

[T44] Perl：条件
来源：http://kfk.daria6918.cn

if ($a > 0) { print "正"; }
来源：http://xzv.shanyushiyangtech.top

[T45] Perl：数组遍历
来源：http://gfn.iojbl.cn

for my $x (@arr) { print $x; }
来源：http://ttv.0kj1m.cn

[T46] Perl：哈希操作
来源：http://kcq.kuanghao11.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bqw.sweek.top

[T47] Perl：正则捕获
来源：http://zgq.snrcjt.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mqe.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://bmy.ybcxt.top

$s =~ s/old/new/g;
来源：http://fei.fengsongda.top

[T49] Perl：函数
来源：http://mmz.zhijiandao.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iln.xuanzx.com

[T50] Perl：逐行读文件
来源：http://ynm.quarkkingdee.top

open my $fh, "<", "a.txt" or die $!;
来源：http://csz.guannengcc.top

while (my $line = <$fh>) { print $line; }
来源：http://gwm.havefunace.top

[T51] Scala：Hello World
来源：http://byd.cashguo.top

println("Hello")
来源：http://zlv.chenlongwang.top

[T52] Scala：变量
来源：http://edt.yongpay.top

val a = 1;  var b = 2
来源：http://rup.jlsjyb.cn

[T53] Scala：字符串插值
来源：http://xtu.jinqigfzy.top

s"值: $b"
来源：http://qpx.jiagoushi.top

[T54] Scala：集合映射
来源：http://gja.shzxlz.cn

List(1, 2, 3).map(_ * 2)
来源：http://kmd.jianghu66.top

[T55] Scala：集合过滤
来源：http://bus.pycfn.com

List(1, 2, 3).filter(_ > 1)
来源：http://byy.0kj1m.cn

[T56] Scala：样例类
来源：http://bsw.redwolf501.top

case class User(name: String, age: Int)
来源：http://dwe.52xcode.cn

[T57] Scala：模式匹配
来源：http://nfp.shzxlz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zpq.tanke756.top

[T58] Scala：函数定义
来源：http://zgo.guannengcc.top

def add(a: Int, b: Int): Int = a + b
来源：http://sfa.yangfankeji.com

[T59] Scala：循环
来源：http://rlu.jinqigufen.top

for (i <- 1 to 10) println(i)
来源：http://anb.zhoulong.xyz

[T60] Scala：折叠
来源：http://mqv.yangfankeji.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xcs.yuanzhike.top

================================================================================
来源：http://ehv.andypj.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cyv.daxiang520.top

================================================================================
来源：http://lxe.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://swq.hfpthk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qie.shanyushiyangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://wqw.ctjpmb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xzx.zhoulong.xyz

[U03] Py：加载 .env 配置
来源：http://kiw.hysaishi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sdt.sxryk.cn

[U04] Py：变量调试打印
来源：http://bux.ctjpmb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eay.hongshengwenyu.top

[U05] Py：列表去重且保序
来源：http://xrj.yj20258.top

list(dict.fromkeys(arr))
来源：http://gnf.aizwys.cn

[U06] Py：合并两个字典
来源：http://pqq.feifeiyinyue.top

{**a, **b}
来源：http://tjz.yangfankeji.com

[U07] Py：反转字典键值
来源：http://wjp.shzxlz.cn

{v: k for k, v in d.items()}
来源：http://kza.haohaochexian.top

[U08] Py：展平二维列表
来源：http://iel.fanxiaobao.xyz

[y for x in nested for y in x]
来源：http://uto.zhengqikj.top

[U09] Py：字典取最大值的键
来源：http://mft.fengsongda.top

max(d, key=d.get)
来源：http://kka.fanxiaobao.xyz

[U10] Py：按值排序字典
来源：http://kdd.nanxinkj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nev.aizwys.cn

[U11] Py：生成器表达式
来源：http://rfp.ivvv.top

(x * 2 for x in arr)
来源：http://tup.ydjk.org.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ypj.hnxiangtu.top

Counter(arr).most_common(3)
来源：http://dkw.chenjidiqi.icu

[U13] Py：固定长度队列
来源：http://uns.fzhhl.top

deque(maxlen=10)
来源：http://lpx.nanxuanxn.top

[U14] Py：分组收集到列表
来源：http://ysd.gogol.net.cn

defaultdict(list)
来源：http://qdp.zhijiandao.cn

[U15] Py：高精度计时
来源：http://rfe.hysaishi.cn

t = time.perf_counter()
来源：http://pbe.yonumen.top

[U16] Py：命令行参数解析
来源：http://ndc.yonumen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ngu.nanxuanxn.top

[U17] Py：初始化日志
来源：http://spw.hongshengwenyu.top

logging.basicConfig(level=logging.INFO)
来源：http://wye.haohaochexian.top

[U18] Py：预编译正则
来源：http://jcd.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://uyt.andypj.xyz

[U19] Py：正则替换带回调
来源：http://uio.hcnkem.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eqy.jyoumei.cn

[U20] Py：缓存函数结果
来源：http://qoj.pycfn.com

@functools.lru_cache(maxsize=None)
来源：http://vqh.guowangkeji.top

[U21] Py：自定义上下文管理器
来源：http://siq.tarul.cn

@contextlib.contextmanager
来源：http://gtm.bbcook.cn

[U22] Py：矩阵转置
来源：http://rnu.zhongyouzk.top

list(zip(*m))
来源：http://rfs.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://bdn.ywan-chungtsiang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dhy.c1oappe.top

[U24] Py：路径操作
来源：http://dha.yj20258888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fpg.chenlongwang.top

[U25] Py：CSV 按字典读
来源：http://bng.sweek.top

csv.DictReader(f)
来源：http://ukt.gaohongyu789.top

[U26] Py：并发下载
来源：http://ajz.sxryk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ysw.yueranfly.top

[U27] Py：异步 HTTP
来源：http://nuw.cashguo.top

aiohttp.ClientSession() 配合 async with
来源：http://fzr.yanxiufei.cn

[U28] Py：类型别名
来源：http://wsp.snrcjt.cn

UserId = int
来源：http://vlt.jinghuilouyu.cn

[U29] Py：属性校验
来源：http://egu.9152youxi.cn

@property 与 @x.setter 配合
来源：http://ksz.xuetiantiany.cn

[U30] Py：数据类
来源：http://rsi.cheryme.top

@dataclass(slots=True)
来源：http://gjl.sjlbkw.cn

[U31] Py：单测
来源：http://ctc.iojbl.cn

python -m pytest -q
来源：http://wcw.ppjwa.cn

[U32] Py：代码格式化
来源：http://jgv.yongpay.top

ruff format . && ruff check --fix .
来源：http://cxy.hcnkem.com

[U33] Py：打包发布
来源：http://mzm.snrcjt.cn

python -m build  （依赖 pyproject.toml）
来源：http://avk.fengsongda.top

[U34] Py：判断编码
来源：http://pmb.ydzc1.top

chardet.detect(raw)
来源：http://ljb.xylfe.cn

[U35] Py：发送邮件
来源：http://prm.mhx1999.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zxv.zdqjudy.top

[U36] Py：定时任务
来源：http://enz.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://rid.fengsongda.top

[U37] Py：读写 Excel
来源：http://hdq.pycfn.com

pandas.read_excel / DataFrame.to_excel
来源：http://wtq.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://agb.daxiang520.top

Path(__file__).resolve().parent
来源：http://rfr.sysykeji.top

[U39] Py：判断是否在交互环境
来源：http://npj.52xcode.cn

sys.stdout.isatty()
来源：http://agu.wangshuangyany.cn

[U40] Py：打印到标准错误
来源：http://gcc.meibo888.top

print("err", file=sys.stderr)
来源：http://sre.yj20258.top

[U41] PHP：初始化 Composer 项目
来源：http://bdy.shanyushiyangtech.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ctd.daria6918.cn

[U42] PHP：PSR-4 自动加载
来源：http://hvj.ydjk.org.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hgo.shuidangran.top

[U43] PHP：声明命名空间
来源：http://nvf.vehdjk.com

namespace App\Http;
来源：http://gvt.shangyingyoupin.top

[U44] PHP：开启严格类型
来源：http://ebq.havefunace.top

declare(strict_types=1);
来源：http://xah.mhx1999.top

[U45] PHP：类型声明与返回类型
来源：http://csh.snrcjt.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vwt.sweek.top

[U46] PHP：可空类型
来源：http://jxs.shanyushiyangkeji.top

?string $name = null
来源：http://ova.ydjk.org.cn

[U47] PHP：联合类型
来源：http://spo.kuanghao11.cn

int|string $id
来源：http://jar.chenzaomai.com

[U48] PHP：纯枚举
来源：http://rcz.hnqzz.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hrf.birdmap.top

[U49] PHP：只读属性
来源：http://stz.cheryme.top

public readonly string $name
来源：http://kdy.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://smv.fzhhl.top

public function __construct(private int $id) {}
来源：http://mvc.mhx1999.top

[U51] PHP：数组解构
来源：http://aok.aizwys.cn

[$a, $b] = $arr;
来源：http://lmw.yongpay.top

[U52] PHP：箭头函数
来源：http://emm.daxiang520.top

$double = fn($x) => $x * 2;
来源：http://bci.jianghu66.top

[U53] PHP：空合并运算符
来源：http://nge.yj202588.top

$v = $a ?? $b ?? "default";
来源：http://nga.hcnkem.com

[U54] PHP：空安全调用
来源：http://kwx.jinqigfzy.top

$obj?->method()
来源：http://gfu.mhx1999.top

[U55] PHP：match 表达式
来源：http://ufw.hysaishi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bcu.chenzaomai.com

[U56] PHP：命名参数
来源：http://rhu.ivvv.top

f(a: 1, b: 2)
来源：http://mie.iojbl.cn

[U57] PHP：字符串插值
来源：http://tls.shangyingyoupin.top

"值: {$a}"
来源：http://iiz.sufxvd.cn

[U58] PHP：数组三件套
来源：http://yvu.andypj.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vtp.sxryk.cn

[U59] PHP：自定义排序
来源：http://pdc.chenjidiqi.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nnu.chenjidiqi.icu

[U60] PHP：JSON 编解码
来源：http://jdc.smart0.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://azj.shanyushiyangkeji.top

[U61] PHP：正则
来源：http://nfe.cdnleiting.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jez.bbcook.cn

[U62] PHP：日期对象
来源：http://obo.xuanzx.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://msv.9152youxi.cn

[U63] PHP：文件读写
来源：http://wlq.pycfn.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aaw.xuanzx.com

[U64] PHP：目录遍历
来源：http://dhm.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://eso.yj20258.top

[U65] PHP：会话
来源：http://oia.zhoulong.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://xrh.zhixingplan.top

[U66] PHP：设置 Cookie
来源：http://qws.ppjwa.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gbp.svipenyu.cn

[U67] PHP：处理文件上传
来源：http://pyh.cdnleiting.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qqn.yuxming.cn

[U68] PHP：PDO 连接
来源：http://dsd.ppjwa.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rpo.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://wpg.yongpay.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zqc.yj202588.top

[U70] PHP：PDO 事务
来源：http://kgi.hfpthk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://grj.gotoacloud.top

[U71] PHP：抛出异常
来源：http://tco.cqqwz.cn

throw new RuntimeException("失败", 500);
来源：http://iig.hesvh.cn

[U72] PHP：写错误日志
来源：http://gam.gogol.net.cn

error_log("失败: " . $e->getMessage());
来源：http://vho.andypj.xyz

[U73] PHP：读取 ini 配置
来源：http://ssi.zycfv.cn

parse_ini_file("config.ini", true)
来源：http://rlv.pengpengdd.cyou

[U74] PHP：读取环境变量
来源：http://iwm.zdqjudy.top

getenv("APP_ENV") ?: "production"
来源：http://xoo.nanxinkj.top

[U75] PHP：依赖注入
来源：http://ovx.ydjk.org.cn

composer require psr/container
来源：http://rvh.quarkkingdee.top

[U76] PHP：简单路由
来源：http://ilz.gotoacloud.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hrj.52xcode.cn

[U77] PHP：模板渲染
来源：http://wmv.hywenlv.cn

composer require twig/twig
来源：http://qxb.ywan-chungtsiang.top

[U78] PHP：单元测试
来源：http://nok.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://cit.zhongyouzk.top

[U79] PHP：静态分析
来源：http://gfs.gaohongyu789.top

composer require --dev phpstan/phpstan
来源：http://ixh.yueranfly.top

[U80] PHP：代码规范修复
来源：http://noy.xziqi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xiw.nanxinkj.top

[U81] JS：初始化项目
来源：http://yaw.xziqi.cn

npm init -y;  npm i express
来源：http://ohv.ybcxt.top

[U82] JS：package.json 脚本
来源：http://rel.zhoulong.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zhw.zhixingplan.top

[U83] JS：ES Module 导入导出
来源：http://lcl.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://bwv.gzhubu.top

[U84] JS：CommonJS 写法
来源：http://xwa.shuidangran.top

module.exports = { a };  const { a } = require("./m");
来源：http://oev.xinyue.icu

[U85] JS：可选链
来源：http://lut.zhijiandao.cn

a?.b?.c
来源：http://zyp.zhoulong.xyz

[U86] JS：空值合并
来源：http://uxl.jinqigfzy.top

a ?? b
来源：http://jio.bbcook.cn

[U87] JS：解构默认值
来源：http://sjy.zhongyouzk.top

const { a = 1, b = 2 } = obj;
来源：http://nfo.yj20258.top

[U88] JS：对象展开合并
来源：http://dsa.shangyingyoupin.top

{ ...a, ...b }
来源：http://pgu.ehwqpu.com

[U89] JS：数组去重
来源：http://cyy.sysykeji.top

[...new Set(arr)]
来源：http://kgl.zhaomingkeji.xyz

[U90] JS：数字数组排序
来源：http://wat.yonumen.top

[...arr].sort((a, b) => a - b)
来源：http://yjs.fktsv.cn

[U91] JS：对象键值遍历
来源：http://vzi.ybcxt.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uyr.jinyuanbaomall.cn

[U92] JS：深拷贝
来源：http://egm.guowangkeji.top

structuredClone(obj)
来源：http://bvy.gogol.net.cn

[U93] JS：模板字符串
来源：http://egg.svipenyu.cn

`共 ${n} 条`
来源：http://hbx.chenlongwang.top

[U94] JS：箭头函数
来源：http://tgy.ydzc1.top

const double = x => x * 2;
来源：http://jvh.yangfankeji.com

[U95] JS：Promise 包装
来源：http://gbo.ppjwa.cn

new Promise((resolve, reject) => {})
来源：http://kbd.dianchejie.cn

[U96] JS：async/await 与异常
来源：http://zhg.xingfuxueyuan.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cgc.yfazqb.com

[U97] JS：并发请求
来源：http://tyj.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kjz.sxryk.cn

[U98] JS：fetch 带 JSON
来源：http://hva.zhengqikj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ntj.yj20258.top

[U99] JS：事件监听
来源：http://jso.meibo888.top

el.addEventListener("click", e => {})
来源：http://fbg.havefunace.top

[U100] JS：DOM 查询
来源：http://gth.hnqzz.top

document.querySelector(".item")
来源：http://qcc.ivvv.top

[U101] JS：classList 操作
来源：http://jvd.jqgufenzy.top

el.classList.toggle("active")
来源：http://fbo.wangdashe.top

[U102] JS：本地存储
来源：http://wvo.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://lbs.jinghuilouyu.cn

[U103] JS：定时器
来源：http://bfw.aizwys.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qzd.pycfn.com

[U104] JS：防抖
来源：http://jhy.jinghuilouyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sll.snrcjt.cn

[U105] JS：节流
来源：http://wto.fzhhl.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dea.fanxiaobao.xyz

[U106] JS：日期格式化
来源：http://jan.jqgufenzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cjb.yfazqb.com

[U107] JS：数字千分位
来源：http://hvb.gaohongyu789.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ylf.daxiang520.top

[U108] JS：随机整数
来源：http://ymf.jinqigfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vzy.wangshuangyany.cn

[U109] JS：数组分组
来源：http://jol.shuidangran.top

Object.groupBy(arr, x => x.type)
来源：http://jmp.chenzaomai.com

[U110] JS：数组分块
来源：http://mdr.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gqh.xziqi.cn


<!-- 参考信息 -->