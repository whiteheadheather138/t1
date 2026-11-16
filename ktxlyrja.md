代发 wailian999

[A22] 获取字符串长度
来源：http://gyq.daxiang520.top

Py:   len(s)
来源：http://eaa.nwbrower.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vrj.52xcode.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fkt.redwolf501.top

TS:   s.length
来源：http://pqn.xinyue.icu

Java: s.length()
来源：http://gtz.aizwys.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vqa.xziqi.cn

Ruby: s.length
来源：http://kcb.ctjpmb.com

C#:   s.Length
来源：http://eya.fktsv.cn

[A23] 大小写转换
来源：http://bcb.smart0.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://ydf.wangdashe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vao.gzhubu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iin.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mec.c1oappe.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rcn.hfpthk.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ezc.ybcxt.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qwa.zdbjq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nty.sweek.top

[A24] 去除首尾空白
来源：http://jxd.aizwys.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hpe.ydjk.org.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vrc.wangshuangyany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uwv.fengsongda.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yhd.pengpengdd.cyou

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bqg.jqgufenzy.top

Go:   strings.TrimSpace(s)
来源：http://dcu.havefunace.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lth.jinqigfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jfh.xuanzx.com

[A25] 字符串比较
来源：http://abg.wangdashe.top

Py:   s1 == s2; s1 != s2
来源：http://nhw.jinqigfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ddt.jianghu66.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rmz.birdmap.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://msg.zdqjudy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ksc.shanyushiyangtech.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bkb.zhiwuduotai.top

Ruby: s1 == s2; s1 <=> s2
来源：http://zld.chenzaomai.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ypc.c1oappe.top

[A26] 类型转换总览
来源：http://xfx.jinqigfzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oip.zhoulong.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iqf.pycfn.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wgh.yongpay.top

TS:   Number() String() Boolean() x as number
来源：http://fhp.hysaishi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nny.zycfv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bkm.cashguo.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vmq.zhaomingkeji.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://riv.chenjidiqi.icu

================================================================================
来源：http://srj.cheryme.top

B. 流程控制
来源：http://tth.jlsjyb.cn

================================================================================
来源：http://jlw.fehbvm.com

[B01] 条件判断 if / else
来源：http://gjt.wangdashe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ece.chenzaomai.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vqa.ppjwa.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wfv.zhixingplan.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xcp.ybcxt.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://eps.nanxuanxn.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uwu.jinqigfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dxi.shzxlz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gnw.smart0.xyz

[B02] 多分支 else if / elif
来源：http://qvg.xuanzx.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rrp.shanyushiyangtech.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zty.hfpthk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://egb.gzhubu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wbc.vqdsnc.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eqp.svipenyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uby.feifeiyinyue.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xzj.andypj.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nzw.hnxiangtu.top

[B03] switch / match / case
来源：http://juu.hnqzz.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fnt.svipenyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ara.haohaochexian.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dem.zhijiandao.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://djh.fzhhl.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ijl.jqgufenzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kit.kuanghao11.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wjy.hongshengwenyu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ohu.hywenlv.cn

[B04] for 计数循环
来源：http://fwl.ivvv.top

Py:   for i in range(10): print(i)
来源：http://oqq.fengsongda.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xvq.fanxiaobao.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hgj.iojbl.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zpp.ctjpmb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dfm.52xcode.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kez.ivvv.top

Ruby: 10.times { |i| puts i }
来源：http://ffs.nwbrower.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://plk.epnwcf.com

[B05] 遍历数组 / 列表
来源：http://aai.hnqzz.top

Py:   for item in arr: print(item)
来源：http://rte.guowangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xbi.jinqigufen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://axv.c1oappe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ilv.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vop.yonumen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rsg.shanyushiyangtech.top

Ruby: arr.each { |item| puts item }
来源：http://zrl.chenzaomai.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jeg.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://mda.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wfh.zhijiandao.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rym.bjfxy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ehx.fzhhl.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ngc.tarul.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vkb.ydzc1.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hpt.aibaodan.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rcv.wangdashe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ucu.tianlin.xyz

[B07] while 循环
来源：http://lrl.vqdsnc.cn

Py:   while i < 10: i += 1
来源：http://zwo.jinqigufen.top

PHP:  while ($i < 10) { $i++; }
来源：http://owv.shzxlz.cn

JS:   while (i < 10) { i++; }
来源：http://wij.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://bdc.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://ngg.hongshengwenyu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cqv.yueranfly.top

Ruby: while i < 10; i += 1; end
来源：http://dfs.fanxiaobao.xyz

C#:   while (i < 10) { i++; }
来源：http://ssc.daxiang520.top

[B08] do-while（至少执行一次）
来源：http://tay.kuanghao11.cn

Py:   # 无 do-while：用 while True + break
来源：http://jtx.jiagoushi.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yti.smart0.xyz

JS:   do { i++; } while (i < 10);
来源：http://icq.tanke756.top

TS:   do { i++; } while (i < 10);
来源：http://bfe.shzxlz.cn

Java: do { i++; } while (i < 10);
来源：http://eec.sufxvd.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qsr.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xoa.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://bms.uphjek.com

[B09] break 与 continue
来源：http://psw.redwolf501.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://arh.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lam.fanxiaobao.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bot.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://toe.yuxming.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jtd.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wmq.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mul.yuxming.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sqv.cucudq.cn

[B10] 遍历同时拿索引
来源：http://sdn.daria6918.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://udr.sufxvd.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://clu.fengsongda.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gsy.0kj1m.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qur.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bdj.pycfn.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mdf.daxiang520.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wip.chenlongwang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nyf.yanxiufei.cn

[B11] 生成数字序列 / 区间
来源：http://hyk.ydzc1.top

Py:   list(range(0, 10, 2))
来源：http://omd.tian-w.cn

PHP:  range(0, 10, 2);
来源：http://xvd.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uyi.hesvh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tfg.yangfankeji.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oba.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nuh.kuanghao11.cn

Ruby: (0...10).step(2).to_a
来源：http://kbp.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wes.fzhhl.top

[B12] 跳出多层循环
来源：http://pus.andypj.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://xcr.wangdashe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://sbc.jqgfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gch.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://atk.zhijiandao.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nmd.chenzaomai.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jtl.0kj1m.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ezh.gogol.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gyu.quarkkingdee.top

[B13] 判断是否为数字
来源：http://mpx.jlsjyb.cn

Py:   isinstance(x, (int, float))
来源：http://xmy.daxiang520.top

PHP:  is_numeric($x)
来源：http://xsv.jinyuanbaomall.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xnx.yfazqb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://liv.jqgufenzy.top

Java: x instanceof Number
来源：http://xzz.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://odc.havefunace.top

Ruby: x.is_a?(Numeric)
来源：http://occ.birdmap.top

C#:   x is int or double or decimal
来源：http://myw.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://nae.xingfuxueyuan.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ubw.gogol.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qlo.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://acv.sjlbkw.cn

TS:   [1, 2, 3].includes(x)
来源：http://zcz.gzhubu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://avb.nwbrower.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wyj.haohaochexian.top

Ruby: [1, 2, 3].include?(x)
来源：http://mde.cheryme.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://izu.chenzaomai.com

[B15] 布尔运算与取反
来源：http://cpn.andypj.xyz

Py:   a and b or not c
来源：http://cdq.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://gua.iojbl.cn

JS:   a && b || !c
来源：http://mtb.yongpay.top

TS:   a && b || !c
来源：http://grs.jlsjyb.cn

Java: a && b || !c
来源：http://hax.iojbl.cn

Go:   a && b || !c
来源：http://cjz.ivvv.top

Ruby: a && b || !c
来源：http://pev.chenlongwang.top

C#:   a && b || !c
来源：http://ypv.vqdsnc.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gqi.52xcode.cn

Py:   if not data: return
来源：http://lsl.snrcjt.cn

PHP:  if (!$data) { return; }
来源：http://lji.sweek.top

JS:   if (!data) return;
来源：http://fft.dashuyun.cn

TS:   if (!data) return;
来源：http://fcn.andypj.xyz

Java: if (data == null) return;
来源：http://wgt.jlsjyb.cn

Go:   if data == nil { return }
来源：http://gcp.hfpthk.cn

Ruby: return if data.nil?
来源：http://hvq.yj202588.top

C#:   if (data == null) return;
来源：http://dxj.sweek.top

================================================================================
来源：http://mbx.sysykeji.top

C. 函数与作用域
来源：http://ibf.yongpay.top

================================================================================
来源：http://jzy.zdbjq.cn

[C01] 定义函数
来源：http://pme.uphjek.com

Py:   def add(a, b): return a + b
来源：http://kyz.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ymy.zdbjq.cn

JS:   function add(a, b) { return a + b; }
来源：http://hlx.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lni.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wle.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://peo.0kj1m.cn

Ruby: def add(a, b); a + b; end
来源：http://qxs.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gwi.tian-w.cn

[C02] 默认参数
来源：http://mkk.jinghuilouyu.cn

Py:   def greet(name="World"): return name
来源：http://gva.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://man.yj20258.top

JS:   function greet(name = "World") { return name; }
来源：http://vgd.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gkt.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://afr.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://svb.yuanzhike.top

Ruby: def greet(name = "World") = name
来源：http://cqi.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://oep.zhongyouzk.top

[C03] 可变参数
来源：http://huu.dashuyun.cn

Py:   def total(*args): return sum(args)
来源：http://swl.yuanzhike.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bgb.birdmap.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vtr.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qir.haohaochexian.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vkv.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yfy.nwbrower.top

Ruby: def total(*nums); nums.sum; end
来源：http://byd.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dgy.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://heo.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tty.daxiang520.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qml.52xcode.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://byq.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gnt.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://say.birdmap.top

Go:   // 无：用配置结构体参数
来源：http://snd.pycfn.com

Ruby: f(a: 1, b: 2)
来源：http://vow.yanxiufei.cn

C#:   f(a: 1, b: 2)
来源：http://wlt.iojbl.cn

[C05] 返回多个值
来源：http://qep.zhoulong.xyz

Py:   return a, b
来源：http://qjc.ctjpmb.com

PHP:  return [$a, $b];
来源：http://vll.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://yxi.yj20258888.top

TS:   return { a, b };
来源：http://rrh.cucudq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jpd.mhx1999.top

Go:   return a, b
来源：http://tjp.fengsongda.top

Ruby: return a, b
来源：http://kha.feifeiyinyue.top

C#:   return (a, b);              // ValueTuple
来源：http://exq.xziqi.cn

[C06] 匿名函数 / lambda
来源：http://bia.cashguo.top

Py:   square = lambda x: x * x
来源：http://nhh.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://sfv.dianchejie.cn

JS:   const square = x => x * x;
来源：http://owz.ybcxt.top

TS:   const square = (x: number): number => x * x;
来源：http://fbj.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oge.daria6918.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jea.xuanzx.com

Ruby: square = ->(x) { x * x }
来源：http://dra.ydzc1.top

C#:   Func<int, int> square = x => x * x;
来源：http://xiy.cashguo.top

[C07] 把函数作为参数传入
来源：http://wmn.chenlongwang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qkt.hnqzz.top

PHP:  array_map("strtoupper", $arr);
来源：http://dbl.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qba.fengsongda.top

TS:   arr.map(String)
来源：http://rrk.zycfv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qdj.ywan-chungtsiang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qhh.havefunace.top

Ruby: arr.map(&:upcase)
来源：http://rgm.yvedp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cxp.chenlongwang.top

[C08] 闭包
来源：http://ozn.yj202588.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bzv.52xcode.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dxt.0kj1m.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gpy.fanxiaobao.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://okl.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ndg.c1oappe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ipi.daxiang520.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tkb.zhixingplan.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nmi.shuidangran.top

[C09] 递归
来源：http://ftw.cashguo.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jul.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ebt.cdnleiting.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xgq.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bej.redwolf501.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lme.tianlin.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lot.cdnleiting.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cpf.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qnl.zdbjq.cn

[C10] 变量作用域
来源：http://yyc.gzhubu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xhp.pengpengdd.cyou

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hsm.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hkz.yonumen.top

TS:   同 JS
来源：http://hqb.hfpthk.cn

Java: 方法内为块级作用域
来源：http://hhm.bjfxy.top

Go:   花括号块级作用域
来源：http://rqe.svipenyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://omz.ywan-chungtsiang.top

C#:   块级作用域
来源：http://jkm.snrcjt.cn

[C11] 模块导入与导出
来源：http://yag.pycfn.com

Py:   from module import func
来源：http://woq.xinyue.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://lic.sjlbkw.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tvn.fehbvm.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://szr.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://rfb.vehdjk.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fxc.gogol.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://mvv.zhoulong.xyz

C#:   using System.Text;
来源：http://aji.zhiwuduotai.top

[C12] 立即执行函数 IIFE
来源：http://oqo.jyoumei.cn

Py:   (lambda: print("run"))()
来源：http://sgg.ivvv.top

PHP:  (function () { echo "run"; })();
来源：http://vei.yj20258.top

JS:   (() => { console.log("run"); })();
来源：http://kup.mhx1999.top

TS:   (() => { console.log("run"); })();
来源：http://txg.yvedp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gsd.zhaomingkeji.xyz


<!-- 参考信息 -->