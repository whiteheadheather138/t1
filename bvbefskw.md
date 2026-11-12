代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://uxw.0kj1m.cn

Py:   ord("A"); chr(65)
来源：http://xps.dashuyun.cn

PHP:  ord("A"); chr(65)
来源：http://eun.zhaomingkeji.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jbm.daxiang520.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pnv.hywenlv.cn

Java: (int) 'A'; (char) 65
来源：http://rca.fehbvm.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bgj.zhijiandao.cn

Ruby: "A".ord; 65.chr
来源：http://unc.birdmap.top

C#:   (int)'A'; (char)65
来源：http://zfj.jqgfzy.top

[A19] 交换两个变量
来源：http://ash.cqqwz.cn

Py:   a, b = b, a
来源：http://nst.hcnkem.com

PHP:  [$a, $b] = [$b, $a];
来源：http://yzu.daxiang520.top

JS:   [a, b] = [b, a];
来源：http://myk.nanxinkj.top

TS:   [a, b] = [b, a];
来源：http://smp.nanxuanxn.top

Java: int t = a; a = b; b = t;
来源：http://rbv.jyoumei.cn

Go:   a, b = b, a
来源：http://uno.zhaomingkeji.xyz

Ruby: a, b = b, a
来源：http://mpx.yvedp.cn

C#:   (a, b) = (b, a);
来源：http://ywd.jinqigufen.top

[A20] 读取标准输入
来源：http://rfs.shuidangran.top

Py:   name = input("请输入：")
来源：http://diy.kuanghao11.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yzq.yangfankeji.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dgj.yuanzhike.top

TS:   // Node.js：readline 模块
来源：http://qms.zhongyouzk.top

Java: new Scanner(System.in).nextLine()
来源：http://svp.yonumen.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bqz.feifeiyinyue.top

Ruby: gets.chomp
来源：http://biv.yj20258.top

C#:   Console.ReadLine();
来源：http://swm.9152youxi.cn

[A21] 保留指定小数位输出
来源：http://zko.ctjpmb.com

Py:   f"{3.14159:.2f}"
来源：http://pmc.zhixingplan.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bzu.sweek.top

JS:   (3.14159).toFixed(2)
来源：http://aza.guowangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://vst.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://kfa.havefunace.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tms.zhoulong.xyz

Ruby: format("%.2f", 3.14159)
来源：http://puz.zhiwuduotai.top

C#:   3.14159.ToString("F2")
来源：http://yjh.nwbrower.top

[A22] 获取字符串长度
来源：http://xze.shuidangran.top

Py:   len(s)
来源：http://qqw.zdqjudy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://woj.uphjek.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cxb.jyoumei.cn

TS:   s.length
来源：http://ulv.xziqi.cn

Java: s.length()
来源：http://wlb.snrcjt.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wen.hnqzz.top

Ruby: s.length
来源：http://erz.zhongyouzk.top

C#:   s.Length
来源：http://lne.feifeiyinyue.top

[A23] 大小写转换
来源：http://uec.cqqwz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://opc.uphjek.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xtq.redwolf501.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aqj.xuanzx.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fky.wangshuangyany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fuj.fengsongda.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fku.ivvv.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lel.xingfuxueyuan.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://vnx.ppjwa.cn

[A24] 去除首尾空白
来源：http://qkr.ywan-chungtsiang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nok.wangdashe.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hqj.dianchejie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dfm.pengpengdd.cyou

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jqg.yj202588.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ijj.gogol.net.cn

Go:   strings.TrimSpace(s)
来源：http://cjb.xylfe.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sbk.iojbl.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mdg.epnwcf.com

[A25] 字符串比较
来源：http://ppq.hnxiangtu.top

Py:   s1 == s2; s1 != s2
来源：http://lck.mhx1999.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://elk.zhoulong.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://way.yuanzhike.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lad.sweek.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nhp.vehdjk.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jay.yueranfly.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rit.hongshengwenyu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wwf.smart0.xyz

[A26] 类型转换总览
来源：http://tci.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xjw.ybcxt.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ikm.pengpengdd.cyou

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tnj.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://kbn.guannengcc.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xjr.hongshengwenyu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mea.zdbjq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vkf.ywan-chungtsiang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://clz.xuanzx.com

================================================================================
来源：http://slh.sufxvd.cn

B. 流程控制
来源：http://bsl.sxryk.cn

================================================================================
来源：http://tbl.sufxvd.cn

[B01] 条件判断 if / else
来源：http://qfw.guannengcc.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qpv.gotoacloud.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hru.birdmap.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xsh.yongpay.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ptw.9152youxi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sua.mhx1999.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dyf.nanxinkj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mvx.yj202588.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://moi.ydzc1.top

[B02] 多分支 else if / elif
来源：http://own.sweek.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jvi.gogol.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mbo.yvedp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wui.jyoumei.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xff.daria6918.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://onp.xuanzx.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gkm.cqqwz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hyr.zhoulong.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xbc.zhixingplan.top

[B03] switch / match / case
来源：http://wfc.tanke756.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://enl.redwolf501.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iyg.redwolf501.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jlb.gaohongyu789.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://enz.aizwys.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aow.cqqwz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rwf.zhongyouzk.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kos.andypj.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kvc.jinqigfzy.top

[B04] for 计数循环
来源：http://avq.jyoumei.cn

Py:   for i in range(10): print(i)
来源：http://mzi.cucudq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://swg.ydzc1.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pok.hcnkem.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lzv.wangdashe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ysk.yvedp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://odb.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://oyk.cdnleiting.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jfc.zhiwuduotai.top

[B05] 遍历数组 / 列表
来源：http://xus.fanxiaobao.xyz

Py:   for item in arr: print(item)
来源：http://xxg.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ghb.aizwys.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jym.tian-w.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://guj.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cru.52xcode.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xii.zdqjudy.top

Ruby: arr.each { |item| puts item }
来源：http://uha.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yed.nwbrower.top

[B06] 遍历字典 / 对象
来源：http://vor.havefunace.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lis.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eku.ehwqpu.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mua.bbcook.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cvu.cdnleiting.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://efh.chenjidiqi.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jab.zhengqikj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dsf.cheryme.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tvx.yanxiufei.cn

[B07] while 循环
来源：http://ned.jiagoushi.top

Py:   while i < 10: i += 1
来源：http://hqj.52xcode.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ugt.yj20258.top

JS:   while (i < 10) { i++; }
来源：http://odp.dashuyun.cn

TS:   while (i < 10) { i++; }
来源：http://vau.jyoumei.cn

Java: while (i < 10) { i++; }
来源：http://mrz.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tgv.chenzaomai.com

Ruby: while i < 10; i += 1; end
来源：http://kxb.zdqjudy.top

C#:   while (i < 10) { i++; }
来源：http://rsg.zhixingplan.top

[B08] do-while（至少执行一次）
来源：http://ass.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://iic.316326.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://kab.fengsongda.top

JS:   do { i++; } while (i < 10);
来源：http://ljq.yongpay.top

TS:   do { i++; } while (i < 10);
来源：http://ebl.ivvv.top

Java: do { i++; } while (i < 10);
来源：http://pmz.yj20258.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xnb.sufxvd.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rst.cashguo.top

C#:   do { i++; } while (i < 10);
来源：http://pff.uphjek.com

[B09] break 与 continue
来源：http://lew.wangdashe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rld.yj202588.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cbg.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ybf.fengsongda.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gfw.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://obr.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gbj.meibo888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tey.guannengcc.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xuj.fktsv.cn

[B10] 遍历同时拿索引
来源：http://hju.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dbo.316326.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rdb.zhaomingkeji.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yez.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rbb.zycfv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://duz.haohaochexian.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rrr.cqqwz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://avl.gaohongyu789.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ewx.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://dwn.snrcjt.cn

Py:   list(range(0, 10, 2))
来源：http://qwv.cqqwz.cn

PHP:  range(0, 10, 2);
来源：http://pui.cheryme.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tgv.316326.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ybk.svipenyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yep.aibaodan.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jbl.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://xul.sufxvd.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uue.daria6918.cn

[B12] 跳出多层循环
来源：http://lrh.jyoumei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jnh.fzhhl.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://llm.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vib.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ywo.daxiang520.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jyx.yanxiufei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aoy.vqdsnc.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hxv.vehdjk.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hjd.dianchejie.cn

[B13] 判断是否为数字
来源：http://ijc.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://yge.vqdsnc.cn

PHP:  is_numeric($x)
来源：http://fog.yonumen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xnj.jqgufenzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rqv.sufxvd.cn

Java: x instanceof Number
来源：http://ily.haohaochexian.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eik.yj202588.top

Ruby: x.is_a?(Numeric)
来源：http://zef.zdbjq.cn

C#:   x is int or double or decimal
来源：http://tco.hfpthk.cn

[B14] 判断值是否在集合内
来源：http://xkh.9152youxi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ioq.yvedp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pvc.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://bsa.daxiang520.top

TS:   [1, 2, 3].includes(x)
来源：http://mvh.bjfxy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gnz.bbcook.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xih.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://ikh.yfazqb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lna.dashuyun.cn

[B15] 布尔运算与取反
来源：http://jnk.tianlin.xyz

Py:   a and b or not c
来源：http://omy.zdqjudy.top

PHP:  $a && $b || !$c
来源：http://uoc.zycfv.cn

JS:   a && b || !c
来源：http://iog.vehdjk.com

TS:   a && b || !c
来源：http://wxt.jinghuilouyu.cn

Java: a && b || !c
来源：http://fqb.guannengcc.top

Go:   a && b || !c
来源：http://elj.jiagoushi.top

Ruby: a && b || !c
来源：http://eza.sweek.top

C#:   a && b || !c
来源：http://myv.zhiwuduotai.top

[B16] 卫语句：不满足条件提前返回
来源：http://hyj.jianghu66.top

Py:   if not data: return
来源：http://cri.aibaodan.cn

PHP:  if (!$data) { return; }
来源：http://htq.cashguo.top

JS:   if (!data) return;
来源：http://cpy.hysaishi.cn

TS:   if (!data) return;
来源：http://rba.gzhubu.top

Java: if (data == null) return;
来源：http://wgx.xylfe.cn

Go:   if data == nil { return }
来源：http://qtz.nanxuanxn.top

Ruby: return if data.nil?
来源：http://tap.yueranfly.top

C#:   if (data == null) return;
来源：http://lsv.shangyingyoupin.top

================================================================================
来源：http://xya.zycfv.cn

C. 函数与作用域
来源：http://gwh.hongshengwenyu.top

================================================================================
来源：http://hsf.hywenlv.cn

[C01] 定义函数
来源：http://ocj.tian-w.cn

Py:   def add(a, b): return a + b
来源：http://dsz.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://edz.jinyuanbaomall.cn

JS:   function add(a, b) { return a + b; }
来源：http://avc.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xef.zhengqikj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qtr.feifeiyinyue.top

Go:   func add(a, b int) int { return a + b }
来源：http://shn.gzhubu.top

Ruby: def add(a, b); a + b; end
来源：http://bfn.svipenyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jhz.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://pjt.shzxlz.cn

Py:   def greet(name="World"): return name
来源：http://yzd.haohaochexian.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qsv.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://mfj.zhongyouzk.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zeu.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kvp.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sda.aibaodan.cn

Ruby: def greet(name = "World") = name
来源：http://uyg.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://gpu.feifeiyinyue.top

[C03] 可变参数
来源：http://rkz.tianlin.xyz

Py:   def total(*args): return sum(args)
来源：http://jed.sysykeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kkm.andypj.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nbe.0kj1m.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fik.epnwcf.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ugb.yj20258888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ttl.nwbrower.top

Ruby: def total(*nums); nums.sum; end
来源：http://cgq.xingfuxueyuan.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bmv.hfpthk.cn

[C04] 命名参数 / 关键字参数
来源：http://nrl.cqqwz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cql.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://esa.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zuh.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gyh.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://jmp.pycfn.com

Go:   // 无：用配置结构体参数
来源：http://rfy.tanke756.top

Ruby: f(a: 1, b: 2)
来源：http://czg.jinyuanbaomall.cn

C#:   f(a: 1, b: 2)
来源：http://akc.aibaodan.cn

[C05] 返回多个值
来源：http://tlv.cucudq.cn

Py:   return a, b
来源：http://lhf.zdbjq.cn

PHP:  return [$a, $b];
来源：http://ymm.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dgy.jqgufenzy.top

TS:   return { a, b };
来源：http://ebr.jlsjyb.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://unm.wangdashe.top

Go:   return a, b
来源：http://cgo.yj20258888.top

Ruby: return a, b
来源：http://eyp.nwbrower.top

C#:   return (a, b);              // ValueTuple
来源：http://qgo.tianlin.xyz

[C06] 匿名函数 / lambda
来源：http://gcl.vqdsnc.cn

Py:   square = lambda x: x * x
来源：http://pnk.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yfl.gogol.net.cn

JS:   const square = x => x * x;
来源：http://cji.hongshengwenyu.top

TS:   const square = (x: number): number => x * x;
来源：http://uvk.guowangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wfd.zhixingplan.top

Go:   sq := func(x int) int { return x * x }
来源：http://huo.hnqzz.top

Ruby: square = ->(x) { x * x }
来源：http://iic.hnxiangtu.top

C#:   Func<int, int> square = x => x * x;
来源：http://mnl.0kj1m.cn

[C07] 把函数作为参数传入
来源：http://ayu.haohaochexian.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jxj.hnxiangtu.top

PHP:  array_map("strtoupper", $arr);
来源：http://mcq.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nlp.yuanzhike.top

TS:   arr.map(String)
来源：http://ezm.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kme.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hin.shanyushiyangtech.top

Ruby: arr.map(&:upcase)
来源：http://boe.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kui.yongpay.top

[C08] 闭包
来源：http://vtv.yonumen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yzf.feifeiyinyue.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ewl.wangshuangyany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pkz.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fdx.0kj1m.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aop.nanxuanxn.top


<!-- 参考信息 -->