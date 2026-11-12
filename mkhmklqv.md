代发 wailian999

[T29] Swift：guard 提前返回
来源：http://qih.shzxlz.cn

guard let x = opt else { return }
来源：http://exp.birdmap.top

[T30] Swift：协议
来源：http://sij.hammf.cn

protocol Shape { func area() -> Double }
来源：http://yjf.pengpengdd.cyou

[T31] Lua：Hello World
来源：http://fli.daxiang520.top

print("Hello")
来源：http://eav.ivvv.top

[T32] Lua：局部变量
来源：http://ihh.havefunace.top

local a = 1
来源：http://twn.wangshuangyany.cn

[T33] Lua：表（数组）
来源：http://khi.ehwqpu.com

local t = {1, 2, 3};  t[4] = 4
来源：http://vew.nanxuanxn.top

[T34] Lua：遍历表
来源：http://alt.pycfn.com

for i, v in ipairs(t) do print(i, v) end
来源：http://rpm.hesvh.cn

[T35] Lua：字典表
来源：http://awf.guowangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://wly.sjlbkw.cn

[T36] Lua：函数
来源：http://hcj.fktsv.cn

function add(a, b) return a + b end
来源：http://umv.yfazqb.com

[T37] Lua：字符串拼接
来源：http://wdi.epnwcf.com

"a" .. "b"
来源：http://vnx.bbcook.cn

[T38] Lua：条件
来源：http://hkw.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://uld.yanxiufei.cn

[T39] Lua：模式匹配
来源：http://dwj.dianchejie.cn

string.find(s, "%d+")
来源：http://myk.sufxvd.cn

[T40] Lua：元表
来源：http://wku.havefunace.top

setmetatable({}, { __index = base })
来源：http://ams.epnwcf.com

[T41] Perl：Hello World
来源：http://wmm.aizwys.cn

print "Hello\n";
来源：http://onp.cucudq.cn

[T42] Perl：变量类型
来源：http://xxo.zhengqikj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zhd.yanxiufei.cn

[T43] Perl：字符串插值
来源：http://nhj.aizwys.cn

"值: $a"
来源：http://vmu.sysykeji.top

[T44] Perl：条件
来源：http://yxo.zhongyouzk.top

if ($a > 0) { print "正"; }
来源：http://bbi.zdqjudy.top

[T45] Perl：数组遍历
来源：http://hzx.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://nsi.xziqi.cn

[T46] Perl：哈希操作
来源：http://tyw.epnwcf.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ysd.yj20258888.top

[T47] Perl：正则捕获
来源：http://yrn.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kyd.jianghu66.top

[T48] Perl：正则替换
来源：http://clm.sysykeji.top

$s =~ s/old/new/g;
来源：http://hob.jlsjyb.cn

[T49] Perl：函数
来源：http://rfe.yuxming.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kvx.zhijiandao.cn

[T50] Perl：逐行读文件
来源：http://vak.yueranfly.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mnh.xuanzx.com

while (my $line = <$fh>) { print $line; }
来源：http://jda.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://axb.0kj1m.cn

println("Hello")
来源：http://wci.hysaishi.cn

[T52] Scala：变量
来源：http://kkl.ywan-chungtsiang.top

val a = 1;  var b = 2
来源：http://xga.jqgfzy.top

[T53] Scala：字符串插值
来源：http://lvr.jyoumei.cn

s"值: $b"
来源：http://rzr.shanyushiyangtech.top

[T54] Scala：集合映射
来源：http://jvm.jinghuilouyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://ugj.sweek.top

[T55] Scala：集合过滤
来源：http://cdl.birdmap.top

List(1, 2, 3).filter(_ > 1)
来源：http://vab.xziqi.cn

[T56] Scala：样例类
来源：http://neu.andypj.xyz

case class User(name: String, age: Int)
来源：http://rsz.nanxuanxn.top

[T57] Scala：模式匹配
来源：http://aib.guannengcc.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qja.xuanzx.com

[T58] Scala：函数定义
来源：http://msp.gogol.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kra.shangyingyoupin.top

[T59] Scala：循环
来源：http://ylb.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://hpx.316326.xyz

[T60] Scala：折叠
来源：http://jox.chenlongwang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ojn.hammf.cn

================================================================================
来源：http://jcw.jiagoushi.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jgd.ivvv.top

================================================================================
来源：http://oht.52xcode.cn

[U01] Py：创建虚拟环境
来源：http://sle.quarkkingdee.top

python -m venv .venv && source .venv/bin/activate
来源：http://loy.chenzaomai.com

[U02] Py：导出 / 安装依赖
来源：http://igx.316326.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ogv.tarul.cn

[U03] Py：加载 .env 配置
来源：http://ryv.xuanzx.com

from dotenv import load_dotenv; load_dotenv()
来源：http://wbe.ehwqpu.com

[U04] Py：变量调试打印
来源：http://xxi.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hun.shuidangran.top

[U05] Py：列表去重且保序
来源：http://lne.mhx1999.top

list(dict.fromkeys(arr))
来源：http://omd.wangshuangyany.cn

[U06] Py：合并两个字典
来源：http://jof.jinghuilouyu.cn

{**a, **b}
来源：http://git.ppjwa.cn

[U07] Py：反转字典键值
来源：http://bmn.hammf.cn

{v: k for k, v in d.items()}
来源：http://qny.guannengcc.top

[U08] Py：展平二维列表
来源：http://pdp.jianghu66.top

[y for x in nested for y in x]
来源：http://hsn.hfpthk.cn

[U09] Py：字典取最大值的键
来源：http://bco.snrcjt.cn

max(d, key=d.get)
来源：http://srh.shzxlz.cn

[U10] Py：按值排序字典
来源：http://acm.sxryk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tvh.yuxming.cn

[U11] Py：生成器表达式
来源：http://dph.shuidangran.top

(x * 2 for x in arr)
来源：http://vef.hfpthk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rtk.meibo888.top

Counter(arr).most_common(3)
来源：http://yyn.dashuyun.cn

[U13] Py：固定长度队列
来源：http://mjj.cqqwz.cn

deque(maxlen=10)
来源：http://twu.sxryk.cn

[U14] Py：分组收集到列表
来源：http://ufh.ywan-chungtsiang.top

defaultdict(list)
来源：http://ewa.redwolf501.top

[U15] Py：高精度计时
来源：http://kcj.shangyingyoupin.top

t = time.perf_counter()
来源：http://qzz.vehdjk.com

[U16] Py：命令行参数解析
来源：http://bym.zhiwuduotai.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cny.jlsjyb.cn

[U17] Py：初始化日志
来源：http://iad.ehwqpu.com

logging.basicConfig(level=logging.INFO)
来源：http://msu.quarkkingdee.top

[U18] Py：预编译正则
来源：http://yuh.chenjidiqi.icu

pat = re.compile(r"\d+")
来源：http://rih.zhixingplan.top

[U19] Py：正则替换带回调
来源：http://vgp.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://unn.fktsv.cn

[U20] Py：缓存函数结果
来源：http://njc.yuxming.cn

@functools.lru_cache(maxsize=None)
来源：http://dcf.jinghuilouyu.cn

[U21] Py：自定义上下文管理器
来源：http://fxx.svipenyu.cn

@contextlib.contextmanager
来源：http://hqu.chenzaomai.com

[U22] Py：矩阵转置
来源：http://uga.wangshuangyany.cn

list(zip(*m))
来源：http://wqo.yonumen.top

[U23] Py：分块读取大文件
来源：http://kqq.nanxinkj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eol.tian-w.cn

[U24] Py：路径操作
来源：http://qzb.hnqzz.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://scd.snrcjt.cn

[U25] Py：CSV 按字典读
来源：http://zmz.zycfv.cn

csv.DictReader(f)
来源：http://svz.sxryk.cn

[U26] Py：并发下载
来源：http://wjb.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ljf.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://mfj.gaohongyu789.top

aiohttp.ClientSession() 配合 async with
来源：http://xpc.dashuyun.cn

[U28] Py：类型别名
来源：http://kak.hesvh.cn

UserId = int
来源：http://vru.zhoulong.xyz

[U29] Py：属性校验
来源：http://dyh.birdmap.top

@property 与 @x.setter 配合
来源：http://tsi.zdqjudy.top

[U30] Py：数据类
来源：http://fch.shanyushiyangkeji.top

@dataclass(slots=True)
来源：http://slz.gogol.net.cn

[U31] Py：单测
来源：http://bls.yangfankeji.com

python -m pytest -q
来源：http://laa.uphjek.com

[U32] Py：代码格式化
来源：http://sre.hnqzz.top

ruff format . && ruff check --fix .
来源：http://ipy.jqgfzy.top

[U33] Py：打包发布
来源：http://qoz.52xcode.cn

python -m build  （依赖 pyproject.toml）
来源：http://vmw.aibaodan.cn

[U34] Py：判断编码
来源：http://kfj.smart0.xyz

chardet.detect(raw)
来源：http://uhp.jinyuanbaomall.cn

[U35] Py：发送邮件
来源：http://mrd.zhiwuduotai.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zvr.pycfn.com

[U36] Py：定时任务
来源：http://wlq.guowangkeji.top

schedule.every(10).minutes.do(job)
来源：http://vub.ivvv.top

[U37] Py：读写 Excel
来源：http://eov.zhengqikj.top

pandas.read_excel / DataFrame.to_excel
来源：http://lfb.dashuyun.cn

[U38] Py：获取脚本所在目录
来源：http://jes.mhx1999.top

Path(__file__).resolve().parent
来源：http://tzz.daxiang520.top

[U39] Py：判断是否在交互环境
来源：http://oma.hcnkem.com

sys.stdout.isatty()
来源：http://rmz.fktsv.cn

[U40] Py：打印到标准错误
来源：http://udu.haohaochexian.top

print("err", file=sys.stderr)
来源：http://vmx.gaohongyu789.top

[U41] PHP：初始化 Composer 项目
来源：http://sao.jianghu66.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qen.xinyue.icu

[U42] PHP：PSR-4 自动加载
来源：http://nna.jinghuilouyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fsd.gotoacloud.top

[U43] PHP：声明命名空间
来源：http://fba.tian-w.cn

namespace App\Http;
来源：http://kbh.havefunace.top

[U44] PHP：开启严格类型
来源：http://zzf.guannengcc.top

declare(strict_types=1);
来源：http://bob.yongpay.top

[U45] PHP：类型声明与返回类型
来源：http://fjc.xinyue.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://fdc.fengsongda.top

[U46] PHP：可空类型
来源：http://rnh.jiagoushi.top

?string $name = null
来源：http://fpk.jinqigufen.top

[U47] PHP：联合类型
来源：http://nnp.jqgufenzy.top

int|string $id
来源：http://vwh.fehbvm.com

[U48] PHP：纯枚举
来源：http://luz.meibo888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gbb.jqgufenzy.top

[U49] PHP：只读属性
来源：http://znw.guowangkeji.top

public readonly string $name
来源：http://kdc.ppjwa.cn

[U50] PHP：构造器属性提升
来源：http://ona.sweek.top

public function __construct(private int $id) {}
来源：http://zjj.9152youxi.cn

[U51] PHP：数组解构
来源：http://syu.chenlongwang.top

[$a, $b] = $arr;
来源：http://bpf.cucudq.cn

[U52] PHP：箭头函数
来源：http://rbd.jinqigufen.top

$double = fn($x) => $x * 2;
来源：http://jvm.ydjk.org.cn

[U53] PHP：空合并运算符
来源：http://ktq.yj202588.top

$v = $a ?? $b ?? "default";
来源：http://qqj.fktsv.cn

[U54] PHP：空安全调用
来源：http://okf.birdmap.top

$obj?->method()
来源：http://izd.ehwqpu.com

[U55] PHP：match 表达式
来源：http://adf.cashguo.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rcv.hnqzz.top

[U56] PHP：命名参数
来源：http://jqo.hnxiangtu.top

f(a: 1, b: 2)
来源：http://kku.cashguo.top

[U57] PHP：字符串插值
来源：http://mno.hcnkem.com

"值: {$a}"
来源：http://ulh.cdnleiting.top

[U58] PHP：数组三件套
来源：http://dkw.ppjwa.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://len.zdqjudy.top

[U59] PHP：自定义排序
来源：http://pck.sxryk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qij.meibo888.top

[U60] PHP：JSON 编解码
来源：http://rmn.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kza.zhaomingkeji.xyz

[U61] PHP：正则
来源：http://wfg.sweek.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uzx.shanyushiyangtech.top

[U62] PHP：日期对象
来源：http://pah.jinghuilouyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xrh.sjlbkw.cn

[U63] PHP：文件读写
来源：http://gur.xziqi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xkc.cdnleiting.top

[U64] PHP：目录遍历
来源：http://sco.cdnleiting.top

glob("dir/*.php");  scandir("dir");
来源：http://neo.fanxiaobao.xyz

[U65] PHP：会话
来源：http://ytw.fanxiaobao.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://sbx.bjfxy.top

[U66] PHP：设置 Cookie
来源：http://ock.fengsongda.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vts.sweek.top

[U67] PHP：处理文件上传
来源：http://yov.316326.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uzk.sysykeji.top

[U68] PHP：PDO 连接
来源：http://mns.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sbm.zhengqikj.top

[U69] PHP：PDO 预处理
来源：http://inc.hcnkem.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tgv.zhixingplan.top

[U70] PHP：PDO 事务
来源：http://cgh.shanyushiyangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://euk.yongpay.top

[U71] PHP：抛出异常
来源：http://clp.chenlongwang.top

throw new RuntimeException("失败", 500);
来源：http://nhe.gzhubu.top

[U72] PHP：写错误日志
来源：http://obr.svipenyu.cn

error_log("失败: " . $e->getMessage());
来源：http://sfe.chenjidiqi.icu

[U73] PHP：读取 ini 配置
来源：http://fqm.jinqigfzy.top

parse_ini_file("config.ini", true)
来源：http://sry.jiagoushi.top

[U74] PHP：读取环境变量
来源：http://sdm.jinqigfzy.top

getenv("APP_ENV") ?: "production"
来源：http://ygu.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://usk.guowangkeji.top

composer require psr/container
来源：http://yji.yj20258.top

[U76] PHP：简单路由
来源：http://nkg.hysaishi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mns.chenzaomai.com

[U77] PHP：模板渲染
来源：http://lnt.xylfe.cn

composer require twig/twig
来源：http://hhk.haohaochexian.top

[U78] PHP：单元测试
来源：http://vff.c1oappe.top

composer require --dev phpunit/phpunit
来源：http://ehb.yangfankeji.com

[U79] PHP：静态分析
来源：http://ska.snrcjt.cn

composer require --dev phpstan/phpstan
来源：http://iiw.yfazqb.com

[U80] PHP：代码规范修复
来源：http://efm.hysaishi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://thd.ehwqpu.com

[U81] JS：初始化项目
来源：http://xjh.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://eqi.jyoumei.cn

[U82] JS：package.json 脚本
来源：http://ugj.jinqigfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kae.ppjwa.cn

[U83] JS：ES Module 导入导出
来源：http://lxf.pycfn.com

export const a = 1;  import { a } from "./m.js";
来源：http://mwn.aizwys.cn

[U84] JS：CommonJS 写法
来源：http://eof.hongshengwenyu.top

module.exports = { a };  const { a } = require("./m");
来源：http://myw.ctjpmb.com

[U85] JS：可选链
来源：http://lgo.zhijiandao.cn

a?.b?.c
来源：http://nfi.shzxlz.cn

[U86] JS：空值合并
来源：http://nqk.pengpengdd.cyou

a ?? b
来源：http://jkp.yvedp.cn

[U87] JS：解构默认值
来源：http://lgh.feifeiyinyue.top

const { a = 1, b = 2 } = obj;
来源：http://tir.chenjidiqi.icu

[U88] JS：对象展开合并
来源：http://cst.zhaomingkeji.xyz

{ ...a, ...b }
来源：http://nek.tanke756.top

[U89] JS：数组去重
来源：http://zfj.svipenyu.cn

[...new Set(arr)]
来源：http://rrz.ctjpmb.com

[U90] JS：数字数组排序
来源：http://oma.jyoumei.cn

[...arr].sort((a, b) => a - b)
来源：http://ipk.zhongyouzk.top

[U91] JS：对象键值遍历
来源：http://ppm.yongpay.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gsh.jinqigufen.top

[U92] JS：深拷贝
来源：http://ywg.andypj.xyz

structuredClone(obj)
来源：http://ems.cqqwz.cn

[U93] JS：模板字符串
来源：http://yjw.hammf.cn

`共 ${n} 条`
来源：http://cdi.mhx1999.top

[U94] JS：箭头函数
来源：http://ilt.guannengcc.top

const double = x => x * 2;
来源：http://ovl.xingfuxueyuan.xyz

[U95] JS：Promise 包装
来源：http://khu.9152youxi.cn

new Promise((resolve, reject) => {})
来源：http://hyy.xuanzx.com

[U96] JS：async/await 与异常
来源：http://xru.xuanzx.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://myr.gaohongyu789.top

[U97] JS：并发请求
来源：http://zbv.shanyushiyangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://wwv.hywenlv.cn

[U98] JS：fetch 带 JSON
来源：http://hgx.jinyuanbaomall.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://how.zhijiandao.cn

[U99] JS：事件监听
来源：http://fvn.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://xpo.zdbjq.cn

[U100] JS：DOM 查询
来源：http://qyu.yj202588.top

document.querySelector(".item")
来源：http://fnr.zhoulong.xyz

[U101] JS：classList 操作
来源：http://jpt.pengpengdd.cyou

el.classList.toggle("active")
来源：http://gyc.shuidangran.top

[U102] JS：本地存储
来源：http://xhz.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pvs.xinyue.icu

[U103] JS：定时器
来源：http://kgp.ybcxt.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oxu.shanyushiyangtech.top

[U104] JS：防抖
来源：http://zaz.gogol.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gag.yj20258.top

[U105] JS：节流
来源：http://cap.9152youxi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://svh.bjfxy.top

[U106] JS：日期格式化
来源：http://vii.zdbjq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wln.hywenlv.cn

[U107] JS：数字千分位
来源：http://mvw.jyoumei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ccd.jlsjyb.cn

[U108] JS：随机整数
来源：http://kti.yfazqb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dsl.jinqigfzy.top

[U109] JS：数组分组
来源：http://xdf.ivvv.top

Object.groupBy(arr, x => x.type)
来源：http://jos.guannengcc.top

[U110] JS：数组分块
来源：http://uxz.ywan-chungtsiang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yzx.sufxvd.cn

[U111] JS：对象转 Map
来源：http://mwt.gotoacloud.top

new Map(Object.entries(obj))
来源：http://yhq.tanke756.top

[U112] JS：字符串补位
来源：http://yjs.wangshuangyany.cn

"7".padStart(3, "0")
来源：http://sug.gogol.net.cn

[U113] JS：正则替换全部
来源：http://ygj.jinqigufen.top

s.replaceAll("a", "b")
来源：http://enb.vehdjk.com

[U114] JS：JSON 深比较
来源：http://tjb.yj202588.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ofz.sweek.top

[U115] JS：生成 UUID
来源：http://tlj.sweek.top

crypto.randomUUID()
来源：http://kyw.cqqwz.cn

[U116] JS：类型检查（JSDoc）
来源：http://isb.quarkkingdee.top

/** @param {string} name */ function f(name) {}
来源：http://gbj.hywenlv.cn


<!-- 参考信息 -->