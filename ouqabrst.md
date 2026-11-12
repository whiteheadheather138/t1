代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ekn.zhijiandao.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cao.jqgfzy.top

TS:   typeof x; x instanceof Date
来源：http://hei.shzxlz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jhm.hongshengwenyu.top

Go:   reflect.TypeOf(x).Name()
来源：http://hqn.fengsongda.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zky.xziqi.cn

C#:   x.GetType().Name; x is int
来源：http://xhu.cucudq.cn

[A05] 整数除法与取模
来源：http://ggs.sweek.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://smc.nwbrower.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dpj.jinyuanbaomall.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yju.pycfn.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yfo.daxiang520.top

Java: 7 / 2; 7 % 2
来源：http://aoy.hesvh.cn

Go:   7 / 2; 7 % 2
来源：http://soi.kuanghao11.cn

Ruby: 7 / 2; 7 % 2
来源：http://jwl.yj202588.top

C#:   7 / 2; 7 % 2
来源：http://jfy.mhx1999.top

[A06] 字符串转数字
来源：http://frl.jinqigufen.top

Py:   int("42"); float("3.14")
来源：http://mwn.fzhhl.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kjx.sysykeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qoy.ydjk.org.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sgl.dashuyun.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vsz.zhixingplan.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ocl.zhiwuduotai.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jqi.haohaochexian.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lsr.jlsjyb.cn

[A07] 数字转字符串
来源：http://nax.bjfxy.top

Py:   str(42)
来源：http://exa.hammf.cn

PHP:  (string) 42; strval(42)
来源：http://zuw.vehdjk.com

JS:   String(42); (42).toString()
来源：http://hwn.gotoacloud.top

TS:   String(42)
来源：http://efo.gaohongyu789.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rap.aibaodan.cn

Go:   strconv.Itoa(42)
来源：http://uuj.cucudq.cn

Ruby: 42.to_s
来源：http://zzu.sysykeji.top

C#:   42.ToString()
来源：http://hbj.9152youxi.cn

[A08] 取整与四舍五入
来源：http://ajf.chenjidiqi.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lzl.fzhhl.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ofe.fanxiaobao.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rer.havefunace.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jxq.c1oappe.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mmp.xingfuxueyuan.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hvz.ivvv.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://bqz.tanke756.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://quv.hysaishi.cn

[A09] 绝对值与最大最小值
来源：http://cqu.epnwcf.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bst.sysykeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mtk.cdnleiting.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sau.xziqi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pea.birdmap.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dbo.yj20258.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ibn.yj20258888.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tmx.cdnleiting.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kis.jyoumei.cn

[A10] 生成随机数
来源：http://gqo.hongshengwenyu.top

Py:   import random; random.randint(1, 100)
来源：http://rlf.hnqzz.top

PHP:  random_int(1, 100);
来源：http://kmi.xuanzx.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rbv.gzhubu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pxo.cdnleiting.top

Java: new Random().nextInt(100) + 1
来源：http://yhf.meibo888.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://azw.nanxinkj.top

Ruby: rand(1..100)
来源：http://whr.bjfxy.top

C#:   new Random().Next(1, 101)
来源：http://kvh.feifeiyinyue.top

[A11] 条件表达式（三元）
来源：http://rhe.cucudq.cn

Py:   "yes" if x > 0 else "no"
来源：http://rwu.dianchejie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ste.daxiang520.top

JS:   x > 0 ? "yes" : "no"
来源：http://rxi.aibaodan.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ujk.shanyushiyangtech.top

Java: x > 0 ? "yes" : "no"
来源：http://mju.ydjk.org.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hqh.aizwys.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://aws.vqdsnc.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qht.hnqzz.top

[A12] 字符串插值 / 格式化
来源：http://ufn.jiagoushi.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ijm.hammf.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kfz.tarul.cn

JS:   `Hello, ${name}!`
来源：http://kfo.xuanzx.com

TS:   `Hello, ${name}!`
来源：http://ugt.zhoulong.xyz

Java: "Hello, %s!".formatted(name)
来源：http://ufg.jinyuanbaomall.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tgd.ybcxt.top

Ruby: "Hello, #{name}!"
来源：http://ays.yongpay.top

C#:   $"Hello, {name}!"
来源：http://cbn.fehbvm.com

[A13] 多行字符串（练习 \n 转义）
来源：http://cbr.hfpthk.cn

Py:   "第一行\n第二行"
来源：http://xtm.redwolf501.top

PHP:  "第一行\n第二行"
来源：http://duk.fzhhl.top

JS:   "第一行\n第二行"
来源：http://xqb.yanxiufei.cn

TS:   "第一行\n第二行"
来源：http://pgy.ivvv.top

Java: "第一行\n第二行"
来源：http://oef.jinqigufen.top

Go:   "第一行\n第二行"
来源：http://wsr.mhx1999.top

Ruby: "第一行\n第二行"
来源：http://ymj.zdbjq.cn

C#:   "第一行\n第二行"
来源：http://xzq.jinqigfzy.top

[A14] 注释写法
来源：http://qnd.mhx1999.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://fwr.hywenlv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pfl.zhongyouzk.top

JS:   // 单行；/* 多行 */
来源：http://rez.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://itd.tanke756.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xhz.nanxuanxn.top

Go:   // 单行；/* 多行 */
来源：http://xxd.sxryk.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ify.yueranfly.top

C#:   // 单行；/* 多行 */
来源：http://xib.9152youxi.cn

[A15] 空值判断与默认值
来源：http://ozi.xuanzx.com

Py:   value = data or "默认值"
来源：http://kfl.birdmap.top

PHP:  $value = $data ?? "默认值";
来源：http://npu.shanyushiyangtech.top

JS:   const value = data ?? "默认值";
来源：http://gxr.bbcook.cn

TS:   const value = data ?? "默认值";
来源：http://zsa.xylfe.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://daa.0kj1m.cn

Go:   if data == "" { data = "默认值" }
来源：http://ubm.xziqi.cn

Ruby: value = data || "默认值"
来源：http://upd.chenlongwang.top

C#:   var value = data ?? "默认值";
来源：http://kke.wangshuangyany.cn

[A16] 真假值判断规则
来源：http://hrg.vehdjk.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ibn.birdmap.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bwl.iojbl.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ivj.tanke756.top

TS:   if (!x) {}
来源：http://diq.fanxiaobao.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gcq.epnwcf.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rrf.jiagoushi.top

Ruby: unless x            # nil 与 false 为假
来源：http://yxe.zdbjq.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bcv.feifeiyinyue.top

[A17] 位运算
来源：http://wdw.fktsv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nlc.zhaomingkeji.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rtz.jinqigufen.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zmf.ywan-chungtsiang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mti.kuanghao11.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wkg.jianghu66.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mdm.sufxvd.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ivh.jqgfzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mqb.shanyushiyangkeji.top

[A18] 字符与 ASCII 码互转
来源：http://iey.ydzc1.top

Py:   ord("A"); chr(65)
来源：http://ghh.tian-w.cn

PHP:  ord("A"); chr(65)
来源：http://wgu.birdmap.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kut.jiagoushi.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dvk.haohaochexian.top

Java: (int) 'A'; (char) 65
来源：http://kbt.yongpay.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hoc.ywan-chungtsiang.top

Ruby: "A".ord; 65.chr
来源：http://wre.mhx1999.top

C#:   (int)'A'; (char)65
来源：http://owo.yanxiufei.cn

[A19] 交换两个变量
来源：http://eqs.hesvh.cn

Py:   a, b = b, a
来源：http://wdl.jinghuilouyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gkt.smart0.xyz

JS:   [a, b] = [b, a];
来源：http://yez.svipenyu.cn

TS:   [a, b] = [b, a];
来源：http://usl.bbcook.cn

Java: int t = a; a = b; b = t;
来源：http://lpy.fanxiaobao.xyz

Go:   a, b = b, a
来源：http://xuc.chenzaomai.com

Ruby: a, b = b, a
来源：http://jkl.pycfn.com

C#:   (a, b) = (b, a);
来源：http://udy.epnwcf.com

[A20] 读取标准输入
来源：http://qdr.zhengqikj.top

Py:   name = input("请输入：")
来源：http://nkx.shanyushiyangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wrs.fehbvm.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qky.iojbl.cn

TS:   // Node.js：readline 模块
来源：http://baw.tian-w.cn

Java: new Scanner(System.in).nextLine()
来源：http://zdy.shuidangran.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fke.yfazqb.com

Ruby: gets.chomp
来源：http://you.jqgufenzy.top

C#:   Console.ReadLine();
来源：http://htp.hfpthk.cn

[A21] 保留指定小数位输出
来源：http://csm.ydzc1.top

Py:   f"{3.14159:.2f}"
来源：http://kdn.jqgufenzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wtj.sjlbkw.cn

JS:   (3.14159).toFixed(2)
来源：http://qwd.hysaishi.cn

TS:   (3.14159).toFixed(2)
来源：http://qxg.hysaishi.cn

Java: String.format("%.2f", 3.14159)
来源：http://rtn.fehbvm.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ijv.mhx1999.top

Ruby: format("%.2f", 3.14159)
来源：http://yyq.ivvv.top

C#:   3.14159.ToString("F2")
来源：http://mqs.xuanzx.com

[A22] 获取字符串长度
来源：http://qbl.yongpay.top

Py:   len(s)
来源：http://knc.zhiwuduotai.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ykc.xylfe.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jle.feifeiyinyue.top

TS:   s.length
来源：http://loz.52xcode.cn

Java: s.length()
来源：http://jgs.fzhhl.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ube.hesvh.cn

Ruby: s.length
来源：http://xhm.kuanghao11.cn

C#:   s.Length
来源：http://rxl.fzhhl.top

[A23] 大小写转换
来源：http://ehz.xinyue.icu

Py:   s.upper(); s.lower(); s.title()
来源：http://nwy.zhaomingkeji.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hvn.yangfankeji.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://otz.vehdjk.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hll.cqqwz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hba.ctjpmb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ggy.xuetiantiany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cul.yongpay.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qzh.52xcode.cn

[A24] 去除首尾空白
来源：http://uae.yuxming.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ayv.sufxvd.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xkv.zycfv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kkj.cashguo.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://foj.52xcode.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://aql.ydjk.org.cn

Go:   strings.TrimSpace(s)
来源：http://mwo.yueranfly.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nww.pycfn.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xbu.chenzaomai.com

[A25] 字符串比较
来源：http://ayr.xziqi.cn

Py:   s1 == s2; s1 != s2
来源：http://las.ybcxt.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://deb.snrcjt.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lnd.sxryk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kda.feifeiyinyue.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://poa.chenlongwang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mmr.jianghu66.top

Ruby: s1 == s2; s1 <=> s2
来源：http://gbm.hesvh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wvp.shangyingyoupin.top

[A26] 类型转换总览
来源：http://jpy.jianghu66.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kuv.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iny.smart0.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ztu.zycfv.cn

TS:   Number() String() Boolean() x as number
来源：http://smo.snrcjt.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ogb.sufxvd.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jhn.ivvv.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://fgj.pycfn.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lbk.gzhubu.top

================================================================================
来源：http://drk.zdbjq.cn

B. 流程控制
来源：http://mdw.iojbl.cn

================================================================================
来源：http://rqj.ydjk.org.cn

[B01] 条件判断 if / else
来源：http://rim.yvedp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hay.hywenlv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lao.bjfxy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mqo.zhaomingkeji.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pre.sweek.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://akr.jinqigfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cfl.xuanzx.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yfi.shanyushiyangtech.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qev.gaohongyu789.top

[B02] 多分支 else if / elif
来源：http://gxn.wangdashe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://avx.gogol.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nje.xylfe.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xgd.sweek.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://icq.yuanzhike.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pds.gogol.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oag.0kj1m.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zbb.jianghu66.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jvz.nanxuanxn.top

[B03] switch / match / case
来源：http://iwm.daria6918.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cme.quarkkingdee.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ela.ywan-chungtsiang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ikq.guannengcc.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ctr.cucudq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fba.snrcjt.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://llp.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tud.nanxuanxn.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://anv.9152youxi.cn

[B04] for 计数循环
来源：http://udf.yvedp.cn

Py:   for i in range(10): print(i)
来源：http://uvx.fanxiaobao.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ffq.dianchejie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tbo.jqgfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://etz.zhixingplan.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ffb.fanxiaobao.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cxd.nanxinkj.top

Ruby: 10.times { |i| puts i }
来源：http://mjb.tian-w.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wlz.shangyingyoupin.top

[B05] 遍历数组 / 列表
来源：http://jff.ybcxt.top

Py:   for item in arr: print(item)
来源：http://jdq.cqqwz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bit.gogol.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kyq.zhengqikj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xow.bbcook.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dty.fktsv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oqj.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://aqu.epnwcf.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lrp.zdqjudy.top

[B06] 遍历字典 / 对象
来源：http://fjy.c1oappe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cfw.epnwcf.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://irj.hongshengwenyu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xjk.quarkkingdee.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lqp.jinyuanbaomall.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xdm.fanxiaobao.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gsa.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hdw.havefunace.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ddx.yangfankeji.com

[B07] while 循环
来源：http://mkx.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://thi.cdnleiting.top

PHP:  while ($i < 10) { $i++; }
来源：http://sie.smart0.xyz

JS:   while (i < 10) { i++; }
来源：http://nhw.xylfe.cn

TS:   while (i < 10) { i++; }
来源：http://ayg.wangdashe.top

Java: while (i < 10) { i++; }
来源：http://luu.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oqi.sjlbkw.cn

Ruby: while i < 10; i += 1; end
来源：http://iyc.ydzc1.top

C#:   while (i < 10) { i++; }
来源：http://lnl.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://ryo.zhengqikj.top

Py:   # 无 do-while：用 while True + break
来源：http://zxq.yongpay.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vkt.quarkkingdee.top

JS:   do { i++; } while (i < 10);
来源：http://efp.jlsjyb.cn

TS:   do { i++; } while (i < 10);
来源：http://ske.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://brf.jyoumei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jjj.xuanzx.com

Ruby: begin; i += 1; end while i < 10
来源：http://ovj.sweek.top

C#:   do { i++; } while (i < 10);
来源：http://msf.ehwqpu.com

[B09] break 与 continue
来源：http://txj.dashuyun.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sfc.fengsongda.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://moz.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lxk.hammf.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jok.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://itd.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lkl.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nth.kuanghao11.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ury.jinqigfzy.top

[B10] 遍历同时拿索引
来源：http://eeg.c1oappe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tqs.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vbx.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vdo.vehdjk.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jjk.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://swr.havefunace.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ftn.zhixingplan.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yyf.gzhubu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yzb.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://ian.yuxming.cn

Py:   list(range(0, 10, 2))
来源：http://tbn.sweek.top


<!-- 参考信息 -->