代发 wailian999

[U07] Py：反转字典键值
来源：http://tyc.hongshengwenyu.top

{v: k for k, v in d.items()}
来源：http://bpl.c1oappe.top

[U08] Py：展平二维列表
来源：http://yja.zhengqikj.top

[y for x in nested for y in x]
来源：http://tlj.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://lrz.chenzaomai.com

max(d, key=d.get)
来源：http://xye.feifeiyinyue.top

[U10] Py：按值排序字典
来源：http://tgl.yj20258.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yuj.zhengqikj.top

[U11] Py：生成器表达式
来源：http://oub.iojbl.cn

(x * 2 for x in arr)
来源：http://bqy.jqgufenzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://wfx.svipenyu.cn

Counter(arr).most_common(3)
来源：http://gbk.ydzc1.top

[U13] Py：固定长度队列
来源：http://smu.yj20258.top

deque(maxlen=10)
来源：http://uia.havefunace.top

[U14] Py：分组收集到列表
来源：http://zdz.iojbl.cn

defaultdict(list)
来源：http://uyd.zhixingplan.top

[U15] Py：高精度计时
来源：http://gdz.yuxming.cn

t = time.perf_counter()
来源：http://fci.cdnleiting.top

[U16] Py：命令行参数解析
来源：http://utz.hammf.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mqp.fzhhl.top

[U17] Py：初始化日志
来源：http://acr.snrcjt.cn

logging.basicConfig(level=logging.INFO)
来源：http://rto.hywenlv.cn

[U18] Py：预编译正则
来源：http://hmi.nanxuanxn.top

pat = re.compile(r"\d+")
来源：http://cyi.tian-w.cn

[U19] Py：正则替换带回调
来源：http://nzt.epnwcf.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zuh.ydzc1.top

[U20] Py：缓存函数结果
来源：http://frc.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://yhs.zycfv.cn

[U21] Py：自定义上下文管理器
来源：http://ooi.aizwys.cn

@contextlib.contextmanager
来源：http://euk.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://utw.zhoulong.xyz

list(zip(*m))
来源：http://vzz.shanyushiyangtech.top

[U23] Py：分块读取大文件
来源：http://uqk.birdmap.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://unn.cucudq.cn

[U24] Py：路径操作
来源：http://dbd.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gcw.yuxming.cn

[U25] Py：CSV 按字典读
来源：http://wlb.tian-w.cn

csv.DictReader(f)
来源：http://zym.zycfv.cn

[U26] Py：并发下载
来源：http://bji.jqgfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qdb.hcnkem.com

[U27] Py：异步 HTTP
来源：http://too.yangfankeji.com

aiohttp.ClientSession() 配合 async with
来源：http://gjw.sysykeji.top

[U28] Py：类型别名
来源：http://hnq.jiagoushi.top

UserId = int
来源：http://zgs.hywenlv.cn

[U29] Py：属性校验
来源：http://lfv.yonumen.top

@property 与 @x.setter 配合
来源：http://vrm.hfpthk.cn

[U30] Py：数据类
来源：http://ymj.guowangkeji.top

@dataclass(slots=True)
来源：http://knb.daxiang520.top

[U31] Py：单测
来源：http://jun.iojbl.cn

python -m pytest -q
来源：http://swv.fehbvm.com

[U32] Py：代码格式化
来源：http://viv.ctjpmb.com

ruff format . && ruff check --fix .
来源：http://khu.yj20258888.top

[U33] Py：打包发布
来源：http://zkn.sweek.top

python -m build  （依赖 pyproject.toml）
来源：http://koc.daria6918.cn

[U34] Py：判断编码
来源：http://fmy.yfazqb.com

chardet.detect(raw)
来源：http://byr.cheryme.top

[U35] Py：发送邮件
来源：http://bfy.tarul.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qij.tian-w.cn

[U36] Py：定时任务
来源：http://yor.snrcjt.cn

schedule.every(10).minutes.do(job)
来源：http://bkh.jinqigufen.top

[U37] Py：读写 Excel
来源：http://qvh.hfpthk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://min.zhaomingkeji.xyz

[U38] Py：获取脚本所在目录
来源：http://unc.andypj.xyz

Path(__file__).resolve().parent
来源：http://rru.cdnleiting.top

[U39] Py：判断是否在交互环境
来源：http://pul.xuanzx.com

sys.stdout.isatty()
来源：http://elw.iojbl.cn

[U40] Py：打印到标准错误
来源：http://pfp.chenzaomai.com

print("err", file=sys.stderr)
来源：http://drs.chenzaomai.com

[U41] PHP：初始化 Composer 项目
来源：http://zpq.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://yze.ybcxt.top

[U42] PHP：PSR-4 自动加载
来源：http://fud.hfpthk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kjb.jlsjyb.cn

[U43] PHP：声明命名空间
来源：http://rvi.redwolf501.top

namespace App\Http;
来源：http://qzl.cashguo.top

[U44] PHP：开启严格类型
来源：http://lsd.zhongyouzk.top

declare(strict_types=1);
来源：http://xgj.yueranfly.top

[U45] PHP：类型声明与返回类型
来源：http://ydm.yongpay.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://umg.gaohongyu789.top

[U46] PHP：可空类型
来源：http://nqz.fktsv.cn

?string $name = null
来源：http://ezr.redwolf501.top

[U47] PHP：联合类型
来源：http://gau.birdmap.top

int|string $id
来源：http://oim.snrcjt.cn

[U48] PHP：纯枚举
来源：http://vpp.xingfuxueyuan.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ypj.xylfe.cn

[U49] PHP：只读属性
来源：http://mhw.sufxvd.cn

public readonly string $name
来源：http://sdk.yj20258.top

[U50] PHP：构造器属性提升
来源：http://yii.iojbl.cn

public function __construct(private int $id) {}
来源：http://fne.yueranfly.top

[U51] PHP：数组解构
来源：http://mhc.nanxuanxn.top

[$a, $b] = $arr;
来源：http://bbc.daxiang520.top

[U52] PHP：箭头函数
来源：http://cxl.jqgufenzy.top

$double = fn($x) => $x * 2;
来源：http://pfc.epnwcf.com

[U53] PHP：空合并运算符
来源：http://nku.gogol.net.cn

$v = $a ?? $b ?? "default";
来源：http://vdj.vqdsnc.cn

[U54] PHP：空安全调用
来源：http://nhs.jlsjyb.cn

$obj?->method()
来源：http://zut.pengpengdd.cyou

[U55] PHP：match 表达式
来源：http://cjs.nanxuanxn.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lid.hnxiangtu.top

[U56] PHP：命名参数
来源：http://etb.jinqigufen.top

f(a: 1, b: 2)
来源：http://qje.guowangkeji.top

[U57] PHP：字符串插值
来源：http://lze.gzhubu.top

"值: {$a}"
来源：http://sjk.c1oappe.top

[U58] PHP：数组三件套
来源：http://rbi.aizwys.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dtv.ybcxt.top

[U59] PHP：自定义排序
来源：http://plo.xuetiantiany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uje.guowangkeji.top

[U60] PHP：JSON 编解码
来源：http://yiw.daxiang520.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eah.meibo888.top

[U61] PHP：正则
来源：http://ncu.andypj.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ger.cqqwz.cn

[U62] PHP：日期对象
来源：http://jok.feifeiyinyue.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://boz.bjfxy.top

[U63] PHP：文件读写
来源：http://smy.jlsjyb.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tls.daria6918.cn

[U64] PHP：目录遍历
来源：http://aov.hfpthk.cn

glob("dir/*.php");  scandir("dir");
来源：http://phz.jinyuanbaomall.cn

[U65] PHP：会话
来源：http://hnj.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ult.bbcook.cn

[U66] PHP：设置 Cookie
来源：http://dmq.nanxinkj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fdn.c1oappe.top

[U67] PHP：处理文件上传
来源：http://nym.c1oappe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vrj.316326.xyz

[U68] PHP：PDO 连接
来源：http://pwt.fanxiaobao.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hsm.tian-w.cn

[U69] PHP：PDO 预处理
来源：http://vlu.cheryme.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jbs.xingfuxueyuan.xyz

[U70] PHP：PDO 事务
来源：http://itm.fehbvm.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dpf.gzhubu.top

[U71] PHP：抛出异常
来源：http://srv.shanyushiyangtech.top

throw new RuntimeException("失败", 500);
来源：http://yro.quarkkingdee.top

[U72] PHP：写错误日志
来源：http://mdo.ehwqpu.com

error_log("失败: " . $e->getMessage());
来源：http://tnb.daxiang520.top

[U73] PHP：读取 ini 配置
来源：http://pns.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://nzg.xziqi.cn

[U74] PHP：读取环境变量
来源：http://qwz.wangdashe.top

getenv("APP_ENV") ?: "production"
来源：http://kip.uphjek.com

[U75] PHP：依赖注入
来源：http://zhx.wangdashe.top

composer require psr/container
来源：http://mvz.chenjidiqi.icu

[U76] PHP：简单路由
来源：http://mrs.hnxiangtu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://azv.aibaodan.cn

[U77] PHP：模板渲染
来源：http://msj.zhoulong.xyz

composer require twig/twig
来源：http://oed.zhoulong.xyz

[U78] PHP：单元测试
来源：http://xxt.jinghuilouyu.cn

composer require --dev phpunit/phpunit
来源：http://wvy.jlsjyb.cn

[U79] PHP：静态分析
来源：http://mrk.jqgufenzy.top

composer require --dev phpstan/phpstan
来源：http://vbj.hysaishi.cn

[U80] PHP：代码规范修复
来源：http://igk.zhixingplan.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://imm.jqgfzy.top

[U81] JS：初始化项目
来源：http://kpg.hcnkem.com

npm init -y;  npm i express
来源：http://kqi.0kj1m.cn

[U82] JS：package.json 脚本
来源：http://jxo.shuidangran.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://toe.zdbjq.cn

[U83] JS：ES Module 导入导出
来源：http://bvd.c1oappe.top

export const a = 1;  import { a } from "./m.js";
来源：http://pio.hnqzz.top

[U84] JS：CommonJS 写法
来源：http://rnj.guowangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://wso.fanxiaobao.xyz

[U85] JS：可选链
来源：http://ilk.nanxuanxn.top

a?.b?.c
来源：http://tpu.yvedp.cn

[U86] JS：空值合并
来源：http://ixg.vehdjk.com

a ?? b
来源：http://fqc.hammf.cn

[U87] JS：解构默认值
来源：http://fkd.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://zmq.ywan-chungtsiang.top

[U88] JS：对象展开合并
来源：http://xim.yueranfly.top

{ ...a, ...b }
来源：http://son.xuetiantiany.cn

[U89] JS：数组去重
来源：http://xgr.ybcxt.top

[...new Set(arr)]
来源：http://vpz.chenlongwang.top

[U90] JS：数字数组排序
来源：http://yaz.jinqigfzy.top

[...arr].sort((a, b) => a - b)
来源：http://jaj.ybcxt.top

[U91] JS：对象键值遍历
来源：http://waz.hammf.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hyz.gogol.net.cn

[U92] JS：深拷贝
来源：http://jkz.yfazqb.com

structuredClone(obj)
来源：http://cwv.gogol.net.cn

[U93] JS：模板字符串
来源：http://mtc.uphjek.com

`共 ${n} 条`
来源：http://vxl.sweek.top

[U94] JS：箭头函数
来源：http://qlk.shuidangran.top

const double = x => x * 2;
来源：http://crs.sxryk.cn

[U95] JS：Promise 包装
来源：http://sgo.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://dqm.yonumen.top

[U96] JS：async/await 与异常
来源：http://ceq.tian-w.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ajc.yvedp.cn

[U97] JS：并发请求
来源：http://lhh.hesvh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jwx.ybcxt.top

[U98] JS：fetch 带 JSON
来源：http://ksw.chenlongwang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ouf.smart0.xyz

[U99] JS：事件监听
来源：http://yho.cqqwz.cn

el.addEventListener("click", e => {})
来源：http://ajs.xuetiantiany.cn

[U100] JS：DOM 查询
来源：http://whw.pengpengdd.cyou

document.querySelector(".item")
来源：http://vaw.cheryme.top

[U101] JS：classList 操作
来源：http://rav.jlsjyb.cn

el.classList.toggle("active")
来源：http://uxf.guowangkeji.top

[U102] JS：本地存储
来源：http://bbi.hfpthk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://isy.tian-w.cn

[U103] JS：定时器
来源：http://vtu.sufxvd.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://srk.shanyushiyangtech.top

[U104] JS：防抖
来源：http://rus.ivvv.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iln.yvedp.cn

[U105] JS：节流
来源：http://yyt.snrcjt.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zzc.zhixingplan.top

[U106] JS：日期格式化
来源：http://mrz.chenzaomai.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mqw.52xcode.cn

[U107] JS：数字千分位
来源：http://ivs.ehwqpu.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dtk.cdnleiting.top

[U108] JS：随机整数
来源：http://gvk.jlsjyb.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ona.jinghuilouyu.cn

[U109] JS：数组分组
来源：http://weg.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://hcj.bbcook.cn

[U110] JS：数组分块
来源：http://eri.zhixingplan.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://epe.aizwys.cn

[U111] JS：对象转 Map
来源：http://xhr.snrcjt.cn

new Map(Object.entries(obj))
来源：http://odg.xinyue.icu

[U112] JS：字符串补位
来源：http://gjw.jinghuilouyu.cn

"7".padStart(3, "0")
来源：http://mrm.yj20258888.top

[U113] JS：正则替换全部
来源：http://rfz.fengsongda.top

s.replaceAll("a", "b")
来源：http://ktg.cashguo.top

[U114] JS：JSON 深比较
来源：http://rck.yj202588.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ugy.bjfxy.top

[U115] JS：生成 UUID
来源：http://vyu.fengsongda.top

crypto.randomUUID()
来源：http://mcc.yj20258.top

[U116] JS：类型检查（JSDoc）
来源：http://jtp.cashguo.top

/** @param {string} name */ function f(name) {}
来源：http://gry.jinyuanbaomall.cn

[U117] JS：单元测试
来源：http://umr.jqgufenzy.top

npm i -D vitest;  npx vitest
来源：http://yks.tanke756.top

[U118] JS：开发服务器
来源：http://yao.tarul.cn

npm i -D vite;  npx vite
来源：http://sta.yonumen.top

[U119] JS：生产构建
来源：http://cwt.gzhubu.top

npx vite build
来源：http://bng.fengsongda.top

[U120] JS：读取环境变量（Vite）
来源：http://lsw.jqgufenzy.top

import.meta.env.VITE_API_URL
来源：http://rjr.yonumen.top

================================================================================
来源：http://fmu.feifeiyinyue.top

统计汇总
来源：http://xhu.daria6918.cn

================================================================================
来源：http://zgu.cdnleiting.top

按语言统计（条）：
来源：http://euo.jyoumei.cn

Python ......... 252
来源：http://cwi.tarul.cn

PHP ............ 252
来源：http://ukv.sxryk.cn

JavaScript ..... 252
来源：http://ufd.jinyuanbaomall.cn

TypeScript ..... 212
来源：http://zyi.cqqwz.cn

Java ........... 212
来源：http://djl.bbcook.cn

Go ............. 212
来源：http://bak.guannengcc.top

Ruby ........... 212
来源：http://seo.cqqwz.cn

C# ............. 212
来源：http://rot.pycfn.com

C .............. 30
来源：http://ckw.daxiang520.top

C++ ............ 30
来源：http://utw.hongshengwenyu.top

SQL ............ 90
来源：http://xir.tanke756.top

Bash ........... 80
来源：http://qcv.zhoulong.xyz

Kotlin ......... 15
来源：http://iuo.sysykeji.top

Swift .......... 15
来源：http://oti.jiagoushi.top

Lua ............ 10
来源：http://oyb.zhaomingkeji.xyz

Perl ........... 10
来源：http://ceb.hongshengwenyu.top

Scala .......... 10
来源：http://ckl.aizwys.cn

------------------------------------
来源：http://meo.jinghuilouyu.cn

合计 ........... 2106 条
来源：http://fdh.hnxiangtu.top

按章节统计：
来源：http://aqz.shanyushiyangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hss.ppjwa.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mse.ehwqpu.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://quy.zdbjq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iwu.yj20258.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zsz.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://juu.zhoulong.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://klx.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iam.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bhl.zdqjudy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fou.yuanzhike.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yki.fengsongda.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://frc.yj20258.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ivg.xingfuxueyuan.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qfh.hysaishi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bnv.ctjpmb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rbe.quarkkingdee.top

Q SQL 专题                              90
来源：http://iyy.sjlbkw.cn

R Bash 专题                             80
来源：http://wha.hesvh.cn

S C / C++ 专题                          60
来源：http://mle.guowangkeji.top

T 其他语言补充                          60
来源：http://ykb.yongpay.top

U 高频实用片段                         120
来源：http://hwq.uphjek.com

------------------------------------
来源：http://mps.hywenlv.cn

合计                                  2106 条
来源：http://wym.vehdjk.com

--------------------------------------------------------------------------------
来源：http://ubo.birdmap.top

使用提醒
来源：http://pay.fehbvm.com

--------------------------------------------------------------------------------
来源：http://nhp.xylfe.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rqi.yj202588.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bmw.chenzaomai.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://poj.ctjpmb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://tmy.feifeiyinyue.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://noi.cqqwz.cn

—— 文件结束 ——
来源：http://qpg.vqdsnc.cn

================================================================================
来源：http://gkw.shanyushiyangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://ybu.jinyuanbaomall.cn

Common Programming Examples Cheat Book
来源：http://udr.ywan-chungtsiang.top

================================================================================
来源：http://mbc.jqgfzy.top

【收录内容】
来源：http://gpd.hammf.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://uie.jinghuilouyu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wwd.hcnkem.com

SQL · Bash · C · C++
来源：http://fqm.wangdashe.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ivj.jiagoushi.top

【使用说明】
来源：http://uky.jyoumei.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kuh.ywan-chungtsiang.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dzp.zhiwuduotai.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ddc.shuidangran.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ddu.guannengcc.top

Bash:  Shell         C:     C             C++:   C++
来源：http://puc.yj20258888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gfd.yanxiufei.cn


<!-- 参考信息 -->