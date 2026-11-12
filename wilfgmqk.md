代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://apu.yj20258888.top

[T55] Scala：集合过滤
来源：http://qhx.sxryk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oee.pycfn.com

[T56] Scala：样例类
来源：http://myr.kuanghao11.cn

case class User(name: String, age: Int)
来源：http://yfg.birdmap.top

[T57] Scala：模式匹配
来源：http://lcg.vqdsnc.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ywd.zdbjq.cn

[T58] Scala：函数定义
来源：http://ftn.nanxuanxn.top

def add(a: Int, b: Int): Int = a + b
来源：http://sps.yangfankeji.com

[T59] Scala：循环
来源：http://mak.yj20258.top

for (i <- 1 to 10) println(i)
来源：http://wyc.jqgfzy.top

[T60] Scala：折叠
来源：http://lmc.sweek.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dle.fengsongda.top

================================================================================
来源：http://ozp.zhengqikj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ozt.xingfuxueyuan.xyz

================================================================================
来源：http://oec.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://bqf.gzhubu.top

python -m venv .venv && source .venv/bin/activate
来源：http://ddz.daxiang520.top

[U02] Py：导出 / 安装依赖
来源：http://grl.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://okj.pengpengdd.cyou

[U03] Py：加载 .env 配置
来源：http://zqy.ehwqpu.com

from dotenv import load_dotenv; load_dotenv()
来源：http://pmj.jinghuilouyu.cn

[U04] Py：变量调试打印
来源：http://fgt.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mvn.cheryme.top

[U05] Py：列表去重且保序
来源：http://suz.jinghuilouyu.cn

list(dict.fromkeys(arr))
来源：http://vyn.sufxvd.cn

[U06] Py：合并两个字典
来源：http://hvs.aizwys.cn

{**a, **b}
来源：http://iif.sweek.top

[U07] Py：反转字典键值
来源：http://ell.snrcjt.cn

{v: k for k, v in d.items()}
来源：http://qts.cashguo.top

[U08] Py：展平二维列表
来源：http://zfw.chenzaomai.com

[y for x in nested for y in x]
来源：http://yax.jianghu66.top

[U09] Py：字典取最大值的键
来源：http://weu.chenlongwang.top

max(d, key=d.get)
来源：http://xhk.ctjpmb.com

[U10] Py：按值排序字典
来源：http://xxn.chenlongwang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wax.smart0.xyz

[U11] Py：生成器表达式
来源：http://kjs.yj20258.top

(x * 2 for x in arr)
来源：http://fdl.yonumen.top

[U12] Py：取出现最多的 3 个元素
来源：http://zis.gzhubu.top

Counter(arr).most_common(3)
来源：http://buz.xuetiantiany.cn

[U13] Py：固定长度队列
来源：http://vok.jinqigufen.top

deque(maxlen=10)
来源：http://ehw.ctjpmb.com

[U14] Py：分组收集到列表
来源：http://yle.nanxuanxn.top

defaultdict(list)
来源：http://uix.nanxinkj.top

[U15] Py：高精度计时
来源：http://ttt.cashguo.top

t = time.perf_counter()
来源：http://qfd.hongshengwenyu.top

[U16] Py：命令行参数解析
来源：http://qjg.xziqi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://svk.hcnkem.com

[U17] Py：初始化日志
来源：http://zmt.yfazqb.com

logging.basicConfig(level=logging.INFO)
来源：http://jnw.dianchejie.cn

[U18] Py：预编译正则
来源：http://mfh.jlsjyb.cn

pat = re.compile(r"\d+")
来源：http://dzu.yj202588.top

[U19] Py：正则替换带回调
来源：http://hpf.yj202588.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://npn.yvedp.cn

[U20] Py：缓存函数结果
来源：http://izq.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://hzv.shanyushiyangtech.top

[U21] Py：自定义上下文管理器
来源：http://tgt.yfazqb.com

@contextlib.contextmanager
来源：http://nug.fktsv.cn

[U22] Py：矩阵转置
来源：http://ddt.fanxiaobao.xyz

list(zip(*m))
来源：http://wwp.9152youxi.cn

[U23] Py：分块读取大文件
来源：http://lts.fanxiaobao.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eah.meibo888.top

[U24] Py：路径操作
来源：http://udh.jyoumei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hqh.zdqjudy.top

[U25] Py：CSV 按字典读
来源：http://zon.aibaodan.cn

csv.DictReader(f)
来源：http://ikc.hammf.cn

[U26] Py：并发下载
来源：http://nwa.yuanzhike.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://odv.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://lpx.haohaochexian.top

aiohttp.ClientSession() 配合 async with
来源：http://xjb.yangfankeji.com

[U28] Py：类型别名
来源：http://aci.tarul.cn

UserId = int
来源：http://sqk.feifeiyinyue.top

[U29] Py：属性校验
来源：http://gwv.yonumen.top

@property 与 @x.setter 配合
来源：http://iks.zhixingplan.top

[U30] Py：数据类
来源：http://sqb.yuxming.cn

@dataclass(slots=True)
来源：http://uqg.hysaishi.cn

[U31] Py：单测
来源：http://csq.epnwcf.com

python -m pytest -q
来源：http://qvm.fktsv.cn

[U32] Py：代码格式化
来源：http://qrt.yfazqb.com

ruff format . && ruff check --fix .
来源：http://lns.sjlbkw.cn

[U33] Py：打包发布
来源：http://jfl.shuidangran.top

python -m build  （依赖 pyproject.toml）
来源：http://zpv.uphjek.com

[U34] Py：判断编码
来源：http://mji.snrcjt.cn

chardet.detect(raw)
来源：http://aiz.yj20258.top

[U35] Py：发送邮件
来源：http://zly.ppjwa.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dfq.xylfe.cn

[U36] Py：定时任务
来源：http://icu.c1oappe.top

schedule.every(10).minutes.do(job)
来源：http://hzk.52xcode.cn

[U37] Py：读写 Excel
来源：http://zeh.tian-w.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wbv.yongpay.top

[U38] Py：获取脚本所在目录
来源：http://gup.gzhubu.top

Path(__file__).resolve().parent
来源：http://jwu.hesvh.cn

[U39] Py：判断是否在交互环境
来源：http://lar.tian-w.cn

sys.stdout.isatty()
来源：http://zad.feifeiyinyue.top

[U40] Py：打印到标准错误
来源：http://nwz.ywan-chungtsiang.top

print("err", file=sys.stderr)
来源：http://pli.iojbl.cn

[U41] PHP：初始化 Composer 项目
来源：http://peg.xuetiantiany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zuo.smart0.xyz

[U42] PHP：PSR-4 自动加载
来源：http://yvc.ivvv.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yhx.zhaomingkeji.xyz

[U43] PHP：声明命名空间
来源：http://ash.bjfxy.top

namespace App\Http;
来源：http://oth.yonumen.top

[U44] PHP：开启严格类型
来源：http://kfv.nanxinkj.top

declare(strict_types=1);
来源：http://zwq.316326.xyz

[U45] PHP：类型声明与返回类型
来源：http://mmo.yj20258888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wpo.fanxiaobao.xyz

[U46] PHP：可空类型
来源：http://sat.9152youxi.cn

?string $name = null
来源：http://tjc.feifeiyinyue.top

[U47] PHP：联合类型
来源：http://fyt.meibo888.top

int|string $id
来源：http://rpr.0kj1m.cn

[U48] PHP：纯枚举
来源：http://kqu.guannengcc.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qfj.aizwys.cn

[U49] PHP：只读属性
来源：http://ubw.daria6918.cn

public readonly string $name
来源：http://iyy.vqdsnc.cn

[U50] PHP：构造器属性提升
来源：http://akp.yvedp.cn

public function __construct(private int $id) {}
来源：http://rfu.birdmap.top

[U51] PHP：数组解构
来源：http://qky.zdbjq.cn

[$a, $b] = $arr;
来源：http://xpr.cucudq.cn

[U52] PHP：箭头函数
来源：http://xhv.daxiang520.top

$double = fn($x) => $x * 2;
来源：http://gcb.wangdashe.top

[U53] PHP：空合并运算符
来源：http://eal.vehdjk.com

$v = $a ?? $b ?? "default";
来源：http://ruv.iojbl.cn

[U54] PHP：空安全调用
来源：http://hct.hcnkem.com

$obj?->method()
来源：http://wwj.jqgufenzy.top

[U55] PHP：match 表达式
来源：http://gml.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uvn.jlsjyb.cn

[U56] PHP：命名参数
来源：http://ifh.cucudq.cn

f(a: 1, b: 2)
来源：http://olb.fktsv.cn

[U57] PHP：字符串插值
来源：http://zks.smart0.xyz

"值: {$a}"
来源：http://vgg.fehbvm.com

[U58] PHP：数组三件套
来源：http://reu.pycfn.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gqb.chenjidiqi.icu

[U59] PHP：自定义排序
来源：http://akr.bjfxy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fcu.yj20258888.top

[U60] PHP：JSON 编解码
来源：http://pum.cheryme.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dyw.zdqjudy.top

[U61] PHP：正则
来源：http://zel.haohaochexian.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kyh.9152youxi.cn

[U62] PHP：日期对象
来源：http://qdk.xinyue.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yws.zdqjudy.top

[U63] PHP：文件读写
来源：http://bek.wangshuangyany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nse.bjfxy.top

[U64] PHP：目录遍历
来源：http://zgf.ehwqpu.com

glob("dir/*.php");  scandir("dir");
来源：http://kam.yj20258888.top

[U65] PHP：会话
来源：http://hbp.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vst.hongshengwenyu.top

[U66] PHP：设置 Cookie
来源：http://pbo.c1oappe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fwz.chenjidiqi.icu

[U67] PHP：处理文件上传
来源：http://bgf.hywenlv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://afh.kuanghao11.cn

[U68] PHP：PDO 连接
来源：http://yhv.yangfankeji.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rch.xingfuxueyuan.xyz

[U69] PHP：PDO 预处理
来源：http://owl.havefunace.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gza.daxiang520.top

[U70] PHP：PDO 事务
来源：http://spg.yj20258.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://idt.hnxiangtu.top

[U71] PHP：抛出异常
来源：http://ohd.xziqi.cn

throw new RuntimeException("失败", 500);
来源：http://ucu.zdqjudy.top

[U72] PHP：写错误日志
来源：http://rdo.shangyingyoupin.top

error_log("失败: " . $e->getMessage());
来源：http://tbl.ctjpmb.com

[U73] PHP：读取 ini 配置
来源：http://qxn.ywan-chungtsiang.top

parse_ini_file("config.ini", true)
来源：http://lko.jqgufenzy.top

[U74] PHP：读取环境变量
来源：http://itk.fengsongda.top

getenv("APP_ENV") ?: "production"
来源：http://stk.vqdsnc.cn

[U75] PHP：依赖注入
来源：http://ces.zhongyouzk.top

composer require psr/container
来源：http://tua.andypj.xyz

[U76] PHP：简单路由
来源：http://lty.0kj1m.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tbz.guannengcc.top

[U77] PHP：模板渲染
来源：http://iww.andypj.xyz

composer require twig/twig
来源：http://bxj.jiagoushi.top

[U78] PHP：单元测试
来源：http://syv.xingfuxueyuan.xyz

composer require --dev phpunit/phpunit
来源：http://kij.hongshengwenyu.top

[U79] PHP：静态分析
来源：http://xgc.dianchejie.cn

composer require --dev phpstan/phpstan
来源：http://jbt.shuidangran.top

[U80] PHP：代码规范修复
来源：http://bha.nanxinkj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jxa.dianchejie.cn

[U81] JS：初始化项目
来源：http://wkx.jinghuilouyu.cn

npm init -y;  npm i express
来源：http://sbo.zhaomingkeji.xyz

[U82] JS：package.json 脚本
来源：http://xwy.hammf.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jbn.jyoumei.cn

[U83] JS：ES Module 导入导出
来源：http://myf.gotoacloud.top

export const a = 1;  import { a } from "./m.js";
来源：http://slv.tian-w.cn

[U84] JS：CommonJS 写法
来源：http://wtz.nanxinkj.top

module.exports = { a };  const { a } = require("./m");
来源：http://wnd.jlsjyb.cn

[U85] JS：可选链
来源：http://xjj.sxryk.cn

a?.b?.c
来源：http://fcb.zdqjudy.top

[U86] JS：空值合并
来源：http://neb.xylfe.cn

a ?? b
来源：http://ebg.gaohongyu789.top

[U87] JS：解构默认值
来源：http://fft.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://aeh.redwolf501.top

[U88] JS：对象展开合并
来源：http://cyp.fanxiaobao.xyz

{ ...a, ...b }
来源：http://xce.pycfn.com

[U89] JS：数组去重
来源：http://mpl.9152youxi.cn

[...new Set(arr)]
来源：http://pqs.jinqigufen.top

[U90] JS：数字数组排序
来源：http://xzv.gzhubu.top

[...arr].sort((a, b) => a - b)
来源：http://hsx.ppjwa.cn

[U91] JS：对象键值遍历
来源：http://jee.316326.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sjp.sxryk.cn

[U92] JS：深拷贝
来源：http://jfq.jinyuanbaomall.cn

structuredClone(obj)
来源：http://kzx.ydzc1.top

[U93] JS：模板字符串
来源：http://xnr.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://rzf.wangdashe.top

[U94] JS：箭头函数
来源：http://ssz.cashguo.top

const double = x => x * 2;
来源：http://zrb.52xcode.cn

[U95] JS：Promise 包装
来源：http://shg.yj202588.top

new Promise((resolve, reject) => {})
来源：http://lwx.316326.xyz

[U96] JS：async/await 与异常
来源：http://bdp.tarul.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mcx.dashuyun.cn

[U97] JS：并发请求
来源：http://tln.feifeiyinyue.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qwo.hywenlv.cn

[U98] JS：fetch 带 JSON
来源：http://byq.haohaochexian.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ogq.redwolf501.top

[U99] JS：事件监听
来源：http://kcm.dianchejie.cn

el.addEventListener("click", e => {})
来源：http://ukp.zycfv.cn

[U100] JS：DOM 查询
来源：http://mwc.epnwcf.com

document.querySelector(".item")
来源：http://hfq.sufxvd.cn

[U101] JS：classList 操作
来源：http://oaj.c1oappe.top

el.classList.toggle("active")
来源：http://qfe.fengsongda.top

[U102] JS：本地存储
来源：http://tpt.fengsongda.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ghk.hysaishi.cn

[U103] JS：定时器
来源：http://krm.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tjk.tian-w.cn

[U104] JS：防抖
来源：http://omj.redwolf501.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pcz.0kj1m.cn

[U105] JS：节流
来源：http://vhz.jinyuanbaomall.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gws.xuanzx.com

[U106] JS：日期格式化
来源：http://kvo.ydzc1.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lau.cqqwz.cn

[U107] JS：数字千分位
来源：http://ntf.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ndm.yanxiufei.cn

[U108] JS：随机整数
来源：http://dwp.shanyushiyangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wyp.gaohongyu789.top

[U109] JS：数组分组
来源：http://lui.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://dvg.hesvh.cn

[U110] JS：数组分块
来源：http://xtj.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fco.xylfe.cn

[U111] JS：对象转 Map
来源：http://ryl.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://kku.hcnkem.com

[U112] JS：字符串补位
来源：http://mkp.hfpthk.cn

"7".padStart(3, "0")
来源：http://etx.hywenlv.cn

[U113] JS：正则替换全部
来源：http://ppn.bjfxy.top

s.replaceAll("a", "b")
来源：http://nme.hcnkem.com

[U114] JS：JSON 深比较
来源：http://ewi.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nuf.shuidangran.top

[U115] JS：生成 UUID
来源：http://sea.jinqigfzy.top

crypto.randomUUID()
来源：http://amb.jiagoushi.top

[U116] JS：类型检查（JSDoc）
来源：http://mvu.sxryk.cn

/** @param {string} name */ function f(name) {}
来源：http://maa.snrcjt.cn

[U117] JS：单元测试
来源：http://sfe.yangfankeji.com

npm i -D vitest;  npx vitest
来源：http://cba.tian-w.cn

[U118] JS：开发服务器
来源：http://nqq.nanxinkj.top

npm i -D vite;  npx vite
来源：http://ytf.yuxming.cn

[U119] JS：生产构建
来源：http://vrh.zhengqikj.top

npx vite build
来源：http://eup.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://owd.svipenyu.cn

import.meta.env.VITE_API_URL
来源：http://mxf.jianghu66.top

================================================================================
来源：http://fpa.gogol.net.cn

统计汇总
来源：http://dem.xingfuxueyuan.xyz

================================================================================
来源：http://gyt.snrcjt.cn

按语言统计（条）：
来源：http://ono.hesvh.cn

Python ......... 252
来源：http://qtt.bbcook.cn

PHP ............ 252
来源：http://bsj.ehwqpu.com

JavaScript ..... 252
来源：http://lvc.yongpay.top

TypeScript ..... 212
来源：http://bqx.yuanzhike.top

Java ........... 212
来源：http://mth.yangfankeji.com

Go ............. 212
来源：http://fwx.zhijiandao.cn

Ruby ........... 212
来源：http://jai.c1oappe.top

C# ............. 212
来源：http://dgu.ybcxt.top

C .............. 30
来源：http://qcv.xinyue.icu

C++ ............ 30
来源：http://rdw.hnxiangtu.top

SQL ............ 90
来源：http://kcs.pycfn.com

Bash ........... 80
来源：http://avf.hywenlv.cn

Kotlin ......... 15
来源：http://imz.feifeiyinyue.top

Swift .......... 15
来源：http://wao.yueranfly.top

Lua ............ 10
来源：http://nso.yonumen.top

Perl ........... 10
来源：http://hsn.bbcook.cn

Scala .......... 10
来源：http://new.sysykeji.top

------------------------------------
来源：http://qpc.hnqzz.top

合计 ........... 2106 条
来源：http://uon.ctjpmb.com

按章节统计：
来源：http://fid.ctjpmb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uuj.aibaodan.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xgw.wangdashe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vec.sweek.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://exa.sufxvd.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kaz.kuanghao11.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bvi.jyoumei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pdo.jlsjyb.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gko.yanxiufei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tpc.pengpengdd.cyou

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zzi.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gkm.smart0.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://psa.iojbl.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ugo.svipenyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ucn.zycfv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zbl.nanxuanxn.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://crb.mhx1999.top

Q SQL 专题                              90
来源：http://naf.wangshuangyany.cn

R Bash 专题                             80
来源：http://pym.guowangkeji.top

S C / C++ 专题                          60
来源：http://osy.hnqzz.top

T 其他语言补充                          60
来源：http://fer.hfpthk.cn


<!-- 参考信息 -->