代发 wailian999

[A14] 注释写法
来源：http://hte.hnxiangtu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://tkl.zdbjq.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://upy.fengsongda.top

JS:   // 单行；/* 多行 */
来源：http://hfp.ywan-chungtsiang.top

TS:   // 单行；/* 多行 */
来源：http://lxe.xingfuxueyuan.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qks.daxiang520.top

Go:   // 单行；/* 多行 */
来源：http://pst.pengpengdd.cyou

Ruby: # 单行；=begin 多行 =end
来源：http://xpk.sxryk.cn

C#:   // 单行；/* 多行 */
来源：http://awp.ydzc1.top

[A15] 空值判断与默认值
来源：http://zgq.bjfxy.top

Py:   value = data or "默认值"
来源：http://jep.cucudq.cn

PHP:  $value = $data ?? "默认值";
来源：http://ikk.shanyushiyangtech.top

JS:   const value = data ?? "默认值";
来源：http://fqy.c1oappe.top

TS:   const value = data ?? "默认值";
来源：http://frc.tianlin.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rpm.yj20258888.top

Go:   if data == "" { data = "默认值" }
来源：http://zsc.dianchejie.cn

Ruby: value = data || "默认值"
来源：http://wnd.xylfe.cn

C#:   var value = data ?? "默认值";
来源：http://cmn.zhongyouzk.top

[A16] 真假值判断规则
来源：http://jbz.jqgfzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gnu.shangyingyoupin.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rgv.chenzaomai.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hta.zdqjudy.top

TS:   if (!x) {}
来源：http://tec.ivvv.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dps.hysaishi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ilq.shuidangran.top

Ruby: unless x            # nil 与 false 为假
来源：http://yhq.haohaochexian.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mdv.aizwys.cn

[A17] 位运算
来源：http://uvi.chenjidiqi.icu

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ybq.bjfxy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rva.ydzc1.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bbs.xingfuxueyuan.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dyn.hnxiangtu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://raa.feifeiyinyue.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pqr.52xcode.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ejn.cheryme.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zup.zhaomingkeji.xyz

[A18] 字符与 ASCII 码互转
来源：http://rlv.jinyuanbaomall.cn

Py:   ord("A"); chr(65)
来源：http://oaj.aizwys.cn

PHP:  ord("A"); chr(65)
来源：http://tbl.9152youxi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://syu.yfazqb.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gsg.zycfv.cn

Java: (int) 'A'; (char) 65
来源：http://vga.zycfv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lmi.fehbvm.com

Ruby: "A".ord; 65.chr
来源：http://maf.0kj1m.cn

C#:   (int)'A'; (char)65
来源：http://wdo.shanyushiyangtech.top

[A19] 交换两个变量
来源：http://pdq.jinyuanbaomall.cn

Py:   a, b = b, a
来源：http://lve.kuanghao11.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://urc.ctjpmb.com

JS:   [a, b] = [b, a];
来源：http://hdo.pycfn.com

TS:   [a, b] = [b, a];
来源：http://zcg.snrcjt.cn

Java: int t = a; a = b; b = t;
来源：http://gbz.zycfv.cn

Go:   a, b = b, a
来源：http://obb.sysykeji.top

Ruby: a, b = b, a
来源：http://ikh.yfazqb.com

C#:   (a, b) = (b, a);
来源：http://tre.vqdsnc.cn

[A20] 读取标准输入
来源：http://ugn.redwolf501.top

Py:   name = input("请输入：")
来源：http://tws.fehbvm.com

PHP:  $name = trim(fgets(STDIN));
来源：http://tum.chenjidiqi.icu

JS:   // Node.js：readline 模块或 process.stdin
来源：http://iyg.havefunace.top

TS:   // Node.js：readline 模块
来源：http://yct.yj20258888.top

Java: new Scanner(System.in).nextLine()
来源：http://ycc.snrcjt.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mna.yj202588.top

Ruby: gets.chomp
来源：http://ffn.chenzaomai.com

C#:   Console.ReadLine();
来源：http://osc.jinghuilouyu.cn

[A21] 保留指定小数位输出
来源：http://iux.bbcook.cn

Py:   f"{3.14159:.2f}"
来源：http://qcw.yvedp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hbe.yj202588.top

JS:   (3.14159).toFixed(2)
来源：http://jwu.nanxinkj.top

TS:   (3.14159).toFixed(2)
来源：http://pfm.nanxinkj.top

Java: String.format("%.2f", 3.14159)
来源：http://qjs.yfazqb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://keu.zdbjq.cn

Ruby: format("%.2f", 3.14159)
来源：http://zgt.52xcode.cn

C#:   3.14159.ToString("F2")
来源：http://oja.snrcjt.cn

[A22] 获取字符串长度
来源：http://upa.mhx1999.top

Py:   len(s)
来源：http://wuj.xinyue.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xat.dianchejie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gsf.bbcook.cn

TS:   s.length
来源：http://rdi.sysykeji.top

Java: s.length()
来源：http://ooo.cqqwz.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wxo.jianghu66.top

Ruby: s.length
来源：http://tkv.quarkkingdee.top

C#:   s.Length
来源：http://dic.xingfuxueyuan.xyz

[A23] 大小写转换
来源：http://nxm.nanxuanxn.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wes.aibaodan.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bpl.aizwys.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kjy.zhaomingkeji.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tby.smart0.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yrh.dashuyun.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://krp.haohaochexian.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zjv.daria6918.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://smf.zhijiandao.cn

[A24] 去除首尾空白
来源：http://dge.tarul.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://agt.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zcn.andypj.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qjr.chenlongwang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ohh.dianchejie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://odg.yvedp.cn

Go:   strings.TrimSpace(s)
来源：http://mxt.tianlin.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dwx.hcnkem.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nkk.xinyue.icu

[A25] 字符串比较
来源：http://efq.haohaochexian.top

Py:   s1 == s2; s1 != s2
来源：http://hhw.gotoacloud.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uaf.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wem.haohaochexian.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://coe.ydjk.org.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nbc.meibo888.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pvx.yueranfly.top

Ruby: s1 == s2; s1 <=> s2
来源：http://chk.wangshuangyany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fqi.hysaishi.cn

[A26] 类型转换总览
来源：http://fog.xinyue.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iyd.ydjk.org.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vyp.hnxiangtu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gqc.pengpengdd.cyou

TS:   Number() String() Boolean() x as number
来源：http://wdz.xylfe.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uxw.ppjwa.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yoe.shuidangran.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qga.mhx1999.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fqb.kuanghao11.cn

================================================================================
来源：http://zln.jinghuilouyu.cn

B. 流程控制
来源：http://vur.smart0.xyz

================================================================================
来源：http://pwl.iojbl.cn

[B01] 条件判断 if / else
来源：http://lgs.quarkkingdee.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jch.gaohongyu789.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yeg.yj202588.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sfi.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pxa.ydjk.org.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uvo.cqqwz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yvi.yuanzhike.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jhf.yangfankeji.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jof.ywan-chungtsiang.top

[B02] 多分支 else if / elif
来源：http://eze.zhiwuduotai.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mgx.zhaomingkeji.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://akt.jqgufenzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tbl.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zln.haohaochexian.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lsu.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nuq.hfpthk.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wnd.gotoacloud.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tyj.jinghuilouyu.cn

[B03] switch / match / case
来源：http://sbj.gaohongyu789.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wcy.gotoacloud.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ipd.yongpay.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hmi.havefunace.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wkv.nwbrower.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xel.zhiwuduotai.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fhh.tanke756.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://six.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xzl.nanxinkj.top

[B04] for 计数循环
来源：http://erx.yj202588.top

Py:   for i in range(10): print(i)
来源：http://hfz.bbcook.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hmf.hywenlv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vzr.quarkkingdee.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ijv.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rml.cheryme.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zss.sjlbkw.cn

Ruby: 10.times { |i| puts i }
来源：http://zhy.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gks.zhijiandao.cn

[B05] 遍历数组 / 列表
来源：http://kkx.hfpthk.cn

Py:   for item in arr: print(item)
来源：http://mul.sxryk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jqq.zdqjudy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rkw.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ves.jianghu66.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fhg.shangyingyoupin.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ajn.zhaomingkeji.xyz

Ruby: arr.each { |item| puts item }
来源：http://fdx.52xcode.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qfc.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://vuo.cashguo.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uiu.nanxuanxn.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cbu.jqgufenzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rxi.gotoacloud.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nxi.zhiwuduotai.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rft.havefunace.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fyw.hongshengwenyu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wkh.xingfuxueyuan.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nfz.andypj.xyz

[B07] while 循环
来源：http://ifm.ydzc1.top

Py:   while i < 10: i += 1
来源：http://slo.gogol.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://shj.fanxiaobao.xyz

JS:   while (i < 10) { i++; }
来源：http://lwm.52xcode.cn

TS:   while (i < 10) { i++; }
来源：http://dmi.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://izq.wangdashe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uve.nwbrower.top

Ruby: while i < 10; i += 1; end
来源：http://znh.smart0.xyz

C#:   while (i < 10) { i++; }
来源：http://tpx.jlsjyb.cn

[B08] do-while（至少执行一次）
来源：http://cdz.hysaishi.cn

Py:   # 无 do-while：用 while True + break
来源：http://fwa.sysykeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qlk.redwolf501.top

JS:   do { i++; } while (i < 10);
来源：http://jyl.jiagoushi.top

TS:   do { i++; } while (i < 10);
来源：http://wjo.daria6918.cn

Java: do { i++; } while (i < 10);
来源：http://gpg.tarul.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jsn.sxryk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dsp.ppjwa.cn

C#:   do { i++; } while (i < 10);
来源：http://ych.gaohongyu789.top

[B09] break 与 continue
来源：http://gnm.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fvc.sufxvd.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://axz.yvedp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xek.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gzt.fengsongda.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://owi.zdbjq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://acr.cqqwz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xzy.chenlongwang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://svw.cheryme.top

[B10] 遍历同时拿索引
来源：http://dym.hfpthk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bow.mhx1999.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dsi.feifeiyinyue.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jna.nwbrower.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jkk.c1oappe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qwl.xziqi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://amx.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://psa.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qmn.cucudq.cn

[B11] 生成数字序列 / 区间
来源：http://nqq.shanyushiyangtech.top

Py:   list(range(0, 10, 2))
来源：http://jol.hfpthk.cn

PHP:  range(0, 10, 2);
来源：http://seo.sweek.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wnr.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lyk.hongshengwenyu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ffa.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hca.52xcode.cn

Ruby: (0...10).step(2).to_a
来源：http://bms.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uny.tanke756.top

[B12] 跳出多层循环
来源：http://ihu.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nmb.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ejj.jqgufenzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zdc.cucudq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rpz.jinghuilouyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://heq.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fvn.yj20258888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ade.sysykeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lnb.9152youxi.cn

[B13] 判断是否为数字
来源：http://ntt.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://uif.tian-w.cn

PHP:  is_numeric($x)
来源：http://ldz.yangfankeji.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bxe.yongpay.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vrk.sysykeji.top

Java: x instanceof Number
来源：http://rca.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gts.zhoulong.xyz

Ruby: x.is_a?(Numeric)
来源：http://xyc.jianghu66.top

C#:   x is int or double or decimal
来源：http://sgt.hesvh.cn

[B14] 判断值是否在集合内
来源：http://uvx.xingfuxueyuan.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wye.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fdq.chenzaomai.com

JS:   [1, 2, 3].includes(x)
来源：http://ssi.yj202588.top

TS:   [1, 2, 3].includes(x)
来源：http://wos.vqdsnc.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ujq.jinghuilouyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pgb.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xne.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qxj.nanxinkj.top

[B15] 布尔运算与取反
来源：http://etd.quarkkingdee.top

Py:   a and b or not c
来源：http://smh.shangyingyoupin.top

PHP:  $a && $b || !$c
来源：http://upz.ywan-chungtsiang.top

JS:   a && b || !c
来源：http://waw.meibo888.top

TS:   a && b || !c
来源：http://zzh.hfpthk.cn

Java: a && b || !c
来源：http://ziq.birdmap.top

Go:   a && b || !c
来源：http://azp.guowangkeji.top

Ruby: a && b || !c
来源：http://swp.xylfe.cn

C#:   a && b || !c
来源：http://jai.pengpengdd.cyou

[B16] 卫语句：不满足条件提前返回
来源：http://sjq.shanyushiyangtech.top

Py:   if not data: return
来源：http://czv.guowangkeji.top

PHP:  if (!$data) { return; }
来源：http://cms.xuetiantiany.cn

JS:   if (!data) return;
来源：http://uij.chenzaomai.com

TS:   if (!data) return;
来源：http://zbd.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://mrk.ydjk.org.cn

Go:   if data == nil { return }
来源：http://fym.andypj.xyz

Ruby: return if data.nil?
来源：http://ahy.tanke756.top

C#:   if (data == null) return;
来源：http://qbp.zhongyouzk.top

================================================================================
来源：http://ejk.fktsv.cn

C. 函数与作用域
来源：http://uwy.yonumen.top

================================================================================
来源：http://dqd.ctjpmb.com

[C01] 定义函数
来源：http://fay.yonumen.top

Py:   def add(a, b): return a + b
来源：http://gtp.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://isr.sjlbkw.cn

JS:   function add(a, b) { return a + b; }
来源：http://ayn.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ocu.yueranfly.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dyf.redwolf501.top

Go:   func add(a, b int) int { return a + b }
来源：http://oja.0kj1m.cn

Ruby: def add(a, b); a + b; end
来源：http://ckw.cheryme.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://isb.xylfe.cn

[C02] 默认参数
来源：http://wte.yuxming.cn

Py:   def greet(name="World"): return name
来源：http://pln.jinghuilouyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tno.hongshengwenyu.top

JS:   function greet(name = "World") { return name; }
来源：http://aed.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mhh.sysykeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kli.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wna.fzhhl.top

Ruby: def greet(name = "World") = name
来源：http://bbt.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://isd.zhiwuduotai.top

[C03] 可变参数
来源：http://oep.zhixingplan.top

Py:   def total(*args): return sum(args)
来源：http://nlk.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nhl.shuidangran.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rrx.yanxiufei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nuw.sysykeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ssk.tarul.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pdt.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://dzx.jinqigufen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iwb.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://vhi.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aqf.xinyue.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pwg.svipenyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zom.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mnc.9152youxi.cn

Java: // 无：用 Builder 模式或 record
来源：http://tdx.birdmap.top


<!-- 参考信息 -->