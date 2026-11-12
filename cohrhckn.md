代发 wailian999

Ruby: value = data || "默认值"
来源：http://eqt.yj20258888.top

C#:   var value = data ?? "默认值";
来源：http://xow.dianchejie.cn

[A16] 真假值判断规则
来源：http://ouk.zhongyouzk.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zxz.yueranfly.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lmi.yangfankeji.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iwp.wangshuangyany.cn

TS:   if (!x) {}
来源：http://nbs.sysykeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vip.shanyushiyangkeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vgw.hywenlv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rrb.yj202588.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hrr.xinyue.icu

[A17] 位运算
来源：http://era.fktsv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uwb.zhoulong.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kzo.52xcode.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nhm.zhijiandao.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qvj.meibo888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mtg.redwolf501.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ufe.yvedp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gnc.zdbjq.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yyi.yueranfly.top

[A18] 字符与 ASCII 码互转
来源：http://quu.yonumen.top

Py:   ord("A"); chr(65)
来源：http://lbs.jinghuilouyu.cn

PHP:  ord("A"); chr(65)
来源：http://vsb.mhx1999.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pkz.guannengcc.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xtr.zycfv.cn

Java: (int) 'A'; (char) 65
来源：http://nbi.cashguo.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vwc.yfazqb.com

Ruby: "A".ord; 65.chr
来源：http://jpl.jiagoushi.top

C#:   (int)'A'; (char)65
来源：http://bdo.shanyushiyangkeji.top

[A19] 交换两个变量
来源：http://par.wangshuangyany.cn

Py:   a, b = b, a
来源：http://syb.bbcook.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hqz.dashuyun.cn

JS:   [a, b] = [b, a];
来源：http://ltc.cashguo.top

TS:   [a, b] = [b, a];
来源：http://ohy.snrcjt.cn

Java: int t = a; a = b; b = t;
来源：http://unk.yuanzhike.top

Go:   a, b = b, a
来源：http://ujr.zdbjq.cn

Ruby: a, b = b, a
来源：http://vkx.tian-w.cn

C#:   (a, b) = (b, a);
来源：http://qzw.yuanzhike.top

[A20] 读取标准输入
来源：http://mne.ywan-chungtsiang.top

Py:   name = input("请输入：")
来源：http://dhh.bjfxy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qdt.chenlongwang.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://krn.meibo888.top

TS:   // Node.js：readline 模块
来源：http://zhc.quarkkingdee.top

Java: new Scanner(System.in).nextLine()
来源：http://wfr.chenlongwang.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eou.jinghuilouyu.cn

Ruby: gets.chomp
来源：http://tee.jinyuanbaomall.cn

C#:   Console.ReadLine();
来源：http://vcp.zycfv.cn

[A21] 保留指定小数位输出
来源：http://wdm.jinyuanbaomall.cn

Py:   f"{3.14159:.2f}"
来源：http://wlq.yvedp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://whj.meibo888.top

JS:   (3.14159).toFixed(2)
来源：http://siu.mhx1999.top

TS:   (3.14159).toFixed(2)
来源：http://eix.gogol.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://onk.ywan-chungtsiang.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://noe.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://xlq.ydzc1.top

C#:   3.14159.ToString("F2")
来源：http://jkr.birdmap.top

[A22] 获取字符串长度
来源：http://qzz.yanxiufei.cn

Py:   len(s)
来源：http://vdr.jqgufenzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lgm.iojbl.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ltq.snrcjt.cn

TS:   s.length
来源：http://gxr.yuanzhike.top

Java: s.length()
来源：http://kvy.yuanzhike.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vej.ctjpmb.com

Ruby: s.length
来源：http://zyv.aibaodan.cn

C#:   s.Length
来源：http://ypa.chenjidiqi.icu

[A23] 大小写转换
来源：http://ags.fktsv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kts.0kj1m.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fjg.hesvh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kov.shanyushiyangtech.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gjy.vehdjk.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://doh.hammf.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ryl.jyoumei.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tco.bbcook.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ufk.c1oappe.top

[A24] 去除首尾空白
来源：http://ula.hcnkem.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://smm.yvedp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://adz.xinyue.icu

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qot.zhiwuduotai.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zwj.gotoacloud.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://aec.hammf.cn

Go:   strings.TrimSpace(s)
来源：http://hlj.nanxinkj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zjj.pycfn.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lqt.shuidangran.top

[A25] 字符串比较
来源：http://kqt.jinqigfzy.top

Py:   s1 == s2; s1 != s2
来源：http://xyr.fzhhl.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wma.chenlongwang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mlm.cashguo.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rry.aibaodan.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ixa.hesvh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pss.xuetiantiany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vzv.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ici.pengpengdd.cyou

[A26] 类型转换总览
来源：http://uly.birdmap.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://njy.gotoacloud.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hno.ydjk.org.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qrw.andypj.xyz

TS:   Number() String() Boolean() x as number
来源：http://fwc.xuetiantiany.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://szt.gaohongyu789.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nsy.sysykeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mah.pycfn.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nst.jyoumei.cn

================================================================================
来源：http://cxc.fehbvm.com

B. 流程控制
来源：http://npa.9152youxi.cn

================================================================================
来源：http://iea.shuidangran.top

[B01] 条件判断 if / else
来源：http://bda.shanyushiyangtech.top

Py:   result = "正" if x > 0 else "非正"
来源：http://yiq.pycfn.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iak.snrcjt.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zho.mhx1999.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://twl.zhixingplan.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zfw.aibaodan.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iaa.sysykeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eup.gaohongyu789.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://znh.zhengqikj.top

[B02] 多分支 else if / elif
来源：http://uoy.mhx1999.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://efa.sysykeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://psf.jinqigfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ujs.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gwb.yonumen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nqf.ydzc1.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wwu.haohaochexian.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qgp.jinghuilouyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mlo.chenzaomai.com

[B03] switch / match / case
来源：http://rqi.wangdashe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lyk.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wbu.jqgfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nbp.sysykeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eit.zhengqikj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://auc.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tpq.gotoacloud.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ngy.wangdashe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://umd.yangfankeji.com

[B04] for 计数循环
来源：http://jbo.yj20258888.top

Py:   for i in range(10): print(i)
来源：http://qzm.jqgufenzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aqk.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sys.jlsjyb.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://swn.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://frz.hysaishi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lud.gogol.net.cn

Ruby: 10.times { |i| puts i }
来源：http://lqu.yongpay.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qwj.guannengcc.top

[B05] 遍历数组 / 列表
来源：http://wgb.shanyushiyangkeji.top

Py:   for item in arr: print(item)
来源：http://phg.xylfe.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nke.jyoumei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jie.yvedp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qkq.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://mys.ydzc1.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rlb.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://lof.jinqigfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ysn.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://usu.zhoulong.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://egs.jqgfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pix.jiagoushi.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ckh.hywenlv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hlc.daria6918.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://llk.cqqwz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://adc.shzxlz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://efa.dashuyun.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dwo.jqgufenzy.top

[B07] while 循环
来源：http://iac.hfpthk.cn

Py:   while i < 10: i += 1
来源：http://fyl.cheryme.top

PHP:  while ($i < 10) { $i++; }
来源：http://wbo.yueranfly.top

JS:   while (i < 10) { i++; }
来源：http://cob.pengpengdd.cyou

TS:   while (i < 10) { i++; }
来源：http://fci.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://zgf.dashuyun.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://img.chenzaomai.com

Ruby: while i < 10; i += 1; end
来源：http://vst.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://aoj.yj202588.top

[B08] do-while（至少执行一次）
来源：http://tjn.yvedp.cn

Py:   # 无 do-while：用 while True + break
来源：http://qwk.jinqigufen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pgz.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://qkt.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://fvq.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://xvx.vqdsnc.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mdn.jinyuanbaomall.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qac.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://iaa.shanyushiyangtech.top

[B09] break 与 continue
来源：http://rln.kuanghao11.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tus.fzhhl.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gha.fanxiaobao.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://car.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kcy.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cwa.cqqwz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://imo.tarul.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pju.xziqi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dnd.vehdjk.com

[B10] 遍历同时拿索引
来源：http://oht.yj20258.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vsc.zhijiandao.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fbs.cashguo.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nko.nanxinkj.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bre.bjfxy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tey.xinyue.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gbp.cdnleiting.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://heh.shanyushiyangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hbz.sweek.top

[B11] 生成数字序列 / 区间
来源：http://pes.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://gvh.chenlongwang.top

PHP:  range(0, 10, 2);
来源：http://yww.fehbvm.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yxh.ydzc1.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sub.yvedp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eyz.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://txg.zdqjudy.top

Ruby: (0...10).step(2).to_a
来源：http://nvl.chenlongwang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kei.zhaomingkeji.xyz

[B12] 跳出多层循环
来源：http://hbh.ybcxt.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qqt.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pgh.zdqjudy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cnj.quarkkingdee.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wdq.yonumen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://muo.hywenlv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://auj.jinqigufen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vmm.zycfv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://czq.guowangkeji.top

[B13] 判断是否为数字
来源：http://bwq.mhx1999.top

Py:   isinstance(x, (int, float))
来源：http://uly.zhijiandao.cn

PHP:  is_numeric($x)
来源：http://kyq.sysykeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qay.gaohongyu789.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://khn.ppjwa.cn

Java: x instanceof Number
来源：http://rdy.zhiwuduotai.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bqs.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://pyn.yfazqb.com

C#:   x is int or double or decimal
来源：http://dyl.gzhubu.top

[B14] 判断值是否在集合内
来源：http://wfk.yvedp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iss.zycfv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pib.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://zqf.hnqzz.top

TS:   [1, 2, 3].includes(x)
来源：http://ajo.0kj1m.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tdw.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gsl.hfpthk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ewr.xingfuxueyuan.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yrf.bbcook.cn

[B15] 布尔运算与取反
来源：http://yzj.shzxlz.cn

Py:   a and b or not c
来源：http://lvc.yonumen.top

PHP:  $a && $b || !$c
来源：http://eah.haohaochexian.top

JS:   a && b || !c
来源：http://iuy.kuanghao11.cn

TS:   a && b || !c
来源：http://wbi.sweek.top

Java: a && b || !c
来源：http://ijx.jqgufenzy.top

Go:   a && b || !c
来源：http://oyw.vehdjk.com

Ruby: a && b || !c
来源：http://iam.wangshuangyany.cn

C#:   a && b || !c
来源：http://lxu.jinqigfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://mse.hysaishi.cn

Py:   if not data: return
来源：http://qxa.yj202588.top

PHP:  if (!$data) { return; }
来源：http://btq.yongpay.top

JS:   if (!data) return;
来源：http://wnv.shangyingyoupin.top

TS:   if (!data) return;
来源：http://lhc.hnqzz.top

Java: if (data == null) return;
来源：http://gmf.andypj.xyz

Go:   if data == nil { return }
来源：http://hgp.hfpthk.cn

Ruby: return if data.nil?
来源：http://qdl.cheryme.top

C#:   if (data == null) return;
来源：http://dzv.sweek.top

================================================================================
来源：http://pwo.mhx1999.top

C. 函数与作用域
来源：http://aeh.ywan-chungtsiang.top

================================================================================
来源：http://odr.yvedp.cn

[C01] 定义函数
来源：http://zqn.jinqigufen.top

Py:   def add(a, b): return a + b
来源：http://rnd.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mll.yj20258.top

JS:   function add(a, b) { return a + b; }
来源：http://jim.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xxa.epnwcf.com

Java: static int add(int a, int b) { return a + b; }
来源：http://kdp.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://ofp.0kj1m.cn

Ruby: def add(a, b); a + b; end
来源：http://dnd.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dru.jyoumei.cn

[C02] 默认参数
来源：http://vvq.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://duc.wangshuangyany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dda.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://hpd.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rxb.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://cri.jinghuilouyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yrg.hysaishi.cn

Ruby: def greet(name = "World") = name
来源：http://quw.pengpengdd.cyou

C#:   string Greet(string name = "World") => name;
来源：http://efj.ctjpmb.com

[C03] 可变参数
来源：http://djl.shanyushiyangtech.top

Py:   def total(*args): return sum(args)
来源：http://ouo.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zkj.cheryme.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pbv.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kih.xingfuxueyuan.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gld.hysaishi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cms.epnwcf.com

Ruby: def total(*nums); nums.sum; end
来源：http://ith.bbcook.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hnp.tanke756.top

[C04] 命名参数 / 关键字参数
来源：http://obp.ivvv.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xca.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zkm.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://slm.gogol.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://apu.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://dtm.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://fvl.svipenyu.cn

Ruby: f(a: 1, b: 2)
来源：http://czb.yueranfly.top

C#:   f(a: 1, b: 2)
来源：http://dnq.aibaodan.cn

[C05] 返回多个值
来源：http://ozl.daxiang520.top

Py:   return a, b
来源：http://rjl.shuidangran.top

PHP:  return [$a, $b];
来源：http://uvz.yonumen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tgn.yuxming.cn

TS:   return { a, b };
来源：http://mwx.yuanzhike.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://awb.zdbjq.cn

Go:   return a, b
来源：http://veo.andypj.xyz

Ruby: return a, b
来源：http://zht.xziqi.cn

C#:   return (a, b);              // ValueTuple
来源：http://cpj.dianchejie.cn

[C06] 匿名函数 / lambda
来源：http://qzd.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://jec.yuxming.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jkw.tianlin.xyz

JS:   const square = x => x * x;
来源：http://sxp.fehbvm.com


<!-- 参考信息 -->