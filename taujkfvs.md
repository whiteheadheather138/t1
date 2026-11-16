代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://srd.sweek.top

Java: (int) 'A'; (char) 65
来源：http://rin.andypj.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wfs.meibo888.top

Ruby: "A".ord; 65.chr
来源：http://yjf.tianlin.xyz

C#:   (int)'A'; (char)65
来源：http://yxb.zhongyouzk.top

[A19] 交换两个变量
来源：http://mtq.pengpengdd.cyou

Py:   a, b = b, a
来源：http://efd.meibo888.top

PHP:  [$a, $b] = [$b, $a];
来源：http://fpo.tarul.cn

JS:   [a, b] = [b, a];
来源：http://ssy.meibo888.top

TS:   [a, b] = [b, a];
来源：http://nlq.fehbvm.com

Java: int t = a; a = b; b = t;
来源：http://flf.bjfxy.top

Go:   a, b = b, a
来源：http://uvx.hnqzz.top

Ruby: a, b = b, a
来源：http://ifa.havefunace.top

C#:   (a, b) = (b, a);
来源：http://xdh.xylfe.cn

[A20] 读取标准输入
来源：http://koh.chenzaomai.com

Py:   name = input("请输入：")
来源：http://wmy.zhoulong.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://ghj.wangdashe.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xff.sjlbkw.cn

TS:   // Node.js：readline 模块
来源：http://zyd.hcnkem.com

Java: new Scanner(System.in).nextLine()
来源：http://wqo.hesvh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wqw.wangdashe.top

Ruby: gets.chomp
来源：http://keu.fengsongda.top

C#:   Console.ReadLine();
来源：http://hmk.sysykeji.top

[A21] 保留指定小数位输出
来源：http://smg.fanxiaobao.xyz

Py:   f"{3.14159:.2f}"
来源：http://poh.wangshuangyany.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qtn.vqdsnc.cn

JS:   (3.14159).toFixed(2)
来源：http://get.fanxiaobao.xyz

TS:   (3.14159).toFixed(2)
来源：http://hkm.ctjpmb.com

Java: String.format("%.2f", 3.14159)
来源：http://pzd.kuanghao11.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jhz.ehwqpu.com

Ruby: format("%.2f", 3.14159)
来源：http://tjk.iojbl.cn

C#:   3.14159.ToString("F2")
来源：http://rxo.shanyushiyangtech.top

[A22] 获取字符串长度
来源：http://amy.zhaomingkeji.xyz

Py:   len(s)
来源：http://yls.fzhhl.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fzn.shuidangran.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dpq.ywan-chungtsiang.top

TS:   s.length
来源：http://afn.meibo888.top

Java: s.length()
来源：http://oke.ivvv.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rza.yongpay.top

Ruby: s.length
来源：http://pvy.jianghu66.top

C#:   s.Length
来源：http://efl.hcnkem.com

[A23] 大小写转换
来源：http://fmk.gotoacloud.top

Py:   s.upper(); s.lower(); s.title()
来源：http://grs.bjfxy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eie.zhixingplan.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xip.yongpay.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hyy.svipenyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ver.fanxiaobao.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wjj.tarul.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qxe.vqdsnc.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://icn.vqdsnc.cn

[A24] 去除首尾空白
来源：http://wjg.guannengcc.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bdc.ybcxt.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://izd.ydjk.org.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bof.jqgufenzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jnf.xylfe.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://trt.jianghu66.top

Go:   strings.TrimSpace(s)
来源：http://okm.zhixingplan.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ura.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ijk.ehwqpu.com

[A25] 字符串比较
来源：http://flc.zhijiandao.cn

Py:   s1 == s2; s1 != s2
来源：http://nwy.hammf.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://whm.mhx1999.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vjo.uphjek.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wcu.redwolf501.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jol.svipenyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xbk.hysaishi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rxc.yuanzhike.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wpr.epnwcf.com

[A26] 类型转换总览
来源：http://ydx.316326.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://usb.jinqigufen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nji.yj20258888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wzw.smart0.xyz

TS:   Number() String() Boolean() x as number
来源：http://dai.ybcxt.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://guq.haohaochexian.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://foq.haohaochexian.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://lmz.ehwqpu.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mlm.cdnleiting.top

================================================================================
来源：http://lfr.mhx1999.top

B. 流程控制
来源：http://soa.ctjpmb.com

================================================================================
来源：http://fqe.ehwqpu.com

[B01] 条件判断 if / else
来源：http://xsv.aibaodan.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bcx.9152youxi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://one.jlsjyb.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ssj.ywan-chungtsiang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cqk.chenjidiqi.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://rre.aibaodan.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oxt.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nxp.hywenlv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tau.aizwys.cn

[B02] 多分支 else if / elif
来源：http://mry.shzxlz.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fxy.hammf.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pxi.ivvv.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gtg.hywenlv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zwf.nanxinkj.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vwj.yueranfly.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lei.yj20258888.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qmd.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://syt.jqgufenzy.top

[B03] switch / match / case
来源：http://gmy.yuxming.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tho.jiagoushi.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lcv.yj20258.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wth.feifeiyinyue.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zyg.guowangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zle.yj202588.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qmu.yj20258.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mdq.hywenlv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fgo.jinqigfzy.top

[B04] for 计数循环
来源：http://ktk.ehwqpu.com

Py:   for i in range(10): print(i)
来源：http://sme.svipenyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tws.sufxvd.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eas.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kwx.wangdashe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qoc.hywenlv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://djo.havefunace.top

Ruby: 10.times { |i| puts i }
来源：http://dzk.c1oappe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://anm.0kj1m.cn

[B05] 遍历数组 / 列表
来源：http://klp.xylfe.cn

Py:   for item in arr: print(item)
来源：http://ytl.xuanzx.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vbw.cucudq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hwt.yueranfly.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ndg.52xcode.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://muq.iojbl.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cdz.wangshuangyany.cn

Ruby: arr.each { |item| puts item }
来源：http://ipm.ppjwa.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://glk.shzxlz.cn

[B06] 遍历字典 / 对象
来源：http://ltc.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zgn.hesvh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gyu.snrcjt.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://low.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://exw.yongpay.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jty.hysaishi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uln.fktsv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tyo.zhaomingkeji.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lch.yvedp.cn

[B07] while 循环
来源：http://ttn.yj202588.top

Py:   while i < 10: i += 1
来源：http://rht.zdqjudy.top

PHP:  while ($i < 10) { $i++; }
来源：http://gdw.xingfuxueyuan.xyz

JS:   while (i < 10) { i++; }
来源：http://vwu.hywenlv.cn

TS:   while (i < 10) { i++; }
来源：http://yxl.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://wit.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ndd.zdbjq.cn

Ruby: while i < 10; i += 1; end
来源：http://kiv.hysaishi.cn

C#:   while (i < 10) { i++; }
来源：http://zyr.cucudq.cn

[B08] do-while（至少执行一次）
来源：http://skb.daxiang520.top

Py:   # 无 do-while：用 while True + break
来源：http://whi.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vdo.aizwys.cn

JS:   do { i++; } while (i < 10);
来源：http://vjp.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://dlz.yuanzhike.top

Java: do { i++; } while (i < 10);
来源：http://mwh.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://ttq.meibo888.top

Ruby: begin; i += 1; end while i < 10
来源：http://stw.zhongyouzk.top

C#:   do { i++; } while (i < 10);
来源：http://com.daxiang520.top

[B09] break 与 continue
来源：http://zog.tarul.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qfz.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ecl.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sdu.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ulo.cheryme.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fip.chenjidiqi.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mtp.yangfankeji.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ghl.shangyingyoupin.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hjp.tanke756.top

[B10] 遍历同时拿索引
来源：http://yjc.c1oappe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wxn.fanxiaobao.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fcl.chenzaomai.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pon.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sxn.yuxming.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qlf.yongpay.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gvm.iojbl.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vzz.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bnw.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://rwr.bbcook.cn

Py:   list(range(0, 10, 2))
来源：http://dff.hysaishi.cn

PHP:  range(0, 10, 2);
来源：http://dse.gzhubu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aix.cqqwz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://afj.9152youxi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cjb.shanyushiyangtech.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://awp.sweek.top

Ruby: (0...10).step(2).to_a
来源：http://fto.hywenlv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ete.bbcook.cn

[B12] 跳出多层循环
来源：http://kxc.zdqjudy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ivi.hammf.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://heg.ydjk.org.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wil.jinqigufen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fpw.hcnkem.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nai.xylfe.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jft.nanxinkj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ffj.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uow.pengpengdd.cyou

[B13] 判断是否为数字
来源：http://uwn.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://cov.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://duy.zdqjudy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oda.fehbvm.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qgn.fzhhl.top

Java: x instanceof Number
来源：http://vcc.jiagoushi.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nvi.fanxiaobao.xyz

Ruby: x.is_a?(Numeric)
来源：http://osy.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://sjw.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://qly.hysaishi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mkz.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hbc.tanke756.top

JS:   [1, 2, 3].includes(x)
来源：http://eab.gogol.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://ltr.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ywe.ivvv.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aqj.jqgfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://nld.zycfv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ups.gogol.net.cn

[B15] 布尔运算与取反
来源：http://vrl.hongshengwenyu.top

Py:   a and b or not c
来源：http://rqr.smart0.xyz

PHP:  $a && $b || !$c
来源：http://tmr.cucudq.cn

JS:   a && b || !c
来源：http://fpp.sjlbkw.cn

TS:   a && b || !c
来源：http://aub.cashguo.top

Java: a && b || !c
来源：http://vvn.uphjek.com

Go:   a && b || !c
来源：http://med.feifeiyinyue.top

Ruby: a && b || !c
来源：http://hkx.jqgufenzy.top

C#:   a && b || !c
来源：http://yct.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://roi.hesvh.cn

Py:   if not data: return
来源：http://hrf.yuanzhike.top

PHP:  if (!$data) { return; }
来源：http://tyo.quarkkingdee.top

JS:   if (!data) return;
来源：http://ubf.guowangkeji.top

TS:   if (!data) return;
来源：http://onq.sufxvd.cn

Java: if (data == null) return;
来源：http://vwn.gotoacloud.top

Go:   if data == nil { return }
来源：http://rnq.jiagoushi.top

Ruby: return if data.nil?
来源：http://ada.sxryk.cn

C#:   if (data == null) return;
来源：http://aty.hnqzz.top

================================================================================
来源：http://vos.cdnleiting.top

C. 函数与作用域
来源：http://wlc.tanke756.top

================================================================================
来源：http://vjq.gzhubu.top

[C01] 定义函数
来源：http://mox.ivvv.top

Py:   def add(a, b): return a + b
来源：http://glk.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ijs.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://eju.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qbo.andypj.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://hws.daxiang520.top

Go:   func add(a, b int) int { return a + b }
来源：http://ffb.chenjidiqi.icu

Ruby: def add(a, b); a + b; end
来源：http://uvv.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pkf.tarul.cn

[C02] 默认参数
来源：http://orq.yvedp.cn

Py:   def greet(name="World"): return name
来源：http://lrc.ywan-chungtsiang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yqp.wangdashe.top

JS:   function greet(name = "World") { return name; }
来源：http://zyg.zhiwuduotai.top

TS:   function greet(name: string = "World") { return name; }
来源：http://atw.nanxinkj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fxv.meibo888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kcn.zycfv.cn

Ruby: def greet(name = "World") = name
来源：http://ldj.ydjk.org.cn

C#:   string Greet(string name = "World") => name;
来源：http://vyy.9152youxi.cn

[C03] 可变参数
来源：http://exn.dianchejie.cn

Py:   def total(*args): return sum(args)
来源：http://ryl.aibaodan.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fjn.andypj.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tfe.0kj1m.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rxx.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://thv.yuxming.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cgx.ydzc1.top

Ruby: def total(*nums); nums.sum; end
来源：http://cfe.fehbvm.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ave.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://qiv.mhx1999.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zns.ppjwa.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kwi.zhoulong.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dul.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kyc.jinqigufen.top

Java: // 无：用 Builder 模式或 record
来源：http://afu.tarul.cn

Go:   // 无：用配置结构体参数
来源：http://nmr.feifeiyinyue.top

Ruby: f(a: 1, b: 2)
来源：http://bbb.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://iqs.smart0.xyz

[C05] 返回多个值
来源：http://cez.bjfxy.top

Py:   return a, b
来源：http://fwg.9152youxi.cn

PHP:  return [$a, $b];
来源：http://xwq.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hxa.hfpthk.cn

TS:   return { a, b };
来源：http://zyj.sjlbkw.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mem.hnxiangtu.top

Go:   return a, b
来源：http://vpl.ydzc1.top

Ruby: return a, b
来源：http://oen.jianghu66.top

C#:   return (a, b);              // ValueTuple
来源：http://qqh.yuxming.cn

[C06] 匿名函数 / lambda
来源：http://ycm.yj20258888.top

Py:   square = lambda x: x * x
来源：http://vmc.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://otr.tian-w.cn

JS:   const square = x => x * x;
来源：http://amx.xziqi.cn

TS:   const square = (x: number): number => x * x;
来源：http://kle.pengpengdd.cyou

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nhq.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://czt.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://xqf.daria6918.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ehx.yanxiufei.cn

[C07] 把函数作为参数传入
来源：http://lpp.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fmr.dashuyun.cn

PHP:  array_map("strtoupper", $arr);
来源：http://raw.sweek.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://khg.tarul.cn

TS:   arr.map(String)
来源：http://pvg.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xnr.ivvv.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rqy.jinqigfzy.top

Ruby: arr.map(&:upcase)
来源：http://nzh.zhiwuduotai.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bbo.zhijiandao.cn

[C08] 闭包
来源：http://iqs.nanxuanxn.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iqe.birdmap.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jtn.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hik.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://egd.316326.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hzt.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zgs.jyoumei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dme.chenlongwang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://suy.jianghu66.top

[C09] 递归
来源：http://ony.aibaodan.cn


<!-- 参考信息 -->