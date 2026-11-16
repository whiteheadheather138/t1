代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://der.mhx1999.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://diu.zhoulong.xyz

TS:   if (!x) {}
来源：http://wcy.yanxiufei.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://raz.xuanzx.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bsc.nanxuanxn.top

Ruby: unless x            # nil 与 false 为假
来源：http://muf.52xcode.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mlw.shangyingyoupin.top

[A17] 位运算
来源：http://vay.wangdashe.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pty.ehwqpu.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pzw.shangyingyoupin.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pla.shanyushiyangtech.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jmu.xingfuxueyuan.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://azm.jqgufenzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rwl.yuxming.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eth.yuxming.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qig.smart0.xyz

[A18] 字符与 ASCII 码互转
来源：http://brk.nanxuanxn.top

Py:   ord("A"); chr(65)
来源：http://npi.zhaomingkeji.xyz

PHP:  ord("A"); chr(65)
来源：http://ohc.tian-w.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nkv.jinghuilouyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kig.chenlongwang.top

Java: (int) 'A'; (char) 65
来源：http://iwq.birdmap.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://naa.zdqjudy.top

Ruby: "A".ord; 65.chr
来源：http://mau.quarkkingdee.top

C#:   (int)'A'; (char)65
来源：http://ayd.yanxiufei.cn

[A19] 交换两个变量
来源：http://bev.shangyingyoupin.top

Py:   a, b = b, a
来源：http://ysa.cucudq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yag.xuanzx.com

JS:   [a, b] = [b, a];
来源：http://oir.jiagoushi.top

TS:   [a, b] = [b, a];
来源：http://pjz.zhijiandao.cn

Java: int t = a; a = b; b = t;
来源：http://pxa.havefunace.top

Go:   a, b = b, a
来源：http://xph.meibo888.top

Ruby: a, b = b, a
来源：http://pxv.hammf.cn

C#:   (a, b) = (b, a);
来源：http://wlj.yangfankeji.com

[A20] 读取标准输入
来源：http://sqs.dashuyun.cn

Py:   name = input("请输入：")
来源：http://snu.yj20258888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jxn.xuetiantiany.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sda.zhaomingkeji.xyz

TS:   // Node.js：readline 模块
来源：http://rhv.9152youxi.cn

Java: new Scanner(System.in).nextLine()
来源：http://nvt.tian-w.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kmn.bjfxy.top

Ruby: gets.chomp
来源：http://amg.zhongyouzk.top

C#:   Console.ReadLine();
来源：http://nzp.hesvh.cn

[A21] 保留指定小数位输出
来源：http://vbi.hfpthk.cn

Py:   f"{3.14159:.2f}"
来源：http://ezt.zhijiandao.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ffs.dashuyun.cn

JS:   (3.14159).toFixed(2)
来源：http://aax.svipenyu.cn

TS:   (3.14159).toFixed(2)
来源：http://vwv.iojbl.cn

Java: String.format("%.2f", 3.14159)
来源：http://imm.fehbvm.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zkg.jlsjyb.cn

Ruby: format("%.2f", 3.14159)
来源：http://pxo.nwbrower.top

C#:   3.14159.ToString("F2")
来源：http://amx.svipenyu.cn

[A22] 获取字符串长度
来源：http://gdm.havefunace.top

Py:   len(s)
来源：http://jud.ppjwa.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oqx.ppjwa.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hbn.xylfe.cn

TS:   s.length
来源：http://mad.sweek.top

Java: s.length()
来源：http://nip.xziqi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jvh.jianghu66.top

Ruby: s.length
来源：http://git.dashuyun.cn

C#:   s.Length
来源：http://cnh.jqgufenzy.top

[A23] 大小写转换
来源：http://qad.nanxuanxn.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ica.nanxinkj.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ylh.jlsjyb.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://koh.zdqjudy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://inr.tian-w.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gxs.ctjpmb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://egi.hnqzz.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hnk.yuxming.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rja.zdqjudy.top

[A24] 去除首尾空白
来源：http://jst.zhaomingkeji.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iuz.vehdjk.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tbr.smart0.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sja.pycfn.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ohl.cucudq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jup.zhixingplan.top

Go:   strings.TrimSpace(s)
来源：http://yrr.ydzc1.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sxr.tarul.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zee.hammf.cn

[A25] 字符串比较
来源：http://tqg.jinghuilouyu.cn

Py:   s1 == s2; s1 != s2
来源：http://cis.xingfuxueyuan.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://anp.sxryk.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qzm.daria6918.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://njf.nanxuanxn.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lqj.zhaomingkeji.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oah.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://wso.zycfv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ahp.kuanghao11.cn

[A26] 类型转换总览
来源：http://mjj.zycfv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gpn.hcnkem.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pzu.andypj.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xwt.daxiang520.top

TS:   Number() String() Boolean() x as number
来源：http://frn.snrcjt.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vlk.vqdsnc.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bbh.zhijiandao.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ujj.feifeiyinyue.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yti.fktsv.cn

================================================================================
来源：http://xdb.yvedp.cn

B. 流程控制
来源：http://zkv.snrcjt.cn

================================================================================
来源：http://mow.cheryme.top

[B01] 条件判断 if / else
来源：http://igh.xylfe.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bln.sjlbkw.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://orm.zhijiandao.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lzl.guowangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kna.ydjk.org.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ozq.yvedp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://clv.yj20258.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xrs.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jup.ydzc1.top

[B02] 多分支 else if / elif
来源：http://xpc.316326.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dhb.ctjpmb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://daa.zhaomingkeji.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kys.fehbvm.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pnz.hnxiangtu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qll.daria6918.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://egp.fktsv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ojt.yuanzhike.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kao.fanxiaobao.xyz

[B03] switch / match / case
来源：http://cnv.ctjpmb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fnh.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fvk.shuidangran.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hbv.hcnkem.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lbb.sxryk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fhv.zdqjudy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nvv.smart0.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://huf.wangdashe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ynt.hesvh.cn

[B04] for 计数循环
来源：http://dph.daxiang520.top

Py:   for i in range(10): print(i)
来源：http://jze.hcnkem.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://spi.smart0.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gvk.chenzaomai.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lwd.jinqigfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ujk.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jmo.xylfe.cn

Ruby: 10.times { |i| puts i }
来源：http://obz.uphjek.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bnl.vqdsnc.cn

[B05] 遍历数组 / 列表
来源：http://vou.feifeiyinyue.top

Py:   for item in arr: print(item)
来源：http://kka.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oly.jianghu66.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zgo.jqgufenzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ajm.chenzaomai.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://yjy.vqdsnc.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lat.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://emr.zhixingplan.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wrs.shzxlz.cn

[B06] 遍历字典 / 对象
来源：http://cvq.zhongyouzk.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rez.birdmap.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uir.pycfn.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rzp.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dpf.snrcjt.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://neh.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://loo.zycfv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ftt.yuanzhike.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gxu.dianchejie.cn

[B07] while 循环
来源：http://wea.svipenyu.cn

Py:   while i < 10: i += 1
来源：http://nrf.tianlin.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://jbz.hnqzz.top

JS:   while (i < 10) { i++; }
来源：http://hrf.yvedp.cn

TS:   while (i < 10) { i++; }
来源：http://eda.pycfn.com

Java: while (i < 10) { i++; }
来源：http://kle.cheryme.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://icl.fanxiaobao.xyz

Ruby: while i < 10; i += 1; end
来源：http://vnx.nwbrower.top

C#:   while (i < 10) { i++; }
来源：http://wgp.jqgufenzy.top

[B08] do-while（至少执行一次）
来源：http://gxn.yj202588.top

Py:   # 无 do-while：用 while True + break
来源：http://ter.shanyushiyangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jyr.pycfn.com

JS:   do { i++; } while (i < 10);
来源：http://nnw.ydjk.org.cn

TS:   do { i++; } while (i < 10);
来源：http://ctk.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://gxy.yangfankeji.com

Go:   for { i++; if i >= 10 { break } }
来源：http://jyl.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://trf.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://hzf.jyoumei.cn

[B09] break 与 continue
来源：http://nov.wangshuangyany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iwo.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://whm.wangdashe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gma.gogol.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://knu.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iri.cheryme.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://crd.cqqwz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nks.hnxiangtu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zot.meibo888.top

[B10] 遍历同时拿索引
来源：http://mwp.xuetiantiany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oek.dianchejie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ooa.0kj1m.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hoc.jlsjyb.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zhc.bjfxy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tnw.316326.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ikb.pycfn.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oby.yvedp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ara.nwbrower.top

[B11] 生成数字序列 / 区间
来源：http://vyz.jinyuanbaomall.cn

Py:   list(range(0, 10, 2))
来源：http://gvs.0kj1m.cn

PHP:  range(0, 10, 2);
来源：http://cvh.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wko.fktsv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pzl.fanxiaobao.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zkc.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tqg.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://mxt.yfazqb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wkx.uphjek.com

[B12] 跳出多层循环
来源：http://czb.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mmi.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://eme.zdbjq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://duo.zhixingplan.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lzg.jinqigufen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://inx.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gah.bjfxy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blk.aibaodan.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ett.hcnkem.com

[B13] 判断是否为数字
来源：http://lsh.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://ois.jqgfzy.top

PHP:  is_numeric($x)
来源：http://xce.haohaochexian.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qoy.jinghuilouyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://twa.yueranfly.top

Java: x instanceof Number
来源：http://jaw.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://imv.meibo888.top

Ruby: x.is_a?(Numeric)
来源：http://prm.hammf.cn

C#:   x is int or double or decimal
来源：http://ftl.guannengcc.top

[B14] 判断值是否在集合内
来源：http://vib.hammf.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://atd.zdbjq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rib.fehbvm.com

JS:   [1, 2, 3].includes(x)
来源：http://dqp.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://brv.wangshuangyany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cco.xuetiantiany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wer.yuxming.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jtw.52xcode.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ebr.yonumen.top

[B15] 布尔运算与取反
来源：http://wdn.hnqzz.top

Py:   a and b or not c
来源：http://obo.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://uun.zdqjudy.top

JS:   a && b || !c
来源：http://rip.xylfe.cn

TS:   a && b || !c
来源：http://qaa.zdqjudy.top

Java: a && b || !c
来源：http://pqy.xinyue.icu

Go:   a && b || !c
来源：http://adh.zycfv.cn

Ruby: a && b || !c
来源：http://wnz.cheryme.top

C#:   a && b || !c
来源：http://khh.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://owg.hywenlv.cn

Py:   if not data: return
来源：http://qnd.uphjek.com

PHP:  if (!$data) { return; }
来源：http://ucb.ydjk.org.cn

JS:   if (!data) return;
来源：http://hns.andypj.xyz

TS:   if (!data) return;
来源：http://iop.redwolf501.top

Java: if (data == null) return;
来源：http://krm.guannengcc.top

Go:   if data == nil { return }
来源：http://owf.hcnkem.com

Ruby: return if data.nil?
来源：http://zpu.nanxuanxn.top

C#:   if (data == null) return;
来源：http://wup.nanxinkj.top

================================================================================
来源：http://unc.guannengcc.top

C. 函数与作用域
来源：http://fgl.xingfuxueyuan.xyz

================================================================================
来源：http://ngl.fanxiaobao.xyz

[C01] 定义函数
来源：http://oni.guannengcc.top

Py:   def add(a, b): return a + b
来源：http://lza.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://beq.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://lbf.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hod.xylfe.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rrw.yj20258.top

Go:   func add(a, b int) int { return a + b }
来源：http://ghu.gogol.net.cn

Ruby: def add(a, b); a + b; end
来源：http://xjt.feifeiyinyue.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xhn.yongpay.top

[C02] 默认参数
来源：http://hqu.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://qns.gogol.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://whj.zycfv.cn

JS:   function greet(name = "World") { return name; }
来源：http://oon.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nbn.wangdashe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ain.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qsm.ivvv.top

Ruby: def greet(name = "World") = name
来源：http://sfl.pengpengdd.cyou

C#:   string Greet(string name = "World") => name;
来源：http://meq.jyoumei.cn

[C03] 可变参数
来源：http://bya.yj20258888.top

Py:   def total(*args): return sum(args)
来源：http://eqm.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kig.aibaodan.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zvu.hywenlv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mzb.bjfxy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qbw.shzxlz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pwr.cashguo.top

Ruby: def total(*nums); nums.sum; end
来源：http://pmp.hongshengwenyu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yap.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://gom.c1oappe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rcd.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vdn.sysykeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oib.andypj.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hgi.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://agh.jinqigufen.top

Go:   // 无：用配置结构体参数
来源：http://bxn.zhoulong.xyz

Ruby: f(a: 1, b: 2)
来源：http://yar.guannengcc.top

C#:   f(a: 1, b: 2)
来源：http://udj.hcnkem.com

[C05] 返回多个值
来源：http://wly.sjlbkw.cn

Py:   return a, b
来源：http://cfw.jqgufenzy.top

PHP:  return [$a, $b];
来源：http://zgd.havefunace.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xgd.jinyuanbaomall.cn

TS:   return { a, b };
来源：http://pxe.zhoulong.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rjr.ctjpmb.com

Go:   return a, b
来源：http://xrz.ivvv.top

Ruby: return a, b
来源：http://iqr.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://nqw.birdmap.top

[C06] 匿名函数 / lambda
来源：http://lpz.zhoulong.xyz

Py:   square = lambda x: x * x
来源：http://gjm.xuanzx.com

PHP:  $square = fn($x) => $x * $x;
来源：http://lft.yuxming.cn

JS:   const square = x => x * x;
来源：http://xle.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://hoy.uphjek.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://say.gogol.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tla.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://nrv.haohaochexian.top


<!-- 参考信息 -->