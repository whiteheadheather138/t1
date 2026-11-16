代发 wailian999

[U15] Py：高精度计时
来源：http://yot.9152youxi.cn

t = time.perf_counter()
来源：http://dvm.wangdashe.top

[U16] Py：命令行参数解析
来源：http://lay.epnwcf.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://smf.zdbjq.cn

[U17] Py：初始化日志
来源：http://wrg.xylfe.cn

logging.basicConfig(level=logging.INFO)
来源：http://ofj.hnxiangtu.top

[U18] Py：预编译正则
来源：http://hur.jyoumei.cn

pat = re.compile(r"\d+")
来源：http://yto.52xcode.cn

[U19] Py：正则替换带回调
来源：http://kbs.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ctk.vqdsnc.cn

[U20] Py：缓存函数结果
来源：http://vet.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://ykv.shuidangran.top

[U21] Py：自定义上下文管理器
来源：http://afy.xuanzx.com

@contextlib.contextmanager
来源：http://vfn.wangshuangyany.cn

[U22] Py：矩阵转置
来源：http://hfk.9152youxi.cn

list(zip(*m))
来源：http://pph.yfazqb.com

[U23] Py：分块读取大文件
来源：http://aci.xinyue.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://itl.0kj1m.cn

[U24] Py：路径操作
来源：http://ttx.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bcm.hammf.cn

[U25] Py：CSV 按字典读
来源：http://zno.jinghuilouyu.cn

csv.DictReader(f)
来源：http://tkf.xuetiantiany.cn

[U26] Py：并发下载
来源：http://wvg.zhijiandao.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yew.birdmap.top

[U27] Py：异步 HTTP
来源：http://gey.sjlbkw.cn

aiohttp.ClientSession() 配合 async with
来源：http://vnk.meibo888.top

[U28] Py：类型别名
来源：http://rjq.gaohongyu789.top

UserId = int
来源：http://gsw.cdnleiting.top

[U29] Py：属性校验
来源：http://ond.haohaochexian.top

@property 与 @x.setter 配合
来源：http://apx.jlsjyb.cn

[U30] Py：数据类
来源：http://dsu.hnqzz.top

@dataclass(slots=True)
来源：http://zth.chenzaomai.com

[U31] Py：单测
来源：http://nzd.jqgufenzy.top

python -m pytest -q
来源：http://axb.ehwqpu.com

[U32] Py：代码格式化
来源：http://hsv.vehdjk.com

ruff format . && ruff check --fix .
来源：http://msm.shzxlz.cn

[U33] Py：打包发布
来源：http://phu.yj202588.top

python -m build  （依赖 pyproject.toml）
来源：http://ozl.yonumen.top

[U34] Py：判断编码
来源：http://cse.fehbvm.com

chardet.detect(raw)
来源：http://lne.fehbvm.com

[U35] Py：发送邮件
来源：http://ukm.tianlin.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://web.c1oappe.top

[U36] Py：定时任务
来源：http://tvx.jinqigfzy.top

schedule.every(10).minutes.do(job)
来源：http://rda.xingfuxueyuan.xyz

[U37] Py：读写 Excel
来源：http://oet.andypj.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://pwy.jqgufenzy.top

[U38] Py：获取脚本所在目录
来源：http://fvs.zhijiandao.cn

Path(__file__).resolve().parent
来源：http://zma.316326.xyz

[U39] Py：判断是否在交互环境
来源：http://hwr.yvedp.cn

sys.stdout.isatty()
来源：http://qbs.ivvv.top

[U40] Py：打印到标准错误
来源：http://vij.zhijiandao.cn

print("err", file=sys.stderr)
来源：http://wrj.fehbvm.com

[U41] PHP：初始化 Composer 项目
来源：http://kjh.jiagoushi.top

composer init;  composer require guzzlehttp/guzzle
来源：http://clx.hnqzz.top

[U42] PHP：PSR-4 自动加载
来源：http://opz.dianchejie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://osz.hnqzz.top

[U43] PHP：声明命名空间
来源：http://aes.fzhhl.top

namespace App\Http;
来源：http://fsl.jinghuilouyu.cn

[U44] PHP：开启严格类型
来源：http://jnm.cdnleiting.top

declare(strict_types=1);
来源：http://fzp.jinqigfzy.top

[U45] PHP：类型声明与返回类型
来源：http://oaz.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://xju.bjfxy.top

[U46] PHP：可空类型
来源：http://rqa.tanke756.top

?string $name = null
来源：http://fwu.yanxiufei.cn

[U47] PHP：联合类型
来源：http://kix.cqqwz.cn

int|string $id
来源：http://xmn.bbcook.cn

[U48] PHP：纯枚举
来源：http://bqp.ivvv.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xeq.ybcxt.top

[U49] PHP：只读属性
来源：http://hyz.ybcxt.top

public readonly string $name
来源：http://sdy.wangdashe.top

[U50] PHP：构造器属性提升
来源：http://oyg.zhoulong.xyz

public function __construct(private int $id) {}
来源：http://nto.cqqwz.cn

[U51] PHP：数组解构
来源：http://jsz.tianlin.xyz

[$a, $b] = $arr;
来源：http://pbs.xuetiantiany.cn

[U52] PHP：箭头函数
来源：http://ptv.zhaomingkeji.xyz

$double = fn($x) => $x * 2;
来源：http://gyc.chenlongwang.top

[U53] PHP：空合并运算符
来源：http://miu.ybcxt.top

$v = $a ?? $b ?? "default";
来源：http://rrf.snrcjt.cn

[U54] PHP：空安全调用
来源：http://ild.shanyushiyangkeji.top

$obj?->method()
来源：http://ucg.zhongyouzk.top

[U55] PHP：match 表达式
来源：http://eov.bbcook.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sdz.sjlbkw.cn

[U56] PHP：命名参数
来源：http://nxn.gogol.net.cn

f(a: 1, b: 2)
来源：http://mzn.snrcjt.cn

[U57] PHP：字符串插值
来源：http://hjs.feifeiyinyue.top

"值: {$a}"
来源：http://yzx.zycfv.cn

[U58] PHP：数组三件套
来源：http://xuo.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mwx.316326.xyz

[U59] PHP：自定义排序
来源：http://cjx.jyoumei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mbw.zhiwuduotai.top

[U60] PHP：JSON 编解码
来源：http://rbr.meibo888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ibr.zhixingplan.top

[U61] PHP：正则
来源：http://vmm.andypj.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ypo.zycfv.cn

[U62] PHP：日期对象
来源：http://bun.sweek.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hyr.ybcxt.top

[U63] PHP：文件读写
来源：http://ood.jinqigfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bpj.jinqigufen.top

[U64] PHP：目录遍历
来源：http://aeh.fzhhl.top

glob("dir/*.php");  scandir("dir");
来源：http://kjg.jianghu66.top

[U65] PHP：会话
来源：http://aat.xuanzx.com

session_start();  $_SESSION["uid"] = 1;
来源：http://hzu.yangfankeji.com

[U66] PHP：设置 Cookie
来源：http://gfr.nanxinkj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yqu.dashuyun.cn

[U67] PHP：处理文件上传
来源：http://nnx.ehwqpu.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://odk.shuidangran.top

[U68] PHP：PDO 连接
来源：http://rss.jianghu66.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://umv.jinyuanbaomall.cn

[U69] PHP：PDO 预处理
来源：http://eay.guowangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zwh.birdmap.top

[U70] PHP：PDO 事务
来源：http://wdk.jinyuanbaomall.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://agw.zycfv.cn

[U71] PHP：抛出异常
来源：http://umf.nanxinkj.top

throw new RuntimeException("失败", 500);
来源：http://lvl.xinyue.icu

[U72] PHP：写错误日志
来源：http://fzc.yvedp.cn

error_log("失败: " . $e->getMessage());
来源：http://iva.ydzc1.top

[U73] PHP：读取 ini 配置
来源：http://gxq.yuxming.cn

parse_ini_file("config.ini", true)
来源：http://obv.xingfuxueyuan.xyz

[U74] PHP：读取环境变量
来源：http://rvz.iojbl.cn

getenv("APP_ENV") ?: "production"
来源：http://wgc.yj20258888.top

[U75] PHP：依赖注入
来源：http://uoz.zhixingplan.top

composer require psr/container
来源：http://hae.gogol.net.cn

[U76] PHP：简单路由
来源：http://qbx.ywan-chungtsiang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gui.haohaochexian.top

[U77] PHP：模板渲染
来源：http://ace.tarul.cn

composer require twig/twig
来源：http://vdd.fktsv.cn

[U78] PHP：单元测试
来源：http://mjy.wangdashe.top

composer require --dev phpunit/phpunit
来源：http://qlp.pengpengdd.cyou

[U79] PHP：静态分析
来源：http://saq.dianchejie.cn

composer require --dev phpstan/phpstan
来源：http://myr.hongshengwenyu.top

[U80] PHP：代码规范修复
来源：http://npv.jiagoushi.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ixo.jinghuilouyu.cn

[U81] JS：初始化项目
来源：http://ssv.jyoumei.cn

npm init -y;  npm i express
来源：http://fse.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://oeo.hcnkem.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lnu.sjlbkw.cn

[U83] JS：ES Module 导入导出
来源：http://mfb.jyoumei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kcr.yangfankeji.com

[U84] JS：CommonJS 写法
来源：http://bco.nwbrower.top

module.exports = { a };  const { a } = require("./m");
来源：http://uys.xuanzx.com

[U85] JS：可选链
来源：http://wgz.ybcxt.top

a?.b?.c
来源：http://syl.yonumen.top

[U86] JS：空值合并
来源：http://ude.zdbjq.cn

a ?? b
来源：http://eoy.zhoulong.xyz

[U87] JS：解构默认值
来源：http://nhi.xinyue.icu

const { a = 1, b = 2 } = obj;
来源：http://tcg.sufxvd.cn

[U88] JS：对象展开合并
来源：http://kqz.snrcjt.cn

{ ...a, ...b }
来源：http://hgx.shanyushiyangtech.top

[U89] JS：数组去重
来源：http://iny.sufxvd.cn

[...new Set(arr)]
来源：http://juf.nanxuanxn.top

[U90] JS：数字数组排序
来源：http://xnt.ivvv.top

[...arr].sort((a, b) => a - b)
来源：http://bgq.dianchejie.cn

[U91] JS：对象键值遍历
来源：http://iuj.xingfuxueyuan.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cuu.jyoumei.cn

[U92] JS：深拷贝
来源：http://etw.birdmap.top

structuredClone(obj)
来源：http://ryc.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://mbk.zhixingplan.top

`共 ${n} 条`
来源：http://wpd.jinyuanbaomall.cn

[U94] JS：箭头函数
来源：http://jew.tanke756.top

const double = x => x * 2;
来源：http://ngh.xingfuxueyuan.xyz

[U95] JS：Promise 包装
来源：http://arc.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://orj.zhengqikj.top

[U96] JS：async/await 与异常
来源：http://sda.redwolf501.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mzs.aizwys.cn

[U97] JS：并发请求
来源：http://cre.kuanghao11.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jau.xinyue.icu

[U98] JS：fetch 带 JSON
来源：http://wak.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mtm.zhaomingkeji.xyz

[U99] JS：事件监听
来源：http://lek.nanxuanxn.top

el.addEventListener("click", e => {})
来源：http://pro.yj20258888.top

[U100] JS：DOM 查询
来源：http://clb.aizwys.cn

document.querySelector(".item")
来源：http://kym.sweek.top

[U101] JS：classList 操作
来源：http://gpp.havefunace.top

el.classList.toggle("active")
来源：http://lcp.tarul.cn

[U102] JS：本地存储
来源：http://ytd.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ord.ydzc1.top

[U103] JS：定时器
来源：http://bkq.wangdashe.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eel.dianchejie.cn

[U104] JS：防抖
来源：http://vzn.nanxuanxn.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gvr.feifeiyinyue.top

[U105] JS：节流
来源：http://bjo.xuetiantiany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ydx.guowangkeji.top

[U106] JS：日期格式化
来源：http://hjx.havefunace.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oys.cucudq.cn

[U107] JS：数字千分位
来源：http://dvb.dianchejie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rmz.yvedp.cn

[U108] JS：随机整数
来源：http://ngc.daria6918.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xqv.sweek.top

[U109] JS：数组分组
来源：http://fhe.jqgfzy.top

Object.groupBy(arr, x => x.type)
来源：http://asg.bjfxy.top

[U110] JS：数组分块
来源：http://glh.vehdjk.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://igo.ctjpmb.com

[U111] JS：对象转 Map
来源：http://ijb.dashuyun.cn

new Map(Object.entries(obj))
来源：http://unu.chenzaomai.com

[U112] JS：字符串补位
来源：http://hto.gogol.net.cn

"7".padStart(3, "0")
来源：http://wjq.shanyushiyangkeji.top

[U113] JS：正则替换全部
来源：http://yjl.daria6918.cn

s.replaceAll("a", "b")
来源：http://nbv.yangfankeji.com

[U114] JS：JSON 深比较
来源：http://bbv.feifeiyinyue.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://eni.svipenyu.cn

[U115] JS：生成 UUID
来源：http://jgb.guowangkeji.top

crypto.randomUUID()
来源：http://gzp.yvedp.cn

[U116] JS：类型检查（JSDoc）
来源：http://bca.shuidangran.top

/** @param {string} name */ function f(name) {}
来源：http://juh.jyoumei.cn

[U117] JS：单元测试
来源：http://utx.iojbl.cn

npm i -D vitest;  npx vitest
来源：http://bvp.jinyuanbaomall.cn

[U118] JS：开发服务器
来源：http://hcv.xylfe.cn

npm i -D vite;  npx vite
来源：http://bxr.yanxiufei.cn

[U119] JS：生产构建
来源：http://hyl.jlsjyb.cn

npx vite build
来源：http://fus.yfazqb.com

[U120] JS：读取环境变量（Vite）
来源：http://smy.guowangkeji.top

import.meta.env.VITE_API_URL
来源：http://vyt.zhijiandao.cn

================================================================================
来源：http://qcv.haohaochexian.top

统计汇总
来源：http://bsk.bjfxy.top

================================================================================
来源：http://tty.shanyushiyangkeji.top

按语言统计（条）：
来源：http://uzj.xingfuxueyuan.xyz

Python ......... 252
来源：http://tzy.gaohongyu789.top

PHP ............ 252
来源：http://bne.fehbvm.com

JavaScript ..... 252
来源：http://egm.yfazqb.com

TypeScript ..... 212
来源：http://yqx.316326.xyz

Java ........... 212
来源：http://ban.wangshuangyany.cn

Go ............. 212
来源：http://oij.zhaomingkeji.xyz

Ruby ........... 212
来源：http://hsr.chenlongwang.top

C# ............. 212
来源：http://mkv.sjlbkw.cn

C .............. 30
来源：http://qwt.52xcode.cn

C++ ............ 30
来源：http://apc.aizwys.cn

SQL ............ 90
来源：http://vin.jinqigufen.top

Bash ........... 80
来源：http://gkw.sufxvd.cn

Kotlin ......... 15
来源：http://wfr.cucudq.cn

Swift .......... 15
来源：http://ses.uphjek.com

Lua ............ 10
来源：http://rgp.tianlin.xyz

Perl ........... 10
来源：http://ejx.hnqzz.top

Scala .......... 10
来源：http://wtt.zhaomingkeji.xyz

------------------------------------
来源：http://xxm.sufxvd.cn

合计 ........... 2106 条
来源：http://rjd.yj20258.top

按章节统计：
来源：http://nup.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zkz.fktsv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://una.yueranfly.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bfv.quarkkingdee.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bss.sxryk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://avz.hnxiangtu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rcd.jlsjyb.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ypf.ivvv.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ujr.ywan-chungtsiang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dqt.guowangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bcv.tianlin.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ene.zdbjq.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yvi.xziqi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kuu.shanyushiyangtech.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fpb.uphjek.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://llv.chenlongwang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://clp.hfpthk.cn

Q SQL 专题                              90
来源：http://ehb.zdbjq.cn

R Bash 专题                             80
来源：http://lcc.hnqzz.top

S C / C++ 专题                          60
来源：http://btz.zhongyouzk.top

T 其他语言补充                          60
来源：http://kax.cucudq.cn

U 高频实用片段                         120
来源：http://gnf.fanxiaobao.xyz

------------------------------------
来源：http://jjv.9152youxi.cn

合计                                  2106 条
来源：http://fhr.tian-w.cn

--------------------------------------------------------------------------------
来源：http://apq.shanyushiyangtech.top

使用提醒
来源：http://sev.xuanzx.com

--------------------------------------------------------------------------------
来源：http://hie.gzhubu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hjc.pycfn.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xsg.ppjwa.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rdf.daria6918.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zhf.dianchejie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ezz.yuxming.cn

—— 文件结束 ——
来源：http://ufo.shuidangran.top

================================================================================
来源：http://ija.zycfv.cn

程序语言常见例子速查手册（2024 版）
来源：http://rbe.xuanzx.com

Common Programming Examples Cheat Book
来源：http://qyi.zdbjq.cn

================================================================================
来源：http://dgl.zdbjq.cn

【收录内容】
来源：http://sot.mhx1999.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ayq.ivvv.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dmx.zhixingplan.top

SQL · Bash · C · C++
来源：http://azv.hongshengwenyu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ysm.jianghu66.top

【使用说明】
来源：http://kgg.sjlbkw.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://new.aizwys.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ajx.quarkkingdee.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eoe.jqgfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://iso.mhx1999.top

Bash:  Shell         C:     C             C++:   C++
来源：http://cvz.jiagoushi.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dkz.zhijiandao.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://guw.0kj1m.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hul.shangyingyoupin.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wlh.quarkkingdee.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wat.dashuyun.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wus.fanxiaobao.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gyf.xuetiantiany.cn

【文件统计】
来源：http://fep.snrcjt.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xju.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://ycs.yvedp.cn

目  录
来源：http://hjy.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://aoy.yanxiufei.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gbj.yangfankeji.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hml.chenlongwang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kep.9152youxi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bbb.bbcook.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ecb.ydzc1.top


<!-- 参考信息 -->