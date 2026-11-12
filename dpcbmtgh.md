代发 wailian999

case class User(name: String, age: Int)
来源：http://hrf.kuanghao11.cn

[T57] Scala：模式匹配
来源：http://voz.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://sxh.hysaishi.cn

[T58] Scala：函数定义
来源：http://wnp.yangfankeji.com

def add(a: Int, b: Int): Int = a + b
来源：http://rjm.hysaishi.cn

[T59] Scala：循环
来源：http://oqq.yfazqb.com

for (i <- 1 to 10) println(i)
来源：http://suj.pycfn.com

[T60] Scala：折叠
来源：http://muy.dashuyun.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hpv.yvedp.cn

================================================================================
来源：http://hru.gogol.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://spl.hysaishi.cn

================================================================================
来源：http://xar.sysykeji.top

[U01] Py：创建虚拟环境
来源：http://tat.cdnleiting.top

python -m venv .venv && source .venv/bin/activate
来源：http://ciy.jianghu66.top

[U02] Py：导出 / 安装依赖
来源：http://ndw.xuetiantiany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vty.epnwcf.com

[U03] Py：加载 .env 配置
来源：http://igz.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jlz.dashuyun.cn

[U04] Py：变量调试打印
来源：http://rmz.hywenlv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://waj.xziqi.cn

[U05] Py：列表去重且保序
来源：http://ynb.jinyuanbaomall.cn

list(dict.fromkeys(arr))
来源：http://bma.birdmap.top

[U06] Py：合并两个字典
来源：http://dpd.9152youxi.cn

{**a, **b}
来源：http://dzi.yj20258888.top

[U07] Py：反转字典键值
来源：http://urw.sufxvd.cn

{v: k for k, v in d.items()}
来源：http://suy.quarkkingdee.top

[U08] Py：展平二维列表
来源：http://zfc.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://qmz.pycfn.com

[U09] Py：字典取最大值的键
来源：http://eum.aibaodan.cn

max(d, key=d.get)
来源：http://nmf.hywenlv.cn

[U10] Py：按值排序字典
来源：http://yro.yueranfly.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gkn.hnqzz.top

[U11] Py：生成器表达式
来源：http://ela.xziqi.cn

(x * 2 for x in arr)
来源：http://knm.zhengqikj.top

[U12] Py：取出现最多的 3 个元素
来源：http://oiu.0kj1m.cn

Counter(arr).most_common(3)
来源：http://ago.cheryme.top

[U13] Py：固定长度队列
来源：http://ppy.fanxiaobao.xyz

deque(maxlen=10)
来源：http://fmx.tanke756.top

[U14] Py：分组收集到列表
来源：http://gph.guannengcc.top

defaultdict(list)
来源：http://auo.9152youxi.cn

[U15] Py：高精度计时
来源：http://iyu.hammf.cn

t = time.perf_counter()
来源：http://toz.andypj.xyz

[U16] Py：命令行参数解析
来源：http://jbf.ydzc1.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wkw.yuanzhike.top

[U17] Py：初始化日志
来源：http://mbp.yfazqb.com

logging.basicConfig(level=logging.INFO)
来源：http://yvd.hcnkem.com

[U18] Py：预编译正则
来源：http://ird.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://cyz.ydzc1.top

[U19] Py：正则替换带回调
来源：http://wxn.guowangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pue.chenjidiqi.icu

[U20] Py：缓存函数结果
来源：http://kee.zhijiandao.cn

@functools.lru_cache(maxsize=None)
来源：http://uan.ydzc1.top

[U21] Py：自定义上下文管理器
来源：http://yrd.hysaishi.cn

@contextlib.contextmanager
来源：http://vjr.yueranfly.top

[U22] Py：矩阵转置
来源：http://pbv.ydzc1.top

list(zip(*m))
来源：http://rod.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://goi.xuetiantiany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://djs.cdnleiting.top

[U24] Py：路径操作
来源：http://vlm.epnwcf.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qpk.vehdjk.com

[U25] Py：CSV 按字典读
来源：http://lss.tarul.cn

csv.DictReader(f)
来源：http://pzz.bjfxy.top

[U26] Py：并发下载
来源：http://gvm.ehwqpu.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qfo.nwbrower.top

[U27] Py：异步 HTTP
来源：http://ydb.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://jlj.shzxlz.cn

[U28] Py：类型别名
来源：http://rxj.chenlongwang.top

UserId = int
来源：http://mcd.gzhubu.top

[U29] Py：属性校验
来源：http://rqo.vehdjk.com

@property 与 @x.setter 配合
来源：http://hwu.haohaochexian.top

[U30] Py：数据类
来源：http://chl.tanke756.top

@dataclass(slots=True)
来源：http://vwm.aibaodan.cn

[U31] Py：单测
来源：http://adl.cheryme.top

python -m pytest -q
来源：http://qwj.jinqigfzy.top

[U32] Py：代码格式化
来源：http://gsi.ppjwa.cn

ruff format . && ruff check --fix .
来源：http://tlt.jinqigfzy.top

[U33] Py：打包发布
来源：http://eoi.cashguo.top

python -m build  （依赖 pyproject.toml）
来源：http://arl.hysaishi.cn

[U34] Py：判断编码
来源：http://jli.guannengcc.top

chardet.detect(raw)
来源：http://qzy.yuxming.cn

[U35] Py：发送邮件
来源：http://qqc.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://boh.ybcxt.top

[U36] Py：定时任务
来源：http://jvk.kuanghao11.cn

schedule.every(10).minutes.do(job)
来源：http://aik.shanyushiyangtech.top

[U37] Py：读写 Excel
来源：http://zcc.snrcjt.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jby.aizwys.cn

[U38] Py：获取脚本所在目录
来源：http://wbv.pycfn.com

Path(__file__).resolve().parent
来源：http://rym.jianghu66.top

[U39] Py：判断是否在交互环境
来源：http://pof.jinqigfzy.top

sys.stdout.isatty()
来源：http://wcx.shuidangran.top

[U40] Py：打印到标准错误
来源：http://pwc.0kj1m.cn

print("err", file=sys.stderr)
来源：http://kua.xingfuxueyuan.xyz

[U41] PHP：初始化 Composer 项目
来源：http://nug.tian-w.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qdn.yanxiufei.cn

[U42] PHP：PSR-4 自动加载
来源：http://cja.jianghu66.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://txh.tarul.cn

[U43] PHP：声明命名空间
来源：http://pcm.hnqzz.top

namespace App\Http;
来源：http://qqn.zhixingplan.top

[U44] PHP：开启严格类型
来源：http://jou.gogol.net.cn

declare(strict_types=1);
来源：http://yda.xinyue.icu

[U45] PHP：类型声明与返回类型
来源：http://har.hnxiangtu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xrr.gzhubu.top

[U46] PHP：可空类型
来源：http://zls.jqgfzy.top

?string $name = null
来源：http://pei.xingfuxueyuan.xyz

[U47] PHP：联合类型
来源：http://rim.dashuyun.cn

int|string $id
来源：http://vic.gaohongyu789.top

[U48] PHP：纯枚举
来源：http://gzd.daria6918.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tvr.chenlongwang.top

[U49] PHP：只读属性
来源：http://fyu.jianghu66.top

public readonly string $name
来源：http://tvx.haohaochexian.top

[U50] PHP：构造器属性提升
来源：http://ptq.sysykeji.top

public function __construct(private int $id) {}
来源：http://okt.hcnkem.com

[U51] PHP：数组解构
来源：http://ude.xziqi.cn

[$a, $b] = $arr;
来源：http://oac.jyoumei.cn

[U52] PHP：箭头函数
来源：http://fpd.9152youxi.cn

$double = fn($x) => $x * 2;
来源：http://zek.iojbl.cn

[U53] PHP：空合并运算符
来源：http://aos.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://ryz.zhijiandao.cn

[U54] PHP：空安全调用
来源：http://exy.316326.xyz

$obj?->method()
来源：http://xvd.shuidangran.top

[U55] PHP：match 表达式
来源：http://mes.havefunace.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://epw.zdqjudy.top

[U56] PHP：命名参数
来源：http://idh.jinqigfzy.top

f(a: 1, b: 2)
来源：http://vut.yongpay.top

[U57] PHP：字符串插值
来源：http://zwa.cheryme.top

"值: {$a}"
来源：http://omc.yuxming.cn

[U58] PHP：数组三件套
来源：http://nir.ctjpmb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zci.zhaomingkeji.xyz

[U59] PHP：自定义排序
来源：http://skt.c1oappe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jnq.meibo888.top

[U60] PHP：JSON 编解码
来源：http://bfw.zdbjq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ndm.chenjidiqi.icu

[U61] PHP：正则
来源：http://xon.zhiwuduotai.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zqk.sweek.top

[U62] PHP：日期对象
来源：http://uqd.tian-w.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zxq.yanxiufei.cn

[U63] PHP：文件读写
来源：http://ihu.shanyushiyangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nyk.redwolf501.top

[U64] PHP：目录遍历
来源：http://fuq.fengsongda.top

glob("dir/*.php");  scandir("dir");
来源：http://tgv.9152youxi.cn

[U65] PHP：会话
来源：http://etb.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zew.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://vgg.sjlbkw.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aho.iojbl.cn

[U67] PHP：处理文件上传
来源：http://rzw.hywenlv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://elz.52xcode.cn

[U68] PHP：PDO 连接
来源：http://ixy.316326.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wvt.zhoulong.xyz

[U69] PHP：PDO 预处理
来源：http://xeq.gogol.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cvw.tanke756.top

[U70] PHP：PDO 事务
来源：http://adb.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bfu.jqgufenzy.top

[U71] PHP：抛出异常
来源：http://ege.daria6918.cn

throw new RuntimeException("失败", 500);
来源：http://atr.zhengqikj.top

[U72] PHP：写错误日志
来源：http://rmy.ydzc1.top

error_log("失败: " . $e->getMessage());
来源：http://jvu.52xcode.cn

[U73] PHP：读取 ini 配置
来源：http://fah.nanxuanxn.top

parse_ini_file("config.ini", true)
来源：http://imw.fktsv.cn

[U74] PHP：读取环境变量
来源：http://out.jianghu66.top

getenv("APP_ENV") ?: "production"
来源：http://uqp.yongpay.top

[U75] PHP：依赖注入
来源：http://bov.jqgfzy.top

composer require psr/container
来源：http://chs.yongpay.top

[U76] PHP：简单路由
来源：http://vtb.gotoacloud.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://art.hnxiangtu.top

[U77] PHP：模板渲染
来源：http://gal.mhx1999.top

composer require twig/twig
来源：http://ckx.dianchejie.cn

[U78] PHP：单元测试
来源：http://wzv.hnxiangtu.top

composer require --dev phpunit/phpunit
来源：http://vwc.snrcjt.cn

[U79] PHP：静态分析
来源：http://uyq.jinqigfzy.top

composer require --dev phpstan/phpstan
来源：http://ztx.hysaishi.cn

[U80] PHP：代码规范修复
来源：http://epv.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://otd.nwbrower.top

[U81] JS：初始化项目
来源：http://pxc.sufxvd.cn

npm init -y;  npm i express
来源：http://xno.zhoulong.xyz

[U82] JS：package.json 脚本
来源：http://myr.shanyushiyangtech.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://udf.bjfxy.top

[U83] JS：ES Module 导入导出
来源：http://ycx.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://kor.zhijiandao.cn

[U84] JS：CommonJS 写法
来源：http://kto.xziqi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fpo.ctjpmb.com

[U85] JS：可选链
来源：http://ryq.smart0.xyz

a?.b?.c
来源：http://uay.vqdsnc.cn

[U86] JS：空值合并
来源：http://jgv.fzhhl.top

a ?? b
来源：http://ban.uphjek.com

[U87] JS：解构默认值
来源：http://kmr.ybcxt.top

const { a = 1, b = 2 } = obj;
来源：http://afy.yongpay.top

[U88] JS：对象展开合并
来源：http://mbl.ydzc1.top

{ ...a, ...b }
来源：http://vor.yfazqb.com

[U89] JS：数组去重
来源：http://ukc.haohaochexian.top

[...new Set(arr)]
来源：http://eov.pycfn.com

[U90] JS：数字数组排序
来源：http://rht.tanke756.top

[...arr].sort((a, b) => a - b)
来源：http://lwa.jqgufenzy.top

[U91] JS：对象键值遍历
来源：http://buh.yangfankeji.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lrx.zhengqikj.top

[U92] JS：深拷贝
来源：http://rdl.ybcxt.top

structuredClone(obj)
来源：http://nou.tarul.cn

[U93] JS：模板字符串
来源：http://rru.aibaodan.cn

`共 ${n} 条`
来源：http://xof.havefunace.top

[U94] JS：箭头函数
来源：http://fld.fengsongda.top

const double = x => x * 2;
来源：http://awn.jiagoushi.top

[U95] JS：Promise 包装
来源：http://lhe.hywenlv.cn

new Promise((resolve, reject) => {})
来源：http://lsk.fengsongda.top

[U96] JS：async/await 与异常
来源：http://oye.haohaochexian.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gkc.chenlongwang.top

[U97] JS：并发请求
来源：http://mlo.fanxiaobao.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://nzz.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://eia.cdnleiting.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hvx.iojbl.cn

[U99] JS：事件监听
来源：http://ytk.xingfuxueyuan.xyz

el.addEventListener("click", e => {})
来源：http://mwn.ivvv.top

[U100] JS：DOM 查询
来源：http://xqy.redwolf501.top

document.querySelector(".item")
来源：http://fmn.zdbjq.cn

[U101] JS：classList 操作
来源：http://tut.tian-w.cn

el.classList.toggle("active")
来源：http://vrn.52xcode.cn

[U102] JS：本地存储
来源：http://clh.epnwcf.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://uvj.sjlbkw.cn

[U103] JS：定时器
来源：http://dya.zycfv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lfg.hesvh.cn

[U104] JS：防抖
来源：http://uer.vehdjk.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ges.fengsongda.top

[U105] JS：节流
来源：http://ykx.sufxvd.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://buc.jinqigfzy.top

[U106] JS：日期格式化
来源：http://xiq.quarkkingdee.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vhb.yuanzhike.top

[U107] JS：数字千分位
来源：http://ygm.sjlbkw.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mvz.yueranfly.top

[U108] JS：随机整数
来源：http://pmm.ywan-chungtsiang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bjy.9152youxi.cn

[U109] JS：数组分组
来源：http://nbr.wangdashe.top

Object.groupBy(arr, x => x.type)
来源：http://rmt.bjfxy.top

[U110] JS：数组分块
来源：http://oys.fehbvm.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://btj.yonumen.top

[U111] JS：对象转 Map
来源：http://ydc.ybcxt.top

new Map(Object.entries(obj))
来源：http://yur.tarul.cn

[U112] JS：字符串补位
来源：http://rgo.redwolf501.top

"7".padStart(3, "0")
来源：http://for.jinyuanbaomall.cn

[U113] JS：正则替换全部
来源：http://urk.fehbvm.com

s.replaceAll("a", "b")
来源：http://fam.uphjek.com

[U114] JS：JSON 深比较
来源：http://zlc.sxryk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ajq.sufxvd.cn

[U115] JS：生成 UUID
来源：http://toh.cashguo.top

crypto.randomUUID()
来源：http://jmg.hcnkem.com

[U116] JS：类型检查（JSDoc）
来源：http://ijt.ydzc1.top

/** @param {string} name */ function f(name) {}
来源：http://tcc.smart0.xyz

[U117] JS：单元测试
来源：http://tan.hammf.cn

npm i -D vitest;  npx vitest
来源：http://ceu.ehwqpu.com

[U118] JS：开发服务器
来源：http://bal.kuanghao11.cn

npm i -D vite;  npx vite
来源：http://rlm.jqgufenzy.top

[U119] JS：生产构建
来源：http://zos.fzhhl.top

npx vite build
来源：http://ezb.sjlbkw.cn

[U120] JS：读取环境变量（Vite）
来源：http://yjg.xylfe.cn

import.meta.env.VITE_API_URL
来源：http://oiv.jinyuanbaomall.cn

================================================================================
来源：http://gdk.cdnleiting.top

统计汇总
来源：http://jnt.jianghu66.top

================================================================================
来源：http://wgs.ywan-chungtsiang.top

按语言统计（条）：
来源：http://ylg.iojbl.cn

Python ......... 252
来源：http://sip.zhixingplan.top

PHP ............ 252
来源：http://swv.sufxvd.cn

JavaScript ..... 252
来源：http://rpa.316326.xyz

TypeScript ..... 212
来源：http://vhe.hfpthk.cn

Java ........... 212
来源：http://rzx.aizwys.cn

Go ............. 212
来源：http://fqf.yueranfly.top

Ruby ........... 212
来源：http://tcq.yangfankeji.com

C# ............. 212
来源：http://gcz.snrcjt.cn

C .............. 30
来源：http://rhb.fengsongda.top

C++ ............ 30
来源：http://bpd.shuidangran.top

SQL ............ 90
来源：http://sip.ppjwa.cn

Bash ........... 80
来源：http://pmw.zycfv.cn

Kotlin ......... 15
来源：http://fvk.yvedp.cn

Swift .......... 15
来源：http://bec.xinyue.icu

Lua ............ 10
来源：http://gup.dashuyun.cn

Perl ........... 10
来源：http://ypq.shangyingyoupin.top

Scala .......... 10
来源：http://qor.316326.xyz

------------------------------------
来源：http://ymk.tarul.cn

合计 ........... 2106 条
来源：http://gxa.feifeiyinyue.top

按章节统计：
来源：http://fkv.hnxiangtu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kgx.yongpay.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://per.svipenyu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lbx.gogol.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zsl.jinqigfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qwi.tarul.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hge.ybcxt.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kel.kuanghao11.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pbl.hysaishi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://unn.birdmap.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vmm.ydjk.org.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hyf.tanke756.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kxc.9152youxi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nct.hywenlv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ucc.9152youxi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yli.hongshengwenyu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xys.guannengcc.top

Q SQL 专题                              90
来源：http://rjr.ywan-chungtsiang.top

R Bash 专题                             80
来源：http://duc.nanxuanxn.top

S C / C++ 专题                          60
来源：http://ykz.cashguo.top

T 其他语言补充                          60
来源：http://qwd.ybcxt.top

U 高频实用片段                         120
来源：http://yrf.shanyushiyangkeji.top

------------------------------------
来源：http://czg.yj20258888.top

合计                                  2106 条
来源：http://dhk.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://qir.wangdashe.top


<!-- 参考信息 -->