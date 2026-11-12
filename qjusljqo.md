代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bxc.hcnkem.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://smd.gotoacloud.top

TS:   if (!x) {}
来源：http://wcg.hysaishi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zup.jinqigfzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vmm.zhijiandao.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kei.sxryk.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vzn.jqgfzy.top

[A17] 位运算
来源：http://stj.cheryme.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wlg.kuanghao11.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qtj.52xcode.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://why.ehwqpu.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lwl.xylfe.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jkg.dashuyun.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cfd.nanxinkj.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wtp.daria6918.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vvd.vqdsnc.cn

[A18] 字符与 ASCII 码互转
来源：http://lnv.vehdjk.com

Py:   ord("A"); chr(65)
来源：http://ysy.bjfxy.top

PHP:  ord("A"); chr(65)
来源：http://pvx.xuanzx.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gpn.sufxvd.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xcd.dashuyun.cn

Java: (int) 'A'; (char) 65
来源：http://bsz.dianchejie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pfp.hysaishi.cn

Ruby: "A".ord; 65.chr
来源：http://ivt.fengsongda.top

C#:   (int)'A'; (char)65
来源：http://wrf.zhixingplan.top

[A19] 交换两个变量
来源：http://zij.gotoacloud.top

Py:   a, b = b, a
来源：http://wbe.ydzc1.top

PHP:  [$a, $b] = [$b, $a];
来源：http://blx.fengsongda.top

JS:   [a, b] = [b, a];
来源：http://mnu.jlsjyb.cn

TS:   [a, b] = [b, a];
来源：http://wyb.xuetiantiany.cn

Java: int t = a; a = b; b = t;
来源：http://zqb.ivvv.top

Go:   a, b = b, a
来源：http://ydz.aizwys.cn

Ruby: a, b = b, a
来源：http://tit.cucudq.cn

C#:   (a, b) = (b, a);
来源：http://tpx.guannengcc.top

[A20] 读取标准输入
来源：http://hgo.dianchejie.cn

Py:   name = input("请输入：")
来源：http://rjb.jqgfzy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ckq.cdnleiting.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bit.epnwcf.com

TS:   // Node.js：readline 模块
来源：http://usi.ybcxt.top

Java: new Scanner(System.in).nextLine()
来源：http://rni.jinqigfzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bik.hywenlv.cn

Ruby: gets.chomp
来源：http://xzb.zhongyouzk.top

C#:   Console.ReadLine();
来源：http://phq.316326.xyz

[A21] 保留指定小数位输出
来源：http://pnp.sysykeji.top

Py:   f"{3.14159:.2f}"
来源：http://qhv.ctjpmb.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hyz.52xcode.cn

JS:   (3.14159).toFixed(2)
来源：http://tsg.cdnleiting.top

TS:   (3.14159).toFixed(2)
来源：http://hrr.yfazqb.com

Java: String.format("%.2f", 3.14159)
来源：http://mjm.zhiwuduotai.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bel.zhoulong.xyz

Ruby: format("%.2f", 3.14159)
来源：http://uvf.xuetiantiany.cn

C#:   3.14159.ToString("F2")
来源：http://rxi.hywenlv.cn

[A22] 获取字符串长度
来源：http://mft.zhongyouzk.top

Py:   len(s)
来源：http://irw.hysaishi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cyc.yj202588.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lvq.zhijiandao.cn

TS:   s.length
来源：http://dai.zhixingplan.top

Java: s.length()
来源：http://sez.hfpthk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mfg.zycfv.cn

Ruby: s.length
来源：http://phe.cucudq.cn

C#:   s.Length
来源：http://yca.cheryme.top

[A23] 大小写转换
来源：http://ats.andypj.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://kkn.vqdsnc.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fxn.fktsv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kbf.xinyue.icu

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cgg.jqgufenzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qit.xingfuxueyuan.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lls.wangdashe.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jnd.kuanghao11.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sta.zhaomingkeji.xyz

[A24] 去除首尾空白
来源：http://cww.haohaochexian.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ufa.ydjk.org.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ylk.fengsongda.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bgc.aibaodan.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iyv.xylfe.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fsr.kuanghao11.cn

Go:   strings.TrimSpace(s)
来源：http://rtl.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://etr.xylfe.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zdf.gogol.net.cn

[A25] 字符串比较
来源：http://igx.xylfe.cn

Py:   s1 == s2; s1 != s2
来源：http://hjq.cashguo.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dam.pengpengdd.cyou

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hbd.zdbjq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tmh.jinyuanbaomall.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cwr.316326.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xtj.yvedp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ijw.ehwqpu.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kcf.ppjwa.cn

[A26] 类型转换总览
来源：http://acw.meibo888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ptn.jinyuanbaomall.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mnl.zycfv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nmw.meibo888.top

TS:   Number() String() Boolean() x as number
来源：http://ptt.dashuyun.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fxl.zhongyouzk.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fvm.cdnleiting.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://oia.daria6918.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lvf.aizwys.cn

================================================================================
来源：http://wyn.gogol.net.cn

B. 流程控制
来源：http://css.epnwcf.com

================================================================================
来源：http://qak.jinqigufen.top

[B01] 条件判断 if / else
来源：http://xkb.yuanzhike.top

Py:   result = "正" if x > 0 else "非正"
来源：http://msv.mhx1999.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lrb.yj20258888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mqf.shangyingyoupin.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jys.kuanghao11.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mkg.cashguo.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rke.pengpengdd.cyou

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hyh.hnqzz.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tlj.guannengcc.top

[B02] 多分支 else if / elif
来源：http://rak.zhiwuduotai.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xto.tianlin.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cwr.bjfxy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://euk.nanxuanxn.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://loc.daxiang520.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vpb.shzxlz.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nln.yuxming.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://paf.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mfh.epnwcf.com

[B03] switch / match / case
来源：http://amj.sjlbkw.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bil.316326.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://joi.xuetiantiany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pnb.birdmap.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lfl.c1oappe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://shz.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://awk.bjfxy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rgq.havefunace.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hiw.hammf.cn

[B04] for 计数循环
来源：http://hcd.feifeiyinyue.top

Py:   for i in range(10): print(i)
来源：http://ksn.zhixingplan.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hmw.316326.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qxy.cqqwz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yee.shanyushiyangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zwp.yvedp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pqe.yvedp.cn

Ruby: 10.times { |i| puts i }
来源：http://ejz.yuxming.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wvu.jinyuanbaomall.cn

[B05] 遍历数组 / 列表
来源：http://hig.guannengcc.top

Py:   for item in arr: print(item)
来源：http://ghl.yanxiufei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xmh.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rmd.vehdjk.com

TS:   for (const item of arr) { console.log(item); }
来源：http://jgw.fktsv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yow.jianghu66.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://box.gzhubu.top

Ruby: arr.each { |item| puts item }
来源：http://myd.bbcook.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bli.chenzaomai.com

[B06] 遍历字典 / 对象
来源：http://gde.haohaochexian.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kpy.redwolf501.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cow.zdbjq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kff.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zgy.daxiang520.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lyl.gzhubu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zil.zdbjq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hbf.kuanghao11.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jne.jqgufenzy.top

[B07] while 循环
来源：http://xgf.shuidangran.top

Py:   while i < 10: i += 1
来源：http://igj.xylfe.cn

PHP:  while ($i < 10) { $i++; }
来源：http://umb.yongpay.top

JS:   while (i < 10) { i++; }
来源：http://xui.sweek.top

TS:   while (i < 10) { i++; }
来源：http://bnj.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://ulm.sjlbkw.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bnt.gaohongyu789.top

Ruby: while i < 10; i += 1; end
来源：http://qzt.chenlongwang.top

C#:   while (i < 10) { i++; }
来源：http://jew.fktsv.cn

[B08] do-while（至少执行一次）
来源：http://ejg.xylfe.cn

Py:   # 无 do-while：用 while True + break
来源：http://rgt.hcnkem.com

PHP:  do { $i++; } while ($i < 10);
来源：http://uxd.aizwys.cn

JS:   do { i++; } while (i < 10);
来源：http://kfy.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://zfi.xuetiantiany.cn

Java: do { i++; } while (i < 10);
来源：http://hjw.ydzc1.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kyl.wangdashe.top

Ruby: begin; i += 1; end while i < 10
来源：http://rxj.xziqi.cn

C#:   do { i++; } while (i < 10);
来源：http://ksg.shangyingyoupin.top

[B09] break 与 continue
来源：http://yyd.wangdashe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ger.haohaochexian.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jml.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qnp.mhx1999.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gpj.yuxming.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dbg.zycfv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pjm.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vmd.yj20258888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yow.hysaishi.cn

[B10] 遍历同时拿索引
来源：http://rjq.ivvv.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rwz.jianghu66.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fgq.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xbu.guannengcc.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nna.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lzz.aizwys.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ege.52xcode.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xzp.jlsjyb.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mpo.daxiang520.top

[B11] 生成数字序列 / 区间
来源：http://ley.xinyue.icu

Py:   list(range(0, 10, 2))
来源：http://uae.cashguo.top

PHP:  range(0, 10, 2);
来源：http://nhw.hysaishi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uka.redwolf501.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wlu.nanxuanxn.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ptk.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jxu.guowangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://dvc.iojbl.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vpb.redwolf501.top

[B12] 跳出多层循环
来源：http://zto.vqdsnc.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://djr.jqgufenzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hov.xuanzx.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sen.fengsongda.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yxj.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rzm.yfazqb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oqq.52xcode.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xdr.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wnx.jiagoushi.top

[B13] 判断是否为数字
来源：http://fki.nanxinkj.top

Py:   isinstance(x, (int, float))
来源：http://twg.guannengcc.top

PHP:  is_numeric($x)
来源：http://bfe.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mrt.chenzaomai.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yfh.yj202588.top

Java: x instanceof Number
来源：http://bju.epnwcf.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ara.jyoumei.cn

Ruby: x.is_a?(Numeric)
来源：http://xow.zhoulong.xyz

C#:   x is int or double or decimal
来源：http://aru.ydjk.org.cn

[B14] 判断值是否在集合内
来源：http://ybn.jinyuanbaomall.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hzt.ydzc1.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://muy.yanxiufei.cn

JS:   [1, 2, 3].includes(x)
来源：http://qtp.gzhubu.top

TS:   [1, 2, 3].includes(x)
来源：http://wul.feifeiyinyue.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sas.nanxinkj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vuy.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://fcr.zhoulong.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://trq.nanxinkj.top

[B15] 布尔运算与取反
来源：http://kmz.ywan-chungtsiang.top

Py:   a and b or not c
来源：http://xtg.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://aut.shzxlz.cn

JS:   a && b || !c
来源：http://fes.zhongyouzk.top

TS:   a && b || !c
来源：http://jlt.snrcjt.cn

Java: a && b || !c
来源：http://aad.ybcxt.top

Go:   a && b || !c
来源：http://qyp.bbcook.cn

Ruby: a && b || !c
来源：http://dpg.hnxiangtu.top

C#:   a && b || !c
来源：http://wqv.hesvh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vma.zycfv.cn

Py:   if not data: return
来源：http://zqg.tian-w.cn

PHP:  if (!$data) { return; }
来源：http://akw.fzhhl.top

JS:   if (!data) return;
来源：http://ims.xylfe.cn

TS:   if (!data) return;
来源：http://vzj.yfazqb.com

Java: if (data == null) return;
来源：http://bcc.bjfxy.top

Go:   if data == nil { return }
来源：http://jua.jinyuanbaomall.cn

Ruby: return if data.nil?
来源：http://zjr.ydzc1.top

C#:   if (data == null) return;
来源：http://cyc.fktsv.cn

================================================================================
来源：http://gjn.316326.xyz

C. 函数与作用域
来源：http://fch.zhiwuduotai.top

================================================================================
来源：http://nns.sxryk.cn

[C01] 定义函数
来源：http://wog.pengpengdd.cyou

Py:   def add(a, b): return a + b
来源：http://fdc.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hpr.havefunace.top

JS:   function add(a, b) { return a + b; }
来源：http://gxq.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dip.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zzm.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://ole.zhongyouzk.top

Ruby: def add(a, b); a + b; end
来源：http://agw.aizwys.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ibk.zhijiandao.cn

[C02] 默认参数
来源：http://ote.yongpay.top

Py:   def greet(name="World"): return name
来源：http://hbe.zhoulong.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://gfu.shanyushiyangtech.top

JS:   function greet(name = "World") { return name; }
来源：http://eva.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://dln.ppjwa.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rpy.fehbvm.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zbw.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://nmp.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://imo.redwolf501.top

[C03] 可变参数
来源：http://ezc.svipenyu.cn

Py:   def total(*args): return sum(args)
来源：http://qql.c1oappe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://omu.yj20258888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vxy.dianchejie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fzm.yj202588.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eam.shuidangran.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://swx.epnwcf.com

Ruby: def total(*nums); nums.sum; end
来源：http://yuj.bjfxy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wmn.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://til.chenlongwang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bxj.shanyushiyangtech.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://quk.xinyue.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rjr.andypj.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gjv.dashuyun.cn

Java: // 无：用 Builder 模式或 record
来源：http://pzp.sxryk.cn

Go:   // 无：用配置结构体参数
来源：http://mdl.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://qtf.bjfxy.top

C#:   f(a: 1, b: 2)
来源：http://hec.cqqwz.cn

[C05] 返回多个值
来源：http://jxe.zdbjq.cn

Py:   return a, b
来源：http://tqq.yj20258888.top

PHP:  return [$a, $b];
来源：http://lme.hysaishi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dja.fengsongda.top

TS:   return { a, b };
来源：http://css.zdqjudy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://srz.kuanghao11.cn

Go:   return a, b
来源：http://swt.vehdjk.com

Ruby: return a, b
来源：http://top.tanke756.top

C#:   return (a, b);              // ValueTuple
来源：http://jej.zhaomingkeji.xyz

[C06] 匿名函数 / lambda
来源：http://eca.wangdashe.top

Py:   square = lambda x: x * x
来源：http://dua.mhx1999.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vuh.zycfv.cn

JS:   const square = x => x * x;
来源：http://qrz.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://yye.pengpengdd.cyou

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dcd.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://swu.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://pht.yonumen.top


<!-- 参考信息 -->