代发 wailian999

[A14] 注释写法
来源：http://lbd.yangfankeji.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://dta.yueranfly.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://rjd.yongpay.top

JS:   // 单行；/* 多行 */
来源：http://xnr.tianlin.xyz

TS:   // 单行；/* 多行 */
来源：http://hyb.daria6918.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dcd.xylfe.cn

Go:   // 单行；/* 多行 */
来源：http://qau.jqgfzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://jjs.vqdsnc.cn

C#:   // 单行；/* 多行 */
来源：http://ory.yvedp.cn

[A15] 空值判断与默认值
来源：http://wxu.zhiwuduotai.top

Py:   value = data or "默认值"
来源：http://aca.sweek.top

PHP:  $value = $data ?? "默认值";
来源：http://pvb.sxryk.cn

JS:   const value = data ?? "默认值";
来源：http://nvb.316326.xyz

TS:   const value = data ?? "默认值";
来源：http://uxe.chenlongwang.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oyo.hesvh.cn

Go:   if data == "" { data = "默认值" }
来源：http://rgl.ctjpmb.com

Ruby: value = data || "默认值"
来源：http://sms.fengsongda.top

C#:   var value = data ?? "默认值";
来源：http://nca.c1oappe.top

[A16] 真假值判断规则
来源：http://ztx.quarkkingdee.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mds.jinghuilouyu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wln.yonumen.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xrd.hysaishi.cn

TS:   if (!x) {}
来源：http://jbi.andypj.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mvq.tanke756.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://szo.hnxiangtu.top

Ruby: unless x            # nil 与 false 为假
来源：http://trq.smart0.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://znf.sxryk.cn

[A17] 位运算
来源：http://xpx.cheryme.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mro.sxryk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mqs.svipenyu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ggb.nanxinkj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://quz.nwbrower.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fvq.redwolf501.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wvd.xinyue.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fck.zhengqikj.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://utv.xuanzx.com

[A18] 字符与 ASCII 码互转
来源：http://ovy.haohaochexian.top

Py:   ord("A"); chr(65)
来源：http://efq.jiagoushi.top

PHP:  ord("A"); chr(65)
来源：http://ucg.cdnleiting.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aeq.nanxinkj.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://inv.nanxinkj.top

Java: (int) 'A'; (char) 65
来源：http://nrl.zdbjq.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zfy.shzxlz.cn

Ruby: "A".ord; 65.chr
来源：http://yyc.yueranfly.top

C#:   (int)'A'; (char)65
来源：http://quk.sxryk.cn

[A19] 交换两个变量
来源：http://utw.havefunace.top

Py:   a, b = b, a
来源：http://ovb.cheryme.top

PHP:  [$a, $b] = [$b, $a];
来源：http://req.cdnleiting.top

JS:   [a, b] = [b, a];
来源：http://wsv.haohaochexian.top

TS:   [a, b] = [b, a];
来源：http://pzm.zhaomingkeji.xyz

Java: int t = a; a = b; b = t;
来源：http://bha.zhiwuduotai.top

Go:   a, b = b, a
来源：http://sof.daria6918.cn

Ruby: a, b = b, a
来源：http://szh.jyoumei.cn

C#:   (a, b) = (b, a);
来源：http://wky.shuidangran.top

[A20] 读取标准输入
来源：http://aai.tian-w.cn

Py:   name = input("请输入：")
来源：http://kxe.hesvh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://idf.gogol.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ekp.shanyushiyangtech.top

TS:   // Node.js：readline 模块
来源：http://vhx.zdqjudy.top

Java: new Scanner(System.in).nextLine()
来源：http://dmr.yuxming.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://aww.ctjpmb.com

Ruby: gets.chomp
来源：http://wwp.jinyuanbaomall.cn

C#:   Console.ReadLine();
来源：http://csg.yuanzhike.top

[A21] 保留指定小数位输出
来源：http://yyp.yanxiufei.cn

Py:   f"{3.14159:.2f}"
来源：http://gza.yfazqb.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cnx.daria6918.cn

JS:   (3.14159).toFixed(2)
来源：http://pux.ywan-chungtsiang.top

TS:   (3.14159).toFixed(2)
来源：http://zhj.sweek.top

Java: String.format("%.2f", 3.14159)
来源：http://diw.jiagoushi.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mdg.xuanzx.com

Ruby: format("%.2f", 3.14159)
来源：http://uwg.fktsv.cn

C#:   3.14159.ToString("F2")
来源：http://ygn.yueranfly.top

[A22] 获取字符串长度
来源：http://ghc.ctjpmb.com

Py:   len(s)
来源：http://pse.sysykeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cht.dashuyun.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://txd.hcnkem.com

TS:   s.length
来源：http://cgw.aizwys.cn

Java: s.length()
来源：http://dgn.ywan-chungtsiang.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rxa.c1oappe.top

Ruby: s.length
来源：http://awb.feifeiyinyue.top

C#:   s.Length
来源：http://jxt.fanxiaobao.xyz

[A23] 大小写转换
来源：http://pit.bjfxy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://npk.xinyue.icu

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qip.jiagoushi.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gvf.316326.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://duv.chenzaomai.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bpd.svipenyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rel.hongshengwenyu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mvk.zhoulong.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://gmx.zdqjudy.top

[A24] 去除首尾空白
来源：http://pxo.chenzaomai.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://czi.daxiang520.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yaw.aizwys.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vnm.jqgfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wes.guannengcc.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bdy.dianchejie.cn

Go:   strings.TrimSpace(s)
来源：http://dmy.wangshuangyany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qyk.sxryk.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xpq.ppjwa.cn

[A25] 字符串比较
来源：http://zvw.shzxlz.cn

Py:   s1 == s2; s1 != s2
来源：http://klk.wangshuangyany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cic.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cbi.yuanzhike.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tad.c1oappe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sgb.daxiang520.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lxi.gaohongyu789.top

Ruby: s1 == s2; s1 <=> s2
来源：http://izq.yuanzhike.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mkn.jianghu66.top

[A26] 类型转换总览
来源：http://gtf.fanxiaobao.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rta.yongpay.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cvk.quarkkingdee.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ezx.bbcook.cn

TS:   Number() String() Boolean() x as number
来源：http://dpu.gaohongyu789.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oew.ppjwa.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://igm.gotoacloud.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xwu.jinyuanbaomall.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xno.haohaochexian.top

================================================================================
来源：http://ngi.feifeiyinyue.top

B. 流程控制
来源：http://fvy.yuxming.cn

================================================================================
来源：http://byh.zhixingplan.top

[B01] 条件判断 if / else
来源：http://syz.jianghu66.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tad.daria6918.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://par.tianlin.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fis.cheryme.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://evz.kuanghao11.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vfa.shanyushiyangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zhk.xinyue.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qer.zhoulong.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sdq.tanke756.top

[B02] 多分支 else if / elif
来源：http://xcc.zdbjq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://brw.hcnkem.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qgh.fengsongda.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aja.wangshuangyany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ygv.yueranfly.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fgy.c1oappe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pcd.yonumen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ovt.epnwcf.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kuh.bbcook.cn

[B03] switch / match / case
来源：http://xyu.vehdjk.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hco.dashuyun.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zen.ctjpmb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sgq.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://olu.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hpx.guannengcc.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jfv.zhengqikj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://war.dashuyun.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wfx.yuxming.cn

[B04] for 计数循环
来源：http://evx.wangdashe.top

Py:   for i in range(10): print(i)
来源：http://lvg.shanyushiyangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yvq.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pgg.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nby.ydzc1.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fzw.chenjidiqi.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://phi.fengsongda.top

Ruby: 10.times { |i| puts i }
来源：http://rpr.kuanghao11.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ggl.cqqwz.cn

[B05] 遍历数组 / 列表
来源：http://neb.c1oappe.top

Py:   for item in arr: print(item)
来源：http://shz.vehdjk.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gel.aizwys.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wlf.xingfuxueyuan.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://jdo.jianghu66.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xtd.sjlbkw.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uox.hnxiangtu.top

Ruby: arr.each { |item| puts item }
来源：http://mkf.gaohongyu789.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bib.c1oappe.top

[B06] 遍历字典 / 对象
来源：http://ghh.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dua.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fut.jinqigfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://axp.shzxlz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ans.jinyuanbaomall.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kvp.jinqigfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://csq.9152youxi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lfw.meibo888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://spa.uphjek.com

[B07] while 循环
来源：http://anm.chenzaomai.com

Py:   while i < 10: i += 1
来源：http://vsr.zycfv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://syd.yfazqb.com

JS:   while (i < 10) { i++; }
来源：http://xhr.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://jbg.zhijiandao.cn

Java: while (i < 10) { i++; }
来源：http://xoq.andypj.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wic.jinqigufen.top

Ruby: while i < 10; i += 1; end
来源：http://tmx.hammf.cn

C#:   while (i < 10) { i++; }
来源：http://lwu.316326.xyz

[B08] do-while（至少执行一次）
来源：http://sjt.zhoulong.xyz

Py:   # 无 do-while：用 while True + break
来源：http://duw.nwbrower.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hgy.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://ynr.zhiwuduotai.top

TS:   do { i++; } while (i < 10);
来源：http://iep.ctjpmb.com

Java: do { i++; } while (i < 10);
来源：http://grn.sufxvd.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ugh.xuetiantiany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oeq.xuanzx.com

C#:   do { i++; } while (i < 10);
来源：http://tph.fanxiaobao.xyz

[B09] break 与 continue
来源：http://fxq.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nbx.tarul.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yuz.zdqjudy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iyk.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uvl.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eiv.aizwys.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ido.c1oappe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jpk.yanxiufei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rnz.fanxiaobao.xyz

[B10] 遍历同时拿索引
来源：http://ycs.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zsd.jinqigufen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://see.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://acu.vehdjk.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wgz.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dwe.haohaochexian.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uff.hysaishi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aov.bbcook.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kch.redwolf501.top

[B11] 生成数字序列 / 区间
来源：http://iro.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://mgm.zhoulong.xyz

PHP:  range(0, 10, 2);
来源：http://gwo.tarul.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uta.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://leg.snrcjt.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cwa.jqgfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dqg.epnwcf.com

Ruby: (0...10).step(2).to_a
来源：http://wpz.cqqwz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uko.316326.xyz

[B12] 跳出多层循环
来源：http://nhh.snrcjt.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yjw.gogol.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://doq.yuanzhike.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hlo.hammf.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jpb.redwolf501.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fbr.hfpthk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bqf.hysaishi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sir.zhiwuduotai.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vhq.xinyue.icu

[B13] 判断是否为数字
来源：http://xuc.dashuyun.cn

Py:   isinstance(x, (int, float))
来源：http://sth.redwolf501.top

PHP:  is_numeric($x)
来源：http://kcj.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hnx.bjfxy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sks.jlsjyb.cn

Java: x instanceof Number
来源：http://jsc.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wbh.gotoacloud.top

Ruby: x.is_a?(Numeric)
来源：http://xrw.tian-w.cn

C#:   x is int or double or decimal
来源：http://wlb.c1oappe.top

[B14] 判断值是否在集合内
来源：http://ozy.pengpengdd.cyou

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tbp.andypj.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fzj.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://mkd.ppjwa.cn

TS:   [1, 2, 3].includes(x)
来源：http://mcl.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qdn.hcnkem.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qvo.zhijiandao.cn

Ruby: [1, 2, 3].include?(x)
来源：http://orr.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xjd.redwolf501.top

[B15] 布尔运算与取反
来源：http://wzz.hnxiangtu.top

Py:   a and b or not c
来源：http://hjc.chenjidiqi.icu

PHP:  $a && $b || !$c
来源：http://hyo.jlsjyb.cn

JS:   a && b || !c
来源：http://egm.hfpthk.cn

TS:   a && b || !c
来源：http://uxj.gogol.net.cn

Java: a && b || !c
来源：http://ucg.ehwqpu.com

Go:   a && b || !c
来源：http://bws.sjlbkw.cn

Ruby: a && b || !c
来源：http://ley.pengpengdd.cyou

C#:   a && b || !c
来源：http://ctc.sysykeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://mdj.xylfe.cn

Py:   if not data: return
来源：http://cvt.sysykeji.top

PHP:  if (!$data) { return; }
来源：http://kuc.zdqjudy.top

JS:   if (!data) return;
来源：http://pgg.sysykeji.top

TS:   if (!data) return;
来源：http://ycz.jinghuilouyu.cn

Java: if (data == null) return;
来源：http://bvg.hfpthk.cn

Go:   if data == nil { return }
来源：http://kac.sxryk.cn

Ruby: return if data.nil?
来源：http://mpl.tanke756.top

C#:   if (data == null) return;
来源：http://yts.pycfn.com

================================================================================
来源：http://joj.9152youxi.cn

C. 函数与作用域
来源：http://rai.fehbvm.com

================================================================================
来源：http://hfq.shangyingyoupin.top

[C01] 定义函数
来源：http://eix.0kj1m.cn

Py:   def add(a, b): return a + b
来源：http://plt.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dkz.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://ybi.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qbc.xinyue.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://jgr.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://ylr.c1oappe.top

Ruby: def add(a, b); a + b; end
来源：http://acr.uphjek.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jyb.nwbrower.top

[C02] 默认参数
来源：http://znf.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://wel.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jlv.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://yyc.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jtb.sweek.top

Java: // 无默认参数：方法重载或 Optional
来源：http://evc.feifeiyinyue.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ide.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://hpo.birdmap.top

C#:   string Greet(string name = "World") => name;
来源：http://mvm.zhongyouzk.top

[C03] 可变参数
来源：http://rok.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://xwr.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gwc.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pmx.zdbjq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nrn.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ruw.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rro.hywenlv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vuq.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://isj.jqgfzy.top

[C04] 命名参数 / 关键字参数
来源：http://aui.bjfxy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tfl.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jbp.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qwl.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yla.cheryme.top

Java: // 无：用 Builder 模式或 record
来源：http://fby.tarul.cn


<!-- 参考信息 -->