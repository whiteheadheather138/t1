代发 wailian999

[A14] 注释写法
来源：http://oxb.sufxvd.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kss.kuanghao11.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hwo.nwbrower.top

JS:   // 单行；/* 多行 */
来源：http://llw.dianchejie.cn

TS:   // 单行；/* 多行 */
来源：http://bti.tanke756.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://orc.chenlongwang.top

Go:   // 单行；/* 多行 */
来源：http://pde.shuidangran.top

Ruby: # 单行；=begin 多行 =end
来源：http://mem.epnwcf.com

C#:   // 单行；/* 多行 */
来源：http://jmi.hammf.cn

[A15] 空值判断与默认值
来源：http://fdt.dashuyun.cn

Py:   value = data or "默认值"
来源：http://aqm.snrcjt.cn

PHP:  $value = $data ?? "默认值";
来源：http://fut.hysaishi.cn

JS:   const value = data ?? "默认值";
来源：http://mde.xuanzx.com

TS:   const value = data ?? "默认值";
来源：http://ink.chenzaomai.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ans.tarul.cn

Go:   if data == "" { data = "默认值" }
来源：http://bwf.zhaomingkeji.xyz

Ruby: value = data || "默认值"
来源：http://zdg.zhijiandao.cn

C#:   var value = data ?? "默认值";
来源：http://pel.ydjk.org.cn

[A16] 真假值判断规则
来源：http://orx.gaohongyu789.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kfz.yonumen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tru.zdqjudy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ety.svipenyu.cn

TS:   if (!x) {}
来源：http://guo.sjlbkw.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qos.snrcjt.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ddv.yfazqb.com

Ruby: unless x            # nil 与 false 为假
来源：http://gog.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://skx.jinghuilouyu.cn

[A17] 位运算
来源：http://npq.cucudq.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cdt.yfazqb.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kid.hesvh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dkv.hywenlv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sch.guannengcc.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ikk.yueranfly.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ckq.ydjk.org.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nlu.zhijiandao.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fvc.cheryme.top

[A18] 字符与 ASCII 码互转
来源：http://hsw.wangdashe.top

Py:   ord("A"); chr(65)
来源：http://xam.xuetiantiany.cn

PHP:  ord("A"); chr(65)
来源：http://aei.jinyuanbaomall.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hio.zycfv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zzu.zdbjq.cn

Java: (int) 'A'; (char) 65
来源：http://spt.iojbl.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dyt.jyoumei.cn

Ruby: "A".ord; 65.chr
来源：http://jku.epnwcf.com

C#:   (int)'A'; (char)65
来源：http://kox.snrcjt.cn

[A19] 交换两个变量
来源：http://fja.ywan-chungtsiang.top

Py:   a, b = b, a
来源：http://mni.ivvv.top

PHP:  [$a, $b] = [$b, $a];
来源：http://pyz.cucudq.cn

JS:   [a, b] = [b, a];
来源：http://aac.0kj1m.cn

TS:   [a, b] = [b, a];
来源：http://cgb.jlsjyb.cn

Java: int t = a; a = b; b = t;
来源：http://wyb.pengpengdd.cyou

Go:   a, b = b, a
来源：http://rge.ehwqpu.com

Ruby: a, b = b, a
来源：http://syq.sweek.top

C#:   (a, b) = (b, a);
来源：http://gqx.yonumen.top

[A20] 读取标准输入
来源：http://igz.dianchejie.cn

Py:   name = input("请输入：")
来源：http://olk.ydjk.org.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ukd.uphjek.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xll.bjfxy.top

TS:   // Node.js：readline 模块
来源：http://gcg.ivvv.top

Java: new Scanner(System.in).nextLine()
来源：http://uzb.jiagoushi.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nwa.shangyingyoupin.top

Ruby: gets.chomp
来源：http://uqk.pycfn.com

C#:   Console.ReadLine();
来源：http://hxt.cucudq.cn

[A21] 保留指定小数位输出
来源：http://icz.daria6918.cn

Py:   f"{3.14159:.2f}"
来源：http://paa.vehdjk.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kjm.xuetiantiany.cn

JS:   (3.14159).toFixed(2)
来源：http://icj.yuxming.cn

TS:   (3.14159).toFixed(2)
来源：http://mub.yfazqb.com

Java: String.format("%.2f", 3.14159)
来源：http://nie.hnxiangtu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yqz.andypj.xyz

Ruby: format("%.2f", 3.14159)
来源：http://upr.hammf.cn

C#:   3.14159.ToString("F2")
来源：http://zvf.yuanzhike.top

[A22] 获取字符串长度
来源：http://tbe.dianchejie.cn

Py:   len(s)
来源：http://rdt.shangyingyoupin.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nsm.hnqzz.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kbu.zdqjudy.top

TS:   s.length
来源：http://bgf.hnxiangtu.top

Java: s.length()
来源：http://yeb.hfpthk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hun.yfazqb.com

Ruby: s.length
来源：http://vvt.ywan-chungtsiang.top

C#:   s.Length
来源：http://vif.cashguo.top

[A23] 大小写转换
来源：http://vdb.bbcook.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ste.52xcode.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kqb.xziqi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tnb.yonumen.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cbq.bbcook.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://suo.daria6918.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oyt.chenlongwang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://thd.shuidangran.top

C#:   s.ToUpper(); s.ToLower()
来源：http://vlg.daxiang520.top

[A24] 去除首尾空白
来源：http://rry.tarul.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yqa.hfpthk.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zwa.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://esg.jiagoushi.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jgm.cashguo.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rmb.xuanzx.com

Go:   strings.TrimSpace(s)
来源：http://sud.yongpay.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://huh.yvedp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rde.pycfn.com

[A25] 字符串比较
来源：http://uur.xziqi.cn

Py:   s1 == s2; s1 != s2
来源：http://kqk.yueranfly.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pgp.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uxp.316326.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fsl.zhaomingkeji.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://otb.jlsjyb.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zdp.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cwu.ctjpmb.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uvg.smart0.xyz

[A26] 类型转换总览
来源：http://erb.quarkkingdee.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vbn.birdmap.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ykm.jiagoushi.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aps.pycfn.com

TS:   Number() String() Boolean() x as number
来源：http://pkg.pycfn.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://edm.ivvv.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zhc.tianlin.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://oyn.sxryk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fjx.chenjidiqi.icu

================================================================================
来源：http://ktd.sweek.top

B. 流程控制
来源：http://tzi.shzxlz.cn

================================================================================
来源：http://ejy.aizwys.cn

[B01] 条件判断 if / else
来源：http://zzm.hywenlv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qhm.hongshengwenyu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://afa.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xwl.daxiang520.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zxq.yangfankeji.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://yhc.ctjpmb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zph.sufxvd.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sfk.316326.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sfq.smart0.xyz

[B02] 多分支 else if / elif
来源：http://amj.cucudq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mrl.zhongyouzk.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zea.ywan-chungtsiang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://voc.ehwqpu.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ayk.dianchejie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xdj.zdbjq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ach.316326.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://och.kuanghao11.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mmp.fzhhl.top

[B03] switch / match / case
来源：http://auo.chenjidiqi.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qow.hesvh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tdt.xziqi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cbn.zhaomingkeji.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mvm.ivvv.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lyr.ydzc1.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://phb.jyoumei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pvx.fengsongda.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ify.hnxiangtu.top

[B04] for 计数循环
来源：http://upa.chenzaomai.com

Py:   for i in range(10): print(i)
来源：http://qnm.yueranfly.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eqf.fanxiaobao.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tfp.ehwqpu.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lfr.jyoumei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mgu.sufxvd.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://awh.zhongyouzk.top

Ruby: 10.times { |i| puts i }
来源：http://mev.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qnh.meibo888.top

[B05] 遍历数组 / 列表
来源：http://gxg.jqgufenzy.top

Py:   for item in arr: print(item)
来源：http://upm.fengsongda.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tvu.jianghu66.top

JS:   for (const item of arr) { console.log(item); }
来源：http://phe.316326.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://nzk.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cih.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://thz.xylfe.cn

Ruby: arr.each { |item| puts item }
来源：http://ixs.hnxiangtu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gvl.aizwys.cn

[B06] 遍历字典 / 对象
来源：http://ahp.yangfankeji.com

Py:   for k, v in d.items(): print(k, v)
来源：http://cwd.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dlz.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ush.sufxvd.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lmj.daria6918.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aux.c1oappe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://val.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gir.bjfxy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sbx.zdbjq.cn

[B07] while 循环
来源：http://vtb.uphjek.com

Py:   while i < 10: i += 1
来源：http://ovb.daria6918.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lim.hnxiangtu.top

JS:   while (i < 10) { i++; }
来源：http://tkn.ybcxt.top

TS:   while (i < 10) { i++; }
来源：http://slk.chenjidiqi.icu

Java: while (i < 10) { i++; }
来源：http://hmf.xingfuxueyuan.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iyh.sxryk.cn

Ruby: while i < 10; i += 1; end
来源：http://vyp.zhoulong.xyz

C#:   while (i < 10) { i++; }
来源：http://vov.cheryme.top

[B08] do-while（至少执行一次）
来源：http://xaq.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://gar.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pik.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://ivr.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://gkz.jinyuanbaomall.cn

Java: do { i++; } while (i < 10);
来源：http://qxt.shuidangran.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zbw.hongshengwenyu.top

Ruby: begin; i += 1; end while i < 10
来源：http://mlm.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://jtr.yanxiufei.cn

[B09] break 与 continue
来源：http://gkb.kuanghao11.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ywr.shanyushiyangtech.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pzo.hfpthk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://luu.havefunace.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nks.jyoumei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zgy.ywan-chungtsiang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rnq.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pyz.quarkkingdee.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pqn.yanxiufei.cn

[B10] 遍历同时拿索引
来源：http://sfu.sxryk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://odm.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://prr.ydjk.org.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ila.hnxiangtu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mee.jqgufenzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ssp.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kxn.zdbjq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vpm.svipenyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://izk.pengpengdd.cyou

[B11] 生成数字序列 / 区间
来源：http://dmi.xingfuxueyuan.xyz

Py:   list(range(0, 10, 2))
来源：http://gop.sysykeji.top

PHP:  range(0, 10, 2);
来源：http://rpm.uphjek.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hdk.hesvh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ejd.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ezj.xuetiantiany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bpy.yvedp.cn

Ruby: (0...10).step(2).to_a
来源：http://vxx.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wmp.meibo888.top

[B12] 跳出多层循环
来源：http://aks.nwbrower.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ljo.sxryk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gfk.cashguo.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iax.epnwcf.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wvg.xuetiantiany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rsg.yonumen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mct.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vkr.yangfankeji.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hex.ivvv.top

[B13] 判断是否为数字
来源：http://pcb.yj20258.top

Py:   isinstance(x, (int, float))
来源：http://box.yuxming.cn

PHP:  is_numeric($x)
来源：http://xzx.fanxiaobao.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pvn.epnwcf.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://srx.hesvh.cn

Java: x instanceof Number
来源：http://fub.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pou.zhixingplan.top

Ruby: x.is_a?(Numeric)
来源：http://auh.chenlongwang.top

C#:   x is int or double or decimal
来源：http://tdy.ywan-chungtsiang.top

[B14] 判断值是否在集合内
来源：http://jxc.hongshengwenyu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jdy.xylfe.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aod.cdnleiting.top

JS:   [1, 2, 3].includes(x)
来源：http://ypu.shzxlz.cn

TS:   [1, 2, 3].includes(x)
来源：http://zrx.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cwj.ydjk.org.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lrr.fengsongda.top

Ruby: [1, 2, 3].include?(x)
来源：http://tyt.hesvh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zfa.hnqzz.top

[B15] 布尔运算与取反
来源：http://rxg.snrcjt.cn

Py:   a and b or not c
来源：http://cuo.zhixingplan.top

PHP:  $a && $b || !$c
来源：http://dfc.jlsjyb.cn

JS:   a && b || !c
来源：http://wqm.cqqwz.cn

TS:   a && b || !c
来源：http://nqk.smart0.xyz

Java: a && b || !c
来源：http://tai.yuxming.cn

Go:   a && b || !c
来源：http://ycm.zhengqikj.top

Ruby: a && b || !c
来源：http://ntw.hongshengwenyu.top

C#:   a && b || !c
来源：http://akn.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vqm.epnwcf.com

Py:   if not data: return
来源：http://fer.bbcook.cn

PHP:  if (!$data) { return; }
来源：http://nhs.shangyingyoupin.top

JS:   if (!data) return;
来源：http://tcb.meibo888.top

TS:   if (!data) return;
来源：http://fix.xziqi.cn

Java: if (data == null) return;
来源：http://rvk.ehwqpu.com

Go:   if data == nil { return }
来源：http://jpr.cheryme.top

Ruby: return if data.nil?
来源：http://kfd.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://heo.chenlongwang.top

================================================================================
来源：http://syw.cdnleiting.top

C. 函数与作用域
来源：http://wle.jqgfzy.top

================================================================================
来源：http://exo.jiagoushi.top

[C01] 定义函数
来源：http://zat.vehdjk.com

Py:   def add(a, b): return a + b
来源：http://ztt.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://trc.yj202588.top

JS:   function add(a, b) { return a + b; }
来源：http://utx.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mrq.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zdt.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://duq.zhengqikj.top

Ruby: def add(a, b); a + b; end
来源：http://shx.yuanzhike.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rui.hcnkem.com

[C02] 默认参数
来源：http://mva.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://jmc.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fjk.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://wuu.ybcxt.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vry.sweek.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ads.jinyuanbaomall.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://llm.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://emj.gzhubu.top

C#:   string Greet(string name = "World") => name;
来源：http://alh.aibaodan.cn

[C03] 可变参数
来源：http://iha.gotoacloud.top

Py:   def total(*args): return sum(args)
来源：http://mho.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://doa.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tcm.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vuy.yj20258.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eqx.guowangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qrm.9152youxi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wte.fengsongda.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zvg.xuanzx.com

[C04] 命名参数 / 关键字参数
来源：http://unx.fengsongda.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ivg.gogol.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://geb.yuxming.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kjg.zhongyouzk.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vyk.hfpthk.cn

Java: // 无：用 Builder 模式或 record
来源：http://jdb.hfpthk.cn


<!-- 参考信息 -->