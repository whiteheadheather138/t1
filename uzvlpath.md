代发 wailian999

[U15] Py：高精度计时
来源：http://npq.yueranfly.top

t = time.perf_counter()
来源：http://sxu.guannengcc.top

[U16] Py：命令行参数解析
来源：http://vfr.aibaodan.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pnt.yuxming.cn

[U17] Py：初始化日志
来源：http://yoi.zhaomingkeji.xyz

logging.basicConfig(level=logging.INFO)
来源：http://mqc.316326.xyz

[U18] Py：预编译正则
来源：http://kfs.fehbvm.com

pat = re.compile(r"\d+")
来源：http://kcf.nanxuanxn.top

[U19] Py：正则替换带回调
来源：http://cuw.andypj.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://muu.yanxiufei.cn

[U20] Py：缓存函数结果
来源：http://dsa.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://ilv.jinyuanbaomall.cn

[U21] Py：自定义上下文管理器
来源：http://btp.jiagoushi.top

@contextlib.contextmanager
来源：http://jth.andypj.xyz

[U22] Py：矩阵转置
来源：http://aui.daria6918.cn

list(zip(*m))
来源：http://cgo.dashuyun.cn

[U23] Py：分块读取大文件
来源：http://vrk.tian-w.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ykz.hcnkem.com

[U24] Py：路径操作
来源：http://ekz.fzhhl.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dod.gaohongyu789.top

[U25] Py：CSV 按字典读
来源：http://mai.xylfe.cn

csv.DictReader(f)
来源：http://xkj.aizwys.cn

[U26] Py：并发下载
来源：http://rrv.shzxlz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://coe.shzxlz.cn

[U27] Py：异步 HTTP
来源：http://ynh.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://okc.yangfankeji.com

[U28] Py：类型别名
来源：http://oha.cheryme.top

UserId = int
来源：http://lrk.nanxuanxn.top

[U29] Py：属性校验
来源：http://hjz.zhixingplan.top

@property 与 @x.setter 配合
来源：http://rkd.jianghu66.top

[U30] Py：数据类
来源：http://hln.xziqi.cn

@dataclass(slots=True)
来源：http://pzn.yfazqb.com

[U31] Py：单测
来源：http://bdk.tian-w.cn

python -m pytest -q
来源：http://odh.meibo888.top

[U32] Py：代码格式化
来源：http://jzl.zhiwuduotai.top

ruff format . && ruff check --fix .
来源：http://ipx.jinqigufen.top

[U33] Py：打包发布
来源：http://qjm.c1oappe.top

python -m build  （依赖 pyproject.toml）
来源：http://tlj.nanxuanxn.top

[U34] Py：判断编码
来源：http://zmj.ybcxt.top

chardet.detect(raw)
来源：http://vzl.jinqigufen.top

[U35] Py：发送邮件
来源：http://gml.ivvv.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xhd.fktsv.cn

[U36] Py：定时任务
来源：http://ymv.hnqzz.top

schedule.every(10).minutes.do(job)
来源：http://rur.cashguo.top

[U37] Py：读写 Excel
来源：http://bqp.xuanzx.com

pandas.read_excel / DataFrame.to_excel
来源：http://ofe.shanyushiyangkeji.top

[U38] Py：获取脚本所在目录
来源：http://onh.jianghu66.top

Path(__file__).resolve().parent
来源：http://vze.yuanzhike.top

[U39] Py：判断是否在交互环境
来源：http://soj.zycfv.cn

sys.stdout.isatty()
来源：http://srg.svipenyu.cn

[U40] Py：打印到标准错误
来源：http://gzt.vehdjk.com

print("err", file=sys.stderr)
来源：http://xfv.wangdashe.top

[U41] PHP：初始化 Composer 项目
来源：http://fme.yonumen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://haj.yvedp.cn

[U42] PHP：PSR-4 自动加载
来源：http://ohw.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jhm.zhongyouzk.top

[U43] PHP：声明命名空间
来源：http://wcx.ybcxt.top

namespace App\Http;
来源：http://gko.mhx1999.top

[U44] PHP：开启严格类型
来源：http://jax.andypj.xyz

declare(strict_types=1);
来源：http://jdn.xuetiantiany.cn

[U45] PHP：类型声明与返回类型
来源：http://jbl.zycfv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jun.yueranfly.top

[U46] PHP：可空类型
来源：http://emn.fktsv.cn

?string $name = null
来源：http://vvv.yvedp.cn

[U47] PHP：联合类型
来源：http://bth.zhoulong.xyz

int|string $id
来源：http://vgb.birdmap.top

[U48] PHP：纯枚举
来源：http://qhv.cashguo.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yyd.mhx1999.top

[U49] PHP：只读属性
来源：http://smv.ivvv.top

public readonly string $name
来源：http://ezi.xingfuxueyuan.xyz

[U50] PHP：构造器属性提升
来源：http://ghc.redwolf501.top

public function __construct(private int $id) {}
来源：http://hph.redwolf501.top

[U51] PHP：数组解构
来源：http://jbi.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://bpp.zdbjq.cn

[U52] PHP：箭头函数
来源：http://xju.fzhhl.top

$double = fn($x) => $x * 2;
来源：http://ort.jqgfzy.top

[U53] PHP：空合并运算符
来源：http://yxy.epnwcf.com

$v = $a ?? $b ?? "default";
来源：http://xrn.cheryme.top

[U54] PHP：空安全调用
来源：http://quc.cashguo.top

$obj?->method()
来源：http://wqn.yanxiufei.cn

[U55] PHP：match 表达式
来源：http://gyq.aibaodan.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://orb.fehbvm.com

[U56] PHP：命名参数
来源：http://gqk.zhijiandao.cn

f(a: 1, b: 2)
来源：http://cab.yueranfly.top

[U57] PHP：字符串插值
来源：http://dbu.gotoacloud.top

"值: {$a}"
来源：http://msl.jqgufenzy.top

[U58] PHP：数组三件套
来源：http://mdw.zycfv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mua.yj20258.top

[U59] PHP：自定义排序
来源：http://pjy.sweek.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xmm.yonumen.top

[U60] PHP：JSON 编解码
来源：http://duv.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zan.chenjidiqi.icu

[U61] PHP：正则
来源：http://ktx.chenzaomai.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ckt.xylfe.cn

[U62] PHP：日期对象
来源：http://igd.fehbvm.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ohu.shanyushiyangkeji.top

[U63] PHP：文件读写
来源：http://drf.yj20258.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://byv.aizwys.cn

[U64] PHP：目录遍历
来源：http://bfj.jinqigufen.top

glob("dir/*.php");  scandir("dir");
来源：http://lfu.aizwys.cn

[U65] PHP：会话
来源：http://phg.yueranfly.top

session_start();  $_SESSION["uid"] = 1;
来源：http://cva.aibaodan.cn

[U66] PHP：设置 Cookie
来源：http://uwp.shuidangran.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bpt.jianghu66.top

[U67] PHP：处理文件上传
来源：http://zsm.dianchejie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gvh.sufxvd.cn

[U68] PHP：PDO 连接
来源：http://vzy.sxryk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xbf.shangyingyoupin.top

[U69] PHP：PDO 预处理
来源：http://npz.daria6918.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fdn.pycfn.com

[U70] PHP：PDO 事务
来源：http://bcz.shuidangran.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jdi.fktsv.cn

[U71] PHP：抛出异常
来源：http://hxk.shanyushiyangtech.top

throw new RuntimeException("失败", 500);
来源：http://ztk.jqgfzy.top

[U72] PHP：写错误日志
来源：http://dws.xylfe.cn

error_log("失败: " . $e->getMessage());
来源：http://lfx.xinyue.icu

[U73] PHP：读取 ini 配置
来源：http://jik.jlsjyb.cn

parse_ini_file("config.ini", true)
来源：http://ifq.havefunace.top

[U74] PHP：读取环境变量
来源：http://cah.nanxinkj.top

getenv("APP_ENV") ?: "production"
来源：http://bdw.yonumen.top

[U75] PHP：依赖注入
来源：http://pet.hammf.cn

composer require psr/container
来源：http://hja.quarkkingdee.top

[U76] PHP：简单路由
来源：http://ufo.jqgufenzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zkx.yj202588.top

[U77] PHP：模板渲染
来源：http://flo.52xcode.cn

composer require twig/twig
来源：http://wwr.hnxiangtu.top

[U78] PHP：单元测试
来源：http://opo.havefunace.top

composer require --dev phpunit/phpunit
来源：http://txq.shanyushiyangkeji.top

[U79] PHP：静态分析
来源：http://yaz.sysykeji.top

composer require --dev phpstan/phpstan
来源：http://yfs.zhijiandao.cn

[U80] PHP：代码规范修复
来源：http://jta.sxryk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bgv.shangyingyoupin.top

[U81] JS：初始化项目
来源：http://jde.hnxiangtu.top

npm init -y;  npm i express
来源：http://znv.nanxuanxn.top

[U82] JS：package.json 脚本
来源：http://zvq.ydzc1.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ger.zhixingplan.top

[U83] JS：ES Module 导入导出
来源：http://vde.fehbvm.com

export const a = 1;  import { a } from "./m.js";
来源：http://xcb.316326.xyz

[U84] JS：CommonJS 写法
来源：http://wsw.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ggz.yueranfly.top

[U85] JS：可选链
来源：http://ild.xinyue.icu

a?.b?.c
来源：http://bjq.smart0.xyz

[U86] JS：空值合并
来源：http://iiz.xuetiantiany.cn

a ?? b
来源：http://pte.feifeiyinyue.top

[U87] JS：解构默认值
来源：http://qkj.xuanzx.com

const { a = 1, b = 2 } = obj;
来源：http://zqp.fktsv.cn

[U88] JS：对象展开合并
来源：http://otm.fengsongda.top

{ ...a, ...b }
来源：http://zwo.hnqzz.top

[U89] JS：数组去重
来源：http://rgm.hnqzz.top

[...new Set(arr)]
来源：http://rdp.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://bkp.cqqwz.cn

[...arr].sort((a, b) => a - b)
来源：http://njd.ehwqpu.com

[U91] JS：对象键值遍历
来源：http://wkw.yj20258.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://daq.yj20258.top

[U92] JS：深拷贝
来源：http://rry.zhoulong.xyz

structuredClone(obj)
来源：http://fgx.ctjpmb.com

[U93] JS：模板字符串
来源：http://oqt.jinghuilouyu.cn

`共 ${n} 条`
来源：http://dsr.xinyue.icu

[U94] JS：箭头函数
来源：http://kyq.andypj.xyz

const double = x => x * 2;
来源：http://ckg.ctjpmb.com

[U95] JS：Promise 包装
来源：http://hti.gaohongyu789.top

new Promise((resolve, reject) => {})
来源：http://lzn.jinyuanbaomall.cn

[U96] JS：async/await 与异常
来源：http://rja.chenjidiqi.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kyw.zdqjudy.top

[U97] JS：并发请求
来源：http://zcn.dashuyun.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rjl.sjlbkw.cn

[U98] JS：fetch 带 JSON
来源：http://chl.ybcxt.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bxz.hongshengwenyu.top

[U99] JS：事件监听
来源：http://san.ywan-chungtsiang.top

el.addEventListener("click", e => {})
来源：http://kav.xylfe.cn

[U100] JS：DOM 查询
来源：http://gzx.yangfankeji.com

document.querySelector(".item")
来源：http://aiw.hongshengwenyu.top

[U101] JS：classList 操作
来源：http://kqr.ivvv.top

el.classList.toggle("active")
来源：http://pxz.cheryme.top

[U102] JS：本地存储
来源：http://lrl.fzhhl.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rox.chenjidiqi.icu

[U103] JS：定时器
来源：http://bau.bbcook.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yda.yanxiufei.cn

[U104] JS：防抖
来源：http://zgz.daxiang520.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yac.wangdashe.top

[U105] JS：节流
来源：http://qln.tianlin.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vtd.andypj.xyz

[U106] JS：日期格式化
来源：http://rpk.xingfuxueyuan.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tig.ydzc1.top

[U107] JS：数字千分位
来源：http://mln.pycfn.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vhf.zdbjq.cn

[U108] JS：随机整数
来源：http://lmq.meibo888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vnr.vqdsnc.cn

[U109] JS：数组分组
来源：http://aac.fehbvm.com

Object.groupBy(arr, x => x.type)
来源：http://hvi.ctjpmb.com

[U110] JS：数组分块
来源：http://zqn.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vhg.ydzc1.top

[U111] JS：对象转 Map
来源：http://jml.zhengqikj.top

new Map(Object.entries(obj))
来源：http://jug.kuanghao11.cn

[U112] JS：字符串补位
来源：http://tgf.hysaishi.cn

"7".padStart(3, "0")
来源：http://uvf.hesvh.cn

[U113] JS：正则替换全部
来源：http://pai.52xcode.cn

s.replaceAll("a", "b")
来源：http://uko.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://kwx.yangfankeji.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://vif.ywan-chungtsiang.top

[U115] JS：生成 UUID
来源：http://tar.cucudq.cn

crypto.randomUUID()
来源：http://epc.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://sen.xingfuxueyuan.xyz

/** @param {string} name */ function f(name) {}
来源：http://rxw.ybcxt.top

[U117] JS：单元测试
来源：http://kig.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://xme.cqqwz.cn

[U118] JS：开发服务器
来源：http://khe.jianghu66.top

npm i -D vite;  npx vite
来源：http://zxd.yj20258.top

[U119] JS：生产构建
来源：http://sty.fzhhl.top

npx vite build
来源：http://urc.yongpay.top

[U120] JS：读取环境变量（Vite）
来源：http://jhd.sysykeji.top

import.meta.env.VITE_API_URL
来源：http://buu.aizwys.cn

================================================================================
来源：http://yle.shanyushiyangtech.top

统计汇总
来源：http://coa.zhiwuduotai.top

================================================================================
来源：http://omu.aibaodan.cn

按语言统计（条）：
来源：http://eav.zdbjq.cn

Python ......... 252
来源：http://ulz.shanyushiyangtech.top

PHP ............ 252
来源：http://hhn.9152youxi.cn

JavaScript ..... 252
来源：http://nur.jlsjyb.cn

TypeScript ..... 212
来源：http://xfk.ppjwa.cn

Java ........... 212
来源：http://gtl.hongshengwenyu.top

Go ............. 212
来源：http://pyu.uphjek.com

Ruby ........... 212
来源：http://erd.ybcxt.top

C# ............. 212
来源：http://qnp.9152youxi.cn

C .............. 30
来源：http://zge.gaohongyu789.top

C++ ............ 30
来源：http://ibw.jlsjyb.cn

SQL ............ 90
来源：http://trk.dianchejie.cn

Bash ........... 80
来源：http://kkh.ppjwa.cn

Kotlin ......... 15
来源：http://nnt.jqgfzy.top

Swift .......... 15
来源：http://udg.9152youxi.cn

Lua ............ 10
来源：http://chj.guannengcc.top

Perl ........... 10
来源：http://nqz.yueranfly.top

Scala .......... 10
来源：http://nqb.fktsv.cn

------------------------------------
来源：http://had.nanxuanxn.top

合计 ........... 2106 条
来源：http://nja.gaohongyu789.top

按章节统计：
来源：http://iez.wangshuangyany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ces.xziqi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nsp.zhengqikj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yxr.jinqigfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zrc.c1oappe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mvy.jqgfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ohj.zhoulong.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xqf.0kj1m.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bix.smart0.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xxj.tianlin.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lzk.nwbrower.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zap.nanxinkj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xkb.fanxiaobao.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dfw.fktsv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cka.ybcxt.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yzb.yfazqb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rhj.yuxming.cn

Q SQL 专题                              90
来源：http://usi.0kj1m.cn

R Bash 专题                             80
来源：http://wln.shangyingyoupin.top

S C / C++ 专题                          60
来源：http://zcm.xuanzx.com

T 其他语言补充                          60
来源：http://cpd.cheryme.top

U 高频实用片段                         120
来源：http://tpj.yuanzhike.top

------------------------------------
来源：http://aeq.ehwqpu.com

合计                                  2106 条
来源：http://ihu.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://zsw.sysykeji.top

使用提醒
来源：http://yhj.yonumen.top

--------------------------------------------------------------------------------
来源：http://sea.sjlbkw.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tqe.tanke756.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bhq.mhx1999.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://anx.cheryme.top

在旧版本上使用前请先确认语法支持情况。
来源：http://eop.sysykeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ioa.gotoacloud.top

—— 文件结束 ——
来源：http://uie.xinyue.icu

================================================================================
来源：http://lja.xziqi.cn

程序语言常见例子速查手册（2024 版）
来源：http://qhc.cheryme.top

Common Programming Examples Cheat Book
来源：http://ndp.ybcxt.top

================================================================================
来源：http://kba.0kj1m.cn

【收录内容】
来源：http://rir.chenzaomai.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://mha.aibaodan.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jew.zdbjq.cn

SQL · Bash · C · C++
来源：http://bmb.xylfe.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://let.sysykeji.top

【使用说明】
来源：http://udv.cqqwz.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qxt.hnqzz.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xrt.vehdjk.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fix.yueranfly.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ofz.chenzaomai.com

Bash:  Shell         C:     C             C++:   C++
来源：http://zrt.haohaochexian.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://exi.xuetiantiany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://svu.smart0.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ffm.epnwcf.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lrr.jinyuanbaomall.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dym.yfazqb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zzb.yuxming.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tfz.nanxuanxn.top

【文件统计】
来源：http://npa.hysaishi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nud.hcnkem.com

--------------------------------------------------------------------------------
来源：http://vhv.tian-w.cn

目  录
来源：http://gvt.iojbl.cn

--------------------------------------------------------------------------------
来源：http://glr.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hds.daxiang520.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kto.fehbvm.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hln.ehwqpu.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qcg.zdbjq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xuc.guannengcc.top


<!-- 参考信息 -->