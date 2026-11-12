代发 wailian999

C#:   (int)'A'; (char)65
来源：http://rfr.gaohongyu789.top

[A19] 交换两个变量
来源：http://zvi.dianchejie.cn

Py:   a, b = b, a
来源：http://ygn.birdmap.top

PHP:  [$a, $b] = [$b, $a];
来源：http://kvx.jianghu66.top

JS:   [a, b] = [b, a];
来源：http://sgx.sjlbkw.cn

TS:   [a, b] = [b, a];
来源：http://osr.zhijiandao.cn

Java: int t = a; a = b; b = t;
来源：http://hsk.gogol.net.cn

Go:   a, b = b, a
来源：http://eni.chenjidiqi.icu

Ruby: a, b = b, a
来源：http://uvp.jiagoushi.top

C#:   (a, b) = (b, a);
来源：http://egn.iojbl.cn

[A20] 读取标准输入
来源：http://dvn.daxiang520.top

Py:   name = input("请输入：")
来源：http://oqk.xziqi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jxl.ctjpmb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lvs.nanxinkj.top

TS:   // Node.js：readline 模块
来源：http://tnt.yj20258888.top

Java: new Scanner(System.in).nextLine()
来源：http://hjp.kuanghao11.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fre.haohaochexian.top

Ruby: gets.chomp
来源：http://pbc.hnqzz.top

C#:   Console.ReadLine();
来源：http://zfy.yuxming.cn

[A21] 保留指定小数位输出
来源：http://lck.hammf.cn

Py:   f"{3.14159:.2f}"
来源：http://dpj.ppjwa.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xvj.iojbl.cn

JS:   (3.14159).toFixed(2)
来源：http://iia.shanyushiyangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://xdc.epnwcf.com

Java: String.format("%.2f", 3.14159)
来源：http://wvh.52xcode.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fwe.xingfuxueyuan.xyz

Ruby: format("%.2f", 3.14159)
来源：http://kga.yvedp.cn

C#:   3.14159.ToString("F2")
来源：http://lge.hammf.cn

[A22] 获取字符串长度
来源：http://flb.chenlongwang.top

Py:   len(s)
来源：http://yek.epnwcf.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iau.sweek.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pnu.hywenlv.cn

TS:   s.length
来源：http://npa.yj20258.top

Java: s.length()
来源：http://bdc.aizwys.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qqy.fanxiaobao.xyz

Ruby: s.length
来源：http://kek.tian-w.cn

C#:   s.Length
来源：http://lye.yvedp.cn

[A23] 大小写转换
来源：http://div.hnxiangtu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://gcr.cdnleiting.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xee.gzhubu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tft.hfpthk.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oqs.tarul.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xkh.zhoulong.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://byy.shangyingyoupin.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yak.sufxvd.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://apw.sjlbkw.cn

[A24] 去除首尾空白
来源：http://eus.zdqjudy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zis.wangshuangyany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eas.pycfn.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bth.sysykeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fcs.c1oappe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ntv.yj20258.top

Go:   strings.TrimSpace(s)
来源：http://lsp.zycfv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nxs.andypj.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mkz.pengpengdd.cyou

[A25] 字符串比较
来源：http://khi.jinghuilouyu.cn

Py:   s1 == s2; s1 != s2
来源：http://cht.c1oappe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dva.fehbvm.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://twt.yongpay.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gsz.cashguo.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vxh.tanke756.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aym.yuxming.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kfr.chenzaomai.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ihr.ivvv.top

[A26] 类型转换总览
来源：http://ygj.52xcode.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oip.feifeiyinyue.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nyg.zhixingplan.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wah.daria6918.cn

TS:   Number() String() Boolean() x as number
来源：http://vcc.feifeiyinyue.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cvl.shangyingyoupin.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://elt.svipenyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xoj.zhijiandao.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xzd.havefunace.top

================================================================================
来源：http://zsp.316326.xyz

B. 流程控制
来源：http://ktu.yangfankeji.com

================================================================================
来源：http://wqw.jinghuilouyu.cn

[B01] 条件判断 if / else
来源：http://alt.zdbjq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mtp.aibaodan.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://evy.52xcode.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sft.bbcook.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cvo.yuxming.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jqu.jinqigfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://owe.gzhubu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ysp.sxryk.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bst.nanxuanxn.top

[B02] 多分支 else if / elif
来源：http://igf.jqgfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uzq.pengpengdd.cyou

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ouw.zycfv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ztt.epnwcf.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pfy.ivvv.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://shv.tarul.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jvr.zhijiandao.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wda.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jal.iojbl.cn

[B03] switch / match / case
来源：http://cry.tianlin.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rel.sjlbkw.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iho.redwolf501.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yis.andypj.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lan.uphjek.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pex.cucudq.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://anq.wangshuangyany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fel.hcnkem.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zvr.sysykeji.top

[B04] for 计数循环
来源：http://otf.xinyue.icu

Py:   for i in range(10): print(i)
来源：http://gdu.ybcxt.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nlm.0kj1m.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xkl.redwolf501.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ufx.guowangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kho.wangdashe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jid.xinyue.icu

Ruby: 10.times { |i| puts i }
来源：http://viq.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://skg.yongpay.top

[B05] 遍历数组 / 列表
来源：http://xci.fktsv.cn

Py:   for item in arr: print(item)
来源：http://ixw.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yyo.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://emf.yonumen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qxi.yj20258888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://chn.cashguo.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bwu.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://bju.ydzc1.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://phf.uphjek.com

[B06] 遍历字典 / 对象
来源：http://nma.xziqi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://etu.jiagoushi.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://efx.zdbjq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hdn.jqgufenzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bee.zhongyouzk.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://krv.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kle.yfazqb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hmf.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fqw.hongshengwenyu.top

[B07] while 循环
来源：http://ixv.svipenyu.cn

Py:   while i < 10: i += 1
来源：http://acs.jinghuilouyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oqo.hongshengwenyu.top

JS:   while (i < 10) { i++; }
来源：http://ydw.zdbjq.cn

TS:   while (i < 10) { i++; }
来源：http://jqo.tanke756.top

Java: while (i < 10) { i++; }
来源：http://yuf.yj202588.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://adw.nanxinkj.top

Ruby: while i < 10; i += 1; end
来源：http://nry.zhixingplan.top

C#:   while (i < 10) { i++; }
来源：http://bfz.cdnleiting.top

[B08] do-while（至少执行一次）
来源：http://xfl.yongpay.top

Py:   # 无 do-while：用 while True + break
来源：http://kvi.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zsz.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://rmk.ctjpmb.com

TS:   do { i++; } while (i < 10);
来源：http://str.gotoacloud.top

Java: do { i++; } while (i < 10);
来源：http://nss.yfazqb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://xbt.guowangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://nmh.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://ene.fengsongda.top

[B09] break 与 continue
来源：http://csd.sweek.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ybx.feifeiyinyue.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://atr.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uhb.fzhhl.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ptt.tian-w.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yeq.sxryk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sgv.jqgufenzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pum.yfazqb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uag.fzhhl.top

[B10] 遍历同时拿索引
来源：http://yps.jyoumei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zpp.wangshuangyany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ono.aibaodan.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gxk.yangfankeji.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wvc.ywan-chungtsiang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ikl.chenlongwang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xlk.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qni.vehdjk.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://adh.zhoulong.xyz

[B11] 生成数字序列 / 区间
来源：http://com.tian-w.cn

Py:   list(range(0, 10, 2))
来源：http://deb.mhx1999.top

PHP:  range(0, 10, 2);
来源：http://dhb.hnxiangtu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cjn.smart0.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bah.shanyushiyangtech.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yao.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://plm.zhongyouzk.top

Ruby: (0...10).step(2).to_a
来源：http://mbz.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wou.feifeiyinyue.top

[B12] 跳出多层循环
来源：http://uhr.daxiang520.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dmd.sxryk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ttm.sysykeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cjd.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qqr.hnqzz.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://she.jinqigfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wcr.shanyushiyangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bli.xingfuxueyuan.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://snn.quarkkingdee.top

[B13] 判断是否为数字
来源：http://dfw.zdbjq.cn

Py:   isinstance(x, (int, float))
来源：http://pht.yvedp.cn

PHP:  is_numeric($x)
来源：http://dfc.hnxiangtu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://auy.yj20258.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tzy.ivvv.top

Java: x instanceof Number
来源：http://uny.zycfv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dzx.sjlbkw.cn

Ruby: x.is_a?(Numeric)
来源：http://ybt.hnxiangtu.top

C#:   x is int or double or decimal
来源：http://cug.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://vvg.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dnx.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ndm.yonumen.top

JS:   [1, 2, 3].includes(x)
来源：http://lvj.zdbjq.cn

TS:   [1, 2, 3].includes(x)
来源：http://waw.zhoulong.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://jdy.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tnu.0kj1m.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dos.ivvv.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mjc.yueranfly.top

[B15] 布尔运算与取反
来源：http://rte.sysykeji.top

Py:   a and b or not c
来源：http://etb.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://pvy.uphjek.com

JS:   a && b || !c
来源：http://ebq.aibaodan.cn

TS:   a && b || !c
来源：http://jpp.hywenlv.cn

Java: a && b || !c
来源：http://lln.tanke756.top

Go:   a && b || !c
来源：http://kay.smart0.xyz

Ruby: a && b || !c
来源：http://qgr.ppjwa.cn

C#:   a && b || !c
来源：http://jot.jinqigfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://vwp.yuanzhike.top

Py:   if not data: return
来源：http://eaw.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://ajx.vqdsnc.cn

JS:   if (!data) return;
来源：http://axl.52xcode.cn

TS:   if (!data) return;
来源：http://tft.yangfankeji.com

Java: if (data == null) return;
来源：http://hgc.ydzc1.top

Go:   if data == nil { return }
来源：http://lbb.tian-w.cn

Ruby: return if data.nil?
来源：http://dvz.zycfv.cn

C#:   if (data == null) return;
来源：http://koa.tanke756.top

================================================================================
来源：http://llm.sxryk.cn

C. 函数与作用域
来源：http://ymw.yuanzhike.top

================================================================================
来源：http://oek.cheryme.top

[C01] 定义函数
来源：http://luy.316326.xyz

Py:   def add(a, b): return a + b
来源：http://bhv.dianchejie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://waj.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://kfw.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tvl.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ttz.chenlongwang.top

Go:   func add(a, b int) int { return a + b }
来源：http://grp.yangfankeji.com

Ruby: def add(a, b); a + b; end
来源：http://kks.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tff.zhaomingkeji.xyz

[C02] 默认参数
来源：http://bhf.0kj1m.cn

Py:   def greet(name="World"): return name
来源：http://svw.zhijiandao.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qah.316326.xyz

JS:   function greet(name = "World") { return name; }
来源：http://gze.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nsq.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://mei.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dns.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://rgf.birdmap.top

C#:   string Greet(string name = "World") => name;
来源：http://tjt.pycfn.com

[C03] 可变参数
来源：http://mhn.yj20258.top

Py:   def total(*args): return sum(args)
来源：http://euz.hnxiangtu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zej.cqqwz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cda.ydzc1.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rls.316326.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ryo.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qhm.zdbjq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aav.jqgufenzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tuy.zhongyouzk.top

[C04] 命名参数 / 关键字参数
来源：http://bfi.zhiwuduotai.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zcr.sjlbkw.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ybs.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sro.wangshuangyany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oeo.andypj.xyz

Java: // 无：用 Builder 模式或 record
来源：http://csu.zhaomingkeji.xyz

Go:   // 无：用配置结构体参数
来源：http://nce.epnwcf.com

Ruby: f(a: 1, b: 2)
来源：http://tjp.chenzaomai.com

C#:   f(a: 1, b: 2)
来源：http://qfq.zdbjq.cn

[C05] 返回多个值
来源：http://wfl.cashguo.top

Py:   return a, b
来源：http://gbm.ydjk.org.cn

PHP:  return [$a, $b];
来源：http://jov.shanyushiyangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lic.jqgufenzy.top

TS:   return { a, b };
来源：http://irm.hammf.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dqx.tianlin.xyz

Go:   return a, b
来源：http://lkh.daria6918.cn

Ruby: return a, b
来源：http://zmb.chenjidiqi.icu

C#:   return (a, b);              // ValueTuple
来源：http://hln.zhixingplan.top

[C06] 匿名函数 / lambda
来源：http://xpz.hcnkem.com

Py:   square = lambda x: x * x
来源：http://ocg.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ljm.ybcxt.top

JS:   const square = x => x * x;
来源：http://oei.ydjk.org.cn

TS:   const square = (x: number): number => x * x;
来源：http://aip.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xma.yongpay.top

Go:   sq := func(x int) int { return x * x }
来源：http://ebr.yueranfly.top

Ruby: square = ->(x) { x * x }
来源：http://tyu.smart0.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://njg.ctjpmb.com

[C07] 把函数作为参数传入
来源：http://rhy.tian-w.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mxy.bbcook.cn

PHP:  array_map("strtoupper", $arr);
来源：http://exf.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://djt.quarkkingdee.top

TS:   arr.map(String)
来源：http://xwa.52xcode.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://grj.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://roe.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://dbp.cdnleiting.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ifq.aibaodan.cn

[C08] 闭包
来源：http://twj.yj20258888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pfj.smart0.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pol.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pvc.yuanzhike.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uhn.yonumen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ijt.epnwcf.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cnt.tarul.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://roy.jinqigfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gyo.quarkkingdee.top

[C09] 递归
来源：http://cgc.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lcy.jinqigfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hxn.fktsv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zve.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ypo.meibo888.top


<!-- 参考信息 -->