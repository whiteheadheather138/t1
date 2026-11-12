代发 wailian999

[U01] Py：创建虚拟环境
来源：http://eub.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://zif.9152youxi.cn

[U02] Py：导出 / 安装依赖
来源：http://ela.pycfn.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iqn.guannengcc.top

[U03] Py：加载 .env 配置
来源：http://wel.yangfankeji.com

from dotenv import load_dotenv; load_dotenv()
来源：http://ckd.zhongyouzk.top

[U04] Py：变量调试打印
来源：http://dpm.bjfxy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mgm.guowangkeji.top

[U05] Py：列表去重且保序
来源：http://dzo.zhixingplan.top

list(dict.fromkeys(arr))
来源：http://ise.guowangkeji.top

[U06] Py：合并两个字典
来源：http://zgp.tarul.cn

{**a, **b}
来源：http://nrl.cdnleiting.top

[U07] Py：反转字典键值
来源：http://xza.vqdsnc.cn

{v: k for k, v in d.items()}
来源：http://wty.yvedp.cn

[U08] Py：展平二维列表
来源：http://hwn.hysaishi.cn

[y for x in nested for y in x]
来源：http://tke.wangdashe.top

[U09] Py：字典取最大值的键
来源：http://mgu.cucudq.cn

max(d, key=d.get)
来源：http://ztw.gogol.net.cn

[U10] Py：按值排序字典
来源：http://obv.hfpthk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lua.daxiang520.top

[U11] Py：生成器表达式
来源：http://wiv.snrcjt.cn

(x * 2 for x in arr)
来源：http://adf.gzhubu.top

[U12] Py：取出现最多的 3 个元素
来源：http://wyc.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://nsq.sufxvd.cn

[U13] Py：固定长度队列
来源：http://kwc.jlsjyb.cn

deque(maxlen=10)
来源：http://ghi.iojbl.cn

[U14] Py：分组收集到列表
来源：http://cfx.zhixingplan.top

defaultdict(list)
来源：http://gxn.haohaochexian.top

[U15] Py：高精度计时
来源：http://lft.birdmap.top

t = time.perf_counter()
来源：http://juz.sufxvd.cn

[U16] Py：命令行参数解析
来源：http://srm.redwolf501.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xqm.tanke756.top

[U17] Py：初始化日志
来源：http://qvf.pycfn.com

logging.basicConfig(level=logging.INFO)
来源：http://nkg.guowangkeji.top

[U18] Py：预编译正则
来源：http://shu.yvedp.cn

pat = re.compile(r"\d+")
来源：http://cwx.ybcxt.top

[U19] Py：正则替换带回调
来源：http://utj.ywan-chungtsiang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://klw.sweek.top

[U20] Py：缓存函数结果
来源：http://doc.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://ffx.gaohongyu789.top

[U21] Py：自定义上下文管理器
来源：http://cvm.bjfxy.top

@contextlib.contextmanager
来源：http://jed.zhoulong.xyz

[U22] Py：矩阵转置
来源：http://dwh.jinqigfzy.top

list(zip(*m))
来源：http://bvu.havefunace.top

[U23] Py：分块读取大文件
来源：http://gdc.smart0.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mpm.jinqigfzy.top

[U24] Py：路径操作
来源：http://klf.ppjwa.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vnc.nanxinkj.top

[U25] Py：CSV 按字典读
来源：http://hgc.wangshuangyany.cn

csv.DictReader(f)
来源：http://spv.cashguo.top

[U26] Py：并发下载
来源：http://oog.52xcode.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yph.jyoumei.cn

[U27] Py：异步 HTTP
来源：http://wbo.jinyuanbaomall.cn

aiohttp.ClientSession() 配合 async with
来源：http://qof.sufxvd.cn

[U28] Py：类型别名
来源：http://zxc.vehdjk.com

UserId = int
来源：http://bkv.fehbvm.com

[U29] Py：属性校验
来源：http://oox.sxryk.cn

@property 与 @x.setter 配合
来源：http://gki.316326.xyz

[U30] Py：数据类
来源：http://jwv.quarkkingdee.top

@dataclass(slots=True)
来源：http://myj.ydzc1.top

[U31] Py：单测
来源：http://xrg.jiagoushi.top

python -m pytest -q
来源：http://wov.hnqzz.top

[U32] Py：代码格式化
来源：http://hce.jinyuanbaomall.cn

ruff format . && ruff check --fix .
来源：http://sur.shangyingyoupin.top

[U33] Py：打包发布
来源：http://zcd.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://wus.yanxiufei.cn

[U34] Py：判断编码
来源：http://wiv.shangyingyoupin.top

chardet.detect(raw)
来源：http://aza.xinyue.icu

[U35] Py：发送邮件
来源：http://eqf.wangshuangyany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pny.fehbvm.com

[U36] Py：定时任务
来源：http://qly.ywan-chungtsiang.top

schedule.every(10).minutes.do(job)
来源：http://eli.yonumen.top

[U37] Py：读写 Excel
来源：http://nrz.aibaodan.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kpd.zhiwuduotai.top

[U38] Py：获取脚本所在目录
来源：http://wpz.iojbl.cn

Path(__file__).resolve().parent
来源：http://zav.yvedp.cn

[U39] Py：判断是否在交互环境
来源：http://svi.jinghuilouyu.cn

sys.stdout.isatty()
来源：http://pqz.xinyue.icu

[U40] Py：打印到标准错误
来源：http://voa.sjlbkw.cn

print("err", file=sys.stderr)
来源：http://ryw.quarkkingdee.top

[U41] PHP：初始化 Composer 项目
来源：http://qze.ydzc1.top

composer init;  composer require guzzlehttp/guzzle
来源：http://hmz.gogol.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://prc.vehdjk.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wzg.ehwqpu.com

[U43] PHP：声明命名空间
来源：http://olf.nanxinkj.top

namespace App\Http;
来源：http://lvc.zhongyouzk.top

[U44] PHP：开启严格类型
来源：http://tkz.shzxlz.cn

declare(strict_types=1);
来源：http://ixl.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://eva.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hys.redwolf501.top

[U46] PHP：可空类型
来源：http://kwg.jlsjyb.cn

?string $name = null
来源：http://ynk.yuxming.cn

[U47] PHP：联合类型
来源：http://smk.hammf.cn

int|string $id
来源：http://xau.shzxlz.cn

[U48] PHP：纯枚举
来源：http://fpf.9152youxi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ace.hnqzz.top

[U49] PHP：只读属性
来源：http://fab.hfpthk.cn

public readonly string $name
来源：http://ame.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://nqf.cheryme.top

public function __construct(private int $id) {}
来源：http://xqa.tarul.cn

[U51] PHP：数组解构
来源：http://gro.xuetiantiany.cn

[$a, $b] = $arr;
来源：http://bvd.yj20258.top

[U52] PHP：箭头函数
来源：http://hnq.xuanzx.com

$double = fn($x) => $x * 2;
来源：http://ati.aizwys.cn

[U53] PHP：空合并运算符
来源：http://mwh.zycfv.cn

$v = $a ?? $b ?? "default";
来源：http://dlc.yuanzhike.top

[U54] PHP：空安全调用
来源：http://krk.zhixingplan.top

$obj?->method()
来源：http://usg.yueranfly.top

[U55] PHP：match 表达式
来源：http://tnj.yuanzhike.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ydr.yuxming.cn

[U56] PHP：命名参数
来源：http://gmh.cashguo.top

f(a: 1, b: 2)
来源：http://vqn.316326.xyz

[U57] PHP：字符串插值
来源：http://zbv.hnqzz.top

"值: {$a}"
来源：http://nmo.dianchejie.cn

[U58] PHP：数组三件套
来源：http://mno.xuanzx.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nnv.meibo888.top

[U59] PHP：自定义排序
来源：http://rxz.nanxuanxn.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lpn.gotoacloud.top

[U60] PHP：JSON 编解码
来源：http://duq.sufxvd.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zdr.ehwqpu.com

[U61] PHP：正则
来源：http://wua.daria6918.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://drw.kuanghao11.cn

[U62] PHP：日期对象
来源：http://dai.yfazqb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eei.yuxming.cn

[U63] PHP：文件读写
来源：http://ick.epnwcf.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hgj.birdmap.top

[U64] PHP：目录遍历
来源：http://heb.yj20258.top

glob("dir/*.php");  scandir("dir");
来源：http://rgu.jyoumei.cn

[U65] PHP：会话
来源：http://xmu.yj202588.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rvz.cqqwz.cn

[U66] PHP：设置 Cookie
来源：http://ngs.yanxiufei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eer.cucudq.cn

[U67] PHP：处理文件上传
来源：http://jjf.shzxlz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://eqy.sufxvd.cn

[U68] PHP：PDO 连接
来源：http://vob.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://aqt.havefunace.top

[U69] PHP：PDO 预处理
来源：http://wpp.ivvv.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wcs.xziqi.cn

[U70] PHP：PDO 事务
来源：http://gsa.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bcb.zycfv.cn

[U71] PHP：抛出异常
来源：http://zdd.gaohongyu789.top

throw new RuntimeException("失败", 500);
来源：http://viv.smart0.xyz

[U72] PHP：写错误日志
来源：http://fod.tanke756.top

error_log("失败: " . $e->getMessage());
来源：http://noj.smart0.xyz

[U73] PHP：读取 ini 配置
来源：http://mdk.svipenyu.cn

parse_ini_file("config.ini", true)
来源：http://hfi.bjfxy.top

[U74] PHP：读取环境变量
来源：http://irv.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://zsv.chenzaomai.com

[U75] PHP：依赖注入
来源：http://jag.fehbvm.com

composer require psr/container
来源：http://zye.shangyingyoupin.top

[U76] PHP：简单路由
来源：http://dno.zdbjq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://auy.dashuyun.cn

[U77] PHP：模板渲染
来源：http://iws.yuxming.cn

composer require twig/twig
来源：http://hyi.pengpengdd.cyou

[U78] PHP：单元测试
来源：http://ltm.xziqi.cn

composer require --dev phpunit/phpunit
来源：http://fgk.cashguo.top

[U79] PHP：静态分析
来源：http://prb.vehdjk.com

composer require --dev phpstan/phpstan
来源：http://vnu.yvedp.cn

[U80] PHP：代码规范修复
来源：http://hsl.fktsv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ruh.xuanzx.com

[U81] JS：初始化项目
来源：http://wyt.tian-w.cn

npm init -y;  npm i express
来源：http://goj.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://ltr.ppjwa.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ked.jinqigfzy.top

[U83] JS：ES Module 导入导出
来源：http://suv.yuanzhike.top

export const a = 1;  import { a } from "./m.js";
来源：http://zcc.yangfankeji.com

[U84] JS：CommonJS 写法
来源：http://ljo.aizwys.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ets.redwolf501.top

[U85] JS：可选链
来源：http://dyc.jinyuanbaomall.cn

a?.b?.c
来源：http://uoi.ydjk.org.cn

[U86] JS：空值合并
来源：http://pnp.zhaomingkeji.xyz

a ?? b
来源：http://vek.bbcook.cn

[U87] JS：解构默认值
来源：http://rwr.dashuyun.cn

const { a = 1, b = 2 } = obj;
来源：http://uad.xuanzx.com

[U88] JS：对象展开合并
来源：http://jnz.pengpengdd.cyou

{ ...a, ...b }
来源：http://mbu.yvedp.cn

[U89] JS：数组去重
来源：http://zxx.jlsjyb.cn

[...new Set(arr)]
来源：http://jsb.jinqigfzy.top

[U90] JS：数字数组排序
来源：http://ebt.aizwys.cn

[...arr].sort((a, b) => a - b)
来源：http://hae.jianghu66.top

[U91] JS：对象键值遍历
来源：http://twk.pengpengdd.cyou

Object.entries(obj).forEach(([k, v]) => {});
来源：http://thu.jqgufenzy.top

[U92] JS：深拷贝
来源：http://xou.yanxiufei.cn

structuredClone(obj)
来源：http://aix.zhengqikj.top

[U93] JS：模板字符串
来源：http://bna.guowangkeji.top

`共 ${n} 条`
来源：http://pud.vehdjk.com

[U94] JS：箭头函数
来源：http://mkq.epnwcf.com

const double = x => x * 2;
来源：http://yfx.zhixingplan.top

[U95] JS：Promise 包装
来源：http://wvg.sufxvd.cn

new Promise((resolve, reject) => {})
来源：http://vgd.fzhhl.top

[U96] JS：async/await 与异常
来源：http://oyl.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cpf.c1oappe.top

[U97] JS：并发请求
来源：http://jjv.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://kli.jyoumei.cn

[U98] JS：fetch 带 JSON
来源：http://lat.nanxuanxn.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tnr.svipenyu.cn

[U99] JS：事件监听
来源：http://xqp.9152youxi.cn

el.addEventListener("click", e => {})
来源：http://yiu.birdmap.top

[U100] JS：DOM 查询
来源：http://jrz.hnqzz.top

document.querySelector(".item")
来源：http://vmz.hfpthk.cn

[U101] JS：classList 操作
来源：http://nnf.vqdsnc.cn

el.classList.toggle("active")
来源：http://lyc.jinyuanbaomall.cn

[U102] JS：本地存储
来源：http://odf.shzxlz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vjd.jqgufenzy.top

[U103] JS：定时器
来源：http://kye.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hip.cashguo.top

[U104] JS：防抖
来源：http://cvm.svipenyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vsh.ydzc1.top

[U105] JS：节流
来源：http://lzy.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://psz.jqgufenzy.top

[U106] JS：日期格式化
来源：http://koq.quarkkingdee.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hiq.wangshuangyany.cn

[U107] JS：数字千分位
来源：http://okl.jlsjyb.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nle.xingfuxueyuan.xyz

[U108] JS：随机整数
来源：http://vbi.52xcode.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://flf.sysykeji.top

[U109] JS：数组分组
来源：http://kyw.hnqzz.top

Object.groupBy(arr, x => x.type)
来源：http://eki.pycfn.com

[U110] JS：数组分块
来源：http://mrx.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aqj.yuxming.cn

[U111] JS：对象转 Map
来源：http://prv.fzhhl.top

new Map(Object.entries(obj))
来源：http://yrq.haohaochexian.top

[U112] JS：字符串补位
来源：http://vnq.jyoumei.cn

"7".padStart(3, "0")
来源：http://odv.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://tma.yfazqb.com

s.replaceAll("a", "b")
来源：http://gbr.feifeiyinyue.top

[U114] JS：JSON 深比较
来源：http://jrj.0kj1m.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ruy.sjlbkw.cn

[U115] JS：生成 UUID
来源：http://wdd.hfpthk.cn

crypto.randomUUID()
来源：http://fkr.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://qjc.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://bjq.zhijiandao.cn

[U117] JS：单元测试
来源：http://qnr.jinqigufen.top

npm i -D vitest;  npx vitest
来源：http://yxe.wangdashe.top

[U118] JS：开发服务器
来源：http://phq.ydzc1.top

npm i -D vite;  npx vite
来源：http://qlw.jinghuilouyu.cn

[U119] JS：生产构建
来源：http://grc.hesvh.cn

npx vite build
来源：http://tbb.ivvv.top

[U120] JS：读取环境变量（Vite）
来源：http://hxe.52xcode.cn

import.meta.env.VITE_API_URL
来源：http://vgo.cdnleiting.top

================================================================================
来源：http://fbp.cdnleiting.top

统计汇总
来源：http://tfz.yvedp.cn

================================================================================
来源：http://rln.dianchejie.cn

按语言统计（条）：
来源：http://oun.dashuyun.cn

Python ......... 252
来源：http://kax.cqqwz.cn

PHP ............ 252
来源：http://bcs.pycfn.com

JavaScript ..... 252
来源：http://znd.316326.xyz

TypeScript ..... 212
来源：http://weq.wangdashe.top

Java ........... 212
来源：http://fgk.xylfe.cn

Go ............. 212
来源：http://cfc.nwbrower.top

Ruby ........... 212
来源：http://mky.svipenyu.cn

C# ............. 212
来源：http://ugr.zhoulong.xyz

C .............. 30
来源：http://pwb.wangdashe.top

C++ ............ 30
来源：http://jhu.jqgufenzy.top

SQL ............ 90
来源：http://qdq.jianghu66.top

Bash ........... 80
来源：http://uug.zdbjq.cn

Kotlin ......... 15
来源：http://ypm.zhoulong.xyz

Swift .......... 15
来源：http://old.yuanzhike.top

Lua ............ 10
来源：http://ouc.ywan-chungtsiang.top

Perl ........... 10
来源：http://jwh.shuidangran.top

Scala .......... 10
来源：http://fzt.cqqwz.cn

------------------------------------
来源：http://ywc.bbcook.cn

合计 ........... 2106 条
来源：http://vza.yongpay.top

按章节统计：
来源：http://abh.jiagoushi.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sec.xylfe.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tjn.ivvv.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://efs.ywan-chungtsiang.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mwl.yongpay.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gpb.xinyue.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://quj.yonumen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://koh.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lzf.jiagoushi.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cbf.snrcjt.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uxf.wangshuangyany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://shk.zhaomingkeji.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ffr.shanyushiyangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hre.wangdashe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xgy.ctjpmb.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kco.xuetiantiany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mwc.shuidangran.top

Q SQL 专题                              90
来源：http://gnv.yuanzhike.top

R Bash 专题                             80
来源：http://xgg.bjfxy.top

S C / C++ 专题                          60
来源：http://ztt.ybcxt.top

T 其他语言补充                          60
来源：http://mma.bjfxy.top

U 高频实用片段                         120
来源：http://teb.jlsjyb.cn

------------------------------------
来源：http://lyr.ehwqpu.com

合计                                  2106 条
来源：http://zah.wangdashe.top

--------------------------------------------------------------------------------
来源：http://dsz.mhx1999.top

使用提醒
来源：http://umk.aizwys.cn

--------------------------------------------------------------------------------
来源：http://mdt.zycfv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zvg.xingfuxueyuan.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ncj.tian-w.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rae.jqgufenzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jvb.hongshengwenyu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tbv.redwolf501.top

—— 文件结束 ——
来源：http://uvi.tianlin.xyz

================================================================================
来源：http://yst.nwbrower.top

程序语言常见例子速查手册（2024 版）
来源：http://bjk.dashuyun.cn

Common Programming Examples Cheat Book
来源：http://yzx.aizwys.cn

================================================================================
来源：http://sxa.zhijiandao.cn


<!-- 参考信息 -->