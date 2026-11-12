代发 wailian999

[T47] Perl：正则捕获
来源：http://bkp.chenlongwang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pes.ydjk.org.cn

[T48] Perl：正则替换
来源：http://hvm.hongshengwenyu.top

$s =~ s/old/new/g;
来源：http://fkt.iojbl.cn

[T49] Perl：函数
来源：http://vuz.shuidangran.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gxv.ppjwa.cn

[T50] Perl：逐行读文件
来源：http://byd.fktsv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jkt.gzhubu.top

while (my $line = <$fh>) { print $line; }
来源：http://iko.hnqzz.top

[T51] Scala：Hello World
来源：http://mpu.yj20258888.top

println("Hello")
来源：http://cvp.zdbjq.cn

[T52] Scala：变量
来源：http://yzq.zdqjudy.top

val a = 1;  var b = 2
来源：http://pzy.cashguo.top

[T53] Scala：字符串插值
来源：http://lfo.gaohongyu789.top

s"值: $b"
来源：http://lux.sjlbkw.cn

[T54] Scala：集合映射
来源：http://sis.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://qdj.ivvv.top

[T55] Scala：集合过滤
来源：http://eqi.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ikk.daxiang520.top

[T56] Scala：样例类
来源：http://kaj.cashguo.top

case class User(name: String, age: Int)
来源：http://ijp.yj202588.top

[T57] Scala：模式匹配
来源：http://ute.gzhubu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bsw.cdnleiting.top

[T58] Scala：函数定义
来源：http://rfr.ppjwa.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qtu.iojbl.cn

[T59] Scala：循环
来源：http://vws.chenzaomai.com

for (i <- 1 to 10) println(i)
来源：http://wde.316326.xyz

[T60] Scala：折叠
来源：http://njs.yonumen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aye.gogol.net.cn

================================================================================
来源：http://ryk.epnwcf.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wxq.zhaomingkeji.xyz

================================================================================
来源：http://hpi.smart0.xyz

[U01] Py：创建虚拟环境
来源：http://jmt.fanxiaobao.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://gcx.meibo888.top

[U02] Py：导出 / 安装依赖
来源：http://tsz.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uyr.aizwys.cn

[U03] Py：加载 .env 配置
来源：http://rry.jiagoushi.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mzd.dashuyun.cn

[U04] Py：变量调试打印
来源：http://pxa.jinqigfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hru.zdqjudy.top

[U05] Py：列表去重且保序
来源：http://yqd.havefunace.top

list(dict.fromkeys(arr))
来源：http://bbw.zycfv.cn

[U06] Py：合并两个字典
来源：http://hwx.shanyushiyangtech.top

{**a, **b}
来源：http://ndn.gzhubu.top

[U07] Py：反转字典键值
来源：http://wte.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://rov.dashuyun.cn

[U08] Py：展平二维列表
来源：http://urn.sjlbkw.cn

[y for x in nested for y in x]
来源：http://eer.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://rhb.sysykeji.top

max(d, key=d.get)
来源：http://svj.zhixingplan.top

[U10] Py：按值排序字典
来源：http://xcd.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pxc.zhixingplan.top

[U11] Py：生成器表达式
来源：http://dpa.tanke756.top

(x * 2 for x in arr)
来源：http://mvk.yj20258.top

[U12] Py：取出现最多的 3 个元素
来源：http://ipi.sjlbkw.cn

Counter(arr).most_common(3)
来源：http://kfe.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://auz.fanxiaobao.xyz

deque(maxlen=10)
来源：http://gdc.tianlin.xyz

[U14] Py：分组收集到列表
来源：http://bvs.xylfe.cn

defaultdict(list)
来源：http://urp.kuanghao11.cn

[U15] Py：高精度计时
来源：http://gfx.yuanzhike.top

t = time.perf_counter()
来源：http://nww.daxiang520.top

[U16] Py：命令行参数解析
来源：http://rdk.ybcxt.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hci.uphjek.com

[U17] Py：初始化日志
来源：http://rnc.gotoacloud.top

logging.basicConfig(level=logging.INFO)
来源：http://alq.yanxiufei.cn

[U18] Py：预编译正则
来源：http://mdp.zhengqikj.top

pat = re.compile(r"\d+")
来源：http://ejc.redwolf501.top

[U19] Py：正则替换带回调
来源：http://awc.zhiwuduotai.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lpi.sufxvd.cn

[U20] Py：缓存函数结果
来源：http://tuf.chenzaomai.com

@functools.lru_cache(maxsize=None)
来源：http://ksy.c1oappe.top

[U21] Py：自定义上下文管理器
来源：http://uce.uphjek.com

@contextlib.contextmanager
来源：http://unl.yangfankeji.com

[U22] Py：矩阵转置
来源：http://oac.zdbjq.cn

list(zip(*m))
来源：http://tim.sweek.top

[U23] Py：分块读取大文件
来源：http://kvd.chenlongwang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zpa.shuidangran.top

[U24] Py：路径操作
来源：http://bdc.gaohongyu789.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uks.redwolf501.top

[U25] Py：CSV 按字典读
来源：http://pel.chenjidiqi.icu

csv.DictReader(f)
来源：http://pnl.ydjk.org.cn

[U26] Py：并发下载
来源：http://hyy.jyoumei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qvf.ywan-chungtsiang.top

[U27] Py：异步 HTTP
来源：http://ahn.meibo888.top

aiohttp.ClientSession() 配合 async with
来源：http://ycn.guowangkeji.top

[U28] Py：类型别名
来源：http://vca.sysykeji.top

UserId = int
来源：http://qoh.ehwqpu.com

[U29] Py：属性校验
来源：http://whz.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://rad.yvedp.cn

[U30] Py：数据类
来源：http://pcb.yvedp.cn

@dataclass(slots=True)
来源：http://aqd.yj20258888.top

[U31] Py：单测
来源：http://uoc.hfpthk.cn

python -m pytest -q
来源：http://rts.yvedp.cn

[U32] Py：代码格式化
来源：http://gsa.yueranfly.top

ruff format . && ruff check --fix .
来源：http://npa.wangdashe.top

[U33] Py：打包发布
来源：http://zbt.epnwcf.com

python -m build  （依赖 pyproject.toml）
来源：http://vlm.tanke756.top

[U34] Py：判断编码
来源：http://nyb.sxryk.cn

chardet.detect(raw)
来源：http://zhb.jyoumei.cn

[U35] Py：发送邮件
来源：http://age.zhoulong.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://auz.gzhubu.top

[U36] Py：定时任务
来源：http://dkl.redwolf501.top

schedule.every(10).minutes.do(job)
来源：http://mmv.nanxuanxn.top

[U37] Py：读写 Excel
来源：http://toy.fanxiaobao.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://ksp.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://ozp.yuxming.cn

Path(__file__).resolve().parent
来源：http://gjn.tarul.cn

[U39] Py：判断是否在交互环境
来源：http://otk.zdqjudy.top

sys.stdout.isatty()
来源：http://fxh.zhiwuduotai.top

[U40] Py：打印到标准错误
来源：http://npf.jyoumei.cn

print("err", file=sys.stderr)
来源：http://auc.jyoumei.cn

[U41] PHP：初始化 Composer 项目
来源：http://dha.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://nnt.hnqzz.top

[U42] PHP：PSR-4 自动加载
来源：http://hwt.mhx1999.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yqc.ehwqpu.com

[U43] PHP：声明命名空间
来源：http://bom.xylfe.cn

namespace App\Http;
来源：http://kzf.nanxinkj.top

[U44] PHP：开启严格类型
来源：http://vgk.daria6918.cn

declare(strict_types=1);
来源：http://elr.52xcode.cn

[U45] PHP：类型声明与返回类型
来源：http://xjw.zhoulong.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://ngd.cheryme.top

[U46] PHP：可空类型
来源：http://xcb.pengpengdd.cyou

?string $name = null
来源：http://peq.tian-w.cn

[U47] PHP：联合类型
来源：http://pxk.snrcjt.cn

int|string $id
来源：http://upn.zdbjq.cn

[U48] PHP：纯枚举
来源：http://sum.jinqigfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ofl.zycfv.cn

[U49] PHP：只读属性
来源：http://clp.xinyue.icu

public readonly string $name
来源：http://cnc.hcnkem.com

[U50] PHP：构造器属性提升
来源：http://run.chenlongwang.top

public function __construct(private int $id) {}
来源：http://ydp.gzhubu.top

[U51] PHP：数组解构
来源：http://lhp.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://plm.jyoumei.cn

[U52] PHP：箭头函数
来源：http://dgg.zhijiandao.cn

$double = fn($x) => $x * 2;
来源：http://gdm.bbcook.cn

[U53] PHP：空合并运算符
来源：http://rcu.sysykeji.top

$v = $a ?? $b ?? "default";
来源：http://dgx.xziqi.cn

[U54] PHP：空安全调用
来源：http://mqt.andypj.xyz

$obj?->method()
来源：http://uea.birdmap.top

[U55] PHP：match 表达式
来源：http://dun.chenlongwang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://icz.dianchejie.cn

[U56] PHP：命名参数
来源：http://rya.ppjwa.cn

f(a: 1, b: 2)
来源：http://kzk.yj202588.top

[U57] PHP：字符串插值
来源：http://wqq.yueranfly.top

"值: {$a}"
来源：http://zwr.ctjpmb.com

[U58] PHP：数组三件套
来源：http://kgd.redwolf501.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zsv.wangdashe.top

[U59] PHP：自定义排序
来源：http://kbs.iojbl.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bgw.mhx1999.top

[U60] PHP：JSON 编解码
来源：http://tuh.birdmap.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zqc.hongshengwenyu.top

[U61] PHP：正则
来源：http://cbt.hesvh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wth.316326.xyz

[U62] PHP：日期对象
来源：http://hgw.hfpthk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mtt.dashuyun.cn

[U63] PHP：文件读写
来源：http://rxm.hysaishi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wts.jqgufenzy.top

[U64] PHP：目录遍历
来源：http://ein.yuanzhike.top

glob("dir/*.php");  scandir("dir");
来源：http://pup.xuanzx.com

[U65] PHP：会话
来源：http://ora.yvedp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ytf.hammf.cn

[U66] PHP：设置 Cookie
来源：http://rdx.hcnkem.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tyg.yfazqb.com

[U67] PHP：处理文件上传
来源：http://ruy.shzxlz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://afd.iojbl.cn

[U68] PHP：PDO 连接
来源：http://bgv.snrcjt.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zgn.smart0.xyz

[U69] PHP：PDO 预处理
来源：http://hoh.zhixingplan.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sdw.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://plm.yueranfly.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dms.c1oappe.top

[U71] PHP：抛出异常
来源：http://ibx.yj20258.top

throw new RuntimeException("失败", 500);
来源：http://rzf.xingfuxueyuan.xyz

[U72] PHP：写错误日志
来源：http://flw.jinyuanbaomall.cn

error_log("失败: " . $e->getMessage());
来源：http://unq.yvedp.cn

[U73] PHP：读取 ini 配置
来源：http://hzt.cheryme.top

parse_ini_file("config.ini", true)
来源：http://ahm.chenlongwang.top

[U74] PHP：读取环境变量
来源：http://msp.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://xfy.yangfankeji.com

[U75] PHP：依赖注入
来源：http://ibz.jinqigufen.top

composer require psr/container
来源：http://vac.zycfv.cn

[U76] PHP：简单路由
来源：http://ooq.shanyushiyangtech.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://edy.9152youxi.cn

[U77] PHP：模板渲染
来源：http://viw.wangshuangyany.cn

composer require twig/twig
来源：http://cjs.hfpthk.cn

[U78] PHP：单元测试
来源：http://bug.jinyuanbaomall.cn

composer require --dev phpunit/phpunit
来源：http://idz.cdnleiting.top

[U79] PHP：静态分析
来源：http://zoe.c1oappe.top

composer require --dev phpstan/phpstan
来源：http://aty.epnwcf.com

[U80] PHP：代码规范修复
来源：http://cru.yj202588.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bzu.xinyue.icu

[U81] JS：初始化项目
来源：http://hpv.zhiwuduotai.top

npm init -y;  npm i express
来源：http://yrt.dashuyun.cn

[U82] JS：package.json 脚本
来源：http://whj.snrcjt.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gnb.yonumen.top

[U83] JS：ES Module 导入导出
来源：http://pdr.chenzaomai.com

export const a = 1;  import { a } from "./m.js";
来源：http://euf.vqdsnc.cn

[U84] JS：CommonJS 写法
来源：http://zqj.hongshengwenyu.top

module.exports = { a };  const { a } = require("./m");
来源：http://sjp.jinghuilouyu.cn

[U85] JS：可选链
来源：http://pym.dianchejie.cn

a?.b?.c
来源：http://lga.sufxvd.cn

[U86] JS：空值合并
来源：http://gxc.jyoumei.cn

a ?? b
来源：http://yui.cheryme.top

[U87] JS：解构默认值
来源：http://jjo.hesvh.cn

const { a = 1, b = 2 } = obj;
来源：http://fyf.hywenlv.cn

[U88] JS：对象展开合并
来源：http://oum.bbcook.cn

{ ...a, ...b }
来源：http://rkb.hysaishi.cn

[U89] JS：数组去重
来源：http://jio.dashuyun.cn

[...new Set(arr)]
来源：http://bpk.epnwcf.com

[U90] JS：数字数组排序
来源：http://lrt.jinghuilouyu.cn

[...arr].sort((a, b) => a - b)
来源：http://lgc.cucudq.cn

[U91] JS：对象键值遍历
来源：http://oha.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hdf.shuidangran.top

[U92] JS：深拷贝
来源：http://csd.xingfuxueyuan.xyz

structuredClone(obj)
来源：http://ezw.jinqigufen.top

[U93] JS：模板字符串
来源：http://fwc.shzxlz.cn

`共 ${n} 条`
来源：http://pwr.zhengqikj.top

[U94] JS：箭头函数
来源：http://hks.gogol.net.cn

const double = x => x * 2;
来源：http://hui.dashuyun.cn

[U95] JS：Promise 包装
来源：http://tdp.yj202588.top

new Promise((resolve, reject) => {})
来源：http://qor.guannengcc.top

[U96] JS：async/await 与异常
来源：http://oho.bbcook.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mei.cheryme.top

[U97] JS：并发请求
来源：http://qgr.gotoacloud.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://nwp.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://nqv.pengpengdd.cyou

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zwf.smart0.xyz

[U99] JS：事件监听
来源：http://xzl.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://ymc.redwolf501.top

[U100] JS：DOM 查询
来源：http://whh.52xcode.cn

document.querySelector(".item")
来源：http://rqd.nanxinkj.top

[U101] JS：classList 操作
来源：http://rrk.fengsongda.top

el.classList.toggle("active")
来源：http://cvf.jinqigufen.top

[U102] JS：本地存储
来源：http://icd.ydzc1.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bzi.ydjk.org.cn

[U103] JS：定时器
来源：http://bts.yonumen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tzp.zhijiandao.cn

[U104] JS：防抖
来源：http://otw.guowangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zuk.tanke756.top

[U105] JS：节流
来源：http://shm.gogol.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tmz.jlsjyb.cn

[U106] JS：日期格式化
来源：http://zed.zhoulong.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zfj.wangdashe.top

[U107] JS：数字千分位
来源：http://avc.jlsjyb.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hyh.zhoulong.xyz

[U108] JS：随机整数
来源：http://jxt.c1oappe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gra.tian-w.cn

[U109] JS：数组分组
来源：http://soa.yanxiufei.cn

Object.groupBy(arr, x => x.type)
来源：http://aeq.aizwys.cn

[U110] JS：数组分块
来源：http://ids.yanxiufei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bxm.meibo888.top

[U111] JS：对象转 Map
来源：http://fvu.zhiwuduotai.top

new Map(Object.entries(obj))
来源：http://obh.meibo888.top

[U112] JS：字符串补位
来源：http://len.0kj1m.cn

"7".padStart(3, "0")
来源：http://wnc.chenlongwang.top

[U113] JS：正则替换全部
来源：http://ajt.havefunace.top

s.replaceAll("a", "b")
来源：http://dki.tanke756.top

[U114] JS：JSON 深比较
来源：http://pwl.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cfm.shanyushiyangtech.top

[U115] JS：生成 UUID
来源：http://ksz.chenzaomai.com

crypto.randomUUID()
来源：http://qtn.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://ktf.daxiang520.top

/** @param {string} name */ function f(name) {}
来源：http://hws.tarul.cn

[U117] JS：单元测试
来源：http://scz.cashguo.top

npm i -D vitest;  npx vitest
来源：http://kxa.svipenyu.cn

[U118] JS：开发服务器
来源：http://tpm.birdmap.top

npm i -D vite;  npx vite
来源：http://qfv.yj20258888.top

[U119] JS：生产构建
来源：http://tpd.quarkkingdee.top

npx vite build
来源：http://pty.svipenyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://vmg.yongpay.top

import.meta.env.VITE_API_URL
来源：http://ghh.yongpay.top

================================================================================
来源：http://ovj.316326.xyz

统计汇总
来源：http://ase.quarkkingdee.top

================================================================================
来源：http://ydy.yj20258888.top

按语言统计（条）：
来源：http://rof.yonumen.top

Python ......... 252
来源：http://kzx.daxiang520.top

PHP ............ 252
来源：http://hsd.chenjidiqi.icu

JavaScript ..... 252
来源：http://hek.zdbjq.cn

TypeScript ..... 212
来源：http://eqg.jianghu66.top

Java ........... 212
来源：http://hiw.wangshuangyany.cn

Go ............. 212
来源：http://xcv.fehbvm.com

Ruby ........... 212
来源：http://uzv.shangyingyoupin.top

C# ............. 212
来源：http://ttd.shuidangran.top

C .............. 30
来源：http://zut.birdmap.top

C++ ............ 30
来源：http://jak.yonumen.top

SQL ............ 90
来源：http://guu.shanyushiyangkeji.top

Bash ........... 80
来源：http://gyz.hfpthk.cn

Kotlin ......... 15
来源：http://wcr.jiagoushi.top

Swift .......... 15
来源：http://sra.wangshuangyany.cn

Lua ............ 10
来源：http://qkp.yanxiufei.cn

Perl ........... 10
来源：http://yce.iojbl.cn

Scala .......... 10
来源：http://bsl.tarul.cn

------------------------------------
来源：http://udw.gaohongyu789.top

合计 ........... 2106 条
来源：http://qvs.guannengcc.top

按章节统计：
来源：http://zqo.kuanghao11.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ajj.yueranfly.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jda.cqqwz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://equ.ywan-chungtsiang.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fhb.yanxiufei.cn


<!-- 参考信息 -->