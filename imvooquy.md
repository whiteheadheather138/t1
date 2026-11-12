代发 wailian999

[T49] Perl：函数
来源：http://gix.jinqigufen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jry.zycfv.cn

[T50] Perl：逐行读文件
来源：http://gch.jianghu66.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rjs.316326.xyz

while (my $line = <$fh>) { print $line; }
来源：http://xtu.shanyushiyangkeji.top

[T51] Scala：Hello World
来源：http://mua.fehbvm.com

println("Hello")
来源：http://bjl.jianghu66.top

[T52] Scala：变量
来源：http://svp.svipenyu.cn

val a = 1;  var b = 2
来源：http://zck.xinyue.icu

[T53] Scala：字符串插值
来源：http://abv.snrcjt.cn

s"值: $b"
来源：http://zty.zhaomingkeji.xyz

[T54] Scala：集合映射
来源：http://nnx.andypj.xyz

List(1, 2, 3).map(_ * 2)
来源：http://gon.guannengcc.top

[T55] Scala：集合过滤
来源：http://emt.hammf.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hpm.dashuyun.cn

[T56] Scala：样例类
来源：http://pew.zhiwuduotai.top

case class User(name: String, age: Int)
来源：http://vdw.zhaomingkeji.xyz

[T57] Scala：模式匹配
来源：http://zxl.fktsv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://opi.meibo888.top

[T58] Scala：函数定义
来源：http://tlk.sufxvd.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pwb.cdnleiting.top

[T59] Scala：循环
来源：http://xwv.ctjpmb.com

for (i <- 1 to 10) println(i)
来源：http://byy.sweek.top

[T60] Scala：折叠
来源：http://nlb.316326.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ugc.snrcjt.cn

================================================================================
来源：http://zzh.ydjk.org.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baw.vehdjk.com

================================================================================
来源：http://jrv.daria6918.cn

[U01] Py：创建虚拟环境
来源：http://ozz.shangyingyoupin.top

python -m venv .venv && source .venv/bin/activate
来源：http://hts.nwbrower.top

[U02] Py：导出 / 安装依赖
来源：http://pmn.jianghu66.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lsa.hongshengwenyu.top

[U03] Py：加载 .env 配置
来源：http://iiy.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lky.jiagoushi.top

[U04] Py：变量调试打印
来源：http://xtk.snrcjt.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zbd.hysaishi.cn

[U05] Py：列表去重且保序
来源：http://rld.cashguo.top

list(dict.fromkeys(arr))
来源：http://ify.aizwys.cn

[U06] Py：合并两个字典
来源：http://rfy.zhongyouzk.top

{**a, **b}
来源：http://nhu.yanxiufei.cn

[U07] Py：反转字典键值
来源：http://ejf.havefunace.top

{v: k for k, v in d.items()}
来源：http://ine.zhijiandao.cn

[U08] Py：展平二维列表
来源：http://gwy.c1oappe.top

[y for x in nested for y in x]
来源：http://ocv.52xcode.cn

[U09] Py：字典取最大值的键
来源：http://sme.sysykeji.top

max(d, key=d.get)
来源：http://rti.cqqwz.cn

[U10] Py：按值排序字典
来源：http://czz.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mcv.cucudq.cn

[U11] Py：生成器表达式
来源：http://hsv.cqqwz.cn

(x * 2 for x in arr)
来源：http://rmj.zhengqikj.top

[U12] Py：取出现最多的 3 个元素
来源：http://rms.gzhubu.top

Counter(arr).most_common(3)
来源：http://sxz.cashguo.top

[U13] Py：固定长度队列
来源：http://zxv.xuetiantiany.cn

deque(maxlen=10)
来源：http://zhr.jiagoushi.top

[U14] Py：分组收集到列表
来源：http://kdi.havefunace.top

defaultdict(list)
来源：http://mbs.cqqwz.cn

[U15] Py：高精度计时
来源：http://qxk.yj20258.top

t = time.perf_counter()
来源：http://iha.kuanghao11.cn

[U16] Py：命令行参数解析
来源：http://ssd.uphjek.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ngk.jlsjyb.cn

[U17] Py：初始化日志
来源：http://qbf.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://dfv.yj20258888.top

[U18] Py：预编译正则
来源：http://ywz.gaohongyu789.top

pat = re.compile(r"\d+")
来源：http://rgx.daria6918.cn

[U19] Py：正则替换带回调
来源：http://oor.zycfv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bda.hcnkem.com

[U20] Py：缓存函数结果
来源：http://izv.nanxinkj.top

@functools.lru_cache(maxsize=None)
来源：http://eaj.feifeiyinyue.top

[U21] Py：自定义上下文管理器
来源：http://vxa.xingfuxueyuan.xyz

@contextlib.contextmanager
来源：http://pxu.yangfankeji.com

[U22] Py：矩阵转置
来源：http://vvr.hysaishi.cn

list(zip(*m))
来源：http://cou.havefunace.top

[U23] Py：分块读取大文件
来源：http://bot.daxiang520.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ist.vehdjk.com

[U24] Py：路径操作
来源：http://wqq.c1oappe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mgg.cashguo.top

[U25] Py：CSV 按字典读
来源：http://msn.mhx1999.top

csv.DictReader(f)
来源：http://iex.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://mdg.9152youxi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fle.hammf.cn

[U27] Py：异步 HTTP
来源：http://xyx.cheryme.top

aiohttp.ClientSession() 配合 async with
来源：http://pzu.jiagoushi.top

[U28] Py：类型别名
来源：http://oxy.52xcode.cn

UserId = int
来源：http://iar.hnqzz.top

[U29] Py：属性校验
来源：http://rhx.smart0.xyz

@property 与 @x.setter 配合
来源：http://yit.redwolf501.top

[U30] Py：数据类
来源：http://ikd.gzhubu.top

@dataclass(slots=True)
来源：http://ruh.zhoulong.xyz

[U31] Py：单测
来源：http://ndi.yueranfly.top

python -m pytest -q
来源：http://cjh.c1oappe.top

[U32] Py：代码格式化
来源：http://ahf.pycfn.com

ruff format . && ruff check --fix .
来源：http://mxb.uphjek.com

[U33] Py：打包发布
来源：http://ufo.zhengqikj.top

python -m build  （依赖 pyproject.toml）
来源：http://ove.yongpay.top

[U34] Py：判断编码
来源：http://dht.hongshengwenyu.top

chardet.detect(raw)
来源：http://sdp.ywan-chungtsiang.top

[U35] Py：发送邮件
来源：http://vdg.yongpay.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rtd.hysaishi.cn

[U36] Py：定时任务
来源：http://coi.jyoumei.cn

schedule.every(10).minutes.do(job)
来源：http://sat.pycfn.com

[U37] Py：读写 Excel
来源：http://gig.yj202588.top

pandas.read_excel / DataFrame.to_excel
来源：http://qax.xuetiantiany.cn

[U38] Py：获取脚本所在目录
来源：http://rjp.ppjwa.cn

Path(__file__).resolve().parent
来源：http://qxq.gotoacloud.top

[U39] Py：判断是否在交互环境
来源：http://mqq.hysaishi.cn

sys.stdout.isatty()
来源：http://shd.jyoumei.cn

[U40] Py：打印到标准错误
来源：http://pqm.sweek.top

print("err", file=sys.stderr)
来源：http://jja.hfpthk.cn

[U41] PHP：初始化 Composer 项目
来源：http://kdw.ywan-chungtsiang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jze.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://jnl.sweek.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gst.yangfankeji.com

[U43] PHP：声明命名空间
来源：http://kex.yj202588.top

namespace App\Http;
来源：http://lvr.hysaishi.cn

[U44] PHP：开启严格类型
来源：http://cwx.haohaochexian.top

declare(strict_types=1);
来源：http://jyw.bbcook.cn

[U45] PHP：类型声明与返回类型
来源：http://wjn.xziqi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lso.wangshuangyany.cn

[U46] PHP：可空类型
来源：http://sfk.cqqwz.cn

?string $name = null
来源：http://mje.jyoumei.cn

[U47] PHP：联合类型
来源：http://eth.daria6918.cn

int|string $id
来源：http://mbx.xylfe.cn

[U48] PHP：纯枚举
来源：http://yud.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cuz.gogol.net.cn

[U49] PHP：只读属性
来源：http://bez.jqgfzy.top

public readonly string $name
来源：http://qsz.0kj1m.cn

[U50] PHP：构造器属性提升
来源：http://psd.c1oappe.top

public function __construct(private int $id) {}
来源：http://eml.shzxlz.cn

[U51] PHP：数组解构
来源：http://txb.xuanzx.com

[$a, $b] = $arr;
来源：http://ozp.sjlbkw.cn

[U52] PHP：箭头函数
来源：http://tqg.0kj1m.cn

$double = fn($x) => $x * 2;
来源：http://ifj.xuetiantiany.cn

[U53] PHP：空合并运算符
来源：http://dtv.zhongyouzk.top

$v = $a ?? $b ?? "default";
来源：http://ywd.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://jge.jiagoushi.top

$obj?->method()
来源：http://sci.0kj1m.cn

[U55] PHP：match 表达式
来源：http://kjc.tarul.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://anj.zhaomingkeji.xyz

[U56] PHP：命名参数
来源：http://nci.gogol.net.cn

f(a: 1, b: 2)
来源：http://lke.jinqigfzy.top

[U57] PHP：字符串插值
来源：http://cpu.uphjek.com

"值: {$a}"
来源：http://qnj.quarkkingdee.top

[U58] PHP：数组三件套
来源：http://pvj.hnqzz.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hai.smart0.xyz

[U59] PHP：自定义排序
来源：http://tyd.xingfuxueyuan.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hsr.aizwys.cn

[U60] PHP：JSON 编解码
来源：http://prx.hcnkem.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://aef.guannengcc.top

[U61] PHP：正则
来源：http://kar.jyoumei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jwl.zdqjudy.top

[U62] PHP：日期对象
来源：http://tuf.yueranfly.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xwh.yueranfly.top

[U63] PHP：文件读写
来源：http://eeq.nwbrower.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yhu.bjfxy.top

[U64] PHP：目录遍历
来源：http://mte.chenlongwang.top

glob("dir/*.php");  scandir("dir");
来源：http://egi.shangyingyoupin.top

[U65] PHP：会话
来源：http://fyd.cdnleiting.top

session_start();  $_SESSION["uid"] = 1;
来源：http://usx.jinyuanbaomall.cn

[U66] PHP：设置 Cookie
来源：http://iyy.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bhi.vehdjk.com

[U67] PHP：处理文件上传
来源：http://iih.mhx1999.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nhs.quarkkingdee.top

[U68] PHP：PDO 连接
来源：http://bga.andypj.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uhy.hnxiangtu.top

[U69] PHP：PDO 预处理
来源：http://wbr.ybcxt.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dsa.9152youxi.cn

[U70] PHP：PDO 事务
来源：http://zsw.daxiang520.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wjs.zhiwuduotai.top

[U71] PHP：抛出异常
来源：http://rdm.wangdashe.top

throw new RuntimeException("失败", 500);
来源：http://rhj.aizwys.cn

[U72] PHP：写错误日志
来源：http://khg.hesvh.cn

error_log("失败: " . $e->getMessage());
来源：http://nui.sysykeji.top

[U73] PHP：读取 ini 配置
来源：http://obu.sysykeji.top

parse_ini_file("config.ini", true)
来源：http://qsa.cucudq.cn

[U74] PHP：读取环境变量
来源：http://ejc.shanyushiyangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://haz.zhengqikj.top

[U75] PHP：依赖注入
来源：http://unb.jyoumei.cn

composer require psr/container
来源：http://gyh.316326.xyz

[U76] PHP：简单路由
来源：http://zjt.gotoacloud.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://esq.gzhubu.top

[U77] PHP：模板渲染
来源：http://vzz.yongpay.top

composer require twig/twig
来源：http://kmy.ydjk.org.cn

[U78] PHP：单元测试
来源：http://jby.yfazqb.com

composer require --dev phpunit/phpunit
来源：http://kus.yuxming.cn

[U79] PHP：静态分析
来源：http://hwc.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://iam.vehdjk.com

[U80] PHP：代码规范修复
来源：http://nxx.xziqi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sln.xuetiantiany.cn

[U81] JS：初始化项目
来源：http://rsz.svipenyu.cn

npm init -y;  npm i express
来源：http://iwx.zdqjudy.top

[U82] JS：package.json 脚本
来源：http://yki.yangfankeji.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vmu.hesvh.cn

[U83] JS：ES Module 导入导出
来源：http://mgp.fanxiaobao.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://nfr.0kj1m.cn

[U84] JS：CommonJS 写法
来源：http://rae.yj202588.top

module.exports = { a };  const { a } = require("./m");
来源：http://vvu.daxiang520.top

[U85] JS：可选链
来源：http://tpk.andypj.xyz

a?.b?.c
来源：http://kmx.kuanghao11.cn

[U86] JS：空值合并
来源：http://yve.feifeiyinyue.top

a ?? b
来源：http://flx.jinghuilouyu.cn

[U87] JS：解构默认值
来源：http://mwz.zhoulong.xyz

const { a = 1, b = 2 } = obj;
来源：http://kuj.zhixingplan.top

[U88] JS：对象展开合并
来源：http://tyg.zycfv.cn

{ ...a, ...b }
来源：http://wmy.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://pmu.zhijiandao.cn

[...new Set(arr)]
来源：http://hkm.wangdashe.top

[U90] JS：数字数组排序
来源：http://pum.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://tma.jlsjyb.cn

[U91] JS：对象键值遍历
来源：http://omf.9152youxi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://eew.svipenyu.cn

[U92] JS：深拷贝
来源：http://pmi.xziqi.cn

structuredClone(obj)
来源：http://sxk.hywenlv.cn

[U93] JS：模板字符串
来源：http://qzl.zhengqikj.top

`共 ${n} 条`
来源：http://kwq.shanyushiyangtech.top

[U94] JS：箭头函数
来源：http://zaz.yvedp.cn

const double = x => x * 2;
来源：http://mdn.ydjk.org.cn

[U95] JS：Promise 包装
来源：http://zrn.fanxiaobao.xyz

new Promise((resolve, reject) => {})
来源：http://udg.bjfxy.top

[U96] JS：async/await 与异常
来源：http://hdv.xuetiantiany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pqe.9152youxi.cn

[U97] JS：并发请求
来源：http://eus.shanyushiyangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://nic.hfpthk.cn

[U98] JS：fetch 带 JSON
来源：http://ctk.zhongyouzk.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ewe.hammf.cn

[U99] JS：事件监听
来源：http://lkj.hfpthk.cn

el.addEventListener("click", e => {})
来源：http://pou.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://zgk.nanxuanxn.top

document.querySelector(".item")
来源：http://mie.jyoumei.cn

[U101] JS：classList 操作
来源：http://qnj.yj202588.top

el.classList.toggle("active")
来源：http://zyc.cheryme.top

[U102] JS：本地存储
来源：http://uqm.zhengqikj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rwm.jiagoushi.top

[U103] JS：定时器
来源：http://ivs.cashguo.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://woy.pycfn.com

[U104] JS：防抖
来源：http://bjd.gotoacloud.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lwv.chenlongwang.top

[U105] JS：节流
来源：http://nzj.hnqzz.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kpz.yfazqb.com

[U106] JS：日期格式化
来源：http://jeq.xinyue.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://swk.yj20258.top

[U107] JS：数字千分位
来源：http://dbm.sysykeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nkd.jyoumei.cn

[U108] JS：随机整数
来源：http://ztr.bjfxy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uhr.cheryme.top

[U109] JS：数组分组
来源：http://ebv.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://fih.cucudq.cn

[U110] JS：数组分块
来源：http://bco.sjlbkw.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zik.hammf.cn

[U111] JS：对象转 Map
来源：http://rhj.zdqjudy.top

new Map(Object.entries(obj))
来源：http://apl.yangfankeji.com

[U112] JS：字符串补位
来源：http://eik.sjlbkw.cn

"7".padStart(3, "0")
来源：http://wau.pengpengdd.cyou

[U113] JS：正则替换全部
来源：http://wpb.xingfuxueyuan.xyz

s.replaceAll("a", "b")
来源：http://plt.xziqi.cn

[U114] JS：JSON 深比较
来源：http://bvb.ivvv.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://swp.cashguo.top

[U115] JS：生成 UUID
来源：http://wba.jyoumei.cn

crypto.randomUUID()
来源：http://agb.ehwqpu.com

[U116] JS：类型检查（JSDoc）
来源：http://gvk.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://mao.vehdjk.com

[U117] JS：单元测试
来源：http://hnc.feifeiyinyue.top

npm i -D vitest;  npx vitest
来源：http://olp.chenjidiqi.icu

[U118] JS：开发服务器
来源：http://lek.redwolf501.top

npm i -D vite;  npx vite
来源：http://tmw.yuanzhike.top

[U119] JS：生产构建
来源：http://fso.birdmap.top

npx vite build
来源：http://xta.zhengqikj.top

[U120] JS：读取环境变量（Vite）
来源：http://tjg.ydzc1.top

import.meta.env.VITE_API_URL
来源：http://aqd.jyoumei.cn

================================================================================
来源：http://ebf.redwolf501.top

统计汇总
来源：http://ebs.yvedp.cn

================================================================================
来源：http://pml.shzxlz.cn

按语言统计（条）：
来源：http://pdo.fzhhl.top

Python ......... 252
来源：http://ebs.fanxiaobao.xyz

PHP ............ 252
来源：http://dte.fzhhl.top

JavaScript ..... 252
来源：http://ico.shanyushiyangtech.top

TypeScript ..... 212
来源：http://isn.xinyue.icu

Java ........... 212
来源：http://nyd.9152youxi.cn

Go ............. 212
来源：http://rsm.chenlongwang.top

Ruby ........... 212
来源：http://lya.yvedp.cn

C# ............. 212
来源：http://ktw.tarul.cn

C .............. 30
来源：http://mjp.quarkkingdee.top

C++ ............ 30
来源：http://vog.snrcjt.cn

SQL ............ 90
来源：http://tkh.guannengcc.top

Bash ........... 80
来源：http://gag.xuanzx.com

Kotlin ......... 15
来源：http://uyl.fktsv.cn

Swift .......... 15
来源：http://wcw.cashguo.top

Lua ............ 10
来源：http://gny.nanxinkj.top

Perl ........... 10
来源：http://cwq.sufxvd.cn

Scala .......... 10
来源：http://rsz.hnqzz.top

------------------------------------
来源：http://siz.snrcjt.cn

合计 ........... 2106 条
来源：http://sry.ehwqpu.com

按章节统计：
来源：http://lxt.hammf.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hrc.aizwys.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jdn.jianghu66.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://knc.cucudq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://scn.jinghuilouyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://omr.aibaodan.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zkv.cheryme.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cxy.zdqjudy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zlv.fengsongda.top


<!-- 参考信息 -->