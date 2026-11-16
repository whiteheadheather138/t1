代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://tsd.aibaodan.cn

[T59] Scala：循环
来源：http://fup.ydzc1.top

for (i <- 1 to 10) println(i)
来源：http://ohv.chenzaomai.com

[T60] Scala：折叠
来源：http://pfi.xziqi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vea.gzhubu.top

================================================================================
来源：http://qsf.hysaishi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nbc.yangfankeji.com

================================================================================
来源：http://ldq.vqdsnc.cn

[U01] Py：创建虚拟环境
来源：http://tpx.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://zvf.zhiwuduotai.top

[U02] Py：导出 / 安装依赖
来源：http://okw.zhixingplan.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zux.zhiwuduotai.top

[U03] Py：加载 .env 配置
来源：http://lrk.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ddx.fzhhl.top

[U04] Py：变量调试打印
来源：http://age.yfazqb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pav.ivvv.top

[U05] Py：列表去重且保序
来源：http://leb.316326.xyz

list(dict.fromkeys(arr))
来源：http://ths.fktsv.cn

[U06] Py：合并两个字典
来源：http://zab.shanyushiyangkeji.top

{**a, **b}
来源：http://vma.jinqigufen.top

[U07] Py：反转字典键值
来源：http://pcn.havefunace.top

{v: k for k, v in d.items()}
来源：http://jhz.yj20258888.top

[U08] Py：展平二维列表
来源：http://ekc.zdbjq.cn

[y for x in nested for y in x]
来源：http://poh.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://ozo.andypj.xyz

max(d, key=d.get)
来源：http://kle.pycfn.com

[U10] Py：按值排序字典
来源：http://hdj.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pai.cdnleiting.top

[U11] Py：生成器表达式
来源：http://ijt.gaohongyu789.top

(x * 2 for x in arr)
来源：http://kyf.smart0.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://uta.ppjwa.cn

Counter(arr).most_common(3)
来源：http://ahe.dashuyun.cn

[U13] Py：固定长度队列
来源：http://uep.zhaomingkeji.xyz

deque(maxlen=10)
来源：http://hje.gogol.net.cn

[U14] Py：分组收集到列表
来源：http://uqp.yueranfly.top

defaultdict(list)
来源：http://qrm.kuanghao11.cn

[U15] Py：高精度计时
来源：http://qmc.shanyushiyangtech.top

t = time.perf_counter()
来源：http://iwi.fengsongda.top

[U16] Py：命令行参数解析
来源：http://tnq.sjlbkw.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fzk.ywan-chungtsiang.top

[U17] Py：初始化日志
来源：http://dhu.gaohongyu789.top

logging.basicConfig(level=logging.INFO)
来源：http://zjj.hywenlv.cn

[U18] Py：预编译正则
来源：http://mqo.uphjek.com

pat = re.compile(r"\d+")
来源：http://kab.mhx1999.top

[U19] Py：正则替换带回调
来源：http://dsn.sjlbkw.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jll.ivvv.top

[U20] Py：缓存函数结果
来源：http://sdf.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://upt.cheryme.top

[U21] Py：自定义上下文管理器
来源：http://ghr.0kj1m.cn

@contextlib.contextmanager
来源：http://zss.fehbvm.com

[U22] Py：矩阵转置
来源：http://azr.ydzc1.top

list(zip(*m))
来源：http://mxs.chenlongwang.top

[U23] Py：分块读取大文件
来源：http://hnb.snrcjt.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ajo.zhiwuduotai.top

[U24] Py：路径操作
来源：http://uqm.hongshengwenyu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zpx.ydzc1.top

[U25] Py：CSV 按字典读
来源：http://let.yj202588.top

csv.DictReader(f)
来源：http://amw.tian-w.cn

[U26] Py：并发下载
来源：http://vwe.tarul.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qzf.jianghu66.top

[U27] Py：异步 HTTP
来源：http://nko.fanxiaobao.xyz

aiohttp.ClientSession() 配合 async with
来源：http://idn.jinqigfzy.top

[U28] Py：类型别名
来源：http://whj.cheryme.top

UserId = int
来源：http://jck.guowangkeji.top

[U29] Py：属性校验
来源：http://ury.tarul.cn

@property 与 @x.setter 配合
来源：http://wxw.yuanzhike.top

[U30] Py：数据类
来源：http://zzo.nanxinkj.top

@dataclass(slots=True)
来源：http://fyg.xuanzx.com

[U31] Py：单测
来源：http://vjk.yvedp.cn

python -m pytest -q
来源：http://nzh.fengsongda.top

[U32] Py：代码格式化
来源：http://tct.redwolf501.top

ruff format . && ruff check --fix .
来源：http://atg.yj202588.top

[U33] Py：打包发布
来源：http://xfr.fktsv.cn

python -m build  （依赖 pyproject.toml）
来源：http://kjq.guowangkeji.top

[U34] Py：判断编码
来源：http://rtg.fengsongda.top

chardet.detect(raw)
来源：http://enj.svipenyu.cn

[U35] Py：发送邮件
来源：http://goq.yuxming.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rpw.cheryme.top

[U36] Py：定时任务
来源：http://rua.ywan-chungtsiang.top

schedule.every(10).minutes.do(job)
来源：http://tpv.ydjk.org.cn

[U37] Py：读写 Excel
来源：http://ttx.chenlongwang.top

pandas.read_excel / DataFrame.to_excel
来源：http://stv.zdqjudy.top

[U38] Py：获取脚本所在目录
来源：http://wry.jianghu66.top

Path(__file__).resolve().parent
来源：http://srz.yanxiufei.cn

[U39] Py：判断是否在交互环境
来源：http://vue.yongpay.top

sys.stdout.isatty()
来源：http://hwk.chenjidiqi.icu

[U40] Py：打印到标准错误
来源：http://huz.cdnleiting.top

print("err", file=sys.stderr)
来源：http://mwz.hysaishi.cn

[U41] PHP：初始化 Composer 项目
来源：http://ybv.zdbjq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sqy.redwolf501.top

[U42] PHP：PSR-4 自动加载
来源：http://wxi.epnwcf.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qxt.yfazqb.com

[U43] PHP：声明命名空间
来源：http://kai.jianghu66.top

namespace App\Http;
来源：http://htl.nwbrower.top

[U44] PHP：开启严格类型
来源：http://hrm.shangyingyoupin.top

declare(strict_types=1);
来源：http://okb.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://vww.wangshuangyany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://egk.chenlongwang.top

[U46] PHP：可空类型
来源：http://uhh.hywenlv.cn

?string $name = null
来源：http://ngc.yj20258888.top

[U47] PHP：联合类型
来源：http://hox.quarkkingdee.top

int|string $id
来源：http://mvg.vqdsnc.cn

[U48] PHP：纯枚举
来源：http://vzd.pengpengdd.cyou

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jqo.yueranfly.top

[U49] PHP：只读属性
来源：http://fjf.haohaochexian.top

public readonly string $name
来源：http://xua.shanyushiyangkeji.top

[U50] PHP：构造器属性提升
来源：http://cdc.epnwcf.com

public function __construct(private int $id) {}
来源：http://jhp.yongpay.top

[U51] PHP：数组解构
来源：http://jqi.vqdsnc.cn

[$a, $b] = $arr;
来源：http://qvy.ybcxt.top

[U52] PHP：箭头函数
来源：http://ehy.mhx1999.top

$double = fn($x) => $x * 2;
来源：http://dvc.hywenlv.cn

[U53] PHP：空合并运算符
来源：http://wno.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://vkg.bbcook.cn

[U54] PHP：空安全调用
来源：http://eiw.xingfuxueyuan.xyz

$obj?->method()
来源：http://egy.ppjwa.cn

[U55] PHP：match 表达式
来源：http://kul.xuanzx.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://opv.hammf.cn

[U56] PHP：命名参数
来源：http://gem.shanyushiyangtech.top

f(a: 1, b: 2)
来源：http://ajy.chenlongwang.top

[U57] PHP：字符串插值
来源：http://ebq.yj20258888.top

"值: {$a}"
来源：http://sod.snrcjt.cn

[U58] PHP：数组三件套
来源：http://mgp.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mku.xylfe.cn

[U59] PHP：自定义排序
来源：http://qug.gaohongyu789.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qjt.ehwqpu.com

[U60] PHP：JSON 编解码
来源：http://xrb.ivvv.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iin.pengpengdd.cyou

[U61] PHP：正则
来源：http://tfd.jinyuanbaomall.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dpg.guowangkeji.top

[U62] PHP：日期对象
来源：http://hwf.yvedp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://shl.ivvv.top

[U63] PHP：文件读写
来源：http://typ.guowangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jwn.yvedp.cn

[U64] PHP：目录遍历
来源：http://kjk.zdqjudy.top

glob("dir/*.php");  scandir("dir");
来源：http://pqr.quarkkingdee.top

[U65] PHP：会话
来源：http://lrw.pycfn.com

session_start();  $_SESSION["uid"] = 1;
来源：http://qfa.ydzc1.top

[U66] PHP：设置 Cookie
来源：http://eyj.feifeiyinyue.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yzm.ybcxt.top

[U67] PHP：处理文件上传
来源：http://nxr.xinyue.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kgl.redwolf501.top

[U68] PHP：PDO 连接
来源：http://ydk.chenjidiqi.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fsf.ydjk.org.cn

[U69] PHP：PDO 预处理
来源：http://lrm.havefunace.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gch.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://rgv.zdqjudy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://iqq.yonumen.top

[U71] PHP：抛出异常
来源：http://efb.cdnleiting.top

throw new RuntimeException("失败", 500);
来源：http://owb.sjlbkw.cn

[U72] PHP：写错误日志
来源：http://yoi.shanyushiyangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://wag.316326.xyz

[U73] PHP：读取 ini 配置
来源：http://ojc.cashguo.top

parse_ini_file("config.ini", true)
来源：http://xyz.hcnkem.com

[U74] PHP：读取环境变量
来源：http://xik.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://efw.tianlin.xyz

[U75] PHP：依赖注入
来源：http://wqi.sxryk.cn

composer require psr/container
来源：http://nvd.zhongyouzk.top

[U76] PHP：简单路由
来源：http://vhe.yuanzhike.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://riu.fehbvm.com

[U77] PHP：模板渲染
来源：http://etr.zhoulong.xyz

composer require twig/twig
来源：http://brl.fzhhl.top

[U78] PHP：单元测试
来源：http://kwt.xziqi.cn

composer require --dev phpunit/phpunit
来源：http://dag.iojbl.cn

[U79] PHP：静态分析
来源：http://wfy.ehwqpu.com

composer require --dev phpstan/phpstan
来源：http://ldw.yueranfly.top

[U80] PHP：代码规范修复
来源：http://kou.fengsongda.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://cxs.cqqwz.cn

[U81] JS：初始化项目
来源：http://jli.shanyushiyangtech.top

npm init -y;  npm i express
来源：http://grh.hammf.cn

[U82] JS：package.json 脚本
来源：http://zir.hammf.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lal.tianlin.xyz

[U83] JS：ES Module 导入导出
来源：http://uyp.dashuyun.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ios.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://jcn.yfazqb.com

module.exports = { a };  const { a } = require("./m");
来源：http://yki.hongshengwenyu.top

[U85] JS：可选链
来源：http://zug.cqqwz.cn

a?.b?.c
来源：http://qsb.yfazqb.com

[U86] JS：空值合并
来源：http://owb.ivvv.top

a ?? b
来源：http://zep.shzxlz.cn

[U87] JS：解构默认值
来源：http://dxh.daria6918.cn

const { a = 1, b = 2 } = obj;
来源：http://owa.fzhhl.top

[U88] JS：对象展开合并
来源：http://prw.yangfankeji.com

{ ...a, ...b }
来源：http://ttd.yvedp.cn

[U89] JS：数组去重
来源：http://pkr.yueranfly.top

[...new Set(arr)]
来源：http://wqt.jyoumei.cn

[U90] JS：数字数组排序
来源：http://ueo.xinyue.icu

[...arr].sort((a, b) => a - b)
来源：http://qqi.dianchejie.cn

[U91] JS：对象键值遍历
来源：http://ote.ivvv.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kmm.chenzaomai.com

[U92] JS：深拷贝
来源：http://tpt.52xcode.cn

structuredClone(obj)
来源：http://qps.uphjek.com

[U93] JS：模板字符串
来源：http://cxs.hongshengwenyu.top

`共 ${n} 条`
来源：http://kph.cucudq.cn

[U94] JS：箭头函数
来源：http://qtm.gzhubu.top

const double = x => x * 2;
来源：http://raz.yvedp.cn

[U95] JS：Promise 包装
来源：http://dqi.yj20258.top

new Promise((resolve, reject) => {})
来源：http://znd.fzhhl.top

[U96] JS：async/await 与异常
来源：http://ota.snrcjt.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yhs.yuanzhike.top

[U97] JS：并发请求
来源：http://yqk.yongpay.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hkw.hfpthk.cn

[U98] JS：fetch 带 JSON
来源：http://wwy.cqqwz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lov.cdnleiting.top

[U99] JS：事件监听
来源：http://rgk.zhoulong.xyz

el.addEventListener("click", e => {})
来源：http://gug.cdnleiting.top

[U100] JS：DOM 查询
来源：http://gxp.bbcook.cn

document.querySelector(".item")
来源：http://dpo.andypj.xyz

[U101] JS：classList 操作
来源：http://ybl.yuanzhike.top

el.classList.toggle("active")
来源：http://qzc.fengsongda.top

[U102] JS：本地存储
来源：http://xvi.shangyingyoupin.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ugb.yonumen.top

[U103] JS：定时器
来源：http://pzt.hammf.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://usv.ybcxt.top

[U104] JS：防抖
来源：http://zam.zhaomingkeji.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qam.vqdsnc.cn

[U105] JS：节流
来源：http://pne.jinqigfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://trl.yanxiufei.cn

[U106] JS：日期格式化
来源：http://sox.yongpay.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ksr.cqqwz.cn

[U107] JS：数字千分位
来源：http://cmk.aizwys.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mpi.52xcode.cn

[U108] JS：随机整数
来源：http://bld.smart0.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://niz.sufxvd.cn

[U109] JS：数组分组
来源：http://onu.pycfn.com

Object.groupBy(arr, x => x.type)
来源：http://nfq.hywenlv.cn

[U110] JS：数组分块
来源：http://gbd.ydzc1.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://axo.jianghu66.top

[U111] JS：对象转 Map
来源：http://sva.epnwcf.com

new Map(Object.entries(obj))
来源：http://qkj.sjlbkw.cn

[U112] JS：字符串补位
来源：http://xaz.cdnleiting.top

"7".padStart(3, "0")
来源：http://ujy.jlsjyb.cn

[U113] JS：正则替换全部
来源：http://rzz.yj20258.top

s.replaceAll("a", "b")
来源：http://fxf.nwbrower.top

[U114] JS：JSON 深比较
来源：http://gwx.hnxiangtu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://eir.yongpay.top

[U115] JS：生成 UUID
来源：http://vvy.birdmap.top

crypto.randomUUID()
来源：http://byf.aibaodan.cn

[U116] JS：类型检查（JSDoc）
来源：http://rxu.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://byq.cucudq.cn

[U117] JS：单元测试
来源：http://akx.nanxuanxn.top

npm i -D vitest;  npx vitest
来源：http://vmx.vqdsnc.cn

[U118] JS：开发服务器
来源：http://byx.jqgufenzy.top

npm i -D vite;  npx vite
来源：http://tgc.sxryk.cn

[U119] JS：生产构建
来源：http://lui.shanyushiyangtech.top

npx vite build
来源：http://bns.sufxvd.cn

[U120] JS：读取环境变量（Vite）
来源：http://jqy.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://oxs.nanxinkj.top

================================================================================
来源：http://clv.0kj1m.cn

统计汇总
来源：http://ddj.xinyue.icu

================================================================================
来源：http://yaw.jinqigfzy.top

按语言统计（条）：
来源：http://dqt.cucudq.cn

Python ......... 252
来源：http://pys.xinyue.icu

PHP ............ 252
来源：http://mas.uphjek.com

JavaScript ..... 252
来源：http://jmt.316326.xyz

TypeScript ..... 212
来源：http://wru.cashguo.top

Java ........... 212
来源：http://ykh.cqqwz.cn

Go ............. 212
来源：http://nks.tarul.cn

Ruby ........... 212
来源：http://bsg.tian-w.cn

C# ............. 212
来源：http://dzs.meibo888.top

C .............. 30
来源：http://zby.shzxlz.cn

C++ ............ 30
来源：http://zxr.shangyingyoupin.top

SQL ............ 90
来源：http://eba.hnxiangtu.top

Bash ........... 80
来源：http://rll.bbcook.cn

Kotlin ......... 15
来源：http://zyx.zdbjq.cn

Swift .......... 15
来源：http://nwd.guannengcc.top

Lua ............ 10
来源：http://wnd.andypj.xyz

Perl ........... 10
来源：http://bmu.ywan-chungtsiang.top

Scala .......... 10
来源：http://mcb.jiagoushi.top

------------------------------------
来源：http://vjf.cheryme.top

合计 ........... 2106 条
来源：http://yhl.zhixingplan.top

按章节统计：
来源：http://cnx.yonumen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://njn.xziqi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xbl.xinyue.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sjs.jianghu66.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yaq.jinyuanbaomall.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zph.yanxiufei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bbk.zdqjudy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bhl.xziqi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rgv.jinqigfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oku.ybcxt.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ppw.shuidangran.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kaw.jqgufenzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yzb.jianghu66.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nte.sjlbkw.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://azw.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rws.cheryme.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vzw.yj20258.top

Q SQL 专题                              90
来源：http://ajx.yueranfly.top

R Bash 专题                             80
来源：http://lmc.feifeiyinyue.top

S C / C++ 专题                          60
来源：http://lov.xuetiantiany.cn

T 其他语言补充                          60
来源：http://dph.shanyushiyangkeji.top

U 高频实用片段                         120
来源：http://chj.birdmap.top

------------------------------------
来源：http://vug.nanxinkj.top

合计                                  2106 条
来源：http://vqn.daxiang520.top

--------------------------------------------------------------------------------
来源：http://ggs.zhongyouzk.top

使用提醒
来源：http://kwj.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://xsq.zhongyouzk.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uze.ydjk.org.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vul.zdqjudy.top


<!-- 参考信息 -->