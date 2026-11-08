代发 wailian999

[A14] 注释写法
来源：https://dv.zhonguo4118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://pq.zhonguo6118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://xb.zhonguo2118.cn

JS:   // 单行；/* 多行 */
来源：https://qi.zhonguo8118.cn

TS:   // 单行；/* 多行 */
来源：https://ap.zhonguo3118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://jv.zhonguo5118.cn

Go:   // 单行；/* 多行 */
来源：https://oi.zhonguo8118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://dq.zhonguo2118.cn

C#:   // 单行；/* 多行 */
来源：https://rw.zhonguo6118.cn

[A15] 空值判断与默认值
来源：https://hj.zhonguo5118.cn

Py:   value = data or "默认值"
来源：https://if.zhonguo1118.cn

PHP:  $value = $data ?? "默认值";
来源：https://bw.zhonguo8118.cn

JS:   const value = data ?? "默认值";
来源：https://uk.zhonguo6118.cn

TS:   const value = data ?? "默认值";
来源：https://gx.zhonguo2118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://ey.zhonguo4118.cn

Go:   if data == "" { data = "默认值" }
来源：https://bo.zhonguo8118.cn

Ruby: value = data || "默认值"
来源：https://vj.zhonguo1118.cn

C#:   var value = data ?? "默认值";
来源：https://mg.zhonguo3118.cn

[A16] 真假值判断规则
来源：https://pj.zhonguo2118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://xr.zhonguo4118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://ac.zhonguo4118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://su.zhonguo7118.cn

TS:   if (!x) {}
来源：https://mo.zhonguo6118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://fy.zhonguo8118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://vc.zhonguo6118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://sl.zhonguo3118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://yn.zhonguo6118.cn

[A17] 位运算
来源：https://bz.zhonguo5118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://eh.zhonguo7118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://rf.zhonguo7118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://xj.zhonguo3118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://rz.zhonguo7118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://wg.zhonguo4118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://id.zhonguo1118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://xd.zhonguo7118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ph.zhonguo4118.cn

[A18] 字符与 ASCII 码互转
来源：https://yt.zhonguo8118.cn

Py:   ord("A"); chr(65)
来源：https://mo.zhonguo2118.cn

PHP:  ord("A"); chr(65)
来源：https://wk.zhonguo2118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://ha.zhonguo7118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://xx.zhonguo6118.cn

Java: (int) 'A'; (char) 65
来源：https://pk.zhonguo8118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://dh.zhonguo5118.cn

Ruby: "A".ord; 65.chr
来源：https://tp.zhonguo2118.cn

C#:   (int)'A'; (char)65
来源：https://ns.zhonguo1118.cn

[A19] 交换两个变量
来源：https://el.zhonguo8118.cn

Py:   a, b = b, a
来源：https://ex.zhonguo3118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://gg.zhonguo2118.cn

JS:   [a, b] = [b, a];
来源：https://hv.zhonguo1118.cn

TS:   [a, b] = [b, a];
来源：https://gr.zhonguo2118.cn

Java: int t = a; a = b; b = t;
来源：https://aa.zhonguo7118.cn

Go:   a, b = b, a
来源：https://cf.zhonguo7118.cn

Ruby: a, b = b, a
来源：https://vk.zhonguo1118.cn

C#:   (a, b) = (b, a);
来源：https://wz.zhonguo3118.cn

[A20] 读取标准输入
来源：https://bt.zhonguo6118.cn

Py:   name = input("请输入：")
来源：https://ts.zhonguo8118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://gp.zhonguo2118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://wr.zhonguo5118.cn

TS:   // Node.js：readline 模块
来源：https://sl.zhonguo6118.cn

Java: new Scanner(System.in).nextLine()
来源：https://bw.zhonguo5118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://wq.zhonguo7118.cn

Ruby: gets.chomp
来源：https://hj.zhonguo6118.cn

C#:   Console.ReadLine();
来源：https://gs.zhonguo8118.cn

[A21] 保留指定小数位输出
来源：https://fk.zhonguo8118.cn

Py:   f"{3.14159:.2f}"
来源：https://sm.zhonguo8118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://cy.zhonguo2118.cn

JS:   (3.14159).toFixed(2)
来源：https://uu.zhonguo2118.cn

TS:   (3.14159).toFixed(2)
来源：https://mz.zhonguo4118.cn

Java: String.format("%.2f", 3.14159)
来源：https://sz.zhonguo6118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://uf.zhonguo4118.cn

Ruby: format("%.2f", 3.14159)
来源：https://qq.zhonguo1118.cn

C#:   3.14159.ToString("F2")
来源：https://qc.zhonguo5118.cn

[A22] 获取字符串长度
来源：https://cj.zhonguo8118.cn

Py:   len(s)
来源：https://hi.zhonguo8118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://qh.zhonguo2118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://mk.zhonguo8118.cn

TS:   s.length
来源：https://gw.zhonguo5118.cn

Java: s.length()
来源：https://jh.zhonguo5118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://rw.zhonguo2118.cn

Ruby: s.length
来源：https://sf.zhonguo6118.cn

C#:   s.Length
来源：https://ov.zhonguo4118.cn

[A23] 大小写转换
来源：https://sp.zhonguo1118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://sl.zhonguo2118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://kn.zhonguo7118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://fc.zhonguo4118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://oj.zhonguo7118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://fp.zhonguo4118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://qv.zhonguo8118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://fc.zhonguo8118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://nq.zhonguo1118.cn

[A24] 去除首尾空白
来源：https://qj.zhonguo7118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://in.zhonguo6118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://ii.zhonguo5118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://pj.zhonguo4118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://yw.zhonguo2118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://jd.zhonguo7118.cn

Go:   strings.TrimSpace(s)
来源：https://gi.zhonguo8118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://mb.zhonguo5118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://dc.zhonguo8118.cn

[A25] 字符串比较
来源：https://go.zhonguo3118.cn

Py:   s1 == s2; s1 != s2
来源：https://qf.zhonguo4118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://vo.zhonguo3118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://ef.zhonguo2118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://yx.zhonguo1118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://ov.zhonguo6118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://di.zhonguo5118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://wy.zhonguo7118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://fv.zhonguo2118.cn

[A26] 类型转换总览
来源：https://tq.zhonguo5118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://sr.zhonguo5118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://fp.zhonguo2118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://ir.zhonguo8118.cn

TS:   Number() String() Boolean() x as number
来源：https://lg.zhonguo8118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://uq.zhonguo8118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://uo.zhonguo4118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://xw.zhonguo6118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://wz.zhonguo8118.cn

================================================================================
来源：https://cl.zhonguo1118.cn

B. 流程控制
来源：https://hg.zhonguo2118.cn

================================================================================
来源：https://go.zhonguo4118.cn

[B01] 条件判断 if / else
来源：https://zx.zhonguo7118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://sr.zhonguo2118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://pj.zhonguo2118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://kl.zhonguo1118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://wa.zhonguo1118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://mh.zhonguo8118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://az.zhonguo6118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://pk.zhonguo8118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://va.zhonguo5118.cn

[B02] 多分支 else if / elif
来源：https://wv.zhonguo1118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://gu.zhonguo2118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://fl.zhonguo6118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://jy.zhonguo2118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://um.zhonguo4118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://tj.zhonguo2118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://mh.zhonguo3118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://lw.zhonguo3118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://lr.zhonguo4118.cn

[B03] switch / match / case
来源：https://ob.zhonguo8118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://qv.zhonguo7118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://tb.zhonguo4118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://zn.zhonguo3118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://dx.zhonguo6118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://eo.zhonguo3118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://if.zhonguo3118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://cr.zhonguo8118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://of.zhonguo7118.cn

[B04] for 计数循环
来源：https://lg.zhonguo1118.cn

Py:   for i in range(10): print(i)
来源：https://mv.zhonguo6118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://rk.zhonguo4118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://eo.zhonguo6118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://zf.zhonguo3118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://px.zhonguo8118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://vg.zhonguo8118.cn

Ruby: 10.times { |i| puts i }
来源：https://wv.zhonguo5118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://bl.zhonguo1118.cn

[B05] 遍历数组 / 列表
来源：https://ll.zhonguo1118.cn

Py:   for item in arr: print(item)
来源：https://ag.zhonguo8118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://rf.zhonguo6118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://ix.zhonguo4118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://rr.zhonguo7118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://tn.zhonguo6118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://us.zhonguo4118.cn

Ruby: arr.each { |item| puts item }
来源：https://ot.zhonguo2118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://rj.zhonguo6118.cn

[B06] 遍历字典 / 对象
来源：https://bi.zhonguo3118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://de.zhonguo2118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://gt.zhonguo8118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://ms.zhonguo1118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://tw.zhonguo1118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://lf.zhonguo8118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://nl.zhonguo1118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://wc.zhonguo4118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://ua.zhonguo6118.cn

[B07] while 循环
来源：https://lw.zhonguo1118.cn

Py:   while i < 10: i += 1
来源：https://dq.zhonguo5118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://qx.zhonguo7118.cn

JS:   while (i < 10) { i++; }
来源：https://lb.zhonguo7118.cn

TS:   while (i < 10) { i++; }
来源：https://rl.zhonguo5118.cn

Java: while (i < 10) { i++; }
来源：https://ng.zhonguo6118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://yv.zhonguo4118.cn

Ruby: while i < 10; i += 1; end
来源：https://fl.zhonguo7118.cn

C#:   while (i < 10) { i++; }
来源：https://bb.zhonguo3118.cn

[B08] do-while（至少执行一次）
来源：https://ll.zhonguo6118.cn

Py:   # 无 do-while：用 while True + break
来源：https://fo.zhonguo2118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://gv.zhonguo4118.cn

JS:   do { i++; } while (i < 10);
来源：https://jf.zhonguo4118.cn

TS:   do { i++; } while (i < 10);
来源：https://qi.zhonguo5118.cn

Java: do { i++; } while (i < 10);
来源：https://oh.zhonguo4118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://hu.zhonguo4118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://qp.zhonguo2118.cn

C#:   do { i++; } while (i < 10);
来源：https://mh.zhonguo6118.cn

[B09] break 与 continue
来源：https://lj.zhonguo6118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://qk.zhonguo5118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://qd.zhonguo6118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://jt.zhonguo3118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://kt.zhonguo3118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ge.zhonguo7118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://ce.zhonguo2118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://so.zhonguo3118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://vu.zhonguo7118.cn

[B10] 遍历同时拿索引
来源：https://nt.zhonguo8118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://ig.zhonguo8118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://gg.zhonguo6118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://eq.zhonguo4118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://su.zhonguo7118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://fq.zhonguo4118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://ku.zhonguo7118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://mf.zhonguo3118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://ia.zhonguo8118.cn

[B11] 生成数字序列 / 区间
来源：https://rs.zhonguo7118.cn

Py:   list(range(0, 10, 2))
来源：https://qu.zhonguo2118.cn

PHP:  range(0, 10, 2);
来源：https://ma.zhonguo7118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://kf.zhonguo4118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://bd.zhonguo2118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://ym.zhonguo5118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://no.zhonguo8118.cn

Ruby: (0...10).step(2).to_a
来源：https://ht.zhonguo1118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://sv.zhonguo8118.cn

[B12] 跳出多层循环
来源：https://di.zhonguo5118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://rq.zhonguo8118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://pq.zhonguo6118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://bn.zhonguo4118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://lb.zhonguo7118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://ac.zhonguo1118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://lf.zhonguo8118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://lp.zhonguo2118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://gd.zhonguo2118.cn

[B13] 判断是否为数字
来源：https://xx.zhonguo6118.cn

Py:   isinstance(x, (int, float))
来源：https://hg.zhonguo8118.cn

PHP:  is_numeric($x)
来源：https://lc.zhonguo1118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://tq.zhonguo7118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ut.zhonguo7118.cn

Java: x instanceof Number
来源：https://du.zhonguo7118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://ad.zhonguo6118.cn

Ruby: x.is_a?(Numeric)
来源：https://qv.zhonguo8118.cn

C#:   x is int or double or decimal
来源：https://el.zhonguo4118.cn

[B14] 判断值是否在集合内
来源：https://nf.zhonguo4118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://hk.zhonguo4118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://wi.zhonguo1118.cn

JS:   [1, 2, 3].includes(x)
来源：https://ic.zhonguo7118.cn

TS:   [1, 2, 3].includes(x)
来源：https://jv.zhonguo1118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://yy.zhonguo4118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://wi.zhonguo6118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://qv.zhonguo3118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://yo.zhonguo3118.cn

[B15] 布尔运算与取反
来源：https://sf.zhonguo3118.cn

Py:   a and b or not c
来源：https://vb.zhonguo4118.cn

PHP:  $a && $b || !$c
来源：https://vv.zhonguo5118.cn

JS:   a && b || !c
来源：https://mf.zhonguo1118.cn

TS:   a && b || !c
来源：https://pb.zhonguo3118.cn

Java: a && b || !c
来源：https://xf.zhonguo6118.cn

Go:   a && b || !c
来源：https://gy.zhonguo4118.cn

Ruby: a && b || !c
来源：https://ss.zhonguo4118.cn

C#:   a && b || !c
来源：https://kf.zhonguo1118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://yg.zhonguo2118.cn

Py:   if not data: return
来源：https://ma.zhonguo4118.cn

PHP:  if (!$data) { return; }
来源：https://tw.zhonguo3118.cn

JS:   if (!data) return;
来源：https://lg.zhonguo5118.cn

TS:   if (!data) return;
来源：https://xy.zhonguo8118.cn

Java: if (data == null) return;
来源：https://ah.zhonguo2118.cn

Go:   if data == nil { return }
来源：https://ri.zhonguo1118.cn

Ruby: return if data.nil?
来源：https://te.zhonguo7118.cn

C#:   if (data == null) return;
来源：https://yh.zhonguo8118.cn

================================================================================
来源：https://bb.zhonguo3118.cn

C. 函数与作用域
来源：https://uo.zhonguo1118.cn

================================================================================
来源：https://fg.zhonguo3118.cn

[C01] 定义函数
来源：https://zf.zhonguo1118.cn

Py:   def add(a, b): return a + b
来源：https://te.zhonguo1118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://pe.zhonguo1118.cn

JS:   function add(a, b) { return a + b; }
来源：https://hh.zhonguo5118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://sd.zhonguo2118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://fj.zhonguo5118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://zv.zhonguo1118.cn

Ruby: def add(a, b); a + b; end
来源：https://bi.zhonguo4118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://dz.zhonguo6118.cn

[C02] 默认参数
来源：https://vb.zhonguo1118.cn

Py:   def greet(name="World"): return name
来源：https://kq.zhonguo8118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://wp.zhonguo4118.cn

JS:   function greet(name = "World") { return name; }
来源：https://ud.zhonguo5118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://hu.zhonguo2118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://bv.zhonguo6118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://wn.zhonguo6118.cn

Ruby: def greet(name = "World") = name
来源：https://gt.zhonguo3118.cn

C#:   string Greet(string name = "World") => name;
来源：https://oa.zhonguo4118.cn

[C03] 可变参数
来源：https://ab.zhonguo2118.cn

Py:   def total(*args): return sum(args)
来源：https://pu.zhonguo6118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://vu.zhonguo6118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://dj.zhonguo1118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://qd.zhonguo4118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://ap.zhonguo3118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://ic.zhonguo8118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://bb.zhonguo1118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://py.zhonguo6118.cn

[C04] 命名参数 / 关键字参数
来源：https://pb.zhonguo3118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://ms.zhonguo5118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://jh.zhonguo8118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://qv.zhonguo6118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://fe.zhonguo7118.cn

Java: // 无：用 Builder 模式或 record
来源：https://ke.zhonguo1118.cn


<!-- 参考信息 -->