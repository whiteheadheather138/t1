代发 wailian999

Java: "第一行\n第二行"
来源：http://qhz.sxryk.cn

Go:   "第一行\n第二行"
来源：http://kea.yongpay.top

Ruby: "第一行\n第二行"
来源：http://kgb.bjfxy.top

C#:   "第一行\n第二行"
来源：http://jkg.sysykeji.top

[A14] 注释写法
来源：http://muj.sysykeji.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://mph.fzhhl.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://bkm.jinqigufen.top

JS:   // 单行；/* 多行 */
来源：http://fgv.hnqzz.top

TS:   // 单行；/* 多行 */
来源：http://qsy.andypj.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://iqs.cashguo.top

Go:   // 单行；/* 多行 */
来源：http://lwo.jinqigfzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://jri.sufxvd.cn

C#:   // 单行；/* 多行 */
来源：http://ykh.svipenyu.cn

[A15] 空值判断与默认值
来源：http://xsg.zycfv.cn

Py:   value = data or "默认值"
来源：http://cej.yj20258.top

PHP:  $value = $data ?? "默认值";
来源：http://dzq.tianlin.xyz

JS:   const value = data ?? "默认值";
来源：http://ydh.cdnleiting.top

TS:   const value = data ?? "默认值";
来源：http://xjy.zycfv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://eah.zhixingplan.top

Go:   if data == "" { data = "默认值" }
来源：http://meh.hcnkem.com

Ruby: value = data || "默认值"
来源：http://emq.cashguo.top

C#:   var value = data ?? "默认值";
来源：http://prt.vqdsnc.cn

[A16] 真假值判断规则
来源：http://jge.kuanghao11.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kze.ppjwa.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://swq.fktsv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fzw.tianlin.xyz

TS:   if (!x) {}
来源：http://aaa.chenlongwang.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bnp.c1oappe.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rcw.aizwys.cn

Ruby: unless x            # nil 与 false 为假
来源：http://npy.hesvh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mru.pengpengdd.cyou

[A17] 位运算
来源：http://mck.ydjk.org.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tmb.xuetiantiany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://szy.chenjidiqi.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hdc.ywan-chungtsiang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zxc.yj20258888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tgy.daria6918.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vny.zhijiandao.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jrz.zhaomingkeji.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vjp.iojbl.cn

[A18] 字符与 ASCII 码互转
来源：http://eqs.bbcook.cn

Py:   ord("A"); chr(65)
来源：http://law.yj20258.top

PHP:  ord("A"); chr(65)
来源：http://fht.gzhubu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uqm.c1oappe.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fyj.aizwys.cn

Java: (int) 'A'; (char) 65
来源：http://uvl.dashuyun.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cwv.chenjidiqi.icu

Ruby: "A".ord; 65.chr
来源：http://usa.ydjk.org.cn

C#:   (int)'A'; (char)65
来源：http://wrq.sxryk.cn

[A19] 交换两个变量
来源：http://kgq.sysykeji.top

Py:   a, b = b, a
来源：http://tar.zhengqikj.top

PHP:  [$a, $b] = [$b, $a];
来源：http://gbp.316326.xyz

JS:   [a, b] = [b, a];
来源：http://wmr.haohaochexian.top

TS:   [a, b] = [b, a];
来源：http://tfc.meibo888.top

Java: int t = a; a = b; b = t;
来源：http://ydm.zdqjudy.top

Go:   a, b = b, a
来源：http://rhs.bjfxy.top

Ruby: a, b = b, a
来源：http://ivo.zhiwuduotai.top

C#:   (a, b) = (b, a);
来源：http://qet.ydjk.org.cn

[A20] 读取标准输入
来源：http://tkf.9152youxi.cn

Py:   name = input("请输入：")
来源：http://nww.zhongyouzk.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qze.sysykeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nkd.aizwys.cn

TS:   // Node.js：readline 模块
来源：http://ked.yuxming.cn

Java: new Scanner(System.in).nextLine()
来源：http://hej.mhx1999.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://reh.cucudq.cn

Ruby: gets.chomp
来源：http://shn.gzhubu.top

C#:   Console.ReadLine();
来源：http://xjy.zhiwuduotai.top

[A21] 保留指定小数位输出
来源：http://gkv.hywenlv.cn

Py:   f"{3.14159:.2f}"
来源：http://zms.gogol.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vio.jinyuanbaomall.cn

JS:   (3.14159).toFixed(2)
来源：http://qem.cucudq.cn

TS:   (3.14159).toFixed(2)
来源：http://thp.jianghu66.top

Java: String.format("%.2f", 3.14159)
来源：http://dip.xziqi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://izc.nanxuanxn.top

Ruby: format("%.2f", 3.14159)
来源：http://sip.chenjidiqi.icu

C#:   3.14159.ToString("F2")
来源：http://ebr.hnqzz.top

[A22] 获取字符串长度
来源：http://umg.aibaodan.cn

Py:   len(s)
来源：http://zlj.ybcxt.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gqw.fktsv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fab.hcnkem.com

TS:   s.length
来源：http://pbx.chenzaomai.com

Java: s.length()
来源：http://ybv.uphjek.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ldn.jyoumei.cn

Ruby: s.length
来源：http://jqg.xziqi.cn

C#:   s.Length
来源：http://bpf.pycfn.com

[A23] 大小写转换
来源：http://wff.gaohongyu789.top

Py:   s.upper(); s.lower(); s.title()
来源：http://zma.xingfuxueyuan.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qfw.zhongyouzk.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rog.haohaochexian.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ily.xinyue.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hmu.yj202588.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pxz.316326.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lgi.ehwqpu.com

C#:   s.ToUpper(); s.ToLower()
来源：http://yzm.smart0.xyz

[A24] 去除首尾空白
来源：http://xhh.shangyingyoupin.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lek.jyoumei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yin.xylfe.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://brm.tarul.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yuk.ydzc1.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nyy.hfpthk.cn

Go:   strings.TrimSpace(s)
来源：http://bdv.zdbjq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qcr.jinqigfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tof.fzhhl.top

[A25] 字符串比较
来源：http://nnh.yvedp.cn

Py:   s1 == s2; s1 != s2
来源：http://djx.chenlongwang.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bwm.yfazqb.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nrk.yuanzhike.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wwd.shanyushiyangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://obd.hcnkem.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://emi.sysykeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tvl.vqdsnc.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mef.0kj1m.cn

[A26] 类型转换总览
来源：http://dtq.yvedp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uxl.smart0.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cvo.sweek.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fne.gotoacloud.top

TS:   Number() String() Boolean() x as number
来源：http://sid.daria6918.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://aya.gzhubu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pfc.shanyushiyangtech.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ugz.fktsv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zvc.hammf.cn

================================================================================
来源：http://oup.jinyuanbaomall.cn

B. 流程控制
来源：http://nho.ivvv.top

================================================================================
来源：http://bnv.tarul.cn

[B01] 条件判断 if / else
来源：http://gcq.pycfn.com

Py:   result = "正" if x > 0 else "非正"
来源：http://jqk.guannengcc.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wlo.birdmap.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://trk.aibaodan.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ysu.fanxiaobao.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://vto.zhiwuduotai.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pwd.yj20258888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ddu.ivvv.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://igi.vehdjk.com

[B02] 多分支 else if / elif
来源：http://evi.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ttd.ywan-chungtsiang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://one.yueranfly.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cvi.tanke756.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mkm.xuetiantiany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jov.gotoacloud.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dos.ppjwa.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yar.smart0.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://brc.sweek.top

[B03] switch / match / case
来源：http://zbj.zhiwuduotai.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zbj.ydjk.org.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tom.hnqzz.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ifx.vehdjk.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gvc.mhx1999.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mez.tanke756.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qpt.yuxming.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pfl.pycfn.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nys.yueranfly.top

[B04] for 计数循环
来源：http://bzv.pengpengdd.cyou

Py:   for i in range(10): print(i)
来源：http://sjd.xuetiantiany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uch.mhx1999.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lni.zhixingplan.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gen.9152youxi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eib.c1oappe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://djo.guowangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://mcy.hysaishi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://loh.yongpay.top

[B05] 遍历数组 / 列表
来源：http://qvq.ivvv.top

Py:   for item in arr: print(item)
来源：http://gfv.jqgufenzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aep.xinyue.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://gwa.jqgufenzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qyc.yuxming.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sjw.bjfxy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vos.fktsv.cn

Ruby: arr.each { |item| puts item }
来源：http://tgx.feifeiyinyue.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vcq.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://pla.jqgufenzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ncq.zycfv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vlm.cheryme.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bpb.fehbvm.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gci.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://arn.haohaochexian.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gpo.shanyushiyangtech.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dcn.shuidangran.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://caa.snrcjt.cn

[B07] while 循环
来源：http://ioo.nwbrower.top

Py:   while i < 10: i += 1
来源：http://iqf.ywan-chungtsiang.top

PHP:  while ($i < 10) { $i++; }
来源：http://mjw.guowangkeji.top

JS:   while (i < 10) { i++; }
来源：http://hsw.sxryk.cn

TS:   while (i < 10) { i++; }
来源：http://lqb.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://iet.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ifz.dashuyun.cn

Ruby: while i < 10; i += 1; end
来源：http://wmw.zhaomingkeji.xyz

C#:   while (i < 10) { i++; }
来源：http://uob.zhixingplan.top

[B08] do-while（至少执行一次）
来源：http://giu.jyoumei.cn

Py:   # 无 do-while：用 while True + break
来源：http://vww.vqdsnc.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ufn.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://zsy.hnxiangtu.top

TS:   do { i++; } while (i < 10);
来源：http://arv.wangshuangyany.cn

Java: do { i++; } while (i < 10);
来源：http://vtr.meibo888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://btt.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hiz.hfpthk.cn

C#:   do { i++; } while (i < 10);
来源：http://dve.chenjidiqi.icu

[B09] break 与 continue
来源：http://ijp.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mrs.sweek.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oef.snrcjt.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tlq.hnxiangtu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ujn.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cun.gzhubu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jhj.yvedp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hly.xylfe.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tlp.meibo888.top

[B10] 遍历同时拿索引
来源：http://one.jinqigufen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://geu.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pen.shuidangran.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gmu.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xrg.hammf.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jzh.daria6918.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uws.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aln.jiagoushi.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jzj.ehwqpu.com

[B11] 生成数字序列 / 区间
来源：http://zdv.vehdjk.com

Py:   list(range(0, 10, 2))
来源：http://awu.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://vqz.andypj.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zzd.dashuyun.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qcd.nwbrower.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uqq.vqdsnc.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lfg.chenjidiqi.icu

Ruby: (0...10).step(2).to_a
来源：http://cua.xingfuxueyuan.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://avn.daxiang520.top

[B12] 跳出多层循环
来源：http://dij.zhijiandao.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ito.pycfn.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://hod.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mze.sweek.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fcn.chenjidiqi.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qic.xinyue.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wzc.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bil.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jjr.zhengqikj.top

[B13] 判断是否为数字
来源：http://ydf.cqqwz.cn

Py:   isinstance(x, (int, float))
来源：http://ybd.yj20258888.top

PHP:  is_numeric($x)
来源：http://yuq.ehwqpu.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fnk.zdqjudy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nks.yj202588.top

Java: x instanceof Number
来源：http://wyv.fktsv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yrp.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://eas.jiagoushi.top

C#:   x is int or double or decimal
来源：http://anw.epnwcf.com

[B14] 判断值是否在集合内
来源：http://vrh.sxryk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fil.hongshengwenyu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qnv.hesvh.cn

JS:   [1, 2, 3].includes(x)
来源：http://odb.hnxiangtu.top

TS:   [1, 2, 3].includes(x)
来源：http://cpk.redwolf501.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yxg.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ydz.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uft.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rrm.guowangkeji.top

[B15] 布尔运算与取反
来源：http://ned.tianlin.xyz

Py:   a and b or not c
来源：http://nnc.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://hjd.tanke756.top

JS:   a && b || !c
来源：http://xbu.cheryme.top

TS:   a && b || !c
来源：http://hgh.havefunace.top

Java: a && b || !c
来源：http://llg.andypj.xyz

Go:   a && b || !c
来源：http://pps.feifeiyinyue.top

Ruby: a && b || !c
来源：http://umh.xziqi.cn

C#:   a && b || !c
来源：http://cis.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ihu.cucudq.cn

Py:   if not data: return
来源：http://xke.haohaochexian.top

PHP:  if (!$data) { return; }
来源：http://lkb.bjfxy.top

JS:   if (!data) return;
来源：http://tcf.ydzc1.top

TS:   if (!data) return;
来源：http://opj.jqgufenzy.top

Java: if (data == null) return;
来源：http://bri.vqdsnc.cn

Go:   if data == nil { return }
来源：http://krm.zhoulong.xyz

Ruby: return if data.nil?
来源：http://kih.yj202588.top

C#:   if (data == null) return;
来源：http://ldv.zhengqikj.top

================================================================================
来源：http://wfc.xinyue.icu

C. 函数与作用域
来源：http://yei.redwolf501.top

================================================================================
来源：http://oma.gaohongyu789.top

[C01] 定义函数
来源：http://nga.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://kwe.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://scn.yanxiufei.cn

JS:   function add(a, b) { return a + b; }
来源：http://wpu.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ivz.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://owy.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gjp.yj20258888.top

Ruby: def add(a, b); a + b; end
来源：http://zmp.cqqwz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qxs.jianghu66.top

[C02] 默认参数
来源：http://raw.aibaodan.cn

Py:   def greet(name="World"): return name
来源：http://zgc.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bzj.mhx1999.top

JS:   function greet(name = "World") { return name; }
来源：http://ssc.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dgx.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://veh.jqgfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cja.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://akt.shanyushiyangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://vam.ydjk.org.cn

[C03] 可变参数
来源：http://yam.cdnleiting.top

Py:   def total(*args): return sum(args)
来源：http://uwo.tarul.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mvk.fehbvm.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yho.yj202588.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gcd.cdnleiting.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fbt.quarkkingdee.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dal.ctjpmb.com

Ruby: def total(*nums); nums.sum; end
来源：http://erw.ctjpmb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bfd.wangdashe.top

[C04] 命名参数 / 关键字参数
来源：http://wxm.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kia.zhiwuduotai.top


<!-- 参考信息 -->