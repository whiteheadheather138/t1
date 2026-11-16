代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cak.haohaochexian.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://knw.kuanghao11.cn

TS:   if (!x) {}
来源：http://zvn.shangyingyoupin.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wvq.xingfuxueyuan.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ryu.daria6918.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ind.0kj1m.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zak.zhijiandao.cn

[A17] 位运算
来源：http://lxv.yueranfly.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ffn.jianghu66.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://aec.zhongyouzk.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rse.shanyushiyangtech.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wrt.hesvh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://akl.yongpay.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fsb.mhx1999.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dkr.birdmap.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dvt.ppjwa.cn

[A18] 字符与 ASCII 码互转
来源：http://spv.jinqigfzy.top

Py:   ord("A"); chr(65)
来源：http://emn.ywan-chungtsiang.top

PHP:  ord("A"); chr(65)
来源：http://wqd.hcnkem.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rth.gotoacloud.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://exk.zhengqikj.top

Java: (int) 'A'; (char) 65
来源：http://hpx.pycfn.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vlx.yueranfly.top

Ruby: "A".ord; 65.chr
来源：http://xwv.fzhhl.top

C#:   (int)'A'; (char)65
来源：http://cab.c1oappe.top

[A19] 交换两个变量
来源：http://bxd.pengpengdd.cyou

Py:   a, b = b, a
来源：http://txp.jinqigufen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hbl.yangfankeji.com

JS:   [a, b] = [b, a];
来源：http://dok.zycfv.cn

TS:   [a, b] = [b, a];
来源：http://gfb.shzxlz.cn

Java: int t = a; a = b; b = t;
来源：http://hld.cdnleiting.top

Go:   a, b = b, a
来源：http://naj.chenlongwang.top

Ruby: a, b = b, a
来源：http://tox.pengpengdd.cyou

C#:   (a, b) = (b, a);
来源：http://fav.hcnkem.com

[A20] 读取标准输入
来源：http://bdq.jinqigfzy.top

Py:   name = input("请输入：")
来源：http://luw.redwolf501.top

PHP:  $name = trim(fgets(STDIN));
来源：http://olm.shzxlz.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vkw.jinyuanbaomall.cn

TS:   // Node.js：readline 模块
来源：http://vdn.xziqi.cn

Java: new Scanner(System.in).nextLine()
来源：http://hzb.snrcjt.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://isa.yongpay.top

Ruby: gets.chomp
来源：http://bdh.jyoumei.cn

C#:   Console.ReadLine();
来源：http://mic.shanyushiyangtech.top

[A21] 保留指定小数位输出
来源：http://olq.sysykeji.top

Py:   f"{3.14159:.2f}"
来源：http://hoo.316326.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lab.iojbl.cn

JS:   (3.14159).toFixed(2)
来源：http://njz.shanyushiyangtech.top

TS:   (3.14159).toFixed(2)
来源：http://zsg.nanxinkj.top

Java: String.format("%.2f", 3.14159)
来源：http://acf.tianlin.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wum.wangshuangyany.cn

Ruby: format("%.2f", 3.14159)
来源：http://gyq.aizwys.cn

C#:   3.14159.ToString("F2")
来源：http://vvq.fanxiaobao.xyz

[A22] 获取字符串长度
来源：http://jwl.hongshengwenyu.top

Py:   len(s)
来源：http://vsv.zhaomingkeji.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hvy.daxiang520.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sni.jyoumei.cn

TS:   s.length
来源：http://hxn.fengsongda.top

Java: s.length()
来源：http://hqk.yonumen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pdp.bbcook.cn

Ruby: s.length
来源：http://kxm.tanke756.top

C#:   s.Length
来源：http://nxo.jqgfzy.top

[A23] 大小写转换
来源：http://dyy.shanyushiyangtech.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ogb.sufxvd.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zas.yonumen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vmb.tanke756.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://joe.xinyue.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oaq.xuetiantiany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hkl.birdmap.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ytl.jianghu66.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kgq.zhongyouzk.top

[A24] 去除首尾空白
来源：http://zom.bjfxy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eej.wangdashe.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://enb.shanyushiyangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bet.zhongyouzk.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gep.guannengcc.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vqn.9152youxi.cn

Go:   strings.TrimSpace(s)
来源：http://dth.yonumen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xpu.yj20258888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dau.hysaishi.cn

[A25] 字符串比较
来源：http://uyv.c1oappe.top

Py:   s1 == s2; s1 != s2
来源：http://nob.cheryme.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bdj.316326.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vlj.ydjk.org.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mtm.zhixingplan.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gqh.yueranfly.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ipf.0kj1m.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ddf.hnxiangtu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sko.jlsjyb.cn

[A26] 类型转换总览
来源：http://dog.jinyuanbaomall.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qef.vehdjk.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fnw.tian-w.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ube.bbcook.cn

TS:   Number() String() Boolean() x as number
来源：http://hxb.chenlongwang.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yyf.xuetiantiany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ooq.snrcjt.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qej.cqqwz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ani.ybcxt.top

================================================================================
来源：http://khg.yj20258888.top

B. 流程控制
来源：http://bop.sxryk.cn

================================================================================
来源：http://jvm.zhoulong.xyz

[B01] 条件判断 if / else
来源：http://iii.dianchejie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uja.tarul.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://voz.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eby.zhongyouzk.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oqa.zhaomingkeji.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://hbt.gogol.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mtc.hcnkem.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://plq.meibo888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yvi.9152youxi.cn

[B02] 多分支 else if / elif
来源：http://xml.sufxvd.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://deo.yuxming.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zje.yongpay.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zki.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://crv.hfpthk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pde.c1oappe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ski.chenlongwang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cti.yangfankeji.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xov.pengpengdd.cyou

[B03] switch / match / case
来源：http://jzi.jiagoushi.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oua.zycfv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ayi.fanxiaobao.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dmj.yongpay.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dwm.wangshuangyany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://msj.jinqigfzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jzi.jqgufenzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jrz.wangdashe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ufc.xylfe.cn

[B04] for 计数循环
来源：http://efk.ydzc1.top

Py:   for i in range(10): print(i)
来源：http://iay.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rtu.yueranfly.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lmb.fanxiaobao.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xtx.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gmu.hnxiangtu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vsm.guannengcc.top

Ruby: 10.times { |i| puts i }
来源：http://hdd.fktsv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uvt.yvedp.cn

[B05] 遍历数组 / 列表
来源：http://wsr.tianlin.xyz

Py:   for item in arr: print(item)
来源：http://fdu.ydjk.org.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://foh.fanxiaobao.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://gtf.ivvv.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qnt.shangyingyoupin.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://peu.vqdsnc.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zop.zhongyouzk.top

Ruby: arr.each { |item| puts item }
来源：http://nfx.fehbvm.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fkn.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://gvh.quarkkingdee.top

Py:   for k, v in d.items(): print(k, v)
来源：http://smu.gotoacloud.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://exe.gogol.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vjn.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zom.smart0.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dgw.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zle.guowangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://trn.pengpengdd.cyou

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ksi.yfazqb.com

[B07] while 循环
来源：http://khc.pycfn.com

Py:   while i < 10: i += 1
来源：http://zyl.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://fis.guannengcc.top

JS:   while (i < 10) { i++; }
来源：http://msq.smart0.xyz

TS:   while (i < 10) { i++; }
来源：http://bdg.chenjidiqi.icu

Java: while (i < 10) { i++; }
来源：http://tny.c1oappe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tjk.zhengqikj.top

Ruby: while i < 10; i += 1; end
来源：http://jkn.nanxuanxn.top

C#:   while (i < 10) { i++; }
来源：http://cqh.jqgfzy.top

[B08] do-while（至少执行一次）
来源：http://iwe.cashguo.top

Py:   # 无 do-while：用 while True + break
来源：http://xhc.cucudq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://acg.fehbvm.com

JS:   do { i++; } while (i < 10);
来源：http://dte.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://tla.chenlongwang.top

Java: do { i++; } while (i < 10);
来源：http://ges.zhiwuduotai.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hhd.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://byw.c1oappe.top

C#:   do { i++; } while (i < 10);
来源：http://hou.vehdjk.com

[B09] break 与 continue
来源：http://ran.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gdg.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sxv.jianghu66.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sis.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ski.vehdjk.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ydv.haohaochexian.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ayc.pycfn.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://svo.guannengcc.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dzw.shzxlz.cn

[B10] 遍历同时拿索引
来源：http://uyh.epnwcf.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://avz.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://erm.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nai.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lds.redwolf501.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oyj.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hub.gaohongyu789.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://noq.uphjek.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ndf.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://yva.haohaochexian.top

Py:   list(range(0, 10, 2))
来源：http://zff.redwolf501.top

PHP:  range(0, 10, 2);
来源：http://vrz.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sib.yangfankeji.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://isc.cheryme.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://alu.tanke756.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bue.wangdashe.top

Ruby: (0...10).step(2).to_a
来源：http://aeg.wangshuangyany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gpr.ivvv.top

[B12] 跳出多层循环
来源：http://vhc.hnqzz.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kdb.haohaochexian.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lps.jqgfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rvr.xylfe.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pgl.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eoe.daria6918.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uuh.kuanghao11.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zbu.zdbjq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qvr.fengsongda.top

[B13] 判断是否为数字
来源：http://bzi.chenlongwang.top

Py:   isinstance(x, (int, float))
来源：http://rvr.pengpengdd.cyou

PHP:  is_numeric($x)
来源：http://skf.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cnc.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qlt.gaohongyu789.top

Java: x instanceof Number
来源：http://sek.yj20258.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dfi.xinyue.icu

Ruby: x.is_a?(Numeric)
来源：http://swg.xuetiantiany.cn

C#:   x is int or double or decimal
来源：http://xkx.bjfxy.top

[B14] 判断值是否在集合内
来源：http://mrn.cqqwz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://knr.uphjek.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vgu.c1oappe.top

JS:   [1, 2, 3].includes(x)
来源：http://emq.jinyuanbaomall.cn

TS:   [1, 2, 3].includes(x)
来源：http://vdi.xingfuxueyuan.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://hvw.shangyingyoupin.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cxz.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://bca.yuanzhike.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rbw.ivvv.top

[B15] 布尔运算与取反
来源：http://fdi.yangfankeji.com

Py:   a and b or not c
来源：http://byg.gaohongyu789.top

PHP:  $a && $b || !$c
来源：http://fbu.xziqi.cn

JS:   a && b || !c
来源：http://bbv.gaohongyu789.top

TS:   a && b || !c
来源：http://abi.hfpthk.cn

Java: a && b || !c
来源：http://isu.jiagoushi.top

Go:   a && b || !c
来源：http://ojg.tarul.cn

Ruby: a && b || !c
来源：http://zfy.fzhhl.top

C#:   a && b || !c
来源：http://iwx.vehdjk.com

[B16] 卫语句：不满足条件提前返回
来源：http://oiu.gogol.net.cn

Py:   if not data: return
来源：http://vpn.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://rak.svipenyu.cn

JS:   if (!data) return;
来源：http://xmm.bjfxy.top

TS:   if (!data) return;
来源：http://zff.vqdsnc.cn

Java: if (data == null) return;
来源：http://oht.shanyushiyangtech.top

Go:   if data == nil { return }
来源：http://xnc.zhoulong.xyz

Ruby: return if data.nil?
来源：http://wvd.aibaodan.cn

C#:   if (data == null) return;
来源：http://ejp.hesvh.cn

================================================================================
来源：http://lku.pengpengdd.cyou

C. 函数与作用域
来源：http://zak.shanyushiyangkeji.top

================================================================================
来源：http://npy.fehbvm.com

[C01] 定义函数
来源：http://zdy.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://eko.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qam.0kj1m.cn

JS:   function add(a, b) { return a + b; }
来源：http://yyl.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xhh.meibo888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qii.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://xko.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://ova.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ljj.zdqjudy.top

[C02] 默认参数
来源：http://oxq.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://ysm.wangshuangyany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zdc.sysykeji.top

JS:   function greet(name = "World") { return name; }
来源：http://ntd.hywenlv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qhj.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zsx.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bjt.yongpay.top

Ruby: def greet(name = "World") = name
来源：http://azp.ydjk.org.cn

C#:   string Greet(string name = "World") => name;
来源：http://zsv.yongpay.top

[C03] 可变参数
来源：http://hkn.jinyuanbaomall.cn

Py:   def total(*args): return sum(args)
来源：http://gfl.jyoumei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mpu.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mfv.nwbrower.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sdz.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ldd.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nxv.aizwys.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pyz.jqgfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://abx.redwolf501.top

[C04] 命名参数 / 关键字参数
来源：http://mcd.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hgv.gogol.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xiu.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ohr.svipenyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ggc.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://xkw.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://vix.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://bwv.9152youxi.cn

C#:   f(a: 1, b: 2)
来源：http://hni.chenzaomai.com

[C05] 返回多个值
来源：http://ghh.bjfxy.top

Py:   return a, b
来源：http://ame.ybcxt.top

PHP:  return [$a, $b];
来源：http://rcs.nanxuanxn.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dfb.shanyushiyangtech.top

TS:   return { a, b };
来源：http://omg.316326.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yff.hysaishi.cn

Go:   return a, b
来源：http://gfe.yuanzhike.top

Ruby: return a, b
来源：http://abl.tianlin.xyz

C#:   return (a, b);              // ValueTuple
来源：http://ydv.kuanghao11.cn

[C06] 匿名函数 / lambda
来源：http://fhw.ctjpmb.com

Py:   square = lambda x: x * x
来源：http://ztc.vqdsnc.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bih.mhx1999.top

JS:   const square = x => x * x;
来源：http://vhe.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://gpy.ehwqpu.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zdp.zhijiandao.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zbx.jinqigfzy.top

Ruby: square = ->(x) { x * x }
来源：http://ioh.9152youxi.cn


<!-- 参考信息 -->