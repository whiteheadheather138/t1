代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sep.haohaochexian.top

Java: (int) 'A'; (char) 65
来源：http://uoj.zhijiandao.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wrp.dashuyun.cn

Ruby: "A".ord; 65.chr
来源：http://mng.andypj.xyz

C#:   (int)'A'; (char)65
来源：http://mau.chenjidiqi.icu

[A19] 交换两个变量
来源：http://vtu.jqgufenzy.top

Py:   a, b = b, a
来源：http://frp.nanxuanxn.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ccj.jqgufenzy.top

JS:   [a, b] = [b, a];
来源：http://oah.daxiang520.top

TS:   [a, b] = [b, a];
来源：http://ong.zdbjq.cn

Java: int t = a; a = b; b = t;
来源：http://opm.cashguo.top

Go:   a, b = b, a
来源：http://ect.nanxinkj.top

Ruby: a, b = b, a
来源：http://tdv.ydzc1.top

C#:   (a, b) = (b, a);
来源：http://ccg.zhaomingkeji.xyz

[A20] 读取标准输入
来源：http://wkt.jqgufenzy.top

Py:   name = input("请输入：")
来源：http://xxy.yonumen.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rmw.fktsv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ibs.yonumen.top

TS:   // Node.js：readline 模块
来源：http://swf.sjlbkw.cn

Java: new Scanner(System.in).nextLine()
来源：http://pju.kuanghao11.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ipw.redwolf501.top

Ruby: gets.chomp
来源：http://mdr.chenzaomai.com

C#:   Console.ReadLine();
来源：http://dxo.redwolf501.top

[A21] 保留指定小数位输出
来源：http://fzs.jinqigufen.top

Py:   f"{3.14159:.2f}"
来源：http://eqd.fehbvm.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ikx.vqdsnc.cn

JS:   (3.14159).toFixed(2)
来源：http://lwm.chenjidiqi.icu

TS:   (3.14159).toFixed(2)
来源：http://tkh.gaohongyu789.top

Java: String.format("%.2f", 3.14159)
来源：http://mdc.kuanghao11.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iic.jinqigfzy.top

Ruby: format("%.2f", 3.14159)
来源：http://mbo.hammf.cn

C#:   3.14159.ToString("F2")
来源：http://tql.cqqwz.cn

[A22] 获取字符串长度
来源：http://fug.iojbl.cn

Py:   len(s)
来源：http://lla.shzxlz.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gbc.fengsongda.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nsc.cucudq.cn

TS:   s.length
来源：http://kgc.jinghuilouyu.cn

Java: s.length()
来源：http://zcc.zhiwuduotai.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://stx.shanyushiyangtech.top

Ruby: s.length
来源：http://rmo.316326.xyz

C#:   s.Length
来源：http://ezg.cqqwz.cn

[A23] 大小写转换
来源：http://mzo.pengpengdd.cyou

Py:   s.upper(); s.lower(); s.title()
来源：http://ohf.sufxvd.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tsq.redwolf501.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lpo.xinyue.icu

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yth.quarkkingdee.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gwy.cqqwz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zfs.tanke756.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eiy.gaohongyu789.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gad.hammf.cn

[A24] 去除首尾空白
来源：http://sjy.ppjwa.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bsf.gogol.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fev.ehwqpu.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yfq.jinqigufen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hyb.hcnkem.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://anu.ywan-chungtsiang.top

Go:   strings.TrimSpace(s)
来源：http://oxy.tianlin.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sse.yongpay.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ahj.meibo888.top

[A25] 字符串比较
来源：http://bjq.ivvv.top

Py:   s1 == s2; s1 != s2
来源：http://vro.sxryk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bxs.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kuj.andypj.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bik.dashuyun.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tfu.gzhubu.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wuf.epnwcf.com

Ruby: s1 == s2; s1 <=> s2
来源：http://dek.bbcook.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nca.fengsongda.top

[A26] 类型转换总览
来源：http://ami.redwolf501.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ipb.yj20258888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wuh.yvedp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hla.pengpengdd.cyou

TS:   Number() String() Boolean() x as number
来源：http://blv.sxryk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hgs.uphjek.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jzl.zdbjq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://upd.shuidangran.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://izm.hywenlv.cn

================================================================================
来源：http://pxd.jyoumei.cn

B. 流程控制
来源：http://plh.jyoumei.cn

================================================================================
来源：http://irr.hongshengwenyu.top

[B01] 条件判断 if / else
来源：http://tzu.tanke756.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zcv.hysaishi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bjb.yangfankeji.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ndj.yj20258888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hwt.yfazqb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://kyw.xinyue.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mls.ehwqpu.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://clw.jlsjyb.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pyn.gogol.net.cn

[B02] 多分支 else if / elif
来源：http://qrg.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vkd.mhx1999.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vuf.yangfankeji.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://quy.52xcode.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cka.tian-w.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yqy.havefunace.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vbs.haohaochexian.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://heq.fktsv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kxx.wangshuangyany.cn

[B03] switch / match / case
来源：http://osk.chenjidiqi.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mbq.aizwys.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eao.ydjk.org.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wso.ctjpmb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lpx.zhiwuduotai.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wni.jianghu66.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pgi.chenjidiqi.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://brz.zycfv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://imk.zdqjudy.top

[B04] for 计数循环
来源：http://qfe.kuanghao11.cn

Py:   for i in range(10): print(i)
来源：http://aeh.yangfankeji.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zmv.chenlongwang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hjm.vqdsnc.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uhq.chenzaomai.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gll.ehwqpu.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yno.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://yjm.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://epr.jinghuilouyu.cn

[B05] 遍历数组 / 列表
来源：http://cwc.jyoumei.cn

Py:   for item in arr: print(item)
来源：http://cms.iojbl.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sak.ydjk.org.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://olf.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://rdq.jinqigufen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gqr.jinqigufen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hwg.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://uux.bjfxy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://led.kuanghao11.cn

[B06] 遍历字典 / 对象
来源：http://qpu.jinqigfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cpe.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rls.jinyuanbaomall.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hma.hfpthk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xjc.xziqi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fdx.yj20258888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://htk.havefunace.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ocw.yfazqb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pev.shuidangran.top

[B07] while 循环
来源：http://nwc.hongshengwenyu.top

Py:   while i < 10: i += 1
来源：http://hhd.kuanghao11.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jje.hnqzz.top

JS:   while (i < 10) { i++; }
来源：http://nij.cdnleiting.top

TS:   while (i < 10) { i++; }
来源：http://pzm.xylfe.cn

Java: while (i < 10) { i++; }
来源：http://idl.pycfn.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xnf.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://mfx.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://gpl.aizwys.cn

[B08] do-while（至少执行一次）
来源：http://xir.cdnleiting.top

Py:   # 无 do-while：用 while True + break
来源：http://bjj.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dwy.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://kvu.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://hle.tanke756.top

Java: do { i++; } while (i < 10);
来源：http://wuw.xinyue.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://zfr.ybcxt.top

Ruby: begin; i += 1; end while i < 10
来源：http://akk.chenjidiqi.icu

C#:   do { i++; } while (i < 10);
来源：http://teh.zhixingplan.top

[B09] break 与 continue
来源：http://lsp.nanxuanxn.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iag.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pjr.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jla.jianghu66.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rnu.jianghu66.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xrh.dashuyun.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lbx.meibo888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fhb.ctjpmb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mue.fzhhl.top

[B10] 遍历同时拿索引
来源：http://nqi.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zjn.zhaomingkeji.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dhd.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hwr.xingfuxueyuan.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wdo.tarul.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kek.316326.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kga.snrcjt.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://arn.snrcjt.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hoj.epnwcf.com

[B11] 生成数字序列 / 区间
来源：http://mhu.cucudq.cn

Py:   list(range(0, 10, 2))
来源：http://zlf.zycfv.cn

PHP:  range(0, 10, 2);
来源：http://iyc.uphjek.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jrg.cucudq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ffv.gzhubu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gez.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://urk.jianghu66.top

Ruby: (0...10).step(2).to_a
来源：http://prt.redwolf501.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ujv.fzhhl.top

[B12] 跳出多层循环
来源：http://ket.dashuyun.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://flk.cqqwz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://egd.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pxo.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xro.daxiang520.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://knl.nanxuanxn.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://haq.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tkd.hysaishi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uqq.52xcode.cn

[B13] 判断是否为数字
来源：http://swd.hammf.cn

Py:   isinstance(x, (int, float))
来源：http://zky.sxryk.cn

PHP:  is_numeric($x)
来源：http://euv.zhiwuduotai.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ggw.shanyushiyangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ckl.epnwcf.com

Java: x instanceof Number
来源：http://dwb.jinyuanbaomall.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zlm.0kj1m.cn

Ruby: x.is_a?(Numeric)
来源：http://pru.chenlongwang.top

C#:   x is int or double or decimal
来源：http://mdm.tarul.cn

[B14] 判断值是否在集合内
来源：http://bhq.cqqwz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mhh.jqgufenzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zwk.tian-w.cn

JS:   [1, 2, 3].includes(x)
来源：http://ecq.sxryk.cn

TS:   [1, 2, 3].includes(x)
来源：http://sok.gaohongyu789.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pnj.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yyk.aizwys.cn

Ruby: [1, 2, 3].include?(x)
来源：http://iwo.yueranfly.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kqk.zhoulong.xyz

[B15] 布尔运算与取反
来源：http://lmr.gaohongyu789.top

Py:   a and b or not c
来源：http://qim.yonumen.top

PHP:  $a && $b || !$c
来源：http://txb.quarkkingdee.top

JS:   a && b || !c
来源：http://qom.jqgufenzy.top

TS:   a && b || !c
来源：http://qhq.meibo888.top

Java: a && b || !c
来源：http://ohk.yuanzhike.top

Go:   a && b || !c
来源：http://kay.haohaochexian.top

Ruby: a && b || !c
来源：http://gjf.ppjwa.cn

C#:   a && b || !c
来源：http://tcw.wangshuangyany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rcp.haohaochexian.top

Py:   if not data: return
来源：http://dsb.redwolf501.top

PHP:  if (!$data) { return; }
来源：http://hzn.sufxvd.cn

JS:   if (!data) return;
来源：http://hxl.xuetiantiany.cn

TS:   if (!data) return;
来源：http://sid.feifeiyinyue.top

Java: if (data == null) return;
来源：http://seh.sjlbkw.cn

Go:   if data == nil { return }
来源：http://wcg.nwbrower.top

Ruby: return if data.nil?
来源：http://pkw.jinyuanbaomall.cn

C#:   if (data == null) return;
来源：http://cek.gzhubu.top

================================================================================
来源：http://uhn.sysykeji.top

C. 函数与作用域
来源：http://bmi.guowangkeji.top

================================================================================
来源：http://scy.fehbvm.com

[C01] 定义函数
来源：http://smt.vehdjk.com

Py:   def add(a, b): return a + b
来源：http://ggz.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ntm.mhx1999.top

JS:   function add(a, b) { return a + b; }
来源：http://fpc.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xww.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dlf.jinqigufen.top

Go:   func add(a, b int) int { return a + b }
来源：http://rfa.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://rvf.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://epa.shangyingyoupin.top

[C02] 默认参数
来源：http://dzm.yj20258.top

Py:   def greet(name="World"): return name
来源：http://aye.bjfxy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jqd.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://sdd.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fmo.bjfxy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nbv.chenzaomai.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sop.52xcode.cn

Ruby: def greet(name = "World") = name
来源：http://awk.shanyushiyangtech.top

C#:   string Greet(string name = "World") => name;
来源：http://ggz.mhx1999.top

[C03] 可变参数
来源：http://csx.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://bbx.hcnkem.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pqb.zhaomingkeji.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gen.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ygj.nwbrower.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oec.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pyo.yongpay.top

Ruby: def total(*nums); nums.sum; end
来源：http://rno.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hhk.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://tra.vqdsnc.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qqf.shanyushiyangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xfw.pycfn.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qii.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wgx.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://qhr.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://ylp.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://kom.hnxiangtu.top

C#:   f(a: 1, b: 2)
来源：http://ltk.vehdjk.com

[C05] 返回多个值
来源：http://zqu.ydjk.org.cn

Py:   return a, b
来源：http://dtg.yj20258888.top

PHP:  return [$a, $b];
来源：http://avk.ivvv.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://uip.pycfn.com

TS:   return { a, b };
来源：http://asc.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eao.yuanzhike.top

Go:   return a, b
来源：http://lyd.hcnkem.com

Ruby: return a, b
来源：http://dwk.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://jpw.yuanzhike.top

[C06] 匿名函数 / lambda
来源：http://gej.cqqwz.cn

Py:   square = lambda x: x * x
来源：http://cow.meibo888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hjb.nwbrower.top

JS:   const square = x => x * x;
来源：http://qiy.birdmap.top

TS:   const square = (x: number): number => x * x;
来源：http://yns.hnxiangtu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://atq.zycfv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ekc.chenzaomai.com

Ruby: square = ->(x) { x * x }
来源：http://zne.hcnkem.com

C#:   Func<int, int> square = x => x * x;
来源：http://ixe.hammf.cn

[C07] 把函数作为参数传入
来源：http://zow.jinqigufen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rev.hywenlv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xqf.yangfankeji.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cxg.zhiwuduotai.top

TS:   arr.map(String)
来源：http://pej.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://idh.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://idm.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://aov.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ixk.xylfe.cn

[C08] 闭包
来源：http://dkr.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hzo.xinyue.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qlq.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ymb.yj20258888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lrj.tanke756.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dmh.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://odu.cdnleiting.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mrl.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eqx.c1oappe.top

[C09] 递归
来源：http://fgl.zhiwuduotai.top


<!-- 参考信息 -->