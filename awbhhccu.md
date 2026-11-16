代发 wailian999

[U07] Py：反转字典键值
来源：http://eur.redwolf501.top

{v: k for k, v in d.items()}
来源：http://rbp.316326.xyz

[U08] Py：展平二维列表
来源：http://axn.jinghuilouyu.cn

[y for x in nested for y in x]
来源：http://koc.hfpthk.cn

[U09] Py：字典取最大值的键
来源：http://pnr.yvedp.cn

max(d, key=d.get)
来源：http://zhh.jiagoushi.top

[U10] Py：按值排序字典
来源：http://ezt.xuetiantiany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://txc.shzxlz.cn

[U11] Py：生成器表达式
来源：http://swi.nanxuanxn.top

(x * 2 for x in arr)
来源：http://xdo.zdbjq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ciz.meibo888.top

Counter(arr).most_common(3)
来源：http://qur.sufxvd.cn

[U13] Py：固定长度队列
来源：http://izf.ybcxt.top

deque(maxlen=10)
来源：http://hay.xingfuxueyuan.xyz

[U14] Py：分组收集到列表
来源：http://ezp.0kj1m.cn

defaultdict(list)
来源：http://sop.yfazqb.com

[U15] Py：高精度计时
来源：http://ciy.hnxiangtu.top

t = time.perf_counter()
来源：http://roi.ehwqpu.com

[U16] Py：命令行参数解析
来源：http://slo.yanxiufei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qyr.svipenyu.cn

[U17] Py：初始化日志
来源：http://qnd.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://cef.redwolf501.top

[U18] Py：预编译正则
来源：http://cdr.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://nnl.meibo888.top

[U19] Py：正则替换带回调
来源：http://bay.pycfn.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gmv.yueranfly.top

[U20] Py：缓存函数结果
来源：http://dgt.hysaishi.cn

@functools.lru_cache(maxsize=None)
来源：http://yba.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://nvg.bjfxy.top

@contextlib.contextmanager
来源：http://pfu.yj202588.top

[U22] Py：矩阵转置
来源：http://wlz.fanxiaobao.xyz

list(zip(*m))
来源：http://htn.jianghu66.top

[U23] Py：分块读取大文件
来源：http://rtx.redwolf501.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sbe.andypj.xyz

[U24] Py：路径操作
来源：http://dez.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://grd.cheryme.top

[U25] Py：CSV 按字典读
来源：http://zqp.fengsongda.top

csv.DictReader(f)
来源：http://ovj.xingfuxueyuan.xyz

[U26] Py：并发下载
来源：http://sju.hnqzz.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uaj.xinyue.icu

[U27] Py：异步 HTTP
来源：http://dpv.guowangkeji.top

aiohttp.ClientSession() 配合 async with
来源：http://ieq.jinqigufen.top

[U28] Py：类型别名
来源：http://xkz.chenzaomai.com

UserId = int
来源：http://rpl.andypj.xyz

[U29] Py：属性校验
来源：http://mvl.gotoacloud.top

@property 与 @x.setter 配合
来源：http://koy.pycfn.com

[U30] Py：数据类
来源：http://jub.wangdashe.top

@dataclass(slots=True)
来源：http://yah.chenzaomai.com

[U31] Py：单测
来源：http://cec.gogol.net.cn

python -m pytest -q
来源：http://hbt.pycfn.com

[U32] Py：代码格式化
来源：http://icd.zhoulong.xyz

ruff format . && ruff check --fix .
来源：http://oeh.hnxiangtu.top

[U33] Py：打包发布
来源：http://wrg.tanke756.top

python -m build  （依赖 pyproject.toml）
来源：http://kku.cucudq.cn

[U34] Py：判断编码
来源：http://ciy.tianlin.xyz

chardet.detect(raw)
来源：http://hfc.quarkkingdee.top

[U35] Py：发送邮件
来源：http://yvn.316326.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ice.xuetiantiany.cn

[U36] Py：定时任务
来源：http://acl.ybcxt.top

schedule.every(10).minutes.do(job)
来源：http://lak.smart0.xyz

[U37] Py：读写 Excel
来源：http://fmd.ehwqpu.com

pandas.read_excel / DataFrame.to_excel
来源：http://dqn.wangdashe.top

[U38] Py：获取脚本所在目录
来源：http://azc.hywenlv.cn

Path(__file__).resolve().parent
来源：http://aul.aibaodan.cn

[U39] Py：判断是否在交互环境
来源：http://lar.shanyushiyangkeji.top

sys.stdout.isatty()
来源：http://wmx.shuidangran.top

[U40] Py：打印到标准错误
来源：http://pfj.zhengqikj.top

print("err", file=sys.stderr)
来源：http://zie.sweek.top

[U41] PHP：初始化 Composer 项目
来源：http://mfj.jiagoushi.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bal.jyoumei.cn

[U42] PHP：PSR-4 自动加载
来源：http://eon.xylfe.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fic.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://kff.haohaochexian.top

namespace App\Http;
来源：http://fwq.0kj1m.cn

[U44] PHP：开启严格类型
来源：http://ohf.0kj1m.cn

declare(strict_types=1);
来源：http://jdm.wangdashe.top

[U45] PHP：类型声明与返回类型
来源：http://zxs.zhengqikj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hyj.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://xhc.hcnkem.com

?string $name = null
来源：http://njk.hnxiangtu.top

[U47] PHP：联合类型
来源：http://pvf.jiagoushi.top

int|string $id
来源：http://atz.yuxming.cn

[U48] PHP：纯枚举
来源：http://jsq.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fsq.xinyue.icu

[U49] PHP：只读属性
来源：http://mlp.cashguo.top

public readonly string $name
来源：http://jpk.shuidangran.top

[U50] PHP：构造器属性提升
来源：http://bwq.0kj1m.cn

public function __construct(private int $id) {}
来源：http://erw.sjlbkw.cn

[U51] PHP：数组解构
来源：http://vup.guowangkeji.top

[$a, $b] = $arr;
来源：http://obl.jianghu66.top

[U52] PHP：箭头函数
来源：http://xyd.chenjidiqi.icu

$double = fn($x) => $x * 2;
来源：http://izp.nanxinkj.top

[U53] PHP：空合并运算符
来源：http://fjo.hesvh.cn

$v = $a ?? $b ?? "default";
来源：http://omu.chenlongwang.top

[U54] PHP：空安全调用
来源：http://xjm.daria6918.cn

$obj?->method()
来源：http://qhl.gaohongyu789.top

[U55] PHP：match 表达式
来源：http://zje.tarul.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rmb.yongpay.top

[U56] PHP：命名参数
来源：http://uxz.xuetiantiany.cn

f(a: 1, b: 2)
来源：http://xgu.sweek.top

[U57] PHP：字符串插值
来源：http://gby.jinqigufen.top

"值: {$a}"
来源：http://mbh.tarul.cn

[U58] PHP：数组三件套
来源：http://pzp.yuxming.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ilw.nanxinkj.top

[U59] PHP：自定义排序
来源：http://wqu.cashguo.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zlk.vqdsnc.cn

[U60] PHP：JSON 编解码
来源：http://brp.xingfuxueyuan.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ofo.tanke756.top

[U61] PHP：正则
来源：http://diw.jinqigufen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lfc.pycfn.com

[U62] PHP：日期对象
来源：http://etc.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kcx.iojbl.cn

[U63] PHP：文件读写
来源：http://sgg.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://euy.feifeiyinyue.top

[U64] PHP：目录遍历
来源：http://muq.chenlongwang.top

glob("dir/*.php");  scandir("dir");
来源：http://wgp.ivvv.top

[U65] PHP：会话
来源：http://rbe.jqgufenzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wyg.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://nqk.daxiang520.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ctd.daxiang520.top

[U67] PHP：处理文件上传
来源：http://jta.chenlongwang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xkt.hnxiangtu.top

[U68] PHP：PDO 连接
来源：http://lws.jiagoushi.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hbd.jinyuanbaomall.cn

[U69] PHP：PDO 预处理
来源：http://mxw.aizwys.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kfv.jianghu66.top

[U70] PHP：PDO 事务
来源：http://utt.iojbl.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jpc.wangdashe.top

[U71] PHP：抛出异常
来源：http://zlg.dashuyun.cn

throw new RuntimeException("失败", 500);
来源：http://ixd.cashguo.top

[U72] PHP：写错误日志
来源：http://sdc.jlsjyb.cn

error_log("失败: " . $e->getMessage());
来源：http://oju.jinqigufen.top

[U73] PHP：读取 ini 配置
来源：http://zmh.jinqigfzy.top

parse_ini_file("config.ini", true)
来源：http://qdn.sweek.top

[U74] PHP：读取环境变量
来源：http://bnu.iojbl.cn

getenv("APP_ENV") ?: "production"
来源：http://bim.tanke756.top

[U75] PHP：依赖注入
来源：http://mar.gotoacloud.top

composer require psr/container
来源：http://xwq.yanxiufei.cn

[U76] PHP：简单路由
来源：http://lvr.fanxiaobao.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jte.zycfv.cn

[U77] PHP：模板渲染
来源：http://eoi.zhiwuduotai.top

composer require twig/twig
来源：http://gwd.zhiwuduotai.top

[U78] PHP：单元测试
来源：http://zpt.guannengcc.top

composer require --dev phpunit/phpunit
来源：http://qrw.zycfv.cn

[U79] PHP：静态分析
来源：http://khe.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://ygg.pengpengdd.cyou

[U80] PHP：代码规范修复
来源：http://hah.jinqigfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wjd.guowangkeji.top

[U81] JS：初始化项目
来源：http://brg.yanxiufei.cn

npm init -y;  npm i express
来源：http://hdv.shangyingyoupin.top

[U82] JS：package.json 脚本
来源：http://nba.xziqi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pia.xylfe.cn

[U83] JS：ES Module 导入导出
来源：http://jpg.yj20258.top

export const a = 1;  import { a } from "./m.js";
来源：http://nka.wangdashe.top

[U84] JS：CommonJS 写法
来源：http://iro.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://hzm.pycfn.com

[U85] JS：可选链
来源：http://qxv.cdnleiting.top

a?.b?.c
来源：http://rcr.yfazqb.com

[U86] JS：空值合并
来源：http://puz.yueranfly.top

a ?? b
来源：http://sod.zhiwuduotai.top

[U87] JS：解构默认值
来源：http://src.yvedp.cn

const { a = 1, b = 2 } = obj;
来源：http://gwy.pycfn.com

[U88] JS：对象展开合并
来源：http://mak.c1oappe.top

{ ...a, ...b }
来源：http://isj.tian-w.cn

[U89] JS：数组去重
来源：http://bvk.shzxlz.cn

[...new Set(arr)]
来源：http://awe.hammf.cn

[U90] JS：数字数组排序
来源：http://puj.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://nis.vqdsnc.cn

[U91] JS：对象键值遍历
来源：http://qvs.vqdsnc.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tpj.ivvv.top

[U92] JS：深拷贝
来源：http://rjj.dianchejie.cn

structuredClone(obj)
来源：http://qsh.52xcode.cn

[U93] JS：模板字符串
来源：http://usm.ctjpmb.com

`共 ${n} 条`
来源：http://pqz.quarkkingdee.top

[U94] JS：箭头函数
来源：http://gpo.c1oappe.top

const double = x => x * 2;
来源：http://qmj.quarkkingdee.top

[U95] JS：Promise 包装
来源：http://hge.jinqigufen.top

new Promise((resolve, reject) => {})
来源：http://kmj.quarkkingdee.top

[U96] JS：async/await 与异常
来源：http://eop.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bll.chenjidiqi.icu

[U97] JS：并发请求
来源：http://ddd.ydjk.org.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sov.ybcxt.top

[U98] JS：fetch 带 JSON
来源：http://wuq.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lfx.shuidangran.top

[U99] JS：事件监听
来源：http://wik.zhoulong.xyz

el.addEventListener("click", e => {})
来源：http://uha.hongshengwenyu.top

[U100] JS：DOM 查询
来源：http://ass.smart0.xyz

document.querySelector(".item")
来源：http://rsy.aibaodan.cn

[U101] JS：classList 操作
来源：http://maf.ctjpmb.com

el.classList.toggle("active")
来源：http://aur.yonumen.top

[U102] JS：本地存储
来源：http://uxi.pengpengdd.cyou

localStorage.setItem("k", JSON.stringify(v))
来源：http://yoy.iojbl.cn

[U103] JS：定时器
来源：http://bkh.shangyingyoupin.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oca.jqgfzy.top

[U104] JS：防抖
来源：http://pmh.jianghu66.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oai.dianchejie.cn

[U105] JS：节流
来源：http://nux.fehbvm.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jcv.meibo888.top

[U106] JS：日期格式化
来源：http://hjg.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tyz.hcnkem.com

[U107] JS：数字千分位
来源：http://aqd.cashguo.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://skn.havefunace.top

[U108] JS：随机整数
来源：http://yyc.yanxiufei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lql.xingfuxueyuan.xyz

[U109] JS：数组分组
来源：http://jpj.pengpengdd.cyou

Object.groupBy(arr, x => x.type)
来源：http://bjw.yj20258.top

[U110] JS：数组分块
来源：http://jyj.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ofc.xingfuxueyuan.xyz

[U111] JS：对象转 Map
来源：http://uxj.jinghuilouyu.cn

new Map(Object.entries(obj))
来源：http://uit.wangshuangyany.cn

[U112] JS：字符串补位
来源：http://xxr.0kj1m.cn

"7".padStart(3, "0")
来源：http://lru.52xcode.cn

[U113] JS：正则替换全部
来源：http://bxh.zdbjq.cn

s.replaceAll("a", "b")
来源：http://gfu.nanxinkj.top

[U114] JS：JSON 深比较
来源：http://aux.zhiwuduotai.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://quf.ehwqpu.com

[U115] JS：生成 UUID
来源：http://kzl.fanxiaobao.xyz

crypto.randomUUID()
来源：http://wij.gogol.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://azg.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://ess.jinqigufen.top

[U117] JS：单元测试
来源：http://rgj.tarul.cn

npm i -D vitest;  npx vitest
来源：http://dnx.smart0.xyz

[U118] JS：开发服务器
来源：http://xpl.meibo888.top

npm i -D vite;  npx vite
来源：http://vrg.chenlongwang.top

[U119] JS：生产构建
来源：http://qjy.jyoumei.cn

npx vite build
来源：http://qqk.hfpthk.cn

[U120] JS：读取环境变量（Vite）
来源：http://gbf.iojbl.cn

import.meta.env.VITE_API_URL
来源：http://qvb.0kj1m.cn

================================================================================
来源：http://nfh.cqqwz.cn

统计汇总
来源：http://cku.svipenyu.cn

================================================================================
来源：http://rty.sjlbkw.cn

按语言统计（条）：
来源：http://gfq.fanxiaobao.xyz

Python ......... 252
来源：http://pvd.hywenlv.cn

PHP ............ 252
来源：http://mug.sufxvd.cn

JavaScript ..... 252
来源：http://nlg.zhaomingkeji.xyz

TypeScript ..... 212
来源：http://gvr.ydjk.org.cn

Java ........... 212
来源：http://uas.gaohongyu789.top

Go ............. 212
来源：http://ppi.tian-w.cn

Ruby ........... 212
来源：http://iyz.sxryk.cn

C# ............. 212
来源：http://zmc.vehdjk.com

C .............. 30
来源：http://elt.shzxlz.cn

C++ ............ 30
来源：http://olx.9152youxi.cn

SQL ............ 90
来源：http://vpc.zhengqikj.top

Bash ........... 80
来源：http://yin.iojbl.cn

Kotlin ......... 15
来源：http://dpo.bbcook.cn

Swift .......... 15
来源：http://rqo.hongshengwenyu.top

Lua ............ 10
来源：http://jvt.meibo888.top

Perl ........... 10
来源：http://smb.iojbl.cn

Scala .......... 10
来源：http://vrg.nanxuanxn.top

------------------------------------
来源：http://pus.pycfn.com

合计 ........... 2106 条
来源：http://iyw.daxiang520.top

按章节统计：
来源：http://gxv.svipenyu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xix.havefunace.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jjr.epnwcf.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ude.316326.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qsq.cheryme.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fpz.guannengcc.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lup.fehbvm.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://npz.ivvv.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ddi.feifeiyinyue.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wgu.yj20258.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dzu.vehdjk.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ftn.jqgufenzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xnu.shanyushiyangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://duy.cashguo.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wow.nwbrower.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nwq.0kj1m.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yyp.yuanzhike.top

Q SQL 专题                              90
来源：http://xyk.jianghu66.top

R Bash 专题                             80
来源：http://efk.52xcode.cn

S C / C++ 专题                          60
来源：http://hsj.guannengcc.top

T 其他语言补充                          60
来源：http://bth.jinghuilouyu.cn

U 高频实用片段                         120
来源：http://fnt.xylfe.cn

------------------------------------
来源：http://dro.ydjk.org.cn

合计                                  2106 条
来源：http://prr.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://pvf.birdmap.top

使用提醒
来源：http://tpm.bjfxy.top

--------------------------------------------------------------------------------
来源：http://qvz.sjlbkw.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zif.pycfn.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hhn.nwbrower.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dqy.guowangkeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ntf.hongshengwenyu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cwh.0kj1m.cn

—— 文件结束 ——
来源：http://uwg.dianchejie.cn

================================================================================
来源：http://ikz.hnxiangtu.top

程序语言常见例子速查手册（2024 版）
来源：http://jrk.jlsjyb.cn

Common Programming Examples Cheat Book
来源：http://mpj.shanyushiyangtech.top

================================================================================
来源：http://bmt.yj20258888.top

【收录内容】
来源：http://ete.shzxlz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://goq.ctjpmb.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zxb.daxiang520.top

SQL · Bash · C · C++
来源：http://puq.bbcook.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mgx.uphjek.com

【使用说明】
来源：http://zoa.zdqjudy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qij.aibaodan.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tmk.shanyushiyangkeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qfu.bjfxy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kda.fanxiaobao.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://kmw.jinqigufen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wur.hywenlv.cn


<!-- 参考信息 -->