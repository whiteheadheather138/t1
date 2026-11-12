代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kkb.cucudq.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zeo.fktsv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ixe.yonumen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kod.yuanzhike.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://odm.pengpengdd.cyou

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rtz.cashguo.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lzn.hammf.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://anj.yuxming.cn

[A18] 字符与 ASCII 码互转
来源：http://ebc.yuanzhike.top

Py:   ord("A"); chr(65)
来源：http://mdd.jinqigufen.top

PHP:  ord("A"); chr(65)
来源：http://vim.shuidangran.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nic.nanxuanxn.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cjn.sxryk.cn

Java: (int) 'A'; (char) 65
来源：http://kgu.yfazqb.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ykh.bjfxy.top

Ruby: "A".ord; 65.chr
来源：http://udo.meibo888.top

C#:   (int)'A'; (char)65
来源：http://zbh.meibo888.top

[A19] 交换两个变量
来源：http://kpn.jqgfzy.top

Py:   a, b = b, a
来源：http://jpt.jiagoushi.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ibo.ppjwa.cn

JS:   [a, b] = [b, a];
来源：http://ghk.xinyue.icu

TS:   [a, b] = [b, a];
来源：http://xwl.snrcjt.cn

Java: int t = a; a = b; b = t;
来源：http://erk.mhx1999.top

Go:   a, b = b, a
来源：http://bzh.chenlongwang.top

Ruby: a, b = b, a
来源：http://osv.0kj1m.cn

C#:   (a, b) = (b, a);
来源：http://ccp.aibaodan.cn

[A20] 读取标准输入
来源：http://hew.uphjek.com

Py:   name = input("请输入：")
来源：http://qwt.wangdashe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rhn.sxryk.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ppb.shuidangran.top

TS:   // Node.js：readline 模块
来源：http://ahu.yj202588.top

Java: new Scanner(System.in).nextLine()
来源：http://stj.wangshuangyany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://thd.shanyushiyangkeji.top

Ruby: gets.chomp
来源：http://dby.mhx1999.top

C#:   Console.ReadLine();
来源：http://xhu.yj20258.top

[A21] 保留指定小数位输出
来源：http://unb.wangshuangyany.cn

Py:   f"{3.14159:.2f}"
来源：http://vkf.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dol.snrcjt.cn

JS:   (3.14159).toFixed(2)
来源：http://ejq.zhongyouzk.top

TS:   (3.14159).toFixed(2)
来源：http://jro.cashguo.top

Java: String.format("%.2f", 3.14159)
来源：http://evi.sufxvd.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ogr.chenlongwang.top

Ruby: format("%.2f", 3.14159)
来源：http://jmp.guannengcc.top

C#:   3.14159.ToString("F2")
来源：http://bmk.sufxvd.cn

[A22] 获取字符串长度
来源：http://tur.52xcode.cn

Py:   len(s)
来源：http://ozz.ehwqpu.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qxj.redwolf501.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vvo.xziqi.cn

TS:   s.length
来源：http://gpw.ivvv.top

Java: s.length()
来源：http://rvn.jqgufenzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pfn.jiagoushi.top

Ruby: s.length
来源：http://fqt.hysaishi.cn

C#:   s.Length
来源：http://gjz.dashuyun.cn

[A23] 大小写转换
来源：http://cqe.nanxinkj.top

Py:   s.upper(); s.lower(); s.title()
来源：http://jbk.chenlongwang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ydc.andypj.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fte.haohaochexian.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://msv.havefunace.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ahq.vqdsnc.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ckq.hammf.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ptz.gaohongyu789.top

C#:   s.ToUpper(); s.ToLower()
来源：http://jfq.sweek.top

[A24] 去除首尾空白
来源：http://lxd.ydjk.org.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fqz.shangyingyoupin.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wdo.hnxiangtu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hyk.jqgfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://doz.uphjek.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mbv.9152youxi.cn

Go:   strings.TrimSpace(s)
来源：http://zgv.hesvh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wfs.316326.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tdc.aizwys.cn

[A25] 字符串比较
来源：http://bfz.daxiang520.top

Py:   s1 == s2; s1 != s2
来源：http://anh.shangyingyoupin.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tdl.tian-w.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jfl.xuetiantiany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zou.snrcjt.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ozg.zhiwuduotai.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qwb.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fab.mhx1999.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xct.zhiwuduotai.top

[A26] 类型转换总览
来源：http://yjy.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yij.hnxiangtu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fkk.guannengcc.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qfz.yueranfly.top

TS:   Number() String() Boolean() x as number
来源：http://fze.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ybf.nanxuanxn.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ipj.dianchejie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jng.316326.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ktx.sysykeji.top

================================================================================
来源：http://jtk.yj20258.top

B. 流程控制
来源：http://fqp.ywan-chungtsiang.top

================================================================================
来源：http://uwz.kuanghao11.cn

[B01] 条件判断 if / else
来源：http://aiz.zdbjq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ocg.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ijw.52xcode.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oqj.smart0.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://akj.hongshengwenyu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cpw.52xcode.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zvv.ctjpmb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pnj.aizwys.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fbu.cashguo.top

[B02] 多分支 else if / elif
来源：http://lkr.guannengcc.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cmi.iojbl.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sfe.ywan-chungtsiang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://byu.chenjidiqi.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wqy.yanxiufei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iul.sweek.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tuo.shangyingyoupin.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fcw.shuidangran.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dvs.aibaodan.cn

[B03] switch / match / case
来源：http://amd.cqqwz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kti.cheryme.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xkd.kuanghao11.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mnt.chenlongwang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dob.gaohongyu789.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jmc.xinyue.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tlk.svipenyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tww.yvedp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fzo.tian-w.cn

[B04] for 计数循环
来源：http://nhd.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://igw.tian-w.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mip.jinqigfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zwz.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://psq.mhx1999.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rws.yfazqb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hyb.bbcook.cn

Ruby: 10.times { |i| puts i }
来源：http://tjc.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://omy.0kj1m.cn

[B05] 遍历数组 / 列表
来源：http://aly.yangfankeji.com

Py:   for item in arr: print(item)
来源：http://vmu.hnqzz.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xbg.redwolf501.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ogp.9152youxi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dkx.zycfv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ams.nwbrower.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kjm.zhijiandao.cn

Ruby: arr.each { |item| puts item }
来源：http://fhd.jinyuanbaomall.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lkb.fehbvm.com

[B06] 遍历字典 / 对象
来源：http://tkl.chenjidiqi.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://ebh.jinqigufen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hyg.iojbl.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nav.zhixingplan.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://llr.chenzaomai.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ikk.aibaodan.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rby.havefunace.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eku.yj20258.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jxh.wangdashe.top

[B07] while 循环
来源：http://yjw.daxiang520.top

Py:   while i < 10: i += 1
来源：http://ljg.zycfv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cai.sjlbkw.cn

JS:   while (i < 10) { i++; }
来源：http://djl.cqqwz.cn

TS:   while (i < 10) { i++; }
来源：http://lqd.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://alt.hywenlv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zss.zhoulong.xyz

Ruby: while i < 10; i += 1; end
来源：http://hfp.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://jax.ivvv.top

[B08] do-while（至少执行一次）
来源：http://kxn.gaohongyu789.top

Py:   # 无 do-while：用 while True + break
来源：http://vju.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rkw.vehdjk.com

JS:   do { i++; } while (i < 10);
来源：http://cff.jinghuilouyu.cn

TS:   do { i++; } while (i < 10);
来源：http://bmu.ppjwa.cn

Java: do { i++; } while (i < 10);
来源：http://gtd.kuanghao11.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jzk.yvedp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://atr.epnwcf.com

C#:   do { i++; } while (i < 10);
来源：http://mjz.tian-w.cn

[B09] break 与 continue
来源：http://fkz.hfpthk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iib.jianghu66.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fwo.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kie.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ism.chenjidiqi.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://khx.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://inn.cashguo.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jtx.havefunace.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zjn.haohaochexian.top

[B10] 遍历同时拿索引
来源：http://prk.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bfc.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zwv.guowangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lct.jianghu66.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ukp.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xxh.yonumen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ulz.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bbc.tianlin.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mrl.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://uwp.ybcxt.top

Py:   list(range(0, 10, 2))
来源：http://mzn.svipenyu.cn

PHP:  range(0, 10, 2);
来源：http://glw.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ffz.mhx1999.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nel.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pya.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ejd.hnxiangtu.top

Ruby: (0...10).step(2).to_a
来源：http://hdx.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qyd.yfazqb.com

[B12] 跳出多层循环
来源：http://cwq.hammf.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hat.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://fft.gzhubu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wvi.chenzaomai.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ioi.xziqi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cmb.yfazqb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tsw.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://txv.yueranfly.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vxx.guannengcc.top

[B13] 判断是否为数字
来源：http://kxi.aibaodan.cn

Py:   isinstance(x, (int, float))
来源：http://qoy.havefunace.top

PHP:  is_numeric($x)
来源：http://npf.cashguo.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vhu.hywenlv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://slg.cheryme.top

Java: x instanceof Number
来源：http://lis.ybcxt.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ejt.havefunace.top

Ruby: x.is_a?(Numeric)
来源：http://fkt.guowangkeji.top

C#:   x is int or double or decimal
来源：http://zne.dashuyun.cn

[B14] 判断值是否在集合内
来源：http://yql.chenjidiqi.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ivz.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://own.cucudq.cn

JS:   [1, 2, 3].includes(x)
来源：http://kmh.ppjwa.cn

TS:   [1, 2, 3].includes(x)
来源：http://pye.meibo888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://phx.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dqx.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://clq.dianchejie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dvs.guowangkeji.top

[B15] 布尔运算与取反
来源：http://rre.jlsjyb.cn

Py:   a and b or not c
来源：http://yym.52xcode.cn

PHP:  $a && $b || !$c
来源：http://qhu.quarkkingdee.top

JS:   a && b || !c
来源：http://reb.zdqjudy.top

TS:   a && b || !c
来源：http://tkn.ydjk.org.cn

Java: a && b || !c
来源：http://fcc.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://gga.hnqzz.top

Ruby: a && b || !c
来源：http://lai.dashuyun.cn

C#:   a && b || !c
来源：http://cvy.ywan-chungtsiang.top

[B16] 卫语句：不满足条件提前返回
来源：http://gaq.xuetiantiany.cn

Py:   if not data: return
来源：http://omv.xylfe.cn

PHP:  if (!$data) { return; }
来源：http://qav.fzhhl.top

JS:   if (!data) return;
来源：http://iye.gogol.net.cn

TS:   if (!data) return;
来源：http://cbl.yfazqb.com

Java: if (data == null) return;
来源：http://ura.jlsjyb.cn

Go:   if data == nil { return }
来源：http://xxd.snrcjt.cn

Ruby: return if data.nil?
来源：http://vkb.gzhubu.top

C#:   if (data == null) return;
来源：http://tzm.cucudq.cn

================================================================================
来源：http://mmq.havefunace.top

C. 函数与作用域
来源：http://pmx.ydjk.org.cn

================================================================================
来源：http://bga.hesvh.cn

[C01] 定义函数
来源：http://kko.sweek.top

Py:   def add(a, b): return a + b
来源：http://mqz.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ips.cucudq.cn

JS:   function add(a, b) { return a + b; }
来源：http://ylu.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fir.guannengcc.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qxv.zhengqikj.top

Go:   func add(a, b int) int { return a + b }
来源：http://wuq.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://goa.zhengqikj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://axo.ctjpmb.com

[C02] 默认参数
来源：http://pvc.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://khs.52xcode.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qfr.ctjpmb.com

JS:   function greet(name = "World") { return name; }
来源：http://hkx.fktsv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wix.daria6918.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://siy.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lax.sweek.top

Ruby: def greet(name = "World") = name
来源：http://toq.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://uxt.kuanghao11.cn

[C03] 可变参数
来源：http://ncf.jiagoushi.top

Py:   def total(*args): return sum(args)
来源：http://pgm.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fnl.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ttv.aibaodan.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xri.ydzc1.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qgr.zdqjudy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qec.zdqjudy.top

Ruby: def total(*nums); nums.sum; end
来源：http://hst.uphjek.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bak.shangyingyoupin.top

[C04] 命名参数 / 关键字参数
来源：http://dvy.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kba.hcnkem.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yny.chenjidiqi.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://apc.gaohongyu789.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wak.jiagoushi.top

Java: // 无：用 Builder 模式或 record
来源：http://umr.jinghuilouyu.cn

Go:   // 无：用配置结构体参数
来源：http://dvt.tian-w.cn

Ruby: f(a: 1, b: 2)
来源：http://pje.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://qzf.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://zqw.cucudq.cn

Py:   return a, b
来源：http://vaj.havefunace.top

PHP:  return [$a, $b];
来源：http://rvx.ctjpmb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://yfo.sweek.top

TS:   return { a, b };
来源：http://ekc.snrcjt.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gnx.hongshengwenyu.top

Go:   return a, b
来源：http://vnd.jinqigfzy.top

Ruby: return a, b
来源：http://mxj.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://kxg.chenzaomai.com

[C06] 匿名函数 / lambda
来源：http://jom.sysykeji.top

Py:   square = lambda x: x * x
来源：http://xdm.chenjidiqi.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://mup.chenzaomai.com

JS:   const square = x => x * x;
来源：http://nyr.smart0.xyz

TS:   const square = (x: number): number => x * x;
来源：http://mqc.guannengcc.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jpy.yanxiufei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://urg.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://ykd.chenlongwang.top

C#:   Func<int, int> square = x => x * x;
来源：http://ncs.nanxinkj.top

[C07] 把函数作为参数传入
来源：http://gyk.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kvm.ywan-chungtsiang.top

PHP:  array_map("strtoupper", $arr);
来源：http://vdv.cdnleiting.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tzq.hammf.cn

TS:   arr.map(String)
来源：http://uzr.hysaishi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mnw.fktsv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eok.fehbvm.com


<!-- 参考信息 -->