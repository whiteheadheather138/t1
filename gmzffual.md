代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://xrg.iojbl.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tvf.havefunace.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cdg.hnxiangtu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kzu.nanxuanxn.top

================================================================================
来源：http://rrf.bbcook.cn

A. 基础语法与类型
来源：http://fqf.zhaomingkeji.xyz

================================================================================
来源：http://bhr.tianlin.xyz

[A01] Hello World
来源：http://xcv.guannengcc.top

Py:   print("Hello, World!")
来源：http://qdy.wangshuangyany.cn

PHP:  echo "Hello, World!";
来源：http://ifx.wangshuangyany.cn

JS:   console.log("Hello, World!");
来源：http://fmo.meibo888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tqy.fzhhl.top

Java: System.out.println("Hello, World!");
来源：http://lhe.iojbl.cn

Go:   fmt.Println("Hello, World!")
来源：http://dtc.dianchejie.cn

Ruby: puts "Hello, World!"
来源：http://syn.tanke756.top

C#:   Console.WriteLine("Hello, World!");
来源：http://tmx.zhijiandao.cn

[A02] 变量声明与赋值
来源：http://wut.cashguo.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gdq.haohaochexian.top

PHP:  $name = "Alex"; $age = 20;
来源：http://qox.uphjek.com

JS:   let name = "Alex"; const age = 20;
来源：http://svy.chenlongwang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oyl.hnqzz.top

Java: String name = "Alex"; int age = 20;
来源：http://heu.ydzc1.top

Go:   name := "Alex"; age := 20
来源：http://prd.tian-w.cn

Ruby: name = "Alex"; age = 20
来源：http://fwn.cqqwz.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cao.gogol.net.cn

[A03] 常量定义
来源：http://xvj.daria6918.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://snq.sysykeji.top

PHP:  const PI = 3.14159;
来源：http://ddw.zhijiandao.cn

JS:   const PI = 3.14159;
来源：http://wur.yj20258.top

TS:   const PI: number = 3.14159;
来源：http://sib.zycfv.cn

Java: static final double PI = 3.14159;
来源：http://wal.sysykeji.top

Go:   const PI = 3.14159
来源：http://czg.kuanghao11.cn

Ruby: PI = 3.14159
来源：http://vrh.wangshuangyany.cn

C#:   const double PI = 3.14159;
来源：http://kir.vqdsnc.cn

[A04] 判断变量类型
来源：http://tbg.cqqwz.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://suk.vqdsnc.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://myr.hnqzz.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qkl.fehbvm.com

TS:   typeof x; x instanceof Date
来源：http://bhf.jinqigufen.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ajr.aibaodan.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ydw.meibo888.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xve.zhengqikj.top

C#:   x.GetType().Name; x is int
来源：http://cxr.cqqwz.cn

[A05] 整数除法与取模
来源：http://enq.hammf.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pju.sysykeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://phf.316326.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pav.zdqjudy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cnw.ydzc1.top

Java: 7 / 2; 7 % 2
来源：http://gbo.cheryme.top

Go:   7 / 2; 7 % 2
来源：http://khe.bjfxy.top

Ruby: 7 / 2; 7 % 2
来源：http://hwq.ctjpmb.com

C#:   7 / 2; 7 % 2
来源：http://vxl.sysykeji.top

[A06] 字符串转数字
来源：http://tug.cdnleiting.top

Py:   int("42"); float("3.14")
来源：http://obe.cashguo.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gxf.ydjk.org.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yzy.jqgfzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://hqa.jinqigufen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fes.hongshengwenyu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://utx.xylfe.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wfo.9152youxi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gie.quarkkingdee.top

[A07] 数字转字符串
来源：http://fci.haohaochexian.top

Py:   str(42)
来源：http://lhu.shangyingyoupin.top

PHP:  (string) 42; strval(42)
来源：http://oro.quarkkingdee.top

JS:   String(42); (42).toString()
来源：http://cvy.chenzaomai.com

TS:   String(42)
来源：http://ynj.mhx1999.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wfi.yueranfly.top

Go:   strconv.Itoa(42)
来源：http://tpm.fehbvm.com

Ruby: 42.to_s
来源：http://blv.bbcook.cn

C#:   42.ToString()
来源：http://lse.feifeiyinyue.top

[A08] 取整与四舍五入
来源：http://drx.wangdashe.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fqx.quarkkingdee.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mkf.iojbl.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wbf.zhixingplan.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gop.fanxiaobao.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pjb.yuanzhike.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rrh.hysaishi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lyr.hesvh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wce.daxiang520.top

[A09] 绝对值与最大最小值
来源：http://uiu.shangyingyoupin.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bar.dashuyun.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ryt.jinqigfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vpr.jinqigufen.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hkn.mhx1999.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://brm.sufxvd.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gni.yangfankeji.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cek.ydzc1.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ovy.yj202588.top

[A10] 生成随机数
来源：http://qih.jqgufenzy.top

Py:   import random; random.randint(1, 100)
来源：http://qbj.nanxinkj.top

PHP:  random_int(1, 100);
来源：http://awo.gzhubu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ujk.havefunace.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fxh.ppjwa.cn

Java: new Random().nextInt(100) + 1
来源：http://ffj.xziqi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dgo.316326.xyz

Ruby: rand(1..100)
来源：http://fvg.vqdsnc.cn

C#:   new Random().Next(1, 101)
来源：http://ykw.xylfe.cn

[A11] 条件表达式（三元）
来源：http://skn.vehdjk.com

Py:   "yes" if x > 0 else "no"
来源：http://enb.svipenyu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ruw.pengpengdd.cyou

JS:   x > 0 ? "yes" : "no"
来源：http://qgo.yuanzhike.top

TS:   x > 0 ? "yes" : "no"
来源：http://zsa.zhengqikj.top

Java: x > 0 ? "yes" : "no"
来源：http://lar.zhaomingkeji.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://ypi.ydjk.org.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qny.yvedp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lpp.zdbjq.cn

[A12] 字符串插值 / 格式化
来源：http://sct.gaohongyu789.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://usp.ydzc1.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ewp.jiagoushi.top

JS:   `Hello, ${name}!`
来源：http://guk.quarkkingdee.top

TS:   `Hello, ${name}!`
来源：http://sit.ywan-chungtsiang.top

Java: "Hello, %s!".formatted(name)
来源：http://rif.fehbvm.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gwx.uphjek.com

Ruby: "Hello, #{name}!"
来源：http://zls.vehdjk.com

C#:   $"Hello, {name}!"
来源：http://pyz.jiagoushi.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qfo.aibaodan.cn

Py:   "第一行\n第二行"
来源：http://agn.cashguo.top

PHP:  "第一行\n第二行"
来源：http://nfq.cqqwz.cn

JS:   "第一行\n第二行"
来源：http://swh.fktsv.cn

TS:   "第一行\n第二行"
来源：http://oac.hysaishi.cn

Java: "第一行\n第二行"
来源：http://lrw.ppjwa.cn

Go:   "第一行\n第二行"
来源：http://enz.gogol.net.cn

Ruby: "第一行\n第二行"
来源：http://cyt.chenjidiqi.icu

C#:   "第一行\n第二行"
来源：http://hhp.fehbvm.com

[A14] 注释写法
来源：http://fma.yj20258.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rln.vehdjk.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://adn.yueranfly.top

JS:   // 单行；/* 多行 */
来源：http://qoi.jlsjyb.cn

TS:   // 单行；/* 多行 */
来源：http://dmj.tian-w.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bpy.zhengqikj.top

Go:   // 单行；/* 多行 */
来源：http://skd.iojbl.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jwt.sysykeji.top

C#:   // 单行；/* 多行 */
来源：http://sqd.fzhhl.top

[A15] 空值判断与默认值
来源：http://omo.sysykeji.top

Py:   value = data or "默认值"
来源：http://asa.yfazqb.com

PHP:  $value = $data ?? "默认值";
来源：http://mce.wangshuangyany.cn

JS:   const value = data ?? "默认值";
来源：http://kmt.svipenyu.cn

TS:   const value = data ?? "默认值";
来源：http://nav.wangdashe.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zng.jinghuilouyu.cn

Go:   if data == "" { data = "默认值" }
来源：http://njy.cqqwz.cn

Ruby: value = data || "默认值"
来源：http://vte.chenlongwang.top

C#:   var value = data ?? "默认值";
来源：http://etc.meibo888.top

[A16] 真假值判断规则
来源：http://lfd.dianchejie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lrn.tianlin.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zsj.chenzaomai.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cbh.ehwqpu.com

TS:   if (!x) {}
来源：http://kzt.zhoulong.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yfi.nanxuanxn.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ucq.shuidangran.top

Ruby: unless x            # nil 与 false 为假
来源：http://aev.chenzaomai.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ngf.cqqwz.cn

[A17] 位运算
来源：http://ohb.fktsv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xiw.yvedp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ybr.tian-w.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xuy.meibo888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mrb.jiagoushi.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pbz.wangdashe.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bqh.fanxiaobao.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qiu.zhiwuduotai.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aur.meibo888.top

[A18] 字符与 ASCII 码互转
来源：http://trq.gzhubu.top

Py:   ord("A"); chr(65)
来源：http://acl.hfpthk.cn

PHP:  ord("A"); chr(65)
来源：http://smt.guowangkeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rzi.shanyushiyangkeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://taj.fehbvm.com

Java: (int) 'A'; (char) 65
来源：http://wqu.quarkkingdee.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://irn.yongpay.top

Ruby: "A".ord; 65.chr
来源：http://hql.aizwys.cn

C#:   (int)'A'; (char)65
来源：http://jyk.chenlongwang.top

[A19] 交换两个变量
来源：http://yzf.jinqigufen.top

Py:   a, b = b, a
来源：http://icd.jyoumei.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ppe.jyoumei.cn

JS:   [a, b] = [b, a];
来源：http://agx.jinghuilouyu.cn

TS:   [a, b] = [b, a];
来源：http://mri.cheryme.top

Java: int t = a; a = b; b = t;
来源：http://sbh.ywan-chungtsiang.top

Go:   a, b = b, a
来源：http://nwr.ywan-chungtsiang.top

Ruby: a, b = b, a
来源：http://gha.zhixingplan.top

C#:   (a, b) = (b, a);
来源：http://iak.daxiang520.top

[A20] 读取标准输入
来源：http://wwc.chenzaomai.com

Py:   name = input("请输入：")
来源：http://ugn.jinghuilouyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qxy.9152youxi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ilu.gotoacloud.top

TS:   // Node.js：readline 模块
来源：http://qow.pycfn.com

Java: new Scanner(System.in).nextLine()
来源：http://kwd.daxiang520.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dzj.zhongyouzk.top

Ruby: gets.chomp
来源：http://psz.aibaodan.cn

C#:   Console.ReadLine();
来源：http://fhu.hnxiangtu.top

[A21] 保留指定小数位输出
来源：http://fxl.bbcook.cn

Py:   f"{3.14159:.2f}"
来源：http://fwm.zhaomingkeji.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oiy.bjfxy.top

JS:   (3.14159).toFixed(2)
来源：http://eme.shangyingyoupin.top

TS:   (3.14159).toFixed(2)
来源：http://vsg.hcnkem.com

Java: String.format("%.2f", 3.14159)
来源：http://wth.xuanzx.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eie.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://otx.zhoulong.xyz

C#:   3.14159.ToString("F2")
来源：http://rha.yj20258.top

[A22] 获取字符串长度
来源：http://nja.wangdashe.top

Py:   len(s)
来源：http://vbz.hnxiangtu.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tbn.yj20258888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zoc.shanyushiyangtech.top

TS:   s.length
来源：http://vie.sysykeji.top

Java: s.length()
来源：http://yww.bbcook.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gqw.yongpay.top

Ruby: s.length
来源：http://jvp.jinghuilouyu.cn

C#:   s.Length
来源：http://hsz.zhijiandao.cn

[A23] 大小写转换
来源：http://hqs.jqgfzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nix.zhijiandao.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wuk.tianlin.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rnk.dianchejie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://njt.yuxming.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wmk.ydjk.org.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xnz.fzhhl.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yzv.andypj.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://jyl.yongpay.top

[A24] 去除首尾空白
来源：http://pqp.sjlbkw.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tev.ywan-chungtsiang.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rfy.hywenlv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://key.yj20258888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dxn.zdbjq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rsy.cucudq.cn

Go:   strings.TrimSpace(s)
来源：http://vgv.shangyingyoupin.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ein.jqgufenzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ouy.birdmap.top

[A25] 字符串比较
来源：http://lby.xziqi.cn

Py:   s1 == s2; s1 != s2
来源：http://ygb.hysaishi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hgr.xingfuxueyuan.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sob.zhaomingkeji.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zgy.pycfn.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://els.jinqigfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jyi.hammf.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://opm.zhongyouzk.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ynz.bjfxy.top

[A26] 类型转换总览
来源：http://pyo.jinqigufen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vdg.cdnleiting.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lus.xuetiantiany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://urk.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://svq.yongpay.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zhz.hcnkem.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bej.feifeiyinyue.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qjy.shanyushiyangkeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hrb.hesvh.cn

================================================================================
来源：http://afr.shangyingyoupin.top

B. 流程控制
来源：http://xhv.kuanghao11.cn

================================================================================
来源：http://ssu.zhijiandao.cn

[B01] 条件判断 if / else
来源：http://mcj.andypj.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://cvp.nwbrower.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hyq.cqqwz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lge.hesvh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qgr.hesvh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mru.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jrb.kuanghao11.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gov.zhixingplan.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cuj.daxiang520.top

[B02] 多分支 else if / elif
来源：http://rma.dianchejie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://euo.jianghu66.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fyi.nanxinkj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cvm.ppjwa.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ufy.sjlbkw.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dnh.fengsongda.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ayg.fengsongda.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tsr.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uzz.ydzc1.top

[B03] switch / match / case
来源：http://hcp.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://anp.zhoulong.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vfl.xuetiantiany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yne.xuanzx.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zkx.iojbl.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nco.guannengcc.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vsz.cqqwz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bwy.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jcy.cdnleiting.top

[B04] for 计数循环
来源：http://rzc.sweek.top

Py:   for i in range(10): print(i)
来源：http://iwn.yfazqb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://txp.shzxlz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rne.feifeiyinyue.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wew.zhengqikj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://myv.cqqwz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xrv.pengpengdd.cyou

Ruby: 10.times { |i| puts i }
来源：http://nyi.nwbrower.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://whi.vqdsnc.cn

[B05] 遍历数组 / 列表
来源：http://urz.hongshengwenyu.top

Py:   for item in arr: print(item)
来源：http://ikq.sweek.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xxh.aibaodan.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mdm.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nfp.jinqigufen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uif.havefunace.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nvp.jiagoushi.top

Ruby: arr.each { |item| puts item }
来源：http://igd.tianlin.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xoi.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://reu.jiagoushi.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nci.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oiq.pycfn.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rhp.sysykeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ocm.quarkkingdee.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ilp.shanyushiyangtech.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mte.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jej.fktsv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://efb.xuanzx.com

[B07] while 循环
来源：http://aop.uphjek.com

Py:   while i < 10: i += 1
来源：http://dlm.gotoacloud.top


<!-- 参考信息 -->