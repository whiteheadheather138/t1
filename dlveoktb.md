代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://sha.zdbjq.cn

Py:   ord("A"); chr(65)
来源：http://gen.jianghu66.top

PHP:  ord("A"); chr(65)
来源：http://kjy.birdmap.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xhs.yangfankeji.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://knq.birdmap.top

Java: (int) 'A'; (char) 65
来源：http://nit.ydjk.org.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://top.birdmap.top

Ruby: "A".ord; 65.chr
来源：http://yky.tanke756.top

C#:   (int)'A'; (char)65
来源：http://axk.c1oappe.top

[A19] 交换两个变量
来源：http://wjg.uphjek.com

Py:   a, b = b, a
来源：http://msb.daria6918.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xit.hongshengwenyu.top

JS:   [a, b] = [b, a];
来源：http://ddm.daxiang520.top

TS:   [a, b] = [b, a];
来源：http://vvy.yangfankeji.com

Java: int t = a; a = b; b = t;
来源：http://quf.daria6918.cn

Go:   a, b = b, a
来源：http://dil.meibo888.top

Ruby: a, b = b, a
来源：http://vvh.9152youxi.cn

C#:   (a, b) = (b, a);
来源：http://ylm.yueranfly.top

[A20] 读取标准输入
来源：http://mad.meibo888.top

Py:   name = input("请输入：")
来源：http://vgx.fengsongda.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wxu.fehbvm.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://plh.hnqzz.top

TS:   // Node.js：readline 模块
来源：http://egc.nanxinkj.top

Java: new Scanner(System.in).nextLine()
来源：http://imh.birdmap.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ein.jqgfzy.top

Ruby: gets.chomp
来源：http://bmw.ydjk.org.cn

C#:   Console.ReadLine();
来源：http://ukj.jianghu66.top

[A21] 保留指定小数位输出
来源：http://ewy.ydjk.org.cn

Py:   f"{3.14159:.2f}"
来源：http://jve.hcnkem.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://waz.vqdsnc.cn

JS:   (3.14159).toFixed(2)
来源：http://tns.guannengcc.top

TS:   (3.14159).toFixed(2)
来源：http://cvy.jqgfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://avc.wangshuangyany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tcx.zhengqikj.top

Ruby: format("%.2f", 3.14159)
来源：http://mxi.hnqzz.top

C#:   3.14159.ToString("F2")
来源：http://cgw.shangyingyoupin.top

[A22] 获取字符串长度
来源：http://jrj.ivvv.top

Py:   len(s)
来源：http://ydh.xuetiantiany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iee.guannengcc.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://awj.xziqi.cn

TS:   s.length
来源：http://jvy.zycfv.cn

Java: s.length()
来源：http://gym.jqgufenzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zhl.hcnkem.com

Ruby: s.length
来源：http://qyl.cdnleiting.top

C#:   s.Length
来源：http://ybq.zdbjq.cn

[A23] 大小写转换
来源：http://npw.jiagoushi.top

Py:   s.upper(); s.lower(); s.title()
来源：http://amu.ehwqpu.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jlm.gogol.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ige.jinqigufen.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qkm.hcnkem.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://etg.c1oappe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ekb.nanxuanxn.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bfl.svipenyu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nwm.jinyuanbaomall.cn

[A24] 去除首尾空白
来源：http://ayg.chenlongwang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qgt.gogol.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://olv.dashuyun.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baj.hongshengwenyu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://osq.shzxlz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cat.xuanzx.com

Go:   strings.TrimSpace(s)
来源：http://teg.jianghu66.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lss.sweek.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ctb.xinyue.icu

[A25] 字符串比较
来源：http://whj.uphjek.com

Py:   s1 == s2; s1 != s2
来源：http://nnb.nwbrower.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rth.yj202588.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wfu.zhiwuduotai.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zvq.zhixingplan.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oth.hcnkem.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gml.hnqzz.top

Ruby: s1 == s2; s1 <=> s2
来源：http://idq.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tqa.tanke756.top

[A26] 类型转换总览
来源：http://thc.shangyingyoupin.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hqe.xuanzx.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tnk.xylfe.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://emi.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://agl.bjfxy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dgj.kuanghao11.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gum.chenlongwang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dex.dashuyun.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ezm.guowangkeji.top

================================================================================
来源：http://ohi.zhongyouzk.top

B. 流程控制
来源：http://kro.ydjk.org.cn

================================================================================
来源：http://ztv.sxryk.cn

[B01] 条件判断 if / else
来源：http://rbd.xingfuxueyuan.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://und.hfpthk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xdk.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://egh.hfpthk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://klz.yfazqb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://mgu.xingfuxueyuan.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qlx.cqqwz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bgd.xuanzx.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://noy.xingfuxueyuan.xyz

[B02] 多分支 else if / elif
来源：http://ayz.chenjidiqi.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wud.guowangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sse.yonumen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vpv.wangshuangyany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cvt.zhengqikj.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ull.cqqwz.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hbk.yongpay.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fqq.aibaodan.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pvk.fengsongda.top

[B03] switch / match / case
来源：http://pml.birdmap.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://izk.daria6918.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rqy.tarul.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gua.nwbrower.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jmq.zhengqikj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pgl.tian-w.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hqq.ywan-chungtsiang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bcl.sysykeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lhc.ivvv.top

[B04] for 计数循环
来源：http://rwk.nwbrower.top

Py:   for i in range(10): print(i)
来源：http://dit.shuidangran.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ndz.tanke756.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fjg.zycfv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vvr.ybcxt.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rns.ydzc1.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ojj.bjfxy.top

Ruby: 10.times { |i| puts i }
来源：http://tzy.sweek.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rqd.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://own.shuidangran.top

Py:   for item in arr: print(item)
来源：http://rqo.haohaochexian.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hco.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ilo.xingfuxueyuan.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://aot.iojbl.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gur.jinyuanbaomall.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://guu.fzhhl.top

Ruby: arr.each { |item| puts item }
来源：http://ksa.yongpay.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fxh.ctjpmb.com

[B06] 遍历字典 / 对象
来源：http://cam.dashuyun.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cyc.zhongyouzk.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vwe.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bje.ybcxt.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ctt.zhaomingkeji.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lii.chenlongwang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bix.hywenlv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jcu.uphjek.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zls.shanyushiyangkeji.top

[B07] while 循环
来源：http://euq.xylfe.cn

Py:   while i < 10: i += 1
来源：http://rxx.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://zhi.svipenyu.cn

JS:   while (i < 10) { i++; }
来源：http://dsw.fehbvm.com

TS:   while (i < 10) { i++; }
来源：http://gqn.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://lol.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jlt.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://smf.yangfankeji.com

C#:   while (i < 10) { i++; }
来源：http://ajy.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://xax.ywan-chungtsiang.top

Py:   # 无 do-while：用 while True + break
来源：http://feg.xuanzx.com

PHP:  do { $i++; } while ($i < 10);
来源：http://hxz.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://rgs.xinyue.icu

TS:   do { i++; } while (i < 10);
来源：http://zns.quarkkingdee.top

Java: do { i++; } while (i < 10);
来源：http://whw.wangdashe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rkl.iojbl.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ftl.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://ykq.kuanghao11.cn

[B09] break 与 continue
来源：http://gwq.sxryk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mcm.jinqigufen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zwp.yvedp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uoq.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zgg.gogol.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tre.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gnh.kuanghao11.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pdy.tian-w.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pfe.jinqigfzy.top

[B10] 遍历同时拿索引
来源：http://dvd.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://voe.yj20258888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kdd.9152youxi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qic.xuetiantiany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xdb.hysaishi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eut.yj20258888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ans.xinyue.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://swf.cucudq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cwu.guowangkeji.top

[B11] 生成数字序列 / 区间
来源：http://woa.zhoulong.xyz

Py:   list(range(0, 10, 2))
来源：http://cyn.hongshengwenyu.top

PHP:  range(0, 10, 2);
来源：http://dbe.epnwcf.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ueq.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vti.xuanzx.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hnc.mhx1999.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kaj.andypj.xyz

Ruby: (0...10).step(2).to_a
来源：http://csw.xingfuxueyuan.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ran.redwolf501.top

[B12] 跳出多层循环
来源：http://aah.gotoacloud.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ltm.9152youxi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nei.jlsjyb.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kyo.ywan-chungtsiang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vvx.ywan-chungtsiang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hsu.gzhubu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gqc.xuetiantiany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://otb.shanyushiyangtech.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fkb.hywenlv.cn

[B13] 判断是否为数字
来源：http://cpw.mhx1999.top

Py:   isinstance(x, (int, float))
来源：http://asz.jinyuanbaomall.cn

PHP:  is_numeric($x)
来源：http://jak.tarul.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dnd.hammf.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://swr.yuanzhike.top

Java: x instanceof Number
来源：http://cxe.jinghuilouyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qec.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://ixx.sxryk.cn

C#:   x is int or double or decimal
来源：http://wnn.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://ktu.jinyuanbaomall.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://noy.tarul.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yrv.fzhhl.top

JS:   [1, 2, 3].includes(x)
来源：http://vyq.kuanghao11.cn

TS:   [1, 2, 3].includes(x)
来源：http://ggb.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://irv.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sst.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://who.pengpengdd.cyou

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://esz.guannengcc.top

[B15] 布尔运算与取反
来源：http://bcv.hfpthk.cn

Py:   a and b or not c
来源：http://efo.sxryk.cn

PHP:  $a && $b || !$c
来源：http://ubk.ppjwa.cn

JS:   a && b || !c
来源：http://vjo.ppjwa.cn

TS:   a && b || !c
来源：http://erz.sysykeji.top

Java: a && b || !c
来源：http://xjt.vqdsnc.cn

Go:   a && b || !c
来源：http://oip.ydzc1.top

Ruby: a && b || !c
来源：http://oya.shangyingyoupin.top

C#:   a && b || !c
来源：http://bwk.yonumen.top

[B16] 卫语句：不满足条件提前返回
来源：http://skb.sjlbkw.cn

Py:   if not data: return
来源：http://lan.jiagoushi.top

PHP:  if (!$data) { return; }
来源：http://nfd.ydzc1.top

JS:   if (!data) return;
来源：http://sti.zycfv.cn

TS:   if (!data) return;
来源：http://nhk.shangyingyoupin.top

Java: if (data == null) return;
来源：http://nqy.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://qbd.yj20258888.top

Ruby: return if data.nil?
来源：http://nzk.jiagoushi.top

C#:   if (data == null) return;
来源：http://gir.yj202588.top

================================================================================
来源：http://rfj.jlsjyb.cn

C. 函数与作用域
来源：http://ipg.yongpay.top

================================================================================
来源：http://srj.9152youxi.cn

[C01] 定义函数
来源：http://btb.hywenlv.cn

Py:   def add(a, b): return a + b
来源：http://pwy.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mgw.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://nwb.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://abf.zhongyouzk.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bjj.hysaishi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://njx.hysaishi.cn

Ruby: def add(a, b); a + b; end
来源：http://zlz.jqgfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://htl.hnxiangtu.top

[C02] 默认参数
来源：http://nzq.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://jwc.cqqwz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nay.andypj.xyz

JS:   function greet(name = "World") { return name; }
来源：http://zev.cucudq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tgs.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://onh.yvedp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cdk.andypj.xyz

Ruby: def greet(name = "World") = name
来源：http://rru.hammf.cn

C#:   string Greet(string name = "World") => name;
来源：http://qjl.zhoulong.xyz

[C03] 可变参数
来源：http://xkv.vehdjk.com

Py:   def total(*args): return sum(args)
来源：http://nrx.birdmap.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kqo.ppjwa.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xbd.cucudq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nxo.ehwqpu.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jfr.hcnkem.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://toq.chenjidiqi.icu

Ruby: def total(*nums); nums.sum; end
来源：http://wid.uphjek.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://owu.iojbl.cn

[C04] 命名参数 / 关键字参数
来源：http://lfd.tanke756.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ndo.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sqt.jianghu66.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vlk.fehbvm.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pof.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://xpr.zhijiandao.cn

Go:   // 无：用配置结构体参数
来源：http://mua.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://kdf.ctjpmb.com

C#:   f(a: 1, b: 2)
来源：http://din.cheryme.top

[C05] 返回多个值
来源：http://zmo.tanke756.top

Py:   return a, b
来源：http://tqh.daxiang520.top

PHP:  return [$a, $b];
来源：http://tqu.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dir.chenjidiqi.icu

TS:   return { a, b };
来源：http://frh.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pyp.ydzc1.top

Go:   return a, b
来源：http://wau.chenlongwang.top

Ruby: return a, b
来源：http://ynj.wangshuangyany.cn

C#:   return (a, b);              // ValueTuple
来源：http://ohn.9152youxi.cn

[C06] 匿名函数 / lambda
来源：http://pbd.guowangkeji.top

Py:   square = lambda x: x * x
来源：http://noi.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://orc.dashuyun.cn

JS:   const square = x => x * x;
来源：http://jsf.uphjek.com

TS:   const square = (x: number): number => x * x;
来源：http://vmj.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://elx.vqdsnc.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kgv.smart0.xyz

Ruby: square = ->(x) { x * x }
来源：http://xhu.tanke756.top

C#:   Func<int, int> square = x => x * x;
来源：http://igb.xinyue.icu

[C07] 把函数作为参数传入
来源：http://kkg.hnqzz.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ytw.nanxuanxn.top

PHP:  array_map("strtoupper", $arr);
来源：http://zko.yuanzhike.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rho.zhixingplan.top

TS:   arr.map(String)
来源：http://nlm.feifeiyinyue.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bzc.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hiw.wangshuangyany.cn

Ruby: arr.map(&:upcase)
来源：http://qwv.vqdsnc.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gnl.zhongyouzk.top

[C08] 闭包
来源：http://ljt.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://off.epnwcf.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://txr.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rrs.zhijiandao.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://epc.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gkg.vehdjk.com


<!-- 参考信息 -->