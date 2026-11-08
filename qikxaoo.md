代发 wailian999

Py:   "第一行\n第二行"
来源：https://fb.zhonguo5118.cn

PHP:  "第一行\n第二行"
来源：https://sa.zhonguo5118.cn

JS:   "第一行\n第二行"
来源：https://vs.zhonguo2118.cn

TS:   "第一行\n第二行"
来源：https://jo.zhonguo6118.cn

Java: "第一行\n第二行"
来源：https://ic.zhonguo3118.cn

Go:   "第一行\n第二行"
来源：https://bf.zhonguo7118.cn

Ruby: "第一行\n第二行"
来源：https://zm.zhonguo7118.cn

C#:   "第一行\n第二行"
来源：https://ve.zhonguo1118.cn

[A14] 注释写法
来源：https://om.zhonguo1118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://gu.zhonguo2118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://mp.zhonguo7118.cn

JS:   // 单行；/* 多行 */
来源：https://si.zhonguo3118.cn

TS:   // 单行；/* 多行 */
来源：https://vt.zhonguo2118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://nb.zhonguo4118.cn

Go:   // 单行；/* 多行 */
来源：https://vh.zhonguo1118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://bc.zhonguo1118.cn

C#:   // 单行；/* 多行 */
来源：https://kv.zhonguo5118.cn

[A15] 空值判断与默认值
来源：https://ku.zhonguo7118.cn

Py:   value = data or "默认值"
来源：https://ij.zhonguo1118.cn

PHP:  $value = $data ?? "默认值";
来源：https://od.zhonguo8118.cn

JS:   const value = data ?? "默认值";
来源：https://an.zhonguo8118.cn

TS:   const value = data ?? "默认值";
来源：https://zd.zhonguo7118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://fo.zhonguo2118.cn

Go:   if data == "" { data = "默认值" }
来源：https://eb.zhonguo2118.cn

Ruby: value = data || "默认值"
来源：https://ca.zhonguo6118.cn

C#:   var value = data ?? "默认值";
来源：https://yt.zhonguo5118.cn

[A16] 真假值判断规则
来源：https://rj.zhonguo8118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://th.zhonguo6118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://fn.zhonguo3118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://un.zhonguo7118.cn

TS:   if (!x) {}
来源：https://wz.zhonguo3118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://ve.zhonguo2118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://yh.zhonguo4118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://za.zhonguo5118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://du.zhonguo1118.cn

[A17] 位运算
来源：https://hy.zhonguo2118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://bj.zhonguo5118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://qo.zhonguo1118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://db.zhonguo7118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://ie.zhonguo3118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://yu.zhonguo6118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://hu.zhonguo6118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://pj.zhonguo1118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://hv.zhonguo1118.cn

[A18] 字符与 ASCII 码互转
来源：https://qh.zhonguo5118.cn

Py:   ord("A"); chr(65)
来源：https://jb.zhonguo3118.cn

PHP:  ord("A"); chr(65)
来源：https://is.zhonguo6118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://rw.zhonguo8118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://fo.zhonguo8118.cn

Java: (int) 'A'; (char) 65
来源：https://lj.zhonguo4118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://ri.zhonguo7118.cn

Ruby: "A".ord; 65.chr
来源：https://or.zhonguo7118.cn

C#:   (int)'A'; (char)65
来源：https://wo.zhonguo2118.cn

[A19] 交换两个变量
来源：https://md.zhonguo6118.cn

Py:   a, b = b, a
来源：https://iu.zhonguo2118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://qr.zhonguo2118.cn

JS:   [a, b] = [b, a];
来源：https://au.zhonguo7118.cn

TS:   [a, b] = [b, a];
来源：https://dq.zhonguo4118.cn

Java: int t = a; a = b; b = t;
来源：https://th.zhonguo4118.cn

Go:   a, b = b, a
来源：https://xe.zhonguo1118.cn

Ruby: a, b = b, a
来源：https://aa.zhonguo2118.cn

C#:   (a, b) = (b, a);
来源：https://yv.zhonguo6118.cn

[A20] 读取标准输入
来源：https://ia.zhonguo2118.cn

Py:   name = input("请输入：")
来源：https://kn.zhonguo4118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://rx.zhonguo5118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://cs.zhonguo3118.cn

TS:   // Node.js：readline 模块
来源：https://mt.zhonguo7118.cn

Java: new Scanner(System.in).nextLine()
来源：https://bm.zhonguo4118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://ev.zhonguo6118.cn

Ruby: gets.chomp
来源：https://yd.zhonguo3118.cn

C#:   Console.ReadLine();
来源：https://ok.zhonguo8118.cn

[A21] 保留指定小数位输出
来源：https://fn.zhonguo3118.cn

Py:   f"{3.14159:.2f}"
来源：https://tu.zhonguo8118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://pn.zhonguo1118.cn

JS:   (3.14159).toFixed(2)
来源：https://vt.zhonguo2118.cn

TS:   (3.14159).toFixed(2)
来源：https://oz.zhonguo4118.cn

Java: String.format("%.2f", 3.14159)
来源：https://mj.zhonguo1118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://ob.zhonguo1118.cn

Ruby: format("%.2f", 3.14159)
来源：https://rv.zhonguo7118.cn

C#:   3.14159.ToString("F2")
来源：https://wn.zhonguo2118.cn

[A22] 获取字符串长度
来源：https://lz.zhonguo2118.cn

Py:   len(s)
来源：https://gq.zhonguo7118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://qg.zhonguo8118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://wh.zhonguo1118.cn

TS:   s.length
来源：https://ev.zhonguo7118.cn

Java: s.length()
来源：https://vl.zhonguo5118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://tn.zhonguo4118.cn

Ruby: s.length
来源：https://ta.zhonguo1118.cn

C#:   s.Length
来源：https://gg.zhonguo2118.cn

[A23] 大小写转换
来源：https://sg.zhonguo1118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://gg.zhonguo2118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://kx.zhonguo3118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://la.zhonguo8118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://rx.zhonguo5118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://ty.zhonguo3118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://qv.zhonguo5118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://dd.zhonguo2118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://tz.zhonguo3118.cn

[A24] 去除首尾空白
来源：https://zc.zhonguo6118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://yz.zhonguo2118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://zm.zhonguo8118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://qb.zhonguo3118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://ll.zhonguo1118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://nu.zhonguo6118.cn

Go:   strings.TrimSpace(s)
来源：https://uh.zhonguo1118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://lc.zhonguo7118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://nv.zhonguo3118.cn

[A25] 字符串比较
来源：https://ip.zhonguo4118.cn

Py:   s1 == s2; s1 != s2
来源：https://cy.zhonguo5118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://tu.zhonguo2118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://tm.zhonguo2118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://ik.zhonguo6118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://lw.zhonguo7118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://nz.zhonguo7118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://qw.zhonguo4118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://af.zhonguo1118.cn

[A26] 类型转换总览
来源：https://iw.zhonguo3118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://se.zhonguo8118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://av.zhonguo2118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://vr.zhonguo2118.cn

TS:   Number() String() Boolean() x as number
来源：https://xw.zhonguo4118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://uo.zhonguo7118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://iz.zhonguo2118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://xx.zhonguo3118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://fw.zhonguo2118.cn

================================================================================
来源：https://sm.zhonguo7118.cn

B. 流程控制
来源：https://ws.zhonguo2118.cn

================================================================================
来源：https://ly.zhonguo1118.cn

[B01] 条件判断 if / else
来源：https://rs.zhonguo5118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://vk.zhonguo4118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://bs.zhonguo2118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://ms.zhonguo6118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://cv.zhonguo5118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://vf.zhonguo2118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://xv.zhonguo3118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://ay.zhonguo5118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://xf.zhonguo3118.cn

[B02] 多分支 else if / elif
来源：https://uc.zhonguo3118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://hs.zhonguo4118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://oc.zhonguo1118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://pl.zhonguo5118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ae.zhonguo4118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ju.zhonguo2118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://xj.zhonguo2118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://yi.zhonguo1118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://cj.zhonguo3118.cn

[B03] switch / match / case
来源：https://ub.zhonguo6118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://er.zhonguo8118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://gb.zhonguo6118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://xm.zhonguo8118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://wt.zhonguo5118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://jy.zhonguo6118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://xu.zhonguo5118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://lv.zhonguo7118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://sm.zhonguo1118.cn

[B04] for 计数循环
来源：https://dh.zhonguo4118.cn

Py:   for i in range(10): print(i)
来源：https://di.zhonguo7118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://ny.zhonguo3118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://xz.zhonguo8118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://zy.zhonguo2118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://sp.zhonguo2118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://tr.zhonguo5118.cn

Ruby: 10.times { |i| puts i }
来源：https://bu.zhonguo4118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://jm.zhonguo2118.cn

[B05] 遍历数组 / 列表
来源：https://bk.zhonguo6118.cn

Py:   for item in arr: print(item)
来源：https://fi.zhonguo1118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://iy.zhonguo2118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://ta.zhonguo2118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://hw.zhonguo4118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://wn.zhonguo1118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://vq.zhonguo8118.cn

Ruby: arr.each { |item| puts item }
来源：https://lf.zhonguo3118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://pv.zhonguo3118.cn

[B06] 遍历字典 / 对象
来源：https://ly.zhonguo4118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://od.zhonguo1118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://zx.zhonguo6118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://kl.zhonguo5118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://gj.zhonguo7118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://zy.zhonguo4118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://mm.zhonguo5118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://vj.zhonguo3118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://go.zhonguo5118.cn

[B07] while 循环
来源：https://wk.zhonguo7118.cn

Py:   while i < 10: i += 1
来源：https://uq.zhonguo7118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://oc.zhonguo2118.cn

JS:   while (i < 10) { i++; }
来源：https://hk.zhonguo1118.cn

TS:   while (i < 10) { i++; }
来源：https://qs.zhonguo8118.cn

Java: while (i < 10) { i++; }
来源：https://ar.zhonguo5118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://mv.zhonguo6118.cn

Ruby: while i < 10; i += 1; end
来源：https://gl.zhonguo2118.cn

C#:   while (i < 10) { i++; }
来源：https://dw.zhonguo1118.cn

[B08] do-while（至少执行一次）
来源：https://rb.zhonguo5118.cn

Py:   # 无 do-while：用 while True + break
来源：https://em.zhonguo3118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://uy.zhonguo3118.cn

JS:   do { i++; } while (i < 10);
来源：https://ro.zhonguo1118.cn

TS:   do { i++; } while (i < 10);
来源：https://iq.zhonguo3118.cn

Java: do { i++; } while (i < 10);
来源：https://bv.zhonguo4118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://tx.zhonguo3118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://ts.zhonguo5118.cn

C#:   do { i++; } while (i < 10);
来源：https://rv.zhonguo2118.cn

[B09] break 与 continue
来源：https://ve.zhonguo4118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://oe.zhonguo6118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://qt.zhonguo1118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://it.zhonguo2118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ow.zhonguo4118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://go.zhonguo5118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://mj.zhonguo8118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://xy.zhonguo1118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://pa.zhonguo5118.cn

[B10] 遍历同时拿索引
来源：https://vo.zhonguo1118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://iq.zhonguo5118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://gd.zhonguo2118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://pr.zhonguo4118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://ml.zhonguo6118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://lz.zhonguo2118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://cb.zhonguo2118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://sn.zhonguo1118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://cc.zhonguo4118.cn

[B11] 生成数字序列 / 区间
来源：https://ls.zhonguo5118.cn

Py:   list(range(0, 10, 2))
来源：https://sv.zhonguo4118.cn

PHP:  range(0, 10, 2);
来源：https://in.zhonguo3118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://yq.zhonguo6118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://zc.zhonguo6118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://ub.zhonguo8118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://wl.zhonguo1118.cn

Ruby: (0...10).step(2).to_a
来源：https://ke.zhonguo7118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://de.zhonguo6118.cn

[B12] 跳出多层循环
来源：https://nl.zhonguo1118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://wv.zhonguo5118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://xq.zhonguo6118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://vz.zhonguo1118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://wm.zhonguo8118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://ca.zhonguo3118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://cv.zhonguo8118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://do.zhonguo4118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://wz.zhonguo1118.cn

[B13] 判断是否为数字
来源：https://cl.zhonguo4118.cn

Py:   isinstance(x, (int, float))
来源：https://pw.zhonguo4118.cn

PHP:  is_numeric($x)
来源：https://uw.zhonguo4118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ck.zhonguo4118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ox.zhonguo6118.cn

Java: x instanceof Number
来源：https://xy.zhonguo7118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://vk.zhonguo5118.cn

Ruby: x.is_a?(Numeric)
来源：https://rg.zhonguo7118.cn

C#:   x is int or double or decimal
来源：https://ge.zhonguo8118.cn

[B14] 判断值是否在集合内
来源：https://nk.zhonguo7118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://un.zhonguo1118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://jx.zhonguo1118.cn

JS:   [1, 2, 3].includes(x)
来源：https://tm.zhonguo7118.cn

TS:   [1, 2, 3].includes(x)
来源：https://gf.zhonguo2118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://mi.zhonguo7118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://op.zhonguo4118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://zh.zhonguo7118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://jm.zhonguo4118.cn

[B15] 布尔运算与取反
来源：https://qh.zhonguo4118.cn

Py:   a and b or not c
来源：https://iy.zhonguo4118.cn

PHP:  $a && $b || !$c
来源：https://jw.zhonguo1118.cn

JS:   a && b || !c
来源：https://tt.zhonguo6118.cn

TS:   a && b || !c
来源：https://ge.zhonguo2118.cn

Java: a && b || !c
来源：https://ef.zhonguo2118.cn

Go:   a && b || !c
来源：https://sl.zhonguo2118.cn

Ruby: a && b || !c
来源：https://gd.zhonguo1118.cn

C#:   a && b || !c
来源：https://tz.zhonguo5118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://at.zhonguo4118.cn

Py:   if not data: return
来源：https://qx.zhonguo8118.cn

PHP:  if (!$data) { return; }
来源：https://ox.zhonguo2118.cn

JS:   if (!data) return;
来源：https://vd.zhonguo5118.cn

TS:   if (!data) return;
来源：https://ab.zhonguo7118.cn

Java: if (data == null) return;
来源：https://fu.zhonguo3118.cn

Go:   if data == nil { return }
来源：https://hj.zhonguo3118.cn

Ruby: return if data.nil?
来源：https://kc.zhonguo7118.cn

C#:   if (data == null) return;
来源：https://ve.zhonguo4118.cn

================================================================================
来源：https://zz.zhonguo3118.cn

C. 函数与作用域
来源：https://re.zhonguo5118.cn

================================================================================
来源：https://mn.zhonguo5118.cn

[C01] 定义函数
来源：https://zx.zhonguo7118.cn

Py:   def add(a, b): return a + b
来源：https://nl.zhonguo6118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://gi.zhonguo1118.cn

JS:   function add(a, b) { return a + b; }
来源：https://qc.zhonguo8118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://hj.zhonguo6118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://kt.zhonguo2118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://dv.zhonguo1118.cn

Ruby: def add(a, b); a + b; end
来源：https://qb.zhonguo8118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://sd.zhonguo8118.cn

[C02] 默认参数
来源：https://ct.zhonguo3118.cn

Py:   def greet(name="World"): return name
来源：https://rn.zhonguo7118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://eg.zhonguo1118.cn

JS:   function greet(name = "World") { return name; }
来源：https://ix.zhonguo1118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://bw.zhonguo4118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://ls.zhonguo6118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://xn.zhonguo7118.cn

Ruby: def greet(name = "World") = name
来源：https://ic.zhonguo7118.cn

C#:   string Greet(string name = "World") => name;
来源：https://ip.zhonguo1118.cn

[C03] 可变参数
来源：https://sy.zhonguo3118.cn

Py:   def total(*args): return sum(args)
来源：https://xa.zhonguo2118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://gx.zhonguo1118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://nq.zhonguo7118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://ca.zhonguo7118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://qc.zhonguo4118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://kd.zhonguo6118.cn


<!-- 参考信息 -->