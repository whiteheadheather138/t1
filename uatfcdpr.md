代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aht.jinqigfzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://euh.mhx1999.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ztw.bbcook.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wgn.yj20258888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://raa.ctjpmb.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bfd.zhaomingkeji.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vvr.wangshuangyany.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gsq.fzhhl.top

[A18] 字符与 ASCII 码互转
来源：http://izb.fzhhl.top

Py:   ord("A"); chr(65)
来源：http://ozq.zhoulong.xyz

PHP:  ord("A"); chr(65)
来源：http://gzg.yuanzhike.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uah.dashuyun.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qld.aizwys.cn

Java: (int) 'A'; (char) 65
来源：http://ysk.andypj.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fjs.sweek.top

Ruby: "A".ord; 65.chr
来源：http://eet.iojbl.cn

C#:   (int)'A'; (char)65
来源：http://mfx.jianghu66.top

[A19] 交换两个变量
来源：http://cyn.andypj.xyz

Py:   a, b = b, a
来源：http://poa.hammf.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jvu.yuanzhike.top

JS:   [a, b] = [b, a];
来源：http://qlb.hysaishi.cn

TS:   [a, b] = [b, a];
来源：http://syp.daxiang520.top

Java: int t = a; a = b; b = t;
来源：http://gec.chenjidiqi.icu

Go:   a, b = b, a
来源：http://odt.snrcjt.cn

Ruby: a, b = b, a
来源：http://boo.cashguo.top

C#:   (a, b) = (b, a);
来源：http://jgk.wangshuangyany.cn

[A20] 读取标准输入
来源：http://jxr.jyoumei.cn

Py:   name = input("请输入：")
来源：http://ean.hcnkem.com

PHP:  $name = trim(fgets(STDIN));
来源：http://pdu.hnxiangtu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://whv.hcnkem.com

TS:   // Node.js：readline 模块
来源：http://adq.jinyuanbaomall.cn

Java: new Scanner(System.in).nextLine()
来源：http://wkr.c1oappe.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hwk.zhoulong.xyz

Ruby: gets.chomp
来源：http://hwo.jiagoushi.top

C#:   Console.ReadLine();
来源：http://qlz.bjfxy.top

[A21] 保留指定小数位输出
来源：http://bnw.fzhhl.top

Py:   f"{3.14159:.2f}"
来源：http://ivg.fehbvm.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://whe.yj20258.top

JS:   (3.14159).toFixed(2)
来源：http://rxd.yangfankeji.com

TS:   (3.14159).toFixed(2)
来源：http://pfz.52xcode.cn

Java: String.format("%.2f", 3.14159)
来源：http://flh.sysykeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fso.tarul.cn

Ruby: format("%.2f", 3.14159)
来源：http://snm.fktsv.cn

C#:   3.14159.ToString("F2")
来源：http://alk.jyoumei.cn

[A22] 获取字符串长度
来源：http://gpt.jinghuilouyu.cn

Py:   len(s)
来源：http://akx.cucudq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://upe.fktsv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dbl.zycfv.cn

TS:   s.length
来源：http://fxg.xinyue.icu

Java: s.length()
来源：http://ltd.uphjek.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oau.shuidangran.top

Ruby: s.length
来源：http://zoh.fengsongda.top

C#:   s.Length
来源：http://jel.epnwcf.com

[A23] 大小写转换
来源：http://lef.uphjek.com

Py:   s.upper(); s.lower(); s.title()
来源：http://hjv.cqqwz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://woe.shanyushiyangtech.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://saf.hcnkem.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mxv.ydzc1.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ygn.hongshengwenyu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cpc.fktsv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bkc.dashuyun.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zmp.kuanghao11.cn

[A24] 去除首尾空白
来源：http://vdl.yj20258888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ozv.yj20258.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wpj.yangfankeji.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cuv.hesvh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://geg.yfazqb.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lgf.ydzc1.top

Go:   strings.TrimSpace(s)
来源：http://yxn.ctjpmb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eyu.birdmap.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hml.hongshengwenyu.top

[A25] 字符串比较
来源：http://awd.ctjpmb.com

Py:   s1 == s2; s1 != s2
来源：http://ocd.smart0.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fzl.jinqigufen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rcl.316326.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jhz.hammf.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zxl.nanxinkj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zvm.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nwj.hfpthk.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ply.cqqwz.cn

[A26] 类型转换总览
来源：http://cat.316326.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rbz.uphjek.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uke.yangfankeji.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://juh.xinyue.icu

TS:   Number() String() Boolean() x as number
来源：http://bsw.iojbl.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lqg.gogol.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vtc.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rrg.smart0.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yru.vqdsnc.cn

================================================================================
来源：http://niy.snrcjt.cn

B. 流程控制
来源：http://gha.yongpay.top

================================================================================
来源：http://ewg.sjlbkw.cn

[B01] 条件判断 if / else
来源：http://jab.zhongyouzk.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cqp.sjlbkw.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kom.jinqigfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hvl.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vwn.zycfv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nlx.quarkkingdee.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rke.nwbrower.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gxw.guowangkeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ypa.zhixingplan.top

[B02] 多分支 else if / elif
来源：http://pqw.jlsjyb.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fek.smart0.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mfg.zhixingplan.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kwd.epnwcf.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pln.hongshengwenyu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://btb.meibo888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kut.tarul.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cnk.zdbjq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kjr.yueranfly.top

[B03] switch / match / case
来源：http://wjq.xinyue.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://upf.chenzaomai.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://anp.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://idh.daxiang520.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blw.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://krm.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ouw.shangyingyoupin.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xrq.tianlin.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nmq.birdmap.top

[B04] for 计数循环
来源：http://mza.ybcxt.top

Py:   for i in range(10): print(i)
来源：http://szy.xuanzx.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pfn.hammf.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eck.tarul.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bvr.xinyue.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://roz.sufxvd.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wzq.svipenyu.cn

Ruby: 10.times { |i| puts i }
来源：http://sul.cqqwz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ezk.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://dwz.hysaishi.cn

Py:   for item in arr: print(item)
来源：http://wjx.9152youxi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ars.yongpay.top

JS:   for (const item of arr) { console.log(item); }
来源：http://geq.zhoulong.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://iqn.chenjidiqi.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://xks.fehbvm.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ylw.sjlbkw.cn

Ruby: arr.each { |item| puts item }
来源：http://zmf.havefunace.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qgo.aibaodan.cn

[B06] 遍历字典 / 对象
来源：http://ldf.ppjwa.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hqw.tanke756.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://trh.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dwu.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://akw.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cgd.daria6918.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wkg.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qdn.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jxc.yongpay.top

[B07] while 循环
来源：http://bfo.daxiang520.top

Py:   while i < 10: i += 1
来源：http://gda.gaohongyu789.top

PHP:  while ($i < 10) { $i++; }
来源：http://efu.pycfn.com

JS:   while (i < 10) { i++; }
来源：http://lco.smart0.xyz

TS:   while (i < 10) { i++; }
来源：http://pfb.sysykeji.top

Java: while (i < 10) { i++; }
来源：http://cku.vqdsnc.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dyv.shangyingyoupin.top

Ruby: while i < 10; i += 1; end
来源：http://mnz.aizwys.cn

C#:   while (i < 10) { i++; }
来源：http://wlu.sjlbkw.cn

[B08] do-while（至少执行一次）
来源：http://sto.jiagoushi.top

Py:   # 无 do-while：用 while True + break
来源：http://mfg.cucudq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bno.jinqigufen.top

JS:   do { i++; } while (i < 10);
来源：http://zup.52xcode.cn

TS:   do { i++; } while (i < 10);
来源：http://mee.hnxiangtu.top

Java: do { i++; } while (i < 10);
来源：http://ppr.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xvt.xziqi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fhg.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://qof.jlsjyb.cn

[B09] break 与 continue
来源：http://itu.tianlin.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dwv.fktsv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ipx.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vze.cdnleiting.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lch.fzhhl.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://psn.zhiwuduotai.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gpz.yfazqb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://arj.cdnleiting.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lal.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://qfr.redwolf501.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xpm.zhengqikj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ics.fengsongda.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bap.birdmap.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iqz.birdmap.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nvd.yfazqb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jlx.pengpengdd.cyou

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rnl.yueranfly.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sff.zhongyouzk.top

[B11] 生成数字序列 / 区间
来源：http://zdl.jinqigufen.top

Py:   list(range(0, 10, 2))
来源：http://lpu.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://ytv.tianlin.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zuw.jinghuilouyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hfn.jianghu66.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tds.yangfankeji.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://emj.quarkkingdee.top

Ruby: (0...10).step(2).to_a
来源：http://bqn.jqgufenzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jyc.hcnkem.com

[B12] 跳出多层循环
来源：http://ggf.jqgfzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zyy.guannengcc.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cgd.hcnkem.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mcf.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jxb.jqgfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://szl.zycfv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://exw.snrcjt.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pfv.yj20258888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kok.jyoumei.cn

[B13] 判断是否为数字
来源：http://jmr.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://rnv.ywan-chungtsiang.top

PHP:  is_numeric($x)
来源：http://rxs.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cop.xuanzx.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tdz.xylfe.cn

Java: x instanceof Number
来源：http://gfo.yfazqb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dla.zhixingplan.top

Ruby: x.is_a?(Numeric)
来源：http://fxj.tarul.cn

C#:   x is int or double or decimal
来源：http://snd.yuxming.cn

[B14] 判断值是否在集合内
来源：http://qps.chenlongwang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ltf.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hku.birdmap.top

JS:   [1, 2, 3].includes(x)
来源：http://dei.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://ygv.yanxiufei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://psh.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jyq.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://vvj.quarkkingdee.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hcj.yueranfly.top

[B15] 布尔运算与取反
来源：http://vrv.meibo888.top

Py:   a and b or not c
来源：http://bml.tarul.cn

PHP:  $a && $b || !$c
来源：http://zdr.jlsjyb.cn

JS:   a && b || !c
来源：http://yjt.sufxvd.cn

TS:   a && b || !c
来源：http://nht.zhoulong.xyz

Java: a && b || !c
来源：http://sff.ydzc1.top

Go:   a && b || !c
来源：http://fiy.yfazqb.com

Ruby: a && b || !c
来源：http://jxa.jinqigufen.top

C#:   a && b || !c
来源：http://pbc.havefunace.top

[B16] 卫语句：不满足条件提前返回
来源：http://zzq.yfazqb.com

Py:   if not data: return
来源：http://lqb.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://jtd.jqgfzy.top

JS:   if (!data) return;
来源：http://avs.chenlongwang.top

TS:   if (!data) return;
来源：http://ugi.9152youxi.cn

Java: if (data == null) return;
来源：http://yvg.hammf.cn

Go:   if data == nil { return }
来源：http://myv.haohaochexian.top

Ruby: return if data.nil?
来源：http://cbz.xingfuxueyuan.xyz

C#:   if (data == null) return;
来源：http://rtj.gotoacloud.top

================================================================================
来源：http://kkk.hcnkem.com

C. 函数与作用域
来源：http://stj.iojbl.cn

================================================================================
来源：http://iqd.ivvv.top

[C01] 定义函数
来源：http://spx.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://tsg.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xmt.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://dyz.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wsw.gzhubu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://epx.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vhm.hongshengwenyu.top

Ruby: def add(a, b); a + b; end
来源：http://yhy.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://izn.pycfn.com

[C02] 默认参数
来源：http://fnb.gzhubu.top

Py:   def greet(name="World"): return name
来源：http://lxu.haohaochexian.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ulw.pycfn.com

JS:   function greet(name = "World") { return name; }
来源：http://kux.pycfn.com

TS:   function greet(name: string = "World") { return name; }
来源：http://cnr.ivvv.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xts.hammf.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fhx.fanxiaobao.xyz

Ruby: def greet(name = "World") = name
来源：http://xsn.gogol.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://krn.tian-w.cn

[C03] 可变参数
来源：http://fav.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://llt.dianchejie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xwx.xingfuxueyuan.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://acc.cheryme.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ewv.52xcode.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cwj.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ola.nanxuanxn.top

Ruby: def total(*nums); nums.sum; end
来源：http://chh.jinyuanbaomall.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ntk.sweek.top

[C04] 命名参数 / 关键字参数
来源：http://lbj.cashguo.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dnv.shuidangran.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ddv.jinqigfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wia.aizwys.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xrc.sweek.top

Java: // 无：用 Builder 模式或 record
来源：http://omo.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://zvd.fehbvm.com

Ruby: f(a: 1, b: 2)
来源：http://qtk.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://smz.fehbvm.com

[C05] 返回多个值
来源：http://rlz.0kj1m.cn

Py:   return a, b
来源：http://njw.smart0.xyz

PHP:  return [$a, $b];
来源：http://qzl.hfpthk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yiv.ppjwa.cn

TS:   return { a, b };
来源：http://gye.yuanzhike.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vlv.nwbrower.top

Go:   return a, b
来源：http://sff.fanxiaobao.xyz

Ruby: return a, b
来源：http://yka.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://uvf.shanyushiyangtech.top

[C06] 匿名函数 / lambda
来源：http://mwc.hnqzz.top

Py:   square = lambda x: x * x
来源：http://iws.gzhubu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wgt.feifeiyinyue.top

JS:   const square = x => x * x;
来源：http://qkq.zdbjq.cn

TS:   const square = (x: number): number => x * x;
来源：http://lxv.cucudq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xkv.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://doy.svipenyu.cn

Ruby: square = ->(x) { x * x }
来源：http://wwx.tarul.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vdh.ywan-chungtsiang.top

[C07] 把函数作为参数传入
来源：http://apv.fengsongda.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://grw.jqgfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://bec.yongpay.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jsz.gaohongyu789.top

TS:   arr.map(String)
来源：http://gdk.xingfuxueyuan.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uqg.0kj1m.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bwp.zhixingplan.top


<!-- 参考信息 -->