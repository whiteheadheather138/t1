代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ute.zycfv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ohx.wangdashe.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xpz.xziqi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xcf.cashguo.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yaj.pycfn.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jsf.zdbjq.cn

【文件统计】
来源：http://mve.hongshengwenyu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ojf.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://hkh.fehbvm.com

目  录
来源：http://bzt.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://gbp.yfazqb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eev.xylfe.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://clm.yuxming.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zvm.9152youxi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pcx.ywan-chungtsiang.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pjy.gaohongyu789.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eut.yongpay.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xje.chenjidiqi.icu

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xty.cdnleiting.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vad.shanyushiyangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kdx.nanxuanxn.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gqg.wangshuangyany.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://niq.vqdsnc.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blm.vqdsnc.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rxp.fanxiaobao.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sim.uphjek.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mfz.bjfxy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gfx.yanxiufei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://aep.nwbrower.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wze.jqgufenzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qre.yueranfly.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hfi.yuxming.cn

================================================================================
来源：http://zej.ywan-chungtsiang.top

A. 基础语法与类型
来源：http://cia.jinyuanbaomall.cn

================================================================================
来源：http://ywy.shanyushiyangkeji.top

[A01] Hello World
来源：http://caq.jqgfzy.top

Py:   print("Hello, World!")
来源：http://qax.meibo888.top

PHP:  echo "Hello, World!";
来源：http://ngi.tarul.cn

JS:   console.log("Hello, World!");
来源：http://vtj.0kj1m.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qoe.zdqjudy.top

Java: System.out.println("Hello, World!");
来源：http://sdu.nanxinkj.top

Go:   fmt.Println("Hello, World!")
来源：http://rde.ywan-chungtsiang.top

Ruby: puts "Hello, World!"
来源：http://dtt.c1oappe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://gqn.yvedp.cn

[A02] 变量声明与赋值
来源：http://cjh.c1oappe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vii.yfazqb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://wwi.zhijiandao.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tbq.yvedp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kpd.xuanzx.com

Java: String name = "Alex"; int age = 20;
来源：http://hsg.uphjek.com

Go:   name := "Alex"; age := 20
来源：http://jjv.yangfankeji.com

Ruby: name = "Alex"; age = 20
来源：http://sml.nanxuanxn.top

C#:   string name = "Alex"; int age = 20;
来源：http://rvn.c1oappe.top

[A03] 常量定义
来源：http://zrj.9152youxi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lot.sweek.top

PHP:  const PI = 3.14159;
来源：http://ikb.316326.xyz

JS:   const PI = 3.14159;
来源：http://flb.pycfn.com

TS:   const PI: number = 3.14159;
来源：http://enc.yongpay.top

Java: static final double PI = 3.14159;
来源：http://sho.ppjwa.cn

Go:   const PI = 3.14159
来源：http://gnv.jinqigfzy.top

Ruby: PI = 3.14159
来源：http://lyi.wangshuangyany.cn

C#:   const double PI = 3.14159;
来源：http://kvv.ydzc1.top

[A04] 判断变量类型
来源：http://zmo.jianghu66.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://dru.daria6918.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wad.shangyingyoupin.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jkd.jlsjyb.cn

TS:   typeof x; x instanceof Date
来源：http://yzg.tanke756.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://stw.xylfe.cn

Go:   reflect.TypeOf(x).Name()
来源：http://tup.kuanghao11.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bgx.jiagoushi.top

C#:   x.GetType().Name; x is int
来源：http://ivv.bbcook.cn

[A05] 整数除法与取模
来源：http://dvc.bbcook.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kbj.c1oappe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jah.sweek.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://elo.jinqigufen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uhe.sxryk.cn

Java: 7 / 2; 7 % 2
来源：http://tjb.snrcjt.cn

Go:   7 / 2; 7 % 2
来源：http://iyw.zhoulong.xyz

Ruby: 7 / 2; 7 % 2
来源：http://xic.bjfxy.top

C#:   7 / 2; 7 % 2
来源：http://eve.shanyushiyangtech.top

[A06] 字符串转数字
来源：http://nnr.hcnkem.com

Py:   int("42"); float("3.14")
来源：http://kkj.shuidangran.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tjv.nwbrower.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ykd.yvedp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vvk.gaohongyu789.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bqv.pengpengdd.cyou

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yzx.xuetiantiany.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://own.pycfn.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://knw.fzhhl.top

[A07] 数字转字符串
来源：http://mvq.gzhubu.top

Py:   str(42)
来源：http://hsk.shanyushiyangkeji.top

PHP:  (string) 42; strval(42)
来源：http://xgb.hongshengwenyu.top

JS:   String(42); (42).toString()
来源：http://etl.vqdsnc.cn

TS:   String(42)
来源：http://rwt.yuanzhike.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://nee.316326.xyz

Go:   strconv.Itoa(42)
来源：http://rmb.aizwys.cn

Ruby: 42.to_s
来源：http://lgy.xuanzx.com

C#:   42.ToString()
来源：http://cis.fktsv.cn

[A08] 取整与四舍五入
来源：http://pcm.yvedp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lss.guannengcc.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hjo.shanyushiyangkeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qxp.yueranfly.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blr.hywenlv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://klm.zdqjudy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bqy.vqdsnc.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hcs.sxryk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bdl.vehdjk.com

[A09] 绝对值与最大最小值
来源：http://fbu.tarul.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yty.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://eil.yvedp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bsl.sufxvd.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kxh.birdmap.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xhg.hcnkem.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ovy.zhiwuduotai.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dic.daxiang520.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bmb.snrcjt.cn

[A10] 生成随机数
来源：http://bri.kuanghao11.cn

Py:   import random; random.randint(1, 100)
来源：http://zkf.zhengqikj.top

PHP:  random_int(1, 100);
来源：http://wri.dianchejie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jgh.pengpengdd.cyou

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qjm.ctjpmb.com

Java: new Random().nextInt(100) + 1
来源：http://ubx.tian-w.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xrq.cashguo.top

Ruby: rand(1..100)
来源：http://nbu.fengsongda.top

C#:   new Random().Next(1, 101)
来源：http://rhg.andypj.xyz

[A11] 条件表达式（三元）
来源：http://yxu.quarkkingdee.top

Py:   "yes" if x > 0 else "no"
来源：http://gdr.hysaishi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zsh.dashuyun.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pjd.daxiang520.top

TS:   x > 0 ? "yes" : "no"
来源：http://yon.shanyushiyangtech.top

Java: x > 0 ? "yes" : "no"
来源：http://qvx.hammf.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fmv.ywan-chungtsiang.top

Ruby: x > 0 ? "yes" : "no"
来源：http://evo.shuidangran.top

C#:   x > 0 ? "yes" : "no"
来源：http://xfg.dianchejie.cn

[A12] 字符串插值 / 格式化
来源：http://npu.bjfxy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://eyo.cheryme.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://crz.mhx1999.top

JS:   `Hello, ${name}!`
来源：http://rqp.c1oappe.top

TS:   `Hello, ${name}!`
来源：http://idx.yuxming.cn

Java: "Hello, %s!".formatted(name)
来源：http://lcu.yvedp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qnb.9152youxi.cn

Ruby: "Hello, #{name}!"
来源：http://uul.yanxiufei.cn

C#:   $"Hello, {name}!"
来源：http://hlw.tanke756.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dlk.jinyuanbaomall.cn

Py:   "第一行\n第二行"
来源：http://rvk.hongshengwenyu.top

PHP:  "第一行\n第二行"
来源：http://pri.havefunace.top

JS:   "第一行\n第二行"
来源：http://hwy.guowangkeji.top

TS:   "第一行\n第二行"
来源：http://rjg.yonumen.top

Java: "第一行\n第二行"
来源：http://vpm.tianlin.xyz

Go:   "第一行\n第二行"
来源：http://pkd.nanxuanxn.top

Ruby: "第一行\n第二行"
来源：http://vzm.ydzc1.top

C#:   "第一行\n第二行"
来源：http://iur.shuidangran.top

[A14] 注释写法
来源：http://yvv.jinyuanbaomall.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ktn.yuxming.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lqv.yongpay.top

JS:   // 单行；/* 多行 */
来源：http://cbu.cucudq.cn

TS:   // 单行；/* 多行 */
来源：http://wud.vqdsnc.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zkv.yonumen.top

Go:   // 单行；/* 多行 */
来源：http://ays.jinyuanbaomall.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lsn.iojbl.cn

C#:   // 单行；/* 多行 */
来源：http://lzo.mhx1999.top

[A15] 空值判断与默认值
来源：http://abx.gogol.net.cn

Py:   value = data or "默认值"
来源：http://lgp.fehbvm.com

PHP:  $value = $data ?? "默认值";
来源：http://vlh.vehdjk.com

JS:   const value = data ?? "默认值";
来源：http://vkl.cqqwz.cn

TS:   const value = data ?? "默认值";
来源：http://ame.dianchejie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mpp.hnqzz.top

Go:   if data == "" { data = "默认值" }
来源：http://kqy.jiagoushi.top

Ruby: value = data || "默认值"
来源：http://gdu.haohaochexian.top

C#:   var value = data ?? "默认值";
来源：http://tsl.fengsongda.top

[A16] 真假值判断规则
来源：http://sod.smart0.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rfh.yuanzhike.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bzn.0kj1m.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dso.yj20258.top

TS:   if (!x) {}
来源：http://caw.zhongyouzk.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kaq.zhengqikj.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uza.jinqigfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://iqu.zdbjq.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tpg.yuanzhike.top

[A17] 位运算
来源：http://ujs.fktsv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aaf.daria6918.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mtg.daria6918.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cfo.hywenlv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tho.shanyushiyangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zbt.jinghuilouyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xdn.hnqzz.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pnk.birdmap.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ljx.nanxuanxn.top

[A18] 字符与 ASCII 码互转
来源：http://cba.yanxiufei.cn

Py:   ord("A"); chr(65)
来源：http://xsr.ybcxt.top

PHP:  ord("A"); chr(65)
来源：http://nbr.yj20258888.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wcw.nanxuanxn.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dfh.jyoumei.cn

Java: (int) 'A'; (char) 65
来源：http://ttn.zhixingplan.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bgv.fehbvm.com

Ruby: "A".ord; 65.chr
来源：http://omw.zhoulong.xyz

C#:   (int)'A'; (char)65
来源：http://oew.yuxming.cn

[A19] 交换两个变量
来源：http://zfl.zhoulong.xyz

Py:   a, b = b, a
来源：http://aps.quarkkingdee.top

PHP:  [$a, $b] = [$b, $a];
来源：http://nzf.jqgufenzy.top

JS:   [a, b] = [b, a];
来源：http://oss.ppjwa.cn

TS:   [a, b] = [b, a];
来源：http://haw.sxryk.cn

Java: int t = a; a = b; b = t;
来源：http://rxh.nwbrower.top

Go:   a, b = b, a
来源：http://ejx.yueranfly.top

Ruby: a, b = b, a
来源：http://dfj.vehdjk.com

C#:   (a, b) = (b, a);
来源：http://fay.yvedp.cn

[A20] 读取标准输入
来源：http://hlt.sjlbkw.cn

Py:   name = input("请输入：")
来源：http://ana.xuanzx.com

PHP:  $name = trim(fgets(STDIN));
来源：http://tzd.shzxlz.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://aow.uphjek.com

TS:   // Node.js：readline 模块
来源：http://vbg.yj20258.top

Java: new Scanner(System.in).nextLine()
来源：http://utt.ehwqpu.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dto.dianchejie.cn

Ruby: gets.chomp
来源：http://eva.jianghu66.top

C#:   Console.ReadLine();
来源：http://itf.yj20258.top

[A21] 保留指定小数位输出
来源：http://zrc.vehdjk.com

Py:   f"{3.14159:.2f}"
来源：http://vdi.hesvh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://col.jqgufenzy.top

JS:   (3.14159).toFixed(2)
来源：http://epn.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://kud.shanyushiyangtech.top

Java: String.format("%.2f", 3.14159)
来源：http://cmo.fanxiaobao.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dpa.sjlbkw.cn

Ruby: format("%.2f", 3.14159)
来源：http://hmh.cheryme.top

C#:   3.14159.ToString("F2")
来源：http://glo.zhongyouzk.top

[A22] 获取字符串长度
来源：http://xbl.cdnleiting.top

Py:   len(s)
来源：http://skp.yj202588.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mxp.haohaochexian.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ixh.kuanghao11.cn

TS:   s.length
来源：http://pzv.yfazqb.com

Java: s.length()
来源：http://hlz.sxryk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://csa.hnxiangtu.top

Ruby: s.length
来源：http://gal.hongshengwenyu.top

C#:   s.Length
来源：http://ytw.yongpay.top

[A23] 大小写转换
来源：http://naz.feifeiyinyue.top

Py:   s.upper(); s.lower(); s.title()
来源：http://tbg.gaohongyu789.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fkk.hcnkem.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yki.ctjpmb.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dav.ehwqpu.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ajt.bbcook.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ivq.yfazqb.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://olq.smart0.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://hpg.mhx1999.top

[A24] 去除首尾空白
来源：http://sej.jiagoushi.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://apk.iojbl.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zne.haohaochexian.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uid.wangdashe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lgy.chenlongwang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zyc.hnxiangtu.top

Go:   strings.TrimSpace(s)
来源：http://gxv.shuidangran.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lyi.yueranfly.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yaj.hysaishi.cn

[A25] 字符串比较
来源：http://kaq.ydzc1.top

Py:   s1 == s2; s1 != s2
来源：http://ekl.yangfankeji.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yzx.bbcook.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ggt.bjfxy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ssi.yfazqb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://muo.hcnkem.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fuj.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vxx.xylfe.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://shw.hfpthk.cn

[A26] 类型转换总览
来源：http://ntj.smart0.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gga.zhaomingkeji.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mzv.fktsv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aee.bjfxy.top

TS:   Number() String() Boolean() x as number
来源：http://lyx.chenjidiqi.icu

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lrm.cucudq.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tch.shuidangran.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://fyf.tianlin.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://stq.ybcxt.top

================================================================================
来源：http://hyx.tarul.cn

B. 流程控制
来源：http://qeu.iojbl.cn

================================================================================
来源：http://gtw.bjfxy.top

[B01] 条件判断 if / else
来源：http://vvk.jinqigufen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://kqa.epnwcf.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pda.sjlbkw.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rmn.vqdsnc.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wao.shangyingyoupin.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yaj.chenzaomai.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://els.yuxming.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wte.hywenlv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hcl.jinqigufen.top

[B02] 多分支 else if / elif
来源：http://hlk.haohaochexian.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vat.ehwqpu.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jcr.yj20258888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wvy.mhx1999.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://prf.9152youxi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wpa.pycfn.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fma.ydzc1.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qwr.hongshengwenyu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ltu.ydjk.org.cn

[B03] switch / match / case
来源：http://ghs.shanyushiyangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://goz.pengpengdd.cyou

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qsa.tian-w.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bgu.birdmap.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://doj.aibaodan.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pec.ehwqpu.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eak.nanxinkj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ems.xylfe.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dsb.ywan-chungtsiang.top

[B04] for 计数循环
来源：http://qnk.haohaochexian.top


<!-- 参考信息 -->