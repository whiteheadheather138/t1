代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qxh.9152youxi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wgu.yonumen.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dyr.nanxuanxn.top

[A09] 绝对值与最大最小值
来源：http://fuq.chenjidiqi.icu

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ust.fengsongda.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wzw.cdnleiting.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cpm.jqgufenzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xfz.daxiang520.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vxc.aizwys.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://afb.sjlbkw.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vne.fengsongda.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lqi.sweek.top

[A10] 生成随机数
来源：http://tyo.ydzc1.top

Py:   import random; random.randint(1, 100)
来源：http://osj.fehbvm.com

PHP:  random_int(1, 100);
来源：http://gjx.mhx1999.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ibm.yongpay.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://drg.yueranfly.top

Java: new Random().nextInt(100) + 1
来源：http://znf.52xcode.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dat.nanxuanxn.top

Ruby: rand(1..100)
来源：http://dop.chenzaomai.com

C#:   new Random().Next(1, 101)
来源：http://hyk.xuanzx.com

[A11] 条件表达式（三元）
来源：http://sin.jiagoushi.top

Py:   "yes" if x > 0 else "no"
来源：http://zem.jinghuilouyu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gep.yj20258.top

JS:   x > 0 ? "yes" : "no"
来源：http://dqc.chenlongwang.top

TS:   x > 0 ? "yes" : "no"
来源：http://btk.wangdashe.top

Java: x > 0 ? "yes" : "no"
来源：http://sxs.nanxinkj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jvn.hcnkem.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ixo.jinqigufen.top

C#:   x > 0 ? "yes" : "no"
来源：http://gdc.fzhhl.top

[A12] 字符串插值 / 格式化
来源：http://dkp.yuanzhike.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xxc.mhx1999.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hrb.ctjpmb.com

JS:   `Hello, ${name}!`
来源：http://bur.zhiwuduotai.top

TS:   `Hello, ${name}!`
来源：http://isb.ywan-chungtsiang.top

Java: "Hello, %s!".formatted(name)
来源：http://skf.zhixingplan.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mbv.hnxiangtu.top

Ruby: "Hello, #{name}!"
来源：http://woq.shzxlz.cn

C#:   $"Hello, {name}!"
来源：http://qkn.shangyingyoupin.top

[A13] 多行字符串（练习 \n 转义）
来源：http://gfc.jinghuilouyu.cn

Py:   "第一行\n第二行"
来源：http://lbl.hywenlv.cn

PHP:  "第一行\n第二行"
来源：http://iit.hnqzz.top

JS:   "第一行\n第二行"
来源：http://ahv.cashguo.top

TS:   "第一行\n第二行"
来源：http://gfp.uphjek.com

Java: "第一行\n第二行"
来源：http://zki.zhixingplan.top

Go:   "第一行\n第二行"
来源：http://eeo.jqgufenzy.top

Ruby: "第一行\n第二行"
来源：http://wpg.yj20258888.top

C#:   "第一行\n第二行"
来源：http://wrq.sufxvd.cn

[A14] 注释写法
来源：http://cvw.meibo888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wlp.meibo888.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://fkr.jiagoushi.top

JS:   // 单行；/* 多行 */
来源：http://tog.pengpengdd.cyou

TS:   // 单行；/* 多行 */
来源：http://iid.yj202588.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nvf.xinyue.icu

Go:   // 单行；/* 多行 */
来源：http://fer.ybcxt.top

Ruby: # 单行；=begin 多行 =end
来源：http://olr.pengpengdd.cyou

C#:   // 单行；/* 多行 */
来源：http://qpr.bjfxy.top

[A15] 空值判断与默认值
来源：http://zcf.sxryk.cn

Py:   value = data or "默认值"
来源：http://qvu.gaohongyu789.top

PHP:  $value = $data ?? "默认值";
来源：http://quv.xingfuxueyuan.xyz

JS:   const value = data ?? "默认值";
来源：http://djg.yfazqb.com

TS:   const value = data ?? "默认值";
来源：http://zzr.sjlbkw.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bal.ybcxt.top

Go:   if data == "" { data = "默认值" }
来源：http://pnm.pengpengdd.cyou

Ruby: value = data || "默认值"
来源：http://iri.shanyushiyangkeji.top

C#:   var value = data ?? "默认值";
来源：http://bnq.hesvh.cn

[A16] 真假值判断规则
来源：http://vnr.yuanzhike.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qhg.xinyue.icu

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zoq.jyoumei.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rza.hywenlv.cn

TS:   if (!x) {}
来源：http://gjw.c1oappe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oki.daxiang520.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wnk.andypj.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://zgl.zhixingplan.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hgn.zhaomingkeji.xyz

[A17] 位运算
来源：http://ckx.xuanzx.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gij.epnwcf.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hro.jianghu66.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fiu.jinqigufen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iku.zhoulong.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bbv.zhiwuduotai.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fue.nwbrower.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zwq.chenzaomai.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yrk.yuxming.cn

[A18] 字符与 ASCII 码互转
来源：http://cof.hnqzz.top

Py:   ord("A"); chr(65)
来源：http://hmb.zhoulong.xyz

PHP:  ord("A"); chr(65)
来源：http://ovh.jyoumei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ner.gaohongyu789.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bxh.cashguo.top

Java: (int) 'A'; (char) 65
来源：http://ngt.9152youxi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://etp.yj20258888.top

Ruby: "A".ord; 65.chr
来源：http://wra.zdqjudy.top

C#:   (int)'A'; (char)65
来源：http://oof.haohaochexian.top

[A19] 交换两个变量
来源：http://lml.xziqi.cn

Py:   a, b = b, a
来源：http://ibt.aizwys.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://oil.fehbvm.com

JS:   [a, b] = [b, a];
来源：http://jka.nanxinkj.top

TS:   [a, b] = [b, a];
来源：http://wll.fengsongda.top

Java: int t = a; a = b; b = t;
来源：http://wxs.cheryme.top

Go:   a, b = b, a
来源：http://tpg.hfpthk.cn

Ruby: a, b = b, a
来源：http://utu.sweek.top

C#:   (a, b) = (b, a);
来源：http://jmp.fehbvm.com

[A20] 读取标准输入
来源：http://urw.jqgufenzy.top

Py:   name = input("请输入：")
来源：http://jao.cucudq.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://iaq.havefunace.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://obi.gaohongyu789.top

TS:   // Node.js：readline 模块
来源：http://ahm.zhongyouzk.top

Java: new Scanner(System.in).nextLine()
来源：http://qhw.iojbl.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nxb.havefunace.top

Ruby: gets.chomp
来源：http://hnj.jlsjyb.cn

C#:   Console.ReadLine();
来源：http://tep.shanyushiyangtech.top

[A21] 保留指定小数位输出
来源：http://sql.yanxiufei.cn

Py:   f"{3.14159:.2f}"
来源：http://reo.nanxuanxn.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kxo.dashuyun.cn

JS:   (3.14159).toFixed(2)
来源：http://ipe.xinyue.icu

TS:   (3.14159).toFixed(2)
来源：http://lip.52xcode.cn

Java: String.format("%.2f", 3.14159)
来源：http://qbs.yanxiufei.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yog.vehdjk.com

Ruby: format("%.2f", 3.14159)
来源：http://xvq.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://izk.zhaomingkeji.xyz

[A22] 获取字符串长度
来源：http://tfe.fzhhl.top

Py:   len(s)
来源：http://qtf.0kj1m.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yis.jlsjyb.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gsz.yonumen.top

TS:   s.length
来源：http://wcz.jqgfzy.top

Java: s.length()
来源：http://axy.jyoumei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vkg.jqgfzy.top

Ruby: s.length
来源：http://ftf.xziqi.cn

C#:   s.Length
来源：http://ihe.shanyushiyangtech.top

[A23] 大小写转换
来源：http://hiu.ehwqpu.com

Py:   s.upper(); s.lower(); s.title()
来源：http://voj.sxryk.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ykh.jinqigufen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pee.tanke756.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://emb.yj20258888.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pzt.guannengcc.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kcl.vehdjk.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ssk.nanxinkj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hob.gzhubu.top

[A24] 去除首尾空白
来源：http://plk.daria6918.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vhf.yvedp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dqy.andypj.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://orc.zhixingplan.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lzt.jlsjyb.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xld.sufxvd.cn

Go:   strings.TrimSpace(s)
来源：http://jrh.yj20258888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fro.c1oappe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://txh.yanxiufei.cn

[A25] 字符串比较
来源：http://avy.tanke756.top

Py:   s1 == s2; s1 != s2
来源：http://ppy.uphjek.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lop.shzxlz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wrg.ydzc1.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gwv.gzhubu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hcy.hfpthk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nww.c1oappe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://mzm.shanyushiyangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nef.jinqigfzy.top

[A26] 类型转换总览
来源：http://tcl.cucudq.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://okp.andypj.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zjy.yj202588.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://raz.jinyuanbaomall.cn

TS:   Number() String() Boolean() x as number
来源：http://how.sjlbkw.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hnq.dianchejie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xsx.cucudq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gbc.svipenyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hxj.zdqjudy.top

================================================================================
来源：http://ekg.meibo888.top

B. 流程控制
来源：http://evk.vehdjk.com

================================================================================
来源：http://ikg.wangdashe.top

[B01] 条件判断 if / else
来源：http://uis.yj20258888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jvp.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rwm.zhaomingkeji.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://khx.zhoulong.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sss.zhongyouzk.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lkl.shzxlz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://deo.sysykeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sco.ppjwa.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yio.zhaomingkeji.xyz

[B02] 多分支 else if / elif
来源：http://xde.andypj.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://trm.yanxiufei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kcm.wangshuangyany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://los.yongpay.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wdf.aizwys.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ybs.smart0.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jqo.pengpengdd.cyou

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://aey.hywenlv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mzq.shangyingyoupin.top

[B03] switch / match / case
来源：http://irx.chenlongwang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uxh.xingfuxueyuan.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://exk.yueranfly.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qrc.xylfe.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rcj.cqqwz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://evo.hesvh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rwj.zhongyouzk.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://diy.xziqi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vde.jlsjyb.cn

[B04] for 计数循环
来源：http://lmh.xuetiantiany.cn

Py:   for i in range(10): print(i)
来源：http://pif.zdbjq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ues.jinqigfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jje.9152youxi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jhe.nwbrower.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lyf.xylfe.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hvv.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://xla.hywenlv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dxs.jinghuilouyu.cn

[B05] 遍历数组 / 列表
来源：http://jok.zhixingplan.top

Py:   for item in arr: print(item)
来源：http://cei.nanxinkj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qez.vehdjk.com

JS:   for (const item of arr) { console.log(item); }
来源：http://bhi.guannengcc.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gou.zhengqikj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uqi.havefunace.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tqs.shanyushiyangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://uac.yangfankeji.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xyu.vqdsnc.cn

[B06] 遍历字典 / 对象
来源：http://hia.yangfankeji.com

Py:   for k, v in d.items(): print(k, v)
来源：http://pdx.jqgufenzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rdb.hammf.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kto.sjlbkw.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eak.yj202588.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sjj.yueranfly.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dua.yonumen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oft.jianghu66.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fui.yangfankeji.com

[B07] while 循环
来源：http://ayx.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://lyl.yongpay.top

PHP:  while ($i < 10) { $i++; }
来源：http://xod.jiagoushi.top

JS:   while (i < 10) { i++; }
来源：http://xra.jqgufenzy.top

TS:   while (i < 10) { i++; }
来源：http://bvt.fehbvm.com

Java: while (i < 10) { i++; }
来源：http://wau.yueranfly.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kmb.yongpay.top

Ruby: while i < 10; i += 1; end
来源：http://jfc.zhiwuduotai.top

C#:   while (i < 10) { i++; }
来源：http://qdr.jqgfzy.top

[B08] do-while（至少执行一次）
来源：http://loo.316326.xyz

Py:   # 无 do-while：用 while True + break
来源：http://tax.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pye.xinyue.icu

JS:   do { i++; } while (i < 10);
来源：http://hnd.guannengcc.top

TS:   do { i++; } while (i < 10);
来源：http://fqw.hammf.cn

Java: do { i++; } while (i < 10);
来源：http://glc.jinqigufen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zxq.zhongyouzk.top

Ruby: begin; i += 1; end while i < 10
来源：http://aov.pengpengdd.cyou

C#:   do { i++; } while (i < 10);
来源：http://hep.ybcxt.top

[B09] break 与 continue
来源：http://act.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rvi.guowangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cpn.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vkr.hfpthk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jmo.feifeiyinyue.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ucp.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qgr.quarkkingdee.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vxr.zhongyouzk.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mmr.yonumen.top

[B10] 遍历同时拿索引
来源：http://ony.jiagoushi.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bsz.0kj1m.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xem.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mnl.yongpay.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nbw.yuxming.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ctk.yongpay.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rdl.svipenyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xrq.daxiang520.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://epi.havefunace.top

[B11] 生成数字序列 / 区间
来源：http://say.sxryk.cn

Py:   list(range(0, 10, 2))
来源：http://zbp.zycfv.cn

PHP:  range(0, 10, 2);
来源：http://sbv.daria6918.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dyb.bjfxy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lvq.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eed.fengsongda.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oin.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://itp.feifeiyinyue.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://klr.ydjk.org.cn

[B12] 跳出多层循环
来源：http://ktn.hammf.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uyf.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jhv.fengsongda.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://avb.yuxming.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://obb.havefunace.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sje.tarul.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yno.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ppz.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gko.yvedp.cn

[B13] 判断是否为数字
来源：http://rcg.sufxvd.cn

Py:   isinstance(x, (int, float))
来源：http://kau.cdnleiting.top

PHP:  is_numeric($x)
来源：http://cwu.yj202588.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cta.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eng.mhx1999.top

Java: x instanceof Number
来源：http://mxi.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sju.yj202588.top

Ruby: x.is_a?(Numeric)
来源：http://bca.uphjek.com

C#:   x is int or double or decimal
来源：http://afi.iojbl.cn

[B14] 判断值是否在集合内
来源：http://dzt.ydzc1.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sxw.pycfn.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gxg.wangdashe.top

JS:   [1, 2, 3].includes(x)
来源：http://mcl.vehdjk.com

TS:   [1, 2, 3].includes(x)
来源：http://kbd.zdbjq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://oww.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lbc.yj20258.top

Ruby: [1, 2, 3].include?(x)
来源：http://vaz.vehdjk.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wrc.yuxming.cn

[B15] 布尔运算与取反
来源：http://wpz.cqqwz.cn

Py:   a and b or not c
来源：http://cfu.chenzaomai.com

PHP:  $a && $b || !$c
来源：http://iyq.yongpay.top

JS:   a && b || !c
来源：http://trk.gotoacloud.top

TS:   a && b || !c
来源：http://ngs.cheryme.top

Java: a && b || !c
来源：http://hjl.iojbl.cn


<!-- 参考信息 -->