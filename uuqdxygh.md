代发 wailian999

JS:   [a, b] = [b, a];
来源：http://ggb.yfazqb.com

TS:   [a, b] = [b, a];
来源：http://hww.snrcjt.cn

Java: int t = a; a = b; b = t;
来源：http://bcg.hysaishi.cn

Go:   a, b = b, a
来源：http://ncn.hfpthk.cn

Ruby: a, b = b, a
来源：http://qnw.cheryme.top

C#:   (a, b) = (b, a);
来源：http://ouq.chenzaomai.com

[A20] 读取标准输入
来源：http://nkk.yuanzhike.top

Py:   name = input("请输入：")
来源：http://mdi.zhixingplan.top

PHP:  $name = trim(fgets(STDIN));
来源：http://sjk.pengpengdd.cyou

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ivf.chenzaomai.com

TS:   // Node.js：readline 模块
来源：http://xpx.xinyue.icu

Java: new Scanner(System.in).nextLine()
来源：http://xlv.ydzc1.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zfm.iojbl.cn

Ruby: gets.chomp
来源：http://msw.feifeiyinyue.top

C#:   Console.ReadLine();
来源：http://vcf.yvedp.cn

[A21] 保留指定小数位输出
来源：http://uub.ydzc1.top

Py:   f"{3.14159:.2f}"
来源：http://gyk.jinghuilouyu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bkw.sweek.top

JS:   (3.14159).toFixed(2)
来源：http://fnd.xylfe.cn

TS:   (3.14159).toFixed(2)
来源：http://prh.xingfuxueyuan.xyz

Java: String.format("%.2f", 3.14159)
来源：http://iym.0kj1m.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zxx.nanxuanxn.top

Ruby: format("%.2f", 3.14159)
来源：http://ddy.sysykeji.top

C#:   3.14159.ToString("F2")
来源：http://dan.pycfn.com

[A22] 获取字符串长度
来源：http://gsu.ydzc1.top

Py:   len(s)
来源：http://asl.vehdjk.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://luy.feifeiyinyue.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ddp.fengsongda.top

TS:   s.length
来源：http://eus.hcnkem.com

Java: s.length()
来源：http://sfy.jqgufenzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dwf.xylfe.cn

Ruby: s.length
来源：http://kau.zhongyouzk.top

C#:   s.Length
来源：http://lcy.guowangkeji.top

[A23] 大小写转换
来源：http://xnm.vqdsnc.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wkn.kuanghao11.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fxy.hnxiangtu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qof.zhaomingkeji.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ojv.daria6918.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zuw.hongshengwenyu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ioc.yongpay.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tgw.jinyuanbaomall.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hgw.chenlongwang.top

[A24] 去除首尾空白
来源：http://ive.sxryk.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jle.pengpengdd.cyou

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rwy.shanyushiyangtech.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wgh.hfpthk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://poh.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://goa.zhongyouzk.top

Go:   strings.TrimSpace(s)
来源：http://zqw.gzhubu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ydo.ppjwa.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://neq.guannengcc.top

[A25] 字符串比较
来源：http://yms.jqgufenzy.top

Py:   s1 == s2; s1 != s2
来源：http://tar.sysykeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bdk.iojbl.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qov.meibo888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pjr.yj20258.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hob.sjlbkw.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tsn.sjlbkw.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xto.sysykeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xlb.jianghu66.top

[A26] 类型转换总览
来源：http://jxj.bbcook.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://paq.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hfn.jlsjyb.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mug.shanyushiyangtech.top

TS:   Number() String() Boolean() x as number
来源：http://gbr.iojbl.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hhg.jinghuilouyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sqk.jinqigfzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://led.52xcode.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gnb.dashuyun.cn

================================================================================
来源：http://bfo.yueranfly.top

B. 流程控制
来源：http://yrq.hywenlv.cn

================================================================================
来源：http://crc.nwbrower.top

[B01] 条件判断 if / else
来源：http://fca.aibaodan.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ula.zdqjudy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://log.yongpay.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dao.ehwqpu.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xfg.ehwqpu.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://foq.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nsv.daxiang520.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qyt.yangfankeji.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lmo.shangyingyoupin.top

[B02] 多分支 else if / elif
来源：http://enk.vqdsnc.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wff.meibo888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cqf.sweek.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oxu.hcnkem.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hkw.nanxuanxn.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eek.gzhubu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yrz.cqqwz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xfc.yuxming.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ioi.chenlongwang.top

[B03] switch / match / case
来源：http://ntj.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ikn.bbcook.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rak.ybcxt.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fke.xuetiantiany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mah.iojbl.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bbu.zhijiandao.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qva.zhiwuduotai.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cqu.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jha.kuanghao11.cn

[B04] for 计数循环
来源：http://wrf.jqgfzy.top

Py:   for i in range(10): print(i)
来源：http://lah.zdqjudy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cks.ppjwa.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vdp.daxiang520.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zty.wangshuangyany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://brm.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://whq.yongpay.top

Ruby: 10.times { |i| puts i }
来源：http://sib.yueranfly.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zen.cheryme.top

[B05] 遍历数组 / 列表
来源：http://mpj.zdqjudy.top

Py:   for item in arr: print(item)
来源：http://qwc.yanxiufei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hcn.havefunace.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ybw.dashuyun.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yym.tanke756.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://lqh.cashguo.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fwm.9152youxi.cn

Ruby: arr.each { |item| puts item }
来源：http://esd.jqgufenzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wkp.zhiwuduotai.top

[B06] 遍历字典 / 对象
来源：http://jzq.zhixingplan.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qwz.xingfuxueyuan.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qkz.birdmap.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lrf.shuidangran.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iap.jqgfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://erz.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jox.yuxming.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bdx.zhaomingkeji.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dlz.sufxvd.cn

[B07] while 循环
来源：http://lvl.uphjek.com

Py:   while i < 10: i += 1
来源：http://uyv.zhongyouzk.top

PHP:  while ($i < 10) { $i++; }
来源：http://vtm.jqgfzy.top

JS:   while (i < 10) { i++; }
来源：http://gcj.jqgfzy.top

TS:   while (i < 10) { i++; }
来源：http://kcy.nanxuanxn.top

Java: while (i < 10) { i++; }
来源：http://ibm.chenzaomai.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xox.bbcook.cn

Ruby: while i < 10; i += 1; end
来源：http://kfo.aizwys.cn

C#:   while (i < 10) { i++; }
来源：http://ohm.cqqwz.cn

[B08] do-while（至少执行一次）
来源：http://atr.hesvh.cn

Py:   # 无 do-while：用 while True + break
来源：http://kdm.fktsv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mnh.yvedp.cn

JS:   do { i++; } while (i < 10);
来源：http://gug.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://prv.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://rgb.chenzaomai.com

Go:   for { i++; if i >= 10 { break } }
来源：http://ooq.cqqwz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ksy.svipenyu.cn

C#:   do { i++; } while (i < 10);
来源：http://ybw.zhengqikj.top

[B09] break 与 continue
来源：http://yvf.yongpay.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hju.ppjwa.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lil.ydjk.org.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ogo.svipenyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wlo.fanxiaobao.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yhr.ivvv.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bux.ehwqpu.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lju.fktsv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kns.pengpengdd.cyou

[B10] 遍历同时拿索引
来源：http://yvq.gzhubu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qmp.guannengcc.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kdt.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pkt.ivvv.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lua.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://khp.smart0.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cvl.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pwo.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://exf.zdbjq.cn

[B11] 生成数字序列 / 区间
来源：http://tud.zycfv.cn

Py:   list(range(0, 10, 2))
来源：http://ndr.nanxuanxn.top

PHP:  range(0, 10, 2);
来源：http://fsb.zhixingplan.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mpg.sjlbkw.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ynl.aizwys.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uzy.jlsjyb.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xor.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://agp.yongpay.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aka.hesvh.cn

[B12] 跳出多层循环
来源：http://sst.xingfuxueyuan.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://lxq.jyoumei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tfd.yonumen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://acc.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xyd.cheryme.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yyi.yj20258888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tfq.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pxk.sysykeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ouy.tarul.cn

[B13] 判断是否为数字
来源：http://zjq.ydjk.org.cn

Py:   isinstance(x, (int, float))
来源：http://aro.gotoacloud.top

PHP:  is_numeric($x)
来源：http://vfq.pengpengdd.cyou

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nzs.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yby.ctjpmb.com

Java: x instanceof Number
来源：http://cxx.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://obv.ydzc1.top

Ruby: x.is_a?(Numeric)
来源：http://gvi.cashguo.top

C#:   x is int or double or decimal
来源：http://iou.kuanghao11.cn

[B14] 判断值是否在集合内
来源：http://ggk.ydjk.org.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vrt.aibaodan.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fji.cqqwz.cn

JS:   [1, 2, 3].includes(x)
来源：http://hkd.tanke756.top

TS:   [1, 2, 3].includes(x)
来源：http://afb.ehwqpu.com

Java: List.of(1, 2, 3).contains(x)
来源：http://uuy.sweek.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zzv.sxryk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rzl.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vbo.nwbrower.top

[B15] 布尔运算与取反
来源：http://klu.ppjwa.cn

Py:   a and b or not c
来源：http://oyt.fehbvm.com

PHP:  $a && $b || !$c
来源：http://owu.zhengqikj.top

JS:   a && b || !c
来源：http://csn.ywan-chungtsiang.top

TS:   a && b || !c
来源：http://pwe.tanke756.top

Java: a && b || !c
来源：http://zok.haohaochexian.top

Go:   a && b || !c
来源：http://nap.chenlongwang.top

Ruby: a && b || !c
来源：http://yzz.jyoumei.cn

C#:   a && b || !c
来源：http://hwa.yj202588.top

[B16] 卫语句：不满足条件提前返回
来源：http://ibe.wangshuangyany.cn

Py:   if not data: return
来源：http://lpl.zhoulong.xyz

PHP:  if (!$data) { return; }
来源：http://rlj.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://sah.jqgfzy.top

TS:   if (!data) return;
来源：http://lro.cheryme.top

Java: if (data == null) return;
来源：http://bap.snrcjt.cn

Go:   if data == nil { return }
来源：http://fns.cheryme.top

Ruby: return if data.nil?
来源：http://rrh.shuidangran.top

C#:   if (data == null) return;
来源：http://pga.jinghuilouyu.cn

================================================================================
来源：http://xci.ivvv.top

C. 函数与作用域
来源：http://bey.nwbrower.top

================================================================================
来源：http://aod.bbcook.cn

[C01] 定义函数
来源：http://mas.iojbl.cn

Py:   def add(a, b): return a + b
来源：http://ntn.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jal.jlsjyb.cn

JS:   function add(a, b) { return a + b; }
来源：http://dob.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pdb.yanxiufei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rrs.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ujc.tianlin.xyz

Ruby: def add(a, b); a + b; end
来源：http://dgt.vqdsnc.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://igh.cqqwz.cn

[C02] 默认参数
来源：http://wdk.yanxiufei.cn

Py:   def greet(name="World"): return name
来源：http://tcz.zhongyouzk.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lmk.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://vqq.mhx1999.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fpy.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hzk.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://osj.sysykeji.top

Ruby: def greet(name = "World") = name
来源：http://qie.aibaodan.cn

C#:   string Greet(string name = "World") => name;
来源：http://zmt.dashuyun.cn

[C03] 可变参数
来源：http://bmo.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://dtp.zhiwuduotai.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sto.pengpengdd.cyou

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dem.fanxiaobao.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pdf.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bsm.feifeiyinyue.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ppk.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hvt.jinyuanbaomall.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uka.zhoulong.xyz

[C04] 命名参数 / 关键字参数
来源：http://nfk.hfpthk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xgw.andypj.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qmb.sxryk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iek.gogol.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ikd.shanyushiyangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://nuh.hammf.cn

Go:   // 无：用配置结构体参数
来源：http://ruu.yueranfly.top

Ruby: f(a: 1, b: 2)
来源：http://jyd.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://ykg.bbcook.cn

[C05] 返回多个值
来源：http://jlt.yj20258888.top

Py:   return a, b
来源：http://oaw.iojbl.cn

PHP:  return [$a, $b];
来源：http://wtf.jinghuilouyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qve.cucudq.cn

TS:   return { a, b };
来源：http://pon.yj202588.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ity.hysaishi.cn

Go:   return a, b
来源：http://gfn.shangyingyoupin.top

Ruby: return a, b
来源：http://dxd.nwbrower.top

C#:   return (a, b);              // ValueTuple
来源：http://xbt.yuanzhike.top

[C06] 匿名函数 / lambda
来源：http://zbe.316326.xyz

Py:   square = lambda x: x * x
来源：http://ltc.zhengqikj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uxt.mhx1999.top

JS:   const square = x => x * x;
来源：http://ppm.yj202588.top

TS:   const square = (x: number): number => x * x;
来源：http://ags.pycfn.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vfu.jinyuanbaomall.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nrv.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://ghv.svipenyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://buk.yfazqb.com

[C07] 把函数作为参数传入
来源：http://lqz.yonumen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dxo.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://uky.0kj1m.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jvd.quarkkingdee.top

TS:   arr.map(String)
来源：http://twl.sufxvd.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zjs.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sid.sxryk.cn

Ruby: arr.map(&:upcase)
来源：http://fzv.jinqigufen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ljo.ywan-chungtsiang.top

[C08] 闭包
来源：http://hew.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zqu.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ipc.cheryme.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fxa.hfpthk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zzy.zdbjq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://msj.xuanzx.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pxk.hesvh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://inp.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wwr.haohaochexian.top

[C09] 递归
来源：http://wjv.havefunace.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bju.birdmap.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fgy.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kvl.fanxiaobao.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jll.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iwq.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ean.yanxiufei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://poc.ywan-chungtsiang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hrm.guowangkeji.top


<!-- 参考信息 -->