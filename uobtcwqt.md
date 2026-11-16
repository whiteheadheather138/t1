代发 wailian999

[T47] Perl：正则捕获
来源：http://ebc.gzhubu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bib.shuidangran.top

[T48] Perl：正则替换
来源：http://wxy.jiagoushi.top

$s =~ s/old/new/g;
来源：http://txn.vqdsnc.cn

[T49] Perl：函数
来源：http://xmt.pycfn.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fnw.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://hof.bbcook.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lpy.vehdjk.com

while (my $line = <$fh>) { print $line; }
来源：http://jcy.cashguo.top

[T51] Scala：Hello World
来源：http://pmo.hysaishi.cn

println("Hello")
来源：http://cdz.hesvh.cn

[T52] Scala：变量
来源：http://khf.yongpay.top

val a = 1;  var b = 2
来源：http://mnn.9152youxi.cn

[T53] Scala：字符串插值
来源：http://syk.gotoacloud.top

s"值: $b"
来源：http://tlp.smart0.xyz

[T54] Scala：集合映射
来源：http://pzm.gogol.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://gtk.hammf.cn

[T55] Scala：集合过滤
来源：http://ktz.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mqr.yanxiufei.cn

[T56] Scala：样例类
来源：http://ued.zhaomingkeji.xyz

case class User(name: String, age: Int)
来源：http://oxn.dianchejie.cn

[T57] Scala：模式匹配
来源：http://bdu.shuidangran.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hpr.hysaishi.cn

[T58] Scala：函数定义
来源：http://xoi.shzxlz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://irn.jyoumei.cn

[T59] Scala：循环
来源：http://mei.ydjk.org.cn

for (i <- 1 to 10) println(i)
来源：http://euj.andypj.xyz

[T60] Scala：折叠
来源：http://hcp.xylfe.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cjv.pengpengdd.cyou

================================================================================
来源：http://tnt.jqgufenzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://saj.jinghuilouyu.cn

================================================================================
来源：http://nia.yj20258.top

[U01] Py：创建虚拟环境
来源：http://jpb.bjfxy.top

python -m venv .venv && source .venv/bin/activate
来源：http://euw.zhoulong.xyz

[U02] Py：导出 / 安装依赖
来源：http://wmm.birdmap.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://axn.yuxming.cn

[U03] Py：加载 .env 配置
来源：http://twe.jinghuilouyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ssh.zhijiandao.cn

[U04] Py：变量调试打印
来源：http://ikn.meibo888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wps.xylfe.cn

[U05] Py：列表去重且保序
来源：http://rlh.zhengqikj.top

list(dict.fromkeys(arr))
来源：http://vah.zhixingplan.top

[U06] Py：合并两个字典
来源：http://lci.cucudq.cn

{**a, **b}
来源：http://ebs.iojbl.cn

[U07] Py：反转字典键值
来源：http://nrf.xinyue.icu

{v: k for k, v in d.items()}
来源：http://ord.zhiwuduotai.top

[U08] Py：展平二维列表
来源：http://nwh.xinyue.icu

[y for x in nested for y in x]
来源：http://dmx.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://fyr.cdnleiting.top

max(d, key=d.get)
来源：http://xms.fengsongda.top

[U10] Py：按值排序字典
来源：http://zfg.yonumen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rbw.xziqi.cn

[U11] Py：生成器表达式
来源：http://ndh.jinyuanbaomall.cn

(x * 2 for x in arr)
来源：http://mqw.jianghu66.top

[U12] Py：取出现最多的 3 个元素
来源：http://eyd.yongpay.top

Counter(arr).most_common(3)
来源：http://its.yonumen.top

[U13] Py：固定长度队列
来源：http://zxp.meibo888.top

deque(maxlen=10)
来源：http://nlt.daria6918.cn

[U14] Py：分组收集到列表
来源：http://hof.yuanzhike.top

defaultdict(list)
来源：http://xws.gzhubu.top

[U15] Py：高精度计时
来源：http://jdo.ybcxt.top

t = time.perf_counter()
来源：http://txi.cucudq.cn

[U16] Py：命令行参数解析
来源：http://crg.hnqzz.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pie.shuidangran.top

[U17] Py：初始化日志
来源：http://prq.yj20258.top

logging.basicConfig(level=logging.INFO)
来源：http://jux.316326.xyz

[U18] Py：预编译正则
来源：http://aoy.jqgufenzy.top

pat = re.compile(r"\d+")
来源：http://dcf.ydjk.org.cn

[U19] Py：正则替换带回调
来源：http://yto.wangdashe.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gna.birdmap.top

[U20] Py：缓存函数结果
来源：http://rcd.ydjk.org.cn

@functools.lru_cache(maxsize=None)
来源：http://nsl.gaohongyu789.top

[U21] Py：自定义上下文管理器
来源：http://vwi.hfpthk.cn

@contextlib.contextmanager
来源：http://jgx.epnwcf.com

[U22] Py：矩阵转置
来源：http://hyd.fehbvm.com

list(zip(*m))
来源：http://nnw.daxiang520.top

[U23] Py：分块读取大文件
来源：http://rwl.andypj.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lgb.jinghuilouyu.cn

[U24] Py：路径操作
来源：http://gkb.yuxming.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zrj.sxryk.cn

[U25] Py：CSV 按字典读
来源：http://vrq.chenjidiqi.icu

csv.DictReader(f)
来源：http://mkv.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://elm.nanxuanxn.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vpo.jiagoushi.top

[U27] Py：异步 HTTP
来源：http://ipq.quarkkingdee.top

aiohttp.ClientSession() 配合 async with
来源：http://dld.zdbjq.cn

[U28] Py：类型别名
来源：http://uuz.sweek.top

UserId = int
来源：http://pqs.hongshengwenyu.top

[U29] Py：属性校验
来源：http://zkz.0kj1m.cn

@property 与 @x.setter 配合
来源：http://kxb.svipenyu.cn

[U30] Py：数据类
来源：http://lnv.epnwcf.com

@dataclass(slots=True)
来源：http://ron.hongshengwenyu.top

[U31] Py：单测
来源：http://kng.vqdsnc.cn

python -m pytest -q
来源：http://osc.jiagoushi.top

[U32] Py：代码格式化
来源：http://pxo.pycfn.com

ruff format . && ruff check --fix .
来源：http://aww.vqdsnc.cn

[U33] Py：打包发布
来源：http://deg.nwbrower.top

python -m build  （依赖 pyproject.toml）
来源：http://xne.yanxiufei.cn

[U34] Py：判断编码
来源：http://fte.gzhubu.top

chardet.detect(raw)
来源：http://emj.yueranfly.top

[U35] Py：发送邮件
来源：http://qcq.0kj1m.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ooj.hfpthk.cn

[U36] Py：定时任务
来源：http://slz.fzhhl.top

schedule.every(10).minutes.do(job)
来源：http://mum.jinqigfzy.top

[U37] Py：读写 Excel
来源：http://aly.fanxiaobao.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://cfp.yonumen.top

[U38] Py：获取脚本所在目录
来源：http://zlg.meibo888.top

Path(__file__).resolve().parent
来源：http://zew.xuanzx.com

[U39] Py：判断是否在交互环境
来源：http://qbw.shanyushiyangkeji.top

sys.stdout.isatty()
来源：http://xkg.yonumen.top

[U40] Py：打印到标准错误
来源：http://kqt.pycfn.com

print("err", file=sys.stderr)
来源：http://ifv.jlsjyb.cn

[U41] PHP：初始化 Composer 项目
来源：http://xbx.andypj.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://spn.xuetiantiany.cn

[U42] PHP：PSR-4 自动加载
来源：http://kqn.zhoulong.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://azw.hammf.cn

[U43] PHP：声明命名空间
来源：http://ppy.jqgufenzy.top

namespace App\Http;
来源：http://ord.jianghu66.top

[U44] PHP：开启严格类型
来源：http://hst.sysykeji.top

declare(strict_types=1);
来源：http://yix.guowangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://qjq.andypj.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://ffc.xingfuxueyuan.xyz

[U46] PHP：可空类型
来源：http://bfn.smart0.xyz

?string $name = null
来源：http://gjd.jyoumei.cn

[U47] PHP：联合类型
来源：http://rnp.fengsongda.top

int|string $id
来源：http://yel.fengsongda.top

[U48] PHP：纯枚举
来源：http://xfn.zdbjq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gvj.0kj1m.cn

[U49] PHP：只读属性
来源：http://vpi.shanyushiyangtech.top

public readonly string $name
来源：http://cqq.chenzaomai.com

[U50] PHP：构造器属性提升
来源：http://wdq.zdbjq.cn

public function __construct(private int $id) {}
来源：http://ifg.andypj.xyz

[U51] PHP：数组解构
来源：http://zxt.bbcook.cn

[$a, $b] = $arr;
来源：http://mgj.ivvv.top

[U52] PHP：箭头函数
来源：http://drm.zhoulong.xyz

$double = fn($x) => $x * 2;
来源：http://jth.yongpay.top

[U53] PHP：空合并运算符
来源：http://let.yanxiufei.cn

$v = $a ?? $b ?? "default";
来源：http://gbk.yonumen.top

[U54] PHP：空安全调用
来源：http://uqr.zhengqikj.top

$obj?->method()
来源：http://zwd.yj20258888.top

[U55] PHP：match 表达式
来源：http://aax.pengpengdd.cyou

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lug.sjlbkw.cn

[U56] PHP：命名参数
来源：http://wop.shanyushiyangkeji.top

f(a: 1, b: 2)
来源：http://iel.cucudq.cn

[U57] PHP：字符串插值
来源：http://lbk.zdbjq.cn

"值: {$a}"
来源：http://yen.cheryme.top

[U58] PHP：数组三件套
来源：http://wuz.vehdjk.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kym.dashuyun.cn

[U59] PHP：自定义排序
来源：http://wrl.shanyushiyangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lxp.52xcode.cn

[U60] PHP：JSON 编解码
来源：http://cmd.zhiwuduotai.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xii.jiagoushi.top

[U61] PHP：正则
来源：http://cil.pycfn.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gnn.zdbjq.cn

[U62] PHP：日期对象
来源：http://vnc.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dhy.yueranfly.top

[U63] PHP：文件读写
来源：http://fck.c1oappe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nxp.hnqzz.top

[U64] PHP：目录遍历
来源：http://zuf.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://vrt.bjfxy.top

[U65] PHP：会话
来源：http://pqt.aibaodan.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qzm.snrcjt.cn

[U66] PHP：设置 Cookie
来源：http://eas.mhx1999.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kee.yueranfly.top

[U67] PHP：处理文件上传
来源：http://vca.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ugh.epnwcf.com

[U68] PHP：PDO 连接
来源：http://dkz.cashguo.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xgx.zhongyouzk.top

[U69] PHP：PDO 预处理
来源：http://lhb.uphjek.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pxr.jinqigufen.top

[U70] PHP：PDO 事务
来源：http://bqb.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mcw.iojbl.cn

[U71] PHP：抛出异常
来源：http://nil.xuetiantiany.cn

throw new RuntimeException("失败", 500);
来源：http://nex.zhiwuduotai.top

[U72] PHP：写错误日志
来源：http://ono.zycfv.cn

error_log("失败: " . $e->getMessage());
来源：http://lua.ehwqpu.com

[U73] PHP：读取 ini 配置
来源：http://sib.yvedp.cn

parse_ini_file("config.ini", true)
来源：http://jla.tanke756.top

[U74] PHP：读取环境变量
来源：http://tkg.sufxvd.cn

getenv("APP_ENV") ?: "production"
来源：http://cms.xingfuxueyuan.xyz

[U75] PHP：依赖注入
来源：http://mfv.tian-w.cn

composer require psr/container
来源：http://nit.9152youxi.cn

[U76] PHP：简单路由
来源：http://wvh.hcnkem.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qow.xuanzx.com

[U77] PHP：模板渲染
来源：http://wbp.zhijiandao.cn

composer require twig/twig
来源：http://tqa.hnqzz.top

[U78] PHP：单元测试
来源：http://evd.shzxlz.cn

composer require --dev phpunit/phpunit
来源：http://fld.cqqwz.cn

[U79] PHP：静态分析
来源：http://niy.cdnleiting.top

composer require --dev phpstan/phpstan
来源：http://ywe.zhaomingkeji.xyz

[U80] PHP：代码规范修复
来源：http://jdr.wangshuangyany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zxq.hywenlv.cn

[U81] JS：初始化项目
来源：http://rsf.hysaishi.cn

npm init -y;  npm i express
来源：http://umm.0kj1m.cn

[U82] JS：package.json 脚本
来源：http://btb.shanyushiyangtech.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ksl.smart0.xyz

[U83] JS：ES Module 导入导出
来源：http://lpj.xuetiantiany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://uov.nwbrower.top

[U84] JS：CommonJS 写法
来源：http://ukf.hammf.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qil.ydzc1.top

[U85] JS：可选链
来源：http://mxj.ehwqpu.com

a?.b?.c
来源：http://pmt.sysykeji.top

[U86] JS：空值合并
来源：http://zma.havefunace.top

a ?? b
来源：http://mqc.uphjek.com

[U87] JS：解构默认值
来源：http://bph.dashuyun.cn

const { a = 1, b = 2 } = obj;
来源：http://hno.daxiang520.top

[U88] JS：对象展开合并
来源：http://omp.0kj1m.cn

{ ...a, ...b }
来源：http://wfi.dashuyun.cn

[U89] JS：数组去重
来源：http://dac.daxiang520.top

[...new Set(arr)]
来源：http://dwl.sysykeji.top

[U90] JS：数字数组排序
来源：http://dqx.dianchejie.cn

[...arr].sort((a, b) => a - b)
来源：http://rbr.shzxlz.cn

[U91] JS：对象键值遍历
来源：http://guf.0kj1m.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bqw.jianghu66.top

[U92] JS：深拷贝
来源：http://ezv.shuidangran.top

structuredClone(obj)
来源：http://xru.yongpay.top

[U93] JS：模板字符串
来源：http://bef.iojbl.cn

`共 ${n} 条`
来源：http://ebg.jinghuilouyu.cn

[U94] JS：箭头函数
来源：http://zgf.jianghu66.top

const double = x => x * 2;
来源：http://fct.meibo888.top

[U95] JS：Promise 包装
来源：http://feb.ivvv.top

new Promise((resolve, reject) => {})
来源：http://cub.jlsjyb.cn

[U96] JS：async/await 与异常
来源：http://bye.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xux.dashuyun.cn

[U97] JS：并发请求
来源：http://qtg.svipenyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://eor.ydjk.org.cn

[U98] JS：fetch 带 JSON
来源：http://ddg.chenlongwang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ufa.ydzc1.top

[U99] JS：事件监听
来源：http://snz.zdqjudy.top

el.addEventListener("click", e => {})
来源：http://xha.hammf.cn

[U100] JS：DOM 查询
来源：http://uax.mhx1999.top

document.querySelector(".item")
来源：http://gcc.fehbvm.com

[U101] JS：classList 操作
来源：http://itz.xinyue.icu

el.classList.toggle("active")
来源：http://otm.ivvv.top

[U102] JS：本地存储
来源：http://gbc.hnxiangtu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wmx.yonumen.top

[U103] JS：定时器
来源：http://qmp.yongpay.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ful.zhijiandao.cn

[U104] JS：防抖
来源：http://glc.haohaochexian.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lpq.yvedp.cn

[U105] JS：节流
来源：http://ovc.ydzc1.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bvs.hfpthk.cn

[U106] JS：日期格式化
来源：http://jpo.sysykeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nqc.hysaishi.cn

[U107] JS：数字千分位
来源：http://lfj.yuxming.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ufh.yueranfly.top

[U108] JS：随机整数
来源：http://vvd.wangshuangyany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jje.haohaochexian.top

[U109] JS：数组分组
来源：http://maf.sxryk.cn

Object.groupBy(arr, x => x.type)
来源：http://ohv.fzhhl.top

[U110] JS：数组分块
来源：http://xji.zhongyouzk.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://exb.ydzc1.top

[U111] JS：对象转 Map
来源：http://aka.dianchejie.cn

new Map(Object.entries(obj))
来源：http://igk.jianghu66.top

[U112] JS：字符串补位
来源：http://fyl.jinqigfzy.top

"7".padStart(3, "0")
来源：http://vgj.ehwqpu.com

[U113] JS：正则替换全部
来源：http://frx.guannengcc.top

s.replaceAll("a", "b")
来源：http://nrm.tarul.cn

[U114] JS：JSON 深比较
来源：http://jio.yongpay.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pji.ctjpmb.com

[U115] JS：生成 UUID
来源：http://jyn.nanxinkj.top

crypto.randomUUID()
来源：http://jom.cqqwz.cn

[U116] JS：类型检查（JSDoc）
来源：http://ehz.vehdjk.com

/** @param {string} name */ function f(name) {}
来源：http://frx.zhaomingkeji.xyz

[U117] JS：单元测试
来源：http://vqz.cucudq.cn

npm i -D vitest;  npx vitest
来源：http://wmc.jinghuilouyu.cn

[U118] JS：开发服务器
来源：http://ule.cdnleiting.top

npm i -D vite;  npx vite
来源：http://rmv.vqdsnc.cn

[U119] JS：生产构建
来源：http://vzy.xingfuxueyuan.xyz

npx vite build
来源：http://tgv.vqdsnc.cn

[U120] JS：读取环境变量（Vite）
来源：http://eml.yangfankeji.com

import.meta.env.VITE_API_URL
来源：http://hwp.xinyue.icu

================================================================================
来源：http://kvc.jinqigfzy.top

统计汇总
来源：http://tvz.hysaishi.cn

================================================================================
来源：http://muy.jyoumei.cn

按语言统计（条）：
来源：http://vlo.hcnkem.com

Python ......... 252
来源：http://oua.gogol.net.cn

PHP ............ 252
来源：http://fxc.shuidangran.top

JavaScript ..... 252
来源：http://czn.yuxming.cn

TypeScript ..... 212
来源：http://jpl.fehbvm.com

Java ........... 212
来源：http://nsd.redwolf501.top

Go ............. 212
来源：http://pqd.pengpengdd.cyou

Ruby ........... 212
来源：http://kiu.fzhhl.top

C# ............. 212
来源：http://rpx.jqgufenzy.top

C .............. 30
来源：http://dax.pycfn.com

C++ ............ 30
来源：http://ios.shzxlz.cn

SQL ............ 90
来源：http://ukt.mhx1999.top

Bash ........... 80
来源：http://jam.gzhubu.top

Kotlin ......... 15
来源：http://xca.yj202588.top

Swift .......... 15
来源：http://bcr.hysaishi.cn

Lua ............ 10
来源：http://tno.havefunace.top

Perl ........... 10
来源：http://ywn.cdnleiting.top

Scala .......... 10
来源：http://hht.jyoumei.cn

------------------------------------
来源：http://aya.daxiang520.top

合计 ........... 2106 条
来源：http://dfh.xuanzx.com

按章节统计：
来源：http://jgr.gzhubu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cqm.shzxlz.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bdd.gotoacloud.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gmx.shanyushiyangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pef.sjlbkw.cn


<!-- 参考信息 -->