代发 wailian999

[U07] Py：反转字典键值
来源：http://fir.zhoulong.xyz

{v: k for k, v in d.items()}
来源：http://qxb.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://ilv.ybcxt.top

[y for x in nested for y in x]
来源：http://feb.pengpengdd.cyou

[U09] Py：字典取最大值的键
来源：http://kzi.snrcjt.cn

max(d, key=d.get)
来源：http://uxv.snrcjt.cn

[U10] Py：按值排序字典
来源：http://rhq.tanke756.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://euz.tianlin.xyz

[U11] Py：生成器表达式
来源：http://zvv.tanke756.top

(x * 2 for x in arr)
来源：http://vgu.xylfe.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ujp.xylfe.cn

Counter(arr).most_common(3)
来源：http://zwb.cqqwz.cn

[U13] Py：固定长度队列
来源：http://grh.hnxiangtu.top

deque(maxlen=10)
来源：http://zmo.wangshuangyany.cn

[U14] Py：分组收集到列表
来源：http://ahw.xingfuxueyuan.xyz

defaultdict(list)
来源：http://qug.aibaodan.cn

[U15] Py：高精度计时
来源：http://rxz.jinghuilouyu.cn

t = time.perf_counter()
来源：http://bzv.yj20258888.top

[U16] Py：命令行参数解析
来源：http://qcl.haohaochexian.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jwq.vqdsnc.cn

[U17] Py：初始化日志
来源：http://aka.meibo888.top

logging.basicConfig(level=logging.INFO)
来源：http://ned.yueranfly.top

[U18] Py：预编译正则
来源：http://vam.hnqzz.top

pat = re.compile(r"\d+")
来源：http://rrj.guannengcc.top

[U19] Py：正则替换带回调
来源：http://zjq.yanxiufei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bzg.xylfe.cn

[U20] Py：缓存函数结果
来源：http://dee.zhaomingkeji.xyz

@functools.lru_cache(maxsize=None)
来源：http://vec.daxiang520.top

[U21] Py：自定义上下文管理器
来源：http://yuk.ppjwa.cn

@contextlib.contextmanager
来源：http://wqn.chenzaomai.com

[U22] Py：矩阵转置
来源：http://srb.haohaochexian.top

list(zip(*m))
来源：http://kfi.yj202588.top

[U23] Py：分块读取大文件
来源：http://ywr.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sfh.zycfv.cn

[U24] Py：路径操作
来源：http://uyj.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xjw.sjlbkw.cn

[U25] Py：CSV 按字典读
来源：http://fdi.jlsjyb.cn

csv.DictReader(f)
来源：http://tnr.yfazqb.com

[U26] Py：并发下载
来源：http://wgi.ppjwa.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xxr.zhiwuduotai.top

[U27] Py：异步 HTTP
来源：http://isa.hammf.cn

aiohttp.ClientSession() 配合 async with
来源：http://ywj.sjlbkw.cn

[U28] Py：类型别名
来源：http://ggc.shanyushiyangtech.top

UserId = int
来源：http://fhn.52xcode.cn

[U29] Py：属性校验
来源：http://mdf.yj202588.top

@property 与 @x.setter 配合
来源：http://dof.ehwqpu.com

[U30] Py：数据类
来源：http://xvv.yvedp.cn

@dataclass(slots=True)
来源：http://bzl.hesvh.cn

[U31] Py：单测
来源：http://max.tanke756.top

python -m pytest -q
来源：http://zdm.hywenlv.cn

[U32] Py：代码格式化
来源：http://cwr.fanxiaobao.xyz

ruff format . && ruff check --fix .
来源：http://zqt.kuanghao11.cn

[U33] Py：打包发布
来源：http://bfd.zhongyouzk.top

python -m build  （依赖 pyproject.toml）
来源：http://grc.xylfe.cn

[U34] Py：判断编码
来源：http://kal.cdnleiting.top

chardet.detect(raw)
来源：http://ops.vehdjk.com

[U35] Py：发送邮件
来源：http://gbu.jqgufenzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sac.cheryme.top

[U36] Py：定时任务
来源：http://zgl.yongpay.top

schedule.every(10).minutes.do(job)
来源：http://ieb.fzhhl.top

[U37] Py：读写 Excel
来源：http://tdr.aizwys.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kwk.xingfuxueyuan.xyz

[U38] Py：获取脚本所在目录
来源：http://vow.cqqwz.cn

Path(__file__).resolve().parent
来源：http://xip.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://ksm.ywan-chungtsiang.top

sys.stdout.isatty()
来源：http://fxf.hnxiangtu.top

[U40] Py：打印到标准错误
来源：http://lxk.snrcjt.cn

print("err", file=sys.stderr)
来源：http://paj.52xcode.cn

[U41] PHP：初始化 Composer 项目
来源：http://prx.guannengcc.top

composer init;  composer require guzzlehttp/guzzle
来源：http://myz.haohaochexian.top

[U42] PHP：PSR-4 自动加载
来源：http://rar.redwolf501.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rfz.pycfn.com

[U43] PHP：声明命名空间
来源：http://yas.yj20258888.top

namespace App\Http;
来源：http://cuz.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://eus.jinqigfzy.top

declare(strict_types=1);
来源：http://alp.mhx1999.top

[U45] PHP：类型声明与返回类型
来源：http://rff.shanyushiyangtech.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yfe.ivvv.top

[U46] PHP：可空类型
来源：http://aiy.xuanzx.com

?string $name = null
来源：http://ukg.cucudq.cn

[U47] PHP：联合类型
来源：http://wjg.zdbjq.cn

int|string $id
来源：http://vtd.yuxming.cn

[U48] PHP：纯枚举
来源：http://aoq.ivvv.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fad.chenjidiqi.icu

[U49] PHP：只读属性
来源：http://wly.epnwcf.com

public readonly string $name
来源：http://els.haohaochexian.top

[U50] PHP：构造器属性提升
来源：http://txd.shanyushiyangkeji.top

public function __construct(private int $id) {}
来源：http://gju.gotoacloud.top

[U51] PHP：数组解构
来源：http://xax.chenlongwang.top

[$a, $b] = $arr;
来源：http://brc.feifeiyinyue.top

[U52] PHP：箭头函数
来源：http://qlx.sjlbkw.cn

$double = fn($x) => $x * 2;
来源：http://vdt.yangfankeji.com

[U53] PHP：空合并运算符
来源：http://rgd.sxryk.cn

$v = $a ?? $b ?? "default";
来源：http://hen.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://mms.aizwys.cn

$obj?->method()
来源：http://rnc.hnqzz.top

[U55] PHP：match 表达式
来源：http://vqh.xuetiantiany.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rnx.ivvv.top

[U56] PHP：命名参数
来源：http://uwb.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://toi.xuanzx.com

[U57] PHP：字符串插值
来源：http://vrk.zhaomingkeji.xyz

"值: {$a}"
来源：http://hul.uphjek.com

[U58] PHP：数组三件套
来源：http://fen.cdnleiting.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dum.shanyushiyangkeji.top

[U59] PHP：自定义排序
来源：http://ddy.fehbvm.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ylk.bbcook.cn

[U60] PHP：JSON 编解码
来源：http://xtu.nwbrower.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://muf.tian-w.cn

[U61] PHP：正则
来源：http://kak.hnqzz.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://itu.9152youxi.cn

[U62] PHP：日期对象
来源：http://dez.aibaodan.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nhi.ywan-chungtsiang.top

[U63] PHP：文件读写
来源：http://akx.hfpthk.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ytk.shanyushiyangkeji.top

[U64] PHP：目录遍历
来源：http://opn.c1oappe.top

glob("dir/*.php");  scandir("dir");
来源：http://tka.shanyushiyangtech.top

[U65] PHP：会话
来源：http://dbq.daxiang520.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xsk.ehwqpu.com

[U66] PHP：设置 Cookie
来源：http://atr.jyoumei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ktd.xinyue.icu

[U67] PHP：处理文件上传
来源：http://hec.yuxming.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wjn.cucudq.cn

[U68] PHP：PDO 连接
来源：http://mro.fzhhl.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://npw.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://usn.nwbrower.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qvu.bbcook.cn

[U70] PHP：PDO 事务
来源：http://fub.jiagoushi.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xwp.daxiang520.top

[U71] PHP：抛出异常
来源：http://kek.jinyuanbaomall.cn

throw new RuntimeException("失败", 500);
来源：http://bjl.tanke756.top

[U72] PHP：写错误日志
来源：http://gsx.jianghu66.top

error_log("失败: " . $e->getMessage());
来源：http://fmg.nwbrower.top

[U73] PHP：读取 ini 配置
来源：http://rfl.zdbjq.cn

parse_ini_file("config.ini", true)
来源：http://ysz.hongshengwenyu.top

[U74] PHP：读取环境变量
来源：http://wkp.yuxming.cn

getenv("APP_ENV") ?: "production"
来源：http://uvf.zhijiandao.cn

[U75] PHP：依赖注入
来源：http://zzs.nanxuanxn.top

composer require psr/container
来源：http://sbx.hywenlv.cn

[U76] PHP：简单路由
来源：http://dvk.tianlin.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://avl.shangyingyoupin.top

[U77] PHP：模板渲染
来源：http://qhe.ivvv.top

composer require twig/twig
来源：http://dpy.zycfv.cn

[U78] PHP：单元测试
来源：http://hgi.hongshengwenyu.top

composer require --dev phpunit/phpunit
来源：http://inf.quarkkingdee.top

[U79] PHP：静态分析
来源：http://bkg.shzxlz.cn

composer require --dev phpstan/phpstan
来源：http://uga.yfazqb.com

[U80] PHP：代码规范修复
来源：http://rmr.zdqjudy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nux.nanxinkj.top

[U81] JS：初始化项目
来源：http://sfx.zycfv.cn

npm init -y;  npm i express
来源：http://xpr.316326.xyz

[U82] JS：package.json 脚本
来源：http://mah.shangyingyoupin.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lns.andypj.xyz

[U83] JS：ES Module 导入导出
来源：http://dqt.andypj.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://lyi.jinqigufen.top

[U84] JS：CommonJS 写法
来源：http://ujt.svipenyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uxb.andypj.xyz

[U85] JS：可选链
来源：http://ygb.cdnleiting.top

a?.b?.c
来源：http://fzx.ivvv.top

[U86] JS：空值合并
来源：http://gim.zdqjudy.top

a ?? b
来源：http://dwx.fehbvm.com

[U87] JS：解构默认值
来源：http://wqy.haohaochexian.top

const { a = 1, b = 2 } = obj;
来源：http://dcl.yuanzhike.top

[U88] JS：对象展开合并
来源：http://laz.kuanghao11.cn

{ ...a, ...b }
来源：http://uyz.yangfankeji.com

[U89] JS：数组去重
来源：http://qxs.sufxvd.cn

[...new Set(arr)]
来源：http://ohc.dashuyun.cn

[U90] JS：数字数组排序
来源：http://spr.meibo888.top

[...arr].sort((a, b) => a - b)
来源：http://jej.zhaomingkeji.xyz

[U91] JS：对象键值遍历
来源：http://ftr.svipenyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pjt.jinyuanbaomall.cn

[U92] JS：深拷贝
来源：http://nbu.chenjidiqi.icu

structuredClone(obj)
来源：http://nku.tian-w.cn

[U93] JS：模板字符串
来源：http://arb.daxiang520.top

`共 ${n} 条`
来源：http://ncr.zhiwuduotai.top

[U94] JS：箭头函数
来源：http://vit.fzhhl.top

const double = x => x * 2;
来源：http://geo.tanke756.top

[U95] JS：Promise 包装
来源：http://jky.chenlongwang.top

new Promise((resolve, reject) => {})
来源：http://mvy.feifeiyinyue.top

[U96] JS：async/await 与异常
来源：http://dqw.hfpthk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iry.316326.xyz

[U97] JS：并发请求
来源：http://qeb.xylfe.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hjy.uphjek.com

[U98] JS：fetch 带 JSON
来源：http://ppa.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xbs.nanxuanxn.top

[U99] JS：事件监听
来源：http://myf.kuanghao11.cn

el.addEventListener("click", e => {})
来源：http://vlt.jlsjyb.cn

[U100] JS：DOM 查询
来源：http://wva.jqgufenzy.top

document.querySelector(".item")
来源：http://dmg.havefunace.top

[U101] JS：classList 操作
来源：http://omj.sweek.top

el.classList.toggle("active")
来源：http://uax.epnwcf.com

[U102] JS：本地存储
来源：http://yqf.jinqigufen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://afa.ctjpmb.com

[U103] JS：定时器
来源：http://pii.sjlbkw.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yzv.quarkkingdee.top

[U104] JS：防抖
来源：http://tsz.sjlbkw.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wie.gogol.net.cn

[U105] JS：节流
来源：http://auq.sysykeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xxm.gogol.net.cn

[U106] JS：日期格式化
来源：http://lao.hammf.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gum.yonumen.top

[U107] JS：数字千分位
来源：http://omw.gogol.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vxd.fzhhl.top

[U108] JS：随机整数
来源：http://xrn.xuanzx.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://idu.redwolf501.top

[U109] JS：数组分组
来源：http://pru.jinghuilouyu.cn

Object.groupBy(arr, x => x.type)
来源：http://ozb.yueranfly.top

[U110] JS：数组分块
来源：http://jku.aibaodan.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ftk.hysaishi.cn

[U111] JS：对象转 Map
来源：http://nsr.cucudq.cn

new Map(Object.entries(obj))
来源：http://cog.zhengqikj.top

[U112] JS：字符串补位
来源：http://asj.ywan-chungtsiang.top

"7".padStart(3, "0")
来源：http://kxy.cdnleiting.top

[U113] JS：正则替换全部
来源：http://lsu.hywenlv.cn

s.replaceAll("a", "b")
来源：http://uxm.jyoumei.cn

[U114] JS：JSON 深比较
来源：http://vmp.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://svn.zhoulong.xyz

[U115] JS：生成 UUID
来源：http://bkl.zhengqikj.top

crypto.randomUUID()
来源：http://wfm.andypj.xyz

[U116] JS：类型检查（JSDoc）
来源：http://rri.c1oappe.top

/** @param {string} name */ function f(name) {}
来源：http://mbg.yanxiufei.cn

[U117] JS：单元测试
来源：http://uaq.vehdjk.com

npm i -D vitest;  npx vitest
来源：http://qee.haohaochexian.top

[U118] JS：开发服务器
来源：http://hxj.cheryme.top

npm i -D vite;  npx vite
来源：http://hne.vqdsnc.cn

[U119] JS：生产构建
来源：http://cbd.sufxvd.cn

npx vite build
来源：http://vjk.ydzc1.top

[U120] JS：读取环境变量（Vite）
来源：http://stg.nwbrower.top

import.meta.env.VITE_API_URL
来源：http://jdp.yanxiufei.cn

================================================================================
来源：http://krp.gotoacloud.top

统计汇总
来源：http://ixg.yvedp.cn

================================================================================
来源：http://ret.vehdjk.com

按语言统计（条）：
来源：http://beb.wangdashe.top

Python ......... 252
来源：http://fpw.52xcode.cn

PHP ............ 252
来源：http://rwu.snrcjt.cn

JavaScript ..... 252
来源：http://zio.yanxiufei.cn

TypeScript ..... 212
来源：http://wti.52xcode.cn

Java ........... 212
来源：http://kvs.jinqigfzy.top

Go ............. 212
来源：http://oua.tianlin.xyz

Ruby ........... 212
来源：http://lan.yfazqb.com

C# ............. 212
来源：http://jyb.yfazqb.com

C .............. 30
来源：http://vnk.ywan-chungtsiang.top

C++ ............ 30
来源：http://wga.yj202588.top

SQL ............ 90
来源：http://hnt.52xcode.cn

Bash ........... 80
来源：http://ytb.ywan-chungtsiang.top

Kotlin ......... 15
来源：http://yhs.haohaochexian.top

Swift .......... 15
来源：http://vuz.cashguo.top

Lua ............ 10
来源：http://dqi.iojbl.cn

Perl ........... 10
来源：http://mha.zhijiandao.cn

Scala .......... 10
来源：http://xhr.sweek.top

------------------------------------
来源：http://mbd.smart0.xyz

合计 ........... 2106 条
来源：http://fmr.yuxming.cn

按章节统计：
来源：http://kcp.yj20258888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gxx.cashguo.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uky.fehbvm.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://txv.aizwys.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lrv.xingfuxueyuan.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qnf.jqgufenzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hai.ydzc1.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kvn.yfazqb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rvn.quarkkingdee.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jzi.yueranfly.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lau.ppjwa.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gps.zhiwuduotai.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zhj.yuanzhike.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hil.fzhhl.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ept.redwolf501.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://foi.zhiwuduotai.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ygl.gaohongyu789.top

Q SQL 专题                              90
来源：http://wnw.xuanzx.com

R Bash 专题                             80
来源：http://ufd.zhengqikj.top

S C / C++ 专题                          60
来源：http://ooq.ybcxt.top

T 其他语言补充                          60
来源：http://dhs.sweek.top

U 高频实用片段                         120
来源：http://mjf.sweek.top

------------------------------------
来源：http://lcz.yuxming.cn

合计                                  2106 条
来源：http://jkb.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://kfh.hesvh.cn

使用提醒
来源：http://wig.ybcxt.top

--------------------------------------------------------------------------------
来源：http://eab.jinqigfzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ril.dianchejie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tpl.dianchejie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eud.zdbjq.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zvk.zhaomingkeji.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vyz.birdmap.top

—— 文件结束 ——
来源：http://hxb.sufxvd.cn

================================================================================
来源：http://rdj.jqgfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://mkh.tian-w.cn

Common Programming Examples Cheat Book
来源：http://qwm.bbcook.cn

================================================================================
来源：http://aej.epnwcf.com

【收录内容】
来源：http://ris.hnxiangtu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bqp.meibo888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://udp.yuanzhike.top

SQL · Bash · C · C++
来源：http://tmr.uphjek.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ntd.yfazqb.com

【使用说明】
来源：http://sqf.aibaodan.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xcr.kuanghao11.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ypj.bbcook.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iln.fzhhl.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ijb.meibo888.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lgz.daxiang520.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xal.smart0.xyz


<!-- 参考信息 -->