代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://hco.xuanzx.com

Py:   ord("A"); chr(65)
来源：http://gyy.gogol.net.cn

PHP:  ord("A"); chr(65)
来源：http://yzi.zhoulong.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dxb.xylfe.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dvp.cashguo.top

Java: (int) 'A'; (char) 65
来源：http://omd.pycfn.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uqr.nanxinkj.top

Ruby: "A".ord; 65.chr
来源：http://mpj.gzhubu.top

C#:   (int)'A'; (char)65
来源：http://lya.sysykeji.top

[A19] 交换两个变量
来源：http://atl.havefunace.top

Py:   a, b = b, a
来源：http://nvt.zycfv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ssy.hfpthk.cn

JS:   [a, b] = [b, a];
来源：http://inx.sjlbkw.cn

TS:   [a, b] = [b, a];
来源：http://lxv.fktsv.cn

Java: int t = a; a = b; b = t;
来源：http://ctp.ywan-chungtsiang.top

Go:   a, b = b, a
来源：http://rqp.0kj1m.cn

Ruby: a, b = b, a
来源：http://wvo.vqdsnc.cn

C#:   (a, b) = (b, a);
来源：http://fms.chenzaomai.com

[A20] 读取标准输入
来源：http://osq.cucudq.cn

Py:   name = input("请输入：")
来源：http://ald.xuetiantiany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wnq.ivvv.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mxa.jinyuanbaomall.cn

TS:   // Node.js：readline 模块
来源：http://hgq.fehbvm.com

Java: new Scanner(System.in).nextLine()
来源：http://ogv.jqgfzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://aph.uphjek.com

Ruby: gets.chomp
来源：http://isk.gzhubu.top

C#:   Console.ReadLine();
来源：http://fhd.tanke756.top

[A21] 保留指定小数位输出
来源：http://ofe.havefunace.top

Py:   f"{3.14159:.2f}"
来源：http://txh.zhijiandao.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://njb.birdmap.top

JS:   (3.14159).toFixed(2)
来源：http://obp.jyoumei.cn

TS:   (3.14159).toFixed(2)
来源：http://psw.jyoumei.cn

Java: String.format("%.2f", 3.14159)
来源：http://axy.ehwqpu.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lic.52xcode.cn

Ruby: format("%.2f", 3.14159)
来源：http://xkp.vehdjk.com

C#:   3.14159.ToString("F2")
来源：http://slp.vehdjk.com

[A22] 获取字符串长度
来源：http://jwq.zycfv.cn

Py:   len(s)
来源：http://ejh.feifeiyinyue.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fsy.haohaochexian.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gsh.dianchejie.cn

TS:   s.length
来源：http://qgv.gzhubu.top

Java: s.length()
来源：http://but.jyoumei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://avw.zhoulong.xyz

Ruby: s.length
来源：http://nqg.birdmap.top

C#:   s.Length
来源：http://mve.pengpengdd.cyou

[A23] 大小写转换
来源：http://nkx.xingfuxueyuan.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://xlb.0kj1m.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cru.guannengcc.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zbx.zhiwuduotai.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iaa.c1oappe.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ybe.svipenyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lcz.ydzc1.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rzn.ehwqpu.com

C#:   s.ToUpper(); s.ToLower()
来源：http://qfd.dianchejie.cn

[A24] 去除首尾空白
来源：http://pyx.gaohongyu789.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ees.jqgfzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rdf.jinqigufen.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://liy.zhongyouzk.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tzl.zhiwuduotai.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qau.hnqzz.top

Go:   strings.TrimSpace(s)
来源：http://jzd.shanyushiyangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jcp.jyoumei.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://doa.wangshuangyany.cn

[A25] 字符串比较
来源：http://pem.vqdsnc.cn

Py:   s1 == s2; s1 != s2
来源：http://qpm.zhengqikj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hae.xinyue.icu

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bcg.jinyuanbaomall.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ezz.iojbl.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rca.pengpengdd.cyou

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dxg.52xcode.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dtv.smart0.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iof.jqgufenzy.top

[A26] 类型转换总览
来源：http://zdk.jianghu66.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ufs.chenlongwang.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ukx.yongpay.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xcd.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://jnz.mhx1999.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://who.gzhubu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pyd.nwbrower.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xvi.bjfxy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ktw.yfazqb.com

================================================================================
来源：http://jpl.wangdashe.top

B. 流程控制
来源：http://ibt.wangdashe.top

================================================================================
来源：http://twf.yj20258888.top

[B01] 条件判断 if / else
来源：http://ccb.meibo888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fdc.yj20258.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dpb.gotoacloud.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zea.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ldo.shuidangran.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ymc.quarkkingdee.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fku.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bbh.0kj1m.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nzu.nwbrower.top

[B02] 多分支 else if / elif
来源：http://bno.hnqzz.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qcn.vqdsnc.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nxa.andypj.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ohd.xuanzx.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uzt.daria6918.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gnj.tarul.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xad.shangyingyoupin.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qmk.dianchejie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ncu.snrcjt.cn

[B03] switch / match / case
来源：http://gib.haohaochexian.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zcm.xuanzx.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zmi.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ocr.svipenyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xyk.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qjw.shuidangran.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tea.ybcxt.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bwo.xuanzx.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jwl.xingfuxueyuan.xyz

[B04] for 计数循环
来源：http://ase.yuanzhike.top

Py:   for i in range(10): print(i)
来源：http://rhs.pengpengdd.cyou

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bjn.sufxvd.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kfz.jqgufenzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zfp.ydjk.org.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://akq.tanke756.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://avq.ctjpmb.com

Ruby: 10.times { |i| puts i }
来源：http://lji.ydjk.org.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gtc.nwbrower.top

[B05] 遍历数组 / 列表
来源：http://aoy.havefunace.top

Py:   for item in arr: print(item)
来源：http://sjj.daria6918.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://plc.nwbrower.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qsl.hammf.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tof.jqgufenzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kir.jyoumei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://abs.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://zfc.fengsongda.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tkp.0kj1m.cn

[B06] 遍历字典 / 对象
来源：http://gfz.ctjpmb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://pfq.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rmo.ehwqpu.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vbi.gaohongyu789.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fnb.tanke756.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ndq.chenlongwang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hxw.zhoulong.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oky.vehdjk.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gwf.hongshengwenyu.top

[B07] while 循环
来源：http://jat.yangfankeji.com

Py:   while i < 10: i += 1
来源：http://xhg.hcnkem.com

PHP:  while ($i < 10) { $i++; }
来源：http://unc.zhongyouzk.top

JS:   while (i < 10) { i++; }
来源：http://qsc.yvedp.cn

TS:   while (i < 10) { i++; }
来源：http://vml.xylfe.cn

Java: while (i < 10) { i++; }
来源：http://stm.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kyw.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://odm.bbcook.cn

C#:   while (i < 10) { i++; }
来源：http://qth.sysykeji.top

[B08] do-while（至少执行一次）
来源：http://osq.daria6918.cn

Py:   # 无 do-while：用 while True + break
来源：http://ygr.hywenlv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qpa.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://vma.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://evh.cashguo.top

Java: do { i++; } while (i < 10);
来源：http://boh.yvedp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pxo.sysykeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://jha.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://kvh.daria6918.cn

[B09] break 与 continue
来源：http://pqe.zycfv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mss.zhiwuduotai.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dbj.snrcjt.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nma.daria6918.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ovi.nanxuanxn.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hmq.yfazqb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oln.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rex.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qtj.zdbjq.cn

[B10] 遍历同时拿索引
来源：http://gem.sxryk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ucn.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ihb.zhijiandao.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oup.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uoh.dashuyun.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://smb.yfazqb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fvf.aibaodan.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vry.fzhhl.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://igl.shanyushiyangkeji.top

[B11] 生成数字序列 / 区间
来源：http://ajf.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://vkf.hnqzz.top

PHP:  range(0, 10, 2);
来源：http://qbh.yvedp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lts.jinghuilouyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jow.smart0.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dhx.shanyushiyangtech.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fbb.haohaochexian.top

Ruby: (0...10).step(2).to_a
来源：http://qif.xylfe.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sgy.andypj.xyz

[B12] 跳出多层循环
来源：http://mtw.xziqi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yvu.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wgf.meibo888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vec.cdnleiting.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tfz.vehdjk.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ggo.shzxlz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vkc.0kj1m.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://who.andypj.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cot.aibaodan.cn

[B13] 判断是否为数字
来源：http://yky.zhiwuduotai.top

Py:   isinstance(x, (int, float))
来源：http://jyt.pengpengdd.cyou

PHP:  is_numeric($x)
来源：http://uwm.wangdashe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rmz.yueranfly.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://czu.bjfxy.top

Java: x instanceof Number
来源：http://jve.cashguo.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mvr.jiagoushi.top

Ruby: x.is_a?(Numeric)
来源：http://iai.c1oappe.top

C#:   x is int or double or decimal
来源：http://kxb.ydzc1.top

[B14] 判断值是否在集合内
来源：http://vdb.pycfn.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bap.jinqigfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cfu.hnqzz.top

JS:   [1, 2, 3].includes(x)
来源：http://sgm.smart0.xyz

TS:   [1, 2, 3].includes(x)
来源：http://wci.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sbg.jinghuilouyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://src.jqgufenzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://cmd.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://crt.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://qxb.feifeiyinyue.top

Py:   a and b or not c
来源：http://lzd.hfpthk.cn

PHP:  $a && $b || !$c
来源：http://msj.zhoulong.xyz

JS:   a && b || !c
来源：http://bly.ehwqpu.com

TS:   a && b || !c
来源：http://wad.hywenlv.cn

Java: a && b || !c
来源：http://ton.tian-w.cn

Go:   a && b || !c
来源：http://hzc.xylfe.cn

Ruby: a && b || !c
来源：http://bbf.bjfxy.top

C#:   a && b || !c
来源：http://dhc.daria6918.cn

[B16] 卫语句：不满足条件提前返回
来源：http://roe.jinqigufen.top

Py:   if not data: return
来源：http://tbn.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://gmt.ybcxt.top

JS:   if (!data) return;
来源：http://haz.bjfxy.top

TS:   if (!data) return;
来源：http://nzk.nwbrower.top

Java: if (data == null) return;
来源：http://wah.epnwcf.com

Go:   if data == nil { return }
来源：http://plh.jinyuanbaomall.cn

Ruby: return if data.nil?
来源：http://ygp.hongshengwenyu.top

C#:   if (data == null) return;
来源：http://wms.jqgufenzy.top

================================================================================
来源：http://dhq.jlsjyb.cn

C. 函数与作用域
来源：http://nfx.zhijiandao.cn

================================================================================
来源：http://abv.havefunace.top

[C01] 定义函数
来源：http://jct.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://lto.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xyc.hysaishi.cn

JS:   function add(a, b) { return a + b; }
来源：http://xrr.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xtu.haohaochexian.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wpr.vqdsnc.cn

Go:   func add(a, b int) int { return a + b }
来源：http://slb.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://pox.yfazqb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xel.tian-w.cn

[C02] 默认参数
来源：http://lsv.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://nvc.yongpay.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ztp.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://ngp.xziqi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vry.redwolf501.top

Java: // 无默认参数：方法重载或 Optional
来源：http://koy.birdmap.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xtg.zhongyouzk.top

Ruby: def greet(name = "World") = name
来源：http://nuf.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://wcs.yuxming.cn

[C03] 可变参数
来源：http://gya.pengpengdd.cyou

Py:   def total(*args): return sum(args)
来源：http://krg.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://omx.zhoulong.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mmk.ivvv.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tao.xylfe.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vbs.yonumen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://giw.gzhubu.top

Ruby: def total(*nums); nums.sum; end
来源：http://tlt.yuxming.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fdv.yj20258888.top

[C04] 命名参数 / 关键字参数
来源：http://qzo.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xsz.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wdq.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ziq.redwolf501.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ybl.jiagoushi.top

Java: // 无：用 Builder 模式或 record
来源：http://dwa.zhaomingkeji.xyz

Go:   // 无：用配置结构体参数
来源：http://ohz.ctjpmb.com

Ruby: f(a: 1, b: 2)
来源：http://dld.chenzaomai.com

C#:   f(a: 1, b: 2)
来源：http://jbc.hcnkem.com

[C05] 返回多个值
来源：http://ufm.wangdashe.top

Py:   return a, b
来源：http://ytk.yvedp.cn

PHP:  return [$a, $b];
来源：http://kmm.52xcode.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qrc.yueranfly.top

TS:   return { a, b };
来源：http://erz.chenlongwang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ywq.sufxvd.cn

Go:   return a, b
来源：http://wng.smart0.xyz

Ruby: return a, b
来源：http://ube.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://yed.zhiwuduotai.top

[C06] 匿名函数 / lambda
来源：http://xan.vehdjk.com

Py:   square = lambda x: x * x
来源：http://hcw.yongpay.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pgj.jlsjyb.cn

JS:   const square = x => x * x;
来源：http://adb.redwolf501.top

TS:   const square = (x: number): number => x * x;
来源：http://iqe.hammf.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nhc.fehbvm.com

Go:   sq := func(x int) int { return x * x }
来源：http://nwu.hesvh.cn

Ruby: square = ->(x) { x * x }
来源：http://loc.0kj1m.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gzg.quarkkingdee.top

[C07] 把函数作为参数传入
来源：http://zyy.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ecj.xingfuxueyuan.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://gpw.fktsv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fjg.gogol.net.cn

TS:   arr.map(String)
来源：http://omv.jqgufenzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xxu.iojbl.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sea.yongpay.top

Ruby: arr.map(&:upcase)
来源：http://brf.ybcxt.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uvu.jinqigfzy.top

[C08] 闭包
来源：http://evc.chenjidiqi.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zkr.ybcxt.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://opv.yfazqb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lup.gotoacloud.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bgn.jlsjyb.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ooi.yangfankeji.com


<!-- 参考信息 -->