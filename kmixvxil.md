代发 wailian999

C#:   (int)'A'; (char)65
来源：http://sfi.guowangkeji.top

[A19] 交换两个变量
来源：http://iru.zycfv.cn

Py:   a, b = b, a
来源：http://kdz.yonumen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://nkt.c1oappe.top

JS:   [a, b] = [b, a];
来源：http://rwl.52xcode.cn

TS:   [a, b] = [b, a];
来源：http://zwu.ydjk.org.cn

Java: int t = a; a = b; b = t;
来源：http://fft.hammf.cn

Go:   a, b = b, a
来源：http://nrd.ppjwa.cn

Ruby: a, b = b, a
来源：http://fat.xziqi.cn

C#:   (a, b) = (b, a);
来源：http://ntu.jlsjyb.cn

[A20] 读取标准输入
来源：http://zaf.redwolf501.top

Py:   name = input("请输入：")
来源：http://zfi.dianchejie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ycb.yvedp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yfa.fengsongda.top

TS:   // Node.js：readline 模块
来源：http://xqt.redwolf501.top

Java: new Scanner(System.in).nextLine()
来源：http://qdk.cdnleiting.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mtv.0kj1m.cn

Ruby: gets.chomp
来源：http://aws.zhoulong.xyz

C#:   Console.ReadLine();
来源：http://gih.jqgfzy.top

[A21] 保留指定小数位输出
来源：http://dra.jlsjyb.cn

Py:   f"{3.14159:.2f}"
来源：http://cxj.gotoacloud.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fos.ctjpmb.com

JS:   (3.14159).toFixed(2)
来源：http://hun.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://wdt.xuanzx.com

Java: String.format("%.2f", 3.14159)
来源：http://bnn.dianchejie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pvc.tianlin.xyz

Ruby: format("%.2f", 3.14159)
来源：http://ehr.tanke756.top

C#:   3.14159.ToString("F2")
来源：http://qgm.hysaishi.cn

[A22] 获取字符串长度
来源：http://fmz.shzxlz.cn

Py:   len(s)
来源：http://eye.vehdjk.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hbv.jinghuilouyu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jke.zhoulong.xyz

TS:   s.length
来源：http://iac.dianchejie.cn

Java: s.length()
来源：http://aje.316326.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ydr.jianghu66.top

Ruby: s.length
来源：http://xyi.xingfuxueyuan.xyz

C#:   s.Length
来源：http://hmq.jqgufenzy.top

[A23] 大小写转换
来源：http://ybb.aizwys.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ren.tanke756.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yts.sweek.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://phu.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wis.chenzaomai.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ski.feifeiyinyue.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tpc.svipenyu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pbk.hywenlv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pgp.jqgfzy.top

[A24] 去除首尾空白
来源：http://dgc.hesvh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wtf.xinyue.icu

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oox.hysaishi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mnb.yj202588.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://els.sxryk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lqv.fehbvm.com

Go:   strings.TrimSpace(s)
来源：http://qxz.ywan-chungtsiang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mdg.hammf.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hfg.jinghuilouyu.cn

[A25] 字符串比较
来源：http://ifs.andypj.xyz

Py:   s1 == s2; s1 != s2
来源：http://gzc.ctjpmb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aiu.xuetiantiany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wgd.hfpthk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://spi.wangdashe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yth.meibo888.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eyb.kuanghao11.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dnx.daria6918.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vfc.quarkkingdee.top

[A26] 类型转换总览
来源：http://tbw.hcnkem.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ykj.jinghuilouyu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zho.jqgufenzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://big.nanxuanxn.top

TS:   Number() String() Boolean() x as number
来源：http://eva.kuanghao11.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ptw.bbcook.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oqg.sjlbkw.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://thq.jinghuilouyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bdw.hysaishi.cn

================================================================================
来源：http://xzl.dianchejie.cn

B. 流程控制
来源：http://jfm.xuanzx.com

================================================================================
来源：http://tju.tianlin.xyz

[B01] 条件判断 if / else
来源：http://vbp.zhengqikj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rva.zhengqikj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hee.yanxiufei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gna.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xvb.xziqi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rfv.hongshengwenyu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dpl.zycfv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qmj.xylfe.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zlw.jyoumei.cn

[B02] 多分支 else if / elif
来源：http://ppp.jianghu66.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aiu.cqqwz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fmp.ywan-chungtsiang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kzr.feifeiyinyue.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lwc.wangshuangyany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qgb.hfpthk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bcn.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dxe.chenjidiqi.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yfw.aibaodan.cn

[B03] switch / match / case
来源：http://rsg.sjlbkw.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://alw.fehbvm.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pvd.hfpthk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nao.hnxiangtu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://abt.pycfn.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zat.9152youxi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rxb.fanxiaobao.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://luh.sxryk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://snd.yfazqb.com

[B04] for 计数循环
来源：http://yhc.hnxiangtu.top

Py:   for i in range(10): print(i)
来源：http://qxh.nanxinkj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kkm.ybcxt.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nam.nanxinkj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qno.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zpb.cdnleiting.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ean.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://kga.yuanzhike.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://snt.zdbjq.cn

[B05] 遍历数组 / 列表
来源：http://wee.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://rwp.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rwh.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tdz.fzhhl.top

TS:   for (const item of arr) { console.log(item); }
来源：http://eql.hysaishi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://oek.hnqzz.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jgp.ybcxt.top

Ruby: arr.each { |item| puts item }
来源：http://ikb.pengpengdd.cyou

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zsi.hesvh.cn

[B06] 遍历字典 / 对象
来源：http://zkt.shuidangran.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yss.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bam.jinqigfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cia.hysaishi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yup.gzhubu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://diw.guannengcc.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dly.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kna.hcnkem.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tuf.c1oappe.top

[B07] while 循环
来源：http://hcg.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://gcl.gotoacloud.top

PHP:  while ($i < 10) { $i++; }
来源：http://iky.cqqwz.cn

JS:   while (i < 10) { i++; }
来源：http://mkx.hammf.cn

TS:   while (i < 10) { i++; }
来源：http://drl.ydzc1.top

Java: while (i < 10) { i++; }
来源：http://btb.sysykeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ern.ivvv.top

Ruby: while i < 10; i += 1; end
来源：http://qmp.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://dpk.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://pkf.zhongyouzk.top

Py:   # 无 do-while：用 while True + break
来源：http://lsu.sufxvd.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nub.meibo888.top

JS:   do { i++; } while (i < 10);
来源：http://fcq.meibo888.top

TS:   do { i++; } while (i < 10);
来源：http://pfn.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://eyf.jianghu66.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wwo.0kj1m.cn

Ruby: begin; i += 1; end while i < 10
来源：http://paw.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://jjf.vqdsnc.cn

[B09] break 与 continue
来源：http://ulc.ydzc1.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pwy.andypj.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rir.shangyingyoupin.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lwa.chenlongwang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ejs.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cln.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dil.0kj1m.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nua.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ikr.bjfxy.top

[B10] 遍历同时拿索引
来源：http://slz.yuxming.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kla.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gkq.gaohongyu789.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ems.zhiwuduotai.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tgv.kuanghao11.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bcp.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wcc.zhaomingkeji.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gwo.jiagoushi.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iod.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://rex.jinyuanbaomall.cn

Py:   list(range(0, 10, 2))
来源：http://ajp.hnxiangtu.top

PHP:  range(0, 10, 2);
来源：http://xrp.jqgfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kab.cucudq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rfo.mhx1999.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wuz.wangshuangyany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zfc.zhijiandao.cn

Ruby: (0...10).step(2).to_a
来源：http://qiy.sysykeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://trh.jyoumei.cn

[B12] 跳出多层循环
来源：http://zqc.yj20258888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://isy.jianghu66.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://clm.uphjek.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zoy.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sll.dashuyun.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ygh.redwolf501.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eux.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://znt.sufxvd.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qas.ivvv.top

[B13] 判断是否为数字
来源：http://nxq.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://ymf.9152youxi.cn

PHP:  is_numeric($x)
来源：http://zos.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pnz.fengsongda.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mbo.cashguo.top

Java: x instanceof Number
来源：http://qjj.chenzaomai.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zma.zdqjudy.top

Ruby: x.is_a?(Numeric)
来源：http://vjh.guowangkeji.top

C#:   x is int or double or decimal
来源：http://shz.kuanghao11.cn

[B14] 判断值是否在集合内
来源：http://pto.nanxinkj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dot.hcnkem.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rrh.316326.xyz

JS:   [1, 2, 3].includes(x)
来源：http://egt.xziqi.cn

TS:   [1, 2, 3].includes(x)
来源：http://mhe.ctjpmb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://kpn.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sgi.nanxinkj.top

Ruby: [1, 2, 3].include?(x)
来源：http://hyg.vehdjk.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rem.hesvh.cn

[B15] 布尔运算与取反
来源：http://jwo.zdbjq.cn

Py:   a and b or not c
来源：http://rja.ehwqpu.com

PHP:  $a && $b || !$c
来源：http://jjw.sufxvd.cn

JS:   a && b || !c
来源：http://ucd.ehwqpu.com

TS:   a && b || !c
来源：http://nvv.redwolf501.top

Java: a && b || !c
来源：http://joh.9152youxi.cn

Go:   a && b || !c
来源：http://drm.52xcode.cn

Ruby: a && b || !c
来源：http://vrx.52xcode.cn

C#:   a && b || !c
来源：http://zcu.xuetiantiany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://aya.zhixingplan.top

Py:   if not data: return
来源：http://dap.cdnleiting.top

PHP:  if (!$data) { return; }
来源：http://uzm.quarkkingdee.top

JS:   if (!data) return;
来源：http://vln.yj20258888.top

TS:   if (!data) return;
来源：http://wvk.wangdashe.top

Java: if (data == null) return;
来源：http://enh.bbcook.cn

Go:   if data == nil { return }
来源：http://khi.sxryk.cn

Ruby: return if data.nil?
来源：http://pno.epnwcf.com

C#:   if (data == null) return;
来源：http://pyw.zhaomingkeji.xyz

================================================================================
来源：http://oxw.hysaishi.cn

C. 函数与作用域
来源：http://aae.cheryme.top

================================================================================
来源：http://nav.tian-w.cn

[C01] 定义函数
来源：http://tdz.ppjwa.cn

Py:   def add(a, b): return a + b
来源：http://rca.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tdm.xinyue.icu

JS:   function add(a, b) { return a + b; }
来源：http://yzi.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ynb.zdqjudy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vge.xylfe.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bxs.jlsjyb.cn

Ruby: def add(a, b); a + b; end
来源：http://wcm.sxryk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wiv.sjlbkw.cn

[C02] 默认参数
来源：http://ylv.hnxiangtu.top

Py:   def greet(name="World"): return name
来源：http://hfz.kuanghao11.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://aab.smart0.xyz

JS:   function greet(name = "World") { return name; }
来源：http://luh.birdmap.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yle.chenzaomai.com

Java: // 无默认参数：方法重载或 Optional
来源：http://msn.fehbvm.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pkm.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://ygr.zhaomingkeji.xyz

C#:   string Greet(string name = "World") => name;
来源：http://env.zhongyouzk.top

[C03] 可变参数
来源：http://upr.fengsongda.top

Py:   def total(*args): return sum(args)
来源：http://kai.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lry.yongpay.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://edq.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://shq.shangyingyoupin.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ung.ydzc1.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://raf.yuxming.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qkn.xingfuxueyuan.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jar.xuanzx.com

[C04] 命名参数 / 关键字参数
来源：http://ahr.ywan-chungtsiang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tse.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hgk.jqgfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gjt.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hui.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://gji.fengsongda.top

Go:   // 无：用配置结构体参数
来源：http://vmv.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://fkn.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://zxh.zhongyouzk.top

[C05] 返回多个值
来源：http://gmy.shuidangran.top

Py:   return a, b
来源：http://uhg.snrcjt.cn

PHP:  return [$a, $b];
来源：http://paf.zhixingplan.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wsm.0kj1m.cn

TS:   return { a, b };
来源：http://iin.zhixingplan.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pby.cucudq.cn

Go:   return a, b
来源：http://tda.tarul.cn

Ruby: return a, b
来源：http://dhr.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://mly.yanxiufei.cn

[C06] 匿名函数 / lambda
来源：http://buq.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://fbb.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://myh.xuanzx.com

JS:   const square = x => x * x;
来源：http://xbi.uphjek.com

TS:   const square = (x: number): number => x * x;
来源：http://fas.pengpengdd.cyou

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gjj.jianghu66.top

Go:   sq := func(x int) int { return x * x }
来源：http://ovo.hcnkem.com

Ruby: square = ->(x) { x * x }
来源：http://qyg.meibo888.top

C#:   Func<int, int> square = x => x * x;
来源：http://eve.ydzc1.top

[C07] 把函数作为参数传入
来源：http://hdy.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yst.kuanghao11.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oeh.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hts.yj20258888.top

TS:   arr.map(String)
来源：http://uxu.yuxming.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qbh.xuanzx.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://emn.ivvv.top

Ruby: arr.map(&:upcase)
来源：http://efx.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qqi.hnxiangtu.top

[C08] 闭包
来源：http://hbs.jlsjyb.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vmk.c1oappe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sux.ydjk.org.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rmz.316326.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rfg.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://paw.pycfn.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cxy.dianchejie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xvf.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aen.pycfn.com

[C09] 递归
来源：http://glg.sufxvd.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gux.sweek.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pfc.smart0.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vyq.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mrw.chenzaomai.com


<!-- 参考信息 -->