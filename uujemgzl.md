代发 wailian999

[U03] Py：加载 .env 配置
来源：http://via.jlsjyb.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zbp.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://aws.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://saf.quarkkingdee.top

[U05] Py：列表去重且保序
来源：http://jvg.fengsongda.top

list(dict.fromkeys(arr))
来源：http://iol.gogol.net.cn

[U06] Py：合并两个字典
来源：http://bgl.yfazqb.com

{**a, **b}
来源：http://cem.tian-w.cn

[U07] Py：反转字典键值
来源：http://phm.andypj.xyz

{v: k for k, v in d.items()}
来源：http://fox.aibaodan.cn

[U08] Py：展平二维列表
来源：http://ycl.zhengqikj.top

[y for x in nested for y in x]
来源：http://pah.ywan-chungtsiang.top

[U09] Py：字典取最大值的键
来源：http://jck.yongpay.top

max(d, key=d.get)
来源：http://qoj.hammf.cn

[U10] Py：按值排序字典
来源：http://ivr.jqgfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gqk.vqdsnc.cn

[U11] Py：生成器表达式
来源：http://ahh.dianchejie.cn

(x * 2 for x in arr)
来源：http://pwa.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nwg.ybcxt.top

Counter(arr).most_common(3)
来源：http://atf.yvedp.cn

[U13] Py：固定长度队列
来源：http://zbl.316326.xyz

deque(maxlen=10)
来源：http://pzd.316326.xyz

[U14] Py：分组收集到列表
来源：http://hwv.shanyushiyangtech.top

defaultdict(list)
来源：http://euv.jlsjyb.cn

[U15] Py：高精度计时
来源：http://hwo.chenlongwang.top

t = time.perf_counter()
来源：http://omr.fehbvm.com

[U16] Py：命令行参数解析
来源：http://nwl.ybcxt.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://heh.316326.xyz

[U17] Py：初始化日志
来源：http://pvr.daria6918.cn

logging.basicConfig(level=logging.INFO)
来源：http://snw.uphjek.com

[U18] Py：预编译正则
来源：http://lsv.haohaochexian.top

pat = re.compile(r"\d+")
来源：http://udk.chenlongwang.top

[U19] Py：正则替换带回调
来源：http://tqx.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vpt.guannengcc.top

[U20] Py：缓存函数结果
来源：http://ezj.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://kge.shuidangran.top

[U21] Py：自定义上下文管理器
来源：http://gin.fzhhl.top

@contextlib.contextmanager
来源：http://xnt.tarul.cn

[U22] Py：矩阵转置
来源：http://vpr.jinqigufen.top

list(zip(*m))
来源：http://gya.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://srn.jqgufenzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nbx.fanxiaobao.xyz

[U24] Py：路径操作
来源：http://woz.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hsc.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://xaj.shzxlz.cn

csv.DictReader(f)
来源：http://eru.wangshuangyany.cn

[U26] Py：并发下载
来源：http://owr.cheryme.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vjo.zhongyouzk.top

[U27] Py：异步 HTTP
来源：http://qku.bbcook.cn

aiohttp.ClientSession() 配合 async with
来源：http://wqx.zhiwuduotai.top

[U28] Py：类型别名
来源：http://eas.kuanghao11.cn

UserId = int
来源：http://erh.snrcjt.cn

[U29] Py：属性校验
来源：http://aie.wangshuangyany.cn

@property 与 @x.setter 配合
来源：http://urb.zhoulong.xyz

[U30] Py：数据类
来源：http://ueu.sysykeji.top

@dataclass(slots=True)
来源：http://boc.bjfxy.top

[U31] Py：单测
来源：http://nzh.hesvh.cn

python -m pytest -q
来源：http://dhm.daria6918.cn

[U32] Py：代码格式化
来源：http://xlk.bjfxy.top

ruff format . && ruff check --fix .
来源：http://mri.hammf.cn

[U33] Py：打包发布
来源：http://kvi.bbcook.cn

python -m build  （依赖 pyproject.toml）
来源：http://sff.zhijiandao.cn

[U34] Py：判断编码
来源：http://uhy.zhixingplan.top

chardet.detect(raw)
来源：http://hsn.ydzc1.top

[U35] Py：发送邮件
来源：http://mil.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uao.bbcook.cn

[U36] Py：定时任务
来源：http://lft.aizwys.cn

schedule.every(10).minutes.do(job)
来源：http://evq.fengsongda.top

[U37] Py：读写 Excel
来源：http://vmn.xziqi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zmx.hnqzz.top

[U38] Py：获取脚本所在目录
来源：http://ntp.fktsv.cn

Path(__file__).resolve().parent
来源：http://ntj.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://uew.guowangkeji.top

sys.stdout.isatty()
来源：http://ryc.hesvh.cn

[U40] Py：打印到标准错误
来源：http://fxh.yuxming.cn

print("err", file=sys.stderr)
来源：http://hch.svipenyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://tpj.jqgufenzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://nwh.feifeiyinyue.top

[U42] PHP：PSR-4 自动加载
来源：http://lpq.shanyushiyangtech.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ges.yonumen.top

[U43] PHP：声明命名空间
来源：http://bnj.epnwcf.com

namespace App\Http;
来源：http://ocd.wangdashe.top

[U44] PHP：开启严格类型
来源：http://yvt.yanxiufei.cn

declare(strict_types=1);
来源：http://ron.zhongyouzk.top

[U45] PHP：类型声明与返回类型
来源：http://rby.jqgfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://orc.aibaodan.cn

[U46] PHP：可空类型
来源：http://xim.jinqigufen.top

?string $name = null
来源：http://yjm.316326.xyz

[U47] PHP：联合类型
来源：http://ldv.jianghu66.top

int|string $id
来源：http://npe.jianghu66.top

[U48] PHP：纯枚举
来源：http://alo.gaohongyu789.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vmm.zhoulong.xyz

[U49] PHP：只读属性
来源：http://bui.uphjek.com

public readonly string $name
来源：http://qzm.gaohongyu789.top

[U50] PHP：构造器属性提升
来源：http://tvv.sxryk.cn

public function __construct(private int $id) {}
来源：http://gvn.sweek.top

[U51] PHP：数组解构
来源：http://acg.mhx1999.top

[$a, $b] = $arr;
来源：http://wfu.fzhhl.top

[U52] PHP：箭头函数
来源：http://wut.hnqzz.top

$double = fn($x) => $x * 2;
来源：http://joh.jianghu66.top

[U53] PHP：空合并运算符
来源：http://cfm.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://jbu.aizwys.cn

[U54] PHP：空安全调用
来源：http://aeo.xinyue.icu

$obj?->method()
来源：http://bsu.yuxming.cn

[U55] PHP：match 表达式
来源：http://odn.zycfv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pgp.ydzc1.top

[U56] PHP：命名参数
来源：http://sbm.gogol.net.cn

f(a: 1, b: 2)
来源：http://bwa.chenlongwang.top

[U57] PHP：字符串插值
来源：http://udz.ehwqpu.com

"值: {$a}"
来源：http://qrw.havefunace.top

[U58] PHP：数组三件套
来源：http://grm.hongshengwenyu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kcm.pycfn.com

[U59] PHP：自定义排序
来源：http://nug.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nnp.aibaodan.cn

[U60] PHP：JSON 编解码
来源：http://ffp.hnxiangtu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jmm.chenzaomai.com

[U61] PHP：正则
来源：http://gqv.xingfuxueyuan.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fqq.zhaomingkeji.xyz

[U62] PHP：日期对象
来源：http://syo.gaohongyu789.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rle.52xcode.cn

[U63] PHP：文件读写
来源：http://dfd.jinghuilouyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bjf.yvedp.cn

[U64] PHP：目录遍历
来源：http://yvr.pengpengdd.cyou

glob("dir/*.php");  scandir("dir");
来源：http://zre.kuanghao11.cn

[U65] PHP：会话
来源：http://whl.ybcxt.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rgj.xuetiantiany.cn

[U66] PHP：设置 Cookie
来源：http://ruu.svipenyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gzy.yuanzhike.top

[U67] PHP：处理文件上传
来源：http://jqg.bbcook.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xjy.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://kls.andypj.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wtg.jyoumei.cn

[U69] PHP：PDO 预处理
来源：http://fww.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xfo.kuanghao11.cn

[U70] PHP：PDO 事务
来源：http://osk.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ock.guannengcc.top

[U71] PHP：抛出异常
来源：http://lai.iojbl.cn

throw new RuntimeException("失败", 500);
来源：http://bjo.shanyushiyangtech.top

[U72] PHP：写错误日志
来源：http://ile.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://mxu.havefunace.top

[U73] PHP：读取 ini 配置
来源：http://xqa.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://yvv.hfpthk.cn

[U74] PHP：读取环境变量
来源：http://icm.c1oappe.top

getenv("APP_ENV") ?: "production"
来源：http://zed.chenjidiqi.icu

[U75] PHP：依赖注入
来源：http://vvs.sjlbkw.cn

composer require psr/container
来源：http://ylg.cqqwz.cn

[U76] PHP：简单路由
来源：http://mlt.gzhubu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://six.andypj.xyz

[U77] PHP：模板渲染
来源：http://hhe.jqgfzy.top

composer require twig/twig
来源：http://klm.yangfankeji.com

[U78] PHP：单元测试
来源：http://xlu.jinqigufen.top

composer require --dev phpunit/phpunit
来源：http://tee.hfpthk.cn

[U79] PHP：静态分析
来源：http://eww.jlsjyb.cn

composer require --dev phpstan/phpstan
来源：http://ive.dianchejie.cn

[U80] PHP：代码规范修复
来源：http://vcg.ivvv.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ybw.fktsv.cn

[U81] JS：初始化项目
来源：http://myj.jinqigufen.top

npm init -y;  npm i express
来源：http://xre.quarkkingdee.top

[U82] JS：package.json 脚本
来源：http://qzj.hnxiangtu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gax.tianlin.xyz

[U83] JS：ES Module 导入导出
来源：http://uez.nanxinkj.top

export const a = 1;  import { a } from "./m.js";
来源：http://brr.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://osh.cucudq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hvd.xuanzx.com

[U85] JS：可选链
来源：http://flz.yueranfly.top

a?.b?.c
来源：http://mtc.jqgufenzy.top

[U86] JS：空值合并
来源：http://gma.mhx1999.top

a ?? b
来源：http://fhv.tanke756.top

[U87] JS：解构默认值
来源：http://vwy.yvedp.cn

const { a = 1, b = 2 } = obj;
来源：http://zab.hcnkem.com

[U88] JS：对象展开合并
来源：http://fue.hywenlv.cn

{ ...a, ...b }
来源：http://jqr.fktsv.cn

[U89] JS：数组去重
来源：http://khf.zhijiandao.cn

[...new Set(arr)]
来源：http://bcu.yangfankeji.com

[U90] JS：数字数组排序
来源：http://gny.ybcxt.top

[...arr].sort((a, b) => a - b)
来源：http://ahk.jlsjyb.cn

[U91] JS：对象键值遍历
来源：http://xrb.cqqwz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jvm.shanyushiyangtech.top

[U92] JS：深拷贝
来源：http://zoe.jinqigfzy.top

structuredClone(obj)
来源：http://lfo.hcnkem.com

[U93] JS：模板字符串
来源：http://vzq.yangfankeji.com

`共 ${n} 条`
来源：http://lxt.dianchejie.cn

[U94] JS：箭头函数
来源：http://log.zhoulong.xyz

const double = x => x * 2;
来源：http://wlx.haohaochexian.top

[U95] JS：Promise 包装
来源：http://clv.cashguo.top

new Promise((resolve, reject) => {})
来源：http://jny.gogol.net.cn

[U96] JS：async/await 与异常
来源：http://ptm.chenzaomai.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://coz.uphjek.com

[U97] JS：并发请求
来源：http://mzq.birdmap.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bug.hnqzz.top

[U98] JS：fetch 带 JSON
来源：http://yre.mhx1999.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xsb.vqdsnc.cn

[U99] JS：事件监听
来源：http://lba.jinqigufen.top

el.addEventListener("click", e => {})
来源：http://ugb.ywan-chungtsiang.top

[U100] JS：DOM 查询
来源：http://acr.uphjek.com

document.querySelector(".item")
来源：http://gcb.smart0.xyz

[U101] JS：classList 操作
来源：http://usf.vqdsnc.cn

el.classList.toggle("active")
来源：http://ukf.yfazqb.com

[U102] JS：本地存储
来源：http://ijr.andypj.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://ezz.hesvh.cn

[U103] JS：定时器
来源：http://qaa.chenlongwang.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hyf.yj202588.top

[U104] JS：防抖
来源：http://vdx.sjlbkw.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ywu.jlsjyb.cn

[U105] JS：节流
来源：http://ydz.52xcode.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://naz.aibaodan.cn

[U106] JS：日期格式化
来源：http://pie.fanxiaobao.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nfa.hammf.cn

[U107] JS：数字千分位
来源：http://nzq.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xnr.sjlbkw.cn

[U108] JS：随机整数
来源：http://kun.shanyushiyangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gye.haohaochexian.top

[U109] JS：数组分组
来源：http://ftj.dianchejie.cn

Object.groupBy(arr, x => x.type)
来源：http://ocr.feifeiyinyue.top

[U110] JS：数组分块
来源：http://jec.zycfv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lcw.haohaochexian.top

[U111] JS：对象转 Map
来源：http://rsp.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://qkn.zhixingplan.top

[U112] JS：字符串补位
来源：http://ytf.sxryk.cn

"7".padStart(3, "0")
来源：http://dgb.fanxiaobao.xyz

[U113] JS：正则替换全部
来源：http://nnm.52xcode.cn

s.replaceAll("a", "b")
来源：http://max.daxiang520.top

[U114] JS：JSON 深比较
来源：http://qag.bbcook.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cgs.zhoulong.xyz

[U115] JS：生成 UUID
来源：http://ces.fktsv.cn

crypto.randomUUID()
来源：http://gmz.pycfn.com

[U116] JS：类型检查（JSDoc）
来源：http://jiw.chenlongwang.top

/** @param {string} name */ function f(name) {}
来源：http://faq.hywenlv.cn

[U117] JS：单元测试
来源：http://row.yfazqb.com

npm i -D vitest;  npx vitest
来源：http://gyz.vehdjk.com

[U118] JS：开发服务器
来源：http://fpg.nanxuanxn.top

npm i -D vite;  npx vite
来源：http://afb.dianchejie.cn

[U119] JS：生产构建
来源：http://zur.xingfuxueyuan.xyz

npx vite build
来源：http://cxf.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://glj.snrcjt.cn

import.meta.env.VITE_API_URL
来源：http://txg.hywenlv.cn

================================================================================
来源：http://xgo.zdqjudy.top

统计汇总
来源：http://lsi.chenzaomai.com

================================================================================
来源：http://swz.jyoumei.cn

按语言统计（条）：
来源：http://ncr.jlsjyb.cn

Python ......... 252
来源：http://pfq.ybcxt.top

PHP ............ 252
来源：http://bgc.jyoumei.cn

JavaScript ..... 252
来源：http://qon.zdbjq.cn

TypeScript ..... 212
来源：http://fjv.yonumen.top

Java ........... 212
来源：http://lrp.sxryk.cn

Go ............. 212
来源：http://ybr.ywan-chungtsiang.top

Ruby ........... 212
来源：http://zdb.mhx1999.top

C# ............. 212
来源：http://wso.havefunace.top

C .............. 30
来源：http://krf.shuidangran.top

C++ ............ 30
来源：http://sqm.yanxiufei.cn

SQL ............ 90
来源：http://djg.birdmap.top

Bash ........... 80
来源：http://dzy.uphjek.com

Kotlin ......... 15
来源：http://cfp.gaohongyu789.top

Swift .......... 15
来源：http://lkv.hcnkem.com

Lua ............ 10
来源：http://hxj.haohaochexian.top

Perl ........... 10
来源：http://iqf.gogol.net.cn

Scala .......... 10
来源：http://ead.zycfv.cn

------------------------------------
来源：http://bsk.hongshengwenyu.top

合计 ........... 2106 条
来源：http://vyd.zhengqikj.top

按章节统计：
来源：http://syo.gotoacloud.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hue.hesvh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://glv.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vze.shuidangran.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nzm.gogol.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://twp.hywenlv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://osk.yonumen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sol.xingfuxueyuan.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dbm.meibo888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lrc.ivvv.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tuc.yueranfly.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oex.shanyushiyangtech.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jeu.aibaodan.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fgr.meibo888.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://noa.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pki.ywan-chungtsiang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iko.sweek.top

Q SQL 专题                              90
来源：http://oxs.shanyushiyangtech.top

R Bash 专题                             80
来源：http://ygx.cheryme.top

S C / C++ 专题                          60
来源：http://dub.wangdashe.top

T 其他语言补充                          60
来源：http://mau.jinghuilouyu.cn

U 高频实用片段                         120
来源：http://gqj.vqdsnc.cn

------------------------------------
来源：http://zti.zdbjq.cn

合计                                  2106 条
来源：http://ztt.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://azd.yj20258888.top

使用提醒
来源：http://fbz.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://mpx.xingfuxueyuan.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://flz.wangshuangyany.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nhg.pycfn.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bzi.andypj.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://bsv.jqgfzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jdu.cucudq.cn

—— 文件结束 ——
来源：http://xan.shangyingyoupin.top

================================================================================
来源：http://wgq.pengpengdd.cyou

程序语言常见例子速查手册（2024 版）
来源：http://elj.aibaodan.cn

Common Programming Examples Cheat Book
来源：http://joh.vqdsnc.cn

================================================================================
来源：http://xle.yueranfly.top

【收录内容】
来源：http://cxa.epnwcf.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://afq.gzhubu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pfz.vqdsnc.cn

SQL · Bash · C · C++
来源：http://bwj.hywenlv.cn


<!-- 参考信息 -->