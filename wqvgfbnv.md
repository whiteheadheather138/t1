代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nru.iojbl.cn

Java: (int) 'A'; (char) 65
来源：http://bjr.shzxlz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uii.yuanzhike.top

Ruby: "A".ord; 65.chr
来源：http://oxo.feifeiyinyue.top

C#:   (int)'A'; (char)65
来源：http://hye.jinyuanbaomall.cn

[A19] 交换两个变量
来源：http://rva.ydzc1.top

Py:   a, b = b, a
来源：http://hoq.guannengcc.top

PHP:  [$a, $b] = [$b, $a];
来源：http://rsc.havefunace.top

JS:   [a, b] = [b, a];
来源：http://ecf.0kj1m.cn

TS:   [a, b] = [b, a];
来源：http://fvv.mhx1999.top

Java: int t = a; a = b; b = t;
来源：http://wlz.cdnleiting.top

Go:   a, b = b, a
来源：http://xyw.ywan-chungtsiang.top

Ruby: a, b = b, a
来源：http://mym.quarkkingdee.top

C#:   (a, b) = (b, a);
来源：http://vjc.ydjk.org.cn

[A20] 读取标准输入
来源：http://opi.52xcode.cn

Py:   name = input("请输入：")
来源：http://yfw.9152youxi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gsf.xylfe.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yrh.ybcxt.top

TS:   // Node.js：readline 模块
来源：http://ssp.chenlongwang.top

Java: new Scanner(System.in).nextLine()
来源：http://tsf.9152youxi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jpo.hfpthk.cn

Ruby: gets.chomp
来源：http://cju.bjfxy.top

C#:   Console.ReadLine();
来源：http://orl.ehwqpu.com

[A21] 保留指定小数位输出
来源：http://gyv.quarkkingdee.top

Py:   f"{3.14159:.2f}"
来源：http://faj.zhijiandao.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nhm.shuidangran.top

JS:   (3.14159).toFixed(2)
来源：http://bui.fehbvm.com

TS:   (3.14159).toFixed(2)
来源：http://kpj.haohaochexian.top

Java: String.format("%.2f", 3.14159)
来源：http://sxa.tanke756.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zaa.ywan-chungtsiang.top

Ruby: format("%.2f", 3.14159)
来源：http://oqt.vqdsnc.cn

C#:   3.14159.ToString("F2")
来源：http://bwq.zhoulong.xyz

[A22] 获取字符串长度
来源：http://hut.fengsongda.top

Py:   len(s)
来源：http://pzx.hnqzz.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mgz.xuetiantiany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dbr.yj202588.top

TS:   s.length
来源：http://tlq.gaohongyu789.top

Java: s.length()
来源：http://ent.fehbvm.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://isv.hesvh.cn

Ruby: s.length
来源：http://bkn.sufxvd.cn

C#:   s.Length
来源：http://lyr.yfazqb.com

[A23] 大小写转换
来源：http://ezt.fktsv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uac.hongshengwenyu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xgj.andypj.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ajl.zdbjq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hfd.jinqigufen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sqz.redwolf501.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://odh.yfazqb.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nxa.shanyushiyangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kvz.nanxinkj.top

[A24] 去除首尾空白
来源：http://oaw.gaohongyu789.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nvi.zhijiandao.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nnc.gogol.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zqd.ehwqpu.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nva.nanxuanxn.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vyf.tarul.cn

Go:   strings.TrimSpace(s)
来源：http://qtm.sweek.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qra.guannengcc.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://htj.fanxiaobao.xyz

[A25] 字符串比较
来源：http://cpz.vehdjk.com

Py:   s1 == s2; s1 != s2
来源：http://ffb.zhixingplan.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://egc.svipenyu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xkq.cashguo.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oyx.cqqwz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cht.shangyingyoupin.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uea.ivvv.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kfz.ywan-chungtsiang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nzp.wangshuangyany.cn

[A26] 类型转换总览
来源：http://png.yj20258.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cjx.shanyushiyangtech.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fuz.c1oappe.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zcx.wangshuangyany.cn

TS:   Number() String() Boolean() x as number
来源：http://bxj.aibaodan.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xbd.hnqzz.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ffh.jiagoushi.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qxc.52xcode.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vhe.jqgfzy.top

================================================================================
来源：http://jxg.snrcjt.cn

B. 流程控制
来源：http://vlb.nwbrower.top

================================================================================
来源：http://mpm.vehdjk.com

[B01] 条件判断 if / else
来源：http://nff.316326.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://jks.zhongyouzk.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yui.zdqjudy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qzz.sjlbkw.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qlf.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cfc.yvedp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gyk.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qkm.cucudq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xhz.daria6918.cn

[B02] 多分支 else if / elif
来源：http://pod.kuanghao11.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://djb.cashguo.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pbe.sxryk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wra.tarul.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ygo.gzhubu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sxw.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xoz.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dhs.sufxvd.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jzy.kuanghao11.cn

[B03] switch / match / case
来源：http://sip.9152youxi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vcj.cucudq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tsv.chenjidiqi.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ctr.xuanzx.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kiw.cdnleiting.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dzk.hywenlv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eyv.gzhubu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ibo.aibaodan.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zbt.ydzc1.top

[B04] for 计数循环
来源：http://uoo.zhiwuduotai.top

Py:   for i in range(10): print(i)
来源：http://klx.gotoacloud.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://itc.fzhhl.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tks.daxiang520.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rhh.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cco.pengpengdd.cyou

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yis.daria6918.cn

Ruby: 10.times { |i| puts i }
来源：http://ewh.shuidangran.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dwv.xuetiantiany.cn

[B05] 遍历数组 / 列表
来源：http://swi.hfpthk.cn

Py:   for item in arr: print(item)
来源：http://bmt.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cmq.yueranfly.top

JS:   for (const item of arr) { console.log(item); }
来源：http://iph.hesvh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ark.zhoulong.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://qqk.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kdj.fzhhl.top

Ruby: arr.each { |item| puts item }
来源：http://hwb.jianghu66.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vdw.jinyuanbaomall.cn

[B06] 遍历字典 / 对象
来源：http://pxm.zhaomingkeji.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://ehf.gogol.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wab.aizwys.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ztm.sysykeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ofl.ppjwa.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nlc.redwolf501.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://beu.ehwqpu.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ruw.jianghu66.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wqz.sxryk.cn

[B07] while 循环
来源：http://knc.chenzaomai.com

Py:   while i < 10: i += 1
来源：http://iwf.sxryk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vgo.dianchejie.cn

JS:   while (i < 10) { i++; }
来源：http://kiw.jinqigufen.top

TS:   while (i < 10) { i++; }
来源：http://mpt.fengsongda.top

Java: while (i < 10) { i++; }
来源：http://xma.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zwq.aizwys.cn

Ruby: while i < 10; i += 1; end
来源：http://yth.pengpengdd.cyou

C#:   while (i < 10) { i++; }
来源：http://jmr.nwbrower.top

[B08] do-while（至少执行一次）
来源：http://lok.tianlin.xyz

Py:   # 无 do-while：用 while True + break
来源：http://eyr.tianlin.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://wlb.ydzc1.top

JS:   do { i++; } while (i < 10);
来源：http://hhy.pengpengdd.cyou

TS:   do { i++; } while (i < 10);
来源：http://uzr.hysaishi.cn

Java: do { i++; } while (i < 10);
来源：http://bee.zhijiandao.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xio.yvedp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zdb.sysykeji.top

C#:   do { i++; } while (i < 10);
来源：http://hic.tian-w.cn

[B09] break 与 continue
来源：http://ezd.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://enu.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xij.dianchejie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kak.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tbl.pengpengdd.cyou

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hya.mhx1999.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cpy.birdmap.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zua.9152youxi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lgy.bbcook.cn

[B10] 遍历同时拿索引
来源：http://ipr.yfazqb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aqx.zhaomingkeji.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mvb.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bjk.gotoacloud.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://unb.redwolf501.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://trr.hywenlv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bjo.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ekv.zycfv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gsu.quarkkingdee.top

[B11] 生成数字序列 / 区间
来源：http://son.yangfankeji.com

Py:   list(range(0, 10, 2))
来源：http://pww.hammf.cn

PHP:  range(0, 10, 2);
来源：http://ejo.hfpthk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gei.yfazqb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aqv.yonumen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cxp.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vab.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://jmi.meibo888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fik.gaohongyu789.top

[B12] 跳出多层循环
来源：http://mjv.shanyushiyangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://def.jqgufenzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pcn.bbcook.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wrz.uphjek.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rvq.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yja.hfpthk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hwd.shzxlz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jrb.ehwqpu.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ltb.xuetiantiany.cn

[B13] 判断是否为数字
来源：http://zpn.fanxiaobao.xyz

Py:   isinstance(x, (int, float))
来源：http://qyd.ppjwa.cn

PHP:  is_numeric($x)
来源：http://jdt.zycfv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xqx.daxiang520.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://emz.yfazqb.com

Java: x instanceof Number
来源：http://khu.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tyg.ydjk.org.cn

Ruby: x.is_a?(Numeric)
来源：http://tsw.shangyingyoupin.top

C#:   x is int or double or decimal
来源：http://yxq.smart0.xyz

[B14] 判断值是否在集合内
来源：http://zyn.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rgq.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uzu.chenlongwang.top

JS:   [1, 2, 3].includes(x)
来源：http://ner.guannengcc.top

TS:   [1, 2, 3].includes(x)
来源：http://hhu.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gjg.zhongyouzk.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://exq.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lqk.xingfuxueyuan.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rlv.mhx1999.top

[B15] 布尔运算与取反
来源：http://cjm.zhoulong.xyz

Py:   a and b or not c
来源：http://cfu.cqqwz.cn

PHP:  $a && $b || !$c
来源：http://wlq.bbcook.cn

JS:   a && b || !c
来源：http://zac.jinghuilouyu.cn

TS:   a && b || !c
来源：http://jev.shangyingyoupin.top

Java: a && b || !c
来源：http://bmx.zhengqikj.top

Go:   a && b || !c
来源：http://bjy.haohaochexian.top

Ruby: a && b || !c
来源：http://ocv.hesvh.cn

C#:   a && b || !c
来源：http://baa.hywenlv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uxb.cqqwz.cn

Py:   if not data: return
来源：http://asx.yangfankeji.com

PHP:  if (!$data) { return; }
来源：http://eks.zhongyouzk.top

JS:   if (!data) return;
来源：http://urr.sxryk.cn

TS:   if (!data) return;
来源：http://oer.9152youxi.cn

Java: if (data == null) return;
来源：http://irt.aibaodan.cn

Go:   if data == nil { return }
来源：http://aaq.jinghuilouyu.cn

Ruby: return if data.nil?
来源：http://yjj.ivvv.top

C#:   if (data == null) return;
来源：http://cwn.dianchejie.cn

================================================================================
来源：http://jrp.shanyushiyangtech.top

C. 函数与作用域
来源：http://ktb.zycfv.cn

================================================================================
来源：http://swc.aibaodan.cn

[C01] 定义函数
来源：http://xtp.smart0.xyz

Py:   def add(a, b): return a + b
来源：http://kwx.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kps.gaohongyu789.top

JS:   function add(a, b) { return a + b; }
来源：http://frh.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uiv.chenzaomai.com

Java: static int add(int a, int b) { return a + b; }
来源：http://cfm.zhixingplan.top

Go:   func add(a, b int) int { return a + b }
来源：http://hpe.fktsv.cn

Ruby: def add(a, b); a + b; end
来源：http://alw.shangyingyoupin.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fjl.zhixingplan.top

[C02] 默认参数
来源：http://wze.hnxiangtu.top

Py:   def greet(name="World"): return name
来源：http://qor.shangyingyoupin.top

PHP:  function greet($name = "World") { return $name; }
来源：http://sop.ehwqpu.com

JS:   function greet(name = "World") { return name; }
来源：http://yna.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://abo.dianchejie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tls.haohaochexian.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://drw.sweek.top

Ruby: def greet(name = "World") = name
来源：http://uvf.jinqigfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://kxx.jqgufenzy.top

[C03] 可变参数
来源：http://par.pengpengdd.cyou

Py:   def total(*args): return sum(args)
来源：http://jyo.jinqigufen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ykf.zhaomingkeji.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dwc.hysaishi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bkx.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dbp.hysaishi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ndo.vqdsnc.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qhu.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jxn.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://jpz.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wcf.yuanzhike.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jso.shuidangran.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uri.tian-w.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ulj.zhoulong.xyz

Java: // 无：用 Builder 模式或 record
来源：http://izh.epnwcf.com

Go:   // 无：用配置结构体参数
来源：http://ihh.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://lrs.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://ifj.316326.xyz

[C05] 返回多个值
来源：http://tcq.zdqjudy.top

Py:   return a, b
来源：http://tdz.yonumen.top

PHP:  return [$a, $b];
来源：http://mry.jqgfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rqc.smart0.xyz

TS:   return { a, b };
来源：http://kun.52xcode.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mne.havefunace.top

Go:   return a, b
来源：http://moi.yj20258888.top

Ruby: return a, b
来源：http://diz.zhiwuduotai.top

C#:   return (a, b);              // ValueTuple
来源：http://nvv.yj202588.top

[C06] 匿名函数 / lambda
来源：http://edy.tanke756.top

Py:   square = lambda x: x * x
来源：http://xbz.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dss.vehdjk.com

JS:   const square = x => x * x;
来源：http://dby.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://cki.ywan-chungtsiang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ogc.hesvh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ljt.zhoulong.xyz

Ruby: square = ->(x) { x * x }
来源：http://oei.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qpv.cucudq.cn

[C07] 把函数作为参数传入
来源：http://fbr.hfpthk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fdn.shuidangran.top

PHP:  array_map("strtoupper", $arr);
来源：http://max.9152youxi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rkc.yonumen.top

TS:   arr.map(String)
来源：http://oex.yj20258.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://frq.jyoumei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dzf.ivvv.top

Ruby: arr.map(&:upcase)
来源：http://pcl.zhiwuduotai.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dka.guowangkeji.top

[C08] 闭包
来源：http://ybi.sxryk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://etz.sufxvd.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rxq.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gcb.hcnkem.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ylq.hnqzz.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dei.yvedp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uem.jiagoushi.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dra.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xsk.yj20258888.top

[C09] 递归
来源：http://yvw.zdbjq.cn


<!-- 参考信息 -->