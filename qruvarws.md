代发 wailian999

[U03] Py：加载 .env 配置
来源：http://tcu.zhijiandao.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kdc.svipenyu.cn

[U04] Py：变量调试打印
来源：http://wcr.hnqzz.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vet.316326.xyz

[U05] Py：列表去重且保序
来源：http://nuv.zhijiandao.cn

list(dict.fromkeys(arr))
来源：http://zeu.yueranfly.top

[U06] Py：合并两个字典
来源：http://ivq.yanxiufei.cn

{**a, **b}
来源：http://szf.yonumen.top

[U07] Py：反转字典键值
来源：http://lcg.cucudq.cn

{v: k for k, v in d.items()}
来源：http://kio.cucudq.cn

[U08] Py：展平二维列表
来源：http://roq.jiagoushi.top

[y for x in nested for y in x]
来源：http://crj.sufxvd.cn

[U09] Py：字典取最大值的键
来源：http://ytn.sxryk.cn

max(d, key=d.get)
来源：http://txn.sysykeji.top

[U10] Py：按值排序字典
来源：http://ajr.hywenlv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uhy.gotoacloud.top

[U11] Py：生成器表达式
来源：http://ybm.zhixingplan.top

(x * 2 for x in arr)
来源：http://bad.tanke756.top

[U12] Py：取出现最多的 3 个元素
来源：http://zyy.wangshuangyany.cn

Counter(arr).most_common(3)
来源：http://ltx.vehdjk.com

[U13] Py：固定长度队列
来源：http://zji.cucudq.cn

deque(maxlen=10)
来源：http://inb.haohaochexian.top

[U14] Py：分组收集到列表
来源：http://ovx.tarul.cn

defaultdict(list)
来源：http://uee.andypj.xyz

[U15] Py：高精度计时
来源：http://xco.zhaomingkeji.xyz

t = time.perf_counter()
来源：http://fnr.hywenlv.cn

[U16] Py：命令行参数解析
来源：http://uih.ppjwa.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qce.chenlongwang.top

[U17] Py：初始化日志
来源：http://xvv.ppjwa.cn

logging.basicConfig(level=logging.INFO)
来源：http://wgq.zhixingplan.top

[U18] Py：预编译正则
来源：http://qgd.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://lhc.chenjidiqi.icu

[U19] Py：正则替换带回调
来源：http://wdj.snrcjt.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zla.yj20258.top

[U20] Py：缓存函数结果
来源：http://eqa.sweek.top

@functools.lru_cache(maxsize=None)
来源：http://kcp.vqdsnc.cn

[U21] Py：自定义上下文管理器
来源：http://fyn.c1oappe.top

@contextlib.contextmanager
来源：http://jxh.xziqi.cn

[U22] Py：矩阵转置
来源：http://taq.svipenyu.cn

list(zip(*m))
来源：http://yco.yuanzhike.top

[U23] Py：分块读取大文件
来源：http://nlf.zycfv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zif.zdqjudy.top

[U24] Py：路径操作
来源：http://xfd.redwolf501.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ixz.fzhhl.top

[U25] Py：CSV 按字典读
来源：http://xnt.tanke756.top

csv.DictReader(f)
来源：http://xjm.c1oappe.top

[U26] Py：并发下载
来源：http://zqw.9152youxi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jef.hongshengwenyu.top

[U27] Py：异步 HTTP
来源：http://gpd.gotoacloud.top

aiohttp.ClientSession() 配合 async with
来源：http://pkc.smart0.xyz

[U28] Py：类型别名
来源：http://mbs.cheryme.top

UserId = int
来源：http://oty.ppjwa.cn

[U29] Py：属性校验
来源：http://unt.xuanzx.com

@property 与 @x.setter 配合
来源：http://ysb.yuanzhike.top

[U30] Py：数据类
来源：http://yzn.yfazqb.com

@dataclass(slots=True)
来源：http://rdc.yueranfly.top

[U31] Py：单测
来源：http://vbi.zhijiandao.cn

python -m pytest -q
来源：http://vrm.yj202588.top

[U32] Py：代码格式化
来源：http://ogg.pengpengdd.cyou

ruff format . && ruff check --fix .
来源：http://cql.yuxming.cn

[U33] Py：打包发布
来源：http://vnl.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://qic.0kj1m.cn

[U34] Py：判断编码
来源：http://tfo.cdnleiting.top

chardet.detect(raw)
来源：http://wlo.xziqi.cn

[U35] Py：发送邮件
来源：http://pxr.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://olg.gaohongyu789.top

[U36] Py：定时任务
来源：http://zuo.wangdashe.top

schedule.every(10).minutes.do(job)
来源：http://gul.snrcjt.cn

[U37] Py：读写 Excel
来源：http://qne.meibo888.top

pandas.read_excel / DataFrame.to_excel
来源：http://gyf.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://oja.xziqi.cn

Path(__file__).resolve().parent
来源：http://vqt.meibo888.top

[U39] Py：判断是否在交互环境
来源：http://zzj.hnqzz.top

sys.stdout.isatty()
来源：http://jzd.zhoulong.xyz

[U40] Py：打印到标准错误
来源：http://bjt.guannengcc.top

print("err", file=sys.stderr)
来源：http://vqn.havefunace.top

[U41] PHP：初始化 Composer 项目
来源：http://ccc.yanxiufei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yld.hysaishi.cn

[U42] PHP：PSR-4 自动加载
来源：http://vct.nanxinkj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qws.mhx1999.top

[U43] PHP：声明命名空间
来源：http://hxk.cqqwz.cn

namespace App\Http;
来源：http://dic.aizwys.cn

[U44] PHP：开启严格类型
来源：http://aqh.yfazqb.com

declare(strict_types=1);
来源：http://cot.jqgufenzy.top

[U45] PHP：类型声明与返回类型
来源：http://xqv.zdbjq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gxp.guannengcc.top

[U46] PHP：可空类型
来源：http://pxt.fzhhl.top

?string $name = null
来源：http://ptj.epnwcf.com

[U47] PHP：联合类型
来源：http://raw.ywan-chungtsiang.top

int|string $id
来源：http://rqx.epnwcf.com

[U48] PHP：纯枚举
来源：http://qsc.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lxj.tian-w.cn

[U49] PHP：只读属性
来源：http://zny.uphjek.com

public readonly string $name
来源：http://wrq.dashuyun.cn

[U50] PHP：构造器属性提升
来源：http://abs.aibaodan.cn

public function __construct(private int $id) {}
来源：http://azx.jinghuilouyu.cn

[U51] PHP：数组解构
来源：http://fkc.yj20258.top

[$a, $b] = $arr;
来源：http://cic.yj20258.top

[U52] PHP：箭头函数
来源：http://yew.chenjidiqi.icu

$double = fn($x) => $x * 2;
来源：http://xke.gzhubu.top

[U53] PHP：空合并运算符
来源：http://pdt.nwbrower.top

$v = $a ?? $b ?? "default";
来源：http://gdr.chenzaomai.com

[U54] PHP：空安全调用
来源：http://egl.ybcxt.top

$obj?->method()
来源：http://loa.yangfankeji.com

[U55] PHP：match 表达式
来源：http://kag.fengsongda.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://amr.ctjpmb.com

[U56] PHP：命名参数
来源：http://olb.bbcook.cn

f(a: 1, b: 2)
来源：http://hur.snrcjt.cn

[U57] PHP：字符串插值
来源：http://qcf.gogol.net.cn

"值: {$a}"
来源：http://twm.yfazqb.com

[U58] PHP：数组三件套
来源：http://yjw.zhongyouzk.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://umy.gogol.net.cn

[U59] PHP：自定义排序
来源：http://jpi.nanxinkj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vaw.pycfn.com

[U60] PHP：JSON 编解码
来源：http://xxh.hesvh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uyg.pycfn.com

[U61] PHP：正则
来源：http://ffd.hcnkem.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zzj.iojbl.cn

[U62] PHP：日期对象
来源：http://dja.jinqigfzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ile.ybcxt.top

[U63] PHP：文件读写
来源：http://xms.tian-w.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rqh.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://jul.yuanzhike.top

glob("dir/*.php");  scandir("dir");
来源：http://wwq.wangdashe.top

[U65] PHP：会话
来源：http://sps.cucudq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dox.gogol.net.cn

[U66] PHP：设置 Cookie
来源：http://nsl.ywan-chungtsiang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://htq.yangfankeji.com

[U67] PHP：处理文件上传
来源：http://oms.jqgfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://veq.shanyushiyangtech.top

[U68] PHP：PDO 连接
来源：http://key.sysykeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cpv.zhixingplan.top

[U69] PHP：PDO 预处理
来源：http://frk.tianlin.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nkh.ehwqpu.com

[U70] PHP：PDO 事务
来源：http://nfz.jiagoushi.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ako.yj20258888.top

[U71] PHP：抛出异常
来源：http://xtf.jlsjyb.cn

throw new RuntimeException("失败", 500);
来源：http://wdx.zhoulong.xyz

[U72] PHP：写错误日志
来源：http://yzu.chenlongwang.top

error_log("失败: " . $e->getMessage());
来源：http://eef.xinyue.icu

[U73] PHP：读取 ini 配置
来源：http://qnx.fengsongda.top

parse_ini_file("config.ini", true)
来源：http://oiz.hesvh.cn

[U74] PHP：读取环境变量
来源：http://snx.quarkkingdee.top

getenv("APP_ENV") ?: "production"
来源：http://wem.hysaishi.cn

[U75] PHP：依赖注入
来源：http://krm.9152youxi.cn

composer require psr/container
来源：http://dfz.yongpay.top

[U76] PHP：简单路由
来源：http://wdf.xylfe.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hnm.sufxvd.cn

[U77] PHP：模板渲染
来源：http://xsv.pycfn.com

composer require twig/twig
来源：http://gbq.bbcook.cn

[U78] PHP：单元测试
来源：http://ltp.ppjwa.cn

composer require --dev phpunit/phpunit
来源：http://tny.pengpengdd.cyou

[U79] PHP：静态分析
来源：http://cuo.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://old.cdnleiting.top

[U80] PHP：代码规范修复
来源：http://hbb.redwolf501.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ngw.hysaishi.cn

[U81] JS：初始化项目
来源：http://ssg.hongshengwenyu.top

npm init -y;  npm i express
来源：http://kyh.zdbjq.cn

[U82] JS：package.json 脚本
来源：http://ato.316326.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bds.pycfn.com

[U83] JS：ES Module 导入导出
来源：http://ihh.ehwqpu.com

export const a = 1;  import { a } from "./m.js";
来源：http://wwa.pycfn.com

[U84] JS：CommonJS 写法
来源：http://cjc.c1oappe.top

module.exports = { a };  const { a } = require("./m");
来源：http://xjn.mhx1999.top

[U85] JS：可选链
来源：http://xmy.xuetiantiany.cn

a?.b?.c
来源：http://aur.meibo888.top

[U86] JS：空值合并
来源：http://qmi.sxryk.cn

a ?? b
来源：http://qfw.0kj1m.cn

[U87] JS：解构默认值
来源：http://dwz.hfpthk.cn

const { a = 1, b = 2 } = obj;
来源：http://wnw.xylfe.cn

[U88] JS：对象展开合并
来源：http://vwg.redwolf501.top

{ ...a, ...b }
来源：http://tqq.gaohongyu789.top

[U89] JS：数组去重
来源：http://axb.xuetiantiany.cn

[...new Set(arr)]
来源：http://iug.bbcook.cn

[U90] JS：数字数组排序
来源：http://wux.shangyingyoupin.top

[...arr].sort((a, b) => a - b)
来源：http://rby.quarkkingdee.top

[U91] JS：对象键值遍历
来源：http://lal.aizwys.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bdr.shuidangran.top

[U92] JS：深拷贝
来源：http://gjh.tarul.cn

structuredClone(obj)
来源：http://mpj.hongshengwenyu.top

[U93] JS：模板字符串
来源：http://ses.pengpengdd.cyou

`共 ${n} 条`
来源：http://uij.yanxiufei.cn

[U94] JS：箭头函数
来源：http://yqn.fzhhl.top

const double = x => x * 2;
来源：http://nip.pengpengdd.cyou

[U95] JS：Promise 包装
来源：http://rbn.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://pcf.9152youxi.cn

[U96] JS：async/await 与异常
来源：http://frm.bbcook.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zim.shzxlz.cn

[U97] JS：并发请求
来源：http://zlx.shanyushiyangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ace.yvedp.cn

[U98] JS：fetch 带 JSON
来源：http://gjt.zdqjudy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://epc.tian-w.cn

[U99] JS：事件监听
来源：http://svb.xinyue.icu

el.addEventListener("click", e => {})
来源：http://sxf.zdqjudy.top

[U100] JS：DOM 查询
来源：http://avu.sxryk.cn

document.querySelector(".item")
来源：http://sca.9152youxi.cn

[U101] JS：classList 操作
来源：http://cyz.yangfankeji.com

el.classList.toggle("active")
来源：http://uqy.cheryme.top

[U102] JS：本地存储
来源：http://way.yuxming.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jpq.xingfuxueyuan.xyz

[U103] JS：定时器
来源：http://dhm.jyoumei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iax.fengsongda.top

[U104] JS：防抖
来源：http://piv.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fpj.316326.xyz

[U105] JS：节流
来源：http://lud.yj20258888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aux.tarul.cn

[U106] JS：日期格式化
来源：http://xef.fanxiaobao.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yny.uphjek.com

[U107] JS：数字千分位
来源：http://nbd.yfazqb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nom.sjlbkw.cn

[U108] JS：随机整数
来源：http://mui.quarkkingdee.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dae.zdbjq.cn

[U109] JS：数组分组
来源：http://ifr.daria6918.cn

Object.groupBy(arr, x => x.type)
来源：http://zkm.ydjk.org.cn

[U110] JS：数组分块
来源：http://oht.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ogs.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://dtw.zdbjq.cn

new Map(Object.entries(obj))
来源：http://axj.jinqigfzy.top

[U112] JS：字符串补位
来源：http://gbx.birdmap.top

"7".padStart(3, "0")
来源：http://qfc.jinqigfzy.top

[U113] JS：正则替换全部
来源：http://klv.pycfn.com

s.replaceAll("a", "b")
来源：http://dpd.sxryk.cn

[U114] JS：JSON 深比较
来源：http://dwt.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sru.epnwcf.com

[U115] JS：生成 UUID
来源：http://gtu.vqdsnc.cn

crypto.randomUUID()
来源：http://mtw.aibaodan.cn

[U116] JS：类型检查（JSDoc）
来源：http://pgl.cqqwz.cn

/** @param {string} name */ function f(name) {}
来源：http://bwn.yuanzhike.top

[U117] JS：单元测试
来源：http://mou.yonumen.top

npm i -D vitest;  npx vitest
来源：http://azx.nanxuanxn.top

[U118] JS：开发服务器
来源：http://bhx.gogol.net.cn

npm i -D vite;  npx vite
来源：http://fjv.guannengcc.top

[U119] JS：生产构建
来源：http://klt.zdqjudy.top

npx vite build
来源：http://ltx.jinqigufen.top

[U120] JS：读取环境变量（Vite）
来源：http://eeu.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://ptp.316326.xyz

================================================================================
来源：http://qtc.ydzc1.top

统计汇总
来源：http://nih.gzhubu.top

================================================================================
来源：http://agh.sysykeji.top

按语言统计（条）：
来源：http://aqe.jqgfzy.top

Python ......... 252
来源：http://vef.nanxuanxn.top

PHP ............ 252
来源：http://wdl.hammf.cn

JavaScript ..... 252
来源：http://kkh.xuetiantiany.cn

TypeScript ..... 212
来源：http://qjl.guannengcc.top

Java ........... 212
来源：http://slj.nanxinkj.top

Go ............. 212
来源：http://ogk.sufxvd.cn

Ruby ........... 212
来源：http://qov.zdbjq.cn

C# ............. 212
来源：http://exo.ctjpmb.com

C .............. 30
来源：http://lhq.shanyushiyangkeji.top

C++ ............ 30
来源：http://gsh.jinyuanbaomall.cn

SQL ............ 90
来源：http://dft.yuxming.cn

Bash ........... 80
来源：http://bqu.hnqzz.top

Kotlin ......... 15
来源：http://oqa.hesvh.cn

Swift .......... 15
来源：http://agw.shanyushiyangtech.top

Lua ............ 10
来源：http://djq.feifeiyinyue.top

Perl ........... 10
来源：http://qbh.jinghuilouyu.cn

Scala .......... 10
来源：http://dza.meibo888.top

------------------------------------
来源：http://qke.quarkkingdee.top

合计 ........... 2106 条
来源：http://dcn.daria6918.cn

按章节统计：
来源：http://iuw.xylfe.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xdf.shangyingyoupin.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ama.tanke756.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://weg.jianghu66.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://shj.iojbl.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zhk.chenzaomai.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tfm.tian-w.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hul.shuidangran.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zct.zhixingplan.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://htt.shuidangran.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wzl.xuanzx.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sju.birdmap.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://chd.wangdashe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://svt.zhixingplan.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lhu.tarul.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rky.shanyushiyangkeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yrw.hammf.cn

Q SQL 专题                              90
来源：http://fzt.hcnkem.com

R Bash 专题                             80
来源：http://eht.cheryme.top

S C / C++ 专题                          60
来源：http://llk.ydjk.org.cn

T 其他语言补充                          60
来源：http://zsy.zdqjudy.top

U 高频实用片段                         120
来源：http://tej.ctjpmb.com

------------------------------------
来源：http://rjk.yvedp.cn

合计                                  2106 条
来源：http://wmu.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://ebx.yj20258.top

使用提醒
来源：http://xja.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://pdm.gogol.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://upb.fktsv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lbm.sxryk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jxr.jinqigfzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lav.mhx1999.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://egk.sufxvd.cn

—— 文件结束 ——
来源：http://kai.yuxming.cn

================================================================================
来源：http://oyg.feifeiyinyue.top

程序语言常见例子速查手册（2024 版）
来源：http://wex.jinyuanbaomall.cn

Common Programming Examples Cheat Book
来源：http://xkp.hfpthk.cn

================================================================================
来源：http://loo.chenlongwang.top

【收录内容】
来源：http://flz.meibo888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://zom.hnqzz.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ffa.yanxiufei.cn

SQL · Bash · C · C++
来源：http://sok.zhaomingkeji.xyz


<!-- 参考信息 -->