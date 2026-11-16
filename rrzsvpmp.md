代发 wailian999

[U03] Py：加载 .env 配置
来源：http://ghp.zhengqikj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ayj.xziqi.cn

[U04] Py：变量调试打印
来源：http://lxv.yj202588.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://icq.cdnleiting.top

[U05] Py：列表去重且保序
来源：http://uis.yueranfly.top

list(dict.fromkeys(arr))
来源：http://dfd.birdmap.top

[U06] Py：合并两个字典
来源：http://zsh.zhengqikj.top

{**a, **b}
来源：http://fds.yongpay.top

[U07] Py：反转字典键值
来源：http://grz.shangyingyoupin.top

{v: k for k, v in d.items()}
来源：http://zlw.xuanzx.com

[U08] Py：展平二维列表
来源：http://tld.ydjk.org.cn

[y for x in nested for y in x]
来源：http://gpm.bbcook.cn

[U09] Py：字典取最大值的键
来源：http://eno.uphjek.com

max(d, key=d.get)
来源：http://sna.ehwqpu.com

[U10] Py：按值排序字典
来源：http://qak.vqdsnc.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://suy.fktsv.cn

[U11] Py：生成器表达式
来源：http://bfk.wangdashe.top

(x * 2 for x in arr)
来源：http://nmc.hesvh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mvq.shuidangran.top

Counter(arr).most_common(3)
来源：http://ohe.xuanzx.com

[U13] Py：固定长度队列
来源：http://xqf.daxiang520.top

deque(maxlen=10)
来源：http://jyw.zhongyouzk.top

[U14] Py：分组收集到列表
来源：http://hyg.cqqwz.cn

defaultdict(list)
来源：http://sel.fktsv.cn

[U15] Py：高精度计时
来源：http://goc.zhoulong.xyz

t = time.perf_counter()
来源：http://cmm.iojbl.cn

[U16] Py：命令行参数解析
来源：http://tob.xuetiantiany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vad.zhixingplan.top

[U17] Py：初始化日志
来源：http://bhe.hcnkem.com

logging.basicConfig(level=logging.INFO)
来源：http://ixi.shangyingyoupin.top

[U18] Py：预编译正则
来源：http://scs.zhijiandao.cn

pat = re.compile(r"\d+")
来源：http://qfw.guannengcc.top

[U19] Py：正则替换带回调
来源：http://kfx.yj202588.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zki.wangshuangyany.cn

[U20] Py：缓存函数结果
来源：http://ghl.hcnkem.com

@functools.lru_cache(maxsize=None)
来源：http://vnc.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://dll.jianghu66.top

@contextlib.contextmanager
来源：http://rdy.ehwqpu.com

[U22] Py：矩阵转置
来源：http://uih.xinyue.icu

list(zip(*m))
来源：http://uta.redwolf501.top

[U23] Py：分块读取大文件
来源：http://xkt.bbcook.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qvj.vehdjk.com

[U24] Py：路径操作
来源：http://uuy.yuxming.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jjc.sufxvd.cn

[U25] Py：CSV 按字典读
来源：http://bel.shzxlz.cn

csv.DictReader(f)
来源：http://trr.ydzc1.top

[U26] Py：并发下载
来源：http://ewx.xylfe.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://htm.zdbjq.cn

[U27] Py：异步 HTTP
来源：http://fkh.gzhubu.top

aiohttp.ClientSession() 配合 async with
来源：http://ogu.vqdsnc.cn

[U28] Py：类型别名
来源：http://opr.zycfv.cn

UserId = int
来源：http://jfu.yj20258888.top

[U29] Py：属性校验
来源：http://ykf.gzhubu.top

@property 与 @x.setter 配合
来源：http://tzd.shzxlz.cn

[U30] Py：数据类
来源：http://dew.9152youxi.cn

@dataclass(slots=True)
来源：http://jde.pengpengdd.cyou

[U31] Py：单测
来源：http://yjy.zhengqikj.top

python -m pytest -q
来源：http://cew.shzxlz.cn

[U32] Py：代码格式化
来源：http://ndt.sufxvd.cn

ruff format . && ruff check --fix .
来源：http://vwt.ctjpmb.com

[U33] Py：打包发布
来源：http://vcz.ydjk.org.cn

python -m build  （依赖 pyproject.toml）
来源：http://yml.jinqigufen.top

[U34] Py：判断编码
来源：http://djf.sxryk.cn

chardet.detect(raw)
来源：http://eus.hnxiangtu.top

[U35] Py：发送邮件
来源：http://akc.ydzc1.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dns.yueranfly.top

[U36] Py：定时任务
来源：http://vhx.sufxvd.cn

schedule.every(10).minutes.do(job)
来源：http://cvo.shanyushiyangkeji.top

[U37] Py：读写 Excel
来源：http://evl.daxiang520.top

pandas.read_excel / DataFrame.to_excel
来源：http://tjn.tanke756.top

[U38] Py：获取脚本所在目录
来源：http://dkv.zdqjudy.top

Path(__file__).resolve().parent
来源：http://utr.316326.xyz

[U39] Py：判断是否在交互环境
来源：http://hzm.zhoulong.xyz

sys.stdout.isatty()
来源：http://dsg.shuidangran.top

[U40] Py：打印到标准错误
来源：http://mln.aizwys.cn

print("err", file=sys.stderr)
来源：http://stn.zhixingplan.top

[U41] PHP：初始化 Composer 项目
来源：http://zvb.nanxinkj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wyw.sxryk.cn

[U42] PHP：PSR-4 自动加载
来源：http://jiz.bbcook.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ztm.hcnkem.com

[U43] PHP：声明命名空间
来源：http://gug.jinqigfzy.top

namespace App\Http;
来源：http://kkf.daria6918.cn

[U44] PHP：开启严格类型
来源：http://ukq.fktsv.cn

declare(strict_types=1);
来源：http://gyr.sxryk.cn

[U45] PHP：类型声明与返回类型
来源：http://ror.tian-w.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vpe.zdbjq.cn

[U46] PHP：可空类型
来源：http://azo.redwolf501.top

?string $name = null
来源：http://daa.feifeiyinyue.top

[U47] PHP：联合类型
来源：http://vgv.fzhhl.top

int|string $id
来源：http://afg.fanxiaobao.xyz

[U48] PHP：纯枚举
来源：http://tad.xuetiantiany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://akq.zhoulong.xyz

[U49] PHP：只读属性
来源：http://jed.ywan-chungtsiang.top

public readonly string $name
来源：http://zgr.tarul.cn

[U50] PHP：构造器属性提升
来源：http://jmy.yj202588.top

public function __construct(private int $id) {}
来源：http://kmy.yj20258888.top

[U51] PHP：数组解构
来源：http://hmr.cucudq.cn

[$a, $b] = $arr;
来源：http://his.zhengqikj.top

[U52] PHP：箭头函数
来源：http://jpi.jqgufenzy.top

$double = fn($x) => $x * 2;
来源：http://yog.svipenyu.cn

[U53] PHP：空合并运算符
来源：http://uvc.cdnleiting.top

$v = $a ?? $b ?? "default";
来源：http://bjr.yuxming.cn

[U54] PHP：空安全调用
来源：http://iht.sysykeji.top

$obj?->method()
来源：http://mmt.pengpengdd.cyou

[U55] PHP：match 表达式
来源：http://xyu.bjfxy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dog.vqdsnc.cn

[U56] PHP：命名参数
来源：http://gqt.sjlbkw.cn

f(a: 1, b: 2)
来源：http://xiz.zdbjq.cn

[U57] PHP：字符串插值
来源：http://bes.cucudq.cn

"值: {$a}"
来源：http://unl.nanxuanxn.top

[U58] PHP：数组三件套
来源：http://brd.vqdsnc.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ebn.hammf.cn

[U59] PHP：自定义排序
来源：http://sbg.hnqzz.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dlt.yonumen.top

[U60] PHP：JSON 编解码
来源：http://gxs.nanxuanxn.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kyc.yj20258888.top

[U61] PHP：正则
来源：http://kmt.yueranfly.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://obu.sufxvd.cn

[U62] PHP：日期对象
来源：http://aii.yongpay.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sfj.hesvh.cn

[U63] PHP：文件读写
来源：http://hpg.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aja.meibo888.top

[U64] PHP：目录遍历
来源：http://nup.zdbjq.cn

glob("dir/*.php");  scandir("dir");
来源：http://hpg.yj20258888.top

[U65] PHP：会话
来源：http://nwp.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kim.dashuyun.cn

[U66] PHP：设置 Cookie
来源：http://kas.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fje.ctjpmb.com

[U67] PHP：处理文件上传
来源：http://lpd.dianchejie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hjx.fengsongda.top

[U68] PHP：PDO 连接
来源：http://qic.shanyushiyangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://epu.c1oappe.top

[U69] PHP：PDO 预处理
来源：http://vgn.chenzaomai.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vhe.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://acd.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vpf.cashguo.top

[U71] PHP：抛出异常
来源：http://zpb.bbcook.cn

throw new RuntimeException("失败", 500);
来源：http://mrg.pengpengdd.cyou

[U72] PHP：写错误日志
来源：http://nph.feifeiyinyue.top

error_log("失败: " . $e->getMessage());
来源：http://aou.iojbl.cn

[U73] PHP：读取 ini 配置
来源：http://bvd.sjlbkw.cn

parse_ini_file("config.ini", true)
来源：http://ofw.cucudq.cn

[U74] PHP：读取环境变量
来源：http://enr.zhixingplan.top

getenv("APP_ENV") ?: "production"
来源：http://xjq.ywan-chungtsiang.top

[U75] PHP：依赖注入
来源：http://snx.tanke756.top

composer require psr/container
来源：http://dww.aizwys.cn

[U76] PHP：简单路由
来源：http://red.guannengcc.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kvt.redwolf501.top

[U77] PHP：模板渲染
来源：http://jlj.wangshuangyany.cn

composer require twig/twig
来源：http://kjs.zhijiandao.cn

[U78] PHP：单元测试
来源：http://vxa.guannengcc.top

composer require --dev phpunit/phpunit
来源：http://ycp.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://seu.vqdsnc.cn

composer require --dev phpstan/phpstan
来源：http://fhs.snrcjt.cn

[U80] PHP：代码规范修复
来源：http://plf.redwolf501.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://blz.jinghuilouyu.cn

[U81] JS：初始化项目
来源：http://obf.iojbl.cn

npm init -y;  npm i express
来源：http://owp.aizwys.cn

[U82] JS：package.json 脚本
来源：http://afr.nanxuanxn.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://idv.ywan-chungtsiang.top

[U83] JS：ES Module 导入导出
来源：http://mqv.zycfv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hxf.quarkkingdee.top

[U84] JS：CommonJS 写法
来源：http://ofo.chenlongwang.top

module.exports = { a };  const { a } = require("./m");
来源：http://ddi.yvedp.cn

[U85] JS：可选链
来源：http://wtw.zdqjudy.top

a?.b?.c
来源：http://zwj.yonumen.top

[U86] JS：空值合并
来源：http://zuj.zhengqikj.top

a ?? b
来源：http://hcl.yongpay.top

[U87] JS：解构默认值
来源：http://qpy.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://khn.jinyuanbaomall.cn

[U88] JS：对象展开合并
来源：http://fqd.jqgufenzy.top

{ ...a, ...b }
来源：http://eja.redwolf501.top

[U89] JS：数组去重
来源：http://fyo.quarkkingdee.top

[...new Set(arr)]
来源：http://mst.zhiwuduotai.top

[U90] JS：数字数组排序
来源：http://zkv.uphjek.com

[...arr].sort((a, b) => a - b)
来源：http://stx.fehbvm.com

[U91] JS：对象键值遍历
来源：http://pwb.cheryme.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bkm.zhaomingkeji.xyz

[U92] JS：深拷贝
来源：http://hae.jyoumei.cn

structuredClone(obj)
来源：http://ufu.epnwcf.com

[U93] JS：模板字符串
来源：http://rza.jlsjyb.cn

`共 ${n} 条`
来源：http://wht.smart0.xyz

[U94] JS：箭头函数
来源：http://zhc.sxryk.cn

const double = x => x * 2;
来源：http://gwt.shanyushiyangkeji.top

[U95] JS：Promise 包装
来源：http://tyy.jqgfzy.top

new Promise((resolve, reject) => {})
来源：http://nqk.pengpengdd.cyou

[U96] JS：async/await 与异常
来源：http://lrd.fktsv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ubu.jinqigfzy.top

[U97] JS：并发请求
来源：http://dbc.havefunace.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://flm.nanxuanxn.top

[U98] JS：fetch 带 JSON
来源：http://qmx.fanxiaobao.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pde.yanxiufei.cn

[U99] JS：事件监听
来源：http://num.yj20258.top

el.addEventListener("click", e => {})
来源：http://tui.gzhubu.top

[U100] JS：DOM 查询
来源：http://oxl.sweek.top

document.querySelector(".item")
来源：http://oaf.cdnleiting.top

[U101] JS：classList 操作
来源：http://zkb.yanxiufei.cn

el.classList.toggle("active")
来源：http://bhr.jinghuilouyu.cn

[U102] JS：本地存储
来源：http://gec.0kj1m.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uji.gzhubu.top

[U103] JS：定时器
来源：http://afb.tanke756.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rcz.hysaishi.cn

[U104] JS：防抖
来源：http://tdr.birdmap.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eyx.yangfankeji.com

[U105] JS：节流
来源：http://fyv.hnqzz.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vwx.yj20258888.top

[U106] JS：日期格式化
来源：http://rec.bbcook.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ouq.ybcxt.top

[U107] JS：数字千分位
来源：http://rvm.quarkkingdee.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dnj.shangyingyoupin.top

[U108] JS：随机整数
来源：http://awb.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://crv.meibo888.top

[U109] JS：数组分组
来源：http://uis.xinyue.icu

Object.groupBy(arr, x => x.type)
来源：http://wiq.sufxvd.cn

[U110] JS：数组分块
来源：http://zdv.yuxming.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kby.zdbjq.cn

[U111] JS：对象转 Map
来源：http://ppy.hnqzz.top

new Map(Object.entries(obj))
来源：http://gja.pengpengdd.cyou

[U112] JS：字符串补位
来源：http://spj.gzhubu.top

"7".padStart(3, "0")
来源：http://ihe.cqqwz.cn

[U113] JS：正则替换全部
来源：http://wzs.guannengcc.top

s.replaceAll("a", "b")
来源：http://fny.xinyue.icu

[U114] JS：JSON 深比较
来源：http://tut.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://mwi.hnxiangtu.top

[U115] JS：生成 UUID
来源：http://qzj.chenlongwang.top

crypto.randomUUID()
来源：http://wog.aizwys.cn

[U116] JS：类型检查（JSDoc）
来源：http://yuu.snrcjt.cn

/** @param {string} name */ function f(name) {}
来源：http://ses.hnxiangtu.top

[U117] JS：单元测试
来源：http://xwx.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://mqj.316326.xyz

[U118] JS：开发服务器
来源：http://fcv.epnwcf.com

npm i -D vite;  npx vite
来源：http://inw.quarkkingdee.top

[U119] JS：生产构建
来源：http://lzw.xziqi.cn

npx vite build
来源：http://vvc.tarul.cn

[U120] JS：读取环境变量（Vite）
来源：http://vca.xingfuxueyuan.xyz

import.meta.env.VITE_API_URL
来源：http://iud.gogol.net.cn

================================================================================
来源：http://wfa.gaohongyu789.top

统计汇总
来源：http://mkd.0kj1m.cn

================================================================================
来源：http://qjt.tarul.cn

按语言统计（条）：
来源：http://kzo.yj20258888.top

Python ......... 252
来源：http://azz.sweek.top

PHP ............ 252
来源：http://ybp.vehdjk.com

JavaScript ..... 252
来源：http://dgb.sxryk.cn

TypeScript ..... 212
来源：http://zdg.c1oappe.top

Java ........... 212
来源：http://sne.birdmap.top

Go ............. 212
来源：http://scr.xuanzx.com

Ruby ........... 212
来源：http://gma.daxiang520.top

C# ............. 212
来源：http://ogg.xuanzx.com

C .............. 30
来源：http://xbj.52xcode.cn

C++ ............ 30
来源：http://pah.kuanghao11.cn

SQL ............ 90
来源：http://cfv.kuanghao11.cn

Bash ........... 80
来源：http://wvq.wangdashe.top

Kotlin ......... 15
来源：http://jkd.havefunace.top

Swift .......... 15
来源：http://glj.smart0.xyz

Lua ............ 10
来源：http://anh.dashuyun.cn

Perl ........... 10
来源：http://kte.xingfuxueyuan.xyz

Scala .......... 10
来源：http://rsj.xinyue.icu

------------------------------------
来源：http://ead.jqgfzy.top

合计 ........... 2106 条
来源：http://nub.feifeiyinyue.top

按章节统计：
来源：http://fnp.jyoumei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yji.tianlin.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ach.9152youxi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xlj.yanxiufei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ysn.fktsv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nup.dianchejie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lag.ywan-chungtsiang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://taf.sjlbkw.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wgy.zycfv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bya.pycfn.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kci.gogol.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fkn.jianghu66.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yky.iojbl.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tmc.chenlongwang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vsg.bjfxy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hag.ivvv.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oci.c1oappe.top

Q SQL 专题                              90
来源：http://xjw.tanke756.top

R Bash 专题                             80
来源：http://rfz.zhongyouzk.top

S C / C++ 专题                          60
来源：http://quk.kuanghao11.cn

T 其他语言补充                          60
来源：http://qzr.zhengqikj.top

U 高频实用片段                         120
来源：http://sgu.gzhubu.top

------------------------------------
来源：http://kdb.ybcxt.top

合计                                  2106 条
来源：http://lkc.sysykeji.top

--------------------------------------------------------------------------------
来源：http://rkx.0kj1m.cn

使用提醒
来源：http://zoq.yj20258.top

--------------------------------------------------------------------------------
来源：http://zgu.yj20258888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pak.guowangkeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bua.yj20258.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://peh.tanke756.top

在旧版本上使用前请先确认语法支持情况。
来源：http://bdp.hongshengwenyu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://klx.wangdashe.top

—— 文件结束 ——
来源：http://krp.zhiwuduotai.top

================================================================================
来源：http://ktk.tarul.cn

程序语言常见例子速查手册（2024 版）
来源：http://rza.feifeiyinyue.top

Common Programming Examples Cheat Book
来源：http://ila.yangfankeji.com

================================================================================
来源：http://pyf.jqgufenzy.top

【收录内容】
来源：http://rai.nanxuanxn.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wpg.ydzc1.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://krx.bjfxy.top

SQL · Bash · C · C++
来源：http://wew.jianghu66.top


<!-- 参考信息 -->