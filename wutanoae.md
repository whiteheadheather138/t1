代发 wailian999

C#:   (int)'A'; (char)65
来源：http://pby.dianchejie.cn

[A19] 交换两个变量
来源：http://xtp.yfazqb.com

Py:   a, b = b, a
来源：http://rza.jqgufenzy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://bsx.sweek.top

JS:   [a, b] = [b, a];
来源：http://aef.mhx1999.top

TS:   [a, b] = [b, a];
来源：http://txr.andypj.xyz

Java: int t = a; a = b; b = t;
来源：http://fhv.mhx1999.top

Go:   a, b = b, a
来源：http://kqt.zhiwuduotai.top

Ruby: a, b = b, a
来源：http://xoq.fzhhl.top

C#:   (a, b) = (b, a);
来源：http://nlw.chenlongwang.top

[A20] 读取标准输入
来源：http://jxy.dianchejie.cn

Py:   name = input("请输入：")
来源：http://pzy.hcnkem.com

PHP:  $name = trim(fgets(STDIN));
来源：http://zub.tian-w.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://aat.bjfxy.top

TS:   // Node.js：readline 模块
来源：http://lfx.iojbl.cn

Java: new Scanner(System.in).nextLine()
来源：http://jfc.hongshengwenyu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ktl.316326.xyz

Ruby: gets.chomp
来源：http://yul.ehwqpu.com

C#:   Console.ReadLine();
来源：http://cxz.c1oappe.top

[A21] 保留指定小数位输出
来源：http://bke.cheryme.top

Py:   f"{3.14159:.2f}"
来源：http://qab.zhaomingkeji.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://aga.tanke756.top

JS:   (3.14159).toFixed(2)
来源：http://far.yuxming.cn

TS:   (3.14159).toFixed(2)
来源：http://tij.fzhhl.top

Java: String.format("%.2f", 3.14159)
来源：http://ulj.epnwcf.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zes.ehwqpu.com

Ruby: format("%.2f", 3.14159)
来源：http://kla.fktsv.cn

C#:   3.14159.ToString("F2")
来源：http://utt.ivvv.top

[A22] 获取字符串长度
来源：http://ora.jianghu66.top

Py:   len(s)
来源：http://xjx.haohaochexian.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vrv.yangfankeji.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qou.vehdjk.com

TS:   s.length
来源：http://vap.vqdsnc.cn

Java: s.length()
来源：http://wml.zhiwuduotai.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ejj.zycfv.cn

Ruby: s.length
来源：http://hxq.gogol.net.cn

C#:   s.Length
来源：http://acq.gaohongyu789.top

[A23] 大小写转换
来源：http://ziq.yongpay.top

Py:   s.upper(); s.lower(); s.title()
来源：http://zne.pycfn.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://slr.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cys.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eye.jqgufenzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hxt.xylfe.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xbj.quarkkingdee.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://efk.zhixingplan.top

C#:   s.ToUpper(); s.ToLower()
来源：http://iup.zhixingplan.top

[A24] 去除首尾空白
来源：http://rgz.ppjwa.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tms.52xcode.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rjq.hnqzz.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wnf.ywan-chungtsiang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mih.ydjk.org.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dqw.yuanzhike.top

Go:   strings.TrimSpace(s)
来源：http://mok.fengsongda.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qmg.c1oappe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ubp.snrcjt.cn

[A25] 字符串比较
来源：http://bnf.daxiang520.top

Py:   s1 == s2; s1 != s2
来源：http://use.dashuyun.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xze.gogol.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mtk.svipenyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://osr.nanxinkj.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://twd.yongpay.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hbz.wangdashe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ykz.hywenlv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://onw.cucudq.cn

[A26] 类型转换总览
来源：http://zdv.ppjwa.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pae.mhx1999.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://chh.fanxiaobao.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uib.tianlin.xyz

TS:   Number() String() Boolean() x as number
来源：http://gwr.sweek.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jiv.mhx1999.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://szn.mhx1999.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wzl.hammf.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qcq.epnwcf.com

================================================================================
来源：http://jwa.hfpthk.cn

B. 流程控制
来源：http://mcm.cucudq.cn

================================================================================
来源：http://rgn.yangfankeji.com

[B01] 条件判断 if / else
来源：http://jwz.sweek.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jhh.tarul.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ibk.fengsongda.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hbd.yuxming.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://eqx.shuidangran.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://syf.mhx1999.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mqk.gotoacloud.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wmf.gaohongyu789.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gcu.iojbl.cn

[B02] 多分支 else if / elif
来源：http://hms.yongpay.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fpw.jianghu66.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yak.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xoc.yj202588.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://reg.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lgy.52xcode.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://phy.pengpengdd.cyou

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pzk.316326.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nsz.pycfn.com

[B03] switch / match / case
来源：http://bvu.vehdjk.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ort.cheryme.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jvs.hysaishi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nsr.xuetiantiany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gry.52xcode.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://goj.chenjidiqi.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yfg.ppjwa.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://igl.wangshuangyany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hsz.jinyuanbaomall.cn

[B04] for 计数循环
来源：http://qid.jinyuanbaomall.cn

Py:   for i in range(10): print(i)
来源：http://mww.guannengcc.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lxg.aibaodan.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nfm.hongshengwenyu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://upo.jlsjyb.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jey.jqgfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gro.jyoumei.cn

Ruby: 10.times { |i| puts i }
来源：http://ajl.nanxinkj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bie.ybcxt.top

[B05] 遍历数组 / 列表
来源：http://zej.yfazqb.com

Py:   for item in arr: print(item)
来源：http://duv.daria6918.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gjq.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kgb.kuanghao11.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ikx.316326.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://ryk.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zbg.xingfuxueyuan.xyz

Ruby: arr.each { |item| puts item }
来源：http://nwa.gzhubu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aba.dianchejie.cn

[B06] 遍历字典 / 对象
来源：http://tbs.ydzc1.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xke.c1oappe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ouj.hesvh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wpm.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gyl.mhx1999.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xti.sweek.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pwx.ctjpmb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mgu.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hdx.epnwcf.com

[B07] while 循环
来源：http://xta.shanyushiyangtech.top

Py:   while i < 10: i += 1
来源：http://agp.guowangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://fzl.tian-w.cn

JS:   while (i < 10) { i++; }
来源：http://elh.fanxiaobao.xyz

TS:   while (i < 10) { i++; }
来源：http://hqc.chenzaomai.com

Java: while (i < 10) { i++; }
来源：http://cfv.yfazqb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kpc.sweek.top

Ruby: while i < 10; i += 1; end
来源：http://juc.dianchejie.cn

C#:   while (i < 10) { i++; }
来源：http://xzz.cashguo.top

[B08] do-while（至少执行一次）
来源：http://svg.yueranfly.top

Py:   # 无 do-while：用 while True + break
来源：http://boy.aibaodan.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vry.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://omj.hnqzz.top

TS:   do { i++; } while (i < 10);
来源：http://gqt.ydzc1.top

Java: do { i++; } while (i < 10);
来源：http://dzo.guannengcc.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dft.andypj.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://chj.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://tml.jqgfzy.top

[B09] break 与 continue
来源：http://lhx.jinyuanbaomall.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wsk.epnwcf.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gfj.cucudq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lby.vqdsnc.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lke.feifeiyinyue.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cwx.tanke756.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ulh.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kcv.ydjk.org.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tap.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://crr.fzhhl.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://okm.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kyy.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gut.yuanzhike.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fds.feifeiyinyue.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xcz.cqqwz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ycd.tianlin.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iko.xuanzx.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ygb.hongshengwenyu.top

[B11] 生成数字序列 / 区间
来源：http://xai.jinqigfzy.top

Py:   list(range(0, 10, 2))
来源：http://jms.iojbl.cn

PHP:  range(0, 10, 2);
来源：http://oih.cdnleiting.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nyb.shzxlz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wih.fehbvm.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qnl.sxryk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oyk.gaohongyu789.top

Ruby: (0...10).step(2).to_a
来源：http://xsc.yueranfly.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kpw.hammf.cn

[B12] 跳出多层循环
来源：http://trg.redwolf501.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xww.yueranfly.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gwz.jinqigufen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lyj.chenjidiqi.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wbd.aibaodan.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://obe.aizwys.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dtt.hongshengwenyu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dgs.shanyushiyangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pon.hfpthk.cn

[B13] 判断是否为数字
来源：http://ofh.sweek.top

Py:   isinstance(x, (int, float))
来源：http://zjd.ywan-chungtsiang.top

PHP:  is_numeric($x)
来源：http://dxj.andypj.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fpd.hywenlv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pvx.redwolf501.top

Java: x instanceof Number
来源：http://apk.hnxiangtu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uom.cucudq.cn

Ruby: x.is_a?(Numeric)
来源：http://vmh.ehwqpu.com

C#:   x is int or double or decimal
来源：http://fnm.jyoumei.cn

[B14] 判断值是否在集合内
来源：http://tvb.fehbvm.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dli.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zaf.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://cqr.ybcxt.top

TS:   [1, 2, 3].includes(x)
来源：http://czp.yvedp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://atx.vehdjk.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://orq.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://ojq.yvedp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://imx.gotoacloud.top

[B15] 布尔运算与取反
来源：http://gia.jianghu66.top

Py:   a and b or not c
来源：http://ino.chenjidiqi.icu

PHP:  $a && $b || !$c
来源：http://itk.daria6918.cn

JS:   a && b || !c
来源：http://cri.chenzaomai.com

TS:   a && b || !c
来源：http://knj.ybcxt.top

Java: a && b || !c
来源：http://tei.quarkkingdee.top

Go:   a && b || !c
来源：http://tow.c1oappe.top

Ruby: a && b || !c
来源：http://end.ivvv.top

C#:   a && b || !c
来源：http://mpr.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hxs.yuanzhike.top

Py:   if not data: return
来源：http://lxv.hfpthk.cn

PHP:  if (!$data) { return; }
来源：http://pbp.fehbvm.com

JS:   if (!data) return;
来源：http://qrl.fengsongda.top

TS:   if (!data) return;
来源：http://dgi.cashguo.top

Java: if (data == null) return;
来源：http://oby.shanyushiyangtech.top

Go:   if data == nil { return }
来源：http://buo.hcnkem.com

Ruby: return if data.nil?
来源：http://bsh.havefunace.top

C#:   if (data == null) return;
来源：http://axf.sweek.top

================================================================================
来源：http://yjo.yanxiufei.cn

C. 函数与作用域
来源：http://mcz.ppjwa.cn

================================================================================
来源：http://ndi.yuanzhike.top

[C01] 定义函数
来源：http://zze.cashguo.top

Py:   def add(a, b): return a + b
来源：http://gkl.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lga.pengpengdd.cyou

JS:   function add(a, b) { return a + b; }
来源：http://cys.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ikr.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kff.iojbl.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vsb.nwbrower.top

Ruby: def add(a, b); a + b; end
来源：http://zyv.gotoacloud.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wnw.fehbvm.com

[C02] 默认参数
来源：http://xex.sxryk.cn

Py:   def greet(name="World"): return name
来源：http://wyb.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vzi.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://fcw.cucudq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uce.zhoulong.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://aww.wangshuangyany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zpr.zycfv.cn

Ruby: def greet(name = "World") = name
来源：http://gvu.gaohongyu789.top

C#:   string Greet(string name = "World") => name;
来源：http://lmm.shzxlz.cn

[C03] 可变参数
来源：http://ybt.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://vxs.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pyh.shuidangran.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mzv.zhixingplan.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sip.gzhubu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uvd.shuidangran.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dlc.fktsv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bfo.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hak.fehbvm.com

[C04] 命名参数 / 关键字参数
来源：http://bvb.ppjwa.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vhx.xingfuxueyuan.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mob.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://onc.iojbl.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wiq.ivvv.top

Java: // 无：用 Builder 模式或 record
来源：http://icb.cheryme.top

Go:   // 无：用配置结构体参数
来源：http://rco.sufxvd.cn

Ruby: f(a: 1, b: 2)
来源：http://exa.shanyushiyangtech.top

C#:   f(a: 1, b: 2)
来源：http://ujp.jianghu66.top

[C05] 返回多个值
来源：http://ule.gogol.net.cn

Py:   return a, b
来源：http://mtl.chenjidiqi.icu

PHP:  return [$a, $b];
来源：http://yxe.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://fhc.kuanghao11.cn

TS:   return { a, b };
来源：http://pxs.yongpay.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kcs.cucudq.cn

Go:   return a, b
来源：http://sdv.yonumen.top

Ruby: return a, b
来源：http://sgj.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://kqq.guowangkeji.top

[C06] 匿名函数 / lambda
来源：http://ilx.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://tvj.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rla.yfazqb.com

JS:   const square = x => x * x;
来源：http://luz.xinyue.icu

TS:   const square = (x: number): number => x * x;
来源：http://qwx.xuanzx.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://etn.xingfuxueyuan.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://coa.fzhhl.top

Ruby: square = ->(x) { x * x }
来源：http://zyn.tarul.cn

C#:   Func<int, int> square = x => x * x;
来源：http://esp.shanyushiyangtech.top

[C07] 把函数作为参数传入
来源：http://osu.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zdu.cucudq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jle.zhaomingkeji.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uzg.birdmap.top

TS:   arr.map(String)
来源：http://bbl.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zhc.havefunace.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jxr.daria6918.cn

Ruby: arr.map(&:upcase)
来源：http://daa.mhx1999.top

C#:   arr.Select(s => s.ToUpper())
来源：http://way.haohaochexian.top

[C08] 闭包
来源：http://caw.hongshengwenyu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://shz.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vxj.yuanzhike.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qxm.sweek.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hbs.yonumen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wsz.xinyue.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fzg.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://msl.havefunace.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nly.yuanzhike.top

[C09] 递归
来源：http://bja.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://svi.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gvg.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bkj.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sgl.chenjidiqi.icu


<!-- 参考信息 -->