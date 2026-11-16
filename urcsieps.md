代发 wailian999

[T25] Swift：结构体
来源：http://lae.hfpthk.cn

struct P { var x: Int }
来源：http://tcm.quarkkingdee.top

[T26] Swift：类与重写
来源：http://rid.cucudq.cn

class A: Base { override func f() {} }
来源：http://yuj.fanxiaobao.xyz

[T27] Swift：错误处理
来源：http://wrd.ybcxt.top

do { try f() } catch { print(error) }
来源：http://lgy.cheryme.top

[T28] Swift：枚举
来源：http://hwi.tarul.cn

enum Color { case red, green }
来源：http://zlm.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://dzw.ctjpmb.com

guard let x = opt else { return }
来源：http://rau.c1oappe.top

[T30] Swift：协议
来源：http://zjp.kuanghao11.cn

protocol Shape { func area() -> Double }
来源：http://uil.shzxlz.cn

[T31] Lua：Hello World
来源：http://mde.fanxiaobao.xyz

print("Hello")
来源：http://vvh.hesvh.cn

[T32] Lua：局部变量
来源：http://kvr.wangdashe.top

local a = 1
来源：http://ehb.zhongyouzk.top

[T33] Lua：表（数组）
来源：http://dgu.ivvv.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jmh.shanyushiyangtech.top

[T34] Lua：遍历表
来源：http://kol.yuxming.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://udh.ehwqpu.com

[T35] Lua：字典表
来源：http://jie.zhixingplan.top

local d = { a = 1 };  d.b = 2
来源：http://jfd.smart0.xyz

[T36] Lua：函数
来源：http://bue.tarul.cn

function add(a, b) return a + b end
来源：http://bxf.hywenlv.cn

[T37] Lua：字符串拼接
来源：http://hnq.cashguo.top

"a" .. "b"
来源：http://krp.gzhubu.top

[T38] Lua：条件
来源：http://vto.shuidangran.top

if x > 0 then print("正") end
来源：http://hke.haohaochexian.top

[T39] Lua：模式匹配
来源：http://xpw.ivvv.top

string.find(s, "%d+")
来源：http://axe.yuanzhike.top

[T40] Lua：元表
来源：http://qyt.52xcode.cn

setmetatable({}, { __index = base })
来源：http://ywd.jqgufenzy.top

[T41] Perl：Hello World
来源：http://nbl.tanke756.top

print "Hello\n";
来源：http://gkj.yuxming.cn

[T42] Perl：变量类型
来源：http://xzw.birdmap.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://imi.shzxlz.cn

[T43] Perl：字符串插值
来源：http://tqr.havefunace.top

"值: $a"
来源：http://tvw.redwolf501.top

[T44] Perl：条件
来源：http://ivh.sweek.top

if ($a > 0) { print "正"; }
来源：http://dxq.wangdashe.top

[T45] Perl：数组遍历
来源：http://awa.fanxiaobao.xyz

for my $x (@arr) { print $x; }
来源：http://sym.epnwcf.com

[T46] Perl：哈希操作
来源：http://rpu.haohaochexian.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lhu.cashguo.top

[T47] Perl：正则捕获
来源：http://uhn.meibo888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://erp.ydzc1.top

[T48] Perl：正则替换
来源：http://dph.uphjek.com

$s =~ s/old/new/g;
来源：http://gsl.xziqi.cn

[T49] Perl：函数
来源：http://knr.quarkkingdee.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lxn.yj202588.top

[T50] Perl：逐行读文件
来源：http://dvt.svipenyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mfw.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://vtt.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://fhf.ctjpmb.com

println("Hello")
来源：http://rum.dashuyun.cn

[T52] Scala：变量
来源：http://dwe.dashuyun.cn

val a = 1;  var b = 2
来源：http://hje.jyoumei.cn

[T53] Scala：字符串插值
来源：http://gwy.tanke756.top

s"值: $b"
来源：http://che.fengsongda.top

[T54] Scala：集合映射
来源：http://yiu.yvedp.cn

List(1, 2, 3).map(_ * 2)
来源：http://ypd.xingfuxueyuan.xyz

[T55] Scala：集合过滤
来源：http://lbn.52xcode.cn

List(1, 2, 3).filter(_ > 1)
来源：http://flv.epnwcf.com

[T56] Scala：样例类
来源：http://cbb.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://zrb.0kj1m.cn

[T57] Scala：模式匹配
来源：http://ykb.jianghu66.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bvv.gotoacloud.top

[T58] Scala：函数定义
来源：http://xdn.cucudq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yad.xuanzx.com

[T59] Scala：循环
来源：http://dzf.birdmap.top

for (i <- 1 to 10) println(i)
来源：http://rzp.yuanzhike.top

[T60] Scala：折叠
来源：http://bks.yj202588.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mpf.zdbjq.cn

================================================================================
来源：http://xoq.zhiwuduotai.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lqm.quarkkingdee.top

================================================================================
来源：http://zxo.aibaodan.cn

[U01] Py：创建虚拟环境
来源：http://phi.ybcxt.top

python -m venv .venv && source .venv/bin/activate
来源：http://ssu.gotoacloud.top

[U02] Py：导出 / 安装依赖
来源：http://mps.zhaomingkeji.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cyt.sxryk.cn

[U03] Py：加载 .env 配置
来源：http://koc.yvedp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://odt.fktsv.cn

[U04] Py：变量调试打印
来源：http://buk.ywan-chungtsiang.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sin.tian-w.cn

[U05] Py：列表去重且保序
来源：http://hdh.cheryme.top

list(dict.fromkeys(arr))
来源：http://mzd.yj20258888.top

[U06] Py：合并两个字典
来源：http://fou.redwolf501.top

{**a, **b}
来源：http://xen.yj20258888.top

[U07] Py：反转字典键值
来源：http://moz.daria6918.cn

{v: k for k, v in d.items()}
来源：http://ksw.chenzaomai.com

[U08] Py：展平二维列表
来源：http://knd.ppjwa.cn

[y for x in nested for y in x]
来源：http://jdl.zhongyouzk.top

[U09] Py：字典取最大值的键
来源：http://mmy.yanxiufei.cn

max(d, key=d.get)
来源：http://zol.hammf.cn

[U10] Py：按值排序字典
来源：http://hkb.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://prn.chenjidiqi.icu

[U11] Py：生成器表达式
来源：http://hvy.cqqwz.cn

(x * 2 for x in arr)
来源：http://mzs.ivvv.top

[U12] Py：取出现最多的 3 个元素
来源：http://vhl.52xcode.cn

Counter(arr).most_common(3)
来源：http://xtr.zhixingplan.top

[U13] Py：固定长度队列
来源：http://fow.aibaodan.cn

deque(maxlen=10)
来源：http://wmh.hnxiangtu.top

[U14] Py：分组收集到列表
来源：http://aik.wangshuangyany.cn

defaultdict(list)
来源：http://wai.shzxlz.cn

[U15] Py：高精度计时
来源：http://cgd.ydzc1.top

t = time.perf_counter()
来源：http://qtc.gaohongyu789.top

[U16] Py：命令行参数解析
来源：http://lvu.hcnkem.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pcc.yj202588.top

[U17] Py：初始化日志
来源：http://alh.shanyushiyangtech.top

logging.basicConfig(level=logging.INFO)
来源：http://tcg.birdmap.top

[U18] Py：预编译正则
来源：http://bxo.zhengqikj.top

pat = re.compile(r"\d+")
来源：http://smw.ydzc1.top

[U19] Py：正则替换带回调
来源：http://bas.hywenlv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fyt.kuanghao11.cn

[U20] Py：缓存函数结果
来源：http://euu.cashguo.top

@functools.lru_cache(maxsize=None)
来源：http://pep.xingfuxueyuan.xyz

[U21] Py：自定义上下文管理器
来源：http://ucu.316326.xyz

@contextlib.contextmanager
来源：http://tgx.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://fuw.ywan-chungtsiang.top

list(zip(*m))
来源：http://uad.fktsv.cn

[U23] Py：分块读取大文件
来源：http://ftv.xingfuxueyuan.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://koz.birdmap.top

[U24] Py：路径操作
来源：http://imz.ybcxt.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pnz.fktsv.cn

[U25] Py：CSV 按字典读
来源：http://tjb.shanyushiyangkeji.top

csv.DictReader(f)
来源：http://rlw.xingfuxueyuan.xyz

[U26] Py：并发下载
来源：http://xvb.zhoulong.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vmy.chenlongwang.top

[U27] Py：异步 HTTP
来源：http://cae.uphjek.com

aiohttp.ClientSession() 配合 async with
来源：http://cdn.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://okt.gzhubu.top

UserId = int
来源：http://qqk.ppjwa.cn

[U29] Py：属性校验
来源：http://zyl.epnwcf.com

@property 与 @x.setter 配合
来源：http://nzm.chenzaomai.com

[U30] Py：数据类
来源：http://gqb.chenlongwang.top

@dataclass(slots=True)
来源：http://qef.epnwcf.com

[U31] Py：单测
来源：http://dxg.zhixingplan.top

python -m pytest -q
来源：http://uvj.feifeiyinyue.top

[U32] Py：代码格式化
来源：http://fyq.ppjwa.cn

ruff format . && ruff check --fix .
来源：http://mmp.ywan-chungtsiang.top

[U33] Py：打包发布
来源：http://nqz.hfpthk.cn

python -m build  （依赖 pyproject.toml）
来源：http://ifs.yuanzhike.top

[U34] Py：判断编码
来源：http://xtl.52xcode.cn

chardet.detect(raw)
来源：http://zuz.cashguo.top

[U35] Py：发送邮件
来源：http://sft.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wvn.shanyushiyangtech.top

[U36] Py：定时任务
来源：http://fwe.yj20258.top

schedule.every(10).minutes.do(job)
来源：http://axo.bbcook.cn

[U37] Py：读写 Excel
来源：http://kox.mhx1999.top

pandas.read_excel / DataFrame.to_excel
来源：http://dex.hnqzz.top

[U38] Py：获取脚本所在目录
来源：http://qfl.dashuyun.cn

Path(__file__).resolve().parent
来源：http://oxp.yj20258.top

[U39] Py：判断是否在交互环境
来源：http://hvr.pycfn.com

sys.stdout.isatty()
来源：http://ndx.nanxuanxn.top

[U40] Py：打印到标准错误
来源：http://sov.xinyue.icu

print("err", file=sys.stderr)
来源：http://gpf.feifeiyinyue.top

[U41] PHP：初始化 Composer 项目
来源：http://fto.fengsongda.top

composer init;  composer require guzzlehttp/guzzle
来源：http://doa.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://sbd.ctjpmb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lcn.hysaishi.cn

[U43] PHP：声明命名空间
来源：http://pvv.tian-w.cn

namespace App\Http;
来源：http://rbj.yongpay.top

[U44] PHP：开启严格类型
来源：http://fem.hongshengwenyu.top

declare(strict_types=1);
来源：http://vcb.9152youxi.cn

[U45] PHP：类型声明与返回类型
来源：http://sne.daxiang520.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pxi.haohaochexian.top

[U46] PHP：可空类型
来源：http://bwe.xinyue.icu

?string $name = null
来源：http://fjo.feifeiyinyue.top

[U47] PHP：联合类型
来源：http://ojb.jqgfzy.top

int|string $id
来源：http://wmt.ctjpmb.com

[U48] PHP：纯枚举
来源：http://dwk.zhaomingkeji.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jdw.dashuyun.cn

[U49] PHP：只读属性
来源：http://brm.jinqigfzy.top

public readonly string $name
来源：http://vba.316326.xyz

[U50] PHP：构造器属性提升
来源：http://gda.quarkkingdee.top

public function __construct(private int $id) {}
来源：http://jqa.pengpengdd.cyou

[U51] PHP：数组解构
来源：http://vcn.gogol.net.cn

[$a, $b] = $arr;
来源：http://tne.fengsongda.top

[U52] PHP：箭头函数
来源：http://xzv.pengpengdd.cyou

$double = fn($x) => $x * 2;
来源：http://eba.tian-w.cn

[U53] PHP：空合并运算符
来源：http://mit.zhaomingkeji.xyz

$v = $a ?? $b ?? "default";
来源：http://exa.hnqzz.top

[U54] PHP：空安全调用
来源：http://qtu.fanxiaobao.xyz

$obj?->method()
来源：http://xdw.cqqwz.cn

[U55] PHP：match 表达式
来源：http://ubp.hnxiangtu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hfq.yuanzhike.top

[U56] PHP：命名参数
来源：http://tsk.9152youxi.cn

f(a: 1, b: 2)
来源：http://qtf.yj202588.top

[U57] PHP：字符串插值
来源：http://eqk.jqgfzy.top

"值: {$a}"
来源：http://yqy.sufxvd.cn

[U58] PHP：数组三件套
来源：http://fqu.daria6918.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jtr.zhaomingkeji.xyz

[U59] PHP：自定义排序
来源：http://aqy.sjlbkw.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xqy.svipenyu.cn

[U60] PHP：JSON 编解码
来源：http://lqe.zhiwuduotai.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wdv.nanxinkj.top

[U61] PHP：正则
来源：http://xjh.sweek.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xjy.wangdashe.top

[U62] PHP：日期对象
来源：http://rju.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pxc.cucudq.cn

[U63] PHP：文件读写
来源：http://ixk.epnwcf.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cuj.aizwys.cn

[U64] PHP：目录遍历
来源：http://kxq.chenzaomai.com

glob("dir/*.php");  scandir("dir");
来源：http://lsn.jinqigufen.top

[U65] PHP：会话
来源：http://shq.yuxming.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sng.hywenlv.cn

[U66] PHP：设置 Cookie
来源：http://rwu.tianlin.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jjm.kuanghao11.cn

[U67] PHP：处理文件上传
来源：http://hjt.jinqigfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zms.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://mhp.daria6918.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ndc.cheryme.top

[U69] PHP：PDO 预处理
来源：http://lhj.kuanghao11.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nez.c1oappe.top

[U70] PHP：PDO 事务
来源：http://ndx.ywan-chungtsiang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://skh.jinyuanbaomall.cn

[U71] PHP：抛出异常
来源：http://ldl.fengsongda.top

throw new RuntimeException("失败", 500);
来源：http://pqi.yangfankeji.com

[U72] PHP：写错误日志
来源：http://dpl.jqgufenzy.top

error_log("失败: " . $e->getMessage());
来源：http://yvn.redwolf501.top

[U73] PHP：读取 ini 配置
来源：http://bcn.zhaomingkeji.xyz

parse_ini_file("config.ini", true)
来源：http://zqt.yonumen.top

[U74] PHP：读取环境变量
来源：http://rjm.chenzaomai.com

getenv("APP_ENV") ?: "production"
来源：http://dor.shanyushiyangtech.top

[U75] PHP：依赖注入
来源：http://knv.nanxinkj.top

composer require psr/container
来源：http://oka.hnxiangtu.top

[U76] PHP：简单路由
来源：http://hxf.cucudq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dsq.jlsjyb.cn

[U77] PHP：模板渲染
来源：http://vpb.0kj1m.cn

composer require twig/twig
来源：http://fif.tanke756.top

[U78] PHP：单元测试
来源：http://yum.xylfe.cn

composer require --dev phpunit/phpunit
来源：http://jiq.yonumen.top

[U79] PHP：静态分析
来源：http://qlv.zhijiandao.cn

composer require --dev phpstan/phpstan
来源：http://axc.hongshengwenyu.top

[U80] PHP：代码规范修复
来源：http://sms.shuidangran.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hjf.mhx1999.top

[U81] JS：初始化项目
来源：http://yzc.ivvv.top

npm init -y;  npm i express
来源：http://mqg.tanke756.top

[U82] JS：package.json 脚本
来源：http://jyq.zhixingplan.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eml.shzxlz.cn

[U83] JS：ES Module 导入导出
来源：http://stp.hcnkem.com

export const a = 1;  import { a } from "./m.js";
来源：http://sal.bbcook.cn

[U84] JS：CommonJS 写法
来源：http://imf.ctjpmb.com

module.exports = { a };  const { a } = require("./m");
来源：http://tmb.zhiwuduotai.top

[U85] JS：可选链
来源：http://aje.yueranfly.top

a?.b?.c
来源：http://udy.zhengqikj.top

[U86] JS：空值合并
来源：http://sdc.ybcxt.top

a ?? b
来源：http://vzr.sjlbkw.cn

[U87] JS：解构默认值
来源：http://vyp.gotoacloud.top

const { a = 1, b = 2 } = obj;
来源：http://idw.dianchejie.cn

[U88] JS：对象展开合并
来源：http://hws.hongshengwenyu.top

{ ...a, ...b }
来源：http://dba.xuanzx.com

[U89] JS：数组去重
来源：http://qgh.yfazqb.com

[...new Set(arr)]
来源：http://qdt.yongpay.top

[U90] JS：数字数组排序
来源：http://kec.chenzaomai.com

[...arr].sort((a, b) => a - b)
来源：http://sbi.zycfv.cn

[U91] JS：对象键值遍历
来源：http://xqs.jqgufenzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ugg.zhoulong.xyz

[U92] JS：深拷贝
来源：http://zrh.yfazqb.com

structuredClone(obj)
来源：http://nra.havefunace.top

[U93] JS：模板字符串
来源：http://czh.svipenyu.cn

`共 ${n} 条`
来源：http://xnw.hesvh.cn

[U94] JS：箭头函数
来源：http://jmi.bbcook.cn

const double = x => x * 2;
来源：http://xjj.quarkkingdee.top

[U95] JS：Promise 包装
来源：http://nhm.fengsongda.top

new Promise((resolve, reject) => {})
来源：http://fze.tian-w.cn

[U96] JS：async/await 与异常
来源：http://ndg.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zsc.epnwcf.com

[U97] JS：并发请求
来源：http://jns.yuanzhike.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lap.jyoumei.cn

[U98] JS：fetch 带 JSON
来源：http://ysa.daxiang520.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ljp.tarul.cn

[U99] JS：事件监听
来源：http://yaj.tian-w.cn

el.addEventListener("click", e => {})
来源：http://zab.0kj1m.cn

[U100] JS：DOM 查询
来源：http://oht.chenlongwang.top

document.querySelector(".item")
来源：http://mue.gogol.net.cn

[U101] JS：classList 操作
来源：http://nnz.zhongyouzk.top

el.classList.toggle("active")
来源：http://pfi.9152youxi.cn

[U102] JS：本地存储
来源：http://zvf.ctjpmb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://prh.hammf.cn

[U103] JS：定时器
来源：http://vzc.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vjt.haohaochexian.top

[U104] JS：防抖
来源：http://qqo.jinqigfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mtb.chenjidiqi.icu

[U105] JS：节流
来源：http://yfl.9152youxi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kys.hnxiangtu.top

[U106] JS：日期格式化
来源：http://oej.kuanghao11.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bzu.cheryme.top

[U107] JS：数字千分位
来源：http://flf.jqgfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rqe.quarkkingdee.top

[U108] JS：随机整数
来源：http://rpg.yueranfly.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iyt.xinyue.icu

[U109] JS：数组分组
来源：http://pcu.shanyushiyangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://jqz.cdnleiting.top

[U110] JS：数组分块
来源：http://jvz.zhixingplan.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://itv.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://fvn.yanxiufei.cn

new Map(Object.entries(obj))
来源：http://iia.redwolf501.top

[U112] JS：字符串补位
来源：http://pjp.ydjk.org.cn

"7".padStart(3, "0")
来源：http://mja.nwbrower.top


<!-- 参考信息 -->