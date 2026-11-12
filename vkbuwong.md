代发 wailian999

C#:   (int)'A'; (char)65
来源：http://jvo.sjlbkw.cn

[A19] 交换两个变量
来源：http://jqg.hesvh.cn

Py:   a, b = b, a
来源：http://zfa.epnwcf.com

PHP:  [$a, $b] = [$b, $a];
来源：http://pyh.haohaochexian.top

JS:   [a, b] = [b, a];
来源：http://ngy.nanxuanxn.top

TS:   [a, b] = [b, a];
来源：http://hbo.jlsjyb.cn

Java: int t = a; a = b; b = t;
来源：http://psm.hcnkem.com

Go:   a, b = b, a
来源：http://tng.dashuyun.cn

Ruby: a, b = b, a
来源：http://gvx.redwolf501.top

C#:   (a, b) = (b, a);
来源：http://qch.shanyushiyangtech.top

[A20] 读取标准输入
来源：http://pdk.redwolf501.top

Py:   name = input("请输入：")
来源：http://qfz.zdqjudy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bkb.vqdsnc.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://btc.snrcjt.cn

TS:   // Node.js：readline 模块
来源：http://oxs.zhiwuduotai.top

Java: new Scanner(System.in).nextLine()
来源：http://uan.shanyushiyangkeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vcd.fehbvm.com

Ruby: gets.chomp
来源：http://beg.yfazqb.com

C#:   Console.ReadLine();
来源：http://bks.hywenlv.cn

[A21] 保留指定小数位输出
来源：http://qup.zhengqikj.top

Py:   f"{3.14159:.2f}"
来源：http://lhx.hnxiangtu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://opx.hnqzz.top

JS:   (3.14159).toFixed(2)
来源：http://ldp.fanxiaobao.xyz

TS:   (3.14159).toFixed(2)
来源：http://zsa.nwbrower.top

Java: String.format("%.2f", 3.14159)
来源：http://wgb.bbcook.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sdc.fengsongda.top

Ruby: format("%.2f", 3.14159)
来源：http://igj.birdmap.top

C#:   3.14159.ToString("F2")
来源：http://hfr.zycfv.cn

[A22] 获取字符串长度
来源：http://umx.xziqi.cn

Py:   len(s)
来源：http://czs.yongpay.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zzh.yvedp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eus.fanxiaobao.xyz

TS:   s.length
来源：http://dxv.xuetiantiany.cn

Java: s.length()
来源：http://rbx.yj20258.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mjt.zdbjq.cn

Ruby: s.length
来源：http://abc.fzhhl.top

C#:   s.Length
来源：http://mum.chenjidiqi.icu

[A23] 大小写转换
来源：http://xnv.shzxlz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vtj.jinqigufen.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gti.chenjidiqi.icu

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ozz.fengsongda.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://riu.shanyushiyangtech.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jsa.xinyue.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://aoy.sxryk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oxz.tian-w.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ipy.tianlin.xyz

[A24] 去除首尾空白
来源：http://kuy.daxiang520.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gvu.ydzc1.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qtt.tian-w.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xpf.daria6918.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qqt.jiagoushi.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uaz.pycfn.com

Go:   strings.TrimSpace(s)
来源：http://rqg.ivvv.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://plo.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jjd.yj20258888.top

[A25] 字符串比较
来源：http://wym.zhaomingkeji.xyz

Py:   s1 == s2; s1 != s2
来源：http://evj.fktsv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pjd.tian-w.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eug.cdnleiting.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xvj.xuetiantiany.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kfd.iojbl.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xja.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://pzl.bjfxy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iqn.hongshengwenyu.top

[A26] 类型转换总览
来源：http://oli.ybcxt.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lwp.yuanzhike.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tha.tian-w.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sti.dianchejie.cn

TS:   Number() String() Boolean() x as number
来源：http://rao.haohaochexian.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cgh.chenlongwang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mag.9152youxi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://etw.aibaodan.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lmf.yj202588.top

================================================================================
来源：http://mqp.zhijiandao.cn

B. 流程控制
来源：http://szs.tian-w.cn

================================================================================
来源：http://qmq.shuidangran.top

[B01] 条件判断 if / else
来源：http://wnk.zycfv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lcj.hcnkem.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jfj.jinyuanbaomall.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vni.birdmap.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hcb.dianchejie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://swx.xingfuxueyuan.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ohd.jinqigufen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://udq.shuidangran.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sra.kuanghao11.cn

[B02] 多分支 else if / elif
来源：http://ofi.yuxming.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vct.ctjpmb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gya.birdmap.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uwh.fengsongda.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mhh.fktsv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://okr.uphjek.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wdy.gotoacloud.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ukv.0kj1m.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://piv.nanxinkj.top

[B03] switch / match / case
来源：http://tgl.birdmap.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://emk.sjlbkw.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ueh.shanyushiyangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lmh.yonumen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mnb.kuanghao11.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jrz.ppjwa.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://klf.gotoacloud.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pqi.zhongyouzk.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cgo.jyoumei.cn

[B04] for 计数循环
来源：http://ioh.jinqigfzy.top

Py:   for i in range(10): print(i)
来源：http://rkl.zhixingplan.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mvv.shuidangran.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yay.smart0.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bro.zhijiandao.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zuo.fanxiaobao.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iru.jinghuilouyu.cn

Ruby: 10.times { |i| puts i }
来源：http://anp.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zpt.ivvv.top

[B05] 遍历数组 / 列表
来源：http://wtc.dianchejie.cn

Py:   for item in arr: print(item)
来源：http://nsi.sjlbkw.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sqi.quarkkingdee.top

JS:   for (const item of arr) { console.log(item); }
来源：http://lci.yongpay.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xye.xuetiantiany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ius.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mpy.wangshuangyany.cn

Ruby: arr.each { |item| puts item }
来源：http://gce.meibo888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lyx.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://bym.cucudq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pld.pycfn.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dhv.jiagoushi.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vxj.jyoumei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hwx.zdqjudy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qep.quarkkingdee.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://svx.shanyushiyangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bsc.snrcjt.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ptk.zhaomingkeji.xyz

[B07] while 循环
来源：http://wxg.zhiwuduotai.top

Py:   while i < 10: i += 1
来源：http://tzf.dashuyun.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cnk.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://rox.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://bzh.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://eqb.fktsv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xun.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://crl.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://hgv.tarul.cn

[B08] do-while（至少执行一次）
来源：http://etu.pengpengdd.cyou

Py:   # 无 do-while：用 while True + break
来源：http://avh.fanxiaobao.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://rzl.zdbjq.cn

JS:   do { i++; } while (i < 10);
来源：http://bmx.xuetiantiany.cn

TS:   do { i++; } while (i < 10);
来源：http://jom.cqqwz.cn

Java: do { i++; } while (i < 10);
来源：http://yom.jinqigufen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kka.jianghu66.top

Ruby: begin; i += 1; end while i < 10
来源：http://whm.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://hmy.guannengcc.top

[B09] break 与 continue
来源：http://qpg.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jec.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://aik.tanke756.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lkl.jiagoushi.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://boy.vehdjk.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pab.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ghw.ydzc1.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ruk.yueranfly.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://whb.jyoumei.cn

[B10] 遍历同时拿索引
来源：http://xki.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fui.iojbl.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uyd.guannengcc.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kkx.jqgufenzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://itf.uphjek.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://siz.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oun.tarul.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ndb.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://stw.meibo888.top

[B11] 生成数字序列 / 区间
来源：http://kym.jlsjyb.cn

Py:   list(range(0, 10, 2))
来源：http://juf.dashuyun.cn

PHP:  range(0, 10, 2);
来源：http://dai.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bbb.zhongyouzk.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ndp.316326.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dth.yanxiufei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ibs.zdbjq.cn

Ruby: (0...10).step(2).to_a
来源：http://rsg.vqdsnc.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ivj.tianlin.xyz

[B12] 跳出多层循环
来源：http://ggz.pycfn.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://ppt.sysykeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ybn.uphjek.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qgw.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zbc.gaohongyu789.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zgo.gotoacloud.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pil.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eos.cucudq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://avr.yvedp.cn

[B13] 判断是否为数字
来源：http://til.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://bfd.jiagoushi.top

PHP:  is_numeric($x)
来源：http://lzn.chenlongwang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hwb.jinqigfzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bod.bjfxy.top

Java: x instanceof Number
来源：http://dir.gotoacloud.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zoe.fengsongda.top

Ruby: x.is_a?(Numeric)
来源：http://trm.yonumen.top

C#:   x is int or double or decimal
来源：http://nhn.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://gem.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xlj.sweek.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vec.yvedp.cn

JS:   [1, 2, 3].includes(x)
来源：http://zyg.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://ipt.yj20258888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vco.0kj1m.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pyk.gotoacloud.top

Ruby: [1, 2, 3].include?(x)
来源：http://vah.cqqwz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rfo.xziqi.cn

[B15] 布尔运算与取反
来源：http://zrq.0kj1m.cn

Py:   a and b or not c
来源：http://zpk.fktsv.cn

PHP:  $a && $b || !$c
来源：http://xpl.sxryk.cn

JS:   a && b || !c
来源：http://uyk.tianlin.xyz

TS:   a && b || !c
来源：http://gtv.jinqigufen.top

Java: a && b || !c
来源：http://kmd.havefunace.top

Go:   a && b || !c
来源：http://dnx.hammf.cn

Ruby: a && b || !c
来源：http://ctt.zhijiandao.cn

C#:   a && b || !c
来源：http://qvd.yuanzhike.top

[B16] 卫语句：不满足条件提前返回
来源：http://qcc.quarkkingdee.top

Py:   if not data: return
来源：http://ude.316326.xyz

PHP:  if (!$data) { return; }
来源：http://cqw.zycfv.cn

JS:   if (!data) return;
来源：http://tbl.chenjidiqi.icu

TS:   if (!data) return;
来源：http://joa.pycfn.com

Java: if (data == null) return;
来源：http://mzd.jinqigufen.top

Go:   if data == nil { return }
来源：http://mkx.snrcjt.cn

Ruby: return if data.nil?
来源：http://hnn.zdqjudy.top

C#:   if (data == null) return;
来源：http://ozs.smart0.xyz

================================================================================
来源：http://lpp.cucudq.cn

C. 函数与作用域
来源：http://ixp.jqgfzy.top

================================================================================
来源：http://snd.shzxlz.cn

[C01] 定义函数
来源：http://vsx.ywan-chungtsiang.top

Py:   def add(a, b): return a + b
来源：http://jqp.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hbw.tian-w.cn

JS:   function add(a, b) { return a + b; }
来源：http://gss.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rbr.birdmap.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nzm.shangyingyoupin.top

Go:   func add(a, b int) int { return a + b }
来源：http://nll.hongshengwenyu.top

Ruby: def add(a, b); a + b; end
来源：http://hcg.c1oappe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dfc.ydjk.org.cn

[C02] 默认参数
来源：http://fuu.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://epd.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://deq.fehbvm.com

JS:   function greet(name = "World") { return name; }
来源：http://ger.hysaishi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cir.jinqigufen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vdv.quarkkingdee.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ocm.cqqwz.cn

Ruby: def greet(name = "World") = name
来源：http://umt.zycfv.cn

C#:   string Greet(string name = "World") => name;
来源：http://ihk.vqdsnc.cn

[C03] 可变参数
来源：http://nvl.yfazqb.com

Py:   def total(*args): return sum(args)
来源：http://pjh.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jsq.daxiang520.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://acz.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pfi.wangdashe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://czo.shanyushiyangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vbs.xinyue.icu

Ruby: def total(*nums); nums.sum; end
来源：http://gjx.9152youxi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://daa.zhoulong.xyz

[C04] 命名参数 / 关键字参数
来源：http://udk.xinyue.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://acf.meibo888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ifl.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jxm.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qiy.shanyushiyangtech.top

Java: // 无：用 Builder 模式或 record
来源：http://fnz.nanxinkj.top

Go:   // 无：用配置结构体参数
来源：http://yol.ctjpmb.com

Ruby: f(a: 1, b: 2)
来源：http://zky.bjfxy.top

C#:   f(a: 1, b: 2)
来源：http://qnf.yonumen.top

[C05] 返回多个值
来源：http://lrs.hongshengwenyu.top

Py:   return a, b
来源：http://doz.cheryme.top

PHP:  return [$a, $b];
来源：http://jsf.xylfe.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ynh.c1oappe.top

TS:   return { a, b };
来源：http://tcb.52xcode.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dyc.zhiwuduotai.top

Go:   return a, b
来源：http://fwn.ctjpmb.com

Ruby: return a, b
来源：http://ckj.shanyushiyangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://dwu.jqgfzy.top

[C06] 匿名函数 / lambda
来源：http://ehd.hnqzz.top

Py:   square = lambda x: x * x
来源：http://pik.jinghuilouyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://guc.yj20258888.top

JS:   const square = x => x * x;
来源：http://hct.guowangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://xyv.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tzg.hfpthk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bjh.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://yon.gzhubu.top

C#:   Func<int, int> square = x => x * x;
来源：http://bex.hesvh.cn

[C07] 把函数作为参数传入
来源：http://qfo.fehbvm.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pch.dashuyun.cn

PHP:  array_map("strtoupper", $arr);
来源：http://elq.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dax.epnwcf.com

TS:   arr.map(String)
来源：http://oru.yj20258.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eba.meibo888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rdy.jqgufenzy.top

Ruby: arr.map(&:upcase)
来源：http://ing.guowangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pqq.cashguo.top

[C08] 闭包
来源：http://plr.chenzaomai.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fcp.ctjpmb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yxg.yanxiufei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yxw.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nsm.ydzc1.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nsm.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cte.yanxiufei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vvc.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ptu.pycfn.com

[C09] 递归
来源：http://gvr.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pwn.zhengqikj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hom.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ibi.xylfe.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qdj.snrcjt.cn


<!-- 参考信息 -->