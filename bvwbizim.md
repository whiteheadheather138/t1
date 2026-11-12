代发 wailian999

val a = 1;  var b = 2
来源：http://bxt.jiagoushi.top

[T53] Scala：字符串插值
来源：http://muw.svipenyu.cn

s"值: $b"
来源：http://xtc.hywenlv.cn

[T54] Scala：集合映射
来源：http://teb.gogol.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://xwk.tianlin.xyz

[T55] Scala：集合过滤
来源：http://iwz.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://lbz.gzhubu.top

[T56] Scala：样例类
来源：http://apq.jiagoushi.top

case class User(name: String, age: Int)
来源：http://bjv.ivvv.top

[T57] Scala：模式匹配
来源：http://aon.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ueh.hongshengwenyu.top

[T58] Scala：函数定义
来源：http://ipw.zhoulong.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://syn.daxiang520.top

[T59] Scala：循环
来源：http://byk.jinqigufen.top

for (i <- 1 to 10) println(i)
来源：http://wmv.hcnkem.com

[T60] Scala：折叠
来源：http://tgz.dianchejie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rkz.zhoulong.xyz

================================================================================
来源：http://woa.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://clo.aibaodan.cn

================================================================================
来源：http://bes.ctjpmb.com

[U01] Py：创建虚拟环境
来源：http://mag.aizwys.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hkw.meibo888.top

[U02] Py：导出 / 安装依赖
来源：http://ubg.snrcjt.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://adv.shangyingyoupin.top

[U03] Py：加载 .env 配置
来源：http://rtw.epnwcf.com

from dotenv import load_dotenv; load_dotenv()
来源：http://jtg.kuanghao11.cn

[U04] Py：变量调试打印
来源：http://bjc.gogol.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bsw.hammf.cn

[U05] Py：列表去重且保序
来源：http://vxd.ivvv.top

list(dict.fromkeys(arr))
来源：http://msq.chenzaomai.com

[U06] Py：合并两个字典
来源：http://bhc.pengpengdd.cyou

{**a, **b}
来源：http://rdz.wangdashe.top

[U07] Py：反转字典键值
来源：http://gjr.haohaochexian.top

{v: k for k, v in d.items()}
来源：http://lyp.jyoumei.cn

[U08] Py：展平二维列表
来源：http://ycv.uphjek.com

[y for x in nested for y in x]
来源：http://zec.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://apr.jinghuilouyu.cn

max(d, key=d.get)
来源：http://rfo.hysaishi.cn

[U10] Py：按值排序字典
来源：http://qxi.pycfn.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nep.tian-w.cn

[U11] Py：生成器表达式
来源：http://vhd.yueranfly.top

(x * 2 for x in arr)
来源：http://ldk.dashuyun.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ckv.cqqwz.cn

Counter(arr).most_common(3)
来源：http://ikz.yueranfly.top

[U13] Py：固定长度队列
来源：http://ujt.sufxvd.cn

deque(maxlen=10)
来源：http://drl.chenlongwang.top

[U14] Py：分组收集到列表
来源：http://nkl.fanxiaobao.xyz

defaultdict(list)
来源：http://yza.xziqi.cn

[U15] Py：高精度计时
来源：http://yfv.hammf.cn

t = time.perf_counter()
来源：http://zku.ctjpmb.com

[U16] Py：命令行参数解析
来源：http://cyx.hongshengwenyu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xov.yvedp.cn

[U17] Py：初始化日志
来源：http://xkc.aizwys.cn

logging.basicConfig(level=logging.INFO)
来源：http://mcy.jyoumei.cn

[U18] Py：预编译正则
来源：http://lkz.gaohongyu789.top

pat = re.compile(r"\d+")
来源：http://qnw.jinqigfzy.top

[U19] Py：正则替换带回调
来源：http://qlu.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kyb.hongshengwenyu.top

[U20] Py：缓存函数结果
来源：http://dgt.jinqigufen.top

@functools.lru_cache(maxsize=None)
来源：http://lmr.cashguo.top

[U21] Py：自定义上下文管理器
来源：http://qgc.iojbl.cn

@contextlib.contextmanager
来源：http://hde.yanxiufei.cn

[U22] Py：矩阵转置
来源：http://gkh.epnwcf.com

list(zip(*m))
来源：http://wvi.shanyushiyangtech.top

[U23] Py：分块读取大文件
来源：http://vof.hywenlv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qqv.cqqwz.cn

[U24] Py：路径操作
来源：http://jpe.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yim.gotoacloud.top

[U25] Py：CSV 按字典读
来源：http://znn.jinghuilouyu.cn

csv.DictReader(f)
来源：http://lzi.zhixingplan.top

[U26] Py：并发下载
来源：http://jmz.meibo888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jbf.sweek.top

[U27] Py：异步 HTTP
来源：http://lus.birdmap.top

aiohttp.ClientSession() 配合 async with
来源：http://lue.jqgufenzy.top

[U28] Py：类型别名
来源：http://ppp.redwolf501.top

UserId = int
来源：http://gmw.yvedp.cn

[U29] Py：属性校验
来源：http://nrr.dianchejie.cn

@property 与 @x.setter 配合
来源：http://fgw.zycfv.cn

[U30] Py：数据类
来源：http://jgq.shzxlz.cn

@dataclass(slots=True)
来源：http://ege.52xcode.cn

[U31] Py：单测
来源：http://qtn.chenjidiqi.icu

python -m pytest -q
来源：http://son.chenzaomai.com

[U32] Py：代码格式化
来源：http://sbe.xinyue.icu

ruff format . && ruff check --fix .
来源：http://yam.cashguo.top

[U33] Py：打包发布
来源：http://hur.pycfn.com

python -m build  （依赖 pyproject.toml）
来源：http://tsr.xziqi.cn

[U34] Py：判断编码
来源：http://mre.nanxuanxn.top

chardet.detect(raw)
来源：http://bih.andypj.xyz

[U35] Py：发送邮件
来源：http://mpr.hnxiangtu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lwp.jinghuilouyu.cn

[U36] Py：定时任务
来源：http://myk.yonumen.top

schedule.every(10).minutes.do(job)
来源：http://qnk.ybcxt.top

[U37] Py：读写 Excel
来源：http://miu.hfpthk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ckr.hfpthk.cn

[U38] Py：获取脚本所在目录
来源：http://eia.jqgufenzy.top

Path(__file__).resolve().parent
来源：http://ecv.smart0.xyz

[U39] Py：判断是否在交互环境
来源：http://oae.hcnkem.com

sys.stdout.isatty()
来源：http://exl.yuxming.cn

[U40] Py：打印到标准错误
来源：http://xvu.tanke756.top

print("err", file=sys.stderr)
来源：http://ehe.pycfn.com

[U41] PHP：初始化 Composer 项目
来源：http://htx.havefunace.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lzg.sufxvd.cn

[U42] PHP：PSR-4 自动加载
来源：http://zoe.wangshuangyany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ujf.jinghuilouyu.cn

[U43] PHP：声明命名空间
来源：http://tvt.birdmap.top

namespace App\Http;
来源：http://pzt.zhijiandao.cn

[U44] PHP：开启严格类型
来源：http://nql.yongpay.top

declare(strict_types=1);
来源：http://lsb.0kj1m.cn

[U45] PHP：类型声明与返回类型
来源：http://xzj.dianchejie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uen.chenlongwang.top

[U46] PHP：可空类型
来源：http://rsv.vehdjk.com

?string $name = null
来源：http://imn.yj20258888.top

[U47] PHP：联合类型
来源：http://rfi.meibo888.top

int|string $id
来源：http://vgc.gogol.net.cn

[U48] PHP：纯枚举
来源：http://mtt.sweek.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yfk.shuidangran.top

[U49] PHP：只读属性
来源：http://gbi.quarkkingdee.top

public readonly string $name
来源：http://tth.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://wfu.gzhubu.top

public function __construct(private int $id) {}
来源：http://lrw.aizwys.cn

[U51] PHP：数组解构
来源：http://pmo.zhoulong.xyz

[$a, $b] = $arr;
来源：http://oov.fktsv.cn

[U52] PHP：箭头函数
来源：http://oxp.wangdashe.top

$double = fn($x) => $x * 2;
来源：http://rcl.hnqzz.top

[U53] PHP：空合并运算符
来源：http://qtx.hysaishi.cn

$v = $a ?? $b ?? "default";
来源：http://rah.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://ljs.haohaochexian.top

$obj?->method()
来源：http://apo.uphjek.com

[U55] PHP：match 表达式
来源：http://xmy.aizwys.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sfr.hcnkem.com

[U56] PHP：命名参数
来源：http://hvn.jqgufenzy.top

f(a: 1, b: 2)
来源：http://ulu.gzhubu.top

[U57] PHP：字符串插值
来源：http://zaj.316326.xyz

"值: {$a}"
来源：http://avj.yueranfly.top

[U58] PHP：数组三件套
来源：http://edw.cdnleiting.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://heb.cdnleiting.top

[U59] PHP：自定义排序
来源：http://vni.jianghu66.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rft.jinyuanbaomall.cn

[U60] PHP：JSON 编解码
来源：http://wak.ywan-chungtsiang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://das.quarkkingdee.top

[U61] PHP：正则
来源：http://fwm.gaohongyu789.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nst.xuanzx.com

[U62] PHP：日期对象
来源：http://lxl.ydzc1.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nkd.fktsv.cn

[U63] PHP：文件读写
来源：http://kxu.wangdashe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qgp.xylfe.cn

[U64] PHP：目录遍历
来源：http://fnx.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://evm.sxryk.cn

[U65] PHP：会话
来源：http://wns.pycfn.com

session_start();  $_SESSION["uid"] = 1;
来源：http://orm.guowangkeji.top

[U66] PHP：设置 Cookie
来源：http://jzl.tarul.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vyw.shanyushiyangtech.top

[U67] PHP：处理文件上传
来源：http://etq.xinyue.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sir.gzhubu.top

[U68] PHP：PDO 连接
来源：http://pmb.xingfuxueyuan.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://atl.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://rur.cheryme.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jri.andypj.xyz

[U70] PHP：PDO 事务
来源：http://wzd.gaohongyu789.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lvf.sxryk.cn

[U71] PHP：抛出异常
来源：http://oea.ydzc1.top

throw new RuntimeException("失败", 500);
来源：http://oxh.guowangkeji.top

[U72] PHP：写错误日志
来源：http://ieh.redwolf501.top

error_log("失败: " . $e->getMessage());
来源：http://xrj.hnqzz.top

[U73] PHP：读取 ini 配置
来源：http://aex.tianlin.xyz

parse_ini_file("config.ini", true)
来源：http://jdx.mhx1999.top

[U74] PHP：读取环境变量
来源：http://aui.tian-w.cn

getenv("APP_ENV") ?: "production"
来源：http://den.zdqjudy.top

[U75] PHP：依赖注入
来源：http://xlp.sufxvd.cn

composer require psr/container
来源：http://jvg.fengsongda.top

[U76] PHP：简单路由
来源：http://liz.iojbl.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xtp.xziqi.cn

[U77] PHP：模板渲染
来源：http://fgf.52xcode.cn

composer require twig/twig
来源：http://gcx.tarul.cn

[U78] PHP：单元测试
来源：http://dld.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://rtj.quarkkingdee.top

[U79] PHP：静态分析
来源：http://dzx.nanxuanxn.top

composer require --dev phpstan/phpstan
来源：http://pkh.gzhubu.top

[U80] PHP：代码规范修复
来源：http://ctb.fanxiaobao.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://jwz.havefunace.top

[U81] JS：初始化项目
来源：http://whv.mhx1999.top

npm init -y;  npm i express
来源：http://fzj.tianlin.xyz

[U82] JS：package.json 脚本
来源：http://qpl.hcnkem.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kmi.nwbrower.top

[U83] JS：ES Module 导入导出
来源：http://stf.andypj.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://pdt.sjlbkw.cn

[U84] JS：CommonJS 写法
来源：http://yst.shanyushiyangtech.top

module.exports = { a };  const { a } = require("./m");
来源：http://tnm.sufxvd.cn

[U85] JS：可选链
来源：http://bug.fzhhl.top

a?.b?.c
来源：http://vtc.fzhhl.top

[U86] JS：空值合并
来源：http://odv.zycfv.cn

a ?? b
来源：http://wrx.zdbjq.cn

[U87] JS：解构默认值
来源：http://ekn.hnqzz.top

const { a = 1, b = 2 } = obj;
来源：http://ofz.chenjidiqi.icu

[U88] JS：对象展开合并
来源：http://bud.havefunace.top

{ ...a, ...b }
来源：http://ozi.ppjwa.cn

[U89] JS：数组去重
来源：http://xcm.xinyue.icu

[...new Set(arr)]
来源：http://kdp.gzhubu.top

[U90] JS：数字数组排序
来源：http://lds.fzhhl.top

[...arr].sort((a, b) => a - b)
来源：http://mrr.fehbvm.com

[U91] JS：对象键值遍历
来源：http://swf.ctjpmb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jwb.nanxuanxn.top

[U92] JS：深拷贝
来源：http://zsz.ywan-chungtsiang.top

structuredClone(obj)
来源：http://pqk.quarkkingdee.top

[U93] JS：模板字符串
来源：http://hvl.yangfankeji.com

`共 ${n} 条`
来源：http://vsm.tarul.cn

[U94] JS：箭头函数
来源：http://vvr.shuidangran.top

const double = x => x * 2;
来源：http://ver.chenlongwang.top

[U95] JS：Promise 包装
来源：http://sxl.ehwqpu.com

new Promise((resolve, reject) => {})
来源：http://pum.xziqi.cn

[U96] JS：async/await 与异常
来源：http://tem.haohaochexian.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iha.daria6918.cn

[U97] JS：并发请求
来源：http://knp.jyoumei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jep.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://xra.cheryme.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gtb.redwolf501.top

[U99] JS：事件监听
来源：http://khc.jinqigufen.top

el.addEventListener("click", e => {})
来源：http://diq.daria6918.cn

[U100] JS：DOM 查询
来源：http://xon.fehbvm.com

document.querySelector(".item")
来源：http://nur.hongshengwenyu.top

[U101] JS：classList 操作
来源：http://roo.yj20258888.top

el.classList.toggle("active")
来源：http://sls.yueranfly.top

[U102] JS：本地存储
来源：http://fam.nanxuanxn.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://sgi.ctjpmb.com

[U103] JS：定时器
来源：http://rmh.chenzaomai.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iyz.svipenyu.cn

[U104] JS：防抖
来源：http://smo.jianghu66.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pfr.birdmap.top

[U105] JS：节流
来源：http://xml.birdmap.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qot.zdqjudy.top

[U106] JS：日期格式化
来源：http://tvk.tanke756.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lgs.shuidangran.top

[U107] JS：数字千分位
来源：http://jfv.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fpf.kuanghao11.cn

[U108] JS：随机整数
来源：http://nrj.uphjek.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tlo.meibo888.top

[U109] JS：数组分组
来源：http://pzs.9152youxi.cn

Object.groupBy(arr, x => x.type)
来源：http://npv.316326.xyz

[U110] JS：数组分块
来源：http://jtf.kuanghao11.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://knr.xziqi.cn

[U111] JS：对象转 Map
来源：http://ioz.uphjek.com

new Map(Object.entries(obj))
来源：http://odt.dianchejie.cn

[U112] JS：字符串补位
来源：http://kxr.zhaomingkeji.xyz

"7".padStart(3, "0")
来源：http://fml.ydzc1.top

[U113] JS：正则替换全部
来源：http://gdj.feifeiyinyue.top

s.replaceAll("a", "b")
来源：http://ogh.sweek.top

[U114] JS：JSON 深比较
来源：http://jqe.cucudq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://thk.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://tkc.gaohongyu789.top

crypto.randomUUID()
来源：http://vyd.kuanghao11.cn

[U116] JS：类型检查（JSDoc）
来源：http://zpd.yvedp.cn

/** @param {string} name */ function f(name) {}
来源：http://egk.dianchejie.cn

[U117] JS：单元测试
来源：http://nbw.tianlin.xyz

npm i -D vitest;  npx vitest
来源：http://lqr.zdbjq.cn

[U118] JS：开发服务器
来源：http://peb.mhx1999.top

npm i -D vite;  npx vite
来源：http://kcb.kuanghao11.cn

[U119] JS：生产构建
来源：http://aoi.hesvh.cn

npx vite build
来源：http://ysw.yonumen.top

[U120] JS：读取环境变量（Vite）
来源：http://lnu.jinqigfzy.top

import.meta.env.VITE_API_URL
来源：http://sqo.pengpengdd.cyou

================================================================================
来源：http://tox.jinqigufen.top

统计汇总
来源：http://zfn.ehwqpu.com

================================================================================
来源：http://hmp.xingfuxueyuan.xyz

按语言统计（条）：
来源：http://eta.jinghuilouyu.cn

Python ......... 252
来源：http://fst.ctjpmb.com

PHP ............ 252
来源：http://mbg.zhiwuduotai.top

JavaScript ..... 252
来源：http://rno.snrcjt.cn

TypeScript ..... 212
来源：http://boy.zhongyouzk.top

Java ........... 212
来源：http://qvl.havefunace.top

Go ............. 212
来源：http://zvz.andypj.xyz

Ruby ........... 212
来源：http://ega.jyoumei.cn

C# ............. 212
来源：http://psh.vqdsnc.cn

C .............. 30
来源：http://xyo.zhaomingkeji.xyz

C++ ............ 30
来源：http://yhs.yonumen.top

SQL ............ 90
来源：http://zmm.fengsongda.top

Bash ........... 80
来源：http://uwr.svipenyu.cn

Kotlin ......... 15
来源：http://sdv.jinqigufen.top

Swift .......... 15
来源：http://xjo.yongpay.top

Lua ............ 10
来源：http://xpc.jqgfzy.top

Perl ........... 10
来源：http://arn.vehdjk.com

Scala .......... 10
来源：http://vtk.hcnkem.com

------------------------------------
来源：http://rvz.iojbl.cn

合计 ........... 2106 条
来源：http://ikf.jlsjyb.cn

按章节统计：
来源：http://clk.birdmap.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nlv.daria6918.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://snr.shuidangran.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ijg.zhongyouzk.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ipk.uphjek.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uqd.yj202588.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fqv.tianlin.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qvu.quarkkingdee.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vxu.ppjwa.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://are.zhaomingkeji.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dwp.bjfxy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yyf.dashuyun.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yuc.ctjpmb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ugc.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://njx.shanyushiyangtech.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://loc.hysaishi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hci.snrcjt.cn


<!-- 参考信息 -->