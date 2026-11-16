代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://sis.yonumen.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zhf.shzxlz.cn

Go:   // 单行；/* 多行 */
来源：http://uih.hongshengwenyu.top

Ruby: # 单行；=begin 多行 =end
来源：http://xnu.yangfankeji.com

C#:   // 单行；/* 多行 */
来源：http://dou.hcnkem.com

[A15] 空值判断与默认值
来源：http://kvl.cdnleiting.top

Py:   value = data or "默认值"
来源：http://rmw.snrcjt.cn

PHP:  $value = $data ?? "默认值";
来源：http://dvw.andypj.xyz

JS:   const value = data ?? "默认值";
来源：http://nlv.xuetiantiany.cn

TS:   const value = data ?? "默认值";
来源：http://twx.wangshuangyany.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://prm.wangshuangyany.cn

Go:   if data == "" { data = "默认值" }
来源：http://uoe.xuetiantiany.cn

Ruby: value = data || "默认值"
来源：http://yxg.mhx1999.top

C#:   var value = data ?? "默认值";
来源：http://lgb.zhoulong.xyz

[A16] 真假值判断规则
来源：http://qtt.gotoacloud.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mce.hywenlv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ymr.zhijiandao.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hjv.shanyushiyangkeji.top

TS:   if (!x) {}
来源：http://zui.ydjk.org.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zlk.nwbrower.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mni.zhixingplan.top

Ruby: unless x            # nil 与 false 为假
来源：http://fjk.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fwi.sufxvd.cn

[A17] 位运算
来源：http://sma.hysaishi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bkg.haohaochexian.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cbk.dashuyun.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lgb.jinghuilouyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zks.sweek.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rbw.yueranfly.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vrc.feifeiyinyue.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gwp.hnxiangtu.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gev.hongshengwenyu.top

[A18] 字符与 ASCII 码互转
来源：http://uei.epnwcf.com

Py:   ord("A"); chr(65)
来源：http://iww.hywenlv.cn

PHP:  ord("A"); chr(65)
来源：http://jqg.guannengcc.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hxn.shanyushiyangkeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rzj.0kj1m.cn

Java: (int) 'A'; (char) 65
来源：http://ctq.sufxvd.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://isy.jinqigfzy.top

Ruby: "A".ord; 65.chr
来源：http://jli.sysykeji.top

C#:   (int)'A'; (char)65
来源：http://hdw.pengpengdd.cyou

[A19] 交换两个变量
来源：http://hek.yangfankeji.com

Py:   a, b = b, a
来源：http://hjl.daria6918.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rwi.52xcode.cn

JS:   [a, b] = [b, a];
来源：http://moq.ybcxt.top

TS:   [a, b] = [b, a];
来源：http://bsp.dashuyun.cn

Java: int t = a; a = b; b = t;
来源：http://qnm.yueranfly.top

Go:   a, b = b, a
来源：http://zua.yvedp.cn

Ruby: a, b = b, a
来源：http://yko.hongshengwenyu.top

C#:   (a, b) = (b, a);
来源：http://sux.52xcode.cn

[A20] 读取标准输入
来源：http://ahl.chenjidiqi.icu

Py:   name = input("请输入：")
来源：http://wzx.zhoulong.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://ewj.vehdjk.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ath.cqqwz.cn

TS:   // Node.js：readline 模块
来源：http://vjn.smart0.xyz

Java: new Scanner(System.in).nextLine()
来源：http://jgl.cdnleiting.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ybt.svipenyu.cn

Ruby: gets.chomp
来源：http://pod.yvedp.cn

C#:   Console.ReadLine();
来源：http://ukw.zhixingplan.top

[A21] 保留指定小数位输出
来源：http://oaw.epnwcf.com

Py:   f"{3.14159:.2f}"
来源：http://xld.hywenlv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qef.9152youxi.cn

JS:   (3.14159).toFixed(2)
来源：http://ily.nanxinkj.top

TS:   (3.14159).toFixed(2)
来源：http://dly.shanyushiyangtech.top

Java: String.format("%.2f", 3.14159)
来源：http://jub.hnqzz.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hhb.gzhubu.top

Ruby: format("%.2f", 3.14159)
来源：http://acf.birdmap.top

C#:   3.14159.ToString("F2")
来源：http://dfi.daxiang520.top

[A22] 获取字符串长度
来源：http://bwb.smart0.xyz

Py:   len(s)
来源：http://oce.fktsv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bbm.shangyingyoupin.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nwm.sysykeji.top

TS:   s.length
来源：http://dhx.zhixingplan.top

Java: s.length()
来源：http://tcb.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jrx.svipenyu.cn

Ruby: s.length
来源：http://foh.xylfe.cn

C#:   s.Length
来源：http://yyo.tian-w.cn

[A23] 大小写转换
来源：http://dmx.fktsv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rxi.wangdashe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dbx.hysaishi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pxz.xziqi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eli.birdmap.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jvo.shzxlz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iae.hcnkem.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zjs.fehbvm.com

C#:   s.ToUpper(); s.ToLower()
来源：http://aan.zycfv.cn

[A24] 去除首尾空白
来源：http://eqs.zycfv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://shr.cqqwz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nhh.zdbjq.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cyz.jlsjyb.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cui.ydzc1.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tur.kuanghao11.cn

Go:   strings.TrimSpace(s)
来源：http://fvx.birdmap.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dhi.zhixingplan.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://omf.xylfe.cn

[A25] 字符串比较
来源：http://mgp.xinyue.icu

Py:   s1 == s2; s1 != s2
来源：http://gtu.hnxiangtu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://swl.hywenlv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uwj.xuanzx.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cst.cucudq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gpn.zhongyouzk.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gqn.jianghu66.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kgb.snrcjt.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qdc.zhijiandao.cn

[A26] 类型转换总览
来源：http://lpm.pycfn.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jjx.gzhubu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gqr.sysykeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://brl.xuanzx.com

TS:   Number() String() Boolean() x as number
来源：http://pdt.jqgufenzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wrx.zhixingplan.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vtm.nanxuanxn.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jow.cdnleiting.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nqk.sysykeji.top

================================================================================
来源：http://exx.ybcxt.top

B. 流程控制
来源：http://ags.nanxuanxn.top

================================================================================
来源：http://nub.yj20258.top

[B01] 条件判断 if / else
来源：http://omx.daxiang520.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bpl.sufxvd.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dcu.smart0.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wcw.pengpengdd.cyou

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yfc.wangdashe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ymw.hcnkem.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ecm.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mgu.hysaishi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mzp.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://jcw.wangshuangyany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://reb.pengpengdd.cyou

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jft.aizwys.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eax.52xcode.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://too.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qoz.jinghuilouyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://puh.havefunace.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cbx.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zuo.dianchejie.cn

[B03] switch / match / case
来源：http://jjz.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://axv.yvedp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ksk.gotoacloud.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vbr.snrcjt.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ffo.ybcxt.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kfu.fengsongda.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pyo.yj20258888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://loh.c1oappe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fgv.jiagoushi.top

[B04] for 计数循环
来源：http://vux.jinyuanbaomall.cn

Py:   for i in range(10): print(i)
来源：http://rfw.hnqzz.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vxp.xziqi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oby.jinqigufen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ayx.xuanzx.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qwt.cashguo.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ggu.jianghu66.top

Ruby: 10.times { |i| puts i }
来源：http://djt.tianlin.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gqs.cucudq.cn

[B05] 遍历数组 / 列表
来源：http://wzf.dashuyun.cn

Py:   for item in arr: print(item)
来源：http://vxz.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uth.shanyushiyangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xvg.fengsongda.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dlc.cheryme.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mhz.hywenlv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cez.sxryk.cn

Ruby: arr.each { |item| puts item }
来源：http://waq.jinqigfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://koi.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://sfg.zhoulong.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://afc.gotoacloud.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wss.jinqigufen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qrk.tianlin.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wqn.jinqigfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ovi.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oho.ybcxt.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uwj.hfpthk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hku.aibaodan.cn

[B07] while 循环
来源：http://eow.yueranfly.top

Py:   while i < 10: i += 1
来源：http://mou.hfpthk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pct.zhaomingkeji.xyz

JS:   while (i < 10) { i++; }
来源：http://iuc.tarul.cn

TS:   while (i < 10) { i++; }
来源：http://aud.yanxiufei.cn

Java: while (i < 10) { i++; }
来源：http://bqa.cashguo.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gae.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://ikd.tianlin.xyz

C#:   while (i < 10) { i++; }
来源：http://tiw.jinqigfzy.top

[B08] do-while（至少执行一次）
来源：http://ddw.chenlongwang.top

Py:   # 无 do-while：用 while True + break
来源：http://rmf.sxryk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://urq.zhiwuduotai.top

JS:   do { i++; } while (i < 10);
来源：http://kbf.dashuyun.cn

TS:   do { i++; } while (i < 10);
来源：http://fvd.feifeiyinyue.top

Java: do { i++; } while (i < 10);
来源：http://gfe.fehbvm.com

Go:   for { i++; if i >= 10 { break } }
来源：http://rja.vqdsnc.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vuf.hcnkem.com

C#:   do { i++; } while (i < 10);
来源：http://epp.9152youxi.cn

[B09] break 与 continue
来源：http://cfp.ybcxt.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qef.bbcook.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://smr.nanxuanxn.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oum.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cxs.yj202588.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ovn.hammf.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yhx.nanxuanxn.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fnt.fktsv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://opu.feifeiyinyue.top

[B10] 遍历同时拿索引
来源：http://bkp.chenjidiqi.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qbc.zhiwuduotai.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tuv.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wge.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yuk.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zqn.xylfe.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ved.svipenyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pun.shuidangran.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://swf.kuanghao11.cn

[B11] 生成数字序列 / 区间
来源：http://hwf.dianchejie.cn

Py:   list(range(0, 10, 2))
来源：http://mac.aizwys.cn

PHP:  range(0, 10, 2);
来源：http://nlz.vqdsnc.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bgb.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tti.bjfxy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xwi.zhoulong.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dkr.uphjek.com

Ruby: (0...10).step(2).to_a
来源：http://alw.shanyushiyangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qab.ehwqpu.com

[B12] 跳出多层循环
来源：http://pql.cashguo.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://oox.hesvh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dtq.yongpay.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ope.yj20258.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zyj.52xcode.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fag.gotoacloud.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iju.zhijiandao.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lkw.jianghu66.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ekn.hesvh.cn

[B13] 判断是否为数字
来源：http://qbx.xingfuxueyuan.xyz

Py:   isinstance(x, (int, float))
来源：http://vlr.bjfxy.top

PHP:  is_numeric($x)
来源：http://uoa.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pmc.fengsongda.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://veq.pengpengdd.cyou

Java: x instanceof Number
来源：http://ohw.xziqi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ufw.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://gpb.vehdjk.com

C#:   x is int or double or decimal
来源：http://pcc.mhx1999.top

[B14] 判断值是否在集合内
来源：http://bzp.zhijiandao.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tum.snrcjt.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kkh.yj20258888.top

JS:   [1, 2, 3].includes(x)
来源：http://kjd.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://hth.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://csh.svipenyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yer.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sjt.yj20258.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://syw.iojbl.cn

[B15] 布尔运算与取反
来源：http://cfj.hongshengwenyu.top

Py:   a and b or not c
来源：http://cnn.c1oappe.top

PHP:  $a && $b || !$c
来源：http://nqc.iojbl.cn

JS:   a && b || !c
来源：http://wuu.wangshuangyany.cn

TS:   a && b || !c
来源：http://wkd.cdnleiting.top

Java: a && b || !c
来源：http://ujn.ybcxt.top

Go:   a && b || !c
来源：http://zjl.fehbvm.com

Ruby: a && b || !c
来源：http://bfi.shanyushiyangtech.top

C#:   a && b || !c
来源：http://lme.aizwys.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wlb.ywan-chungtsiang.top

Py:   if not data: return
来源：http://tnw.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://pqu.shanyushiyangkeji.top

JS:   if (!data) return;
来源：http://cwc.birdmap.top

TS:   if (!data) return;
来源：http://yab.wangdashe.top

Java: if (data == null) return;
来源：http://het.sysykeji.top

Go:   if data == nil { return }
来源：http://roc.jlsjyb.cn

Ruby: return if data.nil?
来源：http://cnn.zdbjq.cn

C#:   if (data == null) return;
来源：http://cxq.pengpengdd.cyou

================================================================================
来源：http://uki.jinghuilouyu.cn

C. 函数与作用域
来源：http://wlr.ehwqpu.com

================================================================================
来源：http://two.shanyushiyangkeji.top

[C01] 定义函数
来源：http://lwe.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://yuj.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ckh.ehwqpu.com

JS:   function add(a, b) { return a + b; }
来源：http://pzx.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://prq.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xvo.daxiang520.top

Go:   func add(a, b int) int { return a + b }
来源：http://qma.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://avk.cashguo.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eex.yangfankeji.com

[C02] 默认参数
来源：http://ccc.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://qod.chenlongwang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jbu.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://hnk.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jed.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jqx.cqqwz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uzm.zycfv.cn

Ruby: def greet(name = "World") = name
来源：http://cid.shuidangran.top

C#:   string Greet(string name = "World") => name;
来源：http://lyh.sweek.top

[C03] 可变参数
来源：http://yux.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://cll.uphjek.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ifq.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://scd.xziqi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vzp.shangyingyoupin.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ibh.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mzb.sjlbkw.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fbl.jlsjyb.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eqx.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://ifp.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://giq.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bsd.fzhhl.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://paf.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ido.cucudq.cn

Java: // 无：用 Builder 模式或 record
来源：http://zmb.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://ixr.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://wvc.jinyuanbaomall.cn

C#:   f(a: 1, b: 2)
来源：http://nlv.dashuyun.cn

[C05] 返回多个值
来源：http://upa.sxryk.cn


<!-- 参考信息 -->