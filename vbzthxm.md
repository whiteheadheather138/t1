代发 wailian999

[A22] 获取字符串长度
来源：https://tr.zhonguo7118.cn

Py:   len(s)
来源：https://bj.zhonguo5118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://sf.zhonguo8118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://yy.zhonguo7118.cn

TS:   s.length
来源：https://os.zhonguo3118.cn

Java: s.length()
来源：https://cu.zhonguo5118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://km.zhonguo7118.cn

Ruby: s.length
来源：https://ed.zhonguo6118.cn

C#:   s.Length
来源：https://bo.zhonguo6118.cn

[A23] 大小写转换
来源：https://mf.zhonguo2118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://ip.zhonguo7118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://cc.zhonguo6118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://ly.zhonguo3118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://wk.zhonguo7118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://so.zhonguo7118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://pl.zhonguo4118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://gy.zhonguo7118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://rw.zhonguo6118.cn

[A24] 去除首尾空白
来源：https://dl.zhonguo5118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://qx.zhonguo6118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://rh.zhonguo2118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://nl.zhonguo3118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://uz.zhonguo1118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://rl.zhonguo5118.cn

Go:   strings.TrimSpace(s)
来源：https://bj.zhonguo5118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://uj.zhonguo7118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://rg.zhonguo5118.cn

[A25] 字符串比较
来源：https://ey.zhonguo2118.cn

Py:   s1 == s2; s1 != s2
来源：https://od.zhonguo4118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://td.zhonguo3118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://tz.zhonguo6118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://hw.zhonguo7118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://in.zhonguo5118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://sz.zhonguo8118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://wo.zhonguo1118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://or.zhonguo8118.cn

[A26] 类型转换总览
来源：https://qr.zhonguo5118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://ju.zhonguo3118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://rg.zhonguo8118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://qo.zhonguo1118.cn

TS:   Number() String() Boolean() x as number
来源：https://ok.zhonguo4118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://mo.zhonguo1118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://ul.zhonguo3118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://vh.zhonguo5118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://oh.zhonguo1118.cn

================================================================================
来源：https://yb.zhonguo6118.cn

B. 流程控制
来源：https://zf.zhonguo1118.cn

================================================================================
来源：https://kn.zhonguo8118.cn

[B01] 条件判断 if / else
来源：https://bo.zhonguo4118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://ur.zhonguo5118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://vc.zhonguo2118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://yg.zhonguo2118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://cu.zhonguo4118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://mp.zhonguo4118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://vu.zhonguo1118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://cv.zhonguo3118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://ip.zhonguo3118.cn

[B02] 多分支 else if / elif
来源：https://fm.zhonguo6118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://po.zhonguo1118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://rf.zhonguo5118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://we.zhonguo5118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ht.zhonguo7118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://to.zhonguo4118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://at.zhonguo1118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://ou.zhonguo4118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://hx.zhonguo4118.cn

[B03] switch / match / case
来源：https://kx.zhonguo3118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://sd.zhonguo4118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://pf.zhonguo6118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://tt.zhonguo2118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://xc.zhonguo1118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://wf.zhonguo2118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://jx.zhonguo6118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://tr.zhonguo1118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://vf.zhonguo8118.cn

[B04] for 计数循环
来源：https://pz.zhonguo7118.cn

Py:   for i in range(10): print(i)
来源：https://fy.zhonguo7118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://ol.zhonguo4118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://ti.zhonguo7118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://jt.zhonguo7118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://nf.zhonguo1118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://hf.zhonguo4118.cn

Ruby: 10.times { |i| puts i }
来源：https://nd.zhonguo7118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://me.zhonguo4118.cn

[B05] 遍历数组 / 列表
来源：https://oj.zhonguo2118.cn

Py:   for item in arr: print(item)
来源：https://rx.zhonguo2118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://jf.zhonguo1118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://xs.zhonguo1118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://lb.zhonguo2118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://ve.zhonguo3118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://gu.zhonguo7118.cn

Ruby: arr.each { |item| puts item }
来源：https://en.zhonguo4118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://eu.zhonguo8118.cn

[B06] 遍历字典 / 对象
来源：https://mc.zhonguo1118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://ql.zhonguo3118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://np.zhonguo4118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://ze.zhonguo3118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://um.zhonguo4118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://lp.zhonguo5118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://hs.zhonguo2118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://jv.zhonguo1118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://yh.zhonguo6118.cn

[B07] while 循环
来源：https://ib.zhonguo6118.cn

Py:   while i < 10: i += 1
来源：https://ya.zhonguo4118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://pm.zhonguo4118.cn

JS:   while (i < 10) { i++; }
来源：https://vw.zhonguo6118.cn

TS:   while (i < 10) { i++; }
来源：https://wv.zhonguo7118.cn

Java: while (i < 10) { i++; }
来源：https://rh.zhonguo1118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://na.zhonguo4118.cn

Ruby: while i < 10; i += 1; end
来源：https://hx.zhonguo4118.cn

C#:   while (i < 10) { i++; }
来源：https://sl.zhonguo1118.cn

[B08] do-while（至少执行一次）
来源：https://pz.zhonguo3118.cn

Py:   # 无 do-while：用 while True + break
来源：https://sm.zhonguo8118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://ai.zhonguo1118.cn

JS:   do { i++; } while (i < 10);
来源：https://ho.zhonguo8118.cn

TS:   do { i++; } while (i < 10);
来源：https://zz.zhonguo5118.cn

Java: do { i++; } while (i < 10);
来源：https://aa.zhonguo7118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://of.zhonguo7118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://ca.zhonguo3118.cn

C#:   do { i++; } while (i < 10);
来源：https://rg.zhonguo3118.cn

[B09] break 与 continue
来源：https://of.zhonguo2118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://zw.zhonguo6118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://kf.zhonguo6118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://jh.zhonguo1118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://jl.zhonguo5118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://yu.zhonguo7118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://jh.zhonguo7118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://rf.zhonguo2118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ea.zhonguo4118.cn

[B10] 遍历同时拿索引
来源：https://mw.zhonguo3118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://cm.zhonguo1118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://sj.zhonguo3118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://nu.zhonguo1118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://hp.zhonguo5118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://jn.zhonguo1118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://mf.zhonguo6118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://ae.zhonguo4118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://ym.zhonguo2118.cn

[B11] 生成数字序列 / 区间
来源：https://on.zhonguo8118.cn

Py:   list(range(0, 10, 2))
来源：https://az.zhonguo4118.cn

PHP:  range(0, 10, 2);
来源：https://dh.zhonguo1118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://ma.zhonguo7118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://zm.zhonguo4118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://pu.zhonguo8118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://hp.zhonguo2118.cn

Ruby: (0...10).step(2).to_a
来源：https://ie.zhonguo1118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://gj.zhonguo5118.cn

[B12] 跳出多层循环
来源：https://sm.zhonguo3118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://ij.zhonguo3118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://or.zhonguo7118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://ad.zhonguo4118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://ae.zhonguo7118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://qj.zhonguo3118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://kp.zhonguo7118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://dy.zhonguo1118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://az.zhonguo1118.cn

[B13] 判断是否为数字
来源：https://fc.zhonguo8118.cn

Py:   isinstance(x, (int, float))
来源：https://go.zhonguo4118.cn

PHP:  is_numeric($x)
来源：https://ut.zhonguo6118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://yn.zhonguo1118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://vm.zhonguo2118.cn

Java: x instanceof Number
来源：https://tm.zhonguo7118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://hb.zhonguo3118.cn

Ruby: x.is_a?(Numeric)
来源：https://vd.zhonguo5118.cn

C#:   x is int or double or decimal
来源：https://ep.zhonguo8118.cn

[B14] 判断值是否在集合内
来源：https://cl.zhonguo2118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://kb.zhonguo4118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://ot.zhonguo6118.cn

JS:   [1, 2, 3].includes(x)
来源：https://ti.zhonguo1118.cn

TS:   [1, 2, 3].includes(x)
来源：https://au.zhonguo7118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://zf.zhonguo2118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://pu.zhonguo6118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://br.zhonguo8118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://rb.zhonguo7118.cn

[B15] 布尔运算与取反
来源：https://yd.zhonguo8118.cn

Py:   a and b or not c
来源：https://hc.zhonguo7118.cn

PHP:  $a && $b || !$c
来源：https://ex.zhonguo7118.cn

JS:   a && b || !c
来源：https://ch.zhonguo8118.cn

TS:   a && b || !c
来源：https://km.zhonguo4118.cn

Java: a && b || !c
来源：https://xt.zhonguo4118.cn

Go:   a && b || !c
来源：https://at.zhonguo8118.cn

Ruby: a && b || !c
来源：https://rq.zhonguo2118.cn

C#:   a && b || !c
来源：https://xo.zhonguo7118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://ns.zhonguo4118.cn

Py:   if not data: return
来源：https://rl.zhonguo2118.cn

PHP:  if (!$data) { return; }
来源：https://bo.zhonguo5118.cn

JS:   if (!data) return;
来源：https://zv.zhonguo1118.cn

TS:   if (!data) return;
来源：https://bt.zhonguo6118.cn

Java: if (data == null) return;
来源：https://ut.zhonguo8118.cn

Go:   if data == nil { return }
来源：https://xg.zhonguo7118.cn

Ruby: return if data.nil?
来源：https://ev.zhonguo1118.cn

C#:   if (data == null) return;
来源：https://wh.zhonguo1118.cn

================================================================================
来源：https://hq.zhonguo6118.cn

C. 函数与作用域
来源：https://ey.zhonguo1118.cn

================================================================================
来源：https://gr.zhonguo8118.cn

[C01] 定义函数
来源：https://gw.zhonguo4118.cn

Py:   def add(a, b): return a + b
来源：https://ue.zhonguo7118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://by.zhonguo3118.cn

JS:   function add(a, b) { return a + b; }
来源：https://yw.zhonguo7118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://qc.zhonguo1118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://ed.zhonguo3118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://zf.zhonguo1118.cn

Ruby: def add(a, b); a + b; end
来源：https://ci.zhonguo7118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://ss.zhonguo5118.cn

[C02] 默认参数
来源：https://xy.zhonguo6118.cn

Py:   def greet(name="World"): return name
来源：https://so.zhonguo5118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://od.zhonguo8118.cn

JS:   function greet(name = "World") { return name; }
来源：https://eh.zhonguo1118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://nk.zhonguo2118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://ki.zhonguo8118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://iw.zhonguo4118.cn

Ruby: def greet(name = "World") = name
来源：https://sz.zhonguo7118.cn

C#:   string Greet(string name = "World") => name;
来源：https://te.zhonguo4118.cn

[C03] 可变参数
来源：https://hy.zhonguo7118.cn

Py:   def total(*args): return sum(args)
来源：https://rg.zhonguo8118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://yg.zhonguo5118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://kq.zhonguo7118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://ia.zhonguo2118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://lr.zhonguo5118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://dy.zhonguo2118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://pl.zhonguo6118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://id.zhonguo7118.cn

[C04] 命名参数 / 关键字参数
来源：https://fz.zhonguo5118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://do.zhonguo4118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://qr.zhonguo2118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://oh.zhonguo3118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://zl.zhonguo5118.cn

Java: // 无：用 Builder 模式或 record
来源：https://xu.zhonguo5118.cn

Go:   // 无：用配置结构体参数
来源：https://cu.zhonguo4118.cn

Ruby: f(a: 1, b: 2)
来源：https://az.zhonguo3118.cn

C#:   f(a: 1, b: 2)
来源：https://sk.zhonguo6118.cn

[C05] 返回多个值
来源：https://ml.zhonguo6118.cn

Py:   return a, b
来源：https://km.zhonguo3118.cn

PHP:  return [$a, $b];
来源：https://ca.zhonguo8118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://vk.zhonguo4118.cn

TS:   return { a, b };
来源：https://si.zhonguo4118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://oz.zhonguo4118.cn

Go:   return a, b
来源：https://gd.zhonguo1118.cn

Ruby: return a, b
来源：https://gw.zhonguo6118.cn

C#:   return (a, b);              // ValueTuple
来源：https://qg.zhonguo8118.cn

[C06] 匿名函数 / lambda
来源：https://mt.zhonguo7118.cn

Py:   square = lambda x: x * x
来源：https://od.zhonguo2118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://ev.zhonguo7118.cn

JS:   const square = x => x * x;
来源：https://ef.zhonguo6118.cn

TS:   const square = (x: number): number => x * x;
来源：https://ho.zhonguo8118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://xd.zhonguo4118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://ss.zhonguo6118.cn

Ruby: square = ->(x) { x * x }
来源：https://gf.zhonguo7118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://sf.zhonguo5118.cn

[C07] 把函数作为参数传入
来源：https://ma.zhonguo4118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://uo.zhonguo5118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://xn.zhonguo6118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://ai.zhonguo4118.cn

TS:   arr.map(String)
来源：https://ly.zhonguo7118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://zc.zhonguo1118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://rn.zhonguo3118.cn

Ruby: arr.map(&:upcase)
来源：https://rm.zhonguo7118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://za.zhonguo3118.cn

[C08] 闭包
来源：https://wa.zhonguo8118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://pb.zhonguo7118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://uq.zhonguo5118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://qe.zhonguo5118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://vr.zhonguo8118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://ij.zhonguo5118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://dq.zhonguo2118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://ff.zhonguo6118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://qo.zhonguo5118.cn

[C09] 递归
来源：https://sr.zhonguo8118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://qu.zhonguo8118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://gv.zhonguo8118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://io.zhonguo5118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://uc.zhonguo2118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://ux.zhonguo1118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://ns.zhonguo7118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://ue.zhonguo8118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://ls.zhonguo8118.cn

[C10] 变量作用域
来源：https://gd.zhonguo3118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://sr.zhonguo8118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://ro.zhonguo6118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://vp.zhonguo1118.cn

TS:   同 JS
来源：https://zd.zhonguo7118.cn

Java: 方法内为块级作用域
来源：https://yp.zhonguo2118.cn

Go:   花括号块级作用域
来源：https://nq.zhonguo8118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://bg.zhonguo2118.cn

C#:   块级作用域
来源：https://xr.zhonguo3118.cn

[C11] 模块导入与导出
来源：https://mb.zhonguo6118.cn

Py:   from module import func
来源：https://gc.zhonguo7118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://yi.zhonguo5118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://gj.zhonguo7118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://gr.zhonguo6118.cn

Java: import java.util.List;
来源：https://hd.zhonguo2118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://is.zhonguo8118.cn

Ruby: require "json"; require_relative "./util"
来源：https://ds.zhonguo7118.cn

C#:   using System.Text;
来源：https://wn.zhonguo1118.cn

[C12] 立即执行函数 IIFE
来源：https://fs.zhonguo4118.cn

Py:   (lambda: print("run"))()
来源：https://xg.zhonguo6118.cn

PHP:  (function () { echo "run"; })();
来源：https://wf.zhonguo8118.cn

JS:   (() => { console.log("run"); })();
来源：https://zh.zhonguo1118.cn

TS:   (() => { console.log("run"); })();
来源：https://pd.zhonguo1118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://fs.zhonguo2118.cn


<!-- 参考信息 -->