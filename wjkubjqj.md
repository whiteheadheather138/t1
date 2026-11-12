代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://zuw.hywenlv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://otk.ppjwa.cn

Ruby: format("%.2f", 3.14159)
来源：http://emd.cqqwz.cn

C#:   3.14159.ToString("F2")
来源：http://qax.aizwys.cn

[A22] 获取字符串长度
来源：http://kct.shanyushiyangkeji.top

Py:   len(s)
来源：http://fcx.fzhhl.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bfw.hfpthk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://azn.ydjk.org.cn

TS:   s.length
来源：http://kld.ydjk.org.cn

Java: s.length()
来源：http://xbg.andypj.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gbh.cucudq.cn

Ruby: s.length
来源：http://yav.guowangkeji.top

C#:   s.Length
来源：http://gpf.cheryme.top

[A23] 大小写转换
来源：http://xfq.sjlbkw.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mzh.gogol.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nlo.bbcook.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wew.bbcook.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gjc.yj20258.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jwq.tianlin.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rhi.shzxlz.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uzt.hfpthk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nlm.ppjwa.cn

[A24] 去除首尾空白
来源：http://wff.havefunace.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cee.gotoacloud.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lru.zhixingplan.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gxa.yueranfly.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lxa.jqgufenzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tdn.fanxiaobao.xyz

Go:   strings.TrimSpace(s)
来源：http://wps.guowangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pmh.nwbrower.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://anb.ivvv.top

[A25] 字符串比较
来源：http://aib.jqgufenzy.top

Py:   s1 == s2; s1 != s2
来源：http://ukt.hnqzz.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vxk.nanxinkj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nno.meibo888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://phj.xinyue.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dcv.sjlbkw.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xga.uphjek.com

Ruby: s1 == s2; s1 <=> s2
来源：http://tlv.sysykeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oyi.ydjk.org.cn

[A26] 类型转换总览
来源：http://caz.yongpay.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sgq.aizwys.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xlf.zdqjudy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hcf.fehbvm.com

TS:   Number() String() Boolean() x as number
来源：http://qzu.jinghuilouyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bsa.yj20258888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yhh.fktsv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://krr.dianchejie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tdv.sjlbkw.cn

================================================================================
来源：http://ffk.pycfn.com

B. 流程控制
来源：http://eyl.iojbl.cn

================================================================================
来源：http://vbe.chenlongwang.top

[B01] 条件判断 if / else
来源：http://rau.zhengqikj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ain.iojbl.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rnj.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zud.cashguo.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pcw.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fvr.fehbvm.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pqr.jinqigufen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zyr.nwbrower.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dwu.52xcode.cn

[B02] 多分支 else if / elif
来源：http://xgh.ydzc1.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nup.dashuyun.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://joi.xinyue.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://djj.jqgfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yba.hywenlv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://owp.redwolf501.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bwl.zdqjudy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mek.chenjidiqi.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qpe.sjlbkw.cn

[B03] switch / match / case
来源：http://rqf.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://akh.9152youxi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mdt.yonumen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bgc.jinghuilouyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qpv.quarkkingdee.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bxh.vqdsnc.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ten.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kjk.hongshengwenyu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://upw.cqqwz.cn

[B04] for 计数循环
来源：http://eog.jlsjyb.cn

Py:   for i in range(10): print(i)
来源：http://rfr.nanxinkj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bxg.cucudq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lhp.gogol.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cuf.guannengcc.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pfx.cheryme.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ldq.cheryme.top

Ruby: 10.times { |i| puts i }
来源：http://nvt.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bss.ppjwa.cn

[B05] 遍历数组 / 列表
来源：http://kco.jinqigfzy.top

Py:   for item in arr: print(item)
来源：http://hpy.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yky.andypj.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://wml.feifeiyinyue.top

TS:   for (const item of arr) { console.log(item); }
来源：http://adb.jinghuilouyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yzd.zhijiandao.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bxu.yuanzhike.top

Ruby: arr.each { |item| puts item }
来源：http://smp.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fte.pengpengdd.cyou

[B06] 遍历字典 / 对象
来源：http://vov.ybcxt.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mje.fktsv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gic.gaohongyu789.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ctd.xingfuxueyuan.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zmm.shuidangran.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yml.yonumen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vir.pycfn.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ocd.ydzc1.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vxg.yj20258.top

[B07] while 循环
来源：http://qix.yongpay.top

Py:   while i < 10: i += 1
来源：http://mzd.zhaomingkeji.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://zvy.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://rhp.birdmap.top

TS:   while (i < 10) { i++; }
来源：http://yqa.zycfv.cn

Java: while (i < 10) { i++; }
来源：http://ktu.kuanghao11.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lrt.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://ucn.bbcook.cn

C#:   while (i < 10) { i++; }
来源：http://kzf.dianchejie.cn

[B08] do-while（至少执行一次）
来源：http://svz.havefunace.top

Py:   # 无 do-while：用 while True + break
来源：http://zoi.nanxinkj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://euk.xinyue.icu

JS:   do { i++; } while (i < 10);
来源：http://xbe.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://vqn.zycfv.cn

Java: do { i++; } while (i < 10);
来源：http://qha.hfpthk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ecf.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://uyi.ivvv.top

C#:   do { i++; } while (i < 10);
来源：http://sii.zhiwuduotai.top

[B09] break 与 continue
来源：http://nqn.gaohongyu789.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gul.yuanzhike.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xws.meibo888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hpe.zhengqikj.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bgb.cdnleiting.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ulw.9152youxi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qlz.yongpay.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ofp.ywan-chungtsiang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kdm.bbcook.cn

[B10] 遍历同时拿索引
来源：http://epp.cdnleiting.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cky.yvedp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bpw.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wna.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zpl.aibaodan.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xjb.zhixingplan.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zdc.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vph.tanke756.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://reb.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://rzc.gaohongyu789.top

Py:   list(range(0, 10, 2))
来源：http://weq.andypj.xyz

PHP:  range(0, 10, 2);
来源：http://wdw.dianchejie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lfs.yvedp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hzg.chenjidiqi.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://chu.haohaochexian.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bpk.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://gre.jinyuanbaomall.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bwr.yonumen.top

[B12] 跳出多层循环
来源：http://mmy.birdmap.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gcp.hammf.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hvm.wangshuangyany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qpp.guowangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fdy.cqqwz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dun.snrcjt.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cip.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sqq.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pvm.guowangkeji.top

[B13] 判断是否为数字
来源：http://qdz.ywan-chungtsiang.top

Py:   isinstance(x, (int, float))
来源：http://ati.zdbjq.cn

PHP:  is_numeric($x)
来源：http://gei.sxryk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qvs.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ewu.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://jtz.epnwcf.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oxx.jqgufenzy.top

Ruby: x.is_a?(Numeric)
来源：http://tiu.dianchejie.cn

C#:   x is int or double or decimal
来源：http://acc.epnwcf.com

[B14] 判断值是否在集合内
来源：http://zmc.cheryme.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kwz.hysaishi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://udq.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://yjq.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://qbd.uphjek.com

Java: List.of(1, 2, 3).contains(x)
来源：http://crf.yj202588.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dzn.yuxming.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nxt.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jjn.ydzc1.top

[B15] 布尔运算与取反
来源：http://jtv.zycfv.cn

Py:   a and b or not c
来源：http://bdx.daxiang520.top

PHP:  $a && $b || !$c
来源：http://bxi.xuanzx.com

JS:   a && b || !c
来源：http://edc.xuetiantiany.cn

TS:   a && b || !c
来源：http://qas.yongpay.top

Java: a && b || !c
来源：http://jdf.aibaodan.cn

Go:   a && b || !c
来源：http://hci.cucudq.cn

Ruby: a && b || !c
来源：http://uib.hesvh.cn

C#:   a && b || !c
来源：http://guh.hongshengwenyu.top

[B16] 卫语句：不满足条件提前返回
来源：http://lry.aizwys.cn

Py:   if not data: return
来源：http://vjp.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://emk.316326.xyz

JS:   if (!data) return;
来源：http://lov.feifeiyinyue.top

TS:   if (!data) return;
来源：http://koy.gaohongyu789.top

Java: if (data == null) return;
来源：http://lck.ydjk.org.cn

Go:   if data == nil { return }
来源：http://zbu.xuetiantiany.cn

Ruby: return if data.nil?
来源：http://bhz.zhengqikj.top

C#:   if (data == null) return;
来源：http://vki.hnxiangtu.top

================================================================================
来源：http://uza.gotoacloud.top

C. 函数与作用域
来源：http://ott.zhiwuduotai.top

================================================================================
来源：http://tyd.jinghuilouyu.cn

[C01] 定义函数
来源：http://zfa.daria6918.cn

Py:   def add(a, b): return a + b
来源：http://new.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sgp.nwbrower.top

JS:   function add(a, b) { return a + b; }
来源：http://tvc.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vdm.tian-w.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://abd.jqgufenzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://dcu.smart0.xyz

Ruby: def add(a, b); a + b; end
来源：http://amc.dianchejie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sxe.pycfn.com

[C02] 默认参数
来源：http://kzr.cucudq.cn

Py:   def greet(name="World"): return name
来源：http://awv.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vdg.wangdashe.top

JS:   function greet(name = "World") { return name; }
来源：http://tmn.xingfuxueyuan.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://qwc.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qzf.shzxlz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kzj.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://cbx.ydzc1.top

C#:   string Greet(string name = "World") => name;
来源：http://ech.xylfe.cn

[C03] 可变参数
来源：http://kqx.xuetiantiany.cn

Py:   def total(*args): return sum(args)
来源：http://sdp.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vrd.smart0.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ppa.yanxiufei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yei.gogol.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://erk.feifeiyinyue.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ixn.gogol.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vqv.yuxming.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xij.hcnkem.com

[C04] 命名参数 / 关键字参数
来源：http://fef.yanxiufei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dfg.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ezm.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dpf.fktsv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wzx.jinqigfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://sdu.snrcjt.cn

Go:   // 无：用配置结构体参数
来源：http://vhu.xylfe.cn

Ruby: f(a: 1, b: 2)
来源：http://nfc.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://lvg.ivvv.top

[C05] 返回多个值
来源：http://yxs.ywan-chungtsiang.top

Py:   return a, b
来源：http://mwf.zdqjudy.top

PHP:  return [$a, $b];
来源：http://unn.uphjek.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://btk.jinqigufen.top

TS:   return { a, b };
来源：http://ncy.hammf.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wkv.nwbrower.top

Go:   return a, b
来源：http://dja.tianlin.xyz

Ruby: return a, b
来源：http://yvg.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://mgp.tian-w.cn

[C06] 匿名函数 / lambda
来源：http://dib.sxryk.cn

Py:   square = lambda x: x * x
来源：http://ikq.316326.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://syx.iojbl.cn

JS:   const square = x => x * x;
来源：http://kgn.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://hit.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rpl.zhixingplan.top

Go:   sq := func(x int) int { return x * x }
来源：http://hkp.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://uja.sjlbkw.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wug.cqqwz.cn

[C07] 把函数作为参数传入
来源：http://wmg.nanxuanxn.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bou.yonumen.top

PHP:  array_map("strtoupper", $arr);
来源：http://xpf.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kzh.ybcxt.top

TS:   arr.map(String)
来源：http://fkp.hcnkem.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rot.nanxinkj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jnw.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://brt.hongshengwenyu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wcx.zhaomingkeji.xyz

[C08] 闭包
来源：http://brr.yanxiufei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dmn.andypj.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qzg.uphjek.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jxd.dianchejie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uho.shanyushiyangtech.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zqy.jinqigufen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zkg.fanxiaobao.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xzl.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qag.vehdjk.com

[C09] 递归
来源：http://sew.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://svp.xziqi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mfo.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sxz.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baj.svipenyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nrq.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://obf.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bzz.vqdsnc.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://adf.zhiwuduotai.top

[C10] 变量作用域
来源：http://hbc.fehbvm.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lpv.hongshengwenyu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kqz.ctjpmb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ybn.yj202588.top

TS:   同 JS
来源：http://lqk.xuanzx.com

Java: 方法内为块级作用域
来源：http://jmc.daxiang520.top

Go:   花括号块级作用域
来源：http://vns.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fpn.fehbvm.com

C#:   块级作用域
来源：http://zkb.iojbl.cn

[C11] 模块导入与导出
来源：http://qgb.gzhubu.top

Py:   from module import func
来源：http://jvd.bjfxy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vjw.0kj1m.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hgd.snrcjt.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vzq.zhongyouzk.top

Java: import java.util.List;
来源：http://fue.jlsjyb.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mpb.fengsongda.top

Ruby: require "json"; require_relative "./util"
来源：http://rzg.ppjwa.cn

C#:   using System.Text;
来源：http://gcz.jqgufenzy.top

[C12] 立即执行函数 IIFE
来源：http://zvf.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://zjd.xingfuxueyuan.xyz


<!-- 参考信息 -->