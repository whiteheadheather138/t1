代发 wailian999

[T17] Swift：变量与常量
来源：https://by.zhonguo4118.cn

var a = 1;  let b = 2
来源：https://gf.zhonguo2118.cn

[T18] Swift：字符串插值
来源：https://qc.zhonguo1118.cn

"值: \(b)"
来源：https://kd.zhonguo4118.cn

[T19] Swift：可选绑定
来源：https://gr.zhonguo7118.cn

if let n = opt { print(n) }
来源：https://mr.zhonguo7118.cn

[T20] Swift：数组操作
来源：https://tr.zhonguo4118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://yg.zhonguo7118.cn

[T21] Swift：遍历
来源：https://tq.zhonguo5118.cn

for x in a { print(x) }
来源：https://ls.zhonguo3118.cn

[T22] Swift：字典
来源：https://qw.zhonguo4118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://tz.zhonguo8118.cn

[T23] Swift：函数
来源：https://nh.zhonguo5118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://ox.zhonguo3118.cn

[T24] Swift：闭包
来源：https://pk.zhonguo3118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://js.zhonguo4118.cn

[T25] Swift：结构体
来源：https://oq.zhonguo3118.cn

struct P { var x: Int }
来源：https://uv.zhonguo1118.cn

[T26] Swift：类与重写
来源：https://iu.zhonguo8118.cn

class A: Base { override func f() {} }
来源：https://gg.zhonguo5118.cn

[T27] Swift：错误处理
来源：https://kb.zhonguo6118.cn

do { try f() } catch { print(error) }
来源：https://ny.zhonguo7118.cn

[T28] Swift：枚举
来源：https://sl.zhonguo6118.cn

enum Color { case red, green }
来源：https://rt.zhonguo8118.cn

[T29] Swift：guard 提前返回
来源：https://en.zhonguo1118.cn

guard let x = opt else { return }
来源：https://nq.zhonguo8118.cn

[T30] Swift：协议
来源：https://be.zhonguo2118.cn

protocol Shape { func area() -> Double }
来源：https://yw.zhonguo6118.cn

[T31] Lua：Hello World
来源：https://nd.zhonguo1118.cn

print("Hello")
来源：https://hg.zhonguo4118.cn

[T32] Lua：局部变量
来源：https://zb.zhonguo2118.cn

local a = 1
来源：https://zt.zhonguo2118.cn

[T33] Lua：表（数组）
来源：https://bu.zhonguo1118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://oq.zhonguo8118.cn

[T34] Lua：遍历表
来源：https://kc.zhonguo5118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://ni.zhonguo7118.cn

[T35] Lua：字典表
来源：https://gs.zhonguo3118.cn

local d = { a = 1 };  d.b = 2
来源：https://bm.zhonguo8118.cn

[T36] Lua：函数
来源：https://wf.zhonguo5118.cn

function add(a, b) return a + b end
来源：https://po.zhonguo5118.cn

[T37] Lua：字符串拼接
来源：https://hy.zhonguo7118.cn

"a" .. "b"
来源：https://yi.zhonguo1118.cn

[T38] Lua：条件
来源：https://rj.zhonguo7118.cn

if x > 0 then print("正") end
来源：https://re.zhonguo5118.cn

[T39] Lua：模式匹配
来源：https://iy.zhonguo7118.cn

string.find(s, "%d+")
来源：https://sd.zhonguo2118.cn

[T40] Lua：元表
来源：https://ef.zhonguo4118.cn

setmetatable({}, { __index = base })
来源：https://ac.zhonguo2118.cn

[T41] Perl：Hello World
来源：https://gh.zhonguo7118.cn

print "Hello\n";
来源：https://wi.zhonguo2118.cn

[T42] Perl：变量类型
来源：https://ke.zhonguo7118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://et.zhonguo6118.cn

[T43] Perl：字符串插值
来源：https://fu.zhonguo6118.cn

"值: $a"
来源：https://lq.zhonguo3118.cn

[T44] Perl：条件
来源：https://ii.zhonguo1118.cn

if ($a > 0) { print "正"; }
来源：https://hi.zhonguo7118.cn

[T45] Perl：数组遍历
来源：https://bl.zhonguo8118.cn

for my $x (@arr) { print $x; }
来源：https://ip.zhonguo2118.cn

[T46] Perl：哈希操作
来源：https://oq.zhonguo7118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://vy.zhonguo5118.cn

[T47] Perl：正则捕获
来源：https://tj.zhonguo2118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://fv.zhonguo5118.cn

[T48] Perl：正则替换
来源：https://bt.zhonguo5118.cn

$s =~ s/old/new/g;
来源：https://el.zhonguo2118.cn

[T49] Perl：函数
来源：https://bt.zhonguo5118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://gg.zhonguo8118.cn

[T50] Perl：逐行读文件
来源：https://xh.zhonguo7118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://gj.zhonguo3118.cn

while (my $line = <$fh>) { print $line; }
来源：https://fp.zhonguo7118.cn

[T51] Scala：Hello World
来源：https://vb.zhonguo2118.cn

println("Hello")
来源：https://zk.zhonguo5118.cn

[T52] Scala：变量
来源：https://td.zhonguo2118.cn

val a = 1;  var b = 2
来源：https://mx.zhonguo8118.cn

[T53] Scala：字符串插值
来源：https://lv.zhonguo7118.cn

s"值: $b"
来源：https://lx.zhonguo6118.cn

[T54] Scala：集合映射
来源：https://zi.zhonguo4118.cn

List(1, 2, 3).map(_ * 2)
来源：https://ys.zhonguo5118.cn

[T55] Scala：集合过滤
来源：https://xi.zhonguo6118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://al.zhonguo7118.cn

[T56] Scala：样例类
来源：https://fm.zhonguo4118.cn

case class User(name: String, age: Int)
来源：https://fn.zhonguo1118.cn

[T57] Scala：模式匹配
来源：https://mf.zhonguo7118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://rv.zhonguo6118.cn

[T58] Scala：函数定义
来源：https://gs.zhonguo2118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://nz.zhonguo5118.cn

[T59] Scala：循环
来源：https://vl.zhonguo5118.cn

for (i <- 1 to 10) println(i)
来源：https://pb.zhonguo2118.cn

[T60] Scala：折叠
来源：https://qw.zhonguo2118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://yn.zhonguo2118.cn

================================================================================
来源：https://or.zhonguo8118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://xr.zhonguo7118.cn

================================================================================
来源：https://ie.zhonguo7118.cn

[U01] Py：创建虚拟环境
来源：https://wt.zhonguo2118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://ug.zhonguo2118.cn

[U02] Py：导出 / 安装依赖
来源：https://sa.zhonguo8118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://fk.zhonguo3118.cn

[U03] Py：加载 .env 配置
来源：https://og.zhonguo2118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://bm.zhonguo8118.cn

[U04] Py：变量调试打印
来源：https://os.zhonguo2118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://je.zhonguo7118.cn

[U05] Py：列表去重且保序
来源：https://qp.zhonguo5118.cn

list(dict.fromkeys(arr))
来源：https://jf.zhonguo3118.cn

[U06] Py：合并两个字典
来源：https://un.zhonguo6118.cn

{**a, **b}
来源：https://lb.zhonguo7118.cn

[U07] Py：反转字典键值
来源：https://ur.zhonguo3118.cn

{v: k for k, v in d.items()}
来源：https://zo.zhonguo6118.cn

[U08] Py：展平二维列表
来源：https://fk.zhonguo4118.cn

[y for x in nested for y in x]
来源：https://xt.zhonguo7118.cn

[U09] Py：字典取最大值的键
来源：https://zm.zhonguo1118.cn

max(d, key=d.get)
来源：https://eu.zhonguo2118.cn

[U10] Py：按值排序字典
来源：https://je.zhonguo6118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://qw.zhonguo7118.cn

[U11] Py：生成器表达式
来源：https://zr.zhonguo1118.cn

(x * 2 for x in arr)
来源：https://jh.zhonguo5118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://xh.zhonguo4118.cn

Counter(arr).most_common(3)
来源：https://dd.zhonguo6118.cn

[U13] Py：固定长度队列
来源：https://cg.zhonguo5118.cn

deque(maxlen=10)
来源：https://hb.zhonguo1118.cn

[U14] Py：分组收集到列表
来源：https://ae.zhonguo6118.cn

defaultdict(list)
来源：https://jp.zhonguo6118.cn

[U15] Py：高精度计时
来源：https://zt.zhonguo3118.cn

t = time.perf_counter()
来源：https://oo.zhonguo8118.cn

[U16] Py：命令行参数解析
来源：https://zm.zhonguo1118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://im.zhonguo1118.cn

[U17] Py：初始化日志
来源：https://pq.zhonguo7118.cn

logging.basicConfig(level=logging.INFO)
来源：https://fl.zhonguo7118.cn

[U18] Py：预编译正则
来源：https://xn.zhonguo4118.cn

pat = re.compile(r"\d+")
来源：https://ll.zhonguo4118.cn

[U19] Py：正则替换带回调
来源：https://zq.zhonguo2118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://aw.zhonguo6118.cn

[U20] Py：缓存函数结果
来源：https://gr.zhonguo1118.cn

@functools.lru_cache(maxsize=None)
来源：https://ct.zhonguo3118.cn

[U21] Py：自定义上下文管理器
来源：https://iv.zhonguo8118.cn

@contextlib.contextmanager
来源：https://aw.zhonguo1118.cn

[U22] Py：矩阵转置
来源：https://jj.zhonguo2118.cn

list(zip(*m))
来源：https://ar.zhonguo4118.cn

[U23] Py：分块读取大文件
来源：https://aq.zhonguo7118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://tk.zhonguo2118.cn

[U24] Py：路径操作
来源：https://wk.zhonguo8118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://yv.zhonguo1118.cn

[U25] Py：CSV 按字典读
来源：https://cr.zhonguo3118.cn

csv.DictReader(f)
来源：https://bt.zhonguo5118.cn

[U26] Py：并发下载
来源：https://hn.zhonguo3118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://fa.zhonguo5118.cn

[U27] Py：异步 HTTP
来源：https://ml.zhonguo1118.cn

aiohttp.ClientSession() 配合 async with
来源：https://jo.zhonguo5118.cn

[U28] Py：类型别名
来源：https://sk.zhonguo8118.cn

UserId = int
来源：https://ai.zhonguo5118.cn

[U29] Py：属性校验
来源：https://jk.zhonguo5118.cn

@property 与 @x.setter 配合
来源：https://zs.zhonguo4118.cn

[U30] Py：数据类
来源：https://tz.zhonguo2118.cn

@dataclass(slots=True)
来源：https://fe.zhonguo7118.cn

[U31] Py：单测
来源：https://dq.zhonguo3118.cn

python -m pytest -q
来源：https://yn.zhonguo3118.cn

[U32] Py：代码格式化
来源：https://pj.zhonguo4118.cn

ruff format . && ruff check --fix .
来源：https://za.zhonguo8118.cn

[U33] Py：打包发布
来源：https://hr.zhonguo3118.cn

python -m build  （依赖 pyproject.toml）
来源：https://ox.zhonguo4118.cn

[U34] Py：判断编码
来源：https://mc.zhonguo3118.cn

chardet.detect(raw)
来源：https://oe.zhonguo4118.cn

[U35] Py：发送邮件
来源：https://fl.zhonguo2118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://qj.zhonguo3118.cn

[U36] Py：定时任务
来源：https://di.zhonguo3118.cn

schedule.every(10).minutes.do(job)
来源：https://ag.zhonguo8118.cn

[U37] Py：读写 Excel
来源：https://uw.zhonguo5118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://et.zhonguo8118.cn

[U38] Py：获取脚本所在目录
来源：https://fg.zhonguo8118.cn

Path(__file__).resolve().parent
来源：https://jd.zhonguo1118.cn

[U39] Py：判断是否在交互环境
来源：https://rg.zhonguo6118.cn

sys.stdout.isatty()
来源：https://wj.zhonguo5118.cn

[U40] Py：打印到标准错误
来源：https://yk.zhonguo4118.cn

print("err", file=sys.stderr)
来源：https://iu.zhonguo5118.cn

[U41] PHP：初始化 Composer 项目
来源：https://fl.zhonguo1118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://lv.zhonguo3118.cn

[U42] PHP：PSR-4 自动加载
来源：https://vx.zhonguo2118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://pc.zhonguo4118.cn

[U43] PHP：声明命名空间
来源：https://jr.zhonguo2118.cn

namespace App\Http;
来源：https://hi.zhonguo5118.cn

[U44] PHP：开启严格类型
来源：https://ip.zhonguo3118.cn

declare(strict_types=1);
来源：https://sw.zhonguo8118.cn

[U45] PHP：类型声明与返回类型
来源：https://ie.zhonguo1118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://xu.zhonguo8118.cn

[U46] PHP：可空类型
来源：https://rn.zhonguo2118.cn

?string $name = null
来源：https://ly.zhonguo3118.cn

[U47] PHP：联合类型
来源：https://qe.zhonguo2118.cn

int|string $id
来源：https://rt.zhonguo1118.cn

[U48] PHP：纯枚举
来源：https://cn.zhonguo7118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://wn.zhonguo4118.cn

[U49] PHP：只读属性
来源：https://fa.zhonguo5118.cn

public readonly string $name
来源：https://im.zhonguo6118.cn

[U50] PHP：构造器属性提升
来源：https://nt.zhonguo8118.cn

public function __construct(private int $id) {}
来源：https://dy.zhonguo4118.cn

[U51] PHP：数组解构
来源：https://uj.zhonguo2118.cn

[$a, $b] = $arr;
来源：https://zp.zhonguo4118.cn

[U52] PHP：箭头函数
来源：https://qi.zhonguo7118.cn

$double = fn($x) => $x * 2;
来源：https://ow.zhonguo4118.cn

[U53] PHP：空合并运算符
来源：https://qq.zhonguo1118.cn

$v = $a ?? $b ?? "default";
来源：https://rz.zhonguo1118.cn

[U54] PHP：空安全调用
来源：https://uf.zhonguo6118.cn

$obj?->method()
来源：https://cz.zhonguo5118.cn

[U55] PHP：match 表达式
来源：https://fw.zhonguo2118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://ey.zhonguo6118.cn

[U56] PHP：命名参数
来源：https://kx.zhonguo3118.cn

f(a: 1, b: 2)
来源：https://tb.zhonguo6118.cn

[U57] PHP：字符串插值
来源：https://jy.zhonguo3118.cn

"值: {$a}"
来源：https://id.zhonguo1118.cn

[U58] PHP：数组三件套
来源：https://mn.zhonguo8118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://fd.zhonguo6118.cn

[U59] PHP：自定义排序
来源：https://kx.zhonguo7118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://dt.zhonguo8118.cn

[U60] PHP：JSON 编解码
来源：https://nd.zhonguo7118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://rk.zhonguo2118.cn

[U61] PHP：正则
来源：https://yn.zhonguo7118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://dr.zhonguo4118.cn

[U62] PHP：日期对象
来源：https://gj.zhonguo5118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://yq.zhonguo8118.cn

[U63] PHP：文件读写
来源：https://qf.zhonguo3118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://lt.zhonguo2118.cn

[U64] PHP：目录遍历
来源：https://dd.zhonguo7118.cn

glob("dir/*.php");  scandir("dir");
来源：https://it.zhonguo2118.cn

[U65] PHP：会话
来源：https://zb.zhonguo7118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://cv.zhonguo3118.cn

[U66] PHP：设置 Cookie
来源：https://xo.zhonguo7118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://uh.zhonguo8118.cn

[U67] PHP：处理文件上传
来源：https://ns.zhonguo6118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://vb.zhonguo6118.cn

[U68] PHP：PDO 连接
来源：https://on.zhonguo8118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://re.zhonguo1118.cn

[U69] PHP：PDO 预处理
来源：https://rj.zhonguo1118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://gu.zhonguo1118.cn

[U70] PHP：PDO 事务
来源：https://nz.zhonguo1118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://wi.zhonguo8118.cn

[U71] PHP：抛出异常
来源：https://pi.zhonguo1118.cn

throw new RuntimeException("失败", 500);
来源：https://fi.zhonguo7118.cn

[U72] PHP：写错误日志
来源：https://qi.zhonguo1118.cn

error_log("失败: " . $e->getMessage());
来源：https://fa.zhonguo7118.cn

[U73] PHP：读取 ini 配置
来源：https://zw.zhonguo2118.cn

parse_ini_file("config.ini", true)
来源：https://cu.zhonguo3118.cn

[U74] PHP：读取环境变量
来源：https://ez.zhonguo1118.cn

getenv("APP_ENV") ?: "production"
来源：https://do.zhonguo2118.cn

[U75] PHP：依赖注入
来源：https://wo.zhonguo8118.cn

composer require psr/container
来源：https://hi.zhonguo8118.cn

[U76] PHP：简单路由
来源：https://up.zhonguo1118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://qn.zhonguo8118.cn

[U77] PHP：模板渲染
来源：https://aa.zhonguo8118.cn

composer require twig/twig
来源：https://qm.zhonguo8118.cn

[U78] PHP：单元测试
来源：https://ik.zhonguo4118.cn

composer require --dev phpunit/phpunit
来源：https://yf.zhonguo8118.cn

[U79] PHP：静态分析
来源：https://pd.zhonguo4118.cn

composer require --dev phpstan/phpstan
来源：https://go.zhonguo3118.cn

[U80] PHP：代码规范修复
来源：https://wu.zhonguo7118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://bi.zhonguo8118.cn

[U81] JS：初始化项目
来源：https://pu.zhonguo4118.cn

npm init -y;  npm i express
来源：https://gm.zhonguo2118.cn

[U82] JS：package.json 脚本
来源：https://cq.zhonguo8118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://zj.zhonguo8118.cn

[U83] JS：ES Module 导入导出
来源：https://va.zhonguo2118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://rt.zhonguo4118.cn

[U84] JS：CommonJS 写法
来源：https://mx.zhonguo7118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://qg.zhonguo2118.cn

[U85] JS：可选链
来源：https://dr.zhonguo5118.cn

a?.b?.c
来源：https://hh.zhonguo8118.cn

[U86] JS：空值合并
来源：https://eq.zhonguo8118.cn

a ?? b
来源：https://rt.zhonguo8118.cn

[U87] JS：解构默认值
来源：https://gn.zhonguo6118.cn

const { a = 1, b = 2 } = obj;
来源：https://lt.zhonguo3118.cn

[U88] JS：对象展开合并
来源：https://bd.zhonguo6118.cn

{ ...a, ...b }
来源：https://la.zhonguo2118.cn

[U89] JS：数组去重
来源：https://ky.zhonguo3118.cn

[...new Set(arr)]
来源：https://sv.zhonguo4118.cn

[U90] JS：数字数组排序
来源：https://pl.zhonguo7118.cn

[...arr].sort((a, b) => a - b)
来源：https://ow.zhonguo6118.cn

[U91] JS：对象键值遍历
来源：https://nr.zhonguo2118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://dn.zhonguo3118.cn

[U92] JS：深拷贝
来源：https://ek.zhonguo8118.cn

structuredClone(obj)
来源：https://if.zhonguo3118.cn

[U93] JS：模板字符串
来源：https://nv.zhonguo6118.cn

`共 ${n} 条`
来源：https://pb.zhonguo2118.cn

[U94] JS：箭头函数
来源：https://ql.zhonguo2118.cn

const double = x => x * 2;
来源：https://ao.zhonguo8118.cn

[U95] JS：Promise 包装
来源：https://xw.zhonguo8118.cn

new Promise((resolve, reject) => {})
来源：https://vd.zhonguo3118.cn

[U96] JS：async/await 与异常
来源：https://yz.zhonguo5118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://tt.zhonguo2118.cn

[U97] JS：并发请求
来源：https://xk.zhonguo2118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://cj.zhonguo4118.cn

[U98] JS：fetch 带 JSON
来源：https://hm.zhonguo5118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://os.zhonguo8118.cn

[U99] JS：事件监听
来源：https://eg.zhonguo2118.cn

el.addEventListener("click", e => {})
来源：https://de.zhonguo2118.cn

[U100] JS：DOM 查询
来源：https://cw.zhonguo4118.cn

document.querySelector(".item")
来源：https://up.zhonguo8118.cn

[U101] JS：classList 操作
来源：https://th.zhonguo2118.cn

el.classList.toggle("active")
来源：https://ay.zhonguo5118.cn

[U102] JS：本地存储
来源：https://ja.zhonguo7118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://ni.zhonguo1118.cn

[U103] JS：定时器
来源：https://gj.zhonguo3118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://fr.zhonguo3118.cn

[U104] JS：防抖
来源：https://cj.zhonguo6118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://lr.zhonguo4118.cn


<!-- 参考信息 -->