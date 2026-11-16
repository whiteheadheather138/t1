代发 wailian999

C#:   (int)'A'; (char)65
来源：http://nct.tanke756.top

[A19] 交换两个变量
来源：http://gcp.yfazqb.com

Py:   a, b = b, a
来源：http://nwb.hammf.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wag.snrcjt.cn

JS:   [a, b] = [b, a];
来源：http://opw.pycfn.com

TS:   [a, b] = [b, a];
来源：http://lpd.nwbrower.top

Java: int t = a; a = b; b = t;
来源：http://hzs.chenlongwang.top

Go:   a, b = b, a
来源：http://drt.hnxiangtu.top

Ruby: a, b = b, a
来源：http://spd.aibaodan.cn

C#:   (a, b) = (b, a);
来源：http://fdz.yj20258888.top

[A20] 读取标准输入
来源：http://mei.daxiang520.top

Py:   name = input("请输入：")
来源：http://hzr.vehdjk.com

PHP:  $name = trim(fgets(STDIN));
来源：http://zoc.ybcxt.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fgi.zhoulong.xyz

TS:   // Node.js：readline 模块
来源：http://kal.ydjk.org.cn

Java: new Scanner(System.in).nextLine()
来源：http://jzp.9152youxi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fuk.yfazqb.com

Ruby: gets.chomp
来源：http://xko.gzhubu.top

C#:   Console.ReadLine();
来源：http://urg.yueranfly.top

[A21] 保留指定小数位输出
来源：http://xwu.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://uxu.kuanghao11.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jpr.hnqzz.top

JS:   (3.14159).toFixed(2)
来源：http://qfe.tanke756.top

TS:   (3.14159).toFixed(2)
来源：http://dxe.nanxinkj.top

Java: String.format("%.2f", 3.14159)
来源：http://wvj.hesvh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jff.bjfxy.top

Ruby: format("%.2f", 3.14159)
来源：http://tif.havefunace.top

C#:   3.14159.ToString("F2")
来源：http://kgl.cqqwz.cn

[A22] 获取字符串长度
来源：http://grs.hfpthk.cn

Py:   len(s)
来源：http://gxw.bjfxy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ssv.zycfv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://crz.jinqigfzy.top

TS:   s.length
来源：http://hin.shuidangran.top

Java: s.length()
来源：http://amg.aizwys.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bsm.jqgfzy.top

Ruby: s.length
来源：http://evk.ctjpmb.com

C#:   s.Length
来源：http://xyd.daxiang520.top

[A23] 大小写转换
来源：http://evo.aizwys.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://alo.pengpengdd.cyou

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ufj.shanyushiyangtech.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ubg.ywan-chungtsiang.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ikz.dashuyun.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ows.xylfe.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://faa.guannengcc.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sxy.zhijiandao.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xji.zdqjudy.top

[A24] 去除首尾空白
来源：http://vwu.yangfankeji.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vsk.shuidangran.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hel.yanxiufei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xcq.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://agb.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rts.yvedp.cn

Go:   strings.TrimSpace(s)
来源：http://lcx.quarkkingdee.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://imi.guowangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ggw.dianchejie.cn

[A25] 字符串比较
来源：http://npu.chenzaomai.com

Py:   s1 == s2; s1 != s2
来源：http://wym.jqgufenzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eta.nanxinkj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tcj.cdnleiting.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qjs.gzhubu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qjx.vehdjk.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xds.fktsv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rns.pengpengdd.cyou

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ffm.bbcook.cn

[A26] 类型转换总览
来源：http://eop.yongpay.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ven.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aco.sufxvd.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hqp.andypj.xyz

TS:   Number() String() Boolean() x as number
来源：http://wto.aizwys.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tyj.feifeiyinyue.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aql.ivvv.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ema.zdbjq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qfd.zhongyouzk.top

================================================================================
来源：http://ccd.hcnkem.com

B. 流程控制
来源：http://ppe.ivvv.top

================================================================================
来源：http://shd.pycfn.com

[B01] 条件判断 if / else
来源：http://mof.quarkkingdee.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rmb.hcnkem.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jtg.sysykeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://syr.meibo888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gmt.nanxinkj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://adc.gogol.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://adk.fehbvm.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lbl.shangyingyoupin.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ehy.ywan-chungtsiang.top

[B02] 多分支 else if / elif
来源：http://uwc.sweek.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cvc.haohaochexian.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aza.tarul.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rcn.xuetiantiany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tau.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pkr.cashguo.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ozk.uphjek.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uta.redwolf501.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://izu.zycfv.cn

[B03] switch / match / case
来源：http://abb.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fyd.zhixingplan.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://axn.yj20258.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nso.nanxinkj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kud.sjlbkw.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xrb.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tvl.zdqjudy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dwe.zhoulong.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://epx.redwolf501.top

[B04] for 计数循环
来源：http://puh.aizwys.cn

Py:   for i in range(10): print(i)
来源：http://yas.fzhhl.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yxw.ydzc1.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bvz.guannengcc.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fmy.ydjk.org.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pet.daria6918.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://noz.ywan-chungtsiang.top

Ruby: 10.times { |i| puts i }
来源：http://ngu.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wud.nanxinkj.top

[B05] 遍历数组 / 列表
来源：http://xtz.hfpthk.cn

Py:   for item in arr: print(item)
来源：http://exc.chenjidiqi.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gsi.bjfxy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cqh.hnqzz.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ajz.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rxz.ywan-chungtsiang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dtb.hnqzz.top

Ruby: arr.each { |item| puts item }
来源：http://apb.cashguo.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cnb.aizwys.cn

[B06] 遍历字典 / 对象
来源：http://mah.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uqr.ywan-chungtsiang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qgp.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dzj.vqdsnc.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://inu.9152youxi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aif.xuanzx.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jmh.hammf.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://psy.9152youxi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ktg.yvedp.cn

[B07] while 循环
来源：http://hvf.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://kpu.feifeiyinyue.top

PHP:  while ($i < 10) { $i++; }
来源：http://qpu.0kj1m.cn

JS:   while (i < 10) { i++; }
来源：http://uew.hywenlv.cn

TS:   while (i < 10) { i++; }
来源：http://fyc.yueranfly.top

Java: while (i < 10) { i++; }
来源：http://kgw.ywan-chungtsiang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uwq.sweek.top

Ruby: while i < 10; i += 1; end
来源：http://iqg.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://jmo.guannengcc.top

[B08] do-while（至少执行一次）
来源：http://uzi.fehbvm.com

Py:   # 无 do-while：用 while True + break
来源：http://rvi.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pnd.shanyushiyangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://mjs.nanxuanxn.top

TS:   do { i++; } while (i < 10);
来源：http://phn.yanxiufei.cn

Java: do { i++; } while (i < 10);
来源：http://ppz.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://dvi.hnxiangtu.top

Ruby: begin; i += 1; end while i < 10
来源：http://wxo.hywenlv.cn

C#:   do { i++; } while (i < 10);
来源：http://wri.havefunace.top

[B09] break 与 continue
来源：http://yoa.yanxiufei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jat.pengpengdd.cyou

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mjw.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ixt.jqgufenzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ime.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dak.dianchejie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dak.tanke756.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mod.sweek.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aas.zhoulong.xyz

[B10] 遍历同时拿索引
来源：http://wgz.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kty.nwbrower.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gvu.shanyushiyangtech.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tgm.zhoulong.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ilb.pycfn.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mxk.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xcl.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mlt.bjfxy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://avp.yj20258.top

[B11] 生成数字序列 / 区间
来源：http://ged.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://ypm.nanxuanxn.top

PHP:  range(0, 10, 2);
来源：http://kln.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wak.fzhhl.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jcl.ivvv.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ufo.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bei.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://kdp.dianchejie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://toj.tanke756.top

[B12] 跳出多层循环
来源：http://tly.gaohongyu789.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kwr.sjlbkw.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ldo.xylfe.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mup.yuanzhike.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lfo.fanxiaobao.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://epu.52xcode.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vuk.kuanghao11.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hii.dashuyun.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bex.hesvh.cn

[B13] 判断是否为数字
来源：http://vmg.xingfuxueyuan.xyz

Py:   isinstance(x, (int, float))
来源：http://smv.yueranfly.top

PHP:  is_numeric($x)
来源：http://orn.cucudq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pgv.ydzc1.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qlo.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://rch.52xcode.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tpi.ydzc1.top

Ruby: x.is_a?(Numeric)
来源：http://ptr.xylfe.cn

C#:   x is int or double or decimal
来源：http://taa.hywenlv.cn

[B14] 判断值是否在集合内
来源：http://zlb.jyoumei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mkm.jinqigufen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gni.sysykeji.top

JS:   [1, 2, 3].includes(x)
来源：http://zmt.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://hzo.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vts.c1oappe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://czy.yfazqb.com

Ruby: [1, 2, 3].include?(x)
来源：http://rbl.chenlongwang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lbc.chenzaomai.com

[B15] 布尔运算与取反
来源：http://twg.tarul.cn

Py:   a and b or not c
来源：http://xjc.kuanghao11.cn

PHP:  $a && $b || !$c
来源：http://iib.shanyushiyangkeji.top

JS:   a && b || !c
来源：http://pdq.dashuyun.cn

TS:   a && b || !c
来源：http://yai.iojbl.cn

Java: a && b || !c
来源：http://wsm.nwbrower.top

Go:   a && b || !c
来源：http://lvk.dashuyun.cn

Ruby: a && b || !c
来源：http://dgo.fanxiaobao.xyz

C#:   a && b || !c
来源：http://pox.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://mun.jlsjyb.cn

Py:   if not data: return
来源：http://vob.gaohongyu789.top

PHP:  if (!$data) { return; }
来源：http://llz.hfpthk.cn

JS:   if (!data) return;
来源：http://tbz.vehdjk.com

TS:   if (!data) return;
来源：http://eiz.pengpengdd.cyou

Java: if (data == null) return;
来源：http://kgv.sxryk.cn

Go:   if data == nil { return }
来源：http://phy.aibaodan.cn

Ruby: return if data.nil?
来源：http://wpx.uphjek.com

C#:   if (data == null) return;
来源：http://uok.tianlin.xyz

================================================================================
来源：http://avx.nwbrower.top

C. 函数与作用域
来源：http://hcd.guannengcc.top

================================================================================
来源：http://ncp.c1oappe.top

[C01] 定义函数
来源：http://wzj.0kj1m.cn

Py:   def add(a, b): return a + b
来源：http://xgj.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fyi.vqdsnc.cn

JS:   function add(a, b) { return a + b; }
来源：http://jxj.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wws.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vbu.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://cxm.xziqi.cn

Ruby: def add(a, b); a + b; end
来源：http://lxs.wangshuangyany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yex.fktsv.cn

[C02] 默认参数
来源：http://qqh.cucudq.cn

Py:   def greet(name="World"): return name
来源：http://fhk.yueranfly.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zyf.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://loz.hcnkem.com

TS:   function greet(name: string = "World") { return name; }
来源：http://ccr.hnxiangtu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mul.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lcs.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://gin.hcnkem.com

C#:   string Greet(string name = "World") => name;
来源：http://vqe.andypj.xyz

[C03] 可变参数
来源：http://cpa.jianghu66.top

Py:   def total(*args): return sum(args)
来源：http://fqr.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://usd.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uze.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pdx.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aun.yvedp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://obn.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://iya.ybcxt.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ufk.kuanghao11.cn

[C04] 命名参数 / 关键字参数
来源：http://hmo.yangfankeji.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ecl.andypj.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nhr.hcnkem.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mup.wangdashe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://shc.pengpengdd.cyou

Java: // 无：用 Builder 模式或 record
来源：http://bge.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://xfa.vqdsnc.cn

Ruby: f(a: 1, b: 2)
来源：http://jun.chenlongwang.top

C#:   f(a: 1, b: 2)
来源：http://ufv.sxryk.cn

[C05] 返回多个值
来源：http://zbp.hywenlv.cn

Py:   return a, b
来源：http://mke.chenlongwang.top

PHP:  return [$a, $b];
来源：http://tzm.yj20258888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xxe.yangfankeji.com

TS:   return { a, b };
来源：http://nuh.tanke756.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zbt.cashguo.top

Go:   return a, b
来源：http://oaj.haohaochexian.top

Ruby: return a, b
来源：http://zel.yonumen.top

C#:   return (a, b);              // ValueTuple
来源：http://ecu.dashuyun.cn

[C06] 匿名函数 / lambda
来源：http://rql.gzhubu.top

Py:   square = lambda x: x * x
来源：http://hlc.hnxiangtu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qkz.shzxlz.cn

JS:   const square = x => x * x;
来源：http://kks.daria6918.cn

TS:   const square = (x: number): number => x * x;
来源：http://qoq.jyoumei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nrm.chenlongwang.top

Go:   sq := func(x int) int { return x * x }
来源：http://wnv.shuidangran.top

Ruby: square = ->(x) { x * x }
来源：http://crb.aibaodan.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zyb.yongpay.top

[C07] 把函数作为参数传入
来源：http://dod.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bic.9152youxi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qpb.9152youxi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kwj.nwbrower.top

TS:   arr.map(String)
来源：http://zoz.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ffp.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aaz.bbcook.cn

Ruby: arr.map(&:upcase)
来源：http://gwz.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://nno.hywenlv.cn

[C08] 闭包
来源：http://ayb.cashguo.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gzb.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ibv.xuetiantiany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ubh.jiagoushi.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wje.feifeiyinyue.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sft.jinghuilouyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://knm.yanxiufei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://itm.gotoacloud.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ojf.epnwcf.com

[C09] 递归
来源：http://qco.jinqigfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zog.jinghuilouyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://noz.birdmap.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jzu.ydjk.org.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nxj.sxryk.cn


<!-- 参考信息 -->