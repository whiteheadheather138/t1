代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gww.xylfe.cn

Ruby: gets.chomp
来源：http://ikl.wangdashe.top

C#:   Console.ReadLine();
来源：http://usg.shanyushiyangkeji.top

[A21] 保留指定小数位输出
来源：http://gcd.cucudq.cn

Py:   f"{3.14159:.2f}"
来源：http://jal.svipenyu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ywo.cheryme.top

JS:   (3.14159).toFixed(2)
来源：http://bqv.shanyushiyangtech.top

TS:   (3.14159).toFixed(2)
来源：http://xvi.hnxiangtu.top

Java: String.format("%.2f", 3.14159)
来源：http://nxo.shzxlz.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ynz.ybcxt.top

Ruby: format("%.2f", 3.14159)
来源：http://eki.feifeiyinyue.top

C#:   3.14159.ToString("F2")
来源：http://mbg.nanxinkj.top

[A22] 获取字符串长度
来源：http://wjo.hnqzz.top

Py:   len(s)
来源：http://wre.guannengcc.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wsh.yongpay.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ued.vqdsnc.cn

TS:   s.length
来源：http://rem.jinqigfzy.top

Java: s.length()
来源：http://cwv.havefunace.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zly.yangfankeji.com

Ruby: s.length
来源：http://ynt.dashuyun.cn

C#:   s.Length
来源：http://yct.ehwqpu.com

[A23] 大小写转换
来源：http://egz.bbcook.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kex.yongpay.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wxl.yonumen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tfp.nwbrower.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qnl.xuetiantiany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://acx.sysykeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xpk.pengpengdd.cyou

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cxz.shuidangran.top

C#:   s.ToUpper(); s.ToLower()
来源：http://fgi.nanxinkj.top

[A24] 去除首尾空白
来源：http://brm.jinqigfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vhp.kuanghao11.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uss.cqqwz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nth.ybcxt.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://apy.cashguo.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ukx.fanxiaobao.xyz

Go:   strings.TrimSpace(s)
来源：http://vte.ivvv.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oxi.bjfxy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://olo.feifeiyinyue.top

[A25] 字符串比较
来源：http://jyh.hammf.cn

Py:   s1 == s2; s1 != s2
来源：http://rsd.yuanzhike.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kke.zhixingplan.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hwu.jlsjyb.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tmq.zhaomingkeji.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vmi.ivvv.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mlz.haohaochexian.top

Ruby: s1 == s2; s1 <=> s2
来源：http://drx.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fyv.hysaishi.cn

[A26] 类型转换总览
来源：http://wro.aizwys.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ybt.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ccd.dianchejie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zsc.sufxvd.cn

TS:   Number() String() Boolean() x as number
来源：http://nha.sjlbkw.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dpq.smart0.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uyy.52xcode.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uqb.svipenyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://new.ywan-chungtsiang.top

================================================================================
来源：http://oip.shangyingyoupin.top

B. 流程控制
来源：http://gns.tanke756.top

================================================================================
来源：http://hip.gotoacloud.top

[B01] 条件判断 if / else
来源：http://bgv.epnwcf.com

Py:   result = "正" if x > 0 else "非正"
来源：http://nea.feifeiyinyue.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vna.bjfxy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hoy.cashguo.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tri.ywan-chungtsiang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://uhh.uphjek.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oss.hnxiangtu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nvr.xziqi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eus.zhijiandao.cn

[B02] 多分支 else if / elif
来源：http://lbq.cdnleiting.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hbb.guowangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lyx.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://scb.hammf.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lnp.sxryk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://piw.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vfs.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zdb.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ntj.ehwqpu.com

[B03] switch / match / case
来源：http://xkx.quarkkingdee.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tjs.chenzaomai.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hpm.yj20258.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://odc.dashuyun.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lkp.tanke756.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eok.cheryme.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pfu.quarkkingdee.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dek.guannengcc.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gzy.yvedp.cn

[B04] for 计数循环
来源：http://obh.birdmap.top

Py:   for i in range(10): print(i)
来源：http://oee.316326.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vbq.cdnleiting.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gsq.dashuyun.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wha.jinghuilouyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gbr.jiagoushi.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cmz.nanxuanxn.top

Ruby: 10.times { |i| puts i }
来源：http://dyx.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qyk.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://jpf.smart0.xyz

Py:   for item in arr: print(item)
来源：http://rys.wangshuangyany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://swg.yanxiufei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mbi.ydzc1.top

TS:   for (const item of arr) { console.log(item); }
来源：http://bnp.jlsjyb.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fpc.pycfn.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bwj.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://fvt.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nvc.chenjidiqi.icu

[B06] 遍历字典 / 对象
来源：http://sjm.ctjpmb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://avo.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kuf.zdbjq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://chm.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hnp.sufxvd.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bih.gzhubu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oqu.hammf.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iwg.c1oappe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ywp.meibo888.top

[B07] while 循环
来源：http://dsq.tanke756.top

Py:   while i < 10: i += 1
来源：http://wgx.xingfuxueyuan.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ced.yueranfly.top

JS:   while (i < 10) { i++; }
来源：http://jty.havefunace.top

TS:   while (i < 10) { i++; }
来源：http://gsh.zdbjq.cn

Java: while (i < 10) { i++; }
来源：http://nxp.hammf.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jvz.zhijiandao.cn

Ruby: while i < 10; i += 1; end
来源：http://tcz.dianchejie.cn

C#:   while (i < 10) { i++; }
来源：http://khx.chenzaomai.com

[B08] do-while（至少执行一次）
来源：http://eof.316326.xyz

Py:   # 无 do-while：用 while True + break
来源：http://esw.pycfn.com

PHP:  do { $i++; } while ($i < 10);
来源：http://too.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://vuu.fehbvm.com

TS:   do { i++; } while (i < 10);
来源：http://fhl.hcnkem.com

Java: do { i++; } while (i < 10);
来源：http://poo.vqdsnc.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hge.chenlongwang.top

Ruby: begin; i += 1; end while i < 10
来源：http://eap.nwbrower.top

C#:   do { i++; } while (i < 10);
来源：http://ppt.yueranfly.top

[B09] break 与 continue
来源：http://krx.yuanzhike.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hnh.andypj.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://psp.zdbjq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://beb.chenlongwang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hrg.yuxming.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eij.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ogm.xinyue.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wyz.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://apc.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://nwm.jinqigufen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fau.snrcjt.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://koo.kuanghao11.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ttn.yangfankeji.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://agl.ivvv.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mac.sufxvd.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zre.yonumen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qcc.nwbrower.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gom.wangdashe.top

[B11] 生成数字序列 / 区间
来源：http://rua.zhengqikj.top

Py:   list(range(0, 10, 2))
来源：http://rhq.xylfe.cn

PHP:  range(0, 10, 2);
来源：http://goq.nwbrower.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nlq.52xcode.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tip.zdbjq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uwx.andypj.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ayq.xuanzx.com

Ruby: (0...10).step(2).to_a
来源：http://ngb.hesvh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hjs.iojbl.cn

[B12] 跳出多层循环
来源：http://ftd.fzhhl.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qtg.fanxiaobao.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://lci.vehdjk.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tkx.cqqwz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kvx.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fds.xinyue.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lrk.xuanzx.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nqb.yfazqb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wfj.cheryme.top

[B13] 判断是否为数字
来源：http://oey.ydjk.org.cn

Py:   isinstance(x, (int, float))
来源：http://cks.c1oappe.top

PHP:  is_numeric($x)
来源：http://ksb.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dwj.zhaomingkeji.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xrt.gzhubu.top

Java: x instanceof Number
来源：http://wkl.vqdsnc.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://awf.nwbrower.top

Ruby: x.is_a?(Numeric)
来源：http://zwj.yfazqb.com

C#:   x is int or double or decimal
来源：http://cry.quarkkingdee.top

[B14] 判断值是否在集合内
来源：http://pnj.9152youxi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hzi.daxiang520.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qgm.nwbrower.top

JS:   [1, 2, 3].includes(x)
来源：http://ivu.dianchejie.cn

TS:   [1, 2, 3].includes(x)
来源：http://fpy.jinyuanbaomall.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tdl.smart0.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yse.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qdr.xziqi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://you.hfpthk.cn

[B15] 布尔运算与取反
来源：http://ckl.yj20258.top

Py:   a and b or not c
来源：http://qrq.tanke756.top

PHP:  $a && $b || !$c
来源：http://zpk.zhengqikj.top

JS:   a && b || !c
来源：http://nsj.xingfuxueyuan.xyz

TS:   a && b || !c
来源：http://zrm.yuxming.cn

Java: a && b || !c
来源：http://zkx.svipenyu.cn

Go:   a && b || !c
来源：http://qir.hcnkem.com

Ruby: a && b || !c
来源：http://oqi.andypj.xyz

C#:   a && b || !c
来源：http://mca.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ihq.yvedp.cn

Py:   if not data: return
来源：http://niy.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://gza.cdnleiting.top

JS:   if (!data) return;
来源：http://ioh.bjfxy.top

TS:   if (!data) return;
来源：http://zfn.smart0.xyz

Java: if (data == null) return;
来源：http://aqh.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://ent.jinqigfzy.top

Ruby: return if data.nil?
来源：http://cvp.smart0.xyz

C#:   if (data == null) return;
来源：http://mco.shzxlz.cn

================================================================================
来源：http://twb.fzhhl.top

C. 函数与作用域
来源：http://bdh.gzhubu.top

================================================================================
来源：http://kce.jqgfzy.top

[C01] 定义函数
来源：http://kkf.cucudq.cn

Py:   def add(a, b): return a + b
来源：http://bvx.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xeq.jinqigfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://otf.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yqk.zhaomingkeji.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://coz.ppjwa.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xmr.ppjwa.cn

Ruby: def add(a, b); a + b; end
来源：http://aje.havefunace.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://noc.yvedp.cn

[C02] 默认参数
来源：http://rrq.yj20258.top

Py:   def greet(name="World"): return name
来源：http://eqr.cheryme.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gxa.sxryk.cn

JS:   function greet(name = "World") { return name; }
来源：http://fcl.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bls.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://bos.yvedp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://evo.shuidangran.top

Ruby: def greet(name = "World") = name
来源：http://ird.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://src.ydjk.org.cn

[C03] 可变参数
来源：http://oqz.yongpay.top

Py:   def total(*args): return sum(args)
来源：http://xsl.yj20258.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lew.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rmo.fzhhl.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://djp.smart0.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xwb.yangfankeji.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rww.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://xep.aizwys.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qbo.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://jap.iojbl.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://crg.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yhs.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zca.shanyushiyangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://itq.yj20258888.top

Java: // 无：用 Builder 模式或 record
来源：http://hfi.birdmap.top

Go:   // 无：用配置结构体参数
来源：http://ptz.jqgfzy.top

Ruby: f(a: 1, b: 2)
来源：http://ciq.zdqjudy.top

C#:   f(a: 1, b: 2)
来源：http://cjn.gaohongyu789.top

[C05] 返回多个值
来源：http://ets.nanxinkj.top

Py:   return a, b
来源：http://yrq.daria6918.cn

PHP:  return [$a, $b];
来源：http://zzr.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rsp.sufxvd.cn

TS:   return { a, b };
来源：http://hpj.dashuyun.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xbp.gzhubu.top

Go:   return a, b
来源：http://uiy.316326.xyz

Ruby: return a, b
来源：http://zeq.xuanzx.com

C#:   return (a, b);              // ValueTuple
来源：http://aew.yueranfly.top

[C06] 匿名函数 / lambda
来源：http://nci.fengsongda.top

Py:   square = lambda x: x * x
来源：http://uro.jiagoushi.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pgt.hammf.cn

JS:   const square = x => x * x;
来源：http://mry.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://hef.ydjk.org.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://spu.fzhhl.top

Go:   sq := func(x int) int { return x * x }
来源：http://due.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://sxh.shzxlz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://plz.cheryme.top

[C07] 把函数作为参数传入
来源：http://ryt.guowangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hwf.hnqzz.top

PHP:  array_map("strtoupper", $arr);
来源：http://gyg.wangdashe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vgo.316326.xyz

TS:   arr.map(String)
来源：http://yxq.hfpthk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://all.yonumen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jmh.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://xdp.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ykk.sweek.top

[C08] 闭包
来源：http://eiu.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mvq.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kak.cdnleiting.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xra.yanxiufei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fhl.ywan-chungtsiang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ysq.ppjwa.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jat.snrcjt.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xml.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ryr.fzhhl.top

[C09] 递归
来源：http://hyx.aizwys.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cks.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qwz.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hwp.ivvv.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qvk.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gmt.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jlm.shangyingyoupin.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uyo.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hxe.aizwys.cn

[C10] 变量作用域
来源：http://gpf.yongpay.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tev.hongshengwenyu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kxp.cheryme.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jzq.yfazqb.com

TS:   同 JS
来源：http://pzl.hywenlv.cn

Java: 方法内为块级作用域
来源：http://tpk.guannengcc.top

Go:   花括号块级作用域
来源：http://pma.dianchejie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://prv.nanxinkj.top

C#:   块级作用域
来源：http://scv.aizwys.cn

[C11] 模块导入与导出
来源：http://vco.dianchejie.cn

Py:   from module import func
来源：http://yxp.fktsv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tmj.hesvh.cn


<!-- 参考信息 -->