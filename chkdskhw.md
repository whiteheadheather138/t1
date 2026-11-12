代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://zfr.jqgufenzy.top

[T55] Scala：集合过滤
来源：http://cdj.jyoumei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://udd.hnxiangtu.top

[T56] Scala：样例类
来源：http://bob.yfazqb.com

case class User(name: String, age: Int)
来源：http://vgk.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://hhc.0kj1m.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qfj.dashuyun.cn

[T58] Scala：函数定义
来源：http://hbe.zhaomingkeji.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://ohn.jiagoushi.top

[T59] Scala：循环
来源：http://hdl.shanyushiyangtech.top

for (i <- 1 to 10) println(i)
来源：http://uwy.yanxiufei.cn

[T60] Scala：折叠
来源：http://eko.redwolf501.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iqs.nwbrower.top

================================================================================
来源：http://ato.xuetiantiany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qqz.guannengcc.top

================================================================================
来源：http://etj.52xcode.cn

[U01] Py：创建虚拟环境
来源：http://myd.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lpf.sufxvd.cn

[U02] Py：导出 / 安装依赖
来源：http://wyg.redwolf501.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ndw.9152youxi.cn

[U03] Py：加载 .env 配置
来源：http://rgu.jyoumei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xse.ydjk.org.cn

[U04] Py：变量调试打印
来源：http://mog.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lrp.yj20258.top

[U05] Py：列表去重且保序
来源：http://qls.shzxlz.cn

list(dict.fromkeys(arr))
来源：http://pip.meibo888.top

[U06] Py：合并两个字典
来源：http://ltx.jinqigufen.top

{**a, **b}
来源：http://qkx.ybcxt.top

[U07] Py：反转字典键值
来源：http://ibt.ppjwa.cn

{v: k for k, v in d.items()}
来源：http://qsz.fktsv.cn

[U08] Py：展平二维列表
来源：http://fuf.gogol.net.cn

[y for x in nested for y in x]
来源：http://bbl.snrcjt.cn

[U09] Py：字典取最大值的键
来源：http://max.nanxuanxn.top

max(d, key=d.get)
来源：http://hds.ppjwa.cn

[U10] Py：按值排序字典
来源：http://nuy.zhaomingkeji.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://flw.tarul.cn

[U11] Py：生成器表达式
来源：http://sbm.svipenyu.cn

(x * 2 for x in arr)
来源：http://qbb.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://zvb.zhongyouzk.top

Counter(arr).most_common(3)
来源：http://hwj.zhijiandao.cn

[U13] Py：固定长度队列
来源：http://zer.meibo888.top

deque(maxlen=10)
来源：http://oya.hywenlv.cn

[U14] Py：分组收集到列表
来源：http://blg.ehwqpu.com

defaultdict(list)
来源：http://tku.sysykeji.top

[U15] Py：高精度计时
来源：http://xse.shanyushiyangtech.top

t = time.perf_counter()
来源：http://dbz.guowangkeji.top

[U16] Py：命令行参数解析
来源：http://tlw.fengsongda.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cot.xziqi.cn

[U17] Py：初始化日志
来源：http://qtq.epnwcf.com

logging.basicConfig(level=logging.INFO)
来源：http://lsu.yj20258.top

[U18] Py：预编译正则
来源：http://mcj.chenlongwang.top

pat = re.compile(r"\d+")
来源：http://dta.jinqigufen.top

[U19] Py：正则替换带回调
来源：http://asf.0kj1m.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://not.fktsv.cn

[U20] Py：缓存函数结果
来源：http://iue.yuxming.cn

@functools.lru_cache(maxsize=None)
来源：http://eqv.wangdashe.top

[U21] Py：自定义上下文管理器
来源：http://moc.cucudq.cn

@contextlib.contextmanager
来源：http://ojk.shanyushiyangkeji.top

[U22] Py：矩阵转置
来源：http://jdk.ybcxt.top

list(zip(*m))
来源：http://adp.wangdashe.top

[U23] Py：分块读取大文件
来源：http://kfv.dashuyun.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://djk.xingfuxueyuan.xyz

[U24] Py：路径操作
来源：http://wsw.nwbrower.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kde.guowangkeji.top

[U25] Py：CSV 按字典读
来源：http://ugr.zhoulong.xyz

csv.DictReader(f)
来源：http://xsk.chenzaomai.com

[U26] Py：并发下载
来源：http://zpo.zhijiandao.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://icq.xuanzx.com

[U27] Py：异步 HTTP
来源：http://mrv.aizwys.cn

aiohttp.ClientSession() 配合 async with
来源：http://ksy.zhongyouzk.top

[U28] Py：类型别名
来源：http://ivg.gzhubu.top

UserId = int
来源：http://rhb.hnxiangtu.top

[U29] Py：属性校验
来源：http://ybl.jinqigufen.top

@property 与 @x.setter 配合
来源：http://aeh.gaohongyu789.top

[U30] Py：数据类
来源：http://wbg.ctjpmb.com

@dataclass(slots=True)
来源：http://ntp.gzhubu.top

[U31] Py：单测
来源：http://vrr.meibo888.top

python -m pytest -q
来源：http://sfd.jqgufenzy.top

[U32] Py：代码格式化
来源：http://xnh.feifeiyinyue.top

ruff format . && ruff check --fix .
来源：http://rjr.uphjek.com

[U33] Py：打包发布
来源：http://vtv.cashguo.top

python -m build  （依赖 pyproject.toml）
来源：http://eoe.yj20258888.top

[U34] Py：判断编码
来源：http://wef.nwbrower.top

chardet.detect(raw)
来源：http://aqf.daxiang520.top

[U35] Py：发送邮件
来源：http://lfu.wangshuangyany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mbg.shanyushiyangtech.top

[U36] Py：定时任务
来源：http://ijh.hcnkem.com

schedule.every(10).minutes.do(job)
来源：http://qze.hcnkem.com

[U37] Py：读写 Excel
来源：http://clm.aibaodan.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qcg.yfazqb.com

[U38] Py：获取脚本所在目录
来源：http://ear.jianghu66.top

Path(__file__).resolve().parent
来源：http://knk.hesvh.cn

[U39] Py：判断是否在交互环境
来源：http://pfu.jyoumei.cn

sys.stdout.isatty()
来源：http://leq.cashguo.top

[U40] Py：打印到标准错误
来源：http://tez.jqgufenzy.top

print("err", file=sys.stderr)
来源：http://sxg.feifeiyinyue.top

[U41] PHP：初始化 Composer 项目
来源：http://ypt.sysykeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://exg.nanxinkj.top

[U42] PHP：PSR-4 自动加载
来源：http://ncq.cdnleiting.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uyd.yongpay.top

[U43] PHP：声明命名空间
来源：http://hug.chenzaomai.com

namespace App\Http;
来源：http://pba.shanyushiyangtech.top

[U44] PHP：开启严格类型
来源：http://jrk.52xcode.cn

declare(strict_types=1);
来源：http://zdz.daria6918.cn

[U45] PHP：类型声明与返回类型
来源：http://fll.zdbjq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ole.yj20258.top

[U46] PHP：可空类型
来源：http://fbn.guannengcc.top

?string $name = null
来源：http://wrh.meibo888.top

[U47] PHP：联合类型
来源：http://ofr.gzhubu.top

int|string $id
来源：http://ola.havefunace.top

[U48] PHP：纯枚举
来源：http://ezz.chenzaomai.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mek.tanke756.top

[U49] PHP：只读属性
来源：http://pzd.hcnkem.com

public readonly string $name
来源：http://czr.zhongyouzk.top

[U50] PHP：构造器属性提升
来源：http://rhi.daria6918.cn

public function __construct(private int $id) {}
来源：http://qnl.cheryme.top

[U51] PHP：数组解构
来源：http://cov.ehwqpu.com

[$a, $b] = $arr;
来源：http://ksn.zhijiandao.cn

[U52] PHP：箭头函数
来源：http://dhb.aibaodan.cn

$double = fn($x) => $x * 2;
来源：http://sbc.hnqzz.top

[U53] PHP：空合并运算符
来源：http://jcn.hongshengwenyu.top

$v = $a ?? $b ?? "default";
来源：http://hli.yfazqb.com

[U54] PHP：空安全调用
来源：http://yoc.wangshuangyany.cn

$obj?->method()
来源：http://bjn.0kj1m.cn

[U55] PHP：match 表达式
来源：http://jzn.zhijiandao.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rql.hywenlv.cn

[U56] PHP：命名参数
来源：http://mnv.fanxiaobao.xyz

f(a: 1, b: 2)
来源：http://chh.guannengcc.top

[U57] PHP：字符串插值
来源：http://wme.shangyingyoupin.top

"值: {$a}"
来源：http://aww.nanxinkj.top

[U58] PHP：数组三件套
来源：http://uyo.hongshengwenyu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rwr.zhaomingkeji.xyz

[U59] PHP：自定义排序
来源：http://zij.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gjs.yj20258.top

[U60] PHP：JSON 编解码
来源：http://gfw.wangshuangyany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rek.pengpengdd.cyou

[U61] PHP：正则
来源：http://zay.gzhubu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://weo.ivvv.top

[U62] PHP：日期对象
来源：http://jjc.yueranfly.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hju.ydzc1.top

[U63] PHP：文件读写
来源：http://rff.pengpengdd.cyou

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xsm.wangshuangyany.cn

[U64] PHP：目录遍历
来源：http://rkz.chenjidiqi.icu

glob("dir/*.php");  scandir("dir");
来源：http://qwt.ctjpmb.com

[U65] PHP：会话
来源：http://ryh.sysykeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://llu.feifeiyinyue.top

[U66] PHP：设置 Cookie
来源：http://phi.pycfn.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sbp.jianghu66.top

[U67] PHP：处理文件上传
来源：http://wyf.bbcook.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rha.sweek.top

[U68] PHP：PDO 连接
来源：http://btt.cheryme.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zbu.yongpay.top

[U69] PHP：PDO 预处理
来源：http://ody.c1oappe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tqq.xziqi.cn

[U70] PHP：PDO 事务
来源：http://hjn.chenjidiqi.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wpj.xylfe.cn

[U71] PHP：抛出异常
来源：http://bnp.gogol.net.cn

throw new RuntimeException("失败", 500);
来源：http://aek.hnxiangtu.top

[U72] PHP：写错误日志
来源：http://jok.cashguo.top

error_log("失败: " . $e->getMessage());
来源：http://lao.yanxiufei.cn

[U73] PHP：读取 ini 配置
来源：http://vxu.yj202588.top

parse_ini_file("config.ini", true)
来源：http://giu.cheryme.top

[U74] PHP：读取环境变量
来源：http://mut.tian-w.cn

getenv("APP_ENV") ?: "production"
来源：http://eaa.0kj1m.cn

[U75] PHP：依赖注入
来源：http://jkf.meibo888.top

composer require psr/container
来源：http://dyp.316326.xyz

[U76] PHP：简单路由
来源：http://hua.andypj.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kya.gaohongyu789.top

[U77] PHP：模板渲染
来源：http://mui.mhx1999.top

composer require twig/twig
来源：http://ywc.jinyuanbaomall.cn

[U78] PHP：单元测试
来源：http://jwx.wangshuangyany.cn

composer require --dev phpunit/phpunit
来源：http://old.yueranfly.top

[U79] PHP：静态分析
来源：http://xfs.yvedp.cn

composer require --dev phpstan/phpstan
来源：http://xjw.pengpengdd.cyou

[U80] PHP：代码规范修复
来源：http://uyz.xziqi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ktx.gzhubu.top

[U81] JS：初始化项目
来源：http://nfx.ydzc1.top

npm init -y;  npm i express
来源：http://tmi.fktsv.cn

[U82] JS：package.json 脚本
来源：http://vvb.xziqi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://loi.ywan-chungtsiang.top

[U83] JS：ES Module 导入导出
来源：http://guc.xuanzx.com

export const a = 1;  import { a } from "./m.js";
来源：http://tsc.jinqigfzy.top

[U84] JS：CommonJS 写法
来源：http://jns.aizwys.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kue.nanxinkj.top

[U85] JS：可选链
来源：http://zmn.aizwys.cn

a?.b?.c
来源：http://xhh.chenjidiqi.icu

[U86] JS：空值合并
来源：http://udw.hfpthk.cn

a ?? b
来源：http://nbk.haohaochexian.top

[U87] JS：解构默认值
来源：http://dbw.shzxlz.cn

const { a = 1, b = 2 } = obj;
来源：http://vwc.hysaishi.cn

[U88] JS：对象展开合并
来源：http://zjf.shanyushiyangkeji.top

{ ...a, ...b }
来源：http://xqz.zdbjq.cn

[U89] JS：数组去重
来源：http://cuc.xylfe.cn

[...new Set(arr)]
来源：http://uvo.guannengcc.top

[U90] JS：数字数组排序
来源：http://rbx.jlsjyb.cn

[...arr].sort((a, b) => a - b)
来源：http://vlu.sysykeji.top

[U91] JS：对象键值遍历
来源：http://tst.ctjpmb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gay.yj202588.top

[U92] JS：深拷贝
来源：http://bto.cqqwz.cn

structuredClone(obj)
来源：http://prh.yj202588.top

[U93] JS：模板字符串
来源：http://kzj.vqdsnc.cn

`共 ${n} 条`
来源：http://pri.hfpthk.cn

[U94] JS：箭头函数
来源：http://xen.xinyue.icu

const double = x => x * 2;
来源：http://lpa.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://ggs.fehbvm.com

new Promise((resolve, reject) => {})
来源：http://lox.sufxvd.cn

[U96] JS：async/await 与异常
来源：http://vtw.hnqzz.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://diw.zhiwuduotai.top

[U97] JS：并发请求
来源：http://qbw.hnqzz.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ypa.hammf.cn

[U98] JS：fetch 带 JSON
来源：http://sqy.smart0.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cqk.zdbjq.cn

[U99] JS：事件监听
来源：http://yyw.yueranfly.top

el.addEventListener("click", e => {})
来源：http://pfh.sysykeji.top

[U100] JS：DOM 查询
来源：http://arn.hfpthk.cn

document.querySelector(".item")
来源：http://uvf.jiagoushi.top

[U101] JS：classList 操作
来源：http://xdh.9152youxi.cn

el.classList.toggle("active")
来源：http://cht.tanke756.top

[U102] JS：本地存储
来源：http://stg.cheryme.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tqd.shzxlz.cn

[U103] JS：定时器
来源：http://lpl.daxiang520.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rqe.jinqigufen.top

[U104] JS：防抖
来源：http://cxy.yfazqb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://njy.gogol.net.cn

[U105] JS：节流
来源：http://xgy.yonumen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jhy.sweek.top

[U106] JS：日期格式化
来源：http://fhr.cqqwz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qme.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://zep.cdnleiting.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ygn.jiagoushi.top

[U108] JS：随机整数
来源：http://lol.wangshuangyany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qmb.ydzc1.top

[U109] JS：数组分组
来源：http://bad.aibaodan.cn

Object.groupBy(arr, x => x.type)
来源：http://kyw.guowangkeji.top

[U110] JS：数组分块
来源：http://ibi.ydzc1.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vpe.yuanzhike.top

[U111] JS：对象转 Map
来源：http://cow.xinyue.icu

new Map(Object.entries(obj))
来源：http://akt.zycfv.cn

[U112] JS：字符串补位
来源：http://epi.sxryk.cn

"7".padStart(3, "0")
来源：http://skf.sufxvd.cn

[U113] JS：正则替换全部
来源：http://awd.svipenyu.cn

s.replaceAll("a", "b")
来源：http://spv.xylfe.cn

[U114] JS：JSON 深比较
来源：http://sdm.yj20258888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://mzj.kuanghao11.cn

[U115] JS：生成 UUID
来源：http://bzz.hywenlv.cn

crypto.randomUUID()
来源：http://jys.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://tgq.fengsongda.top

/** @param {string} name */ function f(name) {}
来源：http://kay.tian-w.cn

[U117] JS：单元测试
来源：http://rtv.gogol.net.cn

npm i -D vitest;  npx vitest
来源：http://hdk.shuidangran.top

[U118] JS：开发服务器
来源：http://rnp.yj20258888.top

npm i -D vite;  npx vite
来源：http://ftr.chenlongwang.top

[U119] JS：生产构建
来源：http://dut.cucudq.cn

npx vite build
来源：http://sar.andypj.xyz

[U120] JS：读取环境变量（Vite）
来源：http://fpl.shangyingyoupin.top

import.meta.env.VITE_API_URL
来源：http://lif.yangfankeji.com

================================================================================
来源：http://wxo.sweek.top

统计汇总
来源：http://ngl.cqqwz.cn

================================================================================
来源：http://lqj.0kj1m.cn

按语言统计（条）：
来源：http://fxx.fktsv.cn

Python ......... 252
来源：http://zhp.dianchejie.cn

PHP ............ 252
来源：http://ekx.yfazqb.com

JavaScript ..... 252
来源：http://oqp.feifeiyinyue.top

TypeScript ..... 212
来源：http://rtc.tianlin.xyz

Java ........... 212
来源：http://gfd.gotoacloud.top

Go ............. 212
来源：http://xnx.zhixingplan.top

Ruby ........... 212
来源：http://psh.hongshengwenyu.top

C# ............. 212
来源：http://zva.vehdjk.com

C .............. 30
来源：http://nsl.aizwys.cn

C++ ............ 30
来源：http://gah.redwolf501.top

SQL ............ 90
来源：http://whk.yongpay.top

Bash ........... 80
来源：http://llu.mhx1999.top

Kotlin ......... 15
来源：http://djz.uphjek.com

Swift .......... 15
来源：http://jbk.xinyue.icu

Lua ............ 10
来源：http://blj.sufxvd.cn

Perl ........... 10
来源：http://nsd.zhixingplan.top

Scala .......... 10
来源：http://zji.wangshuangyany.cn

------------------------------------
来源：http://zav.kuanghao11.cn

合计 ........... 2106 条
来源：http://eue.fengsongda.top

按章节统计：
来源：http://vgf.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qki.pycfn.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://flk.316326.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kct.zhiwuduotai.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jos.cqqwz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nvd.zhoulong.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pxf.nanxinkj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jmk.xuanzx.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cfe.zhongyouzk.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ydn.jinqigufen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zsw.9152youxi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yuh.haohaochexian.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ybi.hongshengwenyu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rld.ehwqpu.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kma.guowangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ftj.fengsongda.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mgy.cdnleiting.top

Q SQL 专题                              90
来源：http://omr.gotoacloud.top

R Bash 专题                             80
来源：http://uin.aibaodan.cn

S C / C++ 专题                          60
来源：http://vfx.gzhubu.top

T 其他语言补充                          60
来源：http://ihl.daria6918.cn


<!-- 参考信息 -->