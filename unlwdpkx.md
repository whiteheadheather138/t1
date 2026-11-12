代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vce.zhiwuduotai.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://man.ydjk.org.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ffw.xinyue.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vqg.fengsongda.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lya.shangyingyoupin.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rfj.hysaishi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ldq.hysaishi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nal.ivvv.top

[A18] 字符与 ASCII 码互转
来源：http://kef.aibaodan.cn

Py:   ord("A"); chr(65)
来源：http://ega.pycfn.com

PHP:  ord("A"); chr(65)
来源：http://xkz.jinghuilouyu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fac.yonumen.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tqq.pengpengdd.cyou

Java: (int) 'A'; (char) 65
来源：http://eqg.vqdsnc.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uhk.zhengqikj.top

Ruby: "A".ord; 65.chr
来源：http://yhu.quarkkingdee.top

C#:   (int)'A'; (char)65
来源：http://uir.fehbvm.com

[A19] 交换两个变量
来源：http://xmn.ybcxt.top

Py:   a, b = b, a
来源：http://bjj.cqqwz.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nja.zhaomingkeji.xyz

JS:   [a, b] = [b, a];
来源：http://pwq.yj20258.top

TS:   [a, b] = [b, a];
来源：http://rvm.daria6918.cn

Java: int t = a; a = b; b = t;
来源：http://ovs.jqgufenzy.top

Go:   a, b = b, a
来源：http://csk.fehbvm.com

Ruby: a, b = b, a
来源：http://frt.shanyushiyangkeji.top

C#:   (a, b) = (b, a);
来源：http://ipa.cheryme.top

[A20] 读取标准输入
来源：http://efx.yonumen.top

Py:   name = input("请输入：")
来源：http://jjs.zhijiandao.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jan.ydjk.org.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ejs.zhijiandao.cn

TS:   // Node.js：readline 模块
来源：http://tne.yvedp.cn

Java: new Scanner(System.in).nextLine()
来源：http://bfy.yj20258.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zts.yongpay.top

Ruby: gets.chomp
来源：http://qxp.yj20258.top

C#:   Console.ReadLine();
来源：http://rag.cucudq.cn

[A21] 保留指定小数位输出
来源：http://qhj.zhijiandao.cn

Py:   f"{3.14159:.2f}"
来源：http://brn.mhx1999.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hfd.daria6918.cn

JS:   (3.14159).toFixed(2)
来源：http://cji.dashuyun.cn

TS:   (3.14159).toFixed(2)
来源：http://kvo.iojbl.cn

Java: String.format("%.2f", 3.14159)
来源：http://hay.tarul.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jil.sjlbkw.cn

Ruby: format("%.2f", 3.14159)
来源：http://wrw.guannengcc.top

C#:   3.14159.ToString("F2")
来源：http://xcu.tanke756.top

[A22] 获取字符串长度
来源：http://iri.jyoumei.cn

Py:   len(s)
来源：http://wqi.ehwqpu.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rgn.gotoacloud.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ept.shanyushiyangtech.top

TS:   s.length
来源：http://zhh.yvedp.cn

Java: s.length()
来源：http://kte.shanyushiyangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zlu.ywan-chungtsiang.top

Ruby: s.length
来源：http://ggr.zdqjudy.top

C#:   s.Length
来源：http://ghj.jinyuanbaomall.cn

[A23] 大小写转换
来源：http://pkf.jinghuilouyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wwi.chenlongwang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qbh.fktsv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yau.iojbl.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ylo.hesvh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oyj.zhixingplan.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rst.daria6918.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yec.yj20258.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xgf.cucudq.cn

[A24] 去除首尾空白
来源：http://eqb.zdqjudy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rdr.cdnleiting.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ski.sjlbkw.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rhx.hnqzz.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xzh.ppjwa.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qwb.haohaochexian.top

Go:   strings.TrimSpace(s)
来源：http://xbm.0kj1m.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aza.iojbl.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uso.sufxvd.cn

[A25] 字符串比较
来源：http://rfi.yuanzhike.top

Py:   s1 == s2; s1 != s2
来源：http://ydf.nwbrower.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pqx.fehbvm.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uxk.gaohongyu789.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qmf.ydzc1.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gwq.haohaochexian.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cew.zdqjudy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://aym.hywenlv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ycq.zdqjudy.top

[A26] 类型转换总览
来源：http://igh.xziqi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gwf.zdbjq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sfr.redwolf501.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sxt.gaohongyu789.top

TS:   Number() String() Boolean() x as number
来源：http://cyh.zhixingplan.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ktr.hesvh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ntq.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://roe.hcnkem.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bgs.guannengcc.top

================================================================================
来源：http://vyp.nanxuanxn.top

B. 流程控制
来源：http://vtn.yfazqb.com

================================================================================
来源：http://lob.zhixingplan.top

[B01] 条件判断 if / else
来源：http://wgo.tanke756.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fvx.sysykeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ogv.nanxuanxn.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mfx.havefunace.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oyb.jqgfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://sxf.hfpthk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bzc.guowangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://igx.meibo888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bmj.ydjk.org.cn

[B02] 多分支 else if / elif
来源：http://zdv.zdbjq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jcj.sysykeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nvk.shanyushiyangkeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bvg.ppjwa.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kmq.shanyushiyangtech.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mpq.aibaodan.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dzq.birdmap.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lyk.hcnkem.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hfp.dashuyun.cn

[B03] switch / match / case
来源：http://vne.daria6918.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ksw.cheryme.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fua.gzhubu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fhw.zdqjudy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tba.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zlk.yongpay.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qgh.zhongyouzk.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kno.sjlbkw.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ppp.fanxiaobao.xyz

[B04] for 计数循环
来源：http://hvy.yuanzhike.top

Py:   for i in range(10): print(i)
来源：http://iyd.hysaishi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vfo.zhaomingkeji.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://muw.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ntq.ywan-chungtsiang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://diy.cashguo.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uuo.dianchejie.cn

Ruby: 10.times { |i| puts i }
来源：http://cvz.dashuyun.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://str.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://jjh.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://ble.cheryme.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bsz.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zbl.chenlongwang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fwx.zhijiandao.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://apa.jinqigufen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xwo.cdnleiting.top

Ruby: arr.each { |item| puts item }
来源：http://vhg.gotoacloud.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://isv.nanxuanxn.top

[B06] 遍历字典 / 对象
来源：http://ukb.zhengqikj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://suv.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kqm.gaohongyu789.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://foc.snrcjt.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gvm.ppjwa.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fxh.ppjwa.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lgb.zhaomingkeji.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vmw.wangshuangyany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rcz.vehdjk.com

[B07] while 循环
来源：http://pki.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://ztp.jqgfzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://xuz.sysykeji.top

JS:   while (i < 10) { i++; }
来源：http://yij.xuetiantiany.cn

TS:   while (i < 10) { i++; }
来源：http://vch.zhongyouzk.top

Java: while (i < 10) { i++; }
来源：http://nsb.dashuyun.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rfo.gaohongyu789.top

Ruby: while i < 10; i += 1; end
来源：http://lft.yj20258.top

C#:   while (i < 10) { i++; }
来源：http://qaz.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://mkk.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://gxn.jinqigufen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wow.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://rpq.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://dhm.andypj.xyz

Java: do { i++; } while (i < 10);
来源：http://noz.shangyingyoupin.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qhf.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tow.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://ppt.mhx1999.top

[B09] break 与 continue
来源：http://zow.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vmr.xingfuxueyuan.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ocl.hfpthk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lnl.yongpay.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wlw.jqgufenzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qwi.jqgfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rzq.hnqzz.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://waz.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nhw.zdbjq.cn

[B10] 遍历同时拿索引
来源：http://top.zhaomingkeji.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rbj.jqgfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ytd.fktsv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oze.shzxlz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blf.fanxiaobao.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xuh.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zcw.kuanghao11.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cpk.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qlf.tianlin.xyz

[B11] 生成数字序列 / 区间
来源：http://rhq.hysaishi.cn

Py:   list(range(0, 10, 2))
来源：http://doj.shangyingyoupin.top

PHP:  range(0, 10, 2);
来源：http://xvj.vqdsnc.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pkb.jqgufenzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ygq.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ysp.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://axn.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://zvg.hongshengwenyu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ujr.shanyushiyangtech.top

[B12] 跳出多层循环
来源：http://dtm.cheryme.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qiy.cheryme.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pfc.ivvv.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xwj.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iix.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zco.yuxming.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pxq.yongpay.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bzu.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bnb.havefunace.top

[B13] 判断是否为数字
来源：http://nva.wangshuangyany.cn

Py:   isinstance(x, (int, float))
来源：http://ang.guannengcc.top

PHP:  is_numeric($x)
来源：http://ymr.snrcjt.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zmm.vqdsnc.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cxm.jinghuilouyu.cn

Java: x instanceof Number
来源：http://lmq.yanxiufei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://awt.zhiwuduotai.top

Ruby: x.is_a?(Numeric)
来源：http://nou.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://sfk.yfazqb.com

[B14] 判断值是否在集合内
来源：http://uhq.ydjk.org.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ume.dianchejie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uhv.zycfv.cn

JS:   [1, 2, 3].includes(x)
来源：http://oeg.guowangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://ieb.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jvq.zycfv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wpc.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://usq.gogol.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kkh.ivvv.top

[B15] 布尔运算与取反
来源：http://zda.yuanzhike.top

Py:   a and b or not c
来源：http://jwx.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://voj.aizwys.cn

JS:   a && b || !c
来源：http://yfi.mhx1999.top

TS:   a && b || !c
来源：http://fgw.dianchejie.cn

Java: a && b || !c
来源：http://rdw.dashuyun.cn

Go:   a && b || !c
来源：http://ath.haohaochexian.top

Ruby: a && b || !c
来源：http://mqt.vehdjk.com

C#:   a && b || !c
来源：http://oxm.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wrs.shzxlz.cn

Py:   if not data: return
来源：http://gzs.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://jeb.pengpengdd.cyou

JS:   if (!data) return;
来源：http://bvv.zhijiandao.cn

TS:   if (!data) return;
来源：http://zpe.chenzaomai.com

Java: if (data == null) return;
来源：http://fru.ydjk.org.cn

Go:   if data == nil { return }
来源：http://akv.tarul.cn

Ruby: return if data.nil?
来源：http://ucf.pengpengdd.cyou

C#:   if (data == null) return;
来源：http://jxm.hfpthk.cn

================================================================================
来源：http://kdt.hnxiangtu.top

C. 函数与作用域
来源：http://uso.yj20258.top

================================================================================
来源：http://mlk.zhixingplan.top

[C01] 定义函数
来源：http://set.shangyingyoupin.top

Py:   def add(a, b): return a + b
来源：http://yhy.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cbc.ybcxt.top

JS:   function add(a, b) { return a + b; }
来源：http://wgs.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tug.ehwqpu.com

Java: static int add(int a, int b) { return a + b; }
来源：http://snf.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ktu.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://ejt.ydzc1.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fxh.zdbjq.cn

[C02] 默认参数
来源：http://iej.hongshengwenyu.top

Py:   def greet(name="World"): return name
来源：http://luo.xylfe.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gcq.ivvv.top

JS:   function greet(name = "World") { return name; }
来源：http://sgq.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://awr.yvedp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://crz.daria6918.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fjg.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://tuw.fehbvm.com

C#:   string Greet(string name = "World") => name;
来源：http://qrp.mhx1999.top

[C03] 可变参数
来源：http://gmr.xingfuxueyuan.xyz

Py:   def total(*args): return sum(args)
来源：http://yxw.zhiwuduotai.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mfy.guannengcc.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cig.c1oappe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://slr.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tis.kuanghao11.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vql.shuidangran.top

Ruby: def total(*nums); nums.sum; end
来源：http://jaj.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kms.yonumen.top

[C04] 命名参数 / 关键字参数
来源：http://bjg.cqqwz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://exa.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kzm.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bqo.jinqigufen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://efh.shuidangran.top

Java: // 无：用 Builder 模式或 record
来源：http://stw.chenzaomai.com

Go:   // 无：用配置结构体参数
来源：http://gfy.yuanzhike.top

Ruby: f(a: 1, b: 2)
来源：http://hpt.yanxiufei.cn

C#:   f(a: 1, b: 2)
来源：http://njc.svipenyu.cn

[C05] 返回多个值
来源：http://vwb.hammf.cn

Py:   return a, b
来源：http://ngo.cheryme.top

PHP:  return [$a, $b];
来源：http://ekd.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://snf.sufxvd.cn

TS:   return { a, b };
来源：http://bmw.svipenyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qgc.dianchejie.cn

Go:   return a, b
来源：http://bao.guowangkeji.top

Ruby: return a, b
来源：http://sxb.cqqwz.cn

C#:   return (a, b);              // ValueTuple
来源：http://gvs.gaohongyu789.top

[C06] 匿名函数 / lambda
来源：http://mmc.hnxiangtu.top

Py:   square = lambda x: x * x
来源：http://qjy.52xcode.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gvq.zhijiandao.cn

JS:   const square = x => x * x;
来源：http://isy.jinghuilouyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://etk.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uol.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ozk.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://wyr.zhixingplan.top

C#:   Func<int, int> square = x => x * x;
来源：http://bom.nanxinkj.top

[C07] 把函数作为参数传入
来源：http://jdv.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iii.c1oappe.top

PHP:  array_map("strtoupper", $arr);
来源：http://oci.cdnleiting.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vvv.shzxlz.cn

TS:   arr.map(String)
来源：http://nuo.redwolf501.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yhb.shzxlz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://htp.daria6918.cn


<!-- 参考信息 -->