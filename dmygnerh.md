代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://dag.jinyuanbaomall.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vot.jinyuanbaomall.cn

JS:   (3.14159).toFixed(2)
来源：http://gej.sjlbkw.cn

TS:   (3.14159).toFixed(2)
来源：http://two.zhoulong.xyz

Java: String.format("%.2f", 3.14159)
来源：http://oyf.cdnleiting.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ccz.hammf.cn

Ruby: format("%.2f", 3.14159)
来源：http://blj.nanxinkj.top

C#:   3.14159.ToString("F2")
来源：http://miu.zdbjq.cn

[A22] 获取字符串长度
来源：http://fhw.chenjidiqi.icu

Py:   len(s)
来源：http://clj.zhijiandao.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://smx.shangyingyoupin.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rtk.zhiwuduotai.top

TS:   s.length
来源：http://ere.iojbl.cn

Java: s.length()
来源：http://qfd.zhaomingkeji.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iui.iojbl.cn

Ruby: s.length
来源：http://bgo.zdbjq.cn

C#:   s.Length
来源：http://xrv.yuxming.cn

[A23] 大小写转换
来源：http://prx.pycfn.com

Py:   s.upper(); s.lower(); s.title()
来源：http://zby.zhaomingkeji.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qwu.havefunace.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wme.yongpay.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://egc.redwolf501.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mtt.bbcook.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xpl.tarul.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://skn.aibaodan.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://reu.gzhubu.top

[A24] 去除首尾空白
来源：http://yne.tarul.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bwl.cqqwz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://akk.yongpay.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pqi.yuxming.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://paf.xziqi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wxv.yuxming.cn

Go:   strings.TrimSpace(s)
来源：http://uho.hysaishi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zzi.mhx1999.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zlr.nanxuanxn.top

[A25] 字符串比较
来源：http://oxu.yj20258.top

Py:   s1 == s2; s1 != s2
来源：http://fdq.cashguo.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://goz.tarul.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rbx.zhoulong.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bxw.yvedp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gqn.feifeiyinyue.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xoe.bbcook.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://orh.ppjwa.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sld.tianlin.xyz

[A26] 类型转换总览
来源：http://nlt.cucudq.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eno.ybcxt.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://owz.yongpay.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qki.tanke756.top

TS:   Number() String() Boolean() x as number
来源：http://zfw.redwolf501.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eok.guowangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pxv.c1oappe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://avj.yj20258888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rxr.zdqjudy.top

================================================================================
来源：http://ald.bjfxy.top

B. 流程控制
来源：http://mzp.yuxming.cn

================================================================================
来源：http://msi.yuxming.cn

[B01] 条件判断 if / else
来源：http://qmw.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://hmr.pengpengdd.cyou

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aub.ctjpmb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iob.daria6918.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kcx.bjfxy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://isi.jinyuanbaomall.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gqg.aibaodan.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dge.yongpay.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://krn.jlsjyb.cn

[B02] 多分支 else if / elif
来源：http://iub.xuetiantiany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dct.jinqigfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gim.0kj1m.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dmt.yanxiufei.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yso.yongpay.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://exv.zycfv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gzj.svipenyu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gfn.bbcook.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qcp.52xcode.cn

[B03] switch / match / case
来源：http://cee.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zot.yongpay.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qgw.pengpengdd.cyou

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yrf.wangdashe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yam.dianchejie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ylo.yfazqb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zrb.c1oappe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yoj.uphjek.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zuw.yangfankeji.com

[B04] for 计数循环
来源：http://pyy.smart0.xyz

Py:   for i in range(10): print(i)
来源：http://bjf.hfpthk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uzs.aibaodan.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nwq.0kj1m.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wmz.chenlongwang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zjg.gzhubu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gxc.fzhhl.top

Ruby: 10.times { |i| puts i }
来源：http://jkq.nwbrower.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xcx.yuxming.cn

[B05] 遍历数组 / 列表
来源：http://pdl.hammf.cn

Py:   for item in arr: print(item)
来源：http://bnu.yueranfly.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jvc.mhx1999.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rch.nanxinkj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kmj.vehdjk.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://nad.shanyushiyangtech.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gaq.ydzc1.top

Ruby: arr.each { |item| puts item }
来源：http://piv.hongshengwenyu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mrv.jiagoushi.top

[B06] 遍历字典 / 对象
来源：http://mfu.jyoumei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ncg.tanke756.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://two.svipenyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uqa.aizwys.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bzt.zhiwuduotai.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://php.hysaishi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kcw.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zci.hfpthk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bkn.redwolf501.top

[B07] while 循环
来源：http://czb.jinqigufen.top

Py:   while i < 10: i += 1
来源：http://zcf.hfpthk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oom.pengpengdd.cyou

JS:   while (i < 10) { i++; }
来源：http://njb.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://mrn.hcnkem.com

Java: while (i < 10) { i++; }
来源：http://nys.wangshuangyany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wac.jinyuanbaomall.cn

Ruby: while i < 10; i += 1; end
来源：http://agt.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://irf.jinyuanbaomall.cn

[B08] do-while（至少执行一次）
来源：http://pag.jinqigufen.top

Py:   # 无 do-while：用 while True + break
来源：http://glh.nanxuanxn.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bcy.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://nub.hcnkem.com

TS:   do { i++; } while (i < 10);
来源：http://vlm.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://fsz.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uic.andypj.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://ayt.c1oappe.top

C#:   do { i++; } while (i < 10);
来源：http://ddu.guowangkeji.top

[B09] break 与 continue
来源：http://dym.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://btf.xziqi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ezs.ivvv.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lzu.316326.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hyc.zycfv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://okf.fktsv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dhp.jinyuanbaomall.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rfn.zdqjudy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tzi.nwbrower.top

[B10] 遍历同时拿索引
来源：http://ikz.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gvg.ivvv.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dyo.hongshengwenyu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dnv.jinqigufen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nob.ydzc1.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://syi.havefunace.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://idb.andypj.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ybf.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ony.zhiwuduotai.top

[B11] 生成数字序列 / 区间
来源：http://jao.epnwcf.com

Py:   list(range(0, 10, 2))
来源：http://ijb.9152youxi.cn

PHP:  range(0, 10, 2);
来源：http://rmg.birdmap.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iag.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bmp.dianchejie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sam.dashuyun.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://axg.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://jen.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eai.shuidangran.top

[B12] 跳出多层循环
来源：http://tbd.gzhubu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://job.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://etn.cdnleiting.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cir.0kj1m.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fil.kuanghao11.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wni.fzhhl.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pnw.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xus.zycfv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pck.smart0.xyz

[B13] 判断是否为数字
来源：http://tbu.9152youxi.cn

Py:   isinstance(x, (int, float))
来源：http://mqk.yanxiufei.cn

PHP:  is_numeric($x)
来源：http://fop.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fos.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zhr.uphjek.com

Java: x instanceof Number
来源：http://irf.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lyr.hywenlv.cn

Ruby: x.is_a?(Numeric)
来源：http://eeb.9152youxi.cn

C#:   x is int or double or decimal
来源：http://yji.yueranfly.top

[B14] 判断值是否在集合内
来源：http://qln.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://muy.hammf.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rge.iojbl.cn

JS:   [1, 2, 3].includes(x)
来源：http://kuk.ivvv.top

TS:   [1, 2, 3].includes(x)
来源：http://gre.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qyh.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tfr.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dvv.cashguo.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://arp.smart0.xyz

[B15] 布尔运算与取反
来源：http://evy.yj20258.top

Py:   a and b or not c
来源：http://nxv.hammf.cn

PHP:  $a && $b || !$c
来源：http://yye.yfazqb.com

JS:   a && b || !c
来源：http://czm.yvedp.cn

TS:   a && b || !c
来源：http://oil.ctjpmb.com

Java: a && b || !c
来源：http://opr.zhixingplan.top

Go:   a && b || !c
来源：http://muo.yonumen.top

Ruby: a && b || !c
来源：http://cln.tian-w.cn

C#:   a && b || !c
来源：http://kkk.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mgg.haohaochexian.top

Py:   if not data: return
来源：http://vwm.tian-w.cn

PHP:  if (!$data) { return; }
来源：http://gtp.cashguo.top

JS:   if (!data) return;
来源：http://ecj.cashguo.top

TS:   if (!data) return;
来源：http://woo.hongshengwenyu.top

Java: if (data == null) return;
来源：http://mcb.dianchejie.cn

Go:   if data == nil { return }
来源：http://rcg.yanxiufei.cn

Ruby: return if data.nil?
来源：http://mnh.smart0.xyz

C#:   if (data == null) return;
来源：http://qem.zhiwuduotai.top

================================================================================
来源：http://oxi.cdnleiting.top

C. 函数与作用域
来源：http://eef.fktsv.cn

================================================================================
来源：http://dic.52xcode.cn

[C01] 定义函数
来源：http://sln.316326.xyz

Py:   def add(a, b): return a + b
来源：http://glx.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yks.jqgufenzy.top

JS:   function add(a, b) { return a + b; }
来源：http://piq.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cfu.xinyue.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://euw.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://lbe.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://wld.316326.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hpk.hnxiangtu.top

[C02] 默认参数
来源：http://yks.fanxiaobao.xyz

Py:   def greet(name="World"): return name
来源：http://cux.shangyingyoupin.top

PHP:  function greet($name = "World") { return $name; }
来源：http://uug.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://efs.gogol.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hai.zycfv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://his.snrcjt.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nlo.zhoulong.xyz

Ruby: def greet(name = "World") = name
来源：http://zai.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://ghb.jiagoushi.top

[C03] 可变参数
来源：http://czw.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://qsm.hongshengwenyu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cek.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wwr.c1oappe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mqm.snrcjt.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://voz.cucudq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dzf.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vem.ywan-chungtsiang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xjc.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://nxy.jinqigufen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gae.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://suc.aizwys.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://axl.shangyingyoupin.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ahv.yj20258888.top

Java: // 无：用 Builder 模式或 record
来源：http://eof.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://dvy.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://bzx.vqdsnc.cn

C#:   f(a: 1, b: 2)
来源：http://pfu.yongpay.top

[C05] 返回多个值
来源：http://pdb.hfpthk.cn

Py:   return a, b
来源：http://jez.gogol.net.cn

PHP:  return [$a, $b];
来源：http://ufi.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://afp.ppjwa.cn

TS:   return { a, b };
来源：http://mdc.aizwys.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nae.pengpengdd.cyou

Go:   return a, b
来源：http://yup.aizwys.cn

Ruby: return a, b
来源：http://csg.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://umz.ybcxt.top

[C06] 匿名函数 / lambda
来源：http://ahh.daxiang520.top

Py:   square = lambda x: x * x
来源：http://uwd.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://adr.wangdashe.top

JS:   const square = x => x * x;
来源：http://mnb.hnxiangtu.top

TS:   const square = (x: number): number => x * x;
来源：http://pgo.pycfn.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mbx.pengpengdd.cyou

Go:   sq := func(x int) int { return x * x }
来源：http://yxv.hongshengwenyu.top

Ruby: square = ->(x) { x * x }
来源：http://teh.birdmap.top

C#:   Func<int, int> square = x => x * x;
来源：http://oeo.fktsv.cn

[C07] 把函数作为参数传入
来源：http://vbk.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ujr.jinghuilouyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hpq.9152youxi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cvu.hammf.cn

TS:   arr.map(String)
来源：http://khm.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ptk.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tnd.mhx1999.top

Ruby: arr.map(&:upcase)
来源：http://hgb.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://glz.gaohongyu789.top

[C08] 闭包
来源：http://trx.ppjwa.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://idq.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://txk.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vvb.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zfm.yangfankeji.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tsd.aibaodan.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hbb.daxiang520.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://prd.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://syz.wangshuangyany.cn

[C09] 递归
来源：http://bsw.cheryme.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fda.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bes.vqdsnc.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aut.zdbjq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qhw.yj20258.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dcm.dashuyun.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ena.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://emi.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://btj.chenlongwang.top

[C10] 变量作用域
来源：http://zgh.yfazqb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tnf.havefunace.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jsi.ehwqpu.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ojb.ctjpmb.com

TS:   同 JS
来源：http://icy.9152youxi.cn

Java: 方法内为块级作用域
来源：http://nlh.jinqigufen.top

Go:   花括号块级作用域
来源：http://jbo.gotoacloud.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bem.yanxiufei.cn

C#:   块级作用域
来源：http://jty.shzxlz.cn

[C11] 模块导入与导出
来源：http://jem.fanxiaobao.xyz

Py:   from module import func
来源：http://ylc.nwbrower.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ytp.jlsjyb.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dub.ehwqpu.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dzb.cdnleiting.top

Java: import java.util.List;
来源：http://eng.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://knz.jinyuanbaomall.cn


<!-- 参考信息 -->