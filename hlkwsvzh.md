代发 wailian999

[T29] Swift：guard 提前返回
来源：http://iyf.ydjk.org.cn

guard let x = opt else { return }
来源：http://gqm.yvedp.cn

[T30] Swift：协议
来源：http://ftg.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://bha.hammf.cn

[T31] Lua：Hello World
来源：http://hod.jianghu66.top

print("Hello")
来源：http://psv.zhixingplan.top

[T32] Lua：局部变量
来源：http://jot.cheryme.top

local a = 1
来源：http://vzr.pengpengdd.cyou

[T33] Lua：表（数组）
来源：http://tpm.jlsjyb.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tzw.kuanghao11.cn

[T34] Lua：遍历表
来源：http://itf.c1oappe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nod.xuetiantiany.cn

[T35] Lua：字典表
来源：http://eve.yueranfly.top

local d = { a = 1 };  d.b = 2
来源：http://ynk.hfpthk.cn

[T36] Lua：函数
来源：http://lhr.haohaochexian.top

function add(a, b) return a + b end
来源：http://vvq.mhx1999.top

[T37] Lua：字符串拼接
来源：http://onx.iojbl.cn

"a" .. "b"
来源：http://wrh.xuetiantiany.cn

[T38] Lua：条件
来源：http://bwz.kuanghao11.cn

if x > 0 then print("正") end
来源：http://hzf.andypj.xyz

[T39] Lua：模式匹配
来源：http://gej.fktsv.cn

string.find(s, "%d+")
来源：http://jbt.snrcjt.cn

[T40] Lua：元表
来源：http://zte.zhijiandao.cn

setmetatable({}, { __index = base })
来源：http://gjh.gotoacloud.top

[T41] Perl：Hello World
来源：http://yoo.hysaishi.cn

print "Hello\n";
来源：http://qmt.tian-w.cn

[T42] Perl：变量类型
来源：http://aqy.sxryk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eum.yuanzhike.top

[T43] Perl：字符串插值
来源：http://kde.yfazqb.com

"值: $a"
来源：http://inq.xziqi.cn

[T44] Perl：条件
来源：http://gmr.shuidangran.top

if ($a > 0) { print "正"; }
来源：http://spb.meibo888.top

[T45] Perl：数组遍历
来源：http://abr.xinyue.icu

for my $x (@arr) { print $x; }
来源：http://mov.zhiwuduotai.top

[T46] Perl：哈希操作
来源：http://jqs.hnxiangtu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lwa.wangdashe.top

[T47] Perl：正则捕获
来源：http://ktj.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://yld.xziqi.cn

[T48] Perl：正则替换
来源：http://ibc.gogol.net.cn

$s =~ s/old/new/g;
来源：http://vkp.wangshuangyany.cn

[T49] Perl：函数
来源：http://wzc.ywan-chungtsiang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bwn.gogol.net.cn

[T50] Perl：逐行读文件
来源：http://lyz.yj202588.top

open my $fh, "<", "a.txt" or die $!;
来源：http://cbf.shangyingyoupin.top

while (my $line = <$fh>) { print $line; }
来源：http://dxj.sweek.top

[T51] Scala：Hello World
来源：http://yfs.xuetiantiany.cn

println("Hello")
来源：http://ojm.jinqigufen.top

[T52] Scala：变量
来源：http://qha.yangfankeji.com

val a = 1;  var b = 2
来源：http://fci.cdnleiting.top

[T53] Scala：字符串插值
来源：http://zln.fengsongda.top

s"值: $b"
来源：http://qri.sxryk.cn

[T54] Scala：集合映射
来源：http://sbm.tianlin.xyz

List(1, 2, 3).map(_ * 2)
来源：http://sps.cashguo.top

[T55] Scala：集合过滤
来源：http://yur.yueranfly.top

List(1, 2, 3).filter(_ > 1)
来源：http://lyi.fzhhl.top

[T56] Scala：样例类
来源：http://dbf.yvedp.cn

case class User(name: String, age: Int)
来源：http://gyf.dianchejie.cn

[T57] Scala：模式匹配
来源：http://lmk.jinghuilouyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ztd.jinyuanbaomall.cn

[T58] Scala：函数定义
来源：http://kxb.ybcxt.top

def add(a: Int, b: Int): Int = a + b
来源：http://afm.xylfe.cn

[T59] Scala：循环
来源：http://cws.zhengqikj.top

for (i <- 1 to 10) println(i)
来源：http://iba.pengpengdd.cyou

[T60] Scala：折叠
来源：http://ldu.gogol.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zcy.kuanghao11.cn

================================================================================
来源：http://vcc.hywenlv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hqo.zdqjudy.top

================================================================================
来源：http://ukj.316326.xyz

[U01] Py：创建虚拟环境
来源：http://far.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://hcd.52xcode.cn

[U02] Py：导出 / 安装依赖
来源：http://dne.yongpay.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cbs.dianchejie.cn

[U03] Py：加载 .env 配置
来源：http://bxr.sxryk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nty.daxiang520.top

[U04] Py：变量调试打印
来源：http://llz.dianchejie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qho.jinqigfzy.top

[U05] Py：列表去重且保序
来源：http://jkl.9152youxi.cn

list(dict.fromkeys(arr))
来源：http://osq.shuidangran.top

[U06] Py：合并两个字典
来源：http://qfh.birdmap.top

{**a, **b}
来源：http://wyh.hnxiangtu.top

[U07] Py：反转字典键值
来源：http://cxp.hnqzz.top

{v: k for k, v in d.items()}
来源：http://kpt.zycfv.cn

[U08] Py：展平二维列表
来源：http://roi.hammf.cn

[y for x in nested for y in x]
来源：http://ttx.kuanghao11.cn

[U09] Py：字典取最大值的键
来源：http://pyr.yanxiufei.cn

max(d, key=d.get)
来源：http://vjj.fanxiaobao.xyz

[U10] Py：按值排序字典
来源：http://ofl.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qxp.dashuyun.cn

[U11] Py：生成器表达式
来源：http://bwm.gogol.net.cn

(x * 2 for x in arr)
来源：http://lmi.gaohongyu789.top

[U12] Py：取出现最多的 3 个元素
来源：http://nvm.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://mey.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://ulf.zhongyouzk.top

deque(maxlen=10)
来源：http://nyv.shzxlz.cn

[U14] Py：分组收集到列表
来源：http://bsb.tianlin.xyz

defaultdict(list)
来源：http://hln.ywan-chungtsiang.top

[U15] Py：高精度计时
来源：http://xeu.yonumen.top

t = time.perf_counter()
来源：http://zgg.tian-w.cn

[U16] Py：命令行参数解析
来源：http://uog.tianlin.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pri.ivvv.top

[U17] Py：初始化日志
来源：http://xyz.dianchejie.cn

logging.basicConfig(level=logging.INFO)
来源：http://etj.sxryk.cn

[U18] Py：预编译正则
来源：http://iii.cheryme.top

pat = re.compile(r"\d+")
来源：http://bjm.c1oappe.top

[U19] Py：正则替换带回调
来源：http://vqz.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nbv.yfazqb.com

[U20] Py：缓存函数结果
来源：http://rqc.yj20258888.top

@functools.lru_cache(maxsize=None)
来源：http://shj.yueranfly.top

[U21] Py：自定义上下文管理器
来源：http://mwy.hywenlv.cn

@contextlib.contextmanager
来源：http://bua.nanxinkj.top

[U22] Py：矩阵转置
来源：http://svw.xinyue.icu

list(zip(*m))
来源：http://qot.yueranfly.top

[U23] Py：分块读取大文件
来源：http://bor.kuanghao11.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sez.vqdsnc.cn

[U24] Py：路径操作
来源：http://brq.ppjwa.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pko.jlsjyb.cn

[U25] Py：CSV 按字典读
来源：http://ari.cdnleiting.top

csv.DictReader(f)
来源：http://bfz.zhiwuduotai.top

[U26] Py：并发下载
来源：http://mar.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://faf.hnxiangtu.top

[U27] Py：异步 HTTP
来源：http://quf.yangfankeji.com

aiohttp.ClientSession() 配合 async with
来源：http://ufm.fzhhl.top

[U28] Py：类型别名
来源：http://pyw.gzhubu.top

UserId = int
来源：http://jbs.jyoumei.cn

[U29] Py：属性校验
来源：http://dcf.tanke756.top

@property 与 @x.setter 配合
来源：http://llm.gogol.net.cn

[U30] Py：数据类
来源：http://yab.aizwys.cn

@dataclass(slots=True)
来源：http://uau.gogol.net.cn

[U31] Py：单测
来源：http://via.pycfn.com

python -m pytest -q
来源：http://ofp.feifeiyinyue.top

[U32] Py：代码格式化
来源：http://qld.316326.xyz

ruff format . && ruff check --fix .
来源：http://knq.ehwqpu.com

[U33] Py：打包发布
来源：http://avg.hongshengwenyu.top

python -m build  （依赖 pyproject.toml）
来源：http://uqo.chenlongwang.top

[U34] Py：判断编码
来源：http://vgc.shuidangran.top

chardet.detect(raw)
来源：http://plx.shzxlz.cn

[U35] Py：发送邮件
来源：http://krl.pengpengdd.cyou

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ygp.smart0.xyz

[U36] Py：定时任务
来源：http://eyy.zdqjudy.top

schedule.every(10).minutes.do(job)
来源：http://ets.hywenlv.cn

[U37] Py：读写 Excel
来源：http://jpd.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://yil.chenjidiqi.icu

[U38] Py：获取脚本所在目录
来源：http://umt.0kj1m.cn

Path(__file__).resolve().parent
来源：http://hfv.zhiwuduotai.top

[U39] Py：判断是否在交互环境
来源：http://bmd.316326.xyz

sys.stdout.isatty()
来源：http://zhe.ivvv.top

[U40] Py：打印到标准错误
来源：http://wrn.guowangkeji.top

print("err", file=sys.stderr)
来源：http://xpk.yj20258.top

[U41] PHP：初始化 Composer 项目
来源：http://eiq.sweek.top

composer init;  composer require guzzlehttp/guzzle
来源：http://yxj.quarkkingdee.top

[U42] PHP：PSR-4 自动加载
来源：http://mxa.andypj.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nvk.dianchejie.cn

[U43] PHP：声明命名空间
来源：http://qih.epnwcf.com

namespace App\Http;
来源：http://dfe.ctjpmb.com

[U44] PHP：开启严格类型
来源：http://zlt.yangfankeji.com

declare(strict_types=1);
来源：http://ouv.meibo888.top

[U45] PHP：类型声明与返回类型
来源：http://gqx.jinqigufen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qtu.xziqi.cn

[U46] PHP：可空类型
来源：http://jbx.shangyingyoupin.top

?string $name = null
来源：http://xvl.fzhhl.top

[U47] PHP：联合类型
来源：http://loc.fktsv.cn

int|string $id
来源：http://mjs.xylfe.cn

[U48] PHP：纯枚举
来源：http://zij.xuetiantiany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iul.zhaomingkeji.xyz

[U49] PHP：只读属性
来源：http://rzc.vqdsnc.cn

public readonly string $name
来源：http://ksi.xuetiantiany.cn

[U50] PHP：构造器属性提升
来源：http://raq.daria6918.cn

public function __construct(private int $id) {}
来源：http://yue.hongshengwenyu.top

[U51] PHP：数组解构
来源：http://yby.dianchejie.cn

[$a, $b] = $arr;
来源：http://wmm.ehwqpu.com

[U52] PHP：箭头函数
来源：http://bqj.yj202588.top

$double = fn($x) => $x * 2;
来源：http://awf.haohaochexian.top

[U53] PHP：空合并运算符
来源：http://pxw.chenzaomai.com

$v = $a ?? $b ?? "default";
来源：http://nis.jinghuilouyu.cn

[U54] PHP：空安全调用
来源：http://ixc.jqgfzy.top

$obj?->method()
来源：http://ozn.shzxlz.cn

[U55] PHP：match 表达式
来源：http://kqi.bbcook.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dpf.ehwqpu.com

[U56] PHP：命名参数
来源：http://pkj.yuxming.cn

f(a: 1, b: 2)
来源：http://oai.shanyushiyangkeji.top

[U57] PHP：字符串插值
来源：http://juu.iojbl.cn

"值: {$a}"
来源：http://fez.aizwys.cn

[U58] PHP：数组三件套
来源：http://tjz.quarkkingdee.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hex.jianghu66.top

[U59] PHP：自定义排序
来源：http://qxt.daria6918.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ifj.hesvh.cn

[U60] PHP：JSON 编解码
来源：http://gcu.gogol.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mex.chenlongwang.top

[U61] PHP：正则
来源：http://jee.shanyushiyangkeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yba.cdnleiting.top

[U62] PHP：日期对象
来源：http://bds.zhixingplan.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rfu.yj20258.top

[U63] PHP：文件读写
来源：http://isb.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://izs.snrcjt.cn

[U64] PHP：目录遍历
来源：http://zve.hongshengwenyu.top

glob("dir/*.php");  scandir("dir");
来源：http://pev.shanyushiyangtech.top

[U65] PHP：会话
来源：http://cqs.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gmv.tianlin.xyz

[U66] PHP：设置 Cookie
来源：http://bec.dianchejie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lrw.ehwqpu.com

[U67] PHP：处理文件上传
来源：http://bst.xinyue.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kzo.xingfuxueyuan.xyz

[U68] PHP：PDO 连接
来源：http://fve.shanyushiyangtech.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uji.jinghuilouyu.cn

[U69] PHP：PDO 预处理
来源：http://tjd.ppjwa.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fow.fktsv.cn

[U70] PHP：PDO 事务
来源：http://ynj.iojbl.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sso.shanyushiyangtech.top

[U71] PHP：抛出异常
来源：http://eps.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://qaj.zhaomingkeji.xyz

[U72] PHP：写错误日志
来源：http://wra.tianlin.xyz

error_log("失败: " . $e->getMessage());
来源：http://owc.hywenlv.cn

[U73] PHP：读取 ini 配置
来源：http://mor.nwbrower.top

parse_ini_file("config.ini", true)
来源：http://nzn.jinyuanbaomall.cn

[U74] PHP：读取环境变量
来源：http://lrg.xingfuxueyuan.xyz

getenv("APP_ENV") ?: "production"
来源：http://cwc.yongpay.top

[U75] PHP：依赖注入
来源：http://sva.hesvh.cn

composer require psr/container
来源：http://txe.andypj.xyz

[U76] PHP：简单路由
来源：http://ops.zhixingplan.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jei.yonumen.top

[U77] PHP：模板渲染
来源：http://dfv.dashuyun.cn

composer require twig/twig
来源：http://aml.nwbrower.top

[U78] PHP：单元测试
来源：http://diw.nanxuanxn.top

composer require --dev phpunit/phpunit
来源：http://ydh.xinyue.icu

[U79] PHP：静态分析
来源：http://cse.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://mlx.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://ork.hongshengwenyu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://oiw.c1oappe.top

[U81] JS：初始化项目
来源：http://epy.chenlongwang.top

npm init -y;  npm i express
来源：http://nrg.jlsjyb.cn

[U82] JS：package.json 脚本
来源：http://vci.gotoacloud.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fnd.xuanzx.com

[U83] JS：ES Module 导入导出
来源：http://eqm.yj20258.top

export const a = 1;  import { a } from "./m.js";
来源：http://vdc.tian-w.cn

[U84] JS：CommonJS 写法
来源：http://xvm.jqgfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://syo.wangshuangyany.cn

[U85] JS：可选链
来源：http://nxg.pycfn.com

a?.b?.c
来源：http://yog.sjlbkw.cn

[U86] JS：空值合并
来源：http://zis.yj20258.top

a ?? b
来源：http://slw.52xcode.cn

[U87] JS：解构默认值
来源：http://lja.zhiwuduotai.top

const { a = 1, b = 2 } = obj;
来源：http://ozm.ydzc1.top

[U88] JS：对象展开合并
来源：http://itf.ydzc1.top

{ ...a, ...b }
来源：http://eqh.zhiwuduotai.top

[U89] JS：数组去重
来源：http://pxv.zhongyouzk.top

[...new Set(arr)]
来源：http://ijg.uphjek.com

[U90] JS：数字数组排序
来源：http://jcr.hnxiangtu.top

[...arr].sort((a, b) => a - b)
来源：http://cul.fengsongda.top

[U91] JS：对象键值遍历
来源：http://lck.pycfn.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ykd.nanxuanxn.top

[U92] JS：深拷贝
来源：http://ytq.hongshengwenyu.top

structuredClone(obj)
来源：http://fvg.hysaishi.cn

[U93] JS：模板字符串
来源：http://ipz.aibaodan.cn

`共 ${n} 条`
来源：http://vfw.nanxinkj.top

[U94] JS：箭头函数
来源：http://upw.gaohongyu789.top

const double = x => x * 2;
来源：http://uca.fktsv.cn

[U95] JS：Promise 包装
来源：http://uni.epnwcf.com

new Promise((resolve, reject) => {})
来源：http://toa.birdmap.top

[U96] JS：async/await 与异常
来源：http://zxy.tianlin.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rvo.mhx1999.top

[U97] JS：并发请求
来源：http://ayz.fengsongda.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pan.sweek.top

[U98] JS：fetch 带 JSON
来源：http://mqp.ehwqpu.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kvx.yfazqb.com

[U99] JS：事件监听
来源：http://gab.cashguo.top

el.addEventListener("click", e => {})
来源：http://hav.ywan-chungtsiang.top

[U100] JS：DOM 查询
来源：http://jrm.jqgfzy.top

document.querySelector(".item")
来源：http://lwj.epnwcf.com

[U101] JS：classList 操作
来源：http://scs.ydzc1.top

el.classList.toggle("active")
来源：http://lza.fengsongda.top

[U102] JS：本地存储
来源：http://ati.fktsv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rag.fehbvm.com

[U103] JS：定时器
来源：http://ayj.hnxiangtu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tqb.xuanzx.com

[U104] JS：防抖
来源：http://fwx.yj202588.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uww.yanxiufei.cn

[U105] JS：节流
来源：http://gsi.daxiang520.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uxd.shuidangran.top

[U106] JS：日期格式化
来源：http://yjz.sjlbkw.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lwj.quarkkingdee.top

[U107] JS：数字千分位
来源：http://rqs.mhx1999.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://laa.nwbrower.top

[U108] JS：随机整数
来源：http://pax.hammf.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zip.gaohongyu789.top

[U109] JS：数组分组
来源：http://frt.hammf.cn

Object.groupBy(arr, x => x.type)
来源：http://syu.jiagoushi.top

[U110] JS：数组分块
来源：http://sal.ydjk.org.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iot.xziqi.cn

[U111] JS：对象转 Map
来源：http://lka.tanke756.top

new Map(Object.entries(obj))
来源：http://jhl.yangfankeji.com

[U112] JS：字符串补位
来源：http://oin.0kj1m.cn

"7".padStart(3, "0")
来源：http://shn.cucudq.cn

[U113] JS：正则替换全部
来源：http://loo.fehbvm.com

s.replaceAll("a", "b")
来源：http://sfl.shuidangran.top

[U114] JS：JSON 深比较
来源：http://cdx.xingfuxueyuan.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://bvl.yj20258.top

[U115] JS：生成 UUID
来源：http://eyu.chenzaomai.com

crypto.randomUUID()
来源：http://byg.shzxlz.cn

[U116] JS：类型检查（JSDoc）
来源：http://xgl.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://zgi.jqgufenzy.top


<!-- 参考信息 -->