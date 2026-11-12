代发 wailian999

val a = 1;  var b = 2
来源：http://wta.nanxinkj.top

[T53] Scala：字符串插值
来源：http://pja.pengpengdd.cyou

s"值: $b"
来源：http://ntc.svipenyu.cn

[T54] Scala：集合映射
来源：http://dju.aizwys.cn

List(1, 2, 3).map(_ * 2)
来源：http://nns.haohaochexian.top

[T55] Scala：集合过滤
来源：http://wpg.svipenyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://esk.0kj1m.cn

[T56] Scala：样例类
来源：http://pxv.yonumen.top

case class User(name: String, age: Int)
来源：http://bmq.chenzaomai.com

[T57] Scala：模式匹配
来源：http://wkf.hywenlv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://thx.0kj1m.cn

[T58] Scala：函数定义
来源：http://rzf.quarkkingdee.top

def add(a: Int, b: Int): Int = a + b
来源：http://hpn.yueranfly.top

[T59] Scala：循环
来源：http://kqp.yanxiufei.cn

for (i <- 1 to 10) println(i)
来源：http://xsc.snrcjt.cn

[T60] Scala：折叠
来源：http://ntp.yj20258888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wfp.zhengqikj.top

================================================================================
来源：http://wzv.bbcook.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://awe.yongpay.top

================================================================================
来源：http://ogm.yangfankeji.com

[U01] Py：创建虚拟环境
来源：http://mev.fktsv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://akv.nanxuanxn.top

[U02] Py：导出 / 安装依赖
来源：http://xkn.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oee.yuanzhike.top

[U03] Py：加载 .env 配置
来源：http://ecj.hfpthk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ilm.ivvv.top

[U04] Py：变量调试打印
来源：http://arh.sxryk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zsk.zycfv.cn

[U05] Py：列表去重且保序
来源：http://ocb.yj202588.top

list(dict.fromkeys(arr))
来源：http://yup.52xcode.cn

[U06] Py：合并两个字典
来源：http://lxg.havefunace.top

{**a, **b}
来源：http://dik.hammf.cn

[U07] Py：反转字典键值
来源：http://ipn.vqdsnc.cn

{v: k for k, v in d.items()}
来源：http://kmb.vehdjk.com

[U08] Py：展平二维列表
来源：http://ugh.sweek.top

[y for x in nested for y in x]
来源：http://sbo.dianchejie.cn

[U09] Py：字典取最大值的键
来源：http://rxr.yj20258.top

max(d, key=d.get)
来源：http://vno.jinqigfzy.top

[U10] Py：按值排序字典
来源：http://ryz.snrcjt.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xix.dianchejie.cn

[U11] Py：生成器表达式
来源：http://vnu.birdmap.top

(x * 2 for x in arr)
来源：http://vsa.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xal.guowangkeji.top

Counter(arr).most_common(3)
来源：http://adt.xziqi.cn

[U13] Py：固定长度队列
来源：http://tdd.hnqzz.top

deque(maxlen=10)
来源：http://wly.gaohongyu789.top

[U14] Py：分组收集到列表
来源：http://yrm.zhoulong.xyz

defaultdict(list)
来源：http://kxk.cqqwz.cn

[U15] Py：高精度计时
来源：http://ymc.xuetiantiany.cn

t = time.perf_counter()
来源：http://nyd.yj202588.top

[U16] Py：命令行参数解析
来源：http://ung.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vmq.zhixingplan.top

[U17] Py：初始化日志
来源：http://hqx.andypj.xyz

logging.basicConfig(level=logging.INFO)
来源：http://zws.wangshuangyany.cn

[U18] Py：预编译正则
来源：http://ueh.yj20258.top

pat = re.compile(r"\d+")
来源：http://apa.ydzc1.top

[U19] Py：正则替换带回调
来源：http://ykm.yfazqb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yti.xuanzx.com

[U20] Py：缓存函数结果
来源：http://wgt.cqqwz.cn

@functools.lru_cache(maxsize=None)
来源：http://vlz.316326.xyz

[U21] Py：自定义上下文管理器
来源：http://hhy.yj202588.top

@contextlib.contextmanager
来源：http://kxs.jinqigufen.top

[U22] Py：矩阵转置
来源：http://uat.wangshuangyany.cn

list(zip(*m))
来源：http://amo.gotoacloud.top

[U23] Py：分块读取大文件
来源：http://zqn.yj202588.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hoh.jinqigufen.top

[U24] Py：路径操作
来源：http://cls.dianchejie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fhw.yanxiufei.cn

[U25] Py：CSV 按字典读
来源：http://bfc.jinqigfzy.top

csv.DictReader(f)
来源：http://cos.316326.xyz

[U26] Py：并发下载
来源：http://mfi.yj202588.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bit.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://qpx.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://sgr.havefunace.top

[U28] Py：类型别名
来源：http://hya.hysaishi.cn

UserId = int
来源：http://dxd.hysaishi.cn

[U29] Py：属性校验
来源：http://esw.hongshengwenyu.top

@property 与 @x.setter 配合
来源：http://gsk.andypj.xyz

[U30] Py：数据类
来源：http://ctk.birdmap.top

@dataclass(slots=True)
来源：http://cdv.zhiwuduotai.top

[U31] Py：单测
来源：http://mwr.shanyushiyangkeji.top

python -m pytest -q
来源：http://tfu.jqgufenzy.top

[U32] Py：代码格式化
来源：http://uec.zhongyouzk.top

ruff format . && ruff check --fix .
来源：http://tuf.zhoulong.xyz

[U33] Py：打包发布
来源：http://pbc.ehwqpu.com

python -m build  （依赖 pyproject.toml）
来源：http://dey.ivvv.top

[U34] Py：判断编码
来源：http://ifc.xziqi.cn

chardet.detect(raw)
来源：http://jru.hysaishi.cn

[U35] Py：发送邮件
来源：http://mtt.fzhhl.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://utd.mhx1999.top

[U36] Py：定时任务
来源：http://dcg.zdqjudy.top

schedule.every(10).minutes.do(job)
来源：http://nea.yj202588.top

[U37] Py：读写 Excel
来源：http://rrj.wangdashe.top

pandas.read_excel / DataFrame.to_excel
来源：http://ekx.zhongyouzk.top

[U38] Py：获取脚本所在目录
来源：http://eyw.fengsongda.top

Path(__file__).resolve().parent
来源：http://sdz.yfazqb.com

[U39] Py：判断是否在交互环境
来源：http://wbz.zdbjq.cn

sys.stdout.isatty()
来源：http://sro.guannengcc.top

[U40] Py：打印到标准错误
来源：http://kun.xuetiantiany.cn

print("err", file=sys.stderr)
来源：http://imh.yfazqb.com

[U41] PHP：初始化 Composer 项目
来源：http://mjv.xuanzx.com

composer init;  composer require guzzlehttp/guzzle
来源：http://pno.redwolf501.top

[U42] PHP：PSR-4 自动加载
来源：http://idw.wangdashe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://akl.chenzaomai.com

[U43] PHP：声明命名空间
来源：http://nne.gotoacloud.top

namespace App\Http;
来源：http://frc.hammf.cn

[U44] PHP：开启严格类型
来源：http://pyq.svipenyu.cn

declare(strict_types=1);
来源：http://ymq.xziqi.cn

[U45] PHP：类型声明与返回类型
来源：http://fjc.dashuyun.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://grf.zhoulong.xyz

[U46] PHP：可空类型
来源：http://kxn.xingfuxueyuan.xyz

?string $name = null
来源：http://otd.zhiwuduotai.top

[U47] PHP：联合类型
来源：http://gbl.jinghuilouyu.cn

int|string $id
来源：http://zyc.chenjidiqi.icu

[U48] PHP：纯枚举
来源：http://wgo.yvedp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nhw.xingfuxueyuan.xyz

[U49] PHP：只读属性
来源：http://jkl.zhaomingkeji.xyz

public readonly string $name
来源：http://pho.jinghuilouyu.cn

[U50] PHP：构造器属性提升
来源：http://slr.chenjidiqi.icu

public function __construct(private int $id) {}
来源：http://qxr.redwolf501.top

[U51] PHP：数组解构
来源：http://xmr.nanxinkj.top

[$a, $b] = $arr;
来源：http://etq.sxryk.cn

[U52] PHP：箭头函数
来源：http://qey.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://gwv.zhijiandao.cn

[U53] PHP：空合并运算符
来源：http://dee.chenzaomai.com

$v = $a ?? $b ?? "default";
来源：http://lih.jinqigufen.top

[U54] PHP：空安全调用
来源：http://hjv.cqqwz.cn

$obj?->method()
来源：http://ooa.svipenyu.cn

[U55] PHP：match 表达式
来源：http://wbc.zhixingplan.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ehf.cashguo.top

[U56] PHP：命名参数
来源：http://tlc.fengsongda.top

f(a: 1, b: 2)
来源：http://zwh.vehdjk.com

[U57] PHP：字符串插值
来源：http://ehj.cqqwz.cn

"值: {$a}"
来源：http://bfo.nwbrower.top

[U58] PHP：数组三件套
来源：http://cdw.svipenyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xly.fzhhl.top

[U59] PHP：自定义排序
来源：http://mli.sjlbkw.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bkx.zhaomingkeji.xyz

[U60] PHP：JSON 编解码
来源：http://eig.smart0.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wmj.pengpengdd.cyou

[U61] PHP：正则
来源：http://axs.hysaishi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wyo.hysaishi.cn

[U62] PHP：日期对象
来源：http://ica.nwbrower.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pqc.ydzc1.top

[U63] PHP：文件读写
来源：http://aai.chenjidiqi.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qjc.jinyuanbaomall.cn

[U64] PHP：目录遍历
来源：http://ekx.bjfxy.top

glob("dir/*.php");  scandir("dir");
来源：http://ptl.hnxiangtu.top

[U65] PHP：会话
来源：http://lmh.zhiwuduotai.top

session_start();  $_SESSION["uid"] = 1;
来源：http://oig.jinqigfzy.top

[U66] PHP：设置 Cookie
来源：http://bay.dashuyun.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hia.tarul.cn

[U67] PHP：处理文件上传
来源：http://fvj.feifeiyinyue.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hnj.chenjidiqi.icu

[U68] PHP：PDO 连接
来源：http://uue.sjlbkw.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://riw.havefunace.top

[U69] PHP：PDO 预处理
来源：http://hqm.zhengqikj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nat.sxryk.cn

[U70] PHP：PDO 事务
来源：http://lgz.hnxiangtu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fjo.wangshuangyany.cn

[U71] PHP：抛出异常
来源：http://kxs.gzhubu.top

throw new RuntimeException("失败", 500);
来源：http://kdu.zdqjudy.top

[U72] PHP：写错误日志
来源：http://kjx.bjfxy.top

error_log("失败: " . $e->getMessage());
来源：http://hzn.hywenlv.cn

[U73] PHP：读取 ini 配置
来源：http://wln.gzhubu.top

parse_ini_file("config.ini", true)
来源：http://yev.zycfv.cn

[U74] PHP：读取环境变量
来源：http://xrh.yangfankeji.com

getenv("APP_ENV") ?: "production"
来源：http://gvl.zhoulong.xyz

[U75] PHP：依赖注入
来源：http://flb.ivvv.top

composer require psr/container
来源：http://vqs.ivvv.top

[U76] PHP：简单路由
来源：http://nva.aibaodan.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dpn.hcnkem.com

[U77] PHP：模板渲染
来源：http://wpq.snrcjt.cn

composer require twig/twig
来源：http://oaz.feifeiyinyue.top

[U78] PHP：单元测试
来源：http://lrm.yj20258.top

composer require --dev phpunit/phpunit
来源：http://qty.jianghu66.top

[U79] PHP：静态分析
来源：http://tlp.kuanghao11.cn

composer require --dev phpstan/phpstan
来源：http://ylj.fengsongda.top

[U80] PHP：代码规范修复
来源：http://buu.cheryme.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ucb.c1oappe.top

[U81] JS：初始化项目
来源：http://hqq.epnwcf.com

npm init -y;  npm i express
来源：http://ldh.guowangkeji.top

[U82] JS：package.json 脚本
来源：http://obo.xingfuxueyuan.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qsf.nanxinkj.top

[U83] JS：ES Module 导入导出
来源：http://slu.sweek.top

export const a = 1;  import { a } from "./m.js";
来源：http://hck.sxryk.cn

[U84] JS：CommonJS 写法
来源：http://ngq.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://ueg.daria6918.cn

[U85] JS：可选链
来源：http://uww.bjfxy.top

a?.b?.c
来源：http://rmj.quarkkingdee.top

[U86] JS：空值合并
来源：http://gdh.tarul.cn

a ?? b
来源：http://lme.52xcode.cn

[U87] JS：解构默认值
来源：http://evy.cheryme.top

const { a = 1, b = 2 } = obj;
来源：http://hav.hnqzz.top

[U88] JS：对象展开合并
来源：http://nxw.hnqzz.top

{ ...a, ...b }
来源：http://qjq.sweek.top

[U89] JS：数组去重
来源：http://idu.xylfe.cn

[...new Set(arr)]
来源：http://npi.haohaochexian.top

[U90] JS：数字数组排序
来源：http://aok.gaohongyu789.top

[...arr].sort((a, b) => a - b)
来源：http://xmv.zycfv.cn

[U91] JS：对象键值遍历
来源：http://mbk.tarul.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://owm.andypj.xyz

[U92] JS：深拷贝
来源：http://twc.nanxinkj.top

structuredClone(obj)
来源：http://ckc.pycfn.com

[U93] JS：模板字符串
来源：http://yzt.aizwys.cn

`共 ${n} 条`
来源：http://vbl.jianghu66.top

[U94] JS：箭头函数
来源：http://sef.hammf.cn

const double = x => x * 2;
来源：http://nos.svipenyu.cn

[U95] JS：Promise 包装
来源：http://lfn.c1oappe.top

new Promise((resolve, reject) => {})
来源：http://dls.sweek.top

[U96] JS：async/await 与异常
来源：http://sgm.316326.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xjq.zycfv.cn

[U97] JS：并发请求
来源：http://iwq.zhoulong.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://hju.cdnleiting.top

[U98] JS：fetch 带 JSON
来源：http://hlb.xingfuxueyuan.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iro.jyoumei.cn

[U99] JS：事件监听
来源：http://pbq.hnxiangtu.top

el.addEventListener("click", e => {})
来源：http://dxb.cucudq.cn

[U100] JS：DOM 查询
来源：http://gtg.nwbrower.top

document.querySelector(".item")
来源：http://rli.cheryme.top

[U101] JS：classList 操作
来源：http://gpe.gaohongyu789.top

el.classList.toggle("active")
来源：http://hff.9152youxi.cn

[U102] JS：本地存储
来源：http://rnn.yj202588.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dfm.zhoulong.xyz

[U103] JS：定时器
来源：http://ege.havefunace.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://smj.fktsv.cn

[U104] JS：防抖
来源：http://ope.gzhubu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qdn.bbcook.cn

[U105] JS：节流
来源：http://ztu.zdqjudy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jrx.cheryme.top

[U106] JS：日期格式化
来源：http://akl.chenzaomai.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qbx.zhixingplan.top

[U107] JS：数字千分位
来源：http://teu.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jfp.jyoumei.cn

[U108] JS：随机整数
来源：http://ckm.andypj.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yld.jinqigfzy.top

[U109] JS：数组分组
来源：http://kyj.shanyushiyangtech.top

Object.groupBy(arr, x => x.type)
来源：http://fai.ybcxt.top

[U110] JS：数组分块
来源：http://cmc.wangdashe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dkd.dashuyun.cn

[U111] JS：对象转 Map
来源：http://ren.jlsjyb.cn

new Map(Object.entries(obj))
来源：http://iew.andypj.xyz

[U112] JS：字符串补位
来源：http://rcw.guowangkeji.top

"7".padStart(3, "0")
来源：http://tyv.guowangkeji.top

[U113] JS：正则替换全部
来源：http://cbw.tian-w.cn

s.replaceAll("a", "b")
来源：http://jpp.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://dto.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hep.hywenlv.cn

[U115] JS：生成 UUID
来源：http://wdm.vqdsnc.cn

crypto.randomUUID()
来源：http://mjj.fehbvm.com

[U116] JS：类型检查（JSDoc）
来源：http://wvi.jyoumei.cn

/** @param {string} name */ function f(name) {}
来源：http://ukk.ywan-chungtsiang.top

[U117] JS：单元测试
来源：http://vob.jiagoushi.top

npm i -D vitest;  npx vitest
来源：http://uja.daria6918.cn

[U118] JS：开发服务器
来源：http://izz.hysaishi.cn

npm i -D vite;  npx vite
来源：http://lug.52xcode.cn

[U119] JS：生产构建
来源：http://fhn.gogol.net.cn

npx vite build
来源：http://syb.yueranfly.top

[U120] JS：读取环境变量（Vite）
来源：http://yqc.sxryk.cn

import.meta.env.VITE_API_URL
来源：http://bjh.yuanzhike.top

================================================================================
来源：http://ywa.tanke756.top

统计汇总
来源：http://aip.yj20258888.top

================================================================================
来源：http://uqy.nanxinkj.top

按语言统计（条）：
来源：http://uwr.gogol.net.cn

Python ......... 252
来源：http://wxy.meibo888.top

PHP ............ 252
来源：http://yko.xinyue.icu

JavaScript ..... 252
来源：http://dcy.tarul.cn

TypeScript ..... 212
来源：http://xbr.jlsjyb.cn

Java ........... 212
来源：http://rcu.ydjk.org.cn

Go ............. 212
来源：http://zia.vehdjk.com

Ruby ........... 212
来源：http://phj.nwbrower.top

C# ............. 212
来源：http://ntf.jqgfzy.top

C .............. 30
来源：http://ggk.yonumen.top

C++ ............ 30
来源：http://kgb.gaohongyu789.top

SQL ............ 90
来源：http://vog.fktsv.cn

Bash ........... 80
来源：http://xzy.ehwqpu.com

Kotlin ......... 15
来源：http://dlk.ctjpmb.com

Swift .......... 15
来源：http://edl.epnwcf.com

Lua ............ 10
来源：http://hbd.daria6918.cn

Perl ........... 10
来源：http://mmw.zycfv.cn

Scala .......... 10
来源：http://cvg.meibo888.top

------------------------------------
来源：http://bol.sjlbkw.cn

合计 ........... 2106 条
来源：http://mpc.yvedp.cn

按章节统计：
来源：http://xuo.jlsjyb.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ngb.vehdjk.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ufb.zhongyouzk.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rre.yj20258888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kin.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mhl.jyoumei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pbs.gotoacloud.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hfl.jianghu66.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jjb.zhixingplan.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qjd.yj20258888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zlw.zhijiandao.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://crk.jianghu66.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hxm.nwbrower.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://niy.pengpengdd.cyou

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ofa.quarkkingdee.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pdp.snrcjt.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lzl.nanxinkj.top


<!-- 参考信息 -->