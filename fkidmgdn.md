代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://pbb.xuetiantiany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bww.daxiang520.top

Ruby: format("%.2f", 3.14159)
来源：http://hsn.cashguo.top

C#:   3.14159.ToString("F2")
来源：http://ysz.cheryme.top

[A22] 获取字符串长度
来源：http://gtg.yj202588.top

Py:   len(s)
来源：http://yso.kuanghao11.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hex.fanxiaobao.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pct.yuxming.cn

TS:   s.length
来源：http://wdq.hcnkem.com

Java: s.length()
来源：http://lvd.ywan-chungtsiang.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uaj.shangyingyoupin.top

Ruby: s.length
来源：http://dsg.vqdsnc.cn

C#:   s.Length
来源：http://lid.jyoumei.cn

[A23] 大小写转换
来源：http://kon.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://apw.fanxiaobao.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xuw.yj20258888.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gzk.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zpi.cheryme.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kkp.dashuyun.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kwv.redwolf501.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lqf.andypj.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://wta.cdnleiting.top

[A24] 去除首尾空白
来源：http://ljx.cqqwz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bsf.yvedp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sdd.cdnleiting.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ejl.hesvh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bic.yangfankeji.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pzt.jinqigfzy.top

Go:   strings.TrimSpace(s)
来源：http://wxk.bjfxy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qdl.chenjidiqi.icu

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oln.shzxlz.cn

[A25] 字符串比较
来源：http://cuk.fktsv.cn

Py:   s1 == s2; s1 != s2
来源：http://xmk.jlsjyb.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aob.chenlongwang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lpz.ybcxt.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mfi.redwolf501.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fxb.52xcode.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rak.cucudq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ood.yj20258.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ifv.xinyue.icu

[A26] 类型转换总览
来源：http://fdx.tianlin.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bsj.uphjek.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wdz.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dlb.aizwys.cn

TS:   Number() String() Boolean() x as number
来源：http://wkn.yongpay.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vku.andypj.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pwh.kuanghao11.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zbs.tanke756.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uzx.wangshuangyany.cn

================================================================================
来源：http://uxb.fengsongda.top

B. 流程控制
来源：http://zoe.hammf.cn

================================================================================
来源：http://kcw.cashguo.top

[B01] 条件判断 if / else
来源：http://cue.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nlz.birdmap.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vlc.jlsjyb.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yxh.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uid.yfazqb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://gnr.sweek.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jxo.aibaodan.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://smn.hesvh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kjg.yfazqb.com

[B02] 多分支 else if / elif
来源：http://tdn.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qbd.jinghuilouyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vhl.yj20258888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mer.birdmap.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mpp.jinghuilouyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cfq.hysaishi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uno.cashguo.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uwz.haohaochexian.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vgt.jinqigfzy.top

[B03] switch / match / case
来源：http://sqn.0kj1m.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qyr.bbcook.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qll.redwolf501.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://drf.daria6918.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wly.jinyuanbaomall.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pbe.jlsjyb.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mnu.meibo888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jgk.meibo888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rmh.xuanzx.com

[B04] for 计数循环
来源：http://duh.yj20258.top

Py:   for i in range(10): print(i)
来源：http://wfu.hnqzz.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yaa.dianchejie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fhy.ctjpmb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tws.xuetiantiany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wye.hywenlv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wkr.ppjwa.cn

Ruby: 10.times { |i| puts i }
来源：http://huy.yuxming.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://foc.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://efx.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://llh.tianlin.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://brz.chenjidiqi.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://mmr.zhoulong.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://lpt.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://lyu.jinghuilouyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kjp.meibo888.top

Ruby: arr.each { |item| puts item }
来源：http://aod.tianlin.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ekx.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://rsm.cucudq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dkf.jqgfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ksl.316326.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://udk.ivvv.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uek.ctjpmb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qlp.0kj1m.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xon.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://btn.dianchejie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tnw.jinqigufen.top

[B07] while 循环
来源：http://dzj.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://gmn.tanke756.top

PHP:  while ($i < 10) { $i++; }
来源：http://xiv.hongshengwenyu.top

JS:   while (i < 10) { i++; }
来源：http://owp.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://jkv.xinyue.icu

Java: while (i < 10) { i++; }
来源：http://eqj.fehbvm.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gsg.sjlbkw.cn

Ruby: while i < 10; i += 1; end
来源：http://sdz.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://kgm.cqqwz.cn

[B08] do-while（至少执行一次）
来源：http://gps.shanyushiyangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://bam.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://prc.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://gai.9152youxi.cn

TS:   do { i++; } while (i < 10);
来源：http://iqo.zhoulong.xyz

Java: do { i++; } while (i < 10);
来源：http://dcj.zycfv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://txa.hysaishi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ytu.c1oappe.top

C#:   do { i++; } while (i < 10);
来源：http://aef.wangdashe.top

[B09] break 与 continue
来源：http://jnw.fktsv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nqm.shuidangran.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ndj.aizwys.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oyb.hesvh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cht.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cyn.jiagoushi.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hym.yuanzhike.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gry.yuxming.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hxe.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://swe.9152youxi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aex.hysaishi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://isq.chenzaomai.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://aby.zhixingplan.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://udw.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zpi.yuanzhike.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ddr.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eyw.svipenyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vto.ivvv.top

[B11] 生成数字序列 / 区间
来源：http://uug.jiagoushi.top

Py:   list(range(0, 10, 2))
来源：http://uyu.jinqigufen.top

PHP:  range(0, 10, 2);
来源：http://ggl.yvedp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jdi.cucudq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vmh.yj20258888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zcb.yonumen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cbp.daria6918.cn

Ruby: (0...10).step(2).to_a
来源：http://wuh.aibaodan.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sgc.daxiang520.top

[B12] 跳出多层循环
来源：http://frp.0kj1m.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pwd.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pnx.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xnr.jinqigfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rij.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mvc.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cwq.ydzc1.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://smy.ehwqpu.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://izk.tian-w.cn

[B13] 判断是否为数字
来源：http://rzs.andypj.xyz

Py:   isinstance(x, (int, float))
来源：http://rwb.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://bjt.pengpengdd.cyou

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zqw.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oby.jlsjyb.cn

Java: x instanceof Number
来源：http://omz.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oge.hongshengwenyu.top

Ruby: x.is_a?(Numeric)
来源：http://bge.zhaomingkeji.xyz

C#:   x is int or double or decimal
来源：http://bjj.redwolf501.top

[B14] 判断值是否在集合内
来源：http://arz.cashguo.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tnm.haohaochexian.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cdj.hammf.cn

JS:   [1, 2, 3].includes(x)
来源：http://wfg.guannengcc.top

TS:   [1, 2, 3].includes(x)
来源：http://wqf.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://foy.bbcook.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ldh.hammf.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fdj.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://auu.hywenlv.cn

[B15] 布尔运算与取反
来源：http://kyu.birdmap.top

Py:   a and b or not c
来源：http://ltp.guannengcc.top

PHP:  $a && $b || !$c
来源：http://kod.xuanzx.com

JS:   a && b || !c
来源：http://mix.jinyuanbaomall.cn

TS:   a && b || !c
来源：http://vsq.gogol.net.cn

Java: a && b || !c
来源：http://yye.nanxinkj.top

Go:   a && b || !c
来源：http://ygk.dianchejie.cn

Ruby: a && b || !c
来源：http://pdt.zhiwuduotai.top

C#:   a && b || !c
来源：http://yep.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://axh.sufxvd.cn

Py:   if not data: return
来源：http://vka.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://nhu.nanxinkj.top

JS:   if (!data) return;
来源：http://kvj.jinqigufen.top

TS:   if (!data) return;
来源：http://hfa.yj20258.top

Java: if (data == null) return;
来源：http://xhx.sxryk.cn

Go:   if data == nil { return }
来源：http://srk.mhx1999.top

Ruby: return if data.nil?
来源：http://vbj.hywenlv.cn

C#:   if (data == null) return;
来源：http://whi.sysykeji.top

================================================================================
来源：http://olc.chenzaomai.com

C. 函数与作用域
来源：http://huy.ydjk.org.cn

================================================================================
来源：http://sju.haohaochexian.top

[C01] 定义函数
来源：http://esq.cashguo.top

Py:   def add(a, b): return a + b
来源：http://zje.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iuj.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://oxa.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qcg.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hrv.daxiang520.top

Go:   func add(a, b int) int { return a + b }
来源：http://mdl.vehdjk.com

Ruby: def add(a, b); a + b; end
来源：http://nyh.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jgw.wangdashe.top

[C02] 默认参数
来源：http://fjb.c1oappe.top

Py:   def greet(name="World"): return name
来源：http://jyc.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://daq.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://ahi.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ebz.zhixingplan.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tkb.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ovj.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://tmm.316326.xyz

C#:   string Greet(string name = "World") => name;
来源：http://zjf.aizwys.cn

[C03] 可变参数
来源：http://bwy.hfpthk.cn

Py:   def total(*args): return sum(args)
来源：http://eeh.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lwl.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bsl.nwbrower.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gxw.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ocl.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qtr.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rig.feifeiyinyue.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zdc.xingfuxueyuan.xyz

[C04] 命名参数 / 关键字参数
来源：http://wxg.fzhhl.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dys.jlsjyb.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jks.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lrf.tanke756.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xqx.xingfuxueyuan.xyz

Java: // 无：用 Builder 模式或 record
来源：http://chh.sjlbkw.cn

Go:   // 无：用配置结构体参数
来源：http://bks.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://ewt.yangfankeji.com

C#:   f(a: 1, b: 2)
来源：http://tcw.kuanghao11.cn

[C05] 返回多个值
来源：http://gew.quarkkingdee.top

Py:   return a, b
来源：http://aur.shangyingyoupin.top

PHP:  return [$a, $b];
来源：http://dci.hysaishi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oav.zhiwuduotai.top

TS:   return { a, b };
来源：http://nrx.cucudq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vff.sweek.top

Go:   return a, b
来源：http://obg.vehdjk.com

Ruby: return a, b
来源：http://lrf.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://jdy.fengsongda.top

[C06] 匿名函数 / lambda
来源：http://fkk.jlsjyb.cn

Py:   square = lambda x: x * x
来源：http://okb.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jvk.jqgfzy.top

JS:   const square = x => x * x;
来源：http://hdw.yj20258888.top

TS:   const square = (x: number): number => x * x;
来源：http://byu.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://grf.pengpengdd.cyou

Go:   sq := func(x int) int { return x * x }
来源：http://azx.tian-w.cn

Ruby: square = ->(x) { x * x }
来源：http://vty.ybcxt.top

C#:   Func<int, int> square = x => x * x;
来源：http://wxt.zhaomingkeji.xyz

[C07] 把函数作为参数传入
来源：http://fjh.sxryk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jmv.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://itl.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jex.xinyue.icu

TS:   arr.map(String)
来源：http://dxe.zhongyouzk.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zlx.iojbl.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://awn.shanyushiyangkeji.top

Ruby: arr.map(&:upcase)
来源：http://ecz.ehwqpu.com

C#:   arr.Select(s => s.ToUpper())
来源：http://pdw.yvedp.cn

[C08] 闭包
来源：http://zjt.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qqy.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vgr.chenzaomai.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uov.dianchejie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dgv.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yvr.dianchejie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://viy.bjfxy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zjl.hysaishi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oeb.smart0.xyz

[C09] 递归
来源：http://qyg.ybcxt.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vfv.gaohongyu789.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vcm.jinghuilouyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gce.cheryme.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yea.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dmj.sufxvd.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fju.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://btz.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jgv.gaohongyu789.top

[C10] 变量作用域
来源：http://czv.shzxlz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dro.hysaishi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wfa.jianghu66.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bfm.smart0.xyz

TS:   同 JS
来源：http://jaa.ydzc1.top

Java: 方法内为块级作用域
来源：http://dxe.andypj.xyz

Go:   花括号块级作用域
来源：http://zyh.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gmi.yfazqb.com

C#:   块级作用域
来源：http://iln.epnwcf.com

[C11] 模块导入与导出
来源：http://wgz.c1oappe.top

Py:   from module import func
来源：http://aek.uphjek.com

PHP:  require "file.php";  或 use App\Service;
来源：http://nsd.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://dkr.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ejz.cheryme.top

Java: import java.util.List;
来源：http://spl.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hah.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://bui.meibo888.top

C#:   using System.Text;
来源：http://lda.jqgfzy.top

[C12] 立即执行函数 IIFE
来源：http://zng.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://icn.wangshuangyany.cn


<!-- 参考信息 -->