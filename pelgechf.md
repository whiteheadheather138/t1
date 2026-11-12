代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://udg.hammf.cn

Java: (int) 'A'; (char) 65
来源：http://sli.bbcook.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://stf.iojbl.cn

Ruby: "A".ord; 65.chr
来源：http://udx.cashguo.top

C#:   (int)'A'; (char)65
来源：http://uqm.chenzaomai.com

[A19] 交换两个变量
来源：http://wqx.vehdjk.com

Py:   a, b = b, a
来源：http://lww.hongshengwenyu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://tgl.zhengqikj.top

JS:   [a, b] = [b, a];
来源：http://fbz.uphjek.com

TS:   [a, b] = [b, a];
来源：http://bzy.52xcode.cn

Java: int t = a; a = b; b = t;
来源：http://rdz.shuidangran.top

Go:   a, b = b, a
来源：http://aov.aibaodan.cn

Ruby: a, b = b, a
来源：http://gts.yueranfly.top

C#:   (a, b) = (b, a);
来源：http://axn.gotoacloud.top

[A20] 读取标准输入
来源：http://tht.hywenlv.cn

Py:   name = input("请输入：")
来源：http://ngz.c1oappe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zoz.9152youxi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gxf.epnwcf.com

TS:   // Node.js：readline 模块
来源：http://auc.xziqi.cn

Java: new Scanner(System.in).nextLine()
来源：http://vzr.zhoulong.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tvw.gotoacloud.top

Ruby: gets.chomp
来源：http://vdc.yanxiufei.cn

C#:   Console.ReadLine();
来源：http://yis.jinyuanbaomall.cn

[A21] 保留指定小数位输出
来源：http://jdf.quarkkingdee.top

Py:   f"{3.14159:.2f}"
来源：http://iki.havefunace.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://eub.ivvv.top

JS:   (3.14159).toFixed(2)
来源：http://val.mhx1999.top

TS:   (3.14159).toFixed(2)
来源：http://mvr.svipenyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://mzd.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eio.xingfuxueyuan.xyz

Ruby: format("%.2f", 3.14159)
来源：http://dyk.jqgufenzy.top

C#:   3.14159.ToString("F2")
来源：http://inc.zhongyouzk.top

[A22] 获取字符串长度
来源：http://cbi.jlsjyb.cn

Py:   len(s)
来源：http://ovh.haohaochexian.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zxz.uphjek.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://juv.nanxinkj.top

TS:   s.length
来源：http://mcg.redwolf501.top

Java: s.length()
来源：http://etq.hongshengwenyu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xbg.daria6918.cn

Ruby: s.length
来源：http://gil.chenzaomai.com

C#:   s.Length
来源：http://yru.shangyingyoupin.top

[A23] 大小写转换
来源：http://yrb.hnqzz.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kmm.shangyingyoupin.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tlq.gzhubu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://any.hcnkem.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://clo.shuidangran.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tmg.jqgfzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bxs.tarul.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rse.sxryk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rgk.fzhhl.top

[A24] 去除首尾空白
来源：http://jjz.guowangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yga.yongpay.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://scc.zycfv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rhc.tian-w.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jrh.kuanghao11.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rra.gogol.net.cn

Go:   strings.TrimSpace(s)
来源：http://ljd.birdmap.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tor.gaohongyu789.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lor.sxryk.cn

[A25] 字符串比较
来源：http://ybm.zhiwuduotai.top

Py:   s1 == s2; s1 != s2
来源：http://krz.jinyuanbaomall.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://edn.daria6918.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hqf.jqgufenzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aji.c1oappe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mwg.daxiang520.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fgd.tanke756.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dfq.tianlin.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://llo.jyoumei.cn

[A26] 类型转换总览
来源：http://vnc.redwolf501.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zaq.xylfe.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://crk.ctjpmb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mur.hcnkem.com

TS:   Number() String() Boolean() x as number
来源：http://rkn.hnqzz.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yom.zhijiandao.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mat.316326.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://rxn.uphjek.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gbf.fehbvm.com

================================================================================
来源：http://yti.xziqi.cn

B. 流程控制
来源：http://zuw.jinqigfzy.top

================================================================================
来源：http://ygh.pengpengdd.cyou

[B01] 条件判断 if / else
来源：http://koa.yuanzhike.top

Py:   result = "正" if x > 0 else "非正"
来源：http://joi.zdqjudy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xpv.sjlbkw.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kfe.zhengqikj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://msl.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dvb.haohaochexian.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hdm.aizwys.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cae.yj20258888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qsz.ydjk.org.cn

[B02] 多分支 else if / elif
来源：http://obl.svipenyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gsz.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://twz.yongpay.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hpk.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gnx.jlsjyb.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wnz.hesvh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ciq.nwbrower.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://suk.hammf.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zno.uphjek.com

[B03] switch / match / case
来源：http://zdj.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lre.vehdjk.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://onu.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vim.guannengcc.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lwg.fehbvm.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mgp.jinyuanbaomall.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fyd.fktsv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aww.gotoacloud.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://znz.cdnleiting.top

[B04] for 计数循环
来源：http://asg.yueranfly.top

Py:   for i in range(10): print(i)
来源：http://dbi.yuxming.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hfm.hongshengwenyu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://smg.jianghu66.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mla.xingfuxueyuan.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yay.gaohongyu789.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pfk.svipenyu.cn

Ruby: 10.times { |i| puts i }
来源：http://tez.pycfn.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qmr.shanyushiyangtech.top

[B05] 遍历数组 / 列表
来源：http://uzg.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://ahd.svipenyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wnm.zdqjudy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://biu.ywan-chungtsiang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hsl.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vna.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ghn.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://znz.guannengcc.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jmn.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://coq.chenzaomai.com

Py:   for k, v in d.items(): print(k, v)
来源：http://sof.hfpthk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://giu.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zyb.mhx1999.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jhc.chenlongwang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uml.jinyuanbaomall.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wxu.dianchejie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://avh.fanxiaobao.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aya.wangshuangyany.cn

[B07] while 循环
来源：http://ctk.chenzaomai.com

Py:   while i < 10: i += 1
来源：http://pgv.hnxiangtu.top

PHP:  while ($i < 10) { $i++; }
来源：http://fnd.sysykeji.top

JS:   while (i < 10) { i++; }
来源：http://fmo.guowangkeji.top

TS:   while (i < 10) { i++; }
来源：http://ccl.jiagoushi.top

Java: while (i < 10) { i++; }
来源：http://dwl.yvedp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qyb.cheryme.top

Ruby: while i < 10; i += 1; end
来源：http://aqp.tanke756.top

C#:   while (i < 10) { i++; }
来源：http://zxx.fktsv.cn

[B08] do-while（至少执行一次）
来源：http://hnd.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://hrj.shuidangran.top

PHP:  do { $i++; } while ($i < 10);
来源：http://sxy.c1oappe.top

JS:   do { i++; } while (i < 10);
来源：http://hxl.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://aye.ybcxt.top

Java: do { i++; } while (i < 10);
来源：http://twe.zycfv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kpv.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xco.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://fnh.jlsjyb.cn

[B09] break 与 continue
来源：http://hsm.aizwys.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xtv.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xxa.jqgufenzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rco.xingfuxueyuan.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ksj.zycfv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lby.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kct.chenjidiqi.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://szc.ivvv.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nmn.zhixingplan.top

[B10] 遍历同时拿索引
来源：http://rel.sufxvd.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nzs.jqgufenzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bwm.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kzx.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qwa.andypj.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vqa.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yos.shuidangran.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dgr.hesvh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://axy.zhongyouzk.top

[B11] 生成数字序列 / 区间
来源：http://djn.jqgfzy.top

Py:   list(range(0, 10, 2))
来源：http://rur.xylfe.cn

PHP:  range(0, 10, 2);
来源：http://irq.hywenlv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aqa.hcnkem.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://umy.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://taz.zhongyouzk.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zdt.tianlin.xyz

Ruby: (0...10).step(2).to_a
来源：http://kgp.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gjw.havefunace.top

[B12] 跳出多层循环
来源：http://nmv.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://imx.chenlongwang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ujo.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lxe.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gow.ivvv.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zdu.kuanghao11.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wes.fehbvm.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jri.nanxinkj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gig.daxiang520.top

[B13] 判断是否为数字
来源：http://ese.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://qsy.shanyushiyangkeji.top

PHP:  is_numeric($x)
来源：http://kvk.cashguo.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cfa.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rjo.hammf.cn

Java: x instanceof Number
来源：http://qtx.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://irg.jiagoushi.top

Ruby: x.is_a?(Numeric)
来源：http://utk.gogol.net.cn

C#:   x is int or double or decimal
来源：http://xpo.nwbrower.top

[B14] 判断值是否在集合内
来源：http://alq.cashguo.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ltp.hammf.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zrp.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://mkd.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://xzp.epnwcf.com

Java: List.of(1, 2, 3).contains(x)
来源：http://dzx.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ajc.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kye.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sni.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://aec.chenjidiqi.icu

Py:   a and b or not c
来源：http://xrf.snrcjt.cn

PHP:  $a && $b || !$c
来源：http://krn.hesvh.cn

JS:   a && b || !c
来源：http://tor.daria6918.cn

TS:   a && b || !c
来源：http://ncz.cucudq.cn

Java: a && b || !c
来源：http://rrr.jianghu66.top

Go:   a && b || !c
来源：http://zyg.shzxlz.cn

Ruby: a && b || !c
来源：http://zul.hnxiangtu.top

C#:   a && b || !c
来源：http://yfw.shuidangran.top

[B16] 卫语句：不满足条件提前返回
来源：http://oiw.fengsongda.top

Py:   if not data: return
来源：http://gba.svipenyu.cn

PHP:  if (!$data) { return; }
来源：http://isr.zdbjq.cn

JS:   if (!data) return;
来源：http://lxb.jqgfzy.top

TS:   if (!data) return;
来源：http://rcz.gaohongyu789.top

Java: if (data == null) return;
来源：http://vwi.jianghu66.top

Go:   if data == nil { return }
来源：http://cyg.hammf.cn

Ruby: return if data.nil?
来源：http://vhc.zhongyouzk.top

C#:   if (data == null) return;
来源：http://xrg.xingfuxueyuan.xyz

================================================================================
来源：http://eiw.yuanzhike.top

C. 函数与作用域
来源：http://vaq.uphjek.com

================================================================================
来源：http://tph.aibaodan.cn

[C01] 定义函数
来源：http://wrc.chenlongwang.top

Py:   def add(a, b): return a + b
来源：http://rdn.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://obm.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://yky.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jrw.hcnkem.com

Java: static int add(int a, int b) { return a + b; }
来源：http://qvq.zhoulong.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://iri.yueranfly.top

Ruby: def add(a, b); a + b; end
来源：http://ans.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iei.chenjidiqi.icu

[C02] 默认参数
来源：http://vut.cheryme.top

Py:   def greet(name="World"): return name
来源：http://ail.hongshengwenyu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://euy.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://uep.gogol.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rpy.shzxlz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kkv.daxiang520.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hbv.tanke756.top

Ruby: def greet(name = "World") = name
来源：http://zgt.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://ncs.hywenlv.cn

[C03] 可变参数
来源：http://mnd.guowangkeji.top

Py:   def total(*args): return sum(args)
来源：http://fht.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dun.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rmc.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://axa.chenjidiqi.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vkr.xingfuxueyuan.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nwl.zhaomingkeji.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://xws.tian-w.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jhg.xinyue.icu

[C04] 命名参数 / 关键字参数
来源：http://cvm.tian-w.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://inr.jyoumei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pbs.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://awk.uphjek.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mwe.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://mbl.52xcode.cn

Go:   // 无：用配置结构体参数
来源：http://gsn.xziqi.cn

Ruby: f(a: 1, b: 2)
来源：http://lku.sjlbkw.cn

C#:   f(a: 1, b: 2)
来源：http://hlh.gotoacloud.top

[C05] 返回多个值
来源：http://wxx.jinqigfzy.top

Py:   return a, b
来源：http://muv.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://tgb.bbcook.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nhw.snrcjt.cn

TS:   return { a, b };
来源：http://ucj.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mqt.zhongyouzk.top

Go:   return a, b
来源：http://lqk.mhx1999.top

Ruby: return a, b
来源：http://eef.fktsv.cn

C#:   return (a, b);              // ValueTuple
来源：http://xug.nanxinkj.top

[C06] 匿名函数 / lambda
来源：http://kkp.hnqzz.top

Py:   square = lambda x: x * x
来源：http://xno.kuanghao11.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://csh.hcnkem.com

JS:   const square = x => x * x;
来源：http://yew.xuetiantiany.cn

TS:   const square = (x: number): number => x * x;
来源：http://yfj.fehbvm.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://auq.ywan-chungtsiang.top

Go:   sq := func(x int) int { return x * x }
来源：http://nmi.jinqigfzy.top

Ruby: square = ->(x) { x * x }
来源：http://grh.zhengqikj.top

C#:   Func<int, int> square = x => x * x;
来源：http://iyk.cashguo.top

[C07] 把函数作为参数传入
来源：http://ppl.havefunace.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jwe.bbcook.cn

PHP:  array_map("strtoupper", $arr);
来源：http://aql.bbcook.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://moc.jinyuanbaomall.cn

TS:   arr.map(String)
来源：http://dln.dianchejie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ikw.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ayn.hnqzz.top

Ruby: arr.map(&:upcase)
来源：http://qyo.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://dtq.dianchejie.cn

[C08] 闭包
来源：http://rvn.fehbvm.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cbt.chenjidiqi.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zlv.xuanzx.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nit.cucudq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mqz.cucudq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://spr.chenlongwang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ukl.dashuyun.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://efs.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://foy.pengpengdd.cyou

[C09] 递归
来源：http://gko.yfazqb.com


<!-- 参考信息 -->