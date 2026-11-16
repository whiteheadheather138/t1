代发 wailian999

[U09] Py：字典取最大值的键
来源：http://mec.jyoumei.cn

max(d, key=d.get)
来源：http://sow.fzhhl.top

[U10] Py：按值排序字典
来源：http://tmh.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hhb.hcnkem.com

[U11] Py：生成器表达式
来源：http://xhx.yj20258.top

(x * 2 for x in arr)
来源：http://ziy.52xcode.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rww.yj20258.top

Counter(arr).most_common(3)
来源：http://jkj.yfazqb.com

[U13] Py：固定长度队列
来源：http://tor.daxiang520.top

deque(maxlen=10)
来源：http://lfe.tianlin.xyz

[U14] Py：分组收集到列表
来源：http://asa.cashguo.top

defaultdict(list)
来源：http://vxx.gaohongyu789.top

[U15] Py：高精度计时
来源：http://tid.shzxlz.cn

t = time.perf_counter()
来源：http://xts.guannengcc.top

[U16] Py：命令行参数解析
来源：http://udm.yj20258888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://exx.jiagoushi.top

[U17] Py：初始化日志
来源：http://efs.yj202588.top

logging.basicConfig(level=logging.INFO)
来源：http://xub.xuetiantiany.cn

[U18] Py：预编译正则
来源：http://czm.yueranfly.top

pat = re.compile(r"\d+")
来源：http://ttv.yonumen.top

[U19] Py：正则替换带回调
来源：http://kwm.yongpay.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wbu.jyoumei.cn

[U20] Py：缓存函数结果
来源：http://ukj.redwolf501.top

@functools.lru_cache(maxsize=None)
来源：http://wsp.zycfv.cn

[U21] Py：自定义上下文管理器
来源：http://qxo.sweek.top

@contextlib.contextmanager
来源：http://xxw.pengpengdd.cyou

[U22] Py：矩阵转置
来源：http://tho.aizwys.cn

list(zip(*m))
来源：http://mdl.yvedp.cn

[U23] Py：分块读取大文件
来源：http://spi.zhijiandao.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dsq.fanxiaobao.xyz

[U24] Py：路径操作
来源：http://grj.tian-w.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fos.gotoacloud.top

[U25] Py：CSV 按字典读
来源：http://hzd.yangfankeji.com

csv.DictReader(f)
来源：http://mxk.redwolf501.top

[U26] Py：并发下载
来源：http://pmn.jinyuanbaomall.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jlt.chenlongwang.top

[U27] Py：异步 HTTP
来源：http://boc.wangdashe.top

aiohttp.ClientSession() 配合 async with
来源：http://rxb.jlsjyb.cn

[U28] Py：类型别名
来源：http://ogn.vqdsnc.cn

UserId = int
来源：http://wdg.vehdjk.com

[U29] Py：属性校验
来源：http://ymf.hcnkem.com

@property 与 @x.setter 配合
来源：http://tif.smart0.xyz

[U30] Py：数据类
来源：http://yeg.ybcxt.top

@dataclass(slots=True)
来源：http://ror.cqqwz.cn

[U31] Py：单测
来源：http://gax.iojbl.cn

python -m pytest -q
来源：http://whw.jqgufenzy.top

[U32] Py：代码格式化
来源：http://dpt.jqgfzy.top

ruff format . && ruff check --fix .
来源：http://exy.bjfxy.top

[U33] Py：打包发布
来源：http://qpg.redwolf501.top

python -m build  （依赖 pyproject.toml）
来源：http://zet.tianlin.xyz

[U34] Py：判断编码
来源：http://gck.jqgufenzy.top

chardet.detect(raw)
来源：http://utt.gotoacloud.top

[U35] Py：发送邮件
来源：http://ved.zhengqikj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zkz.zhengqikj.top

[U36] Py：定时任务
来源：http://daj.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://lwu.jinyuanbaomall.cn

[U37] Py：读写 Excel
来源：http://tti.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://njd.xingfuxueyuan.xyz

[U38] Py：获取脚本所在目录
来源：http://mtf.ctjpmb.com

Path(__file__).resolve().parent
来源：http://tnd.snrcjt.cn

[U39] Py：判断是否在交互环境
来源：http://pyt.yangfankeji.com

sys.stdout.isatty()
来源：http://cfu.hongshengwenyu.top

[U40] Py：打印到标准错误
来源：http://phj.redwolf501.top

print("err", file=sys.stderr)
来源：http://wwt.jianghu66.top

[U41] PHP：初始化 Composer 项目
来源：http://xaj.jyoumei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://veb.nanxuanxn.top

[U42] PHP：PSR-4 自动加载
来源：http://ygw.yvedp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aor.shuidangran.top

[U43] PHP：声明命名空间
来源：http://clu.uphjek.com

namespace App\Http;
来源：http://ppk.haohaochexian.top

[U44] PHP：开启严格类型
来源：http://xio.yongpay.top

declare(strict_types=1);
来源：http://knl.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://wcm.jinghuilouyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vud.xylfe.cn

[U46] PHP：可空类型
来源：http://uqi.hnxiangtu.top

?string $name = null
来源：http://jqz.hammf.cn

[U47] PHP：联合类型
来源：http://pjn.jianghu66.top

int|string $id
来源：http://btc.redwolf501.top

[U48] PHP：纯枚举
来源：http://tpo.jianghu66.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rey.redwolf501.top

[U49] PHP：只读属性
来源：http://fce.mhx1999.top

public readonly string $name
来源：http://rmt.jianghu66.top

[U50] PHP：构造器属性提升
来源：http://qww.jlsjyb.cn

public function __construct(private int $id) {}
来源：http://axx.feifeiyinyue.top

[U51] PHP：数组解构
来源：http://uvm.jianghu66.top

[$a, $b] = $arr;
来源：http://wym.9152youxi.cn

[U52] PHP：箭头函数
来源：http://hmg.jinqigufen.top

$double = fn($x) => $x * 2;
来源：http://tlh.snrcjt.cn

[U53] PHP：空合并运算符
来源：http://vzc.chenjidiqi.icu

$v = $a ?? $b ?? "default";
来源：http://mot.dianchejie.cn

[U54] PHP：空安全调用
来源：http://yps.zhoulong.xyz

$obj?->method()
来源：http://wge.aibaodan.cn

[U55] PHP：match 表达式
来源：http://rne.yongpay.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vya.52xcode.cn

[U56] PHP：命名参数
来源：http://irh.xziqi.cn

f(a: 1, b: 2)
来源：http://klc.ivvv.top

[U57] PHP：字符串插值
来源：http://ysj.yongpay.top

"值: {$a}"
来源：http://hhm.jinghuilouyu.cn

[U58] PHP：数组三件套
来源：http://gft.guowangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bay.tianlin.xyz

[U59] PHP：自定义排序
来源：http://jfi.ybcxt.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wgl.ivvv.top

[U60] PHP：JSON 编解码
来源：http://sgt.aibaodan.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mth.yanxiufei.cn

[U61] PHP：正则
来源：http://pco.daxiang520.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wzs.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://sjw.zdbjq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jcq.meibo888.top

[U63] PHP：文件读写
来源：http://rzu.zhixingplan.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kga.jqgfzy.top

[U64] PHP：目录遍历
来源：http://poy.shzxlz.cn

glob("dir/*.php");  scandir("dir");
来源：http://niw.hysaishi.cn

[U65] PHP：会话
来源：http://zbd.ydzc1.top

session_start();  $_SESSION["uid"] = 1;
来源：http://yse.chenlongwang.top

[U66] PHP：设置 Cookie
来源：http://wsp.zhiwuduotai.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://egs.bbcook.cn

[U67] PHP：处理文件上传
来源：http://xiv.yfazqb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vfw.cucudq.cn

[U68] PHP：PDO 连接
来源：http://cls.fzhhl.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uni.fktsv.cn

[U69] PHP：PDO 预处理
来源：http://amb.snrcjt.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jxp.epnwcf.com

[U70] PHP：PDO 事务
来源：http://oow.cashguo.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zbs.yj20258888.top

[U71] PHP：抛出异常
来源：http://hls.zhijiandao.cn

throw new RuntimeException("失败", 500);
来源：http://ipi.yj202588.top

[U72] PHP：写错误日志
来源：http://jvu.52xcode.cn

error_log("失败: " . $e->getMessage());
来源：http://nwt.jinghuilouyu.cn

[U73] PHP：读取 ini 配置
来源：http://qgk.ydjk.org.cn

parse_ini_file("config.ini", true)
来源：http://tlo.xuetiantiany.cn

[U74] PHP：读取环境变量
来源：http://ddf.xinyue.icu

getenv("APP_ENV") ?: "production"
来源：http://bsy.xingfuxueyuan.xyz

[U75] PHP：依赖注入
来源：http://vrd.daxiang520.top

composer require psr/container
来源：http://zoq.gaohongyu789.top

[U76] PHP：简单路由
来源：http://lga.feifeiyinyue.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://som.daxiang520.top

[U77] PHP：模板渲染
来源：http://uyq.pycfn.com

composer require twig/twig
来源：http://hfh.cucudq.cn

[U78] PHP：单元测试
来源：http://qik.smart0.xyz

composer require --dev phpunit/phpunit
来源：http://lwr.cqqwz.cn

[U79] PHP：静态分析
来源：http://qmt.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://kmc.vehdjk.com

[U80] PHP：代码规范修复
来源：http://lwq.gzhubu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ymc.mhx1999.top

[U81] JS：初始化项目
来源：http://uxi.jqgfzy.top

npm init -y;  npm i express
来源：http://hgo.yongpay.top

[U82] JS：package.json 脚本
来源：http://zqf.havefunace.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pqu.cashguo.top

[U83] JS：ES Module 导入导出
来源：http://esf.hongshengwenyu.top

export const a = 1;  import { a } from "./m.js";
来源：http://ohe.svipenyu.cn

[U84] JS：CommonJS 写法
来源：http://amg.xinyue.icu

module.exports = { a };  const { a } = require("./m");
来源：http://eud.zhongyouzk.top

[U85] JS：可选链
来源：http://sys.ehwqpu.com

a?.b?.c
来源：http://nqt.0kj1m.cn

[U86] JS：空值合并
来源：http://ghu.ybcxt.top

a ?? b
来源：http://pge.xuanzx.com

[U87] JS：解构默认值
来源：http://kzk.jqgufenzy.top

const { a = 1, b = 2 } = obj;
来源：http://dpv.wangdashe.top

[U88] JS：对象展开合并
来源：http://npm.guowangkeji.top

{ ...a, ...b }
来源：http://agw.yangfankeji.com

[U89] JS：数组去重
来源：http://cdg.shzxlz.cn

[...new Set(arr)]
来源：http://yls.havefunace.top

[U90] JS：数字数组排序
来源：http://fvv.dianchejie.cn

[...arr].sort((a, b) => a - b)
来源：http://mth.yj20258888.top

[U91] JS：对象键值遍历
来源：http://vfp.wangshuangyany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://env.hnqzz.top

[U92] JS：深拷贝
来源：http://ija.hongshengwenyu.top

structuredClone(obj)
来源：http://ddm.wangshuangyany.cn

[U93] JS：模板字符串
来源：http://dyg.bbcook.cn

`共 ${n} 条`
来源：http://wbz.tianlin.xyz

[U94] JS：箭头函数
来源：http://khi.iojbl.cn

const double = x => x * 2;
来源：http://scs.aizwys.cn

[U95] JS：Promise 包装
来源：http://bjf.jinghuilouyu.cn

new Promise((resolve, reject) => {})
来源：http://gkw.fzhhl.top

[U96] JS：async/await 与异常
来源：http://lql.shanyushiyangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://thq.cdnleiting.top

[U97] JS：并发请求
来源：http://ykw.aibaodan.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kks.nanxinkj.top

[U98] JS：fetch 带 JSON
来源：http://mpq.jianghu66.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ege.kuanghao11.cn

[U99] JS：事件监听
来源：http://sjk.meibo888.top

el.addEventListener("click", e => {})
来源：http://osq.chenlongwang.top

[U100] JS：DOM 查询
来源：http://hqn.0kj1m.cn

document.querySelector(".item")
来源：http://kmk.xuanzx.com

[U101] JS：classList 操作
来源：http://koh.jyoumei.cn

el.classList.toggle("active")
来源：http://xin.guannengcc.top

[U102] JS：本地存储
来源：http://ykb.ydjk.org.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gob.birdmap.top

[U103] JS：定时器
来源：http://yyh.wangshuangyany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xiw.birdmap.top

[U104] JS：防抖
来源：http://inl.jqgfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tyf.tanke756.top

[U105] JS：节流
来源：http://vrc.havefunace.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://spf.tian-w.cn

[U106] JS：日期格式化
来源：http://jzq.jqgfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kru.sufxvd.cn

[U107] JS：数字千分位
来源：http://bzh.yvedp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://erz.epnwcf.com

[U108] JS：随机整数
来源：http://mjb.nanxinkj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cmj.gzhubu.top

[U109] JS：数组分组
来源：http://tqc.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://blz.tianlin.xyz

[U110] JS：数组分块
来源：http://ici.sjlbkw.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gve.havefunace.top

[U111] JS：对象转 Map
来源：http://oec.dashuyun.cn

new Map(Object.entries(obj))
来源：http://weg.cucudq.cn

[U112] JS：字符串补位
来源：http://sew.gzhubu.top

"7".padStart(3, "0")
来源：http://ptz.xingfuxueyuan.xyz

[U113] JS：正则替换全部
来源：http://bqp.zhoulong.xyz

s.replaceAll("a", "b")
来源：http://kjx.uphjek.com

[U114] JS：JSON 深比较
来源：http://oal.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fcn.dianchejie.cn

[U115] JS：生成 UUID
来源：http://gnm.bbcook.cn

crypto.randomUUID()
来源：http://zvi.xuanzx.com

[U116] JS：类型检查（JSDoc）
来源：http://uzs.hnqzz.top

/** @param {string} name */ function f(name) {}
来源：http://wxb.hnxiangtu.top

[U117] JS：单元测试
来源：http://yxv.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://plj.yuxming.cn

[U118] JS：开发服务器
来源：http://ovp.shuidangran.top

npm i -D vite;  npx vite
来源：http://gdd.snrcjt.cn

[U119] JS：生产构建
来源：http://apb.yj202588.top

npx vite build
来源：http://jrz.cqqwz.cn

[U120] JS：读取环境变量（Vite）
来源：http://kry.wangdashe.top

import.meta.env.VITE_API_URL
来源：http://thf.yj20258.top

================================================================================
来源：http://gbd.yonumen.top

统计汇总
来源：http://wmx.ppjwa.cn

================================================================================
来源：http://rpd.52xcode.cn

按语言统计（条）：
来源：http://kfi.shzxlz.cn

Python ......... 252
来源：http://kss.chenlongwang.top

PHP ............ 252
来源：http://uja.nanxuanxn.top

JavaScript ..... 252
来源：http://mln.jianghu66.top

TypeScript ..... 212
来源：http://wij.epnwcf.com

Java ........... 212
来源：http://kyr.shanyushiyangtech.top

Go ............. 212
来源：http://kvh.hesvh.cn

Ruby ........... 212
来源：http://wli.9152youxi.cn

C# ............. 212
来源：http://hfp.yj20258.top

C .............. 30
来源：http://msh.aizwys.cn

C++ ............ 30
来源：http://ncs.hfpthk.cn

SQL ............ 90
来源：http://bbp.yj20258.top

Bash ........... 80
来源：http://hek.smart0.xyz

Kotlin ......... 15
来源：http://rqh.fktsv.cn

Swift .......... 15
来源：http://nql.yuanzhike.top

Lua ............ 10
来源：http://sve.yangfankeji.com

Perl ........... 10
来源：http://sjm.xuanzx.com

Scala .......... 10
来源：http://sse.fengsongda.top

------------------------------------
来源：http://qtc.smart0.xyz

合计 ........... 2106 条
来源：http://jxf.iojbl.cn

按章节统计：
来源：http://ioo.yfazqb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rre.sjlbkw.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rys.hysaishi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oce.yueranfly.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rpk.9152youxi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wpf.jlsjyb.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jbm.wangdashe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uzw.jyoumei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gvg.feifeiyinyue.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jhl.svipenyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ido.nanxuanxn.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qsr.daria6918.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bme.gzhubu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gae.ehwqpu.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ltd.yuanzhike.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vla.hesvh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://phq.ydjk.org.cn

Q SQL 专题                              90
来源：http://tmj.aibaodan.cn

R Bash 专题                             80
来源：http://fxc.9152youxi.cn

S C / C++ 专题                          60
来源：http://azm.yangfankeji.com

T 其他语言补充                          60
来源：http://axc.zycfv.cn

U 高频实用片段                         120
来源：http://ixe.pycfn.com

------------------------------------
来源：http://ahh.chenzaomai.com

合计                                  2106 条
来源：http://ozf.wangdashe.top

--------------------------------------------------------------------------------
来源：http://jax.dianchejie.cn

使用提醒
来源：http://qdb.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://oto.yfazqb.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qji.cdnleiting.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://csr.nanxinkj.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cmm.zhixingplan.top

在旧版本上使用前请先确认语法支持情况。
来源：http://afi.yonumen.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://njx.jqgfzy.top

—— 文件结束 ——
来源：http://yge.fengsongda.top

================================================================================
来源：http://nyx.ybcxt.top

程序语言常见例子速查手册（2024 版）
来源：http://xew.fzhhl.top

Common Programming Examples Cheat Book
来源：http://cvo.gotoacloud.top

================================================================================
来源：http://bqu.fehbvm.com

【收录内容】
来源：http://fvy.shanyushiyangtech.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://iaq.sweek.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rso.c1oappe.top

SQL · Bash · C · C++
来源：http://nfc.xziqi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ojw.ppjwa.cn

【使用说明】
来源：http://vjc.sjlbkw.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rju.kuanghao11.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://smw.shangyingyoupin.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bvc.sweek.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kbw.xuetiantiany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vzm.dianchejie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://aqi.316326.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dmp.cdnleiting.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hgr.nanxuanxn.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://aed.gzhubu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qtf.meibo888.top


<!-- 参考信息 -->