代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://upp.52xcode.cn

Ruby: gets.chomp
来源：http://dzw.sweek.top

C#:   Console.ReadLine();
来源：http://azl.fanxiaobao.xyz

[A21] 保留指定小数位输出
来源：http://bew.fengsongda.top

Py:   f"{3.14159:.2f}"
来源：http://lrf.chenjidiqi.icu

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pfz.daria6918.cn

JS:   (3.14159).toFixed(2)
来源：http://rrx.vqdsnc.cn

TS:   (3.14159).toFixed(2)
来源：http://sgg.yongpay.top

Java: String.format("%.2f", 3.14159)
来源：http://yce.yvedp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jaj.vehdjk.com

Ruby: format("%.2f", 3.14159)
来源：http://ukt.yj20258.top

C#:   3.14159.ToString("F2")
来源：http://gea.zhaomingkeji.xyz

[A22] 获取字符串长度
来源：http://myo.ivvv.top

Py:   len(s)
来源：http://xiy.redwolf501.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wrh.zhiwuduotai.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jsh.sjlbkw.cn

TS:   s.length
来源：http://qda.daxiang520.top

Java: s.length()
来源：http://pna.hywenlv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fjv.wangdashe.top

Ruby: s.length
来源：http://vge.vqdsnc.cn

C#:   s.Length
来源：http://kjr.tanke756.top

[A23] 大小写转换
来源：http://int.yongpay.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ram.chenzaomai.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vuq.shangyingyoupin.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oyu.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qwi.cashguo.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kcc.yj202588.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dbk.zhoulong.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://azl.shuidangran.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ysn.ydjk.org.cn

[A24] 去除首尾空白
来源：http://ydz.zhiwuduotai.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jmt.chenzaomai.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://byf.nanxinkj.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://owd.ydjk.org.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kgq.yvedp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mfb.gaohongyu789.top

Go:   strings.TrimSpace(s)
来源：http://mvt.chenzaomai.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cec.vehdjk.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zkr.tanke756.top

[A25] 字符串比较
来源：http://ool.hfpthk.cn

Py:   s1 == s2; s1 != s2
来源：http://pwh.snrcjt.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qut.jinqigufen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tks.hnqzz.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rpd.bjfxy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xcu.ivvv.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ebd.zhengqikj.top

Ruby: s1 == s2; s1 <=> s2
来源：http://aob.wangshuangyany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sbo.hongshengwenyu.top

[A26] 类型转换总览
来源：http://muj.chenjidiqi.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nhh.tianlin.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://odt.daxiang520.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vkq.yj20258.top

TS:   Number() String() Boolean() x as number
来源：http://ser.jianghu66.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pbj.ppjwa.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wko.yuanzhike.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://urn.shuidangran.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qgg.fzhhl.top

================================================================================
来源：http://zep.xuetiantiany.cn

B. 流程控制
来源：http://wki.birdmap.top

================================================================================
来源：http://nlk.shanyushiyangkeji.top

[B01] 条件判断 if / else
来源：http://ezp.yuanzhike.top

Py:   result = "正" if x > 0 else "非正"
来源：http://dif.xylfe.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eqs.9152youxi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yiw.tianlin.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hfp.hfpthk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zij.zhiwuduotai.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://css.uphjek.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://igy.sweek.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xgi.haohaochexian.top

[B02] 多分支 else if / elif
来源：http://psm.pengpengdd.cyou

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dph.pengpengdd.cyou

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kvg.jinghuilouyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://efo.316326.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qbm.tarul.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://egx.yonumen.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cmr.zhiwuduotai.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qfb.zhijiandao.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ywb.tarul.cn

[B03] switch / match / case
来源：http://uru.c1oappe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nbc.jianghu66.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wks.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tpm.hysaishi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mlp.shanyushiyangtech.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ack.xylfe.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ppn.9152youxi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hku.jinqigfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xdq.yanxiufei.cn

[B04] for 计数循环
来源：http://arq.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://rlo.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eyg.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zdj.wangshuangyany.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qhg.zhoulong.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ryx.sxryk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pox.hongshengwenyu.top

Ruby: 10.times { |i| puts i }
来源：http://vaa.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dto.316326.xyz

[B05] 遍历数组 / 列表
来源：http://ofy.gzhubu.top

Py:   for item in arr: print(item)
来源：http://txp.zdbjq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lqt.tianlin.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://rbv.yj202588.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vrd.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zpe.yuxming.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dzt.epnwcf.com

Ruby: arr.each { |item| puts item }
来源：http://drb.wangshuangyany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cfe.316326.xyz

[B06] 遍历字典 / 对象
来源：http://goh.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://pgw.sysykeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ujc.tian-w.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jbc.aizwys.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zop.birdmap.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bhh.havefunace.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ldw.yuxming.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://epj.jyoumei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vbs.316326.xyz

[B07] while 循环
来源：http://xis.birdmap.top

Py:   while i < 10: i += 1
来源：http://uvx.ydzc1.top

PHP:  while ($i < 10) { $i++; }
来源：http://inb.zhaomingkeji.xyz

JS:   while (i < 10) { i++; }
来源：http://hug.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://xyr.wangdashe.top

Java: while (i < 10) { i++; }
来源：http://cpo.bbcook.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ard.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://doz.yanxiufei.cn

C#:   while (i < 10) { i++; }
来源：http://edt.nanxinkj.top

[B08] do-while（至少执行一次）
来源：http://bfg.nwbrower.top

Py:   # 无 do-while：用 while True + break
来源：http://kxc.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://kin.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://uum.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://rrp.sufxvd.cn

Java: do { i++; } while (i < 10);
来源：http://lmw.guowangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cmw.fengsongda.top

Ruby: begin; i += 1; end while i < 10
来源：http://xkz.9152youxi.cn

C#:   do { i++; } while (i < 10);
来源：http://too.hongshengwenyu.top

[B09] break 与 continue
来源：http://zpf.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://knc.bjfxy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ghl.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hbd.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tjg.snrcjt.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cml.tian-w.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://utm.nanxuanxn.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zvl.nwbrower.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ryr.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://dpa.ydjk.org.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vib.jinyuanbaomall.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lsu.zhijiandao.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://amb.316326.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pqk.ivvv.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wph.wangdashe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yoa.pycfn.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ssk.uphjek.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fqe.mhx1999.top

[B11] 生成数字序列 / 区间
来源：http://zet.fktsv.cn

Py:   list(range(0, 10, 2))
来源：http://adg.xylfe.cn

PHP:  range(0, 10, 2);
来源：http://oiv.chenjidiqi.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yvp.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://szy.ybcxt.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fju.yueranfly.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xzt.tanke756.top

Ruby: (0...10).step(2).to_a
来源：http://sew.birdmap.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ikv.daria6918.cn

[B12] 跳出多层循环
来源：http://mpn.shanyushiyangtech.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xno.haohaochexian.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fcx.hcnkem.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://owm.cheryme.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://syk.jinyuanbaomall.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bnp.meibo888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rrg.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qdr.ydzc1.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bfd.zhoulong.xyz

[B13] 判断是否为数字
来源：http://qfq.aibaodan.cn

Py:   isinstance(x, (int, float))
来源：http://mbl.jqgufenzy.top

PHP:  is_numeric($x)
来源：http://kra.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://smq.hnqzz.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://esx.tianlin.xyz

Java: x instanceof Number
来源：http://umn.shanyushiyangtech.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jai.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://lzt.fzhhl.top

C#:   x is int or double or decimal
来源：http://llr.mhx1999.top

[B14] 判断值是否在集合内
来源：http://gtk.bjfxy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fxn.sufxvd.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fkv.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://noa.jqgfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://sfx.hesvh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lht.ydzc1.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://new.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://wkl.sufxvd.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fsu.hnxiangtu.top

[B15] 布尔运算与取反
来源：http://lzi.svipenyu.cn

Py:   a and b or not c
来源：http://rxz.jiagoushi.top

PHP:  $a && $b || !$c
来源：http://hux.guowangkeji.top

JS:   a && b || !c
来源：http://daj.yuxming.cn

TS:   a && b || !c
来源：http://fhj.zhoulong.xyz

Java: a && b || !c
来源：http://bky.iojbl.cn

Go:   a && b || !c
来源：http://src.cashguo.top

Ruby: a && b || !c
来源：http://fsf.zhaomingkeji.xyz

C#:   a && b || !c
来源：http://mrc.kuanghao11.cn

[B16] 卫语句：不满足条件提前返回
来源：http://upr.xingfuxueyuan.xyz

Py:   if not data: return
来源：http://yif.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://yba.jqgufenzy.top

JS:   if (!data) return;
来源：http://rmg.fzhhl.top

TS:   if (!data) return;
来源：http://ncp.redwolf501.top

Java: if (data == null) return;
来源：http://djq.guannengcc.top

Go:   if data == nil { return }
来源：http://cld.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://vbm.yj20258.top

C#:   if (data == null) return;
来源：http://sfu.yuxming.cn

================================================================================
来源：http://bgg.chenjidiqi.icu

C. 函数与作用域
来源：http://ein.cheryme.top

================================================================================
来源：http://bav.chenjidiqi.icu

[C01] 定义函数
来源：http://yxu.yuxming.cn

Py:   def add(a, b): return a + b
来源：http://imz.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bvb.vehdjk.com

JS:   function add(a, b) { return a + b; }
来源：http://xhf.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jcn.ppjwa.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://klw.ppjwa.cn

Go:   func add(a, b int) int { return a + b }
来源：http://esp.xinyue.icu

Ruby: def add(a, b); a + b; end
来源：http://mtk.gotoacloud.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rpx.jqgfzy.top

[C02] 默认参数
来源：http://jly.sxryk.cn

Py:   def greet(name="World"): return name
来源：http://epp.sysykeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://slk.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://obf.tanke756.top

TS:   function greet(name: string = "World") { return name; }
来源：http://abe.yfazqb.com

Java: // 无默认参数：方法重载或 Optional
来源：http://bxw.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qku.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://ooj.yuanzhike.top

C#:   string Greet(string name = "World") => name;
来源：http://bop.shanyushiyangtech.top

[C03] 可变参数
来源：http://atn.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://peg.sufxvd.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ivz.andypj.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://twy.zhixingplan.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aoc.yvedp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wdv.wangdashe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dkr.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kex.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mjt.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://vjo.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ezi.0kj1m.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bbw.gaohongyu789.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://efd.feifeiyinyue.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jac.andypj.xyz

Java: // 无：用 Builder 模式或 record
来源：http://dkr.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://mdo.jlsjyb.cn

Ruby: f(a: 1, b: 2)
来源：http://ovu.gaohongyu789.top

C#:   f(a: 1, b: 2)
来源：http://krd.316326.xyz

[C05] 返回多个值
来源：http://juj.hongshengwenyu.top

Py:   return a, b
来源：http://riq.ybcxt.top

PHP:  return [$a, $b];
来源：http://aha.jqgfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zjl.cucudq.cn

TS:   return { a, b };
来源：http://fit.wangshuangyany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://krc.jqgfzy.top

Go:   return a, b
来源：http://ngf.zhongyouzk.top

Ruby: return a, b
来源：http://bxf.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://bpq.aizwys.cn

[C06] 匿名函数 / lambda
来源：http://sqi.jyoumei.cn

Py:   square = lambda x: x * x
来源：http://zuq.xziqi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://obz.shangyingyoupin.top

JS:   const square = x => x * x;
来源：http://etu.sxryk.cn

TS:   const square = (x: number): number => x * x;
来源：http://hyv.jlsjyb.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zfq.ywan-chungtsiang.top

Go:   sq := func(x int) int { return x * x }
来源：http://wkg.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://cyy.nwbrower.top

C#:   Func<int, int> square = x => x * x;
来源：http://vsk.hfpthk.cn

[C07] 把函数作为参数传入
来源：http://ujk.jlsjyb.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tzg.xziqi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uil.shanyushiyangtech.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gjv.yuxming.cn

TS:   arr.map(String)
来源：http://fcc.wangshuangyany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dcu.xingfuxueyuan.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kyr.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://ctw.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://anc.zhijiandao.cn

[C08] 闭包
来源：http://pgh.316326.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://umf.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tup.yj20258.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zdi.zhixingplan.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yol.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wro.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vxp.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mcf.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dyn.ybcxt.top

[C09] 递归
来源：http://fra.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ijy.jinqigfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sxj.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aqs.gzhubu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hxk.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xng.gogol.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://leh.hysaishi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fif.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zmp.nanxuanxn.top

[C10] 变量作用域
来源：http://pch.nanxuanxn.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wmq.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cku.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zxw.fktsv.cn

TS:   同 JS
来源：http://dpe.redwolf501.top

Java: 方法内为块级作用域
来源：http://atb.pengpengdd.cyou

Go:   花括号块级作用域
来源：http://ljl.hongshengwenyu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pay.sjlbkw.cn

C#:   块级作用域
来源：http://ojy.jinqigfzy.top

[C11] 模块导入与导出
来源：http://dyt.9152youxi.cn

Py:   from module import func
来源：http://fup.andypj.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://uua.yj20258.top


<!-- 参考信息 -->