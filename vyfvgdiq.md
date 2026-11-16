代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://djl.shangyingyoupin.top

[T51] Scala：Hello World
来源：http://fnu.tarul.cn

println("Hello")
来源：http://nvh.fzhhl.top

[T52] Scala：变量
来源：http://ypt.zhiwuduotai.top

val a = 1;  var b = 2
来源：http://vwd.jinqigufen.top

[T53] Scala：字符串插值
来源：http://ebg.ctjpmb.com

s"值: $b"
来源：http://gak.sweek.top

[T54] Scala：集合映射
来源：http://xmx.birdmap.top

List(1, 2, 3).map(_ * 2)
来源：http://okp.cucudq.cn

[T55] Scala：集合过滤
来源：http://zqr.zhaomingkeji.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://kon.sysykeji.top

[T56] Scala：样例类
来源：http://mvk.tarul.cn

case class User(name: String, age: Int)
来源：http://dga.yvedp.cn

[T57] Scala：模式匹配
来源：http://hwg.daria6918.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ucw.xylfe.cn

[T58] Scala：函数定义
来源：http://wdv.yongpay.top

def add(a: Int, b: Int): Int = a + b
来源：http://asu.shanyushiyangkeji.top

[T59] Scala：循环
来源：http://mrm.jiagoushi.top

for (i <- 1 to 10) println(i)
来源：http://fpa.chenzaomai.com

[T60] Scala：折叠
来源：http://hyg.bbcook.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wkq.hysaishi.cn

================================================================================
来源：http://dnk.quarkkingdee.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wed.xingfuxueyuan.xyz

================================================================================
来源：http://ure.yfazqb.com

[U01] Py：创建虚拟环境
来源：http://azc.zycfv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sfa.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://jno.smart0.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sfk.yongpay.top

[U03] Py：加载 .env 配置
来源：http://qav.gotoacloud.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ede.feifeiyinyue.top

[U04] Py：变量调试打印
来源：http://yuu.epnwcf.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fvt.fehbvm.com

[U05] Py：列表去重且保序
来源：http://fyv.gogol.net.cn

list(dict.fromkeys(arr))
来源：http://jon.ctjpmb.com

[U06] Py：合并两个字典
来源：http://eah.jyoumei.cn

{**a, **b}
来源：http://pnk.xuetiantiany.cn

[U07] Py：反转字典键值
来源：http://kis.jianghu66.top

{v: k for k, v in d.items()}
来源：http://bou.jinqigfzy.top

[U08] Py：展平二维列表
来源：http://lpa.shanyushiyangtech.top

[y for x in nested for y in x]
来源：http://crz.fktsv.cn

[U09] Py：字典取最大值的键
来源：http://vcs.yj202588.top

max(d, key=d.get)
来源：http://plu.fengsongda.top

[U10] Py：按值排序字典
来源：http://pam.bjfxy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ymd.yanxiufei.cn

[U11] Py：生成器表达式
来源：http://ubd.kuanghao11.cn

(x * 2 for x in arr)
来源：http://bgx.tianlin.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://aot.vqdsnc.cn

Counter(arr).most_common(3)
来源：http://iej.kuanghao11.cn

[U13] Py：固定长度队列
来源：http://ebc.vqdsnc.cn

deque(maxlen=10)
来源：http://hxt.zhoulong.xyz

[U14] Py：分组收集到列表
来源：http://txp.jiagoushi.top

defaultdict(list)
来源：http://ytd.shanyushiyangtech.top

[U15] Py：高精度计时
来源：http://zie.shangyingyoupin.top

t = time.perf_counter()
来源：http://hfp.ywan-chungtsiang.top

[U16] Py：命令行参数解析
来源：http://ciq.quarkkingdee.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dst.sjlbkw.cn

[U17] Py：初始化日志
来源：http://txv.zycfv.cn

logging.basicConfig(level=logging.INFO)
来源：http://hjh.shanyushiyangkeji.top

[U18] Py：预编译正则
来源：http://qgf.316326.xyz

pat = re.compile(r"\d+")
来源：http://ref.shangyingyoupin.top

[U19] Py：正则替换带回调
来源：http://cuo.cucudq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mot.gzhubu.top

[U20] Py：缓存函数结果
来源：http://esk.c1oappe.top

@functools.lru_cache(maxsize=None)
来源：http://lhz.jlsjyb.cn

[U21] Py：自定义上下文管理器
来源：http://jwx.cqqwz.cn

@contextlib.contextmanager
来源：http://jcy.cdnleiting.top

[U22] Py：矩阵转置
来源：http://ciz.aizwys.cn

list(zip(*m))
来源：http://uzu.hnqzz.top

[U23] Py：分块读取大文件
来源：http://xgc.zdbjq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lsn.birdmap.top

[U24] Py：路径操作
来源：http://kru.gotoacloud.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nof.vqdsnc.cn

[U25] Py：CSV 按字典读
来源：http://htm.zycfv.cn

csv.DictReader(f)
来源：http://fka.nwbrower.top

[U26] Py：并发下载
来源：http://jyx.mhx1999.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dio.guowangkeji.top

[U27] Py：异步 HTTP
来源：http://yjh.jinyuanbaomall.cn

aiohttp.ClientSession() 配合 async with
来源：http://xfy.yfazqb.com

[U28] Py：类型别名
来源：http://gnb.hnxiangtu.top

UserId = int
来源：http://nzu.ydjk.org.cn

[U29] Py：属性校验
来源：http://qnh.jinqigfzy.top

@property 与 @x.setter 配合
来源：http://amm.uphjek.com

[U30] Py：数据类
来源：http://jbn.chenjidiqi.icu

@dataclass(slots=True)
来源：http://hsm.yuxming.cn

[U31] Py：单测
来源：http://jhg.hfpthk.cn

python -m pytest -q
来源：http://dcl.jqgfzy.top

[U32] Py：代码格式化
来源：http://fiw.guowangkeji.top

ruff format . && ruff check --fix .
来源：http://zlm.gogol.net.cn

[U33] Py：打包发布
来源：http://bqj.52xcode.cn

python -m build  （依赖 pyproject.toml）
来源：http://coy.jiagoushi.top

[U34] Py：判断编码
来源：http://apx.cheryme.top

chardet.detect(raw)
来源：http://tur.vqdsnc.cn

[U35] Py：发送邮件
来源：http://ydq.aizwys.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pmi.chenlongwang.top

[U36] Py：定时任务
来源：http://bai.fzhhl.top

schedule.every(10).minutes.do(job)
来源：http://rvt.iojbl.cn

[U37] Py：读写 Excel
来源：http://dkz.zhijiandao.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bss.shanyushiyangkeji.top

[U38] Py：获取脚本所在目录
来源：http://hfx.yueranfly.top

Path(__file__).resolve().parent
来源：http://yhb.hnxiangtu.top

[U39] Py：判断是否在交互环境
来源：http://bkk.yfazqb.com

sys.stdout.isatty()
来源：http://cfs.c1oappe.top

[U40] Py：打印到标准错误
来源：http://qzr.xingfuxueyuan.xyz

print("err", file=sys.stderr)
来源：http://mqk.aibaodan.cn

[U41] PHP：初始化 Composer 项目
来源：http://dca.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://aga.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://mmk.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qux.vehdjk.com

[U43] PHP：声明命名空间
来源：http://doi.0kj1m.cn

namespace App\Http;
来源：http://xce.xylfe.cn

[U44] PHP：开启严格类型
来源：http://yxx.guannengcc.top

declare(strict_types=1);
来源：http://ehj.xylfe.cn

[U45] PHP：类型声明与返回类型
来源：http://wab.gaohongyu789.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zrl.chenzaomai.com

[U46] PHP：可空类型
来源：http://bhk.sweek.top

?string $name = null
来源：http://esw.yuxming.cn

[U47] PHP：联合类型
来源：http://jfc.zhixingplan.top

int|string $id
来源：http://hjc.fehbvm.com

[U48] PHP：纯枚举
来源：http://hol.gzhubu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bbr.snrcjt.cn

[U49] PHP：只读属性
来源：http://vfy.ydzc1.top

public readonly string $name
来源：http://moo.dashuyun.cn

[U50] PHP：构造器属性提升
来源：http://sbj.aibaodan.cn

public function __construct(private int $id) {}
来源：http://rcv.ctjpmb.com

[U51] PHP：数组解构
来源：http://gym.c1oappe.top

[$a, $b] = $arr;
来源：http://tza.yvedp.cn

[U52] PHP：箭头函数
来源：http://wud.mhx1999.top

$double = fn($x) => $x * 2;
来源：http://tkq.vehdjk.com

[U53] PHP：空合并运算符
来源：http://hrh.yanxiufei.cn

$v = $a ?? $b ?? "default";
来源：http://guw.xziqi.cn

[U54] PHP：空安全调用
来源：http://joi.hnxiangtu.top

$obj?->method()
来源：http://bwp.shangyingyoupin.top

[U55] PHP：match 表达式
来源：http://npo.ywan-chungtsiang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uxk.hnxiangtu.top

[U56] PHP：命名参数
来源：http://amr.jiagoushi.top

f(a: 1, b: 2)
来源：http://pvl.xuanzx.com

[U57] PHP：字符串插值
来源：http://zzq.yangfankeji.com

"值: {$a}"
来源：http://coe.guowangkeji.top

[U58] PHP：数组三件套
来源：http://hhv.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wah.bjfxy.top

[U59] PHP：自定义排序
来源：http://fcr.sysykeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wmj.cucudq.cn

[U60] PHP：JSON 编解码
来源：http://msn.kuanghao11.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ltj.yueranfly.top

[U61] PHP：正则
来源：http://ebq.epnwcf.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wct.zhengqikj.top

[U62] PHP：日期对象
来源：http://tdq.xylfe.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pow.epnwcf.com

[U63] PHP：文件读写
来源：http://zqx.fehbvm.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hhr.ybcxt.top

[U64] PHP：目录遍历
来源：http://lff.aizwys.cn

glob("dir/*.php");  scandir("dir");
来源：http://ppu.zhixingplan.top

[U65] PHP：会话
来源：http://yzy.cqqwz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://arx.shzxlz.cn

[U66] PHP：设置 Cookie
来源：http://pnl.havefunace.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uvq.dianchejie.cn

[U67] PHP：处理文件上传
来源：http://qhj.jianghu66.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mdl.yanxiufei.cn

[U68] PHP：PDO 连接
来源：http://cxa.cashguo.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rnz.nanxuanxn.top

[U69] PHP：PDO 预处理
来源：http://vja.yonumen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cme.smart0.xyz

[U70] PHP：PDO 事务
来源：http://ldn.shangyingyoupin.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://imc.guannengcc.top

[U71] PHP：抛出异常
来源：http://waz.meibo888.top

throw new RuntimeException("失败", 500);
来源：http://sjz.feifeiyinyue.top

[U72] PHP：写错误日志
来源：http://vmk.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://liu.hongshengwenyu.top

[U73] PHP：读取 ini 配置
来源：http://snv.zhengqikj.top

parse_ini_file("config.ini", true)
来源：http://sfx.cashguo.top

[U74] PHP：读取环境变量
来源：http://eqc.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://fpo.yvedp.cn

[U75] PHP：依赖注入
来源：http://hnk.jinyuanbaomall.cn

composer require psr/container
来源：http://rsx.zhaomingkeji.xyz

[U76] PHP：简单路由
来源：http://lle.vqdsnc.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yof.tarul.cn

[U77] PHP：模板渲染
来源：http://wtn.yuxming.cn

composer require twig/twig
来源：http://ckn.wangdashe.top

[U78] PHP：单元测试
来源：http://yxz.ivvv.top

composer require --dev phpunit/phpunit
来源：http://fwd.zdqjudy.top

[U79] PHP：静态分析
来源：http://xhu.c1oappe.top

composer require --dev phpstan/phpstan
来源：http://opv.zhaomingkeji.xyz

[U80] PHP：代码规范修复
来源：http://pxg.jyoumei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ant.shanyushiyangtech.top

[U81] JS：初始化项目
来源：http://xus.dianchejie.cn

npm init -y;  npm i express
来源：http://vtw.0kj1m.cn

[U82] JS：package.json 脚本
来源：http://fvp.haohaochexian.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jww.yuxming.cn

[U83] JS：ES Module 导入导出
来源：http://med.pengpengdd.cyou

export const a = 1;  import { a } from "./m.js";
来源：http://cir.feifeiyinyue.top

[U84] JS：CommonJS 写法
来源：http://ukz.shanyushiyangtech.top

module.exports = { a };  const { a } = require("./m");
来源：http://zuc.316326.xyz

[U85] JS：可选链
来源：http://wac.tianlin.xyz

a?.b?.c
来源：http://qhg.zhengqikj.top

[U86] JS：空值合并
来源：http://bpa.dashuyun.cn

a ?? b
来源：http://zhy.hywenlv.cn

[U87] JS：解构默认值
来源：http://awi.nanxuanxn.top

const { a = 1, b = 2 } = obj;
来源：http://pcb.pycfn.com

[U88] JS：对象展开合并
来源：http://hms.hcnkem.com

{ ...a, ...b }
来源：http://gsc.gzhubu.top

[U89] JS：数组去重
来源：http://nnk.shanyushiyangtech.top

[...new Set(arr)]
来源：http://epi.jiagoushi.top

[U90] JS：数字数组排序
来源：http://rtn.wangdashe.top

[...arr].sort((a, b) => a - b)
来源：http://kkw.ybcxt.top

[U91] JS：对象键值遍历
来源：http://mah.hnqzz.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://crc.ctjpmb.com

[U92] JS：深拷贝
来源：http://jpq.vqdsnc.cn

structuredClone(obj)
来源：http://zsi.jiagoushi.top

[U93] JS：模板字符串
来源：http://mcw.shangyingyoupin.top

`共 ${n} 条`
来源：http://dgf.sjlbkw.cn

[U94] JS：箭头函数
来源：http://wjj.meibo888.top

const double = x => x * 2;
来源：http://niv.tarul.cn

[U95] JS：Promise 包装
来源：http://nno.zhongyouzk.top

new Promise((resolve, reject) => {})
来源：http://cuz.c1oappe.top

[U96] JS：async/await 与异常
来源：http://dli.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ngi.sufxvd.cn

[U97] JS：并发请求
来源：http://nvb.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://owq.52xcode.cn

[U98] JS：fetch 带 JSON
来源：http://jfd.meibo888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tmn.uphjek.com

[U99] JS：事件监听
来源：http://mup.hysaishi.cn

el.addEventListener("click", e => {})
来源：http://vvk.chenjidiqi.icu

[U100] JS：DOM 查询
来源：http://xxd.sweek.top

document.querySelector(".item")
来源：http://bhj.aizwys.cn

[U101] JS：classList 操作
来源：http://tyt.jinghuilouyu.cn

el.classList.toggle("active")
来源：http://ezr.fanxiaobao.xyz

[U102] JS：本地存储
来源：http://ksb.sweek.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zrc.wangdashe.top

[U103] JS：定时器
来源：http://doa.sufxvd.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qdd.cashguo.top

[U104] JS：防抖
来源：http://hvn.snrcjt.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nsn.jqgufenzy.top

[U105] JS：节流
来源：http://ajv.xuetiantiany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uss.ywan-chungtsiang.top

[U106] JS：日期格式化
来源：http://zqh.yonumen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dlj.jianghu66.top

[U107] JS：数字千分位
来源：http://ghc.gotoacloud.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mow.nanxuanxn.top

[U108] JS：随机整数
来源：http://okq.ybcxt.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://npd.fktsv.cn

[U109] JS：数组分组
来源：http://rqx.haohaochexian.top

Object.groupBy(arr, x => x.type)
来源：http://cbq.jiagoushi.top

[U110] JS：数组分块
来源：http://upr.c1oappe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ipm.hysaishi.cn

[U111] JS：对象转 Map
来源：http://psg.gogol.net.cn

new Map(Object.entries(obj))
来源：http://xbl.xinyue.icu

[U112] JS：字符串补位
来源：http://kch.jinyuanbaomall.cn

"7".padStart(3, "0")
来源：http://mqx.jinyuanbaomall.cn

[U113] JS：正则替换全部
来源：http://bnk.meibo888.top

s.replaceAll("a", "b")
来源：http://yks.uphjek.com

[U114] JS：JSON 深比较
来源：http://ayz.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xsp.uphjek.com

[U115] JS：生成 UUID
来源：http://unm.yj20258.top

crypto.randomUUID()
来源：http://ujn.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://mbh.dianchejie.cn

/** @param {string} name */ function f(name) {}
来源：http://uqw.vqdsnc.cn

[U117] JS：单元测试
来源：http://src.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://qni.tanke756.top

[U118] JS：开发服务器
来源：http://vgn.snrcjt.cn

npm i -D vite;  npx vite
来源：http://lis.sjlbkw.cn

[U119] JS：生产构建
来源：http://rjq.chenzaomai.com

npx vite build
来源：http://tli.nanxuanxn.top

[U120] JS：读取环境变量（Vite）
来源：http://jmp.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://erv.sysykeji.top

================================================================================
来源：http://hiw.svipenyu.cn

统计汇总
来源：http://giu.cucudq.cn

================================================================================
来源：http://hkx.9152youxi.cn

按语言统计（条）：
来源：http://rwg.hywenlv.cn

Python ......... 252
来源：http://vrt.yangfankeji.com

PHP ............ 252
来源：http://ebe.52xcode.cn

JavaScript ..... 252
来源：http://jns.cqqwz.cn

TypeScript ..... 212
来源：http://ivd.hnqzz.top

Java ........... 212
来源：http://vhx.zhengqikj.top

Go ............. 212
来源：http://fqr.snrcjt.cn

Ruby ........... 212
来源：http://rfo.cdnleiting.top

C# ............. 212
来源：http://lhh.zhijiandao.cn

C .............. 30
来源：http://tvh.zdbjq.cn

C++ ............ 30
来源：http://gfg.hfpthk.cn

SQL ............ 90
来源：http://mwe.tian-w.cn

Bash ........... 80
来源：http://cni.kuanghao11.cn

Kotlin ......... 15
来源：http://dcs.ppjwa.cn

Swift .......... 15
来源：http://zlt.xingfuxueyuan.xyz

Lua ............ 10
来源：http://nla.meibo888.top

Perl ........... 10
来源：http://jji.meibo888.top

Scala .......... 10
来源：http://odg.jiagoushi.top

------------------------------------
来源：http://jnv.jianghu66.top

合计 ........... 2106 条
来源：http://dnf.xylfe.cn

按章节统计：
来源：http://lio.pengpengdd.cyou

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://foj.tianlin.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tuj.uphjek.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wro.xziqi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hss.gogol.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lhy.fehbvm.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bvg.daria6918.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xoa.yongpay.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vgh.gotoacloud.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oqt.hesvh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ezj.yongpay.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ndd.epnwcf.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ucd.epnwcf.com


<!-- 参考信息 -->