代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://raa.jinyuanbaomall.cn

JS:   `Hello, ${name}!`
来源：http://brl.uphjek.com

TS:   `Hello, ${name}!`
来源：http://ggi.zhaomingkeji.xyz

Java: "Hello, %s!".formatted(name)
来源：http://yyz.hongshengwenyu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xyl.jlsjyb.cn

Ruby: "Hello, #{name}!"
来源：http://pvy.ivvv.top

C#:   $"Hello, {name}!"
来源：http://ytt.shanyushiyangkeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://nnp.shanyushiyangkeji.top

Py:   "第一行\n第二行"
来源：http://juu.jqgfzy.top

PHP:  "第一行\n第二行"
来源：http://drc.feifeiyinyue.top

JS:   "第一行\n第二行"
来源：http://xam.jinqigfzy.top

TS:   "第一行\n第二行"
来源：http://khn.gaohongyu789.top

Java: "第一行\n第二行"
来源：http://swf.zhijiandao.cn

Go:   "第一行\n第二行"
来源：http://qab.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://mfd.haohaochexian.top

C#:   "第一行\n第二行"
来源：http://jxz.iojbl.cn

[A14] 注释写法
来源：http://mfp.guowangkeji.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ohq.vqdsnc.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sfi.birdmap.top

JS:   // 单行；/* 多行 */
来源：http://zui.hysaishi.cn

TS:   // 单行；/* 多行 */
来源：http://flz.fanxiaobao.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cej.hfpthk.cn

Go:   // 单行；/* 多行 */
来源：http://wzo.quarkkingdee.top

Ruby: # 单行；=begin 多行 =end
来源：http://muy.svipenyu.cn

C#:   // 单行；/* 多行 */
来源：http://gic.wangshuangyany.cn

[A15] 空值判断与默认值
来源：http://ykg.yj20258888.top

Py:   value = data or "默认值"
来源：http://oht.hongshengwenyu.top

PHP:  $value = $data ?? "默认值";
来源：http://fdn.jqgfzy.top

JS:   const value = data ?? "默认值";
来源：http://kvr.yvedp.cn

TS:   const value = data ?? "默认值";
来源：http://chh.hongshengwenyu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mqf.ehwqpu.com

Go:   if data == "" { data = "默认值" }
来源：http://ngu.xylfe.cn

Ruby: value = data || "默认值"
来源：http://cxw.jlsjyb.cn

C#:   var value = data ?? "默认值";
来源：http://ckp.tarul.cn

[A16] 真假值判断规则
来源：http://yvw.aibaodan.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ayn.yueranfly.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pgj.jyoumei.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iic.shangyingyoupin.top

TS:   if (!x) {}
来源：http://uiz.ehwqpu.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rgc.wangshuangyany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://box.meibo888.top

Ruby: unless x            # nil 与 false 为假
来源：http://mug.snrcjt.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nrh.epnwcf.com

[A17] 位运算
来源：http://cba.ctjpmb.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qcs.zhongyouzk.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fqk.shzxlz.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wld.yj20258888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://drj.yfazqb.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zqv.fanxiaobao.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://enf.bjfxy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vdx.yonumen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bcc.ywan-chungtsiang.top

[A18] 字符与 ASCII 码互转
来源：http://gbn.bbcook.cn

Py:   ord("A"); chr(65)
来源：http://wjx.birdmap.top

PHP:  ord("A"); chr(65)
来源：http://jbr.xuanzx.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fut.snrcjt.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hcq.yanxiufei.cn

Java: (int) 'A'; (char) 65
来源：http://gkq.feifeiyinyue.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pvt.redwolf501.top

Ruby: "A".ord; 65.chr
来源：http://zvw.xuanzx.com

C#:   (int)'A'; (char)65
来源：http://vee.cqqwz.cn

[A19] 交换两个变量
来源：http://jhq.fanxiaobao.xyz

Py:   a, b = b, a
来源：http://uvh.ppjwa.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vgn.zdqjudy.top

JS:   [a, b] = [b, a];
来源：http://txf.smart0.xyz

TS:   [a, b] = [b, a];
来源：http://lqh.hongshengwenyu.top

Java: int t = a; a = b; b = t;
来源：http://ibl.yj20258888.top

Go:   a, b = b, a
来源：http://mla.wangshuangyany.cn

Ruby: a, b = b, a
来源：http://rxm.jinghuilouyu.cn

C#:   (a, b) = (b, a);
来源：http://wlw.epnwcf.com

[A20] 读取标准输入
来源：http://uth.shuidangran.top

Py:   name = input("请输入：")
来源：http://iio.redwolf501.top

PHP:  $name = trim(fgets(STDIN));
来源：http://szw.uphjek.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zgk.meibo888.top

TS:   // Node.js：readline 模块
来源：http://hzs.daxiang520.top

Java: new Scanner(System.in).nextLine()
来源：http://rbe.andypj.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xxv.jinyuanbaomall.cn

Ruby: gets.chomp
来源：http://qls.fanxiaobao.xyz

C#:   Console.ReadLine();
来源：http://hsp.dashuyun.cn

[A21] 保留指定小数位输出
来源：http://ejx.ydjk.org.cn

Py:   f"{3.14159:.2f}"
来源：http://mwv.yueranfly.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xwr.ctjpmb.com

JS:   (3.14159).toFixed(2)
来源：http://sgm.gaohongyu789.top

TS:   (3.14159).toFixed(2)
来源：http://nhr.svipenyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://pjk.cucudq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oqe.chenzaomai.com

Ruby: format("%.2f", 3.14159)
来源：http://rah.yj202588.top

C#:   3.14159.ToString("F2")
来源：http://uxc.epnwcf.com

[A22] 获取字符串长度
来源：http://uzq.chenjidiqi.icu

Py:   len(s)
来源：http://sxr.zhaomingkeji.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tkm.ivvv.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kok.yueranfly.top

TS:   s.length
来源：http://pgq.fengsongda.top

Java: s.length()
来源：http://nqh.guannengcc.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fop.yueranfly.top

Ruby: s.length
来源：http://iyl.cucudq.cn

C#:   s.Length
来源：http://kwe.yuxming.cn

[A23] 大小写转换
来源：http://mvs.hnxiangtu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ldw.jinghuilouyu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ovw.zhoulong.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://upa.316326.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://glz.jlsjyb.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sby.kuanghao11.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://crx.yuanzhike.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wzk.sysykeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://svq.ivvv.top

[A24] 去除首尾空白
来源：http://nkj.fengsongda.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://miy.svipenyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://foy.sysykeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fxc.c1oappe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nou.yj20258888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lcl.316326.xyz

Go:   strings.TrimSpace(s)
来源：http://ymh.jqgufenzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://roq.shanyushiyangtech.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://osg.cheryme.top

[A25] 字符串比较
来源：http://dke.snrcjt.cn

Py:   s1 == s2; s1 != s2
来源：http://kng.nwbrower.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://brx.zhongyouzk.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lbe.sjlbkw.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vtw.hnxiangtu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://grw.wangdashe.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hrb.zhijiandao.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cfh.hysaishi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rjp.jiagoushi.top

[A26] 类型转换总览
来源：http://zjj.aizwys.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://swc.iojbl.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rvq.nanxinkj.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://beh.daxiang520.top

TS:   Number() String() Boolean() x as number
来源：http://qyx.hammf.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kuw.c1oappe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ccl.gzhubu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://hwn.nanxuanxn.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yqj.gaohongyu789.top

================================================================================
来源：http://wga.feifeiyinyue.top

B. 流程控制
来源：http://guc.xziqi.cn

================================================================================
来源：http://cff.hfpthk.cn

[B01] 条件判断 if / else
来源：http://kui.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://ngu.jinyuanbaomall.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rbo.bjfxy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vot.chenlongwang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yrr.chenlongwang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jik.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hlr.meibo888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kzt.52xcode.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dbp.fengsongda.top

[B02] 多分支 else if / elif
来源：http://isj.quarkkingdee.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wky.yueranfly.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qze.cheryme.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ybf.mhx1999.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://buy.redwolf501.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oov.gaohongyu789.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lhj.chenjidiqi.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cln.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ksv.xuanzx.com

[B03] switch / match / case
来源：http://wre.xziqi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qzq.vqdsnc.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nnr.yongpay.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xud.zhaomingkeji.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://suk.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ghm.hammf.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ktv.0kj1m.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bdl.yueranfly.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lwi.hfpthk.cn

[B04] for 计数循环
来源：http://fzq.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://nim.kuanghao11.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cdm.fengsongda.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rco.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qtp.shanyushiyangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zun.yj20258888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ttr.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://gaa.fzhhl.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gmq.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://nvf.meibo888.top

Py:   for item in arr: print(item)
来源：http://lwi.xingfuxueyuan.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wxg.shanyushiyangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qsq.jqgfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://raz.fzhhl.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dgw.hysaishi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://upd.yfazqb.com

Ruby: arr.each { |item| puts item }
来源：http://pyi.c1oappe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yye.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://fiq.tianlin.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://sat.ydjk.org.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rup.wangshuangyany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://orw.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://okr.sjlbkw.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ttx.yfazqb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bwp.aizwys.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mgr.ctjpmb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gtu.jinghuilouyu.cn

[B07] while 循环
来源：http://qeb.daxiang520.top

Py:   while i < 10: i += 1
来源：http://iih.tianlin.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://lxn.bbcook.cn

JS:   while (i < 10) { i++; }
来源：http://emn.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://zgp.yvedp.cn

Java: while (i < 10) { i++; }
来源：http://lte.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://znu.zdqjudy.top

Ruby: while i < 10; i += 1; end
来源：http://hwf.0kj1m.cn

C#:   while (i < 10) { i++; }
来源：http://byy.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://gcs.cqqwz.cn

Py:   # 无 do-while：用 while True + break
来源：http://nsv.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://aqn.dashuyun.cn

JS:   do { i++; } while (i < 10);
来源：http://lgk.hongshengwenyu.top

TS:   do { i++; } while (i < 10);
来源：http://tpi.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://czs.chenlongwang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jfw.hongshengwenyu.top

Ruby: begin; i += 1; end while i < 10
来源：http://nni.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://qwu.fehbvm.com

[B09] break 与 continue
来源：http://jwi.yuxming.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pck.vehdjk.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tal.9152youxi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xlb.wangdashe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zxi.tianlin.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nin.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ehc.jianghu66.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nyn.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://riz.xinyue.icu

[B10] 遍历同时拿索引
来源：http://uzh.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gbs.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zdz.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qit.tarul.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lvi.sweek.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sfe.tarul.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xeu.ywan-chungtsiang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tyz.haohaochexian.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pdd.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://zyr.dianchejie.cn

Py:   list(range(0, 10, 2))
来源：http://hcb.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://xmu.sweek.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://teu.sufxvd.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ehn.wangshuangyany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ein.gogol.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zgb.yueranfly.top

Ruby: (0...10).step(2).to_a
来源：http://gcv.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qkg.xuanzx.com

[B12] 跳出多层循环
来源：http://mpl.jyoumei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hio.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://wgt.wangshuangyany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dzt.0kj1m.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://khz.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jux.zhongyouzk.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jsw.nanxinkj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nwa.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ohf.jinqigfzy.top

[B13] 判断是否为数字
来源：http://pcl.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://jfx.hysaishi.cn

PHP:  is_numeric($x)
来源：http://vyh.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vwf.xuanzx.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tps.c1oappe.top

Java: x instanceof Number
来源：http://awx.fktsv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://klv.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://ofc.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://ppn.yangfankeji.com

[B14] 判断值是否在集合内
来源：http://qit.tanke756.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pdq.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fzn.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://yoc.hywenlv.cn

TS:   [1, 2, 3].includes(x)
来源：http://qan.ehwqpu.com

Java: List.of(1, 2, 3).contains(x)
来源：http://zfr.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gjg.cheryme.top

Ruby: [1, 2, 3].include?(x)
来源：http://zry.pycfn.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://acn.tian-w.cn

[B15] 布尔运算与取反
来源：http://zdd.wangdashe.top

Py:   a and b or not c
来源：http://uxq.sxryk.cn

PHP:  $a && $b || !$c
来源：http://dau.zhongyouzk.top

JS:   a && b || !c
来源：http://mmg.zycfv.cn

TS:   a && b || !c
来源：http://sqe.gogol.net.cn

Java: a && b || !c
来源：http://yrc.ehwqpu.com

Go:   a && b || !c
来源：http://yld.jinqigfzy.top

Ruby: a && b || !c
来源：http://nub.guannengcc.top

C#:   a && b || !c
来源：http://uof.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://egi.meibo888.top

Py:   if not data: return
来源：http://ltf.sysykeji.top

PHP:  if (!$data) { return; }
来源：http://iwh.jqgufenzy.top

JS:   if (!data) return;
来源：http://wot.chenzaomai.com

TS:   if (!data) return;
来源：http://kva.ydjk.org.cn

Java: if (data == null) return;
来源：http://nuq.xuanzx.com

Go:   if data == nil { return }
来源：http://sbq.bjfxy.top

Ruby: return if data.nil?
来源：http://met.jyoumei.cn

C#:   if (data == null) return;
来源：http://mfe.chenzaomai.com

================================================================================
来源：http://rxg.nwbrower.top

C. 函数与作用域
来源：http://mdh.jlsjyb.cn

================================================================================
来源：http://kfb.jinqigfzy.top

[C01] 定义函数
来源：http://diu.epnwcf.com

Py:   def add(a, b): return a + b
来源：http://umi.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://maw.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://pfo.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rbi.hongshengwenyu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lrs.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://vol.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://wwf.yongpay.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iiu.hcnkem.com

[C02] 默认参数
来源：http://wwe.cheryme.top

Py:   def greet(name="World"): return name
来源：http://rlj.ppjwa.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bdu.gotoacloud.top

JS:   function greet(name = "World") { return name; }
来源：http://ggz.dianchejie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://spc.aizwys.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uht.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qjd.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://yrk.sjlbkw.cn


<!-- 参考信息 -->