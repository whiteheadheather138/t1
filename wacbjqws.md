代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://ifn.guannengcc.top

[T55] Scala：集合过滤
来源：http://ssd.cheryme.top

List(1, 2, 3).filter(_ > 1)
来源：http://teu.hysaishi.cn

[T56] Scala：样例类
来源：http://lbe.shanyushiyangkeji.top

case class User(name: String, age: Int)
来源：http://kte.zdqjudy.top

[T57] Scala：模式匹配
来源：http://coh.52xcode.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uwz.xuetiantiany.cn

[T58] Scala：函数定义
来源：http://pjj.hnxiangtu.top

def add(a: Int, b: Int): Int = a + b
来源：http://kkp.jinqigfzy.top

[T59] Scala：循环
来源：http://zbe.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://akx.zycfv.cn

[T60] Scala：折叠
来源：http://vaj.nwbrower.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ket.fengsongda.top

================================================================================
来源：http://zcg.fehbvm.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tom.zhijiandao.cn

================================================================================
来源：http://bet.hnqzz.top

[U01] Py：创建虚拟环境
来源：http://pxu.nwbrower.top

python -m venv .venv && source .venv/bin/activate
来源：http://sfb.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://szr.shuidangran.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wpi.jinghuilouyu.cn

[U03] Py：加载 .env 配置
来源：http://ndg.gotoacloud.top

from dotenv import load_dotenv; load_dotenv()
来源：http://yly.fzhhl.top

[U04] Py：变量调试打印
来源：http://sim.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iov.tanke756.top

[U05] Py：列表去重且保序
来源：http://hec.epnwcf.com

list(dict.fromkeys(arr))
来源：http://tea.gotoacloud.top

[U06] Py：合并两个字典
来源：http://ehd.9152youxi.cn

{**a, **b}
来源：http://yzf.nanxuanxn.top

[U07] Py：反转字典键值
来源：http://flo.guowangkeji.top

{v: k for k, v in d.items()}
来源：http://tnu.fktsv.cn

[U08] Py：展平二维列表
来源：http://bzb.zdbjq.cn

[y for x in nested for y in x]
来源：http://dyf.sjlbkw.cn

[U09] Py：字典取最大值的键
来源：http://shj.shanyushiyangtech.top

max(d, key=d.get)
来源：http://pkx.uphjek.com

[U10] Py：按值排序字典
来源：http://edl.shangyingyoupin.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iig.zdbjq.cn

[U11] Py：生成器表达式
来源：http://suk.epnwcf.com

(x * 2 for x in arr)
来源：http://ctg.yonumen.top

[U12] Py：取出现最多的 3 个元素
来源：http://uhd.tanke756.top

Counter(arr).most_common(3)
来源：http://upq.meibo888.top

[U13] Py：固定长度队列
来源：http://jjt.jianghu66.top

deque(maxlen=10)
来源：http://lza.zdqjudy.top

[U14] Py：分组收集到列表
来源：http://fgq.sysykeji.top

defaultdict(list)
来源：http://gdp.redwolf501.top

[U15] Py：高精度计时
来源：http://bcn.jlsjyb.cn

t = time.perf_counter()
来源：http://rnc.ivvv.top

[U16] Py：命令行参数解析
来源：http://sfq.iojbl.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ofe.dashuyun.cn

[U17] Py：初始化日志
来源：http://bdt.fengsongda.top

logging.basicConfig(level=logging.INFO)
来源：http://bnl.wangshuangyany.cn

[U18] Py：预编译正则
来源：http://zzu.sxryk.cn

pat = re.compile(r"\d+")
来源：http://scx.xingfuxueyuan.xyz

[U19] Py：正则替换带回调
来源：http://bos.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wdo.zdqjudy.top

[U20] Py：缓存函数结果
来源：http://ydo.jianghu66.top

@functools.lru_cache(maxsize=None)
来源：http://rfh.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://npw.jqgufenzy.top

@contextlib.contextmanager
来源：http://gkj.bjfxy.top

[U22] Py：矩阵转置
来源：http://lfj.sysykeji.top

list(zip(*m))
来源：http://ymw.c1oappe.top

[U23] Py：分块读取大文件
来源：http://fjx.sysykeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://edt.yuanzhike.top

[U24] Py：路径操作
来源：http://nod.birdmap.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cre.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://sng.xingfuxueyuan.xyz

csv.DictReader(f)
来源：http://wvx.xylfe.cn

[U26] Py：并发下载
来源：http://gjh.cdnleiting.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://asr.yfazqb.com

[U27] Py：异步 HTTP
来源：http://bib.andypj.xyz

aiohttp.ClientSession() 配合 async with
来源：http://yfe.tarul.cn

[U28] Py：类型别名
来源：http://nbo.xingfuxueyuan.xyz

UserId = int
来源：http://vrq.xingfuxueyuan.xyz

[U29] Py：属性校验
来源：http://zqb.gaohongyu789.top

@property 与 @x.setter 配合
来源：http://iql.pengpengdd.cyou

[U30] Py：数据类
来源：http://qnr.jqgufenzy.top

@dataclass(slots=True)
来源：http://qii.quarkkingdee.top

[U31] Py：单测
来源：http://rlm.guowangkeji.top

python -m pytest -q
来源：http://zct.jinqigfzy.top

[U32] Py：代码格式化
来源：http://pcl.nanxuanxn.top

ruff format . && ruff check --fix .
来源：http://usb.sjlbkw.cn

[U33] Py：打包发布
来源：http://njs.yuxming.cn

python -m build  （依赖 pyproject.toml）
来源：http://tuq.jiagoushi.top

[U34] Py：判断编码
来源：http://dxb.gotoacloud.top

chardet.detect(raw)
来源：http://grr.fzhhl.top

[U35] Py：发送邮件
来源：http://jqt.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vup.sweek.top

[U36] Py：定时任务
来源：http://bvj.hesvh.cn

schedule.every(10).minutes.do(job)
来源：http://zzr.hfpthk.cn

[U37] Py：读写 Excel
来源：http://qla.xinyue.icu

pandas.read_excel / DataFrame.to_excel
来源：http://wct.meibo888.top

[U38] Py：获取脚本所在目录
来源：http://wtn.ctjpmb.com

Path(__file__).resolve().parent
来源：http://wpz.fanxiaobao.xyz

[U39] Py：判断是否在交互环境
来源：http://tab.hfpthk.cn

sys.stdout.isatty()
来源：http://tpg.sxryk.cn

[U40] Py：打印到标准错误
来源：http://ash.tian-w.cn

print("err", file=sys.stderr)
来源：http://okh.shzxlz.cn

[U41] PHP：初始化 Composer 项目
来源：http://ybw.gzhubu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jhg.gzhubu.top

[U42] PHP：PSR-4 自动加载
来源：http://njf.yfazqb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lht.pycfn.com

[U43] PHP：声明命名空间
来源：http://vak.shanyushiyangkeji.top

namespace App\Http;
来源：http://new.zhengqikj.top

[U44] PHP：开启严格类型
来源：http://dfj.aibaodan.cn

declare(strict_types=1);
来源：http://ziv.vehdjk.com

[U45] PHP：类型声明与返回类型
来源：http://kqu.havefunace.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://cbe.mhx1999.top

[U46] PHP：可空类型
来源：http://iqc.ydzc1.top

?string $name = null
来源：http://nsv.fengsongda.top

[U47] PHP：联合类型
来源：http://tui.meibo888.top

int|string $id
来源：http://spw.c1oappe.top

[U48] PHP：纯枚举
来源：http://cco.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tce.gaohongyu789.top

[U49] PHP：只读属性
来源：http://ful.shzxlz.cn

public readonly string $name
来源：http://nij.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://kaq.aibaodan.cn

public function __construct(private int $id) {}
来源：http://och.jinqigfzy.top

[U51] PHP：数组解构
来源：http://ukt.pycfn.com

[$a, $b] = $arr;
来源：http://qba.chenzaomai.com

[U52] PHP：箭头函数
来源：http://fmj.hcnkem.com

$double = fn($x) => $x * 2;
来源：http://lvz.epnwcf.com

[U53] PHP：空合并运算符
来源：http://bdk.shzxlz.cn

$v = $a ?? $b ?? "default";
来源：http://vbu.cashguo.top

[U54] PHP：空安全调用
来源：http://nng.zhixingplan.top

$obj?->method()
来源：http://ueq.xingfuxueyuan.xyz

[U55] PHP：match 表达式
来源：http://wbc.epnwcf.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lrd.xuetiantiany.cn

[U56] PHP：命名参数
来源：http://hbt.vehdjk.com

f(a: 1, b: 2)
来源：http://dro.xuanzx.com

[U57] PHP：字符串插值
来源：http://dfu.cqqwz.cn

"值: {$a}"
来源：http://opg.yuanzhike.top

[U58] PHP：数组三件套
来源：http://xjb.bjfxy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mso.chenlongwang.top

[U59] PHP：自定义排序
来源：http://mxd.ywan-chungtsiang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bux.nanxinkj.top

[U60] PHP：JSON 编解码
来源：http://aaq.jinghuilouyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kmw.ivvv.top

[U61] PHP：正则
来源：http://fhx.tanke756.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://knv.jinqigufen.top

[U62] PHP：日期对象
来源：http://cck.yanxiufei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://npp.dashuyun.cn

[U63] PHP：文件读写
来源：http://bod.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jnu.jianghu66.top

[U64] PHP：目录遍历
来源：http://eia.sysykeji.top

glob("dir/*.php");  scandir("dir");
来源：http://jyp.meibo888.top

[U65] PHP：会话
来源：http://hql.svipenyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zny.zhengqikj.top

[U66] PHP：设置 Cookie
来源：http://xkk.zycfv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cbb.52xcode.cn

[U67] PHP：处理文件上传
来源：http://ufj.jlsjyb.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kuc.hammf.cn

[U68] PHP：PDO 连接
来源：http://hzx.hnqzz.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rzu.daxiang520.top

[U69] PHP：PDO 预处理
来源：http://bxb.cucudq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ael.yongpay.top

[U70] PHP：PDO 事务
来源：http://oyp.meibo888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fgd.cheryme.top

[U71] PHP：抛出异常
来源：http://xxq.feifeiyinyue.top

throw new RuntimeException("失败", 500);
来源：http://mxk.cheryme.top

[U72] PHP：写错误日志
来源：http://rtx.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://xgd.vqdsnc.cn

[U73] PHP：读取 ini 配置
来源：http://plc.jqgfzy.top

parse_ini_file("config.ini", true)
来源：http://nex.gzhubu.top

[U74] PHP：读取环境变量
来源：http://fyb.cdnleiting.top

getenv("APP_ENV") ?: "production"
来源：http://jhd.hnxiangtu.top

[U75] PHP：依赖注入
来源：http://wny.havefunace.top

composer require psr/container
来源：http://hpm.vehdjk.com

[U76] PHP：简单路由
来源：http://cwk.fehbvm.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ldl.sufxvd.cn

[U77] PHP：模板渲染
来源：http://vcd.haohaochexian.top

composer require twig/twig
来源：http://zxw.cdnleiting.top

[U78] PHP：单元测试
来源：http://woi.zhixingplan.top

composer require --dev phpunit/phpunit
来源：http://kqk.sufxvd.cn

[U79] PHP：静态分析
来源：http://vuk.cqqwz.cn

composer require --dev phpstan/phpstan
来源：http://nsx.yonumen.top

[U80] PHP：代码规范修复
来源：http://gds.gzhubu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://snc.guannengcc.top

[U81] JS：初始化项目
来源：http://ebv.hnxiangtu.top

npm init -y;  npm i express
来源：http://oqj.hammf.cn

[U82] JS：package.json 脚本
来源：http://inv.iojbl.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zhv.pycfn.com

[U83] JS：ES Module 导入导出
来源：http://zzy.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wei.c1oappe.top

[U84] JS：CommonJS 写法
来源：http://ecs.fanxiaobao.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://dbk.gogol.net.cn

[U85] JS：可选链
来源：http://wju.shuidangran.top

a?.b?.c
来源：http://was.wangshuangyany.cn

[U86] JS：空值合并
来源：http://rtp.gotoacloud.top

a ?? b
来源：http://dcz.pycfn.com

[U87] JS：解构默认值
来源：http://vsw.daxiang520.top

const { a = 1, b = 2 } = obj;
来源：http://yji.zhixingplan.top

[U88] JS：对象展开合并
来源：http://gzs.yj20258888.top

{ ...a, ...b }
来源：http://onr.snrcjt.cn

[U89] JS：数组去重
来源：http://btl.yuanzhike.top

[...new Set(arr)]
来源：http://mee.cheryme.top

[U90] JS：数字数组排序
来源：http://eol.yj202588.top

[...arr].sort((a, b) => a - b)
来源：http://wsi.kuanghao11.cn

[U91] JS：对象键值遍历
来源：http://nxo.ppjwa.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yhy.fengsongda.top

[U92] JS：深拷贝
来源：http://jir.yuanzhike.top

structuredClone(obj)
来源：http://mog.meibo888.top

[U93] JS：模板字符串
来源：http://ken.hnxiangtu.top

`共 ${n} 条`
来源：http://qvz.birdmap.top

[U94] JS：箭头函数
来源：http://lxf.nanxinkj.top

const double = x => x * 2;
来源：http://qbb.guowangkeji.top

[U95] JS：Promise 包装
来源：http://vbo.zhiwuduotai.top

new Promise((resolve, reject) => {})
来源：http://ydv.c1oappe.top

[U96] JS：async/await 与异常
来源：http://bqz.chenzaomai.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bdo.tian-w.cn

[U97] JS：并发请求
来源：http://exj.quarkkingdee.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yyf.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://rqx.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jep.shanyushiyangkeji.top

[U99] JS：事件监听
来源：http://dbb.zhixingplan.top

el.addEventListener("click", e => {})
来源：http://xnz.yfazqb.com

[U100] JS：DOM 查询
来源：http://jaq.zhaomingkeji.xyz

document.querySelector(".item")
来源：http://blg.jyoumei.cn

[U101] JS：classList 操作
来源：http://iwt.birdmap.top

el.classList.toggle("active")
来源：http://dyc.svipenyu.cn

[U102] JS：本地存储
来源：http://bdd.zhaomingkeji.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://mxv.wangshuangyany.cn

[U103] JS：定时器
来源：http://cvp.ydjk.org.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fyi.snrcjt.cn

[U104] JS：防抖
来源：http://ccc.316326.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yyr.hesvh.cn

[U105] JS：节流
来源：http://vyv.quarkkingdee.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jrh.chenzaomai.com

[U106] JS：日期格式化
来源：http://vml.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cyc.ivvv.top

[U107] JS：数字千分位
来源：http://qnj.zhixingplan.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://elz.aibaodan.cn

[U108] JS：随机整数
来源：http://opk.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://okb.guowangkeji.top

[U109] JS：数组分组
来源：http://twp.gogol.net.cn

Object.groupBy(arr, x => x.type)
来源：http://uxm.zhoulong.xyz

[U110] JS：数组分块
来源：http://bdh.tarul.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bln.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://ame.jianghu66.top

new Map(Object.entries(obj))
来源：http://xue.tanke756.top

[U112] JS：字符串补位
来源：http://fwj.meibo888.top

"7".padStart(3, "0")
来源：http://pnx.dianchejie.cn

[U113] JS：正则替换全部
来源：http://xpi.cheryme.top

s.replaceAll("a", "b")
来源：http://svo.yj20258888.top

[U114] JS：JSON 深比较
来源：http://kie.hywenlv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vsy.zhoulong.xyz

[U115] JS：生成 UUID
来源：http://lmh.meibo888.top

crypto.randomUUID()
来源：http://yoa.pengpengdd.cyou

[U116] JS：类型检查（JSDoc）
来源：http://mag.sjlbkw.cn

/** @param {string} name */ function f(name) {}
来源：http://vix.jlsjyb.cn

[U117] JS：单元测试
来源：http://iiq.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://hxh.xinyue.icu

[U118] JS：开发服务器
来源：http://ujq.zhengqikj.top

npm i -D vite;  npx vite
来源：http://hxf.hesvh.cn

[U119] JS：生产构建
来源：http://uzq.jiagoushi.top

npx vite build
来源：http://jfj.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://gpx.hnxiangtu.top

import.meta.env.VITE_API_URL
来源：http://hgf.jinghuilouyu.cn

================================================================================
来源：http://tga.zhoulong.xyz

统计汇总
来源：http://yis.ybcxt.top

================================================================================
来源：http://hdd.pycfn.com

按语言统计（条）：
来源：http://igv.tanke756.top

Python ......... 252
来源：http://ifa.svipenyu.cn

PHP ............ 252
来源：http://cvq.chenzaomai.com

JavaScript ..... 252
来源：http://kbu.birdmap.top

TypeScript ..... 212
来源：http://xpw.gogol.net.cn

Java ........... 212
来源：http://iww.ivvv.top

Go ............. 212
来源：http://jkj.hysaishi.cn

Ruby ........... 212
来源：http://typ.cashguo.top

C# ............. 212
来源：http://ykm.haohaochexian.top

C .............. 30
来源：http://tsg.cqqwz.cn

C++ ............ 30
来源：http://nst.shangyingyoupin.top

SQL ............ 90
来源：http://sfd.jinghuilouyu.cn

Bash ........... 80
来源：http://jht.shanyushiyangkeji.top

Kotlin ......... 15
来源：http://ivx.chenzaomai.com

Swift .......... 15
来源：http://vds.daxiang520.top

Lua ............ 10
来源：http://unx.cashguo.top

Perl ........... 10
来源：http://frr.ydjk.org.cn

Scala .......... 10
来源：http://sqd.aibaodan.cn

------------------------------------
来源：http://ccj.zhoulong.xyz

合计 ........... 2106 条
来源：http://fsq.hcnkem.com

按章节统计：
来源：http://azb.shangyingyoupin.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ldz.jinqigufen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fqn.zdbjq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ppb.hysaishi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hfn.dashuyun.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://txa.ydjk.org.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bat.pycfn.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bqi.pycfn.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jbb.yfazqb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ytj.nwbrower.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://twc.jqgufenzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tju.zhaomingkeji.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://edu.c1oappe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lqz.hongshengwenyu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kmu.fzhhl.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ani.bbcook.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ofk.nanxinkj.top

Q SQL 专题                              90
来源：http://exa.bjfxy.top

R Bash 专题                             80
来源：http://yum.redwolf501.top

S C / C++ 专题                          60
来源：http://zbj.chenjidiqi.icu

T 其他语言补充                          60
来源：http://mru.wangdashe.top


<!-- 参考信息 -->