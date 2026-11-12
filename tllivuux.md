代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://hox.hywenlv.cn

[T55] Scala：集合过滤
来源：http://kqa.havefunace.top

List(1, 2, 3).filter(_ > 1)
来源：http://bbz.hysaishi.cn

[T56] Scala：样例类
来源：http://awf.hnxiangtu.top

case class User(name: String, age: Int)
来源：http://zrn.gogol.net.cn

[T57] Scala：模式匹配
来源：http://jwl.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rea.xuetiantiany.cn

[T58] Scala：函数定义
来源：http://umv.tian-w.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fme.iojbl.cn

[T59] Scala：循环
来源：http://eke.yfazqb.com

for (i <- 1 to 10) println(i)
来源：http://ans.quarkkingdee.top

[T60] Scala：折叠
来源：http://gzc.yuxming.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dyx.tianlin.xyz

================================================================================
来源：http://okn.jinqigufen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sgz.nanxinkj.top

================================================================================
来源：http://kro.yonumen.top

[U01] Py：创建虚拟环境
来源：http://nxk.ehwqpu.com

python -m venv .venv && source .venv/bin/activate
来源：http://emg.sysykeji.top

[U02] Py：导出 / 安装依赖
来源：http://gdr.ivvv.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mcs.cashguo.top

[U03] Py：加载 .env 配置
来源：http://ihd.shangyingyoupin.top

from dotenv import load_dotenv; load_dotenv()
来源：http://nuf.fengsongda.top

[U04] Py：变量调试打印
来源：http://adk.shuidangran.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mfq.yonumen.top

[U05] Py：列表去重且保序
来源：http://ybt.c1oappe.top

list(dict.fromkeys(arr))
来源：http://otw.hongshengwenyu.top

[U06] Py：合并两个字典
来源：http://hud.sweek.top

{**a, **b}
来源：http://nwd.316326.xyz

[U07] Py：反转字典键值
来源：http://ywg.ppjwa.cn

{v: k for k, v in d.items()}
来源：http://sov.hongshengwenyu.top

[U08] Py：展平二维列表
来源：http://oru.epnwcf.com

[y for x in nested for y in x]
来源：http://ndn.jiagoushi.top

[U09] Py：字典取最大值的键
来源：http://drh.52xcode.cn

max(d, key=d.get)
来源：http://ufs.epnwcf.com

[U10] Py：按值排序字典
来源：http://ofm.shanyushiyangtech.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wyn.yangfankeji.com

[U11] Py：生成器表达式
来源：http://zgi.yuanzhike.top

(x * 2 for x in arr)
来源：http://jfz.yuanzhike.top

[U12] Py：取出现最多的 3 个元素
来源：http://wpk.pengpengdd.cyou

Counter(arr).most_common(3)
来源：http://jdw.yanxiufei.cn

[U13] Py：固定长度队列
来源：http://ewt.guannengcc.top

deque(maxlen=10)
来源：http://avs.quarkkingdee.top

[U14] Py：分组收集到列表
来源：http://kgu.jqgufenzy.top

defaultdict(list)
来源：http://hvk.uphjek.com

[U15] Py：高精度计时
来源：http://hqm.hnxiangtu.top

t = time.perf_counter()
来源：http://bha.cashguo.top

[U16] Py：命令行参数解析
来源：http://mrn.bjfxy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pkh.pycfn.com

[U17] Py：初始化日志
来源：http://ays.chenlongwang.top

logging.basicConfig(level=logging.INFO)
来源：http://umj.sysykeji.top

[U18] Py：预编译正则
来源：http://lsk.gogol.net.cn

pat = re.compile(r"\d+")
来源：http://uvd.iojbl.cn

[U19] Py：正则替换带回调
来源：http://tlu.yongpay.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bgx.cheryme.top

[U20] Py：缓存函数结果
来源：http://zqa.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://meb.zhiwuduotai.top

[U21] Py：自定义上下文管理器
来源：http://rta.uphjek.com

@contextlib.contextmanager
来源：http://nod.zhiwuduotai.top

[U22] Py：矩阵转置
来源：http://pjy.tian-w.cn

list(zip(*m))
来源：http://esz.fktsv.cn

[U23] Py：分块读取大文件
来源：http://muv.sweek.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://njn.yuanzhike.top

[U24] Py：路径操作
来源：http://sif.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://idm.cqqwz.cn

[U25] Py：CSV 按字典读
来源：http://vow.sjlbkw.cn

csv.DictReader(f)
来源：http://gua.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://baj.uphjek.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jys.mhx1999.top

[U27] Py：异步 HTTP
来源：http://vth.316326.xyz

aiohttp.ClientSession() 配合 async with
来源：http://sbb.nanxinkj.top

[U28] Py：类型别名
来源：http://wwa.chenlongwang.top

UserId = int
来源：http://hbo.jqgfzy.top

[U29] Py：属性校验
来源：http://ngs.shanyushiyangtech.top

@property 与 @x.setter 配合
来源：http://gyo.jyoumei.cn

[U30] Py：数据类
来源：http://gom.zhixingplan.top

@dataclass(slots=True)
来源：http://dhz.tianlin.xyz

[U31] Py：单测
来源：http://yse.yuxming.cn

python -m pytest -q
来源：http://vsd.smart0.xyz

[U32] Py：代码格式化
来源：http://hcn.xuanzx.com

ruff format . && ruff check --fix .
来源：http://qmk.yfazqb.com

[U33] Py：打包发布
来源：http://jtw.9152youxi.cn

python -m build  （依赖 pyproject.toml）
来源：http://kgn.ydjk.org.cn

[U34] Py：判断编码
来源：http://uzo.feifeiyinyue.top

chardet.detect(raw)
来源：http://lhj.zdqjudy.top

[U35] Py：发送邮件
来源：http://ury.jiagoushi.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cmz.fengsongda.top

[U36] Py：定时任务
来源：http://bvs.pycfn.com

schedule.every(10).minutes.do(job)
来源：http://mzm.fengsongda.top

[U37] Py：读写 Excel
来源：http://nlf.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://apb.hammf.cn

[U38] Py：获取脚本所在目录
来源：http://vsr.hammf.cn

Path(__file__).resolve().parent
来源：http://qny.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://aif.xuanzx.com

sys.stdout.isatty()
来源：http://rut.ivvv.top

[U40] Py：打印到标准错误
来源：http://dxl.c1oappe.top

print("err", file=sys.stderr)
来源：http://wxi.mhx1999.top

[U41] PHP：初始化 Composer 项目
来源：http://dks.xuetiantiany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wcf.yangfankeji.com

[U42] PHP：PSR-4 自动加载
来源：http://pma.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rdy.0kj1m.cn

[U43] PHP：声明命名空间
来源：http://nut.ivvv.top

namespace App\Http;
来源：http://pcr.tianlin.xyz

[U44] PHP：开启严格类型
来源：http://tbl.ppjwa.cn

declare(strict_types=1);
来源：http://gkj.yj20258.top

[U45] PHP：类型声明与返回类型
来源：http://fja.yfazqb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://hxp.hesvh.cn

[U46] PHP：可空类型
来源：http://ttd.yuxming.cn

?string $name = null
来源：http://nqt.nanxinkj.top

[U47] PHP：联合类型
来源：http://pvd.shzxlz.cn

int|string $id
来源：http://opd.jianghu66.top

[U48] PHP：纯枚举
来源：http://gke.shuidangran.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ols.52xcode.cn

[U49] PHP：只读属性
来源：http://yda.zhengqikj.top

public readonly string $name
来源：http://gny.redwolf501.top

[U50] PHP：构造器属性提升
来源：http://pzy.jinghuilouyu.cn

public function __construct(private int $id) {}
来源：http://qoh.tian-w.cn

[U51] PHP：数组解构
来源：http://sxs.zhoulong.xyz

[$a, $b] = $arr;
来源：http://jer.bjfxy.top

[U52] PHP：箭头函数
来源：http://sjj.jlsjyb.cn

$double = fn($x) => $x * 2;
来源：http://njs.chenlongwang.top

[U53] PHP：空合并运算符
来源：http://xwk.yj20258.top

$v = $a ?? $b ?? "default";
来源：http://rib.sxryk.cn

[U54] PHP：空安全调用
来源：http://mrs.cdnleiting.top

$obj?->method()
来源：http://jme.sufxvd.cn

[U55] PHP：match 表达式
来源：http://fgr.zhaomingkeji.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vhj.zycfv.cn

[U56] PHP：命名参数
来源：http://ygs.dashuyun.cn

f(a: 1, b: 2)
来源：http://hjq.yonumen.top

[U57] PHP：字符串插值
来源：http://wbn.mhx1999.top

"值: {$a}"
来源：http://xdg.cashguo.top

[U58] PHP：数组三件套
来源：http://bxn.daria6918.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lhk.hysaishi.cn

[U59] PHP：自定义排序
来源：http://ugg.jinqigufen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mjz.yuxming.cn

[U60] PHP：JSON 编解码
来源：http://wng.daria6918.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jhd.316326.xyz

[U61] PHP：正则
来源：http://zxf.jqgufenzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://boi.daria6918.cn

[U62] PHP：日期对象
来源：http://uay.bjfxy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gee.fzhhl.top

[U63] PHP：文件读写
来源：http://gri.ywan-chungtsiang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rtf.yfazqb.com

[U64] PHP：目录遍历
来源：http://ecl.zdbjq.cn

glob("dir/*.php");  scandir("dir");
来源：http://exf.haohaochexian.top

[U65] PHP：会话
来源：http://pqp.zhongyouzk.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xev.fehbvm.com

[U66] PHP：设置 Cookie
来源：http://hdb.jiagoushi.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eay.wangdashe.top

[U67] PHP：处理文件上传
来源：http://rcu.haohaochexian.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zdr.zhiwuduotai.top

[U68] PHP：PDO 连接
来源：http://tfp.cdnleiting.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kaa.guannengcc.top

[U69] PHP：PDO 预处理
来源：http://qqp.jinqigufen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://twb.cucudq.cn

[U70] PHP：PDO 事务
来源：http://xah.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ucv.meibo888.top

[U71] PHP：抛出异常
来源：http://ovr.guannengcc.top

throw new RuntimeException("失败", 500);
来源：http://dst.guowangkeji.top

[U72] PHP：写错误日志
来源：http://hiz.yj20258888.top

error_log("失败: " . $e->getMessage());
来源：http://cod.gaohongyu789.top

[U73] PHP：读取 ini 配置
来源：http://opo.xuanzx.com

parse_ini_file("config.ini", true)
来源：http://hod.redwolf501.top

[U74] PHP：读取环境变量
来源：http://cda.jinqigfzy.top

getenv("APP_ENV") ?: "production"
来源：http://bat.ivvv.top

[U75] PHP：依赖注入
来源：http://bou.jlsjyb.cn

composer require psr/container
来源：http://raz.yj20258888.top

[U76] PHP：简单路由
来源：http://yxx.ybcxt.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oei.fanxiaobao.xyz

[U77] PHP：模板渲染
来源：http://zxu.daxiang520.top

composer require twig/twig
来源：http://gfh.tanke756.top

[U78] PHP：单元测试
来源：http://tgr.cdnleiting.top

composer require --dev phpunit/phpunit
来源：http://ojm.hywenlv.cn

[U79] PHP：静态分析
来源：http://nnv.zhongyouzk.top

composer require --dev phpstan/phpstan
来源：http://muw.hnxiangtu.top

[U80] PHP：代码规范修复
来源：http://vtf.ehwqpu.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://epw.quarkkingdee.top

[U81] JS：初始化项目
来源：http://vjs.xinyue.icu

npm init -y;  npm i express
来源：http://zzy.ivvv.top

[U82] JS：package.json 脚本
来源：http://xzr.nanxuanxn.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nbv.dianchejie.cn

[U83] JS：ES Module 导入导出
来源：http://wgb.yonumen.top

export const a = 1;  import { a } from "./m.js";
来源：http://kkh.shuidangran.top

[U84] JS：CommonJS 写法
来源：http://jqr.ctjpmb.com

module.exports = { a };  const { a } = require("./m");
来源：http://lbt.sjlbkw.cn

[U85] JS：可选链
来源：http://bwy.zhijiandao.cn

a?.b?.c
来源：http://tqo.jinqigufen.top

[U86] JS：空值合并
来源：http://edw.ywan-chungtsiang.top

a ?? b
来源：http://ozw.uphjek.com

[U87] JS：解构默认值
来源：http://ibq.ybcxt.top

const { a = 1, b = 2 } = obj;
来源：http://zps.bjfxy.top

[U88] JS：对象展开合并
来源：http://lii.jqgfzy.top

{ ...a, ...b }
来源：http://djs.hysaishi.cn

[U89] JS：数组去重
来源：http://pbp.gaohongyu789.top

[...new Set(arr)]
来源：http://hhv.shzxlz.cn

[U90] JS：数字数组排序
来源：http://kxu.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://rtm.smart0.xyz

[U91] JS：对象键值遍历
来源：http://qpa.zhixingplan.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://quo.jinghuilouyu.cn

[U92] JS：深拷贝
来源：http://fwp.sweek.top

structuredClone(obj)
来源：http://fcw.aizwys.cn

[U93] JS：模板字符串
来源：http://iov.cqqwz.cn

`共 ${n} 条`
来源：http://ynx.xuetiantiany.cn

[U94] JS：箭头函数
来源：http://eyx.dashuyun.cn

const double = x => x * 2;
来源：http://lly.jyoumei.cn

[U95] JS：Promise 包装
来源：http://fky.ctjpmb.com

new Promise((resolve, reject) => {})
来源：http://mnp.ydzc1.top

[U96] JS：async/await 与异常
来源：http://lxk.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nqf.dashuyun.cn

[U97] JS：并发请求
来源：http://kml.xylfe.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fmc.cqqwz.cn

[U98] JS：fetch 带 JSON
来源：http://wbm.hesvh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gsv.wangshuangyany.cn

[U99] JS：事件监听
来源：http://dnk.feifeiyinyue.top

el.addEventListener("click", e => {})
来源：http://mxn.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://hgx.yuxming.cn

document.querySelector(".item")
来源：http://nvg.tian-w.cn

[U101] JS：classList 操作
来源：http://brl.fengsongda.top

el.classList.toggle("active")
来源：http://npo.fehbvm.com

[U102] JS：本地存储
来源：http://pmd.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sgm.redwolf501.top

[U103] JS：定时器
来源：http://qrc.ywan-chungtsiang.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ajs.meibo888.top

[U104] JS：防抖
来源：http://hkw.zhiwuduotai.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lrq.hcnkem.com

[U105] JS：节流
来源：http://qvu.xuetiantiany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vss.xylfe.cn

[U106] JS：日期格式化
来源：http://xnp.hesvh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oet.zhixingplan.top

[U107] JS：数字千分位
来源：http://iyi.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uav.hysaishi.cn

[U108] JS：随机整数
来源：http://xlb.zdbjq.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pkk.hysaishi.cn

[U109] JS：数组分组
来源：http://ujq.yuxming.cn

Object.groupBy(arr, x => x.type)
来源：http://lni.hnxiangtu.top

[U110] JS：数组分块
来源：http://qvv.bbcook.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mig.cdnleiting.top

[U111] JS：对象转 Map
来源：http://rbo.wangdashe.top

new Map(Object.entries(obj))
来源：http://rfm.zhaomingkeji.xyz

[U112] JS：字符串补位
来源：http://rwi.chenlongwang.top

"7".padStart(3, "0")
来源：http://xwi.sxryk.cn

[U113] JS：正则替换全部
来源：http://wqu.wangshuangyany.cn

s.replaceAll("a", "b")
来源：http://eqc.shangyingyoupin.top

[U114] JS：JSON 深比较
来源：http://tkm.guannengcc.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yka.xziqi.cn

[U115] JS：生成 UUID
来源：http://hcy.ppjwa.cn

crypto.randomUUID()
来源：http://odv.hcnkem.com

[U116] JS：类型检查（JSDoc）
来源：http://qka.gogol.net.cn

/** @param {string} name */ function f(name) {}
来源：http://biq.yongpay.top

[U117] JS：单元测试
来源：http://cql.hammf.cn

npm i -D vitest;  npx vitest
来源：http://vnd.yj202588.top

[U118] JS：开发服务器
来源：http://eei.cashguo.top

npm i -D vite;  npx vite
来源：http://ldh.jinyuanbaomall.cn

[U119] JS：生产构建
来源：http://cnv.jlsjyb.cn

npx vite build
来源：http://nya.hywenlv.cn

[U120] JS：读取环境变量（Vite）
来源：http://pkj.daria6918.cn

import.meta.env.VITE_API_URL
来源：http://aet.jyoumei.cn

================================================================================
来源：http://jde.jqgufenzy.top

统计汇总
来源：http://knw.jqgufenzy.top

================================================================================
来源：http://iat.haohaochexian.top

按语言统计（条）：
来源：http://rql.zhijiandao.cn

Python ......... 252
来源：http://ewg.zhiwuduotai.top

PHP ............ 252
来源：http://ybn.gotoacloud.top

JavaScript ..... 252
来源：http://mgh.9152youxi.cn

TypeScript ..... 212
来源：http://ckt.cdnleiting.top

Java ........... 212
来源：http://nax.hammf.cn

Go ............. 212
来源：http://ezo.tanke756.top

Ruby ........... 212
来源：http://gtw.xziqi.cn

C# ............. 212
来源：http://eux.chenzaomai.com

C .............. 30
来源：http://jto.yvedp.cn

C++ ............ 30
来源：http://lij.chenzaomai.com

SQL ............ 90
来源：http://eds.tarul.cn

Bash ........... 80
来源：http://ewu.9152youxi.cn

Kotlin ......... 15
来源：http://xmq.hcnkem.com

Swift .......... 15
来源：http://ida.yangfankeji.com

Lua ............ 10
来源：http://coi.ydjk.org.cn

Perl ........... 10
来源：http://bfh.c1oappe.top

Scala .......... 10
来源：http://nzg.chenjidiqi.icu

------------------------------------
来源：http://zqf.uphjek.com

合计 ........... 2106 条
来源：http://jjr.jinyuanbaomall.cn

按章节统计：
来源：http://aal.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ccj.yuxming.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://msl.hnqzz.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gts.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mwt.cheryme.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wxt.ybcxt.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ijx.cqqwz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xlf.yanxiufei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xan.hysaishi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://szt.yueranfly.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dwf.yangfankeji.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vwc.hongshengwenyu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ypg.redwolf501.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jey.andypj.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://aua.jinqigufen.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vos.hnxiangtu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dte.pengpengdd.cyou

Q SQL 专题                              90
来源：http://skc.xuetiantiany.cn

R Bash 专题                             80
来源：http://drp.jiagoushi.top

S C / C++ 专题                          60
来源：http://lup.hesvh.cn

T 其他语言补充                          60
来源：http://cmp.zhongyouzk.top


<!-- 参考信息 -->