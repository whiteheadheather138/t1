代发 wailian999

C#:   (int)'A'; (char)65
来源：http://hwd.fktsv.cn

[A19] 交换两个变量
来源：http://htd.dianchejie.cn

Py:   a, b = b, a
来源：http://cdl.jinghuilouyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://atn.ywan-chungtsiang.top

JS:   [a, b] = [b, a];
来源：http://bmc.chenjidiqi.icu

TS:   [a, b] = [b, a];
来源：http://dkn.hnqzz.top

Java: int t = a; a = b; b = t;
来源：http://zad.haohaochexian.top

Go:   a, b = b, a
来源：http://kuq.ctjpmb.com

Ruby: a, b = b, a
来源：http://gwn.birdmap.top

C#:   (a, b) = (b, a);
来源：http://ifd.gotoacloud.top

[A20] 读取标准输入
来源：http://ryq.hfpthk.cn

Py:   name = input("请输入：")
来源：http://acj.cheryme.top

PHP:  $name = trim(fgets(STDIN));
来源：http://fnh.tianlin.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://klq.jqgfzy.top

TS:   // Node.js：readline 模块
来源：http://ltm.hysaishi.cn

Java: new Scanner(System.in).nextLine()
来源：http://acf.zhiwuduotai.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://slz.guowangkeji.top

Ruby: gets.chomp
来源：http://mtf.gaohongyu789.top

C#:   Console.ReadLine();
来源：http://vef.hnqzz.top

[A21] 保留指定小数位输出
来源：http://kba.daxiang520.top

Py:   f"{3.14159:.2f}"
来源：http://yks.tarul.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://agu.hnxiangtu.top

JS:   (3.14159).toFixed(2)
来源：http://rho.guowangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://ntn.ctjpmb.com

Java: String.format("%.2f", 3.14159)
来源：http://kdt.sxryk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gez.yanxiufei.cn

Ruby: format("%.2f", 3.14159)
来源：http://xey.chenzaomai.com

C#:   3.14159.ToString("F2")
来源：http://uxm.guowangkeji.top

[A22] 获取字符串长度
来源：http://zmh.yangfankeji.com

Py:   len(s)
来源：http://yrx.vehdjk.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ico.yj20258.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fcs.guowangkeji.top

TS:   s.length
来源：http://rzk.xziqi.cn

Java: s.length()
来源：http://dyr.sxryk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hfb.guowangkeji.top

Ruby: s.length
来源：http://jhc.quarkkingdee.top

C#:   s.Length
来源：http://haz.yangfankeji.com

[A23] 大小写转换
来源：http://kbf.tianlin.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://xxs.feifeiyinyue.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ywn.cqqwz.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vhm.redwolf501.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xja.shuidangran.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://awd.ppjwa.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zyg.ehwqpu.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kff.sysykeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ejy.yj20258888.top

[A24] 去除首尾空白
来源：http://nup.sufxvd.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tqo.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://edg.sufxvd.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uge.gaohongyu789.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qnc.yonumen.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qxs.jinqigufen.top

Go:   strings.TrimSpace(s)
来源：http://lxi.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vzf.zycfv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://guv.hywenlv.cn

[A25] 字符串比较
来源：http://wns.hnxiangtu.top

Py:   s1 == s2; s1 != s2
来源：http://ubr.fehbvm.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xhj.jqgfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vim.chenlongwang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qvg.cdnleiting.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jca.bjfxy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gca.fehbvm.com

Ruby: s1 == s2; s1 <=> s2
来源：http://osw.jqgfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lzq.zhijiandao.cn

[A26] 类型转换总览
来源：http://ckf.aizwys.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cyd.aizwys.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uct.guowangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://crp.yuanzhike.top

TS:   Number() String() Boolean() x as number
来源：http://wrl.zdbjq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yth.nwbrower.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://php.jqgfzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://yup.52xcode.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dsn.svipenyu.cn

================================================================================
来源：http://thj.yuxming.cn

B. 流程控制
来源：http://qlb.dianchejie.cn

================================================================================
来源：http://ryq.shuidangran.top

[B01] 条件判断 if / else
来源：http://tdh.gaohongyu789.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rmo.wangdashe.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eeg.yonumen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://svo.cucudq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tza.ivvv.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cit.hammf.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://out.dianchejie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tya.jyoumei.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zrc.c1oappe.top

[B02] 多分支 else if / elif
来源：http://cmn.shanyushiyangtech.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://krr.yj202588.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aud.ywan-chungtsiang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iec.zhoulong.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ewb.vqdsnc.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kxf.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zcr.cqqwz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://byg.dianchejie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bwi.sysykeji.top

[B03] switch / match / case
来源：http://ejq.ydjk.org.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://def.chenzaomai.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uxu.sweek.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kua.zdqjudy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cwb.redwolf501.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wts.xuanzx.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://opg.sysykeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tcy.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ypi.xuanzx.com

[B04] for 计数循环
来源：http://jnq.ivvv.top

Py:   for i in range(10): print(i)
来源：http://igl.nwbrower.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://txi.zhiwuduotai.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kve.fktsv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fgn.zdqjudy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qjm.nanxinkj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iqw.fktsv.cn

Ruby: 10.times { |i| puts i }
来源：http://skt.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qfb.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://fbl.pycfn.com

Py:   for item in arr: print(item)
来源：http://zgo.yj20258888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rpq.zhoulong.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://xea.shuidangran.top

TS:   for (const item of arr) { console.log(item); }
来源：http://avb.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://jkp.fehbvm.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ggm.guowangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://opg.bbcook.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yez.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://elk.chenjidiqi.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://awk.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zts.yj20258.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fld.9152youxi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://psg.snrcjt.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gar.yj20258888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://whs.gotoacloud.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mbo.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xrv.kuanghao11.cn

[B07] while 循环
来源：http://nqd.svipenyu.cn

Py:   while i < 10: i += 1
来源：http://oze.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://zpj.ydjk.org.cn

JS:   while (i < 10) { i++; }
来源：http://prp.dashuyun.cn

TS:   while (i < 10) { i++; }
来源：http://fdk.nwbrower.top

Java: while (i < 10) { i++; }
来源：http://wbo.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uni.jiagoushi.top

Ruby: while i < 10; i += 1; end
来源：http://ttr.shangyingyoupin.top

C#:   while (i < 10) { i++; }
来源：http://oam.xingfuxueyuan.xyz

[B08] do-while（至少执行一次）
来源：http://eos.jqgufenzy.top

Py:   # 无 do-while：用 while True + break
来源：http://tan.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://hob.redwolf501.top

JS:   do { i++; } while (i < 10);
来源：http://idt.cqqwz.cn

TS:   do { i++; } while (i < 10);
来源：http://kuz.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://ald.bbcook.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ddq.shanyushiyangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://zle.jinyuanbaomall.cn

C#:   do { i++; } while (i < 10);
来源：http://udq.tarul.cn

[B09] break 与 continue
来源：http://qba.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://akv.snrcjt.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xxr.tarul.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nis.chenzaomai.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hue.bjfxy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cqs.gzhubu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jlk.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blg.gogol.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fzi.hongshengwenyu.top

[B10] 遍历同时拿索引
来源：http://ohf.mhx1999.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fmi.chenzaomai.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ras.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qba.jyoumei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jsw.daxiang520.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aeq.hysaishi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qfk.zhijiandao.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dpc.aibaodan.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uvf.guannengcc.top

[B11] 生成数字序列 / 区间
来源：http://xpy.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://ehc.cashguo.top

PHP:  range(0, 10, 2);
来源：http://ndh.shuidangran.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ocz.quarkkingdee.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mln.feifeiyinyue.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kgo.bbcook.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xww.andypj.xyz

Ruby: (0...10).step(2).to_a
来源：http://lvx.wangshuangyany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://omh.hnqzz.top

[B12] 跳出多层循环
来源：http://gpo.hywenlv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jjg.quarkkingdee.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vqp.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://joz.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zjh.hysaishi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://irm.0kj1m.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://icy.daria6918.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tsg.jianghu66.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wng.pycfn.com

[B13] 判断是否为数字
来源：http://lwd.cashguo.top

Py:   isinstance(x, (int, float))
来源：http://hcu.jinghuilouyu.cn

PHP:  is_numeric($x)
来源：http://hjs.xylfe.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cbl.meibo888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tuj.jianghu66.top

Java: x instanceof Number
来源：http://vjz.ehwqpu.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ydh.jyoumei.cn

Ruby: x.is_a?(Numeric)
来源：http://buy.xuetiantiany.cn

C#:   x is int or double or decimal
来源：http://mfj.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://twh.zhongyouzk.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zop.xylfe.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rxc.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://sbl.vehdjk.com

TS:   [1, 2, 3].includes(x)
来源：http://sla.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hhi.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fki.sjlbkw.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kkn.xuanzx.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xug.cheryme.top

[B15] 布尔运算与取反
来源：http://tvp.ivvv.top

Py:   a and b or not c
来源：http://ved.hcnkem.com

PHP:  $a && $b || !$c
来源：http://gmt.epnwcf.com

JS:   a && b || !c
来源：http://ysm.birdmap.top

TS:   a && b || !c
来源：http://mxs.ivvv.top

Java: a && b || !c
来源：http://omn.tarul.cn

Go:   a && b || !c
来源：http://kiu.daxiang520.top

Ruby: a && b || !c
来源：http://frm.zhoulong.xyz

C#:   a && b || !c
来源：http://yoo.birdmap.top

[B16] 卫语句：不满足条件提前返回
来源：http://qgh.yj20258.top

Py:   if not data: return
来源：http://alg.xylfe.cn

PHP:  if (!$data) { return; }
来源：http://hwu.ehwqpu.com

JS:   if (!data) return;
来源：http://qen.mhx1999.top

TS:   if (!data) return;
来源：http://hnv.zhijiandao.cn

Java: if (data == null) return;
来源：http://uqd.ppjwa.cn

Go:   if data == nil { return }
来源：http://uix.cashguo.top

Ruby: return if data.nil?
来源：http://zfs.fanxiaobao.xyz

C#:   if (data == null) return;
来源：http://jzc.quarkkingdee.top

================================================================================
来源：http://ivt.sufxvd.cn

C. 函数与作用域
来源：http://vmi.dashuyun.cn

================================================================================
来源：http://llz.52xcode.cn

[C01] 定义函数
来源：http://cdd.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://rcz.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sdh.smart0.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ywz.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nbn.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ynu.haohaochexian.top

Go:   func add(a, b int) int { return a + b }
来源：http://ips.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://ugh.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://htb.feifeiyinyue.top

[C02] 默认参数
来源：http://ipw.hesvh.cn

Py:   def greet(name="World"): return name
来源：http://rzz.epnwcf.com

PHP:  function greet($name = "World") { return $name; }
来源：http://fnj.fehbvm.com

JS:   function greet(name = "World") { return name; }
来源：http://jvm.svipenyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ljv.xingfuxueyuan.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://wae.jqgfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cjc.yfazqb.com

Ruby: def greet(name = "World") = name
来源：http://gbe.quarkkingdee.top

C#:   string Greet(string name = "World") => name;
来源：http://glm.jqgfzy.top

[C03] 可变参数
来源：http://kru.9152youxi.cn

Py:   def total(*args): return sum(args)
来源：http://thp.yfazqb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bsu.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vsf.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://upm.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mlf.haohaochexian.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mug.cucudq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nei.hnxiangtu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://axu.yongpay.top

[C04] 命名参数 / 关键字参数
来源：http://gdw.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hdv.c1oappe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ibm.pengpengdd.cyou

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xfw.snrcjt.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wnu.snrcjt.cn

Java: // 无：用 Builder 模式或 record
来源：http://yxs.shanyushiyangtech.top

Go:   // 无：用配置结构体参数
来源：http://pjy.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://kfo.cucudq.cn

C#:   f(a: 1, b: 2)
来源：http://bpg.jiagoushi.top

[C05] 返回多个值
来源：http://qnh.zhaomingkeji.xyz

Py:   return a, b
来源：http://uiz.haohaochexian.top

PHP:  return [$a, $b];
来源：http://nwp.ydjk.org.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://eic.svipenyu.cn

TS:   return { a, b };
来源：http://anf.dashuyun.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lbb.xingfuxueyuan.xyz

Go:   return a, b
来源：http://cww.9152youxi.cn

Ruby: return a, b
来源：http://wwz.dashuyun.cn

C#:   return (a, b);              // ValueTuple
来源：http://jvk.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://imr.zhijiandao.cn

Py:   square = lambda x: x * x
来源：http://qys.kuanghao11.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gtd.jianghu66.top

JS:   const square = x => x * x;
来源：http://hcp.xylfe.cn

TS:   const square = (x: number): number => x * x;
来源：http://lsl.fehbvm.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nyd.jqgufenzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://dgh.nwbrower.top

Ruby: square = ->(x) { x * x }
来源：http://khe.tian-w.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xyo.cqqwz.cn

[C07] 把函数作为参数传入
来源：http://sbx.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kbk.zhongyouzk.top

PHP:  array_map("strtoupper", $arr);
来源：http://ecf.tian-w.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gop.cucudq.cn

TS:   arr.map(String)
来源：http://byg.andypj.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zsp.yj202588.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qxn.0kj1m.cn

Ruby: arr.map(&:upcase)
来源：http://xbj.zhaomingkeji.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://pdg.dashuyun.cn

[C08] 闭包
来源：http://fks.dianchejie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wbw.shanyushiyangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://git.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bwk.chenzaomai.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zur.jinghuilouyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://njw.daria6918.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qov.xingfuxueyuan.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://swx.guannengcc.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fto.316326.xyz

[C09] 递归
来源：http://hxk.pycfn.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ovr.pengpengdd.cyou

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rup.sxryk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zll.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vql.redwolf501.top


<!-- 参考信息 -->