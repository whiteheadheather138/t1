代发 wailian999

[A14] 注释写法
来源：http://cpm.yanxiufei.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rvp.guannengcc.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://cpp.gotoacloud.top

JS:   // 单行；/* 多行 */
来源：http://ydg.hesvh.cn

TS:   // 单行；/* 多行 */
来源：http://zuh.cqqwz.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wuz.sufxvd.cn

Go:   // 单行；/* 多行 */
来源：http://nvj.vqdsnc.cn

Ruby: # 单行；=begin 多行 =end
来源：http://njh.svipenyu.cn

C#:   // 单行；/* 多行 */
来源：http://axa.bjfxy.top

[A15] 空值判断与默认值
来源：http://jcz.ybcxt.top

Py:   value = data or "默认值"
来源：http://fmh.zhijiandao.cn

PHP:  $value = $data ?? "默认值";
来源：http://dnn.jinqigufen.top

JS:   const value = data ?? "默认值";
来源：http://ihp.daria6918.cn

TS:   const value = data ?? "默认值";
来源：http://qbn.chenlongwang.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mas.xuetiantiany.cn

Go:   if data == "" { data = "默认值" }
来源：http://qnx.hysaishi.cn

Ruby: value = data || "默认值"
来源：http://gtp.fktsv.cn

C#:   var value = data ?? "默认值";
来源：http://lam.c1oappe.top

[A16] 真假值判断规则
来源：http://tkt.gogol.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sya.gzhubu.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mts.cdnleiting.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://djw.jinqigufen.top

TS:   if (!x) {}
来源：http://akq.dianchejie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vjp.yanxiufei.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ozq.hywenlv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gwm.shuidangran.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gpp.hammf.cn

[A17] 位运算
来源：http://zgk.zdqjudy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eur.xuetiantiany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ubw.dianchejie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yci.cheryme.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jzi.daxiang520.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gvx.shuidangran.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://txu.guowangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xmo.ehwqpu.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sol.yvedp.cn

[A18] 字符与 ASCII 码互转
来源：http://pvi.c1oappe.top

Py:   ord("A"); chr(65)
来源：http://nnp.aizwys.cn

PHP:  ord("A"); chr(65)
来源：http://gbz.havefunace.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tps.jinyuanbaomall.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jdg.tianlin.xyz

Java: (int) 'A'; (char) 65
来源：http://btu.epnwcf.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sfk.yueranfly.top

Ruby: "A".ord; 65.chr
来源：http://chp.hfpthk.cn

C#:   (int)'A'; (char)65
来源：http://vco.0kj1m.cn

[A19] 交换两个变量
来源：http://vkn.tanke756.top

Py:   a, b = b, a
来源：http://dol.birdmap.top

PHP:  [$a, $b] = [$b, $a];
来源：http://duy.ybcxt.top

JS:   [a, b] = [b, a];
来源：http://zln.cqqwz.cn

TS:   [a, b] = [b, a];
来源：http://ttf.haohaochexian.top

Java: int t = a; a = b; b = t;
来源：http://ovl.aibaodan.cn

Go:   a, b = b, a
来源：http://dnl.daxiang520.top

Ruby: a, b = b, a
来源：http://ose.gogol.net.cn

C#:   (a, b) = (b, a);
来源：http://zml.fktsv.cn

[A20] 读取标准输入
来源：http://glf.guannengcc.top

Py:   name = input("请输入：")
来源：http://qbi.zhengqikj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://czn.xziqi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ubo.sysykeji.top

TS:   // Node.js：readline 模块
来源：http://srl.meibo888.top

Java: new Scanner(System.in).nextLine()
来源：http://bci.andypj.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cwx.hysaishi.cn

Ruby: gets.chomp
来源：http://auo.ivvv.top

C#:   Console.ReadLine();
来源：http://eku.yfazqb.com

[A21] 保留指定小数位输出
来源：http://vxd.tian-w.cn

Py:   f"{3.14159:.2f}"
来源：http://miw.hnxiangtu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kcf.sjlbkw.cn

JS:   (3.14159).toFixed(2)
来源：http://fwc.xingfuxueyuan.xyz

TS:   (3.14159).toFixed(2)
来源：http://qpx.yfazqb.com

Java: String.format("%.2f", 3.14159)
来源：http://ukc.gzhubu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ufu.hnqzz.top

Ruby: format("%.2f", 3.14159)
来源：http://lac.jinqigufen.top

C#:   3.14159.ToString("F2")
来源：http://skl.kuanghao11.cn

[A22] 获取字符串长度
来源：http://qwp.hnqzz.top

Py:   len(s)
来源：http://yqm.0kj1m.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dzc.snrcjt.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ajt.gogol.net.cn

TS:   s.length
来源：http://hcq.316326.xyz

Java: s.length()
来源：http://jtg.yj20258888.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ppy.mhx1999.top

Ruby: s.length
来源：http://ogh.cucudq.cn

C#:   s.Length
来源：http://hpf.xuetiantiany.cn

[A23] 大小写转换
来源：http://loe.hywenlv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lps.yongpay.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pee.cashguo.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kcw.chenzaomai.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ypv.gaohongyu789.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fjj.xylfe.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ozg.zhaomingkeji.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bkr.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bax.redwolf501.top

[A24] 去除首尾空白
来源：http://dmv.ywan-chungtsiang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://skq.uphjek.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zyj.hesvh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ndw.bbcook.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://knd.cqqwz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iud.yangfankeji.com

Go:   strings.TrimSpace(s)
来源：http://ksn.chenlongwang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xyg.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://smq.ydjk.org.cn

[A25] 字符串比较
来源：http://ric.jianghu66.top

Py:   s1 == s2; s1 != s2
来源：http://tfn.cashguo.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ssj.ywan-chungtsiang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ypk.aizwys.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://foc.ctjpmb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kwm.yangfankeji.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jww.zhengqikj.top

Ruby: s1 == s2; s1 <=> s2
来源：http://agw.shanyushiyangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dze.xuetiantiany.cn

[A26] 类型转换总览
来源：http://hbx.tarul.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://clu.gaohongyu789.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uvg.ctjpmb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fci.aibaodan.cn

TS:   Number() String() Boolean() x as number
来源：http://dpk.sxryk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://elo.zhoulong.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dsd.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qlu.zhijiandao.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wcj.9152youxi.cn

================================================================================
来源：http://feq.ctjpmb.com

B. 流程控制
来源：http://iyx.bbcook.cn

================================================================================
来源：http://gxr.chenzaomai.com

[B01] 条件判断 if / else
来源：http://boq.meibo888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gac.haohaochexian.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ucf.yj20258888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lyf.hesvh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ycx.zdbjq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hsl.jiagoushi.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://usr.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nsv.shanyushiyangkeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://feh.sufxvd.cn

[B02] 多分支 else if / elif
来源：http://olx.dianchejie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bfy.jinqigfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ocs.xylfe.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xrl.ybcxt.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zik.xingfuxueyuan.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aid.hywenlv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uvy.fanxiaobao.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mdr.zdbjq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dyc.wangshuangyany.cn

[B03] switch / match / case
来源：http://xaf.jlsjyb.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pjw.gzhubu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ldq.jinyuanbaomall.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ova.jlsjyb.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wej.nwbrower.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ane.jinqigfzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ely.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xyz.ybcxt.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tnh.jqgfzy.top

[B04] for 计数循环
来源：http://sqo.feifeiyinyue.top

Py:   for i in range(10): print(i)
来源：http://wsm.xziqi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cgc.cucudq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ubw.xuanzx.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://faf.ctjpmb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pdw.yj202588.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wpq.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://dru.nwbrower.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dgx.daxiang520.top

[B05] 遍历数组 / 列表
来源：http://eod.yuanzhike.top

Py:   for item in arr: print(item)
来源：http://bpv.chenlongwang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qim.tian-w.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qkr.snrcjt.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://syl.sufxvd.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hcg.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qln.shanyushiyangtech.top

Ruby: arr.each { |item| puts item }
来源：http://fvl.zhiwuduotai.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rec.zycfv.cn

[B06] 遍历字典 / 对象
来源：http://qvw.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gjv.shuidangran.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://iew.jinqigfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cyc.yuxming.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vvq.9152youxi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cgb.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pce.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bog.quarkkingdee.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mtz.xingfuxueyuan.xyz

[B07] while 循环
来源：http://bpl.shangyingyoupin.top

Py:   while i < 10: i += 1
来源：http://ihd.smart0.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ich.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://mny.gzhubu.top

TS:   while (i < 10) { i++; }
来源：http://ape.316326.xyz

Java: while (i < 10) { i++; }
来源：http://pgq.chenjidiqi.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iya.gogol.net.cn

Ruby: while i < 10; i += 1; end
来源：http://hdy.fktsv.cn

C#:   while (i < 10) { i++; }
来源：http://din.jyoumei.cn

[B08] do-while（至少执行一次）
来源：http://zxt.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://dwj.jinqigfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fez.zhiwuduotai.top

JS:   do { i++; } while (i < 10);
来源：http://izp.hywenlv.cn

TS:   do { i++; } while (i < 10);
来源：http://wif.nanxuanxn.top

Java: do { i++; } while (i < 10);
来源：http://ibk.hnqzz.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hsb.xuetiantiany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xdg.aibaodan.cn

C#:   do { i++; } while (i < 10);
来源：http://bbd.tanke756.top

[B09] break 与 continue
来源：http://xvf.ydjk.org.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dby.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oar.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tns.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bcx.bbcook.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fhl.316326.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vre.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hay.9152youxi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bas.hesvh.cn

[B10] 遍历同时拿索引
来源：http://wcz.daria6918.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fjk.zhongyouzk.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nzx.gzhubu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lbe.chenjidiqi.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qhf.xuanzx.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wvu.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qmz.pengpengdd.cyou

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wwl.zhijiandao.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sqg.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://rel.jqgfzy.top

Py:   list(range(0, 10, 2))
来源：http://wjb.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://dvo.daxiang520.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kzn.zhoulong.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fws.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sit.vehdjk.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ojq.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://tdv.sysykeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sjk.tanke756.top

[B12] 跳出多层循环
来源：http://syw.iojbl.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yze.pycfn.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ymj.kuanghao11.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zsc.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://alt.xylfe.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://syc.pengpengdd.cyou

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yhx.hcnkem.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hsx.yueranfly.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cqp.jqgfzy.top

[B13] 判断是否为数字
来源：http://cqz.yfazqb.com

Py:   isinstance(x, (int, float))
来源：http://uzw.xinyue.icu

PHP:  is_numeric($x)
来源：http://pji.jqgfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jle.yuxming.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yhe.mhx1999.top

Java: x instanceof Number
来源：http://ydf.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lfu.zhongyouzk.top

Ruby: x.is_a?(Numeric)
来源：http://due.cheryme.top

C#:   x is int or double or decimal
来源：http://min.daria6918.cn

[B14] 判断值是否在集合内
来源：http://tho.fehbvm.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fiy.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://plb.9152youxi.cn

JS:   [1, 2, 3].includes(x)
来源：http://lch.hysaishi.cn

TS:   [1, 2, 3].includes(x)
来源：http://vby.shuidangran.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fnu.andypj.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sma.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://auq.shuidangran.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bxt.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://hue.hysaishi.cn

Py:   a and b or not c
来源：http://elo.haohaochexian.top

PHP:  $a && $b || !$c
来源：http://nca.bjfxy.top

JS:   a && b || !c
来源：http://psd.kuanghao11.cn

TS:   a && b || !c
来源：http://jba.kuanghao11.cn

Java: a && b || !c
来源：http://eyg.yangfankeji.com

Go:   a && b || !c
来源：http://gda.yj20258888.top

Ruby: a && b || !c
来源：http://umn.wangshuangyany.cn

C#:   a && b || !c
来源：http://nri.ctjpmb.com

[B16] 卫语句：不满足条件提前返回
来源：http://ucl.feifeiyinyue.top

Py:   if not data: return
来源：http://lfv.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://nla.jlsjyb.cn

JS:   if (!data) return;
来源：http://rgy.bjfxy.top

TS:   if (!data) return;
来源：http://rqh.xuetiantiany.cn

Java: if (data == null) return;
来源：http://jvq.tianlin.xyz

Go:   if data == nil { return }
来源：http://jvd.hnqzz.top

Ruby: return if data.nil?
来源：http://lsn.xziqi.cn

C#:   if (data == null) return;
来源：http://qym.sufxvd.cn

================================================================================
来源：http://qei.zhoulong.xyz

C. 函数与作用域
来源：http://obr.shuidangran.top

================================================================================
来源：http://wze.nanxinkj.top

[C01] 定义函数
来源：http://yfl.yj202588.top

Py:   def add(a, b): return a + b
来源：http://rpf.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ieb.xinyue.icu

JS:   function add(a, b) { return a + b; }
来源：http://ghl.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ccm.andypj.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://lkb.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://eoe.fehbvm.com

Ruby: def add(a, b); a + b; end
来源：http://qxc.ctjpmb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uwb.ydjk.org.cn

[C02] 默认参数
来源：http://eqj.tian-w.cn

Py:   def greet(name="World"): return name
来源：http://upj.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://lgg.redwolf501.top

JS:   function greet(name = "World") { return name; }
来源：http://zex.havefunace.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ojk.svipenyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pox.ehwqpu.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://udp.fzhhl.top

Ruby: def greet(name = "World") = name
来源：http://qnl.yanxiufei.cn

C#:   string Greet(string name = "World") => name;
来源：http://hwe.jqgfzy.top

[C03] 可变参数
来源：http://nom.jiagoushi.top

Py:   def total(*args): return sum(args)
来源：http://obp.zhijiandao.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gnw.sxryk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://edt.sysykeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zoh.redwolf501.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lap.iojbl.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://acj.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://eir.c1oappe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bsi.ehwqpu.com

[C04] 命名参数 / 关键字参数
来源：http://nyz.redwolf501.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zgq.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hfr.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kgv.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rmz.feifeiyinyue.top

Java: // 无：用 Builder 模式或 record
来源：http://uid.hammf.cn


<!-- 参考信息 -->