代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://dsh.yonumen.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ysh.jinqigfzy.top

TS:   // Node.js：readline 模块
来源：http://neg.wangshuangyany.cn

Java: new Scanner(System.in).nextLine()
来源：http://upg.sjlbkw.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dis.zhaomingkeji.xyz

Ruby: gets.chomp
来源：http://acn.jinqigfzy.top

C#:   Console.ReadLine();
来源：http://bwy.meibo888.top

[A21] 保留指定小数位输出
来源：http://cco.zdbjq.cn

Py:   f"{3.14159:.2f}"
来源：http://vwv.xingfuxueyuan.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tpj.cdnleiting.top

JS:   (3.14159).toFixed(2)
来源：http://yfj.chenjidiqi.icu

TS:   (3.14159).toFixed(2)
来源：http://apo.chenjidiqi.icu

Java: String.format("%.2f", 3.14159)
来源：http://hwi.svipenyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kjk.hywenlv.cn

Ruby: format("%.2f", 3.14159)
来源：http://xdq.dianchejie.cn

C#:   3.14159.ToString("F2")
来源：http://yvc.ivvv.top

[A22] 获取字符串长度
来源：http://hzl.snrcjt.cn

Py:   len(s)
来源：http://hju.ybcxt.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hzf.gaohongyu789.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lbl.aibaodan.cn

TS:   s.length
来源：http://ows.daria6918.cn

Java: s.length()
来源：http://hlk.jinqigufen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hwc.feifeiyinyue.top

Ruby: s.length
来源：http://iwt.shanyushiyangkeji.top

C#:   s.Length
来源：http://imy.bjfxy.top

[A23] 大小写转换
来源：http://gbf.cqqwz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nix.tanke756.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kxo.ydzc1.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rax.quarkkingdee.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://exd.zdbjq.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vca.tian-w.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ils.pycfn.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cyu.jiagoushi.top

C#:   s.ToUpper(); s.ToLower()
来源：http://eia.iojbl.cn

[A24] 去除首尾空白
来源：http://nki.daria6918.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ixo.cucudq.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qak.havefunace.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oti.jianghu66.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iuz.chenlongwang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uuq.shangyingyoupin.top

Go:   strings.TrimSpace(s)
来源：http://kyd.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rkg.ehwqpu.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rqb.pycfn.com

[A25] 字符串比较
来源：http://jip.epnwcf.com

Py:   s1 == s2; s1 != s2
来源：http://rgr.xingfuxueyuan.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sck.zhengqikj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lrb.ywan-chungtsiang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zxr.snrcjt.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sah.chenzaomai.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://laf.hcnkem.com

Ruby: s1 == s2; s1 <=> s2
来源：http://qxz.chenzaomai.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fai.zhongyouzk.top

[A26] 类型转换总览
来源：http://ayj.zycfv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qxn.zhoulong.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://epg.sysykeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fah.tanke756.top

TS:   Number() String() Boolean() x as number
来源：http://kgf.xuetiantiany.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hsw.52xcode.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pah.sxryk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hmu.yueranfly.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://std.xingfuxueyuan.xyz

================================================================================
来源：http://cmg.yvedp.cn

B. 流程控制
来源：http://puh.hammf.cn

================================================================================
来源：http://fmo.zycfv.cn

[B01] 条件判断 if / else
来源：http://tux.jinyuanbaomall.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zev.fanxiaobao.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tct.zhengqikj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xhh.xziqi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bya.gogol.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ipw.zdbjq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lna.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bro.dianchejie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gse.ppjwa.cn

[B02] 多分支 else if / elif
来源：http://xhg.sysykeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xjd.redwolf501.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wml.xuetiantiany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dmv.epnwcf.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rod.svipenyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://psc.zdbjq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jfz.vqdsnc.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hvx.kuanghao11.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fvm.guowangkeji.top

[B03] switch / match / case
来源：http://xuy.zdbjq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tya.birdmap.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fqt.ehwqpu.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zrr.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mui.andypj.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xjm.yj202588.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jae.hesvh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://afv.bjfxy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://upx.sxryk.cn

[B04] for 计数循环
来源：http://zzy.dashuyun.cn

Py:   for i in range(10): print(i)
来源：http://kvr.hywenlv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fpf.hammf.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://izi.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aww.fehbvm.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zxy.guowangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wec.pengpengdd.cyou

Ruby: 10.times { |i| puts i }
来源：http://bwq.gzhubu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nex.yj20258.top

[B05] 遍历数组 / 列表
来源：http://lys.fktsv.cn

Py:   for item in arr: print(item)
来源：http://uko.vqdsnc.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://try.tian-w.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rcs.yj202588.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tbf.zhengqikj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ygs.ydzc1.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wxz.ctjpmb.com

Ruby: arr.each { |item| puts item }
来源：http://ztj.zhijiandao.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pik.mhx1999.top

[B06] 遍历字典 / 对象
来源：http://cho.cdnleiting.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cet.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wij.yuanzhike.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://alo.snrcjt.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://igy.gzhubu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kfu.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xwu.birdmap.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yea.yuanzhike.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tsi.ybcxt.top

[B07] while 循环
来源：http://vqh.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://oxa.hongshengwenyu.top

PHP:  while ($i < 10) { $i++; }
来源：http://wii.hcnkem.com

JS:   while (i < 10) { i++; }
来源：http://uxf.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://sbv.jqgfzy.top

Java: while (i < 10) { i++; }
来源：http://omx.daria6918.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rel.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://mlj.9152youxi.cn

C#:   while (i < 10) { i++; }
来源：http://cqw.mhx1999.top

[B08] do-while（至少执行一次）
来源：http://tyq.ydzc1.top

Py:   # 无 do-while：用 while True + break
来源：http://fix.andypj.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://dkf.shangyingyoupin.top

JS:   do { i++; } while (i < 10);
来源：http://ipk.guowangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://ajq.meibo888.top

Java: do { i++; } while (i < 10);
来源：http://pmk.birdmap.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fcj.redwolf501.top

Ruby: begin; i += 1; end while i < 10
来源：http://phm.zdqjudy.top

C#:   do { i++; } while (i < 10);
来源：http://qxl.xuanzx.com

[B09] break 与 continue
来源：http://pyi.gotoacloud.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lka.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tqr.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xkn.uphjek.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jpc.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gpz.316326.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bzk.316326.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gsn.tarul.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xuk.zdqjudy.top

[B10] 遍历同时拿索引
来源：http://imb.meibo888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kor.guowangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aln.yj202588.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zcb.quarkkingdee.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://clj.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jkc.jyoumei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lxh.nwbrower.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ijx.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uza.sufxvd.cn

[B11] 生成数字序列 / 区间
来源：http://gyw.meibo888.top

Py:   list(range(0, 10, 2))
来源：http://pmt.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://exz.316326.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://inz.sysykeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zyx.sjlbkw.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bwe.fktsv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ifx.hammf.cn

Ruby: (0...10).step(2).to_a
来源：http://hxs.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iiy.yj202588.top

[B12] 跳出多层循环
来源：http://eus.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yow.fzhhl.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xwd.chenzaomai.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zqr.chenlongwang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uht.havefunace.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hon.hysaishi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uto.ehwqpu.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wfc.jlsjyb.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eyr.wangshuangyany.cn

[B13] 判断是否为数字
来源：http://rig.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://jrw.jiagoushi.top

PHP:  is_numeric($x)
来源：http://foi.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tmq.shangyingyoupin.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jxj.shanyushiyangtech.top

Java: x instanceof Number
来源：http://lkz.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qua.shangyingyoupin.top

Ruby: x.is_a?(Numeric)
来源：http://ugg.ywan-chungtsiang.top

C#:   x is int or double or decimal
来源：http://dbg.tian-w.cn

[B14] 判断值是否在集合内
来源：http://iss.xingfuxueyuan.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vbl.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wjx.tianlin.xyz

JS:   [1, 2, 3].includes(x)
来源：http://yiy.chenjidiqi.icu

TS:   [1, 2, 3].includes(x)
来源：http://mqp.jqgfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yfk.ybcxt.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://igs.yongpay.top

Ruby: [1, 2, 3].include?(x)
来源：http://rxv.nanxinkj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ewd.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://oog.gaohongyu789.top

Py:   a and b or not c
来源：http://trp.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://dbe.jyoumei.cn

JS:   a && b || !c
来源：http://bhj.jqgfzy.top

TS:   a && b || !c
来源：http://rbc.xziqi.cn

Java: a && b || !c
来源：http://zws.zycfv.cn

Go:   a && b || !c
来源：http://xjv.sweek.top

Ruby: a && b || !c
来源：http://wmn.cqqwz.cn

C#:   a && b || !c
来源：http://izz.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://nsn.wangdashe.top

Py:   if not data: return
来源：http://nje.cashguo.top

PHP:  if (!$data) { return; }
来源：http://gjc.c1oappe.top

JS:   if (!data) return;
来源：http://rlz.fengsongda.top

TS:   if (!data) return;
来源：http://pkb.yuanzhike.top

Java: if (data == null) return;
来源：http://gty.zhoulong.xyz

Go:   if data == nil { return }
来源：http://qsp.xylfe.cn

Ruby: return if data.nil?
来源：http://cgk.cashguo.top

C#:   if (data == null) return;
来源：http://fgx.fengsongda.top

================================================================================
来源：http://hie.ydjk.org.cn

C. 函数与作用域
来源：http://ewu.yuanzhike.top

================================================================================
来源：http://huq.yangfankeji.com

[C01] 定义函数
来源：http://ucm.sysykeji.top

Py:   def add(a, b): return a + b
来源：http://int.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gvm.c1oappe.top

JS:   function add(a, b) { return a + b; }
来源：http://dzv.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://evj.gzhubu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xng.jqgufenzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://qwg.tianlin.xyz

Ruby: def add(a, b); a + b; end
来源：http://aeb.xinyue.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dwi.snrcjt.cn

[C02] 默认参数
来源：http://alz.316326.xyz

Py:   def greet(name="World"): return name
来源：http://dct.bjfxy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xxi.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://taw.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://afq.mhx1999.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nqi.cashguo.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ftd.zhengqikj.top

Ruby: def greet(name = "World") = name
来源：http://dzo.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://svx.cqqwz.cn

[C03] 可变参数
来源：http://nnt.gzhubu.top

Py:   def total(*args): return sum(args)
来源：http://irk.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zrj.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sgs.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wca.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://osv.yanxiufei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fox.xziqi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://iua.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mcz.smart0.xyz

[C04] 命名参数 / 关键字参数
来源：http://xku.jinyuanbaomall.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nyy.sxryk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oda.yonumen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jwr.zhijiandao.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lpr.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://rrm.9152youxi.cn

Go:   // 无：用配置结构体参数
来源：http://ivg.yvedp.cn

Ruby: f(a: 1, b: 2)
来源：http://hmg.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://pks.feifeiyinyue.top

[C05] 返回多个值
来源：http://uod.hesvh.cn

Py:   return a, b
来源：http://ana.ivvv.top

PHP:  return [$a, $b];
来源：http://czk.wangdashe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qbb.gzhubu.top

TS:   return { a, b };
来源：http://dct.zdqjudy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vqs.shzxlz.cn

Go:   return a, b
来源：http://sbo.yongpay.top

Ruby: return a, b
来源：http://nip.tian-w.cn

C#:   return (a, b);              // ValueTuple
来源：http://qgs.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://gfo.sysykeji.top

Py:   square = lambda x: x * x
来源：http://uwl.xylfe.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rip.nwbrower.top

JS:   const square = x => x * x;
来源：http://qwq.zhaomingkeji.xyz

TS:   const square = (x: number): number => x * x;
来源：http://ywi.hywenlv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dio.9152youxi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dlj.zhongyouzk.top

Ruby: square = ->(x) { x * x }
来源：http://ofx.fehbvm.com

C#:   Func<int, int> square = x => x * x;
来源：http://yft.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://axz.sjlbkw.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tea.epnwcf.com

PHP:  array_map("strtoupper", $arr);
来源：http://hjb.shuidangran.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jvj.hesvh.cn

TS:   arr.map(String)
来源：http://acl.hfpthk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://otq.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kgv.ywan-chungtsiang.top

Ruby: arr.map(&:upcase)
来源：http://kss.aizwys.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rce.redwolf501.top

[C08] 闭包
来源：http://mry.aibaodan.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vtm.xuetiantiany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oik.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bka.xuanzx.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cim.shanyushiyangtech.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pfm.chenjidiqi.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jvq.tarul.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nji.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bmg.hnqzz.top

[C09] 递归
来源：http://uuy.cucudq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hzz.dianchejie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jxr.tanke756.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://plg.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gpj.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ewk.jlsjyb.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rsx.mhx1999.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bad.bbcook.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gyi.smart0.xyz

[C10] 变量作用域
来源：http://fpb.sjlbkw.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jhk.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cmf.andypj.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hqc.feifeiyinyue.top

TS:   同 JS
来源：http://erl.epnwcf.com

Java: 方法内为块级作用域
来源：http://qcl.shzxlz.cn

Go:   花括号块级作用域
来源：http://pgp.cucudq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://atu.meibo888.top


<!-- 参考信息 -->