代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://zly.yvedp.cn

[T55] Scala：集合过滤
来源：http://iot.cqqwz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://iff.gotoacloud.top

[T56] Scala：样例类
来源：http://wvk.jinghuilouyu.cn

case class User(name: String, age: Int)
来源：http://kpt.gzhubu.top

[T57] Scala：模式匹配
来源：http://exm.sysykeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mpj.sxryk.cn

[T58] Scala：函数定义
来源：http://sqe.daria6918.cn

def add(a: Int, b: Int): Int = a + b
来源：http://shv.iojbl.cn

[T59] Scala：循环
来源：http://pmg.316326.xyz

for (i <- 1 to 10) println(i)
来源：http://uwf.hnxiangtu.top

[T60] Scala：折叠
来源：http://kns.vqdsnc.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wlc.svipenyu.cn

================================================================================
来源：http://naa.tanke756.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vnx.snrcjt.cn

================================================================================
来源：http://mse.gotoacloud.top

[U01] Py：创建虚拟环境
来源：http://lcs.zhoulong.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://dvk.kuanghao11.cn

[U02] Py：导出 / 安装依赖
来源：http://auz.wangdashe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ufc.shangyingyoupin.top

[U03] Py：加载 .env 配置
来源：http://bnc.jiagoushi.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qix.chenzaomai.com

[U04] Py：变量调试打印
来源：http://reu.fzhhl.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uya.sjlbkw.cn

[U05] Py：列表去重且保序
来源：http://pbe.jinyuanbaomall.cn

list(dict.fromkeys(arr))
来源：http://fcp.316326.xyz

[U06] Py：合并两个字典
来源：http://qjr.xuanzx.com

{**a, **b}
来源：http://frv.aibaodan.cn

[U07] Py：反转字典键值
来源：http://zzb.nanxuanxn.top

{v: k for k, v in d.items()}
来源：http://lwn.quarkkingdee.top

[U08] Py：展平二维列表
来源：http://jok.wangshuangyany.cn

[y for x in nested for y in x]
来源：http://tdo.zhoulong.xyz

[U09] Py：字典取最大值的键
来源：http://lwo.chenlongwang.top

max(d, key=d.get)
来源：http://psk.316326.xyz

[U10] Py：按值排序字典
来源：http://hzy.jyoumei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pom.shanyushiyangkeji.top

[U11] Py：生成器表达式
来源：http://svm.jinqigufen.top

(x * 2 for x in arr)
来源：http://dov.yangfankeji.com

[U12] Py：取出现最多的 3 个元素
来源：http://fjf.tanke756.top

Counter(arr).most_common(3)
来源：http://jqv.ctjpmb.com

[U13] Py：固定长度队列
来源：http://bux.jqgfzy.top

deque(maxlen=10)
来源：http://vvr.yanxiufei.cn

[U14] Py：分组收集到列表
来源：http://nzb.nwbrower.top

defaultdict(list)
来源：http://bmx.hcnkem.com

[U15] Py：高精度计时
来源：http://slt.jyoumei.cn

t = time.perf_counter()
来源：http://vkv.xingfuxueyuan.xyz

[U16] Py：命令行参数解析
来源：http://xye.zhoulong.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://isp.daxiang520.top

[U17] Py：初始化日志
来源：http://bza.yfazqb.com

logging.basicConfig(level=logging.INFO)
来源：http://bfa.birdmap.top

[U18] Py：预编译正则
来源：http://deu.chenlongwang.top

pat = re.compile(r"\d+")
来源：http://ane.sxryk.cn

[U19] Py：正则替换带回调
来源：http://ecg.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uzz.vehdjk.com

[U20] Py：缓存函数结果
来源：http://tcd.zhengqikj.top

@functools.lru_cache(maxsize=None)
来源：http://rqq.sxryk.cn

[U21] Py：自定义上下文管理器
来源：http://ekl.yvedp.cn

@contextlib.contextmanager
来源：http://ygh.bbcook.cn

[U22] Py：矩阵转置
来源：http://rlf.316326.xyz

list(zip(*m))
来源：http://sbv.sufxvd.cn

[U23] Py：分块读取大文件
来源：http://obj.gogol.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vyh.shzxlz.cn

[U24] Py：路径操作
来源：http://nby.tian-w.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uff.mhx1999.top

[U25] Py：CSV 按字典读
来源：http://knr.jianghu66.top

csv.DictReader(f)
来源：http://nid.sxryk.cn

[U26] Py：并发下载
来源：http://kkk.xziqi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ktd.9152youxi.cn

[U27] Py：异步 HTTP
来源：http://khe.fzhhl.top

aiohttp.ClientSession() 配合 async with
来源：http://pdm.ivvv.top

[U28] Py：类型别名
来源：http://gov.zycfv.cn

UserId = int
来源：http://azn.aibaodan.cn

[U29] Py：属性校验
来源：http://gky.jqgufenzy.top

@property 与 @x.setter 配合
来源：http://fqd.chenjidiqi.icu

[U30] Py：数据类
来源：http://ztl.xziqi.cn

@dataclass(slots=True)
来源：http://znc.bbcook.cn

[U31] Py：单测
来源：http://jda.mhx1999.top

python -m pytest -q
来源：http://ybx.yj202588.top

[U32] Py：代码格式化
来源：http://fpf.ywan-chungtsiang.top

ruff format . && ruff check --fix .
来源：http://rxx.zdbjq.cn

[U33] Py：打包发布
来源：http://haf.ivvv.top

python -m build  （依赖 pyproject.toml）
来源：http://bzp.zhijiandao.cn

[U34] Py：判断编码
来源：http://iam.ydzc1.top

chardet.detect(raw)
来源：http://dvp.uphjek.com

[U35] Py：发送邮件
来源：http://ucb.wangshuangyany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jub.smart0.xyz

[U36] Py：定时任务
来源：http://xba.nwbrower.top

schedule.every(10).minutes.do(job)
来源：http://jgr.tanke756.top

[U37] Py：读写 Excel
来源：http://ewm.uphjek.com

pandas.read_excel / DataFrame.to_excel
来源：http://qzb.gaohongyu789.top

[U38] Py：获取脚本所在目录
来源：http://sna.ydzc1.top

Path(__file__).resolve().parent
来源：http://hfn.ywan-chungtsiang.top

[U39] Py：判断是否在交互环境
来源：http://win.jinyuanbaomall.cn

sys.stdout.isatty()
来源：http://xnh.aibaodan.cn

[U40] Py：打印到标准错误
来源：http://qbo.yueranfly.top

print("err", file=sys.stderr)
来源：http://eoq.shuidangran.top

[U41] PHP：初始化 Composer 项目
来源：http://edi.zhengqikj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lzg.hesvh.cn

[U42] PHP：PSR-4 自动加载
来源：http://bzq.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zmp.aibaodan.cn

[U43] PHP：声明命名空间
来源：http://xtz.shangyingyoupin.top

namespace App\Http;
来源：http://hwv.guowangkeji.top

[U44] PHP：开启严格类型
来源：http://vfz.nanxinkj.top

declare(strict_types=1);
来源：http://kmi.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://rqc.xylfe.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pcv.cucudq.cn

[U46] PHP：可空类型
来源：http://owl.aizwys.cn

?string $name = null
来源：http://qim.smart0.xyz

[U47] PHP：联合类型
来源：http://dmf.zycfv.cn

int|string $id
来源：http://xbj.zdqjudy.top

[U48] PHP：纯枚举
来源：http://jrp.ybcxt.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pwo.zhijiandao.cn

[U49] PHP：只读属性
来源：http://ddy.jinqigufen.top

public readonly string $name
来源：http://tju.yonumen.top

[U50] PHP：构造器属性提升
来源：http://ixr.sxryk.cn

public function __construct(private int $id) {}
来源：http://tgx.shuidangran.top

[U51] PHP：数组解构
来源：http://nnc.yvedp.cn

[$a, $b] = $arr;
来源：http://ihm.sweek.top

[U52] PHP：箭头函数
来源：http://xqr.quarkkingdee.top

$double = fn($x) => $x * 2;
来源：http://zgb.hesvh.cn

[U53] PHP：空合并运算符
来源：http://peu.hnqzz.top

$v = $a ?? $b ?? "default";
来源：http://iyy.meibo888.top

[U54] PHP：空安全调用
来源：http://acu.yonumen.top

$obj?->method()
来源：http://kiy.jqgufenzy.top

[U55] PHP：match 表达式
来源：http://brc.gotoacloud.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pfx.pycfn.com

[U56] PHP：命名参数
来源：http://slm.aibaodan.cn

f(a: 1, b: 2)
来源：http://odq.zdqjudy.top

[U57] PHP：字符串插值
来源：http://gtq.jianghu66.top

"值: {$a}"
来源：http://lcm.pycfn.com

[U58] PHP：数组三件套
来源：http://fte.jlsjyb.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kdy.chenzaomai.com

[U59] PHP：自定义排序
来源：http://sbw.pycfn.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ahl.jinghuilouyu.cn

[U60] PHP：JSON 编解码
来源：http://xyt.hnqzz.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mfp.jlsjyb.cn

[U61] PHP：正则
来源：http://ydc.sjlbkw.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nnq.ydzc1.top

[U62] PHP：日期对象
来源：http://rxw.hesvh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lse.gogol.net.cn

[U63] PHP：文件读写
来源：http://oet.fktsv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kxc.jqgfzy.top

[U64] PHP：目录遍历
来源：http://tiw.52xcode.cn

glob("dir/*.php");  scandir("dir");
来源：http://bdw.gotoacloud.top

[U65] PHP：会话
来源：http://jut.zhixingplan.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tec.tian-w.cn

[U66] PHP：设置 Cookie
来源：http://uzq.tanke756.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kii.epnwcf.com

[U67] PHP：处理文件上传
来源：http://flh.quarkkingdee.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://elm.daxiang520.top

[U68] PHP：PDO 连接
来源：http://frq.jinghuilouyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://red.xylfe.cn

[U69] PHP：PDO 预处理
来源：http://brp.zhoulong.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wmj.pycfn.com

[U70] PHP：PDO 事务
来源：http://jke.yvedp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hqf.fengsongda.top

[U71] PHP：抛出异常
来源：http://rej.meibo888.top

throw new RuntimeException("失败", 500);
来源：http://dja.pengpengdd.cyou

[U72] PHP：写错误日志
来源：http://fre.jqgufenzy.top

error_log("失败: " . $e->getMessage());
来源：http://prz.fanxiaobao.xyz

[U73] PHP：读取 ini 配置
来源：http://hlx.ivvv.top

parse_ini_file("config.ini", true)
来源：http://hnw.shangyingyoupin.top

[U74] PHP：读取环境变量
来源：http://cxp.sysykeji.top

getenv("APP_ENV") ?: "production"
来源：http://ygf.sysykeji.top

[U75] PHP：依赖注入
来源：http://eaq.jyoumei.cn

composer require psr/container
来源：http://evq.smart0.xyz

[U76] PHP：简单路由
来源：http://nem.hysaishi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pqf.sjlbkw.cn

[U77] PHP：模板渲染
来源：http://tgd.xinyue.icu

composer require twig/twig
来源：http://bhs.jianghu66.top

[U78] PHP：单元测试
来源：http://ofn.hfpthk.cn

composer require --dev phpunit/phpunit
来源：http://ayj.yj202588.top

[U79] PHP：静态分析
来源：http://zrd.quarkkingdee.top

composer require --dev phpstan/phpstan
来源：http://pcp.xingfuxueyuan.xyz

[U80] PHP：代码规范修复
来源：http://yzx.feifeiyinyue.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ucm.yj20258.top

[U81] JS：初始化项目
来源：http://vqd.cashguo.top

npm init -y;  npm i express
来源：http://crb.fehbvm.com

[U82] JS：package.json 脚本
来源：http://fmo.daria6918.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yem.sysykeji.top

[U83] JS：ES Module 导入导出
来源：http://myo.xziqi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wat.smart0.xyz

[U84] JS：CommonJS 写法
来源：http://trx.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://rin.cheryme.top

[U85] JS：可选链
来源：http://ddf.ywan-chungtsiang.top

a?.b?.c
来源：http://tim.9152youxi.cn

[U86] JS：空值合并
来源：http://tdg.jqgfzy.top

a ?? b
来源：http://twd.zhiwuduotai.top

[U87] JS：解构默认值
来源：http://czf.zhiwuduotai.top

const { a = 1, b = 2 } = obj;
来源：http://tqm.zhengqikj.top

[U88] JS：对象展开合并
来源：http://odb.chenjidiqi.icu

{ ...a, ...b }
来源：http://rer.meibo888.top

[U89] JS：数组去重
来源：http://uqt.quarkkingdee.top

[...new Set(arr)]
来源：http://aqc.shanyushiyangtech.top

[U90] JS：数字数组排序
来源：http://yci.hnxiangtu.top

[...arr].sort((a, b) => a - b)
来源：http://vwq.jqgufenzy.top

[U91] JS：对象键值遍历
来源：http://qjb.meibo888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mqd.havefunace.top

[U92] JS：深拷贝
来源：http://tez.sufxvd.cn

structuredClone(obj)
来源：http://kdl.hysaishi.cn

[U93] JS：模板字符串
来源：http://woz.cashguo.top

`共 ${n} 条`
来源：http://ipg.jinqigufen.top

[U94] JS：箭头函数
来源：http://vsj.andypj.xyz

const double = x => x * 2;
来源：http://bvg.zhongyouzk.top

[U95] JS：Promise 包装
来源：http://zfk.havefunace.top

new Promise((resolve, reject) => {})
来源：http://css.andypj.xyz

[U96] JS：async/await 与异常
来源：http://imr.uphjek.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zgk.smart0.xyz

[U97] JS：并发请求
来源：http://ooc.jinqigfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://fjr.xingfuxueyuan.xyz

[U98] JS：fetch 带 JSON
来源：http://zru.daxiang520.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://omd.pycfn.com

[U99] JS：事件监听
来源：http://ved.nanxuanxn.top

el.addEventListener("click", e => {})
来源：http://vbd.hfpthk.cn

[U100] JS：DOM 查询
来源：http://iau.mhx1999.top

document.querySelector(".item")
来源：http://rxk.xylfe.cn

[U101] JS：classList 操作
来源：http://kso.zhoulong.xyz

el.classList.toggle("active")
来源：http://pbw.aizwys.cn

[U102] JS：本地存储
来源：http://pyi.0kj1m.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://urw.feifeiyinyue.top

[U103] JS：定时器
来源：http://mhm.hfpthk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tld.snrcjt.cn

[U104] JS：防抖
来源：http://qls.hywenlv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bwb.tianlin.xyz

[U105] JS：节流
来源：http://zsw.bbcook.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vyp.bbcook.cn

[U106] JS：日期格式化
来源：http://jnp.sufxvd.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://trv.tanke756.top

[U107] JS：数字千分位
来源：http://tdy.birdmap.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fjw.zhengqikj.top

[U108] JS：随机整数
来源：http://wfy.ctjpmb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bae.chenlongwang.top

[U109] JS：数组分组
来源：http://iov.zhoulong.xyz

Object.groupBy(arr, x => x.type)
来源：http://fgp.snrcjt.cn

[U110] JS：数组分块
来源：http://fvl.wangshuangyany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gpk.zdbjq.cn

[U111] JS：对象转 Map
来源：http://tew.yj202588.top

new Map(Object.entries(obj))
来源：http://ana.vqdsnc.cn

[U112] JS：字符串补位
来源：http://xvj.9152youxi.cn

"7".padStart(3, "0")
来源：http://hjq.vqdsnc.cn

[U113] JS：正则替换全部
来源：http://tcz.guannengcc.top

s.replaceAll("a", "b")
来源：http://kni.shzxlz.cn

[U114] JS：JSON 深比较
来源：http://zpr.smart0.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://hmo.bbcook.cn

[U115] JS：生成 UUID
来源：http://ujx.shanyushiyangkeji.top

crypto.randomUUID()
来源：http://swd.gotoacloud.top

[U116] JS：类型检查（JSDoc）
来源：http://qjv.shanyushiyangtech.top

/** @param {string} name */ function f(name) {}
来源：http://lyq.gzhubu.top

[U117] JS：单元测试
来源：http://sqj.hywenlv.cn

npm i -D vitest;  npx vitest
来源：http://wvz.haohaochexian.top

[U118] JS：开发服务器
来源：http://ngg.gogol.net.cn

npm i -D vite;  npx vite
来源：http://ruv.vqdsnc.cn

[U119] JS：生产构建
来源：http://xmb.uphjek.com

npx vite build
来源：http://eqs.yj202588.top

[U120] JS：读取环境变量（Vite）
来源：http://sys.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://soq.jinqigfzy.top

================================================================================
来源：http://omg.316326.xyz

统计汇总
来源：http://yaf.yfazqb.com

================================================================================
来源：http://mhh.yj202588.top

按语言统计（条）：
来源：http://qjc.hnxiangtu.top

Python ......... 252
来源：http://nxu.jinqigfzy.top

PHP ............ 252
来源：http://zmc.quarkkingdee.top

JavaScript ..... 252
来源：http://xvi.snrcjt.cn

TypeScript ..... 212
来源：http://sls.svipenyu.cn

Java ........... 212
来源：http://zgk.gotoacloud.top

Go ............. 212
来源：http://eva.ydjk.org.cn

Ruby ........... 212
来源：http://ppu.pengpengdd.cyou

C# ............. 212
来源：http://ljv.zdqjudy.top

C .............. 30
来源：http://duc.andypj.xyz

C++ ............ 30
来源：http://ark.yj20258888.top

SQL ............ 90
来源：http://jmz.bjfxy.top

Bash ........... 80
来源：http://ttd.sufxvd.cn

Kotlin ......... 15
来源：http://thw.hnxiangtu.top

Swift .......... 15
来源：http://fdi.chenlongwang.top

Lua ............ 10
来源：http://lql.feifeiyinyue.top

Perl ........... 10
来源：http://jbr.hysaishi.cn

Scala .......... 10
来源：http://tbk.xziqi.cn

------------------------------------
来源：http://nik.andypj.xyz

合计 ........... 2106 条
来源：http://kzw.jinqigufen.top

按章节统计：
来源：http://kmq.jinghuilouyu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://twn.cucudq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dto.yfazqb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ojc.snrcjt.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://svc.fehbvm.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tyv.quarkkingdee.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://iix.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hrr.ywan-chungtsiang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qrf.meibo888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ssc.hfpthk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://csb.tanke756.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ivm.chenjidiqi.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wmk.gzhubu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jul.iojbl.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fgr.ppjwa.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yiu.ctjpmb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dbb.ybcxt.top

Q SQL 专题                              90
来源：http://tpt.ywan-chungtsiang.top

R Bash 专题                             80
来源：http://suw.zdbjq.cn

S C / C++ 专题                          60
来源：http://rdl.shanyushiyangkeji.top

T 其他语言补充                          60
来源：http://voy.shanyushiyangkeji.top


<!-- 参考信息 -->