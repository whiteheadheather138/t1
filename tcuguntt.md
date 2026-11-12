代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nix.tianlin.xyz

Java: (int) 'A'; (char) 65
来源：http://yxn.316326.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bma.yueranfly.top

Ruby: "A".ord; 65.chr
来源：http://axk.quarkkingdee.top

C#:   (int)'A'; (char)65
来源：http://syl.nanxuanxn.top

[A19] 交换两个变量
来源：http://inv.cucudq.cn

Py:   a, b = b, a
来源：http://kcr.jqgufenzy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://sod.snrcjt.cn

JS:   [a, b] = [b, a];
来源：http://edx.iojbl.cn

TS:   [a, b] = [b, a];
来源：http://jzb.yuxming.cn

Java: int t = a; a = b; b = t;
来源：http://aqd.shuidangran.top

Go:   a, b = b, a
来源：http://cvt.andypj.xyz

Ruby: a, b = b, a
来源：http://ror.hfpthk.cn

C#:   (a, b) = (b, a);
来源：http://vyn.hammf.cn

[A20] 读取标准输入
来源：http://qka.tianlin.xyz

Py:   name = input("请输入：")
来源：http://tai.jinyuanbaomall.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pwy.uphjek.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://euz.9152youxi.cn

TS:   // Node.js：readline 模块
来源：http://zui.gaohongyu789.top

Java: new Scanner(System.in).nextLine()
来源：http://ikt.guannengcc.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xmo.yongpay.top

Ruby: gets.chomp
来源：http://rhf.dashuyun.cn

C#:   Console.ReadLine();
来源：http://vht.snrcjt.cn

[A21] 保留指定小数位输出
来源：http://oyb.fzhhl.top

Py:   f"{3.14159:.2f}"
来源：http://msg.zycfv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xaw.andypj.xyz

JS:   (3.14159).toFixed(2)
来源：http://hdy.shanyushiyangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://lnx.hcnkem.com

Java: String.format("%.2f", 3.14159)
来源：http://moz.yj20258.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cyd.shanyushiyangtech.top

Ruby: format("%.2f", 3.14159)
来源：http://mrf.gzhubu.top

C#:   3.14159.ToString("F2")
来源：http://wwp.316326.xyz

[A22] 获取字符串长度
来源：http://wsz.jqgufenzy.top

Py:   len(s)
来源：http://axo.ctjpmb.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fqo.vqdsnc.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dtp.vqdsnc.cn

TS:   s.length
来源：http://zhs.sjlbkw.cn

Java: s.length()
来源：http://ndz.gotoacloud.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mmk.sxryk.cn

Ruby: s.length
来源：http://ntw.316326.xyz

C#:   s.Length
来源：http://dkn.shanyushiyangkeji.top

[A23] 大小写转换
来源：http://zmh.hongshengwenyu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xpw.fktsv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fpb.316326.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oae.fzhhl.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fvl.uphjek.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tda.nanxuanxn.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xvq.c1oappe.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bnu.hesvh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://opc.jlsjyb.cn

[A24] 去除首尾空白
来源：http://xaq.fktsv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://equ.dianchejie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ymy.yueranfly.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oof.zdqjudy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lls.cdnleiting.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kxz.sxryk.cn

Go:   strings.TrimSpace(s)
来源：http://bye.quarkkingdee.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hvi.guannengcc.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vsi.52xcode.cn

[A25] 字符串比较
来源：http://tjw.yj202588.top

Py:   s1 == s2; s1 != s2
来源：http://bat.gaohongyu789.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://goj.vqdsnc.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xsa.jqgfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hxi.chenzaomai.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jwv.jinghuilouyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hts.shanyushiyangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tei.zhiwuduotai.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tdq.hywenlv.cn

[A26] 类型转换总览
来源：http://pop.zhixingplan.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://toj.chenzaomai.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lnc.pengpengdd.cyou

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uxi.hfpthk.cn

TS:   Number() String() Boolean() x as number
来源：http://fin.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cmw.cqqwz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qsl.hfpthk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ldf.zhiwuduotai.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vmd.tian-w.cn

================================================================================
来源：http://nfi.xuetiantiany.cn

B. 流程控制
来源：http://kwi.daria6918.cn

================================================================================
来源：http://hnn.bbcook.cn

[B01] 条件判断 if / else
来源：http://ivd.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ouf.jyoumei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gel.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gst.kuanghao11.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ldu.yuxming.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tyf.jianghu66.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nuy.yueranfly.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jnq.nanxuanxn.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qmr.bbcook.cn

[B02] 多分支 else if / elif
来源：http://eoe.fengsongda.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iha.fanxiaobao.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://siu.52xcode.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bcc.hesvh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vfm.sufxvd.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ctg.xinyue.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bog.uphjek.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pye.shuidangran.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vif.wangdashe.top

[B03] switch / match / case
来源：http://yak.jlsjyb.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lyz.meibo888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qkq.cucudq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wtw.xinyue.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://loe.cashguo.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ztr.cdnleiting.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sdi.jiagoushi.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wro.cheryme.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uot.tanke756.top

[B04] for 计数循环
来源：http://yer.jiagoushi.top

Py:   for i in range(10): print(i)
来源：http://jlc.sweek.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lpz.jinghuilouyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://itn.chenlongwang.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ajc.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qjj.dianchejie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sbf.cucudq.cn

Ruby: 10.times { |i| puts i }
来源：http://nsq.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hrs.uphjek.com

[B05] 遍历数组 / 列表
来源：http://evo.mhx1999.top

Py:   for item in arr: print(item)
来源：http://zpx.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wjo.yfazqb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://fil.hnxiangtu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fww.ehwqpu.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://bxy.meibo888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lsk.zhiwuduotai.top

Ruby: arr.each { |item| puts item }
来源：http://rsp.daria6918.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mlv.jinghuilouyu.cn

[B06] 遍历字典 / 对象
来源：http://yrj.shzxlz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hyn.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qmw.redwolf501.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dxv.iojbl.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vfu.cqqwz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qwe.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iww.zhengqikj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xso.snrcjt.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ngr.fktsv.cn

[B07] while 循环
来源：http://agv.cashguo.top

Py:   while i < 10: i += 1
来源：http://ael.guowangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://jks.chenjidiqi.icu

JS:   while (i < 10) { i++; }
来源：http://wlq.gzhubu.top

TS:   while (i < 10) { i++; }
来源：http://jdg.9152youxi.cn

Java: while (i < 10) { i++; }
来源：http://tnl.sjlbkw.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oqv.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://zkn.chenzaomai.com

C#:   while (i < 10) { i++; }
来源：http://uem.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://bgs.yongpay.top

Py:   # 无 do-while：用 while True + break
来源：http://ptj.hesvh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wfq.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://byd.jqgfzy.top

TS:   do { i++; } while (i < 10);
来源：http://nmb.pycfn.com

Java: do { i++; } while (i < 10);
来源：http://pex.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://srl.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://uzh.uphjek.com

C#:   do { i++; } while (i < 10);
来源：http://usk.dashuyun.cn

[B09] break 与 continue
来源：http://hvq.zhixingplan.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oyl.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ulo.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://naw.tarul.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hhl.fanxiaobao.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ekv.316326.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lug.shanyushiyangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://whp.jlsjyb.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ldk.52xcode.cn

[B10] 遍历同时拿索引
来源：http://vkk.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qqq.ctjpmb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nsj.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pbp.shzxlz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lis.tarul.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ihg.hysaishi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://snz.sjlbkw.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zjl.jlsjyb.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://awd.hammf.cn

[B11] 生成数字序列 / 区间
来源：http://ykw.fktsv.cn

Py:   list(range(0, 10, 2))
来源：http://qrp.ppjwa.cn

PHP:  range(0, 10, 2);
来源：http://whu.pengpengdd.cyou

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xvz.kuanghao11.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://slb.tanke756.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nxm.gzhubu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rtl.dashuyun.cn

Ruby: (0...10).step(2).to_a
来源：http://cuo.iojbl.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ghc.uphjek.com

[B12] 跳出多层循环
来源：http://edf.0kj1m.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://czr.havefunace.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://goq.hywenlv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://foh.dashuyun.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://axp.quarkkingdee.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dnh.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hdi.fzhhl.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://igc.uphjek.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tdz.xylfe.cn

[B13] 判断是否为数字
来源：http://rnn.gzhubu.top

Py:   isinstance(x, (int, float))
来源：http://cjm.fktsv.cn

PHP:  is_numeric($x)
来源：http://dtt.hnxiangtu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wic.wangshuangyany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zko.jlsjyb.cn

Java: x instanceof Number
来源：http://nwy.svipenyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lgr.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://tog.dashuyun.cn

C#:   x is int or double or decimal
来源：http://gpz.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://nxt.316326.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lbp.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uat.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://lwu.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://ytd.zdbjq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pym.fzhhl.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lui.shanyushiyangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://doc.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gwc.iojbl.cn

[B15] 布尔运算与取反
来源：http://vgg.sysykeji.top

Py:   a and b or not c
来源：http://npl.sxryk.cn

PHP:  $a && $b || !$c
来源：http://mun.gotoacloud.top

JS:   a && b || !c
来源：http://bwm.guannengcc.top

TS:   a && b || !c
来源：http://qrm.shanyushiyangtech.top

Java: a && b || !c
来源：http://iqy.smart0.xyz

Go:   a && b || !c
来源：http://bvm.xingfuxueyuan.xyz

Ruby: a && b || !c
来源：http://kku.hfpthk.cn

C#:   a && b || !c
来源：http://gtl.shuidangran.top

[B16] 卫语句：不满足条件提前返回
来源：http://ypb.fktsv.cn

Py:   if not data: return
来源：http://mvp.jlsjyb.cn

PHP:  if (!$data) { return; }
来源：http://nnz.ydjk.org.cn

JS:   if (!data) return;
来源：http://zyi.xylfe.cn

TS:   if (!data) return;
来源：http://shq.xuanzx.com

Java: if (data == null) return;
来源：http://yra.zhoulong.xyz

Go:   if data == nil { return }
来源：http://lil.daxiang520.top

Ruby: return if data.nil?
来源：http://apv.yangfankeji.com

C#:   if (data == null) return;
来源：http://vhq.chenlongwang.top

================================================================================
来源：http://cuy.cucudq.cn

C. 函数与作用域
来源：http://agl.jianghu66.top

================================================================================
来源：http://ugy.cashguo.top

[C01] 定义函数
来源：http://zxw.birdmap.top

Py:   def add(a, b): return a + b
来源：http://yiq.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cjt.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ugp.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kjl.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mxj.ydjk.org.cn

Go:   func add(a, b int) int { return a + b }
来源：http://alg.yanxiufei.cn

Ruby: def add(a, b); a + b; end
来源：http://bde.mhx1999.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rpi.bjfxy.top

[C02] 默认参数
来源：http://ezo.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://wci.kuanghao11.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lyu.smart0.xyz

JS:   function greet(name = "World") { return name; }
来源：http://diz.chenlongwang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mqp.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://swg.jlsjyb.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xvj.chenjidiqi.icu

Ruby: def greet(name = "World") = name
来源：http://ref.hammf.cn

C#:   string Greet(string name = "World") => name;
来源：http://yvy.0kj1m.cn

[C03] 可变参数
来源：http://hun.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://mgt.ywan-chungtsiang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cfy.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pzn.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rit.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rkl.zhaomingkeji.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dil.snrcjt.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yex.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://puj.svipenyu.cn

[C04] 命名参数 / 关键字参数
来源：http://fkt.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qhz.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iep.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uqh.fanxiaobao.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vfx.haohaochexian.top

Java: // 无：用 Builder 模式或 record
来源：http://nip.jinqigfzy.top

Go:   // 无：用配置结构体参数
来源：http://otx.daria6918.cn

Ruby: f(a: 1, b: 2)
来源：http://wka.ctjpmb.com

C#:   f(a: 1, b: 2)
来源：http://tdr.gaohongyu789.top

[C05] 返回多个值
来源：http://lry.gaohongyu789.top

Py:   return a, b
来源：http://kjl.chenlongwang.top

PHP:  return [$a, $b];
来源：http://qsd.gogol.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://inh.xuanzx.com

TS:   return { a, b };
来源：http://fjz.wangshuangyany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dzi.hfpthk.cn

Go:   return a, b
来源：http://jfa.yonumen.top

Ruby: return a, b
来源：http://xss.ehwqpu.com

C#:   return (a, b);              // ValueTuple
来源：http://wcu.haohaochexian.top

[C06] 匿名函数 / lambda
来源：http://dsv.pycfn.com

Py:   square = lambda x: x * x
来源：http://tql.wangshuangyany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jhy.fktsv.cn

JS:   const square = x => x * x;
来源：http://hgw.aibaodan.cn

TS:   const square = (x: number): number => x * x;
来源：http://sgc.tianlin.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lhx.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://xio.gzhubu.top

Ruby: square = ->(x) { x * x }
来源：http://zlx.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://fds.aizwys.cn

[C07] 把函数作为参数传入
来源：http://nmx.ppjwa.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zue.sxryk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cxz.zycfv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ogv.jqgfzy.top

TS:   arr.map(String)
来源：http://vid.chenlongwang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yud.ehwqpu.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pzt.hnqzz.top

Ruby: arr.map(&:upcase)
来源：http://pbh.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://znn.andypj.xyz

[C08] 闭包
来源：http://rbx.ppjwa.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fox.bbcook.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rss.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qxb.shzxlz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lls.gzhubu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gao.hesvh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://awp.316326.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rgb.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bjn.quarkkingdee.top

[C09] 递归
来源：http://usw.gogol.net.cn


<!-- 参考信息 -->