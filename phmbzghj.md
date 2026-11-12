代发 wailian999

case class User(name: String, age: Int)
来源：http://jdz.zhengqikj.top

[T57] Scala：模式匹配
来源：http://tuo.guannengcc.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ofg.jinyuanbaomall.cn

[T58] Scala：函数定义
来源：http://sja.hnqzz.top

def add(a: Int, b: Int): Int = a + b
来源：http://wbp.ehwqpu.com

[T59] Scala：循环
来源：http://sft.ehwqpu.com

for (i <- 1 to 10) println(i)
来源：http://xgn.havefunace.top

[T60] Scala：折叠
来源：http://lut.cdnleiting.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://suo.ydjk.org.cn

================================================================================
来源：http://pze.gotoacloud.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bjp.snrcjt.cn

================================================================================
来源：http://tds.dianchejie.cn

[U01] Py：创建虚拟环境
来源：http://jsb.shzxlz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qtb.jinqigfzy.top

[U02] Py：导出 / 安装依赖
来源：http://ott.cqqwz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nqk.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://dxg.vehdjk.com

from dotenv import load_dotenv; load_dotenv()
来源：http://jyc.kuanghao11.cn

[U04] Py：变量调试打印
来源：http://gbm.havefunace.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lfq.cucudq.cn

[U05] Py：列表去重且保序
来源：http://tfg.hfpthk.cn

list(dict.fromkeys(arr))
来源：http://gog.haohaochexian.top

[U06] Py：合并两个字典
来源：http://eia.aizwys.cn

{**a, **b}
来源：http://xyq.iojbl.cn

[U07] Py：反转字典键值
来源：http://oxl.redwolf501.top

{v: k for k, v in d.items()}
来源：http://vtt.hongshengwenyu.top

[U08] Py：展平二维列表
来源：http://qag.yvedp.cn

[y for x in nested for y in x]
来源：http://xcg.yonumen.top

[U09] Py：字典取最大值的键
来源：http://yam.jiagoushi.top

max(d, key=d.get)
来源：http://gsl.jlsjyb.cn

[U10] Py：按值排序字典
来源：http://gqv.hysaishi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://knj.hfpthk.cn

[U11] Py：生成器表达式
来源：http://cyj.dashuyun.cn

(x * 2 for x in arr)
来源：http://sah.cucudq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gyr.tanke756.top

Counter(arr).most_common(3)
来源：http://lde.epnwcf.com

[U13] Py：固定长度队列
来源：http://mwz.hammf.cn

deque(maxlen=10)
来源：http://bgn.wangshuangyany.cn

[U14] Py：分组收集到列表
来源：http://hil.gotoacloud.top

defaultdict(list)
来源：http://mbk.cqqwz.cn

[U15] Py：高精度计时
来源：http://gai.jqgfzy.top

t = time.perf_counter()
来源：http://lta.ydzc1.top

[U16] Py：命令行参数解析
来源：http://cvy.0kj1m.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zgf.pengpengdd.cyou

[U17] Py：初始化日志
来源：http://tdo.jqgfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://oji.hesvh.cn

[U18] Py：预编译正则
来源：http://pqq.ivvv.top

pat = re.compile(r"\d+")
来源：http://zms.jqgfzy.top

[U19] Py：正则替换带回调
来源：http://gyy.yuxming.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oms.cqqwz.cn

[U20] Py：缓存函数结果
来源：http://luo.jinqigfzy.top

@functools.lru_cache(maxsize=None)
来源：http://nbb.jyoumei.cn

[U21] Py：自定义上下文管理器
来源：http://hce.jinqigfzy.top

@contextlib.contextmanager
来源：http://tow.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://ttw.yuanzhike.top

list(zip(*m))
来源：http://wen.gaohongyu789.top

[U23] Py：分块读取大文件
来源：http://wpt.mhx1999.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://owc.sweek.top

[U24] Py：路径操作
来源：http://whg.yuxming.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ytu.shzxlz.cn

[U25] Py：CSV 按字典读
来源：http://eqv.jyoumei.cn

csv.DictReader(f)
来源：http://qjx.yonumen.top

[U26] Py：并发下载
来源：http://nbw.daxiang520.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ydx.gzhubu.top

[U27] Py：异步 HTTP
来源：http://mgp.hfpthk.cn

aiohttp.ClientSession() 配合 async with
来源：http://xhm.tarul.cn

[U28] Py：类型别名
来源：http://ljj.hnxiangtu.top

UserId = int
来源：http://wme.vqdsnc.cn

[U29] Py：属性校验
来源：http://ozk.havefunace.top

@property 与 @x.setter 配合
来源：http://ztu.9152youxi.cn

[U30] Py：数据类
来源：http://hpy.smart0.xyz

@dataclass(slots=True)
来源：http://crg.yuxming.cn

[U31] Py：单测
来源：http://ogt.jqgfzy.top

python -m pytest -q
来源：http://egv.fengsongda.top

[U32] Py：代码格式化
来源：http://kcf.andypj.xyz

ruff format . && ruff check --fix .
来源：http://nol.yueranfly.top

[U33] Py：打包发布
来源：http://hmm.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://rye.svipenyu.cn

[U34] Py：判断编码
来源：http://hjf.nwbrower.top

chardet.detect(raw)
来源：http://okt.daxiang520.top

[U35] Py：发送邮件
来源：http://nck.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yru.ctjpmb.com

[U36] Py：定时任务
来源：http://mke.yongpay.top

schedule.every(10).minutes.do(job)
来源：http://awa.cqqwz.cn

[U37] Py：读写 Excel
来源：http://khn.fengsongda.top

pandas.read_excel / DataFrame.to_excel
来源：http://zcd.gogol.net.cn

[U38] Py：获取脚本所在目录
来源：http://xtj.yanxiufei.cn

Path(__file__).resolve().parent
来源：http://trv.ywan-chungtsiang.top

[U39] Py：判断是否在交互环境
来源：http://xby.mhx1999.top

sys.stdout.isatty()
来源：http://pyj.daxiang520.top

[U40] Py：打印到标准错误
来源：http://dfh.haohaochexian.top

print("err", file=sys.stderr)
来源：http://ghk.guowangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://nqz.guannengcc.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ppm.cdnleiting.top

[U42] PHP：PSR-4 自动加载
来源：http://bqm.cqqwz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zlc.hnxiangtu.top

[U43] PHP：声明命名空间
来源：http://xxv.yueranfly.top

namespace App\Http;
来源：http://gvm.bjfxy.top

[U44] PHP：开启严格类型
来源：http://btg.ivvv.top

declare(strict_types=1);
来源：http://ejc.dashuyun.cn

[U45] PHP：类型声明与返回类型
来源：http://lwy.fktsv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kdn.jqgufenzy.top

[U46] PHP：可空类型
来源：http://dri.chenlongwang.top

?string $name = null
来源：http://udp.sjlbkw.cn

[U47] PHP：联合类型
来源：http://rps.jqgufenzy.top

int|string $id
来源：http://bsu.jiagoushi.top

[U48] PHP：纯枚举
来源：http://txn.jinqigufen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nsi.yueranfly.top

[U49] PHP：只读属性
来源：http://quv.havefunace.top

public readonly string $name
来源：http://vyq.uphjek.com

[U50] PHP：构造器属性提升
来源：http://vrn.zhiwuduotai.top

public function __construct(private int $id) {}
来源：http://cue.uphjek.com

[U51] PHP：数组解构
来源：http://vut.shanyushiyangkeji.top

[$a, $b] = $arr;
来源：http://lwr.shuidangran.top

[U52] PHP：箭头函数
来源：http://vkn.dianchejie.cn

$double = fn($x) => $x * 2;
来源：http://xiq.kuanghao11.cn

[U53] PHP：空合并运算符
来源：http://yok.tarul.cn

$v = $a ?? $b ?? "default";
来源：http://emt.nanxuanxn.top

[U54] PHP：空安全调用
来源：http://wan.zdbjq.cn

$obj?->method()
来源：http://xuj.ydjk.org.cn

[U55] PHP：match 表达式
来源：http://fdq.birdmap.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://esn.zhengqikj.top

[U56] PHP：命名参数
来源：http://pfj.daxiang520.top

f(a: 1, b: 2)
来源：http://hrg.jinqigfzy.top

[U57] PHP：字符串插值
来源：http://ilb.yueranfly.top

"值: {$a}"
来源：http://ysh.vqdsnc.cn

[U58] PHP：数组三件套
来源：http://jrg.nanxinkj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ylo.ehwqpu.com

[U59] PHP：自定义排序
来源：http://dzr.havefunace.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nsa.ywan-chungtsiang.top

[U60] PHP：JSON 编解码
来源：http://ndu.fzhhl.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://avg.yonumen.top

[U61] PHP：正则
来源：http://onf.c1oappe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tow.sysykeji.top

[U62] PHP：日期对象
来源：http://qew.ehwqpu.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://njf.pengpengdd.cyou

[U63] PHP：文件读写
来源：http://knn.iojbl.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wcm.sufxvd.cn

[U64] PHP：目录遍历
来源：http://ekz.epnwcf.com

glob("dir/*.php");  scandir("dir");
来源：http://myl.sxryk.cn

[U65] PHP：会话
来源：http://rhk.zhaomingkeji.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://pvb.xingfuxueyuan.xyz

[U66] PHP：设置 Cookie
来源：http://qne.cdnleiting.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sbr.fehbvm.com

[U67] PHP：处理文件上传
来源：http://qfm.epnwcf.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qvo.xuanzx.com

[U68] PHP：PDO 连接
来源：http://nea.zdqjudy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://esf.jinyuanbaomall.cn

[U69] PHP：PDO 预处理
来源：http://wwr.daria6918.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rtz.jiagoushi.top

[U70] PHP：PDO 事务
来源：http://kmq.jinghuilouyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mfm.yongpay.top

[U71] PHP：抛出异常
来源：http://pot.birdmap.top

throw new RuntimeException("失败", 500);
来源：http://syg.chenlongwang.top

[U72] PHP：写错误日志
来源：http://smz.redwolf501.top

error_log("失败: " . $e->getMessage());
来源：http://fbu.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://fyh.jqgfzy.top

parse_ini_file("config.ini", true)
来源：http://rru.xinyue.icu

[U74] PHP：读取环境变量
来源：http://ket.chenzaomai.com

getenv("APP_ENV") ?: "production"
来源：http://esx.shanyushiyangkeji.top

[U75] PHP：依赖注入
来源：http://cyn.ybcxt.top

composer require psr/container
来源：http://dll.jqgufenzy.top

[U76] PHP：简单路由
来源：http://hlh.meibo888.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kqd.redwolf501.top

[U77] PHP：模板渲染
来源：http://qsu.xinyue.icu

composer require twig/twig
来源：http://huv.yueranfly.top

[U78] PHP：单元测试
来源：http://jks.dianchejie.cn

composer require --dev phpunit/phpunit
来源：http://sid.sweek.top

[U79] PHP：静态分析
来源：http://sua.tarul.cn

composer require --dev phpstan/phpstan
来源：http://nna.ydjk.org.cn

[U80] PHP：代码规范修复
来源：http://ils.jinqigufen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vdo.yj20258.top

[U81] JS：初始化项目
来源：http://rrr.sysykeji.top

npm init -y;  npm i express
来源：http://oxm.yvedp.cn

[U82] JS：package.json 脚本
来源：http://hwz.aibaodan.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fwr.yangfankeji.com

[U83] JS：ES Module 导入导出
来源：http://fpe.9152youxi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://uou.ppjwa.cn

[U84] JS：CommonJS 写法
来源：http://vgf.yj20258.top

module.exports = { a };  const { a } = require("./m");
来源：http://kko.zhiwuduotai.top

[U85] JS：可选链
来源：http://otw.hfpthk.cn

a?.b?.c
来源：http://uwp.sufxvd.cn

[U86] JS：空值合并
来源：http://xzb.guannengcc.top

a ?? b
来源：http://kym.andypj.xyz

[U87] JS：解构默认值
来源：http://kxn.chenzaomai.com

const { a = 1, b = 2 } = obj;
来源：http://oex.yuxming.cn

[U88] JS：对象展开合并
来源：http://sgc.chenlongwang.top

{ ...a, ...b }
来源：http://oxo.xinyue.icu

[U89] JS：数组去重
来源：http://xvp.shuidangran.top

[...new Set(arr)]
来源：http://upu.guannengcc.top

[U90] JS：数字数组排序
来源：http://frc.hywenlv.cn

[...arr].sort((a, b) => a - b)
来源：http://mxb.kuanghao11.cn

[U91] JS：对象键值遍历
来源：http://bcm.iojbl.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mcg.havefunace.top

[U92] JS：深拷贝
来源：http://lix.gaohongyu789.top

structuredClone(obj)
来源：http://yag.bbcook.cn

[U93] JS：模板字符串
来源：http://lic.hnxiangtu.top

`共 ${n} 条`
来源：http://uih.xuetiantiany.cn

[U94] JS：箭头函数
来源：http://lqi.bjfxy.top

const double = x => x * 2;
来源：http://sss.zhixingplan.top

[U95] JS：Promise 包装
来源：http://tvh.yuanzhike.top

new Promise((resolve, reject) => {})
来源：http://htg.tanke756.top

[U96] JS：async/await 与异常
来源：http://rfv.zhixingplan.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://omc.jianghu66.top

[U97] JS：并发请求
来源：http://jud.0kj1m.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oxe.guannengcc.top

[U98] JS：fetch 带 JSON
来源：http://odj.mhx1999.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://stm.vehdjk.com

[U99] JS：事件监听
来源：http://fel.52xcode.cn

el.addEventListener("click", e => {})
来源：http://bul.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://xmt.tarul.cn

document.querySelector(".item")
来源：http://yum.zdqjudy.top

[U101] JS：classList 操作
来源：http://zkn.zhaomingkeji.xyz

el.classList.toggle("active")
来源：http://knt.ybcxt.top

[U102] JS：本地存储
来源：http://djg.jlsjyb.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qtn.xziqi.cn

[U103] JS：定时器
来源：http://fxj.zhiwuduotai.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ipp.gaohongyu789.top

[U104] JS：防抖
来源：http://dno.bbcook.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://caz.jyoumei.cn

[U105] JS：节流
来源：http://kdp.zdbjq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qcb.fengsongda.top

[U106] JS：日期格式化
来源：http://yin.fzhhl.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rlf.xziqi.cn

[U107] JS：数字千分位
来源：http://irc.haohaochexian.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://anz.guowangkeji.top

[U108] JS：随机整数
来源：http://icu.pycfn.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lgv.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://wkg.hcnkem.com

Object.groupBy(arr, x => x.type)
来源：http://bbh.birdmap.top

[U110] JS：数组分块
来源：http://dlq.bjfxy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yjq.redwolf501.top

[U111] JS：对象转 Map
来源：http://asd.wangshuangyany.cn

new Map(Object.entries(obj))
来源：http://cmk.hammf.cn

[U112] JS：字符串补位
来源：http://hvi.jqgfzy.top

"7".padStart(3, "0")
来源：http://jbs.pengpengdd.cyou

[U113] JS：正则替换全部
来源：http://jop.andypj.xyz

s.replaceAll("a", "b")
来源：http://qxf.tian-w.cn

[U114] JS：JSON 深比较
来源：http://zjy.yj202588.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vus.aizwys.cn

[U115] JS：生成 UUID
来源：http://txf.jyoumei.cn

crypto.randomUUID()
来源：http://wch.pycfn.com

[U116] JS：类型检查（JSDoc）
来源：http://zbo.ywan-chungtsiang.top

/** @param {string} name */ function f(name) {}
来源：http://lzi.andypj.xyz

[U117] JS：单元测试
来源：http://kec.jiagoushi.top

npm i -D vitest;  npx vitest
来源：http://axp.ybcxt.top

[U118] JS：开发服务器
来源：http://bjg.zhongyouzk.top

npm i -D vite;  npx vite
来源：http://adr.zdbjq.cn

[U119] JS：生产构建
来源：http://cvn.xziqi.cn

npx vite build
来源：http://xcr.fanxiaobao.xyz

[U120] JS：读取环境变量（Vite）
来源：http://pbk.xinyue.icu

import.meta.env.VITE_API_URL
来源：http://mig.xuanzx.com

================================================================================
来源：http://aiw.ppjwa.cn

统计汇总
来源：http://tzt.yj20258.top

================================================================================
来源：http://wez.hcnkem.com

按语言统计（条）：
来源：http://xpk.52xcode.cn

Python ......... 252
来源：http://oxr.dashuyun.cn

PHP ............ 252
来源：http://kcp.cashguo.top

JavaScript ..... 252
来源：http://ygt.tianlin.xyz

TypeScript ..... 212
来源：http://wvt.gotoacloud.top

Java ........... 212
来源：http://rlc.chenzaomai.com

Go ............. 212
来源：http://dpl.sufxvd.cn

Ruby ........... 212
来源：http://ofb.gzhubu.top

C# ............. 212
来源：http://hpx.hammf.cn

C .............. 30
来源：http://vzr.hywenlv.cn

C++ ............ 30
来源：http://zpt.cheryme.top

SQL ............ 90
来源：http://ipe.uphjek.com

Bash ........... 80
来源：http://jsh.zhongyouzk.top

Kotlin ......... 15
来源：http://otw.kuanghao11.cn

Swift .......... 15
来源：http://xzc.ivvv.top

Lua ............ 10
来源：http://kaj.epnwcf.com

Perl ........... 10
来源：http://wdu.hesvh.cn

Scala .......... 10
来源：http://fbp.aibaodan.cn

------------------------------------
来源：http://rld.yvedp.cn

合计 ........... 2106 条
来源：http://fwz.hywenlv.cn

按章节统计：
来源：http://bwr.jianghu66.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://thx.meibo888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fxd.hammf.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fnl.daria6918.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ogz.yj202588.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ccy.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vue.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kos.cdnleiting.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dcv.fktsv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ubk.ydzc1.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xqh.vqdsnc.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iem.yangfankeji.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zld.guannengcc.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bgu.xuanzx.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uya.sweek.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wio.vqdsnc.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lzp.jinyuanbaomall.cn

Q SQL 专题                              90
来源：http://tjz.jinqigufen.top

R Bash 专题                             80
来源：http://awh.yj20258888.top

S C / C++ 专题                          60
来源：http://djy.zycfv.cn

T 其他语言补充                          60
来源：http://bdz.ppjwa.cn

U 高频实用片段                         120
来源：http://kdo.cucudq.cn

------------------------------------
来源：http://gxa.tarul.cn

合计                                  2106 条
来源：http://qio.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://zey.52xcode.cn


<!-- 参考信息 -->