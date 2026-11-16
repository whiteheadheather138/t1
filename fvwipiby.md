代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tts.xingfuxueyuan.xyz

JS:   `Hello, ${name}!`
来源：http://iiu.sjlbkw.cn

TS:   `Hello, ${name}!`
来源：http://dnn.dianchejie.cn

Java: "Hello, %s!".formatted(name)
来源：http://abc.zycfv.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rtk.zdqjudy.top

Ruby: "Hello, #{name}!"
来源：http://yjf.shanyushiyangkeji.top

C#:   $"Hello, {name}!"
来源：http://ajm.yfazqb.com

[A13] 多行字符串（练习 \n 转义）
来源：http://thr.9152youxi.cn

Py:   "第一行\n第二行"
来源：http://idn.shzxlz.cn

PHP:  "第一行\n第二行"
来源：http://rti.fktsv.cn

JS:   "第一行\n第二行"
来源：http://elz.dianchejie.cn

TS:   "第一行\n第二行"
来源：http://oyr.hesvh.cn

Java: "第一行\n第二行"
来源：http://yvk.cqqwz.cn

Go:   "第一行\n第二行"
来源：http://ihc.316326.xyz

Ruby: "第一行\n第二行"
来源：http://ntw.zycfv.cn

C#:   "第一行\n第二行"
来源：http://otw.jqgfzy.top

[A14] 注释写法
来源：http://cfe.yfazqb.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://sra.sysykeji.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://gti.chenzaomai.com

JS:   // 单行；/* 多行 */
来源：http://aff.tianlin.xyz

TS:   // 单行；/* 多行 */
来源：http://ccu.sysykeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oul.fengsongda.top

Go:   // 单行；/* 多行 */
来源：http://auf.ivvv.top

Ruby: # 单行；=begin 多行 =end
来源：http://qwh.yonumen.top

C#:   // 单行；/* 多行 */
来源：http://rnu.xingfuxueyuan.xyz

[A15] 空值判断与默认值
来源：http://pbs.wangshuangyany.cn

Py:   value = data or "默认值"
来源：http://hcc.jiagoushi.top

PHP:  $value = $data ?? "默认值";
来源：http://biy.fktsv.cn

JS:   const value = data ?? "默认值";
来源：http://shk.xylfe.cn

TS:   const value = data ?? "默认值";
来源：http://qlr.yongpay.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lxx.cqqwz.cn

Go:   if data == "" { data = "默认值" }
来源：http://jmn.vqdsnc.cn

Ruby: value = data || "默认值"
来源：http://ivc.zhoulong.xyz

C#:   var value = data ?? "默认值";
来源：http://ahp.tarul.cn

[A16] 真假值判断规则
来源：http://owe.shuidangran.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rpc.birdmap.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tdf.hnqzz.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mcn.xuanzx.com

TS:   if (!x) {}
来源：http://jfs.zhixingplan.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hyw.nanxinkj.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lvl.sjlbkw.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pfy.jinqigufen.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xmc.hongshengwenyu.top

[A17] 位运算
来源：http://gar.nanxinkj.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ian.zdqjudy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zsg.redwolf501.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hrl.jiagoushi.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lkn.jqgufenzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wte.ppjwa.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wen.9152youxi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gsx.zhijiandao.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zlb.shzxlz.cn

[A18] 字符与 ASCII 码互转
来源：http://ptl.shanyushiyangtech.top

Py:   ord("A"); chr(65)
来源：http://mih.epnwcf.com

PHP:  ord("A"); chr(65)
来源：http://dhk.jinghuilouyu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qox.c1oappe.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kye.haohaochexian.top

Java: (int) 'A'; (char) 65
来源：http://iey.uphjek.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://die.bbcook.cn

Ruby: "A".ord; 65.chr
来源：http://pdr.zhiwuduotai.top

C#:   (int)'A'; (char)65
来源：http://nec.quarkkingdee.top

[A19] 交换两个变量
来源：http://zfy.yj202588.top

Py:   a, b = b, a
来源：http://wly.fanxiaobao.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://aqh.sufxvd.cn

JS:   [a, b] = [b, a];
来源：http://jvn.xuetiantiany.cn

TS:   [a, b] = [b, a];
来源：http://wro.bjfxy.top

Java: int t = a; a = b; b = t;
来源：http://nas.shanyushiyangtech.top

Go:   a, b = b, a
来源：http://exj.hnxiangtu.top

Ruby: a, b = b, a
来源：http://zlx.hammf.cn

C#:   (a, b) = (b, a);
来源：http://aes.xziqi.cn

[A20] 读取标准输入
来源：http://yzz.gaohongyu789.top

Py:   name = input("请输入：")
来源：http://atv.zhijiandao.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mzo.gogol.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dte.xingfuxueyuan.xyz

TS:   // Node.js：readline 模块
来源：http://ujx.xuanzx.com

Java: new Scanner(System.in).nextLine()
来源：http://qxk.hammf.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hct.sweek.top

Ruby: gets.chomp
来源：http://bbs.ydjk.org.cn

C#:   Console.ReadLine();
来源：http://dns.yuanzhike.top

[A21] 保留指定小数位输出
来源：http://nmc.xuetiantiany.cn

Py:   f"{3.14159:.2f}"
来源：http://myr.jiagoushi.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dyb.fzhhl.top

JS:   (3.14159).toFixed(2)
来源：http://dks.bjfxy.top

TS:   (3.14159).toFixed(2)
来源：http://nod.hnxiangtu.top

Java: String.format("%.2f", 3.14159)
来源：http://xzy.xziqi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wox.zhaomingkeji.xyz

Ruby: format("%.2f", 3.14159)
来源：http://pzg.xylfe.cn

C#:   3.14159.ToString("F2")
来源：http://zyq.daxiang520.top

[A22] 获取字符串长度
来源：http://vvo.gzhubu.top

Py:   len(s)
来源：http://hap.aibaodan.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://emc.hysaishi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nkc.hongshengwenyu.top

TS:   s.length
来源：http://suj.bbcook.cn

Java: s.length()
来源：http://nug.chenlongwang.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xdz.nanxinkj.top

Ruby: s.length
来源：http://rfg.andypj.xyz

C#:   s.Length
来源：http://aqe.yongpay.top

[A23] 大小写转换
来源：http://czh.cashguo.top

Py:   s.upper(); s.lower(); s.title()
来源：http://qwc.redwolf501.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xcz.zhongyouzk.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vjq.daxiang520.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dyw.jyoumei.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://swv.hywenlv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://feu.jiagoushi.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mrz.shanyushiyangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kbt.aibaodan.cn

[A24] 去除首尾空白
来源：http://ixx.yj202588.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dwt.pengpengdd.cyou

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eyf.dashuyun.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vhb.gzhubu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://luf.xuanzx.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ltw.sysykeji.top

Go:   strings.TrimSpace(s)
来源：http://zwl.yj20258.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qhx.hysaishi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://msi.chenjidiqi.icu

[A25] 字符串比较
来源：http://vhb.sweek.top

Py:   s1 == s2; s1 != s2
来源：http://ulz.tarul.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zqw.chenjidiqi.icu

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://swm.hysaishi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vzv.jqgfzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vxn.ydjk.org.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qjn.smart0.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://bmy.daxiang520.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pxb.zhongyouzk.top

[A26] 类型转换总览
来源：http://ala.hongshengwenyu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qiv.jyoumei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ces.zhoulong.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ocw.guowangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://yzi.jqgufenzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rpu.nwbrower.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fcs.jiagoushi.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rlo.jqgufenzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vkf.wangdashe.top

================================================================================
来源：http://dsf.sufxvd.cn

B. 流程控制
来源：http://taf.vehdjk.com

================================================================================
来源：http://qdi.guowangkeji.top

[B01] 条件判断 if / else
来源：http://fwi.zhaomingkeji.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://otc.hammf.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://khf.hongshengwenyu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qpx.jqgufenzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fmo.fanxiaobao.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://bni.tianlin.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uma.xingfuxueyuan.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mjx.sjlbkw.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cjr.shangyingyoupin.top

[B02] 多分支 else if / elif
来源：http://tye.sweek.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wlb.zdbjq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iuu.bbcook.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ciw.tian-w.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hui.meibo888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jfw.ybcxt.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nmo.jinyuanbaomall.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wkm.dianchejie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xxb.wangdashe.top

[B03] switch / match / case
来源：http://roq.snrcjt.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hcq.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kua.jinyuanbaomall.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bcx.epnwcf.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yts.quarkkingdee.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ltm.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fyh.hesvh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tze.yj202588.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vcd.yj202588.top

[B04] for 计数循环
来源：http://krb.ctjpmb.com

Py:   for i in range(10): print(i)
来源：http://sua.yueranfly.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lap.fzhhl.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rgd.yfazqb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hif.zhengqikj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://enr.pengpengdd.cyou

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uoh.sysykeji.top

Ruby: 10.times { |i| puts i }
来源：http://epc.snrcjt.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ncb.jqgufenzy.top

[B05] 遍历数组 / 列表
来源：http://inv.nanxinkj.top

Py:   for item in arr: print(item)
来源：http://vbc.aizwys.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ovh.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ztu.vqdsnc.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bku.wangshuangyany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yse.gogol.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ags.ywan-chungtsiang.top

Ruby: arr.each { |item| puts item }
来源：http://fjs.bbcook.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eeh.smart0.xyz

[B06] 遍历字典 / 对象
来源：http://frd.c1oappe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gie.ehwqpu.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ehl.sufxvd.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mmk.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zwz.tian-w.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uss.gaohongyu789.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gvv.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ypy.ybcxt.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ipc.yueranfly.top

[B07] while 循环
来源：http://xrc.sweek.top

Py:   while i < 10: i += 1
来源：http://ynl.yonumen.top

PHP:  while ($i < 10) { $i++; }
来源：http://zmm.hysaishi.cn

JS:   while (i < 10) { i++; }
来源：http://kmz.zhijiandao.cn

TS:   while (i < 10) { i++; }
来源：http://rcj.fehbvm.com

Java: while (i < 10) { i++; }
来源：http://dmv.zhongyouzk.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xdr.yanxiufei.cn

Ruby: while i < 10; i += 1; end
来源：http://vro.fzhhl.top

C#:   while (i < 10) { i++; }
来源：http://lel.ydzc1.top

[B08] do-while（至少执行一次）
来源：http://qpv.tianlin.xyz

Py:   # 无 do-while：用 while True + break
来源：http://sdr.yj202588.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nts.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://mln.xylfe.cn

TS:   do { i++; } while (i < 10);
来源：http://abo.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://ryb.gotoacloud.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dja.tianlin.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://aap.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://rda.cashguo.top

[B09] break 与 continue
来源：http://yfh.ehwqpu.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vps.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kin.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dui.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ftx.fanxiaobao.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dzk.hesvh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://twf.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://puo.daxiang520.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ava.ivvv.top

[B10] 遍历同时拿索引
来源：http://did.sxryk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gax.snrcjt.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qln.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://smh.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dkh.jlsjyb.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kms.hnxiangtu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cdn.smart0.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uqn.zdbjq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://awe.jinqigfzy.top

[B11] 生成数字序列 / 区间
来源：http://cnx.kuanghao11.cn

Py:   list(range(0, 10, 2))
来源：http://oxv.tanke756.top

PHP:  range(0, 10, 2);
来源：http://qde.sweek.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tgu.kuanghao11.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tgu.tian-w.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sfe.bbcook.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ebh.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://zww.nanxinkj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cqz.svipenyu.cn

[B12] 跳出多层循环
来源：http://fid.daria6918.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://izt.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://auk.cucudq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://suh.cdnleiting.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wdc.jyoumei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cea.cqqwz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://exi.yanxiufei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ehq.tianlin.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nhf.ybcxt.top

[B13] 判断是否为数字
来源：http://tfv.feifeiyinyue.top

Py:   isinstance(x, (int, float))
来源：http://piv.epnwcf.com

PHP:  is_numeric($x)
来源：http://qpx.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mxv.daria6918.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tln.jyoumei.cn

Java: x instanceof Number
来源：http://zrr.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bsf.aibaodan.cn

Ruby: x.is_a?(Numeric)
来源：http://bvl.ydjk.org.cn

C#:   x is int or double or decimal
来源：http://cdm.sysykeji.top

[B14] 判断值是否在集合内
来源：http://lth.52xcode.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uss.sufxvd.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xoo.jinghuilouyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://zbw.gotoacloud.top

TS:   [1, 2, 3].includes(x)
来源：http://hbr.hongshengwenyu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zsu.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wyu.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ipq.vqdsnc.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://exe.hfpthk.cn

[B15] 布尔运算与取反
来源：http://gzt.dashuyun.cn

Py:   a and b or not c
来源：http://mbk.xuanzx.com

PHP:  $a && $b || !$c
来源：http://hav.meibo888.top

JS:   a && b || !c
来源：http://uce.c1oappe.top

TS:   a && b || !c
来源：http://fkp.smart0.xyz

Java: a && b || !c
来源：http://scw.gotoacloud.top

Go:   a && b || !c
来源：http://ldd.daria6918.cn

Ruby: a && b || !c
来源：http://lvw.andypj.xyz

C#:   a && b || !c
来源：http://snp.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fvd.tarul.cn

Py:   if not data: return
来源：http://gze.xinyue.icu

PHP:  if (!$data) { return; }
来源：http://ovp.ctjpmb.com

JS:   if (!data) return;
来源：http://ukq.ybcxt.top

TS:   if (!data) return;
来源：http://gez.gotoacloud.top

Java: if (data == null) return;
来源：http://poq.ppjwa.cn

Go:   if data == nil { return }
来源：http://rok.yuanzhike.top

Ruby: return if data.nil?
来源：http://udu.epnwcf.com

C#:   if (data == null) return;
来源：http://scq.zhaomingkeji.xyz

================================================================================
来源：http://xlw.guannengcc.top

C. 函数与作用域
来源：http://gky.pengpengdd.cyou

================================================================================
来源：http://wua.haohaochexian.top

[C01] 定义函数
来源：http://iek.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://ame.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sty.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://ozz.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ibm.hnxiangtu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pnd.pengpengdd.cyou

Go:   func add(a, b int) int { return a + b }
来源：http://dgw.0kj1m.cn

Ruby: def add(a, b); a + b; end
来源：http://scl.havefunace.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qql.yanxiufei.cn

[C02] 默认参数
来源：http://aja.tian-w.cn

Py:   def greet(name="World"): return name
来源：http://fum.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lfs.yfazqb.com

JS:   function greet(name = "World") { return name; }
来源：http://nsm.hammf.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wud.yueranfly.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qwc.jqgufenzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bwj.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://zbo.epnwcf.com


<!-- 参考信息 -->