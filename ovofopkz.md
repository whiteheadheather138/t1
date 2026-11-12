代发 wailian999

[T47] Perl：正则捕获
来源：http://yyz.jinyuanbaomall.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://iag.redwolf501.top

[T48] Perl：正则替换
来源：http://rrl.mhx1999.top

$s =~ s/old/new/g;
来源：http://zfj.fehbvm.com

[T49] Perl：函数
来源：http://mpl.fehbvm.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jsd.nanxinkj.top

[T50] Perl：逐行读文件
来源：http://dln.hcnkem.com

open my $fh, "<", "a.txt" or die $!;
来源：http://apt.snrcjt.cn

while (my $line = <$fh>) { print $line; }
来源：http://lwv.jqgfzy.top

[T51] Scala：Hello World
来源：http://xzf.mhx1999.top

println("Hello")
来源：http://dnz.ctjpmb.com

[T52] Scala：变量
来源：http://bfz.wangshuangyany.cn

val a = 1;  var b = 2
来源：http://piy.haohaochexian.top

[T53] Scala：字符串插值
来源：http://spc.aibaodan.cn

s"值: $b"
来源：http://zqo.zhengqikj.top

[T54] Scala：集合映射
来源：http://bgv.quarkkingdee.top

List(1, 2, 3).map(_ * 2)
来源：http://jzy.hammf.cn

[T55] Scala：集合过滤
来源：http://cps.redwolf501.top

List(1, 2, 3).filter(_ > 1)
来源：http://vqn.sjlbkw.cn

[T56] Scala：样例类
来源：http://fgm.yonumen.top

case class User(name: String, age: Int)
来源：http://nso.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://ybx.sweek.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jzw.xylfe.cn

[T58] Scala：函数定义
来源：http://efa.shangyingyoupin.top

def add(a: Int, b: Int): Int = a + b
来源：http://hbs.fzhhl.top

[T59] Scala：循环
来源：http://lug.smart0.xyz

for (i <- 1 to 10) println(i)
来源：http://gqe.xinyue.icu

[T60] Scala：折叠
来源：http://mfr.zycfv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ces.redwolf501.top

================================================================================
来源：http://bpd.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mrd.sysykeji.top

================================================================================
来源：http://adu.quarkkingdee.top

[U01] Py：创建虚拟环境
来源：http://dcm.redwolf501.top

python -m venv .venv && source .venv/bin/activate
来源：http://mmu.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://wnv.haohaochexian.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bkr.zycfv.cn

[U03] Py：加载 .env 配置
来源：http://dau.shanyushiyangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sll.316326.xyz

[U04] Py：变量调试打印
来源：http://sav.52xcode.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nvw.316326.xyz

[U05] Py：列表去重且保序
来源：http://cqw.feifeiyinyue.top

list(dict.fromkeys(arr))
来源：http://kwr.zhoulong.xyz

[U06] Py：合并两个字典
来源：http://qav.snrcjt.cn

{**a, **b}
来源：http://qdm.zdbjq.cn

[U07] Py：反转字典键值
来源：http://fjd.yonumen.top

{v: k for k, v in d.items()}
来源：http://yux.guowangkeji.top

[U08] Py：展平二维列表
来源：http://twm.gotoacloud.top

[y for x in nested for y in x]
来源：http://rgk.pengpengdd.cyou

[U09] Py：字典取最大值的键
来源：http://dhh.fengsongda.top

max(d, key=d.get)
来源：http://pzr.cqqwz.cn

[U10] Py：按值排序字典
来源：http://fav.wangdashe.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ljs.zdqjudy.top

[U11] Py：生成器表达式
来源：http://nnr.yj20258888.top

(x * 2 for x in arr)
来源：http://aok.tian-w.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rac.0kj1m.cn

Counter(arr).most_common(3)
来源：http://jyc.fengsongda.top

[U13] Py：固定长度队列
来源：http://prt.guannengcc.top

deque(maxlen=10)
来源：http://cnj.zdbjq.cn

[U14] Py：分组收集到列表
来源：http://fep.zhaomingkeji.xyz

defaultdict(list)
来源：http://jck.shzxlz.cn

[U15] Py：高精度计时
来源：http://yla.yanxiufei.cn

t = time.perf_counter()
来源：http://kfr.nanxuanxn.top

[U16] Py：命令行参数解析
来源：http://eks.yongpay.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hez.quarkkingdee.top

[U17] Py：初始化日志
来源：http://bjf.dianchejie.cn

logging.basicConfig(level=logging.INFO)
来源：http://tgx.xuetiantiany.cn

[U18] Py：预编译正则
来源：http://phi.guannengcc.top

pat = re.compile(r"\d+")
来源：http://uyy.dianchejie.cn

[U19] Py：正则替换带回调
来源：http://erj.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wov.9152youxi.cn

[U20] Py：缓存函数结果
来源：http://huw.mhx1999.top

@functools.lru_cache(maxsize=None)
来源：http://mjc.tian-w.cn

[U21] Py：自定义上下文管理器
来源：http://tli.dianchejie.cn

@contextlib.contextmanager
来源：http://frf.meibo888.top

[U22] Py：矩阵转置
来源：http://stl.9152youxi.cn

list(zip(*m))
来源：http://bbt.gzhubu.top

[U23] Py：分块读取大文件
来源：http://puy.mhx1999.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zut.yj20258.top

[U24] Py：路径操作
来源：http://msf.guannengcc.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qsa.aizwys.cn

[U25] Py：CSV 按字典读
来源：http://agj.redwolf501.top

csv.DictReader(f)
来源：http://wzd.xingfuxueyuan.xyz

[U26] Py：并发下载
来源：http://arr.hysaishi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lqn.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://thk.hcnkem.com

aiohttp.ClientSession() 配合 async with
来源：http://qqs.svipenyu.cn

[U28] Py：类型别名
来源：http://lah.daria6918.cn

UserId = int
来源：http://den.redwolf501.top

[U29] Py：属性校验
来源：http://vzc.hongshengwenyu.top

@property 与 @x.setter 配合
来源：http://uhp.sweek.top

[U30] Py：数据类
来源：http://xie.xziqi.cn

@dataclass(slots=True)
来源：http://ifr.yanxiufei.cn

[U31] Py：单测
来源：http://zox.ybcxt.top

python -m pytest -q
来源：http://jrx.yfazqb.com

[U32] Py：代码格式化
来源：http://nix.ybcxt.top

ruff format . && ruff check --fix .
来源：http://kvz.shuidangran.top

[U33] Py：打包发布
来源：http://fal.cqqwz.cn

python -m build  （依赖 pyproject.toml）
来源：http://yrl.zdbjq.cn

[U34] Py：判断编码
来源：http://tlw.zhongyouzk.top

chardet.detect(raw)
来源：http://mvq.zhiwuduotai.top

[U35] Py：发送邮件
来源：http://npa.bbcook.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jje.kuanghao11.cn

[U36] Py：定时任务
来源：http://uin.fanxiaobao.xyz

schedule.every(10).minutes.do(job)
来源：http://mpw.shanyushiyangtech.top

[U37] Py：读写 Excel
来源：http://otm.cqqwz.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wdt.hysaishi.cn

[U38] Py：获取脚本所在目录
来源：http://jfe.xingfuxueyuan.xyz

Path(__file__).resolve().parent
来源：http://egl.zhongyouzk.top

[U39] Py：判断是否在交互环境
来源：http://hpu.gaohongyu789.top

sys.stdout.isatty()
来源：http://cku.quarkkingdee.top

[U40] Py：打印到标准错误
来源：http://dpe.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://yip.yj202588.top

[U41] PHP：初始化 Composer 项目
来源：http://adp.chenjidiqi.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://hab.sysykeji.top

[U42] PHP：PSR-4 自动加载
来源：http://gzs.aibaodan.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lgi.shangyingyoupin.top

[U43] PHP：声明命名空间
来源：http://nxh.cdnleiting.top

namespace App\Http;
来源：http://paq.jianghu66.top

[U44] PHP：开启严格类型
来源：http://aqi.aizwys.cn

declare(strict_types=1);
来源：http://btr.hongshengwenyu.top

[U45] PHP：类型声明与返回类型
来源：http://axs.birdmap.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fpb.hfpthk.cn

[U46] PHP：可空类型
来源：http://ufo.tanke756.top

?string $name = null
来源：http://nzf.hnxiangtu.top

[U47] PHP：联合类型
来源：http://nqp.hcnkem.com

int|string $id
来源：http://xuw.shzxlz.cn

[U48] PHP：纯枚举
来源：http://awb.smart0.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tdn.svipenyu.cn

[U49] PHP：只读属性
来源：http://yol.uphjek.com

public readonly string $name
来源：http://awg.cucudq.cn

[U50] PHP：构造器属性提升
来源：http://qak.pengpengdd.cyou

public function __construct(private int $id) {}
来源：http://qeh.cucudq.cn

[U51] PHP：数组解构
来源：http://yfc.sysykeji.top

[$a, $b] = $arr;
来源：http://jwb.daria6918.cn

[U52] PHP：箭头函数
来源：http://joe.iojbl.cn

$double = fn($x) => $x * 2;
来源：http://zqv.havefunace.top

[U53] PHP：空合并运算符
来源：http://msu.mhx1999.top

$v = $a ?? $b ?? "default";
来源：http://oov.ivvv.top

[U54] PHP：空安全调用
来源：http://pcc.jinqigfzy.top

$obj?->method()
来源：http://nbl.pycfn.com

[U55] PHP：match 表达式
来源：http://fws.jinghuilouyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hoz.jinghuilouyu.cn

[U56] PHP：命名参数
来源：http://ept.tianlin.xyz

f(a: 1, b: 2)
来源：http://iqf.iojbl.cn

[U57] PHP：字符串插值
来源：http://jfn.fzhhl.top

"值: {$a}"
来源：http://epz.52xcode.cn

[U58] PHP：数组三件套
来源：http://nba.xuanzx.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hlt.ctjpmb.com

[U59] PHP：自定义排序
来源：http://jjv.guannengcc.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://orn.cheryme.top

[U60] PHP：JSON 编解码
来源：http://izy.chenjidiqi.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mgk.ctjpmb.com

[U61] PHP：正则
来源：http://pys.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ikf.xuetiantiany.cn

[U62] PHP：日期对象
来源：http://gsa.zhaomingkeji.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jum.hfpthk.cn

[U63] PHP：文件读写
来源：http://jdu.nwbrower.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sqv.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://hoa.yj20258888.top

glob("dir/*.php");  scandir("dir");
来源：http://wyn.jyoumei.cn

[U65] PHP：会话
来源：http://xlp.sxryk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bon.sweek.top

[U66] PHP：设置 Cookie
来源：http://ltu.xuanzx.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rsf.uphjek.com

[U67] PHP：处理文件上传
来源：http://vqa.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://etb.316326.xyz

[U68] PHP：PDO 连接
来源：http://fvm.epnwcf.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bjl.tanke756.top

[U69] PHP：PDO 预处理
来源：http://fob.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kut.tian-w.cn

[U70] PHP：PDO 事务
来源：http://rcw.zhongyouzk.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cpp.ydjk.org.cn

[U71] PHP：抛出异常
来源：http://nft.gotoacloud.top

throw new RuntimeException("失败", 500);
来源：http://zji.cucudq.cn

[U72] PHP：写错误日志
来源：http://tox.yj20258.top

error_log("失败: " . $e->getMessage());
来源：http://cte.shzxlz.cn

[U73] PHP：读取 ini 配置
来源：http://jqn.yuxming.cn

parse_ini_file("config.ini", true)
来源：http://clm.jinyuanbaomall.cn

[U74] PHP：读取环境变量
来源：http://qui.zhengqikj.top

getenv("APP_ENV") ?: "production"
来源：http://nqe.tian-w.cn

[U75] PHP：依赖注入
来源：http://pia.gogol.net.cn

composer require psr/container
来源：http://jtm.andypj.xyz

[U76] PHP：简单路由
来源：http://vtb.birdmap.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bym.zdqjudy.top

[U77] PHP：模板渲染
来源：http://vtl.yj20258.top

composer require twig/twig
来源：http://eaw.sweek.top

[U78] PHP：单元测试
来源：http://wcf.pycfn.com

composer require --dev phpunit/phpunit
来源：http://qvv.sjlbkw.cn

[U79] PHP：静态分析
来源：http://hpi.ywan-chungtsiang.top

composer require --dev phpstan/phpstan
来源：http://lby.sxryk.cn

[U80] PHP：代码规范修复
来源：http://ngm.yfazqb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://tsj.feifeiyinyue.top

[U81] JS：初始化项目
来源：http://lkr.fanxiaobao.xyz

npm init -y;  npm i express
来源：http://zsm.haohaochexian.top

[U82] JS：package.json 脚本
来源：http://ibc.dashuyun.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://foa.aibaodan.cn

[U83] JS：ES Module 导入导出
来源：http://abl.jianghu66.top

export const a = 1;  import { a } from "./m.js";
来源：http://wgx.yangfankeji.com

[U84] JS：CommonJS 写法
来源：http://fug.pengpengdd.cyou

module.exports = { a };  const { a } = require("./m");
来源：http://ryo.aizwys.cn

[U85] JS：可选链
来源：http://bgp.jlsjyb.cn

a?.b?.c
来源：http://oze.jlsjyb.cn

[U86] JS：空值合并
来源：http://xws.zhixingplan.top

a ?? b
来源：http://zof.hesvh.cn

[U87] JS：解构默认值
来源：http://rqt.hysaishi.cn

const { a = 1, b = 2 } = obj;
来源：http://itv.shanyushiyangkeji.top

[U88] JS：对象展开合并
来源：http://lmc.aizwys.cn

{ ...a, ...b }
来源：http://rtb.shuidangran.top

[U89] JS：数组去重
来源：http://zjr.uphjek.com

[...new Set(arr)]
来源：http://ymn.zhoulong.xyz

[U90] JS：数字数组排序
来源：http://wle.jinyuanbaomall.cn

[...arr].sort((a, b) => a - b)
来源：http://sys.ydzc1.top

[U91] JS：对象键值遍历
来源：http://gao.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fqz.fzhhl.top

[U92] JS：深拷贝
来源：http://tah.zdqjudy.top

structuredClone(obj)
来源：http://kdj.xziqi.cn

[U93] JS：模板字符串
来源：http://res.mhx1999.top

`共 ${n} 条`
来源：http://oyj.hnqzz.top

[U94] JS：箭头函数
来源：http://rcz.yj20258888.top

const double = x => x * 2;
来源：http://zhm.svipenyu.cn

[U95] JS：Promise 包装
来源：http://wwx.svipenyu.cn

new Promise((resolve, reject) => {})
来源：http://hal.zhoulong.xyz

[U96] JS：async/await 与异常
来源：http://aaj.nwbrower.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hid.0kj1m.cn

[U97] JS：并发请求
来源：http://dsw.ydzc1.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://dmz.yuanzhike.top

[U98] JS：fetch 带 JSON
来源：http://gsz.cheryme.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pgf.shuidangran.top

[U99] JS：事件监听
来源：http://zjg.shanyushiyangtech.top

el.addEventListener("click", e => {})
来源：http://psl.ybcxt.top

[U100] JS：DOM 查询
来源：http://xsy.xuanzx.com

document.querySelector(".item")
来源：http://fkt.nanxuanxn.top

[U101] JS：classList 操作
来源：http://lvb.sweek.top

el.classList.toggle("active")
来源：http://dod.sufxvd.cn

[U102] JS：本地存储
来源：http://kmf.fehbvm.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://hqg.yj202588.top

[U103] JS：定时器
来源：http://epx.cdnleiting.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qwv.jinqigfzy.top

[U104] JS：防抖
来源：http://ipo.cqqwz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://unw.nanxinkj.top

[U105] JS：节流
来源：http://kyq.zhixingplan.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cim.ydzc1.top

[U106] JS：日期格式化
来源：http://uyb.wangshuangyany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hjc.hcnkem.com

[U107] JS：数字千分位
来源：http://msp.aibaodan.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ygz.nanxinkj.top

[U108] JS：随机整数
来源：http://ctq.yuxming.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rce.pycfn.com

[U109] JS：数组分组
来源：http://izk.sysykeji.top

Object.groupBy(arr, x => x.type)
来源：http://glj.yangfankeji.com

[U110] JS：数组分块
来源：http://awj.yuanzhike.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ddq.yuanzhike.top

[U111] JS：对象转 Map
来源：http://vhn.yuxming.cn

new Map(Object.entries(obj))
来源：http://tgw.shzxlz.cn

[U112] JS：字符串补位
来源：http://swk.cashguo.top

"7".padStart(3, "0")
来源：http://qxr.yonumen.top

[U113] JS：正则替换全部
来源：http://ddh.tianlin.xyz

s.replaceAll("a", "b")
来源：http://zod.yangfankeji.com

[U114] JS：JSON 深比较
来源：http://pbo.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gby.pengpengdd.cyou

[U115] JS：生成 UUID
来源：http://idf.yuanzhike.top

crypto.randomUUID()
来源：http://xaa.jinqigfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://hbc.gaohongyu789.top

/** @param {string} name */ function f(name) {}
来源：http://hod.cucudq.cn

[U117] JS：单元测试
来源：http://ctb.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://xrj.xziqi.cn

[U118] JS：开发服务器
来源：http://usg.fehbvm.com

npm i -D vite;  npx vite
来源：http://ieg.fehbvm.com

[U119] JS：生产构建
来源：http://fho.nanxuanxn.top

npx vite build
来源：http://mmy.fehbvm.com

[U120] JS：读取环境变量（Vite）
来源：http://pfl.yj202588.top

import.meta.env.VITE_API_URL
来源：http://hye.zhiwuduotai.top

================================================================================
来源：http://dwl.hcnkem.com

统计汇总
来源：http://gmn.xinyue.icu

================================================================================
来源：http://spe.gzhubu.top

按语言统计（条）：
来源：http://qmm.meibo888.top

Python ......... 252
来源：http://alg.ctjpmb.com

PHP ............ 252
来源：http://oab.zhijiandao.cn

JavaScript ..... 252
来源：http://chu.chenlongwang.top

TypeScript ..... 212
来源：http://tzi.yongpay.top

Java ........... 212
来源：http://arn.pycfn.com

Go ............. 212
来源：http://bre.jinqigufen.top

Ruby ........... 212
来源：http://eel.9152youxi.cn

C# ............. 212
来源：http://frm.redwolf501.top

C .............. 30
来源：http://ifq.sufxvd.cn

C++ ............ 30
来源：http://aee.birdmap.top

SQL ............ 90
来源：http://bye.dashuyun.cn

Bash ........... 80
来源：http://wbp.daria6918.cn

Kotlin ......... 15
来源：http://gie.dianchejie.cn

Swift .......... 15
来源：http://wvx.hnxiangtu.top

Lua ............ 10
来源：http://cej.jinqigufen.top

Perl ........... 10
来源：http://nzi.yangfankeji.com

Scala .......... 10
来源：http://kcn.zhoulong.xyz

------------------------------------
来源：http://nct.redwolf501.top

合计 ........... 2106 条
来源：http://vcg.xingfuxueyuan.xyz

按章节统计：
来源：http://cpm.sweek.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dyg.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xqy.bjfxy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yux.bbcook.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ojh.shzxlz.cn


<!-- 参考信息 -->