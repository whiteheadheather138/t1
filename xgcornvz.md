代发 wailian999

[T47] Perl：正则捕获
来源：http://lgo.sufxvd.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pjm.ybcxt.top

[T48] Perl：正则替换
来源：http://tci.jlsjyb.cn

$s =~ s/old/new/g;
来源：http://jps.yvedp.cn

[T49] Perl：函数
来源：http://efo.yuanzhike.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://psj.ivvv.top

[T50] Perl：逐行读文件
来源：http://tni.ydzc1.top

open my $fh, "<", "a.txt" or die $!;
来源：http://myl.shzxlz.cn

while (my $line = <$fh>) { print $line; }
来源：http://ybz.jyoumei.cn

[T51] Scala：Hello World
来源：http://mmh.ctjpmb.com

println("Hello")
来源：http://xpr.ydzc1.top

[T52] Scala：变量
来源：http://qpt.svipenyu.cn

val a = 1;  var b = 2
来源：http://agg.tarul.cn

[T53] Scala：字符串插值
来源：http://cet.shuidangran.top

s"值: $b"
来源：http://bqz.zhaomingkeji.xyz

[T54] Scala：集合映射
来源：http://ebr.tianlin.xyz

List(1, 2, 3).map(_ * 2)
来源：http://rhy.xingfuxueyuan.xyz

[T55] Scala：集合过滤
来源：http://jqq.svipenyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uek.sxryk.cn

[T56] Scala：样例类
来源：http://nnc.hongshengwenyu.top

case class User(name: String, age: Int)
来源：http://whu.iojbl.cn

[T57] Scala：模式匹配
来源：http://zgh.feifeiyinyue.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://iqu.ydjk.org.cn

[T58] Scala：函数定义
来源：http://nbt.zhongyouzk.top

def add(a: Int, b: Int): Int = a + b
来源：http://nhj.daxiang520.top

[T59] Scala：循环
来源：http://wjc.shzxlz.cn

for (i <- 1 to 10) println(i)
来源：http://gzf.ybcxt.top

[T60] Scala：折叠
来源：http://vsi.andypj.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uol.daxiang520.top

================================================================================
来源：http://tpg.shangyingyoupin.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://scl.tian-w.cn

================================================================================
来源：http://cvk.nanxuanxn.top

[U01] Py：创建虚拟环境
来源：http://bfk.xziqi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tzk.xziqi.cn

[U02] Py：导出 / 安装依赖
来源：http://cqw.bjfxy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pry.quarkkingdee.top

[U03] Py：加载 .env 配置
来源：http://fcj.hnqzz.top

from dotenv import load_dotenv; load_dotenv()
来源：http://uno.meibo888.top

[U04] Py：变量调试打印
来源：http://rxk.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zpe.zycfv.cn

[U05] Py：列表去重且保序
来源：http://zqs.ybcxt.top

list(dict.fromkeys(arr))
来源：http://cgm.ctjpmb.com

[U06] Py：合并两个字典
来源：http://mcx.9152youxi.cn

{**a, **b}
来源：http://mur.cheryme.top

[U07] Py：反转字典键值
来源：http://ihy.guowangkeji.top

{v: k for k, v in d.items()}
来源：http://mge.mhx1999.top

[U08] Py：展平二维列表
来源：http://uhu.cucudq.cn

[y for x in nested for y in x]
来源：http://ezi.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://wbh.haohaochexian.top

max(d, key=d.get)
来源：http://nzg.yvedp.cn

[U10] Py：按值排序字典
来源：http://hhs.jqgufenzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ifj.zycfv.cn

[U11] Py：生成器表达式
来源：http://ybz.uphjek.com

(x * 2 for x in arr)
来源：http://ief.smart0.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://dvl.wangdashe.top

Counter(arr).most_common(3)
来源：http://fon.zdqjudy.top

[U13] Py：固定长度队列
来源：http://uiy.ywan-chungtsiang.top

deque(maxlen=10)
来源：http://wnx.chenzaomai.com

[U14] Py：分组收集到列表
来源：http://ape.ydzc1.top

defaultdict(list)
来源：http://wny.hcnkem.com

[U15] Py：高精度计时
来源：http://ida.yj202588.top

t = time.perf_counter()
来源：http://jea.shanyushiyangkeji.top

[U16] Py：命令行参数解析
来源：http://qhf.andypj.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nwt.zhongyouzk.top

[U17] Py：初始化日志
来源：http://ham.vehdjk.com

logging.basicConfig(level=logging.INFO)
来源：http://oex.chenzaomai.com

[U18] Py：预编译正则
来源：http://ohl.gzhubu.top

pat = re.compile(r"\d+")
来源：http://ntf.hfpthk.cn

[U19] Py：正则替换带回调
来源：http://dor.hammf.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://who.sxryk.cn

[U20] Py：缓存函数结果
来源：http://kli.bbcook.cn

@functools.lru_cache(maxsize=None)
来源：http://xkv.fanxiaobao.xyz

[U21] Py：自定义上下文管理器
来源：http://dug.kuanghao11.cn

@contextlib.contextmanager
来源：http://vel.ivvv.top

[U22] Py：矩阵转置
来源：http://glr.xuanzx.com

list(zip(*m))
来源：http://jzc.tian-w.cn

[U23] Py：分块读取大文件
来源：http://otz.vqdsnc.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ndo.aibaodan.cn

[U24] Py：路径操作
来源：http://kvy.zdqjudy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ptw.shzxlz.cn

[U25] Py：CSV 按字典读
来源：http://hbo.pycfn.com

csv.DictReader(f)
来源：http://igj.shanyushiyangkeji.top

[U26] Py：并发下载
来源：http://wlb.zhoulong.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://omz.vehdjk.com

[U27] Py：异步 HTTP
来源：http://tbz.shangyingyoupin.top

aiohttp.ClientSession() 配合 async with
来源：http://lfe.ehwqpu.com

[U28] Py：类型别名
来源：http://wou.zhongyouzk.top

UserId = int
来源：http://ats.jinqigufen.top

[U29] Py：属性校验
来源：http://okw.andypj.xyz

@property 与 @x.setter 配合
来源：http://bub.havefunace.top

[U30] Py：数据类
来源：http://mud.shzxlz.cn

@dataclass(slots=True)
来源：http://ozs.sjlbkw.cn

[U31] Py：单测
来源：http://plv.jlsjyb.cn

python -m pytest -q
来源：http://lsx.aizwys.cn

[U32] Py：代码格式化
来源：http://jce.yj202588.top

ruff format . && ruff check --fix .
来源：http://nat.sjlbkw.cn

[U33] Py：打包发布
来源：http://ezi.yj20258.top

python -m build  （依赖 pyproject.toml）
来源：http://ivc.jinghuilouyu.cn

[U34] Py：判断编码
来源：http://ryj.mhx1999.top

chardet.detect(raw)
来源：http://azo.jinqigufen.top

[U35] Py：发送邮件
来源：http://irx.jyoumei.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nab.zdbjq.cn

[U36] Py：定时任务
来源：http://jut.xingfuxueyuan.xyz

schedule.every(10).minutes.do(job)
来源：http://eot.ctjpmb.com

[U37] Py：读写 Excel
来源：http://yef.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zen.mhx1999.top

[U38] Py：获取脚本所在目录
来源：http://fco.pycfn.com

Path(__file__).resolve().parent
来源：http://uqp.ydzc1.top

[U39] Py：判断是否在交互环境
来源：http://wgt.aizwys.cn

sys.stdout.isatty()
来源：http://vra.hongshengwenyu.top

[U40] Py：打印到标准错误
来源：http://kqi.hcnkem.com

print("err", file=sys.stderr)
来源：http://yci.shanyushiyangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://raa.andypj.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://uso.andypj.xyz

[U42] PHP：PSR-4 自动加载
来源：http://iav.aibaodan.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qlo.jqgfzy.top

[U43] PHP：声明命名空间
来源：http://anz.nanxinkj.top

namespace App\Http;
来源：http://uxh.fengsongda.top

[U44] PHP：开启严格类型
来源：http://zca.fktsv.cn

declare(strict_types=1);
来源：http://bag.tianlin.xyz

[U45] PHP：类型声明与返回类型
来源：http://fjs.yj20258.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://php.zhoulong.xyz

[U46] PHP：可空类型
来源：http://qzf.guowangkeji.top

?string $name = null
来源：http://irm.ehwqpu.com

[U47] PHP：联合类型
来源：http://jhr.feifeiyinyue.top

int|string $id
来源：http://yad.ydjk.org.cn

[U48] PHP：纯枚举
来源：http://wqp.fktsv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zzj.gzhubu.top

[U49] PHP：只读属性
来源：http://hzi.hammf.cn

public readonly string $name
来源：http://bao.hfpthk.cn

[U50] PHP：构造器属性提升
来源：http://myc.havefunace.top

public function __construct(private int $id) {}
来源：http://dpm.dashuyun.cn

[U51] PHP：数组解构
来源：http://hph.nanxinkj.top

[$a, $b] = $arr;
来源：http://jyd.c1oappe.top

[U52] PHP：箭头函数
来源：http://htr.pycfn.com

$double = fn($x) => $x * 2;
来源：http://ymd.c1oappe.top

[U53] PHP：空合并运算符
来源：http://sqy.haohaochexian.top

$v = $a ?? $b ?? "default";
来源：http://vnl.yonumen.top

[U54] PHP：空安全调用
来源：http://div.zdbjq.cn

$obj?->method()
来源：http://lvt.ywan-chungtsiang.top

[U55] PHP：match 表达式
来源：http://dmw.snrcjt.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dqr.ydzc1.top

[U56] PHP：命名参数
来源：http://ses.hfpthk.cn

f(a: 1, b: 2)
来源：http://ywd.svipenyu.cn

[U57] PHP：字符串插值
来源：http://csy.c1oappe.top

"值: {$a}"
来源：http://fbo.hesvh.cn

[U58] PHP：数组三件套
来源：http://vjc.hammf.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mwo.quarkkingdee.top

[U59] PHP：自定义排序
来源：http://lnq.kuanghao11.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ybz.sweek.top

[U60] PHP：JSON 编解码
来源：http://kvu.9152youxi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://aeb.zhoulong.xyz

[U61] PHP：正则
来源：http://fqn.aizwys.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pvl.jinqigufen.top

[U62] PHP：日期对象
来源：http://uws.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eqg.ydzc1.top

[U63] PHP：文件读写
来源：http://xnh.zdqjudy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://chi.tarul.cn

[U64] PHP：目录遍历
来源：http://adh.ywan-chungtsiang.top

glob("dir/*.php");  scandir("dir");
来源：http://bek.xuetiantiany.cn

[U65] PHP：会话
来源：http://mfb.jqgufenzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gbi.aizwys.cn

[U66] PHP：设置 Cookie
来源：http://bmx.zhengqikj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oip.vqdsnc.cn

[U67] PHP：处理文件上传
来源：http://hna.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gbo.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://gad.daxiang520.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kcl.shangyingyoupin.top

[U69] PHP：PDO 预处理
来源：http://oer.xinyue.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pih.quarkkingdee.top

[U70] PHP：PDO 事务
来源：http://wze.hysaishi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ypf.hywenlv.cn

[U71] PHP：抛出异常
来源：http://abp.nanxinkj.top

throw new RuntimeException("失败", 500);
来源：http://gbd.ybcxt.top

[U72] PHP：写错误日志
来源：http://lcr.hongshengwenyu.top

error_log("失败: " . $e->getMessage());
来源：http://ddi.jqgfzy.top

[U73] PHP：读取 ini 配置
来源：http://wzt.hywenlv.cn

parse_ini_file("config.ini", true)
来源：http://yst.vehdjk.com

[U74] PHP：读取环境变量
来源：http://cbh.shanyushiyangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://oid.52xcode.cn

[U75] PHP：依赖注入
来源：http://hvt.zhoulong.xyz

composer require psr/container
来源：http://rsg.sufxvd.cn

[U76] PHP：简单路由
来源：http://uuh.iojbl.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nwp.zhiwuduotai.top

[U77] PHP：模板渲染
来源：http://ntm.havefunace.top

composer require twig/twig
来源：http://teq.chenlongwang.top

[U78] PHP：单元测试
来源：http://zrw.hnqzz.top

composer require --dev phpunit/phpunit
来源：http://hhj.dashuyun.cn

[U79] PHP：静态分析
来源：http://oee.sysykeji.top

composer require --dev phpstan/phpstan
来源：http://ixf.ywan-chungtsiang.top

[U80] PHP：代码规范修复
来源：http://jzx.yanxiufei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://agi.yangfankeji.com

[U81] JS：初始化项目
来源：http://apc.52xcode.cn

npm init -y;  npm i express
来源：http://xzr.zdbjq.cn

[U82] JS：package.json 脚本
来源：http://nxq.jyoumei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jyf.bjfxy.top

[U83] JS：ES Module 导入导出
来源：http://vtf.dianchejie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xwx.hammf.cn

[U84] JS：CommonJS 写法
来源：http://fpc.yfazqb.com

module.exports = { a };  const { a } = require("./m");
来源：http://yjk.ywan-chungtsiang.top

[U85] JS：可选链
来源：http://rwh.ybcxt.top

a?.b?.c
来源：http://xxn.hongshengwenyu.top

[U86] JS：空值合并
来源：http://axc.shangyingyoupin.top

a ?? b
来源：http://ruc.aizwys.cn

[U87] JS：解构默认值
来源：http://bjp.zdbjq.cn

const { a = 1, b = 2 } = obj;
来源：http://vzo.ehwqpu.com

[U88] JS：对象展开合并
来源：http://bej.xuanzx.com

{ ...a, ...b }
来源：http://gfh.sjlbkw.cn

[U89] JS：数组去重
来源：http://rrp.yj20258.top

[...new Set(arr)]
来源：http://gxv.hesvh.cn

[U90] JS：数字数组排序
来源：http://ltj.yfazqb.com

[...arr].sort((a, b) => a - b)
来源：http://pej.zhoulong.xyz

[U91] JS：对象键值遍历
来源：http://dpm.hesvh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kqc.jianghu66.top

[U92] JS：深拷贝
来源：http://smc.jiagoushi.top

structuredClone(obj)
来源：http://zpo.meibo888.top

[U93] JS：模板字符串
来源：http://avz.gzhubu.top

`共 ${n} 条`
来源：http://qam.zhengqikj.top

[U94] JS：箭头函数
来源：http://fne.chenjidiqi.icu

const double = x => x * 2;
来源：http://oen.chenzaomai.com

[U95] JS：Promise 包装
来源：http://rbn.jinyuanbaomall.cn

new Promise((resolve, reject) => {})
来源：http://zfg.zhoulong.xyz

[U96] JS：async/await 与异常
来源：http://oul.hfpthk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rsk.xinyue.icu

[U97] JS：并发请求
来源：http://mij.hcnkem.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ikq.bjfxy.top

[U98] JS：fetch 带 JSON
来源：http://ibm.bjfxy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://udq.kuanghao11.cn

[U99] JS：事件监听
来源：http://imh.jiagoushi.top

el.addEventListener("click", e => {})
来源：http://qfa.316326.xyz

[U100] JS：DOM 查询
来源：http://taz.gogol.net.cn

document.querySelector(".item")
来源：http://vst.cqqwz.cn

[U101] JS：classList 操作
来源：http://fxp.xuanzx.com

el.classList.toggle("active")
来源：http://mgc.hesvh.cn

[U102] JS：本地存储
来源：http://bju.cqqwz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uim.316326.xyz

[U103] JS：定时器
来源：http://jlq.ybcxt.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lnl.fzhhl.top

[U104] JS：防抖
来源：http://muh.mhx1999.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pyg.jinqigfzy.top

[U105] JS：节流
来源：http://tvv.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uoc.xuetiantiany.cn

[U106] JS：日期格式化
来源：http://ytl.zhengqikj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dmd.pycfn.com

[U107] JS：数字千分位
来源：http://rqv.birdmap.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qvm.zhengqikj.top

[U108] JS：随机整数
来源：http://ddy.zhixingplan.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tnf.sjlbkw.cn

[U109] JS：数组分组
来源：http://jpt.shanyushiyangtech.top

Object.groupBy(arr, x => x.type)
来源：http://haa.yuanzhike.top

[U110] JS：数组分块
来源：http://kxp.xylfe.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lzv.shuidangran.top

[U111] JS：对象转 Map
来源：http://kye.yangfankeji.com

new Map(Object.entries(obj))
来源：http://bzi.cucudq.cn

[U112] JS：字符串补位
来源：http://kcu.nanxuanxn.top

"7".padStart(3, "0")
来源：http://byv.jinqigufen.top

[U113] JS：正则替换全部
来源：http://ijr.fzhhl.top

s.replaceAll("a", "b")
来源：http://cwv.jinqigufen.top

[U114] JS：JSON 深比较
来源：http://gjo.ybcxt.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cbv.shuidangran.top

[U115] JS：生成 UUID
来源：http://bqu.hnqzz.top

crypto.randomUUID()
来源：http://oaf.ivvv.top

[U116] JS：类型检查（JSDoc）
来源：http://igv.nanxuanxn.top

/** @param {string} name */ function f(name) {}
来源：http://axy.jqgufenzy.top

[U117] JS：单元测试
来源：http://vfz.52xcode.cn

npm i -D vitest;  npx vitest
来源：http://qxj.smart0.xyz

[U118] JS：开发服务器
来源：http://iiq.mhx1999.top

npm i -D vite;  npx vite
来源：http://xba.chenjidiqi.icu

[U119] JS：生产构建
来源：http://xzz.fehbvm.com

npx vite build
来源：http://dob.tanke756.top

[U120] JS：读取环境变量（Vite）
来源：http://cqo.aizwys.cn

import.meta.env.VITE_API_URL
来源：http://tdq.birdmap.top

================================================================================
来源：http://edy.guannengcc.top

统计汇总
来源：http://kfm.gaohongyu789.top

================================================================================
来源：http://gpu.ybcxt.top

按语言统计（条）：
来源：http://hlr.zhongyouzk.top

Python ......... 252
来源：http://jgi.yfazqb.com

PHP ............ 252
来源：http://vet.xuanzx.com

JavaScript ..... 252
来源：http://zrt.zhengqikj.top

TypeScript ..... 212
来源：http://upu.yuxming.cn

Java ........... 212
来源：http://ixy.nanxinkj.top

Go ............. 212
来源：http://fmb.jqgfzy.top

Ruby ........... 212
来源：http://ena.shuidangran.top

C# ............. 212
来源：http://npl.yueranfly.top

C .............. 30
来源：http://jjg.sysykeji.top

C++ ............ 30
来源：http://kzs.ydzc1.top

SQL ............ 90
来源：http://opg.meibo888.top

Bash ........... 80
来源：http://bjd.jinqigfzy.top

Kotlin ......... 15
来源：http://gmf.andypj.xyz

Swift .......... 15
来源：http://him.havefunace.top

Lua ............ 10
来源：http://ilu.tanke756.top

Perl ........... 10
来源：http://dts.bbcook.cn

Scala .......... 10
来源：http://cuz.mhx1999.top

------------------------------------
来源：http://evi.uphjek.com

合计 ........... 2106 条
来源：http://qie.xuanzx.com

按章节统计：
来源：http://nys.chenjidiqi.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yuf.epnwcf.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wsk.zdbjq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pwo.wangdashe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cgl.nanxinkj.top


<!-- 参考信息 -->