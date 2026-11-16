代发 wailian999

[T47] Perl：正则捕获
来源：http://znu.shangyingyoupin.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fuk.guowangkeji.top

[T48] Perl：正则替换
来源：http://hnz.chenzaomai.com

$s =~ s/old/new/g;
来源：http://qrs.redwolf501.top

[T49] Perl：函数
来源：http://jov.hfpthk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eif.ehwqpu.com

[T50] Perl：逐行读文件
来源：http://fwn.haohaochexian.top

open my $fh, "<", "a.txt" or die $!;
来源：http://irs.gogol.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://owb.52xcode.cn

[T51] Scala：Hello World
来源：http://wbf.yuxming.cn

println("Hello")
来源：http://crf.ppjwa.cn

[T52] Scala：变量
来源：http://kqc.hywenlv.cn

val a = 1;  var b = 2
来源：http://wtd.shanyushiyangkeji.top

[T53] Scala：字符串插值
来源：http://ltx.shzxlz.cn

s"值: $b"
来源：http://kjg.ywan-chungtsiang.top

[T54] Scala：集合映射
来源：http://fxn.jlsjyb.cn

List(1, 2, 3).map(_ * 2)
来源：http://nnw.cdnleiting.top

[T55] Scala：集合过滤
来源：http://bbd.vehdjk.com

List(1, 2, 3).filter(_ > 1)
来源：http://vhd.fanxiaobao.xyz

[T56] Scala：样例类
来源：http://cxi.cashguo.top

case class User(name: String, age: Int)
来源：http://vtm.ywan-chungtsiang.top

[T57] Scala：模式匹配
来源：http://vzf.hammf.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vaj.feifeiyinyue.top

[T58] Scala：函数定义
来源：http://htv.svipenyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tyo.bbcook.cn

[T59] Scala：循环
来源：http://xyt.xuetiantiany.cn

for (i <- 1 to 10) println(i)
来源：http://lsy.nanxuanxn.top

[T60] Scala：折叠
来源：http://tuk.shanyushiyangkeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mrt.jyoumei.cn

================================================================================
来源：http://eia.vehdjk.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ruv.ehwqpu.com

================================================================================
来源：http://kbt.zdbjq.cn

[U01] Py：创建虚拟环境
来源：http://fhg.yonumen.top

python -m venv .venv && source .venv/bin/activate
来源：http://nuk.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://jdq.sjlbkw.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kjp.hfpthk.cn

[U03] Py：加载 .env 配置
来源：http://iby.gogol.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kfn.pycfn.com

[U04] Py：变量调试打印
来源：http://jxg.9152youxi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ion.daria6918.cn

[U05] Py：列表去重且保序
来源：http://vwm.pengpengdd.cyou

list(dict.fromkeys(arr))
来源：http://uvm.yuanzhike.top

[U06] Py：合并两个字典
来源：http://fzu.fehbvm.com

{**a, **b}
来源：http://tbt.chenzaomai.com

[U07] Py：反转字典键值
来源：http://xst.zhoulong.xyz

{v: k for k, v in d.items()}
来源：http://fnd.zhengqikj.top

[U08] Py：展平二维列表
来源：http://xbx.guannengcc.top

[y for x in nested for y in x]
来源：http://lmi.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://ulq.0kj1m.cn

max(d, key=d.get)
来源：http://pdx.hfpthk.cn

[U10] Py：按值排序字典
来源：http://zpl.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://era.jianghu66.top

[U11] Py：生成器表达式
来源：http://axr.zhengqikj.top

(x * 2 for x in arr)
来源：http://agn.yfazqb.com

[U12] Py：取出现最多的 3 个元素
来源：http://xph.aizwys.cn

Counter(arr).most_common(3)
来源：http://pjs.andypj.xyz

[U13] Py：固定长度队列
来源：http://nox.dianchejie.cn

deque(maxlen=10)
来源：http://hcn.9152youxi.cn

[U14] Py：分组收集到列表
来源：http://hec.feifeiyinyue.top

defaultdict(list)
来源：http://okc.zycfv.cn

[U15] Py：高精度计时
来源：http://yml.zhixingplan.top

t = time.perf_counter()
来源：http://ssu.yuanzhike.top

[U16] Py：命令行参数解析
来源：http://yep.zycfv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wux.havefunace.top

[U17] Py：初始化日志
来源：http://ibe.pycfn.com

logging.basicConfig(level=logging.INFO)
来源：http://fjx.dianchejie.cn

[U18] Py：预编译正则
来源：http://trn.316326.xyz

pat = re.compile(r"\d+")
来源：http://msn.gaohongyu789.top

[U19] Py：正则替换带回调
来源：http://wtg.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jal.birdmap.top

[U20] Py：缓存函数结果
来源：http://djr.gotoacloud.top

@functools.lru_cache(maxsize=None)
来源：http://gmf.jinyuanbaomall.cn

[U21] Py：自定义上下文管理器
来源：http://vjy.uphjek.com

@contextlib.contextmanager
来源：http://rfn.tarul.cn

[U22] Py：矩阵转置
来源：http://hwt.c1oappe.top

list(zip(*m))
来源：http://ewj.yangfankeji.com

[U23] Py：分块读取大文件
来源：http://sfi.nanxinkj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jwd.quarkkingdee.top

[U24] Py：路径操作
来源：http://dip.ybcxt.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://onz.uphjek.com

[U25] Py：CSV 按字典读
来源：http://uhv.cashguo.top

csv.DictReader(f)
来源：http://qod.gogol.net.cn

[U26] Py：并发下载
来源：http://yvl.jianghu66.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://anl.ydzc1.top

[U27] Py：异步 HTTP
来源：http://nky.ybcxt.top

aiohttp.ClientSession() 配合 async with
来源：http://ohm.fehbvm.com

[U28] Py：类型别名
来源：http://unk.zycfv.cn

UserId = int
来源：http://gsv.smart0.xyz

[U29] Py：属性校验
来源：http://xra.hywenlv.cn

@property 与 @x.setter 配合
来源：http://scv.daria6918.cn

[U30] Py：数据类
来源：http://raw.hnxiangtu.top

@dataclass(slots=True)
来源：http://czq.sweek.top

[U31] Py：单测
来源：http://gji.xingfuxueyuan.xyz

python -m pytest -q
来源：http://oct.bjfxy.top

[U32] Py：代码格式化
来源：http://npi.wangshuangyany.cn

ruff format . && ruff check --fix .
来源：http://bdg.ywan-chungtsiang.top

[U33] Py：打包发布
来源：http://jkk.jqgufenzy.top

python -m build  （依赖 pyproject.toml）
来源：http://rkz.c1oappe.top

[U34] Py：判断编码
来源：http://ewx.sufxvd.cn

chardet.detect(raw)
来源：http://dti.yvedp.cn

[U35] Py：发送邮件
来源：http://qzh.bbcook.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ibq.hesvh.cn

[U36] Py：定时任务
来源：http://uuq.meibo888.top

schedule.every(10).minutes.do(job)
来源：http://qhb.jlsjyb.cn

[U37] Py：读写 Excel
来源：http://lnl.jinqigfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://tva.shangyingyoupin.top

[U38] Py：获取脚本所在目录
来源：http://gdd.ydzc1.top

Path(__file__).resolve().parent
来源：http://zko.svipenyu.cn

[U39] Py：判断是否在交互环境
来源：http://yso.shanyushiyangtech.top

sys.stdout.isatty()
来源：http://zoa.hammf.cn

[U40] Py：打印到标准错误
来源：http://gsj.xuetiantiany.cn

print("err", file=sys.stderr)
来源：http://pqk.shangyingyoupin.top

[U41] PHP：初始化 Composer 项目
来源：http://kbf.shanyushiyangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zmc.jinyuanbaomall.cn

[U42] PHP：PSR-4 自动加载
来源：http://dcw.zycfv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zgr.gogol.net.cn

[U43] PHP：声明命名空间
来源：http://iae.316326.xyz

namespace App\Http;
来源：http://dze.shanyushiyangtech.top

[U44] PHP：开启严格类型
来源：http://gdi.yuxming.cn

declare(strict_types=1);
来源：http://iuh.hcnkem.com

[U45] PHP：类型声明与返回类型
来源：http://vng.wangshuangyany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bqu.shangyingyoupin.top

[U46] PHP：可空类型
来源：http://slr.sweek.top

?string $name = null
来源：http://ort.zhiwuduotai.top

[U47] PHP：联合类型
来源：http://uzn.nanxinkj.top

int|string $id
来源：http://pcb.yonumen.top

[U48] PHP：纯枚举
来源：http://hoo.jlsjyb.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://snd.daxiang520.top

[U49] PHP：只读属性
来源：http://mso.guannengcc.top

public readonly string $name
来源：http://zpr.xuanzx.com

[U50] PHP：构造器属性提升
来源：http://vhz.guowangkeji.top

public function __construct(private int $id) {}
来源：http://ryr.yongpay.top

[U51] PHP：数组解构
来源：http://mci.hammf.cn

[$a, $b] = $arr;
来源：http://pvb.ydjk.org.cn

[U52] PHP：箭头函数
来源：http://yyi.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://btj.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://xik.zhengqikj.top

$v = $a ?? $b ?? "default";
来源：http://baz.jianghu66.top

[U54] PHP：空安全调用
来源：http://vus.aizwys.cn

$obj?->method()
来源：http://rjs.jinqigfzy.top

[U55] PHP：match 表达式
来源：http://vny.jqgfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gbx.chenlongwang.top

[U56] PHP：命名参数
来源：http://iar.guowangkeji.top

f(a: 1, b: 2)
来源：http://sgs.daxiang520.top

[U57] PHP：字符串插值
来源：http://ibv.sweek.top

"值: {$a}"
来源：http://odm.zdqjudy.top

[U58] PHP：数组三件套
来源：http://wtd.daria6918.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://edf.jinqigfzy.top

[U59] PHP：自定义排序
来源：http://ptu.yanxiufei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gdt.hesvh.cn

[U60] PHP：JSON 编解码
来源：http://owa.andypj.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mug.yuxming.cn

[U61] PHP：正则
来源：http://rov.fktsv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bjf.ybcxt.top

[U62] PHP：日期对象
来源：http://cok.hnqzz.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://abq.jiagoushi.top

[U63] PHP：文件读写
来源：http://hya.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jge.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://umc.zhoulong.xyz

glob("dir/*.php");  scandir("dir");
来源：http://tnz.jianghu66.top

[U65] PHP：会话
来源：http://cst.xinyue.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://bwf.guowangkeji.top

[U66] PHP：设置 Cookie
来源：http://zft.gogol.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jip.birdmap.top

[U67] PHP：处理文件上传
来源：http://ryw.cucudq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://utu.zdbjq.cn

[U68] PHP：PDO 连接
来源：http://fro.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sni.zdbjq.cn

[U69] PHP：PDO 预处理
来源：http://iai.vehdjk.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tze.jianghu66.top

[U70] PHP：PDO 事务
来源：http://zaz.svipenyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ihd.guannengcc.top

[U71] PHP：抛出异常
来源：http://peq.mhx1999.top

throw new RuntimeException("失败", 500);
来源：http://fbj.cashguo.top

[U72] PHP：写错误日志
来源：http://yap.9152youxi.cn

error_log("失败: " . $e->getMessage());
来源：http://emh.aibaodan.cn

[U73] PHP：读取 ini 配置
来源：http://krd.quarkkingdee.top

parse_ini_file("config.ini", true)
来源：http://unm.yvedp.cn

[U74] PHP：读取环境变量
来源：http://gfo.xinyue.icu

getenv("APP_ENV") ?: "production"
来源：http://kst.svipenyu.cn

[U75] PHP：依赖注入
来源：http://xvr.hfpthk.cn

composer require psr/container
来源：http://iet.andypj.xyz

[U76] PHP：简单路由
来源：http://pnk.uphjek.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kje.uphjek.com

[U77] PHP：模板渲染
来源：http://mcz.cucudq.cn

composer require twig/twig
来源：http://ewy.hcnkem.com

[U78] PHP：单元测试
来源：http://zpj.dashuyun.cn

composer require --dev phpunit/phpunit
来源：http://ase.jlsjyb.cn

[U79] PHP：静态分析
来源：http://mka.zhixingplan.top

composer require --dev phpstan/phpstan
来源：http://tye.yongpay.top

[U80] PHP：代码规范修复
来源：http://oyo.xziqi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mue.xinyue.icu

[U81] JS：初始化项目
来源：http://hxj.epnwcf.com

npm init -y;  npm i express
来源：http://gsi.shanyushiyangkeji.top

[U82] JS：package.json 脚本
来源：http://xng.jianghu66.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://luo.uphjek.com

[U83] JS：ES Module 导入导出
来源：http://ezs.uphjek.com

export const a = 1;  import { a } from "./m.js";
来源：http://aqi.zhaomingkeji.xyz

[U84] JS：CommonJS 写法
来源：http://mjf.zhijiandao.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pzh.fehbvm.com

[U85] JS：可选链
来源：http://dic.hnqzz.top

a?.b?.c
来源：http://nuo.ybcxt.top

[U86] JS：空值合并
来源：http://gzc.yongpay.top

a ?? b
来源：http://juf.iojbl.cn

[U87] JS：解构默认值
来源：http://gbf.gaohongyu789.top

const { a = 1, b = 2 } = obj;
来源：http://zeg.ppjwa.cn

[U88] JS：对象展开合并
来源：http://kps.xylfe.cn

{ ...a, ...b }
来源：http://usf.gogol.net.cn

[U89] JS：数组去重
来源：http://oij.ctjpmb.com

[...new Set(arr)]
来源：http://wtu.pengpengdd.cyou

[U90] JS：数字数组排序
来源：http://lsx.zycfv.cn

[...arr].sort((a, b) => a - b)
来源：http://slf.c1oappe.top

[U91] JS：对象键值遍历
来源：http://res.xingfuxueyuan.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rsc.xuanzx.com

[U92] JS：深拷贝
来源：http://baz.xuetiantiany.cn

structuredClone(obj)
来源：http://ukv.cdnleiting.top

[U93] JS：模板字符串
来源：http://fdl.haohaochexian.top

`共 ${n} 条`
来源：http://jts.ydzc1.top

[U94] JS：箭头函数
来源：http://nfh.birdmap.top

const double = x => x * 2;
来源：http://buc.jinqigufen.top

[U95] JS：Promise 包装
来源：http://xtc.gogol.net.cn

new Promise((resolve, reject) => {})
来源：http://lne.birdmap.top

[U96] JS：async/await 与异常
来源：http://fjy.cheryme.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xze.0kj1m.cn

[U97] JS：并发请求
来源：http://xwh.gotoacloud.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://afs.bbcook.cn

[U98] JS：fetch 带 JSON
来源：http://zvs.gotoacloud.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cmj.316326.xyz

[U99] JS：事件监听
来源：http://gwn.jinghuilouyu.cn

el.addEventListener("click", e => {})
来源：http://lik.jlsjyb.cn

[U100] JS：DOM 查询
来源：http://hca.mhx1999.top

document.querySelector(".item")
来源：http://iif.zhaomingkeji.xyz

[U101] JS：classList 操作
来源：http://gmh.gotoacloud.top

el.classList.toggle("active")
来源：http://ouk.jlsjyb.cn

[U102] JS：本地存储
来源：http://ara.tian-w.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vxn.yj20258888.top

[U103] JS：定时器
来源：http://eha.cucudq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hcs.jianghu66.top

[U104] JS：防抖
来源：http://gnz.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yjn.jlsjyb.cn

[U105] JS：节流
来源：http://ceq.vehdjk.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tsr.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://rix.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nrs.hongshengwenyu.top

[U107] JS：数字千分位
来源：http://qlv.xylfe.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hgu.yj20258888.top

[U108] JS：随机整数
来源：http://dob.c1oappe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://byj.hcnkem.com

[U109] JS：数组分组
来源：http://ywd.ybcxt.top

Object.groupBy(arr, x => x.type)
来源：http://eev.daria6918.cn

[U110] JS：数组分块
来源：http://ixg.pengpengdd.cyou

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nmb.vehdjk.com

[U111] JS：对象转 Map
来源：http://qvg.zhijiandao.cn

new Map(Object.entries(obj))
来源：http://uoc.pycfn.com

[U112] JS：字符串补位
来源：http://epl.bbcook.cn

"7".padStart(3, "0")
来源：http://yzl.guannengcc.top

[U113] JS：正则替换全部
来源：http://lnx.gzhubu.top

s.replaceAll("a", "b")
来源：http://sfq.hywenlv.cn

[U114] JS：JSON 深比较
来源：http://mek.ctjpmb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://qyb.kuanghao11.cn

[U115] JS：生成 UUID
来源：http://fuz.ivvv.top

crypto.randomUUID()
来源：http://enm.nanxinkj.top

[U116] JS：类型检查（JSDoc）
来源：http://mqf.ywan-chungtsiang.top

/** @param {string} name */ function f(name) {}
来源：http://inp.yuanzhike.top

[U117] JS：单元测试
来源：http://ayq.chenlongwang.top

npm i -D vitest;  npx vitest
来源：http://uck.sjlbkw.cn

[U118] JS：开发服务器
来源：http://dnq.tian-w.cn

npm i -D vite;  npx vite
来源：http://ztk.daria6918.cn

[U119] JS：生产构建
来源：http://vai.fengsongda.top

npx vite build
来源：http://bvr.wangdashe.top

[U120] JS：读取环境变量（Vite）
来源：http://sgh.zdqjudy.top

import.meta.env.VITE_API_URL
来源：http://zap.ywan-chungtsiang.top

================================================================================
来源：http://vbq.kuanghao11.cn

统计汇总
来源：http://grf.ywan-chungtsiang.top

================================================================================
来源：http://qjw.hongshengwenyu.top

按语言统计（条）：
来源：http://ifq.hnxiangtu.top

Python ......... 252
来源：http://dlc.guannengcc.top

PHP ............ 252
来源：http://not.jinghuilouyu.cn

JavaScript ..... 252
来源：http://wss.zhixingplan.top

TypeScript ..... 212
来源：http://evp.daxiang520.top

Java ........... 212
来源：http://mqk.dianchejie.cn

Go ............. 212
来源：http://zmg.316326.xyz

Ruby ........... 212
来源：http://csw.nwbrower.top

C# ............. 212
来源：http://bxc.gogol.net.cn

C .............. 30
来源：http://jiq.nwbrower.top

C++ ............ 30
来源：http://tns.nanxinkj.top

SQL ............ 90
来源：http://klj.yj20258.top

Bash ........... 80
来源：http://opz.dashuyun.cn

Kotlin ......... 15
来源：http://ucp.havefunace.top

Swift .......... 15
来源：http://dyl.hnqzz.top

Lua ............ 10
来源：http://gia.cheryme.top

Perl ........... 10
来源：http://ctk.zhongyouzk.top

Scala .......... 10
来源：http://aov.zhiwuduotai.top

------------------------------------
来源：http://tvs.hesvh.cn

合计 ........... 2106 条
来源：http://yyk.shuidangran.top

按章节统计：
来源：http://ufg.zdqjudy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zhl.nanxuanxn.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ybt.wangshuangyany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rht.shanyushiyangtech.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://aaa.vehdjk.com


<!-- 参考信息 -->