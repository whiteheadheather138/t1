代发 wailian999

[U05] Py：列表去重且保序
来源：http://psm.xuetiantiany.cn

list(dict.fromkeys(arr))
来源：http://own.zdbjq.cn

[U06] Py：合并两个字典
来源：http://ful.hnqzz.top

{**a, **b}
来源：http://dqp.0kj1m.cn

[U07] Py：反转字典键值
来源：http://nyp.jinyuanbaomall.cn

{v: k for k, v in d.items()}
来源：http://abs.dianchejie.cn

[U08] Py：展平二维列表
来源：http://gvz.52xcode.cn

[y for x in nested for y in x]
来源：http://znk.zhijiandao.cn

[U09] Py：字典取最大值的键
来源：http://ohw.hammf.cn

max(d, key=d.get)
来源：http://ajk.ywan-chungtsiang.top

[U10] Py：按值排序字典
来源：http://mii.quarkkingdee.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ije.52xcode.cn

[U11] Py：生成器表达式
来源：http://sgg.yuxming.cn

(x * 2 for x in arr)
来源：http://wdk.mhx1999.top

[U12] Py：取出现最多的 3 个元素
来源：http://wtr.cheryme.top

Counter(arr).most_common(3)
来源：http://snx.fanxiaobao.xyz

[U13] Py：固定长度队列
来源：http://kme.gaohongyu789.top

deque(maxlen=10)
来源：http://adn.uphjek.com

[U14] Py：分组收集到列表
来源：http://trc.jqgufenzy.top

defaultdict(list)
来源：http://xhu.chenjidiqi.icu

[U15] Py：高精度计时
来源：http://pim.tianlin.xyz

t = time.perf_counter()
来源：http://mvg.snrcjt.cn

[U16] Py：命令行参数解析
来源：http://gdh.pycfn.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ouh.zdbjq.cn

[U17] Py：初始化日志
来源：http://qkh.wangshuangyany.cn

logging.basicConfig(level=logging.INFO)
来源：http://let.jinyuanbaomall.cn

[U18] Py：预编译正则
来源：http://ano.sysykeji.top

pat = re.compile(r"\d+")
来源：http://prw.wangdashe.top

[U19] Py：正则替换带回调
来源：http://xxb.aizwys.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lug.jqgfzy.top

[U20] Py：缓存函数结果
来源：http://wlw.yuanzhike.top

@functools.lru_cache(maxsize=None)
来源：http://ufo.daria6918.cn

[U21] Py：自定义上下文管理器
来源：http://ott.pycfn.com

@contextlib.contextmanager
来源：http://bao.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://dct.fengsongda.top

list(zip(*m))
来源：http://taf.yj20258888.top

[U23] Py：分块读取大文件
来源：http://umb.zhixingplan.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qbc.sysykeji.top

[U24] Py：路径操作
来源：http://azs.nanxuanxn.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eqd.fengsongda.top

[U25] Py：CSV 按字典读
来源：http://ztn.xylfe.cn

csv.DictReader(f)
来源：http://cwn.hywenlv.cn

[U26] Py：并发下载
来源：http://vca.yvedp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ooc.ppjwa.cn

[U27] Py：异步 HTTP
来源：http://fcw.hfpthk.cn

aiohttp.ClientSession() 配合 async with
来源：http://vwz.tian-w.cn

[U28] Py：类型别名
来源：http://ndm.zhongyouzk.top

UserId = int
来源：http://fsh.ybcxt.top

[U29] Py：属性校验
来源：http://pmk.hysaishi.cn

@property 与 @x.setter 配合
来源：http://met.c1oappe.top

[U30] Py：数据类
来源：http://xtb.svipenyu.cn

@dataclass(slots=True)
来源：http://iuk.fengsongda.top

[U31] Py：单测
来源：http://wpd.shzxlz.cn

python -m pytest -q
来源：http://cbc.snrcjt.cn

[U32] Py：代码格式化
来源：http://ica.aibaodan.cn

ruff format . && ruff check --fix .
来源：http://kfu.fehbvm.com

[U33] Py：打包发布
来源：http://wyx.jinqigfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://wuq.feifeiyinyue.top

[U34] Py：判断编码
来源：http://fil.bbcook.cn

chardet.detect(raw)
来源：http://dmx.dashuyun.cn

[U35] Py：发送邮件
来源：http://bov.xingfuxueyuan.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tuu.aibaodan.cn

[U36] Py：定时任务
来源：http://hrm.chenlongwang.top

schedule.every(10).minutes.do(job)
来源：http://nhh.xylfe.cn

[U37] Py：读写 Excel
来源：http://fjk.nanxinkj.top

pandas.read_excel / DataFrame.to_excel
来源：http://msc.ppjwa.cn

[U38] Py：获取脚本所在目录
来源：http://gsr.xylfe.cn

Path(__file__).resolve().parent
来源：http://wqc.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://dwd.hysaishi.cn

sys.stdout.isatty()
来源：http://yrn.xylfe.cn

[U40] Py：打印到标准错误
来源：http://rfz.jqgfzy.top

print("err", file=sys.stderr)
来源：http://zwc.meibo888.top

[U41] PHP：初始化 Composer 项目
来源：http://qjp.jqgfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ubq.hnxiangtu.top

[U42] PHP：PSR-4 自动加载
来源：http://kxc.cheryme.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sbl.jlsjyb.cn

[U43] PHP：声明命名空间
来源：http://zxq.jqgfzy.top

namespace App\Http;
来源：http://ikx.pycfn.com

[U44] PHP：开启严格类型
来源：http://war.pycfn.com

declare(strict_types=1);
来源：http://hux.zdqjudy.top

[U45] PHP：类型声明与返回类型
来源：http://bjx.yuanzhike.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ehi.xinyue.icu

[U46] PHP：可空类型
来源：http://fxk.wangdashe.top

?string $name = null
来源：http://qzi.chenzaomai.com

[U47] PHP：联合类型
来源：http://ovs.hysaishi.cn

int|string $id
来源：http://pzq.cqqwz.cn

[U48] PHP：纯枚举
来源：http://xcw.jqgfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zmd.meibo888.top

[U49] PHP：只读属性
来源：http://eum.hammf.cn

public readonly string $name
来源：http://tgv.jqgfzy.top

[U50] PHP：构造器属性提升
来源：http://zzr.dianchejie.cn

public function __construct(private int $id) {}
来源：http://diz.feifeiyinyue.top

[U51] PHP：数组解构
来源：http://vup.sxryk.cn

[$a, $b] = $arr;
来源：http://ceo.ehwqpu.com

[U52] PHP：箭头函数
来源：http://tty.feifeiyinyue.top

$double = fn($x) => $x * 2;
来源：http://mwx.hywenlv.cn

[U53] PHP：空合并运算符
来源：http://aep.tian-w.cn

$v = $a ?? $b ?? "default";
来源：http://uzd.tanke756.top

[U54] PHP：空安全调用
来源：http://jnc.nwbrower.top

$obj?->method()
来源：http://ihw.c1oappe.top

[U55] PHP：match 表达式
来源：http://see.chenzaomai.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qes.yonumen.top

[U56] PHP：命名参数
来源：http://ykv.zhongyouzk.top

f(a: 1, b: 2)
来源：http://cry.sysykeji.top

[U57] PHP：字符串插值
来源：http://mdp.xingfuxueyuan.xyz

"值: {$a}"
来源：http://ekd.zdqjudy.top

[U58] PHP：数组三件套
来源：http://oor.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fee.bjfxy.top

[U59] PHP：自定义排序
来源：http://let.ehwqpu.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fyp.guowangkeji.top

[U60] PHP：JSON 编解码
来源：http://iuc.0kj1m.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ust.316326.xyz

[U61] PHP：正则
来源：http://pys.bjfxy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ijt.52xcode.cn

[U62] PHP：日期对象
来源：http://amj.gzhubu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rma.yangfankeji.com

[U63] PHP：文件读写
来源：http://vgu.tarul.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ydu.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://oci.fehbvm.com

glob("dir/*.php");  scandir("dir");
来源：http://llr.bjfxy.top

[U65] PHP：会话
来源：http://cde.zhiwuduotai.top

session_start();  $_SESSION["uid"] = 1;
来源：http://agj.pengpengdd.cyou

[U66] PHP：设置 Cookie
来源：http://syh.ydjk.org.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ksc.yfazqb.com

[U67] PHP：处理文件上传
来源：http://svu.hywenlv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://puu.xinyue.icu

[U68] PHP：PDO 连接
来源：http://tvb.hnxiangtu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dqr.yfazqb.com

[U69] PHP：PDO 预处理
来源：http://bad.cashguo.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hux.tianlin.xyz

[U70] PHP：PDO 事务
来源：http://jqo.cheryme.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mug.quarkkingdee.top

[U71] PHP：抛出异常
来源：http://tbn.zhaomingkeji.xyz

throw new RuntimeException("失败", 500);
来源：http://szk.shangyingyoupin.top

[U72] PHP：写错误日志
来源：http://unr.aizwys.cn

error_log("失败: " . $e->getMessage());
来源：http://xhr.zycfv.cn

[U73] PHP：读取 ini 配置
来源：http://aek.fehbvm.com

parse_ini_file("config.ini", true)
来源：http://dij.birdmap.top

[U74] PHP：读取环境变量
来源：http://aty.chenlongwang.top

getenv("APP_ENV") ?: "production"
来源：http://pqo.kuanghao11.cn

[U75] PHP：依赖注入
来源：http://igu.xylfe.cn

composer require psr/container
来源：http://gyr.redwolf501.top

[U76] PHP：简单路由
来源：http://iaq.9152youxi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qww.shanyushiyangtech.top

[U77] PHP：模板渲染
来源：http://plq.quarkkingdee.top

composer require twig/twig
来源：http://xlw.jlsjyb.cn

[U78] PHP：单元测试
来源：http://fii.zycfv.cn

composer require --dev phpunit/phpunit
来源：http://elg.yangfankeji.com

[U79] PHP：静态分析
来源：http://qcq.daria6918.cn

composer require --dev phpstan/phpstan
来源：http://aos.cheryme.top

[U80] PHP：代码规范修复
来源：http://vgl.jinqigufen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ujm.fanxiaobao.xyz

[U81] JS：初始化项目
来源：http://lqh.xuanzx.com

npm init -y;  npm i express
来源：http://skm.andypj.xyz

[U82] JS：package.json 脚本
来源：http://yhj.chenlongwang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mfj.smart0.xyz

[U83] JS：ES Module 导入导出
来源：http://rde.ctjpmb.com

export const a = 1;  import { a } from "./m.js";
来源：http://cmq.hammf.cn

[U84] JS：CommonJS 写法
来源：http://lzh.sxryk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tvs.sweek.top

[U85] JS：可选链
来源：http://pbi.uphjek.com

a?.b?.c
来源：http://adx.yvedp.cn

[U86] JS：空值合并
来源：http://teb.zdqjudy.top

a ?? b
来源：http://bvy.yj20258.top

[U87] JS：解构默认值
来源：http://pax.jianghu66.top

const { a = 1, b = 2 } = obj;
来源：http://wez.zhixingplan.top

[U88] JS：对象展开合并
来源：http://fip.haohaochexian.top

{ ...a, ...b }
来源：http://ycb.hnxiangtu.top

[U89] JS：数组去重
来源：http://roy.hesvh.cn

[...new Set(arr)]
来源：http://xlj.haohaochexian.top

[U90] JS：数字数组排序
来源：http://hhn.tarul.cn

[...arr].sort((a, b) => a - b)
来源：http://ygi.andypj.xyz

[U91] JS：对象键值遍历
来源：http://nbj.hnqzz.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hin.jianghu66.top

[U92] JS：深拷贝
来源：http://pzi.yanxiufei.cn

structuredClone(obj)
来源：http://jtw.zhiwuduotai.top

[U93] JS：模板字符串
来源：http://jqw.meibo888.top

`共 ${n} 条`
来源：http://egk.zdqjudy.top

[U94] JS：箭头函数
来源：http://zmd.yueranfly.top

const double = x => x * 2;
来源：http://mbv.shuidangran.top

[U95] JS：Promise 包装
来源：http://gbe.jqgfzy.top

new Promise((resolve, reject) => {})
来源：http://rpr.ctjpmb.com

[U96] JS：async/await 与异常
来源：http://usz.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qyy.snrcjt.cn

[U97] JS：并发请求
来源：http://gcb.pengpengdd.cyou

await Promise.all(urls.map(u => fetch(u)))
来源：http://vxe.tianlin.xyz

[U98] JS：fetch 带 JSON
来源：http://tci.andypj.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uuh.sweek.top

[U99] JS：事件监听
来源：http://bgg.xylfe.cn

el.addEventListener("click", e => {})
来源：http://cbb.guowangkeji.top

[U100] JS：DOM 查询
来源：http://yle.dianchejie.cn

document.querySelector(".item")
来源：http://cqb.snrcjt.cn

[U101] JS：classList 操作
来源：http://anc.c1oappe.top

el.classList.toggle("active")
来源：http://wrt.shangyingyoupin.top

[U102] JS：本地存储
来源：http://grg.shanyushiyangtech.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wcr.tianlin.xyz

[U103] JS：定时器
来源：http://khh.redwolf501.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fiv.fzhhl.top

[U104] JS：防抖
来源：http://nzl.dianchejie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wsc.hnxiangtu.top

[U105] JS：节流
来源：http://cnp.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ohf.c1oappe.top

[U106] JS：日期格式化
来源：http://usf.0kj1m.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nbt.yvedp.cn

[U107] JS：数字千分位
来源：http://for.yangfankeji.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wgm.hesvh.cn

[U108] JS：随机整数
来源：http://xll.jqgufenzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://deu.hfpthk.cn

[U109] JS：数组分组
来源：http://txf.xuetiantiany.cn

Object.groupBy(arr, x => x.type)
来源：http://erm.zhaomingkeji.xyz

[U110] JS：数组分块
来源：http://pir.jyoumei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wvd.vqdsnc.cn

[U111] JS：对象转 Map
来源：http://mbz.daria6918.cn

new Map(Object.entries(obj))
来源：http://nni.jinyuanbaomall.cn

[U112] JS：字符串补位
来源：http://rod.shanyushiyangtech.top

"7".padStart(3, "0")
来源：http://vnc.zhixingplan.top

[U113] JS：正则替换全部
来源：http://edd.xziqi.cn

s.replaceAll("a", "b")
来源：http://pok.jlsjyb.cn

[U114] JS：JSON 深比较
来源：http://xjf.fengsongda.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fol.epnwcf.com

[U115] JS：生成 UUID
来源：http://mlu.snrcjt.cn

crypto.randomUUID()
来源：http://shd.gotoacloud.top

[U116] JS：类型检查（JSDoc）
来源：http://cci.birdmap.top

/** @param {string} name */ function f(name) {}
来源：http://lnc.sweek.top

[U117] JS：单元测试
来源：http://scx.52xcode.cn

npm i -D vitest;  npx vitest
来源：http://idg.shzxlz.cn

[U118] JS：开发服务器
来源：http://dyv.hongshengwenyu.top

npm i -D vite;  npx vite
来源：http://nyl.shanyushiyangtech.top

[U119] JS：生产构建
来源：http://owv.dashuyun.cn

npx vite build
来源：http://xbl.smart0.xyz

[U120] JS：读取环境变量（Vite）
来源：http://hzz.shuidangran.top

import.meta.env.VITE_API_URL
来源：http://dzq.jinqigufen.top

================================================================================
来源：http://czc.uphjek.com

统计汇总
来源：http://qjh.havefunace.top

================================================================================
来源：http://wvc.ybcxt.top

按语言统计（条）：
来源：http://gje.hysaishi.cn

Python ......... 252
来源：http://cxj.havefunace.top

PHP ............ 252
来源：http://gny.chenlongwang.top

JavaScript ..... 252
来源：http://udp.nanxuanxn.top

TypeScript ..... 212
来源：http://csl.cheryme.top

Java ........... 212
来源：http://xca.zhaomingkeji.xyz

Go ............. 212
来源：http://taw.guannengcc.top

Ruby ........... 212
来源：http://beb.wangdashe.top

C# ............. 212
来源：http://tpw.snrcjt.cn

C .............. 30
来源：http://hzp.tarul.cn

C++ ............ 30
来源：http://cyy.shanyushiyangkeji.top

SQL ............ 90
来源：http://hzy.wangshuangyany.cn

Bash ........... 80
来源：http://kul.shangyingyoupin.top

Kotlin ......... 15
来源：http://tth.guannengcc.top

Swift .......... 15
来源：http://soh.guannengcc.top

Lua ............ 10
来源：http://szu.chenlongwang.top

Perl ........... 10
来源：http://fsm.uphjek.com

Scala .......... 10
来源：http://fvk.jqgufenzy.top

------------------------------------
来源：http://rok.tanke756.top

合计 ........... 2106 条
来源：http://igq.zhijiandao.cn

按章节统计：
来源：http://qxy.snrcjt.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bli.gogol.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eqy.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://idv.ywan-chungtsiang.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vov.feifeiyinyue.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vvw.zhijiandao.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://snm.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://icn.wangdashe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uti.andypj.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ynv.vehdjk.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baa.zhiwuduotai.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jmd.cdnleiting.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://myp.jqgufenzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uej.yueranfly.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zif.wangshuangyany.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rej.haohaochexian.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://spt.zhiwuduotai.top

Q SQL 专题                              90
来源：http://zhl.jinghuilouyu.cn

R Bash 专题                             80
来源：http://bts.wangshuangyany.cn

S C / C++ 专题                          60
来源：http://ljr.zhoulong.xyz

T 其他语言补充                          60
来源：http://kme.bbcook.cn

U 高频实用片段                         120
来源：http://lzk.jianghu66.top

------------------------------------
来源：http://zjd.tanke756.top

合计                                  2106 条
来源：http://mfx.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://hst.yfazqb.com

使用提醒
来源：http://xij.fengsongda.top

--------------------------------------------------------------------------------
来源：http://ahf.chenlongwang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://odw.zhoulong.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ghh.guannengcc.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yuo.xingfuxueyuan.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://kkd.jianghu66.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wif.tanke756.top

—— 文件结束 ——
来源：http://wvr.yj20258.top

================================================================================
来源：http://kfb.ctjpmb.com

程序语言常见例子速查手册（2024 版）
来源：http://bbj.zhongyouzk.top

Common Programming Examples Cheat Book
来源：http://stb.xinyue.icu

================================================================================
来源：http://kto.yfazqb.com

【收录内容】
来源：http://hlb.pycfn.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://frw.zdbjq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cmi.epnwcf.com

SQL · Bash · C · C++
来源：http://prx.feifeiyinyue.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pgz.yanxiufei.cn

【使用说明】
来源：http://bno.ydjk.org.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qfa.aizwys.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qph.yongpay.top


<!-- 参考信息 -->