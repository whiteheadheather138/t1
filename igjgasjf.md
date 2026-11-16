代发 wailian999

val a = 1;  var b = 2
来源：http://uox.fanxiaobao.xyz

[T53] Scala：字符串插值
来源：http://ljh.gaohongyu789.top

s"值: $b"
来源：http://hfj.0kj1m.cn

[T54] Scala：集合映射
来源：http://knj.ybcxt.top

List(1, 2, 3).map(_ * 2)
来源：http://afi.jinqigfzy.top

[T55] Scala：集合过滤
来源：http://zxb.mhx1999.top

List(1, 2, 3).filter(_ > 1)
来源：http://pfm.gzhubu.top

[T56] Scala：样例类
来源：http://wfn.jiagoushi.top

case class User(name: String, age: Int)
来源：http://mrh.yanxiufei.cn

[T57] Scala：模式匹配
来源：http://ctf.sjlbkw.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://emm.dianchejie.cn

[T58] Scala：函数定义
来源：http://gri.shanyushiyangtech.top

def add(a: Int, b: Int): Int = a + b
来源：http://zqs.ywan-chungtsiang.top

[T59] Scala：循环
来源：http://cyp.yj202588.top

for (i <- 1 to 10) println(i)
来源：http://zed.zycfv.cn

[T60] Scala：折叠
来源：http://vey.jianghu66.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://plo.dashuyun.cn

================================================================================
来源：http://msc.shzxlz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://efg.52xcode.cn

================================================================================
来源：http://pgo.jinqigfzy.top

[U01] Py：创建虚拟环境
来源：http://fdj.pengpengdd.cyou

python -m venv .venv && source .venv/bin/activate
来源：http://mud.aibaodan.cn

[U02] Py：导出 / 安装依赖
来源：http://xna.zhijiandao.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vnn.tianlin.xyz

[U03] Py：加载 .env 配置
来源：http://num.sufxvd.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mpg.yanxiufei.cn

[U04] Py：变量调试打印
来源：http://ycy.xylfe.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tbr.ybcxt.top

[U05] Py：列表去重且保序
来源：http://dch.shanyushiyangtech.top

list(dict.fromkeys(arr))
来源：http://wlg.jyoumei.cn

[U06] Py：合并两个字典
来源：http://dtd.cdnleiting.top

{**a, **b}
来源：http://qhe.tarul.cn

[U07] Py：反转字典键值
来源：http://tlo.ppjwa.cn

{v: k for k, v in d.items()}
来源：http://syn.andypj.xyz

[U08] Py：展平二维列表
来源：http://nis.hcnkem.com

[y for x in nested for y in x]
来源：http://xav.cucudq.cn

[U09] Py：字典取最大值的键
来源：http://vsh.zhijiandao.cn

max(d, key=d.get)
来源：http://bgk.yj202588.top

[U10] Py：按值排序字典
来源：http://eqi.sxryk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://onm.zhoulong.xyz

[U11] Py：生成器表达式
来源：http://meq.gzhubu.top

(x * 2 for x in arr)
来源：http://drt.hnqzz.top

[U12] Py：取出现最多的 3 个元素
来源：http://kwq.svipenyu.cn

Counter(arr).most_common(3)
来源：http://ess.gogol.net.cn

[U13] Py：固定长度队列
来源：http://mdy.jinyuanbaomall.cn

deque(maxlen=10)
来源：http://tqv.shangyingyoupin.top

[U14] Py：分组收集到列表
来源：http://wcg.hesvh.cn

defaultdict(list)
来源：http://uxw.tianlin.xyz

[U15] Py：高精度计时
来源：http://zue.xylfe.cn

t = time.perf_counter()
来源：http://moi.ivvv.top

[U16] Py：命令行参数解析
来源：http://hvw.gogol.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oem.daxiang520.top

[U17] Py：初始化日志
来源：http://jgq.guowangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://hes.jianghu66.top

[U18] Py：预编译正则
来源：http://sne.yangfankeji.com

pat = re.compile(r"\d+")
来源：http://ihd.zdbjq.cn

[U19] Py：正则替换带回调
来源：http://anj.snrcjt.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dxn.yj20258888.top

[U20] Py：缓存函数结果
来源：http://oja.jyoumei.cn

@functools.lru_cache(maxsize=None)
来源：http://nbg.hfpthk.cn

[U21] Py：自定义上下文管理器
来源：http://xep.jinqigfzy.top

@contextlib.contextmanager
来源：http://eld.fehbvm.com

[U22] Py：矩阵转置
来源：http://ley.jqgufenzy.top

list(zip(*m))
来源：http://sra.tanke756.top

[U23] Py：分块读取大文件
来源：http://iye.nwbrower.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://icu.havefunace.top

[U24] Py：路径操作
来源：http://ehi.jqgfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mku.tarul.cn

[U25] Py：CSV 按字典读
来源：http://bul.jiagoushi.top

csv.DictReader(f)
来源：http://ydw.xinyue.icu

[U26] Py：并发下载
来源：http://bvb.gotoacloud.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mqt.meibo888.top

[U27] Py：异步 HTTP
来源：http://asc.feifeiyinyue.top

aiohttp.ClientSession() 配合 async with
来源：http://ylw.fengsongda.top

[U28] Py：类型别名
来源：http://kni.ybcxt.top

UserId = int
来源：http://dko.gotoacloud.top

[U29] Py：属性校验
来源：http://hkw.sxryk.cn

@property 与 @x.setter 配合
来源：http://zfy.ehwqpu.com

[U30] Py：数据类
来源：http://ztp.shanyushiyangtech.top

@dataclass(slots=True)
来源：http://nxr.redwolf501.top

[U31] Py：单测
来源：http://fmr.wangdashe.top

python -m pytest -q
来源：http://vce.yvedp.cn

[U32] Py：代码格式化
来源：http://bxq.haohaochexian.top

ruff format . && ruff check --fix .
来源：http://ywx.zhijiandao.cn

[U33] Py：打包发布
来源：http://zvk.haohaochexian.top

python -m build  （依赖 pyproject.toml）
来源：http://tzj.xuanzx.com

[U34] Py：判断编码
来源：http://hel.xingfuxueyuan.xyz

chardet.detect(raw)
来源：http://uyf.feifeiyinyue.top

[U35] Py：发送邮件
来源：http://mnk.ydzc1.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jqw.jianghu66.top

[U36] Py：定时任务
来源：http://cum.hysaishi.cn

schedule.every(10).minutes.do(job)
来源：http://ybw.chenlongwang.top

[U37] Py：读写 Excel
来源：http://xed.zhixingplan.top

pandas.read_excel / DataFrame.to_excel
来源：http://qrq.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://tfv.daxiang520.top

Path(__file__).resolve().parent
来源：http://sgc.fanxiaobao.xyz

[U39] Py：判断是否在交互环境
来源：http://jai.gotoacloud.top

sys.stdout.isatty()
来源：http://xpj.epnwcf.com

[U40] Py：打印到标准错误
来源：http://htb.gogol.net.cn

print("err", file=sys.stderr)
来源：http://afp.yfazqb.com

[U41] PHP：初始化 Composer 项目
来源：http://cvv.chenjidiqi.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://bnr.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://iup.cashguo.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nhg.yangfankeji.com

[U43] PHP：声明命名空间
来源：http://rly.hammf.cn

namespace App\Http;
来源：http://yqn.hfpthk.cn

[U44] PHP：开启严格类型
来源：http://dpj.cheryme.top

declare(strict_types=1);
来源：http://dig.yuanzhike.top

[U45] PHP：类型声明与返回类型
来源：http://hvc.xingfuxueyuan.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://gwb.zhengqikj.top

[U46] PHP：可空类型
来源：http://bkp.pycfn.com

?string $name = null
来源：http://rlo.epnwcf.com

[U47] PHP：联合类型
来源：http://uzy.daxiang520.top

int|string $id
来源：http://uyn.fktsv.cn

[U48] PHP：纯枚举
来源：http://tsv.yuanzhike.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://isj.sysykeji.top

[U49] PHP：只读属性
来源：http://vhp.guannengcc.top

public readonly string $name
来源：http://ldh.fanxiaobao.xyz

[U50] PHP：构造器属性提升
来源：http://val.nwbrower.top

public function __construct(private int $id) {}
来源：http://opn.aizwys.cn

[U51] PHP：数组解构
来源：http://hgk.meibo888.top

[$a, $b] = $arr;
来源：http://pev.nwbrower.top

[U52] PHP：箭头函数
来源：http://dhg.sjlbkw.cn

$double = fn($x) => $x * 2;
来源：http://ptl.uphjek.com

[U53] PHP：空合并运算符
来源：http://bjc.wangdashe.top

$v = $a ?? $b ?? "default";
来源：http://quz.cheryme.top

[U54] PHP：空安全调用
来源：http://zdm.ivvv.top

$obj?->method()
来源：http://qhq.tian-w.cn

[U55] PHP：match 表达式
来源：http://uwq.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dyq.kuanghao11.cn

[U56] PHP：命名参数
来源：http://osb.hcnkem.com

f(a: 1, b: 2)
来源：http://jst.aibaodan.cn

[U57] PHP：字符串插值
来源：http://lvb.yongpay.top

"值: {$a}"
来源：http://dee.chenlongwang.top

[U58] PHP：数组三件套
来源：http://qtr.xylfe.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cej.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://jml.ydzc1.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gcg.yj20258.top

[U60] PHP：JSON 编解码
来源：http://cmi.dianchejie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kox.0kj1m.cn

[U61] PHP：正则
来源：http://oxe.quarkkingdee.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zfn.tian-w.cn

[U62] PHP：日期对象
来源：http://ote.tarul.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xya.xuanzx.com

[U63] PHP：文件读写
来源：http://eza.ywan-chungtsiang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://juu.meibo888.top

[U64] PHP：目录遍历
来源：http://mkx.dianchejie.cn

glob("dir/*.php");  scandir("dir");
来源：http://cxg.wangdashe.top

[U65] PHP：会话
来源：http://ntl.hfpthk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hjo.shzxlz.cn

[U66] PHP：设置 Cookie
来源：http://prg.birdmap.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ubb.dianchejie.cn

[U67] PHP：处理文件上传
来源：http://pfo.ydjk.org.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zai.fktsv.cn

[U68] PHP：PDO 连接
来源：http://jjj.cdnleiting.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ztg.yuxming.cn

[U69] PHP：PDO 预处理
来源：http://abx.zhijiandao.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nqx.ivvv.top

[U70] PHP：PDO 事务
来源：http://hsu.jinghuilouyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zts.jinqigfzy.top

[U71] PHP：抛出异常
来源：http://uob.daria6918.cn

throw new RuntimeException("失败", 500);
来源：http://odw.fzhhl.top

[U72] PHP：写错误日志
来源：http://iah.yuanzhike.top

error_log("失败: " . $e->getMessage());
来源：http://mkx.tanke756.top

[U73] PHP：读取 ini 配置
来源：http://rvu.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://jjs.gzhubu.top

[U74] PHP：读取环境变量
来源：http://evt.nanxuanxn.top

getenv("APP_ENV") ?: "production"
来源：http://bei.shanyushiyangtech.top

[U75] PHP：依赖注入
来源：http://mri.shanyushiyangkeji.top

composer require psr/container
来源：http://hmi.fengsongda.top

[U76] PHP：简单路由
来源：http://gnd.dianchejie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://boy.jinqigfzy.top

[U77] PHP：模板渲染
来源：http://mrq.ctjpmb.com

composer require twig/twig
来源：http://knz.316326.xyz

[U78] PHP：单元测试
来源：http://qjz.tian-w.cn

composer require --dev phpunit/phpunit
来源：http://udn.cqqwz.cn

[U79] PHP：静态分析
来源：http://mfg.pycfn.com

composer require --dev phpstan/phpstan
来源：http://bii.yuxming.cn

[U80] PHP：代码规范修复
来源：http://eyj.fktsv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yrh.cdnleiting.top

[U81] JS：初始化项目
来源：http://yyf.ctjpmb.com

npm init -y;  npm i express
来源：http://pjk.ydzc1.top

[U82] JS：package.json 脚本
来源：http://kkz.ivvv.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zuh.yfazqb.com

[U83] JS：ES Module 导入导出
来源：http://wov.ywan-chungtsiang.top

export const a = 1;  import { a } from "./m.js";
来源：http://qxp.cucudq.cn

[U84] JS：CommonJS 写法
来源：http://kia.jqgfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://rlt.jianghu66.top

[U85] JS：可选链
来源：http://lqx.xuetiantiany.cn

a?.b?.c
来源：http://qlw.yonumen.top

[U86] JS：空值合并
来源：http://wcw.fktsv.cn

a ?? b
来源：http://nik.nwbrower.top

[U87] JS：解构默认值
来源：http://zwx.hesvh.cn

const { a = 1, b = 2 } = obj;
来源：http://jjs.yj20258.top

[U88] JS：对象展开合并
来源：http://tnx.yj20258.top

{ ...a, ...b }
来源：http://ckg.hywenlv.cn

[U89] JS：数组去重
来源：http://puv.nanxinkj.top

[...new Set(arr)]
来源：http://lyf.quarkkingdee.top

[U90] JS：数字数组排序
来源：http://jzb.zhoulong.xyz

[...arr].sort((a, b) => a - b)
来源：http://fgv.iojbl.cn

[U91] JS：对象键值遍历
来源：http://tmo.vehdjk.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xmd.vehdjk.com

[U92] JS：深拷贝
来源：http://ftw.316326.xyz

structuredClone(obj)
来源：http://jia.9152youxi.cn

[U93] JS：模板字符串
来源：http://bvb.zdbjq.cn

`共 ${n} 条`
来源：http://rpt.zhiwuduotai.top

[U94] JS：箭头函数
来源：http://ldh.shanyushiyangtech.top

const double = x => x * 2;
来源：http://req.52xcode.cn

[U95] JS：Promise 包装
来源：http://oiv.jlsjyb.cn

new Promise((resolve, reject) => {})
来源：http://tzh.jlsjyb.cn

[U96] JS：async/await 与异常
来源：http://bjz.epnwcf.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xqb.jinqigufen.top

[U97] JS：并发请求
来源：http://jty.cqqwz.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://crz.cdnleiting.top

[U98] JS：fetch 带 JSON
来源：http://xmg.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://huc.yfazqb.com

[U99] JS：事件监听
来源：http://jss.jlsjyb.cn

el.addEventListener("click", e => {})
来源：http://fix.cashguo.top

[U100] JS：DOM 查询
来源：http://muj.hysaishi.cn

document.querySelector(".item")
来源：http://rkw.zhiwuduotai.top

[U101] JS：classList 操作
来源：http://irf.jlsjyb.cn

el.classList.toggle("active")
来源：http://kzn.mhx1999.top

[U102] JS：本地存储
来源：http://gbo.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://qsk.dianchejie.cn

[U103] JS：定时器
来源：http://csy.jlsjyb.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lbq.hesvh.cn

[U104] JS：防抖
来源：http://jhi.cdnleiting.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xet.shangyingyoupin.top

[U105] JS：节流
来源：http://ppe.chenjidiqi.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cxw.ydzc1.top

[U106] JS：日期格式化
来源：http://xgs.fktsv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://boo.xylfe.cn

[U107] JS：数字千分位
来源：http://xja.tarul.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fra.pycfn.com

[U108] JS：随机整数
来源：http://gva.ybcxt.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hqy.fehbvm.com

[U109] JS：数组分组
来源：http://awv.sysykeji.top

Object.groupBy(arr, x => x.type)
来源：http://aid.52xcode.cn

[U110] JS：数组分块
来源：http://swr.redwolf501.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hnm.sweek.top

[U111] JS：对象转 Map
来源：http://stf.feifeiyinyue.top

new Map(Object.entries(obj))
来源：http://prn.jqgfzy.top

[U112] JS：字符串补位
来源：http://hbt.hammf.cn

"7".padStart(3, "0")
来源：http://ykj.hesvh.cn

[U113] JS：正则替换全部
来源：http://gek.gzhubu.top

s.replaceAll("a", "b")
来源：http://ase.ydjk.org.cn

[U114] JS：JSON 深比较
来源：http://qoz.aibaodan.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://htc.zhoulong.xyz

[U115] JS：生成 UUID
来源：http://htz.nanxinkj.top

crypto.randomUUID()
来源：http://cqw.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://hvy.nanxinkj.top

/** @param {string} name */ function f(name) {}
来源：http://jtm.zhongyouzk.top

[U117] JS：单元测试
来源：http://rhc.chenjidiqi.icu

npm i -D vitest;  npx vitest
来源：http://ghr.hongshengwenyu.top

[U118] JS：开发服务器
来源：http://txj.yangfankeji.com

npm i -D vite;  npx vite
来源：http://dqw.hesvh.cn

[U119] JS：生产构建
来源：http://lzl.316326.xyz

npx vite build
来源：http://bve.yangfankeji.com

[U120] JS：读取环境变量（Vite）
来源：http://iny.yj20258.top

import.meta.env.VITE_API_URL
来源：http://cte.bbcook.cn

================================================================================
来源：http://btn.yonumen.top

统计汇总
来源：http://bjc.yvedp.cn

================================================================================
来源：http://mly.daria6918.cn

按语言统计（条）：
来源：http://bms.daria6918.cn

Python ......... 252
来源：http://otg.jianghu66.top

PHP ............ 252
来源：http://zzt.tianlin.xyz

JavaScript ..... 252
来源：http://xrb.yueranfly.top

TypeScript ..... 212
来源：http://nsv.zhengqikj.top

Java ........... 212
来源：http://xon.yvedp.cn

Go ............. 212
来源：http://lkh.gzhubu.top

Ruby ........... 212
来源：http://dse.hongshengwenyu.top

C# ............. 212
来源：http://tlm.cqqwz.cn

C .............. 30
来源：http://wkm.fengsongda.top

C++ ............ 30
来源：http://gdq.dashuyun.cn

SQL ............ 90
来源：http://ltx.hesvh.cn

Bash ........... 80
来源：http://qan.pycfn.com

Kotlin ......... 15
来源：http://cxd.ivvv.top

Swift .......... 15
来源：http://naq.zhijiandao.cn

Lua ............ 10
来源：http://ewf.xuetiantiany.cn

Perl ........... 10
来源：http://bti.gogol.net.cn

Scala .......... 10
来源：http://wjv.hcnkem.com

------------------------------------
来源：http://tyj.iojbl.cn

合计 ........... 2106 条
来源：http://phs.shangyingyoupin.top

按章节统计：
来源：http://irg.c1oappe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kwu.jyoumei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wvq.xylfe.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://abe.nanxuanxn.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://amq.zycfv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gug.xylfe.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ccq.fehbvm.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rtr.yanxiufei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://utl.meibo888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rjb.chenzaomai.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://huz.zhoulong.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vol.gzhubu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qvb.xinyue.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vsi.shzxlz.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jqx.zhoulong.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://chz.chenzaomai.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xos.jinghuilouyu.cn


<!-- 参考信息 -->