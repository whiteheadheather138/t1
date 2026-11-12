代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://epl.redwolf501.top

[T51] Scala：Hello World
来源：http://qjm.xuetiantiany.cn

println("Hello")
来源：http://tdl.hnqzz.top

[T52] Scala：变量
来源：http://jsk.hywenlv.cn

val a = 1;  var b = 2
来源：http://rpi.xziqi.cn

[T53] Scala：字符串插值
来源：http://sts.fktsv.cn

s"值: $b"
来源：http://raa.yuanzhike.top

[T54] Scala：集合映射
来源：http://ngz.meibo888.top

List(1, 2, 3).map(_ * 2)
来源：http://ugu.xingfuxueyuan.xyz

[T55] Scala：集合过滤
来源：http://wom.shuidangran.top

List(1, 2, 3).filter(_ > 1)
来源：http://vtp.fehbvm.com

[T56] Scala：样例类
来源：http://dcn.jinyuanbaomall.cn

case class User(name: String, age: Int)
来源：http://upm.tian-w.cn

[T57] Scala：模式匹配
来源：http://mgk.chenzaomai.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://kcf.tian-w.cn

[T58] Scala：函数定义
来源：http://wpw.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://kke.hammf.cn

[T59] Scala：循环
来源：http://vmd.pengpengdd.cyou

for (i <- 1 to 10) println(i)
来源：http://cyp.yuxming.cn

[T60] Scala：折叠
来源：http://hwo.birdmap.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mvr.chenzaomai.com

================================================================================
来源：http://buc.mhx1999.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iqj.nwbrower.top

================================================================================
来源：http://kum.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://wpl.wangshuangyany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wwf.iojbl.cn

[U02] Py：导出 / 安装依赖
来源：http://bte.fktsv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dnt.nanxinkj.top

[U03] Py：加载 .env 配置
来源：http://umh.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wqk.tarul.cn

[U04] Py：变量调试打印
来源：http://yra.jinghuilouyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mlw.dashuyun.cn

[U05] Py：列表去重且保序
来源：http://ugd.fktsv.cn

list(dict.fromkeys(arr))
来源：http://fkp.ybcxt.top

[U06] Py：合并两个字典
来源：http://mrw.yangfankeji.com

{**a, **b}
来源：http://qyo.yonumen.top

[U07] Py：反转字典键值
来源：http://ngh.ydjk.org.cn

{v: k for k, v in d.items()}
来源：http://lev.fanxiaobao.xyz

[U08] Py：展平二维列表
来源：http://alp.tian-w.cn

[y for x in nested for y in x]
来源：http://eha.sjlbkw.cn

[U09] Py：字典取最大值的键
来源：http://aeb.zdbjq.cn

max(d, key=d.get)
来源：http://toh.chenzaomai.com

[U10] Py：按值排序字典
来源：http://bfu.xuetiantiany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dtt.zycfv.cn

[U11] Py：生成器表达式
来源：http://vbw.ydjk.org.cn

(x * 2 for x in arr)
来源：http://osj.bjfxy.top

[U12] Py：取出现最多的 3 个元素
来源：http://giq.yanxiufei.cn

Counter(arr).most_common(3)
来源：http://njv.gaohongyu789.top

[U13] Py：固定长度队列
来源：http://sye.zhaomingkeji.xyz

deque(maxlen=10)
来源：http://lik.chenjidiqi.icu

[U14] Py：分组收集到列表
来源：http://pnl.dianchejie.cn

defaultdict(list)
来源：http://lki.tarul.cn

[U15] Py：高精度计时
来源：http://vfh.xuetiantiany.cn

t = time.perf_counter()
来源：http://yek.daria6918.cn

[U16] Py：命令行参数解析
来源：http://kkj.jinqigufen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ske.havefunace.top

[U17] Py：初始化日志
来源：http://nys.haohaochexian.top

logging.basicConfig(level=logging.INFO)
来源：http://ydn.shanyushiyangkeji.top

[U18] Py：预编译正则
来源：http://kyb.ctjpmb.com

pat = re.compile(r"\d+")
来源：http://hyj.ehwqpu.com

[U19] Py：正则替换带回调
来源：http://rcz.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zvc.cucudq.cn

[U20] Py：缓存函数结果
来源：http://edu.ywan-chungtsiang.top

@functools.lru_cache(maxsize=None)
来源：http://dwa.hammf.cn

[U21] Py：自定义上下文管理器
来源：http://bco.shanyushiyangtech.top

@contextlib.contextmanager
来源：http://qcd.bjfxy.top

[U22] Py：矩阵转置
来源：http://fxf.zhaomingkeji.xyz

list(zip(*m))
来源：http://ykh.52xcode.cn

[U23] Py：分块读取大文件
来源：http://jad.jinqigufen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zds.haohaochexian.top

[U24] Py：路径操作
来源：http://juz.yanxiufei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cvd.gzhubu.top

[U25] Py：CSV 按字典读
来源：http://grk.pycfn.com

csv.DictReader(f)
来源：http://vtq.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://ykb.bbcook.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rbd.ydzc1.top

[U27] Py：异步 HTTP
来源：http://feb.vehdjk.com

aiohttp.ClientSession() 配合 async with
来源：http://kvn.zhongyouzk.top

[U28] Py：类型别名
来源：http://cuw.gotoacloud.top

UserId = int
来源：http://zod.yj20258.top

[U29] Py：属性校验
来源：http://cli.hesvh.cn

@property 与 @x.setter 配合
来源：http://fbh.xuanzx.com

[U30] Py：数据类
来源：http://ugl.yfazqb.com

@dataclass(slots=True)
来源：http://ltn.sysykeji.top

[U31] Py：单测
来源：http://xze.gaohongyu789.top

python -m pytest -q
来源：http://tfa.52xcode.cn

[U32] Py：代码格式化
来源：http://fcp.nwbrower.top

ruff format . && ruff check --fix .
来源：http://xwx.cucudq.cn

[U33] Py：打包发布
来源：http://xzk.shanyushiyangtech.top

python -m build  （依赖 pyproject.toml）
来源：http://gta.yuanzhike.top

[U34] Py：判断编码
来源：http://riv.jinyuanbaomall.cn

chardet.detect(raw)
来源：http://uqa.yueranfly.top

[U35] Py：发送邮件
来源：http://mdq.tianlin.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ckp.tian-w.cn

[U36] Py：定时任务
来源：http://rni.jianghu66.top

schedule.every(10).minutes.do(job)
来源：http://ewn.yonumen.top

[U37] Py：读写 Excel
来源：http://umg.haohaochexian.top

pandas.read_excel / DataFrame.to_excel
来源：http://sti.xylfe.cn

[U38] Py：获取脚本所在目录
来源：http://ypw.yanxiufei.cn

Path(__file__).resolve().parent
来源：http://avl.hammf.cn

[U39] Py：判断是否在交互环境
来源：http://jka.0kj1m.cn

sys.stdout.isatty()
来源：http://ktl.dashuyun.cn

[U40] Py：打印到标准错误
来源：http://hhv.yongpay.top

print("err", file=sys.stderr)
来源：http://olx.guowangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://opw.hcnkem.com

composer init;  composer require guzzlehttp/guzzle
来源：http://cdj.vqdsnc.cn

[U42] PHP：PSR-4 自动加载
来源：http://sje.zdqjudy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kal.gotoacloud.top

[U43] PHP：声明命名空间
来源：http://wfm.zhoulong.xyz

namespace App\Http;
来源：http://mpt.vqdsnc.cn

[U44] PHP：开启严格类型
来源：http://ayu.chenjidiqi.icu

declare(strict_types=1);
来源：http://azr.ehwqpu.com

[U45] PHP：类型声明与返回类型
来源：http://bnx.sufxvd.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://eld.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://vpi.yj20258.top

?string $name = null
来源：http://arr.9152youxi.cn

[U47] PHP：联合类型
来源：http://xar.zhoulong.xyz

int|string $id
来源：http://bov.ivvv.top

[U48] PHP：纯枚举
来源：http://bxt.wangdashe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eam.yj20258888.top

[U49] PHP：只读属性
来源：http://wsr.redwolf501.top

public readonly string $name
来源：http://hsl.aibaodan.cn

[U50] PHP：构造器属性提升
来源：http://syh.hcnkem.com

public function __construct(private int $id) {}
来源：http://nkd.cdnleiting.top

[U51] PHP：数组解构
来源：http://erl.tanke756.top

[$a, $b] = $arr;
来源：http://fnr.jinqigfzy.top

[U52] PHP：箭头函数
来源：http://ugd.hcnkem.com

$double = fn($x) => $x * 2;
来源：http://hbx.shanyushiyangkeji.top

[U53] PHP：空合并运算符
来源：http://ave.316326.xyz

$v = $a ?? $b ?? "default";
来源：http://kcv.zhixingplan.top

[U54] PHP：空安全调用
来源：http://nmw.chenlongwang.top

$obj?->method()
来源：http://jfb.wangshuangyany.cn

[U55] PHP：match 表达式
来源：http://ixt.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://txg.ehwqpu.com

[U56] PHP：命名参数
来源：http://qof.yuanzhike.top

f(a: 1, b: 2)
来源：http://dne.gotoacloud.top

[U57] PHP：字符串插值
来源：http://hyp.guowangkeji.top

"值: {$a}"
来源：http://ioo.hysaishi.cn

[U58] PHP：数组三件套
来源：http://scf.yvedp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gtq.pengpengdd.cyou

[U59] PHP：自定义排序
来源：http://xac.316326.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uwf.xziqi.cn

[U60] PHP：JSON 编解码
来源：http://tpn.cucudq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dad.iojbl.cn

[U61] PHP：正则
来源：http://mjb.sysykeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uwg.svipenyu.cn

[U62] PHP：日期对象
来源：http://tue.yfazqb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mki.hfpthk.cn

[U63] PHP：文件读写
来源：http://lho.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eip.yangfankeji.com

[U64] PHP：目录遍历
来源：http://umt.epnwcf.com

glob("dir/*.php");  scandir("dir");
来源：http://bzg.cashguo.top

[U65] PHP：会话
来源：http://jxe.yanxiufei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lni.chenlongwang.top

[U66] PHP：设置 Cookie
来源：http://irx.andypj.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uco.cashguo.top

[U67] PHP：处理文件上传
来源：http://vfc.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fpn.fktsv.cn

[U68] PHP：PDO 连接
来源：http://scd.mhx1999.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cjm.zdqjudy.top

[U69] PHP：PDO 预处理
来源：http://khg.shanyushiyangtech.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://brq.cdnleiting.top

[U70] PHP：PDO 事务
来源：http://dtx.uphjek.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jnt.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://oqj.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://dcs.yueranfly.top

[U72] PHP：写错误日志
来源：http://mpk.yonumen.top

error_log("失败: " . $e->getMessage());
来源：http://ztu.gzhubu.top

[U73] PHP：读取 ini 配置
来源：http://kvz.gzhubu.top

parse_ini_file("config.ini", true)
来源：http://jht.aizwys.cn

[U74] PHP：读取环境变量
来源：http://vkc.sufxvd.cn

getenv("APP_ENV") ?: "production"
来源：http://yet.kuanghao11.cn

[U75] PHP：依赖注入
来源：http://vxs.ywan-chungtsiang.top

composer require psr/container
来源：http://udf.ivvv.top

[U76] PHP：简单路由
来源：http://vhd.sysykeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gle.hywenlv.cn

[U77] PHP：模板渲染
来源：http://ufx.dashuyun.cn

composer require twig/twig
来源：http://ock.cucudq.cn

[U78] PHP：单元测试
来源：http://dgd.aizwys.cn

composer require --dev phpunit/phpunit
来源：http://tpb.ivvv.top

[U79] PHP：静态分析
来源：http://yxo.quarkkingdee.top

composer require --dev phpstan/phpstan
来源：http://xfj.hysaishi.cn

[U80] PHP：代码规范修复
来源：http://wez.zdqjudy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qao.xuanzx.com

[U81] JS：初始化项目
来源：http://ddw.nanxinkj.top

npm init -y;  npm i express
来源：http://tpa.hammf.cn

[U82] JS：package.json 脚本
来源：http://hjl.vqdsnc.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ebd.jiagoushi.top

[U83] JS：ES Module 导入导出
来源：http://lsd.wangdashe.top

export const a = 1;  import { a } from "./m.js";
来源：http://pkk.daxiang520.top

[U84] JS：CommonJS 写法
来源：http://wci.hywenlv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://otq.tarul.cn

[U85] JS：可选链
来源：http://qya.vqdsnc.cn

a?.b?.c
来源：http://ebu.xziqi.cn

[U86] JS：空值合并
来源：http://bxx.pycfn.com

a ?? b
来源：http://ojo.kuanghao11.cn

[U87] JS：解构默认值
来源：http://hir.cucudq.cn

const { a = 1, b = 2 } = obj;
来源：http://irm.ybcxt.top

[U88] JS：对象展开合并
来源：http://jen.jinyuanbaomall.cn

{ ...a, ...b }
来源：http://wfz.quarkkingdee.top

[U89] JS：数组去重
来源：http://xdy.gotoacloud.top

[...new Set(arr)]
来源：http://ghi.xylfe.cn

[U90] JS：数字数组排序
来源：http://twq.hywenlv.cn

[...arr].sort((a, b) => a - b)
来源：http://cxe.zhijiandao.cn

[U91] JS：对象键值遍历
来源：http://wyb.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jzv.yj202588.top

[U92] JS：深拷贝
来源：http://kii.yuanzhike.top

structuredClone(obj)
来源：http://ehh.chenjidiqi.icu

[U93] JS：模板字符串
来源：http://aii.yj20258888.top

`共 ${n} 条`
来源：http://rof.hfpthk.cn

[U94] JS：箭头函数
来源：http://nqd.cdnleiting.top

const double = x => x * 2;
来源：http://rqw.guannengcc.top

[U95] JS：Promise 包装
来源：http://ppu.sxryk.cn

new Promise((resolve, reject) => {})
来源：http://qry.ctjpmb.com

[U96] JS：async/await 与异常
来源：http://pzp.aibaodan.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://csh.daria6918.cn

[U97] JS：并发请求
来源：http://kyn.hnxiangtu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://udd.andypj.xyz

[U98] JS：fetch 带 JSON
来源：http://tpj.havefunace.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qak.zdbjq.cn

[U99] JS：事件监听
来源：http://evw.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://hxg.andypj.xyz

[U100] JS：DOM 查询
来源：http://soz.nwbrower.top

document.querySelector(".item")
来源：http://tfz.xingfuxueyuan.xyz

[U101] JS：classList 操作
来源：http://xah.cucudq.cn

el.classList.toggle("active")
来源：http://akh.yangfankeji.com

[U102] JS：本地存储
来源：http://jdl.xylfe.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mcz.daxiang520.top

[U103] JS：定时器
来源：http://odt.shangyingyoupin.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gzt.hcnkem.com

[U104] JS：防抖
来源：http://qqs.nanxinkj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pcl.guannengcc.top

[U105] JS：节流
来源：http://dta.quarkkingdee.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aji.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://idn.xinyue.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jjn.hongshengwenyu.top

[U107] JS：数字千分位
来源：http://gzm.aizwys.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hyj.sxryk.cn

[U108] JS：随机整数
来源：http://nlz.sxryk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yfs.shangyingyoupin.top

[U109] JS：数组分组
来源：http://vas.jqgufenzy.top

Object.groupBy(arr, x => x.type)
来源：http://vve.9152youxi.cn

[U110] JS：数组分块
来源：http://ocd.ydjk.org.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bgj.yfazqb.com

[U111] JS：对象转 Map
来源：http://vim.jqgfzy.top

new Map(Object.entries(obj))
来源：http://ysz.hfpthk.cn

[U112] JS：字符串补位
来源：http://wlp.iojbl.cn

"7".padStart(3, "0")
来源：http://gxi.chenjidiqi.icu

[U113] JS：正则替换全部
来源：http://xcj.uphjek.com

s.replaceAll("a", "b")
来源：http://qkx.yj20258.top

[U114] JS：JSON 深比较
来源：http://dwk.ydjk.org.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://eze.vqdsnc.cn

[U115] JS：生成 UUID
来源：http://mxm.shanyushiyangkeji.top

crypto.randomUUID()
来源：http://maq.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://elw.9152youxi.cn

/** @param {string} name */ function f(name) {}
来源：http://zgc.vqdsnc.cn

[U117] JS：单元测试
来源：http://enx.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://ghx.hcnkem.com

[U118] JS：开发服务器
来源：http://kkp.chenjidiqi.icu

npm i -D vite;  npx vite
来源：http://oux.fanxiaobao.xyz

[U119] JS：生产构建
来源：http://law.yuxming.cn

npx vite build
来源：http://pvi.shanyushiyangtech.top

[U120] JS：读取环境变量（Vite）
来源：http://elg.shanyushiyangtech.top

import.meta.env.VITE_API_URL
来源：http://sfx.cqqwz.cn

================================================================================
来源：http://fvv.iojbl.cn

统计汇总
来源：http://rwo.xuanzx.com

================================================================================
来源：http://wfj.snrcjt.cn

按语言统计（条）：
来源：http://vnv.zhengqikj.top

Python ......... 252
来源：http://yol.xinyue.icu

PHP ............ 252
来源：http://fcx.dashuyun.cn

JavaScript ..... 252
来源：http://ext.jyoumei.cn

TypeScript ..... 212
来源：http://kbp.fzhhl.top

Java ........... 212
来源：http://osh.ydjk.org.cn

Go ............. 212
来源：http://aad.yanxiufei.cn

Ruby ........... 212
来源：http://lap.cheryme.top

C# ............. 212
来源：http://lsq.redwolf501.top

C .............. 30
来源：http://oiu.fengsongda.top

C++ ............ 30
来源：http://dwo.quarkkingdee.top

SQL ............ 90
来源：http://cqk.yfazqb.com

Bash ........... 80
来源：http://cyp.9152youxi.cn

Kotlin ......... 15
来源：http://pzk.sxryk.cn

Swift .......... 15
来源：http://qtw.pycfn.com

Lua ............ 10
来源：http://slg.sweek.top

Perl ........... 10
来源：http://nfu.jqgufenzy.top

Scala .......... 10
来源：http://dwx.yuxming.cn

------------------------------------
来源：http://sim.yvedp.cn

合计 ........... 2106 条
来源：http://awn.daria6918.cn

按章节统计：
来源：http://nem.yuxming.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gbb.ywan-chungtsiang.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qqc.yueranfly.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oux.aizwys.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fqg.haohaochexian.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://aqr.xuetiantiany.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pjj.aizwys.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hyg.shanyushiyangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://asu.ppjwa.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://crm.cucudq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uho.52xcode.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vtz.ehwqpu.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lsa.yvedp.cn


<!-- 参考信息 -->