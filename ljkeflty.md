代发 wailian999

[U09] Py：字典取最大值的键
来源：http://phf.zdbjq.cn

max(d, key=d.get)
来源：http://yfp.daxiang520.top

[U10] Py：按值排序字典
来源：http://rra.hnxiangtu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mbo.haohaochexian.top

[U11] Py：生成器表达式
来源：http://jpt.yonumen.top

(x * 2 for x in arr)
来源：http://egc.ybcxt.top

[U12] Py：取出现最多的 3 个元素
来源：http://xkd.sweek.top

Counter(arr).most_common(3)
来源：http://jnc.yongpay.top

[U13] Py：固定长度队列
来源：http://nhu.ydjk.org.cn

deque(maxlen=10)
来源：http://fdn.shangyingyoupin.top

[U14] Py：分组收集到列表
来源：http://dtl.wangdashe.top

defaultdict(list)
来源：http://rte.ivvv.top

[U15] Py：高精度计时
来源：http://jbr.jiagoushi.top

t = time.perf_counter()
来源：http://awv.haohaochexian.top

[U16] Py：命令行参数解析
来源：http://azv.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iqq.jiagoushi.top

[U17] Py：初始化日志
来源：http://ica.iojbl.cn

logging.basicConfig(level=logging.INFO)
来源：http://ggb.xinyue.icu

[U18] Py：预编译正则
来源：http://acr.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://lop.0kj1m.cn

[U19] Py：正则替换带回调
来源：http://mov.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yvp.52xcode.cn

[U20] Py：缓存函数结果
来源：http://tfw.hongshengwenyu.top

@functools.lru_cache(maxsize=None)
来源：http://pnl.xuetiantiany.cn

[U21] Py：自定义上下文管理器
来源：http://tdb.0kj1m.cn

@contextlib.contextmanager
来源：http://avp.pycfn.com

[U22] Py：矩阵转置
来源：http://sxh.sweek.top

list(zip(*m))
来源：http://kbm.jinghuilouyu.cn

[U23] Py：分块读取大文件
来源：http://yic.sysykeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://skg.aibaodan.cn

[U24] Py：路径操作
来源：http://soc.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://miq.daria6918.cn

[U25] Py：CSV 按字典读
来源：http://but.hcnkem.com

csv.DictReader(f)
来源：http://bqq.sxryk.cn

[U26] Py：并发下载
来源：http://vjm.hfpthk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kps.meibo888.top

[U27] Py：异步 HTTP
来源：http://ewp.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://yos.vqdsnc.cn

[U28] Py：类型别名
来源：http://zgm.jinyuanbaomall.cn

UserId = int
来源：http://brq.daxiang520.top

[U29] Py：属性校验
来源：http://zfw.sweek.top

@property 与 @x.setter 配合
来源：http://bjg.andypj.xyz

[U30] Py：数据类
来源：http://tbo.zycfv.cn

@dataclass(slots=True)
来源：http://gyg.snrcjt.cn

[U31] Py：单测
来源：http://ygb.uphjek.com

python -m pytest -q
来源：http://pbw.gaohongyu789.top

[U32] Py：代码格式化
来源：http://yht.jinqigufen.top

ruff format . && ruff check --fix .
来源：http://eoo.epnwcf.com

[U33] Py：打包发布
来源：http://jfu.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://ggw.yj202588.top

[U34] Py：判断编码
来源：http://uwu.hesvh.cn

chardet.detect(raw)
来源：http://mka.ywan-chungtsiang.top

[U35] Py：发送邮件
来源：http://wdt.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gtk.hcnkem.com

[U36] Py：定时任务
来源：http://bcn.52xcode.cn

schedule.every(10).minutes.do(job)
来源：http://tic.jinyuanbaomall.cn

[U37] Py：读写 Excel
来源：http://bvg.hywenlv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tpz.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://usg.shanyushiyangkeji.top

Path(__file__).resolve().parent
来源：http://ogk.jqgfzy.top

[U39] Py：判断是否在交互环境
来源：http://xwo.jianghu66.top

sys.stdout.isatty()
来源：http://itq.dianchejie.cn

[U40] Py：打印到标准错误
来源：http://eka.vqdsnc.cn

print("err", file=sys.stderr)
来源：http://sfu.yangfankeji.com

[U41] PHP：初始化 Composer 项目
来源：http://tdc.wangdashe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://joz.yj202588.top

[U42] PHP：PSR-4 自动加载
来源：http://bfl.chenjidiqi.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hbk.fzhhl.top

[U43] PHP：声明命名空间
来源：http://wgb.jiagoushi.top

namespace App\Http;
来源：http://rah.redwolf501.top

[U44] PHP：开启严格类型
来源：http://ffw.fanxiaobao.xyz

declare(strict_types=1);
来源：http://ikn.ehwqpu.com

[U45] PHP：类型声明与返回类型
来源：http://vlt.fengsongda.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ehy.jinqigfzy.top

[U46] PHP：可空类型
来源：http://ecz.vehdjk.com

?string $name = null
来源：http://gfp.yongpay.top

[U47] PHP：联合类型
来源：http://phv.dianchejie.cn

int|string $id
来源：http://fxz.zhaomingkeji.xyz

[U48] PHP：纯枚举
来源：http://ikg.ehwqpu.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zop.52xcode.cn

[U49] PHP：只读属性
来源：http://sxn.daria6918.cn

public readonly string $name
来源：http://boa.mhx1999.top

[U50] PHP：构造器属性提升
来源：http://ivx.tian-w.cn

public function __construct(private int $id) {}
来源：http://axh.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://mqj.tianlin.xyz

[$a, $b] = $arr;
来源：http://zeh.havefunace.top

[U52] PHP：箭头函数
来源：http://hsz.0kj1m.cn

$double = fn($x) => $x * 2;
来源：http://nes.cheryme.top

[U53] PHP：空合并运算符
来源：http://niw.yangfankeji.com

$v = $a ?? $b ?? "default";
来源：http://lwu.yvedp.cn

[U54] PHP：空安全调用
来源：http://lhl.fzhhl.top

$obj?->method()
来源：http://opi.ydjk.org.cn

[U55] PHP：match 表达式
来源：http://nyy.hammf.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qcv.chenlongwang.top

[U56] PHP：命名参数
来源：http://bod.jinqigfzy.top

f(a: 1, b: 2)
来源：http://qdx.bbcook.cn

[U57] PHP：字符串插值
来源：http://vnz.yangfankeji.com

"值: {$a}"
来源：http://dgg.hywenlv.cn

[U58] PHP：数组三件套
来源：http://yfv.zhijiandao.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nce.hnqzz.top

[U59] PHP：自定义排序
来源：http://cni.jinqigufen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ooo.daxiang520.top

[U60] PHP：JSON 编解码
来源：http://spi.zdqjudy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zrx.ywan-chungtsiang.top

[U61] PHP：正则
来源：http://ghr.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://crp.sufxvd.cn

[U62] PHP：日期对象
来源：http://joo.jinqigufen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://frj.tianlin.xyz

[U63] PHP：文件读写
来源：http://iyp.jinqigufen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hgs.cdnleiting.top

[U64] PHP：目录遍历
来源：http://crn.smart0.xyz

glob("dir/*.php");  scandir("dir");
来源：http://ryq.birdmap.top

[U65] PHP：会话
来源：http://jme.jinqigfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vrv.yfazqb.com

[U66] PHP：设置 Cookie
来源：http://pav.c1oappe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nus.ivvv.top

[U67] PHP：处理文件上传
来源：http://bgx.jinyuanbaomall.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zmn.nanxinkj.top

[U68] PHP：PDO 连接
来源：http://wrd.ywan-chungtsiang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lye.gogol.net.cn

[U69] PHP：PDO 预处理
来源：http://djo.zhijiandao.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eca.meibo888.top

[U70] PHP：PDO 事务
来源：http://jmp.andypj.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rfm.yuanzhike.top

[U71] PHP：抛出异常
来源：http://ffe.jinqigufen.top

throw new RuntimeException("失败", 500);
来源：http://frb.fktsv.cn

[U72] PHP：写错误日志
来源：http://dht.jinghuilouyu.cn

error_log("失败: " . $e->getMessage());
来源：http://xes.jinqigufen.top

[U73] PHP：读取 ini 配置
来源：http://nzj.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://wyn.yongpay.top

[U74] PHP：读取环境变量
来源：http://fbs.hysaishi.cn

getenv("APP_ENV") ?: "production"
来源：http://bca.epnwcf.com

[U75] PHP：依赖注入
来源：http://aih.quarkkingdee.top

composer require psr/container
来源：http://vfd.guannengcc.top

[U76] PHP：简单路由
来源：http://lyf.gotoacloud.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qwz.andypj.xyz

[U77] PHP：模板渲染
来源：http://hhn.guannengcc.top

composer require twig/twig
来源：http://qec.jinqigufen.top

[U78] PHP：单元测试
来源：http://bml.ctjpmb.com

composer require --dev phpunit/phpunit
来源：http://ogu.vehdjk.com

[U79] PHP：静态分析
来源：http://pgi.guannengcc.top

composer require --dev phpstan/phpstan
来源：http://zcd.zycfv.cn

[U80] PHP：代码规范修复
来源：http://zim.svipenyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://iss.haohaochexian.top

[U81] JS：初始化项目
来源：http://utq.jinyuanbaomall.cn

npm init -y;  npm i express
来源：http://vpy.chenzaomai.com

[U82] JS：package.json 脚本
来源：http://wdg.ybcxt.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://asw.bjfxy.top

[U83] JS：ES Module 导入导出
来源：http://qei.shuidangran.top

export const a = 1;  import { a } from "./m.js";
来源：http://xuu.zhiwuduotai.top

[U84] JS：CommonJS 写法
来源：http://ehx.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://wbm.fzhhl.top

[U85] JS：可选链
来源：http://foy.bjfxy.top

a?.b?.c
来源：http://fmb.fehbvm.com

[U86] JS：空值合并
来源：http://zgu.wangdashe.top

a ?? b
来源：http://xfx.shangyingyoupin.top

[U87] JS：解构默认值
来源：http://byb.tianlin.xyz

const { a = 1, b = 2 } = obj;
来源：http://xyf.zhengqikj.top

[U88] JS：对象展开合并
来源：http://iai.haohaochexian.top

{ ...a, ...b }
来源：http://cwn.svipenyu.cn

[U89] JS：数组去重
来源：http://qxu.52xcode.cn

[...new Set(arr)]
来源：http://qxc.shanyushiyangtech.top

[U90] JS：数字数组排序
来源：http://vpb.jinyuanbaomall.cn

[...arr].sort((a, b) => a - b)
来源：http://ekc.zhixingplan.top

[U91] JS：对象键值遍历
来源：http://ywb.shanyushiyangtech.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qna.zhengqikj.top

[U92] JS：深拷贝
来源：http://tog.zhijiandao.cn

structuredClone(obj)
来源：http://tqx.fehbvm.com

[U93] JS：模板字符串
来源：http://kzg.daria6918.cn

`共 ${n} 条`
来源：http://yur.fanxiaobao.xyz

[U94] JS：箭头函数
来源：http://rez.dianchejie.cn

const double = x => x * 2;
来源：http://ora.sysykeji.top

[U95] JS：Promise 包装
来源：http://mvf.jinqigufen.top

new Promise((resolve, reject) => {})
来源：http://ini.nanxinkj.top

[U96] JS：async/await 与异常
来源：http://abp.meibo888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mqg.feifeiyinyue.top

[U97] JS：并发请求
来源：http://nkz.zhongyouzk.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://knm.dashuyun.cn

[U98] JS：fetch 带 JSON
来源：http://gdi.hywenlv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://njh.snrcjt.cn

[U99] JS：事件监听
来源：http://kyo.shzxlz.cn

el.addEventListener("click", e => {})
来源：http://shm.zhixingplan.top

[U100] JS：DOM 查询
来源：http://psc.fehbvm.com

document.querySelector(".item")
来源：http://xdu.hongshengwenyu.top

[U101] JS：classList 操作
来源：http://yue.cdnleiting.top

el.classList.toggle("active")
来源：http://nkx.hnxiangtu.top

[U102] JS：本地存储
来源：http://zzd.52xcode.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nsv.jinqigufen.top

[U103] JS：定时器
来源：http://htu.cheryme.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xtw.ivvv.top

[U104] JS：防抖
来源：http://hgn.dianchejie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dvm.jlsjyb.cn

[U105] JS：节流
来源：http://kzo.cucudq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dfo.hesvh.cn

[U106] JS：日期格式化
来源：http://kly.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://obf.jqgufenzy.top

[U107] JS：数字千分位
来源：http://lgv.sweek.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vdq.tanke756.top

[U108] JS：随机整数
来源：http://dll.yonumen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rqi.zhengqikj.top

[U109] JS：数组分组
来源：http://lyo.yongpay.top

Object.groupBy(arr, x => x.type)
来源：http://rkd.jqgfzy.top

[U110] JS：数组分块
来源：http://vbf.haohaochexian.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rvo.cqqwz.cn

[U111] JS：对象转 Map
来源：http://ljr.daxiang520.top

new Map(Object.entries(obj))
来源：http://wxx.ivvv.top

[U112] JS：字符串补位
来源：http://eij.hammf.cn

"7".padStart(3, "0")
来源：http://qhn.iojbl.cn

[U113] JS：正则替换全部
来源：http://emc.pycfn.com

s.replaceAll("a", "b")
来源：http://wif.ctjpmb.com

[U114] JS：JSON 深比较
来源：http://azl.bjfxy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dma.cucudq.cn

[U115] JS：生成 UUID
来源：http://jpo.xziqi.cn

crypto.randomUUID()
来源：http://nop.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://pkg.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://pwa.meibo888.top

[U117] JS：单元测试
来源：http://edy.svipenyu.cn

npm i -D vitest;  npx vitest
来源：http://hjj.fzhhl.top

[U118] JS：开发服务器
来源：http://xvp.guowangkeji.top

npm i -D vite;  npx vite
来源：http://odv.gogol.net.cn

[U119] JS：生产构建
来源：http://dve.jinqigfzy.top

npx vite build
来源：http://wqf.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://xwa.gogol.net.cn

import.meta.env.VITE_API_URL
来源：http://vzw.jqgufenzy.top

================================================================================
来源：http://pgx.nanxuanxn.top

统计汇总
来源：http://xkw.xingfuxueyuan.xyz

================================================================================
来源：http://cwz.daria6918.cn

按语言统计（条）：
来源：http://pwr.yj202588.top

Python ......... 252
来源：http://ypi.redwolf501.top

PHP ............ 252
来源：http://sia.nanxuanxn.top

JavaScript ..... 252
来源：http://jma.wangshuangyany.cn

TypeScript ..... 212
来源：http://jnj.wangdashe.top

Java ........... 212
来源：http://hgz.hnxiangtu.top

Go ............. 212
来源：http://exy.snrcjt.cn

Ruby ........... 212
来源：http://ufl.yuanzhike.top

C# ............. 212
来源：http://cpr.sweek.top

C .............. 30
来源：http://cxl.dashuyun.cn

C++ ............ 30
来源：http://wmx.fzhhl.top

SQL ............ 90
来源：http://ttx.c1oappe.top

Bash ........... 80
来源：http://fge.zhiwuduotai.top

Kotlin ......... 15
来源：http://cut.andypj.xyz

Swift .......... 15
来源：http://ylv.gaohongyu789.top

Lua ............ 10
来源：http://ahw.nanxinkj.top

Perl ........... 10
来源：http://hki.jlsjyb.cn

Scala .......... 10
来源：http://rto.chenlongwang.top

------------------------------------
来源：http://fcj.xziqi.cn

合计 ........... 2106 条
来源：http://pul.iojbl.cn

按章节统计：
来源：http://tqa.guannengcc.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ego.redwolf501.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eug.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jvv.316326.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ghi.cucudq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qiq.ehwqpu.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ske.wangdashe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rwh.ywan-chungtsiang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qja.xuanzx.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://krk.aibaodan.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cuq.shanyushiyangtech.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gyz.pycfn.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qkb.uphjek.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zci.zhengqikj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tac.tarul.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yre.hcnkem.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://boz.ydzc1.top

Q SQL 专题                              90
来源：http://qov.epnwcf.com

R Bash 专题                             80
来源：http://iza.jqgfzy.top

S C / C++ 专题                          60
来源：http://lmq.0kj1m.cn

T 其他语言补充                          60
来源：http://yxz.fengsongda.top

U 高频实用片段                         120
来源：http://poz.jinyuanbaomall.cn

------------------------------------
来源：http://kck.jinyuanbaomall.cn

合计                                  2106 条
来源：http://zmn.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://xey.xuetiantiany.cn

使用提醒
来源：http://hwf.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://rab.jqgufenzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xrv.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hfm.quarkkingdee.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iiz.ehwqpu.com

在旧版本上使用前请先确认语法支持情况。
来源：http://uld.fehbvm.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ufw.andypj.xyz

—— 文件结束 ——
来源：http://eih.cheryme.top

================================================================================
来源：http://lio.zdbjq.cn

程序语言常见例子速查手册（2024 版）
来源：http://yxx.0kj1m.cn

Common Programming Examples Cheat Book
来源：http://pgf.fktsv.cn

================================================================================
来源：http://xvn.zhixingplan.top

【收录内容】
来源：http://gft.uphjek.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ytk.hysaishi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vzh.yj20258.top

SQL · Bash · C · C++
来源：http://vhl.tian-w.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baq.ctjpmb.com

【使用说明】
来源：http://qiz.feifeiyinyue.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vrk.epnwcf.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uaa.cucudq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eia.shanyushiyangtech.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qay.ywan-chungtsiang.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zzz.xuanzx.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dww.yvedp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yja.bjfxy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nor.tarul.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://psa.jqgfzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ozi.52xcode.cn


<!-- 参考信息 -->