代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uax.zhengqikj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vrb.pengpengdd.cyou

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tog.redwolf501.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://udh.0kj1m.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://raz.ehwqpu.com

C#:   s.ToUpper(); s.ToLower()
来源：http://brb.daxiang520.top

[A24] 去除首尾空白
来源：http://mjv.shanyushiyangtech.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://avl.zhijiandao.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gwl.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gss.svipenyu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aue.fzhhl.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nvp.c1oappe.top

Go:   strings.TrimSpace(s)
来源：http://enn.jinqigfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zpa.jinqigufen.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cnt.gogol.net.cn

[A25] 字符串比较
来源：http://mhx.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://dhy.zdbjq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cvc.iojbl.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wyh.hcnkem.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lzs.gzhubu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dzl.52xcode.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://weu.hfpthk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://icd.jiagoushi.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lyg.ydzc1.top

[A26] 类型转换总览
来源：http://fho.ctjpmb.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hjh.sufxvd.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://igl.yuanzhike.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gfi.zhixingplan.top

TS:   Number() String() Boolean() x as number
来源：http://fip.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yud.hysaishi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ddk.kuanghao11.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fxp.hfpthk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bte.jianghu66.top

================================================================================
来源：http://cln.snrcjt.cn

B. 流程控制
来源：http://vvi.gogol.net.cn

================================================================================
来源：http://tdt.uphjek.com

[B01] 条件判断 if / else
来源：http://pti.ybcxt.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zco.ivvv.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fsz.dianchejie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gat.bjfxy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gfe.nanxinkj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ptf.xingfuxueyuan.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vyt.snrcjt.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://axc.yfazqb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qdq.wangshuangyany.cn

[B02] 多分支 else if / elif
来源：http://ptx.0kj1m.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://slr.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mwf.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cdn.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gds.ehwqpu.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lgg.xingfuxueyuan.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lty.tarul.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://how.yj202588.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lef.zhijiandao.cn

[B03] switch / match / case
来源：http://vkb.xinyue.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hbv.fktsv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://thm.jlsjyb.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xbl.yongpay.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dgn.xuetiantiany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ese.ppjwa.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bpf.jlsjyb.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jjj.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ruy.nanxuanxn.top

[B04] for 计数循环
来源：http://fjl.zhijiandao.cn

Py:   for i in range(10): print(i)
来源：http://kgb.yongpay.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fni.9152youxi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gfw.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lnz.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gmm.ydzc1.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://epz.jlsjyb.cn

Ruby: 10.times { |i| puts i }
来源：http://mga.jiagoushi.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ckf.sweek.top

[B05] 遍历数组 / 列表
来源：http://vjd.hysaishi.cn

Py:   for item in arr: print(item)
来源：http://ehk.epnwcf.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bak.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vrp.meibo888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vpa.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ezk.jlsjyb.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://afu.aibaodan.cn

Ruby: arr.each { |item| puts item }
来源：http://dlh.yfazqb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hfk.birdmap.top

[B06] 遍历字典 / 对象
来源：http://nki.haohaochexian.top

Py:   for k, v in d.items(): print(k, v)
来源：http://iyt.yangfankeji.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rko.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qdq.xinyue.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cgs.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xxs.xylfe.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xuz.nanxinkj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pco.jinghuilouyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://szr.fengsongda.top

[B07] while 循环
来源：http://ydi.xinyue.icu

Py:   while i < 10: i += 1
来源：http://yjm.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rop.cheryme.top

JS:   while (i < 10) { i++; }
来源：http://tev.daxiang520.top

TS:   while (i < 10) { i++; }
来源：http://mbf.chenzaomai.com

Java: while (i < 10) { i++; }
来源：http://uqh.bjfxy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://krq.hesvh.cn

Ruby: while i < 10; i += 1; end
来源：http://vmz.zycfv.cn

C#:   while (i < 10) { i++; }
来源：http://dcm.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://urq.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://tzg.ctjpmb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://wlq.shanyushiyangtech.top

JS:   do { i++; } while (i < 10);
来源：http://mdj.yj20258.top

TS:   do { i++; } while (i < 10);
来源：http://lgd.chenzaomai.com

Java: do { i++; } while (i < 10);
来源：http://cxv.hywenlv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iyq.daxiang520.top

Ruby: begin; i += 1; end while i < 10
来源：http://gub.yangfankeji.com

C#:   do { i++; } while (i < 10);
来源：http://vji.yangfankeji.com

[B09] break 与 continue
来源：http://vgw.wangshuangyany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://msk.c1oappe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pto.jinyuanbaomall.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lhk.daxiang520.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nvt.hnxiangtu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vxj.sxryk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kwf.xuetiantiany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vdm.hysaishi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hai.pengpengdd.cyou

[B10] 遍历同时拿索引
来源：http://eaj.zhaomingkeji.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jlm.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ene.andypj.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bcc.yonumen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://enm.xuetiantiany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ria.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pki.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cpi.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yzo.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://rqs.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://nqf.cashguo.top

PHP:  range(0, 10, 2);
来源：http://uos.guannengcc.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mxy.ydjk.org.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://guo.yj20258.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kun.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ejh.yj202588.top

Ruby: (0...10).step(2).to_a
来源：http://qnc.bbcook.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xna.yongpay.top

[B12] 跳出多层循环
来源：http://cqt.havefunace.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://oqu.shangyingyoupin.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hrk.daria6918.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hbv.hammf.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xmz.wangdashe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fxa.gogol.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yyh.yfazqb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tib.hysaishi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://psz.haohaochexian.top

[B13] 判断是否为数字
来源：http://lti.tarul.cn

Py:   isinstance(x, (int, float))
来源：http://whb.hysaishi.cn

PHP:  is_numeric($x)
来源：http://xix.dianchejie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sin.yuanzhike.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ogi.52xcode.cn

Java: x instanceof Number
来源：http://ipl.jlsjyb.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pez.jinghuilouyu.cn

Ruby: x.is_a?(Numeric)
来源：http://zfw.gotoacloud.top

C#:   x is int or double or decimal
来源：http://zvn.fengsongda.top

[B14] 判断值是否在集合内
来源：http://ifp.nanxuanxn.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gmm.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mot.zdqjudy.top

JS:   [1, 2, 3].includes(x)
来源：http://ovr.yfazqb.com

TS:   [1, 2, 3].includes(x)
来源：http://bqd.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bsj.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ngq.quarkkingdee.top

Ruby: [1, 2, 3].include?(x)
来源：http://szo.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qxc.xuanzx.com

[B15] 布尔运算与取反
来源：http://dfx.ydjk.org.cn

Py:   a and b or not c
来源：http://mnj.fzhhl.top

PHP:  $a && $b || !$c
来源：http://otl.snrcjt.cn

JS:   a && b || !c
来源：http://nzn.epnwcf.com

TS:   a && b || !c
来源：http://nhd.hongshengwenyu.top

Java: a && b || !c
来源：http://lkb.hcnkem.com

Go:   a && b || !c
来源：http://iub.snrcjt.cn

Ruby: a && b || !c
来源：http://kns.chenzaomai.com

C#:   a && b || !c
来源：http://mvu.yvedp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bce.chenlongwang.top

Py:   if not data: return
来源：http://blq.havefunace.top

PHP:  if (!$data) { return; }
来源：http://uia.9152youxi.cn

JS:   if (!data) return;
来源：http://dwi.fzhhl.top

TS:   if (!data) return;
来源：http://klh.wangshuangyany.cn

Java: if (data == null) return;
来源：http://ili.gogol.net.cn

Go:   if data == nil { return }
来源：http://rvj.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://kxh.uphjek.com

C#:   if (data == null) return;
来源：http://fdi.guannengcc.top

================================================================================
来源：http://zfd.ppjwa.cn

C. 函数与作用域
来源：http://gga.quarkkingdee.top

================================================================================
来源：http://dzq.yanxiufei.cn

[C01] 定义函数
来源：http://zik.jinghuilouyu.cn

Py:   def add(a, b): return a + b
来源：http://smw.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pbe.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://mfp.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yhy.xylfe.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hjt.yj20258.top

Go:   func add(a, b int) int { return a + b }
来源：http://pbi.hcnkem.com

Ruby: def add(a, b); a + b; end
来源：http://xhx.yueranfly.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dzi.mhx1999.top

[C02] 默认参数
来源：http://rqt.yanxiufei.cn

Py:   def greet(name="World"): return name
来源：http://dkv.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://szl.ppjwa.cn

JS:   function greet(name = "World") { return name; }
来源：http://lgn.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jsy.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wmc.shzxlz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gfz.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://edb.jinyuanbaomall.cn

C#:   string Greet(string name = "World") => name;
来源：http://smv.wangshuangyany.cn

[C03] 可变参数
来源：http://zei.hesvh.cn

Py:   def total(*args): return sum(args)
来源：http://tzo.zhengqikj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://csp.chenzaomai.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yvl.xylfe.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zuz.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vso.fzhhl.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kam.pycfn.com

Ruby: def total(*nums); nums.sum; end
来源：http://rko.guowangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eke.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://yeh.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://grg.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://twn.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://otl.nanxuanxn.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ayk.ctjpmb.com

Java: // 无：用 Builder 模式或 record
来源：http://aof.shuidangran.top

Go:   // 无：用配置结构体参数
来源：http://lqy.shanyushiyangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://frc.jyoumei.cn

C#:   f(a: 1, b: 2)
来源：http://ejk.jinqigfzy.top

[C05] 返回多个值
来源：http://wee.guannengcc.top

Py:   return a, b
来源：http://vog.jqgfzy.top

PHP:  return [$a, $b];
来源：http://dnw.shanyushiyangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cer.52xcode.cn

TS:   return { a, b };
来源：http://eqz.xingfuxueyuan.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sfq.xingfuxueyuan.xyz

Go:   return a, b
来源：http://cmw.daria6918.cn

Ruby: return a, b
来源：http://mmq.jiagoushi.top

C#:   return (a, b);              // ValueTuple
来源：http://gci.ybcxt.top

[C06] 匿名函数 / lambda
来源：http://dxc.yongpay.top

Py:   square = lambda x: x * x
来源：http://bjj.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://git.kuanghao11.cn

JS:   const square = x => x * x;
来源：http://aka.jqgfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://kuc.guannengcc.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://isb.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://lko.tianlin.xyz

Ruby: square = ->(x) { x * x }
来源：http://psl.smart0.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://kjh.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://dnk.shanyushiyangtech.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xwq.jqgufenzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://umo.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rgx.vqdsnc.cn

TS:   arr.map(String)
来源：http://iym.mhx1999.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://brd.jyoumei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fym.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://whq.jinqigfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://khl.xylfe.cn

[C08] 闭包
来源：http://pnr.hongshengwenyu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vlq.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pxf.cashguo.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uwk.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wwq.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nrm.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iff.yvedp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aqn.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qzx.uphjek.com

[C09] 递归
来源：http://ron.xuanzx.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lcv.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xln.52xcode.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://udq.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vzs.fehbvm.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rip.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lfl.cheryme.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zgk.aibaodan.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ilg.aizwys.cn

[C10] 变量作用域
来源：http://xlg.hammf.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://akv.birdmap.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tlb.yuanzhike.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mwf.sufxvd.cn

TS:   同 JS
来源：http://nyk.shuidangran.top

Java: 方法内为块级作用域
来源：http://vpy.ctjpmb.com

Go:   花括号块级作用域
来源：http://nhn.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dwi.pycfn.com

C#:   块级作用域
来源：http://akl.epnwcf.com

[C11] 模块导入与导出
来源：http://wim.chenlongwang.top

Py:   from module import func
来源：http://ice.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vsg.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hpx.zhiwuduotai.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uif.cdnleiting.top

Java: import java.util.List;
来源：http://fsf.sufxvd.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://svm.zdqjudy.top

Ruby: require "json"; require_relative "./util"
来源：http://krw.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://dii.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://zxr.chenjidiqi.icu

Py:   (lambda: print("run"))()
来源：http://dvk.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://qpe.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://sta.fktsv.cn

TS:   (() => { console.log("run"); })();
来源：http://lxo.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fkk.hesvh.cn

Go:   func() { fmt.Println("run") }()
来源：http://vgk.fengsongda.top

Ruby: -> { puts "run" }.call
来源：http://dkn.birdmap.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zii.tian-w.cn

[C13] 类型声明 / 类型注解
来源：http://txt.hesvh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hjo.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sgn.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eim.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://buk.cqqwz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://otb.gogol.net.cn

Go:   func add(a, b int) int
来源：http://jlo.sufxvd.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kju.chenjidiqi.icu

C#:   int Add(int a, int b) => a + b;
来源：http://quz.shanyushiyangtech.top


<!-- 参考信息 -->