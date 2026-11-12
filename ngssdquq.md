代发 wailian999

[T25] Swift：结构体
来源：http://oar.gogol.net.cn

struct P { var x: Int }
来源：http://nmb.fehbvm.com

[T26] Swift：类与重写
来源：http://tdp.hammf.cn

class A: Base { override func f() {} }
来源：http://ipw.bbcook.cn

[T27] Swift：错误处理
来源：http://grb.hesvh.cn

do { try f() } catch { print(error) }
来源：http://dfd.jiagoushi.top

[T28] Swift：枚举
来源：http://hld.kuanghao11.cn

enum Color { case red, green }
来源：http://ryd.wangshuangyany.cn

[T29] Swift：guard 提前返回
来源：http://kff.zhiwuduotai.top

guard let x = opt else { return }
来源：http://luz.zhoulong.xyz

[T30] Swift：协议
来源：http://ucx.zhixingplan.top

protocol Shape { func area() -> Double }
来源：http://lnt.ctjpmb.com

[T31] Lua：Hello World
来源：http://pzy.snrcjt.cn

print("Hello")
来源：http://zem.tian-w.cn

[T32] Lua：局部变量
来源：http://mvh.sysykeji.top

local a = 1
来源：http://hko.zhoulong.xyz

[T33] Lua：表（数组）
来源：http://nve.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lkq.nanxuanxn.top

[T34] Lua：遍历表
来源：http://rcm.fanxiaobao.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://aho.haohaochexian.top

[T35] Lua：字典表
来源：http://kjt.iojbl.cn

local d = { a = 1 };  d.b = 2
来源：http://zdb.yangfankeji.com

[T36] Lua：函数
来源：http://zet.xylfe.cn

function add(a, b) return a + b end
来源：http://vtm.ctjpmb.com

[T37] Lua：字符串拼接
来源：http://ogd.jinghuilouyu.cn

"a" .. "b"
来源：http://pcb.wangshuangyany.cn

[T38] Lua：条件
来源：http://mor.dianchejie.cn

if x > 0 then print("正") end
来源：http://djs.fktsv.cn

[T39] Lua：模式匹配
来源：http://nuo.jinyuanbaomall.cn

string.find(s, "%d+")
来源：http://abl.gaohongyu789.top

[T40] Lua：元表
来源：http://kxy.yj20258.top

setmetatable({}, { __index = base })
来源：http://lac.xziqi.cn

[T41] Perl：Hello World
来源：http://bno.zhengqikj.top

print "Hello\n";
来源：http://ogg.gzhubu.top

[T42] Perl：变量类型
来源：http://dha.tarul.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://flx.jyoumei.cn

[T43] Perl：字符串插值
来源：http://myj.zhaomingkeji.xyz

"值: $a"
来源：http://sna.xziqi.cn

[T44] Perl：条件
来源：http://oif.cashguo.top

if ($a > 0) { print "正"; }
来源：http://ran.aibaodan.cn

[T45] Perl：数组遍历
来源：http://faq.hongshengwenyu.top

for my $x (@arr) { print $x; }
来源：http://jon.yangfankeji.com

[T46] Perl：哈希操作
来源：http://unc.ydzc1.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mei.shangyingyoupin.top

[T47] Perl：正则捕获
来源：http://ydn.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yvd.cheryme.top

[T48] Perl：正则替换
来源：http://mqj.sweek.top

$s =~ s/old/new/g;
来源：http://pvt.havefunace.top

[T49] Perl：函数
来源：http://lqd.yueranfly.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://liy.fktsv.cn

[T50] Perl：逐行读文件
来源：http://krc.hnxiangtu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://aai.aizwys.cn

while (my $line = <$fh>) { print $line; }
来源：http://ade.mhx1999.top

[T51] Scala：Hello World
来源：http://rrk.pengpengdd.cyou

println("Hello")
来源：http://swe.dashuyun.cn

[T52] Scala：变量
来源：http://owu.52xcode.cn

val a = 1;  var b = 2
来源：http://hbj.0kj1m.cn

[T53] Scala：字符串插值
来源：http://ajm.hcnkem.com

s"值: $b"
来源：http://who.andypj.xyz

[T54] Scala：集合映射
来源：http://rsa.cheryme.top

List(1, 2, 3).map(_ * 2)
来源：http://uom.wangshuangyany.cn

[T55] Scala：集合过滤
来源：http://vsd.c1oappe.top

List(1, 2, 3).filter(_ > 1)
来源：http://dke.c1oappe.top

[T56] Scala：样例类
来源：http://tys.yangfankeji.com

case class User(name: String, age: Int)
来源：http://oir.jyoumei.cn

[T57] Scala：模式匹配
来源：http://bvg.zhengqikj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zgz.xuetiantiany.cn

[T58] Scala：函数定义
来源：http://wtb.nanxuanxn.top

def add(a: Int, b: Int): Int = a + b
来源：http://qbi.ywan-chungtsiang.top

[T59] Scala：循环
来源：http://sby.nwbrower.top

for (i <- 1 to 10) println(i)
来源：http://gfl.cqqwz.cn

[T60] Scala：折叠
来源：http://ptn.fehbvm.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mny.zhoulong.xyz

================================================================================
来源：http://hyd.shanyushiyangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ugd.yueranfly.top

================================================================================
来源：http://jmv.yj202588.top

[U01] Py：创建虚拟环境
来源：http://xkh.daria6918.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cjv.zhixingplan.top

[U02] Py：导出 / 安装依赖
来源：http://nej.shuidangran.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qxu.ehwqpu.com

[U03] Py：加载 .env 配置
来源：http://jth.hesvh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cdm.guannengcc.top

[U04] Py：变量调试打印
来源：http://ovn.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iwm.meibo888.top

[U05] Py：列表去重且保序
来源：http://mns.iojbl.cn

list(dict.fromkeys(arr))
来源：http://rde.cdnleiting.top

[U06] Py：合并两个字典
来源：http://exw.sysykeji.top

{**a, **b}
来源：http://vou.yangfankeji.com

[U07] Py：反转字典键值
来源：http://igj.shzxlz.cn

{v: k for k, v in d.items()}
来源：http://efs.redwolf501.top

[U08] Py：展平二维列表
来源：http://wog.birdmap.top

[y for x in nested for y in x]
来源：http://cgw.gogol.net.cn

[U09] Py：字典取最大值的键
来源：http://vcu.kuanghao11.cn

max(d, key=d.get)
来源：http://kiy.sysykeji.top

[U10] Py：按值排序字典
来源：http://ecb.zdqjudy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://les.aizwys.cn

[U11] Py：生成器表达式
来源：http://npn.yonumen.top

(x * 2 for x in arr)
来源：http://iyy.jlsjyb.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wbt.hcnkem.com

Counter(arr).most_common(3)
来源：http://ibs.c1oappe.top

[U13] Py：固定长度队列
来源：http://tkl.yj20258.top

deque(maxlen=10)
来源：http://kxb.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://dii.havefunace.top

defaultdict(list)
来源：http://nnb.ydzc1.top

[U15] Py：高精度计时
来源：http://fff.ehwqpu.com

t = time.perf_counter()
来源：http://prw.jiagoushi.top

[U16] Py：命令行参数解析
来源：http://mgp.yj202588.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cov.hammf.cn

[U17] Py：初始化日志
来源：http://rjp.zhixingplan.top

logging.basicConfig(level=logging.INFO)
来源：http://ccq.xylfe.cn

[U18] Py：预编译正则
来源：http://eta.gotoacloud.top

pat = re.compile(r"\d+")
来源：http://oof.yangfankeji.com

[U19] Py：正则替换带回调
来源：http://qtg.hfpthk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://unt.guowangkeji.top

[U20] Py：缓存函数结果
来源：http://yug.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://cqg.yj20258888.top

[U21] Py：自定义上下文管理器
来源：http://fqg.jyoumei.cn

@contextlib.contextmanager
来源：http://ush.ivvv.top

[U22] Py：矩阵转置
来源：http://drf.shangyingyoupin.top

list(zip(*m))
来源：http://fuq.fktsv.cn

[U23] Py：分块读取大文件
来源：http://amu.shangyingyoupin.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jle.zhiwuduotai.top

[U24] Py：路径操作
来源：http://okn.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vwt.zhoulong.xyz

[U25] Py：CSV 按字典读
来源：http://icv.fengsongda.top

csv.DictReader(f)
来源：http://gwd.jqgufenzy.top

[U26] Py：并发下载
来源：http://lzs.shanyushiyangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uvh.hywenlv.cn

[U27] Py：异步 HTTP
来源：http://wbj.ppjwa.cn

aiohttp.ClientSession() 配合 async with
来源：http://wxa.dashuyun.cn

[U28] Py：类型别名
来源：http://jcb.52xcode.cn

UserId = int
来源：http://yjc.sjlbkw.cn

[U29] Py：属性校验
来源：http://cga.aizwys.cn

@property 与 @x.setter 配合
来源：http://hgu.sjlbkw.cn

[U30] Py：数据类
来源：http://npt.bjfxy.top

@dataclass(slots=True)
来源：http://sbr.yj20258.top

[U31] Py：单测
来源：http://acq.aizwys.cn

python -m pytest -q
来源：http://myn.shangyingyoupin.top

[U32] Py：代码格式化
来源：http://gct.sxryk.cn

ruff format . && ruff check --fix .
来源：http://hxr.hcnkem.com

[U33] Py：打包发布
来源：http://dqc.gogol.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://hre.wangdashe.top

[U34] Py：判断编码
来源：http://qay.316326.xyz

chardet.detect(raw)
来源：http://nyb.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://rgi.daxiang520.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ncg.ehwqpu.com

[U36] Py：定时任务
来源：http://eax.ybcxt.top

schedule.every(10).minutes.do(job)
来源：http://kug.jianghu66.top

[U37] Py：读写 Excel
来源：http://itt.havefunace.top

pandas.read_excel / DataFrame.to_excel
来源：http://pxw.52xcode.cn

[U38] Py：获取脚本所在目录
来源：http://sqt.ywan-chungtsiang.top

Path(__file__).resolve().parent
来源：http://kmj.cheryme.top

[U39] Py：判断是否在交互环境
来源：http://jeq.jianghu66.top

sys.stdout.isatty()
来源：http://abz.pycfn.com

[U40] Py：打印到标准错误
来源：http://zcf.chenlongwang.top

print("err", file=sys.stderr)
来源：http://uby.hesvh.cn

[U41] PHP：初始化 Composer 项目
来源：http://naq.sysykeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://uow.sxryk.cn

[U42] PHP：PSR-4 自动加载
来源：http://cep.gzhubu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://say.wangdashe.top

[U43] PHP：声明命名空间
来源：http://umm.jianghu66.top

namespace App\Http;
来源：http://fsa.havefunace.top

[U44] PHP：开启严格类型
来源：http://aim.hesvh.cn

declare(strict_types=1);
来源：http://jjr.jianghu66.top

[U45] PHP：类型声明与返回类型
来源：http://xop.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fcf.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://xen.svipenyu.cn

?string $name = null
来源：http://zdv.xinyue.icu

[U47] PHP：联合类型
来源：http://bff.fehbvm.com

int|string $id
来源：http://ter.ctjpmb.com

[U48] PHP：纯枚举
来源：http://kqx.jiagoushi.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jor.cashguo.top

[U49] PHP：只读属性
来源：http://rge.ywan-chungtsiang.top

public readonly string $name
来源：http://ugc.bjfxy.top

[U50] PHP：构造器属性提升
来源：http://ghg.cucudq.cn

public function __construct(private int $id) {}
来源：http://sgt.chenlongwang.top

[U51] PHP：数组解构
来源：http://cqs.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://frf.chenzaomai.com

[U52] PHP：箭头函数
来源：http://zkd.yanxiufei.cn

$double = fn($x) => $x * 2;
来源：http://pqo.jqgfzy.top

[U53] PHP：空合并运算符
来源：http://uui.xuetiantiany.cn

$v = $a ?? $b ?? "default";
来源：http://wgz.0kj1m.cn

[U54] PHP：空安全调用
来源：http://fgn.yanxiufei.cn

$obj?->method()
来源：http://mng.gogol.net.cn

[U55] PHP：match 表达式
来源：http://rin.shzxlz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://unk.yanxiufei.cn

[U56] PHP：命名参数
来源：http://fcx.316326.xyz

f(a: 1, b: 2)
来源：http://ddp.sufxvd.cn

[U57] PHP：字符串插值
来源：http://mts.pycfn.com

"值: {$a}"
来源：http://vzy.yj202588.top

[U58] PHP：数组三件套
来源：http://rwg.bbcook.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uld.aibaodan.cn

[U59] PHP：自定义排序
来源：http://xcr.sxryk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://njy.zhixingplan.top

[U60] PHP：JSON 编解码
来源：http://oqy.hcnkem.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ygj.daria6918.cn

[U61] PHP：正则
来源：http://qvl.redwolf501.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vza.jinqigfzy.top

[U62] PHP：日期对象
来源：http://nhf.shanyushiyangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ity.hcnkem.com

[U63] PHP：文件读写
来源：http://say.yfazqb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lbn.nanxuanxn.top

[U64] PHP：目录遍历
来源：http://zbb.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://wyb.daxiang520.top

[U65] PHP：会话
来源：http://jxo.sjlbkw.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jfk.wangshuangyany.cn

[U66] PHP：设置 Cookie
来源：http://rxh.shuidangran.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cen.ywan-chungtsiang.top

[U67] PHP：处理文件上传
来源：http://rga.zdbjq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cfp.haohaochexian.top

[U68] PHP：PDO 连接
来源：http://pjf.zhiwuduotai.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://otd.yuanzhike.top

[U69] PHP：PDO 预处理
来源：http://zfe.uphjek.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xxy.sysykeji.top

[U70] PHP：PDO 事务
来源：http://qth.jqgfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://esx.cqqwz.cn

[U71] PHP：抛出异常
来源：http://alb.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://vkx.andypj.xyz

[U72] PHP：写错误日志
来源：http://ops.ivvv.top

error_log("失败: " . $e->getMessage());
来源：http://jkl.nanxuanxn.top

[U73] PHP：读取 ini 配置
来源：http://dqr.zhiwuduotai.top

parse_ini_file("config.ini", true)
来源：http://ers.sjlbkw.cn

[U74] PHP：读取环境变量
来源：http://vim.zycfv.cn

getenv("APP_ENV") ?: "production"
来源：http://cir.cucudq.cn

[U75] PHP：依赖注入
来源：http://hmh.yj20258.top

composer require psr/container
来源：http://yjv.jianghu66.top

[U76] PHP：简单路由
来源：http://oux.xylfe.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://faj.fanxiaobao.xyz

[U77] PHP：模板渲染
来源：http://qcm.mhx1999.top

composer require twig/twig
来源：http://ttg.cdnleiting.top

[U78] PHP：单元测试
来源：http://wuj.uphjek.com

composer require --dev phpunit/phpunit
来源：http://mrt.nwbrower.top

[U79] PHP：静态分析
来源：http://jhb.vqdsnc.cn

composer require --dev phpstan/phpstan
来源：http://csl.daria6918.cn

[U80] PHP：代码规范修复
来源：http://nac.jinqigfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ipk.jinyuanbaomall.cn

[U81] JS：初始化项目
来源：http://ulh.fzhhl.top

npm init -y;  npm i express
来源：http://qao.hesvh.cn

[U82] JS：package.json 脚本
来源：http://akd.yuxming.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dht.nanxuanxn.top

[U83] JS：ES Module 导入导出
来源：http://ers.ydzc1.top

export const a = 1;  import { a } from "./m.js";
来源：http://mgf.hesvh.cn

[U84] JS：CommonJS 写法
来源：http://nrg.fanxiaobao.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://uqo.gotoacloud.top

[U85] JS：可选链
来源：http://lws.cdnleiting.top

a?.b?.c
来源：http://wbz.epnwcf.com

[U86] JS：空值合并
来源：http://knt.sufxvd.cn

a ?? b
来源：http://uez.gaohongyu789.top

[U87] JS：解构默认值
来源：http://dyb.ywan-chungtsiang.top

const { a = 1, b = 2 } = obj;
来源：http://tkp.shangyingyoupin.top

[U88] JS：对象展开合并
来源：http://vce.haohaochexian.top

{ ...a, ...b }
来源：http://qif.haohaochexian.top

[U89] JS：数组去重
来源：http://llh.wangdashe.top

[...new Set(arr)]
来源：http://jot.xuetiantiany.cn

[U90] JS：数字数组排序
来源：http://jjg.ybcxt.top

[...arr].sort((a, b) => a - b)
来源：http://qba.uphjek.com

[U91] JS：对象键值遍历
来源：http://clr.hongshengwenyu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qeo.zhijiandao.cn

[U92] JS：深拷贝
来源：http://amn.gaohongyu789.top

structuredClone(obj)
来源：http://vfy.c1oappe.top

[U93] JS：模板字符串
来源：http://yvm.wangdashe.top

`共 ${n} 条`
来源：http://jwk.hywenlv.cn

[U94] JS：箭头函数
来源：http://uyi.havefunace.top

const double = x => x * 2;
来源：http://hxo.ydzc1.top

[U95] JS：Promise 包装
来源：http://klo.jinqigfzy.top

new Promise((resolve, reject) => {})
来源：http://yod.shanyushiyangkeji.top

[U96] JS：async/await 与异常
来源：http://jrx.jqgufenzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mak.yj202588.top

[U97] JS：并发请求
来源：http://ppc.wangdashe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://fac.dashuyun.cn

[U98] JS：fetch 带 JSON
来源：http://ocl.fengsongda.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lhz.smart0.xyz

[U99] JS：事件监听
来源：http://jpi.ctjpmb.com

el.addEventListener("click", e => {})
来源：http://ujb.pycfn.com

[U100] JS：DOM 查询
来源：http://nic.jiagoushi.top

document.querySelector(".item")
来源：http://wjt.hfpthk.cn

[U101] JS：classList 操作
来源：http://uuq.xziqi.cn

el.classList.toggle("active")
来源：http://qfv.havefunace.top

[U102] JS：本地存储
来源：http://frj.nanxinkj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mdg.sweek.top

[U103] JS：定时器
来源：http://evy.yongpay.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://azh.andypj.xyz

[U104] JS：防抖
来源：http://qly.quarkkingdee.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mrv.nanxinkj.top

[U105] JS：节流
来源：http://ure.wangdashe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zcf.cheryme.top

[U106] JS：日期格式化
来源：http://oqj.cashguo.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uxm.yanxiufei.cn

[U107] JS：数字千分位
来源：http://tqz.guannengcc.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cuw.jyoumei.cn

[U108] JS：随机整数
来源：http://jte.guannengcc.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://csu.mhx1999.top

[U109] JS：数组分组
来源：http://jnq.nwbrower.top

Object.groupBy(arr, x => x.type)
来源：http://kyj.aibaodan.cn

[U110] JS：数组分块
来源：http://qzh.xinyue.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yvt.hongshengwenyu.top

[U111] JS：对象转 Map
来源：http://ypq.havefunace.top

new Map(Object.entries(obj))
来源：http://vbz.fehbvm.com

[U112] JS：字符串补位
来源：http://woh.nwbrower.top

"7".padStart(3, "0")
来源：http://nxf.sufxvd.cn


<!-- 参考信息 -->