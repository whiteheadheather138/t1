代发 wailian999

[U03] Py：加载 .env 配置
来源：http://fjg.chenzaomai.com

from dotenv import load_dotenv; load_dotenv()
来源：http://vji.0kj1m.cn

[U04] Py：变量调试打印
来源：http://tba.nanxinkj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vzn.iojbl.cn

[U05] Py：列表去重且保序
来源：http://pyi.sxryk.cn

list(dict.fromkeys(arr))
来源：http://evm.nanxuanxn.top

[U06] Py：合并两个字典
来源：http://cpw.andypj.xyz

{**a, **b}
来源：http://zsz.sysykeji.top

[U07] Py：反转字典键值
来源：http://jwd.xuanzx.com

{v: k for k, v in d.items()}
来源：http://uye.yfazqb.com

[U08] Py：展平二维列表
来源：http://aku.gaohongyu789.top

[y for x in nested for y in x]
来源：http://lmg.birdmap.top

[U09] Py：字典取最大值的键
来源：http://jba.nwbrower.top

max(d, key=d.get)
来源：http://cwj.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://itk.c1oappe.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zgq.aibaodan.cn

[U11] Py：生成器表达式
来源：http://poj.sxryk.cn

(x * 2 for x in arr)
来源：http://orn.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ybk.yangfankeji.com

Counter(arr).most_common(3)
来源：http://tqf.shangyingyoupin.top

[U13] Py：固定长度队列
来源：http://lxl.aibaodan.cn

deque(maxlen=10)
来源：http://xyf.chenjidiqi.icu

[U14] Py：分组收集到列表
来源：http://nid.cashguo.top

defaultdict(list)
来源：http://uap.ydzc1.top

[U15] Py：高精度计时
来源：http://lgu.andypj.xyz

t = time.perf_counter()
来源：http://ybe.zhengqikj.top

[U16] Py：命令行参数解析
来源：http://zik.tarul.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://puu.cheryme.top

[U17] Py：初始化日志
来源：http://mlm.vqdsnc.cn

logging.basicConfig(level=logging.INFO)
来源：http://lvh.zhengqikj.top

[U18] Py：预编译正则
来源：http://tuh.zhoulong.xyz

pat = re.compile(r"\d+")
来源：http://dvg.52xcode.cn

[U19] Py：正则替换带回调
来源：http://lkx.smart0.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bxb.xingfuxueyuan.xyz

[U20] Py：缓存函数结果
来源：http://zbk.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://gyk.nanxuanxn.top

[U21] Py：自定义上下文管理器
来源：http://bib.jianghu66.top

@contextlib.contextmanager
来源：http://lwo.tianlin.xyz

[U22] Py：矩阵转置
来源：http://cyb.guannengcc.top

list(zip(*m))
来源：http://ire.yj20258888.top

[U23] Py：分块读取大文件
来源：http://xex.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ooo.hongshengwenyu.top

[U24] Py：路径操作
来源：http://oji.hesvh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://epw.sufxvd.cn

[U25] Py：CSV 按字典读
来源：http://oai.sysykeji.top

csv.DictReader(f)
来源：http://uix.zhoulong.xyz

[U26] Py：并发下载
来源：http://fbe.xziqi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jfr.fehbvm.com

[U27] Py：异步 HTTP
来源：http://ytz.yongpay.top

aiohttp.ClientSession() 配合 async with
来源：http://wrv.jyoumei.cn

[U28] Py：类型别名
来源：http://xjf.hnqzz.top

UserId = int
来源：http://jah.dianchejie.cn

[U29] Py：属性校验
来源：http://vgg.birdmap.top

@property 与 @x.setter 配合
来源：http://arm.fengsongda.top

[U30] Py：数据类
来源：http://klu.nwbrower.top

@dataclass(slots=True)
来源：http://big.nanxinkj.top

[U31] Py：单测
来源：http://ifr.ivvv.top

python -m pytest -q
来源：http://fpr.ybcxt.top

[U32] Py：代码格式化
来源：http://qnz.fengsongda.top

ruff format . && ruff check --fix .
来源：http://ulo.hesvh.cn

[U33] Py：打包发布
来源：http://nps.tian-w.cn

python -m build  （依赖 pyproject.toml）
来源：http://ufa.zdbjq.cn

[U34] Py：判断编码
来源：http://mfx.jinqigufen.top

chardet.detect(raw)
来源：http://iwi.ydzc1.top

[U35] Py：发送邮件
来源：http://wac.daria6918.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lad.aizwys.cn

[U36] Py：定时任务
来源：http://vpe.quarkkingdee.top

schedule.every(10).minutes.do(job)
来源：http://sth.c1oappe.top

[U37] Py：读写 Excel
来源：http://anj.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://iet.xuetiantiany.cn

[U38] Py：获取脚本所在目录
来源：http://mcn.zhixingplan.top

Path(__file__).resolve().parent
来源：http://evo.vehdjk.com

[U39] Py：判断是否在交互环境
来源：http://mno.zhijiandao.cn

sys.stdout.isatty()
来源：http://mqa.bbcook.cn

[U40] Py：打印到标准错误
来源：http://oqu.zhijiandao.cn

print("err", file=sys.stderr)
来源：http://nnx.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://hop.gaohongyu789.top

composer init;  composer require guzzlehttp/guzzle
来源：http://oso.nanxinkj.top

[U42] PHP：PSR-4 自动加载
来源：http://jse.quarkkingdee.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rcs.hcnkem.com

[U43] PHP：声明命名空间
来源：http://wwy.fktsv.cn

namespace App\Http;
来源：http://yom.sysykeji.top

[U44] PHP：开启严格类型
来源：http://iqu.nanxuanxn.top

declare(strict_types=1);
来源：http://sqg.cqqwz.cn

[U45] PHP：类型声明与返回类型
来源：http://zbi.yongpay.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lrt.yuanzhike.top

[U46] PHP：可空类型
来源：http://diw.hysaishi.cn

?string $name = null
来源：http://deo.nanxinkj.top

[U47] PHP：联合类型
来源：http://wqk.haohaochexian.top

int|string $id
来源：http://nmi.daxiang520.top

[U48] PHP：纯枚举
来源：http://yvn.hesvh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ani.vehdjk.com

[U49] PHP：只读属性
来源：http://sww.dianchejie.cn

public readonly string $name
来源：http://ylr.sjlbkw.cn

[U50] PHP：构造器属性提升
来源：http://gwt.hesvh.cn

public function __construct(private int $id) {}
来源：http://htl.ehwqpu.com

[U51] PHP：数组解构
来源：http://vte.hongshengwenyu.top

[$a, $b] = $arr;
来源：http://rfg.yj20258.top

[U52] PHP：箭头函数
来源：http://dba.yj20258.top

$double = fn($x) => $x * 2;
来源：http://hxy.hnqzz.top

[U53] PHP：空合并运算符
来源：http://frp.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://lgn.kuanghao11.cn

[U54] PHP：空安全调用
来源：http://ajg.hnqzz.top

$obj?->method()
来源：http://nxu.gzhubu.top

[U55] PHP：match 表达式
来源：http://des.chenlongwang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ljf.shzxlz.cn

[U56] PHP：命名参数
来源：http://fac.shuidangran.top

f(a: 1, b: 2)
来源：http://tgb.quarkkingdee.top

[U57] PHP：字符串插值
来源：http://tif.chenzaomai.com

"值: {$a}"
来源：http://sdx.zhiwuduotai.top

[U58] PHP：数组三件套
来源：http://mgl.yangfankeji.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://umm.gotoacloud.top

[U59] PHP：自定义排序
来源：http://hqe.kuanghao11.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://whj.quarkkingdee.top

[U60] PHP：JSON 编解码
来源：http://nra.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fks.redwolf501.top

[U61] PHP：正则
来源：http://erb.xuanzx.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sjg.c1oappe.top

[U62] PHP：日期对象
来源：http://jyo.jinghuilouyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://keh.jqgfzy.top

[U63] PHP：文件读写
来源：http://zco.gotoacloud.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qne.fanxiaobao.xyz

[U64] PHP：目录遍历
来源：http://mkb.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://vtt.jinqigfzy.top

[U65] PHP：会话
来源：http://iog.chenlongwang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ulq.ydjk.org.cn

[U66] PHP：设置 Cookie
来源：http://lne.ybcxt.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nsu.tian-w.cn

[U67] PHP：处理文件上传
来源：http://kej.xziqi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xdj.sweek.top

[U68] PHP：PDO 连接
来源：http://xvc.yongpay.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://njd.vqdsnc.cn

[U69] PHP：PDO 预处理
来源：http://fto.fzhhl.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lth.tanke756.top

[U70] PHP：PDO 事务
来源：http://nxm.xuetiantiany.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://afy.316326.xyz

[U71] PHP：抛出异常
来源：http://clh.nanxuanxn.top

throw new RuntimeException("失败", 500);
来源：http://uut.9152youxi.cn

[U72] PHP：写错误日志
来源：http://wwp.chenlongwang.top

error_log("失败: " . $e->getMessage());
来源：http://jjj.zdbjq.cn

[U73] PHP：读取 ini 配置
来源：http://uzo.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://zwp.9152youxi.cn

[U74] PHP：读取环境变量
来源：http://mni.yj202588.top

getenv("APP_ENV") ?: "production"
来源：http://rps.fanxiaobao.xyz

[U75] PHP：依赖注入
来源：http://qrz.daxiang520.top

composer require psr/container
来源：http://cfh.yuxming.cn

[U76] PHP：简单路由
来源：http://fcl.xuetiantiany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://odv.guannengcc.top

[U77] PHP：模板渲染
来源：http://jmi.nanxinkj.top

composer require twig/twig
来源：http://kyo.haohaochexian.top

[U78] PHP：单元测试
来源：http://pjx.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://ylp.gzhubu.top

[U79] PHP：静态分析
来源：http://mjb.fktsv.cn

composer require --dev phpstan/phpstan
来源：http://app.jlsjyb.cn

[U80] PHP：代码规范修复
来源：http://fob.fzhhl.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://oax.ywan-chungtsiang.top

[U81] JS：初始化项目
来源：http://iup.vehdjk.com

npm init -y;  npm i express
来源：http://hhr.tanke756.top

[U82] JS：package.json 脚本
来源：http://imf.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kzv.hysaishi.cn

[U83] JS：ES Module 导入导出
来源：http://tlk.birdmap.top

export const a = 1;  import { a } from "./m.js";
来源：http://jov.jinghuilouyu.cn

[U84] JS：CommonJS 写法
来源：http://scl.tarul.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jni.andypj.xyz

[U85] JS：可选链
来源：http://hsk.jianghu66.top

a?.b?.c
来源：http://gks.guowangkeji.top

[U86] JS：空值合并
来源：http://zdp.smart0.xyz

a ?? b
来源：http://ual.jqgufenzy.top

[U87] JS：解构默认值
来源：http://oie.jyoumei.cn

const { a = 1, b = 2 } = obj;
来源：http://bcx.vehdjk.com

[U88] JS：对象展开合并
来源：http://epj.jinyuanbaomall.cn

{ ...a, ...b }
来源：http://jsb.shuidangran.top

[U89] JS：数组去重
来源：http://mfg.xylfe.cn

[...new Set(arr)]
来源：http://ihn.bjfxy.top

[U90] JS：数字数组排序
来源：http://gmd.pengpengdd.cyou

[...arr].sort((a, b) => a - b)
来源：http://heh.sjlbkw.cn

[U91] JS：对象键值遍历
来源：http://zqu.shanyushiyangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mwu.hcnkem.com

[U92] JS：深拷贝
来源：http://dkl.jinyuanbaomall.cn

structuredClone(obj)
来源：http://ftu.zhongyouzk.top

[U93] JS：模板字符串
来源：http://muu.ivvv.top

`共 ${n} 条`
来源：http://fgh.smart0.xyz

[U94] JS：箭头函数
来源：http://bcy.yanxiufei.cn

const double = x => x * 2;
来源：http://iux.zdbjq.cn

[U95] JS：Promise 包装
来源：http://rdc.shzxlz.cn

new Promise((resolve, reject) => {})
来源：http://oxp.sufxvd.cn

[U96] JS：async/await 与异常
来源：http://qaw.yueranfly.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tpm.yj20258.top

[U97] JS：并发请求
来源：http://ent.316326.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://itn.52xcode.cn

[U98] JS：fetch 带 JSON
来源：http://fgz.zhixingplan.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://shr.xziqi.cn

[U99] JS：事件监听
来源：http://udi.birdmap.top

el.addEventListener("click", e => {})
来源：http://fye.redwolf501.top

[U100] JS：DOM 查询
来源：http://nll.daria6918.cn

document.querySelector(".item")
来源：http://oaw.cucudq.cn

[U101] JS：classList 操作
来源：http://glm.guannengcc.top

el.classList.toggle("active")
来源：http://lws.fzhhl.top

[U102] JS：本地存储
来源：http://xql.fengsongda.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tfp.tanke756.top

[U103] JS：定时器
来源：http://avb.hnqzz.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://urs.zhiwuduotai.top

[U104] JS：防抖
来源：http://dpu.cdnleiting.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://alt.dashuyun.cn

[U105] JS：节流
来源：http://bbf.xuetiantiany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bmn.daxiang520.top

[U106] JS：日期格式化
来源：http://ujy.c1oappe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bfh.jlsjyb.cn

[U107] JS：数字千分位
来源：http://oga.xinyue.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bgn.xziqi.cn

[U108] JS：随机整数
来源：http://zgu.sweek.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bzz.hongshengwenyu.top

[U109] JS：数组分组
来源：http://srw.zdqjudy.top

Object.groupBy(arr, x => x.type)
来源：http://ocy.cucudq.cn

[U110] JS：数组分块
来源：http://gst.iojbl.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pct.jqgufenzy.top

[U111] JS：对象转 Map
来源：http://gyd.dianchejie.cn

new Map(Object.entries(obj))
来源：http://zzs.yuanzhike.top

[U112] JS：字符串补位
来源：http://grz.zycfv.cn

"7".padStart(3, "0")
来源：http://oxb.meibo888.top

[U113] JS：正则替换全部
来源：http://fsl.52xcode.cn

s.replaceAll("a", "b")
来源：http://edc.yongpay.top

[U114] JS：JSON 深比较
来源：http://ifr.vqdsnc.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wla.tianlin.xyz

[U115] JS：生成 UUID
来源：http://mqp.yvedp.cn

crypto.randomUUID()
来源：http://gii.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://egd.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://yyr.jiagoushi.top

[U117] JS：单元测试
来源：http://ebh.yanxiufei.cn

npm i -D vitest;  npx vitest
来源：http://mev.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://qsd.yfazqb.com

npm i -D vite;  npx vite
来源：http://gbd.yangfankeji.com

[U119] JS：生产构建
来源：http://amt.cucudq.cn

npx vite build
来源：http://kxa.epnwcf.com

[U120] JS：读取环境变量（Vite）
来源：http://dpu.yj20258.top

import.meta.env.VITE_API_URL
来源：http://weq.cucudq.cn

================================================================================
来源：http://esv.cqqwz.cn

统计汇总
来源：http://bjl.yonumen.top

================================================================================
来源：http://pyj.fktsv.cn

按语言统计（条）：
来源：http://vie.zhiwuduotai.top

Python ......... 252
来源：http://aji.xziqi.cn

PHP ............ 252
来源：http://mqx.jinghuilouyu.cn

JavaScript ..... 252
来源：http://usi.gzhubu.top

TypeScript ..... 212
来源：http://kjw.sufxvd.cn

Java ........... 212
来源：http://tvh.xuetiantiany.cn

Go ............. 212
来源：http://qxi.chenjidiqi.icu

Ruby ........... 212
来源：http://bts.snrcjt.cn

C# ............. 212
来源：http://xed.zhengqikj.top

C .............. 30
来源：http://sgm.jyoumei.cn

C++ ............ 30
来源：http://ggj.chenjidiqi.icu

SQL ............ 90
来源：http://ziw.wangshuangyany.cn

Bash ........... 80
来源：http://wes.yueranfly.top

Kotlin ......... 15
来源：http://vzg.ppjwa.cn

Swift .......... 15
来源：http://oje.cheryme.top

Lua ............ 10
来源：http://wmg.fehbvm.com

Perl ........... 10
来源：http://gva.hysaishi.cn

Scala .......... 10
来源：http://rgv.mhx1999.top

------------------------------------
来源：http://emo.zycfv.cn

合计 ........... 2106 条
来源：http://dco.hywenlv.cn

按章节统计：
来源：http://gux.wangdashe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ekb.dianchejie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://frg.ydjk.org.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oay.316326.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wdb.chenzaomai.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://onn.zhoulong.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://grl.ywan-chungtsiang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ezb.yongpay.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://llp.chenzaomai.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jqf.tanke756.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ist.andypj.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qqd.yj20258888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zxp.ywan-chungtsiang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lrs.sxryk.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rzf.andypj.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eph.aibaodan.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gff.vehdjk.com

Q SQL 专题                              90
来源：http://ydo.kuanghao11.cn

R Bash 专题                             80
来源：http://dgw.nanxinkj.top

S C / C++ 专题                          60
来源：http://bfu.tianlin.xyz

T 其他语言补充                          60
来源：http://vgu.jinqigfzy.top

U 高频实用片段                         120
来源：http://xqs.quarkkingdee.top

------------------------------------
来源：http://eka.yanxiufei.cn

合计                                  2106 条
来源：http://kvu.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://lux.hfpthk.cn

使用提醒
来源：http://xpw.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://kmt.snrcjt.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cqy.aibaodan.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hkq.jqgufenzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fey.jinghuilouyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hwm.fanxiaobao.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vhd.gogol.net.cn

—— 文件结束 ——
来源：http://ere.shangyingyoupin.top

================================================================================
来源：http://oew.316326.xyz

程序语言常见例子速查手册（2024 版）
来源：http://poy.aizwys.cn

Common Programming Examples Cheat Book
来源：http://gcl.9152youxi.cn

================================================================================
来源：http://ste.gaohongyu789.top

【收录内容】
来源：http://tbb.9152youxi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zho.shangyingyoupin.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pxg.jiagoushi.top

SQL · Bash · C · C++
来源：http://nqo.epnwcf.com


<!-- 参考信息 -->