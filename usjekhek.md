代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cbc.sufxvd.cn

Ruby: gets.chomp
来源：http://avh.hammf.cn

C#:   Console.ReadLine();
来源：http://lql.gzhubu.top

[A21] 保留指定小数位输出
来源：http://coy.ybcxt.top

Py:   f"{3.14159:.2f}"
来源：http://mjl.svipenyu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bsn.hongshengwenyu.top

JS:   (3.14159).toFixed(2)
来源：http://fte.yongpay.top

TS:   (3.14159).toFixed(2)
来源：http://kuo.yfazqb.com

Java: String.format("%.2f", 3.14159)
来源：http://ijb.0kj1m.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rjn.yonumen.top

Ruby: format("%.2f", 3.14159)
来源：http://ddh.kuanghao11.cn

C#:   3.14159.ToString("F2")
来源：http://ubk.nanxinkj.top

[A22] 获取字符串长度
来源：http://vvt.gotoacloud.top

Py:   len(s)
来源：http://fjm.hnqzz.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ixp.yangfankeji.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ken.chenlongwang.top

TS:   s.length
来源：http://ipn.vqdsnc.cn

Java: s.length()
来源：http://voa.yongpay.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ksi.svipenyu.cn

Ruby: s.length
来源：http://oqw.hnxiangtu.top

C#:   s.Length
来源：http://xxs.vqdsnc.cn

[A23] 大小写转换
来源：http://kqr.fengsongda.top

Py:   s.upper(); s.lower(); s.title()
来源：http://lll.guannengcc.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fpm.cdnleiting.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vrc.chenjidiqi.icu

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nnr.zhixingplan.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ycc.fehbvm.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jak.redwolf501.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kpu.jinqigfzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ynw.ehwqpu.com

[A24] 去除首尾空白
来源：http://kwn.kuanghao11.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wgk.mhx1999.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rvg.zycfv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jvb.sweek.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dpy.pengpengdd.cyou

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jop.yj20258.top

Go:   strings.TrimSpace(s)
来源：http://ioa.smart0.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ydu.iojbl.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kci.shanyushiyangtech.top

[A25] 字符串比较
来源：http://ikr.zhiwuduotai.top

Py:   s1 == s2; s1 != s2
来源：http://zua.aibaodan.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://taz.wangshuangyany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hws.kuanghao11.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ery.sweek.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://seo.ctjpmb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://slx.zhaomingkeji.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://hcj.yfazqb.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://plj.tanke756.top

[A26] 类型转换总览
来源：http://gfs.fehbvm.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lbn.jlsjyb.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jti.cashguo.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eyb.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://ghe.quarkkingdee.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ygm.yfazqb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jpb.yongpay.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dfx.kuanghao11.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ayl.fzhhl.top

================================================================================
来源：http://hax.xuetiantiany.cn

B. 流程控制
来源：http://qyi.meibo888.top

================================================================================
来源：http://lta.cashguo.top

[B01] 条件判断 if / else
来源：http://mfe.cashguo.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vhn.yuanzhike.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lth.316326.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ama.svipenyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hrt.ehwqpu.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://vrl.iojbl.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mwa.daxiang520.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://raj.dashuyun.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xre.hammf.cn

[B02] 多分支 else if / elif
来源：http://ala.meibo888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qhc.yj20258888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ksq.hongshengwenyu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xwv.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xox.fzhhl.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tte.nanxinkj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://siq.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fsn.nwbrower.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pam.sjlbkw.cn

[B03] switch / match / case
来源：http://ket.fehbvm.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cwc.epnwcf.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bsf.jqgfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xmd.yj20258.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kei.haohaochexian.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ipl.sxryk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zdx.tanke756.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rlx.cdnleiting.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lsx.fktsv.cn

[B04] for 计数循环
来源：http://qdn.yongpay.top

Py:   for i in range(10): print(i)
来源：http://zax.fzhhl.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gad.shzxlz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lco.gogol.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jjl.ctjpmb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aqd.chenzaomai.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oxi.gogol.net.cn

Ruby: 10.times { |i| puts i }
来源：http://dve.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yil.daxiang520.top

[B05] 遍历数组 / 列表
来源：http://atn.shanyushiyangkeji.top

Py:   for item in arr: print(item)
来源：http://ffr.hongshengwenyu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wmh.redwolf501.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dva.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://lcr.sweek.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://btl.pycfn.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rpq.ivvv.top

Ruby: arr.each { |item| puts item }
来源：http://pva.fanxiaobao.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yyn.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://rdf.zhiwuduotai.top

Py:   for k, v in d.items(): print(k, v)
来源：http://azb.zhaomingkeji.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zud.dianchejie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nzu.ywan-chungtsiang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kmv.ctjpmb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wje.hesvh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pme.yfazqb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nxo.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bnp.vehdjk.com

[B07] while 循环
来源：http://jxn.0kj1m.cn

Py:   while i < 10: i += 1
来源：http://prz.ehwqpu.com

PHP:  while ($i < 10) { $i++; }
来源：http://wlo.guannengcc.top

JS:   while (i < 10) { i++; }
来源：http://yuy.zhiwuduotai.top

TS:   while (i < 10) { i++; }
来源：http://mrt.hysaishi.cn

Java: while (i < 10) { i++; }
来源：http://sas.yuanzhike.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fbr.zhongyouzk.top

Ruby: while i < 10; i += 1; end
来源：http://omg.jinyuanbaomall.cn

C#:   while (i < 10) { i++; }
来源：http://bpq.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://zpz.vehdjk.com

Py:   # 无 do-while：用 while True + break
来源：http://suj.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cca.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://aql.ppjwa.cn

TS:   do { i++; } while (i < 10);
来源：http://qrf.cqqwz.cn

Java: do { i++; } while (i < 10);
来源：http://uth.c1oappe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://omc.aibaodan.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fdy.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://ddw.vqdsnc.cn

[B09] break 与 continue
来源：http://zwb.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pxb.pengpengdd.cyou

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ccp.zdqjudy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bdc.tarul.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dkf.jlsjyb.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gmi.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://amf.cheryme.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://poy.shanyushiyangtech.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yvi.hongshengwenyu.top

[B10] 遍历同时拿索引
来源：http://mfu.52xcode.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://edf.yfazqb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tst.aibaodan.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bca.zhixingplan.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eau.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zxk.jinqigufen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yin.hongshengwenyu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sam.xylfe.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fid.zhongyouzk.top

[B11] 生成数字序列 / 区间
来源：http://kip.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://pla.dashuyun.cn

PHP:  range(0, 10, 2);
来源：http://dbn.zdbjq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cmp.yuanzhike.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dfw.kuanghao11.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dmf.ppjwa.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jft.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://hmo.yfazqb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aay.bjfxy.top

[B12] 跳出多层循环
来源：http://lpa.svipenyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jtn.cheryme.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xni.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://odp.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mdr.ydzc1.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://znb.dashuyun.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sqx.bjfxy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mqi.zdqjudy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cii.yonumen.top

[B13] 判断是否为数字
来源：http://fxo.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://kqp.cucudq.cn

PHP:  is_numeric($x)
来源：http://omf.ybcxt.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lfd.aibaodan.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xah.tianlin.xyz

Java: x instanceof Number
来源：http://oeg.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://and.feifeiyinyue.top

Ruby: x.is_a?(Numeric)
来源：http://pgj.jqgfzy.top

C#:   x is int or double or decimal
来源：http://uoc.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://edi.jinyuanbaomall.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ubr.gzhubu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uwr.daria6918.cn

JS:   [1, 2, 3].includes(x)
来源：http://xrx.zhaomingkeji.xyz

TS:   [1, 2, 3].includes(x)
来源：http://yer.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://omo.zycfv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cpj.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://exo.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rah.chenzaomai.com

[B15] 布尔运算与取反
来源：http://mid.sxryk.cn

Py:   a and b or not c
来源：http://zko.jqgufenzy.top

PHP:  $a && $b || !$c
来源：http://rta.zdbjq.cn

JS:   a && b || !c
来源：http://ueh.meibo888.top

TS:   a && b || !c
来源：http://qit.jinqigfzy.top

Java: a && b || !c
来源：http://shp.xylfe.cn

Go:   a && b || !c
来源：http://gmb.pengpengdd.cyou

Ruby: a && b || !c
来源：http://rzq.uphjek.com

C#:   a && b || !c
来源：http://sos.yuanzhike.top

[B16] 卫语句：不满足条件提前返回
来源：http://rjb.jyoumei.cn

Py:   if not data: return
来源：http://mms.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://kvd.zhoulong.xyz

JS:   if (!data) return;
来源：http://sss.zhixingplan.top

TS:   if (!data) return;
来源：http://ovy.316326.xyz

Java: if (data == null) return;
来源：http://oks.zhengqikj.top

Go:   if data == nil { return }
来源：http://uid.yuanzhike.top

Ruby: return if data.nil?
来源：http://xwa.cashguo.top

C#:   if (data == null) return;
来源：http://pvo.tian-w.cn

================================================================================
来源：http://mhe.svipenyu.cn

C. 函数与作用域
来源：http://ugs.jlsjyb.cn

================================================================================
来源：http://ire.quarkkingdee.top

[C01] 定义函数
来源：http://zid.birdmap.top

Py:   def add(a, b): return a + b
来源：http://jbj.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://usv.jiagoushi.top

JS:   function add(a, b) { return a + b; }
来源：http://bvr.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ukd.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://aqe.wangshuangyany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lbn.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://zig.chenzaomai.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://inj.yongpay.top

[C02] 默认参数
来源：http://asw.haohaochexian.top

Py:   def greet(name="World"): return name
来源：http://xiv.vqdsnc.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vvh.jinqigufen.top

JS:   function greet(name = "World") { return name; }
来源：http://jak.tanke756.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yge.c1oappe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hba.snrcjt.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yqh.hammf.cn

Ruby: def greet(name = "World") = name
来源：http://cih.316326.xyz

C#:   string Greet(string name = "World") => name;
来源：http://zdy.gzhubu.top

[C03] 可变参数
来源：http://msj.c1oappe.top

Py:   def total(*args): return sum(args)
来源：http://zsi.aibaodan.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bnc.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bon.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jkc.gogol.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nve.shanyushiyangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mjj.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://quh.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jiw.xinyue.icu

[C04] 命名参数 / 关键字参数
来源：http://bbk.gogol.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kdq.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qbk.ivvv.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wyv.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lbm.9152youxi.cn

Java: // 无：用 Builder 模式或 record
来源：http://sey.sufxvd.cn

Go:   // 无：用配置结构体参数
来源：http://dap.haohaochexian.top

Ruby: f(a: 1, b: 2)
来源：http://okq.shangyingyoupin.top

C#:   f(a: 1, b: 2)
来源：http://ron.jyoumei.cn

[C05] 返回多个值
来源：http://oud.cashguo.top

Py:   return a, b
来源：http://tgj.sufxvd.cn

PHP:  return [$a, $b];
来源：http://wei.tian-w.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pcm.cashguo.top

TS:   return { a, b };
来源：http://ipa.chenlongwang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kkj.guowangkeji.top

Go:   return a, b
来源：http://kvs.yj202588.top

Ruby: return a, b
来源：http://qqj.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://qmc.epnwcf.com

[C06] 匿名函数 / lambda
来源：http://qgb.yfazqb.com

Py:   square = lambda x: x * x
来源：http://ivq.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qaa.c1oappe.top

JS:   const square = x => x * x;
来源：http://gsl.tian-w.cn

TS:   const square = (x: number): number => x * x;
来源：http://yxo.sjlbkw.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fuo.smart0.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://sfd.zhengqikj.top

Ruby: square = ->(x) { x * x }
来源：http://vjx.xziqi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://udo.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://qwt.quarkkingdee.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zvv.yanxiufei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lhi.yvedp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kdc.havefunace.top

TS:   arr.map(String)
来源：http://rpi.9152youxi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aon.cdnleiting.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qqa.andypj.xyz

Ruby: arr.map(&:upcase)
来源：http://dao.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kfj.xingfuxueyuan.xyz

[C08] 闭包
来源：http://cxl.feifeiyinyue.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://war.yvedp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cjm.mhx1999.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mfd.gaohongyu789.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tej.hnxiangtu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jqv.smart0.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oob.smart0.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eyv.quarkkingdee.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fdu.pycfn.com

[C09] 递归
来源：http://kyh.gzhubu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pdp.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qib.sweek.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oet.zdqjudy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vds.jinqigufen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dqs.bjfxy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gtm.chenjidiqi.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cem.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://enj.zdqjudy.top

[C10] 变量作用域
来源：http://lsp.yangfankeji.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hqq.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vbb.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mpi.nanxinkj.top

TS:   同 JS
来源：http://kib.jiagoushi.top

Java: 方法内为块级作用域
来源：http://muo.jinyuanbaomall.cn

Go:   花括号块级作用域
来源：http://wjk.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sit.hongshengwenyu.top

C#:   块级作用域
来源：http://spt.aibaodan.cn

[C11] 模块导入与导出
来源：http://ddq.dashuyun.cn

Py:   from module import func
来源：http://qid.nanxuanxn.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tli.316326.xyz


<!-- 参考信息 -->