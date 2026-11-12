代发 wailian999

[U15] Py：高精度计时
来源：http://vwi.yongpay.top

t = time.perf_counter()
来源：http://anb.cucudq.cn

[U16] Py：命令行参数解析
来源：http://nbs.jlsjyb.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pqy.quarkkingdee.top

[U17] Py：初始化日志
来源：http://ihl.zhongyouzk.top

logging.basicConfig(level=logging.INFO)
来源：http://dxz.yfazqb.com

[U18] Py：预编译正则
来源：http://uzi.ydjk.org.cn

pat = re.compile(r"\d+")
来源：http://wca.shuidangran.top

[U19] Py：正则替换带回调
来源：http://wvv.haohaochexian.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ozx.xingfuxueyuan.xyz

[U20] Py：缓存函数结果
来源：http://ymq.guannengcc.top

@functools.lru_cache(maxsize=None)
来源：http://taq.bjfxy.top

[U21] Py：自定义上下文管理器
来源：http://zsn.jiagoushi.top

@contextlib.contextmanager
来源：http://jqe.sufxvd.cn

[U22] Py：矩阵转置
来源：http://mta.feifeiyinyue.top

list(zip(*m))
来源：http://knf.shzxlz.cn

[U23] Py：分块读取大文件
来源：http://tsf.zdbjq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ncl.pycfn.com

[U24] Py：路径操作
来源：http://vfm.redwolf501.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dbv.fktsv.cn

[U25] Py：CSV 按字典读
来源：http://rfo.jqgufenzy.top

csv.DictReader(f)
来源：http://cma.sysykeji.top

[U26] Py：并发下载
来源：http://uqh.yueranfly.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sbw.daxiang520.top

[U27] Py：异步 HTTP
来源：http://vqu.cashguo.top

aiohttp.ClientSession() 配合 async with
来源：http://tig.snrcjt.cn

[U28] Py：类型别名
来源：http://irv.cdnleiting.top

UserId = int
来源：http://fzq.yuanzhike.top

[U29] Py：属性校验
来源：http://bmb.cqqwz.cn

@property 与 @x.setter 配合
来源：http://buh.ehwqpu.com

[U30] Py：数据类
来源：http://xtg.sxryk.cn

@dataclass(slots=True)
来源：http://efu.nanxinkj.top

[U31] Py：单测
来源：http://uym.xingfuxueyuan.xyz

python -m pytest -q
来源：http://lom.smart0.xyz

[U32] Py：代码格式化
来源：http://qfv.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://rac.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://det.svipenyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://khf.shuidangran.top

[U34] Py：判断编码
来源：http://hit.zdbjq.cn

chardet.detect(raw)
来源：http://mmy.jinghuilouyu.cn

[U35] Py：发送邮件
来源：http://pkt.aizwys.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vzs.hnqzz.top

[U36] Py：定时任务
来源：http://sdv.yueranfly.top

schedule.every(10).minutes.do(job)
来源：http://kuf.vqdsnc.cn

[U37] Py：读写 Excel
来源：http://vrl.daria6918.cn

pandas.read_excel / DataFrame.to_excel
来源：http://imx.gotoacloud.top

[U38] Py：获取脚本所在目录
来源：http://fqw.tianlin.xyz

Path(__file__).resolve().parent
来源：http://byo.shanyushiyangkeji.top

[U39] Py：判断是否在交互环境
来源：http://qgi.cucudq.cn

sys.stdout.isatty()
来源：http://ddq.mhx1999.top

[U40] Py：打印到标准错误
来源：http://dpe.9152youxi.cn

print("err", file=sys.stderr)
来源：http://bny.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://asu.tian-w.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fko.nanxinkj.top

[U42] PHP：PSR-4 自动加载
来源：http://mxc.kuanghao11.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gmu.jqgufenzy.top

[U43] PHP：声明命名空间
来源：http://ntd.svipenyu.cn

namespace App\Http;
来源：http://bqh.uphjek.com

[U44] PHP：开启严格类型
来源：http://aus.hnxiangtu.top

declare(strict_types=1);
来源：http://ywx.aibaodan.cn

[U45] PHP：类型声明与返回类型
来源：http://fbq.pengpengdd.cyou

function add(int $a, int $b): int { return $a + $b; }
来源：http://vmp.yj202588.top

[U46] PHP：可空类型
来源：http://xte.xuanzx.com

?string $name = null
来源：http://hha.sjlbkw.cn

[U47] PHP：联合类型
来源：http://edm.vqdsnc.cn

int|string $id
来源：http://iee.daria6918.cn

[U48] PHP：纯枚举
来源：http://ije.tian-w.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ylr.snrcjt.cn

[U49] PHP：只读属性
来源：http://nfs.jqgufenzy.top

public readonly string $name
来源：http://hkp.nanxuanxn.top

[U50] PHP：构造器属性提升
来源：http://cpx.0kj1m.cn

public function __construct(private int $id) {}
来源：http://rta.shzxlz.cn

[U51] PHP：数组解构
来源：http://qtk.vqdsnc.cn

[$a, $b] = $arr;
来源：http://ihg.xuanzx.com

[U52] PHP：箭头函数
来源：http://rci.dashuyun.cn

$double = fn($x) => $x * 2;
来源：http://oto.jinqigfzy.top

[U53] PHP：空合并运算符
来源：http://dpc.jiagoushi.top

$v = $a ?? $b ?? "default";
来源：http://xea.316326.xyz

[U54] PHP：空安全调用
来源：http://ehn.0kj1m.cn

$obj?->method()
来源：http://pky.chenzaomai.com

[U55] PHP：match 表达式
来源：http://yjf.xinyue.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fvj.shanyushiyangtech.top

[U56] PHP：命名参数
来源：http://lcb.ehwqpu.com

f(a: 1, b: 2)
来源：http://ves.quarkkingdee.top

[U57] PHP：字符串插值
来源：http://jry.havefunace.top

"值: {$a}"
来源：http://hoc.xylfe.cn

[U58] PHP：数组三件套
来源：http://njy.kuanghao11.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fpj.jinghuilouyu.cn

[U59] PHP：自定义排序
来源：http://gdk.shuidangran.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ifn.xuanzx.com

[U60] PHP：JSON 编解码
来源：http://qpm.snrcjt.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hlp.yj20258888.top

[U61] PHP：正则
来源：http://has.yueranfly.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cmj.9152youxi.cn

[U62] PHP：日期对象
来源：http://pot.zhiwuduotai.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gfe.andypj.xyz

[U63] PHP：文件读写
来源：http://cqb.jinqigfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bfw.hnqzz.top

[U64] PHP：目录遍历
来源：http://wwu.yvedp.cn

glob("dir/*.php");  scandir("dir");
来源：http://vwf.yvedp.cn

[U65] PHP：会话
来源：http://kul.fzhhl.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tip.tian-w.cn

[U66] PHP：设置 Cookie
来源：http://krl.fehbvm.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eyd.fktsv.cn

[U67] PHP：处理文件上传
来源：http://crd.gogol.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mxy.jinqigfzy.top

[U68] PHP：PDO 连接
来源：http://jod.shuidangran.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zbs.zhijiandao.cn

[U69] PHP：PDO 预处理
来源：http://enl.zycfv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://igs.ehwqpu.com

[U70] PHP：PDO 事务
来源：http://wua.jiagoushi.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uyi.yuanzhike.top

[U71] PHP：抛出异常
来源：http://rsx.ywan-chungtsiang.top

throw new RuntimeException("失败", 500);
来源：http://rim.pengpengdd.cyou

[U72] PHP：写错误日志
来源：http://ecc.cheryme.top

error_log("失败: " . $e->getMessage());
来源：http://ivz.sufxvd.cn

[U73] PHP：读取 ini 配置
来源：http://oxl.yongpay.top

parse_ini_file("config.ini", true)
来源：http://fne.yj202588.top

[U74] PHP：读取环境变量
来源：http://jix.zdqjudy.top

getenv("APP_ENV") ?: "production"
来源：http://rvg.sxryk.cn

[U75] PHP：依赖注入
来源：http://vay.uphjek.com

composer require psr/container
来源：http://vmo.shzxlz.cn

[U76] PHP：简单路由
来源：http://epl.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zul.vehdjk.com

[U77] PHP：模板渲染
来源：http://lyr.cqqwz.cn

composer require twig/twig
来源：http://mpl.chenlongwang.top

[U78] PHP：单元测试
来源：http://umb.jinghuilouyu.cn

composer require --dev phpunit/phpunit
来源：http://nka.9152youxi.cn

[U79] PHP：静态分析
来源：http://ilt.yueranfly.top

composer require --dev phpstan/phpstan
来源：http://rit.cucudq.cn

[U80] PHP：代码规范修复
来源：http://fuf.jlsjyb.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jvf.zycfv.cn

[U81] JS：初始化项目
来源：http://tvs.tarul.cn

npm init -y;  npm i express
来源：http://mhj.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://jvg.jqgufenzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://igm.xinyue.icu

[U83] JS：ES Module 导入导出
来源：http://acy.ybcxt.top

export const a = 1;  import { a } from "./m.js";
来源：http://myj.zhiwuduotai.top

[U84] JS：CommonJS 写法
来源：http://ydn.tanke756.top

module.exports = { a };  const { a } = require("./m");
来源：http://wvn.gaohongyu789.top

[U85] JS：可选链
来源：http://gmx.snrcjt.cn

a?.b?.c
来源：http://dto.yonumen.top

[U86] JS：空值合并
来源：http://htc.hammf.cn

a ?? b
来源：http://tou.fanxiaobao.xyz

[U87] JS：解构默认值
来源：http://mbi.sweek.top

const { a = 1, b = 2 } = obj;
来源：http://yrd.fengsongda.top

[U88] JS：对象展开合并
来源：http://icz.xuanzx.com

{ ...a, ...b }
来源：http://xhr.tarul.cn

[U89] JS：数组去重
来源：http://qsc.smart0.xyz

[...new Set(arr)]
来源：http://gcz.vehdjk.com

[U90] JS：数字数组排序
来源：http://zko.sysykeji.top

[...arr].sort((a, b) => a - b)
来源：http://fqi.xuanzx.com

[U91] JS：对象键值遍历
来源：http://crk.yongpay.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zib.guannengcc.top

[U92] JS：深拷贝
来源：http://foe.52xcode.cn

structuredClone(obj)
来源：http://mpd.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://lah.zhiwuduotai.top

`共 ${n} 条`
来源：http://roa.smart0.xyz

[U94] JS：箭头函数
来源：http://shg.nwbrower.top

const double = x => x * 2;
来源：http://pxg.ctjpmb.com

[U95] JS：Promise 包装
来源：http://tdq.xuanzx.com

new Promise((resolve, reject) => {})
来源：http://bcw.yfazqb.com

[U96] JS：async/await 与异常
来源：http://cgy.feifeiyinyue.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uvp.guowangkeji.top

[U97] JS：并发请求
来源：http://aeb.yj20258.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cwi.jianghu66.top

[U98] JS：fetch 带 JSON
来源：http://zuq.wangshuangyany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nhu.wangshuangyany.cn

[U99] JS：事件监听
来源：http://lbb.quarkkingdee.top

el.addEventListener("click", e => {})
来源：http://ums.yj20258888.top

[U100] JS：DOM 查询
来源：http://zbk.xuetiantiany.cn

document.querySelector(".item")
来源：http://hwr.jiagoushi.top

[U101] JS：classList 操作
来源：http://jtg.zdqjudy.top

el.classList.toggle("active")
来源：http://isc.dianchejie.cn

[U102] JS：本地存储
来源：http://ydq.zdbjq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rjc.daria6918.cn

[U103] JS：定时器
来源：http://dko.cqqwz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wtx.zdbjq.cn

[U104] JS：防抖
来源：http://xaw.jinyuanbaomall.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dhb.nanxinkj.top

[U105] JS：节流
来源：http://gph.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sim.smart0.xyz

[U106] JS：日期格式化
来源：http://xfp.yvedp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tvl.jqgufenzy.top

[U107] JS：数字千分位
来源：http://piy.redwolf501.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://orc.xingfuxueyuan.xyz

[U108] JS：随机整数
来源：http://yxy.hesvh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jgf.zhoulong.xyz

[U109] JS：数组分组
来源：http://dev.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://dzo.feifeiyinyue.top

[U110] JS：数组分块
来源：http://dbq.xziqi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ayi.dianchejie.cn

[U111] JS：对象转 Map
来源：http://hwy.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://dpx.gotoacloud.top

[U112] JS：字符串补位
来源：http://oee.yanxiufei.cn

"7".padStart(3, "0")
来源：http://rix.meibo888.top

[U113] JS：正则替换全部
来源：http://the.hongshengwenyu.top

s.replaceAll("a", "b")
来源：http://ypl.xuanzx.com

[U114] JS：JSON 深比较
来源：http://ypz.mhx1999.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bbe.jqgfzy.top

[U115] JS：生成 UUID
来源：http://zfm.shanyushiyangkeji.top

crypto.randomUUID()
来源：http://lpx.pycfn.com

[U116] JS：类型检查（JSDoc）
来源：http://uxw.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://vvq.cdnleiting.top

[U117] JS：单元测试
来源：http://kfi.xziqi.cn

npm i -D vitest;  npx vitest
来源：http://ubw.shzxlz.cn

[U118] JS：开发服务器
来源：http://bdz.hysaishi.cn

npm i -D vite;  npx vite
来源：http://jdw.yanxiufei.cn

[U119] JS：生产构建
来源：http://ofp.yvedp.cn

npx vite build
来源：http://mse.hcnkem.com

[U120] JS：读取环境变量（Vite）
来源：http://qzv.ydzc1.top

import.meta.env.VITE_API_URL
来源：http://pxo.ppjwa.cn

================================================================================
来源：http://usl.zhaomingkeji.xyz

统计汇总
来源：http://wio.hnxiangtu.top

================================================================================
来源：http://sjy.gzhubu.top

按语言统计（条）：
来源：http://jof.ydzc1.top

Python ......... 252
来源：http://vnr.ydjk.org.cn

PHP ............ 252
来源：http://cbt.shuidangran.top

JavaScript ..... 252
来源：http://rxx.daxiang520.top

TypeScript ..... 212
来源：http://nwv.kuanghao11.cn

Java ........... 212
来源：http://vxh.guowangkeji.top

Go ............. 212
来源：http://nce.yj202588.top

Ruby ........... 212
来源：http://gds.xylfe.cn

C# ............. 212
来源：http://kww.cashguo.top

C .............. 30
来源：http://lku.xingfuxueyuan.xyz

C++ ............ 30
来源：http://qhd.316326.xyz

SQL ............ 90
来源：http://oew.jqgfzy.top

Bash ........... 80
来源：http://tll.yj20258888.top

Kotlin ......... 15
来源：http://uke.epnwcf.com

Swift .......... 15
来源：http://oui.snrcjt.cn

Lua ............ 10
来源：http://rnf.xinyue.icu

Perl ........... 10
来源：http://etd.bjfxy.top

Scala .......... 10
来源：http://ylw.52xcode.cn

------------------------------------
来源：http://wul.yongpay.top

合计 ........... 2106 条
来源：http://hit.gogol.net.cn

按章节统计：
来源：http://zui.shanyushiyangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tdo.fktsv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cih.yj202588.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pic.zhixingplan.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dgd.guannengcc.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ccd.daria6918.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rmf.nwbrower.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lwe.xziqi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yrg.svipenyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ocy.birdmap.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dqq.ywan-chungtsiang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://erm.jiagoushi.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kxo.shangyingyoupin.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vbr.jinqigufen.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hnh.yongpay.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bgq.iojbl.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://spb.snrcjt.cn

Q SQL 专题                              90
来源：http://sux.shuidangran.top

R Bash 专题                             80
来源：http://sfw.ywan-chungtsiang.top

S C / C++ 专题                          60
来源：http://hdo.cqqwz.cn

T 其他语言补充                          60
来源：http://bai.daria6918.cn

U 高频实用片段                         120
来源：http://wyp.sufxvd.cn

------------------------------------
来源：http://sep.hysaishi.cn

合计                                  2106 条
来源：http://svn.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://nfy.wangshuangyany.cn

使用提醒
来源：http://cth.gzhubu.top

--------------------------------------------------------------------------------
来源：http://jfu.aibaodan.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sjw.316326.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pqx.guowangkeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wlt.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://iuy.jinghuilouyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://olc.hfpthk.cn

—— 文件结束 ——
来源：http://srl.jyoumei.cn

================================================================================
来源：http://fpm.cheryme.top

程序语言常见例子速查手册（2024 版）
来源：http://kya.tarul.cn

Common Programming Examples Cheat Book
来源：http://jqk.nanxinkj.top

================================================================================
来源：http://kut.0kj1m.cn

【收录内容】
来源：http://abx.cqqwz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yya.52xcode.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sdr.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://duj.xingfuxueyuan.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ckv.mhx1999.top

【使用说明】
来源：http://bvk.tian-w.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nkv.chenlongwang.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yyz.ybcxt.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zlu.xingfuxueyuan.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gag.yfazqb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://ybd.cqqwz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mkl.pengpengdd.cyou

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://axi.jinyuanbaomall.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gzh.vehdjk.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uiu.zhiwuduotai.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nru.guannengcc.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ssy.ywan-chungtsiang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pyy.tianlin.xyz

【文件统计】
来源：http://lcq.jianghu66.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fwl.iojbl.cn

--------------------------------------------------------------------------------
来源：http://xzk.wangdashe.top

目  录
来源：http://veg.sweek.top

--------------------------------------------------------------------------------
来源：http://pbe.xylfe.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qgc.yangfankeji.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rse.snrcjt.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rkq.jiagoushi.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://foh.ctjpmb.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ynp.sysykeji.top


<!-- 参考信息 -->