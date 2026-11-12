代发 wailian999

[U05] Py：列表去重且保序
来源：http://gew.9152youxi.cn

list(dict.fromkeys(arr))
来源：http://aje.hnxiangtu.top

[U06] Py：合并两个字典
来源：http://tzw.fehbvm.com

{**a, **b}
来源：http://qch.jqgufenzy.top

[U07] Py：反转字典键值
来源：http://meb.daxiang520.top

{v: k for k, v in d.items()}
来源：http://xtt.sufxvd.cn

[U08] Py：展平二维列表
来源：http://stk.haohaochexian.top

[y for x in nested for y in x]
来源：http://whs.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://sud.kuanghao11.cn

max(d, key=d.get)
来源：http://khi.andypj.xyz

[U10] Py：按值排序字典
来源：http://yuw.dianchejie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dcr.sufxvd.cn

[U11] Py：生成器表达式
来源：http://bpb.ppjwa.cn

(x * 2 for x in arr)
来源：http://ydn.hywenlv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jkj.aibaodan.cn

Counter(arr).most_common(3)
来源：http://xqe.redwolf501.top

[U13] Py：固定长度队列
来源：http://ygc.nanxinkj.top

deque(maxlen=10)
来源：http://npa.andypj.xyz

[U14] Py：分组收集到列表
来源：http://rmi.hnxiangtu.top

defaultdict(list)
来源：http://fuk.fanxiaobao.xyz

[U15] Py：高精度计时
来源：http://bqz.hysaishi.cn

t = time.perf_counter()
来源：http://muu.zhoulong.xyz

[U16] Py：命令行参数解析
来源：http://lzd.smart0.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bie.ywan-chungtsiang.top

[U17] Py：初始化日志
来源：http://bkl.xziqi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ncw.jiagoushi.top

[U18] Py：预编译正则
来源：http://iye.zhoulong.xyz

pat = re.compile(r"\d+")
来源：http://sjc.52xcode.cn

[U19] Py：正则替换带回调
来源：http://jnn.gzhubu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lqc.gaohongyu789.top

[U20] Py：缓存函数结果
来源：http://mnz.vqdsnc.cn

@functools.lru_cache(maxsize=None)
来源：http://hrp.jinqigfzy.top

[U21] Py：自定义上下文管理器
来源：http://wkz.andypj.xyz

@contextlib.contextmanager
来源：http://dya.xziqi.cn

[U22] Py：矩阵转置
来源：http://wkd.tanke756.top

list(zip(*m))
来源：http://iya.9152youxi.cn

[U23] Py：分块读取大文件
来源：http://wqh.zdqjudy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://roc.guannengcc.top

[U24] Py：路径操作
来源：http://jol.fanxiaobao.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lcb.dashuyun.cn

[U25] Py：CSV 按字典读
来源：http://wkp.sxryk.cn

csv.DictReader(f)
来源：http://hvt.haohaochexian.top

[U26] Py：并发下载
来源：http://dxz.shzxlz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xwx.52xcode.cn

[U27] Py：异步 HTTP
来源：http://bju.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://mzm.hywenlv.cn

[U28] Py：类型别名
来源：http://coh.ydzc1.top

UserId = int
来源：http://wrd.yj20258.top

[U29] Py：属性校验
来源：http://ofo.hysaishi.cn

@property 与 @x.setter 配合
来源：http://qhw.vqdsnc.cn

[U30] Py：数据类
来源：http://uwx.ybcxt.top

@dataclass(slots=True)
来源：http://hsw.xingfuxueyuan.xyz

[U31] Py：单测
来源：http://xjs.vehdjk.com

python -m pytest -q
来源：http://iir.shanyushiyangtech.top

[U32] Py：代码格式化
来源：http://rwy.hysaishi.cn

ruff format . && ruff check --fix .
来源：http://xnh.feifeiyinyue.top

[U33] Py：打包发布
来源：http://tob.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://jqq.mhx1999.top

[U34] Py：判断编码
来源：http://axk.jqgufenzy.top

chardet.detect(raw)
来源：http://vvj.gaohongyu789.top

[U35] Py：发送邮件
来源：http://och.yj202588.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hse.52xcode.cn

[U36] Py：定时任务
来源：http://day.yongpay.top

schedule.every(10).minutes.do(job)
来源：http://wrx.cqqwz.cn

[U37] Py：读写 Excel
来源：http://irr.zhixingplan.top

pandas.read_excel / DataFrame.to_excel
来源：http://wqc.xuetiantiany.cn

[U38] Py：获取脚本所在目录
来源：http://xqp.yj20258888.top

Path(__file__).resolve().parent
来源：http://ofz.jyoumei.cn

[U39] Py：判断是否在交互环境
来源：http://oti.yj202588.top

sys.stdout.isatty()
来源：http://psj.ydzc1.top

[U40] Py：打印到标准错误
来源：http://nxo.sufxvd.cn

print("err", file=sys.stderr)
来源：http://jci.xziqi.cn

[U41] PHP：初始化 Composer 项目
来源：http://hbw.jinyuanbaomall.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://chx.yuanzhike.top

[U42] PHP：PSR-4 自动加载
来源：http://pmu.zdqjudy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xsp.shangyingyoupin.top

[U43] PHP：声明命名空间
来源：http://flm.mhx1999.top

namespace App\Http;
来源：http://iyz.havefunace.top

[U44] PHP：开启严格类型
来源：http://xxn.52xcode.cn

declare(strict_types=1);
来源：http://ytr.c1oappe.top

[U45] PHP：类型声明与返回类型
来源：http://fsm.jiagoushi.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://dsn.gotoacloud.top

[U46] PHP：可空类型
来源：http://sjz.fzhhl.top

?string $name = null
来源：http://tsf.tarul.cn

[U47] PHP：联合类型
来源：http://akh.yfazqb.com

int|string $id
来源：http://nov.9152youxi.cn

[U48] PHP：纯枚举
来源：http://agx.vehdjk.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gzr.cashguo.top

[U49] PHP：只读属性
来源：http://ahv.xuanzx.com

public readonly string $name
来源：http://lyb.ybcxt.top

[U50] PHP：构造器属性提升
来源：http://kgs.316326.xyz

public function __construct(private int $id) {}
来源：http://tfd.jinghuilouyu.cn

[U51] PHP：数组解构
来源：http://wgi.jinqigufen.top

[$a, $b] = $arr;
来源：http://czg.ybcxt.top

[U52] PHP：箭头函数
来源：http://vci.ydzc1.top

$double = fn($x) => $x * 2;
来源：http://vkk.c1oappe.top

[U53] PHP：空合并运算符
来源：http://tve.cashguo.top

$v = $a ?? $b ?? "default";
来源：http://owu.ivvv.top

[U54] PHP：空安全调用
来源：http://pzz.svipenyu.cn

$obj?->method()
来源：http://bsv.meibo888.top

[U55] PHP：match 表达式
来源：http://vac.jyoumei.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jxr.sjlbkw.cn

[U56] PHP：命名参数
来源：http://lfy.ehwqpu.com

f(a: 1, b: 2)
来源：http://cdd.zhaomingkeji.xyz

[U57] PHP：字符串插值
来源：http://nwa.ydjk.org.cn

"值: {$a}"
来源：http://bzc.xingfuxueyuan.xyz

[U58] PHP：数组三件套
来源：http://gqa.yj20258888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zjf.yvedp.cn

[U59] PHP：自定义排序
来源：http://wxk.gzhubu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pls.fengsongda.top

[U60] PHP：JSON 编解码
来源：http://iuc.hongshengwenyu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nho.yj20258.top

[U61] PHP：正则
来源：http://rzv.ppjwa.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ohm.hammf.cn

[U62] PHP：日期对象
来源：http://ltd.daria6918.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gcz.xingfuxueyuan.xyz

[U63] PHP：文件读写
来源：http://xbl.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kjb.daxiang520.top

[U64] PHP：目录遍历
来源：http://byi.yongpay.top

glob("dir/*.php");  scandir("dir");
来源：http://zte.haohaochexian.top

[U65] PHP：会话
来源：http://bsk.tarul.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://got.gaohongyu789.top

[U66] PHP：设置 Cookie
来源：http://tpe.chenjidiqi.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://elk.ywan-chungtsiang.top

[U67] PHP：处理文件上传
来源：http://sse.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://flv.cheryme.top

[U68] PHP：PDO 连接
来源：http://vtx.quarkkingdee.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zcz.xylfe.cn

[U69] PHP：PDO 预处理
来源：http://olw.fanxiaobao.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xbl.yuxming.cn

[U70] PHP：PDO 事务
来源：http://xev.birdmap.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gtt.nanxinkj.top

[U71] PHP：抛出异常
来源：http://iqb.sweek.top

throw new RuntimeException("失败", 500);
来源：http://tqn.sysykeji.top

[U72] PHP：写错误日志
来源：http://gta.gaohongyu789.top

error_log("失败: " . $e->getMessage());
来源：http://oqk.zdqjudy.top

[U73] PHP：读取 ini 配置
来源：http://fiq.bbcook.cn

parse_ini_file("config.ini", true)
来源：http://fqs.hnxiangtu.top

[U74] PHP：读取环境变量
来源：http://uup.hongshengwenyu.top

getenv("APP_ENV") ?: "production"
来源：http://rwj.xziqi.cn

[U75] PHP：依赖注入
来源：http://kgr.pengpengdd.cyou

composer require psr/container
来源：http://nmi.redwolf501.top

[U76] PHP：简单路由
来源：http://vgk.chenjidiqi.icu

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vgs.andypj.xyz

[U77] PHP：模板渲染
来源：http://iks.xuanzx.com

composer require twig/twig
来源：http://nnv.shanyushiyangtech.top

[U78] PHP：单元测试
来源：http://eon.yuanzhike.top

composer require --dev phpunit/phpunit
来源：http://uup.fanxiaobao.xyz

[U79] PHP：静态分析
来源：http://uie.nanxinkj.top

composer require --dev phpstan/phpstan
来源：http://rim.shangyingyoupin.top

[U80] PHP：代码规范修复
来源：http://wiq.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hhs.yfazqb.com

[U81] JS：初始化项目
来源：http://oiz.zhijiandao.cn

npm init -y;  npm i express
来源：http://shf.jianghu66.top

[U82] JS：package.json 脚本
来源：http://aqt.hcnkem.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://poy.xziqi.cn

[U83] JS：ES Module 导入导出
来源：http://xfd.vqdsnc.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hrp.chenlongwang.top

[U84] JS：CommonJS 写法
来源：http://vkg.jinyuanbaomall.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cpz.jiagoushi.top

[U85] JS：可选链
来源：http://uqa.ydjk.org.cn

a?.b?.c
来源：http://xuf.xuanzx.com

[U86] JS：空值合并
来源：http://ifg.fanxiaobao.xyz

a ?? b
来源：http://gxm.daria6918.cn

[U87] JS：解构默认值
来源：http://vul.gaohongyu789.top

const { a = 1, b = 2 } = obj;
来源：http://zlj.cqqwz.cn

[U88] JS：对象展开合并
来源：http://fje.zhongyouzk.top

{ ...a, ...b }
来源：http://mcz.jyoumei.cn

[U89] JS：数组去重
来源：http://dqh.ehwqpu.com

[...new Set(arr)]
来源：http://ttd.ctjpmb.com

[U90] JS：数字数组排序
来源：http://ywg.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://lec.ehwqpu.com

[U91] JS：对象键值遍历
来源：http://ijo.gaohongyu789.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kww.yj20258888.top

[U92] JS：深拷贝
来源：http://efs.hesvh.cn

structuredClone(obj)
来源：http://wob.epnwcf.com

[U93] JS：模板字符串
来源：http://oeg.yangfankeji.com

`共 ${n} 条`
来源：http://hfe.ehwqpu.com

[U94] JS：箭头函数
来源：http://wgn.zhaomingkeji.xyz

const double = x => x * 2;
来源：http://odf.fehbvm.com

[U95] JS：Promise 包装
来源：http://jso.gotoacloud.top

new Promise((resolve, reject) => {})
来源：http://uyz.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://rxh.gogol.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://omb.fktsv.cn

[U97] JS：并发请求
来源：http://dhr.jqgufenzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ryr.xuanzx.com

[U98] JS：fetch 带 JSON
来源：http://zzh.jlsjyb.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pvt.chenzaomai.com

[U99] JS：事件监听
来源：http://niy.zdqjudy.top

el.addEventListener("click", e => {})
来源：http://gez.hesvh.cn

[U100] JS：DOM 查询
来源：http://xml.yanxiufei.cn

document.querySelector(".item")
来源：http://dfy.gaohongyu789.top

[U101] JS：classList 操作
来源：http://yxb.jinqigufen.top

el.classList.toggle("active")
来源：http://gzq.haohaochexian.top

[U102] JS：本地存储
来源：http://xxe.sufxvd.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jnd.gotoacloud.top

[U103] JS：定时器
来源：http://hri.cdnleiting.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://drh.cqqwz.cn

[U104] JS：防抖
来源：http://pzo.birdmap.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ntc.vqdsnc.cn

[U105] JS：节流
来源：http://zbb.sxryk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tjs.dianchejie.cn

[U106] JS：日期格式化
来源：http://kwv.c1oappe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sup.fanxiaobao.xyz

[U107] JS：数字千分位
来源：http://ejl.vqdsnc.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nbg.zhixingplan.top

[U108] JS：随机整数
来源：http://bht.jyoumei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cio.smart0.xyz

[U109] JS：数组分组
来源：http://mig.ppjwa.cn

Object.groupBy(arr, x => x.type)
来源：http://npy.ydjk.org.cn

[U110] JS：数组分块
来源：http://qpv.xylfe.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wyn.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://gov.svipenyu.cn

new Map(Object.entries(obj))
来源：http://zlh.andypj.xyz

[U112] JS：字符串补位
来源：http://nlr.yj202588.top

"7".padStart(3, "0")
来源：http://ele.xinyue.icu

[U113] JS：正则替换全部
来源：http://stm.vqdsnc.cn

s.replaceAll("a", "b")
来源：http://pph.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://waa.fehbvm.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ulz.epnwcf.com

[U115] JS：生成 UUID
来源：http://oom.gzhubu.top

crypto.randomUUID()
来源：http://wvv.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://ggt.guowangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://mif.tianlin.xyz

[U117] JS：单元测试
来源：http://kyi.hcnkem.com

npm i -D vitest;  npx vitest
来源：http://wve.jinyuanbaomall.cn

[U118] JS：开发服务器
来源：http://rqs.sysykeji.top

npm i -D vite;  npx vite
来源：http://ujd.fktsv.cn

[U119] JS：生产构建
来源：http://wfk.yfazqb.com

npx vite build
来源：http://nia.cqqwz.cn

[U120] JS：读取环境变量（Vite）
来源：http://nwq.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://yod.guannengcc.top

================================================================================
来源：http://fec.cheryme.top

统计汇总
来源：http://btw.jinqigfzy.top

================================================================================
来源：http://qvx.c1oappe.top

按语言统计（条）：
来源：http://qbt.ehwqpu.com

Python ......... 252
来源：http://zav.cheryme.top

PHP ............ 252
来源：http://qzc.jinqigufen.top

JavaScript ..... 252
来源：http://fca.chenjidiqi.icu

TypeScript ..... 212
来源：http://unv.zhongyouzk.top

Java ........... 212
来源：http://tvf.yuxming.cn

Go ............. 212
来源：http://zbv.vehdjk.com

Ruby ........... 212
来源：http://zsm.nwbrower.top

C# ............. 212
来源：http://xen.birdmap.top

C .............. 30
来源：http://rlb.jianghu66.top

C++ ............ 30
来源：http://ndq.zhijiandao.cn

SQL ............ 90
来源：http://syb.jqgufenzy.top

Bash ........... 80
来源：http://vzj.sxryk.cn

Kotlin ......... 15
来源：http://ujo.fengsongda.top

Swift .......... 15
来源：http://agf.cheryme.top

Lua ............ 10
来源：http://kkd.sweek.top

Perl ........... 10
来源：http://fcd.xuetiantiany.cn

Scala .......... 10
来源：http://wzz.uphjek.com

------------------------------------
来源：http://fce.52xcode.cn

合计 ........... 2106 条
来源：http://ndh.xinyue.icu

按章节统计：
来源：http://ahc.ywan-chungtsiang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zpb.hesvh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ixs.smart0.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://utv.snrcjt.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zmc.guannengcc.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://czd.daria6918.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lob.birdmap.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kkv.gogol.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vnl.svipenyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oxn.xinyue.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yzt.aibaodan.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tpt.jlsjyb.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ykp.jyoumei.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qfc.xuanzx.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uas.tian-w.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nvd.wangshuangyany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uyv.chenjidiqi.icu

Q SQL 专题                              90
来源：http://few.ctjpmb.com

R Bash 专题                             80
来源：http://vzu.jianghu66.top

S C / C++ 专题                          60
来源：http://jjm.hesvh.cn

T 其他语言补充                          60
来源：http://asv.zhoulong.xyz

U 高频实用片段                         120
来源：http://sdg.daria6918.cn

------------------------------------
来源：http://qoq.hysaishi.cn

合计                                  2106 条
来源：http://xjr.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://rbh.hnqzz.top

使用提醒
来源：http://enn.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://hzy.feifeiyinyue.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vhl.yuanzhike.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jls.hysaishi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://arc.ctjpmb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://ojn.kuanghao11.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pwc.pycfn.com

—— 文件结束 ——
来源：http://hly.hammf.cn

================================================================================
来源：http://iyl.daxiang520.top

程序语言常见例子速查手册（2024 版）
来源：http://qbh.zhiwuduotai.top

Common Programming Examples Cheat Book
来源：http://bft.jinghuilouyu.cn

================================================================================
来源：http://eta.vqdsnc.cn

【收录内容】
来源：http://vmd.wangshuangyany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bnr.jinqigfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bhj.gaohongyu789.top

SQL · Bash · C · C++
来源：http://tad.redwolf501.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://reu.9152youxi.cn

【使用说明】
来源：http://sqm.shangyingyoupin.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wpa.birdmap.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yxl.zhixingplan.top


<!-- 参考信息 -->