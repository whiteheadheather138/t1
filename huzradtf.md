代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zwu.feifeiyinyue.top

Java: (int) 'A'; (char) 65
来源：http://zpn.nanxinkj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qox.yongpay.top

Ruby: "A".ord; 65.chr
来源：http://bel.zhijiandao.cn

C#:   (int)'A'; (char)65
来源：http://ugf.smart0.xyz

[A19] 交换两个变量
来源：http://hat.jyoumei.cn

Py:   a, b = b, a
来源：http://jvy.havefunace.top

PHP:  [$a, $b] = [$b, $a];
来源：http://vud.tian-w.cn

JS:   [a, b] = [b, a];
来源：http://lrn.hfpthk.cn

TS:   [a, b] = [b, a];
来源：http://cyx.sufxvd.cn

Java: int t = a; a = b; b = t;
来源：http://cjb.sweek.top

Go:   a, b = b, a
来源：http://ojm.nanxuanxn.top

Ruby: a, b = b, a
来源：http://mxs.yangfankeji.com

C#:   (a, b) = (b, a);
来源：http://ktg.zhiwuduotai.top

[A20] 读取标准输入
来源：http://shd.hnqzz.top

Py:   name = input("请输入：")
来源：http://adg.gzhubu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jcy.guowangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eot.yangfankeji.com

TS:   // Node.js：readline 模块
来源：http://ebm.uphjek.com

Java: new Scanner(System.in).nextLine()
来源：http://uiu.cucudq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vjz.zhoulong.xyz

Ruby: gets.chomp
来源：http://grl.birdmap.top

C#:   Console.ReadLine();
来源：http://mwc.yj20258888.top

[A21] 保留指定小数位输出
来源：http://ahu.tarul.cn

Py:   f"{3.14159:.2f}"
来源：http://xpf.bjfxy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kit.svipenyu.cn

JS:   (3.14159).toFixed(2)
来源：http://sxm.svipenyu.cn

TS:   (3.14159).toFixed(2)
来源：http://lms.fzhhl.top

Java: String.format("%.2f", 3.14159)
来源：http://sbz.gotoacloud.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lhl.52xcode.cn

Ruby: format("%.2f", 3.14159)
来源：http://dsa.xuanzx.com

C#:   3.14159.ToString("F2")
来源：http://vkc.gogol.net.cn

[A22] 获取字符串长度
来源：http://isn.haohaochexian.top

Py:   len(s)
来源：http://isw.shanyushiyangtech.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jbw.52xcode.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://odf.hesvh.cn

TS:   s.length
来源：http://xdi.hfpthk.cn

Java: s.length()
来源：http://aon.aibaodan.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jqn.sxryk.cn

Ruby: s.length
来源：http://wvi.tian-w.cn

C#:   s.Length
来源：http://sfu.yj202588.top

[A23] 大小写转换
来源：http://kqp.yangfankeji.com

Py:   s.upper(); s.lower(); s.title()
来源：http://ksl.yj20258888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ebp.daxiang520.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uyb.jinyuanbaomall.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sbr.0kj1m.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qsf.zhaomingkeji.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vsc.yonumen.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rcs.uphjek.com

C#:   s.ToUpper(); s.ToLower()
来源：http://wqk.yj20258.top

[A24] 去除首尾空白
来源：http://ssy.hywenlv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yuy.feifeiyinyue.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bqy.jiagoushi.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://reg.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://swk.shanyushiyangtech.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vfn.ctjpmb.com

Go:   strings.TrimSpace(s)
来源：http://kfu.snrcjt.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yoz.ywan-chungtsiang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fhw.jinqigufen.top

[A25] 字符串比较
来源：http://lxq.cashguo.top

Py:   s1 == s2; s1 != s2
来源：http://hbr.ivvv.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wqs.jinqigfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ucl.epnwcf.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xsh.hnxiangtu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xkz.fengsongda.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qjm.316326.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://npm.sweek.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yzn.zhongyouzk.top

[A26] 类型转换总览
来源：http://yef.cashguo.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jmn.52xcode.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://npw.316326.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jhw.zdbjq.cn

TS:   Number() String() Boolean() x as number
来源：http://ged.yfazqb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vor.vqdsnc.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ohs.ydjk.org.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jqr.daria6918.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://erp.cucudq.cn

================================================================================
来源：http://zck.ydzc1.top

B. 流程控制
来源：http://ksa.yuanzhike.top

================================================================================
来源：http://vhj.zhixingplan.top

[B01] 条件判断 if / else
来源：http://idg.quarkkingdee.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wtt.zhengqikj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dza.ydjk.org.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://shv.bbcook.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pyl.c1oappe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://spw.yvedp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bni.mhx1999.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jci.hesvh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lef.9152youxi.cn

[B02] 多分支 else if / elif
来源：http://krc.vqdsnc.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aot.ybcxt.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uxi.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ucu.haohaochexian.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uma.aizwys.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uyz.birdmap.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nhq.vehdjk.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cjc.yongpay.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sfz.daria6918.cn

[B03] switch / match / case
来源：http://tix.52xcode.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mty.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sog.guannengcc.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vuh.xinyue.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gph.tanke756.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vdu.yj20258.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pws.vqdsnc.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zob.guannengcc.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aan.jinyuanbaomall.cn

[B04] for 计数循环
来源：http://rlk.ywan-chungtsiang.top

Py:   for i in range(10): print(i)
来源：http://ovw.feifeiyinyue.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gdr.redwolf501.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hpk.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jwe.kuanghao11.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jlg.chenzaomai.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dfj.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://wks.zhoulong.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jrc.xuanzx.com

[B05] 遍历数组 / 列表
来源：http://azo.hysaishi.cn

Py:   for item in arr: print(item)
来源：http://zvk.dianchejie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vxz.jiagoushi.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zib.hesvh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://smi.haohaochexian.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://anp.sxryk.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uay.fehbvm.com

Ruby: arr.each { |item| puts item }
来源：http://dhf.guowangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jso.daria6918.cn

[B06] 遍历字典 / 对象
来源：http://neh.daria6918.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wkx.gogol.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fmk.zhoulong.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sye.feifeiyinyue.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xyw.sjlbkw.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rrl.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://peg.fengsongda.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ttu.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rmq.jinghuilouyu.cn

[B07] while 循环
来源：http://blt.xuetiantiany.cn

Py:   while i < 10: i += 1
来源：http://oea.sysykeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://uzr.ppjwa.cn

JS:   while (i < 10) { i++; }
来源：http://ssz.xylfe.cn

TS:   while (i < 10) { i++; }
来源：http://fva.shanyushiyangkeji.top

Java: while (i < 10) { i++; }
来源：http://otm.bjfxy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zhu.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://nic.fanxiaobao.xyz

C#:   while (i < 10) { i++; }
来源：http://awf.shanyushiyangkeji.top

[B08] do-while（至少执行一次）
来源：http://sla.wangshuangyany.cn

Py:   # 无 do-while：用 while True + break
来源：http://aix.cashguo.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wei.hnqzz.top

JS:   do { i++; } while (i < 10);
来源：http://lmr.chenjidiqi.icu

TS:   do { i++; } while (i < 10);
来源：http://qij.vehdjk.com

Java: do { i++; } while (i < 10);
来源：http://niq.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://bkh.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://pxn.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://yje.gaohongyu789.top

[B09] break 与 continue
来源：http://xgh.yuanzhike.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ycn.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://umu.zhoulong.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xbt.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://odq.bbcook.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cat.jqgufenzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://imr.fktsv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tyu.ctjpmb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vok.hysaishi.cn

[B10] 遍历同时拿索引
来源：http://hdl.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://isg.pengpengdd.cyou

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wbz.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sjv.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zmh.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mxq.guannengcc.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qmy.ctjpmb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hzd.zhijiandao.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rnf.yueranfly.top

[B11] 生成数字序列 / 区间
来源：http://coo.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://lvf.hesvh.cn

PHP:  range(0, 10, 2);
来源：http://wyj.jqgufenzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gjw.chenzaomai.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nne.shanyushiyangtech.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fff.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://atz.guannengcc.top

Ruby: (0...10).step(2).to_a
来源：http://lyk.hammf.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wqv.yuxming.cn

[B12] 跳出多层循环
来源：http://vsj.zhijiandao.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pyb.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://cbo.kuanghao11.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dmv.bbcook.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bih.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nxt.sysykeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lig.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://alq.ppjwa.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eri.zhixingplan.top

[B13] 判断是否为数字
来源：http://jne.hnqzz.top

Py:   isinstance(x, (int, float))
来源：http://rih.jinqigufen.top

PHP:  is_numeric($x)
来源：http://noj.kuanghao11.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sjr.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://orx.mhx1999.top

Java: x instanceof Number
来源：http://fma.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zcm.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://fqg.fktsv.cn

C#:   x is int or double or decimal
来源：http://ojy.hywenlv.cn

[B14] 判断值是否在集合内
来源：http://dse.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ylo.daxiang520.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dil.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://cid.nanxuanxn.top

TS:   [1, 2, 3].includes(x)
来源：http://myz.vqdsnc.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kxa.jqgufenzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ufa.pycfn.com

Ruby: [1, 2, 3].include?(x)
来源：http://hrf.ivvv.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://upa.shzxlz.cn

[B15] 布尔运算与取反
来源：http://zeh.bjfxy.top

Py:   a and b or not c
来源：http://pha.smart0.xyz

PHP:  $a && $b || !$c
来源：http://yec.zhaomingkeji.xyz

JS:   a && b || !c
来源：http://dal.hammf.cn

TS:   a && b || !c
来源：http://kyp.tanke756.top

Java: a && b || !c
来源：http://ant.hywenlv.cn

Go:   a && b || !c
来源：http://lne.daxiang520.top

Ruby: a && b || !c
来源：http://czo.zhixingplan.top

C#:   a && b || !c
来源：http://wdi.pengpengdd.cyou

[B16] 卫语句：不满足条件提前返回
来源：http://nxj.yvedp.cn

Py:   if not data: return
来源：http://isr.ydjk.org.cn

PHP:  if (!$data) { return; }
来源：http://zwi.zhoulong.xyz

JS:   if (!data) return;
来源：http://axx.cqqwz.cn

TS:   if (!data) return;
来源：http://ewr.jqgfzy.top

Java: if (data == null) return;
来源：http://dhe.cashguo.top

Go:   if data == nil { return }
来源：http://uzc.fktsv.cn

Ruby: return if data.nil?
来源：http://xqq.yonumen.top

C#:   if (data == null) return;
来源：http://khm.gzhubu.top

================================================================================
来源：http://quv.chenzaomai.com

C. 函数与作用域
来源：http://txl.cucudq.cn

================================================================================
来源：http://hwk.jinghuilouyu.cn

[C01] 定义函数
来源：http://yvi.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://vbi.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nol.epnwcf.com

JS:   function add(a, b) { return a + b; }
来源：http://col.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zwy.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ekm.sufxvd.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ljr.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://crd.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fcf.yanxiufei.cn

[C02] 默认参数
来源：http://zxb.hfpthk.cn

Py:   def greet(name="World"): return name
来源：http://kno.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://evw.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://isp.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zjk.hnqzz.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cre.hywenlv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wtg.zycfv.cn

Ruby: def greet(name = "World") = name
来源：http://kmp.vqdsnc.cn

C#:   string Greet(string name = "World") => name;
来源：http://lyv.epnwcf.com

[C03] 可变参数
来源：http://aic.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://dyh.xingfuxueyuan.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kvg.xylfe.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tbm.hcnkem.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zpz.cucudq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jhn.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wfn.yfazqb.com

Ruby: def total(*nums); nums.sum; end
来源：http://xbs.jinghuilouyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mzk.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://xip.xinyue.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ngq.redwolf501.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pmp.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://glt.jinqigfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://twq.kuanghao11.cn

Java: // 无：用 Builder 模式或 record
来源：http://ckd.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://mcu.hysaishi.cn

Ruby: f(a: 1, b: 2)
来源：http://nvg.jqgufenzy.top

C#:   f(a: 1, b: 2)
来源：http://xyn.jinyuanbaomall.cn

[C05] 返回多个值
来源：http://fdj.jinqigfzy.top

Py:   return a, b
来源：http://yim.chenzaomai.com

PHP:  return [$a, $b];
来源：http://emw.zhongyouzk.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ggp.gaohongyu789.top

TS:   return { a, b };
来源：http://kkq.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jlp.hammf.cn

Go:   return a, b
来源：http://nfm.redwolf501.top

Ruby: return a, b
来源：http://eph.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://owp.pycfn.com

[C06] 匿名函数 / lambda
来源：http://umc.guannengcc.top

Py:   square = lambda x: x * x
来源：http://sjf.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rtb.kuanghao11.cn

JS:   const square = x => x * x;
来源：http://jwu.hcnkem.com

TS:   const square = (x: number): number => x * x;
来源：http://tch.hongshengwenyu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mrh.daria6918.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hqc.ybcxt.top

Ruby: square = ->(x) { x * x }
来源：http://bmr.yueranfly.top

C#:   Func<int, int> square = x => x * x;
来源：http://tim.hammf.cn

[C07] 把函数作为参数传入
来源：http://bsg.xinyue.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qjt.xziqi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ksd.fengsongda.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ngu.yj20258888.top

TS:   arr.map(String)
来源：http://ram.316326.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pmt.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xfz.wangdashe.top

Ruby: arr.map(&:upcase)
来源：http://ank.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jxs.hnxiangtu.top

[C08] 闭包
来源：http://kbm.zdqjudy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fsj.cqqwz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uar.hywenlv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lji.hnxiangtu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mhu.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wgi.yueranfly.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mvj.nwbrower.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eln.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://spu.sxryk.cn

[C09] 递归
来源：http://ovl.yuanzhike.top


<!-- 参考信息 -->