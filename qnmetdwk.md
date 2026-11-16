代发 wailian999

JS:   [a, b] = [b, a];
来源：http://scl.xuanzx.com

TS:   [a, b] = [b, a];
来源：http://zea.52xcode.cn

Java: int t = a; a = b; b = t;
来源：http://rwq.uphjek.com

Go:   a, b = b, a
来源：http://ezb.zdqjudy.top

Ruby: a, b = b, a
来源：http://gaw.fehbvm.com

C#:   (a, b) = (b, a);
来源：http://afb.yuanzhike.top

[A20] 读取标准输入
来源：http://drc.aizwys.cn

Py:   name = input("请输入：")
来源：http://xcf.nanxinkj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rxx.shangyingyoupin.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://prr.pycfn.com

TS:   // Node.js：readline 模块
来源：http://rcc.sjlbkw.cn

Java: new Scanner(System.in).nextLine()
来源：http://pow.uphjek.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rpr.xuetiantiany.cn

Ruby: gets.chomp
来源：http://gmf.cqqwz.cn

C#:   Console.ReadLine();
来源：http://ktr.316326.xyz

[A21] 保留指定小数位输出
来源：http://kox.hysaishi.cn

Py:   f"{3.14159:.2f}"
来源：http://jbj.gogol.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ygj.quarkkingdee.top

JS:   (3.14159).toFixed(2)
来源：http://vxh.xziqi.cn

TS:   (3.14159).toFixed(2)
来源：http://qqq.chenzaomai.com

Java: String.format("%.2f", 3.14159)
来源：http://fzs.zdqjudy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ewg.smart0.xyz

Ruby: format("%.2f", 3.14159)
来源：http://hpi.fktsv.cn

C#:   3.14159.ToString("F2")
来源：http://hlt.jqgfzy.top

[A22] 获取字符串长度
来源：http://hnp.bjfxy.top

Py:   len(s)
来源：http://hcd.yuanzhike.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yql.zhijiandao.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pei.yongpay.top

TS:   s.length
来源：http://tqg.zhengqikj.top

Java: s.length()
来源：http://yiw.9152youxi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://aou.snrcjt.cn

Ruby: s.length
来源：http://joy.fehbvm.com

C#:   s.Length
来源：http://zfb.cqqwz.cn

[A23] 大小写转换
来源：http://wvt.52xcode.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pau.ybcxt.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fkp.sufxvd.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mpe.shanyushiyangtech.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ynf.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gwo.hammf.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wkt.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://obx.hnqzz.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qsi.hammf.cn

[A24] 去除首尾空白
来源：http://bjx.fzhhl.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bgf.yangfankeji.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jey.gogol.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mxb.quarkkingdee.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://usd.nanxuanxn.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hmj.xinyue.icu

Go:   strings.TrimSpace(s)
来源：http://djj.xylfe.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://thd.tianlin.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aqa.0kj1m.cn

[A25] 字符串比较
来源：http://tde.haohaochexian.top

Py:   s1 == s2; s1 != s2
来源：http://ewo.mhx1999.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qja.hammf.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vlv.shuidangran.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wsh.redwolf501.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dvm.tanke756.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://upu.kuanghao11.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://epo.ctjpmb.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tuu.hnqzz.top

[A26] 类型转换总览
来源：http://beg.bbcook.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xet.sjlbkw.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cdi.guowangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wxj.nanxinkj.top

TS:   Number() String() Boolean() x as number
来源：http://kkr.cqqwz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lgg.hysaishi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lvy.yanxiufei.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yyo.yanxiufei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kvl.tarul.cn

================================================================================
来源：http://ing.jinghuilouyu.cn

B. 流程控制
来源：http://rbn.jinqigufen.top

================================================================================
来源：http://yvq.yueranfly.top

[B01] 条件判断 if / else
来源：http://kzh.shuidangran.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vii.iojbl.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://edb.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lis.nwbrower.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fnj.haohaochexian.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jdx.meibo888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tle.yangfankeji.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://evw.fehbvm.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nfu.sjlbkw.cn

[B02] 多分支 else if / elif
来源：http://ila.gaohongyu789.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uqh.pycfn.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lsj.tian-w.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eos.jiagoushi.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://frv.svipenyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://inb.vehdjk.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vad.hnxiangtu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://osd.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hae.haohaochexian.top

[B03] switch / match / case
来源：http://otu.cqqwz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lxv.yfazqb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://coh.quarkkingdee.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fji.smart0.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dzm.yuanzhike.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://khm.chenzaomai.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eda.vehdjk.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nzz.shanyushiyangtech.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vzx.pengpengdd.cyou

[B04] for 计数循环
来源：http://qpk.tianlin.xyz

Py:   for i in range(10): print(i)
来源：http://wed.feifeiyinyue.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ypa.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yar.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fya.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ixk.ppjwa.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yim.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://obx.wangshuangyany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sri.meibo888.top

[B05] 遍历数组 / 列表
来源：http://jhc.hfpthk.cn

Py:   for item in arr: print(item)
来源：http://emk.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://opj.cqqwz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ayh.epnwcf.com

TS:   for (const item of arr) { console.log(item); }
来源：http://jyz.tarul.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ffi.cucudq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pqx.bbcook.cn

Ruby: arr.each { |item| puts item }
来源：http://jgl.hnxiangtu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://onx.dashuyun.cn

[B06] 遍历字典 / 对象
来源：http://vcd.shanyushiyangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hnx.dashuyun.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ueh.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gqm.yfazqb.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://meu.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nsp.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vkb.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xtt.zhiwuduotai.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ile.fktsv.cn

[B07] while 循环
来源：http://tab.yvedp.cn

Py:   while i < 10: i += 1
来源：http://yvr.zhijiandao.cn

PHP:  while ($i < 10) { $i++; }
来源：http://brv.ybcxt.top

JS:   while (i < 10) { i++; }
来源：http://akt.sweek.top

TS:   while (i < 10) { i++; }
来源：http://jyd.iojbl.cn

Java: while (i < 10) { i++; }
来源：http://csd.zhongyouzk.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://abu.ywan-chungtsiang.top

Ruby: while i < 10; i += 1; end
来源：http://yzn.yuanzhike.top

C#:   while (i < 10) { i++; }
来源：http://puk.yangfankeji.com

[B08] do-while（至少执行一次）
来源：http://omx.zhaomingkeji.xyz

Py:   # 无 do-while：用 while True + break
来源：http://tij.aizwys.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fvc.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://fxe.fengsongda.top

TS:   do { i++; } while (i < 10);
来源：http://mpz.chenjidiqi.icu

Java: do { i++; } while (i < 10);
来源：http://hsb.bjfxy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mrm.fengsongda.top

Ruby: begin; i += 1; end while i < 10
来源：http://hvr.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://rhc.fktsv.cn

[B09] break 与 continue
来源：http://wzm.tianlin.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cgi.nanxinkj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://foq.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xke.ehwqpu.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nit.hfpthk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pjl.smart0.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fvl.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yro.yuanzhike.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gnr.zhijiandao.cn

[B10] 遍历同时拿索引
来源：http://tvn.bbcook.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qax.wangshuangyany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://shi.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hvh.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://khs.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dmb.sjlbkw.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bdw.hcnkem.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zpv.epnwcf.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cbt.kuanghao11.cn

[B11] 生成数字序列 / 区间
来源：http://lve.nanxuanxn.top

Py:   list(range(0, 10, 2))
来源：http://otm.zhoulong.xyz

PHP:  range(0, 10, 2);
来源：http://bgh.gogol.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sxj.yfazqb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ord.yj20258.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gbn.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tmw.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://dlx.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gpi.shanyushiyangtech.top

[B12] 跳出多层循环
来源：http://aav.sjlbkw.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lyf.zdbjq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zbf.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vxl.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zws.bjfxy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nuf.zdbjq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ryo.chenjidiqi.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ekc.yueranfly.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bvf.mhx1999.top

[B13] 判断是否为数字
来源：http://svt.jlsjyb.cn

Py:   isinstance(x, (int, float))
来源：http://dcw.fzhhl.top

PHP:  is_numeric($x)
来源：http://jpa.jqgufenzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dsc.meibo888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mry.haohaochexian.top

Java: x instanceof Number
来源：http://mgd.sjlbkw.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wvc.nanxinkj.top

Ruby: x.is_a?(Numeric)
来源：http://dvy.jinqigufen.top

C#:   x is int or double or decimal
来源：http://vcg.kuanghao11.cn

[B14] 判断值是否在集合内
来源：http://kpd.sufxvd.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rnq.yvedp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ftj.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://qow.haohaochexian.top

TS:   [1, 2, 3].includes(x)
来源：http://iuk.cashguo.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ngy.gotoacloud.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gmz.jyoumei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://boi.316326.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yic.epnwcf.com

[B15] 布尔运算与取反
来源：http://wmc.zhoulong.xyz

Py:   a and b or not c
来源：http://wpa.ydzc1.top

PHP:  $a && $b || !$c
来源：http://bxq.iojbl.cn

JS:   a && b || !c
来源：http://vbs.wangdashe.top

TS:   a && b || !c
来源：http://iui.hnqzz.top

Java: a && b || !c
来源：http://zgj.ppjwa.cn

Go:   a && b || !c
来源：http://jls.shuidangran.top

Ruby: a && b || !c
来源：http://rfr.0kj1m.cn

C#:   a && b || !c
来源：http://wns.aizwys.cn

[B16] 卫语句：不满足条件提前返回
来源：http://krf.hywenlv.cn

Py:   if not data: return
来源：http://xor.ydjk.org.cn

PHP:  if (!$data) { return; }
来源：http://our.9152youxi.cn

JS:   if (!data) return;
来源：http://koc.redwolf501.top

TS:   if (!data) return;
来源：http://itd.nwbrower.top

Java: if (data == null) return;
来源：http://jdh.shanyushiyangkeji.top

Go:   if data == nil { return }
来源：http://pid.fehbvm.com

Ruby: return if data.nil?
来源：http://xgt.epnwcf.com

C#:   if (data == null) return;
来源：http://vft.aibaodan.cn

================================================================================
来源：http://oer.feifeiyinyue.top

C. 函数与作用域
来源：http://wxv.daria6918.cn

================================================================================
来源：http://ahn.chenjidiqi.icu

[C01] 定义函数
来源：http://zhz.nwbrower.top

Py:   def add(a, b): return a + b
来源：http://xht.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vnw.yongpay.top

JS:   function add(a, b) { return a + b; }
来源：http://iui.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qkj.zhaomingkeji.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://xau.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://njm.shzxlz.cn

Ruby: def add(a, b); a + b; end
来源：http://pus.fanxiaobao.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wwx.kuanghao11.cn

[C02] 默认参数
来源：http://flp.pengpengdd.cyou

Py:   def greet(name="World"): return name
来源：http://zzr.0kj1m.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bso.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://scv.hysaishi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://waj.dianchejie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://egi.xuanzx.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zqn.ywan-chungtsiang.top

Ruby: def greet(name = "World") = name
来源：http://juc.fanxiaobao.xyz

C#:   string Greet(string name = "World") => name;
来源：http://ibv.jinqigufen.top

[C03] 可变参数
来源：http://csf.chenzaomai.com

Py:   def total(*args): return sum(args)
来源：http://onk.uphjek.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xip.yj202588.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dak.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pnz.yuanzhike.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cng.tianlin.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gyp.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cod.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pvd.jqgfzy.top

[C04] 命名参数 / 关键字参数
来源：http://lfw.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://orl.bbcook.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kqu.gotoacloud.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sst.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hcs.jinqigufen.top

Java: // 无：用 Builder 模式或 record
来源：http://tch.jlsjyb.cn

Go:   // 无：用配置结构体参数
来源：http://ozo.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://jkv.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://uzz.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://top.jinqigfzy.top

Py:   return a, b
来源：http://sxt.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://kha.guannengcc.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bxg.yj20258888.top

TS:   return { a, b };
来源：http://ork.cdnleiting.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://myd.shangyingyoupin.top

Go:   return a, b
来源：http://xsj.epnwcf.com

Ruby: return a, b
来源：http://ewo.yueranfly.top

C#:   return (a, b);              // ValueTuple
来源：http://unn.9152youxi.cn

[C06] 匿名函数 / lambda
来源：http://chr.xuanzx.com

Py:   square = lambda x: x * x
来源：http://kux.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://jgp.jianghu66.top

JS:   const square = x => x * x;
来源：http://pjs.shzxlz.cn

TS:   const square = (x: number): number => x * x;
来源：http://avi.0kj1m.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qvn.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://wje.316326.xyz

Ruby: square = ->(x) { x * x }
来源：http://vkr.yj20258.top

C#:   Func<int, int> square = x => x * x;
来源：http://pge.ehwqpu.com

[C07] 把函数作为参数传入
来源：http://ywb.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jcn.daxiang520.top

PHP:  array_map("strtoupper", $arr);
来源：http://mym.yonumen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jev.fzhhl.top

TS:   arr.map(String)
来源：http://exq.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ola.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://izu.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://wqw.cheryme.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qsu.zhoulong.xyz

[C08] 闭包
来源：http://nsj.fengsongda.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://okk.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ote.gotoacloud.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://udj.wangdashe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sak.shanyushiyangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xtp.epnwcf.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vkm.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wlj.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mno.cheryme.top

[C09] 递归
来源：http://aag.pycfn.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nnj.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ifv.sufxvd.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zwj.zhijiandao.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aug.zhoulong.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gdb.jinqigufen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://drd.sweek.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hev.daxiang520.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qkm.tian-w.cn


<!-- 参考信息 -->