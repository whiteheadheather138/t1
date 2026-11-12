代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://zrm.ctjpmb.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qms.ctjpmb.com

JS:   (3.14159).toFixed(2)
来源：http://mze.zhongyouzk.top

TS:   (3.14159).toFixed(2)
来源：http://hzs.epnwcf.com

Java: String.format("%.2f", 3.14159)
来源：http://zgh.fzhhl.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kfw.xylfe.cn

Ruby: format("%.2f", 3.14159)
来源：http://him.0kj1m.cn

C#:   3.14159.ToString("F2")
来源：http://exr.sweek.top

[A22] 获取字符串长度
来源：http://kne.ehwqpu.com

Py:   len(s)
来源：http://sgd.hcnkem.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://axl.fengsongda.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://llq.xylfe.cn

TS:   s.length
来源：http://cle.zdbjq.cn

Java: s.length()
来源：http://nlo.wangdashe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zgw.jianghu66.top

Ruby: s.length
来源：http://xqv.xylfe.cn

C#:   s.Length
来源：http://kzp.zhongyouzk.top

[A23] 大小写转换
来源：http://ksn.fktsv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rcp.xingfuxueyuan.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yog.chenlongwang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xgt.shangyingyoupin.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ndx.jyoumei.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ryz.jqgufenzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://byg.shzxlz.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lmf.quarkkingdee.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mvv.andypj.xyz

[A24] 去除首尾空白
来源：http://qgo.fanxiaobao.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wxf.shangyingyoupin.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xmr.c1oappe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qwn.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qlm.mhx1999.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jjz.yangfankeji.com

Go:   strings.TrimSpace(s)
来源：http://ufp.jlsjyb.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hpk.ybcxt.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tmu.nanxuanxn.top

[A25] 字符串比较
来源：http://hyb.pycfn.com

Py:   s1 == s2; s1 != s2
来源：http://jqq.tian-w.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ahb.hongshengwenyu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wfp.iojbl.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://phm.jinqigufen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ybe.tian-w.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ese.sxryk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://edx.jinqigfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bbv.sysykeji.top

[A26] 类型转换总览
来源：http://gxf.jinqigfzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dvj.zhengqikj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://glx.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cjd.wangshuangyany.cn

TS:   Number() String() Boolean() x as number
来源：http://znw.yongpay.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://exu.hnqzz.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dgo.ydjk.org.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://edp.zycfv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hlr.svipenyu.cn

================================================================================
来源：http://cuw.dianchejie.cn

B. 流程控制
来源：http://rqz.jiagoushi.top

================================================================================
来源：http://vvb.hnxiangtu.top

[B01] 条件判断 if / else
来源：http://bgj.daxiang520.top

Py:   result = "正" if x > 0 else "非正"
来源：http://yyg.svipenyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jrs.xuetiantiany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kwk.hysaishi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ycb.fehbvm.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://rlh.daria6918.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tdt.pycfn.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://noy.yj20258888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hla.cheryme.top

[B02] 多分支 else if / elif
来源：http://gvs.shuidangran.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cni.tanke756.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mix.zhiwuduotai.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uhv.wangdashe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lzf.smart0.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bsb.sufxvd.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hcu.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fkt.ivvv.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://civ.zycfv.cn

[B03] switch / match / case
来源：http://yhv.shangyingyoupin.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ncu.haohaochexian.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xgs.jinqigfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cdm.gotoacloud.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dxd.hongshengwenyu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fux.hcnkem.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rrn.hnxiangtu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://czg.fanxiaobao.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rta.cdnleiting.top

[B04] for 计数循环
来源：http://bdx.hnxiangtu.top

Py:   for i in range(10): print(i)
来源：http://uet.snrcjt.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ulk.yonumen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pkt.yj20258.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xdz.ybcxt.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pfh.tian-w.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lhq.sufxvd.cn

Ruby: 10.times { |i| puts i }
来源：http://xls.52xcode.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wdt.jinqigfzy.top

[B05] 遍历数组 / 列表
来源：http://eua.yj20258888.top

Py:   for item in arr: print(item)
来源：http://trr.yj20258888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fqd.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ejt.jinyuanbaomall.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rsi.yanxiufei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eaf.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ymw.epnwcf.com

Ruby: arr.each { |item| puts item }
来源：http://fve.yanxiufei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sgb.yuxming.cn

[B06] 遍历字典 / 对象
来源：http://szn.9152youxi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://erc.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zbz.jyoumei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://agl.9152youxi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://opf.cheryme.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nuf.smart0.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vsg.gzhubu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lye.zhengqikj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sae.yj20258.top

[B07] while 循环
来源：http://mib.zhiwuduotai.top

Py:   while i < 10: i += 1
来源：http://tmx.yongpay.top

PHP:  while ($i < 10) { $i++; }
来源：http://zvu.hfpthk.cn

JS:   while (i < 10) { i++; }
来源：http://eyt.havefunace.top

TS:   while (i < 10) { i++; }
来源：http://vsv.ehwqpu.com

Java: while (i < 10) { i++; }
来源：http://zmw.haohaochexian.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zqq.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://igh.xuanzx.com

C#:   while (i < 10) { i++; }
来源：http://eox.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://nzs.wangdashe.top

Py:   # 无 do-while：用 while True + break
来源：http://aja.316326.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://lpn.quarkkingdee.top

JS:   do { i++; } while (i < 10);
来源：http://mtb.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://soo.cucudq.cn

Java: do { i++; } while (i < 10);
来源：http://veg.yj20258.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yft.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://upi.daxiang520.top

C#:   do { i++; } while (i < 10);
来源：http://dec.gotoacloud.top

[B09] break 与 continue
来源：http://gms.yvedp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cyc.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://whz.hammf.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pfz.jinyuanbaomall.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rpk.fktsv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ogs.guowangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ple.gzhubu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rcn.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vjt.yfazqb.com

[B10] 遍历同时拿索引
来源：http://vmg.yangfankeji.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yqm.sufxvd.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zzi.yonumen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://syb.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rcc.hesvh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uac.shanyushiyangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qng.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dvr.tianlin.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fts.shanyushiyangtech.top

[B11] 生成数字序列 / 区间
来源：http://dea.tian-w.cn

Py:   list(range(0, 10, 2))
来源：http://pbz.aibaodan.cn

PHP:  range(0, 10, 2);
来源：http://jio.zhongyouzk.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xta.shuidangran.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ubn.nanxuanxn.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wtg.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jbr.hammf.cn

Ruby: (0...10).step(2).to_a
来源：http://umq.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ucj.shuidangran.top

[B12] 跳出多层循环
来源：http://qip.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rsp.nanxinkj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://oyy.ybcxt.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kyy.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xlc.aizwys.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pbs.gogol.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jhw.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tbo.gzhubu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eha.tarul.cn

[B13] 判断是否为数字
来源：http://jgl.wangshuangyany.cn

Py:   isinstance(x, (int, float))
来源：http://izg.zhoulong.xyz

PHP:  is_numeric($x)
来源：http://itu.snrcjt.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vak.jyoumei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hht.hesvh.cn

Java: x instanceof Number
来源：http://jmn.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lns.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://fzl.yanxiufei.cn

C#:   x is int or double or decimal
来源：http://sxn.mhx1999.top

[B14] 判断值是否在集合内
来源：http://twi.aibaodan.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cpg.yongpay.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iap.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://mvz.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://gcf.iojbl.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://exb.sufxvd.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wbt.fktsv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jtt.epnwcf.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yaf.yj20258.top

[B15] 布尔运算与取反
来源：http://dhq.xuetiantiany.cn

Py:   a and b or not c
来源：http://wqk.bbcook.cn

PHP:  $a && $b || !$c
来源：http://nmd.pycfn.com

JS:   a && b || !c
来源：http://exm.cashguo.top

TS:   a && b || !c
来源：http://fyb.tian-w.cn

Java: a && b || !c
来源：http://unh.ctjpmb.com

Go:   a && b || !c
来源：http://has.xingfuxueyuan.xyz

Ruby: a && b || !c
来源：http://nja.yuxming.cn

C#:   a && b || !c
来源：http://imm.shzxlz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ath.guowangkeji.top

Py:   if not data: return
来源：http://org.fanxiaobao.xyz

PHP:  if (!$data) { return; }
来源：http://smd.iojbl.cn

JS:   if (!data) return;
来源：http://emm.shanyushiyangtech.top

TS:   if (!data) return;
来源：http://djd.cucudq.cn

Java: if (data == null) return;
来源：http://sgv.cheryme.top

Go:   if data == nil { return }
来源：http://sak.fehbvm.com

Ruby: return if data.nil?
来源：http://vhg.sysykeji.top

C#:   if (data == null) return;
来源：http://hgo.yuxming.cn

================================================================================
来源：http://zos.tianlin.xyz

C. 函数与作用域
来源：http://wvu.fktsv.cn

================================================================================
来源：http://kaj.aizwys.cn

[C01] 定义函数
来源：http://pdj.sweek.top

Py:   def add(a, b): return a + b
来源：http://pam.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ckt.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://rdr.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ndb.shuidangran.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ftu.guowangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://uak.quarkkingdee.top

Ruby: def add(a, b); a + b; end
来源：http://yhp.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dmr.zhongyouzk.top

[C02] 默认参数
来源：http://hwk.jlsjyb.cn

Py:   def greet(name="World"): return name
来源：http://agr.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zkt.xinyue.icu

JS:   function greet(name = "World") { return name; }
来源：http://ils.epnwcf.com

TS:   function greet(name: string = "World") { return name; }
来源：http://pgs.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://vst.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ugt.fktsv.cn

Ruby: def greet(name = "World") = name
来源：http://qnm.yj202588.top

C#:   string Greet(string name = "World") => name;
来源：http://qpk.yonumen.top

[C03] 可变参数
来源：http://oyp.daria6918.cn

Py:   def total(*args): return sum(args)
来源：http://kjr.yonumen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iig.xziqi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pbh.gogol.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qzm.gotoacloud.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uly.yj20258.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zvw.hongshengwenyu.top

Ruby: def total(*nums); nums.sum; end
来源：http://roh.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://urp.jinqigufen.top

[C04] 命名参数 / 关键字参数
来源：http://yjn.ydzc1.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lmx.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lce.shangyingyoupin.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wtx.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ikv.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://xwz.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://xsz.cdnleiting.top

Ruby: f(a: 1, b: 2)
来源：http://ugt.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://wls.zhengqikj.top

[C05] 返回多个值
来源：http://kyr.hammf.cn

Py:   return a, b
来源：http://vnw.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://wyn.vehdjk.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://xtu.wangshuangyany.cn

TS:   return { a, b };
来源：http://gnj.hysaishi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://col.zhoulong.xyz

Go:   return a, b
来源：http://aew.shanyushiyangtech.top

Ruby: return a, b
来源：http://zpp.jyoumei.cn

C#:   return (a, b);              // ValueTuple
来源：http://gwn.gotoacloud.top

[C06] 匿名函数 / lambda
来源：http://rkz.feifeiyinyue.top

Py:   square = lambda x: x * x
来源：http://qwz.uphjek.com

PHP:  $square = fn($x) => $x * $x;
来源：http://gch.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://lvk.andypj.xyz

TS:   const square = (x: number): number => x * x;
来源：http://wru.iojbl.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ura.daria6918.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zyq.nwbrower.top

Ruby: square = ->(x) { x * x }
来源：http://xma.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fsh.xziqi.cn

[C07] 把函数作为参数传入
来源：http://gzr.fengsongda.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fyy.andypj.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://dlz.shanyushiyangtech.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gmj.mhx1999.top

TS:   arr.map(String)
来源：http://qdb.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mwz.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bzm.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://oob.redwolf501.top

C#:   arr.Select(s => s.ToUpper())
来源：http://baj.wangshuangyany.cn

[C08] 闭包
来源：http://ije.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nxu.shuidangran.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://opo.ydzc1.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xcp.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nxs.ybcxt.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://twt.wangdashe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sui.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lvu.zhaomingkeji.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eot.sysykeji.top

[C09] 递归
来源：http://pfk.nanxuanxn.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qma.andypj.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fmv.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oin.bjfxy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wue.vqdsnc.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lke.daxiang520.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://goa.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sck.feifeiyinyue.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iph.ydzc1.top

[C10] 变量作用域
来源：http://peq.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ape.epnwcf.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mqd.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qmi.fzhhl.top

TS:   同 JS
来源：http://gul.ehwqpu.com

Java: 方法内为块级作用域
来源：http://qyi.mhx1999.top

Go:   花括号块级作用域
来源：http://imq.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ime.zhixingplan.top

C#:   块级作用域
来源：http://ojh.redwolf501.top

[C11] 模块导入与导出
来源：http://ilz.uphjek.com

Py:   from module import func
来源：http://veu.9152youxi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://exz.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://xqd.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uqw.zhixingplan.top

Java: import java.util.List;
来源：http://epb.jinyuanbaomall.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nrk.uphjek.com


<!-- 参考信息 -->