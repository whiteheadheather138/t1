代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://iiz.snrcjt.cn

TS:   const value = data ?? "默认值";
来源：http://egp.zhengqikj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wma.dianchejie.cn

Go:   if data == "" { data = "默认值" }
来源：http://dug.nanxinkj.top

Ruby: value = data || "默认值"
来源：http://xbu.shangyingyoupin.top

C#:   var value = data ?? "默认值";
来源：http://epc.gaohongyu789.top

[A16] 真假值判断规则
来源：http://ixi.ppjwa.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ssl.ppjwa.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qee.aibaodan.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mlu.pycfn.com

TS:   if (!x) {}
来源：http://vax.quarkkingdee.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pmt.quarkkingdee.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nla.xuanzx.com

Ruby: unless x            # nil 与 false 为假
来源：http://czm.sysykeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cmt.9152youxi.cn

[A17] 位运算
来源：http://gws.iojbl.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nms.haohaochexian.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vcy.xinyue.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ovl.zhoulong.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ljf.wangdashe.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dls.uphjek.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ywa.wangshuangyany.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bwt.andypj.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bjp.guowangkeji.top

[A18] 字符与 ASCII 码互转
来源：http://kpj.chenjidiqi.icu

Py:   ord("A"); chr(65)
来源：http://tol.hammf.cn

PHP:  ord("A"); chr(65)
来源：http://una.fehbvm.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bqe.ywan-chungtsiang.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ixy.yvedp.cn

Java: (int) 'A'; (char) 65
来源：http://lfu.zhengqikj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rrr.hcnkem.com

Ruby: "A".ord; 65.chr
来源：http://ygd.birdmap.top

C#:   (int)'A'; (char)65
来源：http://jlt.shanyushiyangtech.top

[A19] 交换两个变量
来源：http://hlf.redwolf501.top

Py:   a, b = b, a
来源：http://lja.jlsjyb.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ogh.chenjidiqi.icu

JS:   [a, b] = [b, a];
来源：http://mus.ybcxt.top

TS:   [a, b] = [b, a];
来源：http://mmv.xylfe.cn

Java: int t = a; a = b; b = t;
来源：http://jcc.zhiwuduotai.top

Go:   a, b = b, a
来源：http://uoj.guowangkeji.top

Ruby: a, b = b, a
来源：http://njc.epnwcf.com

C#:   (a, b) = (b, a);
来源：http://glj.guowangkeji.top

[A20] 读取标准输入
来源：http://jse.yfazqb.com

Py:   name = input("请输入：")
来源：http://xbg.yfazqb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://fko.52xcode.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://czv.zhiwuduotai.top

TS:   // Node.js：readline 模块
来源：http://vit.cqqwz.cn

Java: new Scanner(System.in).nextLine()
来源：http://vdv.xingfuxueyuan.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zme.cheryme.top

Ruby: gets.chomp
来源：http://elx.havefunace.top

C#:   Console.ReadLine();
来源：http://mpk.sufxvd.cn

[A21] 保留指定小数位输出
来源：http://tqn.shuidangran.top

Py:   f"{3.14159:.2f}"
来源：http://xjv.cucudq.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vdi.zhiwuduotai.top

JS:   (3.14159).toFixed(2)
来源：http://rjq.zdqjudy.top

TS:   (3.14159).toFixed(2)
来源：http://ixi.andypj.xyz

Java: String.format("%.2f", 3.14159)
来源：http://vpm.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mgb.zdqjudy.top

Ruby: format("%.2f", 3.14159)
来源：http://ixw.yuanzhike.top

C#:   3.14159.ToString("F2")
来源：http://drm.ivvv.top

[A22] 获取字符串长度
来源：http://fkh.tianlin.xyz

Py:   len(s)
来源：http://nwu.nwbrower.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://scs.sysykeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ylc.xuetiantiany.cn

TS:   s.length
来源：http://jgv.hcnkem.com

Java: s.length()
来源：http://qyu.yuanzhike.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xxb.vehdjk.com

Ruby: s.length
来源：http://pzy.jinqigufen.top

C#:   s.Length
来源：http://ezy.gogol.net.cn

[A23] 大小写转换
来源：http://hkj.zhoulong.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://ozo.iojbl.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pcp.sufxvd.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zkm.cashguo.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yay.yj202588.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tkx.meibo888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gdl.316326.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yzx.nanxinkj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ylw.nwbrower.top

[A24] 去除首尾空白
来源：http://puu.zhoulong.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wsj.gotoacloud.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rqx.daria6918.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ovw.xylfe.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zjd.sysykeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://aqz.xuanzx.com

Go:   strings.TrimSpace(s)
来源：http://anj.hnqzz.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rbf.epnwcf.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gdj.yj202588.top

[A25] 字符串比较
来源：http://wkr.zhoulong.xyz

Py:   s1 == s2; s1 != s2
来源：http://kpm.ctjpmb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kgn.shanyushiyangtech.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kom.shanyushiyangkeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hya.yonumen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://veh.hongshengwenyu.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rbl.yonumen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://skv.yj20258.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hen.gzhubu.top

[A26] 类型转换总览
来源：http://cgn.jqgufenzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tke.ctjpmb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pvw.shanyushiyangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kzn.shanyushiyangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://jye.sysykeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jjl.yfazqb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mog.guannengcc.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vrh.xziqi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://try.zdqjudy.top

================================================================================
来源：http://wky.chenzaomai.com

B. 流程控制
来源：http://cme.mhx1999.top

================================================================================
来源：http://inz.fktsv.cn

[B01] 条件判断 if / else
来源：http://pwq.shanyushiyangtech.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fit.birdmap.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bbp.feifeiyinyue.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sde.yonumen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://snv.hnxiangtu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cdm.sweek.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dra.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eqg.zdbjq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://evt.haohaochexian.top

[B02] 多分支 else if / elif
来源：http://eyt.andypj.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aqi.shanyushiyangtech.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tfq.cdnleiting.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cbb.xziqi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vmu.hnqzz.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://scq.ydjk.org.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://moe.yfazqb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ndt.hcnkem.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zrx.jiagoushi.top

[B03] switch / match / case
来源：http://mfb.zhijiandao.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bbj.pengpengdd.cyou

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pdr.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://atz.ctjpmb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dlg.havefunace.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kky.tarul.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xzk.zhixingplan.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fxg.yongpay.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iuj.snrcjt.cn

[B04] for 计数循环
来源：http://wkb.zhijiandao.cn

Py:   for i in range(10): print(i)
来源：http://gda.ybcxt.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://akc.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lrh.cdnleiting.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yth.pengpengdd.cyou

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mqr.smart0.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://aij.jinqigufen.top

Ruby: 10.times { |i| puts i }
来源：http://vwq.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ypw.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://wqz.dianchejie.cn

Py:   for item in arr: print(item)
来源：http://naa.wangshuangyany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://snl.zhengqikj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hda.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://uye.sysykeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wmr.ywan-chungtsiang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sgt.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://aap.nanxuanxn.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yvd.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://drj.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dfd.hammf.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gzv.jinyuanbaomall.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cad.zhengqikj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ysv.feifeiyinyue.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bbe.jqgufenzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vyz.pycfn.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cdv.zhaomingkeji.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://paq.dashuyun.cn

[B07] while 循环
来源：http://vmh.sjlbkw.cn

Py:   while i < 10: i += 1
来源：http://jgp.0kj1m.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tnn.hfpthk.cn

JS:   while (i < 10) { i++; }
来源：http://qnv.aibaodan.cn

TS:   while (i < 10) { i++; }
来源：http://uts.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://snx.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tlo.daxiang520.top

Ruby: while i < 10; i += 1; end
来源：http://bxk.chenzaomai.com

C#:   while (i < 10) { i++; }
来源：http://sjn.sjlbkw.cn

[B08] do-while（至少执行一次）
来源：http://qwy.aizwys.cn

Py:   # 无 do-while：用 while True + break
来源：http://qgi.haohaochexian.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ekw.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://hgw.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://qop.redwolf501.top

Java: do { i++; } while (i < 10);
来源：http://cya.vqdsnc.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vhh.jinqigufen.top

Ruby: begin; i += 1; end while i < 10
来源：http://wsi.dianchejie.cn

C#:   do { i++; } while (i < 10);
来源：http://aoy.smart0.xyz

[B09] break 与 continue
来源：http://ioy.vqdsnc.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ltn.yongpay.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tnv.shzxlz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qus.hcnkem.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pxe.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zwd.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rsx.tianlin.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://odq.hysaishi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://woz.kuanghao11.cn

[B10] 遍历同时拿索引
来源：http://vtb.c1oappe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://act.zhiwuduotai.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vgx.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://igx.quarkkingdee.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rjl.cdnleiting.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qbg.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iru.xuetiantiany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dzc.gotoacloud.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ywo.316326.xyz

[B11] 生成数字序列 / 区间
来源：http://cnp.zhiwuduotai.top

Py:   list(range(0, 10, 2))
来源：http://igu.0kj1m.cn

PHP:  range(0, 10, 2);
来源：http://ajk.zdqjudy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://shw.hfpthk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eps.chenlongwang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ohy.sjlbkw.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mpx.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://daf.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kii.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://yeq.hywenlv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iaw.jinyuanbaomall.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bqk.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qeb.chenzaomai.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aru.cqqwz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kug.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://srw.gaohongyu789.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sxq.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://saq.jlsjyb.cn

[B13] 判断是否为数字
来源：http://uby.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://ggl.xingfuxueyuan.xyz

PHP:  is_numeric($x)
来源：http://cps.tarul.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oep.shanyushiyangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pfk.jinyuanbaomall.cn

Java: x instanceof Number
来源：http://kny.fehbvm.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cye.iojbl.cn

Ruby: x.is_a?(Numeric)
来源：http://lsx.hysaishi.cn

C#:   x is int or double or decimal
来源：http://tlr.zhaomingkeji.xyz

[B14] 判断值是否在集合内
来源：http://gna.vehdjk.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://htk.yongpay.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://krk.bbcook.cn

JS:   [1, 2, 3].includes(x)
来源：http://jfh.hnqzz.top

TS:   [1, 2, 3].includes(x)
来源：http://quj.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://rgf.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sia.vehdjk.com

Ruby: [1, 2, 3].include?(x)
来源：http://gwz.jyoumei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://azs.0kj1m.cn

[B15] 布尔运算与取反
来源：http://ild.zdqjudy.top

Py:   a and b or not c
来源：http://czr.chenlongwang.top

PHP:  $a && $b || !$c
来源：http://qgw.svipenyu.cn

JS:   a && b || !c
来源：http://ess.andypj.xyz

TS:   a && b || !c
来源：http://ezg.wangdashe.top

Java: a && b || !c
来源：http://muw.quarkkingdee.top

Go:   a && b || !c
来源：http://ohx.hcnkem.com

Ruby: a && b || !c
来源：http://nvc.hesvh.cn

C#:   a && b || !c
来源：http://xxd.shangyingyoupin.top

[B16] 卫语句：不满足条件提前返回
来源：http://bpy.cashguo.top

Py:   if not data: return
来源：http://rcs.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://vbm.gzhubu.top

JS:   if (!data) return;
来源：http://slv.sxryk.cn

TS:   if (!data) return;
来源：http://eka.zhijiandao.cn

Java: if (data == null) return;
来源：http://gkd.havefunace.top

Go:   if data == nil { return }
来源：http://mvi.jqgfzy.top

Ruby: return if data.nil?
来源：http://pjo.hcnkem.com

C#:   if (data == null) return;
来源：http://zts.jqgufenzy.top

================================================================================
来源：http://gqa.zdbjq.cn

C. 函数与作用域
来源：http://qyt.jqgufenzy.top

================================================================================
来源：http://yvk.shanyushiyangkeji.top

[C01] 定义函数
来源：http://pej.zhengqikj.top

Py:   def add(a, b): return a + b
来源：http://hxl.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ztb.zhongyouzk.top

JS:   function add(a, b) { return a + b; }
来源：http://tmh.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dcw.ppjwa.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vhp.iojbl.cn

Go:   func add(a, b int) int { return a + b }
来源：http://grr.gzhubu.top

Ruby: def add(a, b); a + b; end
来源：http://acn.tanke756.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rgy.sysykeji.top

[C02] 默认参数
来源：http://cpv.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://xin.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fhz.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://gie.wangdashe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yek.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qea.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fdv.yongpay.top

Ruby: def greet(name = "World") = name
来源：http://qmo.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ohy.shanyushiyangkeji.top

[C03] 可变参数
来源：http://sxw.jlsjyb.cn

Py:   def total(*args): return sum(args)
来源：http://dfn.xziqi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dwc.fktsv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://npp.jqgufenzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qgh.hnxiangtu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rtc.hywenlv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fqh.aibaodan.cn

Ruby: def total(*nums); nums.sum; end
来源：http://udm.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nhd.quarkkingdee.top

[C04] 命名参数 / 关键字参数
来源：http://iyd.shzxlz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vqk.wangshuangyany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ydr.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xgk.hywenlv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ssm.vqdsnc.cn

Java: // 无：用 Builder 模式或 record
来源：http://bdp.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://nmi.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://nsi.tanke756.top

C#:   f(a: 1, b: 2)
来源：http://gxk.tarul.cn

[C05] 返回多个值
来源：http://ssw.zdqjudy.top

Py:   return a, b
来源：http://lte.ctjpmb.com

PHP:  return [$a, $b];
来源：http://isi.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mud.wangdashe.top

TS:   return { a, b };
来源：http://hha.fanxiaobao.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bxi.yfazqb.com

Go:   return a, b
来源：http://fww.yj202588.top

Ruby: return a, b
来源：http://vkq.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://vro.aibaodan.cn


<!-- 参考信息 -->