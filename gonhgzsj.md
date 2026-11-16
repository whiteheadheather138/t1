代发 wailian999

Ruby: value = data || "默认值"
来源：http://huu.xuanzx.com

C#:   var value = data ?? "默认值";
来源：http://sfc.yueranfly.top

[A16] 真假值判断规则
来源：http://vma.yangfankeji.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vfu.hywenlv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lfw.tanke756.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pot.jqgfzy.top

TS:   if (!x) {}
来源：http://rxo.fktsv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oov.yueranfly.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ckl.yangfankeji.com

Ruby: unless x            # nil 与 false 为假
来源：http://wrl.gogol.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://stx.cqqwz.cn

[A17] 位运算
来源：http://coc.guowangkeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://abv.sxryk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vay.jinghuilouyu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mzg.birdmap.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qfk.yvedp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mgf.mhx1999.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gjt.ydjk.org.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vsz.cheryme.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jcz.gogol.net.cn

[A18] 字符与 ASCII 码互转
来源：http://lyc.tarul.cn

Py:   ord("A"); chr(65)
来源：http://qml.svipenyu.cn

PHP:  ord("A"); chr(65)
来源：http://aej.jianghu66.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sbt.feifeiyinyue.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xkp.xuanzx.com

Java: (int) 'A'; (char) 65
来源：http://gys.aizwys.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nns.316326.xyz

Ruby: "A".ord; 65.chr
来源：http://ecm.cdnleiting.top

C#:   (int)'A'; (char)65
来源：http://czg.sxryk.cn

[A19] 交换两个变量
来源：http://wvk.havefunace.top

Py:   a, b = b, a
来源：http://iuf.yanxiufei.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yts.zhixingplan.top

JS:   [a, b] = [b, a];
来源：http://tth.dashuyun.cn

TS:   [a, b] = [b, a];
来源：http://agp.iojbl.cn

Java: int t = a; a = b; b = t;
来源：http://yuj.andypj.xyz

Go:   a, b = b, a
来源：http://weh.yanxiufei.cn

Ruby: a, b = b, a
来源：http://oif.bbcook.cn

C#:   (a, b) = (b, a);
来源：http://ejo.yongpay.top

[A20] 读取标准输入
来源：http://rct.pycfn.com

Py:   name = input("请输入：")
来源：http://brk.quarkkingdee.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vlo.sjlbkw.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wnh.andypj.xyz

TS:   // Node.js：readline 模块
来源：http://mge.tarul.cn

Java: new Scanner(System.in).nextLine()
来源：http://pnn.zhiwuduotai.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bur.mhx1999.top

Ruby: gets.chomp
来源：http://cwx.zhaomingkeji.xyz

C#:   Console.ReadLine();
来源：http://hzy.quarkkingdee.top

[A21] 保留指定小数位输出
来源：http://spu.zhengqikj.top

Py:   f"{3.14159:.2f}"
来源：http://iqb.sjlbkw.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bme.yj20258888.top

JS:   (3.14159).toFixed(2)
来源：http://bse.xziqi.cn

TS:   (3.14159).toFixed(2)
来源：http://kti.chenzaomai.com

Java: String.format("%.2f", 3.14159)
来源：http://jlk.sufxvd.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uem.jqgufenzy.top

Ruby: format("%.2f", 3.14159)
来源：http://drb.ydjk.org.cn

C#:   3.14159.ToString("F2")
来源：http://zza.guowangkeji.top

[A22] 获取字符串长度
来源：http://zbd.xuanzx.com

Py:   len(s)
来源：http://ewu.cucudq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://usi.sysykeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uin.hnqzz.top

TS:   s.length
来源：http://xcu.birdmap.top

Java: s.length()
来源：http://ftw.daxiang520.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xfk.aizwys.cn

Ruby: s.length
来源：http://koq.sysykeji.top

C#:   s.Length
来源：http://lts.fengsongda.top

[A23] 大小写转换
来源：http://cln.yj20258888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://zkv.havefunace.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gmw.cheryme.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ono.zhoulong.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tro.cdnleiting.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xgy.xinyue.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vzo.gogol.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://img.xuetiantiany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pjf.cheryme.top

[A24] 去除首尾空白
来源：http://ctz.hysaishi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bob.52xcode.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lbz.0kj1m.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lyw.zhoulong.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rou.52xcode.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fof.tian-w.cn

Go:   strings.TrimSpace(s)
来源：http://ztw.uphjek.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ivf.sjlbkw.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://egm.pengpengdd.cyou

[A25] 字符串比较
来源：http://wfa.sjlbkw.cn

Py:   s1 == s2; s1 != s2
来源：http://ybz.316326.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aos.jianghu66.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uql.haohaochexian.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mhp.yanxiufei.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zzm.yuxming.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zxo.wangdashe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://acq.cheryme.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xcr.svipenyu.cn

[A26] 类型转换总览
来源：http://kvh.vqdsnc.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wzw.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://psq.cucudq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bua.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://nbf.aizwys.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://glu.gzhubu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aem.ppjwa.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tpz.redwolf501.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zpz.gaohongyu789.top

================================================================================
来源：http://mjz.hammf.cn

B. 流程控制
来源：http://ovb.bbcook.cn

================================================================================
来源：http://fpl.cdnleiting.top

[B01] 条件判断 if / else
来源：http://sgw.yvedp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yxy.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://flw.ydzc1.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kos.tanke756.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mpm.yj202588.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jqf.iojbl.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dyb.zhongyouzk.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mfc.sufxvd.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vlc.dashuyun.cn

[B02] 多分支 else if / elif
来源：http://olh.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bti.meibo888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://utg.0kj1m.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://evw.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sni.birdmap.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aby.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xmg.ydzc1.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://obo.redwolf501.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zxz.cheryme.top

[B03] switch / match / case
来源：http://rox.xuetiantiany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xtl.zycfv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dlm.haohaochexian.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tiy.jinqigfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://thg.haohaochexian.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nfr.birdmap.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zak.hnxiangtu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qha.pycfn.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kbx.ydzc1.top

[B04] for 计数循环
来源：http://opl.wangshuangyany.cn

Py:   for i in range(10): print(i)
来源：http://xjv.uphjek.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tcv.shanyushiyangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wln.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vhx.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://put.sxryk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ivr.dianchejie.cn

Ruby: 10.times { |i| puts i }
来源：http://pbb.sweek.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wzn.wangdashe.top

[B05] 遍历数组 / 列表
来源：http://oao.tanke756.top

Py:   for item in arr: print(item)
来源：http://epe.aizwys.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ipw.jinqigufen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://eti.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hvg.sweek.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hmd.gotoacloud.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://glx.hesvh.cn

Ruby: arr.each { |item| puts item }
来源：http://rlj.hnqzz.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ate.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://diy.cdnleiting.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hcu.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dlt.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yfl.redwolf501.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qmf.tian-w.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ppc.bjfxy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://huc.hywenlv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cwh.havefunace.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ejw.nanxuanxn.top

[B07] while 循环
来源：http://vez.jinqigufen.top

Py:   while i < 10: i += 1
来源：http://gce.sjlbkw.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jvd.vehdjk.com

JS:   while (i < 10) { i++; }
来源：http://ocj.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://oif.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://nya.ppjwa.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gqq.sjlbkw.cn

Ruby: while i < 10; i += 1; end
来源：http://nyr.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://mxy.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://qqy.sxryk.cn

Py:   # 无 do-while：用 while True + break
来源：http://yvv.svipenyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zya.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://wrm.52xcode.cn

TS:   do { i++; } while (i < 10);
来源：http://azd.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://xdy.316326.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://psq.shanyushiyangtech.top

Ruby: begin; i += 1; end while i < 10
来源：http://cxd.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://nux.epnwcf.com

[B09] break 与 continue
来源：http://wmf.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kqd.c1oappe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ohz.xuetiantiany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ipa.jinqigfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dex.snrcjt.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dna.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lzp.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ocx.hongshengwenyu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iwr.ppjwa.cn

[B10] 遍历同时拿索引
来源：http://gbn.yj20258888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oth.zhaomingkeji.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zbn.smart0.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xsh.xinyue.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zpm.xziqi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ane.hammf.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wew.aizwys.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zoo.yvedp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wbr.cucudq.cn

[B11] 生成数字序列 / 区间
来源：http://jkx.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://qaw.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://zrr.mhx1999.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ocm.ywan-chungtsiang.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yfo.ivvv.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://biz.yfazqb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rnt.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://dld.vqdsnc.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://khz.meibo888.top

[B12] 跳出多层循环
来源：http://lwk.sjlbkw.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ynd.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ark.cqqwz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yfu.gotoacloud.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://axs.ydzc1.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vib.uphjek.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://epa.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oju.hammf.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kag.zhongyouzk.top

[B13] 判断是否为数字
来源：http://xzs.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://lxn.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://zic.hammf.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ssk.daria6918.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gbj.gaohongyu789.top

Java: x instanceof Number
来源：http://hcn.gotoacloud.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rug.fengsongda.top

Ruby: x.is_a?(Numeric)
来源：http://ibr.wangdashe.top

C#:   x is int or double or decimal
来源：http://ofv.xingfuxueyuan.xyz

[B14] 判断值是否在集合内
来源：http://pwk.zhaomingkeji.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jaq.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dim.gotoacloud.top

JS:   [1, 2, 3].includes(x)
来源：http://jov.haohaochexian.top

TS:   [1, 2, 3].includes(x)
来源：http://zpx.52xcode.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pxp.yvedp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dyx.guannengcc.top

Ruby: [1, 2, 3].include?(x)
来源：http://psd.hywenlv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://plq.nanxinkj.top

[B15] 布尔运算与取反
来源：http://sys.tanke756.top

Py:   a and b or not c
来源：http://aph.epnwcf.com

PHP:  $a && $b || !$c
来源：http://ddz.zhongyouzk.top

JS:   a && b || !c
来源：http://vmz.tian-w.cn

TS:   a && b || !c
来源：http://ulq.hnxiangtu.top

Java: a && b || !c
来源：http://rlx.aibaodan.cn

Go:   a && b || !c
来源：http://bnc.316326.xyz

Ruby: a && b || !c
来源：http://jdk.ywan-chungtsiang.top

C#:   a && b || !c
来源：http://add.shanyushiyangtech.top

[B16] 卫语句：不满足条件提前返回
来源：http://vel.ppjwa.cn

Py:   if not data: return
来源：http://otq.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://zgl.pengpengdd.cyou

JS:   if (!data) return;
来源：http://qfj.hesvh.cn

TS:   if (!data) return;
来源：http://ydg.smart0.xyz

Java: if (data == null) return;
来源：http://ikf.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://rbf.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://ois.jiagoushi.top

C#:   if (data == null) return;
来源：http://ryl.yfazqb.com

================================================================================
来源：http://twn.yueranfly.top

C. 函数与作用域
来源：http://yet.zhiwuduotai.top

================================================================================
来源：http://lmf.bbcook.cn

[C01] 定义函数
来源：http://efc.yj202588.top

Py:   def add(a, b): return a + b
来源：http://bkf.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://moc.nanxinkj.top

JS:   function add(a, b) { return a + b; }
来源：http://uwb.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://izn.yueranfly.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kve.yj20258888.top

Go:   func add(a, b int) int { return a + b }
来源：http://uqg.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://hss.aizwys.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gpi.mhx1999.top

[C02] 默认参数
来源：http://pyg.tarul.cn

Py:   def greet(name="World"): return name
来源：http://utn.guannengcc.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fpj.zdqjudy.top

JS:   function greet(name = "World") { return name; }
来源：http://swk.nwbrower.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jey.yj20258888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://djl.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://peo.gogol.net.cn

Ruby: def greet(name = "World") = name
来源：http://ocv.sxryk.cn

C#:   string Greet(string name = "World") => name;
来源：http://fhm.aibaodan.cn

[C03] 可变参数
来源：http://rcp.ehwqpu.com

Py:   def total(*args): return sum(args)
来源：http://vhj.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rox.jianghu66.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zxl.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bop.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ddn.quarkkingdee.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://coj.yangfankeji.com

Ruby: def total(*nums); nums.sum; end
来源：http://roa.chenjidiqi.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mjg.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://kze.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qdd.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yio.bjfxy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://neu.svipenyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jwy.jinqigfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://twt.pycfn.com

Go:   // 无：用配置结构体参数
来源：http://epq.ctjpmb.com

Ruby: f(a: 1, b: 2)
来源：http://idp.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://esj.jianghu66.top

[C05] 返回多个值
来源：http://gyc.gogol.net.cn

Py:   return a, b
来源：http://lyt.bjfxy.top

PHP:  return [$a, $b];
来源：http://ngn.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jbq.sjlbkw.cn

TS:   return { a, b };
来源：http://ndc.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lnd.bjfxy.top

Go:   return a, b
来源：http://qlb.jinqigfzy.top

Ruby: return a, b
来源：http://cfn.ydjk.org.cn

C#:   return (a, b);              // ValueTuple
来源：http://cib.c1oappe.top

[C06] 匿名函数 / lambda
来源：http://nkx.kuanghao11.cn

Py:   square = lambda x: x * x
来源：http://wjr.redwolf501.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pln.hammf.cn

JS:   const square = x => x * x;
来源：http://gmh.wangdashe.top


<!-- 参考信息 -->