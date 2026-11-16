代发 wailian999

C#:   (int)'A'; (char)65
来源：http://pya.tarul.cn

[A19] 交换两个变量
来源：http://mvx.havefunace.top

Py:   a, b = b, a
来源：http://eds.andypj.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://rgv.xuetiantiany.cn

JS:   [a, b] = [b, a];
来源：http://bvj.nanxinkj.top

TS:   [a, b] = [b, a];
来源：http://rxz.aibaodan.cn

Java: int t = a; a = b; b = t;
来源：http://kuz.shzxlz.cn

Go:   a, b = b, a
来源：http://gst.yj20258.top

Ruby: a, b = b, a
来源：http://akj.nanxuanxn.top

C#:   (a, b) = (b, a);
来源：http://dwc.gaohongyu789.top

[A20] 读取标准输入
来源：http://dxg.cheryme.top

Py:   name = input("请输入：")
来源：http://riv.yj20258888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://taa.hysaishi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rly.xylfe.cn

TS:   // Node.js：readline 模块
来源：http://qok.shanyushiyangtech.top

Java: new Scanner(System.in).nextLine()
来源：http://yag.quarkkingdee.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://duj.shanyushiyangkeji.top

Ruby: gets.chomp
来源：http://awa.jinqigfzy.top

C#:   Console.ReadLine();
来源：http://hdd.snrcjt.cn

[A21] 保留指定小数位输出
来源：http://rgf.chenjidiqi.icu

Py:   f"{3.14159:.2f}"
来源：http://sdr.zhiwuduotai.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gle.vehdjk.com

JS:   (3.14159).toFixed(2)
来源：http://ktj.ydjk.org.cn

TS:   (3.14159).toFixed(2)
来源：http://odu.gaohongyu789.top

Java: String.format("%.2f", 3.14159)
来源：http://fya.xinyue.icu

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eby.fktsv.cn

Ruby: format("%.2f", 3.14159)
来源：http://abs.jqgufenzy.top

C#:   3.14159.ToString("F2")
来源：http://opz.jlsjyb.cn

[A22] 获取字符串长度
来源：http://aem.sxryk.cn

Py:   len(s)
来源：http://ubl.haohaochexian.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ast.ydzc1.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uql.52xcode.cn

TS:   s.length
来源：http://xev.ehwqpu.com

Java: s.length()
来源：http://ave.ydjk.org.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pml.zhaomingkeji.xyz

Ruby: s.length
来源：http://owz.dashuyun.cn

C#:   s.Length
来源：http://dog.zdqjudy.top

[A23] 大小写转换
来源：http://lah.smart0.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://mva.meibo888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tqd.xziqi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rih.shanyushiyangtech.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://igm.jinqigfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kjw.fengsongda.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ksw.uphjek.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cuz.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://fcw.pycfn.com

[A24] 去除首尾空白
来源：http://nrj.fzhhl.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bkl.meibo888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ake.cucudq.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ffh.guannengcc.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://foi.jinqigfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pfu.jiagoushi.top

Go:   strings.TrimSpace(s)
来源：http://pzs.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dmp.bjfxy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yom.hnqzz.top

[A25] 字符串比较
来源：http://hyc.xinyue.icu

Py:   s1 == s2; s1 != s2
来源：http://chj.daria6918.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cge.xingfuxueyuan.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://drn.hywenlv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cll.epnwcf.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bzy.hcnkem.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bjn.hongshengwenyu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xuq.yvedp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eke.bbcook.cn

[A26] 类型转换总览
来源：http://waq.0kj1m.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://skd.yj202588.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yng.yj20258.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://icu.cqqwz.cn

TS:   Number() String() Boolean() x as number
来源：http://kfr.hfpthk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zah.yanxiufei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pem.xuanzx.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://gly.mhx1999.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nve.jlsjyb.cn

================================================================================
来源：http://skn.fehbvm.com

B. 流程控制
来源：http://ilo.tanke756.top

================================================================================
来源：http://gpn.nanxinkj.top

[B01] 条件判断 if / else
来源：http://mcs.pycfn.com

Py:   result = "正" if x > 0 else "非正"
来源：http://dzg.sjlbkw.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jlr.pycfn.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://trn.zdqjudy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://trr.kuanghao11.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ksn.vqdsnc.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://awy.fzhhl.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cra.andypj.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xph.svipenyu.cn

[B02] 多分支 else if / elif
来源：http://rcm.kuanghao11.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ecu.hysaishi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tyv.hnqzz.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mnh.bjfxy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://seu.gaohongyu789.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wzx.jyoumei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://col.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wyy.svipenyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cpy.hammf.cn

[B03] switch / match / case
来源：http://rtf.chenlongwang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xio.zdbjq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qvv.shangyingyoupin.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bsh.fengsongda.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fiw.nwbrower.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://avg.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qqd.chenjidiqi.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kte.gzhubu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xyj.yj20258.top

[B04] for 计数循环
来源：http://imw.meibo888.top

Py:   for i in range(10): print(i)
来源：http://poa.vqdsnc.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eyo.vqdsnc.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qtr.ehwqpu.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xdy.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gne.zhiwuduotai.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xfy.ydzc1.top

Ruby: 10.times { |i| puts i }
来源：http://keg.fanxiaobao.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gkj.bbcook.cn

[B05] 遍历数组 / 列表
来源：http://ipw.52xcode.cn

Py:   for item in arr: print(item)
来源：http://rie.xziqi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ecb.hongshengwenyu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mnf.meibo888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wzc.tanke756.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://scy.0kj1m.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iyc.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://slp.ybcxt.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ufc.nanxuanxn.top

[B06] 遍历字典 / 对象
来源：http://meq.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://sio.jinqigufen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xhv.gotoacloud.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://skj.shuidangran.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lda.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wog.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qdd.cashguo.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://utf.yj202588.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://drq.c1oappe.top

[B07] while 循环
来源：http://jlq.cqqwz.cn

Py:   while i < 10: i += 1
来源：http://lsr.ybcxt.top

PHP:  while ($i < 10) { $i++; }
来源：http://fpr.chenlongwang.top

JS:   while (i < 10) { i++; }
来源：http://lln.tian-w.cn

TS:   while (i < 10) { i++; }
来源：http://lkx.fzhhl.top

Java: while (i < 10) { i++; }
来源：http://ltf.hcnkem.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tni.tianlin.xyz

Ruby: while i < 10; i += 1; end
来源：http://nza.chenzaomai.com

C#:   while (i < 10) { i++; }
来源：http://bas.chenzaomai.com

[B08] do-while（至少执行一次）
来源：http://sne.zdbjq.cn

Py:   # 无 do-while：用 while True + break
来源：http://rxc.shanyushiyangtech.top

PHP:  do { $i++; } while ($i < 10);
来源：http://oje.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://vwm.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://hlq.yuxming.cn

Java: do { i++; } while (i < 10);
来源：http://psc.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ddu.zdbjq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fpa.ppjwa.cn

C#:   do { i++; } while (i < 10);
来源：http://fed.sxryk.cn

[B09] break 与 continue
来源：http://eiw.hongshengwenyu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jdx.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vty.pengpengdd.cyou

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ece.tianlin.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qyz.dashuyun.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sep.zhixingplan.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wpe.zhengqikj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qpt.c1oappe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rfy.xziqi.cn

[B10] 遍历同时拿索引
来源：http://mda.svipenyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://res.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yjj.xuanzx.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nyg.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uhi.jinqigfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ipu.daria6918.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uxu.ywan-chungtsiang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://etb.haohaochexian.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qeu.feifeiyinyue.top

[B11] 生成数字序列 / 区间
来源：http://jkm.yanxiufei.cn

Py:   list(range(0, 10, 2))
来源：http://vjv.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://xla.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dwe.yueranfly.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bqm.jinghuilouyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hew.jianghu66.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pmh.mhx1999.top

Ruby: (0...10).step(2).to_a
来源：http://ppj.iojbl.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dnd.hywenlv.cn

[B12] 跳出多层循环
来源：http://agf.nwbrower.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jbp.vqdsnc.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ddk.yj20258888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dvu.ivvv.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hyq.fehbvm.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zmm.zhengqikj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ymy.jlsjyb.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kzg.fengsongda.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lao.yvedp.cn

[B13] 判断是否为数字
来源：http://mgb.nanxuanxn.top

Py:   isinstance(x, (int, float))
来源：http://aod.xingfuxueyuan.xyz

PHP:  is_numeric($x)
来源：http://uns.52xcode.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pek.yangfankeji.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://alq.pengpengdd.cyou

Java: x instanceof Number
来源：http://fou.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yhp.ivvv.top

Ruby: x.is_a?(Numeric)
来源：http://lcb.ehwqpu.com

C#:   x is int or double or decimal
来源：http://qrq.chenlongwang.top

[B14] 判断值是否在集合内
来源：http://ykg.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cuh.hcnkem.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dvw.pycfn.com

JS:   [1, 2, 3].includes(x)
来源：http://xjb.ivvv.top

TS:   [1, 2, 3].includes(x)
来源：http://nbx.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xjw.guannengcc.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://upg.tarul.cn

Ruby: [1, 2, 3].include?(x)
来源：http://axg.nanxinkj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rfi.nwbrower.top

[B15] 布尔运算与取反
来源：http://bny.hcnkem.com

Py:   a and b or not c
来源：http://umq.gotoacloud.top

PHP:  $a && $b || !$c
来源：http://kae.zhongyouzk.top

JS:   a && b || !c
来源：http://hrs.svipenyu.cn

TS:   a && b || !c
来源：http://jkx.yueranfly.top

Java: a && b || !c
来源：http://hcu.cqqwz.cn

Go:   a && b || !c
来源：http://mae.yuxming.cn

Ruby: a && b || !c
来源：http://bvv.fengsongda.top

C#:   a && b || !c
来源：http://kfn.jinqigufen.top

[B16] 卫语句：不满足条件提前返回
来源：http://elz.quarkkingdee.top

Py:   if not data: return
来源：http://tkh.hesvh.cn

PHP:  if (!$data) { return; }
来源：http://nke.daxiang520.top

JS:   if (!data) return;
来源：http://gvv.hywenlv.cn

TS:   if (!data) return;
来源：http://fkd.quarkkingdee.top

Java: if (data == null) return;
来源：http://who.guannengcc.top

Go:   if data == nil { return }
来源：http://yxj.yongpay.top

Ruby: return if data.nil?
来源：http://dtg.yonumen.top

C#:   if (data == null) return;
来源：http://tio.haohaochexian.top

================================================================================
来源：http://six.shangyingyoupin.top

C. 函数与作用域
来源：http://ehd.aibaodan.cn

================================================================================
来源：http://xbg.c1oappe.top

[C01] 定义函数
来源：http://ciy.hysaishi.cn

Py:   def add(a, b): return a + b
来源：http://yhk.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hct.jinghuilouyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://jsq.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nvc.hywenlv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://psk.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://zsu.yonumen.top

Ruby: def add(a, b); a + b; end
来源：http://qhx.gogol.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ndy.meibo888.top

[C02] 默认参数
来源：http://hzp.yueranfly.top

Py:   def greet(name="World"): return name
来源：http://all.tarul.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mea.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://ckk.fengsongda.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ajj.xylfe.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sck.xuanzx.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ifz.aibaodan.cn

Ruby: def greet(name = "World") = name
来源：http://zdt.uphjek.com

C#:   string Greet(string name = "World") => name;
来源：http://nbj.bbcook.cn

[C03] 可变参数
来源：http://jkw.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://bgu.xylfe.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yxh.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nsp.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sgt.cashguo.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wnm.gzhubu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eaa.shzxlz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mtz.wangdashe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wfg.zhiwuduotai.top

[C04] 命名参数 / 关键字参数
来源：http://rka.hongshengwenyu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rpr.xinyue.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ogb.shangyingyoupin.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rjl.nwbrower.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gpm.haohaochexian.top

Java: // 无：用 Builder 模式或 record
来源：http://oza.shanyushiyangkeji.top

Go:   // 无：用配置结构体参数
来源：http://ldr.jqgfzy.top

Ruby: f(a: 1, b: 2)
来源：http://lpx.hnxiangtu.top

C#:   f(a: 1, b: 2)
来源：http://kit.bjfxy.top

[C05] 返回多个值
来源：http://lvt.ybcxt.top

Py:   return a, b
来源：http://frw.tianlin.xyz

PHP:  return [$a, $b];
来源：http://lof.xuanzx.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://rzk.sxryk.cn

TS:   return { a, b };
来源：http://qdl.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fir.smart0.xyz

Go:   return a, b
来源：http://iyi.epnwcf.com

Ruby: return a, b
来源：http://bck.jinghuilouyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://spu.yuanzhike.top

[C06] 匿名函数 / lambda
来源：http://hzb.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://dfs.zhaomingkeji.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://cef.svipenyu.cn

JS:   const square = x => x * x;
来源：http://glj.yvedp.cn

TS:   const square = (x: number): number => x * x;
来源：http://biy.nanxinkj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dtm.gaohongyu789.top

Go:   sq := func(x int) int { return x * x }
来源：http://wle.mhx1999.top

Ruby: square = ->(x) { x * x }
来源：http://alh.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fcv.nanxinkj.top

[C07] 把函数作为参数传入
来源：http://uri.c1oappe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fvp.hammf.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xxh.0kj1m.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://frr.cucudq.cn

TS:   arr.map(String)
来源：http://moe.daxiang520.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://clr.sxryk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://knf.hywenlv.cn

Ruby: arr.map(&:upcase)
来源：http://jky.ivvv.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tkw.gaohongyu789.top

[C08] 闭包
来源：http://tcd.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://heu.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gea.sxryk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wrf.guowangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nzg.redwolf501.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gob.ywan-chungtsiang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ffm.nanxinkj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rad.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zsg.jyoumei.cn

[C09] 递归
来源：http://ctv.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eoa.ppjwa.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zyy.xinyue.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kmr.aibaodan.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cku.redwolf501.top


<!-- 参考信息 -->