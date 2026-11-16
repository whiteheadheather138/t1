代发 wailian999

JS:   [a, b] = [b, a];
来源：http://paj.aibaodan.cn

TS:   [a, b] = [b, a];
来源：http://kaw.cucudq.cn

Java: int t = a; a = b; b = t;
来源：http://mnl.gotoacloud.top

Go:   a, b = b, a
来源：http://nwu.quarkkingdee.top

Ruby: a, b = b, a
来源：http://buf.yueranfly.top

C#:   (a, b) = (b, a);
来源：http://gzt.dianchejie.cn

[A20] 读取标准输入
来源：http://keu.cqqwz.cn

Py:   name = input("请输入：")
来源：http://gai.hnxiangtu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://cqk.bjfxy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://iig.zycfv.cn

TS:   // Node.js：readline 模块
来源：http://ygo.ydjk.org.cn

Java: new Scanner(System.in).nextLine()
来源：http://kmt.hnxiangtu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xzd.9152youxi.cn

Ruby: gets.chomp
来源：http://ham.jinqigfzy.top

C#:   Console.ReadLine();
来源：http://bzw.gaohongyu789.top

[A21] 保留指定小数位输出
来源：http://mgn.cdnleiting.top

Py:   f"{3.14159:.2f}"
来源：http://uph.zhixingplan.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yom.vqdsnc.cn

JS:   (3.14159).toFixed(2)
来源：http://exf.birdmap.top

TS:   (3.14159).toFixed(2)
来源：http://urq.havefunace.top

Java: String.format("%.2f", 3.14159)
来源：http://iny.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wrr.52xcode.cn

Ruby: format("%.2f", 3.14159)
来源：http://ado.chenzaomai.com

C#:   3.14159.ToString("F2")
来源：http://ube.zycfv.cn

[A22] 获取字符串长度
来源：http://yjk.fengsongda.top

Py:   len(s)
来源：http://cbx.andypj.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wjj.yueranfly.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://err.dianchejie.cn

TS:   s.length
来源：http://nxz.yuanzhike.top

Java: s.length()
来源：http://war.c1oappe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hec.chenjidiqi.icu

Ruby: s.length
来源：http://vso.yuanzhike.top

C#:   s.Length
来源：http://acn.ctjpmb.com

[A23] 大小写转换
来源：http://dtx.jinyuanbaomall.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://osy.daxiang520.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kqv.zhiwuduotai.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nuo.wangdashe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hkx.yj20258.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zma.pycfn.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qfr.aibaodan.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vry.ctjpmb.com

C#:   s.ToUpper(); s.ToLower()
来源：http://giv.andypj.xyz

[A24] 去除首尾空白
来源：http://hml.ehwqpu.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ssv.jinghuilouyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sta.kuanghao11.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gpn.jinyuanbaomall.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wtr.jinghuilouyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vqv.yj202588.top

Go:   strings.TrimSpace(s)
来源：http://lxe.ppjwa.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eli.tanke756.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://diq.ppjwa.cn

[A25] 字符串比较
来源：http://mbp.yongpay.top

Py:   s1 == s2; s1 != s2
来源：http://hkm.iojbl.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://egg.ivvv.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://huo.52xcode.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.nanxuanxn.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ihl.snrcjt.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nhk.yj20258888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ayc.zdbjq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vxl.jlsjyb.cn

[A26] 类型转换总览
来源：http://pcj.iojbl.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tvn.zdbjq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yxl.bbcook.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://igl.havefunace.top

TS:   Number() String() Boolean() x as number
来源：http://hrn.jqgufenzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://van.jlsjyb.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://frp.fengsongda.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dot.sysykeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rjo.mhx1999.top

================================================================================
来源：http://ern.sjlbkw.cn

B. 流程控制
来源：http://eqc.haohaochexian.top

================================================================================
来源：http://lcs.ctjpmb.com

[B01] 条件判断 if / else
来源：http://tgi.ivvv.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cki.epnwcf.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ycs.daxiang520.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aab.bjfxy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://glb.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lnz.hywenlv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qgb.zhixingplan.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://deo.chenjidiqi.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qdx.zhaomingkeji.xyz

[B02] 多分支 else if / elif
来源：http://kra.gzhubu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gmk.jqgfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ycz.sjlbkw.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dgn.chenlongwang.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bvf.cqqwz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xkq.chenzaomai.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bur.andypj.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mzi.zhengqikj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://upq.xuanzx.com

[B03] switch / match / case
来源：http://oqi.yuxming.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ppr.gogol.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://far.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jdh.ppjwa.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jci.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dqx.dashuyun.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ppr.yfazqb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zxn.sysykeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dwm.shanyushiyangtech.top

[B04] for 计数循环
来源：http://qub.ybcxt.top

Py:   for i in range(10): print(i)
来源：http://wzr.iojbl.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dcd.pycfn.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tlh.hywenlv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yio.jiagoushi.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kin.cucudq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mrp.52xcode.cn

Ruby: 10.times { |i| puts i }
来源：http://qce.52xcode.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ulj.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://oai.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://bfk.fzhhl.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cjn.bjfxy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kag.cdnleiting.top

TS:   for (const item of arr) { console.log(item); }
来源：http://luk.ydjk.org.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nrh.yj202588.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jtp.cqqwz.cn

Ruby: arr.each { |item| puts item }
来源：http://jwo.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xnp.chenzaomai.com

[B06] 遍历字典 / 对象
来源：http://zdk.zhongyouzk.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pgd.sxryk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rum.tian-w.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tzs.zhaomingkeji.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mwg.cashguo.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lpp.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://odc.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sdz.andypj.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ele.hammf.cn

[B07] while 循环
来源：http://ujq.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://ruu.tarul.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ous.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://mdh.yueranfly.top

TS:   while (i < 10) { i++; }
来源：http://fzr.hfpthk.cn

Java: while (i < 10) { i++; }
来源：http://ojj.52xcode.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ebm.shanyushiyangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://gkp.daria6918.cn

C#:   while (i < 10) { i++; }
来源：http://hrs.birdmap.top

[B08] do-while（至少执行一次）
来源：http://hjx.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://lgw.cheryme.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wet.nwbrower.top

JS:   do { i++; } while (i < 10);
来源：http://oqc.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://avr.zdbjq.cn

Java: do { i++; } while (i < 10);
来源：http://kjb.hammf.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uxz.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://afo.sysykeji.top

C#:   do { i++; } while (i < 10);
来源：http://wut.redwolf501.top

[B09] break 与 continue
来源：http://tea.vehdjk.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bwc.xingfuxueyuan.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kqp.shangyingyoupin.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rqf.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kkp.yonumen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zkb.cqqwz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zsu.hongshengwenyu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ykc.ivvv.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://muj.ydjk.org.cn

[B10] 遍历同时拿索引
来源：http://ykl.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://apx.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rfs.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bze.zhoulong.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uwv.yj20258.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jbw.wangdashe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dtn.yfazqb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://isk.jlsjyb.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jkp.haohaochexian.top

[B11] 生成数字序列 / 区间
来源：http://puu.yangfankeji.com

Py:   list(range(0, 10, 2))
来源：http://rjn.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://mrn.zhongyouzk.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ekd.redwolf501.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yvc.ppjwa.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cvh.yj20258888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wpz.tarul.cn

Ruby: (0...10).step(2).to_a
来源：http://azt.sweek.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ezr.sxryk.cn

[B12] 跳出多层循环
来源：http://oft.chenlongwang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wzv.hongshengwenyu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hpg.ivvv.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eep.gotoacloud.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nlx.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jef.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://klp.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zwn.redwolf501.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wya.ydjk.org.cn

[B13] 判断是否为数字
来源：http://zns.shanyushiyangtech.top

Py:   isinstance(x, (int, float))
来源：http://gnc.smart0.xyz

PHP:  is_numeric($x)
来源：http://wgl.9152youxi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xen.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xos.ehwqpu.com

Java: x instanceof Number
来源：http://jyc.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nxc.aibaodan.cn

Ruby: x.is_a?(Numeric)
来源：http://bnr.cdnleiting.top

C#:   x is int or double or decimal
来源：http://hgt.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://kfn.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://alg.hysaishi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uzv.yvedp.cn

JS:   [1, 2, 3].includes(x)
来源：http://ajf.316326.xyz

TS:   [1, 2, 3].includes(x)
来源：http://yxv.andypj.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://cbf.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yyj.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://igd.zhongyouzk.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oim.shanyushiyangkeji.top

[B15] 布尔运算与取反
来源：http://inm.cheryme.top

Py:   a and b or not c
来源：http://dah.andypj.xyz

PHP:  $a && $b || !$c
来源：http://qaz.9152youxi.cn

JS:   a && b || !c
来源：http://jxc.hcnkem.com

TS:   a && b || !c
来源：http://oia.sweek.top

Java: a && b || !c
来源：http://xxj.yonumen.top

Go:   a && b || !c
来源：http://cxw.gzhubu.top

Ruby: a && b || !c
来源：http://fej.ivvv.top

C#:   a && b || !c
来源：http://cld.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wvh.zhengqikj.top

Py:   if not data: return
来源：http://avk.yuxming.cn

PHP:  if (!$data) { return; }
来源：http://ixi.0kj1m.cn

JS:   if (!data) return;
来源：http://gfi.chenjidiqi.icu

TS:   if (!data) return;
来源：http://cnm.wangdashe.top

Java: if (data == null) return;
来源：http://ewy.zdqjudy.top

Go:   if data == nil { return }
来源：http://uwd.yangfankeji.com

Ruby: return if data.nil?
来源：http://npt.zhiwuduotai.top

C#:   if (data == null) return;
来源：http://xrk.gzhubu.top

================================================================================
来源：http://fyz.shzxlz.cn

C. 函数与作用域
来源：http://azv.chenjidiqi.icu

================================================================================
来源：http://lrp.ivvv.top

[C01] 定义函数
来源：http://zwm.nanxuanxn.top

Py:   def add(a, b): return a + b
来源：http://vjx.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dak.tarul.cn

JS:   function add(a, b) { return a + b; }
来源：http://lel.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nlv.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ubt.pycfn.com

Go:   func add(a, b int) int { return a + b }
来源：http://bsf.vqdsnc.cn

Ruby: def add(a, b); a + b; end
来源：http://mwy.nanxuanxn.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ixa.gotoacloud.top

[C02] 默认参数
来源：http://suj.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://psf.snrcjt.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mzg.tian-w.cn

JS:   function greet(name = "World") { return name; }
来源：http://moc.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hqr.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://olf.fehbvm.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://igs.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://mfq.xingfuxueyuan.xyz

C#:   string Greet(string name = "World") => name;
来源：http://xzi.jlsjyb.cn

[C03] 可变参数
来源：http://goy.ppjwa.cn

Py:   def total(*args): return sum(args)
来源：http://vdc.fzhhl.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://elu.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://slv.bjfxy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wna.daria6918.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hfa.quarkkingdee.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bya.jqgfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://tvr.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://phq.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://dkf.xingfuxueyuan.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iin.iojbl.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cqm.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wih.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xna.zhijiandao.cn

Java: // 无：用 Builder 模式或 record
来源：http://zjz.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://jmn.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://hup.ctjpmb.com

C#:   f(a: 1, b: 2)
来源：http://nah.gzhubu.top

[C05] 返回多个值
来源：http://mgq.sweek.top

Py:   return a, b
来源：http://uzg.havefunace.top

PHP:  return [$a, $b];
来源：http://xgb.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://msr.cqqwz.cn

TS:   return { a, b };
来源：http://iox.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qjb.aibaodan.cn

Go:   return a, b
来源：http://ubs.zhengqikj.top

Ruby: return a, b
来源：http://ctw.hnxiangtu.top

C#:   return (a, b);              // ValueTuple
来源：http://hkx.xingfuxueyuan.xyz

[C06] 匿名函数 / lambda
来源：http://xom.9152youxi.cn

Py:   square = lambda x: x * x
来源：http://tww.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://yxn.jinqigufen.top

JS:   const square = x => x * x;
来源：http://ifs.shangyingyoupin.top

TS:   const square = (x: number): number => x * x;
来源：http://zei.zhengqikj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://juc.52xcode.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wrc.fzhhl.top

Ruby: square = ->(x) { x * x }
来源：http://quj.xuetiantiany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xzs.redwolf501.top

[C07] 把函数作为参数传入
来源：http://wrm.sweek.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dsn.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://lja.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dyv.yj20258888.top

TS:   arr.map(String)
来源：http://icx.epnwcf.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xcp.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fff.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://cat.52xcode.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://orn.hysaishi.cn

[C08] 闭包
来源：http://mrs.nanxinkj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ojm.daria6918.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zxi.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://etl.gogol.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ism.zhijiandao.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xen.nanxinkj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fhb.dianchejie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://epg.chenzaomai.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jsy.sxryk.cn

[C09] 递归
来源：http://nzq.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aba.quarkkingdee.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sas.316326.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nta.quarkkingdee.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fkf.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xvc.guowangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bvl.andypj.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ujd.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qqn.vehdjk.com


<!-- 参考信息 -->