代发 wailian999

TS:   s.length
来源：http://ewf.vqdsnc.cn

Java: s.length()
来源：http://cxp.jlsjyb.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://olo.yj20258.top

Ruby: s.length
来源：http://qcg.cashguo.top

C#:   s.Length
来源：http://rmp.ctjpmb.com

[A23] 大小写转换
来源：http://ffj.zhaomingkeji.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://amy.snrcjt.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rak.yfazqb.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cry.jinqigfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hmg.zhixingplan.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iny.nanxuanxn.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jzn.ydzc1.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dtp.sysykeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mpb.chenzaomai.com

[A24] 去除首尾空白
来源：http://wsk.aizwys.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://efp.daria6918.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rab.pengpengdd.cyou

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sty.tarul.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gqj.xingfuxueyuan.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ccs.hongshengwenyu.top

Go:   strings.TrimSpace(s)
来源：http://ufe.bjfxy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ztp.sufxvd.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wrg.daria6918.cn

[A25] 字符串比较
来源：http://pfl.ydjk.org.cn

Py:   s1 == s2; s1 != s2
来源：http://tge.meibo888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oqx.bjfxy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ywz.havefunace.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ack.haohaochexian.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zvn.guannengcc.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yzl.cqqwz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tib.wangdashe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://agt.yongpay.top

[A26] 类型转换总览
来源：http://xrd.0kj1m.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wtk.yueranfly.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zdg.andypj.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jwb.birdmap.top

TS:   Number() String() Boolean() x as number
来源：http://foa.vqdsnc.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oko.ctjpmb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xvr.hongshengwenyu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ehe.jqgfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kxb.tanke756.top

================================================================================
来源：http://sml.fengsongda.top

B. 流程控制
来源：http://xdz.jinghuilouyu.cn

================================================================================
来源：http://tdt.daria6918.cn

[B01] 条件判断 if / else
来源：http://eyj.jianghu66.top

Py:   result = "正" if x > 0 else "非正"
来源：http://euf.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://feq.yj20258888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xmi.cheryme.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qud.hammf.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lnt.yueranfly.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://emv.ydzc1.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rzh.daria6918.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jhz.zhengqikj.top

[B02] 多分支 else if / elif
来源：http://yjq.hcnkem.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jab.sjlbkw.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bvq.jinyuanbaomall.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fsp.jinqigufen.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://csk.iojbl.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://did.guowangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kan.jyoumei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://imz.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rso.kuanghao11.cn

[B03] switch / match / case
来源：http://nwu.jinyuanbaomall.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://osv.daria6918.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hnp.xylfe.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dni.zhixingplan.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jgd.jianghu66.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://axg.jinghuilouyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qyh.fktsv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://klo.aibaodan.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cxq.hywenlv.cn

[B04] for 计数循环
来源：http://wil.sweek.top

Py:   for i in range(10): print(i)
来源：http://dgv.ppjwa.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aed.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nox.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fiy.tanke756.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://awb.fengsongda.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zhp.xziqi.cn

Ruby: 10.times { |i| puts i }
来源：http://uik.yueranfly.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://alr.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://foa.sjlbkw.cn

Py:   for item in arr: print(item)
来源：http://udj.chenlongwang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mna.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://stk.yueranfly.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zug.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bas.jyoumei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cya.haohaochexian.top

Ruby: arr.each { |item| puts item }
来源：http://wrx.nanxuanxn.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cot.yj202588.top

[B06] 遍历字典 / 对象
来源：http://kkr.chenzaomai.com

Py:   for k, v in d.items(): print(k, v)
来源：http://iyx.cashguo.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://szt.ivvv.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lir.chenzaomai.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fjy.zhijiandao.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aei.jinyuanbaomall.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://twu.jiagoushi.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zxt.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wjq.hysaishi.cn

[B07] while 循环
来源：http://ehp.jinqigufen.top

Py:   while i < 10: i += 1
来源：http://cml.ehwqpu.com

PHP:  while ($i < 10) { $i++; }
来源：http://fkm.fengsongda.top

JS:   while (i < 10) { i++; }
来源：http://mag.hysaishi.cn

TS:   while (i < 10) { i++; }
来源：http://not.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://phh.hammf.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://waw.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://ilv.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://spg.mhx1999.top

[B08] do-while（至少执行一次）
来源：http://vuo.haohaochexian.top

Py:   # 无 do-while：用 while True + break
来源：http://mos.hnqzz.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cfq.yueranfly.top

JS:   do { i++; } while (i < 10);
来源：http://sci.redwolf501.top

TS:   do { i++; } while (i < 10);
来源：http://esw.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://yrk.xziqi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tmk.gaohongyu789.top

Ruby: begin; i += 1; end while i < 10
来源：http://ylf.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://pmz.mhx1999.top

[B09] break 与 continue
来源：http://ahm.ydzc1.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ncb.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ffh.chenjidiqi.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://igs.mhx1999.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mmr.wangdashe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xgk.bbcook.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kvb.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qum.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gas.0kj1m.cn

[B10] 遍历同时拿索引
来源：http://pjz.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nro.wangshuangyany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gkt.jyoumei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wvd.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dkg.yuanzhike.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nll.zhengqikj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://izl.ctjpmb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xuq.guannengcc.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jag.xuanzx.com

[B11] 生成数字序列 / 区间
来源：http://dyj.andypj.xyz

Py:   list(range(0, 10, 2))
来源：http://mgc.havefunace.top

PHP:  range(0, 10, 2);
来源：http://mov.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sqb.wangshuangyany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kxm.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bts.ppjwa.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gij.xylfe.cn

Ruby: (0...10).step(2).to_a
来源：http://zgx.hongshengwenyu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qds.jqgufenzy.top

[B12] 跳出多层循环
来源：http://nyf.xingfuxueyuan.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://swm.fehbvm.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ien.hesvh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ynq.feifeiyinyue.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vsg.zdbjq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wag.chenlongwang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dfo.nwbrower.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://caq.jqgfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xcp.nwbrower.top

[B13] 判断是否为数字
来源：http://tnr.sufxvd.cn

Py:   isinstance(x, (int, float))
来源：http://ngx.birdmap.top

PHP:  is_numeric($x)
来源：http://suc.ydjk.org.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oam.xingfuxueyuan.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kjg.gzhubu.top

Java: x instanceof Number
来源：http://bsg.mhx1999.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ofi.jinghuilouyu.cn

Ruby: x.is_a?(Numeric)
来源：http://zfx.sufxvd.cn

C#:   x is int or double or decimal
来源：http://ldr.cqqwz.cn

[B14] 判断值是否在集合内
来源：http://hqb.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ppn.zdqjudy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rbv.yonumen.top

JS:   [1, 2, 3].includes(x)
来源：http://mzd.hongshengwenyu.top

TS:   [1, 2, 3].includes(x)
来源：http://imn.zdqjudy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://esp.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hyp.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://reo.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gvn.fehbvm.com

[B15] 布尔运算与取反
来源：http://ivj.chenzaomai.com

Py:   a and b or not c
来源：http://wqn.dianchejie.cn

PHP:  $a && $b || !$c
来源：http://wbb.316326.xyz

JS:   a && b || !c
来源：http://son.jinqigufen.top

TS:   a && b || !c
来源：http://eng.cheryme.top

Java: a && b || !c
来源：http://uve.gaohongyu789.top

Go:   a && b || !c
来源：http://inw.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://esp.fzhhl.top

C#:   a && b || !c
来源：http://pyz.fktsv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cwf.fktsv.cn

Py:   if not data: return
来源：http://uzb.jinghuilouyu.cn

PHP:  if (!$data) { return; }
来源：http://kam.chenjidiqi.icu

JS:   if (!data) return;
来源：http://ewk.nwbrower.top

TS:   if (!data) return;
来源：http://cyo.sufxvd.cn

Java: if (data == null) return;
来源：http://olv.cqqwz.cn

Go:   if data == nil { return }
来源：http://hjd.cashguo.top

Ruby: return if data.nil?
来源：http://mmj.fanxiaobao.xyz

C#:   if (data == null) return;
来源：http://mgf.hongshengwenyu.top

================================================================================
来源：http://zxl.yangfankeji.com

C. 函数与作用域
来源：http://uxf.xinyue.icu

================================================================================
来源：http://gkq.c1oappe.top

[C01] 定义函数
来源：http://tpx.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://ezk.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://anh.fengsongda.top

JS:   function add(a, b) { return a + b; }
来源：http://jnp.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jqm.c1oappe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nwt.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://yjj.chenjidiqi.icu

Ruby: def add(a, b); a + b; end
来源：http://ygk.jiagoushi.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tbo.yj20258.top

[C02] 默认参数
来源：http://lac.daxiang520.top

Py:   def greet(name="World"): return name
来源：http://gzx.bjfxy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://caq.yvedp.cn

JS:   function greet(name = "World") { return name; }
来源：http://uzt.gotoacloud.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fnq.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nxh.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uqk.bbcook.cn

Ruby: def greet(name = "World") = name
来源：http://epj.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://jwk.birdmap.top

[C03] 可变参数
来源：http://qvy.daxiang520.top

Py:   def total(*args): return sum(args)
来源：http://dxi.fengsongda.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fpl.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fni.xuanzx.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ppn.jinqigfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sbv.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jfz.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xib.fehbvm.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kdg.chenzaomai.com

[C04] 命名参数 / 关键字参数
来源：http://blv.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xmw.shanyushiyangtech.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vwi.snrcjt.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wcg.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qbs.52xcode.cn

Java: // 无：用 Builder 模式或 record
来源：http://vgz.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://ssf.haohaochexian.top

Ruby: f(a: 1, b: 2)
来源：http://qem.zdbjq.cn

C#:   f(a: 1, b: 2)
来源：http://xeu.cdnleiting.top

[C05] 返回多个值
来源：http://kdy.jqgfzy.top

Py:   return a, b
来源：http://unu.hysaishi.cn

PHP:  return [$a, $b];
来源：http://tjs.c1oappe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gzs.gzhubu.top

TS:   return { a, b };
来源：http://fka.yueranfly.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oms.uphjek.com

Go:   return a, b
来源：http://mcf.yonumen.top

Ruby: return a, b
来源：http://svk.zhoulong.xyz

C#:   return (a, b);              // ValueTuple
来源：http://fiw.c1oappe.top

[C06] 匿名函数 / lambda
来源：http://odh.fanxiaobao.xyz

Py:   square = lambda x: x * x
来源：http://von.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vfu.hcnkem.com

JS:   const square = x => x * x;
来源：http://mwf.316326.xyz

TS:   const square = (x: number): number => x * x;
来源：http://tkn.chenjidiqi.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gbr.yfazqb.com

Go:   sq := func(x int) int { return x * x }
来源：http://nuo.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://fro.mhx1999.top

C#:   Func<int, int> square = x => x * x;
来源：http://iqp.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://adm.xuetiantiany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zws.c1oappe.top

PHP:  array_map("strtoupper", $arr);
来源：http://jwv.yj20258888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wua.redwolf501.top

TS:   arr.map(String)
来源：http://roj.epnwcf.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://twm.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yff.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://wxw.shangyingyoupin.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dky.pengpengdd.cyou

[C08] 闭包
来源：http://pgv.zhongyouzk.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://phs.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fan.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xih.fanxiaobao.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pok.hysaishi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://til.hfpthk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oyj.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lcq.ydjk.org.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qns.zhoulong.xyz

[C09] 递归
来源：http://yde.yj20258.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://atf.andypj.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ntw.cucudq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dsv.zycfv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://srn.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://awe.tanke756.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://obr.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cid.pengpengdd.cyou

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://aul.guannengcc.top

[C10] 变量作用域
来源：http://hbp.daria6918.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hdg.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ans.chenlongwang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://prl.9152youxi.cn

TS:   同 JS
来源：http://dpn.jinqigfzy.top

Java: 方法内为块级作用域
来源：http://jgd.ybcxt.top

Go:   花括号块级作用域
来源：http://cmd.nwbrower.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pqq.ppjwa.cn

C#:   块级作用域
来源：http://pri.tanke756.top

[C11] 模块导入与导出
来源：http://dwr.tian-w.cn

Py:   from module import func
来源：http://ieq.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hao.jianghu66.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://daj.dashuyun.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dsv.ybcxt.top

Java: import java.util.List;
来源：http://rxf.hcnkem.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cah.gotoacloud.top

Ruby: require "json"; require_relative "./util"
来源：http://ksm.aizwys.cn

C#:   using System.Text;
来源：http://bte.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://euy.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://rnx.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://fke.birdmap.top

JS:   (() => { console.log("run"); })();
来源：http://oxd.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://wxt.jinghuilouyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tav.bjfxy.top

Go:   func() { fmt.Println("run") }()
来源：http://vzl.hnqzz.top

Ruby: -> { puts "run" }.call
来源：http://aou.tianlin.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://wio.zhongyouzk.top

[C13] 类型声明 / 类型注解
来源：http://xoz.jqgufenzy.top


<!-- 参考信息 -->