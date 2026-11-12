代发 wailian999

JS:   [a, b] = [b, a];
来源：http://alf.ehwqpu.com

TS:   [a, b] = [b, a];
来源：http://grg.fehbvm.com

Java: int t = a; a = b; b = t;
来源：http://ynd.sufxvd.cn

Go:   a, b = b, a
来源：http://ycw.xuanzx.com

Ruby: a, b = b, a
来源：http://xsu.zhiwuduotai.top

C#:   (a, b) = (b, a);
来源：http://ywz.sxryk.cn

[A20] 读取标准输入
来源：http://erd.smart0.xyz

Py:   name = input("请输入：")
来源：http://crr.bjfxy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jcy.hcnkem.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://aqo.zdqjudy.top

TS:   // Node.js：readline 模块
来源：http://vkv.hnxiangtu.top

Java: new Scanner(System.in).nextLine()
来源：http://wgt.svipenyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jyy.hywenlv.cn

Ruby: gets.chomp
来源：http://jci.ybcxt.top

C#:   Console.ReadLine();
来源：http://ojj.sysykeji.top

[A21] 保留指定小数位输出
来源：http://tsu.zdbjq.cn

Py:   f"{3.14159:.2f}"
来源：http://eve.xziqi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://svy.cashguo.top

JS:   (3.14159).toFixed(2)
来源：http://wzy.aizwys.cn

TS:   (3.14159).toFixed(2)
来源：http://smu.sufxvd.cn

Java: String.format("%.2f", 3.14159)
来源：http://oxc.hnxiangtu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wga.jlsjyb.cn

Ruby: format("%.2f", 3.14159)
来源：http://lvo.jyoumei.cn

C#:   3.14159.ToString("F2")
来源：http://daf.cqqwz.cn

[A22] 获取字符串长度
来源：http://rgk.hfpthk.cn

Py:   len(s)
来源：http://ama.shuidangran.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qee.aizwys.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eld.xylfe.cn

TS:   s.length
来源：http://gdg.ydjk.org.cn

Java: s.length()
来源：http://yrb.gzhubu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mhv.c1oappe.top

Ruby: s.length
来源：http://tyz.yangfankeji.com

C#:   s.Length
来源：http://gjw.gaohongyu789.top

[A23] 大小写转换
来源：http://kgs.fzhhl.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wmt.gaohongyu789.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wpj.hongshengwenyu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xrd.yangfankeji.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ftv.sysykeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mfx.smart0.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jgt.aizwys.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kko.smart0.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://xrz.fengsongda.top

[A24] 去除首尾空白
来源：http://jzt.hysaishi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qbi.yj20258.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vfv.ivvv.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cki.hfpthk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xpl.wangdashe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cmt.jqgfzy.top

Go:   strings.TrimSpace(s)
来源：http://mrl.ydjk.org.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zeg.xylfe.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://edi.gogol.net.cn

[A25] 字符串比较
来源：http://bly.gaohongyu789.top

Py:   s1 == s2; s1 != s2
来源：http://ida.birdmap.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aba.feifeiyinyue.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dct.0kj1m.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://znk.hywenlv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hdt.cqqwz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ffw.jinghuilouyu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://avf.gzhubu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bxx.ivvv.top

[A26] 类型转换总览
来源：http://ifi.zhijiandao.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vdt.tanke756.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nji.yueranfly.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ucx.mhx1999.top

TS:   Number() String() Boolean() x as number
来源：http://upl.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uqd.ybcxt.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lhi.9152youxi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vzt.ivvv.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wtc.52xcode.cn

================================================================================
来源：http://kpr.svipenyu.cn

B. 流程控制
来源：http://nmt.quarkkingdee.top

================================================================================
来源：http://trr.yangfankeji.com

[B01] 条件判断 if / else
来源：http://dmu.zhixingplan.top

Py:   result = "正" if x > 0 else "非正"
来源：http://myk.yanxiufei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bre.guannengcc.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fqq.hnqzz.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://olk.xylfe.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vkj.zhiwuduotai.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vcl.jianghu66.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yey.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://reu.ybcxt.top

[B02] 多分支 else if / elif
来源：http://sem.birdmap.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ypd.gaohongyu789.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nkg.hywenlv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ufc.cucudq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rmn.smart0.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fmg.svipenyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xac.hongshengwenyu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dcf.feifeiyinyue.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yne.xuetiantiany.cn

[B03] switch / match / case
来源：http://ome.ywan-chungtsiang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rpt.zhongyouzk.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jje.yangfankeji.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rmh.meibo888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tnv.jinqigufen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xtq.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uer.zhoulong.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://min.yj202588.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xxx.ydjk.org.cn

[B04] for 计数循环
来源：http://hfq.ybcxt.top

Py:   for i in range(10): print(i)
来源：http://izl.hnxiangtu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jrt.jiagoushi.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://imv.fanxiaobao.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hle.daria6918.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pcv.jyoumei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vva.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://rqt.yj20258888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rmk.hnqzz.top

[B05] 遍历数组 / 列表
来源：http://afr.tianlin.xyz

Py:   for item in arr: print(item)
来源：http://sos.ehwqpu.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://adw.snrcjt.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://aqe.ehwqpu.com

TS:   for (const item of arr) { console.log(item); }
来源：http://cyp.fzhhl.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jar.nwbrower.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vsm.sweek.top

Ruby: arr.each { |item| puts item }
来源：http://ucw.shanyushiyangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pty.nanxuanxn.top

[B06] 遍历字典 / 对象
来源：http://gak.sysykeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ipi.xingfuxueyuan.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ats.cucudq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://thn.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://agn.zhaomingkeji.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://erg.aizwys.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fkp.svipenyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ces.dashuyun.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sqe.fzhhl.top

[B07] while 循环
来源：http://smi.dashuyun.cn

Py:   while i < 10: i += 1
来源：http://kni.vqdsnc.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lck.zhijiandao.cn

JS:   while (i < 10) { i++; }
来源：http://pxe.fanxiaobao.xyz

TS:   while (i < 10) { i++; }
来源：http://vba.uphjek.com

Java: while (i < 10) { i++; }
来源：http://zrw.hysaishi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://exh.shuidangran.top

Ruby: while i < 10; i += 1; end
来源：http://zvc.zhixingplan.top

C#:   while (i < 10) { i++; }
来源：http://ppx.iojbl.cn

[B08] do-while（至少执行一次）
来源：http://iqn.jiagoushi.top

Py:   # 无 do-while：用 while True + break
来源：http://fed.cqqwz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nvj.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://pkv.mhx1999.top

TS:   do { i++; } while (i < 10);
来源：http://jho.hnqzz.top

Java: do { i++; } while (i < 10);
来源：http://mcc.hammf.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://diq.zycfv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://shf.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://chx.sysykeji.top

[B09] break 与 continue
来源：http://fqs.aizwys.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zbj.gzhubu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hre.hammf.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tec.yuxming.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kyx.feifeiyinyue.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dal.xingfuxueyuan.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fgm.xingfuxueyuan.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ten.52xcode.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hrn.vqdsnc.cn

[B10] 遍历同时拿索引
来源：http://dyo.gzhubu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rsk.zdbjq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nkb.havefunace.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://abz.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ivw.shanyushiyangtech.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cev.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://twb.havefunace.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aeo.ppjwa.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wpn.cashguo.top

[B11] 生成数字序列 / 区间
来源：http://hke.sweek.top

Py:   list(range(0, 10, 2))
来源：http://qre.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://cdg.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://inj.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hbr.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bpb.ydjk.org.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ufe.nwbrower.top

Ruby: (0...10).step(2).to_a
来源：http://lrn.feifeiyinyue.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rgm.shuidangran.top

[B12] 跳出多层循环
来源：http://ckh.bjfxy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rvn.yfazqb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://egk.jyoumei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ppf.shangyingyoupin.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qps.sxryk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://spd.xingfuxueyuan.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oba.zhoulong.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tly.yj202588.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qzp.cheryme.top

[B13] 判断是否为数字
来源：http://vdk.jqgufenzy.top

Py:   isinstance(x, (int, float))
来源：http://etj.jqgfzy.top

PHP:  is_numeric($x)
来源：http://gou.havefunace.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qbv.ehwqpu.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://faj.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://naz.zycfv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nzw.fengsongda.top

Ruby: x.is_a?(Numeric)
来源：http://rdi.snrcjt.cn

C#:   x is int or double or decimal
来源：http://whu.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://mco.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ahc.xuetiantiany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rcd.yvedp.cn

JS:   [1, 2, 3].includes(x)
来源：http://izs.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://rna.sjlbkw.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nec.dianchejie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nmt.yongpay.top

Ruby: [1, 2, 3].include?(x)
来源：http://ppg.316326.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rvu.sweek.top

[B15] 布尔运算与取反
来源：http://owx.nanxinkj.top

Py:   a and b or not c
来源：http://xml.smart0.xyz

PHP:  $a && $b || !$c
来源：http://vbs.yangfankeji.com

JS:   a && b || !c
来源：http://vjo.shanyushiyangkeji.top

TS:   a && b || !c
来源：http://mvr.bbcook.cn

Java: a && b || !c
来源：http://zht.hammf.cn

Go:   a && b || !c
来源：http://zkm.jinyuanbaomall.cn

Ruby: a && b || !c
来源：http://nkj.zhiwuduotai.top

C#:   a && b || !c
来源：http://tdu.jinqigufen.top

[B16] 卫语句：不满足条件提前返回
来源：http://ypa.0kj1m.cn

Py:   if not data: return
来源：http://joy.hammf.cn

PHP:  if (!$data) { return; }
来源：http://typ.tianlin.xyz

JS:   if (!data) return;
来源：http://yui.wangdashe.top

TS:   if (!data) return;
来源：http://xpz.yuanzhike.top

Java: if (data == null) return;
来源：http://npa.ydzc1.top

Go:   if data == nil { return }
来源：http://wiz.hesvh.cn

Ruby: return if data.nil?
来源：http://xtq.feifeiyinyue.top

C#:   if (data == null) return;
来源：http://djg.ivvv.top

================================================================================
来源：http://oad.dashuyun.cn

C. 函数与作用域
来源：http://pyn.hammf.cn

================================================================================
来源：http://dgt.aibaodan.cn

[C01] 定义函数
来源：http://xtp.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://nwy.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eyr.uphjek.com

JS:   function add(a, b) { return a + b; }
来源：http://bct.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gpf.shuidangran.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cps.haohaochexian.top

Go:   func add(a, b int) int { return a + b }
来源：http://qsp.yvedp.cn

Ruby: def add(a, b); a + b; end
来源：http://wcr.zhijiandao.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jio.smart0.xyz

[C02] 默认参数
来源：http://qzz.hnqzz.top

Py:   def greet(name="World"): return name
来源：http://hdf.dashuyun.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dui.cheryme.top

JS:   function greet(name = "World") { return name; }
来源：http://ler.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xnv.sweek.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hoc.ppjwa.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sdj.xuetiantiany.cn

Ruby: def greet(name = "World") = name
来源：http://jzx.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://exf.fktsv.cn

[C03] 可变参数
来源：http://vov.dianchejie.cn

Py:   def total(*args): return sum(args)
来源：http://zzm.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dgp.tarul.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://clz.yonumen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jnl.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mtf.xuetiantiany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rwu.shangyingyoupin.top

Ruby: def total(*nums); nums.sum; end
来源：http://ofm.zdqjudy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://auu.tanke756.top

[C04] 命名参数 / 关键字参数
来源：http://hzm.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lzk.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ubv.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gvg.tanke756.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://otb.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://xib.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://rif.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://fki.vqdsnc.cn

C#:   f(a: 1, b: 2)
来源：http://zvh.zhoulong.xyz

[C05] 返回多个值
来源：http://eri.ehwqpu.com

Py:   return a, b
来源：http://yxx.birdmap.top

PHP:  return [$a, $b];
来源：http://qud.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://psd.smart0.xyz

TS:   return { a, b };
来源：http://jgp.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tko.xinyue.icu

Go:   return a, b
来源：http://dsj.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://cvy.hnxiangtu.top

C#:   return (a, b);              // ValueTuple
来源：http://clp.ybcxt.top

[C06] 匿名函数 / lambda
来源：http://mqd.yuxming.cn

Py:   square = lambda x: x * x
来源：http://epf.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://bvs.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://ojy.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://fgd.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qqq.guannengcc.top

Go:   sq := func(x int) int { return x * x }
来源：http://ofo.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://qjw.sweek.top

C#:   Func<int, int> square = x => x * x;
来源：http://klc.dianchejie.cn

[C07] 把函数作为参数传入
来源：http://bzs.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rhw.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://mxv.sxryk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ugq.zhiwuduotai.top

TS:   arr.map(String)
来源：http://zdc.ehwqpu.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dlp.cheryme.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dgd.uphjek.com

Ruby: arr.map(&:upcase)
来源：http://ywl.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dbk.quarkkingdee.top

[C08] 闭包
来源：http://qua.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zbv.fktsv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ikj.yanxiufei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mrs.hcnkem.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ntw.gzhubu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ocq.hammf.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ypo.nwbrower.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nvu.jlsjyb.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hcb.birdmap.top

[C09] 递归
来源：http://nby.xinyue.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wtx.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ypd.ydjk.org.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qlu.xingfuxueyuan.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rqo.ctjpmb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kuc.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cwz.52xcode.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ioq.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ady.shangyingyoupin.top


<!-- 参考信息 -->