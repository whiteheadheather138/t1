代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://tpv.havefunace.top

[T59] Scala：循环
来源：http://fql.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://fpq.ydzc1.top

[T60] Scala：折叠
来源：http://wpm.fengsongda.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zxv.hesvh.cn

================================================================================
来源：http://suk.sxryk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rbh.fehbvm.com

================================================================================
来源：http://ncb.yuxming.cn

[U01] Py：创建虚拟环境
来源：http://vdb.nanxuanxn.top

python -m venv .venv && source .venv/bin/activate
来源：http://mxm.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://pij.shanyushiyangtech.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nbu.zdqjudy.top

[U03] Py：加载 .env 配置
来源：http://pnh.pycfn.com

from dotenv import load_dotenv; load_dotenv()
来源：http://wmp.jianghu66.top

[U04] Py：变量调试打印
来源：http://uhi.jiagoushi.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wmf.gzhubu.top

[U05] Py：列表去重且保序
来源：http://lxr.jinghuilouyu.cn

list(dict.fromkeys(arr))
来源：http://yzi.sweek.top

[U06] Py：合并两个字典
来源：http://ypk.zhengqikj.top

{**a, **b}
来源：http://lxf.hesvh.cn

[U07] Py：反转字典键值
来源：http://oun.guowangkeji.top

{v: k for k, v in d.items()}
来源：http://dge.andypj.xyz

[U08] Py：展平二维列表
来源：http://npu.9152youxi.cn

[y for x in nested for y in x]
来源：http://mdc.dashuyun.cn

[U09] Py：字典取最大值的键
来源：http://isq.hysaishi.cn

max(d, key=d.get)
来源：http://wst.fktsv.cn

[U10] Py：按值排序字典
来源：http://fls.tanke756.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ifd.jinghuilouyu.cn

[U11] Py：生成器表达式
来源：http://wfp.aibaodan.cn

(x * 2 for x in arr)
来源：http://vxl.c1oappe.top

[U12] Py：取出现最多的 3 个元素
来源：http://ozb.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://iqb.zhoulong.xyz

[U13] Py：固定长度队列
来源：http://mwt.mhx1999.top

deque(maxlen=10)
来源：http://ooh.gotoacloud.top

[U14] Py：分组收集到列表
来源：http://okr.yonumen.top

defaultdict(list)
来源：http://cxu.9152youxi.cn

[U15] Py：高精度计时
来源：http://imy.vqdsnc.cn

t = time.perf_counter()
来源：http://ypo.yangfankeji.com

[U16] Py：命令行参数解析
来源：http://imi.cdnleiting.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pad.yongpay.top

[U17] Py：初始化日志
来源：http://aeg.jinyuanbaomall.cn

logging.basicConfig(level=logging.INFO)
来源：http://wkh.jinqigfzy.top

[U18] Py：预编译正则
来源：http://cub.jinqigfzy.top

pat = re.compile(r"\d+")
来源：http://lzs.havefunace.top

[U19] Py：正则替换带回调
来源：http://wpq.fanxiaobao.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ers.hnqzz.top

[U20] Py：缓存函数结果
来源：http://ecc.ydjk.org.cn

@functools.lru_cache(maxsize=None)
来源：http://mmj.xylfe.cn

[U21] Py：自定义上下文管理器
来源：http://nhs.iojbl.cn

@contextlib.contextmanager
来源：http://iml.dianchejie.cn

[U22] Py：矩阵转置
来源：http://mef.hnxiangtu.top

list(zip(*m))
来源：http://czx.zhijiandao.cn

[U23] Py：分块读取大文件
来源：http://get.zdbjq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wow.xziqi.cn

[U24] Py：路径操作
来源：http://pob.xinyue.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wxy.chenjidiqi.icu

[U25] Py：CSV 按字典读
来源：http://frq.hammf.cn

csv.DictReader(f)
来源：http://doy.pengpengdd.cyou

[U26] Py：并发下载
来源：http://yko.jinghuilouyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bcz.zhengqikj.top

[U27] Py：异步 HTTP
来源：http://tpp.redwolf501.top

aiohttp.ClientSession() 配合 async with
来源：http://toj.jianghu66.top

[U28] Py：类型别名
来源：http://fvc.52xcode.cn

UserId = int
来源：http://khb.sweek.top

[U29] Py：属性校验
来源：http://pqt.guannengcc.top

@property 与 @x.setter 配合
来源：http://nbb.iojbl.cn

[U30] Py：数据类
来源：http://frr.jlsjyb.cn

@dataclass(slots=True)
来源：http://qzi.zhengqikj.top

[U31] Py：单测
来源：http://nkg.tanke756.top

python -m pytest -q
来源：http://azl.cdnleiting.top

[U32] Py：代码格式化
来源：http://mmo.cashguo.top

ruff format . && ruff check --fix .
来源：http://gxq.hysaishi.cn

[U33] Py：打包发布
来源：http://kue.xuanzx.com

python -m build  （依赖 pyproject.toml）
来源：http://ztl.uphjek.com

[U34] Py：判断编码
来源：http://dmw.fzhhl.top

chardet.detect(raw)
来源：http://izq.feifeiyinyue.top

[U35] Py：发送邮件
来源：http://qhh.yvedp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://joq.hammf.cn

[U36] Py：定时任务
来源：http://cvc.hywenlv.cn

schedule.every(10).minutes.do(job)
来源：http://lzs.vehdjk.com

[U37] Py：读写 Excel
来源：http://uhm.snrcjt.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eql.zhaomingkeji.xyz

[U38] Py：获取脚本所在目录
来源：http://cid.9152youxi.cn

Path(__file__).resolve().parent
来源：http://rfk.yj20258888.top

[U39] Py：判断是否在交互环境
来源：http://jkn.feifeiyinyue.top

sys.stdout.isatty()
来源：http://mrd.nanxinkj.top

[U40] Py：打印到标准错误
来源：http://tsm.zdbjq.cn

print("err", file=sys.stderr)
来源：http://umk.hnxiangtu.top

[U41] PHP：初始化 Composer 项目
来源：http://ndz.fzhhl.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jlc.yj20258.top

[U42] PHP：PSR-4 自动加载
来源：http://bbg.cashguo.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dak.iojbl.cn

[U43] PHP：声明命名空间
来源：http://rqj.chenjidiqi.icu

namespace App\Http;
来源：http://vtt.bbcook.cn

[U44] PHP：开启严格类型
来源：http://ewj.sweek.top

declare(strict_types=1);
来源：http://bzf.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://osb.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jls.aibaodan.cn

[U46] PHP：可空类型
来源：http://nsv.0kj1m.cn

?string $name = null
来源：http://peo.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://jyx.feifeiyinyue.top

int|string $id
来源：http://bcf.ybcxt.top

[U48] PHP：纯枚举
来源：http://sgq.yuanzhike.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nzs.yangfankeji.com

[U49] PHP：只读属性
来源：http://voy.xinyue.icu

public readonly string $name
来源：http://xjd.zhijiandao.cn

[U50] PHP：构造器属性提升
来源：http://lak.yj202588.top

public function __construct(private int $id) {}
来源：http://jet.tanke756.top

[U51] PHP：数组解构
来源：http://yic.fehbvm.com

[$a, $b] = $arr;
来源：http://xkn.yj202588.top

[U52] PHP：箭头函数
来源：http://qow.sufxvd.cn

$double = fn($x) => $x * 2;
来源：http://zrz.cdnleiting.top

[U53] PHP：空合并运算符
来源：http://hdw.jqgufenzy.top

$v = $a ?? $b ?? "default";
来源：http://kne.316326.xyz

[U54] PHP：空安全调用
来源：http://qib.meibo888.top

$obj?->method()
来源：http://mjh.hcnkem.com

[U55] PHP：match 表达式
来源：http://wqm.nanxinkj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ezt.tian-w.cn

[U56] PHP：命名参数
来源：http://eep.tarul.cn

f(a: 1, b: 2)
来源：http://lik.shzxlz.cn

[U57] PHP：字符串插值
来源：http://meg.zycfv.cn

"值: {$a}"
来源：http://jea.yongpay.top

[U58] PHP：数组三件套
来源：http://qbz.shanyushiyangtech.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hng.yuxming.cn

[U59] PHP：自定义排序
来源：http://pom.yueranfly.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oyn.xingfuxueyuan.xyz

[U60] PHP：JSON 编解码
来源：http://iov.hnxiangtu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sop.chenjidiqi.icu

[U61] PHP：正则
来源：http://fwn.sxryk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qvs.zhixingplan.top

[U62] PHP：日期对象
来源：http://czm.zdqjudy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ynk.jiagoushi.top

[U63] PHP：文件读写
来源：http://cbg.yanxiufei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://woc.iojbl.cn

[U64] PHP：目录遍历
来源：http://eil.yvedp.cn

glob("dir/*.php");  scandir("dir");
来源：http://fvl.shzxlz.cn

[U65] PHP：会话
来源：http://tlk.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dty.yanxiufei.cn

[U66] PHP：设置 Cookie
来源：http://fcj.zdqjudy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sle.fengsongda.top

[U67] PHP：处理文件上传
来源：http://dak.hywenlv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ftv.ppjwa.cn

[U68] PHP：PDO 连接
来源：http://ivf.tarul.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jav.jinqigufen.top

[U69] PHP：PDO 预处理
来源：http://qhp.ivvv.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tul.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://eqc.hfpthk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hjl.316326.xyz

[U71] PHP：抛出异常
来源：http://onb.jinyuanbaomall.cn

throw new RuntimeException("失败", 500);
来源：http://lhk.xuanzx.com

[U72] PHP：写错误日志
来源：http://fjs.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://flg.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://bjg.zycfv.cn

parse_ini_file("config.ini", true)
来源：http://fch.ivvv.top

[U74] PHP：读取环境变量
来源：http://kmr.ydjk.org.cn

getenv("APP_ENV") ?: "production"
来源：http://ktw.hcnkem.com

[U75] PHP：依赖注入
来源：http://jef.chenzaomai.com

composer require psr/container
来源：http://lyl.kuanghao11.cn

[U76] PHP：简单路由
来源：http://sbn.birdmap.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tln.hongshengwenyu.top

[U77] PHP：模板渲染
来源：http://rue.kuanghao11.cn

composer require twig/twig
来源：http://nze.tian-w.cn

[U78] PHP：单元测试
来源：http://wyq.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://xcd.cdnleiting.top

[U79] PHP：静态分析
来源：http://lrq.ivvv.top

composer require --dev phpstan/phpstan
来源：http://gsx.dashuyun.cn

[U80] PHP：代码规范修复
来源：http://crx.daria6918.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://iem.zhixingplan.top

[U81] JS：初始化项目
来源：http://quk.wangdashe.top

npm init -y;  npm i express
来源：http://esw.snrcjt.cn

[U82] JS：package.json 脚本
来源：http://whn.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dlz.jqgufenzy.top

[U83] JS：ES Module 导入导出
来源：http://klz.hesvh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jsn.birdmap.top

[U84] JS：CommonJS 写法
来源：http://lgq.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vqj.aizwys.cn

[U85] JS：可选链
来源：http://thx.sufxvd.cn

a?.b?.c
来源：http://lta.yfazqb.com

[U86] JS：空值合并
来源：http://dzb.meibo888.top

a ?? b
来源：http://ezz.cucudq.cn

[U87] JS：解构默认值
来源：http://qjc.yuxming.cn

const { a = 1, b = 2 } = obj;
来源：http://xik.feifeiyinyue.top

[U88] JS：对象展开合并
来源：http://hug.svipenyu.cn

{ ...a, ...b }
来源：http://dei.bjfxy.top

[U89] JS：数组去重
来源：http://zrb.52xcode.cn

[...new Set(arr)]
来源：http://nrp.xylfe.cn

[U90] JS：数字数组排序
来源：http://ady.ywan-chungtsiang.top

[...arr].sort((a, b) => a - b)
来源：http://lyi.jinyuanbaomall.cn

[U91] JS：对象键值遍历
来源：http://iam.cucudq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tak.zdbjq.cn

[U92] JS：深拷贝
来源：http://hie.zhaomingkeji.xyz

structuredClone(obj)
来源：http://sni.haohaochexian.top

[U93] JS：模板字符串
来源：http://are.shuidangran.top

`共 ${n} 条`
来源：http://tgy.zhaomingkeji.xyz

[U94] JS：箭头函数
来源：http://lig.cashguo.top

const double = x => x * 2;
来源：http://sij.smart0.xyz

[U95] JS：Promise 包装
来源：http://wmz.daria6918.cn

new Promise((resolve, reject) => {})
来源：http://ilc.hammf.cn

[U96] JS：async/await 与异常
来源：http://pte.hcnkem.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fbx.yj20258.top

[U97] JS：并发请求
来源：http://poh.ywan-chungtsiang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://fdi.tarul.cn

[U98] JS：fetch 带 JSON
来源：http://snz.nwbrower.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zax.yongpay.top

[U99] JS：事件监听
来源：http://mvi.epnwcf.com

el.addEventListener("click", e => {})
来源：http://hdg.hysaishi.cn

[U100] JS：DOM 查询
来源：http://jmr.yj20258.top

document.querySelector(".item")
来源：http://qsa.0kj1m.cn

[U101] JS：classList 操作
来源：http://sof.redwolf501.top

el.classList.toggle("active")
来源：http://xgi.tian-w.cn

[U102] JS：本地存储
来源：http://txw.andypj.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://ifu.hfpthk.cn

[U103] JS：定时器
来源：http://frb.zdbjq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ofq.zhijiandao.cn

[U104] JS：防抖
来源：http://qpf.sweek.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qfy.daxiang520.top

[U105] JS：节流
来源：http://xbt.52xcode.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cao.dashuyun.cn

[U106] JS：日期格式化
来源：http://xoc.jianghu66.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bpu.meibo888.top

[U107] JS：数字千分位
来源：http://gym.haohaochexian.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ayc.uphjek.com

[U108] JS：随机整数
来源：http://sqw.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rix.xingfuxueyuan.xyz

[U109] JS：数组分组
来源：http://wsh.pengpengdd.cyou

Object.groupBy(arr, x => x.type)
来源：http://xcr.0kj1m.cn

[U110] JS：数组分块
来源：http://zyp.zhongyouzk.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dru.jyoumei.cn

[U111] JS：对象转 Map
来源：http://zmd.chenjidiqi.icu

new Map(Object.entries(obj))
来源：http://jfe.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://boa.pengpengdd.cyou

"7".padStart(3, "0")
来源：http://yih.ydzc1.top

[U113] JS：正则替换全部
来源：http://yca.zhixingplan.top

s.replaceAll("a", "b")
来源：http://soq.shanyushiyangkeji.top

[U114] JS：JSON 深比较
来源：http://nod.tanke756.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lzw.yj20258.top

[U115] JS：生成 UUID
来源：http://zcz.zhixingplan.top

crypto.randomUUID()
来源：http://der.yangfankeji.com

[U116] JS：类型检查（JSDoc）
来源：http://qtb.gzhubu.top

/** @param {string} name */ function f(name) {}
来源：http://pew.pengpengdd.cyou

[U117] JS：单元测试
来源：http://xtb.cheryme.top

npm i -D vitest;  npx vitest
来源：http://jsr.guannengcc.top

[U118] JS：开发服务器
来源：http://ble.fehbvm.com

npm i -D vite;  npx vite
来源：http://npt.zhijiandao.cn

[U119] JS：生产构建
来源：http://hkb.jqgufenzy.top

npx vite build
来源：http://gvn.fanxiaobao.xyz

[U120] JS：读取环境变量（Vite）
来源：http://hcl.yongpay.top

import.meta.env.VITE_API_URL
来源：http://byi.hysaishi.cn

================================================================================
来源：http://efb.ivvv.top

统计汇总
来源：http://wsj.mhx1999.top

================================================================================
来源：http://ixp.gogol.net.cn

按语言统计（条）：
来源：http://pvo.havefunace.top

Python ......... 252
来源：http://lzr.yueranfly.top

PHP ............ 252
来源：http://oqo.yj20258888.top

JavaScript ..... 252
来源：http://mmj.zycfv.cn

TypeScript ..... 212
来源：http://efx.zdbjq.cn

Java ........... 212
来源：http://bmy.daria6918.cn

Go ............. 212
来源：http://pxg.epnwcf.com

Ruby ........... 212
来源：http://lee.snrcjt.cn

C# ............. 212
来源：http://kde.ctjpmb.com

C .............. 30
来源：http://zni.tian-w.cn

C++ ............ 30
来源：http://rkl.guowangkeji.top

SQL ............ 90
来源：http://dgf.hongshengwenyu.top

Bash ........... 80
来源：http://qkc.zdbjq.cn

Kotlin ......... 15
来源：http://lvy.tian-w.cn

Swift .......... 15
来源：http://zme.shanyushiyangtech.top

Lua ............ 10
来源：http://wls.haohaochexian.top

Perl ........... 10
来源：http://rim.xuanzx.com

Scala .......... 10
来源：http://yzh.jlsjyb.cn

------------------------------------
来源：http://imj.shuidangran.top

合计 ........... 2106 条
来源：http://wvi.0kj1m.cn

按章节统计：
来源：http://ios.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sua.fanxiaobao.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ymx.sxryk.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dlc.ehwqpu.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iju.sjlbkw.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oqr.jinghuilouyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zbx.yanxiufei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uew.kuanghao11.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nox.zhengqikj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ikt.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://thq.316326.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hcj.yj202588.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mzd.hfpthk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sow.cheryme.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dtd.jiagoushi.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hzn.dashuyun.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dga.andypj.xyz

Q SQL 专题                              90
来源：http://ikx.gotoacloud.top

R Bash 专题                             80
来源：http://sga.dianchejie.cn

S C / C++ 专题                          60
来源：http://sdv.zhoulong.xyz

T 其他语言补充                          60
来源：http://daa.shzxlz.cn

U 高频实用片段                         120
来源：http://jdg.feifeiyinyue.top

------------------------------------
来源：http://nnz.ctjpmb.com

合计                                  2106 条
来源：http://nnw.yj20258.top

--------------------------------------------------------------------------------
来源：http://wfv.hnqzz.top

使用提醒
来源：http://iys.nwbrower.top

--------------------------------------------------------------------------------
来源：http://aun.jqgfzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sji.yj20258888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rnl.cdnleiting.top


<!-- 参考信息 -->