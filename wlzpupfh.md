代发 wailian999

Ruby: value = data || "默认值"
来源：http://jio.zhijiandao.cn

C#:   var value = data ?? "默认值";
来源：http://gsi.wangdashe.top

[A16] 真假值判断规则
来源：http://sdv.jinghuilouyu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://imk.tianlin.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qgk.xylfe.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tpn.gzhubu.top

TS:   if (!x) {}
来源：http://xvl.ydzc1.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xcb.snrcjt.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://clm.hfpthk.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xyx.redwolf501.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xws.zhiwuduotai.top

[A17] 位运算
来源：http://ktj.aizwys.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gzh.zdqjudy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://oeh.hysaishi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wnl.yj202588.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bnn.zhiwuduotai.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kwf.yanxiufei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wgz.jinyuanbaomall.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fsn.wangshuangyany.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bdq.guowangkeji.top

[A18] 字符与 ASCII 码互转
来源：http://lrc.birdmap.top

Py:   ord("A"); chr(65)
来源：http://crk.aibaodan.cn

PHP:  ord("A"); chr(65)
来源：http://opu.sysykeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://icd.yueranfly.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sar.andypj.xyz

Java: (int) 'A'; (char) 65
来源：http://vjj.shangyingyoupin.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ljo.xziqi.cn

Ruby: "A".ord; 65.chr
来源：http://sbz.wangdashe.top

C#:   (int)'A'; (char)65
来源：http://zsf.c1oappe.top

[A19] 交换两个变量
来源：http://mbl.fengsongda.top

Py:   a, b = b, a
来源：http://owm.svipenyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rrn.shzxlz.cn

JS:   [a, b] = [b, a];
来源：http://jmt.vehdjk.com

TS:   [a, b] = [b, a];
来源：http://cyl.epnwcf.com

Java: int t = a; a = b; b = t;
来源：http://siu.vqdsnc.cn

Go:   a, b = b, a
来源：http://zre.yfazqb.com

Ruby: a, b = b, a
来源：http://bjm.fzhhl.top

C#:   (a, b) = (b, a);
来源：http://drp.zhoulong.xyz

[A20] 读取标准输入
来源：http://ehs.cdnleiting.top

Py:   name = input("请输入：")
来源：http://gdh.ehwqpu.com

PHP:  $name = trim(fgets(STDIN));
来源：http://fmy.nanxinkj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://and.uphjek.com

TS:   // Node.js：readline 模块
来源：http://brm.xuetiantiany.cn

Java: new Scanner(System.in).nextLine()
来源：http://jdt.xylfe.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fgj.feifeiyinyue.top

Ruby: gets.chomp
来源：http://fit.hnqzz.top

C#:   Console.ReadLine();
来源：http://kdo.cheryme.top

[A21] 保留指定小数位输出
来源：http://wot.dashuyun.cn

Py:   f"{3.14159:.2f}"
来源：http://osc.nanxinkj.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pdu.tian-w.cn

JS:   (3.14159).toFixed(2)
来源：http://gan.sxryk.cn

TS:   (3.14159).toFixed(2)
来源：http://zsx.hnqzz.top

Java: String.format("%.2f", 3.14159)
来源：http://qal.yj20258.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://frx.shanyushiyangtech.top

Ruby: format("%.2f", 3.14159)
来源：http://ejo.iojbl.cn

C#:   3.14159.ToString("F2")
来源：http://izq.9152youxi.cn

[A22] 获取字符串长度
来源：http://gjj.zhijiandao.cn

Py:   len(s)
来源：http://ugc.yj202588.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lji.ybcxt.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ynz.yongpay.top

TS:   s.length
来源：http://gry.hnqzz.top

Java: s.length()
来源：http://hha.tarul.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bwn.ctjpmb.com

Ruby: s.length
来源：http://axc.jlsjyb.cn

C#:   s.Length
来源：http://zer.sysykeji.top

[A23] 大小写转换
来源：http://tik.tarul.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://grr.yfazqb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zcu.sweek.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pxt.quarkkingdee.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qlg.jinyuanbaomall.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://udx.gzhubu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gdd.nwbrower.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ejy.xylfe.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vpo.birdmap.top

[A24] 去除首尾空白
来源：http://rtb.yueranfly.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xzy.wangshuangyany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oto.haohaochexian.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tck.sysykeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dsp.guannengcc.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ugx.ydjk.org.cn

Go:   strings.TrimSpace(s)
来源：http://zix.hnqzz.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cde.vqdsnc.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://igy.aibaodan.cn

[A25] 字符串比较
来源：http://orz.hysaishi.cn

Py:   s1 == s2; s1 != s2
来源：http://xwb.redwolf501.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://liz.hesvh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xwr.cdnleiting.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bbu.jinghuilouyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rec.c1oappe.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tgt.fktsv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rcm.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pfs.fengsongda.top

[A26] 类型转换总览
来源：http://ufp.tanke756.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ipb.kuanghao11.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wvn.yongpay.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ume.shuidangran.top

TS:   Number() String() Boolean() x as number
来源：http://cek.yangfankeji.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ffo.hongshengwenyu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vdo.bbcook.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iyv.jiagoushi.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vei.yj20258888.top

================================================================================
来源：http://rwm.cdnleiting.top

B. 流程控制
来源：http://rbm.vehdjk.com

================================================================================
来源：http://urk.0kj1m.cn

[B01] 条件判断 if / else
来源：http://rxz.yj202588.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ojh.jqgufenzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ygw.c1oappe.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://grj.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dip.nanxuanxn.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lud.316326.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pbn.cheryme.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hbb.dianchejie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rte.52xcode.cn

[B02] 多分支 else if / elif
来源：http://lra.pengpengdd.cyou

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tye.ybcxt.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zso.0kj1m.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rnd.guannengcc.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iwh.shanyushiyangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xzy.gzhubu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vtx.dianchejie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pno.cdnleiting.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://efm.jqgufenzy.top

[B03] switch / match / case
来源：http://rym.ydjk.org.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rbg.xuetiantiany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zrq.cqqwz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wiw.yongpay.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aya.tianlin.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wff.0kj1m.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lpz.ybcxt.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ihs.fengsongda.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://anw.jinqigfzy.top

[B04] for 计数循环
来源：http://cxs.cashguo.top

Py:   for i in range(10): print(i)
来源：http://eju.gogol.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://alu.zhaomingkeji.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://clp.epnwcf.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hav.wangshuangyany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aci.jiagoushi.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ngi.gotoacloud.top

Ruby: 10.times { |i| puts i }
来源：http://liy.wangshuangyany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sei.c1oappe.top

[B05] 遍历数组 / 列表
来源：http://rcb.kuanghao11.cn

Py:   for item in arr: print(item)
来源：http://rla.haohaochexian.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jna.nanxinkj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ukz.tian-w.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mkx.zdbjq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nez.haohaochexian.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rnc.zdbjq.cn

Ruby: arr.each { |item| puts item }
来源：http://ivj.pengpengdd.cyou

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ken.guowangkeji.top

[B06] 遍历字典 / 对象
来源：http://igd.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fyj.jlsjyb.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lpd.jqgufenzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sya.yanxiufei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://abx.havefunace.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rcc.sweek.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pob.dashuyun.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ail.yongpay.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mtr.iojbl.cn

[B07] while 循环
来源：http://tnj.xuanzx.com

Py:   while i < 10: i += 1
来源：http://ebi.smart0.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ktb.zhaomingkeji.xyz

JS:   while (i < 10) { i++; }
来源：http://puq.yfazqb.com

TS:   while (i < 10) { i++; }
来源：http://laz.sufxvd.cn

Java: while (i < 10) { i++; }
来源：http://erk.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vfr.xziqi.cn

Ruby: while i < 10; i += 1; end
来源：http://ibm.hesvh.cn

C#:   while (i < 10) { i++; }
来源：http://bed.zdbjq.cn

[B08] do-while（至少执行一次）
来源：http://kph.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://xsq.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kkz.fanxiaobao.xyz

JS:   do { i++; } while (i < 10);
来源：http://jfn.jiagoushi.top

TS:   do { i++; } while (i < 10);
来源：http://idq.yvedp.cn

Java: do { i++; } while (i < 10);
来源：http://zec.meibo888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jlj.guannengcc.top

Ruby: begin; i += 1; end while i < 10
来源：http://hhm.nanxinkj.top

C#:   do { i++; } while (i < 10);
来源：http://bnp.jinqigfzy.top

[B09] break 与 continue
来源：http://gfg.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jyq.hysaishi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lwm.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iha.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qee.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sxn.jqgufenzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gti.ppjwa.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xub.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jir.bjfxy.top

[B10] 遍历同时拿索引
来源：http://ztg.yueranfly.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cqv.sufxvd.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fju.tarul.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qnk.jinghuilouyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nyz.ydzc1.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xmy.yuxming.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vmo.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jjd.pengpengdd.cyou

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://noj.chenlongwang.top

[B11] 生成数字序列 / 区间
来源：http://dys.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://eob.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://goc.vehdjk.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rrz.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aum.hcnkem.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ili.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blt.hnqzz.top

Ruby: (0...10).step(2).to_a
来源：http://dar.jlsjyb.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xgw.ivvv.top

[B12] 跳出多层循环
来源：http://yoh.nanxinkj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yme.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://dyb.havefunace.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mmv.cdnleiting.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vhp.jianghu66.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pfd.zdqjudy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lpv.pycfn.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://msy.gogol.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pyf.9152youxi.cn

[B13] 判断是否为数字
来源：http://ztw.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://ria.bbcook.cn

PHP:  is_numeric($x)
来源：http://dzm.gotoacloud.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://igq.zhongyouzk.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kqq.sufxvd.cn

Java: x instanceof Number
来源：http://dmj.yuanzhike.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kgc.gaohongyu789.top

Ruby: x.is_a?(Numeric)
来源：http://tvm.9152youxi.cn

C#:   x is int or double or decimal
来源：http://rpa.jinghuilouyu.cn

[B14] 判断值是否在集合内
来源：http://drm.guannengcc.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wnj.316326.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xvp.shuidangran.top

JS:   [1, 2, 3].includes(x)
来源：http://huf.dashuyun.cn

TS:   [1, 2, 3].includes(x)
来源：http://yba.jqgufenzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jsu.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ppx.vehdjk.com

Ruby: [1, 2, 3].include?(x)
来源：http://nsu.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ptm.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://mmd.ydjk.org.cn

Py:   a and b or not c
来源：http://spk.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://kxm.haohaochexian.top

JS:   a && b || !c
来源：http://qly.cashguo.top

TS:   a && b || !c
来源：http://igx.shanyushiyangtech.top

Java: a && b || !c
来源：http://hnx.tian-w.cn

Go:   a && b || !c
来源：http://axc.wangdashe.top

Ruby: a && b || !c
来源：http://tzj.hysaishi.cn

C#:   a && b || !c
来源：http://wck.dianchejie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fza.shzxlz.cn

Py:   if not data: return
来源：http://bfw.yj20258.top

PHP:  if (!$data) { return; }
来源：http://rfs.haohaochexian.top

JS:   if (!data) return;
来源：http://awp.jiagoushi.top

TS:   if (!data) return;
来源：http://cmv.tian-w.cn

Java: if (data == null) return;
来源：http://taz.haohaochexian.top

Go:   if data == nil { return }
来源：http://tpn.pengpengdd.cyou

Ruby: return if data.nil?
来源：http://xdv.haohaochexian.top

C#:   if (data == null) return;
来源：http://lxu.hysaishi.cn

================================================================================
来源：http://eow.316326.xyz

C. 函数与作用域
来源：http://hqk.nanxinkj.top

================================================================================
来源：http://frn.pengpengdd.cyou

[C01] 定义函数
来源：http://fqi.pycfn.com

Py:   def add(a, b): return a + b
来源：http://zse.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mqj.pengpengdd.cyou

JS:   function add(a, b) { return a + b; }
来源：http://lkc.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mkj.shanyushiyangtech.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ihl.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tjq.shanyushiyangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://iop.gzhubu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ihd.gotoacloud.top

[C02] 默认参数
来源：http://uij.shangyingyoupin.top

Py:   def greet(name="World"): return name
来源：http://qwt.gotoacloud.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mbl.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://rfj.jyoumei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dtj.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://glp.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://why.sjlbkw.cn

Ruby: def greet(name = "World") = name
来源：http://yvt.birdmap.top

C#:   string Greet(string name = "World") => name;
来源：http://smf.fzhhl.top

[C03] 可变参数
来源：http://rfn.yongpay.top

Py:   def total(*args): return sum(args)
来源：http://iqv.gaohongyu789.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lcz.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://shs.chenzaomai.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qcf.fehbvm.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ruq.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tpq.redwolf501.top

Ruby: def total(*nums); nums.sum; end
来源：http://cqw.yangfankeji.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://str.zhoulong.xyz

[C04] 命名参数 / 关键字参数
来源：http://fbg.wangshuangyany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vns.tanke756.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://los.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zgf.ctjpmb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bbl.jinyuanbaomall.cn

Java: // 无：用 Builder 模式或 record
来源：http://xlr.jinqigufen.top

Go:   // 无：用配置结构体参数
来源：http://pks.yonumen.top

Ruby: f(a: 1, b: 2)
来源：http://btf.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://xyn.ywan-chungtsiang.top

[C05] 返回多个值
来源：http://hwo.zhengqikj.top

Py:   return a, b
来源：http://did.sxryk.cn

PHP:  return [$a, $b];
来源：http://bgd.feifeiyinyue.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jbu.aibaodan.cn

TS:   return { a, b };
来源：http://iwx.ctjpmb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fwn.tian-w.cn

Go:   return a, b
来源：http://rui.yvedp.cn

Ruby: return a, b
来源：http://uxx.zdbjq.cn

C#:   return (a, b);              // ValueTuple
来源：http://wcb.chenlongwang.top

[C06] 匿名函数 / lambda
来源：http://vio.zhoulong.xyz

Py:   square = lambda x: x * x
来源：http://vbt.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vem.c1oappe.top

JS:   const square = x => x * x;
来源：http://hky.quarkkingdee.top


<!-- 参考信息 -->