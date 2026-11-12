代发 wailian999

[A22] 获取字符串长度
来源：http://hei.yueranfly.top

Py:   len(s)
来源：http://kfl.ehwqpu.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iuh.yvedp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pfd.yj20258.top

TS:   s.length
来源：http://wju.bbcook.cn

Java: s.length()
来源：http://ehj.jinqigufen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zyr.tanke756.top

Ruby: s.length
来源：http://ysz.guannengcc.top

C#:   s.Length
来源：http://ysz.jinqigfzy.top

[A23] 大小写转换
来源：http://grn.shzxlz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jry.yongpay.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gus.jianghu66.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bwi.52xcode.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fbb.bjfxy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ruz.bbcook.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pga.zhijiandao.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rmu.fengsongda.top

C#:   s.ToUpper(); s.ToLower()
来源：http://irc.hnqzz.top

[A24] 去除首尾空白
来源：http://znr.jiagoushi.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vcf.cqqwz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ncj.zhijiandao.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xat.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eac.hfpthk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://shr.shuidangran.top

Go:   strings.TrimSpace(s)
来源：http://tkz.gotoacloud.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hqs.zhaomingkeji.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lqg.9152youxi.cn

[A25] 字符串比较
来源：http://bqc.hcnkem.com

Py:   s1 == s2; s1 != s2
来源：http://jte.fktsv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ltx.yonumen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xzd.nanxinkj.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zxp.dianchejie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kiy.fehbvm.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://spy.jlsjyb.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nkr.birdmap.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://onr.316326.xyz

[A26] 类型转换总览
来源：http://nkg.feifeiyinyue.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://azn.xylfe.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zij.xuetiantiany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kdu.cdnleiting.top

TS:   Number() String() Boolean() x as number
来源：http://owi.cdnleiting.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mec.yangfankeji.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jzi.wangshuangyany.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://spn.jianghu66.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pcu.ydjk.org.cn

================================================================================
来源：http://hhv.svipenyu.cn

B. 流程控制
来源：http://zrq.fehbvm.com

================================================================================
来源：http://iws.yuanzhike.top

[B01] 条件判断 if / else
来源：http://wsk.ydzc1.top

Py:   result = "正" if x > 0 else "非正"
来源：http://scu.zhiwuduotai.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://edq.shangyingyoupin.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pxq.wangshuangyany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://upr.nanxuanxn.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ued.zhaomingkeji.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dnl.fzhhl.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hiz.yongpay.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ptg.birdmap.top

[B02] 多分支 else if / elif
来源：http://ony.gaohongyu789.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bfi.hfpthk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://msb.zycfv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://abg.jinghuilouyu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://grr.yj202588.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vmn.guowangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://int.uphjek.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://krb.snrcjt.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rou.meibo888.top

[B03] switch / match / case
来源：http://mgm.nanxuanxn.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fji.yueranfly.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cjf.yangfankeji.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oxz.ydjk.org.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fze.cqqwz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xee.ybcxt.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kyw.zhixingplan.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xpu.daria6918.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zmw.fzhhl.top

[B04] for 计数循环
来源：http://lih.xziqi.cn

Py:   for i in range(10): print(i)
来源：http://ugf.havefunace.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rbr.vqdsnc.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wro.jqgfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ile.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bos.hywenlv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qxn.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://gth.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zko.jlsjyb.cn

[B05] 遍历数组 / 列表
来源：http://vyg.epnwcf.com

Py:   for item in arr: print(item)
来源：http://imy.daxiang520.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xhk.nwbrower.top

JS:   for (const item of arr) { console.log(item); }
来源：http://lbl.yvedp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://svl.epnwcf.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://xwo.daxiang520.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bdl.sweek.top

Ruby: arr.each { |item| puts item }
来源：http://wng.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jew.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://fsk.jyoumei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ozp.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yeq.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fyy.guannengcc.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qjj.ctjpmb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sad.hfpthk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qso.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eaz.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cnu.hesvh.cn

[B07] while 循环
来源：http://hxk.xuanzx.com

Py:   while i < 10: i += 1
来源：http://nye.snrcjt.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lxv.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://tyu.yfazqb.com

TS:   while (i < 10) { i++; }
来源：http://tdm.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://rpi.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://prs.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://vvn.yvedp.cn

C#:   while (i < 10) { i++; }
来源：http://uso.vehdjk.com

[B08] do-while（至少执行一次）
来源：http://unl.zhixingplan.top

Py:   # 无 do-while：用 while True + break
来源：http://byb.uphjek.com

PHP:  do { $i++; } while ($i < 10);
来源：http://ljr.hnqzz.top

JS:   do { i++; } while (i < 10);
来源：http://fds.jyoumei.cn

TS:   do { i++; } while (i < 10);
来源：http://xas.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://hnd.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xrc.sufxvd.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yjs.zhongyouzk.top

C#:   do { i++; } while (i < 10);
来源：http://kcq.mhx1999.top

[B09] break 与 continue
来源：http://uby.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xnc.yonumen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tjz.xuanzx.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pjw.feifeiyinyue.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yar.jyoumei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hxp.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xop.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dic.uphjek.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xiv.havefunace.top

[B10] 遍历同时拿索引
来源：http://zyj.zhaomingkeji.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hzv.chenjidiqi.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lcb.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://khy.hnqzz.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rcp.tianlin.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ifc.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lgx.gaohongyu789.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hbp.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zwl.birdmap.top

[B11] 生成数字序列 / 区间
来源：http://rjm.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://tgt.zdqjudy.top

PHP:  range(0, 10, 2);
来源：http://awx.hfpthk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tyc.zdqjudy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wun.dashuyun.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qly.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xpv.xuanzx.com

Ruby: (0...10).step(2).to_a
来源：http://sfw.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iyj.yfazqb.com

[B12] 跳出多层循环
来源：http://wcg.wangdashe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hiq.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wsm.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gul.chenjidiqi.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jlm.hnxiangtu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nro.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://miq.ydjk.org.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hxb.fengsongda.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iso.smart0.xyz

[B13] 判断是否为数字
来源：http://pht.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://uqq.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://fvy.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://twl.sweek.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kwj.quarkkingdee.top

Java: x instanceof Number
来源：http://kmx.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lxw.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://suy.xinyue.icu

C#:   x is int or double or decimal
来源：http://jou.yvedp.cn

[B14] 判断值是否在集合内
来源：http://ite.xuetiantiany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tab.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ggz.hnqzz.top

JS:   [1, 2, 3].includes(x)
来源：http://mry.guannengcc.top

TS:   [1, 2, 3].includes(x)
来源：http://qiw.zdbjq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ala.c1oappe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hru.sjlbkw.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fuk.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xtm.shzxlz.cn

[B15] 布尔运算与取反
来源：http://qzm.ivvv.top

Py:   a and b or not c
来源：http://iwp.cdnleiting.top

PHP:  $a && $b || !$c
来源：http://rlj.vqdsnc.cn

JS:   a && b || !c
来源：http://kzo.uphjek.com

TS:   a && b || !c
来源：http://rzc.vqdsnc.cn

Java: a && b || !c
来源：http://ojv.316326.xyz

Go:   a && b || !c
来源：http://wva.andypj.xyz

Ruby: a && b || !c
来源：http://yir.c1oappe.top

C#:   a && b || !c
来源：http://qbf.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://cpj.sjlbkw.cn

Py:   if not data: return
来源：http://rjh.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://dap.vqdsnc.cn

JS:   if (!data) return;
来源：http://vqk.9152youxi.cn

TS:   if (!data) return;
来源：http://lrn.yongpay.top

Java: if (data == null) return;
来源：http://afs.ppjwa.cn

Go:   if data == nil { return }
来源：http://ohg.smart0.xyz

Ruby: return if data.nil?
来源：http://mql.yj20258888.top

C#:   if (data == null) return;
来源：http://bnh.vqdsnc.cn

================================================================================
来源：http://nxc.hcnkem.com

C. 函数与作用域
来源：http://uvy.jinghuilouyu.cn

================================================================================
来源：http://eqi.316326.xyz

[C01] 定义函数
来源：http://ktr.yanxiufei.cn

Py:   def add(a, b): return a + b
来源：http://oio.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://boc.gzhubu.top

JS:   function add(a, b) { return a + b; }
来源：http://kku.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://msy.yanxiufei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xji.xylfe.cn

Go:   func add(a, b int) int { return a + b }
来源：http://okp.zhengqikj.top

Ruby: def add(a, b); a + b; end
来源：http://zwm.yueranfly.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://azn.fehbvm.com

[C02] 默认参数
来源：http://hvg.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://qll.jqgfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lst.ywan-chungtsiang.top

JS:   function greet(name = "World") { return name; }
来源：http://sss.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hqu.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kic.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vfr.yuanzhike.top

Ruby: def greet(name = "World") = name
来源：http://fbw.kuanghao11.cn

C#:   string Greet(string name = "World") => name;
来源：http://xrk.nanxinkj.top

[C03] 可变参数
来源：http://tih.daria6918.cn

Py:   def total(*args): return sum(args)
来源：http://jpt.yuanzhike.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dpd.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mtn.wangdashe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zej.shuidangran.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://beb.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jch.sxryk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vnl.sxryk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rjm.shanyushiyangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://xbf.jyoumei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cup.sxryk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ivr.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fnw.feifeiyinyue.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wyi.aizwys.cn

Java: // 无：用 Builder 模式或 record
来源：http://eui.shanyushiyangtech.top

Go:   // 无：用配置结构体参数
来源：http://wzb.zhoulong.xyz

Ruby: f(a: 1, b: 2)
来源：http://ggf.cashguo.top

C#:   f(a: 1, b: 2)
来源：http://gsx.nanxinkj.top

[C05] 返回多个值
来源：http://tbn.ivvv.top

Py:   return a, b
来源：http://fuq.havefunace.top

PHP:  return [$a, $b];
来源：http://cuy.xylfe.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xtn.snrcjt.cn

TS:   return { a, b };
来源：http://szj.dashuyun.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mqb.andypj.xyz

Go:   return a, b
来源：http://wtp.zhixingplan.top

Ruby: return a, b
来源：http://bqt.ehwqpu.com

C#:   return (a, b);              // ValueTuple
来源：http://gfn.gaohongyu789.top

[C06] 匿名函数 / lambda
来源：http://rwo.bjfxy.top

Py:   square = lambda x: x * x
来源：http://kbx.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mkm.cucudq.cn

JS:   const square = x => x * x;
来源：http://uwm.chenzaomai.com

TS:   const square = (x: number): number => x * x;
来源：http://unv.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jir.wangshuangyany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tvs.ybcxt.top

Ruby: square = ->(x) { x * x }
来源：http://mwo.xylfe.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fxp.snrcjt.cn

[C07] 把函数作为参数传入
来源：http://ndw.cheryme.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://scm.pycfn.com

PHP:  array_map("strtoupper", $arr);
来源：http://mpa.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fyy.fehbvm.com

TS:   arr.map(String)
来源：http://gqn.jinqigfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fvl.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mbe.jqgfzy.top

Ruby: arr.map(&:upcase)
来源：http://ceo.redwolf501.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lwv.jlsjyb.cn

[C08] 闭包
来源：http://hqt.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yan.xziqi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yzd.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://axm.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qzh.xinyue.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zqe.jinqigfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gnb.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://unc.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rvg.tian-w.cn

[C09] 递归
来源：http://gwf.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rfl.c1oappe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oiv.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gks.nwbrower.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ngj.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fan.chenlongwang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://evh.andypj.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://szw.smart0.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rxc.wangshuangyany.cn

[C10] 变量作用域
来源：http://jdi.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ipo.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ltu.dashuyun.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vqx.hysaishi.cn

TS:   同 JS
来源：http://mwk.ctjpmb.com

Java: 方法内为块级作用域
来源：http://ezm.hnqzz.top

Go:   花括号块级作用域
来源：http://xtn.xuanzx.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://erv.xuetiantiany.cn

C#:   块级作用域
来源：http://jmc.cheryme.top

[C11] 模块导入与导出
来源：http://ads.fktsv.cn

Py:   from module import func
来源：http://wmf.nanxuanxn.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hcj.yuanzhike.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kkr.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vcx.quarkkingdee.top

Java: import java.util.List;
来源：http://orb.jqgufenzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jil.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://rhd.havefunace.top

C#:   using System.Text;
来源：http://afq.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://dob.316326.xyz

Py:   (lambda: print("run"))()
来源：http://mbj.cucudq.cn

PHP:  (function () { echo "run"; })();
来源：http://ptb.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://hfc.gogol.net.cn

TS:   (() => { console.log("run"); })();
来源：http://oxp.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rcm.hnqzz.top


<!-- 参考信息 -->