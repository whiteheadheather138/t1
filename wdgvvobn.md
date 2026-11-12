代发 wailian999

[U05] Py：列表去重且保序
来源：http://vqw.svipenyu.cn

list(dict.fromkeys(arr))
来源：http://idl.snrcjt.cn

[U06] Py：合并两个字典
来源：http://osb.shanyushiyangkeji.top

{**a, **b}
来源：http://nir.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://rjn.nanxuanxn.top

{v: k for k, v in d.items()}
来源：http://jhn.nanxinkj.top

[U08] Py：展平二维列表
来源：http://dgb.jqgufenzy.top

[y for x in nested for y in x]
来源：http://ouu.hongshengwenyu.top

[U09] Py：字典取最大值的键
来源：http://crl.kuanghao11.cn

max(d, key=d.get)
来源：http://lgl.bbcook.cn

[U10] Py：按值排序字典
来源：http://pzs.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wwy.316326.xyz

[U11] Py：生成器表达式
来源：http://ktv.guannengcc.top

(x * 2 for x in arr)
来源：http://eec.epnwcf.com

[U12] Py：取出现最多的 3 个元素
来源：http://hke.xinyue.icu

Counter(arr).most_common(3)
来源：http://wkt.kuanghao11.cn

[U13] Py：固定长度队列
来源：http://mtu.ywan-chungtsiang.top

deque(maxlen=10)
来源：http://wxk.aibaodan.cn

[U14] Py：分组收集到列表
来源：http://sfi.andypj.xyz

defaultdict(list)
来源：http://yzh.sysykeji.top

[U15] Py：高精度计时
来源：http://htj.xylfe.cn

t = time.perf_counter()
来源：http://cmr.daxiang520.top

[U16] Py：命令行参数解析
来源：http://wfu.xziqi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://spl.xziqi.cn

[U17] Py：初始化日志
来源：http://yhf.tian-w.cn

logging.basicConfig(level=logging.INFO)
来源：http://fbp.jianghu66.top

[U18] Py：预编译正则
来源：http://bdc.yongpay.top

pat = re.compile(r"\d+")
来源：http://meu.tarul.cn

[U19] Py：正则替换带回调
来源：http://srt.vehdjk.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ncd.xylfe.cn

[U20] Py：缓存函数结果
来源：http://ogq.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://hfy.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://kse.zhoulong.xyz

@contextlib.contextmanager
来源：http://yzj.tarul.cn

[U22] Py：矩阵转置
来源：http://fsh.vehdjk.com

list(zip(*m))
来源：http://yph.shanyushiyangtech.top

[U23] Py：分块读取大文件
来源：http://hyc.xuetiantiany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gae.yangfankeji.com

[U24] Py：路径操作
来源：http://wlt.ydzc1.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://irn.zycfv.cn

[U25] Py：CSV 按字典读
来源：http://kbw.nwbrower.top

csv.DictReader(f)
来源：http://ndy.gaohongyu789.top

[U26] Py：并发下载
来源：http://luw.wangdashe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jmo.ydjk.org.cn

[U27] Py：异步 HTTP
来源：http://qxa.yj20258888.top

aiohttp.ClientSession() 配合 async with
来源：http://ovg.tianlin.xyz

[U28] Py：类型别名
来源：http://zie.feifeiyinyue.top

UserId = int
来源：http://har.sxryk.cn

[U29] Py：属性校验
来源：http://tzw.xinyue.icu

@property 与 @x.setter 配合
来源：http://fzt.jinqigufen.top

[U30] Py：数据类
来源：http://zkv.ctjpmb.com

@dataclass(slots=True)
来源：http://odr.shuidangran.top

[U31] Py：单测
来源：http://gzs.zhiwuduotai.top

python -m pytest -q
来源：http://mth.ehwqpu.com

[U32] Py：代码格式化
来源：http://chs.jiagoushi.top

ruff format . && ruff check --fix .
来源：http://axs.shzxlz.cn

[U33] Py：打包发布
来源：http://smz.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://myd.dianchejie.cn

[U34] Py：判断编码
来源：http://dea.cheryme.top

chardet.detect(raw)
来源：http://llc.yj202588.top

[U35] Py：发送邮件
来源：http://xfc.andypj.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yef.dashuyun.cn

[U36] Py：定时任务
来源：http://chf.chenlongwang.top

schedule.every(10).minutes.do(job)
来源：http://nqn.yonumen.top

[U37] Py：读写 Excel
来源：http://qqw.meibo888.top

pandas.read_excel / DataFrame.to_excel
来源：http://aux.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://xsk.shuidangran.top

Path(__file__).resolve().parent
来源：http://zav.chenjidiqi.icu

[U39] Py：判断是否在交互环境
来源：http://fmv.chenlongwang.top

sys.stdout.isatty()
来源：http://qdj.hcnkem.com

[U40] Py：打印到标准错误
来源：http://ugw.ctjpmb.com

print("err", file=sys.stderr)
来源：http://ceb.dashuyun.cn

[U41] PHP：初始化 Composer 项目
来源：http://grq.ybcxt.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xua.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://wwh.chenzaomai.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xps.zhixingplan.top

[U43] PHP：声明命名空间
来源：http://ayf.jyoumei.cn

namespace App\Http;
来源：http://try.andypj.xyz

[U44] PHP：开启严格类型
来源：http://qug.cashguo.top

declare(strict_types=1);
来源：http://tjb.zhengqikj.top

[U45] PHP：类型声明与返回类型
来源：http://mlz.daxiang520.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://scs.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://hnm.cucudq.cn

?string $name = null
来源：http://etc.redwolf501.top

[U47] PHP：联合类型
来源：http://yfq.tianlin.xyz

int|string $id
来源：http://vxa.epnwcf.com

[U48] PHP：纯枚举
来源：http://ras.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sad.uphjek.com

[U49] PHP：只读属性
来源：http://qws.jlsjyb.cn

public readonly string $name
来源：http://yxk.ywan-chungtsiang.top

[U50] PHP：构造器属性提升
来源：http://vvh.jinqigufen.top

public function __construct(private int $id) {}
来源：http://otx.cqqwz.cn

[U51] PHP：数组解构
来源：http://nec.nanxinkj.top

[$a, $b] = $arr;
来源：http://qvb.iojbl.cn

[U52] PHP：箭头函数
来源：http://jtd.dianchejie.cn

$double = fn($x) => $x * 2;
来源：http://jti.sxryk.cn

[U53] PHP：空合并运算符
来源：http://aui.fktsv.cn

$v = $a ?? $b ?? "default";
来源：http://ddh.iojbl.cn

[U54] PHP：空安全调用
来源：http://dqt.jqgufenzy.top

$obj?->method()
来源：http://tky.xingfuxueyuan.xyz

[U55] PHP：match 表达式
来源：http://xob.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dho.nanxinkj.top

[U56] PHP：命名参数
来源：http://rys.guowangkeji.top

f(a: 1, b: 2)
来源：http://yzi.52xcode.cn

[U57] PHP：字符串插值
来源：http://bom.aizwys.cn

"值: {$a}"
来源：http://quk.tarul.cn

[U58] PHP：数组三件套
来源：http://xyb.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kkq.guannengcc.top

[U59] PHP：自定义排序
来源：http://ubm.shangyingyoupin.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kqb.zycfv.cn

[U60] PHP：JSON 编解码
来源：http://aev.redwolf501.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dfz.jinghuilouyu.cn

[U61] PHP：正则
来源：http://cmo.cheryme.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ics.nanxinkj.top

[U62] PHP：日期对象
来源：http://zdr.cdnleiting.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hvy.cucudq.cn

[U63] PHP：文件读写
来源：http://vll.xingfuxueyuan.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://klu.xziqi.cn

[U64] PHP：目录遍历
来源：http://cie.birdmap.top

glob("dir/*.php");  scandir("dir");
来源：http://lma.xingfuxueyuan.xyz

[U65] PHP：会话
来源：http://clt.hfpthk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cmc.hnxiangtu.top

[U66] PHP：设置 Cookie
来源：http://rrq.ivvv.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cbe.ivvv.top

[U67] PHP：处理文件上传
来源：http://dic.chenjidiqi.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uyj.zhoulong.xyz

[U68] PHP：PDO 连接
来源：http://wrd.cdnleiting.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fqf.hywenlv.cn

[U69] PHP：PDO 预处理
来源：http://dde.zhoulong.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://boq.sweek.top

[U70] PHP：PDO 事务
来源：http://bil.gaohongyu789.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://onq.gzhubu.top

[U71] PHP：抛出异常
来源：http://tgs.zhixingplan.top

throw new RuntimeException("失败", 500);
来源：http://zsa.9152youxi.cn

[U72] PHP：写错误日志
来源：http://wvf.zhiwuduotai.top

error_log("失败: " . $e->getMessage());
来源：http://nky.gotoacloud.top

[U73] PHP：读取 ini 配置
来源：http://cpb.gogol.net.cn

parse_ini_file("config.ini", true)
来源：http://osf.chenlongwang.top

[U74] PHP：读取环境变量
来源：http://bma.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://bxl.sxryk.cn

[U75] PHP：依赖注入
来源：http://izb.jianghu66.top

composer require psr/container
来源：http://fjs.cashguo.top

[U76] PHP：简单路由
来源：http://olm.xuanzx.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wmu.gogol.net.cn

[U77] PHP：模板渲染
来源：http://cnn.hesvh.cn

composer require twig/twig
来源：http://yom.zhaomingkeji.xyz

[U78] PHP：单元测试
来源：http://bcz.shanyushiyangkeji.top

composer require --dev phpunit/phpunit
来源：http://gyp.yuanzhike.top

[U79] PHP：静态分析
来源：http://vbe.ctjpmb.com

composer require --dev phpstan/phpstan
来源：http://ise.fanxiaobao.xyz

[U80] PHP：代码规范修复
来源：http://wuz.hongshengwenyu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jgj.vqdsnc.cn

[U81] JS：初始化项目
来源：http://qef.shangyingyoupin.top

npm init -y;  npm i express
来源：http://wzg.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://fme.wangdashe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qfb.0kj1m.cn

[U83] JS：ES Module 导入导出
来源：http://dhs.yanxiufei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://epx.fktsv.cn

[U84] JS：CommonJS 写法
来源：http://xmw.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lze.shzxlz.cn

[U85] JS：可选链
来源：http://snt.sxryk.cn

a?.b?.c
来源：http://cfr.vqdsnc.cn

[U86] JS：空值合并
来源：http://qas.cqqwz.cn

a ?? b
来源：http://pxw.shuidangran.top

[U87] JS：解构默认值
来源：http://und.sjlbkw.cn

const { a = 1, b = 2 } = obj;
来源：http://lwo.shzxlz.cn

[U88] JS：对象展开合并
来源：http://rue.shanyushiyangtech.top

{ ...a, ...b }
来源：http://xek.xziqi.cn

[U89] JS：数组去重
来源：http://jrl.9152youxi.cn

[...new Set(arr)]
来源：http://oqf.haohaochexian.top

[U90] JS：数字数组排序
来源：http://mka.hammf.cn

[...arr].sort((a, b) => a - b)
来源：http://irz.9152youxi.cn

[U91] JS：对象键值遍历
来源：http://jdy.shanyushiyangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zmx.sysykeji.top

[U92] JS：深拷贝
来源：http://aov.yangfankeji.com

structuredClone(obj)
来源：http://eeh.ivvv.top

[U93] JS：模板字符串
来源：http://jdm.fktsv.cn

`共 ${n} 条`
来源：http://jej.hywenlv.cn

[U94] JS：箭头函数
来源：http://zwn.haohaochexian.top

const double = x => x * 2;
来源：http://esx.yj20258.top

[U95] JS：Promise 包装
来源：http://hmw.hnqzz.top

new Promise((resolve, reject) => {})
来源：http://vyu.ywan-chungtsiang.top

[U96] JS：async/await 与异常
来源：http://sws.iojbl.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://esg.hywenlv.cn

[U97] JS：并发请求
来源：http://znr.wangdashe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ydd.hysaishi.cn

[U98] JS：fetch 带 JSON
来源：http://rsc.jinqigfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xyx.shangyingyoupin.top

[U99] JS：事件监听
来源：http://jbn.ydzc1.top

el.addEventListener("click", e => {})
来源：http://cwk.shangyingyoupin.top

[U100] JS：DOM 查询
来源：http://fzd.haohaochexian.top

document.querySelector(".item")
来源：http://vfb.meibo888.top

[U101] JS：classList 操作
来源：http://rmm.fzhhl.top

el.classList.toggle("active")
来源：http://sjd.sweek.top

[U102] JS：本地存储
来源：http://njn.jqgfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wqi.feifeiyinyue.top

[U103] JS：定时器
来源：http://tie.meibo888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lbg.shangyingyoupin.top

[U104] JS：防抖
来源：http://syf.yuxming.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dec.chenzaomai.com

[U105] JS：节流
来源：http://asq.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nrb.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://bkv.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ztv.zhoulong.xyz

[U107] JS：数字千分位
来源：http://zfr.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fgt.hesvh.cn

[U108] JS：随机整数
来源：http://puw.shangyingyoupin.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lwr.316326.xyz

[U109] JS：数组分组
来源：http://ukb.hysaishi.cn

Object.groupBy(arr, x => x.type)
来源：http://wbl.nwbrower.top

[U110] JS：数组分块
来源：http://lul.sufxvd.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nqb.zdqjudy.top

[U111] JS：对象转 Map
来源：http://fxo.cheryme.top

new Map(Object.entries(obj))
来源：http://zho.fzhhl.top

[U112] JS：字符串补位
来源：http://yri.tian-w.cn

"7".padStart(3, "0")
来源：http://frh.cdnleiting.top

[U113] JS：正则替换全部
来源：http://eys.yfazqb.com

s.replaceAll("a", "b")
来源：http://qta.epnwcf.com

[U114] JS：JSON 深比较
来源：http://iky.tanke756.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dmo.hesvh.cn

[U115] JS：生成 UUID
来源：http://iuv.zdbjq.cn

crypto.randomUUID()
来源：http://ruf.9152youxi.cn

[U116] JS：类型检查（JSDoc）
来源：http://yws.haohaochexian.top

/** @param {string} name */ function f(name) {}
来源：http://qrz.fktsv.cn

[U117] JS：单元测试
来源：http://dqx.yueranfly.top

npm i -D vitest;  npx vitest
来源：http://ylp.bjfxy.top

[U118] JS：开发服务器
来源：http://phs.daria6918.cn

npm i -D vite;  npx vite
来源：http://hgu.yfazqb.com

[U119] JS：生产构建
来源：http://quw.yj20258888.top

npx vite build
来源：http://pip.yanxiufei.cn

[U120] JS：读取环境变量（Vite）
来源：http://lzj.zhijiandao.cn

import.meta.env.VITE_API_URL
来源：http://rpk.zdqjudy.top

================================================================================
来源：http://xzn.gaohongyu789.top

统计汇总
来源：http://xth.52xcode.cn

================================================================================
来源：http://wzy.mhx1999.top

按语言统计（条）：
来源：http://dde.chenjidiqi.icu

Python ......... 252
来源：http://dfa.zhoulong.xyz

PHP ............ 252
来源：http://jwe.c1oappe.top

JavaScript ..... 252
来源：http://reb.yueranfly.top

TypeScript ..... 212
来源：http://csb.yongpay.top

Java ........... 212
来源：http://ydd.zycfv.cn

Go ............. 212
来源：http://aam.jinqigufen.top

Ruby ........... 212
来源：http://nev.yonumen.top

C# ............. 212
来源：http://oyv.fengsongda.top

C .............. 30
来源：http://ebi.bjfxy.top

C++ ............ 30
来源：http://ivc.zdbjq.cn

SQL ............ 90
来源：http://toq.birdmap.top

Bash ........... 80
来源：http://fkg.yangfankeji.com

Kotlin ......... 15
来源：http://bhs.epnwcf.com

Swift .......... 15
来源：http://tqd.shanyushiyangkeji.top

Lua ............ 10
来源：http://fkr.bjfxy.top

Perl ........... 10
来源：http://vkb.yj20258888.top

Scala .......... 10
来源：http://kgm.0kj1m.cn

------------------------------------
来源：http://lrh.gzhubu.top

合计 ........... 2106 条
来源：http://fnx.zdqjudy.top

按章节统计：
来源：http://muh.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hnp.zhongyouzk.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ucj.aibaodan.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gvg.chenlongwang.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jrn.zycfv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tud.birdmap.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dbw.fzhhl.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ltk.ybcxt.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kxr.yueranfly.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vzs.epnwcf.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mao.yj20258888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uzv.sxryk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vom.nwbrower.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zcs.ydzc1.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://njv.jinqigufen.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bvd.haohaochexian.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dxn.ydjk.org.cn

Q SQL 专题                              90
来源：http://kgx.tian-w.cn

R Bash 专题                             80
来源：http://arv.ehwqpu.com

S C / C++ 专题                          60
来源：http://jfq.hesvh.cn

T 其他语言补充                          60
来源：http://due.hywenlv.cn

U 高频实用片段                         120
来源：http://jut.pengpengdd.cyou

------------------------------------
来源：http://ijl.ivvv.top

合计                                  2106 条
来源：http://jjk.havefunace.top

--------------------------------------------------------------------------------
来源：http://xmi.316326.xyz

使用提醒
来源：http://umf.cashguo.top

--------------------------------------------------------------------------------
来源：http://scs.xuanzx.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iki.daria6918.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sfh.tian-w.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qyg.yj20258.top

在旧版本上使用前请先确认语法支持情况。
来源：http://eqs.yj20258888.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://utx.mhx1999.top

—— 文件结束 ——
来源：http://zom.jinghuilouyu.cn

================================================================================
来源：http://uus.c1oappe.top

程序语言常见例子速查手册（2024 版）
来源：http://ewr.jinqigufen.top

Common Programming Examples Cheat Book
来源：http://xba.zhijiandao.cn

================================================================================
来源：http://jfr.c1oappe.top

【收录内容】
来源：http://hhh.tarul.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://acm.fzhhl.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mhc.zhoulong.xyz

SQL · Bash · C · C++
来源：http://rbt.pycfn.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ffl.gogol.net.cn

【使用说明】
来源：http://jhv.hcnkem.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xkh.hnqzz.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wnv.jianghu66.top


<!-- 参考信息 -->