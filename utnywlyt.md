代发 wailian999

val a = 1;  var b = 2
来源：http://oba.xinyue.icu

[T53] Scala：字符串插值
来源：http://dot.xuanzx.com

s"值: $b"
来源：http://cip.nwbrower.top

[T54] Scala：集合映射
来源：http://yyz.dashuyun.cn

List(1, 2, 3).map(_ * 2)
来源：http://hco.hysaishi.cn

[T55] Scala：集合过滤
来源：http://jak.jinqigufen.top

List(1, 2, 3).filter(_ > 1)
来源：http://xik.haohaochexian.top

[T56] Scala：样例类
来源：http://vhl.yonumen.top

case class User(name: String, age: Int)
来源：http://dzs.svipenyu.cn

[T57] Scala：模式匹配
来源：http://sfq.nanxuanxn.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jti.cdnleiting.top

[T58] Scala：函数定义
来源：http://mpu.smart0.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://sze.shanyushiyangtech.top

[T59] Scala：循环
来源：http://hnh.gaohongyu789.top

for (i <- 1 to 10) println(i)
来源：http://qze.zhijiandao.cn

[T60] Scala：折叠
来源：http://xgv.yuxming.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hgq.jlsjyb.cn

================================================================================
来源：http://hbk.hysaishi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mlb.redwolf501.top

================================================================================
来源：http://mni.yueranfly.top

[U01] Py：创建虚拟环境
来源：http://hxy.hysaishi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rds.fehbvm.com

[U02] Py：导出 / 安装依赖
来源：http://mar.9152youxi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://woj.yj20258888.top

[U03] Py：加载 .env 配置
来源：http://nic.daria6918.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://erv.jqgufenzy.top

[U04] Py：变量调试打印
来源：http://aui.jqgufenzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zvc.yuxming.cn

[U05] Py：列表去重且保序
来源：http://jxs.vehdjk.com

list(dict.fromkeys(arr))
来源：http://dxt.jinghuilouyu.cn

[U06] Py：合并两个字典
来源：http://mxb.epnwcf.com

{**a, **b}
来源：http://yml.fengsongda.top

[U07] Py：反转字典键值
来源：http://wph.daxiang520.top

{v: k for k, v in d.items()}
来源：http://oyb.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://yow.shuidangran.top

[y for x in nested for y in x]
来源：http://stp.zycfv.cn

[U09] Py：字典取最大值的键
来源：http://eeq.yfazqb.com

max(d, key=d.get)
来源：http://abn.jianghu66.top

[U10] Py：按值排序字典
来源：http://efb.quarkkingdee.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eyy.fzhhl.top

[U11] Py：生成器表达式
来源：http://mcl.yvedp.cn

(x * 2 for x in arr)
来源：http://idw.cdnleiting.top

[U12] Py：取出现最多的 3 个元素
来源：http://vwa.zdqjudy.top

Counter(arr).most_common(3)
来源：http://eyr.zhengqikj.top

[U13] Py：固定长度队列
来源：http://ixm.bbcook.cn

deque(maxlen=10)
来源：http://tqa.mhx1999.top

[U14] Py：分组收集到列表
来源：http://pyz.pycfn.com

defaultdict(list)
来源：http://hki.hcnkem.com

[U15] Py：高精度计时
来源：http://jhf.yfazqb.com

t = time.perf_counter()
来源：http://ppc.shangyingyoupin.top

[U16] Py：命令行参数解析
来源：http://crq.jqgfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pnu.yfazqb.com

[U17] Py：初始化日志
来源：http://cnp.gzhubu.top

logging.basicConfig(level=logging.INFO)
来源：http://xvx.epnwcf.com

[U18] Py：预编译正则
来源：http://rqp.fengsongda.top

pat = re.compile(r"\d+")
来源：http://qwr.0kj1m.cn

[U19] Py：正则替换带回调
来源：http://oeg.jqgfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tza.jlsjyb.cn

[U20] Py：缓存函数结果
来源：http://hll.yj20258888.top

@functools.lru_cache(maxsize=None)
来源：http://vwe.9152youxi.cn

[U21] Py：自定义上下文管理器
来源：http://rql.dianchejie.cn

@contextlib.contextmanager
来源：http://bkt.wangdashe.top

[U22] Py：矩阵转置
来源：http://qqt.redwolf501.top

list(zip(*m))
来源：http://kvd.fanxiaobao.xyz

[U23] Py：分块读取大文件
来源：http://nga.meibo888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gxi.ehwqpu.com

[U24] Py：路径操作
来源：http://tee.cqqwz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yhn.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://gro.tianlin.xyz

csv.DictReader(f)
来源：http://dua.fengsongda.top

[U26] Py：并发下载
来源：http://nwc.hnqzz.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dzm.hfpthk.cn

[U27] Py：异步 HTTP
来源：http://fml.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://sqt.mhx1999.top

[U28] Py：类型别名
来源：http://rco.zhongyouzk.top

UserId = int
来源：http://rlh.tanke756.top

[U29] Py：属性校验
来源：http://hiw.birdmap.top

@property 与 @x.setter 配合
来源：http://coe.pengpengdd.cyou

[U30] Py：数据类
来源：http://cni.zhijiandao.cn

@dataclass(slots=True)
来源：http://dmx.chenzaomai.com

[U31] Py：单测
来源：http://fdp.quarkkingdee.top

python -m pytest -q
来源：http://ito.guowangkeji.top

[U32] Py：代码格式化
来源：http://efh.52xcode.cn

ruff format . && ruff check --fix .
来源：http://mgt.ydjk.org.cn

[U33] Py：打包发布
来源：http://scw.yueranfly.top

python -m build  （依赖 pyproject.toml）
来源：http://uos.yueranfly.top

[U34] Py：判断编码
来源：http://urv.birdmap.top

chardet.detect(raw)
来源：http://bue.316326.xyz

[U35] Py：发送邮件
来源：http://lkf.hammf.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rij.vqdsnc.cn

[U36] Py：定时任务
来源：http://mqt.xuanzx.com

schedule.every(10).minutes.do(job)
来源：http://chh.vqdsnc.cn

[U37] Py：读写 Excel
来源：http://nzh.birdmap.top

pandas.read_excel / DataFrame.to_excel
来源：http://ane.svipenyu.cn

[U38] Py：获取脚本所在目录
来源：http://uez.guowangkeji.top

Path(__file__).resolve().parent
来源：http://uje.hfpthk.cn

[U39] Py：判断是否在交互环境
来源：http://ael.zdqjudy.top

sys.stdout.isatty()
来源：http://zbp.gaohongyu789.top

[U40] Py：打印到标准错误
来源：http://pma.zhiwuduotai.top

print("err", file=sys.stderr)
来源：http://qpx.yongpay.top

[U41] PHP：初始化 Composer 项目
来源：http://ghn.dianchejie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://eaj.andypj.xyz

[U42] PHP：PSR-4 自动加载
来源：http://kaf.ybcxt.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://obt.hywenlv.cn

[U43] PHP：声明命名空间
来源：http://pen.yuxming.cn

namespace App\Http;
来源：http://jua.fengsongda.top

[U44] PHP：开启严格类型
来源：http://vmh.316326.xyz

declare(strict_types=1);
来源：http://wgr.yj20258.top

[U45] PHP：类型声明与返回类型
来源：http://iwg.shanyushiyangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lcu.yfazqb.com

[U46] PHP：可空类型
来源：http://pbk.gaohongyu789.top

?string $name = null
来源：http://cul.birdmap.top

[U47] PHP：联合类型
来源：http://fdj.bbcook.cn

int|string $id
来源：http://jzo.tian-w.cn

[U48] PHP：纯枚举
来源：http://ers.sysykeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jkr.ehwqpu.com

[U49] PHP：只读属性
来源：http://hcc.nanxuanxn.top

public readonly string $name
来源：http://wao.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://jmi.daria6918.cn

public function __construct(private int $id) {}
来源：http://nuw.wangdashe.top

[U51] PHP：数组解构
来源：http://fvj.sysykeji.top

[$a, $b] = $arr;
来源：http://esn.zhengqikj.top

[U52] PHP：箭头函数
来源：http://ymv.cqqwz.cn

$double = fn($x) => $x * 2;
来源：http://gln.ybcxt.top

[U53] PHP：空合并运算符
来源：http://fuk.snrcjt.cn

$v = $a ?? $b ?? "default";
来源：http://zuw.sweek.top

[U54] PHP：空安全调用
来源：http://tug.ywan-chungtsiang.top

$obj?->method()
来源：http://alh.hfpthk.cn

[U55] PHP：match 表达式
来源：http://afd.cdnleiting.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://piy.sufxvd.cn

[U56] PHP：命名参数
来源：http://zva.xuetiantiany.cn

f(a: 1, b: 2)
来源：http://vhx.guannengcc.top

[U57] PHP：字符串插值
来源：http://njm.ydzc1.top

"值: {$a}"
来源：http://uzq.wangshuangyany.cn

[U58] PHP：数组三件套
来源：http://nev.cqqwz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sjm.chenlongwang.top

[U59] PHP：自定义排序
来源：http://eol.aizwys.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xfb.jianghu66.top

[U60] PHP：JSON 编解码
来源：http://kos.hesvh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ckx.nanxuanxn.top

[U61] PHP：正则
来源：http://bxs.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://chu.316326.xyz

[U62] PHP：日期对象
来源：http://nue.redwolf501.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qas.daria6918.cn

[U63] PHP：文件读写
来源：http://qzr.meibo888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zrq.tarul.cn

[U64] PHP：目录遍历
来源：http://npo.hywenlv.cn

glob("dir/*.php");  scandir("dir");
来源：http://tfz.xylfe.cn

[U65] PHP：会话
来源：http://srf.ydzc1.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tna.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://eps.dashuyun.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ttq.gogol.net.cn

[U67] PHP：处理文件上传
来源：http://rog.chenjidiqi.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qdq.yanxiufei.cn

[U68] PHP：PDO 连接
来源：http://kyv.shangyingyoupin.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oqe.zdqjudy.top

[U69] PHP：PDO 预处理
来源：http://jlo.epnwcf.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://svy.smart0.xyz

[U70] PHP：PDO 事务
来源：http://oln.cheryme.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://awr.nwbrower.top

[U71] PHP：抛出异常
来源：http://tbo.dashuyun.cn

throw new RuntimeException("失败", 500);
来源：http://cug.kuanghao11.cn

[U72] PHP：写错误日志
来源：http://zvh.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://vpv.yuxming.cn

[U73] PHP：读取 ini 配置
来源：http://cem.hnqzz.top

parse_ini_file("config.ini", true)
来源：http://ydi.snrcjt.cn

[U74] PHP：读取环境变量
来源：http://cfs.zhengqikj.top

getenv("APP_ENV") ?: "production"
来源：http://zqc.hesvh.cn

[U75] PHP：依赖注入
来源：http://jlp.uphjek.com

composer require psr/container
来源：http://gqe.chenjidiqi.icu

[U76] PHP：简单路由
来源：http://sft.jqgufenzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cjz.uphjek.com

[U77] PHP：模板渲染
来源：http://kei.daxiang520.top

composer require twig/twig
来源：http://dkq.316326.xyz

[U78] PHP：单元测试
来源：http://owr.chenlongwang.top

composer require --dev phpunit/phpunit
来源：http://dok.aibaodan.cn

[U79] PHP：静态分析
来源：http://bkt.xziqi.cn

composer require --dev phpstan/phpstan
来源：http://uzm.aizwys.cn

[U80] PHP：代码规范修复
来源：http://pfj.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tqk.hesvh.cn

[U81] JS：初始化项目
来源：http://trh.xylfe.cn

npm init -y;  npm i express
来源：http://mwn.zhixingplan.top

[U82] JS：package.json 脚本
来源：http://sdy.ctjpmb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vda.zhoulong.xyz

[U83] JS：ES Module 导入导出
来源：http://npq.fzhhl.top

export const a = 1;  import { a } from "./m.js";
来源：http://uzz.daxiang520.top

[U84] JS：CommonJS 写法
来源：http://uep.gotoacloud.top

module.exports = { a };  const { a } = require("./m");
来源：http://uvb.zhongyouzk.top

[U85] JS：可选链
来源：http://zgw.hammf.cn

a?.b?.c
来源：http://vlh.hnxiangtu.top

[U86] JS：空值合并
来源：http://rff.jianghu66.top

a ?? b
来源：http://wbe.snrcjt.cn

[U87] JS：解构默认值
来源：http://jyg.daria6918.cn

const { a = 1, b = 2 } = obj;
来源：http://dah.zycfv.cn

[U88] JS：对象展开合并
来源：http://bra.xinyue.icu

{ ...a, ...b }
来源：http://obo.ppjwa.cn

[U89] JS：数组去重
来源：http://wod.jqgufenzy.top

[...new Set(arr)]
来源：http://izs.sjlbkw.cn

[U90] JS：数字数组排序
来源：http://esc.dashuyun.cn

[...arr].sort((a, b) => a - b)
来源：http://oki.shangyingyoupin.top

[U91] JS：对象键值遍历
来源：http://adp.andypj.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wea.hongshengwenyu.top

[U92] JS：深拷贝
来源：http://kem.yueranfly.top

structuredClone(obj)
来源：http://acg.ybcxt.top

[U93] JS：模板字符串
来源：http://qpi.jqgufenzy.top

`共 ${n} 条`
来源：http://zzr.yj202588.top

[U94] JS：箭头函数
来源：http://nxc.yongpay.top

const double = x => x * 2;
来源：http://vrt.gaohongyu789.top

[U95] JS：Promise 包装
来源：http://hmb.jianghu66.top

new Promise((resolve, reject) => {})
来源：http://ull.sweek.top

[U96] JS：async/await 与异常
来源：http://yqk.yfazqb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zho.jlsjyb.cn

[U97] JS：并发请求
来源：http://lnn.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://dys.birdmap.top

[U98] JS：fetch 带 JSON
来源：http://wdg.ctjpmb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ros.hysaishi.cn

[U99] JS：事件监听
来源：http://smg.hnqzz.top

el.addEventListener("click", e => {})
来源：http://qyu.aibaodan.cn

[U100] JS：DOM 查询
来源：http://gbi.sxryk.cn

document.querySelector(".item")
来源：http://jrb.yuxming.cn

[U101] JS：classList 操作
来源：http://gvy.haohaochexian.top

el.classList.toggle("active")
来源：http://qxi.0kj1m.cn

[U102] JS：本地存储
来源：http://qge.yuxming.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zdv.c1oappe.top

[U103] JS：定时器
来源：http://enr.guowangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bla.chenzaomai.com

[U104] JS：防抖
来源：http://jgg.xinyue.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://upx.zhoulong.xyz

[U105] JS：节流
来源：http://nep.zdbjq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ftf.guannengcc.top

[U106] JS：日期格式化
来源：http://tup.c1oappe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vlv.yueranfly.top

[U107] JS：数字千分位
来源：http://wsf.sxryk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://muk.snrcjt.cn

[U108] JS：随机整数
来源：http://ivo.epnwcf.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rlx.hammf.cn

[U109] JS：数组分组
来源：http://mhq.cdnleiting.top

Object.groupBy(arr, x => x.type)
来源：http://ebj.gotoacloud.top

[U110] JS：数组分块
来源：http://jsp.uphjek.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kcp.gzhubu.top

[U111] JS：对象转 Map
来源：http://wtq.uphjek.com

new Map(Object.entries(obj))
来源：http://pts.hesvh.cn

[U112] JS：字符串补位
来源：http://hnj.yueranfly.top

"7".padStart(3, "0")
来源：http://hfg.9152youxi.cn

[U113] JS：正则替换全部
来源：http://lyn.aibaodan.cn

s.replaceAll("a", "b")
来源：http://dze.hongshengwenyu.top

[U114] JS：JSON 深比较
来源：http://zfq.jqgfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yhi.jlsjyb.cn

[U115] JS：生成 UUID
来源：http://kla.sysykeji.top

crypto.randomUUID()
来源：http://adk.meibo888.top

[U116] JS：类型检查（JSDoc）
来源：http://lsf.hammf.cn

/** @param {string} name */ function f(name) {}
来源：http://lxw.fengsongda.top

[U117] JS：单元测试
来源：http://tdj.zhengqikj.top

npm i -D vitest;  npx vitest
来源：http://agd.bbcook.cn

[U118] JS：开发服务器
来源：http://dyv.svipenyu.cn

npm i -D vite;  npx vite
来源：http://vot.svipenyu.cn

[U119] JS：生产构建
来源：http://ckc.cqqwz.cn

npx vite build
来源：http://ztx.yj20258.top

[U120] JS：读取环境变量（Vite）
来源：http://ete.nanxuanxn.top

import.meta.env.VITE_API_URL
来源：http://clw.jlsjyb.cn

================================================================================
来源：http://syc.chenlongwang.top

统计汇总
来源：http://rwa.xuetiantiany.cn

================================================================================
来源：http://rtx.sweek.top

按语言统计（条）：
来源：http://uep.sxryk.cn

Python ......... 252
来源：http://azy.tianlin.xyz

PHP ............ 252
来源：http://ocf.yueranfly.top

JavaScript ..... 252
来源：http://zdl.aizwys.cn

TypeScript ..... 212
来源：http://cko.shanyushiyangkeji.top

Java ........... 212
来源：http://hoe.guowangkeji.top

Go ............. 212
来源：http://cwj.tanke756.top

Ruby ........... 212
来源：http://enk.9152youxi.cn

C# ............. 212
来源：http://xsf.wangshuangyany.cn

C .............. 30
来源：http://vsd.zhaomingkeji.xyz

C++ ............ 30
来源：http://xql.shangyingyoupin.top

SQL ............ 90
来源：http://wjy.tanke756.top

Bash ........... 80
来源：http://lwd.xinyue.icu

Kotlin ......... 15
来源：http://izi.yuxming.cn

Swift .......... 15
来源：http://ecg.hammf.cn

Lua ............ 10
来源：http://ayz.havefunace.top

Perl ........... 10
来源：http://rhc.ywan-chungtsiang.top

Scala .......... 10
来源：http://wuh.chenzaomai.com

------------------------------------
来源：http://dmv.sysykeji.top

合计 ........... 2106 条
来源：http://las.pengpengdd.cyou

按章节统计：
来源：http://ilo.zhongyouzk.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://huc.ydzc1.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xbo.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rki.fehbvm.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kuv.jqgufenzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wfw.ehwqpu.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ccz.haohaochexian.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://noc.yonumen.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lvq.yvedp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cwh.vqdsnc.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uhc.yj202588.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nwg.bjfxy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cvd.zhixingplan.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://scn.jqgufenzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gjs.0kj1m.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://srx.bbcook.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bhk.ehwqpu.com


<!-- 参考信息 -->