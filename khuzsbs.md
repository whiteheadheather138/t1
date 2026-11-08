代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：https://yn.zhonguo2118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://sw.zhonguo2118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://jx.zhonguo4118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://ks.zhonguo3118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://dk.zhonguo4118.cn

[A07] 数字转字符串
来源：https://lg.zhonguo3118.cn

Py:   str(42)
来源：https://gw.zhonguo6118.cn

PHP:  (string) 42; strval(42)
来源：https://xk.zhonguo6118.cn

JS:   String(42); (42).toString()
来源：https://yb.zhonguo8118.cn

TS:   String(42)
来源：https://uv.zhonguo5118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://hb.zhonguo3118.cn

Go:   strconv.Itoa(42)
来源：https://li.zhonguo3118.cn

Ruby: 42.to_s
来源：https://ce.zhonguo1118.cn

C#:   42.ToString()
来源：https://xd.zhonguo2118.cn

[A08] 取整与四舍五入
来源：https://aa.zhonguo6118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://iw.zhonguo8118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://xd.zhonguo1118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://fc.zhonguo4118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://pg.zhonguo6118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://mr.zhonguo7118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://vf.zhonguo3118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://df.zhonguo5118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://kd.zhonguo6118.cn

[A09] 绝对值与最大最小值
来源：https://ja.zhonguo6118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://uj.zhonguo7118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://jj.zhonguo5118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://pe.zhonguo5118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://qv.zhonguo8118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://ka.zhonguo8118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://my.zhonguo8118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://bn.zhonguo4118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://ch.zhonguo1118.cn

[A10] 生成随机数
来源：https://pr.zhonguo7118.cn

Py:   import random; random.randint(1, 100)
来源：https://lm.zhonguo4118.cn

PHP:  random_int(1, 100);
来源：https://vg.zhonguo4118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://cv.zhonguo8118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://of.zhonguo8118.cn

Java: new Random().nextInt(100) + 1
来源：https://iz.zhonguo8118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://gv.zhonguo5118.cn

Ruby: rand(1..100)
来源：https://pk.zhonguo8118.cn

C#:   new Random().Next(1, 101)
来源：https://mg.zhonguo6118.cn

[A11] 条件表达式（三元）
来源：https://by.zhonguo3118.cn

Py:   "yes" if x > 0 else "no"
来源：https://du.zhonguo8118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://bw.zhonguo3118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://il.zhonguo2118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://pw.zhonguo8118.cn

Java: x > 0 ? "yes" : "no"
来源：https://vf.zhonguo5118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://kw.zhonguo7118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://oe.zhonguo8118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://zw.zhonguo1118.cn

[A12] 字符串插值 / 格式化
来源：https://fb.zhonguo3118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://oi.zhonguo4118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://hp.zhonguo6118.cn

JS:   `Hello, ${name}!`
来源：https://vh.zhonguo5118.cn

TS:   `Hello, ${name}!`
来源：https://xs.zhonguo3118.cn

Java: "Hello, %s!".formatted(name)
来源：https://af.zhonguo5118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://xc.zhonguo5118.cn

Ruby: "Hello, #{name}!"
来源：https://dc.zhonguo7118.cn

C#:   $"Hello, {name}!"
来源：https://qu.zhonguo7118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://dc.zhonguo4118.cn

Py:   "第一行\n第二行"
来源：https://vq.zhonguo5118.cn

PHP:  "第一行\n第二行"
来源：https://zs.zhonguo2118.cn

JS:   "第一行\n第二行"
来源：https://yb.zhonguo5118.cn

TS:   "第一行\n第二行"
来源：https://ej.zhonguo8118.cn

Java: "第一行\n第二行"
来源：https://pe.zhonguo7118.cn

Go:   "第一行\n第二行"
来源：https://ys.zhonguo2118.cn

Ruby: "第一行\n第二行"
来源：https://nz.zhonguo5118.cn

C#:   "第一行\n第二行"
来源：https://uj.zhonguo7118.cn

[A14] 注释写法
来源：https://vp.zhonguo1118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://gk.zhonguo5118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://ae.zhonguo1118.cn

JS:   // 单行；/* 多行 */
来源：https://eo.zhonguo5118.cn

TS:   // 单行；/* 多行 */
来源：https://fv.zhonguo1118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://pz.zhonguo6118.cn

Go:   // 单行；/* 多行 */
来源：https://qc.zhonguo2118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://qh.zhonguo3118.cn

C#:   // 单行；/* 多行 */
来源：https://oz.zhonguo3118.cn

[A15] 空值判断与默认值
来源：https://im.zhonguo2118.cn

Py:   value = data or "默认值"
来源：https://qs.zhonguo8118.cn

PHP:  $value = $data ?? "默认值";
来源：https://np.zhonguo1118.cn

JS:   const value = data ?? "默认值";
来源：https://mo.zhonguo7118.cn

TS:   const value = data ?? "默认值";
来源：https://mc.zhonguo5118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://ki.zhonguo5118.cn

Go:   if data == "" { data = "默认值" }
来源：https://xr.zhonguo2118.cn

Ruby: value = data || "默认值"
来源：https://hq.zhonguo7118.cn

C#:   var value = data ?? "默认值";
来源：https://in.zhonguo6118.cn

[A16] 真假值判断规则
来源：https://eg.zhonguo5118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://vy.zhonguo4118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://xu.zhonguo3118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://uz.zhonguo6118.cn

TS:   if (!x) {}
来源：https://af.zhonguo4118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://rw.zhonguo1118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://my.zhonguo6118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://or.zhonguo1118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://zr.zhonguo6118.cn

[A17] 位运算
来源：https://sf.zhonguo6118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ue.zhonguo5118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://ff.zhonguo8118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://wv.zhonguo1118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://fr.zhonguo8118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://hi.zhonguo3118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://qx.zhonguo2118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ss.zhonguo7118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://wk.zhonguo3118.cn

[A18] 字符与 ASCII 码互转
来源：https://ps.zhonguo6118.cn

Py:   ord("A"); chr(65)
来源：https://mr.zhonguo4118.cn

PHP:  ord("A"); chr(65)
来源：https://va.zhonguo3118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://dy.zhonguo3118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://vp.zhonguo2118.cn

Java: (int) 'A'; (char) 65
来源：https://cl.zhonguo2118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://tu.zhonguo1118.cn

Ruby: "A".ord; 65.chr
来源：https://ui.zhonguo5118.cn

C#:   (int)'A'; (char)65
来源：https://nx.zhonguo7118.cn

[A19] 交换两个变量
来源：https://sz.zhonguo4118.cn

Py:   a, b = b, a
来源：https://gr.zhonguo7118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://fi.zhonguo6118.cn

JS:   [a, b] = [b, a];
来源：https://kt.zhonguo3118.cn

TS:   [a, b] = [b, a];
来源：https://iw.zhonguo1118.cn

Java: int t = a; a = b; b = t;
来源：https://xk.zhonguo2118.cn

Go:   a, b = b, a
来源：https://uu.zhonguo1118.cn

Ruby: a, b = b, a
来源：https://rf.zhonguo2118.cn

C#:   (a, b) = (b, a);
来源：https://an.zhonguo7118.cn

[A20] 读取标准输入
来源：https://vs.zhonguo5118.cn

Py:   name = input("请输入：")
来源：https://jr.zhonguo5118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://ee.zhonguo7118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://mh.zhonguo3118.cn

TS:   // Node.js：readline 模块
来源：https://pe.zhonguo5118.cn

Java: new Scanner(System.in).nextLine()
来源：https://aa.zhonguo1118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://ir.zhonguo8118.cn

Ruby: gets.chomp
来源：https://sx.zhonguo2118.cn

C#:   Console.ReadLine();
来源：https://ro.zhonguo8118.cn

[A21] 保留指定小数位输出
来源：https://du.zhonguo4118.cn

Py:   f"{3.14159:.2f}"
来源：https://cp.zhonguo3118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://eg.zhonguo2118.cn

JS:   (3.14159).toFixed(2)
来源：https://ni.zhonguo1118.cn

TS:   (3.14159).toFixed(2)
来源：https://kv.zhonguo1118.cn

Java: String.format("%.2f", 3.14159)
来源：https://nf.zhonguo8118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://kh.zhonguo4118.cn

Ruby: format("%.2f", 3.14159)
来源：https://nm.zhonguo8118.cn

C#:   3.14159.ToString("F2")
来源：https://dm.zhonguo5118.cn

[A22] 获取字符串长度
来源：https://do.zhonguo1118.cn

Py:   len(s)
来源：https://fc.zhonguo7118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://rp.zhonguo4118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://fh.zhonguo8118.cn

TS:   s.length
来源：https://jc.zhonguo7118.cn

Java: s.length()
来源：https://rj.zhonguo7118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://je.zhonguo7118.cn

Ruby: s.length
来源：https://wk.zhonguo2118.cn

C#:   s.Length
来源：https://es.zhonguo5118.cn

[A23] 大小写转换
来源：https://os.zhonguo8118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://tp.zhonguo2118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://rg.zhonguo2118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://xb.zhonguo7118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://yh.zhonguo7118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://sp.zhonguo7118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://vk.zhonguo4118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://uv.zhonguo8118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://rh.zhonguo1118.cn

[A24] 去除首尾空白
来源：https://mu.zhonguo3118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://ic.zhonguo1118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://aj.zhonguo3118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://ui.zhonguo6118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://hi.zhonguo1118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://xc.zhonguo3118.cn

Go:   strings.TrimSpace(s)
来源：https://or.zhonguo5118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://zq.zhonguo8118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://ov.zhonguo6118.cn

[A25] 字符串比较
来源：https://oh.zhonguo5118.cn

Py:   s1 == s2; s1 != s2
来源：https://kx.zhonguo7118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://tb.zhonguo6118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://hr.zhonguo2118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://qc.zhonguo1118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://zy.zhonguo6118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://eg.zhonguo3118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://ab.zhonguo2118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://kh.zhonguo6118.cn

[A26] 类型转换总览
来源：https://rd.zhonguo6118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://ng.zhonguo1118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://wr.zhonguo8118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://rd.zhonguo3118.cn

TS:   Number() String() Boolean() x as number
来源：https://yt.zhonguo1118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://di.zhonguo4118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://mh.zhonguo2118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://yu.zhonguo2118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://ya.zhonguo4118.cn

================================================================================
来源：https://jy.zhonguo6118.cn

B. 流程控制
来源：https://qv.zhonguo6118.cn

================================================================================
来源：https://bb.zhonguo3118.cn

[B01] 条件判断 if / else
来源：https://wo.zhonguo3118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://ko.zhonguo5118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://hr.zhonguo4118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://fs.zhonguo1118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://qs.zhonguo6118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://jw.zhonguo2118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://kv.zhonguo6118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://fa.zhonguo3118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://fs.zhonguo8118.cn

[B02] 多分支 else if / elif
来源：https://eh.zhonguo6118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://oh.zhonguo8118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://tv.zhonguo2118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://oh.zhonguo4118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://lv.zhonguo6118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://la.zhonguo3118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://yq.zhonguo4118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://sl.zhonguo3118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://cv.zhonguo3118.cn

[B03] switch / match / case
来源：https://zd.zhonguo2118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://er.zhonguo6118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://lc.zhonguo8118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://qi.zhonguo6118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://cn.zhonguo8118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://xc.zhonguo6118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://uz.zhonguo6118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://ov.zhonguo3118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://iy.zhonguo1118.cn

[B04] for 计数循环
来源：https://do.zhonguo7118.cn

Py:   for i in range(10): print(i)
来源：https://ml.zhonguo2118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://as.zhonguo4118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://uk.zhonguo2118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://lc.zhonguo8118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://xe.zhonguo4118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://qw.zhonguo6118.cn

Ruby: 10.times { |i| puts i }
来源：https://ph.zhonguo3118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://no.zhonguo1118.cn

[B05] 遍历数组 / 列表
来源：https://ai.zhonguo1118.cn

Py:   for item in arr: print(item)
来源：https://cg.zhonguo6118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://lg.zhonguo7118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://dt.zhonguo3118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://hf.zhonguo1118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://ba.zhonguo2118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://jk.zhonguo3118.cn

Ruby: arr.each { |item| puts item }
来源：https://tl.zhonguo7118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://qz.zhonguo7118.cn

[B06] 遍历字典 / 对象
来源：https://or.zhonguo7118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://ao.zhonguo5118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://rg.zhonguo1118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://xl.zhonguo6118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://ci.zhonguo1118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://jm.zhonguo5118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://ow.zhonguo8118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://xt.zhonguo1118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://pk.zhonguo6118.cn

[B07] while 循环
来源：https://af.zhonguo4118.cn

Py:   while i < 10: i += 1
来源：https://ir.zhonguo7118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://qn.zhonguo3118.cn

JS:   while (i < 10) { i++; }
来源：https://ft.zhonguo6118.cn

TS:   while (i < 10) { i++; }
来源：https://az.zhonguo7118.cn

Java: while (i < 10) { i++; }
来源：https://ce.zhonguo2118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://me.zhonguo2118.cn

Ruby: while i < 10; i += 1; end
来源：https://fs.zhonguo1118.cn

C#:   while (i < 10) { i++; }
来源：https://kb.zhonguo8118.cn

[B08] do-while（至少执行一次）
来源：https://xp.zhonguo8118.cn

Py:   # 无 do-while：用 while True + break
来源：https://gt.zhonguo6118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://mz.zhonguo5118.cn

JS:   do { i++; } while (i < 10);
来源：https://rv.zhonguo8118.cn

TS:   do { i++; } while (i < 10);
来源：https://iy.zhonguo8118.cn

Java: do { i++; } while (i < 10);
来源：https://he.zhonguo4118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://cs.zhonguo7118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://ny.zhonguo3118.cn

C#:   do { i++; } while (i < 10);
来源：https://xr.zhonguo6118.cn

[B09] break 与 continue
来源：https://ch.zhonguo2118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://ky.zhonguo1118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://me.zhonguo1118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://pu.zhonguo5118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://pk.zhonguo2118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://qi.zhonguo8118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://lb.zhonguo4118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://ow.zhonguo5118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://pg.zhonguo2118.cn

[B10] 遍历同时拿索引
来源：https://fz.zhonguo7118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://ou.zhonguo2118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://xn.zhonguo4118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://nz.zhonguo2118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://ig.zhonguo6118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://hk.zhonguo1118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://yh.zhonguo7118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://wk.zhonguo8118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://en.zhonguo6118.cn

[B11] 生成数字序列 / 区间
来源：https://yl.zhonguo6118.cn

Py:   list(range(0, 10, 2))
来源：https://rs.zhonguo6118.cn

PHP:  range(0, 10, 2);
来源：https://wu.zhonguo7118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://no.zhonguo4118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://gy.zhonguo8118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://dx.zhonguo6118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://vf.zhonguo7118.cn

Ruby: (0...10).step(2).to_a
来源：https://jc.zhonguo6118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://ee.zhonguo3118.cn

[B12] 跳出多层循环
来源：https://pj.zhonguo8118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://vb.zhonguo3118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://eo.zhonguo7118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://xz.zhonguo1118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://wl.zhonguo1118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://vh.zhonguo4118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://rj.zhonguo3118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://oo.zhonguo6118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://cv.zhonguo7118.cn

[B13] 判断是否为数字
来源：https://ov.zhonguo1118.cn

Py:   isinstance(x, (int, float))
来源：https://mo.zhonguo5118.cn

PHP:  is_numeric($x)
来源：https://ac.zhonguo3118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://gc.zhonguo2118.cn


<!-- 参考信息 -->