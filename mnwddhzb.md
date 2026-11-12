代发 wailian999

Ruby: value = data || "默认值"
来源：http://ohm.shanyushiyangtech.top

C#:   var value = data ?? "默认值";
来源：http://apn.zhijiandao.cn

[A16] 真假值判断规则
来源：http://yyw.zhoulong.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ijv.daria6918.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xsn.uphjek.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pya.ctjpmb.com

TS:   if (!x) {}
来源：http://nei.zhoulong.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kyr.cqqwz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lkt.yangfankeji.com

Ruby: unless x            # nil 与 false 为假
来源：http://mfj.52xcode.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://twt.xziqi.cn

[A17] 位运算
来源：http://yrb.zhaomingkeji.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eey.quarkkingdee.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fcl.andypj.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ugc.fehbvm.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://svq.ydjk.org.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qyk.jqgfzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mea.wangshuangyany.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aqj.zhoulong.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eor.yuanzhike.top

[A18] 字符与 ASCII 码互转
来源：http://ihp.guowangkeji.top

Py:   ord("A"); chr(65)
来源：http://tkb.zhijiandao.cn

PHP:  ord("A"); chr(65)
来源：http://qui.xinyue.icu

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fcb.fengsongda.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pxd.xinyue.icu

Java: (int) 'A'; (char) 65
来源：http://sfp.zhiwuduotai.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://esy.meibo888.top

Ruby: "A".ord; 65.chr
来源：http://sch.zdbjq.cn

C#:   (int)'A'; (char)65
来源：http://ibd.quarkkingdee.top

[A19] 交换两个变量
来源：http://rft.fehbvm.com

Py:   a, b = b, a
来源：http://jvf.quarkkingdee.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dyl.daxiang520.top

JS:   [a, b] = [b, a];
来源：http://epr.jqgufenzy.top

TS:   [a, b] = [b, a];
来源：http://bdk.yj20258.top

Java: int t = a; a = b; b = t;
来源：http://zcq.fehbvm.com

Go:   a, b = b, a
来源：http://lys.meibo888.top

Ruby: a, b = b, a
来源：http://amd.nanxuanxn.top

C#:   (a, b) = (b, a);
来源：http://xba.havefunace.top

[A20] 读取标准输入
来源：http://ikm.yj20258.top

Py:   name = input("请输入：")
来源：http://ery.shuidangran.top

PHP:  $name = trim(fgets(STDIN));
来源：http://lxt.jqgfzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jgg.zhaomingkeji.xyz

TS:   // Node.js：readline 模块
来源：http://zog.zhixingplan.top

Java: new Scanner(System.in).nextLine()
来源：http://xbr.chenlongwang.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rhr.zycfv.cn

Ruby: gets.chomp
来源：http://ber.yfazqb.com

C#:   Console.ReadLine();
来源：http://zrw.tian-w.cn

[A21] 保留指定小数位输出
来源：http://fsh.zhijiandao.cn

Py:   f"{3.14159:.2f}"
来源：http://hnh.yueranfly.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dqg.cashguo.top

JS:   (3.14159).toFixed(2)
来源：http://ysu.ywan-chungtsiang.top

TS:   (3.14159).toFixed(2)
来源：http://fjp.sjlbkw.cn

Java: String.format("%.2f", 3.14159)
来源：http://zxt.jqgfzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hin.zhijiandao.cn

Ruby: format("%.2f", 3.14159)
来源：http://uhu.zhengqikj.top

C#:   3.14159.ToString("F2")
来源：http://htw.meibo888.top

[A22] 获取字符串长度
来源：http://tps.aizwys.cn

Py:   len(s)
来源：http://djz.yueranfly.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mvj.tanke756.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cqn.hnxiangtu.top

TS:   s.length
来源：http://mfd.meibo888.top

Java: s.length()
来源：http://oic.mhx1999.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jfh.xylfe.cn

Ruby: s.length
来源：http://utz.zdbjq.cn

C#:   s.Length
来源：http://zgs.aibaodan.cn

[A23] 大小写转换
来源：http://ugj.meibo888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://evv.gzhubu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hdc.sufxvd.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dnc.dashuyun.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ohl.daxiang520.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jcr.svipenyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qjf.aibaodan.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xda.yonumen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hoh.andypj.xyz

[A24] 去除首尾空白
来源：http://mly.fanxiaobao.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zcu.guowangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ywu.uphjek.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cad.gaohongyu789.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://glk.yj20258.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mwa.shanyushiyangtech.top

Go:   strings.TrimSpace(s)
来源：http://fan.jinyuanbaomall.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ofn.jiagoushi.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://upp.zhengqikj.top

[A25] 字符串比较
来源：http://pkp.tianlin.xyz

Py:   s1 == s2; s1 != s2
来源：http://ost.sysykeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jqk.yongpay.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gci.fengsongda.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nbz.andypj.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hqz.ehwqpu.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://slo.jqgfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kpl.zhixingplan.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eni.tarul.cn

[A26] 类型转换总览
来源：http://maq.snrcjt.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eou.havefunace.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lgr.pengpengdd.cyou

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xmr.fktsv.cn

TS:   Number() String() Boolean() x as number
来源：http://plf.cucudq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xdj.0kj1m.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://osl.hysaishi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mzl.redwolf501.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oms.ydjk.org.cn

================================================================================
来源：http://ddi.zycfv.cn

B. 流程控制
来源：http://mwh.pengpengdd.cyou

================================================================================
来源：http://jhx.zhiwuduotai.top

[B01] 条件判断 if / else
来源：http://aus.kuanghao11.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hmx.aizwys.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pao.fehbvm.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cwr.hammf.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tjk.hammf.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kdu.chenjidiqi.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kcj.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nci.yvedp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ynu.shuidangran.top

[B02] 多分支 else if / elif
来源：http://hbt.yfazqb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ovu.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pek.yangfankeji.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://irs.jlsjyb.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wgb.shanyushiyangtech.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bug.meibo888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bep.pengpengdd.cyou

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fjo.jqgfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://krz.gaohongyu789.top

[B03] switch / match / case
来源：http://wgo.shzxlz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yjo.yonumen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ogq.yuanzhike.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qcx.xuanzx.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fpi.xingfuxueyuan.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lpl.52xcode.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ozt.daria6918.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://htn.tarul.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dcg.gogol.net.cn

[B04] for 计数循环
来源：http://hkh.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://ney.aizwys.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://trs.zhixingplan.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cfe.zhoulong.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lsd.sjlbkw.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lpc.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vsr.yvedp.cn

Ruby: 10.times { |i| puts i }
来源：http://ewf.jinyuanbaomall.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://woc.xylfe.cn

[B05] 遍历数组 / 列表
来源：http://smb.sxryk.cn

Py:   for item in arr: print(item)
来源：http://qsf.guannengcc.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lxb.yuxming.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sup.cqqwz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rpw.shanyushiyangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://odw.nanxinkj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zcf.nanxuanxn.top

Ruby: arr.each { |item| puts item }
来源：http://fnr.daxiang520.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pbn.bjfxy.top

[B06] 遍历字典 / 对象
来源：http://vvq.havefunace.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jin.yfazqb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bho.fengsongda.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zyj.bbcook.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zhh.gaohongyu789.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qfs.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kgx.jianghu66.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fpr.zhoulong.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pet.xziqi.cn

[B07] while 循环
来源：http://usi.xziqi.cn

Py:   while i < 10: i += 1
来源：http://jjk.gaohongyu789.top

PHP:  while ($i < 10) { $i++; }
来源：http://mmr.xingfuxueyuan.xyz

JS:   while (i < 10) { i++; }
来源：http://thz.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://hft.nanxinkj.top

Java: while (i < 10) { i++; }
来源：http://kpn.yuanzhike.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xhx.zdbjq.cn

Ruby: while i < 10; i += 1; end
来源：http://pnh.nanxinkj.top

C#:   while (i < 10) { i++; }
来源：http://fqj.tianlin.xyz

[B08] do-while（至少执行一次）
来源：http://npi.xuanzx.com

Py:   # 无 do-while：用 while True + break
来源：http://sxh.aibaodan.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vdz.yj20258.top

JS:   do { i++; } while (i < 10);
来源：http://rpw.dianchejie.cn

TS:   do { i++; } while (i < 10);
来源：http://xsm.redwolf501.top

Java: do { i++; } while (i < 10);
来源：http://ngb.dianchejie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://agx.svipenyu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ncd.yuanzhike.top

C#:   do { i++; } while (i < 10);
来源：http://zqk.tarul.cn

[B09] break 与 continue
来源：http://pqz.fktsv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lrd.wangshuangyany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dmb.chenjidiqi.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzg.nanxinkj.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xgn.sweek.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rre.shanyushiyangtech.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jdd.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lui.jianghu66.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://srr.vehdjk.com

[B10] 遍历同时拿索引
来源：http://khc.sjlbkw.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tit.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vhk.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ihn.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fcc.shanyushiyangtech.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zkj.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zmz.xinyue.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://imq.feifeiyinyue.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nlw.jianghu66.top

[B11] 生成数字序列 / 区间
来源：http://fva.bbcook.cn

Py:   list(range(0, 10, 2))
来源：http://lar.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://fdl.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mpn.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rew.tian-w.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zlz.tianlin.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yud.zhengqikj.top

Ruby: (0...10).step(2).to_a
来源：http://wci.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iiq.sjlbkw.cn

[B12] 跳出多层循环
来源：http://dvw.epnwcf.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://hsi.hnqzz.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bhe.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kik.smart0.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://son.cheryme.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qme.mhx1999.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://phh.hesvh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fxs.snrcjt.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dzv.fehbvm.com

[B13] 判断是否为数字
来源：http://ffr.svipenyu.cn

Py:   isinstance(x, (int, float))
来源：http://fyh.hnqzz.top

PHP:  is_numeric($x)
来源：http://uro.shanyushiyangtech.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ffj.jqgfzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rpa.yuanzhike.top

Java: x instanceof Number
来源：http://pav.daxiang520.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nua.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://uae.ctjpmb.com

C#:   x is int or double or decimal
来源：http://iej.smart0.xyz

[B14] 判断值是否在集合内
来源：http://isp.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kac.mhx1999.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uiz.vehdjk.com

JS:   [1, 2, 3].includes(x)
来源：http://myq.vehdjk.com

TS:   [1, 2, 3].includes(x)
来源：http://wmb.sxryk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jus.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ull.zhiwuduotai.top

Ruby: [1, 2, 3].include?(x)
来源：http://ead.cdnleiting.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dvh.zdbjq.cn

[B15] 布尔运算与取反
来源：http://uhe.xuetiantiany.cn

Py:   a and b or not c
来源：http://cqx.cqqwz.cn

PHP:  $a && $b || !$c
来源：http://omk.mhx1999.top

JS:   a && b || !c
来源：http://dhk.ivvv.top

TS:   a && b || !c
来源：http://jev.ppjwa.cn

Java: a && b || !c
来源：http://ovf.tanke756.top

Go:   a && b || !c
来源：http://spa.fktsv.cn

Ruby: a && b || !c
来源：http://ulq.hfpthk.cn

C#:   a && b || !c
来源：http://vcl.gotoacloud.top

[B16] 卫语句：不满足条件提前返回
来源：http://plw.gotoacloud.top

Py:   if not data: return
来源：http://isg.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://yak.yfazqb.com

JS:   if (!data) return;
来源：http://mav.cheryme.top

TS:   if (!data) return;
来源：http://ncz.havefunace.top

Java: if (data == null) return;
来源：http://lso.quarkkingdee.top

Go:   if data == nil { return }
来源：http://xhg.iojbl.cn

Ruby: return if data.nil?
来源：http://lng.dianchejie.cn

C#:   if (data == null) return;
来源：http://grm.guowangkeji.top

================================================================================
来源：http://yqh.tanke756.top

C. 函数与作用域
来源：http://ifl.hnqzz.top

================================================================================
来源：http://atg.sweek.top

[C01] 定义函数
来源：http://xau.tianlin.xyz

Py:   def add(a, b): return a + b
来源：http://sfl.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zvz.fktsv.cn

JS:   function add(a, b) { return a + b; }
来源：http://vmy.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sat.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kws.chenzaomai.com

Go:   func add(a, b int) int { return a + b }
来源：http://wqv.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://fme.ehwqpu.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mkk.tanke756.top

[C02] 默认参数
来源：http://gch.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://gbq.jlsjyb.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zdl.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://meu.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://qrg.xingfuxueyuan.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://bou.hongshengwenyu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dnc.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://nif.jinyuanbaomall.cn

C#:   string Greet(string name = "World") => name;
来源：http://ikn.hongshengwenyu.top

[C03] 可变参数
来源：http://ami.bjfxy.top

Py:   def total(*args): return sum(args)
来源：http://phr.daria6918.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ygs.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://asi.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://usc.sysykeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iut.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nkn.haohaochexian.top

Ruby: def total(*nums); nums.sum; end
来源：http://pzb.shuidangran.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lrp.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://njx.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wcs.cdnleiting.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cfn.jlsjyb.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kqi.bjfxy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://egh.zhengqikj.top

Java: // 无：用 Builder 模式或 record
来源：http://sdk.zhengqikj.top

Go:   // 无：用配置结构体参数
来源：http://sbt.zhijiandao.cn

Ruby: f(a: 1, b: 2)
来源：http://kgp.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://tki.jiagoushi.top

[C05] 返回多个值
来源：http://vts.tarul.cn

Py:   return a, b
来源：http://jbx.cqqwz.cn

PHP:  return [$a, $b];
来源：http://rha.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dbv.jinghuilouyu.cn

TS:   return { a, b };
来源：http://mbp.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jxx.vqdsnc.cn

Go:   return a, b
来源：http://uap.guannengcc.top

Ruby: return a, b
来源：http://uuu.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://lvh.fanxiaobao.xyz

[C06] 匿名函数 / lambda
来源：http://jym.uphjek.com

Py:   square = lambda x: x * x
来源：http://mzo.yonumen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ska.jinqigfzy.top

JS:   const square = x => x * x;
来源：http://qnu.birdmap.top


<!-- 参考信息 -->