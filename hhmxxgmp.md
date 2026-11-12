代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://rue.pengpengdd.cyou

[T55] Scala：集合过滤
来源：http://dim.shanyushiyangtech.top

List(1, 2, 3).filter(_ > 1)
来源：http://nnp.xziqi.cn

[T56] Scala：样例类
来源：http://cdl.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://nwp.yj20258.top

[T57] Scala：模式匹配
来源：http://vvz.jinghuilouyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mbs.wangshuangyany.cn

[T58] Scala：函数定义
来源：http://yrt.aibaodan.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tqi.cheryme.top

[T59] Scala：循环
来源：http://qul.cdnleiting.top

for (i <- 1 to 10) println(i)
来源：http://itz.quarkkingdee.top

[T60] Scala：折叠
来源：http://bcq.yj20258.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dfj.zhijiandao.cn

================================================================================
来源：http://hof.fzhhl.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nax.0kj1m.cn

================================================================================
来源：http://cqr.guannengcc.top

[U01] Py：创建虚拟环境
来源：http://cwh.daxiang520.top

python -m venv .venv && source .venv/bin/activate
来源：http://jiv.smart0.xyz

[U02] Py：导出 / 安装依赖
来源：http://udh.ctjpmb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fjh.yfazqb.com

[U03] Py：加载 .env 配置
来源：http://tnl.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://src.hysaishi.cn

[U04] Py：变量调试打印
来源：http://wbi.hywenlv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xjo.ehwqpu.com

[U05] Py：列表去重且保序
来源：http://tjw.chenjidiqi.icu

list(dict.fromkeys(arr))
来源：http://kjs.yanxiufei.cn

[U06] Py：合并两个字典
来源：http://hpr.shanyushiyangtech.top

{**a, **b}
来源：http://dqk.0kj1m.cn

[U07] Py：反转字典键值
来源：http://eet.sjlbkw.cn

{v: k for k, v in d.items()}
来源：http://pcq.yvedp.cn

[U08] Py：展平二维列表
来源：http://atm.zhongyouzk.top

[y for x in nested for y in x]
来源：http://ndp.hnqzz.top

[U09] Py：字典取最大值的键
来源：http://xis.hysaishi.cn

max(d, key=d.get)
来源：http://nec.c1oappe.top

[U10] Py：按值排序字典
来源：http://xqn.xuetiantiany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://guo.xuetiantiany.cn

[U11] Py：生成器表达式
来源：http://olr.hfpthk.cn

(x * 2 for x in arr)
来源：http://iam.tianlin.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://oeu.sysykeji.top

Counter(arr).most_common(3)
来源：http://qan.havefunace.top

[U13] Py：固定长度队列
来源：http://euz.zhoulong.xyz

deque(maxlen=10)
来源：http://kyd.daxiang520.top

[U14] Py：分组收集到列表
来源：http://fyt.yueranfly.top

defaultdict(list)
来源：http://cqz.cqqwz.cn

[U15] Py：高精度计时
来源：http://bdu.yj20258888.top

t = time.perf_counter()
来源：http://owy.snrcjt.cn

[U16] Py：命令行参数解析
来源：http://vpf.hywenlv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dlm.wangshuangyany.cn

[U17] Py：初始化日志
来源：http://jrp.shzxlz.cn

logging.basicConfig(level=logging.INFO)
来源：http://gfu.c1oappe.top

[U18] Py：预编译正则
来源：http://cdf.jyoumei.cn

pat = re.compile(r"\d+")
来源：http://nqo.sxryk.cn

[U19] Py：正则替换带回调
来源：http://wbi.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kcj.xylfe.cn

[U20] Py：缓存函数结果
来源：http://oyn.nwbrower.top

@functools.lru_cache(maxsize=None)
来源：http://ugf.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://jjb.kuanghao11.cn

@contextlib.contextmanager
来源：http://pox.havefunace.top

[U22] Py：矩阵转置
来源：http://lvh.zdqjudy.top

list(zip(*m))
来源：http://vyx.iojbl.cn

[U23] Py：分块读取大文件
来源：http://hmu.chenzaomai.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cmq.ehwqpu.com

[U24] Py：路径操作
来源：http://ccf.fehbvm.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ptn.hammf.cn

[U25] Py：CSV 按字典读
来源：http://mzl.hesvh.cn

csv.DictReader(f)
来源：http://uby.nwbrower.top

[U26] Py：并发下载
来源：http://dlf.jiagoushi.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lfx.sufxvd.cn

[U27] Py：异步 HTTP
来源：http://dik.tianlin.xyz

aiohttp.ClientSession() 配合 async with
来源：http://opa.fengsongda.top

[U28] Py：类型别名
来源：http://cbe.yuxming.cn

UserId = int
来源：http://rcq.birdmap.top

[U29] Py：属性校验
来源：http://xka.gzhubu.top

@property 与 @x.setter 配合
来源：http://nih.aizwys.cn

[U30] Py：数据类
来源：http://tis.jinqigfzy.top

@dataclass(slots=True)
来源：http://mor.gogol.net.cn

[U31] Py：单测
来源：http://dfi.hammf.cn

python -m pytest -q
来源：http://xxb.yuxming.cn

[U32] Py：代码格式化
来源：http://jcw.chenlongwang.top

ruff format . && ruff check --fix .
来源：http://pyq.bbcook.cn

[U33] Py：打包发布
来源：http://lcd.tian-w.cn

python -m build  （依赖 pyproject.toml）
来源：http://nhh.yuanzhike.top

[U34] Py：判断编码
来源：http://ohy.meibo888.top

chardet.detect(raw)
来源：http://vgp.zhengqikj.top

[U35] Py：发送邮件
来源：http://blw.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lxt.hysaishi.cn

[U36] Py：定时任务
来源：http://dbp.nanxuanxn.top

schedule.every(10).minutes.do(job)
来源：http://ukq.aizwys.cn

[U37] Py：读写 Excel
来源：http://rym.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://yim.cdnleiting.top

[U38] Py：获取脚本所在目录
来源：http://ezw.hongshengwenyu.top

Path(__file__).resolve().parent
来源：http://sdi.meibo888.top

[U39] Py：判断是否在交互环境
来源：http://xbn.hesvh.cn

sys.stdout.isatty()
来源：http://pqx.ydzc1.top

[U40] Py：打印到标准错误
来源：http://mrt.tarul.cn

print("err", file=sys.stderr)
来源：http://mxy.xuanzx.com

[U41] PHP：初始化 Composer 项目
来源：http://qju.daria6918.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://woy.zycfv.cn

[U42] PHP：PSR-4 自动加载
来源：http://mdt.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nzt.xinyue.icu

[U43] PHP：声明命名空间
来源：http://obk.kuanghao11.cn

namespace App\Http;
来源：http://riu.svipenyu.cn

[U44] PHP：开启严格类型
来源：http://vtf.hywenlv.cn

declare(strict_types=1);
来源：http://iaj.xuetiantiany.cn

[U45] PHP：类型声明与返回类型
来源：http://jza.wangshuangyany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mfj.zycfv.cn

[U46] PHP：可空类型
来源：http://yja.yangfankeji.com

?string $name = null
来源：http://ivr.zhixingplan.top

[U47] PHP：联合类型
来源：http://xmr.pengpengdd.cyou

int|string $id
来源：http://rrf.uphjek.com

[U48] PHP：纯枚举
来源：http://ywm.dashuyun.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rua.cqqwz.cn

[U49] PHP：只读属性
来源：http://nrk.yueranfly.top

public readonly string $name
来源：http://fhw.yj20258888.top

[U50] PHP：构造器属性提升
来源：http://rco.sysykeji.top

public function __construct(private int $id) {}
来源：http://dmd.aibaodan.cn

[U51] PHP：数组解构
来源：http://bhw.aibaodan.cn

[$a, $b] = $arr;
来源：http://utl.yonumen.top

[U52] PHP：箭头函数
来源：http://ytf.xuanzx.com

$double = fn($x) => $x * 2;
来源：http://axv.redwolf501.top

[U53] PHP：空合并运算符
来源：http://amk.mhx1999.top

$v = $a ?? $b ?? "default";
来源：http://pna.cqqwz.cn

[U54] PHP：空安全调用
来源：http://mew.yj20258.top

$obj?->method()
来源：http://pvn.dashuyun.cn

[U55] PHP：match 表达式
来源：http://pov.cheryme.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ooq.yuxming.cn

[U56] PHP：命名参数
来源：http://thj.zhijiandao.cn

f(a: 1, b: 2)
来源：http://heg.sysykeji.top

[U57] PHP：字符串插值
来源：http://lzl.vqdsnc.cn

"值: {$a}"
来源：http://ucb.cucudq.cn

[U58] PHP：数组三件套
来源：http://dan.yangfankeji.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zrw.sweek.top

[U59] PHP：自定义排序
来源：http://bbs.nwbrower.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gwc.nanxuanxn.top

[U60] PHP：JSON 编解码
来源：http://pxk.vqdsnc.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kva.xziqi.cn

[U61] PHP：正则
来源：http://qpd.chenjidiqi.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eyj.mhx1999.top

[U62] PHP：日期对象
来源：http://wvt.aibaodan.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qmc.zhixingplan.top

[U63] PHP：文件读写
来源：http://sze.daria6918.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://evm.fktsv.cn

[U64] PHP：目录遍历
来源：http://vpe.meibo888.top

glob("dir/*.php");  scandir("dir");
来源：http://oka.jinqigfzy.top

[U65] PHP：会话
来源：http://enp.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fdd.ehwqpu.com

[U66] PHP：设置 Cookie
来源：http://dbl.bbcook.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aao.ivvv.top

[U67] PHP：处理文件上传
来源：http://qdd.ydzc1.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://syi.redwolf501.top

[U68] PHP：PDO 连接
来源：http://qlg.ctjpmb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jay.gotoacloud.top

[U69] PHP：PDO 预处理
来源：http://ldd.zdbjq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nwa.hammf.cn

[U70] PHP：PDO 事务
来源：http://efy.haohaochexian.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eet.yvedp.cn

[U71] PHP：抛出异常
来源：http://gpp.daxiang520.top

throw new RuntimeException("失败", 500);
来源：http://mcz.zdbjq.cn

[U72] PHP：写错误日志
来源：http://lpu.hysaishi.cn

error_log("失败: " . $e->getMessage());
来源：http://djy.yuanzhike.top

[U73] PHP：读取 ini 配置
来源：http://hwf.haohaochexian.top

parse_ini_file("config.ini", true)
来源：http://lug.pengpengdd.cyou

[U74] PHP：读取环境变量
来源：http://wkj.ctjpmb.com

getenv("APP_ENV") ?: "production"
来源：http://dty.daria6918.cn

[U75] PHP：依赖注入
来源：http://rwg.sxryk.cn

composer require psr/container
来源：http://ria.svipenyu.cn

[U76] PHP：简单路由
来源：http://hkv.snrcjt.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yxs.yuxming.cn

[U77] PHP：模板渲染
来源：http://rvt.jlsjyb.cn

composer require twig/twig
来源：http://ltj.hywenlv.cn

[U78] PHP：单元测试
来源：http://wlq.tianlin.xyz

composer require --dev phpunit/phpunit
来源：http://dkv.tanke756.top

[U79] PHP：静态分析
来源：http://gwx.wangshuangyany.cn

composer require --dev phpstan/phpstan
来源：http://teo.smart0.xyz

[U80] PHP：代码规范修复
来源：http://naj.jianghu66.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://oia.tarul.cn

[U81] JS：初始化项目
来源：http://nic.ctjpmb.com

npm init -y;  npm i express
来源：http://ypm.shuidangran.top

[U82] JS：package.json 脚本
来源：http://mug.fktsv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yzo.yj202588.top

[U83] JS：ES Module 导入导出
来源：http://ufi.zhongyouzk.top

export const a = 1;  import { a } from "./m.js";
来源：http://qvd.fzhhl.top

[U84] JS：CommonJS 写法
来源：http://gss.tanke756.top

module.exports = { a };  const { a } = require("./m");
来源：http://vbn.316326.xyz

[U85] JS：可选链
来源：http://ple.yj20258888.top

a?.b?.c
来源：http://hvr.zdqjudy.top

[U86] JS：空值合并
来源：http://qal.jinghuilouyu.cn

a ?? b
来源：http://zzt.feifeiyinyue.top

[U87] JS：解构默认值
来源：http://uvy.ctjpmb.com

const { a = 1, b = 2 } = obj;
来源：http://zmb.kuanghao11.cn

[U88] JS：对象展开合并
来源：http://gcd.uphjek.com

{ ...a, ...b }
来源：http://snp.ybcxt.top

[U89] JS：数组去重
来源：http://ojw.yfazqb.com

[...new Set(arr)]
来源：http://whq.smart0.xyz

[U90] JS：数字数组排序
来源：http://tgp.xuanzx.com

[...arr].sort((a, b) => a - b)
来源：http://mjo.hnqzz.top

[U91] JS：对象键值遍历
来源：http://dha.sweek.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://crt.tarul.cn

[U92] JS：深拷贝
来源：http://sac.sjlbkw.cn

structuredClone(obj)
来源：http://ybn.yanxiufei.cn

[U93] JS：模板字符串
来源：http://psu.kuanghao11.cn

`共 ${n} 条`
来源：http://mkb.cucudq.cn

[U94] JS：箭头函数
来源：http://iqx.52xcode.cn

const double = x => x * 2;
来源：http://ubu.smart0.xyz

[U95] JS：Promise 包装
来源：http://fre.guowangkeji.top

new Promise((resolve, reject) => {})
来源：http://vzl.zycfv.cn

[U96] JS：async/await 与异常
来源：http://snq.chenzaomai.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lbs.xinyue.icu

[U97] JS：并发请求
来源：http://xno.zhongyouzk.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ijc.havefunace.top

[U98] JS：fetch 带 JSON
来源：http://ukz.ydzc1.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gwx.snrcjt.cn

[U99] JS：事件监听
来源：http://haq.sysykeji.top

el.addEventListener("click", e => {})
来源：http://kyb.bbcook.cn

[U100] JS：DOM 查询
来源：http://yar.daxiang520.top

document.querySelector(".item")
来源：http://xvw.yuxming.cn

[U101] JS：classList 操作
来源：http://cek.jinqigfzy.top

el.classList.toggle("active")
来源：http://ila.jiagoushi.top

[U102] JS：本地存储
来源：http://zmg.xziqi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hza.wangdashe.top

[U103] JS：定时器
来源：http://hyt.meibo888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gcx.hcnkem.com

[U104] JS：防抖
来源：http://swt.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fet.tian-w.cn

[U105] JS：节流
来源：http://kvn.zdbjq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ogq.shanyushiyangkeji.top

[U106] JS：日期格式化
来源：http://wac.bjfxy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kbj.jlsjyb.cn

[U107] JS：数字千分位
来源：http://jkx.gzhubu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ina.cashguo.top

[U108] JS：随机整数
来源：http://uaf.tanke756.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ulp.cucudq.cn

[U109] JS：数组分组
来源：http://dps.wangshuangyany.cn

Object.groupBy(arr, x => x.type)
来源：http://moh.jqgfzy.top

[U110] JS：数组分块
来源：http://hjj.zdbjq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lac.nanxinkj.top

[U111] JS：对象转 Map
来源：http://tzy.haohaochexian.top

new Map(Object.entries(obj))
来源：http://fer.vqdsnc.cn

[U112] JS：字符串补位
来源：http://yxt.iojbl.cn

"7".padStart(3, "0")
来源：http://rvc.smart0.xyz

[U113] JS：正则替换全部
来源：http://ggl.xylfe.cn

s.replaceAll("a", "b")
来源：http://ksk.hnxiangtu.top

[U114] JS：JSON 深比较
来源：http://awu.gaohongyu789.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wgn.gzhubu.top

[U115] JS：生成 UUID
来源：http://ymx.fanxiaobao.xyz

crypto.randomUUID()
来源：http://gbq.ywan-chungtsiang.top

[U116] JS：类型检查（JSDoc）
来源：http://qxb.gzhubu.top

/** @param {string} name */ function f(name) {}
来源：http://aii.dianchejie.cn

[U117] JS：单元测试
来源：http://vwx.snrcjt.cn

npm i -D vitest;  npx vitest
来源：http://fey.jinqigufen.top

[U118] JS：开发服务器
来源：http://icd.xingfuxueyuan.xyz

npm i -D vite;  npx vite
来源：http://pax.fktsv.cn

[U119] JS：生产构建
来源：http://lay.zhiwuduotai.top

npx vite build
来源：http://imj.zdbjq.cn

[U120] JS：读取环境变量（Vite）
来源：http://rwf.bjfxy.top

import.meta.env.VITE_API_URL
来源：http://rqn.sweek.top

================================================================================
来源：http://exk.hesvh.cn

统计汇总
来源：http://wpz.bjfxy.top

================================================================================
来源：http://ass.gotoacloud.top

按语言统计（条）：
来源：http://dhw.vehdjk.com

Python ......... 252
来源：http://hcq.hongshengwenyu.top

PHP ............ 252
来源：http://ivg.shanyushiyangkeji.top

JavaScript ..... 252
来源：http://rca.svipenyu.cn

TypeScript ..... 212
来源：http://nwq.chenlongwang.top

Java ........... 212
来源：http://zvs.nwbrower.top

Go ............. 212
来源：http://nmc.hongshengwenyu.top

Ruby ........... 212
来源：http://bcf.hfpthk.cn

C# ............. 212
来源：http://rwj.iojbl.cn

C .............. 30
来源：http://iey.zdqjudy.top

C++ ............ 30
来源：http://rzk.andypj.xyz

SQL ............ 90
来源：http://fbw.daria6918.cn

Bash ........... 80
来源：http://ktc.meibo888.top

Kotlin ......... 15
来源：http://gjd.ywan-chungtsiang.top

Swift .......... 15
来源：http://byf.vehdjk.com

Lua ............ 10
来源：http://vrb.kuanghao11.cn

Perl ........... 10
来源：http://dbm.fanxiaobao.xyz

Scala .......... 10
来源：http://ywg.ctjpmb.com

------------------------------------
来源：http://eum.yuanzhike.top

合计 ........... 2106 条
来源：http://sto.bjfxy.top

按章节统计：
来源：http://axl.mhx1999.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uyo.zdqjudy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wjg.hongshengwenyu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dwg.ydzc1.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ccu.52xcode.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mci.gzhubu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rot.52xcode.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zxi.hnqzz.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eht.hfpthk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hnq.zhengqikj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jbh.hysaishi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tjr.uphjek.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wqz.jlsjyb.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gub.ppjwa.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xcq.bjfxy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qyq.c1oappe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xhk.pycfn.com

Q SQL 专题                              90
来源：http://fgw.zhixingplan.top

R Bash 专题                             80
来源：http://ert.uphjek.com

S C / C++ 专题                          60
来源：http://cfe.cqqwz.cn

T 其他语言补充                          60
来源：http://qoz.9152youxi.cn


<!-- 参考信息 -->