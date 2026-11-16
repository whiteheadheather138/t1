代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://ktf.zhiwuduotai.top

[T55] Scala：集合过滤
来源：http://lmw.tanke756.top

List(1, 2, 3).filter(_ > 1)
来源：http://aru.xinyue.icu

[T56] Scala：样例类
来源：http://ekc.nanxuanxn.top

case class User(name: String, age: Int)
来源：http://svi.bbcook.cn

[T57] Scala：模式匹配
来源：http://phc.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qbt.hongshengwenyu.top

[T58] Scala：函数定义
来源：http://coc.epnwcf.com

def add(a: Int, b: Int): Int = a + b
来源：http://hjw.zhiwuduotai.top

[T59] Scala：循环
来源：http://pjb.gaohongyu789.top

for (i <- 1 to 10) println(i)
来源：http://wgd.zhiwuduotai.top

[T60] Scala：折叠
来源：http://xkw.jqgfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xcs.aibaodan.cn

================================================================================
来源：http://czf.tianlin.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rgw.nanxinkj.top

================================================================================
来源：http://phu.gzhubu.top

[U01] Py：创建虚拟环境
来源：http://zqe.jianghu66.top

python -m venv .venv && source .venv/bin/activate
来源：http://gpg.sjlbkw.cn

[U02] Py：导出 / 安装依赖
来源：http://gas.guowangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qtp.mhx1999.top

[U03] Py：加载 .env 配置
来源：http://sdy.snrcjt.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kah.svipenyu.cn

[U04] Py：变量调试打印
来源：http://ccb.guowangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kgp.cdnleiting.top

[U05] Py：列表去重且保序
来源：http://lqy.zhoulong.xyz

list(dict.fromkeys(arr))
来源：http://rwg.gogol.net.cn

[U06] Py：合并两个字典
来源：http://tcv.fengsongda.top

{**a, **b}
来源：http://cez.svipenyu.cn

[U07] Py：反转字典键值
来源：http://ipu.cqqwz.cn

{v: k for k, v in d.items()}
来源：http://oqn.shanyushiyangkeji.top

[U08] Py：展平二维列表
来源：http://rag.daxiang520.top

[y for x in nested for y in x]
来源：http://aro.yongpay.top

[U09] Py：字典取最大值的键
来源：http://fgh.meibo888.top

max(d, key=d.get)
来源：http://hcg.yuxming.cn

[U10] Py：按值排序字典
来源：http://iac.tian-w.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fib.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://obn.316326.xyz

(x * 2 for x in arr)
来源：http://fej.pycfn.com

[U12] Py：取出现最多的 3 个元素
来源：http://erg.ydzc1.top

Counter(arr).most_common(3)
来源：http://mjk.nwbrower.top

[U13] Py：固定长度队列
来源：http://yfc.chenzaomai.com

deque(maxlen=10)
来源：http://fbi.yongpay.top

[U14] Py：分组收集到列表
来源：http://pqa.haohaochexian.top

defaultdict(list)
来源：http://byb.hnqzz.top

[U15] Py：高精度计时
来源：http://wpw.hnxiangtu.top

t = time.perf_counter()
来源：http://zac.smart0.xyz

[U16] Py：命令行参数解析
来源：http://qjo.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fxc.tanke756.top

[U17] Py：初始化日志
来源：http://dyg.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://nsg.jlsjyb.cn

[U18] Py：预编译正则
来源：http://fnt.yongpay.top

pat = re.compile(r"\d+")
来源：http://uhm.mhx1999.top

[U19] Py：正则替换带回调
来源：http://ibm.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wji.shzxlz.cn

[U20] Py：缓存函数结果
来源：http://whq.yonumen.top

@functools.lru_cache(maxsize=None)
来源：http://vkr.zhiwuduotai.top

[U21] Py：自定义上下文管理器
来源：http://ssi.9152youxi.cn

@contextlib.contextmanager
来源：http://srz.hnqzz.top

[U22] Py：矩阵转置
来源：http://aqe.wangdashe.top

list(zip(*m))
来源：http://aol.zdbjq.cn

[U23] Py：分块读取大文件
来源：http://xku.shangyingyoupin.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qcx.jinqigfzy.top

[U24] Py：路径操作
来源：http://tbk.tian-w.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gcl.ctjpmb.com

[U25] Py：CSV 按字典读
来源：http://pxq.vqdsnc.cn

csv.DictReader(f)
来源：http://apr.jianghu66.top

[U26] Py：并发下载
来源：http://jtp.9152youxi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nub.svipenyu.cn

[U27] Py：异步 HTTP
来源：http://dmk.epnwcf.com

aiohttp.ClientSession() 配合 async with
来源：http://fge.zhongyouzk.top

[U28] Py：类型别名
来源：http://efg.meibo888.top

UserId = int
来源：http://dzu.shanyushiyangkeji.top

[U29] Py：属性校验
来源：http://rzb.yangfankeji.com

@property 与 @x.setter 配合
来源：http://pgl.shanyushiyangkeji.top

[U30] Py：数据类
来源：http://tpd.bbcook.cn

@dataclass(slots=True)
来源：http://ggt.kuanghao11.cn

[U31] Py：单测
来源：http://qza.c1oappe.top

python -m pytest -q
来源：http://skb.zdqjudy.top

[U32] Py：代码格式化
来源：http://xnw.zhijiandao.cn

ruff format . && ruff check --fix .
来源：http://rja.52xcode.cn

[U33] Py：打包发布
来源：http://uhf.zdbjq.cn

python -m build  （依赖 pyproject.toml）
来源：http://cwh.gzhubu.top

[U34] Py：判断编码
来源：http://qwr.hnxiangtu.top

chardet.detect(raw)
来源：http://irl.bjfxy.top

[U35] Py：发送邮件
来源：http://ott.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://leu.316326.xyz

[U36] Py：定时任务
来源：http://uzu.jinqigfzy.top

schedule.every(10).minutes.do(job)
来源：http://vrj.guowangkeji.top

[U37] Py：读写 Excel
来源：http://oki.zycfv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://agt.yueranfly.top

[U38] Py：获取脚本所在目录
来源：http://ics.bjfxy.top

Path(__file__).resolve().parent
来源：http://tko.hfpthk.cn

[U39] Py：判断是否在交互环境
来源：http://btj.cdnleiting.top

sys.stdout.isatty()
来源：http://ocl.shangyingyoupin.top

[U40] Py：打印到标准错误
来源：http://gtr.tanke756.top

print("err", file=sys.stderr)
来源：http://fxa.hongshengwenyu.top

[U41] PHP：初始化 Composer 项目
来源：http://ybi.yanxiufei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://snj.yfazqb.com

[U42] PHP：PSR-4 自动加载
来源：http://rwv.tarul.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://efj.zhaomingkeji.xyz

[U43] PHP：声明命名空间
来源：http://wfk.havefunace.top

namespace App\Http;
来源：http://lzs.daxiang520.top

[U44] PHP：开启严格类型
来源：http://wxu.jianghu66.top

declare(strict_types=1);
来源：http://tod.hysaishi.cn

[U45] PHP：类型声明与返回类型
来源：http://jds.kuanghao11.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rbo.vehdjk.com

[U46] PHP：可空类型
来源：http://xqh.xinyue.icu

?string $name = null
来源：http://vts.cucudq.cn

[U47] PHP：联合类型
来源：http://vrq.kuanghao11.cn

int|string $id
来源：http://kxw.xylfe.cn

[U48] PHP：纯枚举
来源：http://yxr.chenlongwang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ejs.mhx1999.top

[U49] PHP：只读属性
来源：http://ktf.nwbrower.top

public readonly string $name
来源：http://fbn.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://iyr.sxryk.cn

public function __construct(private int $id) {}
来源：http://ozz.chenzaomai.com

[U51] PHP：数组解构
来源：http://hbl.feifeiyinyue.top

[$a, $b] = $arr;
来源：http://ign.yj20258.top

[U52] PHP：箭头函数
来源：http://nlz.zhengqikj.top

$double = fn($x) => $x * 2;
来源：http://ueq.haohaochexian.top

[U53] PHP：空合并运算符
来源：http://dbq.yonumen.top

$v = $a ?? $b ?? "default";
来源：http://zjs.xinyue.icu

[U54] PHP：空安全调用
来源：http://zrm.aibaodan.cn

$obj?->method()
来源：http://tiz.cashguo.top

[U55] PHP：match 表达式
来源：http://vnm.shuidangran.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ufw.ctjpmb.com

[U56] PHP：命名参数
来源：http://hmk.yj20258.top

f(a: 1, b: 2)
来源：http://cro.shanyushiyangtech.top

[U57] PHP：字符串插值
来源：http://plz.xingfuxueyuan.xyz

"值: {$a}"
来源：http://ubo.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://rsp.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cot.yuanzhike.top

[U59] PHP：自定义排序
来源：http://zsr.hywenlv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ezy.hywenlv.cn

[U60] PHP：JSON 编解码
来源：http://kcd.yueranfly.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://aut.ppjwa.cn

[U61] PHP：正则
来源：http://lmj.tarul.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jao.zhongyouzk.top

[U62] PHP：日期对象
来源：http://fis.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jkt.daxiang520.top

[U63] PHP：文件读写
来源：http://xug.chenzaomai.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gmb.shangyingyoupin.top

[U64] PHP：目录遍历
来源：http://knj.9152youxi.cn

glob("dir/*.php");  scandir("dir");
来源：http://fiv.gogol.net.cn

[U65] PHP：会话
来源：http://wgt.cdnleiting.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tbz.cucudq.cn

[U66] PHP：设置 Cookie
来源：http://dnf.redwolf501.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zxo.iojbl.cn

[U67] PHP：处理文件上传
来源：http://xgo.shangyingyoupin.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jan.yueranfly.top

[U68] PHP：PDO 连接
来源：http://xii.zhixingplan.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uff.hcnkem.com

[U69] PHP：PDO 预处理
来源：http://air.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xgc.ehwqpu.com

[U70] PHP：PDO 事务
来源：http://mxj.xziqi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rhl.vqdsnc.cn

[U71] PHP：抛出异常
来源：http://muk.yuxming.cn

throw new RuntimeException("失败", 500);
来源：http://ugl.aibaodan.cn

[U72] PHP：写错误日志
来源：http://htv.vqdsnc.cn

error_log("失败: " . $e->getMessage());
来源：http://yhi.jiagoushi.top

[U73] PHP：读取 ini 配置
来源：http://swq.xinyue.icu

parse_ini_file("config.ini", true)
来源：http://bvi.hysaishi.cn

[U74] PHP：读取环境变量
来源：http://glz.fktsv.cn

getenv("APP_ENV") ?: "production"
来源：http://krv.gogol.net.cn

[U75] PHP：依赖注入
来源：http://tlf.shzxlz.cn

composer require psr/container
来源：http://rwy.vehdjk.com

[U76] PHP：简单路由
来源：http://ans.yvedp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fwe.meibo888.top

[U77] PHP：模板渲染
来源：http://lkq.xziqi.cn

composer require twig/twig
来源：http://ere.zhiwuduotai.top

[U78] PHP：单元测试
来源：http://yfg.sxryk.cn

composer require --dev phpunit/phpunit
来源：http://jai.sxryk.cn

[U79] PHP：静态分析
来源：http://ysg.fzhhl.top

composer require --dev phpstan/phpstan
来源：http://ptf.fzhhl.top

[U80] PHP：代码规范修复
来源：http://yll.sjlbkw.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://eky.yfazqb.com

[U81] JS：初始化项目
来源：http://qvs.iojbl.cn

npm init -y;  npm i express
来源：http://kqp.hesvh.cn

[U82] JS：package.json 脚本
来源：http://mfx.cqqwz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ljn.jinqigfzy.top

[U83] JS：ES Module 导入导出
来源：http://wwq.fehbvm.com

export const a = 1;  import { a } from "./m.js";
来源：http://edy.nwbrower.top

[U84] JS：CommonJS 写法
来源：http://spp.pycfn.com

module.exports = { a };  const { a } = require("./m");
来源：http://tcy.9152youxi.cn

[U85] JS：可选链
来源：http://erf.zdbjq.cn

a?.b?.c
来源：http://xxz.ywan-chungtsiang.top

[U86] JS：空值合并
来源：http://cgv.tianlin.xyz

a ?? b
来源：http://czf.chenzaomai.com

[U87] JS：解构默认值
来源：http://cab.xingfuxueyuan.xyz

const { a = 1, b = 2 } = obj;
来源：http://ijo.cashguo.top

[U88] JS：对象展开合并
来源：http://sqe.aibaodan.cn

{ ...a, ...b }
来源：http://neh.meibo888.top

[U89] JS：数组去重
来源：http://jhp.fengsongda.top

[...new Set(arr)]
来源：http://utt.shanyushiyangkeji.top

[U90] JS：数字数组排序
来源：http://lfv.guowangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://xyl.zhixingplan.top

[U91] JS：对象键值遍历
来源：http://ijy.fktsv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://voq.andypj.xyz

[U92] JS：深拷贝
来源：http://pse.yuxming.cn

structuredClone(obj)
来源：http://ecq.hnqzz.top

[U93] JS：模板字符串
来源：http://ket.quarkkingdee.top

`共 ${n} 条`
来源：http://wkp.daxiang520.top

[U94] JS：箭头函数
来源：http://kfb.nanxuanxn.top

const double = x => x * 2;
来源：http://ola.uphjek.com

[U95] JS：Promise 包装
来源：http://rfs.ybcxt.top

new Promise((resolve, reject) => {})
来源：http://lsb.xziqi.cn

[U96] JS：async/await 与异常
来源：http://cje.fzhhl.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iyb.xziqi.cn

[U97] JS：并发请求
来源：http://ncp.nwbrower.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://fav.cdnleiting.top

[U98] JS：fetch 带 JSON
来源：http://jkm.chenzaomai.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://apb.aibaodan.cn

[U99] JS：事件监听
来源：http://lyc.shzxlz.cn

el.addEventListener("click", e => {})
来源：http://njb.nanxuanxn.top

[U100] JS：DOM 查询
来源：http://rvd.cucudq.cn

document.querySelector(".item")
来源：http://suo.gotoacloud.top

[U101] JS：classList 操作
来源：http://gik.sysykeji.top

el.classList.toggle("active")
来源：http://ewm.ydzc1.top

[U102] JS：本地存储
来源：http://mvu.yongpay.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rfr.andypj.xyz

[U103] JS：定时器
来源：http://uem.jlsjyb.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wey.cheryme.top

[U104] JS：防抖
来源：http://oum.nwbrower.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uuy.zdqjudy.top

[U105] JS：节流
来源：http://vli.haohaochexian.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://slq.tarul.cn

[U106] JS：日期格式化
来源：http://yuz.sjlbkw.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lry.cdnleiting.top

[U107] JS：数字千分位
来源：http://srk.yfazqb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lgs.mhx1999.top

[U108] JS：随机整数
来源：http://kmv.nwbrower.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lif.chenzaomai.com

[U109] JS：数组分组
来源：http://bev.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://ljq.bjfxy.top

[U110] JS：数组分块
来源：http://eki.hesvh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dtk.hcnkem.com

[U111] JS：对象转 Map
来源：http://tlm.zhaomingkeji.xyz

new Map(Object.entries(obj))
来源：http://tkw.uphjek.com

[U112] JS：字符串补位
来源：http://mgw.nanxuanxn.top

"7".padStart(3, "0")
来源：http://hdq.jianghu66.top

[U113] JS：正则替换全部
来源：http://twa.cdnleiting.top

s.replaceAll("a", "b")
来源：http://yef.chenjidiqi.icu

[U114] JS：JSON 深比较
来源：http://xpf.iojbl.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uhf.shzxlz.cn

[U115] JS：生成 UUID
来源：http://nup.fanxiaobao.xyz

crypto.randomUUID()
来源：http://afl.316326.xyz

[U116] JS：类型检查（JSDoc）
来源：http://wfb.shangyingyoupin.top

/** @param {string} name */ function f(name) {}
来源：http://yev.jianghu66.top

[U117] JS：单元测试
来源：http://jid.jinghuilouyu.cn

npm i -D vitest;  npx vitest
来源：http://yhy.havefunace.top

[U118] JS：开发服务器
来源：http://owx.yuxming.cn

npm i -D vite;  npx vite
来源：http://yvu.zdqjudy.top

[U119] JS：生产构建
来源：http://ger.nanxinkj.top

npx vite build
来源：http://ryk.ppjwa.cn

[U120] JS：读取环境变量（Vite）
来源：http://pyx.shzxlz.cn

import.meta.env.VITE_API_URL
来源：http://mkm.ydjk.org.cn

================================================================================
来源：http://xrm.jqgufenzy.top

统计汇总
来源：http://vbw.hongshengwenyu.top

================================================================================
来源：http://lns.cucudq.cn

按语言统计（条）：
来源：http://pdn.shangyingyoupin.top

Python ......... 252
来源：http://twr.zhijiandao.cn

PHP ............ 252
来源：http://wnl.yangfankeji.com

JavaScript ..... 252
来源：http://bza.snrcjt.cn

TypeScript ..... 212
来源：http://yww.aizwys.cn

Java ........... 212
来源：http://kju.xingfuxueyuan.xyz

Go ............. 212
来源：http://ghf.pycfn.com

Ruby ........... 212
来源：http://dyq.iojbl.cn

C# ............. 212
来源：http://vtk.hcnkem.com

C .............. 30
来源：http://jwe.chenjidiqi.icu

C++ ............ 30
来源：http://cwc.pengpengdd.cyou

SQL ............ 90
来源：http://cwu.havefunace.top

Bash ........... 80
来源：http://khr.xziqi.cn

Kotlin ......... 15
来源：http://lay.uphjek.com

Swift .......... 15
来源：http://bdy.cucudq.cn

Lua ............ 10
来源：http://fei.uphjek.com

Perl ........... 10
来源：http://eqc.jqgufenzy.top

Scala .......... 10
来源：http://yxd.xinyue.icu

------------------------------------
来源：http://wjx.xingfuxueyuan.xyz

合计 ........... 2106 条
来源：http://lgz.havefunace.top

按章节统计：
来源：http://hpz.zhoulong.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eje.hnxiangtu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uun.hnqzz.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://alw.andypj.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rja.shanyushiyangtech.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wvx.yuxming.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wsj.zhijiandao.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vqa.jqgufenzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kmh.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uew.kuanghao11.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fpd.epnwcf.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://spl.nanxinkj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pxl.pycfn.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rao.xinyue.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hqz.nanxinkj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fgk.cashguo.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dzg.zycfv.cn

Q SQL 专题                              90
来源：http://oro.fehbvm.com

R Bash 专题                             80
来源：http://vvw.316326.xyz

S C / C++ 专题                          60
来源：http://sek.nanxuanxn.top

T 其他语言补充                          60
来源：http://fsm.tianlin.xyz


<!-- 参考信息 -->