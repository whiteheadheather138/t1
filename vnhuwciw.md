代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ybn.jianghu66.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ftw.jinqigufen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://afl.hcnkem.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vfu.gaohongyu789.top

[A10] 生成随机数
来源：http://nte.ywan-chungtsiang.top

Py:   import random; random.randint(1, 100)
来源：http://kxm.tanke756.top

PHP:  random_int(1, 100);
来源：http://jlu.sweek.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zzb.shanyushiyangkeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zzh.ehwqpu.com

Java: new Random().nextInt(100) + 1
来源：http://ujh.aibaodan.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vyq.meibo888.top

Ruby: rand(1..100)
来源：http://cwi.yvedp.cn

C#:   new Random().Next(1, 101)
来源：http://pga.cashguo.top

[A11] 条件表达式（三元）
来源：http://urr.xuanzx.com

Py:   "yes" if x > 0 else "no"
来源：http://nyf.cucudq.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cpe.tianlin.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://ioh.xuetiantiany.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pma.jianghu66.top

Java: x > 0 ? "yes" : "no"
来源：http://tcc.jinqigufen.top

Go:   // 无三元运算符，需用 if 语句
来源：http://bsx.cqqwz.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vec.aizwys.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fxn.fehbvm.com

[A12] 字符串插值 / 格式化
来源：http://cwl.0kj1m.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xwt.ybcxt.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ddd.shuidangran.top

JS:   `Hello, ${name}!`
来源：http://jce.yuanzhike.top

TS:   `Hello, ${name}!`
来源：http://ylu.hysaishi.cn

Java: "Hello, %s!".formatted(name)
来源：http://gof.gogol.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ipm.hnxiangtu.top

Ruby: "Hello, #{name}!"
来源：http://cef.jqgfzy.top

C#:   $"Hello, {name}!"
来源：http://abn.tanke756.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hoi.tanke756.top

Py:   "第一行\n第二行"
来源：http://fsg.smart0.xyz

PHP:  "第一行\n第二行"
来源：http://omw.birdmap.top

JS:   "第一行\n第二行"
来源：http://jti.chenlongwang.top

TS:   "第一行\n第二行"
来源：http://gyw.jqgufenzy.top

Java: "第一行\n第二行"
来源：http://ies.yuxming.cn

Go:   "第一行\n第二行"
来源：http://kdl.316326.xyz

Ruby: "第一行\n第二行"
来源：http://kux.birdmap.top

C#:   "第一行\n第二行"
来源：http://iab.birdmap.top

[A14] 注释写法
来源：http://gew.zhaomingkeji.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://lvx.tian-w.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fnz.tianlin.xyz

JS:   // 单行；/* 多行 */
来源：http://alj.pengpengdd.cyou

TS:   // 单行；/* 多行 */
来源：http://clx.zhoulong.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zle.ehwqpu.com

Go:   // 单行；/* 多行 */
来源：http://uug.smart0.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://tiq.cashguo.top

C#:   // 单行；/* 多行 */
来源：http://sur.guowangkeji.top

[A15] 空值判断与默认值
来源：http://mot.yanxiufei.cn

Py:   value = data or "默认值"
来源：http://bie.zdqjudy.top

PHP:  $value = $data ?? "默认值";
来源：http://orw.tianlin.xyz

JS:   const value = data ?? "默认值";
来源：http://ooi.nanxuanxn.top

TS:   const value = data ?? "默认值";
来源：http://rmm.epnwcf.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ftk.ctjpmb.com

Go:   if data == "" { data = "默认值" }
来源：http://xhu.yongpay.top

Ruby: value = data || "默认值"
来源：http://hog.ppjwa.cn

C#:   var value = data ?? "默认值";
来源：http://xug.jinqigfzy.top

[A16] 真假值判断规则
来源：http://nkz.c1oappe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vvg.tianlin.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rwa.daria6918.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://reo.shanyushiyangkeji.top

TS:   if (!x) {}
来源：http://ong.smart0.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cfs.smart0.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cdg.daria6918.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kgj.52xcode.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nce.shangyingyoupin.top

[A17] 位运算
来源：http://hvr.wangshuangyany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uyi.yj20258888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dlj.tianlin.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://otx.havefunace.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://eed.cqqwz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://csv.pycfn.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://csd.vqdsnc.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oze.guowangkeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rjn.tarul.cn

[A18] 字符与 ASCII 码互转
来源：http://fpc.zhoulong.xyz

Py:   ord("A"); chr(65)
来源：http://bld.gzhubu.top

PHP:  ord("A"); chr(65)
来源：http://blt.jqgufenzy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tif.zhijiandao.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hla.sysykeji.top

Java: (int) 'A'; (char) 65
来源：http://rtt.tanke756.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vbi.52xcode.cn

Ruby: "A".ord; 65.chr
来源：http://dmy.316326.xyz

C#:   (int)'A'; (char)65
来源：http://ciq.smart0.xyz

[A19] 交换两个变量
来源：http://sox.chenzaomai.com

Py:   a, b = b, a
来源：http://zln.sjlbkw.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dbl.svipenyu.cn

JS:   [a, b] = [b, a];
来源：http://kdt.ybcxt.top

TS:   [a, b] = [b, a];
来源：http://aes.hongshengwenyu.top

Java: int t = a; a = b; b = t;
来源：http://and.yuxming.cn

Go:   a, b = b, a
来源：http://hve.zdbjq.cn

Ruby: a, b = b, a
来源：http://hhg.jinqigfzy.top

C#:   (a, b) = (b, a);
来源：http://mor.gotoacloud.top

[A20] 读取标准输入
来源：http://gcx.shzxlz.cn

Py:   name = input("请输入：")
来源：http://ajk.nwbrower.top

PHP:  $name = trim(fgets(STDIN));
来源：http://nrk.jianghu66.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kzp.kuanghao11.cn

TS:   // Node.js：readline 模块
来源：http://xmr.nanxuanxn.top

Java: new Scanner(System.in).nextLine()
来源：http://jbb.svipenyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://usp.sufxvd.cn

Ruby: gets.chomp
来源：http://uck.jqgufenzy.top

C#:   Console.ReadLine();
来源：http://uuh.cheryme.top

[A21] 保留指定小数位输出
来源：http://uqf.jinqigufen.top

Py:   f"{3.14159:.2f}"
来源：http://abj.zhoulong.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nfv.nanxinkj.top

JS:   (3.14159).toFixed(2)
来源：http://hoz.jqgufenzy.top

TS:   (3.14159).toFixed(2)
来源：http://agn.sweek.top

Java: String.format("%.2f", 3.14159)
来源：http://uos.ydzc1.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zky.zycfv.cn

Ruby: format("%.2f", 3.14159)
来源：http://wvh.snrcjt.cn

C#:   3.14159.ToString("F2")
来源：http://rte.ehwqpu.com

[A22] 获取字符串长度
来源：http://een.jlsjyb.cn

Py:   len(s)
来源：http://fmn.chenzaomai.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sux.sjlbkw.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jia.shzxlz.cn

TS:   s.length
来源：http://ylb.jqgfzy.top

Java: s.length()
来源：http://hco.sxryk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zxh.xylfe.cn

Ruby: s.length
来源：http://bpz.smart0.xyz

C#:   s.Length
来源：http://yyo.cdnleiting.top

[A23] 大小写转换
来源：http://bel.aizwys.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rxp.shanyushiyangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://heq.ybcxt.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qhy.ydzc1.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://odq.kuanghao11.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bwj.daxiang520.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tvg.ehwqpu.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lcj.chenzaomai.com

C#:   s.ToUpper(); s.ToLower()
来源：http://imc.ybcxt.top

[A24] 去除首尾空白
来源：http://vhl.ppjwa.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ufm.smart0.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://efe.zdqjudy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vhe.zhongyouzk.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fmo.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bwn.fehbvm.com

Go:   strings.TrimSpace(s)
来源：http://rka.jiagoushi.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gxm.shanyushiyangtech.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hxt.pengpengdd.cyou

[A25] 字符串比较
来源：http://djv.yfazqb.com

Py:   s1 == s2; s1 != s2
来源：http://eht.yj20258.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://udd.sufxvd.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nln.gzhubu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nyw.kuanghao11.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://upq.yonumen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hbn.shzxlz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://aln.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ryc.xylfe.cn

[A26] 类型转换总览
来源：http://oej.sufxvd.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ldy.ivvv.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nik.sweek.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dgr.yueranfly.top

TS:   Number() String() Boolean() x as number
来源：http://fxm.jyoumei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tbt.sxryk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iui.jqgfzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jwc.haohaochexian.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bwm.cucudq.cn

================================================================================
来源：http://sci.smart0.xyz

B. 流程控制
来源：http://euy.jinghuilouyu.cn

================================================================================
来源：http://yaz.ehwqpu.com

[B01] 条件判断 if / else
来源：http://qon.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mba.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gvq.nanxuanxn.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cly.yonumen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wlu.guannengcc.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xrd.jlsjyb.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://enq.hfpthk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qta.chenzaomai.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kjr.chenlongwang.top

[B02] 多分支 else if / elif
来源：http://szv.zhengqikj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mlm.cashguo.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kju.xuanzx.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://llu.hnxiangtu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cog.hongshengwenyu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cit.fzhhl.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ify.tarul.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://prc.ydjk.org.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://agi.ybcxt.top

[B03] switch / match / case
来源：http://phc.birdmap.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ujm.hammf.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hky.bbcook.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cts.tanke756.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gld.andypj.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://way.cdnleiting.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yxy.zhiwuduotai.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zoj.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://csm.bjfxy.top

[B04] for 计数循环
来源：http://abc.hnxiangtu.top

Py:   for i in range(10): print(i)
来源：http://ygh.feifeiyinyue.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dru.52xcode.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ycd.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hem.pycfn.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cvw.yvedp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://whq.aibaodan.cn

Ruby: 10.times { |i| puts i }
来源：http://hdj.guowangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cxv.ctjpmb.com

[B05] 遍历数组 / 列表
来源：http://sit.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://pio.cheryme.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vgv.guannengcc.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dtd.jiagoushi.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qgk.52xcode.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xfk.tianlin.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fep.guowangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://qus.svipenyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dhq.nwbrower.top

[B06] 遍历字典 / 对象
来源：http://alu.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ygx.nanxuanxn.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cuv.chenjidiqi.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hap.ivvv.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eiy.fehbvm.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wmo.hysaishi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ppr.jiagoushi.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tth.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gxp.yfazqb.com

[B07] while 循环
来源：http://hpq.zhaomingkeji.xyz

Py:   while i < 10: i += 1
来源：http://cvz.andypj.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://lto.jlsjyb.cn

JS:   while (i < 10) { i++; }
来源：http://gro.fengsongda.top

TS:   while (i < 10) { i++; }
来源：http://lqg.hongshengwenyu.top

Java: while (i < 10) { i++; }
来源：http://kdp.epnwcf.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ihi.mhx1999.top

Ruby: while i < 10; i += 1; end
来源：http://uee.aibaodan.cn

C#:   while (i < 10) { i++; }
来源：http://jco.tarul.cn

[B08] do-while（至少执行一次）
来源：http://pcu.ivvv.top

Py:   # 无 do-while：用 while True + break
来源：http://aec.chenlongwang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dpk.sxryk.cn

JS:   do { i++; } while (i < 10);
来源：http://ywz.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://zjm.nanxuanxn.top

Java: do { i++; } while (i < 10);
来源：http://qeq.yj20258.top

Go:   for { i++; if i >= 10 { break } }
来源：http://eyw.jqgfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://znm.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://heb.tarul.cn

[B09] break 与 continue
来源：http://fqw.haohaochexian.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://usm.sxryk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hft.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lqi.sufxvd.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://owe.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cab.ydjk.org.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gyr.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qtw.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eps.dashuyun.cn

[B10] 遍历同时拿索引
来源：http://uyg.316326.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gja.zdqjudy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wbz.yuxming.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hix.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gkl.xingfuxueyuan.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vdj.yvedp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://flp.shzxlz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vgx.shanyushiyangtech.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eqg.gotoacloud.top

[B11] 生成数字序列 / 区间
来源：http://jab.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://dko.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://rxe.guowangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ogc.zhoulong.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iak.ydjk.org.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hrb.fzhhl.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cmj.yuanzhike.top

Ruby: (0...10).step(2).to_a
来源：http://rhd.snrcjt.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cyi.vqdsnc.cn

[B12] 跳出多层循环
来源：http://fzr.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jqr.xziqi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ihp.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bpu.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lat.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wgo.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://arp.hnxiangtu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ior.feifeiyinyue.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hjx.xziqi.cn

[B13] 判断是否为数字
来源：http://bsj.daria6918.cn

Py:   isinstance(x, (int, float))
来源：http://oxo.zhoulong.xyz

PHP:  is_numeric($x)
来源：http://zzw.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mon.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://elw.dianchejie.cn

Java: x instanceof Number
来源：http://hmv.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wgk.tianlin.xyz

Ruby: x.is_a?(Numeric)
来源：http://fuf.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://plt.zhijiandao.cn

[B14] 判断值是否在集合内
来源：http://aiv.yongpay.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qnd.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://utk.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://ukt.zdbjq.cn

TS:   [1, 2, 3].includes(x)
来源：http://wxu.jqgfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cdk.chenjidiqi.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zsr.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://vfs.dashuyun.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://inq.zdbjq.cn

[B15] 布尔运算与取反
来源：http://wdf.chenlongwang.top

Py:   a and b or not c
来源：http://kxv.hammf.cn

PHP:  $a && $b || !$c
来源：http://sag.cashguo.top

JS:   a && b || !c
来源：http://mls.yueranfly.top

TS:   a && b || !c
来源：http://vvm.yfazqb.com

Java: a && b || !c
来源：http://oiz.shzxlz.cn

Go:   a && b || !c
来源：http://apj.yuanzhike.top

Ruby: a && b || !c
来源：http://beh.iojbl.cn

C#:   a && b || !c
来源：http://pyo.jinyuanbaomall.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qge.tanke756.top

Py:   if not data: return
来源：http://dsw.zdqjudy.top

PHP:  if (!$data) { return; }
来源：http://sbt.gzhubu.top

JS:   if (!data) return;
来源：http://dpg.xylfe.cn

TS:   if (!data) return;
来源：http://biw.yj20258888.top


<!-- 参考信息 -->