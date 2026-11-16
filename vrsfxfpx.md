代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bgm.hysaishi.cn

================================================================================
来源：http://mim.hywenlv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sgz.jinghuilouyu.cn

================================================================================
来源：http://cev.ywan-chungtsiang.top

[U01] Py：创建虚拟环境
来源：http://mgv.fktsv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ilo.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://ofy.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ehv.ywan-chungtsiang.top

[U03] Py：加载 .env 配置
来源：http://rkb.yangfankeji.com

from dotenv import load_dotenv; load_dotenv()
来源：http://tuk.cucudq.cn

[U04] Py：变量调试打印
来源：http://zpb.xylfe.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nmi.cdnleiting.top

[U05] Py：列表去重且保序
来源：http://ghn.havefunace.top

list(dict.fromkeys(arr))
来源：http://gsz.shuidangran.top

[U06] Py：合并两个字典
来源：http://xof.hesvh.cn

{**a, **b}
来源：http://azh.dashuyun.cn

[U07] Py：反转字典键值
来源：http://pkd.wangdashe.top

{v: k for k, v in d.items()}
来源：http://flu.daxiang520.top

[U08] Py：展平二维列表
来源：http://qjz.yj202588.top

[y for x in nested for y in x]
来源：http://hcp.xuanzx.com

[U09] Py：字典取最大值的键
来源：http://ice.yj20258888.top

max(d, key=d.get)
来源：http://pdv.ctjpmb.com

[U10] Py：按值排序字典
来源：http://thc.xuetiantiany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://drc.zhengqikj.top

[U11] Py：生成器表达式
来源：http://tig.gzhubu.top

(x * 2 for x in arr)
来源：http://vho.hnqzz.top

[U12] Py：取出现最多的 3 个元素
来源：http://zdr.xinyue.icu

Counter(arr).most_common(3)
来源：http://pbv.yangfankeji.com

[U13] Py：固定长度队列
来源：http://pge.chenzaomai.com

deque(maxlen=10)
来源：http://wwt.cheryme.top

[U14] Py：分组收集到列表
来源：http://zil.shzxlz.cn

defaultdict(list)
来源：http://iyd.ehwqpu.com

[U15] Py：高精度计时
来源：http://eyh.fengsongda.top

t = time.perf_counter()
来源：http://eyb.zhijiandao.cn

[U16] Py：命令行参数解析
来源：http://knk.daxiang520.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vfe.jianghu66.top

[U17] Py：初始化日志
来源：http://uxu.yuanzhike.top

logging.basicConfig(level=logging.INFO)
来源：http://urj.fktsv.cn

[U18] Py：预编译正则
来源：http://mvs.fehbvm.com

pat = re.compile(r"\d+")
来源：http://hvy.feifeiyinyue.top

[U19] Py：正则替换带回调
来源：http://tsj.fengsongda.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wlx.fehbvm.com

[U20] Py：缓存函数结果
来源：http://utx.mhx1999.top

@functools.lru_cache(maxsize=None)
来源：http://gtf.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://atv.jyoumei.cn

@contextlib.contextmanager
来源：http://gbp.0kj1m.cn

[U22] Py：矩阵转置
来源：http://zeb.guannengcc.top

list(zip(*m))
来源：http://fma.sufxvd.cn

[U23] Py：分块读取大文件
来源：http://uju.feifeiyinyue.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dmn.zhixingplan.top

[U24] Py：路径操作
来源：http://cfe.nanxinkj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sgu.cdnleiting.top

[U25] Py：CSV 按字典读
来源：http://aia.yueranfly.top

csv.DictReader(f)
来源：http://zsa.tian-w.cn

[U26] Py：并发下载
来源：http://afx.zhaomingkeji.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zsj.yonumen.top

[U27] Py：异步 HTTP
来源：http://taj.zhaomingkeji.xyz

aiohttp.ClientSession() 配合 async with
来源：http://qyn.zhoulong.xyz

[U28] Py：类型别名
来源：http://rte.yvedp.cn

UserId = int
来源：http://loz.wangshuangyany.cn

[U29] Py：属性校验
来源：http://kxu.hcnkem.com

@property 与 @x.setter 配合
来源：http://eke.yj202588.top

[U30] Py：数据类
来源：http://gmo.fzhhl.top

@dataclass(slots=True)
来源：http://yfo.feifeiyinyue.top

[U31] Py：单测
来源：http://cwz.hysaishi.cn

python -m pytest -q
来源：http://mmq.aizwys.cn

[U32] Py：代码格式化
来源：http://ttn.yueranfly.top

ruff format . && ruff check --fix .
来源：http://abx.jiagoushi.top

[U33] Py：打包发布
来源：http://red.316326.xyz

python -m build  （依赖 pyproject.toml）
来源：http://lzv.daxiang520.top

[U34] Py：判断编码
来源：http://fff.aibaodan.cn

chardet.detect(raw)
来源：http://rfu.ehwqpu.com

[U35] Py：发送邮件
来源：http://ihb.c1oappe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://aia.yanxiufei.cn

[U36] Py：定时任务
来源：http://van.pengpengdd.cyou

schedule.every(10).minutes.do(job)
来源：http://sfc.nwbrower.top

[U37] Py：读写 Excel
来源：http://lbh.guowangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://abo.gzhubu.top

[U38] Py：获取脚本所在目录
来源：http://mrd.ehwqpu.com

Path(__file__).resolve().parent
来源：http://fnp.nanxinkj.top

[U39] Py：判断是否在交互环境
来源：http://yhb.daria6918.cn

sys.stdout.isatty()
来源：http://pos.vqdsnc.cn

[U40] Py：打印到标准错误
来源：http://kjf.smart0.xyz

print("err", file=sys.stderr)
来源：http://tnj.ppjwa.cn

[U41] PHP：初始化 Composer 项目
来源：http://sqp.mhx1999.top

composer init;  composer require guzzlehttp/guzzle
来源：http://sht.guannengcc.top

[U42] PHP：PSR-4 自动加载
来源：http://vey.wangdashe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ett.daria6918.cn

[U43] PHP：声明命名空间
来源：http://bgv.yj202588.top

namespace App\Http;
来源：http://dix.xylfe.cn

[U44] PHP：开启严格类型
来源：http://hqv.yj202588.top

declare(strict_types=1);
来源：http://kba.ywan-chungtsiang.top

[U45] PHP：类型声明与返回类型
来源：http://mlw.zdqjudy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://voj.cdnleiting.top

[U46] PHP：可空类型
来源：http://rbp.sweek.top

?string $name = null
来源：http://aht.xuanzx.com

[U47] PHP：联合类型
来源：http://iip.andypj.xyz

int|string $id
来源：http://mbd.jlsjyb.cn

[U48] PHP：纯枚举
来源：http://yql.c1oappe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aoo.iojbl.cn

[U49] PHP：只读属性
来源：http://akl.svipenyu.cn

public readonly string $name
来源：http://kkj.jinqigfzy.top

[U50] PHP：构造器属性提升
来源：http://sto.c1oappe.top

public function __construct(private int $id) {}
来源：http://odr.fanxiaobao.xyz

[U51] PHP：数组解构
来源：http://ytv.nanxuanxn.top

[$a, $b] = $arr;
来源：http://vqo.ehwqpu.com

[U52] PHP：箭头函数
来源：http://ggu.fzhhl.top

$double = fn($x) => $x * 2;
来源：http://aws.yj20258.top

[U53] PHP：空合并运算符
来源：http://phw.52xcode.cn

$v = $a ?? $b ?? "default";
来源：http://ujb.cqqwz.cn

[U54] PHP：空安全调用
来源：http://pcd.jinqigufen.top

$obj?->method()
来源：http://ubo.nwbrower.top

[U55] PHP：match 表达式
来源：http://qjg.hnqzz.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://des.mhx1999.top

[U56] PHP：命名参数
来源：http://pol.zhengqikj.top

f(a: 1, b: 2)
来源：http://sls.ybcxt.top

[U57] PHP：字符串插值
来源：http://nun.xylfe.cn

"值: {$a}"
来源：http://sce.nanxinkj.top

[U58] PHP：数组三件套
来源：http://hin.yongpay.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dhr.wangshuangyany.cn

[U59] PHP：自定义排序
来源：http://dsv.redwolf501.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vlo.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://zdl.ydjk.org.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dus.yueranfly.top

[U61] PHP：正则
来源：http://ttd.yonumen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bwq.feifeiyinyue.top

[U62] PHP：日期对象
来源：http://hge.hcnkem.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pjf.wangshuangyany.cn

[U63] PHP：文件读写
来源：http://ams.ctjpmb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kfz.gogol.net.cn

[U64] PHP：目录遍历
来源：http://kmy.yueranfly.top

glob("dir/*.php");  scandir("dir");
来源：http://jxf.ybcxt.top

[U65] PHP：会话
来源：http://fah.bjfxy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://sdt.quarkkingdee.top

[U66] PHP：设置 Cookie
来源：http://oii.jiagoushi.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jfr.jinghuilouyu.cn

[U67] PHP：处理文件上传
来源：http://dtr.yj20258.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wse.jyoumei.cn

[U68] PHP：PDO 连接
来源：http://pww.yfazqb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yti.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://zjp.nanxuanxn.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yaa.chenzaomai.com

[U70] PHP：PDO 事务
来源：http://cpq.zhoulong.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://syi.ivvv.top

[U71] PHP：抛出异常
来源：http://pay.52xcode.cn

throw new RuntimeException("失败", 500);
来源：http://yew.hnqzz.top

[U72] PHP：写错误日志
来源：http://zyr.c1oappe.top

error_log("失败: " . $e->getMessage());
来源：http://vzr.fanxiaobao.xyz

[U73] PHP：读取 ini 配置
来源：http://wgq.jinqigfzy.top

parse_ini_file("config.ini", true)
来源：http://xaq.chenlongwang.top

[U74] PHP：读取环境变量
来源：http://mpd.yj20258888.top

getenv("APP_ENV") ?: "production"
来源：http://wza.xinyue.icu

[U75] PHP：依赖注入
来源：http://brc.fzhhl.top

composer require psr/container
来源：http://pot.fanxiaobao.xyz

[U76] PHP：简单路由
来源：http://joa.snrcjt.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iij.jinghuilouyu.cn

[U77] PHP：模板渲染
来源：http://imi.hcnkem.com

composer require twig/twig
来源：http://rzy.zhijiandao.cn

[U78] PHP：单元测试
来源：http://qdz.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://zyf.zycfv.cn

[U79] PHP：静态分析
来源：http://zqu.cheryme.top

composer require --dev phpstan/phpstan
来源：http://xnj.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://scn.xinyue.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://jip.daxiang520.top

[U81] JS：初始化项目
来源：http://jda.mhx1999.top

npm init -y;  npm i express
来源：http://htg.zhongyouzk.top

[U82] JS：package.json 脚本
来源：http://pcp.yanxiufei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://axb.jinghuilouyu.cn

[U83] JS：ES Module 导入导出
来源：http://ktk.hnxiangtu.top

export const a = 1;  import { a } from "./m.js";
来源：http://wyt.yj20258.top

[U84] JS：CommonJS 写法
来源：http://mco.fehbvm.com

module.exports = { a };  const { a } = require("./m");
来源：http://frz.shanyushiyangkeji.top

[U85] JS：可选链
来源：http://ewq.fzhhl.top

a?.b?.c
来源：http://bnz.52xcode.cn

[U86] JS：空值合并
来源：http://kpa.chenlongwang.top

a ?? b
来源：http://fag.wangshuangyany.cn

[U87] JS：解构默认值
来源：http://lzq.hammf.cn

const { a = 1, b = 2 } = obj;
来源：http://btn.yvedp.cn

[U88] JS：对象展开合并
来源：http://vyr.hcnkem.com

{ ...a, ...b }
来源：http://mnf.gotoacloud.top

[U89] JS：数组去重
来源：http://bub.daria6918.cn

[...new Set(arr)]
来源：http://esq.hfpthk.cn

[U90] JS：数字数组排序
来源：http://lzo.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://cio.gogol.net.cn

[U91] JS：对象键值遍历
来源：http://fyn.jinqigufen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tbw.cheryme.top

[U92] JS：深拷贝
来源：http://vno.uphjek.com

structuredClone(obj)
来源：http://lpg.yvedp.cn

[U93] JS：模板字符串
来源：http://rpb.jinqigfzy.top

`共 ${n} 条`
来源：http://abw.yongpay.top

[U94] JS：箭头函数
来源：http://yer.jlsjyb.cn

const double = x => x * 2;
来源：http://ulo.zhixingplan.top

[U95] JS：Promise 包装
来源：http://lfk.fengsongda.top

new Promise((resolve, reject) => {})
来源：http://vva.guowangkeji.top

[U96] JS：async/await 与异常
来源：http://kuu.zdqjudy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://man.sxryk.cn

[U97] JS：并发请求
来源：http://vue.ivvv.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gdw.sysykeji.top

[U98] JS：fetch 带 JSON
来源：http://eka.wangshuangyany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://atf.aibaodan.cn

[U99] JS：事件监听
来源：http://gpi.pengpengdd.cyou

el.addEventListener("click", e => {})
来源：http://sif.xuanzx.com

[U100] JS：DOM 查询
来源：http://rod.uphjek.com

document.querySelector(".item")
来源：http://bsi.hysaishi.cn

[U101] JS：classList 操作
来源：http://xhv.tarul.cn

el.classList.toggle("active")
来源：http://cik.zhixingplan.top

[U102] JS：本地存储
来源：http://ccg.xingfuxueyuan.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://tli.hongshengwenyu.top

[U103] JS：定时器
来源：http://ofl.zhoulong.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pju.bjfxy.top

[U104] JS：防抖
来源：http://cam.mhx1999.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://die.ydzc1.top

[U105] JS：节流
来源：http://tbj.guannengcc.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pho.ehwqpu.com

[U106] JS：日期格式化
来源：http://wgb.vqdsnc.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qwb.tian-w.cn

[U107] JS：数字千分位
来源：http://oan.quarkkingdee.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://siq.ywan-chungtsiang.top

[U108] JS：随机整数
来源：http://tgw.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bww.jianghu66.top

[U109] JS：数组分组
来源：http://ztt.hcnkem.com

Object.groupBy(arr, x => x.type)
来源：http://tsi.sjlbkw.cn

[U110] JS：数组分块
来源：http://ema.ywan-chungtsiang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fth.daria6918.cn

[U111] JS：对象转 Map
来源：http://all.ehwqpu.com

new Map(Object.entries(obj))
来源：http://xtf.ywan-chungtsiang.top

[U112] JS：字符串补位
来源：http://tby.zhijiandao.cn

"7".padStart(3, "0")
来源：http://tgs.xziqi.cn

[U113] JS：正则替换全部
来源：http://rps.jianghu66.top

s.replaceAll("a", "b")
来源：http://rdg.epnwcf.com

[U114] JS：JSON 深比较
来源：http://bmw.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nmv.fengsongda.top

[U115] JS：生成 UUID
来源：http://czc.svipenyu.cn

crypto.randomUUID()
来源：http://nix.ydjk.org.cn

[U116] JS：类型检查（JSDoc）
来源：http://jbu.gzhubu.top

/** @param {string} name */ function f(name) {}
来源：http://rlq.havefunace.top

[U117] JS：单元测试
来源：http://umr.sweek.top

npm i -D vitest;  npx vitest
来源：http://ofi.epnwcf.com

[U118] JS：开发服务器
来源：http://sen.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://fvs.jyoumei.cn

[U119] JS：生产构建
来源：http://fwm.yj20258888.top

npx vite build
来源：http://uto.jyoumei.cn

[U120] JS：读取环境变量（Vite）
来源：http://yxm.zhiwuduotai.top

import.meta.env.VITE_API_URL
来源：http://vlt.jiagoushi.top

================================================================================
来源：http://wsd.yvedp.cn

统计汇总
来源：http://yaq.fengsongda.top

================================================================================
来源：http://oxg.jlsjyb.cn

按语言统计（条）：
来源：http://qwr.sjlbkw.cn

Python ......... 252
来源：http://aip.316326.xyz

PHP ............ 252
来源：http://frd.jqgfzy.top

JavaScript ..... 252
来源：http://ftl.hnqzz.top

TypeScript ..... 212
来源：http://ved.fengsongda.top

Java ........... 212
来源：http://zda.zhaomingkeji.xyz

Go ............. 212
来源：http://txb.pycfn.com

Ruby ........... 212
来源：http://izk.zdbjq.cn

C# ............. 212
来源：http://adf.xuanzx.com

C .............. 30
来源：http://dih.shanyushiyangkeji.top

C++ ............ 30
来源：http://vrw.haohaochexian.top

SQL ............ 90
来源：http://zte.0kj1m.cn

Bash ........... 80
来源：http://ydj.ivvv.top

Kotlin ......... 15
来源：http://yyz.gaohongyu789.top

Swift .......... 15
来源：http://gxg.ydzc1.top

Lua ............ 10
来源：http://yoi.ybcxt.top

Perl ........... 10
来源：http://dlj.quarkkingdee.top

Scala .......... 10
来源：http://wpy.jiagoushi.top

------------------------------------
来源：http://bbb.xuanzx.com

合计 ........... 2106 条
来源：http://gjp.yj20258.top

按章节统计：
来源：http://ofz.hnxiangtu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://msd.nanxuanxn.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rmv.shanyushiyangtech.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mqf.yuxming.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gig.zhoulong.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bxb.yj20258.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xeb.hammf.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rnk.ctjpmb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kht.yj20258.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fvs.jlsjyb.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yrz.uphjek.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zsb.chenlongwang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gdl.hongshengwenyu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gnn.aizwys.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mbt.0kj1m.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eon.hywenlv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hoz.cashguo.top

Q SQL 专题                              90
来源：http://guy.daxiang520.top

R Bash 专题                             80
来源：http://tjd.tanke756.top

S C / C++ 专题                          60
来源：http://cdl.cucudq.cn

T 其他语言补充                          60
来源：http://pjd.xylfe.cn

U 高频实用片段                         120
来源：http://rrs.zdbjq.cn

------------------------------------
来源：http://yll.meibo888.top

合计                                  2106 条
来源：http://tjz.redwolf501.top

--------------------------------------------------------------------------------
来源：http://lta.zhoulong.xyz

使用提醒
来源：http://byc.guannengcc.top

--------------------------------------------------------------------------------
来源：http://xqi.hywenlv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wto.bjfxy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ibf.mhx1999.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jvn.shuidangran.top

在旧版本上使用前请先确认语法支持情况。
来源：http://emg.fktsv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nii.zdbjq.cn

—— 文件结束 ——
来源：http://wua.chenzaomai.com


<!-- 参考信息 -->