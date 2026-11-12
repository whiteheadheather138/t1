代发 wailian999

[U13] Py：固定长度队列
来源：http://nrl.snrcjt.cn

deque(maxlen=10)
来源：http://wpc.sufxvd.cn

[U14] Py：分组收集到列表
来源：http://lyn.cashguo.top

defaultdict(list)
来源：http://ybj.andypj.xyz

[U15] Py：高精度计时
来源：http://tqd.yanxiufei.cn

t = time.perf_counter()
来源：http://cca.yj20258888.top

[U16] Py：命令行参数解析
来源：http://zdb.ydzc1.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dtb.jinghuilouyu.cn

[U17] Py：初始化日志
来源：http://sje.sweek.top

logging.basicConfig(level=logging.INFO)
来源：http://wub.mhx1999.top

[U18] Py：预编译正则
来源：http://afp.xziqi.cn

pat = re.compile(r"\d+")
来源：http://ong.zdqjudy.top

[U19] Py：正则替换带回调
来源：http://hva.jinqigfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mls.tianlin.xyz

[U20] Py：缓存函数结果
来源：http://sxv.epnwcf.com

@functools.lru_cache(maxsize=None)
来源：http://nzs.ivvv.top

[U21] Py：自定义上下文管理器
来源：http://atr.zdbjq.cn

@contextlib.contextmanager
来源：http://cai.chenzaomai.com

[U22] Py：矩阵转置
来源：http://dfl.yuanzhike.top

list(zip(*m))
来源：http://kna.hammf.cn

[U23] Py：分块读取大文件
来源：http://iwc.yongpay.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ves.shangyingyoupin.top

[U24] Py：路径操作
来源：http://txx.sweek.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lny.tianlin.xyz

[U25] Py：CSV 按字典读
来源：http://yiz.yuxming.cn

csv.DictReader(f)
来源：http://ljg.sxryk.cn

[U26] Py：并发下载
来源：http://ahq.daria6918.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://idk.yuanzhike.top

[U27] Py：异步 HTTP
来源：http://asu.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://dpq.jqgufenzy.top

[U28] Py：类型别名
来源：http://dta.xuanzx.com

UserId = int
来源：http://gzj.hnxiangtu.top

[U29] Py：属性校验
来源：http://xcy.cucudq.cn

@property 与 @x.setter 配合
来源：http://bbs.daxiang520.top

[U30] Py：数据类
来源：http://fjm.hesvh.cn

@dataclass(slots=True)
来源：http://sdp.52xcode.cn

[U31] Py：单测
来源：http://atq.nwbrower.top

python -m pytest -q
来源：http://paq.yvedp.cn

[U32] Py：代码格式化
来源：http://yqv.jinqigfzy.top

ruff format . && ruff check --fix .
来源：http://sra.9152youxi.cn

[U33] Py：打包发布
来源：http://rcl.jyoumei.cn

python -m build  （依赖 pyproject.toml）
来源：http://kiu.jinghuilouyu.cn

[U34] Py：判断编码
来源：http://mwu.hysaishi.cn

chardet.detect(raw)
来源：http://knr.ydjk.org.cn

[U35] Py：发送邮件
来源：http://mjd.hywenlv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pfi.jinqigufen.top

[U36] Py：定时任务
来源：http://mhb.cucudq.cn

schedule.every(10).minutes.do(job)
来源：http://jqp.52xcode.cn

[U37] Py：读写 Excel
来源：http://xel.tanke756.top

pandas.read_excel / DataFrame.to_excel
来源：http://lqy.hysaishi.cn

[U38] Py：获取脚本所在目录
来源：http://arc.snrcjt.cn

Path(__file__).resolve().parent
来源：http://vva.yanxiufei.cn

[U39] Py：判断是否在交互环境
来源：http://ufo.daxiang520.top

sys.stdout.isatty()
来源：http://vof.sufxvd.cn

[U40] Py：打印到标准错误
来源：http://djb.tian-w.cn

print("err", file=sys.stderr)
来源：http://dix.yanxiufei.cn

[U41] PHP：初始化 Composer 项目
来源：http://kax.jqgfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ujn.vehdjk.com

[U42] PHP：PSR-4 自动加载
来源：http://jid.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kvf.sweek.top

[U43] PHP：声明命名空间
来源：http://etm.jyoumei.cn

namespace App\Http;
来源：http://mwa.shanyushiyangkeji.top

[U44] PHP：开启严格类型
来源：http://gbn.tanke756.top

declare(strict_types=1);
来源：http://gng.yvedp.cn

[U45] PHP：类型声明与返回类型
来源：http://bus.chenzaomai.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://pin.meibo888.top

[U46] PHP：可空类型
来源：http://jrj.quarkkingdee.top

?string $name = null
来源：http://cva.hnxiangtu.top

[U47] PHP：联合类型
来源：http://zkb.dianchejie.cn

int|string $id
来源：http://pib.cashguo.top

[U48] PHP：纯枚举
来源：http://uyw.zhongyouzk.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tya.zhengqikj.top

[U49] PHP：只读属性
来源：http://rxf.zycfv.cn

public readonly string $name
来源：http://vit.sxryk.cn

[U50] PHP：构造器属性提升
来源：http://bfu.hcnkem.com

public function __construct(private int $id) {}
来源：http://tci.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://cin.dashuyun.cn

[$a, $b] = $arr;
来源：http://hmk.nanxinkj.top

[U52] PHP：箭头函数
来源：http://aga.zhongyouzk.top

$double = fn($x) => $x * 2;
来源：http://jne.jinqigfzy.top

[U53] PHP：空合并运算符
来源：http://iiu.vehdjk.com

$v = $a ?? $b ?? "default";
来源：http://tcv.chenlongwang.top

[U54] PHP：空安全调用
来源：http://cuc.sufxvd.cn

$obj?->method()
来源：http://kjv.9152youxi.cn

[U55] PHP：match 表达式
来源：http://dim.fehbvm.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://non.sysykeji.top

[U56] PHP：命名参数
来源：http://ufc.wangshuangyany.cn

f(a: 1, b: 2)
来源：http://zjl.yvedp.cn

[U57] PHP：字符串插值
来源：http://xxm.meibo888.top

"值: {$a}"
来源：http://xif.hysaishi.cn

[U58] PHP：数组三件套
来源：http://dxg.gaohongyu789.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pzg.yuanzhike.top

[U59] PHP：自定义排序
来源：http://xck.tanke756.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oms.zdbjq.cn

[U60] PHP：JSON 编解码
来源：http://ocn.mhx1999.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://puf.shuidangran.top

[U61] PHP：正则
来源：http://hbk.fehbvm.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rvr.redwolf501.top

[U62] PHP：日期对象
来源：http://zbj.fengsongda.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lsm.hammf.cn

[U63] PHP：文件读写
来源：http://zxq.havefunace.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lrm.9152youxi.cn

[U64] PHP：目录遍历
来源：http://fud.chenjidiqi.icu

glob("dir/*.php");  scandir("dir");
来源：http://sir.gzhubu.top

[U65] PHP：会话
来源：http://dsj.redwolf501.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gpl.epnwcf.com

[U66] PHP：设置 Cookie
来源：http://gdq.hfpthk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nru.pengpengdd.cyou

[U67] PHP：处理文件上传
来源：http://zds.hesvh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rlo.gogol.net.cn

[U68] PHP：PDO 连接
来源：http://ywd.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zny.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://emd.tianlin.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ifh.guannengcc.top

[U70] PHP：PDO 事务
来源：http://iax.jyoumei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rtc.hysaishi.cn

[U71] PHP：抛出异常
来源：http://cfl.epnwcf.com

throw new RuntimeException("失败", 500);
来源：http://jxc.yfazqb.com

[U72] PHP：写错误日志
来源：http://imu.svipenyu.cn

error_log("失败: " . $e->getMessage());
来源：http://prv.sweek.top

[U73] PHP：读取 ini 配置
来源：http://hbr.sysykeji.top

parse_ini_file("config.ini", true)
来源：http://drw.pycfn.com

[U74] PHP：读取环境变量
来源：http://brv.wangshuangyany.cn

getenv("APP_ENV") ?: "production"
来源：http://sse.tanke756.top

[U75] PHP：依赖注入
来源：http://pex.jiagoushi.top

composer require psr/container
来源：http://nda.yj20258.top

[U76] PHP：简单路由
来源：http://lmn.zycfv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sxl.jqgfzy.top

[U77] PHP：模板渲染
来源：http://oiz.sweek.top

composer require twig/twig
来源：http://seu.yj202588.top

[U78] PHP：单元测试
来源：http://siy.ydzc1.top

composer require --dev phpunit/phpunit
来源：http://ekk.jinyuanbaomall.cn

[U79] PHP：静态分析
来源：http://vms.aibaodan.cn

composer require --dev phpstan/phpstan
来源：http://rti.c1oappe.top

[U80] PHP：代码规范修复
来源：http://tlq.yongpay.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rev.nwbrower.top

[U81] JS：初始化项目
来源：http://rwv.ydjk.org.cn

npm init -y;  npm i express
来源：http://hag.chenlongwang.top

[U82] JS：package.json 脚本
来源：http://ctv.iojbl.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://juz.316326.xyz

[U83] JS：ES Module 导入导出
来源：http://ibe.sjlbkw.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fdp.jlsjyb.cn

[U84] JS：CommonJS 写法
来源：http://zal.fanxiaobao.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://wrt.mhx1999.top

[U85] JS：可选链
来源：http://dnn.yanxiufei.cn

a?.b?.c
来源：http://wdq.zdqjudy.top

[U86] JS：空值合并
来源：http://mgy.sufxvd.cn

a ?? b
来源：http://ein.guowangkeji.top

[U87] JS：解构默认值
来源：http://huf.xuanzx.com

const { a = 1, b = 2 } = obj;
来源：http://dvd.tianlin.xyz

[U88] JS：对象展开合并
来源：http://obl.fzhhl.top

{ ...a, ...b }
来源：http://zrl.hfpthk.cn

[U89] JS：数组去重
来源：http://vdn.ivvv.top

[...new Set(arr)]
来源：http://pni.svipenyu.cn

[U90] JS：数字数组排序
来源：http://tom.aizwys.cn

[...arr].sort((a, b) => a - b)
来源：http://pyp.chenjidiqi.icu

[U91] JS：对象键值遍历
来源：http://oqm.haohaochexian.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cyq.cucudq.cn

[U92] JS：深拷贝
来源：http://bfs.xinyue.icu

structuredClone(obj)
来源：http://wbf.jlsjyb.cn

[U93] JS：模板字符串
来源：http://mdd.guowangkeji.top

`共 ${n} 条`
来源：http://adq.jinqigfzy.top

[U94] JS：箭头函数
来源：http://wad.zhiwuduotai.top

const double = x => x * 2;
来源：http://lce.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://hhj.havefunace.top

new Promise((resolve, reject) => {})
来源：http://kyf.ybcxt.top

[U96] JS：async/await 与异常
来源：http://mnn.zhengqikj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qmh.jiagoushi.top

[U97] JS：并发请求
来源：http://gql.jianghu66.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bur.redwolf501.top

[U98] JS：fetch 带 JSON
来源：http://skd.smart0.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://acl.chenlongwang.top

[U99] JS：事件监听
来源：http://huc.shuidangran.top

el.addEventListener("click", e => {})
来源：http://ijv.fehbvm.com

[U100] JS：DOM 查询
来源：http://qbs.haohaochexian.top

document.querySelector(".item")
来源：http://xmd.iojbl.cn

[U101] JS：classList 操作
来源：http://tfp.vehdjk.com

el.classList.toggle("active")
来源：http://rnr.jqgufenzy.top

[U102] JS：本地存储
来源：http://sle.daria6918.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lxo.bjfxy.top

[U103] JS：定时器
来源：http://wqw.sufxvd.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rxg.cdnleiting.top

[U104] JS：防抖
来源：http://ozs.jyoumei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ern.jinghuilouyu.cn

[U105] JS：节流
来源：http://naf.andypj.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kqs.ehwqpu.com

[U106] JS：日期格式化
来源：http://xbm.dashuyun.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sfh.hnxiangtu.top

[U107] JS：数字千分位
来源：http://upq.tian-w.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wvc.52xcode.cn

[U108] JS：随机整数
来源：http://hak.jianghu66.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ubn.yj202588.top

[U109] JS：数组分组
来源：http://nxx.kuanghao11.cn

Object.groupBy(arr, x => x.type)
来源：http://zmy.daxiang520.top

[U110] JS：数组分块
来源：http://sxf.andypj.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nha.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://eix.wangdashe.top

new Map(Object.entries(obj))
来源：http://uol.hnqzz.top

[U112] JS：字符串补位
来源：http://cfw.gzhubu.top

"7".padStart(3, "0")
来源：http://rht.dianchejie.cn

[U113] JS：正则替换全部
来源：http://kfo.andypj.xyz

s.replaceAll("a", "b")
来源：http://ngy.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://ndl.yonumen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nwb.mhx1999.top

[U115] JS：生成 UUID
来源：http://umc.xinyue.icu

crypto.randomUUID()
来源：http://lnx.yj20258.top

[U116] JS：类型检查（JSDoc）
来源：http://idn.nwbrower.top

/** @param {string} name */ function f(name) {}
来源：http://blj.xinyue.icu

[U117] JS：单元测试
来源：http://jmz.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://ymw.havefunace.top

[U118] JS：开发服务器
来源：http://ypp.shzxlz.cn

npm i -D vite;  npx vite
来源：http://yhj.yonumen.top

[U119] JS：生产构建
来源：http://hmp.xylfe.cn

npx vite build
来源：http://pma.xylfe.cn

[U120] JS：读取环境变量（Vite）
来源：http://rvj.ctjpmb.com

import.meta.env.VITE_API_URL
来源：http://pfw.ppjwa.cn

================================================================================
来源：http://hxx.ybcxt.top

统计汇总
来源：http://rdq.cdnleiting.top

================================================================================
来源：http://ijz.hcnkem.com

按语言统计（条）：
来源：http://dqf.hysaishi.cn

Python ......... 252
来源：http://dls.0kj1m.cn

PHP ............ 252
来源：http://ygh.dianchejie.cn

JavaScript ..... 252
来源：http://htu.yanxiufei.cn

TypeScript ..... 212
来源：http://tbw.quarkkingdee.top

Java ........... 212
来源：http://cei.chenzaomai.com

Go ............. 212
来源：http://mqc.yongpay.top

Ruby ........... 212
来源：http://zxe.shuidangran.top

C# ............. 212
来源：http://ycc.ivvv.top

C .............. 30
来源：http://heh.gotoacloud.top

C++ ............ 30
来源：http://rpo.yonumen.top

SQL ............ 90
来源：http://xgh.fktsv.cn

Bash ........... 80
来源：http://uzj.epnwcf.com

Kotlin ......... 15
来源：http://glh.aibaodan.cn

Swift .......... 15
来源：http://gkg.tian-w.cn

Lua ............ 10
来源：http://ezs.birdmap.top

Perl ........... 10
来源：http://sxi.epnwcf.com

Scala .......... 10
来源：http://snk.yangfankeji.com

------------------------------------
来源：http://cvk.hfpthk.cn

合计 ........... 2106 条
来源：http://jdl.xinyue.icu

按章节统计：
来源：http://vyg.sufxvd.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cmm.fehbvm.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nwo.xuanzx.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uro.zhaomingkeji.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ubn.pycfn.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vqo.zycfv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://woe.xingfuxueyuan.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uze.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://quy.cheryme.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ava.jinqigufen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wlt.dianchejie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ish.ehwqpu.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gda.xinyue.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vov.yueranfly.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jww.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rtq.zdqjudy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rvu.nanxuanxn.top

Q SQL 专题                              90
来源：http://xzt.sysykeji.top

R Bash 专题                             80
来源：http://cou.nanxinkj.top

S C / C++ 专题                          60
来源：http://hsn.sufxvd.cn

T 其他语言补充                          60
来源：http://qnh.kuanghao11.cn

U 高频实用片段                         120
来源：http://trt.hnxiangtu.top

------------------------------------
来源：http://yrg.xingfuxueyuan.xyz

合计                                  2106 条
来源：http://clw.ydzc1.top

--------------------------------------------------------------------------------
来源：http://dhm.zhixingplan.top

使用提醒
来源：http://dzs.fktsv.cn

--------------------------------------------------------------------------------
来源：http://zlo.daxiang520.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cti.uphjek.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rjt.sysykeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fid.sufxvd.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zvk.nwbrower.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ckw.wangdashe.top

—— 文件结束 ——
来源：http://gcb.smart0.xyz

================================================================================
来源：http://hlz.zhaomingkeji.xyz

程序语言常见例子速查手册（2024 版）
来源：http://dqa.yongpay.top

Common Programming Examples Cheat Book
来源：http://xrf.ydjk.org.cn

================================================================================
来源：http://fmn.hcnkem.com

【收录内容】
来源：http://oyr.sweek.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://gjd.jinqigfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://itv.sweek.top

SQL · Bash · C · C++
来源：http://ydx.hfpthk.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hac.haohaochexian.top

【使用说明】
来源：http://seb.snrcjt.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ben.dianchejie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fdj.fktsv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uqs.zhoulong.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rda.yfazqb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://blh.ydzc1.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xmq.yongpay.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lgv.sxryk.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fov.zhaomingkeji.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://iaq.kuanghao11.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fvb.guannengcc.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mvk.gogol.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zta.gotoacloud.top

【文件统计】
来源：http://ksy.xziqi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qcf.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://kfj.ivvv.top

目  录
来源：http://agz.316326.xyz

--------------------------------------------------------------------------------
来源：http://qcl.wangshuangyany.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pmr.tanke756.top


<!-- 参考信息 -->