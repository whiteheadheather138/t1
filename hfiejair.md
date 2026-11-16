代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://gjz.aizwys.cn

[A15] 空值判断与默认值
来源：http://kls.yangfankeji.com

Py:   value = data or "默认值"
来源：http://jeg.cheryme.top

PHP:  $value = $data ?? "默认值";
来源：http://btl.redwolf501.top

JS:   const value = data ?? "默认值";
来源：http://jwn.zhongyouzk.top

TS:   const value = data ?? "默认值";
来源：http://ocj.shzxlz.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zzg.sufxvd.cn

Go:   if data == "" { data = "默认值" }
来源：http://xtt.yj20258.top

Ruby: value = data || "默认值"
来源：http://jmw.vqdsnc.cn

C#:   var value = data ?? "默认值";
来源：http://nes.wangshuangyany.cn

[A16] 真假值判断规则
来源：http://cyz.gzhubu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://clr.shanyushiyangtech.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vvn.52xcode.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jix.sjlbkw.cn

TS:   if (!x) {}
来源：http://upr.hysaishi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vui.vqdsnc.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://key.chenjidiqi.icu

Ruby: unless x            # nil 与 false 为假
来源：http://adu.gzhubu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hxk.fengsongda.top

[A17] 位运算
来源：http://yml.kuanghao11.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nam.ydzc1.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wrl.smart0.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mqk.kuanghao11.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xxt.havefunace.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oee.hnxiangtu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xrx.jinghuilouyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lso.daria6918.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ahk.hnxiangtu.top

[A18] 字符与 ASCII 码互转
来源：http://omg.zhongyouzk.top

Py:   ord("A"); chr(65)
来源：http://oaf.hnqzz.top

PHP:  ord("A"); chr(65)
来源：http://gxx.shuidangran.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://slm.feifeiyinyue.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://azj.fktsv.cn

Java: (int) 'A'; (char) 65
来源：http://gjq.daria6918.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dah.andypj.xyz

Ruby: "A".ord; 65.chr
来源：http://vfx.pycfn.com

C#:   (int)'A'; (char)65
来源：http://bjb.gotoacloud.top

[A19] 交换两个变量
来源：http://spo.hesvh.cn

Py:   a, b = b, a
来源：http://dkq.chenzaomai.com

PHP:  [$a, $b] = [$b, $a];
来源：http://loa.hfpthk.cn

JS:   [a, b] = [b, a];
来源：http://ncd.fanxiaobao.xyz

TS:   [a, b] = [b, a];
来源：http://acm.wangdashe.top

Java: int t = a; a = b; b = t;
来源：http://njr.xuetiantiany.cn

Go:   a, b = b, a
来源：http://gvn.jinqigufen.top

Ruby: a, b = b, a
来源：http://fnt.yueranfly.top

C#:   (a, b) = (b, a);
来源：http://wxw.havefunace.top

[A20] 读取标准输入
来源：http://gsp.sxryk.cn

Py:   name = input("请输入：")
来源：http://gci.hongshengwenyu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ouh.gogol.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fbn.yangfankeji.com

TS:   // Node.js：readline 模块
来源：http://rrn.hnxiangtu.top

Java: new Scanner(System.in).nextLine()
来源：http://vqb.yuanzhike.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pvj.gotoacloud.top

Ruby: gets.chomp
来源：http://trl.zhoulong.xyz

C#:   Console.ReadLine();
来源：http://jpf.hongshengwenyu.top

[A21] 保留指定小数位输出
来源：http://yzp.yj20258888.top

Py:   f"{3.14159:.2f}"
来源：http://cla.zhaomingkeji.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rft.yonumen.top

JS:   (3.14159).toFixed(2)
来源：http://rdr.zhijiandao.cn

TS:   (3.14159).toFixed(2)
来源：http://fnl.yuxming.cn

Java: String.format("%.2f", 3.14159)
来源：http://ety.chenjidiqi.icu

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hgx.jyoumei.cn

Ruby: format("%.2f", 3.14159)
来源：http://eyx.dashuyun.cn

C#:   3.14159.ToString("F2")
来源：http://ojg.jyoumei.cn

[A22] 获取字符串长度
来源：http://clx.wangshuangyany.cn

Py:   len(s)
来源：http://eof.fengsongda.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lzd.mhx1999.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rgi.haohaochexian.top

TS:   s.length
来源：http://jti.svipenyu.cn

Java: s.length()
来源：http://skx.fzhhl.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dfi.gogol.net.cn

Ruby: s.length
来源：http://myb.redwolf501.top

C#:   s.Length
来源：http://vym.zhixingplan.top

[A23] 大小写转换
来源：http://psl.jlsjyb.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lni.tian-w.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nzn.jlsjyb.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://whb.bbcook.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xie.jlsjyb.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hkc.fzhhl.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ukw.zhongyouzk.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zye.tarul.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://icb.xylfe.cn

[A24] 去除首尾空白
来源：http://zyw.yuanzhike.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sdd.kuanghao11.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hzr.fengsongda.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ukd.xylfe.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bhf.meibo888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lck.guannengcc.top

Go:   strings.TrimSpace(s)
来源：http://syf.yj20258888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://suq.shanyushiyangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ojb.xinyue.icu

[A25] 字符串比较
来源：http://byg.iojbl.cn

Py:   s1 == s2; s1 != s2
来源：http://jxm.pycfn.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ybs.zhaomingkeji.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vzk.nwbrower.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rqv.hysaishi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iqp.tianlin.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iga.yangfankeji.com

Ruby: s1 == s2; s1 <=> s2
来源：http://jqw.wangshuangyany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kdu.havefunace.top

[A26] 类型转换总览
来源：http://fxy.ydjk.org.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xbm.wangdashe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vsc.gogol.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hwv.vehdjk.com

TS:   Number() String() Boolean() x as number
来源：http://xft.chenzaomai.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tyc.tanke756.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gfm.hnxiangtu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xnx.gogol.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wpc.c1oappe.top

================================================================================
来源：http://vit.nanxuanxn.top

B. 流程控制
来源：http://snd.yuanzhike.top

================================================================================
来源：http://kxi.shangyingyoupin.top

[B01] 条件判断 if / else
来源：http://nff.zhengqikj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ncx.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qve.fktsv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eel.yj202588.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zmg.sweek.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ynl.zhoulong.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ekv.cqqwz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wdh.nanxuanxn.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://axk.andypj.xyz

[B02] 多分支 else if / elif
来源：http://qjr.jinghuilouyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cvk.birdmap.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mme.nanxinkj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nrk.sufxvd.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iib.ydjk.org.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ban.mhx1999.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ytz.sysykeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qrl.shangyingyoupin.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qct.hysaishi.cn

[B03] switch / match / case
来源：http://gfd.cucudq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qwm.xingfuxueyuan.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oxf.ehwqpu.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dde.guannengcc.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dbi.0kj1m.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uyw.cashguo.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nbn.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pxr.yueranfly.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zwy.zhengqikj.top

[B04] for 计数循环
来源：http://mlo.ctjpmb.com

Py:   for i in range(10): print(i)
来源：http://stg.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dsk.aibaodan.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eez.svipenyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cnt.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mvx.xuanzx.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ydz.guowangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://uhc.cqqwz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nbe.bbcook.cn

[B05] 遍历数组 / 列表
来源：http://tod.jianghu66.top

Py:   for item in arr: print(item)
来源：http://mii.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://plt.yj202588.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vhm.mhx1999.top

TS:   for (const item of arr) { console.log(item); }
来源：http://djn.yvedp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://irc.fehbvm.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://knw.yongpay.top

Ruby: arr.each { |item| puts item }
来源：http://nrq.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dmk.bjfxy.top

[B06] 遍历字典 / 对象
来源：http://swl.gaohongyu789.top

Py:   for k, v in d.items(): print(k, v)
来源：http://sgs.9152youxi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ydq.tian-w.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qlu.epnwcf.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jnc.aizwys.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lkd.xziqi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uwx.zdqjudy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://flh.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bvy.nanxuanxn.top

[B07] while 循环
来源：http://fqf.sxryk.cn

Py:   while i < 10: i += 1
来源：http://tfx.cqqwz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kyx.shangyingyoupin.top

JS:   while (i < 10) { i++; }
来源：http://ylf.aibaodan.cn

TS:   while (i < 10) { i++; }
来源：http://bgj.yonumen.top

Java: while (i < 10) { i++; }
来源：http://ehd.iojbl.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xzf.hongshengwenyu.top

Ruby: while i < 10; i += 1; end
来源：http://ofe.yj202588.top

C#:   while (i < 10) { i++; }
来源：http://dnt.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://nwv.jlsjyb.cn

Py:   # 无 do-while：用 while True + break
来源：http://yjo.fehbvm.com

PHP:  do { $i++; } while ($i < 10);
来源：http://gae.snrcjt.cn

JS:   do { i++; } while (i < 10);
来源：http://lte.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://clx.yueranfly.top

Java: do { i++; } while (i < 10);
来源：http://xer.zdqjudy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pdz.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://xtr.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://kbs.ybcxt.top

[B09] break 与 continue
来源：http://yiu.cdnleiting.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jvt.ehwqpu.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uex.wangshuangyany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iiz.cashguo.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://axz.shangyingyoupin.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nso.daria6918.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zkj.cashguo.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bux.jinghuilouyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rqg.smart0.xyz

[B10] 遍历同时拿索引
来源：http://btw.aibaodan.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://can.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ozs.uphjek.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://irj.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dgk.jiagoushi.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hbk.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://spx.shanyushiyangtech.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nak.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jvb.gotoacloud.top

[B11] 生成数字序列 / 区间
来源：http://xer.xziqi.cn

Py:   list(range(0, 10, 2))
来源：http://qee.sysykeji.top

PHP:  range(0, 10, 2);
来源：http://too.jinyuanbaomall.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pyh.svipenyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xle.kuanghao11.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gwl.guowangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eqk.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://czv.shanyushiyangtech.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://khh.zycfv.cn

[B12] 跳出多层循环
来源：http://sol.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jhm.zhiwuduotai.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ogk.kuanghao11.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tzr.havefunace.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wux.gzhubu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://epj.redwolf501.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mfy.chenjidiqi.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nci.fanxiaobao.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cjp.yonumen.top

[B13] 判断是否为数字
来源：http://hgb.yanxiufei.cn

Py:   isinstance(x, (int, float))
来源：http://fgc.hnqzz.top

PHP:  is_numeric($x)
来源：http://isv.jqgfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fej.svipenyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iyg.chenzaomai.com

Java: x instanceof Number
来源：http://qng.nanxinkj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tvp.svipenyu.cn

Ruby: x.is_a?(Numeric)
来源：http://dkb.cqqwz.cn

C#:   x is int or double or decimal
来源：http://str.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://ojw.chenjidiqi.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://plh.316326.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://khp.ydzc1.top

JS:   [1, 2, 3].includes(x)
来源：http://piq.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://ioj.cqqwz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dhn.meibo888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hde.svipenyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mxx.jlsjyb.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pla.sjlbkw.cn

[B15] 布尔运算与取反
来源：http://vgn.jqgufenzy.top

Py:   a and b or not c
来源：http://ihs.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://ley.sxryk.cn

JS:   a && b || !c
来源：http://yjg.smart0.xyz

TS:   a && b || !c
来源：http://dll.hesvh.cn

Java: a && b || !c
来源：http://usr.yongpay.top

Go:   a && b || !c
来源：http://cuy.xinyue.icu

Ruby: a && b || !c
来源：http://ula.hfpthk.cn

C#:   a && b || !c
来源：http://pwo.uphjek.com

[B16] 卫语句：不满足条件提前返回
来源：http://lyi.gzhubu.top

Py:   if not data: return
来源：http://pof.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://djh.ydzc1.top

JS:   if (!data) return;
来源：http://iob.chenjidiqi.icu

TS:   if (!data) return;
来源：http://guh.ivvv.top

Java: if (data == null) return;
来源：http://acq.nwbrower.top

Go:   if data == nil { return }
来源：http://ffj.gzhubu.top

Ruby: return if data.nil?
来源：http://evh.shuidangran.top

C#:   if (data == null) return;
来源：http://lnb.iojbl.cn

================================================================================
来源：http://xur.xziqi.cn

C. 函数与作用域
来源：http://arr.yfazqb.com

================================================================================
来源：http://gav.zdqjudy.top

[C01] 定义函数
来源：http://gon.cucudq.cn

Py:   def add(a, b): return a + b
来源：http://jvo.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vil.ydjk.org.cn

JS:   function add(a, b) { return a + b; }
来源：http://vqq.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bqs.epnwcf.com

Java: static int add(int a, int b) { return a + b; }
来源：http://zdi.xziqi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oen.pycfn.com

Ruby: def add(a, b); a + b; end
来源：http://rrj.vqdsnc.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eek.zhongyouzk.top

[C02] 默认参数
来源：http://zva.gogol.net.cn

Py:   def greet(name="World"): return name
来源：http://ofx.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://lhe.quarkkingdee.top

JS:   function greet(name = "World") { return name; }
来源：http://zwa.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lkb.yangfankeji.com

Java: // 无默认参数：方法重载或 Optional
来源：http://hph.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gwd.kuanghao11.cn

Ruby: def greet(name = "World") = name
来源：http://mne.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://tlt.shanyushiyangkeji.top

[C03] 可变参数
来源：http://jsv.ydjk.org.cn

Py:   def total(*args): return sum(args)
来源：http://ukq.redwolf501.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pki.fanxiaobao.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iro.yueranfly.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jxb.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jbx.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zkm.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://dcy.fzhhl.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wli.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://qex.52xcode.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qoy.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cxu.hysaishi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bbk.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zcc.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://ide.jinqigufen.top

Go:   // 无：用配置结构体参数
来源：http://srz.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://mty.zhoulong.xyz

C#:   f(a: 1, b: 2)
来源：http://kpm.xziqi.cn

[C05] 返回多个值
来源：http://kvl.gaohongyu789.top

Py:   return a, b
来源：http://phi.cucudq.cn

PHP:  return [$a, $b];
来源：http://pht.zdbjq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zps.uphjek.com

TS:   return { a, b };
来源：http://wvp.cdnleiting.top


<!-- 参考信息 -->