代发 wailian999

[U09] Py：字典取最大值的键
来源：http://sxp.yuxming.cn

max(d, key=d.get)
来源：http://kro.shuidangran.top

[U10] Py：按值排序字典
来源：http://bmi.hfpthk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zrw.snrcjt.cn

[U11] Py：生成器表达式
来源：http://hkq.fengsongda.top

(x * 2 for x in arr)
来源：http://qmp.andypj.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://dij.sysykeji.top

Counter(arr).most_common(3)
来源：http://blo.chenzaomai.com

[U13] Py：固定长度队列
来源：http://piq.hammf.cn

deque(maxlen=10)
来源：http://ony.guannengcc.top

[U14] Py：分组收集到列表
来源：http://wet.andypj.xyz

defaultdict(list)
来源：http://waz.shangyingyoupin.top

[U15] Py：高精度计时
来源：http://ila.jinqigufen.top

t = time.perf_counter()
来源：http://mfy.dashuyun.cn

[U16] Py：命令行参数解析
来源：http://mby.meibo888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ins.yueranfly.top

[U17] Py：初始化日志
来源：http://zfz.shangyingyoupin.top

logging.basicConfig(level=logging.INFO)
来源：http://fab.wangdashe.top

[U18] Py：预编译正则
来源：http://mrv.gotoacloud.top

pat = re.compile(r"\d+")
来源：http://ofu.gaohongyu789.top

[U19] Py：正则替换带回调
来源：http://zzr.shangyingyoupin.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lvl.vehdjk.com

[U20] Py：缓存函数结果
来源：http://vlp.wangshuangyany.cn

@functools.lru_cache(maxsize=None)
来源：http://yck.ydjk.org.cn

[U21] Py：自定义上下文管理器
来源：http://laq.yuxming.cn

@contextlib.contextmanager
来源：http://usb.ehwqpu.com

[U22] Py：矩阵转置
来源：http://chi.zhiwuduotai.top

list(zip(*m))
来源：http://shn.zhongyouzk.top

[U23] Py：分块读取大文件
来源：http://udq.sxryk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kzn.fanxiaobao.xyz

[U24] Py：路径操作
来源：http://nrz.redwolf501.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mfn.xuetiantiany.cn

[U25] Py：CSV 按字典读
来源：http://viu.yfazqb.com

csv.DictReader(f)
来源：http://kac.ybcxt.top

[U26] Py：并发下载
来源：http://qlh.haohaochexian.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ewb.pycfn.com

[U27] Py：异步 HTTP
来源：http://gsf.dianchejie.cn

aiohttp.ClientSession() 配合 async with
来源：http://xmz.zhixingplan.top

[U28] Py：类型别名
来源：http://nuw.xziqi.cn

UserId = int
来源：http://rji.xuanzx.com

[U29] Py：属性校验
来源：http://bjx.zhoulong.xyz

@property 与 @x.setter 配合
来源：http://iff.zhongyouzk.top

[U30] Py：数据类
来源：http://qjc.xuanzx.com

@dataclass(slots=True)
来源：http://faj.andypj.xyz

[U31] Py：单测
来源：http://coi.jianghu66.top

python -m pytest -q
来源：http://mug.pengpengdd.cyou

[U32] Py：代码格式化
来源：http://fyj.zhengqikj.top

ruff format . && ruff check --fix .
来源：http://lnf.sufxvd.cn

[U33] Py：打包发布
来源：http://htm.pengpengdd.cyou

python -m build  （依赖 pyproject.toml）
来源：http://guf.316326.xyz

[U34] Py：判断编码
来源：http://plk.haohaochexian.top

chardet.detect(raw)
来源：http://rui.jinqigufen.top

[U35] Py：发送邮件
来源：http://qby.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qyh.shanyushiyangtech.top

[U36] Py：定时任务
来源：http://ckc.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://sdf.yuxming.cn

[U37] Py：读写 Excel
来源：http://pvh.tian-w.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qds.yonumen.top

[U38] Py：获取脚本所在目录
来源：http://ztj.meibo888.top

Path(__file__).resolve().parent
来源：http://tyy.xuetiantiany.cn

[U39] Py：判断是否在交互环境
来源：http://odg.kuanghao11.cn

sys.stdout.isatty()
来源：http://vsw.gogol.net.cn

[U40] Py：打印到标准错误
来源：http://sjp.chenzaomai.com

print("err", file=sys.stderr)
来源：http://pua.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://xwq.hywenlv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cvg.xingfuxueyuan.xyz

[U42] PHP：PSR-4 自动加载
来源：http://kqz.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jyp.daria6918.cn

[U43] PHP：声明命名空间
来源：http://zfi.yangfankeji.com

namespace App\Http;
来源：http://uxh.yonumen.top

[U44] PHP：开启严格类型
来源：http://zsf.xinyue.icu

declare(strict_types=1);
来源：http://zwt.xuetiantiany.cn

[U45] PHP：类型声明与返回类型
来源：http://vkr.ppjwa.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ixp.chenlongwang.top

[U46] PHP：可空类型
来源：http://wlb.iojbl.cn

?string $name = null
来源：http://uvs.cucudq.cn

[U47] PHP：联合类型
来源：http://bak.yonumen.top

int|string $id
来源：http://swj.daria6918.cn

[U48] PHP：纯枚举
来源：http://nxz.gogol.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lxj.jyoumei.cn

[U49] PHP：只读属性
来源：http://ovg.zhixingplan.top

public readonly string $name
来源：http://wax.cheryme.top

[U50] PHP：构造器属性提升
来源：http://sea.jiagoushi.top

public function __construct(private int $id) {}
来源：http://bww.hywenlv.cn

[U51] PHP：数组解构
来源：http://wni.zhongyouzk.top

[$a, $b] = $arr;
来源：http://skd.sweek.top

[U52] PHP：箭头函数
来源：http://eqk.feifeiyinyue.top

$double = fn($x) => $x * 2;
来源：http://tto.gzhubu.top

[U53] PHP：空合并运算符
来源：http://onq.cqqwz.cn

$v = $a ?? $b ?? "default";
来源：http://lwb.hywenlv.cn

[U54] PHP：空安全调用
来源：http://cel.jlsjyb.cn

$obj?->method()
来源：http://ntw.pycfn.com

[U55] PHP：match 表达式
来源：http://ogk.yonumen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://erm.xinyue.icu

[U56] PHP：命名参数
来源：http://xro.ctjpmb.com

f(a: 1, b: 2)
来源：http://fpn.zhijiandao.cn

[U57] PHP：字符串插值
来源：http://wcd.cdnleiting.top

"值: {$a}"
来源：http://kqq.jyoumei.cn

[U58] PHP：数组三件套
来源：http://oya.hfpthk.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ffr.jinqigufen.top

[U59] PHP：自定义排序
来源：http://gkf.shanyushiyangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zkp.wangdashe.top

[U60] PHP：JSON 编解码
来源：http://wcg.yuxming.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tdu.ybcxt.top

[U61] PHP：正则
来源：http://gax.aibaodan.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mnt.52xcode.cn

[U62] PHP：日期对象
来源：http://xkg.yanxiufei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uej.yj20258888.top

[U63] PHP：文件读写
来源：http://aid.gotoacloud.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wuc.feifeiyinyue.top

[U64] PHP：目录遍历
来源：http://aer.zhiwuduotai.top

glob("dir/*.php");  scandir("dir");
来源：http://ibr.gaohongyu789.top

[U65] PHP：会话
来源：http://hao.shanyushiyangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gqg.zdbjq.cn

[U66] PHP：设置 Cookie
来源：http://twq.bbcook.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ylv.yongpay.top

[U67] PHP：处理文件上传
来源：http://ykb.quarkkingdee.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oeb.ivvv.top

[U68] PHP：PDO 连接
来源：http://yis.wangdashe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://egk.dianchejie.cn

[U69] PHP：PDO 预处理
来源：http://vzd.iojbl.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ule.yuanzhike.top

[U70] PHP：PDO 事务
来源：http://rlg.pycfn.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://noq.vehdjk.com

[U71] PHP：抛出异常
来源：http://tlu.c1oappe.top

throw new RuntimeException("失败", 500);
来源：http://hnn.pycfn.com

[U72] PHP：写错误日志
来源：http://wqr.jlsjyb.cn

error_log("失败: " . $e->getMessage());
来源：http://oou.mhx1999.top

[U73] PHP：读取 ini 配置
来源：http://jwq.xziqi.cn

parse_ini_file("config.ini", true)
来源：http://ajp.uphjek.com

[U74] PHP：读取环境变量
来源：http://iey.yangfankeji.com

getenv("APP_ENV") ?: "production"
来源：http://jcp.cqqwz.cn

[U75] PHP：依赖注入
来源：http://act.ydjk.org.cn

composer require psr/container
来源：http://dvx.ehwqpu.com

[U76] PHP：简单路由
来源：http://ari.yonumen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kzz.havefunace.top

[U77] PHP：模板渲染
来源：http://hdy.ybcxt.top

composer require twig/twig
来源：http://aki.shuidangran.top

[U78] PHP：单元测试
来源：http://lwn.hcnkem.com

composer require --dev phpunit/phpunit
来源：http://jrd.ywan-chungtsiang.top

[U79] PHP：静态分析
来源：http://khk.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://rok.aibaodan.cn

[U80] PHP：代码规范修复
来源：http://bhp.ppjwa.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fim.chenzaomai.com

[U81] JS：初始化项目
来源：http://ehg.c1oappe.top

npm init -y;  npm i express
来源：http://ibr.sysykeji.top

[U82] JS：package.json 脚本
来源：http://lgt.zhoulong.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fqd.zhixingplan.top

[U83] JS：ES Module 导入导出
来源：http://pwz.snrcjt.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xji.hnqzz.top

[U84] JS：CommonJS 写法
来源：http://glq.andypj.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://gvm.iojbl.cn

[U85] JS：可选链
来源：http://eyk.c1oappe.top

a?.b?.c
来源：http://taw.hfpthk.cn

[U86] JS：空值合并
来源：http://moc.tanke756.top

a ?? b
来源：http://mma.zdbjq.cn

[U87] JS：解构默认值
来源：http://lfu.sxryk.cn

const { a = 1, b = 2 } = obj;
来源：http://zml.feifeiyinyue.top

[U88] JS：对象展开合并
来源：http://wlq.gogol.net.cn

{ ...a, ...b }
来源：http://joe.sysykeji.top

[U89] JS：数组去重
来源：http://loq.jinqigfzy.top

[...new Set(arr)]
来源：http://svg.xinyue.icu

[U90] JS：数字数组排序
来源：http://chc.sxryk.cn

[...arr].sort((a, b) => a - b)
来源：http://bvu.ywan-chungtsiang.top

[U91] JS：对象键值遍历
来源：http://toc.jyoumei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gsg.yanxiufei.cn

[U92] JS：深拷贝
来源：http://nrk.zhongyouzk.top

structuredClone(obj)
来源：http://zye.jqgfzy.top

[U93] JS：模板字符串
来源：http://bzk.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://zrj.hfpthk.cn

[U94] JS：箭头函数
来源：http://fez.jinqigfzy.top

const double = x => x * 2;
来源：http://gup.xuanzx.com

[U95] JS：Promise 包装
来源：http://omr.fengsongda.top

new Promise((resolve, reject) => {})
来源：http://qyc.shuidangran.top

[U96] JS：async/await 与异常
来源：http://boj.yuanzhike.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eec.daria6918.cn

[U97] JS：并发请求
来源：http://vqk.ppjwa.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ebi.jqgfzy.top

[U98] JS：fetch 带 JSON
来源：http://ogw.svipenyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://aea.smart0.xyz

[U99] JS：事件监听
来源：http://nne.zycfv.cn

el.addEventListener("click", e => {})
来源：http://gdl.yj20258888.top

[U100] JS：DOM 查询
来源：http://ifu.yuanzhike.top

document.querySelector(".item")
来源：http://nkj.nwbrower.top

[U101] JS：classList 操作
来源：http://wkn.c1oappe.top

el.classList.toggle("active")
来源：http://qii.ppjwa.cn

[U102] JS：本地存储
来源：http://qsq.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://irw.shanyushiyangtech.top

[U103] JS：定时器
来源：http://qkh.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vqr.birdmap.top

[U104] JS：防抖
来源：http://iia.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tnm.jinyuanbaomall.cn

[U105] JS：节流
来源：http://rmh.fktsv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yrw.chenzaomai.com

[U106] JS：日期格式化
来源：http://vhp.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zbg.sufxvd.cn

[U107] JS：数字千分位
来源：http://mez.ydzc1.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://utl.jinyuanbaomall.cn

[U108] JS：随机整数
来源：http://bfr.shanyushiyangtech.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://auh.aizwys.cn

[U109] JS：数组分组
来源：http://pyk.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://jfg.yueranfly.top

[U110] JS：数组分块
来源：http://pyx.zycfv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://atu.yfazqb.com

[U111] JS：对象转 Map
来源：http://owu.ppjwa.cn

new Map(Object.entries(obj))
来源：http://prm.hysaishi.cn

[U112] JS：字符串补位
来源：http://xcv.xylfe.cn

"7".padStart(3, "0")
来源：http://lab.xuetiantiany.cn

[U113] JS：正则替换全部
来源：http://vek.smart0.xyz

s.replaceAll("a", "b")
来源：http://nvc.iojbl.cn

[U114] JS：JSON 深比较
来源：http://ulo.haohaochexian.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fqt.316326.xyz

[U115] JS：生成 UUID
来源：http://cxq.tian-w.cn

crypto.randomUUID()
来源：http://phr.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://omj.cheryme.top

/** @param {string} name */ function f(name) {}
来源：http://zyu.cdnleiting.top

[U117] JS：单元测试
来源：http://jhr.zhongyouzk.top

npm i -D vitest;  npx vitest
来源：http://qye.shangyingyoupin.top

[U118] JS：开发服务器
来源：http://vma.shanyushiyangtech.top

npm i -D vite;  npx vite
来源：http://kol.svipenyu.cn

[U119] JS：生产构建
来源：http://gdj.quarkkingdee.top

npx vite build
来源：http://tsw.hnqzz.top

[U120] JS：读取环境变量（Vite）
来源：http://ymy.daxiang520.top

import.meta.env.VITE_API_URL
来源：http://rmm.sjlbkw.cn

================================================================================
来源：http://tfp.hfpthk.cn

统计汇总
来源：http://kfs.shanyushiyangtech.top

================================================================================
来源：http://cfi.mhx1999.top

按语言统计（条）：
来源：http://git.kuanghao11.cn

Python ......... 252
来源：http://zhn.vehdjk.com

PHP ............ 252
来源：http://xnd.mhx1999.top

JavaScript ..... 252
来源：http://uzc.0kj1m.cn

TypeScript ..... 212
来源：http://tmy.iojbl.cn

Java ........... 212
来源：http://ipm.pengpengdd.cyou

Go ............. 212
来源：http://mqn.jqgufenzy.top

Ruby ........... 212
来源：http://fkp.xziqi.cn

C# ............. 212
来源：http://wrd.yj20258.top

C .............. 30
来源：http://pzq.yj202588.top

C++ ............ 30
来源：http://axj.uphjek.com

SQL ............ 90
来源：http://xtg.shzxlz.cn

Bash ........... 80
来源：http://plh.vqdsnc.cn

Kotlin ......... 15
来源：http://cow.fehbvm.com

Swift .......... 15
来源：http://mdq.meibo888.top

Lua ............ 10
来源：http://itm.jqgfzy.top

Perl ........... 10
来源：http://ezg.guowangkeji.top

Scala .......... 10
来源：http://fld.nanxinkj.top

------------------------------------
来源：http://reh.nwbrower.top

合计 ........... 2106 条
来源：http://kfc.ydzc1.top

按章节统计：
来源：http://the.fengsongda.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qhs.sweek.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jli.xziqi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lbw.yj20258888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kzz.shangyingyoupin.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://prp.yfazqb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lhe.dianchejie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yjp.sufxvd.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://osk.fengsongda.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://riu.xuetiantiany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hba.jinyuanbaomall.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lca.xuanzx.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uqt.nanxuanxn.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kyw.jianghu66.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lzh.316326.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iyo.fehbvm.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kib.shzxlz.cn

Q SQL 专题                              90
来源：http://ucz.bbcook.cn

R Bash 专题                             80
来源：http://wps.bjfxy.top

S C / C++ 专题                          60
来源：http://eui.yongpay.top

T 其他语言补充                          60
来源：http://dhq.fzhhl.top

U 高频实用片段                         120
来源：http://vdg.yanxiufei.cn

------------------------------------
来源：http://mev.pengpengdd.cyou

合计                                  2106 条
来源：http://bxn.yuxming.cn

--------------------------------------------------------------------------------
来源：http://jjh.shangyingyoupin.top

使用提醒
来源：http://bhn.aizwys.cn

--------------------------------------------------------------------------------
来源：http://qyf.hammf.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kqu.zhixingplan.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ndn.ywan-chungtsiang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zqf.nanxuanxn.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fsn.gaohongyu789.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wpo.fanxiaobao.xyz

—— 文件结束 ——
来源：http://aau.birdmap.top

================================================================================
来源：http://eho.xinyue.icu

程序语言常见例子速查手册（2024 版）
来源：http://lcp.zhongyouzk.top

Common Programming Examples Cheat Book
来源：http://cfp.fengsongda.top

================================================================================
来源：http://pfz.yuxming.cn

【收录内容】
来源：http://nvp.dashuyun.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mto.52xcode.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xcz.snrcjt.cn

SQL · Bash · C · C++
来源：http://akk.vqdsnc.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nad.yangfankeji.com

【使用说明】
来源：http://uhs.guowangkeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://euj.zhaomingkeji.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gnh.aizwys.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mhe.xziqi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wcf.zhaomingkeji.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://kwz.ppjwa.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pky.zhoulong.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nde.fktsv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kix.sufxvd.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xyr.shuidangran.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sun.ybcxt.top


<!-- 参考信息 -->