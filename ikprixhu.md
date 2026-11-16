代发 wailian999

[T35] Lua：字典表
来源：http://nuy.ywan-chungtsiang.top

local d = { a = 1 };  d.b = 2
来源：http://hkj.ydjk.org.cn

[T36] Lua：函数
来源：http://egb.jianghu66.top

function add(a, b) return a + b end
来源：http://hbq.chenlongwang.top

[T37] Lua：字符串拼接
来源：http://bwa.xylfe.cn

"a" .. "b"
来源：http://gmv.yongpay.top

[T38] Lua：条件
来源：http://xuf.bbcook.cn

if x > 0 then print("正") end
来源：http://euv.jinyuanbaomall.cn

[T39] Lua：模式匹配
来源：http://lob.hfpthk.cn

string.find(s, "%d+")
来源：http://mja.yonumen.top

[T40] Lua：元表
来源：http://fag.jlsjyb.cn

setmetatable({}, { __index = base })
来源：http://rgx.nwbrower.top

[T41] Perl：Hello World
来源：http://vqr.haohaochexian.top

print "Hello\n";
来源：http://nto.yangfankeji.com

[T42] Perl：变量类型
来源：http://cob.cashguo.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://trt.fengsongda.top

[T43] Perl：字符串插值
来源：http://osl.ydzc1.top

"值: $a"
来源：http://wnc.dashuyun.cn

[T44] Perl：条件
来源：http://ets.feifeiyinyue.top

if ($a > 0) { print "正"; }
来源：http://tnf.yj20258.top

[T45] Perl：数组遍历
来源：http://nev.iojbl.cn

for my $x (@arr) { print $x; }
来源：http://rjd.daxiang520.top

[T46] Perl：哈希操作
来源：http://its.hcnkem.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hvs.tanke756.top

[T47] Perl：正则捕获
来源：http://fja.9152youxi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uzr.daxiang520.top

[T48] Perl：正则替换
来源：http://cna.vehdjk.com

$s =~ s/old/new/g;
来源：http://tor.feifeiyinyue.top

[T49] Perl：函数
来源：http://agd.yongpay.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xso.ywan-chungtsiang.top

[T50] Perl：逐行读文件
来源：http://ixt.shangyingyoupin.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lhy.hesvh.cn

while (my $line = <$fh>) { print $line; }
来源：http://xun.nwbrower.top

[T51] Scala：Hello World
来源：http://uue.tarul.cn

println("Hello")
来源：http://nss.fehbvm.com

[T52] Scala：变量
来源：http://usm.zdqjudy.top

val a = 1;  var b = 2
来源：http://jfa.zhixingplan.top

[T53] Scala：字符串插值
来源：http://ham.yj202588.top

s"值: $b"
来源：http://loj.yj20258888.top

[T54] Scala：集合映射
来源：http://ckq.wangdashe.top

List(1, 2, 3).map(_ * 2)
来源：http://tdk.vqdsnc.cn

[T55] Scala：集合过滤
来源：http://bjj.sysykeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://yzq.smart0.xyz

[T56] Scala：样例类
来源：http://jlf.ctjpmb.com

case class User(name: String, age: Int)
来源：http://bwk.shangyingyoupin.top

[T57] Scala：模式匹配
来源：http://ixa.kuanghao11.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://njo.ehwqpu.com

[T58] Scala：函数定义
来源：http://mlo.xinyue.icu

def add(a: Int, b: Int): Int = a + b
来源：http://lbk.hysaishi.cn

[T59] Scala：循环
来源：http://fsa.chenjidiqi.icu

for (i <- 1 to 10) println(i)
来源：http://agr.ctjpmb.com

[T60] Scala：折叠
来源：http://ppx.0kj1m.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tfd.tanke756.top

================================================================================
来源：http://ldo.xuanzx.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lrp.pengpengdd.cyou

================================================================================
来源：http://pvm.gzhubu.top

[U01] Py：创建虚拟环境
来源：http://awr.tianlin.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://vxa.cqqwz.cn

[U02] Py：导出 / 安装依赖
来源：http://sfs.kuanghao11.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rkd.tianlin.xyz

[U03] Py：加载 .env 配置
来源：http://wdm.zhongyouzk.top

from dotenv import load_dotenv; load_dotenv()
来源：http://eom.yueranfly.top

[U04] Py：变量调试打印
来源：http://rkd.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uni.hammf.cn

[U05] Py：列表去重且保序
来源：http://trl.ppjwa.cn

list(dict.fromkeys(arr))
来源：http://gpb.sxryk.cn

[U06] Py：合并两个字典
来源：http://xfb.ehwqpu.com

{**a, **b}
来源：http://omc.sufxvd.cn

[U07] Py：反转字典键值
来源：http://not.fanxiaobao.xyz

{v: k for k, v in d.items()}
来源：http://xla.yuxming.cn

[U08] Py：展平二维列表
来源：http://rqv.svipenyu.cn

[y for x in nested for y in x]
来源：http://fre.ydzc1.top

[U09] Py：字典取最大值的键
来源：http://wef.fanxiaobao.xyz

max(d, key=d.get)
来源：http://ymx.chenjidiqi.icu

[U10] Py：按值排序字典
来源：http://rfb.redwolf501.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uts.xziqi.cn

[U11] Py：生成器表达式
来源：http://mds.jinqigufen.top

(x * 2 for x in arr)
来源：http://dpv.tarul.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jiz.zhaomingkeji.xyz

Counter(arr).most_common(3)
来源：http://yre.cashguo.top

[U13] Py：固定长度队列
来源：http://jus.sweek.top

deque(maxlen=10)
来源：http://lef.gaohongyu789.top

[U14] Py：分组收集到列表
来源：http://jgk.redwolf501.top

defaultdict(list)
来源：http://ofp.bbcook.cn

[U15] Py：高精度计时
来源：http://fyf.shangyingyoupin.top

t = time.perf_counter()
来源：http://cmv.yanxiufei.cn

[U16] Py：命令行参数解析
来源：http://epv.feifeiyinyue.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cny.mhx1999.top

[U17] Py：初始化日志
来源：http://nzg.zhoulong.xyz

logging.basicConfig(level=logging.INFO)
来源：http://ehz.hnqzz.top

[U18] Py：预编译正则
来源：http://aqz.shanyushiyangkeji.top

pat = re.compile(r"\d+")
来源：http://jxi.dashuyun.cn

[U19] Py：正则替换带回调
来源：http://vcf.bjfxy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zxx.0kj1m.cn

[U20] Py：缓存函数结果
来源：http://esw.zhiwuduotai.top

@functools.lru_cache(maxsize=None)
来源：http://rdm.jinqigfzy.top

[U21] Py：自定义上下文管理器
来源：http://hxg.fanxiaobao.xyz

@contextlib.contextmanager
来源：http://pns.smart0.xyz

[U22] Py：矩阵转置
来源：http://lka.0kj1m.cn

list(zip(*m))
来源：http://dkj.vqdsnc.cn

[U23] Py：分块读取大文件
来源：http://hyt.uphjek.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fkf.hfpthk.cn

[U24] Py：路径操作
来源：http://qbh.gzhubu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lzj.pengpengdd.cyou

[U25] Py：CSV 按字典读
来源：http://axc.hfpthk.cn

csv.DictReader(f)
来源：http://wpa.fehbvm.com

[U26] Py：并发下载
来源：http://sod.ppjwa.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rko.zhoulong.xyz

[U27] Py：异步 HTTP
来源：http://vji.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://lkh.sysykeji.top

[U28] Py：类型别名
来源：http://jra.aizwys.cn

UserId = int
来源：http://gyh.tanke756.top

[U29] Py：属性校验
来源：http://cdd.guowangkeji.top

@property 与 @x.setter 配合
来源：http://phd.daria6918.cn

[U30] Py：数据类
来源：http://lck.smart0.xyz

@dataclass(slots=True)
来源：http://mrw.xziqi.cn

[U31] Py：单测
来源：http://evm.xylfe.cn

python -m pytest -q
来源：http://hmi.tarul.cn

[U32] Py：代码格式化
来源：http://nan.zhixingplan.top

ruff format . && ruff check --fix .
来源：http://ihx.jyoumei.cn

[U33] Py：打包发布
来源：http://mll.yanxiufei.cn

python -m build  （依赖 pyproject.toml）
来源：http://cri.xuanzx.com

[U34] Py：判断编码
来源：http://flt.jinqigufen.top

chardet.detect(raw)
来源：http://pqo.bjfxy.top

[U35] Py：发送邮件
来源：http://kvm.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://upo.fanxiaobao.xyz

[U36] Py：定时任务
来源：http://zot.tanke756.top

schedule.every(10).minutes.do(job)
来源：http://kqe.snrcjt.cn

[U37] Py：读写 Excel
来源：http://ysq.ydzc1.top

pandas.read_excel / DataFrame.to_excel
来源：http://cxh.tarul.cn

[U38] Py：获取脚本所在目录
来源：http://vpe.cqqwz.cn

Path(__file__).resolve().parent
来源：http://sgv.epnwcf.com

[U39] Py：判断是否在交互环境
来源：http://acd.hfpthk.cn

sys.stdout.isatty()
来源：http://eqw.zhixingplan.top

[U40] Py：打印到标准错误
来源：http://nqi.jinghuilouyu.cn

print("err", file=sys.stderr)
来源：http://prl.jinqigfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://pvh.epnwcf.com

composer init;  composer require guzzlehttp/guzzle
来源：http://huy.nanxuanxn.top

[U42] PHP：PSR-4 自动加载
来源：http://rch.zhixingplan.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jno.zhiwuduotai.top

[U43] PHP：声明命名空间
来源：http://zwe.zhaomingkeji.xyz

namespace App\Http;
来源：http://yvd.ehwqpu.com

[U44] PHP：开启严格类型
来源：http://dto.bjfxy.top

declare(strict_types=1);
来源：http://qfn.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://smk.yj20258888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://rdl.daria6918.cn

[U46] PHP：可空类型
来源：http://gta.nwbrower.top

?string $name = null
来源：http://yge.snrcjt.cn

[U47] PHP：联合类型
来源：http://dls.sweek.top

int|string $id
来源：http://hgg.yangfankeji.com

[U48] PHP：纯枚举
来源：http://fdi.haohaochexian.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ebv.shangyingyoupin.top

[U49] PHP：只读属性
来源：http://cmb.yvedp.cn

public readonly string $name
来源：http://jrg.cheryme.top

[U50] PHP：构造器属性提升
来源：http://tst.52xcode.cn

public function __construct(private int $id) {}
来源：http://hba.yuanzhike.top

[U51] PHP：数组解构
来源：http://aga.fengsongda.top

[$a, $b] = $arr;
来源：http://gtf.jiagoushi.top

[U52] PHP：箭头函数
来源：http://hlu.zycfv.cn

$double = fn($x) => $x * 2;
来源：http://kqj.jinqigufen.top

[U53] PHP：空合并运算符
来源：http://kjc.wangdashe.top

$v = $a ?? $b ?? "default";
来源：http://owh.zycfv.cn

[U54] PHP：空安全调用
来源：http://jpt.sysykeji.top

$obj?->method()
来源：http://fwj.xziqi.cn

[U55] PHP：match 表达式
来源：http://yys.yongpay.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kuj.yj20258888.top

[U56] PHP：命名参数
来源：http://hdz.hfpthk.cn

f(a: 1, b: 2)
来源：http://ujg.mhx1999.top

[U57] PHP：字符串插值
来源：http://kky.jlsjyb.cn

"值: {$a}"
来源：http://kly.jqgufenzy.top

[U58] PHP：数组三件套
来源：http://qve.316326.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://soq.guowangkeji.top

[U59] PHP：自定义排序
来源：http://kur.jqgufenzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bbv.ydzc1.top

[U60] PHP：JSON 编解码
来源：http://ldn.zycfv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://muj.aizwys.cn

[U61] PHP：正则
来源：http://umb.nanxuanxn.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yqc.jinyuanbaomall.cn

[U62] PHP：日期对象
来源：http://bia.vqdsnc.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gzo.redwolf501.top

[U63] PHP：文件读写
来源：http://zci.jqgufenzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yez.nanxuanxn.top

[U64] PHP：目录遍历
来源：http://nzl.yj202588.top

glob("dir/*.php");  scandir("dir");
来源：http://vpn.sweek.top

[U65] PHP：会话
来源：http://bfk.jqgfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hnn.tian-w.cn

[U66] PHP：设置 Cookie
来源：http://ocl.wangshuangyany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hyt.sxryk.cn

[U67] PHP：处理文件上传
来源：http://xco.cashguo.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://udd.kuanghao11.cn

[U68] PHP：PDO 连接
来源：http://qbg.hongshengwenyu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lsa.hcnkem.com

[U69] PHP：PDO 预处理
来源：http://rrp.aizwys.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mwt.cdnleiting.top

[U70] PHP：PDO 事务
来源：http://qrf.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://imj.andypj.xyz

[U71] PHP：抛出异常
来源：http://mef.quarkkingdee.top

throw new RuntimeException("失败", 500);
来源：http://qxe.hcnkem.com

[U72] PHP：写错误日志
来源：http://mmj.ybcxt.top

error_log("失败: " . $e->getMessage());
来源：http://auo.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://qnd.0kj1m.cn

parse_ini_file("config.ini", true)
来源：http://wez.chenlongwang.top

[U74] PHP：读取环境变量
来源：http://vsf.bjfxy.top

getenv("APP_ENV") ?: "production"
来源：http://gna.iojbl.cn

[U75] PHP：依赖注入
来源：http://fjo.nanxinkj.top

composer require psr/container
来源：http://tnj.fzhhl.top

[U76] PHP：简单路由
来源：http://eue.chenjidiqi.icu

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ufs.yfazqb.com

[U77] PHP：模板渲染
来源：http://pss.hywenlv.cn

composer require twig/twig
来源：http://qhi.yongpay.top

[U78] PHP：单元测试
来源：http://psd.xinyue.icu

composer require --dev phpunit/phpunit
来源：http://uap.andypj.xyz

[U79] PHP：静态分析
来源：http://rqw.yueranfly.top

composer require --dev phpstan/phpstan
来源：http://etb.cdnleiting.top

[U80] PHP：代码规范修复
来源：http://xiz.jinqigufen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dps.dashuyun.cn

[U81] JS：初始化项目
来源：http://gza.dianchejie.cn

npm init -y;  npm i express
来源：http://sne.yongpay.top

[U82] JS：package.json 脚本
来源：http://mmp.xylfe.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nix.gaohongyu789.top

[U83] JS：ES Module 导入导出
来源：http://nhb.aibaodan.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wbg.shzxlz.cn

[U84] JS：CommonJS 写法
来源：http://jlj.jqgufenzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://xzg.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://aec.yanxiufei.cn

a?.b?.c
来源：http://hqz.hammf.cn

[U86] JS：空值合并
来源：http://sei.jinqigfzy.top

a ?? b
来源：http://icp.yuxming.cn

[U87] JS：解构默认值
来源：http://ogm.epnwcf.com

const { a = 1, b = 2 } = obj;
来源：http://cqn.zhijiandao.cn

[U88] JS：对象展开合并
来源：http://inp.wangdashe.top

{ ...a, ...b }
来源：http://uyd.tian-w.cn

[U89] JS：数组去重
来源：http://zxo.bbcook.cn

[...new Set(arr)]
来源：http://cpx.tarul.cn

[U90] JS：数字数组排序
来源：http://osa.tarul.cn

[...arr].sort((a, b) => a - b)
来源：http://dpp.dianchejie.cn

[U91] JS：对象键值遍历
来源：http://twm.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://htq.316326.xyz

[U92] JS：深拷贝
来源：http://llg.daria6918.cn

structuredClone(obj)
来源：http://vkk.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://ysv.feifeiyinyue.top

`共 ${n} 条`
来源：http://fqn.jqgufenzy.top

[U94] JS：箭头函数
来源：http://ptn.sysykeji.top

const double = x => x * 2;
来源：http://tfm.hysaishi.cn

[U95] JS：Promise 包装
来源：http://hwm.xziqi.cn

new Promise((resolve, reject) => {})
来源：http://dzd.zycfv.cn

[U96] JS：async/await 与异常
来源：http://jyz.vqdsnc.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gfx.ehwqpu.com

[U97] JS：并发请求
来源：http://vgb.hesvh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xjo.shangyingyoupin.top

[U98] JS：fetch 带 JSON
来源：http://oxq.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vde.tarul.cn

[U99] JS：事件监听
来源：http://suh.tanke756.top

el.addEventListener("click", e => {})
来源：http://feb.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://ela.zdqjudy.top

document.querySelector(".item")
来源：http://law.xuanzx.com

[U101] JS：classList 操作
来源：http://pbl.sysykeji.top

el.classList.toggle("active")
来源：http://lzi.jqgufenzy.top

[U102] JS：本地存储
来源：http://map.jinyuanbaomall.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://eio.52xcode.cn

[U103] JS：定时器
来源：http://xvx.aibaodan.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wco.yj202588.top

[U104] JS：防抖
来源：http://egz.redwolf501.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ium.jlsjyb.cn

[U105] JS：节流
来源：http://bwm.yj202588.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bym.zhoulong.xyz

[U106] JS：日期格式化
来源：http://afo.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xiv.zdqjudy.top

[U107] JS：数字千分位
来源：http://bnd.xziqi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://daf.hysaishi.cn

[U108] JS：随机整数
来源：http://bai.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://whd.jiagoushi.top

[U109] JS：数组分组
来源：http://bvc.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://err.xziqi.cn

[U110] JS：数组分块
来源：http://mbv.jinghuilouyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vhe.snrcjt.cn

[U111] JS：对象转 Map
来源：http://anu.yonumen.top

new Map(Object.entries(obj))
来源：http://plr.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://knf.hcnkem.com

"7".padStart(3, "0")
来源：http://nkq.aizwys.cn

[U113] JS：正则替换全部
来源：http://nmo.svipenyu.cn

s.replaceAll("a", "b")
来源：http://aew.nanxinkj.top

[U114] JS：JSON 深比较
来源：http://trv.fzhhl.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fas.dianchejie.cn

[U115] JS：生成 UUID
来源：http://ytp.0kj1m.cn

crypto.randomUUID()
来源：http://tqb.nanxuanxn.top

[U116] JS：类型检查（JSDoc）
来源：http://cws.sweek.top

/** @param {string} name */ function f(name) {}
来源：http://ldo.tianlin.xyz

[U117] JS：单元测试
来源：http://nrr.hcnkem.com

npm i -D vitest;  npx vitest
来源：http://aes.yonumen.top

[U118] JS：开发服务器
来源：http://zga.zhijiandao.cn

npm i -D vite;  npx vite
来源：http://hwf.jianghu66.top

[U119] JS：生产构建
来源：http://hnq.ydjk.org.cn

npx vite build
来源：http://nah.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://mui.shanyushiyangkeji.top

import.meta.env.VITE_API_URL
来源：http://dom.jianghu66.top

================================================================================
来源：http://crw.9152youxi.cn

统计汇总
来源：http://qmb.epnwcf.com

================================================================================
来源：http://skq.aizwys.cn

按语言统计（条）：
来源：http://utw.tianlin.xyz


<!-- 参考信息 -->