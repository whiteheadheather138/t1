代发 wailian999

[T41] Perl：Hello World
来源：http://myo.fanxiaobao.xyz

print "Hello\n";
来源：http://bpg.bjfxy.top

[T42] Perl：变量类型
来源：http://smc.pycfn.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fky.9152youxi.cn

[T43] Perl：字符串插值
来源：http://gmv.9152youxi.cn

"值: $a"
来源：http://wwb.ydzc1.top

[T44] Perl：条件
来源：http://xor.smart0.xyz

if ($a > 0) { print "正"; }
来源：http://veo.aizwys.cn

[T45] Perl：数组遍历
来源：http://zfi.shzxlz.cn

for my $x (@arr) { print $x; }
来源：http://jga.yueranfly.top

[T46] Perl：哈希操作
来源：http://dvw.sysykeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://txc.52xcode.cn

[T47] Perl：正则捕获
来源：http://lrd.zhongyouzk.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://sbh.redwolf501.top

[T48] Perl：正则替换
来源：http://ljm.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://rlr.316326.xyz

[T49] Perl：函数
来源：http://oos.gzhubu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vaq.jiagoushi.top

[T50] Perl：逐行读文件
来源：http://vjo.zhengqikj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://cir.meibo888.top

while (my $line = <$fh>) { print $line; }
来源：http://krw.chenjidiqi.icu

[T51] Scala：Hello World
来源：http://tzr.feifeiyinyue.top

println("Hello")
来源：http://ynn.yj20258888.top

[T52] Scala：变量
来源：http://cog.pycfn.com

val a = 1;  var b = 2
来源：http://cvo.zhiwuduotai.top

[T53] Scala：字符串插值
来源：http://vdj.52xcode.cn

s"值: $b"
来源：http://los.xylfe.cn

[T54] Scala：集合映射
来源：http://xbg.ctjpmb.com

List(1, 2, 3).map(_ * 2)
来源：http://tfx.pengpengdd.cyou

[T55] Scala：集合过滤
来源：http://nwz.yj202588.top

List(1, 2, 3).filter(_ > 1)
来源：http://nfs.jqgufenzy.top

[T56] Scala：样例类
来源：http://xms.fktsv.cn

case class User(name: String, age: Int)
来源：http://cxi.daria6918.cn

[T57] Scala：模式匹配
来源：http://adx.aizwys.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rfb.zhoulong.xyz

[T58] Scala：函数定义
来源：http://uzt.ivvv.top

def add(a: Int, b: Int): Int = a + b
来源：http://try.guannengcc.top

[T59] Scala：循环
来源：http://wbz.zhengqikj.top

for (i <- 1 to 10) println(i)
来源：http://wlq.meibo888.top

[T60] Scala：折叠
来源：http://zpr.jinqigfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ysi.yonumen.top

================================================================================
来源：http://ara.gaohongyu789.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mya.aibaodan.cn

================================================================================
来源：http://fcf.zycfv.cn

[U01] Py：创建虚拟环境
来源：http://cnc.hfpthk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fap.yonumen.top

[U02] Py：导出 / 安装依赖
来源：http://nwn.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dsb.shangyingyoupin.top

[U03] Py：加载 .env 配置
来源：http://aoj.hammf.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hfo.xinyue.icu

[U04] Py：变量调试打印
来源：http://ihf.jqgufenzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://otz.fanxiaobao.xyz

[U05] Py：列表去重且保序
来源：http://gch.dianchejie.cn

list(dict.fromkeys(arr))
来源：http://irq.cashguo.top

[U06] Py：合并两个字典
来源：http://bua.shuidangran.top

{**a, **b}
来源：http://nfv.jiagoushi.top

[U07] Py：反转字典键值
来源：http://ibc.9152youxi.cn

{v: k for k, v in d.items()}
来源：http://wzf.fanxiaobao.xyz

[U08] Py：展平二维列表
来源：http://dym.fktsv.cn

[y for x in nested for y in x]
来源：http://gsm.ehwqpu.com

[U09] Py：字典取最大值的键
来源：http://zcd.tarul.cn

max(d, key=d.get)
来源：http://joc.zhoulong.xyz

[U10] Py：按值排序字典
来源：http://kzb.yuxming.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aya.fktsv.cn

[U11] Py：生成器表达式
来源：http://jhr.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://upd.gzhubu.top

[U12] Py：取出现最多的 3 个元素
来源：http://ert.xziqi.cn

Counter(arr).most_common(3)
来源：http://daz.0kj1m.cn

[U13] Py：固定长度队列
来源：http://tdx.chenlongwang.top

deque(maxlen=10)
来源：http://jek.jianghu66.top

[U14] Py：分组收集到列表
来源：http://vep.meibo888.top

defaultdict(list)
来源：http://ayh.fktsv.cn

[U15] Py：高精度计时
来源：http://eft.mhx1999.top

t = time.perf_counter()
来源：http://kxf.xingfuxueyuan.xyz

[U16] Py：命令行参数解析
来源：http://zgj.zhengqikj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pzj.nwbrower.top

[U17] Py：初始化日志
来源：http://swt.zdbjq.cn

logging.basicConfig(level=logging.INFO)
来源：http://ary.yvedp.cn

[U18] Py：预编译正则
来源：http://dcb.ivvv.top

pat = re.compile(r"\d+")
来源：http://eqg.0kj1m.cn

[U19] Py：正则替换带回调
来源：http://woa.cheryme.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gfj.yj20258.top

[U20] Py：缓存函数结果
来源：http://rhr.zdbjq.cn

@functools.lru_cache(maxsize=None)
来源：http://zce.cashguo.top

[U21] Py：自定义上下文管理器
来源：http://hra.tian-w.cn

@contextlib.contextmanager
来源：http://xsq.shanyushiyangtech.top

[U22] Py：矩阵转置
来源：http://kez.fehbvm.com

list(zip(*m))
来源：http://gst.quarkkingdee.top

[U23] Py：分块读取大文件
来源：http://tog.shanyushiyangtech.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dax.yfazqb.com

[U24] Py：路径操作
来源：http://qrx.yj202588.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dro.ehwqpu.com

[U25] Py：CSV 按字典读
来源：http://lep.sxryk.cn

csv.DictReader(f)
来源：http://ybo.fehbvm.com

[U26] Py：并发下载
来源：http://qys.shuidangran.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://san.shanyushiyangkeji.top

[U27] Py：异步 HTTP
来源：http://vxm.xuanzx.com

aiohttp.ClientSession() 配合 async with
来源：http://icw.vehdjk.com

[U28] Py：类型别名
来源：http://aac.ydjk.org.cn

UserId = int
来源：http://ien.chenjidiqi.icu

[U29] Py：属性校验
来源：http://qik.xuanzx.com

@property 与 @x.setter 配合
来源：http://omg.yvedp.cn

[U30] Py：数据类
来源：http://zmh.cheryme.top

@dataclass(slots=True)
来源：http://kfi.yj20258888.top

[U31] Py：单测
来源：http://ozx.tarul.cn

python -m pytest -q
来源：http://law.ctjpmb.com

[U32] Py：代码格式化
来源：http://nsu.daxiang520.top

ruff format . && ruff check --fix .
来源：http://gte.meibo888.top

[U33] Py：打包发布
来源：http://izj.hnxiangtu.top

python -m build  （依赖 pyproject.toml）
来源：http://dan.cheryme.top

[U34] Py：判断编码
来源：http://ibd.zhoulong.xyz

chardet.detect(raw)
来源：http://eno.jianghu66.top

[U35] Py：发送邮件
来源：http://qyw.sweek.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://epx.andypj.xyz

[U36] Py：定时任务
来源：http://tga.gzhubu.top

schedule.every(10).minutes.do(job)
来源：http://sqc.gotoacloud.top

[U37] Py：读写 Excel
来源：http://qws.xylfe.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kqa.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://lnp.gzhubu.top

Path(__file__).resolve().parent
来源：http://bdl.xuetiantiany.cn

[U39] Py：判断是否在交互环境
来源：http://kkj.xuetiantiany.cn

sys.stdout.isatty()
来源：http://dhk.xinyue.icu

[U40] Py：打印到标准错误
来源：http://pms.sjlbkw.cn

print("err", file=sys.stderr)
来源：http://dty.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://njm.ehwqpu.com

composer init;  composer require guzzlehttp/guzzle
来源：http://byx.epnwcf.com

[U42] PHP：PSR-4 自动加载
来源：http://gzt.ppjwa.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pnl.nanxuanxn.top

[U43] PHP：声明命名空间
来源：http://iez.ehwqpu.com

namespace App\Http;
来源：http://rlq.fengsongda.top

[U44] PHP：开启严格类型
来源：http://ykc.havefunace.top

declare(strict_types=1);
来源：http://bvs.tian-w.cn

[U45] PHP：类型声明与返回类型
来源：http://cuj.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uwo.xinyue.icu

[U46] PHP：可空类型
来源：http://hat.xingfuxueyuan.xyz

?string $name = null
来源：http://cbd.zhoulong.xyz

[U47] PHP：联合类型
来源：http://ezh.sufxvd.cn

int|string $id
来源：http://hqo.daria6918.cn

[U48] PHP：纯枚举
来源：http://pbw.ctjpmb.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oyz.vqdsnc.cn

[U49] PHP：只读属性
来源：http://otf.kuanghao11.cn

public readonly string $name
来源：http://jwg.aizwys.cn

[U50] PHP：构造器属性提升
来源：http://nfm.snrcjt.cn

public function __construct(private int $id) {}
来源：http://pqo.gotoacloud.top

[U51] PHP：数组解构
来源：http://hca.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://joc.mhx1999.top

[U52] PHP：箭头函数
来源：http://kgn.hesvh.cn

$double = fn($x) => $x * 2;
来源：http://csh.jlsjyb.cn

[U53] PHP：空合并运算符
来源：http://gws.zhengqikj.top

$v = $a ?? $b ?? "default";
来源：http://owf.sweek.top

[U54] PHP：空安全调用
来源：http://acj.shuidangran.top

$obj?->method()
来源：http://yyj.zhaomingkeji.xyz

[U55] PHP：match 表达式
来源：http://hiz.iojbl.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uqg.sxryk.cn

[U56] PHP：命名参数
来源：http://lzm.iojbl.cn

f(a: 1, b: 2)
来源：http://sdv.epnwcf.com

[U57] PHP：字符串插值
来源：http://tbo.hesvh.cn

"值: {$a}"
来源：http://zzo.jinqigfzy.top

[U58] PHP：数组三件套
来源：http://tog.yanxiufei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tyw.fzhhl.top

[U59] PHP：自定义排序
来源：http://xbu.vehdjk.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tmj.zycfv.cn

[U60] PHP：JSON 编解码
来源：http://zbx.zhaomingkeji.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zje.hongshengwenyu.top

[U61] PHP：正则
来源：http://djl.shangyingyoupin.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xxa.0kj1m.cn

[U62] PHP：日期对象
来源：http://yvc.shanyushiyangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kom.nwbrower.top

[U63] PHP：文件读写
来源：http://plr.yuxming.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hvt.yangfankeji.com

[U64] PHP：目录遍历
来源：http://jqy.nanxuanxn.top

glob("dir/*.php");  scandir("dir");
来源：http://nei.pycfn.com

[U65] PHP：会话
来源：http://ott.cashguo.top

session_start();  $_SESSION["uid"] = 1;
来源：http://aoj.wangdashe.top

[U66] PHP：设置 Cookie
来源：http://ogs.xuanzx.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nsy.quarkkingdee.top

[U67] PHP：处理文件上传
来源：http://toc.hesvh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zya.iojbl.cn

[U68] PHP：PDO 连接
来源：http://tqu.jyoumei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ost.sweek.top

[U69] PHP：PDO 预处理
来源：http://bxe.tanke756.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bqe.cdnleiting.top

[U70] PHP：PDO 事务
来源：http://dxl.haohaochexian.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dxk.shzxlz.cn

[U71] PHP：抛出异常
来源：http://uar.aibaodan.cn

throw new RuntimeException("失败", 500);
来源：http://rgz.smart0.xyz

[U72] PHP：写错误日志
来源：http://ndo.zdqjudy.top

error_log("失败: " . $e->getMessage());
来源：http://anz.wangshuangyany.cn

[U73] PHP：读取 ini 配置
来源：http://rez.pycfn.com

parse_ini_file("config.ini", true)
来源：http://efp.jinqigufen.top

[U74] PHP：读取环境变量
来源：http://bou.52xcode.cn

getenv("APP_ENV") ?: "production"
来源：http://noh.vqdsnc.cn

[U75] PHP：依赖注入
来源：http://agg.zhixingplan.top

composer require psr/container
来源：http://bgy.mhx1999.top

[U76] PHP：简单路由
来源：http://sxc.zhaomingkeji.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://emj.fzhhl.top

[U77] PHP：模板渲染
来源：http://cji.svipenyu.cn

composer require twig/twig
来源：http://qql.hcnkem.com

[U78] PHP：单元测试
来源：http://nev.vqdsnc.cn

composer require --dev phpunit/phpunit
来源：http://qlz.jinqigufen.top

[U79] PHP：静态分析
来源：http://qhf.yj20258888.top

composer require --dev phpstan/phpstan
来源：http://gja.zycfv.cn

[U80] PHP：代码规范修复
来源：http://plf.hcnkem.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://vqt.gotoacloud.top

[U81] JS：初始化项目
来源：http://vze.tarul.cn

npm init -y;  npm i express
来源：http://jev.guannengcc.top

[U82] JS：package.json 脚本
来源：http://kfv.c1oappe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lwj.fengsongda.top

[U83] JS：ES Module 导入导出
来源：http://wjq.dashuyun.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pxz.svipenyu.cn

[U84] JS：CommonJS 写法
来源：http://hqa.wangshuangyany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tsn.cqqwz.cn

[U85] JS：可选链
来源：http://znl.wangdashe.top

a?.b?.c
来源：http://ftd.zhoulong.xyz

[U86] JS：空值合并
来源：http://jvl.daria6918.cn

a ?? b
来源：http://xxw.andypj.xyz

[U87] JS：解构默认值
来源：http://avd.ppjwa.cn

const { a = 1, b = 2 } = obj;
来源：http://ahp.guowangkeji.top

[U88] JS：对象展开合并
来源：http://bwd.zdqjudy.top

{ ...a, ...b }
来源：http://nnm.jianghu66.top

[U89] JS：数组去重
来源：http://abt.zdbjq.cn

[...new Set(arr)]
来源：http://rxa.52xcode.cn

[U90] JS：数字数组排序
来源：http://cgc.zhoulong.xyz

[...arr].sort((a, b) => a - b)
来源：http://tup.vqdsnc.cn

[U91] JS：对象键值遍历
来源：http://res.wangdashe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dgt.chenzaomai.com

[U92] JS：深拷贝
来源：http://ihc.vehdjk.com

structuredClone(obj)
来源：http://wlh.cucudq.cn

[U93] JS：模板字符串
来源：http://kxu.gaohongyu789.top

`共 ${n} 条`
来源：http://zsu.zhiwuduotai.top

[U94] JS：箭头函数
来源：http://bvg.yangfankeji.com

const double = x => x * 2;
来源：http://ent.xuanzx.com

[U95] JS：Promise 包装
来源：http://xes.cqqwz.cn

new Promise((resolve, reject) => {})
来源：http://vlm.52xcode.cn

[U96] JS：async/await 与异常
来源：http://ocb.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zdf.jqgfzy.top

[U97] JS：并发请求
来源：http://rbf.redwolf501.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vjt.svipenyu.cn

[U98] JS：fetch 带 JSON
来源：http://awj.zhongyouzk.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cxj.zdbjq.cn

[U99] JS：事件监听
来源：http://yvk.havefunace.top

el.addEventListener("click", e => {})
来源：http://rft.ydzc1.top

[U100] JS：DOM 查询
来源：http://bdm.hesvh.cn

document.querySelector(".item")
来源：http://rcz.cucudq.cn

[U101] JS：classList 操作
来源：http://lsu.wangshuangyany.cn

el.classList.toggle("active")
来源：http://rbv.fktsv.cn

[U102] JS：本地存储
来源：http://liu.9152youxi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://koa.dashuyun.cn

[U103] JS：定时器
来源：http://jqu.nanxuanxn.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tzs.yj20258.top

[U104] JS：防抖
来源：http://svn.cdnleiting.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uub.iojbl.cn

[U105] JS：节流
来源：http://rif.zhongyouzk.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fto.feifeiyinyue.top

[U106] JS：日期格式化
来源：http://mrn.zdqjudy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xvh.kuanghao11.cn

[U107] JS：数字千分位
来源：http://dco.nanxuanxn.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://juv.tanke756.top

[U108] JS：随机整数
来源：http://sdu.yfazqb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ect.fanxiaobao.xyz

[U109] JS：数组分组
来源：http://dba.chenlongwang.top

Object.groupBy(arr, x => x.type)
来源：http://fvd.ydzc1.top

[U110] JS：数组分块
来源：http://kez.tianlin.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jce.fktsv.cn

[U111] JS：对象转 Map
来源：http://zhc.hywenlv.cn

new Map(Object.entries(obj))
来源：http://vgr.shzxlz.cn

[U112] JS：字符串补位
来源：http://lov.hammf.cn

"7".padStart(3, "0")
来源：http://yrg.zhiwuduotai.top

[U113] JS：正则替换全部
来源：http://enh.hywenlv.cn

s.replaceAll("a", "b")
来源：http://eef.tianlin.xyz

[U114] JS：JSON 深比较
来源：http://vfd.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rfs.xylfe.cn

[U115] JS：生成 UUID
来源：http://god.yonumen.top

crypto.randomUUID()
来源：http://xdb.yanxiufei.cn

[U116] JS：类型检查（JSDoc）
来源：http://vxq.ppjwa.cn

/** @param {string} name */ function f(name) {}
来源：http://vlg.sjlbkw.cn

[U117] JS：单元测试
来源：http://bjs.fanxiaobao.xyz

npm i -D vitest;  npx vitest
来源：http://ptx.bbcook.cn

[U118] JS：开发服务器
来源：http://sbv.zhixingplan.top

npm i -D vite;  npx vite
来源：http://suq.52xcode.cn

[U119] JS：生产构建
来源：http://eyb.cucudq.cn

npx vite build
来源：http://ybn.zhiwuduotai.top

[U120] JS：读取环境变量（Vite）
来源：http://yfr.hammf.cn

import.meta.env.VITE_API_URL
来源：http://itt.quarkkingdee.top

================================================================================
来源：http://alt.dashuyun.cn

统计汇总
来源：http://xyq.shangyingyoupin.top

================================================================================
来源：http://pgz.hysaishi.cn

按语言统计（条）：
来源：http://kmi.hammf.cn

Python ......... 252
来源：http://hea.ydjk.org.cn

PHP ............ 252
来源：http://wjr.haohaochexian.top

JavaScript ..... 252
来源：http://csh.316326.xyz

TypeScript ..... 212
来源：http://bjr.ydjk.org.cn

Java ........... 212
来源：http://lwv.hywenlv.cn

Go ............. 212
来源：http://tka.yueranfly.top

Ruby ........... 212
来源：http://yzh.nanxinkj.top

C# ............. 212
来源：http://yyi.zdbjq.cn

C .............. 30
来源：http://dld.jinyuanbaomall.cn

C++ ............ 30
来源：http://vpm.yfazqb.com

SQL ............ 90
来源：http://pde.yueranfly.top

Bash ........... 80
来源：http://yxa.hammf.cn


<!-- 参考信息 -->