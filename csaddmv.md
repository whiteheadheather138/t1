代发 wailian999

Ruby: value = data || "默认值"
来源：https://qm.zhonguo4118.cn

C#:   var value = data ?? "默认值";
来源：https://wn.zhonguo4118.cn

[A16] 真假值判断规则
来源：https://rv.zhonguo5118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://jn.zhonguo6118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://fv.zhonguo3118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://ys.zhonguo8118.cn

TS:   if (!x) {}
来源：https://pw.zhonguo2118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://hx.zhonguo7118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://yu.zhonguo4118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://ub.zhonguo6118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://gc.zhonguo8118.cn

[A17] 位运算
来源：https://er.zhonguo2118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ok.zhonguo6118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://dc.zhonguo4118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://vd.zhonguo6118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://ck.zhonguo2118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://qs.zhonguo5118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://zb.zhonguo2118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://cj.zhonguo8118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://nx.zhonguo4118.cn

[A18] 字符与 ASCII 码互转
来源：https://ku.zhonguo5118.cn

Py:   ord("A"); chr(65)
来源：https://wr.zhonguo1118.cn

PHP:  ord("A"); chr(65)
来源：https://zz.zhonguo6118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://qq.zhonguo8118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://mh.zhonguo8118.cn

Java: (int) 'A'; (char) 65
来源：https://cg.zhonguo5118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://gt.zhonguo1118.cn

Ruby: "A".ord; 65.chr
来源：https://ic.zhonguo3118.cn

C#:   (int)'A'; (char)65
来源：https://de.zhonguo2118.cn

[A19] 交换两个变量
来源：https://ug.zhonguo2118.cn

Py:   a, b = b, a
来源：https://sm.zhonguo2118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://yy.zhonguo1118.cn

JS:   [a, b] = [b, a];
来源：https://tm.zhonguo7118.cn

TS:   [a, b] = [b, a];
来源：https://yf.zhonguo4118.cn

Java: int t = a; a = b; b = t;
来源：https://nk.zhonguo3118.cn

Go:   a, b = b, a
来源：https://ax.zhonguo3118.cn

Ruby: a, b = b, a
来源：https://kf.zhonguo8118.cn

C#:   (a, b) = (b, a);
来源：https://eo.zhonguo8118.cn

[A20] 读取标准输入
来源：https://ys.zhonguo8118.cn

Py:   name = input("请输入：")
来源：https://ee.zhonguo5118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://vw.zhonguo8118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://ha.zhonguo6118.cn

TS:   // Node.js：readline 模块
来源：https://si.zhonguo4118.cn

Java: new Scanner(System.in).nextLine()
来源：https://mf.zhonguo4118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://gy.zhonguo2118.cn

Ruby: gets.chomp
来源：https://tv.zhonguo7118.cn

C#:   Console.ReadLine();
来源：https://ch.zhonguo6118.cn

[A21] 保留指定小数位输出
来源：https://wk.zhonguo3118.cn

Py:   f"{3.14159:.2f}"
来源：https://go.zhonguo6118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://hw.zhonguo6118.cn

JS:   (3.14159).toFixed(2)
来源：https://ud.zhonguo3118.cn

TS:   (3.14159).toFixed(2)
来源：https://mn.zhonguo4118.cn

Java: String.format("%.2f", 3.14159)
来源：https://sb.zhonguo1118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://ry.zhonguo2118.cn

Ruby: format("%.2f", 3.14159)
来源：https://ky.zhonguo8118.cn

C#:   3.14159.ToString("F2")
来源：https://tx.zhonguo7118.cn

[A22] 获取字符串长度
来源：https://im.zhonguo5118.cn

Py:   len(s)
来源：https://lk.zhonguo4118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://yf.zhonguo3118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://tb.zhonguo4118.cn

TS:   s.length
来源：https://yc.zhonguo8118.cn

Java: s.length()
来源：https://gf.zhonguo8118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://zp.zhonguo1118.cn

Ruby: s.length
来源：https://rn.zhonguo5118.cn

C#:   s.Length
来源：https://qh.zhonguo2118.cn

[A23] 大小写转换
来源：https://ft.zhonguo4118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://yo.zhonguo6118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://ph.zhonguo7118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://yf.zhonguo8118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://ao.zhonguo3118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://xm.zhonguo2118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://sa.zhonguo7118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://qy.zhonguo4118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://xa.zhonguo2118.cn

[A24] 去除首尾空白
来源：https://uf.zhonguo6118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://gy.zhonguo7118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://mc.zhonguo4118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://zh.zhonguo5118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://rx.zhonguo6118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://ht.zhonguo2118.cn

Go:   strings.TrimSpace(s)
来源：https://lk.zhonguo7118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://wq.zhonguo2118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://he.zhonguo2118.cn

[A25] 字符串比较
来源：https://sn.zhonguo6118.cn

Py:   s1 == s2; s1 != s2
来源：https://zp.zhonguo2118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://rn.zhonguo2118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://nt.zhonguo8118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://bc.zhonguo7118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://jc.zhonguo1118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://le.zhonguo3118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://fs.zhonguo7118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://qj.zhonguo4118.cn

[A26] 类型转换总览
来源：https://nk.zhonguo5118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://uu.zhonguo4118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://ev.zhonguo6118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://wi.zhonguo2118.cn

TS:   Number() String() Boolean() x as number
来源：https://nh.zhonguo5118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://hw.zhonguo6118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://qf.zhonguo1118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://qa.zhonguo8118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://ay.zhonguo6118.cn

================================================================================
来源：https://qe.zhonguo1118.cn

B. 流程控制
来源：https://pu.zhonguo6118.cn

================================================================================
来源：https://zl.zhonguo8118.cn

[B01] 条件判断 if / else
来源：https://zs.zhonguo5118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://pg.zhonguo4118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://dp.zhonguo8118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://oh.zhonguo8118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://ht.zhonguo3118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://qy.zhonguo7118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://us.zhonguo2118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://cz.zhonguo4118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://rs.zhonguo7118.cn

[B02] 多分支 else if / elif
来源：https://qv.zhonguo1118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://bk.zhonguo5118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://ix.zhonguo7118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://hs.zhonguo1118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://fu.zhonguo2118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://dn.zhonguo6118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://sp.zhonguo8118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://be.zhonguo1118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://gz.zhonguo5118.cn

[B03] switch / match / case
来源：https://cw.zhonguo8118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://wb.zhonguo1118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://zd.zhonguo2118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://rj.zhonguo2118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://px.zhonguo4118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://ww.zhonguo7118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://zd.zhonguo2118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://zs.zhonguo7118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://fw.zhonguo4118.cn

[B04] for 计数循环
来源：https://nv.zhonguo1118.cn

Py:   for i in range(10): print(i)
来源：https://jh.zhonguo6118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://cx.zhonguo8118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://jb.zhonguo2118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://ph.zhonguo5118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://vb.zhonguo7118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://cp.zhonguo6118.cn

Ruby: 10.times { |i| puts i }
来源：https://nw.zhonguo5118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://gi.zhonguo1118.cn

[B05] 遍历数组 / 列表
来源：https://rv.zhonguo2118.cn

Py:   for item in arr: print(item)
来源：https://ox.zhonguo8118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://sl.zhonguo7118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://eo.zhonguo4118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://cl.zhonguo6118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://zq.zhonguo8118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://zx.zhonguo5118.cn

Ruby: arr.each { |item| puts item }
来源：https://sg.zhonguo8118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://ls.zhonguo6118.cn

[B06] 遍历字典 / 对象
来源：https://rg.zhonguo8118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://th.zhonguo2118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://en.zhonguo3118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://bk.zhonguo1118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://py.zhonguo4118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://tq.zhonguo6118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://bt.zhonguo6118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://qa.zhonguo1118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://kv.zhonguo3118.cn

[B07] while 循环
来源：https://tb.zhonguo1118.cn

Py:   while i < 10: i += 1
来源：https://dk.zhonguo8118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://zo.zhonguo5118.cn

JS:   while (i < 10) { i++; }
来源：https://hl.zhonguo5118.cn

TS:   while (i < 10) { i++; }
来源：https://pg.zhonguo4118.cn

Java: while (i < 10) { i++; }
来源：https://hg.zhonguo6118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://zo.zhonguo4118.cn

Ruby: while i < 10; i += 1; end
来源：https://aw.zhonguo6118.cn

C#:   while (i < 10) { i++; }
来源：https://pf.zhonguo6118.cn

[B08] do-while（至少执行一次）
来源：https://qi.zhonguo3118.cn

Py:   # 无 do-while：用 while True + break
来源：https://ua.zhonguo7118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://uo.zhonguo4118.cn

JS:   do { i++; } while (i < 10);
来源：https://ue.zhonguo6118.cn

TS:   do { i++; } while (i < 10);
来源：https://aj.zhonguo6118.cn

Java: do { i++; } while (i < 10);
来源：https://kh.zhonguo7118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://pf.zhonguo1118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://hk.zhonguo5118.cn

C#:   do { i++; } while (i < 10);
来源：https://zx.zhonguo3118.cn

[B09] break 与 continue
来源：https://ok.zhonguo4118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://jn.zhonguo8118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://ad.zhonguo5118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://br.zhonguo8118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://kc.zhonguo5118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ab.zhonguo1118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://nu.zhonguo5118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://gh.zhonguo6118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://lt.zhonguo7118.cn

[B10] 遍历同时拿索引
来源：https://dh.zhonguo6118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://cz.zhonguo2118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://bg.zhonguo3118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://ad.zhonguo4118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://xz.zhonguo4118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://xm.zhonguo1118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://pq.zhonguo7118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://op.zhonguo2118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://cz.zhonguo1118.cn

[B11] 生成数字序列 / 区间
来源：https://kh.zhonguo3118.cn

Py:   list(range(0, 10, 2))
来源：https://dl.zhonguo5118.cn

PHP:  range(0, 10, 2);
来源：https://jq.zhonguo6118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://th.zhonguo4118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://zb.zhonguo1118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://bi.zhonguo2118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://hf.zhonguo5118.cn

Ruby: (0...10).step(2).to_a
来源：https://hi.zhonguo1118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://sk.zhonguo4118.cn

[B12] 跳出多层循环
来源：https://au.zhonguo4118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://sw.zhonguo5118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://dv.zhonguo7118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://jw.zhonguo2118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://tb.zhonguo3118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://pn.zhonguo3118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://ke.zhonguo3118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://ic.zhonguo3118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://ny.zhonguo7118.cn

[B13] 判断是否为数字
来源：https://pm.zhonguo5118.cn

Py:   isinstance(x, (int, float))
来源：https://uq.zhonguo2118.cn

PHP:  is_numeric($x)
来源：https://wu.zhonguo2118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://yj.zhonguo8118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://vx.zhonguo6118.cn

Java: x instanceof Number
来源：https://no.zhonguo3118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://bg.zhonguo6118.cn

Ruby: x.is_a?(Numeric)
来源：https://pz.zhonguo3118.cn

C#:   x is int or double or decimal
来源：https://sh.zhonguo6118.cn

[B14] 判断值是否在集合内
来源：https://rq.zhonguo5118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://bo.zhonguo6118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://pn.zhonguo6118.cn

JS:   [1, 2, 3].includes(x)
来源：https://it.zhonguo2118.cn

TS:   [1, 2, 3].includes(x)
来源：https://pr.zhonguo1118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://sp.zhonguo5118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://kz.zhonguo5118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://wk.zhonguo2118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://yw.zhonguo4118.cn

[B15] 布尔运算与取反
来源：https://zt.zhonguo1118.cn

Py:   a and b or not c
来源：https://fx.zhonguo6118.cn

PHP:  $a && $b || !$c
来源：https://ih.zhonguo3118.cn

JS:   a && b || !c
来源：https://ki.zhonguo3118.cn

TS:   a && b || !c
来源：https://uw.zhonguo8118.cn

Java: a && b || !c
来源：https://zr.zhonguo7118.cn

Go:   a && b || !c
来源：https://lo.zhonguo5118.cn

Ruby: a && b || !c
来源：https://co.zhonguo4118.cn

C#:   a && b || !c
来源：https://dv.zhonguo4118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://ss.zhonguo2118.cn

Py:   if not data: return
来源：https://dg.zhonguo5118.cn

PHP:  if (!$data) { return; }
来源：https://bt.zhonguo5118.cn

JS:   if (!data) return;
来源：https://eg.zhonguo7118.cn

TS:   if (!data) return;
来源：https://ld.zhonguo5118.cn

Java: if (data == null) return;
来源：https://vn.zhonguo1118.cn

Go:   if data == nil { return }
来源：https://cn.zhonguo4118.cn

Ruby: return if data.nil?
来源：https://qf.zhonguo1118.cn

C#:   if (data == null) return;
来源：https://wz.zhonguo4118.cn

================================================================================
来源：https://di.zhonguo8118.cn

C. 函数与作用域
来源：https://an.zhonguo2118.cn

================================================================================
来源：https://tt.zhonguo6118.cn

[C01] 定义函数
来源：https://jq.zhonguo7118.cn

Py:   def add(a, b): return a + b
来源：https://ix.zhonguo8118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://ty.zhonguo6118.cn

JS:   function add(a, b) { return a + b; }
来源：https://fo.zhonguo8118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://xm.zhonguo3118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://ut.zhonguo7118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://wc.zhonguo7118.cn

Ruby: def add(a, b); a + b; end
来源：https://zl.zhonguo8118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://zg.zhonguo3118.cn

[C02] 默认参数
来源：https://ph.zhonguo5118.cn

Py:   def greet(name="World"): return name
来源：https://hg.zhonguo3118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://bz.zhonguo6118.cn

JS:   function greet(name = "World") { return name; }
来源：https://ml.zhonguo4118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://pl.zhonguo3118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://fz.zhonguo2118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://fh.zhonguo2118.cn

Ruby: def greet(name = "World") = name
来源：https://nk.zhonguo1118.cn

C#:   string Greet(string name = "World") => name;
来源：https://zo.zhonguo1118.cn

[C03] 可变参数
来源：https://ly.zhonguo6118.cn

Py:   def total(*args): return sum(args)
来源：https://yc.zhonguo1118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://qx.zhonguo1118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://me.zhonguo5118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://ax.zhonguo7118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://fo.zhonguo8118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://lc.zhonguo7118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://ql.zhonguo4118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://ds.zhonguo7118.cn

[C04] 命名参数 / 关键字参数
来源：https://rv.zhonguo6118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://wi.zhonguo2118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://jk.zhonguo7118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://qg.zhonguo2118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://ie.zhonguo8118.cn

Java: // 无：用 Builder 模式或 record
来源：https://df.zhonguo6118.cn

Go:   // 无：用配置结构体参数
来源：https://cq.zhonguo2118.cn

Ruby: f(a: 1, b: 2)
来源：https://ze.zhonguo3118.cn

C#:   f(a: 1, b: 2)
来源：https://ti.zhonguo1118.cn

[C05] 返回多个值
来源：https://yp.zhonguo3118.cn

Py:   return a, b
来源：https://tm.zhonguo7118.cn

PHP:  return [$a, $b];
来源：https://yt.zhonguo5118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://co.zhonguo7118.cn

TS:   return { a, b };
来源：https://ya.zhonguo5118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://eu.zhonguo1118.cn

Go:   return a, b
来源：https://wq.zhonguo3118.cn

Ruby: return a, b
来源：https://by.zhonguo1118.cn

C#:   return (a, b);              // ValueTuple
来源：https://bs.zhonguo3118.cn

[C06] 匿名函数 / lambda
来源：https://ze.zhonguo1118.cn

Py:   square = lambda x: x * x
来源：https://eu.zhonguo6118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://er.zhonguo7118.cn

JS:   const square = x => x * x;
来源：https://be.zhonguo2118.cn


<!-- 参考信息 -->