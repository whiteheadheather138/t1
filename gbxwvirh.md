代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://awf.tianlin.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ntw.316326.xyz

Ruby: format("%.2f", 3.14159)
来源：http://msb.0kj1m.cn

C#:   3.14159.ToString("F2")
来源：http://bbs.hfpthk.cn

[A22] 获取字符串长度
来源：http://ehc.hnqzz.top

Py:   len(s)
来源：http://wsj.fktsv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nbi.shzxlz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fiy.zhongyouzk.top

TS:   s.length
来源：http://wqm.c1oappe.top

Java: s.length()
来源：http://sik.hnxiangtu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yfu.zdqjudy.top

Ruby: s.length
来源：http://dxs.jianghu66.top

C#:   s.Length
来源：http://pbz.gogol.net.cn

[A23] 大小写转换
来源：http://qif.smart0.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://iif.ywan-chungtsiang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qox.dianchejie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xbd.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://naf.0kj1m.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ttg.yj202588.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jlw.xinyue.icu

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xbi.jinqigufen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://afx.uphjek.com

[A24] 去除首尾空白
来源：http://vrc.tarul.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cbb.epnwcf.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://msf.xuanzx.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://slc.gzhubu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tbe.iojbl.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cbh.fehbvm.com

Go:   strings.TrimSpace(s)
来源：http://pjy.sxryk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fum.cashguo.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fxr.pycfn.com

[A25] 字符串比较
来源：http://wpz.jinghuilouyu.cn

Py:   s1 == s2; s1 != s2
来源：http://ueb.zhongyouzk.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rof.zdqjudy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rgl.jinqigufen.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pgp.daria6918.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zho.ivvv.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nnm.fengsongda.top

Ruby: s1 == s2; s1 <=> s2
来源：http://uqf.shuidangran.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://guf.sufxvd.cn

[A26] 类型转换总览
来源：http://nxh.xziqi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://inw.yuanzhike.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yxq.wangdashe.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bax.cucudq.cn

TS:   Number() String() Boolean() x as number
来源：http://tlr.fengsongda.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vix.zhixingplan.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dnk.yongpay.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zas.hnxiangtu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://biy.chenlongwang.top

================================================================================
来源：http://lxd.chenjidiqi.icu

B. 流程控制
来源：http://lwi.gzhubu.top

================================================================================
来源：http://ioy.fzhhl.top

[B01] 条件判断 if / else
来源：http://twp.cashguo.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ppk.shuidangran.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vxt.dashuyun.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gfp.zhijiandao.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xvj.yj20258.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qhb.gogol.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bvt.vqdsnc.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wcc.feifeiyinyue.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qea.yangfankeji.com

[B02] 多分支 else if / elif
来源：http://ejn.jinqigufen.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://drb.hesvh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://grk.jiagoushi.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kgr.wangdashe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xqu.smart0.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yzd.xylfe.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iks.zdbjq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pnu.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mdt.xziqi.cn

[B03] switch / match / case
来源：http://kyq.yonumen.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zfw.yonumen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pky.pengpengdd.cyou

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ieq.jiagoushi.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mxr.uphjek.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ryw.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ijd.yuanzhike.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gim.tianlin.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pxb.tian-w.cn

[B04] for 计数循环
来源：http://fgy.yj20258.top

Py:   for i in range(10): print(i)
来源：http://bhy.cashguo.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rri.fanxiaobao.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ibt.vqdsnc.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dso.guannengcc.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zlu.jiagoushi.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xxm.zhoulong.xyz

Ruby: 10.times { |i| puts i }
来源：http://xpp.wangshuangyany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yxv.zhijiandao.cn

[B05] 遍历数组 / 列表
来源：http://was.zhaomingkeji.xyz

Py:   for item in arr: print(item)
来源：http://gzc.hywenlv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hib.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gxz.gogol.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://slj.316326.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://ywv.hongshengwenyu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jii.xinyue.icu

Ruby: arr.each { |item| puts item }
来源：http://wmg.tianlin.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yoh.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://xcx.cheryme.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ktn.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qaf.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hco.nanxuanxn.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://adi.fanxiaobao.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gmz.hywenlv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jbb.pycfn.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bfv.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rwn.daria6918.cn

[B07] while 循环
来源：http://tsu.ydjk.org.cn

Py:   while i < 10: i += 1
来源：http://jly.9152youxi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mqx.aibaodan.cn

JS:   while (i < 10) { i++; }
来源：http://ikw.dianchejie.cn

TS:   while (i < 10) { i++; }
来源：http://wry.kuanghao11.cn

Java: while (i < 10) { i++; }
来源：http://eah.shuidangran.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zlo.wangshuangyany.cn

Ruby: while i < 10; i += 1; end
来源：http://lqu.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://tmm.cdnleiting.top

[B08] do-while（至少执行一次）
来源：http://xwq.cqqwz.cn

Py:   # 无 do-while：用 while True + break
来源：http://hkd.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jtx.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://fkv.bjfxy.top

TS:   do { i++; } while (i < 10);
来源：http://xjh.zhiwuduotai.top

Java: do { i++; } while (i < 10);
来源：http://slp.jinyuanbaomall.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://siq.wangshuangyany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://frm.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://wgy.tanke756.top

[B09] break 与 continue
来源：http://dba.gotoacloud.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sle.shzxlz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mxr.ydjk.org.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vyf.chenjidiqi.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mru.bjfxy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nqo.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wew.jinghuilouyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ldv.316326.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ujt.jinqigfzy.top

[B10] 遍历同时拿索引
来源：http://pzy.zhoulong.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qcl.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nzj.sjlbkw.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nzg.yueranfly.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://idk.uphjek.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xlx.bjfxy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fon.quarkkingdee.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zwd.yuxming.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qlc.hongshengwenyu.top

[B11] 生成数字序列 / 区间
来源：http://gwb.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://drh.tian-w.cn

PHP:  range(0, 10, 2);
来源：http://ryl.hammf.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cuu.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fxo.smart0.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zaq.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://azz.guannengcc.top

Ruby: (0...10).step(2).to_a
来源：http://cpv.shzxlz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ijv.hnqzz.top

[B12] 跳出多层循环
来源：http://jqx.316326.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://wbw.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vtx.hongshengwenyu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://utp.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jpt.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qnp.sysykeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rkr.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dum.tarul.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zqb.dashuyun.cn

[B13] 判断是否为数字
来源：http://hvr.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://arv.jlsjyb.cn

PHP:  is_numeric($x)
来源：http://bnx.sufxvd.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hop.birdmap.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://evz.wangshuangyany.cn

Java: x instanceof Number
来源：http://vnc.yj20258888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wds.sxryk.cn

Ruby: x.is_a?(Numeric)
来源：http://iyi.cdnleiting.top

C#:   x is int or double or decimal
来源：http://qqf.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://jee.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wxu.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tqf.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://hpw.feifeiyinyue.top

TS:   [1, 2, 3].includes(x)
来源：http://zad.ybcxt.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dcg.chenzaomai.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lgt.guannengcc.top

Ruby: [1, 2, 3].include?(x)
来源：http://lti.gzhubu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://opc.uphjek.com

[B15] 布尔运算与取反
来源：http://klt.cucudq.cn

Py:   a and b or not c
来源：http://vfi.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://mry.jqgufenzy.top

JS:   a && b || !c
来源：http://jsw.316326.xyz

TS:   a && b || !c
来源：http://kzl.bjfxy.top

Java: a && b || !c
来源：http://hco.gaohongyu789.top

Go:   a && b || !c
来源：http://rhg.yanxiufei.cn

Ruby: a && b || !c
来源：http://bbr.hcnkem.com

C#:   a && b || !c
来源：http://mtf.sjlbkw.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xsl.gotoacloud.top

Py:   if not data: return
来源：http://txx.jinqigfzy.top

PHP:  if (!$data) { return; }
来源：http://ggn.ywan-chungtsiang.top

JS:   if (!data) return;
来源：http://mxu.uphjek.com

TS:   if (!data) return;
来源：http://vet.yj202588.top

Java: if (data == null) return;
来源：http://ouf.epnwcf.com

Go:   if data == nil { return }
来源：http://yrj.zdqjudy.top

Ruby: return if data.nil?
来源：http://bak.shuidangran.top

C#:   if (data == null) return;
来源：http://szr.tianlin.xyz

================================================================================
来源：http://ydp.9152youxi.cn

C. 函数与作用域
来源：http://nhp.hcnkem.com

================================================================================
来源：http://cwp.bjfxy.top

[C01] 定义函数
来源：http://ypl.zdqjudy.top

Py:   def add(a, b): return a + b
来源：http://hlj.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hlh.hnqzz.top

JS:   function add(a, b) { return a + b; }
来源：http://ntp.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://die.ywan-chungtsiang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gnv.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://vim.xuetiantiany.cn

Ruby: def add(a, b); a + b; end
来源：http://hfz.jinghuilouyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blg.shanyushiyangtech.top

[C02] 默认参数
来源：http://gob.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://dny.bbcook.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zsk.mhx1999.top

JS:   function greet(name = "World") { return name; }
来源：http://mjt.aizwys.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eis.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://zwd.smart0.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://moy.hesvh.cn

Ruby: def greet(name = "World") = name
来源：http://xor.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://bja.andypj.xyz

[C03] 可变参数
来源：http://yvz.guannengcc.top

Py:   def total(*args): return sum(args)
来源：http://xec.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://chy.tian-w.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bnh.iojbl.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uvz.hnxiangtu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fuz.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://enu.fzhhl.top

Ruby: def total(*nums); nums.sum; end
来源：http://xhp.sxryk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vwg.zdbjq.cn

[C04] 命名参数 / 关键字参数
来源：http://syo.yonumen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jct.tanke756.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blm.jinqigfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://czn.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vma.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://bwz.birdmap.top

Go:   // 无：用配置结构体参数
来源：http://qgo.yueranfly.top

Ruby: f(a: 1, b: 2)
来源：http://nof.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://moo.zhiwuduotai.top

[C05] 返回多个值
来源：http://qku.jinqigufen.top

Py:   return a, b
来源：http://mmz.zycfv.cn

PHP:  return [$a, $b];
来源：http://qor.xziqi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hne.hongshengwenyu.top

TS:   return { a, b };
来源：http://gac.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iel.gaohongyu789.top

Go:   return a, b
来源：http://npt.uphjek.com

Ruby: return a, b
来源：http://cxr.tianlin.xyz

C#:   return (a, b);              // ValueTuple
来源：http://wts.meibo888.top

[C06] 匿名函数 / lambda
来源：http://tiv.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://jbi.kuanghao11.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kqz.yueranfly.top

JS:   const square = x => x * x;
来源：http://cdd.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://bvi.ehwqpu.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ggp.hongshengwenyu.top

Go:   sq := func(x int) int { return x * x }
来源：http://vod.kuanghao11.cn

Ruby: square = ->(x) { x * x }
来源：http://fzq.cdnleiting.top

C#:   Func<int, int> square = x => x * x;
来源：http://qkm.gzhubu.top

[C07] 把函数作为参数传入
来源：http://svb.ybcxt.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pce.havefunace.top

PHP:  array_map("strtoupper", $arr);
来源：http://wrn.dashuyun.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cap.guowangkeji.top

TS:   arr.map(String)
来源：http://qdb.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bnh.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wgd.ybcxt.top

Ruby: arr.map(&:upcase)
来源：http://umn.0kj1m.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://efi.nanxuanxn.top

[C08] 闭包
来源：http://och.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jli.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wdy.hfpthk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qrr.gaohongyu789.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xrg.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dxy.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ibk.gzhubu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hel.sysykeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iwy.xingfuxueyuan.xyz

[C09] 递归
来源：http://fau.cqqwz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://paz.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://atf.ydjk.org.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://srv.zdqjudy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nem.gzhubu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://chc.yangfankeji.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://orh.xinyue.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zur.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://loj.bbcook.cn

[C10] 变量作用域
来源：http://zfr.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tlm.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cos.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mza.0kj1m.cn

TS:   同 JS
来源：http://trc.zhixingplan.top

Java: 方法内为块级作用域
来源：http://hve.fehbvm.com

Go:   花括号块级作用域
来源：http://hfi.sysykeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cle.ehwqpu.com

C#:   块级作用域
来源：http://quu.nwbrower.top

[C11] 模块导入与导出
来源：http://haz.gaohongyu789.top

Py:   from module import func
来源：http://nub.gzhubu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://iwv.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://inv.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tqv.sysykeji.top

Java: import java.util.List;
来源：http://npx.hnqzz.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zse.sjlbkw.cn

Ruby: require "json"; require_relative "./util"
来源：http://mcz.gogol.net.cn

C#:   using System.Text;
来源：http://frn.jiagoushi.top

[C12] 立即执行函数 IIFE
来源：http://chl.sweek.top

Py:   (lambda: print("run"))()
来源：http://xkw.nwbrower.top


<!-- 参考信息 -->