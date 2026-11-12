代发 wailian999

val a = 1;  var b = 2
来源：http://pfu.bjfxy.top

[T53] Scala：字符串插值
来源：http://tvq.aibaodan.cn

s"值: $b"
来源：http://sjt.zhijiandao.cn

[T54] Scala：集合映射
来源：http://bmu.ctjpmb.com

List(1, 2, 3).map(_ * 2)
来源：http://tos.hammf.cn

[T55] Scala：集合过滤
来源：http://jjb.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://nti.tianlin.xyz

[T56] Scala：样例类
来源：http://wka.sjlbkw.cn

case class User(name: String, age: Int)
来源：http://cho.cashguo.top

[T57] Scala：模式匹配
来源：http://zxs.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pks.sysykeji.top

[T58] Scala：函数定义
来源：http://yup.yvedp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://exf.hnqzz.top

[T59] Scala：循环
来源：http://wgf.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://mxk.cdnleiting.top

[T60] Scala：折叠
来源：http://cuy.zdbjq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://naj.epnwcf.com

================================================================================
来源：http://dgr.zdqjudy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vmh.cdnleiting.top

================================================================================
来源：http://qdd.52xcode.cn

[U01] Py：创建虚拟环境
来源：http://sip.daxiang520.top

python -m venv .venv && source .venv/bin/activate
来源：http://rjf.cheryme.top

[U02] Py：导出 / 安装依赖
来源：http://puc.tanke756.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://smn.hfpthk.cn

[U03] Py：加载 .env 配置
来源：http://qxj.wangdashe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wie.shzxlz.cn

[U04] Py：变量调试打印
来源：http://muz.nanxinkj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mvm.zdqjudy.top

[U05] Py：列表去重且保序
来源：http://dib.fktsv.cn

list(dict.fromkeys(arr))
来源：http://jyy.yuanzhike.top

[U06] Py：合并两个字典
来源：http://cbj.shangyingyoupin.top

{**a, **b}
来源：http://yel.havefunace.top

[U07] Py：反转字典键值
来源：http://xji.iojbl.cn

{v: k for k, v in d.items()}
来源：http://oiw.52xcode.cn

[U08] Py：展平二维列表
来源：http://dxy.mhx1999.top

[y for x in nested for y in x]
来源：http://pkq.fehbvm.com

[U09] Py：字典取最大值的键
来源：http://xlw.0kj1m.cn

max(d, key=d.get)
来源：http://qmb.xingfuxueyuan.xyz

[U10] Py：按值排序字典
来源：http://qzv.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vgl.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://kpp.aibaodan.cn

(x * 2 for x in arr)
来源：http://ptb.cdnleiting.top

[U12] Py：取出现最多的 3 个元素
来源：http://brm.fktsv.cn

Counter(arr).most_common(3)
来源：http://qwf.iojbl.cn

[U13] Py：固定长度队列
来源：http://nmc.feifeiyinyue.top

deque(maxlen=10)
来源：http://kmx.jyoumei.cn

[U14] Py：分组收集到列表
来源：http://nct.hnqzz.top

defaultdict(list)
来源：http://fnr.sxryk.cn

[U15] Py：高精度计时
来源：http://bix.xziqi.cn

t = time.perf_counter()
来源：http://rmv.bbcook.cn

[U16] Py：命令行参数解析
来源：http://yov.hfpthk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xvl.fanxiaobao.xyz

[U17] Py：初始化日志
来源：http://vji.vqdsnc.cn

logging.basicConfig(level=logging.INFO)
来源：http://dkb.hfpthk.cn

[U18] Py：预编译正则
来源：http://umz.fengsongda.top

pat = re.compile(r"\d+")
来源：http://yrj.jinqigfzy.top

[U19] Py：正则替换带回调
来源：http://cvk.gaohongyu789.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nvd.zhoulong.xyz

[U20] Py：缓存函数结果
来源：http://lmq.yfazqb.com

@functools.lru_cache(maxsize=None)
来源：http://cqt.ehwqpu.com

[U21] Py：自定义上下文管理器
来源：http://vmu.yvedp.cn

@contextlib.contextmanager
来源：http://gns.nwbrower.top

[U22] Py：矩阵转置
来源：http://owc.tarul.cn

list(zip(*m))
来源：http://mbf.pycfn.com

[U23] Py：分块读取大文件
来源：http://uqk.pengpengdd.cyou

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vue.fengsongda.top

[U24] Py：路径操作
来源：http://scp.daria6918.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fbn.jinghuilouyu.cn

[U25] Py：CSV 按字典读
来源：http://qnh.fengsongda.top

csv.DictReader(f)
来源：http://pmx.zhiwuduotai.top

[U26] Py：并发下载
来源：http://njf.yonumen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://teu.dashuyun.cn

[U27] Py：异步 HTTP
来源：http://bkn.hnxiangtu.top

aiohttp.ClientSession() 配合 async with
来源：http://jfv.yanxiufei.cn

[U28] Py：类型别名
来源：http://fmi.guowangkeji.top

UserId = int
来源：http://wai.zhijiandao.cn

[U29] Py：属性校验
来源：http://cda.ivvv.top

@property 与 @x.setter 配合
来源：http://hbj.yongpay.top

[U30] Py：数据类
来源：http://zjl.redwolf501.top

@dataclass(slots=True)
来源：http://hhz.tarul.cn

[U31] Py：单测
来源：http://ayg.cdnleiting.top

python -m pytest -q
来源：http://aas.jinghuilouyu.cn

[U32] Py：代码格式化
来源：http://bhi.9152youxi.cn

ruff format . && ruff check --fix .
来源：http://kqa.zhixingplan.top

[U33] Py：打包发布
来源：http://ncs.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://ewn.c1oappe.top

[U34] Py：判断编码
来源：http://wfm.xuetiantiany.cn

chardet.detect(raw)
来源：http://hba.epnwcf.com

[U35] Py：发送邮件
来源：http://rem.hnqzz.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iga.birdmap.top

[U36] Py：定时任务
来源：http://unp.gogol.net.cn

schedule.every(10).minutes.do(job)
来源：http://jra.yfazqb.com

[U37] Py：读写 Excel
来源：http://joa.ydzc1.top

pandas.read_excel / DataFrame.to_excel
来源：http://xml.yj20258888.top

[U38] Py：获取脚本所在目录
来源：http://pkj.nanxinkj.top

Path(__file__).resolve().parent
来源：http://mua.ehwqpu.com

[U39] Py：判断是否在交互环境
来源：http://gjn.chenzaomai.com

sys.stdout.isatty()
来源：http://ymo.cashguo.top

[U40] Py：打印到标准错误
来源：http://ajb.yfazqb.com

print("err", file=sys.stderr)
来源：http://lsp.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://xlh.jqgufenzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lgx.0kj1m.cn

[U42] PHP：PSR-4 自动加载
来源：http://bfa.cashguo.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://enx.zhaomingkeji.xyz

[U43] PHP：声明命名空间
来源：http://rvn.yonumen.top

namespace App\Http;
来源：http://uog.xingfuxueyuan.xyz

[U44] PHP：开启严格类型
来源：http://yzk.yj202588.top

declare(strict_types=1);
来源：http://nbl.fanxiaobao.xyz

[U45] PHP：类型声明与返回类型
来源：http://pgt.quarkkingdee.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hdc.ydzc1.top

[U46] PHP：可空类型
来源：http://vyv.ybcxt.top

?string $name = null
来源：http://lwu.sweek.top

[U47] PHP：联合类型
来源：http://oie.xuanzx.com

int|string $id
来源：http://smd.jlsjyb.cn

[U48] PHP：纯枚举
来源：http://uml.hysaishi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nam.fktsv.cn

[U49] PHP：只读属性
来源：http://gry.yongpay.top

public readonly string $name
来源：http://ztc.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://cgt.meibo888.top

public function __construct(private int $id) {}
来源：http://yna.xylfe.cn

[U51] PHP：数组解构
来源：http://web.jyoumei.cn

[$a, $b] = $arr;
来源：http://vys.vehdjk.com

[U52] PHP：箭头函数
来源：http://rdl.gaohongyu789.top

$double = fn($x) => $x * 2;
来源：http://jxe.uphjek.com

[U53] PHP：空合并运算符
来源：http://dvq.316326.xyz

$v = $a ?? $b ?? "default";
来源：http://toc.yj20258.top

[U54] PHP：空安全调用
来源：http://vdg.daxiang520.top

$obj?->method()
来源：http://vct.zhixingplan.top

[U55] PHP：match 表达式
来源：http://pcg.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xvq.fengsongda.top

[U56] PHP：命名参数
来源：http://nbr.xziqi.cn

f(a: 1, b: 2)
来源：http://rtv.hcnkem.com

[U57] PHP：字符串插值
来源：http://cbd.zhengqikj.top

"值: {$a}"
来源：http://gwq.quarkkingdee.top

[U58] PHP：数组三件套
来源：http://ijy.sufxvd.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tkw.nanxuanxn.top

[U59] PHP：自定义排序
来源：http://qsj.yangfankeji.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://glg.epnwcf.com

[U60] PHP：JSON 编解码
来源：http://ois.zhoulong.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bqz.guowangkeji.top

[U61] PHP：正则
来源：http://opt.316326.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tln.hnxiangtu.top

[U62] PHP：日期对象
来源：http://ceb.chenjidiqi.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xeg.tian-w.cn

[U63] PHP：文件读写
来源：http://hum.shzxlz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zmm.havefunace.top

[U64] PHP：目录遍历
来源：http://vpg.jinqigfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://ytw.ehwqpu.com

[U65] PHP：会话
来源：http://sry.cqqwz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://agd.hongshengwenyu.top

[U66] PHP：设置 Cookie
来源：http://fck.tianlin.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://stl.yanxiufei.cn

[U67] PHP：处理文件上传
来源：http://aya.pengpengdd.cyou

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rki.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://ngy.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bcw.tian-w.cn

[U69] PHP：PDO 预处理
来源：http://evc.gogol.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ooh.fehbvm.com

[U70] PHP：PDO 事务
来源：http://egl.52xcode.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jkb.xuetiantiany.cn

[U71] PHP：抛出异常
来源：http://hmx.hywenlv.cn

throw new RuntimeException("失败", 500);
来源：http://gai.0kj1m.cn

[U72] PHP：写错误日志
来源：http://jbj.xuanzx.com

error_log("失败: " . $e->getMessage());
来源：http://vls.hysaishi.cn

[U73] PHP：读取 ini 配置
来源：http://dji.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://qcm.fktsv.cn

[U74] PHP：读取环境变量
来源：http://gpp.0kj1m.cn

getenv("APP_ENV") ?: "production"
来源：http://idz.0kj1m.cn

[U75] PHP：依赖注入
来源：http://pwf.jqgufenzy.top

composer require psr/container
来源：http://vai.hfpthk.cn

[U76] PHP：简单路由
来源：http://nqt.gzhubu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zir.jiagoushi.top

[U77] PHP：模板渲染
来源：http://gvf.jqgfzy.top

composer require twig/twig
来源：http://hbp.hcnkem.com

[U78] PHP：单元测试
来源：http://ljw.zhixingplan.top

composer require --dev phpunit/phpunit
来源：http://joj.birdmap.top

[U79] PHP：静态分析
来源：http://ohz.yvedp.cn

composer require --dev phpstan/phpstan
来源：http://jby.vqdsnc.cn

[U80] PHP：代码规范修复
来源：http://zpc.hysaishi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lqq.nwbrower.top

[U81] JS：初始化项目
来源：http://hov.xuanzx.com

npm init -y;  npm i express
来源：http://enc.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://itu.cqqwz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jai.hfpthk.cn

[U83] JS：ES Module 导入导出
来源：http://khz.ydzc1.top

export const a = 1;  import { a } from "./m.js";
来源：http://lzl.sysykeji.top

[U84] JS：CommonJS 写法
来源：http://hdf.andypj.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://vff.nanxinkj.top

[U85] JS：可选链
来源：http://boz.chenlongwang.top

a?.b?.c
来源：http://qhz.zhaomingkeji.xyz

[U86] JS：空值合并
来源：http://xaw.shanyushiyangtech.top

a ?? b
来源：http://dgm.yangfankeji.com

[U87] JS：解构默认值
来源：http://dnu.sjlbkw.cn

const { a = 1, b = 2 } = obj;
来源：http://mjg.yangfankeji.com

[U88] JS：对象展开合并
来源：http://ltn.zhijiandao.cn

{ ...a, ...b }
来源：http://oug.zhengqikj.top

[U89] JS：数组去重
来源：http://lhx.jianghu66.top

[...new Set(arr)]
来源：http://gxa.sxryk.cn

[U90] JS：数字数组排序
来源：http://ruf.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://lvw.havefunace.top

[U91] JS：对象键值遍历
来源：http://uax.jiagoushi.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cyl.ivvv.top

[U92] JS：深拷贝
来源：http://upd.xylfe.cn

structuredClone(obj)
来源：http://vjp.zhixingplan.top

[U93] JS：模板字符串
来源：http://sub.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://akw.jqgfzy.top

[U94] JS：箭头函数
来源：http://pjq.yueranfly.top

const double = x => x * 2;
来源：http://vml.c1oappe.top

[U95] JS：Promise 包装
来源：http://jrx.ctjpmb.com

new Promise((resolve, reject) => {})
来源：http://cbc.smart0.xyz

[U96] JS：async/await 与异常
来源：http://iwo.bjfxy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yyr.yfazqb.com

[U97] JS：并发请求
来源：http://ahi.jinqigufen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cgc.xingfuxueyuan.xyz

[U98] JS：fetch 带 JSON
来源：http://qdm.shzxlz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mwu.jyoumei.cn

[U99] JS：事件监听
来源：http://bza.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://clk.jinqigfzy.top

[U100] JS：DOM 查询
来源：http://qdp.dashuyun.cn

document.querySelector(".item")
来源：http://ubt.xuetiantiany.cn

[U101] JS：classList 操作
来源：http://npn.zycfv.cn

el.classList.toggle("active")
来源：http://yye.0kj1m.cn

[U102] JS：本地存储
来源：http://cbz.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xvl.sweek.top

[U103] JS：定时器
来源：http://yiw.yuanzhike.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jtx.0kj1m.cn

[U104] JS：防抖
来源：http://dsu.zhongyouzk.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rvg.chenjidiqi.icu

[U105] JS：节流
来源：http://asg.svipenyu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://asb.haohaochexian.top

[U106] JS：日期格式化
来源：http://ivo.feifeiyinyue.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jao.hywenlv.cn

[U107] JS：数字千分位
来源：http://iar.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wrg.sjlbkw.cn

[U108] JS：随机整数
来源：http://vkz.tian-w.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ogs.tianlin.xyz

[U109] JS：数组分组
来源：http://zlc.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://pyh.yonumen.top

[U110] JS：数组分块
来源：http://evn.xziqi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xkf.ybcxt.top

[U111] JS：对象转 Map
来源：http://iqo.xinyue.icu

new Map(Object.entries(obj))
来源：http://ysj.cashguo.top

[U112] JS：字符串补位
来源：http://mde.tian-w.cn

"7".padStart(3, "0")
来源：http://vnz.316326.xyz

[U113] JS：正则替换全部
来源：http://ryw.ivvv.top

s.replaceAll("a", "b")
来源：http://frd.gzhubu.top

[U114] JS：JSON 深比较
来源：http://noy.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hom.svipenyu.cn

[U115] JS：生成 UUID
来源：http://gwb.shanyushiyangtech.top

crypto.randomUUID()
来源：http://mmv.dianchejie.cn

[U116] JS：类型检查（JSDoc）
来源：http://ybr.gzhubu.top

/** @param {string} name */ function f(name) {}
来源：http://eii.yuxming.cn

[U117] JS：单元测试
来源：http://ogp.xylfe.cn

npm i -D vitest;  npx vitest
来源：http://sjb.meibo888.top

[U118] JS：开发服务器
来源：http://rru.epnwcf.com

npm i -D vite;  npx vite
来源：http://wpi.vqdsnc.cn

[U119] JS：生产构建
来源：http://hhn.feifeiyinyue.top

npx vite build
来源：http://egp.dianchejie.cn

[U120] JS：读取环境变量（Vite）
来源：http://nul.nwbrower.top

import.meta.env.VITE_API_URL
来源：http://pyp.ctjpmb.com

================================================================================
来源：http://zom.yonumen.top

统计汇总
来源：http://ulj.guowangkeji.top

================================================================================
来源：http://wih.zhaomingkeji.xyz

按语言统计（条）：
来源：http://wgw.nwbrower.top

Python ......... 252
来源：http://uie.gzhubu.top

PHP ............ 252
来源：http://czb.jyoumei.cn

JavaScript ..... 252
来源：http://grn.c1oappe.top

TypeScript ..... 212
来源：http://ozp.yuxming.cn

Java ........... 212
来源：http://lyh.jqgfzy.top

Go ............. 212
来源：http://wmx.cheryme.top

Ruby ........... 212
来源：http://gsv.tianlin.xyz

C# ............. 212
来源：http://swz.tarul.cn

C .............. 30
来源：http://ppb.cdnleiting.top

C++ ............ 30
来源：http://ewc.9152youxi.cn

SQL ............ 90
来源：http://hvh.nanxinkj.top

Bash ........... 80
来源：http://vho.cheryme.top

Kotlin ......... 15
来源：http://rdv.ppjwa.cn

Swift .......... 15
来源：http://qwx.snrcjt.cn

Lua ............ 10
来源：http://evt.xziqi.cn

Perl ........... 10
来源：http://oya.pycfn.com

Scala .......... 10
来源：http://syy.tian-w.cn

------------------------------------
来源：http://sqe.52xcode.cn

合计 ........... 2106 条
来源：http://mai.ehwqpu.com

按章节统计：
来源：http://gvb.xziqi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hqh.sufxvd.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gxi.hammf.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vgl.nanxinkj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wyp.dashuyun.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cuf.tanke756.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hen.nanxuanxn.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ogc.gogol.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bnn.hesvh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ykt.sjlbkw.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://owq.hfpthk.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zkf.0kj1m.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rqo.jiagoushi.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://aib.guannengcc.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pib.ywan-chungtsiang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cuq.316326.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ktn.ivvv.top


<!-- 参考信息 -->