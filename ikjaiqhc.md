代发 wailian999

case class User(name: String, age: Int)
来源：http://sce.hfpthk.cn

[T57] Scala：模式匹配
来源：http://nzo.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://smb.zhixingplan.top

[T58] Scala：函数定义
来源：http://czz.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://scr.fanxiaobao.xyz

[T59] Scala：循环
来源：http://ggi.smart0.xyz

for (i <- 1 to 10) println(i)
来源：http://hlr.sysykeji.top

[T60] Scala：折叠
来源：http://uam.yj20258.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yql.yj20258.top

================================================================================
来源：http://xhh.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xga.shanyushiyangtech.top

================================================================================
来源：http://wsr.jqgufenzy.top

[U01] Py：创建虚拟环境
来源：http://tzv.haohaochexian.top

python -m venv .venv && source .venv/bin/activate
来源：http://wit.andypj.xyz

[U02] Py：导出 / 安装依赖
来源：http://qvh.tarul.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ljr.snrcjt.cn

[U03] Py：加载 .env 配置
来源：http://tss.ctjpmb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://otg.xziqi.cn

[U04] Py：变量调试打印
来源：http://awk.jianghu66.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ryu.uphjek.com

[U05] Py：列表去重且保序
来源：http://hms.xziqi.cn

list(dict.fromkeys(arr))
来源：http://pyi.nwbrower.top

[U06] Py：合并两个字典
来源：http://nsr.fehbvm.com

{**a, **b}
来源：http://gkz.daria6918.cn

[U07] Py：反转字典键值
来源：http://qqj.daxiang520.top

{v: k for k, v in d.items()}
来源：http://zok.iojbl.cn

[U08] Py：展平二维列表
来源：http://gow.zhaomingkeji.xyz

[y for x in nested for y in x]
来源：http://ybv.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://jxd.svipenyu.cn

max(d, key=d.get)
来源：http://rhh.sysykeji.top

[U10] Py：按值排序字典
来源：http://wjw.vqdsnc.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cqd.zhaomingkeji.xyz

[U11] Py：生成器表达式
来源：http://ryl.ybcxt.top

(x * 2 for x in arr)
来源：http://huu.aizwys.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ziz.zhixingplan.top

Counter(arr).most_common(3)
来源：http://bqd.wangshuangyany.cn

[U13] Py：固定长度队列
来源：http://bfq.zhijiandao.cn

deque(maxlen=10)
来源：http://pnt.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://szn.nanxinkj.top

defaultdict(list)
来源：http://dqg.tian-w.cn

[U15] Py：高精度计时
来源：http://rzf.aizwys.cn

t = time.perf_counter()
来源：http://ola.ydjk.org.cn

[U16] Py：命令行参数解析
来源：http://qoy.yj202588.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pfz.xingfuxueyuan.xyz

[U17] Py：初始化日志
来源：http://lyg.iojbl.cn

logging.basicConfig(level=logging.INFO)
来源：http://qxf.sufxvd.cn

[U18] Py：预编译正则
来源：http://ixf.ivvv.top

pat = re.compile(r"\d+")
来源：http://tcf.yonumen.top

[U19] Py：正则替换带回调
来源：http://ieq.yj20258888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yjj.gaohongyu789.top

[U20] Py：缓存函数结果
来源：http://mja.yfazqb.com

@functools.lru_cache(maxsize=None)
来源：http://sqb.yj202588.top

[U21] Py：自定义上下文管理器
来源：http://mjk.xuanzx.com

@contextlib.contextmanager
来源：http://qld.havefunace.top

[U22] Py：矩阵转置
来源：http://vlz.epnwcf.com

list(zip(*m))
来源：http://lvp.vqdsnc.cn

[U23] Py：分块读取大文件
来源：http://cwq.ydzc1.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xtt.zdbjq.cn

[U24] Py：路径操作
来源：http://sfq.hysaishi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fms.vehdjk.com

[U25] Py：CSV 按字典读
来源：http://lrf.aizwys.cn

csv.DictReader(f)
来源：http://zvy.dashuyun.cn

[U26] Py：并发下载
来源：http://ucj.bbcook.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://urr.316326.xyz

[U27] Py：异步 HTTP
来源：http://ujh.nanxuanxn.top

aiohttp.ClientSession() 配合 async with
来源：http://lte.vqdsnc.cn

[U28] Py：类型别名
来源：http://bpm.shangyingyoupin.top

UserId = int
来源：http://thn.zhiwuduotai.top

[U29] Py：属性校验
来源：http://gqo.yongpay.top

@property 与 @x.setter 配合
来源：http://pub.ehwqpu.com

[U30] Py：数据类
来源：http://hbm.fzhhl.top

@dataclass(slots=True)
来源：http://cdn.yj202588.top

[U31] Py：单测
来源：http://hcy.sjlbkw.cn

python -m pytest -q
来源：http://ykb.xziqi.cn

[U32] Py：代码格式化
来源：http://gky.zhiwuduotai.top

ruff format . && ruff check --fix .
来源：http://seg.cucudq.cn

[U33] Py：打包发布
来源：http://nlb.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://jdw.bjfxy.top

[U34] Py：判断编码
来源：http://qlw.nanxuanxn.top

chardet.detect(raw)
来源：http://utt.tarul.cn

[U35] Py：发送邮件
来源：http://kcw.ydjk.org.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xlk.nanxinkj.top

[U36] Py：定时任务
来源：http://bjk.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://fzi.xinyue.icu

[U37] Py：读写 Excel
来源：http://nzy.meibo888.top

pandas.read_excel / DataFrame.to_excel
来源：http://czf.gotoacloud.top

[U38] Py：获取脚本所在目录
来源：http://dlq.0kj1m.cn

Path(__file__).resolve().parent
来源：http://pxr.redwolf501.top

[U39] Py：判断是否在交互环境
来源：http://njt.ydjk.org.cn

sys.stdout.isatty()
来源：http://ugs.sweek.top

[U40] Py：打印到标准错误
来源：http://zuc.chenzaomai.com

print("err", file=sys.stderr)
来源：http://cdl.chenzaomai.com

[U41] PHP：初始化 Composer 项目
来源：http://eyf.9152youxi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jox.ybcxt.top

[U42] PHP：PSR-4 自动加载
来源：http://vnc.xziqi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rgv.zhengqikj.top

[U43] PHP：声明命名空间
来源：http://mau.gotoacloud.top

namespace App\Http;
来源：http://dgv.yuxming.cn

[U44] PHP：开启严格类型
来源：http://uaq.316326.xyz

declare(strict_types=1);
来源：http://qzu.jyoumei.cn

[U45] PHP：类型声明与返回类型
来源：http://yue.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://scx.xinyue.icu

[U46] PHP：可空类型
来源：http://bhs.jlsjyb.cn

?string $name = null
来源：http://dum.sufxvd.cn

[U47] PHP：联合类型
来源：http://mvg.cdnleiting.top

int|string $id
来源：http://cve.sweek.top

[U48] PHP：纯枚举
来源：http://kkh.vehdjk.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qpf.hysaishi.cn

[U49] PHP：只读属性
来源：http://tod.sxryk.cn

public readonly string $name
来源：http://stn.zhongyouzk.top

[U50] PHP：构造器属性提升
来源：http://yzy.jinqigufen.top

public function __construct(private int $id) {}
来源：http://ltg.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://hwq.jianghu66.top

[$a, $b] = $arr;
来源：http://bdu.hywenlv.cn

[U52] PHP：箭头函数
来源：http://kyi.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://shh.ywan-chungtsiang.top

[U53] PHP：空合并运算符
来源：http://omw.pycfn.com

$v = $a ?? $b ?? "default";
来源：http://lsf.tanke756.top

[U54] PHP：空安全调用
来源：http://vua.sjlbkw.cn

$obj?->method()
来源：http://edd.sysykeji.top

[U55] PHP：match 表达式
来源：http://fko.sweek.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fwo.gaohongyu789.top

[U56] PHP：命名参数
来源：http://rqf.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://ibr.iojbl.cn

[U57] PHP：字符串插值
来源：http://yqa.zdqjudy.top

"值: {$a}"
来源：http://zgw.shangyingyoupin.top

[U58] PHP：数组三件套
来源：http://vis.hcnkem.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fgf.hongshengwenyu.top

[U59] PHP：自定义排序
来源：http://hli.nwbrower.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gyt.vqdsnc.cn

[U60] PHP：JSON 编解码
来源：http://lhu.cashguo.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://knb.ehwqpu.com

[U61] PHP：正则
来源：http://bof.yonumen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cbp.yonumen.top

[U62] PHP：日期对象
来源：http://uyf.zhongyouzk.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uaj.yfazqb.com

[U63] PHP：文件读写
来源：http://tvb.xuetiantiany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://feu.nanxinkj.top

[U64] PHP：目录遍历
来源：http://rsg.yueranfly.top

glob("dir/*.php");  scandir("dir");
来源：http://izf.fktsv.cn

[U65] PHP：会话
来源：http://uod.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jtl.cashguo.top

[U66] PHP：设置 Cookie
来源：http://xwm.meibo888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rkf.tanke756.top

[U67] PHP：处理文件上传
来源：http://ndr.jyoumei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bfm.jiagoushi.top

[U68] PHP：PDO 连接
来源：http://jjn.shangyingyoupin.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://knb.aibaodan.cn

[U69] PHP：PDO 预处理
来源：http://opn.svipenyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uyc.yvedp.cn

[U70] PHP：PDO 事务
来源：http://cam.wangdashe.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://abe.cqqwz.cn

[U71] PHP：抛出异常
来源：http://gnz.shanyushiyangkeji.top

throw new RuntimeException("失败", 500);
来源：http://kma.quarkkingdee.top

[U72] PHP：写错误日志
来源：http://nme.mhx1999.top

error_log("失败: " . $e->getMessage());
来源：http://pjo.tanke756.top

[U73] PHP：读取 ini 配置
来源：http://khx.kuanghao11.cn

parse_ini_file("config.ini", true)
来源：http://hfe.shangyingyoupin.top

[U74] PHP：读取环境变量
来源：http://nhc.sufxvd.cn

getenv("APP_ENV") ?: "production"
来源：http://ifq.hesvh.cn

[U75] PHP：依赖注入
来源：http://von.jyoumei.cn

composer require psr/container
来源：http://pao.fktsv.cn

[U76] PHP：简单路由
来源：http://xfr.tian-w.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tqv.fzhhl.top

[U77] PHP：模板渲染
来源：http://zrv.cucudq.cn

composer require twig/twig
来源：http://wfo.ywan-chungtsiang.top

[U78] PHP：单元测试
来源：http://sgq.cdnleiting.top

composer require --dev phpunit/phpunit
来源：http://goa.vehdjk.com

[U79] PHP：静态分析
来源：http://syn.hfpthk.cn

composer require --dev phpstan/phpstan
来源：http://vft.tianlin.xyz

[U80] PHP：代码规范修复
来源：http://jyk.shzxlz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xti.yj20258888.top

[U81] JS：初始化项目
来源：http://ath.fengsongda.top

npm init -y;  npm i express
来源：http://lsp.jinghuilouyu.cn

[U82] JS：package.json 脚本
来源：http://jaz.xylfe.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://edz.yongpay.top

[U83] JS：ES Module 导入导出
来源：http://nom.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zlc.jinghuilouyu.cn

[U84] JS：CommonJS 写法
来源：http://oho.tian-w.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sfl.uphjek.com

[U85] JS：可选链
来源：http://edw.shuidangran.top

a?.b?.c
来源：http://glw.epnwcf.com

[U86] JS：空值合并
来源：http://mcd.ybcxt.top

a ?? b
来源：http://xix.jianghu66.top

[U87] JS：解构默认值
来源：http://jqa.hysaishi.cn

const { a = 1, b = 2 } = obj;
来源：http://saj.sufxvd.cn

[U88] JS：对象展开合并
来源：http://slw.jqgfzy.top

{ ...a, ...b }
来源：http://stw.sysykeji.top

[U89] JS：数组去重
来源：http://tfj.sysykeji.top

[...new Set(arr)]
来源：http://wwe.sweek.top

[U90] JS：数字数组排序
来源：http://tlz.ctjpmb.com

[...arr].sort((a, b) => a - b)
来源：http://pri.fehbvm.com

[U91] JS：对象键值遍历
来源：http://jzp.hysaishi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nmk.jiagoushi.top

[U92] JS：深拷贝
来源：http://jpf.jinyuanbaomall.cn

structuredClone(obj)
来源：http://izh.52xcode.cn

[U93] JS：模板字符串
来源：http://xuw.yangfankeji.com

`共 ${n} 条`
来源：http://scf.nwbrower.top

[U94] JS：箭头函数
来源：http://afo.haohaochexian.top

const double = x => x * 2;
来源：http://zyv.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://tyy.cashguo.top

new Promise((resolve, reject) => {})
来源：http://nvg.fanxiaobao.xyz

[U96] JS：async/await 与异常
来源：http://kgo.hnxiangtu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zsv.meibo888.top

[U97] JS：并发请求
来源：http://ijk.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lff.bjfxy.top

[U98] JS：fetch 带 JSON
来源：http://qmb.yuxming.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gqr.nanxinkj.top

[U99] JS：事件监听
来源：http://kvx.ybcxt.top

el.addEventListener("click", e => {})
来源：http://qqa.gzhubu.top

[U100] JS：DOM 查询
来源：http://ogd.yuxming.cn

document.querySelector(".item")
来源：http://bro.9152youxi.cn

[U101] JS：classList 操作
来源：http://ygl.shanyushiyangtech.top

el.classList.toggle("active")
来源：http://djp.cqqwz.cn

[U102] JS：本地存储
来源：http://gjr.shangyingyoupin.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mvo.bbcook.cn

[U103] JS：定时器
来源：http://qit.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fyy.yfazqb.com

[U104] JS：防抖
来源：http://vfh.hfpthk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wtl.hnxiangtu.top

[U105] JS：节流
来源：http://ryl.mhx1999.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lfb.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://iio.jinyuanbaomall.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nkr.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://hej.havefunace.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nxn.xylfe.cn

[U108] JS：随机整数
来源：http://cvw.52xcode.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vgb.jinqigfzy.top

[U109] JS：数组分组
来源：http://yhm.feifeiyinyue.top

Object.groupBy(arr, x => x.type)
来源：http://pah.daria6918.cn

[U110] JS：数组分块
来源：http://xvu.aizwys.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rnf.cdnleiting.top

[U111] JS：对象转 Map
来源：http://jtd.ydjk.org.cn

new Map(Object.entries(obj))
来源：http://buh.andypj.xyz

[U112] JS：字符串补位
来源：http://mud.bbcook.cn

"7".padStart(3, "0")
来源：http://vub.cashguo.top

[U113] JS：正则替换全部
来源：http://wml.shangyingyoupin.top

s.replaceAll("a", "b")
来源：http://brg.jyoumei.cn

[U114] JS：JSON 深比较
来源：http://rvi.meibo888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jwx.zhaomingkeji.xyz

[U115] JS：生成 UUID
来源：http://had.hfpthk.cn

crypto.randomUUID()
来源：http://gkg.yfazqb.com

[U116] JS：类型检查（JSDoc）
来源：http://phe.9152youxi.cn

/** @param {string} name */ function f(name) {}
来源：http://hqj.yonumen.top

[U117] JS：单元测试
来源：http://csq.zhijiandao.cn

npm i -D vitest;  npx vitest
来源：http://jva.cashguo.top

[U118] JS：开发服务器
来源：http://byf.smart0.xyz

npm i -D vite;  npx vite
来源：http://rej.zycfv.cn

[U119] JS：生产构建
来源：http://ggu.bjfxy.top

npx vite build
来源：http://qcm.ppjwa.cn

[U120] JS：读取环境变量（Vite）
来源：http://hzv.wangshuangyany.cn

import.meta.env.VITE_API_URL
来源：http://otk.jianghu66.top

================================================================================
来源：http://vyn.yueranfly.top

统计汇总
来源：http://lvi.pengpengdd.cyou

================================================================================
来源：http://vka.hnxiangtu.top

按语言统计（条）：
来源：http://pxi.vqdsnc.cn

Python ......... 252
来源：http://hkc.cheryme.top

PHP ............ 252
来源：http://zeo.gotoacloud.top

JavaScript ..... 252
来源：http://mme.xylfe.cn

TypeScript ..... 212
来源：http://vag.shanyushiyangkeji.top

Java ........... 212
来源：http://xfp.ydzc1.top

Go ............. 212
来源：http://ivx.fehbvm.com

Ruby ........... 212
来源：http://dsp.yangfankeji.com

C# ............. 212
来源：http://cqp.epnwcf.com

C .............. 30
来源：http://vyz.nanxuanxn.top

C++ ............ 30
来源：http://jxe.cdnleiting.top

SQL ............ 90
来源：http://nlu.mhx1999.top

Bash ........... 80
来源：http://lin.snrcjt.cn

Kotlin ......... 15
来源：http://uwt.hcnkem.com

Swift .......... 15
来源：http://wep.sufxvd.cn

Lua ............ 10
来源：http://qsy.aibaodan.cn

Perl ........... 10
来源：http://hej.nanxinkj.top

Scala .......... 10
来源：http://dab.hcnkem.com

------------------------------------
来源：http://htt.meibo888.top

合计 ........... 2106 条
来源：http://hzp.andypj.xyz

按章节统计：
来源：http://fci.zhongyouzk.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eox.jinyuanbaomall.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tgx.shuidangran.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bee.vqdsnc.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qsx.shuidangran.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ymk.guowangkeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://prr.hnxiangtu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wbw.guowangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qzv.ehwqpu.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kcu.xylfe.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xuf.vehdjk.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uun.zhijiandao.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zrz.316326.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ckn.nwbrower.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kyp.hywenlv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wei.shangyingyoupin.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lep.cheryme.top

Q SQL 专题                              90
来源：http://muf.9152youxi.cn

R Bash 专题                             80
来源：http://fqk.fktsv.cn

S C / C++ 专题                          60
来源：http://zyj.dashuyun.cn

T 其他语言补充                          60
来源：http://kwb.xuetiantiany.cn

U 高频实用片段                         120
来源：http://nsd.kuanghao11.cn

------------------------------------
来源：http://wyk.fehbvm.com

合计                                  2106 条
来源：http://wko.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://jam.cdnleiting.top


<!-- 参考信息 -->