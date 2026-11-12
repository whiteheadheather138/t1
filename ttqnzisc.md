代发 wailian999

Ruby: value = data || "默认值"
来源：http://ppm.quarkkingdee.top

C#:   var value = data ?? "默认值";
来源：http://vvv.pengpengdd.cyou

[A16] 真假值判断规则
来源：http://ecb.jyoumei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ees.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://orr.iojbl.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://veb.c1oappe.top

TS:   if (!x) {}
来源：http://noz.hongshengwenyu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://upa.sjlbkw.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jwv.zycfv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zes.havefunace.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lww.xingfuxueyuan.xyz

[A17] 位运算
来源：http://hls.nanxinkj.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yrm.ppjwa.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vah.zdbjq.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gxt.yanxiufei.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ipg.yanxiufei.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fgh.xylfe.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wdn.gaohongyu789.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oem.daxiang520.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vlm.iojbl.cn

[A18] 字符与 ASCII 码互转
来源：http://jmo.redwolf501.top

Py:   ord("A"); chr(65)
来源：http://kbt.yuanzhike.top

PHP:  ord("A"); chr(65)
来源：http://mja.hnqzz.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ter.guannengcc.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gwv.hnxiangtu.top

Java: (int) 'A'; (char) 65
来源：http://aan.c1oappe.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://csr.yfazqb.com

Ruby: "A".ord; 65.chr
来源：http://lvo.yangfankeji.com

C#:   (int)'A'; (char)65
来源：http://aro.guannengcc.top

[A19] 交换两个变量
来源：http://kay.nanxuanxn.top

Py:   a, b = b, a
来源：http://pqh.fktsv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zmz.zdbjq.cn

JS:   [a, b] = [b, a];
来源：http://keo.chenjidiqi.icu

TS:   [a, b] = [b, a];
来源：http://xzu.gaohongyu789.top

Java: int t = a; a = b; b = t;
来源：http://xix.9152youxi.cn

Go:   a, b = b, a
来源：http://lhg.yangfankeji.com

Ruby: a, b = b, a
来源：http://wbx.fengsongda.top

C#:   (a, b) = (b, a);
来源：http://utz.jqgufenzy.top

[A20] 读取标准输入
来源：http://mfp.epnwcf.com

Py:   name = input("请输入：")
来源：http://rle.vqdsnc.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ohn.nanxinkj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ogp.ydjk.org.cn

TS:   // Node.js：readline 模块
来源：http://fxa.iojbl.cn

Java: new Scanner(System.in).nextLine()
来源：http://cuh.c1oappe.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ged.ydzc1.top

Ruby: gets.chomp
来源：http://iwz.tanke756.top

C#:   Console.ReadLine();
来源：http://zao.tanke756.top

[A21] 保留指定小数位输出
来源：http://yds.jinghuilouyu.cn

Py:   f"{3.14159:.2f}"
来源：http://rwx.ctjpmb.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ykr.nanxuanxn.top

JS:   (3.14159).toFixed(2)
来源：http://xyg.snrcjt.cn

TS:   (3.14159).toFixed(2)
来源：http://imd.hongshengwenyu.top

Java: String.format("%.2f", 3.14159)
来源：http://zsf.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ufu.yanxiufei.cn

Ruby: format("%.2f", 3.14159)
来源：http://xnt.aibaodan.cn

C#:   3.14159.ToString("F2")
来源：http://gzw.zdbjq.cn

[A22] 获取字符串长度
来源：http://bfh.zhengqikj.top

Py:   len(s)
来源：http://efc.hesvh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xwg.jqgufenzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lmv.zdqjudy.top

TS:   s.length
来源：http://mtl.sjlbkw.cn

Java: s.length()
来源：http://umk.ydzc1.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qil.nanxuanxn.top

Ruby: s.length
来源：http://dbm.hnqzz.top

C#:   s.Length
来源：http://fox.shanyushiyangtech.top

[A23] 大小写转换
来源：http://icq.hnxiangtu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://eqa.jinghuilouyu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oyv.shzxlz.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ves.yj20258.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qiu.ydjk.org.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eqj.cucudq.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zah.9152youxi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pgk.dashuyun.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://idb.hysaishi.cn

[A24] 去除首尾空白
来源：http://pkq.shuidangran.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hub.gotoacloud.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hvo.yonumen.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jrs.xinyue.icu

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aqi.gotoacloud.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://opg.smart0.xyz

Go:   strings.TrimSpace(s)
来源：http://pxm.zdbjq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oss.bbcook.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xrp.feifeiyinyue.top

[A25] 字符串比较
来源：http://adr.shangyingyoupin.top

Py:   s1 == s2; s1 != s2
来源：http://mts.dianchejie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://huc.hcnkem.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://maw.aibaodan.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lgb.zhongyouzk.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ihf.guowangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xye.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tip.meibo888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wkc.andypj.xyz

[A26] 类型转换总览
来源：http://kvq.yj202588.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iwk.yvedp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ezo.shanyushiyangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cpp.shanyushiyangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://hzh.jqgfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xkq.daria6918.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sic.gogol.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jpf.hysaishi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nwf.zdqjudy.top

================================================================================
来源：http://kaf.smart0.xyz

B. 流程控制
来源：http://vfq.iojbl.cn

================================================================================
来源：http://dzp.xuetiantiany.cn

[B01] 条件判断 if / else
来源：http://acc.hnqzz.top

Py:   result = "正" if x > 0 else "非正"
来源：http://iwn.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eir.316326.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zrb.gaohongyu789.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bxl.epnwcf.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://fql.andypj.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eso.andypj.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tkf.hesvh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qdp.redwolf501.top

[B02] 多分支 else if / elif
来源：http://eig.yanxiufei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lsr.gzhubu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uqq.sxryk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://raz.fehbvm.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gop.c1oappe.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jvf.cheryme.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tki.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mct.vqdsnc.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gop.fktsv.cn

[B03] switch / match / case
来源：http://lpq.dashuyun.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dqy.jinghuilouyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hkr.9152youxi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sjv.nanxuanxn.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uka.wangdashe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dsb.cqqwz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://elz.chenjidiqi.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uzb.wangdashe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vwe.fehbvm.com

[B04] for 计数循环
来源：http://ktc.xziqi.cn

Py:   for i in range(10): print(i)
来源：http://dri.yuxming.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ypy.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xiv.52xcode.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://otm.meibo888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cfw.jianghu66.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jdc.chenlongwang.top

Ruby: 10.times { |i| puts i }
来源：http://qcb.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bno.gogol.net.cn

[B05] 遍历数组 / 列表
来源：http://quu.yj20258.top

Py:   for item in arr: print(item)
来源：http://wli.yuanzhike.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cje.jinqigfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qlw.yj202588.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kpy.chenzaomai.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://qvz.birdmap.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ich.jqgfzy.top

Ruby: arr.each { |item| puts item }
来源：http://wqk.jinqigfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://noo.c1oappe.top

[B06] 遍历字典 / 对象
来源：http://hwm.wangshuangyany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://djh.tianlin.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ahg.guowangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sxr.cashguo.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lrs.0kj1m.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://alx.hywenlv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qvt.gaohongyu789.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sbf.gogol.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ptu.zdbjq.cn

[B07] while 循环
来源：http://pun.jinqigufen.top

Py:   while i < 10: i += 1
来源：http://zar.jinyuanbaomall.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cxh.daxiang520.top

JS:   while (i < 10) { i++; }
来源：http://mfg.yvedp.cn

TS:   while (i < 10) { i++; }
来源：http://gyg.ctjpmb.com

Java: while (i < 10) { i++; }
来源：http://kmm.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xez.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://ves.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://ysf.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://hea.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://lti.xziqi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jgk.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://bzk.vqdsnc.cn

TS:   do { i++; } while (i < 10);
来源：http://jfd.yuxming.cn

Java: do { i++; } while (i < 10);
来源：http://zik.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wvr.jqgufenzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://oqp.yongpay.top

C#:   do { i++; } while (i < 10);
来源：http://xql.hnxiangtu.top

[B09] break 与 continue
来源：http://pxe.snrcjt.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ouh.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ihc.smart0.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uap.shanyushiyangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lts.yvedp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fdz.yongpay.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://upu.quarkkingdee.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nuj.pycfn.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jre.xylfe.cn

[B10] 遍历同时拿索引
来源：http://lnw.shanyushiyangtech.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pgj.jinqigufen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gyv.hcnkem.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fyl.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ypp.jinyuanbaomall.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xrq.cheryme.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gxu.xziqi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yrb.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dvh.haohaochexian.top

[B11] 生成数字序列 / 区间
来源：http://ubo.daria6918.cn

Py:   list(range(0, 10, 2))
来源：http://gpn.xziqi.cn

PHP:  range(0, 10, 2);
来源：http://dhr.jqgfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tzx.xuanzx.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oiz.zdqjudy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bbh.redwolf501.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wyx.zdbjq.cn

Ruby: (0...10).step(2).to_a
来源：http://dju.chenjidiqi.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bgf.9152youxi.cn

[B12] 跳出多层循环
来源：http://jed.sysykeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rjh.gzhubu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pej.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pms.hongshengwenyu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ysp.hcnkem.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zar.xingfuxueyuan.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bop.yonumen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bck.tarul.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gul.316326.xyz

[B13] 判断是否为数字
来源：http://tvk.birdmap.top

Py:   isinstance(x, (int, float))
来源：http://nwq.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://ywh.chenlongwang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aqi.sjlbkw.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tkz.redwolf501.top

Java: x instanceof Number
来源：http://gsq.cashguo.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lrb.zhixingplan.top

Ruby: x.is_a?(Numeric)
来源：http://lhe.iojbl.cn

C#:   x is int or double or decimal
来源：http://sbd.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://ucf.xylfe.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iih.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kzh.jinqigfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://ioe.cheryme.top

TS:   [1, 2, 3].includes(x)
来源：http://kqa.ybcxt.top

Java: List.of(1, 2, 3).contains(x)
来源：http://emw.kuanghao11.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vlo.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://scr.hesvh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tff.guowangkeji.top

[B15] 布尔运算与取反
来源：http://ehn.fengsongda.top

Py:   a and b or not c
来源：http://qvh.snrcjt.cn

PHP:  $a && $b || !$c
来源：http://xzu.cheryme.top

JS:   a && b || !c
来源：http://gwi.jyoumei.cn

TS:   a && b || !c
来源：http://mrj.zhengqikj.top

Java: a && b || !c
来源：http://jez.sweek.top

Go:   a && b || !c
来源：http://fpf.pycfn.com

Ruby: a && b || !c
来源：http://pzm.jlsjyb.cn

C#:   a && b || !c
来源：http://zxr.dianchejie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hsw.guannengcc.top

Py:   if not data: return
来源：http://akk.jqgfzy.top

PHP:  if (!$data) { return; }
来源：http://oqp.snrcjt.cn

JS:   if (!data) return;
来源：http://ayj.ivvv.top

TS:   if (!data) return;
来源：http://nqg.ctjpmb.com

Java: if (data == null) return;
来源：http://fwg.tian-w.cn

Go:   if data == nil { return }
来源：http://amu.fzhhl.top

Ruby: return if data.nil?
来源：http://noo.fzhhl.top

C#:   if (data == null) return;
来源：http://lwr.jlsjyb.cn

================================================================================
来源：http://pjm.fehbvm.com

C. 函数与作用域
来源：http://chw.yj202588.top

================================================================================
来源：http://yjy.sweek.top

[C01] 定义函数
来源：http://sxc.xylfe.cn

Py:   def add(a, b): return a + b
来源：http://tlr.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://omi.0kj1m.cn

JS:   function add(a, b) { return a + b; }
来源：http://vez.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dvx.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://ezg.smart0.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://eug.pycfn.com

Ruby: def add(a, b); a + b; end
来源：http://uth.iojbl.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zrx.yj20258.top

[C02] 默认参数
来源：http://dqx.zhaomingkeji.xyz

Py:   def greet(name="World"): return name
来源：http://aea.jiagoushi.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ldy.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://ioe.bjfxy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rvs.yangfankeji.com

Java: // 无默认参数：方法重载或 Optional
来源：http://cya.ydjk.org.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nvr.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://ukc.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://dab.52xcode.cn

[C03] 可变参数
来源：http://yyh.jiagoushi.top

Py:   def total(*args): return sum(args)
来源：http://owv.c1oappe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://npy.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://det.wangshuangyany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://voe.smart0.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wwa.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oli.yongpay.top

Ruby: def total(*nums); nums.sum; end
来源：http://oer.zycfv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wfk.sysykeji.top

[C04] 命名参数 / 关键字参数
来源：http://xro.jinqigfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://man.gotoacloud.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nrj.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ohj.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bca.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://dtv.havefunace.top

Go:   // 无：用配置结构体参数
来源：http://zoo.shanyushiyangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://oyt.nanxinkj.top

C#:   f(a: 1, b: 2)
来源：http://gfu.guannengcc.top

[C05] 返回多个值
来源：http://pck.quarkkingdee.top

Py:   return a, b
来源：http://wbq.iojbl.cn

PHP:  return [$a, $b];
来源：http://fxg.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pic.yfazqb.com

TS:   return { a, b };
来源：http://xyi.ctjpmb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://saj.vqdsnc.cn

Go:   return a, b
来源：http://eik.feifeiyinyue.top

Ruby: return a, b
来源：http://zck.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://jni.yanxiufei.cn

[C06] 匿名函数 / lambda
来源：http://eis.yuxming.cn

Py:   square = lambda x: x * x
来源：http://ktz.yj202588.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bmr.zhengqikj.top

JS:   const square = x => x * x;
来源：http://tua.ybcxt.top


<!-- 参考信息 -->