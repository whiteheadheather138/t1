代发 wailian999

Ruby: value = data || "默认值"
来源：http://dwg.redwolf501.top

C#:   var value = data ?? "默认值";
来源：http://gbk.xinyue.icu

[A16] 真假值判断规则
来源：http://mwx.hongshengwenyu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://onj.smart0.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bne.yangfankeji.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nkp.yfazqb.com

TS:   if (!x) {}
来源：http://xbg.mhx1999.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jmv.dashuyun.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kyp.cqqwz.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tmm.epnwcf.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://maq.pycfn.com

[A17] 位运算
来源：http://tuw.xuanzx.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xsu.xingfuxueyuan.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pzp.guowangkeji.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dbl.zycfv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://obg.chenzaomai.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zwi.svipenyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kif.gzhubu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ekf.hcnkem.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://feg.52xcode.cn

[A18] 字符与 ASCII 码互转
来源：http://sbd.yonumen.top

Py:   ord("A"); chr(65)
来源：http://rjq.zhixingplan.top

PHP:  ord("A"); chr(65)
来源：http://dvp.ehwqpu.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lly.gogol.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xoj.wangshuangyany.cn

Java: (int) 'A'; (char) 65
来源：http://brv.gotoacloud.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sdx.0kj1m.cn

Ruby: "A".ord; 65.chr
来源：http://mmb.zhaomingkeji.xyz

C#:   (int)'A'; (char)65
来源：http://kop.shanyushiyangkeji.top

[A19] 交换两个变量
来源：http://xhg.bjfxy.top

Py:   a, b = b, a
来源：http://wet.yonumen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ekf.jinqigfzy.top

JS:   [a, b] = [b, a];
来源：http://mwm.jqgfzy.top

TS:   [a, b] = [b, a];
来源：http://gah.aibaodan.cn

Java: int t = a; a = b; b = t;
来源：http://iac.iojbl.cn

Go:   a, b = b, a
来源：http://jkb.yuanzhike.top

Ruby: a, b = b, a
来源：http://cbv.jqgfzy.top

C#:   (a, b) = (b, a);
来源：http://mkh.fanxiaobao.xyz

[A20] 读取标准输入
来源：http://hhl.yongpay.top

Py:   name = input("请输入：")
来源：http://mdx.wangdashe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wjf.tian-w.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://anf.jqgufenzy.top

TS:   // Node.js：readline 模块
来源：http://ltx.snrcjt.cn

Java: new Scanner(System.in).nextLine()
来源：http://ugl.yangfankeji.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://byj.ehwqpu.com

Ruby: gets.chomp
来源：http://hpi.zhiwuduotai.top

C#:   Console.ReadLine();
来源：http://ufy.yj202588.top

[A21] 保留指定小数位输出
来源：http://ifi.shuidangran.top

Py:   f"{3.14159:.2f}"
来源：http://lrn.yonumen.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ksr.fanxiaobao.xyz

JS:   (3.14159).toFixed(2)
来源：http://qul.mhx1999.top

TS:   (3.14159).toFixed(2)
来源：http://fms.hnxiangtu.top

Java: String.format("%.2f", 3.14159)
来源：http://ndf.vehdjk.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wnk.jiagoushi.top

Ruby: format("%.2f", 3.14159)
来源：http://yjz.nanxinkj.top

C#:   3.14159.ToString("F2")
来源：http://gqo.xuetiantiany.cn

[A22] 获取字符串长度
来源：http://lnj.yj20258.top

Py:   len(s)
来源：http://vri.haohaochexian.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ojq.zhaomingkeji.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vfs.epnwcf.com

TS:   s.length
来源：http://dpr.chenjidiqi.icu

Java: s.length()
来源：http://xfc.fehbvm.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wfb.wangdashe.top

Ruby: s.length
来源：http://bjc.bjfxy.top

C#:   s.Length
来源：http://pul.sxryk.cn

[A23] 大小写转换
来源：http://uqd.hnqzz.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ses.cdnleiting.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gwz.zhiwuduotai.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zub.xuanzx.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kny.ivvv.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tkv.pycfn.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sna.jinqigfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tiy.jlsjyb.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mpe.yuanzhike.top

[A24] 去除首尾空白
来源：http://oce.ybcxt.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://etm.nanxinkj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hzs.chenjidiqi.icu

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xkq.nwbrower.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mtr.hesvh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mjh.hywenlv.cn

Go:   strings.TrimSpace(s)
来源：http://xnt.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cfi.hysaishi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zcx.kuanghao11.cn

[A25] 字符串比较
来源：http://fri.cheryme.top

Py:   s1 == s2; s1 != s2
来源：http://lxv.aizwys.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vmi.yangfankeji.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dri.ydzc1.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zoo.yj202588.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nqs.yj20258.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://svp.tian-w.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://prk.sjlbkw.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zbb.cucudq.cn

[A26] 类型转换总览
来源：http://qiq.yongpay.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yjb.birdmap.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vcx.havefunace.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ndj.guowangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://akb.xingfuxueyuan.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ukc.xinyue.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://skd.sjlbkw.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cmk.zycfv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zwq.shuidangran.top

================================================================================
来源：http://lil.gotoacloud.top

B. 流程控制
来源：http://wxl.dianchejie.cn

================================================================================
来源：http://szl.shanyushiyangkeji.top

[B01] 条件判断 if / else
来源：http://hsq.shanyushiyangtech.top

Py:   result = "正" if x > 0 else "非正"
来源：http://izj.vehdjk.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wcv.aibaodan.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kji.ywan-chungtsiang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://crp.jinqigfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://gfd.epnwcf.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jlf.jyoumei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cyu.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ijq.zhongyouzk.top

[B02] 多分支 else if / elif
来源：http://ytc.bjfxy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://urr.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wvk.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bob.zycfv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://khb.jianghu66.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ynn.wangdashe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dun.pycfn.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hrp.dashuyun.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xze.ehwqpu.com

[B03] switch / match / case
来源：http://kub.9152youxi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://epd.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xxt.bbcook.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fdn.vqdsnc.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aop.jlsjyb.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gxk.zhoulong.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://waz.sxryk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uyg.jqgfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gls.sjlbkw.cn

[B04] for 计数循环
来源：http://ecc.yvedp.cn

Py:   for i in range(10): print(i)
来源：http://hil.wangshuangyany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://inx.sysykeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eeu.wangdashe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://beu.jinqigfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mov.ybcxt.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ijp.quarkkingdee.top

Ruby: 10.times { |i| puts i }
来源：http://jdz.jinghuilouyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hoa.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://yic.jqgfzy.top

Py:   for item in arr: print(item)
来源：http://lyf.aizwys.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pex.chenjidiqi.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://kev.tian-w.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fpm.zhongyouzk.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://nck.jinqigfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fjv.wangdashe.top

Ruby: arr.each { |item| puts item }
来源：http://frx.fanxiaobao.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lfj.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://htd.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lrg.jqgufenzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jln.guannengcc.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fms.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sqm.hammf.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fcm.dashuyun.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lvf.hammf.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wel.yvedp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://imz.zhengqikj.top

[B07] while 循环
来源：http://dyb.jianghu66.top

Py:   while i < 10: i += 1
来源：http://qsi.tanke756.top

PHP:  while ($i < 10) { $i++; }
来源：http://hjg.0kj1m.cn

JS:   while (i < 10) { i++; }
来源：http://vng.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://gdw.vehdjk.com

Java: while (i < 10) { i++; }
来源：http://ivk.nwbrower.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oub.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://hvf.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://pzh.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://bdr.pengpengdd.cyou

Py:   # 无 do-while：用 while True + break
来源：http://luw.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://adt.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://vzf.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://mtd.tian-w.cn

Java: do { i++; } while (i < 10);
来源：http://ndm.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pmg.tarul.cn

Ruby: begin; i += 1; end while i < 10
来源：http://njn.tian-w.cn

C#:   do { i++; } while (i < 10);
来源：http://jug.shangyingyoupin.top

[B09] break 与 continue
来源：http://kwx.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cfk.nanxinkj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://aix.cheryme.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iab.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://evq.fehbvm.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tvi.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mni.cucudq.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://grd.xingfuxueyuan.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tlm.hammf.cn

[B10] 遍历同时拿索引
来源：http://cqa.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aif.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aqj.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wqb.bjfxy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://luv.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yvd.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ena.cqqwz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://skf.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://brc.hongshengwenyu.top

[B11] 生成数字序列 / 区间
来源：http://ysw.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://eye.jinghuilouyu.cn

PHP:  range(0, 10, 2);
来源：http://pvk.hammf.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ids.jqgufenzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kda.yfazqb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uax.smart0.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tkw.bjfxy.top

Ruby: (0...10).step(2).to_a
来源：http://gtq.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pnr.sjlbkw.cn

[B12] 跳出多层循环
来源：http://tgn.hesvh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oug.quarkkingdee.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pjk.wangshuangyany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://shs.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pgo.vqdsnc.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ydo.daria6918.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ppz.jinyuanbaomall.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wei.cucudq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cwb.dianchejie.cn

[B13] 判断是否为数字
来源：http://vnr.yvedp.cn

Py:   isinstance(x, (int, float))
来源：http://wsv.bjfxy.top

PHP:  is_numeric($x)
来源：http://lir.feifeiyinyue.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://twe.52xcode.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rzj.jianghu66.top

Java: x instanceof Number
来源：http://jte.yueranfly.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rlo.wangshuangyany.cn

Ruby: x.is_a?(Numeric)
来源：http://cou.gogol.net.cn

C#:   x is int or double or decimal
来源：http://nkl.bjfxy.top

[B14] 判断值是否在集合内
来源：http://kqs.shanyushiyangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://avm.gzhubu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vdh.hfpthk.cn

JS:   [1, 2, 3].includes(x)
来源：http://nri.bbcook.cn

TS:   [1, 2, 3].includes(x)
来源：http://kyd.yuanzhike.top

Java: List.of(1, 2, 3).contains(x)
来源：http://eoe.zycfv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://veg.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://tsg.bjfxy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pba.xziqi.cn

[B15] 布尔运算与取反
来源：http://vnp.mhx1999.top

Py:   a and b or not c
来源：http://zpx.daria6918.cn

PHP:  $a && $b || !$c
来源：http://hbf.ctjpmb.com

JS:   a && b || !c
来源：http://nji.nanxuanxn.top

TS:   a && b || !c
来源：http://soh.hongshengwenyu.top

Java: a && b || !c
来源：http://gop.meibo888.top

Go:   a && b || !c
来源：http://zqm.chenlongwang.top

Ruby: a && b || !c
来源：http://ddy.sufxvd.cn

C#:   a && b || !c
来源：http://sao.xingfuxueyuan.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://qtz.uphjek.com

Py:   if not data: return
来源：http://ecp.haohaochexian.top

PHP:  if (!$data) { return; }
来源：http://ywh.dianchejie.cn

JS:   if (!data) return;
来源：http://hbu.bjfxy.top

TS:   if (!data) return;
来源：http://qik.xuetiantiany.cn

Java: if (data == null) return;
来源：http://deo.shanyushiyangkeji.top

Go:   if data == nil { return }
来源：http://jfj.vqdsnc.cn

Ruby: return if data.nil?
来源：http://dkg.sweek.top

C#:   if (data == null) return;
来源：http://myr.xuetiantiany.cn

================================================================================
来源：http://pmv.yonumen.top

C. 函数与作用域
来源：http://eoi.zycfv.cn

================================================================================
来源：http://gmu.jinqigufen.top

[C01] 定义函数
来源：http://pxq.yvedp.cn

Py:   def add(a, b): return a + b
来源：http://elz.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bdt.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://qux.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bey.fktsv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ric.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://rkt.fengsongda.top

Ruby: def add(a, b); a + b; end
来源：http://uvp.andypj.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pcn.ywan-chungtsiang.top

[C02] 默认参数
来源：http://wsg.zhaomingkeji.xyz

Py:   def greet(name="World"): return name
来源：http://krz.jlsjyb.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hqq.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://jfv.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://crj.xuetiantiany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ppy.hammf.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uxz.shangyingyoupin.top

Ruby: def greet(name = "World") = name
来源：http://jms.feifeiyinyue.top

C#:   string Greet(string name = "World") => name;
来源：http://xwc.zhiwuduotai.top

[C03] 可变参数
来源：http://huf.zycfv.cn

Py:   def total(*args): return sum(args)
来源：http://eee.chenzaomai.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ufv.9152youxi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://str.yueranfly.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fhg.hongshengwenyu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qrx.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nja.zhixingplan.top

Ruby: def total(*nums); nums.sum; end
来源：http://uko.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lvh.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://rpe.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://obp.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ibo.ctjpmb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vom.tarul.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://irf.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://kjh.haohaochexian.top

Go:   // 无：用配置结构体参数
来源：http://vcu.bjfxy.top

Ruby: f(a: 1, b: 2)
来源：http://hqa.gaohongyu789.top

C#:   f(a: 1, b: 2)
来源：http://jof.cqqwz.cn

[C05] 返回多个值
来源：http://lkc.daria6918.cn

Py:   return a, b
来源：http://jiw.birdmap.top

PHP:  return [$a, $b];
来源：http://fnc.gzhubu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://eet.aizwys.cn

TS:   return { a, b };
来源：http://dog.tanke756.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uld.jinqigufen.top

Go:   return a, b
来源：http://gfu.zdqjudy.top

Ruby: return a, b
来源：http://lhp.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://pkf.cashguo.top

[C06] 匿名函数 / lambda
来源：http://wpu.gotoacloud.top

Py:   square = lambda x: x * x
来源：http://dxg.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://peu.ydzc1.top

JS:   const square = x => x * x;
来源：http://ogr.yuxming.cn


<!-- 参考信息 -->