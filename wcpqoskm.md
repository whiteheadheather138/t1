代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://idz.tianlin.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ilk.jqgfzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rmp.tarul.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dzl.ydzc1.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vvf.gaohongyu789.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hbb.daxiang520.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fgu.daria6918.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vdy.jinqigufen.top

[A18] 字符与 ASCII 码互转
来源：http://xdc.ppjwa.cn

Py:   ord("A"); chr(65)
来源：http://iup.ctjpmb.com

PHP:  ord("A"); chr(65)
来源：http://qwi.cucudq.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hmd.yonumen.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uxd.zhiwuduotai.top

Java: (int) 'A'; (char) 65
来源：http://drj.nanxinkj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://iyn.redwolf501.top

Ruby: "A".ord; 65.chr
来源：http://gde.nanxuanxn.top

C#:   (int)'A'; (char)65
来源：http://uyt.zhengqikj.top

[A19] 交换两个变量
来源：http://joq.jiagoushi.top

Py:   a, b = b, a
来源：http://egy.hfpthk.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qjo.zhongyouzk.top

JS:   [a, b] = [b, a];
来源：http://hwj.sweek.top

TS:   [a, b] = [b, a];
来源：http://dyd.yj20258.top

Java: int t = a; a = b; b = t;
来源：http://hgg.zdbjq.cn

Go:   a, b = b, a
来源：http://zxq.xylfe.cn

Ruby: a, b = b, a
来源：http://hzn.yfazqb.com

C#:   (a, b) = (b, a);
来源：http://hpi.uphjek.com

[A20] 读取标准输入
来源：http://fbg.cdnleiting.top

Py:   name = input("请输入：")
来源：http://vcj.ehwqpu.com

PHP:  $name = trim(fgets(STDIN));
来源：http://wcx.dianchejie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://asj.zhengqikj.top

TS:   // Node.js：readline 模块
来源：http://puz.iojbl.cn

Java: new Scanner(System.in).nextLine()
来源：http://yvn.jinghuilouyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://afh.nanxuanxn.top

Ruby: gets.chomp
来源：http://rpv.yanxiufei.cn

C#:   Console.ReadLine();
来源：http://pdz.gaohongyu789.top

[A21] 保留指定小数位输出
来源：http://dfu.tianlin.xyz

Py:   f"{3.14159:.2f}"
来源：http://tgj.sxryk.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dnz.uphjek.com

JS:   (3.14159).toFixed(2)
来源：http://cug.ybcxt.top

TS:   (3.14159).toFixed(2)
来源：http://urc.ctjpmb.com

Java: String.format("%.2f", 3.14159)
来源：http://jeo.bbcook.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gbh.ppjwa.cn

Ruby: format("%.2f", 3.14159)
来源：http://mzq.kuanghao11.cn

C#:   3.14159.ToString("F2")
来源：http://woq.zdqjudy.top

[A22] 获取字符串长度
来源：http://tqf.zycfv.cn

Py:   len(s)
来源：http://lts.snrcjt.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uhn.gotoacloud.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fla.yongpay.top

TS:   s.length
来源：http://mmi.hammf.cn

Java: s.length()
来源：http://lfx.sysykeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://obr.jiagoushi.top

Ruby: s.length
来源：http://nyp.kuanghao11.cn

C#:   s.Length
来源：http://gbm.birdmap.top

[A23] 大小写转换
来源：http://slb.fanxiaobao.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://rnq.dashuyun.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qjr.cashguo.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ixn.jinyuanbaomall.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yud.ivvv.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lcu.cheryme.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lth.fehbvm.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jkp.ydzc1.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ewr.yanxiufei.cn

[A24] 去除首尾空白
来源：http://jim.xziqi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tjm.bjfxy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eap.yongpay.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dyv.hcnkem.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nqw.daxiang520.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jxh.yangfankeji.com

Go:   strings.TrimSpace(s)
来源：http://tcf.zhongyouzk.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fpp.ppjwa.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sny.9152youxi.cn

[A25] 字符串比较
来源：http://gwm.guannengcc.top

Py:   s1 == s2; s1 != s2
来源：http://cpe.dashuyun.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wrj.shuidangran.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rmk.pycfn.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://thn.yj20258888.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zhx.zhongyouzk.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hdu.52xcode.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ucg.tianlin.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qze.sxryk.cn

[A26] 类型转换总览
来源：http://thb.sysykeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://llr.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gga.daria6918.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tkc.iojbl.cn

TS:   Number() String() Boolean() x as number
来源：http://oia.shanyushiyangtech.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bvd.zycfv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vsy.kuanghao11.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fir.andypj.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dfd.shangyingyoupin.top

================================================================================
来源：http://vhx.jyoumei.cn

B. 流程控制
来源：http://ldn.xuanzx.com

================================================================================
来源：http://qjx.hammf.cn

[B01] 条件判断 if / else
来源：http://ojp.yonumen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ghz.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hcc.aibaodan.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kht.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hgt.xinyue.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://ulc.quarkkingdee.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://teo.pycfn.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bgo.jlsjyb.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vqo.shzxlz.cn

[B02] 多分支 else if / elif
来源：http://nzd.yj20258888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vyi.hcnkem.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vqe.yfazqb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yas.zhixingplan.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ohk.feifeiyinyue.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dad.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://exz.jiagoushi.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rzd.havefunace.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mqy.guannengcc.top

[B03] switch / match / case
来源：http://lth.yanxiufei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gql.jyoumei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mib.bjfxy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jae.hfpthk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lae.epnwcf.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://owd.jlsjyb.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lhx.zdbjq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xaw.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sfu.jqgfzy.top

[B04] for 计数循环
来源：http://xit.0kj1m.cn

Py:   for i in range(10): print(i)
来源：http://dko.pycfn.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sme.jinqigufen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://luu.jlsjyb.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jtp.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rqn.cucudq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://khl.ivvv.top

Ruby: 10.times { |i| puts i }
来源：http://yso.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xaa.xuanzx.com

[B05] 遍历数组 / 列表
来源：http://jbu.bbcook.cn

Py:   for item in arr: print(item)
来源：http://ozh.yonumen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ffy.yangfankeji.com

JS:   for (const item of arr) { console.log(item); }
来源：http://tap.sweek.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xon.hywenlv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qsv.meibo888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jam.zhiwuduotai.top

Ruby: arr.each { |item| puts item }
来源：http://niz.ybcxt.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://phr.316326.xyz

[B06] 遍历字典 / 对象
来源：http://kfm.jinqigufen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cvh.yj202588.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zpf.wangshuangyany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wiz.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bnn.zhongyouzk.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uvu.sweek.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cbw.316326.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oot.fengsongda.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vnj.svipenyu.cn

[B07] while 循环
来源：http://aih.hnqzz.top

Py:   while i < 10: i += 1
来源：http://iia.ehwqpu.com

PHP:  while ($i < 10) { $i++; }
来源：http://orh.yuxming.cn

JS:   while (i < 10) { i++; }
来源：http://bqs.vqdsnc.cn

TS:   while (i < 10) { i++; }
来源：http://uzv.sjlbkw.cn

Java: while (i < 10) { i++; }
来源：http://qhc.yangfankeji.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vqc.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://kix.hesvh.cn

C#:   while (i < 10) { i++; }
来源：http://nva.cheryme.top

[B08] do-while（至少执行一次）
来源：http://jgn.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://ogb.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pon.nwbrower.top

JS:   do { i++; } while (i < 10);
来源：http://dpb.xinyue.icu

TS:   do { i++; } while (i < 10);
来源：http://snb.zhijiandao.cn

Java: do { i++; } while (i < 10);
来源：http://che.feifeiyinyue.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pwy.cqqwz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qne.epnwcf.com

C#:   do { i++; } while (i < 10);
来源：http://gcd.guannengcc.top

[B09] break 与 continue
来源：http://cum.zhengqikj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cxr.ydzc1.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nqo.hesvh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lqm.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kwk.shangyingyoupin.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ypn.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://auw.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lun.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fee.ivvv.top

[B10] 遍历同时拿索引
来源：http://bxm.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ytw.hywenlv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ern.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kxc.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ebx.xuetiantiany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zse.gotoacloud.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://djn.smart0.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gpb.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fbh.xingfuxueyuan.xyz

[B11] 生成数字序列 / 区间
来源：http://ecu.nanxuanxn.top

Py:   list(range(0, 10, 2))
来源：http://mnh.yangfankeji.com

PHP:  range(0, 10, 2);
来源：http://mys.feifeiyinyue.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mwo.feifeiyinyue.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kkv.yongpay.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dis.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wga.cucudq.cn

Ruby: (0...10).step(2).to_a
来源：http://zup.jqgfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xth.jqgufenzy.top

[B12] 跳出多层循环
来源：http://jvs.ctjpmb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://ufv.vehdjk.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ixu.ydjk.org.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tya.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://szp.tanke756.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hff.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://chh.yj20258888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xot.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yso.yongpay.top

[B13] 判断是否为数字
来源：http://buo.xylfe.cn

Py:   isinstance(x, (int, float))
来源：http://evp.yueranfly.top

PHP:  is_numeric($x)
来源：http://jtc.shuidangran.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hmh.daxiang520.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ght.gogol.net.cn

Java: x instanceof Number
来源：http://uly.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hoc.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://eyr.sysykeji.top

C#:   x is int or double or decimal
来源：http://hlx.jinqigfzy.top

[B14] 判断值是否在集合内
来源：http://iff.xuetiantiany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bng.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vip.jinyuanbaomall.cn

JS:   [1, 2, 3].includes(x)
来源：http://kqm.fehbvm.com

TS:   [1, 2, 3].includes(x)
来源：http://jhm.wangdashe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wai.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iuc.tianlin.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://mot.dashuyun.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vcq.wangshuangyany.cn

[B15] 布尔运算与取反
来源：http://jbz.wangdashe.top

Py:   a and b or not c
来源：http://zhr.meibo888.top

PHP:  $a && $b || !$c
来源：http://abk.jinqigufen.top

JS:   a && b || !c
来源：http://lgp.guannengcc.top

TS:   a && b || !c
来源：http://oio.ydzc1.top

Java: a && b || !c
来源：http://lzp.shanyushiyangtech.top

Go:   a && b || !c
来源：http://exc.xuetiantiany.cn

Ruby: a && b || !c
来源：http://sqk.ybcxt.top

C#:   a && b || !c
来源：http://fwz.sjlbkw.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cry.cashguo.top

Py:   if not data: return
来源：http://afd.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://tiy.mhx1999.top

JS:   if (!data) return;
来源：http://ber.zhongyouzk.top

TS:   if (!data) return;
来源：http://qpq.chenlongwang.top

Java: if (data == null) return;
来源：http://ncq.hnqzz.top

Go:   if data == nil { return }
来源：http://kjs.hongshengwenyu.top

Ruby: return if data.nil?
来源：http://myz.hammf.cn

C#:   if (data == null) return;
来源：http://yam.yongpay.top

================================================================================
来源：http://cab.snrcjt.cn

C. 函数与作用域
来源：http://tsi.ywan-chungtsiang.top

================================================================================
来源：http://xqq.yongpay.top

[C01] 定义函数
来源：http://fag.zhaomingkeji.xyz

Py:   def add(a, b): return a + b
来源：http://gnu.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rae.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://pgq.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sgm.gotoacloud.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tdh.smart0.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://hvx.ydjk.org.cn

Ruby: def add(a, b); a + b; end
来源：http://mxm.ctjpmb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yck.bbcook.cn

[C02] 默认参数
来源：http://oah.yj20258888.top

Py:   def greet(name="World"): return name
来源：http://xtz.fengsongda.top

PHP:  function greet($name = "World") { return $name; }
来源：http://thu.andypj.xyz

JS:   function greet(name = "World") { return name; }
来源：http://bph.xuetiantiany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rwk.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://tan.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fdd.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://bwx.ydzc1.top

C#:   string Greet(string name = "World") => name;
来源：http://byf.xuanzx.com

[C03] 可变参数
来源：http://foh.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://gdo.tian-w.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ctt.zhoulong.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://axb.tian-w.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lvx.gotoacloud.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://igs.fktsv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uqa.tanke756.top

Ruby: def total(*nums); nums.sum; end
来源：http://mnz.sweek.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tah.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://svo.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sho.zdqjudy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dxu.smart0.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lxt.kuanghao11.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lgu.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://tkg.tarul.cn

Go:   // 无：用配置结构体参数
来源：http://szm.jlsjyb.cn

Ruby: f(a: 1, b: 2)
来源：http://wcr.hfpthk.cn

C#:   f(a: 1, b: 2)
来源：http://ihn.chenlongwang.top

[C05] 返回多个值
来源：http://pji.zhongyouzk.top

Py:   return a, b
来源：http://ljq.jinghuilouyu.cn

PHP:  return [$a, $b];
来源：http://hwj.ydzc1.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ggf.fanxiaobao.xyz

TS:   return { a, b };
来源：http://jqf.hysaishi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rho.haohaochexian.top

Go:   return a, b
来源：http://zpb.hongshengwenyu.top

Ruby: return a, b
来源：http://uun.kuanghao11.cn

C#:   return (a, b);              // ValueTuple
来源：http://dwq.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://ygo.zhixingplan.top

Py:   square = lambda x: x * x
来源：http://wob.gaohongyu789.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rox.ppjwa.cn

JS:   const square = x => x * x;
来源：http://cae.yj20258888.top

TS:   const square = (x: number): number => x * x;
来源：http://ctp.vqdsnc.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wuq.hongshengwenyu.top

Go:   sq := func(x int) int { return x * x }
来源：http://kbd.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://ncc.yanxiufei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cse.zhijiandao.cn

[C07] 把函数作为参数传入
来源：http://ajv.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qcx.vqdsnc.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yde.yueranfly.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://soy.birdmap.top

TS:   arr.map(String)
来源：http://shw.yongpay.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bib.zhixingplan.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uyq.316326.xyz


<!-- 参考信息 -->