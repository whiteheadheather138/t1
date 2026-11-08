代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：https://dm.zhonguo4118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://es.zhonguo5118.cn

[A12] 字符串插值 / 格式化
来源：https://jd.zhonguo7118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://mo.zhonguo1118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://cc.zhonguo7118.cn

JS:   `Hello, ${name}!`
来源：https://gd.zhonguo8118.cn

TS:   `Hello, ${name}!`
来源：https://dt.zhonguo1118.cn

Java: "Hello, %s!".formatted(name)
来源：https://vs.zhonguo7118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://jh.zhonguo5118.cn

Ruby: "Hello, #{name}!"
来源：https://qc.zhonguo4118.cn

C#:   $"Hello, {name}!"
来源：https://vx.zhonguo4118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://jn.zhonguo4118.cn

Py:   "第一行\n第二行"
来源：https://tw.zhonguo8118.cn

PHP:  "第一行\n第二行"
来源：https://gz.zhonguo3118.cn

JS:   "第一行\n第二行"
来源：https://fy.zhonguo2118.cn

TS:   "第一行\n第二行"
来源：https://tn.zhonguo8118.cn

Java: "第一行\n第二行"
来源：https://fe.zhonguo4118.cn

Go:   "第一行\n第二行"
来源：https://gc.zhonguo2118.cn

Ruby: "第一行\n第二行"
来源：https://jd.zhonguo2118.cn

C#:   "第一行\n第二行"
来源：https://yp.zhonguo6118.cn

[A14] 注释写法
来源：https://wi.zhonguo2118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://qk.zhonguo5118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://ba.zhonguo3118.cn

JS:   // 单行；/* 多行 */
来源：https://yx.zhonguo8118.cn

TS:   // 单行；/* 多行 */
来源：https://il.zhonguo3118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://ql.zhonguo5118.cn

Go:   // 单行；/* 多行 */
来源：https://md.zhonguo4118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://nd.zhonguo3118.cn

C#:   // 单行；/* 多行 */
来源：https://kv.zhonguo5118.cn

[A15] 空值判断与默认值
来源：https://ks.zhonguo8118.cn

Py:   value = data or "默认值"
来源：https://ms.zhonguo2118.cn

PHP:  $value = $data ?? "默认值";
来源：https://rc.zhonguo6118.cn

JS:   const value = data ?? "默认值";
来源：https://vj.zhonguo5118.cn

TS:   const value = data ?? "默认值";
来源：https://wk.zhonguo1118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://tt.zhonguo3118.cn

Go:   if data == "" { data = "默认值" }
来源：https://nk.zhonguo8118.cn

Ruby: value = data || "默认值"
来源：https://rw.zhonguo3118.cn

C#:   var value = data ?? "默认值";
来源：https://qc.zhonguo5118.cn

[A16] 真假值判断规则
来源：https://if.zhonguo3118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://tc.zhonguo7118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://hg.zhonguo7118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://qv.zhonguo1118.cn

TS:   if (!x) {}
来源：https://xe.zhonguo4118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://ww.zhonguo1118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://eq.zhonguo6118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://pz.zhonguo2118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://hr.zhonguo5118.cn

[A17] 位运算
来源：https://pf.zhonguo4118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ma.zhonguo2118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://ut.zhonguo6118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://gh.zhonguo3118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://lj.zhonguo5118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://tx.zhonguo8118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://ch.zhonguo2118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://et.zhonguo7118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://st.zhonguo1118.cn

[A18] 字符与 ASCII 码互转
来源：https://kp.zhonguo6118.cn

Py:   ord("A"); chr(65)
来源：https://ue.zhonguo7118.cn

PHP:  ord("A"); chr(65)
来源：https://gj.zhonguo5118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://kp.zhonguo3118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://jg.zhonguo6118.cn

Java: (int) 'A'; (char) 65
来源：https://aw.zhonguo2118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://ki.zhonguo6118.cn

Ruby: "A".ord; 65.chr
来源：https://ja.zhonguo4118.cn

C#:   (int)'A'; (char)65
来源：https://ey.zhonguo6118.cn

[A19] 交换两个变量
来源：https://rj.zhonguo4118.cn

Py:   a, b = b, a
来源：https://qo.zhonguo4118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://ej.zhonguo8118.cn

JS:   [a, b] = [b, a];
来源：https://zs.zhonguo8118.cn

TS:   [a, b] = [b, a];
来源：https://kl.zhonguo1118.cn

Java: int t = a; a = b; b = t;
来源：https://iq.zhonguo7118.cn

Go:   a, b = b, a
来源：https://ie.zhonguo4118.cn

Ruby: a, b = b, a
来源：https://ln.zhonguo5118.cn

C#:   (a, b) = (b, a);
来源：https://lb.zhonguo8118.cn

[A20] 读取标准输入
来源：https://dt.zhonguo1118.cn

Py:   name = input("请输入：")
来源：https://vj.zhonguo4118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://ql.zhonguo2118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://xl.zhonguo5118.cn

TS:   // Node.js：readline 模块
来源：https://fe.zhonguo5118.cn

Java: new Scanner(System.in).nextLine()
来源：https://ww.zhonguo5118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://dk.zhonguo1118.cn

Ruby: gets.chomp
来源：https://dq.zhonguo5118.cn

C#:   Console.ReadLine();
来源：https://xj.zhonguo8118.cn

[A21] 保留指定小数位输出
来源：https://vv.zhonguo3118.cn

Py:   f"{3.14159:.2f}"
来源：https://pt.zhonguo2118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://rj.zhonguo2118.cn

JS:   (3.14159).toFixed(2)
来源：https://sr.zhonguo2118.cn

TS:   (3.14159).toFixed(2)
来源：https://bl.zhonguo2118.cn

Java: String.format("%.2f", 3.14159)
来源：https://ta.zhonguo6118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://we.zhonguo3118.cn

Ruby: format("%.2f", 3.14159)
来源：https://un.zhonguo7118.cn

C#:   3.14159.ToString("F2")
来源：https://zo.zhonguo4118.cn

[A22] 获取字符串长度
来源：https://fq.zhonguo8118.cn

Py:   len(s)
来源：https://oc.zhonguo6118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://yi.zhonguo8118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://fe.zhonguo7118.cn

TS:   s.length
来源：https://by.zhonguo6118.cn

Java: s.length()
来源：https://lo.zhonguo5118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://dx.zhonguo1118.cn

Ruby: s.length
来源：https://ie.zhonguo6118.cn

C#:   s.Length
来源：https://my.zhonguo3118.cn

[A23] 大小写转换
来源：https://oj.zhonguo4118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://iq.zhonguo2118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://hf.zhonguo2118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://sv.zhonguo3118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://zo.zhonguo2118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://bj.zhonguo2118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://ds.zhonguo1118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://ot.zhonguo4118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://sx.zhonguo7118.cn

[A24] 去除首尾空白
来源：https://qa.zhonguo6118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://uh.zhonguo5118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://lm.zhonguo8118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://cz.zhonguo4118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://ka.zhonguo8118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://gi.zhonguo5118.cn

Go:   strings.TrimSpace(s)
来源：https://dm.zhonguo1118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://xi.zhonguo7118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://dq.zhonguo6118.cn

[A25] 字符串比较
来源：https://nw.zhonguo7118.cn

Py:   s1 == s2; s1 != s2
来源：https://go.zhonguo7118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://wd.zhonguo7118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://lk.zhonguo4118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://nt.zhonguo1118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://yk.zhonguo5118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://dy.zhonguo3118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://lg.zhonguo3118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://st.zhonguo6118.cn

[A26] 类型转换总览
来源：https://la.zhonguo3118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://ul.zhonguo5118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://mx.zhonguo7118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://dy.zhonguo2118.cn

TS:   Number() String() Boolean() x as number
来源：https://se.zhonguo3118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://lc.zhonguo1118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://qi.zhonguo3118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://lg.zhonguo4118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://lh.zhonguo5118.cn

================================================================================
来源：https://mp.zhonguo3118.cn

B. 流程控制
来源：https://lt.zhonguo2118.cn

================================================================================
来源：https://dz.zhonguo4118.cn

[B01] 条件判断 if / else
来源：https://gm.zhonguo6118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://tt.zhonguo8118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://ne.zhonguo8118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://hz.zhonguo3118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://fq.zhonguo7118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://bq.zhonguo4118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://jv.zhonguo2118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://ve.zhonguo8118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://ix.zhonguo5118.cn

[B02] 多分支 else if / elif
来源：https://xa.zhonguo5118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://gv.zhonguo7118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://no.zhonguo6118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ek.zhonguo6118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://wp.zhonguo6118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ep.zhonguo6118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://ei.zhonguo7118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://wj.zhonguo5118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://qv.zhonguo4118.cn

[B03] switch / match / case
来源：https://fq.zhonguo6118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://ir.zhonguo5118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://dr.zhonguo3118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://ue.zhonguo4118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://sl.zhonguo7118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://nv.zhonguo2118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://bi.zhonguo1118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://oy.zhonguo3118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://mh.zhonguo7118.cn

[B04] for 计数循环
来源：https://ku.zhonguo5118.cn

Py:   for i in range(10): print(i)
来源：https://he.zhonguo7118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://xs.zhonguo2118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://xo.zhonguo7118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://kk.zhonguo3118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://qr.zhonguo7118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://nw.zhonguo4118.cn

Ruby: 10.times { |i| puts i }
来源：https://hj.zhonguo8118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://sk.zhonguo3118.cn

[B05] 遍历数组 / 列表
来源：https://sx.zhonguo3118.cn

Py:   for item in arr: print(item)
来源：https://nl.zhonguo6118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://bq.zhonguo7118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://sc.zhonguo5118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://bj.zhonguo6118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://vm.zhonguo2118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://pu.zhonguo8118.cn

Ruby: arr.each { |item| puts item }
来源：https://sm.zhonguo8118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://re.zhonguo1118.cn

[B06] 遍历字典 / 对象
来源：https://no.zhonguo7118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://sf.zhonguo4118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://bu.zhonguo4118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://lh.zhonguo8118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://mg.zhonguo7118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://ql.zhonguo2118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://mm.zhonguo6118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://vw.zhonguo4118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://lq.zhonguo4118.cn

[B07] while 循环
来源：https://ag.zhonguo8118.cn

Py:   while i < 10: i += 1
来源：https://nk.zhonguo2118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://lg.zhonguo6118.cn

JS:   while (i < 10) { i++; }
来源：https://sp.zhonguo2118.cn

TS:   while (i < 10) { i++; }
来源：https://oc.zhonguo4118.cn

Java: while (i < 10) { i++; }
来源：https://sf.zhonguo1118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://ht.zhonguo4118.cn

Ruby: while i < 10; i += 1; end
来源：https://ua.zhonguo6118.cn

C#:   while (i < 10) { i++; }
来源：https://pu.zhonguo1118.cn

[B08] do-while（至少执行一次）
来源：https://xj.zhonguo4118.cn

Py:   # 无 do-while：用 while True + break
来源：https://tt.zhonguo7118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://kv.zhonguo2118.cn

JS:   do { i++; } while (i < 10);
来源：https://di.zhonguo5118.cn

TS:   do { i++; } while (i < 10);
来源：https://iq.zhonguo8118.cn

Java: do { i++; } while (i < 10);
来源：https://bj.zhonguo5118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://hn.zhonguo4118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://pv.zhonguo4118.cn

C#:   do { i++; } while (i < 10);
来源：https://sg.zhonguo2118.cn

[B09] break 与 continue
来源：https://ot.zhonguo8118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://zv.zhonguo7118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://ui.zhonguo5118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://le.zhonguo2118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://yc.zhonguo4118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://vj.zhonguo8118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://jn.zhonguo4118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://hr.zhonguo1118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ci.zhonguo3118.cn

[B10] 遍历同时拿索引
来源：https://sq.zhonguo2118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://lw.zhonguo5118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://hv.zhonguo7118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://kp.zhonguo4118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://qe.zhonguo3118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://dd.zhonguo8118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://ih.zhonguo1118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://gu.zhonguo5118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://ep.zhonguo7118.cn

[B11] 生成数字序列 / 区间
来源：https://pk.zhonguo7118.cn

Py:   list(range(0, 10, 2))
来源：https://vi.zhonguo6118.cn

PHP:  range(0, 10, 2);
来源：https://ra.zhonguo4118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://qm.zhonguo5118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://ye.zhonguo3118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://qv.zhonguo4118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://io.zhonguo7118.cn

Ruby: (0...10).step(2).to_a
来源：https://ru.zhonguo8118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://sr.zhonguo4118.cn

[B12] 跳出多层循环
来源：https://cg.zhonguo8118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://yt.zhonguo6118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://th.zhonguo7118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://vn.zhonguo2118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://ji.zhonguo7118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://cb.zhonguo6118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://sq.zhonguo8118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://ii.zhonguo1118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://il.zhonguo4118.cn

[B13] 判断是否为数字
来源：https://mi.zhonguo2118.cn

Py:   isinstance(x, (int, float))
来源：https://fz.zhonguo6118.cn

PHP:  is_numeric($x)
来源：https://xv.zhonguo4118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ue.zhonguo6118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ey.zhonguo7118.cn

Java: x instanceof Number
来源：https://zj.zhonguo2118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://oi.zhonguo3118.cn

Ruby: x.is_a?(Numeric)
来源：https://ns.zhonguo4118.cn

C#:   x is int or double or decimal
来源：https://jq.zhonguo6118.cn

[B14] 判断值是否在集合内
来源：https://gu.zhonguo7118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://tk.zhonguo2118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://dc.zhonguo7118.cn

JS:   [1, 2, 3].includes(x)
来源：https://fv.zhonguo3118.cn

TS:   [1, 2, 3].includes(x)
来源：https://rw.zhonguo7118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://ny.zhonguo1118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://bf.zhonguo1118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://sj.zhonguo5118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://cq.zhonguo1118.cn

[B15] 布尔运算与取反
来源：https://eb.zhonguo5118.cn

Py:   a and b or not c
来源：https://ht.zhonguo8118.cn

PHP:  $a && $b || !$c
来源：https://cy.zhonguo8118.cn

JS:   a && b || !c
来源：https://zc.zhonguo2118.cn

TS:   a && b || !c
来源：https://zf.zhonguo4118.cn

Java: a && b || !c
来源：https://nz.zhonguo8118.cn

Go:   a && b || !c
来源：https://vg.zhonguo5118.cn

Ruby: a && b || !c
来源：https://ui.zhonguo3118.cn

C#:   a && b || !c
来源：https://tv.zhonguo8118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://rf.zhonguo1118.cn

Py:   if not data: return
来源：https://jf.zhonguo8118.cn

PHP:  if (!$data) { return; }
来源：https://hi.zhonguo8118.cn

JS:   if (!data) return;
来源：https://zq.zhonguo8118.cn

TS:   if (!data) return;
来源：https://kg.zhonguo7118.cn

Java: if (data == null) return;
来源：https://bj.zhonguo5118.cn

Go:   if data == nil { return }
来源：https://np.zhonguo2118.cn

Ruby: return if data.nil?
来源：https://ul.zhonguo3118.cn

C#:   if (data == null) return;
来源：https://ns.zhonguo8118.cn

================================================================================
来源：https://ae.zhonguo5118.cn

C. 函数与作用域
来源：https://ap.zhonguo2118.cn

================================================================================
来源：https://ao.zhonguo2118.cn

[C01] 定义函数
来源：https://ww.zhonguo3118.cn

Py:   def add(a, b): return a + b
来源：https://ty.zhonguo4118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://jz.zhonguo7118.cn

JS:   function add(a, b) { return a + b; }
来源：https://tt.zhonguo1118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://ov.zhonguo1118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://hm.zhonguo4118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://nz.zhonguo7118.cn

Ruby: def add(a, b); a + b; end
来源：https://yx.zhonguo1118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://kq.zhonguo7118.cn

[C02] 默认参数
来源：https://aa.zhonguo3118.cn

Py:   def greet(name="World"): return name
来源：https://zi.zhonguo8118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://oc.zhonguo8118.cn

JS:   function greet(name = "World") { return name; }
来源：https://xy.zhonguo2118.cn


<!-- 参考信息 -->