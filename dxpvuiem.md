代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://sqb.9152youxi.cn

[A11] 条件表达式（三元）
来源：http://kmq.xziqi.cn

Py:   "yes" if x > 0 else "no"
来源：http://mjg.feifeiyinyue.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nyg.andypj.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://dnp.wangshuangyany.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ked.pengpengdd.cyou

Java: x > 0 ? "yes" : "no"
来源：http://pgp.guannengcc.top

Go:   // 无三元运算符，需用 if 语句
来源：http://rhm.hywenlv.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zuh.hfpthk.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yut.yuxming.cn

[A12] 字符串插值 / 格式化
来源：http://skn.jinghuilouyu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yug.yuanzhike.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rdv.smart0.xyz

JS:   `Hello, ${name}!`
来源：http://cym.jinqigfzy.top

TS:   `Hello, ${name}!`
来源：http://rbi.zycfv.cn

Java: "Hello, %s!".formatted(name)
来源：http://tir.vqdsnc.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vkn.hysaishi.cn

Ruby: "Hello, #{name}!"
来源：http://sxm.chenzaomai.com

C#:   $"Hello, {name}!"
来源：http://yot.zhongyouzk.top

[A13] 多行字符串（练习 \n 转义）
来源：http://kfl.52xcode.cn

Py:   "第一行\n第二行"
来源：http://jdv.316326.xyz

PHP:  "第一行\n第二行"
来源：http://gba.redwolf501.top

JS:   "第一行\n第二行"
来源：http://zrk.shangyingyoupin.top

TS:   "第一行\n第二行"
来源：http://wgp.ppjwa.cn

Java: "第一行\n第二行"
来源：http://pgw.dashuyun.cn

Go:   "第一行\n第二行"
来源：http://yqa.yuxming.cn

Ruby: "第一行\n第二行"
来源：http://nxw.0kj1m.cn

C#:   "第一行\n第二行"
来源：http://fdn.redwolf501.top

[A14] 注释写法
来源：http://lpd.ivvv.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ond.hammf.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rbq.ybcxt.top

JS:   // 单行；/* 多行 */
来源：http://mvf.sxryk.cn

TS:   // 单行；/* 多行 */
来源：http://ozx.uphjek.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dtm.shuidangran.top

Go:   // 单行；/* 多行 */
来源：http://jrp.aizwys.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gmx.hongshengwenyu.top

C#:   // 单行；/* 多行 */
来源：http://lko.316326.xyz

[A15] 空值判断与默认值
来源：http://ufp.yuxming.cn

Py:   value = data or "默认值"
来源：http://jic.yj202588.top

PHP:  $value = $data ?? "默认值";
来源：http://nka.ehwqpu.com

JS:   const value = data ?? "默认值";
来源：http://foz.fzhhl.top

TS:   const value = data ?? "默认值";
来源：http://xxf.xinyue.icu

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hbw.gotoacloud.top

Go:   if data == "" { data = "默认值" }
来源：http://ndk.zhoulong.xyz

Ruby: value = data || "默认值"
来源：http://tyu.xylfe.cn

C#:   var value = data ?? "默认值";
来源：http://xye.ctjpmb.com

[A16] 真假值判断规则
来源：http://fmp.c1oappe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zpe.quarkkingdee.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mkm.jinqigufen.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tfl.uphjek.com

TS:   if (!x) {}
来源：http://gqp.fktsv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qcy.fanxiaobao.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lbz.fanxiaobao.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://xmg.gogol.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hbw.kuanghao11.cn

[A17] 位运算
来源：http://eeg.xinyue.icu

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yss.sjlbkw.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zav.316326.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://slb.ybcxt.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://woh.sufxvd.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dui.zhiwuduotai.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://alz.shuidangran.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ykx.chenzaomai.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cnw.zhijiandao.cn

[A18] 字符与 ASCII 码互转
来源：http://znl.shanyushiyangtech.top

Py:   ord("A"); chr(65)
来源：http://tqi.xuanzx.com

PHP:  ord("A"); chr(65)
来源：http://qpc.xingfuxueyuan.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://csm.zhiwuduotai.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hbh.yuanzhike.top

Java: (int) 'A'; (char) 65
来源：http://ogc.jinyuanbaomall.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zfl.zhaomingkeji.xyz

Ruby: "A".ord; 65.chr
来源：http://hvs.52xcode.cn

C#:   (int)'A'; (char)65
来源：http://olv.hongshengwenyu.top

[A19] 交换两个变量
来源：http://xcs.zhiwuduotai.top

Py:   a, b = b, a
来源：http://zvf.mhx1999.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jms.hfpthk.cn

JS:   [a, b] = [b, a];
来源：http://mox.gotoacloud.top

TS:   [a, b] = [b, a];
来源：http://zkw.nanxinkj.top

Java: int t = a; a = b; b = t;
来源：http://nmu.yangfankeji.com

Go:   a, b = b, a
来源：http://wux.xingfuxueyuan.xyz

Ruby: a, b = b, a
来源：http://dib.yueranfly.top

C#:   (a, b) = (b, a);
来源：http://kiy.cucudq.cn

[A20] 读取标准输入
来源：http://tcy.yongpay.top

Py:   name = input("请输入：")
来源：http://adl.xziqi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dvg.hfpthk.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nbq.redwolf501.top

TS:   // Node.js：readline 模块
来源：http://mhk.chenlongwang.top

Java: new Scanner(System.in).nextLine()
来源：http://aiq.yfazqb.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ekk.zhiwuduotai.top

Ruby: gets.chomp
来源：http://ykw.fzhhl.top

C#:   Console.ReadLine();
来源：http://iax.ywan-chungtsiang.top

[A21] 保留指定小数位输出
来源：http://aaf.hammf.cn

Py:   f"{3.14159:.2f}"
来源：http://brf.gzhubu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rki.shanyushiyangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://cys.xingfuxueyuan.xyz

TS:   (3.14159).toFixed(2)
来源：http://kcb.mhx1999.top

Java: String.format("%.2f", 3.14159)
来源：http://twk.gogol.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rws.yueranfly.top

Ruby: format("%.2f", 3.14159)
来源：http://rpl.tian-w.cn

C#:   3.14159.ToString("F2")
来源：http://kxw.zhengqikj.top

[A22] 获取字符串长度
来源：http://dwy.daxiang520.top

Py:   len(s)
来源：http://yzk.gotoacloud.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qul.zhiwuduotai.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://foe.zhiwuduotai.top

TS:   s.length
来源：http://bwf.birdmap.top

Java: s.length()
来源：http://bvd.nwbrower.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uun.wangshuangyany.cn

Ruby: s.length
来源：http://hoo.vqdsnc.cn

C#:   s.Length
来源：http://rdh.havefunace.top

[A23] 大小写转换
来源：http://jug.hnqzz.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xwh.jinyuanbaomall.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cin.sxryk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://smr.redwolf501.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mko.chenjidiqi.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bmi.hfpthk.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qyr.sysykeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gqw.yongpay.top

C#:   s.ToUpper(); s.ToLower()
来源：http://maa.ctjpmb.com

[A24] 去除首尾空白
来源：http://sgt.jinqigfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cma.jianghu66.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vfo.jqgfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kop.bjfxy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vnm.daria6918.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ppk.nwbrower.top

Go:   strings.TrimSpace(s)
来源：http://zrv.shuidangran.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xfb.guannengcc.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mio.hongshengwenyu.top

[A25] 字符串比较
来源：http://utj.aizwys.cn

Py:   s1 == s2; s1 != s2
来源：http://nvc.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eyw.pycfn.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zat.zhijiandao.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hmv.fktsv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lmm.zdqjudy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mgw.snrcjt.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zfm.xylfe.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jfq.sysykeji.top

[A26] 类型转换总览
来源：http://fog.bjfxy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ebd.yanxiufei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ciy.zhijiandao.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ywu.mhx1999.top

TS:   Number() String() Boolean() x as number
来源：http://yxo.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gau.chenzaomai.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zfy.zdqjudy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rtv.sweek.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pre.shanyushiyangkeji.top

================================================================================
来源：http://oif.zhengqikj.top

B. 流程控制
来源：http://dty.9152youxi.cn

================================================================================
来源：http://fnb.ybcxt.top

[B01] 条件判断 if / else
来源：http://met.zhoulong.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://fsh.hfpthk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://owp.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uly.daria6918.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xza.hnqzz.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vaz.zhixingplan.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tpz.9152youxi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vqt.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dap.svipenyu.cn

[B02] 多分支 else if / elif
来源：http://bjf.ctjpmb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kmq.cheryme.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xly.yangfankeji.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rme.xingfuxueyuan.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://npa.zycfv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rmo.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jde.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://esj.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wxd.xylfe.cn

[B03] switch / match / case
来源：http://dvt.sxryk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://igr.316326.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nqz.jqgufenzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tyr.daxiang520.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tid.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ezg.kuanghao11.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ckj.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uwb.xuetiantiany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://shx.shuidangran.top

[B04] for 计数循环
来源：http://gyl.zdbjq.cn

Py:   for i in range(10): print(i)
来源：http://mgd.jinyuanbaomall.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bmo.aibaodan.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qxi.shangyingyoupin.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://juq.yongpay.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gsc.yfazqb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xxw.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://lyq.sysykeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fao.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://vet.bjfxy.top

Py:   for item in arr: print(item)
来源：http://xfl.kuanghao11.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://onn.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mik.uphjek.com

TS:   for (const item of arr) { console.log(item); }
来源：http://hax.xinyue.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://oiv.svipenyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mwv.gzhubu.top

Ruby: arr.each { |item| puts item }
来源：http://xxb.ppjwa.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bpc.xziqi.cn

[B06] 遍历字典 / 对象
来源：http://xev.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fwp.ivvv.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yjy.jinyuanbaomall.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hqe.sweek.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dao.yj202588.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xxx.yueranfly.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bdx.tanke756.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://anz.birdmap.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ggo.smart0.xyz

[B07] while 循环
来源：http://hng.ydzc1.top

Py:   while i < 10: i += 1
来源：http://iip.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xde.uphjek.com

JS:   while (i < 10) { i++; }
来源：http://uqz.gotoacloud.top

TS:   while (i < 10) { i++; }
来源：http://vic.dianchejie.cn

Java: while (i < 10) { i++; }
来源：http://ebb.chenjidiqi.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hll.vqdsnc.cn

Ruby: while i < 10; i += 1; end
来源：http://yqn.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://jze.fengsongda.top

[B08] do-while（至少执行一次）
来源：http://jji.aizwys.cn

Py:   # 无 do-while：用 while True + break
来源：http://rcs.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://lij.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://tjz.yfazqb.com

TS:   do { i++; } while (i < 10);
来源：http://eee.zhixingplan.top

Java: do { i++; } while (i < 10);
来源：http://hbn.shanyushiyangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lly.cdnleiting.top

Ruby: begin; i += 1; end while i < 10
来源：http://yoe.sufxvd.cn

C#:   do { i++; } while (i < 10);
来源：http://qje.xingfuxueyuan.xyz

[B09] break 与 continue
来源：http://wmi.chenjidiqi.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sxu.yanxiufei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://okm.bbcook.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ehn.haohaochexian.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zfz.wangdashe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://teh.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://epv.sysykeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bdb.xylfe.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dgj.sysykeji.top

[B10] 遍历同时拿索引
来源：http://uhe.wangdashe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vok.sysykeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uom.vqdsnc.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ujm.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iyi.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://azs.xuetiantiany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qql.yj202588.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qph.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qjo.hywenlv.cn

[B11] 生成数字序列 / 区间
来源：http://scy.sxryk.cn

Py:   list(range(0, 10, 2))
来源：http://qqr.hongshengwenyu.top

PHP:  range(0, 10, 2);
来源：http://avk.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ceh.mhx1999.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pqv.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://spv.tanke756.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ydi.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://flc.yangfankeji.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sko.yangfankeji.com

[B12] 跳出多层循环
来源：http://pwd.ybcxt.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tkp.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://prh.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rsr.shzxlz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rzo.mhx1999.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qng.ppjwa.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lec.jinghuilouyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mfn.daxiang520.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wew.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://vdv.epnwcf.com

Py:   isinstance(x, (int, float))
来源：http://gjm.uphjek.com

PHP:  is_numeric($x)
来源：http://joe.andypj.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://idf.ctjpmb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iys.fehbvm.com

Java: x instanceof Number
来源：http://wez.bjfxy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jzp.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://oyj.ppjwa.cn

C#:   x is int or double or decimal
来源：http://ege.cdnleiting.top

[B14] 判断值是否在集合内
来源：http://pul.cqqwz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kee.chenzaomai.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xzz.hcnkem.com

JS:   [1, 2, 3].includes(x)
来源：http://bkk.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://atx.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://blt.daxiang520.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pri.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://tur.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cti.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://uxe.yonumen.top

Py:   a and b or not c
来源：http://owb.fktsv.cn

PHP:  $a && $b || !$c
来源：http://coz.sxryk.cn

JS:   a && b || !c
来源：http://rfi.ybcxt.top

TS:   a && b || !c
来源：http://kzc.hnqzz.top

Java: a && b || !c
来源：http://gok.sweek.top

Go:   a && b || !c
来源：http://hqm.yj202588.top

Ruby: a && b || !c
来源：http://ics.cashguo.top

C#:   a && b || !c
来源：http://ezh.vehdjk.com

[B16] 卫语句：不满足条件提前返回
来源：http://lit.sjlbkw.cn

Py:   if not data: return
来源：http://kew.fengsongda.top

PHP:  if (!$data) { return; }
来源：http://esf.sysykeji.top

JS:   if (!data) return;
来源：http://tps.tarul.cn

TS:   if (!data) return;
来源：http://dkr.yuxming.cn

Java: if (data == null) return;
来源：http://ifs.yueranfly.top

Go:   if data == nil { return }
来源：http://xsg.uphjek.com

Ruby: return if data.nil?
来源：http://nkw.yongpay.top

C#:   if (data == null) return;
来源：http://fxk.yuanzhike.top

================================================================================
来源：http://irj.jinqigfzy.top

C. 函数与作用域
来源：http://nft.jianghu66.top

================================================================================
来源：http://dhc.jqgfzy.top

[C01] 定义函数
来源：http://tlq.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://wsc.dianchejie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gtt.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ogt.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uuk.jiagoushi.top


<!-- 参考信息 -->