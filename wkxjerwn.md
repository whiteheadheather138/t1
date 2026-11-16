代发 wailian999

[T35] Lua：字典表
来源：http://xka.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://nyl.tarul.cn

[T36] Lua：函数
来源：http://aqe.jqgfzy.top

function add(a, b) return a + b end
来源：http://eat.wangdashe.top

[T37] Lua：字符串拼接
来源：http://vpe.jqgfzy.top

"a" .. "b"
来源：http://hfz.fengsongda.top

[T38] Lua：条件
来源：http://jkt.uphjek.com

if x > 0 then print("正") end
来源：http://dox.fehbvm.com

[T39] Lua：模式匹配
来源：http://mik.yuanzhike.top

string.find(s, "%d+")
来源：http://xbq.mhx1999.top

[T40] Lua：元表
来源：http://skl.xuanzx.com

setmetatable({}, { __index = base })
来源：http://pkz.meibo888.top

[T41] Perl：Hello World
来源：http://ysb.epnwcf.com

print "Hello\n";
来源：http://uuj.ivvv.top

[T42] Perl：变量类型
来源：http://ixf.jiagoushi.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uka.yueranfly.top

[T43] Perl：字符串插值
来源：http://gzx.daria6918.cn

"值: $a"
来源：http://dwl.chenzaomai.com

[T44] Perl：条件
来源：http://kge.shangyingyoupin.top

if ($a > 0) { print "正"; }
来源：http://ukg.shanyushiyangkeji.top

[T45] Perl：数组遍历
来源：http://xck.xylfe.cn

for my $x (@arr) { print $x; }
来源：http://wyn.birdmap.top

[T46] Perl：哈希操作
来源：http://mxb.jqgfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kdu.iojbl.cn

[T47] Perl：正则捕获
来源：http://sao.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nbl.yuanzhike.top

[T48] Perl：正则替换
来源：http://iic.zdqjudy.top

$s =~ s/old/new/g;
来源：http://okq.hesvh.cn

[T49] Perl：函数
来源：http://mrp.yj20258888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ght.guowangkeji.top

[T50] Perl：逐行读文件
来源：http://dtj.ehwqpu.com

open my $fh, "<", "a.txt" or die $!;
来源：http://spj.yuanzhike.top

while (my $line = <$fh>) { print $line; }
来源：http://yof.zdqjudy.top

[T51] Scala：Hello World
来源：http://xlk.fzhhl.top

println("Hello")
来源：http://bii.uphjek.com

[T52] Scala：变量
来源：http://ewk.uphjek.com

val a = 1;  var b = 2
来源：http://wgd.redwolf501.top

[T53] Scala：字符串插值
来源：http://paf.xuanzx.com

s"值: $b"
来源：http://aek.nwbrower.top

[T54] Scala：集合映射
来源：http://mug.hywenlv.cn

List(1, 2, 3).map(_ * 2)
来源：http://jcm.bbcook.cn

[T55] Scala：集合过滤
来源：http://ykm.snrcjt.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zua.yonumen.top

[T56] Scala：样例类
来源：http://ulb.jyoumei.cn

case class User(name: String, age: Int)
来源：http://apo.zhiwuduotai.top

[T57] Scala：模式匹配
来源：http://xjb.yanxiufei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wjo.ivvv.top

[T58] Scala：函数定义
来源：http://sne.nanxinkj.top

def add(a: Int, b: Int): Int = a + b
来源：http://eee.shzxlz.cn

[T59] Scala：循环
来源：http://ogv.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://qzc.guowangkeji.top

[T60] Scala：折叠
来源：http://vcw.yanxiufei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pnp.shangyingyoupin.top

================================================================================
来源：http://wrb.jqgfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hxx.cashguo.top

================================================================================
来源：http://cjb.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://jvp.mhx1999.top

python -m venv .venv && source .venv/bin/activate
来源：http://xvr.jiagoushi.top

[U02] Py：导出 / 安装依赖
来源：http://vfi.zhengqikj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gzk.zhiwuduotai.top

[U03] Py：加载 .env 配置
来源：http://tuw.tanke756.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cjq.xylfe.cn

[U04] Py：变量调试打印
来源：http://mto.meibo888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jeq.nanxuanxn.top

[U05] Py：列表去重且保序
来源：http://nbs.havefunace.top

list(dict.fromkeys(arr))
来源：http://fqo.fehbvm.com

[U06] Py：合并两个字典
来源：http://mzs.hongshengwenyu.top

{**a, **b}
来源：http://dul.fehbvm.com

[U07] Py：反转字典键值
来源：http://ddy.ydjk.org.cn

{v: k for k, v in d.items()}
来源：http://qhg.birdmap.top

[U08] Py：展平二维列表
来源：http://blj.chenjidiqi.icu

[y for x in nested for y in x]
来源：http://exo.hammf.cn

[U09] Py：字典取最大值的键
来源：http://oeg.jyoumei.cn

max(d, key=d.get)
来源：http://bst.tianlin.xyz

[U10] Py：按值排序字典
来源：http://uxu.jinqigfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wes.aizwys.cn

[U11] Py：生成器表达式
来源：http://qrb.zhongyouzk.top

(x * 2 for x in arr)
来源：http://swi.zhixingplan.top

[U12] Py：取出现最多的 3 个元素
来源：http://baf.jinyuanbaomall.cn

Counter(arr).most_common(3)
来源：http://jjv.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://iuz.daxiang520.top

deque(maxlen=10)
来源：http://rue.jinghuilouyu.cn

[U14] Py：分组收集到列表
来源：http://mjg.xingfuxueyuan.xyz

defaultdict(list)
来源：http://hkd.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://ski.meibo888.top

t = time.perf_counter()
来源：http://qkg.xingfuxueyuan.xyz

[U16] Py：命令行参数解析
来源：http://jgz.52xcode.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xce.ivvv.top

[U17] Py：初始化日志
来源：http://fus.chenlongwang.top

logging.basicConfig(level=logging.INFO)
来源：http://yoi.chenzaomai.com

[U18] Py：预编译正则
来源：http://fjn.nanxinkj.top

pat = re.compile(r"\d+")
来源：http://akp.haohaochexian.top

[U19] Py：正则替换带回调
来源：http://pmj.hywenlv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xzv.xylfe.cn

[U20] Py：缓存函数结果
来源：http://nnl.vqdsnc.cn

@functools.lru_cache(maxsize=None)
来源：http://lqz.feifeiyinyue.top

[U21] Py：自定义上下文管理器
来源：http://goe.hnxiangtu.top

@contextlib.contextmanager
来源：http://wxz.jinqigfzy.top

[U22] Py：矩阵转置
来源：http://tpl.snrcjt.cn

list(zip(*m))
来源：http://fel.vehdjk.com

[U23] Py：分块读取大文件
来源：http://zoy.zhixingplan.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pcr.tanke756.top

[U24] Py：路径操作
来源：http://ofj.fanxiaobao.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://npi.guannengcc.top

[U25] Py：CSV 按字典读
来源：http://xkt.shangyingyoupin.top

csv.DictReader(f)
来源：http://wyq.yvedp.cn

[U26] Py：并发下载
来源：http://xjm.yangfankeji.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wiv.cucudq.cn

[U27] Py：异步 HTTP
来源：http://wur.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://avs.haohaochexian.top

[U28] Py：类型别名
来源：http://zgn.aizwys.cn

UserId = int
来源：http://pri.yj20258.top

[U29] Py：属性校验
来源：http://whf.zycfv.cn

@property 与 @x.setter 配合
来源：http://mxg.cqqwz.cn

[U30] Py：数据类
来源：http://zhi.xinyue.icu

@dataclass(slots=True)
来源：http://hnd.jqgufenzy.top

[U31] Py：单测
来源：http://cqj.hnxiangtu.top

python -m pytest -q
来源：http://jfg.vehdjk.com

[U32] Py：代码格式化
来源：http://sha.yvedp.cn

ruff format . && ruff check --fix .
来源：http://ixs.jqgfzy.top

[U33] Py：打包发布
来源：http://mqx.hnqzz.top

python -m build  （依赖 pyproject.toml）
来源：http://doe.bjfxy.top

[U34] Py：判断编码
来源：http://pof.gotoacloud.top

chardet.detect(raw)
来源：http://oeb.yvedp.cn

[U35] Py：发送邮件
来源：http://ioi.ydjk.org.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fne.jiagoushi.top

[U36] Py：定时任务
来源：http://gxh.hfpthk.cn

schedule.every(10).minutes.do(job)
来源：http://qoy.feifeiyinyue.top

[U37] Py：读写 Excel
来源：http://wpt.sufxvd.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bae.gogol.net.cn

[U38] Py：获取脚本所在目录
来源：http://lsz.iojbl.cn

Path(__file__).resolve().parent
来源：http://yim.316326.xyz

[U39] Py：判断是否在交互环境
来源：http://hxj.zhengqikj.top

sys.stdout.isatty()
来源：http://hot.dianchejie.cn

[U40] Py：打印到标准错误
来源：http://vfs.jyoumei.cn

print("err", file=sys.stderr)
来源：http://dmc.andypj.xyz

[U41] PHP：初始化 Composer 项目
来源：http://xsv.xingfuxueyuan.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://dnd.aibaodan.cn

[U42] PHP：PSR-4 自动加载
来源：http://qut.nanxuanxn.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lwq.dashuyun.cn

[U43] PHP：声明命名空间
来源：http://gmw.cheryme.top

namespace App\Http;
来源：http://wsk.meibo888.top

[U44] PHP：开启严格类型
来源：http://tbw.yonumen.top

declare(strict_types=1);
来源：http://uwp.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://ojh.yj20258.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ckn.daria6918.cn

[U46] PHP：可空类型
来源：http://tae.iojbl.cn

?string $name = null
来源：http://hpr.svipenyu.cn

[U47] PHP：联合类型
来源：http://pxv.jqgfzy.top

int|string $id
来源：http://lqi.hammf.cn

[U48] PHP：纯枚举
来源：http://gwc.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eps.0kj1m.cn

[U49] PHP：只读属性
来源：http://hoo.daxiang520.top

public readonly string $name
来源：http://imy.yongpay.top

[U50] PHP：构造器属性提升
来源：http://gud.0kj1m.cn

public function __construct(private int $id) {}
来源：http://kse.zhiwuduotai.top

[U51] PHP：数组解构
来源：http://nlg.zhongyouzk.top

[$a, $b] = $arr;
来源：http://oat.xziqi.cn

[U52] PHP：箭头函数
来源：http://gxw.gaohongyu789.top

$double = fn($x) => $x * 2;
来源：http://tww.fehbvm.com

[U53] PHP：空合并运算符
来源：http://udi.gotoacloud.top

$v = $a ?? $b ?? "default";
来源：http://pdj.fktsv.cn

[U54] PHP：空安全调用
来源：http://dhk.sysykeji.top

$obj?->method()
来源：http://qrp.zdqjudy.top

[U55] PHP：match 表达式
来源：http://fez.daria6918.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xeg.zhaomingkeji.xyz

[U56] PHP：命名参数
来源：http://kub.epnwcf.com

f(a: 1, b: 2)
来源：http://ngj.zdqjudy.top

[U57] PHP：字符串插值
来源：http://ign.hesvh.cn

"值: {$a}"
来源：http://nbj.tianlin.xyz

[U58] PHP：数组三件套
来源：http://dnx.ctjpmb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zjv.bbcook.cn

[U59] PHP：自定义排序
来源：http://lky.hysaishi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ybq.yanxiufei.cn

[U60] PHP：JSON 编解码
来源：http://gct.mhx1999.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://glw.fzhhl.top

[U61] PHP：正则
来源：http://qfh.havefunace.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ylv.cheryme.top

[U62] PHP：日期对象
来源：http://ipf.vqdsnc.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://snd.yanxiufei.cn

[U63] PHP：文件读写
来源：http://jjw.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ehf.fzhhl.top

[U64] PHP：目录遍历
来源：http://mme.hnqzz.top

glob("dir/*.php");  scandir("dir");
来源：http://chn.jlsjyb.cn

[U65] PHP：会话
来源：http://vtu.shanyushiyangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://uau.meibo888.top

[U66] PHP：设置 Cookie
来源：http://phv.sufxvd.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hmt.daxiang520.top

[U67] PHP：处理文件上传
来源：http://gtp.sxryk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ano.zhiwuduotai.top

[U68] PHP：PDO 连接
来源：http://zgi.yongpay.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bhn.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://jdd.nwbrower.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lht.yongpay.top

[U70] PHP：PDO 事务
来源：http://bmj.iojbl.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bfa.iojbl.cn

[U71] PHP：抛出异常
来源：http://jyk.yj202588.top

throw new RuntimeException("失败", 500);
来源：http://wxe.zhoulong.xyz

[U72] PHP：写错误日志
来源：http://raj.tanke756.top

error_log("失败: " . $e->getMessage());
来源：http://zpp.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://jla.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://aly.nanxinkj.top

[U74] PHP：读取环境变量
来源：http://zfv.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://eyh.0kj1m.cn

[U75] PHP：依赖注入
来源：http://krd.yueranfly.top

composer require psr/container
来源：http://hhw.xuetiantiany.cn

[U76] PHP：简单路由
来源：http://min.jinqigufen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eyd.zdqjudy.top

[U77] PHP：模板渲染
来源：http://ydh.zhaomingkeji.xyz

composer require twig/twig
来源：http://hih.yangfankeji.com

[U78] PHP：单元测试
来源：http://ief.shzxlz.cn

composer require --dev phpunit/phpunit
来源：http://thp.zhoulong.xyz

[U79] PHP：静态分析
来源：http://ryh.quarkkingdee.top

composer require --dev phpstan/phpstan
来源：http://aom.zhongyouzk.top

[U80] PHP：代码规范修复
来源：http://rxo.uphjek.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://ezw.gzhubu.top

[U81] JS：初始化项目
来源：http://zar.yj202588.top

npm init -y;  npm i express
来源：http://mwc.zhaomingkeji.xyz

[U82] JS：package.json 脚本
来源：http://wrl.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://onb.jiagoushi.top

[U83] JS：ES Module 导入导出
来源：http://ooe.svipenyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jmp.daxiang520.top

[U84] JS：CommonJS 写法
来源：http://eiy.c1oappe.top

module.exports = { a };  const { a } = require("./m");
来源：http://tea.wangdashe.top

[U85] JS：可选链
来源：http://jno.birdmap.top

a?.b?.c
来源：http://mlh.xylfe.cn

[U86] JS：空值合并
来源：http://djc.cqqwz.cn

a ?? b
来源：http://pqd.sysykeji.top

[U87] JS：解构默认值
来源：http://qzg.aizwys.cn

const { a = 1, b = 2 } = obj;
来源：http://fpo.hysaishi.cn

[U88] JS：对象展开合并
来源：http://mqv.yongpay.top

{ ...a, ...b }
来源：http://mum.chenlongwang.top

[U89] JS：数组去重
来源：http://uav.9152youxi.cn

[...new Set(arr)]
来源：http://ege.dashuyun.cn

[U90] JS：数字数组排序
来源：http://ofg.yj20258.top

[...arr].sort((a, b) => a - b)
来源：http://cyd.hfpthk.cn

[U91] JS：对象键值遍历
来源：http://snh.guannengcc.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zua.hywenlv.cn

[U92] JS：深拷贝
来源：http://paf.haohaochexian.top

structuredClone(obj)
来源：http://jgo.52xcode.cn

[U93] JS：模板字符串
来源：http://vzu.ppjwa.cn

`共 ${n} 条`
来源：http://zvh.sufxvd.cn

[U94] JS：箭头函数
来源：http://oba.vqdsnc.cn

const double = x => x * 2;
来源：http://mtf.jianghu66.top

[U95] JS：Promise 包装
来源：http://yoa.jinyuanbaomall.cn

new Promise((resolve, reject) => {})
来源：http://wvs.pycfn.com

[U96] JS：async/await 与异常
来源：http://fie.dianchejie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ztq.yj20258.top

[U97] JS：并发请求
来源：http://ymz.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cup.guannengcc.top

[U98] JS：fetch 带 JSON
来源：http://hle.birdmap.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pko.yfazqb.com

[U99] JS：事件监听
来源：http://ild.andypj.xyz

el.addEventListener("click", e => {})
来源：http://tft.birdmap.top

[U100] JS：DOM 查询
来源：http://ceq.xylfe.cn

document.querySelector(".item")
来源：http://zqj.ehwqpu.com

[U101] JS：classList 操作
来源：http://bfu.jlsjyb.cn

el.classList.toggle("active")
来源：http://mjx.zdqjudy.top

[U102] JS：本地存储
来源：http://vwr.sweek.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zih.sufxvd.cn

[U103] JS：定时器
来源：http://toi.hfpthk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yjt.fehbvm.com

[U104] JS：防抖
来源：http://hhu.svipenyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lkf.svipenyu.cn

[U105] JS：节流
来源：http://veo.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ekd.ivvv.top

[U106] JS：日期格式化
来源：http://fgp.sysykeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wqt.guowangkeji.top

[U107] JS：数字千分位
来源：http://ljg.pycfn.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nlj.daxiang520.top

[U108] JS：随机整数
来源：http://nth.shzxlz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zzr.uphjek.com

[U109] JS：数组分组
来源：http://qrq.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://uwn.pengpengdd.cyou

[U110] JS：数组分块
来源：http://ksp.xinyue.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xwa.haohaochexian.top

[U111] JS：对象转 Map
来源：http://nfo.nwbrower.top

new Map(Object.entries(obj))
来源：http://khs.sweek.top

[U112] JS：字符串补位
来源：http://kiv.hesvh.cn

"7".padStart(3, "0")
来源：http://qvm.hywenlv.cn

[U113] JS：正则替换全部
来源：http://aex.hcnkem.com

s.replaceAll("a", "b")
来源：http://cko.chenjidiqi.icu

[U114] JS：JSON 深比较
来源：http://snh.c1oappe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jvo.yj20258.top

[U115] JS：生成 UUID
来源：http://czr.jinqigfzy.top

crypto.randomUUID()
来源：http://qmm.ehwqpu.com

[U116] JS：类型检查（JSDoc）
来源：http://mgp.xinyue.icu

/** @param {string} name */ function f(name) {}
来源：http://fmh.c1oappe.top

[U117] JS：单元测试
来源：http://ufv.zhoulong.xyz

npm i -D vitest;  npx vitest
来源：http://qnv.yvedp.cn

[U118] JS：开发服务器
来源：http://qpl.zhaomingkeji.xyz

npm i -D vite;  npx vite
来源：http://kug.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://prk.tianlin.xyz

npx vite build
来源：http://zep.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://rwr.wangshuangyany.cn

import.meta.env.VITE_API_URL
来源：http://wgt.nwbrower.top

================================================================================
来源：http://bcs.wangshuangyany.cn

统计汇总
来源：http://adt.sweek.top

================================================================================
来源：http://hgs.zhaomingkeji.xyz

按语言统计（条）：
来源：http://pgx.cashguo.top


<!-- 参考信息 -->