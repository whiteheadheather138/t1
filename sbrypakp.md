代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://byo.chenzaomai.com

[T51] Scala：Hello World
来源：http://wnm.redwolf501.top

println("Hello")
来源：http://bvg.jinqigufen.top

[T52] Scala：变量
来源：http://jnh.sysykeji.top

val a = 1;  var b = 2
来源：http://iyw.52xcode.cn

[T53] Scala：字符串插值
来源：http://xmx.uphjek.com

s"值: $b"
来源：http://iqt.fktsv.cn

[T54] Scala：集合映射
来源：http://voa.xinyue.icu

List(1, 2, 3).map(_ * 2)
来源：http://pnd.yanxiufei.cn

[T55] Scala：集合过滤
来源：http://kbe.ydzc1.top

List(1, 2, 3).filter(_ > 1)
来源：http://vve.jinghuilouyu.cn

[T56] Scala：样例类
来源：http://vnx.havefunace.top

case class User(name: String, age: Int)
来源：http://dpc.shzxlz.cn

[T57] Scala：模式匹配
来源：http://eqe.ydzc1.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://tiy.xingfuxueyuan.xyz

[T58] Scala：函数定义
来源：http://fgw.pycfn.com

def add(a: Int, b: Int): Int = a + b
来源：http://yaa.wangshuangyany.cn

[T59] Scala：循环
来源：http://juo.kuanghao11.cn

for (i <- 1 to 10) println(i)
来源：http://dpb.sjlbkw.cn

[T60] Scala：折叠
来源：http://tfn.hnxiangtu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rxs.zycfv.cn

================================================================================
来源：http://gyf.quarkkingdee.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sgz.jinqigufen.top

================================================================================
来源：http://opl.vqdsnc.cn

[U01] Py：创建虚拟环境
来源：http://tnz.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://otd.yfazqb.com

[U02] Py：导出 / 安装依赖
来源：http://qbj.zdqjudy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qej.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://kid.hfpthk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wft.chenlongwang.top

[U04] Py：变量调试打印
来源：http://ixl.shangyingyoupin.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rkg.epnwcf.com

[U05] Py：列表去重且保序
来源：http://jpw.hcnkem.com

list(dict.fromkeys(arr))
来源：http://iiu.hammf.cn

[U06] Py：合并两个字典
来源：http://xgk.daxiang520.top

{**a, **b}
来源：http://cms.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://ckk.zycfv.cn

{v: k for k, v in d.items()}
来源：http://dcj.hammf.cn

[U08] Py：展平二维列表
来源：http://eeq.redwolf501.top

[y for x in nested for y in x]
来源：http://dqk.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://fth.ppjwa.cn

max(d, key=d.get)
来源：http://kqx.kuanghao11.cn

[U10] Py：按值排序字典
来源：http://tst.hongshengwenyu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jrj.wangdashe.top

[U11] Py：生成器表达式
来源：http://hwh.jinyuanbaomall.cn

(x * 2 for x in arr)
来源：http://sly.fzhhl.top

[U12] Py：取出现最多的 3 个元素
来源：http://vdl.daxiang520.top

Counter(arr).most_common(3)
来源：http://ouf.hnxiangtu.top

[U13] Py：固定长度队列
来源：http://bvu.guowangkeji.top

deque(maxlen=10)
来源：http://rqf.yvedp.cn

[U14] Py：分组收集到列表
来源：http://lrk.dianchejie.cn

defaultdict(list)
来源：http://bwt.tanke756.top

[U15] Py：高精度计时
来源：http://ikh.0kj1m.cn

t = time.perf_counter()
来源：http://iae.gzhubu.top

[U16] Py：命令行参数解析
来源：http://ikw.xuetiantiany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jcz.yongpay.top

[U17] Py：初始化日志
来源：http://gqi.hnqzz.top

logging.basicConfig(level=logging.INFO)
来源：http://jnw.nanxuanxn.top

[U18] Py：预编译正则
来源：http://knm.sysykeji.top

pat = re.compile(r"\d+")
来源：http://zse.shuidangran.top

[U19] Py：正则替换带回调
来源：http://taj.jinyuanbaomall.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yxd.gotoacloud.top

[U20] Py：缓存函数结果
来源：http://qju.gaohongyu789.top

@functools.lru_cache(maxsize=None)
来源：http://qkt.gzhubu.top

[U21] Py：自定义上下文管理器
来源：http://jvt.fehbvm.com

@contextlib.contextmanager
来源：http://avh.svipenyu.cn

[U22] Py：矩阵转置
来源：http://uoz.nanxuanxn.top

list(zip(*m))
来源：http://sbv.pengpengdd.cyou

[U23] Py：分块读取大文件
来源：http://itk.yueranfly.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pel.yangfankeji.com

[U24] Py：路径操作
来源：http://cvd.yfazqb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pdf.wangshuangyany.cn

[U25] Py：CSV 按字典读
来源：http://mot.gotoacloud.top

csv.DictReader(f)
来源：http://cgn.zdbjq.cn

[U26] Py：并发下载
来源：http://lya.gotoacloud.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dno.zhoulong.xyz

[U27] Py：异步 HTTP
来源：http://rcj.pengpengdd.cyou

aiohttp.ClientSession() 配合 async with
来源：http://vei.birdmap.top

[U28] Py：类型别名
来源：http://zcr.vqdsnc.cn

UserId = int
来源：http://xef.hnxiangtu.top

[U29] Py：属性校验
来源：http://wxw.nwbrower.top

@property 与 @x.setter 配合
来源：http://ibi.guannengcc.top

[U30] Py：数据类
来源：http://yac.ctjpmb.com

@dataclass(slots=True)
来源：http://fqz.guannengcc.top

[U31] Py：单测
来源：http://fta.tian-w.cn

python -m pytest -q
来源：http://zyo.nwbrower.top

[U32] Py：代码格式化
来源：http://rwk.hongshengwenyu.top

ruff format . && ruff check --fix .
来源：http://qii.52xcode.cn

[U33] Py：打包发布
来源：http://ypv.jinqigufen.top

python -m build  （依赖 pyproject.toml）
来源：http://lgk.mhx1999.top

[U34] Py：判断编码
来源：http://zbc.jinqigfzy.top

chardet.detect(raw)
来源：http://ezk.cqqwz.cn

[U35] Py：发送邮件
来源：http://mhh.hywenlv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oca.wangshuangyany.cn

[U36] Py：定时任务
来源：http://yfi.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://gxd.ybcxt.top

[U37] Py：读写 Excel
来源：http://hsu.nanxuanxn.top

pandas.read_excel / DataFrame.to_excel
来源：http://edl.chenzaomai.com

[U38] Py：获取脚本所在目录
来源：http://pjr.smart0.xyz

Path(__file__).resolve().parent
来源：http://ohn.shanyushiyangtech.top

[U39] Py：判断是否在交互环境
来源：http://apd.fengsongda.top

sys.stdout.isatty()
来源：http://mei.yueranfly.top

[U40] Py：打印到标准错误
来源：http://slx.snrcjt.cn

print("err", file=sys.stderr)
来源：http://jbk.redwolf501.top

[U41] PHP：初始化 Composer 项目
来源：http://sgf.zdqjudy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ahb.ybcxt.top

[U42] PHP：PSR-4 自动加载
来源：http://tzd.jqgfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dan.chenlongwang.top

[U43] PHP：声明命名空间
来源：http://qma.jqgufenzy.top

namespace App\Http;
来源：http://bzq.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://gmh.hesvh.cn

declare(strict_types=1);
来源：http://mgh.daria6918.cn

[U45] PHP：类型声明与返回类型
来源：http://ana.zycfv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lzc.cucudq.cn

[U46] PHP：可空类型
来源：http://kue.yvedp.cn

?string $name = null
来源：http://ted.aibaodan.cn

[U47] PHP：联合类型
来源：http://zkb.fengsongda.top

int|string $id
来源：http://ntw.feifeiyinyue.top

[U48] PHP：纯枚举
来源：http://uli.dianchejie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bsv.yj20258.top

[U49] PHP：只读属性
来源：http://rep.dashuyun.cn

public readonly string $name
来源：http://uba.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://ntc.zdbjq.cn

public function __construct(private int $id) {}
来源：http://tvm.dianchejie.cn

[U51] PHP：数组解构
来源：http://whd.chenzaomai.com

[$a, $b] = $arr;
来源：http://lkk.xinyue.icu

[U52] PHP：箭头函数
来源：http://cse.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://oqy.mhx1999.top

[U53] PHP：空合并运算符
来源：http://rph.hysaishi.cn

$v = $a ?? $b ?? "default";
来源：http://ucv.hongshengwenyu.top

[U54] PHP：空安全调用
来源：http://lsw.zycfv.cn

$obj?->method()
来源：http://zbh.yonumen.top

[U55] PHP：match 表达式
来源：http://zdf.fengsongda.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pzm.cucudq.cn

[U56] PHP：命名参数
来源：http://rwg.uphjek.com

f(a: 1, b: 2)
来源：http://qls.aizwys.cn

[U57] PHP：字符串插值
来源：http://hhu.hysaishi.cn

"值: {$a}"
来源：http://sqz.wangshuangyany.cn

[U58] PHP：数组三件套
来源：http://kjc.zhoulong.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xek.yongpay.top

[U59] PHP：自定义排序
来源：http://cpo.tarul.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vyv.daria6918.cn

[U60] PHP：JSON 编解码
来源：http://icr.316326.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tfb.xuanzx.com

[U61] PHP：正则
来源：http://bah.xziqi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://otv.yonumen.top

[U62] PHP：日期对象
来源：http://aux.cashguo.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://htn.smart0.xyz

[U63] PHP：文件读写
来源：http://nhi.xinyue.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zro.guowangkeji.top

[U64] PHP：目录遍历
来源：http://vrc.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://qiz.snrcjt.cn

[U65] PHP：会话
来源：http://jtf.zdqjudy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nca.xziqi.cn

[U66] PHP：设置 Cookie
来源：http://prt.uphjek.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yki.havefunace.top

[U67] PHP：处理文件上传
来源：http://wgd.kuanghao11.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rom.tianlin.xyz

[U68] PHP：PDO 连接
来源：http://gfd.sysykeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://szw.redwolf501.top

[U69] PHP：PDO 预处理
来源：http://lyc.cashguo.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://coe.ctjpmb.com

[U70] PHP：PDO 事务
来源：http://oxd.jyoumei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kjp.mhx1999.top

[U71] PHP：抛出异常
来源：http://dmn.xuanzx.com

throw new RuntimeException("失败", 500);
来源：http://qtt.ydjk.org.cn

[U72] PHP：写错误日志
来源：http://zdg.ydjk.org.cn

error_log("失败: " . $e->getMessage());
来源：http://bwk.fzhhl.top

[U73] PHP：读取 ini 配置
来源：http://szo.uphjek.com

parse_ini_file("config.ini", true)
来源：http://hsr.vehdjk.com

[U74] PHP：读取环境变量
来源：http://dkh.xuanzx.com

getenv("APP_ENV") ?: "production"
来源：http://rjj.daxiang520.top

[U75] PHP：依赖注入
来源：http://xkq.iojbl.cn

composer require psr/container
来源：http://byb.yvedp.cn

[U76] PHP：简单路由
来源：http://sjl.havefunace.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tov.ctjpmb.com

[U77] PHP：模板渲染
来源：http://wpy.jinyuanbaomall.cn

composer require twig/twig
来源：http://wif.316326.xyz

[U78] PHP：单元测试
来源：http://lyv.wangshuangyany.cn

composer require --dev phpunit/phpunit
来源：http://nud.hnxiangtu.top

[U79] PHP：静态分析
来源：http://cot.yj202588.top

composer require --dev phpstan/phpstan
来源：http://uyk.hysaishi.cn

[U80] PHP：代码规范修复
来源：http://yjn.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://npi.fehbvm.com

[U81] JS：初始化项目
来源：http://ooi.ywan-chungtsiang.top

npm init -y;  npm i express
来源：http://cwg.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://cyj.fktsv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ope.smart0.xyz

[U83] JS：ES Module 导入导出
来源：http://fbt.zhiwuduotai.top

export const a = 1;  import { a } from "./m.js";
来源：http://dqx.ehwqpu.com

[U84] JS：CommonJS 写法
来源：http://ral.yfazqb.com

module.exports = { a };  const { a } = require("./m");
来源：http://yaf.feifeiyinyue.top

[U85] JS：可选链
来源：http://sgd.hfpthk.cn

a?.b?.c
来源：http://hhs.cqqwz.cn

[U86] JS：空值合并
来源：http://oek.sweek.top

a ?? b
来源：http://ony.jqgfzy.top

[U87] JS：解构默认值
来源：http://tkd.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://ajy.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://czu.meibo888.top

{ ...a, ...b }
来源：http://tcr.jinghuilouyu.cn

[U89] JS：数组去重
来源：http://cvd.yvedp.cn

[...new Set(arr)]
来源：http://bdt.ydzc1.top

[U90] JS：数字数组排序
来源：http://ckg.hfpthk.cn

[...arr].sort((a, b) => a - b)
来源：http://foq.daria6918.cn

[U91] JS：对象键值遍历
来源：http://cex.c1oappe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xug.daria6918.cn

[U92] JS：深拷贝
来源：http://jkp.jqgfzy.top

structuredClone(obj)
来源：http://vyv.yangfankeji.com

[U93] JS：模板字符串
来源：http://eer.ywan-chungtsiang.top

`共 ${n} 条`
来源：http://abg.nanxuanxn.top

[U94] JS：箭头函数
来源：http://gii.hnxiangtu.top

const double = x => x * 2;
来源：http://zqv.yonumen.top

[U95] JS：Promise 包装
来源：http://yln.yanxiufei.cn

new Promise((resolve, reject) => {})
来源：http://aia.hongshengwenyu.top

[U96] JS：async/await 与异常
来源：http://sfo.zhongyouzk.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ydm.yanxiufei.cn

[U97] JS：并发请求
来源：http://hlt.andypj.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://fsq.ehwqpu.com

[U98] JS：fetch 带 JSON
来源：http://uwj.yuanzhike.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://czt.52xcode.cn

[U99] JS：事件监听
来源：http://lwz.fktsv.cn

el.addEventListener("click", e => {})
来源：http://ltt.bjfxy.top

[U100] JS：DOM 查询
来源：http://yxz.pycfn.com

document.querySelector(".item")
来源：http://nfi.jinghuilouyu.cn

[U101] JS：classList 操作
来源：http://wum.fehbvm.com

el.classList.toggle("active")
来源：http://bkx.zhixingplan.top

[U102] JS：本地存储
来源：http://han.zhoulong.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://aik.xuanzx.com

[U103] JS：定时器
来源：http://whf.smart0.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jee.uphjek.com

[U104] JS：防抖
来源：http://yfh.sjlbkw.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://avx.dianchejie.cn

[U105] JS：节流
来源：http://jzc.dashuyun.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bns.pycfn.com

[U106] JS：日期格式化
来源：http://ssb.ivvv.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uyx.fehbvm.com

[U107] JS：数字千分位
来源：http://suk.xuetiantiany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uyq.meibo888.top

[U108] JS：随机整数
来源：http://rxt.ivvv.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yjp.xinyue.icu

[U109] JS：数组分组
来源：http://hxh.zhixingplan.top

Object.groupBy(arr, x => x.type)
来源：http://gil.ydjk.org.cn

[U110] JS：数组分块
来源：http://xka.zhaomingkeji.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oke.fanxiaobao.xyz

[U111] JS：对象转 Map
来源：http://zqi.chenlongwang.top

new Map(Object.entries(obj))
来源：http://pbo.ywan-chungtsiang.top

[U112] JS：字符串补位
来源：http://xgw.birdmap.top

"7".padStart(3, "0")
来源：http://zgw.yj20258.top

[U113] JS：正则替换全部
来源：http://ftx.hcnkem.com

s.replaceAll("a", "b")
来源：http://dfl.guannengcc.top

[U114] JS：JSON 深比较
来源：http://ope.0kj1m.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hjz.snrcjt.cn

[U115] JS：生成 UUID
来源：http://yrk.cheryme.top

crypto.randomUUID()
来源：http://hkx.yfazqb.com

[U116] JS：类型检查（JSDoc）
来源：http://spe.cashguo.top

/** @param {string} name */ function f(name) {}
来源：http://aax.cdnleiting.top

[U117] JS：单元测试
来源：http://wvj.yvedp.cn

npm i -D vitest;  npx vitest
来源：http://dvp.andypj.xyz

[U118] JS：开发服务器
来源：http://ewn.zhixingplan.top

npm i -D vite;  npx vite
来源：http://ojm.hammf.cn

[U119] JS：生产构建
来源：http://oqw.birdmap.top

npx vite build
来源：http://lbx.dashuyun.cn

[U120] JS：读取环境变量（Vite）
来源：http://xgh.jlsjyb.cn

import.meta.env.VITE_API_URL
来源：http://bhe.yongpay.top

================================================================================
来源：http://ecj.andypj.xyz

统计汇总
来源：http://nit.shanyushiyangkeji.top

================================================================================
来源：http://axp.shangyingyoupin.top

按语言统计（条）：
来源：http://mgq.shangyingyoupin.top

Python ......... 252
来源：http://yrn.xingfuxueyuan.xyz

PHP ............ 252
来源：http://fgm.chenlongwang.top

JavaScript ..... 252
来源：http://cgm.svipenyu.cn

TypeScript ..... 212
来源：http://oxm.ybcxt.top

Java ........... 212
来源：http://pkz.feifeiyinyue.top

Go ............. 212
来源：http://kcx.cqqwz.cn

Ruby ........... 212
来源：http://kzn.aizwys.cn

C# ............. 212
来源：http://zqj.chenjidiqi.icu

C .............. 30
来源：http://wdf.hesvh.cn

C++ ............ 30
来源：http://dfv.jyoumei.cn

SQL ............ 90
来源：http://shd.jinqigufen.top

Bash ........... 80
来源：http://dif.sjlbkw.cn

Kotlin ......... 15
来源：http://ian.cucudq.cn

Swift .......... 15
来源：http://xbb.ivvv.top

Lua ............ 10
来源：http://gyd.wangdashe.top

Perl ........... 10
来源：http://zqd.chenlongwang.top

Scala .......... 10
来源：http://jbf.epnwcf.com

------------------------------------
来源：http://cgg.ppjwa.cn

合计 ........... 2106 条
来源：http://kbo.shangyingyoupin.top

按章节统计：
来源：http://tlz.xuetiantiany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yho.tian-w.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sfi.chenzaomai.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xyj.fanxiaobao.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rpi.jiagoushi.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ron.cdnleiting.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hww.hfpthk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eoc.tarul.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sbl.nwbrower.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yhr.jyoumei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fmq.bjfxy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lmo.jlsjyb.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hix.gaohongyu789.top


<!-- 参考信息 -->