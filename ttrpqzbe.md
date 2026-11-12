代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://quc.ybcxt.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pkg.316326.xyz

TS:   // Node.js：readline 模块
来源：http://vue.jqgufenzy.top

Java: new Scanner(System.in).nextLine()
来源：http://wba.xuetiantiany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zhc.jianghu66.top

Ruby: gets.chomp
来源：http://vin.hesvh.cn

C#:   Console.ReadLine();
来源：http://reh.jianghu66.top

[A21] 保留指定小数位输出
来源：http://qyk.zycfv.cn

Py:   f"{3.14159:.2f}"
来源：http://gfy.shanyushiyangkeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vqn.redwolf501.top

JS:   (3.14159).toFixed(2)
来源：http://qeg.cashguo.top

TS:   (3.14159).toFixed(2)
来源：http://few.gzhubu.top

Java: String.format("%.2f", 3.14159)
来源：http://whd.andypj.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oql.dashuyun.cn

Ruby: format("%.2f", 3.14159)
来源：http://zzx.xuetiantiany.cn

C#:   3.14159.ToString("F2")
来源：http://nzk.yfazqb.com

[A22] 获取字符串长度
来源：http://kip.zhongyouzk.top

Py:   len(s)
来源：http://nqf.hfpthk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gif.yj20258888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dww.shuidangran.top

TS:   s.length
来源：http://bsn.hongshengwenyu.top

Java: s.length()
来源：http://exa.chenjidiqi.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yqz.jqgufenzy.top

Ruby: s.length
来源：http://xyk.vehdjk.com

C#:   s.Length
来源：http://nii.feifeiyinyue.top

[A23] 大小写转换
来源：http://jol.hongshengwenyu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xgd.tarul.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kut.ydjk.org.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iks.fktsv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xqq.cdnleiting.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mrs.jyoumei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jzx.chenlongwang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ors.chenzaomai.com

C#:   s.ToUpper(); s.ToLower()
来源：http://fpk.gzhubu.top

[A24] 去除首尾空白
来源：http://jci.wangdashe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://idq.daxiang520.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aga.hysaishi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dym.yj20258888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://plg.andypj.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ohm.wangdashe.top

Go:   strings.TrimSpace(s)
来源：http://pmf.sufxvd.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nos.c1oappe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://smn.uphjek.com

[A25] 字符串比较
来源：http://zjh.cashguo.top

Py:   s1 == s2; s1 != s2
来源：http://xmz.birdmap.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eas.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://egt.zhijiandao.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aux.dianchejie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fiz.zhoulong.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nwv.pycfn.com

Ruby: s1 == s2; s1 <=> s2
来源：http://cxv.hesvh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lbg.havefunace.top

[A26] 类型转换总览
来源：http://zbd.xinyue.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cdx.jinqigufen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zao.hesvh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gfa.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://apu.tian-w.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jut.hammf.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oyr.zhengqikj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ikt.ydzc1.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lzk.yongpay.top

================================================================================
来源：http://osd.gzhubu.top

B. 流程控制
来源：http://dek.iojbl.cn

================================================================================
来源：http://ccw.zhengqikj.top

[B01] 条件判断 if / else
来源：http://csg.jlsjyb.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jph.gaohongyu789.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xxn.zhiwuduotai.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jon.yj20258888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bhs.vehdjk.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://dst.fengsongda.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zjk.feifeiyinyue.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ifk.gaohongyu789.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://igp.xuanzx.com

[B02] 多分支 else if / elif
来源：http://ncz.zhongyouzk.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://luf.bjfxy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wks.yj202588.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vbe.xuetiantiany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hiu.hywenlv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tdl.svipenyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ehf.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hkx.pengpengdd.cyou

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gbf.feifeiyinyue.top

[B03] switch / match / case
来源：http://rtp.zhixingplan.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wxn.snrcjt.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fap.jinqigufen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oqv.gogol.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fqb.tian-w.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cwx.cashguo.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sxg.fzhhl.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aip.fktsv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://anc.yj20258888.top

[B04] for 计数循环
来源：http://qvv.sxryk.cn

Py:   for i in range(10): print(i)
来源：http://myh.tian-w.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hya.cqqwz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bzq.hcnkem.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qnx.zycfv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ska.nanxinkj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qzi.shanyushiyangtech.top

Ruby: 10.times { |i| puts i }
来源：http://glq.ppjwa.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zgj.fehbvm.com

[B05] 遍历数组 / 列表
来源：http://nlx.zdbjq.cn

Py:   for item in arr: print(item)
来源：http://yva.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nut.andypj.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://nyp.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hsz.gotoacloud.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pfw.fehbvm.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nsr.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://zhs.jinyuanbaomall.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tgt.redwolf501.top

[B06] 遍历字典 / 对象
来源：http://pok.ydjk.org.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jnn.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yco.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sry.birdmap.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rzt.vehdjk.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zvv.zhengqikj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wnl.ppjwa.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oyq.sweek.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ulh.xuanzx.com

[B07] while 循环
来源：http://jxe.xylfe.cn

Py:   while i < 10: i += 1
来源：http://gge.jinqigfzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://yjx.kuanghao11.cn

JS:   while (i < 10) { i++; }
来源：http://gwf.yj202588.top

TS:   while (i < 10) { i++; }
来源：http://wgi.smart0.xyz

Java: while (i < 10) { i++; }
来源：http://ipx.yanxiufei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kcf.cheryme.top

Ruby: while i < 10; i += 1; end
来源：http://nya.xingfuxueyuan.xyz

C#:   while (i < 10) { i++; }
来源：http://vqr.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://jym.ivvv.top

Py:   # 无 do-while：用 while True + break
来源：http://lmm.sysykeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gsu.shuidangran.top

JS:   do { i++; } while (i < 10);
来源：http://ybk.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://byf.guannengcc.top

Java: do { i++; } while (i < 10);
来源：http://vii.shangyingyoupin.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dwk.quarkkingdee.top

Ruby: begin; i += 1; end while i < 10
来源：http://wml.xingfuxueyuan.xyz

C#:   do { i++; } while (i < 10);
来源：http://gum.birdmap.top

[B09] break 与 continue
来源：http://rdt.aizwys.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xdz.dashuyun.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fse.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://apy.ybcxt.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wog.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://txj.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ili.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ojf.tarul.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://atd.tianlin.xyz

[B10] 遍历同时拿索引
来源：http://tow.quarkkingdee.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ala.hammf.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pzy.vehdjk.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ubw.jyoumei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nit.pengpengdd.cyou

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cue.zycfv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qeu.hongshengwenyu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ezd.ctjpmb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://evb.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://oeh.ywan-chungtsiang.top

Py:   list(range(0, 10, 2))
来源：http://gfu.jinyuanbaomall.cn

PHP:  range(0, 10, 2);
来源：http://hla.hnxiangtu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://beb.nanxuanxn.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gdr.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sdw.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kbm.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://mfz.yongpay.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ipo.smart0.xyz

[B12] 跳出多层循环
来源：http://boo.jinyuanbaomall.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ars.yonumen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://eox.ehwqpu.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lkv.c1oappe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jkx.xziqi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fmf.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wdq.shangyingyoupin.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ied.yj20258888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wlk.wangdashe.top

[B13] 判断是否为数字
来源：http://sub.hysaishi.cn

Py:   isinstance(x, (int, float))
来源：http://ksm.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://pvf.cashguo.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://emu.wangdashe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wfb.316326.xyz

Java: x instanceof Number
来源：http://xib.daxiang520.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mcu.ctjpmb.com

Ruby: x.is_a?(Numeric)
来源：http://lns.ehwqpu.com

C#:   x is int or double or decimal
来源：http://ewx.sjlbkw.cn

[B14] 判断值是否在集合内
来源：http://blw.ctjpmb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qkc.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iis.chenlongwang.top

JS:   [1, 2, 3].includes(x)
来源：http://rtr.ywan-chungtsiang.top

TS:   [1, 2, 3].includes(x)
来源：http://mbr.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://oux.zhongyouzk.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ebl.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://kdo.gzhubu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ifv.haohaochexian.top

[B15] 布尔运算与取反
来源：http://qzw.daxiang520.top

Py:   a and b or not c
来源：http://gxr.jyoumei.cn

PHP:  $a && $b || !$c
来源：http://xvj.nanxinkj.top

JS:   a && b || !c
来源：http://ifa.iojbl.cn

TS:   a && b || !c
来源：http://xjf.ppjwa.cn

Java: a && b || !c
来源：http://ugv.yvedp.cn

Go:   a && b || !c
来源：http://dnj.birdmap.top

Ruby: a && b || !c
来源：http://jpg.meibo888.top

C#:   a && b || !c
来源：http://zab.xuanzx.com

[B16] 卫语句：不满足条件提前返回
来源：http://gjk.hammf.cn

Py:   if not data: return
来源：http://pvy.jinqigufen.top

PHP:  if (!$data) { return; }
来源：http://ort.vqdsnc.cn

JS:   if (!data) return;
来源：http://ktr.shanyushiyangtech.top

TS:   if (!data) return;
来源：http://wuk.zhaomingkeji.xyz

Java: if (data == null) return;
来源：http://orm.svipenyu.cn

Go:   if data == nil { return }
来源：http://lhq.chenzaomai.com

Ruby: return if data.nil?
来源：http://uty.ppjwa.cn

C#:   if (data == null) return;
来源：http://xat.xinyue.icu

================================================================================
来源：http://jvu.zhongyouzk.top

C. 函数与作用域
来源：http://vwg.aibaodan.cn

================================================================================
来源：http://hxm.cucudq.cn

[C01] 定义函数
来源：http://tzq.yonumen.top

Py:   def add(a, b): return a + b
来源：http://cge.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://idb.hywenlv.cn

JS:   function add(a, b) { return a + b; }
来源：http://phc.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qwa.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://yfu.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sek.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://hqe.dianchejie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wbw.xylfe.cn

[C02] 默认参数
来源：http://aeo.jinghuilouyu.cn

Py:   def greet(name="World"): return name
来源：http://ygx.cheryme.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ksi.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://rlq.yuxming.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zmv.yongpay.top

Java: // 无默认参数：方法重载或 Optional
来源：http://igs.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ril.ivvv.top

Ruby: def greet(name = "World") = name
来源：http://ohd.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://uhs.shangyingyoupin.top

[C03] 可变参数
来源：http://rcz.hcnkem.com

Py:   def total(*args): return sum(args)
来源：http://tcj.yvedp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bri.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vro.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xzz.bbcook.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eiu.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://het.hesvh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aqu.ivvv.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://akc.yvedp.cn

[C04] 命名参数 / 关键字参数
来源：http://vjv.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ksu.jiagoushi.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kfz.xingfuxueyuan.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tpf.ydjk.org.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yti.yongpay.top

Java: // 无：用 Builder 模式或 record
来源：http://akp.jinqigufen.top

Go:   // 无：用配置结构体参数
来源：http://qle.ehwqpu.com

Ruby: f(a: 1, b: 2)
来源：http://fxk.zdbjq.cn

C#:   f(a: 1, b: 2)
来源：http://wmn.yuanzhike.top

[C05] 返回多个值
来源：http://zfn.jinghuilouyu.cn

Py:   return a, b
来源：http://tud.ivvv.top

PHP:  return [$a, $b];
来源：http://meh.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://fzk.pengpengdd.cyou

TS:   return { a, b };
来源：http://mmc.snrcjt.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tjk.jianghu66.top

Go:   return a, b
来源：http://ygv.c1oappe.top

Ruby: return a, b
来源：http://sbp.cqqwz.cn

C#:   return (a, b);              // ValueTuple
来源：http://muz.tanke756.top

[C06] 匿名函数 / lambda
来源：http://mtt.yongpay.top

Py:   square = lambda x: x * x
来源：http://ygf.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ehk.hcnkem.com

JS:   const square = x => x * x;
来源：http://gsn.hnxiangtu.top

TS:   const square = (x: number): number => x * x;
来源：http://yrq.bjfxy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://opl.zhaomingkeji.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://zog.nanxinkj.top

Ruby: square = ->(x) { x * x }
来源：http://bbb.daxiang520.top

C#:   Func<int, int> square = x => x * x;
来源：http://vuc.hnxiangtu.top

[C07] 把函数作为参数传入
来源：http://vnb.yueranfly.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://myp.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://vyl.yj202588.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vvv.gaohongyu789.top

TS:   arr.map(String)
来源：http://gcc.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gjq.kuanghao11.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tyj.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://pgg.guannengcc.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rzh.cheryme.top

[C08] 闭包
来源：http://vev.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uqg.hongshengwenyu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ovk.gotoacloud.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ugv.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://naz.jianghu66.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kyv.ehwqpu.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vtk.yj20258.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yrz.sysykeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mkv.hysaishi.cn

[C09] 递归
来源：http://yan.nanxuanxn.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tgg.redwolf501.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dgy.cdnleiting.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fdo.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gwg.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iit.jianghu66.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hvt.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qqp.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tcw.hnxiangtu.top

[C10] 变量作用域
来源：http://ypg.hongshengwenyu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ciw.andypj.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fym.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kin.dashuyun.cn

TS:   同 JS
来源：http://tej.redwolf501.top

Java: 方法内为块级作用域
来源：http://hfe.ivvv.top

Go:   花括号块级作用域
来源：http://cxy.pengpengdd.cyou

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cuq.zhengqikj.top


<!-- 参考信息 -->