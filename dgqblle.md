代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：https://jn.zhonguo3118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://ix.zhonguo3118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://fy.zhonguo3118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://hp.zhonguo3118.cn

[A10] 生成随机数
来源：https://mf.zhonguo5118.cn

Py:   import random; random.randint(1, 100)
来源：https://fn.zhonguo4118.cn

PHP:  random_int(1, 100);
来源：https://oh.zhonguo2118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://nf.zhonguo4118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://yl.zhonguo2118.cn

Java: new Random().nextInt(100) + 1
来源：https://pg.zhonguo2118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://nm.zhonguo3118.cn

Ruby: rand(1..100)
来源：https://aw.zhonguo3118.cn

C#:   new Random().Next(1, 101)
来源：https://ct.zhonguo5118.cn

[A11] 条件表达式（三元）
来源：https://zt.zhonguo2118.cn

Py:   "yes" if x > 0 else "no"
来源：https://fp.zhonguo4118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://ym.zhonguo6118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://ge.zhonguo3118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://mm.zhonguo8118.cn

Java: x > 0 ? "yes" : "no"
来源：https://cf.zhonguo7118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://lj.zhonguo1118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://kr.zhonguo3118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://yq.zhonguo2118.cn

[A12] 字符串插值 / 格式化
来源：https://id.zhonguo3118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://li.zhonguo5118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://fw.zhonguo7118.cn

JS:   `Hello, ${name}!`
来源：https://mr.zhonguo5118.cn

TS:   `Hello, ${name}!`
来源：https://wn.zhonguo7118.cn

Java: "Hello, %s!".formatted(name)
来源：https://tl.zhonguo4118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://vq.zhonguo8118.cn

Ruby: "Hello, #{name}!"
来源：https://mr.zhonguo6118.cn

C#:   $"Hello, {name}!"
来源：https://vc.zhonguo1118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://pe.zhonguo8118.cn

Py:   "第一行\n第二行"
来源：https://sj.zhonguo8118.cn

PHP:  "第一行\n第二行"
来源：https://mt.zhonguo3118.cn

JS:   "第一行\n第二行"
来源：https://zz.zhonguo1118.cn

TS:   "第一行\n第二行"
来源：https://lc.zhonguo6118.cn

Java: "第一行\n第二行"
来源：https://oh.zhonguo6118.cn

Go:   "第一行\n第二行"
来源：https://en.zhonguo4118.cn

Ruby: "第一行\n第二行"
来源：https://ne.zhonguo8118.cn

C#:   "第一行\n第二行"
来源：https://sr.zhonguo4118.cn

[A14] 注释写法
来源：https://gj.zhonguo5118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://bw.zhonguo8118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://jl.zhonguo8118.cn

JS:   // 单行；/* 多行 */
来源：https://xe.zhonguo4118.cn

TS:   // 单行；/* 多行 */
来源：https://rj.zhonguo3118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://ow.zhonguo3118.cn

Go:   // 单行；/* 多行 */
来源：https://lo.zhonguo6118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://hr.zhonguo1118.cn

C#:   // 单行；/* 多行 */
来源：https://ah.zhonguo2118.cn

[A15] 空值判断与默认值
来源：https://sr.zhonguo3118.cn

Py:   value = data or "默认值"
来源：https://gy.zhonguo3118.cn

PHP:  $value = $data ?? "默认值";
来源：https://tw.zhonguo6118.cn

JS:   const value = data ?? "默认值";
来源：https://lf.zhonguo6118.cn

TS:   const value = data ?? "默认值";
来源：https://rz.zhonguo2118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://gi.zhonguo1118.cn

Go:   if data == "" { data = "默认值" }
来源：https://mu.zhonguo7118.cn

Ruby: value = data || "默认值"
来源：https://rd.zhonguo8118.cn

C#:   var value = data ?? "默认值";
来源：https://zq.zhonguo5118.cn

[A16] 真假值判断规则
来源：https://ao.zhonguo6118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://rp.zhonguo3118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://cl.zhonguo4118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://dl.zhonguo1118.cn

TS:   if (!x) {}
来源：https://xr.zhonguo6118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://gg.zhonguo5118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://yj.zhonguo4118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://uh.zhonguo3118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://tv.zhonguo6118.cn

[A17] 位运算
来源：https://gb.zhonguo8118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://xh.zhonguo2118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://ef.zhonguo2118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ai.zhonguo3118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://zq.zhonguo7118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://fk.zhonguo7118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://fz.zhonguo4118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://li.zhonguo4118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://hg.zhonguo4118.cn

[A18] 字符与 ASCII 码互转
来源：https://tt.zhonguo8118.cn

Py:   ord("A"); chr(65)
来源：https://xg.zhonguo2118.cn

PHP:  ord("A"); chr(65)
来源：https://cy.zhonguo1118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://cc.zhonguo2118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://zf.zhonguo3118.cn

Java: (int) 'A'; (char) 65
来源：https://ba.zhonguo7118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://vc.zhonguo8118.cn

Ruby: "A".ord; 65.chr
来源：https://jq.zhonguo1118.cn

C#:   (int)'A'; (char)65
来源：https://jb.zhonguo7118.cn

[A19] 交换两个变量
来源：https://tz.zhonguo7118.cn

Py:   a, b = b, a
来源：https://wu.zhonguo2118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://ph.zhonguo1118.cn

JS:   [a, b] = [b, a];
来源：https://pl.zhonguo5118.cn

TS:   [a, b] = [b, a];
来源：https://gt.zhonguo3118.cn

Java: int t = a; a = b; b = t;
来源：https://rq.zhonguo7118.cn

Go:   a, b = b, a
来源：https://zq.zhonguo2118.cn

Ruby: a, b = b, a
来源：https://bp.zhonguo7118.cn

C#:   (a, b) = (b, a);
来源：https://iv.zhonguo4118.cn

[A20] 读取标准输入
来源：https://ad.zhonguo5118.cn

Py:   name = input("请输入：")
来源：https://kf.zhonguo2118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://ro.zhonguo3118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://xm.zhonguo3118.cn

TS:   // Node.js：readline 模块
来源：https://jr.zhonguo1118.cn

Java: new Scanner(System.in).nextLine()
来源：https://mq.zhonguo2118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://kg.zhonguo3118.cn

Ruby: gets.chomp
来源：https://lf.zhonguo6118.cn

C#:   Console.ReadLine();
来源：https://yo.zhonguo8118.cn

[A21] 保留指定小数位输出
来源：https://vx.zhonguo6118.cn

Py:   f"{3.14159:.2f}"
来源：https://wh.zhonguo1118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://hb.zhonguo3118.cn

JS:   (3.14159).toFixed(2)
来源：https://dk.zhonguo2118.cn

TS:   (3.14159).toFixed(2)
来源：https://gk.zhonguo8118.cn

Java: String.format("%.2f", 3.14159)
来源：https://po.zhonguo4118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://le.zhonguo7118.cn

Ruby: format("%.2f", 3.14159)
来源：https://hv.zhonguo3118.cn

C#:   3.14159.ToString("F2")
来源：https://mo.zhonguo8118.cn

[A22] 获取字符串长度
来源：https://si.zhonguo7118.cn

Py:   len(s)
来源：https://tc.zhonguo2118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://gt.zhonguo3118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://pw.zhonguo5118.cn

TS:   s.length
来源：https://px.zhonguo2118.cn

Java: s.length()
来源：https://kq.zhonguo4118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://dl.zhonguo8118.cn

Ruby: s.length
来源：https://ts.zhonguo4118.cn

C#:   s.Length
来源：https://vx.zhonguo1118.cn

[A23] 大小写转换
来源：https://en.zhonguo6118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://kt.zhonguo5118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://ej.zhonguo2118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://nc.zhonguo2118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://vu.zhonguo8118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://tm.zhonguo4118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://od.zhonguo5118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://bi.zhonguo2118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://qx.zhonguo5118.cn

[A24] 去除首尾空白
来源：https://hf.zhonguo1118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://ao.zhonguo3118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://au.zhonguo2118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://aj.zhonguo7118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://lv.zhonguo5118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://pw.zhonguo4118.cn

Go:   strings.TrimSpace(s)
来源：https://ig.zhonguo7118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://ra.zhonguo2118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://jt.zhonguo3118.cn

[A25] 字符串比较
来源：https://or.zhonguo6118.cn

Py:   s1 == s2; s1 != s2
来源：https://fe.zhonguo5118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://au.zhonguo2118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://su.zhonguo8118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://ju.zhonguo4118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://bf.zhonguo4118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://ch.zhonguo8118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://rc.zhonguo1118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://ha.zhonguo3118.cn

[A26] 类型转换总览
来源：https://bk.zhonguo7118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://jb.zhonguo4118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://lj.zhonguo5118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://iy.zhonguo8118.cn

TS:   Number() String() Boolean() x as number
来源：https://om.zhonguo6118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://gw.zhonguo1118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://kg.zhonguo4118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://vr.zhonguo7118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://fh.zhonguo1118.cn

================================================================================
来源：https://kv.zhonguo7118.cn

B. 流程控制
来源：https://mw.zhonguo2118.cn

================================================================================
来源：https://iv.zhonguo2118.cn

[B01] 条件判断 if / else
来源：https://to.zhonguo7118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://ws.zhonguo4118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://el.zhonguo8118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://xt.zhonguo1118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://hz.zhonguo7118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://oa.zhonguo8118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://uu.zhonguo6118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://pk.zhonguo4118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://em.zhonguo1118.cn

[B02] 多分支 else if / elif
来源：https://rn.zhonguo8118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://yo.zhonguo4118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://ht.zhonguo4118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ji.zhonguo3118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ee.zhonguo6118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://vd.zhonguo6118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://cy.zhonguo5118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://sd.zhonguo3118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://cl.zhonguo6118.cn

[B03] switch / match / case
来源：https://gy.zhonguo7118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://oh.zhonguo4118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://tl.zhonguo7118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://im.zhonguo2118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://ke.zhonguo7118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://rf.zhonguo3118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://bc.zhonguo6118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://hy.zhonguo7118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://xu.zhonguo1118.cn

[B04] for 计数循环
来源：https://sn.zhonguo5118.cn

Py:   for i in range(10): print(i)
来源：https://mo.zhonguo8118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://ec.zhonguo6118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://xe.zhonguo3118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://wv.zhonguo6118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://hi.zhonguo7118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://wu.zhonguo6118.cn

Ruby: 10.times { |i| puts i }
来源：https://qv.zhonguo2118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://os.zhonguo6118.cn

[B05] 遍历数组 / 列表
来源：https://on.zhonguo4118.cn

Py:   for item in arr: print(item)
来源：https://ra.zhonguo7118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://so.zhonguo8118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://pa.zhonguo2118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://rt.zhonguo7118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://do.zhonguo8118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://cw.zhonguo1118.cn

Ruby: arr.each { |item| puts item }
来源：https://nb.zhonguo5118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://mi.zhonguo2118.cn

[B06] 遍历字典 / 对象
来源：https://yp.zhonguo3118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://hv.zhonguo2118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://kn.zhonguo3118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://xg.zhonguo7118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://nr.zhonguo3118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://cj.zhonguo8118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://cj.zhonguo3118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://dp.zhonguo2118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://jk.zhonguo4118.cn

[B07] while 循环
来源：https://ja.zhonguo8118.cn

Py:   while i < 10: i += 1
来源：https://sd.zhonguo6118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://lf.zhonguo4118.cn

JS:   while (i < 10) { i++; }
来源：https://iq.zhonguo2118.cn

TS:   while (i < 10) { i++; }
来源：https://zz.zhonguo4118.cn

Java: while (i < 10) { i++; }
来源：https://he.zhonguo2118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://nu.zhonguo4118.cn

Ruby: while i < 10; i += 1; end
来源：https://xo.zhonguo6118.cn

C#:   while (i < 10) { i++; }
来源：https://uu.zhonguo4118.cn

[B08] do-while（至少执行一次）
来源：https://mc.zhonguo1118.cn

Py:   # 无 do-while：用 while True + break
来源：https://ux.zhonguo8118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://lg.zhonguo6118.cn

JS:   do { i++; } while (i < 10);
来源：https://bm.zhonguo1118.cn

TS:   do { i++; } while (i < 10);
来源：https://pm.zhonguo8118.cn

Java: do { i++; } while (i < 10);
来源：https://kt.zhonguo4118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://xo.zhonguo6118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://wd.zhonguo7118.cn

C#:   do { i++; } while (i < 10);
来源：https://uo.zhonguo7118.cn

[B09] break 与 continue
来源：https://gl.zhonguo7118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://hq.zhonguo8118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://ux.zhonguo4118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://mo.zhonguo1118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://xe.zhonguo2118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ng.zhonguo6118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://fk.zhonguo2118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://qu.zhonguo1118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ya.zhonguo2118.cn

[B10] 遍历同时拿索引
来源：https://es.zhonguo6118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://fv.zhonguo3118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://xu.zhonguo7118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://qv.zhonguo6118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://nj.zhonguo8118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://yg.zhonguo2118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://gz.zhonguo1118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://vv.zhonguo5118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://kz.zhonguo2118.cn

[B11] 生成数字序列 / 区间
来源：https://nq.zhonguo7118.cn

Py:   list(range(0, 10, 2))
来源：https://zj.zhonguo6118.cn

PHP:  range(0, 10, 2);
来源：https://rc.zhonguo7118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://tu.zhonguo8118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://eg.zhonguo7118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://ul.zhonguo3118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://os.zhonguo4118.cn

Ruby: (0...10).step(2).to_a
来源：https://rv.zhonguo5118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://by.zhonguo1118.cn

[B12] 跳出多层循环
来源：https://yh.zhonguo5118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://br.zhonguo4118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://fx.zhonguo7118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://ng.zhonguo4118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://su.zhonguo2118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://xe.zhonguo1118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://cw.zhonguo1118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://ga.zhonguo5118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://qy.zhonguo3118.cn

[B13] 判断是否为数字
来源：https://ui.zhonguo8118.cn

Py:   isinstance(x, (int, float))
来源：https://mv.zhonguo6118.cn

PHP:  is_numeric($x)
来源：https://zd.zhonguo2118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://re.zhonguo4118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ym.zhonguo6118.cn

Java: x instanceof Number
来源：https://ju.zhonguo4118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://sp.zhonguo2118.cn

Ruby: x.is_a?(Numeric)
来源：https://wx.zhonguo6118.cn

C#:   x is int or double or decimal
来源：https://co.zhonguo7118.cn

[B14] 判断值是否在集合内
来源：https://vh.zhonguo6118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://ly.zhonguo3118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://dx.zhonguo5118.cn

JS:   [1, 2, 3].includes(x)
来源：https://dw.zhonguo1118.cn

TS:   [1, 2, 3].includes(x)
来源：https://zq.zhonguo2118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://bf.zhonguo3118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://bt.zhonguo7118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://rl.zhonguo1118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://iu.zhonguo8118.cn

[B15] 布尔运算与取反
来源：https://ni.zhonguo7118.cn

Py:   a and b or not c
来源：https://tx.zhonguo2118.cn

PHP:  $a && $b || !$c
来源：https://rj.zhonguo5118.cn

JS:   a && b || !c
来源：https://sh.zhonguo5118.cn

TS:   a && b || !c
来源：https://pm.zhonguo1118.cn

Java: a && b || !c
来源：https://tk.zhonguo6118.cn

Go:   a && b || !c
来源：https://ix.zhonguo3118.cn

Ruby: a && b || !c
来源：https://bx.zhonguo7118.cn

C#:   a && b || !c
来源：https://bz.zhonguo6118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://nm.zhonguo4118.cn

Py:   if not data: return
来源：https://uk.zhonguo1118.cn

PHP:  if (!$data) { return; }
来源：https://gb.zhonguo3118.cn

JS:   if (!data) return;
来源：https://jc.zhonguo6118.cn

TS:   if (!data) return;
来源：https://xx.zhonguo5118.cn


<!-- 参考信息 -->