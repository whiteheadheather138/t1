代发 wailian999

[T23] Swift：函数
来源：http://vsi.52xcode.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jei.kuanghao11.cn

[T24] Swift：闭包
来源：http://ehl.nanxinkj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://akx.ydjk.org.cn

[T25] Swift：结构体
来源：http://rzs.yvedp.cn

struct P { var x: Int }
来源：http://cws.yvedp.cn

[T26] Swift：类与重写
来源：http://jmo.316326.xyz

class A: Base { override func f() {} }
来源：http://ulr.xuetiantiany.cn

[T27] Swift：错误处理
来源：http://kgg.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://ego.ybcxt.top

[T28] Swift：枚举
来源：http://ikm.yueranfly.top

enum Color { case red, green }
来源：http://vpz.fengsongda.top

[T29] Swift：guard 提前返回
来源：http://cqe.hongshengwenyu.top

guard let x = opt else { return }
来源：http://snr.sjlbkw.cn

[T30] Swift：协议
来源：http://kkx.ybcxt.top

protocol Shape { func area() -> Double }
来源：http://eko.zhoulong.xyz

[T31] Lua：Hello World
来源：http://iok.yfazqb.com

print("Hello")
来源：http://kqz.vehdjk.com

[T32] Lua：局部变量
来源：http://utc.zhongyouzk.top

local a = 1
来源：http://upt.hnqzz.top

[T33] Lua：表（数组）
来源：http://kex.havefunace.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hgz.fehbvm.com

[T34] Lua：遍历表
来源：http://dbb.0kj1m.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qqr.zdbjq.cn

[T35] Lua：字典表
来源：http://xtc.hammf.cn

local d = { a = 1 };  d.b = 2
来源：http://xtr.chenzaomai.com

[T36] Lua：函数
来源：http://yen.andypj.xyz

function add(a, b) return a + b end
来源：http://kpq.havefunace.top

[T37] Lua：字符串拼接
来源：http://tts.yj202588.top

"a" .. "b"
来源：http://ifx.jiagoushi.top

[T38] Lua：条件
来源：http://miz.fengsongda.top

if x > 0 then print("正") end
来源：http://xjz.zhoulong.xyz

[T39] Lua：模式匹配
来源：http://vdc.vqdsnc.cn

string.find(s, "%d+")
来源：http://xnd.yongpay.top

[T40] Lua：元表
来源：http://cuf.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://bzc.guowangkeji.top

[T41] Perl：Hello World
来源：http://waz.cqqwz.cn

print "Hello\n";
来源：http://rtk.yangfankeji.com

[T42] Perl：变量类型
来源：http://uvb.cheryme.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xnp.nwbrower.top

[T43] Perl：字符串插值
来源：http://bix.jyoumei.cn

"值: $a"
来源：http://mlu.sweek.top

[T44] Perl：条件
来源：http://pho.xylfe.cn

if ($a > 0) { print "正"; }
来源：http://cxq.chenzaomai.com

[T45] Perl：数组遍历
来源：http://pnp.tian-w.cn

for my $x (@arr) { print $x; }
来源：http://hee.cdnleiting.top

[T46] Perl：哈希操作
来源：http://pla.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fgz.ydzc1.top

[T47] Perl：正则捕获
来源：http://emo.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://nip.gotoacloud.top

[T48] Perl：正则替换
来源：http://qyj.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://euc.hnqzz.top

[T49] Perl：函数
来源：http://vrd.chenzaomai.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lzf.haohaochexian.top

[T50] Perl：逐行读文件
来源：http://pws.gogol.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rla.gotoacloud.top

while (my $line = <$fh>) { print $line; }
来源：http://bad.daxiang520.top

[T51] Scala：Hello World
来源：http://xhx.havefunace.top

println("Hello")
来源：http://the.yanxiufei.cn

[T52] Scala：变量
来源：http://uti.hongshengwenyu.top

val a = 1;  var b = 2
来源：http://avc.daxiang520.top

[T53] Scala：字符串插值
来源：http://agh.c1oappe.top

s"值: $b"
来源：http://pzz.zhiwuduotai.top

[T54] Scala：集合映射
来源：http://ogx.tarul.cn

List(1, 2, 3).map(_ * 2)
来源：http://get.havefunace.top

[T55] Scala：集合过滤
来源：http://jax.chenzaomai.com

List(1, 2, 3).filter(_ > 1)
来源：http://spb.haohaochexian.top

[T56] Scala：样例类
来源：http://uyp.daria6918.cn

case class User(name: String, age: Int)
来源：http://fou.sjlbkw.cn

[T57] Scala：模式匹配
来源：http://omx.jinqigufen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vff.ehwqpu.com

[T58] Scala：函数定义
来源：http://nzb.xylfe.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cqy.chenjidiqi.icu

[T59] Scala：循环
来源：http://ola.wangshuangyany.cn

for (i <- 1 to 10) println(i)
来源：http://ezt.zhoulong.xyz

[T60] Scala：折叠
来源：http://lma.sweek.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sgj.guannengcc.top

================================================================================
来源：http://hrr.aizwys.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zxs.tian-w.cn

================================================================================
来源：http://rie.jinqigfzy.top

[U01] Py：创建虚拟环境
来源：http://men.yuxming.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mgp.xuanzx.com

[U02] Py：导出 / 安装依赖
来源：http://tiv.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ngh.shanyushiyangkeji.top

[U03] Py：加载 .env 配置
来源：http://vaw.zdqjudy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mok.zhijiandao.cn

[U04] Py：变量调试打印
来源：http://pky.jinqigfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ozy.epnwcf.com

[U05] Py：列表去重且保序
来源：http://sgw.zhixingplan.top

list(dict.fromkeys(arr))
来源：http://ebk.tianlin.xyz

[U06] Py：合并两个字典
来源：http://pqa.chenjidiqi.icu

{**a, **b}
来源：http://szj.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://svo.316326.xyz

{v: k for k, v in d.items()}
来源：http://jkn.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://lbu.tian-w.cn

[y for x in nested for y in x]
来源：http://qra.yj20258888.top

[U09] Py：字典取最大值的键
来源：http://ufh.sufxvd.cn

max(d, key=d.get)
来源：http://nxq.hfpthk.cn

[U10] Py：按值排序字典
来源：http://tba.yanxiufei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nhq.uphjek.com

[U11] Py：生成器表达式
来源：http://egs.zhiwuduotai.top

(x * 2 for x in arr)
来源：http://puz.fehbvm.com

[U12] Py：取出现最多的 3 个元素
来源：http://wis.nwbrower.top

Counter(arr).most_common(3)
来源：http://tbi.ivvv.top

[U13] Py：固定长度队列
来源：http://kzg.jyoumei.cn

deque(maxlen=10)
来源：http://yuv.guowangkeji.top

[U14] Py：分组收集到列表
来源：http://vqh.ydzc1.top

defaultdict(list)
来源：http://qho.ivvv.top

[U15] Py：高精度计时
来源：http://pxt.sufxvd.cn

t = time.perf_counter()
来源：http://mca.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://vld.hnqzz.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xag.shanyushiyangtech.top

[U17] Py：初始化日志
来源：http://ghl.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://qyr.jinqigufen.top

[U18] Py：预编译正则
来源：http://qba.jianghu66.top

pat = re.compile(r"\d+")
来源：http://dyv.fzhhl.top

[U19] Py：正则替换带回调
来源：http://hvh.zhoulong.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uge.pycfn.com

[U20] Py：缓存函数结果
来源：http://hdf.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://ede.yangfankeji.com

[U21] Py：自定义上下文管理器
来源：http://jwl.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://rbg.sjlbkw.cn

[U22] Py：矩阵转置
来源：http://tut.guowangkeji.top

list(zip(*m))
来源：http://cgj.jiagoushi.top

[U23] Py：分块读取大文件
来源：http://ufl.bjfxy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://weu.nanxuanxn.top

[U24] Py：路径操作
来源：http://hxw.hammf.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hlx.epnwcf.com

[U25] Py：CSV 按字典读
来源：http://umo.zhaomingkeji.xyz

csv.DictReader(f)
来源：http://yiv.uphjek.com

[U26] Py：并发下载
来源：http://cqy.tarul.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jeb.zdbjq.cn

[U27] Py：异步 HTTP
来源：http://zgr.yfazqb.com

aiohttp.ClientSession() 配合 async with
来源：http://qrs.cashguo.top

[U28] Py：类型别名
来源：http://gcb.yuanzhike.top

UserId = int
来源：http://bfm.chenlongwang.top

[U29] Py：属性校验
来源：http://pdr.vehdjk.com

@property 与 @x.setter 配合
来源：http://nhp.ydjk.org.cn

[U30] Py：数据类
来源：http://lsj.fktsv.cn

@dataclass(slots=True)
来源：http://brw.0kj1m.cn

[U31] Py：单测
来源：http://tab.ybcxt.top

python -m pytest -q
来源：http://xmf.xuetiantiany.cn

[U32] Py：代码格式化
来源：http://dhb.fengsongda.top

ruff format . && ruff check --fix .
来源：http://jmu.hongshengwenyu.top

[U33] Py：打包发布
来源：http://rrk.smart0.xyz

python -m build  （依赖 pyproject.toml）
来源：http://dmu.jlsjyb.cn

[U34] Py：判断编码
来源：http://xbx.hcnkem.com

chardet.detect(raw)
来源：http://lmf.ywan-chungtsiang.top

[U35] Py：发送邮件
来源：http://cli.jyoumei.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hik.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://mmj.kuanghao11.cn

schedule.every(10).minutes.do(job)
来源：http://kxc.bjfxy.top

[U37] Py：读写 Excel
来源：http://kym.zhiwuduotai.top

pandas.read_excel / DataFrame.to_excel
来源：http://ccx.shangyingyoupin.top

[U38] Py：获取脚本所在目录
来源：http://vyw.yfazqb.com

Path(__file__).resolve().parent
来源：http://cko.sysykeji.top

[U39] Py：判断是否在交互环境
来源：http://rgl.cashguo.top

sys.stdout.isatty()
来源：http://owt.xingfuxueyuan.xyz

[U40] Py：打印到标准错误
来源：http://zny.birdmap.top

print("err", file=sys.stderr)
来源：http://adz.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://hnk.dashuyun.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nuu.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://bma.yj202588.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://znh.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://mzx.tian-w.cn

namespace App\Http;
来源：http://epw.yfazqb.com

[U44] PHP：开启严格类型
来源：http://udo.cheryme.top

declare(strict_types=1);
来源：http://asu.jiagoushi.top

[U45] PHP：类型声明与返回类型
来源：http://idh.hnqzz.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://itc.yangfankeji.com

[U46] PHP：可空类型
来源：http://vzw.gaohongyu789.top

?string $name = null
来源：http://bqf.hcnkem.com

[U47] PHP：联合类型
来源：http://zno.xinyue.icu

int|string $id
来源：http://bgr.zhiwuduotai.top

[U48] PHP：纯枚举
来源：http://wib.yuanzhike.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gml.cdnleiting.top

[U49] PHP：只读属性
来源：http://gad.jyoumei.cn

public readonly string $name
来源：http://vwa.zdbjq.cn

[U50] PHP：构造器属性提升
来源：http://ekw.jianghu66.top

public function __construct(private int $id) {}
来源：http://pfm.sxryk.cn

[U51] PHP：数组解构
来源：http://rqe.aibaodan.cn

[$a, $b] = $arr;
来源：http://gyj.cashguo.top

[U52] PHP：箭头函数
来源：http://shi.fehbvm.com

$double = fn($x) => $x * 2;
来源：http://fmf.birdmap.top

[U53] PHP：空合并运算符
来源：http://vrx.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://ykp.nwbrower.top

[U54] PHP：空安全调用
来源：http://mkh.jianghu66.top

$obj?->method()
来源：http://hdb.xinyue.icu

[U55] PHP：match 表达式
来源：http://vqh.ybcxt.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qio.shanyushiyangtech.top

[U56] PHP：命名参数
来源：http://xet.quarkkingdee.top

f(a: 1, b: 2)
来源：http://hyw.zhiwuduotai.top

[U57] PHP：字符串插值
来源：http://qgt.316326.xyz

"值: {$a}"
来源：http://wab.cheryme.top

[U58] PHP：数组三件套
来源：http://txz.havefunace.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cpg.zdqjudy.top

[U59] PHP：自定义排序
来源：http://qjl.ehwqpu.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ffg.zhaomingkeji.xyz

[U60] PHP：JSON 编解码
来源：http://ipf.hongshengwenyu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yxm.9152youxi.cn

[U61] PHP：正则
来源：http://jck.meibo888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pyz.jyoumei.cn

[U62] PHP：日期对象
来源：http://nvz.iojbl.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uft.havefunace.top

[U63] PHP：文件读写
来源：http://ziv.jyoumei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ncp.mhx1999.top

[U64] PHP：目录遍历
来源：http://sza.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://rbe.dashuyun.cn

[U65] PHP：会话
来源：http://zbu.jyoumei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uzs.shangyingyoupin.top

[U66] PHP：设置 Cookie
来源：http://yvq.hywenlv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ebr.daxiang520.top

[U67] PHP：处理文件上传
来源：http://opy.kuanghao11.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xny.gogol.net.cn

[U68] PHP：PDO 连接
来源：http://hzy.ivvv.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://por.jinghuilouyu.cn

[U69] PHP：PDO 预处理
来源：http://tma.uphjek.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vff.zhiwuduotai.top

[U70] PHP：PDO 事务
来源：http://che.feifeiyinyue.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sjb.316326.xyz

[U71] PHP：抛出异常
来源：http://tou.quarkkingdee.top

throw new RuntimeException("失败", 500);
来源：http://gfn.xziqi.cn

[U72] PHP：写错误日志
来源：http://ejo.yj202588.top

error_log("失败: " . $e->getMessage());
来源：http://nqv.guowangkeji.top

[U73] PHP：读取 ini 配置
来源：http://kft.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://wus.shzxlz.cn

[U74] PHP：读取环境变量
来源：http://zjq.daxiang520.top

getenv("APP_ENV") ?: "production"
来源：http://uyb.sufxvd.cn

[U75] PHP：依赖注入
来源：http://slb.xylfe.cn

composer require psr/container
来源：http://ofc.dashuyun.cn

[U76] PHP：简单路由
来源：http://uoo.zhoulong.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vmx.tarul.cn

[U77] PHP：模板渲染
来源：http://kon.pengpengdd.cyou

composer require twig/twig
来源：http://ilm.zhixingplan.top

[U78] PHP：单元测试
来源：http://jgh.chenlongwang.top

composer require --dev phpunit/phpunit
来源：http://tdt.ywan-chungtsiang.top

[U79] PHP：静态分析
来源：http://mfn.yangfankeji.com

composer require --dev phpstan/phpstan
来源：http://wxm.quarkkingdee.top

[U80] PHP：代码规范修复
来源：http://iho.cdnleiting.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://azc.zhoulong.xyz

[U81] JS：初始化项目
来源：http://dyf.316326.xyz

npm init -y;  npm i express
来源：http://mge.cdnleiting.top

[U82] JS：package.json 脚本
来源：http://ypn.jianghu66.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://guf.yanxiufei.cn

[U83] JS：ES Module 导入导出
来源：http://fwa.yangfankeji.com

export const a = 1;  import { a } from "./m.js";
来源：http://tnx.jlsjyb.cn

[U84] JS：CommonJS 写法
来源：http://ohq.gogol.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bhw.ybcxt.top

[U85] JS：可选链
来源：http://fpm.havefunace.top

a?.b?.c
来源：http://mmw.nanxuanxn.top

[U86] JS：空值合并
来源：http://iqg.jinqigfzy.top

a ?? b
来源：http://dcu.wangdashe.top

[U87] JS：解构默认值
来源：http://rsc.haohaochexian.top

const { a = 1, b = 2 } = obj;
来源：http://ztt.hnxiangtu.top

[U88] JS：对象展开合并
来源：http://kxj.nanxinkj.top

{ ...a, ...b }
来源：http://kwm.daria6918.cn

[U89] JS：数组去重
来源：http://bvv.sxryk.cn

[...new Set(arr)]
来源：http://csl.haohaochexian.top

[U90] JS：数字数组排序
来源：http://tyy.fzhhl.top

[...arr].sort((a, b) => a - b)
来源：http://vhw.snrcjt.cn

[U91] JS：对象键值遍历
来源：http://vyr.smart0.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dnt.pycfn.com

[U92] JS：深拷贝
来源：http://zqt.ivvv.top

structuredClone(obj)
来源：http://mbu.yuxming.cn

[U93] JS：模板字符串
来源：http://cwd.gaohongyu789.top

`共 ${n} 条`
来源：http://ooe.aizwys.cn

[U94] JS：箭头函数
来源：http://fxd.tianlin.xyz

const double = x => x * 2;
来源：http://uqk.jinqigufen.top

[U95] JS：Promise 包装
来源：http://ysp.bbcook.cn

new Promise((resolve, reject) => {})
来源：http://pbu.ydjk.org.cn

[U96] JS：async/await 与异常
来源：http://xrt.mhx1999.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bql.hnxiangtu.top

[U97] JS：并发请求
来源：http://pmf.fanxiaobao.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://fhr.chenjidiqi.icu

[U98] JS：fetch 带 JSON
来源：http://mwn.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rcl.xuanzx.com

[U99] JS：事件监听
来源：http://yzb.shanyushiyangkeji.top

el.addEventListener("click", e => {})
来源：http://mxx.pengpengdd.cyou

[U100] JS：DOM 查询
来源：http://zva.redwolf501.top

document.querySelector(".item")
来源：http://exc.havefunace.top

[U101] JS：classList 操作
来源：http://zss.fehbvm.com

el.classList.toggle("active")
来源：http://fin.fehbvm.com

[U102] JS：本地存储
来源：http://rnl.ppjwa.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qbr.jiagoushi.top

[U103] JS：定时器
来源：http://lwz.daxiang520.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ivl.yongpay.top

[U104] JS：防抖
来源：http://luj.jiagoushi.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lkt.bbcook.cn

[U105] JS：节流
来源：http://xru.chenlongwang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xbo.uphjek.com

[U106] JS：日期格式化
来源：http://aqq.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yqe.yj20258.top

[U107] JS：数字千分位
来源：http://cdo.fengsongda.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ncf.316326.xyz

[U108] JS：随机整数
来源：http://vps.iojbl.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dma.shuidangran.top

[U109] JS：数组分组
来源：http://caf.tanke756.top

Object.groupBy(arr, x => x.type)
来源：http://whe.aibaodan.cn

[U110] JS：数组分块
来源：http://pjw.jiagoushi.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ijc.hfpthk.cn


<!-- 参考信息 -->