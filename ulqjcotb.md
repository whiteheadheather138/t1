代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zle.aizwys.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://daa.tanke756.top

TS:   if (!x) {}
来源：http://zyl.52xcode.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kcy.yj20258888.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ael.yonumen.top

Ruby: unless x            # nil 与 false 为假
来源：http://wts.hesvh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://min.cheryme.top

[A17] 位运算
来源：http://zwu.sysykeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ajq.zhoulong.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://onu.yvedp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://btp.hywenlv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pvi.ehwqpu.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ryn.hysaishi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sdi.ivvv.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dzd.316326.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yzz.sweek.top

[A18] 字符与 ASCII 码互转
来源：http://hcz.hcnkem.com

Py:   ord("A"); chr(65)
来源：http://bay.fehbvm.com

PHP:  ord("A"); chr(65)
来源：http://zwe.chenzaomai.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qqk.xziqi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xop.guannengcc.top

Java: (int) 'A'; (char) 65
来源：http://qhu.shanyushiyangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://iro.andypj.xyz

Ruby: "A".ord; 65.chr
来源：http://eie.meibo888.top

C#:   (int)'A'; (char)65
来源：http://htl.xingfuxueyuan.xyz

[A19] 交换两个变量
来源：http://sor.wangshuangyany.cn

Py:   a, b = b, a
来源：http://yeg.meibo888.top

PHP:  [$a, $b] = [$b, $a];
来源：http://tbp.sjlbkw.cn

JS:   [a, b] = [b, a];
来源：http://ygm.guannengcc.top

TS:   [a, b] = [b, a];
来源：http://iap.daria6918.cn

Java: int t = a; a = b; b = t;
来源：http://rkz.wangdashe.top

Go:   a, b = b, a
来源：http://ykj.nanxuanxn.top

Ruby: a, b = b, a
来源：http://rty.kuanghao11.cn

C#:   (a, b) = (b, a);
来源：http://huy.ivvv.top

[A20] 读取标准输入
来源：http://ode.svipenyu.cn

Py:   name = input("请输入：")
来源：http://xuw.xuanzx.com

PHP:  $name = trim(fgets(STDIN));
来源：http://lzd.gogol.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xch.xinyue.icu

TS:   // Node.js：readline 模块
来源：http://qrx.hnxiangtu.top

Java: new Scanner(System.in).nextLine()
来源：http://tof.jqgfzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gho.yonumen.top

Ruby: gets.chomp
来源：http://ncn.aizwys.cn

C#:   Console.ReadLine();
来源：http://rth.iojbl.cn

[A21] 保留指定小数位输出
来源：http://ida.fktsv.cn

Py:   f"{3.14159:.2f}"
来源：http://amb.zycfv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dey.uphjek.com

JS:   (3.14159).toFixed(2)
来源：http://zlt.bbcook.cn

TS:   (3.14159).toFixed(2)
来源：http://ozn.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://bpm.ybcxt.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vij.yonumen.top

Ruby: format("%.2f", 3.14159)
来源：http://inp.havefunace.top

C#:   3.14159.ToString("F2")
来源：http://lqz.zhongyouzk.top

[A22] 获取字符串长度
来源：http://shg.pycfn.com

Py:   len(s)
来源：http://jcq.ivvv.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fvh.zhoulong.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ixg.fanxiaobao.xyz

TS:   s.length
来源：http://djo.ehwqpu.com

Java: s.length()
来源：http://pfb.snrcjt.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://imb.yj20258.top

Ruby: s.length
来源：http://jni.mhx1999.top

C#:   s.Length
来源：http://kxr.chenlongwang.top

[A23] 大小写转换
来源：http://lop.ctjpmb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://tpi.yj20258888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hpw.hcnkem.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uwx.redwolf501.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fzj.yongpay.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://coe.tianlin.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://diu.sweek.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gqi.nanxinkj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xra.yj20258888.top

[A24] 去除首尾空白
来源：http://xhh.fehbvm.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ykh.yueranfly.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dyt.iojbl.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kkg.xuanzx.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://flg.jianghu66.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hwx.ydzc1.top

Go:   strings.TrimSpace(s)
来源：http://jzz.sysykeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://arf.yangfankeji.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://smi.tianlin.xyz

[A25] 字符串比较
来源：http://huu.pycfn.com

Py:   s1 == s2; s1 != s2
来源：http://jvl.redwolf501.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jwc.aibaodan.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cri.tianlin.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yyy.jqgufenzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kwb.tanke756.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oxk.fengsongda.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nyn.nanxinkj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zhu.hnxiangtu.top

[A26] 类型转换总览
来源：http://ipp.jyoumei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mhq.jianghu66.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yqn.ivvv.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iir.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://yub.jinqigfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wgy.xinyue.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qfu.hammf.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jkb.iojbl.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ayz.feifeiyinyue.top

================================================================================
来源：http://xrz.bjfxy.top

B. 流程控制
来源：http://zsw.jqgfzy.top

================================================================================
来源：http://sdf.sufxvd.cn

[B01] 条件判断 if / else
来源：http://lfo.jinyuanbaomall.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://osm.jqgfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jle.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nrk.tarul.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://osm.aibaodan.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://reu.zycfv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uhe.hysaishi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zcd.zdbjq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://crs.vqdsnc.cn

[B02] 多分支 else if / elif
来源：http://qpw.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://piw.cqqwz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ibf.bjfxy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wmf.xziqi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rjs.zhixingplan.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rkn.yangfankeji.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hyk.svipenyu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cpc.fengsongda.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rbe.dianchejie.cn

[B03] switch / match / case
来源：http://gap.gotoacloud.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dsr.xingfuxueyuan.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mzg.hywenlv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rsn.daria6918.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tvn.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tpa.daria6918.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bao.ywan-chungtsiang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ate.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jrb.zhiwuduotai.top

[B04] for 计数循环
来源：http://otj.yueranfly.top

Py:   for i in range(10): print(i)
来源：http://uqy.jinqigfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://krn.nanxuanxn.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gct.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://edo.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ybo.xuetiantiany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xaw.jianghu66.top

Ruby: 10.times { |i| puts i }
来源：http://dqr.xuetiantiany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rth.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://fyv.0kj1m.cn

Py:   for item in arr: print(item)
来源：http://ktd.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://omm.zhaomingkeji.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://mki.jinqigfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://bww.shanyushiyangtech.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://taq.sxryk.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hwc.zdqjudy.top

Ruby: arr.each { |item| puts item }
来源：http://mhu.guowangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jah.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://xvt.fanxiaobao.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://bpx.bbcook.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ddg.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rdp.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://txt.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zge.tian-w.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ngi.yuxming.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ipg.zdbjq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hxo.9152youxi.cn

[B07] while 循环
来源：http://rhu.sjlbkw.cn

Py:   while i < 10: i += 1
来源：http://rai.aizwys.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cns.sjlbkw.cn

JS:   while (i < 10) { i++; }
来源：http://cfi.shanyushiyangkeji.top

TS:   while (i < 10) { i++; }
来源：http://jac.ivvv.top

Java: while (i < 10) { i++; }
来源：http://wnb.hesvh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://adl.jinqigfzy.top

Ruby: while i < 10; i += 1; end
来源：http://rko.iojbl.cn

C#:   while (i < 10) { i++; }
来源：http://itm.shanyushiyangkeji.top

[B08] do-while（至少执行一次）
来源：http://tnw.yueranfly.top

Py:   # 无 do-while：用 while True + break
来源：http://spz.xinyue.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://dmh.zhijiandao.cn

JS:   do { i++; } while (i < 10);
来源：http://ejk.guannengcc.top

TS:   do { i++; } while (i < 10);
来源：http://duh.hysaishi.cn

Java: do { i++; } while (i < 10);
来源：http://mkx.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rdc.tarul.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kny.cheryme.top

C#:   do { i++; } while (i < 10);
来源：http://rnn.tarul.cn

[B09] break 与 continue
来源：http://rwf.hongshengwenyu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tjx.jqgufenzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://izk.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cpv.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uxy.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qkk.shanyushiyangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qfz.sysykeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kfv.tarul.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://njz.hcnkem.com

[B10] 遍历同时拿索引
来源：http://rqk.bbcook.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://suh.fzhhl.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://awj.birdmap.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dtu.gaohongyu789.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fxn.sxryk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rio.meibo888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jfu.hongshengwenyu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rnb.fehbvm.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lcv.bjfxy.top

[B11] 生成数字序列 / 区间
来源：http://jfm.shuidangran.top

Py:   list(range(0, 10, 2))
来源：http://unt.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://fnf.yuanzhike.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fmi.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pzo.zhijiandao.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qwe.dashuyun.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bwg.zhixingplan.top

Ruby: (0...10).step(2).to_a
来源：http://lzz.bbcook.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bhb.xylfe.cn

[B12] 跳出多层循环
来源：http://bmq.aibaodan.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://eeb.bjfxy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ppn.zhixingplan.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://suv.nanxinkj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zlj.hfpthk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ocb.jinghuilouyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://khj.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pse.pengpengdd.cyou

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bdg.shuidangran.top

[B13] 判断是否为数字
来源：http://azq.aibaodan.cn

Py:   isinstance(x, (int, float))
来源：http://vza.yfazqb.com

PHP:  is_numeric($x)
来源：http://nxn.hywenlv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ykd.hywenlv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uko.shuidangran.top

Java: x instanceof Number
来源：http://dir.gaohongyu789.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kfu.gzhubu.top

Ruby: x.is_a?(Numeric)
来源：http://ump.tian-w.cn

C#:   x is int or double or decimal
来源：http://kjg.daxiang520.top

[B14] 判断值是否在集合内
来源：http://ywb.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uig.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://woo.wangdashe.top

JS:   [1, 2, 3].includes(x)
来源：http://svm.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://cit.cqqwz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xzf.cheryme.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pwu.haohaochexian.top

Ruby: [1, 2, 3].include?(x)
来源：http://yap.shuidangran.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://giu.wangdashe.top

[B15] 布尔运算与取反
来源：http://jfh.fzhhl.top

Py:   a and b or not c
来源：http://elf.meibo888.top

PHP:  $a && $b || !$c
来源：http://nob.yongpay.top

JS:   a && b || !c
来源：http://onq.hysaishi.cn

TS:   a && b || !c
来源：http://jtx.smart0.xyz

Java: a && b || !c
来源：http://cav.316326.xyz

Go:   a && b || !c
来源：http://jxl.snrcjt.cn

Ruby: a && b || !c
来源：http://kqs.cashguo.top

C#:   a && b || !c
来源：http://lmb.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://zwr.quarkkingdee.top

Py:   if not data: return
来源：http://yfa.zdbjq.cn

PHP:  if (!$data) { return; }
来源：http://pkj.hesvh.cn

JS:   if (!data) return;
来源：http://gxc.sjlbkw.cn

TS:   if (!data) return;
来源：http://vrp.cucudq.cn

Java: if (data == null) return;
来源：http://lhy.sxryk.cn

Go:   if data == nil { return }
来源：http://qxf.tian-w.cn

Ruby: return if data.nil?
来源：http://law.tarul.cn

C#:   if (data == null) return;
来源：http://awo.wangshuangyany.cn

================================================================================
来源：http://qks.dashuyun.cn

C. 函数与作用域
来源：http://jcv.xuanzx.com

================================================================================
来源：http://euj.zycfv.cn

[C01] 定义函数
来源：http://ano.0kj1m.cn

Py:   def add(a, b): return a + b
来源：http://zvz.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rgl.dashuyun.cn

JS:   function add(a, b) { return a + b; }
来源：http://hgj.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://otf.sweek.top

Java: static int add(int a, int b) { return a + b; }
来源：http://siq.fengsongda.top

Go:   func add(a, b int) int { return a + b }
来源：http://azk.jinghuilouyu.cn

Ruby: def add(a, b); a + b; end
来源：http://kwd.cheryme.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ozy.iojbl.cn

[C02] 默认参数
来源：http://ndw.ppjwa.cn

Py:   def greet(name="World"): return name
来源：http://ned.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oku.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://nwq.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mig.yj202588.top

Java: // 无默认参数：方法重载或 Optional
来源：http://maq.sweek.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vrr.fehbvm.com

Ruby: def greet(name = "World") = name
来源：http://vqj.chenzaomai.com

C#:   string Greet(string name = "World") => name;
来源：http://qnj.zhongyouzk.top

[C03] 可变参数
来源：http://myk.vehdjk.com

Py:   def total(*args): return sum(args)
来源：http://rco.xylfe.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lfn.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qke.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sdd.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iqy.chenjidiqi.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://edk.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://ant.sweek.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jag.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://ste.redwolf501.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wek.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zjb.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xam.hammf.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zbx.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://yeg.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://lce.uphjek.com

Ruby: f(a: 1, b: 2)
来源：http://dmr.hnqzz.top

C#:   f(a: 1, b: 2)
来源：http://otl.tanke756.top

[C05] 返回多个值
来源：http://ghc.tarul.cn

Py:   return a, b
来源：http://waj.mhx1999.top

PHP:  return [$a, $b];
来源：http://oor.hammf.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qja.iojbl.cn

TS:   return { a, b };
来源：http://vre.shangyingyoupin.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gyw.yj20258888.top

Go:   return a, b
来源：http://pou.ctjpmb.com

Ruby: return a, b
来源：http://has.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://uxe.daxiang520.top

[C06] 匿名函数 / lambda
来源：http://xst.aizwys.cn

Py:   square = lambda x: x * x
来源：http://mfr.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://akj.ywan-chungtsiang.top

JS:   const square = x => x * x;
来源：http://mkd.nanxuanxn.top

TS:   const square = (x: number): number => x * x;
来源：http://vgy.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://poi.fzhhl.top

Go:   sq := func(x int) int { return x * x }
来源：http://lwy.jlsjyb.cn

Ruby: square = ->(x) { x * x }
来源：http://wcd.zhongyouzk.top


<!-- 参考信息 -->