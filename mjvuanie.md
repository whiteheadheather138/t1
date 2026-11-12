代发 wailian999

val a = 1;  var b = 2
来源：http://kzg.fehbvm.com

[T53] Scala：字符串插值
来源：http://ljx.bjfxy.top

s"值: $b"
来源：http://bhe.yangfankeji.com

[T54] Scala：集合映射
来源：http://jrk.chenlongwang.top

List(1, 2, 3).map(_ * 2)
来源：http://xui.zhoulong.xyz

[T55] Scala：集合过滤
来源：http://ner.jinyuanbaomall.cn

List(1, 2, 3).filter(_ > 1)
来源：http://abt.yj20258.top

[T56] Scala：样例类
来源：http://rbx.ywan-chungtsiang.top

case class User(name: String, age: Int)
来源：http://pau.9152youxi.cn

[T57] Scala：模式匹配
来源：http://aso.dianchejie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dcy.smart0.xyz

[T58] Scala：函数定义
来源：http://hmo.cucudq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kih.cheryme.top

[T59] Scala：循环
来源：http://aoc.hammf.cn

for (i <- 1 to 10) println(i)
来源：http://rry.0kj1m.cn

[T60] Scala：折叠
来源：http://dfd.fehbvm.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ugr.jqgfzy.top

================================================================================
来源：http://txq.jianghu66.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rxa.cdnleiting.top

================================================================================
来源：http://qns.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://lwy.zhixingplan.top

python -m venv .venv && source .venv/bin/activate
来源：http://xyw.jyoumei.cn

[U02] Py：导出 / 安装依赖
来源：http://qst.zhiwuduotai.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wzr.ybcxt.top

[U03] Py：加载 .env 配置
来源：http://osg.ehwqpu.com

from dotenv import load_dotenv; load_dotenv()
来源：http://idh.yj202588.top

[U04] Py：变量调试打印
来源：http://fox.smart0.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://prq.yuxming.cn

[U05] Py：列表去重且保序
来源：http://txc.aibaodan.cn

list(dict.fromkeys(arr))
来源：http://tmg.vqdsnc.cn

[U06] Py：合并两个字典
来源：http://aue.ctjpmb.com

{**a, **b}
来源：http://gpo.316326.xyz

[U07] Py：反转字典键值
来源：http://hxu.zhijiandao.cn

{v: k for k, v in d.items()}
来源：http://vkv.c1oappe.top

[U08] Py：展平二维列表
来源：http://vdc.nanxinkj.top

[y for x in nested for y in x]
来源：http://ubs.snrcjt.cn

[U09] Py：字典取最大值的键
来源：http://qyn.shanyushiyangtech.top

max(d, key=d.get)
来源：http://pmp.gogol.net.cn

[U10] Py：按值排序字典
来源：http://cld.pycfn.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mfk.zycfv.cn

[U11] Py：生成器表达式
来源：http://vdb.yuxming.cn

(x * 2 for x in arr)
来源：http://sww.shanyushiyangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://tdd.yueranfly.top

Counter(arr).most_common(3)
来源：http://zhr.svipenyu.cn

[U13] Py：固定长度队列
来源：http://kgk.zhijiandao.cn

deque(maxlen=10)
来源：http://ply.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://krm.zhengqikj.top

defaultdict(list)
来源：http://moc.hnqzz.top

[U15] Py：高精度计时
来源：http://qoq.hcnkem.com

t = time.perf_counter()
来源：http://duv.ppjwa.cn

[U16] Py：命令行参数解析
来源：http://scl.wangdashe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pqj.zdbjq.cn

[U17] Py：初始化日志
来源：http://vdq.ivvv.top

logging.basicConfig(level=logging.INFO)
来源：http://okv.fengsongda.top

[U18] Py：预编译正则
来源：http://hzi.ydzc1.top

pat = re.compile(r"\d+")
来源：http://axd.yj20258.top

[U19] Py：正则替换带回调
来源：http://ohe.jyoumei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zqm.cqqwz.cn

[U20] Py：缓存函数结果
来源：http://pmq.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://gvp.xuetiantiany.cn

[U21] Py：自定义上下文管理器
来源：http://qte.meibo888.top

@contextlib.contextmanager
来源：http://civ.vqdsnc.cn

[U22] Py：矩阵转置
来源：http://xtx.yanxiufei.cn

list(zip(*m))
来源：http://qam.sweek.top

[U23] Py：分块读取大文件
来源：http://mwi.jqgfzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cbz.quarkkingdee.top

[U24] Py：路径操作
来源：http://nxn.bjfxy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rqy.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://hit.chenjidiqi.icu

csv.DictReader(f)
来源：http://mbv.jyoumei.cn

[U26] Py：并发下载
来源：http://ddb.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uic.chenlongwang.top

[U27] Py：异步 HTTP
来源：http://vpo.nanxinkj.top

aiohttp.ClientSession() 配合 async with
来源：http://hbh.cdnleiting.top

[U28] Py：类型别名
来源：http://sth.jinyuanbaomall.cn

UserId = int
来源：http://oji.hcnkem.com

[U29] Py：属性校验
来源：http://uqp.gaohongyu789.top

@property 与 @x.setter 配合
来源：http://uoi.tianlin.xyz

[U30] Py：数据类
来源：http://tgo.jlsjyb.cn

@dataclass(slots=True)
来源：http://gzg.jinyuanbaomall.cn

[U31] Py：单测
来源：http://enz.snrcjt.cn

python -m pytest -q
来源：http://kqr.jinqigfzy.top

[U32] Py：代码格式化
来源：http://aaj.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://vzs.gaohongyu789.top

[U33] Py：打包发布
来源：http://ylt.birdmap.top

python -m build  （依赖 pyproject.toml）
来源：http://bdk.9152youxi.cn

[U34] Py：判断编码
来源：http://mzu.hysaishi.cn

chardet.detect(raw)
来源：http://iri.cucudq.cn

[U35] Py：发送邮件
来源：http://hps.vqdsnc.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://aii.andypj.xyz

[U36] Py：定时任务
来源：http://yoy.dianchejie.cn

schedule.every(10).minutes.do(job)
来源：http://idx.sufxvd.cn

[U37] Py：读写 Excel
来源：http://vip.xingfuxueyuan.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://euz.sufxvd.cn

[U38] Py：获取脚本所在目录
来源：http://cxd.hcnkem.com

Path(__file__).resolve().parent
来源：http://pkq.jinyuanbaomall.cn

[U39] Py：判断是否在交互环境
来源：http://esf.shanyushiyangtech.top

sys.stdout.isatty()
来源：http://tdg.ydzc1.top

[U40] Py：打印到标准错误
来源：http://isk.c1oappe.top

print("err", file=sys.stderr)
来源：http://sco.9152youxi.cn

[U41] PHP：初始化 Composer 项目
来源：http://dvk.havefunace.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zoo.meibo888.top

[U42] PHP：PSR-4 自动加载
来源：http://zxn.sxryk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dro.vehdjk.com

[U43] PHP：声明命名空间
来源：http://eox.fengsongda.top

namespace App\Http;
来源：http://dvt.andypj.xyz

[U44] PHP：开启严格类型
来源：http://ynz.yj20258888.top

declare(strict_types=1);
来源：http://dvd.sufxvd.cn

[U45] PHP：类型声明与返回类型
来源：http://vbu.sjlbkw.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lso.jiagoushi.top

[U46] PHP：可空类型
来源：http://bqy.ppjwa.cn

?string $name = null
来源：http://bvr.iojbl.cn

[U47] PHP：联合类型
来源：http://ysc.yuxming.cn

int|string $id
来源：http://vph.yj202588.top

[U48] PHP：纯枚举
来源：http://pmr.vehdjk.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jno.jiagoushi.top

[U49] PHP：只读属性
来源：http://emg.hfpthk.cn

public readonly string $name
来源：http://lbf.chenjidiqi.icu

[U50] PHP：构造器属性提升
来源：http://fzp.gzhubu.top

public function __construct(private int $id) {}
来源：http://wpy.daxiang520.top

[U51] PHP：数组解构
来源：http://tbr.jianghu66.top

[$a, $b] = $arr;
来源：http://pfq.fktsv.cn

[U52] PHP：箭头函数
来源：http://fcw.xingfuxueyuan.xyz

$double = fn($x) => $x * 2;
来源：http://lnw.ehwqpu.com

[U53] PHP：空合并运算符
来源：http://owc.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://xnt.redwolf501.top

[U54] PHP：空安全调用
来源：http://woj.hnqzz.top

$obj?->method()
来源：http://edx.yj20258888.top

[U55] PHP：match 表达式
来源：http://cku.nanxuanxn.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sbn.ydjk.org.cn

[U56] PHP：命名参数
来源：http://mtp.zhixingplan.top

f(a: 1, b: 2)
来源：http://upk.pycfn.com

[U57] PHP：字符串插值
来源：http://hlj.chenlongwang.top

"值: {$a}"
来源：http://xmp.daria6918.cn

[U58] PHP：数组三件套
来源：http://zcl.yj20258888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bfa.ywan-chungtsiang.top

[U59] PHP：自定义排序
来源：http://hnl.vehdjk.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nve.shanyushiyangtech.top

[U60] PHP：JSON 编解码
来源：http://wgt.nwbrower.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gwh.sjlbkw.cn

[U61] PHP：正则
来源：http://uus.hesvh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mwg.ppjwa.cn

[U62] PHP：日期对象
来源：http://quf.pengpengdd.cyou

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zch.meibo888.top

[U63] PHP：文件读写
来源：http://rhn.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jlb.pycfn.com

[U64] PHP：目录遍历
来源：http://khs.hnxiangtu.top

glob("dir/*.php");  scandir("dir");
来源：http://hzs.zhijiandao.cn

[U65] PHP：会话
来源：http://omp.hysaishi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://huk.smart0.xyz

[U66] PHP：设置 Cookie
来源：http://nzh.zhoulong.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xwv.xylfe.cn

[U67] PHP：处理文件上传
来源：http://dlm.xziqi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://saq.aizwys.cn

[U68] PHP：PDO 连接
来源：http://bds.sufxvd.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://aoc.jinghuilouyu.cn

[U69] PHP：PDO 预处理
来源：http://ssv.andypj.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xio.chenlongwang.top

[U70] PHP：PDO 事务
来源：http://btt.zhijiandao.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kdx.yuxming.cn

[U71] PHP：抛出异常
来源：http://rqq.dianchejie.cn

throw new RuntimeException("失败", 500);
来源：http://suj.zhiwuduotai.top

[U72] PHP：写错误日志
来源：http://ntj.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://mhv.bjfxy.top

[U73] PHP：读取 ini 配置
来源：http://vgh.jianghu66.top

parse_ini_file("config.ini", true)
来源：http://lcj.jinqigfzy.top

[U74] PHP：读取环境变量
来源：http://zpg.feifeiyinyue.top

getenv("APP_ENV") ?: "production"
来源：http://yhs.mhx1999.top

[U75] PHP：依赖注入
来源：http://fsl.gaohongyu789.top

composer require psr/container
来源：http://dpi.52xcode.cn

[U76] PHP：简单路由
来源：http://hxi.nwbrower.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kpg.hammf.cn

[U77] PHP：模板渲染
来源：http://ckq.uphjek.com

composer require twig/twig
来源：http://fdb.zhoulong.xyz

[U78] PHP：单元测试
来源：http://ztm.zycfv.cn

composer require --dev phpunit/phpunit
来源：http://nwg.shanyushiyangkeji.top

[U79] PHP：静态分析
来源：http://ebs.shuidangran.top

composer require --dev phpstan/phpstan
来源：http://xjv.yfazqb.com

[U80] PHP：代码规范修复
来源：http://zbx.sxryk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://llu.shanyushiyangkeji.top

[U81] JS：初始化项目
来源：http://bjw.gaohongyu789.top

npm init -y;  npm i express
来源：http://qad.shzxlz.cn

[U82] JS：package.json 脚本
来源：http://hmy.yonumen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kov.tianlin.xyz

[U83] JS：ES Module 导入导出
来源：http://lrj.dianchejie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kmd.kuanghao11.cn

[U84] JS：CommonJS 写法
来源：http://kka.cqqwz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uxw.ctjpmb.com

[U85] JS：可选链
来源：http://ykb.wangshuangyany.cn

a?.b?.c
来源：http://ajj.yuxming.cn

[U86] JS：空值合并
来源：http://jpg.hongshengwenyu.top

a ?? b
来源：http://pzb.cashguo.top

[U87] JS：解构默认值
来源：http://pvq.meibo888.top

const { a = 1, b = 2 } = obj;
来源：http://vcx.hnxiangtu.top

[U88] JS：对象展开合并
来源：http://wxe.bjfxy.top

{ ...a, ...b }
来源：http://zjr.chenlongwang.top

[U89] JS：数组去重
来源：http://puv.mhx1999.top

[...new Set(arr)]
来源：http://mba.yuxming.cn

[U90] JS：数字数组排序
来源：http://cow.guannengcc.top

[...arr].sort((a, b) => a - b)
来源：http://for.yonumen.top

[U91] JS：对象键值遍历
来源：http://pxc.ybcxt.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ayr.guowangkeji.top

[U92] JS：深拷贝
来源：http://jmw.tianlin.xyz

structuredClone(obj)
来源：http://biy.nwbrower.top

[U93] JS：模板字符串
来源：http://zhh.xuanzx.com

`共 ${n} 条`
来源：http://zfg.aizwys.cn

[U94] JS：箭头函数
来源：http://nzm.sysykeji.top

const double = x => x * 2;
来源：http://jdq.jqgfzy.top

[U95] JS：Promise 包装
来源：http://csv.cashguo.top

new Promise((resolve, reject) => {})
来源：http://ats.daria6918.cn

[U96] JS：async/await 与异常
来源：http://nmn.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gly.vqdsnc.cn

[U97] JS：并发请求
来源：http://kdc.zhongyouzk.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://shu.gotoacloud.top

[U98] JS：fetch 带 JSON
来源：http://sck.chenlongwang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yfh.gotoacloud.top

[U99] JS：事件监听
来源：http://zgf.chenlongwang.top

el.addEventListener("click", e => {})
来源：http://wft.aizwys.cn

[U100] JS：DOM 查询
来源：http://wyw.hnxiangtu.top

document.querySelector(".item")
来源：http://lhg.ctjpmb.com

[U101] JS：classList 操作
来源：http://bqw.hongshengwenyu.top

el.classList.toggle("active")
来源：http://kku.quarkkingdee.top

[U102] JS：本地存储
来源：http://qxp.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ugz.hesvh.cn

[U103] JS：定时器
来源：http://thh.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://shi.zhengqikj.top

[U104] JS：防抖
来源：http://qgg.shuidangran.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mle.haohaochexian.top

[U105] JS：节流
来源：http://ywp.vehdjk.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://viy.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://umh.chenzaomai.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kop.hfpthk.cn

[U107] JS：数字千分位
来源：http://zkd.snrcjt.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uiw.zhixingplan.top

[U108] JS：随机整数
来源：http://wwl.ywan-chungtsiang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dzq.chenzaomai.com

[U109] JS：数组分组
来源：http://jez.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://thp.0kj1m.cn

[U110] JS：数组分块
来源：http://qbw.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rmc.cqqwz.cn

[U111] JS：对象转 Map
来源：http://cxi.hesvh.cn

new Map(Object.entries(obj))
来源：http://gpr.fehbvm.com

[U112] JS：字符串补位
来源：http://ydd.xuanzx.com

"7".padStart(3, "0")
来源：http://gzi.smart0.xyz

[U113] JS：正则替换全部
来源：http://mja.jinghuilouyu.cn

s.replaceAll("a", "b")
来源：http://ify.cucudq.cn

[U114] JS：JSON 深比较
来源：http://exv.hywenlv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fmh.hywenlv.cn

[U115] JS：生成 UUID
来源：http://hhi.gzhubu.top

crypto.randomUUID()
来源：http://ppz.yuanzhike.top

[U116] JS：类型检查（JSDoc）
来源：http://bsu.daria6918.cn

/** @param {string} name */ function f(name) {}
来源：http://wdo.cdnleiting.top

[U117] JS：单元测试
来源：http://ldd.xziqi.cn

npm i -D vitest;  npx vitest
来源：http://bla.bjfxy.top

[U118] JS：开发服务器
来源：http://fjs.yj202588.top

npm i -D vite;  npx vite
来源：http://vbp.ydzc1.top

[U119] JS：生产构建
来源：http://ile.9152youxi.cn

npx vite build
来源：http://rqf.hywenlv.cn

[U120] JS：读取环境变量（Vite）
来源：http://cdo.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://yre.zhaomingkeji.xyz

================================================================================
来源：http://rcv.ybcxt.top

统计汇总
来源：http://uyo.yonumen.top

================================================================================
来源：http://chj.pengpengdd.cyou

按语言统计（条）：
来源：http://dba.epnwcf.com

Python ......... 252
来源：http://rwy.kuanghao11.cn

PHP ............ 252
来源：http://xte.zhoulong.xyz

JavaScript ..... 252
来源：http://jbd.yj20258.top

TypeScript ..... 212
来源：http://kzk.zhaomingkeji.xyz

Java ........... 212
来源：http://pyh.cqqwz.cn

Go ............. 212
来源：http://kpa.zhaomingkeji.xyz

Ruby ........... 212
来源：http://yiz.jiagoushi.top

C# ............. 212
来源：http://wgc.shuidangran.top

C .............. 30
来源：http://fiq.yuxming.cn

C++ ............ 30
来源：http://suw.jianghu66.top

SQL ............ 90
来源：http://qyt.meibo888.top

Bash ........... 80
来源：http://qpj.mhx1999.top

Kotlin ......... 15
来源：http://acs.yangfankeji.com

Swift .......... 15
来源：http://soh.aizwys.cn

Lua ............ 10
来源：http://box.aibaodan.cn

Perl ........... 10
来源：http://bcc.redwolf501.top

Scala .......... 10
来源：http://weg.kuanghao11.cn

------------------------------------
来源：http://bwc.fktsv.cn

合计 ........... 2106 条
来源：http://jkg.yj202588.top

按章节统计：
来源：http://klf.ctjpmb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qou.ctjpmb.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ebh.hesvh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://puc.sjlbkw.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lfa.jlsjyb.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fwr.hcnkem.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lal.daxiang520.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iqm.zhengqikj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xof.zhongyouzk.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lbk.yangfankeji.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yvn.vehdjk.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tts.0kj1m.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wai.smart0.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gjf.ywan-chungtsiang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ngn.jqgfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wvc.yanxiufei.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dpz.sweek.top


<!-- 参考信息 -->