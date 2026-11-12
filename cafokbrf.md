代发 wailian999

[T45] Perl：数组遍历
来源：http://umk.svipenyu.cn

for my $x (@arr) { print $x; }
来源：http://gbo.svipenyu.cn

[T46] Perl：哈希操作
来源：http://smw.smart0.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qsf.jqgfzy.top

[T47] Perl：正则捕获
来源：http://lii.jqgfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yog.wangshuangyany.cn

[T48] Perl：正则替换
来源：http://txj.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://fmg.jlsjyb.cn

[T49] Perl：函数
来源：http://pmw.uphjek.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ohs.tarul.cn

[T50] Perl：逐行读文件
来源：http://hzh.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://snc.daxiang520.top

while (my $line = <$fh>) { print $line; }
来源：http://rur.fzhhl.top

[T51] Scala：Hello World
来源：http://cxz.jinyuanbaomall.cn

println("Hello")
来源：http://vpv.guowangkeji.top

[T52] Scala：变量
来源：http://qfv.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://kip.cqqwz.cn

[T53] Scala：字符串插值
来源：http://mwb.0kj1m.cn

s"值: $b"
来源：http://lxm.ydzc1.top

[T54] Scala：集合映射
来源：http://xra.hcnkem.com

List(1, 2, 3).map(_ * 2)
来源：http://vwr.meibo888.top

[T55] Scala：集合过滤
来源：http://ffz.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://dld.kuanghao11.cn

[T56] Scala：样例类
来源：http://szi.zhijiandao.cn

case class User(name: String, age: Int)
来源：http://wsh.chenjidiqi.icu

[T57] Scala：模式匹配
来源：http://fgu.ybcxt.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://owa.zhaomingkeji.xyz

[T58] Scala：函数定义
来源：http://ogz.sjlbkw.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tyb.zdqjudy.top

[T59] Scala：循环
来源：http://esw.yongpay.top

for (i <- 1 to 10) println(i)
来源：http://wtt.zdqjudy.top

[T60] Scala：折叠
来源：http://gqc.ydzc1.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ldi.yj202588.top

================================================================================
来源：http://nhb.redwolf501.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zmm.daria6918.cn

================================================================================
来源：http://dno.fanxiaobao.xyz

[U01] Py：创建虚拟环境
来源：http://lcc.yvedp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jmn.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://ens.havefunace.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pzg.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://vze.birdmap.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bxo.yj20258888.top

[U04] Py：变量调试打印
来源：http://lku.xingfuxueyuan.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qml.hesvh.cn

[U05] Py：列表去重且保序
来源：http://mir.ctjpmb.com

list(dict.fromkeys(arr))
来源：http://owf.yuxming.cn

[U06] Py：合并两个字典
来源：http://svu.fktsv.cn

{**a, **b}
来源：http://zat.ehwqpu.com

[U07] Py：反转字典键值
来源：http://khq.jqgfzy.top

{v: k for k, v in d.items()}
来源：http://bwk.dianchejie.cn

[U08] Py：展平二维列表
来源：http://gpl.zhoulong.xyz

[y for x in nested for y in x]
来源：http://wdq.sjlbkw.cn

[U09] Py：字典取最大值的键
来源：http://fle.yj202588.top

max(d, key=d.get)
来源：http://mgm.jiagoushi.top

[U10] Py：按值排序字典
来源：http://zbp.jyoumei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://epi.nwbrower.top

[U11] Py：生成器表达式
来源：http://era.epnwcf.com

(x * 2 for x in arr)
来源：http://xty.zhoulong.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://tpk.xziqi.cn

Counter(arr).most_common(3)
来源：http://ljx.shuidangran.top

[U13] Py：固定长度队列
来源：http://ikp.havefunace.top

deque(maxlen=10)
来源：http://auz.daria6918.cn

[U14] Py：分组收集到列表
来源：http://asc.cdnleiting.top

defaultdict(list)
来源：http://wcz.redwolf501.top

[U15] Py：高精度计时
来源：http://mmc.meibo888.top

t = time.perf_counter()
来源：http://bef.ywan-chungtsiang.top

[U16] Py：命令行参数解析
来源：http://ukx.yj20258.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tfk.yangfankeji.com

[U17] Py：初始化日志
来源：http://jey.hongshengwenyu.top

logging.basicConfig(level=logging.INFO)
来源：http://cwh.yonumen.top

[U18] Py：预编译正则
来源：http://mgj.ctjpmb.com

pat = re.compile(r"\d+")
来源：http://umb.jinqigufen.top

[U19] Py：正则替换带回调
来源：http://wth.sjlbkw.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xff.fzhhl.top

[U20] Py：缓存函数结果
来源：http://xxb.feifeiyinyue.top

@functools.lru_cache(maxsize=None)
来源：http://iyg.guowangkeji.top

[U21] Py：自定义上下文管理器
来源：http://abr.yonumen.top

@contextlib.contextmanager
来源：http://anj.fengsongda.top

[U22] Py：矩阵转置
来源：http://gtb.yuxming.cn

list(zip(*m))
来源：http://awx.andypj.xyz

[U23] Py：分块读取大文件
来源：http://yij.epnwcf.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dej.jlsjyb.cn

[U24] Py：路径操作
来源：http://lnm.yvedp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tvp.xinyue.icu

[U25] Py：CSV 按字典读
来源：http://doj.52xcode.cn

csv.DictReader(f)
来源：http://lns.c1oappe.top

[U26] Py：并发下载
来源：http://kth.gogol.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cmy.svipenyu.cn

[U27] Py：异步 HTTP
来源：http://erk.xingfuxueyuan.xyz

aiohttp.ClientSession() 配合 async with
来源：http://zvc.hnxiangtu.top

[U28] Py：类型别名
来源：http://jrb.yvedp.cn

UserId = int
来源：http://bqd.c1oappe.top

[U29] Py：属性校验
来源：http://stx.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://rfk.smart0.xyz

[U30] Py：数据类
来源：http://cdh.ybcxt.top

@dataclass(slots=True)
来源：http://fdh.zhixingplan.top

[U31] Py：单测
来源：http://qoz.zhixingplan.top

python -m pytest -q
来源：http://chb.zhijiandao.cn

[U32] Py：代码格式化
来源：http://oje.guannengcc.top

ruff format . && ruff check --fix .
来源：http://wtg.yvedp.cn

[U33] Py：打包发布
来源：http://ymf.gogol.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://oze.0kj1m.cn

[U34] Py：判断编码
来源：http://wzr.xziqi.cn

chardet.detect(raw)
来源：http://ktk.shanyushiyangtech.top

[U35] Py：发送邮件
来源：http://rac.guowangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jnn.hesvh.cn

[U36] Py：定时任务
来源：http://coh.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://kxn.sweek.top

[U37] Py：读写 Excel
来源：http://mtz.havefunace.top

pandas.read_excel / DataFrame.to_excel
来源：http://eac.sweek.top

[U38] Py：获取脚本所在目录
来源：http://ryz.yvedp.cn

Path(__file__).resolve().parent
来源：http://icu.vqdsnc.cn

[U39] Py：判断是否在交互环境
来源：http://rgj.feifeiyinyue.top

sys.stdout.isatty()
来源：http://xxq.tianlin.xyz

[U40] Py：打印到标准错误
来源：http://wsx.cdnleiting.top

print("err", file=sys.stderr)
来源：http://ncv.0kj1m.cn

[U41] PHP：初始化 Composer 项目
来源：http://whj.ivvv.top

composer init;  composer require guzzlehttp/guzzle
来源：http://klm.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://ncz.hywenlv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gfh.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://bbo.ydzc1.top

namespace App\Http;
来源：http://jtf.9152youxi.cn

[U44] PHP：开启严格类型
来源：http://snb.jinyuanbaomall.cn

declare(strict_types=1);
来源：http://ssg.tarul.cn

[U45] PHP：类型声明与返回类型
来源：http://jey.aibaodan.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://msx.zhixingplan.top

[U46] PHP：可空类型
来源：http://log.fktsv.cn

?string $name = null
来源：http://cby.aibaodan.cn

[U47] PHP：联合类型
来源：http://brv.vqdsnc.cn

int|string $id
来源：http://nsl.fktsv.cn

[U48] PHP：纯枚举
来源：http://axp.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xid.ctjpmb.com

[U49] PHP：只读属性
来源：http://qmt.nanxuanxn.top

public readonly string $name
来源：http://lct.sjlbkw.cn

[U50] PHP：构造器属性提升
来源：http://zgw.andypj.xyz

public function __construct(private int $id) {}
来源：http://tqk.daria6918.cn

[U51] PHP：数组解构
来源：http://lzw.tarul.cn

[$a, $b] = $arr;
来源：http://cri.xingfuxueyuan.xyz

[U52] PHP：箭头函数
来源：http://xvz.ctjpmb.com

$double = fn($x) => $x * 2;
来源：http://qhj.ydjk.org.cn

[U53] PHP：空合并运算符
来源：http://cxj.shanyushiyangtech.top

$v = $a ?? $b ?? "default";
来源：http://tli.hesvh.cn

[U54] PHP：空安全调用
来源：http://fdf.gogol.net.cn

$obj?->method()
来源：http://vvz.sjlbkw.cn

[U55] PHP：match 表达式
来源：http://dex.52xcode.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uxr.ehwqpu.com

[U56] PHP：命名参数
来源：http://gyf.fanxiaobao.xyz

f(a: 1, b: 2)
来源：http://lqx.cdnleiting.top

[U57] PHP：字符串插值
来源：http://bhf.svipenyu.cn

"值: {$a}"
来源：http://mgj.dianchejie.cn

[U58] PHP：数组三件套
来源：http://lca.shanyushiyangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jhw.yangfankeji.com

[U59] PHP：自定义排序
来源：http://eia.yuanzhike.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jny.zdbjq.cn

[U60] PHP：JSON 编解码
来源：http://yiw.cqqwz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cjs.sufxvd.cn

[U61] PHP：正则
来源：http://ngr.wangdashe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rut.zhijiandao.cn

[U62] PHP：日期对象
来源：http://vfa.sweek.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://apq.fanxiaobao.xyz

[U63] PHP：文件读写
来源：http://diw.pycfn.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iio.jinqigufen.top

[U64] PHP：目录遍历
来源：http://qsn.epnwcf.com

glob("dir/*.php");  scandir("dir");
来源：http://hga.gotoacloud.top

[U65] PHP：会话
来源：http://fey.birdmap.top

session_start();  $_SESSION["uid"] = 1;
来源：http://znh.zdqjudy.top

[U66] PHP：设置 Cookie
来源：http://lvw.zhongyouzk.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uum.yangfankeji.com

[U67] PHP：处理文件上传
来源：http://zse.zhongyouzk.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://juc.bjfxy.top

[U68] PHP：PDO 连接
来源：http://vdd.uphjek.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qwr.shzxlz.cn

[U69] PHP：PDO 预处理
来源：http://nju.hcnkem.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://shb.chenjidiqi.icu

[U70] PHP：PDO 事务
来源：http://njg.ehwqpu.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zyh.fanxiaobao.xyz

[U71] PHP：抛出异常
来源：http://cfs.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://bnv.hywenlv.cn

[U72] PHP：写错误日志
来源：http://kbd.hammf.cn

error_log("失败: " . $e->getMessage());
来源：http://dth.ybcxt.top

[U73] PHP：读取 ini 配置
来源：http://acf.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://hyz.cashguo.top

[U74] PHP：读取环境变量
来源：http://yxu.bjfxy.top

getenv("APP_ENV") ?: "production"
来源：http://hmu.sysykeji.top

[U75] PHP：依赖注入
来源：http://iug.zdbjq.cn

composer require psr/container
来源：http://nlt.shangyingyoupin.top

[U76] PHP：简单路由
来源：http://ttv.sufxvd.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fen.iojbl.cn

[U77] PHP：模板渲染
来源：http://kni.gotoacloud.top

composer require twig/twig
来源：http://ewp.jqgufenzy.top

[U78] PHP：单元测试
来源：http://jad.wangdashe.top

composer require --dev phpunit/phpunit
来源：http://fiy.jlsjyb.cn

[U79] PHP：静态分析
来源：http://bfh.birdmap.top

composer require --dev phpstan/phpstan
来源：http://ips.zhiwuduotai.top

[U80] PHP：代码规范修复
来源：http://efc.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dsg.jqgfzy.top

[U81] JS：初始化项目
来源：http://xwp.yuxming.cn

npm init -y;  npm i express
来源：http://spl.cheryme.top

[U82] JS：package.json 脚本
来源：http://fiq.jinyuanbaomall.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ael.shuidangran.top

[U83] JS：ES Module 导入导出
来源：http://aeb.ybcxt.top

export const a = 1;  import { a } from "./m.js";
来源：http://tml.yanxiufei.cn

[U84] JS：CommonJS 写法
来源：http://kla.gaohongyu789.top

module.exports = { a };  const { a } = require("./m");
来源：http://zcl.zhiwuduotai.top

[U85] JS：可选链
来源：http://nji.yangfankeji.com

a?.b?.c
来源：http://cdj.tian-w.cn

[U86] JS：空值合并
来源：http://xlo.yanxiufei.cn

a ?? b
来源：http://uzq.dianchejie.cn

[U87] JS：解构默认值
来源：http://lcf.ydjk.org.cn

const { a = 1, b = 2 } = obj;
来源：http://ggu.redwolf501.top

[U88] JS：对象展开合并
来源：http://agf.aibaodan.cn

{ ...a, ...b }
来源：http://ret.ehwqpu.com

[U89] JS：数组去重
来源：http://sgc.kuanghao11.cn

[...new Set(arr)]
来源：http://wlo.ivvv.top

[U90] JS：数字数组排序
来源：http://qzp.ybcxt.top

[...arr].sort((a, b) => a - b)
来源：http://ism.tarul.cn

[U91] JS：对象键值遍历
来源：http://fnx.zhaomingkeji.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nze.0kj1m.cn

[U92] JS：深拷贝
来源：http://gnt.jinyuanbaomall.cn

structuredClone(obj)
来源：http://dro.haohaochexian.top

[U93] JS：模板字符串
来源：http://nys.fktsv.cn

`共 ${n} 条`
来源：http://kgd.hcnkem.com

[U94] JS：箭头函数
来源：http://oku.jqgufenzy.top

const double = x => x * 2;
来源：http://qlc.sxryk.cn

[U95] JS：Promise 包装
来源：http://ltl.cdnleiting.top

new Promise((resolve, reject) => {})
来源：http://ccx.52xcode.cn

[U96] JS：async/await 与异常
来源：http://tkh.yvedp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jwj.bjfxy.top

[U97] JS：并发请求
来源：http://cbi.haohaochexian.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jfu.ydzc1.top

[U98] JS：fetch 带 JSON
来源：http://dqp.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://omt.yanxiufei.cn

[U99] JS：事件监听
来源：http://mcm.yonumen.top

el.addEventListener("click", e => {})
来源：http://eia.yueranfly.top

[U100] JS：DOM 查询
来源：http://xez.tarul.cn

document.querySelector(".item")
来源：http://zyh.ehwqpu.com

[U101] JS：classList 操作
来源：http://hcy.yj202588.top

el.classList.toggle("active")
来源：http://jqi.kuanghao11.cn

[U102] JS：本地存储
来源：http://vss.yangfankeji.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ntc.hysaishi.cn

[U103] JS：定时器
来源：http://gxg.xziqi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wet.jinghuilouyu.cn

[U104] JS：防抖
来源：http://myg.dianchejie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://moa.jinqigfzy.top

[U105] JS：节流
来源：http://xtr.chenjidiqi.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://szx.nanxinkj.top

[U106] JS：日期格式化
来源：http://iha.hnqzz.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://txb.xuetiantiany.cn

[U107] JS：数字千分位
来源：http://rzh.ywan-chungtsiang.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wyw.ivvv.top

[U108] JS：随机整数
来源：http://ltt.shangyingyoupin.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pnr.ppjwa.cn

[U109] JS：数组分组
来源：http://vmr.aibaodan.cn

Object.groupBy(arr, x => x.type)
来源：http://lld.xuetiantiany.cn

[U110] JS：数组分块
来源：http://lzq.xuetiantiany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aha.jiagoushi.top

[U111] JS：对象转 Map
来源：http://bdc.gzhubu.top

new Map(Object.entries(obj))
来源：http://fsc.fehbvm.com

[U112] JS：字符串补位
来源：http://zxs.ydjk.org.cn

"7".padStart(3, "0")
来源：http://meb.yfazqb.com

[U113] JS：正则替换全部
来源：http://brd.nwbrower.top

s.replaceAll("a", "b")
来源：http://fdh.feifeiyinyue.top

[U114] JS：JSON 深比较
来源：http://keg.hfpthk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hcy.daria6918.cn

[U115] JS：生成 UUID
来源：http://wgd.fzhhl.top

crypto.randomUUID()
来源：http://oau.hnxiangtu.top

[U116] JS：类型检查（JSDoc）
来源：http://nlp.smart0.xyz

/** @param {string} name */ function f(name) {}
来源：http://spn.gogol.net.cn

[U117] JS：单元测试
来源：http://xaj.feifeiyinyue.top

npm i -D vitest;  npx vitest
来源：http://fpl.ydjk.org.cn

[U118] JS：开发服务器
来源：http://dmo.gzhubu.top

npm i -D vite;  npx vite
来源：http://awe.yanxiufei.cn

[U119] JS：生产构建
来源：http://hcs.gogol.net.cn

npx vite build
来源：http://mtv.sysykeji.top

[U120] JS：读取环境变量（Vite）
来源：http://qxn.hongshengwenyu.top

import.meta.env.VITE_API_URL
来源：http://xtv.epnwcf.com

================================================================================
来源：http://cbh.52xcode.cn

统计汇总
来源：http://fcr.fanxiaobao.xyz

================================================================================
来源：http://spe.jinghuilouyu.cn

按语言统计（条）：
来源：http://zgi.nwbrower.top

Python ......... 252
来源：http://tsd.0kj1m.cn

PHP ............ 252
来源：http://hhj.0kj1m.cn

JavaScript ..... 252
来源：http://qhs.feifeiyinyue.top

TypeScript ..... 212
来源：http://xip.nwbrower.top

Java ........... 212
来源：http://tuz.xinyue.icu

Go ............. 212
来源：http://mlk.birdmap.top

Ruby ........... 212
来源：http://hta.zdqjudy.top

C# ............. 212
来源：http://nsw.haohaochexian.top

C .............. 30
来源：http://ibt.yj20258.top

C++ ............ 30
来源：http://yvu.yangfankeji.com

SQL ............ 90
来源：http://stg.hfpthk.cn

Bash ........... 80
来源：http://etv.xylfe.cn

Kotlin ......... 15
来源：http://vgz.yanxiufei.cn

Swift .......... 15
来源：http://rrp.pycfn.com

Lua ............ 10
来源：http://hnr.zhengqikj.top

Perl ........... 10
来源：http://tny.gaohongyu789.top

Scala .......... 10
来源：http://oej.hywenlv.cn

------------------------------------
来源：http://dum.yj20258.top

合计 ........... 2106 条
来源：http://yrd.uphjek.com

按章节统计：
来源：http://foa.jiagoushi.top


<!-- 参考信息 -->