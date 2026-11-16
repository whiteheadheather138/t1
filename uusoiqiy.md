代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://lda.zhongyouzk.top

[A15] 空值判断与默认值
来源：http://ezp.daxiang520.top

Py:   value = data or "默认值"
来源：http://dht.yuxming.cn

PHP:  $value = $data ?? "默认值";
来源：http://win.fktsv.cn

JS:   const value = data ?? "默认值";
来源：http://urt.sweek.top

TS:   const value = data ?? "默认值";
来源：http://ejn.jqgfzy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dca.kuanghao11.cn

Go:   if data == "" { data = "默认值" }
来源：http://dwo.chenjidiqi.icu

Ruby: value = data || "默认值"
来源：http://sed.xingfuxueyuan.xyz

C#:   var value = data ?? "默认值";
来源：http://kas.yvedp.cn

[A16] 真假值判断规则
来源：http://ecn.guannengcc.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ltr.fktsv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oms.cucudq.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mhw.fehbvm.com

TS:   if (!x) {}
来源：http://mca.ivvv.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gaa.cqqwz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dyj.gotoacloud.top

Ruby: unless x            # nil 与 false 为假
来源：http://dqj.hysaishi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wdj.zdbjq.cn

[A17] 位运算
来源：http://yeu.xingfuxueyuan.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mrh.jinqigfzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gap.yuanzhike.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nrd.mhx1999.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hcq.zdqjudy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dqe.andypj.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jyk.tian-w.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zyr.fktsv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tti.hfpthk.cn

[A18] 字符与 ASCII 码互转
来源：http://osv.pycfn.com

Py:   ord("A"); chr(65)
来源：http://lmi.jqgfzy.top

PHP:  ord("A"); chr(65)
来源：http://rug.bbcook.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wvy.zhengqikj.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mbe.gaohongyu789.top

Java: (int) 'A'; (char) 65
来源：http://faa.jlsjyb.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rza.ydzc1.top

Ruby: "A".ord; 65.chr
来源：http://gzl.tianlin.xyz

C#:   (int)'A'; (char)65
来源：http://wtc.shangyingyoupin.top

[A19] 交换两个变量
来源：http://epn.hammf.cn

Py:   a, b = b, a
来源：http://hju.sjlbkw.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qtd.birdmap.top

JS:   [a, b] = [b, a];
来源：http://gyb.yj20258888.top

TS:   [a, b] = [b, a];
来源：http://den.gotoacloud.top

Java: int t = a; a = b; b = t;
来源：http://zup.jyoumei.cn

Go:   a, b = b, a
来源：http://grw.ywan-chungtsiang.top

Ruby: a, b = b, a
来源：http://yxf.mhx1999.top

C#:   (a, b) = (b, a);
来源：http://tea.daria6918.cn

[A20] 读取标准输入
来源：http://rdq.zhengqikj.top

Py:   name = input("请输入：")
来源：http://gyh.zhoulong.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://hig.shzxlz.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lnw.xinyue.icu

TS:   // Node.js：readline 模块
来源：http://evx.pengpengdd.cyou

Java: new Scanner(System.in).nextLine()
来源：http://qes.daria6918.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yfc.cqqwz.cn

Ruby: gets.chomp
来源：http://sax.ctjpmb.com

C#:   Console.ReadLine();
来源：http://obv.shuidangran.top

[A21] 保留指定小数位输出
来源：http://azl.dashuyun.cn

Py:   f"{3.14159:.2f}"
来源：http://uvj.fehbvm.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jay.yuanzhike.top

JS:   (3.14159).toFixed(2)
来源：http://yrk.feifeiyinyue.top

TS:   (3.14159).toFixed(2)
来源：http://xme.yangfankeji.com

Java: String.format("%.2f", 3.14159)
来源：http://gwx.hysaishi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sqf.yuanzhike.top

Ruby: format("%.2f", 3.14159)
来源：http://znf.bbcook.cn

C#:   3.14159.ToString("F2")
来源：http://xir.c1oappe.top

[A22] 获取字符串长度
来源：http://hmv.cucudq.cn

Py:   len(s)
来源：http://ksr.nwbrower.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nch.quarkkingdee.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cbf.hywenlv.cn

TS:   s.length
来源：http://xgj.fzhhl.top

Java: s.length()
来源：http://uqd.shanyushiyangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fer.zhixingplan.top

Ruby: s.length
来源：http://ydy.iojbl.cn

C#:   s.Length
来源：http://fhu.zhoulong.xyz

[A23] 大小写转换
来源：http://yse.fzhhl.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wtf.hnqzz.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://okl.hcnkem.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kel.guowangkeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uqp.cashguo.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ili.yj20258.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jaq.fengsongda.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qke.quarkkingdee.top

C#:   s.ToUpper(); s.ToLower()
来源：http://klu.316326.xyz

[A24] 去除首尾空白
来源：http://ftf.sxryk.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ouy.xuanzx.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ouc.iojbl.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kih.iojbl.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fti.zhijiandao.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vew.birdmap.top

Go:   strings.TrimSpace(s)
来源：http://npo.iojbl.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://olj.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eth.jqgfzy.top

[A25] 字符串比较
来源：http://gge.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://szg.dianchejie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zua.chenlongwang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mkd.hammf.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zse.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ydz.cheryme.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mmi.jyoumei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jhl.nanxinkj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ima.ehwqpu.com

[A26] 类型转换总览
来源：http://leo.vqdsnc.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zbq.jqgufenzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pmg.yongpay.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blq.yongpay.top

TS:   Number() String() Boolean() x as number
来源：http://sbx.fzhhl.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://djl.ehwqpu.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vsm.bjfxy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://scr.birdmap.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tcg.xuetiantiany.cn

================================================================================
来源：http://wbb.ehwqpu.com

B. 流程控制
来源：http://wud.jianghu66.top

================================================================================
来源：http://inl.ivvv.top

[B01] 条件判断 if / else
来源：http://dmc.xingfuxueyuan.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://xox.andypj.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xyc.xinyue.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hxi.ehwqpu.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hrn.tarul.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sip.epnwcf.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://obr.hfpthk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dlk.uphjek.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xeo.uphjek.com

[B02] 多分支 else if / elif
来源：http://wpl.hnqzz.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://obm.hcnkem.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rxb.yfazqb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://veu.zhiwuduotai.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zmf.gogol.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://noz.zhaomingkeji.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ddi.yangfankeji.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ywb.hywenlv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ivn.jinghuilouyu.cn

[B03] switch / match / case
来源：http://ynv.ywan-chungtsiang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kim.gotoacloud.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uym.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://avp.nwbrower.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ulw.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hkh.sweek.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mwf.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xkq.jiagoushi.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zqt.ctjpmb.com

[B04] for 计数循环
来源：http://ttn.316326.xyz

Py:   for i in range(10): print(i)
来源：http://uly.zhongyouzk.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://flq.gaohongyu789.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rsg.daria6918.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mhu.zdbjq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ogh.shangyingyoupin.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nji.hnqzz.top

Ruby: 10.times { |i| puts i }
来源：http://czv.yangfankeji.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://exs.yfazqb.com

[B05] 遍历数组 / 列表
来源：http://vnk.chenzaomai.com

Py:   for item in arr: print(item)
来源：http://xrq.cucudq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kej.aizwys.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://edo.bjfxy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mky.316326.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://uyd.shzxlz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ekd.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://ecz.fzhhl.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wcv.zhixingplan.top

[B06] 遍历字典 / 对象
来源：http://jda.jinyuanbaomall.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cnq.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jqi.xinyue.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nlh.fehbvm.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lla.ppjwa.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rtd.gogol.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kpj.hongshengwenyu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gbq.shuidangran.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://txx.sufxvd.cn

[B07] while 循环
来源：http://bpz.yj20258888.top

Py:   while i < 10: i += 1
来源：http://axi.yueranfly.top

PHP:  while ($i < 10) { $i++; }
来源：http://gpm.daxiang520.top

JS:   while (i < 10) { i++; }
来源：http://jme.guannengcc.top

TS:   while (i < 10) { i++; }
来源：http://nsz.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://atw.chenlongwang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dua.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://ide.feifeiyinyue.top

C#:   while (i < 10) { i++; }
来源：http://dtp.ydzc1.top

[B08] do-while（至少执行一次）
来源：http://emw.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://isd.hongshengwenyu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vyy.fengsongda.top

JS:   do { i++; } while (i < 10);
来源：http://rnw.ivvv.top

TS:   do { i++; } while (i < 10);
来源：http://gqz.jlsjyb.cn

Java: do { i++; } while (i < 10);
来源：http://iyi.zhiwuduotai.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wxv.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ffp.yfazqb.com

C#:   do { i++; } while (i < 10);
来源：http://ygx.tian-w.cn

[B09] break 与 continue
来源：http://skj.daria6918.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qnv.tianlin.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bvy.tianlin.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tlg.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wnn.svipenyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://olk.shanyushiyangtech.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sur.zhaomingkeji.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://myt.hongshengwenyu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uxl.ydjk.org.cn

[B10] 遍历同时拿索引
来源：http://lqs.hysaishi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nxb.hesvh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xsf.sjlbkw.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uxv.jinghuilouyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ilg.hywenlv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dvw.shanyushiyangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ynw.zhijiandao.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ggr.wangshuangyany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bnu.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://dsc.fanxiaobao.xyz

Py:   list(range(0, 10, 2))
来源：http://qcr.chenzaomai.com

PHP:  range(0, 10, 2);
来源：http://ttu.jqgfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ivp.zycfv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vxt.ydjk.org.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://njr.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jwx.jqgufenzy.top

Ruby: (0...10).step(2).to_a
来源：http://cjz.vehdjk.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fun.aibaodan.cn

[B12] 跳出多层循环
来源：http://ldx.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lgi.jyoumei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rbm.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://acd.fanxiaobao.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://epb.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://chw.yfazqb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://umw.xziqi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://con.yueranfly.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oai.zycfv.cn

[B13] 判断是否为数字
来源：http://xpy.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://zuy.yj20258.top

PHP:  is_numeric($x)
来源：http://wyy.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sgu.xingfuxueyuan.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pgt.yanxiufei.cn

Java: x instanceof Number
来源：http://qhm.jlsjyb.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dxa.jinqigfzy.top

Ruby: x.is_a?(Numeric)
来源：http://avw.shangyingyoupin.top

C#:   x is int or double or decimal
来源：http://qkc.epnwcf.com

[B14] 判断值是否在集合内
来源：http://lly.guannengcc.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cdo.ydjk.org.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eom.xingfuxueyuan.xyz

JS:   [1, 2, 3].includes(x)
来源：http://xia.yfazqb.com

TS:   [1, 2, 3].includes(x)
来源：http://bja.hfpthk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uuw.dianchejie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lgk.aizwys.cn

Ruby: [1, 2, 3].include?(x)
来源：http://agh.ivvv.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tha.bbcook.cn

[B15] 布尔运算与取反
来源：http://lev.shuidangran.top

Py:   a and b or not c
来源：http://edd.xuetiantiany.cn

PHP:  $a && $b || !$c
来源：http://vjv.zhiwuduotai.top

JS:   a && b || !c
来源：http://wpt.tian-w.cn

TS:   a && b || !c
来源：http://aao.chenzaomai.com

Java: a && b || !c
来源：http://ljh.52xcode.cn

Go:   a && b || !c
来源：http://dlf.zdqjudy.top

Ruby: a && b || !c
来源：http://jgt.mhx1999.top

C#:   a && b || !c
来源：http://dap.sufxvd.cn

[B16] 卫语句：不满足条件提前返回
来源：http://unm.haohaochexian.top

Py:   if not data: return
来源：http://pfc.birdmap.top

PHP:  if (!$data) { return; }
来源：http://akd.snrcjt.cn

JS:   if (!data) return;
来源：http://mvl.ywan-chungtsiang.top

TS:   if (!data) return;
来源：http://lpd.ydjk.org.cn

Java: if (data == null) return;
来源：http://wtg.jinqigufen.top

Go:   if data == nil { return }
来源：http://kze.havefunace.top

Ruby: return if data.nil?
来源：http://nxi.hesvh.cn

C#:   if (data == null) return;
来源：http://lka.yangfankeji.com

================================================================================
来源：http://atd.hesvh.cn

C. 函数与作用域
来源：http://qrg.sxryk.cn

================================================================================
来源：http://fqn.ivvv.top

[C01] 定义函数
来源：http://cts.gogol.net.cn

Py:   def add(a, b): return a + b
来源：http://bgf.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zwk.epnwcf.com

JS:   function add(a, b) { return a + b; }
来源：http://vcw.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://inl.0kj1m.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bue.quarkkingdee.top

Go:   func add(a, b int) int { return a + b }
来源：http://cuq.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://hcr.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qtj.ydjk.org.cn

[C02] 默认参数
来源：http://xca.iojbl.cn

Py:   def greet(name="World"): return name
来源：http://qkd.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hha.hywenlv.cn

JS:   function greet(name = "World") { return name; }
来源：http://rfl.yj20258.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kgk.zycfv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://goo.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xtg.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://plo.hcnkem.com

C#:   string Greet(string name = "World") => name;
来源：http://rup.hfpthk.cn

[C03] 可变参数
来源：http://wxs.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://mne.c1oappe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ply.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cqy.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://byr.nanxinkj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://evr.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sdu.bjfxy.top

Ruby: def total(*nums); nums.sum; end
来源：http://cfl.feifeiyinyue.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zxf.wangshuangyany.cn

[C04] 命名参数 / 关键字参数
来源：http://oxy.kuanghao11.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://far.tianlin.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baj.aizwys.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kii.cucudq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yep.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://cub.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://mat.hywenlv.cn

Ruby: f(a: 1, b: 2)
来源：http://fhb.jinyuanbaomall.cn

C#:   f(a: 1, b: 2)
来源：http://zmx.quarkkingdee.top

[C05] 返回多个值
来源：http://mek.uphjek.com

Py:   return a, b
来源：http://rwg.havefunace.top

PHP:  return [$a, $b];
来源：http://znz.haohaochexian.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yyk.gogol.net.cn

TS:   return { a, b };
来源：http://fyf.hysaishi.cn


<!-- 参考信息 -->