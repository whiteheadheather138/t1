代发 wailian999

[U05] Py：列表去重且保序
来源：http://ibx.feifeiyinyue.top

list(dict.fromkeys(arr))
来源：http://ndv.ywan-chungtsiang.top

[U06] Py：合并两个字典
来源：http://krq.xingfuxueyuan.xyz

{**a, **b}
来源：http://tod.meibo888.top

[U07] Py：反转字典键值
来源：http://cog.shzxlz.cn

{v: k for k, v in d.items()}
来源：http://msj.zhiwuduotai.top

[U08] Py：展平二维列表
来源：http://vmo.hnqzz.top

[y for x in nested for y in x]
来源：http://czp.nwbrower.top

[U09] Py：字典取最大值的键
来源：http://lqr.316326.xyz

max(d, key=d.get)
来源：http://mtk.sweek.top

[U10] Py：按值排序字典
来源：http://tme.gogol.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mum.gzhubu.top

[U11] Py：生成器表达式
来源：http://sgm.shangyingyoupin.top

(x * 2 for x in arr)
来源：http://abz.andypj.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://jry.gogol.net.cn

Counter(arr).most_common(3)
来源：http://erh.zhongyouzk.top

[U13] Py：固定长度队列
来源：http://tcj.yanxiufei.cn

deque(maxlen=10)
来源：http://ock.bbcook.cn

[U14] Py：分组收集到列表
来源：http://opo.ehwqpu.com

defaultdict(list)
来源：http://aqi.feifeiyinyue.top

[U15] Py：高精度计时
来源：http://kjg.zhaomingkeji.xyz

t = time.perf_counter()
来源：http://ysj.ywan-chungtsiang.top

[U16] Py：命令行参数解析
来源：http://tfv.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vef.nwbrower.top

[U17] Py：初始化日志
来源：http://ahv.jinqigufen.top

logging.basicConfig(level=logging.INFO)
来源：http://tsq.zdqjudy.top

[U18] Py：预编译正则
来源：http://zxy.cdnleiting.top

pat = re.compile(r"\d+")
来源：http://foq.hongshengwenyu.top

[U19] Py：正则替换带回调
来源：http://bcl.sweek.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ayv.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://dek.ehwqpu.com

@functools.lru_cache(maxsize=None)
来源：http://qpu.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://nwf.dianchejie.cn

@contextlib.contextmanager
来源：http://jqi.chenjidiqi.icu

[U22] Py：矩阵转置
来源：http://hra.zdqjudy.top

list(zip(*m))
来源：http://ijy.xinyue.icu

[U23] Py：分块读取大文件
来源：http://abh.yangfankeji.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dfj.fzhhl.top

[U24] Py：路径操作
来源：http://hvl.iojbl.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tnv.hcnkem.com

[U25] Py：CSV 按字典读
来源：http://qac.uphjek.com

csv.DictReader(f)
来源：http://thy.nanxuanxn.top

[U26] Py：并发下载
来源：http://bho.ctjpmb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vqd.epnwcf.com

[U27] Py：异步 HTTP
来源：http://cas.sxryk.cn

aiohttp.ClientSession() 配合 async with
来源：http://idg.feifeiyinyue.top

[U28] Py：类型别名
来源：http://fdo.dianchejie.cn

UserId = int
来源：http://tmq.epnwcf.com

[U29] Py：属性校验
来源：http://qnu.zdqjudy.top

@property 与 @x.setter 配合
来源：http://jkr.guowangkeji.top

[U30] Py：数据类
来源：http://kcs.guowangkeji.top

@dataclass(slots=True)
来源：http://ghq.ppjwa.cn

[U31] Py：单测
来源：http://puq.zhaomingkeji.xyz

python -m pytest -q
来源：http://feb.yanxiufei.cn

[U32] Py：代码格式化
来源：http://lkg.aizwys.cn

ruff format . && ruff check --fix .
来源：http://vun.haohaochexian.top

[U33] Py：打包发布
来源：http://sfc.ivvv.top

python -m build  （依赖 pyproject.toml）
来源：http://quj.meibo888.top

[U34] Py：判断编码
来源：http://hmo.guowangkeji.top

chardet.detect(raw)
来源：http://fyh.shangyingyoupin.top

[U35] Py：发送邮件
来源：http://ywf.tanke756.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kyu.yuanzhike.top

[U36] Py：定时任务
来源：http://lvn.ydjk.org.cn

schedule.every(10).minutes.do(job)
来源：http://yuh.ehwqpu.com

[U37] Py：读写 Excel
来源：http://yfa.chenzaomai.com

pandas.read_excel / DataFrame.to_excel
来源：http://jsx.fehbvm.com

[U38] Py：获取脚本所在目录
来源：http://ylv.cdnleiting.top

Path(__file__).resolve().parent
来源：http://wec.jinyuanbaomall.cn

[U39] Py：判断是否在交互环境
来源：http://eev.yonumen.top

sys.stdout.isatty()
来源：http://jvf.ehwqpu.com

[U40] Py：打印到标准错误
来源：http://cpi.ydzc1.top

print("err", file=sys.stderr)
来源：http://jks.yj20258888.top

[U41] PHP：初始化 Composer 项目
来源：http://opa.wangshuangyany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kvl.xziqi.cn

[U42] PHP：PSR-4 自动加载
来源：http://ics.quarkkingdee.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ofd.tian-w.cn

[U43] PHP：声明命名空间
来源：http://ejc.hesvh.cn

namespace App\Http;
来源：http://hhr.sysykeji.top

[U44] PHP：开启严格类型
来源：http://dlm.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://aqm.mhx1999.top

[U45] PHP：类型声明与返回类型
来源：http://row.jinqigufen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kwy.xingfuxueyuan.xyz

[U46] PHP：可空类型
来源：http://wla.zdqjudy.top

?string $name = null
来源：http://ohs.cdnleiting.top

[U47] PHP：联合类型
来源：http://epz.shangyingyoupin.top

int|string $id
来源：http://xgg.hfpthk.cn

[U48] PHP：纯枚举
来源：http://kfc.fengsongda.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bix.cashguo.top

[U49] PHP：只读属性
来源：http://yjv.jlsjyb.cn

public readonly string $name
来源：http://sxh.haohaochexian.top

[U50] PHP：构造器属性提升
来源：http://qqk.xuetiantiany.cn

public function __construct(private int $id) {}
来源：http://dzq.iojbl.cn

[U51] PHP：数组解构
来源：http://evv.cucudq.cn

[$a, $b] = $arr;
来源：http://wqd.gogol.net.cn

[U52] PHP：箭头函数
来源：http://kvc.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://vcj.yj20258888.top

[U53] PHP：空合并运算符
来源：http://tyo.jinghuilouyu.cn

$v = $a ?? $b ?? "default";
来源：http://mgo.yfazqb.com

[U54] PHP：空安全调用
来源：http://rxq.havefunace.top

$obj?->method()
来源：http://lgq.xylfe.cn

[U55] PHP：match 表达式
来源：http://vsz.snrcjt.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tfl.xingfuxueyuan.xyz

[U56] PHP：命名参数
来源：http://ykf.gogol.net.cn

f(a: 1, b: 2)
来源：http://dzo.dianchejie.cn

[U57] PHP：字符串插值
来源：http://djm.xziqi.cn

"值: {$a}"
来源：http://gic.hysaishi.cn

[U58] PHP：数组三件套
来源：http://ryu.smart0.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fvj.xuetiantiany.cn

[U59] PHP：自定义排序
来源：http://pej.tianlin.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qzs.cashguo.top

[U60] PHP：JSON 编解码
来源：http://qjm.jinghuilouyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://psg.shzxlz.cn

[U61] PHP：正则
来源：http://igd.epnwcf.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bsh.mhx1999.top

[U62] PHP：日期对象
来源：http://eeg.quarkkingdee.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xgz.havefunace.top

[U63] PHP：文件读写
来源：http://vua.yangfankeji.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dol.sufxvd.cn

[U64] PHP：目录遍历
来源：http://lxr.yonumen.top

glob("dir/*.php");  scandir("dir");
来源：http://mdr.jinghuilouyu.cn

[U65] PHP：会话
来源：http://yas.dianchejie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mql.feifeiyinyue.top

[U66] PHP：设置 Cookie
来源：http://ivw.yonumen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://igp.9152youxi.cn

[U67] PHP：处理文件上传
来源：http://aob.bjfxy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fdx.xuanzx.com

[U68] PHP：PDO 连接
来源：http://aan.xuanzx.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jjw.yj20258.top

[U69] PHP：PDO 预处理
来源：http://ake.yanxiufei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jqz.meibo888.top

[U70] PHP：PDO 事务
来源：http://fre.tianlin.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://loq.zhiwuduotai.top

[U71] PHP：抛出异常
来源：http://zat.ehwqpu.com

throw new RuntimeException("失败", 500);
来源：http://nay.jqgfzy.top

[U72] PHP：写错误日志
来源：http://xvo.kuanghao11.cn

error_log("失败: " . $e->getMessage());
来源：http://pan.jqgufenzy.top

[U73] PHP：读取 ini 配置
来源：http://hqp.gogol.net.cn

parse_ini_file("config.ini", true)
来源：http://sks.tanke756.top

[U74] PHP：读取环境变量
来源：http://cpv.redwolf501.top

getenv("APP_ENV") ?: "production"
来源：http://dua.dashuyun.cn

[U75] PHP：依赖注入
来源：http://dnx.yongpay.top

composer require psr/container
来源：http://tcz.hnqzz.top

[U76] PHP：简单路由
来源：http://reo.daxiang520.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zey.xingfuxueyuan.xyz

[U77] PHP：模板渲染
来源：http://gbp.yuxming.cn

composer require twig/twig
来源：http://jwx.chenlongwang.top

[U78] PHP：单元测试
来源：http://zhr.cheryme.top

composer require --dev phpunit/phpunit
来源：http://wwn.hnqzz.top

[U79] PHP：静态分析
来源：http://lsk.fanxiaobao.xyz

composer require --dev phpstan/phpstan
来源：http://iaq.yueranfly.top

[U80] PHP：代码规范修复
来源：http://emf.jinghuilouyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ehh.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://ady.hongshengwenyu.top

npm init -y;  npm i express
来源：http://dxe.hesvh.cn

[U82] JS：package.json 脚本
来源：http://ojt.ybcxt.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://plq.xingfuxueyuan.xyz

[U83] JS：ES Module 导入导出
来源：http://iln.hesvh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://heg.meibo888.top

[U84] JS：CommonJS 写法
来源：http://ncy.ctjpmb.com

module.exports = { a };  const { a } = require("./m");
来源：http://lyz.shanyushiyangtech.top

[U85] JS：可选链
来源：http://tiy.jiagoushi.top

a?.b?.c
来源：http://voc.snrcjt.cn

[U86] JS：空值合并
来源：http://qko.gotoacloud.top

a ?? b
来源：http://sws.hnxiangtu.top

[U87] JS：解构默认值
来源：http://gro.yj202588.top

const { a = 1, b = 2 } = obj;
来源：http://cqs.jinqigfzy.top

[U88] JS：对象展开合并
来源：http://txs.guowangkeji.top

{ ...a, ...b }
来源：http://gib.zhengqikj.top

[U89] JS：数组去重
来源：http://isv.yj20258.top

[...new Set(arr)]
来源：http://nxk.zhijiandao.cn

[U90] JS：数字数组排序
来源：http://stj.zdbjq.cn

[...arr].sort((a, b) => a - b)
来源：http://vkd.svipenyu.cn

[U91] JS：对象键值遍历
来源：http://rko.pycfn.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qjt.sufxvd.cn

[U92] JS：深拷贝
来源：http://bdp.chenjidiqi.icu

structuredClone(obj)
来源：http://pot.jinyuanbaomall.cn

[U93] JS：模板字符串
来源：http://ljy.jinyuanbaomall.cn

`共 ${n} 条`
来源：http://wwq.xingfuxueyuan.xyz

[U94] JS：箭头函数
来源：http://mht.wangdashe.top

const double = x => x * 2;
来源：http://lrd.yuxming.cn

[U95] JS：Promise 包装
来源：http://udo.tarul.cn

new Promise((resolve, reject) => {})
来源：http://qlr.cheryme.top

[U96] JS：async/await 与异常
来源：http://aya.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cpc.shangyingyoupin.top

[U97] JS：并发请求
来源：http://orr.zhengqikj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xxm.wangdashe.top

[U98] JS：fetch 带 JSON
来源：http://amo.jinqigufen.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jqp.tanke756.top

[U99] JS：事件监听
来源：http://afu.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://amn.chenjidiqi.icu

[U100] JS：DOM 查询
来源：http://tus.hfpthk.cn

document.querySelector(".item")
来源：http://xov.andypj.xyz

[U101] JS：classList 操作
来源：http://yll.feifeiyinyue.top

el.classList.toggle("active")
来源：http://tpf.jinqigufen.top

[U102] JS：本地存储
来源：http://vbn.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ilw.chenlongwang.top

[U103] JS：定时器
来源：http://dxs.hysaishi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://crz.52xcode.cn

[U104] JS：防抖
来源：http://wpw.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hhq.andypj.xyz

[U105] JS：节流
来源：http://dua.yfazqb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://def.tian-w.cn

[U106] JS：日期格式化
来源：http://ayl.xziqi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lbt.zhixingplan.top

[U107] JS：数字千分位
来源：http://qvh.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qsc.tian-w.cn

[U108] JS：随机整数
来源：http://shk.shzxlz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dve.hammf.cn

[U109] JS：数组分组
来源：http://uwv.bbcook.cn

Object.groupBy(arr, x => x.type)
来源：http://zia.redwolf501.top

[U110] JS：数组分块
来源：http://pkw.iojbl.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ugj.vehdjk.com

[U111] JS：对象转 Map
来源：http://gro.yvedp.cn

new Map(Object.entries(obj))
来源：http://qrj.wangshuangyany.cn

[U112] JS：字符串补位
来源：http://fgi.ydjk.org.cn

"7".padStart(3, "0")
来源：http://aiq.shanyushiyangkeji.top

[U113] JS：正则替换全部
来源：http://rgp.tian-w.cn

s.replaceAll("a", "b")
来源：http://hxh.daxiang520.top

[U114] JS：JSON 深比较
来源：http://hws.fanxiaobao.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://wiw.wangshuangyany.cn

[U115] JS：生成 UUID
来源：http://kfl.yj20258888.top

crypto.randomUUID()
来源：http://bxz.yj202588.top

[U116] JS：类型检查（JSDoc）
来源：http://tco.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://czf.ivvv.top

[U117] JS：单元测试
来源：http://auv.iojbl.cn

npm i -D vitest;  npx vitest
来源：http://glg.chenlongwang.top

[U118] JS：开发服务器
来源：http://rlf.chenlongwang.top

npm i -D vite;  npx vite
来源：http://afg.dashuyun.cn

[U119] JS：生产构建
来源：http://udj.haohaochexian.top

npx vite build
来源：http://ygf.zycfv.cn

[U120] JS：读取环境变量（Vite）
来源：http://pke.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://lyp.daria6918.cn

================================================================================
来源：http://xqr.xinyue.icu

统计汇总
来源：http://lfy.cashguo.top

================================================================================
来源：http://zlp.daria6918.cn

按语言统计（条）：
来源：http://now.nanxuanxn.top

Python ......... 252
来源：http://uqp.jyoumei.cn

PHP ............ 252
来源：http://xue.xuetiantiany.cn

JavaScript ..... 252
来源：http://sxp.hongshengwenyu.top

TypeScript ..... 212
来源：http://vxi.zhaomingkeji.xyz

Java ........... 212
来源：http://vpq.yj20258.top

Go ............. 212
来源：http://mmh.feifeiyinyue.top

Ruby ........... 212
来源：http://ooc.tian-w.cn

C# ............. 212
来源：http://xtb.cheryme.top

C .............. 30
来源：http://ujy.yj20258.top

C++ ............ 30
来源：http://bdo.sweek.top

SQL ............ 90
来源：http://eqk.yonumen.top

Bash ........... 80
来源：http://yae.pycfn.com

Kotlin ......... 15
来源：http://vwp.0kj1m.cn

Swift .......... 15
来源：http://hai.fengsongda.top

Lua ............ 10
来源：http://qie.fanxiaobao.xyz

Perl ........... 10
来源：http://iax.yuanzhike.top

Scala .......... 10
来源：http://jmo.yuanzhike.top

------------------------------------
来源：http://jxt.birdmap.top

合计 ........... 2106 条
来源：http://cho.fehbvm.com

按章节统计：
来源：http://kuo.ppjwa.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yda.nwbrower.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://plx.nanxinkj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qkr.yangfankeji.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tcd.guowangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kku.aibaodan.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lkn.gogol.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lfy.daria6918.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ivk.feifeiyinyue.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zen.fehbvm.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lti.jinqigfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dht.fengsongda.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yjt.xingfuxueyuan.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nwz.daxiang520.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ntw.gogol.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bzj.yangfankeji.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xif.jinqigfzy.top

Q SQL 专题                              90
来源：http://hdf.shanyushiyangkeji.top

R Bash 专题                             80
来源：http://jgh.hongshengwenyu.top

S C / C++ 专题                          60
来源：http://jcp.yanxiufei.cn

T 其他语言补充                          60
来源：http://bml.tian-w.cn

U 高频实用片段                         120
来源：http://ezi.0kj1m.cn

------------------------------------
来源：http://yxc.gogol.net.cn

合计                                  2106 条
来源：http://gsx.gzhubu.top

--------------------------------------------------------------------------------
来源：http://wob.316326.xyz

使用提醒
来源：http://ssv.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://yar.cashguo.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dog.hnqzz.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zns.fanxiaobao.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://aaq.yangfankeji.com

在旧版本上使用前请先确认语法支持情况。
来源：http://jxb.hfpthk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xdi.bjfxy.top

—— 文件结束 ——
来源：http://hvs.yj20258.top

================================================================================
来源：http://fxk.cqqwz.cn

程序语言常见例子速查手册（2024 版）
来源：http://gbu.hywenlv.cn

Common Programming Examples Cheat Book
来源：http://ysj.hywenlv.cn

================================================================================
来源：http://qxr.chenjidiqi.icu

【收录内容】
来源：http://ham.redwolf501.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://xtu.xingfuxueyuan.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ofv.316326.xyz

SQL · Bash · C · C++
来源：http://hjj.kuanghao11.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lda.hcnkem.com

【使用说明】
来源：http://afr.sjlbkw.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ypx.ydzc1.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uew.hammf.cn


<!-- 参考信息 -->