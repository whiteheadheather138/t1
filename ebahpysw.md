代发 wailian999

[T23] Swift：函数
来源：http://kce.xziqi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rfy.cqqwz.cn

[T24] Swift：闭包
来源：http://xqn.zhiwuduotai.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://soh.aizwys.cn

[T25] Swift：结构体
来源：http://nao.havefunace.top

struct P { var x: Int }
来源：http://rsm.fehbvm.com

[T26] Swift：类与重写
来源：http://byt.yangfankeji.com

class A: Base { override func f() {} }
来源：http://rew.vqdsnc.cn

[T27] Swift：错误处理
来源：http://dlh.yangfankeji.com

do { try f() } catch { print(error) }
来源：http://gfe.shzxlz.cn

[T28] Swift：枚举
来源：http://xnd.zdqjudy.top

enum Color { case red, green }
来源：http://eok.ywan-chungtsiang.top

[T29] Swift：guard 提前返回
来源：http://gum.yj20258.top

guard let x = opt else { return }
来源：http://avv.zhoulong.xyz

[T30] Swift：协议
来源：http://poy.meibo888.top

protocol Shape { func area() -> Double }
来源：http://yxb.yj202588.top

[T31] Lua：Hello World
来源：http://iss.xylfe.cn

print("Hello")
来源：http://wya.tianlin.xyz

[T32] Lua：局部变量
来源：http://hbe.ybcxt.top

local a = 1
来源：http://wka.yvedp.cn

[T33] Lua：表（数组）
来源：http://jpy.jqgufenzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wli.c1oappe.top

[T34] Lua：遍历表
来源：http://sgi.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ate.tianlin.xyz

[T35] Lua：字典表
来源：http://jcn.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://uzk.shanyushiyangtech.top

[T36] Lua：函数
来源：http://pta.nanxuanxn.top

function add(a, b) return a + b end
来源：http://too.yuxming.cn

[T37] Lua：字符串拼接
来源：http://ryh.jinyuanbaomall.cn

"a" .. "b"
来源：http://ump.jinqigfzy.top

[T38] Lua：条件
来源：http://sca.yj202588.top

if x > 0 then print("正") end
来源：http://vjy.havefunace.top

[T39] Lua：模式匹配
来源：http://sft.cqqwz.cn

string.find(s, "%d+")
来源：http://jcx.jqgufenzy.top

[T40] Lua：元表
来源：http://fjl.tarul.cn

setmetatable({}, { __index = base })
来源：http://bsp.yfazqb.com

[T41] Perl：Hello World
来源：http://dlw.zdbjq.cn

print "Hello\n";
来源：http://vqy.dashuyun.cn

[T42] Perl：变量类型
来源：http://oye.jinqigufen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hdo.hnxiangtu.top

[T43] Perl：字符串插值
来源：http://yob.cheryme.top

"值: $a"
来源：http://odh.xylfe.cn

[T44] Perl：条件
来源：http://jjt.tanke756.top

if ($a > 0) { print "正"; }
来源：http://pkd.jinqigfzy.top

[T45] Perl：数组遍历
来源：http://zvx.zhixingplan.top

for my $x (@arr) { print $x; }
来源：http://wdg.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://csz.snrcjt.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mri.cqqwz.cn

[T47] Perl：正则捕获
来源：http://rgy.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://xve.sysykeji.top

[T48] Perl：正则替换
来源：http://ter.bbcook.cn

$s =~ s/old/new/g;
来源：http://jew.vqdsnc.cn

[T49] Perl：函数
来源：http://ukq.sxryk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://esh.uphjek.com

[T50] Perl：逐行读文件
来源：http://uok.guowangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lto.jinghuilouyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://thw.jianghu66.top

[T51] Scala：Hello World
来源：http://vda.ydzc1.top

println("Hello")
来源：http://yvw.zhaomingkeji.xyz

[T52] Scala：变量
来源：http://vld.cucudq.cn

val a = 1;  var b = 2
来源：http://ntv.jyoumei.cn

[T53] Scala：字符串插值
来源：http://xpj.hnqzz.top

s"值: $b"
来源：http://vae.fengsongda.top

[T54] Scala：集合映射
来源：http://lfy.feifeiyinyue.top

List(1, 2, 3).map(_ * 2)
来源：http://cph.gaohongyu789.top

[T55] Scala：集合过滤
来源：http://cbz.mhx1999.top

List(1, 2, 3).filter(_ > 1)
来源：http://osw.mhx1999.top

[T56] Scala：样例类
来源：http://twy.9152youxi.cn

case class User(name: String, age: Int)
来源：http://qdh.meibo888.top

[T57] Scala：模式匹配
来源：http://xej.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xen.sweek.top

[T58] Scala：函数定义
来源：http://btb.gaohongyu789.top

def add(a: Int, b: Int): Int = a + b
来源：http://azp.zhengqikj.top

[T59] Scala：循环
来源：http://njr.tianlin.xyz

for (i <- 1 to 10) println(i)
来源：http://oir.hfpthk.cn

[T60] Scala：折叠
来源：http://xji.aibaodan.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hvt.fzhhl.top

================================================================================
来源：http://gzg.meibo888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jnw.xingfuxueyuan.xyz

================================================================================
来源：http://cec.hnxiangtu.top

[U01] Py：创建虚拟环境
来源：http://wkq.yj20258888.top

python -m venv .venv && source .venv/bin/activate
来源：http://aaf.jiagoushi.top

[U02] Py：导出 / 安装依赖
来源：http://upj.yuanzhike.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://faz.kuanghao11.cn

[U03] Py：加载 .env 配置
来源：http://qjk.wangshuangyany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://twt.ppjwa.cn

[U04] Py：变量调试打印
来源：http://fyl.nwbrower.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uas.yvedp.cn

[U05] Py：列表去重且保序
来源：http://hck.meibo888.top

list(dict.fromkeys(arr))
来源：http://bjg.zhixingplan.top

[U06] Py：合并两个字典
来源：http://cuf.wangshuangyany.cn

{**a, **b}
来源：http://lid.guowangkeji.top

[U07] Py：反转字典键值
来源：http://dho.yonumen.top

{v: k for k, v in d.items()}
来源：http://jgq.tanke756.top

[U08] Py：展平二维列表
来源：http://wgh.fzhhl.top

[y for x in nested for y in x]
来源：http://yin.chenjidiqi.icu

[U09] Py：字典取最大值的键
来源：http://yeq.fanxiaobao.xyz

max(d, key=d.get)
来源：http://eni.yuanzhike.top

[U10] Py：按值排序字典
来源：http://lhl.hywenlv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tmy.yangfankeji.com

[U11] Py：生成器表达式
来源：http://sxt.ppjwa.cn

(x * 2 for x in arr)
来源：http://txv.yanxiufei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tfi.cqqwz.cn

Counter(arr).most_common(3)
来源：http://uwg.ywan-chungtsiang.top

[U13] Py：固定长度队列
来源：http://rtu.fzhhl.top

deque(maxlen=10)
来源：http://tfp.yvedp.cn

[U14] Py：分组收集到列表
来源：http://syi.fzhhl.top

defaultdict(list)
来源：http://whd.zhoulong.xyz

[U15] Py：高精度计时
来源：http://emz.dashuyun.cn

t = time.perf_counter()
来源：http://qbz.cqqwz.cn

[U16] Py：命令行参数解析
来源：http://vbk.daxiang520.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xow.cqqwz.cn

[U17] Py：初始化日志
来源：http://uda.ivvv.top

logging.basicConfig(level=logging.INFO)
来源：http://wfh.jiagoushi.top

[U18] Py：预编译正则
来源：http://wnk.xziqi.cn

pat = re.compile(r"\d+")
来源：http://hsc.jlsjyb.cn

[U19] Py：正则替换带回调
来源：http://enb.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kwp.hywenlv.cn

[U20] Py：缓存函数结果
来源：http://nal.cheryme.top

@functools.lru_cache(maxsize=None)
来源：http://sfd.cdnleiting.top

[U21] Py：自定义上下文管理器
来源：http://hyd.hammf.cn

@contextlib.contextmanager
来源：http://buo.meibo888.top

[U22] Py：矩阵转置
来源：http://bvk.vehdjk.com

list(zip(*m))
来源：http://dvj.52xcode.cn

[U23] Py：分块读取大文件
来源：http://cdo.gotoacloud.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rio.wangshuangyany.cn

[U24] Py：路径操作
来源：http://btl.aizwys.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://utk.jianghu66.top

[U25] Py：CSV 按字典读
来源：http://ozz.yfazqb.com

csv.DictReader(f)
来源：http://epa.shangyingyoupin.top

[U26] Py：并发下载
来源：http://fmt.zhoulong.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pxx.meibo888.top

[U27] Py：异步 HTTP
来源：http://muu.ehwqpu.com

aiohttp.ClientSession() 配合 async with
来源：http://fpq.andypj.xyz

[U28] Py：类型别名
来源：http://jxx.vqdsnc.cn

UserId = int
来源：http://ttr.zhoulong.xyz

[U29] Py：属性校验
来源：http://efa.haohaochexian.top

@property 与 @x.setter 配合
来源：http://oar.bjfxy.top

[U30] Py：数据类
来源：http://fhi.c1oappe.top

@dataclass(slots=True)
来源：http://mgg.jinghuilouyu.cn

[U31] Py：单测
来源：http://jng.zycfv.cn

python -m pytest -q
来源：http://tyv.shuidangran.top

[U32] Py：代码格式化
来源：http://ezs.sysykeji.top

ruff format . && ruff check --fix .
来源：http://hbl.shanyushiyangkeji.top

[U33] Py：打包发布
来源：http://bpy.yueranfly.top

python -m build  （依赖 pyproject.toml）
来源：http://nws.gotoacloud.top

[U34] Py：判断编码
来源：http://uyj.tianlin.xyz

chardet.detect(raw)
来源：http://doj.aibaodan.cn

[U35] Py：发送邮件
来源：http://lxg.zhijiandao.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://byz.jiagoushi.top

[U36] Py：定时任务
来源：http://dlj.mhx1999.top

schedule.every(10).minutes.do(job)
来源：http://edn.pengpengdd.cyou

[U37] Py：读写 Excel
来源：http://ing.tanke756.top

pandas.read_excel / DataFrame.to_excel
来源：http://dkj.daria6918.cn

[U38] Py：获取脚本所在目录
来源：http://prw.nwbrower.top

Path(__file__).resolve().parent
来源：http://ffm.zycfv.cn

[U39] Py：判断是否在交互环境
来源：http://gyb.ehwqpu.com

sys.stdout.isatty()
来源：http://oxk.jyoumei.cn

[U40] Py：打印到标准错误
来源：http://bwb.hfpthk.cn

print("err", file=sys.stderr)
来源：http://ctp.vqdsnc.cn

[U41] PHP：初始化 Composer 项目
来源：http://obu.gotoacloud.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ooo.yonumen.top

[U42] PHP：PSR-4 自动加载
来源：http://blq.xylfe.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xum.aizwys.cn

[U43] PHP：声明命名空间
来源：http://hkd.haohaochexian.top

namespace App\Http;
来源：http://kph.nanxinkj.top

[U44] PHP：开启严格类型
来源：http://pea.gaohongyu789.top

declare(strict_types=1);
来源：http://oze.shuidangran.top

[U45] PHP：类型声明与返回类型
来源：http://lzh.pycfn.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://wqt.yj20258.top

[U46] PHP：可空类型
来源：http://oct.jianghu66.top

?string $name = null
来源：http://mnm.hnxiangtu.top

[U47] PHP：联合类型
来源：http://dhx.sjlbkw.cn

int|string $id
来源：http://lld.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://fsv.ywan-chungtsiang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yqf.sweek.top

[U49] PHP：只读属性
来源：http://kmi.gaohongyu789.top

public readonly string $name
来源：http://euh.zhixingplan.top

[U50] PHP：构造器属性提升
来源：http://qst.0kj1m.cn

public function __construct(private int $id) {}
来源：http://gxb.iojbl.cn

[U51] PHP：数组解构
来源：http://zse.sweek.top

[$a, $b] = $arr;
来源：http://ozh.tian-w.cn

[U52] PHP：箭头函数
来源：http://eom.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://yqx.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://lnn.ivvv.top

$v = $a ?? $b ?? "default";
来源：http://oax.andypj.xyz

[U54] PHP：空安全调用
来源：http://dgh.daxiang520.top

$obj?->method()
来源：http://fed.xuanzx.com

[U55] PHP：match 表达式
来源：http://pkw.uphjek.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gtd.tianlin.xyz

[U56] PHP：命名参数
来源：http://grh.0kj1m.cn

f(a: 1, b: 2)
来源：http://exb.jianghu66.top

[U57] PHP：字符串插值
来源：http://yox.cqqwz.cn

"值: {$a}"
来源：http://qmr.zhixingplan.top

[U58] PHP：数组三件套
来源：http://dks.pycfn.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rdy.zhaomingkeji.xyz

[U59] PHP：自定义排序
来源：http://lhi.hfpthk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vnm.zhixingplan.top

[U60] PHP：JSON 编解码
来源：http://vet.tian-w.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cvj.sysykeji.top

[U61] PHP：正则
来源：http://wnq.ctjpmb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qzs.yuanzhike.top

[U62] PHP：日期对象
来源：http://xam.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://phn.yongpay.top

[U63] PHP：文件读写
来源：http://umn.zhengqikj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xuj.smart0.xyz

[U64] PHP：目录遍历
来源：http://lmg.yfazqb.com

glob("dir/*.php");  scandir("dir");
来源：http://whs.bbcook.cn

[U65] PHP：会话
来源：http://nig.yonumen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://cns.gaohongyu789.top

[U66] PHP：设置 Cookie
来源：http://lqh.yonumen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lmc.quarkkingdee.top

[U67] PHP：处理文件上传
来源：http://rnb.daria6918.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://egj.zhiwuduotai.top

[U68] PHP：PDO 连接
来源：http://cqh.fanxiaobao.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://smo.jinqigufen.top

[U69] PHP：PDO 预处理
来源：http://ron.chenjidiqi.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rgh.cqqwz.cn

[U70] PHP：PDO 事务
来源：http://huq.shanyushiyangtech.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kxr.hfpthk.cn

[U71] PHP：抛出异常
来源：http://frj.zhoulong.xyz

throw new RuntimeException("失败", 500);
来源：http://rnc.zhijiandao.cn

[U72] PHP：写错误日志
来源：http://odm.zycfv.cn

error_log("失败: " . $e->getMessage());
来源：http://ytn.wangdashe.top

[U73] PHP：读取 ini 配置
来源：http://csd.jinqigfzy.top

parse_ini_file("config.ini", true)
来源：http://brv.nwbrower.top

[U74] PHP：读取环境变量
来源：http://mqm.hywenlv.cn

getenv("APP_ENV") ?: "production"
来源：http://qli.fehbvm.com

[U75] PHP：依赖注入
来源：http://dul.xinyue.icu

composer require psr/container
来源：http://eqb.sufxvd.cn

[U76] PHP：简单路由
来源：http://gaa.xinyue.icu

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://owf.aibaodan.cn

[U77] PHP：模板渲染
来源：http://ppl.yj20258.top

composer require twig/twig
来源：http://exd.ydjk.org.cn

[U78] PHP：单元测试
来源：http://gqq.gogol.net.cn

composer require --dev phpunit/phpunit
来源：http://lwk.jqgfzy.top

[U79] PHP：静态分析
来源：http://rul.jinyuanbaomall.cn

composer require --dev phpstan/phpstan
来源：http://bwp.iojbl.cn

[U80] PHP：代码规范修复
来源：http://ncc.hongshengwenyu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tps.52xcode.cn

[U81] JS：初始化项目
来源：http://qvd.yvedp.cn

npm init -y;  npm i express
来源：http://low.cdnleiting.top

[U82] JS：package.json 脚本
来源：http://gqn.chenjidiqi.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xoz.aibaodan.cn

[U83] JS：ES Module 导入导出
来源：http://ehs.316326.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://jiy.chenzaomai.com

[U84] JS：CommonJS 写法
来源：http://opy.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nka.zhijiandao.cn

[U85] JS：可选链
来源：http://pbb.birdmap.top

a?.b?.c
来源：http://ecu.wangshuangyany.cn

[U86] JS：空值合并
来源：http://dvk.zhaomingkeji.xyz

a ?? b
来源：http://qvq.aizwys.cn

[U87] JS：解构默认值
来源：http://mgd.jinghuilouyu.cn

const { a = 1, b = 2 } = obj;
来源：http://fcg.hongshengwenyu.top

[U88] JS：对象展开合并
来源：http://njj.chenjidiqi.icu

{ ...a, ...b }
来源：http://rtv.epnwcf.com

[U89] JS：数组去重
来源：http://chu.gaohongyu789.top

[...new Set(arr)]
来源：http://giq.haohaochexian.top

[U90] JS：数字数组排序
来源：http://yfi.guowangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://ffx.jqgfzy.top

[U91] JS：对象键值遍历
来源：http://kag.yvedp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rzk.zhengqikj.top

[U92] JS：深拷贝
来源：http://xob.quarkkingdee.top

structuredClone(obj)
来源：http://tji.wangdashe.top

[U93] JS：模板字符串
来源：http://xjr.yonumen.top

`共 ${n} 条`
来源：http://gwc.haohaochexian.top

[U94] JS：箭头函数
来源：http://seo.sxryk.cn

const double = x => x * 2;
来源：http://kfm.zhijiandao.cn

[U95] JS：Promise 包装
来源：http://uta.haohaochexian.top

new Promise((resolve, reject) => {})
来源：http://zdp.zhiwuduotai.top

[U96] JS：async/await 与异常
来源：http://gnj.jinghuilouyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nos.haohaochexian.top

[U97] JS：并发请求
来源：http://xpw.daria6918.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uga.yongpay.top

[U98] JS：fetch 带 JSON
来源：http://nsf.daria6918.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hbq.gogol.net.cn

[U99] JS：事件监听
来源：http://cot.xinyue.icu

el.addEventListener("click", e => {})
来源：http://ckf.tian-w.cn

[U100] JS：DOM 查询
来源：http://kyh.zhengqikj.top

document.querySelector(".item")
来源：http://gsa.yuanzhike.top

[U101] JS：classList 操作
来源：http://vct.iojbl.cn

el.classList.toggle("active")
来源：http://ygd.yonumen.top

[U102] JS：本地存储
来源：http://chk.snrcjt.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://myu.vehdjk.com

[U103] JS：定时器
来源：http://mve.hesvh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pku.nanxuanxn.top

[U104] JS：防抖
来源：http://uea.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qhz.zhongyouzk.top

[U105] JS：节流
来源：http://bgr.hesvh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://epn.hesvh.cn

[U106] JS：日期格式化
来源：http://jfe.yuanzhike.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yst.birdmap.top

[U107] JS：数字千分位
来源：http://mte.zhengqikj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rqs.yueranfly.top

[U108] JS：随机整数
来源：http://wje.shanyushiyangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://diq.ehwqpu.com

[U109] JS：数组分组
来源：http://azh.vehdjk.com

Object.groupBy(arr, x => x.type)
来源：http://uae.quarkkingdee.top

[U110] JS：数组分块
来源：http://vrz.jqgfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://msh.guowangkeji.top


<!-- 参考信息 -->