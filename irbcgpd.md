代发 wailian999

TS:   // 单行；/* 多行 */
来源：https://wg.zhonguo1118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://jj.zhonguo3118.cn

Go:   // 单行；/* 多行 */
来源：https://hr.zhonguo7118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://uh.zhonguo8118.cn

C#:   // 单行；/* 多行 */
来源：https://lx.zhonguo1118.cn

[A15] 空值判断与默认值
来源：https://je.zhonguo5118.cn

Py:   value = data or "默认值"
来源：https://oz.zhonguo7118.cn

PHP:  $value = $data ?? "默认值";
来源：https://lh.zhonguo4118.cn

JS:   const value = data ?? "默认值";
来源：https://rb.zhonguo3118.cn

TS:   const value = data ?? "默认值";
来源：https://xa.zhonguo6118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://bw.zhonguo8118.cn

Go:   if data == "" { data = "默认值" }
来源：https://yw.zhonguo7118.cn

Ruby: value = data || "默认值"
来源：https://pr.zhonguo8118.cn

C#:   var value = data ?? "默认值";
来源：https://zo.zhonguo6118.cn

[A16] 真假值判断规则
来源：https://jc.zhonguo4118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://ji.zhonguo5118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://nz.zhonguo1118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://wz.zhonguo2118.cn

TS:   if (!x) {}
来源：https://ia.zhonguo6118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://vf.zhonguo6118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://eq.zhonguo7118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://tp.zhonguo2118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://pt.zhonguo8118.cn

[A17] 位运算
来源：https://ov.zhonguo3118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://rv.zhonguo7118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://pe.zhonguo2118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://cx.zhonguo6118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://zz.zhonguo7118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://oe.zhonguo8118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://ki.zhonguo6118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://az.zhonguo7118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ix.zhonguo2118.cn

[A18] 字符与 ASCII 码互转
来源：https://ag.zhonguo3118.cn

Py:   ord("A"); chr(65)
来源：https://la.zhonguo4118.cn

PHP:  ord("A"); chr(65)
来源：https://lu.zhonguo8118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://im.zhonguo2118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://jl.zhonguo5118.cn

Java: (int) 'A'; (char) 65
来源：https://tq.zhonguo3118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://by.zhonguo6118.cn

Ruby: "A".ord; 65.chr
来源：https://uy.zhonguo1118.cn

C#:   (int)'A'; (char)65
来源：https://fb.zhonguo7118.cn

[A19] 交换两个变量
来源：https://he.zhonguo4118.cn

Py:   a, b = b, a
来源：https://te.zhonguo1118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://dh.zhonguo4118.cn

JS:   [a, b] = [b, a];
来源：https://my.zhonguo7118.cn

TS:   [a, b] = [b, a];
来源：https://tu.zhonguo5118.cn

Java: int t = a; a = b; b = t;
来源：https://xf.zhonguo8118.cn

Go:   a, b = b, a
来源：https://be.zhonguo8118.cn

Ruby: a, b = b, a
来源：https://xx.zhonguo5118.cn

C#:   (a, b) = (b, a);
来源：https://nm.zhonguo6118.cn

[A20] 读取标准输入
来源：https://pq.zhonguo7118.cn

Py:   name = input("请输入：")
来源：https://ma.zhonguo3118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://mx.zhonguo2118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://aw.zhonguo8118.cn

TS:   // Node.js：readline 模块
来源：https://qs.zhonguo6118.cn

Java: new Scanner(System.in).nextLine()
来源：https://yd.zhonguo8118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://dm.zhonguo5118.cn

Ruby: gets.chomp
来源：https://bg.zhonguo6118.cn

C#:   Console.ReadLine();
来源：https://um.zhonguo1118.cn

[A21] 保留指定小数位输出
来源：https://nc.zhonguo3118.cn

Py:   f"{3.14159:.2f}"
来源：https://df.zhonguo4118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://rt.zhonguo1118.cn

JS:   (3.14159).toFixed(2)
来源：https://qo.zhonguo3118.cn

TS:   (3.14159).toFixed(2)
来源：https://ot.zhonguo6118.cn

Java: String.format("%.2f", 3.14159)
来源：https://qf.zhonguo4118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://rm.zhonguo8118.cn

Ruby: format("%.2f", 3.14159)
来源：https://jl.zhonguo8118.cn

C#:   3.14159.ToString("F2")
来源：https://mo.zhonguo5118.cn

[A22] 获取字符串长度
来源：https://zt.zhonguo2118.cn

Py:   len(s)
来源：https://gw.zhonguo8118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://wd.zhonguo3118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://id.zhonguo3118.cn

TS:   s.length
来源：https://kr.zhonguo5118.cn

Java: s.length()
来源：https://ig.zhonguo5118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://cd.zhonguo4118.cn

Ruby: s.length
来源：https://tj.zhonguo7118.cn

C#:   s.Length
来源：https://zx.zhonguo1118.cn

[A23] 大小写转换
来源：https://ve.zhonguo6118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://fs.zhonguo3118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://gz.zhonguo1118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://sn.zhonguo2118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://jd.zhonguo3118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://rc.zhonguo5118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://xf.zhonguo3118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://bh.zhonguo7118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://vr.zhonguo2118.cn

[A24] 去除首尾空白
来源：https://gs.zhonguo2118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://br.zhonguo7118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://ag.zhonguo5118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://tf.zhonguo3118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://nl.zhonguo8118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://gu.zhonguo2118.cn

Go:   strings.TrimSpace(s)
来源：https://tc.zhonguo3118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://rg.zhonguo3118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://vv.zhonguo1118.cn

[A25] 字符串比较
来源：https://jm.zhonguo8118.cn

Py:   s1 == s2; s1 != s2
来源：https://ky.zhonguo8118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://lh.zhonguo6118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://vw.zhonguo6118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://ur.zhonguo4118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://lo.zhonguo1118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://qu.zhonguo4118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://ro.zhonguo8118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://lr.zhonguo5118.cn

[A26] 类型转换总览
来源：https://oo.zhonguo3118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://na.zhonguo1118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://af.zhonguo8118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://px.zhonguo8118.cn

TS:   Number() String() Boolean() x as number
来源：https://fu.zhonguo3118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://aj.zhonguo1118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://wd.zhonguo7118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://tq.zhonguo7118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://bs.zhonguo3118.cn

================================================================================
来源：https://zs.zhonguo7118.cn

B. 流程控制
来源：https://hi.zhonguo4118.cn

================================================================================
来源：https://gp.zhonguo7118.cn

[B01] 条件判断 if / else
来源：https://vb.zhonguo2118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://zw.zhonguo5118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://ot.zhonguo8118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://jl.zhonguo1118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://ou.zhonguo3118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://yz.zhonguo2118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://on.zhonguo4118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://jn.zhonguo8118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://kc.zhonguo1118.cn

[B02] 多分支 else if / elif
来源：https://ms.zhonguo6118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://il.zhonguo7118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://gd.zhonguo1118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://dm.zhonguo1118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://sr.zhonguo6118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://jy.zhonguo4118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://kk.zhonguo7118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://lh.zhonguo7118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://vo.zhonguo4118.cn

[B03] switch / match / case
来源：https://av.zhonguo3118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://sv.zhonguo3118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://uh.zhonguo6118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://wb.zhonguo5118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://hh.zhonguo4118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://wt.zhonguo5118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://fn.zhonguo5118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://mc.zhonguo4118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://tl.zhonguo8118.cn

[B04] for 计数循环
来源：https://fv.zhonguo2118.cn

Py:   for i in range(10): print(i)
来源：https://cc.zhonguo1118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://qz.zhonguo8118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://up.zhonguo5118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://xe.zhonguo4118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://eh.zhonguo1118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://kb.zhonguo6118.cn

Ruby: 10.times { |i| puts i }
来源：https://gc.zhonguo5118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://sq.zhonguo6118.cn

[B05] 遍历数组 / 列表
来源：https://rh.zhonguo6118.cn

Py:   for item in arr: print(item)
来源：https://hg.zhonguo6118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://kr.zhonguo3118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://uq.zhonguo5118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://ou.zhonguo8118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://wo.zhonguo6118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://no.zhonguo1118.cn

Ruby: arr.each { |item| puts item }
来源：https://ai.zhonguo5118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://qs.zhonguo5118.cn

[B06] 遍历字典 / 对象
来源：https://oz.zhonguo5118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://aa.zhonguo7118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://sw.zhonguo4118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://gl.zhonguo8118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://wm.zhonguo1118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://sw.zhonguo7118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://oj.zhonguo4118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://if.zhonguo7118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://ps.zhonguo1118.cn

[B07] while 循环
来源：https://df.zhonguo3118.cn

Py:   while i < 10: i += 1
来源：https://ar.zhonguo3118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://tu.zhonguo8118.cn

JS:   while (i < 10) { i++; }
来源：https://gy.zhonguo4118.cn

TS:   while (i < 10) { i++; }
来源：https://ab.zhonguo5118.cn

Java: while (i < 10) { i++; }
来源：https://jo.zhonguo2118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://an.zhonguo2118.cn

Ruby: while i < 10; i += 1; end
来源：https://za.zhonguo8118.cn

C#:   while (i < 10) { i++; }
来源：https://sa.zhonguo7118.cn

[B08] do-while（至少执行一次）
来源：https://yj.zhonguo7118.cn

Py:   # 无 do-while：用 while True + break
来源：https://rz.zhonguo1118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://fl.zhonguo5118.cn

JS:   do { i++; } while (i < 10);
来源：https://ao.zhonguo4118.cn

TS:   do { i++; } while (i < 10);
来源：https://fr.zhonguo8118.cn

Java: do { i++; } while (i < 10);
来源：https://gk.zhonguo4118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://bh.zhonguo2118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://ap.zhonguo7118.cn

C#:   do { i++; } while (i < 10);
来源：https://rj.zhonguo4118.cn

[B09] break 与 continue
来源：https://vy.zhonguo7118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://uv.zhonguo1118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://mt.zhonguo5118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://sp.zhonguo5118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://qc.zhonguo2118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://yz.zhonguo7118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://yy.zhonguo1118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://ji.zhonguo3118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://lx.zhonguo4118.cn

[B10] 遍历同时拿索引
来源：https://ip.zhonguo8118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://ub.zhonguo2118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://tl.zhonguo7118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://qk.zhonguo4118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://zp.zhonguo8118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://ve.zhonguo6118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://yb.zhonguo7118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://pq.zhonguo2118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://os.zhonguo5118.cn

[B11] 生成数字序列 / 区间
来源：https://we.zhonguo1118.cn

Py:   list(range(0, 10, 2))
来源：https://fg.zhonguo8118.cn

PHP:  range(0, 10, 2);
来源：https://wa.zhonguo5118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://hm.zhonguo4118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://wp.zhonguo3118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://xy.zhonguo4118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://bv.zhonguo4118.cn

Ruby: (0...10).step(2).to_a
来源：https://bi.zhonguo8118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://rw.zhonguo4118.cn

[B12] 跳出多层循环
来源：https://wl.zhonguo6118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://ei.zhonguo4118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://eo.zhonguo8118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://jg.zhonguo7118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://ve.zhonguo3118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://ex.zhonguo5118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://ge.zhonguo2118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://ef.zhonguo4118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://rk.zhonguo5118.cn

[B13] 判断是否为数字
来源：https://mg.zhonguo5118.cn

Py:   isinstance(x, (int, float))
来源：https://gc.zhonguo1118.cn

PHP:  is_numeric($x)
来源：https://xz.zhonguo8118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ws.zhonguo6118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ks.zhonguo6118.cn

Java: x instanceof Number
来源：https://go.zhonguo1118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://ny.zhonguo4118.cn

Ruby: x.is_a?(Numeric)
来源：https://gg.zhonguo3118.cn

C#:   x is int or double or decimal
来源：https://qy.zhonguo6118.cn

[B14] 判断值是否在集合内
来源：https://gm.zhonguo1118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://nv.zhonguo4118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://bj.zhonguo8118.cn

JS:   [1, 2, 3].includes(x)
来源：https://sq.zhonguo5118.cn

TS:   [1, 2, 3].includes(x)
来源：https://iy.zhonguo3118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://tf.zhonguo5118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://ff.zhonguo3118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://ah.zhonguo8118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://aa.zhonguo6118.cn

[B15] 布尔运算与取反
来源：https://mq.zhonguo6118.cn

Py:   a and b or not c
来源：https://mp.zhonguo2118.cn

PHP:  $a && $b || !$c
来源：https://qh.zhonguo3118.cn

JS:   a && b || !c
来源：https://rs.zhonguo7118.cn

TS:   a && b || !c
来源：https://xu.zhonguo6118.cn

Java: a && b || !c
来源：https://wr.zhonguo4118.cn

Go:   a && b || !c
来源：https://vz.zhonguo8118.cn

Ruby: a && b || !c
来源：https://zi.zhonguo3118.cn

C#:   a && b || !c
来源：https://ns.zhonguo8118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://mv.zhonguo8118.cn

Py:   if not data: return
来源：https://bi.zhonguo7118.cn

PHP:  if (!$data) { return; }
来源：https://gi.zhonguo2118.cn

JS:   if (!data) return;
来源：https://yb.zhonguo2118.cn

TS:   if (!data) return;
来源：https://uj.zhonguo6118.cn

Java: if (data == null) return;
来源：https://oa.zhonguo8118.cn

Go:   if data == nil { return }
来源：https://ka.zhonguo4118.cn

Ruby: return if data.nil?
来源：https://ne.zhonguo2118.cn

C#:   if (data == null) return;
来源：https://ed.zhonguo8118.cn

================================================================================
来源：https://bn.zhonguo8118.cn

C. 函数与作用域
来源：https://xn.zhonguo6118.cn

================================================================================
来源：https://cx.zhonguo2118.cn

[C01] 定义函数
来源：https://ts.zhonguo3118.cn

Py:   def add(a, b): return a + b
来源：https://jf.zhonguo7118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://vo.zhonguo3118.cn

JS:   function add(a, b) { return a + b; }
来源：https://fj.zhonguo6118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://le.zhonguo3118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://om.zhonguo8118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://tk.zhonguo8118.cn

Ruby: def add(a, b); a + b; end
来源：https://dk.zhonguo3118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://ob.zhonguo3118.cn

[C02] 默认参数
来源：https://se.zhonguo6118.cn

Py:   def greet(name="World"): return name
来源：https://ns.zhonguo7118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://mr.zhonguo3118.cn

JS:   function greet(name = "World") { return name; }
来源：https://oy.zhonguo7118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://aa.zhonguo4118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://cu.zhonguo2118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://ez.zhonguo1118.cn

Ruby: def greet(name = "World") = name
来源：https://ef.zhonguo7118.cn

C#:   string Greet(string name = "World") => name;
来源：https://xf.zhonguo5118.cn

[C03] 可变参数
来源：https://pc.zhonguo5118.cn

Py:   def total(*args): return sum(args)
来源：https://jk.zhonguo2118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://hy.zhonguo4118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://pz.zhonguo3118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://wm.zhonguo4118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://xw.zhonguo7118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://mn.zhonguo5118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://fr.zhonguo7118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://bz.zhonguo6118.cn

[C04] 命名参数 / 关键字参数
来源：https://bv.zhonguo8118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://cj.zhonguo6118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://bd.zhonguo3118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://fj.zhonguo6118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://gr.zhonguo2118.cn

Java: // 无：用 Builder 模式或 record
来源：https://ry.zhonguo3118.cn

Go:   // 无：用配置结构体参数
来源：https://dq.zhonguo8118.cn

Ruby: f(a: 1, b: 2)
来源：https://rq.zhonguo8118.cn

C#:   f(a: 1, b: 2)
来源：https://je.zhonguo4118.cn

[C05] 返回多个值
来源：https://sk.zhonguo8118.cn


<!-- 参考信息 -->