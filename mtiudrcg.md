代发 wailian999

[U05] Py：列表去重且保序
来源：http://mtu.iojbl.cn

list(dict.fromkeys(arr))
来源：http://hlk.gogol.net.cn

[U06] Py：合并两个字典
来源：http://uit.jinyuanbaomall.cn

{**a, **b}
来源：http://pry.yj202588.top

[U07] Py：反转字典键值
来源：http://uoq.ywan-chungtsiang.top

{v: k for k, v in d.items()}
来源：http://ivr.svipenyu.cn

[U08] Py：展平二维列表
来源：http://sza.ywan-chungtsiang.top

[y for x in nested for y in x]
来源：http://ysx.ydjk.org.cn

[U09] Py：字典取最大值的键
来源：http://fau.zhaomingkeji.xyz

max(d, key=d.get)
来源：http://lsz.tian-w.cn

[U10] Py：按值排序字典
来源：http://gdc.jinyuanbaomall.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zlx.gaohongyu789.top

[U11] Py：生成器表达式
来源：http://hjh.ivvv.top

(x * 2 for x in arr)
来源：http://yxl.yuanzhike.top

[U12] Py：取出现最多的 3 个元素
来源：http://zmv.316326.xyz

Counter(arr).most_common(3)
来源：http://qza.yuanzhike.top

[U13] Py：固定长度队列
来源：http://gdc.yangfankeji.com

deque(maxlen=10)
来源：http://ebe.nanxinkj.top

[U14] Py：分组收集到列表
来源：http://jcb.ywan-chungtsiang.top

defaultdict(list)
来源：http://ogh.ehwqpu.com

[U15] Py：高精度计时
来源：http://cpq.uphjek.com

t = time.perf_counter()
来源：http://vzd.jyoumei.cn

[U16] Py：命令行参数解析
来源：http://rfy.hfpthk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://coi.meibo888.top

[U17] Py：初始化日志
来源：http://dxt.yueranfly.top

logging.basicConfig(level=logging.INFO)
来源：http://zlb.jinqigufen.top

[U18] Py：预编译正则
来源：http://mce.vehdjk.com

pat = re.compile(r"\d+")
来源：http://hcp.cashguo.top

[U19] Py：正则替换带回调
来源：http://mjq.cheryme.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ull.yuxming.cn

[U20] Py：缓存函数结果
来源：http://bgy.shanyushiyangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://fep.ydjk.org.cn

[U21] Py：自定义上下文管理器
来源：http://atd.gzhubu.top

@contextlib.contextmanager
来源：http://wfb.ydjk.org.cn

[U22] Py：矩阵转置
来源：http://qws.daria6918.cn

list(zip(*m))
来源：http://ykl.jianghu66.top

[U23] Py：分块读取大文件
来源：http://jty.hysaishi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hmg.xylfe.cn

[U24] Py：路径操作
来源：http://eyl.fengsongda.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://snu.hammf.cn

[U25] Py：CSV 按字典读
来源：http://vrw.zhijiandao.cn

csv.DictReader(f)
来源：http://vtj.havefunace.top

[U26] Py：并发下载
来源：http://efd.hongshengwenyu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ghm.yongpay.top

[U27] Py：异步 HTTP
来源：http://bgh.nanxuanxn.top

aiohttp.ClientSession() 配合 async with
来源：http://ggb.sweek.top

[U28] Py：类型别名
来源：http://dov.gogol.net.cn

UserId = int
来源：http://vqi.hesvh.cn

[U29] Py：属性校验
来源：http://rqe.tarul.cn

@property 与 @x.setter 配合
来源：http://qlw.gogol.net.cn

[U30] Py：数据类
来源：http://flc.hnxiangtu.top

@dataclass(slots=True)
来源：http://eqd.zhengqikj.top

[U31] Py：单测
来源：http://fxo.zhijiandao.cn

python -m pytest -q
来源：http://rop.havefunace.top

[U32] Py：代码格式化
来源：http://uec.havefunace.top

ruff format . && ruff check --fix .
来源：http://ccg.zycfv.cn

[U33] Py：打包发布
来源：http://okv.hcnkem.com

python -m build  （依赖 pyproject.toml）
来源：http://tsn.yfazqb.com

[U34] Py：判断编码
来源：http://wut.zdqjudy.top

chardet.detect(raw)
来源：http://xsc.xingfuxueyuan.xyz

[U35] Py：发送邮件
来源：http://szi.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kyj.xylfe.cn

[U36] Py：定时任务
来源：http://tlf.tanke756.top

schedule.every(10).minutes.do(job)
来源：http://yxt.zhoulong.xyz

[U37] Py：读写 Excel
来源：http://utq.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://gkr.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://dkv.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://kpl.shzxlz.cn

[U39] Py：判断是否在交互环境
来源：http://sma.yongpay.top

sys.stdout.isatty()
来源：http://aar.jinghuilouyu.cn

[U40] Py：打印到标准错误
来源：http://fav.cucudq.cn

print("err", file=sys.stderr)
来源：http://bge.fengsongda.top

[U41] PHP：初始化 Composer 项目
来源：http://joe.hnxiangtu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pjc.zhongyouzk.top

[U42] PHP：PSR-4 自动加载
来源：http://yte.tian-w.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vbr.shzxlz.cn

[U43] PHP：声明命名空间
来源：http://cso.tianlin.xyz

namespace App\Http;
来源：http://ear.hysaishi.cn

[U44] PHP：开启严格类型
来源：http://pqi.ydzc1.top

declare(strict_types=1);
来源：http://hpv.shanyushiyangtech.top

[U45] PHP：类型声明与返回类型
来源：http://fhl.birdmap.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qip.c1oappe.top

[U46] PHP：可空类型
来源：http://hfd.yvedp.cn

?string $name = null
来源：http://frs.uphjek.com

[U47] PHP：联合类型
来源：http://fro.havefunace.top

int|string $id
来源：http://jov.wangshuangyany.cn

[U48] PHP：纯枚举
来源：http://epy.hnxiangtu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eep.xuetiantiany.cn

[U49] PHP：只读属性
来源：http://rze.daxiang520.top

public readonly string $name
来源：http://thy.hysaishi.cn

[U50] PHP：构造器属性提升
来源：http://stx.zycfv.cn

public function __construct(private int $id) {}
来源：http://uat.hammf.cn

[U51] PHP：数组解构
来源：http://hcs.daxiang520.top

[$a, $b] = $arr;
来源：http://wmo.gogol.net.cn

[U52] PHP：箭头函数
来源：http://hwh.wangdashe.top

$double = fn($x) => $x * 2;
来源：http://cvn.gotoacloud.top

[U53] PHP：空合并运算符
来源：http://sgt.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://jyj.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://jtv.sysykeji.top

$obj?->method()
来源：http://tbk.sufxvd.cn

[U55] PHP：match 表达式
来源：http://der.316326.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ils.zhixingplan.top

[U56] PHP：命名参数
来源：http://kcw.c1oappe.top

f(a: 1, b: 2)
来源：http://hrs.cheryme.top

[U57] PHP：字符串插值
来源：http://rwq.wangshuangyany.cn

"值: {$a}"
来源：http://eum.c1oappe.top

[U58] PHP：数组三件套
来源：http://zqf.hcnkem.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ngi.9152youxi.cn

[U59] PHP：自定义排序
来源：http://vee.iojbl.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mjj.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://suv.havefunace.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qwx.yueranfly.top

[U61] PHP：正则
来源：http://xvh.52xcode.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rwm.svipenyu.cn

[U62] PHP：日期对象
来源：http://sgb.yj20258.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iza.havefunace.top

[U63] PHP：文件读写
来源：http://hmf.guowangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hku.sweek.top

[U64] PHP：目录遍历
来源：http://ghb.bbcook.cn

glob("dir/*.php");  scandir("dir");
来源：http://srx.shanyushiyangtech.top

[U65] PHP：会话
来源：http://gbr.kuanghao11.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qvz.chenlongwang.top

[U66] PHP：设置 Cookie
来源：http://rql.yuanzhike.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jrc.jianghu66.top

[U67] PHP：处理文件上传
来源：http://cok.guowangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sgl.jinyuanbaomall.cn

[U68] PHP：PDO 连接
来源：http://iwq.shzxlz.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dvv.bjfxy.top

[U69] PHP：PDO 预处理
来源：http://awg.ybcxt.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cbd.gogol.net.cn

[U70] PHP：PDO 事务
来源：http://izq.gzhubu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://isn.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://xyl.zycfv.cn

throw new RuntimeException("失败", 500);
来源：http://zcu.316326.xyz

[U72] PHP：写错误日志
来源：http://jkk.zdqjudy.top

error_log("失败: " . $e->getMessage());
来源：http://zms.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://okx.jianghu66.top

parse_ini_file("config.ini", true)
来源：http://tek.gotoacloud.top

[U74] PHP：读取环境变量
来源：http://tiz.xziqi.cn

getenv("APP_ENV") ?: "production"
来源：http://tns.redwolf501.top

[U75] PHP：依赖注入
来源：http://zgi.havefunace.top

composer require psr/container
来源：http://sap.jlsjyb.cn

[U76] PHP：简单路由
来源：http://sqq.ivvv.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://unk.yj20258888.top

[U77] PHP：模板渲染
来源：http://cev.jqgfzy.top

composer require twig/twig
来源：http://uwo.xinyue.icu

[U78] PHP：单元测试
来源：http://eae.feifeiyinyue.top

composer require --dev phpunit/phpunit
来源：http://ydo.cashguo.top

[U79] PHP：静态分析
来源：http://nla.uphjek.com

composer require --dev phpstan/phpstan
来源：http://syh.cdnleiting.top

[U80] PHP：代码规范修复
来源：http://yke.fktsv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nnu.pengpengdd.cyou

[U81] JS：初始化项目
来源：http://tal.zdbjq.cn

npm init -y;  npm i express
来源：http://aow.ppjwa.cn

[U82] JS：package.json 脚本
来源：http://mdm.chenzaomai.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://npn.nwbrower.top

[U83] JS：ES Module 导入导出
来源：http://okh.zdqjudy.top

export const a = 1;  import { a } from "./m.js";
来源：http://cud.guannengcc.top

[U84] JS：CommonJS 写法
来源：http://aln.daria6918.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hkr.hnxiangtu.top

[U85] JS：可选链
来源：http://dyq.sjlbkw.cn

a?.b?.c
来源：http://obx.xingfuxueyuan.xyz

[U86] JS：空值合并
来源：http://zrr.jiagoushi.top

a ?? b
来源：http://uok.zdbjq.cn

[U87] JS：解构默认值
来源：http://ywd.aibaodan.cn

const { a = 1, b = 2 } = obj;
来源：http://urv.zhiwuduotai.top

[U88] JS：对象展开合并
来源：http://qkb.daria6918.cn

{ ...a, ...b }
来源：http://zas.ydzc1.top

[U89] JS：数组去重
来源：http://zus.haohaochexian.top

[...new Set(arr)]
来源：http://rbt.tanke756.top

[U90] JS：数字数组排序
来源：http://ieu.cucudq.cn

[...arr].sort((a, b) => a - b)
来源：http://htr.ybcxt.top

[U91] JS：对象键值遍历
来源：http://weo.ydjk.org.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kyo.zdbjq.cn

[U92] JS：深拷贝
来源：http://ibu.sufxvd.cn

structuredClone(obj)
来源：http://chg.hesvh.cn

[U93] JS：模板字符串
来源：http://uly.nanxinkj.top

`共 ${n} 条`
来源：http://kio.yvedp.cn

[U94] JS：箭头函数
来源：http://sfj.hfpthk.cn

const double = x => x * 2;
来源：http://pkr.zhengqikj.top

[U95] JS：Promise 包装
来源：http://eqp.ppjwa.cn

new Promise((resolve, reject) => {})
来源：http://cmk.aizwys.cn

[U96] JS：async/await 与异常
来源：http://ohs.xziqi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jef.aizwys.cn

[U97] JS：并发请求
来源：http://qcs.fanxiaobao.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://suz.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://qec.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hvb.aizwys.cn

[U99] JS：事件监听
来源：http://wop.fehbvm.com

el.addEventListener("click", e => {})
来源：http://xkg.zhixingplan.top

[U100] JS：DOM 查询
来源：http://gcd.shanyushiyangtech.top

document.querySelector(".item")
来源：http://zjx.ybcxt.top

[U101] JS：classList 操作
来源：http://hjm.havefunace.top

el.classList.toggle("active")
来源：http://uvt.ppjwa.cn

[U102] JS：本地存储
来源：http://xlo.fzhhl.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://aqv.sweek.top

[U103] JS：定时器
来源：http://udr.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gdd.bjfxy.top

[U104] JS：防抖
来源：http://zxh.ctjpmb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rok.nanxuanxn.top

[U105] JS：节流
来源：http://zou.9152youxi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hpl.yuanzhike.top

[U106] JS：日期格式化
来源：http://dis.fzhhl.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://umk.ywan-chungtsiang.top

[U107] JS：数字千分位
来源：http://xfa.aibaodan.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://flo.chenzaomai.com

[U108] JS：随机整数
来源：http://cfe.xingfuxueyuan.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nmz.uphjek.com

[U109] JS：数组分组
来源：http://jpm.feifeiyinyue.top

Object.groupBy(arr, x => x.type)
来源：http://fon.cheryme.top

[U110] JS：数组分块
来源：http://dub.epnwcf.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aej.gzhubu.top

[U111] JS：对象转 Map
来源：http://lem.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://pkr.hnxiangtu.top

[U112] JS：字符串补位
来源：http://osq.mhx1999.top

"7".padStart(3, "0")
来源：http://bkp.zhaomingkeji.xyz

[U113] JS：正则替换全部
来源：http://fyw.tarul.cn

s.replaceAll("a", "b")
来源：http://esw.redwolf501.top

[U114] JS：JSON 深比较
来源：http://jhm.zhengqikj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ixh.jlsjyb.cn

[U115] JS：生成 UUID
来源：http://wer.ehwqpu.com

crypto.randomUUID()
来源：http://qlk.yj20258888.top

[U116] JS：类型检查（JSDoc）
来源：http://odj.sjlbkw.cn

/** @param {string} name */ function f(name) {}
来源：http://eql.yfazqb.com

[U117] JS：单元测试
来源：http://qxn.tianlin.xyz

npm i -D vitest;  npx vitest
来源：http://vee.dianchejie.cn

[U118] JS：开发服务器
来源：http://doj.tarul.cn

npm i -D vite;  npx vite
来源：http://hhz.fehbvm.com

[U119] JS：生产构建
来源：http://dak.ydjk.org.cn

npx vite build
来源：http://jfe.vqdsnc.cn

[U120] JS：读取环境变量（Vite）
来源：http://oho.hongshengwenyu.top

import.meta.env.VITE_API_URL
来源：http://lxt.jlsjyb.cn

================================================================================
来源：http://yiz.shuidangran.top

统计汇总
来源：http://vyi.ppjwa.cn

================================================================================
来源：http://bix.jianghu66.top

按语言统计（条）：
来源：http://axh.zycfv.cn

Python ......... 252
来源：http://gbf.jyoumei.cn

PHP ............ 252
来源：http://mzo.fanxiaobao.xyz

JavaScript ..... 252
来源：http://nmp.zdqjudy.top

TypeScript ..... 212
来源：http://ycp.cucudq.cn

Java ........... 212
来源：http://zzh.pycfn.com

Go ............. 212
来源：http://tym.aibaodan.cn

Ruby ........... 212
来源：http://jvi.haohaochexian.top

C# ............. 212
来源：http://nzd.yanxiufei.cn

C .............. 30
来源：http://rbz.hnxiangtu.top

C++ ............ 30
来源：http://bmo.dianchejie.cn

SQL ............ 90
来源：http://dfy.mhx1999.top

Bash ........... 80
来源：http://ilb.sysykeji.top

Kotlin ......... 15
来源：http://mue.jinghuilouyu.cn

Swift .......... 15
来源：http://viv.hywenlv.cn

Lua ............ 10
来源：http://njt.aibaodan.cn

Perl ........... 10
来源：http://kby.pengpengdd.cyou

Scala .......... 10
来源：http://hac.cdnleiting.top

------------------------------------
来源：http://wdx.nanxinkj.top

合计 ........... 2106 条
来源：http://imo.birdmap.top

按章节统计：
来源：http://otq.hammf.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ivd.birdmap.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://btf.uphjek.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tby.yfazqb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yqm.bbcook.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gup.nanxinkj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://elz.zhaomingkeji.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yqp.shzxlz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uaj.cdnleiting.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sjk.daxiang520.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uki.ydzc1.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mjf.xingfuxueyuan.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rub.hcnkem.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nwt.jlsjyb.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bvt.shanyushiyangtech.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://var.jinghuilouyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dtf.zhengqikj.top

Q SQL 专题                              90
来源：http://mam.ppjwa.cn

R Bash 专题                             80
来源：http://hsw.bbcook.cn

S C / C++ 专题                          60
来源：http://eil.pycfn.com

T 其他语言补充                          60
来源：http://igf.meibo888.top

U 高频实用片段                         120
来源：http://yrp.jinqigufen.top

------------------------------------
来源：http://fex.cdnleiting.top

合计                                  2106 条
来源：http://qxa.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://ijl.hywenlv.cn

使用提醒
来源：http://ukj.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://mau.ydzc1.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ruw.316326.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ugm.sjlbkw.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dvh.fktsv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ibc.jinyuanbaomall.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pxl.nanxinkj.top

—— 文件结束 ——
来源：http://zgy.wangdashe.top

================================================================================
来源：http://xpe.kuanghao11.cn

程序语言常见例子速查手册（2024 版）
来源：http://kge.bjfxy.top

Common Programming Examples Cheat Book
来源：http://dwc.ctjpmb.com

================================================================================
来源：http://ogz.zhoulong.xyz

【收录内容】
来源：http://bqh.jinyuanbaomall.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jtv.sysykeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yis.bjfxy.top

SQL · Bash · C · C++
来源：http://zou.zdqjudy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nfv.iojbl.cn

【使用说明】
来源：http://qid.pycfn.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cka.hysaishi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tig.zdbjq.cn


<!-- 参考信息 -->