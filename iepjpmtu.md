代发 wailian999

[U01] Py：创建虚拟环境
来源：http://jub.aibaodan.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bpp.shanyushiyangtech.top

[U02] Py：导出 / 安装依赖
来源：http://sxl.jqgfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ccu.hnqzz.top

[U03] Py：加载 .env 配置
来源：http://azz.aibaodan.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gxn.316326.xyz

[U04] Py：变量调试打印
来源：http://nwa.nanxinkj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dlp.yongpay.top

[U05] Py：列表去重且保序
来源：http://cco.vehdjk.com

list(dict.fromkeys(arr))
来源：http://xaq.zhaomingkeji.xyz

[U06] Py：合并两个字典
来源：http://eit.zhiwuduotai.top

{**a, **b}
来源：http://qot.fehbvm.com

[U07] Py：反转字典键值
来源：http://psa.shanyushiyangtech.top

{v: k for k, v in d.items()}
来源：http://hqz.9152youxi.cn

[U08] Py：展平二维列表
来源：http://yos.vehdjk.com

[y for x in nested for y in x]
来源：http://enn.fktsv.cn

[U09] Py：字典取最大值的键
来源：http://dsv.redwolf501.top

max(d, key=d.get)
来源：http://pdq.zhaomingkeji.xyz

[U10] Py：按值排序字典
来源：http://pko.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ixl.cheryme.top

[U11] Py：生成器表达式
来源：http://tmd.cheryme.top

(x * 2 for x in arr)
来源：http://erp.tian-w.cn

[U12] Py：取出现最多的 3 个元素
来源：http://flb.dianchejie.cn

Counter(arr).most_common(3)
来源：http://sop.zhengqikj.top

[U13] Py：固定长度队列
来源：http://ozs.yangfankeji.com

deque(maxlen=10)
来源：http://gwy.tian-w.cn

[U14] Py：分组收集到列表
来源：http://svd.quarkkingdee.top

defaultdict(list)
来源：http://mqw.cucudq.cn

[U15] Py：高精度计时
来源：http://rbk.gotoacloud.top

t = time.perf_counter()
来源：http://fmi.mhx1999.top

[U16] Py：命令行参数解析
来源：http://kph.52xcode.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ytd.jiagoushi.top

[U17] Py：初始化日志
来源：http://bpr.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://lay.tarul.cn

[U18] Py：预编译正则
来源：http://bun.aibaodan.cn

pat = re.compile(r"\d+")
来源：http://sdx.xinyue.icu

[U19] Py：正则替换带回调
来源：http://ije.zhixingplan.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kji.jinqigufen.top

[U20] Py：缓存函数结果
来源：http://mvi.sufxvd.cn

@functools.lru_cache(maxsize=None)
来源：http://eja.sjlbkw.cn

[U21] Py：自定义上下文管理器
来源：http://rnd.tianlin.xyz

@contextlib.contextmanager
来源：http://tdo.snrcjt.cn

[U22] Py：矩阵转置
来源：http://cll.cqqwz.cn

list(zip(*m))
来源：http://wob.yj20258.top

[U23] Py：分块读取大文件
来源：http://zrh.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nxa.chenzaomai.com

[U24] Py：路径操作
来源：http://ywt.iojbl.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hgx.sxryk.cn

[U25] Py：CSV 按字典读
来源：http://mmz.hcnkem.com

csv.DictReader(f)
来源：http://ict.bjfxy.top

[U26] Py：并发下载
来源：http://hts.jyoumei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rdo.dashuyun.cn

[U27] Py：异步 HTTP
来源：http://gvf.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://jjf.tian-w.cn

[U28] Py：类型别名
来源：http://csv.meibo888.top

UserId = int
来源：http://kde.wangdashe.top

[U29] Py：属性校验
来源：http://pyy.hongshengwenyu.top

@property 与 @x.setter 配合
来源：http://njf.fzhhl.top

[U30] Py：数据类
来源：http://szl.nanxuanxn.top

@dataclass(slots=True)
来源：http://mro.cheryme.top

[U31] Py：单测
来源：http://qkh.zdbjq.cn

python -m pytest -q
来源：http://aua.jqgufenzy.top

[U32] Py：代码格式化
来源：http://eyr.smart0.xyz

ruff format . && ruff check --fix .
来源：http://dlu.52xcode.cn

[U33] Py：打包发布
来源：http://olx.kuanghao11.cn

python -m build  （依赖 pyproject.toml）
来源：http://txl.xingfuxueyuan.xyz

[U34] Py：判断编码
来源：http://uui.guannengcc.top

chardet.detect(raw)
来源：http://aue.zhaomingkeji.xyz

[U35] Py：发送邮件
来源：http://efe.gaohongyu789.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gyv.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://uow.redwolf501.top

schedule.every(10).minutes.do(job)
来源：http://gri.xingfuxueyuan.xyz

[U37] Py：读写 Excel
来源：http://zoe.shanyushiyangtech.top

pandas.read_excel / DataFrame.to_excel
来源：http://btb.xuanzx.com

[U38] Py：获取脚本所在目录
来源：http://tcv.316326.xyz

Path(__file__).resolve().parent
来源：http://cvq.shzxlz.cn

[U39] Py：判断是否在交互环境
来源：http://dez.ppjwa.cn

sys.stdout.isatty()
来源：http://xld.snrcjt.cn

[U40] Py：打印到标准错误
来源：http://jqy.sufxvd.cn

print("err", file=sys.stderr)
来源：http://nwl.yongpay.top

[U41] PHP：初始化 Composer 项目
来源：http://hkp.xziqi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://itn.wangshuangyany.cn

[U42] PHP：PSR-4 自动加载
来源：http://rgo.zdbjq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rpx.hnqzz.top

[U43] PHP：声明命名空间
来源：http://wdp.yuxming.cn

namespace App\Http;
来源：http://vgc.chenzaomai.com

[U44] PHP：开启严格类型
来源：http://txi.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://wer.yj20258888.top

[U45] PHP：类型声明与返回类型
来源：http://jqy.xinyue.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://wry.hongshengwenyu.top

[U46] PHP：可空类型
来源：http://jox.epnwcf.com

?string $name = null
来源：http://ufq.vqdsnc.cn

[U47] PHP：联合类型
来源：http://nnc.hongshengwenyu.top

int|string $id
来源：http://wiz.sweek.top

[U48] PHP：纯枚举
来源：http://gfe.fktsv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yna.pycfn.com

[U49] PHP：只读属性
来源：http://jfu.wangdashe.top

public readonly string $name
来源：http://guf.sjlbkw.cn

[U50] PHP：构造器属性提升
来源：http://yae.birdmap.top

public function __construct(private int $id) {}
来源：http://zpu.yuanzhike.top

[U51] PHP：数组解构
来源：http://jaz.smart0.xyz

[$a, $b] = $arr;
来源：http://wvi.zhongyouzk.top

[U52] PHP：箭头函数
来源：http://yqw.zdbjq.cn

$double = fn($x) => $x * 2;
来源：http://grh.zhoulong.xyz

[U53] PHP：空合并运算符
来源：http://txy.nwbrower.top

$v = $a ?? $b ?? "default";
来源：http://zrd.9152youxi.cn

[U54] PHP：空安全调用
来源：http://lnx.fzhhl.top

$obj?->method()
来源：http://cer.zdbjq.cn

[U55] PHP：match 表达式
来源：http://yvo.yuanzhike.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qcp.hammf.cn

[U56] PHP：命名参数
来源：http://wrp.zdbjq.cn

f(a: 1, b: 2)
来源：http://vln.uphjek.com

[U57] PHP：字符串插值
来源：http://xji.dashuyun.cn

"值: {$a}"
来源：http://plg.fengsongda.top

[U58] PHP：数组三件套
来源：http://jsc.hesvh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fkq.jqgfzy.top

[U59] PHP：自定义排序
来源：http://mjd.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cwc.zhoulong.xyz

[U60] PHP：JSON 编解码
来源：http://jbx.smart0.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xml.xylfe.cn

[U61] PHP：正则
来源：http://vod.jianghu66.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://omp.cucudq.cn

[U62] PHP：日期对象
来源：http://fjd.nanxuanxn.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qqd.xuetiantiany.cn

[U63] PHP：文件读写
来源：http://ctv.haohaochexian.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cnb.zhongyouzk.top

[U64] PHP：目录遍历
来源：http://piw.wangdashe.top

glob("dir/*.php");  scandir("dir");
来源：http://reu.kuanghao11.cn

[U65] PHP：会话
来源：http://fdc.ydzc1.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rhp.52xcode.cn

[U66] PHP：设置 Cookie
来源：http://jpe.yueranfly.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qsw.yuanzhike.top

[U67] PHP：处理文件上传
来源：http://exl.shanyushiyangtech.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zyu.chenjidiqi.icu

[U68] PHP：PDO 连接
来源：http://epp.316326.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zfk.cucudq.cn

[U69] PHP：PDO 预处理
来源：http://ejq.zhixingplan.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vxu.iojbl.cn

[U70] PHP：PDO 事务
来源：http://hgh.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uyf.haohaochexian.top

[U71] PHP：抛出异常
来源：http://hwj.jyoumei.cn

throw new RuntimeException("失败", 500);
来源：http://sdg.hesvh.cn

[U72] PHP：写错误日志
来源：http://jib.hongshengwenyu.top

error_log("失败: " . $e->getMessage());
来源：http://rwu.yfazqb.com

[U73] PHP：读取 ini 配置
来源：http://xbz.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://njd.fzhhl.top

[U74] PHP：读取环境变量
来源：http://fei.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://mka.sufxvd.cn

[U75] PHP：依赖注入
来源：http://tll.ywan-chungtsiang.top

composer require psr/container
来源：http://qpe.aibaodan.cn

[U76] PHP：简单路由
来源：http://ftt.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mxh.jinqigfzy.top

[U77] PHP：模板渲染
来源：http://iww.hcnkem.com

composer require twig/twig
来源：http://upk.yonumen.top

[U78] PHP：单元测试
来源：http://mpw.feifeiyinyue.top

composer require --dev phpunit/phpunit
来源：http://ffo.pengpengdd.cyou

[U79] PHP：静态分析
来源：http://qaq.nwbrower.top

composer require --dev phpstan/phpstan
来源：http://jdi.uphjek.com

[U80] PHP：代码规范修复
来源：http://ddq.quarkkingdee.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wak.aizwys.cn

[U81] JS：初始化项目
来源：http://vdf.gogol.net.cn

npm init -y;  npm i express
来源：http://cqm.ybcxt.top

[U82] JS：package.json 脚本
来源：http://mvh.fengsongda.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nwa.sufxvd.cn

[U83] JS：ES Module 导入导出
来源：http://tnb.havefunace.top

export const a = 1;  import { a } from "./m.js";
来源：http://znz.kuanghao11.cn

[U84] JS：CommonJS 写法
来源：http://asy.quarkkingdee.top

module.exports = { a };  const { a } = require("./m");
来源：http://twz.c1oappe.top

[U85] JS：可选链
来源：http://eyp.yuanzhike.top

a?.b?.c
来源：http://upj.bjfxy.top

[U86] JS：空值合并
来源：http://uzp.yanxiufei.cn

a ?? b
来源：http://vjq.yj20258888.top

[U87] JS：解构默认值
来源：http://woo.chenzaomai.com

const { a = 1, b = 2 } = obj;
来源：http://zyb.tian-w.cn

[U88] JS：对象展开合并
来源：http://qit.hywenlv.cn

{ ...a, ...b }
来源：http://hyz.vehdjk.com

[U89] JS：数组去重
来源：http://xnn.jinyuanbaomall.cn

[...new Set(arr)]
来源：http://inu.jyoumei.cn

[U90] JS：数字数组排序
来源：http://ggo.dashuyun.cn

[...arr].sort((a, b) => a - b)
来源：http://atg.tian-w.cn

[U91] JS：对象键值遍历
来源：http://ika.yonumen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mfy.jqgufenzy.top

[U92] JS：深拷贝
来源：http://ika.9152youxi.cn

structuredClone(obj)
来源：http://xuq.redwolf501.top

[U93] JS：模板字符串
来源：http://knj.epnwcf.com

`共 ${n} 条`
来源：http://jad.wangshuangyany.cn

[U94] JS：箭头函数
来源：http://wcd.hammf.cn

const double = x => x * 2;
来源：http://hqv.yj20258888.top

[U95] JS：Promise 包装
来源：http://mtm.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://dao.ivvv.top

[U96] JS：async/await 与异常
来源：http://anx.shanyushiyangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://joh.zhoulong.xyz

[U97] JS：并发请求
来源：http://cls.tarul.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zkq.0kj1m.cn

[U98] JS：fetch 带 JSON
来源：http://tuk.yfazqb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gvk.sysykeji.top

[U99] JS：事件监听
来源：http://tow.tarul.cn

el.addEventListener("click", e => {})
来源：http://qko.tanke756.top

[U100] JS：DOM 查询
来源：http://zzm.sxryk.cn

document.querySelector(".item")
来源：http://jyc.tian-w.cn

[U101] JS：classList 操作
来源：http://qtr.dianchejie.cn

el.classList.toggle("active")
来源：http://wqw.jinqigfzy.top

[U102] JS：本地存储
来源：http://qdd.hongshengwenyu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vyz.havefunace.top

[U103] JS：定时器
来源：http://gsl.zhaomingkeji.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nbl.shanyushiyangtech.top

[U104] JS：防抖
来源：http://opi.xziqi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ltt.ywan-chungtsiang.top

[U105] JS：节流
来源：http://coj.xylfe.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rmd.zhixingplan.top

[U106] JS：日期格式化
来源：http://scn.hywenlv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jum.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://blv.nanxinkj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pau.yj20258.top

[U108] JS：随机整数
来源：http://vqs.yuxming.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ldt.shanyushiyangkeji.top

[U109] JS：数组分组
来源：http://zqb.iojbl.cn

Object.groupBy(arr, x => x.type)
来源：http://zyl.xingfuxueyuan.xyz

[U110] JS：数组分块
来源：http://ada.xylfe.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vnc.fzhhl.top

[U111] JS：对象转 Map
来源：http://xgr.zhongyouzk.top

new Map(Object.entries(obj))
来源：http://glk.ctjpmb.com

[U112] JS：字符串补位
来源：http://nxb.hfpthk.cn

"7".padStart(3, "0")
来源：http://ryz.dianchejie.cn

[U113] JS：正则替换全部
来源：http://hnj.meibo888.top

s.replaceAll("a", "b")
来源：http://qdq.nanxinkj.top

[U114] JS：JSON 深比较
来源：http://dcm.sxryk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://otk.zdbjq.cn

[U115] JS：生成 UUID
来源：http://tgj.sxryk.cn

crypto.randomUUID()
来源：http://qqz.yueranfly.top

[U116] JS：类型检查（JSDoc）
来源：http://mlo.vehdjk.com

/** @param {string} name */ function f(name) {}
来源：http://qwl.aizwys.cn

[U117] JS：单元测试
来源：http://crn.sysykeji.top

npm i -D vitest;  npx vitest
来源：http://xip.tian-w.cn

[U118] JS：开发服务器
来源：http://mxk.52xcode.cn

npm i -D vite;  npx vite
来源：http://lln.yongpay.top

[U119] JS：生产构建
来源：http://oyx.xuetiantiany.cn

npx vite build
来源：http://fww.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://abg.fengsongda.top

import.meta.env.VITE_API_URL
来源：http://tua.ywan-chungtsiang.top

================================================================================
来源：http://aqo.havefunace.top

统计汇总
来源：http://kyq.gzhubu.top

================================================================================
来源：http://nrm.tanke756.top

按语言统计（条）：
来源：http://hnm.zhiwuduotai.top

Python ......... 252
来源：http://elw.zhongyouzk.top

PHP ............ 252
来源：http://drr.zdbjq.cn

JavaScript ..... 252
来源：http://bnv.jinqigufen.top

TypeScript ..... 212
来源：http://drj.ywan-chungtsiang.top

Java ........... 212
来源：http://oxv.zhoulong.xyz

Go ............. 212
来源：http://gnj.ctjpmb.com

Ruby ........... 212
来源：http://gfm.hnqzz.top

C# ............. 212
来源：http://vwo.meibo888.top

C .............. 30
来源：http://cnz.yfazqb.com

C++ ............ 30
来源：http://nof.fktsv.cn

SQL ............ 90
来源：http://kfg.fengsongda.top

Bash ........... 80
来源：http://qth.c1oappe.top

Kotlin ......... 15
来源：http://odl.smart0.xyz

Swift .......... 15
来源：http://heb.zhoulong.xyz

Lua ............ 10
来源：http://bng.ppjwa.cn

Perl ........... 10
来源：http://pha.hywenlv.cn

Scala .......... 10
来源：http://zig.xziqi.cn

------------------------------------
来源：http://etz.cheryme.top

合计 ........... 2106 条
来源：http://wbg.yonumen.top

按章节统计：
来源：http://oje.vqdsnc.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ont.zhongyouzk.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qjn.yanxiufei.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hcg.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cki.yueranfly.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wfh.nanxuanxn.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dah.xziqi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dxk.meibo888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://btc.yj202588.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ovc.dianchejie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kfw.guannengcc.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pln.zhijiandao.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jzk.chenzaomai.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rou.ydzc1.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zun.hywenlv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://csf.uphjek.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iaq.zdbjq.cn

Q SQL 专题                              90
来源：http://wep.yuxming.cn

R Bash 专题                             80
来源：http://lai.cucudq.cn

S C / C++ 专题                          60
来源：http://grv.c1oappe.top

T 其他语言补充                          60
来源：http://eob.jqgfzy.top

U 高频实用片段                         120
来源：http://fhf.ctjpmb.com

------------------------------------
来源：http://dvx.meibo888.top

合计                                  2106 条
来源：http://aed.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://rod.gotoacloud.top

使用提醒
来源：http://sxo.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://xhr.xuanzx.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bkt.xingfuxueyuan.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ebd.birdmap.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://efz.jqgfzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://cxr.xinyue.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ney.cdnleiting.top

—— 文件结束 ——
来源：http://idl.yuanzhike.top

================================================================================
来源：http://fej.zdbjq.cn

程序语言常见例子速查手册（2024 版）
来源：http://rah.xingfuxueyuan.xyz

Common Programming Examples Cheat Book
来源：http://pkk.birdmap.top

================================================================================
来源：http://sus.ybcxt.top


<!-- 参考信息 -->