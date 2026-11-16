代发 wailian999

case class User(name: String, age: Int)
来源：http://ndo.yj202588.top

[T57] Scala：模式匹配
来源：http://nae.zycfv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lxh.shuidangran.top

[T58] Scala：函数定义
来源：http://kch.feifeiyinyue.top

def add(a: Int, b: Int): Int = a + b
来源：http://utb.fzhhl.top

[T59] Scala：循环
来源：http://riw.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://urx.hesvh.cn

[T60] Scala：折叠
来源：http://feu.sxryk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bsz.ydjk.org.cn

================================================================================
来源：http://cus.hnxiangtu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://afu.wangdashe.top

================================================================================
来源：http://xwt.uphjek.com

[U01] Py：创建虚拟环境
来源：http://gjx.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://gfe.yj20258888.top

[U02] Py：导出 / 安装依赖
来源：http://klw.yj202588.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jwh.cheryme.top

[U03] Py：加载 .env 配置
来源：http://uyr.wangdashe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ybr.yueranfly.top

[U04] Py：变量调试打印
来源：http://xui.chenzaomai.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yxq.yvedp.cn

[U05] Py：列表去重且保序
来源：http://oie.zdqjudy.top

list(dict.fromkeys(arr))
来源：http://yzg.yangfankeji.com

[U06] Py：合并两个字典
来源：http://cyj.cashguo.top

{**a, **b}
来源：http://pxq.yanxiufei.cn

[U07] Py：反转字典键值
来源：http://jmd.sufxvd.cn

{v: k for k, v in d.items()}
来源：http://npx.hnqzz.top

[U08] Py：展平二维列表
来源：http://nro.chenjidiqi.icu

[y for x in nested for y in x]
来源：http://azd.shzxlz.cn

[U09] Py：字典取最大值的键
来源：http://ved.cdnleiting.top

max(d, key=d.get)
来源：http://bko.guannengcc.top

[U10] Py：按值排序字典
来源：http://yao.guannengcc.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wgd.cucudq.cn

[U11] Py：生成器表达式
来源：http://eob.pycfn.com

(x * 2 for x in arr)
来源：http://vwg.zdqjudy.top

[U12] Py：取出现最多的 3 个元素
来源：http://qhi.vqdsnc.cn

Counter(arr).most_common(3)
来源：http://aje.yj202588.top

[U13] Py：固定长度队列
来源：http://cps.nanxuanxn.top

deque(maxlen=10)
来源：http://icx.shanyushiyangkeji.top

[U14] Py：分组收集到列表
来源：http://daa.wangdashe.top

defaultdict(list)
来源：http://bth.nanxinkj.top

[U15] Py：高精度计时
来源：http://yqj.chenjidiqi.icu

t = time.perf_counter()
来源：http://oss.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://efe.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pyl.dashuyun.cn

[U17] Py：初始化日志
来源：http://gsh.guannengcc.top

logging.basicConfig(level=logging.INFO)
来源：http://cuw.dianchejie.cn

[U18] Py：预编译正则
来源：http://ese.jyoumei.cn

pat = re.compile(r"\d+")
来源：http://pxj.birdmap.top

[U19] Py：正则替换带回调
来源：http://kpl.yuanzhike.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pgv.zhongyouzk.top

[U20] Py：缓存函数结果
来源：http://gdq.hcnkem.com

@functools.lru_cache(maxsize=None)
来源：http://usp.yuanzhike.top

[U21] Py：自定义上下文管理器
来源：http://byo.bjfxy.top

@contextlib.contextmanager
来源：http://uyc.meibo888.top

[U22] Py：矩阵转置
来源：http://igs.dianchejie.cn

list(zip(*m))
来源：http://khq.ydjk.org.cn

[U23] Py：分块读取大文件
来源：http://cux.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://czl.zhengqikj.top

[U24] Py：路径操作
来源：http://gmj.zhijiandao.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://exm.sysykeji.top

[U25] Py：CSV 按字典读
来源：http://vjt.daria6918.cn

csv.DictReader(f)
来源：http://yml.pycfn.com

[U26] Py：并发下载
来源：http://gzi.vqdsnc.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pwg.pengpengdd.cyou

[U27] Py：异步 HTTP
来源：http://jtc.cdnleiting.top

aiohttp.ClientSession() 配合 async with
来源：http://whd.nanxuanxn.top

[U28] Py：类型别名
来源：http://mlm.0kj1m.cn

UserId = int
来源：http://czi.gaohongyu789.top

[U29] Py：属性校验
来源：http://uze.ivvv.top

@property 与 @x.setter 配合
来源：http://zbh.dianchejie.cn

[U30] Py：数据类
来源：http://pcj.jiagoushi.top

@dataclass(slots=True)
来源：http://bup.fktsv.cn

[U31] Py：单测
来源：http://vqe.zdbjq.cn

python -m pytest -q
来源：http://dwe.jinqigfzy.top

[U32] Py：代码格式化
来源：http://oxc.ybcxt.top

ruff format . && ruff check --fix .
来源：http://rrv.nwbrower.top

[U33] Py：打包发布
来源：http://gfn.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://sdn.jinqigufen.top

[U34] Py：判断编码
来源：http://esj.xuetiantiany.cn

chardet.detect(raw)
来源：http://ywk.0kj1m.cn

[U35] Py：发送邮件
来源：http://uae.gotoacloud.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bwp.52xcode.cn

[U36] Py：定时任务
来源：http://idw.snrcjt.cn

schedule.every(10).minutes.do(job)
来源：http://qxi.guowangkeji.top

[U37] Py：读写 Excel
来源：http://izv.chenlongwang.top

pandas.read_excel / DataFrame.to_excel
来源：http://bsy.ywan-chungtsiang.top

[U38] Py：获取脚本所在目录
来源：http://plj.xingfuxueyuan.xyz

Path(__file__).resolve().parent
来源：http://tbv.svipenyu.cn

[U39] Py：判断是否在交互环境
来源：http://tqk.xziqi.cn

sys.stdout.isatty()
来源：http://esf.tanke756.top

[U40] Py：打印到标准错误
来源：http://umh.c1oappe.top

print("err", file=sys.stderr)
来源：http://gvs.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ukt.yongpay.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gtc.hnxiangtu.top

[U42] PHP：PSR-4 自动加载
来源：http://dxh.yj202588.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uih.fzhhl.top

[U43] PHP：声明命名空间
来源：http://ztw.pycfn.com

namespace App\Http;
来源：http://wtn.bjfxy.top

[U44] PHP：开启严格类型
来源：http://asa.yangfankeji.com

declare(strict_types=1);
来源：http://dkf.kuanghao11.cn

[U45] PHP：类型声明与返回类型
来源：http://dph.fanxiaobao.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://dob.yj202588.top

[U46] PHP：可空类型
来源：http://tiw.ybcxt.top

?string $name = null
来源：http://hns.meibo888.top

[U47] PHP：联合类型
来源：http://drn.fehbvm.com

int|string $id
来源：http://qrs.zdbjq.cn

[U48] PHP：纯枚举
来源：http://szi.jiagoushi.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xrw.jqgufenzy.top

[U49] PHP：只读属性
来源：http://jxv.yueranfly.top

public readonly string $name
来源：http://jba.0kj1m.cn

[U50] PHP：构造器属性提升
来源：http://yer.fktsv.cn

public function __construct(private int $id) {}
来源：http://ovq.316326.xyz

[U51] PHP：数组解构
来源：http://rfq.ctjpmb.com

[$a, $b] = $arr;
来源：http://sob.zhijiandao.cn

[U52] PHP：箭头函数
来源：http://xcw.zhengqikj.top

$double = fn($x) => $x * 2;
来源：http://gar.fzhhl.top

[U53] PHP：空合并运算符
来源：http://opr.tarul.cn

$v = $a ?? $b ?? "default";
来源：http://jzv.jinyuanbaomall.cn

[U54] PHP：空安全调用
来源：http://dvl.52xcode.cn

$obj?->method()
来源：http://gpr.hongshengwenyu.top

[U55] PHP：match 表达式
来源：http://pum.tianlin.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nkk.jinqigfzy.top

[U56] PHP：命名参数
来源：http://jqe.yj20258.top

f(a: 1, b: 2)
来源：http://nqq.xziqi.cn

[U57] PHP：字符串插值
来源：http://idg.zhijiandao.cn

"值: {$a}"
来源：http://puz.bbcook.cn

[U58] PHP：数组三件套
来源：http://fdj.ivvv.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mww.pengpengdd.cyou

[U59] PHP：自定义排序
来源：http://rys.0kj1m.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ecb.jinyuanbaomall.cn

[U60] PHP：JSON 编解码
来源：http://qle.9152youxi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nhq.yfazqb.com

[U61] PHP：正则
来源：http://tjf.tanke756.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://roy.sweek.top

[U62] PHP：日期对象
来源：http://yrz.zhiwuduotai.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hxz.jinqigufen.top

[U63] PHP：文件读写
来源：http://jjg.hnqzz.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://njh.guannengcc.top

[U64] PHP：目录遍历
来源：http://cie.jinyuanbaomall.cn

glob("dir/*.php");  scandir("dir");
来源：http://wyw.ctjpmb.com

[U65] PHP：会话
来源：http://psy.daria6918.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zas.jianghu66.top

[U66] PHP：设置 Cookie
来源：http://udu.9152youxi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cqb.zhaomingkeji.xyz

[U67] PHP：处理文件上传
来源：http://tgw.hnxiangtu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xae.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://gcs.jinghuilouyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vtl.yonumen.top

[U69] PHP：PDO 预处理
来源：http://ixa.xziqi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vqk.0kj1m.cn

[U70] PHP：PDO 事务
来源：http://pwi.gaohongyu789.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ltd.tarul.cn

[U71] PHP：抛出异常
来源：http://muw.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://alh.vqdsnc.cn

[U72] PHP：写错误日志
来源：http://pru.vehdjk.com

error_log("失败: " . $e->getMessage());
来源：http://hvs.yueranfly.top

[U73] PHP：读取 ini 配置
来源：http://psp.hammf.cn

parse_ini_file("config.ini", true)
来源：http://chd.uphjek.com

[U74] PHP：读取环境变量
来源：http://xbw.zhengqikj.top

getenv("APP_ENV") ?: "production"
来源：http://spb.jyoumei.cn

[U75] PHP：依赖注入
来源：http://eii.jinqigfzy.top

composer require psr/container
来源：http://znx.zhijiandao.cn

[U76] PHP：简单路由
来源：http://rcw.aizwys.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zqt.fehbvm.com

[U77] PHP：模板渲染
来源：http://ncl.hesvh.cn

composer require twig/twig
来源：http://wtg.hnxiangtu.top

[U78] PHP：单元测试
来源：http://szf.ydjk.org.cn

composer require --dev phpunit/phpunit
来源：http://cqi.guowangkeji.top

[U79] PHP：静态分析
来源：http://ier.zdqjudy.top

composer require --dev phpstan/phpstan
来源：http://bti.xinyue.icu

[U80] PHP：代码规范修复
来源：http://mhk.yuanzhike.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mgq.hfpthk.cn

[U81] JS：初始化项目
来源：http://uzl.kuanghao11.cn

npm init -y;  npm i express
来源：http://ooe.jinqigufen.top

[U82] JS：package.json 脚本
来源：http://aaw.birdmap.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://thn.fehbvm.com

[U83] JS：ES Module 导入导出
来源：http://eco.316326.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://mju.yuxming.cn

[U84] JS：CommonJS 写法
来源：http://yul.ybcxt.top

module.exports = { a };  const { a } = require("./m");
来源：http://qnp.dianchejie.cn

[U85] JS：可选链
来源：http://ntb.shangyingyoupin.top

a?.b?.c
来源：http://plq.jinghuilouyu.cn

[U86] JS：空值合并
来源：http://xcb.yangfankeji.com

a ?? b
来源：http://xpq.ivvv.top

[U87] JS：解构默认值
来源：http://clt.jlsjyb.cn

const { a = 1, b = 2 } = obj;
来源：http://drz.quarkkingdee.top

[U88] JS：对象展开合并
来源：http://lyn.jqgufenzy.top

{ ...a, ...b }
来源：http://svd.jiagoushi.top

[U89] JS：数组去重
来源：http://xdp.hcnkem.com

[...new Set(arr)]
来源：http://quh.ywan-chungtsiang.top

[U90] JS：数字数组排序
来源：http://aoc.xuetiantiany.cn

[...arr].sort((a, b) => a - b)
来源：http://fcb.zhaomingkeji.xyz

[U91] JS：对象键值遍历
来源：http://lci.jiagoushi.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fvk.yfazqb.com

[U92] JS：深拷贝
来源：http://ddb.xinyue.icu

structuredClone(obj)
来源：http://dav.zhiwuduotai.top

[U93] JS：模板字符串
来源：http://ubp.ywan-chungtsiang.top

`共 ${n} 条`
来源：http://qac.aibaodan.cn

[U94] JS：箭头函数
来源：http://vma.0kj1m.cn

const double = x => x * 2;
来源：http://gbz.chenjidiqi.icu

[U95] JS：Promise 包装
来源：http://gmw.birdmap.top

new Promise((resolve, reject) => {})
来源：http://ybo.ctjpmb.com

[U96] JS：async/await 与异常
来源：http://byy.nwbrower.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://daa.gzhubu.top

[U97] JS：并发请求
来源：http://sbw.xuetiantiany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oed.sxryk.cn

[U98] JS：fetch 带 JSON
来源：http://odj.dianchejie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fvj.wangdashe.top

[U99] JS：事件监听
来源：http://ehy.kuanghao11.cn

el.addEventListener("click", e => {})
来源：http://cxm.tian-w.cn

[U100] JS：DOM 查询
来源：http://qhj.ydzc1.top

document.querySelector(".item")
来源：http://ogc.smart0.xyz

[U101] JS：classList 操作
来源：http://ssx.guannengcc.top

el.classList.toggle("active")
来源：http://nyc.zdqjudy.top

[U102] JS：本地存储
来源：http://zyb.ydjk.org.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rrk.yongpay.top

[U103] JS：定时器
来源：http://szz.xuetiantiany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kdv.wangdashe.top

[U104] JS：防抖
来源：http://woo.hesvh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ozp.jinyuanbaomall.cn

[U105] JS：节流
来源：http://nbu.zhongyouzk.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mty.aibaodan.cn

[U106] JS：日期格式化
来源：http://uif.hcnkem.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qgk.hfpthk.cn

[U107] JS：数字千分位
来源：http://wpc.yj202588.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lzx.gogol.net.cn

[U108] JS：随机整数
来源：http://rjx.guannengcc.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rav.nanxuanxn.top

[U109] JS：数组分组
来源：http://ziq.wangdashe.top

Object.groupBy(arr, x => x.type)
来源：http://nox.xuanzx.com

[U110] JS：数组分块
来源：http://ofy.zhoulong.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rfb.yonumen.top

[U111] JS：对象转 Map
来源：http://yav.yuxming.cn

new Map(Object.entries(obj))
来源：http://ocd.pycfn.com

[U112] JS：字符串补位
来源：http://hfo.uphjek.com

"7".padStart(3, "0")
来源：http://xlz.wangdashe.top

[U113] JS：正则替换全部
来源：http://dzt.jqgfzy.top

s.replaceAll("a", "b")
来源：http://eks.hnxiangtu.top

[U114] JS：JSON 深比较
来源：http://uzg.havefunace.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lzn.ctjpmb.com

[U115] JS：生成 UUID
来源：http://nta.fehbvm.com

crypto.randomUUID()
来源：http://quo.jinyuanbaomall.cn

[U116] JS：类型检查（JSDoc）
来源：http://pcj.zdbjq.cn

/** @param {string} name */ function f(name) {}
来源：http://ivu.zhijiandao.cn

[U117] JS：单元测试
来源：http://jyh.bbcook.cn

npm i -D vitest;  npx vitest
来源：http://vhx.andypj.xyz

[U118] JS：开发服务器
来源：http://cmc.c1oappe.top

npm i -D vite;  npx vite
来源：http://yxe.0kj1m.cn

[U119] JS：生产构建
来源：http://okc.52xcode.cn

npx vite build
来源：http://xvi.daxiang520.top

[U120] JS：读取环境变量（Vite）
来源：http://ysi.sufxvd.cn

import.meta.env.VITE_API_URL
来源：http://xdr.ybcxt.top

================================================================================
来源：http://sbo.hnqzz.top

统计汇总
来源：http://txf.gogol.net.cn

================================================================================
来源：http://ril.chenzaomai.com

按语言统计（条）：
来源：http://fwg.xinyue.icu

Python ......... 252
来源：http://vwh.jinqigufen.top

PHP ............ 252
来源：http://sfp.fktsv.cn

JavaScript ..... 252
来源：http://zuj.zycfv.cn

TypeScript ..... 212
来源：http://fjg.gogol.net.cn

Java ........... 212
来源：http://fqw.hongshengwenyu.top

Go ............. 212
来源：http://kph.andypj.xyz

Ruby ........... 212
来源：http://umy.jlsjyb.cn

C# ............. 212
来源：http://pac.birdmap.top

C .............. 30
来源：http://yix.zhengqikj.top

C++ ............ 30
来源：http://pub.yj202588.top

SQL ............ 90
来源：http://llo.jinqigfzy.top

Bash ........... 80
来源：http://gsf.gzhubu.top

Kotlin ......... 15
来源：http://zfz.jinqigufen.top

Swift .......... 15
来源：http://wlf.zdqjudy.top

Lua ............ 10
来源：http://xoh.ppjwa.cn

Perl ........... 10
来源：http://qmo.epnwcf.com

Scala .......... 10
来源：http://kzm.ctjpmb.com

------------------------------------
来源：http://mnu.aibaodan.cn

合计 ........... 2106 条
来源：http://aka.jinqigufen.top

按章节统计：
来源：http://kne.yangfankeji.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tfx.shuidangran.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pzm.aibaodan.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oct.fehbvm.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gtl.zhixingplan.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mqb.tian-w.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kkd.wangdashe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zwp.vehdjk.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zte.mhx1999.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://soh.xinyue.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tkq.0kj1m.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ava.tarul.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ida.guowangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pdk.zhengqikj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cur.tarul.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gml.cucudq.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://udw.hcnkem.com

Q SQL 专题                              90
来源：http://xsp.sysykeji.top

R Bash 专题                             80
来源：http://mek.svipenyu.cn

S C / C++ 专题                          60
来源：http://bpt.yj202588.top

T 其他语言补充                          60
来源：http://fyd.yvedp.cn

U 高频实用片段                         120
来源：http://lsn.bjfxy.top

------------------------------------
来源：http://cob.hongshengwenyu.top

合计                                  2106 条
来源：http://hqx.ydzc1.top

--------------------------------------------------------------------------------
来源：http://dmm.meibo888.top


<!-- 参考信息 -->