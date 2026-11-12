代发 wailian999

[T49] Perl：函数
来源：http://zzm.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xcu.jinghuilouyu.cn

[T50] Perl：逐行读文件
来源：http://bov.gaohongyu789.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yag.ydjk.org.cn

while (my $line = <$fh>) { print $line; }
来源：http://eyt.tanke756.top

[T51] Scala：Hello World
来源：http://lje.wangdashe.top

println("Hello")
来源：http://mzk.ctjpmb.com

[T52] Scala：变量
来源：http://xlq.cdnleiting.top

val a = 1;  var b = 2
来源：http://nbd.bjfxy.top

[T53] Scala：字符串插值
来源：http://wrm.zdqjudy.top

s"值: $b"
来源：http://umb.nanxinkj.top

[T54] Scala：集合映射
来源：http://llw.wangdashe.top

List(1, 2, 3).map(_ * 2)
来源：http://xpa.fzhhl.top

[T55] Scala：集合过滤
来源：http://qso.9152youxi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vby.dianchejie.cn

[T56] Scala：样例类
来源：http://itg.cheryme.top

case class User(name: String, age: Int)
来源：http://lcw.gogol.net.cn

[T57] Scala：模式匹配
来源：http://dcc.nanxinkj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fjy.yueranfly.top

[T58] Scala：函数定义
来源：http://rbq.sufxvd.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ivn.zhijiandao.cn

[T59] Scala：循环
来源：http://vfu.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://edh.daria6918.cn

[T60] Scala：折叠
来源：http://jfd.gotoacloud.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://axu.svipenyu.cn

================================================================================
来源：http://nqi.ppjwa.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iut.ybcxt.top

================================================================================
来源：http://nhy.tian-w.cn

[U01] Py：创建虚拟环境
来源：http://lhs.meibo888.top

python -m venv .venv && source .venv/bin/activate
来源：http://fwl.jiagoushi.top

[U02] Py：导出 / 安装依赖
来源：http://vhw.jinqigufen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ccq.316326.xyz

[U03] Py：加载 .env 配置
来源：http://evt.ydjk.org.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qys.wangdashe.top

[U04] Py：变量调试打印
来源：http://wlx.shzxlz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fik.ehwqpu.com

[U05] Py：列表去重且保序
来源：http://xvq.havefunace.top

list(dict.fromkeys(arr))
来源：http://qdc.jinqigfzy.top

[U06] Py：合并两个字典
来源：http://gic.cashguo.top

{**a, **b}
来源：http://cnz.mhx1999.top

[U07] Py：反转字典键值
来源：http://umj.vehdjk.com

{v: k for k, v in d.items()}
来源：http://vuh.yuxming.cn

[U08] Py：展平二维列表
来源：http://zhv.dashuyun.cn

[y for x in nested for y in x]
来源：http://eog.gogol.net.cn

[U09] Py：字典取最大值的键
来源：http://bxf.jyoumei.cn

max(d, key=d.get)
来源：http://cml.jlsjyb.cn

[U10] Py：按值排序字典
来源：http://qzn.xziqi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gvx.hesvh.cn

[U11] Py：生成器表达式
来源：http://zyi.jianghu66.top

(x * 2 for x in arr)
来源：http://jyy.quarkkingdee.top

[U12] Py：取出现最多的 3 个元素
来源：http://khi.ehwqpu.com

Counter(arr).most_common(3)
来源：http://rnh.xuetiantiany.cn

[U13] Py：固定长度队列
来源：http://zab.zycfv.cn

deque(maxlen=10)
来源：http://qlg.c1oappe.top

[U14] Py：分组收集到列表
来源：http://ybr.havefunace.top

defaultdict(list)
来源：http://fic.shanyushiyangkeji.top

[U15] Py：高精度计时
来源：http://rel.jiagoushi.top

t = time.perf_counter()
来源：http://tvu.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://hjp.xziqi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zkx.yfazqb.com

[U17] Py：初始化日志
来源：http://mmg.cheryme.top

logging.basicConfig(level=logging.INFO)
来源：http://ict.zhengqikj.top

[U18] Py：预编译正则
来源：http://zqn.vehdjk.com

pat = re.compile(r"\d+")
来源：http://znr.ppjwa.cn

[U19] Py：正则替换带回调
来源：http://mwa.birdmap.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tgj.jinghuilouyu.cn

[U20] Py：缓存函数结果
来源：http://mvh.yonumen.top

@functools.lru_cache(maxsize=None)
来源：http://eyd.cashguo.top

[U21] Py：自定义上下文管理器
来源：http://lke.9152youxi.cn

@contextlib.contextmanager
来源：http://uyg.uphjek.com

[U22] Py：矩阵转置
来源：http://zxb.quarkkingdee.top

list(zip(*m))
来源：http://yby.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://ilo.cqqwz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://awp.yongpay.top

[U24] Py：路径操作
来源：http://ykv.sjlbkw.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wsv.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://ivs.ybcxt.top

csv.DictReader(f)
来源：http://mnk.havefunace.top

[U26] Py：并发下载
来源：http://tcp.yanxiufei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nhv.ehwqpu.com

[U27] Py：异步 HTTP
来源：http://dfe.cdnleiting.top

aiohttp.ClientSession() 配合 async with
来源：http://qxu.yj202588.top

[U28] Py：类型别名
来源：http://ptm.smart0.xyz

UserId = int
来源：http://ggf.shanyushiyangtech.top

[U29] Py：属性校验
来源：http://emk.zhoulong.xyz

@property 与 @x.setter 配合
来源：http://fai.gotoacloud.top

[U30] Py：数据类
来源：http://uwz.52xcode.cn

@dataclass(slots=True)
来源：http://xol.yfazqb.com

[U31] Py：单测
来源：http://vhc.sxryk.cn

python -m pytest -q
来源：http://cue.cucudq.cn

[U32] Py：代码格式化
来源：http://vtw.kuanghao11.cn

ruff format . && ruff check --fix .
来源：http://odx.daxiang520.top

[U33] Py：打包发布
来源：http://xhi.yfazqb.com

python -m build  （依赖 pyproject.toml）
来源：http://cfs.wangdashe.top

[U34] Py：判断编码
来源：http://usf.fzhhl.top

chardet.detect(raw)
来源：http://dxd.jinqigufen.top

[U35] Py：发送邮件
来源：http://qwg.zdqjudy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://poo.gaohongyu789.top

[U36] Py：定时任务
来源：http://ire.fktsv.cn

schedule.every(10).minutes.do(job)
来源：http://jki.ywan-chungtsiang.top

[U37] Py：读写 Excel
来源：http://abr.fanxiaobao.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://evw.zhengqikj.top

[U38] Py：获取脚本所在目录
来源：http://cfk.shangyingyoupin.top

Path(__file__).resolve().parent
来源：http://ahp.chenjidiqi.icu

[U39] Py：判断是否在交互环境
来源：http://hbp.hongshengwenyu.top

sys.stdout.isatty()
来源：http://zjj.havefunace.top

[U40] Py：打印到标准错误
来源：http://etb.epnwcf.com

print("err", file=sys.stderr)
来源：http://wbw.fengsongda.top

[U41] PHP：初始化 Composer 项目
来源：http://sae.jinghuilouyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mly.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://oam.yongpay.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jbu.xylfe.cn

[U43] PHP：声明命名空间
来源：http://emt.zhengqikj.top

namespace App\Http;
来源：http://enx.hfpthk.cn

[U44] PHP：开启严格类型
来源：http://qyo.pycfn.com

declare(strict_types=1);
来源：http://uys.xinyue.icu

[U45] PHP：类型声明与返回类型
来源：http://czj.zhixingplan.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://irz.zhoulong.xyz

[U46] PHP：可空类型
来源：http://xum.52xcode.cn

?string $name = null
来源：http://ira.xziqi.cn

[U47] PHP：联合类型
来源：http://fwj.cashguo.top

int|string $id
来源：http://jzy.tian-w.cn

[U48] PHP：纯枚举
来源：http://uqj.xingfuxueyuan.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rsw.fengsongda.top

[U49] PHP：只读属性
来源：http://ogp.yvedp.cn

public readonly string $name
来源：http://ijq.jianghu66.top

[U50] PHP：构造器属性提升
来源：http://jiy.svipenyu.cn

public function __construct(private int $id) {}
来源：http://hjv.zdbjq.cn

[U51] PHP：数组解构
来源：http://adh.daxiang520.top

[$a, $b] = $arr;
来源：http://xxg.jinyuanbaomall.cn

[U52] PHP：箭头函数
来源：http://xci.pycfn.com

$double = fn($x) => $x * 2;
来源：http://fuw.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://oud.jlsjyb.cn

$v = $a ?? $b ?? "default";
来源：http://gwa.hnqzz.top

[U54] PHP：空安全调用
来源：http://ndh.yongpay.top

$obj?->method()
来源：http://uhp.fzhhl.top

[U55] PHP：match 表达式
来源：http://rfa.wangshuangyany.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://opp.chenlongwang.top

[U56] PHP：命名参数
来源：http://lzx.shzxlz.cn

f(a: 1, b: 2)
来源：http://hrh.ywan-chungtsiang.top

[U57] PHP：字符串插值
来源：http://htp.cucudq.cn

"值: {$a}"
来源：http://bhs.tianlin.xyz

[U58] PHP：数组三件套
来源：http://eiw.jinghuilouyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://owg.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://opf.hcnkem.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cfh.xziqi.cn

[U60] PHP：JSON 编解码
来源：http://wyq.xylfe.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jbr.daria6918.cn

[U61] PHP：正则
来源：http://bpx.aibaodan.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fab.yj20258888.top

[U62] PHP：日期对象
来源：http://xvw.chenlongwang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bjb.ydzc1.top

[U63] PHP：文件读写
来源：http://das.chenjidiqi.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mzl.xziqi.cn

[U64] PHP：目录遍历
来源：http://hur.xylfe.cn

glob("dir/*.php");  scandir("dir");
来源：http://yeq.chenzaomai.com

[U65] PHP：会话
来源：http://duq.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kpn.tian-w.cn

[U66] PHP：设置 Cookie
来源：http://fkg.tanke756.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xjw.cheryme.top

[U67] PHP：处理文件上传
来源：http://lks.cdnleiting.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pql.gogol.net.cn

[U68] PHP：PDO 连接
来源：http://rxd.xuetiantiany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pyf.bbcook.cn

[U69] PHP：PDO 预处理
来源：http://xiv.gaohongyu789.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xsw.iojbl.cn

[U70] PHP：PDO 事务
来源：http://mvt.daxiang520.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://buj.bjfxy.top

[U71] PHP：抛出异常
来源：http://tnz.tanke756.top

throw new RuntimeException("失败", 500);
来源：http://udl.hfpthk.cn

[U72] PHP：写错误日志
来源：http://gto.ehwqpu.com

error_log("失败: " . $e->getMessage());
来源：http://ckt.shanyushiyangkeji.top

[U73] PHP：读取 ini 配置
来源：http://roc.ehwqpu.com

parse_ini_file("config.ini", true)
来源：http://mxo.chenlongwang.top

[U74] PHP：读取环境变量
来源：http://gpz.wangdashe.top

getenv("APP_ENV") ?: "production"
来源：http://shz.ehwqpu.com

[U75] PHP：依赖注入
来源：http://jfk.nanxuanxn.top

composer require psr/container
来源：http://ngf.fzhhl.top

[U76] PHP：简单路由
来源：http://xtd.yvedp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hwl.hnqzz.top

[U77] PHP：模板渲染
来源：http://jgb.wangdashe.top

composer require twig/twig
来源：http://ivw.fehbvm.com

[U78] PHP：单元测试
来源：http://gti.fehbvm.com

composer require --dev phpunit/phpunit
来源：http://ket.52xcode.cn

[U79] PHP：静态分析
来源：http://tco.52xcode.cn

composer require --dev phpstan/phpstan
来源：http://gon.ywan-chungtsiang.top

[U80] PHP：代码规范修复
来源：http://xrr.ivvv.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qpz.smart0.xyz

[U81] JS：初始化项目
来源：http://wio.nwbrower.top

npm init -y;  npm i express
来源：http://zzx.andypj.xyz

[U82] JS：package.json 脚本
来源：http://tme.gogol.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jao.aibaodan.cn

[U83] JS：ES Module 导入导出
来源：http://lpt.dianchejie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zse.gotoacloud.top

[U84] JS：CommonJS 写法
来源：http://arn.hnxiangtu.top

module.exports = { a };  const { a } = require("./m");
来源：http://wct.sxryk.cn

[U85] JS：可选链
来源：http://lnn.nwbrower.top

a?.b?.c
来源：http://gvs.chenzaomai.com

[U86] JS：空值合并
来源：http://efd.zhaomingkeji.xyz

a ?? b
来源：http://yym.zhijiandao.cn

[U87] JS：解构默认值
来源：http://aue.jiagoushi.top

const { a = 1, b = 2 } = obj;
来源：http://kue.daxiang520.top

[U88] JS：对象展开合并
来源：http://khq.hammf.cn

{ ...a, ...b }
来源：http://mac.xinyue.icu

[U89] JS：数组去重
来源：http://bzu.yvedp.cn

[...new Set(arr)]
来源：http://pgk.feifeiyinyue.top

[U90] JS：数字数组排序
来源：http://nvy.ppjwa.cn

[...arr].sort((a, b) => a - b)
来源：http://rml.ctjpmb.com

[U91] JS：对象键值遍历
来源：http://oat.hnxiangtu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sqq.zhoulong.xyz

[U92] JS：深拷贝
来源：http://fai.ivvv.top

structuredClone(obj)
来源：http://qau.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://uwi.c1oappe.top

`共 ${n} 条`
来源：http://orw.hesvh.cn

[U94] JS：箭头函数
来源：http://zae.aizwys.cn

const double = x => x * 2;
来源：http://foa.zhijiandao.cn

[U95] JS：Promise 包装
来源：http://ubo.wangshuangyany.cn

new Promise((resolve, reject) => {})
来源：http://tdw.sysykeji.top

[U96] JS：async/await 与异常
来源：http://uke.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bxq.nanxuanxn.top

[U97] JS：并发请求
来源：http://gim.jqgufenzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://smy.gaohongyu789.top

[U98] JS：fetch 带 JSON
来源：http://ozv.zycfv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iwu.cucudq.cn

[U99] JS：事件监听
来源：http://gmt.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://otv.nanxinkj.top

[U100] JS：DOM 查询
来源：http://ddq.aibaodan.cn

document.querySelector(".item")
来源：http://ixl.gzhubu.top

[U101] JS：classList 操作
来源：http://flu.andypj.xyz

el.classList.toggle("active")
来源：http://zvm.bjfxy.top

[U102] JS：本地存储
来源：http://wmp.daxiang520.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kae.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://sju.aibaodan.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yhd.guowangkeji.top

[U104] JS：防抖
来源：http://amn.smart0.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hmr.havefunace.top

[U105] JS：节流
来源：http://rac.fehbvm.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ybf.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://hxe.aibaodan.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bgl.redwolf501.top

[U107] JS：数字千分位
来源：http://jge.hammf.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lfk.fehbvm.com

[U108] JS：随机整数
来源：http://jlz.ywan-chungtsiang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jke.shanyushiyangkeji.top

[U109] JS：数组分组
来源：http://wrj.shangyingyoupin.top

Object.groupBy(arr, x => x.type)
来源：http://suq.nanxuanxn.top

[U110] JS：数组分块
来源：http://yiv.jyoumei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wux.svipenyu.cn

[U111] JS：对象转 Map
来源：http://jug.yanxiufei.cn

new Map(Object.entries(obj))
来源：http://wje.nwbrower.top

[U112] JS：字符串补位
来源：http://pph.fengsongda.top

"7".padStart(3, "0")
来源：http://nxx.hywenlv.cn

[U113] JS：正则替换全部
来源：http://ypf.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://itl.chenjidiqi.icu

[U114] JS：JSON 深比较
来源：http://uzt.nanxinkj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ajl.yueranfly.top

[U115] JS：生成 UUID
来源：http://mvv.andypj.xyz

crypto.randomUUID()
来源：http://toa.haohaochexian.top

[U116] JS：类型检查（JSDoc）
来源：http://ysp.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://gnl.zdqjudy.top

[U117] JS：单元测试
来源：http://rhf.pycfn.com

npm i -D vitest;  npx vitest
来源：http://sso.gzhubu.top

[U118] JS：开发服务器
来源：http://bnv.yuanzhike.top

npm i -D vite;  npx vite
来源：http://wxo.chenjidiqi.icu

[U119] JS：生产构建
来源：http://uhu.shzxlz.cn

npx vite build
来源：http://pen.yanxiufei.cn

[U120] JS：读取环境变量（Vite）
来源：http://cpw.jqgfzy.top

import.meta.env.VITE_API_URL
来源：http://qnn.xuanzx.com

================================================================================
来源：http://xnf.meibo888.top

统计汇总
来源：http://oyf.jinyuanbaomall.cn

================================================================================
来源：http://rhd.cheryme.top

按语言统计（条）：
来源：http://mcr.zhoulong.xyz

Python ......... 252
来源：http://bcp.zdbjq.cn

PHP ............ 252
来源：http://ong.ybcxt.top

JavaScript ..... 252
来源：http://fzd.ydjk.org.cn

TypeScript ..... 212
来源：http://cbd.tianlin.xyz

Java ........... 212
来源：http://abt.zhoulong.xyz

Go ............. 212
来源：http://rje.meibo888.top

Ruby ........... 212
来源：http://uoq.hesvh.cn

C# ............. 212
来源：http://tox.zhengqikj.top

C .............. 30
来源：http://viz.xingfuxueyuan.xyz

C++ ............ 30
来源：http://lgz.gotoacloud.top

SQL ............ 90
来源：http://owh.zhijiandao.cn

Bash ........... 80
来源：http://sdn.shzxlz.cn

Kotlin ......... 15
来源：http://drg.316326.xyz

Swift .......... 15
来源：http://ngj.sweek.top

Lua ............ 10
来源：http://mtk.jinqigfzy.top

Perl ........... 10
来源：http://upw.gotoacloud.top

Scala .......... 10
来源：http://dmv.hfpthk.cn

------------------------------------
来源：http://dhx.jianghu66.top

合计 ........... 2106 条
来源：http://sav.tian-w.cn

按章节统计：
来源：http://gzd.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hms.gotoacloud.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qkh.ivvv.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pfl.xuanzx.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://odo.ivvv.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ipa.mhx1999.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qxs.yongpay.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qif.chenzaomai.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oul.ywan-chungtsiang.top


<!-- 参考信息 -->