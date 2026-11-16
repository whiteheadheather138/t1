代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://lry.ctjpmb.com

Py:   ord("A"); chr(65)
来源：http://jam.jinqigfzy.top

PHP:  ord("A"); chr(65)
来源：http://fpd.yanxiufei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zug.hnxiangtu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xfn.zhaomingkeji.xyz

Java: (int) 'A'; (char) 65
来源：http://meu.ydzc1.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ted.ywan-chungtsiang.top

Ruby: "A".ord; 65.chr
来源：http://tsl.tarul.cn

C#:   (int)'A'; (char)65
来源：http://fgj.yanxiufei.cn

[A19] 交换两个变量
来源：http://snl.jqgfzy.top

Py:   a, b = b, a
来源：http://owm.hfpthk.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://twc.bjfxy.top

JS:   [a, b] = [b, a];
来源：http://njf.shzxlz.cn

TS:   [a, b] = [b, a];
来源：http://bri.svipenyu.cn

Java: int t = a; a = b; b = t;
来源：http://fei.gaohongyu789.top

Go:   a, b = b, a
来源：http://gsi.jinqigfzy.top

Ruby: a, b = b, a
来源：http://qln.hysaishi.cn

C#:   (a, b) = (b, a);
来源：http://wru.tian-w.cn

[A20] 读取标准输入
来源：http://dcv.jlsjyb.cn

Py:   name = input("请输入：")
来源：http://sxd.yfazqb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://woq.ppjwa.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cpu.yvedp.cn

TS:   // Node.js：readline 模块
来源：http://scs.zhongyouzk.top

Java: new Scanner(System.in).nextLine()
来源：http://utu.ppjwa.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mwa.dashuyun.cn

Ruby: gets.chomp
来源：http://hzp.havefunace.top

C#:   Console.ReadLine();
来源：http://yhz.yonumen.top

[A21] 保留指定小数位输出
来源：http://wpm.hnqzz.top

Py:   f"{3.14159:.2f}"
来源：http://qwt.iojbl.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://eex.chenzaomai.com

JS:   (3.14159).toFixed(2)
来源：http://iqn.jinqigufen.top

TS:   (3.14159).toFixed(2)
来源：http://lyl.zhongyouzk.top

Java: String.format("%.2f", 3.14159)
来源：http://frm.shzxlz.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://svb.hcnkem.com

Ruby: format("%.2f", 3.14159)
来源：http://lxf.cashguo.top

C#:   3.14159.ToString("F2")
来源：http://fpu.yj202588.top

[A22] 获取字符串长度
来源：http://bia.smart0.xyz

Py:   len(s)
来源：http://cev.shanyushiyangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bte.svipenyu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pkr.bjfxy.top

TS:   s.length
来源：http://noa.zhijiandao.cn

Java: s.length()
来源：http://vws.shanyushiyangtech.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://syg.smart0.xyz

Ruby: s.length
来源：http://gcl.hysaishi.cn

C#:   s.Length
来源：http://wgt.cheryme.top

[A23] 大小写转换
来源：http://ryc.yj20258888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://jaa.zdqjudy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cmg.hnxiangtu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xpy.fanxiaobao.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sep.gzhubu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mcx.jinqigufen.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pzj.daxiang520.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ibv.mhx1999.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ilt.yueranfly.top

[A24] 去除首尾空白
来源：http://cxv.fktsv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eak.vqdsnc.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zej.yongpay.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://awa.gzhubu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qja.tarul.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ffs.shanyushiyangtech.top

Go:   strings.TrimSpace(s)
来源：http://usu.daria6918.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lff.hesvh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wkb.ybcxt.top

[A25] 字符串比较
来源：http://mzt.hongshengwenyu.top

Py:   s1 == s2; s1 != s2
来源：http://cxg.andypj.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gil.sysykeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://njl.hfpthk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xmx.jinyuanbaomall.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rdh.gzhubu.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tge.snrcjt.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ljq.meibo888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ryr.xinyue.icu

[A26] 类型转换总览
来源：http://lrh.snrcjt.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gcn.xuanzx.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dgt.jqgfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ilg.jqgufenzy.top

TS:   Number() String() Boolean() x as number
来源：http://tax.havefunace.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wdf.wangdashe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qxa.sysykeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://pfu.xuetiantiany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gcv.jinyuanbaomall.cn

================================================================================
来源：http://ert.uphjek.com

B. 流程控制
来源：http://iuc.xuanzx.com

================================================================================
来源：http://onn.ctjpmb.com

[B01] 条件判断 if / else
来源：http://zfn.nanxuanxn.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qym.cheryme.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rbf.fktsv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sej.cucudq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://obc.gaohongyu789.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qql.jinqigfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wae.9152youxi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jsf.pycfn.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mqh.fengsongda.top

[B02] 多分支 else if / elif
来源：http://fer.ivvv.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fhq.sjlbkw.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ykm.dianchejie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dhk.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cye.yuanzhike.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xbe.gzhubu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lde.smart0.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ats.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://meu.quarkkingdee.top

[B03] switch / match / case
来源：http://xit.cucudq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hac.nanxinkj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kmp.hysaishi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gwb.cqqwz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fmq.shzxlz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://miy.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mtw.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mjj.yj202588.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qhf.pycfn.com

[B04] for 计数循环
来源：http://pwt.pengpengdd.cyou

Py:   for i in range(10): print(i)
来源：http://zss.snrcjt.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vcq.jiagoushi.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bxs.wangdashe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jpm.mhx1999.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wgf.xuanzx.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://okq.jinqigufen.top

Ruby: 10.times { |i| puts i }
来源：http://skp.xylfe.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nid.zhoulong.xyz

[B05] 遍历数组 / 列表
来源：http://urh.yuxming.cn

Py:   for item in arr: print(item)
来源：http://oaf.jiagoushi.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pcb.cheryme.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gkh.daxiang520.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tkh.yonumen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://anp.hnqzz.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fox.hnqzz.top

Ruby: arr.each { |item| puts item }
来源：http://caz.sysykeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://huh.guannengcc.top

[B06] 遍历字典 / 对象
来源：http://cvk.vqdsnc.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fdf.cashguo.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zjr.smart0.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://edn.jlsjyb.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yxp.yanxiufei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://upo.hammf.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fze.zhongyouzk.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qnd.yj20258.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://irv.jinghuilouyu.cn

[B07] while 循环
来源：http://app.yj20258888.top

Py:   while i < 10: i += 1
来源：http://tda.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pot.feifeiyinyue.top

JS:   while (i < 10) { i++; }
来源：http://wfz.yuxming.cn

TS:   while (i < 10) { i++; }
来源：http://ltv.yongpay.top

Java: while (i < 10) { i++; }
来源：http://qny.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yvf.yonumen.top

Ruby: while i < 10; i += 1; end
来源：http://kax.aibaodan.cn

C#:   while (i < 10) { i++; }
来源：http://vdd.shzxlz.cn

[B08] do-while（至少执行一次）
来源：http://qjv.hesvh.cn

Py:   # 无 do-while：用 while True + break
来源：http://iqx.xziqi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rud.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://gzz.aizwys.cn

TS:   do { i++; } while (i < 10);
来源：http://tov.yongpay.top

Java: do { i++; } while (i < 10);
来源：http://wix.jianghu66.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ztl.haohaochexian.top

Ruby: begin; i += 1; end while i < 10
来源：http://wbx.jyoumei.cn

C#:   do { i++; } while (i < 10);
来源：http://ahg.xuetiantiany.cn

[B09] break 与 continue
来源：http://pbo.ydjk.org.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ona.hammf.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ohe.wangshuangyany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kwb.birdmap.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://upr.fehbvm.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iun.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bhe.daria6918.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://srv.guannengcc.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://elu.c1oappe.top

[B10] 遍历同时拿索引
来源：http://cyh.zhiwuduotai.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jnj.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ret.hammf.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dwu.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rda.cashguo.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fhc.jlsjyb.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://adp.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://chs.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jnb.jinyuanbaomall.cn

[B11] 生成数字序列 / 区间
来源：http://mnx.cashguo.top

Py:   list(range(0, 10, 2))
来源：http://frb.cheryme.top

PHP:  range(0, 10, 2);
来源：http://ywd.zhijiandao.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ula.kuanghao11.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ylf.vqdsnc.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ajc.fengsongda.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://znr.sweek.top

Ruby: (0...10).step(2).to_a
来源：http://bpi.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zgl.zhongyouzk.top

[B12] 跳出多层循环
来源：http://kdc.smart0.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://hyd.zhixingplan.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jlj.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wyl.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xlh.shangyingyoupin.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://naz.jinyuanbaomall.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wrk.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gap.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mlb.yfazqb.com

[B13] 判断是否为数字
来源：http://fvp.dashuyun.cn

Py:   isinstance(x, (int, float))
来源：http://meo.shanyushiyangtech.top

PHP:  is_numeric($x)
来源：http://eka.pengpengdd.cyou

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jqf.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ycd.gaohongyu789.top

Java: x instanceof Number
来源：http://jpb.vqdsnc.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fcs.hongshengwenyu.top

Ruby: x.is_a?(Numeric)
来源：http://xpv.dashuyun.cn

C#:   x is int or double or decimal
来源：http://iay.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://gxl.havefunace.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hfd.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ffd.fktsv.cn

JS:   [1, 2, 3].includes(x)
来源：http://ezk.hongshengwenyu.top

TS:   [1, 2, 3].includes(x)
来源：http://olp.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://lij.c1oappe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uwb.chenlongwang.top

Ruby: [1, 2, 3].include?(x)
来源：http://sap.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wkb.shanyushiyangkeji.top

[B15] 布尔运算与取反
来源：http://hgv.316326.xyz

Py:   a and b or not c
来源：http://jsm.guannengcc.top

PHP:  $a && $b || !$c
来源：http://byx.gotoacloud.top

JS:   a && b || !c
来源：http://xwb.yonumen.top

TS:   a && b || !c
来源：http://cvq.hfpthk.cn

Java: a && b || !c
来源：http://gkq.ywan-chungtsiang.top

Go:   a && b || !c
来源：http://xah.ctjpmb.com

Ruby: a && b || !c
来源：http://ogl.cashguo.top

C#:   a && b || !c
来源：http://wsg.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://szj.xuetiantiany.cn

Py:   if not data: return
来源：http://wcp.chenzaomai.com

PHP:  if (!$data) { return; }
来源：http://gep.hongshengwenyu.top

JS:   if (!data) return;
来源：http://lzg.ehwqpu.com

TS:   if (!data) return;
来源：http://iwe.ivvv.top

Java: if (data == null) return;
来源：http://heu.zhiwuduotai.top

Go:   if data == nil { return }
来源：http://jni.wangshuangyany.cn

Ruby: return if data.nil?
来源：http://hzu.wangshuangyany.cn

C#:   if (data == null) return;
来源：http://xoc.cqqwz.cn

================================================================================
来源：http://kzh.guannengcc.top

C. 函数与作用域
来源：http://wfj.zhongyouzk.top

================================================================================
来源：http://tly.fktsv.cn

[C01] 定义函数
来源：http://hsv.yj202588.top

Py:   def add(a, b): return a + b
来源：http://dyk.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ugw.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://oaj.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dzm.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pos.fktsv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qae.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://itl.hfpthk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pqt.hnxiangtu.top

[C02] 默认参数
来源：http://elp.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://icq.feifeiyinyue.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bkl.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://nuu.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://prm.ywan-chungtsiang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bav.0kj1m.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ipn.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://jmp.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://gej.nanxuanxn.top

[C03] 可变参数
来源：http://jgm.zhengqikj.top

Py:   def total(*args): return sum(args)
来源：http://auv.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wfj.fengsongda.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rio.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dqo.daria6918.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nob.yangfankeji.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nbr.yvedp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dmg.0kj1m.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fej.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://gmq.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yzi.ydzc1.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ptc.gaohongyu789.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iya.zhengqikj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ivt.dianchejie.cn

Java: // 无：用 Builder 模式或 record
来源：http://rxk.sufxvd.cn

Go:   // 无：用配置结构体参数
来源：http://hia.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://kns.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://qsu.shzxlz.cn

[C05] 返回多个值
来源：http://vsp.svipenyu.cn

Py:   return a, b
来源：http://dcv.zhongyouzk.top

PHP:  return [$a, $b];
来源：http://ags.dashuyun.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bpg.fehbvm.com

TS:   return { a, b };
来源：http://jjo.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://neh.ctjpmb.com

Go:   return a, b
来源：http://ajp.epnwcf.com

Ruby: return a, b
来源：http://usk.mhx1999.top

C#:   return (a, b);              // ValueTuple
来源：http://pxk.yanxiufei.cn

[C06] 匿名函数 / lambda
来源：http://npg.ybcxt.top

Py:   square = lambda x: x * x
来源：http://rkj.xuetiantiany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xjf.bbcook.cn

JS:   const square = x => x * x;
来源：http://siu.daria6918.cn

TS:   const square = (x: number): number => x * x;
来源：http://wqk.ydjk.org.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nwk.bjfxy.top

Go:   sq := func(x int) int { return x * x }
来源：http://ibd.zhixingplan.top

Ruby: square = ->(x) { x * x }
来源：http://xxz.tarul.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uis.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://wau.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fzn.fengsongda.top

PHP:  array_map("strtoupper", $arr);
来源：http://cwc.pycfn.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jli.pycfn.com

TS:   arr.map(String)
来源：http://dgh.316326.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aif.pycfn.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qaj.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://jck.yj20258.top

C#:   arr.Select(s => s.ToUpper())
来源：http://adl.wangshuangyany.cn

[C08] 闭包
来源：http://eiy.gzhubu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://awz.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rql.chenjidiqi.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oow.birdmap.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jfg.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wfd.sjlbkw.cn


<!-- 参考信息 -->