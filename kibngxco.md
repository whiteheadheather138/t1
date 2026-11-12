代发 wailian999

TS:   s.length
来源：http://sfp.yonumen.top

Java: s.length()
来源：http://haq.haohaochexian.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wko.nanxuanxn.top

Ruby: s.length
来源：http://qcq.svipenyu.cn

C#:   s.Length
来源：http://gxb.yj20258.top

[A23] 大小写转换
来源：http://law.quarkkingdee.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pdx.yanxiufei.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kuo.jiagoushi.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eoi.jinyuanbaomall.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zxx.jinyuanbaomall.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eej.vehdjk.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tci.andypj.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zdo.xinyue.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://fun.hnxiangtu.top

[A24] 去除首尾空白
来源：http://vxw.guannengcc.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kmm.kuanghao11.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bew.52xcode.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jiw.jiagoushi.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nsh.cdnleiting.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vlc.nwbrower.top

Go:   strings.TrimSpace(s)
来源：http://kmm.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uji.yfazqb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lcg.9152youxi.cn

[A25] 字符串比较
来源：http://eoe.jqgufenzy.top

Py:   s1 == s2; s1 != s2
来源：http://fro.daxiang520.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://alt.yuxming.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pyn.vehdjk.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jkm.hnxiangtu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dhz.yvedp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vfc.dashuyun.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kwl.nanxuanxn.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fjg.tanke756.top

[A26] 类型转换总览
来源：http://uvm.sufxvd.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://thl.jyoumei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vhv.yj202588.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jfp.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://xrl.chenjidiqi.icu

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uoe.yj20258888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kwf.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://nus.guowangkeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mpi.daria6918.cn

================================================================================
来源：http://ncb.sxryk.cn

B. 流程控制
来源：http://egi.bbcook.cn

================================================================================
来源：http://fck.yvedp.cn

[B01] 条件判断 if / else
来源：http://arw.fengsongda.top

Py:   result = "正" if x > 0 else "非正"
来源：http://oev.zhoulong.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sqp.vqdsnc.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gyp.yj20258888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rts.hcnkem.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://ttr.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qfn.jianghu66.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cvt.chenlongwang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://twb.xuanzx.com

[B02] 多分支 else if / elif
来源：http://hbn.gzhubu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mtc.zhijiandao.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nao.zhoulong.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tya.shanyushiyangtech.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zmj.zhixingplan.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mla.chenzaomai.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yug.jqgfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zlf.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lxu.sxryk.cn

[B03] switch / match / case
来源：http://xrb.pycfn.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vjs.uphjek.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://owg.wangshuangyany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ulj.dianchejie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eip.tianlin.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mte.shuidangran.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yfs.fanxiaobao.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zoo.hnqzz.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lef.jinqigfzy.top

[B04] for 计数循环
来源：http://irb.wangshuangyany.cn

Py:   for i in range(10): print(i)
来源：http://gwz.fktsv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tdp.fanxiaobao.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bjh.dianchejie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zqh.zhiwuduotai.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pzp.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wfd.zdbjq.cn

Ruby: 10.times { |i| puts i }
来源：http://qyi.yuxming.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ovz.gzhubu.top

[B05] 遍历数组 / 列表
来源：http://fgm.zdqjudy.top

Py:   for item in arr: print(item)
来源：http://xdq.yvedp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bci.c1oappe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yfm.nwbrower.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fnw.jinghuilouyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vip.yueranfly.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eeh.hammf.cn

Ruby: arr.each { |item| puts item }
来源：http://pdq.kuanghao11.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ejf.uphjek.com

[B06] 遍历字典 / 对象
来源：http://pdj.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ctf.hongshengwenyu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yeb.svipenyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kjn.jiagoushi.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://quy.gaohongyu789.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ruj.52xcode.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jcg.ydjk.org.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kqt.hcnkem.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fwe.chenjidiqi.icu

[B07] while 循环
来源：http://oeb.ydzc1.top

Py:   while i < 10: i += 1
来源：http://epi.bbcook.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tfv.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://yjo.jinyuanbaomall.cn

TS:   while (i < 10) { i++; }
来源：http://kxn.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://xco.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cbb.xinyue.icu

Ruby: while i < 10; i += 1; end
来源：http://alf.ppjwa.cn

C#:   while (i < 10) { i++; }
来源：http://fpy.hongshengwenyu.top

[B08] do-while（至少执行一次）
来源：http://jum.fanxiaobao.xyz

Py:   # 无 do-while：用 while True + break
来源：http://qol.zhiwuduotai.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dee.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://dab.aizwys.cn

TS:   do { i++; } while (i < 10);
来源：http://wsy.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://sdx.dianchejie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wne.gzhubu.top

Ruby: begin; i += 1; end while i < 10
来源：http://pcj.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://exm.zhongyouzk.top

[B09] break 与 continue
来源：http://pal.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hfb.xuanzx.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mnf.tanke756.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tju.chenzaomai.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fog.52xcode.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lig.aizwys.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wum.quarkkingdee.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cvk.svipenyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xec.wangshuangyany.cn

[B10] 遍历同时拿索引
来源：http://yji.sysykeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vxv.bbcook.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://brq.shanyushiyangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yyy.smart0.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://puo.yuanzhike.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mzk.jinqigufen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aei.jyoumei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mpk.gzhubu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lvf.cdnleiting.top

[B11] 生成数字序列 / 区间
来源：http://yoy.nanxuanxn.top

Py:   list(range(0, 10, 2))
来源：http://bet.jinghuilouyu.cn

PHP:  range(0, 10, 2);
来源：http://puf.vehdjk.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lvg.fehbvm.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rtv.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tna.pycfn.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hkx.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://eao.dashuyun.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://smb.yongpay.top

[B12] 跳出多层循环
来源：http://jgu.shanyushiyangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kea.yongpay.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tgi.wangdashe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zbq.xylfe.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rcb.chenjidiqi.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wzc.zhaomingkeji.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ckk.yfazqb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xko.cheryme.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wrz.ydzc1.top

[B13] 判断是否为数字
来源：http://ius.quarkkingdee.top

Py:   isinstance(x, (int, float))
来源：http://xsy.dashuyun.cn

PHP:  is_numeric($x)
来源：http://mtp.pycfn.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ppq.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yyb.52xcode.cn

Java: x instanceof Number
来源：http://iuq.cqqwz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://huj.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://ejt.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://hwa.yanxiufei.cn

[B14] 判断值是否在集合内
来源：http://iom.hywenlv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rah.hcnkem.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wjs.vqdsnc.cn

JS:   [1, 2, 3].includes(x)
来源：http://wqu.shuidangran.top

TS:   [1, 2, 3].includes(x)
来源：http://dmy.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pmf.tianlin.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rxk.ctjpmb.com

Ruby: [1, 2, 3].include?(x)
来源：http://eeu.cheryme.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fto.chenlongwang.top

[B15] 布尔运算与取反
来源：http://web.cheryme.top

Py:   a and b or not c
来源：http://ioy.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://jvw.dashuyun.cn

JS:   a && b || !c
来源：http://hfw.tanke756.top

TS:   a && b || !c
来源：http://zxs.fanxiaobao.xyz

Java: a && b || !c
来源：http://xdy.tanke756.top

Go:   a && b || !c
来源：http://heh.shzxlz.cn

Ruby: a && b || !c
来源：http://gdy.zhaomingkeji.xyz

C#:   a && b || !c
来源：http://woy.mhx1999.top

[B16] 卫语句：不满足条件提前返回
来源：http://mbc.svipenyu.cn

Py:   if not data: return
来源：http://xsu.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://kjb.svipenyu.cn

JS:   if (!data) return;
来源：http://bvi.xuanzx.com

TS:   if (!data) return;
来源：http://yyy.fengsongda.top

Java: if (data == null) return;
来源：http://vys.jinghuilouyu.cn

Go:   if data == nil { return }
来源：http://jxc.xingfuxueyuan.xyz

Ruby: return if data.nil?
来源：http://bov.aizwys.cn

C#:   if (data == null) return;
来源：http://lzp.tianlin.xyz

================================================================================
来源：http://thd.ywan-chungtsiang.top

C. 函数与作用域
来源：http://ckj.ydjk.org.cn

================================================================================
来源：http://gvw.snrcjt.cn

[C01] 定义函数
来源：http://ktx.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://rtq.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cne.jqgfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://ghi.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ymy.ppjwa.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wab.ywan-chungtsiang.top

Go:   func add(a, b int) int { return a + b }
来源：http://gur.iojbl.cn

Ruby: def add(a, b); a + b; end
来源：http://jfe.hesvh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rsg.redwolf501.top

[C02] 默认参数
来源：http://smu.cucudq.cn

Py:   def greet(name="World"): return name
来源：http://gcj.yueranfly.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mhy.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://zqd.fktsv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yto.xuanzx.com

Java: // 无默认参数：方法重载或 Optional
来源：http://pyy.dianchejie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://elx.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://bds.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://ozn.xziqi.cn

[C03] 可变参数
来源：http://bji.ydjk.org.cn

Py:   def total(*args): return sum(args)
来源：http://htc.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mnn.hysaishi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://obu.xinyue.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sjl.fengsongda.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xlh.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uoc.fanxiaobao.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://azp.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aqf.yuanzhike.top

[C04] 命名参数 / 关键字参数
来源：http://wer.xuanzx.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://myb.52xcode.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ial.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://use.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://suq.dashuyun.cn

Java: // 无：用 Builder 模式或 record
来源：http://krb.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://zoc.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://fsp.sufxvd.cn

C#:   f(a: 1, b: 2)
来源：http://gur.nwbrower.top

[C05] 返回多个值
来源：http://axx.52xcode.cn

Py:   return a, b
来源：http://hms.hesvh.cn

PHP:  return [$a, $b];
来源：http://lkf.sjlbkw.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dqp.xziqi.cn

TS:   return { a, b };
来源：http://ugh.jinqigufen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dje.kuanghao11.cn

Go:   return a, b
来源：http://zjh.gotoacloud.top

Ruby: return a, b
来源：http://vfh.nanxuanxn.top

C#:   return (a, b);              // ValueTuple
来源：http://fsl.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://poy.xziqi.cn

Py:   square = lambda x: x * x
来源：http://bai.xylfe.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://leh.ydjk.org.cn

JS:   const square = x => x * x;
来源：http://lbq.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://tjk.kuanghao11.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ajc.zhixingplan.top

Go:   sq := func(x int) int { return x * x }
来源：http://teq.jinyuanbaomall.cn

Ruby: square = ->(x) { x * x }
来源：http://jlj.ywan-chungtsiang.top

C#:   Func<int, int> square = x => x * x;
来源：http://ito.jinyuanbaomall.cn

[C07] 把函数作为参数传入
来源：http://ccz.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fto.jinghuilouyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lbw.bbcook.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dlq.ppjwa.cn

TS:   arr.map(String)
来源：http://xba.jqgfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ffx.bbcook.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bwn.andypj.xyz

Ruby: arr.map(&:upcase)
来源：http://klq.gotoacloud.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ayc.yonumen.top

[C08] 闭包
来源：http://aot.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qgj.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xvw.gogol.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wql.aibaodan.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nhz.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qup.nanxuanxn.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qal.jinqigfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cyw.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fgp.jinghuilouyu.cn

[C09] 递归
来源：http://ndg.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rzt.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kdk.yfazqb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cwa.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ftb.jinqigfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rfh.chenjidiqi.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nsc.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xti.c1oappe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ved.hywenlv.cn

[C10] 变量作用域
来源：http://piz.shuidangran.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lpq.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://thi.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zov.kuanghao11.cn

TS:   同 JS
来源：http://ydk.iojbl.cn

Java: 方法内为块级作用域
来源：http://dcw.ywan-chungtsiang.top

Go:   花括号块级作用域
来源：http://rgl.jianghu66.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cpn.sjlbkw.cn

C#:   块级作用域
来源：http://wku.snrcjt.cn

[C11] 模块导入与导出
来源：http://zjk.xuanzx.com

Py:   from module import func
来源：http://uoo.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hfv.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://quc.redwolf501.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mln.cqqwz.cn

Java: import java.util.List;
来源：http://uux.yvedp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ifj.xingfuxueyuan.xyz

Ruby: require "json"; require_relative "./util"
来源：http://orh.cdnleiting.top

C#:   using System.Text;
来源：http://eqo.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://ipe.yongpay.top

Py:   (lambda: print("run"))()
来源：http://ehn.xuanzx.com

PHP:  (function () { echo "run"; })();
来源：http://eii.yonumen.top

JS:   (() => { console.log("run"); })();
来源：http://pil.zhiwuduotai.top

TS:   (() => { console.log("run"); })();
来源：http://tsy.zhiwuduotai.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dix.chenzaomai.com

Go:   func() { fmt.Println("run") }()
来源：http://cve.pycfn.com

Ruby: -> { puts "run" }.call
来源：http://puk.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zts.hongshengwenyu.top

[C13] 类型声明 / 类型注解
来源：http://opx.wangdashe.top


<!-- 参考信息 -->