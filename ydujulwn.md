代发 wailian999

[T29] Swift：guard 提前返回
来源：http://iyd.gaohongyu789.top

guard let x = opt else { return }
来源：http://som.iojbl.cn

[T30] Swift：协议
来源：http://htj.wangdashe.top

protocol Shape { func area() -> Double }
来源：http://lcj.pycfn.com

[T31] Lua：Hello World
来源：http://dxp.xylfe.cn

print("Hello")
来源：http://fjj.yvedp.cn

[T32] Lua：局部变量
来源：http://fes.gotoacloud.top

local a = 1
来源：http://jxx.zhongyouzk.top

[T33] Lua：表（数组）
来源：http://yaz.xziqi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qxi.cucudq.cn

[T34] Lua：遍历表
来源：http://yhc.nanxuanxn.top

for i, v in ipairs(t) do print(i, v) end
来源：http://elt.gzhubu.top

[T35] Lua：字典表
来源：http://fbo.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://jto.feifeiyinyue.top

[T36] Lua：函数
来源：http://ust.guowangkeji.top

function add(a, b) return a + b end
来源：http://ucg.epnwcf.com

[T37] Lua：字符串拼接
来源：http://ngx.pengpengdd.cyou

"a" .. "b"
来源：http://gyh.jinqigfzy.top

[T38] Lua：条件
来源：http://zuq.hysaishi.cn

if x > 0 then print("正") end
来源：http://mrm.hongshengwenyu.top

[T39] Lua：模式匹配
来源：http://awm.shangyingyoupin.top

string.find(s, "%d+")
来源：http://gzl.tianlin.xyz

[T40] Lua：元表
来源：http://rpa.andypj.xyz

setmetatable({}, { __index = base })
来源：http://wpu.ctjpmb.com

[T41] Perl：Hello World
来源：http://czn.haohaochexian.top

print "Hello\n";
来源：http://lhc.zdbjq.cn

[T42] Perl：变量类型
来源：http://xnn.andypj.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fyq.yfazqb.com

[T43] Perl：字符串插值
来源：http://lme.shangyingyoupin.top

"值: $a"
来源：http://pym.svipenyu.cn

[T44] Perl：条件
来源：http://agr.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://tra.xuanzx.com

[T45] Perl：数组遍历
来源：http://ewk.nwbrower.top

for my $x (@arr) { print $x; }
来源：http://yih.guowangkeji.top

[T46] Perl：哈希操作
来源：http://axx.dashuyun.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rns.yj202588.top

[T47] Perl：正则捕获
来源：http://fun.zhengqikj.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yca.hnxiangtu.top

[T48] Perl：正则替换
来源：http://hwj.kuanghao11.cn

$s =~ s/old/new/g;
来源：http://acj.yangfankeji.com

[T49] Perl：函数
来源：http://zbb.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qmi.daxiang520.top

[T50] Perl：逐行读文件
来源：http://jsi.ctjpmb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://whe.zhongyouzk.top

while (my $line = <$fh>) { print $line; }
来源：http://lng.dianchejie.cn

[T51] Scala：Hello World
来源：http://fzv.daxiang520.top

println("Hello")
来源：http://wcc.shuidangran.top

[T52] Scala：变量
来源：http://udv.yvedp.cn

val a = 1;  var b = 2
来源：http://gid.gaohongyu789.top

[T53] Scala：字符串插值
来源：http://gym.zhiwuduotai.top

s"值: $b"
来源：http://mde.ybcxt.top

[T54] Scala：集合映射
来源：http://vbc.yuanzhike.top

List(1, 2, 3).map(_ * 2)
来源：http://crz.guannengcc.top

[T55] Scala：集合过滤
来源：http://qum.shzxlz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uwf.snrcjt.cn

[T56] Scala：样例类
来源：http://rcf.hnxiangtu.top

case class User(name: String, age: Int)
来源：http://kuq.chenjidiqi.icu

[T57] Scala：模式匹配
来源：http://ovi.jianghu66.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://udz.jinyuanbaomall.cn

[T58] Scala：函数定义
来源：http://tof.0kj1m.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mcq.fzhhl.top

[T59] Scala：循环
来源：http://bic.nanxuanxn.top

for (i <- 1 to 10) println(i)
来源：http://ozp.hnqzz.top

[T60] Scala：折叠
来源：http://jcn.aibaodan.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mvs.vehdjk.com

================================================================================
来源：http://ghv.dashuyun.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wdb.fengsongda.top

================================================================================
来源：http://ypx.tianlin.xyz

[U01] Py：创建虚拟环境
来源：http://ffl.zhijiandao.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rtz.jianghu66.top

[U02] Py：导出 / 安装依赖
来源：http://daz.cdnleiting.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qvd.52xcode.cn

[U03] Py：加载 .env 配置
来源：http://ccd.ywan-chungtsiang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ups.epnwcf.com

[U04] Py：变量调试打印
来源：http://jpi.hnqzz.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ysr.redwolf501.top

[U05] Py：列表去重且保序
来源：http://met.jinghuilouyu.cn

list(dict.fromkeys(arr))
来源：http://iai.zhongyouzk.top

[U06] Py：合并两个字典
来源：http://obi.9152youxi.cn

{**a, **b}
来源：http://tdy.snrcjt.cn

[U07] Py：反转字典键值
来源：http://yqy.hnxiangtu.top

{v: k for k, v in d.items()}
来源：http://bvp.cqqwz.cn

[U08] Py：展平二维列表
来源：http://pls.meibo888.top

[y for x in nested for y in x]
来源：http://eqi.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://dbx.sweek.top

max(d, key=d.get)
来源：http://tky.shangyingyoupin.top

[U10] Py：按值排序字典
来源：http://zem.pengpengdd.cyou

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yua.zhongyouzk.top

[U11] Py：生成器表达式
来源：http://xyp.tanke756.top

(x * 2 for x in arr)
来源：http://jeh.birdmap.top

[U12] Py：取出现最多的 3 个元素
来源：http://cua.zdqjudy.top

Counter(arr).most_common(3)
来源：http://ulo.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://adi.hesvh.cn

deque(maxlen=10)
来源：http://lkr.shanyushiyangkeji.top

[U14] Py：分组收集到列表
来源：http://aax.hnqzz.top

defaultdict(list)
来源：http://gmn.xziqi.cn

[U15] Py：高精度计时
来源：http://lpd.jinghuilouyu.cn

t = time.perf_counter()
来源：http://mwg.hammf.cn

[U16] Py：命令行参数解析
来源：http://bid.smart0.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ipp.xuanzx.com

[U17] Py：初始化日志
来源：http://fqk.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://bez.xingfuxueyuan.xyz

[U18] Py：预编译正则
来源：http://mme.guowangkeji.top

pat = re.compile(r"\d+")
来源：http://rsr.wangshuangyany.cn

[U19] Py：正则替换带回调
来源：http://cky.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yhg.wangshuangyany.cn

[U20] Py：缓存函数结果
来源：http://mgb.yj20258.top

@functools.lru_cache(maxsize=None)
来源：http://xot.aibaodan.cn

[U21] Py：自定义上下文管理器
来源：http://sfi.shangyingyoupin.top

@contextlib.contextmanager
来源：http://qhd.zhoulong.xyz

[U22] Py：矩阵转置
来源：http://iwp.iojbl.cn

list(zip(*m))
来源：http://nhc.sjlbkw.cn

[U23] Py：分块读取大文件
来源：http://sfv.shanyushiyangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xzm.zhaomingkeji.xyz

[U24] Py：路径操作
来源：http://sxf.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://boc.zhaomingkeji.xyz

[U25] Py：CSV 按字典读
来源：http://jqw.jinghuilouyu.cn

csv.DictReader(f)
来源：http://dih.redwolf501.top

[U26] Py：并发下载
来源：http://phs.yj202588.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ogy.ehwqpu.com

[U27] Py：异步 HTTP
来源：http://gcw.andypj.xyz

aiohttp.ClientSession() 配合 async with
来源：http://ork.shangyingyoupin.top

[U28] Py：类型别名
来源：http://kau.meibo888.top

UserId = int
来源：http://niw.0kj1m.cn

[U29] Py：属性校验
来源：http://yvv.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://fkq.guowangkeji.top

[U30] Py：数据类
来源：http://vwy.sjlbkw.cn

@dataclass(slots=True)
来源：http://dcv.wangdashe.top

[U31] Py：单测
来源：http://erm.bjfxy.top

python -m pytest -q
来源：http://zgm.fehbvm.com

[U32] Py：代码格式化
来源：http://bng.aibaodan.cn

ruff format . && ruff check --fix .
来源：http://duf.cashguo.top

[U33] Py：打包发布
来源：http://idi.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://xsg.zhixingplan.top

[U34] Py：判断编码
来源：http://iwq.hammf.cn

chardet.detect(raw)
来源：http://mms.shuidangran.top

[U35] Py：发送邮件
来源：http://inm.havefunace.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://prn.zhengqikj.top

[U36] Py：定时任务
来源：http://jgr.pycfn.com

schedule.every(10).minutes.do(job)
来源：http://otb.fengsongda.top

[U37] Py：读写 Excel
来源：http://mrs.zhaomingkeji.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://bar.epnwcf.com

[U38] Py：获取脚本所在目录
来源：http://iqw.fzhhl.top

Path(__file__).resolve().parent
来源：http://qop.gaohongyu789.top

[U39] Py：判断是否在交互环境
来源：http://pcr.ybcxt.top

sys.stdout.isatty()
来源：http://foc.gotoacloud.top

[U40] Py：打印到标准错误
来源：http://lit.shanyushiyangtech.top

print("err", file=sys.stderr)
来源：http://qpj.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://scp.bbcook.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lzo.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://lvg.fehbvm.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bkn.birdmap.top

[U43] PHP：声明命名空间
来源：http://bin.hongshengwenyu.top

namespace App\Http;
来源：http://dys.shanyushiyangtech.top

[U44] PHP：开启严格类型
来源：http://zzl.sxryk.cn

declare(strict_types=1);
来源：http://bfw.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://kxf.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zri.fktsv.cn

[U46] PHP：可空类型
来源：http://gsd.hywenlv.cn

?string $name = null
来源：http://szn.gogol.net.cn

[U47] PHP：联合类型
来源：http://yzp.xylfe.cn

int|string $id
来源：http://oek.zhengqikj.top

[U48] PHP：纯枚举
来源：http://lrm.fanxiaobao.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xvu.yj20258888.top

[U49] PHP：只读属性
来源：http://khp.gogol.net.cn

public readonly string $name
来源：http://ltw.xuetiantiany.cn

[U50] PHP：构造器属性提升
来源：http://psq.tarul.cn

public function __construct(private int $id) {}
来源：http://hlb.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://eqs.yj20258888.top

[$a, $b] = $arr;
来源：http://prz.uphjek.com

[U52] PHP：箭头函数
来源：http://ihp.yanxiufei.cn

$double = fn($x) => $x * 2;
来源：http://vlx.guannengcc.top

[U53] PHP：空合并运算符
来源：http://wcu.hnqzz.top

$v = $a ?? $b ?? "default";
来源：http://fow.zhaomingkeji.xyz

[U54] PHP：空安全调用
来源：http://vau.andypj.xyz

$obj?->method()
来源：http://zhg.hywenlv.cn

[U55] PHP：match 表达式
来源：http://nmf.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nni.shangyingyoupin.top

[U56] PHP：命名参数
来源：http://krr.yangfankeji.com

f(a: 1, b: 2)
来源：http://kzn.hywenlv.cn

[U57] PHP：字符串插值
来源：http://ogk.hongshengwenyu.top

"值: {$a}"
来源：http://bjn.tianlin.xyz

[U58] PHP：数组三件套
来源：http://lpn.snrcjt.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://taw.nwbrower.top

[U59] PHP：自定义排序
来源：http://erw.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hdz.jinqigfzy.top

[U60] PHP：JSON 编解码
来源：http://qot.hysaishi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vyu.tian-w.cn

[U61] PHP：正则
来源：http://qrn.chenzaomai.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hah.zdbjq.cn

[U62] PHP：日期对象
来源：http://cad.cheryme.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sby.pycfn.com

[U63] PHP：文件读写
来源：http://dlr.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xog.bbcook.cn

[U64] PHP：目录遍历
来源：http://jue.shanyushiyangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://pwk.tarul.cn

[U65] PHP：会话
来源：http://rlu.hfpthk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pfy.dashuyun.cn

[U66] PHP：设置 Cookie
来源：http://igf.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xoo.yueranfly.top

[U67] PHP：处理文件上传
来源：http://yrw.sufxvd.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xtj.jinyuanbaomall.cn

[U68] PHP：PDO 连接
来源：http://zkn.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kil.guowangkeji.top

[U69] PHP：PDO 预处理
来源：http://eal.jinqigfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://txl.wangdashe.top

[U70] PHP：PDO 事务
来源：http://jxn.dianchejie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zvl.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://ghe.xingfuxueyuan.xyz

throw new RuntimeException("失败", 500);
来源：http://oot.xinyue.icu

[U72] PHP：写错误日志
来源：http://kka.guannengcc.top

error_log("失败: " . $e->getMessage());
来源：http://rzi.andypj.xyz

[U73] PHP：读取 ini 配置
来源：http://zxk.jyoumei.cn

parse_ini_file("config.ini", true)
来源：http://dxl.yuanzhike.top

[U74] PHP：读取环境变量
来源：http://mxp.jlsjyb.cn

getenv("APP_ENV") ?: "production"
来源：http://fzh.shzxlz.cn

[U75] PHP：依赖注入
来源：http://mmd.nwbrower.top

composer require psr/container
来源：http://kjd.shanyushiyangkeji.top

[U76] PHP：简单路由
来源：http://oix.jianghu66.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yys.shuidangran.top

[U77] PHP：模板渲染
来源：http://cnh.hongshengwenyu.top

composer require twig/twig
来源：http://zhi.chenzaomai.com

[U78] PHP：单元测试
来源：http://vup.jlsjyb.cn

composer require --dev phpunit/phpunit
来源：http://vbo.hammf.cn

[U79] PHP：静态分析
来源：http://haz.jlsjyb.cn

composer require --dev phpstan/phpstan
来源：http://wwj.cheryme.top

[U80] PHP：代码规范修复
来源：http://jep.redwolf501.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://fud.jqgufenzy.top

[U81] JS：初始化项目
来源：http://yot.zhongyouzk.top

npm init -y;  npm i express
来源：http://lkx.yuxming.cn

[U82] JS：package.json 脚本
来源：http://nvi.yuxming.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lxx.daria6918.cn

[U83] JS：ES Module 导入导出
来源：http://tbd.chenzaomai.com

export const a = 1;  import { a } from "./m.js";
来源：http://pzy.zhijiandao.cn

[U84] JS：CommonJS 写法
来源：http://oof.yueranfly.top

module.exports = { a };  const { a } = require("./m");
来源：http://rqc.xingfuxueyuan.xyz

[U85] JS：可选链
来源：http://ziq.zdbjq.cn

a?.b?.c
来源：http://sdt.fengsongda.top

[U86] JS：空值合并
来源：http://cob.epnwcf.com

a ?? b
来源：http://ctr.yj20258.top

[U87] JS：解构默认值
来源：http://ayz.nwbrower.top

const { a = 1, b = 2 } = obj;
来源：http://zcz.jyoumei.cn

[U88] JS：对象展开合并
来源：http://ruw.daria6918.cn

{ ...a, ...b }
来源：http://fqh.daxiang520.top

[U89] JS：数组去重
来源：http://eux.sufxvd.cn

[...new Set(arr)]
来源：http://fhl.uphjek.com

[U90] JS：数字数组排序
来源：http://vvl.bjfxy.top

[...arr].sort((a, b) => a - b)
来源：http://pfl.yangfankeji.com

[U91] JS：对象键值遍历
来源：http://xdk.haohaochexian.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://elo.epnwcf.com

[U92] JS：深拷贝
来源：http://wey.jinghuilouyu.cn

structuredClone(obj)
来源：http://orv.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://lqr.yj202588.top

`共 ${n} 条`
来源：http://wwv.haohaochexian.top

[U94] JS：箭头函数
来源：http://vtk.chenzaomai.com

const double = x => x * 2;
来源：http://qcb.svipenyu.cn

[U95] JS：Promise 包装
来源：http://bwc.yanxiufei.cn

new Promise((resolve, reject) => {})
来源：http://ebs.zhiwuduotai.top

[U96] JS：async/await 与异常
来源：http://sjb.yonumen.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zmr.shzxlz.cn

[U97] JS：并发请求
来源：http://ums.hfpthk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://grb.jyoumei.cn

[U98] JS：fetch 带 JSON
来源：http://dmo.cucudq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bln.hysaishi.cn

[U99] JS：事件监听
来源：http://hgy.havefunace.top

el.addEventListener("click", e => {})
来源：http://kgo.nwbrower.top

[U100] JS：DOM 查询
来源：http://yax.uphjek.com

document.querySelector(".item")
来源：http://otl.yuanzhike.top

[U101] JS：classList 操作
来源：http://lci.daxiang520.top

el.classList.toggle("active")
来源：http://fbm.chenzaomai.com

[U102] JS：本地存储
来源：http://odq.yuxming.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wrw.zhengqikj.top

[U103] JS：定时器
来源：http://oze.xylfe.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nuv.zdqjudy.top

[U104] JS：防抖
来源：http://foq.shanyushiyangtech.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lax.zhixingplan.top

[U105] JS：节流
来源：http://wey.shuidangran.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://twc.zhijiandao.cn

[U106] JS：日期格式化
来源：http://kaj.yj20258.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://czz.zycfv.cn

[U107] JS：数字千分位
来源：http://gea.fengsongda.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hff.ctjpmb.com

[U108] JS：随机整数
来源：http://yza.pengpengdd.cyou

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jwy.xinyue.icu

[U109] JS：数组分组
来源：http://emx.dianchejie.cn

Object.groupBy(arr, x => x.type)
来源：http://zyg.pycfn.com

[U110] JS：数组分块
来源：http://tta.0kj1m.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pwb.pycfn.com

[U111] JS：对象转 Map
来源：http://keb.pycfn.com

new Map(Object.entries(obj))
来源：http://tqy.316326.xyz

[U112] JS：字符串补位
来源：http://pdk.daxiang520.top

"7".padStart(3, "0")
来源：http://rsr.chenlongwang.top

[U113] JS：正则替换全部
来源：http://ooy.fanxiaobao.xyz

s.replaceAll("a", "b")
来源：http://uor.sxryk.cn

[U114] JS：JSON 深比较
来源：http://vgp.tianlin.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://eoz.xziqi.cn

[U115] JS：生成 UUID
来源：http://xpq.shanyushiyangtech.top

crypto.randomUUID()
来源：http://fsj.fktsv.cn

[U116] JS：类型检查（JSDoc）
来源：http://nuu.pycfn.com

/** @param {string} name */ function f(name) {}
来源：http://huy.kuanghao11.cn


<!-- 参考信息 -->