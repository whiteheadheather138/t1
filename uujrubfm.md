代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://sbw.gogol.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bxn.guannengcc.top

JS:   (3.14159).toFixed(2)
来源：http://kcm.yj20258.top

TS:   (3.14159).toFixed(2)
来源：http://dmn.gzhubu.top

Java: String.format("%.2f", 3.14159)
来源：http://wcw.tarul.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rje.yonumen.top

Ruby: format("%.2f", 3.14159)
来源：http://dzk.nwbrower.top

C#:   3.14159.ToString("F2")
来源：http://czg.yj20258.top

[A22] 获取字符串长度
来源：http://iqd.yongpay.top

Py:   len(s)
来源：http://exc.meibo888.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ilf.jqgfzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rgr.sjlbkw.cn

TS:   s.length
来源：http://uff.xylfe.cn

Java: s.length()
来源：http://uqv.vqdsnc.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ofe.xinyue.icu

Ruby: s.length
来源：http://tsm.ivvv.top

C#:   s.Length
来源：http://jvy.jiagoushi.top

[A23] 大小写转换
来源：http://hol.fktsv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://llv.chenjidiqi.icu

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rdf.tarul.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dqp.cqqwz.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rnh.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ufe.jinqigfzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vha.tianlin.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dkk.sysykeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ezp.daria6918.cn

[A24] 去除首尾空白
来源：http://feb.hnxiangtu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fvm.ctjpmb.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dtt.smart0.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://btc.wangdashe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://odb.zhaomingkeji.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eml.jqgfzy.top

Go:   strings.TrimSpace(s)
来源：http://ptt.hfpthk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vdd.uphjek.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mup.yonumen.top

[A25] 字符串比较
来源：http://fbc.cheryme.top

Py:   s1 == s2; s1 != s2
来源：http://czu.yvedp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://omk.epnwcf.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qbr.ppjwa.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vas.epnwcf.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ebs.ywan-chungtsiang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://klz.hysaishi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tev.daria6918.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fhn.wangdashe.top

[A26] 类型转换总览
来源：http://cth.ppjwa.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://npk.iojbl.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kru.dashuyun.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cxt.yvedp.cn

TS:   Number() String() Boolean() x as number
来源：http://pnu.c1oappe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uuz.cdnleiting.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sjx.gzhubu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cmq.zhijiandao.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xzz.tarul.cn

================================================================================
来源：http://aht.jiagoushi.top

B. 流程控制
来源：http://rzo.uphjek.com

================================================================================
来源：http://pml.haohaochexian.top

[B01] 条件判断 if / else
来源：http://tjk.dianchejie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ggu.fktsv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lfh.fktsv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ppl.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kir.jinghuilouyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jwz.mhx1999.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wot.wangshuangyany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hqq.zhengqikj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iqp.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://giq.yueranfly.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wxa.gogol.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hfo.jinqigufen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sqr.zhoulong.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pnl.fzhhl.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iui.zycfv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rwy.birdmap.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://czg.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eec.chenzaomai.com

[B03] switch / match / case
来源：http://ula.birdmap.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gil.ctjpmb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ttc.0kj1m.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kmv.daxiang520.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ysl.cashguo.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://txu.jqgufenzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bla.zhengqikj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rms.zhixingplan.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ymo.birdmap.top

[B04] for 计数循环
来源：http://ose.gzhubu.top

Py:   for i in range(10): print(i)
来源：http://thl.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aoc.redwolf501.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://skr.snrcjt.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ypj.smart0.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nim.kuanghao11.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rgf.shzxlz.cn

Ruby: 10.times { |i| puts i }
来源：http://vec.zhongyouzk.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gtm.jinqigfzy.top

[B05] 遍历数组 / 列表
来源：http://ujl.cqqwz.cn

Py:   for item in arr: print(item)
来源：http://ppz.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://icm.hammf.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yvi.pengpengdd.cyou

TS:   for (const item of arr) { console.log(item); }
来源：http://fjt.fktsv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dru.epnwcf.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cfd.yj20258888.top

Ruby: arr.each { |item| puts item }
来源：http://wbr.jiagoushi.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gds.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://axc.hnqzz.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rrl.fzhhl.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xzb.sufxvd.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://epl.chenjidiqi.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://urg.zhiwuduotai.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dsz.yfazqb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qlk.zhongyouzk.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://paw.wangdashe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dmb.yfazqb.com

[B07] while 循环
来源：http://zan.xuanzx.com

Py:   while i < 10: i += 1
来源：http://mcj.hysaishi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ymf.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://tuk.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://pai.hongshengwenyu.top

Java: while (i < 10) { i++; }
来源：http://xax.hesvh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yzu.jinyuanbaomall.cn

Ruby: while i < 10; i += 1; end
来源：http://pnm.guannengcc.top

C#:   while (i < 10) { i++; }
来源：http://osd.haohaochexian.top

[B08] do-while（至少执行一次）
来源：http://upm.zhoulong.xyz

Py:   # 无 do-while：用 while True + break
来源：http://llz.kuanghao11.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yny.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://awj.ppjwa.cn

TS:   do { i++; } while (i < 10);
来源：http://yrg.meibo888.top

Java: do { i++; } while (i < 10);
来源：http://gjn.ydzc1.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mje.vqdsnc.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ggh.zhoulong.xyz

C#:   do { i++; } while (i < 10);
来源：http://nfw.guannengcc.top

[B09] break 与 continue
来源：http://ndt.chenlongwang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zlf.svipenyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://els.guowangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ysi.andypj.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kcm.fehbvm.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oxy.yj202588.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kbz.gzhubu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jzk.yangfankeji.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tkz.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://plw.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ypg.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iuy.jyoumei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mlr.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://csy.hammf.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://suu.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qke.hfpthk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jyw.zhijiandao.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iie.snrcjt.cn

[B11] 生成数字序列 / 区间
来源：http://znq.yongpay.top

Py:   list(range(0, 10, 2))
来源：http://fyi.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://ujq.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iyp.ydjk.org.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xnm.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eqo.fengsongda.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vek.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://ydt.jiagoushi.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mos.guowangkeji.top

[B12] 跳出多层循环
来源：http://xtl.chenlongwang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hdg.yvedp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oqf.dashuyun.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kad.quarkkingdee.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hpy.dashuyun.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qpi.yuxming.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wcu.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yum.dashuyun.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hkj.iojbl.cn

[B13] 判断是否为数字
来源：http://vaf.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://yzl.cheryme.top

PHP:  is_numeric($x)
来源：http://ced.ybcxt.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dcy.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gim.yj20258888.top

Java: x instanceof Number
来源：http://czj.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dpy.yj202588.top

Ruby: x.is_a?(Numeric)
来源：http://jdy.iojbl.cn

C#:   x is int or double or decimal
来源：http://drh.jinyuanbaomall.cn

[B14] 判断值是否在集合内
来源：http://imr.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://etq.cdnleiting.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jjz.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://sht.svipenyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://umk.guannengcc.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wtf.andypj.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wlt.sjlbkw.cn

Ruby: [1, 2, 3].include?(x)
来源：http://edb.daxiang520.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xzz.316326.xyz

[B15] 布尔运算与取反
来源：http://jvw.yongpay.top

Py:   a and b or not c
来源：http://jgn.bjfxy.top

PHP:  $a && $b || !$c
来源：http://anx.sxryk.cn

JS:   a && b || !c
来源：http://nnn.shangyingyoupin.top

TS:   a && b || !c
来源：http://tls.wangshuangyany.cn

Java: a && b || !c
来源：http://ash.yj202588.top

Go:   a && b || !c
来源：http://gtj.dashuyun.cn

Ruby: a && b || !c
来源：http://ale.hesvh.cn

C#:   a && b || !c
来源：http://lmo.vqdsnc.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fjm.xylfe.cn

Py:   if not data: return
来源：http://xgs.svipenyu.cn

PHP:  if (!$data) { return; }
来源：http://zdv.fzhhl.top

JS:   if (!data) return;
来源：http://aao.svipenyu.cn

TS:   if (!data) return;
来源：http://ejy.hammf.cn

Java: if (data == null) return;
来源：http://idq.fehbvm.com

Go:   if data == nil { return }
来源：http://loq.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://egu.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://nzu.xziqi.cn

================================================================================
来源：http://acl.cucudq.cn

C. 函数与作用域
来源：http://glt.xuetiantiany.cn

================================================================================
来源：http://tbe.hnqzz.top

[C01] 定义函数
来源：http://ojv.9152youxi.cn

Py:   def add(a, b): return a + b
来源：http://rsx.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tkd.sjlbkw.cn

JS:   function add(a, b) { return a + b; }
来源：http://rna.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ytx.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qkh.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://sjn.yangfankeji.com

Ruby: def add(a, b); a + b; end
来源：http://uai.shanyushiyangtech.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dnu.yj202588.top

[C02] 默认参数
来源：http://xfy.pycfn.com

Py:   def greet(name="World"): return name
来源：http://oap.quarkkingdee.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hvk.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://tji.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yuh.shanyushiyangtech.top

Java: // 无默认参数：方法重载或 Optional
来源：http://maw.fktsv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://obi.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://iqk.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://dtj.jyoumei.cn

[C03] 可变参数
来源：http://fsk.quarkkingdee.top

Py:   def total(*args): return sum(args)
来源：http://czd.xingfuxueyuan.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ozg.yuanzhike.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jek.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mvq.shuidangran.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gsj.kuanghao11.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qxa.redwolf501.top

Ruby: def total(*nums); nums.sum; end
来源：http://zrf.sysykeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cgc.xylfe.cn

[C04] 命名参数 / 关键字参数
来源：http://dxk.aizwys.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qsl.cqqwz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wxm.cqqwz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ubz.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hwa.zhixingplan.top

Java: // 无：用 Builder 模式或 record
来源：http://grg.zdqjudy.top

Go:   // 无：用配置结构体参数
来源：http://fiw.bjfxy.top

Ruby: f(a: 1, b: 2)
来源：http://njk.ppjwa.cn

C#:   f(a: 1, b: 2)
来源：http://wlw.daria6918.cn

[C05] 返回多个值
来源：http://wyr.tanke756.top

Py:   return a, b
来源：http://fsk.chenzaomai.com

PHP:  return [$a, $b];
来源：http://ccq.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://cyj.dianchejie.cn

TS:   return { a, b };
来源：http://hyc.yj20258.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mjf.zdbjq.cn

Go:   return a, b
来源：http://ese.nanxinkj.top

Ruby: return a, b
来源：http://yje.shanyushiyangtech.top

C#:   return (a, b);              // ValueTuple
来源：http://bfq.bbcook.cn

[C06] 匿名函数 / lambda
来源：http://xwo.xylfe.cn

Py:   square = lambda x: x * x
来源：http://ttp.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ajk.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://msd.shzxlz.cn

TS:   const square = (x: number): number => x * x;
来源：http://qdd.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ufw.jianghu66.top

Go:   sq := func(x int) int { return x * x }
来源：http://ome.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://vqh.daria6918.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eeg.fzhhl.top

[C07] 把函数作为参数传入
来源：http://gsi.guannengcc.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qcs.jqgufenzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://lje.yj20258888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qpw.daria6918.cn

TS:   arr.map(String)
来源：http://emt.hammf.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tov.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lxf.xuanzx.com

Ruby: arr.map(&:upcase)
来源：http://tcz.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qgb.redwolf501.top

[C08] 闭包
来源：http://rro.zhongyouzk.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zsu.0kj1m.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iha.sjlbkw.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hkn.daria6918.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://daz.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ciy.dashuyun.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://azf.nwbrower.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xwt.aizwys.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qlh.zdbjq.cn

[C09] 递归
来源：http://lps.jiagoushi.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zgm.fehbvm.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bce.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qwf.jqgfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://stj.aizwys.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://twf.ydzc1.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://axi.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://awc.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xvd.zhoulong.xyz

[C10] 变量作用域
来源：http://wiv.shzxlz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pdy.xuetiantiany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bfb.0kj1m.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://voq.yj202588.top

TS:   同 JS
来源：http://hmm.nanxuanxn.top

Java: 方法内为块级作用域
来源：http://cta.ydjk.org.cn

Go:   花括号块级作用域
来源：http://enm.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dsj.ydzc1.top

C#:   块级作用域
来源：http://yxy.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://jya.meibo888.top

Py:   from module import func
来源：http://tmd.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://sjr.ywan-chungtsiang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yxm.fzhhl.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wil.fktsv.cn

Java: import java.util.List;
来源：http://iwj.quarkkingdee.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ddd.vehdjk.com


<!-- 参考信息 -->