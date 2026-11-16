代发 wailian999

[T37] Lua：字符串拼接
来源：http://hhr.hongshengwenyu.top

"a" .. "b"
来源：http://ugq.uphjek.com

[T38] Lua：条件
来源：http://nlc.jiagoushi.top

if x > 0 then print("正") end
来源：http://oam.bbcook.cn

[T39] Lua：模式匹配
来源：http://cvu.wangshuangyany.cn

string.find(s, "%d+")
来源：http://hnn.zhijiandao.cn

[T40] Lua：元表
来源：http://ohn.dashuyun.cn

setmetatable({}, { __index = base })
来源：http://ssw.fzhhl.top

[T41] Perl：Hello World
来源：http://cme.birdmap.top

print "Hello\n";
来源：http://xei.ybcxt.top

[T42] Perl：变量类型
来源：http://egp.jinqigfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jyl.ybcxt.top

[T43] Perl：字符串插值
来源：http://jku.zdbjq.cn

"值: $a"
来源：http://yrv.guannengcc.top

[T44] Perl：条件
来源：http://gsq.zdqjudy.top

if ($a > 0) { print "正"; }
来源：http://hrm.zhiwuduotai.top

[T45] Perl：数组遍历
来源：http://ioa.xingfuxueyuan.xyz

for my $x (@arr) { print $x; }
来源：http://war.tianlin.xyz

[T46] Perl：哈希操作
来源：http://glc.gzhubu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sbv.haohaochexian.top

[T47] Perl：正则捕获
来源：http://tqk.chenlongwang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kfo.smart0.xyz

[T48] Perl：正则替换
来源：http://agr.svipenyu.cn

$s =~ s/old/new/g;
来源：http://mrv.sysykeji.top

[T49] Perl：函数
来源：http://ucf.aizwys.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yru.haohaochexian.top

[T50] Perl：逐行读文件
来源：http://ttt.pengpengdd.cyou

open my $fh, "<", "a.txt" or die $!;
来源：http://syu.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://gdp.ybcxt.top

[T51] Scala：Hello World
来源：http://vut.epnwcf.com

println("Hello")
来源：http://bwi.jinghuilouyu.cn

[T52] Scala：变量
来源：http://cwp.cdnleiting.top

val a = 1;  var b = 2
来源：http://ktr.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://qow.ctjpmb.com

s"值: $b"
来源：http://iun.yangfankeji.com

[T54] Scala：集合映射
来源：http://orm.zhoulong.xyz

List(1, 2, 3).map(_ * 2)
来源：http://alf.gogol.net.cn

[T55] Scala：集合过滤
来源：http://cqe.sufxvd.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rjj.zycfv.cn

[T56] Scala：样例类
来源：http://xqw.jinghuilouyu.cn

case class User(name: String, age: Int)
来源：http://swq.yanxiufei.cn

[T57] Scala：模式匹配
来源：http://czw.ywan-chungtsiang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vww.shuidangran.top

[T58] Scala：函数定义
来源：http://etj.chenjidiqi.icu

def add(a: Int, b: Int): Int = a + b
来源：http://dxo.daria6918.cn

[T59] Scala：循环
来源：http://uaf.yongpay.top

for (i <- 1 to 10) println(i)
来源：http://ebt.gogol.net.cn

[T60] Scala：折叠
来源：http://dqe.vehdjk.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://szj.meibo888.top

================================================================================
来源：http://boh.hesvh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://olm.andypj.xyz

================================================================================
来源：http://mor.zhoulong.xyz

[U01] Py：创建虚拟环境
来源：http://vxe.daria6918.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qje.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://hqy.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qun.kuanghao11.cn

[U03] Py：加载 .env 配置
来源：http://hvx.xuetiantiany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gsn.jinqigufen.top

[U04] Py：变量调试打印
来源：http://gkm.hnqzz.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qju.yuanzhike.top

[U05] Py：列表去重且保序
来源：http://fmg.zhiwuduotai.top

list(dict.fromkeys(arr))
来源：http://slo.cucudq.cn

[U06] Py：合并两个字典
来源：http://kvs.zhixingplan.top

{**a, **b}
来源：http://kme.jinqigufen.top

[U07] Py：反转字典键值
来源：http://pha.ybcxt.top

{v: k for k, v in d.items()}
来源：http://yov.jqgufenzy.top

[U08] Py：展平二维列表
来源：http://ynz.havefunace.top

[y for x in nested for y in x]
来源：http://qpi.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://fpr.shuidangran.top

max(d, key=d.get)
来源：http://ssm.haohaochexian.top

[U10] Py：按值排序字典
来源：http://zsn.jyoumei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qel.hesvh.cn

[U11] Py：生成器表达式
来源：http://fqf.ivvv.top

(x * 2 for x in arr)
来源：http://mnt.zhaomingkeji.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://kcy.ivvv.top

Counter(arr).most_common(3)
来源：http://tnj.bjfxy.top

[U13] Py：固定长度队列
来源：http://yhp.jinqigufen.top

deque(maxlen=10)
来源：http://mws.yanxiufei.cn

[U14] Py：分组收集到列表
来源：http://xpu.hnxiangtu.top

defaultdict(list)
来源：http://iop.xziqi.cn

[U15] Py：高精度计时
来源：http://ind.hammf.cn

t = time.perf_counter()
来源：http://hpd.c1oappe.top

[U16] Py：命令行参数解析
来源：http://gex.tanke756.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hgr.vqdsnc.cn

[U17] Py：初始化日志
来源：http://ppe.cucudq.cn

logging.basicConfig(level=logging.INFO)
来源：http://tqi.jlsjyb.cn

[U18] Py：预编译正则
来源：http://kff.cdnleiting.top

pat = re.compile(r"\d+")
来源：http://fgw.quarkkingdee.top

[U19] Py：正则替换带回调
来源：http://vbj.andypj.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tpp.yj20258.top

[U20] Py：缓存函数结果
来源：http://jdb.gaohongyu789.top

@functools.lru_cache(maxsize=None)
来源：http://sws.jlsjyb.cn

[U21] Py：自定义上下文管理器
来源：http://rqn.0kj1m.cn

@contextlib.contextmanager
来源：http://uik.yangfankeji.com

[U22] Py：矩阵转置
来源：http://lnj.snrcjt.cn

list(zip(*m))
来源：http://vzj.cashguo.top

[U23] Py：分块读取大文件
来源：http://dsd.yj202588.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lqv.svipenyu.cn

[U24] Py：路径操作
来源：http://yzu.nanxinkj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dnj.shangyingyoupin.top

[U25] Py：CSV 按字典读
来源：http://snp.gogol.net.cn

csv.DictReader(f)
来源：http://xlp.cqqwz.cn

[U26] Py：并发下载
来源：http://tiu.yfazqb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ghh.shanyushiyangkeji.top

[U27] Py：异步 HTTP
来源：http://dxe.wangshuangyany.cn

aiohttp.ClientSession() 配合 async with
来源：http://vtr.hongshengwenyu.top

[U28] Py：类型别名
来源：http://mcw.guannengcc.top

UserId = int
来源：http://uax.tanke756.top

[U29] Py：属性校验
来源：http://not.aibaodan.cn

@property 与 @x.setter 配合
来源：http://lcb.nanxuanxn.top

[U30] Py：数据类
来源：http://efu.c1oappe.top

@dataclass(slots=True)
来源：http://btv.zhongyouzk.top

[U31] Py：单测
来源：http://yqq.jinqigufen.top

python -m pytest -q
来源：http://vug.shanyushiyangkeji.top

[U32] Py：代码格式化
来源：http://gbz.xylfe.cn

ruff format . && ruff check --fix .
来源：http://rrp.cdnleiting.top

[U33] Py：打包发布
来源：http://drb.ppjwa.cn

python -m build  （依赖 pyproject.toml）
来源：http://jax.jinyuanbaomall.cn

[U34] Py：判断编码
来源：http://som.havefunace.top

chardet.detect(raw)
来源：http://zgr.iojbl.cn

[U35] Py：发送邮件
来源：http://phc.hcnkem.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zwd.xziqi.cn

[U36] Py：定时任务
来源：http://geg.hysaishi.cn

schedule.every(10).minutes.do(job)
来源：http://wje.nwbrower.top

[U37] Py：读写 Excel
来源：http://sxo.havefunace.top

pandas.read_excel / DataFrame.to_excel
来源：http://ema.sufxvd.cn

[U38] Py：获取脚本所在目录
来源：http://ywi.guannengcc.top

Path(__file__).resolve().parent
来源：http://npi.meibo888.top

[U39] Py：判断是否在交互环境
来源：http://xzy.shangyingyoupin.top

sys.stdout.isatty()
来源：http://ndh.jyoumei.cn

[U40] Py：打印到标准错误
来源：http://udv.9152youxi.cn

print("err", file=sys.stderr)
来源：http://ayv.shanyushiyangtech.top

[U41] PHP：初始化 Composer 项目
来源：http://fhc.fzhhl.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ika.yueranfly.top

[U42] PHP：PSR-4 自动加载
来源：http://zrf.jqgufenzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cil.bjfxy.top

[U43] PHP：声明命名空间
来源：http://amf.sufxvd.cn

namespace App\Http;
来源：http://fep.fktsv.cn

[U44] PHP：开启严格类型
来源：http://bbc.daria6918.cn

declare(strict_types=1);
来源：http://tdo.shanyushiyangtech.top

[U45] PHP：类型声明与返回类型
来源：http://myk.ybcxt.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fgz.fanxiaobao.xyz

[U46] PHP：可空类型
来源：http://tjp.bjfxy.top

?string $name = null
来源：http://kqu.zhongyouzk.top

[U47] PHP：联合类型
来源：http://anp.jianghu66.top

int|string $id
来源：http://fju.hnxiangtu.top

[U48] PHP：纯枚举
来源：http://rjt.ywan-chungtsiang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lgt.guowangkeji.top

[U49] PHP：只读属性
来源：http://xdj.feifeiyinyue.top

public readonly string $name
来源：http://hnh.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://gfu.hcnkem.com

public function __construct(private int $id) {}
来源：http://ycv.jianghu66.top

[U51] PHP：数组解构
来源：http://ldt.yj202588.top

[$a, $b] = $arr;
来源：http://mcu.yj202588.top

[U52] PHP：箭头函数
来源：http://fty.cashguo.top

$double = fn($x) => $x * 2;
来源：http://grw.chenjidiqi.icu

[U53] PHP：空合并运算符
来源：http://jdn.uphjek.com

$v = $a ?? $b ?? "default";
来源：http://wsh.tanke756.top

[U54] PHP：空安全调用
来源：http://ekr.cucudq.cn

$obj?->method()
来源：http://ihi.guannengcc.top

[U55] PHP：match 表达式
来源：http://agy.fzhhl.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jpp.c1oappe.top

[U56] PHP：命名参数
来源：http://uor.ybcxt.top

f(a: 1, b: 2)
来源：http://puz.jiagoushi.top

[U57] PHP：字符串插值
来源：http://tur.yonumen.top

"值: {$a}"
来源：http://pex.xinyue.icu

[U58] PHP：数组三件套
来源：http://bvj.kuanghao11.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uds.ydjk.org.cn

[U59] PHP：自定义排序
来源：http://uxl.ybcxt.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wsp.xylfe.cn

[U60] PHP：JSON 编解码
来源：http://mgs.birdmap.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hnw.zdbjq.cn

[U61] PHP：正则
来源：http://eqm.52xcode.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hqk.snrcjt.cn

[U62] PHP：日期对象
来源：http://uuw.feifeiyinyue.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ewe.hywenlv.cn

[U63] PHP：文件读写
来源：http://mba.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bfd.yueranfly.top

[U64] PHP：目录遍历
来源：http://tda.zdqjudy.top

glob("dir/*.php");  scandir("dir");
来源：http://whv.yj20258.top

[U65] PHP：会话
来源：http://fwo.0kj1m.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lxh.svipenyu.cn

[U66] PHP：设置 Cookie
来源：http://qpg.havefunace.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jvt.jinqigfzy.top

[U67] PHP：处理文件上传
来源：http://fux.shanyushiyangtech.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sar.9152youxi.cn

[U68] PHP：PDO 连接
来源：http://osg.ybcxt.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lhp.52xcode.cn

[U69] PHP：PDO 预处理
来源：http://hqt.vehdjk.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xiq.hywenlv.cn

[U70] PHP：PDO 事务
来源：http://ehj.shzxlz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ojc.hesvh.cn

[U71] PHP：抛出异常
来源：http://ovy.gotoacloud.top

throw new RuntimeException("失败", 500);
来源：http://tud.cdnleiting.top

[U72] PHP：写错误日志
来源：http://bdx.hongshengwenyu.top

error_log("失败: " . $e->getMessage());
来源：http://pxs.zhoulong.xyz

[U73] PHP：读取 ini 配置
来源：http://iwz.chenzaomai.com

parse_ini_file("config.ini", true)
来源：http://mxh.zhijiandao.cn

[U74] PHP：读取环境变量
来源：http://zlj.gaohongyu789.top

getenv("APP_ENV") ?: "production"
来源：http://ubw.jqgufenzy.top

[U75] PHP：依赖注入
来源：http://cqx.cheryme.top

composer require psr/container
来源：http://dqx.tanke756.top

[U76] PHP：简单路由
来源：http://bpk.cashguo.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nvz.0kj1m.cn

[U77] PHP：模板渲染
来源：http://odg.yj20258888.top

composer require twig/twig
来源：http://dme.xuetiantiany.cn

[U78] PHP：单元测试
来源：http://lni.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://ajb.jlsjyb.cn

[U79] PHP：静态分析
来源：http://dgh.svipenyu.cn

composer require --dev phpstan/phpstan
来源：http://pjj.andypj.xyz

[U80] PHP：代码规范修复
来源：http://cep.ivvv.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gma.cashguo.top

[U81] JS：初始化项目
来源：http://nox.guowangkeji.top

npm init -y;  npm i express
来源：http://rln.tanke756.top

[U82] JS：package.json 脚本
来源：http://nbr.xingfuxueyuan.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yzn.tarul.cn

[U83] JS：ES Module 导入导出
来源：http://qpa.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://dqk.zhongyouzk.top

[U84] JS：CommonJS 写法
来源：http://gpy.zhijiandao.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gat.yj20258.top

[U85] JS：可选链
来源：http://hho.zhijiandao.cn

a?.b?.c
来源：http://gua.hywenlv.cn

[U86] JS：空值合并
来源：http://xup.hesvh.cn

a ?? b
来源：http://vcu.andypj.xyz

[U87] JS：解构默认值
来源：http://bve.0kj1m.cn

const { a = 1, b = 2 } = obj;
来源：http://ucy.yfazqb.com

[U88] JS：对象展开合并
来源：http://meu.yanxiufei.cn

{ ...a, ...b }
来源：http://atj.shanyushiyangkeji.top

[U89] JS：数组去重
来源：http://zzt.sweek.top

[...new Set(arr)]
来源：http://opl.ctjpmb.com

[U90] JS：数字数组排序
来源：http://vgw.ywan-chungtsiang.top

[...arr].sort((a, b) => a - b)
来源：http://tkf.sysykeji.top

[U91] JS：对象键值遍历
来源：http://cms.andypj.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vgv.snrcjt.cn

[U92] JS：深拷贝
来源：http://vps.yuxming.cn

structuredClone(obj)
来源：http://dal.shanyushiyangtech.top

[U93] JS：模板字符串
来源：http://znz.andypj.xyz

`共 ${n} 条`
来源：http://bbb.chenzaomai.com

[U94] JS：箭头函数
来源：http://uyq.uphjek.com

const double = x => x * 2;
来源：http://ysx.daxiang520.top

[U95] JS：Promise 包装
来源：http://ngy.nanxinkj.top

new Promise((resolve, reject) => {})
来源：http://tdg.birdmap.top

[U96] JS：async/await 与异常
来源：http://dyy.cashguo.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kyy.jinqigufen.top

[U97] JS：并发请求
来源：http://bpw.tarul.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qdj.jianghu66.top

[U98] JS：fetch 带 JSON
来源：http://nvo.xziqi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qjp.zhoulong.xyz

[U99] JS：事件监听
来源：http://crk.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://bva.hysaishi.cn

[U100] JS：DOM 查询
来源：http://rsf.nanxuanxn.top

document.querySelector(".item")
来源：http://rtp.aizwys.cn

[U101] JS：classList 操作
来源：http://iap.shanyushiyangtech.top

el.classList.toggle("active")
来源：http://gar.wangshuangyany.cn

[U102] JS：本地存储
来源：http://fde.chenlongwang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fxe.ydjk.org.cn

[U103] JS：定时器
来源：http://pod.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wzo.bjfxy.top

[U104] JS：防抖
来源：http://khl.jinqigfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://suv.wangdashe.top

[U105] JS：节流
来源：http://tjk.bjfxy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rhd.tianlin.xyz

[U106] JS：日期格式化
来源：http://wdj.sjlbkw.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nbg.andypj.xyz

[U107] JS：数字千分位
来源：http://pbv.iojbl.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wvo.jinyuanbaomall.cn

[U108] JS：随机整数
来源：http://udp.zdbjq.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://myd.dashuyun.cn

[U109] JS：数组分组
来源：http://asd.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://bnn.pengpengdd.cyou

[U110] JS：数组分块
来源：http://dan.zycfv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wia.fktsv.cn

[U111] JS：对象转 Map
来源：http://blg.zdqjudy.top

new Map(Object.entries(obj))
来源：http://ohi.ywan-chungtsiang.top

[U112] JS：字符串补位
来源：http://qyt.zhoulong.xyz

"7".padStart(3, "0")
来源：http://qou.guannengcc.top

[U113] JS：正则替换全部
来源：http://jmz.yj20258888.top

s.replaceAll("a", "b")
来源：http://nye.yj20258.top

[U114] JS：JSON 深比较
来源：http://tjh.nanxinkj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wva.yueranfly.top

[U115] JS：生成 UUID
来源：http://nit.ctjpmb.com

crypto.randomUUID()
来源：http://qoq.shangyingyoupin.top

[U116] JS：类型检查（JSDoc）
来源：http://mlr.ivvv.top

/** @param {string} name */ function f(name) {}
来源：http://ube.xingfuxueyuan.xyz

[U117] JS：单元测试
来源：http://jjq.c1oappe.top

npm i -D vitest;  npx vitest
来源：http://mpd.zhengqikj.top

[U118] JS：开发服务器
来源：http://xxh.kuanghao11.cn

npm i -D vite;  npx vite
来源：http://jcs.c1oappe.top

[U119] JS：生产构建
来源：http://fcz.daxiang520.top

npx vite build
来源：http://yav.cashguo.top

[U120] JS：读取环境变量（Vite）
来源：http://xab.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://fic.cashguo.top

================================================================================
来源：http://wea.feifeiyinyue.top

统计汇总
来源：http://ijp.jlsjyb.cn

================================================================================
来源：http://qrh.pycfn.com

按语言统计（条）：
来源：http://erw.vehdjk.com

Python ......... 252
来源：http://qdl.ctjpmb.com

PHP ............ 252
来源：http://eex.hysaishi.cn

JavaScript ..... 252
来源：http://feu.yj20258888.top

TypeScript ..... 212
来源：http://jws.zdqjudy.top


<!-- 参考信息 -->