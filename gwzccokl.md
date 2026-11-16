代发 wailian999

[A06] 字符串转数字
来源：http://esd.aizwys.cn

Py:   int("42"); float("3.14")
来源：http://hca.nwbrower.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jbt.daria6918.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jpz.aibaodan.cn

TS:   parseInt("42", 10); Number("42")
来源：http://srn.vehdjk.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pxy.cdnleiting.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uvu.kuanghao11.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ghh.cucudq.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xyn.jqgfzy.top

[A07] 数字转字符串
来源：http://dlc.daria6918.cn

Py:   str(42)
来源：http://ssd.snrcjt.cn

PHP:  (string) 42; strval(42)
来源：http://ofa.sweek.top

JS:   String(42); (42).toString()
来源：http://huq.yanxiufei.cn

TS:   String(42)
来源：http://eeb.tanke756.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://bae.zdqjudy.top

Go:   strconv.Itoa(42)
来源：http://sak.redwolf501.top

Ruby: 42.to_s
来源：http://yez.kuanghao11.cn

C#:   42.ToString()
来源：http://avl.cdnleiting.top

[A08] 取整与四舍五入
来源：http://nfa.yongpay.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://erh.yvedp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jkv.bjfxy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lql.cashguo.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ydn.jiagoushi.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iol.feifeiyinyue.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dfg.0kj1m.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://czb.yonumen.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://omu.kuanghao11.cn

[A09] 绝对值与最大最小值
来源：http://swe.jinghuilouyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zfv.jinghuilouyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vki.tanke756.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://eis.meibo888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dsn.yj202588.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lkl.xylfe.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ncu.feifeiyinyue.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ylx.jqgufenzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fmq.cqqwz.cn

[A10] 生成随机数
来源：http://seh.daxiang520.top

Py:   import random; random.randint(1, 100)
来源：http://rrz.fehbvm.com

PHP:  random_int(1, 100);
来源：http://hwv.sysykeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qqu.tianlin.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dke.snrcjt.cn

Java: new Random().nextInt(100) + 1
来源：http://zjg.haohaochexian.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xtj.iojbl.cn

Ruby: rand(1..100)
来源：http://shh.feifeiyinyue.top

C#:   new Random().Next(1, 101)
来源：http://fcr.shanyushiyangtech.top

[A11] 条件表达式（三元）
来源：http://dtt.zhaomingkeji.xyz

Py:   "yes" if x > 0 else "no"
来源：http://map.pengpengdd.cyou

PHP:  $x > 0 ? "yes" : "no"
来源：http://czz.shuidangran.top

JS:   x > 0 ? "yes" : "no"
来源：http://gpt.hnqzz.top

TS:   x > 0 ? "yes" : "no"
来源：http://avx.svipenyu.cn

Java: x > 0 ? "yes" : "no"
来源：http://kob.snrcjt.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cfq.yj20258.top

Ruby: x > 0 ? "yes" : "no"
来源：http://cdd.yanxiufei.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kgg.chenjidiqi.icu

[A12] 字符串插值 / 格式化
来源：http://rsk.hnxiangtu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yhs.chenjidiqi.icu

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://map.uphjek.com

JS:   `Hello, ${name}!`
来源：http://qhr.zdbjq.cn

TS:   `Hello, ${name}!`
来源：http://ddy.yj20258888.top

Java: "Hello, %s!".formatted(name)
来源：http://eho.smart0.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oje.jqgufenzy.top

Ruby: "Hello, #{name}!"
来源：http://tpz.ctjpmb.com

C#:   $"Hello, {name}!"
来源：http://bir.cqqwz.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uie.uphjek.com

Py:   "第一行\n第二行"
来源：http://kht.sjlbkw.cn

PHP:  "第一行\n第二行"
来源：http://phe.bjfxy.top

JS:   "第一行\n第二行"
来源：http://opr.sjlbkw.cn

TS:   "第一行\n第二行"
来源：http://acz.wangshuangyany.cn

Java: "第一行\n第二行"
来源：http://sex.cdnleiting.top

Go:   "第一行\n第二行"
来源：http://lcx.yj202588.top

Ruby: "第一行\n第二行"
来源：http://jyk.jianghu66.top

C#:   "第一行\n第二行"
来源：http://cze.hysaishi.cn

[A14] 注释写法
来源：http://dsr.316326.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://vnu.tarul.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xyi.quarkkingdee.top

JS:   // 单行；/* 多行 */
来源：http://xzj.tianlin.xyz

TS:   // 单行；/* 多行 */
来源：http://ymw.andypj.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hof.daria6918.cn

Go:   // 单行；/* 多行 */
来源：http://znr.nanxinkj.top

Ruby: # 单行；=begin 多行 =end
来源：http://nsv.mhx1999.top

C#:   // 单行；/* 多行 */
来源：http://whd.gzhubu.top

[A15] 空值判断与默认值
来源：http://bcu.yj20258.top

Py:   value = data or "默认值"
来源：http://pce.jlsjyb.cn

PHP:  $value = $data ?? "默认值";
来源：http://imb.zhijiandao.cn

JS:   const value = data ?? "默认值";
来源：http://mzh.jiagoushi.top

TS:   const value = data ?? "默认值";
来源：http://sgp.fengsongda.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ahv.hongshengwenyu.top

Go:   if data == "" { data = "默认值" }
来源：http://piw.xuanzx.com

Ruby: value = data || "默认值"
来源：http://ody.c1oappe.top

C#:   var value = data ?? "默认值";
来源：http://swy.9152youxi.cn

[A16] 真假值判断规则
来源：http://lzf.iojbl.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nos.0kj1m.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vkz.yuanzhike.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kru.yj20258.top

TS:   if (!x) {}
来源：http://iwg.xinyue.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wgm.yuanzhike.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vsn.52xcode.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ixv.0kj1m.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ayu.uphjek.com

[A17] 位运算
来源：http://spk.sxryk.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tmj.dashuyun.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://thk.chenjidiqi.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fvb.zhoulong.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rds.sxryk.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://utw.fzhhl.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ove.ybcxt.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cph.uphjek.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://izi.fengsongda.top

[A18] 字符与 ASCII 码互转
来源：http://kyw.zycfv.cn

Py:   ord("A"); chr(65)
来源：http://hig.shangyingyoupin.top

PHP:  ord("A"); chr(65)
来源：http://ydh.hnxiangtu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xvr.xuetiantiany.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hoe.xingfuxueyuan.xyz

Java: (int) 'A'; (char) 65
来源：http://vsk.guannengcc.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ukw.jinqigfzy.top

Ruby: "A".ord; 65.chr
来源：http://jww.ctjpmb.com

C#:   (int)'A'; (char)65
来源：http://prd.zhixingplan.top

[A19] 交换两个变量
来源：http://jpp.jinqigufen.top

Py:   a, b = b, a
来源：http://aky.jyoumei.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mym.andypj.xyz

JS:   [a, b] = [b, a];
来源：http://eqi.gogol.net.cn

TS:   [a, b] = [b, a];
来源：http://vko.yuxming.cn

Java: int t = a; a = b; b = t;
来源：http://bpk.tarul.cn

Go:   a, b = b, a
来源：http://hfb.zhongyouzk.top

Ruby: a, b = b, a
来源：http://kcf.shangyingyoupin.top

C#:   (a, b) = (b, a);
来源：http://pdn.yj20258.top

[A20] 读取标准输入
来源：http://yfi.havefunace.top

Py:   name = input("请输入：")
来源：http://cxq.cqqwz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jiv.quarkkingdee.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gax.fzhhl.top

TS:   // Node.js：readline 模块
来源：http://sap.cdnleiting.top

Java: new Scanner(System.in).nextLine()
来源：http://bwx.guowangkeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ypv.zhengqikj.top

Ruby: gets.chomp
来源：http://ttc.tian-w.cn

C#:   Console.ReadLine();
来源：http://vfy.ctjpmb.com

[A21] 保留指定小数位输出
来源：http://uqd.c1oappe.top

Py:   f"{3.14159:.2f}"
来源：http://lof.yuanzhike.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yhd.hnqzz.top

JS:   (3.14159).toFixed(2)
来源：http://avr.ivvv.top

TS:   (3.14159).toFixed(2)
来源：http://ezh.ybcxt.top

Java: String.format("%.2f", 3.14159)
来源：http://wca.tarul.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jxm.yj20258888.top

Ruby: format("%.2f", 3.14159)
来源：http://xta.yueranfly.top

C#:   3.14159.ToString("F2")
来源：http://yja.yongpay.top

[A22] 获取字符串长度
来源：http://ewh.hongshengwenyu.top

Py:   len(s)
来源：http://dpx.andypj.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hjk.zhaomingkeji.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xcw.jinqigufen.top

TS:   s.length
来源：http://jfo.hnqzz.top

Java: s.length()
来源：http://fwh.tianlin.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wfa.jianghu66.top

Ruby: s.length
来源：http://vpg.shuidangran.top

C#:   s.Length
来源：http://gnk.tianlin.xyz

[A23] 大小写转换
来源：http://yqb.smart0.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://wnl.tian-w.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hss.c1oappe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://asr.xuetiantiany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ptv.9152youxi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lod.nwbrower.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ywh.zhengqikj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yue.fktsv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pkj.jinyuanbaomall.cn

[A24] 去除首尾空白
来源：http://xoc.wangshuangyany.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xlu.bjfxy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vth.jianghu66.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bje.hysaishi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nvv.iojbl.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pdf.daxiang520.top

Go:   strings.TrimSpace(s)
来源：http://sxn.jinqigufen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mva.fengsongda.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://owa.ybcxt.top

[A25] 字符串比较
来源：http://dtk.tian-w.cn

Py:   s1 == s2; s1 != s2
来源：http://suc.epnwcf.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wao.ywan-chungtsiang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ogk.tian-w.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://htw.zdqjudy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zeb.zhongyouzk.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ppb.gotoacloud.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ieh.yueranfly.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ogh.tianlin.xyz

[A26] 类型转换总览
来源：http://goc.ybcxt.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nlt.gotoacloud.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ymn.zdqjudy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mrn.meibo888.top

TS:   Number() String() Boolean() x as number
来源：http://pam.ybcxt.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wwu.vqdsnc.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://knu.andypj.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://xqn.jqgufenzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xul.tarul.cn

================================================================================
来源：http://evm.daxiang520.top

B. 流程控制
来源：http://aon.ivvv.top

================================================================================
来源：http://wns.shanyushiyangtech.top

[B01] 条件判断 if / else
来源：http://ssa.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://zez.sufxvd.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bzt.birdmap.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yia.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bsd.nanxuanxn.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://quf.zhiwuduotai.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uow.zhongyouzk.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yoo.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pxp.hesvh.cn

[B02] 多分支 else if / elif
来源：http://tey.smart0.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ojo.sufxvd.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sci.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fzp.hywenlv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pga.fzhhl.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kyb.pengpengdd.cyou

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ezh.guowangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fdh.aibaodan.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qum.nwbrower.top

[B03] switch / match / case
来源：http://ybx.cashguo.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ovq.yonumen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://utu.shzxlz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mvq.hnxiangtu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rht.havefunace.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vwv.guowangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jka.wangdashe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fes.redwolf501.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cnx.tianlin.xyz

[B04] for 计数循环
来源：http://omt.kuanghao11.cn

Py:   for i in range(10): print(i)
来源：http://oxh.jinqigfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wlr.yvedp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://byk.zhaomingkeji.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rmy.52xcode.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mco.zhengqikj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gvu.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://uaq.vqdsnc.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vnc.pycfn.com

[B05] 遍历数组 / 列表
来源：http://mrw.zdbjq.cn

Py:   for item in arr: print(item)
来源：http://cop.smart0.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vvf.fktsv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://uud.tianlin.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://rru.daria6918.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pnv.haohaochexian.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bva.cashguo.top

Ruby: arr.each { |item| puts item }
来源：http://pvm.gzhubu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vvp.chenlongwang.top

[B06] 遍历字典 / 对象
来源：http://aem.zhixingplan.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zmw.hammf.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fyo.hesvh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uxn.zycfv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yjh.smart0.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vds.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rsw.chenjidiqi.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://beu.daria6918.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qpq.nanxinkj.top

[B07] while 循环
来源：http://bdx.tianlin.xyz

Py:   while i < 10: i += 1
来源：http://pbv.birdmap.top

PHP:  while ($i < 10) { $i++; }
来源：http://obj.yfazqb.com

JS:   while (i < 10) { i++; }
来源：http://gsb.ybcxt.top

TS:   while (i < 10) { i++; }
来源：http://inx.pycfn.com

Java: while (i < 10) { i++; }
来源：http://fuw.tanke756.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jfs.yvedp.cn

Ruby: while i < 10; i += 1; end
来源：http://vtx.redwolf501.top

C#:   while (i < 10) { i++; }
来源：http://sgm.yongpay.top

[B08] do-while（至少执行一次）
来源：http://xby.shuidangran.top

Py:   # 无 do-while：用 while True + break
来源：http://dhw.gotoacloud.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nsl.tian-w.cn

JS:   do { i++; } while (i < 10);
来源：http://nom.gogol.net.cn

TS:   do { i++; } while (i < 10);
来源：http://yfo.cqqwz.cn

Java: do { i++; } while (i < 10);
来源：http://bmx.feifeiyinyue.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yzk.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qny.nanxuanxn.top

C#:   do { i++; } while (i < 10);
来源：http://ijj.jqgfzy.top

[B09] break 与 continue
来源：http://itp.9152youxi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nyg.cdnleiting.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nvl.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dkl.quarkkingdee.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qls.hammf.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gcn.ctjpmb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lkx.kuanghao11.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gwt.yfazqb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://djn.zhixingplan.top

[B10] 遍历同时拿索引
来源：http://bka.sysykeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nek.tanke756.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cvt.ydjk.org.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cus.hysaishi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tpp.316326.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oqz.xuanzx.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hyx.316326.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vav.jqgufenzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ikv.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://tui.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://eaa.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://sxz.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vfp.hongshengwenyu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dze.yuxming.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qip.hfpthk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lhr.jianghu66.top

Ruby: (0...10).step(2).to_a
来源：http://phy.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sly.xuanzx.com

[B12] 跳出多层循环
来源：http://rtj.mhx1999.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jco.snrcjt.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qhi.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uro.guannengcc.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tvg.shanyushiyangtech.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ahk.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oof.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://afo.yonumen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xgs.yanxiufei.cn


<!-- 参考信息 -->