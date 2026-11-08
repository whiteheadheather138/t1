代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：https://ja.zhonguo4118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://mn.zhonguo6118.cn

[A12] 字符串插值 / 格式化
来源：https://yg.zhonguo6118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://et.zhonguo3118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://eb.zhonguo4118.cn

JS:   `Hello, ${name}!`
来源：https://ig.zhonguo4118.cn

TS:   `Hello, ${name}!`
来源：https://gs.zhonguo6118.cn

Java: "Hello, %s!".formatted(name)
来源：https://ex.zhonguo2118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://ig.zhonguo1118.cn

Ruby: "Hello, #{name}!"
来源：https://ca.zhonguo4118.cn

C#:   $"Hello, {name}!"
来源：https://hx.zhonguo2118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://co.zhonguo2118.cn

Py:   "第一行\n第二行"
来源：https://wp.zhonguo6118.cn

PHP:  "第一行\n第二行"
来源：https://de.zhonguo8118.cn

JS:   "第一行\n第二行"
来源：https://jm.zhonguo3118.cn

TS:   "第一行\n第二行"
来源：https://pq.zhonguo2118.cn

Java: "第一行\n第二行"
来源：https://gb.zhonguo7118.cn

Go:   "第一行\n第二行"
来源：https://lb.zhonguo4118.cn

Ruby: "第一行\n第二行"
来源：https://ol.zhonguo7118.cn

C#:   "第一行\n第二行"
来源：https://nw.zhonguo2118.cn

[A14] 注释写法
来源：https://xf.zhonguo3118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://dt.zhonguo4118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://ya.zhonguo8118.cn

JS:   // 单行；/* 多行 */
来源：https://jz.zhonguo1118.cn

TS:   // 单行；/* 多行 */
来源：https://pj.zhonguo1118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://df.zhonguo3118.cn

Go:   // 单行；/* 多行 */
来源：https://js.zhonguo4118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://kj.zhonguo8118.cn

C#:   // 单行；/* 多行 */
来源：https://iv.zhonguo8118.cn

[A15] 空值判断与默认值
来源：https://we.zhonguo5118.cn

Py:   value = data or "默认值"
来源：https://ws.zhonguo2118.cn

PHP:  $value = $data ?? "默认值";
来源：https://no.zhonguo7118.cn

JS:   const value = data ?? "默认值";
来源：https://cv.zhonguo5118.cn

TS:   const value = data ?? "默认值";
来源：https://xk.zhonguo1118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://so.zhonguo3118.cn

Go:   if data == "" { data = "默认值" }
来源：https://tt.zhonguo4118.cn

Ruby: value = data || "默认值"
来源：https://zg.zhonguo2118.cn

C#:   var value = data ?? "默认值";
来源：https://ks.zhonguo7118.cn

[A16] 真假值判断规则
来源：https://nl.zhonguo3118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://fv.zhonguo1118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://gv.zhonguo5118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://nb.zhonguo2118.cn

TS:   if (!x) {}
来源：https://hh.zhonguo4118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://rx.zhonguo5118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://uw.zhonguo2118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://fu.zhonguo3118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://lh.zhonguo5118.cn

[A17] 位运算
来源：https://fj.zhonguo3118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ty.zhonguo1118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://aa.zhonguo7118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://vm.zhonguo7118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://no.zhonguo4118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://lo.zhonguo2118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://ja.zhonguo5118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ju.zhonguo6118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ta.zhonguo6118.cn

[A18] 字符与 ASCII 码互转
来源：https://ro.zhonguo2118.cn

Py:   ord("A"); chr(65)
来源：https://ct.zhonguo2118.cn

PHP:  ord("A"); chr(65)
来源：https://cl.zhonguo8118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://wd.zhonguo2118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://mm.zhonguo1118.cn

Java: (int) 'A'; (char) 65
来源：https://qu.zhonguo4118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://rc.zhonguo7118.cn

Ruby: "A".ord; 65.chr
来源：https://zh.zhonguo2118.cn

C#:   (int)'A'; (char)65
来源：https://fv.zhonguo5118.cn

[A19] 交换两个变量
来源：https://se.zhonguo4118.cn

Py:   a, b = b, a
来源：https://bd.zhonguo6118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://tn.zhonguo6118.cn

JS:   [a, b] = [b, a];
来源：https://it.zhonguo1118.cn

TS:   [a, b] = [b, a];
来源：https://jg.zhonguo5118.cn

Java: int t = a; a = b; b = t;
来源：https://nz.zhonguo7118.cn

Go:   a, b = b, a
来源：https://jw.zhonguo8118.cn

Ruby: a, b = b, a
来源：https://tj.zhonguo8118.cn

C#:   (a, b) = (b, a);
来源：https://bt.zhonguo6118.cn

[A20] 读取标准输入
来源：https://et.zhonguo5118.cn

Py:   name = input("请输入：")
来源：https://rs.zhonguo7118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://gw.zhonguo5118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://cn.zhonguo6118.cn

TS:   // Node.js：readline 模块
来源：https://zu.zhonguo8118.cn

Java: new Scanner(System.in).nextLine()
来源：https://xj.zhonguo5118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://jq.zhonguo5118.cn

Ruby: gets.chomp
来源：https://cn.zhonguo1118.cn

C#:   Console.ReadLine();
来源：https://op.zhonguo3118.cn

[A21] 保留指定小数位输出
来源：https://uh.zhonguo6118.cn

Py:   f"{3.14159:.2f}"
来源：https://nn.zhonguo7118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://jl.zhonguo6118.cn

JS:   (3.14159).toFixed(2)
来源：https://xg.zhonguo1118.cn

TS:   (3.14159).toFixed(2)
来源：https://pq.zhonguo8118.cn

Java: String.format("%.2f", 3.14159)
来源：https://iu.zhonguo1118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://st.zhonguo5118.cn

Ruby: format("%.2f", 3.14159)
来源：https://su.zhonguo3118.cn

C#:   3.14159.ToString("F2")
来源：https://sl.zhonguo1118.cn

[A22] 获取字符串长度
来源：https://dz.zhonguo6118.cn

Py:   len(s)
来源：https://ad.zhonguo2118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://ib.zhonguo6118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://lx.zhonguo3118.cn

TS:   s.length
来源：https://ri.zhonguo6118.cn

Java: s.length()
来源：https://en.zhonguo4118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://br.zhonguo3118.cn

Ruby: s.length
来源：https://pg.zhonguo7118.cn

C#:   s.Length
来源：https://df.zhonguo1118.cn

[A23] 大小写转换
来源：https://el.zhonguo5118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://gx.zhonguo7118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://qe.zhonguo1118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://be.zhonguo2118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://vw.zhonguo1118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://kh.zhonguo4118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://tg.zhonguo4118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://qn.zhonguo4118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://mh.zhonguo5118.cn

[A24] 去除首尾空白
来源：https://bt.zhonguo1118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://tp.zhonguo1118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://ug.zhonguo7118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://fo.zhonguo1118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://wb.zhonguo1118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://fr.zhonguo3118.cn

Go:   strings.TrimSpace(s)
来源：https://wu.zhonguo1118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://vq.zhonguo5118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://tn.zhonguo5118.cn

[A25] 字符串比较
来源：https://no.zhonguo5118.cn

Py:   s1 == s2; s1 != s2
来源：https://na.zhonguo6118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://wl.zhonguo7118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://at.zhonguo1118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://qg.zhonguo3118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://rn.zhonguo7118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://mf.zhonguo6118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://dm.zhonguo4118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://he.zhonguo1118.cn

[A26] 类型转换总览
来源：https://jw.zhonguo6118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://lc.zhonguo1118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://nk.zhonguo1118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://da.zhonguo1118.cn

TS:   Number() String() Boolean() x as number
来源：https://gx.zhonguo3118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://jv.zhonguo5118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://ei.zhonguo5118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://dn.zhonguo5118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://ek.zhonguo1118.cn

================================================================================
来源：https://ng.zhonguo3118.cn

B. 流程控制
来源：https://ye.zhonguo5118.cn

================================================================================
来源：https://yi.zhonguo7118.cn

[B01] 条件判断 if / else
来源：https://cl.zhonguo7118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://tb.zhonguo6118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://ql.zhonguo2118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://gf.zhonguo4118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://bz.zhonguo6118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://xh.zhonguo6118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://ad.zhonguo2118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://nj.zhonguo7118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://nh.zhonguo5118.cn

[B02] 多分支 else if / elif
来源：https://ye.zhonguo3118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://dm.zhonguo1118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://gn.zhonguo5118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://fo.zhonguo1118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ud.zhonguo8118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://fq.zhonguo5118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://mj.zhonguo1118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://wi.zhonguo4118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ko.zhonguo4118.cn

[B03] switch / match / case
来源：https://qj.zhonguo1118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://yp.zhonguo6118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://yz.zhonguo1118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://ql.zhonguo5118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://dh.zhonguo7118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://ax.zhonguo6118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://ab.zhonguo3118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://fi.zhonguo6118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://xm.zhonguo2118.cn

[B04] for 计数循环
来源：https://dn.zhonguo7118.cn

Py:   for i in range(10): print(i)
来源：https://qi.zhonguo1118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://az.zhonguo8118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://dw.zhonguo8118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://kw.zhonguo3118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://en.zhonguo2118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://ar.zhonguo3118.cn

Ruby: 10.times { |i| puts i }
来源：https://zw.zhonguo5118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://of.zhonguo1118.cn

[B05] 遍历数组 / 列表
来源：https://nm.zhonguo2118.cn

Py:   for item in arr: print(item)
来源：https://aa.zhonguo1118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://gx.zhonguo2118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://hd.zhonguo5118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://rs.zhonguo5118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://tc.zhonguo1118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://ix.zhonguo4118.cn

Ruby: arr.each { |item| puts item }
来源：https://sp.zhonguo8118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://ty.zhonguo5118.cn

[B06] 遍历字典 / 对象
来源：https://uj.zhonguo7118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://ba.zhonguo5118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://qn.zhonguo8118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://cv.zhonguo2118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://of.zhonguo4118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://ea.zhonguo1118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://yg.zhonguo2118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://hy.zhonguo5118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://la.zhonguo1118.cn

[B07] while 循环
来源：https://jn.zhonguo8118.cn

Py:   while i < 10: i += 1
来源：https://gb.zhonguo6118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://eu.zhonguo2118.cn

JS:   while (i < 10) { i++; }
来源：https://ix.zhonguo7118.cn

TS:   while (i < 10) { i++; }
来源：https://up.zhonguo4118.cn

Java: while (i < 10) { i++; }
来源：https://ze.zhonguo6118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://eo.zhonguo7118.cn

Ruby: while i < 10; i += 1; end
来源：https://qi.zhonguo7118.cn

C#:   while (i < 10) { i++; }
来源：https://pk.zhonguo7118.cn

[B08] do-while（至少执行一次）
来源：https://oq.zhonguo6118.cn

Py:   # 无 do-while：用 while True + break
来源：https://jk.zhonguo3118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://rj.zhonguo8118.cn

JS:   do { i++; } while (i < 10);
来源：https://sa.zhonguo2118.cn

TS:   do { i++; } while (i < 10);
来源：https://ja.zhonguo2118.cn

Java: do { i++; } while (i < 10);
来源：https://ro.zhonguo2118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://vf.zhonguo3118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://ti.zhonguo2118.cn

C#:   do { i++; } while (i < 10);
来源：https://gw.zhonguo6118.cn

[B09] break 与 continue
来源：https://bl.zhonguo3118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://lr.zhonguo8118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://sg.zhonguo3118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://db.zhonguo2118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://fc.zhonguo7118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://oy.zhonguo8118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://ng.zhonguo7118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://rd.zhonguo8118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://yw.zhonguo7118.cn

[B10] 遍历同时拿索引
来源：https://ug.zhonguo2118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://ny.zhonguo5118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://fj.zhonguo8118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://ug.zhonguo7118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://ke.zhonguo8118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://od.zhonguo4118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://qm.zhonguo5118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://ow.zhonguo2118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://cr.zhonguo5118.cn

[B11] 生成数字序列 / 区间
来源：https://to.zhonguo1118.cn

Py:   list(range(0, 10, 2))
来源：https://zy.zhonguo1118.cn

PHP:  range(0, 10, 2);
来源：https://hm.zhonguo1118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://ad.zhonguo1118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://yl.zhonguo6118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://oj.zhonguo7118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://fc.zhonguo4118.cn

Ruby: (0...10).step(2).to_a
来源：https://xh.zhonguo7118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://ng.zhonguo2118.cn

[B12] 跳出多层循环
来源：https://ua.zhonguo5118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://uh.zhonguo4118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://di.zhonguo6118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://pp.zhonguo1118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://yc.zhonguo5118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://yd.zhonguo7118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://pi.zhonguo8118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://cc.zhonguo4118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://ee.zhonguo3118.cn

[B13] 判断是否为数字
来源：https://ag.zhonguo4118.cn

Py:   isinstance(x, (int, float))
来源：https://gp.zhonguo3118.cn

PHP:  is_numeric($x)
来源：https://xd.zhonguo8118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://is.zhonguo1118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://fd.zhonguo7118.cn

Java: x instanceof Number
来源：https://ff.zhonguo2118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://dx.zhonguo3118.cn

Ruby: x.is_a?(Numeric)
来源：https://fn.zhonguo8118.cn

C#:   x is int or double or decimal
来源：https://lg.zhonguo1118.cn

[B14] 判断值是否在集合内
来源：https://mu.zhonguo7118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://bi.zhonguo7118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://sa.zhonguo5118.cn

JS:   [1, 2, 3].includes(x)
来源：https://zo.zhonguo7118.cn

TS:   [1, 2, 3].includes(x)
来源：https://ws.zhonguo5118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://il.zhonguo1118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://oi.zhonguo6118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://qs.zhonguo7118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://di.zhonguo2118.cn

[B15] 布尔运算与取反
来源：https://qn.zhonguo5118.cn

Py:   a and b or not c
来源：https://vg.zhonguo6118.cn

PHP:  $a && $b || !$c
来源：https://xk.zhonguo7118.cn

JS:   a && b || !c
来源：https://yj.zhonguo1118.cn

TS:   a && b || !c
来源：https://eo.zhonguo3118.cn

Java: a && b || !c
来源：https://fj.zhonguo7118.cn

Go:   a && b || !c
来源：https://ek.zhonguo3118.cn

Ruby: a && b || !c
来源：https://ci.zhonguo3118.cn

C#:   a && b || !c
来源：https://pr.zhonguo1118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://yn.zhonguo3118.cn

Py:   if not data: return
来源：https://ww.zhonguo2118.cn

PHP:  if (!$data) { return; }
来源：https://te.zhonguo7118.cn

JS:   if (!data) return;
来源：https://sr.zhonguo7118.cn

TS:   if (!data) return;
来源：https://yy.zhonguo1118.cn

Java: if (data == null) return;
来源：https://ao.zhonguo1118.cn

Go:   if data == nil { return }
来源：https://xg.zhonguo1118.cn

Ruby: return if data.nil?
来源：https://jb.zhonguo3118.cn

C#:   if (data == null) return;
来源：https://sb.zhonguo3118.cn

================================================================================
来源：https://ot.zhonguo4118.cn

C. 函数与作用域
来源：https://hc.zhonguo4118.cn

================================================================================
来源：https://fe.zhonguo6118.cn

[C01] 定义函数
来源：https://hl.zhonguo6118.cn

Py:   def add(a, b): return a + b
来源：https://ii.zhonguo1118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://lh.zhonguo3118.cn

JS:   function add(a, b) { return a + b; }
来源：https://mz.zhonguo6118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://rd.zhonguo4118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://tu.zhonguo3118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://zu.zhonguo2118.cn

Ruby: def add(a, b); a + b; end
来源：https://fs.zhonguo1118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://br.zhonguo7118.cn

[C02] 默认参数
来源：https://ct.zhonguo2118.cn

Py:   def greet(name="World"): return name
来源：https://im.zhonguo8118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://dm.zhonguo2118.cn

JS:   function greet(name = "World") { return name; }
来源：https://tb.zhonguo2118.cn


<!-- 参考信息 -->