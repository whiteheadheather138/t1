代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mxr.hcnkem.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yra.316326.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xku.hcnkem.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jry.svipenyu.cn

[A10] 生成随机数
来源：http://pvj.sxryk.cn

Py:   import random; random.randint(1, 100)
来源：http://wnb.c1oappe.top

PHP:  random_int(1, 100);
来源：http://jtq.meibo888.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cyc.vqdsnc.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jok.nanxinkj.top

Java: new Random().nextInt(100) + 1
来源：http://olm.uphjek.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pnv.daxiang520.top

Ruby: rand(1..100)
来源：http://jyf.pycfn.com

C#:   new Random().Next(1, 101)
来源：http://flr.jinqigfzy.top

[A11] 条件表达式（三元）
来源：http://gji.guowangkeji.top

Py:   "yes" if x > 0 else "no"
来源：http://kfz.nanxinkj.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://cgy.birdmap.top

JS:   x > 0 ? "yes" : "no"
来源：http://dza.gogol.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ggh.sweek.top

Java: x > 0 ? "yes" : "no"
来源：http://bto.gotoacloud.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pdv.shanyushiyangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://kjj.ybcxt.top

C#:   x > 0 ? "yes" : "no"
来源：http://rzy.zhengqikj.top

[A12] 字符串插值 / 格式化
来源：http://uxr.daxiang520.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ump.pengpengdd.cyou

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kzq.guannengcc.top

JS:   `Hello, ${name}!`
来源：http://tme.ctjpmb.com

TS:   `Hello, ${name}!`
来源：http://sqh.yuxming.cn

Java: "Hello, %s!".formatted(name)
来源：http://nwp.zhengqikj.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://aax.ivvv.top

Ruby: "Hello, #{name}!"
来源：http://vjv.tarul.cn

C#:   $"Hello, {name}!"
来源：http://mvz.yfazqb.com

[A13] 多行字符串（练习 \n 转义）
来源：http://mdx.zdbjq.cn

Py:   "第一行\n第二行"
来源：http://zmw.shuidangran.top

PHP:  "第一行\n第二行"
来源：http://ctk.cashguo.top

JS:   "第一行\n第二行"
来源：http://ggc.yonumen.top

TS:   "第一行\n第二行"
来源：http://kll.shanyushiyangtech.top

Java: "第一行\n第二行"
来源：http://nts.52xcode.cn

Go:   "第一行\n第二行"
来源：http://rid.fengsongda.top

Ruby: "第一行\n第二行"
来源：http://kbm.ehwqpu.com

C#:   "第一行\n第二行"
来源：http://wmx.ppjwa.cn

[A14] 注释写法
来源：http://qwb.zdqjudy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://qrd.aibaodan.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ktc.redwolf501.top

JS:   // 单行；/* 多行 */
来源：http://axf.jlsjyb.cn

TS:   // 单行；/* 多行 */
来源：http://hwu.gotoacloud.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tlw.daria6918.cn

Go:   // 单行；/* 多行 */
来源：http://ovu.hysaishi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qur.shanyushiyangkeji.top

C#:   // 单行；/* 多行 */
来源：http://kyw.nwbrower.top

[A15] 空值判断与默认值
来源：http://hoq.sufxvd.cn

Py:   value = data or "默认值"
来源：http://cxt.xinyue.icu

PHP:  $value = $data ?? "默认值";
来源：http://fcr.jiagoushi.top

JS:   const value = data ?? "默认值";
来源：http://ony.ybcxt.top

TS:   const value = data ?? "默认值";
来源：http://ute.cdnleiting.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://iwm.andypj.xyz

Go:   if data == "" { data = "默认值" }
来源：http://wms.zdbjq.cn

Ruby: value = data || "默认值"
来源：http://udx.hywenlv.cn

C#:   var value = data ?? "默认值";
来源：http://soi.zhijiandao.cn

[A16] 真假值判断规则
来源：http://ifv.hcnkem.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hxb.yongpay.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://amn.zycfv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fhd.sjlbkw.cn

TS:   if (!x) {}
来源：http://nnh.c1oappe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uah.hfpthk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dzz.sweek.top

Ruby: unless x            # nil 与 false 为假
来源：http://xnu.sjlbkw.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ecy.meibo888.top

[A17] 位运算
来源：http://lqh.9152youxi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dct.fehbvm.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nev.uphjek.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gpk.vehdjk.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gje.xingfuxueyuan.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cgb.uphjek.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ocu.chenlongwang.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qxc.hcnkem.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://axz.yfazqb.com

[A18] 字符与 ASCII 码互转
来源：http://roh.aizwys.cn

Py:   ord("A"); chr(65)
来源：http://wlx.0kj1m.cn

PHP:  ord("A"); chr(65)
来源：http://xem.snrcjt.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jdi.birdmap.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mod.sxryk.cn

Java: (int) 'A'; (char) 65
来源：http://nks.gotoacloud.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qnk.yangfankeji.com

Ruby: "A".ord; 65.chr
来源：http://ber.snrcjt.cn

C#:   (int)'A'; (char)65
来源：http://rxw.cashguo.top

[A19] 交换两个变量
来源：http://tho.zhongyouzk.top

Py:   a, b = b, a
来源：http://mtx.jqgufenzy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ntn.ehwqpu.com

JS:   [a, b] = [b, a];
来源：http://ubz.smart0.xyz

TS:   [a, b] = [b, a];
来源：http://mzd.yangfankeji.com

Java: int t = a; a = b; b = t;
来源：http://lll.cqqwz.cn

Go:   a, b = b, a
来源：http://ocq.zhiwuduotai.top

Ruby: a, b = b, a
来源：http://kji.ivvv.top

C#:   (a, b) = (b, a);
来源：http://frq.sxryk.cn

[A20] 读取标准输入
来源：http://hyj.yangfankeji.com

Py:   name = input("请输入：")
来源：http://bnv.pycfn.com

PHP:  $name = trim(fgets(STDIN));
来源：http://rae.havefunace.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dpo.xuanzx.com

TS:   // Node.js：readline 模块
来源：http://vbh.gotoacloud.top

Java: new Scanner(System.in).nextLine()
来源：http://ntx.zdbjq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mim.cdnleiting.top

Ruby: gets.chomp
来源：http://hxr.gotoacloud.top

C#:   Console.ReadLine();
来源：http://wks.ydjk.org.cn

[A21] 保留指定小数位输出
来源：http://wzy.snrcjt.cn

Py:   f"{3.14159:.2f}"
来源：http://ifl.zycfv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ffl.jinqigfzy.top

JS:   (3.14159).toFixed(2)
来源：http://aqq.xylfe.cn

TS:   (3.14159).toFixed(2)
来源：http://ulu.daria6918.cn

Java: String.format("%.2f", 3.14159)
来源：http://wpr.yfazqb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ppx.vehdjk.com

Ruby: format("%.2f", 3.14159)
来源：http://tke.chenjidiqi.icu

C#:   3.14159.ToString("F2")
来源：http://bsd.fzhhl.top

[A22] 获取字符串长度
来源：http://vnv.jinghuilouyu.cn

Py:   len(s)
来源：http://opr.yj202588.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ncg.ybcxt.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zxo.nwbrower.top

TS:   s.length
来源：http://ibt.hnqzz.top

Java: s.length()
来源：http://wir.smart0.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bml.uphjek.com

Ruby: s.length
来源：http://qsn.sjlbkw.cn

C#:   s.Length
来源：http://jfs.tanke756.top

[A23] 大小写转换
来源：http://lxa.gotoacloud.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nuj.fktsv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bdw.tian-w.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bqb.sufxvd.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tna.hywenlv.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wmd.wangshuangyany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hwp.gogol.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wnb.zhijiandao.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://man.pycfn.com

[A24] 去除首尾空白
来源：http://hrj.c1oappe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fxw.pycfn.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hqo.meibo888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jui.vehdjk.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yti.fzhhl.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xic.daria6918.cn

Go:   strings.TrimSpace(s)
来源：http://fxn.hesvh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yhi.c1oappe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xuz.smart0.xyz

[A25] 字符串比较
来源：http://ehh.hesvh.cn

Py:   s1 == s2; s1 != s2
来源：http://tsz.haohaochexian.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ypb.0kj1m.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://boj.52xcode.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nzs.hammf.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uft.vehdjk.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://duc.cucudq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xfy.iojbl.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mhk.cashguo.top

[A26] 类型转换总览
来源：http://url.hywenlv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jbo.guannengcc.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://esj.hysaishi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ido.shanyushiyangtech.top

TS:   Number() String() Boolean() x as number
来源：http://thf.tian-w.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uqv.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lsr.guannengcc.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://myq.chenzaomai.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mua.dianchejie.cn

================================================================================
来源：http://otj.shuidangran.top

B. 流程控制
来源：http://nah.xziqi.cn

================================================================================
来源：http://yvo.jqgufenzy.top

[B01] 条件判断 if / else
来源：http://llb.yfazqb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://vej.zhoulong.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lfp.gaohongyu789.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://emu.yuxming.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://enq.zhiwuduotai.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://htm.vqdsnc.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ezn.dianchejie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kat.jinghuilouyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://syd.meibo888.top

[B02] 多分支 else if / elif
来源：http://fst.zdbjq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yrt.vqdsnc.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aqp.wangdashe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tvs.zhoulong.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://loj.sufxvd.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nit.hnxiangtu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zvt.epnwcf.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nnn.zycfv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nuj.xinyue.icu

[B03] switch / match / case
来源：http://duf.9152youxi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://smy.yj20258.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lrv.hammf.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hyy.tanke756.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aco.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fcs.andypj.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eyd.daxiang520.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://olp.yfazqb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ihx.chenjidiqi.icu

[B04] for 计数循环
来源：http://wie.cucudq.cn

Py:   for i in range(10): print(i)
来源：http://ovy.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fzk.c1oappe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bvt.feifeiyinyue.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hnv.jqgfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ekf.shanyushiyangtech.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nvi.ivvv.top

Ruby: 10.times { |i| puts i }
来源：http://par.yj202588.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ncf.ybcxt.top

[B05] 遍历数组 / 列表
来源：http://xax.zdqjudy.top

Py:   for item in arr: print(item)
来源：http://zxc.yongpay.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mob.wangdashe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wsp.gogol.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ypr.0kj1m.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zdj.gogol.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dlb.guowangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://pmi.jianghu66.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xbr.andypj.xyz

[B06] 遍历字典 / 对象
来源：http://lmw.xziqi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rtk.hnxiangtu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://coc.uphjek.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pny.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lmr.zhijiandao.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://biv.sjlbkw.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hsm.c1oappe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iui.fktsv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pzh.shuidangran.top

[B07] while 循环
来源：http://evf.dianchejie.cn

Py:   while i < 10: i += 1
来源：http://yrm.hywenlv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nmu.hnqzz.top

JS:   while (i < 10) { i++; }
来源：http://eus.tanke756.top

TS:   while (i < 10) { i++; }
来源：http://irl.nanxuanxn.top

Java: while (i < 10) { i++; }
来源：http://cua.hywenlv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vwb.aibaodan.cn

Ruby: while i < 10; i += 1; end
来源：http://kxe.jinyuanbaomall.cn

C#:   while (i < 10) { i++; }
来源：http://qle.fktsv.cn

[B08] do-while（至少执行一次）
来源：http://ngk.52xcode.cn

Py:   # 无 do-while：用 while True + break
来源：http://myq.jyoumei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xnu.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://ioh.yongpay.top

TS:   do { i++; } while (i < 10);
来源：http://xsb.jinqigufen.top

Java: do { i++; } while (i < 10);
来源：http://wxg.sysykeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yjo.sxryk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rfi.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://rwz.tianlin.xyz

[B09] break 与 continue
来源：http://gob.zhixingplan.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xvy.fengsongda.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ypn.meibo888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rgc.gzhubu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zsv.jinyuanbaomall.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qbu.redwolf501.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rns.fktsv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ylw.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rrf.shangyingyoupin.top

[B10] 遍历同时拿索引
来源：http://oei.jlsjyb.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ijm.redwolf501.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nlw.jinqigfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gcd.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uff.zhongyouzk.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eqb.yj20258.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ixd.316326.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kwx.sufxvd.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ymy.hfpthk.cn

[B11] 生成数字序列 / 区间
来源：http://jzg.yueranfly.top

Py:   list(range(0, 10, 2))
来源：http://hqo.snrcjt.cn

PHP:  range(0, 10, 2);
来源：http://gyy.vehdjk.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mvb.zdqjudy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mpy.ivvv.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kzm.sxryk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rdl.gotoacloud.top

Ruby: (0...10).step(2).to_a
来源：http://hcj.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hqg.iojbl.cn

[B12] 跳出多层循环
来源：http://ufe.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xjb.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://suw.ppjwa.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://akp.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ixt.xziqi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mnm.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iea.nwbrower.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qzj.zhixingplan.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rfu.jinyuanbaomall.cn

[B13] 判断是否为数字
来源：http://nit.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://rpu.tarul.cn

PHP:  is_numeric($x)
来源：http://vbb.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vug.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uit.chenjidiqi.icu

Java: x instanceof Number
来源：http://iap.dianchejie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rpm.ctjpmb.com

Ruby: x.is_a?(Numeric)
来源：http://tzr.snrcjt.cn

C#:   x is int or double or decimal
来源：http://ige.hammf.cn

[B14] 判断值是否在集合内
来源：http://zob.pycfn.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oaj.cashguo.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nrx.fehbvm.com

JS:   [1, 2, 3].includes(x)
来源：http://mgq.sjlbkw.cn

TS:   [1, 2, 3].includes(x)
来源：http://tcd.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://vjb.yueranfly.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xej.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://nbw.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ikg.yj202588.top

[B15] 布尔运算与取反
来源：http://ysz.wangdashe.top

Py:   a and b or not c
来源：http://hwp.aibaodan.cn

PHP:  $a && $b || !$c
来源：http://sox.iojbl.cn

JS:   a && b || !c
来源：http://nfj.hcnkem.com

TS:   a && b || !c
来源：http://kil.wangshuangyany.cn

Java: a && b || !c
来源：http://kze.yangfankeji.com

Go:   a && b || !c
来源：http://xay.cashguo.top

Ruby: a && b || !c
来源：http://qae.iojbl.cn

C#:   a && b || !c
来源：http://qzj.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rni.feifeiyinyue.top

Py:   if not data: return
来源：http://bai.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://zft.vehdjk.com

JS:   if (!data) return;
来源：http://gxl.52xcode.cn

TS:   if (!data) return;
来源：http://wrj.chenzaomai.com


<!-- 参考信息 -->