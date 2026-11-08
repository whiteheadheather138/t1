代发 wailian999

Java: "第一行\n第二行"
来源：https://si.zhonguo6118.cn

Go:   "第一行\n第二行"
来源：https://uc.zhonguo1118.cn

Ruby: "第一行\n第二行"
来源：https://oy.zhonguo6118.cn

C#:   "第一行\n第二行"
来源：https://pk.zhonguo8118.cn

[A14] 注释写法
来源：https://sc.zhonguo4118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://ht.zhonguo4118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://ou.zhonguo7118.cn

JS:   // 单行；/* 多行 */
来源：https://ks.zhonguo6118.cn

TS:   // 单行；/* 多行 */
来源：https://rq.zhonguo1118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://df.zhonguo6118.cn

Go:   // 单行；/* 多行 */
来源：https://re.zhonguo2118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://nk.zhonguo6118.cn

C#:   // 单行；/* 多行 */
来源：https://iy.zhonguo3118.cn

[A15] 空值判断与默认值
来源：https://wt.zhonguo1118.cn

Py:   value = data or "默认值"
来源：https://yo.zhonguo3118.cn

PHP:  $value = $data ?? "默认值";
来源：https://nq.zhonguo7118.cn

JS:   const value = data ?? "默认值";
来源：https://km.zhonguo6118.cn

TS:   const value = data ?? "默认值";
来源：https://bs.zhonguo4118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://en.zhonguo3118.cn

Go:   if data == "" { data = "默认值" }
来源：https://tf.zhonguo2118.cn

Ruby: value = data || "默认值"
来源：https://bk.zhonguo2118.cn

C#:   var value = data ?? "默认值";
来源：https://xv.zhonguo7118.cn

[A16] 真假值判断规则
来源：https://dj.zhonguo2118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://zp.zhonguo6118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://hv.zhonguo4118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://hh.zhonguo6118.cn

TS:   if (!x) {}
来源：https://ki.zhonguo4118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://xy.zhonguo3118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://jc.zhonguo4118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://sb.zhonguo5118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://ja.zhonguo4118.cn

[A17] 位运算
来源：https://yf.zhonguo8118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://jd.zhonguo7118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://az.zhonguo6118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://hc.zhonguo1118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://fs.zhonguo4118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ox.zhonguo3118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://gt.zhonguo4118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://vi.zhonguo4118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://qo.zhonguo7118.cn

[A18] 字符与 ASCII 码互转
来源：https://ce.zhonguo4118.cn

Py:   ord("A"); chr(65)
来源：https://rt.zhonguo1118.cn

PHP:  ord("A"); chr(65)
来源：https://bt.zhonguo5118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://bq.zhonguo3118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://bd.zhonguo7118.cn

Java: (int) 'A'; (char) 65
来源：https://gg.zhonguo8118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://zu.zhonguo2118.cn

Ruby: "A".ord; 65.chr
来源：https://to.zhonguo2118.cn

C#:   (int)'A'; (char)65
来源：https://hc.zhonguo2118.cn

[A19] 交换两个变量
来源：https://cz.zhonguo4118.cn

Py:   a, b = b, a
来源：https://oy.zhonguo6118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://vr.zhonguo6118.cn

JS:   [a, b] = [b, a];
来源：https://ql.zhonguo2118.cn

TS:   [a, b] = [b, a];
来源：https://ez.zhonguo2118.cn

Java: int t = a; a = b; b = t;
来源：https://iw.zhonguo6118.cn

Go:   a, b = b, a
来源：https://uy.zhonguo3118.cn

Ruby: a, b = b, a
来源：https://pg.zhonguo8118.cn

C#:   (a, b) = (b, a);
来源：https://eq.zhonguo8118.cn

[A20] 读取标准输入
来源：https://cx.zhonguo5118.cn

Py:   name = input("请输入：")
来源：https://cc.zhonguo5118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://br.zhonguo7118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://rt.zhonguo1118.cn

TS:   // Node.js：readline 模块
来源：https://cy.zhonguo7118.cn

Java: new Scanner(System.in).nextLine()
来源：https://gp.zhonguo8118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://rf.zhonguo1118.cn

Ruby: gets.chomp
来源：https://ot.zhonguo4118.cn

C#:   Console.ReadLine();
来源：https://fk.zhonguo7118.cn

[A21] 保留指定小数位输出
来源：https://xg.zhonguo4118.cn

Py:   f"{3.14159:.2f}"
来源：https://fl.zhonguo7118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://nv.zhonguo6118.cn

JS:   (3.14159).toFixed(2)
来源：https://wi.zhonguo3118.cn

TS:   (3.14159).toFixed(2)
来源：https://sl.zhonguo7118.cn

Java: String.format("%.2f", 3.14159)
来源：https://uz.zhonguo7118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://eo.zhonguo5118.cn

Ruby: format("%.2f", 3.14159)
来源：https://td.zhonguo4118.cn

C#:   3.14159.ToString("F2")
来源：https://at.zhonguo4118.cn

[A22] 获取字符串长度
来源：https://uf.zhonguo8118.cn

Py:   len(s)
来源：https://ka.zhonguo3118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://ss.zhonguo4118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://bt.zhonguo2118.cn

TS:   s.length
来源：https://ui.zhonguo3118.cn

Java: s.length()
来源：https://xe.zhonguo5118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://hm.zhonguo4118.cn

Ruby: s.length
来源：https://zy.zhonguo7118.cn

C#:   s.Length
来源：https://iv.zhonguo7118.cn

[A23] 大小写转换
来源：https://ae.zhonguo4118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://rd.zhonguo5118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://tf.zhonguo6118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://kw.zhonguo6118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://ip.zhonguo2118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://pa.zhonguo8118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://cs.zhonguo2118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://il.zhonguo2118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://aj.zhonguo8118.cn

[A24] 去除首尾空白
来源：https://xs.zhonguo1118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://tq.zhonguo2118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://ze.zhonguo8118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://kw.zhonguo4118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://kq.zhonguo2118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://df.zhonguo8118.cn

Go:   strings.TrimSpace(s)
来源：https://ao.zhonguo3118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://yy.zhonguo2118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://dt.zhonguo7118.cn

[A25] 字符串比较
来源：https://uk.zhonguo4118.cn

Py:   s1 == s2; s1 != s2
来源：https://bp.zhonguo8118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://sl.zhonguo8118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://eb.zhonguo5118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://ez.zhonguo6118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://ar.zhonguo4118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://px.zhonguo1118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://nc.zhonguo1118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://mx.zhonguo5118.cn

[A26] 类型转换总览
来源：https://al.zhonguo6118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://qg.zhonguo3118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://oy.zhonguo1118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://mr.zhonguo8118.cn

TS:   Number() String() Boolean() x as number
来源：https://vu.zhonguo5118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://se.zhonguo5118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://lk.zhonguo5118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://ag.zhonguo3118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://qh.zhonguo3118.cn

================================================================================
来源：https://jq.zhonguo4118.cn

B. 流程控制
来源：https://ff.zhonguo2118.cn

================================================================================
来源：https://bl.zhonguo8118.cn

[B01] 条件判断 if / else
来源：https://pi.zhonguo8118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://aw.zhonguo4118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://pd.zhonguo1118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://cp.zhonguo8118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://dj.zhonguo1118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://vm.zhonguo2118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://dl.zhonguo2118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://qt.zhonguo6118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://sf.zhonguo8118.cn

[B02] 多分支 else if / elif
来源：https://my.zhonguo8118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://ar.zhonguo5118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://us.zhonguo6118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://pu.zhonguo8118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://uw.zhonguo3118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ob.zhonguo4118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://nn.zhonguo2118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://ns.zhonguo6118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://rr.zhonguo6118.cn

[B03] switch / match / case
来源：https://kq.zhonguo2118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://dz.zhonguo1118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://zf.zhonguo8118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://kg.zhonguo7118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://vi.zhonguo6118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://vn.zhonguo6118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://ld.zhonguo5118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://me.zhonguo2118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://ct.zhonguo7118.cn

[B04] for 计数循环
来源：https://lu.zhonguo3118.cn

Py:   for i in range(10): print(i)
来源：https://gr.zhonguo2118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://ux.zhonguo5118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://me.zhonguo4118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://yy.zhonguo5118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://tk.zhonguo2118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://ez.zhonguo5118.cn

Ruby: 10.times { |i| puts i }
来源：https://ur.zhonguo2118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://je.zhonguo7118.cn

[B05] 遍历数组 / 列表
来源：https://nj.zhonguo1118.cn

Py:   for item in arr: print(item)
来源：https://xh.zhonguo7118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://rc.zhonguo7118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://ue.zhonguo6118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://df.zhonguo1118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://xq.zhonguo5118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://vf.zhonguo4118.cn

Ruby: arr.each { |item| puts item }
来源：https://gc.zhonguo1118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://dz.zhonguo8118.cn

[B06] 遍历字典 / 对象
来源：https://su.zhonguo5118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://az.zhonguo3118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://zt.zhonguo1118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://dx.zhonguo3118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://hg.zhonguo4118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://ht.zhonguo1118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://iq.zhonguo6118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://vv.zhonguo3118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://ug.zhonguo1118.cn

[B07] while 循环
来源：https://bt.zhonguo2118.cn

Py:   while i < 10: i += 1
来源：https://ks.zhonguo1118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://du.zhonguo8118.cn

JS:   while (i < 10) { i++; }
来源：https://fc.zhonguo7118.cn

TS:   while (i < 10) { i++; }
来源：https://qk.zhonguo1118.cn

Java: while (i < 10) { i++; }
来源：https://xk.zhonguo6118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://dr.zhonguo8118.cn

Ruby: while i < 10; i += 1; end
来源：https://eo.zhonguo8118.cn

C#:   while (i < 10) { i++; }
来源：https://zm.zhonguo4118.cn

[B08] do-while（至少执行一次）
来源：https://aj.zhonguo2118.cn

Py:   # 无 do-while：用 while True + break
来源：https://ct.zhonguo6118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://vo.zhonguo8118.cn

JS:   do { i++; } while (i < 10);
来源：https://wn.zhonguo3118.cn

TS:   do { i++; } while (i < 10);
来源：https://cr.zhonguo8118.cn

Java: do { i++; } while (i < 10);
来源：https://fe.zhonguo6118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://ep.zhonguo2118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://le.zhonguo8118.cn

C#:   do { i++; } while (i < 10);
来源：https://ks.zhonguo6118.cn

[B09] break 与 continue
来源：https://uv.zhonguo6118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://al.zhonguo6118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://hp.zhonguo7118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ua.zhonguo2118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://lj.zhonguo4118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://zl.zhonguo3118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://vn.zhonguo1118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://lg.zhonguo7118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://uo.zhonguo7118.cn

[B10] 遍历同时拿索引
来源：https://eu.zhonguo6118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://qm.zhonguo4118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://ga.zhonguo5118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://ux.zhonguo5118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://hs.zhonguo8118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://vi.zhonguo4118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://fe.zhonguo3118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://dn.zhonguo3118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://lv.zhonguo3118.cn

[B11] 生成数字序列 / 区间
来源：https://lo.zhonguo4118.cn

Py:   list(range(0, 10, 2))
来源：https://zo.zhonguo7118.cn

PHP:  range(0, 10, 2);
来源：https://ue.zhonguo5118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://aa.zhonguo3118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://fp.zhonguo1118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://oa.zhonguo2118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://xe.zhonguo4118.cn

Ruby: (0...10).step(2).to_a
来源：https://fm.zhonguo1118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://du.zhonguo8118.cn

[B12] 跳出多层循环
来源：https://sb.zhonguo3118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://lt.zhonguo5118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://ck.zhonguo1118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://ro.zhonguo6118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://zt.zhonguo4118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://on.zhonguo1118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://hm.zhonguo4118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://ux.zhonguo1118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://pn.zhonguo7118.cn

[B13] 判断是否为数字
来源：https://wx.zhonguo2118.cn

Py:   isinstance(x, (int, float))
来源：https://eg.zhonguo3118.cn

PHP:  is_numeric($x)
来源：https://gf.zhonguo3118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ec.zhonguo6118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://zr.zhonguo1118.cn

Java: x instanceof Number
来源：https://hv.zhonguo1118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://wz.zhonguo4118.cn

Ruby: x.is_a?(Numeric)
来源：https://mn.zhonguo1118.cn

C#:   x is int or double or decimal
来源：https://by.zhonguo6118.cn

[B14] 判断值是否在集合内
来源：https://te.zhonguo6118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://dd.zhonguo7118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://go.zhonguo2118.cn

JS:   [1, 2, 3].includes(x)
来源：https://fk.zhonguo6118.cn

TS:   [1, 2, 3].includes(x)
来源：https://fr.zhonguo6118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://sr.zhonguo8118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://nv.zhonguo7118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://wc.zhonguo4118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://an.zhonguo3118.cn

[B15] 布尔运算与取反
来源：https://kw.zhonguo5118.cn

Py:   a and b or not c
来源：https://ue.zhonguo4118.cn

PHP:  $a && $b || !$c
来源：https://zc.zhonguo6118.cn

JS:   a && b || !c
来源：https://rl.zhonguo2118.cn

TS:   a && b || !c
来源：https://bg.zhonguo3118.cn

Java: a && b || !c
来源：https://xi.zhonguo3118.cn

Go:   a && b || !c
来源：https://fu.zhonguo8118.cn

Ruby: a && b || !c
来源：https://hn.zhonguo2118.cn

C#:   a && b || !c
来源：https://sp.zhonguo1118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://rd.zhonguo2118.cn

Py:   if not data: return
来源：https://co.zhonguo4118.cn

PHP:  if (!$data) { return; }
来源：https://tl.zhonguo4118.cn

JS:   if (!data) return;
来源：https://il.zhonguo3118.cn

TS:   if (!data) return;
来源：https://qg.zhonguo4118.cn

Java: if (data == null) return;
来源：https://cy.zhonguo2118.cn

Go:   if data == nil { return }
来源：https://vl.zhonguo4118.cn

Ruby: return if data.nil?
来源：https://mz.zhonguo8118.cn

C#:   if (data == null) return;
来源：https://eg.zhonguo8118.cn

================================================================================
来源：https://bo.zhonguo1118.cn

C. 函数与作用域
来源：https://qd.zhonguo5118.cn

================================================================================
来源：https://um.zhonguo1118.cn

[C01] 定义函数
来源：https://eb.zhonguo4118.cn

Py:   def add(a, b): return a + b
来源：https://hr.zhonguo6118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://ss.zhonguo7118.cn

JS:   function add(a, b) { return a + b; }
来源：https://oc.zhonguo8118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://xn.zhonguo6118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://ej.zhonguo3118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://gb.zhonguo1118.cn

Ruby: def add(a, b); a + b; end
来源：https://fk.zhonguo2118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://wh.zhonguo3118.cn

[C02] 默认参数
来源：https://tr.zhonguo8118.cn

Py:   def greet(name="World"): return name
来源：https://zn.zhonguo3118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://dz.zhonguo3118.cn

JS:   function greet(name = "World") { return name; }
来源：https://un.zhonguo6118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://ls.zhonguo6118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://po.zhonguo2118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://km.zhonguo3118.cn

Ruby: def greet(name = "World") = name
来源：https://ed.zhonguo8118.cn

C#:   string Greet(string name = "World") => name;
来源：https://sn.zhonguo1118.cn

[C03] 可变参数
来源：https://xe.zhonguo2118.cn

Py:   def total(*args): return sum(args)
来源：https://iv.zhonguo3118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://ky.zhonguo4118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://dc.zhonguo3118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://cr.zhonguo2118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://sf.zhonguo1118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://bu.zhonguo6118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://bz.zhonguo7118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://qp.zhonguo1118.cn

[C04] 命名参数 / 关键字参数
来源：https://mm.zhonguo5118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://ta.zhonguo7118.cn


<!-- 参考信息 -->