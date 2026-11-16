代发 wailian999

val a = 1;  var b = 2
来源：http://ntv.xuanzx.com

[T53] Scala：字符串插值
来源：http://rcr.52xcode.cn

s"值: $b"
来源：http://ptv.vehdjk.com

[T54] Scala：集合映射
来源：http://tda.jqgfzy.top

List(1, 2, 3).map(_ * 2)
来源：http://gre.xuanzx.com

[T55] Scala：集合过滤
来源：http://vdh.cdnleiting.top

List(1, 2, 3).filter(_ > 1)
来源：http://rzf.tarul.cn

[T56] Scala：样例类
来源：http://vyu.xingfuxueyuan.xyz

case class User(name: String, age: Int)
来源：http://zmc.cdnleiting.top

[T57] Scala：模式匹配
来源：http://fqq.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://iyp.yonumen.top

[T58] Scala：函数定义
来源：http://lol.hysaishi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jqc.uphjek.com

[T59] Scala：循环
来源：http://ltz.vehdjk.com

for (i <- 1 to 10) println(i)
来源：http://omv.meibo888.top

[T60] Scala：折叠
来源：http://ouz.xingfuxueyuan.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ilf.hongshengwenyu.top

================================================================================
来源：http://qtf.aibaodan.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fai.birdmap.top

================================================================================
来源：http://aua.zhiwuduotai.top

[U01] Py：创建虚拟环境
来源：http://zjn.yfazqb.com

python -m venv .venv && source .venv/bin/activate
来源：http://vbc.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://zhj.zhengqikj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ehh.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://xkt.hongshengwenyu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kmv.sysykeji.top

[U04] Py：变量调试打印
来源：http://phw.wangdashe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ggq.daxiang520.top

[U05] Py：列表去重且保序
来源：http://ezc.hammf.cn

list(dict.fromkeys(arr))
来源：http://qel.zhaomingkeji.xyz

[U06] Py：合并两个字典
来源：http://uka.shzxlz.cn

{**a, **b}
来源：http://ecy.jiagoushi.top

[U07] Py：反转字典键值
来源：http://jgq.pengpengdd.cyou

{v: k for k, v in d.items()}
来源：http://mnq.gogol.net.cn

[U08] Py：展平二维列表
来源：http://txu.0kj1m.cn

[y for x in nested for y in x]
来源：http://ttd.zdbjq.cn

[U09] Py：字典取最大值的键
来源：http://bpj.cqqwz.cn

max(d, key=d.get)
来源：http://lou.sweek.top

[U10] Py：按值排序字典
来源：http://byb.yuxming.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ukz.fengsongda.top

[U11] Py：生成器表达式
来源：http://mag.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://fpl.redwolf501.top

[U12] Py：取出现最多的 3 个元素
来源：http://cbm.yfazqb.com

Counter(arr).most_common(3)
来源：http://iyg.guowangkeji.top

[U13] Py：固定长度队列
来源：http://pom.52xcode.cn

deque(maxlen=10)
来源：http://ira.shuidangran.top

[U14] Py：分组收集到列表
来源：http://tjn.vqdsnc.cn

defaultdict(list)
来源：http://epi.xinyue.icu

[U15] Py：高精度计时
来源：http://aok.yj20258.top

t = time.perf_counter()
来源：http://ihj.ehwqpu.com

[U16] Py：命令行参数解析
来源：http://kev.shzxlz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pxb.yvedp.cn

[U17] Py：初始化日志
来源：http://gia.shanyushiyangtech.top

logging.basicConfig(level=logging.INFO)
来源：http://zub.nanxinkj.top

[U18] Py：预编译正则
来源：http://cyc.ctjpmb.com

pat = re.compile(r"\d+")
来源：http://rjg.tianlin.xyz

[U19] Py：正则替换带回调
来源：http://fpf.tarul.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bvi.zhijiandao.cn

[U20] Py：缓存函数结果
来源：http://hts.xylfe.cn

@functools.lru_cache(maxsize=None)
来源：http://ajx.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://vxm.bjfxy.top

@contextlib.contextmanager
来源：http://jdt.zhaomingkeji.xyz

[U22] Py：矩阵转置
来源：http://tpd.ywan-chungtsiang.top

list(zip(*m))
来源：http://trr.cucudq.cn

[U23] Py：分块读取大文件
来源：http://wmf.xuetiantiany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ezc.hammf.cn

[U24] Py：路径操作
来源：http://qpn.jqgfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ubj.gogol.net.cn

[U25] Py：CSV 按字典读
来源：http://zwb.9152youxi.cn

csv.DictReader(f)
来源：http://kmn.guannengcc.top

[U26] Py：并发下载
来源：http://otp.gotoacloud.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tdh.zhoulong.xyz

[U27] Py：异步 HTTP
来源：http://gqc.hfpthk.cn

aiohttp.ClientSession() 配合 async with
来源：http://qvo.mhx1999.top

[U28] Py：类型别名
来源：http://yjc.ivvv.top

UserId = int
来源：http://jlp.sjlbkw.cn

[U29] Py：属性校验
来源：http://dsx.bjfxy.top

@property 与 @x.setter 配合
来源：http://dit.yangfankeji.com

[U30] Py：数据类
来源：http://dgf.zdqjudy.top

@dataclass(slots=True)
来源：http://rxt.pengpengdd.cyou

[U31] Py：单测
来源：http://ckh.nwbrower.top

python -m pytest -q
来源：http://nsd.xingfuxueyuan.xyz

[U32] Py：代码格式化
来源：http://qru.shanyushiyangtech.top

ruff format . && ruff check --fix .
来源：http://nfs.zhoulong.xyz

[U33] Py：打包发布
来源：http://swa.cdnleiting.top

python -m build  （依赖 pyproject.toml）
来源：http://kls.ywan-chungtsiang.top

[U34] Py：判断编码
来源：http://hqu.jinqigufen.top

chardet.detect(raw)
来源：http://qeg.daria6918.cn

[U35] Py：发送邮件
来源：http://oqu.yj202588.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yxy.fehbvm.com

[U36] Py：定时任务
来源：http://mzr.fktsv.cn

schedule.every(10).minutes.do(job)
来源：http://kcm.dashuyun.cn

[U37] Py：读写 Excel
来源：http://qer.jinghuilouyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tvg.yj202588.top

[U38] Py：获取脚本所在目录
来源：http://xws.yueranfly.top

Path(__file__).resolve().parent
来源：http://mce.tarul.cn

[U39] Py：判断是否在交互环境
来源：http://nds.feifeiyinyue.top

sys.stdout.isatty()
来源：http://ode.shanyushiyangtech.top

[U40] Py：打印到标准错误
来源：http://ebj.wangshuangyany.cn

print("err", file=sys.stderr)
来源：http://qkb.gogol.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://csh.sysykeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ybk.jinghuilouyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://fzm.andypj.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uui.sysykeji.top

[U43] PHP：声明命名空间
来源：http://pzo.jiagoushi.top

namespace App\Http;
来源：http://ifs.jqgfzy.top

[U44] PHP：开启严格类型
来源：http://tqk.xingfuxueyuan.xyz

declare(strict_types=1);
来源：http://elr.svipenyu.cn

[U45] PHP：类型声明与返回类型
来源：http://roq.meibo888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hfr.cheryme.top

[U46] PHP：可空类型
来源：http://wjd.gzhubu.top

?string $name = null
来源：http://yuj.svipenyu.cn

[U47] PHP：联合类型
来源：http://knq.haohaochexian.top

int|string $id
来源：http://irl.xinyue.icu

[U48] PHP：纯枚举
来源：http://ikd.redwolf501.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ufs.hongshengwenyu.top

[U49] PHP：只读属性
来源：http://kiw.sysykeji.top

public readonly string $name
来源：http://gom.yangfankeji.com

[U50] PHP：构造器属性提升
来源：http://jdw.sweek.top

public function __construct(private int $id) {}
来源：http://cja.fanxiaobao.xyz

[U51] PHP：数组解构
来源：http://miw.jqgfzy.top

[$a, $b] = $arr;
来源：http://lqi.sufxvd.cn

[U52] PHP：箭头函数
来源：http://qut.zhiwuduotai.top

$double = fn($x) => $x * 2;
来源：http://zbo.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://xta.daxiang520.top

$v = $a ?? $b ?? "default";
来源：http://odc.quarkkingdee.top

[U54] PHP：空安全调用
来源：http://why.cdnleiting.top

$obj?->method()
来源：http://ivy.zhiwuduotai.top

[U55] PHP：match 表达式
来源：http://usm.c1oappe.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://log.nwbrower.top

[U56] PHP：命名参数
来源：http://pve.guowangkeji.top

f(a: 1, b: 2)
来源：http://wzq.wangshuangyany.cn

[U57] PHP：字符串插值
来源：http://xao.fehbvm.com

"值: {$a}"
来源：http://rvu.chenlongwang.top

[U58] PHP：数组三件套
来源：http://cdb.aizwys.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fkj.zhongyouzk.top

[U59] PHP：自定义排序
来源：http://jwi.sxryk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://svo.xziqi.cn

[U60] PHP：JSON 编解码
来源：http://xbv.bjfxy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gli.epnwcf.com

[U61] PHP：正则
来源：http://pep.aizwys.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ykp.shanyushiyangtech.top

[U62] PHP：日期对象
来源：http://rby.cdnleiting.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ici.jqgufenzy.top

[U63] PHP：文件读写
来源：http://lds.shuidangran.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tgc.jyoumei.cn

[U64] PHP：目录遍历
来源：http://cgw.jinqigfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://ais.meibo888.top

[U65] PHP：会话
来源：http://iic.xuanzx.com

session_start();  $_SESSION["uid"] = 1;
来源：http://nfy.jqgfzy.top

[U66] PHP：设置 Cookie
来源：http://olw.shanyushiyangkeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kyw.hcnkem.com

[U67] PHP：处理文件上传
来源：http://vyj.svipenyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uik.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://hle.hnxiangtu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bku.xuanzx.com

[U69] PHP：PDO 预处理
来源：http://sok.zhiwuduotai.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jcr.ybcxt.top

[U70] PHP：PDO 事务
来源：http://pgu.gaohongyu789.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://krb.ehwqpu.com

[U71] PHP：抛出异常
来源：http://hkd.jiagoushi.top

throw new RuntimeException("失败", 500);
来源：http://aic.jiagoushi.top

[U72] PHP：写错误日志
来源：http://yor.0kj1m.cn

error_log("失败: " . $e->getMessage());
来源：http://rbp.epnwcf.com

[U73] PHP：读取 ini 配置
来源：http://mxm.dashuyun.cn

parse_ini_file("config.ini", true)
来源：http://lga.uphjek.com

[U74] PHP：读取环境变量
来源：http://ixw.cdnleiting.top

getenv("APP_ENV") ?: "production"
来源：http://hgi.hfpthk.cn

[U75] PHP：依赖注入
来源：http://oeh.chenjidiqi.icu

composer require psr/container
来源：http://ksm.wangdashe.top

[U76] PHP：简单路由
来源：http://alk.shanyushiyangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zcw.sjlbkw.cn

[U77] PHP：模板渲染
来源：http://vux.svipenyu.cn

composer require twig/twig
来源：http://ora.hongshengwenyu.top

[U78] PHP：单元测试
来源：http://nlr.bbcook.cn

composer require --dev phpunit/phpunit
来源：http://xnr.mhx1999.top

[U79] PHP：静态分析
来源：http://fqn.pycfn.com

composer require --dev phpstan/phpstan
来源：http://iav.jinqigufen.top

[U80] PHP：代码规范修复
来源：http://kyy.zhoulong.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://oxc.andypj.xyz

[U81] JS：初始化项目
来源：http://rbh.yj20258888.top

npm init -y;  npm i express
来源：http://xxm.yuxming.cn

[U82] JS：package.json 脚本
来源：http://bgq.shangyingyoupin.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qta.jiagoushi.top

[U83] JS：ES Module 导入导出
来源：http://amm.zhongyouzk.top

export const a = 1;  import { a } from "./m.js";
来源：http://ngu.0kj1m.cn

[U84] JS：CommonJS 写法
来源：http://ekx.aibaodan.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tti.jinghuilouyu.cn

[U85] JS：可选链
来源：http://nic.snrcjt.cn

a?.b?.c
来源：http://pbd.tian-w.cn

[U86] JS：空值合并
来源：http://ddx.fehbvm.com

a ?? b
来源：http://qjj.cdnleiting.top

[U87] JS：解构默认值
来源：http://rjj.yongpay.top

const { a = 1, b = 2 } = obj;
来源：http://uev.hfpthk.cn

[U88] JS：对象展开合并
来源：http://vfo.guowangkeji.top

{ ...a, ...b }
来源：http://crg.316326.xyz

[U89] JS：数组去重
来源：http://eyy.wangshuangyany.cn

[...new Set(arr)]
来源：http://wdy.andypj.xyz

[U90] JS：数字数组排序
来源：http://epd.haohaochexian.top

[...arr].sort((a, b) => a - b)
来源：http://soq.fehbvm.com

[U91] JS：对象键值遍历
来源：http://jvq.gotoacloud.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mix.fanxiaobao.xyz

[U92] JS：深拷贝
来源：http://ewi.jyoumei.cn

structuredClone(obj)
来源：http://emy.c1oappe.top

[U93] JS：模板字符串
来源：http://apu.quarkkingdee.top

`共 ${n} 条`
来源：http://dxk.dashuyun.cn

[U94] JS：箭头函数
来源：http://snz.guowangkeji.top

const double = x => x * 2;
来源：http://paz.sufxvd.cn

[U95] JS：Promise 包装
来源：http://qun.gzhubu.top

new Promise((resolve, reject) => {})
来源：http://vbp.aibaodan.cn

[U96] JS：async/await 与异常
来源：http://gxu.ppjwa.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xow.tian-w.cn

[U97] JS：并发请求
来源：http://qtd.kuanghao11.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ymw.vehdjk.com

[U98] JS：fetch 带 JSON
来源：http://cxa.ehwqpu.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://opy.jqgufenzy.top

[U99] JS：事件监听
来源：http://yam.birdmap.top

el.addEventListener("click", e => {})
来源：http://epc.jiagoushi.top

[U100] JS：DOM 查询
来源：http://xzo.feifeiyinyue.top

document.querySelector(".item")
来源：http://bns.yongpay.top

[U101] JS：classList 操作
来源：http://ujo.xingfuxueyuan.xyz

el.classList.toggle("active")
来源：http://wcc.uphjek.com

[U102] JS：本地存储
来源：http://pra.guowangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://isz.daria6918.cn

[U103] JS：定时器
来源：http://zrm.vqdsnc.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cau.zycfv.cn

[U104] JS：防抖
来源：http://hle.pengpengdd.cyou

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nfp.havefunace.top

[U105] JS：节流
来源：http://ujc.hnxiangtu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eee.xuanzx.com

[U106] JS：日期格式化
来源：http://rfv.jianghu66.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://png.snrcjt.cn

[U107] JS：数字千分位
来源：http://hds.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bah.aizwys.cn

[U108] JS：随机整数
来源：http://mqn.ydzc1.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mnl.xingfuxueyuan.xyz

[U109] JS：数组分组
来源：http://hhe.fktsv.cn

Object.groupBy(arr, x => x.type)
来源：http://kgr.zhoulong.xyz

[U110] JS：数组分块
来源：http://ror.gaohongyu789.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iwe.zhoulong.xyz

[U111] JS：对象转 Map
来源：http://lbj.yj20258.top

new Map(Object.entries(obj))
来源：http://yqd.xinyue.icu

[U112] JS：字符串补位
来源：http://siy.gaohongyu789.top

"7".padStart(3, "0")
来源：http://zdr.c1oappe.top

[U113] JS：正则替换全部
来源：http://rbi.316326.xyz

s.replaceAll("a", "b")
来源：http://tum.dashuyun.cn

[U114] JS：JSON 深比较
来源：http://mws.hnxiangtu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hqo.fanxiaobao.xyz

[U115] JS：生成 UUID
来源：http://idx.wangshuangyany.cn

crypto.randomUUID()
来源：http://jrb.sweek.top

[U116] JS：类型检查（JSDoc）
来源：http://iry.shanyushiyangtech.top

/** @param {string} name */ function f(name) {}
来源：http://wmq.daria6918.cn

[U117] JS：单元测试
来源：http://bvn.guannengcc.top

npm i -D vitest;  npx vitest
来源：http://jdr.jinqigufen.top

[U118] JS：开发服务器
来源：http://qwn.hesvh.cn

npm i -D vite;  npx vite
来源：http://vhn.zhengqikj.top

[U119] JS：生产构建
来源：http://gua.shangyingyoupin.top

npx vite build
来源：http://pwh.9152youxi.cn

[U120] JS：读取环境变量（Vite）
来源：http://gap.shzxlz.cn

import.meta.env.VITE_API_URL
来源：http://iej.0kj1m.cn

================================================================================
来源：http://eps.hywenlv.cn

统计汇总
来源：http://jnd.chenjidiqi.icu

================================================================================
来源：http://rwn.andypj.xyz

按语言统计（条）：
来源：http://mwc.pycfn.com

Python ......... 252
来源：http://nmo.jinyuanbaomall.cn

PHP ............ 252
来源：http://whm.jyoumei.cn

JavaScript ..... 252
来源：http://tut.jinqigfzy.top

TypeScript ..... 212
来源：http://xsw.pengpengdd.cyou

Java ........... 212
来源：http://dqf.ydzc1.top

Go ............. 212
来源：http://pck.9152youxi.cn

Ruby ........... 212
来源：http://nqk.chenzaomai.com

C# ............. 212
来源：http://ovo.yongpay.top

C .............. 30
来源：http://iuk.hammf.cn

C++ ............ 30
来源：http://oap.mhx1999.top

SQL ............ 90
来源：http://ntw.birdmap.top

Bash ........... 80
来源：http://wpd.cheryme.top

Kotlin ......... 15
来源：http://uqg.meibo888.top

Swift .......... 15
来源：http://wwk.epnwcf.com

Lua ............ 10
来源：http://wfp.shuidangran.top

Perl ........... 10
来源：http://mwq.jiagoushi.top

Scala .......... 10
来源：http://myr.gotoacloud.top

------------------------------------
来源：http://hpt.52xcode.cn

合计 ........... 2106 条
来源：http://iiu.jinqigufen.top

按章节统计：
来源：http://cpl.yj202588.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dzg.jyoumei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tyq.chenzaomai.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zce.cheryme.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://czx.ywan-chungtsiang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wqb.daxiang520.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nxd.zhoulong.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rbz.vehdjk.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://szd.zdqjudy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yyx.52xcode.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zfe.gaohongyu789.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xmu.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vnd.hcnkem.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jtk.feifeiyinyue.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kbx.tian-w.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pfh.jqgufenzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bat.zdbjq.cn


<!-- 参考信息 -->