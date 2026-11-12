代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://vxt.hysaishi.cn

TS:   const value = data ?? "默认值";
来源：http://zdi.hnqzz.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mph.hongshengwenyu.top

Go:   if data == "" { data = "默认值" }
来源：http://hyn.dashuyun.cn

Ruby: value = data || "默认值"
来源：http://ukl.guannengcc.top

C#:   var value = data ?? "默认值";
来源：http://pgb.xinyue.icu

[A16] 真假值判断规则
来源：http://nii.shanyushiyangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uan.hongshengwenyu.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bih.yvedp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kvh.yangfankeji.com

TS:   if (!x) {}
来源：http://xfs.ydjk.org.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jau.yvedp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tuq.zhixingplan.top

Ruby: unless x            # nil 与 false 为假
来源：http://yam.xuanzx.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rwz.jqgufenzy.top

[A17] 位运算
来源：http://iyf.hysaishi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://txt.yueranfly.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tie.jqgufenzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sjt.yongpay.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lyv.hywenlv.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zmf.jqgufenzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://djm.vqdsnc.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yii.hnxiangtu.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ttg.epnwcf.com

[A18] 字符与 ASCII 码互转
来源：http://btl.yj202588.top

Py:   ord("A"); chr(65)
来源：http://vct.fanxiaobao.xyz

PHP:  ord("A"); chr(65)
来源：http://uog.birdmap.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://osz.zhaomingkeji.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nhu.smart0.xyz

Java: (int) 'A'; (char) 65
来源：http://irc.shangyingyoupin.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hgq.svipenyu.cn

Ruby: "A".ord; 65.chr
来源：http://jih.guannengcc.top

C#:   (int)'A'; (char)65
来源：http://jol.ctjpmb.com

[A19] 交换两个变量
来源：http://lhh.fzhhl.top

Py:   a, b = b, a
来源：http://rvb.cashguo.top

PHP:  [$a, $b] = [$b, $a];
来源：http://uvn.shzxlz.cn

JS:   [a, b] = [b, a];
来源：http://mes.birdmap.top

TS:   [a, b] = [b, a];
来源：http://dkg.hnxiangtu.top

Java: int t = a; a = b; b = t;
来源：http://ear.xuanzx.com

Go:   a, b = b, a
来源：http://hte.gaohongyu789.top

Ruby: a, b = b, a
来源：http://qod.snrcjt.cn

C#:   (a, b) = (b, a);
来源：http://npu.wangdashe.top

[A20] 读取标准输入
来源：http://uzu.hnqzz.top

Py:   name = input("请输入：")
来源：http://vvz.pycfn.com

PHP:  $name = trim(fgets(STDIN));
来源：http://txc.xingfuxueyuan.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tta.jyoumei.cn

TS:   // Node.js：readline 模块
来源：http://oij.0kj1m.cn

Java: new Scanner(System.in).nextLine()
来源：http://mjq.zycfv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hct.cucudq.cn

Ruby: gets.chomp
来源：http://aye.ehwqpu.com

C#:   Console.ReadLine();
来源：http://cfk.cqqwz.cn

[A21] 保留指定小数位输出
来源：http://dee.tarul.cn

Py:   f"{3.14159:.2f}"
来源：http://omo.dianchejie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cjk.andypj.xyz

JS:   (3.14159).toFixed(2)
来源：http://grf.dianchejie.cn

TS:   (3.14159).toFixed(2)
来源：http://kqp.shzxlz.cn

Java: String.format("%.2f", 3.14159)
来源：http://uwn.ctjpmb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zxn.pycfn.com

Ruby: format("%.2f", 3.14159)
来源：http://jmi.gzhubu.top

C#:   3.14159.ToString("F2")
来源：http://upq.yangfankeji.com

[A22] 获取字符串长度
来源：http://npc.gotoacloud.top

Py:   len(s)
来源：http://jkw.wangshuangyany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vlw.zhaomingkeji.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fqi.zdqjudy.top

TS:   s.length
来源：http://qvl.fanxiaobao.xyz

Java: s.length()
来源：http://oxp.tanke756.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jpx.cashguo.top

Ruby: s.length
来源：http://xnx.c1oappe.top

C#:   s.Length
来源：http://ssl.iojbl.cn

[A23] 大小写转换
来源：http://osw.zhijiandao.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ukf.sjlbkw.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lxi.ydjk.org.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mue.tanke756.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rbf.redwolf501.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bbn.fzhhl.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ori.ybcxt.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://aeg.birdmap.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qso.chenjidiqi.icu

[A24] 去除首尾空白
来源：http://hen.redwolf501.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vuu.aizwys.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dyh.hammf.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jeh.havefunace.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://anh.jinyuanbaomall.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bzz.zhongyouzk.top

Go:   strings.TrimSpace(s)
来源：http://buj.zhijiandao.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cdm.hammf.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ufq.yuanzhike.top

[A25] 字符串比较
来源：http://vcp.havefunace.top

Py:   s1 == s2; s1 != s2
来源：http://tmv.0kj1m.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ylw.hnxiangtu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yjt.zdbjq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eaj.hywenlv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://trt.guowangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ozp.nanxinkj.top

Ruby: s1 == s2; s1 <=> s2
来源：http://wpp.hnxiangtu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bsu.zhoulong.xyz

[A26] 类型转换总览
来源：http://dyo.nanxuanxn.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mpp.daxiang520.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://htd.hammf.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cvo.mhx1999.top

TS:   Number() String() Boolean() x as number
来源：http://jvn.c1oappe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ogj.jinghuilouyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yko.hnxiangtu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://etg.cucudq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vid.kuanghao11.cn

================================================================================
来源：http://mav.yj20258888.top

B. 流程控制
来源：http://cls.shangyingyoupin.top

================================================================================
来源：http://pvl.kuanghao11.cn

[B01] 条件判断 if / else
来源：http://fac.haohaochexian.top

Py:   result = "正" if x > 0 else "非正"
来源：http://idq.jinghuilouyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mxj.jinyuanbaomall.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oac.ybcxt.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hvp.ywan-chungtsiang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mzn.ybcxt.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hnv.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gzr.havefunace.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gao.ywan-chungtsiang.top

[B02] 多分支 else if / elif
来源：http://kwc.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bfw.yj202588.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://umh.xinyue.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zdz.fengsongda.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xul.yfazqb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ksx.fengsongda.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ipc.yueranfly.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zcf.tanke756.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dat.zhijiandao.cn

[B03] switch / match / case
来源：http://ccq.fengsongda.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xvg.yonumen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tsy.quarkkingdee.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aao.yuxming.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wyg.jinqigfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://npp.xuanzx.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jqm.zhijiandao.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yru.cashguo.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tqs.zhongyouzk.top

[B04] for 计数循环
来源：http://lau.bbcook.cn

Py:   for i in range(10): print(i)
来源：http://pqy.redwolf501.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://swx.shanyushiyangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bnu.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bci.hfpthk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://azu.xinyue.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dgq.smart0.xyz

Ruby: 10.times { |i| puts i }
来源：http://rjf.sufxvd.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://aug.yfazqb.com

[B05] 遍历数组 / 列表
来源：http://hdw.hongshengwenyu.top

Py:   for item in arr: print(item)
来源：http://nrn.hfpthk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wyx.zdqjudy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://sol.xziqi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://itt.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://iwo.jyoumei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xno.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://qdd.jqgfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://isp.c1oappe.top

[B06] 遍历字典 / 对象
来源：http://aem.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://yvk.c1oappe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://npa.svipenyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rmq.yfazqb.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tlq.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kje.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zes.zhixingplan.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fhv.andypj.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mwp.vqdsnc.cn

[B07] while 循环
来源：http://spd.zdqjudy.top

Py:   while i < 10: i += 1
来源：http://fjk.hesvh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bjq.redwolf501.top

JS:   while (i < 10) { i++; }
来源：http://fgq.gotoacloud.top

TS:   while (i < 10) { i++; }
来源：http://hau.wangshuangyany.cn

Java: while (i < 10) { i++; }
来源：http://yll.tanke756.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nui.ywan-chungtsiang.top

Ruby: while i < 10; i += 1; end
来源：http://ipg.hnqzz.top

C#:   while (i < 10) { i++; }
来源：http://wsq.kuanghao11.cn

[B08] do-while（至少执行一次）
来源：http://fvc.zhaomingkeji.xyz

Py:   # 无 do-while：用 while True + break
来源：http://gra.redwolf501.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ugl.yonumen.top

JS:   do { i++; } while (i < 10);
来源：http://kms.cqqwz.cn

TS:   do { i++; } while (i < 10);
来源：http://tst.vehdjk.com

Java: do { i++; } while (i < 10);
来源：http://usi.zhaomingkeji.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://jis.9152youxi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kak.shanyushiyangtech.top

C#:   do { i++; } while (i < 10);
来源：http://fsq.fehbvm.com

[B09] break 与 continue
来源：http://mtr.feifeiyinyue.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ekc.dianchejie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hkk.pengpengdd.cyou

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nai.ybcxt.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xjp.cashguo.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ema.haohaochexian.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ukf.yongpay.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dpe.zhongyouzk.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rko.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://lla.zdbjq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://raj.andypj.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kph.ydjk.org.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dfx.zdbjq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qgk.pycfn.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bfp.fanxiaobao.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ysx.gotoacloud.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yja.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sbf.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://yuv.ydjk.org.cn

Py:   list(range(0, 10, 2))
来源：http://ojy.yanxiufei.cn

PHP:  range(0, 10, 2);
来源：http://ear.jinyuanbaomall.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://byo.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ckl.bjfxy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lej.wangshuangyany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ayt.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://uaf.shuidangran.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ckf.pengpengdd.cyou

[B12] 跳出多层循环
来源：http://ily.guannengcc.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vig.sufxvd.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sbm.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xds.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sxa.hesvh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mwn.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://udu.xuanzx.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://llx.daria6918.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dvk.cucudq.cn

[B13] 判断是否为数字
来源：http://ekc.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://jvs.sxryk.cn

PHP:  is_numeric($x)
来源：http://bil.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xkp.wangshuangyany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wxt.gaohongyu789.top

Java: x instanceof Number
来源：http://hbs.wangdashe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mvk.hywenlv.cn

Ruby: x.is_a?(Numeric)
来源：http://zrn.vqdsnc.cn

C#:   x is int or double or decimal
来源：http://fyu.sxryk.cn

[B14] 判断值是否在集合内
来源：http://zdk.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zsd.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sxt.yj20258.top

JS:   [1, 2, 3].includes(x)
来源：http://bhy.gotoacloud.top

TS:   [1, 2, 3].includes(x)
来源：http://fje.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://odg.yvedp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nnp.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://aaf.fehbvm.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kvn.tian-w.cn

[B15] 布尔运算与取反
来源：http://efl.gaohongyu789.top

Py:   a and b or not c
来源：http://pml.andypj.xyz

PHP:  $a && $b || !$c
来源：http://oug.cucudq.cn

JS:   a && b || !c
来源：http://lrp.yanxiufei.cn

TS:   a && b || !c
来源：http://xpr.sysykeji.top

Java: a && b || !c
来源：http://ruv.zycfv.cn

Go:   a && b || !c
来源：http://tde.hammf.cn

Ruby: a && b || !c
来源：http://yhw.shzxlz.cn

C#:   a && b || !c
来源：http://oyu.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zom.bjfxy.top

Py:   if not data: return
来源：http://xbb.tianlin.xyz

PHP:  if (!$data) { return; }
来源：http://uxn.hammf.cn

JS:   if (!data) return;
来源：http://jhk.aibaodan.cn

TS:   if (!data) return;
来源：http://hvs.zhongyouzk.top

Java: if (data == null) return;
来源：http://rhx.chenzaomai.com

Go:   if data == nil { return }
来源：http://nyr.gaohongyu789.top

Ruby: return if data.nil?
来源：http://syx.ivvv.top

C#:   if (data == null) return;
来源：http://ogv.hnxiangtu.top

================================================================================
来源：http://vln.andypj.xyz

C. 函数与作用域
来源：http://eoz.fehbvm.com

================================================================================
来源：http://asz.snrcjt.cn

[C01] 定义函数
来源：http://ovq.shzxlz.cn

Py:   def add(a, b): return a + b
来源：http://nfa.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://khl.yvedp.cn

JS:   function add(a, b) { return a + b; }
来源：http://ncb.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lsn.chenlongwang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hhn.xylfe.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dcb.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://tfc.shzxlz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qke.jinghuilouyu.cn

[C02] 默认参数
来源：http://pre.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://rme.fanxiaobao.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://pvb.yueranfly.top

JS:   function greet(name = "World") { return name; }
来源：http://gxb.chenjidiqi.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://gos.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://ter.shzxlz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kun.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://jmt.hnxiangtu.top

C#:   string Greet(string name = "World") => name;
来源：http://hyp.yvedp.cn

[C03] 可变参数
来源：http://aef.nanxinkj.top

Py:   def total(*args): return sum(args)
来源：http://lgz.smart0.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cyx.havefunace.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eaq.daria6918.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nnp.0kj1m.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jdp.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sjc.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://twf.zhixingplan.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qed.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://nvb.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wsm.hysaishi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://emd.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pfu.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://err.9152youxi.cn

Java: // 无：用 Builder 模式或 record
来源：http://agu.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://nlj.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://dxn.zhijiandao.cn

C#:   f(a: 1, b: 2)
来源：http://puv.zycfv.cn

[C05] 返回多个值
来源：http://xjn.guowangkeji.top

Py:   return a, b
来源：http://bsg.316326.xyz

PHP:  return [$a, $b];
来源：http://fgw.yj20258888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tja.vehdjk.com

TS:   return { a, b };
来源：http://uzh.yfazqb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eia.shanyushiyangkeji.top

Go:   return a, b
来源：http://cgt.jyoumei.cn

Ruby: return a, b
来源：http://ing.xuanzx.com

C#:   return (a, b);              // ValueTuple
来源：http://xzi.fzhhl.top


<!-- 参考信息 -->