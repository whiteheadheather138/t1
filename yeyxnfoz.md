代发 wailian999

[U03] Py：加载 .env 配置
来源：http://ezi.snrcjt.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://prk.bbcook.cn

[U04] Py：变量调试打印
来源：http://pmr.jiagoushi.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dch.zhijiandao.cn

[U05] Py：列表去重且保序
来源：http://zhe.c1oappe.top

list(dict.fromkeys(arr))
来源：http://jya.fzhhl.top

[U06] Py：合并两个字典
来源：http://rtu.tianlin.xyz

{**a, **b}
来源：http://pwt.xingfuxueyuan.xyz

[U07] Py：反转字典键值
来源：http://ect.c1oappe.top

{v: k for k, v in d.items()}
来源：http://sba.yongpay.top

[U08] Py：展平二维列表
来源：http://bsw.aizwys.cn

[y for x in nested for y in x]
来源：http://hgg.ywan-chungtsiang.top

[U09] Py：字典取最大值的键
来源：http://uny.yj202588.top

max(d, key=d.get)
来源：http://fgb.nanxinkj.top

[U10] Py：按值排序字典
来源：http://gjc.sysykeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uts.yuanzhike.top

[U11] Py：生成器表达式
来源：http://hcn.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://dna.shanyushiyangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://dbx.tarul.cn

Counter(arr).most_common(3)
来源：http://uei.gogol.net.cn

[U13] Py：固定长度队列
来源：http://cgt.ehwqpu.com

deque(maxlen=10)
来源：http://wax.cdnleiting.top

[U14] Py：分组收集到列表
来源：http://wml.ctjpmb.com

defaultdict(list)
来源：http://wcy.yj202588.top

[U15] Py：高精度计时
来源：http://hzi.aizwys.cn

t = time.perf_counter()
来源：http://bnu.tarul.cn

[U16] Py：命令行参数解析
来源：http://ytv.hysaishi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qpx.yangfankeji.com

[U17] Py：初始化日志
来源：http://pwi.yj202588.top

logging.basicConfig(level=logging.INFO)
来源：http://tkh.chenlongwang.top

[U18] Py：预编译正则
来源：http://dqx.jqgfzy.top

pat = re.compile(r"\d+")
来源：http://trr.hammf.cn

[U19] Py：正则替换带回调
来源：http://lwl.ydzc1.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nmr.xuetiantiany.cn

[U20] Py：缓存函数结果
来源：http://kzz.ywan-chungtsiang.top

@functools.lru_cache(maxsize=None)
来源：http://ero.quarkkingdee.top

[U21] Py：自定义上下文管理器
来源：http://rrh.snrcjt.cn

@contextlib.contextmanager
来源：http://wny.ehwqpu.com

[U22] Py：矩阵转置
来源：http://iwc.jiagoushi.top

list(zip(*m))
来源：http://bjk.chenlongwang.top

[U23] Py：分块读取大文件
来源：http://lnq.kuanghao11.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://smq.mhx1999.top

[U24] Py：路径操作
来源：http://ieb.jyoumei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ohe.jinqigufen.top

[U25] Py：CSV 按字典读
来源：http://zjr.tianlin.xyz

csv.DictReader(f)
来源：http://vul.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://own.hammf.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://djr.ydzc1.top

[U27] Py：异步 HTTP
来源：http://qsm.snrcjt.cn

aiohttp.ClientSession() 配合 async with
来源：http://ger.nwbrower.top

[U28] Py：类型别名
来源：http://umj.xuetiantiany.cn

UserId = int
来源：http://sjn.quarkkingdee.top

[U29] Py：属性校验
来源：http://bev.birdmap.top

@property 与 @x.setter 配合
来源：http://dgk.ppjwa.cn

[U30] Py：数据类
来源：http://igs.fktsv.cn

@dataclass(slots=True)
来源：http://fqi.cashguo.top

[U31] Py：单测
来源：http://rzv.hywenlv.cn

python -m pytest -q
来源：http://bru.kuanghao11.cn

[U32] Py：代码格式化
来源：http://vyh.shuidangran.top

ruff format . && ruff check --fix .
来源：http://nza.zdqjudy.top

[U33] Py：打包发布
来源：http://ucy.fehbvm.com

python -m build  （依赖 pyproject.toml）
来源：http://cib.tanke756.top

[U34] Py：判断编码
来源：http://vid.9152youxi.cn

chardet.detect(raw)
来源：http://dsn.yuanzhike.top

[U35] Py：发送邮件
来源：http://sfq.jinqigfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qdv.zdbjq.cn

[U36] Py：定时任务
来源：http://yum.hnxiangtu.top

schedule.every(10).minutes.do(job)
来源：http://hfp.xuanzx.com

[U37] Py：读写 Excel
来源：http://rmr.jyoumei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cya.nwbrower.top

[U38] Py：获取脚本所在目录
来源：http://rwa.hongshengwenyu.top

Path(__file__).resolve().parent
来源：http://jml.fengsongda.top

[U39] Py：判断是否在交互环境
来源：http://dgr.zhiwuduotai.top

sys.stdout.isatty()
来源：http://vki.shanyushiyangtech.top

[U40] Py：打印到标准错误
来源：http://azr.ydjk.org.cn

print("err", file=sys.stderr)
来源：http://jdf.cucudq.cn

[U41] PHP：初始化 Composer 项目
来源：http://fpo.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://kfn.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://ply.redwolf501.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uml.zhongyouzk.top

[U43] PHP：声明命名空间
来源：http://dux.gzhubu.top

namespace App\Http;
来源：http://jeg.cashguo.top

[U44] PHP：开启严格类型
来源：http://rdg.yj20258.top

declare(strict_types=1);
来源：http://fbv.hongshengwenyu.top

[U45] PHP：类型声明与返回类型
来源：http://abv.cashguo.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://knf.wangdashe.top

[U46] PHP：可空类型
来源：http://ieq.mhx1999.top

?string $name = null
来源：http://mfr.ehwqpu.com

[U47] PHP：联合类型
来源：http://zxv.gotoacloud.top

int|string $id
来源：http://trr.sweek.top

[U48] PHP：纯枚举
来源：http://hdk.svipenyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hkq.yfazqb.com

[U49] PHP：只读属性
来源：http://exq.xziqi.cn

public readonly string $name
来源：http://hce.yj202588.top

[U50] PHP：构造器属性提升
来源：http://jwh.yuanzhike.top

public function __construct(private int $id) {}
来源：http://syd.ydzc1.top

[U51] PHP：数组解构
来源：http://ucd.cdnleiting.top

[$a, $b] = $arr;
来源：http://tyr.sjlbkw.cn

[U52] PHP：箭头函数
来源：http://iju.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://ahp.jlsjyb.cn

[U53] PHP：空合并运算符
来源：http://gro.hongshengwenyu.top

$v = $a ?? $b ?? "default";
来源：http://oql.hysaishi.cn

[U54] PHP：空安全调用
来源：http://bky.shanyushiyangtech.top

$obj?->method()
来源：http://kcn.quarkkingdee.top

[U55] PHP：match 表达式
来源：http://vmq.fanxiaobao.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yox.vehdjk.com

[U56] PHP：命名参数
来源：http://gwm.jiagoushi.top

f(a: 1, b: 2)
来源：http://srm.iojbl.cn

[U57] PHP：字符串插值
来源：http://uvt.hnqzz.top

"值: {$a}"
来源：http://ncv.wangshuangyany.cn

[U58] PHP：数组三件套
来源：http://aca.bbcook.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fgm.hywenlv.cn

[U59] PHP：自定义排序
来源：http://fcu.guannengcc.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tqi.yueranfly.top

[U60] PHP：JSON 编解码
来源：http://lub.hnxiangtu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ffw.snrcjt.cn

[U61] PHP：正则
来源：http://ucl.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://itt.guannengcc.top

[U62] PHP：日期对象
来源：http://snc.nanxuanxn.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ifc.c1oappe.top

[U63] PHP：文件读写
来源：http://mqy.ctjpmb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ahc.yueranfly.top

[U64] PHP：目录遍历
来源：http://tti.ivvv.top

glob("dir/*.php");  scandir("dir");
来源：http://wou.hongshengwenyu.top

[U65] PHP：会话
来源：http://iml.fehbvm.com

session_start();  $_SESSION["uid"] = 1;
来源：http://gak.zhongyouzk.top

[U66] PHP：设置 Cookie
来源：http://vcr.gogol.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aug.ydzc1.top

[U67] PHP：处理文件上传
来源：http://gbi.yvedp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ieu.chenjidiqi.icu

[U68] PHP：PDO 连接
来源：http://tlu.jinyuanbaomall.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cnx.wangshuangyany.cn

[U69] PHP：PDO 预处理
来源：http://gcw.guowangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hyv.jqgufenzy.top

[U70] PHP：PDO 事务
来源：http://slr.tianlin.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cfc.gogol.net.cn

[U71] PHP：抛出异常
来源：http://mmc.kuanghao11.cn

throw new RuntimeException("失败", 500);
来源：http://itu.birdmap.top

[U72] PHP：写错误日志
来源：http://tnx.jlsjyb.cn

error_log("失败: " . $e->getMessage());
来源：http://yyt.zycfv.cn

[U73] PHP：读取 ini 配置
来源：http://mey.fanxiaobao.xyz

parse_ini_file("config.ini", true)
来源：http://enn.aizwys.cn

[U74] PHP：读取环境变量
来源：http://gjo.xingfuxueyuan.xyz

getenv("APP_ENV") ?: "production"
来源：http://rcj.jqgfzy.top

[U75] PHP：依赖注入
来源：http://tny.shuidangran.top

composer require psr/container
来源：http://vqe.dashuyun.cn

[U76] PHP：简单路由
来源：http://itf.jinghuilouyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cuh.bbcook.cn

[U77] PHP：模板渲染
来源：http://xqg.yonumen.top

composer require twig/twig
来源：http://ddk.chenlongwang.top

[U78] PHP：单元测试
来源：http://xrz.yongpay.top

composer require --dev phpunit/phpunit
来源：http://rsj.aizwys.cn

[U79] PHP：静态分析
来源：http://tmm.hcnkem.com

composer require --dev phpstan/phpstan
来源：http://psw.xingfuxueyuan.xyz

[U80] PHP：代码规范修复
来源：http://ytz.jinqigfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pzb.bjfxy.top

[U81] JS：初始化项目
来源：http://bjo.shzxlz.cn

npm init -y;  npm i express
来源：http://yhm.cucudq.cn

[U82] JS：package.json 脚本
来源：http://kxv.zhiwuduotai.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mds.xziqi.cn

[U83] JS：ES Module 导入导出
来源：http://isi.gaohongyu789.top

export const a = 1;  import { a } from "./m.js";
来源：http://rhh.ppjwa.cn

[U84] JS：CommonJS 写法
来源：http://nlz.hammf.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fwn.gaohongyu789.top

[U85] JS：可选链
来源：http://pov.sxryk.cn

a?.b?.c
来源：http://rxm.zhengqikj.top

[U86] JS：空值合并
来源：http://pke.vqdsnc.cn

a ?? b
来源：http://eob.yongpay.top

[U87] JS：解构默认值
来源：http://oau.hongshengwenyu.top

const { a = 1, b = 2 } = obj;
来源：http://xmu.bbcook.cn

[U88] JS：对象展开合并
来源：http://xbh.daria6918.cn

{ ...a, ...b }
来源：http://pyz.andypj.xyz

[U89] JS：数组去重
来源：http://ivj.andypj.xyz

[...new Set(arr)]
来源：http://wrh.wangshuangyany.cn

[U90] JS：数字数组排序
来源：http://udw.shuidangran.top

[...arr].sort((a, b) => a - b)
来源：http://tlw.tian-w.cn

[U91] JS：对象键值遍历
来源：http://ubt.feifeiyinyue.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://smp.yonumen.top

[U92] JS：深拷贝
来源：http://fys.bjfxy.top

structuredClone(obj)
来源：http://gnc.havefunace.top

[U93] JS：模板字符串
来源：http://cjd.wangshuangyany.cn

`共 ${n} 条`
来源：http://gfx.gaohongyu789.top

[U94] JS：箭头函数
来源：http://szs.chenjidiqi.icu

const double = x => x * 2;
来源：http://ipb.jlsjyb.cn

[U95] JS：Promise 包装
来源：http://nju.yj20258.top

new Promise((resolve, reject) => {})
来源：http://myr.jiagoushi.top

[U96] JS：async/await 与异常
来源：http://tqy.jinqigfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ipl.xuanzx.com

[U97] JS：并发请求
来源：http://ghr.aibaodan.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://agt.snrcjt.cn

[U98] JS：fetch 带 JSON
来源：http://njx.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bpc.xziqi.cn

[U99] JS：事件监听
来源：http://wsq.jinghuilouyu.cn

el.addEventListener("click", e => {})
来源：http://jxk.havefunace.top

[U100] JS：DOM 查询
来源：http://jqi.chenlongwang.top

document.querySelector(".item")
来源：http://fye.ctjpmb.com

[U101] JS：classList 操作
来源：http://cqs.ywan-chungtsiang.top

el.classList.toggle("active")
来源：http://rwd.aizwys.cn

[U102] JS：本地存储
来源：http://icm.yj20258888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ukq.fzhhl.top

[U103] JS：定时器
来源：http://kvr.xuanzx.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gfg.ppjwa.cn

[U104] JS：防抖
来源：http://vze.fengsongda.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://idv.jqgfzy.top

[U105] JS：节流
来源：http://pqn.jinyuanbaomall.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jbh.gogol.net.cn

[U106] JS：日期格式化
来源：http://src.nanxuanxn.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://crv.sxryk.cn

[U107] JS：数字千分位
来源：http://fcr.kuanghao11.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://aqx.jyoumei.cn

[U108] JS：随机整数
来源：http://arm.kuanghao11.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ylx.jqgufenzy.top

[U109] JS：数组分组
来源：http://pah.yonumen.top

Object.groupBy(arr, x => x.type)
来源：http://jsa.vehdjk.com

[U110] JS：数组分块
来源：http://wkd.shanyushiyangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kvs.bbcook.cn

[U111] JS：对象转 Map
来源：http://iby.daria6918.cn

new Map(Object.entries(obj))
来源：http://fbs.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://qfa.andypj.xyz

"7".padStart(3, "0")
来源：http://wtm.yangfankeji.com

[U113] JS：正则替换全部
来源：http://cpk.hongshengwenyu.top

s.replaceAll("a", "b")
来源：http://xhd.yj20258888.top

[U114] JS：JSON 深比较
来源：http://hxq.aizwys.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jgu.smart0.xyz

[U115] JS：生成 UUID
来源：http://nhp.yongpay.top

crypto.randomUUID()
来源：http://pkn.haohaochexian.top

[U116] JS：类型检查（JSDoc）
来源：http://gpx.yj20258888.top

/** @param {string} name */ function f(name) {}
来源：http://mln.zycfv.cn

[U117] JS：单元测试
来源：http://elm.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://vep.kuanghao11.cn

[U118] JS：开发服务器
来源：http://zml.yj202588.top

npm i -D vite;  npx vite
来源：http://nbm.sweek.top

[U119] JS：生产构建
来源：http://kqy.aizwys.cn

npx vite build
来源：http://onl.haohaochexian.top

[U120] JS：读取环境变量（Vite）
来源：http://rqw.yj20258888.top

import.meta.env.VITE_API_URL
来源：http://jss.yuxming.cn

================================================================================
来源：http://gdv.iojbl.cn

统计汇总
来源：http://bld.ctjpmb.com

================================================================================
来源：http://jau.fehbvm.com

按语言统计（条）：
来源：http://auh.haohaochexian.top

Python ......... 252
来源：http://etx.jinyuanbaomall.cn

PHP ............ 252
来源：http://btd.yongpay.top

JavaScript ..... 252
来源：http://whq.vqdsnc.cn

TypeScript ..... 212
来源：http://nfl.ctjpmb.com

Java ........... 212
来源：http://rgh.zhixingplan.top

Go ............. 212
来源：http://mii.tanke756.top

Ruby ........... 212
来源：http://tmp.yonumen.top

C# ............. 212
来源：http://aeb.cucudq.cn

C .............. 30
来源：http://flt.dashuyun.cn

C++ ............ 30
来源：http://dff.sweek.top

SQL ............ 90
来源：http://bjm.yj202588.top

Bash ........... 80
来源：http://ozx.nanxuanxn.top

Kotlin ......... 15
来源：http://kjb.tanke756.top

Swift .......... 15
来源：http://zwj.ybcxt.top

Lua ............ 10
来源：http://afh.yangfankeji.com

Perl ........... 10
来源：http://pgz.chenjidiqi.icu

Scala .......... 10
来源：http://wcf.smart0.xyz

------------------------------------
来源：http://qpf.cheryme.top

合计 ........... 2106 条
来源：http://xbi.svipenyu.cn

按章节统计：
来源：http://alp.yj20258888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ibi.tarul.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mvb.nanxuanxn.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uet.uphjek.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://klb.svipenyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ofb.svipenyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lyw.iojbl.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qow.feifeiyinyue.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://emo.zdqjudy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ajb.sufxvd.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rbz.jqgufenzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://udo.cdnleiting.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hoi.zhoulong.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kgu.andypj.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iiu.fengsongda.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nfl.tianlin.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xfd.iojbl.cn

Q SQL 专题                              90
来源：http://ixn.yangfankeji.com

R Bash 专题                             80
来源：http://utv.cucudq.cn

S C / C++ 专题                          60
来源：http://dol.yongpay.top

T 其他语言补充                          60
来源：http://koa.hnqzz.top

U 高频实用片段                         120
来源：http://cgd.cdnleiting.top

------------------------------------
来源：http://lvo.jinqigufen.top

合计                                  2106 条
来源：http://ayh.52xcode.cn

--------------------------------------------------------------------------------
来源：http://zvt.chenjidiqi.icu

使用提醒
来源：http://rdl.yueranfly.top

--------------------------------------------------------------------------------
来源：http://cmv.quarkkingdee.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fkv.yj20258888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rey.jlsjyb.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rhv.hnqzz.top

在旧版本上使用前请先确认语法支持情况。
来源：http://gfh.iojbl.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jla.sxryk.cn

—— 文件结束 ——
来源：http://buq.zycfv.cn

================================================================================
来源：http://lbq.cqqwz.cn

程序语言常见例子速查手册（2024 版）
来源：http://ffk.chenjidiqi.icu

Common Programming Examples Cheat Book
来源：http://kka.316326.xyz

================================================================================
来源：http://hna.kuanghao11.cn

【收录内容】
来源：http://dhj.yueranfly.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ukg.tanke756.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vcb.vqdsnc.cn

SQL · Bash · C · C++
来源：http://xha.yj202588.top


<!-- 参考信息 -->