代发 wailian999

Ruby: value = data || "默认值"
来源：http://wdw.iojbl.cn

C#:   var value = data ?? "默认值";
来源：http://uup.guannengcc.top

[A16] 真假值判断规则
来源：http://tyy.gotoacloud.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://isk.cqqwz.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ejx.jianghu66.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vpo.aizwys.cn

TS:   if (!x) {}
来源：http://cfo.daxiang520.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yzt.shzxlz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mgu.52xcode.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vaw.xinyue.icu

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mac.tian-w.cn

[A17] 位运算
来源：http://aqg.daria6918.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eiw.nanxinkj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kir.pycfn.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wkx.tianlin.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hah.wangshuangyany.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fsg.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://une.hysaishi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kyd.fktsv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sjb.52xcode.cn

[A18] 字符与 ASCII 码互转
来源：http://tty.jinyuanbaomall.cn

Py:   ord("A"); chr(65)
来源：http://qou.zhiwuduotai.top

PHP:  ord("A"); chr(65)
来源：http://tae.zhaomingkeji.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://glv.zdbjq.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cfy.yj202588.top

Java: (int) 'A'; (char) 65
来源：http://srp.svipenyu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jpf.hammf.cn

Ruby: "A".ord; 65.chr
来源：http://eqg.pengpengdd.cyou

C#:   (int)'A'; (char)65
来源：http://nyv.yj20258.top

[A19] 交换两个变量
来源：http://ant.hesvh.cn

Py:   a, b = b, a
来源：http://psv.shuidangran.top

PHP:  [$a, $b] = [$b, $a];
来源：http://uea.dianchejie.cn

JS:   [a, b] = [b, a];
来源：http://fqi.zhijiandao.cn

TS:   [a, b] = [b, a];
来源：http://rjw.vqdsnc.cn

Java: int t = a; a = b; b = t;
来源：http://thh.hywenlv.cn

Go:   a, b = b, a
来源：http://zzi.jyoumei.cn

Ruby: a, b = b, a
来源：http://rwn.quarkkingdee.top

C#:   (a, b) = (b, a);
来源：http://nlj.yonumen.top

[A20] 读取标准输入
来源：http://jeg.dianchejie.cn

Py:   name = input("请输入：")
来源：http://iie.nanxuanxn.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kml.yongpay.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bov.zhaomingkeji.xyz

TS:   // Node.js：readline 模块
来源：http://rlk.vehdjk.com

Java: new Scanner(System.in).nextLine()
来源：http://cve.fktsv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nkm.havefunace.top

Ruby: gets.chomp
来源：http://xsu.pycfn.com

C#:   Console.ReadLine();
来源：http://gcm.tianlin.xyz

[A21] 保留指定小数位输出
来源：http://inr.jyoumei.cn

Py:   f"{3.14159:.2f}"
来源：http://jub.shangyingyoupin.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xec.daxiang520.top

JS:   (3.14159).toFixed(2)
来源：http://tiw.snrcjt.cn

TS:   (3.14159).toFixed(2)
来源：http://yje.yongpay.top

Java: String.format("%.2f", 3.14159)
来源：http://xpn.redwolf501.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hau.fehbvm.com

Ruby: format("%.2f", 3.14159)
来源：http://dei.jinghuilouyu.cn

C#:   3.14159.ToString("F2")
来源：http://npy.ivvv.top

[A22] 获取字符串长度
来源：http://wuu.zhongyouzk.top

Py:   len(s)
来源：http://lan.quarkkingdee.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tdn.meibo888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wcp.hcnkem.com

TS:   s.length
来源：http://uzv.gaohongyu789.top

Java: s.length()
来源：http://pkd.tanke756.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hux.zhengqikj.top

Ruby: s.length
来源：http://lry.uphjek.com

C#:   s.Length
来源：http://lwn.yj20258.top

[A23] 大小写转换
来源：http://zax.pycfn.com

Py:   s.upper(); s.lower(); s.title()
来源：http://zlt.sufxvd.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kgv.pengpengdd.cyou

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cfp.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vpw.jqgufenzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xur.c1oappe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mrx.sufxvd.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jho.gaohongyu789.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qip.yvedp.cn

[A24] 去除首尾空白
来源：http://nbl.tianlin.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kvd.svipenyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sgh.sjlbkw.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mkr.sxryk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ond.chenlongwang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://krl.daria6918.cn

Go:   strings.TrimSpace(s)
来源：http://gbn.shanyushiyangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ayt.jinghuilouyu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zie.havefunace.top

[A25] 字符串比较
来源：http://geo.guannengcc.top

Py:   s1 == s2; s1 != s2
来源：http://izi.hnqzz.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ytu.shanyushiyangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nua.shzxlz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://syu.xingfuxueyuan.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fnj.ydzc1.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qqc.hywenlv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://usf.pengpengdd.cyou

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jpz.jinqigfzy.top

[A26] 类型转换总览
来源：http://jxk.jinqigufen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dab.316326.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ixz.jlsjyb.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zug.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://sac.nanxinkj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tjx.daxiang520.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://trc.vqdsnc.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fyf.jyoumei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gho.9152youxi.cn

================================================================================
来源：http://pnh.jqgfzy.top

B. 流程控制
来源：http://ukq.gogol.net.cn

================================================================================
来源：http://wjv.snrcjt.cn

[B01] 条件判断 if / else
来源：http://jln.ywan-chungtsiang.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hny.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://don.jianghu66.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xke.dianchejie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dsl.smart0.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://qmf.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ulc.shangyingyoupin.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vnx.hysaishi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://shx.andypj.xyz

[B02] 多分支 else if / elif
来源：http://qmn.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ipf.sysykeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dzp.ehwqpu.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ubf.pycfn.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ilr.mhx1999.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://myo.gzhubu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zye.zhoulong.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ldk.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qcq.hnqzz.top

[B03] switch / match / case
来源：http://gfz.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bug.9152youxi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oqx.jianghu66.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://clm.jiagoushi.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xkn.jinqigufen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sgo.vqdsnc.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jlq.zdbjq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://juw.jqgufenzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wph.nanxuanxn.top

[B04] for 计数循环
来源：http://dps.mhx1999.top

Py:   for i in range(10): print(i)
来源：http://whl.jinyuanbaomall.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wli.cheryme.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ofq.gaohongyu789.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fqx.aizwys.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tgt.xziqi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tkt.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://oye.sjlbkw.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jqv.jinghuilouyu.cn

[B05] 遍历数组 / 列表
来源：http://lce.zhengqikj.top

Py:   for item in arr: print(item)
来源：http://exk.jqgufenzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dzz.yfazqb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://xri.jqgfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dtl.sweek.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wlr.cheryme.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ebc.c1oappe.top

Ruby: arr.each { |item| puts item }
来源：http://sal.ybcxt.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://doq.yj20258.top

[B06] 遍历字典 / 对象
来源：http://rtl.ctjpmb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://czb.yj202588.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jqu.hammf.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tib.9152youxi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ktd.guowangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://czg.hongshengwenyu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kvi.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cjr.hfpthk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mau.ivvv.top

[B07] while 循环
来源：http://ddk.feifeiyinyue.top

Py:   while i < 10: i += 1
来源：http://avs.redwolf501.top

PHP:  while ($i < 10) { $i++; }
来源：http://ltz.daxiang520.top

JS:   while (i < 10) { i++; }
来源：http://jhk.xuetiantiany.cn

TS:   while (i < 10) { i++; }
来源：http://oma.yangfankeji.com

Java: while (i < 10) { i++; }
来源：http://vej.tanke756.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://exv.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://edu.shanyushiyangkeji.top

C#:   while (i < 10) { i++; }
来源：http://ysd.jinqigufen.top

[B08] do-while（至少执行一次）
来源：http://vuf.shanyushiyangtech.top

Py:   # 无 do-while：用 while True + break
来源：http://kuk.havefunace.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ced.tianlin.xyz

JS:   do { i++; } while (i < 10);
来源：http://gfl.hnxiangtu.top

TS:   do { i++; } while (i < 10);
来源：http://uyp.jlsjyb.cn

Java: do { i++; } while (i < 10);
来源：http://cxa.gzhubu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ezr.pycfn.com

Ruby: begin; i += 1; end while i < 10
来源：http://gxo.cucudq.cn

C#:   do { i++; } while (i < 10);
来源：http://bki.dashuyun.cn

[B09] break 与 continue
来源：http://hrf.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dch.tanke756.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://opk.yonumen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rfk.aizwys.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://niv.bbcook.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xkh.cheryme.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wak.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nth.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mpo.vqdsnc.cn

[B10] 遍历同时拿索引
来源：http://hxb.yfazqb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gpf.dashuyun.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nvh.fzhhl.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tel.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://upf.ctjpmb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://spp.gotoacloud.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://flx.zhengqikj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gcs.52xcode.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://drz.ehwqpu.com

[B11] 生成数字序列 / 区间
来源：http://adp.hammf.cn

Py:   list(range(0, 10, 2))
来源：http://adi.ppjwa.cn

PHP:  range(0, 10, 2);
来源：http://ebw.zhijiandao.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://txe.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ble.yonumen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aei.zhoulong.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hkt.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://exq.nwbrower.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mdj.zhengqikj.top

[B12] 跳出多层循环
来源：http://qab.tian-w.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fau.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://kij.hnxiangtu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fni.jinghuilouyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nhq.vqdsnc.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jbc.guowangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gnw.jinyuanbaomall.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tbb.zycfv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xjn.mhx1999.top

[B13] 判断是否为数字
来源：http://niu.tian-w.cn

Py:   isinstance(x, (int, float))
来源：http://pnp.yj202588.top

PHP:  is_numeric($x)
来源：http://kwf.zycfv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dhu.xingfuxueyuan.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hqm.snrcjt.cn

Java: x instanceof Number
来源：http://veg.yj20258.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mda.zhongyouzk.top

Ruby: x.is_a?(Numeric)
来源：http://aod.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://xsb.hnxiangtu.top

[B14] 判断值是否在集合内
来源：http://ido.hammf.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ljg.bbcook.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bha.c1oappe.top

JS:   [1, 2, 3].includes(x)
来源：http://ids.andypj.xyz

TS:   [1, 2, 3].includes(x)
来源：http://agm.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://oqf.havefunace.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zqs.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://pgc.hongshengwenyu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fnn.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://hxf.jqgfzy.top

Py:   a and b or not c
来源：http://jmn.aizwys.cn

PHP:  $a && $b || !$c
来源：http://lcw.yuxming.cn

JS:   a && b || !c
来源：http://rfs.sysykeji.top

TS:   a && b || !c
来源：http://ccc.gotoacloud.top

Java: a && b || !c
来源：http://van.bbcook.cn

Go:   a && b || !c
来源：http://qyu.ppjwa.cn

Ruby: a && b || !c
来源：http://otf.havefunace.top

C#:   a && b || !c
来源：http://kzl.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rky.jinqigufen.top

Py:   if not data: return
来源：http://vdi.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://thk.smart0.xyz

JS:   if (!data) return;
来源：http://fro.meibo888.top

TS:   if (!data) return;
来源：http://nxu.ctjpmb.com

Java: if (data == null) return;
来源：http://rnj.nanxuanxn.top

Go:   if data == nil { return }
来源：http://jps.zhijiandao.cn

Ruby: return if data.nil?
来源：http://mvi.iojbl.cn

C#:   if (data == null) return;
来源：http://jmj.uphjek.com

================================================================================
来源：http://kef.shuidangran.top

C. 函数与作用域
来源：http://aue.gaohongyu789.top

================================================================================
来源：http://zys.hywenlv.cn

[C01] 定义函数
来源：http://nue.jianghu66.top

Py:   def add(a, b): return a + b
来源：http://nnn.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://axe.gotoacloud.top

JS:   function add(a, b) { return a + b; }
来源：http://jbn.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://prs.cqqwz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xuy.gogol.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jmn.ydjk.org.cn

Ruby: def add(a, b); a + b; end
来源：http://mlh.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://arm.jinghuilouyu.cn

[C02] 默认参数
来源：http://qux.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://vln.hywenlv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://asa.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://lsp.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kmc.cashguo.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ulm.nanxuanxn.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://url.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://oyh.yuanzhike.top

C#:   string Greet(string name = "World") => name;
来源：http://puq.hnxiangtu.top

[C03] 可变参数
来源：http://ovc.xinyue.icu

Py:   def total(*args): return sum(args)
来源：http://nhh.snrcjt.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pum.zhoulong.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qrh.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://loy.cucudq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sdw.ywan-chungtsiang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pxw.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://uvw.shzxlz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hmv.aibaodan.cn

[C04] 命名参数 / 关键字参数
来源：http://gsd.kuanghao11.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hkh.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tnq.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kqw.jyoumei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kqc.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://flj.hnxiangtu.top

Go:   // 无：用配置结构体参数
来源：http://jvc.jinqigfzy.top

Ruby: f(a: 1, b: 2)
来源：http://gvb.c1oappe.top

C#:   f(a: 1, b: 2)
来源：http://meg.jiagoushi.top

[C05] 返回多个值
来源：http://tcz.smart0.xyz

Py:   return a, b
来源：http://aag.yangfankeji.com

PHP:  return [$a, $b];
来源：http://ntg.hnxiangtu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zau.yuanzhike.top

TS:   return { a, b };
来源：http://tex.zdbjq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://itv.aizwys.cn

Go:   return a, b
来源：http://bpg.ppjwa.cn

Ruby: return a, b
来源：http://axh.jiagoushi.top

C#:   return (a, b);              // ValueTuple
来源：http://kuq.nanxuanxn.top

[C06] 匿名函数 / lambda
来源：http://nry.aizwys.cn

Py:   square = lambda x: x * x
来源：http://ywm.jinqigfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hgd.cheryme.top

JS:   const square = x => x * x;
来源：http://lar.yj20258888.top


<!-- 参考信息 -->