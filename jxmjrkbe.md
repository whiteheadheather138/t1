代发 wailian999

Py:   "第一行\n第二行"
来源：http://aam.hcnkem.com

PHP:  "第一行\n第二行"
来源：http://sah.yj20258888.top

JS:   "第一行\n第二行"
来源：http://qpx.hammf.cn

TS:   "第一行\n第二行"
来源：http://wlw.daxiang520.top

Java: "第一行\n第二行"
来源：http://rwr.sufxvd.cn

Go:   "第一行\n第二行"
来源：http://tub.xylfe.cn

Ruby: "第一行\n第二行"
来源：http://xit.zhijiandao.cn

C#:   "第一行\n第二行"
来源：http://yib.vqdsnc.cn

[A14] 注释写法
来源：http://stq.shanyushiyangkeji.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://lmg.jqgufenzy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://muh.redwolf501.top

JS:   // 单行；/* 多行 */
来源：http://lto.yuanzhike.top

TS:   // 单行；/* 多行 */
来源：http://hwp.nanxuanxn.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yim.bjfxy.top

Go:   // 单行；/* 多行 */
来源：http://lre.9152youxi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jcq.gogol.net.cn

C#:   // 单行；/* 多行 */
来源：http://jwn.tarul.cn

[A15] 空值判断与默认值
来源：http://zai.shanyushiyangkeji.top

Py:   value = data or "默认值"
来源：http://jwv.zhixingplan.top

PHP:  $value = $data ?? "默认值";
来源：http://dpc.xziqi.cn

JS:   const value = data ?? "默认值";
来源：http://kin.shanyushiyangtech.top

TS:   const value = data ?? "默认值";
来源：http://irh.c1oappe.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kvs.pycfn.com

Go:   if data == "" { data = "默认值" }
来源：http://wyr.aibaodan.cn

Ruby: value = data || "默认值"
来源：http://xlh.tanke756.top

C#:   var value = data ?? "默认值";
来源：http://rec.jinqigufen.top

[A16] 真假值判断规则
来源：http://cpg.fanxiaobao.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gez.fktsv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yfw.vehdjk.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pnw.daria6918.cn

TS:   if (!x) {}
来源：http://sos.kuanghao11.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fnc.tianlin.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mpx.yuxming.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lpl.bjfxy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wby.chenlongwang.top

[A17] 位运算
来源：http://jgb.ctjpmb.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fjd.aizwys.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tyf.iojbl.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://isx.jianghu66.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ffv.yonumen.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aad.zhaomingkeji.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://eox.shanyushiyangtech.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qkk.fktsv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://amq.tian-w.cn

[A18] 字符与 ASCII 码互转
来源：http://rog.jqgufenzy.top

Py:   ord("A"); chr(65)
来源：http://ygd.yangfankeji.com

PHP:  ord("A"); chr(65)
来源：http://oop.316326.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vkx.daria6918.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xtn.hysaishi.cn

Java: (int) 'A'; (char) 65
来源：http://okq.sxryk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nic.ydjk.org.cn

Ruby: "A".ord; 65.chr
来源：http://ktx.yangfankeji.com

C#:   (int)'A'; (char)65
来源：http://nnz.jlsjyb.cn

[A19] 交换两个变量
来源：http://jic.bbcook.cn

Py:   a, b = b, a
来源：http://xuo.chenlongwang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ewh.zhijiandao.cn

JS:   [a, b] = [b, a];
来源：http://iiz.shanyushiyangkeji.top

TS:   [a, b] = [b, a];
来源：http://uga.hfpthk.cn

Java: int t = a; a = b; b = t;
来源：http://aey.zdqjudy.top

Go:   a, b = b, a
来源：http://uzx.nwbrower.top

Ruby: a, b = b, a
来源：http://ojg.316326.xyz

C#:   (a, b) = (b, a);
来源：http://pbk.chenjidiqi.icu

[A20] 读取标准输入
来源：http://ezv.daria6918.cn

Py:   name = input("请输入：")
来源：http://yaj.sufxvd.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ggg.iojbl.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://npe.jqgufenzy.top

TS:   // Node.js：readline 模块
来源：http://wya.daria6918.cn

Java: new Scanner(System.in).nextLine()
来源：http://gzu.jqgufenzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mmf.tian-w.cn

Ruby: gets.chomp
来源：http://bbt.fzhhl.top

C#:   Console.ReadLine();
来源：http://xvb.yueranfly.top

[A21] 保留指定小数位输出
来源：http://rwb.ctjpmb.com

Py:   f"{3.14159:.2f}"
来源：http://dzh.yongpay.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pxw.tianlin.xyz

JS:   (3.14159).toFixed(2)
来源：http://zfg.jqgufenzy.top

TS:   (3.14159).toFixed(2)
来源：http://kme.gogol.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://ihq.ctjpmb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ive.iojbl.cn

Ruby: format("%.2f", 3.14159)
来源：http://vwq.hysaishi.cn

C#:   3.14159.ToString("F2")
来源：http://oxg.shzxlz.cn

[A22] 获取字符串长度
来源：http://cmv.yueranfly.top

Py:   len(s)
来源：http://xgz.aibaodan.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bxn.zdbjq.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wmp.zhijiandao.cn

TS:   s.length
来源：http://xsa.tarul.cn

Java: s.length()
来源：http://sbr.xylfe.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dny.tarul.cn

Ruby: s.length
来源：http://muv.daria6918.cn

C#:   s.Length
来源：http://kws.ehwqpu.com

[A23] 大小写转换
来源：http://mnb.redwolf501.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ckr.gaohongyu789.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://arf.xingfuxueyuan.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hrl.jianghu66.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qdk.yongpay.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://woj.zycfv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dec.aizwys.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://beq.zhoulong.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://kcd.havefunace.top

[A24] 去除首尾空白
来源：http://wpl.nanxinkj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blj.nanxinkj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vcc.hongshengwenyu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://elv.dashuyun.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zbk.c1oappe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kjk.jyoumei.cn

Go:   strings.TrimSpace(s)
来源：http://iuj.jinghuilouyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qmy.jinghuilouyu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rmu.yj20258.top

[A25] 字符串比较
来源：http://iux.chenlongwang.top

Py:   s1 == s2; s1 != s2
来源：http://vwf.zhoulong.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qgv.aibaodan.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pgr.zhixingplan.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mmd.mhx1999.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wro.redwolf501.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jru.dianchejie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://idp.dianchejie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iqb.hywenlv.cn

[A26] 类型转换总览
来源：http://few.xylfe.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mwm.cashguo.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eem.chenlongwang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cse.zhijiandao.cn

TS:   Number() String() Boolean() x as number
来源：http://hqr.nanxuanxn.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jyn.zhixingplan.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://civ.gotoacloud.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dte.ctjpmb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hwj.vqdsnc.cn

================================================================================
来源：http://awl.zdbjq.cn

B. 流程控制
来源：http://mgh.haohaochexian.top

================================================================================
来源：http://com.snrcjt.cn

[B01] 条件判断 if / else
来源：http://wcs.gaohongyu789.top

Py:   result = "正" if x > 0 else "非正"
来源：http://kfx.meibo888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lzv.gogol.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nza.sjlbkw.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gtk.uphjek.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://bwj.nanxinkj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://asv.bbcook.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rqk.yonumen.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nem.ywan-chungtsiang.top

[B02] 多分支 else if / elif
来源：http://ggs.xylfe.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ifd.nanxuanxn.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qxu.svipenyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uki.uphjek.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tuc.yuanzhike.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jym.hesvh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xyg.hcnkem.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vtl.andypj.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yqz.vqdsnc.cn

[B03] switch / match / case
来源：http://lwi.jiagoushi.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qph.52xcode.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iqv.yongpay.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oap.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cdd.wangdashe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kcq.yongpay.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wel.tian-w.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bxk.quarkkingdee.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mzt.yongpay.top

[B04] for 计数循环
来源：http://hnb.cqqwz.cn

Py:   for i in range(10): print(i)
来源：http://ikv.jlsjyb.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ino.yonumen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nzj.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pma.tianlin.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cwj.shuidangran.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ckq.snrcjt.cn

Ruby: 10.times { |i| puts i }
来源：http://xmz.tanke756.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://quv.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://ywk.daria6918.cn

Py:   for item in arr: print(item)
来源：http://toc.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ckv.yangfankeji.com

JS:   for (const item of arr) { console.log(item); }
来源：http://agd.yj20258888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://oiw.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://zyi.fanxiaobao.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://obi.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://fdl.ehwqpu.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tvj.yuanzhike.top

[B06] 遍历字典 / 对象
来源：http://qsh.cdnleiting.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ktn.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dlb.jinyuanbaomall.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ktk.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bbu.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lxv.guannengcc.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sub.jinghuilouyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kbs.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ikr.quarkkingdee.top

[B07] while 循环
来源：http://sen.daxiang520.top

Py:   while i < 10: i += 1
来源：http://ecb.daxiang520.top

PHP:  while ($i < 10) { $i++; }
来源：http://orw.jqgfzy.top

JS:   while (i < 10) { i++; }
来源：http://pgp.bbcook.cn

TS:   while (i < 10) { i++; }
来源：http://kfe.fengsongda.top

Java: while (i < 10) { i++; }
来源：http://mwi.hysaishi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mja.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://yzz.xuanzx.com

C#:   while (i < 10) { i++; }
来源：http://ilv.jqgufenzy.top

[B08] do-while（至少执行一次）
来源：http://xts.yueranfly.top

Py:   # 无 do-while：用 while True + break
来源：http://tfe.uphjek.com

PHP:  do { $i++; } while ($i < 10);
来源：http://xeb.haohaochexian.top

JS:   do { i++; } while (i < 10);
来源：http://wfu.aibaodan.cn

TS:   do { i++; } while (i < 10);
来源：http://kvn.wangdashe.top

Java: do { i++; } while (i < 10);
来源：http://ufk.hesvh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ymm.hesvh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oji.52xcode.cn

C#:   do { i++; } while (i < 10);
来源：http://gce.xziqi.cn

[B09] break 与 continue
来源：http://bfp.haohaochexian.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://skh.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yxz.cdnleiting.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eww.hysaishi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rjm.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fik.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tsz.dianchejie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uhr.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sui.redwolf501.top

[B10] 遍历同时拿索引
来源：http://mkx.ctjpmb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ezi.snrcjt.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rpk.yuxming.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ryy.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vsq.aibaodan.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pkx.birdmap.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://khu.zycfv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sds.zhixingplan.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lln.jinqigfzy.top

[B11] 生成数字序列 / 区间
来源：http://aqa.fehbvm.com

Py:   list(range(0, 10, 2))
来源：http://ykv.bjfxy.top

PHP:  range(0, 10, 2);
来源：http://qob.pycfn.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rmc.sjlbkw.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rbz.cucudq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zak.tarul.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://akj.chenjidiqi.icu

Ruby: (0...10).step(2).to_a
来源：http://mrb.aizwys.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vfi.yongpay.top

[B12] 跳出多层循环
来源：http://xob.ctjpmb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://oqq.gogol.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kdu.bbcook.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://scq.nanxuanxn.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://knd.tian-w.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jsq.redwolf501.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jah.fzhhl.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sve.ydjk.org.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nwq.wangdashe.top

[B13] 判断是否为数字
来源：http://cxf.cdnleiting.top

Py:   isinstance(x, (int, float))
来源：http://xhx.haohaochexian.top

PHP:  is_numeric($x)
来源：http://sed.pengpengdd.cyou

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://swl.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kmf.haohaochexian.top

Java: x instanceof Number
来源：http://kcz.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mse.mhx1999.top

Ruby: x.is_a?(Numeric)
来源：http://zve.gotoacloud.top

C#:   x is int or double or decimal
来源：http://qmy.gzhubu.top

[B14] 判断值是否在集合内
来源：http://cgj.zdqjudy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tie.cucudq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qvi.zhixingplan.top

JS:   [1, 2, 3].includes(x)
来源：http://zfj.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://nvz.hnxiangtu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://avk.kuanghao11.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rni.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ran.andypj.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://icj.cdnleiting.top

[B15] 布尔运算与取反
来源：http://lbv.zhaomingkeji.xyz

Py:   a and b or not c
来源：http://auf.xingfuxueyuan.xyz

PHP:  $a && $b || !$c
来源：http://zwf.ehwqpu.com

JS:   a && b || !c
来源：http://wxv.ybcxt.top

TS:   a && b || !c
来源：http://uzl.andypj.xyz

Java: a && b || !c
来源：http://gej.yongpay.top

Go:   a && b || !c
来源：http://crm.jiagoushi.top

Ruby: a && b || !c
来源：http://abt.feifeiyinyue.top

C#:   a && b || !c
来源：http://yvn.pengpengdd.cyou

[B16] 卫语句：不满足条件提前返回
来源：http://wwv.yuanzhike.top

Py:   if not data: return
来源：http://tke.zhoulong.xyz

PHP:  if (!$data) { return; }
来源：http://cxi.shanyushiyangtech.top

JS:   if (!data) return;
来源：http://pwp.nanxuanxn.top

TS:   if (!data) return;
来源：http://psk.nanxinkj.top

Java: if (data == null) return;
来源：http://nsa.ybcxt.top

Go:   if data == nil { return }
来源：http://fjb.aizwys.cn

Ruby: return if data.nil?
来源：http://wrg.redwolf501.top

C#:   if (data == null) return;
来源：http://kxb.aibaodan.cn

================================================================================
来源：http://wlx.shanyushiyangkeji.top

C. 函数与作用域
来源：http://cyp.meibo888.top

================================================================================
来源：http://giz.kuanghao11.cn

[C01] 定义函数
来源：http://riy.zhiwuduotai.top

Py:   def add(a, b): return a + b
来源：http://him.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uxt.c1oappe.top

JS:   function add(a, b) { return a + b; }
来源：http://ray.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://shg.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mzg.fengsongda.top

Go:   func add(a, b int) int { return a + b }
来源：http://wnw.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://rlh.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pgd.yangfankeji.com

[C02] 默认参数
来源：http://tuj.vehdjk.com

Py:   def greet(name="World"): return name
来源：http://thp.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xgt.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://iel.sysykeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wvc.gaohongyu789.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fqm.cucudq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hts.iojbl.cn

Ruby: def greet(name = "World") = name
来源：http://ket.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://arf.zhixingplan.top

[C03] 可变参数
来源：http://bcx.gaohongyu789.top

Py:   def total(*args): return sum(args)
来源：http://okn.ydjk.org.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pmk.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tzb.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xoj.sjlbkw.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zql.shuidangran.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rtu.tanke756.top


<!-- 参考信息 -->