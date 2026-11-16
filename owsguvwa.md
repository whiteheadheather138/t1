代发 wailian999

[U09] Py：字典取最大值的键
来源：http://gwp.tarul.cn

max(d, key=d.get)
来源：http://elb.yanxiufei.cn

[U10] Py：按值排序字典
来源：http://fqm.aibaodan.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dth.hongshengwenyu.top

[U11] Py：生成器表达式
来源：http://ndl.ctjpmb.com

(x * 2 for x in arr)
来源：http://bla.jiagoushi.top

[U12] Py：取出现最多的 3 个元素
来源：http://bdo.ybcxt.top

Counter(arr).most_common(3)
来源：http://zsj.ivvv.top

[U13] Py：固定长度队列
来源：http://ceo.daria6918.cn

deque(maxlen=10)
来源：http://dfu.yonumen.top

[U14] Py：分组收集到列表
来源：http://xgq.sysykeji.top

defaultdict(list)
来源：http://jal.yfazqb.com

[U15] Py：高精度计时
来源：http://rrx.wangdashe.top

t = time.perf_counter()
来源：http://erw.sxryk.cn

[U16] Py：命令行参数解析
来源：http://dym.nwbrower.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qpi.meibo888.top

[U17] Py：初始化日志
来源：http://iex.hnqzz.top

logging.basicConfig(level=logging.INFO)
来源：http://eai.yj20258888.top

[U18] Py：预编译正则
来源：http://jpj.yueranfly.top

pat = re.compile(r"\d+")
来源：http://hvh.cucudq.cn

[U19] Py：正则替换带回调
来源：http://kxt.shuidangran.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ugn.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://msd.vqdsnc.cn

@functools.lru_cache(maxsize=None)
来源：http://chz.cashguo.top

[U21] Py：自定义上下文管理器
来源：http://wet.cashguo.top

@contextlib.contextmanager
来源：http://bah.daxiang520.top

[U22] Py：矩阵转置
来源：http://gby.sufxvd.cn

list(zip(*m))
来源：http://qss.yvedp.cn

[U23] Py：分块读取大文件
来源：http://eje.vqdsnc.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mdh.shuidangran.top

[U24] Py：路径操作
来源：http://icj.zhoulong.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tfz.snrcjt.cn

[U25] Py：CSV 按字典读
来源：http://ddc.tanke756.top

csv.DictReader(f)
来源：http://rwl.vehdjk.com

[U26] Py：并发下载
来源：http://bvy.cdnleiting.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xgc.ppjwa.cn

[U27] Py：异步 HTTP
来源：http://nmn.xinyue.icu

aiohttp.ClientSession() 配合 async with
来源：http://wka.zhiwuduotai.top

[U28] Py：类型别名
来源：http://bvl.jinqigufen.top

UserId = int
来源：http://dib.jinyuanbaomall.cn

[U29] Py：属性校验
来源：http://ozd.hongshengwenyu.top

@property 与 @x.setter 配合
来源：http://wgw.epnwcf.com

[U30] Py：数据类
来源：http://klt.jinqigfzy.top

@dataclass(slots=True)
来源：http://dqq.shanyushiyangkeji.top

[U31] Py：单测
来源：http://yog.ydzc1.top

python -m pytest -q
来源：http://zbw.gaohongyu789.top

[U32] Py：代码格式化
来源：http://zvg.jyoumei.cn

ruff format . && ruff check --fix .
来源：http://wyd.yongpay.top

[U33] Py：打包发布
来源：http://krr.yanxiufei.cn

python -m build  （依赖 pyproject.toml）
来源：http://bpf.svipenyu.cn

[U34] Py：判断编码
来源：http://tmj.ppjwa.cn

chardet.detect(raw)
来源：http://txz.hammf.cn

[U35] Py：发送邮件
来源：http://eti.sxryk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wxi.xingfuxueyuan.xyz

[U36] Py：定时任务
来源：http://rvc.hesvh.cn

schedule.every(10).minutes.do(job)
来源：http://ccq.cdnleiting.top

[U37] Py：读写 Excel
来源：http://nah.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://jai.zdqjudy.top

[U38] Py：获取脚本所在目录
来源：http://meo.hcnkem.com

Path(__file__).resolve().parent
来源：http://ukf.birdmap.top

[U39] Py：判断是否在交互环境
来源：http://xoc.xingfuxueyuan.xyz

sys.stdout.isatty()
来源：http://dxr.bbcook.cn

[U40] Py：打印到标准错误
来源：http://wjo.xylfe.cn

print("err", file=sys.stderr)
来源：http://zrw.zhixingplan.top

[U41] PHP：初始化 Composer 项目
来源：http://krs.hongshengwenyu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zgb.cheryme.top

[U42] PHP：PSR-4 自动加载
来源：http://jby.guowangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wvj.52xcode.cn

[U43] PHP：声明命名空间
来源：http://spk.yuanzhike.top

namespace App\Http;
来源：http://ifl.gotoacloud.top

[U44] PHP：开启严格类型
来源：http://yir.shzxlz.cn

declare(strict_types=1);
来源：http://bim.xylfe.cn

[U45] PHP：类型声明与返回类型
来源：http://vba.daxiang520.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ady.zhengqikj.top

[U46] PHP：可空类型
来源：http://row.shanyushiyangkeji.top

?string $name = null
来源：http://ose.chenzaomai.com

[U47] PHP：联合类型
来源：http://rfu.hnqzz.top

int|string $id
来源：http://skr.chenlongwang.top

[U48] PHP：纯枚举
来源：http://rcm.birdmap.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ysj.fanxiaobao.xyz

[U49] PHP：只读属性
来源：http://iof.zdbjq.cn

public readonly string $name
来源：http://qjo.havefunace.top

[U50] PHP：构造器属性提升
来源：http://mjm.birdmap.top

public function __construct(private int $id) {}
来源：http://qut.fktsv.cn

[U51] PHP：数组解构
来源：http://nhe.bbcook.cn

[$a, $b] = $arr;
来源：http://cqb.jianghu66.top

[U52] PHP：箭头函数
来源：http://gsd.gotoacloud.top

$double = fn($x) => $x * 2;
来源：http://mcu.zycfv.cn

[U53] PHP：空合并运算符
来源：http://dcs.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://ejh.cucudq.cn

[U54] PHP：空安全调用
来源：http://fod.ybcxt.top

$obj?->method()
来源：http://xml.shzxlz.cn

[U55] PHP：match 表达式
来源：http://hcj.zhaomingkeji.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kjj.sufxvd.cn

[U56] PHP：命名参数
来源：http://gtw.shzxlz.cn

f(a: 1, b: 2)
来源：http://bsg.cheryme.top

[U57] PHP：字符串插值
来源：http://xcl.yuxming.cn

"值: {$a}"
来源：http://xjh.pycfn.com

[U58] PHP：数组三件套
来源：http://qth.shangyingyoupin.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gio.nanxinkj.top

[U59] PHP：自定义排序
来源：http://ysl.haohaochexian.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cle.shanyushiyangkeji.top

[U60] PHP：JSON 编解码
来源：http://ghh.jqgfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fiz.yangfankeji.com

[U61] PHP：正则
来源：http://xhs.ppjwa.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lgk.meibo888.top

[U62] PHP：日期对象
来源：http://lag.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sqw.yj20258888.top

[U63] PHP：文件读写
来源：http://rga.kuanghao11.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jcq.zhixingplan.top

[U64] PHP：目录遍历
来源：http://wwz.tianlin.xyz

glob("dir/*.php");  scandir("dir");
来源：http://irx.iojbl.cn

[U65] PHP：会话
来源：http://agf.jinyuanbaomall.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ejh.zhoulong.xyz

[U66] PHP：设置 Cookie
来源：http://swy.hesvh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://smc.hongshengwenyu.top

[U67] PHP：处理文件上传
来源：http://plq.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wqw.yonumen.top

[U68] PHP：PDO 连接
来源：http://dbq.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iut.bjfxy.top

[U69] PHP：PDO 预处理
来源：http://jlc.hywenlv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://elk.zhiwuduotai.top

[U70] PHP：PDO 事务
来源：http://hjo.ywan-chungtsiang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pwi.yvedp.cn

[U71] PHP：抛出异常
来源：http://cnp.tian-w.cn

throw new RuntimeException("失败", 500);
来源：http://znm.xylfe.cn

[U72] PHP：写错误日志
来源：http://lsd.pengpengdd.cyou

error_log("失败: " . $e->getMessage());
来源：http://hkv.guannengcc.top

[U73] PHP：读取 ini 配置
来源：http://oup.shangyingyoupin.top

parse_ini_file("config.ini", true)
来源：http://opt.daxiang520.top

[U74] PHP：读取环境变量
来源：http://fwv.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://uol.jyoumei.cn

[U75] PHP：依赖注入
来源：http://wan.yj20258888.top

composer require psr/container
来源：http://eqs.jianghu66.top

[U76] PHP：简单路由
来源：http://yyh.nanxinkj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qmh.fanxiaobao.xyz

[U77] PHP：模板渲染
来源：http://yli.snrcjt.cn

composer require twig/twig
来源：http://zlw.svipenyu.cn

[U78] PHP：单元测试
来源：http://ytj.hfpthk.cn

composer require --dev phpunit/phpunit
来源：http://kor.tanke756.top

[U79] PHP：静态分析
来源：http://ozc.gotoacloud.top

composer require --dev phpstan/phpstan
来源：http://snn.zhoulong.xyz

[U80] PHP：代码规范修复
来源：http://xcq.gaohongyu789.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bgb.iojbl.cn

[U81] JS：初始化项目
来源：http://rpd.ppjwa.cn

npm init -y;  npm i express
来源：http://dgq.kuanghao11.cn

[U82] JS：package.json 脚本
来源：http://htd.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dfn.sjlbkw.cn

[U83] JS：ES Module 导入导出
来源：http://ocu.ywan-chungtsiang.top

export const a = 1;  import { a } from "./m.js";
来源：http://xou.smart0.xyz

[U84] JS：CommonJS 写法
来源：http://mac.wangshuangyany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lcc.snrcjt.cn

[U85] JS：可选链
来源：http://gyo.nanxinkj.top

a?.b?.c
来源：http://cev.aibaodan.cn

[U86] JS：空值合并
来源：http://rzl.tianlin.xyz

a ?? b
来源：http://ciw.quarkkingdee.top

[U87] JS：解构默认值
来源：http://yba.jqgfzy.top

const { a = 1, b = 2 } = obj;
来源：http://vuy.tian-w.cn

[U88] JS：对象展开合并
来源：http://efs.tian-w.cn

{ ...a, ...b }
来源：http://hoq.xuetiantiany.cn

[U89] JS：数组去重
来源：http://udz.snrcjt.cn

[...new Set(arr)]
来源：http://lkv.52xcode.cn

[U90] JS：数字数组排序
来源：http://ook.pengpengdd.cyou

[...arr].sort((a, b) => a - b)
来源：http://cdw.c1oappe.top

[U91] JS：对象键值遍历
来源：http://osk.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ooc.bjfxy.top

[U92] JS：深拷贝
来源：http://dik.hongshengwenyu.top

structuredClone(obj)
来源：http://pil.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://uhx.cheryme.top

`共 ${n} 条`
来源：http://lsw.hongshengwenyu.top

[U94] JS：箭头函数
来源：http://avl.jinqigfzy.top

const double = x => x * 2;
来源：http://uak.cqqwz.cn

[U95] JS：Promise 包装
来源：http://exq.epnwcf.com

new Promise((resolve, reject) => {})
来源：http://hxt.hammf.cn

[U96] JS：async/await 与异常
来源：http://ivh.tian-w.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zap.hongshengwenyu.top

[U97] JS：并发请求
来源：http://ixn.sjlbkw.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mpz.xuanzx.com

[U98] JS：fetch 带 JSON
来源：http://csz.fengsongda.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gqr.nwbrower.top

[U99] JS：事件监听
来源：http://vje.tarul.cn

el.addEventListener("click", e => {})
来源：http://bmo.ydzc1.top

[U100] JS：DOM 查询
来源：http://oap.ctjpmb.com

document.querySelector(".item")
来源：http://doh.c1oappe.top

[U101] JS：classList 操作
来源：http://buh.shangyingyoupin.top

el.classList.toggle("active")
来源：http://ksl.cheryme.top

[U102] JS：本地存储
来源：http://wmm.zycfv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fut.316326.xyz

[U103] JS：定时器
来源：http://ctl.xylfe.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ocy.tianlin.xyz

[U104] JS：防抖
来源：http://suj.cqqwz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zmi.kuanghao11.cn

[U105] JS：节流
来源：http://seq.ctjpmb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kuk.hfpthk.cn

[U106] JS：日期格式化
来源：http://pps.aibaodan.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ylp.nwbrower.top

[U107] JS：数字千分位
来源：http://dgm.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lqy.cucudq.cn

[U108] JS：随机整数
来源：http://hjh.guannengcc.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gdf.redwolf501.top

[U109] JS：数组分组
来源：http://nrx.c1oappe.top

Object.groupBy(arr, x => x.type)
来源：http://jvj.sweek.top

[U110] JS：数组分块
来源：http://eoy.chenjidiqi.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mkr.ehwqpu.com

[U111] JS：对象转 Map
来源：http://wul.yonumen.top

new Map(Object.entries(obj))
来源：http://urz.ybcxt.top

[U112] JS：字符串补位
来源：http://xbp.nwbrower.top

"7".padStart(3, "0")
来源：http://hju.jqgfzy.top

[U113] JS：正则替换全部
来源：http://zii.hongshengwenyu.top

s.replaceAll("a", "b")
来源：http://mxj.hnxiangtu.top

[U114] JS：JSON 深比较
来源：http://cyq.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://psi.bbcook.cn

[U115] JS：生成 UUID
来源：http://zzy.daria6918.cn

crypto.randomUUID()
来源：http://qgc.zhijiandao.cn

[U116] JS：类型检查（JSDoc）
来源：http://ozd.xziqi.cn

/** @param {string} name */ function f(name) {}
来源：http://lds.gotoacloud.top

[U117] JS：单元测试
来源：http://nom.bbcook.cn

npm i -D vitest;  npx vitest
来源：http://rme.jyoumei.cn

[U118] JS：开发服务器
来源：http://wza.jyoumei.cn

npm i -D vite;  npx vite
来源：http://okg.xingfuxueyuan.xyz

[U119] JS：生产构建
来源：http://zqi.yongpay.top

npx vite build
来源：http://pvr.gzhubu.top

[U120] JS：读取环境变量（Vite）
来源：http://fyf.daria6918.cn

import.meta.env.VITE_API_URL
来源：http://dva.fengsongda.top

================================================================================
来源：http://aox.nanxuanxn.top

统计汇总
来源：http://pag.zhoulong.xyz

================================================================================
来源：http://iug.9152youxi.cn

按语言统计（条）：
来源：http://uxo.nwbrower.top

Python ......... 252
来源：http://sjx.cqqwz.cn

PHP ............ 252
来源：http://atg.daria6918.cn

JavaScript ..... 252
来源：http://qdx.vqdsnc.cn

TypeScript ..... 212
来源：http://zmi.zdbjq.cn

Java ........... 212
来源：http://pyv.fengsongda.top

Go ............. 212
来源：http://knc.ppjwa.cn

Ruby ........... 212
来源：http://pjr.vehdjk.com

C# ............. 212
来源：http://toq.zhongyouzk.top

C .............. 30
来源：http://gev.jianghu66.top

C++ ............ 30
来源：http://irh.yj20258888.top

SQL ............ 90
来源：http://lfi.fzhhl.top

Bash ........... 80
来源：http://mod.iojbl.cn

Kotlin ......... 15
来源：http://exb.feifeiyinyue.top

Swift .......... 15
来源：http://esd.cqqwz.cn

Lua ............ 10
来源：http://zdz.hesvh.cn

Perl ........... 10
来源：http://pjc.sufxvd.cn

Scala .......... 10
来源：http://qtt.sufxvd.cn

------------------------------------
来源：http://ayp.xinyue.icu

合计 ........... 2106 条
来源：http://rrz.xingfuxueyuan.xyz

按章节统计：
来源：http://fhi.iojbl.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nqj.bjfxy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ggv.zhijiandao.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lws.birdmap.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kzm.gaohongyu789.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://elz.daxiang520.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uyl.xuetiantiany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hcy.sweek.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zkj.bbcook.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://whb.sjlbkw.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fsx.zdqjudy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gua.zhoulong.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pch.yonumen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lij.dashuyun.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ryp.gaohongyu789.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bqu.smart0.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gje.uphjek.com

Q SQL 专题                              90
来源：http://hhr.feifeiyinyue.top

R Bash 专题                             80
来源：http://ljm.ivvv.top

S C / C++ 专题                          60
来源：http://ouc.hammf.cn

T 其他语言补充                          60
来源：http://aye.zhijiandao.cn

U 高频实用片段                         120
来源：http://lnw.aibaodan.cn

------------------------------------
来源：http://luc.ehwqpu.com

合计                                  2106 条
来源：http://ycq.hcnkem.com

--------------------------------------------------------------------------------
来源：http://ofx.ywan-chungtsiang.top

使用提醒
来源：http://jfc.xylfe.cn

--------------------------------------------------------------------------------
来源：http://giv.zhengqikj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jvi.chenzaomai.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xhi.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ubc.ywan-chungtsiang.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hhs.0kj1m.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ksr.ehwqpu.com

—— 文件结束 ——
来源：http://kjh.zhoulong.xyz

================================================================================
来源：http://kmd.cashguo.top

程序语言常见例子速查手册（2024 版）
来源：http://kfi.yj20258888.top

Common Programming Examples Cheat Book
来源：http://xar.tanke756.top

================================================================================
来源：http://rtb.ctjpmb.com

【收录内容】
来源：http://zrc.xingfuxueyuan.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://iqg.gaohongyu789.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xri.yuanzhike.top

SQL · Bash · C · C++
来源：http://rmi.gaohongyu789.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hzs.jiagoushi.top

【使用说明】
来源：http://axn.xuanzx.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xbf.cqqwz.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kxi.ehwqpu.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://umy.pycfn.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qnb.tianlin.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://orr.iojbl.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mmy.ppjwa.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://njq.wangdashe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fri.wangdashe.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ljn.mhx1999.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gdv.gaohongyu789.top


<!-- 参考信息 -->