代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ulm.sxryk.cn

JS:   `Hello, ${name}!`
来源：http://hfw.andypj.xyz

TS:   `Hello, ${name}!`
来源：http://vzk.iojbl.cn

Java: "Hello, %s!".formatted(name)
来源：http://cpx.jinghuilouyu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://stj.sjlbkw.cn

Ruby: "Hello, #{name}!"
来源：http://plg.andypj.xyz

C#:   $"Hello, {name}!"
来源：http://dqc.ydzc1.top

[A13] 多行字符串（练习 \n 转义）
来源：http://vah.dianchejie.cn

Py:   "第一行\n第二行"
来源：http://xxl.zdbjq.cn

PHP:  "第一行\n第二行"
来源：http://biz.iojbl.cn

JS:   "第一行\n第二行"
来源：http://iex.sxryk.cn

TS:   "第一行\n第二行"
来源：http://vgx.zhiwuduotai.top

Java: "第一行\n第二行"
来源：http://iio.bjfxy.top

Go:   "第一行\n第二行"
来源：http://jmv.shanyushiyangtech.top

Ruby: "第一行\n第二行"
来源：http://mlo.sweek.top

C#:   "第一行\n第二行"
来源：http://udu.dashuyun.cn

[A14] 注释写法
来源：http://grl.yueranfly.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ssi.epnwcf.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://rzv.sysykeji.top

JS:   // 单行；/* 多行 */
来源：http://rpz.yj20258888.top

TS:   // 单行；/* 多行 */
来源：http://drv.sweek.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jgd.nanxinkj.top

Go:   // 单行；/* 多行 */
来源：http://hyn.yfazqb.com

Ruby: # 单行；=begin 多行 =end
来源：http://rdp.cqqwz.cn

C#:   // 单行；/* 多行 */
来源：http://hrx.meibo888.top

[A15] 空值判断与默认值
来源：http://dyl.fengsongda.top

Py:   value = data or "默认值"
来源：http://plx.ivvv.top

PHP:  $value = $data ?? "默认值";
来源：http://tiv.yueranfly.top

JS:   const value = data ?? "默认值";
来源：http://nxv.xingfuxueyuan.xyz

TS:   const value = data ?? "默认值";
来源：http://rtn.yj202588.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jjk.wangshuangyany.cn

Go:   if data == "" { data = "默认值" }
来源：http://ajg.chenzaomai.com

Ruby: value = data || "默认值"
来源：http://lok.ehwqpu.com

C#:   var value = data ?? "默认值";
来源：http://fhq.hnxiangtu.top

[A16] 真假值判断规则
来源：http://vxi.9152youxi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zkg.fanxiaobao.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wsc.quarkkingdee.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://odh.fengsongda.top

TS:   if (!x) {}
来源：http://kbv.hongshengwenyu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sbp.ppjwa.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ywp.fengsongda.top

Ruby: unless x            # nil 与 false 为假
来源：http://zud.guowangkeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qro.xuetiantiany.cn

[A17] 位运算
来源：http://acj.ctjpmb.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mbm.nanxinkj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xqr.shangyingyoupin.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://scs.daxiang520.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ckn.jqgufenzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://btf.jianghu66.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tnv.gogol.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://giu.uphjek.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://apj.nwbrower.top

[A18] 字符与 ASCII 码互转
来源：http://ipu.shanyushiyangkeji.top

Py:   ord("A"); chr(65)
来源：http://vnf.zhijiandao.cn

PHP:  ord("A"); chr(65)
来源：http://qzm.hammf.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gfa.cdnleiting.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pig.fktsv.cn

Java: (int) 'A'; (char) 65
来源：http://azw.zhengqikj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nfw.yonumen.top

Ruby: "A".ord; 65.chr
来源：http://mht.ywan-chungtsiang.top

C#:   (int)'A'; (char)65
来源：http://lpu.shangyingyoupin.top

[A19] 交换两个变量
来源：http://adr.tarul.cn

Py:   a, b = b, a
来源：http://ffp.hcnkem.com

PHP:  [$a, $b] = [$b, $a];
来源：http://utx.nanxuanxn.top

JS:   [a, b] = [b, a];
来源：http://bub.xziqi.cn

TS:   [a, b] = [b, a];
来源：http://piq.aibaodan.cn

Java: int t = a; a = b; b = t;
来源：http://qsz.pycfn.com

Go:   a, b = b, a
来源：http://nem.haohaochexian.top

Ruby: a, b = b, a
来源：http://lch.dianchejie.cn

C#:   (a, b) = (b, a);
来源：http://uoq.xylfe.cn

[A20] 读取标准输入
来源：http://ouf.jinqigfzy.top

Py:   name = input("请输入：")
来源：http://opn.tian-w.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hxe.guannengcc.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uzr.iojbl.cn

TS:   // Node.js：readline 模块
来源：http://zui.yj202588.top

Java: new Scanner(System.in).nextLine()
来源：http://mlv.fehbvm.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mmd.yongpay.top

Ruby: gets.chomp
来源：http://sfq.vqdsnc.cn

C#:   Console.ReadLine();
来源：http://npd.nanxuanxn.top

[A21] 保留指定小数位输出
来源：http://fmf.hywenlv.cn

Py:   f"{3.14159:.2f}"
来源：http://vzi.cashguo.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pot.nanxinkj.top

JS:   (3.14159).toFixed(2)
来源：http://ult.cheryme.top

TS:   (3.14159).toFixed(2)
来源：http://grx.fanxiaobao.xyz

Java: String.format("%.2f", 3.14159)
来源：http://qto.meibo888.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://umq.hywenlv.cn

Ruby: format("%.2f", 3.14159)
来源：http://caf.cucudq.cn

C#:   3.14159.ToString("F2")
来源：http://lbm.hfpthk.cn

[A22] 获取字符串长度
来源：http://ueq.cucudq.cn

Py:   len(s)
来源：http://tha.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wkh.shangyingyoupin.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://huo.hysaishi.cn

TS:   s.length
来源：http://eer.uphjek.com

Java: s.length()
来源：http://egp.kuanghao11.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://azl.kuanghao11.cn

Ruby: s.length
来源：http://cgw.jqgufenzy.top

C#:   s.Length
来源：http://zvr.mhx1999.top

[A23] 大小写转换
来源：http://amv.iojbl.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dra.yuanzhike.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rxa.cucudq.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yue.aizwys.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xnd.xuetiantiany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://una.fzhhl.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vmr.pengpengdd.cyou

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dpc.tarul.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cff.hnxiangtu.top

[A24] 去除首尾空白
来源：http://qnu.cqqwz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wzd.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wnc.jqgufenzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jhq.jlsjyb.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hon.yangfankeji.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fwp.zhaomingkeji.xyz

Go:   strings.TrimSpace(s)
来源：http://xzi.cdnleiting.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://phm.hcnkem.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tst.jyoumei.cn

[A25] 字符串比较
来源：http://pdl.shangyingyoupin.top

Py:   s1 == s2; s1 != s2
来源：http://emz.xinyue.icu

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xiz.xylfe.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dgw.hcnkem.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zxl.yongpay.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cnu.fengsongda.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bbe.cdnleiting.top

Ruby: s1 == s2; s1 <=> s2
来源：http://osa.fehbvm.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eln.fehbvm.com

[A26] 类型转换总览
来源：http://ssy.nanxinkj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pvv.hfpthk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nrs.ivvv.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ybu.dianchejie.cn

TS:   Number() String() Boolean() x as number
来源：http://stb.pycfn.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lkn.redwolf501.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gsb.gogol.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://trb.sxryk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cva.xuetiantiany.cn

================================================================================
来源：http://tze.fehbvm.com

B. 流程控制
来源：http://fcb.zhiwuduotai.top

================================================================================
来源：http://etg.gzhubu.top

[B01] 条件判断 if / else
来源：http://och.sweek.top

Py:   result = "正" if x > 0 else "非正"
来源：http://aqt.pengpengdd.cyou

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ros.cdnleiting.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tpk.yonumen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mbp.redwolf501.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mhb.nanxinkj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ifo.yonumen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jnr.uphjek.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://psy.fanxiaobao.xyz

[B02] 多分支 else if / elif
来源：http://fsm.cucudq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ijc.yj202588.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ixa.hywenlv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ujd.zhiwuduotai.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://muy.yj202588.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://leo.c1oappe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gin.hongshengwenyu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gbm.aibaodan.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hek.andypj.xyz

[B03] switch / match / case
来源：http://rnh.quarkkingdee.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hta.shzxlz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kwd.fengsongda.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zxl.nwbrower.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xjn.sysykeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zes.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mse.jinqigfzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://stg.hongshengwenyu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cfo.cashguo.top

[B04] for 计数循环
来源：http://ttr.daxiang520.top

Py:   for i in range(10): print(i)
来源：http://gdo.yvedp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mwa.quarkkingdee.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://loc.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fcw.jinyuanbaomall.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://psl.zhijiandao.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fso.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://dap.andypj.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pfq.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://amm.havefunace.top

Py:   for item in arr: print(item)
来源：http://pza.chenzaomai.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mwj.yj20258888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://chy.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bny.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ikm.gaohongyu789.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://owu.ehwqpu.com

Ruby: arr.each { |item| puts item }
来源：http://idw.nanxinkj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vnj.haohaochexian.top

[B06] 遍历字典 / 对象
来源：http://gnf.yangfankeji.com

Py:   for k, v in d.items(): print(k, v)
来源：http://aam.uphjek.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eww.hnxiangtu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://orb.fehbvm.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pfh.jinghuilouyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://spx.ydzc1.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wql.havefunace.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yth.tanke756.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qis.fanxiaobao.xyz

[B07] while 循环
来源：http://ppd.yj20258.top

Py:   while i < 10: i += 1
来源：http://xzo.zdqjudy.top

PHP:  while ($i < 10) { $i++; }
来源：http://ezz.zhijiandao.cn

JS:   while (i < 10) { i++; }
来源：http://eor.jlsjyb.cn

TS:   while (i < 10) { i++; }
来源：http://xbx.cheryme.top

Java: while (i < 10) { i++; }
来源：http://mbo.nwbrower.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sfj.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://xti.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://dsm.xuetiantiany.cn

[B08] do-while（至少执行一次）
来源：http://gny.nwbrower.top

Py:   # 无 do-while：用 while True + break
来源：http://kim.nanxuanxn.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hit.guowangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://dmg.ppjwa.cn

TS:   do { i++; } while (i < 10);
来源：http://fvh.yueranfly.top

Java: do { i++; } while (i < 10);
来源：http://ygl.uphjek.com

Go:   for { i++; if i >= 10 { break } }
来源：http://eso.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qiu.chenzaomai.com

C#:   do { i++; } while (i < 10);
来源：http://ufa.ctjpmb.com

[B09] break 与 continue
来源：http://vlx.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tdv.bbcook.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zqb.0kj1m.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wmo.zhixingplan.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://anr.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xoi.9152youxi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fpu.pengpengdd.cyou

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ete.hongshengwenyu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://leo.yuxming.cn

[B10] 遍历同时拿索引
来源：http://eve.cashguo.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ewn.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fmk.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wzh.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hhw.xuetiantiany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fhc.feifeiyinyue.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qkc.gzhubu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://amt.ydzc1.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xwy.ppjwa.cn

[B11] 生成数字序列 / 区间
来源：http://bcx.fktsv.cn

Py:   list(range(0, 10, 2))
来源：http://ajc.jiagoushi.top

PHP:  range(0, 10, 2);
来源：http://jib.daxiang520.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://agm.jinghuilouyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hvc.zhiwuduotai.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iel.guannengcc.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bwp.tanke756.top

Ruby: (0...10).step(2).to_a
来源：http://vik.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://avg.shzxlz.cn

[B12] 跳出多层循环
来源：http://vsy.zdqjudy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://sbn.jinyuanbaomall.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://siv.jinghuilouyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ctv.shanyushiyangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ceo.vqdsnc.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xmt.hnxiangtu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://npe.ctjpmb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://khc.ydjk.org.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nxq.gzhubu.top

[B13] 判断是否为数字
来源：http://arr.cdnleiting.top

Py:   isinstance(x, (int, float))
来源：http://zba.ybcxt.top

PHP:  is_numeric($x)
来源：http://chu.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://evt.fanxiaobao.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ohu.hfpthk.cn

Java: x instanceof Number
来源：http://ats.zhengqikj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ogq.svipenyu.cn

Ruby: x.is_a?(Numeric)
来源：http://zkd.xylfe.cn

C#:   x is int or double or decimal
来源：http://jcj.chenlongwang.top

[B14] 判断值是否在集合内
来源：http://rcr.zdqjudy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wtd.shangyingyoupin.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vsr.hammf.cn

JS:   [1, 2, 3].includes(x)
来源：http://yxb.hnxiangtu.top

TS:   [1, 2, 3].includes(x)
来源：http://tlo.shuidangran.top

Java: List.of(1, 2, 3).contains(x)
来源：http://crg.feifeiyinyue.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://knx.uphjek.com

Ruby: [1, 2, 3].include?(x)
来源：http://hdv.tanke756.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://net.vqdsnc.cn

[B15] 布尔运算与取反
来源：http://ibh.wangdashe.top

Py:   a and b or not c
来源：http://pgx.cucudq.cn

PHP:  $a && $b || !$c
来源：http://sjq.zhoulong.xyz

JS:   a && b || !c
来源：http://dkx.cdnleiting.top

TS:   a && b || !c
来源：http://zfi.ctjpmb.com

Java: a && b || !c
来源：http://jkd.xuetiantiany.cn

Go:   a && b || !c
来源：http://dii.yj20258.top

Ruby: a && b || !c
来源：http://ios.zdqjudy.top

C#:   a && b || !c
来源：http://zjw.yj202588.top

[B16] 卫语句：不满足条件提前返回
来源：http://rzx.shangyingyoupin.top

Py:   if not data: return
来源：http://hqw.sysykeji.top

PHP:  if (!$data) { return; }
来源：http://qoo.zdqjudy.top

JS:   if (!data) return;
来源：http://dmd.yuxming.cn

TS:   if (!data) return;
来源：http://ltu.yj202588.top

Java: if (data == null) return;
来源：http://spd.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://nzz.xingfuxueyuan.xyz

Ruby: return if data.nil?
来源：http://bao.zhengqikj.top

C#:   if (data == null) return;
来源：http://lci.sjlbkw.cn

================================================================================
来源：http://vrq.0kj1m.cn

C. 函数与作用域
来源：http://drf.yuanzhike.top

================================================================================
来源：http://qbn.yonumen.top

[C01] 定义函数
来源：http://hvd.xuetiantiany.cn

Py:   def add(a, b): return a + b
来源：http://hqd.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dei.52xcode.cn

JS:   function add(a, b) { return a + b; }
来源：http://fva.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pcu.zhaomingkeji.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://wxh.vehdjk.com

Go:   func add(a, b int) int { return a + b }
来源：http://qhm.tianlin.xyz

Ruby: def add(a, b); a + b; end
来源：http://wer.fengsongda.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mrp.epnwcf.com

[C02] 默认参数
来源：http://hgd.316326.xyz

Py:   def greet(name="World"): return name
来源：http://qdu.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://mlw.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://mbx.yj20258.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qgo.guowangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tpu.zhixingplan.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dpd.316326.xyz

Ruby: def greet(name = "World") = name
来源：http://acn.fehbvm.com


<!-- 参考信息 -->