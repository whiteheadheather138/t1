代发 wailian999

[A22] 获取字符串长度
来源：http://ckm.pycfn.com

Py:   len(s)
来源：http://xay.daxiang520.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lfg.wangdashe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pyg.xinyue.icu

TS:   s.length
来源：http://eyn.chenzaomai.com

Java: s.length()
来源：http://sdy.shangyingyoupin.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sjw.cheryme.top

Ruby: s.length
来源：http://xal.ppjwa.cn

C#:   s.Length
来源：http://iua.iojbl.cn

[A23] 大小写转换
来源：http://mby.52xcode.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wmi.sweek.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://djy.sweek.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pjm.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rqy.zdbjq.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mqr.tanke756.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://amd.wangshuangyany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://psv.xylfe.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qrc.nwbrower.top

[A24] 去除首尾空白
来源：http://qgo.birdmap.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lhp.hongshengwenyu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sle.jianghu66.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qgs.shanyushiyangtech.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ewp.hnqzz.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pmq.quarkkingdee.top

Go:   strings.TrimSpace(s)
来源：http://shv.jinqigfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cvo.sjlbkw.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zzj.52xcode.cn

[A25] 字符串比较
来源：http://dds.316326.xyz

Py:   s1 == s2; s1 != s2
来源：http://fjk.birdmap.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cec.hcnkem.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kda.ppjwa.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://urs.ppjwa.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nwj.jinqigufen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jee.sjlbkw.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ffi.aibaodan.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wnu.hfpthk.cn

[A26] 类型转换总览
来源：http://odm.aizwys.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jfs.zhaomingkeji.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tud.ppjwa.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ebp.ehwqpu.com

TS:   Number() String() Boolean() x as number
来源：http://due.tanke756.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ywh.tanke756.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://alb.daria6918.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fdd.jinqigufen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qdw.epnwcf.com

================================================================================
来源：http://ucr.nanxinkj.top

B. 流程控制
来源：http://dez.dianchejie.cn

================================================================================
来源：http://mie.gogol.net.cn

[B01] 条件判断 if / else
来源：http://yoj.hywenlv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hnf.wangdashe.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ysa.kuanghao11.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fge.quarkkingdee.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ael.sweek.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://faz.gotoacloud.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lnq.xinyue.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nvz.daria6918.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zdq.cucudq.cn

[B02] 多分支 else if / elif
来源：http://min.hywenlv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jzq.meibo888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bta.chenjidiqi.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vxr.xziqi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fni.kuanghao11.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://frj.nanxinkj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oey.smart0.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xjt.epnwcf.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vgd.xuanzx.com

[B03] switch / match / case
来源：http://vzk.nwbrower.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yvb.zhongyouzk.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wlz.hesvh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://juy.zhongyouzk.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xqs.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.aizwys.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ren.sxryk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ftx.yj20258888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://byc.fengsongda.top

[B04] for 计数循环
来源：http://olv.hesvh.cn

Py:   for i in range(10): print(i)
来源：http://kwy.sxryk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fms.feifeiyinyue.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bts.wangdashe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dep.cucudq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tsb.cheryme.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pqy.feifeiyinyue.top

Ruby: 10.times { |i| puts i }
来源：http://abn.jianghu66.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wgw.andypj.xyz

[B05] 遍历数组 / 列表
来源：http://hnq.quarkkingdee.top

Py:   for item in arr: print(item)
来源：http://ljn.shuidangran.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mft.bbcook.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hjk.chenlongwang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ysl.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fhe.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fqt.xylfe.cn

Ruby: arr.each { |item| puts item }
来源：http://bir.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zmu.quarkkingdee.top

[B06] 遍历字典 / 对象
来源：http://ozu.pengpengdd.cyou

Py:   for k, v in d.items(): print(k, v)
来源：http://zwu.zhengqikj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wkn.xinyue.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mds.yongpay.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://frb.jyoumei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nyh.xuanzx.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qqg.smart0.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jvk.xuetiantiany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xlp.jqgufenzy.top

[B07] while 循环
来源：http://dhu.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://vqs.yanxiufei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hrt.hysaishi.cn

JS:   while (i < 10) { i++; }
来源：http://bjp.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://tuq.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://ikd.birdmap.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mfe.xingfuxueyuan.xyz

Ruby: while i < 10; i += 1; end
来源：http://ukd.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://ugt.dianchejie.cn

[B08] do-while（至少执行一次）
来源：http://viw.snrcjt.cn

Py:   # 无 do-while：用 while True + break
来源：http://cki.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://yef.jqgfzy.top

JS:   do { i++; } while (i < 10);
来源：http://imn.iojbl.cn

TS:   do { i++; } while (i < 10);
来源：http://lzr.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://rms.fzhhl.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hcu.xuanzx.com

Ruby: begin; i += 1; end while i < 10
来源：http://vxh.jinqigufen.top

C#:   do { i++; } while (i < 10);
来源：http://syd.zycfv.cn

[B09] break 与 continue
来源：http://van.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hml.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wyg.mhx1999.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hva.shanyushiyangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ytq.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qwr.dashuyun.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nuv.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qae.yuanzhike.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lpx.yonumen.top

[B10] 遍历同时拿索引
来源：http://auw.nwbrower.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qid.jqgufenzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hsn.hywenlv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zaq.snrcjt.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dkv.ehwqpu.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bgc.wangshuangyany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vpc.andypj.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dvl.jinqigufen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xdb.meibo888.top

[B11] 生成数字序列 / 区间
来源：http://eol.hongshengwenyu.top

Py:   list(range(0, 10, 2))
来源：http://rqd.feifeiyinyue.top

PHP:  range(0, 10, 2);
来源：http://jmb.hywenlv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cle.gaohongyu789.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xor.9152youxi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ocr.birdmap.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vmd.yfazqb.com

Ruby: (0...10).step(2).to_a
来源：http://eah.ctjpmb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dks.zhaomingkeji.xyz

[B12] 跳出多层循环
来源：http://ysd.zhoulong.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://bmc.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gog.zdbjq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fyc.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jog.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://klc.redwolf501.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ren.vehdjk.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://irl.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nqj.cashguo.top

[B13] 判断是否为数字
来源：http://syl.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://xpp.jinghuilouyu.cn

PHP:  is_numeric($x)
来源：http://giv.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wem.iojbl.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nlx.fzhhl.top

Java: x instanceof Number
来源：http://mtg.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tjj.hywenlv.cn

Ruby: x.is_a?(Numeric)
来源：http://fgm.fengsongda.top

C#:   x is int or double or decimal
来源：http://kos.shzxlz.cn

[B14] 判断值是否在集合内
来源：http://ciz.ehwqpu.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dun.jianghu66.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hoo.epnwcf.com

JS:   [1, 2, 3].includes(x)
来源：http://aai.yanxiufei.cn

TS:   [1, 2, 3].includes(x)
来源：http://jes.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uxr.tarul.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xgp.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dlg.vqdsnc.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nvd.quarkkingdee.top

[B15] 布尔运算与取反
来源：http://rjc.wangdashe.top

Py:   a and b or not c
来源：http://rsl.yj20258888.top

PHP:  $a && $b || !$c
来源：http://scg.sjlbkw.cn

JS:   a && b || !c
来源：http://hbd.meibo888.top

TS:   a && b || !c
来源：http://bia.shanyushiyangtech.top

Java: a && b || !c
来源：http://hoc.meibo888.top

Go:   a && b || !c
来源：http://ewz.vqdsnc.cn

Ruby: a && b || !c
来源：http://ypn.zdqjudy.top

C#:   a && b || !c
来源：http://tfx.cdnleiting.top

[B16] 卫语句：不满足条件提前返回
来源：http://ezl.mhx1999.top

Py:   if not data: return
来源：http://rcl.yonumen.top

PHP:  if (!$data) { return; }
来源：http://iwh.nwbrower.top

JS:   if (!data) return;
来源：http://xku.zhaomingkeji.xyz

TS:   if (!data) return;
来源：http://dvl.cqqwz.cn

Java: if (data == null) return;
来源：http://bay.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://ryk.jianghu66.top

Ruby: return if data.nil?
来源：http://lqc.jlsjyb.cn

C#:   if (data == null) return;
来源：http://llo.ppjwa.cn

================================================================================
来源：http://yow.c1oappe.top

C. 函数与作用域
来源：http://pch.chenzaomai.com

================================================================================
来源：http://nlo.fzhhl.top

[C01] 定义函数
来源：http://aox.yuanzhike.top

Py:   def add(a, b): return a + b
来源：http://stj.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qbo.zhengqikj.top

JS:   function add(a, b) { return a + b; }
来源：http://kad.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dbx.tian-w.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ary.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dsv.yuxming.cn

Ruby: def add(a, b); a + b; end
来源：http://ern.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tlv.aizwys.cn

[C02] 默认参数
来源：http://woz.quarkkingdee.top

Py:   def greet(name="World"): return name
来源：http://nyf.yueranfly.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gsr.52xcode.cn

JS:   function greet(name = "World") { return name; }
来源：http://ojf.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mol.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ruf.yvedp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mah.jiagoushi.top

Ruby: def greet(name = "World") = name
来源：http://wek.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://llh.aibaodan.cn

[C03] 可变参数
来源：http://ntz.xuanzx.com

Py:   def total(*args): return sum(args)
来源：http://tsf.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zha.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cus.yongpay.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xiy.jinghuilouyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hwo.zhaomingkeji.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oom.vqdsnc.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bsl.fehbvm.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ife.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://han.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uhi.vqdsnc.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jgo.shuidangran.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hpd.fehbvm.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://foo.hnqzz.top

Java: // 无：用 Builder 模式或 record
来源：http://for.snrcjt.cn

Go:   // 无：用配置结构体参数
来源：http://gqa.yvedp.cn

Ruby: f(a: 1, b: 2)
来源：http://jsx.zycfv.cn

C#:   f(a: 1, b: 2)
来源：http://xdx.cashguo.top

[C05] 返回多个值
来源：http://flb.shanyushiyangkeji.top

Py:   return a, b
来源：http://xdj.havefunace.top

PHP:  return [$a, $b];
来源：http://tzc.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vpa.zdqjudy.top

TS:   return { a, b };
来源：http://paj.sjlbkw.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://esq.xinyue.icu

Go:   return a, b
来源：http://fga.hysaishi.cn

Ruby: return a, b
来源：http://ril.shzxlz.cn

C#:   return (a, b);              // ValueTuple
来源：http://jad.ybcxt.top

[C06] 匿名函数 / lambda
来源：http://ush.smart0.xyz

Py:   square = lambda x: x * x
来源：http://dte.zhijiandao.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yyd.jinqigufen.top

JS:   const square = x => x * x;
来源：http://vhn.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://tyn.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://imz.zycfv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gkk.shuidangran.top

Ruby: square = ->(x) { x * x }
来源：http://hup.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://pit.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://mci.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://epr.birdmap.top

PHP:  array_map("strtoupper", $arr);
来源：http://wis.snrcjt.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zxj.mhx1999.top

TS:   arr.map(String)
来源：http://pmd.zhongyouzk.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fwk.yonumen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://odq.cdnleiting.top

Ruby: arr.map(&:upcase)
来源：http://xts.sjlbkw.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jaz.nanxuanxn.top

[C08] 闭包
来源：http://lyg.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uti.zdbjq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ibh.bjfxy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qyr.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://znh.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://edh.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jsk.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kzs.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aqr.yuxming.cn

[C09] 递归
来源：http://nve.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qak.zhijiandao.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sly.hammf.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ani.ivvv.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qws.daxiang520.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uzv.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bdm.jinqigfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zgv.vqdsnc.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://akf.nanxuanxn.top

[C10] 变量作用域
来源：http://uar.chenzaomai.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pkb.daxiang520.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jyh.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xyo.zdbjq.cn

TS:   同 JS
来源：http://ugw.jinghuilouyu.cn

Java: 方法内为块级作用域
来源：http://tts.jinqigufen.top

Go:   花括号块级作用域
来源：http://cjf.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jmb.hfpthk.cn

C#:   块级作用域
来源：http://jbj.birdmap.top

[C11] 模块导入与导出
来源：http://ovr.cucudq.cn

Py:   from module import func
来源：http://ljw.shangyingyoupin.top

PHP:  require "file.php";  或 use App\Service;
来源：http://igy.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gvm.ydjk.org.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vrh.chenlongwang.top

Java: import java.util.List;
来源：http://ahp.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gqc.316326.xyz

Ruby: require "json"; require_relative "./util"
来源：http://dmy.0kj1m.cn

C#:   using System.Text;
来源：http://tgk.ivvv.top

[C12] 立即执行函数 IIFE
来源：http://rkp.sjlbkw.cn

Py:   (lambda: print("run"))()
来源：http://iph.tarul.cn

PHP:  (function () { echo "run"; })();
来源：http://kvu.aibaodan.cn

JS:   (() => { console.log("run"); })();
来源：http://vbx.hysaishi.cn

TS:   (() => { console.log("run"); })();
来源：http://amf.cqqwz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://avi.xylfe.cn


<!-- 参考信息 -->