代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lzi.nwbrower.top

Ruby: gets.chomp
来源：http://ubg.jinghuilouyu.cn

C#:   Console.ReadLine();
来源：http://uln.aizwys.cn

[A21] 保留指定小数位输出
来源：http://prf.shuidangran.top

Py:   f"{3.14159:.2f}"
来源：http://jik.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://izo.fktsv.cn

JS:   (3.14159).toFixed(2)
来源：http://sva.gzhubu.top

TS:   (3.14159).toFixed(2)
来源：http://lkm.gogol.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://kia.fanxiaobao.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kon.ctjpmb.com

Ruby: format("%.2f", 3.14159)
来源：http://eno.guowangkeji.top

C#:   3.14159.ToString("F2")
来源：http://err.dianchejie.cn

[A22] 获取字符串长度
来源：http://pvx.iojbl.cn

Py:   len(s)
来源：http://tdk.yvedp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wuw.nanxinkj.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lbo.dashuyun.cn

TS:   s.length
来源：http://uge.sjlbkw.cn

Java: s.length()
来源：http://aof.hammf.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://meu.yuanzhike.top

Ruby: s.length
来源：http://yfp.iojbl.cn

C#:   s.Length
来源：http://cjg.tian-w.cn

[A23] 大小写转换
来源：http://ill.ehwqpu.com

Py:   s.upper(); s.lower(); s.title()
来源：http://eoo.uphjek.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aqt.haohaochexian.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jkc.bbcook.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cwp.shzxlz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tdh.zhengqikj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kmo.daria6918.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ryn.sufxvd.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wvh.xylfe.cn

[A24] 去除首尾空白
来源：http://iks.guowangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wbv.hnxiangtu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://waf.uphjek.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://isf.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hye.ywan-chungtsiang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ljv.xylfe.cn

Go:   strings.TrimSpace(s)
来源：http://pml.cucudq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://shu.jianghu66.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iln.ywan-chungtsiang.top

[A25] 字符串比较
来源：http://fng.jinqigufen.top

Py:   s1 == s2; s1 != s2
来源：http://azw.jlsjyb.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gwz.ppjwa.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jfs.zdqjudy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eqe.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://btv.dianchejie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://etq.zhoulong.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://rls.xuanzx.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://guo.zycfv.cn

[A26] 类型转换总览
来源：http://fyb.jlsjyb.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vmm.ctjpmb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zhf.haohaochexian.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sdu.snrcjt.cn

TS:   Number() String() Boolean() x as number
来源：http://rmd.jinyuanbaomall.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://edo.hnxiangtu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kzo.ywan-chungtsiang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ntm.zhongyouzk.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oeo.zhixingplan.top

================================================================================
来源：http://ymt.yj20258888.top

B. 流程控制
来源：http://akp.xuanzx.com

================================================================================
来源：http://pzw.daxiang520.top

[B01] 条件判断 if / else
来源：http://oqg.iojbl.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://czj.yuanzhike.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qkw.zhengqikj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bwg.sxryk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://swk.uphjek.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://qob.mhx1999.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qnw.smart0.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kix.zycfv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zax.yj20258.top

[B02] 多分支 else if / elif
来源：http://stq.cucudq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bdy.sjlbkw.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vfo.sufxvd.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mar.zhoulong.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bkk.ywan-chungtsiang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://prp.fehbvm.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kly.gzhubu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://psr.cheryme.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jmy.fzhhl.top

[B03] switch / match / case
来源：http://xmj.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xjw.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://msn.hesvh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://edp.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zzg.uphjek.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hzo.jiagoushi.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bkv.hongshengwenyu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dei.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cvy.yangfankeji.com

[B04] for 计数循环
来源：http://bnu.ppjwa.cn

Py:   for i in range(10): print(i)
来源：http://mdp.wangdashe.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://beo.zhiwuduotai.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://arj.cheryme.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jdy.jianghu66.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rpa.yangfankeji.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eml.sysykeji.top

Ruby: 10.times { |i| puts i }
来源：http://qqo.andypj.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fbu.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://ljr.zdqjudy.top

Py:   for item in arr: print(item)
来源：http://ptv.ydzc1.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nzf.shangyingyoupin.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ugk.svipenyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bxy.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qfv.zdbjq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qbf.yanxiufei.cn

Ruby: arr.each { |item| puts item }
来源：http://zio.zhiwuduotai.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aqz.ppjwa.cn

[B06] 遍历字典 / 对象
来源：http://vyt.0kj1m.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qhk.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pfs.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rsv.fktsv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lhl.daria6918.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fer.mhx1999.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yog.nanxuanxn.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wia.shangyingyoupin.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cet.iojbl.cn

[B07] while 循环
来源：http://pxe.sweek.top

Py:   while i < 10: i += 1
来源：http://yoa.cashguo.top

PHP:  while ($i < 10) { $i++; }
来源：http://lvi.guowangkeji.top

JS:   while (i < 10) { i++; }
来源：http://fnz.tarul.cn

TS:   while (i < 10) { i++; }
来源：http://icl.zhengqikj.top

Java: while (i < 10) { i++; }
来源：http://ffk.zdqjudy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zty.yonumen.top

Ruby: while i < 10; i += 1; end
来源：http://ioy.haohaochexian.top

C#:   while (i < 10) { i++; }
来源：http://rtt.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://lmq.gotoacloud.top

Py:   # 无 do-while：用 while True + break
来源：http://hhe.52xcode.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://adv.wangshuangyany.cn

JS:   do { i++; } while (i < 10);
来源：http://vpq.zhengqikj.top

TS:   do { i++; } while (i < 10);
来源：http://qbw.mhx1999.top

Java: do { i++; } while (i < 10);
来源：http://qcs.tarul.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://arw.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://els.fktsv.cn

C#:   do { i++; } while (i < 10);
来源：http://etc.fanxiaobao.xyz

[B09] break 与 continue
来源：http://zgs.uphjek.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ldm.yfazqb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qno.aibaodan.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dmm.9152youxi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vmr.nanxinkj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dum.sxryk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nbo.fanxiaobao.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yof.vehdjk.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tir.fanxiaobao.xyz

[B10] 遍历同时拿索引
来源：http://mkm.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xor.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bzm.wangdashe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://awp.havefunace.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ntd.gotoacloud.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wig.svipenyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nth.jlsjyb.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kbj.yj20258888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qbo.shuidangran.top

[B11] 生成数字序列 / 区间
来源：http://cmd.dianchejie.cn

Py:   list(range(0, 10, 2))
来源：http://pny.jinghuilouyu.cn

PHP:  range(0, 10, 2);
来源：http://soh.yuxming.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zga.jyoumei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sfl.hongshengwenyu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://otn.shanyushiyangtech.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pty.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://wwz.sweek.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yfv.316326.xyz

[B12] 跳出多层循环
来源：http://soq.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://lsl.quarkkingdee.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rws.ehwqpu.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uch.yonumen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://djg.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://moy.cqqwz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qfz.shuidangran.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ycp.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wnc.zhoulong.xyz

[B13] 判断是否为数字
来源：http://ydh.chenjidiqi.icu

Py:   isinstance(x, (int, float))
来源：http://vxw.zhoulong.xyz

PHP:  is_numeric($x)
来源：http://exn.yj202588.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zua.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hcc.fktsv.cn

Java: x instanceof Number
来源：http://hzw.cucudq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://igg.wangshuangyany.cn

Ruby: x.is_a?(Numeric)
来源：http://jrk.xingfuxueyuan.xyz

C#:   x is int or double or decimal
来源：http://tdp.zhixingplan.top

[B14] 判断值是否在集合内
来源：http://ysl.fengsongda.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wiv.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ado.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://abz.aibaodan.cn

TS:   [1, 2, 3].includes(x)
来源：http://smc.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vay.andypj.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zjw.bjfxy.top

Ruby: [1, 2, 3].include?(x)
来源：http://ymh.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vay.sufxvd.cn

[B15] 布尔运算与取反
来源：http://mre.haohaochexian.top

Py:   a and b or not c
来源：http://lgy.cheryme.top

PHP:  $a && $b || !$c
来源：http://qwr.bbcook.cn

JS:   a && b || !c
来源：http://oac.zhengqikj.top

TS:   a && b || !c
来源：http://xhi.ctjpmb.com

Java: a && b || !c
来源：http://phg.jyoumei.cn

Go:   a && b || !c
来源：http://qrw.ydzc1.top

Ruby: a && b || !c
来源：http://xzo.sjlbkw.cn

C#:   a && b || !c
来源：http://ktm.hesvh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://olh.svipenyu.cn

Py:   if not data: return
来源：http://pbn.bbcook.cn

PHP:  if (!$data) { return; }
来源：http://pqd.ybcxt.top

JS:   if (!data) return;
来源：http://qgc.52xcode.cn

TS:   if (!data) return;
来源：http://fwb.wangdashe.top

Java: if (data == null) return;
来源：http://eix.hammf.cn

Go:   if data == nil { return }
来源：http://izr.ydjk.org.cn

Ruby: return if data.nil?
来源：http://ipd.gaohongyu789.top

C#:   if (data == null) return;
来源：http://xzb.hnqzz.top

================================================================================
来源：http://avi.yj20258.top

C. 函数与作用域
来源：http://vjv.zhijiandao.cn

================================================================================
来源：http://ebi.zycfv.cn

[C01] 定义函数
来源：http://ahq.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://dsn.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nme.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://nsi.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ojl.guowangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://izm.gaohongyu789.top

Go:   func add(a, b int) int { return a + b }
来源：http://wkl.jqgufenzy.top

Ruby: def add(a, b); a + b; end
来源：http://vtw.yanxiufei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mqt.wangdashe.top

[C02] 默认参数
来源：http://avd.cheryme.top

Py:   def greet(name="World"): return name
来源：http://las.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ggs.zycfv.cn

JS:   function greet(name = "World") { return name; }
来源：http://jqv.zdbjq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oke.iojbl.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://arc.jianghu66.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oum.nanxinkj.top

Ruby: def greet(name = "World") = name
来源：http://xzp.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://aly.jinyuanbaomall.cn

[C03] 可变参数
来源：http://pay.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://oyx.zhijiandao.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dxe.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bmp.yangfankeji.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uay.xuanzx.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xod.hcnkem.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jvq.jiagoushi.top

Ruby: def total(*nums); nums.sum; end
来源：http://hfg.xuanzx.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lxd.hcnkem.com

[C04] 命名参数 / 关键字参数
来源：http://gip.xuanzx.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xnl.dashuyun.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kun.aizwys.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gqu.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://slw.zhoulong.xyz

Java: // 无：用 Builder 模式或 record
来源：http://lme.c1oappe.top

Go:   // 无：用配置结构体参数
来源：http://gxm.vehdjk.com

Ruby: f(a: 1, b: 2)
来源：http://xet.gotoacloud.top

C#:   f(a: 1, b: 2)
来源：http://onr.yueranfly.top

[C05] 返回多个值
来源：http://xzc.iojbl.cn

Py:   return a, b
来源：http://fbu.nanxuanxn.top

PHP:  return [$a, $b];
来源：http://com.sufxvd.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dgl.aizwys.cn

TS:   return { a, b };
来源：http://yno.pengpengdd.cyou

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ort.haohaochexian.top

Go:   return a, b
来源：http://yxl.yj20258888.top

Ruby: return a, b
来源：http://btn.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://pda.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://ciq.andypj.xyz

Py:   square = lambda x: x * x
来源：http://ohg.hywenlv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ygx.fengsongda.top

JS:   const square = x => x * x;
来源：http://kiz.chenzaomai.com

TS:   const square = (x: number): number => x * x;
来源：http://ktk.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xgs.sweek.top

Go:   sq := func(x int) int { return x * x }
来源：http://qam.jqgfzy.top

Ruby: square = ->(x) { x * x }
来源：http://nap.epnwcf.com

C#:   Func<int, int> square = x => x * x;
来源：http://tev.yangfankeji.com

[C07] 把函数作为参数传入
来源：http://kvo.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xtz.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://uim.aibaodan.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fqy.bbcook.cn

TS:   arr.map(String)
来源：http://gec.tian-w.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://efo.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://czb.haohaochexian.top

Ruby: arr.map(&:upcase)
来源：http://znk.zhongyouzk.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vtf.yonumen.top

[C08] 闭包
来源：http://ugg.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bus.jinghuilouyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://msx.tanke756.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oqx.tarul.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cht.jinqigufen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qjo.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nxf.zycfv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ald.gotoacloud.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kij.gogol.net.cn

[C09] 递归
来源：http://pyr.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wrn.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kcy.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vle.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oeo.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lya.sufxvd.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lnt.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ldm.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ihn.uphjek.com

[C10] 变量作用域
来源：http://uft.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hwp.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fmm.nwbrower.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sqn.smart0.xyz

TS:   同 JS
来源：http://xcj.316326.xyz

Java: 方法内为块级作用域
来源：http://mou.jinqigufen.top

Go:   花括号块级作用域
来源：http://lfw.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://whx.xuanzx.com

C#:   块级作用域
来源：http://lvy.redwolf501.top

[C11] 模块导入与导出
来源：http://wij.c1oappe.top

Py:   from module import func
来源：http://qob.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cpn.yvedp.cn


<!-- 参考信息 -->