代发 wailian999

[A14] 注释写法
来源：https://gz.zhonguo4118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://oy.zhonguo7118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://vh.zhonguo1118.cn

JS:   // 单行；/* 多行 */
来源：https://hu.zhonguo1118.cn

TS:   // 单行；/* 多行 */
来源：https://za.zhonguo4118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://pb.zhonguo6118.cn

Go:   // 单行；/* 多行 */
来源：https://cr.zhonguo8118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://yq.zhonguo4118.cn

C#:   // 单行；/* 多行 */
来源：https://kf.zhonguo2118.cn

[A15] 空值判断与默认值
来源：https://jj.zhonguo5118.cn

Py:   value = data or "默认值"
来源：https://um.zhonguo6118.cn

PHP:  $value = $data ?? "默认值";
来源：https://jy.zhonguo2118.cn

JS:   const value = data ?? "默认值";
来源：https://zi.zhonguo5118.cn

TS:   const value = data ?? "默认值";
来源：https://tc.zhonguo5118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://ka.zhonguo8118.cn

Go:   if data == "" { data = "默认值" }
来源：https://ya.zhonguo4118.cn

Ruby: value = data || "默认值"
来源：https://vd.zhonguo2118.cn

C#:   var value = data ?? "默认值";
来源：https://io.zhonguo8118.cn

[A16] 真假值判断规则
来源：https://rs.zhonguo4118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://hh.zhonguo4118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://uo.zhonguo1118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://zd.zhonguo1118.cn

TS:   if (!x) {}
来源：https://vn.zhonguo7118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://nq.zhonguo5118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://jw.zhonguo4118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://pm.zhonguo4118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://bc.zhonguo2118.cn

[A17] 位运算
来源：https://xt.zhonguo3118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://no.zhonguo8118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://pi.zhonguo1118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ng.zhonguo5118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://kt.zhonguo2118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://hp.zhonguo8118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://yv.zhonguo7118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://pd.zhonguo2118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ma.zhonguo6118.cn

[A18] 字符与 ASCII 码互转
来源：https://qm.zhonguo5118.cn

Py:   ord("A"); chr(65)
来源：https://zs.zhonguo8118.cn

PHP:  ord("A"); chr(65)
来源：https://fb.zhonguo1118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://eb.zhonguo7118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://qq.zhonguo1118.cn

Java: (int) 'A'; (char) 65
来源：https://gk.zhonguo5118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://in.zhonguo7118.cn

Ruby: "A".ord; 65.chr
来源：https://us.zhonguo5118.cn

C#:   (int)'A'; (char)65
来源：https://co.zhonguo6118.cn

[A19] 交换两个变量
来源：https://ek.zhonguo4118.cn

Py:   a, b = b, a
来源：https://wv.zhonguo1118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://as.zhonguo8118.cn

JS:   [a, b] = [b, a];
来源：https://hy.zhonguo3118.cn

TS:   [a, b] = [b, a];
来源：https://er.zhonguo4118.cn

Java: int t = a; a = b; b = t;
来源：https://mq.zhonguo5118.cn

Go:   a, b = b, a
来源：https://mz.zhonguo8118.cn

Ruby: a, b = b, a
来源：https://ho.zhonguo5118.cn

C#:   (a, b) = (b, a);
来源：https://an.zhonguo1118.cn

[A20] 读取标准输入
来源：https://pq.zhonguo3118.cn

Py:   name = input("请输入：")
来源：https://mt.zhonguo8118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://vc.zhonguo5118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://vf.zhonguo4118.cn

TS:   // Node.js：readline 模块
来源：https://ep.zhonguo4118.cn

Java: new Scanner(System.in).nextLine()
来源：https://os.zhonguo7118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://ce.zhonguo2118.cn

Ruby: gets.chomp
来源：https://fp.zhonguo4118.cn

C#:   Console.ReadLine();
来源：https://mv.zhonguo1118.cn

[A21] 保留指定小数位输出
来源：https://mx.zhonguo6118.cn

Py:   f"{3.14159:.2f}"
来源：https://om.zhonguo3118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://zh.zhonguo1118.cn

JS:   (3.14159).toFixed(2)
来源：https://vo.zhonguo2118.cn

TS:   (3.14159).toFixed(2)
来源：https://dt.zhonguo1118.cn

Java: String.format("%.2f", 3.14159)
来源：https://ii.zhonguo3118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://cm.zhonguo5118.cn

Ruby: format("%.2f", 3.14159)
来源：https://cv.zhonguo4118.cn

C#:   3.14159.ToString("F2")
来源：https://yi.zhonguo3118.cn

[A22] 获取字符串长度
来源：https://bg.zhonguo8118.cn

Py:   len(s)
来源：https://ey.zhonguo3118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://mf.zhonguo4118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://rf.zhonguo3118.cn

TS:   s.length
来源：https://tj.zhonguo8118.cn

Java: s.length()
来源：https://dy.zhonguo6118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://pk.zhonguo7118.cn

Ruby: s.length
来源：https://hi.zhonguo2118.cn

C#:   s.Length
来源：https://cm.zhonguo2118.cn

[A23] 大小写转换
来源：https://qc.zhonguo6118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://ae.zhonguo8118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://hh.zhonguo8118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://kz.zhonguo1118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://di.zhonguo3118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://ft.zhonguo1118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://ja.zhonguo3118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://vu.zhonguo2118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://rr.zhonguo3118.cn

[A24] 去除首尾空白
来源：https://xm.zhonguo1118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://kn.zhonguo8118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://ua.zhonguo1118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://qr.zhonguo3118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://rs.zhonguo3118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://vz.zhonguo6118.cn

Go:   strings.TrimSpace(s)
来源：https://wt.zhonguo8118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://my.zhonguo2118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://pd.zhonguo6118.cn

[A25] 字符串比较
来源：https://js.zhonguo7118.cn

Py:   s1 == s2; s1 != s2
来源：https://yj.zhonguo4118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://fb.zhonguo4118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://kb.zhonguo7118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://kb.zhonguo6118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://od.zhonguo8118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://ih.zhonguo6118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://ks.zhonguo5118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://wi.zhonguo1118.cn

[A26] 类型转换总览
来源：https://mb.zhonguo4118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://xf.zhonguo1118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://ck.zhonguo4118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://eb.zhonguo3118.cn

TS:   Number() String() Boolean() x as number
来源：https://ub.zhonguo6118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://db.zhonguo3118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://bx.zhonguo1118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://cq.zhonguo7118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://cg.zhonguo6118.cn

================================================================================
来源：https://ik.zhonguo6118.cn

B. 流程控制
来源：https://sz.zhonguo5118.cn

================================================================================
来源：https://rn.zhonguo7118.cn

[B01] 条件判断 if / else
来源：https://pr.zhonguo6118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://ar.zhonguo6118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://tc.zhonguo4118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://nf.zhonguo1118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://mm.zhonguo4118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://to.zhonguo3118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://ed.zhonguo1118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://pa.zhonguo8118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://rf.zhonguo4118.cn

[B02] 多分支 else if / elif
来源：https://rn.zhonguo5118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://af.zhonguo6118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://vo.zhonguo1118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ln.zhonguo6118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://de.zhonguo3118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://la.zhonguo7118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://qe.zhonguo7118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://va.zhonguo5118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ch.zhonguo3118.cn

[B03] switch / match / case
来源：https://ag.zhonguo6118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://bw.zhonguo5118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://tj.zhonguo6118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://wg.zhonguo1118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://ot.zhonguo4118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://fm.zhonguo4118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://zw.zhonguo1118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://nh.zhonguo1118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://yz.zhonguo4118.cn

[B04] for 计数循环
来源：https://pk.zhonguo5118.cn

Py:   for i in range(10): print(i)
来源：https://cs.zhonguo1118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://al.zhonguo3118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://cb.zhonguo2118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://qo.zhonguo2118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://ie.zhonguo3118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://zy.zhonguo5118.cn

Ruby: 10.times { |i| puts i }
来源：https://xy.zhonguo3118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://xa.zhonguo1118.cn

[B05] 遍历数组 / 列表
来源：https://yl.zhonguo1118.cn

Py:   for item in arr: print(item)
来源：https://rl.zhonguo6118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://bq.zhonguo6118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://re.zhonguo1118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://ad.zhonguo3118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://fm.zhonguo8118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://qw.zhonguo6118.cn

Ruby: arr.each { |item| puts item }
来源：https://wm.zhonguo1118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://cg.zhonguo2118.cn

[B06] 遍历字典 / 对象
来源：https://am.zhonguo3118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://gk.zhonguo3118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://vp.zhonguo3118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://pl.zhonguo1118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://wl.zhonguo7118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://vf.zhonguo3118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://ea.zhonguo3118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://qd.zhonguo3118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://fa.zhonguo8118.cn

[B07] while 循环
来源：https://zc.zhonguo2118.cn

Py:   while i < 10: i += 1
来源：https://sy.zhonguo7118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://ua.zhonguo7118.cn

JS:   while (i < 10) { i++; }
来源：https://jo.zhonguo4118.cn

TS:   while (i < 10) { i++; }
来源：https://kt.zhonguo4118.cn

Java: while (i < 10) { i++; }
来源：https://as.zhonguo7118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://mo.zhonguo4118.cn

Ruby: while i < 10; i += 1; end
来源：https://dt.zhonguo6118.cn

C#:   while (i < 10) { i++; }
来源：https://gu.zhonguo8118.cn

[B08] do-while（至少执行一次）
来源：https://sv.zhonguo3118.cn

Py:   # 无 do-while：用 while True + break
来源：https://fj.zhonguo1118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://ye.zhonguo5118.cn

JS:   do { i++; } while (i < 10);
来源：https://mi.zhonguo4118.cn

TS:   do { i++; } while (i < 10);
来源：https://gp.zhonguo4118.cn

Java: do { i++; } while (i < 10);
来源：https://au.zhonguo4118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://pn.zhonguo1118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://lp.zhonguo6118.cn

C#:   do { i++; } while (i < 10);
来源：https://tc.zhonguo1118.cn

[B09] break 与 continue
来源：https://ye.zhonguo3118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://kl.zhonguo1118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://mf.zhonguo8118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://vs.zhonguo5118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://rn.zhonguo4118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://qy.zhonguo8118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://wr.zhonguo2118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://in.zhonguo3118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://re.zhonguo3118.cn

[B10] 遍历同时拿索引
来源：https://bc.zhonguo3118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://bi.zhonguo8118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://ry.zhonguo7118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://wu.zhonguo2118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://jm.zhonguo7118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://hn.zhonguo1118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://ym.zhonguo4118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://sb.zhonguo3118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://og.zhonguo2118.cn

[B11] 生成数字序列 / 区间
来源：https://ds.zhonguo7118.cn

Py:   list(range(0, 10, 2))
来源：https://co.zhonguo1118.cn

PHP:  range(0, 10, 2);
来源：https://lr.zhonguo1118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://ks.zhonguo2118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://jd.zhonguo1118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://af.zhonguo7118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://yw.zhonguo8118.cn

Ruby: (0...10).step(2).to_a
来源：https://kb.zhonguo4118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://ks.zhonguo2118.cn

[B12] 跳出多层循环
来源：https://rh.zhonguo7118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://ky.zhonguo4118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://tp.zhonguo3118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://gn.zhonguo6118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://xb.zhonguo3118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://na.zhonguo1118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://mz.zhonguo7118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://da.zhonguo8118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://uv.zhonguo1118.cn

[B13] 判断是否为数字
来源：https://qp.zhonguo3118.cn

Py:   isinstance(x, (int, float))
来源：https://st.zhonguo2118.cn

PHP:  is_numeric($x)
来源：https://rm.zhonguo2118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://gv.zhonguo3118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ue.zhonguo8118.cn

Java: x instanceof Number
来源：https://tl.zhonguo4118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://ef.zhonguo3118.cn

Ruby: x.is_a?(Numeric)
来源：https://uq.zhonguo2118.cn

C#:   x is int or double or decimal
来源：https://go.zhonguo6118.cn

[B14] 判断值是否在集合内
来源：https://yh.zhonguo3118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://nx.zhonguo4118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://xc.zhonguo4118.cn

JS:   [1, 2, 3].includes(x)
来源：https://nw.zhonguo7118.cn

TS:   [1, 2, 3].includes(x)
来源：https://vg.zhonguo4118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://yw.zhonguo8118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://sg.zhonguo4118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://dz.zhonguo7118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://ei.zhonguo5118.cn

[B15] 布尔运算与取反
来源：https://sq.zhonguo3118.cn

Py:   a and b or not c
来源：https://zo.zhonguo7118.cn

PHP:  $a && $b || !$c
来源：https://ku.zhonguo5118.cn

JS:   a && b || !c
来源：https://zn.zhonguo5118.cn

TS:   a && b || !c
来源：https://zu.zhonguo5118.cn

Java: a && b || !c
来源：https://uo.zhonguo6118.cn

Go:   a && b || !c
来源：https://so.zhonguo3118.cn

Ruby: a && b || !c
来源：https://tc.zhonguo2118.cn

C#:   a && b || !c
来源：https://ym.zhonguo5118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://aa.zhonguo2118.cn

Py:   if not data: return
来源：https://wo.zhonguo2118.cn

PHP:  if (!$data) { return; }
来源：https://uu.zhonguo6118.cn

JS:   if (!data) return;
来源：https://vm.zhonguo2118.cn

TS:   if (!data) return;
来源：https://jc.zhonguo2118.cn

Java: if (data == null) return;
来源：https://si.zhonguo2118.cn

Go:   if data == nil { return }
来源：https://en.zhonguo8118.cn

Ruby: return if data.nil?
来源：https://bf.zhonguo4118.cn

C#:   if (data == null) return;
来源：https://hr.zhonguo4118.cn

================================================================================
来源：https://gh.zhonguo5118.cn

C. 函数与作用域
来源：https://qb.zhonguo4118.cn

================================================================================
来源：https://wb.zhonguo8118.cn

[C01] 定义函数
来源：https://vb.zhonguo4118.cn

Py:   def add(a, b): return a + b
来源：https://xd.zhonguo5118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://gv.zhonguo1118.cn

JS:   function add(a, b) { return a + b; }
来源：https://hm.zhonguo3118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://la.zhonguo6118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://xt.zhonguo7118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://eu.zhonguo4118.cn

Ruby: def add(a, b); a + b; end
来源：https://of.zhonguo8118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://ju.zhonguo3118.cn

[C02] 默认参数
来源：https://ch.zhonguo6118.cn

Py:   def greet(name="World"): return name
来源：https://pj.zhonguo6118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://yc.zhonguo8118.cn

JS:   function greet(name = "World") { return name; }
来源：https://qv.zhonguo3118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://ic.zhonguo2118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://hs.zhonguo1118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://mj.zhonguo2118.cn

Ruby: def greet(name = "World") = name
来源：https://nr.zhonguo5118.cn

C#:   string Greet(string name = "World") => name;
来源：https://qe.zhonguo3118.cn

[C03] 可变参数
来源：https://rs.zhonguo8118.cn

Py:   def total(*args): return sum(args)
来源：https://oa.zhonguo5118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://jk.zhonguo6118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://wy.zhonguo7118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://xf.zhonguo6118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://oa.zhonguo3118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://su.zhonguo8118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://cf.zhonguo1118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://cg.zhonguo3118.cn

[C04] 命名参数 / 关键字参数
来源：https://bm.zhonguo8118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://ts.zhonguo1118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://re.zhonguo6118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://tb.zhonguo2118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://gq.zhonguo1118.cn

Java: // 无：用 Builder 模式或 record
来源：https://za.zhonguo8118.cn


<!-- 参考信息 -->