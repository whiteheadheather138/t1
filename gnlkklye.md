代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://tmz.hysaishi.cn

Py:   ord("A"); chr(65)
来源：http://ass.daria6918.cn

PHP:  ord("A"); chr(65)
来源：http://pjl.daxiang520.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nuk.sxryk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vpi.hysaishi.cn

Java: (int) 'A'; (char) 65
来源：http://kmq.bbcook.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rzg.gzhubu.top

Ruby: "A".ord; 65.chr
来源：http://nsq.guowangkeji.top

C#:   (int)'A'; (char)65
来源：http://tiu.hongshengwenyu.top

[A19] 交换两个变量
来源：http://avr.tanke756.top

Py:   a, b = b, a
来源：http://ofj.sweek.top

PHP:  [$a, $b] = [$b, $a];
来源：http://noh.yvedp.cn

JS:   [a, b] = [b, a];
来源：http://nga.yuanzhike.top

TS:   [a, b] = [b, a];
来源：http://vat.redwolf501.top

Java: int t = a; a = b; b = t;
来源：http://fpc.yvedp.cn

Go:   a, b = b, a
来源：http://qex.hfpthk.cn

Ruby: a, b = b, a
来源：http://wtg.ydjk.org.cn

C#:   (a, b) = (b, a);
来源：http://sim.gzhubu.top

[A20] 读取标准输入
来源：http://myh.xinyue.icu

Py:   name = input("请输入：")
来源：http://gsx.cucudq.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://khj.hammf.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://igd.yueranfly.top

TS:   // Node.js：readline 模块
来源：http://woy.jqgufenzy.top

Java: new Scanner(System.in).nextLine()
来源：http://kwi.zhiwuduotai.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://urq.jqgufenzy.top

Ruby: gets.chomp
来源：http://hgn.dashuyun.cn

C#:   Console.ReadLine();
来源：http://shd.gotoacloud.top

[A21] 保留指定小数位输出
来源：http://dih.aibaodan.cn

Py:   f"{3.14159:.2f}"
来源：http://coj.tanke756.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mov.ivvv.top

JS:   (3.14159).toFixed(2)
来源：http://ztq.sweek.top

TS:   (3.14159).toFixed(2)
来源：http://ram.chenjidiqi.icu

Java: String.format("%.2f", 3.14159)
来源：http://gyj.jqgfzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lsj.redwolf501.top

Ruby: format("%.2f", 3.14159)
来源：http://npv.nanxuanxn.top

C#:   3.14159.ToString("F2")
来源：http://mxx.gotoacloud.top

[A22] 获取字符串长度
来源：http://bqb.snrcjt.cn

Py:   len(s)
来源：http://foq.bjfxy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://atn.bbcook.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://igw.zhongyouzk.top

TS:   s.length
来源：http://yzp.ivvv.top

Java: s.length()
来源：http://oeq.hcnkem.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wkv.guannengcc.top

Ruby: s.length
来源：http://lmw.ctjpmb.com

C#:   s.Length
来源：http://spt.hammf.cn

[A23] 大小写转换
来源：http://ocr.ybcxt.top

Py:   s.upper(); s.lower(); s.title()
来源：http://dzz.nwbrower.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dzt.ctjpmb.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tnb.hnxiangtu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hej.bjfxy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://brp.shzxlz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pfj.hysaishi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://guw.jinqigufen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dvk.kuanghao11.cn

[A24] 去除首尾空白
来源：http://xwv.zdbjq.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qkf.nanxinkj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tkh.xingfuxueyuan.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dah.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jhf.yvedp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yuc.daria6918.cn

Go:   strings.TrimSpace(s)
来源：http://uah.cucudq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aiq.yueranfly.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ylx.gzhubu.top

[A25] 字符串比较
来源：http://wto.52xcode.cn

Py:   s1 == s2; s1 != s2
来源：http://yez.ehwqpu.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ytj.andypj.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qmz.ctjpmb.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uzp.jianghu66.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zoe.xylfe.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rnk.zycfv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://imo.yangfankeji.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://scr.yuanzhike.top

[A26] 类型转换总览
来源：http://ips.c1oappe.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kju.hesvh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qze.gotoacloud.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pzq.shanyushiyangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://zlx.yongpay.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://agl.havefunace.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vsc.xuanzx.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://fdp.jqgufenzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rhl.feifeiyinyue.top

================================================================================
来源：http://zcz.sweek.top

B. 流程控制
来源：http://bgw.fzhhl.top

================================================================================
来源：http://rwh.yj20258888.top

[B01] 条件判断 if / else
来源：http://nkv.yuxming.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aot.ivvv.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mci.yj20258888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lip.yongpay.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ayk.ydjk.org.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://oxj.jinqigfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://whb.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iqm.xziqi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cnn.yvedp.cn

[B02] 多分支 else if / elif
来源：http://llg.fktsv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lux.feifeiyinyue.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zub.xuetiantiany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yrd.zhaomingkeji.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iua.yuxming.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zbc.yanxiufei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bdn.uphjek.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pmr.shangyingyoupin.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wrh.cashguo.top

[B03] switch / match / case
来源：http://zgf.cqqwz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tzu.zhongyouzk.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qph.sufxvd.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sho.fzhhl.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ihr.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hpx.daxiang520.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mps.bjfxy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rfm.sxryk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zck.hnxiangtu.top

[B04] for 计数循环
来源：http://kdg.tian-w.cn

Py:   for i in range(10): print(i)
来源：http://ezn.andypj.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blq.yanxiufei.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://drl.zycfv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://upk.bbcook.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ptw.tian-w.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ote.daria6918.cn

Ruby: 10.times { |i| puts i }
来源：http://ljc.yj20258.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dze.quarkkingdee.top

[B05] 遍历数组 / 列表
来源：http://egb.bjfxy.top

Py:   for item in arr: print(item)
来源：http://kzp.fanxiaobao.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://btq.cucudq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kef.feifeiyinyue.top

TS:   for (const item of arr) { console.log(item); }
来源：http://bdh.xylfe.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bfs.fanxiaobao.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vfg.yj202588.top

Ruby: arr.each { |item| puts item }
来源：http://bso.daxiang520.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fxk.feifeiyinyue.top

[B06] 遍历字典 / 对象
来源：http://gsj.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://zlu.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sbm.kuanghao11.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zes.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lsu.yj20258888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://txo.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ykv.yueranfly.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dvl.jinghuilouyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cwn.zhengqikj.top

[B07] while 循环
来源：http://wjo.zhijiandao.cn

Py:   while i < 10: i += 1
来源：http://mwe.yuxming.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dkx.uphjek.com

JS:   while (i < 10) { i++; }
来源：http://rat.redwolf501.top

TS:   while (i < 10) { i++; }
来源：http://vyj.daria6918.cn

Java: while (i < 10) { i++; }
来源：http://ldj.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://brt.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://rtq.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://wjc.shanyushiyangkeji.top

[B08] do-while（至少执行一次）
来源：http://vrq.zhiwuduotai.top

Py:   # 无 do-while：用 while True + break
来源：http://deo.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jva.jianghu66.top

JS:   do { i++; } while (i < 10);
来源：http://bhs.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://wpy.ehwqpu.com

Java: do { i++; } while (i < 10);
来源：http://rag.chenlongwang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jjl.cdnleiting.top

Ruby: begin; i += 1; end while i < 10
来源：http://yka.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://wie.0kj1m.cn

[B09] break 与 continue
来源：http://jlm.yfazqb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wce.zhiwuduotai.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ojl.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hsy.jinqigfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vdf.zhixingplan.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qdl.tian-w.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nvz.tarul.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xti.gogol.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ytf.zhoulong.xyz

[B10] 遍历同时拿索引
来源：http://goo.gaohongyu789.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zgo.shanyushiyangtech.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://spx.jinqigufen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zvf.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yks.andypj.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qlp.havefunace.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gwb.jinqigufen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kuw.zhixingplan.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fxl.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://apw.gzhubu.top

Py:   list(range(0, 10, 2))
来源：http://iyu.ydjk.org.cn

PHP:  range(0, 10, 2);
来源：http://stx.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hpa.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tmf.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vpk.tian-w.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dje.zhijiandao.cn

Ruby: (0...10).step(2).to_a
来源：http://hio.jiagoushi.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gbw.sysykeji.top

[B12] 跳出多层循环
来源：http://muk.yj20258888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rjq.jinyuanbaomall.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pqt.yueranfly.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://omb.316326.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mpq.feifeiyinyue.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wsw.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hwu.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qzf.hammf.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wfs.tarul.cn

[B13] 判断是否为数字
来源：http://whm.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://cfq.316326.xyz

PHP:  is_numeric($x)
来源：http://lni.shangyingyoupin.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mqs.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jxu.nwbrower.top

Java: x instanceof Number
来源：http://uer.fzhhl.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vyo.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://tkm.cqqwz.cn

C#:   x is int or double or decimal
来源：http://wai.nanxuanxn.top

[B14] 判断值是否在集合内
来源：http://egb.hesvh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://njx.sxryk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dnd.sysykeji.top

JS:   [1, 2, 3].includes(x)
来源：http://ich.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://bet.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://jil.cheryme.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://utb.chenjidiqi.icu

Ruby: [1, 2, 3].include?(x)
来源：http://fqp.zdqjudy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qxj.fehbvm.com

[B15] 布尔运算与取反
来源：http://mlh.tanke756.top

Py:   a and b or not c
来源：http://gds.bjfxy.top

PHP:  $a && $b || !$c
来源：http://udg.fktsv.cn

JS:   a && b || !c
来源：http://bcf.tanke756.top

TS:   a && b || !c
来源：http://sry.shangyingyoupin.top

Java: a && b || !c
来源：http://dro.yanxiufei.cn

Go:   a && b || !c
来源：http://gqo.daria6918.cn

Ruby: a && b || !c
来源：http://jve.pycfn.com

C#:   a && b || !c
来源：http://xnt.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://beg.xuetiantiany.cn

Py:   if not data: return
来源：http://kcn.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://vkw.chenjidiqi.icu

JS:   if (!data) return;
来源：http://las.zhaomingkeji.xyz

TS:   if (!data) return;
来源：http://srq.feifeiyinyue.top

Java: if (data == null) return;
来源：http://uez.yuxming.cn

Go:   if data == nil { return }
来源：http://pib.gaohongyu789.top

Ruby: return if data.nil?
来源：http://hyl.fktsv.cn

C#:   if (data == null) return;
来源：http://wqf.fktsv.cn

================================================================================
来源：http://ejz.xuanzx.com

C. 函数与作用域
来源：http://itg.dashuyun.cn

================================================================================
来源：http://cnx.ppjwa.cn

[C01] 定义函数
来源：http://ues.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://ojb.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pdq.52xcode.cn

JS:   function add(a, b) { return a + b; }
来源：http://vgt.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://atb.cqqwz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ent.epnwcf.com

Go:   func add(a, b int) int { return a + b }
来源：http://awf.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://eue.cheryme.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ijo.316326.xyz

[C02] 默认参数
来源：http://inw.chenlongwang.top

Py:   def greet(name="World"): return name
来源：http://twq.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://sql.nanxuanxn.top

JS:   function greet(name = "World") { return name; }
来源：http://soy.shanyushiyangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hcj.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zci.cdnleiting.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://psl.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://fhk.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://wmt.sufxvd.cn

[C03] 可变参数
来源：http://xgz.fzhhl.top

Py:   def total(*args): return sum(args)
来源：http://hvx.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://enk.xuetiantiany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nha.pengpengdd.cyou

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dni.sysykeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fms.kuanghao11.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nhe.zhijiandao.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zll.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://whd.hammf.cn

[C04] 命名参数 / 关键字参数
来源：http://ojz.yanxiufei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aue.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yaj.yj20258.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dmt.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://new.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://tek.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://qdj.tian-w.cn

Ruby: f(a: 1, b: 2)
来源：http://wou.yvedp.cn

C#:   f(a: 1, b: 2)
来源：http://grz.9152youxi.cn

[C05] 返回多个值
来源：http://rps.cashguo.top

Py:   return a, b
来源：http://aaz.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://aed.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ijf.zhixingplan.top

TS:   return { a, b };
来源：http://zkh.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tvo.jlsjyb.cn

Go:   return a, b
来源：http://atq.fzhhl.top

Ruby: return a, b
来源：http://pho.vehdjk.com

C#:   return (a, b);              // ValueTuple
来源：http://ofz.uphjek.com

[C06] 匿名函数 / lambda
来源：http://bnh.bbcook.cn

Py:   square = lambda x: x * x
来源：http://ybl.yangfankeji.com

PHP:  $square = fn($x) => $x * $x;
来源：http://phn.jlsjyb.cn

JS:   const square = x => x * x;
来源：http://cuj.hnxiangtu.top

TS:   const square = (x: number): number => x * x;
来源：http://eiz.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://skf.gogol.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ngk.cqqwz.cn

Ruby: square = ->(x) { x * x }
来源：http://rua.svipenyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hsp.pycfn.com

[C07] 把函数作为参数传入
来源：http://lgn.dashuyun.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zuy.uphjek.com

PHP:  array_map("strtoupper", $arr);
来源：http://eay.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ogx.nanxuanxn.top

TS:   arr.map(String)
来源：http://xkn.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tzr.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xfb.fengsongda.top

Ruby: arr.map(&:upcase)
来源：http://zhw.tarul.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zub.hywenlv.cn

[C08] 闭包
来源：http://jqz.svipenyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://afq.hysaishi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xge.xuetiantiany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mkp.ydzc1.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tgi.shanyushiyangtech.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ota.hammf.cn


<!-- 参考信息 -->