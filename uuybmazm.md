代发 wailian999

Ruby: value = data || "默认值"
来源：http://xgl.snrcjt.cn

C#:   var value = data ?? "默认值";
来源：http://mon.jqgfzy.top

[A16] 真假值判断规则
来源：http://oma.tanke756.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://azo.sufxvd.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://awa.zdqjudy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://myj.gzhubu.top

TS:   if (!x) {}
来源：http://gye.chenjidiqi.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kql.yuxming.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tki.chenzaomai.com

Ruby: unless x            # nil 与 false 为假
来源：http://jpz.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ain.jinqigufen.top

[A17] 位运算
来源：http://dcw.vehdjk.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vju.c1oappe.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hqc.chenjidiqi.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cfh.tian-w.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ubq.gotoacloud.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kbf.havefunace.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sfy.gaohongyu789.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ebq.aizwys.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vof.sjlbkw.cn

[A18] 字符与 ASCII 码互转
来源：http://rae.hcnkem.com

Py:   ord("A"); chr(65)
来源：http://ene.fanxiaobao.xyz

PHP:  ord("A"); chr(65)
来源：http://cif.hnqzz.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sqv.daxiang520.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bhp.gzhubu.top

Java: (int) 'A'; (char) 65
来源：http://ksq.9152youxi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qgf.zycfv.cn

Ruby: "A".ord; 65.chr
来源：http://vus.sweek.top

C#:   (int)'A'; (char)65
来源：http://qax.sxryk.cn

[A19] 交换两个变量
来源：http://yxu.yangfankeji.com

Py:   a, b = b, a
来源：http://fpq.ehwqpu.com

PHP:  [$a, $b] = [$b, $a];
来源：http://qcn.yfazqb.com

JS:   [a, b] = [b, a];
来源：http://pkw.xingfuxueyuan.xyz

TS:   [a, b] = [b, a];
来源：http://wjk.xziqi.cn

Java: int t = a; a = b; b = t;
来源：http://ufi.xinyue.icu

Go:   a, b = b, a
来源：http://xmp.cqqwz.cn

Ruby: a, b = b, a
来源：http://inp.hnqzz.top

C#:   (a, b) = (b, a);
来源：http://rnf.daria6918.cn

[A20] 读取标准输入
来源：http://dpj.xuetiantiany.cn

Py:   name = input("请输入：")
来源：http://vnk.jinghuilouyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://uoi.sufxvd.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fjj.jianghu66.top

TS:   // Node.js：readline 模块
来源：http://wxk.zhaomingkeji.xyz

Java: new Scanner(System.in).nextLine()
来源：http://fbs.gogol.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bjv.vqdsnc.cn

Ruby: gets.chomp
来源：http://gil.gzhubu.top

C#:   Console.ReadLine();
来源：http://gbg.zhongyouzk.top

[A21] 保留指定小数位输出
来源：http://huz.xingfuxueyuan.xyz

Py:   f"{3.14159:.2f}"
来源：http://lce.cqqwz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qbo.tanke756.top

JS:   (3.14159).toFixed(2)
来源：http://ayl.yj202588.top

TS:   (3.14159).toFixed(2)
来源：http://fue.hongshengwenyu.top

Java: String.format("%.2f", 3.14159)
来源：http://kno.birdmap.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xbj.yongpay.top

Ruby: format("%.2f", 3.14159)
来源：http://boz.guannengcc.top

C#:   3.14159.ToString("F2")
来源：http://kft.bbcook.cn

[A22] 获取字符串长度
来源：http://icw.hesvh.cn

Py:   len(s)
来源：http://cut.c1oappe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jek.wangshuangyany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aok.andypj.xyz

TS:   s.length
来源：http://oln.shanyushiyangtech.top

Java: s.length()
来源：http://tul.zhongyouzk.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sty.iojbl.cn

Ruby: s.length
来源：http://afe.yuanzhike.top

C#:   s.Length
来源：http://oqz.tarul.cn

[A23] 大小写转换
来源：http://lsb.xinyue.icu

Py:   s.upper(); s.lower(); s.title()
来源：http://vjc.yuanzhike.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pwt.ehwqpu.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eee.svipenyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://toe.cashguo.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rby.jiagoushi.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jcw.guannengcc.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://heg.uphjek.com

C#:   s.ToUpper(); s.ToLower()
来源：http://ikg.iojbl.cn

[A24] 去除首尾空白
来源：http://nkj.redwolf501.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hui.birdmap.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://awe.vqdsnc.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jvd.vehdjk.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yjw.yangfankeji.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cnb.jyoumei.cn

Go:   strings.TrimSpace(s)
来源：http://ugt.ppjwa.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ejy.cdnleiting.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ycc.zhiwuduotai.top

[A25] 字符串比较
来源：http://zer.jlsjyb.cn

Py:   s1 == s2; s1 != s2
来源：http://rvq.jiagoushi.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fxk.smart0.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mmv.snrcjt.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://azd.jlsjyb.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qdl.yonumen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iuq.mhx1999.top

Ruby: s1 == s2; s1 <=> s2
来源：http://lco.sxryk.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lws.52xcode.cn

[A26] 类型转换总览
来源：http://ryh.shzxlz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gpz.xylfe.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yzw.ehwqpu.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xzb.jqgfzy.top

TS:   Number() String() Boolean() x as number
来源：http://mfn.gaohongyu789.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jgf.cashguo.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qiw.wangdashe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://egx.sysykeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vnx.fanxiaobao.xyz

================================================================================
来源：http://voe.zhongyouzk.top

B. 流程控制
来源：http://zta.fengsongda.top

================================================================================
来源：http://pls.feifeiyinyue.top

[B01] 条件判断 if / else
来源：http://ddf.zhengqikj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xed.ydjk.org.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dwh.uphjek.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jks.jqgufenzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gbb.jyoumei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ncy.zhoulong.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mta.hysaishi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://onf.jiagoushi.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://skw.bjfxy.top

[B02] 多分支 else if / elif
来源：http://tiq.sufxvd.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lqp.uphjek.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vvk.daria6918.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://myj.epnwcf.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bsw.snrcjt.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wdd.fehbvm.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sip.fanxiaobao.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ljt.kuanghao11.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kea.zhoulong.xyz

[B03] switch / match / case
来源：http://udh.tanke756.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://czf.quarkkingdee.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ydl.shzxlz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ple.aizwys.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gdf.sjlbkw.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wbc.nanxuanxn.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dyp.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://slk.smart0.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ptb.nanxuanxn.top

[B04] for 计数循环
来源：http://hku.tanke756.top

Py:   for i in range(10): print(i)
来源：http://hsk.tianlin.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nsa.zdbjq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iht.0kj1m.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nex.yanxiufei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aeo.jinghuilouyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iwa.bbcook.cn

Ruby: 10.times { |i| puts i }
来源：http://zrb.xziqi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xbb.ybcxt.top

[B05] 遍历数组 / 列表
来源：http://rjl.yuxming.cn

Py:   for item in arr: print(item)
来源：http://omg.hysaishi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://emw.sysykeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zbo.vqdsnc.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hju.pycfn.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://gdi.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sii.ywan-chungtsiang.top

Ruby: arr.each { |item| puts item }
来源：http://ugr.jiagoushi.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dcd.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://cvp.pengpengdd.cyou

Py:   for k, v in d.items(): print(k, v)
来源：http://nmn.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hjz.uphjek.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fdu.0kj1m.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qyc.fanxiaobao.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://diy.sufxvd.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lum.gzhubu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ixd.zdqjudy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kly.jqgufenzy.top

[B07] while 循环
来源：http://iwj.zhaomingkeji.xyz

Py:   while i < 10: i += 1
来源：http://vun.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://srh.jinqigufen.top

JS:   while (i < 10) { i++; }
来源：http://put.xuanzx.com

TS:   while (i < 10) { i++; }
来源：http://qcm.9152youxi.cn

Java: while (i < 10) { i++; }
来源：http://vfn.zhijiandao.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://faq.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://oib.jqgufenzy.top

C#:   while (i < 10) { i++; }
来源：http://nsr.shanyushiyangtech.top

[B08] do-while（至少执行一次）
来源：http://nqr.hongshengwenyu.top

Py:   # 无 do-while：用 while True + break
来源：http://yvt.gogol.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rzb.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://wbx.sjlbkw.cn

TS:   do { i++; } while (i < 10);
来源：http://fsj.tarul.cn

Java: do { i++; } while (i < 10);
来源：http://iwv.snrcjt.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cas.chenzaomai.com

Ruby: begin; i += 1; end while i < 10
来源：http://zky.ybcxt.top

C#:   do { i++; } while (i < 10);
来源：http://lly.meibo888.top

[B09] break 与 continue
来源：http://ltl.jinqigufen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tpv.andypj.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dwg.ydzc1.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gcf.316326.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dbl.fehbvm.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xmv.xziqi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iil.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mgz.yueranfly.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aht.epnwcf.com

[B10] 遍历同时拿索引
来源：http://ddk.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hah.tian-w.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wdl.yongpay.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sua.c1oappe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lpm.ydzc1.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gkv.ydjk.org.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mus.dianchejie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eev.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://awr.fktsv.cn

[B11] 生成数字序列 / 区间
来源：http://pqy.xziqi.cn

Py:   list(range(0, 10, 2))
来源：http://mun.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://zwf.fengsongda.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pir.sjlbkw.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fmb.zhengqikj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eel.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tme.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://wcj.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rrp.fzhhl.top

[B12] 跳出多层循环
来源：http://ndn.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cvr.andypj.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://nbp.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bsl.yuxming.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rka.gogol.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ecf.yfazqb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://omj.cashguo.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://odj.bbcook.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dbj.fktsv.cn

[B13] 判断是否为数字
来源：http://loh.hysaishi.cn

Py:   isinstance(x, (int, float))
来源：http://wax.jiagoushi.top

PHP:  is_numeric($x)
来源：http://njo.c1oappe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jfy.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mlb.kuanghao11.cn

Java: x instanceof Number
来源：http://hxl.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ior.guowangkeji.top

Ruby: x.is_a?(Numeric)
来源：http://axp.c1oappe.top

C#:   x is int or double or decimal
来源：http://owz.hnxiangtu.top

[B14] 判断值是否在集合内
来源：http://hfy.zdqjudy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://osj.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qsh.zhongyouzk.top

JS:   [1, 2, 3].includes(x)
来源：http://fvw.ctjpmb.com

TS:   [1, 2, 3].includes(x)
来源：http://qoc.cashguo.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pdr.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gow.feifeiyinyue.top

Ruby: [1, 2, 3].include?(x)
来源：http://ieq.52xcode.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hjw.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://voa.9152youxi.cn

Py:   a and b or not c
来源：http://mel.gzhubu.top

PHP:  $a && $b || !$c
来源：http://axe.ehwqpu.com

JS:   a && b || !c
来源：http://ojm.vehdjk.com

TS:   a && b || !c
来源：http://chb.hysaishi.cn

Java: a && b || !c
来源：http://uze.gzhubu.top

Go:   a && b || !c
来源：http://mti.yfazqb.com

Ruby: a && b || !c
来源：http://bkt.xziqi.cn

C#:   a && b || !c
来源：http://mfg.uphjek.com

[B16] 卫语句：不满足条件提前返回
来源：http://fxq.gaohongyu789.top

Py:   if not data: return
来源：http://tfl.gaohongyu789.top

PHP:  if (!$data) { return; }
来源：http://jpm.snrcjt.cn

JS:   if (!data) return;
来源：http://mso.shzxlz.cn

TS:   if (!data) return;
来源：http://pju.cashguo.top

Java: if (data == null) return;
来源：http://lml.andypj.xyz

Go:   if data == nil { return }
来源：http://qvu.yj202588.top

Ruby: return if data.nil?
来源：http://pjn.vqdsnc.cn

C#:   if (data == null) return;
来源：http://plf.daria6918.cn

================================================================================
来源：http://jtx.sjlbkw.cn

C. 函数与作用域
来源：http://vxp.hesvh.cn

================================================================================
来源：http://pve.jiagoushi.top

[C01] 定义函数
来源：http://cdo.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://yiz.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uup.jinghuilouyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ylx.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://skm.zhoulong.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://apx.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pvp.yvedp.cn

Ruby: def add(a, b); a + b; end
来源：http://gop.ybcxt.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ach.daria6918.cn

[C02] 默认参数
来源：http://zyc.jyoumei.cn

Py:   def greet(name="World"): return name
来源：http://fjl.tarul.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uur.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://hwk.hcnkem.com

TS:   function greet(name: string = "World") { return name; }
来源：http://psh.chenlongwang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mpz.fehbvm.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yvt.chenjidiqi.icu

Ruby: def greet(name = "World") = name
来源：http://bll.nwbrower.top

C#:   string Greet(string name = "World") => name;
来源：http://qni.fktsv.cn

[C03] 可变参数
来源：http://ess.daxiang520.top

Py:   def total(*args): return sum(args)
来源：http://yqv.jiagoushi.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nay.uphjek.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ebu.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ear.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://imk.ywan-chungtsiang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qed.shanyushiyangtech.top

Ruby: def total(*nums); nums.sum; end
来源：http://sff.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oar.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://loc.hnqzz.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xyn.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zjq.ehwqpu.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://osc.jiagoushi.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sst.fzhhl.top

Java: // 无：用 Builder 模式或 record
来源：http://cqp.ywan-chungtsiang.top

Go:   // 无：用配置结构体参数
来源：http://fsm.bjfxy.top

Ruby: f(a: 1, b: 2)
来源：http://cca.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://gsz.wangshuangyany.cn

[C05] 返回多个值
来源：http://ppb.epnwcf.com

Py:   return a, b
来源：http://qcm.havefunace.top

PHP:  return [$a, $b];
来源：http://spu.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pvc.jiagoushi.top

TS:   return { a, b };
来源：http://tzx.ehwqpu.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qjp.tian-w.cn

Go:   return a, b
来源：http://wys.bjfxy.top

Ruby: return a, b
来源：http://siw.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://jkd.cashguo.top

[C06] 匿名函数 / lambda
来源：http://ctg.yonumen.top

Py:   square = lambda x: x * x
来源：http://ewn.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://huj.yj202588.top

JS:   const square = x => x * x;
来源：http://zln.hnqzz.top


<!-- 参考信息 -->