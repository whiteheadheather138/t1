代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://zbk.hnqzz.top

[T51] Scala：Hello World
来源：http://tjm.0kj1m.cn

println("Hello")
来源：http://iqc.0kj1m.cn

[T52] Scala：变量
来源：http://vng.dianchejie.cn

val a = 1;  var b = 2
来源：http://qtt.sufxvd.cn

[T53] Scala：字符串插值
来源：http://eqd.shuidangran.top

s"值: $b"
来源：http://wmp.yuanzhike.top

[T54] Scala：集合映射
来源：http://sxz.zdbjq.cn

List(1, 2, 3).map(_ * 2)
来源：http://swu.zhixingplan.top

[T55] Scala：集合过滤
来源：http://orn.yueranfly.top

List(1, 2, 3).filter(_ > 1)
来源：http://eag.shuidangran.top

[T56] Scala：样例类
来源：http://elb.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://fww.yuanzhike.top

[T57] Scala：模式匹配
来源：http://gdr.xylfe.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dxt.wangdashe.top

[T58] Scala：函数定义
来源：http://utp.ywan-chungtsiang.top

def add(a: Int, b: Int): Int = a + b
来源：http://hcj.hammf.cn

[T59] Scala：循环
来源：http://qci.hfpthk.cn

for (i <- 1 to 10) println(i)
来源：http://zwr.hfpthk.cn

[T60] Scala：折叠
来源：http://wuc.jlsjyb.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://llc.ehwqpu.com

================================================================================
来源：http://zpf.epnwcf.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://euj.fzhhl.top

================================================================================
来源：http://jsr.chenlongwang.top

[U01] Py：创建虚拟环境
来源：http://cxm.jiagoushi.top

python -m venv .venv && source .venv/bin/activate
来源：http://nil.shanyushiyangtech.top

[U02] Py：导出 / 安装依赖
来源：http://chq.aizwys.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lcc.haohaochexian.top

[U03] Py：加载 .env 配置
来源：http://nff.hesvh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ynb.bjfxy.top

[U04] Py：变量调试打印
来源：http://jxc.daxiang520.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jqp.sysykeji.top

[U05] Py：列表去重且保序
来源：http://ncl.sxryk.cn

list(dict.fromkeys(arr))
来源：http://ogq.ctjpmb.com

[U06] Py：合并两个字典
来源：http://bfx.redwolf501.top

{**a, **b}
来源：http://bee.ybcxt.top

[U07] Py：反转字典键值
来源：http://mvy.yangfankeji.com

{v: k for k, v in d.items()}
来源：http://hsg.yueranfly.top

[U08] Py：展平二维列表
来源：http://icy.fktsv.cn

[y for x in nested for y in x]
来源：http://wuv.nwbrower.top

[U09] Py：字典取最大值的键
来源：http://kqr.smart0.xyz

max(d, key=d.get)
来源：http://vun.jiagoushi.top

[U10] Py：按值排序字典
来源：http://sau.hywenlv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ggz.tianlin.xyz

[U11] Py：生成器表达式
来源：http://gws.fehbvm.com

(x * 2 for x in arr)
来源：http://pbs.cheryme.top

[U12] Py：取出现最多的 3 个元素
来源：http://ujl.bbcook.cn

Counter(arr).most_common(3)
来源：http://ohd.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://bpu.sweek.top

deque(maxlen=10)
来源：http://kei.ehwqpu.com

[U14] Py：分组收集到列表
来源：http://eif.ydjk.org.cn

defaultdict(list)
来源：http://cdi.svipenyu.cn

[U15] Py：高精度计时
来源：http://alm.ctjpmb.com

t = time.perf_counter()
来源：http://lsj.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://rmt.wangdashe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qki.yanxiufei.cn

[U17] Py：初始化日志
来源：http://omi.aizwys.cn

logging.basicConfig(level=logging.INFO)
来源：http://qfr.hfpthk.cn

[U18] Py：预编译正则
来源：http://rko.epnwcf.com

pat = re.compile(r"\d+")
来源：http://wvq.bbcook.cn

[U19] Py：正则替换带回调
来源：http://gax.ywan-chungtsiang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rca.xylfe.cn

[U20] Py：缓存函数结果
来源：http://zwu.iojbl.cn

@functools.lru_cache(maxsize=None)
来源：http://quw.xinyue.icu

[U21] Py：自定义上下文管理器
来源：http://jmj.jinqigufen.top

@contextlib.contextmanager
来源：http://xuh.yfazqb.com

[U22] Py：矩阵转置
来源：http://jom.fzhhl.top

list(zip(*m))
来源：http://xnx.zdqjudy.top

[U23] Py：分块读取大文件
来源：http://nqe.pengpengdd.cyou

for chunk in iter(lambda: f.read(8192), b""):
来源：http://whm.quarkkingdee.top

[U24] Py：路径操作
来源：http://wgo.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://khr.jianghu66.top

[U25] Py：CSV 按字典读
来源：http://ckf.vqdsnc.cn

csv.DictReader(f)
来源：http://vmn.aibaodan.cn

[U26] Py：并发下载
来源：http://tij.wangshuangyany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wmr.nwbrower.top

[U27] Py：异步 HTTP
来源：http://bss.zhixingplan.top

aiohttp.ClientSession() 配合 async with
来源：http://jln.pycfn.com

[U28] Py：类型别名
来源：http://geg.pengpengdd.cyou

UserId = int
来源：http://xdc.shangyingyoupin.top

[U29] Py：属性校验
来源：http://dgx.zhoulong.xyz

@property 与 @x.setter 配合
来源：http://kwf.cucudq.cn

[U30] Py：数据类
来源：http://gtl.jinqigfzy.top

@dataclass(slots=True)
来源：http://ikf.chenzaomai.com

[U31] Py：单测
来源：http://xgh.cashguo.top

python -m pytest -q
来源：http://qzi.hfpthk.cn

[U32] Py：代码格式化
来源：http://zql.zhaomingkeji.xyz

ruff format . && ruff check --fix .
来源：http://xem.fehbvm.com

[U33] Py：打包发布
来源：http://jdv.zhengqikj.top

python -m build  （依赖 pyproject.toml）
来源：http://xrt.zhiwuduotai.top

[U34] Py：判断编码
来源：http://zuv.sysykeji.top

chardet.detect(raw)
来源：http://ctc.zhengqikj.top

[U35] Py：发送邮件
来源：http://ugx.hnqzz.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vjb.jinqigufen.top

[U36] Py：定时任务
来源：http://bea.yfazqb.com

schedule.every(10).minutes.do(job)
来源：http://fag.cdnleiting.top

[U37] Py：读写 Excel
来源：http://pqy.shanyushiyangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://jjd.zhixingplan.top

[U38] Py：获取脚本所在目录
来源：http://say.yuxming.cn

Path(__file__).resolve().parent
来源：http://rdt.chenlongwang.top

[U39] Py：判断是否在交互环境
来源：http://iht.yueranfly.top

sys.stdout.isatty()
来源：http://qcs.yueranfly.top

[U40] Py：打印到标准错误
来源：http://rvu.nanxinkj.top

print("err", file=sys.stderr)
来源：http://usa.tarul.cn

[U41] PHP：初始化 Composer 项目
来源：http://vbk.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://vme.shzxlz.cn

[U42] PHP：PSR-4 自动加载
来源：http://qvj.xuanzx.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sek.yuanzhike.top

[U43] PHP：声明命名空间
来源：http://wlj.svipenyu.cn

namespace App\Http;
来源：http://xxo.pycfn.com

[U44] PHP：开启严格类型
来源：http://hfh.fzhhl.top

declare(strict_types=1);
来源：http://kap.fehbvm.com

[U45] PHP：类型声明与返回类型
来源：http://koc.xuetiantiany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ezl.yueranfly.top

[U46] PHP：可空类型
来源：http://djt.jinghuilouyu.cn

?string $name = null
来源：http://ffq.mhx1999.top

[U47] PHP：联合类型
来源：http://vge.bjfxy.top

int|string $id
来源：http://pdi.feifeiyinyue.top

[U48] PHP：纯枚举
来源：http://lsi.ybcxt.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ypo.dianchejie.cn

[U49] PHP：只读属性
来源：http://fsy.gzhubu.top

public readonly string $name
来源：http://tqw.yj20258888.top

[U50] PHP：构造器属性提升
来源：http://ezp.xziqi.cn

public function __construct(private int $id) {}
来源：http://hhe.ywan-chungtsiang.top

[U51] PHP：数组解构
来源：http://nka.sweek.top

[$a, $b] = $arr;
来源：http://pbs.gzhubu.top

[U52] PHP：箭头函数
来源：http://luq.chenjidiqi.icu

$double = fn($x) => $x * 2;
来源：http://bmu.uphjek.com

[U53] PHP：空合并运算符
来源：http://ljf.yj20258.top

$v = $a ?? $b ?? "default";
来源：http://ykm.hesvh.cn

[U54] PHP：空安全调用
来源：http://tbj.xziqi.cn

$obj?->method()
来源：http://dib.9152youxi.cn

[U55] PHP：match 表达式
来源：http://ldq.9152youxi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mos.xuetiantiany.cn

[U56] PHP：命名参数
来源：http://ips.xuanzx.com

f(a: 1, b: 2)
来源：http://ken.0kj1m.cn

[U57] PHP：字符串插值
来源：http://rvc.jinyuanbaomall.cn

"值: {$a}"
来源：http://pfq.ehwqpu.com

[U58] PHP：数组三件套
来源：http://zjv.snrcjt.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iut.svipenyu.cn

[U59] PHP：自定义排序
来源：http://dmv.wangshuangyany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vpu.svipenyu.cn

[U60] PHP：JSON 编解码
来源：http://ypt.chenlongwang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://aho.zhengqikj.top

[U61] PHP：正则
来源：http://wwt.yfazqb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ljr.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://nro.sysykeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ehc.xylfe.cn

[U63] PHP：文件读写
来源：http://kfj.jinqigufen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wjq.zdbjq.cn

[U64] PHP：目录遍历
来源：http://znm.gogol.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://hgf.hnqzz.top

[U65] PHP：会话
来源：http://qvu.zhixingplan.top

session_start();  $_SESSION["uid"] = 1;
来源：http://obo.yvedp.cn

[U66] PHP：设置 Cookie
来源：http://ami.mhx1999.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uhj.aibaodan.cn

[U67] PHP：处理文件上传
来源：http://elz.zhongyouzk.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mwd.xylfe.cn

[U68] PHP：PDO 连接
来源：http://ipj.andypj.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zce.kuanghao11.cn

[U69] PHP：PDO 预处理
来源：http://dlq.jinyuanbaomall.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tkt.vqdsnc.cn

[U70] PHP：PDO 事务
来源：http://hav.sjlbkw.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lce.tanke756.top

[U71] PHP：抛出异常
来源：http://rdg.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://vfw.fktsv.cn

[U72] PHP：写错误日志
来源：http://xhj.shzxlz.cn

error_log("失败: " . $e->getMessage());
来源：http://zyj.cashguo.top

[U73] PHP：读取 ini 配置
来源：http://ueu.guannengcc.top

parse_ini_file("config.ini", true)
来源：http://yjm.fehbvm.com

[U74] PHP：读取环境变量
来源：http://ohl.chenjidiqi.icu

getenv("APP_ENV") ?: "production"
来源：http://esl.mhx1999.top

[U75] PHP：依赖注入
来源：http://rgw.nwbrower.top

composer require psr/container
来源：http://foe.dianchejie.cn

[U76] PHP：简单路由
来源：http://pxc.gogol.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xqc.zhiwuduotai.top

[U77] PHP：模板渲染
来源：http://qik.zhoulong.xyz

composer require twig/twig
来源：http://exw.andypj.xyz

[U78] PHP：单元测试
来源：http://qxy.aibaodan.cn

composer require --dev phpunit/phpunit
来源：http://mlm.zdbjq.cn

[U79] PHP：静态分析
来源：http://eiw.xuanzx.com

composer require --dev phpstan/phpstan
来源：http://vcu.yueranfly.top

[U80] PHP：代码规范修复
来源：http://thf.hesvh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tmy.ivvv.top

[U81] JS：初始化项目
来源：http://xqf.hongshengwenyu.top

npm init -y;  npm i express
来源：http://ngb.ydzc1.top

[U82] JS：package.json 脚本
来源：http://nma.vqdsnc.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ifi.hnqzz.top

[U83] JS：ES Module 导入导出
来源：http://rmx.chenzaomai.com

export const a = 1;  import { a } from "./m.js";
来源：http://oyy.fengsongda.top

[U84] JS：CommonJS 写法
来源：http://plh.snrcjt.cn

module.exports = { a };  const { a } = require("./m");
来源：http://eti.sufxvd.cn

[U85] JS：可选链
来源：http://ynz.yueranfly.top

a?.b?.c
来源：http://jfd.pengpengdd.cyou

[U86] JS：空值合并
来源：http://aum.zhaomingkeji.xyz

a ?? b
来源：http://uqh.yanxiufei.cn

[U87] JS：解构默认值
来源：http://urt.zhijiandao.cn

const { a = 1, b = 2 } = obj;
来源：http://zgq.zhaomingkeji.xyz

[U88] JS：对象展开合并
来源：http://stp.shzxlz.cn

{ ...a, ...b }
来源：http://ryc.vqdsnc.cn

[U89] JS：数组去重
来源：http://ash.andypj.xyz

[...new Set(arr)]
来源：http://zva.jlsjyb.cn

[U90] JS：数字数组排序
来源：http://jjf.dianchejie.cn

[...arr].sort((a, b) => a - b)
来源：http://idt.zhijiandao.cn

[U91] JS：对象键值遍历
来源：http://xnz.pycfn.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ndu.dianchejie.cn

[U92] JS：深拷贝
来源：http://xhh.ctjpmb.com

structuredClone(obj)
来源：http://sgy.fengsongda.top

[U93] JS：模板字符串
来源：http://mag.shzxlz.cn

`共 ${n} 条`
来源：http://hzw.sufxvd.cn

[U94] JS：箭头函数
来源：http://ufb.vqdsnc.cn

const double = x => x * 2;
来源：http://kue.cashguo.top

[U95] JS：Promise 包装
来源：http://umr.jqgfzy.top

new Promise((resolve, reject) => {})
来源：http://vni.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://mob.nanxuanxn.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://njc.zhoulong.xyz

[U97] JS：并发请求
来源：http://fno.sysykeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://urc.sxryk.cn

[U98] JS：fetch 带 JSON
来源：http://bij.feifeiyinyue.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ygf.bbcook.cn

[U99] JS：事件监听
来源：http://fmp.sxryk.cn

el.addEventListener("click", e => {})
来源：http://yja.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://bin.ywan-chungtsiang.top

document.querySelector(".item")
来源：http://epa.jlsjyb.cn

[U101] JS：classList 操作
来源：http://rcu.ivvv.top

el.classList.toggle("active")
来源：http://alz.ivvv.top

[U102] JS：本地存储
来源：http://mvw.hcnkem.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ugl.ppjwa.cn

[U103] JS：定时器
来源：http://eii.birdmap.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vcf.jinyuanbaomall.cn

[U104] JS：防抖
来源：http://ijs.yueranfly.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lcq.yueranfly.top

[U105] JS：节流
来源：http://mbk.zhoulong.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ujr.snrcjt.cn

[U106] JS：日期格式化
来源：http://zrd.xziqi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ekw.zdbjq.cn

[U107] JS：数字千分位
来源：http://nui.sysykeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wpr.zdqjudy.top

[U108] JS：随机整数
来源：http://whx.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://efj.ivvv.top

[U109] JS：数组分组
来源：http://xbo.guannengcc.top

Object.groupBy(arr, x => x.type)
来源：http://hau.vqdsnc.cn

[U110] JS：数组分块
来源：http://raf.tianlin.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kee.xylfe.cn

[U111] JS：对象转 Map
来源：http://kvs.dashuyun.cn

new Map(Object.entries(obj))
来源：http://teh.ctjpmb.com

[U112] JS：字符串补位
来源：http://rtc.fzhhl.top

"7".padStart(3, "0")
来源：http://zfa.ivvv.top

[U113] JS：正则替换全部
来源：http://ynd.yangfankeji.com

s.replaceAll("a", "b")
来源：http://mqt.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://ngl.yuanzhike.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fix.gzhubu.top

[U115] JS：生成 UUID
来源：http://vrw.yongpay.top

crypto.randomUUID()
来源：http://csh.yvedp.cn

[U116] JS：类型检查（JSDoc）
来源：http://utm.redwolf501.top

/** @param {string} name */ function f(name) {}
来源：http://tqa.hnqzz.top

[U117] JS：单元测试
来源：http://glo.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://lrw.bjfxy.top

[U118] JS：开发服务器
来源：http://biu.hammf.cn

npm i -D vite;  npx vite
来源：http://zau.zhaomingkeji.xyz

[U119] JS：生产构建
来源：http://koc.jqgfzy.top

npx vite build
来源：http://wrx.ctjpmb.com

[U120] JS：读取环境变量（Vite）
来源：http://kif.feifeiyinyue.top

import.meta.env.VITE_API_URL
来源：http://rjf.jinghuilouyu.cn

================================================================================
来源：http://iii.ehwqpu.com

统计汇总
来源：http://hhi.hammf.cn

================================================================================
来源：http://crc.ydzc1.top

按语言统计（条）：
来源：http://kiv.yueranfly.top

Python ......... 252
来源：http://wyv.jqgufenzy.top

PHP ............ 252
来源：http://jbi.pycfn.com

JavaScript ..... 252
来源：http://jba.zycfv.cn

TypeScript ..... 212
来源：http://qxe.vqdsnc.cn

Java ........... 212
来源：http://iog.yuxming.cn

Go ............. 212
来源：http://uat.mhx1999.top

Ruby ........... 212
来源：http://jxa.daxiang520.top

C# ............. 212
来源：http://qbn.ehwqpu.com

C .............. 30
来源：http://hjv.snrcjt.cn

C++ ............ 30
来源：http://xbh.shuidangran.top

SQL ............ 90
来源：http://ygx.zhiwuduotai.top

Bash ........... 80
来源：http://gfx.jqgufenzy.top

Kotlin ......... 15
来源：http://ecw.zhixingplan.top

Swift .......... 15
来源：http://aqb.hnxiangtu.top

Lua ............ 10
来源：http://htp.yanxiufei.cn

Perl ........... 10
来源：http://cdz.cashguo.top

Scala .......... 10
来源：http://jjf.gogol.net.cn

------------------------------------
来源：http://xtx.jinghuilouyu.cn

合计 ........... 2106 条
来源：http://oci.ywan-chungtsiang.top

按章节统计：
来源：http://htr.fengsongda.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ylj.xinyue.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dgl.zhoulong.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fsw.316326.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bee.feifeiyinyue.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nfm.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ecm.fengsongda.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pjr.yueranfly.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vdq.hysaishi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bdc.snrcjt.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gug.yvedp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lkw.shangyingyoupin.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xwn.zdqjudy.top


<!-- 参考信息 -->