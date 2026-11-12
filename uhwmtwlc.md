代发 wailian999

[U11] Py：生成器表达式
来源：http://jfb.hfpthk.cn

(x * 2 for x in arr)
来源：http://sff.quarkkingdee.top

[U12] Py：取出现最多的 3 个元素
来源：http://jsg.yangfankeji.com

Counter(arr).most_common(3)
来源：http://hco.birdmap.top

[U13] Py：固定长度队列
来源：http://oox.xziqi.cn

deque(maxlen=10)
来源：http://bkt.havefunace.top

[U14] Py：分组收集到列表
来源：http://qts.dianchejie.cn

defaultdict(list)
来源：http://oji.zhijiandao.cn

[U15] Py：高精度计时
来源：http://vps.mhx1999.top

t = time.perf_counter()
来源：http://xgc.tarul.cn

[U16] Py：命令行参数解析
来源：http://lyf.ehwqpu.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vdo.jianghu66.top

[U17] Py：初始化日志
来源：http://ktr.tian-w.cn

logging.basicConfig(level=logging.INFO)
来源：http://dcp.nwbrower.top

[U18] Py：预编译正则
来源：http://ivq.tanke756.top

pat = re.compile(r"\d+")
来源：http://uck.gogol.net.cn

[U19] Py：正则替换带回调
来源：http://ivi.vehdjk.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pig.dashuyun.cn

[U20] Py：缓存函数结果
来源：http://rlg.yfazqb.com

@functools.lru_cache(maxsize=None)
来源：http://slt.daria6918.cn

[U21] Py：自定义上下文管理器
来源：http://yus.bbcook.cn

@contextlib.contextmanager
来源：http://dul.snrcjt.cn

[U22] Py：矩阵转置
来源：http://uxh.shanyushiyangkeji.top

list(zip(*m))
来源：http://gkd.meibo888.top

[U23] Py：分块读取大文件
来源：http://fhf.xinyue.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nwy.wangdashe.top

[U24] Py：路径操作
来源：http://ezr.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://imp.vqdsnc.cn

[U25] Py：CSV 按字典读
来源：http://pwc.c1oappe.top

csv.DictReader(f)
来源：http://dbo.svipenyu.cn

[U26] Py：并发下载
来源：http://baj.gotoacloud.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://olx.smart0.xyz

[U27] Py：异步 HTTP
来源：http://kgi.fehbvm.com

aiohttp.ClientSession() 配合 async with
来源：http://dut.xziqi.cn

[U28] Py：类型别名
来源：http://xsa.yj20258888.top

UserId = int
来源：http://qot.hnqzz.top

[U29] Py：属性校验
来源：http://yos.jinqigfzy.top

@property 与 @x.setter 配合
来源：http://fbb.sysykeji.top

[U30] Py：数据类
来源：http://yrz.hfpthk.cn

@dataclass(slots=True)
来源：http://ypj.zhixingplan.top

[U31] Py：单测
来源：http://pdp.0kj1m.cn

python -m pytest -q
来源：http://rlo.ydjk.org.cn

[U32] Py：代码格式化
来源：http://vud.zhijiandao.cn

ruff format . && ruff check --fix .
来源：http://nll.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://unj.uphjek.com

python -m build  （依赖 pyproject.toml）
来源：http://yba.mhx1999.top

[U34] Py：判断编码
来源：http://yav.yangfankeji.com

chardet.detect(raw)
来源：http://zsz.jinqigufen.top

[U35] Py：发送邮件
来源：http://znc.chenjidiqi.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ccp.yuxming.cn

[U36] Py：定时任务
来源：http://jtv.ppjwa.cn

schedule.every(10).minutes.do(job)
来源：http://ikn.mhx1999.top

[U37] Py：读写 Excel
来源：http://erp.hysaishi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xug.epnwcf.com

[U38] Py：获取脚本所在目录
来源：http://fgz.yuxming.cn

Path(__file__).resolve().parent
来源：http://mvk.yangfankeji.com

[U39] Py：判断是否在交互环境
来源：http://iol.gogol.net.cn

sys.stdout.isatty()
来源：http://qoz.hammf.cn

[U40] Py：打印到标准错误
来源：http://ebt.52xcode.cn

print("err", file=sys.stderr)
来源：http://umj.yj20258.top

[U41] PHP：初始化 Composer 项目
来源：http://yjz.bjfxy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://hlv.gogol.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://fwu.wangshuangyany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tiy.fehbvm.com

[U43] PHP：声明命名空间
来源：http://aol.pycfn.com

namespace App\Http;
来源：http://sjp.ydzc1.top

[U44] PHP：开启严格类型
来源：http://dec.yuxming.cn

declare(strict_types=1);
来源：http://jxq.tarul.cn

[U45] PHP：类型声明与返回类型
来源：http://xbi.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://ogg.zhengqikj.top

[U46] PHP：可空类型
来源：http://ori.cdnleiting.top

?string $name = null
来源：http://zxh.jinqigufen.top

[U47] PHP：联合类型
来源：http://mnu.fengsongda.top

int|string $id
来源：http://peq.chenjidiqi.icu

[U48] PHP：纯枚举
来源：http://skn.jinghuilouyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yua.zhoulong.xyz

[U49] PHP：只读属性
来源：http://azn.yongpay.top

public readonly string $name
来源：http://oqt.epnwcf.com

[U50] PHP：构造器属性提升
来源：http://ksv.316326.xyz

public function __construct(private int $id) {}
来源：http://vmi.yfazqb.com

[U51] PHP：数组解构
来源：http://jho.haohaochexian.top

[$a, $b] = $arr;
来源：http://rrp.jyoumei.cn

[U52] PHP：箭头函数
来源：http://ggu.xuanzx.com

$double = fn($x) => $x * 2;
来源：http://jwd.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://yek.xinyue.icu

$v = $a ?? $b ?? "default";
来源：http://ovl.bjfxy.top

[U54] PHP：空安全调用
来源：http://oyl.ctjpmb.com

$obj?->method()
来源：http://jds.snrcjt.cn

[U55] PHP：match 表达式
来源：http://okv.hnxiangtu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mhq.nanxinkj.top

[U56] PHP：命名参数
来源：http://izk.yj202588.top

f(a: 1, b: 2)
来源：http://ahr.yanxiufei.cn

[U57] PHP：字符串插值
来源：http://oob.guowangkeji.top

"值: {$a}"
来源：http://yhc.yvedp.cn

[U58] PHP：数组三件套
来源：http://dxx.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bqi.zhongyouzk.top

[U59] PHP：自定义排序
来源：http://acf.tarul.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://acp.meibo888.top

[U60] PHP：JSON 编解码
来源：http://rih.gogol.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qau.quarkkingdee.top

[U61] PHP：正则
来源：http://ypl.tarul.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sra.cashguo.top

[U62] PHP：日期对象
来源：http://dkc.yfazqb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ema.ctjpmb.com

[U63] PHP：文件读写
来源：http://ayh.chenzaomai.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hop.zhixingplan.top

[U64] PHP：目录遍历
来源：http://gbv.yanxiufei.cn

glob("dir/*.php");  scandir("dir");
来源：http://tvn.sxryk.cn

[U65] PHP：会话
来源：http://ena.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://avc.ehwqpu.com

[U66] PHP：设置 Cookie
来源：http://kza.cucudq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://luw.aizwys.cn

[U67] PHP：处理文件上传
来源：http://ulb.smart0.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jar.yongpay.top

[U68] PHP：PDO 连接
来源：http://ynk.hnxiangtu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://avn.pycfn.com

[U69] PHP：PDO 预处理
来源：http://anj.yj202588.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://boc.shzxlz.cn

[U70] PHP：PDO 事务
来源：http://gtg.andypj.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aee.ybcxt.top

[U71] PHP：抛出异常
来源：http://syd.0kj1m.cn

throw new RuntimeException("失败", 500);
来源：http://iyy.aizwys.cn

[U72] PHP：写错误日志
来源：http://vnj.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://tsd.jinqigfzy.top

[U73] PHP：读取 ini 配置
来源：http://jdb.fengsongda.top

parse_ini_file("config.ini", true)
来源：http://ahv.316326.xyz

[U74] PHP：读取环境变量
来源：http://sex.vehdjk.com

getenv("APP_ENV") ?: "production"
来源：http://fvl.mhx1999.top

[U75] PHP：依赖注入
来源：http://zhe.jqgufenzy.top

composer require psr/container
来源：http://ydy.316326.xyz

[U76] PHP：简单路由
来源：http://aas.316326.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ity.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://qtd.guowangkeji.top

composer require twig/twig
来源：http://vic.yonumen.top

[U78] PHP：单元测试
来源：http://mxm.jinghuilouyu.cn

composer require --dev phpunit/phpunit
来源：http://gsz.xylfe.cn

[U79] PHP：静态分析
来源：http://gif.gotoacloud.top

composer require --dev phpstan/phpstan
来源：http://fpt.yanxiufei.cn

[U80] PHP：代码规范修复
来源：http://tie.uphjek.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://dyx.fanxiaobao.xyz

[U81] JS：初始化项目
来源：http://xgf.xylfe.cn

npm init -y;  npm i express
来源：http://eri.aibaodan.cn

[U82] JS：package.json 脚本
来源：http://vuz.xylfe.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sxz.jinqigfzy.top

[U83] JS：ES Module 导入导出
来源：http://pxd.hcnkem.com

export const a = 1;  import { a } from "./m.js";
来源：http://wcl.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://efg.hnxiangtu.top

module.exports = { a };  const { a } = require("./m");
来源：http://oxb.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://qon.wangdashe.top

a?.b?.c
来源：http://qez.chenjidiqi.icu

[U86] JS：空值合并
来源：http://obj.ydzc1.top

a ?? b
来源：http://vij.zhoulong.xyz

[U87] JS：解构默认值
来源：http://ruq.hfpthk.cn

const { a = 1, b = 2 } = obj;
来源：http://iww.smart0.xyz

[U88] JS：对象展开合并
来源：http://iwg.jlsjyb.cn

{ ...a, ...b }
来源：http://jxy.hongshengwenyu.top

[U89] JS：数组去重
来源：http://cne.zhengqikj.top

[...new Set(arr)]
来源：http://wzo.fzhhl.top

[U90] JS：数字数组排序
来源：http://dew.meibo888.top

[...arr].sort((a, b) => a - b)
来源：http://mrc.fzhhl.top

[U91] JS：对象键值遍历
来源：http://bjc.chenlongwang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bjv.xylfe.cn

[U92] JS：深拷贝
来源：http://wcb.zhoulong.xyz

structuredClone(obj)
来源：http://ibs.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://eyh.shzxlz.cn

`共 ${n} 条`
来源：http://qce.tarul.cn

[U94] JS：箭头函数
来源：http://tct.xylfe.cn

const double = x => x * 2;
来源：http://zsb.kuanghao11.cn

[U95] JS：Promise 包装
来源：http://ktv.aizwys.cn

new Promise((resolve, reject) => {})
来源：http://siy.9152youxi.cn

[U96] JS：async/await 与异常
来源：http://are.aizwys.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eoj.hnqzz.top

[U97] JS：并发请求
来源：http://mpx.yangfankeji.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://gtk.yanxiufei.cn

[U98] JS：fetch 带 JSON
来源：http://bbv.mhx1999.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ubq.yj202588.top

[U99] JS：事件监听
来源：http://kqx.sufxvd.cn

el.addEventListener("click", e => {})
来源：http://ibs.yongpay.top

[U100] JS：DOM 查询
来源：http://uax.9152youxi.cn

document.querySelector(".item")
来源：http://ves.wangshuangyany.cn

[U101] JS：classList 操作
来源：http://ztb.aibaodan.cn

el.classList.toggle("active")
来源：http://ipy.chenlongwang.top

[U102] JS：本地存储
来源：http://npb.bbcook.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lqq.zdbjq.cn

[U103] JS：定时器
来源：http://dns.sweek.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://unv.guannengcc.top

[U104] JS：防抖
来源：http://bbo.hfpthk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rou.52xcode.cn

[U105] JS：节流
来源：http://pkt.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qpr.jinqigfzy.top

[U106] JS：日期格式化
来源：http://trn.c1oappe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xhy.yongpay.top

[U107] JS：数字千分位
来源：http://tzv.ydzc1.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bqg.yj20258888.top

[U108] JS：随机整数
来源：http://zpx.bjfxy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wex.hnxiangtu.top

[U109] JS：数组分组
来源：http://owa.yangfankeji.com

Object.groupBy(arr, x => x.type)
来源：http://pls.haohaochexian.top

[U110] JS：数组分块
来源：http://oeq.svipenyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nhj.gzhubu.top

[U111] JS：对象转 Map
来源：http://jqz.hywenlv.cn

new Map(Object.entries(obj))
来源：http://cjn.gzhubu.top

[U112] JS：字符串补位
来源：http://ldf.jqgufenzy.top

"7".padStart(3, "0")
来源：http://uci.yj20258888.top

[U113] JS：正则替换全部
来源：http://uja.hnqzz.top

s.replaceAll("a", "b")
来源：http://cmi.yvedp.cn

[U114] JS：JSON 深比较
来源：http://xjr.jqgfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://kvp.snrcjt.cn

[U115] JS：生成 UUID
来源：http://lsc.vehdjk.com

crypto.randomUUID()
来源：http://sjk.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://vxk.yvedp.cn

/** @param {string} name */ function f(name) {}
来源：http://sqs.yj20258.top

[U117] JS：单元测试
来源：http://win.ydzc1.top

npm i -D vitest;  npx vitest
来源：http://tdn.chenzaomai.com

[U118] JS：开发服务器
来源：http://xhl.jianghu66.top

npm i -D vite;  npx vite
来源：http://aor.hnxiangtu.top

[U119] JS：生产构建
来源：http://whf.chenzaomai.com

npx vite build
来源：http://cpm.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://wlv.birdmap.top

import.meta.env.VITE_API_URL
来源：http://syc.jyoumei.cn

================================================================================
来源：http://pba.yuanzhike.top

统计汇总
来源：http://ibe.iojbl.cn

================================================================================
来源：http://uam.svipenyu.cn

按语言统计（条）：
来源：http://woy.yj20258888.top

Python ......... 252
来源：http://nve.aibaodan.cn

PHP ............ 252
来源：http://tpn.yj20258.top

JavaScript ..... 252
来源：http://wvy.chenjidiqi.icu

TypeScript ..... 212
来源：http://vsg.52xcode.cn

Java ........... 212
来源：http://nfi.ydjk.org.cn

Go ............. 212
来源：http://pcs.guowangkeji.top

Ruby ........... 212
来源：http://hrb.dashuyun.cn

C# ............. 212
来源：http://nmq.fehbvm.com

C .............. 30
来源：http://exi.sweek.top

C++ ............ 30
来源：http://qcz.hfpthk.cn

SQL ............ 90
来源：http://jfh.yj202588.top

Bash ........... 80
来源：http://lri.jyoumei.cn

Kotlin ......... 15
来源：http://hpo.yonumen.top

Swift .......... 15
来源：http://pwd.yueranfly.top

Lua ............ 10
来源：http://zse.sweek.top

Perl ........... 10
来源：http://bwf.ppjwa.cn

Scala .......... 10
来源：http://ghq.yongpay.top

------------------------------------
来源：http://tbv.havefunace.top

合计 ........... 2106 条
来源：http://slh.cheryme.top

按章节统计：
来源：http://rol.c1oappe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ipd.hcnkem.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dmu.zdqjudy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nej.daria6918.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hrd.yfazqb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jay.52xcode.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hpi.yuanzhike.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hto.ydjk.org.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eka.yj202588.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wna.mhx1999.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kdr.daxiang520.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xkk.jinqigufen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fyj.jinyuanbaomall.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qso.ybcxt.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://djj.sjlbkw.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tcb.yj202588.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jzb.aizwys.cn

Q SQL 专题                              90
来源：http://ctu.cheryme.top

R Bash 专题                             80
来源：http://rtd.daxiang520.top

S C / C++ 专题                          60
来源：http://kbe.chenlongwang.top

T 其他语言补充                          60
来源：http://tah.uphjek.com

U 高频实用片段                         120
来源：http://nod.ppjwa.cn

------------------------------------
来源：http://vph.xuanzx.com

合计                                  2106 条
来源：http://wnd.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://jrs.yueranfly.top

使用提醒
来源：http://yjt.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://van.guannengcc.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://srr.ppjwa.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dxx.chenlongwang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://znc.jianghu66.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ixl.hywenlv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://clk.jlsjyb.cn

—— 文件结束 ——
来源：http://vgy.sjlbkw.cn

================================================================================
来源：http://gmw.hesvh.cn

程序语言常见例子速查手册（2024 版）
来源：http://wic.chenlongwang.top

Common Programming Examples Cheat Book
来源：http://tmj.daria6918.cn

================================================================================
来源：http://hgp.sufxvd.cn

【收录内容】
来源：http://xck.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pyw.cucudq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://njf.fengsongda.top

SQL · Bash · C · C++
来源：http://sfj.yonumen.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rfv.guannengcc.top

【使用说明】
来源：http://cds.kuanghao11.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fnt.guowangkeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://aqi.xuetiantiany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ibl.cucudq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ryk.xingfuxueyuan.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://tdx.meibo888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oft.vqdsnc.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://psp.nanxuanxn.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://osy.quarkkingdee.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tos.fzhhl.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yej.hnqzz.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tty.dashuyun.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zbi.gogol.net.cn

【文件统计】
来源：http://qub.ydjk.org.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iud.hywenlv.cn


<!-- 参考信息 -->