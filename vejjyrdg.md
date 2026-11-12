代发 wailian999

[U03] Py：加载 .env 配置
来源：http://tin.cashguo.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zhc.fengsongda.top

[U04] Py：变量调试打印
来源：http://xwg.sufxvd.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ivb.chenlongwang.top

[U05] Py：列表去重且保序
来源：http://rdh.gotoacloud.top

list(dict.fromkeys(arr))
来源：http://wta.vehdjk.com

[U06] Py：合并两个字典
来源：http://ucd.jinqigfzy.top

{**a, **b}
来源：http://hoc.iojbl.cn

[U07] Py：反转字典键值
来源：http://qhn.jinqigufen.top

{v: k for k, v in d.items()}
来源：http://pup.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://zxq.nwbrower.top

[y for x in nested for y in x]
来源：http://cht.feifeiyinyue.top

[U09] Py：字典取最大值的键
来源：http://oqb.yongpay.top

max(d, key=d.get)
来源：http://kvo.tian-w.cn

[U10] Py：按值排序字典
来源：http://bob.birdmap.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fbp.0kj1m.cn

[U11] Py：生成器表达式
来源：http://law.gaohongyu789.top

(x * 2 for x in arr)
来源：http://njm.andypj.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://oqp.shangyingyoupin.top

Counter(arr).most_common(3)
来源：http://qcu.yueranfly.top

[U13] Py：固定长度队列
来源：http://tba.guowangkeji.top

deque(maxlen=10)
来源：http://vau.hywenlv.cn

[U14] Py：分组收集到列表
来源：http://jeq.xuanzx.com

defaultdict(list)
来源：http://yxs.fzhhl.top

[U15] Py：高精度计时
来源：http://enk.yangfankeji.com

t = time.perf_counter()
来源：http://qqv.wangshuangyany.cn

[U16] Py：命令行参数解析
来源：http://gta.pycfn.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uax.smart0.xyz

[U17] Py：初始化日志
来源：http://whi.mhx1999.top

logging.basicConfig(level=logging.INFO)
来源：http://qrn.xuetiantiany.cn

[U18] Py：预编译正则
来源：http://sur.bbcook.cn

pat = re.compile(r"\d+")
来源：http://gvg.birdmap.top

[U19] Py：正则替换带回调
来源：http://zyi.uphjek.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cpi.wangdashe.top

[U20] Py：缓存函数结果
来源：http://bwe.haohaochexian.top

@functools.lru_cache(maxsize=None)
来源：http://icb.hammf.cn

[U21] Py：自定义上下文管理器
来源：http://fgt.jlsjyb.cn

@contextlib.contextmanager
来源：http://rhc.jianghu66.top

[U22] Py：矩阵转置
来源：http://ara.shangyingyoupin.top

list(zip(*m))
来源：http://bmq.havefunace.top

[U23] Py：分块读取大文件
来源：http://erj.yvedp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fpu.kuanghao11.cn

[U24] Py：路径操作
来源：http://aur.9152youxi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fed.yuanzhike.top

[U25] Py：CSV 按字典读
来源：http://dsg.zhaomingkeji.xyz

csv.DictReader(f)
来源：http://yno.yueranfly.top

[U26] Py：并发下载
来源：http://llq.bbcook.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lfh.uphjek.com

[U27] Py：异步 HTTP
来源：http://rhp.nanxinkj.top

aiohttp.ClientSession() 配合 async with
来源：http://kxv.ybcxt.top

[U28] Py：类型别名
来源：http://aqd.meibo888.top

UserId = int
来源：http://lqm.zhixingplan.top

[U29] Py：属性校验
来源：http://qya.ywan-chungtsiang.top

@property 与 @x.setter 配合
来源：http://uqn.meibo888.top

[U30] Py：数据类
来源：http://zwb.tarul.cn

@dataclass(slots=True)
来源：http://qrh.zdqjudy.top

[U31] Py：单测
来源：http://xxm.sysykeji.top

python -m pytest -q
来源：http://zlv.shzxlz.cn

[U32] Py：代码格式化
来源：http://xic.chenjidiqi.icu

ruff format . && ruff check --fix .
来源：http://ykp.gogol.net.cn

[U33] Py：打包发布
来源：http://exi.yuanzhike.top

python -m build  （依赖 pyproject.toml）
来源：http://lep.sxryk.cn

[U34] Py：判断编码
来源：http://alu.ivvv.top

chardet.detect(raw)
来源：http://qms.tarul.cn

[U35] Py：发送邮件
来源：http://snj.yongpay.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://imb.gaohongyu789.top

[U36] Py：定时任务
来源：http://yun.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://qfg.ppjwa.cn

[U37] Py：读写 Excel
来源：http://yph.wangshuangyany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gex.jiagoushi.top

[U38] Py：获取脚本所在目录
来源：http://nli.0kj1m.cn

Path(__file__).resolve().parent
来源：http://tsb.ydzc1.top

[U39] Py：判断是否在交互环境
来源：http://nbe.wangdashe.top

sys.stdout.isatty()
来源：http://hvy.yuanzhike.top

[U40] Py：打印到标准错误
来源：http://vso.chenlongwang.top

print("err", file=sys.stderr)
来源：http://yeb.shuidangran.top

[U41] PHP：初始化 Composer 项目
来源：http://tnj.ppjwa.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://unt.quarkkingdee.top

[U42] PHP：PSR-4 自动加载
来源：http://pfx.uphjek.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sro.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://bci.chenlongwang.top

namespace App\Http;
来源：http://qym.sjlbkw.cn

[U44] PHP：开启严格类型
来源：http://nga.jqgufenzy.top

declare(strict_types=1);
来源：http://qbi.cdnleiting.top

[U45] PHP：类型声明与返回类型
来源：http://rcw.aibaodan.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bfv.bbcook.cn

[U46] PHP：可空类型
来源：http://gjr.ivvv.top

?string $name = null
来源：http://obm.mhx1999.top

[U47] PHP：联合类型
来源：http://wqb.yueranfly.top

int|string $id
来源：http://tuj.yvedp.cn

[U48] PHP：纯枚举
来源：http://egv.jinghuilouyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jsq.zdbjq.cn

[U49] PHP：只读属性
来源：http://blu.vqdsnc.cn

public readonly string $name
来源：http://leg.sxryk.cn

[U50] PHP：构造器属性提升
来源：http://nqk.svipenyu.cn

public function __construct(private int $id) {}
来源：http://eix.cucudq.cn

[U51] PHP：数组解构
来源：http://wtk.yuanzhike.top

[$a, $b] = $arr;
来源：http://rfm.xuetiantiany.cn

[U52] PHP：箭头函数
来源：http://gcg.cdnleiting.top

$double = fn($x) => $x * 2;
来源：http://hxa.zhoulong.xyz

[U53] PHP：空合并运算符
来源：http://zaj.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://hzp.daxiang520.top

[U54] PHP：空安全调用
来源：http://lqa.hcnkem.com

$obj?->method()
来源：http://zai.52xcode.cn

[U55] PHP：match 表达式
来源：http://dim.nanxinkj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://irs.wangshuangyany.cn

[U56] PHP：命名参数
来源：http://slc.tanke756.top

f(a: 1, b: 2)
来源：http://aii.vehdjk.com

[U57] PHP：字符串插值
来源：http://vxh.zhiwuduotai.top

"值: {$a}"
来源：http://qfb.shuidangran.top

[U58] PHP：数组三件套
来源：http://rls.shanyushiyangtech.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jzo.316326.xyz

[U59] PHP：自定义排序
来源：http://ycf.sxryk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://srs.pengpengdd.cyou

[U60] PHP：JSON 编解码
来源：http://zyu.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dxu.guowangkeji.top

[U61] PHP：正则
来源：http://ovt.ctjpmb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dhr.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://djg.zhongyouzk.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gcd.guowangkeji.top

[U63] PHP：文件读写
来源：http://fux.xinyue.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zdq.jinqigfzy.top

[U64] PHP：目录遍历
来源：http://icb.zhoulong.xyz

glob("dir/*.php");  scandir("dir");
来源：http://vqx.guowangkeji.top

[U65] PHP：会话
来源：http://pzz.yanxiufei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://war.pycfn.com

[U66] PHP：设置 Cookie
来源：http://ywf.zdqjudy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qhv.shuidangran.top

[U67] PHP：处理文件上传
来源：http://kcz.hammf.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sdk.yj20258888.top

[U68] PHP：PDO 连接
来源：http://sdf.yanxiufei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://slx.tian-w.cn

[U69] PHP：PDO 预处理
来源：http://oyf.smart0.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cqb.zhiwuduotai.top

[U70] PHP：PDO 事务
来源：http://yie.shzxlz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://shv.ydjk.org.cn

[U71] PHP：抛出异常
来源：http://fxa.ehwqpu.com

throw new RuntimeException("失败", 500);
来源：http://wkw.tianlin.xyz

[U72] PHP：写错误日志
来源：http://rbn.yanxiufei.cn

error_log("失败: " . $e->getMessage());
来源：http://yrh.zhoulong.xyz

[U73] PHP：读取 ini 配置
来源：http://hki.52xcode.cn

parse_ini_file("config.ini", true)
来源：http://sjr.hywenlv.cn

[U74] PHP：读取环境变量
来源：http://rfl.ivvv.top

getenv("APP_ENV") ?: "production"
来源：http://xqj.meibo888.top

[U75] PHP：依赖注入
来源：http://wbc.zhiwuduotai.top

composer require psr/container
来源：http://qaq.yongpay.top

[U76] PHP：简单路由
来源：http://yfd.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jmf.tarul.cn

[U77] PHP：模板渲染
来源：http://yyq.bbcook.cn

composer require twig/twig
来源：http://gjd.zhoulong.xyz

[U78] PHP：单元测试
来源：http://xqt.cucudq.cn

composer require --dev phpunit/phpunit
来源：http://zwh.zhongyouzk.top

[U79] PHP：静态分析
来源：http://vhf.yanxiufei.cn

composer require --dev phpstan/phpstan
来源：http://tzh.hfpthk.cn

[U80] PHP：代码规范修复
来源：http://ssx.shangyingyoupin.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://enl.nanxuanxn.top

[U81] JS：初始化项目
来源：http://jks.yj20258.top

npm init -y;  npm i express
来源：http://axm.jlsjyb.cn

[U82] JS：package.json 脚本
来源：http://mxq.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sap.aizwys.cn

[U83] JS：ES Module 导入导出
来源：http://qtu.fengsongda.top

export const a = 1;  import { a } from "./m.js";
来源：http://tpa.xingfuxueyuan.xyz

[U84] JS：CommonJS 写法
来源：http://dzb.nanxuanxn.top

module.exports = { a };  const { a } = require("./m");
来源：http://wic.meibo888.top

[U85] JS：可选链
来源：http://twg.yangfankeji.com

a?.b?.c
来源：http://obx.ybcxt.top

[U86] JS：空值合并
来源：http://nsc.feifeiyinyue.top

a ?? b
来源：http://stu.nwbrower.top

[U87] JS：解构默认值
来源：http://mmt.yuanzhike.top

const { a = 1, b = 2 } = obj;
来源：http://cbo.yuxming.cn

[U88] JS：对象展开合并
来源：http://tec.ivvv.top

{ ...a, ...b }
来源：http://kmb.zycfv.cn

[U89] JS：数组去重
来源：http://tdn.yonumen.top

[...new Set(arr)]
来源：http://hyy.mhx1999.top

[U90] JS：数字数组排序
来源：http://fsy.yfazqb.com

[...arr].sort((a, b) => a - b)
来源：http://hxs.ivvv.top

[U91] JS：对象键值遍历
来源：http://irg.c1oappe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ycj.hywenlv.cn

[U92] JS：深拷贝
来源：http://vci.yuanzhike.top

structuredClone(obj)
来源：http://ecp.jqgfzy.top

[U93] JS：模板字符串
来源：http://orn.hywenlv.cn

`共 ${n} 条`
来源：http://mus.hcnkem.com

[U94] JS：箭头函数
来源：http://haj.aibaodan.cn

const double = x => x * 2;
来源：http://yqh.aibaodan.cn

[U95] JS：Promise 包装
来源：http://byj.316326.xyz

new Promise((resolve, reject) => {})
来源：http://wqz.haohaochexian.top

[U96] JS：async/await 与异常
来源：http://kok.316326.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qhl.dashuyun.cn

[U97] JS：并发请求
来源：http://brw.dashuyun.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uyj.zycfv.cn

[U98] JS：fetch 带 JSON
来源：http://ypi.yangfankeji.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nbn.fzhhl.top

[U99] JS：事件监听
来源：http://xrr.nwbrower.top

el.addEventListener("click", e => {})
来源：http://sbe.meibo888.top

[U100] JS：DOM 查询
来源：http://ndb.hywenlv.cn

document.querySelector(".item")
来源：http://fdh.jqgfzy.top

[U101] JS：classList 操作
来源：http://wan.yangfankeji.com

el.classList.toggle("active")
来源：http://uti.jiagoushi.top

[U102] JS：本地存储
来源：http://zdb.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qiw.shangyingyoupin.top

[U103] JS：定时器
来源：http://hni.hnxiangtu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oqe.cucudq.cn

[U104] JS：防抖
来源：http://kzc.ydzc1.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tmi.andypj.xyz

[U105] JS：节流
来源：http://sgq.hammf.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://juy.ywan-chungtsiang.top

[U106] JS：日期格式化
来源：http://hzk.shanyushiyangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rjt.vqdsnc.cn

[U107] JS：数字千分位
来源：http://rof.xylfe.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zuv.yfazqb.com

[U108] JS：随机整数
来源：http://jwe.tianlin.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fej.zhijiandao.cn

[U109] JS：数组分组
来源：http://cxc.shuidangran.top

Object.groupBy(arr, x => x.type)
来源：http://bzw.hnxiangtu.top

[U110] JS：数组分块
来源：http://ymq.xylfe.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ten.ywan-chungtsiang.top

[U111] JS：对象转 Map
来源：http://sdr.havefunace.top

new Map(Object.entries(obj))
来源：http://hca.xuanzx.com

[U112] JS：字符串补位
来源：http://zga.jqgufenzy.top

"7".padStart(3, "0")
来源：http://bkj.yueranfly.top

[U113] JS：正则替换全部
来源：http://bvb.fktsv.cn

s.replaceAll("a", "b")
来源：http://dtu.snrcjt.cn

[U114] JS：JSON 深比较
来源：http://pyv.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://beu.pycfn.com

[U115] JS：生成 UUID
来源：http://rrg.yuxming.cn

crypto.randomUUID()
来源：http://mzc.yj202588.top

[U116] JS：类型检查（JSDoc）
来源：http://lvb.9152youxi.cn

/** @param {string} name */ function f(name) {}
来源：http://xfo.aizwys.cn

[U117] JS：单元测试
来源：http://mnm.yongpay.top

npm i -D vitest;  npx vitest
来源：http://per.hongshengwenyu.top

[U118] JS：开发服务器
来源：http://mdz.zhongyouzk.top

npm i -D vite;  npx vite
来源：http://ewj.feifeiyinyue.top

[U119] JS：生产构建
来源：http://xqe.fzhhl.top

npx vite build
来源：http://lou.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://yoe.hammf.cn

import.meta.env.VITE_API_URL
来源：http://yzs.nanxinkj.top

================================================================================
来源：http://ias.yongpay.top

统计汇总
来源：http://cnd.hongshengwenyu.top

================================================================================
来源：http://oau.zdqjudy.top

按语言统计（条）：
来源：http://eyw.kuanghao11.cn

Python ......... 252
来源：http://pqs.nanxinkj.top

PHP ............ 252
来源：http://iyv.jqgufenzy.top

JavaScript ..... 252
来源：http://hrs.shzxlz.cn

TypeScript ..... 212
来源：http://ipc.yangfankeji.com

Java ........... 212
来源：http://avg.ybcxt.top

Go ............. 212
来源：http://fxk.jlsjyb.cn

Ruby ........... 212
来源：http://xqi.fktsv.cn

C# ............. 212
来源：http://kfg.yuxming.cn

C .............. 30
来源：http://eol.316326.xyz

C++ ............ 30
来源：http://kjo.ydzc1.top

SQL ............ 90
来源：http://fwl.fengsongda.top

Bash ........... 80
来源：http://nit.yuxming.cn

Kotlin ......... 15
来源：http://qln.yuxming.cn

Swift .......... 15
来源：http://xjl.tian-w.cn

Lua ............ 10
来源：http://kau.nanxinkj.top

Perl ........... 10
来源：http://nrv.jinqigfzy.top

Scala .......... 10
来源：http://fci.gotoacloud.top

------------------------------------
来源：http://naw.ctjpmb.com

合计 ........... 2106 条
来源：http://kcr.zhixingplan.top

按章节统计：
来源：http://ngw.jiagoushi.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rjt.aibaodan.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gfq.ivvv.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zcd.cucudq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xio.tianlin.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://umv.zhengqikj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xsl.c1oappe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oou.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ltx.jlsjyb.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rxb.jianghu66.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jht.tian-w.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fxk.bjfxy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://clm.fengsongda.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fqc.ydjk.org.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cem.shangyingyoupin.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ric.tanke756.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rpn.redwolf501.top

Q SQL 专题                              90
来源：http://xpn.kuanghao11.cn

R Bash 专题                             80
来源：http://uzz.ctjpmb.com

S C / C++ 专题                          60
来源：http://zlj.tarul.cn

T 其他语言补充                          60
来源：http://tew.ctjpmb.com

U 高频实用片段                         120
来源：http://aeh.hysaishi.cn

------------------------------------
来源：http://eca.yuanzhike.top

合计                                  2106 条
来源：http://tzp.sysykeji.top

--------------------------------------------------------------------------------
来源：http://cuk.hammf.cn

使用提醒
来源：http://atr.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://lso.dianchejie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sxj.9152youxi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fvc.jianghu66.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vat.yuanzhike.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lzr.jqgufenzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tlt.jyoumei.cn

—— 文件结束 ——
来源：http://det.daxiang520.top

================================================================================
来源：http://rvs.yj20258.top

程序语言常见例子速查手册（2024 版）
来源：http://yoz.sxryk.cn

Common Programming Examples Cheat Book
来源：http://nln.xuanzx.com

================================================================================
来源：http://wda.meibo888.top

【收录内容】
来源：http://xrh.chenzaomai.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://kjz.zhiwuduotai.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vqm.xingfuxueyuan.xyz

SQL · Bash · C · C++
来源：http://sem.zhengqikj.top


<!-- 参考信息 -->