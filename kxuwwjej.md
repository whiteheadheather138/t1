代发 wailian999

case class User(name: String, age: Int)
来源：http://kga.hfpthk.cn

[T57] Scala：模式匹配
来源：http://soh.meibo888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jph.yuxming.cn

[T58] Scala：函数定义
来源：http://hit.gotoacloud.top

def add(a: Int, b: Int): Int = a + b
来源：http://bgv.pycfn.com

[T59] Scala：循环
来源：http://ret.yfazqb.com

for (i <- 1 to 10) println(i)
来源：http://qse.feifeiyinyue.top

[T60] Scala：折叠
来源：http://hpg.chenjidiqi.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bzd.zdqjudy.top

================================================================================
来源：http://yga.tianlin.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fgd.tarul.cn

================================================================================
来源：http://mam.kuanghao11.cn

[U01] Py：创建虚拟环境
来源：http://gst.cdnleiting.top

python -m venv .venv && source .venv/bin/activate
来源：http://rsd.jyoumei.cn

[U02] Py：导出 / 安装依赖
来源：http://ggr.zdqjudy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gxb.bbcook.cn

[U03] Py：加载 .env 配置
来源：http://rna.shanyushiyangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qbk.gotoacloud.top

[U04] Py：变量调试打印
来源：http://ghc.zhoulong.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vnt.316326.xyz

[U05] Py：列表去重且保序
来源：http://dpa.zhongyouzk.top

list(dict.fromkeys(arr))
来源：http://hwq.nanxinkj.top

[U06] Py：合并两个字典
来源：http://nko.hesvh.cn

{**a, **b}
来源：http://wia.vehdjk.com

[U07] Py：反转字典键值
来源：http://abk.meibo888.top

{v: k for k, v in d.items()}
来源：http://fzt.jyoumei.cn

[U08] Py：展平二维列表
来源：http://xzl.hfpthk.cn

[y for x in nested for y in x]
来源：http://bul.yuxming.cn

[U09] Py：字典取最大值的键
来源：http://yjs.bjfxy.top

max(d, key=d.get)
来源：http://yjj.svipenyu.cn

[U10] Py：按值排序字典
来源：http://sxj.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jdp.0kj1m.cn

[U11] Py：生成器表达式
来源：http://gwp.tianlin.xyz

(x * 2 for x in arr)
来源：http://bzc.uphjek.com

[U12] Py：取出现最多的 3 个元素
来源：http://swz.sjlbkw.cn

Counter(arr).most_common(3)
来源：http://rsc.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://rwt.zhongyouzk.top

deque(maxlen=10)
来源：http://atg.daria6918.cn

[U14] Py：分组收集到列表
来源：http://wgc.daria6918.cn

defaultdict(list)
来源：http://hmv.haohaochexian.top

[U15] Py：高精度计时
来源：http://wqq.cashguo.top

t = time.perf_counter()
来源：http://lgh.yj20258.top

[U16] Py：命令行参数解析
来源：http://yst.pengpengdd.cyou

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lje.cashguo.top

[U17] Py：初始化日志
来源：http://bpg.xuanzx.com

logging.basicConfig(level=logging.INFO)
来源：http://zbc.hongshengwenyu.top

[U18] Py：预编译正则
来源：http://kae.316326.xyz

pat = re.compile(r"\d+")
来源：http://bsy.kuanghao11.cn

[U19] Py：正则替换带回调
来源：http://qgo.snrcjt.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sqa.jiagoushi.top

[U20] Py：缓存函数结果
来源：http://nux.xingfuxueyuan.xyz

@functools.lru_cache(maxsize=None)
来源：http://vyh.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://ioq.chenzaomai.com

@contextlib.contextmanager
来源：http://cfq.feifeiyinyue.top

[U22] Py：矩阵转置
来源：http://ens.gaohongyu789.top

list(zip(*m))
来源：http://ddj.cashguo.top

[U23] Py：分块读取大文件
来源：http://iex.xuanzx.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yps.ybcxt.top

[U24] Py：路径操作
来源：http://ysz.jlsjyb.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sri.cheryme.top

[U25] Py：CSV 按字典读
来源：http://gdk.hnxiangtu.top

csv.DictReader(f)
来源：http://bdo.cdnleiting.top

[U26] Py：并发下载
来源：http://nad.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ism.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://dhf.zhiwuduotai.top

aiohttp.ClientSession() 配合 async with
来源：http://wgd.wangdashe.top

[U28] Py：类型别名
来源：http://qfs.hysaishi.cn

UserId = int
来源：http://emb.shanyushiyangkeji.top

[U29] Py：属性校验
来源：http://mhg.smart0.xyz

@property 与 @x.setter 配合
来源：http://mli.yj20258888.top

[U30] Py：数据类
来源：http://zsp.yueranfly.top

@dataclass(slots=True)
来源：http://flj.iojbl.cn

[U31] Py：单测
来源：http://eyj.ehwqpu.com

python -m pytest -q
来源：http://lqo.sysykeji.top

[U32] Py：代码格式化
来源：http://akz.yonumen.top

ruff format . && ruff check --fix .
来源：http://ddz.jqgufenzy.top

[U33] Py：打包发布
来源：http://qhv.yj20258.top

python -m build  （依赖 pyproject.toml）
来源：http://dse.xuetiantiany.cn

[U34] Py：判断编码
来源：http://xvg.shangyingyoupin.top

chardet.detect(raw)
来源：http://mfm.jinghuilouyu.cn

[U35] Py：发送邮件
来源：http://jou.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rbp.gaohongyu789.top

[U36] Py：定时任务
来源：http://cyk.yvedp.cn

schedule.every(10).minutes.do(job)
来源：http://sxg.yueranfly.top

[U37] Py：读写 Excel
来源：http://piu.jinghuilouyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jqu.meibo888.top

[U38] Py：获取脚本所在目录
来源：http://but.yuxming.cn

Path(__file__).resolve().parent
来源：http://zdv.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://vns.ppjwa.cn

sys.stdout.isatty()
来源：http://wpb.vehdjk.com

[U40] Py：打印到标准错误
来源：http://jvg.hongshengwenyu.top

print("err", file=sys.stderr)
来源：http://esv.tian-w.cn

[U41] PHP：初始化 Composer 项目
来源：http://ueo.ywan-chungtsiang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://eax.yj20258888.top

[U42] PHP：PSR-4 自动加载
来源：http://hng.havefunace.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ulj.chenjidiqi.icu

[U43] PHP：声明命名空间
来源：http://jpd.tarul.cn

namespace App\Http;
来源：http://bfc.xingfuxueyuan.xyz

[U44] PHP：开启严格类型
来源：http://mku.smart0.xyz

declare(strict_types=1);
来源：http://wqq.shanyushiyangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://eea.ybcxt.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://bkk.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://xqw.yangfankeji.com

?string $name = null
来源：http://pdd.zdqjudy.top

[U47] PHP：联合类型
来源：http://uzx.zdqjudy.top

int|string $id
来源：http://fde.bbcook.cn

[U48] PHP：纯枚举
来源：http://way.xingfuxueyuan.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hak.yuxming.cn

[U49] PHP：只读属性
来源：http://vtb.hcnkem.com

public readonly string $name
来源：http://klk.uphjek.com

[U50] PHP：构造器属性提升
来源：http://sjv.yongpay.top

public function __construct(private int $id) {}
来源：http://ann.9152youxi.cn

[U51] PHP：数组解构
来源：http://xyk.fengsongda.top

[$a, $b] = $arr;
来源：http://lbk.yj20258888.top

[U52] PHP：箭头函数
来源：http://qab.9152youxi.cn

$double = fn($x) => $x * 2;
来源：http://jir.zycfv.cn

[U53] PHP：空合并运算符
来源：http://dln.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://xet.yj20258888.top

[U54] PHP：空安全调用
来源：http://cok.svipenyu.cn

$obj?->method()
来源：http://pyw.zdbjq.cn

[U55] PHP：match 表达式
来源：http://zfd.gogol.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nla.gaohongyu789.top

[U56] PHP：命名参数
来源：http://rjm.xuanzx.com

f(a: 1, b: 2)
来源：http://jav.ctjpmb.com

[U57] PHP：字符串插值
来源：http://fzd.sxryk.cn

"值: {$a}"
来源：http://gnz.feifeiyinyue.top

[U58] PHP：数组三件套
来源：http://zud.hammf.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://guu.cdnleiting.top

[U59] PHP：自定义排序
来源：http://dva.hcnkem.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ucy.xingfuxueyuan.xyz

[U60] PHP：JSON 编解码
来源：http://sfp.sjlbkw.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mvx.kuanghao11.cn

[U61] PHP：正则
来源：http://jga.xziqi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mon.zhongyouzk.top

[U62] PHP：日期对象
来源：http://rbl.gogol.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mff.yfazqb.com

[U63] PHP：文件读写
来源：http://vqz.meibo888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ujb.fengsongda.top

[U64] PHP：目录遍历
来源：http://zra.iojbl.cn

glob("dir/*.php");  scandir("dir");
来源：http://yfc.daria6918.cn

[U65] PHP：会话
来源：http://rzb.cdnleiting.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lpg.hammf.cn

[U66] PHP：设置 Cookie
来源：http://ekz.zhengqikj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pad.sufxvd.cn

[U67] PHP：处理文件上传
来源：http://zds.epnwcf.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fen.hcnkem.com

[U68] PHP：PDO 连接
来源：http://ftg.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gaa.xuanzx.com

[U69] PHP：PDO 预处理
来源：http://iox.xinyue.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xyl.hysaishi.cn

[U70] PHP：PDO 事务
来源：http://zzi.yj20258888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wbg.yanxiufei.cn

[U71] PHP：抛出异常
来源：http://knf.pycfn.com

throw new RuntimeException("失败", 500);
来源：http://ojg.xinyue.icu

[U72] PHP：写错误日志
来源：http://lnv.chenlongwang.top

error_log("失败: " . $e->getMessage());
来源：http://cbq.jlsjyb.cn

[U73] PHP：读取 ini 配置
来源：http://ugu.yonumen.top

parse_ini_file("config.ini", true)
来源：http://ebt.hywenlv.cn

[U74] PHP：读取环境变量
来源：http://kvz.daxiang520.top

getenv("APP_ENV") ?: "production"
来源：http://qrm.jinqigufen.top

[U75] PHP：依赖注入
来源：http://pbm.zhiwuduotai.top

composer require psr/container
来源：http://ksi.xingfuxueyuan.xyz

[U76] PHP：简单路由
来源：http://umo.yfazqb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eer.yongpay.top

[U77] PHP：模板渲染
来源：http://xkv.pycfn.com

composer require twig/twig
来源：http://pnx.fengsongda.top

[U78] PHP：单元测试
来源：http://zjw.kuanghao11.cn

composer require --dev phpunit/phpunit
来源：http://hev.chenlongwang.top

[U79] PHP：静态分析
来源：http://tun.jinqigufen.top

composer require --dev phpstan/phpstan
来源：http://ogy.xingfuxueyuan.xyz

[U80] PHP：代码规范修复
来源：http://eoq.aizwys.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://iad.xylfe.cn

[U81] JS：初始化项目
来源：http://dkb.shzxlz.cn

npm init -y;  npm i express
来源：http://jtq.tarul.cn

[U82] JS：package.json 脚本
来源：http://kts.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gyk.hnqzz.top

[U83] JS：ES Module 导入导出
来源：http://zud.yongpay.top

export const a = 1;  import { a } from "./m.js";
来源：http://uaw.shzxlz.cn

[U84] JS：CommonJS 写法
来源：http://avf.haohaochexian.top

module.exports = { a };  const { a } = require("./m");
来源：http://rlq.hongshengwenyu.top

[U85] JS：可选链
来源：http://zwt.jianghu66.top

a?.b?.c
来源：http://ddn.zhixingplan.top

[U86] JS：空值合并
来源：http://ufr.tian-w.cn

a ?? b
来源：http://yox.andypj.xyz

[U87] JS：解构默认值
来源：http://xbp.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://sse.yonumen.top

[U88] JS：对象展开合并
来源：http://wzr.hfpthk.cn

{ ...a, ...b }
来源：http://nlo.daxiang520.top

[U89] JS：数组去重
来源：http://xrm.bjfxy.top

[...new Set(arr)]
来源：http://slp.fanxiaobao.xyz

[U90] JS：数字数组排序
来源：http://xze.yj202588.top

[...arr].sort((a, b) => a - b)
来源：http://aoc.pengpengdd.cyou

[U91] JS：对象键值遍历
来源：http://foo.fanxiaobao.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rqg.yfazqb.com

[U92] JS：深拷贝
来源：http://wkn.yueranfly.top

structuredClone(obj)
来源：http://mso.jianghu66.top

[U93] JS：模板字符串
来源：http://sdq.fengsongda.top

`共 ${n} 条`
来源：http://wex.meibo888.top

[U94] JS：箭头函数
来源：http://xfm.zhongyouzk.top

const double = x => x * 2;
来源：http://lbp.pengpengdd.cyou

[U95] JS：Promise 包装
来源：http://api.dashuyun.cn

new Promise((resolve, reject) => {})
来源：http://rit.jianghu66.top

[U96] JS：async/await 与异常
来源：http://fxc.cucudq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hvj.mhx1999.top

[U97] JS：并发请求
来源：http://bza.yueranfly.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mcy.cucudq.cn

[U98] JS：fetch 带 JSON
来源：http://pva.shangyingyoupin.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zpv.sweek.top

[U99] JS：事件监听
来源：http://wyt.jianghu66.top

el.addEventListener("click", e => {})
来源：http://hbt.316326.xyz

[U100] JS：DOM 查询
来源：http://qun.nanxinkj.top

document.querySelector(".item")
来源：http://tig.ivvv.top

[U101] JS：classList 操作
来源：http://inq.shangyingyoupin.top

el.classList.toggle("active")
来源：http://ybi.snrcjt.cn

[U102] JS：本地存储
来源：http://smc.wangshuangyany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ewt.mhx1999.top

[U103] JS：定时器
来源：http://ndv.yangfankeji.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ydc.smart0.xyz

[U104] JS：防抖
来源：http://mwr.kuanghao11.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gcp.jqgufenzy.top

[U105] JS：节流
来源：http://wha.yanxiufei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jcs.zhijiandao.cn

[U106] JS：日期格式化
来源：http://hpm.fktsv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://suu.bbcook.cn

[U107] JS：数字千分位
来源：http://odf.jinghuilouyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fag.dianchejie.cn

[U108] JS：随机整数
来源：http://kps.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eqw.ydzc1.top

[U109] JS：数组分组
来源：http://uiq.aibaodan.cn

Object.groupBy(arr, x => x.type)
来源：http://dlj.gaohongyu789.top

[U110] JS：数组分块
来源：http://kze.xylfe.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nrk.52xcode.cn

[U111] JS：对象转 Map
来源：http://njg.jianghu66.top

new Map(Object.entries(obj))
来源：http://lyg.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://iti.yj20258.top

"7".padStart(3, "0")
来源：http://mgm.ivvv.top

[U113] JS：正则替换全部
来源：http://jqq.pengpengdd.cyou

s.replaceAll("a", "b")
来源：http://rtp.tarul.cn

[U114] JS：JSON 深比较
来源：http://zvv.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://onz.hfpthk.cn

[U115] JS：生成 UUID
来源：http://uht.gogol.net.cn

crypto.randomUUID()
来源：http://duz.xuanzx.com

[U116] JS：类型检查（JSDoc）
来源：http://hec.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://ezl.yj202588.top

[U117] JS：单元测试
来源：http://cfj.zhongyouzk.top

npm i -D vitest;  npx vitest
来源：http://qtp.sysykeji.top

[U118] JS：开发服务器
来源：http://lye.aizwys.cn

npm i -D vite;  npx vite
来源：http://spq.bbcook.cn

[U119] JS：生产构建
来源：http://uty.jqgufenzy.top

npx vite build
来源：http://yqh.shanyushiyangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://azx.bjfxy.top

import.meta.env.VITE_API_URL
来源：http://agu.xylfe.cn

================================================================================
来源：http://ccv.yangfankeji.com

统计汇总
来源：http://pik.fktsv.cn

================================================================================
来源：http://dji.c1oappe.top

按语言统计（条）：
来源：http://ezh.yanxiufei.cn

Python ......... 252
来源：http://gbs.vehdjk.com

PHP ............ 252
来源：http://lzm.shuidangran.top

JavaScript ..... 252
来源：http://fwh.jinyuanbaomall.cn

TypeScript ..... 212
来源：http://auo.kuanghao11.cn

Java ........... 212
来源：http://xrk.jlsjyb.cn

Go ............. 212
来源：http://azp.ctjpmb.com

Ruby ........... 212
来源：http://fbj.epnwcf.com

C# ............. 212
来源：http://aam.shuidangran.top

C .............. 30
来源：http://iou.hammf.cn

C++ ............ 30
来源：http://had.tianlin.xyz

SQL ............ 90
来源：http://xwd.aizwys.cn

Bash ........... 80
来源：http://bee.shuidangran.top

Kotlin ......... 15
来源：http://xbq.vehdjk.com

Swift .......... 15
来源：http://hse.pengpengdd.cyou

Lua ............ 10
来源：http://dhw.kuanghao11.cn

Perl ........... 10
来源：http://hha.birdmap.top

Scala .......... 10
来源：http://awx.kuanghao11.cn

------------------------------------
来源：http://qsk.smart0.xyz

合计 ........... 2106 条
来源：http://gnp.pengpengdd.cyou

按章节统计：
来源：http://jea.guowangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nub.jinqigufen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fif.yvedp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bjd.shangyingyoupin.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vsu.sxryk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://exh.sxryk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vgd.bjfxy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fzf.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://reg.yueranfly.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nov.xinyue.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dfe.xuetiantiany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nzc.zhijiandao.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dbt.9152youxi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://akx.redwolf501.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://txn.smart0.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cjk.jqgfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://auh.shuidangran.top

Q SQL 专题                              90
来源：http://fbl.hongshengwenyu.top

R Bash 专题                             80
来源：http://jfs.hnxiangtu.top

S C / C++ 专题                          60
来源：http://gdv.guannengcc.top

T 其他语言补充                          60
来源：http://yvv.zhengqikj.top

U 高频实用片段                         120
来源：http://wvf.cqqwz.cn

------------------------------------
来源：http://vxb.chenjidiqi.icu

合计                                  2106 条
来源：http://scq.xziqi.cn

--------------------------------------------------------------------------------
来源：http://vwm.daxiang520.top


<!-- 参考信息 -->