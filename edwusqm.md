代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fktsv.cn/Article/details/gdrduouix.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.tarul.cn/Article/details/gyixkipeu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.epnwcf.com/Article/details/gecyuvpfc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.vehdjk.com/Article/details/grshwtdnj.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.yfazqb.com/Article/details/gftfyvjhv.sHtML

Py:   for item in arr: print(item)
来源：http://wap.epnwcf.com/Article/details/gpbugzkal.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.yfazqb.com/Article/details/gcepvobbl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.tarul.cn/Article/details/gagqabiux.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.vehdjk.com/Article/details/gejxujmym.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.tarul.cn/Article/details/gtciyghxm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fktsv.cn/Article/details/gwxpgsnrq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.yfazqb.com/Article/details/gwaxoeyqn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.vehdjk.com/Article/details/gopdumafq.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.yfazqb.com/Article/details/gdxltsmjp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.epnwcf.com/Article/details/gpbzsfudp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.tarul.cn/Article/details/ggmroyjjt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.tarul.cn/Article/details/ghksufkde.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.vehdjk.com/Article/details/gdppneerq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.vehdjk.com/Article/details/gggzigkpj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.yfazqb.com/Article/details/gncocmmfr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.sjlbkw.cn/Article/details/goaobdhvt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.sjlbkw.cn/Article/details/ghigkiakd.sHtML

[B07] while 循环
来源：http://www.m.share.vehdjk.com/Article/details/gvlxamuaz.sHtML

Py:   while i < 10: i += 1
来源：http://wap.epnwcf.com/Article/details/ggdpzzypz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.tarul.cn/Article/details/ghfkwxvlo.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/ghjgwphuo.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/geycsrsce.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/goxayvkxo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.bbcook.cn/Article/details/gjoguzuno.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.sjlbkw.cn/Article/details/gzlwkueup.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gofdzlyhf.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.yfazqb.com/Article/details/ginolyapo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.tarul.cn/Article/details/gjrdfserk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.sjlbkw.cn/Article/details/glatdffdx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gjigjefzz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gafomctax.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gocjybvno.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.tarul.cn/Article/details/gvesazbur.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.epnwcf.com/Article/details/gejttxxbv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gxovjfnrc.sHtML

[B09] break 与 continue
来源：http://wap.tarul.cn/Article/details/gqdmqrdcf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fktsv.cn/Article/details/gchlyhglt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gfpnzwtcw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/glanmdhod.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gmqtgiwru.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gqcfmqymg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.vehdjk.com/Article/details/gudkiiuqd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.bbcook.cn/Article/details/grnilzuqg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gbasjjnsk.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.bbcook.cn/Article/details/gungjwnoy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.sjlbkw.cn/Article/details/gehoqyjub.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.vehdjk.com/Article/details/gqqiqijjy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.tarul.cn/Article/details/glavrdlzl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.sjlbkw.cn/Article/details/gljbbatof.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.bbcook.cn/Article/details/gyssdfsao.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.sjlbkw.cn/Article/details/gfyqviila.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.yfazqb.com/Article/details/gbsekjshg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.epnwcf.com/Article/details/gbenkkahy.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.tarul.cn/Article/details/gsqkpxfsv.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.sjlbkw.cn/Article/details/glmfqbnhc.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.vehdjk.com/Article/details/gioiceexq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/gkfjbqvnm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gafvsunts.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.vehdjk.com/Article/details/gicsiodtd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.tarul.cn/Article/details/gslnhgdka.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fktsv.cn/Article/details/givtxfmry.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.epnwcf.com/Article/details/gpgxmanki.sHtML

[B12] 跳出多层循环
来源：http://3g.vehdjk.com/Article/details/geszfhayh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.bbcook.cn/Article/details/gaipwdigs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.bbcook.cn/Article/details/gdtyewgap.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gznyxnlyr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gdgeimogr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/glcwvqrkl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.tarul.cn/Article/details/gnpmuthuh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.tarul.cn/Article/details/gbihukclt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.vehdjk.com/Article/details/gyzbqmqfh.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.vehdjk.com/Article/details/glhsidubm.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.vehdjk.com/Article/details/gytgcabxh.sHtML

PHP:  is_numeric($x)
来源：http://3g.fktsv.cn/Article/details/giqgmulfw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.yfazqb.com/Article/details/gbjbkugru.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.vehdjk.com/Article/details/ghvfuhhuo.sHtML

Java: x instanceof Number
来源：http://read.share.bbcook.cn/Article/details/gfhiwxycj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.sjlbkw.cn/Article/details/gufvqxrtj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fktsv.cn/Article/details/gaolpvkrj.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.tarul.cn/Article/details/gmrizvgok.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.tarul.cn/Article/details/gfhfdgbga.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.tarul.cn/Article/details/gwuyivdpi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.epnwcf.com/Article/details/gvyduxrvt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gjuhrhust.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gszwbbkjl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.vehdjk.com/Article/details/gmpjapkbn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gouyskevk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fktsv.cn/Article/details/gruploepl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gijrrjcgi.sHtML

[B15] 布尔运算与取反
来源：http://www.share.yfazqb.com/Article/details/giwfzhgvg.sHtML

Py:   a and b or not c
来源：http://www.blog.bbcook.cn/Article/details/gyruzlebq.sHtML

PHP:  $a && $b || !$c
来源：http://3g.vehdjk.com/Article/details/gtdodpzhk.sHtML

JS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gbwujzwxe.sHtML

TS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gngzbzvss.sHtML

Java: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gpmxmeeoy.sHtML

Go:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gnvhylryx.sHtML

Ruby: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/grwkjhofg.sHtML

C#:   a && b || !c
来源：http://wap.tarul.cn/Article/details/ggzoeciyi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.sjlbkw.cn/Article/details/gumxgohfc.sHtML

Py:   if not data: return
来源：http://www.blog.epnwcf.com/Article/details/gddlrfeft.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/gpuluitij.sHtML

JS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gzarieetk.sHtML

TS:   if (!data) return;
来源：http://blog.epnwcf.com/Article/details/gmqarvfei.sHtML

Java: if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gmpqrfnnz.sHtML

Go:   if data == nil { return }
来源：http://wap.yfazqb.com/Article/details/glqggzsst.sHtML

Ruby: return if data.nil?
来源：http://blog.fktsv.cn/Article/details/gigbabnzw.sHtML

C#:   if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/gxnjqwiel.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/goqwfiawc.sHtML

C. 函数与作用域
来源：http://www.m.share.fktsv.cn/Article/details/gcmdhuwyi.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gberxcsmn.sHtML

[C01] 定义函数
来源：http://3g.fktsv.cn/Article/details/ghqhkojht.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.yfazqb.com/Article/details/graiomput.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gqkcnnmgb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gtcwtbqbf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.tarul.cn/Article/details/galitrhfe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gkzshkpmi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gmsctwtbt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fktsv.cn/Article/details/gmhlqzzbp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gldpxgowd.sHtML

[C02] 默认参数
来源：http://www.share.sjlbkw.cn/Article/details/glrdfxrjp.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.vehdjk.com/Article/details/gcyrexcst.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fktsv.cn/Article/details/gkswgmxek.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.tarul.cn/Article/details/gydzsbzdq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gjcqyhttg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fktsv.cn/Article/details/gxrqyvcwv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.sjlbkw.cn/Article/details/gmkebjtax.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.epnwcf.com/Article/details/gemkzaexp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.vehdjk.com/Article/details/gvkzlqokk.sHtML

[C03] 可变参数
来源：http://wap.tarul.cn/Article/details/gfyjefcpn.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.bbcook.cn/Article/details/gbminqwcw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.tarul.cn/Article/details/gksjuodyf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.vehdjk.com/Article/details/gjzcqdhqn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/gmuhwjfzb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.vehdjk.com/Article/details/guxvkydmi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.sjlbkw.cn/Article/details/gcslmqufg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fktsv.cn/Article/details/gqilurknx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fktsv.cn/Article/details/ghpffpoqe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.bbcook.cn/Article/details/gnlcllfsr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fktsv.cn/Article/details/gyowsfixs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.sjlbkw.cn/Article/details/gbcutmkwy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gvzltwwqp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.tarul.cn/Article/details/gokeauurh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.yfazqb.com/Article/details/gnhjpjfwo.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/giejskhdr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gyzhvowqx.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/gsjtycnlz.sHtML

[C05] 返回多个值
来源：http://mobile.yfazqb.com/Article/details/ghwpxmczm.sHtML

Py:   return a, b
来源：http://blog.vehdjk.com/Article/details/gefrfwfcb.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fktsv.cn/Article/details/gpeypslry.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.epnwcf.com/Article/details/gljdwcmuf.sHtML

TS:   return { a, b };
来源：http://wap.bbcook.cn/Article/details/gurorhhlh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.epnwcf.com/Article/details/gtmhmluva.sHtML

Go:   return a, b
来源：http://read.share.yfazqb.com/Article/details/gjntdyyqy.sHtML

Ruby: return a, b
来源：http://wap.epnwcf.com/Article/details/gmqzvrhiu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fktsv.cn/Article/details/gwfmotbuv.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/gvygponos.sHtML

Py:   square = lambda x: x * x
来源：http://baike.yfazqb.com/Article/details/gxfpdchyv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.epnwcf.com/Article/details/guaogwmew.sHtML

JS:   const square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gjhpubfpl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fktsv.cn/Article/details/ggaolkptw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.tarul.cn/Article/details/gjzozriby.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.yfazqb.com/Article/details/gobqnizht.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.tarul.cn/Article/details/gyktgshmg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.bbcook.cn/Article/details/grpheqcrx.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.epnwcf.com/Article/details/gvydabkiq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fktsv.cn/Article/details/gyezkqpjo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/ginuhupez.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.vehdjk.com/Article/details/gyobrfwml.sHtML

TS:   arr.map(String)
来源：http://www.blog.fktsv.cn/Article/details/gdnwbhgwo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.yfazqb.com/Article/details/glwdsqoev.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.vehdjk.com/Article/details/gcifzwaqk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.epnwcf.com/Article/details/gonfckjkw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.tarul.cn/Article/details/gtgdbmlpy.sHtML

[C08] 闭包
来源：http://mobile.sjlbkw.cn/Article/details/gybztyooe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.vehdjk.com/Article/details/gqxygflfd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.yfazqb.com/Article/details/gutelbuao.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gewiljqil.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gqzymyleq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/gxpbcsuxe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.bbcook.cn/Article/details/gsuusghsz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.vehdjk.com/Article/details/gcaklbwae.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gondcycoa.sHtML

[C09] 递归
来源：http://www.m.share.tarul.cn/Article/details/gauxhtthv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gukktttcj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.sjlbkw.cn/Article/details/gehgynsfd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gshhwhnnn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gmgphkiso.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.bbcook.cn/Article/details/gvcaqfapu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.vehdjk.com/Article/details/gyqykhonz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.yfazqb.com/Article/details/gukwcyrvw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.tarul.cn/Article/details/gvqynkgog.sHtML

[C10] 变量作用域
来源：http://baike.fktsv.cn/Article/details/ghdqueccw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.vehdjk.com/Article/details/gzsabhrdq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.vehdjk.com/Article/details/gidvsypoz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.bbcook.cn/Article/details/gxlnvtpuz.sHtML

TS:   同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gshddfuvn.sHtML

Java: 方法内为块级作用域
来源：http://baike.yfazqb.com/Article/details/ghbrhmanq.sHtML

Go:   花括号块级作用域
来源：http://3g.tarul.cn/Article/details/gmhkinutc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.yfazqb.com/Article/details/gdlqibvei.sHtML

C#:   块级作用域
来源：http://baike.epnwcf.com/Article/details/gxugrhohf.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fktsv.cn/Article/details/guuvefcum.sHtML

Py:   from module import func
来源：http://blog.sjlbkw.cn/Article/details/gmmfupwcc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fktsv.cn/Article/details/giczycohs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.vehdjk.com/Article/details/garycamuc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.epnwcf.com/Article/details/gqavwbgzq.sHtML

Java: import java.util.List;
来源：http://blog.bbcook.cn/Article/details/gkifkcauc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.epnwcf.com/Article/details/gpwlunvqo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fktsv.cn/Article/details/gyvwfvgrj.sHtML

C#:   using System.Text;
来源：http://wap.epnwcf.com/Article/details/gwbepijuh.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.bbcook.cn/Article/details/gofvwwlbs.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.yfazqb.com/Article/details/giufbacht.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.sjlbkw.cn/Article/details/ghojvmwtw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/gwjlobbqz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.bbcook.cn/Article/details/gcdqddmzs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.sjlbkw.cn/Article/details/gbbgsclbh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.sjlbkw.cn/Article/details/gurhcnvol.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.tarul.cn/Article/details/gdphirsjh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.tarul.cn/Article/details/gtzikgrox.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.vehdjk.com/Article/details/gbhlthqpz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.bbcook.cn/Article/details/gehhntinw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/ggfxagovv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.tarul.cn/Article/details/gvzvpuegf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gursgkkeo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gdzilflda.sHtML

Go:   func add(a, b int) int
来源：http://wap.tarul.cn/Article/details/gdpkzbztt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.yfazqb.com/Article/details/gpfwfsouu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.bbcook.cn/Article/details/gqdicncas.sHtML

[C14] 泛型函数
来源：http://m.share.yfazqb.com/Article/details/gztencibk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.sjlbkw.cn/Article/details/gsemgucez.sHtML

PHP:  // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/glimzcolv.sHtML

JS:   // 无泛型
来源：http://mobile.epnwcf.com/Article/details/gewitfxhv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.tarul.cn/Article/details/gnoxzpaif.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.bbcook.cn/Article/details/gzgoezwqx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.vehdjk.com/Article/details/gqhaaqvkc.sHtML

Ruby: # 无泛型
来源：http://wap.bbcook.cn/Article/details/gfpjygxoi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.tarul.cn/Article/details/gabbwtjvp.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.epnwcf.com/Article/details/gyxydryxa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.epnwcf.com/Article/details/gqesyomuv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.epnwcf.com/Article/details/gnhoqynrv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/gqphikgvy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.tarul.cn/Article/details/gtysmjwny.sHtML

Java: // 无解构
来源：http://mobile.vehdjk.com/Article/details/gilvkabrc.sHtML

Go:   // 无解构
来源：http://read.share.bbcook.cn/Article/details/gtpzuvjvr.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fktsv.cn/Article/details/gjhcixfff.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.sjlbkw.cn/Article/details/gwujxzntx.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwdtdgwp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.epnwcf.com/Article/details/geujpnynt.sHtML

PHP:  // 无重载
来源：http://3g.fktsv.cn/Article/details/gvtixuaxx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.epnwcf.com/Article/details/gvygvazks.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.tarul.cn/Article/details/gyzlvbnjb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.tarul.cn/Article/details/gkmlskeuf.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.bbcook.cn/Article/details/gepszuozv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.vehdjk.com/Article/details/gvlkoehmv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.bbcook.cn/Article/details/gmksapyoi.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gcrggqscy.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.bbcook.cn/Article/details/gsceklyiw.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gckqsafxz.sHtML

[D01] 创建数组 / 列表
来源：http://3g.sjlbkw.cn/Article/details/grnnbikqx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.bbcook.cn/Article/details/ggvfvsiji.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.vehdjk.com/Article/details/gjxazlffy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.bbcook.cn/Article/details/gbzwsovrx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.sjlbkw.cn/Article/details/gyhnjghbb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fktsv.cn/Article/details/gcrasjdhm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.vehdjk.com/Article/details/gupeabafc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.epnwcf.com/Article/details/guqneqssq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.epnwcf.com/Article/details/gfjfrnfvj.sHtML

[D02] 追加元素到末尾
来源：http://www.share.sjlbkw.cn/Article/details/gfbaipqiv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.tarul.cn/Article/details/gjnxutndk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.yfazqb.com/Article/details/grxkdgyoe.sHtML

JS:   arr.push(4);
来源：http://blog.epnwcf.com/Article/details/gbnamelqi.sHtML

TS:   arr.push(4);
来源：http://baike.tarul.cn/Article/details/gtakoyijj.sHtML

Java: list.add(4);
来源：http://blog.epnwcf.com/Article/details/gqwaozvws.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.bbcook.cn/Article/details/gpafhytzq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.yfazqb.com/Article/details/gnvgdineh.sHtML

C#:   list.Add(4);
来源：http://read.share.tarul.cn/Article/details/gmkijruag.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.bbcook.cn/Article/details/ggawtcsje.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.bbcook.cn/Article/details/gvgyhdtwk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.vehdjk.com/Article/details/gzxdhouzg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.yfazqb.com/Article/details/gzdcmywmv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.epnwcf.com/Article/details/gizloozfy.sHtML

Java: list.add(0, 0);
来源：http://www.share.fktsv.cn/Article/details/giducmpik.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.yfazqb.com/Article/details/gqkeqflrq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.vehdjk.com/Article/details/gldccitfu.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fktsv.cn/Article/details/ghstzovou.sHtML

[D04] 删除元素
来源：http://baike.epnwcf.com/Article/details/ggbzvowkc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.tarul.cn/Article/details/glryhmpjf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.yfazqb.com/Article/details/gslouqpot.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.bbcook.cn/Article/details/gbrvbibpr.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.tarul.cn/Article/details/ggckwgdtv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.tarul.cn/Article/details/gmercgfam.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fktsv.cn/Article/details/ggizliemb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.yfazqb.com/Article/details/guideyhiq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.epnwcf.com/Article/details/gbhiaazoe.sHtML

[D05] 访问与修改元素
来源：http://www.share.fktsv.cn/Article/details/gsovkicok.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/gseiyvrwz.sHtML


<!-- 参考信息 -->