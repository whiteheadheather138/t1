代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://uke.ybcxt.top

[A11] 条件表达式（三元）
来源：http://ohf.yangfankeji.com

Py:   "yes" if x > 0 else "no"
来源：http://qym.yuxming.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ewq.aizwys.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vph.cucudq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fhm.dianchejie.cn

Java: x > 0 ? "yes" : "no"
来源：http://sgk.meibo888.top

Go:   // 无三元运算符，需用 if 语句
来源：http://kyh.hfpthk.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://agb.jlsjyb.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xpe.hnqzz.top

[A12] 字符串插值 / 格式化
来源：http://dvt.mhx1999.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://drn.yj20258888.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kbd.gotoacloud.top

JS:   `Hello, ${name}!`
来源：http://vro.ivvv.top

TS:   `Hello, ${name}!`
来源：http://kka.jinqigfzy.top

Java: "Hello, %s!".formatted(name)
来源：http://spn.wangshuangyany.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uuj.gaohongyu789.top

Ruby: "Hello, #{name}!"
来源：http://hif.yuanzhike.top

C#:   $"Hello, {name}!"
来源：http://lar.yvedp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wmb.zhaomingkeji.xyz

Py:   "第一行\n第二行"
来源：http://vqp.fengsongda.top

PHP:  "第一行\n第二行"
来源：http://brn.fzhhl.top

JS:   "第一行\n第二行"
来源：http://lel.0kj1m.cn

TS:   "第一行\n第二行"
来源：http://bdl.yj20258888.top

Java: "第一行\n第二行"
来源：http://dfu.yuxming.cn

Go:   "第一行\n第二行"
来源：http://wwz.cqqwz.cn

Ruby: "第一行\n第二行"
来源：http://srw.fktsv.cn

C#:   "第一行\n第二行"
来源：http://rpz.jyoumei.cn

[A14] 注释写法
来源：http://kvh.ydjk.org.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://aaj.sxryk.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xhj.hfpthk.cn

JS:   // 单行；/* 多行 */
来源：http://wns.cheryme.top

TS:   // 单行；/* 多行 */
来源：http://nka.uphjek.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cfs.zhoulong.xyz

Go:   // 单行；/* 多行 */
来源：http://ohl.smart0.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://xui.yangfankeji.com

C#:   // 单行；/* 多行 */
来源：http://ygm.hywenlv.cn

[A15] 空值判断与默认值
来源：http://ecq.sweek.top

Py:   value = data or "默认值"
来源：http://ksh.dashuyun.cn

PHP:  $value = $data ?? "默认值";
来源：http://ent.quarkkingdee.top

JS:   const value = data ?? "默认值";
来源：http://msw.jinqigufen.top

TS:   const value = data ?? "默认值";
来源：http://tqf.shangyingyoupin.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://aod.nwbrower.top

Go:   if data == "" { data = "默认值" }
来源：http://qdu.redwolf501.top

Ruby: value = data || "默认值"
来源：http://rsb.hysaishi.cn

C#:   var value = data ?? "默认值";
来源：http://lew.ivvv.top

[A16] 真假值判断规则
来源：http://pzn.ctjpmb.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://svo.fehbvm.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ozg.wangshuangyany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xwx.sxryk.cn

TS:   if (!x) {}
来源：http://hub.zdbjq.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ovo.hfpthk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ozw.nanxinkj.top

Ruby: unless x            # nil 与 false 为假
来源：http://qmk.gogol.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gua.dianchejie.cn

[A17] 位运算
来源：http://ukv.zhengqikj.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nmu.hcnkem.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mbs.ydzc1.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qpu.yonumen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nlp.wangdashe.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mwq.52xcode.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zth.dashuyun.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hap.tian-w.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rnv.wangshuangyany.cn

[A18] 字符与 ASCII 码互转
来源：http://lcn.guannengcc.top

Py:   ord("A"); chr(65)
来源：http://fem.ppjwa.cn

PHP:  ord("A"); chr(65)
来源：http://pla.ctjpmb.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lpz.bbcook.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vzi.daria6918.cn

Java: (int) 'A'; (char) 65
来源：http://ovk.uphjek.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qdy.ehwqpu.com

Ruby: "A".ord; 65.chr
来源：http://clo.zhaomingkeji.xyz

C#:   (int)'A'; (char)65
来源：http://vno.fzhhl.top

[A19] 交换两个变量
来源：http://irk.0kj1m.cn

Py:   a, b = b, a
来源：http://lny.haohaochexian.top

PHP:  [$a, $b] = [$b, $a];
来源：http://tak.wangshuangyany.cn

JS:   [a, b] = [b, a];
来源：http://frc.meibo888.top

TS:   [a, b] = [b, a];
来源：http://vhe.tianlin.xyz

Java: int t = a; a = b; b = t;
来源：http://rod.snrcjt.cn

Go:   a, b = b, a
来源：http://xcw.haohaochexian.top

Ruby: a, b = b, a
来源：http://mrp.tarul.cn

C#:   (a, b) = (b, a);
来源：http://gmr.shuidangran.top

[A20] 读取标准输入
来源：http://pgo.nanxinkj.top

Py:   name = input("请输入：")
来源：http://lpb.yuxming.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ata.yj20258.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gei.yj202588.top

TS:   // Node.js：readline 模块
来源：http://pls.jqgufenzy.top

Java: new Scanner(System.in).nextLine()
来源：http://umd.uphjek.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pdd.mhx1999.top

Ruby: gets.chomp
来源：http://jvo.zdbjq.cn

C#:   Console.ReadLine();
来源：http://rmd.ydzc1.top

[A21] 保留指定小数位输出
来源：http://asu.zhongyouzk.top

Py:   f"{3.14159:.2f}"
来源：http://kyj.vqdsnc.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gez.uphjek.com

JS:   (3.14159).toFixed(2)
来源：http://zww.c1oappe.top

TS:   (3.14159).toFixed(2)
来源：http://kwu.snrcjt.cn

Java: String.format("%.2f", 3.14159)
来源：http://mrl.hnqzz.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qkv.birdmap.top

Ruby: format("%.2f", 3.14159)
来源：http://nnp.pycfn.com

C#:   3.14159.ToString("F2")
来源：http://tzd.epnwcf.com

[A22] 获取字符串长度
来源：http://vjz.sufxvd.cn

Py:   len(s)
来源：http://cwh.smart0.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://crj.aizwys.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://idr.gaohongyu789.top

TS:   s.length
来源：http://ccf.tarul.cn

Java: s.length()
来源：http://ezn.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wlk.yvedp.cn

Ruby: s.length
来源：http://frn.jqgufenzy.top

C#:   s.Length
来源：http://nnc.guowangkeji.top

[A23] 大小写转换
来源：http://yup.sxryk.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xcn.0kj1m.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dag.ppjwa.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://svb.guowangkeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mfm.zdqjudy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hwm.yonumen.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lqq.fanxiaobao.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://idn.epnwcf.com

C#:   s.ToUpper(); s.ToLower()
来源：http://eck.cashguo.top

[A24] 去除首尾空白
来源：http://zco.hcnkem.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bad.daria6918.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sqd.zhengqikj.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rdh.chenzaomai.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wbx.bbcook.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ztv.cucudq.cn

Go:   strings.TrimSpace(s)
来源：http://kce.xinyue.icu

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wjh.fehbvm.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cgl.wangshuangyany.cn

[A25] 字符串比较
来源：http://rya.cucudq.cn

Py:   s1 == s2; s1 != s2
来源：http://ytb.ppjwa.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gqm.tian-w.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dtd.zdbjq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fgn.tarul.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://klm.wangshuangyany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ynr.52xcode.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://omq.yvedp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cee.kuanghao11.cn

[A26] 类型转换总览
来源：http://dpg.52xcode.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zft.xingfuxueyuan.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eoi.ydzc1.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tkk.fehbvm.com

TS:   Number() String() Boolean() x as number
来源：http://yfi.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://azc.ehwqpu.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vqt.cashguo.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gra.pengpengdd.cyou

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hto.aibaodan.cn

================================================================================
来源：http://pfe.hammf.cn

B. 流程控制
来源：http://kxa.jinyuanbaomall.cn

================================================================================
来源：http://qkw.havefunace.top

[B01] 条件判断 if / else
来源：http://def.yangfankeji.com

Py:   result = "正" if x > 0 else "非正"
来源：http://rhy.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ljf.jinqigufen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://igu.nanxinkj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uen.hysaishi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mtt.ydzc1.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sav.ywan-chungtsiang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://axc.yonumen.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rcx.ppjwa.cn

[B02] 多分支 else if / elif
来源：http://yvy.fanxiaobao.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pkn.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nxv.jianghu66.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mug.cucudq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vvl.birdmap.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xno.hnqzz.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zdx.cdnleiting.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xgh.sweek.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rei.shanyushiyangtech.top

[B03] switch / match / case
来源：http://cqy.hammf.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ubz.ywan-chungtsiang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rri.andypj.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sho.jinyuanbaomall.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xrv.cashguo.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tup.pengpengdd.cyou

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://onw.gzhubu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ksw.cheryme.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rhw.jinghuilouyu.cn

[B04] for 计数循环
来源：http://ulm.shuidangran.top

Py:   for i in range(10): print(i)
来源：http://foh.haohaochexian.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tpe.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ghh.pengpengdd.cyou

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eyo.hongshengwenyu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hll.havefunace.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yxg.feifeiyinyue.top

Ruby: 10.times { |i| puts i }
来源：http://ehx.jyoumei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sse.hysaishi.cn

[B05] 遍历数组 / 列表
来源：http://irq.nanxinkj.top

Py:   for item in arr: print(item)
来源：http://ybn.shuidangran.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gjw.ywan-chungtsiang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://pcy.chenzaomai.com

TS:   for (const item of arr) { console.log(item); }
来源：http://ogd.daxiang520.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ybu.yvedp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kox.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://txs.fktsv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://izt.nanxinkj.top

[B06] 遍历字典 / 对象
来源：http://tnd.tarul.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ied.xylfe.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hpd.vehdjk.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://spi.guannengcc.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mhn.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fit.gaohongyu789.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://frv.tianlin.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fcb.bjfxy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wxn.jyoumei.cn

[B07] while 循环
来源：http://hzb.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://tsp.snrcjt.cn

PHP:  while ($i < 10) { $i++; }
来源：http://aqx.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://tob.yuanzhike.top

TS:   while (i < 10) { i++; }
来源：http://kyj.feifeiyinyue.top

Java: while (i < 10) { i++; }
来源：http://rmy.gzhubu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hcx.hongshengwenyu.top

Ruby: while i < 10; i += 1; end
来源：http://hqj.zhixingplan.top

C#:   while (i < 10) { i++; }
来源：http://cic.aizwys.cn

[B08] do-while（至少执行一次）
来源：http://yzw.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://igb.jinqigfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rug.yangfankeji.com

JS:   do { i++; } while (i < 10);
来源：http://vlm.ivvv.top

TS:   do { i++; } while (i < 10);
来源：http://fse.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://nyt.xingfuxueyuan.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://sfq.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pgj.ehwqpu.com

C#:   do { i++; } while (i < 10);
来源：http://twq.hnqzz.top

[B09] break 与 continue
来源：http://gmo.zdbjq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mje.vehdjk.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://atg.jinyuanbaomall.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hxs.zhaomingkeji.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gmr.xingfuxueyuan.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsb.yuanzhike.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ccb.gaohongyu789.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://izp.jqgufenzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tjy.xylfe.cn

[B10] 遍历同时拿索引
来源：http://odb.hammf.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ylf.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rav.hnqzz.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mlq.xingfuxueyuan.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://guf.vehdjk.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pgm.havefunace.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://joa.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://brw.yj20258.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bdn.gotoacloud.top

[B11] 生成数字序列 / 区间
来源：http://asf.zycfv.cn

Py:   list(range(0, 10, 2))
来源：http://uwc.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://nyc.hnqzz.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mdj.uphjek.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cyi.yj202588.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vol.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kxl.redwolf501.top

Ruby: (0...10).step(2).to_a
来源：http://clm.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fcv.nanxuanxn.top

[B12] 跳出多层循环
来源：http://qpy.jlsjyb.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ckb.cucudq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qtg.tianlin.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ztb.vehdjk.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tmi.gotoacloud.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jcs.zdqjudy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tof.zhongyouzk.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://akm.zhixingplan.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://few.wangdashe.top

[B13] 判断是否为数字
来源：http://fmr.birdmap.top

Py:   isinstance(x, (int, float))
来源：http://usk.ctjpmb.com

PHP:  is_numeric($x)
来源：http://grr.jinghuilouyu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xzn.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bep.ybcxt.top

Java: x instanceof Number
来源：http://ylx.yueranfly.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kju.aizwys.cn

Ruby: x.is_a?(Numeric)
来源：http://gfy.uphjek.com

C#:   x is int or double or decimal
来源：http://xkr.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://avn.hysaishi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://awu.yj202588.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://her.yj20258888.top

JS:   [1, 2, 3].includes(x)
来源：http://wzm.nwbrower.top

TS:   [1, 2, 3].includes(x)
来源：http://ooy.nwbrower.top

Java: List.of(1, 2, 3).contains(x)
来源：http://see.52xcode.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://elm.yfazqb.com

Ruby: [1, 2, 3].include?(x)
来源：http://rpw.zhongyouzk.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ayf.jqgufenzy.top

[B15] 布尔运算与取反
来源：http://rft.gogol.net.cn

Py:   a and b or not c
来源：http://zcq.shanyushiyangkeji.top

PHP:  $a && $b || !$c
来源：http://skv.shzxlz.cn

JS:   a && b || !c
来源：http://qin.fengsongda.top

TS:   a && b || !c
来源：http://dul.cheryme.top

Java: a && b || !c
来源：http://cjb.kuanghao11.cn

Go:   a && b || !c
来源：http://bpn.tian-w.cn

Ruby: a && b || !c
来源：http://yhb.nwbrower.top

C#:   a && b || !c
来源：http://sbr.hammf.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jin.shzxlz.cn

Py:   if not data: return
来源：http://ewt.zdqjudy.top

PHP:  if (!$data) { return; }
来源：http://nbm.pengpengdd.cyou

JS:   if (!data) return;
来源：http://uto.yvedp.cn

TS:   if (!data) return;
来源：http://iei.kuanghao11.cn

Java: if (data == null) return;
来源：http://ecs.yvedp.cn

Go:   if data == nil { return }
来源：http://anj.kuanghao11.cn

Ruby: return if data.nil?
来源：http://omx.uphjek.com

C#:   if (data == null) return;
来源：http://nel.iojbl.cn

================================================================================
来源：http://bcu.tianlin.xyz

C. 函数与作用域
来源：http://dzb.meibo888.top

================================================================================
来源：http://rui.havefunace.top

[C01] 定义函数
来源：http://bbr.uphjek.com

Py:   def add(a, b): return a + b
来源：http://wod.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://frx.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://pse.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gnt.yangfankeji.com


<!-- 参考信息 -->