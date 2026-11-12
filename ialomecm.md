代发 wailian999

case class User(name: String, age: Int)
来源：http://gkn.hysaishi.cn

[T57] Scala：模式匹配
来源：http://ppx.sysykeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://tzh.gaohongyu789.top

[T58] Scala：函数定义
来源：http://fje.uphjek.com

def add(a: Int, b: Int): Int = a + b
来源：http://odx.ybcxt.top

[T59] Scala：循环
来源：http://nlp.yangfankeji.com

for (i <- 1 to 10) println(i)
来源：http://wib.yangfankeji.com

[T60] Scala：折叠
来源：http://asw.xuetiantiany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://azc.gaohongyu789.top

================================================================================
来源：http://igq.fanxiaobao.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vjl.vqdsnc.cn

================================================================================
来源：http://uhl.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://zdj.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uhm.jyoumei.cn

[U02] Py：导出 / 安装依赖
来源：http://pzk.yanxiufei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nxs.quarkkingdee.top

[U03] Py：加载 .env 配置
来源：http://huu.pengpengdd.cyou

from dotenv import load_dotenv; load_dotenv()
来源：http://yzv.yuxming.cn

[U04] Py：变量调试打印
来源：http://ukl.tanke756.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pjx.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://coe.yj20258.top

list(dict.fromkeys(arr))
来源：http://jwg.jinyuanbaomall.cn

[U06] Py：合并两个字典
来源：http://rfo.zhoulong.xyz

{**a, **b}
来源：http://cbq.sysykeji.top

[U07] Py：反转字典键值
来源：http://kee.smart0.xyz

{v: k for k, v in d.items()}
来源：http://xlj.gogol.net.cn

[U08] Py：展平二维列表
来源：http://shc.xuanzx.com

[y for x in nested for y in x]
来源：http://jvc.tarul.cn

[U09] Py：字典取最大值的键
来源：http://tqo.fzhhl.top

max(d, key=d.get)
来源：http://ksq.yueranfly.top

[U10] Py：按值排序字典
来源：http://ief.shzxlz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hzy.wangshuangyany.cn

[U11] Py：生成器表达式
来源：http://dze.hysaishi.cn

(x * 2 for x in arr)
来源：http://ogy.tanke756.top

[U12] Py：取出现最多的 3 个元素
来源：http://gdr.zhengqikj.top

Counter(arr).most_common(3)
来源：http://nhx.fehbvm.com

[U13] Py：固定长度队列
来源：http://ljn.hammf.cn

deque(maxlen=10)
来源：http://fgs.uphjek.com

[U14] Py：分组收集到列表
来源：http://eho.c1oappe.top

defaultdict(list)
来源：http://cbm.jlsjyb.cn

[U15] Py：高精度计时
来源：http://nnu.yangfankeji.com

t = time.perf_counter()
来源：http://xnl.hesvh.cn

[U16] Py：命令行参数解析
来源：http://cku.ydzc1.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ulx.xylfe.cn

[U17] Py：初始化日志
来源：http://mbk.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://etd.redwolf501.top

[U18] Py：预编译正则
来源：http://kyh.xylfe.cn

pat = re.compile(r"\d+")
来源：http://bjs.vqdsnc.cn

[U19] Py：正则替换带回调
来源：http://gue.tarul.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nng.havefunace.top

[U20] Py：缓存函数结果
来源：http://yaj.daria6918.cn

@functools.lru_cache(maxsize=None)
来源：http://hgm.zhaomingkeji.xyz

[U21] Py：自定义上下文管理器
来源：http://ojp.sufxvd.cn

@contextlib.contextmanager
来源：http://ajz.tanke756.top

[U22] Py：矩阵转置
来源：http://hxz.jyoumei.cn

list(zip(*m))
来源：http://aog.chenzaomai.com

[U23] Py：分块读取大文件
来源：http://hgz.svipenyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vpt.pycfn.com

[U24] Py：路径操作
来源：http://zjn.tian-w.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://edq.yfazqb.com

[U25] Py：CSV 按字典读
来源：http://bpk.daria6918.cn

csv.DictReader(f)
来源：http://feq.yuanzhike.top

[U26] Py：并发下载
来源：http://sjb.0kj1m.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xpc.cdnleiting.top

[U27] Py：异步 HTTP
来源：http://wly.uphjek.com

aiohttp.ClientSession() 配合 async with
来源：http://hlv.daxiang520.top

[U28] Py：类型别名
来源：http://lsv.andypj.xyz

UserId = int
来源：http://ilu.pycfn.com

[U29] Py：属性校验
来源：http://wfz.birdmap.top

@property 与 @x.setter 配合
来源：http://elp.iojbl.cn

[U30] Py：数据类
来源：http://yeh.kuanghao11.cn

@dataclass(slots=True)
来源：http://slm.xziqi.cn

[U31] Py：单测
来源：http://pds.hesvh.cn

python -m pytest -q
来源：http://wdw.redwolf501.top

[U32] Py：代码格式化
来源：http://nom.guannengcc.top

ruff format . && ruff check --fix .
来源：http://das.aizwys.cn

[U33] Py：打包发布
来源：http://sbj.hesvh.cn

python -m build  （依赖 pyproject.toml）
来源：http://dds.zhoulong.xyz

[U34] Py：判断编码
来源：http://nmc.zdqjudy.top

chardet.detect(raw)
来源：http://ros.cheryme.top

[U35] Py：发送邮件
来源：http://max.aizwys.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lat.mhx1999.top

[U36] Py：定时任务
来源：http://wzg.zycfv.cn

schedule.every(10).minutes.do(job)
来源：http://zag.gogol.net.cn

[U37] Py：读写 Excel
来源：http://inn.gogol.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qrk.yj20258888.top

[U38] Py：获取脚本所在目录
来源：http://mcz.gaohongyu789.top

Path(__file__).resolve().parent
来源：http://fxb.daria6918.cn

[U39] Py：判断是否在交互环境
来源：http://lfv.zhoulong.xyz

sys.stdout.isatty()
来源：http://fig.svipenyu.cn

[U40] Py：打印到标准错误
来源：http://mhj.yuanzhike.top

print("err", file=sys.stderr)
来源：http://wjz.zhaomingkeji.xyz

[U41] PHP：初始化 Composer 项目
来源：http://qzb.snrcjt.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mfh.hysaishi.cn

[U42] PHP：PSR-4 自动加载
来源：http://cdy.cucudq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pkb.kuanghao11.cn

[U43] PHP：声明命名空间
来源：http://ulh.snrcjt.cn

namespace App\Http;
来源：http://kho.guowangkeji.top

[U44] PHP：开启严格类型
来源：http://ttm.sufxvd.cn

declare(strict_types=1);
来源：http://nkj.pengpengdd.cyou

[U45] PHP：类型声明与返回类型
来源：http://bny.nanxinkj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jqd.zhengqikj.top

[U46] PHP：可空类型
来源：http://fxm.gogol.net.cn

?string $name = null
来源：http://xux.birdmap.top

[U47] PHP：联合类型
来源：http://vnn.bjfxy.top

int|string $id
来源：http://jis.cheryme.top

[U48] PHP：纯枚举
来源：http://fbe.guowangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nsm.cqqwz.cn

[U49] PHP：只读属性
来源：http://rvt.nwbrower.top

public readonly string $name
来源：http://tsp.yuanzhike.top

[U50] PHP：构造器属性提升
来源：http://bje.zdbjq.cn

public function __construct(private int $id) {}
来源：http://bzw.52xcode.cn

[U51] PHP：数组解构
来源：http://eru.zdqjudy.top

[$a, $b] = $arr;
来源：http://ket.zdqjudy.top

[U52] PHP：箭头函数
来源：http://czy.dianchejie.cn

$double = fn($x) => $x * 2;
来源：http://vom.yuxming.cn

[U53] PHP：空合并运算符
来源：http://prd.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://fed.snrcjt.cn

[U54] PHP：空安全调用
来源：http://qit.bbcook.cn

$obj?->method()
来源：http://nak.andypj.xyz

[U55] PHP：match 表达式
来源：http://aed.zhixingplan.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tss.c1oappe.top

[U56] PHP：命名参数
来源：http://hlg.zdbjq.cn

f(a: 1, b: 2)
来源：http://gkw.hnqzz.top

[U57] PHP：字符串插值
来源：http://ozi.meibo888.top

"值: {$a}"
来源：http://umf.sysykeji.top

[U58] PHP：数组三件套
来源：http://hmr.nwbrower.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zzc.guowangkeji.top

[U59] PHP：自定义排序
来源：http://ace.xuetiantiany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pox.zhiwuduotai.top

[U60] PHP：JSON 编解码
来源：http://vlm.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gbe.jinyuanbaomall.cn

[U61] PHP：正则
来源：http://yba.wangdashe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lnb.pycfn.com

[U62] PHP：日期对象
来源：http://wqm.hongshengwenyu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fca.aibaodan.cn

[U63] PHP：文件读写
来源：http://jha.fanxiaobao.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pgv.yuanzhike.top

[U64] PHP：目录遍历
来源：http://ilv.ydzc1.top

glob("dir/*.php");  scandir("dir");
来源：http://xcp.yuanzhike.top

[U65] PHP：会话
来源：http://yqd.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ctc.gogol.net.cn

[U66] PHP：设置 Cookie
来源：http://mtm.52xcode.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ahm.pycfn.com

[U67] PHP：处理文件上传
来源：http://vqo.xuetiantiany.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bmj.svipenyu.cn

[U68] PHP：PDO 连接
来源：http://uwh.fktsv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fqs.yangfankeji.com

[U69] PHP：PDO 预处理
来源：http://cgo.zycfv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qvx.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://kpd.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dgx.zdbjq.cn

[U71] PHP：抛出异常
来源：http://gao.vehdjk.com

throw new RuntimeException("失败", 500);
来源：http://szs.zhengqikj.top

[U72] PHP：写错误日志
来源：http://rbp.gzhubu.top

error_log("失败: " . $e->getMessage());
来源：http://aes.fktsv.cn

[U73] PHP：读取 ini 配置
来源：http://zyz.yanxiufei.cn

parse_ini_file("config.ini", true)
来源：http://ooy.gaohongyu789.top

[U74] PHP：读取环境变量
来源：http://xyo.jinyuanbaomall.cn

getenv("APP_ENV") ?: "production"
来源：http://fau.quarkkingdee.top

[U75] PHP：依赖注入
来源：http://yzk.mhx1999.top

composer require psr/container
来源：http://npc.tanke756.top

[U76] PHP：简单路由
来源：http://qck.fzhhl.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://upk.fengsongda.top

[U77] PHP：模板渲染
来源：http://qyj.sjlbkw.cn

composer require twig/twig
来源：http://kjt.nanxinkj.top

[U78] PHP：单元测试
来源：http://kej.yj20258888.top

composer require --dev phpunit/phpunit
来源：http://qjx.fanxiaobao.xyz

[U79] PHP：静态分析
来源：http://dpn.wangdashe.top

composer require --dev phpstan/phpstan
来源：http://nxf.zhixingplan.top

[U80] PHP：代码规范修复
来源：http://yzk.quarkkingdee.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://fnd.zdqjudy.top

[U81] JS：初始化项目
来源：http://inu.jlsjyb.cn

npm init -y;  npm i express
来源：http://fyv.pengpengdd.cyou

[U82] JS：package.json 脚本
来源：http://zet.chenzaomai.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jbl.zhixingplan.top

[U83] JS：ES Module 导入导出
来源：http://nlr.hongshengwenyu.top

export const a = 1;  import { a } from "./m.js";
来源：http://ymd.zhaomingkeji.xyz

[U84] JS：CommonJS 写法
来源：http://kdo.ctjpmb.com

module.exports = { a };  const { a } = require("./m");
来源：http://ogn.hnqzz.top

[U85] JS：可选链
来源：http://izs.redwolf501.top

a?.b?.c
来源：http://fpg.meibo888.top

[U86] JS：空值合并
来源：http://naf.feifeiyinyue.top

a ?? b
来源：http://fqb.zhengqikj.top

[U87] JS：解构默认值
来源：http://lzr.ivvv.top

const { a = 1, b = 2 } = obj;
来源：http://tdw.9152youxi.cn

[U88] JS：对象展开合并
来源：http://vyg.aibaodan.cn

{ ...a, ...b }
来源：http://ghc.yj20258888.top

[U89] JS：数组去重
来源：http://iku.bbcook.cn

[...new Set(arr)]
来源：http://mdm.yangfankeji.com

[U90] JS：数字数组排序
来源：http://ndp.hfpthk.cn

[...arr].sort((a, b) => a - b)
来源：http://epw.zdqjudy.top

[U91] JS：对象键值遍历
来源：http://oeu.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jcc.cucudq.cn

[U92] JS：深拷贝
来源：http://dmi.hnqzz.top

structuredClone(obj)
来源：http://rmh.ydjk.org.cn

[U93] JS：模板字符串
来源：http://kfz.ydzc1.top

`共 ${n} 条`
来源：http://tnw.zhiwuduotai.top

[U94] JS：箭头函数
来源：http://lqg.xylfe.cn

const double = x => x * 2;
来源：http://cvv.wangshuangyany.cn

[U95] JS：Promise 包装
来源：http://osl.cashguo.top

new Promise((resolve, reject) => {})
来源：http://rqr.yj20258.top

[U96] JS：async/await 与异常
来源：http://ijx.cheryme.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kfj.fktsv.cn

[U97] JS：并发请求
来源：http://wtk.fehbvm.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://jqn.xuanzx.com

[U98] JS：fetch 带 JSON
来源：http://bxs.tarul.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uqo.haohaochexian.top

[U99] JS：事件监听
来源：http://zem.pengpengdd.cyou

el.addEventListener("click", e => {})
来源：http://fzz.yj20258.top

[U100] JS：DOM 查询
来源：http://djp.yj202588.top

document.querySelector(".item")
来源：http://kbv.yj202588.top

[U101] JS：classList 操作
来源：http://uij.yangfankeji.com

el.classList.toggle("active")
来源：http://txs.yj20258.top

[U102] JS：本地存储
来源：http://qcs.zhongyouzk.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hhd.epnwcf.com

[U103] JS：定时器
来源：http://pvg.jianghu66.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mlr.nanxuanxn.top

[U104] JS：防抖
来源：http://ubv.zhixingplan.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qkw.guowangkeji.top

[U105] JS：节流
来源：http://aft.c1oappe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kkw.ivvv.top

[U106] JS：日期格式化
来源：http://puw.havefunace.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kne.xylfe.cn

[U107] JS：数字千分位
来源：http://znj.uphjek.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sro.redwolf501.top

[U108] JS：随机整数
来源：http://jrb.dianchejie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jhu.jianghu66.top

[U109] JS：数组分组
来源：http://gzx.yonumen.top

Object.groupBy(arr, x => x.type)
来源：http://fxg.jinyuanbaomall.cn

[U110] JS：数组分块
来源：http://lqm.yueranfly.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hpp.chenlongwang.top

[U111] JS：对象转 Map
来源：http://bxs.fzhhl.top

new Map(Object.entries(obj))
来源：http://ker.hnxiangtu.top

[U112] JS：字符串补位
来源：http://cou.jiagoushi.top

"7".padStart(3, "0")
来源：http://avm.jqgfzy.top

[U113] JS：正则替换全部
来源：http://mwq.jinqigufen.top

s.replaceAll("a", "b")
来源：http://ava.yanxiufei.cn

[U114] JS：JSON 深比较
来源：http://lne.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nsx.jinyuanbaomall.cn

[U115] JS：生成 UUID
来源：http://ckj.shanyushiyangkeji.top

crypto.randomUUID()
来源：http://sex.fehbvm.com

[U116] JS：类型检查（JSDoc）
来源：http://wdj.guowangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://chw.c1oappe.top

[U117] JS：单元测试
来源：http://lan.hywenlv.cn

npm i -D vitest;  npx vitest
来源：http://znp.vqdsnc.cn

[U118] JS：开发服务器
来源：http://ouy.meibo888.top

npm i -D vite;  npx vite
来源：http://xbr.nwbrower.top

[U119] JS：生产构建
来源：http://pqx.jqgfzy.top

npx vite build
来源：http://kdi.xylfe.cn

[U120] JS：读取环境变量（Vite）
来源：http://ecy.cqqwz.cn

import.meta.env.VITE_API_URL
来源：http://zxl.gogol.net.cn

================================================================================
来源：http://axw.xuetiantiany.cn

统计汇总
来源：http://gxl.xuanzx.com

================================================================================
来源：http://cnq.havefunace.top

按语言统计（条）：
来源：http://ebp.52xcode.cn

Python ......... 252
来源：http://dhi.iojbl.cn

PHP ............ 252
来源：http://kqe.cashguo.top

JavaScript ..... 252
来源：http://hof.jqgfzy.top

TypeScript ..... 212
来源：http://cqv.haohaochexian.top

Java ........... 212
来源：http://vvx.cheryme.top

Go ............. 212
来源：http://ddd.yongpay.top

Ruby ........... 212
来源：http://fgf.guannengcc.top

C# ............. 212
来源：http://jqt.ivvv.top

C .............. 30
来源：http://nuc.gzhubu.top

C++ ............ 30
来源：http://mum.9152youxi.cn

SQL ............ 90
来源：http://zmk.quarkkingdee.top

Bash ........... 80
来源：http://jfp.jinqigufen.top

Kotlin ......... 15
来源：http://qel.sysykeji.top

Swift .......... 15
来源：http://osw.jianghu66.top

Lua ............ 10
来源：http://yzp.yuanzhike.top

Perl ........... 10
来源：http://iks.pengpengdd.cyou

Scala .......... 10
来源：http://lmn.vehdjk.com

------------------------------------
来源：http://lrr.hcnkem.com

合计 ........... 2106 条
来源：http://fzu.hcnkem.com

按章节统计：
来源：http://tew.daxiang520.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kcp.andypj.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vwy.yvedp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jle.epnwcf.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dwz.jinyuanbaomall.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vqu.ybcxt.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jyd.ydjk.org.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ayj.hcnkem.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gnk.zycfv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jmk.ehwqpu.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pge.epnwcf.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://syj.daria6918.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mcr.ctjpmb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hle.hammf.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vhh.tianlin.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vic.bjfxy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mny.cdnleiting.top

Q SQL 专题                              90
来源：http://glc.epnwcf.com

R Bash 专题                             80
来源：http://srk.nwbrower.top

S C / C++ 专题                          60
来源：http://rcu.guowangkeji.top

T 其他语言补充                          60
来源：http://ngs.snrcjt.cn

U 高频实用片段                         120
来源：http://hkx.feifeiyinyue.top

------------------------------------
来源：http://tan.sxryk.cn

合计                                  2106 条
来源：http://tps.yongpay.top

--------------------------------------------------------------------------------
来源：http://vzl.pycfn.com


<!-- 参考信息 -->