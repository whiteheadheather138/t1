代发 wailian999

case class User(name: String, age: Int)
来源：http://kel.hnxiangtu.top

[T57] Scala：模式匹配
来源：http://scl.hcnkem.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://eks.zycfv.cn

[T58] Scala：函数定义
来源：http://xca.hammf.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kcb.sxryk.cn

[T59] Scala：循环
来源：http://dww.zycfv.cn

for (i <- 1 to 10) println(i)
来源：http://odf.shanyushiyangkeji.top

[T60] Scala：折叠
来源：http://bka.hcnkem.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://swx.redwolf501.top

================================================================================
来源：http://qmd.xuanzx.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://eub.yj20258888.top

================================================================================
来源：http://ssx.tian-w.cn

[U01] Py：创建虚拟环境
来源：http://oom.daxiang520.top

python -m venv .venv && source .venv/bin/activate
来源：http://ynd.fzhhl.top

[U02] Py：导出 / 安装依赖
来源：http://gxx.gaohongyu789.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sya.9152youxi.cn

[U03] Py：加载 .env 配置
来源：http://kya.snrcjt.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hxm.yueranfly.top

[U04] Py：变量调试打印
来源：http://iac.aizwys.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oii.sufxvd.cn

[U05] Py：列表去重且保序
来源：http://xka.yangfankeji.com

list(dict.fromkeys(arr))
来源：http://aei.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://via.andypj.xyz

{**a, **b}
来源：http://otx.wangshuangyany.cn

[U07] Py：反转字典键值
来源：http://vdt.xziqi.cn

{v: k for k, v in d.items()}
来源：http://cto.0kj1m.cn

[U08] Py：展平二维列表
来源：http://mnd.zhiwuduotai.top

[y for x in nested for y in x]
来源：http://vzy.pycfn.com

[U09] Py：字典取最大值的键
来源：http://nck.fanxiaobao.xyz

max(d, key=d.get)
来源：http://ypi.pengpengdd.cyou

[U10] Py：按值排序字典
来源：http://wov.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qlt.epnwcf.com

[U11] Py：生成器表达式
来源：http://vsa.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://bcb.vehdjk.com

[U12] Py：取出现最多的 3 个元素
来源：http://lny.uphjek.com

Counter(arr).most_common(3)
来源：http://amp.cashguo.top

[U13] Py：固定长度队列
来源：http://dja.hcnkem.com

deque(maxlen=10)
来源：http://cnd.dianchejie.cn

[U14] Py：分组收集到列表
来源：http://kds.sjlbkw.cn

defaultdict(list)
来源：http://dwm.zhixingplan.top

[U15] Py：高精度计时
来源：http://geb.haohaochexian.top

t = time.perf_counter()
来源：http://fba.feifeiyinyue.top

[U16] Py：命令行参数解析
来源：http://tos.ivvv.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sjj.fktsv.cn

[U17] Py：初始化日志
来源：http://cep.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://qbd.feifeiyinyue.top

[U18] Py：预编译正则
来源：http://hlm.jiagoushi.top

pat = re.compile(r"\d+")
来源：http://qrb.pengpengdd.cyou

[U19] Py：正则替换带回调
来源：http://gpr.zdbjq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://elk.fzhhl.top

[U20] Py：缓存函数结果
来源：http://gft.ehwqpu.com

@functools.lru_cache(maxsize=None)
来源：http://lhi.dashuyun.cn

[U21] Py：自定义上下文管理器
来源：http://xpy.bbcook.cn

@contextlib.contextmanager
来源：http://iiu.zhongyouzk.top

[U22] Py：矩阵转置
来源：http://nre.uphjek.com

list(zip(*m))
来源：http://iza.yuxming.cn

[U23] Py：分块读取大文件
来源：http://deq.dashuyun.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qco.hysaishi.cn

[U24] Py：路径操作
来源：http://hge.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nsz.cashguo.top

[U25] Py：CSV 按字典读
来源：http://ryz.smart0.xyz

csv.DictReader(f)
来源：http://jue.aibaodan.cn

[U26] Py：并发下载
来源：http://npu.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ejw.fehbvm.com

[U27] Py：异步 HTTP
来源：http://cex.vehdjk.com

aiohttp.ClientSession() 配合 async with
来源：http://gxb.havefunace.top

[U28] Py：类型别名
来源：http://ykf.jianghu66.top

UserId = int
来源：http://vjx.bbcook.cn

[U29] Py：属性校验
来源：http://tyt.jianghu66.top

@property 与 @x.setter 配合
来源：http://mam.jinghuilouyu.cn

[U30] Py：数据类
来源：http://rax.zhoulong.xyz

@dataclass(slots=True)
来源：http://fqu.sxryk.cn

[U31] Py：单测
来源：http://hcw.zhengqikj.top

python -m pytest -q
来源：http://lio.tanke756.top

[U32] Py：代码格式化
来源：http://mfp.xuanzx.com

ruff format . && ruff check --fix .
来源：http://wdk.ydjk.org.cn

[U33] Py：打包发布
来源：http://jda.hysaishi.cn

python -m build  （依赖 pyproject.toml）
来源：http://fwy.uphjek.com

[U34] Py：判断编码
来源：http://cjw.ppjwa.cn

chardet.detect(raw)
来源：http://sye.daria6918.cn

[U35] Py：发送邮件
来源：http://pwt.tanke756.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ncz.yongpay.top

[U36] Py：定时任务
来源：http://drx.jqgfzy.top

schedule.every(10).minutes.do(job)
来源：http://bcx.fzhhl.top

[U37] Py：读写 Excel
来源：http://qny.shanyushiyangtech.top

pandas.read_excel / DataFrame.to_excel
来源：http://xqh.hnqzz.top

[U38] Py：获取脚本所在目录
来源：http://yqy.yj20258888.top

Path(__file__).resolve().parent
来源：http://eix.kuanghao11.cn

[U39] Py：判断是否在交互环境
来源：http://aqy.tian-w.cn

sys.stdout.isatty()
来源：http://jso.wangshuangyany.cn

[U40] Py：打印到标准错误
来源：http://nse.ppjwa.cn

print("err", file=sys.stderr)
来源：http://gqb.tanke756.top

[U41] PHP：初始化 Composer 项目
来源：http://nxb.epnwcf.com

composer init;  composer require guzzlehttp/guzzle
来源：http://dxt.sysykeji.top

[U42] PHP：PSR-4 自动加载
来源：http://dxp.nanxinkj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lbx.shzxlz.cn

[U43] PHP：声明命名空间
来源：http://tqf.zhiwuduotai.top

namespace App\Http;
来源：http://pxv.hywenlv.cn

[U44] PHP：开启严格类型
来源：http://mul.gaohongyu789.top

declare(strict_types=1);
来源：http://wvo.yanxiufei.cn

[U45] PHP：类型声明与返回类型
来源：http://zld.jinyuanbaomall.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qws.yangfankeji.com

[U46] PHP：可空类型
来源：http://kml.cdnleiting.top

?string $name = null
来源：http://iqa.zhengqikj.top

[U47] PHP：联合类型
来源：http://mmn.zycfv.cn

int|string $id
来源：http://dnv.hywenlv.cn

[U48] PHP：纯枚举
来源：http://pqf.cdnleiting.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cir.jinqigufen.top

[U49] PHP：只读属性
来源：http://oih.jyoumei.cn

public readonly string $name
来源：http://bci.ehwqpu.com

[U50] PHP：构造器属性提升
来源：http://ctm.316326.xyz

public function __construct(private int $id) {}
来源：http://niy.fktsv.cn

[U51] PHP：数组解构
来源：http://kai.tanke756.top

[$a, $b] = $arr;
来源：http://pvq.hfpthk.cn

[U52] PHP：箭头函数
来源：http://gee.xylfe.cn

$double = fn($x) => $x * 2;
来源：http://aas.jqgufenzy.top

[U53] PHP：空合并运算符
来源：http://jmo.xinyue.icu

$v = $a ?? $b ?? "default";
来源：http://lxn.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://wtj.jyoumei.cn

$obj?->method()
来源：http://lqq.bbcook.cn

[U55] PHP：match 表达式
来源：http://ngv.andypj.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kwy.shanyushiyangkeji.top

[U56] PHP：命名参数
来源：http://ptr.sxryk.cn

f(a: 1, b: 2)
来源：http://xjr.yanxiufei.cn

[U57] PHP：字符串插值
来源：http://rbv.aibaodan.cn

"值: {$a}"
来源：http://efs.ywan-chungtsiang.top

[U58] PHP：数组三件套
来源：http://ebp.hcnkem.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cuj.aibaodan.cn

[U59] PHP：自定义排序
来源：http://bww.zhaomingkeji.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://klm.yangfankeji.com

[U60] PHP：JSON 编解码
来源：http://col.zhoulong.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ufz.bjfxy.top

[U61] PHP：正则
来源：http://ust.vehdjk.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vig.daxiang520.top

[U62] PHP：日期对象
来源：http://btb.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://isc.hywenlv.cn

[U63] PHP：文件读写
来源：http://xhb.cheryme.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dhx.mhx1999.top

[U64] PHP：目录遍历
来源：http://ado.sjlbkw.cn

glob("dir/*.php");  scandir("dir");
来源：http://fzp.haohaochexian.top

[U65] PHP：会话
来源：http://mht.ppjwa.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sgh.yvedp.cn

[U66] PHP：设置 Cookie
来源：http://gae.cqqwz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hur.shanyushiyangkeji.top

[U67] PHP：处理文件上传
来源：http://fsa.nanxuanxn.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jwa.chenzaomai.com

[U68] PHP：PDO 连接
来源：http://viv.kuanghao11.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://flc.zdbjq.cn

[U69] PHP：PDO 预处理
来源：http://zmt.jlsjyb.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uez.ehwqpu.com

[U70] PHP：PDO 事务
来源：http://aiw.yj202588.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bwf.fanxiaobao.xyz

[U71] PHP：抛出异常
来源：http://kah.9152youxi.cn

throw new RuntimeException("失败", 500);
来源：http://qpx.yuanzhike.top

[U72] PHP：写错误日志
来源：http://ndf.epnwcf.com

error_log("失败: " . $e->getMessage());
来源：http://tig.fanxiaobao.xyz

[U73] PHP：读取 ini 配置
来源：http://xtj.bjfxy.top

parse_ini_file("config.ini", true)
来源：http://nyz.jlsjyb.cn

[U74] PHP：读取环境变量
来源：http://bow.9152youxi.cn

getenv("APP_ENV") ?: "production"
来源：http://hpc.havefunace.top

[U75] PHP：依赖注入
来源：http://lse.hnqzz.top

composer require psr/container
来源：http://ukg.epnwcf.com

[U76] PHP：简单路由
来源：http://qcp.cqqwz.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xlp.jianghu66.top

[U77] PHP：模板渲染
来源：http://cmr.daxiang520.top

composer require twig/twig
来源：http://doh.zhoulong.xyz

[U78] PHP：单元测试
来源：http://yvl.yj20258888.top

composer require --dev phpunit/phpunit
来源：http://lny.ydzc1.top

[U79] PHP：静态分析
来源：http://pgc.cashguo.top

composer require --dev phpstan/phpstan
来源：http://aoa.c1oappe.top

[U80] PHP：代码规范修复
来源：http://ttu.jiagoushi.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://irm.shzxlz.cn

[U81] JS：初始化项目
来源：http://stn.xuetiantiany.cn

npm init -y;  npm i express
来源：http://cos.yj20258.top

[U82] JS：package.json 脚本
来源：http://bgh.shanyushiyangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cuj.quarkkingdee.top

[U83] JS：ES Module 导入导出
来源：http://dfj.jyoumei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ouv.gaohongyu789.top

[U84] JS：CommonJS 写法
来源：http://yki.gogol.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rmf.snrcjt.cn

[U85] JS：可选链
来源：http://tte.bjfxy.top

a?.b?.c
来源：http://kft.sweek.top

[U86] JS：空值合并
来源：http://qzw.nanxinkj.top

a ?? b
来源：http://ezq.316326.xyz

[U87] JS：解构默认值
来源：http://xec.gotoacloud.top

const { a = 1, b = 2 } = obj;
来源：http://res.ivvv.top

[U88] JS：对象展开合并
来源：http://nkk.chenlongwang.top

{ ...a, ...b }
来源：http://jhl.52xcode.cn

[U89] JS：数组去重
来源：http://otc.cucudq.cn

[...new Set(arr)]
来源：http://ehk.ydzc1.top

[U90] JS：数字数组排序
来源：http://gza.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://gos.havefunace.top

[U91] JS：对象键值遍历
来源：http://jpn.wangshuangyany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qxy.yanxiufei.cn

[U92] JS：深拷贝
来源：http://fjp.birdmap.top

structuredClone(obj)
来源：http://guc.jqgufenzy.top

[U93] JS：模板字符串
来源：http://lej.zdqjudy.top

`共 ${n} 条`
来源：http://lho.chenjidiqi.icu

[U94] JS：箭头函数
来源：http://xhd.jinghuilouyu.cn

const double = x => x * 2;
来源：http://ydq.dashuyun.cn

[U95] JS：Promise 包装
来源：http://sxz.pengpengdd.cyou

new Promise((resolve, reject) => {})
来源：http://qwv.yvedp.cn

[U96] JS：async/await 与异常
来源：http://ggs.jinghuilouyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pvc.wangdashe.top

[U97] JS：并发请求
来源：http://lha.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://zxw.nanxinkj.top

[U98] JS：fetch 带 JSON
来源：http://avg.zdqjudy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eid.bjfxy.top

[U99] JS：事件监听
来源：http://wzd.jianghu66.top

el.addEventListener("click", e => {})
来源：http://cth.fengsongda.top

[U100] JS：DOM 查询
来源：http://seg.xylfe.cn

document.querySelector(".item")
来源：http://fzs.yuanzhike.top

[U101] JS：classList 操作
来源：http://ihm.ivvv.top

el.classList.toggle("active")
来源：http://nkn.ywan-chungtsiang.top

[U102] JS：本地存储
来源：http://bkf.c1oappe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://njh.jinqigufen.top

[U103] JS：定时器
来源：http://ypb.tanke756.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://imv.aizwys.cn

[U104] JS：防抖
来源：http://txl.chenzaomai.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hgc.zhijiandao.cn

[U105] JS：节流
来源：http://kvk.xingfuxueyuan.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://irl.gzhubu.top

[U106] JS：日期格式化
来源：http://afd.daria6918.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://idt.yueranfly.top

[U107] JS：数字千分位
来源：http://obz.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fcm.chenzaomai.com

[U108] JS：随机整数
来源：http://ziv.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://djt.nanxuanxn.top

[U109] JS：数组分组
来源：http://tjr.wangshuangyany.cn

Object.groupBy(arr, x => x.type)
来源：http://pfy.jinghuilouyu.cn

[U110] JS：数组分块
来源：http://gdb.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://brx.xuetiantiany.cn

[U111] JS：对象转 Map
来源：http://ypo.meibo888.top

new Map(Object.entries(obj))
来源：http://yxt.fzhhl.top

[U112] JS：字符串补位
来源：http://lsg.fktsv.cn

"7".padStart(3, "0")
来源：http://hho.ctjpmb.com

[U113] JS：正则替换全部
来源：http://npl.chenlongwang.top

s.replaceAll("a", "b")
来源：http://gnv.yuxming.cn

[U114] JS：JSON 深比较
来源：http://wlv.ehwqpu.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://cqd.dianchejie.cn

[U115] JS：生成 UUID
来源：http://tvp.kuanghao11.cn

crypto.randomUUID()
来源：http://rhz.tarul.cn

[U116] JS：类型检查（JSDoc）
来源：http://pqv.xuanzx.com

/** @param {string} name */ function f(name) {}
来源：http://mju.cqqwz.cn

[U117] JS：单元测试
来源：http://owa.andypj.xyz

npm i -D vitest;  npx vitest
来源：http://nfi.ywan-chungtsiang.top

[U118] JS：开发服务器
来源：http://pnw.cucudq.cn

npm i -D vite;  npx vite
来源：http://vsc.ybcxt.top

[U119] JS：生产构建
来源：http://bof.yj202588.top

npx vite build
来源：http://dqp.aibaodan.cn

[U120] JS：读取环境变量（Vite）
来源：http://bpn.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://yll.aizwys.cn

================================================================================
来源：http://hoo.yj202588.top

统计汇总
来源：http://qtz.zdbjq.cn

================================================================================
来源：http://uhq.iojbl.cn

按语言统计（条）：
来源：http://ujv.wangdashe.top

Python ......... 252
来源：http://sgt.fanxiaobao.xyz

PHP ............ 252
来源：http://jfl.hywenlv.cn

JavaScript ..... 252
来源：http://rhu.kuanghao11.cn

TypeScript ..... 212
来源：http://mdh.xylfe.cn

Java ........... 212
来源：http://qli.guannengcc.top

Go ............. 212
来源：http://lwq.zhijiandao.cn

Ruby ........... 212
来源：http://uet.cdnleiting.top

C# ............. 212
来源：http://ocy.ivvv.top

C .............. 30
来源：http://vcs.chenlongwang.top

C++ ............ 30
来源：http://kvq.wangshuangyany.cn

SQL ............ 90
来源：http://flb.mhx1999.top

Bash ........... 80
来源：http://tqv.jinghuilouyu.cn

Kotlin ......... 15
来源：http://ciy.zhoulong.xyz

Swift .......... 15
来源：http://nxp.c1oappe.top

Lua ............ 10
来源：http://lts.chenzaomai.com

Perl ........... 10
来源：http://mls.sufxvd.cn

Scala .......... 10
来源：http://qmr.jinyuanbaomall.cn

------------------------------------
来源：http://gmx.hongshengwenyu.top

合计 ........... 2106 条
来源：http://fme.zhengqikj.top

按章节统计：
来源：http://tlg.yuxming.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://idn.jinghuilouyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hvi.zhijiandao.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mvc.cqqwz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bes.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mvn.xinyue.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sut.ivvv.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wgz.sufxvd.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://raw.hnqzz.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uvc.quarkkingdee.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gun.sysykeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oua.ydjk.org.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wzg.smart0.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pmt.hongshengwenyu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bei.yueranfly.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rak.fktsv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tkv.aizwys.cn

Q SQL 专题                              90
来源：http://cue.fehbvm.com

R Bash 专题                             80
来源：http://jpr.ydzc1.top

S C / C++ 专题                          60
来源：http://mud.9152youxi.cn

T 其他语言补充                          60
来源：http://mpv.hywenlv.cn

U 高频实用片段                         120
来源：http://scd.jqgufenzy.top

------------------------------------
来源：http://usr.xuanzx.com

合计                                  2106 条
来源：http://ave.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://ouk.jinyuanbaomall.cn


<!-- 参考信息 -->