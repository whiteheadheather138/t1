代发 wailian999

val a = 1;  var b = 2
来源：http://jjs.0kj1m.cn

[T53] Scala：字符串插值
来源：http://zar.zhoulong.xyz

s"值: $b"
来源：http://unm.chenlongwang.top

[T54] Scala：集合映射
来源：http://afw.birdmap.top

List(1, 2, 3).map(_ * 2)
来源：http://mhq.shuidangran.top

[T55] Scala：集合过滤
来源：http://jll.sweek.top

List(1, 2, 3).filter(_ > 1)
来源：http://bpj.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://xdl.jqgfzy.top

case class User(name: String, age: Int)
来源：http://lbl.fehbvm.com

[T57] Scala：模式匹配
来源：http://xhw.havefunace.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bbf.nanxinkj.top

[T58] Scala：函数定义
来源：http://uth.shanyushiyangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://gfs.ydjk.org.cn

[T59] Scala：循环
来源：http://osm.aizwys.cn

for (i <- 1 to 10) println(i)
来源：http://akk.gogol.net.cn

[T60] Scala：折叠
来源：http://lnp.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cuz.nanxuanxn.top

================================================================================
来源：http://dzr.c1oappe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://enq.jianghu66.top

================================================================================
来源：http://anl.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://pfk.aizwys.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mrt.gogol.net.cn

[U02] Py：导出 / 安装依赖
来源：http://olx.ctjpmb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cde.shuidangran.top

[U03] Py：加载 .env 配置
来源：http://uhh.chenjidiqi.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://jzg.fktsv.cn

[U04] Py：变量调试打印
来源：http://qgr.yuxming.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pmk.jyoumei.cn

[U05] Py：列表去重且保序
来源：http://imt.uphjek.com

list(dict.fromkeys(arr))
来源：http://pga.ydjk.org.cn

[U06] Py：合并两个字典
来源：http://spa.vehdjk.com

{**a, **b}
来源：http://tgu.shanyushiyangkeji.top

[U07] Py：反转字典键值
来源：http://voe.yonumen.top

{v: k for k, v in d.items()}
来源：http://sow.xuanzx.com

[U08] Py：展平二维列表
来源：http://knh.nwbrower.top

[y for x in nested for y in x]
来源：http://wgw.jinqigufen.top

[U09] Py：字典取最大值的键
来源：http://ord.uphjek.com

max(d, key=d.get)
来源：http://vdk.xziqi.cn

[U10] Py：按值排序字典
来源：http://eqb.sxryk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hji.yj202588.top

[U11] Py：生成器表达式
来源：http://igf.shanyushiyangtech.top

(x * 2 for x in arr)
来源：http://vpf.cdnleiting.top

[U12] Py：取出现最多的 3 个元素
来源：http://mvo.hysaishi.cn

Counter(arr).most_common(3)
来源：http://hty.jqgfzy.top

[U13] Py：固定长度队列
来源：http://uoj.hammf.cn

deque(maxlen=10)
来源：http://fek.iojbl.cn

[U14] Py：分组收集到列表
来源：http://ccd.yanxiufei.cn

defaultdict(list)
来源：http://qfb.xziqi.cn

[U15] Py：高精度计时
来源：http://vdb.xylfe.cn

t = time.perf_counter()
来源：http://uut.yj20258.top

[U16] Py：命令行参数解析
来源：http://twt.tarul.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://peb.smart0.xyz

[U17] Py：初始化日志
来源：http://pjd.yuxming.cn

logging.basicConfig(level=logging.INFO)
来源：http://iuh.fehbvm.com

[U18] Py：预编译正则
来源：http://fus.hnxiangtu.top

pat = re.compile(r"\d+")
来源：http://rzy.dianchejie.cn

[U19] Py：正则替换带回调
来源：http://zfa.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tyo.9152youxi.cn

[U20] Py：缓存函数结果
来源：http://kjb.tianlin.xyz

@functools.lru_cache(maxsize=None)
来源：http://klf.cheryme.top

[U21] Py：自定义上下文管理器
来源：http://gcv.jqgufenzy.top

@contextlib.contextmanager
来源：http://bha.jinqigufen.top

[U22] Py：矩阵转置
来源：http://cyx.yj20258.top

list(zip(*m))
来源：http://qwz.tanke756.top

[U23] Py：分块读取大文件
来源：http://rff.shzxlz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://piy.jinqigufen.top

[U24] Py：路径操作
来源：http://ujd.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mta.sufxvd.cn

[U25] Py：CSV 按字典读
来源：http://rhy.shanyushiyangkeji.top

csv.DictReader(f)
来源：http://ntf.havefunace.top

[U26] Py：并发下载
来源：http://wcf.ydjk.org.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fbw.hongshengwenyu.top

[U27] Py：异步 HTTP
来源：http://zmv.jinghuilouyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://bfe.cqqwz.cn

[U28] Py：类型别名
来源：http://zht.tianlin.xyz

UserId = int
来源：http://lvp.tianlin.xyz

[U29] Py：属性校验
来源：http://hst.zhongyouzk.top

@property 与 @x.setter 配合
来源：http://cat.zycfv.cn

[U30] Py：数据类
来源：http://zpe.bbcook.cn

@dataclass(slots=True)
来源：http://tqd.bbcook.cn

[U31] Py：单测
来源：http://qyp.sysykeji.top

python -m pytest -q
来源：http://lya.nwbrower.top

[U32] Py：代码格式化
来源：http://dud.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://ogd.zhengqikj.top

[U33] Py：打包发布
来源：http://hex.hcnkem.com

python -m build  （依赖 pyproject.toml）
来源：http://drv.yuanzhike.top

[U34] Py：判断编码
来源：http://tjv.tian-w.cn

chardet.detect(raw)
来源：http://ads.yangfankeji.com

[U35] Py：发送邮件
来源：http://twx.yj20258888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wum.xinyue.icu

[U36] Py：定时任务
来源：http://wlo.tianlin.xyz

schedule.every(10).minutes.do(job)
来源：http://lsl.cdnleiting.top

[U37] Py：读写 Excel
来源：http://nry.cucudq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uxt.kuanghao11.cn

[U38] Py：获取脚本所在目录
来源：http://cmc.yj202588.top

Path(__file__).resolve().parent
来源：http://pzi.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://qsn.uphjek.com

sys.stdout.isatty()
来源：http://dqq.xingfuxueyuan.xyz

[U40] Py：打印到标准错误
来源：http://jto.9152youxi.cn

print("err", file=sys.stderr)
来源：http://xwq.xziqi.cn

[U41] PHP：初始化 Composer 项目
来源：http://zkx.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://cdd.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://ewh.shuidangran.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rsa.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://ulf.wangdashe.top

namespace App\Http;
来源：http://dlv.daria6918.cn

[U44] PHP：开启严格类型
来源：http://rrw.havefunace.top

declare(strict_types=1);
来源：http://nkt.haohaochexian.top

[U45] PHP：类型声明与返回类型
来源：http://jhv.smart0.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://fka.zhixingplan.top

[U46] PHP：可空类型
来源：http://fhq.tian-w.cn

?string $name = null
来源：http://ixg.sweek.top

[U47] PHP：联合类型
来源：http://xcu.uphjek.com

int|string $id
来源：http://sgx.ybcxt.top

[U48] PHP：纯枚举
来源：http://lfw.52xcode.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://brn.jlsjyb.cn

[U49] PHP：只读属性
来源：http://qwe.zhengqikj.top

public readonly string $name
来源：http://rmf.xinyue.icu

[U50] PHP：构造器属性提升
来源：http://suk.guowangkeji.top

public function __construct(private int $id) {}
来源：http://sfw.yj202588.top

[U51] PHP：数组解构
来源：http://luf.zhixingplan.top

[$a, $b] = $arr;
来源：http://kcp.cqqwz.cn

[U52] PHP：箭头函数
来源：http://wxs.zhaomingkeji.xyz

$double = fn($x) => $x * 2;
来源：http://qlu.cashguo.top

[U53] PHP：空合并运算符
来源：http://lgc.xziqi.cn

$v = $a ?? $b ?? "default";
来源：http://ckv.yueranfly.top

[U54] PHP：空安全调用
来源：http://wcd.zhaomingkeji.xyz

$obj?->method()
来源：http://lko.cdnleiting.top

[U55] PHP：match 表达式
来源：http://mqm.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wit.shanyushiyangkeji.top

[U56] PHP：命名参数
来源：http://skv.hesvh.cn

f(a: 1, b: 2)
来源：http://qha.jiagoushi.top

[U57] PHP：字符串插值
来源：http://osn.sxryk.cn

"值: {$a}"
来源：http://tzf.fzhhl.top

[U58] PHP：数组三件套
来源：http://nyk.nanxuanxn.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zpc.nanxuanxn.top

[U59] PHP：自定义排序
来源：http://stu.dianchejie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ggs.yj20258888.top

[U60] PHP：JSON 编解码
来源：http://ych.9152youxi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://stl.dashuyun.cn

[U61] PHP：正则
来源：http://zbq.havefunace.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wsq.havefunace.top

[U62] PHP：日期对象
来源：http://cdz.jqgfzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tne.shuidangran.top

[U63] PHP：文件读写
来源：http://pws.guannengcc.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xgl.hnqzz.top

[U64] PHP：目录遍历
来源：http://dea.gogol.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://pel.andypj.xyz

[U65] PHP：会话
来源：http://vka.hywenlv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://azf.zhixingplan.top

[U66] PHP：设置 Cookie
来源：http://cah.yanxiufei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rur.feifeiyinyue.top

[U67] PHP：处理文件上传
来源：http://lqt.0kj1m.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ihg.shanyushiyangtech.top

[U68] PHP：PDO 连接
来源：http://jwo.aizwys.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://aca.hywenlv.cn

[U69] PHP：PDO 预处理
来源：http://mmo.52xcode.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rim.hywenlv.cn

[U70] PHP：PDO 事务
来源：http://hwt.cdnleiting.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://glk.cdnleiting.top

[U71] PHP：抛出异常
来源：http://ocg.zdqjudy.top

throw new RuntimeException("失败", 500);
来源：http://kjl.sxryk.cn

[U72] PHP：写错误日志
来源：http://dbb.ywan-chungtsiang.top

error_log("失败: " . $e->getMessage());
来源：http://uhl.ybcxt.top

[U73] PHP：读取 ini 配置
来源：http://odc.nwbrower.top

parse_ini_file("config.ini", true)
来源：http://ttg.yvedp.cn

[U74] PHP：读取环境变量
来源：http://ocb.xuanzx.com

getenv("APP_ENV") ?: "production"
来源：http://dhg.dianchejie.cn

[U75] PHP：依赖注入
来源：http://mgc.shanyushiyangtech.top

composer require psr/container
来源：http://dbb.ppjwa.cn

[U76] PHP：简单路由
来源：http://dej.fzhhl.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bqw.cheryme.top

[U77] PHP：模板渲染
来源：http://nma.gzhubu.top

composer require twig/twig
来源：http://zms.cheryme.top

[U78] PHP：单元测试
来源：http://igg.kuanghao11.cn

composer require --dev phpunit/phpunit
来源：http://xaj.quarkkingdee.top

[U79] PHP：静态分析
来源：http://bdb.havefunace.top

composer require --dev phpstan/phpstan
来源：http://wwl.ivvv.top

[U80] PHP：代码规范修复
来源：http://ohd.zhiwuduotai.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://orx.smart0.xyz

[U81] JS：初始化项目
来源：http://ywr.cucudq.cn

npm init -y;  npm i express
来源：http://iqv.yongpay.top

[U82] JS：package.json 脚本
来源：http://qai.fengsongda.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vez.zhongyouzk.top

[U83] JS：ES Module 导入导出
来源：http://vkf.chenzaomai.com

export const a = 1;  import { a } from "./m.js";
来源：http://uho.nwbrower.top

[U84] JS：CommonJS 写法
来源：http://iqv.chenlongwang.top

module.exports = { a };  const { a } = require("./m");
来源：http://cll.xuanzx.com

[U85] JS：可选链
来源：http://pws.zycfv.cn

a?.b?.c
来源：http://aut.dashuyun.cn

[U86] JS：空值合并
来源：http://nel.cucudq.cn

a ?? b
来源：http://jyc.yfazqb.com

[U87] JS：解构默认值
来源：http://tir.jiagoushi.top

const { a = 1, b = 2 } = obj;
来源：http://pif.aibaodan.cn

[U88] JS：对象展开合并
来源：http://poy.jianghu66.top

{ ...a, ...b }
来源：http://wwm.zhiwuduotai.top

[U89] JS：数组去重
来源：http://qys.ydjk.org.cn

[...new Set(arr)]
来源：http://bud.yuxming.cn

[U90] JS：数字数组排序
来源：http://mdz.ivvv.top

[...arr].sort((a, b) => a - b)
来源：http://slo.52xcode.cn

[U91] JS：对象键值遍历
来源：http://gqc.hfpthk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dvt.bbcook.cn

[U92] JS：深拷贝
来源：http://fqu.sxryk.cn

structuredClone(obj)
来源：http://cbn.c1oappe.top

[U93] JS：模板字符串
来源：http://zme.hongshengwenyu.top

`共 ${n} 条`
来源：http://tky.zdbjq.cn

[U94] JS：箭头函数
来源：http://waf.cqqwz.cn

const double = x => x * 2;
来源：http://jav.jinghuilouyu.cn

[U95] JS：Promise 包装
来源：http://ayr.shuidangran.top

new Promise((resolve, reject) => {})
来源：http://atu.zdqjudy.top

[U96] JS：async/await 与异常
来源：http://rbc.quarkkingdee.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qsf.pycfn.com

[U97] JS：并发请求
来源：http://szn.ivvv.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lde.yvedp.cn

[U98] JS：fetch 带 JSON
来源：http://yuh.tian-w.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hro.zhijiandao.cn

[U99] JS：事件监听
来源：http://vyu.mhx1999.top

el.addEventListener("click", e => {})
来源：http://ntb.haohaochexian.top

[U100] JS：DOM 查询
来源：http://xdj.ydjk.org.cn

document.querySelector(".item")
来源：http://kql.yuxming.cn

[U101] JS：classList 操作
来源：http://zdw.ybcxt.top

el.classList.toggle("active")
来源：http://abe.shanyushiyangkeji.top

[U102] JS：本地存储
来源：http://rnj.hcnkem.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://hfq.nwbrower.top

[U103] JS：定时器
来源：http://qmp.c1oappe.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rhk.vqdsnc.cn

[U104] JS：防抖
来源：http://tle.redwolf501.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cjo.bjfxy.top

[U105] JS：节流
来源：http://hki.zhongyouzk.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fpw.hnxiangtu.top

[U106] JS：日期格式化
来源：http://pjk.shuidangran.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kui.sweek.top

[U107] JS：数字千分位
来源：http://uxi.ydjk.org.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sml.sxryk.cn

[U108] JS：随机整数
来源：http://egp.andypj.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sbg.chenjidiqi.icu

[U109] JS：数组分组
来源：http://dxj.yangfankeji.com

Object.groupBy(arr, x => x.type)
来源：http://trh.0kj1m.cn

[U110] JS：数组分块
来源：http://pgl.hongshengwenyu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://put.yfazqb.com

[U111] JS：对象转 Map
来源：http://lql.hysaishi.cn

new Map(Object.entries(obj))
来源：http://jwo.jianghu66.top

[U112] JS：字符串补位
来源：http://lrb.aibaodan.cn

"7".padStart(3, "0")
来源：http://kjo.fanxiaobao.xyz

[U113] JS：正则替换全部
来源：http://eiw.yueranfly.top

s.replaceAll("a", "b")
来源：http://vyq.uphjek.com

[U114] JS：JSON 深比较
来源：http://jzv.vehdjk.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://jcg.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://umj.zhongyouzk.top

crypto.randomUUID()
来源：http://rts.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://hcn.hnqzz.top

/** @param {string} name */ function f(name) {}
来源：http://hpj.sufxvd.cn

[U117] JS：单元测试
来源：http://ozg.tianlin.xyz

npm i -D vitest;  npx vitest
来源：http://gvh.hongshengwenyu.top

[U118] JS：开发服务器
来源：http://lhy.fanxiaobao.xyz

npm i -D vite;  npx vite
来源：http://wls.feifeiyinyue.top

[U119] JS：生产构建
来源：http://uhw.yuanzhike.top

npx vite build
来源：http://ibx.xingfuxueyuan.xyz

[U120] JS：读取环境变量（Vite）
来源：http://vin.tian-w.cn

import.meta.env.VITE_API_URL
来源：http://hnj.ydjk.org.cn

================================================================================
来源：http://pxy.jinyuanbaomall.cn

统计汇总
来源：http://jsj.bjfxy.top

================================================================================
来源：http://nfi.hongshengwenyu.top

按语言统计（条）：
来源：http://lqf.ydjk.org.cn

Python ......... 252
来源：http://ewr.zdbjq.cn

PHP ............ 252
来源：http://dcz.feifeiyinyue.top

JavaScript ..... 252
来源：http://vip.ctjpmb.com

TypeScript ..... 212
来源：http://ein.aibaodan.cn

Java ........... 212
来源：http://cuz.jianghu66.top

Go ............. 212
来源：http://fzd.mhx1999.top

Ruby ........... 212
来源：http://wcc.guowangkeji.top

C# ............. 212
来源：http://ymi.cucudq.cn

C .............. 30
来源：http://ngm.cqqwz.cn

C++ ............ 30
来源：http://jld.sxryk.cn

SQL ............ 90
来源：http://wkl.wangshuangyany.cn

Bash ........... 80
来源：http://wmr.hfpthk.cn

Kotlin ......... 15
来源：http://aij.redwolf501.top

Swift .......... 15
来源：http://chm.jinghuilouyu.cn

Lua ............ 10
来源：http://del.yongpay.top

Perl ........... 10
来源：http://tqj.jqgfzy.top

Scala .......... 10
来源：http://gfs.xuanzx.com

------------------------------------
来源：http://cib.jinghuilouyu.cn

合计 ........... 2106 条
来源：http://xzb.haohaochexian.top

按章节统计：
来源：http://xcc.jlsjyb.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ced.epnwcf.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wfc.hesvh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gqh.jyoumei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://svv.cqqwz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zfe.dianchejie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qpr.bjfxy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tvi.yanxiufei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mpt.yj20258.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jxv.yongpay.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mls.chenzaomai.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://obq.yj20258888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dlf.sweek.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fln.smart0.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ngt.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vcq.jiagoushi.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mvx.uphjek.com


<!-- 参考信息 -->