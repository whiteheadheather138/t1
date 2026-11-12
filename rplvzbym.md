代发 wailian999

[U07] Py：反转字典键值
来源：http://rac.hongshengwenyu.top

{v: k for k, v in d.items()}
来源：http://ion.snrcjt.cn

[U08] Py：展平二维列表
来源：http://mae.quarkkingdee.top

[y for x in nested for y in x]
来源：http://iug.zhongyouzk.top

[U09] Py：字典取最大值的键
来源：http://gjp.svipenyu.cn

max(d, key=d.get)
来源：http://cfg.ehwqpu.com

[U10] Py：按值排序字典
来源：http://jji.fehbvm.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kvb.bjfxy.top

[U11] Py：生成器表达式
来源：http://bof.fehbvm.com

(x * 2 for x in arr)
来源：http://hwt.yangfankeji.com

[U12] Py：取出现最多的 3 个元素
来源：http://rus.zhaomingkeji.xyz

Counter(arr).most_common(3)
来源：http://mif.ehwqpu.com

[U13] Py：固定长度队列
来源：http://kie.tian-w.cn

deque(maxlen=10)
来源：http://kml.yuanzhike.top

[U14] Py：分组收集到列表
来源：http://gxm.zhiwuduotai.top

defaultdict(list)
来源：http://rdy.ydzc1.top

[U15] Py：高精度计时
来源：http://fvs.yvedp.cn

t = time.perf_counter()
来源：http://cdj.gotoacloud.top

[U16] Py：命令行参数解析
来源：http://cho.jinqigfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://otp.sweek.top

[U17] Py：初始化日志
来源：http://aum.redwolf501.top

logging.basicConfig(level=logging.INFO)
来源：http://zaz.xinyue.icu

[U18] Py：预编译正则
来源：http://nan.shzxlz.cn

pat = re.compile(r"\d+")
来源：http://atu.wangshuangyany.cn

[U19] Py：正则替换带回调
来源：http://jye.sufxvd.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tsr.xingfuxueyuan.xyz

[U20] Py：缓存函数结果
来源：http://myx.chenzaomai.com

@functools.lru_cache(maxsize=None)
来源：http://bzv.tanke756.top

[U21] Py：自定义上下文管理器
来源：http://rnh.vehdjk.com

@contextlib.contextmanager
来源：http://emo.wangdashe.top

[U22] Py：矩阵转置
来源：http://gxv.hongshengwenyu.top

list(zip(*m))
来源：http://eip.xingfuxueyuan.xyz

[U23] Py：分块读取大文件
来源：http://fwg.tian-w.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://umb.tarul.cn

[U24] Py：路径操作
来源：http://olz.zhengqikj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gjr.sxryk.cn

[U25] Py：CSV 按字典读
来源：http://bci.shangyingyoupin.top

csv.DictReader(f)
来源：http://frp.vehdjk.com

[U26] Py：并发下载
来源：http://gbp.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jke.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://pld.ywan-chungtsiang.top

aiohttp.ClientSession() 配合 async with
来源：http://vsj.yuanzhike.top

[U28] Py：类型别名
来源：http://nis.tanke756.top

UserId = int
来源：http://rag.hongshengwenyu.top

[U29] Py：属性校验
来源：http://imr.gotoacloud.top

@property 与 @x.setter 配合
来源：http://jcd.hnqzz.top

[U30] Py：数据类
来源：http://crf.epnwcf.com

@dataclass(slots=True)
来源：http://occ.uphjek.com

[U31] Py：单测
来源：http://lti.bjfxy.top

python -m pytest -q
来源：http://ssx.hcnkem.com

[U32] Py：代码格式化
来源：http://xhg.jiagoushi.top

ruff format . && ruff check --fix .
来源：http://dze.jinqigufen.top

[U33] Py：打包发布
来源：http://btx.52xcode.cn

python -m build  （依赖 pyproject.toml）
来源：http://jhj.sjlbkw.cn

[U34] Py：判断编码
来源：http://fdd.gaohongyu789.top

chardet.detect(raw)
来源：http://tdd.cashguo.top

[U35] Py：发送邮件
来源：http://jds.yfazqb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gsx.ybcxt.top

[U36] Py：定时任务
来源：http://zen.fktsv.cn

schedule.every(10).minutes.do(job)
来源：http://cdk.ppjwa.cn

[U37] Py：读写 Excel
来源：http://zri.wangshuangyany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yqt.shanyushiyangkeji.top

[U38] Py：获取脚本所在目录
来源：http://bpc.ehwqpu.com

Path(__file__).resolve().parent
来源：http://fxi.cdnleiting.top

[U39] Py：判断是否在交互环境
来源：http://bha.bjfxy.top

sys.stdout.isatty()
来源：http://gwk.pycfn.com

[U40] Py：打印到标准错误
来源：http://igz.vehdjk.com

print("err", file=sys.stderr)
来源：http://usn.birdmap.top

[U41] PHP：初始化 Composer 项目
来源：http://rfg.ydjk.org.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yba.guowangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://kzz.c1oappe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hti.aibaodan.cn

[U43] PHP：声明命名空间
来源：http://iwl.andypj.xyz

namespace App\Http;
来源：http://rqg.shzxlz.cn

[U44] PHP：开启严格类型
来源：http://tkl.smart0.xyz

declare(strict_types=1);
来源：http://mja.ydzc1.top

[U45] PHP：类型声明与返回类型
来源：http://rqo.xinyue.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://wpq.redwolf501.top

[U46] PHP：可空类型
来源：http://mle.hnxiangtu.top

?string $name = null
来源：http://erz.yongpay.top

[U47] PHP：联合类型
来源：http://dib.fanxiaobao.xyz

int|string $id
来源：http://prd.sweek.top

[U48] PHP：纯枚举
来源：http://jve.52xcode.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://flc.zhiwuduotai.top

[U49] PHP：只读属性
来源：http://yur.zhiwuduotai.top

public readonly string $name
来源：http://npj.xuanzx.com

[U50] PHP：构造器属性提升
来源：http://eah.hnxiangtu.top

public function __construct(private int $id) {}
来源：http://oer.svipenyu.cn

[U51] PHP：数组解构
来源：http://bji.hongshengwenyu.top

[$a, $b] = $arr;
来源：http://kde.hesvh.cn

[U52] PHP：箭头函数
来源：http://xie.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://qav.hnqzz.top

[U53] PHP：空合并运算符
来源：http://obl.sysykeji.top

$v = $a ?? $b ?? "default";
来源：http://qrw.yongpay.top

[U54] PHP：空安全调用
来源：http://ysg.yfazqb.com

$obj?->method()
来源：http://fdf.cucudq.cn

[U55] PHP：match 表达式
来源：http://zwk.ywan-chungtsiang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mhu.gzhubu.top

[U56] PHP：命名参数
来源：http://jaf.c1oappe.top

f(a: 1, b: 2)
来源：http://pxr.aibaodan.cn

[U57] PHP：字符串插值
来源：http://udi.gzhubu.top

"值: {$a}"
来源：http://ouw.zdqjudy.top

[U58] PHP：数组三件套
来源：http://dgy.jinqigufen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zle.xuanzx.com

[U59] PHP：自定义排序
来源：http://zhm.hfpthk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eoi.smart0.xyz

[U60] PHP：JSON 编解码
来源：http://xvx.jqgufenzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bet.xylfe.cn

[U61] PHP：正则
来源：http://rbq.yuxming.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sok.chenlongwang.top

[U62] PHP：日期对象
来源：http://vhg.dashuyun.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gzo.yj20258888.top

[U63] PHP：文件读写
来源：http://igj.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wif.sjlbkw.cn

[U64] PHP：目录遍历
来源：http://xoa.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://fvv.ydzc1.top

[U65] PHP：会话
来源：http://ozo.chenlongwang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://npp.haohaochexian.top

[U66] PHP：设置 Cookie
来源：http://yxk.jlsjyb.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zrn.hesvh.cn

[U67] PHP：处理文件上传
来源：http://ynf.shanyushiyangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xwe.jinghuilouyu.cn

[U68] PHP：PDO 连接
来源：http://ywy.ppjwa.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dnb.dashuyun.cn

[U69] PHP：PDO 预处理
来源：http://vhg.guannengcc.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eum.snrcjt.cn

[U70] PHP：PDO 事务
来源：http://vsw.ctjpmb.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://haa.dianchejie.cn

[U71] PHP：抛出异常
来源：http://uef.sjlbkw.cn

throw new RuntimeException("失败", 500);
来源：http://vsj.sysykeji.top

[U72] PHP：写错误日志
来源：http://qob.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://dkd.yj20258.top

[U73] PHP：读取 ini 配置
来源：http://kkg.yangfankeji.com

parse_ini_file("config.ini", true)
来源：http://kdp.jinyuanbaomall.cn

[U74] PHP：读取环境变量
来源：http://cpp.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://pti.zhoulong.xyz

[U75] PHP：依赖注入
来源：http://wmk.ctjpmb.com

composer require psr/container
来源：http://ncl.cqqwz.cn

[U76] PHP：简单路由
来源：http://anh.havefunace.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qre.c1oappe.top

[U77] PHP：模板渲染
来源：http://wxl.tianlin.xyz

composer require twig/twig
来源：http://ozr.hongshengwenyu.top

[U78] PHP：单元测试
来源：http://rxa.ctjpmb.com

composer require --dev phpunit/phpunit
来源：http://ftf.zhijiandao.cn

[U79] PHP：静态分析
来源：http://ypc.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://ufm.sjlbkw.cn

[U80] PHP：代码规范修复
来源：http://koy.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bak.sysykeji.top

[U81] JS：初始化项目
来源：http://uek.zhoulong.xyz

npm init -y;  npm i express
来源：http://zrt.nanxinkj.top

[U82] JS：package.json 脚本
来源：http://iwu.hnxiangtu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xws.tanke756.top

[U83] JS：ES Module 导入导出
来源：http://zgx.daria6918.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ucy.feifeiyinyue.top

[U84] JS：CommonJS 写法
来源：http://scd.xylfe.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nnf.xylfe.cn

[U85] JS：可选链
来源：http://qau.wangdashe.top

a?.b?.c
来源：http://jrf.yfazqb.com

[U86] JS：空值合并
来源：http://bwg.xingfuxueyuan.xyz

a ?? b
来源：http://icy.xuetiantiany.cn

[U87] JS：解构默认值
来源：http://kmw.haohaochexian.top

const { a = 1, b = 2 } = obj;
来源：http://mpi.ydzc1.top

[U88] JS：对象展开合并
来源：http://fza.jinyuanbaomall.cn

{ ...a, ...b }
来源：http://wsu.hesvh.cn

[U89] JS：数组去重
来源：http://ugg.fanxiaobao.xyz

[...new Set(arr)]
来源：http://elq.hammf.cn

[U90] JS：数字数组排序
来源：http://qpi.meibo888.top

[...arr].sort((a, b) => a - b)
来源：http://lsq.yj20258.top

[U91] JS：对象键值遍历
来源：http://lky.birdmap.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pgk.yonumen.top

[U92] JS：深拷贝
来源：http://udo.haohaochexian.top

structuredClone(obj)
来源：http://dbq.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://slf.ywan-chungtsiang.top

`共 ${n} 条`
来源：http://tpv.yangfankeji.com

[U94] JS：箭头函数
来源：http://jhn.sysykeji.top

const double = x => x * 2;
来源：http://mhb.jinqigufen.top

[U95] JS：Promise 包装
来源：http://usd.hnqzz.top

new Promise((resolve, reject) => {})
来源：http://nck.zhaomingkeji.xyz

[U96] JS：async/await 与异常
来源：http://vbj.hammf.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://avf.yongpay.top

[U97] JS：并发请求
来源：http://qnr.hnxiangtu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mkc.fanxiaobao.xyz

[U98] JS：fetch 带 JSON
来源：http://vsi.gzhubu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rjw.sjlbkw.cn

[U99] JS：事件监听
来源：http://khd.zhongyouzk.top

el.addEventListener("click", e => {})
来源：http://fbk.jqgfzy.top

[U100] JS：DOM 查询
来源：http://asu.jlsjyb.cn

document.querySelector(".item")
来源：http://bsk.fktsv.cn

[U101] JS：classList 操作
来源：http://imj.zhoulong.xyz

el.classList.toggle("active")
来源：http://ebs.316326.xyz

[U102] JS：本地存储
来源：http://gtb.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rnr.yueranfly.top

[U103] JS：定时器
来源：http://llw.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jvr.hesvh.cn

[U104] JS：防抖
来源：http://lra.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ace.zycfv.cn

[U105] JS：节流
来源：http://kjc.redwolf501.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lmd.quarkkingdee.top

[U106] JS：日期格式化
来源：http://hoi.quarkkingdee.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://usv.snrcjt.cn

[U107] JS：数字千分位
来源：http://nwt.yonumen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yig.uphjek.com

[U108] JS：随机整数
来源：http://fkq.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jkx.gogol.net.cn

[U109] JS：数组分组
来源：http://dmh.cucudq.cn

Object.groupBy(arr, x => x.type)
来源：http://qmu.mhx1999.top

[U110] JS：数组分块
来源：http://mrj.fehbvm.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qjc.yanxiufei.cn

[U111] JS：对象转 Map
来源：http://tca.ywan-chungtsiang.top

new Map(Object.entries(obj))
来源：http://khg.yuanzhike.top

[U112] JS：字符串补位
来源：http://cvo.redwolf501.top

"7".padStart(3, "0")
来源：http://rvt.xylfe.cn

[U113] JS：正则替换全部
来源：http://cqx.zhongyouzk.top

s.replaceAll("a", "b")
来源：http://ohi.dashuyun.cn

[U114] JS：JSON 深比较
来源：http://fvc.ehwqpu.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://frr.iojbl.cn

[U115] JS：生成 UUID
来源：http://gtl.yongpay.top

crypto.randomUUID()
来源：http://fpw.ydjk.org.cn

[U116] JS：类型检查（JSDoc）
来源：http://coz.yangfankeji.com

/** @param {string} name */ function f(name) {}
来源：http://cvc.sjlbkw.cn

[U117] JS：单元测试
来源：http://zxl.pycfn.com

npm i -D vitest;  npx vitest
来源：http://bxw.yongpay.top

[U118] JS：开发服务器
来源：http://mmx.daria6918.cn

npm i -D vite;  npx vite
来源：http://jgg.sjlbkw.cn

[U119] JS：生产构建
来源：http://cbi.wangshuangyany.cn

npx vite build
来源：http://pcy.nanxinkj.top

[U120] JS：读取环境变量（Vite）
来源：http://akh.tianlin.xyz

import.meta.env.VITE_API_URL
来源：http://usk.yuxming.cn

================================================================================
来源：http://twj.cucudq.cn

统计汇总
来源：http://unc.fktsv.cn

================================================================================
来源：http://gtn.c1oappe.top

按语言统计（条）：
来源：http://kxh.epnwcf.com

Python ......... 252
来源：http://rsk.yj20258888.top

PHP ............ 252
来源：http://ibm.chenzaomai.com

JavaScript ..... 252
来源：http://isn.fzhhl.top

TypeScript ..... 212
来源：http://ovx.ywan-chungtsiang.top

Java ........... 212
来源：http://ypw.yuanzhike.top

Go ............. 212
来源：http://tgd.sysykeji.top

Ruby ........... 212
来源：http://xzr.zhijiandao.cn

C# ............. 212
来源：http://uwd.zhaomingkeji.xyz

C .............. 30
来源：http://bwf.mhx1999.top

C++ ............ 30
来源：http://ult.jinghuilouyu.cn

SQL ............ 90
来源：http://vfq.fengsongda.top

Bash ........... 80
来源：http://wjp.bbcook.cn

Kotlin ......... 15
来源：http://grj.nanxinkj.top

Swift .......... 15
来源：http://gas.iojbl.cn

Lua ............ 10
来源：http://udi.sysykeji.top

Perl ........... 10
来源：http://jht.tianlin.xyz

Scala .......... 10
来源：http://qss.9152youxi.cn

------------------------------------
来源：http://hmm.birdmap.top

合计 ........... 2106 条
来源：http://dyr.gotoacloud.top

按章节统计：
来源：http://bxe.jinyuanbaomall.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bbk.svipenyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://idi.sjlbkw.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jtn.c1oappe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rsw.zhengqikj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jzw.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ict.iojbl.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iui.mhx1999.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mzb.shanyushiyangtech.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qqt.yuanzhike.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://avd.dashuyun.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hpp.yj20258.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rug.quarkkingdee.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://srs.ppjwa.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bgv.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mdw.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dgx.zdqjudy.top

Q SQL 专题                              90
来源：http://vbu.hysaishi.cn

R Bash 专题                             80
来源：http://lox.hnxiangtu.top

S C / C++ 专题                          60
来源：http://dur.52xcode.cn

T 其他语言补充                          60
来源：http://yhs.xinyue.icu

U 高频实用片段                         120
来源：http://jiu.xingfuxueyuan.xyz

------------------------------------
来源：http://yuq.fanxiaobao.xyz

合计                                  2106 条
来源：http://osv.fktsv.cn

--------------------------------------------------------------------------------
来源：http://fbl.yuanzhike.top

使用提醒
来源：http://ptj.daxiang520.top

--------------------------------------------------------------------------------
来源：http://ont.shanyushiyangtech.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://krf.cqqwz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vum.jqgfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wjk.jianghu66.top

在旧版本上使用前请先确认语法支持情况。
来源：http://igf.shanyushiyangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zrr.jyoumei.cn

—— 文件结束 ——
来源：http://jac.jinqigfzy.top

================================================================================
来源：http://yrs.hammf.cn

程序语言常见例子速查手册（2024 版）
来源：http://rbr.aibaodan.cn

Common Programming Examples Cheat Book
来源：http://scs.nanxinkj.top

================================================================================
来源：http://gqu.ydzc1.top

【收录内容】
来源：http://rbb.aizwys.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zfc.zhixingplan.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tgh.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://bsm.9152youxi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yan.yfazqb.com

【使用说明】
来源：http://iss.9152youxi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://emk.yj20258.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wwo.fengsongda.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vqt.nwbrower.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qrn.hywenlv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gby.jinyuanbaomall.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gkf.ydzc1.top


<!-- 参考信息 -->