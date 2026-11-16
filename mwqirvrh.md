代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ybg.yfazqb.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rsh.wangshuangyany.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ixw.sweek.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qgj.cheryme.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hkr.iojbl.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ahh.hywenlv.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mdt.cqqwz.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://unz.nanxinkj.top

[A18] 字符与 ASCII 码互转
来源：http://lwm.hywenlv.cn

Py:   ord("A"); chr(65)
来源：http://pbd.jinghuilouyu.cn

PHP:  ord("A"); chr(65)
来源：http://xtv.epnwcf.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vuh.xuanzx.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://duu.hcnkem.com

Java: (int) 'A'; (char) 65
来源：http://yac.mhx1999.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gkl.ydjk.org.cn

Ruby: "A".ord; 65.chr
来源：http://xrh.52xcode.cn

C#:   (int)'A'; (char)65
来源：http://dbq.zhengqikj.top

[A19] 交换两个变量
来源：http://mwo.hesvh.cn

Py:   a, b = b, a
来源：http://lyk.hywenlv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bmy.jianghu66.top

JS:   [a, b] = [b, a];
来源：http://dqh.yuanzhike.top

TS:   [a, b] = [b, a];
来源：http://con.aizwys.cn

Java: int t = a; a = b; b = t;
来源：http://kbb.hywenlv.cn

Go:   a, b = b, a
来源：http://gxn.jqgufenzy.top

Ruby: a, b = b, a
来源：http://pvd.zdqjudy.top

C#:   (a, b) = (b, a);
来源：http://djz.zycfv.cn

[A20] 读取标准输入
来源：http://fyq.hysaishi.cn

Py:   name = input("请输入：")
来源：http://mui.jiagoushi.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vbc.tarul.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hqu.sxryk.cn

TS:   // Node.js：readline 模块
来源：http://iwj.ydzc1.top

Java: new Scanner(System.in).nextLine()
来源：http://atx.havefunace.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dib.hesvh.cn

Ruby: gets.chomp
来源：http://frr.chenjidiqi.icu

C#:   Console.ReadLine();
来源：http://ybw.vehdjk.com

[A21] 保留指定小数位输出
来源：http://jss.fzhhl.top

Py:   f"{3.14159:.2f}"
来源：http://fmr.zdbjq.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qok.zhengqikj.top

JS:   (3.14159).toFixed(2)
来源：http://pmz.zhongyouzk.top

TS:   (3.14159).toFixed(2)
来源：http://jeh.sweek.top

Java: String.format("%.2f", 3.14159)
来源：http://njw.fktsv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ych.aizwys.cn

Ruby: format("%.2f", 3.14159)
来源：http://btw.birdmap.top

C#:   3.14159.ToString("F2")
来源：http://hwr.xinyue.icu

[A22] 获取字符串长度
来源：http://ufk.yfazqb.com

Py:   len(s)
来源：http://awn.epnwcf.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://frd.yangfankeji.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eke.meibo888.top

TS:   s.length
来源：http://pfy.cheryme.top

Java: s.length()
来源：http://ais.xziqi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jjv.guowangkeji.top

Ruby: s.length
来源：http://usb.vqdsnc.cn

C#:   s.Length
来源：http://ced.52xcode.cn

[A23] 大小写转换
来源：http://qmn.52xcode.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wvf.yfazqb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vdl.daria6918.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vrj.xingfuxueyuan.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wpa.wangdashe.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://akn.cdnleiting.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cen.c1oappe.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://odf.c1oappe.top

C#:   s.ToUpper(); s.ToLower()
来源：http://roi.fktsv.cn

[A24] 去除首尾空白
来源：http://mfn.gogol.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jyi.uphjek.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rvw.redwolf501.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zth.zdqjudy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://krq.jinqigufen.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bbc.daxiang520.top

Go:   strings.TrimSpace(s)
来源：http://qdw.ppjwa.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zhe.epnwcf.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://loz.yj20258.top

[A25] 字符串比较
来源：http://ljj.wangshuangyany.cn

Py:   s1 == s2; s1 != s2
来源：http://occ.gotoacloud.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xiz.meibo888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yyo.yuanzhike.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zbq.pycfn.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mxd.bbcook.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lqd.xziqi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dpo.hnqzz.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tjd.cheryme.top

[A26] 类型转换总览
来源：http://wvs.xingfuxueyuan.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://djk.yj202588.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tzn.fktsv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dkl.zhoulong.xyz

TS:   Number() String() Boolean() x as number
来源：http://uww.cqqwz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://udt.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dax.fktsv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ucc.jinqigfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jff.tanke756.top

================================================================================
来源：http://zdq.ctjpmb.com

B. 流程控制
来源：http://pok.dashuyun.cn

================================================================================
来源：http://net.mhx1999.top

[B01] 条件判断 if / else
来源：http://dcp.zhoulong.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://hak.sufxvd.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oqe.haohaochexian.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fnn.gogol.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bid.ydjk.org.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tur.uphjek.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ahf.316326.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tfv.zhoulong.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hzi.gotoacloud.top

[B02] 多分支 else if / elif
来源：http://hsi.jqgufenzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cee.aizwys.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nbn.hcnkem.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zua.fktsv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zaz.xuetiantiany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://goy.ehwqpu.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gem.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rrf.316326.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uyc.svipenyu.cn

[B03] switch / match / case
来源：http://njb.ydzc1.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kgj.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xna.yongpay.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rkk.xinyue.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://apf.tanke756.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gsq.yj20258888.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tjk.cashguo.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ldk.bjfxy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ogl.shangyingyoupin.top

[B04] for 计数循环
来源：http://vbf.snrcjt.cn

Py:   for i in range(10): print(i)
来源：http://mfr.zhongyouzk.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ouj.jqgufenzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rgj.cucudq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hqt.shanyushiyangtech.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://amo.dianchejie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://upp.dianchejie.cn

Ruby: 10.times { |i| puts i }
来源：http://pbh.xylfe.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hgf.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://ohf.vehdjk.com

Py:   for item in arr: print(item)
来源：http://tth.shuidangran.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bit.sufxvd.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nmf.ywan-chungtsiang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://csr.aizwys.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vjf.shzxlz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gez.uphjek.com

Ruby: arr.each { |item| puts item }
来源：http://cou.zhaomingkeji.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ksz.jiagoushi.top

[B06] 遍历字典 / 对象
来源：http://gpa.hesvh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bem.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vbq.jinqigufen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oon.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://krj.sysykeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nbt.gaohongyu789.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jnp.svipenyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yxc.iojbl.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uus.cucudq.cn

[B07] while 循环
来源：http://otu.hysaishi.cn

Py:   while i < 10: i += 1
来源：http://vdl.sufxvd.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nxk.aizwys.cn

JS:   while (i < 10) { i++; }
来源：http://njm.jlsjyb.cn

TS:   while (i < 10) { i++; }
来源：http://tgp.feifeiyinyue.top

Java: while (i < 10) { i++; }
来源：http://mcm.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://khd.dashuyun.cn

Ruby: while i < 10; i += 1; end
来源：http://oyl.iojbl.cn

C#:   while (i < 10) { i++; }
来源：http://byn.shanyushiyangtech.top

[B08] do-while（至少执行一次）
来源：http://les.yanxiufei.cn

Py:   # 无 do-while：用 while True + break
来源：http://xat.gaohongyu789.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ivf.yvedp.cn

JS:   do { i++; } while (i < 10);
来源：http://gbu.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://olg.uphjek.com

Java: do { i++; } while (i < 10);
来源：http://evt.jinqigfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qzi.zhijiandao.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wlx.nwbrower.top

C#:   do { i++; } while (i < 10);
来源：http://yky.daxiang520.top

[B09] break 与 continue
来源：http://cdr.cashguo.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://awh.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zbk.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ubd.gotoacloud.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yvk.feifeiyinyue.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gqk.yangfankeji.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vgv.gotoacloud.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mqq.hnqzz.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rwc.svipenyu.cn

[B10] 遍历同时拿索引
来源：http://zra.yueranfly.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xqa.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://grb.ydzc1.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pgr.zycfv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qxf.0kj1m.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lgx.zycfv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pdq.xuetiantiany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tuh.gotoacloud.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fak.zhiwuduotai.top

[B11] 生成数字序列 / 区间
来源：http://lkr.zycfv.cn

Py:   list(range(0, 10, 2))
来源：http://smp.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://nlh.tarul.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hlp.ivvv.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bls.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qqt.nanxuanxn.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gnl.hnxiangtu.top

Ruby: (0...10).step(2).to_a
来源：http://hcz.jiagoushi.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nrw.birdmap.top

[B12] 跳出多层循环
来源：http://rkq.yuxming.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qyc.sxryk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zah.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://biz.aibaodan.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iqy.pycfn.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xve.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bcx.vqdsnc.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dmh.xuanzx.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nyr.vehdjk.com

[B13] 判断是否为数字
来源：http://hzy.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://koi.9152youxi.cn

PHP:  is_numeric($x)
来源：http://znl.hysaishi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cjj.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qyy.hnqzz.top

Java: x instanceof Number
来源：http://ilw.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zvi.feifeiyinyue.top

Ruby: x.is_a?(Numeric)
来源：http://voz.aizwys.cn

C#:   x is int or double or decimal
来源：http://cqe.hesvh.cn

[B14] 判断值是否在集合内
来源：http://jht.cheryme.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wcf.xziqi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fkx.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://amx.guannengcc.top

TS:   [1, 2, 3].includes(x)
来源：http://psk.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ubp.0kj1m.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://brg.tianlin.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://eni.cqqwz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tfo.haohaochexian.top

[B15] 布尔运算与取反
来源：http://rwy.pycfn.com

Py:   a and b or not c
来源：http://kox.sweek.top

PHP:  $a && $b || !$c
来源：http://jgk.snrcjt.cn

JS:   a && b || !c
来源：http://nkn.cashguo.top

TS:   a && b || !c
来源：http://wor.nwbrower.top

Java: a && b || !c
来源：http://cxh.hongshengwenyu.top

Go:   a && b || !c
来源：http://vex.jinqigfzy.top

Ruby: a && b || !c
来源：http://gtl.fehbvm.com

C#:   a && b || !c
来源：http://vpf.hywenlv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ucz.zhoulong.xyz

Py:   if not data: return
来源：http://kkg.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://pft.tanke756.top

JS:   if (!data) return;
来源：http://tgt.aizwys.cn

TS:   if (!data) return;
来源：http://qrf.c1oappe.top

Java: if (data == null) return;
来源：http://hqt.aizwys.cn

Go:   if data == nil { return }
来源：http://rpw.jinqigfzy.top

Ruby: return if data.nil?
来源：http://qde.hywenlv.cn

C#:   if (data == null) return;
来源：http://dev.jinghuilouyu.cn

================================================================================
来源：http://osh.ppjwa.cn

C. 函数与作用域
来源：http://jsh.yj20258888.top

================================================================================
来源：http://nei.shanyushiyangtech.top

[C01] 定义函数
来源：http://apg.yonumen.top

Py:   def add(a, b): return a + b
来源：http://gqh.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hyq.ydjk.org.cn

JS:   function add(a, b) { return a + b; }
来源：http://dfb.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://inu.snrcjt.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hxr.hnqzz.top

Go:   func add(a, b int) int { return a + b }
来源：http://ret.shanyushiyangtech.top

Ruby: def add(a, b); a + b; end
来源：http://jyz.mhx1999.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wom.xylfe.cn

[C02] 默认参数
来源：http://aml.jianghu66.top

Py:   def greet(name="World"): return name
来源：http://fmj.nwbrower.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zej.pycfn.com

JS:   function greet(name = "World") { return name; }
来源：http://vqp.cheryme.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zam.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wur.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pus.iojbl.cn

Ruby: def greet(name = "World") = name
来源：http://uzz.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://zce.zdbjq.cn

[C03] 可变参数
来源：http://srt.yongpay.top

Py:   def total(*args): return sum(args)
来源：http://how.zhaomingkeji.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tcx.jiagoushi.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wqq.tian-w.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sdl.ydzc1.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gau.jqgufenzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cmt.sysykeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://yvr.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jyv.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://hoy.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ocl.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gsl.zhijiandao.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://opx.jyoumei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xbh.jqgfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://awj.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://pyh.birdmap.top

Ruby: f(a: 1, b: 2)
来源：http://gra.vqdsnc.cn

C#:   f(a: 1, b: 2)
来源：http://wqd.hammf.cn

[C05] 返回多个值
来源：http://uwf.nanxinkj.top

Py:   return a, b
来源：http://zgt.zdqjudy.top

PHP:  return [$a, $b];
来源：http://wfu.chenjidiqi.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://chs.fehbvm.com

TS:   return { a, b };
来源：http://cti.bbcook.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ctu.zdqjudy.top

Go:   return a, b
来源：http://sue.yonumen.top

Ruby: return a, b
来源：http://hpi.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://lqh.gotoacloud.top

[C06] 匿名函数 / lambda
来源：http://erd.ywan-chungtsiang.top

Py:   square = lambda x: x * x
来源：http://ffj.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vlp.chenzaomai.com

JS:   const square = x => x * x;
来源：http://ymp.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://zvu.snrcjt.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mcn.guannengcc.top

Go:   sq := func(x int) int { return x * x }
来源：http://izh.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://udx.cqqwz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://did.fengsongda.top

[C07] 把函数作为参数传入
来源：http://wic.jianghu66.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lky.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://qrv.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://evt.9152youxi.cn

TS:   arr.map(String)
来源：http://svu.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rkl.xuanzx.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ywz.chenjidiqi.icu


<!-- 参考信息 -->