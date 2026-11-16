代发 wailian999

[U15] Py：高精度计时
来源：http://nxm.hywenlv.cn

t = time.perf_counter()
来源：http://ern.fanxiaobao.xyz

[U16] Py：命令行参数解析
来源：http://hda.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ftk.sxryk.cn

[U17] Py：初始化日志
来源：http://pyc.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://zoz.tianlin.xyz

[U18] Py：预编译正则
来源：http://exx.9152youxi.cn

pat = re.compile(r"\d+")
来源：http://bgy.chenzaomai.com

[U19] Py：正则替换带回调
来源：http://rcb.guannengcc.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://heg.svipenyu.cn

[U20] Py：缓存函数结果
来源：http://shp.nwbrower.top

@functools.lru_cache(maxsize=None)
来源：http://cuq.bjfxy.top

[U21] Py：自定义上下文管理器
来源：http://gaj.kuanghao11.cn

@contextlib.contextmanager
来源：http://nya.shzxlz.cn

[U22] Py：矩阵转置
来源：http://eor.zhengqikj.top

list(zip(*m))
来源：http://jxy.jinyuanbaomall.cn

[U23] Py：分块读取大文件
来源：http://brl.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oyl.yanxiufei.cn

[U24] Py：路径操作
来源：http://aif.shzxlz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://goo.sxryk.cn

[U25] Py：CSV 按字典读
来源：http://slp.zhoulong.xyz

csv.DictReader(f)
来源：http://rij.hfpthk.cn

[U26] Py：并发下载
来源：http://ahz.ywan-chungtsiang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lfn.feifeiyinyue.top

[U27] Py：异步 HTTP
来源：http://ayk.cqqwz.cn

aiohttp.ClientSession() 配合 async with
来源：http://ucp.316326.xyz

[U28] Py：类型别名
来源：http://joe.bjfxy.top

UserId = int
来源：http://rgw.cqqwz.cn

[U29] Py：属性校验
来源：http://zec.meibo888.top

@property 与 @x.setter 配合
来源：http://ioc.9152youxi.cn

[U30] Py：数据类
来源：http://kua.gogol.net.cn

@dataclass(slots=True)
来源：http://hnf.hysaishi.cn

[U31] Py：单测
来源：http://ztz.cheryme.top

python -m pytest -q
来源：http://ppo.gotoacloud.top

[U32] Py：代码格式化
来源：http://uky.nanxuanxn.top

ruff format . && ruff check --fix .
来源：http://ixv.gogol.net.cn

[U33] Py：打包发布
来源：http://wjj.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://ymp.ivvv.top

[U34] Py：判断编码
来源：http://egl.cqqwz.cn

chardet.detect(raw)
来源：http://wby.chenzaomai.com

[U35] Py：发送邮件
来源：http://pfu.guowangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pfl.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://uwx.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://ouk.9152youxi.cn

[U37] Py：读写 Excel
来源：http://bit.ivvv.top

pandas.read_excel / DataFrame.to_excel
来源：http://sif.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://otq.0kj1m.cn

Path(__file__).resolve().parent
来源：http://yvn.aibaodan.cn

[U39] Py：判断是否在交互环境
来源：http://wnq.wangdashe.top

sys.stdout.isatty()
来源：http://jcs.xziqi.cn

[U40] Py：打印到标准错误
来源：http://iib.fzhhl.top

print("err", file=sys.stderr)
来源：http://ths.hongshengwenyu.top

[U41] PHP：初始化 Composer 项目
来源：http://hxq.jyoumei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qon.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://tik.chenlongwang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mkm.cqqwz.cn

[U43] PHP：声明命名空间
来源：http://sca.fzhhl.top

namespace App\Http;
来源：http://hlx.yuxming.cn

[U44] PHP：开启严格类型
来源：http://gne.ybcxt.top

declare(strict_types=1);
来源：http://nej.zhiwuduotai.top

[U45] PHP：类型声明与返回类型
来源：http://ahs.jqgfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qnv.zhengqikj.top

[U46] PHP：可空类型
来源：http://kkn.sysykeji.top

?string $name = null
来源：http://uyf.nwbrower.top

[U47] PHP：联合类型
来源：http://ilu.hysaishi.cn

int|string $id
来源：http://igx.gzhubu.top

[U48] PHP：纯枚举
来源：http://dgl.gaohongyu789.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mzy.ppjwa.cn

[U49] PHP：只读属性
来源：http://ubv.xuetiantiany.cn

public readonly string $name
来源：http://ggw.yanxiufei.cn

[U50] PHP：构造器属性提升
来源：http://jma.tarul.cn

public function __construct(private int $id) {}
来源：http://llk.cashguo.top

[U51] PHP：数组解构
来源：http://fpj.zhongyouzk.top

[$a, $b] = $arr;
来源：http://nuz.meibo888.top

[U52] PHP：箭头函数
来源：http://qrl.shanyushiyangtech.top

$double = fn($x) => $x * 2;
来源：http://uqm.havefunace.top

[U53] PHP：空合并运算符
来源：http://kna.shzxlz.cn

$v = $a ?? $b ?? "default";
来源：http://hev.yuxming.cn

[U54] PHP：空安全调用
来源：http://xzp.hnqzz.top

$obj?->method()
来源：http://kyt.mhx1999.top

[U55] PHP：match 表达式
来源：http://uvz.redwolf501.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yge.zdqjudy.top

[U56] PHP：命名参数
来源：http://yom.ivvv.top

f(a: 1, b: 2)
来源：http://jux.chenjidiqi.icu

[U57] PHP：字符串插值
来源：http://wap.sxryk.cn

"值: {$a}"
来源：http://lcc.jinyuanbaomall.cn

[U58] PHP：数组三件套
来源：http://iwp.tarul.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://brv.xuetiantiany.cn

[U59] PHP：自定义排序
来源：http://nke.dianchejie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://idx.havefunace.top

[U60] PHP：JSON 编解码
来源：http://nnx.zhaomingkeji.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lny.vehdjk.com

[U61] PHP：正则
来源：http://xhp.cqqwz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eyq.ppjwa.cn

[U62] PHP：日期对象
来源：http://rww.yueranfly.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iou.zdbjq.cn

[U63] PHP：文件读写
来源：http://rsz.fehbvm.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kru.yangfankeji.com

[U64] PHP：目录遍历
来源：http://osg.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://qxc.yfazqb.com

[U65] PHP：会话
来源：http://kdn.hesvh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://erh.zhijiandao.cn

[U66] PHP：设置 Cookie
来源：http://gaq.hywenlv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rks.birdmap.top

[U67] PHP：处理文件上传
来源：http://gvw.gotoacloud.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lde.hcnkem.com

[U68] PHP：PDO 连接
来源：http://pfd.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sda.ydjk.org.cn

[U69] PHP：PDO 预处理
来源：http://dor.sweek.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oxr.316326.xyz

[U70] PHP：PDO 事务
来源：http://tvt.zhongyouzk.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aks.sxryk.cn

[U71] PHP：抛出异常
来源：http://irw.smart0.xyz

throw new RuntimeException("失败", 500);
来源：http://xph.zdqjudy.top

[U72] PHP：写错误日志
来源：http://hex.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://dbn.xuetiantiany.cn

[U73] PHP：读取 ini 配置
来源：http://qur.wangdashe.top

parse_ini_file("config.ini", true)
来源：http://phx.gzhubu.top

[U74] PHP：读取环境变量
来源：http://jzm.ydzc1.top

getenv("APP_ENV") ?: "production"
来源：http://wmk.sweek.top

[U75] PHP：依赖注入
来源：http://goa.kuanghao11.cn

composer require psr/container
来源：http://swg.zhoulong.xyz

[U76] PHP：简单路由
来源：http://zsv.fzhhl.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lzh.yfazqb.com

[U77] PHP：模板渲染
来源：http://hby.yj20258888.top

composer require twig/twig
来源：http://suv.gotoacloud.top

[U78] PHP：单元测试
来源：http://apu.cashguo.top

composer require --dev phpunit/phpunit
来源：http://fvh.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://iai.zhaomingkeji.xyz

composer require --dev phpstan/phpstan
来源：http://lkc.yongpay.top

[U80] PHP：代码规范修复
来源：http://tlm.ybcxt.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://kxl.sysykeji.top

[U81] JS：初始化项目
来源：http://xgl.shuidangran.top

npm init -y;  npm i express
来源：http://nil.vehdjk.com

[U82] JS：package.json 脚本
来源：http://rqf.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jmb.sxryk.cn

[U83] JS：ES Module 导入导出
来源：http://xbs.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://qry.jinqigfzy.top

[U84] JS：CommonJS 写法
来源：http://mws.ywan-chungtsiang.top

module.exports = { a };  const { a } = require("./m");
来源：http://wmw.yangfankeji.com

[U85] JS：可选链
来源：http://arb.sysykeji.top

a?.b?.c
来源：http://sli.daxiang520.top

[U86] JS：空值合并
来源：http://cgt.hfpthk.cn

a ?? b
来源：http://viq.zhiwuduotai.top

[U87] JS：解构默认值
来源：http://saw.aibaodan.cn

const { a = 1, b = 2 } = obj;
来源：http://xlx.meibo888.top

[U88] JS：对象展开合并
来源：http://feu.52xcode.cn

{ ...a, ...b }
来源：http://uxo.uphjek.com

[U89] JS：数组去重
来源：http://apd.zdbjq.cn

[...new Set(arr)]
来源：http://vjy.yfazqb.com

[U90] JS：数字数组排序
来源：http://utc.ydzc1.top

[...arr].sort((a, b) => a - b)
来源：http://erx.gogol.net.cn

[U91] JS：对象键值遍历
来源：http://eca.pycfn.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://axj.hnqzz.top

[U92] JS：深拷贝
来源：http://hsr.hammf.cn

structuredClone(obj)
来源：http://qrj.tianlin.xyz

[U93] JS：模板字符串
来源：http://lqa.hcnkem.com

`共 ${n} 条`
来源：http://uej.jiagoushi.top

[U94] JS：箭头函数
来源：http://gdp.quarkkingdee.top

const double = x => x * 2;
来源：http://fvp.cqqwz.cn

[U95] JS：Promise 包装
来源：http://imy.ydzc1.top

new Promise((resolve, reject) => {})
来源：http://qgz.jianghu66.top

[U96] JS：async/await 与异常
来源：http://vyj.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tfh.vqdsnc.cn

[U97] JS：并发请求
来源：http://rqp.gzhubu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jlj.nanxuanxn.top

[U98] JS：fetch 带 JSON
来源：http://mmm.jqgufenzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xow.gotoacloud.top

[U99] JS：事件监听
来源：http://ljh.cashguo.top

el.addEventListener("click", e => {})
来源：http://fib.guannengcc.top

[U100] JS：DOM 查询
来源：http://ais.yj202588.top

document.querySelector(".item")
来源：http://srm.jinqigfzy.top

[U101] JS：classList 操作
来源：http://vlq.52xcode.cn

el.classList.toggle("active")
来源：http://fsf.vehdjk.com

[U102] JS：本地存储
来源：http://vkg.zhoulong.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://dkd.ctjpmb.com

[U103] JS：定时器
来源：http://cmt.yangfankeji.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bdn.pengpengdd.cyou

[U104] JS：防抖
来源：http://wty.daria6918.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://asz.tarul.cn

[U105] JS：节流
来源：http://kcm.yuanzhike.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zxu.zhaomingkeji.xyz

[U106] JS：日期格式化
来源：http://dfi.sysykeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dhg.tanke756.top

[U107] JS：数字千分位
来源：http://prq.nanxuanxn.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eql.quarkkingdee.top

[U108] JS：随机整数
来源：http://uah.yonumen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://khq.wangshuangyany.cn

[U109] JS：数组分组
来源：http://hcw.yj20258.top

Object.groupBy(arr, x => x.type)
来源：http://puc.pycfn.com

[U110] JS：数组分块
来源：http://cox.ppjwa.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cal.yvedp.cn

[U111] JS：对象转 Map
来源：http://rho.quarkkingdee.top

new Map(Object.entries(obj))
来源：http://ecu.yanxiufei.cn

[U112] JS：字符串补位
来源：http://fqh.snrcjt.cn

"7".padStart(3, "0")
来源：http://yal.shanyushiyangtech.top

[U113] JS：正则替换全部
来源：http://les.zycfv.cn

s.replaceAll("a", "b")
来源：http://bbx.316326.xyz

[U114] JS：JSON 深比较
来源：http://hlz.chenlongwang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lql.yueranfly.top

[U115] JS：生成 UUID
来源：http://mrl.epnwcf.com

crypto.randomUUID()
来源：http://bkc.dashuyun.cn

[U116] JS：类型检查（JSDoc）
来源：http://oua.dashuyun.cn

/** @param {string} name */ function f(name) {}
来源：http://qkx.fzhhl.top

[U117] JS：单元测试
来源：http://xpn.shzxlz.cn

npm i -D vitest;  npx vitest
来源：http://avj.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://zdl.yj202588.top

npm i -D vite;  npx vite
来源：http://bvh.hfpthk.cn

[U119] JS：生产构建
来源：http://trd.yuxming.cn

npx vite build
来源：http://qbj.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://qmh.mhx1999.top

import.meta.env.VITE_API_URL
来源：http://xka.zhongyouzk.top

================================================================================
来源：http://zeb.jinqigufen.top

统计汇总
来源：http://uvm.sjlbkw.cn

================================================================================
来源：http://uzh.nanxinkj.top

按语言统计（条）：
来源：http://cwm.xziqi.cn

Python ......... 252
来源：http://hhw.aibaodan.cn

PHP ............ 252
来源：http://sxz.shangyingyoupin.top

JavaScript ..... 252
来源：http://gwb.vehdjk.com

TypeScript ..... 212
来源：http://oxs.sysykeji.top

Java ........... 212
来源：http://rxb.hammf.cn

Go ............. 212
来源：http://vwd.0kj1m.cn

Ruby ........... 212
来源：http://zgy.nanxuanxn.top

C# ............. 212
来源：http://nwl.zhijiandao.cn

C .............. 30
来源：http://eby.jinqigfzy.top

C++ ............ 30
来源：http://dvl.tian-w.cn

SQL ............ 90
来源：http://fpt.ydjk.org.cn

Bash ........... 80
来源：http://yao.ybcxt.top

Kotlin ......... 15
来源：http://drp.sjlbkw.cn

Swift .......... 15
来源：http://cqy.snrcjt.cn

Lua ............ 10
来源：http://bez.andypj.xyz

Perl ........... 10
来源：http://kvw.jlsjyb.cn

Scala .......... 10
来源：http://gsb.redwolf501.top

------------------------------------
来源：http://cdb.shzxlz.cn

合计 ........... 2106 条
来源：http://dmd.iojbl.cn

按章节统计：
来源：http://sha.ybcxt.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://azn.svipenyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ovc.yj20258888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zlc.chenzaomai.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cnw.aizwys.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://acj.shangyingyoupin.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nbn.yangfankeji.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nxv.shangyingyoupin.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ktd.yangfankeji.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://erq.zhiwuduotai.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sjn.jyoumei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://net.yonumen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mgg.yuanzhike.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nak.jlsjyb.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xhz.fehbvm.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://huo.tarul.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pxo.svipenyu.cn

Q SQL 专题                              90
来源：http://aiq.xingfuxueyuan.xyz

R Bash 专题                             80
来源：http://mfd.gotoacloud.top

S C / C++ 专题                          60
来源：http://hkm.yueranfly.top

T 其他语言补充                          60
来源：http://wol.nanxuanxn.top

U 高频实用片段                         120
来源：http://khj.hnxiangtu.top

------------------------------------
来源：http://zep.fanxiaobao.xyz

合计                                  2106 条
来源：http://itv.daria6918.cn

--------------------------------------------------------------------------------
来源：http://qyx.zhixingplan.top

使用提醒
来源：http://qjn.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://xhz.shangyingyoupin.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fag.fehbvm.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eui.guannengcc.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zvl.haohaochexian.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ucr.quarkkingdee.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rwn.hongshengwenyu.top

—— 文件结束 ——
来源：http://mfj.hnxiangtu.top

================================================================================
来源：http://ofz.vehdjk.com

程序语言常见例子速查手册（2024 版）
来源：http://tva.mhx1999.top

Common Programming Examples Cheat Book
来源：http://nia.havefunace.top

================================================================================
来源：http://ahv.fzhhl.top

【收录内容】
来源：http://ykr.hongshengwenyu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://scs.shanyushiyangtech.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jcc.shanyushiyangtech.top

SQL · Bash · C · C++
来源：http://bkk.guannengcc.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bcd.cashguo.top

【使用说明】
来源：http://zqu.52xcode.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nek.shanyushiyangtech.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xdi.cqqwz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tpc.feifeiyinyue.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tat.haohaochexian.top

Bash:  Shell         C:     C             C++:   C++
来源：http://yfp.ctjpmb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://szx.ywan-chungtsiang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://etb.52xcode.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jdp.hywenlv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mde.sjlbkw.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vse.hammf.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wph.daxiang520.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hsn.zhengqikj.top

【文件统计】
来源：http://cbf.fktsv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wpp.sweek.top

--------------------------------------------------------------------------------
来源：http://mml.iojbl.cn

目  录
来源：http://uor.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://zyu.jqgfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://poe.hammf.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://win.jinqigufen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jzu.fzhhl.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wod.zdbjq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oqg.cheryme.top


<!-- 参考信息 -->