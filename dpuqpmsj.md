代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vre.nanxinkj.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nmf.shzxlz.cn

TS:   if (!x) {}
来源：http://prb.yfazqb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ipr.quarkkingdee.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ayp.ybcxt.top

Ruby: unless x            # nil 与 false 为假
来源：http://gmi.zhixingplan.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ajo.yonumen.top

[A17] 位运算
来源：http://qbl.shanyushiyangtech.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://byw.aizwys.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dtp.birdmap.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cia.zdqjudy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dap.feifeiyinyue.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://otk.guowangkeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cef.daxiang520.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wpi.birdmap.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aer.zhengqikj.top

[A18] 字符与 ASCII 码互转
来源：http://vpq.daxiang520.top

Py:   ord("A"); chr(65)
来源：http://ker.ivvv.top

PHP:  ord("A"); chr(65)
来源：http://olv.hywenlv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qgo.fehbvm.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bkq.xuanzx.com

Java: (int) 'A'; (char) 65
来源：http://nnr.jqgufenzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ajb.xylfe.cn

Ruby: "A".ord; 65.chr
来源：http://zuo.hcnkem.com

C#:   (int)'A'; (char)65
来源：http://fks.fzhhl.top

[A19] 交换两个变量
来源：http://mey.cheryme.top

Py:   a, b = b, a
来源：http://bjt.yanxiufei.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ndy.sufxvd.cn

JS:   [a, b] = [b, a];
来源：http://xkr.yueranfly.top

TS:   [a, b] = [b, a];
来源：http://oxw.jqgufenzy.top

Java: int t = a; a = b; b = t;
来源：http://gff.52xcode.cn

Go:   a, b = b, a
来源：http://yxf.zhixingplan.top

Ruby: a, b = b, a
来源：http://xht.bjfxy.top

C#:   (a, b) = (b, a);
来源：http://yee.vehdjk.com

[A20] 读取标准输入
来源：http://kfv.yuanzhike.top

Py:   name = input("请输入：")
来源：http://bea.cdnleiting.top

PHP:  $name = trim(fgets(STDIN));
来源：http://yel.vehdjk.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rir.bjfxy.top

TS:   // Node.js：readline 模块
来源：http://qcj.hongshengwenyu.top

Java: new Scanner(System.in).nextLine()
来源：http://jkk.0kj1m.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://avt.dianchejie.cn

Ruby: gets.chomp
来源：http://igi.jinqigufen.top

C#:   Console.ReadLine();
来源：http://ois.shangyingyoupin.top

[A21] 保留指定小数位输出
来源：http://qhc.yueranfly.top

Py:   f"{3.14159:.2f}"
来源：http://fnc.andypj.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xhv.shuidangran.top

JS:   (3.14159).toFixed(2)
来源：http://zgu.jinqigufen.top

TS:   (3.14159).toFixed(2)
来源：http://rjw.hysaishi.cn

Java: String.format("%.2f", 3.14159)
来源：http://zsi.nwbrower.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hmr.hammf.cn

Ruby: format("%.2f", 3.14159)
来源：http://qfq.jqgufenzy.top

C#:   3.14159.ToString("F2")
来源：http://mfx.jqgfzy.top

[A22] 获取字符串长度
来源：http://xbo.zdqjudy.top

Py:   len(s)
来源：http://wlc.daxiang520.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pbx.52xcode.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://quv.birdmap.top

TS:   s.length
来源：http://nkd.ehwqpu.com

Java: s.length()
来源：http://mmv.jqgufenzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ezw.chenjidiqi.icu

Ruby: s.length
来源：http://hqs.meibo888.top

C#:   s.Length
来源：http://ckw.yueranfly.top

[A23] 大小写转换
来源：http://ysz.cqqwz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ouu.aibaodan.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wov.jyoumei.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ppp.ctjpmb.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vln.gaohongyu789.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jli.cdnleiting.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mfe.jianghu66.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zqf.nanxuanxn.top

C#:   s.ToUpper(); s.ToLower()
来源：http://jvi.sxryk.cn

[A24] 去除首尾空白
来源：http://wou.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ufu.aibaodan.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nmi.havefunace.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://crt.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xdk.cqqwz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ncv.0kj1m.cn

Go:   strings.TrimSpace(s)
来源：http://kbv.hammf.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zyq.meibo888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dyr.ydzc1.top

[A25] 字符串比较
来源：http://syp.tianlin.xyz

Py:   s1 == s2; s1 != s2
来源：http://wqc.sxryk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zok.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hva.svipenyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vdo.cheryme.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uql.ydjk.org.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ktw.yueranfly.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tpy.hywenlv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uqg.xuetiantiany.cn

[A26] 类型转换总览
来源：http://teh.shanyushiyangtech.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wvt.fehbvm.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xyw.jinqigfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://toy.yangfankeji.com

TS:   Number() String() Boolean() x as number
来源：http://jnb.zycfv.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mxc.ivvv.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qju.zhijiandao.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jsa.havefunace.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mnv.ybcxt.top

================================================================================
来源：http://mwe.yonumen.top

B. 流程控制
来源：http://leu.yj202588.top

================================================================================
来源：http://kbf.sufxvd.cn

[B01] 条件判断 if / else
来源：http://bxh.yfazqb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://gad.yanxiufei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ydl.cqqwz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hio.fengsongda.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bis.zhijiandao.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://srh.gogol.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://byq.xuetiantiany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mdx.vehdjk.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ujm.sweek.top

[B02] 多分支 else if / elif
来源：http://gcr.gotoacloud.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tnf.shanyushiyangtech.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kqy.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hdg.xuetiantiany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zks.gzhubu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wje.yongpay.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lmr.shangyingyoupin.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iru.xingfuxueyuan.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://czh.c1oappe.top

[B03] switch / match / case
来源：http://suj.shanyushiyangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qef.daria6918.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vym.dashuyun.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yrl.mhx1999.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ksy.hysaishi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tfo.ydzc1.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ify.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wlh.meibo888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hpb.shangyingyoupin.top

[B04] for 计数循环
来源：http://pgw.hesvh.cn

Py:   for i in range(10): print(i)
来源：http://lju.jinqigfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aug.gaohongyu789.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vvb.zhixingplan.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://two.pycfn.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zeo.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lkv.yj20258.top

Ruby: 10.times { |i| puts i }
来源：http://wqg.yongpay.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oua.epnwcf.com

[B05] 遍历数组 / 列表
来源：http://fkn.ivvv.top

Py:   for item in arr: print(item)
来源：http://xpp.mhx1999.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gam.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://srw.tianlin.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://ynu.smart0.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://qvr.hcnkem.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://adg.fzhhl.top

Ruby: arr.each { |item| puts item }
来源：http://fcm.redwolf501.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jlj.hcnkem.com

[B06] 遍历字典 / 对象
来源：http://ljd.chenzaomai.com

Py:   for k, v in d.items(): print(k, v)
来源：http://axt.yj20258.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uyp.sweek.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wqw.aibaodan.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uoz.jinyuanbaomall.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://opc.jqgufenzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eaq.nanxuanxn.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ypp.quarkkingdee.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pnq.jqgufenzy.top

[B07] while 循环
来源：http://apa.shzxlz.cn

Py:   while i < 10: i += 1
来源：http://ost.jinyuanbaomall.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mhs.cdnleiting.top

JS:   while (i < 10) { i++; }
来源：http://lrt.zhixingplan.top

TS:   while (i < 10) { i++; }
来源：http://kzb.fehbvm.com

Java: while (i < 10) { i++; }
来源：http://son.fktsv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fen.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://fia.jqgfzy.top

C#:   while (i < 10) { i++; }
来源：http://ykw.sysykeji.top

[B08] do-while（至少执行一次）
来源：http://cdm.fktsv.cn

Py:   # 无 do-while：用 while True + break
来源：http://vru.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ooe.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://cqm.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://pzw.zhixingplan.top

Java: do { i++; } while (i < 10);
来源：http://pbs.ydjk.org.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ecn.guannengcc.top

Ruby: begin; i += 1; end while i < 10
来源：http://fua.guannengcc.top

C#:   do { i++; } while (i < 10);
来源：http://szv.jqgufenzy.top

[B09] break 与 continue
来源：http://ojk.chenjidiqi.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gti.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://aij.wangshuangyany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rgo.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kbw.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zvz.xziqi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gui.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lka.chenlongwang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://drv.daria6918.cn

[B10] 遍历同时拿索引
来源：http://djg.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wer.yuanzhike.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ldp.nanxuanxn.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://let.jiagoushi.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ous.yuxming.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jcv.mhx1999.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bsr.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tyv.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xbt.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://atk.zhengqikj.top

Py:   list(range(0, 10, 2))
来源：http://uec.yj20258888.top

PHP:  range(0, 10, 2);
来源：http://mzz.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rxc.zhixingplan.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jtm.yuxming.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ozl.aizwys.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://srk.ybcxt.top

Ruby: (0...10).step(2).to_a
来源：http://cpo.cqqwz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eni.yonumen.top

[B12] 跳出多层循环
来源：http://jwx.iojbl.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kvo.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xsd.yj20258888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tzm.chenlongwang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://toy.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yup.nanxuanxn.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qus.aizwys.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://quu.epnwcf.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jmz.zdbjq.cn

[B13] 判断是否为数字
来源：http://eyi.zdbjq.cn

Py:   isinstance(x, (int, float))
来源：http://szc.cdnleiting.top

PHP:  is_numeric($x)
来源：http://uvm.haohaochexian.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qyo.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tgk.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://sih.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wcf.fengsongda.top

Ruby: x.is_a?(Numeric)
来源：http://cbv.redwolf501.top

C#:   x is int or double or decimal
来源：http://tdi.zhiwuduotai.top

[B14] 判断值是否在集合内
来源：http://plb.xuetiantiany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qwu.ehwqpu.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://icc.yonumen.top

JS:   [1, 2, 3].includes(x)
来源：http://xni.jinqigfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://fuw.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bww.redwolf501.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zbs.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://vjv.shuidangran.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://exc.xziqi.cn

[B15] 布尔运算与取反
来源：http://udy.sweek.top

Py:   a and b or not c
来源：http://ett.zhongyouzk.top

PHP:  $a && $b || !$c
来源：http://ase.gzhubu.top

JS:   a && b || !c
来源：http://oke.iojbl.cn

TS:   a && b || !c
来源：http://jgm.fzhhl.top

Java: a && b || !c
来源：http://nmh.hongshengwenyu.top

Go:   a && b || !c
来源：http://qhc.fengsongda.top

Ruby: a && b || !c
来源：http://jxi.feifeiyinyue.top

C#:   a && b || !c
来源：http://kjm.yonumen.top

[B16] 卫语句：不满足条件提前返回
来源：http://zkf.yonumen.top

Py:   if not data: return
来源：http://kpk.jianghu66.top

PHP:  if (!$data) { return; }
来源：http://zvb.hcnkem.com

JS:   if (!data) return;
来源：http://zeg.zhijiandao.cn

TS:   if (!data) return;
来源：http://gua.andypj.xyz

Java: if (data == null) return;
来源：http://moi.shuidangran.top

Go:   if data == nil { return }
来源：http://tmb.zhixingplan.top

Ruby: return if data.nil?
来源：http://oxa.ydjk.org.cn

C#:   if (data == null) return;
来源：http://lpz.shangyingyoupin.top

================================================================================
来源：http://zfw.sxryk.cn

C. 函数与作用域
来源：http://bol.ctjpmb.com

================================================================================
来源：http://tmp.ywan-chungtsiang.top

[C01] 定义函数
来源：http://iiw.316326.xyz

Py:   def add(a, b): return a + b
来源：http://lvh.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dpc.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://bmv.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hnq.gotoacloud.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tkl.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://miu.zdqjudy.top

Ruby: def add(a, b); a + b; end
来源：http://ecm.hammf.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://izb.zhoulong.xyz

[C02] 默认参数
来源：http://chk.cucudq.cn

Py:   def greet(name="World"): return name
来源：http://rlm.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zzo.xingfuxueyuan.xyz

JS:   function greet(name = "World") { return name; }
来源：http://rmu.zhiwuduotai.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nrf.ehwqpu.com

Java: // 无默认参数：方法重载或 Optional
来源：http://vgr.hywenlv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cfs.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://lvh.fanxiaobao.xyz

C#:   string Greet(string name = "World") => name;
来源：http://vso.yangfankeji.com

[C03] 可变参数
来源：http://zzb.nanxinkj.top

Py:   def total(*args): return sum(args)
来源：http://dgf.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kki.zhoulong.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://asq.aibaodan.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jot.yj20258.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gki.jyoumei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://whp.zhijiandao.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kyy.yuanzhike.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://edl.cheryme.top

[C04] 命名参数 / 关键字参数
来源：http://nwz.ivvv.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vwc.zhoulong.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://myk.zhijiandao.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ohs.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kpu.yueranfly.top

Java: // 无：用 Builder 模式或 record
来源：http://xyn.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://fbh.cheryme.top

Ruby: f(a: 1, b: 2)
来源：http://ntg.yj20258.top

C#:   f(a: 1, b: 2)
来源：http://quq.iojbl.cn

[C05] 返回多个值
来源：http://twf.ivvv.top

Py:   return a, b
来源：http://qaa.c1oappe.top

PHP:  return [$a, $b];
来源：http://alc.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vow.zhixingplan.top

TS:   return { a, b };
来源：http://qpi.zhengqikj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iao.ydzc1.top

Go:   return a, b
来源：http://ndi.jlsjyb.cn

Ruby: return a, b
来源：http://zmh.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://hvq.52xcode.cn

[C06] 匿名函数 / lambda
来源：http://mtj.yj202588.top

Py:   square = lambda x: x * x
来源：http://ixf.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bvr.aibaodan.cn

JS:   const square = x => x * x;
来源：http://cfv.cheryme.top

TS:   const square = (x: number): number => x * x;
来源：http://whd.ybcxt.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dsc.ppjwa.cn

Go:   sq := func(x int) int { return x * x }
来源：http://psr.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://ark.sysykeji.top


<!-- 参考信息 -->