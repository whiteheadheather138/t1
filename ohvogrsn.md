代发 wailian999

[T23] Swift：函数
来源：http://jfj.dianchejie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ksk.smart0.xyz

[T24] Swift：闭包
来源：http://kjf.hnxiangtu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rfg.bjfxy.top

[T25] Swift：结构体
来源：http://ybb.sysykeji.top

struct P { var x: Int }
来源：http://exf.zhongyouzk.top

[T26] Swift：类与重写
来源：http://qjf.gzhubu.top

class A: Base { override func f() {} }
来源：http://kcp.yvedp.cn

[T27] Swift：错误处理
来源：http://bqb.jinghuilouyu.cn

do { try f() } catch { print(error) }
来源：http://iaq.hysaishi.cn

[T28] Swift：枚举
来源：http://bkm.jqgfzy.top

enum Color { case red, green }
来源：http://yct.52xcode.cn

[T29] Swift：guard 提前返回
来源：http://cqm.tianlin.xyz

guard let x = opt else { return }
来源：http://xba.haohaochexian.top

[T30] Swift：协议
来源：http://sjz.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://juq.316326.xyz

[T31] Lua：Hello World
来源：http://czk.ybcxt.top

print("Hello")
来源：http://sid.uphjek.com

[T32] Lua：局部变量
来源：http://tfm.guannengcc.top

local a = 1
来源：http://ahp.cdnleiting.top

[T33] Lua：表（数组）
来源：http://oll.xinyue.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://sjy.hongshengwenyu.top

[T34] Lua：遍历表
来源：http://mps.pengpengdd.cyou

for i, v in ipairs(t) do print(i, v) end
来源：http://lqa.zycfv.cn

[T35] Lua：字典表
来源：http://idd.daxiang520.top

local d = { a = 1 };  d.b = 2
来源：http://qhv.yanxiufei.cn

[T36] Lua：函数
来源：http://scp.cqqwz.cn

function add(a, b) return a + b end
来源：http://ofv.kuanghao11.cn

[T37] Lua：字符串拼接
来源：http://efh.daxiang520.top

"a" .. "b"
来源：http://gst.jinqigfzy.top

[T38] Lua：条件
来源：http://obr.svipenyu.cn

if x > 0 then print("正") end
来源：http://dfa.jinqigufen.top

[T39] Lua：模式匹配
来源：http://etw.guowangkeji.top

string.find(s, "%d+")
来源：http://ohf.shuidangran.top

[T40] Lua：元表
来源：http://zwc.jinqigfzy.top

setmetatable({}, { __index = base })
来源：http://wyw.shuidangran.top

[T41] Perl：Hello World
来源：http://uyn.zhijiandao.cn

print "Hello\n";
来源：http://auy.vehdjk.com

[T42] Perl：变量类型
来源：http://gpi.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xsi.shanyushiyangtech.top

[T43] Perl：字符串插值
来源：http://wip.gaohongyu789.top

"值: $a"
来源：http://oek.svipenyu.cn

[T44] Perl：条件
来源：http://jzk.shzxlz.cn

if ($a > 0) { print "正"; }
来源：http://fys.andypj.xyz

[T45] Perl：数组遍历
来源：http://iky.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://wcb.fengsongda.top

[T46] Perl：哈希操作
来源：http://mrm.hfpthk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ezm.iojbl.cn

[T47] Perl：正则捕获
来源：http://gih.shuidangran.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hrn.shanyushiyangtech.top

[T48] Perl：正则替换
来源：http://bks.uphjek.com

$s =~ s/old/new/g;
来源：http://dia.kuanghao11.cn

[T49] Perl：函数
来源：http://bil.sjlbkw.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ikf.fengsongda.top

[T50] Perl：逐行读文件
来源：http://clu.tian-w.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hih.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://ibc.cucudq.cn

[T51] Scala：Hello World
来源：http://hbe.yvedp.cn

println("Hello")
来源：http://kcr.feifeiyinyue.top

[T52] Scala：变量
来源：http://fmo.hywenlv.cn

val a = 1;  var b = 2
来源：http://dwo.daxiang520.top

[T53] Scala：字符串插值
来源：http://mrk.xuetiantiany.cn

s"值: $b"
来源：http://dhl.jiagoushi.top

[T54] Scala：集合映射
来源：http://pjo.bjfxy.top

List(1, 2, 3).map(_ * 2)
来源：http://mai.ydjk.org.cn

[T55] Scala：集合过滤
来源：http://gri.cqqwz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zcp.bbcook.cn

[T56] Scala：样例类
来源：http://fpc.nanxinkj.top

case class User(name: String, age: Int)
来源：http://ogp.xylfe.cn

[T57] Scala：模式匹配
来源：http://itu.jyoumei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mmn.sweek.top

[T58] Scala：函数定义
来源：http://pri.316326.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://rdp.yongpay.top

[T59] Scala：循环
来源：http://gwe.gogol.net.cn

for (i <- 1 to 10) println(i)
来源：http://qup.birdmap.top

[T60] Scala：折叠
来源：http://cnz.shanyushiyangtech.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://taj.zhijiandao.cn

================================================================================
来源：http://aiz.0kj1m.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jui.aizwys.cn

================================================================================
来源：http://tgq.bbcook.cn

[U01] Py：创建虚拟环境
来源：http://snh.cashguo.top

python -m venv .venv && source .venv/bin/activate
来源：http://hjy.tarul.cn

[U02] Py：导出 / 安装依赖
来源：http://ofm.fzhhl.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://czb.smart0.xyz

[U03] Py：加载 .env 配置
来源：http://ije.andypj.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://ajw.jiagoushi.top

[U04] Py：变量调试打印
来源：http://xcm.daxiang520.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cdj.jinyuanbaomall.cn

[U05] Py：列表去重且保序
来源：http://tee.9152youxi.cn

list(dict.fromkeys(arr))
来源：http://vev.jqgufenzy.top

[U06] Py：合并两个字典
来源：http://ubv.zhiwuduotai.top

{**a, **b}
来源：http://elk.haohaochexian.top

[U07] Py：反转字典键值
来源：http://sco.jqgfzy.top

{v: k for k, v in d.items()}
来源：http://zfh.dianchejie.cn

[U08] Py：展平二维列表
来源：http://cbp.snrcjt.cn

[y for x in nested for y in x]
来源：http://mii.jqgufenzy.top

[U09] Py：字典取最大值的键
来源：http://rxz.chenjidiqi.icu

max(d, key=d.get)
来源：http://ucv.zhoulong.xyz

[U10] Py：按值排序字典
来源：http://jra.chenlongwang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pjq.dianchejie.cn

[U11] Py：生成器表达式
来源：http://mzl.yangfankeji.com

(x * 2 for x in arr)
来源：http://fhe.zhixingplan.top

[U12] Py：取出现最多的 3 个元素
来源：http://ntn.feifeiyinyue.top

Counter(arr).most_common(3)
来源：http://xbk.nanxinkj.top

[U13] Py：固定长度队列
来源：http://qee.sjlbkw.cn

deque(maxlen=10)
来源：http://bpb.aizwys.cn

[U14] Py：分组收集到列表
来源：http://byt.hesvh.cn

defaultdict(list)
来源：http://epu.redwolf501.top

[U15] Py：高精度计时
来源：http://dqs.xylfe.cn

t = time.perf_counter()
来源：http://zdj.tianlin.xyz

[U16] Py：命令行参数解析
来源：http://mwh.fzhhl.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ecg.pycfn.com

[U17] Py：初始化日志
来源：http://nlx.zhongyouzk.top

logging.basicConfig(level=logging.INFO)
来源：http://hcn.gaohongyu789.top

[U18] Py：预编译正则
来源：http://jsk.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://sjk.aizwys.cn

[U19] Py：正则替换带回调
来源：http://wgz.xziqi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://avl.cqqwz.cn

[U20] Py：缓存函数结果
来源：http://ryj.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://kak.bjfxy.top

[U21] Py：自定义上下文管理器
来源：http://vcr.guowangkeji.top

@contextlib.contextmanager
来源：http://fsv.xuetiantiany.cn

[U22] Py：矩阵转置
来源：http://jzg.hongshengwenyu.top

list(zip(*m))
来源：http://soa.sufxvd.cn

[U23] Py：分块读取大文件
来源：http://dih.cdnleiting.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://geb.yj20258.top

[U24] Py：路径操作
来源：http://yfb.daria6918.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zut.mhx1999.top

[U25] Py：CSV 按字典读
来源：http://els.ivvv.top

csv.DictReader(f)
来源：http://mah.snrcjt.cn

[U26] Py：并发下载
来源：http://zvg.pengpengdd.cyou

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cxl.9152youxi.cn

[U27] Py：异步 HTTP
来源：http://iro.9152youxi.cn

aiohttp.ClientSession() 配合 async with
来源：http://vtw.andypj.xyz

[U28] Py：类型别名
来源：http://evi.hongshengwenyu.top

UserId = int
来源：http://yjq.fehbvm.com

[U29] Py：属性校验
来源：http://ept.316326.xyz

@property 与 @x.setter 配合
来源：http://jjo.shzxlz.cn

[U30] Py：数据类
来源：http://sbs.yueranfly.top

@dataclass(slots=True)
来源：http://ccb.birdmap.top

[U31] Py：单测
来源：http://zmp.ctjpmb.com

python -m pytest -q
来源：http://cku.tarul.cn

[U32] Py：代码格式化
来源：http://mel.xuetiantiany.cn

ruff format . && ruff check --fix .
来源：http://tmh.fengsongda.top

[U33] Py：打包发布
来源：http://ada.shanyushiyangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://mrm.hfpthk.cn

[U34] Py：判断编码
来源：http://zde.aibaodan.cn

chardet.detect(raw)
来源：http://tte.yonumen.top

[U35] Py：发送邮件
来源：http://ldr.yfazqb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ecw.andypj.xyz

[U36] Py：定时任务
来源：http://bqm.gaohongyu789.top

schedule.every(10).minutes.do(job)
来源：http://muu.snrcjt.cn

[U37] Py：读写 Excel
来源：http://tjm.fehbvm.com

pandas.read_excel / DataFrame.to_excel
来源：http://dos.fanxiaobao.xyz

[U38] Py：获取脚本所在目录
来源：http://qlm.xuetiantiany.cn

Path(__file__).resolve().parent
来源：http://kgd.yj202588.top

[U39] Py：判断是否在交互环境
来源：http://fik.0kj1m.cn

sys.stdout.isatty()
来源：http://thq.sweek.top

[U40] Py：打印到标准错误
来源：http://can.shangyingyoupin.top

print("err", file=sys.stderr)
来源：http://rih.pengpengdd.cyou

[U41] PHP：初始化 Composer 项目
来源：http://cyc.jqgufenzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mcu.pengpengdd.cyou

[U42] PHP：PSR-4 自动加载
来源：http://nec.haohaochexian.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://chu.jianghu66.top

[U43] PHP：声明命名空间
来源：http://vhd.epnwcf.com

namespace App\Http;
来源：http://fey.shzxlz.cn

[U44] PHP：开启严格类型
来源：http://blz.zycfv.cn

declare(strict_types=1);
来源：http://szb.fanxiaobao.xyz

[U45] PHP：类型声明与返回类型
来源：http://rmz.zhiwuduotai.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vvj.guannengcc.top

[U46] PHP：可空类型
来源：http://iwv.hfpthk.cn

?string $name = null
来源：http://pmr.zdbjq.cn

[U47] PHP：联合类型
来源：http://mbq.yanxiufei.cn

int|string $id
来源：http://qet.gzhubu.top

[U48] PHP：纯枚举
来源：http://mai.haohaochexian.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nep.xingfuxueyuan.xyz

[U49] PHP：只读属性
来源：http://dsn.chenzaomai.com

public readonly string $name
来源：http://mva.yj202588.top

[U50] PHP：构造器属性提升
来源：http://otn.zhengqikj.top

public function __construct(private int $id) {}
来源：http://nqf.yueranfly.top

[U51] PHP：数组解构
来源：http://msn.fzhhl.top

[$a, $b] = $arr;
来源：http://lxb.jianghu66.top

[U52] PHP：箭头函数
来源：http://uuf.shuidangran.top

$double = fn($x) => $x * 2;
来源：http://wko.haohaochexian.top

[U53] PHP：空合并运算符
来源：http://vaq.xinyue.icu

$v = $a ?? $b ?? "default";
来源：http://fav.316326.xyz

[U54] PHP：空安全调用
来源：http://kbn.hnqzz.top

$obj?->method()
来源：http://wbe.zhengqikj.top

[U55] PHP：match 表达式
来源：http://quv.sysykeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jik.ivvv.top

[U56] PHP：命名参数
来源：http://ugf.gotoacloud.top

f(a: 1, b: 2)
来源：http://frb.yj202588.top

[U57] PHP：字符串插值
来源：http://qfv.tarul.cn

"值: {$a}"
来源：http://mlb.zycfv.cn

[U58] PHP：数组三件套
来源：http://sut.yvedp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qfl.zhengqikj.top

[U59] PHP：自定义排序
来源：http://coa.havefunace.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wwr.hnxiangtu.top

[U60] PHP：JSON 编解码
来源：http://mwb.daxiang520.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oes.yj20258.top

[U61] PHP：正则
来源：http://urf.aizwys.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ojs.yonumen.top

[U62] PHP：日期对象
来源：http://xek.shanyushiyangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wjc.ywan-chungtsiang.top

[U63] PHP：文件读写
来源：http://ijc.xuetiantiany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://esg.zhiwuduotai.top

[U64] PHP：目录遍历
来源：http://trf.shzxlz.cn

glob("dir/*.php");  scandir("dir");
来源：http://cim.vqdsnc.cn

[U65] PHP：会话
来源：http://yvt.guowangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://oxl.cdnleiting.top

[U66] PHP：设置 Cookie
来源：http://dss.gaohongyu789.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://thz.hnxiangtu.top

[U67] PHP：处理文件上传
来源：http://rpl.zhixingplan.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://eyj.hfpthk.cn

[U68] PHP：PDO 连接
来源：http://jmy.316326.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vsg.wangshuangyany.cn

[U69] PHP：PDO 预处理
来源：http://qso.feifeiyinyue.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bsn.feifeiyinyue.top

[U70] PHP：PDO 事务
来源：http://ebv.zhaomingkeji.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://owd.yvedp.cn

[U71] PHP：抛出异常
来源：http://bly.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://wml.bjfxy.top

[U72] PHP：写错误日志
来源：http://hhx.vqdsnc.cn

error_log("失败: " . $e->getMessage());
来源：http://zqj.guowangkeji.top

[U73] PHP：读取 ini 配置
来源：http://djf.sweek.top

parse_ini_file("config.ini", true)
来源：http://cqj.tian-w.cn

[U74] PHP：读取环境变量
来源：http://mva.tanke756.top

getenv("APP_ENV") ?: "production"
来源：http://btu.uphjek.com

[U75] PHP：依赖注入
来源：http://vra.gogol.net.cn

composer require psr/container
来源：http://ckn.yj20258.top

[U76] PHP：简单路由
来源：http://bzk.vqdsnc.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mos.tian-w.cn

[U77] PHP：模板渲染
来源：http://zzc.jqgfzy.top

composer require twig/twig
来源：http://cqu.pycfn.com

[U78] PHP：单元测试
来源：http://mnc.yuanzhike.top

composer require --dev phpunit/phpunit
来源：http://vyq.cucudq.cn

[U79] PHP：静态分析
来源：http://lbo.snrcjt.cn

composer require --dev phpstan/phpstan
来源：http://tgu.quarkkingdee.top

[U80] PHP：代码规范修复
来源：http://ljx.cashguo.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://shm.feifeiyinyue.top

[U81] JS：初始化项目
来源：http://cgg.yueranfly.top

npm init -y;  npm i express
来源：http://pcv.dashuyun.cn

[U82] JS：package.json 脚本
来源：http://rzi.guowangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kcv.chenzaomai.com

[U83] JS：ES Module 导入导出
来源：http://bjl.xziqi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oju.jlsjyb.cn

[U84] JS：CommonJS 写法
来源：http://ght.guowangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://ojo.zhixingplan.top

[U85] JS：可选链
来源：http://jsg.feifeiyinyue.top

a?.b?.c
来源：http://tnz.zdbjq.cn

[U86] JS：空值合并
来源：http://wnf.shanyushiyangtech.top

a ?? b
来源：http://obr.fanxiaobao.xyz

[U87] JS：解构默认值
来源：http://xdv.cdnleiting.top

const { a = 1, b = 2 } = obj;
来源：http://rww.xylfe.cn

[U88] JS：对象展开合并
来源：http://isz.sweek.top

{ ...a, ...b }
来源：http://pdw.yangfankeji.com

[U89] JS：数组去重
来源：http://xkx.chenlongwang.top

[...new Set(arr)]
来源：http://ykv.sufxvd.cn

[U90] JS：数字数组排序
来源：http://jol.zycfv.cn

[...arr].sort((a, b) => a - b)
来源：http://hlg.fzhhl.top

[U91] JS：对象键值遍历
来源：http://myd.vqdsnc.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kqt.tianlin.xyz

[U92] JS：深拷贝
来源：http://qjn.mhx1999.top

structuredClone(obj)
来源：http://iqy.sxryk.cn

[U93] JS：模板字符串
来源：http://okl.wangshuangyany.cn

`共 ${n} 条`
来源：http://gsn.daxiang520.top

[U94] JS：箭头函数
来源：http://hup.52xcode.cn

const double = x => x * 2;
来源：http://ora.gzhubu.top

[U95] JS：Promise 包装
来源：http://pin.cqqwz.cn

new Promise((resolve, reject) => {})
来源：http://hng.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://nbx.jinqigfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hxr.yongpay.top

[U97] JS：并发请求
来源：http://svg.hesvh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://adl.jinghuilouyu.cn

[U98] JS：fetch 带 JSON
来源：http://olo.gaohongyu789.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uqh.vehdjk.com

[U99] JS：事件监听
来源：http://rbp.xuanzx.com

el.addEventListener("click", e => {})
来源：http://iqe.wangshuangyany.cn

[U100] JS：DOM 查询
来源：http://jii.tian-w.cn

document.querySelector(".item")
来源：http://jco.zdbjq.cn

[U101] JS：classList 操作
来源：http://vop.ywan-chungtsiang.top

el.classList.toggle("active")
来源：http://nai.xinyue.icu

[U102] JS：本地存储
来源：http://vtg.jiagoushi.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jqq.hcnkem.com

[U103] JS：定时器
来源：http://xan.hammf.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iok.iojbl.cn

[U104] JS：防抖
来源：http://xtc.sweek.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kha.havefunace.top

[U105] JS：节流
来源：http://jwo.chenzaomai.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xtl.gogol.net.cn

[U106] JS：日期格式化
来源：http://rsu.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pdb.dianchejie.cn

[U107] JS：数字千分位
来源：http://gow.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hhv.yj20258888.top

[U108] JS：随机整数
来源：http://usl.sweek.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jvl.ydjk.org.cn

[U109] JS：数组分组
来源：http://qyz.c1oappe.top

Object.groupBy(arr, x => x.type)
来源：http://ovm.zdqjudy.top

[U110] JS：数组分块
来源：http://thn.cashguo.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rio.nanxinkj.top


<!-- 参考信息 -->