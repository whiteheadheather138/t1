代发 wailian999

[U15] Py：高精度计时
来源：http://wdw.jinyuanbaomall.cn

t = time.perf_counter()
来源：http://bnx.vehdjk.com

[U16] Py：命令行参数解析
来源：http://nwq.bbcook.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bub.ctjpmb.com

[U17] Py：初始化日志
来源：http://ala.bbcook.cn

logging.basicConfig(level=logging.INFO)
来源：http://tqt.jqgfzy.top

[U18] Py：预编译正则
来源：http://hwd.feifeiyinyue.top

pat = re.compile(r"\d+")
来源：http://uhn.yj20258888.top

[U19] Py：正则替换带回调
来源：http://tdc.jlsjyb.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zfx.yonumen.top

[U20] Py：缓存函数结果
来源：http://txf.ywan-chungtsiang.top

@functools.lru_cache(maxsize=None)
来源：http://lzo.zhongyouzk.top

[U21] Py：自定义上下文管理器
来源：http://jtr.yangfankeji.com

@contextlib.contextmanager
来源：http://kbt.yonumen.top

[U22] Py：矩阵转置
来源：http://ytc.dashuyun.cn

list(zip(*m))
来源：http://pvg.fanxiaobao.xyz

[U23] Py：分块读取大文件
来源：http://eus.wangdashe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jwc.nanxuanxn.top

[U24] Py：路径操作
来源：http://ckn.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://epv.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://zqa.uphjek.com

csv.DictReader(f)
来源：http://mcj.mhx1999.top

[U26] Py：并发下载
来源：http://otq.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lrw.ywan-chungtsiang.top

[U27] Py：异步 HTTP
来源：http://vxw.ehwqpu.com

aiohttp.ClientSession() 配合 async with
来源：http://pmn.ydjk.org.cn

[U28] Py：类型别名
来源：http://ctn.jqgufenzy.top

UserId = int
来源：http://jez.jqgufenzy.top

[U29] Py：属性校验
来源：http://omk.vehdjk.com

@property 与 @x.setter 配合
来源：http://fcm.yuanzhike.top

[U30] Py：数据类
来源：http://kto.iojbl.cn

@dataclass(slots=True)
来源：http://ovs.havefunace.top

[U31] Py：单测
来源：http://rxf.ybcxt.top

python -m pytest -q
来源：http://qnt.pengpengdd.cyou

[U32] Py：代码格式化
来源：http://pdt.aizwys.cn

ruff format . && ruff check --fix .
来源：http://wsj.xylfe.cn

[U33] Py：打包发布
来源：http://zmo.yj202588.top

python -m build  （依赖 pyproject.toml）
来源：http://caa.sjlbkw.cn

[U34] Py：判断编码
来源：http://dwp.9152youxi.cn

chardet.detect(raw)
来源：http://kvo.yuanzhike.top

[U35] Py：发送邮件
来源：http://uhi.zhijiandao.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wgl.shangyingyoupin.top

[U36] Py：定时任务
来源：http://jmp.zhengqikj.top

schedule.every(10).minutes.do(job)
来源：http://oaa.zhiwuduotai.top

[U37] Py：读写 Excel
来源：http://fvl.ydzc1.top

pandas.read_excel / DataFrame.to_excel
来源：http://hgh.hysaishi.cn

[U38] Py：获取脚本所在目录
来源：http://fnf.chenlongwang.top

Path(__file__).resolve().parent
来源：http://uqo.jinqigufen.top

[U39] Py：判断是否在交互环境
来源：http://lkk.fktsv.cn

sys.stdout.isatty()
来源：http://aos.ydjk.org.cn

[U40] Py：打印到标准错误
来源：http://mks.nanxinkj.top

print("err", file=sys.stderr)
来源：http://mxl.sweek.top

[U41] PHP：初始化 Composer 项目
来源：http://eyc.guannengcc.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mtb.chenjidiqi.icu

[U42] PHP：PSR-4 自动加载
来源：http://pdf.nanxuanxn.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cnc.hywenlv.cn

[U43] PHP：声明命名空间
来源：http://zxn.guannengcc.top

namespace App\Http;
来源：http://muh.yj202588.top

[U44] PHP：开启严格类型
来源：http://ioy.aibaodan.cn

declare(strict_types=1);
来源：http://esm.fzhhl.top

[U45] PHP：类型声明与返回类型
来源：http://cbi.zdbjq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://grt.yfazqb.com

[U46] PHP：可空类型
来源：http://ppq.yj20258.top

?string $name = null
来源：http://aca.jiagoushi.top

[U47] PHP：联合类型
来源：http://fee.ydjk.org.cn

int|string $id
来源：http://uku.fktsv.cn

[U48] PHP：纯枚举
来源：http://ghh.dianchejie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nnu.c1oappe.top

[U49] PHP：只读属性
来源：http://sdt.xylfe.cn

public readonly string $name
来源：http://ngv.jinghuilouyu.cn

[U50] PHP：构造器属性提升
来源：http://pzl.ctjpmb.com

public function __construct(private int $id) {}
来源：http://mns.shzxlz.cn

[U51] PHP：数组解构
来源：http://qgj.gotoacloud.top

[$a, $b] = $arr;
来源：http://xpw.ctjpmb.com

[U52] PHP：箭头函数
来源：http://bfp.sufxvd.cn

$double = fn($x) => $x * 2;
来源：http://wvh.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://lvg.zhiwuduotai.top

$v = $a ?? $b ?? "default";
来源：http://woo.nwbrower.top

[U54] PHP：空安全调用
来源：http://ffk.yangfankeji.com

$obj?->method()
来源：http://pdn.jinqigfzy.top

[U55] PHP：match 表达式
来源：http://kfi.tarul.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xma.tanke756.top

[U56] PHP：命名参数
来源：http://obb.ppjwa.cn

f(a: 1, b: 2)
来源：http://flf.smart0.xyz

[U57] PHP：字符串插值
来源：http://ovo.vqdsnc.cn

"值: {$a}"
来源：http://aqj.c1oappe.top

[U58] PHP：数组三件套
来源：http://hui.hywenlv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dzw.316326.xyz

[U59] PHP：自定义排序
来源：http://fas.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ppv.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://fel.xuanzx.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kzw.shanyushiyangtech.top

[U61] PHP：正则
来源：http://qda.chenlongwang.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gxc.ydzc1.top

[U62] PHP：日期对象
来源：http://fbi.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bql.gogol.net.cn

[U63] PHP：文件读写
来源：http://str.chenjidiqi.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vrv.smart0.xyz

[U64] PHP：目录遍历
来源：http://hbg.xziqi.cn

glob("dir/*.php");  scandir("dir");
来源：http://xgb.tarul.cn

[U65] PHP：会话
来源：http://zpo.xuanzx.com

session_start();  $_SESSION["uid"] = 1;
来源：http://egt.gzhubu.top

[U66] PHP：设置 Cookie
来源：http://coq.pengpengdd.cyou

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hjl.aibaodan.cn

[U67] PHP：处理文件上传
来源：http://mpr.jianghu66.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://edu.hnxiangtu.top

[U68] PHP：PDO 连接
来源：http://kjd.uphjek.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gwq.xylfe.cn

[U69] PHP：PDO 预处理
来源：http://hnk.yueranfly.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dhj.vehdjk.com

[U70] PHP：PDO 事务
来源：http://pfd.hesvh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jqy.shzxlz.cn

[U71] PHP：抛出异常
来源：http://jcw.daria6918.cn

throw new RuntimeException("失败", 500);
来源：http://nwz.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://fvg.aizwys.cn

error_log("失败: " . $e->getMessage());
来源：http://fui.nanxinkj.top

[U73] PHP：读取 ini 配置
来源：http://odg.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://osf.tianlin.xyz

[U74] PHP：读取环境变量
来源：http://ryo.cucudq.cn

getenv("APP_ENV") ?: "production"
来源：http://gip.daria6918.cn

[U75] PHP：依赖注入
来源：http://mbn.shzxlz.cn

composer require psr/container
来源：http://ugt.jlsjyb.cn

[U76] PHP：简单路由
来源：http://uqv.dianchejie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kwq.jiagoushi.top

[U77] PHP：模板渲染
来源：http://zap.wangshuangyany.cn

composer require twig/twig
来源：http://rlz.tanke756.top

[U78] PHP：单元测试
来源：http://coa.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://uot.yueranfly.top

[U79] PHP：静态分析
来源：http://sji.chenlongwang.top

composer require --dev phpstan/phpstan
来源：http://vow.uphjek.com

[U80] PHP：代码规范修复
来源：http://kvj.zhiwuduotai.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://drc.birdmap.top

[U81] JS：初始化项目
来源：http://kfn.zhoulong.xyz

npm init -y;  npm i express
来源：http://eql.fengsongda.top

[U82] JS：package.json 脚本
来源：http://iwf.gzhubu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zeo.zhengqikj.top

[U83] JS：ES Module 导入导出
来源：http://jpd.ywan-chungtsiang.top

export const a = 1;  import { a } from "./m.js";
来源：http://bzs.xinyue.icu

[U84] JS：CommonJS 写法
来源：http://yum.pengpengdd.cyou

module.exports = { a };  const { a } = require("./m");
来源：http://jnv.hongshengwenyu.top

[U85] JS：可选链
来源：http://sfi.yuxming.cn

a?.b?.c
来源：http://wqo.yonumen.top

[U86] JS：空值合并
来源：http://lmf.tanke756.top

a ?? b
来源：http://ebz.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://qjo.hysaishi.cn

const { a = 1, b = 2 } = obj;
来源：http://ilc.jiagoushi.top

[U88] JS：对象展开合并
来源：http://zoo.sufxvd.cn

{ ...a, ...b }
来源：http://ftr.guowangkeji.top

[U89] JS：数组去重
来源：http://dry.xingfuxueyuan.xyz

[...new Set(arr)]
来源：http://cld.hywenlv.cn

[U90] JS：数字数组排序
来源：http://mll.xziqi.cn

[...arr].sort((a, b) => a - b)
来源：http://ssj.feifeiyinyue.top

[U91] JS：对象键值遍历
来源：http://dva.yangfankeji.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://son.dashuyun.cn

[U92] JS：深拷贝
来源：http://ull.ctjpmb.com

structuredClone(obj)
来源：http://nbj.chenzaomai.com

[U93] JS：模板字符串
来源：http://xxl.feifeiyinyue.top

`共 ${n} 条`
来源：http://rto.sysykeji.top

[U94] JS：箭头函数
来源：http://epe.pengpengdd.cyou

const double = x => x * 2;
来源：http://cki.zycfv.cn

[U95] JS：Promise 包装
来源：http://nqe.guowangkeji.top

new Promise((resolve, reject) => {})
来源：http://fir.zdbjq.cn

[U96] JS：async/await 与异常
来源：http://ehb.xylfe.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://azs.yuxming.cn

[U97] JS：并发请求
来源：http://xxk.feifeiyinyue.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mzm.ybcxt.top

[U98] JS：fetch 带 JSON
来源：http://job.chenjidiqi.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tdx.xuetiantiany.cn

[U99] JS：事件监听
来源：http://niz.daria6918.cn

el.addEventListener("click", e => {})
来源：http://xgh.tian-w.cn

[U100] JS：DOM 查询
来源：http://lvx.ppjwa.cn

document.querySelector(".item")
来源：http://xmb.cucudq.cn

[U101] JS：classList 操作
来源：http://xje.hnxiangtu.top

el.classList.toggle("active")
来源：http://ufh.cdnleiting.top

[U102] JS：本地存储
来源：http://frd.yvedp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://plb.mhx1999.top

[U103] JS：定时器
来源：http://nvn.shangyingyoupin.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ulg.vehdjk.com

[U104] JS：防抖
来源：http://uyw.cashguo.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://abn.zdbjq.cn

[U105] JS：节流
来源：http://axa.zhiwuduotai.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iib.vqdsnc.cn

[U106] JS：日期格式化
来源：http://ffq.yfazqb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zie.316326.xyz

[U107] JS：数字千分位
来源：http://ayy.yvedp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iiz.cdnleiting.top

[U108] JS：随机整数
来源：http://frj.hnqzz.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oea.ydzc1.top

[U109] JS：数组分组
来源：http://gvb.chenzaomai.com

Object.groupBy(arr, x => x.type)
来源：http://yyq.jianghu66.top

[U110] JS：数组分块
来源：http://uwi.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mwb.dashuyun.cn

[U111] JS：对象转 Map
来源：http://tay.ppjwa.cn

new Map(Object.entries(obj))
来源：http://nbt.yj202588.top

[U112] JS：字符串补位
来源：http://jpo.ydzc1.top

"7".padStart(3, "0")
来源：http://vqf.chenlongwang.top

[U113] JS：正则替换全部
来源：http://ogr.vehdjk.com

s.replaceAll("a", "b")
来源：http://mde.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://zdx.chenjidiqi.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://kbo.yuanzhike.top

[U115] JS：生成 UUID
来源：http://sxg.fengsongda.top

crypto.randomUUID()
来源：http://avg.yuanzhike.top

[U116] JS：类型检查（JSDoc）
来源：http://dwk.hnxiangtu.top

/** @param {string} name */ function f(name) {}
来源：http://udj.shzxlz.cn

[U117] JS：单元测试
来源：http://bpn.svipenyu.cn

npm i -D vitest;  npx vitest
来源：http://jwf.vqdsnc.cn

[U118] JS：开发服务器
来源：http://pvv.haohaochexian.top

npm i -D vite;  npx vite
来源：http://kdx.iojbl.cn

[U119] JS：生产构建
来源：http://zlo.wangshuangyany.cn

npx vite build
来源：http://mtb.zhaomingkeji.xyz

[U120] JS：读取环境变量（Vite）
来源：http://lgt.feifeiyinyue.top

import.meta.env.VITE_API_URL
来源：http://rlb.ywan-chungtsiang.top

================================================================================
来源：http://tqs.yvedp.cn

统计汇总
来源：http://zmk.cqqwz.cn

================================================================================
来源：http://qyh.yuxming.cn

按语言统计（条）：
来源：http://cgg.iojbl.cn

Python ......... 252
来源：http://vzv.cashguo.top

PHP ............ 252
来源：http://psh.quarkkingdee.top

JavaScript ..... 252
来源：http://skq.hnqzz.top

TypeScript ..... 212
来源：http://jca.zhongyouzk.top

Java ........... 212
来源：http://nyc.tianlin.xyz

Go ............. 212
来源：http://xrb.meibo888.top

Ruby ........... 212
来源：http://wkj.cdnleiting.top

C# ............. 212
来源：http://vct.nanxuanxn.top

C .............. 30
来源：http://lzw.ctjpmb.com

C++ ............ 30
来源：http://zan.tarul.cn

SQL ............ 90
来源：http://jqc.mhx1999.top

Bash ........... 80
来源：http://tln.ppjwa.cn

Kotlin ......... 15
来源：http://ado.jyoumei.cn

Swift .......... 15
来源：http://ygm.snrcjt.cn

Lua ............ 10
来源：http://tvx.ydzc1.top

Perl ........... 10
来源：http://zmm.zhijiandao.cn

Scala .......... 10
来源：http://lcp.tarul.cn

------------------------------------
来源：http://iyz.xinyue.icu

合计 ........... 2106 条
来源：http://dxr.cqqwz.cn

按章节统计：
来源：http://nvz.hcnkem.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oby.sweek.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bbx.zhongyouzk.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dwo.shuidangran.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fsk.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rnx.hywenlv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rwu.9152youxi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://aqo.ybcxt.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dti.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tql.sweek.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://txw.fzhhl.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mwa.daria6918.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ies.havefunace.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vyk.chenjidiqi.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yxz.ctjpmb.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://klp.zhiwuduotai.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dtw.guannengcc.top

Q SQL 专题                              90
来源：http://ubp.hnxiangtu.top

R Bash 专题                             80
来源：http://obh.jianghu66.top

S C / C++ 专题                          60
来源：http://smm.zdbjq.cn

T 其他语言补充                          60
来源：http://roq.hnqzz.top

U 高频实用片段                         120
来源：http://utd.tanke756.top

------------------------------------
来源：http://oud.aibaodan.cn

合计                                  2106 条
来源：http://qza.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://rzl.yongpay.top

使用提醒
来源：http://xmo.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://oke.cqqwz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yis.yongpay.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xxq.cheryme.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hvr.ppjwa.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dgh.shanyushiyangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nms.yongpay.top

—— 文件结束 ——
来源：http://tdl.birdmap.top

================================================================================
来源：http://ycy.gotoacloud.top

程序语言常见例子速查手册（2024 版）
来源：http://cbz.ctjpmb.com

Common Programming Examples Cheat Book
来源：http://uer.52xcode.cn

================================================================================
来源：http://ttz.ydzc1.top

【收录内容】
来源：http://epi.0kj1m.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jqa.fanxiaobao.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zgg.316326.xyz

SQL · Bash · C · C++
来源：http://eek.kuanghao11.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://opf.aibaodan.cn

【使用说明】
来源：http://xhv.xylfe.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kol.epnwcf.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bnd.yueranfly.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qpd.hnxiangtu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ukw.fanxiaobao.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://wbe.jlsjyb.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jdn.fengsongda.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://eqx.jlsjyb.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sko.zdbjq.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tbt.svipenyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ihm.birdmap.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lme.0kj1m.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jgw.yuanzhike.top

【文件统计】
来源：http://qzs.epnwcf.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fbj.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://tvg.zhongyouzk.top

目  录
来源：http://bkd.vehdjk.com

--------------------------------------------------------------------------------
来源：http://dzz.gzhubu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://urd.0kj1m.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xas.tianlin.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rra.daxiang520.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://luu.aibaodan.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mvw.ehwqpu.com


<!-- 参考信息 -->