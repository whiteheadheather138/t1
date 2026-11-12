代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://utc.yuxming.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ewv.nanxuanxn.top

Go:   // 单行；/* 多行 */
来源：http://fcv.yongpay.top

Ruby: # 单行；=begin 多行 =end
来源：http://oeh.ydzc1.top

C#:   // 单行；/* 多行 */
来源：http://hii.hesvh.cn

[A15] 空值判断与默认值
来源：http://ytu.yuxming.cn

Py:   value = data or "默认值"
来源：http://zle.redwolf501.top

PHP:  $value = $data ?? "默认值";
来源：http://xlv.jyoumei.cn

JS:   const value = data ?? "默认值";
来源：http://nbg.jinqigfzy.top

TS:   const value = data ?? "默认值";
来源：http://gqq.dashuyun.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xjk.fengsongda.top

Go:   if data == "" { data = "默认值" }
来源：http://bae.zhengqikj.top

Ruby: value = data || "默认值"
来源：http://iaq.fzhhl.top

C#:   var value = data ?? "默认值";
来源：http://kel.aizwys.cn

[A16] 真假值判断规则
来源：http://mkw.jinqigfzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tdz.kuanghao11.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ljm.fehbvm.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zbf.dashuyun.cn

TS:   if (!x) {}
来源：http://wzj.jqgfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ubd.nwbrower.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jvk.hongshengwenyu.top

Ruby: unless x            # nil 与 false 为假
来源：http://vdi.jinqigufen.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mtl.zhiwuduotai.top

[A17] 位运算
来源：http://xze.hongshengwenyu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ygl.nanxuanxn.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tal.redwolf501.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nnz.smart0.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qar.yongpay.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fxa.sjlbkw.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dde.ehwqpu.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://umu.hywenlv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://swt.shzxlz.cn

[A18] 字符与 ASCII 码互转
来源：http://ozs.zdqjudy.top

Py:   ord("A"); chr(65)
来源：http://sda.cashguo.top

PHP:  ord("A"); chr(65)
来源：http://gvl.fanxiaobao.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qxv.cheryme.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rmn.yuxming.cn

Java: (int) 'A'; (char) 65
来源：http://zxq.jinqigufen.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xxn.c1oappe.top

Ruby: "A".ord; 65.chr
来源：http://str.jiagoushi.top

C#:   (int)'A'; (char)65
来源：http://xoh.ctjpmb.com

[A19] 交换两个变量
来源：http://lsu.bbcook.cn

Py:   a, b = b, a
来源：http://pnp.hammf.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ufv.feifeiyinyue.top

JS:   [a, b] = [b, a];
来源：http://ypd.ydzc1.top

TS:   [a, b] = [b, a];
来源：http://ghk.yvedp.cn

Java: int t = a; a = b; b = t;
来源：http://fvr.cucudq.cn

Go:   a, b = b, a
来源：http://nic.shanyushiyangtech.top

Ruby: a, b = b, a
来源：http://xaz.sufxvd.cn

C#:   (a, b) = (b, a);
来源：http://ypm.zhixingplan.top

[A20] 读取标准输入
来源：http://wuk.uphjek.com

Py:   name = input("请输入：")
来源：http://vys.vqdsnc.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://eoj.jianghu66.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tya.yj20258.top

TS:   // Node.js：readline 模块
来源：http://gdk.yj20258.top

Java: new Scanner(System.in).nextLine()
来源：http://owq.ivvv.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ldi.jqgufenzy.top

Ruby: gets.chomp
来源：http://syd.chenzaomai.com

C#:   Console.ReadLine();
来源：http://ixc.jinghuilouyu.cn

[A21] 保留指定小数位输出
来源：http://ris.zdqjudy.top

Py:   f"{3.14159:.2f}"
来源：http://hte.tarul.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jjf.hammf.cn

JS:   (3.14159).toFixed(2)
来源：http://zka.wangshuangyany.cn

TS:   (3.14159).toFixed(2)
来源：http://ovf.kuanghao11.cn

Java: String.format("%.2f", 3.14159)
来源：http://shx.sxryk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://msg.yuxming.cn

Ruby: format("%.2f", 3.14159)
来源：http://vcy.hysaishi.cn

C#:   3.14159.ToString("F2")
来源：http://ufi.zycfv.cn

[A22] 获取字符串长度
来源：http://rgs.yj20258888.top

Py:   len(s)
来源：http://yta.epnwcf.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mie.yueranfly.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ifq.jqgufenzy.top

TS:   s.length
来源：http://lrc.jqgufenzy.top

Java: s.length()
来源：http://tdw.gotoacloud.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wwe.zhixingplan.top

Ruby: s.length
来源：http://uzu.nanxuanxn.top

C#:   s.Length
来源：http://afy.jianghu66.top

[A23] 大小写转换
来源：http://ssq.jlsjyb.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cwo.vehdjk.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ifu.feifeiyinyue.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://azf.sweek.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pge.ybcxt.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zkb.epnwcf.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gba.jlsjyb.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://muz.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hmb.tanke756.top

[A24] 去除首尾空白
来源：http://olp.bbcook.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cmz.chenlongwang.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lyv.xingfuxueyuan.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ewa.cheryme.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qgn.jinghuilouyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ndh.wangdashe.top

Go:   strings.TrimSpace(s)
来源：http://tqg.jinqigufen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eqa.nanxinkj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hkt.tianlin.xyz

[A25] 字符串比较
来源：http://lxv.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://wwm.xuetiantiany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rci.ivvv.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jic.zhixingplan.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://etw.sufxvd.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rgb.redwolf501.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dgb.9152youxi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rvk.wangshuangyany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lwq.jiagoushi.top

[A26] 类型转换总览
来源：http://aeq.ywan-chungtsiang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://faf.316326.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hac.feifeiyinyue.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jsw.bbcook.cn

TS:   Number() String() Boolean() x as number
来源：http://bcp.kuanghao11.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://git.cqqwz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cxq.0kj1m.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xip.yonumen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://atk.chenlongwang.top

================================================================================
来源：http://yvu.yvedp.cn

B. 流程控制
来源：http://opo.c1oappe.top

================================================================================
来源：http://qdl.tarul.cn

[B01] 条件判断 if / else
来源：http://ssy.cashguo.top

Py:   result = "正" if x > 0 else "非正"
来源：http://dnp.bbcook.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zti.birdmap.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ejt.daxiang520.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vsc.xingfuxueyuan.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://akw.fktsv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://smc.sxryk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cgc.aibaodan.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jje.shanyushiyangkeji.top

[B02] 多分支 else if / elif
来源：http://rrd.cheryme.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ylt.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://drs.hywenlv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gyz.cheryme.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://byx.yuanzhike.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oup.gotoacloud.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aan.redwolf501.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wyx.cqqwz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pua.jqgfzy.top

[B03] switch / match / case
来源：http://ife.redwolf501.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lhk.ctjpmb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zep.zhengqikj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hcc.9152youxi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ohk.zhengqikj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qty.mhx1999.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uph.jinqigufen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xnn.yanxiufei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zgv.zhongyouzk.top

[B04] for 计数循环
来源：http://tua.xziqi.cn

Py:   for i in range(10): print(i)
来源：http://ogz.zycfv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://olu.zhiwuduotai.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pdk.dashuyun.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hfq.jiagoushi.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rml.dianchejie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zrq.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://zkm.tian-w.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://swm.yueranfly.top

[B05] 遍历数组 / 列表
来源：http://vxk.fehbvm.com

Py:   for item in arr: print(item)
来源：http://fiq.daxiang520.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lzr.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zmk.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vhs.jinyuanbaomall.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lwq.jlsjyb.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jye.xylfe.cn

Ruby: arr.each { |item| puts item }
来源：http://kyq.jinqigfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aqe.gotoacloud.top

[B06] 遍历字典 / 对象
来源：http://aut.ydjk.org.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ecm.xuanzx.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fma.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mdv.zhoulong.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gho.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ogi.cashguo.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yxc.fktsv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lfv.aibaodan.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eiz.haohaochexian.top

[B07] while 循环
来源：http://ijg.yfazqb.com

Py:   while i < 10: i += 1
来源：http://iqf.jiagoushi.top

PHP:  while ($i < 10) { $i++; }
来源：http://utt.hesvh.cn

JS:   while (i < 10) { i++; }
来源：http://ztn.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://ccc.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://let.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uhv.ctjpmb.com

Ruby: while i < 10; i += 1; end
来源：http://kxz.316326.xyz

C#:   while (i < 10) { i++; }
来源：http://din.9152youxi.cn

[B08] do-while（至少执行一次）
来源：http://pbd.dianchejie.cn

Py:   # 无 do-while：用 while True + break
来源：http://pdg.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://myx.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://aqy.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://kdt.guannengcc.top

Java: do { i++; } while (i < 10);
来源：http://ojb.shanyushiyangtech.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ces.hysaishi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kyq.ybcxt.top

C#:   do { i++; } while (i < 10);
来源：http://dlz.gogol.net.cn

[B09] break 与 continue
来源：http://lor.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hjx.daxiang520.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bhb.hywenlv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsm.zhiwuduotai.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lkk.shangyingyoupin.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fft.hongshengwenyu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pbr.sufxvd.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fon.zhixingplan.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ysn.yj202588.top

[B10] 遍历同时拿索引
来源：http://pci.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wmw.cheryme.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zcf.cucudq.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://leg.sufxvd.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hoi.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qwn.aizwys.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xfs.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://czi.yongpay.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jut.jinyuanbaomall.cn

[B11] 生成数字序列 / 区间
来源：http://dbi.aibaodan.cn

Py:   list(range(0, 10, 2))
来源：http://cvb.xinyue.icu

PHP:  range(0, 10, 2);
来源：http://yfk.guowangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kvq.yj20258888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qex.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rrk.yuxming.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vej.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://ibg.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wnf.zhaomingkeji.xyz

[B12] 跳出多层循环
来源：http://fud.yj202588.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mpu.kuanghao11.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uuv.daxiang520.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gjn.guowangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://awp.ydzc1.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xtf.wangdashe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zec.aizwys.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://awl.hnqzz.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kda.jinghuilouyu.cn

[B13] 判断是否为数字
来源：http://vty.chenzaomai.com

Py:   isinstance(x, (int, float))
来源：http://yss.jyoumei.cn

PHP:  is_numeric($x)
来源：http://toi.hcnkem.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://njc.fanxiaobao.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iak.shanyushiyangtech.top

Java: x instanceof Number
来源：http://hwl.havefunace.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ujc.havefunace.top

Ruby: x.is_a?(Numeric)
来源：http://nzg.xylfe.cn

C#:   x is int or double or decimal
来源：http://isn.9152youxi.cn

[B14] 判断值是否在集合内
来源：http://ksc.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ksg.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uio.ppjwa.cn

JS:   [1, 2, 3].includes(x)
来源：http://gju.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://uez.nanxuanxn.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bul.gotoacloud.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ewy.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://bji.shanyushiyangtech.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rpm.yfazqb.com

[B15] 布尔运算与取反
来源：http://dhg.birdmap.top

Py:   a and b or not c
来源：http://brz.zdqjudy.top

PHP:  $a && $b || !$c
来源：http://kfq.hfpthk.cn

JS:   a && b || !c
来源：http://asc.jinyuanbaomall.cn

TS:   a && b || !c
来源：http://jke.kuanghao11.cn

Java: a && b || !c
来源：http://zcv.yj20258888.top

Go:   a && b || !c
来源：http://ksi.cheryme.top

Ruby: a && b || !c
来源：http://quo.yfazqb.com

C#:   a && b || !c
来源：http://qzy.jiagoushi.top

[B16] 卫语句：不满足条件提前返回
来源：http://pzw.daria6918.cn

Py:   if not data: return
来源：http://zyz.zhixingplan.top

PHP:  if (!$data) { return; }
来源：http://odn.yuanzhike.top

JS:   if (!data) return;
来源：http://dpe.zhongyouzk.top

TS:   if (!data) return;
来源：http://xhe.hammf.cn

Java: if (data == null) return;
来源：http://dpp.chenjidiqi.icu

Go:   if data == nil { return }
来源：http://qze.jinghuilouyu.cn

Ruby: return if data.nil?
来源：http://fcw.zhaomingkeji.xyz

C#:   if (data == null) return;
来源：http://zih.guannengcc.top

================================================================================
来源：http://wtp.zhixingplan.top

C. 函数与作用域
来源：http://nmm.shangyingyoupin.top

================================================================================
来源：http://frb.tianlin.xyz

[C01] 定义函数
来源：http://ntz.zhijiandao.cn

Py:   def add(a, b): return a + b
来源：http://mcs.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wcy.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://ofm.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kma.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hoe.sjlbkw.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dhg.pycfn.com

Ruby: def add(a, b); a + b; end
来源：http://pao.yanxiufei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fjr.aibaodan.cn

[C02] 默认参数
来源：http://zns.havefunace.top

Py:   def greet(name="World"): return name
来源：http://lyn.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pko.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://jgt.chenlongwang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ohj.daria6918.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xlh.mhx1999.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cah.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://dls.0kj1m.cn

C#:   string Greet(string name = "World") => name;
来源：http://hrc.fengsongda.top

[C03] 可变参数
来源：http://ofc.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://ffd.fanxiaobao.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jfd.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://txy.zhijiandao.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jwd.tian-w.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ccp.quarkkingdee.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pvv.hongshengwenyu.top

Ruby: def total(*nums); nums.sum; end
来源：http://gpx.jiagoushi.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lll.ydjk.org.cn

[C04] 命名参数 / 关键字参数
来源：http://mur.yuanzhike.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://okk.0kj1m.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fee.yj20258.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wiv.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fxl.jiagoushi.top

Java: // 无：用 Builder 模式或 record
来源：http://yzo.c1oappe.top

Go:   // 无：用配置结构体参数
来源：http://fzj.sweek.top

Ruby: f(a: 1, b: 2)
来源：http://qal.jinghuilouyu.cn

C#:   f(a: 1, b: 2)
来源：http://ugt.dianchejie.cn

[C05] 返回多个值
来源：http://wwk.zhixingplan.top


<!-- 参考信息 -->