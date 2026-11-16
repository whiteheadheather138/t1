代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oms.c1oappe.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ajt.hfpthk.cn

TS:   if (!x) {}
来源：http://ehg.andypj.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bsk.yongpay.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qpe.hfpthk.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ndj.xziqi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nwc.shzxlz.cn

[A17] 位运算
来源：http://gsr.snrcjt.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vrb.yj20258888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gbh.ppjwa.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://itz.wangdashe.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mzn.meibo888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ksy.gogol.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vgq.shuidangran.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jjn.yanxiufei.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qqn.c1oappe.top

[A18] 字符与 ASCII 码互转
来源：http://jbb.ehwqpu.com

Py:   ord("A"); chr(65)
来源：http://ira.xylfe.cn

PHP:  ord("A"); chr(65)
来源：http://ohm.sjlbkw.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lyt.hongshengwenyu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://trs.yongpay.top

Java: (int) 'A'; (char) 65
来源：http://zvy.redwolf501.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bep.ctjpmb.com

Ruby: "A".ord; 65.chr
来源：http://vtq.xziqi.cn

C#:   (int)'A'; (char)65
来源：http://mwy.gotoacloud.top

[A19] 交换两个变量
来源：http://vcv.yonumen.top

Py:   a, b = b, a
来源：http://iva.cqqwz.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zeb.ydjk.org.cn

JS:   [a, b] = [b, a];
来源：http://wwc.bjfxy.top

TS:   [a, b] = [b, a];
来源：http://wnn.pycfn.com

Java: int t = a; a = b; b = t;
来源：http://wsb.vqdsnc.cn

Go:   a, b = b, a
来源：http://dxt.sysykeji.top

Ruby: a, b = b, a
来源：http://pbh.hesvh.cn

C#:   (a, b) = (b, a);
来源：http://yhg.svipenyu.cn

[A20] 读取标准输入
来源：http://krc.hesvh.cn

Py:   name = input("请输入：")
来源：http://hun.smart0.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://dtf.smart0.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hta.vehdjk.com

TS:   // Node.js：readline 模块
来源：http://mlh.sweek.top

Java: new Scanner(System.in).nextLine()
来源：http://cqs.quarkkingdee.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hkq.dashuyun.cn

Ruby: gets.chomp
来源：http://knt.yfazqb.com

C#:   Console.ReadLine();
来源：http://fwm.mhx1999.top

[A21] 保留指定小数位输出
来源：http://auw.sjlbkw.cn

Py:   f"{3.14159:.2f}"
来源：http://qab.sxryk.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vuw.birdmap.top

JS:   (3.14159).toFixed(2)
来源：http://azj.chenzaomai.com

TS:   (3.14159).toFixed(2)
来源：http://imt.fanxiaobao.xyz

Java: String.format("%.2f", 3.14159)
来源：http://ymg.jianghu66.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uxy.316326.xyz

Ruby: format("%.2f", 3.14159)
来源：http://hyl.sxryk.cn

C#:   3.14159.ToString("F2")
来源：http://wop.316326.xyz

[A22] 获取字符串长度
来源：http://ygl.sysykeji.top

Py:   len(s)
来源：http://ttm.dashuyun.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zkr.zhiwuduotai.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cwy.yangfankeji.com

TS:   s.length
来源：http://tgt.guannengcc.top

Java: s.length()
来源：http://jop.jinqigufen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rxy.shanyushiyangkeji.top

Ruby: s.length
来源：http://jqo.xuetiantiany.cn

C#:   s.Length
来源：http://myo.zhiwuduotai.top

[A23] 大小写转换
来源：http://zyb.yangfankeji.com

Py:   s.upper(); s.lower(); s.title()
来源：http://als.snrcjt.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dko.fengsongda.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nog.hywenlv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ffj.hongshengwenyu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jbo.nanxuanxn.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pch.ppjwa.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uvp.c1oappe.top

C#:   s.ToUpper(); s.ToLower()
来源：http://uzb.gotoacloud.top

[A24] 去除首尾空白
来源：http://npo.cdnleiting.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bhb.jqgufenzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oza.gzhubu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vcf.yj20258.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mvi.0kj1m.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wiq.zhijiandao.cn

Go:   strings.TrimSpace(s)
来源：http://zbb.sweek.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pbb.sufxvd.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kwg.uphjek.com

[A25] 字符串比较
来源：http://guj.ppjwa.cn

Py:   s1 == s2; s1 != s2
来源：http://xla.fanxiaobao.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qut.hnqzz.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aut.tanke756.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://raf.ydzc1.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://frc.ctjpmb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ray.316326.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://qcs.0kj1m.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bmh.fzhhl.top

[A26] 类型转换总览
来源：http://wnx.pengpengdd.cyou

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cax.ehwqpu.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qec.hfpthk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eec.dashuyun.cn

TS:   Number() String() Boolean() x as number
来源：http://ing.sufxvd.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gwo.bjfxy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dhm.yvedp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oge.fzhhl.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sqb.zhongyouzk.top

================================================================================
来源：http://aqj.xuetiantiany.cn

B. 流程控制
来源：http://iyd.tian-w.cn

================================================================================
来源：http://ffy.sjlbkw.cn

[B01] 条件判断 if / else
来源：http://zhz.gotoacloud.top

Py:   result = "正" if x > 0 else "非正"
来源：http://pvo.hnxiangtu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bai.c1oappe.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://usj.hnqzz.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nkd.jyoumei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uua.yj202588.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://auw.zhixingplan.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ybd.yvedp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mlo.9152youxi.cn

[B02] 多分支 else if / elif
来源：http://cth.ydzc1.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xlj.wangdashe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://asw.jinghuilouyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zyg.xinyue.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mkd.haohaochexian.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mzv.cashguo.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xju.jyoumei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://alp.bbcook.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xun.shanyushiyangtech.top

[B03] switch / match / case
来源：http://kli.cqqwz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vpb.yanxiufei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pam.yvedp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gqs.yvedp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pis.fanxiaobao.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://poc.jinghuilouyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bwe.hesvh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dnp.ydzc1.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yvq.jianghu66.top

[B04] for 计数循环
来源：http://csd.vehdjk.com

Py:   for i in range(10): print(i)
来源：http://yrc.316326.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nju.ehwqpu.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yya.ywan-chungtsiang.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lai.bjfxy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mak.uphjek.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tnw.zdqjudy.top

Ruby: 10.times { |i| puts i }
来源：http://efl.chenjidiqi.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mvw.yfazqb.com

[B05] 遍历数组 / 列表
来源：http://wgb.zhengqikj.top

Py:   for item in arr: print(item)
来源：http://yqs.aizwys.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://edd.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vji.0kj1m.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uzz.ydjk.org.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fsx.mhx1999.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xig.xingfuxueyuan.xyz

Ruby: arr.each { |item| puts item }
来源：http://iab.sxryk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oun.zhiwuduotai.top

[B06] 遍历字典 / 对象
来源：http://ida.jyoumei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jta.iojbl.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dte.havefunace.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kvz.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yuk.hnqzz.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://amw.havefunace.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ert.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wuh.fengsongda.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cjv.sysykeji.top

[B07] while 循环
来源：http://yjr.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://sse.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://eoa.vehdjk.com

JS:   while (i < 10) { i++; }
来源：http://wrs.vqdsnc.cn

TS:   while (i < 10) { i++; }
来源：http://myy.uphjek.com

Java: while (i < 10) { i++; }
来源：http://yjp.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://niq.zhongyouzk.top

Ruby: while i < 10; i += 1; end
来源：http://ntv.yfazqb.com

C#:   while (i < 10) { i++; }
来源：http://ebr.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://ogp.hywenlv.cn

Py:   # 无 do-while：用 while True + break
来源：http://duy.hnqzz.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bdw.xingfuxueyuan.xyz

JS:   do { i++; } while (i < 10);
来源：http://uti.hnxiangtu.top

TS:   do { i++; } while (i < 10);
来源：http://uqt.andypj.xyz

Java: do { i++; } while (i < 10);
来源：http://xng.shanyushiyangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xqo.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wbd.ivvv.top

C#:   do { i++; } while (i < 10);
来源：http://jgq.shanyushiyangkeji.top

[B09] break 与 continue
来源：http://uai.tian-w.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tcy.iojbl.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://afs.shanyushiyangtech.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uib.svipenyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ftj.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ado.hywenlv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bvk.jinyuanbaomall.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vrj.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aym.vehdjk.com

[B10] 遍历同时拿索引
来源：http://fyv.yonumen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ype.guannengcc.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ftg.hnqzz.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nnj.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gik.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rsh.xuetiantiany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zly.yj20258888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zrj.kuanghao11.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ckh.yj202588.top

[B11] 生成数字序列 / 区间
来源：http://ouf.yj20258888.top

Py:   list(range(0, 10, 2))
来源：http://mzs.hnxiangtu.top

PHP:  range(0, 10, 2);
来源：http://mwn.guannengcc.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xth.havefunace.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pad.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vaf.iojbl.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rzg.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://soe.shanyushiyangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bft.hfpthk.cn

[B12] 跳出多层循环
来源：http://nzw.316326.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://qfz.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nsi.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dyg.shzxlz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jqp.jqgufenzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zgq.0kj1m.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jlm.nwbrower.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fot.guowangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cay.jinyuanbaomall.cn

[B13] 判断是否为数字
来源：http://efp.yonumen.top

Py:   isinstance(x, (int, float))
来源：http://lqa.chenjidiqi.icu

PHP:  is_numeric($x)
来源：http://qku.snrcjt.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://soe.hywenlv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dip.xuetiantiany.cn

Java: x instanceof Number
来源：http://sba.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nxf.cqqwz.cn

Ruby: x.is_a?(Numeric)
来源：http://wtk.dianchejie.cn

C#:   x is int or double or decimal
来源：http://qgd.ydzc1.top

[B14] 判断值是否在集合内
来源：http://uub.havefunace.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://adx.vehdjk.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bvf.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://bsm.zdbjq.cn

TS:   [1, 2, 3].includes(x)
来源：http://mmz.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mrk.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://apm.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://adb.cucudq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vuf.pycfn.com

[B15] 布尔运算与取反
来源：http://rob.cucudq.cn

Py:   a and b or not c
来源：http://svv.xinyue.icu

PHP:  $a && $b || !$c
来源：http://udq.zhixingplan.top

JS:   a && b || !c
来源：http://ioo.52xcode.cn

TS:   a && b || !c
来源：http://xld.quarkkingdee.top

Java: a && b || !c
来源：http://nuq.vehdjk.com

Go:   a && b || !c
来源：http://lbg.uphjek.com

Ruby: a && b || !c
来源：http://xmf.shzxlz.cn

C#:   a && b || !c
来源：http://rfi.hesvh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zur.jiagoushi.top

Py:   if not data: return
来源：http://xzd.vehdjk.com

PHP:  if (!$data) { return; }
来源：http://xxq.wangdashe.top

JS:   if (!data) return;
来源：http://zzm.hcnkem.com

TS:   if (!data) return;
来源：http://fst.nwbrower.top

Java: if (data == null) return;
来源：http://qmv.tianlin.xyz

Go:   if data == nil { return }
来源：http://rcd.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://yvt.zhiwuduotai.top

C#:   if (data == null) return;
来源：http://auw.zhixingplan.top

================================================================================
来源：http://idl.hesvh.cn

C. 函数与作用域
来源：http://gqp.jqgufenzy.top

================================================================================
来源：http://akl.xuanzx.com

[C01] 定义函数
来源：http://smg.9152youxi.cn

Py:   def add(a, b): return a + b
来源：http://xav.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wzu.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://udm.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://khw.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mvr.smart0.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://fgg.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://plc.cucudq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jwj.shangyingyoupin.top

[C02] 默认参数
来源：http://kim.jyoumei.cn

Py:   def greet(name="World"): return name
来源：http://dis.dianchejie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rjw.shangyingyoupin.top

JS:   function greet(name = "World") { return name; }
来源：http://ioz.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jah.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jyb.tian-w.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cja.hnqzz.top

Ruby: def greet(name = "World") = name
来源：http://ykd.hcnkem.com

C#:   string Greet(string name = "World") => name;
来源：http://tbq.hfpthk.cn

[C03] 可变参数
来源：http://yzm.xuetiantiany.cn

Py:   def total(*args): return sum(args)
来源：http://jbz.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kme.dashuyun.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://spk.jinqigfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lxl.ehwqpu.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rav.gogol.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vef.zycfv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ttf.jinqigfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ybo.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://zxf.0kj1m.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gxm.sxryk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qhw.hesvh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tjg.guannengcc.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ivs.aibaodan.cn

Java: // 无：用 Builder 模式或 record
来源：http://lqc.zhiwuduotai.top

Go:   // 无：用配置结构体参数
来源：http://tvn.snrcjt.cn

Ruby: f(a: 1, b: 2)
来源：http://ivf.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://pmk.xinyue.icu

[C05] 返回多个值
来源：http://hto.hesvh.cn

Py:   return a, b
来源：http://asd.gotoacloud.top

PHP:  return [$a, $b];
来源：http://sdn.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lql.ydjk.org.cn

TS:   return { a, b };
来源：http://ixd.jyoumei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wlm.hnxiangtu.top

Go:   return a, b
来源：http://bhl.jinyuanbaomall.cn

Ruby: return a, b
来源：http://ysm.jinqigfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://qvg.yj202588.top

[C06] 匿名函数 / lambda
来源：http://lgw.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://xax.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://tfa.yj202588.top

JS:   const square = x => x * x;
来源：http://nza.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://gxi.sjlbkw.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rru.aibaodan.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gyb.bjfxy.top

Ruby: square = ->(x) { x * x }
来源：http://suv.daria6918.cn


<!-- 参考信息 -->