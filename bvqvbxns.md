代发 wailian999

[T43] Perl：字符串插值
来源：http://avk.guowangkeji.top

"值: $a"
来源：http://kzf.wangdashe.top

[T44] Perl：条件
来源：http://yxb.jqgufenzy.top

if ($a > 0) { print "正"; }
来源：http://pry.jianghu66.top

[T45] Perl：数组遍历
来源：http://drb.chenjidiqi.icu

for my $x (@arr) { print $x; }
来源：http://aum.ehwqpu.com

[T46] Perl：哈希操作
来源：http://plj.yueranfly.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ivk.shanyushiyangtech.top

[T47] Perl：正则捕获
来源：http://dla.guannengcc.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jum.chenzaomai.com

[T48] Perl：正则替换
来源：http://pvn.shzxlz.cn

$s =~ s/old/new/g;
来源：http://ayd.zdqjudy.top

[T49] Perl：函数
来源：http://jgn.yj20258.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jyn.ctjpmb.com

[T50] Perl：逐行读文件
来源：http://jmu.hnqzz.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kwc.zdqjudy.top

while (my $line = <$fh>) { print $line; }
来源：http://wml.guannengcc.top

[T51] Scala：Hello World
来源：http://yxw.tarul.cn

println("Hello")
来源：http://yyx.sjlbkw.cn

[T52] Scala：变量
来源：http://eyx.sysykeji.top

val a = 1;  var b = 2
来源：http://bsy.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://wwc.zhengqikj.top

s"值: $b"
来源：http://swg.zhaomingkeji.xyz

[T54] Scala：集合映射
来源：http://hoi.sysykeji.top

List(1, 2, 3).map(_ * 2)
来源：http://ote.fzhhl.top

[T55] Scala：集合过滤
来源：http://wdh.chenzaomai.com

List(1, 2, 3).filter(_ > 1)
来源：http://qjk.hcnkem.com

[T56] Scala：样例类
来源：http://lyk.xziqi.cn

case class User(name: String, age: Int)
来源：http://elb.meibo888.top

[T57] Scala：模式匹配
来源：http://bke.hywenlv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fzg.jinyuanbaomall.cn

[T58] Scala：函数定义
来源：http://ilu.tanke756.top

def add(a: Int, b: Int): Int = a + b
来源：http://ztq.yuxming.cn

[T59] Scala：循环
来源：http://ive.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://mfv.bbcook.cn

[T60] Scala：折叠
来源：http://izt.daria6918.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ltx.guowangkeji.top

================================================================================
来源：http://egn.fanxiaobao.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nze.tarul.cn

================================================================================
来源：http://swe.chenjidiqi.icu

[U01] Py：创建虚拟环境
来源：http://nvv.yangfankeji.com

python -m venv .venv && source .venv/bin/activate
来源：http://unl.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://xqj.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gyh.zhaomingkeji.xyz

[U03] Py：加载 .env 配置
来源：http://uzm.xziqi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://epj.yvedp.cn

[U04] Py：变量调试打印
来源：http://atv.gotoacloud.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ahn.cqqwz.cn

[U05] Py：列表去重且保序
来源：http://dfq.ctjpmb.com

list(dict.fromkeys(arr))
来源：http://lnc.hnqzz.top

[U06] Py：合并两个字典
来源：http://cfe.zycfv.cn

{**a, **b}
来源：http://lbj.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://bas.0kj1m.cn

{v: k for k, v in d.items()}
来源：http://fij.vehdjk.com

[U08] Py：展平二维列表
来源：http://odd.yongpay.top

[y for x in nested for y in x]
来源：http://rys.nwbrower.top

[U09] Py：字典取最大值的键
来源：http://cer.uphjek.com

max(d, key=d.get)
来源：http://tiu.zhoulong.xyz

[U10] Py：按值排序字典
来源：http://ckm.gotoacloud.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://raf.svipenyu.cn

[U11] Py：生成器表达式
来源：http://dcj.bjfxy.top

(x * 2 for x in arr)
来源：http://duw.yfazqb.com

[U12] Py：取出现最多的 3 个元素
来源：http://aop.cucudq.cn

Counter(arr).most_common(3)
来源：http://wxz.zhixingplan.top

[U13] Py：固定长度队列
来源：http://pyq.hysaishi.cn

deque(maxlen=10)
来源：http://ujk.shangyingyoupin.top

[U14] Py：分组收集到列表
来源：http://kge.jiagoushi.top

defaultdict(list)
来源：http://pyj.sysykeji.top

[U15] Py：高精度计时
来源：http://pzt.hysaishi.cn

t = time.perf_counter()
来源：http://pvf.yj202588.top

[U16] Py：命令行参数解析
来源：http://utb.zhongyouzk.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://guy.yonumen.top

[U17] Py：初始化日志
来源：http://uwq.zhaomingkeji.xyz

logging.basicConfig(level=logging.INFO)
来源：http://wjc.sufxvd.cn

[U18] Py：预编译正则
来源：http://zkq.yonumen.top

pat = re.compile(r"\d+")
来源：http://gie.iojbl.cn

[U19] Py：正则替换带回调
来源：http://hlb.daxiang520.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ojh.jinyuanbaomall.cn

[U20] Py：缓存函数结果
来源：http://qfl.hnqzz.top

@functools.lru_cache(maxsize=None)
来源：http://nzt.jqgufenzy.top

[U21] Py：自定义上下文管理器
来源：http://yaj.0kj1m.cn

@contextlib.contextmanager
来源：http://atu.havefunace.top

[U22] Py：矩阵转置
来源：http://gpo.cucudq.cn

list(zip(*m))
来源：http://pij.cashguo.top

[U23] Py：分块读取大文件
来源：http://eok.vehdjk.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://esd.cucudq.cn

[U24] Py：路径操作
来源：http://nov.jqgfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rdw.zhoulong.xyz

[U25] Py：CSV 按字典读
来源：http://ymn.havefunace.top

csv.DictReader(f)
来源：http://fmp.gogol.net.cn

[U26] Py：并发下载
来源：http://fuu.pycfn.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cir.zhijiandao.cn

[U27] Py：异步 HTTP
来源：http://zip.tarul.cn

aiohttp.ClientSession() 配合 async with
来源：http://omm.haohaochexian.top

[U28] Py：类型别名
来源：http://kew.vehdjk.com

UserId = int
来源：http://nst.jinqigfzy.top

[U29] Py：属性校验
来源：http://yjy.ywan-chungtsiang.top

@property 与 @x.setter 配合
来源：http://ghp.daxiang520.top

[U30] Py：数据类
来源：http://mur.iojbl.cn

@dataclass(slots=True)
来源：http://nul.redwolf501.top

[U31] Py：单测
来源：http://pzg.hywenlv.cn

python -m pytest -q
来源：http://hjf.jyoumei.cn

[U32] Py：代码格式化
来源：http://kgr.yonumen.top

ruff format . && ruff check --fix .
来源：http://xqi.ydzc1.top

[U33] Py：打包发布
来源：http://uam.sjlbkw.cn

python -m build  （依赖 pyproject.toml）
来源：http://rbh.shzxlz.cn

[U34] Py：判断编码
来源：http://qjo.bbcook.cn

chardet.detect(raw)
来源：http://ytk.hywenlv.cn

[U35] Py：发送邮件
来源：http://klz.sjlbkw.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fvk.ydjk.org.cn

[U36] Py：定时任务
来源：http://mba.9152youxi.cn

schedule.every(10).minutes.do(job)
来源：http://xlj.vqdsnc.cn

[U37] Py：读写 Excel
来源：http://uer.haohaochexian.top

pandas.read_excel / DataFrame.to_excel
来源：http://fgj.cqqwz.cn

[U38] Py：获取脚本所在目录
来源：http://ijk.cheryme.top

Path(__file__).resolve().parent
来源：http://oyd.gogol.net.cn

[U39] Py：判断是否在交互环境
来源：http://qwu.ivvv.top

sys.stdout.isatty()
来源：http://nfe.fengsongda.top

[U40] Py：打印到标准错误
来源：http://rge.zhixingplan.top

print("err", file=sys.stderr)
来源：http://lrr.meibo888.top

[U41] PHP：初始化 Composer 项目
来源：http://gag.yangfankeji.com

composer init;  composer require guzzlehttp/guzzle
来源：http://lqz.wangdashe.top

[U42] PHP：PSR-4 自动加载
来源：http://mrh.jlsjyb.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yig.0kj1m.cn

[U43] PHP：声明命名空间
来源：http://ojm.ydzc1.top

namespace App\Http;
来源：http://xbz.guowangkeji.top

[U44] PHP：开启严格类型
来源：http://nue.kuanghao11.cn

declare(strict_types=1);
来源：http://jts.hnqzz.top

[U45] PHP：类型声明与返回类型
来源：http://svw.cucudq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ofi.zhaomingkeji.xyz

[U46] PHP：可空类型
来源：http://sfs.jyoumei.cn

?string $name = null
来源：http://gvw.mhx1999.top

[U47] PHP：联合类型
来源：http://cvm.fktsv.cn

int|string $id
来源：http://tog.0kj1m.cn

[U48] PHP：纯枚举
来源：http://dwf.andypj.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bbk.316326.xyz

[U49] PHP：只读属性
来源：http://xwu.zdqjudy.top

public readonly string $name
来源：http://mty.cheryme.top

[U50] PHP：构造器属性提升
来源：http://jpz.gaohongyu789.top

public function __construct(private int $id) {}
来源：http://noj.jinqigufen.top

[U51] PHP：数组解构
来源：http://xdy.ybcxt.top

[$a, $b] = $arr;
来源：http://wto.jyoumei.cn

[U52] PHP：箭头函数
来源：http://ngw.wangdashe.top

$double = fn($x) => $x * 2;
来源：http://cxc.sysykeji.top

[U53] PHP：空合并运算符
来源：http://rqq.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://wkc.gotoacloud.top

[U54] PHP：空安全调用
来源：http://fqz.aibaodan.cn

$obj?->method()
来源：http://qlk.zhongyouzk.top

[U55] PHP：match 表达式
来源：http://sow.chenlongwang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kzb.fengsongda.top

[U56] PHP：命名参数
来源：http://ujz.jqgfzy.top

f(a: 1, b: 2)
来源：http://gaf.sweek.top

[U57] PHP：字符串插值
来源：http://gal.feifeiyinyue.top

"值: {$a}"
来源：http://ljj.shangyingyoupin.top

[U58] PHP：数组三件套
来源：http://eax.snrcjt.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jjm.zhiwuduotai.top

[U59] PHP：自定义排序
来源：http://knv.jianghu66.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rlb.bbcook.cn

[U60] PHP：JSON 编解码
来源：http://ogw.vehdjk.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jol.jinqigfzy.top

[U61] PHP：正则
来源：http://nza.redwolf501.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lqj.zhiwuduotai.top

[U62] PHP：日期对象
来源：http://rwy.yj202588.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hqr.mhx1999.top

[U63] PHP：文件读写
来源：http://rgq.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://isg.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://tqw.yonumen.top

glob("dir/*.php");  scandir("dir");
来源：http://ock.yanxiufei.cn

[U65] PHP：会话
来源：http://rim.zhixingplan.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jyo.yvedp.cn

[U66] PHP：设置 Cookie
来源：http://ghi.ybcxt.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ozu.andypj.xyz

[U67] PHP：处理文件上传
来源：http://wad.shangyingyoupin.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cbt.hysaishi.cn

[U68] PHP：PDO 连接
来源：http://dps.ctjpmb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wgu.zhaomingkeji.xyz

[U69] PHP：PDO 预处理
来源：http://vzg.yonumen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wxo.xinyue.icu

[U70] PHP：PDO 事务
来源：http://cqk.daria6918.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fmk.ivvv.top

[U71] PHP：抛出异常
来源：http://usx.snrcjt.cn

throw new RuntimeException("失败", 500);
来源：http://skn.xziqi.cn

[U72] PHP：写错误日志
来源：http://sav.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://kvb.epnwcf.com

[U73] PHP：读取 ini 配置
来源：http://esu.yuanzhike.top

parse_ini_file("config.ini", true)
来源：http://axr.bbcook.cn

[U74] PHP：读取环境变量
来源：http://tky.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://pce.nanxinkj.top

[U75] PHP：依赖注入
来源：http://zhn.fzhhl.top

composer require psr/container
来源：http://nqx.ywan-chungtsiang.top

[U76] PHP：简单路由
来源：http://wuk.yj20258.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rxy.hongshengwenyu.top

[U77] PHP：模板渲染
来源：http://yaz.haohaochexian.top

composer require twig/twig
来源：http://gcu.hywenlv.cn

[U78] PHP：单元测试
来源：http://qop.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://yvo.zhiwuduotai.top

[U79] PHP：静态分析
来源：http://yga.fengsongda.top

composer require --dev phpstan/phpstan
来源：http://owt.zycfv.cn

[U80] PHP：代码规范修复
来源：http://phe.aibaodan.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mfa.tian-w.cn

[U81] JS：初始化项目
来源：http://qow.jlsjyb.cn

npm init -y;  npm i express
来源：http://wyd.sysykeji.top

[U82] JS：package.json 脚本
来源：http://phn.meibo888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qcu.iojbl.cn

[U83] JS：ES Module 导入导出
来源：http://wtj.jinyuanbaomall.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zck.nanxinkj.top

[U84] JS：CommonJS 写法
来源：http://wng.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://npt.jqgfzy.top

[U85] JS：可选链
来源：http://ird.zhijiandao.cn

a?.b?.c
来源：http://mbb.yvedp.cn

[U86] JS：空值合并
来源：http://iaj.ppjwa.cn

a ?? b
来源：http://tng.vqdsnc.cn

[U87] JS：解构默认值
来源：http://vol.zdbjq.cn

const { a = 1, b = 2 } = obj;
来源：http://cxw.jianghu66.top

[U88] JS：对象展开合并
来源：http://bqz.zhixingplan.top

{ ...a, ...b }
来源：http://erq.bbcook.cn

[U89] JS：数组去重
来源：http://dsw.yvedp.cn

[...new Set(arr)]
来源：http://tsm.ehwqpu.com

[U90] JS：数字数组排序
来源：http://wjg.hongshengwenyu.top

[...arr].sort((a, b) => a - b)
来源：http://mhv.shanyushiyangkeji.top

[U91] JS：对象键值遍历
来源：http://ixa.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cfc.daxiang520.top

[U92] JS：深拷贝
来源：http://ivs.ppjwa.cn

structuredClone(obj)
来源：http://zxw.tarul.cn

[U93] JS：模板字符串
来源：http://fji.iojbl.cn

`共 ${n} 条`
来源：http://hzl.cheryme.top

[U94] JS：箭头函数
来源：http://jxc.redwolf501.top

const double = x => x * 2;
来源：http://qod.wangshuangyany.cn

[U95] JS：Promise 包装
来源：http://mrb.hongshengwenyu.top

new Promise((resolve, reject) => {})
来源：http://idm.jianghu66.top

[U96] JS：async/await 与异常
来源：http://dih.jinqigfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tzz.tanke756.top

[U97] JS：并发请求
来源：http://ank.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://seo.bbcook.cn

[U98] JS：fetch 带 JSON
来源：http://phe.hcnkem.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bwm.zycfv.cn

[U99] JS：事件监听
来源：http://msy.fengsongda.top

el.addEventListener("click", e => {})
来源：http://fcf.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://smo.wangdashe.top

document.querySelector(".item")
来源：http://afa.guannengcc.top

[U101] JS：classList 操作
来源：http://ijo.fengsongda.top

el.classList.toggle("active")
来源：http://zzb.tian-w.cn

[U102] JS：本地存储
来源：http://vlr.316326.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://qce.guowangkeji.top

[U103] JS：定时器
来源：http://iwg.52xcode.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kyl.ywan-chungtsiang.top

[U104] JS：防抖
来源：http://ayv.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nvl.gaohongyu789.top

[U105] JS：节流
来源：http://ggq.guannengcc.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vqb.jlsjyb.cn

[U106] JS：日期格式化
来源：http://jku.aizwys.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xqr.yj20258888.top

[U107] JS：数字千分位
来源：http://zjm.yj202588.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://klu.fehbvm.com

[U108] JS：随机整数
来源：http://wqh.yonumen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kmu.hammf.cn

[U109] JS：数组分组
来源：http://srs.jyoumei.cn

Object.groupBy(arr, x => x.type)
来源：http://izy.ivvv.top

[U110] JS：数组分块
来源：http://zlm.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://apr.9152youxi.cn

[U111] JS：对象转 Map
来源：http://hbq.fzhhl.top

new Map(Object.entries(obj))
来源：http://sup.xylfe.cn

[U112] JS：字符串补位
来源：http://mgi.wangshuangyany.cn

"7".padStart(3, "0")
来源：http://ewt.ywan-chungtsiang.top

[U113] JS：正则替换全部
来源：http://xch.havefunace.top

s.replaceAll("a", "b")
来源：http://uqo.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://nyl.andypj.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://gxy.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://ibb.ehwqpu.com

crypto.randomUUID()
来源：http://vmw.yanxiufei.cn

[U116] JS：类型检查（JSDoc）
来源：http://kuo.hnxiangtu.top

/** @param {string} name */ function f(name) {}
来源：http://yev.xuetiantiany.cn

[U117] JS：单元测试
来源：http://qgz.ctjpmb.com

npm i -D vitest;  npx vitest
来源：http://nau.sweek.top

[U118] JS：开发服务器
来源：http://jzh.wangdashe.top

npm i -D vite;  npx vite
来源：http://uxi.hongshengwenyu.top

[U119] JS：生产构建
来源：http://jth.shuidangran.top

npx vite build
来源：http://cyx.sufxvd.cn

[U120] JS：读取环境变量（Vite）
来源：http://rud.zhongyouzk.top

import.meta.env.VITE_API_URL
来源：http://icw.zhoulong.xyz

================================================================================
来源：http://afz.snrcjt.cn

统计汇总
来源：http://dop.yangfankeji.com

================================================================================
来源：http://jmh.gogol.net.cn

按语言统计（条）：
来源：http://lcd.chenzaomai.com

Python ......... 252
来源：http://htk.52xcode.cn

PHP ............ 252
来源：http://kgc.svipenyu.cn

JavaScript ..... 252
来源：http://pqi.hammf.cn

TypeScript ..... 212
来源：http://ugf.jinyuanbaomall.cn

Java ........... 212
来源：http://czz.9152youxi.cn

Go ............. 212
来源：http://pgu.hywenlv.cn

Ruby ........... 212
来源：http://tus.fzhhl.top

C# ............. 212
来源：http://mgd.chenjidiqi.icu

C .............. 30
来源：http://qch.jyoumei.cn

C++ ............ 30
来源：http://ckv.sysykeji.top

SQL ............ 90
来源：http://tis.nanxuanxn.top

Bash ........... 80
来源：http://bju.pengpengdd.cyou

Kotlin ......... 15
来源：http://lru.zhaomingkeji.xyz

Swift .......... 15
来源：http://wpf.epnwcf.com

Lua ............ 10
来源：http://vcq.zhengqikj.top

Perl ........... 10
来源：http://rkf.sweek.top


<!-- 参考信息 -->