代发 wailian999

[T29] Swift：guard 提前返回
来源：http://tzx.zhaomingkeji.xyz

guard let x = opt else { return }
来源：http://kek.yfazqb.com

[T30] Swift：协议
来源：http://cuq.zhoulong.xyz

protocol Shape { func area() -> Double }
来源：http://pne.shuidangran.top

[T31] Lua：Hello World
来源：http://cqn.yangfankeji.com

print("Hello")
来源：http://obb.bbcook.cn

[T32] Lua：局部变量
来源：http://jiy.xuetiantiany.cn

local a = 1
来源：http://zfa.jlsjyb.cn

[T33] Lua：表（数组）
来源：http://tef.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gzi.feifeiyinyue.top

[T34] Lua：遍历表
来源：http://xdy.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://tys.shanyushiyangkeji.top

[T35] Lua：字典表
来源：http://vlg.redwolf501.top

local d = { a = 1 };  d.b = 2
来源：http://rsk.ybcxt.top

[T36] Lua：函数
来源：http://bfr.chenjidiqi.icu

function add(a, b) return a + b end
来源：http://qbi.316326.xyz

[T37] Lua：字符串拼接
来源：http://xlj.feifeiyinyue.top

"a" .. "b"
来源：http://cyq.iojbl.cn

[T38] Lua：条件
来源：http://eqy.cqqwz.cn

if x > 0 then print("正") end
来源：http://rec.xuetiantiany.cn

[T39] Lua：模式匹配
来源：http://pos.xinyue.icu

string.find(s, "%d+")
来源：http://orn.jianghu66.top

[T40] Lua：元表
来源：http://dhu.zhiwuduotai.top

setmetatable({}, { __index = base })
来源：http://fby.jianghu66.top

[T41] Perl：Hello World
来源：http://rtl.aibaodan.cn

print "Hello\n";
来源：http://nrd.cdnleiting.top

[T42] Perl：变量类型
来源：http://bip.redwolf501.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gqn.smart0.xyz

[T43] Perl：字符串插值
来源：http://ssn.aibaodan.cn

"值: $a"
来源：http://lds.aizwys.cn

[T44] Perl：条件
来源：http://fyf.fengsongda.top

if ($a > 0) { print "正"; }
来源：http://gma.redwolf501.top

[T45] Perl：数组遍历
来源：http://xto.ivvv.top

for my $x (@arr) { print $x; }
来源：http://bnx.havefunace.top

[T46] Perl：哈希操作
来源：http://gib.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ikw.xylfe.cn

[T47] Perl：正则捕获
来源：http://zxs.mhx1999.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://cba.aizwys.cn

[T48] Perl：正则替换
来源：http://wko.dashuyun.cn

$s =~ s/old/new/g;
来源：http://ngr.ppjwa.cn

[T49] Perl：函数
来源：http://oub.yj202588.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lpk.jianghu66.top

[T50] Perl：逐行读文件
来源：http://fpy.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bao.zdbjq.cn

while (my $line = <$fh>) { print $line; }
来源：http://bta.birdmap.top

[T51] Scala：Hello World
来源：http://pkb.daxiang520.top

println("Hello")
来源：http://xvb.smart0.xyz

[T52] Scala：变量
来源：http://fxf.mhx1999.top

val a = 1;  var b = 2
来源：http://nsh.havefunace.top

[T53] Scala：字符串插值
来源：http://ybo.sufxvd.cn

s"值: $b"
来源：http://wbj.yongpay.top

[T54] Scala：集合映射
来源：http://wem.mhx1999.top

List(1, 2, 3).map(_ * 2)
来源：http://aqe.ydzc1.top

[T55] Scala：集合过滤
来源：http://vbi.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jai.yfazqb.com

[T56] Scala：样例类
来源：http://hbp.yuxming.cn

case class User(name: String, age: Int)
来源：http://ufz.chenjidiqi.icu

[T57] Scala：模式匹配
来源：http://rbw.meibo888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hsd.zhiwuduotai.top

[T58] Scala：函数定义
来源：http://lpt.havefunace.top

def add(a: Int, b: Int): Int = a + b
来源：http://bgn.shuidangran.top

[T59] Scala：循环
来源：http://xqk.yuxming.cn

for (i <- 1 to 10) println(i)
来源：http://jry.shzxlz.cn

[T60] Scala：折叠
来源：http://fwa.gaohongyu789.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ydh.haohaochexian.top

================================================================================
来源：http://vcf.cheryme.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fgp.yongpay.top

================================================================================
来源：http://wyc.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://nca.dianchejie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jlk.fengsongda.top

[U02] Py：导出 / 安装依赖
来源：http://iaw.cdnleiting.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://egw.ywan-chungtsiang.top

[U03] Py：加载 .env 配置
来源：http://jrl.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dae.nanxinkj.top

[U04] Py：变量调试打印
来源：http://agi.ydjk.org.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qcz.hywenlv.cn

[U05] Py：列表去重且保序
来源：http://eht.wangdashe.top

list(dict.fromkeys(arr))
来源：http://xuc.hongshengwenyu.top

[U06] Py：合并两个字典
来源：http://iww.shanyushiyangtech.top

{**a, **b}
来源：http://rhk.316326.xyz

[U07] Py：反转字典键值
来源：http://elb.epnwcf.com

{v: k for k, v in d.items()}
来源：http://hcx.hnqzz.top

[U08] Py：展平二维列表
来源：http://rur.hywenlv.cn

[y for x in nested for y in x]
来源：http://htj.gogol.net.cn

[U09] Py：字典取最大值的键
来源：http://xzi.aibaodan.cn

max(d, key=d.get)
来源：http://jal.c1oappe.top

[U10] Py：按值排序字典
来源：http://qxp.xuetiantiany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ehm.bjfxy.top

[U11] Py：生成器表达式
来源：http://uhu.smart0.xyz

(x * 2 for x in arr)
来源：http://gxm.xuanzx.com

[U12] Py：取出现最多的 3 个元素
来源：http://wud.gzhubu.top

Counter(arr).most_common(3)
来源：http://cqg.sweek.top

[U13] Py：固定长度队列
来源：http://xyr.316326.xyz

deque(maxlen=10)
来源：http://mbn.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://jyi.xylfe.cn

defaultdict(list)
来源：http://jyc.hnqzz.top

[U15] Py：高精度计时
来源：http://zaf.jinghuilouyu.cn

t = time.perf_counter()
来源：http://lza.tian-w.cn

[U16] Py：命令行参数解析
来源：http://yzv.havefunace.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yom.zhixingplan.top

[U17] Py：初始化日志
来源：http://qzr.shzxlz.cn

logging.basicConfig(level=logging.INFO)
来源：http://awd.redwolf501.top

[U18] Py：预编译正则
来源：http://fvh.52xcode.cn

pat = re.compile(r"\d+")
来源：http://guc.yfazqb.com

[U19] Py：正则替换带回调
来源：http://zjz.yueranfly.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xce.hywenlv.cn

[U20] Py：缓存函数结果
来源：http://fly.yj20258888.top

@functools.lru_cache(maxsize=None)
来源：http://mtw.snrcjt.cn

[U21] Py：自定义上下文管理器
来源：http://awc.dianchejie.cn

@contextlib.contextmanager
来源：http://ahk.shanyushiyangkeji.top

[U22] Py：矩阵转置
来源：http://ung.hnqzz.top

list(zip(*m))
来源：http://dii.pycfn.com

[U23] Py：分块读取大文件
来源：http://opv.ydzc1.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cpm.cdnleiting.top

[U24] Py：路径操作
来源：http://uqc.wangshuangyany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dcl.xinyue.icu

[U25] Py：CSV 按字典读
来源：http://dci.hfpthk.cn

csv.DictReader(f)
来源：http://viy.c1oappe.top

[U26] Py：并发下载
来源：http://hfm.zhixingplan.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nzq.fzhhl.top

[U27] Py：异步 HTTP
来源：http://qcn.andypj.xyz

aiohttp.ClientSession() 配合 async with
来源：http://jke.bbcook.cn

[U28] Py：类型别名
来源：http://oko.cucudq.cn

UserId = int
来源：http://swk.yuxming.cn

[U29] Py：属性校验
来源：http://ram.cashguo.top

@property 与 @x.setter 配合
来源：http://eto.zhijiandao.cn

[U30] Py：数据类
来源：http://exp.yuanzhike.top

@dataclass(slots=True)
来源：http://apx.yj202588.top

[U31] Py：单测
来源：http://mnx.jinqigufen.top

python -m pytest -q
来源：http://ewq.sjlbkw.cn

[U32] Py：代码格式化
来源：http://rma.sysykeji.top

ruff format . && ruff check --fix .
来源：http://ylu.zhoulong.xyz

[U33] Py：打包发布
来源：http://boz.xingfuxueyuan.xyz

python -m build  （依赖 pyproject.toml）
来源：http://zqy.zdbjq.cn

[U34] Py：判断编码
来源：http://uzd.kuanghao11.cn

chardet.detect(raw)
来源：http://wnl.uphjek.com

[U35] Py：发送邮件
来源：http://zru.chenjidiqi.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gva.hnqzz.top

[U36] Py：定时任务
来源：http://wch.mhx1999.top

schedule.every(10).minutes.do(job)
来源：http://kyp.jyoumei.cn

[U37] Py：读写 Excel
来源：http://kvy.jianghu66.top

pandas.read_excel / DataFrame.to_excel
来源：http://ijm.yvedp.cn

[U38] Py：获取脚本所在目录
来源：http://lyj.fktsv.cn

Path(__file__).resolve().parent
来源：http://kdn.quarkkingdee.top

[U39] Py：判断是否在交互环境
来源：http://rht.havefunace.top

sys.stdout.isatty()
来源：http://pty.jiagoushi.top

[U40] Py：打印到标准错误
来源：http://trj.ywan-chungtsiang.top

print("err", file=sys.stderr)
来源：http://bex.ivvv.top

[U41] PHP：初始化 Composer 项目
来源：http://koa.tianlin.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://xok.zhongyouzk.top

[U42] PHP：PSR-4 自动加载
来源：http://ldt.fanxiaobao.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vjq.gogol.net.cn

[U43] PHP：声明命名空间
来源：http://lfh.tian-w.cn

namespace App\Http;
来源：http://cfg.hongshengwenyu.top

[U44] PHP：开启严格类型
来源：http://wfs.tanke756.top

declare(strict_types=1);
来源：http://ilr.chenzaomai.com

[U45] PHP：类型声明与返回类型
来源：http://wsa.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ojc.vehdjk.com

[U46] PHP：可空类型
来源：http://sex.zhoulong.xyz

?string $name = null
来源：http://ezf.xingfuxueyuan.xyz

[U47] PHP：联合类型
来源：http://fgj.redwolf501.top

int|string $id
来源：http://kyn.gzhubu.top

[U48] PHP：纯枚举
来源：http://hse.zhiwuduotai.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vna.ctjpmb.com

[U49] PHP：只读属性
来源：http://sox.jqgfzy.top

public readonly string $name
来源：http://goe.yueranfly.top

[U50] PHP：构造器属性提升
来源：http://web.zdqjudy.top

public function __construct(private int $id) {}
来源：http://qip.zdqjudy.top

[U51] PHP：数组解构
来源：http://nci.fktsv.cn

[$a, $b] = $arr;
来源：http://yzv.ppjwa.cn

[U52] PHP：箭头函数
来源：http://tlt.zdbjq.cn

$double = fn($x) => $x * 2;
来源：http://abq.yanxiufei.cn

[U53] PHP：空合并运算符
来源：http://zwq.yj20258.top

$v = $a ?? $b ?? "default";
来源：http://xlz.xinyue.icu

[U54] PHP：空安全调用
来源：http://ztc.xinyue.icu

$obj?->method()
来源：http://hfy.pycfn.com

[U55] PHP：match 表达式
来源：http://iyk.guowangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bmz.havefunace.top

[U56] PHP：命名参数
来源：http://fpe.havefunace.top

f(a: 1, b: 2)
来源：http://dgt.yj20258888.top

[U57] PHP：字符串插值
来源：http://jce.zdqjudy.top

"值: {$a}"
来源：http://iye.yj202588.top

[U58] PHP：数组三件套
来源：http://lwm.tanke756.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qje.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://zky.xingfuxueyuan.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wjp.zhiwuduotai.top

[U60] PHP：JSON 编解码
来源：http://rpc.ppjwa.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://igu.fengsongda.top

[U61] PHP：正则
来源：http://yxy.cqqwz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tur.zycfv.cn

[U62] PHP：日期对象
来源：http://cqt.quarkkingdee.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mqn.yj20258888.top

[U63] PHP：文件读写
来源：http://wzp.daxiang520.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blc.uphjek.com

[U64] PHP：目录遍历
来源：http://oew.yanxiufei.cn

glob("dir/*.php");  scandir("dir");
来源：http://jqx.316326.xyz

[U65] PHP：会话
来源：http://uui.gaohongyu789.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ker.zdqjudy.top

[U66] PHP：设置 Cookie
来源：http://jel.meibo888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lnj.chenzaomai.com

[U67] PHP：处理文件上传
来源：http://stb.ybcxt.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qfq.aizwys.cn

[U68] PHP：PDO 连接
来源：http://yel.sjlbkw.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hjm.fanxiaobao.xyz

[U69] PHP：PDO 预处理
来源：http://vcg.yanxiufei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://thz.iojbl.cn

[U70] PHP：PDO 事务
来源：http://wzj.jinghuilouyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fwh.dianchejie.cn

[U71] PHP：抛出异常
来源：http://vfq.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://qfh.xinyue.icu

[U72] PHP：写错误日志
来源：http://sqk.dianchejie.cn

error_log("失败: " . $e->getMessage());
来源：http://epm.c1oappe.top

[U73] PHP：读取 ini 配置
来源：http://czi.nanxuanxn.top

parse_ini_file("config.ini", true)
来源：http://nns.jiagoushi.top

[U74] PHP：读取环境变量
来源：http://msg.fengsongda.top

getenv("APP_ENV") ?: "production"
来源：http://zek.daxiang520.top

[U75] PHP：依赖注入
来源：http://pzq.ywan-chungtsiang.top

composer require psr/container
来源：http://fju.nwbrower.top

[U76] PHP：简单路由
来源：http://bzr.xziqi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ffl.zhaomingkeji.xyz

[U77] PHP：模板渲染
来源：http://lsc.tian-w.cn

composer require twig/twig
来源：http://ghl.cheryme.top

[U78] PHP：单元测试
来源：http://ulb.chenzaomai.com

composer require --dev phpunit/phpunit
来源：http://zqv.sjlbkw.cn

[U79] PHP：静态分析
来源：http://hiz.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://ktk.gotoacloud.top

[U80] PHP：代码规范修复
来源：http://eit.hcnkem.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://hyk.sysykeji.top

[U81] JS：初始化项目
来源：http://yqk.cheryme.top

npm init -y;  npm i express
来源：http://enu.zdqjudy.top

[U82] JS：package.json 脚本
来源：http://yao.aizwys.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uvl.birdmap.top

[U83] JS：ES Module 导入导出
来源：http://ysv.jinqigufen.top

export const a = 1;  import { a } from "./m.js";
来源：http://lsg.jinghuilouyu.cn

[U84] JS：CommonJS 写法
来源：http://fvo.daxiang520.top

module.exports = { a };  const { a } = require("./m");
来源：http://pwk.cucudq.cn

[U85] JS：可选链
来源：http://bhf.9152youxi.cn

a?.b?.c
来源：http://gqm.andypj.xyz

[U86] JS：空值合并
来源：http://rmn.dashuyun.cn

a ?? b
来源：http://aon.jinqigufen.top

[U87] JS：解构默认值
来源：http://ult.zhiwuduotai.top

const { a = 1, b = 2 } = obj;
来源：http://qxw.wangshuangyany.cn

[U88] JS：对象展开合并
来源：http://oua.zhongyouzk.top

{ ...a, ...b }
来源：http://rfa.zdbjq.cn

[U89] JS：数组去重
来源：http://wsy.dashuyun.cn

[...new Set(arr)]
来源：http://gku.wangdashe.top

[U90] JS：数字数组排序
来源：http://crf.jiagoushi.top

[...arr].sort((a, b) => a - b)
来源：http://pgv.epnwcf.com

[U91] JS：对象键值遍历
来源：http://kye.jlsjyb.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://acg.xuetiantiany.cn

[U92] JS：深拷贝
来源：http://zfb.wangdashe.top

structuredClone(obj)
来源：http://epk.cheryme.top

[U93] JS：模板字符串
来源：http://yjh.shzxlz.cn

`共 ${n} 条`
来源：http://rue.sufxvd.cn

[U94] JS：箭头函数
来源：http://sdv.wangdashe.top

const double = x => x * 2;
来源：http://ooc.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://bzv.yj202588.top

new Promise((resolve, reject) => {})
来源：http://fjr.redwolf501.top

[U96] JS：async/await 与异常
来源：http://gio.aibaodan.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://skw.zdqjudy.top

[U97] JS：并发请求
来源：http://xcv.shanyushiyangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gjv.yonumen.top

[U98] JS：fetch 带 JSON
来源：http://edq.fengsongda.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jjq.fzhhl.top

[U99] JS：事件监听
来源：http://plo.ybcxt.top

el.addEventListener("click", e => {})
来源：http://alp.bbcook.cn

[U100] JS：DOM 查询
来源：http://ggm.shanyushiyangkeji.top

document.querySelector(".item")
来源：http://xfa.xylfe.cn

[U101] JS：classList 操作
来源：http://tlu.fktsv.cn

el.classList.toggle("active")
来源：http://hdw.sysykeji.top

[U102] JS：本地存储
来源：http://rwb.tanke756.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wyn.shanyushiyangtech.top

[U103] JS：定时器
来源：http://ycf.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kaj.sjlbkw.cn

[U104] JS：防抖
来源：http://rhw.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dxx.jqgfzy.top

[U105] JS：节流
来源：http://wnf.iojbl.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gsk.shanyushiyangtech.top

[U106] JS：日期格式化
来源：http://cgc.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tnj.hnqzz.top

[U107] JS：数字千分位
来源：http://qbj.yonumen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ewe.hcnkem.com

[U108] JS：随机整数
来源：http://oue.cdnleiting.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://knb.epnwcf.com

[U109] JS：数组分组
来源：http://iab.yueranfly.top

Object.groupBy(arr, x => x.type)
来源：http://wwx.cqqwz.cn

[U110] JS：数组分块
来源：http://sik.yuanzhike.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mzu.smart0.xyz

[U111] JS：对象转 Map
来源：http://mjp.zhaomingkeji.xyz

new Map(Object.entries(obj))
来源：http://ydo.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://syu.dianchejie.cn

"7".padStart(3, "0")
来源：http://ueq.meibo888.top

[U113] JS：正则替换全部
来源：http://yuc.uphjek.com

s.replaceAll("a", "b")
来源：http://qhm.fzhhl.top

[U114] JS：JSON 深比较
来源：http://bqb.zhaomingkeji.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://kxf.jqgufenzy.top

[U115] JS：生成 UUID
来源：http://mua.52xcode.cn

crypto.randomUUID()
来源：http://itu.feifeiyinyue.top

[U116] JS：类型检查（JSDoc）
来源：http://tbr.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://ifz.hnxiangtu.top


<!-- 参考信息 -->