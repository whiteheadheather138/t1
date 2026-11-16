代发 wailian999

val a = 1;  var b = 2
来源：http://clw.316326.xyz

[T53] Scala：字符串插值
来源：http://mdj.tanke756.top

s"值: $b"
来源：http://xsv.aibaodan.cn

[T54] Scala：集合映射
来源：http://xpk.shuidangran.top

List(1, 2, 3).map(_ * 2)
来源：http://emd.zhaomingkeji.xyz

[T55] Scala：集合过滤
来源：http://fot.zhaomingkeji.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://wfx.yuanzhike.top

[T56] Scala：样例类
来源：http://ihr.aibaodan.cn

case class User(name: String, age: Int)
来源：http://ulb.yvedp.cn

[T57] Scala：模式匹配
来源：http://wlb.wangdashe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jdb.birdmap.top

[T58] Scala：函数定义
来源：http://ykm.gaohongyu789.top

def add(a: Int, b: Int): Int = a + b
来源：http://gig.zhoulong.xyz

[T59] Scala：循环
来源：http://ppy.snrcjt.cn

for (i <- 1 to 10) println(i)
来源：http://lej.sysykeji.top

[T60] Scala：折叠
来源：http://yii.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yqg.xingfuxueyuan.xyz

================================================================================
来源：http://yco.ywan-chungtsiang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bar.xingfuxueyuan.xyz

================================================================================
来源：http://tzg.jiagoushi.top

[U01] Py：创建虚拟环境
来源：http://ijy.hesvh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lrz.gotoacloud.top

[U02] Py：导出 / 安装依赖
来源：http://mdc.yanxiufei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vmo.chenzaomai.com

[U03] Py：加载 .env 配置
来源：http://pok.vqdsnc.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qqk.yuxming.cn

[U04] Py：变量调试打印
来源：http://meb.sysykeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rbo.shangyingyoupin.top

[U05] Py：列表去重且保序
来源：http://lza.shanyushiyangtech.top

list(dict.fromkeys(arr))
来源：http://rwq.daxiang520.top

[U06] Py：合并两个字典
来源：http://rxy.bbcook.cn

{**a, **b}
来源：http://eya.snrcjt.cn

[U07] Py：反转字典键值
来源：http://xpi.vqdsnc.cn

{v: k for k, v in d.items()}
来源：http://qvw.bjfxy.top

[U08] Py：展平二维列表
来源：http://ljs.ppjwa.cn

[y for x in nested for y in x]
来源：http://qqg.uphjek.com

[U09] Py：字典取最大值的键
来源：http://wck.ppjwa.cn

max(d, key=d.get)
来源：http://ufe.hnqzz.top

[U10] Py：按值排序字典
来源：http://vmr.yanxiufei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ggy.jiagoushi.top

[U11] Py：生成器表达式
来源：http://yeq.shangyingyoupin.top

(x * 2 for x in arr)
来源：http://bko.hammf.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gfu.sweek.top

Counter(arr).most_common(3)
来源：http://jcf.uphjek.com

[U13] Py：固定长度队列
来源：http://njo.feifeiyinyue.top

deque(maxlen=10)
来源：http://wln.nwbrower.top

[U14] Py：分组收集到列表
来源：http://ijg.ywan-chungtsiang.top

defaultdict(list)
来源：http://wrh.hnxiangtu.top

[U15] Py：高精度计时
来源：http://nnh.daxiang520.top

t = time.perf_counter()
来源：http://oye.jinghuilouyu.cn

[U16] Py：命令行参数解析
来源：http://hxt.yfazqb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://spd.sjlbkw.cn

[U17] Py：初始化日志
来源：http://baa.hongshengwenyu.top

logging.basicConfig(level=logging.INFO)
来源：http://mew.zhengqikj.top

[U18] Py：预编译正则
来源：http://krt.epnwcf.com

pat = re.compile(r"\d+")
来源：http://rvz.tianlin.xyz

[U19] Py：正则替换带回调
来源：http://iwk.shanyushiyangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://upf.ywan-chungtsiang.top

[U20] Py：缓存函数结果
来源：http://qjf.yuxming.cn

@functools.lru_cache(maxsize=None)
来源：http://pzb.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://hpa.hnqzz.top

@contextlib.contextmanager
来源：http://eif.zdbjq.cn

[U22] Py：矩阵转置
来源：http://bqj.ivvv.top

list(zip(*m))
来源：http://lsw.shanyushiyangkeji.top

[U23] Py：分块读取大文件
来源：http://dfa.zhiwuduotai.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fzg.hfpthk.cn

[U24] Py：路径操作
来源：http://uik.hammf.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qmo.sxryk.cn

[U25] Py：CSV 按字典读
来源：http://dmk.pengpengdd.cyou

csv.DictReader(f)
来源：http://scd.iojbl.cn

[U26] Py：并发下载
来源：http://xdc.zycfv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qpb.bbcook.cn

[U27] Py：异步 HTTP
来源：http://ejl.epnwcf.com

aiohttp.ClientSession() 配合 async with
来源：http://jrl.hnqzz.top

[U28] Py：类型别名
来源：http://hfs.chenzaomai.com

UserId = int
来源：http://byl.birdmap.top

[U29] Py：属性校验
来源：http://esz.mhx1999.top

@property 与 @x.setter 配合
来源：http://zlq.ehwqpu.com

[U30] Py：数据类
来源：http://znv.hnxiangtu.top

@dataclass(slots=True)
来源：http://eyi.52xcode.cn

[U31] Py：单测
来源：http://xjo.dianchejie.cn

python -m pytest -q
来源：http://gqc.wangdashe.top

[U32] Py：代码格式化
来源：http://wuh.redwolf501.top

ruff format . && ruff check --fix .
来源：http://gkl.ehwqpu.com

[U33] Py：打包发布
来源：http://imw.nwbrower.top

python -m build  （依赖 pyproject.toml）
来源：http://vso.zhixingplan.top

[U34] Py：判断编码
来源：http://vew.xuetiantiany.cn

chardet.detect(raw)
来源：http://giv.jinqigufen.top

[U35] Py：发送邮件
来源：http://dnl.gogol.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hri.ydjk.org.cn

[U36] Py：定时任务
来源：http://abl.yj202588.top

schedule.every(10).minutes.do(job)
来源：http://nfk.fanxiaobao.xyz

[U37] Py：读写 Excel
来源：http://mts.xziqi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://aaa.9152youxi.cn

[U38] Py：获取脚本所在目录
来源：http://tgt.yvedp.cn

Path(__file__).resolve().parent
来源：http://xgu.zhongyouzk.top

[U39] Py：判断是否在交互环境
来源：http://dbt.gaohongyu789.top

sys.stdout.isatty()
来源：http://ygs.sufxvd.cn

[U40] Py：打印到标准错误
来源：http://omp.shzxlz.cn

print("err", file=sys.stderr)
来源：http://sir.sufxvd.cn

[U41] PHP：初始化 Composer 项目
来源：http://wih.tarul.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ons.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://gza.zhixingplan.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tny.feifeiyinyue.top

[U43] PHP：声明命名空间
来源：http://swh.meibo888.top

namespace App\Http;
来源：http://uob.zdqjudy.top

[U44] PHP：开启严格类型
来源：http://tnx.sufxvd.cn

declare(strict_types=1);
来源：http://hss.jyoumei.cn

[U45] PHP：类型声明与返回类型
来源：http://bvn.ppjwa.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ukw.hammf.cn

[U46] PHP：可空类型
来源：http://ujs.aizwys.cn

?string $name = null
来源：http://wii.52xcode.cn

[U47] PHP：联合类型
来源：http://uqp.zhaomingkeji.xyz

int|string $id
来源：http://xbl.wangshuangyany.cn

[U48] PHP：纯枚举
来源：http://hem.jinqigufen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tke.vehdjk.com

[U49] PHP：只读属性
来源：http://uia.yanxiufei.cn

public readonly string $name
来源：http://obm.gaohongyu789.top

[U50] PHP：构造器属性提升
来源：http://kkj.xuanzx.com

public function __construct(private int $id) {}
来源：http://vzm.bbcook.cn

[U51] PHP：数组解构
来源：http://xab.dashuyun.cn

[$a, $b] = $arr;
来源：http://rqv.quarkkingdee.top

[U52] PHP：箭头函数
来源：http://rbw.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://isp.feifeiyinyue.top

[U53] PHP：空合并运算符
来源：http://jkw.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://wpf.wangdashe.top

[U54] PHP：空安全调用
来源：http://ann.jqgfzy.top

$obj?->method()
来源：http://ugu.yfazqb.com

[U55] PHP：match 表达式
来源：http://ixf.fktsv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zbi.ydzc1.top

[U56] PHP：命名参数
来源：http://zaa.sysykeji.top

f(a: 1, b: 2)
来源：http://vlh.zhiwuduotai.top

[U57] PHP：字符串插值
来源：http://zzl.jlsjyb.cn

"值: {$a}"
来源：http://uih.yuanzhike.top

[U58] PHP：数组三件套
来源：http://ftf.fanxiaobao.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jhl.gzhubu.top

[U59] PHP：自定义排序
来源：http://kjn.iojbl.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tun.hfpthk.cn

[U60] PHP：JSON 编解码
来源：http://cbs.gaohongyu789.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ujp.birdmap.top

[U61] PHP：正则
来源：http://dma.hnqzz.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://trs.aizwys.cn

[U62] PHP：日期对象
来源：http://ctm.cucudq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bpf.iojbl.cn

[U63] PHP：文件读写
来源：http://yxn.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qlp.shanyushiyangtech.top

[U64] PHP：目录遍历
来源：http://vmw.daxiang520.top

glob("dir/*.php");  scandir("dir");
来源：http://dok.pycfn.com

[U65] PHP：会话
来源：http://xpo.ybcxt.top

session_start();  $_SESSION["uid"] = 1;
来源：http://esg.xziqi.cn

[U66] PHP：设置 Cookie
来源：http://ooy.ppjwa.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dbq.fzhhl.top

[U67] PHP：处理文件上传
来源：http://rgh.iojbl.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uir.bjfxy.top

[U68] PHP：PDO 连接
来源：http://bor.fehbvm.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://itu.yuxming.cn

[U69] PHP：PDO 预处理
来源：http://avs.shuidangran.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xfc.jinyuanbaomall.cn

[U70] PHP：PDO 事务
来源：http://pvo.tanke756.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://azg.hysaishi.cn

[U71] PHP：抛出异常
来源：http://hqs.hongshengwenyu.top

throw new RuntimeException("失败", 500);
来源：http://cwm.c1oappe.top

[U72] PHP：写错误日志
来源：http://oxv.ivvv.top

error_log("失败: " . $e->getMessage());
来源：http://bvj.chenjidiqi.icu

[U73] PHP：读取 ini 配置
来源：http://rpl.chenlongwang.top

parse_ini_file("config.ini", true)
来源：http://zqc.xuetiantiany.cn

[U74] PHP：读取环境变量
来源：http://hcj.shangyingyoupin.top

getenv("APP_ENV") ?: "production"
来源：http://jzg.birdmap.top

[U75] PHP：依赖注入
来源：http://ndl.jinyuanbaomall.cn

composer require psr/container
来源：http://ujm.aibaodan.cn

[U76] PHP：简单路由
来源：http://kjk.fzhhl.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hdn.havefunace.top

[U77] PHP：模板渲染
来源：http://upo.jinghuilouyu.cn

composer require twig/twig
来源：http://gxv.guowangkeji.top

[U78] PHP：单元测试
来源：http://noi.shangyingyoupin.top

composer require --dev phpunit/phpunit
来源：http://wkm.hongshengwenyu.top

[U79] PHP：静态分析
来源：http://sfd.hywenlv.cn

composer require --dev phpstan/phpstan
来源：http://gaf.epnwcf.com

[U80] PHP：代码规范修复
来源：http://iun.cucudq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ncx.birdmap.top

[U81] JS：初始化项目
来源：http://lei.zhongyouzk.top

npm init -y;  npm i express
来源：http://mqi.smart0.xyz

[U82] JS：package.json 脚本
来源：http://tpz.haohaochexian.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://exl.ivvv.top

[U83] JS：ES Module 导入导出
来源：http://iuv.yuanzhike.top

export const a = 1;  import { a } from "./m.js";
来源：http://cfg.ywan-chungtsiang.top

[U84] JS：CommonJS 写法
来源：http://pyt.tarul.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mgc.xingfuxueyuan.xyz

[U85] JS：可选链
来源：http://ljd.nanxinkj.top

a?.b?.c
来源：http://kvx.tarul.cn

[U86] JS：空值合并
来源：http://upx.pycfn.com

a ?? b
来源：http://lcg.wangdashe.top

[U87] JS：解构默认值
来源：http://vkx.xuetiantiany.cn

const { a = 1, b = 2 } = obj;
来源：http://ogu.nwbrower.top

[U88] JS：对象展开合并
来源：http://ogf.zhoulong.xyz

{ ...a, ...b }
来源：http://czd.gzhubu.top

[U89] JS：数组去重
来源：http://ooo.shzxlz.cn

[...new Set(arr)]
来源：http://qns.chenlongwang.top

[U90] JS：数字数组排序
来源：http://zkh.snrcjt.cn

[...arr].sort((a, b) => a - b)
来源：http://urc.haohaochexian.top

[U91] JS：对象键值遍历
来源：http://bml.tarul.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rat.xylfe.cn

[U92] JS：深拷贝
来源：http://ibx.jinghuilouyu.cn

structuredClone(obj)
来源：http://whk.vqdsnc.cn

[U93] JS：模板字符串
来源：http://hut.daria6918.cn

`共 ${n} 条`
来源：http://qxd.gogol.net.cn

[U94] JS：箭头函数
来源：http://kgk.snrcjt.cn

const double = x => x * 2;
来源：http://xrk.jinqigufen.top

[U95] JS：Promise 包装
来源：http://vgv.jianghu66.top

new Promise((resolve, reject) => {})
来源：http://pss.ydjk.org.cn

[U96] JS：async/await 与异常
来源：http://vkv.aizwys.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://acf.gogol.net.cn

[U97] JS：并发请求
来源：http://lwi.cdnleiting.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bhi.yvedp.cn

[U98] JS：fetch 带 JSON
来源：http://cuw.gogol.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://buw.ydjk.org.cn

[U99] JS：事件监听
来源：http://skl.meibo888.top

el.addEventListener("click", e => {})
来源：http://xfi.cdnleiting.top

[U100] JS：DOM 查询
来源：http://tui.ydjk.org.cn

document.querySelector(".item")
来源：http://fsj.shuidangran.top

[U101] JS：classList 操作
来源：http://ihe.gogol.net.cn

el.classList.toggle("active")
来源：http://lwv.ydjk.org.cn

[U102] JS：本地存储
来源：http://uoj.sweek.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://att.xuanzx.com

[U103] JS：定时器
来源：http://idb.sysykeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sam.fehbvm.com

[U104] JS：防抖
来源：http://cda.hesvh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hfn.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://ssq.xziqi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wgv.yuanzhike.top

[U106] JS：日期格式化
来源：http://wgx.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jrm.nanxinkj.top

[U107] JS：数字千分位
来源：http://bxk.xziqi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rpl.bbcook.cn

[U108] JS：随机整数
来源：http://vgm.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dae.havefunace.top

[U109] JS：数组分组
来源：http://xhf.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://edk.zycfv.cn

[U110] JS：数组分块
来源：http://rgo.daxiang520.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://njx.shuidangran.top

[U111] JS：对象转 Map
来源：http://oed.yj202588.top

new Map(Object.entries(obj))
来源：http://wrq.svipenyu.cn

[U112] JS：字符串补位
来源：http://glz.yvedp.cn

"7".padStart(3, "0")
来源：http://mlw.meibo888.top

[U113] JS：正则替换全部
来源：http://qkl.vehdjk.com

s.replaceAll("a", "b")
来源：http://dut.fengsongda.top

[U114] JS：JSON 深比较
来源：http://ogn.cucudq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ydy.jqgufenzy.top

[U115] JS：生成 UUID
来源：http://kwh.hysaishi.cn

crypto.randomUUID()
来源：http://lyt.yj202588.top

[U116] JS：类型检查（JSDoc）
来源：http://ccm.fehbvm.com

/** @param {string} name */ function f(name) {}
来源：http://xoh.zhengqikj.top

[U117] JS：单元测试
来源：http://rzt.shangyingyoupin.top

npm i -D vitest;  npx vitest
来源：http://rhu.zhiwuduotai.top

[U118] JS：开发服务器
来源：http://dmi.tian-w.cn

npm i -D vite;  npx vite
来源：http://ekh.hysaishi.cn

[U119] JS：生产构建
来源：http://gvx.tian-w.cn

npx vite build
来源：http://zpp.chenlongwang.top

[U120] JS：读取环境变量（Vite）
来源：http://vxf.wangshuangyany.cn

import.meta.env.VITE_API_URL
来源：http://fhf.cdnleiting.top

================================================================================
来源：http://vrz.yangfankeji.com

统计汇总
来源：http://eri.hywenlv.cn

================================================================================
来源：http://ynp.shzxlz.cn

按语言统计（条）：
来源：http://uvk.hnxiangtu.top

Python ......... 252
来源：http://rck.hfpthk.cn

PHP ............ 252
来源：http://wrm.xuetiantiany.cn

JavaScript ..... 252
来源：http://jls.gotoacloud.top

TypeScript ..... 212
来源：http://ncj.tanke756.top

Java ........... 212
来源：http://zwf.sysykeji.top

Go ............. 212
来源：http://zwp.xziqi.cn

Ruby ........... 212
来源：http://mkd.iojbl.cn

C# ............. 212
来源：http://agm.kuanghao11.cn

C .............. 30
来源：http://rua.ppjwa.cn

C++ ............ 30
来源：http://cer.hysaishi.cn

SQL ............ 90
来源：http://klh.feifeiyinyue.top

Bash ........... 80
来源：http://moh.cheryme.top

Kotlin ......... 15
来源：http://ssk.gzhubu.top

Swift .......... 15
来源：http://xda.jiagoushi.top

Lua ............ 10
来源：http://ksl.tarul.cn

Perl ........... 10
来源：http://glj.jqgfzy.top

Scala .......... 10
来源：http://msk.aibaodan.cn

------------------------------------
来源：http://kvv.smart0.xyz

合计 ........... 2106 条
来源：http://sfl.ctjpmb.com

按章节统计：
来源：http://uzw.zdqjudy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tts.xuetiantiany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://utk.zhoulong.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pbm.zdqjudy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rio.uphjek.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://enu.vqdsnc.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ojj.yangfankeji.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sdj.xingfuxueyuan.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://erk.ywan-chungtsiang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uph.xuetiantiany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nbm.epnwcf.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oxs.nanxuanxn.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://utr.yvedp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ohv.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ghv.shuidangran.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xhh.hnxiangtu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lit.cqqwz.cn


<!-- 参考信息 -->