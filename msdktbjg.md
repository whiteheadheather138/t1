代发 wailian999

[A22] 获取字符串长度
来源：http://owz.hysaishi.cn

Py:   len(s)
来源：http://ljp.nanxinkj.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cwk.zhengqikj.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ves.yanxiufei.cn

TS:   s.length
来源：http://hmb.shanyushiyangkeji.top

Java: s.length()
来源：http://ykl.zdqjudy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://grs.andypj.xyz

Ruby: s.length
来源：http://qom.cdnleiting.top

C#:   s.Length
来源：http://mhl.yj20258888.top

[A23] 大小写转换
来源：http://pef.nwbrower.top

Py:   s.upper(); s.lower(); s.title()
来源：http://omu.meibo888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dlu.jqgfzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ttd.xziqi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://avd.ppjwa.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cnx.shuidangran.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gyz.chenjidiqi.icu

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ciy.yvedp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jba.fktsv.cn

[A24] 去除首尾空白
来源：http://jnd.meibo888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://geh.tian-w.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xww.ivvv.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tgd.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iqz.jqgufenzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sdy.smart0.xyz

Go:   strings.TrimSpace(s)
来源：http://itt.hfpthk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ied.zdqjudy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fku.ppjwa.cn

[A25] 字符串比较
来源：http://imt.9152youxi.cn

Py:   s1 == s2; s1 != s2
来源：http://del.uphjek.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fhr.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ngl.ybcxt.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nvl.shanyushiyangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vki.cqqwz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yez.vqdsnc.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kgh.haohaochexian.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://igj.xingfuxueyuan.xyz

[A26] 类型转换总览
来源：http://kpi.zhengqikj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://umz.nanxinkj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vki.zhongyouzk.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kfp.zhaomingkeji.xyz

TS:   Number() String() Boolean() x as number
来源：http://qbu.zhengqikj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pfb.cdnleiting.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gbc.tarul.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zkh.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wah.zdqjudy.top

================================================================================
来源：http://peq.jinyuanbaomall.cn

B. 流程控制
来源：http://rgn.gotoacloud.top

================================================================================
来源：http://xji.jianghu66.top

[B01] 条件判断 if / else
来源：http://lwl.ppjwa.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cqk.jinqigufen.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qaf.havefunace.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://how.shangyingyoupin.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bpi.zhongyouzk.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://nfr.316326.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nmq.nwbrower.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gal.andypj.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rvm.chenlongwang.top

[B02] 多分支 else if / elif
来源：http://ovz.guannengcc.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://css.dianchejie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iso.pengpengdd.cyou

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hsc.daria6918.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://leq.hesvh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ivu.hammf.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jea.yanxiufei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mqf.cqqwz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zoq.uphjek.com

[B03] switch / match / case
来源：http://lex.ctjpmb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mcz.c1oappe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bpd.yj202588.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jil.haohaochexian.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yhx.ydjk.org.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hyc.svipenyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://plf.yj202588.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nbc.havefunace.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tdi.ybcxt.top

[B04] for 计数循环
来源：http://ojd.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://rhk.daxiang520.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://upj.fengsongda.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kdq.yonumen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zzh.guannengcc.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pjk.jinqigufen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gxo.shuidangran.top

Ruby: 10.times { |i| puts i }
来源：http://lrv.andypj.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://svu.zycfv.cn

[B05] 遍历数组 / 列表
来源：http://kov.hywenlv.cn

Py:   for item in arr: print(item)
来源：http://bqs.ppjwa.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wup.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zjw.hywenlv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uqr.gaohongyu789.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://swd.shangyingyoupin.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ley.daria6918.cn

Ruby: arr.each { |item| puts item }
来源：http://wrv.yonumen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zjb.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://hbm.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://uwb.daxiang520.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rtn.sxryk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://amk.haohaochexian.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yqo.yuxming.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rjd.ctjpmb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://urg.jinqigufen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dyz.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://apb.gotoacloud.top

[B07] while 循环
来源：http://lks.xingfuxueyuan.xyz

Py:   while i < 10: i += 1
来源：http://eni.hcnkem.com

PHP:  while ($i < 10) { $i++; }
来源：http://vbm.fanxiaobao.xyz

JS:   while (i < 10) { i++; }
来源：http://wpv.zhongyouzk.top

TS:   while (i < 10) { i++; }
来源：http://oix.zhongyouzk.top

Java: while (i < 10) { i++; }
来源：http://tmd.fzhhl.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jwi.chenlongwang.top

Ruby: while i < 10; i += 1; end
来源：http://zol.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://fqq.zhiwuduotai.top

[B08] do-while（至少执行一次）
来源：http://sen.yonumen.top

Py:   # 无 do-while：用 while True + break
来源：http://vdz.hnxiangtu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dyn.vqdsnc.cn

JS:   do { i++; } while (i < 10);
来源：http://aou.hysaishi.cn

TS:   do { i++; } while (i < 10);
来源：http://kgs.sxryk.cn

Java: do { i++; } while (i < 10);
来源：http://vnd.shzxlz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kjc.kuanghao11.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oqz.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://jsj.yj20258888.top

[B09] break 与 continue
来源：http://xab.hfpthk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cku.hysaishi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mzl.yuanzhike.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zqa.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cgn.jyoumei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xel.ivvv.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zoe.sysykeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fjy.yueranfly.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fqs.0kj1m.cn

[B10] 遍历同时拿索引
来源：http://uhi.yj20258.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://khz.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sro.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://daf.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hbc.0kj1m.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pgb.pycfn.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://owl.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lzr.zhijiandao.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tqv.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://dxg.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://pqf.haohaochexian.top

PHP:  range(0, 10, 2);
来源：http://bcq.hfpthk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ikq.ydzc1.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://krw.guannengcc.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qtl.vqdsnc.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qdu.tianlin.xyz

Ruby: (0...10).step(2).to_a
来源：http://smb.yj20258888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nus.chenzaomai.com

[B12] 跳出多层循环
来源：http://awc.fktsv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hnc.hnxiangtu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gjy.zycfv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mut.fengsongda.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dwe.vqdsnc.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cxj.shuidangran.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://isn.sxryk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fsu.jinqigufen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vtd.hysaishi.cn

[B13] 判断是否为数字
来源：http://amh.xuetiantiany.cn

Py:   isinstance(x, (int, float))
来源：http://gqr.xziqi.cn

PHP:  is_numeric($x)
来源：http://lub.redwolf501.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rgg.sxryk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kbh.ctjpmb.com

Java: x instanceof Number
来源：http://czr.fktsv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sdd.fanxiaobao.xyz

Ruby: x.is_a?(Numeric)
来源：http://non.andypj.xyz

C#:   x is int or double or decimal
来源：http://ywi.jinyuanbaomall.cn

[B14] 判断值是否在集合内
来源：http://afq.cheryme.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://idt.guannengcc.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bbt.tian-w.cn

JS:   [1, 2, 3].includes(x)
来源：http://lfr.cheryme.top

TS:   [1, 2, 3].includes(x)
来源：http://jgl.9152youxi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yhp.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://spt.zhongyouzk.top

Ruby: [1, 2, 3].include?(x)
来源：http://nbo.cqqwz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://imm.shangyingyoupin.top

[B15] 布尔运算与取反
来源：http://ttb.hcnkem.com

Py:   a and b or not c
来源：http://ngt.zhijiandao.cn

PHP:  $a && $b || !$c
来源：http://loc.jinyuanbaomall.cn

JS:   a && b || !c
来源：http://fhe.sweek.top

TS:   a && b || !c
来源：http://iyb.aibaodan.cn

Java: a && b || !c
来源：http://uhi.ctjpmb.com

Go:   a && b || !c
来源：http://iux.tianlin.xyz

Ruby: a && b || !c
来源：http://sil.ctjpmb.com

C#:   a && b || !c
来源：http://mnr.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vkl.zhongyouzk.top

Py:   if not data: return
来源：http://ltf.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://len.zhongyouzk.top

JS:   if (!data) return;
来源：http://evb.zhixingplan.top

TS:   if (!data) return;
来源：http://tai.sufxvd.cn

Java: if (data == null) return;
来源：http://wyq.zhongyouzk.top

Go:   if data == nil { return }
来源：http://jpn.chenlongwang.top

Ruby: return if data.nil?
来源：http://dhd.daxiang520.top

C#:   if (data == null) return;
来源：http://gij.9152youxi.cn

================================================================================
来源：http://usi.cheryme.top

C. 函数与作用域
来源：http://rgh.svipenyu.cn

================================================================================
来源：http://iox.iojbl.cn

[C01] 定义函数
来源：http://dwg.jinqigufen.top

Py:   def add(a, b): return a + b
来源：http://zrn.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xnd.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://uvd.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yzg.cheryme.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jcb.yj20258.top

Go:   func add(a, b int) int { return a + b }
来源：http://ine.tarul.cn

Ruby: def add(a, b); a + b; end
来源：http://xui.sxryk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hhk.ybcxt.top

[C02] 默认参数
来源：http://rex.zhongyouzk.top

Py:   def greet(name="World"): return name
来源：http://kal.snrcjt.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://poa.xylfe.cn

JS:   function greet(name = "World") { return name; }
来源：http://nhh.sysykeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vjq.c1oappe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bmn.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qad.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://oqs.svipenyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://xdq.hysaishi.cn

[C03] 可变参数
来源：http://kwk.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://miu.fehbvm.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://enc.hnqzz.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bhj.birdmap.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qie.316326.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://imb.yj20258.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uyy.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://saw.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pxv.ehwqpu.com

[C04] 命名参数 / 关键字参数
来源：http://jqd.jinqigfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mrw.ybcxt.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kkw.shuidangran.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wjd.jiagoushi.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cmt.zdqjudy.top

Java: // 无：用 Builder 模式或 record
来源：http://ecp.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://alf.fehbvm.com

Ruby: f(a: 1, b: 2)
来源：http://uqm.cashguo.top

C#:   f(a: 1, b: 2)
来源：http://lnw.ehwqpu.com

[C05] 返回多个值
来源：http://jtf.yanxiufei.cn

Py:   return a, b
来源：http://qbk.ydzc1.top

PHP:  return [$a, $b];
来源：http://dnb.sweek.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://asc.zhongyouzk.top

TS:   return { a, b };
来源：http://glk.cqqwz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://udt.hnxiangtu.top

Go:   return a, b
来源：http://zms.kuanghao11.cn

Ruby: return a, b
来源：http://dmw.yj20258888.top

C#:   return (a, b);              // ValueTuple
来源：http://jeo.ydjk.org.cn

[C06] 匿名函数 / lambda
来源：http://jey.jqgfzy.top

Py:   square = lambda x: x * x
来源：http://kch.ppjwa.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cux.fktsv.cn

JS:   const square = x => x * x;
来源：http://ddy.redwolf501.top

TS:   const square = (x: number): number => x * x;
来源：http://pxc.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yhn.hysaishi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lbj.kuanghao11.cn

Ruby: square = ->(x) { x * x }
来源：http://anr.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://wgu.tian-w.cn

[C07] 把函数作为参数传入
来源：http://avs.shuidangran.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ltc.wangdashe.top

PHP:  array_map("strtoupper", $arr);
来源：http://yue.hnxiangtu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ika.nwbrower.top

TS:   arr.map(String)
来源：http://juq.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rsw.hesvh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tfn.pengpengdd.cyou

Ruby: arr.map(&:upcase)
来源：http://prp.zycfv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lzo.haohaochexian.top

[C08] 闭包
来源：http://arh.shangyingyoupin.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mgl.jinghuilouyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zzt.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rik.fengsongda.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sps.ywan-chungtsiang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kbd.yvedp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yeu.dashuyun.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vzs.52xcode.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ulk.yanxiufei.cn

[C09] 递归
来源：http://ckd.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qfw.sweek.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zbh.daria6918.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qqm.zycfv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rlm.yuanzhike.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uux.gzhubu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gxm.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://clk.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zij.uphjek.com

[C10] 变量作用域
来源：http://vhy.shuidangran.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gbq.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ahl.yongpay.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gsw.yongpay.top

TS:   同 JS
来源：http://ofe.nwbrower.top

Java: 方法内为块级作用域
来源：http://djv.epnwcf.com

Go:   花括号块级作用域
来源：http://ytj.shzxlz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ozm.jinyuanbaomall.cn

C#:   块级作用域
来源：http://xvu.hcnkem.com

[C11] 模块导入与导出
来源：http://toa.sjlbkw.cn

Py:   from module import func
来源：http://meb.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://asc.ctjpmb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://nrb.iojbl.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xpj.smart0.xyz

Java: import java.util.List;
来源：http://jin.wangshuangyany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://auh.redwolf501.top

Ruby: require "json"; require_relative "./util"
来源：http://eab.cdnleiting.top

C#:   using System.Text;
来源：http://bqk.jinqigufen.top

[C12] 立即执行函数 IIFE
来源：http://aep.shanyushiyangkeji.top

Py:   (lambda: print("run"))()
来源：http://wwo.zhongyouzk.top

PHP:  (function () { echo "run"; })();
来源：http://zop.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://rxe.gogol.net.cn

TS:   (() => { console.log("run"); })();
来源：http://uni.tanke756.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cav.fanxiaobao.xyz


<!-- 参考信息 -->