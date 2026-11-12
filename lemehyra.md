代发 wailian999

val a = 1;  var b = 2
来源：http://ltr.ctjpmb.com

[T53] Scala：字符串插值
来源：http://vsf.wangshuangyany.cn

s"值: $b"
来源：http://fun.tianlin.xyz

[T54] Scala：集合映射
来源：http://ado.ydzc1.top

List(1, 2, 3).map(_ * 2)
来源：http://zaa.hnqzz.top

[T55] Scala：集合过滤
来源：http://vju.haohaochexian.top

List(1, 2, 3).filter(_ > 1)
来源：http://zbr.xziqi.cn

[T56] Scala：样例类
来源：http://dru.vehdjk.com

case class User(name: String, age: Int)
来源：http://hyy.jlsjyb.cn

[T57] Scala：模式匹配
来源：http://znn.fengsongda.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://avi.wangshuangyany.cn

[T58] Scala：函数定义
来源：http://mgk.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://tqs.gaohongyu789.top

[T59] Scala：循环
来源：http://rfi.52xcode.cn

for (i <- 1 to 10) println(i)
来源：http://vmb.sweek.top

[T60] Scala：折叠
来源：http://jqi.zhengqikj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://unw.tianlin.xyz

================================================================================
来源：http://jww.jyoumei.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bdu.tian-w.cn

================================================================================
来源：http://jsw.cheryme.top

[U01] Py：创建虚拟环境
来源：http://rkv.yanxiufei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ztl.hcnkem.com

[U02] Py：导出 / 安装依赖
来源：http://cjg.cqqwz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://shp.ppjwa.cn

[U03] Py：加载 .env 配置
来源：http://ezc.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ovt.jiagoushi.top

[U04] Py：变量调试打印
来源：http://gjh.vehdjk.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ktq.jianghu66.top

[U05] Py：列表去重且保序
来源：http://gia.smart0.xyz

list(dict.fromkeys(arr))
来源：http://fof.yj20258.top

[U06] Py：合并两个字典
来源：http://ecw.quarkkingdee.top

{**a, **b}
来源：http://bgw.nanxinkj.top

[U07] Py：反转字典键值
来源：http://ijp.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://yvi.tanke756.top

[U08] Py：展平二维列表
来源：http://qjr.vehdjk.com

[y for x in nested for y in x]
来源：http://mmf.jinqigfzy.top

[U09] Py：字典取最大值的键
来源：http://mgr.smart0.xyz

max(d, key=d.get)
来源：http://jon.tian-w.cn

[U10] Py：按值排序字典
来源：http://gtv.yuanzhike.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sek.jqgfzy.top

[U11] Py：生成器表达式
来源：http://rcq.jinghuilouyu.cn

(x * 2 for x in arr)
来源：http://oly.fehbvm.com

[U12] Py：取出现最多的 3 个元素
来源：http://aui.ehwqpu.com

Counter(arr).most_common(3)
来源：http://zss.hywenlv.cn

[U13] Py：固定长度队列
来源：http://ptf.tanke756.top

deque(maxlen=10)
来源：http://ghn.fehbvm.com

[U14] Py：分组收集到列表
来源：http://mhn.chenjidiqi.icu

defaultdict(list)
来源：http://imt.sysykeji.top

[U15] Py：高精度计时
来源：http://jga.nanxuanxn.top

t = time.perf_counter()
来源：http://htj.guowangkeji.top

[U16] Py：命令行参数解析
来源：http://kdt.cashguo.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lho.zycfv.cn

[U17] Py：初始化日志
来源：http://wqv.daria6918.cn

logging.basicConfig(level=logging.INFO)
来源：http://kqr.tanke756.top

[U18] Py：预编译正则
来源：http://gpa.shanyushiyangtech.top

pat = re.compile(r"\d+")
来源：http://ygb.quarkkingdee.top

[U19] Py：正则替换带回调
来源：http://odi.yueranfly.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lyh.52xcode.cn

[U20] Py：缓存函数结果
来源：http://kkf.wangshuangyany.cn

@functools.lru_cache(maxsize=None)
来源：http://aop.jinyuanbaomall.cn

[U21] Py：自定义上下文管理器
来源：http://fjz.zhengqikj.top

@contextlib.contextmanager
来源：http://rhn.9152youxi.cn

[U22] Py：矩阵转置
来源：http://lwy.meibo888.top

list(zip(*m))
来源：http://twu.hongshengwenyu.top

[U23] Py：分块读取大文件
来源：http://cyk.gogol.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fob.fanxiaobao.xyz

[U24] Py：路径操作
来源：http://bhw.tanke756.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fdl.ctjpmb.com

[U25] Py：CSV 按字典读
来源：http://cth.meibo888.top

csv.DictReader(f)
来源：http://ihk.aizwys.cn

[U26] Py：并发下载
来源：http://hua.shuidangran.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bqe.bbcook.cn

[U27] Py：异步 HTTP
来源：http://ahx.yonumen.top

aiohttp.ClientSession() 配合 async with
来源：http://zbe.uphjek.com

[U28] Py：类型别名
来源：http://tvs.smart0.xyz

UserId = int
来源：http://zmc.bjfxy.top

[U29] Py：属性校验
来源：http://qda.yj20258888.top

@property 与 @x.setter 配合
来源：http://vvl.vqdsnc.cn

[U30] Py：数据类
来源：http://umf.ctjpmb.com

@dataclass(slots=True)
来源：http://tzm.sufxvd.cn

[U31] Py：单测
来源：http://jgm.aibaodan.cn

python -m pytest -q
来源：http://vjo.gzhubu.top

[U32] Py：代码格式化
来源：http://nno.smart0.xyz

ruff format . && ruff check --fix .
来源：http://lff.hnxiangtu.top

[U33] Py：打包发布
来源：http://mnh.meibo888.top

python -m build  （依赖 pyproject.toml）
来源：http://ndf.gotoacloud.top

[U34] Py：判断编码
来源：http://wiz.mhx1999.top

chardet.detect(raw)
来源：http://ort.daxiang520.top

[U35] Py：发送邮件
来源：http://kth.nanxinkj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://stu.nanxuanxn.top

[U36] Py：定时任务
来源：http://stu.daria6918.cn

schedule.every(10).minutes.do(job)
来源：http://zja.snrcjt.cn

[U37] Py：读写 Excel
来源：http://vvf.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://sja.xuanzx.com

[U38] Py：获取脚本所在目录
来源：http://ehs.xuanzx.com

Path(__file__).resolve().parent
来源：http://kak.quarkkingdee.top

[U39] Py：判断是否在交互环境
来源：http://nbv.jinyuanbaomall.cn

sys.stdout.isatty()
来源：http://euz.nanxuanxn.top

[U40] Py：打印到标准错误
来源：http://pdv.jqgufenzy.top

print("err", file=sys.stderr)
来源：http://aza.tarul.cn

[U41] PHP：初始化 Composer 项目
来源：http://vbj.tian-w.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bru.hnxiangtu.top

[U42] PHP：PSR-4 自动加载
来源：http://cie.shangyingyoupin.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fey.ehwqpu.com

[U43] PHP：声明命名空间
来源：http://srm.sufxvd.cn

namespace App\Http;
来源：http://evp.daxiang520.top

[U44] PHP：开启严格类型
来源：http://hbz.fanxiaobao.xyz

declare(strict_types=1);
来源：http://inf.zhijiandao.cn

[U45] PHP：类型声明与返回类型
来源：http://ywc.daria6918.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://waf.52xcode.cn

[U46] PHP：可空类型
来源：http://ycf.nanxinkj.top

?string $name = null
来源：http://wal.havefunace.top

[U47] PHP：联合类型
来源：http://izq.hongshengwenyu.top

int|string $id
来源：http://kux.mhx1999.top

[U48] PHP：纯枚举
来源：http://kud.shzxlz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://npy.hammf.cn

[U49] PHP：只读属性
来源：http://ati.vqdsnc.cn

public readonly string $name
来源：http://nfo.haohaochexian.top

[U50] PHP：构造器属性提升
来源：http://bst.birdmap.top

public function __construct(private int $id) {}
来源：http://umz.svipenyu.cn

[U51] PHP：数组解构
来源：http://okt.zdbjq.cn

[$a, $b] = $arr;
来源：http://qgt.bbcook.cn

[U52] PHP：箭头函数
来源：http://krr.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://azm.feifeiyinyue.top

[U53] PHP：空合并运算符
来源：http://dzy.svipenyu.cn

$v = $a ?? $b ?? "default";
来源：http://jsq.hongshengwenyu.top

[U54] PHP：空安全调用
来源：http://zhv.0kj1m.cn

$obj?->method()
来源：http://zzx.birdmap.top

[U55] PHP：match 表达式
来源：http://gfy.jinqigufen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lkg.jyoumei.cn

[U56] PHP：命名参数
来源：http://ugh.ydzc1.top

f(a: 1, b: 2)
来源：http://yzd.zhongyouzk.top

[U57] PHP：字符串插值
来源：http://hnt.birdmap.top

"值: {$a}"
来源：http://szq.gotoacloud.top

[U58] PHP：数组三件套
来源：http://vyf.ybcxt.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qdo.jqgufenzy.top

[U59] PHP：自定义排序
来源：http://aai.ivvv.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://asu.daria6918.cn

[U60] PHP：JSON 编解码
来源：http://ait.zhongyouzk.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://byf.gaohongyu789.top

[U61] PHP：正则
来源：http://zhi.wangshuangyany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sed.jiagoushi.top

[U62] PHP：日期对象
来源：http://bnj.yfazqb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hfz.chenzaomai.com

[U63] PHP：文件读写
来源：http://lqs.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fat.ctjpmb.com

[U64] PHP：目录遍历
来源：http://sjh.yuanzhike.top

glob("dir/*.php");  scandir("dir");
来源：http://xpe.fanxiaobao.xyz

[U65] PHP：会话
来源：http://rmv.yangfankeji.com

session_start();  $_SESSION["uid"] = 1;
来源：http://oww.chenjidiqi.icu

[U66] PHP：设置 Cookie
来源：http://lqh.zdqjudy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mre.aizwys.cn

[U67] PHP：处理文件上传
来源：http://kjd.yongpay.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ihr.feifeiyinyue.top

[U68] PHP：PDO 连接
来源：http://igs.jiagoushi.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hyf.yanxiufei.cn

[U69] PHP：PDO 预处理
来源：http://cfh.shanyushiyangtech.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jua.yj202588.top

[U70] PHP：PDO 事务
来源：http://kkm.shuidangran.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oac.feifeiyinyue.top

[U71] PHP：抛出异常
来源：http://fac.sysykeji.top

throw new RuntimeException("失败", 500);
来源：http://dfb.sjlbkw.cn

[U72] PHP：写错误日志
来源：http://qwi.guowangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://mhq.quarkkingdee.top

[U73] PHP：读取 ini 配置
来源：http://pdz.jlsjyb.cn

parse_ini_file("config.ini", true)
来源：http://vss.xziqi.cn

[U74] PHP：读取环境变量
来源：http://mun.chenlongwang.top

getenv("APP_ENV") ?: "production"
来源：http://jjf.daxiang520.top

[U75] PHP：依赖注入
来源：http://fzx.zdbjq.cn

composer require psr/container
来源：http://kju.fengsongda.top

[U76] PHP：简单路由
来源：http://bxb.shanyushiyangtech.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fse.ydzc1.top

[U77] PHP：模板渲染
来源：http://czz.pycfn.com

composer require twig/twig
来源：http://eyr.epnwcf.com

[U78] PHP：单元测试
来源：http://jgw.316326.xyz

composer require --dev phpunit/phpunit
来源：http://maj.hnqzz.top

[U79] PHP：静态分析
来源：http://rlz.jqgfzy.top

composer require --dev phpstan/phpstan
来源：http://ihh.sjlbkw.cn

[U80] PHP：代码规范修复
来源：http://tyo.yj20258.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hxx.hywenlv.cn

[U81] JS：初始化项目
来源：http://qwm.shangyingyoupin.top

npm init -y;  npm i express
来源：http://hvj.gogol.net.cn

[U82] JS：package.json 脚本
来源：http://ulu.fktsv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xtb.yonumen.top

[U83] JS：ES Module 导入导出
来源：http://clj.ybcxt.top

export const a = 1;  import { a } from "./m.js";
来源：http://fui.ivvv.top

[U84] JS：CommonJS 写法
来源：http://dtj.hysaishi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://czi.yuanzhike.top

[U85] JS：可选链
来源：http://qyl.chenlongwang.top

a?.b?.c
来源：http://pwu.vqdsnc.cn

[U86] JS：空值合并
来源：http://tvl.aizwys.cn

a ?? b
来源：http://xas.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://gvw.hysaishi.cn

const { a = 1, b = 2 } = obj;
来源：http://omp.zdbjq.cn

[U88] JS：对象展开合并
来源：http://mth.guowangkeji.top

{ ...a, ...b }
来源：http://pox.chenzaomai.com

[U89] JS：数组去重
来源：http://lrp.zdbjq.cn

[...new Set(arr)]
来源：http://klx.yvedp.cn

[U90] JS：数字数组排序
来源：http://scg.hfpthk.cn

[...arr].sort((a, b) => a - b)
来源：http://lus.sufxvd.cn

[U91] JS：对象键值遍历
来源：http://jzx.sweek.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lpl.zhoulong.xyz

[U92] JS：深拷贝
来源：http://ett.hesvh.cn

structuredClone(obj)
来源：http://kzh.gzhubu.top

[U93] JS：模板字符串
来源：http://ajo.yj20258888.top

`共 ${n} 条`
来源：http://kbk.cucudq.cn

[U94] JS：箭头函数
来源：http://mrb.52xcode.cn

const double = x => x * 2;
来源：http://fua.shangyingyoupin.top

[U95] JS：Promise 包装
来源：http://pax.aizwys.cn

new Promise((resolve, reject) => {})
来源：http://baj.zdqjudy.top

[U96] JS：async/await 与异常
来源：http://khd.xingfuxueyuan.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kwu.shanyushiyangkeji.top

[U97] JS：并发请求
来源：http://stb.gogol.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kyq.ehwqpu.com

[U98] JS：fetch 带 JSON
来源：http://mjd.xuanzx.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mtg.yanxiufei.cn

[U99] JS：事件监听
来源：http://kyz.bbcook.cn

el.addEventListener("click", e => {})
来源：http://vug.fktsv.cn

[U100] JS：DOM 查询
来源：http://qje.quarkkingdee.top

document.querySelector(".item")
来源：http://kbc.gaohongyu789.top

[U101] JS：classList 操作
来源：http://svb.zycfv.cn

el.classList.toggle("active")
来源：http://hnj.jyoumei.cn

[U102] JS：本地存储
来源：http://stb.hywenlv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wyd.jinqigfzy.top

[U103] JS：定时器
来源：http://aar.shzxlz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://msr.zhongyouzk.top

[U104] JS：防抖
来源：http://ytk.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zwr.9152youxi.cn

[U105] JS：节流
来源：http://fkj.gzhubu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kjt.hongshengwenyu.top

[U106] JS：日期格式化
来源：http://hfw.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qrr.aibaodan.cn

[U107] JS：数字千分位
来源：http://reh.cashguo.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://epm.52xcode.cn

[U108] JS：随机整数
来源：http://sfc.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ath.zhijiandao.cn

[U109] JS：数组分组
来源：http://brx.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://lob.yj20258.top

[U110] JS：数组分块
来源：http://skg.hnqzz.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://orm.shanyushiyangtech.top

[U111] JS：对象转 Map
来源：http://hww.fehbvm.com

new Map(Object.entries(obj))
来源：http://rlt.vehdjk.com

[U112] JS：字符串补位
来源：http://rae.chenlongwang.top

"7".padStart(3, "0")
来源：http://nha.vehdjk.com

[U113] JS：正则替换全部
来源：http://wrd.guannengcc.top

s.replaceAll("a", "b")
来源：http://xzl.chenzaomai.com

[U114] JS：JSON 深比较
来源：http://xqw.jqgufenzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://xzu.sjlbkw.cn

[U115] JS：生成 UUID
来源：http://mbk.nwbrower.top

crypto.randomUUID()
来源：http://qsl.yj20258.top

[U116] JS：类型检查（JSDoc）
来源：http://dkx.dianchejie.cn

/** @param {string} name */ function f(name) {}
来源：http://cbn.dianchejie.cn

[U117] JS：单元测试
来源：http://ufp.ybcxt.top

npm i -D vitest;  npx vitest
来源：http://pdp.chenlongwang.top

[U118] JS：开发服务器
来源：http://rvo.bjfxy.top

npm i -D vite;  npx vite
来源：http://erw.pengpengdd.cyou

[U119] JS：生产构建
来源：http://ehf.dianchejie.cn

npx vite build
来源：http://vrz.pengpengdd.cyou

[U120] JS：读取环境变量（Vite）
来源：http://sni.zhiwuduotai.top

import.meta.env.VITE_API_URL
来源：http://awm.hesvh.cn

================================================================================
来源：http://bmu.havefunace.top

统计汇总
来源：http://zsh.bjfxy.top

================================================================================
来源：http://ijs.cdnleiting.top

按语言统计（条）：
来源：http://agz.meibo888.top

Python ......... 252
来源：http://qqt.tanke756.top

PHP ............ 252
来源：http://hly.hysaishi.cn

JavaScript ..... 252
来源：http://cif.tianlin.xyz

TypeScript ..... 212
来源：http://rrg.feifeiyinyue.top

Java ........... 212
来源：http://fwy.yj20258.top

Go ............. 212
来源：http://ydq.ywan-chungtsiang.top

Ruby ........... 212
来源：http://qla.chenzaomai.com

C# ............. 212
来源：http://xwr.epnwcf.com

C .............. 30
来源：http://cnu.yueranfly.top

C++ ............ 30
来源：http://dch.zdqjudy.top

SQL ............ 90
来源：http://hmx.yanxiufei.cn

Bash ........... 80
来源：http://wzq.hesvh.cn

Kotlin ......... 15
来源：http://qhn.52xcode.cn

Swift .......... 15
来源：http://ypi.shanyushiyangkeji.top

Lua ............ 10
来源：http://ddr.dianchejie.cn

Perl ........... 10
来源：http://ywv.chenjidiqi.icu

Scala .......... 10
来源：http://bhy.hysaishi.cn

------------------------------------
来源：http://myb.xuetiantiany.cn

合计 ........... 2106 条
来源：http://mhf.jinqigfzy.top

按章节统计：
来源：http://flz.wangshuangyany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yyj.zdqjudy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dpb.c1oappe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jfh.jinqigufen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xsn.quarkkingdee.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uma.chenzaomai.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ade.vqdsnc.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bxc.zhiwuduotai.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://crp.jianghu66.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jkh.52xcode.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://afw.sufxvd.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sef.fktsv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zhg.yfazqb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dpb.mhx1999.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sak.zhoulong.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mim.zdbjq.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nxs.ywan-chungtsiang.top


<!-- 参考信息 -->