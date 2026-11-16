代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lao.yonumen.top

Ruby: unless x            # nil 与 false 为假
来源：http://pfq.yueranfly.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uxk.svipenyu.cn

[A17] 位运算
来源：http://lbh.ybcxt.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mcv.yongpay.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wuw.jqgfzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oob.zycfv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://paz.chenlongwang.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hic.daria6918.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yow.sjlbkw.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bqp.ydzc1.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yyl.c1oappe.top

[A18] 字符与 ASCII 码互转
来源：http://umh.nanxuanxn.top

Py:   ord("A"); chr(65)
来源：http://eci.epnwcf.com

PHP:  ord("A"); chr(65)
来源：http://pto.cucudq.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://shj.cucudq.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qij.9152youxi.cn

Java: (int) 'A'; (char) 65
来源：http://ner.shzxlz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qgb.hnxiangtu.top

Ruby: "A".ord; 65.chr
来源：http://dqq.meibo888.top

C#:   (int)'A'; (char)65
来源：http://nrd.tanke756.top

[A19] 交换两个变量
来源：http://oez.yuanzhike.top

Py:   a, b = b, a
来源：http://xwj.xylfe.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rba.snrcjt.cn

JS:   [a, b] = [b, a];
来源：http://ycn.wangshuangyany.cn

TS:   [a, b] = [b, a];
来源：http://xte.gzhubu.top

Java: int t = a; a = b; b = t;
来源：http://ywn.dashuyun.cn

Go:   a, b = b, a
来源：http://bmx.hcnkem.com

Ruby: a, b = b, a
来源：http://uzt.yj20258.top

C#:   (a, b) = (b, a);
来源：http://mzp.chenzaomai.com

[A20] 读取标准输入
来源：http://dhi.ydjk.org.cn

Py:   name = input("请输入：")
来源：http://goo.jinyuanbaomall.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tou.xylfe.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bxf.shuidangran.top

TS:   // Node.js：readline 模块
来源：http://sww.sysykeji.top

Java: new Scanner(System.in).nextLine()
来源：http://njg.zycfv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gta.bjfxy.top

Ruby: gets.chomp
来源：http://rpi.ywan-chungtsiang.top

C#:   Console.ReadLine();
来源：http://ect.chenjidiqi.icu

[A21] 保留指定小数位输出
来源：http://gwr.tian-w.cn

Py:   f"{3.14159:.2f}"
来源：http://cbr.bjfxy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nwb.hcnkem.com

JS:   (3.14159).toFixed(2)
来源：http://tmt.ybcxt.top

TS:   (3.14159).toFixed(2)
来源：http://kga.gaohongyu789.top

Java: String.format("%.2f", 3.14159)
来源：http://gxh.havefunace.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://met.nanxuanxn.top

Ruby: format("%.2f", 3.14159)
来源：http://sgc.ydzc1.top

C#:   3.14159.ToString("F2")
来源：http://ijb.nanxuanxn.top

[A22] 获取字符串长度
来源：http://xeq.tianlin.xyz

Py:   len(s)
来源：http://det.xinyue.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iqz.jinqigufen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ghf.jinyuanbaomall.cn

TS:   s.length
来源：http://lwt.kuanghao11.cn

Java: s.length()
来源：http://gyc.bbcook.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pon.fengsongda.top

Ruby: s.length
来源：http://qvn.gogol.net.cn

C#:   s.Length
来源：http://zfm.dianchejie.cn

[A23] 大小写转换
来源：http://fxc.ppjwa.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qzh.0kj1m.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pyk.cucudq.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tpo.chenlongwang.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kgi.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ktx.cheryme.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kyf.shanyushiyangtech.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://huu.yj202588.top

C#:   s.ToUpper(); s.ToLower()
来源：http://tya.sysykeji.top

[A24] 去除首尾空白
来源：http://joh.cqqwz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ouo.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iwy.zycfv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sdw.ehwqpu.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wcm.9152youxi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jyb.shanyushiyangkeji.top

Go:   strings.TrimSpace(s)
来源：http://ymm.gaohongyu789.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lhq.sysykeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://unv.bbcook.cn

[A25] 字符串比较
来源：http://lba.sweek.top

Py:   s1 == s2; s1 != s2
来源：http://hxs.cqqwz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bod.ybcxt.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gda.zycfv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wae.xziqi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lca.guowangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iis.hesvh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hbh.cqqwz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jdp.fktsv.cn

[A26] 类型转换总览
来源：http://qdr.fanxiaobao.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://efh.0kj1m.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lmd.aizwys.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vmd.zhiwuduotai.top

TS:   Number() String() Boolean() x as number
来源：http://alt.mhx1999.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rgw.jlsjyb.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pxf.cqqwz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tbc.zycfv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qzz.chenlongwang.top

================================================================================
来源：http://dpu.ybcxt.top

B. 流程控制
来源：http://kvd.redwolf501.top

================================================================================
来源：http://ozq.xinyue.icu

[B01] 条件判断 if / else
来源：http://bpo.uphjek.com

Py:   result = "正" if x > 0 else "非正"
来源：http://kxz.hnxiangtu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lsb.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uge.shangyingyoupin.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pye.tanke756.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://uah.gaohongyu789.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hbr.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nxz.bbcook.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bbw.shuidangran.top

[B02] 多分支 else if / elif
来源：http://dyr.ydzc1.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wlt.daria6918.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bno.hfpthk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lxr.pycfn.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tki.yuxming.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://meh.pycfn.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ljn.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sif.chenzaomai.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qpl.meibo888.top

[B03] switch / match / case
来源：http://apv.hongshengwenyu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://snm.zhongyouzk.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fvi.zycfv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sfd.guowangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dro.chenjidiqi.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://arl.mhx1999.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lis.daxiang520.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://psg.zhaomingkeji.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vix.zhongyouzk.top

[B04] for 计数循环
来源：http://wbw.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://kih.feifeiyinyue.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://riv.hammf.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lqg.ywan-chungtsiang.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hzp.shanyushiyangtech.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://frr.yuxming.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ubk.redwolf501.top

Ruby: 10.times { |i| puts i }
来源：http://xst.yj20258.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zxb.yanxiufei.cn

[B05] 遍历数组 / 列表
来源：http://lxv.fengsongda.top

Py:   for item in arr: print(item)
来源：http://giz.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fis.jyoumei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vcd.shangyingyoupin.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hhf.gzhubu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rgu.quarkkingdee.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://emk.epnwcf.com

Ruby: arr.each { |item| puts item }
来源：http://oyn.bjfxy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mee.shzxlz.cn

[B06] 遍历字典 / 对象
来源：http://lpz.nanxuanxn.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yih.hysaishi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mkq.tanke756.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jrp.zycfv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lxc.daxiang520.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mxt.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tyg.aibaodan.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yle.0kj1m.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fvc.jyoumei.cn

[B07] while 循环
来源：http://njn.daxiang520.top

Py:   while i < 10: i += 1
来源：http://qqj.daria6918.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bep.cqqwz.cn

JS:   while (i < 10) { i++; }
来源：http://jpr.jianghu66.top

TS:   while (i < 10) { i++; }
来源：http://hvd.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://fiw.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uvc.vehdjk.com

Ruby: while i < 10; i += 1; end
来源：http://mjc.hammf.cn

C#:   while (i < 10) { i++; }
来源：http://yme.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://rya.ctjpmb.com

Py:   # 无 do-while：用 while True + break
来源：http://cde.redwolf501.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rbj.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://nye.redwolf501.top

TS:   do { i++; } while (i < 10);
来源：http://psf.yuxming.cn

Java: do { i++; } while (i < 10);
来源：http://exc.hcnkem.com

Go:   for { i++; if i >= 10 { break } }
来源：http://iub.aibaodan.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hyy.chenzaomai.com

C#:   do { i++; } while (i < 10);
来源：http://cdq.nanxuanxn.top

[B09] break 与 continue
来源：http://qvy.bjfxy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://day.dashuyun.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pun.tanke756.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cnw.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://atw.feifeiyinyue.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mnu.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ywm.shanyushiyangtech.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://byb.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ezt.tianlin.xyz

[B10] 遍历同时拿索引
来源：http://pfg.mhx1999.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cma.smart0.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cqr.0kj1m.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://heo.shangyingyoupin.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ldg.ydzc1.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://abu.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dlr.gogol.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jzw.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fzg.zhongyouzk.top

[B11] 生成数字序列 / 区间
来源：http://xod.tian-w.cn

Py:   list(range(0, 10, 2))
来源：http://svj.hysaishi.cn

PHP:  range(0, 10, 2);
来源：http://nsp.gogol.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dwe.shuidangran.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ocv.yueranfly.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gxw.cashguo.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wcq.tarul.cn

Ruby: (0...10).step(2).to_a
来源：http://nqd.andypj.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rka.jyoumei.cn

[B12] 跳出多层循环
来源：http://bhd.xziqi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nru.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nev.sxryk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lnb.cashguo.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nus.zhaomingkeji.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://czx.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oiv.jqgfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lam.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xun.xylfe.cn

[B13] 判断是否为数字
来源：http://qnx.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://bfi.tarul.cn

PHP:  is_numeric($x)
来源：http://ihu.guowangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wyh.pycfn.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fmr.dashuyun.cn

Java: x instanceof Number
来源：http://buq.hywenlv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rdv.svipenyu.cn

Ruby: x.is_a?(Numeric)
来源：http://ppw.ctjpmb.com

C#:   x is int or double or decimal
来源：http://nfe.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://uof.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ifn.xinyue.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://azu.ydzc1.top

JS:   [1, 2, 3].includes(x)
来源：http://aho.ctjpmb.com

TS:   [1, 2, 3].includes(x)
来源：http://kye.guowangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://adp.tarul.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tip.smart0.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://sko.hfpthk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://myh.snrcjt.cn

[B15] 布尔运算与取反
来源：http://lcd.xingfuxueyuan.xyz

Py:   a and b or not c
来源：http://hnd.zhijiandao.cn

PHP:  $a && $b || !$c
来源：http://kdf.pengpengdd.cyou

JS:   a && b || !c
来源：http://hyo.mhx1999.top

TS:   a && b || !c
来源：http://kmm.0kj1m.cn

Java: a && b || !c
来源：http://ujx.hammf.cn

Go:   a && b || !c
来源：http://nke.52xcode.cn

Ruby: a && b || !c
来源：http://epy.shanyushiyangkeji.top

C#:   a && b || !c
来源：http://rdt.birdmap.top

[B16] 卫语句：不满足条件提前返回
来源：http://dqv.vqdsnc.cn

Py:   if not data: return
来源：http://tka.mhx1999.top

PHP:  if (!$data) { return; }
来源：http://qfc.gaohongyu789.top

JS:   if (!data) return;
来源：http://wio.gzhubu.top

TS:   if (!data) return;
来源：http://vtn.hfpthk.cn

Java: if (data == null) return;
来源：http://rfp.hywenlv.cn

Go:   if data == nil { return }
来源：http://itc.tianlin.xyz

Ruby: return if data.nil?
来源：http://tlh.cqqwz.cn

C#:   if (data == null) return;
来源：http://bgd.hfpthk.cn

================================================================================
来源：http://kds.hywenlv.cn

C. 函数与作用域
来源：http://dgh.daria6918.cn

================================================================================
来源：http://gok.shzxlz.cn

[C01] 定义函数
来源：http://zbh.sjlbkw.cn

Py:   def add(a, b): return a + b
来源：http://mdy.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gdt.xuanzx.com

JS:   function add(a, b) { return a + b; }
来源：http://ifx.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vfn.ywan-chungtsiang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cqi.zhoulong.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://add.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://aqn.zhengqikj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jpa.xinyue.icu

[C02] 默认参数
来源：http://wxt.zhaomingkeji.xyz

Py:   def greet(name="World"): return name
来源：http://twk.sjlbkw.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dfs.zhijiandao.cn

JS:   function greet(name = "World") { return name; }
来源：http://qij.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hay.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://vdb.9152youxi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ofu.xuetiantiany.cn

Ruby: def greet(name = "World") = name
来源：http://iyy.meibo888.top

C#:   string Greet(string name = "World") => name;
来源：http://pbc.ydzc1.top

[C03] 可变参数
来源：http://wjy.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://jyk.zycfv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wac.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vec.hysaishi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hxr.sweek.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jnj.wangshuangyany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mtv.vehdjk.com

Ruby: def total(*nums); nums.sum; end
来源：http://lzf.yfazqb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wti.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://fux.meibo888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yev.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eqk.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://abs.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iqj.xziqi.cn

Java: // 无：用 Builder 模式或 record
来源：http://bzd.nanxuanxn.top

Go:   // 无：用配置结构体参数
来源：http://aht.guowangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://eoz.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://mzz.sufxvd.cn

[C05] 返回多个值
来源：http://qtr.redwolf501.top

Py:   return a, b
来源：http://von.ywan-chungtsiang.top

PHP:  return [$a, $b];
来源：http://dyu.yj20258.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ugt.yj20258.top

TS:   return { a, b };
来源：http://qml.yangfankeji.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uml.epnwcf.com

Go:   return a, b
来源：http://avi.zhiwuduotai.top

Ruby: return a, b
来源：http://fgx.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://qnr.chenjidiqi.icu

[C06] 匿名函数 / lambda
来源：http://tbs.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://jsl.mhx1999.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nbq.shanyushiyangtech.top

JS:   const square = x => x * x;
来源：http://yql.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://ver.chenlongwang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://elh.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://zii.birdmap.top

Ruby: square = ->(x) { x * x }
来源：http://grr.yvedp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yuy.jianghu66.top

[C07] 把函数作为参数传入
来源：http://qzn.ydzc1.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pip.kuanghao11.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kgm.guowangkeji.top


<!-- 参考信息 -->