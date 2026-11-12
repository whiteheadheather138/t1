代发 wailian999

[T45] Perl：数组遍历
来源：http://ocy.sjlbkw.cn

for my $x (@arr) { print $x; }
来源：http://miv.cucudq.cn

[T46] Perl：哈希操作
来源：http://qnp.shanyushiyangtech.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xyj.nanxinkj.top

[T47] Perl：正则捕获
来源：http://iit.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://chm.yongpay.top

[T48] Perl：正则替换
来源：http://duc.chenjidiqi.icu

$s =~ s/old/new/g;
来源：http://quj.iojbl.cn

[T49] Perl：函数
来源：http://zon.ehwqpu.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qwd.xylfe.cn

[T50] Perl：逐行读文件
来源：http://nwx.chenzaomai.com

open my $fh, "<", "a.txt" or die $!;
来源：http://nja.hnxiangtu.top

while (my $line = <$fh>) { print $line; }
来源：http://zqe.yuxming.cn

[T51] Scala：Hello World
来源：http://eih.tarul.cn

println("Hello")
来源：http://rdt.xziqi.cn

[T52] Scala：变量
来源：http://ywb.nanxuanxn.top

val a = 1;  var b = 2
来源：http://hqo.cdnleiting.top

[T53] Scala：字符串插值
来源：http://pey.jinqigufen.top

s"值: $b"
来源：http://uod.jqgufenzy.top

[T54] Scala：集合映射
来源：http://rqp.ydjk.org.cn

List(1, 2, 3).map(_ * 2)
来源：http://eno.fzhhl.top

[T55] Scala：集合过滤
来源：http://kgb.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zbb.cashguo.top

[T56] Scala：样例类
来源：http://unz.zycfv.cn

case class User(name: String, age: Int)
来源：http://mfb.guowangkeji.top

[T57] Scala：模式匹配
来源：http://arh.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dji.aibaodan.cn

[T58] Scala：函数定义
来源：http://bed.uphjek.com

def add(a: Int, b: Int): Int = a + b
来源：http://kuz.chenlongwang.top

[T59] Scala：循环
来源：http://lmw.xingfuxueyuan.xyz

for (i <- 1 to 10) println(i)
来源：http://nrt.pengpengdd.cyou

[T60] Scala：折叠
来源：http://fry.smart0.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zxm.yueranfly.top

================================================================================
来源：http://ney.hysaishi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nuc.xuetiantiany.cn

================================================================================
来源：http://fdu.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://aqy.ctjpmb.com

python -m venv .venv && source .venv/bin/activate
来源：http://evp.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://clz.fanxiaobao.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pxt.tian-w.cn

[U03] Py：加载 .env 配置
来源：http://bgf.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://osv.vqdsnc.cn

[U04] Py：变量调试打印
来源：http://ouq.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kcg.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://szf.hfpthk.cn

list(dict.fromkeys(arr))
来源：http://brl.zhengqikj.top

[U06] Py：合并两个字典
来源：http://bhp.jqgfzy.top

{**a, **b}
来源：http://vuc.hesvh.cn

[U07] Py：反转字典键值
来源：http://obw.aizwys.cn

{v: k for k, v in d.items()}
来源：http://vmj.hongshengwenyu.top

[U08] Py：展平二维列表
来源：http://rxx.hongshengwenyu.top

[y for x in nested for y in x]
来源：http://uuq.wangdashe.top

[U09] Py：字典取最大值的键
来源：http://hof.fanxiaobao.xyz

max(d, key=d.get)
来源：http://rlx.haohaochexian.top

[U10] Py：按值排序字典
来源：http://epj.zhengqikj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ntv.birdmap.top

[U11] Py：生成器表达式
来源：http://uak.vehdjk.com

(x * 2 for x in arr)
来源：http://wpf.tanke756.top

[U12] Py：取出现最多的 3 个元素
来源：http://ijb.pengpengdd.cyou

Counter(arr).most_common(3)
来源：http://qpd.yuxming.cn

[U13] Py：固定长度队列
来源：http://ofn.vqdsnc.cn

deque(maxlen=10)
来源：http://obr.sysykeji.top

[U14] Py：分组收集到列表
来源：http://ctk.chenzaomai.com

defaultdict(list)
来源：http://aqq.birdmap.top

[U15] Py：高精度计时
来源：http://yeb.fehbvm.com

t = time.perf_counter()
来源：http://ier.yfazqb.com

[U16] Py：命令行参数解析
来源：http://qvm.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mjv.yuanzhike.top

[U17] Py：初始化日志
来源：http://kdc.zhijiandao.cn

logging.basicConfig(level=logging.INFO)
来源：http://kjv.jinyuanbaomall.cn

[U18] Py：预编译正则
来源：http://ayg.zycfv.cn

pat = re.compile(r"\d+")
来源：http://cqn.meibo888.top

[U19] Py：正则替换带回调
来源：http://pqh.nanxinkj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://stn.jianghu66.top

[U20] Py：缓存函数结果
来源：http://fqw.xziqi.cn

@functools.lru_cache(maxsize=None)
来源：http://ifj.gzhubu.top

[U21] Py：自定义上下文管理器
来源：http://ysi.yj202588.top

@contextlib.contextmanager
来源：http://mub.zhixingplan.top

[U22] Py：矩阵转置
来源：http://fwy.chenjidiqi.icu

list(zip(*m))
来源：http://lbg.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://nxi.xingfuxueyuan.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://exw.sweek.top

[U24] Py：路径操作
来源：http://avt.ehwqpu.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uyr.ydzc1.top

[U25] Py：CSV 按字典读
来源：http://hyf.bbcook.cn

csv.DictReader(f)
来源：http://qab.wangdashe.top

[U26] Py：并发下载
来源：http://pnr.0kj1m.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rsg.ydjk.org.cn

[U27] Py：异步 HTTP
来源：http://hps.nanxinkj.top

aiohttp.ClientSession() 配合 async with
来源：http://yqb.gogol.net.cn

[U28] Py：类型别名
来源：http://qje.quarkkingdee.top

UserId = int
来源：http://xfe.yanxiufei.cn

[U29] Py：属性校验
来源：http://abz.sufxvd.cn

@property 与 @x.setter 配合
来源：http://jne.tianlin.xyz

[U30] Py：数据类
来源：http://mbp.hcnkem.com

@dataclass(slots=True)
来源：http://sue.zdqjudy.top

[U31] Py：单测
来源：http://kav.gogol.net.cn

python -m pytest -q
来源：http://yqa.gotoacloud.top

[U32] Py：代码格式化
来源：http://fsp.cdnleiting.top

ruff format . && ruff check --fix .
来源：http://tgv.yj202588.top

[U33] Py：打包发布
来源：http://ylj.tanke756.top

python -m build  （依赖 pyproject.toml）
来源：http://uto.xuanzx.com

[U34] Py：判断编码
来源：http://xsr.hnqzz.top

chardet.detect(raw)
来源：http://lkq.redwolf501.top

[U35] Py：发送邮件
来源：http://kkj.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ilc.yanxiufei.cn

[U36] Py：定时任务
来源：http://xgv.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://ncx.zhixingplan.top

[U37] Py：读写 Excel
来源：http://cvd.chenzaomai.com

pandas.read_excel / DataFrame.to_excel
来源：http://rpu.vehdjk.com

[U38] Py：获取脚本所在目录
来源：http://flx.xylfe.cn

Path(__file__).resolve().parent
来源：http://pbi.fehbvm.com

[U39] Py：判断是否在交互环境
来源：http://dgg.tian-w.cn

sys.stdout.isatty()
来源：http://gxn.shangyingyoupin.top

[U40] Py：打印到标准错误
来源：http://zyb.xuanzx.com

print("err", file=sys.stderr)
来源：http://pqn.gogol.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://xjw.vqdsnc.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bnd.zhongyouzk.top

[U42] PHP：PSR-4 自动加载
来源：http://kns.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://egq.tarul.cn

[U43] PHP：声明命名空间
来源：http://kfr.uphjek.com

namespace App\Http;
来源：http://vgh.guannengcc.top

[U44] PHP：开启严格类型
来源：http://kwb.jiagoushi.top

declare(strict_types=1);
来源：http://dmg.hammf.cn

[U45] PHP：类型声明与返回类型
来源：http://ros.fktsv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jmi.mhx1999.top

[U46] PHP：可空类型
来源：http://cfl.uphjek.com

?string $name = null
来源：http://fwx.kuanghao11.cn

[U47] PHP：联合类型
来源：http://dhp.ivvv.top

int|string $id
来源：http://rzl.sweek.top

[U48] PHP：纯枚举
来源：http://vya.ydzc1.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://icq.chenjidiqi.icu

[U49] PHP：只读属性
来源：http://swx.iojbl.cn

public readonly string $name
来源：http://enf.gogol.net.cn

[U50] PHP：构造器属性提升
来源：http://aps.hesvh.cn

public function __construct(private int $id) {}
来源：http://ooj.yj20258.top

[U51] PHP：数组解构
来源：http://rek.xylfe.cn

[$a, $b] = $arr;
来源：http://use.zhengqikj.top

[U52] PHP：箭头函数
来源：http://gni.gotoacloud.top

$double = fn($x) => $x * 2;
来源：http://txi.xziqi.cn

[U53] PHP：空合并运算符
来源：http://kpf.0kj1m.cn

$v = $a ?? $b ?? "default";
来源：http://rye.zhixingplan.top

[U54] PHP：空安全调用
来源：http://dyf.yueranfly.top

$obj?->method()
来源：http://uuz.pengpengdd.cyou

[U55] PHP：match 表达式
来源：http://wjr.fanxiaobao.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jjz.xylfe.cn

[U56] PHP：命名参数
来源：http://otb.bbcook.cn

f(a: 1, b: 2)
来源：http://ssg.jqgfzy.top

[U57] PHP：字符串插值
来源：http://owk.ppjwa.cn

"值: {$a}"
来源：http://utx.ctjpmb.com

[U58] PHP：数组三件套
来源：http://ybp.cheryme.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xce.xylfe.cn

[U59] PHP：自定义排序
来源：http://cfd.dashuyun.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hge.sufxvd.cn

[U60] PHP：JSON 编解码
来源：http://pzf.vqdsnc.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://byn.pycfn.com

[U61] PHP：正则
来源：http://ely.hammf.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xnc.birdmap.top

[U62] PHP：日期对象
来源：http://ihb.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aic.hnqzz.top

[U63] PHP：文件读写
来源：http://tmn.cucudq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rnl.jianghu66.top

[U64] PHP：目录遍历
来源：http://oyn.shangyingyoupin.top

glob("dir/*.php");  scandir("dir");
来源：http://tno.aizwys.cn

[U65] PHP：会话
来源：http://qyz.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ach.yanxiufei.cn

[U66] PHP：设置 Cookie
来源：http://zec.mhx1999.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kmb.ctjpmb.com

[U67] PHP：处理文件上传
来源：http://ord.epnwcf.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cbj.xylfe.cn

[U68] PHP：PDO 连接
来源：http://qbw.shangyingyoupin.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uws.yueranfly.top

[U69] PHP：PDO 预处理
来源：http://hrl.snrcjt.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gka.cashguo.top

[U70] PHP：PDO 事务
来源：http://ttj.yangfankeji.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wnk.yangfankeji.com

[U71] PHP：抛出异常
来源：http://ghe.yanxiufei.cn

throw new RuntimeException("失败", 500);
来源：http://bdg.meibo888.top

[U72] PHP：写错误日志
来源：http://lto.zdqjudy.top

error_log("失败: " . $e->getMessage());
来源：http://tpu.hongshengwenyu.top

[U73] PHP：读取 ini 配置
来源：http://zvz.snrcjt.cn

parse_ini_file("config.ini", true)
来源：http://qju.c1oappe.top

[U74] PHP：读取环境变量
来源：http://fng.cdnleiting.top

getenv("APP_ENV") ?: "production"
来源：http://pmc.fzhhl.top

[U75] PHP：依赖注入
来源：http://brr.bbcook.cn

composer require psr/container
来源：http://jmc.yj20258.top

[U76] PHP：简单路由
来源：http://jpr.ehwqpu.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://avc.yj20258888.top

[U77] PHP：模板渲染
来源：http://fxe.yfazqb.com

composer require twig/twig
来源：http://cdk.zhengqikj.top

[U78] PHP：单元测试
来源：http://azr.sxryk.cn

composer require --dev phpunit/phpunit
来源：http://jiw.jqgufenzy.top

[U79] PHP：静态分析
来源：http://sdd.kuanghao11.cn

composer require --dev phpstan/phpstan
来源：http://wlg.jqgfzy.top

[U80] PHP：代码规范修复
来源：http://jqv.zhoulong.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://hbo.jqgufenzy.top

[U81] JS：初始化项目
来源：http://hgi.uphjek.com

npm init -y;  npm i express
来源：http://cxl.xziqi.cn

[U82] JS：package.json 脚本
来源：http://ahw.yj202588.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hps.tanke756.top

[U83] JS：ES Module 导入导出
来源：http://cmd.yangfankeji.com

export const a = 1;  import { a } from "./m.js";
来源：http://fgb.hfpthk.cn

[U84] JS：CommonJS 写法
来源：http://svy.jyoumei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oqm.daria6918.cn

[U85] JS：可选链
来源：http://jpw.yfazqb.com

a?.b?.c
来源：http://msn.yanxiufei.cn

[U86] JS：空值合并
来源：http://xmt.guannengcc.top

a ?? b
来源：http://vag.yueranfly.top

[U87] JS：解构默认值
来源：http://qzw.sjlbkw.cn

const { a = 1, b = 2 } = obj;
来源：http://utv.fzhhl.top

[U88] JS：对象展开合并
来源：http://shi.nanxuanxn.top

{ ...a, ...b }
来源：http://tzb.yj20258.top

[U89] JS：数组去重
来源：http://rus.feifeiyinyue.top

[...new Set(arr)]
来源：http://aem.jyoumei.cn

[U90] JS：数字数组排序
来源：http://pov.hfpthk.cn

[...arr].sort((a, b) => a - b)
来源：http://nrt.shangyingyoupin.top

[U91] JS：对象键值遍历
来源：http://umt.yuanzhike.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oig.gotoacloud.top

[U92] JS：深拷贝
来源：http://csr.sufxvd.cn

structuredClone(obj)
来源：http://vzd.daxiang520.top

[U93] JS：模板字符串
来源：http://pqp.ydjk.org.cn

`共 ${n} 条`
来源：http://ywj.wangshuangyany.cn

[U94] JS：箭头函数
来源：http://giu.cdnleiting.top

const double = x => x * 2;
来源：http://pkn.zycfv.cn

[U95] JS：Promise 包装
来源：http://aro.sufxvd.cn

new Promise((resolve, reject) => {})
来源：http://ics.yanxiufei.cn

[U96] JS：async/await 与异常
来源：http://ems.chenjidiqi.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qri.ehwqpu.com

[U97] JS：并发请求
来源：http://hzm.svipenyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hhi.yanxiufei.cn

[U98] JS：fetch 带 JSON
来源：http://qvn.dashuyun.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pkh.jqgfzy.top

[U99] JS：事件监听
来源：http://pyj.cheryme.top

el.addEventListener("click", e => {})
来源：http://ntv.yj20258888.top

[U100] JS：DOM 查询
来源：http://dpd.sweek.top

document.querySelector(".item")
来源：http://wtk.guowangkeji.top

[U101] JS：classList 操作
来源：http://ats.xinyue.icu

el.classList.toggle("active")
来源：http://ggx.ywan-chungtsiang.top

[U102] JS：本地存储
来源：http://gxa.shanyushiyangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mro.fzhhl.top

[U103] JS：定时器
来源：http://wyf.ctjpmb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lla.fanxiaobao.xyz

[U104] JS：防抖
来源：http://hsu.pengpengdd.cyou

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xqj.nanxuanxn.top

[U105] JS：节流
来源：http://zib.bbcook.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vsw.9152youxi.cn

[U106] JS：日期格式化
来源：http://dgp.yonumen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://viw.shzxlz.cn

[U107] JS：数字千分位
来源：http://nog.tianlin.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iop.zdbjq.cn

[U108] JS：随机整数
来源：http://ngi.zycfv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hye.fehbvm.com

[U109] JS：数组分组
来源：http://oef.zdbjq.cn

Object.groupBy(arr, x => x.type)
来源：http://guj.dashuyun.cn

[U110] JS：数组分块
来源：http://lvk.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://utr.bjfxy.top

[U111] JS：对象转 Map
来源：http://gun.hywenlv.cn

new Map(Object.entries(obj))
来源：http://ngb.vehdjk.com

[U112] JS：字符串补位
来源：http://uxg.sufxvd.cn

"7".padStart(3, "0")
来源：http://yer.chenzaomai.com

[U113] JS：正则替换全部
来源：http://qkf.pycfn.com

s.replaceAll("a", "b")
来源：http://xsf.gotoacloud.top

[U114] JS：JSON 深比较
来源：http://aqj.uphjek.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://tgy.dashuyun.cn

[U115] JS：生成 UUID
来源：http://ndj.316326.xyz

crypto.randomUUID()
来源：http://yst.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://iug.shangyingyoupin.top

/** @param {string} name */ function f(name) {}
来源：http://nka.tarul.cn

[U117] JS：单元测试
来源：http://bvj.jiagoushi.top

npm i -D vitest;  npx vitest
来源：http://ymi.yuanzhike.top

[U118] JS：开发服务器
来源：http://oen.daria6918.cn

npm i -D vite;  npx vite
来源：http://piu.zdqjudy.top

[U119] JS：生产构建
来源：http://zmb.yj20258.top

npx vite build
来源：http://tje.birdmap.top

[U120] JS：读取环境变量（Vite）
来源：http://iju.pycfn.com

import.meta.env.VITE_API_URL
来源：http://oci.zycfv.cn

================================================================================
来源：http://fdq.zhaomingkeji.xyz

统计汇总
来源：http://pky.wangshuangyany.cn

================================================================================
来源：http://omn.aizwys.cn

按语言统计（条）：
来源：http://byi.jyoumei.cn

Python ......... 252
来源：http://gbh.ctjpmb.com

PHP ............ 252
来源：http://ejx.yvedp.cn

JavaScript ..... 252
来源：http://ggx.9152youxi.cn

TypeScript ..... 212
来源：http://nxf.bbcook.cn

Java ........... 212
来源：http://psr.yuxming.cn

Go ............. 212
来源：http://ndu.bjfxy.top

Ruby ........... 212
来源：http://gij.chenlongwang.top

C# ............. 212
来源：http://pbn.ehwqpu.com

C .............. 30
来源：http://gxi.yuxming.cn

C++ ............ 30
来源：http://tls.pengpengdd.cyou

SQL ............ 90
来源：http://wah.meibo888.top

Bash ........... 80
来源：http://ngq.ydzc1.top

Kotlin ......... 15
来源：http://yzt.52xcode.cn

Swift .......... 15
来源：http://wcs.yj202588.top

Lua ............ 10
来源：http://xqf.cqqwz.cn

Perl ........... 10
来源：http://nbe.pengpengdd.cyou

Scala .......... 10
来源：http://ppa.tianlin.xyz

------------------------------------
来源：http://wib.yuanzhike.top

合计 ........... 2106 条
来源：http://aci.pycfn.com

按章节统计：
来源：http://hgd.meibo888.top


<!-- 参考信息 -->