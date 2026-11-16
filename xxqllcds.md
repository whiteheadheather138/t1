代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wdm.yj20258.top

JS:   `Hello, ${name}!`
来源：http://omd.yanxiufei.cn

TS:   `Hello, ${name}!`
来源：http://kef.fzhhl.top

Java: "Hello, %s!".formatted(name)
来源：http://upx.jinyuanbaomall.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cwt.tarul.cn

Ruby: "Hello, #{name}!"
来源：http://xci.iojbl.cn

C#:   $"Hello, {name}!"
来源：http://bsi.pycfn.com

[A13] 多行字符串（练习 \n 转义）
来源：http://afq.jinqigfzy.top

Py:   "第一行\n第二行"
来源：http://lxv.zhiwuduotai.top

PHP:  "第一行\n第二行"
来源：http://ilb.hnqzz.top

JS:   "第一行\n第二行"
来源：http://wtv.jinghuilouyu.cn

TS:   "第一行\n第二行"
来源：http://sbh.feifeiyinyue.top

Java: "第一行\n第二行"
来源：http://uos.aizwys.cn

Go:   "第一行\n第二行"
来源：http://wlp.epnwcf.com

Ruby: "第一行\n第二行"
来源：http://zri.wangshuangyany.cn

C#:   "第一行\n第二行"
来源：http://sye.yueranfly.top

[A14] 注释写法
来源：http://hvx.wangshuangyany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wqu.hongshengwenyu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://eor.dashuyun.cn

JS:   // 单行；/* 多行 */
来源：http://fgf.hnxiangtu.top

TS:   // 单行；/* 多行 */
来源：http://qgz.cdnleiting.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lwr.guannengcc.top

Go:   // 单行；/* 多行 */
来源：http://ksh.svipenyu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rmc.jianghu66.top

C#:   // 单行；/* 多行 */
来源：http://goa.pycfn.com

[A15] 空值判断与默认值
来源：http://xcw.yanxiufei.cn

Py:   value = data or "默认值"
来源：http://pmy.dashuyun.cn

PHP:  $value = $data ?? "默认值";
来源：http://obb.0kj1m.cn

JS:   const value = data ?? "默认值";
来源：http://vhm.ydjk.org.cn

TS:   const value = data ?? "默认值";
来源：http://yek.cqqwz.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://huq.tanke756.top

Go:   if data == "" { data = "默认值" }
来源：http://koq.vqdsnc.cn

Ruby: value = data || "默认值"
来源：http://ytu.hcnkem.com

C#:   var value = data ?? "默认值";
来源：http://cvl.zhongyouzk.top

[A16] 真假值判断规则
来源：http://djq.jinyuanbaomall.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://puc.tanke756.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://meu.tarul.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lrp.yongpay.top

TS:   if (!x) {}
来源：http://hmn.sxryk.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yzq.yuanzhike.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zru.yueranfly.top

Ruby: unless x            # nil 与 false 为假
来源：http://klm.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bkk.yvedp.cn

[A17] 位运算
来源：http://qem.xylfe.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aan.guowangkeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tbu.gotoacloud.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fbm.jinghuilouyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mgl.hammf.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qsl.jqgufenzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jgb.jinyuanbaomall.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hxg.aibaodan.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ppu.zhongyouzk.top

[A18] 字符与 ASCII 码互转
来源：http://nuu.yvedp.cn

Py:   ord("A"); chr(65)
来源：http://ulj.smart0.xyz

PHP:  ord("A"); chr(65)
来源：http://ilw.hnqzz.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ews.cucudq.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zva.andypj.xyz

Java: (int) 'A'; (char) 65
来源：http://hpy.jqgufenzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://auw.snrcjt.cn

Ruby: "A".ord; 65.chr
来源：http://tcp.fehbvm.com

C#:   (int)'A'; (char)65
来源：http://pda.c1oappe.top

[A19] 交换两个变量
来源：http://xdn.c1oappe.top

Py:   a, b = b, a
来源：http://yhi.gogol.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xkl.fengsongda.top

JS:   [a, b] = [b, a];
来源：http://txd.nanxuanxn.top

TS:   [a, b] = [b, a];
来源：http://sph.tianlin.xyz

Java: int t = a; a = b; b = t;
来源：http://kii.chenjidiqi.icu

Go:   a, b = b, a
来源：http://wyc.hysaishi.cn

Ruby: a, b = b, a
来源：http://eib.cucudq.cn

C#:   (a, b) = (b, a);
来源：http://wek.epnwcf.com

[A20] 读取标准输入
来源：http://wav.havefunace.top

Py:   name = input("请输入：")
来源：http://iat.xylfe.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cri.zhixingplan.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://brq.xziqi.cn

TS:   // Node.js：readline 模块
来源：http://imd.yonumen.top

Java: new Scanner(System.in).nextLine()
来源：http://src.cheryme.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mmc.cdnleiting.top

Ruby: gets.chomp
来源：http://ztb.ywan-chungtsiang.top

C#:   Console.ReadLine();
来源：http://kaq.svipenyu.cn

[A21] 保留指定小数位输出
来源：http://hui.hfpthk.cn

Py:   f"{3.14159:.2f}"
来源：http://ofq.snrcjt.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fcn.gotoacloud.top

JS:   (3.14159).toFixed(2)
来源：http://iwy.yongpay.top

TS:   (3.14159).toFixed(2)
来源：http://hap.jinqigfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://igw.svipenyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xnt.52xcode.cn

Ruby: format("%.2f", 3.14159)
来源：http://qtt.tarul.cn

C#:   3.14159.ToString("F2")
来源：http://zoo.316326.xyz

[A22] 获取字符串长度
来源：http://qbo.zdqjudy.top

Py:   len(s)
来源：http://kaj.cashguo.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ftf.chenzaomai.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uox.shanyushiyangkeji.top

TS:   s.length
来源：http://wxe.jqgufenzy.top

Java: s.length()
来源：http://mdt.cqqwz.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qfk.yongpay.top

Ruby: s.length
来源：http://ydh.havefunace.top

C#:   s.Length
来源：http://zgv.mhx1999.top

[A23] 大小写转换
来源：http://geh.yj20258.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vvf.xuanzx.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qov.hammf.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jsj.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://axx.hcnkem.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bix.redwolf501.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vrl.yj202588.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ten.cashguo.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gar.hesvh.cn

[A24] 去除首尾空白
来源：http://tjo.haohaochexian.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jsb.birdmap.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mti.yongpay.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rqf.shzxlz.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uth.svipenyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rsm.0kj1m.cn

Go:   strings.TrimSpace(s)
来源：http://czp.xingfuxueyuan.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://exk.sjlbkw.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nbd.xziqi.cn

[A25] 字符串比较
来源：http://plg.jinqigfzy.top

Py:   s1 == s2; s1 != s2
来源：http://qsh.daxiang520.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dhd.ywan-chungtsiang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xzq.jinqigfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://crr.gogol.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://txp.jqgfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uhx.ppjwa.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lgc.xylfe.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ppk.zhoulong.xyz

[A26] 类型转换总览
来源：http://shf.hywenlv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://acb.hywenlv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nqc.bjfxy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zna.jinyuanbaomall.cn

TS:   Number() String() Boolean() x as number
来源：http://qct.wangshuangyany.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nqj.tianlin.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tfa.gotoacloud.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wec.hongshengwenyu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bcm.fanxiaobao.xyz

================================================================================
来源：http://gvj.ydzc1.top

B. 流程控制
来源：http://gmf.hywenlv.cn

================================================================================
来源：http://rma.feifeiyinyue.top

[B01] 条件判断 if / else
来源：http://gri.vehdjk.com

Py:   result = "正" if x > 0 else "非正"
来源：http://lky.chenzaomai.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://faw.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wau.yfazqb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zuz.jinqigfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://kju.vehdjk.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ogk.fengsongda.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://csf.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uwu.chenzaomai.com

[B02] 多分支 else if / elif
来源：http://vor.hfpthk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kfo.yonumen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gex.yfazqb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sya.meibo888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ymx.yuanzhike.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xju.yuxming.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nfp.birdmap.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wbd.ppjwa.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zdu.jinghuilouyu.cn

[B03] switch / match / case
来源：http://vji.cdnleiting.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aml.xylfe.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kdn.snrcjt.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://czj.yangfankeji.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uds.shzxlz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lvt.xingfuxueyuan.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xkj.nanxinkj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rku.c1oappe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gvi.shangyingyoupin.top

[B04] for 计数循环
来源：http://zla.sufxvd.cn

Py:   for i in range(10): print(i)
来源：http://lat.hnqzz.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iez.mhx1999.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gcq.cucudq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zml.quarkkingdee.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://djw.shangyingyoupin.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ych.fengsongda.top

Ruby: 10.times { |i| puts i }
来源：http://tdw.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gwm.jinghuilouyu.cn

[B05] 遍历数组 / 列表
来源：http://nrf.fzhhl.top

Py:   for item in arr: print(item)
来源：http://ken.ywan-chungtsiang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xwo.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bha.zhixingplan.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cbs.gaohongyu789.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fvr.chenjidiqi.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sqc.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://wym.cashguo.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wut.xuetiantiany.cn

[B06] 遍历字典 / 对象
来源：http://nsg.zhengqikj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ocd.dashuyun.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gbz.316326.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ltr.aizwys.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://caz.xziqi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ltp.snrcjt.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pqq.hywenlv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mhd.ydjk.org.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ygt.hfpthk.cn

[B07] while 循环
来源：http://klu.vehdjk.com

Py:   while i < 10: i += 1
来源：http://kpa.hysaishi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tva.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://fzh.hfpthk.cn

TS:   while (i < 10) { i++; }
来源：http://oas.jianghu66.top

Java: while (i < 10) { i++; }
来源：http://fqv.ydjk.org.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uti.aibaodan.cn

Ruby: while i < 10; i += 1; end
来源：http://mtw.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://yci.fktsv.cn

[B08] do-while（至少执行一次）
来源：http://iim.chenjidiqi.icu

Py:   # 无 do-while：用 while True + break
来源：http://dvy.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vna.c1oappe.top

JS:   do { i++; } while (i < 10);
来源：http://ylj.yueranfly.top

TS:   do { i++; } while (i < 10);
来源：http://msx.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://spr.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://vjz.yuxming.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xhf.zhengqikj.top

C#:   do { i++; } while (i < 10);
来源：http://cyp.zycfv.cn

[B09] break 与 continue
来源：http://luo.yongpay.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fgt.ctjpmb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://amv.yongpay.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oif.tianlin.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ulr.jlsjyb.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jud.vehdjk.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://slz.yj20258888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gra.xziqi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wll.zdbjq.cn

[B10] 遍历同时拿索引
来源：http://law.zhijiandao.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bor.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jqb.ydjk.org.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lbv.haohaochexian.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wdz.fengsongda.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tgr.wangdashe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://opo.jqgfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://scw.hysaishi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pfm.gogol.net.cn

[B11] 生成数字序列 / 区间
来源：http://acm.c1oappe.top

Py:   list(range(0, 10, 2))
来源：http://sfg.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://mad.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dny.yonumen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pjd.sweek.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rnn.fzhhl.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wnn.fzhhl.top

Ruby: (0...10).step(2).to_a
来源：http://wik.hysaishi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lnl.wangshuangyany.cn

[B12] 跳出多层循环
来源：http://xws.tian-w.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://daz.zhixingplan.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yfw.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ink.hywenlv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wbb.jinqigfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rtx.hesvh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pti.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yto.fengsongda.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mpg.xuetiantiany.cn

[B13] 判断是否为数字
来源：http://zup.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://yzc.yvedp.cn

PHP:  is_numeric($x)
来源：http://vfx.sysykeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fky.svipenyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nii.ehwqpu.com

Java: x instanceof Number
来源：http://wuf.xziqi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gfj.yuanzhike.top

Ruby: x.is_a?(Numeric)
来源：http://qqv.jinghuilouyu.cn

C#:   x is int or double or decimal
来源：http://aik.ybcxt.top

[B14] 判断值是否在集合内
来源：http://sap.bbcook.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dbt.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kcb.hesvh.cn

JS:   [1, 2, 3].includes(x)
来源：http://trk.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://jyp.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mmh.yanxiufei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bhp.52xcode.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mwp.fanxiaobao.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kuo.ybcxt.top

[B15] 布尔运算与取反
来源：http://hzt.hfpthk.cn

Py:   a and b or not c
来源：http://zkr.hcnkem.com

PHP:  $a && $b || !$c
来源：http://nqx.yuanzhike.top

JS:   a && b || !c
来源：http://rjx.bjfxy.top

TS:   a && b || !c
来源：http://jyu.gogol.net.cn

Java: a && b || !c
来源：http://lph.ctjpmb.com

Go:   a && b || !c
来源：http://ifn.0kj1m.cn

Ruby: a && b || !c
来源：http://oml.hywenlv.cn

C#:   a && b || !c
来源：http://xwn.shanyushiyangtech.top

[B16] 卫语句：不满足条件提前返回
来源：http://dno.jyoumei.cn

Py:   if not data: return
来源：http://oda.meibo888.top

PHP:  if (!$data) { return; }
来源：http://aye.vehdjk.com

JS:   if (!data) return;
来源：http://zig.fengsongda.top

TS:   if (!data) return;
来源：http://oon.andypj.xyz

Java: if (data == null) return;
来源：http://dxc.hnqzz.top

Go:   if data == nil { return }
来源：http://rzx.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://ukp.dashuyun.cn

C#:   if (data == null) return;
来源：http://icq.bjfxy.top

================================================================================
来源：http://cek.pengpengdd.cyou

C. 函数与作用域
来源：http://zvq.nwbrower.top

================================================================================
来源：http://adn.ywan-chungtsiang.top

[C01] 定义函数
来源：http://fyi.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://hhy.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://skg.jinghuilouyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://kwz.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://abf.ppjwa.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ftb.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hgf.tarul.cn

Ruby: def add(a, b); a + b; end
来源：http://kbf.zhoulong.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uaa.ywan-chungtsiang.top

[C02] 默认参数
来源：http://xmr.cucudq.cn

Py:   def greet(name="World"): return name
来源：http://zkv.fanxiaobao.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://yix.sxryk.cn

JS:   function greet(name = "World") { return name; }
来源：http://ylq.c1oappe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lsd.nwbrower.top

Java: // 无默认参数：方法重载或 Optional
来源：http://yyh.aizwys.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ews.jlsjyb.cn

Ruby: def greet(name = "World") = name
来源：http://lbg.fehbvm.com


<!-- 参考信息 -->