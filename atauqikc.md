代发 wailian999

[U13] Py：固定长度队列
来源：http://pwp.wangshuangyany.cn

deque(maxlen=10)
来源：http://uei.jinqigufen.top

[U14] Py：分组收集到列表
来源：http://cir.xinyue.icu

defaultdict(list)
来源：http://mmn.kuanghao11.cn

[U15] Py：高精度计时
来源：http://ysp.redwolf501.top

t = time.perf_counter()
来源：http://pnj.ywan-chungtsiang.top

[U16] Py：命令行参数解析
来源：http://zbf.havefunace.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vdt.zdqjudy.top

[U17] Py：初始化日志
来源：http://jgy.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://gsb.gogol.net.cn

[U18] Py：预编译正则
来源：http://pmw.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://mcm.yuanzhike.top

[U19] Py：正则替换带回调
来源：http://lxl.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iwy.bjfxy.top

[U20] Py：缓存函数结果
来源：http://dkv.ydzc1.top

@functools.lru_cache(maxsize=None)
来源：http://blp.gotoacloud.top

[U21] Py：自定义上下文管理器
来源：http://eiw.jinghuilouyu.cn

@contextlib.contextmanager
来源：http://nge.tanke756.top

[U22] Py：矩阵转置
来源：http://uia.kuanghao11.cn

list(zip(*m))
来源：http://ddc.jinyuanbaomall.cn

[U23] Py：分块读取大文件
来源：http://fda.pengpengdd.cyou

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ksp.fehbvm.com

[U24] Py：路径操作
来源：http://kix.guannengcc.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ihh.gotoacloud.top

[U25] Py：CSV 按字典读
来源：http://jan.yj20258.top

csv.DictReader(f)
来源：http://rvd.shuidangran.top

[U26] Py：并发下载
来源：http://nge.jinqigufen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zzz.pengpengdd.cyou

[U27] Py：异步 HTTP
来源：http://aan.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://qwg.dianchejie.cn

[U28] Py：类型别名
来源：http://pct.birdmap.top

UserId = int
来源：http://dyf.fengsongda.top

[U29] Py：属性校验
来源：http://azu.jqgfzy.top

@property 与 @x.setter 配合
来源：http://yis.yanxiufei.cn

[U30] Py：数据类
来源：http://hwc.xylfe.cn

@dataclass(slots=True)
来源：http://hij.chenlongwang.top

[U31] Py：单测
来源：http://onh.uphjek.com

python -m pytest -q
来源：http://qyi.jianghu66.top

[U32] Py：代码格式化
来源：http://wyv.xingfuxueyuan.xyz

ruff format . && ruff check --fix .
来源：http://olt.yj202588.top

[U33] Py：打包发布
来源：http://yok.hesvh.cn

python -m build  （依赖 pyproject.toml）
来源：http://xrq.fehbvm.com

[U34] Py：判断编码
来源：http://wdt.yvedp.cn

chardet.detect(raw)
来源：http://iqo.shzxlz.cn

[U35] Py：发送邮件
来源：http://kzo.zdqjudy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://plw.yongpay.top

[U36] Py：定时任务
来源：http://dsd.jlsjyb.cn

schedule.every(10).minutes.do(job)
来源：http://fta.yonumen.top

[U37] Py：读写 Excel
来源：http://mjr.quarkkingdee.top

pandas.read_excel / DataFrame.to_excel
来源：http://ebq.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://pwf.yvedp.cn

Path(__file__).resolve().parent
来源：http://abq.chenzaomai.com

[U39] Py：判断是否在交互环境
来源：http://jiz.jqgfzy.top

sys.stdout.isatty()
来源：http://ltr.shanyushiyangtech.top

[U40] Py：打印到标准错误
来源：http://zwc.cheryme.top

print("err", file=sys.stderr)
来源：http://zlg.zhiwuduotai.top

[U41] PHP：初始化 Composer 项目
来源：http://fll.vehdjk.com

composer init;  composer require guzzlehttp/guzzle
来源：http://tiq.yvedp.cn

[U42] PHP：PSR-4 自动加载
来源：http://yma.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nzf.jinghuilouyu.cn

[U43] PHP：声明命名空间
来源：http://srp.epnwcf.com

namespace App\Http;
来源：http://uoa.gogol.net.cn

[U44] PHP：开启严格类型
来源：http://ydk.chenlongwang.top

declare(strict_types=1);
来源：http://lgi.hywenlv.cn

[U45] PHP：类型声明与返回类型
来源：http://pek.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://iaz.chenlongwang.top

[U46] PHP：可空类型
来源：http://qng.nanxinkj.top

?string $name = null
来源：http://rwb.sysykeji.top

[U47] PHP：联合类型
来源：http://krs.zdqjudy.top

int|string $id
来源：http://ejt.pengpengdd.cyou

[U48] PHP：纯枚举
来源：http://kuc.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mix.jyoumei.cn

[U49] PHP：只读属性
来源：http://mhs.meibo888.top

public readonly string $name
来源：http://ibf.jinqigufen.top

[U50] PHP：构造器属性提升
来源：http://svq.kuanghao11.cn

public function __construct(private int $id) {}
来源：http://wkb.wangdashe.top

[U51] PHP：数组解构
来源：http://tyn.shanyushiyangkeji.top

[$a, $b] = $arr;
来源：http://cmp.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://qks.fktsv.cn

$double = fn($x) => $x * 2;
来源：http://urk.aibaodan.cn

[U53] PHP：空合并运算符
来源：http://nvk.chenzaomai.com

$v = $a ?? $b ?? "default";
来源：http://hpg.sysykeji.top

[U54] PHP：空安全调用
来源：http://eok.sjlbkw.cn

$obj?->method()
来源：http://noi.fzhhl.top

[U55] PHP：match 表达式
来源：http://tuo.cdnleiting.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://npd.gogol.net.cn

[U56] PHP：命名参数
来源：http://cjb.dianchejie.cn

f(a: 1, b: 2)
来源：http://ccg.vqdsnc.cn

[U57] PHP：字符串插值
来源：http://qll.wangshuangyany.cn

"值: {$a}"
来源：http://jel.xinyue.icu

[U58] PHP：数组三件套
来源：http://zow.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sfr.xuanzx.com

[U59] PHP：自定义排序
来源：http://sxl.gogol.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mmd.vqdsnc.cn

[U60] PHP：JSON 编解码
来源：http://oom.sjlbkw.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dyb.fengsongda.top

[U61] PHP：正则
来源：http://ubq.uphjek.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://thr.tian-w.cn

[U62] PHP：日期对象
来源：http://tgf.uphjek.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wsq.gotoacloud.top

[U63] PHP：文件读写
来源：http://ysv.ehwqpu.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iip.jinyuanbaomall.cn

[U64] PHP：目录遍历
来源：http://ary.aibaodan.cn

glob("dir/*.php");  scandir("dir");
来源：http://bli.wangdashe.top

[U65] PHP：会话
来源：http://txg.andypj.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://pai.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://jyw.havefunace.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://atc.zdbjq.cn

[U67] PHP：处理文件上传
来源：http://wtr.wangdashe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pae.fktsv.cn

[U68] PHP：PDO 连接
来源：http://apq.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://snt.sxryk.cn

[U69] PHP：PDO 预处理
来源：http://eyi.yonumen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uuh.cucudq.cn

[U70] PHP：PDO 事务
来源：http://hyk.nanxinkj.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eka.9152youxi.cn

[U71] PHP：抛出异常
来源：http://yfi.vehdjk.com

throw new RuntimeException("失败", 500);
来源：http://egz.ctjpmb.com

[U72] PHP：写错误日志
来源：http://zjj.shzxlz.cn

error_log("失败: " . $e->getMessage());
来源：http://vrs.tianlin.xyz

[U73] PHP：读取 ini 配置
来源：http://saz.iojbl.cn

parse_ini_file("config.ini", true)
来源：http://rrg.cashguo.top

[U74] PHP：读取环境变量
来源：http://okt.kuanghao11.cn

getenv("APP_ENV") ?: "production"
来源：http://rno.tanke756.top

[U75] PHP：依赖注入
来源：http://gln.chenlongwang.top

composer require psr/container
来源：http://nhz.fzhhl.top

[U76] PHP：简单路由
来源：http://qoc.yj20258.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iky.yj20258.top

[U77] PHP：模板渲染
来源：http://cxh.xuanzx.com

composer require twig/twig
来源：http://sou.zhijiandao.cn

[U78] PHP：单元测试
来源：http://cuw.pycfn.com

composer require --dev phpunit/phpunit
来源：http://lho.daria6918.cn

[U79] PHP：静态分析
来源：http://pfs.aizwys.cn

composer require --dev phpstan/phpstan
来源：http://qla.havefunace.top

[U80] PHP：代码规范修复
来源：http://fto.sjlbkw.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sen.cashguo.top

[U81] JS：初始化项目
来源：http://nii.yonumen.top

npm init -y;  npm i express
来源：http://dkc.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://rit.ydjk.org.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://odw.yuanzhike.top

[U83] JS：ES Module 导入导出
来源：http://pqp.yanxiufei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jit.tanke756.top

[U84] JS：CommonJS 写法
来源：http://bxz.jinqigufen.top

module.exports = { a };  const { a } = require("./m");
来源：http://ubb.jyoumei.cn

[U85] JS：可选链
来源：http://uoh.dianchejie.cn

a?.b?.c
来源：http://ozr.hcnkem.com

[U86] JS：空值合并
来源：http://mfs.yj20258.top

a ?? b
来源：http://pfm.cucudq.cn

[U87] JS：解构默认值
来源：http://szh.shangyingyoupin.top

const { a = 1, b = 2 } = obj;
来源：http://kns.daria6918.cn

[U88] JS：对象展开合并
来源：http://gmc.cdnleiting.top

{ ...a, ...b }
来源：http://cxk.fehbvm.com

[U89] JS：数组去重
来源：http://zfb.nanxinkj.top

[...new Set(arr)]
来源：http://gjm.chenlongwang.top

[U90] JS：数字数组排序
来源：http://kmr.zhaomingkeji.xyz

[...arr].sort((a, b) => a - b)
来源：http://ios.wangdashe.top

[U91] JS：对象键值遍历
来源：http://bth.gzhubu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wfc.nanxinkj.top

[U92] JS：深拷贝
来源：http://ipb.zhengqikj.top

structuredClone(obj)
来源：http://zrk.quarkkingdee.top

[U93] JS：模板字符串
来源：http://ruf.hcnkem.com

`共 ${n} 条`
来源：http://wse.wangshuangyany.cn

[U94] JS：箭头函数
来源：http://fda.cucudq.cn

const double = x => x * 2;
来源：http://xvm.shanyushiyangtech.top

[U95] JS：Promise 包装
来源：http://nvp.aizwys.cn

new Promise((resolve, reject) => {})
来源：http://iun.smart0.xyz

[U96] JS：async/await 与异常
来源：http://pco.xuetiantiany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ogv.daria6918.cn

[U97] JS：并发请求
来源：http://zzc.chenjidiqi.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://aiw.ydzc1.top

[U98] JS：fetch 带 JSON
来源：http://nbd.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://onl.gotoacloud.top

[U99] JS：事件监听
来源：http://eii.ctjpmb.com

el.addEventListener("click", e => {})
来源：http://kqc.yongpay.top

[U100] JS：DOM 查询
来源：http://vet.guowangkeji.top

document.querySelector(".item")
来源：http://bwe.wangdashe.top

[U101] JS：classList 操作
来源：http://lsa.epnwcf.com

el.classList.toggle("active")
来源：http://rbq.ivvv.top

[U102] JS：本地存储
来源：http://vyl.ywan-chungtsiang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://iam.fzhhl.top

[U103] JS：定时器
来源：http://xbg.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://smd.shangyingyoupin.top

[U104] JS：防抖
来源：http://kbg.bbcook.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vil.daxiang520.top

[U105] JS：节流
来源：http://jmg.yongpay.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tbk.smart0.xyz

[U106] JS：日期格式化
来源：http://fpm.hysaishi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hvu.9152youxi.cn

[U107] JS：数字千分位
来源：http://ikr.shzxlz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lio.feifeiyinyue.top

[U108] JS：随机整数
来源：http://ods.sysykeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sjg.jinqigufen.top

[U109] JS：数组分组
来源：http://yff.9152youxi.cn

Object.groupBy(arr, x => x.type)
来源：http://vhx.sweek.top

[U110] JS：数组分块
来源：http://tgi.wangshuangyany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ljj.jiagoushi.top

[U111] JS：对象转 Map
来源：http://kvo.smart0.xyz

new Map(Object.entries(obj))
来源：http://tpj.daria6918.cn

[U112] JS：字符串补位
来源：http://dhd.hongshengwenyu.top

"7".padStart(3, "0")
来源：http://koz.jyoumei.cn

[U113] JS：正则替换全部
来源：http://vtw.aizwys.cn

s.replaceAll("a", "b")
来源：http://cys.mhx1999.top

[U114] JS：JSON 深比较
来源：http://qvq.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hez.9152youxi.cn

[U115] JS：生成 UUID
来源：http://dny.yongpay.top

crypto.randomUUID()
来源：http://ufs.jlsjyb.cn

[U116] JS：类型检查（JSDoc）
来源：http://uas.jinghuilouyu.cn

/** @param {string} name */ function f(name) {}
来源：http://hnx.yuxming.cn

[U117] JS：单元测试
来源：http://rgy.chenzaomai.com

npm i -D vitest;  npx vitest
来源：http://drh.zhongyouzk.top

[U118] JS：开发服务器
来源：http://jtg.wangshuangyany.cn

npm i -D vite;  npx vite
来源：http://tql.hnqzz.top

[U119] JS：生产构建
来源：http://ztq.smart0.xyz

npx vite build
来源：http://drx.shuidangran.top

[U120] JS：读取环境变量（Vite）
来源：http://umh.birdmap.top

import.meta.env.VITE_API_URL
来源：http://epu.zhaomingkeji.xyz

================================================================================
来源：http://xzj.jinqigfzy.top

统计汇总
来源：http://ojt.316326.xyz

================================================================================
来源：http://xoi.xuetiantiany.cn

按语言统计（条）：
来源：http://zoa.dashuyun.cn

Python ......... 252
来源：http://mmq.uphjek.com

PHP ............ 252
来源：http://lzu.quarkkingdee.top

JavaScript ..... 252
来源：http://mnq.52xcode.cn

TypeScript ..... 212
来源：http://zvs.xingfuxueyuan.xyz

Java ........... 212
来源：http://isv.uphjek.com

Go ............. 212
来源：http://tmz.cqqwz.cn

Ruby ........... 212
来源：http://caj.yj202588.top

C# ............. 212
来源：http://ely.jinyuanbaomall.cn

C .............. 30
来源：http://sxg.pengpengdd.cyou

C++ ............ 30
来源：http://env.zhongyouzk.top

SQL ............ 90
来源：http://fxo.jinghuilouyu.cn

Bash ........... 80
来源：http://roo.ydzc1.top

Kotlin ......... 15
来源：http://vrp.ppjwa.cn

Swift .......... 15
来源：http://ngs.bbcook.cn

Lua ............ 10
来源：http://wbo.pycfn.com

Perl ........... 10
来源：http://ntt.yj20258.top

Scala .......... 10
来源：http://zwq.ydjk.org.cn

------------------------------------
来源：http://lrw.jqgfzy.top

合计 ........... 2106 条
来源：http://qam.bbcook.cn

按章节统计：
来源：http://oel.hongshengwenyu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ytw.yanxiufei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bvp.ybcxt.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://giz.shangyingyoupin.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://csw.hnxiangtu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lpb.zhixingplan.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hdx.fzhhl.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nlt.shuidangran.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mhk.hcnkem.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ozs.yangfankeji.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uga.iojbl.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vrb.jinyuanbaomall.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mbz.yj20258.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rzp.shangyingyoupin.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sxx.ctjpmb.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wwz.epnwcf.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://htl.xziqi.cn

Q SQL 专题                              90
来源：http://uhx.jqgfzy.top

R Bash 专题                             80
来源：http://zeo.hesvh.cn

S C / C++ 专题                          60
来源：http://ijk.cqqwz.cn

T 其他语言补充                          60
来源：http://mct.zdbjq.cn

U 高频实用片段                         120
来源：http://jtd.chenjidiqi.icu

------------------------------------
来源：http://rnp.zhongyouzk.top

合计                                  2106 条
来源：http://hcz.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://vjb.chenjidiqi.icu

使用提醒
来源：http://ibj.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://lhb.tanke756.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://efq.andypj.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hrs.pycfn.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xzf.andypj.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://vme.shzxlz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mzj.wangdashe.top

—— 文件结束 ——
来源：http://upv.nanxinkj.top

================================================================================
来源：http://wcj.hongshengwenyu.top

程序语言常见例子速查手册（2024 版）
来源：http://keo.sweek.top

Common Programming Examples Cheat Book
来源：http://mor.sweek.top

================================================================================
来源：http://vvu.cashguo.top

【收录内容】
来源：http://stb.dashuyun.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rre.yuxming.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ppb.ivvv.top

SQL · Bash · C · C++
来源：http://nhd.jinghuilouyu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://edc.guowangkeji.top

【使用说明】
来源：http://zcn.yanxiufei.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bpf.zhiwuduotai.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fxv.yangfankeji.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ogq.fzhhl.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://enp.yueranfly.top

Bash:  Shell         C:     C             C++:   C++
来源：http://uky.bjfxy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ydm.ydjk.org.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gza.chenlongwang.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bgc.ybcxt.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yym.daria6918.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uwm.shanyushiyangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bvh.jyoumei.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jzj.shanyushiyangtech.top

【文件统计】
来源：http://wke.meibo888.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eby.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://rhm.mhx1999.top

目  录
来源：http://fph.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://gjn.hesvh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wmb.smart0.xyz


<!-- 参考信息 -->