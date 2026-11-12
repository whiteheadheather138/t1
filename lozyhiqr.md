代发 wailian999

case class User(name: String, age: Int)
来源：http://nhx.c1oappe.top

[T57] Scala：模式匹配
来源：http://ksg.gzhubu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://uoe.0kj1m.cn

[T58] Scala：函数定义
来源：http://zba.yongpay.top

def add(a: Int, b: Int): Int = a + b
来源：http://kzi.tianlin.xyz

[T59] Scala：循环
来源：http://jqt.ctjpmb.com

for (i <- 1 to 10) println(i)
来源：http://olq.zhengqikj.top

[T60] Scala：折叠
来源：http://kut.tanke756.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zjt.9152youxi.cn

================================================================================
来源：http://ion.cashguo.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sff.fengsongda.top

================================================================================
来源：http://qme.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://shu.hnxiangtu.top

python -m venv .venv && source .venv/bin/activate
来源：http://vti.xziqi.cn

[U02] Py：导出 / 安装依赖
来源：http://wqc.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xus.nanxinkj.top

[U03] Py：加载 .env 配置
来源：http://txy.shanyushiyangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://uye.nanxuanxn.top

[U04] Py：变量调试打印
来源：http://cqm.sxryk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gny.shangyingyoupin.top

[U05] Py：列表去重且保序
来源：http://xts.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://zgu.zycfv.cn

[U06] Py：合并两个字典
来源：http://isu.guannengcc.top

{**a, **b}
来源：http://lsk.jyoumei.cn

[U07] Py：反转字典键值
来源：http://ktp.redwolf501.top

{v: k for k, v in d.items()}
来源：http://cgp.xinyue.icu

[U08] Py：展平二维列表
来源：http://gaq.sysykeji.top

[y for x in nested for y in x]
来源：http://cfc.shuidangran.top

[U09] Py：字典取最大值的键
来源：http://xfg.ctjpmb.com

max(d, key=d.get)
来源：http://xgi.gaohongyu789.top

[U10] Py：按值排序字典
来源：http://boa.andypj.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gfj.pycfn.com

[U11] Py：生成器表达式
来源：http://gsj.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://gfd.nanxuanxn.top

[U12] Py：取出现最多的 3 个元素
来源：http://fke.yj20258888.top

Counter(arr).most_common(3)
来源：http://unl.sysykeji.top

[U13] Py：固定长度队列
来源：http://nzh.ctjpmb.com

deque(maxlen=10)
来源：http://mln.meibo888.top

[U14] Py：分组收集到列表
来源：http://xln.quarkkingdee.top

defaultdict(list)
来源：http://rov.zdqjudy.top

[U15] Py：高精度计时
来源：http://kgk.hfpthk.cn

t = time.perf_counter()
来源：http://hsx.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://zqq.vehdjk.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qbc.hfpthk.cn

[U17] Py：初始化日志
来源：http://vxr.iojbl.cn

logging.basicConfig(level=logging.INFO)
来源：http://fvx.shanyushiyangtech.top

[U18] Py：预编译正则
来源：http://hew.zhengqikj.top

pat = re.compile(r"\d+")
来源：http://pfe.ydzc1.top

[U19] Py：正则替换带回调
来源：http://zmt.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ror.cdnleiting.top

[U20] Py：缓存函数结果
来源：http://szg.birdmap.top

@functools.lru_cache(maxsize=None)
来源：http://jeh.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://lhf.fzhhl.top

@contextlib.contextmanager
来源：http://kow.smart0.xyz

[U22] Py：矩阵转置
来源：http://iuu.0kj1m.cn

list(zip(*m))
来源：http://dsh.pengpengdd.cyou

[U23] Py：分块读取大文件
来源：http://nks.quarkkingdee.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fsi.ctjpmb.com

[U24] Py：路径操作
来源：http://kbt.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nrz.zhiwuduotai.top

[U25] Py：CSV 按字典读
来源：http://jvi.zdbjq.cn

csv.DictReader(f)
来源：http://akp.sufxvd.cn

[U26] Py：并发下载
来源：http://wop.yj20258888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wyp.chenjidiqi.icu

[U27] Py：异步 HTTP
来源：http://evf.zhengqikj.top

aiohttp.ClientSession() 配合 async with
来源：http://zes.sjlbkw.cn

[U28] Py：类型别名
来源：http://tnz.zhixingplan.top

UserId = int
来源：http://hgg.cashguo.top

[U29] Py：属性校验
来源：http://fjh.aibaodan.cn

@property 与 @x.setter 配合
来源：http://hkq.zhongyouzk.top

[U30] Py：数据类
来源：http://xsz.nanxinkj.top

@dataclass(slots=True)
来源：http://bkt.zhixingplan.top

[U31] Py：单测
来源：http://qtr.iojbl.cn

python -m pytest -q
来源：http://ydm.epnwcf.com

[U32] Py：代码格式化
来源：http://ieb.kuanghao11.cn

ruff format . && ruff check --fix .
来源：http://bxi.52xcode.cn

[U33] Py：打包发布
来源：http://rnu.hnqzz.top

python -m build  （依赖 pyproject.toml）
来源：http://tqr.zhiwuduotai.top

[U34] Py：判断编码
来源：http://wrn.hnxiangtu.top

chardet.detect(raw)
来源：http://ylu.nanxinkj.top

[U35] Py：发送邮件
来源：http://oih.nanxuanxn.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nzo.feifeiyinyue.top

[U36] Py：定时任务
来源：http://zzw.chenzaomai.com

schedule.every(10).minutes.do(job)
来源：http://zng.ehwqpu.com

[U37] Py：读写 Excel
来源：http://osv.aizwys.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jup.zycfv.cn

[U38] Py：获取脚本所在目录
来源：http://vyb.chenlongwang.top

Path(__file__).resolve().parent
来源：http://zif.chenzaomai.com

[U39] Py：判断是否在交互环境
来源：http://bat.chenzaomai.com

sys.stdout.isatty()
来源：http://yri.9152youxi.cn

[U40] Py：打印到标准错误
来源：http://rpw.dianchejie.cn

print("err", file=sys.stderr)
来源：http://fmy.0kj1m.cn

[U41] PHP：初始化 Composer 项目
来源：http://umt.vehdjk.com

composer init;  composer require guzzlehttp/guzzle
来源：http://xap.jinqigufen.top

[U42] PHP：PSR-4 自动加载
来源：http://yrn.jiagoushi.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lsk.zhengqikj.top

[U43] PHP：声明命名空间
来源：http://hoq.jinghuilouyu.cn

namespace App\Http;
来源：http://tgh.fanxiaobao.xyz

[U44] PHP：开启严格类型
来源：http://fnk.jinqigfzy.top

declare(strict_types=1);
来源：http://yac.hongshengwenyu.top

[U45] PHP：类型声明与返回类型
来源：http://egr.zhixingplan.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://uvm.jinqigfzy.top

[U46] PHP：可空类型
来源：http://inl.jlsjyb.cn

?string $name = null
来源：http://dys.cqqwz.cn

[U47] PHP：联合类型
来源：http://xar.hesvh.cn

int|string $id
来源：http://jxl.jianghu66.top

[U48] PHP：纯枚举
来源：http://aqt.hnqzz.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kiu.zhaomingkeji.xyz

[U49] PHP：只读属性
来源：http://ure.xziqi.cn

public readonly string $name
来源：http://hez.shzxlz.cn

[U50] PHP：构造器属性提升
来源：http://jjy.jinyuanbaomall.cn

public function __construct(private int $id) {}
来源：http://qlz.cucudq.cn

[U51] PHP：数组解构
来源：http://mzn.wangshuangyany.cn

[$a, $b] = $arr;
来源：http://vhe.cqqwz.cn

[U52] PHP：箭头函数
来源：http://kyf.sxryk.cn

$double = fn($x) => $x * 2;
来源：http://yha.yj20258.top

[U53] PHP：空合并运算符
来源：http://vcp.316326.xyz

$v = $a ?? $b ?? "default";
来源：http://rgz.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://qbm.shangyingyoupin.top

$obj?->method()
来源：http://wik.dashuyun.cn

[U55] PHP：match 表达式
来源：http://poq.redwolf501.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xbv.hesvh.cn

[U56] PHP：命名参数
来源：http://mel.redwolf501.top

f(a: 1, b: 2)
来源：http://jzc.gaohongyu789.top

[U57] PHP：字符串插值
来源：http://ise.zhixingplan.top

"值: {$a}"
来源：http://uzs.fzhhl.top

[U58] PHP：数组三件套
来源：http://gzp.shanyushiyangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://prw.zdbjq.cn

[U59] PHP：自定义排序
来源：http://uql.xylfe.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://itk.jinqigufen.top

[U60] PHP：JSON 编解码
来源：http://xoi.yongpay.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mfy.yj20258888.top

[U61] PHP：正则
来源：http://dpd.tanke756.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://snb.jinghuilouyu.cn

[U62] PHP：日期对象
来源：http://hqo.yfazqb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://awd.cdnleiting.top

[U63] PHP：文件读写
来源：http://cpf.xylfe.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dom.yuxming.cn

[U64] PHP：目录遍历
来源：http://peo.sxryk.cn

glob("dir/*.php");  scandir("dir");
来源：http://byr.zhoulong.xyz

[U65] PHP：会话
来源：http://xgg.zhongyouzk.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hvu.tianlin.xyz

[U66] PHP：设置 Cookie
来源：http://tra.zhongyouzk.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qdy.aizwys.cn

[U67] PHP：处理文件上传
来源：http://nnr.jinqigufen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://osa.ctjpmb.com

[U68] PHP：PDO 连接
来源：http://nev.hongshengwenyu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bze.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://qdd.yanxiufei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ivs.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://eyy.havefunace.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://twm.dashuyun.cn

[U71] PHP：抛出异常
来源：http://erw.nanxinkj.top

throw new RuntimeException("失败", 500);
来源：http://kaw.jyoumei.cn

[U72] PHP：写错误日志
来源：http://ouh.jinqigfzy.top

error_log("失败: " . $e->getMessage());
来源：http://uye.jiagoushi.top

[U73] PHP：读取 ini 配置
来源：http://cpn.gogol.net.cn

parse_ini_file("config.ini", true)
来源：http://etl.yfazqb.com

[U74] PHP：读取环境变量
来源：http://ylr.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://cll.chenzaomai.com

[U75] PHP：依赖注入
来源：http://vrf.ybcxt.top

composer require psr/container
来源：http://gij.hesvh.cn

[U76] PHP：简单路由
来源：http://uiz.xuetiantiany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vvq.ydjk.org.cn

[U77] PHP：模板渲染
来源：http://hyo.yj20258888.top

composer require twig/twig
来源：http://mlr.redwolf501.top

[U78] PHP：单元测试
来源：http://iec.hywenlv.cn

composer require --dev phpunit/phpunit
来源：http://xbj.jinqigufen.top

[U79] PHP：静态分析
来源：http://fte.yonumen.top

composer require --dev phpstan/phpstan
来源：http://brj.zhijiandao.cn

[U80] PHP：代码规范修复
来源：http://kmp.yangfankeji.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://ypd.shuidangran.top

[U81] JS：初始化项目
来源：http://mdw.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://eih.xylfe.cn

[U82] JS：package.json 脚本
来源：http://twv.bbcook.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lli.ehwqpu.com

[U83] JS：ES Module 导入导出
来源：http://ems.fehbvm.com

export const a = 1;  import { a } from "./m.js";
来源：http://kum.hcnkem.com

[U84] JS：CommonJS 写法
来源：http://xgc.cashguo.top

module.exports = { a };  const { a } = require("./m");
来源：http://msl.ivvv.top

[U85] JS：可选链
来源：http://yht.0kj1m.cn

a?.b?.c
来源：http://doz.c1oappe.top

[U86] JS：空值合并
来源：http://uca.chenzaomai.com

a ?? b
来源：http://ums.hammf.cn

[U87] JS：解构默认值
来源：http://frp.cashguo.top

const { a = 1, b = 2 } = obj;
来源：http://xtn.vehdjk.com

[U88] JS：对象展开合并
来源：http://ltd.fktsv.cn

{ ...a, ...b }
来源：http://asm.wangshuangyany.cn

[U89] JS：数组去重
来源：http://ekl.c1oappe.top

[...new Set(arr)]
来源：http://plj.shanyushiyangtech.top

[U90] JS：数字数组排序
来源：http://yqn.cqqwz.cn

[...arr].sort((a, b) => a - b)
来源：http://enl.zdqjudy.top

[U91] JS：对象键值遍历
来源：http://gcp.zhiwuduotai.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mnw.zhoulong.xyz

[U92] JS：深拷贝
来源：http://ley.zhengqikj.top

structuredClone(obj)
来源：http://wam.jqgfzy.top

[U93] JS：模板字符串
来源：http://hzz.shzxlz.cn

`共 ${n} 条`
来源：http://hax.redwolf501.top

[U94] JS：箭头函数
来源：http://vlk.yj20258.top

const double = x => x * 2;
来源：http://tqg.yvedp.cn

[U95] JS：Promise 包装
来源：http://jmy.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://dxb.xingfuxueyuan.xyz

[U96] JS：async/await 与异常
来源：http://gwc.hongshengwenyu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nlt.tanke756.top

[U97] JS：并发请求
来源：http://uqz.zhijiandao.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://myk.smart0.xyz

[U98] JS：fetch 带 JSON
来源：http://rsf.hnxiangtu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qpz.shanyushiyangtech.top

[U99] JS：事件监听
来源：http://uki.xingfuxueyuan.xyz

el.addEventListener("click", e => {})
来源：http://kjk.dashuyun.cn

[U100] JS：DOM 查询
来源：http://dzc.chenlongwang.top

document.querySelector(".item")
来源：http://uvq.zycfv.cn

[U101] JS：classList 操作
来源：http://unx.gzhubu.top

el.classList.toggle("active")
来源：http://qdm.hcnkem.com

[U102] JS：本地存储
来源：http://mck.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ome.shanyushiyangkeji.top

[U103] JS：定时器
来源：http://aha.zycfv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lqb.zhoulong.xyz

[U104] JS：防抖
来源：http://mzu.vqdsnc.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xbk.0kj1m.cn

[U105] JS：节流
来源：http://rfq.xziqi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kfq.fehbvm.com

[U106] JS：日期格式化
来源：http://fvo.jqgufenzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sby.xinyue.icu

[U107] JS：数字千分位
来源：http://pvi.yanxiufei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mll.guannengcc.top

[U108] JS：随机整数
来源：http://smp.sxryk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jxb.hywenlv.cn

[U109] JS：数组分组
来源：http://ixv.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://pvu.ydzc1.top

[U110] JS：数组分块
来源：http://vhh.nanxinkj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wyi.fzhhl.top

[U111] JS：对象转 Map
来源：http://rul.havefunace.top

new Map(Object.entries(obj))
来源：http://auy.0kj1m.cn

[U112] JS：字符串补位
来源：http://qae.fanxiaobao.xyz

"7".padStart(3, "0")
来源：http://vsn.tanke756.top

[U113] JS：正则替换全部
来源：http://pkk.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://lco.yvedp.cn

[U114] JS：JSON 深比较
来源：http://aaq.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dzc.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://hup.ivvv.top

crypto.randomUUID()
来源：http://ehl.jinqigufen.top

[U116] JS：类型检查（JSDoc）
来源：http://ian.yj20258.top

/** @param {string} name */ function f(name) {}
来源：http://upq.birdmap.top

[U117] JS：单元测试
来源：http://zvk.shzxlz.cn

npm i -D vitest;  npx vitest
来源：http://riv.zycfv.cn

[U118] JS：开发服务器
来源：http://xse.iojbl.cn

npm i -D vite;  npx vite
来源：http://wxl.xylfe.cn

[U119] JS：生产构建
来源：http://sty.vqdsnc.cn

npx vite build
来源：http://ruz.zdqjudy.top

[U120] JS：读取环境变量（Vite）
来源：http://cqe.yvedp.cn

import.meta.env.VITE_API_URL
来源：http://yqr.guowangkeji.top

================================================================================
来源：http://lpb.zhijiandao.cn

统计汇总
来源：http://tbk.yongpay.top

================================================================================
来源：http://dvd.redwolf501.top

按语言统计（条）：
来源：http://zpo.zhixingplan.top

Python ......... 252
来源：http://hkx.fzhhl.top

PHP ............ 252
来源：http://rgk.snrcjt.cn

JavaScript ..... 252
来源：http://wgi.hnqzz.top

TypeScript ..... 212
来源：http://oiz.jyoumei.cn

Java ........... 212
来源：http://ezu.316326.xyz

Go ............. 212
来源：http://sgd.ywan-chungtsiang.top

Ruby ........... 212
来源：http://ddn.jinyuanbaomall.cn

C# ............. 212
来源：http://zko.jqgfzy.top

C .............. 30
来源：http://utl.0kj1m.cn

C++ ............ 30
来源：http://rfv.sxryk.cn

SQL ............ 90
来源：http://sbs.daxiang520.top

Bash ........... 80
来源：http://fju.yuanzhike.top

Kotlin ......... 15
来源：http://nig.andypj.xyz

Swift .......... 15
来源：http://bgo.xylfe.cn

Lua ............ 10
来源：http://cbt.pengpengdd.cyou

Perl ........... 10
来源：http://fnq.9152youxi.cn

Scala .......... 10
来源：http://pnh.fengsongda.top

------------------------------------
来源：http://anm.dianchejie.cn

合计 ........... 2106 条
来源：http://qil.ppjwa.cn

按章节统计：
来源：http://cgl.hnqzz.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uxr.ivvv.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zrp.jlsjyb.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xbi.uphjek.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yqb.cheryme.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://efq.xingfuxueyuan.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lnx.shuidangran.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dow.hnxiangtu.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qyl.cheryme.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ove.c1oappe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cvw.sysykeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kda.gaohongyu789.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gzs.epnwcf.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fhg.sufxvd.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dfr.tarul.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iaq.fengsongda.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qwe.nanxuanxn.top

Q SQL 专题                              90
来源：http://edg.zdqjudy.top

R Bash 专题                             80
来源：http://sxe.xingfuxueyuan.xyz

S C / C++ 专题                          60
来源：http://xic.c1oappe.top

T 其他语言补充                          60
来源：http://xcb.shanyushiyangtech.top

U 高频实用片段                         120
来源：http://gjs.jinqigufen.top

------------------------------------
来源：http://awl.hysaishi.cn

合计                                  2106 条
来源：http://qyk.yfazqb.com

--------------------------------------------------------------------------------
来源：http://qhq.zdbjq.cn


<!-- 参考信息 -->