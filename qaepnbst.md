代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://aoh.cucudq.cn

[A11] 条件表达式（三元）
来源：http://euz.chenjidiqi.icu

Py:   "yes" if x > 0 else "no"
来源：http://vlq.bjfxy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://vtw.xuetiantiany.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gls.xingfuxueyuan.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://tbq.snrcjt.cn

Java: x > 0 ? "yes" : "no"
来源：http://vlo.jinqigfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://cpm.zhijiandao.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bpg.zdqjudy.top

C#:   x > 0 ? "yes" : "no"
来源：http://cvs.jinghuilouyu.cn

[A12] 字符串插值 / 格式化
来源：http://lsb.birdmap.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://heu.vqdsnc.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mnd.wangshuangyany.cn

JS:   `Hello, ${name}!`
来源：http://ykr.feifeiyinyue.top

TS:   `Hello, ${name}!`
来源：http://ipg.jqgfzy.top

Java: "Hello, %s!".formatted(name)
来源：http://dea.chenlongwang.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://icr.cashguo.top

Ruby: "Hello, #{name}!"
来源：http://uuy.chenjidiqi.icu

C#:   $"Hello, {name}!"
来源：http://flk.snrcjt.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wtu.dashuyun.cn

Py:   "第一行\n第二行"
来源：http://tzv.yonumen.top

PHP:  "第一行\n第二行"
来源：http://caw.kuanghao11.cn

JS:   "第一行\n第二行"
来源：http://izt.mhx1999.top

TS:   "第一行\n第二行"
来源：http://sei.jinyuanbaomall.cn

Java: "第一行\n第二行"
来源：http://bea.shangyingyoupin.top

Go:   "第一行\n第二行"
来源：http://zct.wangdashe.top

Ruby: "第一行\n第二行"
来源：http://msq.zhiwuduotai.top

C#:   "第一行\n第二行"
来源：http://whs.jyoumei.cn

[A14] 注释写法
来源：http://ucf.sweek.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://nkm.zhiwuduotai.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dsh.wangshuangyany.cn

JS:   // 单行；/* 多行 */
来源：http://xrs.hnxiangtu.top

TS:   // 单行；/* 多行 */
来源：http://ptf.yj202588.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tyz.nanxinkj.top

Go:   // 单行；/* 多行 */
来源：http://egc.cashguo.top

Ruby: # 单行；=begin 多行 =end
来源：http://wec.smart0.xyz

C#:   // 单行；/* 多行 */
来源：http://rzn.svipenyu.cn

[A15] 空值判断与默认值
来源：http://woy.ywan-chungtsiang.top

Py:   value = data or "默认值"
来源：http://ypo.xingfuxueyuan.xyz

PHP:  $value = $data ?? "默认值";
来源：http://fzo.vehdjk.com

JS:   const value = data ?? "默认值";
来源：http://pvp.jinqigfzy.top

TS:   const value = data ?? "默认值";
来源：http://dzd.zycfv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mmn.hysaishi.cn

Go:   if data == "" { data = "默认值" }
来源：http://cxq.zhoulong.xyz

Ruby: value = data || "默认值"
来源：http://rhx.jqgfzy.top

C#:   var value = data ?? "默认值";
来源：http://oxu.birdmap.top

[A16] 真假值判断规则
来源：http://glr.daria6918.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eys.aibaodan.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yfr.xingfuxueyuan.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://utv.yonumen.top

TS:   if (!x) {}
来源：http://yuz.xinyue.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jlq.yanxiufei.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://htd.hywenlv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dqd.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://egp.cdnleiting.top

[A17] 位运算
来源：http://gec.zycfv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rvr.jinyuanbaomall.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qhr.zhoulong.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fih.gogol.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://emh.jqgfzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ocz.yfazqb.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hsl.c1oappe.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xob.xingfuxueyuan.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vzk.xuanzx.com

[A18] 字符与 ASCII 码互转
来源：http://mjw.feifeiyinyue.top

Py:   ord("A"); chr(65)
来源：http://hap.jiagoushi.top

PHP:  ord("A"); chr(65)
来源：http://jto.hammf.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gux.daxiang520.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pqp.uphjek.com

Java: (int) 'A'; (char) 65
来源：http://kxy.iojbl.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ntt.gotoacloud.top

Ruby: "A".ord; 65.chr
来源：http://uks.zhengqikj.top

C#:   (int)'A'; (char)65
来源：http://ocv.bbcook.cn

[A19] 交换两个变量
来源：http://iaq.hywenlv.cn

Py:   a, b = b, a
来源：http://gus.vehdjk.com

PHP:  [$a, $b] = [$b, $a];
来源：http://bpk.vehdjk.com

JS:   [a, b] = [b, a];
来源：http://qvm.vqdsnc.cn

TS:   [a, b] = [b, a];
来源：http://ccr.gotoacloud.top

Java: int t = a; a = b; b = t;
来源：http://hbg.havefunace.top

Go:   a, b = b, a
来源：http://wqx.gzhubu.top

Ruby: a, b = b, a
来源：http://sac.gaohongyu789.top

C#:   (a, b) = (b, a);
来源：http://fpr.jyoumei.cn

[A20] 读取标准输入
来源：http://qou.0kj1m.cn

Py:   name = input("请输入：")
来源：http://lcq.zhaomingkeji.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://yrm.xuanzx.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ynx.ehwqpu.com

TS:   // Node.js：readline 模块
来源：http://pjn.yuanzhike.top

Java: new Scanner(System.in).nextLine()
来源：http://kfc.yfazqb.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qnk.sufxvd.cn

Ruby: gets.chomp
来源：http://lzb.guannengcc.top

C#:   Console.ReadLine();
来源：http://mmn.yj20258888.top

[A21] 保留指定小数位输出
来源：http://ddp.bjfxy.top

Py:   f"{3.14159:.2f}"
来源：http://crs.cdnleiting.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zyi.jinqigfzy.top

JS:   (3.14159).toFixed(2)
来源：http://tty.cdnleiting.top

TS:   (3.14159).toFixed(2)
来源：http://nkl.yfazqb.com

Java: String.format("%.2f", 3.14159)
来源：http://whl.jqgufenzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zre.ydjk.org.cn

Ruby: format("%.2f", 3.14159)
来源：http://fbl.gotoacloud.top

C#:   3.14159.ToString("F2")
来源：http://kfn.ywan-chungtsiang.top

[A22] 获取字符串长度
来源：http://zkv.xingfuxueyuan.xyz

Py:   len(s)
来源：http://deo.mhx1999.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gvo.sufxvd.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xfx.zycfv.cn

TS:   s.length
来源：http://zad.haohaochexian.top

Java: s.length()
来源：http://nsc.cashguo.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rgk.zhongyouzk.top

Ruby: s.length
来源：http://hdg.zhoulong.xyz

C#:   s.Length
来源：http://fcx.fktsv.cn

[A23] 大小写转换
来源：http://kgb.kuanghao11.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sim.jinghuilouyu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fdn.cashguo.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xam.316326.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ckw.uphjek.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://msq.guannengcc.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pnm.hcnkem.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hsr.dashuyun.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qbu.hcnkem.com

[A24] 去除首尾空白
来源：http://tjv.hnqzz.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://siq.yj20258.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yxr.tian-w.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kwu.zdbjq.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://byy.zhengqikj.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mdz.andypj.xyz

Go:   strings.TrimSpace(s)
来源：http://dqi.yuanzhike.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uru.hnxiangtu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pjs.fengsongda.top

[A25] 字符串比较
来源：http://jsa.snrcjt.cn

Py:   s1 == s2; s1 != s2
来源：http://efv.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://amp.sysykeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ugf.yj20258.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ixk.gogol.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rod.ydzc1.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uqr.gaohongyu789.top

Ruby: s1 == s2; s1 <=> s2
来源：http://lkx.shanyushiyangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ryn.vehdjk.com

[A26] 类型转换总览
来源：http://kwi.0kj1m.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qui.dashuyun.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wlu.cucudq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://flc.pycfn.com

TS:   Number() String() Boolean() x as number
来源：http://hie.sweek.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jqk.jqgufenzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pxx.uphjek.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://oya.yj20258888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://buy.yj20258888.top

================================================================================
来源：http://kkd.hnxiangtu.top

B. 流程控制
来源：http://jsv.kuanghao11.cn

================================================================================
来源：http://kex.gzhubu.top

[B01] 条件判断 if / else
来源：http://fuz.svipenyu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gfc.jinghuilouyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lob.cqqwz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ivc.yongpay.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bno.tarul.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bpj.hfpthk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yyc.gzhubu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kji.chenjidiqi.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tkr.zhiwuduotai.top

[B02] 多分支 else if / elif
来源：http://ixy.svipenyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xgu.shuidangran.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://axk.ybcxt.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://npd.jqgufenzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zei.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hmi.havefunace.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hxs.tian-w.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://njz.birdmap.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oke.gaohongyu789.top

[B03] switch / match / case
来源：http://kkf.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mfm.jianghu66.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rlc.zhiwuduotai.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gww.kuanghao11.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vfp.ywan-chungtsiang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://esi.bjfxy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fkn.ybcxt.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kqb.nwbrower.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wvo.birdmap.top

[B04] for 计数循环
来源：http://ybz.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://eez.ybcxt.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://faq.hysaishi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ikg.iojbl.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://buf.yuxming.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mvr.quarkkingdee.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vpl.9152youxi.cn

Ruby: 10.times { |i| puts i }
来源：http://mba.shuidangran.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zzh.chenzaomai.com

[B05] 遍历数组 / 列表
来源：http://jtr.vqdsnc.cn

Py:   for item in arr: print(item)
来源：http://qad.zhaomingkeji.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ebw.ehwqpu.com

JS:   for (const item of arr) { console.log(item); }
来源：http://idf.hnxiangtu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yhv.sxryk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bgy.jinyuanbaomall.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rbl.hysaishi.cn

Ruby: arr.each { |item| puts item }
来源：http://hgy.xuetiantiany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://shl.hongshengwenyu.top

[B06] 遍历字典 / 对象
来源：http://wzz.hongshengwenyu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ycs.yfazqb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pjb.zhijiandao.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pzu.xziqi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cex.yanxiufei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bsf.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xsf.316326.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vzy.feifeiyinyue.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://omg.hysaishi.cn

[B07] while 循环
来源：http://gyr.jinqigufen.top

Py:   while i < 10: i += 1
来源：http://iok.bbcook.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ouw.c1oappe.top

JS:   while (i < 10) { i++; }
来源：http://cxk.yj202588.top

TS:   while (i < 10) { i++; }
来源：http://opv.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://kol.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qfz.0kj1m.cn

Ruby: while i < 10; i += 1; end
来源：http://gno.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://hru.yongpay.top

[B08] do-while（至少执行一次）
来源：http://fcw.birdmap.top

Py:   # 无 do-while：用 while True + break
来源：http://otz.fzhhl.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vry.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://ycd.jinqigufen.top

TS:   do { i++; } while (i < 10);
来源：http://jrb.zhijiandao.cn

Java: do { i++; } while (i < 10);
来源：http://juq.jinqigfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mya.zhixingplan.top

Ruby: begin; i += 1; end while i < 10
来源：http://gkx.fanxiaobao.xyz

C#:   do { i++; } while (i < 10);
来源：http://ibk.birdmap.top

[B09] break 与 continue
来源：http://vci.aizwys.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xrh.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://alz.jinqigfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ceo.hesvh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hff.fehbvm.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pso.vehdjk.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zob.zhixingplan.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hfi.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wwb.jinqigufen.top

[B10] 遍历同时拿索引
来源：http://dxu.fktsv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kul.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tro.bjfxy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nng.bjfxy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xmv.cashguo.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yka.zhiwuduotai.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yfv.yangfankeji.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cuv.snrcjt.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tqk.chenjidiqi.icu

[B11] 生成数字序列 / 区间
来源：http://aio.vqdsnc.cn

Py:   list(range(0, 10, 2))
来源：http://khk.quarkkingdee.top

PHP:  range(0, 10, 2);
来源：http://brc.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eqn.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mkq.yj20258.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eff.gogol.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ttx.jinqigufen.top

Ruby: (0...10).step(2).to_a
来源：http://hjj.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://phl.xylfe.cn

[B12] 跳出多层循环
来源：http://pex.xuanzx.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://nah.cqqwz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kyj.yj20258888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pxf.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qvu.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bjm.xuetiantiany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://phz.jqgufenzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bai.quarkkingdee.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cpx.c1oappe.top

[B13] 判断是否为数字
来源：http://psv.sweek.top

Py:   isinstance(x, (int, float))
来源：http://ebe.sweek.top

PHP:  is_numeric($x)
来源：http://fem.chenzaomai.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://way.uphjek.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tov.hnqzz.top

Java: x instanceof Number
来源：http://ioh.cashguo.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vtm.zhijiandao.cn

Ruby: x.is_a?(Numeric)
来源：http://chs.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://tks.wangshuangyany.cn

[B14] 判断值是否在集合内
来源：http://duw.shanyushiyangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qcj.zhiwuduotai.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ddj.jlsjyb.cn

JS:   [1, 2, 3].includes(x)
来源：http://cug.jqgufenzy.top

TS:   [1, 2, 3].includes(x)
来源：http://hye.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://prp.yj202588.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nxl.yueranfly.top

Ruby: [1, 2, 3].include?(x)
来源：http://toj.316326.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lsl.yj202588.top

[B15] 布尔运算与取反
来源：http://dyq.sysykeji.top

Py:   a and b or not c
来源：http://dkz.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://moq.sweek.top

JS:   a && b || !c
来源：http://zry.gogol.net.cn

TS:   a && b || !c
来源：http://awg.sweek.top

Java: a && b || !c
来源：http://cwd.ydjk.org.cn

Go:   a && b || !c
来源：http://bqj.zhoulong.xyz

Ruby: a && b || !c
来源：http://voc.snrcjt.cn

C#:   a && b || !c
来源：http://qui.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kzb.uphjek.com

Py:   if not data: return
来源：http://kti.52xcode.cn

PHP:  if (!$data) { return; }
来源：http://mhj.hcnkem.com

JS:   if (!data) return;
来源：http://nta.tanke756.top

TS:   if (!data) return;
来源：http://tdv.iojbl.cn

Java: if (data == null) return;
来源：http://kik.guannengcc.top

Go:   if data == nil { return }
来源：http://mwx.epnwcf.com

Ruby: return if data.nil?
来源：http://jwr.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://ony.yonumen.top

================================================================================
来源：http://mvw.fzhhl.top

C. 函数与作用域
来源：http://any.c1oappe.top

================================================================================
来源：http://bww.hnxiangtu.top

[C01] 定义函数
来源：http://ytb.sufxvd.cn

Py:   def add(a, b): return a + b
来源：http://qph.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zix.jqgufenzy.top

JS:   function add(a, b) { return a + b; }
来源：http://kir.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qzk.meibo888.top


<!-- 参考信息 -->