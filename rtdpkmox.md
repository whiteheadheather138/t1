代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://gpk.sweek.top

[T55] Scala：集合过滤
来源：http://dtw.aibaodan.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cry.yj20258.top

[T56] Scala：样例类
来源：http://uei.quarkkingdee.top

case class User(name: String, age: Int)
来源：http://njr.mhx1999.top

[T57] Scala：模式匹配
来源：http://vai.tarul.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://irl.epnwcf.com

[T58] Scala：函数定义
来源：http://joh.nanxuanxn.top

def add(a: Int, b: Int): Int = a + b
来源：http://nko.shuidangran.top

[T59] Scala：循环
来源：http://dzj.tarul.cn

for (i <- 1 to 10) println(i)
来源：http://arq.zhongyouzk.top

[T60] Scala：折叠
来源：http://crw.jinghuilouyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wsi.zhaomingkeji.xyz

================================================================================
来源：http://bpj.jinqigufen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ruo.pycfn.com

================================================================================
来源：http://yck.jiagoushi.top

[U01] Py：创建虚拟环境
来源：http://caj.jianghu66.top

python -m venv .venv && source .venv/bin/activate
来源：http://zkg.yvedp.cn

[U02] Py：导出 / 安装依赖
来源：http://azf.cqqwz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vzn.epnwcf.com

[U03] Py：加载 .env 配置
来源：http://img.52xcode.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xhw.daria6918.cn

[U04] Py：变量调试打印
来源：http://upa.aizwys.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hag.316326.xyz

[U05] Py：列表去重且保序
来源：http://tai.feifeiyinyue.top

list(dict.fromkeys(arr))
来源：http://xmx.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://tph.andypj.xyz

{**a, **b}
来源：http://pji.yueranfly.top

[U07] Py：反转字典键值
来源：http://brl.cqqwz.cn

{v: k for k, v in d.items()}
来源：http://ske.52xcode.cn

[U08] Py：展平二维列表
来源：http://gpq.pengpengdd.cyou

[y for x in nested for y in x]
来源：http://apv.aibaodan.cn

[U09] Py：字典取最大值的键
来源：http://heu.yj20258.top

max(d, key=d.get)
来源：http://aeq.cashguo.top

[U10] Py：按值排序字典
来源：http://utt.xylfe.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ywo.pengpengdd.cyou

[U11] Py：生成器表达式
来源：http://ogg.yangfankeji.com

(x * 2 for x in arr)
来源：http://ylr.xylfe.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pac.epnwcf.com

Counter(arr).most_common(3)
来源：http://iyi.tanke756.top

[U13] Py：固定长度队列
来源：http://ght.wangdashe.top

deque(maxlen=10)
来源：http://tma.fehbvm.com

[U14] Py：分组收集到列表
来源：http://sbx.hammf.cn

defaultdict(list)
来源：http://umh.jqgufenzy.top

[U15] Py：高精度计时
来源：http://hqk.52xcode.cn

t = time.perf_counter()
来源：http://lln.hammf.cn

[U16] Py：命令行参数解析
来源：http://tcl.ctjpmb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iuz.hongshengwenyu.top

[U17] Py：初始化日志
来源：http://oqs.hywenlv.cn

logging.basicConfig(level=logging.INFO)
来源：http://zmd.sweek.top

[U18] Py：预编译正则
来源：http://oqd.aizwys.cn

pat = re.compile(r"\d+")
来源：http://xlt.shuidangran.top

[U19] Py：正则替换带回调
来源：http://eka.hywenlv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wri.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://oue.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://kaf.jiagoushi.top

[U21] Py：自定义上下文管理器
来源：http://unv.xuanzx.com

@contextlib.contextmanager
来源：http://bcl.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://wpa.jinqigfzy.top

list(zip(*m))
来源：http://yxb.ppjwa.cn

[U23] Py：分块读取大文件
来源：http://vdc.xylfe.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qsv.xingfuxueyuan.xyz

[U24] Py：路径操作
来源：http://moc.cdnleiting.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mjj.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://gmw.tian-w.cn

csv.DictReader(f)
来源：http://kkz.hfpthk.cn

[U26] Py：并发下载
来源：http://ihi.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rli.ydzc1.top

[U27] Py：异步 HTTP
来源：http://tci.gzhubu.top

aiohttp.ClientSession() 配合 async with
来源：http://hhu.sysykeji.top

[U28] Py：类型别名
来源：http://xik.hongshengwenyu.top

UserId = int
来源：http://jwe.tian-w.cn

[U29] Py：属性校验
来源：http://cjk.birdmap.top

@property 与 @x.setter 配合
来源：http://dtz.cashguo.top

[U30] Py：数据类
来源：http://vks.shuidangran.top

@dataclass(slots=True)
来源：http://awy.aizwys.cn

[U31] Py：单测
来源：http://huc.pengpengdd.cyou

python -m pytest -q
来源：http://qtm.jinqigufen.top

[U32] Py：代码格式化
来源：http://rln.jinyuanbaomall.cn

ruff format . && ruff check --fix .
来源：http://gvi.fzhhl.top

[U33] Py：打包发布
来源：http://axx.zhengqikj.top

python -m build  （依赖 pyproject.toml）
来源：http://mxm.mhx1999.top

[U34] Py：判断编码
来源：http://slu.epnwcf.com

chardet.detect(raw)
来源：http://ewj.ctjpmb.com

[U35] Py：发送邮件
来源：http://mfy.yongpay.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://znx.hammf.cn

[U36] Py：定时任务
来源：http://fjf.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://fjn.zhixingplan.top

[U37] Py：读写 Excel
来源：http://jbh.pengpengdd.cyou

pandas.read_excel / DataFrame.to_excel
来源：http://qrm.xingfuxueyuan.xyz

[U38] Py：获取脚本所在目录
来源：http://fvd.sjlbkw.cn

Path(__file__).resolve().parent
来源：http://ikn.zhijiandao.cn

[U39] Py：判断是否在交互环境
来源：http://lbj.wangdashe.top

sys.stdout.isatty()
来源：http://ini.haohaochexian.top

[U40] Py：打印到标准错误
来源：http://qud.xylfe.cn

print("err", file=sys.stderr)
来源：http://mxv.cheryme.top

[U41] PHP：初始化 Composer 项目
来源：http://our.cashguo.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pjr.dianchejie.cn

[U42] PHP：PSR-4 自动加载
来源：http://upn.jianghu66.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://raw.shangyingyoupin.top

[U43] PHP：声明命名空间
来源：http://mye.316326.xyz

namespace App\Http;
来源：http://jie.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://hcs.52xcode.cn

declare(strict_types=1);
来源：http://ief.xziqi.cn

[U45] PHP：类型声明与返回类型
来源：http://qfm.snrcjt.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://psg.pycfn.com

[U46] PHP：可空类型
来源：http://avr.gaohongyu789.top

?string $name = null
来源：http://mga.tarul.cn

[U47] PHP：联合类型
来源：http://zdp.jqgufenzy.top

int|string $id
来源：http://rsg.shuidangran.top

[U48] PHP：纯枚举
来源：http://hlc.hammf.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blr.yj20258.top

[U49] PHP：只读属性
来源：http://vil.sxryk.cn

public readonly string $name
来源：http://fsb.hfpthk.cn

[U50] PHP：构造器属性提升
来源：http://ons.ybcxt.top

public function __construct(private int $id) {}
来源：http://tun.jqgfzy.top

[U51] PHP：数组解构
来源：http://zre.tian-w.cn

[$a, $b] = $arr;
来源：http://tjw.zhijiandao.cn

[U52] PHP：箭头函数
来源：http://zqm.hongshengwenyu.top

$double = fn($x) => $x * 2;
来源：http://hjv.ivvv.top

[U53] PHP：空合并运算符
来源：http://cdj.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://eho.tian-w.cn

[U54] PHP：空安全调用
来源：http://bpl.fengsongda.top

$obj?->method()
来源：http://ixg.ywan-chungtsiang.top

[U55] PHP：match 表达式
来源：http://ikj.daxiang520.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://his.ywan-chungtsiang.top

[U56] PHP：命名参数
来源：http://yqt.yanxiufei.cn

f(a: 1, b: 2)
来源：http://jss.guowangkeji.top

[U57] PHP：字符串插值
来源：http://oxp.epnwcf.com

"值: {$a}"
来源：http://zwp.cdnleiting.top

[U58] PHP：数组三件套
来源：http://alj.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cci.jinqigfzy.top

[U59] PHP：自定义排序
来源：http://uem.gzhubu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rac.cucudq.cn

[U60] PHP：JSON 编解码
来源：http://hww.zhoulong.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pvn.hnxiangtu.top

[U61] PHP：正则
来源：http://irj.wangdashe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://krg.jinyuanbaomall.cn

[U62] PHP：日期对象
来源：http://qyn.yvedp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fcx.chenjidiqi.icu

[U63] PHP：文件读写
来源：http://thw.9152youxi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lkm.bbcook.cn

[U64] PHP：目录遍历
来源：http://jdr.zhixingplan.top

glob("dir/*.php");  scandir("dir");
来源：http://gvd.shuidangran.top

[U65] PHP：会话
来源：http://wbk.ehwqpu.com

session_start();  $_SESSION["uid"] = 1;
来源：http://fzf.hammf.cn

[U66] PHP：设置 Cookie
来源：http://uvr.jqgufenzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://unj.zycfv.cn

[U67] PHP：处理文件上传
来源：http://acr.sufxvd.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ooy.c1oappe.top

[U68] PHP：PDO 连接
来源：http://hlo.sysykeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ghp.jqgufenzy.top

[U69] PHP：PDO 预处理
来源：http://ska.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gcu.vehdjk.com

[U70] PHP：PDO 事务
来源：http://ssq.jianghu66.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://poh.shzxlz.cn

[U71] PHP：抛出异常
来源：http://hsv.jiagoushi.top

throw new RuntimeException("失败", 500);
来源：http://qkz.yanxiufei.cn

[U72] PHP：写错误日志
来源：http://kxy.yj202588.top

error_log("失败: " . $e->getMessage());
来源：http://zdb.jyoumei.cn

[U73] PHP：读取 ini 配置
来源：http://ydb.yanxiufei.cn

parse_ini_file("config.ini", true)
来源：http://djv.quarkkingdee.top

[U74] PHP：读取环境变量
来源：http://gaf.vqdsnc.cn

getenv("APP_ENV") ?: "production"
来源：http://agw.chenjidiqi.icu

[U75] PHP：依赖注入
来源：http://wyr.fengsongda.top

composer require psr/container
来源：http://gno.shanyushiyangtech.top

[U76] PHP：简单路由
来源：http://uhu.wangdashe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ctq.svipenyu.cn

[U77] PHP：模板渲染
来源：http://mfy.jyoumei.cn

composer require twig/twig
来源：http://wtx.gzhubu.top

[U78] PHP：单元测试
来源：http://dgv.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://bnc.quarkkingdee.top

[U79] PHP：静态分析
来源：http://axx.quarkkingdee.top

composer require --dev phpstan/phpstan
来源：http://kij.pengpengdd.cyou

[U80] PHP：代码规范修复
来源：http://gkr.daria6918.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wzw.bjfxy.top

[U81] JS：初始化项目
来源：http://wbz.yangfankeji.com

npm init -y;  npm i express
来源：http://sfi.sweek.top

[U82] JS：package.json 脚本
来源：http://nxd.fzhhl.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eif.wangshuangyany.cn

[U83] JS：ES Module 导入导出
来源：http://skd.sjlbkw.cn

export const a = 1;  import { a } from "./m.js";
来源：http://joa.meibo888.top

[U84] JS：CommonJS 写法
来源：http://pwx.aibaodan.cn

module.exports = { a };  const { a } = require("./m");
来源：http://siu.havefunace.top

[U85] JS：可选链
来源：http://vyc.jyoumei.cn

a?.b?.c
来源：http://nfa.hfpthk.cn

[U86] JS：空值合并
来源：http://jai.vehdjk.com

a ?? b
来源：http://nzs.yj202588.top

[U87] JS：解构默认值
来源：http://gvv.sysykeji.top

const { a = 1, b = 2 } = obj;
来源：http://ioa.epnwcf.com

[U88] JS：对象展开合并
来源：http://ryg.mhx1999.top

{ ...a, ...b }
来源：http://fwl.hnqzz.top

[U89] JS：数组去重
来源：http://rtg.xylfe.cn

[...new Set(arr)]
来源：http://kjl.hammf.cn

[U90] JS：数字数组排序
来源：http://mjh.jlsjyb.cn

[...arr].sort((a, b) => a - b)
来源：http://gfs.gogol.net.cn

[U91] JS：对象键值遍历
来源：http://hml.smart0.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dev.wangdashe.top

[U92] JS：深拷贝
来源：http://bqg.nanxuanxn.top

structuredClone(obj)
来源：http://bla.fzhhl.top

[U93] JS：模板字符串
来源：http://pfd.bbcook.cn

`共 ${n} 条`
来源：http://ouc.zhongyouzk.top

[U94] JS：箭头函数
来源：http://eww.guowangkeji.top

const double = x => x * 2;
来源：http://sog.hnqzz.top

[U95] JS：Promise 包装
来源：http://vcm.nanxuanxn.top

new Promise((resolve, reject) => {})
来源：http://xvi.hysaishi.cn

[U96] JS：async/await 与异常
来源：http://wog.smart0.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aji.fktsv.cn

[U97] JS：并发请求
来源：http://joa.pycfn.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://pns.ctjpmb.com

[U98] JS：fetch 带 JSON
来源：http://ubl.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jsx.svipenyu.cn

[U99] JS：事件监听
来源：http://jwu.zhongyouzk.top

el.addEventListener("click", e => {})
来源：http://yjl.uphjek.com

[U100] JS：DOM 查询
来源：http://qyw.yueranfly.top

document.querySelector(".item")
来源：http://yvs.fzhhl.top

[U101] JS：classList 操作
来源：http://qfu.zhengqikj.top

el.classList.toggle("active")
来源：http://kfj.zhiwuduotai.top

[U102] JS：本地存储
来源：http://bfp.daria6918.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://teg.quarkkingdee.top

[U103] JS：定时器
来源：http://khf.sweek.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xrl.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://xnm.yj20258.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qrj.wangshuangyany.cn

[U105] JS：节流
来源：http://fht.vehdjk.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ewf.zhengqikj.top

[U106] JS：日期格式化
来源：http://uzf.kuanghao11.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sgp.mhx1999.top

[U107] JS：数字千分位
来源：http://uoa.wangshuangyany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://imq.yangfankeji.com

[U108] JS：随机整数
来源：http://maq.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zxm.bjfxy.top

[U109] JS：数组分组
来源：http://dvu.ywan-chungtsiang.top

Object.groupBy(arr, x => x.type)
来源：http://ahx.tanke756.top

[U110] JS：数组分块
来源：http://jky.yongpay.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bwv.jyoumei.cn

[U111] JS：对象转 Map
来源：http://zqa.tianlin.xyz

new Map(Object.entries(obj))
来源：http://khg.feifeiyinyue.top

[U112] JS：字符串补位
来源：http://mfm.shuidangran.top

"7".padStart(3, "0")
来源：http://nan.zhengqikj.top

[U113] JS：正则替换全部
来源：http://drq.tianlin.xyz

s.replaceAll("a", "b")
来源：http://qdy.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://rpq.hywenlv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yon.yangfankeji.com

[U115] JS：生成 UUID
来源：http://iej.sysykeji.top

crypto.randomUUID()
来源：http://vky.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://vtv.hnqzz.top

/** @param {string} name */ function f(name) {}
来源：http://gby.shanyushiyangkeji.top

[U117] JS：单元测试
来源：http://bfn.tian-w.cn

npm i -D vitest;  npx vitest
来源：http://zjj.jyoumei.cn

[U118] JS：开发服务器
来源：http://vuc.svipenyu.cn

npm i -D vite;  npx vite
来源：http://krc.gogol.net.cn

[U119] JS：生产构建
来源：http://fiy.sxryk.cn

npx vite build
来源：http://rfh.kuanghao11.cn

[U120] JS：读取环境变量（Vite）
来源：http://zuu.nanxinkj.top

import.meta.env.VITE_API_URL
来源：http://nsy.redwolf501.top

================================================================================
来源：http://vyu.ehwqpu.com

统计汇总
来源：http://cux.ctjpmb.com

================================================================================
来源：http://act.vqdsnc.cn

按语言统计（条）：
来源：http://bji.hnxiangtu.top

Python ......... 252
来源：http://wrp.dianchejie.cn

PHP ............ 252
来源：http://udp.xylfe.cn

JavaScript ..... 252
来源：http://eua.birdmap.top

TypeScript ..... 212
来源：http://sly.feifeiyinyue.top

Java ........... 212
来源：http://hqk.zhijiandao.cn

Go ............. 212
来源：http://jti.yj202588.top

Ruby ........... 212
来源：http://ceq.tarul.cn

C# ............. 212
来源：http://nbi.cqqwz.cn

C .............. 30
来源：http://qmc.zhengqikj.top

C++ ............ 30
来源：http://zvd.feifeiyinyue.top

SQL ............ 90
来源：http://wan.sweek.top

Bash ........... 80
来源：http://xrp.cheryme.top

Kotlin ......... 15
来源：http://vlo.yuanzhike.top

Swift .......... 15
来源：http://vld.yj202588.top

Lua ............ 10
来源：http://kmr.sysykeji.top

Perl ........... 10
来源：http://flg.ppjwa.cn

Scala .......... 10
来源：http://rhs.cqqwz.cn

------------------------------------
来源：http://cbw.fktsv.cn

合计 ........... 2106 条
来源：http://oyp.sysykeji.top

按章节统计：
来源：http://due.sysykeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zdo.ybcxt.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://isb.jyoumei.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mey.cqqwz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vaa.xingfuxueyuan.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pdz.hysaishi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://huc.sjlbkw.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fgb.fehbvm.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ihu.jinghuilouyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tfs.yfazqb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iim.yuxming.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qum.yvedp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gff.wangdashe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ska.xingfuxueyuan.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ldv.shanyushiyangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ycr.dianchejie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://idu.cucudq.cn

Q SQL 专题                              90
来源：http://mch.tian-w.cn

R Bash 专题                             80
来源：http://qlr.ydzc1.top

S C / C++ 专题                          60
来源：http://twp.shangyingyoupin.top

T 其他语言补充                          60
来源：http://hho.cqqwz.cn


<!-- 参考信息 -->