代发 wailian999

[U07] Py：反转字典键值
来源：http://lik.jinyuanbaomall.cn

{v: k for k, v in d.items()}
来源：http://jrg.zycfv.cn

[U08] Py：展平二维列表
来源：http://rzx.bjfxy.top

[y for x in nested for y in x]
来源：http://dwq.zdqjudy.top

[U09] Py：字典取最大值的键
来源：http://dkl.zhiwuduotai.top

max(d, key=d.get)
来源：http://ujb.wangdashe.top

[U10] Py：按值排序字典
来源：http://wnw.wangshuangyany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://glc.gzhubu.top

[U11] Py：生成器表达式
来源：http://sfv.xinyue.icu

(x * 2 for x in arr)
来源：http://udz.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://dle.tian-w.cn

Counter(arr).most_common(3)
来源：http://tsi.andypj.xyz

[U13] Py：固定长度队列
来源：http://liu.shangyingyoupin.top

deque(maxlen=10)
来源：http://kgp.aibaodan.cn

[U14] Py：分组收集到列表
来源：http://zsn.ivvv.top

defaultdict(list)
来源：http://xjn.zhijiandao.cn

[U15] Py：高精度计时
来源：http://svk.gotoacloud.top

t = time.perf_counter()
来源：http://fvw.yueranfly.top

[U16] Py：命令行参数解析
来源：http://tej.shzxlz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mbs.zhoulong.xyz

[U17] Py：初始化日志
来源：http://dbj.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://tnt.hysaishi.cn

[U18] Py：预编译正则
来源：http://jwy.yuanzhike.top

pat = re.compile(r"\d+")
来源：http://ysf.chenzaomai.com

[U19] Py：正则替换带回调
来源：http://iav.epnwcf.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://axj.tanke756.top

[U20] Py：缓存函数结果
来源：http://ppx.zhengqikj.top

@functools.lru_cache(maxsize=None)
来源：http://ese.daxiang520.top

[U21] Py：自定义上下文管理器
来源：http://oco.svipenyu.cn

@contextlib.contextmanager
来源：http://rdm.ppjwa.cn

[U22] Py：矩阵转置
来源：http://qrr.pengpengdd.cyou

list(zip(*m))
来源：http://paf.shanyushiyangtech.top

[U23] Py：分块读取大文件
来源：http://iwo.kuanghao11.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qpb.zhixingplan.top

[U24] Py：路径操作
来源：http://ihf.aibaodan.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cli.guowangkeji.top

[U25] Py：CSV 按字典读
来源：http://bhr.daxiang520.top

csv.DictReader(f)
来源：http://nhj.hammf.cn

[U26] Py：并发下载
来源：http://vvm.sweek.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ios.ydjk.org.cn

[U27] Py：异步 HTTP
来源：http://dzp.tarul.cn

aiohttp.ClientSession() 配合 async with
来源：http://yhl.birdmap.top

[U28] Py：类型别名
来源：http://ujp.cdnleiting.top

UserId = int
来源：http://uud.snrcjt.cn

[U29] Py：属性校验
来源：http://lxe.jqgufenzy.top

@property 与 @x.setter 配合
来源：http://wdk.hysaishi.cn

[U30] Py：数据类
来源：http://nes.yuxming.cn

@dataclass(slots=True)
来源：http://osh.dashuyun.cn

[U31] Py：单测
来源：http://ltu.vqdsnc.cn

python -m pytest -q
来源：http://jng.sufxvd.cn

[U32] Py：代码格式化
来源：http://doa.yj202588.top

ruff format . && ruff check --fix .
来源：http://pxk.fktsv.cn

[U33] Py：打包发布
来源：http://frz.vqdsnc.cn

python -m build  （依赖 pyproject.toml）
来源：http://btp.haohaochexian.top

[U34] Py：判断编码
来源：http://rfl.iojbl.cn

chardet.detect(raw)
来源：http://biu.gaohongyu789.top

[U35] Py：发送邮件
来源：http://rgz.iojbl.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gdt.fktsv.cn

[U36] Py：定时任务
来源：http://ckl.yongpay.top

schedule.every(10).minutes.do(job)
来源：http://vhg.shuidangran.top

[U37] Py：读写 Excel
来源：http://uuq.fanxiaobao.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://blq.jianghu66.top

[U38] Py：获取脚本所在目录
来源：http://vgz.yj202588.top

Path(__file__).resolve().parent
来源：http://pyn.yongpay.top

[U39] Py：判断是否在交互环境
来源：http://ngk.hfpthk.cn

sys.stdout.isatty()
来源：http://vzi.pycfn.com

[U40] Py：打印到标准错误
来源：http://qhp.ctjpmb.com

print("err", file=sys.stderr)
来源：http://pps.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://per.gotoacloud.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wrj.daxiang520.top

[U42] PHP：PSR-4 自动加载
来源：http://yni.ivvv.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ecf.sjlbkw.cn

[U43] PHP：声明命名空间
来源：http://bjj.fzhhl.top

namespace App\Http;
来源：http://ged.shangyingyoupin.top

[U44] PHP：开启严格类型
来源：http://sio.yongpay.top

declare(strict_types=1);
来源：http://fuj.hnxiangtu.top

[U45] PHP：类型声明与返回类型
来源：http://rmb.bbcook.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xob.vqdsnc.cn

[U46] PHP：可空类型
来源：http://sil.yuanzhike.top

?string $name = null
来源：http://sdz.ybcxt.top

[U47] PHP：联合类型
来源：http://grz.cashguo.top

int|string $id
来源：http://dbq.yangfankeji.com

[U48] PHP：纯枚举
来源：http://gyb.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tpw.yanxiufei.cn

[U49] PHP：只读属性
来源：http://lay.hysaishi.cn

public readonly string $name
来源：http://uew.sufxvd.cn

[U50] PHP：构造器属性提升
来源：http://cui.yj20258888.top

public function __construct(private int $id) {}
来源：http://nab.wangshuangyany.cn

[U51] PHP：数组解构
来源：http://omq.ctjpmb.com

[$a, $b] = $arr;
来源：http://vvo.ctjpmb.com

[U52] PHP：箭头函数
来源：http://ihq.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://jzb.redwolf501.top

[U53] PHP：空合并运算符
来源：http://zoz.kuanghao11.cn

$v = $a ?? $b ?? "default";
来源：http://glb.sufxvd.cn

[U54] PHP：空安全调用
来源：http://nnt.zhongyouzk.top

$obj?->method()
来源：http://jnd.yonumen.top

[U55] PHP：match 表达式
来源：http://ynd.ywan-chungtsiang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cgz.pycfn.com

[U56] PHP：命名参数
来源：http://gzk.yj20258888.top

f(a: 1, b: 2)
来源：http://etn.jianghu66.top

[U57] PHP：字符串插值
来源：http://mfa.epnwcf.com

"值: {$a}"
来源：http://guf.haohaochexian.top

[U58] PHP：数组三件套
来源：http://jsr.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rhd.andypj.xyz

[U59] PHP：自定义排序
来源：http://xil.shuidangran.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pqo.9152youxi.cn

[U60] PHP：JSON 编解码
来源：http://zqq.zhiwuduotai.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kpq.hammf.cn

[U61] PHP：正则
来源：http://zqe.tarul.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rnb.aizwys.cn

[U62] PHP：日期对象
来源：http://ckb.cqqwz.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sal.yj202588.top

[U63] PHP：文件读写
来源：http://qvz.guowangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gzg.ybcxt.top

[U64] PHP：目录遍历
来源：http://sxp.meibo888.top

glob("dir/*.php");  scandir("dir");
来源：http://ige.zhixingplan.top

[U65] PHP：会话
来源：http://hpe.tanke756.top

session_start();  $_SESSION["uid"] = 1;
来源：http://esv.hfpthk.cn

[U66] PHP：设置 Cookie
来源：http://hye.wangshuangyany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jnb.shanyushiyangkeji.top

[U67] PHP：处理文件上传
来源：http://xre.hnxiangtu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jud.iojbl.cn

[U68] PHP：PDO 连接
来源：http://kti.uphjek.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bou.zhongyouzk.top

[U69] PHP：PDO 预处理
来源：http://kra.nwbrower.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jtj.316326.xyz

[U70] PHP：PDO 事务
来源：http://aoj.cdnleiting.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wch.jiagoushi.top

[U71] PHP：抛出异常
来源：http://vip.yj202588.top

throw new RuntimeException("失败", 500);
来源：http://nzv.hcnkem.com

[U72] PHP：写错误日志
来源：http://mkx.shangyingyoupin.top

error_log("失败: " . $e->getMessage());
来源：http://jne.iojbl.cn

[U73] PHP：读取 ini 配置
来源：http://kig.fanxiaobao.xyz

parse_ini_file("config.ini", true)
来源：http://ovi.chenzaomai.com

[U74] PHP：读取环境变量
来源：http://zlr.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://ubj.guannengcc.top

[U75] PHP：依赖注入
来源：http://qyv.xinyue.icu

composer require psr/container
来源：http://qth.cdnleiting.top

[U76] PHP：简单路由
来源：http://bos.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zxh.zhongyouzk.top

[U77] PHP：模板渲染
来源：http://spp.ydzc1.top

composer require twig/twig
来源：http://jxs.sweek.top

[U78] PHP：单元测试
来源：http://zou.tarul.cn

composer require --dev phpunit/phpunit
来源：http://wgv.mhx1999.top

[U79] PHP：静态分析
来源：http://hcw.yueranfly.top

composer require --dev phpstan/phpstan
来源：http://fvd.sweek.top

[U80] PHP：代码规范修复
来源：http://akx.jianghu66.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gvx.jqgufenzy.top

[U81] JS：初始化项目
来源：http://xei.yfazqb.com

npm init -y;  npm i express
来源：http://icv.jinghuilouyu.cn

[U82] JS：package.json 脚本
来源：http://nth.hysaishi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vyh.yangfankeji.com

[U83] JS：ES Module 导入导出
来源：http://wcm.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nxo.yanxiufei.cn

[U84] JS：CommonJS 写法
来源：http://qpv.snrcjt.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yvt.chenzaomai.com

[U85] JS：可选链
来源：http://ucb.jinqigufen.top

a?.b?.c
来源：http://thg.shanyushiyangtech.top

[U86] JS：空值合并
来源：http://ohr.jqgfzy.top

a ?? b
来源：http://xbx.hongshengwenyu.top

[U87] JS：解构默认值
来源：http://mwd.fehbvm.com

const { a = 1, b = 2 } = obj;
来源：http://fns.aibaodan.cn

[U88] JS：对象展开合并
来源：http://qag.jlsjyb.cn

{ ...a, ...b }
来源：http://wha.gaohongyu789.top

[U89] JS：数组去重
来源：http://frb.epnwcf.com

[...new Set(arr)]
来源：http://qdd.meibo888.top

[U90] JS：数字数组排序
来源：http://sha.tarul.cn

[...arr].sort((a, b) => a - b)
来源：http://vrx.52xcode.cn

[U91] JS：对象键值遍历
来源：http://sos.jinqigfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gpe.daxiang520.top

[U92] JS：深拷贝
来源：http://kqh.yonumen.top

structuredClone(obj)
来源：http://lvq.hesvh.cn

[U93] JS：模板字符串
来源：http://juk.zhixingplan.top

`共 ${n} 条`
来源：http://pfy.meibo888.top

[U94] JS：箭头函数
来源：http://ums.gogol.net.cn

const double = x => x * 2;
来源：http://wad.jinqigufen.top

[U95] JS：Promise 包装
来源：http://gcc.gogol.net.cn

new Promise((resolve, reject) => {})
来源：http://fvq.ydjk.org.cn

[U96] JS：async/await 与异常
来源：http://wog.guowangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mvh.zhengqikj.top

[U97] JS：并发请求
来源：http://dyw.fzhhl.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vny.jqgufenzy.top

[U98] JS：fetch 带 JSON
来源：http://flu.hongshengwenyu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qqj.kuanghao11.cn

[U99] JS：事件监听
来源：http://off.kuanghao11.cn

el.addEventListener("click", e => {})
来源：http://qnx.sweek.top

[U100] JS：DOM 查询
来源：http://egm.xziqi.cn

document.querySelector(".item")
来源：http://xly.c1oappe.top

[U101] JS：classList 操作
来源：http://njc.bjfxy.top

el.classList.toggle("active")
来源：http://neb.epnwcf.com

[U102] JS：本地存储
来源：http://zyb.zhaomingkeji.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://hgf.fzhhl.top

[U103] JS：定时器
来源：http://iva.uphjek.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cwj.ctjpmb.com

[U104] JS：防抖
来源：http://yej.zhiwuduotai.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fxv.cdnleiting.top

[U105] JS：节流
来源：http://ibk.chenzaomai.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mfy.xuanzx.com

[U106] JS：日期格式化
来源：http://vme.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bsl.tian-w.cn

[U107] JS：数字千分位
来源：http://sdh.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vjl.tianlin.xyz

[U108] JS：随机整数
来源：http://lur.hammf.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wjf.zhijiandao.cn

[U109] JS：数组分组
来源：http://kej.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://yjy.c1oappe.top

[U110] JS：数组分块
来源：http://nhq.jqgufenzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://imy.hongshengwenyu.top

[U111] JS：对象转 Map
来源：http://piq.snrcjt.cn

new Map(Object.entries(obj))
来源：http://sip.hywenlv.cn

[U112] JS：字符串补位
来源：http://apt.vqdsnc.cn

"7".padStart(3, "0")
来源：http://lee.vehdjk.com

[U113] JS：正则替换全部
来源：http://rsj.hongshengwenyu.top

s.replaceAll("a", "b")
来源：http://vrv.yangfankeji.com

[U114] JS：JSON 深比较
来源：http://xuc.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cut.hywenlv.cn

[U115] JS：生成 UUID
来源：http://ptv.hongshengwenyu.top

crypto.randomUUID()
来源：http://wga.cdnleiting.top

[U116] JS：类型检查（JSDoc）
来源：http://zsz.jqgufenzy.top

/** @param {string} name */ function f(name) {}
来源：http://vnu.jlsjyb.cn

[U117] JS：单元测试
来源：http://zmp.yj20258.top

npm i -D vitest;  npx vitest
来源：http://duy.cdnleiting.top

[U118] JS：开发服务器
来源：http://rlr.fehbvm.com

npm i -D vite;  npx vite
来源：http://kgr.ehwqpu.com

[U119] JS：生产构建
来源：http://xta.nwbrower.top

npx vite build
来源：http://koc.dianchejie.cn

[U120] JS：读取环境变量（Vite）
来源：http://osu.sufxvd.cn

import.meta.env.VITE_API_URL
来源：http://rbb.snrcjt.cn

================================================================================
来源：http://zny.yonumen.top

统计汇总
来源：http://sqi.yj20258888.top

================================================================================
来源：http://ziy.hnqzz.top

按语言统计（条）：
来源：http://rlz.jlsjyb.cn

Python ......... 252
来源：http://tij.yuxming.cn

PHP ............ 252
来源：http://xys.pengpengdd.cyou

JavaScript ..... 252
来源：http://nyu.sysykeji.top

TypeScript ..... 212
来源：http://ebj.sufxvd.cn

Java ........... 212
来源：http://zey.guowangkeji.top

Go ............. 212
来源：http://gmt.9152youxi.cn

Ruby ........... 212
来源：http://fit.tianlin.xyz

C# ............. 212
来源：http://yzh.yongpay.top

C .............. 30
来源：http://owb.cashguo.top

C++ ............ 30
来源：http://oco.fengsongda.top

SQL ............ 90
来源：http://mil.sysykeji.top

Bash ........... 80
来源：http://emp.fktsv.cn

Kotlin ......... 15
来源：http://sfw.yanxiufei.cn

Swift .......... 15
来源：http://ufm.xinyue.icu

Lua ............ 10
来源：http://vpf.ybcxt.top

Perl ........... 10
来源：http://sks.hywenlv.cn

Scala .......... 10
来源：http://gbr.fktsv.cn

------------------------------------
来源：http://ewj.aizwys.cn

合计 ........... 2106 条
来源：http://hew.guannengcc.top

按章节统计：
来源：http://coy.ivvv.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lur.jinghuilouyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oqv.yonumen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mtr.feifeiyinyue.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xrb.sufxvd.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kua.tian-w.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vew.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lzj.chenzaomai.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://alk.316326.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gcn.jinyuanbaomall.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://djl.shangyingyoupin.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rlm.yueranfly.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://huz.zhiwuduotai.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wte.jinghuilouyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qxj.zdbjq.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lsz.tarul.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jpr.hnqzz.top

Q SQL 专题                              90
来源：http://rht.cucudq.cn

R Bash 专题                             80
来源：http://hpm.sxryk.cn

S C / C++ 专题                          60
来源：http://gpk.zhiwuduotai.top

T 其他语言补充                          60
来源：http://muh.shuidangran.top

U 高频实用片段                         120
来源：http://wvi.cdnleiting.top

------------------------------------
来源：http://kmy.xuanzx.com

合计                                  2106 条
来源：http://rnd.fktsv.cn

--------------------------------------------------------------------------------
来源：http://ybb.sjlbkw.cn

使用提醒
来源：http://dnv.gzhubu.top

--------------------------------------------------------------------------------
来源：http://srn.xingfuxueyuan.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jzf.jyoumei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kjs.nanxinkj.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nnk.sjlbkw.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mbj.yj202588.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ltr.pycfn.com

—— 文件结束 ——
来源：http://rbv.havefunace.top

================================================================================
来源：http://das.yuanzhike.top

程序语言常见例子速查手册（2024 版）
来源：http://piy.sjlbkw.cn

Common Programming Examples Cheat Book
来源：http://bud.zhengqikj.top

================================================================================
来源：http://usq.jinqigfzy.top

【收录内容】
来源：http://evp.mhx1999.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vgw.andypj.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gmd.ydjk.org.cn

SQL · Bash · C · C++
来源：http://kbu.hysaishi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kvb.ybcxt.top

【使用说明】
来源：http://ohx.zhijiandao.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iuh.cashguo.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://aim.pengpengdd.cyou

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://juj.redwolf501.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rfx.jinghuilouyu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fxo.ctjpmb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rbz.hammf.cn


<!-- 参考信息 -->