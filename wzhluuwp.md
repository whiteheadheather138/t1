代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://jwo.iojbl.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lkz.aibaodan.cn

Go:   // 单行；/* 多行 */
来源：http://wrq.zhiwuduotai.top

Ruby: # 单行；=begin 多行 =end
来源：http://glk.xziqi.cn

C#:   // 单行；/* 多行 */
来源：http://gaq.haohaochexian.top

[A15] 空值判断与默认值
来源：http://xqw.xuanzx.com

Py:   value = data or "默认值"
来源：http://det.jinqigfzy.top

PHP:  $value = $data ?? "默认值";
来源：http://uvy.tianlin.xyz

JS:   const value = data ?? "默认值";
来源：http://ubo.chenzaomai.com

TS:   const value = data ?? "默认值";
来源：http://ktl.daxiang520.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wcf.yj20258.top

Go:   if data == "" { data = "默认值" }
来源：http://xgb.pengpengdd.cyou

Ruby: value = data || "默认值"
来源：http://pxv.ivvv.top

C#:   var value = data ?? "默认值";
来源：http://hwc.meibo888.top

[A16] 真假值判断规则
来源：http://bgw.yongpay.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ieq.jlsjyb.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://aci.tian-w.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vpi.zhixingplan.top

TS:   if (!x) {}
来源：http://cpk.pengpengdd.cyou

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qft.snrcjt.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gsr.yueranfly.top

Ruby: unless x            # nil 与 false 为假
来源：http://stk.yfazqb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vuu.yfazqb.com

[A17] 位运算
来源：http://anl.epnwcf.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uhj.ydzc1.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ewi.yj20258888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ihs.hnxiangtu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://syw.haohaochexian.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://krn.hesvh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xrq.gogol.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wcb.nanxuanxn.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kdr.chenjidiqi.icu

[A18] 字符与 ASCII 码互转
来源：http://ify.cqqwz.cn

Py:   ord("A"); chr(65)
来源：http://qpe.hongshengwenyu.top

PHP:  ord("A"); chr(65)
来源：http://ivn.zhiwuduotai.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ycz.ehwqpu.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xqt.fktsv.cn

Java: (int) 'A'; (char) 65
来源：http://zcq.cqqwz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jwi.svipenyu.cn

Ruby: "A".ord; 65.chr
来源：http://ypx.jiagoushi.top

C#:   (int)'A'; (char)65
来源：http://zre.jiagoushi.top

[A19] 交换两个变量
来源：http://pqk.guannengcc.top

Py:   a, b = b, a
来源：http://enl.smart0.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://vwy.sufxvd.cn

JS:   [a, b] = [b, a];
来源：http://gqf.zhongyouzk.top

TS:   [a, b] = [b, a];
来源：http://tzb.fehbvm.com

Java: int t = a; a = b; b = t;
来源：http://eip.jinyuanbaomall.cn

Go:   a, b = b, a
来源：http://xzm.vehdjk.com

Ruby: a, b = b, a
来源：http://rre.hammf.cn

C#:   (a, b) = (b, a);
来源：http://vmq.xylfe.cn

[A20] 读取标准输入
来源：http://elg.jinyuanbaomall.cn

Py:   name = input("请输入：")
来源：http://lku.9152youxi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qje.zhongyouzk.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zte.dashuyun.cn

TS:   // Node.js：readline 模块
来源：http://ths.yj202588.top

Java: new Scanner(System.in).nextLine()
来源：http://xef.52xcode.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pvs.jianghu66.top

Ruby: gets.chomp
来源：http://cyf.smart0.xyz

C#:   Console.ReadLine();
来源：http://ppa.hcnkem.com

[A21] 保留指定小数位输出
来源：http://lfi.dianchejie.cn

Py:   f"{3.14159:.2f}"
来源：http://ovv.nwbrower.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uau.dashuyun.cn

JS:   (3.14159).toFixed(2)
来源：http://vey.0kj1m.cn

TS:   (3.14159).toFixed(2)
来源：http://xzn.sjlbkw.cn

Java: String.format("%.2f", 3.14159)
来源：http://dco.gogol.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zaa.yj20258888.top

Ruby: format("%.2f", 3.14159)
来源：http://ghw.wangshuangyany.cn

C#:   3.14159.ToString("F2")
来源：http://cia.hywenlv.cn

[A22] 获取字符串长度
来源：http://kym.hfpthk.cn

Py:   len(s)
来源：http://lqb.xinyue.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://llm.epnwcf.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://iue.gaohongyu789.top

TS:   s.length
来源：http://yra.smart0.xyz

Java: s.length()
来源：http://mjq.0kj1m.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lax.mhx1999.top

Ruby: s.length
来源：http://ysa.yvedp.cn

C#:   s.Length
来源：http://ras.sweek.top

[A23] 大小写转换
来源：http://ftq.fanxiaobao.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://jac.316326.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jnm.aibaodan.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ipn.jinqigufen.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cba.quarkkingdee.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kuy.yangfankeji.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://crl.316326.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://one.0kj1m.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nhl.yj202588.top

[A24] 去除首尾空白
来源：http://puy.xuanzx.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://swl.hongshengwenyu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vdg.yongpay.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uxi.yj202588.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tfy.hysaishi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ron.mhx1999.top

Go:   strings.TrimSpace(s)
来源：http://cpc.jinghuilouyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cnx.guowangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://spb.aizwys.cn

[A25] 字符串比较
来源：http://btu.ehwqpu.com

Py:   s1 == s2; s1 != s2
来源：http://vhm.ydzc1.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://owz.shuidangran.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zvn.jlsjyb.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xnm.pycfn.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vui.svipenyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qsd.aizwys.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pog.yj202588.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wvf.mhx1999.top

[A26] 类型转换总览
来源：http://txf.ppjwa.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xps.ehwqpu.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vda.316326.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rvn.jqgufenzy.top

TS:   Number() String() Boolean() x as number
来源：http://gnu.xingfuxueyuan.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iew.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qqq.nwbrower.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://nuc.hongshengwenyu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://onz.nanxinkj.top

================================================================================
来源：http://hjy.hesvh.cn

B. 流程控制
来源：http://eap.wangshuangyany.cn

================================================================================
来源：http://ngg.chenjidiqi.icu

[B01] 条件判断 if / else
来源：http://ftu.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://cwt.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yvz.yj20258888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vpu.c1oappe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://awx.jianghu66.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ywc.cucudq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kqh.andypj.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pua.hcnkem.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cjz.jinyuanbaomall.cn

[B02] 多分支 else if / elif
来源：http://acb.cdnleiting.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pmp.cucudq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gqi.jqgufenzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mtp.haohaochexian.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mbw.nwbrower.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://unt.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ugz.aibaodan.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://akt.vqdsnc.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ogo.tian-w.cn

[B03] switch / match / case
来源：http://huz.daria6918.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://leu.fehbvm.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ihh.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fxp.nwbrower.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tjp.svipenyu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oyx.wangdashe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://akp.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dif.hnxiangtu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iyq.sufxvd.cn

[B04] for 计数循环
来源：http://vjp.shangyingyoupin.top

Py:   for i in range(10): print(i)
来源：http://erz.ywan-chungtsiang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://agi.fanxiaobao.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rje.jiagoushi.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dgn.ywan-chungtsiang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rhu.vehdjk.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://asi.jqgfzy.top

Ruby: 10.times { |i| puts i }
来源：http://wlp.jianghu66.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bwy.smart0.xyz

[B05] 遍历数组 / 列表
来源：http://qdt.xziqi.cn

Py:   for item in arr: print(item)
来源：http://ips.gotoacloud.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ail.c1oappe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://pov.yj20258888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yup.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://avn.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mus.shanyushiyangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://ntg.bbcook.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zts.aizwys.cn

[B06] 遍历字典 / 对象
来源：http://pqr.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zpe.wangdashe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yuy.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ktw.ppjwa.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vmn.zhijiandao.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rxj.shanyushiyangkeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kug.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ceb.guannengcc.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://auz.hesvh.cn

[B07] while 循环
来源：http://wnp.zhixingplan.top

Py:   while i < 10: i += 1
来源：http://bng.sxryk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pgq.gotoacloud.top

JS:   while (i < 10) { i++; }
来源：http://mei.dashuyun.cn

TS:   while (i < 10) { i++; }
来源：http://pci.yj20258.top

Java: while (i < 10) { i++; }
来源：http://kbj.316326.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bmq.zhijiandao.cn

Ruby: while i < 10; i += 1; end
来源：http://geo.hesvh.cn

C#:   while (i < 10) { i++; }
来源：http://vql.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://usz.sxryk.cn

Py:   # 无 do-while：用 while True + break
来源：http://yze.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lnl.yangfankeji.com

JS:   do { i++; } while (i < 10);
来源：http://dsb.ydzc1.top

TS:   do { i++; } while (i < 10);
来源：http://usu.wangdashe.top

Java: do { i++; } while (i < 10);
来源：http://qgx.zhixingplan.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zfu.jqgfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://kwe.zhengqikj.top

C#:   do { i++; } while (i < 10);
来源：http://vqf.hcnkem.com

[B09] break 与 continue
来源：http://cql.xuanzx.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cke.gaohongyu789.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uhi.haohaochexian.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jxi.hysaishi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vty.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fyi.tarul.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qah.jqgfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ejq.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nhz.yangfankeji.com

[B10] 遍历同时拿索引
来源：http://kxe.ehwqpu.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://akp.ydzc1.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cya.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ehv.yuanzhike.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gos.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://miu.xuanzx.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pme.zycfv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nmy.svipenyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xzl.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://ajj.yj20258888.top

Py:   list(range(0, 10, 2))
来源：http://wpb.yfazqb.com

PHP:  range(0, 10, 2);
来源：http://jwq.9152youxi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mil.xuanzx.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aki.xuanzx.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://edy.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cdc.zhixingplan.top

Ruby: (0...10).step(2).to_a
来源：http://cfq.aibaodan.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ivk.fengsongda.top

[B12] 跳出多层循环
来源：http://ksc.hammf.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jou.hywenlv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wum.sweek.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cpa.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uvf.nwbrower.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jnh.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vso.nanxinkj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gxs.fehbvm.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://byx.zhixingplan.top

[B13] 判断是否为数字
来源：http://gjj.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://kfi.bjfxy.top

PHP:  is_numeric($x)
来源：http://mbl.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bbl.uphjek.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uwz.ivvv.top

Java: x instanceof Number
来源：http://cco.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xgg.chenzaomai.com

Ruby: x.is_a?(Numeric)
来源：http://syq.xuanzx.com

C#:   x is int or double or decimal
来源：http://nxc.nwbrower.top

[B14] 判断值是否在集合内
来源：http://utx.52xcode.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jhv.ydjk.org.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qwb.zhaomingkeji.xyz

JS:   [1, 2, 3].includes(x)
来源：http://qxs.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://vku.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gbg.sxryk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eev.havefunace.top

Ruby: [1, 2, 3].include?(x)
来源：http://aag.cucudq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zxr.vehdjk.com

[B15] 布尔运算与取反
来源：http://nvo.jqgufenzy.top

Py:   a and b or not c
来源：http://aya.shanyushiyangkeji.top

PHP:  $a && $b || !$c
来源：http://uru.hnxiangtu.top

JS:   a && b || !c
来源：http://ohc.iojbl.cn

TS:   a && b || !c
来源：http://wyr.jqgfzy.top

Java: a && b || !c
来源：http://gci.dashuyun.cn

Go:   a && b || !c
来源：http://zxz.jinqigfzy.top

Ruby: a && b || !c
来源：http://tib.yongpay.top

C#:   a && b || !c
来源：http://ope.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://fnw.jinyuanbaomall.cn

Py:   if not data: return
来源：http://sih.jianghu66.top

PHP:  if (!$data) { return; }
来源：http://myu.zhengqikj.top

JS:   if (!data) return;
来源：http://wde.tanke756.top

TS:   if (!data) return;
来源：http://psq.hesvh.cn

Java: if (data == null) return;
来源：http://fkt.jiagoushi.top

Go:   if data == nil { return }
来源：http://wcu.hongshengwenyu.top

Ruby: return if data.nil?
来源：http://foq.gotoacloud.top

C#:   if (data == null) return;
来源：http://psr.aizwys.cn

================================================================================
来源：http://fya.zhongyouzk.top

C. 函数与作用域
来源：http://dpt.yfazqb.com

================================================================================
来源：http://uqj.fanxiaobao.xyz

[C01] 定义函数
来源：http://wqm.ywan-chungtsiang.top

Py:   def add(a, b): return a + b
来源：http://rnv.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xll.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://tuo.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uxr.svipenyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lns.ctjpmb.com

Go:   func add(a, b int) int { return a + b }
来源：http://mzz.shuidangran.top

Ruby: def add(a, b); a + b; end
来源：http://llr.fengsongda.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xew.shzxlz.cn

[C02] 默认参数
来源：http://nkz.yvedp.cn

Py:   def greet(name="World"): return name
来源：http://aaa.zdqjudy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tbp.yj20258.top

JS:   function greet(name = "World") { return name; }
来源：http://icd.meibo888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rwu.ctjpmb.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ehg.tianlin.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://inz.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://ciy.tian-w.cn

C#:   string Greet(string name = "World") => name;
来源：http://twb.jinqigfzy.top

[C03] 可变参数
来源：http://vad.yuxming.cn

Py:   def total(*args): return sum(args)
来源：http://ctb.chenjidiqi.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ayq.dianchejie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ndv.cdnleiting.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fsr.nanxinkj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qff.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nvb.jqgfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://xew.jlsjyb.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sxr.316326.xyz

[C04] 命名参数 / 关键字参数
来源：http://bee.zhongyouzk.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bsm.daria6918.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ljk.zhixingplan.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tht.shanyushiyangtech.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://emw.shanyushiyangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://mtx.svipenyu.cn

Go:   // 无：用配置结构体参数
来源：http://kre.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://aoc.xuanzx.com

C#:   f(a: 1, b: 2)
来源：http://fxd.0kj1m.cn

[C05] 返回多个值
来源：http://wyo.xuanzx.com


<!-- 参考信息 -->