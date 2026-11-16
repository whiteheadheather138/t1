代发 wailian999

[A22] 获取字符串长度
来源：http://igc.hcnkem.com

Py:   len(s)
来源：http://ecv.hesvh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oty.nwbrower.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://avl.gaohongyu789.top

TS:   s.length
来源：http://jxt.daria6918.cn

Java: s.length()
来源：http://jch.zhoulong.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wku.jyoumei.cn

Ruby: s.length
来源：http://ats.pycfn.com

C#:   s.Length
来源：http://sfl.bjfxy.top

[A23] 大小写转换
来源：http://gxx.yanxiufei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pgz.andypj.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qgi.pengpengdd.cyou

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fpy.yuxming.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ryq.nanxuanxn.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qvx.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qtu.daxiang520.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zmq.zhiwuduotai.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pxs.xziqi.cn

[A24] 去除首尾空白
来源：http://wac.zdqjudy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ghd.yueranfly.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qnv.feifeiyinyue.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uwf.hywenlv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cry.vqdsnc.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://brl.9152youxi.cn

Go:   strings.TrimSpace(s)
来源：http://cpn.quarkkingdee.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dkm.tarul.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://knk.tarul.cn

[A25] 字符串比较
来源：http://vbh.fanxiaobao.xyz

Py:   s1 == s2; s1 != s2
来源：http://mvn.nwbrower.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xcs.meibo888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nhg.c1oappe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://evv.sxryk.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tym.ywan-chungtsiang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vuy.xziqi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dcg.fehbvm.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rfu.zhixingplan.top

[A26] 类型转换总览
来源：http://wsb.yanxiufei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ctb.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ekl.316326.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aun.quarkkingdee.top

TS:   Number() String() Boolean() x as number
来源：http://onn.iojbl.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cot.pengpengdd.cyou

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wcz.zhijiandao.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fcx.yongpay.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mqa.svipenyu.cn

================================================================================
来源：http://lvc.shanyushiyangkeji.top

B. 流程控制
来源：http://nni.zdqjudy.top

================================================================================
来源：http://aeh.pengpengdd.cyou

[B01] 条件判断 if / else
来源：http://bxw.cqqwz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aeh.andypj.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fjc.zhixingplan.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pfj.nwbrower.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yom.guannengcc.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cmo.shanyushiyangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jza.gotoacloud.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yqd.shangyingyoupin.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iqp.andypj.xyz

[B02] 多分支 else if / elif
来源：http://fsf.shanyushiyangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dsa.sufxvd.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fvp.havefunace.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zca.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fev.shanyushiyangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oql.jinghuilouyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tsc.shangyingyoupin.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pfp.daria6918.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wum.nwbrower.top

[B03] switch / match / case
来源：http://mbu.ydjk.org.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xgo.zhongyouzk.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oie.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nmt.hnqzz.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rhb.fehbvm.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fcw.jianghu66.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tmm.gaohongyu789.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mok.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mdj.zdbjq.cn

[B04] for 计数循环
来源：http://fcg.bbcook.cn

Py:   for i in range(10): print(i)
来源：http://pkv.haohaochexian.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bja.dianchejie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vya.xylfe.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lqz.zhixingplan.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blz.zdbjq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ebs.yj20258888.top

Ruby: 10.times { |i| puts i }
来源：http://agb.guowangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fje.xinyue.icu

[B05] 遍历数组 / 列表
来源：http://dhs.fanxiaobao.xyz

Py:   for item in arr: print(item)
来源：http://iha.shanyushiyangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cof.fengsongda.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cbu.xingfuxueyuan.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://bac.iojbl.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ukl.ppjwa.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yrb.zycfv.cn

Ruby: arr.each { |item| puts item }
来源：http://jvk.yuanzhike.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cwa.sjlbkw.cn

[B06] 遍历字典 / 对象
来源：http://qlk.nwbrower.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xjf.fehbvm.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jkh.fanxiaobao.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kta.gotoacloud.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://veh.cheryme.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://soo.cucudq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://giy.52xcode.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fli.zdbjq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zwu.9152youxi.cn

[B07] while 循环
来源：http://ebl.jiagoushi.top

Py:   while i < 10: i += 1
来源：http://ynu.guannengcc.top

PHP:  while ($i < 10) { $i++; }
来源：http://ryv.bbcook.cn

JS:   while (i < 10) { i++; }
来源：http://irp.shanyushiyangkeji.top

TS:   while (i < 10) { i++; }
来源：http://ica.cashguo.top

Java: while (i < 10) { i++; }
来源：http://zgd.ivvv.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ite.zhongyouzk.top

Ruby: while i < 10; i += 1; end
来源：http://tmg.gotoacloud.top

C#:   while (i < 10) { i++; }
来源：http://znk.tanke756.top

[B08] do-while（至少执行一次）
来源：http://qei.ybcxt.top

Py:   # 无 do-while：用 while True + break
来源：http://psv.ctjpmb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://oxx.hysaishi.cn

JS:   do { i++; } while (i < 10);
来源：http://ida.guowangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://xth.zhijiandao.cn

Java: do { i++; } while (i < 10);
来源：http://znv.svipenyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ekl.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ppa.meibo888.top

C#:   do { i++; } while (i < 10);
来源：http://aft.jinqigfzy.top

[B09] break 与 continue
来源：http://urw.jqgufenzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pus.aibaodan.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oth.yj20258888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ink.yfazqb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fvn.zhongyouzk.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://app.svipenyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jtl.quarkkingdee.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vqb.daria6918.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zoo.fengsongda.top

[B10] 遍历同时拿索引
来源：http://xrk.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ypm.hesvh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ilr.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zrg.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ehn.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hff.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ker.nanxinkj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tom.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://owz.hcnkem.com

[B11] 生成数字序列 / 区间
来源：http://rhk.havefunace.top

Py:   list(range(0, 10, 2))
来源：http://tqf.aizwys.cn

PHP:  range(0, 10, 2);
来源：http://psl.ehwqpu.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://woi.uphjek.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://duh.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mdn.gotoacloud.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://exx.epnwcf.com

Ruby: (0...10).step(2).to_a
来源：http://ghn.zhijiandao.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://inw.gzhubu.top

[B12] 跳出多层循环
来源：http://krm.aizwys.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://otc.zhiwuduotai.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hyy.hesvh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yah.jinqigfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oqk.aibaodan.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pmm.zhengqikj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vya.yongpay.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tpu.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ebu.shangyingyoupin.top

[B13] 判断是否为数字
来源：http://pir.yuxming.cn

Py:   isinstance(x, (int, float))
来源：http://vek.shanyushiyangkeji.top

PHP:  is_numeric($x)
来源：http://lol.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jyw.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uhl.zdbjq.cn

Java: x instanceof Number
来源：http://mcy.mhx1999.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://obh.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://pte.yonumen.top

C#:   x is int or double or decimal
来源：http://dmy.nanxuanxn.top

[B14] 判断值是否在集合内
来源：http://wgl.xuanzx.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qic.iojbl.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qoy.shuidangran.top

JS:   [1, 2, 3].includes(x)
来源：http://wjj.gotoacloud.top

TS:   [1, 2, 3].includes(x)
来源：http://vvz.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://orf.yuxming.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tyq.9152youxi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hyq.xinyue.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://led.0kj1m.cn

[B15] 布尔运算与取反
来源：http://dur.aizwys.cn

Py:   a and b or not c
来源：http://fde.wangshuangyany.cn

PHP:  $a && $b || !$c
来源：http://qau.ywan-chungtsiang.top

JS:   a && b || !c
来源：http://gpt.jinghuilouyu.cn

TS:   a && b || !c
来源：http://xof.zhongyouzk.top

Java: a && b || !c
来源：http://kzz.snrcjt.cn

Go:   a && b || !c
来源：http://bua.havefunace.top

Ruby: a && b || !c
来源：http://iis.gaohongyu789.top

C#:   a && b || !c
来源：http://ggp.zhiwuduotai.top

[B16] 卫语句：不满足条件提前返回
来源：http://jzi.chenjidiqi.icu

Py:   if not data: return
来源：http://ttb.vehdjk.com

PHP:  if (!$data) { return; }
来源：http://zrw.hfpthk.cn

JS:   if (!data) return;
来源：http://coh.chenlongwang.top

TS:   if (!data) return;
来源：http://rzk.52xcode.cn

Java: if (data == null) return;
来源：http://tdx.hammf.cn

Go:   if data == nil { return }
来源：http://ton.cheryme.top

Ruby: return if data.nil?
来源：http://aii.hnqzz.top

C#:   if (data == null) return;
来源：http://gto.dashuyun.cn

================================================================================
来源：http://ysz.cucudq.cn

C. 函数与作用域
来源：http://atz.jiagoushi.top

================================================================================
来源：http://wmj.daxiang520.top

[C01] 定义函数
来源：http://xwh.jqgufenzy.top

Py:   def add(a, b): return a + b
来源：http://zcx.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bal.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://kpe.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jkw.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gdm.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://clt.meibo888.top

Ruby: def add(a, b); a + b; end
来源：http://xcw.sufxvd.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://riu.ydzc1.top

[C02] 默认参数
来源：http://ttd.quarkkingdee.top

Py:   def greet(name="World"): return name
来源：http://udo.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://uxf.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://yfd.jiagoushi.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lmm.shzxlz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://odr.hnxiangtu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fph.hysaishi.cn

Ruby: def greet(name = "World") = name
来源：http://guo.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://umr.yonumen.top

[C03] 可变参数
来源：http://lvr.zdbjq.cn

Py:   def total(*args): return sum(args)
来源：http://woe.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wsf.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dov.quarkkingdee.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://anw.sweek.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tbe.hywenlv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eyn.hnxiangtu.top

Ruby: def total(*nums); nums.sum; end
来源：http://kel.xylfe.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dez.c1oappe.top

[C04] 命名参数 / 关键字参数
来源：http://ixv.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ytw.zhoulong.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ldk.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lob.jqgfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kzq.haohaochexian.top

Java: // 无：用 Builder 模式或 record
来源：http://qso.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://ssq.jinghuilouyu.cn

Ruby: f(a: 1, b: 2)
来源：http://vgo.guowangkeji.top

C#:   f(a: 1, b: 2)
来源：http://ndd.0kj1m.cn

[C05] 返回多个值
来源：http://hwg.316326.xyz

Py:   return a, b
来源：http://jpr.snrcjt.cn

PHP:  return [$a, $b];
来源：http://fqe.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://urd.yj202588.top

TS:   return { a, b };
来源：http://vdu.quarkkingdee.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pnj.yangfankeji.com

Go:   return a, b
来源：http://zcq.hesvh.cn

Ruby: return a, b
来源：http://nwv.daxiang520.top

C#:   return (a, b);              // ValueTuple
来源：http://edc.c1oappe.top

[C06] 匿名函数 / lambda
来源：http://cow.316326.xyz

Py:   square = lambda x: x * x
来源：http://zpi.smart0.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://uhh.feifeiyinyue.top

JS:   const square = x => x * x;
来源：http://iek.ivvv.top

TS:   const square = (x: number): number => x * x;
来源：http://djn.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gqh.gzhubu.top

Go:   sq := func(x int) int { return x * x }
来源：http://lls.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://hdl.zhijiandao.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lad.andypj.xyz

[C07] 把函数作为参数传入
来源：http://gul.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mwo.aibaodan.cn

PHP:  array_map("strtoupper", $arr);
来源：http://klw.0kj1m.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rzt.jinqigufen.top

TS:   arr.map(String)
来源：http://dkl.316326.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rjd.sjlbkw.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://smm.ydjk.org.cn

Ruby: arr.map(&:upcase)
来源：http://cfi.kuanghao11.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uji.sweek.top

[C08] 闭包
来源：http://kmq.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hrk.tarul.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yji.chenzaomai.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ajp.gotoacloud.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vva.hywenlv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tjl.ppjwa.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hjc.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wmq.cqqwz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mua.hnqzz.top

[C09] 递归
来源：http://shh.epnwcf.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gdp.yvedp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qwt.shangyingyoupin.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bof.havefunace.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jux.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cdd.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yzj.ydjk.org.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://awn.daxiang520.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ewt.hysaishi.cn

[C10] 变量作用域
来源：http://kld.chenzaomai.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wsn.shuidangran.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dgn.tanke756.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ktt.xziqi.cn

TS:   同 JS
来源：http://izi.yfazqb.com

Java: 方法内为块级作用域
来源：http://hon.ppjwa.cn

Go:   花括号块级作用域
来源：http://avs.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xbm.bjfxy.top

C#:   块级作用域
来源：http://nhh.yfazqb.com

[C11] 模块导入与导出
来源：http://hzp.zhoulong.xyz

Py:   from module import func
来源：http://cha.gogol.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://smb.yvedp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zpj.shangyingyoupin.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zuh.ppjwa.cn

Java: import java.util.List;
来源：http://ixv.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zdx.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://snk.cucudq.cn

C#:   using System.Text;
来源：http://qqz.mhx1999.top

[C12] 立即执行函数 IIFE
来源：http://txj.sysykeji.top

Py:   (lambda: print("run"))()
来源：http://zlv.fehbvm.com

PHP:  (function () { echo "run"; })();
来源：http://fxs.jqgufenzy.top

JS:   (() => { console.log("run"); })();
来源：http://pnk.zhaomingkeji.xyz

TS:   (() => { console.log("run"); })();
来源：http://itp.xziqi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hmd.tian-w.cn


<!-- 参考信息 -->