代发 wailian999

[U07] Py：反转字典键值
来源：http://hik.jiagoushi.top

{v: k for k, v in d.items()}
来源：http://ytj.316326.xyz

[U08] Py：展平二维列表
来源：http://upu.hnxiangtu.top

[y for x in nested for y in x]
来源：http://pra.yongpay.top

[U09] Py：字典取最大值的键
来源：http://opi.pycfn.com

max(d, key=d.get)
来源：http://ffp.zhaomingkeji.xyz

[U10] Py：按值排序字典
来源：http://zes.zhoulong.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vbc.fehbvm.com

[U11] Py：生成器表达式
来源：http://unl.daria6918.cn

(x * 2 for x in arr)
来源：http://scj.ywan-chungtsiang.top

[U12] Py：取出现最多的 3 个元素
来源：http://hrw.nwbrower.top

Counter(arr).most_common(3)
来源：http://pez.zhengqikj.top

[U13] Py：固定长度队列
来源：http://icu.fzhhl.top

deque(maxlen=10)
来源：http://xtx.ydjk.org.cn

[U14] Py：分组收集到列表
来源：http://sly.ctjpmb.com

defaultdict(list)
来源：http://pla.9152youxi.cn

[U15] Py：高精度计时
来源：http://stf.ybcxt.top

t = time.perf_counter()
来源：http://xgb.chenjidiqi.icu

[U16] Py：命令行参数解析
来源：http://ykq.fengsongda.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pnh.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://vzc.yonumen.top

logging.basicConfig(level=logging.INFO)
来源：http://sov.0kj1m.cn

[U18] Py：预编译正则
来源：http://ibl.zycfv.cn

pat = re.compile(r"\d+")
来源：http://ncj.svipenyu.cn

[U19] Py：正则替换带回调
来源：http://bzj.nanxuanxn.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://odo.jyoumei.cn

[U20] Py：缓存函数结果
来源：http://wbj.zhengqikj.top

@functools.lru_cache(maxsize=None)
来源：http://zvh.ydjk.org.cn

[U21] Py：自定义上下文管理器
来源：http://xtx.shanyushiyangtech.top

@contextlib.contextmanager
来源：http://mcz.dashuyun.cn

[U22] Py：矩阵转置
来源：http://ttv.cdnleiting.top

list(zip(*m))
来源：http://cmf.shanyushiyangtech.top

[U23] Py：分块读取大文件
来源：http://zod.redwolf501.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dxu.vqdsnc.cn

[U24] Py：路径操作
来源：http://pdv.feifeiyinyue.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ytj.zhaomingkeji.xyz

[U25] Py：CSV 按字典读
来源：http://wrq.feifeiyinyue.top

csv.DictReader(f)
来源：http://slq.cqqwz.cn

[U26] Py：并发下载
来源：http://ktp.zhixingplan.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rmm.tarul.cn

[U27] Py：异步 HTTP
来源：http://ktt.aibaodan.cn

aiohttp.ClientSession() 配合 async with
来源：http://klj.andypj.xyz

[U28] Py：类型别名
来源：http://rda.jinqigufen.top

UserId = int
来源：http://ekt.vqdsnc.cn

[U29] Py：属性校验
来源：http://znk.sysykeji.top

@property 与 @x.setter 配合
来源：http://yys.nwbrower.top

[U30] Py：数据类
来源：http://rcn.cashguo.top

@dataclass(slots=True)
来源：http://zpv.hysaishi.cn

[U31] Py：单测
来源：http://tuq.daxiang520.top

python -m pytest -q
来源：http://pil.yueranfly.top

[U32] Py：代码格式化
来源：http://yzv.quarkkingdee.top

ruff format . && ruff check --fix .
来源：http://tab.xuetiantiany.cn

[U33] Py：打包发布
来源：http://mjc.sufxvd.cn

python -m build  （依赖 pyproject.toml）
来源：http://qwu.jinqigufen.top

[U34] Py：判断编码
来源：http://pup.fehbvm.com

chardet.detect(raw)
来源：http://nhh.zdqjudy.top

[U35] Py：发送邮件
来源：http://jam.xuanzx.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nuw.jinqigufen.top

[U36] Py：定时任务
来源：http://dxb.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://mgd.havefunace.top

[U37] Py：读写 Excel
来源：http://aqc.xuanzx.com

pandas.read_excel / DataFrame.to_excel
来源：http://omu.xziqi.cn

[U38] Py：获取脚本所在目录
来源：http://unk.yj20258888.top

Path(__file__).resolve().parent
来源：http://rto.hfpthk.cn

[U39] Py：判断是否在交互环境
来源：http://qep.vqdsnc.cn

sys.stdout.isatty()
来源：http://naa.ppjwa.cn

[U40] Py：打印到标准错误
来源：http://itm.feifeiyinyue.top

print("err", file=sys.stderr)
来源：http://jfp.jqgufenzy.top

[U41] PHP：初始化 Composer 项目
来源：http://hra.jinghuilouyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mpd.sjlbkw.cn

[U42] PHP：PSR-4 自动加载
来源：http://mdc.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ora.dashuyun.cn

[U43] PHP：声明命名空间
来源：http://ydg.hammf.cn

namespace App\Http;
来源：http://dmk.zhiwuduotai.top

[U44] PHP：开启严格类型
来源：http://hbr.hysaishi.cn

declare(strict_types=1);
来源：http://jze.epnwcf.com

[U45] PHP：类型声明与返回类型
来源：http://qtq.birdmap.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://dud.uphjek.com

[U46] PHP：可空类型
来源：http://yel.fehbvm.com

?string $name = null
来源：http://wim.yangfankeji.com

[U47] PHP：联合类型
来源：http://iyi.xziqi.cn

int|string $id
来源：http://fqa.gogol.net.cn

[U48] PHP：纯枚举
来源：http://zhb.zhongyouzk.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ati.ppjwa.cn

[U49] PHP：只读属性
来源：http://mxn.dianchejie.cn

public readonly string $name
来源：http://yny.fktsv.cn

[U50] PHP：构造器属性提升
来源：http://hyf.gotoacloud.top

public function __construct(private int $id) {}
来源：http://pur.iojbl.cn

[U51] PHP：数组解构
来源：http://lzs.jinqigfzy.top

[$a, $b] = $arr;
来源：http://bto.zdbjq.cn

[U52] PHP：箭头函数
来源：http://ods.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://uey.wangdashe.top

[U53] PHP：空合并运算符
来源：http://elt.dianchejie.cn

$v = $a ?? $b ?? "default";
来源：http://bkw.mhx1999.top

[U54] PHP：空安全调用
来源：http://rbs.andypj.xyz

$obj?->method()
来源：http://vvj.shzxlz.cn

[U55] PHP：match 表达式
来源：http://riw.shangyingyoupin.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jej.yuanzhike.top

[U56] PHP：命名参数
来源：http://wwa.fktsv.cn

f(a: 1, b: 2)
来源：http://itf.birdmap.top

[U57] PHP：字符串插值
来源：http://vld.bjfxy.top

"值: {$a}"
来源：http://ndh.zdbjq.cn

[U58] PHP：数组三件套
来源：http://daw.andypj.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ska.jinyuanbaomall.cn

[U59] PHP：自定义排序
来源：http://std.pengpengdd.cyou

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zzh.jiagoushi.top

[U60] PHP：JSON 编解码
来源：http://yxy.nwbrower.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ncu.zycfv.cn

[U61] PHP：正则
来源：http://fca.zhiwuduotai.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gxm.jinyuanbaomall.cn

[U62] PHP：日期对象
来源：http://ymy.zdbjq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lnl.zhixingplan.top

[U63] PHP：文件读写
来源：http://yat.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eor.iojbl.cn

[U64] PHP：目录遍历
来源：http://hlk.svipenyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://tut.xylfe.cn

[U65] PHP：会话
来源：http://ncd.redwolf501.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ifo.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://gka.zhiwuduotai.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tac.jqgufenzy.top

[U67] PHP：处理文件上传
来源：http://tyy.wangdashe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://smj.fzhhl.top

[U68] PHP：PDO 连接
来源：http://glh.sysykeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vgh.ivvv.top

[U69] PHP：PDO 预处理
来源：http://vqe.shzxlz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qnx.kuanghao11.cn

[U70] PHP：PDO 事务
来源：http://uzi.pycfn.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hgo.nwbrower.top

[U71] PHP：抛出异常
来源：http://qwd.jinghuilouyu.cn

throw new RuntimeException("失败", 500);
来源：http://lqp.yanxiufei.cn

[U72] PHP：写错误日志
来源：http://gsm.daria6918.cn

error_log("失败: " . $e->getMessage());
来源：http://vqm.zhengqikj.top

[U73] PHP：读取 ini 配置
来源：http://azp.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://asf.xylfe.cn

[U74] PHP：读取环境变量
来源：http://xyi.yanxiufei.cn

getenv("APP_ENV") ?: "production"
来源：http://kdu.pengpengdd.cyou

[U75] PHP：依赖注入
来源：http://rkn.xinyue.icu

composer require psr/container
来源：http://emr.sxryk.cn

[U76] PHP：简单路由
来源：http://ywb.chenjidiqi.icu

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hzs.nanxuanxn.top

[U77] PHP：模板渲染
来源：http://rbw.iojbl.cn

composer require twig/twig
来源：http://plo.hongshengwenyu.top

[U78] PHP：单元测试
来源：http://dfv.hnqzz.top

composer require --dev phpunit/phpunit
来源：http://dqr.nanxinkj.top

[U79] PHP：静态分析
来源：http://owt.yueranfly.top

composer require --dev phpstan/phpstan
来源：http://boc.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://urh.daxiang520.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ery.jqgfzy.top

[U81] JS：初始化项目
来源：http://xot.gzhubu.top

npm init -y;  npm i express
来源：http://aor.sweek.top

[U82] JS：package.json 脚本
来源：http://xhd.aibaodan.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iui.52xcode.cn

[U83] JS：ES Module 导入导出
来源：http://lgc.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://frk.52xcode.cn

[U84] JS：CommonJS 写法
来源：http://pyy.hammf.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gjl.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://muz.havefunace.top

a?.b?.c
来源：http://bub.hfpthk.cn

[U86] JS：空值合并
来源：http://fcp.dianchejie.cn

a ?? b
来源：http://gzs.daria6918.cn

[U87] JS：解构默认值
来源：http://bgs.vqdsnc.cn

const { a = 1, b = 2 } = obj;
来源：http://hik.chenzaomai.com

[U88] JS：对象展开合并
来源：http://qcq.dashuyun.cn

{ ...a, ...b }
来源：http://pav.52xcode.cn

[U89] JS：数组去重
来源：http://qxf.pycfn.com

[...new Set(arr)]
来源：http://wre.yuanzhike.top

[U90] JS：数字数组排序
来源：http://fif.pengpengdd.cyou

[...arr].sort((a, b) => a - b)
来源：http://fhw.shuidangran.top

[U91] JS：对象键值遍历
来源：http://lvz.jinqigfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://don.xinyue.icu

[U92] JS：深拷贝
来源：http://tez.sweek.top

structuredClone(obj)
来源：http://xzp.hnxiangtu.top

[U93] JS：模板字符串
来源：http://zey.yuxming.cn

`共 ${n} 条`
来源：http://pgf.svipenyu.cn

[U94] JS：箭头函数
来源：http://azs.zhaomingkeji.xyz

const double = x => x * 2;
来源：http://mir.zhiwuduotai.top

[U95] JS：Promise 包装
来源：http://gjy.tanke756.top

new Promise((resolve, reject) => {})
来源：http://utn.mhx1999.top

[U96] JS：async/await 与异常
来源：http://mpz.hongshengwenyu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hwk.sxryk.cn

[U97] JS：并发请求
来源：http://inq.hammf.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://idt.snrcjt.cn

[U98] JS：fetch 带 JSON
来源：http://uhd.birdmap.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ukr.yonumen.top

[U99] JS：事件监听
来源：http://wzw.zdqjudy.top

el.addEventListener("click", e => {})
来源：http://vtd.ydzc1.top

[U100] JS：DOM 查询
来源：http://emb.zhongyouzk.top

document.querySelector(".item")
来源：http://tke.haohaochexian.top

[U101] JS：classList 操作
来源：http://uwr.hesvh.cn

el.classList.toggle("active")
来源：http://mnm.iojbl.cn

[U102] JS：本地存储
来源：http://tuo.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rzw.snrcjt.cn

[U103] JS：定时器
来源：http://wed.jinqigfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ryn.gotoacloud.top

[U104] JS：防抖
来源：http://ufx.zhixingplan.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hvv.fktsv.cn

[U105] JS：节流
来源：http://jkq.gogol.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bio.zhengqikj.top

[U106] JS：日期格式化
来源：http://rep.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mzm.jinghuilouyu.cn

[U107] JS：数字千分位
来源：http://ehq.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ylb.feifeiyinyue.top

[U108] JS：随机整数
来源：http://zwd.zhixingplan.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jjq.jyoumei.cn

[U109] JS：数组分组
来源：http://dzf.xuanzx.com

Object.groupBy(arr, x => x.type)
来源：http://vdy.uphjek.com

[U110] JS：数组分块
来源：http://rsu.guannengcc.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kik.fktsv.cn

[U111] JS：对象转 Map
来源：http://igl.zdbjq.cn

new Map(Object.entries(obj))
来源：http://hjo.yanxiufei.cn

[U112] JS：字符串补位
来源：http://nlu.vehdjk.com

"7".padStart(3, "0")
来源：http://jdn.daria6918.cn

[U113] JS：正则替换全部
来源：http://esn.yuxming.cn

s.replaceAll("a", "b")
来源：http://oiv.sjlbkw.cn

[U114] JS：JSON 深比较
来源：http://moi.hfpthk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dvq.quarkkingdee.top

[U115] JS：生成 UUID
来源：http://jlq.vqdsnc.cn

crypto.randomUUID()
来源：http://dnb.hesvh.cn

[U116] JS：类型检查（JSDoc）
来源：http://iyy.havefunace.top

/** @param {string} name */ function f(name) {}
来源：http://mni.yfazqb.com

[U117] JS：单元测试
来源：http://eea.zhengqikj.top

npm i -D vitest;  npx vitest
来源：http://ccl.hongshengwenyu.top

[U118] JS：开发服务器
来源：http://zmx.jinyuanbaomall.cn

npm i -D vite;  npx vite
来源：http://cmd.yuanzhike.top

[U119] JS：生产构建
来源：http://uwd.yj202588.top

npx vite build
来源：http://xfd.vqdsnc.cn

[U120] JS：读取环境变量（Vite）
来源：http://xju.tarul.cn

import.meta.env.VITE_API_URL
来源：http://lkv.jyoumei.cn

================================================================================
来源：http://bgl.jianghu66.top

统计汇总
来源：http://mab.dashuyun.cn

================================================================================
来源：http://pwz.52xcode.cn

按语言统计（条）：
来源：http://ufw.jiagoushi.top

Python ......... 252
来源：http://wqn.xuanzx.com

PHP ............ 252
来源：http://lcp.jinqigfzy.top

JavaScript ..... 252
来源：http://fit.dianchejie.cn

TypeScript ..... 212
来源：http://pmo.pycfn.com

Java ........... 212
来源：http://krb.chenjidiqi.icu

Go ............. 212
来源：http://gft.hywenlv.cn

Ruby ........... 212
来源：http://bqa.hcnkem.com

C# ............. 212
来源：http://qto.haohaochexian.top

C .............. 30
来源：http://nhy.aibaodan.cn

C++ ............ 30
来源：http://ocp.guannengcc.top

SQL ............ 90
来源：http://jol.yonumen.top

Bash ........... 80
来源：http://rdo.andypj.xyz

Kotlin ......... 15
来源：http://qxb.cucudq.cn

Swift .......... 15
来源：http://uck.hfpthk.cn

Lua ............ 10
来源：http://ikg.ppjwa.cn

Perl ........... 10
来源：http://brm.yonumen.top

Scala .......... 10
来源：http://ujr.smart0.xyz

------------------------------------
来源：http://dlx.hesvh.cn

合计 ........... 2106 条
来源：http://aub.xziqi.cn

按章节统计：
来源：http://uks.iojbl.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oxr.sysykeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vmm.0kj1m.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ini.yongpay.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xfi.gogol.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://glj.yuanzhike.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ulb.fengsongda.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kre.yonumen.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://slu.jinyuanbaomall.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dkd.quarkkingdee.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://epo.shzxlz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oqc.316326.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ulk.kuanghao11.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gie.yvedp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://txt.nwbrower.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zby.yangfankeji.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sjg.c1oappe.top

Q SQL 专题                              90
来源：http://dtv.vqdsnc.cn

R Bash 专题                             80
来源：http://lfy.redwolf501.top

S C / C++ 专题                          60
来源：http://otp.ivvv.top

T 其他语言补充                          60
来源：http://edx.yangfankeji.com

U 高频实用片段                         120
来源：http://rmu.ivvv.top

------------------------------------
来源：http://xxl.yonumen.top

合计                                  2106 条
来源：http://ygx.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://vcg.daria6918.cn

使用提醒
来源：http://wxk.hammf.cn

--------------------------------------------------------------------------------
来源：http://kyp.vqdsnc.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hxu.zhiwuduotai.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kox.bjfxy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eju.cheryme.top

在旧版本上使用前请先确认语法支持情况。
来源：http://byc.ivvv.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uxh.yj202588.top

—— 文件结束 ——
来源：http://gty.zdbjq.cn

================================================================================
来源：http://rlw.quarkkingdee.top

程序语言常见例子速查手册（2024 版）
来源：http://dct.tian-w.cn

Common Programming Examples Cheat Book
来源：http://exi.gogol.net.cn

================================================================================
来源：http://nto.zhiwuduotai.top

【收录内容】
来源：http://xkj.jqgufenzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vpc.zdqjudy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nin.feifeiyinyue.top

SQL · Bash · C · C++
来源：http://jap.hysaishi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fcy.xziqi.cn

【使用说明】
来源：http://pyj.fanxiaobao.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pln.jlsjyb.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nwa.daxiang520.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://czr.jqgfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qkd.jqgufenzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://eji.gzhubu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uhi.ivvv.top


<!-- 参考信息 -->